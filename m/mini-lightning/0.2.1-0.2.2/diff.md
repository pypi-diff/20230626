# Comparing `tmp/mini-lightning-0.2.1.tar.gz` & `tmp/mini-lightning-0.2.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mini-lightning-0.2.1.tar", last modified: Sun May 14 15:34:58 2023, max compression
+gzip compressed data, was "mini-lightning-0.2.2.tar", last modified: Mon Jun 26 16:59:05 2023, max compression
```

## Comparing `mini-lightning-0.2.1.tar` & `mini-lightning-0.2.2.tar`

### file list

```diff
@@ -1,26 +1,27 @@
-drwxrwxr-x   0 jintao    (1000) jintao    (1000)        0 2023-05-14 15:34:58.387335 mini-lightning-0.2.1/
--rw-rw-r--   0 jintao    (1000) jintao    (1000)     1063 2022-09-17 07:21:40.000000 mini-lightning-0.2.1/LICENSE
--rw-rw-r--   0 jintao    (1000) jintao    (1000)       24 2022-09-07 13:36:40.000000 mini-lightning-0.2.1/MANIFEST.in
--rw-rw-r--   0 jintao    (1000) jintao    (1000)     4669 2023-05-14 15:34:58.387335 mini-lightning-0.2.1/PKG-INFO
--rw-rw-r--   0 jintao    (1000) jintao    (1000)     3841 2023-03-26 15:35:20.000000 mini-lightning-0.2.1/README.md
-drwxrwxr-x   0 jintao    (1000) jintao    (1000)        0 2023-05-14 15:34:58.387335 mini-lightning-0.2.1/mini_lightning/
--rw-rw-r--   0 jintao    (1000) jintao    (1000)      106 2023-02-24 13:16:36.000000 mini-lightning-0.2.1/mini_lightning/__init__.py
--rw-rw-r--   0 jintao    (1000) jintao    (1000)    46084 2023-05-14 15:32:31.000000 mini-lightning-0.2.1/mini_lightning/_mini_lightning.py
--rw-rw-r--   0 jintao    (1000) jintao    (1000)     1401 2023-05-04 16:37:55.000000 mini-lightning-0.2.1/mini_lightning/_types.py
--rw-rw-r--   0 jintao    (1000) jintao    (1000)    11778 2023-05-10 13:09:19.000000 mini-lightning-0.2.1/mini_lightning/_utils.py
--rw-rw-r--   0 jintao    (1000) jintao    (1000)     1210 2023-03-19 07:36:09.000000 mini-lightning-0.2.1/mini_lightning/_visualize.py
--rw-rw-r--   0 jintao    (1000) jintao    (1000)     3326 2023-04-02 05:49:42.000000 mini-lightning-0.2.1/mini_lightning/_warmup_lrs.py
-drwxrwxr-x   0 jintao    (1000) jintao    (1000)        0 2023-05-14 15:34:58.387335 mini-lightning-0.2.1/mini_lightning.egg-info/
--rw-rw-r--   0 jintao    (1000) jintao    (1000)     4669 2023-05-14 15:34:58.000000 mini-lightning-0.2.1/mini_lightning.egg-info/PKG-INFO
--rw-rw-r--   0 jintao    (1000) jintao    (1000)      505 2023-05-14 15:34:58.000000 mini-lightning-0.2.1/mini_lightning.egg-info/SOURCES.txt
--rw-rw-r--   0 jintao    (1000) jintao    (1000)        1 2023-05-14 15:34:58.000000 mini-lightning-0.2.1/mini_lightning.egg-info/dependency_links.txt
--rw-rw-r--   0 jintao    (1000) jintao    (1000)      100 2023-05-14 15:34:58.000000 mini-lightning-0.2.1/mini_lightning.egg-info/requires.txt
--rw-rw-r--   0 jintao    (1000) jintao    (1000)       15 2023-05-14 15:34:58.000000 mini-lightning-0.2.1/mini_lightning.egg-info/top_level.txt
--rw-rw-r--   0 jintao    (1000) jintao    (1000)       99 2023-05-09 15:54:03.000000 mini-lightning-0.2.1/requirements.txt
--rw-rw-r--   0 jintao    (1000) jintao    (1000)       38 2023-05-14 15:34:58.387335 mini-lightning-0.2.1/setup.cfg
--rw-rw-r--   0 jintao    (1000) jintao    (1000)     1259 2023-05-04 16:40:28.000000 mini-lightning-0.2.1/setup.py
-drwxrwxr-x   0 jintao    (1000) jintao    (1000)        0 2023-05-14 15:34:58.387335 mini-lightning-0.2.1/tests/
--rw-rw-r--   0 jintao    (1000) jintao    (1000)     2181 2023-03-16 17:26:26.000000 mini-lightning-0.2.1/tests/test_lrs.py
--rw-rw-r--   0 jintao    (1000) jintao    (1000)      184 2023-03-09 12:27:51.000000 mini-lightning-0.2.1/tests/test_mini_lightning.py
--rw-rw-r--   0 jintao    (1000) jintao    (1000)     2219 2023-03-09 12:28:08.000000 mini-lightning-0.2.1/tests/test_utils.py
--rw-rw-r--   0 jintao    (1000) jintao    (1000)      977 2023-03-09 12:28:17.000000 mini-lightning-0.2.1/tests/test_visualize.py
+drwxrwxr-x   0 jintao    (1000) jintao    (1000)        0 2023-06-26 16:59:05.886924 mini-lightning-0.2.2/
+-rw-rw-r--   0 jintao    (1000) jintao    (1000)     1063 2022-09-17 07:21:40.000000 mini-lightning-0.2.2/LICENSE
+-rw-rw-r--   0 jintao    (1000) jintao    (1000)       24 2022-09-07 13:36:40.000000 mini-lightning-0.2.2/MANIFEST.in
+-rw-rw-r--   0 jintao    (1000) jintao    (1000)     5183 2023-06-26 16:59:05.886924 mini-lightning-0.2.2/PKG-INFO
+-rw-rw-r--   0 jintao    (1000) jintao    (1000)     4355 2023-06-26 16:57:44.000000 mini-lightning-0.2.2/README.md
+drwxrwxr-x   0 jintao    (1000) jintao    (1000)        0 2023-06-26 16:59:05.882924 mini-lightning-0.2.2/mini_lightning/
+-rw-rw-r--   0 jintao    (1000) jintao    (1000)      106 2023-02-24 13:16:36.000000 mini-lightning-0.2.2/mini_lightning/__init__.py
+-rw-rw-r--   0 jintao    (1000) jintao    (1000)    47600 2023-06-26 16:57:44.000000 mini-lightning-0.2.2/mini_lightning/_mini_lightning.py
+-rw-rw-r--   0 jintao    (1000) jintao    (1000)     1436 2023-06-23 07:58:45.000000 mini-lightning-0.2.2/mini_lightning/_types.py
+-rw-rw-r--   0 jintao    (1000) jintao    (1000)    14305 2023-06-26 15:10:13.000000 mini-lightning-0.2.2/mini_lightning/_utils.py
+-rw-rw-r--   0 jintao    (1000) jintao    (1000)     1210 2023-03-19 07:36:09.000000 mini-lightning-0.2.2/mini_lightning/_visualize.py
+-rw-rw-r--   0 jintao    (1000) jintao    (1000)     2476 2023-06-23 07:58:45.000000 mini-lightning-0.2.2/mini_lightning/_warmup_lrs.py
+drwxrwxr-x   0 jintao    (1000) jintao    (1000)        0 2023-06-26 16:59:05.886924 mini-lightning-0.2.2/mini_lightning.egg-info/
+-rw-rw-r--   0 jintao    (1000) jintao    (1000)     5183 2023-06-26 16:59:05.000000 mini-lightning-0.2.2/mini_lightning.egg-info/PKG-INFO
+-rw-rw-r--   0 jintao    (1000) jintao    (1000)      533 2023-06-26 16:59:05.000000 mini-lightning-0.2.2/mini_lightning.egg-info/SOURCES.txt
+-rw-rw-r--   0 jintao    (1000) jintao    (1000)        1 2023-06-26 16:59:05.000000 mini-lightning-0.2.2/mini_lightning.egg-info/dependency_links.txt
+-rw-rw-r--   0 jintao    (1000) jintao    (1000)      100 2023-06-26 16:59:05.000000 mini-lightning-0.2.2/mini_lightning.egg-info/requires.txt
+-rw-rw-r--   0 jintao    (1000) jintao    (1000)       15 2023-06-26 16:59:05.000000 mini-lightning-0.2.2/mini_lightning.egg-info/top_level.txt
+-rw-rw-r--   0 jintao    (1000) jintao    (1000)       99 2023-05-09 15:54:03.000000 mini-lightning-0.2.2/requirements.txt
+-rw-rw-r--   0 jintao    (1000) jintao    (1000)       38 2023-06-26 16:59:05.886924 mini-lightning-0.2.2/setup.cfg
+-rw-rw-r--   0 jintao    (1000) jintao    (1000)     1259 2023-05-24 12:58:21.000000 mini-lightning-0.2.2/setup.py
+drwxrwxr-x   0 jintao    (1000) jintao    (1000)        0 2023-06-26 16:59:05.886924 mini-lightning-0.2.2/tests/
+-rw-rw-r--   0 jintao    (1000) jintao    (1000)      184 2023-03-09 12:27:51.000000 mini-lightning-0.2.2/tests/test_mini_lightning.py
+-rw-rw-r--   0 jintao    (1000) jintao    (1000)      524 2023-06-07 08:59:17.000000 mini-lightning-0.2.2/tests/test_select_device.py
+-rw-rw-r--   0 jintao    (1000) jintao    (1000)      535 2023-06-26 15:10:13.000000 mini-lightning-0.2.2/tests/test_url.py
+-rw-rw-r--   0 jintao    (1000) jintao    (1000)     2669 2023-06-26 15:10:13.000000 mini-lightning-0.2.2/tests/test_utils.py
+-rw-rw-r--   0 jintao    (1000) jintao    (1000)      977 2023-03-09 12:28:17.000000 mini-lightning-0.2.2/tests/test_visualize.py
```

### Comparing `mini-lightning-0.2.1/LICENSE` & `mini-lightning-0.2.2/LICENSE`

 * *Files identical despite different names*

### Comparing `mini-lightning-0.2.1/PKG-INFO` & `mini-lightning-0.2.2/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mini-lightning
-Version: 0.2.1
+Version: 0.2.2
 Summary: Mini-Lightning is a lightweight machine learning training library, which is a mini version of Pytorch-Lightning with only 1k lines of code. It has the advantages of faster, more concise and more flexible.
 Home-page: https://github.com/ustcml/mini-lightning/
 Author: Jintao Huang
 Author-email: huangjintao@mail.ustc.edu.cn
 License: MIT
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
@@ -23,15 +23,15 @@
 [![PyPI Status](https://badge.fury.io/py/mini-lightning.svg)](https://pypi.org/project/mini-lightning/)
 [![License](https://img.shields.io/badge/License-MIT-yellowgreen.svg)](https://github.com/ustcml/mini-lightning/blob/main/LICENSE)
 [![Downloads](https://pepy.tech/badge/mini-lightning)](https://pepy.tech/project/mini-lightning)
 
 
 ## Introduction
 1. [Mini-Lightning](https://github.com/ustcml/mini-lightning/) is a **lightweight** machine learning training library, which is a mini version of [Pytorch-Lightning](https://www.pytorchlightning.ai/) with only **1k lines of code**. It has the advantages of **faster, more concise and more flexible**.
-2. **Existing features**: support for DDP(multi-node and multi-gpu), Sync-BN, DP, AMP, gradient accumulation, warmup and lr_scheduler, grad clip, tensorboard, model and result saving, beautiful console log, torchmetrics, etc.
+2. **Existing features**: support for DDP(multi-node and multi-gpu), Sync-BN, DP, MP(model parallelism), AMP, gradient accumulation, warmup and lr_scheduler, grad clip, tensorboard, huggingface, peft, LLM, torchmetrics, model and result saving, beautiful console log, etc.
 3. Only the **minimal interfaces** are exposed, keeping the features of **simplicity, easy to read, use and extend**.
 4. **examples** can be found in `examples/`
 5. If you have any problems or bug finding, please **raise issue**, Thank you.
 
 
 ## Installation
 1. Create a virtual environment and install Python (>= 3.8)
@@ -40,73 +40,82 @@
 ```bash
 # from pypi
 pip install mini-lightning -U
 
 # Or download the files from the repository to local,
 # and go to the folder where setup.py is located, and run the following command
 # (Recommended) You can enjoy the latest features and functions (including bug fixes)
-pip install .
+pip install -e .  # -e: editable mode
 ```
 
 
 ## Examples
 1. First, you need to install the Mini-Lightning
 2. Run the following examples
 
 ```bash
 ### test environment
 python examples/test_env.py
 
-### cv.py
+### cv
 pip install "torchvision>=0.13"
 python examples/cv.py
-# Using DP (not recommended, please use DDP)
+# cv+dp (not recommended, please use DDP)
 python examples/cv.py  # setting device_ids=[0, 1]
 
-### nlp.py
-pip install "transformers>=4.25" "datasets>=2.7"
-python examples/nlp.py
+### nlp: bert gpt
+pip install "transformers>=4.25" "datasets>=2.7" "peft>=0.3"
+python examples/nlp_bert_mlm.py
+python examples/nlp_bert_seq_cls.py
+python examples/nlp_gpt_lm.py
+python examples/nlp_gpt_seq_cls.py
+# sft
+python examples/nlp_gpt_zh_sft_adapter.py
+python examples/nlp_gpt_zh_sft_lora.py
+# llm (model parallelism)
+#   Ref: https://modelscope.cn/models/baichuan-inc/baichuan-7B/summary
+python examples/nlp_baichuan_sft_lora.py
+#   Ref: https://modelscope.cn/models/ZhipuAI/chatglm2-6b/summary
+python examples/nlp_chatglm2_sft_lora.py
 
-### dqn.py
+### dqn
 pip install "gym>=0.26.2" "pygame>=2.1.2"
 python examples/dqn.py
 
-### gan.py
+### gan
 pip install "torchvision>=0.13"
 python examples/gan.py
 
-### cl.py  (contrastive_learning)
+### contrastive learning
 pip install "torchvision>=0.13" "scikit-learn>=1.2"
 python examples/cl.py
-
-### cl_ddp.py
+# cl+ddp
 torchrun --nproc_per_node 2 examples/cl_ddp.py --device_ids 0 1
 
-### gnn.py gnn2.py
+### gnn
 # download torch_geometric
 #   Ref: https://pytorch-geometric.readthedocs.io/en/latest/notes/installation.html
-python examples/gnn.py
-python examples/gnn2.py
-python examples/gnn3.py
+python examples/gnn_node.py
+python examples/gnn_edge.py
+python examples/gnn_graph.py
 
-### ae.py
+### ae
 pip install "torchvision>=0.13" "scikit-learn>=1.2"
 python examples/ae.py
 
-### vae.py
+### vae
 pip install "torchvision>=0.13"
 python examples/vae.py
 
-### meta_learning.py
+### meta learning
 pip install "torchvision>=0.13"
 python examples/meta_learning.py
 
 
 ########## ddp
-### cv_ddp.py; cv_ddp_spawn.py
 # torchrun (Recommended)
 #   Ref: https://pytorch.org/docs/stable/elastic/run.html
 # spawn
 #   Ref: https://pytorch.org/docs/stable/notes/ddp.html
 ## single-node, multi-gpu
 torchrun --nproc_per_node 2 examples/cv_ddp.py --device_ids 0 1
 python cv_ddp_spawn.py  # setting device_ids=[0, 1]
@@ -117,7 +126,9 @@
 torchrun --nnodes 2 --node_rank 1 --master_addr xxx.xxx.xxx.xxx --nproc_per_node 4 examples/cv_ddp.py --device_ids 0 1 2 3
 ```
 
 
 ## TODO
 1. Automatic parameter adjustment
 2. Examples: Audio, Meta-learning, Diffusion, Auto-regressive, Reinforcement Learning
+3. Support multi-gpu test
+4. Output .log file
```

### Comparing `mini-lightning-0.2.1/README.md` & `mini-lightning-0.2.2/README.md`

 * *Files 10% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 [![PyPI Status](https://badge.fury.io/py/mini-lightning.svg)](https://pypi.org/project/mini-lightning/)
 [![License](https://img.shields.io/badge/License-MIT-yellowgreen.svg)](https://github.com/ustcml/mini-lightning/blob/main/LICENSE)
 [![Downloads](https://pepy.tech/badge/mini-lightning)](https://pepy.tech/project/mini-lightning)
 
 
 ## Introduction
 1. [Mini-Lightning](https://github.com/ustcml/mini-lightning/) is a **lightweight** machine learning training library, which is a mini version of [Pytorch-Lightning](https://www.pytorchlightning.ai/) with only **1k lines of code**. It has the advantages of **faster, more concise and more flexible**.
-2. **Existing features**: support for DDP(multi-node and multi-gpu), Sync-BN, DP, AMP, gradient accumulation, warmup and lr_scheduler, grad clip, tensorboard, model and result saving, beautiful console log, torchmetrics, etc.
+2. **Existing features**: support for DDP(multi-node and multi-gpu), Sync-BN, DP, MP(model parallelism), AMP, gradient accumulation, warmup and lr_scheduler, grad clip, tensorboard, huggingface, peft, LLM, torchmetrics, model and result saving, beautiful console log, etc.
 3. Only the **minimal interfaces** are exposed, keeping the features of **simplicity, easy to read, use and extend**.
 4. **examples** can be found in `examples/`
 5. If you have any problems or bug finding, please **raise issue**, Thank you.
 
 
 ## Installation
 1. Create a virtual environment and install Python (>= 3.8)
@@ -21,73 +21,82 @@
 ```bash
 # from pypi
 pip install mini-lightning -U
 
 # Or download the files from the repository to local,
 # and go to the folder where setup.py is located, and run the following command
 # (Recommended) You can enjoy the latest features and functions (including bug fixes)
-pip install .
+pip install -e .  # -e: editable mode
 ```
 
 
 ## Examples
 1. First, you need to install the Mini-Lightning
 2. Run the following examples
 
 ```bash
 ### test environment
 python examples/test_env.py
 
-### cv.py
+### cv
 pip install "torchvision>=0.13"
 python examples/cv.py
-# Using DP (not recommended, please use DDP)
+# cv+dp (not recommended, please use DDP)
 python examples/cv.py  # setting device_ids=[0, 1]
 
-### nlp.py
-pip install "transformers>=4.25" "datasets>=2.7"
-python examples/nlp.py
+### nlp: bert gpt
+pip install "transformers>=4.25" "datasets>=2.7" "peft>=0.3"
+python examples/nlp_bert_mlm.py
+python examples/nlp_bert_seq_cls.py
+python examples/nlp_gpt_lm.py
+python examples/nlp_gpt_seq_cls.py
+# sft
+python examples/nlp_gpt_zh_sft_adapter.py
+python examples/nlp_gpt_zh_sft_lora.py
+# llm (model parallelism)
+#   Ref: https://modelscope.cn/models/baichuan-inc/baichuan-7B/summary
+python examples/nlp_baichuan_sft_lora.py
+#   Ref: https://modelscope.cn/models/ZhipuAI/chatglm2-6b/summary
+python examples/nlp_chatglm2_sft_lora.py
 
-### dqn.py
+### dqn
 pip install "gym>=0.26.2" "pygame>=2.1.2"
 python examples/dqn.py
 
-### gan.py
+### gan
 pip install "torchvision>=0.13"
 python examples/gan.py
 
-### cl.py  (contrastive_learning)
+### contrastive learning
 pip install "torchvision>=0.13" "scikit-learn>=1.2"
 python examples/cl.py
-
-### cl_ddp.py
+# cl+ddp
 torchrun --nproc_per_node 2 examples/cl_ddp.py --device_ids 0 1
 
-### gnn.py gnn2.py
+### gnn
 # download torch_geometric
 #   Ref: https://pytorch-geometric.readthedocs.io/en/latest/notes/installation.html
-python examples/gnn.py
-python examples/gnn2.py
-python examples/gnn3.py
+python examples/gnn_node.py
+python examples/gnn_edge.py
+python examples/gnn_graph.py
 
-### ae.py
+### ae
 pip install "torchvision>=0.13" "scikit-learn>=1.2"
 python examples/ae.py
 
-### vae.py
+### vae
 pip install "torchvision>=0.13"
 python examples/vae.py
 
-### meta_learning.py
+### meta learning
 pip install "torchvision>=0.13"
 python examples/meta_learning.py
 
 
 ########## ddp
-### cv_ddp.py; cv_ddp_spawn.py
 # torchrun (Recommended)
 #   Ref: https://pytorch.org/docs/stable/elastic/run.html
 # spawn
 #   Ref: https://pytorch.org/docs/stable/notes/ddp.html
 ## single-node, multi-gpu
 torchrun --nproc_per_node 2 examples/cv_ddp.py --device_ids 0 1
 python cv_ddp_spawn.py  # setting device_ids=[0, 1]
@@ -98,7 +107,9 @@
 torchrun --nnodes 2 --node_rank 1 --master_addr xxx.xxx.xxx.xxx --nproc_per_node 4 examples/cv_ddp.py --device_ids 0 1 2 3
 ```
 
 
 ## TODO
 1. Automatic parameter adjustment
 2. Examples: Audio, Meta-learning, Diffusion, Auto-regressive, Reinforcement Learning
+3. Support multi-gpu test
+4. Output .log file
```

### Comparing `mini-lightning-0.2.1/mini_lightning/_mini_lightning.py` & `mini-lightning-0.2.2/mini_lightning/_mini_lightning.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,106 +1,106 @@
 # Author: Jintao Huang
 # Email: huangjintao@mail.ustc.edu.cn
 # Date:
 
 from ._types import *
+from ._warmup_lrs import _lr_scheduler_rerun
 from ._utils import (
     en_parallel, de_parallel, get_dist_setting, select_device,
     logger, write_to_yaml, write_to_csv, read_from_yaml,
     print_model_info, load_ckpt, save_ckpt, ModelCheckpoint, ResumeFromCkpt
 )
 
 
-# Note: global_epoch, batch_idx start from 0. 
+# Note: global_epoch, batch_idx start from 0.
 #   global_step starts from 1.
 __all__ = ["LModule", "LDataModule", "Trainer"]
 #
 
 
 class LModule:
     def __init__(
         self,
         optimizers: List[Optimizer],
+        lr_schedulers: List[LRScheduler],
         metrics: Dict[str, Metric],
         hparams: Any = None
     ) -> None:
         """
         optimizers: Use List, for supporting GAN
         hparams: Hyperparameters to be saved
             object or Dict[str, Any] or None
         """
         # _models: for trainer_init(device, ddp), _epoch_start(train, eval); print_model_info; save_ckpt
         self._models: List[str] = []
         self.optimizers = optimizers
+        self.lr_schedulers = lr_schedulers
         self.metrics = metrics
         self.hparams = hparams
         self.trainer: Optional["Trainer"] = None
 
     @property
     def global_step(self) -> int:
         # global_step starts from 1
+        # optimizer_step
         assert self.trainer is not None
         return self.trainer.global_step
 
     @property
     def global_epoch(self) -> int:
         # global_epoch starts from 0
         assert self.trainer is not None
         return self.trainer.global_epoch
 
     @property
-    def global_optimizer_step(self) -> int:
-        assert self.trainer is not None
-        return self.trainer.global_optimizer_step
-
-    @property
     def device(self) -> Optional[Device]:
         assert self.trainer is not None
         return self.trainer.device
 
     #
-    def log(self, k: str, v: Union[Tensor, float], *, prog_bar_mean=True) -> None:
+    def log(self, k: str, v: Union[Tensor, float], *, prog_bar_mean: bool = True) -> None:
         """
         prog_bar_mean: mean of values in epoch is showed in prog_bar. (e.g. `loss`, `acc`: True. `lr`: False)
             note: `lr`, `global_step` logs automatically, no manual log is required.
         """
         assert self.trainer is not None
         if isinstance(v, Tensor):
             v = v.item()
         self.trainer._new_mes[k] = v
         self.trainer._prog_bar_mean[k] = prog_bar_mean
 
-    def log_dict(self, _dict: Dict[str, Union[Tensor, float]], *, prog_bar_mean=True) -> None:
+    def log_dict(self, _dict: Dict[str, Union[Tensor, float]], *, prog_bar_mean: bool = True) -> None:
         for k, v in _dict.items():
             self.log(k, v, prog_bar_mean=prog_bar_mean)
 
     def __call__(self, *args, **kwargs) -> Any:
         return self.forward(*args, **kwargs)
 
     #
     def trainer_init(self, trainer: "Trainer") -> None:
         self.trainer = trainer
         device = trainer.device
         #
         for s in self._models:
             model: Module = getattr(self, s)
-            model.to(device)
+            if next(model.parameters()).device.type == "cpu":
+                model.to(device)
             model = en_parallel(model, trainer.parallel_mode, trainer.sync_bn)
             setattr(self, s, model)
-        # 
+        #
         for o in self.optimizers:
             o.load_state_dict(o.state_dict())  # to device
-        # 
+        #
         for metric in self.metrics.values():
             metric.to(device)
 
     @classmethod
     def batch_to_device(cls, batch: Any, device: Device) -> Any:
         if callable(getattr(batch, "to", None)):
-            # Ref: https://github.com/Lightning-AI/lightning/blob/master/src/lightning_lite/utilities/apply_func.py
+            # Ref: https://github.com/Lightning-AI/lightning/blob/master/src/lightning/fabric/utilities/apply_func.py#L92
             #   same as pytorch-lightning
             kwargs = {}
             if isinstance(batch, Tensor) and device not in (Device("cpu"), "cpu"):
                 kwargs["non_blocking"] = True
             return batch.to(device=device, **kwargs)
         #
         if isinstance(batch, Mapping):
@@ -140,15 +140,15 @@
     def training_epoch_start(self) -> None:
         self._epoch_start("train")
 
     def validation_epoch_start(self) -> None:
         self._epoch_start("val_test")
 
     def test_epoch_start(self) -> None:
-        self._epoch_start("val_test")
+        self.validation_epoch_start()
 
     #
     def toggle_optimizer(self, opt_idx: int) -> None:
         """
         Ref: https://pytorch-lightning.readthedocs.io/en/latest/common/lightning_module.html#toggle-optimizer
         """
         optimizer_requires_grad: Dict[Parameter, bool] = {}
@@ -315,89 +315,110 @@
 
 
 class Trainer:
     def __init__(
         self,
         lmodel: LModule,
         device_ids: List[int],
-        max_epochs: int,
+        max_epochs: Optional[int],  # None for only test
         runs_dir: str,
         model_checkpoint: Optional[ModelCheckpoint] = None,
         n_accumulate_grad: Union[int, Dict[int, int]] = 1,
         amp: bool = False,
         gradient_clip_norm: Optional[float] = None,
         sync_bn: bool = False,
         replace_sampler_ddp: bool = True,
         resume_from_ckpt: Union[str, ResumeFromCkpt, None] = None,
         #
-        tb_every_n_steps: int = 10,
+        use_dp: bool = False,  # This parameter is valid only when len(device_ids) is >1
+        tb_every_n_steps: int = 5,
         prog_bar_n_steps: int = 1,
         deterministic:  Optional[bool] = None,
         benchmark: Optional[bool] = None,
         verbose: bool = True,
     ) -> None:
         """
         About ddp mode: you can see example in `examples/cv_ddp.py`
             note: DDP: multi-gpu/node will be used for training, while single gpu will be used for validation or test
                 to avoid the metrics error caused by the inability to evenly split the last batch
                 Ref: https://torchmetrics.readthedocs.io/en/stable/pages/overview.html#metrics-in-distributed-data-parallel-ddp-mode
             note: DDP is recommended instead of DP.
                 DDP uses multiple processes and DP uses multiple threads. DDP is faster than DP.
                 In addition, DDP supports sync-BN.
         #
-        device_ids: if len(device_ids) > 1, use DP. (by setting the `CUDA_VISIBLE_DEVICES` environment variable to select device)
-            e.g. []: stands for "cpu "; [0]; [0, 1, 2]
+        device_ids: if len(device_ids) > 1, use DP(if use_dp=True)/MP. 
+            e.g. []: stands for "cpu"; [0]; [0, 1, 2]
             note: DP: batch_size is split to each GPU. Make sure: batch_size % n_gpus == 0.
                 DDP: total batch_size = batch_size * world_size. (different from DP)
             note: DP, DDP, sync_bn will modify lmodel.model (en_parallel). You need to de_parallel, de_sync_batchnorm manually if you want to get original model.
-        n_accumulate_grad: Accumulates gradient every n batch (Use mean accumulation instead of sum)
-            Ref: https://pytorch-lightning.readthedocs.io/en/latest/_modules/pytorch_lightning/loops/optimization/optimizer_loop.html (Search: self.trainer.accumulate_grad_batches)
+        n_accumulate_grad: Accumulates gradient every n batch. `batch_idx %`
+            Ref: https://lightning.ai/docs/pytorch/stable/common/optimization.html#gradient-accumulation
             if n_accumulate_grad is Dict[int, int]: e.g. {5:2, 20:4} or {0:1, 5:2, 20:4}.
                 Indicates 1 for 0-4 epoch, 2 for 5-19, and 4 after 20 epoch.
                 This can accelerate the training speed in the initial stage, and get nice convergence performance in the end.
                 (like bigger batch_size if you don't use bn); with big batch_size, you can increase the learning rate appropriately.
-            note: It will changes the frequency of optimizer_step() calls.
-                So adjust the parameters of the lr_scheduler called in optimizer_step() (e.g. warmup, T_max, etc.). you can use ml.get_T_max() to get T_max
-            note: the unupdated grad of the last batch will be updated before validation. 
-                Same behavior as PyTorch Lightning. `batch_idx %`
+            note: the unupdated grad of the last batch will be updated before validation. Same behavior as PyTorch Lightning. 
         amp: Whether to use mixed precision training.
             Ref: https://pytorch.org/docs/stable/notes/amp_examples.html
             Effects: Speed up training and reduce memory consumption. Slightly (or not) decrease performance.
-            note: Recommended for use in large models. Small models do not speed up training.
-            note: some environments may not support AMP
-        gradient_clip_norm: gradient clipping (norm) to prevents gradient explosion and log `grad_norm` before clipping if verbose=True. It's usually set to 5, 10, 20.
+            note: Recommended for use in large models(e.g. GPT, BERT). Small models do not speed up training. 
+        gradient_clip_norm: gradient clipping (norm) to prevents gradient explosion and log `grad_norm` before clipping if verbose=True. 
+            It's usually set to 5, 10, 20.
             note: inf and nan check is added if gradient_clip_norm is not None. This can improve the stability of training.
                 If inf or nan is found, this update will be skipped. (If amp=True, inf check is handled by amp)
         sync_bn: (valid only in DDP mode)
             This generally improves training accuracy and stability, but slightly slows down training speed.
-        replace_sampler_ddp: (valid only in DDP mode) whether to use DistributedSampler (train_dataloader only) in DDP mode.
+        replace_sampler_ddp: (valid only in DDP mode) whether to use DistributedSampler in DDP mode.
             replace_sampler_ddp=False: each gpu will use the complete dataset.
             replace_sampler_ddp=True: It will slice the dataset into world_size chunks and distribute them to each gpu.
             note: Replace train_dataloader only. Because DDP uses a single gpu for val/test.
-        resume_from_ckpt: only load model_state_dict. `*.ckpt`
+        resume_from_ckpt: e.g. `*.ckpt`
             If you want to resume from ckpt. please see examples in `examples/test_env.py`
         *
-        tb_every_n_steps: Frequency of writing information to the tensorboard(sampling per n steps, not mean; all gpus). `global_step % `
+        tb_every_n_steps: Frequency of writing information to the tensorboard. `global_step % `
         prog_bar_n_steps: updating Frequency of progress bar. `batch_idx % `. (rank=0)
             note: torchmetrics is recommended for metrics calculation.
                 if you use `self.log` in training, errors will occur when the length of the last batch is not equal to batch_size.
-                    and it will just log rank=0 if in ddp mode.
-                please don't use `self.log` in validation
-            note: train: scalar of inf, nan will be skipped, val/test: scalar of inf, nan will be recorded.
+                    and it will just log rank=0 in ddp mode. (for faster)
+                please don't use `self.log` in validation. (please use metrics["xxx"].update, for more precision)
+            note: train: scalar of inf, nan will be skipped; val/test: scalar of inf, nan will be recorded.
         deterministic:
             deterministic=None: not modify
-        benchmark: same as Pytorch Lightning behavior.
+        benchmark: 
             benchmark=True, can speed up training. (Pytorch defaults to False)
                 Ref: https://pytorch.org/docs/stable/backends.html#torch.backends.cudnn.torch.backends.cudnn.benchmark
-            benchmark=None: if cudnn.deterministic=False, benchmark=True. else benchmark=False.
-        verbose: records global_step, lr, (grad_norm if gradient_clip_norm=True) automatically. (tensorboard will always record)
+            benchmark=None: if cudnn.deterministic=False, benchmark=True. else benchmark=False. 
+                same as Pytorch Lightning behavior.
+        verbose: records global_step, lr, (grad_norm if gradient_clip_norm=True) automatically. 
+            (Only the prog bar is affected, tensorboard will always record)
             verbose=True: log in prog_bar.
             verbose=False: not log in prog_bar, making the prog_bar cleaner
         """
         self.rank, self.local_rank, self.world_size = get_dist_setting()
+        self.version = None
+        if self.rank in {-1, 0}:
+            runs_dir = os.path.abspath(runs_dir)
+            self.version = self._get_version(runs_dir)
+            time = dt.datetime.now().strftime("%Y%m%d-%H%M%S.%f")  # window not support `:`
+            runs_dir = os.path.join(runs_dir, f"v{self.version}-{time}")
+            #
+            self.runs_dir = runs_dir
+            self.ckpt_dir = os.path.join(runs_dir, "checkpoints")
+            self.tb_dir = os.path.join(runs_dir, "runs")  # tensorboard
+            self.hparams_path = os.path.join(runs_dir, "hparams.yaml")
+            self.result_yaml_path = os.path.join(runs_dir, "result.yaml")
+            self.result_csv_path = os.path.join(runs_dir, "result.csv")
+            self.log_path = os.path.join(runs_dir, "output.log")
+            os.makedirs(self.ckpt_dir, exist_ok=True)
+            os.makedirs(self.tb_dir, exist_ok=True)
+            #
+            self.save_hparams(lmodel.hparams)
+            logger.info(f"runs_dir: {runs_dir}")
+            self.tb_logger = SummaryWriter(self.tb_dir)
+        #
         logger.info(f"Using local_rank: {self.local_rank}, rank: {self.rank}, world_size: {self.world_size}")
         #
         self.lmodel = lmodel
         self.device_ids = device_ids
         #
         if deterministic is not None:
             torch.backends.cudnn.deterministic = deterministic
@@ -406,27 +427,29 @@
             benchmark = False
         else:
             benchmark = True if benchmark is None else benchmark
         torch.backends.cudnn.benchmark = benchmark
         logger.info(f"Setting deterministic: {deterministic}")
         logger.info(f"Setting benchmark: {benchmark}")
         #
-        self.device = select_device(device_ids)
+        device = select_device(device_ids)
         if self.rank == -1:
-            parallel_mode = "DP" if len(device_ids) > 1 else None
+            self.device = device
+            parallel_mode = "DP" if len(device_ids) > 1 and use_dp else None
         else:
             parallel_mode = "DDP"
             self.device = Device(self.local_rank)  # cover
             cuda.set_device(self.local_rank)  # set current cuda
             assert dist.is_available()
             if not dist.is_initialized():
                 # nccl is not available in windows
                 backend = "nccl" if dist.is_nccl_available() else "gloo"
                 logger.info(f"Using backend: {backend}")
                 dist.init_process_group(backend=backend, rank=self.rank, world_size=self.world_size)
+        self.use_dp = use_dp
         self.parallel_mode: Literal["DP", "DDP", None] = parallel_mode
         self.sync_bn = sync_bn
         self.amp = amp
         logger.info(f"Using amp: {amp}")
         #
         self.max_epochs = max_epochs
         self.n_accumulate_grad = n_accumulate_grad
@@ -444,74 +467,52 @@
         self.deterministic = deterministic
         self.benchmark = benchmark
         #
         self.scaler = GradScaler(enabled=amp)
         self.best_metric: Optional[float] = None
         self.best_ckpt_path: Optional[str] = None
         self.last_ckpt_path: Optional[str] = None
-        self.global_step = 0
-        self.global_optimizer_step = 0
+        self.global_step = 0  # optim_step
+        self._last_optimize = False   # for last optimize before validation
+        self._after_optimize = False
         self.global_epoch = -1
         # for log
         self._new_mes: Dict[str, float] = {}
         self._prog_bar_mean: Dict[str, bool] = {}
         # check inf nan
         self._found_inf = False
         self._found_nan = False
         # for last_val
         self._last_val = False
         # for train epoch
         self._rec_mes_train: Dict[str, float] = {}
         self._mean_metrics_train: Dict[str, MeanMetric] = {}
-        # for last optimize before validation
-        self._last_optimize = False
+        self._tb_mean_metrics_train: Dict[str, MeanMetric] = {}
         #
-        self.version = None
-        self.model_checkpoint = model_checkpoint if model_checkpoint is not None else ModelCheckpoint()
-        if self.rank in {-1, 0}:
-            runs_dir = os.path.abspath(runs_dir)
-            self.version = self._get_version(runs_dir)
-            if platform.system().lower() == "windows":
-                time = dt.datetime.now().strftime("%Y-%m-%d_%H-%M-%S")  # window not support `:`
-                runs_dir = os.path.join(runs_dir, f"v{self.version}_{time}")
-            else:  # "linux"
-                time = dt.datetime.now().strftime("%Y:%m:%d-%H:%M:%S")
-                runs_dir = os.path.join(runs_dir, f"v{self.version}-{time}")
-            logger.info(f"runs_dir: {runs_dir}")
-            #
-            self.runs_dir = runs_dir
-            self.ckpt_dir = os.path.join(runs_dir, "checkpoints")
-            self.tb_dir = os.path.join(runs_dir, "runs")  # tensorboard
-            self.hparams_path = os.path.join(runs_dir, "hparams.yaml")
-            self.result_yaml_path = os.path.join(runs_dir, "result.yaml")
-            self.result_csv_path = os.path.join(runs_dir, "result.csv")
-            os.makedirs(self.ckpt_dir, exist_ok=True)
-            os.makedirs(self.tb_dir, exist_ok=True)
-            #
-            self.tb_logger = SummaryWriter(self.tb_dir)
-            hparams = lmodel.hparams
-            self.save_hparams(hparams)
+        self._saveing_n: int = 0  # nums of saving last models (epoch/step mode)
         #
+        self.model_checkpoint = model_checkpoint if model_checkpoint is not None else ModelCheckpoint()
         self.resume_from_ckpt = resume_from_ckpt
         if resume_from_ckpt is not None:
             rfc = resume_from_ckpt
             if isinstance(rfc, str):
-                self._load_ckpt(rfc, False, False, False)
+                self._load_ckpt(rfc, False, False, False, False)
                 logger.info(f"Using ckpt: {rfc}")
             elif isinstance(rfc, ResumeFromCkpt):
                 if rfc.ckpt_path is not None:
-                    self._load_ckpt(rfc.ckpt_path, rfc.load_optimizers, rfc.load_message, False)
+                    self._load_ckpt(rfc.ckpt_path, rfc.load_optimizers, rfc.load_lr_schedulers, 
+                                    rfc.load_message, False)
                     logger.info(f"Using ckpt: {rfc.ckpt_path}, resume_from_ckpt: {rfc}")
             else:
                 raise ValueError(f"resume_from_ckpt: {rfc}")
-            
+
         lmodel.trainer_init(self)
         for s in lmodel._models:
             model: Module = getattr(lmodel, s)
-            print_model_info(s, model, None)
+            print_model_info(model, s, None)
 
     @staticmethod
     def _get_version(runs_dir: str) -> int:
         if os.path.isdir(runs_dir):
             fnames = os.listdir(runs_dir)
         else:
             fnames = []
@@ -583,15 +584,15 @@
         elif mode == "last" and self.last_ckpt_path is not None:
             os.remove(self.last_ckpt_path)
 
     def _result_saving(self, mes: Dict[str, float]) -> None:
         if self.rank not in {-1, 0}:
             return
         mc = self.model_checkpoint
-        
+
         if mc.val_mode == "epoch":
             val_mode_val = self.global_epoch  # validation_mode_value
         else:
             val_mode_val = self.global_step
         #
         mode = mes["mode"]
         write_to_yaml({f"{mode}[{mc.val_mode}={val_mode_val}]": mes}, self.result_yaml_path, mode="a")
@@ -636,38 +637,64 @@
         if self.rank not in {-1, 0}:
             return
         lmodel = self.lmodel
         mc = self.model_checkpoint
         kwargs: Dict[str, Any] = {
             "global_step": self.global_step,
             "global_epoch": self.global_epoch,
-            "global_optimizer_step": self.global_optimizer_step,
             "core_metric": {
                 "name": mc.core_metric_name,
                 "higher_is_better": mc.higher_is_better,
                 "best_value": self.best_metric
             }
         }
         model_list = {s: de_parallel(getattr(lmodel, s)) for s in lmodel._models}
         optimizers = lmodel.optimizers if mc.saving_optimizers else []
-        save_ckpt(fpath, model_list, optimizers, **kwargs)
+        lr_schedulers = lmodel.lr_schedulers if mc.saving_lr_schedulers else []
+        # 
+        if mc.saving_hf_mode: 
+            models_sd = {}
+            _dir_path, _fname = os.path.split(fpath)
+            if _fname.startswith("best"):
+                save_dir = os.path.join(_dir_path, "best")
+            else:
+                save_dir = os.path.join(_dir_path, "last")
+            #
+            os.makedirs(save_dir, exist_ok=True)
+            for m in model_list.values():
+                if hasattr(m, "save_pretrained"):
+                    m.save_pretrained(save_dir)
+        else:
+            models_sd  =  {k: m.state_dict() for k, m in model_list.items()}
+        save_ckpt(fpath, models_sd, optimizers, lr_schedulers, **kwargs)
 
-    def _load_ckpt(self, fpath: str, load_optimizers: bool = False, load_mes: bool = False, strict: bool = True) -> None:
-        map_location = self.device
-        models_state_dict, optimizers_state_dict,  mes = load_ckpt(fpath, map_location)
+    def _load_ckpt(self, fpath: str, load_optimizers: bool, load_lr_schedulers: bool,
+                   load_mes: bool, strict: bool) -> None:
+        # fpath: `*.ckpt`
         lmodel = self.lmodel
+        map_location = self.device
+        models_sd, optimizers_sd_list, lr_s_sd_list, mes = load_ckpt(fpath, map_location)
+        if len(models_sd) == 0:
+            # if mc.saving_hf_mode is True: please use model.from_pretrained
+            logger.warning(f"[{fpath} load failed] len(models_sd) == 0")
+            return
         if load_optimizers:
-            for optimizer, o_sd in zip(self.lmodel.optimizers,optimizers_state_dict):
+            for optimizer, o_sd in zip(lmodel.optimizers, optimizers_sd_list):
                 optimizer.load_state_dict(o_sd)
+        if load_lr_schedulers:
+            for lr_s, lr_s_sd in zip(lmodel.lr_schedulers, lr_s_sd_list):
+                lr_s_sd = {k: v for k, v in lr_s_sd.items() if not ismethod(v)}
+                lr_s.load_state_dict(lr_s_sd)
+                _lr_scheduler_rerun(lr_s)
+        #
         if load_mes:
             self.global_step = mes["global_step"]
             self.global_epoch = mes["global_epoch"]
-            self.global_optimizer_step = mes.get("global_optimizer_step", 0)
         #
-        for k, state_dict in models_state_dict.items():
+        for k, state_dict in models_sd.items():
             model: Module = getattr(lmodel, k)
             load_sd_mes = model.load_state_dict(state_dict, strict=strict)
             if strict is False:
                 logger.info(load_sd_mes)
 
     def _model_saving(self, core_metric: Optional[float]) -> None:
         if self.rank not in {-1, 0}:
@@ -676,41 +703,43 @@
         metric_str = ""
         mc = self.model_checkpoint
         if mc.val_mode == "epoch":
             val_mode_val = self.global_epoch
         else:
             val_mode_val = self.global_step
         #
-        if core_metric is not None:
+        if mc.saving_best_model and core_metric is not None:
             assert mc.higher_is_better is not None
             tag = "+" if mc.higher_is_better else "-"
             metric_str = f"-{mc.core_metric_name}[{tag}]={core_metric:.6f}"
             if self._is_better_than(core_metric, self.best_metric, mc.higher_is_better):
                 self._remove_ckpt("best")
                 self.best_metric = core_metric
                 ckpt_fname = f"best-{mc.val_mode}={val_mode_val}{metric_str}.ckpt"
                 self.best_ckpt_path = os.path.join(self.ckpt_dir, ckpt_fname)
                 self._save_ckpt(self.best_ckpt_path)
                 logger.info((f"Best model, saving model `{ckpt_fname}`"))
         #
-        self._remove_ckpt("last")
-        ckpt_fname = f"last-{mc.val_mode}={val_mode_val}{metric_str}.ckpt"
-        self.last_ckpt_path = os.path.join(self.ckpt_dir, ckpt_fname)
-        self._save_ckpt(self.last_ckpt_path)
+        self._saveing_n += 1
+        if mc.saving_last_model_every_n and self._saveing_n % mc.saving_last_model_every_n == 0:
+            self._remove_ckpt("last")
+            ckpt_fname = f"last-{mc.val_mode}={val_mode_val}{metric_str}.ckpt"
+            self.last_ckpt_path = os.path.join(self.ckpt_dir, ckpt_fname)
+            self._save_ckpt(self.last_ckpt_path)
 
-    def _get_res_mes(self, mean_metrics: Dict[str, MeanMetric], new_mes: Dict[str, float],
+    def _get_res_mes(self, mean_metrics: Dict[str, MeanMetric], rec_mes: Dict[str, float],
                      mode: Literal["tb", "result", "prog_bar"]) -> Dict[str, float]:
         """not inplace"""
-        res = new_mes.copy()
+        res = rec_mes.copy()
+        res.update(self._metrics_compute(mean_metrics))
         if mode == "tb":
             res["global_epoch"] = self.global_epoch
-            res.pop("global_step")
+            res.pop("global_step", None)
             return res
         #
-        res.update(self._metrics_compute(mean_metrics))
         if mode == "result":
             res["global_epoch"] = self.global_epoch
             return res
         # prog_bar
         prog_bar_res = {}
         for k in res.keys():
             if not self.verbose and (k == "global_step" or k.startswith("lr") or k.startswith("grad_norm")):
@@ -749,17 +778,21 @@
         logger.info(f"Using DistributedSampler: shuffle={shuffle}")
         dataloader = DataLoader(dataloader.dataset, dataloader.batch_size, sampler=sampler,
                                 num_workers=dataloader.num_workers, pin_memory=dataloader.pin_memory,
                                 drop_last=dataloader.drop_last, collate_fn=dataloader.collate_fn)
         return dataloader
 
     def _optimize_step(self) -> None:
+        self._last_optimize = False
+        self._after_optimize = True
+        self.global_step += 1
+        #
         lmodel = self.lmodel
         scaler = self.scaler
-        self.global_optimizer_step += 1
+        lmodel.log(f"global_step", self.global_step, prog_bar_mean=False)
         for opt_idx, opt in enumerate(lmodel.optimizers):
             if self.gradient_clip_norm is not None:
                 scaler.unscale_(opt)
                 grad_norm = clip_grad_norm_(  # scalar
                     (p for pg in opt.param_groups for p in pg["params"]),
                     max_norm=self.gradient_clip_norm, error_if_nonfinite=False
                 )
@@ -812,66 +845,68 @@
         if mc.val_mode == "epoch" and (self.global_epoch + 1) % mc.val_every_n == 0:  # need val after this epoch
             _leave = True
         elif self.global_epoch + 1 == self.max_epochs:
             _leave = True
         #
         _rec_mes = self._rec_mes_train
         _mean_metrics = self._mean_metrics_train
+        _tb_mean_metrics = self._tb_mean_metrics_train
         prog_bar = tqdm(total=total,
                         desc=f"Epoch {self.global_epoch}", dynamic_ncols=True, disable=self.rank > 0, leave=_leave)  # mininterval=0.01
         batch_idx = -1  # avoid unbound
         self._prog_bar_mean.clear()
         for batch_idx, batch in enumerate(dataloader):
-            self.global_step += 1
-            self._last_val = True
+            self._after_optimize = False
+            self._last_optimize = True
+            self._last_val = True  # need last val
             self._new_mes.clear()
-            lmodel.log(f"global_step", self.global_step, prog_bar_mean=False)
             #
             batch = lmodel.batch_to_device(batch, device)
-            self._last_optimize = True
             for opt_idx in range(len(lmodel.optimizers)):
                 if len(lmodel.optimizers) > 1:
                     lmodel.toggle_optimizer(opt_idx)
                 with autocast(device_type=self.device.type, enabled=self.amp):
                     loss = lmodel.training_step(batch, opt_idx)
                 #
                 loss.div_(n_accumulate_grad)
                 self.scaler.scale(loss).backward()
                 if len(lmodel.optimizers) > 1:
                     lmodel.untoggle_optimizer(opt_idx)
             # optimize
             if (batch_idx + 1) % n_accumulate_grad == 0:
-                self._last_optimize = False
                 self._optimize_step()
             #
             self._metrics_update(_mean_metrics, self._new_mes, self._prog_bar_mean, device, True)
+            self._metrics_update(_tb_mean_metrics, self._new_mes, self._prog_bar_mean, device, True)
             _rec_mes.update(self._new_mes)
             # prog_bar
             if (batch_idx + 1) % self.prog_bar_n_steps == 0:
                 prog_bar_mes = self._get_res_mes(_mean_metrics, _rec_mes, "prog_bar")
                 if self.rank >= 0:
                     prog_bar_mes = self._reduce_mes(prog_bar_mes, device)
                     #
                 if self.rank in {-1, 0}:
+                    if "global_step" in prog_bar_mes:
+                        prog_bar_mes["global_step"] = str(int(prog_bar_mes["global_step"]))
                     prog_bar_mes["v"] = self.version
-                    prog_bar_mes["global_step"] = str(int(prog_bar_mes["global_step"]))
                 prog_bar.set_postfix(prog_bar_mes, refresh=False)  # rank > 0 disable.
                 prog_bar.update(self.prog_bar_n_steps)
             # tensorboard
-            if self.global_step % self.tb_every_n_steps == 0:
-                tb_mes = self._get_res_mes(_mean_metrics, _rec_mes, "tb")
+            if self.global_step % self.tb_every_n_steps == 0 and self._after_optimize:
+                tb_mes = self._get_res_mes(_tb_mean_metrics, _rec_mes, "tb")
+                _tb_mean_metrics.clear()
                 if self.rank >= 0:
                     tb_mes = self._reduce_mes(tb_mes, device)
                 self._tb_logger_add_scalars(tb_mes, self.global_step)
             # val
-            if mc.val_mode == "step" and self.global_step % mc.val_every_n == 0:
+            if mc.val_mode == "step" and self.global_step % mc.val_every_n == 0 and self._after_optimize:
                 res_mes = self._get_res_mes(_mean_metrics, _rec_mes, "result")
+                prog_bar.refresh()
                 if not prog_bar.disable:
                     prog_bar.fp.write("\n")
-                prog_bar.refresh()
                 self._val_and_save_after_train(val_dataloader, res_mes)
         #
         if (batch_idx + 1 - prog_bar.n) > 0:
             prog_bar.update(batch_idx + 1 - prog_bar.n)
         prog_bar.close()
         res_mes = self._get_res_mes(_mean_metrics, _rec_mes, "result")
         #
@@ -950,15 +985,17 @@
         with torch.no_grad():
             metrics = val_test_epoch_end()
         res_mes.update(metrics)
         if mc.val_mode == "epoch":
             step = self.global_epoch
         else:
             step = self.global_step
-        self._tb_logger_add_scalars(res_mes, step)
+        tb_mes = res_mes.copy()
+        tb_mes.pop("global_epoch")
+        self._tb_logger_add_scalars(tb_mes, step)
         #
         core_metric = None
         if len(metrics) > 0:
             logger.info(self._get_epoch_end_string(metrics))
             if stage == "val":
                 core_metric_name = "val_" + mc.core_metric_name
                 core_metric = metrics[core_metric_name]
@@ -967,16 +1004,15 @@
             setattr(lmodel, s, model)
         for k, b in metrics_r.items():
             lmodel.metrics[k]._to_sync = b
             lmodel.metrics[k].sync_on_compute = b
         #
         if self.rank == 0:
             dist.barrier()
-        res_mes.update({"global_epoch": self.global_epoch, "global_step": self.global_step, 
-                        "global_optimizer_step": self.global_optimizer_step})
+        res_mes.update({"global_epoch": self.global_epoch, "global_step": self.global_step})
         return core_metric, res_mes
 
     def _val_and_save_after_train(self, val_dataloader: Optional[DataLoader], train_mes: Dict[str, float]) -> None:
         if self._last_optimize:
             self._optimize_step()
         core_metric, val_mes = self._val_test(val_dataloader, "val", "  Val: ")
         val_mes.update(train_mes)
@@ -993,27 +1029,27 @@
         self.lmodel.training_epoch_start()
 
     def _test(self, dataloader: Optional[DataLoader],
               model_type: Literal["last", "best"]) -> None:
         #
         if model_type == "best":
             assert self.best_ckpt_path is not None
-            self._load_ckpt(self.best_ckpt_path, False, True, True)
+            self._load_ckpt(self.best_ckpt_path, False, False, True, True)
             title = f"Test Best(Epoch={self.global_epoch})"
         else:
             title = f"Test Last(Epoch={self.global_epoch})"
         desc = title + ": "
         #
         _, res_mes = self._val_test(dataloader, "test", desc)
         res_mes["mode"] = f"test_{model_type}"
         self._result_saving(res_mes)
         #
         if model_type == "best":
             assert self.last_ckpt_path is not None
-            self._load_ckpt(self.last_ckpt_path, False, True, True)
+            self._load_ckpt(self.last_ckpt_path, False, False, True, True)
 
     def _best_ckpt_is_last(self) -> bool:
         if self.best_ckpt_path is None or self.last_ckpt_path is None:
             return False
 
         best_ckpt_fname = os.path.basename(self.best_ckpt_path)
         m = re.match(r"best-(epoch|step)=(\d+)", best_ckpt_fname)
@@ -1032,31 +1068,32 @@
         mc = self.model_checkpoint
         if val_dataloader is not None:
             assert mc.core_metric_name is not None
             assert mc.higher_is_better is not None
         #
         self.lmodel.training_epoch_start()
         train_mes = {}
+        assert self.max_epochs is not None
         for _ in range(self.global_epoch + 1, self.max_epochs):
             self.global_epoch += 1
             train_mes = self._train_epoch(train_dataloader, val_dataloader)
             if mc.val_mode == "epoch" and (self.global_epoch + 1) % mc.val_every_n == 0:
                 self._val_and_save_after_train(val_dataloader, train_mes)
         if self._last_val:
             self._val_and_save_after_train(val_dataloader, train_mes)
         cuda.empty_cache()
 
     def test(self, dataloader: Optional[DataLoader], test_best: bool = True, test_last: bool = True) -> None:
         if test_best:
             # If last first, last will be overridden in tensorboard. So best first.
             if self.best_ckpt_path is None:
-                logger.warning("Ignore test best: self.best_ckpt_path is None")
+                logger.warning("[Ignore test best] self.best_ckpt_path is None")
                 test_best = False
             else:
                 self._test(dataloader, "best")
         #
         if test_last:  # just current model
             if self._best_ckpt_is_last() and test_best:
-                logger.info("Ignore test last: the best ckpt and the last ckpt is the same")
+                logger.info("[Ignore test last] the best ckpt and the last ckpt is the same")
             else:
                 self._test(dataloader, "last")
         cuda.empty_cache()
```

### Comparing `mini-lightning-0.2.1/mini_lightning/_types.py` & `mini-lightning-0.2.2/mini_lightning/_types.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,21 +1,24 @@
 import os
 import re
 import math
 import datetime as dt
-import platform 
+from inspect import ismethod
+import platform
 import logging
 from logging import Logger, Handler
 import random
 import csv
 import time
 from bisect import bisect_right
 from copy import deepcopy
 from collections import defaultdict
-from typing import List, Any, Dict, Optional, Tuple, Callable, Union, Sequence, Mapping, Literal, Set,  TypeVar
+from typing import (
+    List, Any, Dict, Optional, Tuple, Callable, Union, Sequence, Mapping, Literal, Set,  TypeVar
+)
 from argparse import ArgumentParser, Namespace
 #
 import yaml
 from tqdm import tqdm
 import numpy as np
 from numpy import ndarray
 #
@@ -31,9 +34,9 @@
 from torch.nn.utils.clip_grad import clip_grad_norm_
 from torch.optim import Optimizer
 from torch.optim.lr_scheduler import _LRScheduler as LRScheduler
 from torch.cuda.amp.grad_scaler import GradScaler
 from torch.amp.autocast_mode import autocast
 # Ref: https://torchmetrics.readthedocs.io/en/stable/pages/overview.html. (torchmetrics support ddp)
 from torchmetrics import Metric, MeanMetric
-# 
+#
 from tensorboard.backend.event_processing.event_accumulator import EventAccumulator
```

### Comparing `mini-lightning-0.2.1/mini_lightning/_utils.py` & `mini-lightning-0.2.2/mini_lightning/_utils.py`

 * *Files 19% similar despite different names*

```diff
@@ -4,47 +4,50 @@
 
 
 from ._types import *
 
 __all__ = [
     "get_dist_setting", "logger",
     "en_parallel", "de_parallel", "de_sync_batchnorm", "select_device",
-    "_remove_keys", "_key_add_suffix", "freeze_layers", "stat_array",
+    "_remove_keys", "_key_add_suffix", "freeze_layers", "activate_layers", "stat_array",
     "test_time", "seed_everything", "time_synchronize",
     "print_model_info", "write_to_yaml", "read_from_yaml", "write_to_csv",
     "get_date_now", "load_ckpt", "save_ckpt",
-    "ModelCheckpoint", "ResumeFromCkpt", "parse_device_ids"
+    "ModelCheckpoint", "ResumeFromCkpt", "parse_device_ids",
 ]
 #
+_T = TypeVar("_T")
 
 
 def get_dist_setting() -> Tuple[int, int, int]:
     """return rank, local_rank, world_size"""
     rank = int(os.getenv("RANK", -1))
     local_rank = int(os.getenv("LOCAL_RANK", -1))
     world_size = int(os.getenv("WORLD_SIZE", 1))
     return rank, local_rank, world_size
 
 
-def _get_logger() -> logging.Logger:
+def _get_logger(verbose_format: bool = False) -> logging.Logger:
     level = logging.INFO
     name = "mini-lightning"
     #
     logger: Logger = logging.getLogger(name)
     logger.setLevel(level)
     handler: Handler = logging.StreamHandler()
-    handler.setFormatter(logging.Formatter(f"[%(levelname)s: {name}] %(message)s"))
+    if verbose_format:
+        _format = f"[%(levelname)s: {logger.name}] %(message)s [%(filename)s:%(lineno)d - %(asctime)s]"
+    else:
+        _format = f"[%(levelname)s: {logger.name}] %(message)s"
+    handler.setFormatter(logging.Formatter(_format))
     handler.setLevel(level)
     logger.addHandler(handler)
     return logger
 
 
-#
 logger = _get_logger()
-#
 
 
 def en_parallel(model: Module, parallel_mode: Literal["DP", "DDP", None], sync_bn: bool = False) -> Module:
     if parallel_mode is None:
         assert sync_bn is False
         return model
 
@@ -102,62 +105,89 @@
 
 
 def select_device(device_ids: List[int]) -> Device:
     """
     device: e.g. []: "cpu", [0], [0, 1, 2]
     Note: Please select CUDA before Torch initializes CUDA, otherwise it will not work
     """
+    if torch.cuda.is_initialized():
+        logger.warning("CUDA has been initialized! Device selection fails!")
+        return torch.device("cuda:0")
+    #
     log_s = "Using device: "
     if len(device_ids) == 0:
         os.environ["CUDA_VISIBLE_DEVICES"] = "-1"
         device: str = "cpu"
         log_s += device
     else:
         os.environ["CUDA_VISIBLE_DEVICES"] = ",".join([str(d) for d in device_ids])
         assert torch.cuda.is_available() and torch.cuda.device_count() >= len(device_ids)
         log_s += f"cuda:{','.join([str(d) for d in device_ids])}"  # e.g. "cuda:1,7,8"
         device = "cuda:0"
     logger.info(log_s)
     return torch.device(device)
 
 
-def _remove_keys(state_dict: Dict[str, Any], prefix_keys: List[str]) -> Dict[str, Any]:
+def _remove_keys(state_dict: Dict[str, _T], prefix_keys: List[str]) -> Dict[str, _T]:
     """Delete keys(not inplace) with a prefix. Application: load_state_dict"""
     res = {}
     for k, v in state_dict.items():
         need_saved = True
         for pk in prefix_keys:
             if k.startswith(pk):
                 need_saved = False
                 break
         if need_saved:
             res[k] = v
     return res
 
 
-def _key_add_suffix(_dict: Dict[str, Any], suffix: str) -> Dict[str, Any]:
+def _key_add_suffix(_dict: Dict[str, _T], suffix: str) -> Dict[str, _T]:
     """not inplace"""
     res = {}
     for k, v in _dict.items():
         res[k + suffix] = v
     return res
 
 
 def freeze_layers(model: Module, layer_prefix_names: List[str], verbose: bool = True) -> None:
     # e.g. ml.freeze_layers(model, ["roberta.embeddings."] + [f"roberta.encoder.layer.{i}." for i in range(2)], True)
-    lpns = set(layer_prefix_names)
+    layer_prefix_names = set(layer_prefix_names)
     for n, p in model.named_parameters():
         requires_grad = True
-        for lpn in lpns:
+        for lpn in layer_prefix_names:
             if n.startswith(lpn):
                 requires_grad = False
                 break
+        p.requires_grad_(requires_grad)
+        if verbose:
+            logger.info(f"Setting {n}.requires_grad: {requires_grad}")
+
+
+def activate_layers(model: Module, layer_suffix_names: Optional[List[str]] = None, verbose: bool = True) -> None:
+    """
+    layer_suffix_names 
+        None: show layers state.
+    """
+    if layer_suffix_names is None:
+        assert verbose is True
+    else:
+        layer_suffix_names = set(layer_suffix_names)
+    for n, p in model.named_parameters():
+        if layer_suffix_names is not None:
+            requires_grad = False
+            for lpn in layer_suffix_names:
+                if n.endswith(lpn):
+                    requires_grad = True
+                    break
+            p.requires_grad_(requires_grad)
+        else:
+            requires_grad = p.requires_grad
         if verbose:
             logger.info(f"Setting {n}.requires_grad: {requires_grad}")
-        p.requires_grad_(requires_grad)
 
 
 def stat_array(x: ndarray) -> Tuple[Tuple[float, float, float, float, int], str]:
     """statistics. return: (mean, std, min_, max_, _len), stat_str"""
     mean = x.mean().item()
     std = x.std().item()
     min_ = x.min().item()
@@ -221,15 +251,18 @@
 
 
 def time_synchronize() -> float:
     cuda.synchronize()
     return time.perf_counter()  # second
 
 
-def print_model_info(name: str, model: Module, inputs: Optional[Tuple[Any, ...]] = None) -> None:
+def print_model_info(model: Module, name: Optional[str] = None, inputs: Optional[Tuple[Any, ...]] = None) -> None:
+    if name is None:
+        name = model.__class__.__name__
+    #
     n_layers = len(list(model.modules()))
     n_params = sum(p.numel() for p in model.parameters())
     n_grads = sum(p.numel() for p in model.parameters() if p.requires_grad)
     n_buffers = sum(p.numel() for p in model.buffers())
     #
     n_params /= 1e6
     n_grads /= 1e6
@@ -284,76 +317,101 @@
     }
     return mes, date.strftime(fmt)
 
 
 def save_ckpt(
     fpath: str,
     #
-    models: Dict[str, Module],
+    models_sd: Dict[str, Dict[str, Tensor]],
     optimizers: List[Optimizer],
+    lr_schedulers: List[LRScheduler],
     **kwargs
 ) -> None:
+    lr_schedulers_sd = []
+    for lr_s in lr_schedulers:
+        lr_schedulers_sd.append({k: v for k, v in lr_s.state_dict().items() if not ismethod(v)})
+
     ckpt: Dict[str, Any] = {
-        "models": {k: m.state_dict() for k, m in models.items()},
+        "models": models_sd,
         "optimizers": [o.state_dict() for o in optimizers],
+        "lr_schedulers": lr_schedulers_sd,
     }
     #
     kwargs["date"] = get_date_now()[1]
     #
     ckpt["mes"] = kwargs
     torch.save(ckpt, fpath)
 
 
 StateDict = Dict[str, Any]
 
 
 def load_ckpt(fpath: str, map_location: Optional[Device] = None) -> \
-        Tuple[Dict[str, StateDict], List[StateDict], Dict[str, Any]]:
-    ckpt = torch.load(fpath, map_location=map_location)
-    models_state_dict = ckpt["models"]
-    optimizers_state_dict = ckpt["optimizers"]
-    return models_state_dict, optimizers_state_dict, ckpt["mes"]
+        Tuple[Dict[str, StateDict], List[StateDict], List[StateDict], Dict[str, Any]]:
+    ckpt: Dict[str, Any] = torch.load(fpath, map_location=map_location)
+    models_sd = ckpt["models"]
+    optimizers_sd = ckpt.get("optimizers", [])
+    lr_s_sd = ckpt.get("lr_schedulers", [])
+    return models_sd, optimizers_sd, lr_s_sd, ckpt["mes"]
 
 
 class ModelCheckpoint:
     def __init__(
         self,
         # Define what is a good model (for model saving)
         core_metric_name: Optional[str] = None,  # e.g. "acc".
         higher_is_better: Optional[bool] = None,  # e.g. True
         # note: the last epoch/step will always be validated
-        val_every_n: int = 1,  # val_every_n_epoch or val_every_n_steps
+        val_every_n: int = 1,  # val_every_n_epoch or val_every_n_steps. (include saving best model)
         val_mode: Literal["epoch", "step"] = "epoch",
-        #
+        saving_best_model: bool = True,
+        # 
+        saving_last_model_every_n: int = 1, 
+        saving_hf_mode: bool  = False,  
+        # False: for saving memory
         saving_optimizers: bool = False,  # state_dict
-
+        saving_lr_schedulers: bool = True,  # state_dict
         write_result_csv: bool = True,
     ) -> None:
         #
         self.core_metric_name = core_metric_name
         self.higher_is_better = higher_is_better
         self.val_every_n = val_every_n
         self.val_mode: Literal["epoch", "step"] = val_mode
+        #
+        self.saving_best_model = saving_best_model
+        self.saving_last_model_every_n = saving_last_model_every_n
+        if not self.saving_best_model and not self.saving_last_model_every_n:
+            if saving_optimizers:
+                saving_optimizers = False
+                logger.warning(f"Setting saving_optimizers: {saving_optimizers}")
+            if saving_lr_schedulers:
+                saving_lr_schedulers = False
+                logger.warning(f"Setting saving_lr_schedulers: {saving_lr_schedulers}")
+        self.saving_hf_mode = saving_hf_mode
         self.saving_optimizers = saving_optimizers
+        self.saving_lr_schedulers = saving_lr_schedulers
         self.write_result_csv = write_result_csv
 
     def __repr__(self) -> str:
         attr_str = ", ".join([f"{k}={v!r}" for k, v in self.__dict__.items()])
         return f"{self.__class__.__name__}({attr_str})"
 
 
 class ResumeFromCkpt:
     def __init__(
         self,
         ckpt_path: str,   # e.g. `trainer.last_ckpt_path`, `*.ckpt`
         load_optimizers: bool = False,
+        load_lr_schedulers: bool = False,
         load_message: bool = False,  # global_step, global_epoch...
     ) -> None:
         self.ckpt_path = ckpt_path
         self.load_optimizers = load_optimizers
+        self.load_lr_schedulers = load_lr_schedulers
         self.load_message = load_message
 
     def __repr__(self) -> str:
         attr_str = ", ".join([f"{k}={v!r}" for k, v in self.__dict__.items()])
         return f"{self.__class__.__name__}({attr_str})"
```

### Comparing `mini-lightning-0.2.1/mini_lightning/_visualize.py` & `mini-lightning-0.2.2/mini_lightning/_visualize.py`

 * *Files identical despite different names*

### Comparing `mini-lightning-0.2.1/mini_lightning.egg-info/PKG-INFO` & `mini-lightning-0.2.2/mini_lightning.egg-info/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mini-lightning
-Version: 0.2.1
+Version: 0.2.2
 Summary: Mini-Lightning is a lightweight machine learning training library, which is a mini version of Pytorch-Lightning with only 1k lines of code. It has the advantages of faster, more concise and more flexible.
 Home-page: https://github.com/ustcml/mini-lightning/
 Author: Jintao Huang
 Author-email: huangjintao@mail.ustc.edu.cn
 License: MIT
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
@@ -23,15 +23,15 @@
 [![PyPI Status](https://badge.fury.io/py/mini-lightning.svg)](https://pypi.org/project/mini-lightning/)
 [![License](https://img.shields.io/badge/License-MIT-yellowgreen.svg)](https://github.com/ustcml/mini-lightning/blob/main/LICENSE)
 [![Downloads](https://pepy.tech/badge/mini-lightning)](https://pepy.tech/project/mini-lightning)
 
 
 ## Introduction
 1. [Mini-Lightning](https://github.com/ustcml/mini-lightning/) is a **lightweight** machine learning training library, which is a mini version of [Pytorch-Lightning](https://www.pytorchlightning.ai/) with only **1k lines of code**. It has the advantages of **faster, more concise and more flexible**.
-2. **Existing features**: support for DDP(multi-node and multi-gpu), Sync-BN, DP, AMP, gradient accumulation, warmup and lr_scheduler, grad clip, tensorboard, model and result saving, beautiful console log, torchmetrics, etc.
+2. **Existing features**: support for DDP(multi-node and multi-gpu), Sync-BN, DP, MP(model parallelism), AMP, gradient accumulation, warmup and lr_scheduler, grad clip, tensorboard, huggingface, peft, LLM, torchmetrics, model and result saving, beautiful console log, etc.
 3. Only the **minimal interfaces** are exposed, keeping the features of **simplicity, easy to read, use and extend**.
 4. **examples** can be found in `examples/`
 5. If you have any problems or bug finding, please **raise issue**, Thank you.
 
 
 ## Installation
 1. Create a virtual environment and install Python (>= 3.8)
@@ -40,73 +40,82 @@
 ```bash
 # from pypi
 pip install mini-lightning -U
 
 # Or download the files from the repository to local,
 # and go to the folder where setup.py is located, and run the following command
 # (Recommended) You can enjoy the latest features and functions (including bug fixes)
-pip install .
+pip install -e .  # -e: editable mode
 ```
 
 
 ## Examples
 1. First, you need to install the Mini-Lightning
 2. Run the following examples
 
 ```bash
 ### test environment
 python examples/test_env.py
 
-### cv.py
+### cv
 pip install "torchvision>=0.13"
 python examples/cv.py
-# Using DP (not recommended, please use DDP)
+# cv+dp (not recommended, please use DDP)
 python examples/cv.py  # setting device_ids=[0, 1]
 
-### nlp.py
-pip install "transformers>=4.25" "datasets>=2.7"
-python examples/nlp.py
+### nlp: bert gpt
+pip install "transformers>=4.25" "datasets>=2.7" "peft>=0.3"
+python examples/nlp_bert_mlm.py
+python examples/nlp_bert_seq_cls.py
+python examples/nlp_gpt_lm.py
+python examples/nlp_gpt_seq_cls.py
+# sft
+python examples/nlp_gpt_zh_sft_adapter.py
+python examples/nlp_gpt_zh_sft_lora.py
+# llm (model parallelism)
+#   Ref: https://modelscope.cn/models/baichuan-inc/baichuan-7B/summary
+python examples/nlp_baichuan_sft_lora.py
+#   Ref: https://modelscope.cn/models/ZhipuAI/chatglm2-6b/summary
+python examples/nlp_chatglm2_sft_lora.py
 
-### dqn.py
+### dqn
 pip install "gym>=0.26.2" "pygame>=2.1.2"
 python examples/dqn.py
 
-### gan.py
+### gan
 pip install "torchvision>=0.13"
 python examples/gan.py
 
-### cl.py  (contrastive_learning)
+### contrastive learning
 pip install "torchvision>=0.13" "scikit-learn>=1.2"
 python examples/cl.py
-
-### cl_ddp.py
+# cl+ddp
 torchrun --nproc_per_node 2 examples/cl_ddp.py --device_ids 0 1
 
-### gnn.py gnn2.py
+### gnn
 # download torch_geometric
 #   Ref: https://pytorch-geometric.readthedocs.io/en/latest/notes/installation.html
-python examples/gnn.py
-python examples/gnn2.py
-python examples/gnn3.py
+python examples/gnn_node.py
+python examples/gnn_edge.py
+python examples/gnn_graph.py
 
-### ae.py
+### ae
 pip install "torchvision>=0.13" "scikit-learn>=1.2"
 python examples/ae.py
 
-### vae.py
+### vae
 pip install "torchvision>=0.13"
 python examples/vae.py
 
-### meta_learning.py
+### meta learning
 pip install "torchvision>=0.13"
 python examples/meta_learning.py
 
 
 ########## ddp
-### cv_ddp.py; cv_ddp_spawn.py
 # torchrun (Recommended)
 #   Ref: https://pytorch.org/docs/stable/elastic/run.html
 # spawn
 #   Ref: https://pytorch.org/docs/stable/notes/ddp.html
 ## single-node, multi-gpu
 torchrun --nproc_per_node 2 examples/cv_ddp.py --device_ids 0 1
 python cv_ddp_spawn.py  # setting device_ids=[0, 1]
@@ -117,7 +126,9 @@
 torchrun --nnodes 2 --node_rank 1 --master_addr xxx.xxx.xxx.xxx --nproc_per_node 4 examples/cv_ddp.py --device_ids 0 1 2 3
 ```
 
 
 ## TODO
 1. Automatic parameter adjustment
 2. Examples: Audio, Meta-learning, Diffusion, Auto-regressive, Reinforcement Learning
+3. Support multi-gpu test
+4. Output .log file
```

### Comparing `mini-lightning-0.2.1/setup.py` & `mini-lightning-0.2.2/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -17,15 +17,15 @@
     "Programming Language :: Python :: 3",
     "Programming Language :: Python :: 3.8",
     "Programming Language :: Python :: 3.9",
     "Programming Language :: Python :: 3.10",
 ]
 setup(
     name="mini-lightning",
-    version="0.2.1",
+    version="0.2.2",
     description=description,
     long_description=long_description,
     long_description_content_type="text/markdown",
     license="MIT",
     url="https://github.com/ustcml/mini-lightning/",
     author="Jintao Huang",
     author_email="huangjintao@mail.ustc.edu.cn",
```

### Comparing `mini-lightning-0.2.1/tests/test_utils.py` & `mini-lightning-0.2.2/tests/test_utils.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,13 +1,15 @@
 import unittest as ut
 #
 import torch
 import torch.nn as nn
 from torch import optim
+from torch.optim.lr_scheduler import LambdaLR, _LRScheduler
 #
+import os
 import mini_lightning as ml
 from torchvision.models import resnet18
 
 
 class TestUtils(ut.TestCase):
     def test_de_sync_batchnorm(self) -> None:
         # inplace
@@ -41,30 +43,42 @@
 
     def test_print_model_info(self) -> None:
         # test print_model_info
         from torchvision.models import resnet50
         import torch
         model = resnet50()
         input = torch.randn(1, 3, 224, 224)
-        ml.print_model_info("resnet", model, (input, ))
-        ml.print_model_info("resnet", model)
-        ml.print_model_info("resnet", model, (input, ))
+        ml.print_model_info(model, None, (input, ))
+        ml.print_model_info(model, "resnet", )
+        ml.print_model_info(model, "resnet", (input, ))
 
     def test_ckpt(self) -> None:
         model = resnet18()
         optimizer = optim.SGD(model.parameters(), lr=0.1, momentum=0.9)
+
+        def lr_lambda(epoch: int) -> float:
+            # 返回scale
+            if epoch < 10:
+                return 1.
+            elif epoch < 20:
+                return 0.1
+            else:
+                return 0.01
+        #
+        lr_s: _LRScheduler = LambdaLR(optimizer, lr_lambda)
         for _ in range(10):
             x = torch.randn(16, 3, 224, 224)
             loss = model(x).mean()
             optimizer.zero_grad()
             loss.backward()
             optimizer.step()
-        ml.save_ckpt("asset/tmp.ckpt", {"model": model}, [])
-        ml.save_ckpt("asset/tmp2.ckpt", {"model": model}, [optimizer])
+        os.makedirs("asset", exist_ok=True)
+        ml.save_ckpt("asset/tmp.ckpt", {"model": model.state_dict()}, [], [])
+        ml.save_ckpt("asset/tmp2.ckpt", {"model": model.state_dict()}, [optimizer], [lr_s])
         #
-        models_state_dict, _, mes = ml.load_ckpt("asset/tmp.ckpt")
+        models_state_dict, _, _,  mes = ml.load_ckpt("asset/tmp.ckpt")
         model = models_state_dict["model"]
         print(mes)
 
 
 if __name__ == "__main__":
     ut.main()
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `mini-lightning-0.2.1/tests/test_visualize.py` & `mini-lightning-0.2.2/tests/test_visualize.py`

 * *Files identical despite different names*

