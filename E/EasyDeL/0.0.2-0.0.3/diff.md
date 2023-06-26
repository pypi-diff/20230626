# Comparing `tmp/EasyDeL-0.0.2.tar.gz` & `tmp/EasyDeL-0.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "EasyDeL-0.0.2.tar", last modified: Fri Jun 23 11:25:32 2023, max compression
+gzip compressed data, was "EasyDeL-0.0.3.tar", last modified: Mon Jun 26 17:44:49 2023, max compression
```

## Comparing `EasyDeL-0.0.2.tar` & `EasyDeL-0.0.3.tar`

### file list

```diff
@@ -1,49 +1,53 @@
-drwxrwxr-x   0 erfan     (1000) erfan     (1000)        0 2023-06-23 11:25:32.747718 EasyDeL-0.0.2/
-drwxrwxr-x   0 erfan     (1000) erfan     (1000)        0 2023-06-23 11:25:32.743718 EasyDeL-0.0.2/EasyDeL.egg-info/
--rw-rw-r--   0 erfan     (1000) erfan     (1000)     3329 2023-06-23 11:25:32.000000 EasyDeL-0.0.2/EasyDeL.egg-info/PKG-INFO
--rw-rw-r--   0 erfan     (1000) erfan     (1000)     1117 2023-06-23 11:25:32.000000 EasyDeL-0.0.2/EasyDeL.egg-info/SOURCES.txt
--rw-rw-r--   0 erfan     (1000) erfan     (1000)        1 2023-06-23 11:25:32.000000 EasyDeL-0.0.2/EasyDeL.egg-info/dependency_links.txt
--rw-rw-r--   0 erfan     (1000) erfan     (1000)       14 2023-06-23 11:25:32.000000 EasyDeL-0.0.2/EasyDeL.egg-info/requires.txt
--rw-rw-r--   0 erfan     (1000) erfan     (1000)        8 2023-06-23 11:25:32.000000 EasyDeL-0.0.2/EasyDeL.egg-info/top_level.txt
-drwxrwxr-x   0 erfan     (1000) erfan     (1000)        0 2023-06-23 11:25:32.743718 EasyDeL-0.0.2/EasyDel/
--rw-rw-r--   0 erfan     (1000) erfan     (1000)     1382 2023-06-23 11:08:05.000000 EasyDeL-0.0.2/EasyDel/__init__.py
-drwxrwxr-x   0 erfan     (1000) erfan     (1000)        0 2023-06-23 11:25:32.743718 EasyDeL-0.0.2/EasyDel/modules/
--rw-rw-r--   0 erfan     (1000) erfan     (1000)     1041 2023-06-23 11:08:05.000000 EasyDeL-0.0.2/EasyDel/modules/__init__.py
-drwxrwxr-x   0 erfan     (1000) erfan     (1000)        0 2023-06-23 11:25:32.743718 EasyDeL-0.0.2/EasyDel/modules/falcon/
--rw-rw-r--   0 erfan     (1000) erfan     (1000)       88 2023-06-15 12:27:13.000000 EasyDeL-0.0.2/EasyDel/modules/falcon/__init__.py
--rw-rw-r--   0 erfan     (1000) erfan     (1000)    18490 2023-06-23 11:13:28.000000 EasyDeL-0.0.2/EasyDel/modules/falcon/modelling_falcon_flax.py
-drwxrwxr-x   0 erfan     (1000) erfan     (1000)        0 2023-06-23 11:25:32.743718 EasyDeL-0.0.2/EasyDel/modules/gpt_j/
--rw-rw-r--   0 erfan     (1000) erfan     (1000)      130 2023-06-14 16:25:08.000000 EasyDeL-0.0.2/EasyDel/modules/gpt_j/__init__.py
--rw-rw-r--   0 erfan     (1000) erfan     (1000)    31319 2023-06-14 16:25:08.000000 EasyDeL-0.0.2/EasyDel/modules/gpt_j/modelling_gpt_j_flax.py
-drwxrwxr-x   0 erfan     (1000) erfan     (1000)        0 2023-06-23 11:25:32.743718 EasyDeL-0.0.2/EasyDel/modules/gpt_neo_x/
--rw-rw-r--   0 erfan     (1000) erfan     (1000)       94 2023-06-23 11:08:05.000000 EasyDeL-0.0.2/EasyDel/modules/gpt_neo_x/__init__.py
--rw-rw-r--   0 erfan     (1000) erfan     (1000)    16080 2023-06-23 11:13:00.000000 EasyDeL-0.0.2/EasyDel/modules/gpt_neo_x/modelling_gpt_neo_x_flax.py
-drwxrwxr-x   0 erfan     (1000) erfan     (1000)        0 2023-06-23 11:25:32.743718 EasyDeL-0.0.2/EasyDel/modules/llama/
--rw-rw-r--   0 erfan     (1000) erfan     (1000)      150 2023-06-14 16:42:09.000000 EasyDeL-0.0.2/EasyDel/modules/llama/__init__.py
--rw-rw-r--   0 erfan     (1000) erfan     (1000)    34039 2023-06-23 11:21:06.000000 EasyDeL-0.0.2/EasyDel/modules/llama/modelling_llama_flax.py
--rw-rw-r--   0 erfan     (1000) erfan     (1000)    17225 2023-06-14 16:38:59.000000 EasyDeL-0.0.2/EasyDel/modules/llama/modelling_llama_pytorch.py
-drwxrwxr-x   0 erfan     (1000) erfan     (1000)        0 2023-06-23 11:25:32.747718 EasyDeL-0.0.2/EasyDel/modules/lucid_transformer/
--rw-rw-r--   0 erfan     (1000) erfan     (1000)       95 2023-06-14 16:25:08.000000 EasyDeL-0.0.2/EasyDel/modules/lucid_transformer/__init__.py
--rw-rw-r--   0 erfan     (1000) erfan     (1000)    13528 2023-06-14 16:25:08.000000 EasyDeL-0.0.2/EasyDel/modules/lucid_transformer/modelling_lt_flax.py
-drwxrwxr-x   0 erfan     (1000) erfan     (1000)        0 2023-06-23 11:25:32.747718 EasyDeL-0.0.2/EasyDel/modules/mosaic_mpt/
--rw-rw-r--   0 erfan     (1000) erfan     (1000)       76 2023-06-14 16:34:35.000000 EasyDeL-0.0.2/EasyDel/modules/mosaic_mpt/__init__.py
--rw-rw-r--   0 erfan     (1000) erfan     (1000)    17799 2023-06-22 04:42:44.000000 EasyDeL-0.0.2/EasyDel/modules/mosaic_mpt/modelling_mpt_flax.py
-drwxrwxr-x   0 erfan     (1000) erfan     (1000)        0 2023-06-23 11:25:32.747718 EasyDeL-0.0.2/EasyDel/serve/
--rw-rw-r--   0 erfan     (1000) erfan     (1000)       38 2023-06-18 16:37:39.000000 EasyDeL-0.0.2/EasyDel/serve/__init__.py
--rw-rw-r--   0 erfan     (1000) erfan     (1000)     1482 2023-06-18 16:37:39.000000 EasyDeL-0.0.2/EasyDel/serve/serve_utils.py
-drwxrwxr-x   0 erfan     (1000) erfan     (1000)        0 2023-06-23 11:25:32.747718 EasyDeL-0.0.2/EasyDel/utils/
--rw-rw-r--   0 erfan     (1000) erfan     (1000)      402 2023-06-14 16:25:08.000000 EasyDeL-0.0.2/EasyDel/utils/__init__.py
--rw-rw-r--   0 erfan     (1000) erfan     (1000)      389 2023-06-14 16:25:08.000000 EasyDeL-0.0.2/EasyDel/utils/checker.py
--rw-rw-r--   0 erfan     (1000) erfan     (1000)     2557 2023-06-21 16:33:05.000000 EasyDeL-0.0.2/EasyDel/utils/utils.py
-drwxrwxr-x   0 erfan     (1000) erfan     (1000)        0 2023-06-23 11:25:32.747718 EasyDeL-0.0.2/EasyDel/weight_convertor/
--rw-rw-r--   0 erfan     (1000) erfan     (1000)        0 2023-06-15 13:20:11.000000 EasyDeL-0.0.2/EasyDel/weight_convertor/__init__.py
--rw-rw-r--   0 erfan     (1000) erfan     (1000)     6215 2023-06-18 16:37:39.000000 EasyDeL-0.0.2/EasyDel/weight_convertor/falcon.py
--rw-rw-r--   0 erfan     (1000) erfan     (1000)     5077 2023-06-22 11:28:16.000000 EasyDeL-0.0.2/EasyDel/weight_convertor/llama.py
--rw-rw-r--   0 erfan     (1000) erfan     (1000)     9833 2023-06-18 16:37:39.000000 EasyDeL-0.0.2/EasyDel/weight_convertor/mpt.py
--rw-rw-r--   0 erfan     (1000) erfan     (1000)      858 2023-06-18 16:37:39.000000 EasyDeL-0.0.2/EasyDel/weight_convertor/utils.py
--rw-rw-r--   0 erfan     (1000) erfan     (1000)    11357 2023-06-14 16:25:08.000000 EasyDeL-0.0.2/LICENSE
--rw-rw-r--   0 erfan     (1000) erfan     (1000)     3329 2023-06-23 11:25:32.747718 EasyDeL-0.0.2/PKG-INFO
--rw-rw-r--   0 erfan     (1000) erfan     (1000)     2435 2023-06-21 16:33:05.000000 EasyDeL-0.0.2/README.md
--rw-rw-r--   0 erfan     (1000) erfan     (1000)      608 2023-06-23 10:45:58.000000 EasyDeL-0.0.2/pyproject.toml
--rw-rw-r--   0 erfan     (1000) erfan     (1000)       38 2023-06-23 11:25:32.747718 EasyDeL-0.0.2/setup.cfg
--rw-rw-r--   0 erfan     (1000) erfan     (1000)     1124 2023-06-23 11:25:27.000000 EasyDeL-0.0.2/setup.py
+drwxrwxr-x   0 erfan     (1000) erfan     (1000)        0 2023-06-26 17:44:49.741107 EasyDeL-0.0.3/
+drwxrwxr-x   0 erfan     (1000) erfan     (1000)        0 2023-06-26 17:44:49.737107 EasyDeL-0.0.3/EasyDeL.egg-info/
+-rw-rw-r--   0 erfan     (1000) erfan     (1000)     6280 2023-06-26 17:44:49.000000 EasyDeL-0.0.3/EasyDeL.egg-info/PKG-INFO
+-rw-rw-r--   0 erfan     (1000) erfan     (1000)     1201 2023-06-26 17:44:49.000000 EasyDeL-0.0.3/EasyDeL.egg-info/SOURCES.txt
+-rw-rw-r--   0 erfan     (1000) erfan     (1000)        1 2023-06-26 17:44:49.000000 EasyDeL-0.0.3/EasyDeL.egg-info/dependency_links.txt
+-rw-rw-r--   0 erfan     (1000) erfan     (1000)       14 2023-06-26 17:44:49.000000 EasyDeL-0.0.3/EasyDeL.egg-info/requires.txt
+-rw-rw-r--   0 erfan     (1000) erfan     (1000)        8 2023-06-26 17:44:49.000000 EasyDeL-0.0.3/EasyDeL.egg-info/top_level.txt
+drwxrwxr-x   0 erfan     (1000) erfan     (1000)        0 2023-06-26 17:44:49.737107 EasyDeL-0.0.3/EasyDel/
+-rw-rw-r--   0 erfan     (1000) erfan     (1000)     1502 2023-06-26 17:07:45.000000 EasyDeL-0.0.3/EasyDel/__init__.py
+drwxrwxr-x   0 erfan     (1000) erfan     (1000)        0 2023-06-26 17:44:49.737107 EasyDeL-0.0.3/EasyDel/modules/
+-rw-rw-r--   0 erfan     (1000) erfan     (1000)     1041 2023-06-23 11:08:05.000000 EasyDeL-0.0.3/EasyDel/modules/__init__.py
+drwxrwxr-x   0 erfan     (1000) erfan     (1000)        0 2023-06-26 17:44:49.737107 EasyDeL-0.0.3/EasyDel/modules/falcon/
+-rw-rw-r--   0 erfan     (1000) erfan     (1000)       88 2023-06-15 12:27:13.000000 EasyDeL-0.0.3/EasyDel/modules/falcon/__init__.py
+-rw-rw-r--   0 erfan     (1000) erfan     (1000)    18490 2023-06-23 11:13:28.000000 EasyDeL-0.0.3/EasyDel/modules/falcon/modelling_falcon_flax.py
+drwxrwxr-x   0 erfan     (1000) erfan     (1000)        0 2023-06-26 17:44:49.737107 EasyDeL-0.0.3/EasyDel/modules/gpt_j/
+-rw-rw-r--   0 erfan     (1000) erfan     (1000)      130 2023-06-14 16:25:08.000000 EasyDeL-0.0.3/EasyDel/modules/gpt_j/__init__.py
+-rw-rw-r--   0 erfan     (1000) erfan     (1000)    31319 2023-06-14 16:25:08.000000 EasyDeL-0.0.3/EasyDel/modules/gpt_j/modelling_gpt_j_flax.py
+drwxrwxr-x   0 erfan     (1000) erfan     (1000)        0 2023-06-26 17:44:49.737107 EasyDeL-0.0.3/EasyDel/modules/gpt_neo_x/
+-rw-rw-r--   0 erfan     (1000) erfan     (1000)       94 2023-06-23 11:08:05.000000 EasyDeL-0.0.3/EasyDel/modules/gpt_neo_x/__init__.py
+-rw-rw-r--   0 erfan     (1000) erfan     (1000)    16080 2023-06-23 11:13:00.000000 EasyDeL-0.0.3/EasyDel/modules/gpt_neo_x/modelling_gpt_neo_x_flax.py
+drwxrwxr-x   0 erfan     (1000) erfan     (1000)        0 2023-06-26 17:44:49.737107 EasyDeL-0.0.3/EasyDel/modules/llama/
+-rw-rw-r--   0 erfan     (1000) erfan     (1000)      150 2023-06-14 16:42:09.000000 EasyDeL-0.0.3/EasyDel/modules/llama/__init__.py
+-rw-rw-r--   0 erfan     (1000) erfan     (1000)    34039 2023-06-23 11:21:06.000000 EasyDeL-0.0.3/EasyDel/modules/llama/modelling_llama_flax.py
+-rw-rw-r--   0 erfan     (1000) erfan     (1000)    17266 2023-06-26 16:41:56.000000 EasyDeL-0.0.3/EasyDel/modules/llama/modelling_llama_pytorch.py
+drwxrwxr-x   0 erfan     (1000) erfan     (1000)        0 2023-06-26 17:44:49.737107 EasyDeL-0.0.3/EasyDel/modules/lucid_transformer/
+-rw-rw-r--   0 erfan     (1000) erfan     (1000)       95 2023-06-14 16:25:08.000000 EasyDeL-0.0.3/EasyDel/modules/lucid_transformer/__init__.py
+-rw-rw-r--   0 erfan     (1000) erfan     (1000)    13528 2023-06-14 16:25:08.000000 EasyDeL-0.0.3/EasyDel/modules/lucid_transformer/modelling_lt_flax.py
+drwxrwxr-x   0 erfan     (1000) erfan     (1000)        0 2023-06-26 17:44:49.737107 EasyDeL-0.0.3/EasyDel/modules/mosaic_mpt/
+-rw-rw-r--   0 erfan     (1000) erfan     (1000)       76 2023-06-14 16:34:35.000000 EasyDeL-0.0.3/EasyDel/modules/mosaic_mpt/__init__.py
+-rw-rw-r--   0 erfan     (1000) erfan     (1000)    17799 2023-06-22 04:42:44.000000 EasyDeL-0.0.3/EasyDel/modules/mosaic_mpt/modelling_mpt_flax.py
+drwxrwxr-x   0 erfan     (1000) erfan     (1000)        0 2023-06-26 17:44:49.737107 EasyDeL-0.0.3/EasyDel/serve/
+-rw-rw-r--   0 erfan     (1000) erfan     (1000)       38 2023-06-18 16:37:39.000000 EasyDeL-0.0.3/EasyDel/serve/__init__.py
+-rw-rw-r--   0 erfan     (1000) erfan     (1000)     1482 2023-06-18 16:37:39.000000 EasyDeL-0.0.3/EasyDel/serve/serve_utils.py
+drwxrwxr-x   0 erfan     (1000) erfan     (1000)        0 2023-06-26 17:44:49.737107 EasyDeL-0.0.3/EasyDel/trainer/
+-rw-rw-r--   0 erfan     (1000) erfan     (1000)      146 2023-06-26 17:06:26.000000 EasyDeL-0.0.3/EasyDel/trainer/__init__.py
+-rw-rw-r--   0 erfan     (1000) erfan     (1000)     8996 2023-06-26 16:41:56.000000 EasyDeL-0.0.3/EasyDel/trainer/config.py
+-rw-rw-r--   0 erfan     (1000) erfan     (1000)    11011 2023-06-26 17:03:31.000000 EasyDeL-0.0.3/EasyDel/trainer/fsdp_train.py
+drwxrwxr-x   0 erfan     (1000) erfan     (1000)        0 2023-06-26 17:44:49.737107 EasyDeL-0.0.3/EasyDel/utils/
+-rw-rw-r--   0 erfan     (1000) erfan     (1000)      402 2023-06-14 16:25:08.000000 EasyDeL-0.0.3/EasyDel/utils/__init__.py
+-rw-rw-r--   0 erfan     (1000) erfan     (1000)      389 2023-06-14 16:25:08.000000 EasyDeL-0.0.3/EasyDel/utils/checker.py
+-rw-rw-r--   0 erfan     (1000) erfan     (1000)     4584 2023-06-26 16:41:56.000000 EasyDeL-0.0.3/EasyDel/utils/utils.py
+drwxrwxr-x   0 erfan     (1000) erfan     (1000)        0 2023-06-26 17:44:49.741107 EasyDeL-0.0.3/EasyDel/weight_convertor/
+-rw-rw-r--   0 erfan     (1000) erfan     (1000)        0 2023-06-15 13:20:11.000000 EasyDeL-0.0.3/EasyDel/weight_convertor/__init__.py
+-rw-rw-r--   0 erfan     (1000) erfan     (1000)     6215 2023-06-18 16:37:39.000000 EasyDeL-0.0.3/EasyDel/weight_convertor/falcon.py
+-rw-rw-r--   0 erfan     (1000) erfan     (1000)     5077 2023-06-22 11:28:16.000000 EasyDeL-0.0.3/EasyDel/weight_convertor/llama.py
+-rw-rw-r--   0 erfan     (1000) erfan     (1000)     9833 2023-06-18 16:37:39.000000 EasyDeL-0.0.3/EasyDel/weight_convertor/mpt.py
+-rw-rw-r--   0 erfan     (1000) erfan     (1000)      858 2023-06-18 16:37:39.000000 EasyDeL-0.0.3/EasyDel/weight_convertor/utils.py
+-rw-rw-r--   0 erfan     (1000) erfan     (1000)    11357 2023-06-14 16:25:08.000000 EasyDeL-0.0.3/LICENSE
+-rw-rw-r--   0 erfan     (1000) erfan     (1000)     6280 2023-06-26 17:44:49.741107 EasyDeL-0.0.3/PKG-INFO
+-rw-rw-r--   0 erfan     (1000) erfan     (1000)     5386 2023-06-26 17:43:32.000000 EasyDeL-0.0.3/README.md
+-rw-rw-r--   0 erfan     (1000) erfan     (1000)      608 2023-06-23 10:45:58.000000 EasyDeL-0.0.3/pyproject.toml
+-rw-rw-r--   0 erfan     (1000) erfan     (1000)       38 2023-06-26 17:44:49.741107 EasyDeL-0.0.3/setup.cfg
+-rw-rw-r--   0 erfan     (1000) erfan     (1000)     1124 2023-06-26 17:35:48.000000 EasyDeL-0.0.3/setup.py
```

### Comparing `EasyDeL-0.0.2/EasyDeL.egg-info/SOURCES.txt` & `EasyDeL-0.0.3/EasyDeL.egg-info/SOURCES.txt`

 * *Files 3% similar despite different names*

```diff
@@ -20,14 +20,17 @@
 EasyDel/modules/llama/modelling_llama_pytorch.py
 EasyDel/modules/lucid_transformer/__init__.py
 EasyDel/modules/lucid_transformer/modelling_lt_flax.py
 EasyDel/modules/mosaic_mpt/__init__.py
 EasyDel/modules/mosaic_mpt/modelling_mpt_flax.py
 EasyDel/serve/__init__.py
 EasyDel/serve/serve_utils.py
+EasyDel/trainer/__init__.py
+EasyDel/trainer/config.py
+EasyDel/trainer/fsdp_train.py
 EasyDel/utils/__init__.py
 EasyDel/utils/checker.py
 EasyDel/utils/utils.py
 EasyDel/weight_convertor/__init__.py
 EasyDel/weight_convertor/falcon.py
 EasyDel/weight_convertor/llama.py
 EasyDel/weight_convertor/mpt.py
```

### Comparing `EasyDeL-0.0.2/EasyDel/__init__.py` & `EasyDeL-0.0.3/EasyDel/__init__.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-__version__ = '0.0.2'
+__version__ = '0.0.3'
 
 from .utils.checker import package_checker, is_jax_available, is_torch_available, is_flax_available, \
     is_tensorflow_available
 
 if is_torch_available():
     ...
 if is_jax_available():
@@ -10,16 +10,18 @@
 if is_tensorflow_available():
     ...
 if is_flax_available():
     from .modules import FlaxLlamaModel, LlamaConfig, FlaxLlamaForCausalLM, LlamaModel, LlamaForCausalLM, \
         FlaxLTModelModule, FlaxLTConfig, FlaxLTForCausalLM, FlaxLTModel, GPTJConfig, FlaxGPTJModule, \
         FlaxGPTJForCausalLMModule, FlaxGPTJModel, FlaxGPTJForCausalLM, FlaxMptForCausalLM, MptConfig, FlaxMptModel, \
         FlaxFalconForCausalLM, FlaxFalconModel, FalconConfig, FlaxGPTNeoXForCausalLM, GPTNeoXConfig, FlaxGPTNeoXModel
+from .trainer import finetuner, TrainArguments, fsdp_train_step
 
 __all__ = __version__, 'package_checker', 'is_jax_available', 'is_torch_available', 'is_flax_available', \
-    'is_tensorflow_available', 'LlamaConfig', 'LlamaForCausalLM', 'LlamaModel', 'FlaxLlamaForCausalLM', \
+    'is_tensorflow_available', "finetuner", "TrainArguments", "fsdp_train_step", \
+    'LlamaConfig', 'LlamaForCausalLM', 'LlamaModel', 'FlaxLlamaForCausalLM', \
     'FlaxLlamaModel', 'FlaxGPTJModule', 'FlaxGPTJForCausalLMModule', \
     'FlaxGPTJModel', 'FlaxGPTJForCausalLM', 'GPTJConfig', \
     'FlaxLTModel', 'FlaxLTConfig', 'FlaxLTModelModule', 'FlaxLTForCausalLM', \
     "FlaxMptForCausalLM", "MptConfig", "FlaxMptModel", \
     "FlaxFalconForCausalLM", "FlaxFalconModel", "FalconConfig", \
     "FlaxGPTNeoXForCausalLM", "GPTNeoXConfig", "FlaxGPTNeoXModel"
```

### Comparing `EasyDeL-0.0.2/EasyDel/modules/__init__.py` & `EasyDeL-0.0.3/EasyDel/modules/__init__.py`

 * *Files identical despite different names*

### Comparing `EasyDeL-0.0.2/EasyDel/modules/falcon/modelling_falcon_flax.py` & `EasyDeL-0.0.3/EasyDel/modules/falcon/modelling_falcon_flax.py`

 * *Files identical despite different names*

### Comparing `EasyDeL-0.0.2/EasyDel/modules/gpt_j/modelling_gpt_j_flax.py` & `EasyDeL-0.0.3/EasyDel/modules/gpt_j/modelling_gpt_j_flax.py`

 * *Files identical despite different names*

### Comparing `EasyDeL-0.0.2/EasyDel/modules/gpt_neo_x/modelling_gpt_neo_x_flax.py` & `EasyDeL-0.0.3/EasyDel/modules/gpt_neo_x/modelling_gpt_neo_x_flax.py`

 * *Files identical despite different names*

### Comparing `EasyDeL-0.0.2/EasyDel/modules/llama/modelling_llama_flax.py` & `EasyDeL-0.0.3/EasyDel/modules/llama/modelling_llama_flax.py`

 * *Files identical despite different names*

### Comparing `EasyDeL-0.0.2/EasyDel/modules/llama/modelling_llama_pytorch.py` & `EasyDeL-0.0.3/EasyDel/modules/llama/modelling_llama_pytorch.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,19 +1,24 @@
 import math
 import os
 from dataclasses import dataclass
 from typing import Optional, Union, Any
 
 import torch
 import torch.utils.checkpoint
-from erutils import make2d
+
 from torch import nn
 from transformers import PretrainedConfig, PreTrainedModel
 from transformers.utils import logging
 
+
+def make2d(tensor):
+    return tensor.view(-1, tensor.size(-1))
+
+
 logger = logging.get_logger(__name__)
 
 try:
     if os.environ['USE_JIT'] == '1':
         Module = torch.jit.ScriptModule
         function = torch.jit.script_method
     else:
```

### Comparing `EasyDeL-0.0.2/EasyDel/modules/lucid_transformer/modelling_lt_flax.py` & `EasyDeL-0.0.3/EasyDel/modules/lucid_transformer/modelling_lt_flax.py`

 * *Files identical despite different names*

### Comparing `EasyDeL-0.0.2/EasyDel/modules/mosaic_mpt/modelling_mpt_flax.py` & `EasyDeL-0.0.3/EasyDel/modules/mosaic_mpt/modelling_mpt_flax.py`

 * *Files identical despite different names*

### Comparing `EasyDeL-0.0.2/EasyDel/serve/serve_utils.py` & `EasyDeL-0.0.3/EasyDel/serve/serve_utils.py`

 * *Files identical despite different names*

### Comparing `EasyDeL-0.0.2/EasyDel/weight_convertor/falcon.py` & `EasyDeL-0.0.3/EasyDel/weight_convertor/falcon.py`

 * *Files identical despite different names*

### Comparing `EasyDeL-0.0.2/EasyDel/weight_convertor/llama.py` & `EasyDeL-0.0.3/EasyDel/weight_convertor/llama.py`

 * *Files identical despite different names*

### Comparing `EasyDeL-0.0.2/EasyDel/weight_convertor/mpt.py` & `EasyDeL-0.0.3/EasyDel/weight_convertor/mpt.py`

 * *Files identical despite different names*

### Comparing `EasyDeL-0.0.2/EasyDel/weight_convertor/utils.py` & `EasyDeL-0.0.3/EasyDel/weight_convertor/utils.py`

 * *Files identical despite different names*

### Comparing `EasyDeL-0.0.2/LICENSE` & `EasyDeL-0.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `EasyDeL-0.0.2/pyproject.toml` & `EasyDeL-0.0.3/pyproject.toml`

 * *Files identical despite different names*

### Comparing `EasyDeL-0.0.2/setup.py` & `EasyDeL-0.0.3/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
     name='EasyDeL',
-    version='0.0.2',
+    version='0.0.3',
     author='Erfan Zare Chavoshi',
     author_email='erfanzare82@eyahoo.com',
     description='An open-source library to make training faster and more optimized in Jax/Flax',
     url='https://github.com/erfanzar/EasyDeL',
     packages=find_packages(),
     long_description=open('README.md').read(),
     long_description_content_type='text/markdown',
```

