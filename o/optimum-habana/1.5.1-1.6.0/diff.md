# Comparing `tmp/optimum-habana-1.5.1.tar.gz` & `tmp/optimum-habana-1.6.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "optimum-habana-1.5.1.tar", last modified: Thu May 11 09:04:14 2023, max compression
+gzip compressed data, was "optimum-habana-1.6.0.tar", last modified: Mon Jun 26 08:33:39 2023, max compression
```

## Comparing `optimum-habana-1.5.1.tar` & `optimum-habana-1.6.0.tar`

### file list

```diff
@@ -1,72 +1,89 @@
-drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-05-11 09:04:14.257275 optimum-habana-1.5.1/
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    11357 2023-04-08 17:50:23.000000 optimum-habana-1.5.1/LICENSE
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      651 2023-04-08 17:50:23.000000 optimum-habana-1.5.1/MANIFEST.in
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    12792 2023-05-11 09:04:14.257275 optimum-habana-1.5.1/PKG-INFO
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    11641 2023-05-11 08:56:51.000000 optimum-habana-1.5.1/README.md
-drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-05-11 09:04:14.249275 optimum-habana-1.5.1/optimum/
-drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-05-11 09:04:14.253275 optimum-habana-1.5.1/optimum/habana/
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      974 2023-05-11 08:56:51.000000 optimum-habana-1.5.1/optimum/habana/__init__.py
-drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-05-11 09:04:14.253275 optimum-habana-1.5.1/optimum/habana/diffusers/
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      199 2023-04-08 17:50:23.000000 optimum-habana-1.5.1/optimum/habana/diffusers/__init__.py
-drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-05-11 09:04:14.253275 optimum-habana-1.5.1/optimum/habana/diffusers/pipelines/
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    12732 2023-05-11 08:56:51.000000 optimum-habana-1.5.1/optimum/habana/diffusers/pipelines/pipeline_utils.py
-drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-05-11 09:04:14.253275 optimum-habana-1.5.1/optimum/habana/diffusers/pipelines/stable_diffusion/
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    39462 2023-05-11 08:56:51.000000 optimum-habana-1.5.1/optimum/habana/diffusers/pipelines/stable_diffusion/pipeline_stable_diffusion.py
-drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-05-11 09:04:14.253275 optimum-habana-1.5.1/optimum/habana/diffusers/schedulers/
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)       48 2023-04-08 17:50:23.000000 optimum-habana-1.5.1/optimum/habana/diffusers/schedulers/__init__.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    14640 2023-05-06 19:21:21.000000 optimum-habana-1.5.1/optimum/habana/diffusers/schedulers/scheduling_ddim.py
-drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-05-11 09:04:14.253275 optimum-habana-1.5.1/optimum/habana/distributed/
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)       50 2023-04-28 10:18:20.000000 optimum-habana-1.5.1/optimum/habana/distributed/__init__.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    10759 2023-05-06 19:21:21.000000 optimum-habana-1.5.1/optimum/habana/distributed/distributed_runner.py
-drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-05-11 09:04:14.253275 optimum-habana-1.5.1/optimum/habana/transformers/
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1031 2023-04-08 17:50:23.000000 optimum-habana-1.5.1/optimum/habana/transformers/__init__.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     8435 2023-05-06 19:21:21.000000 optimum-habana-1.5.1/optimum/habana/transformers/deepspeed.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     2696 2023-05-06 19:21:21.000000 optimum-habana-1.5.1/optimum/habana/transformers/gaudi_configuration.py
-drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-05-11 09:04:14.253275 optimum-habana-1.5.1/optimum/habana/transformers/generation/
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)       40 2023-04-08 17:50:23.000000 optimum-habana-1.5.1/optimum/habana/transformers/generation/__init__.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)   113660 2023-05-06 19:21:21.000000 optimum-habana-1.5.1/optimum/habana/transformers/generation/utils.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     8675 2023-05-06 19:21:21.000000 optimum-habana-1.5.1/optimum/habana/transformers/gradient_checkpointing.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     3810 2023-05-11 08:56:51.000000 optimum-habana-1.5.1/optimum/habana/transformers/modeling_utils.py
-drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-05-11 09:04:14.253275 optimum-habana-1.5.1/optimum/habana/transformers/models/
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      561 2023-05-11 08:56:51.000000 optimum-habana-1.5.1/optimum/habana/transformers/models/__init__.py
-drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-05-11 09:04:14.253275 optimum-habana-1.5.1/optimum/habana/transformers/models/albert/
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)       50 2023-04-08 17:50:23.000000 optimum-habana-1.5.1/optimum/habana/transformers/models/albert/__init__.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     4422 2023-05-06 19:21:21.000000 optimum-habana-1.5.1/optimum/habana/transformers/models/albert/modeling_albert.py
-drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-05-11 09:04:14.253275 optimum-habana-1.5.1/optimum/habana/transformers/models/bloom/
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      165 2023-05-06 19:21:21.000000 optimum-habana-1.5.1/optimum/habana/transformers/models/bloom/__init__.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    20630 2023-05-06 19:21:21.000000 optimum-habana-1.5.1/optimum/habana/transformers/models/bloom/modeling_bloom.py
-drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-05-11 09:04:14.253275 optimum-habana-1.5.1/optimum/habana/transformers/models/gpt2/
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)       46 2023-05-06 19:21:21.000000 optimum-habana-1.5.1/optimum/habana/transformers/models/gpt2/__init__.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    10396 2023-05-06 19:21:21.000000 optimum-habana-1.5.1/optimum/habana/transformers/models/gpt2/modeling_gpt2.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     4914 2023-05-11 08:56:51.000000 optimum-habana-1.5.1/optimum/habana/transformers/models/modeling_all_models.py
-drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-05-11 09:04:14.253275 optimum-habana-1.5.1/optimum/habana/transformers/models/vit/
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)       59 2023-04-08 17:50:23.000000 optimum-habana-1.5.1/optimum/habana/transformers/models/vit/__init__.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     2572 2023-05-06 19:21:21.000000 optimum-habana-1.5.1/optimum/habana/transformers/models/vit/modeling_vit.py
-drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-05-11 09:04:14.253275 optimum-habana-1.5.1/optimum/habana/transformers/models/wav2vec2/
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      190 2023-04-08 17:50:23.000000 optimum-habana-1.5.1/optimum/habana/transformers/models/wav2vec2/__init__.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    11639 2023-05-06 19:21:21.000000 optimum-habana-1.5.1/optimum/habana/transformers/models/wav2vec2/modeling_wav2vec2.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    84175 2023-05-11 08:56:51.000000 optimum-habana-1.5.1/optimum/habana/transformers/trainer.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    17409 2023-05-06 19:21:21.000000 optimum-habana-1.5.1/optimum/habana/transformers/trainer_seq2seq.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     2675 2023-05-06 19:21:21.000000 optimum-habana-1.5.1/optimum/habana/transformers/trainer_utils.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    23777 2023-05-11 08:56:51.000000 optimum-habana-1.5.1/optimum/habana/transformers/training_args.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     4082 2023-05-11 08:56:51.000000 optimum-habana-1.5.1/optimum/habana/transformers/training_args_seq2seq.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     4725 2023-05-11 08:56:51.000000 optimum-habana-1.5.1/optimum/habana/utils.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      644 2023-05-11 08:57:48.000000 optimum-habana-1.5.1/optimum/habana/version.py
-drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-05-11 09:04:14.257275 optimum-habana-1.5.1/optimum_habana.egg-info/
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    12792 2023-05-11 09:04:14.000000 optimum-habana-1.5.1/optimum_habana.egg-info/PKG-INFO
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     2165 2023-05-11 09:04:14.000000 optimum-habana-1.5.1/optimum_habana.egg-info/SOURCES.txt
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)        1 2023-05-11 09:04:14.000000 optimum-habana-1.5.1/optimum_habana.egg-info/dependency_links.txt
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)        1 2023-05-11 09:04:07.000000 optimum-habana-1.5.1/optimum_habana.egg-info/not-zip-safe
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      198 2023-05-11 09:04:14.000000 optimum-habana-1.5.1/optimum_habana.egg-info/requires.txt
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)        8 2023-05-11 09:04:14.000000 optimum-habana-1.5.1/optimum_habana.egg-info/top_level.txt
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1047 2023-04-08 17:50:23.000000 optimum-habana-1.5.1/pyproject.toml
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      112 2023-05-11 09:04:14.257275 optimum-habana-1.5.1/setup.cfg
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     2967 2023-05-11 08:57:55.000000 optimum-habana-1.5.1/setup.py
-drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-05-11 09:04:14.257275 optimum-habana-1.5.1/tests/
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    19824 2023-05-11 08:56:51.000000 optimum-habana-1.5.1/tests/test_diffusers.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    17839 2023-05-11 08:56:51.000000 optimum-habana-1.5.1/tests/test_examples.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     3251 2023-04-08 17:50:23.000000 optimum-habana-1.5.1/tests/test_examples_match_transformers.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     2774 2023-04-08 17:50:23.000000 optimum-habana-1.5.1/tests/test_gaudi_configuration.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    85824 2023-05-06 19:21:21.000000 optimum-habana-1.5.1/tests/test_trainer.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     5354 2023-05-06 19:21:21.000000 optimum-habana-1.5.1/tests/test_trainer_distributed.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     4733 2023-05-11 08:56:51.000000 optimum-habana-1.5.1/tests/test_trainer_seq2seq.py
+drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-06-26 08:33:39.489526 optimum-habana-1.6.0/
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    11357 2023-06-01 21:37:59.000000 optimum-habana-1.6.0/LICENSE
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      651 2023-06-01 21:37:59.000000 optimum-habana-1.6.0/MANIFEST.in
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    12706 2023-06-26 08:33:39.489526 optimum-habana-1.6.0/PKG-INFO
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    11555 2023-06-18 22:07:26.000000 optimum-habana-1.6.0/README.md
+drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-06-26 08:33:39.481526 optimum-habana-1.6.0/optimum/
+drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-06-26 08:33:39.485526 optimum-habana-1.6.0/optimum/habana/
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1040 2023-06-01 21:37:59.000000 optimum-habana-1.6.0/optimum/habana/__init__.py
+drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-06-26 08:33:39.485526 optimum-habana-1.6.0/optimum/habana/diffusers/
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      199 2023-06-01 21:37:59.000000 optimum-habana-1.6.0/optimum/habana/diffusers/__init__.py
+drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-06-26 08:33:39.485526 optimum-habana-1.6.0/optimum/habana/diffusers/pipelines/
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    15117 2023-06-23 22:41:23.000000 optimum-habana-1.6.0/optimum/habana/diffusers/pipelines/pipeline_utils.py
+drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-06-26 08:33:39.485526 optimum-habana-1.6.0/optimum/habana/diffusers/pipelines/stable_diffusion/
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    41120 2023-06-23 22:41:23.000000 optimum-habana-1.6.0/optimum/habana/diffusers/pipelines/stable_diffusion/pipeline_stable_diffusion.py
+drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-06-26 08:33:39.485526 optimum-habana-1.6.0/optimum/habana/diffusers/schedulers/
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)       48 2023-06-01 21:37:59.000000 optimum-habana-1.6.0/optimum/habana/diffusers/schedulers/__init__.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    14640 2023-06-01 21:37:59.000000 optimum-habana-1.6.0/optimum/habana/diffusers/schedulers/scheduling_ddim.py
+drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-06-26 08:33:39.485526 optimum-habana-1.6.0/optimum/habana/distributed/
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)       93 2023-06-18 14:54:24.000000 optimum-habana-1.6.0/optimum/habana/distributed/__init__.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    10759 2023-06-01 21:37:59.000000 optimum-habana-1.6.0/optimum/habana/distributed/distributed_runner.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     6103 2023-06-22 14:31:34.000000 optimum-habana-1.6.0/optimum/habana/distributed/fast_ddp.py
+drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-06-26 08:33:39.485526 optimum-habana-1.6.0/optimum/habana/transformers/
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1031 2023-06-01 21:37:59.000000 optimum-habana-1.6.0/optimum/habana/transformers/__init__.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     8387 2023-06-18 14:54:24.000000 optimum-habana-1.6.0/optimum/habana/transformers/deepspeed.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     3105 2023-06-18 14:54:24.000000 optimum-habana-1.6.0/optimum/habana/transformers/gaudi_configuration.py
+drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-06-26 08:33:39.485526 optimum-habana-1.6.0/optimum/habana/transformers/generation/
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)       40 2023-06-01 21:37:59.000000 optimum-habana-1.6.0/optimum/habana/transformers/generation/__init__.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)   118439 2023-06-18 14:54:24.000000 optimum-habana-1.6.0/optimum/habana/transformers/generation/utils.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     8675 2023-06-18 17:50:35.000000 optimum-habana-1.6.0/optimum/habana/transformers/gradient_checkpointing.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     8063 2023-06-23 17:28:42.000000 optimum-habana-1.6.0/optimum/habana/transformers/modeling_utils.py
+drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-06-26 08:33:39.485526 optimum-habana-1.6.0/optimum/habana/transformers/models/
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1759 2023-06-23 17:28:42.000000 optimum-habana-1.6.0/optimum/habana/transformers/models/__init__.py
+drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-06-26 08:33:39.485526 optimum-habana-1.6.0/optimum/habana/transformers/models/albert/
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)       50 2023-06-01 21:37:59.000000 optimum-habana-1.6.0/optimum/habana/transformers/models/albert/__init__.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     4422 2023-06-01 21:37:59.000000 optimum-habana-1.6.0/optimum/habana/transformers/models/albert/modeling_albert.py
+drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-06-26 08:33:39.485526 optimum-habana-1.6.0/optimum/habana/transformers/models/bloom/
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      258 2023-06-23 17:28:42.000000 optimum-habana-1.6.0/optimum/habana/transformers/models/bloom/__init__.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    24977 2023-06-23 17:28:42.000000 optimum-habana-1.6.0/optimum/habana/transformers/models/bloom/modeling_bloom.py
+drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-06-26 08:33:39.485526 optimum-habana-1.6.0/optimum/habana/transformers/models/esm/
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      317 2023-06-23 17:28:42.000000 optimum-habana-1.6.0/optimum/habana/transformers/models/esm/__init__.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      470 2023-06-23 17:28:42.000000 optimum-habana-1.6.0/optimum/habana/transformers/models/esm/modeling_esm.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    15054 2023-06-06 13:54:31.000000 optimum-habana-1.6.0/optimum/habana/transformers/models/esm/modeling_esmfold.py
+drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-06-26 08:33:39.485526 optimum-habana-1.6.0/optimum/habana/transformers/models/gpt2/
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      114 2023-06-06 13:54:31.000000 optimum-habana-1.6.0/optimum/habana/transformers/models/gpt2/__init__.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    28275 2023-06-06 13:54:31.000000 optimum-habana-1.6.0/optimum/habana/transformers/models/gpt2/modeling_gpt2.py
+drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-06-26 08:33:39.485526 optimum-habana-1.6.0/optimum/habana/transformers/models/gpt_neox/
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      170 2023-06-16 12:51:49.000000 optimum-habana-1.6.0/optimum/habana/transformers/models/gpt_neox/__init__.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    15756 2023-06-16 12:51:49.000000 optimum-habana-1.6.0/optimum/habana/transformers/models/gpt_neox/modeling_gpt_neox.py
+drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-06-26 08:33:39.485526 optimum-habana-1.6.0/optimum/habana/transformers/models/gptj/
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      151 2023-06-16 12:51:49.000000 optimum-habana-1.6.0/optimum/habana/transformers/models/gptj/__init__.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    18811 2023-06-16 12:51:49.000000 optimum-habana-1.6.0/optimum/habana/transformers/models/gptj/modeling_gptj.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     5419 2023-06-01 21:37:59.000000 optimum-habana-1.6.0/optimum/habana/transformers/models/modeling_all_models.py
+drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-06-26 08:33:39.489526 optimum-habana-1.6.0/optimum/habana/transformers/models/opt/
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      225 2023-06-06 13:54:31.000000 optimum-habana-1.6.0/optimum/habana/transformers/models/opt/__init__.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    21921 2023-06-06 13:54:31.000000 optimum-habana-1.6.0/optimum/habana/transformers/models/opt/modeling_opt.py
+drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-06-26 08:33:39.489526 optimum-habana-1.6.0/optimum/habana/transformers/models/t5/
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      218 2023-06-23 17:28:42.000000 optimum-habana-1.6.0/optimum/habana/transformers/models/t5/__init__.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     7784 2023-06-23 17:28:42.000000 optimum-habana-1.6.0/optimum/habana/transformers/models/t5/modeling_t5.py
+drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-06-26 08:33:39.489526 optimum-habana-1.6.0/optimum/habana/transformers/models/vit/
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)       59 2023-06-01 21:37:59.000000 optimum-habana-1.6.0/optimum/habana/transformers/models/vit/__init__.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     2572 2023-06-01 21:37:59.000000 optimum-habana-1.6.0/optimum/habana/transformers/models/vit/modeling_vit.py
+drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-06-26 08:33:39.489526 optimum-habana-1.6.0/optimum/habana/transformers/models/wav2vec2/
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      190 2023-06-01 21:37:59.000000 optimum-habana-1.6.0/optimum/habana/transformers/models/wav2vec2/__init__.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    11639 2023-06-01 21:37:59.000000 optimum-habana-1.6.0/optimum/habana/transformers/models/wav2vec2/modeling_wav2vec2.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    92734 2023-06-23 17:28:42.000000 optimum-habana-1.6.0/optimum/habana/transformers/trainer.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    17150 2023-06-18 14:54:24.000000 optimum-habana-1.6.0/optimum/habana/transformers/trainer_seq2seq.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     2675 2023-06-01 21:37:59.000000 optimum-habana-1.6.0/optimum/habana/transformers/trainer_utils.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    29336 2023-06-18 14:54:24.000000 optimum-habana-1.6.0/optimum/habana/transformers/training_args.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     4267 2023-06-01 21:37:59.000000 optimum-habana-1.6.0/optimum/habana/transformers/training_args_seq2seq.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     9955 2023-06-18 14:54:24.000000 optimum-habana-1.6.0/optimum/habana/utils.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      644 2023-06-26 08:12:18.000000 optimum-habana-1.6.0/optimum/habana/version.py
+drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-06-26 08:33:39.489526 optimum-habana-1.6.0/optimum_habana.egg-info/
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    12706 2023-06-26 08:33:39.000000 optimum-habana-1.6.0/optimum_habana.egg-info/PKG-INFO
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     2808 2023-06-26 08:33:39.000000 optimum-habana-1.6.0/optimum_habana.egg-info/SOURCES.txt
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)        1 2023-06-26 08:33:39.000000 optimum-habana-1.6.0/optimum_habana.egg-info/dependency_links.txt
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)        1 2023-06-26 08:33:27.000000 optimum-habana-1.6.0/optimum_habana.egg-info/not-zip-safe
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      198 2023-06-26 08:33:39.000000 optimum-habana-1.6.0/optimum_habana.egg-info/requires.txt
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)        8 2023-06-26 08:33:39.000000 optimum-habana-1.6.0/optimum_habana.egg-info/top_level.txt
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1047 2023-06-01 21:37:59.000000 optimum-habana-1.6.0/pyproject.toml
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      112 2023-06-26 08:33:39.489526 optimum-habana-1.6.0/setup.cfg
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     2967 2023-06-26 08:12:31.000000 optimum-habana-1.6.0/setup.py
+drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-06-26 08:33:39.489526 optimum-habana-1.6.0/tests/
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    21789 2023-06-23 22:41:23.000000 optimum-habana-1.6.0/tests/test_diffusers.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    18420 2023-06-18 14:54:24.000000 optimum-habana-1.6.0/tests/test_examples.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     3251 2023-06-01 21:37:59.000000 optimum-habana-1.6.0/tests/test_examples_match_transformers.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     2843 2023-06-18 14:54:24.000000 optimum-habana-1.6.0/tests/test_gaudi_configuration.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    86178 2023-06-18 14:54:24.000000 optimum-habana-1.6.0/tests/test_trainer.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     5804 2023-06-18 14:54:24.000000 optimum-habana-1.6.0/tests/test_trainer_distributed.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     4743 2023-06-18 14:54:24.000000 optimum-habana-1.6.0/tests/test_trainer_seq2seq.py
```

### Comparing `optimum-habana-1.5.1/LICENSE` & `optimum-habana-1.6.0/LICENSE`

 * *Files identical despite different names*

### Comparing `optimum-habana-1.5.1/MANIFEST.in` & `optimum-habana-1.6.0/MANIFEST.in`

 * *Files identical despite different names*

### Comparing `optimum-habana-1.5.1/PKG-INFO` & `optimum-habana-1.6.0/PKG-INFO`

 * *Files 25% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: optimum-habana
-Version: 1.5.1
+Version: 1.6.0
 Summary: Optimum Habana is the interface between the Hugging Face Transformers and Diffusers libraries and Habana's Gaudi processor (HPU). It provides a set of tools enabling easy model loading, training and inference on single- and multi-HPU settings for different downstream tasks.
 Home-page: https://huggingface.co/hardware/habana
 Author: HuggingFace Inc. Special Ops Team
 Author-email: hardware@huggingface.co
 License: Apache
 Keywords: transformers,diffusers,mixed-precision training,fine-tuning,gaudi,hpu
 Classifier: Development Status :: 5 - Production/Stable
@@ -59,15 +59,15 @@
 
 ```bash
 pip install optimum[habana]
 ```
 
 > To use DeepSpeed on HPUs, you also need to run the following command:
 >```bash
->pip install git+https://github.com/HabanaAI/DeepSpeed.git@1.9.0
+>pip install git+https://github.com/HabanaAI/DeepSpeed.git@1.10.0
 >```
 
 Optimum Habana is a fast-moving project, and you may want to install it from source:
 
 ```bash
 pip install git+https://github.com/huggingface/optimum-habana.git
 ```
@@ -91,105 +91,43 @@
 There are two main classes one needs to know:
 - [GaudiTrainer](https://huggingface.co/docs/optimum/habana/package_reference/trainer): the trainer class that takes care of compiling (lazy or eager mode) and distributing the model to run on HPUs, and performing training and evaluation.
 - [GaudiConfig](https://huggingface.co/docs/optimum/habana/package_reference/gaudi_config): the class that enables to configure Habana Mixed Precision and to decide whether optimized operators and optimizers should be used or not.
 
 The [GaudiTrainer](https://huggingface.co/docs/optimum/habana/package_reference/trainer) is very similar to the [🤗 Transformers Trainer](https://huggingface.co/docs/transformers/main_classes/trainer), and adapting a script using the Trainer to make it work with Gaudi will mostly consist in simply swapping the `Trainer` class for the `GaudiTrainer` one.
 That's how most of the [example scripts](https://github.com/huggingface/optimum-habana/tree/main/examples) were adapted from their [original counterparts](https://github.com/huggingface/transformers/tree/main/examples/pytorch).
 
-Original script:
-```python
-from transformers import Trainer, TrainingArguments
+Here is an example:
+```diff
+- from transformers import Trainer, TrainingArguments
++ from optimum.habana import GaudiConfig, GaudiTrainer, GaudiTrainingArguments
 
-training_args = TrainingArguments(
+- training_args = TrainingArguments(
++ training_args = GaudiTrainingArguments(
   # training arguments...
++ use_habana=True,
++ use_lazy_mode=True,  # whether to use lazy or eager mode
++ gaudi_config_name=path_to_gaudi_config,
 )
 
 # A lot of code here
 
 # Initialize our Trainer
-trainer = Trainer(
+- trainer = Trainer(
++ trainer = GaudiTrainer(
     model=model,
     args=training_args,  # Original training arguments.
     train_dataset=train_dataset if training_args.do_train else None,
     eval_dataset=eval_dataset if training_args.do_eval else None,
     compute_metrics=compute_metrics,
     tokenizer=tokenizer,
     data_collator=data_collator,
 )
 ```
 
-
-Transformed version that can run on Gaudi:
-```python
-from optimum.habana import GaudiConfig, GaudiTrainer, GaudiTrainingArguments
-
-training_args = GaudiTrainingArguments(
-  # same training arguments...
-  use_habana=True,
-  use_lazy_mode=True,  # whether to use lazy or eager mode
-  use_hpu_graphs=True,  # whether to use HPU graphs for inference
-  gaudi_config_name=path_to_gaudi_config,
-)
-
-# A lot of the same code as the original script here
-
-# Initialize our Trainer
-trainer = GaudiTrainer(
-    model=model,
-    # You can manually specify the Gaudi configuration to use with
-    # gaudi_config=my_gaudi_config
-    args=training_args,
-    train_dataset=train_dataset if training_args.do_train else None,
-    eval_dataset=eval_dataset if training_args.do_eval else None,
-    compute_metrics=compute_metrics,
-    tokenizer=tokenizer,
-    data_collator=data_collator,
-)
-```
-
-where `gaudi_config_name` is the name of a model from the [Hub](https://huggingface.co/Habana) (Gaudi configurations are stored in model repositories). You can also give the path to a custom Gaudi configuration written in a JSON file such as this one:
-```json
-{
-  "use_habana_mixed_precision": true,
-  "hmp_is_verbose": false,
-  "use_fused_adam": true,
-  "use_fused_clip_norm": true,
-  "hmp_bf16_ops": [
-    "add",
-    "addmm",
-    "bmm",
-    "div",
-    "dropout",
-    "gelu",
-    "iadd",
-    "linear",
-    "layer_norm",
-    "matmul",
-    "mm",
-    "rsub",
-    "softmax",
-    "truediv"
-  ],
-  "hmp_fp32_ops": [
-    "embedding",
-    "nll_loss",
-    "log_softmax"
-  ]
-}
-```
-
-If you prefer to instantiate a Gaudi configuration to work on it before giving it to the trainer, you can do it as follows:
-```python
-gaudi_config = GaudiConfig.from_pretrained(
-    gaudi_config_name,
-    cache_dir=model_args.cache_dir,
-    revision=model_args.model_revision,
-    use_auth_token=True if model_args.use_auth_token else None,
-)
-```
+where `gaudi_config_name` is the name of a model from the [Hub](https://huggingface.co/Habana) (Gaudi configurations are stored in model repositories) or a path to a local Gaudi configuration file (you can see [here](https://huggingface.co/docs/optimum/habana/package_reference/gaudi_config) how to write your own).
 
 
 #### Diffusers Interface
 
 You can generate images from prompts using Stable Diffusion on Gaudi using the [`GaudiStableDiffusionPipeline`](https://huggingface.co/docs/optimum/habana/package_reference/stable_diffusion_pipeline) class and the [`GaudiDDIMScheduler`] which have been both optimized for HPUs. Here is how to use them and the differences with the 🤗 Diffusers library:
 
 ```diff
@@ -232,30 +170,40 @@
 
 | Architecture | Single Card | Multi Card | DeepSpeed | <center>Tasks</center> |
 |--------------|:-----------:|:----------:|:---------:|------------------------|
 | BERT         | :heavy_check_mark: | :heavy_check_mark: | :heavy_check_mark: | <li>[text classification](https://github.com/huggingface/optimum-habana/tree/main/examples/text-classification)</li><li>[question answering](https://github.com/huggingface/optimum-habana/tree/main/examples/question-answering)</li><li>[language modeling](https://github.com/huggingface/optimum-habana/tree/main/examples/language-modeling)</li> |
 | RoBERTa | :heavy_check_mark: | :heavy_check_mark: | :heavy_check_mark: | <li>[question answering](https://github.com/huggingface/optimum-habana/tree/main/examples/question-answering)</li><li>[language modeling](https://github.com/huggingface/optimum-habana/tree/main/examples/language-modeling)</li> |
 | ALBERT | :heavy_check_mark: | :heavy_check_mark: | :heavy_check_mark: | <li>[question answering](https://github.com/huggingface/optimum-habana/tree/main/examples/question-answering)</li><li>[language modeling](https://github.com/huggingface/optimum-habana/tree/main/examples/language-modeling)</li> |
 | DistilBERT |:heavy_check_mark: | :heavy_check_mark: | :heavy_check_mark: | <li>[question answering](https://github.com/huggingface/optimum-habana/tree/main/examples/question-answering)</li><li>[language modeling](https://github.com/huggingface/optimum-habana/tree/main/examples/language-modeling)</li> |
-| GPT2             | :heavy_check_mark: | :heavy_check_mark: | :heavy_check_mark: | <li>[language modeling](https://github.com/huggingface/optimum-habana/tree/main/examples/language-modeling)</li> |
-| T5 | :heavy_check_mark: | :heavy_check_mark: | :heavy_check_mark: | <li>[summarization](https://github.com/huggingface/optimum-habana/tree/main/examples/summarization)</li><li>[translation](https://github.com/huggingface/optimum-habana/tree/main/examples/translation)</li> |
+| GPT2             | :heavy_check_mark: | :heavy_check_mark: | :heavy_check_mark: | <li>[language modeling](https://github.com/huggingface/optimum-habana/tree/main/examples/language-modeling)</li><li>[text generation](https://github.com/huggingface/optimum-habana/tree/main/examples/text-generation)</li> |
+| T5 | :heavy_check_mark: | :heavy_check_mark: | :heavy_check_mark: | <li>[summarization](https://github.com/huggingface/optimum-habana/tree/main/examples/summarization)</li><li>[translation](https://github.com/huggingface/optimum-habana/tree/main/examples/translation)</li><li>[question answering](https://github.com/huggingface/optimum-habana/tree/main/examples/question-answering#fine-tuning-t5-on-squad20)</li> |
 | ViT | :heavy_check_mark: | :heavy_check_mark: | :heavy_check_mark: | <li>[image classification](https://github.com/huggingface/optimum-habana/tree/main/examples/image-classification)</li> |
 | Swin | :heavy_check_mark: | :heavy_check_mark: | :heavy_check_mark: | <li>[image classification](https://github.com/huggingface/optimum-habana/tree/main/examples/image-classification)</li> |
 | Wav2Vec2 | :heavy_check_mark: | :heavy_check_mark: | :heavy_check_mark: | <li>[audio classification](https://github.com/huggingface/optimum-habana/tree/main/examples/audio-classification)</li><li>[speech recognition](https://github.com/huggingface/optimum-habana/tree/main/examples/speech-recognition)</li> |
 | Stable Diffusion | :heavy_check_mark: | ✗ | ✗ | <li>[text-to-image generation](https://github.com/huggingface/optimum-habana/tree/main/examples/stable-diffusion)</li> |
 | CLIP | :heavy_check_mark: | :heavy_check_mark: | :heavy_check_mark: | <li>[contrastive image-text training](https://github.com/huggingface/optimum-habana/tree/main/examples/contrastive-image-text)</li> |
 | BLOOM(Z) | ✗ | ✗ | :heavy_check_mark: | <li>[text generation](https://github.com/huggingface/optimum-habana/tree/main/examples/text-generation)</li> |
+| StarCoder | :heavy_check_mark: | ✗ | :heavy_check_mark: | <li>[text generation](https://github.com/huggingface/optimum-habana/tree/main/examples/text-generation)</li> |
+| ESMFold | :heavy_check_mark: | ✗ | ✗ | <li>[protein folding](https://github.com/huggingface/optimum-habana/tree/main/examples/protein-folding)</li> |
+| GPT-J | :heavy_check_mark: | ✗ | :heavy_check_mark: | <li>[text generation](https://github.com/huggingface/optimum-habana/tree/main/examples/text-generation)</li> |
+| GPT-NeoX | :heavy_check_mark: | ✗ | :heavy_check_mark: | <li>[text generation](https://github.com/huggingface/optimum-habana/tree/main/examples/text-generation)</li> |
+| OPT | :heavy_check_mark: | ✗ | :heavy_check_mark: | <li>[text generation](https://github.com/huggingface/optimum-habana/tree/main/examples/text-generation)</li> |
 
 </div>
 
 Other models and tasks supported by the 🤗 Transformers library may also work. You can refer to this [section](https://github.com/huggingface/optimum-habana#how-to-use-it) for using them with 🤗 Optimum Habana. Besides, [this page](https://github.com/huggingface/optimum-habana/tree/main/examples) explains how to modify any [example](https://github.com/huggingface/transformers/tree/main/examples/pytorch) from the 🤗 Transformers library to make it work with 🤗 Optimum Habana.
 
 If you find any issue while using those, please open an issue or a pull request.
 
 
 ## Gaudi Setup
 
 Please refer to Habana Gaudi's official [installation guide](https://docs.habana.ai/en/latest/Installation_Guide/index.html).
 
 > Tests should be run in a Docker container based on Habana Docker images.
 >
-> The current version has been validated for SynapseAI 1.9.
+> The current version has been validated for SynapseAI 1.10.
+
+
+## Development
+
+Check the [contributor guide](https://github.com/huggingface/optimum/blob/main/CONTRIBUTING.md) for instructions.
```

### Comparing `optimum-habana-1.5.1/README.md` & `optimum-habana-1.6.0/optimum_habana.egg-info/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,7 +1,30 @@
+Metadata-Version: 2.1
+Name: optimum-habana
+Version: 1.6.0
+Summary: Optimum Habana is the interface between the Hugging Face Transformers and Diffusers libraries and Habana's Gaudi processor (HPU). It provides a set of tools enabling easy model loading, training and inference on single- and multi-HPU settings for different downstream tasks.
+Home-page: https://huggingface.co/hardware/habana
+Author: HuggingFace Inc. Special Ops Team
+Author-email: hardware@huggingface.co
+License: Apache
+Keywords: transformers,diffusers,mixed-precision training,fine-tuning,gaudi,hpu
+Classifier: Development Status :: 5 - Production/Stable
+Classifier: License :: OSI Approved :: Apache Software License
+Classifier: Intended Audience :: Developers
+Classifier: Intended Audience :: Education
+Classifier: Intended Audience :: Science/Research
+Classifier: Operating System :: OS Independent
+Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Topic :: Scientific/Engineering :: Artificial Intelligence
+Description-Content-Type: text/markdown
+Provides-Extra: tests
+Provides-Extra: quality
+License-File: LICENSE
+
 <!---
 Copyright 2022 The HuggingFace Team. All rights reserved.
 
 Licensed under the Apache License, Version 2.0 (the "License");
 you may not use this file except in compliance with the License.
 You may obtain a copy of the License at
 
@@ -36,15 +59,15 @@
 
 ```bash
 pip install optimum[habana]
 ```
 
 > To use DeepSpeed on HPUs, you also need to run the following command:
 >```bash
->pip install git+https://github.com/HabanaAI/DeepSpeed.git@1.9.0
+>pip install git+https://github.com/HabanaAI/DeepSpeed.git@1.10.0
 >```
 
 Optimum Habana is a fast-moving project, and you may want to install it from source:
 
 ```bash
 pip install git+https://github.com/huggingface/optimum-habana.git
 ```
@@ -68,105 +91,43 @@
 There are two main classes one needs to know:
 - [GaudiTrainer](https://huggingface.co/docs/optimum/habana/package_reference/trainer): the trainer class that takes care of compiling (lazy or eager mode) and distributing the model to run on HPUs, and performing training and evaluation.
 - [GaudiConfig](https://huggingface.co/docs/optimum/habana/package_reference/gaudi_config): the class that enables to configure Habana Mixed Precision and to decide whether optimized operators and optimizers should be used or not.
 
 The [GaudiTrainer](https://huggingface.co/docs/optimum/habana/package_reference/trainer) is very similar to the [🤗 Transformers Trainer](https://huggingface.co/docs/transformers/main_classes/trainer), and adapting a script using the Trainer to make it work with Gaudi will mostly consist in simply swapping the `Trainer` class for the `GaudiTrainer` one.
 That's how most of the [example scripts](https://github.com/huggingface/optimum-habana/tree/main/examples) were adapted from their [original counterparts](https://github.com/huggingface/transformers/tree/main/examples/pytorch).
 
-Original script:
-```python
-from transformers import Trainer, TrainingArguments
+Here is an example:
+```diff
+- from transformers import Trainer, TrainingArguments
++ from optimum.habana import GaudiConfig, GaudiTrainer, GaudiTrainingArguments
 
-training_args = TrainingArguments(
+- training_args = TrainingArguments(
++ training_args = GaudiTrainingArguments(
   # training arguments...
++ use_habana=True,
++ use_lazy_mode=True,  # whether to use lazy or eager mode
++ gaudi_config_name=path_to_gaudi_config,
 )
 
 # A lot of code here
 
 # Initialize our Trainer
-trainer = Trainer(
+- trainer = Trainer(
++ trainer = GaudiTrainer(
     model=model,
     args=training_args,  # Original training arguments.
     train_dataset=train_dataset if training_args.do_train else None,
     eval_dataset=eval_dataset if training_args.do_eval else None,
     compute_metrics=compute_metrics,
     tokenizer=tokenizer,
     data_collator=data_collator,
 )
 ```
 
-
-Transformed version that can run on Gaudi:
-```python
-from optimum.habana import GaudiConfig, GaudiTrainer, GaudiTrainingArguments
-
-training_args = GaudiTrainingArguments(
-  # same training arguments...
-  use_habana=True,
-  use_lazy_mode=True,  # whether to use lazy or eager mode
-  use_hpu_graphs=True,  # whether to use HPU graphs for inference
-  gaudi_config_name=path_to_gaudi_config,
-)
-
-# A lot of the same code as the original script here
-
-# Initialize our Trainer
-trainer = GaudiTrainer(
-    model=model,
-    # You can manually specify the Gaudi configuration to use with
-    # gaudi_config=my_gaudi_config
-    args=training_args,
-    train_dataset=train_dataset if training_args.do_train else None,
-    eval_dataset=eval_dataset if training_args.do_eval else None,
-    compute_metrics=compute_metrics,
-    tokenizer=tokenizer,
-    data_collator=data_collator,
-)
-```
-
-where `gaudi_config_name` is the name of a model from the [Hub](https://huggingface.co/Habana) (Gaudi configurations are stored in model repositories). You can also give the path to a custom Gaudi configuration written in a JSON file such as this one:
-```json
-{
-  "use_habana_mixed_precision": true,
-  "hmp_is_verbose": false,
-  "use_fused_adam": true,
-  "use_fused_clip_norm": true,
-  "hmp_bf16_ops": [
-    "add",
-    "addmm",
-    "bmm",
-    "div",
-    "dropout",
-    "gelu",
-    "iadd",
-    "linear",
-    "layer_norm",
-    "matmul",
-    "mm",
-    "rsub",
-    "softmax",
-    "truediv"
-  ],
-  "hmp_fp32_ops": [
-    "embedding",
-    "nll_loss",
-    "log_softmax"
-  ]
-}
-```
-
-If you prefer to instantiate a Gaudi configuration to work on it before giving it to the trainer, you can do it as follows:
-```python
-gaudi_config = GaudiConfig.from_pretrained(
-    gaudi_config_name,
-    cache_dir=model_args.cache_dir,
-    revision=model_args.model_revision,
-    use_auth_token=True if model_args.use_auth_token else None,
-)
-```
+where `gaudi_config_name` is the name of a model from the [Hub](https://huggingface.co/Habana) (Gaudi configurations are stored in model repositories) or a path to a local Gaudi configuration file (you can see [here](https://huggingface.co/docs/optimum/habana/package_reference/gaudi_config) how to write your own).
 
 
 #### Diffusers Interface
 
 You can generate images from prompts using Stable Diffusion on Gaudi using the [`GaudiStableDiffusionPipeline`](https://huggingface.co/docs/optimum/habana/package_reference/stable_diffusion_pipeline) class and the [`GaudiDDIMScheduler`] which have been both optimized for HPUs. Here is how to use them and the differences with the 🤗 Diffusers library:
 
 ```diff
@@ -209,30 +170,40 @@
 
 | Architecture | Single Card | Multi Card | DeepSpeed | <center>Tasks</center> |
 |--------------|:-----------:|:----------:|:---------:|------------------------|
 | BERT         | :heavy_check_mark: | :heavy_check_mark: | :heavy_check_mark: | <li>[text classification](https://github.com/huggingface/optimum-habana/tree/main/examples/text-classification)</li><li>[question answering](https://github.com/huggingface/optimum-habana/tree/main/examples/question-answering)</li><li>[language modeling](https://github.com/huggingface/optimum-habana/tree/main/examples/language-modeling)</li> |
 | RoBERTa | :heavy_check_mark: | :heavy_check_mark: | :heavy_check_mark: | <li>[question answering](https://github.com/huggingface/optimum-habana/tree/main/examples/question-answering)</li><li>[language modeling](https://github.com/huggingface/optimum-habana/tree/main/examples/language-modeling)</li> |
 | ALBERT | :heavy_check_mark: | :heavy_check_mark: | :heavy_check_mark: | <li>[question answering](https://github.com/huggingface/optimum-habana/tree/main/examples/question-answering)</li><li>[language modeling](https://github.com/huggingface/optimum-habana/tree/main/examples/language-modeling)</li> |
 | DistilBERT |:heavy_check_mark: | :heavy_check_mark: | :heavy_check_mark: | <li>[question answering](https://github.com/huggingface/optimum-habana/tree/main/examples/question-answering)</li><li>[language modeling](https://github.com/huggingface/optimum-habana/tree/main/examples/language-modeling)</li> |
-| GPT2             | :heavy_check_mark: | :heavy_check_mark: | :heavy_check_mark: | <li>[language modeling](https://github.com/huggingface/optimum-habana/tree/main/examples/language-modeling)</li> |
-| T5 | :heavy_check_mark: | :heavy_check_mark: | :heavy_check_mark: | <li>[summarization](https://github.com/huggingface/optimum-habana/tree/main/examples/summarization)</li><li>[translation](https://github.com/huggingface/optimum-habana/tree/main/examples/translation)</li> |
+| GPT2             | :heavy_check_mark: | :heavy_check_mark: | :heavy_check_mark: | <li>[language modeling](https://github.com/huggingface/optimum-habana/tree/main/examples/language-modeling)</li><li>[text generation](https://github.com/huggingface/optimum-habana/tree/main/examples/text-generation)</li> |
+| T5 | :heavy_check_mark: | :heavy_check_mark: | :heavy_check_mark: | <li>[summarization](https://github.com/huggingface/optimum-habana/tree/main/examples/summarization)</li><li>[translation](https://github.com/huggingface/optimum-habana/tree/main/examples/translation)</li><li>[question answering](https://github.com/huggingface/optimum-habana/tree/main/examples/question-answering#fine-tuning-t5-on-squad20)</li> |
 | ViT | :heavy_check_mark: | :heavy_check_mark: | :heavy_check_mark: | <li>[image classification](https://github.com/huggingface/optimum-habana/tree/main/examples/image-classification)</li> |
 | Swin | :heavy_check_mark: | :heavy_check_mark: | :heavy_check_mark: | <li>[image classification](https://github.com/huggingface/optimum-habana/tree/main/examples/image-classification)</li> |
 | Wav2Vec2 | :heavy_check_mark: | :heavy_check_mark: | :heavy_check_mark: | <li>[audio classification](https://github.com/huggingface/optimum-habana/tree/main/examples/audio-classification)</li><li>[speech recognition](https://github.com/huggingface/optimum-habana/tree/main/examples/speech-recognition)</li> |
 | Stable Diffusion | :heavy_check_mark: | ✗ | ✗ | <li>[text-to-image generation](https://github.com/huggingface/optimum-habana/tree/main/examples/stable-diffusion)</li> |
 | CLIP | :heavy_check_mark: | :heavy_check_mark: | :heavy_check_mark: | <li>[contrastive image-text training](https://github.com/huggingface/optimum-habana/tree/main/examples/contrastive-image-text)</li> |
 | BLOOM(Z) | ✗ | ✗ | :heavy_check_mark: | <li>[text generation](https://github.com/huggingface/optimum-habana/tree/main/examples/text-generation)</li> |
+| StarCoder | :heavy_check_mark: | ✗ | :heavy_check_mark: | <li>[text generation](https://github.com/huggingface/optimum-habana/tree/main/examples/text-generation)</li> |
+| ESMFold | :heavy_check_mark: | ✗ | ✗ | <li>[protein folding](https://github.com/huggingface/optimum-habana/tree/main/examples/protein-folding)</li> |
+| GPT-J | :heavy_check_mark: | ✗ | :heavy_check_mark: | <li>[text generation](https://github.com/huggingface/optimum-habana/tree/main/examples/text-generation)</li> |
+| GPT-NeoX | :heavy_check_mark: | ✗ | :heavy_check_mark: | <li>[text generation](https://github.com/huggingface/optimum-habana/tree/main/examples/text-generation)</li> |
+| OPT | :heavy_check_mark: | ✗ | :heavy_check_mark: | <li>[text generation](https://github.com/huggingface/optimum-habana/tree/main/examples/text-generation)</li> |
 
 </div>
 
 Other models and tasks supported by the 🤗 Transformers library may also work. You can refer to this [section](https://github.com/huggingface/optimum-habana#how-to-use-it) for using them with 🤗 Optimum Habana. Besides, [this page](https://github.com/huggingface/optimum-habana/tree/main/examples) explains how to modify any [example](https://github.com/huggingface/transformers/tree/main/examples/pytorch) from the 🤗 Transformers library to make it work with 🤗 Optimum Habana.
 
 If you find any issue while using those, please open an issue or a pull request.
 
 
 ## Gaudi Setup
 
 Please refer to Habana Gaudi's official [installation guide](https://docs.habana.ai/en/latest/Installation_Guide/index.html).
 
 > Tests should be run in a Docker container based on Habana Docker images.
 >
-> The current version has been validated for SynapseAI 1.9.
+> The current version has been validated for SynapseAI 1.10.
+
+
+## Development
+
+Check the [contributor guide](https://github.com/huggingface/optimum/blob/main/CONTRIBUTING.md) for instructions.
```

### Comparing `optimum-habana-1.5.1/optimum/habana/__init__.py` & `optimum-habana-1.6.0/optimum/habana/__init__.py`

 * *Files 20% similar despite different names*

```diff
@@ -19,8 +19,11 @@
 from .transformers import (
     GaudiConfig,
     GaudiSeq2SeqTrainer,
     GaudiSeq2SeqTrainingArguments,
     GaudiTrainer,
     GaudiTrainingArguments,
 )
+from .utils import check_synapse_version
 from .version import __version__
+
+check_synapse_version()
```

### Comparing `optimum-habana-1.5.1/optimum/habana/diffusers/pipelines/pipeline_utils.py` & `optimum-habana-1.6.0/optimum/habana/diffusers/pipelines/pipeline_utils.py`

 * *Files 20% similar despite different names*

```diff
@@ -14,14 +14,15 @@
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
 import copy
 import importlib
 import inspect
 import os
+import sys
 import tempfile
 from typing import Optional, Union
 
 import torch
 from diffusers.pipelines import DiffusionPipeline
 from diffusers.utils import is_compiled_module
 
@@ -68,21 +69,25 @@
         use_habana (bool, defaults to `False`):
             Whether to use Gaudi (`True`) or CPU (`False`).
         use_hpu_graphs (bool, defaults to `False`):
             Whether to use HPU graphs or not.
         gaudi_config (Union[str, [`GaudiConfig`]], defaults to `None`):
             Gaudi configuration to use. Can be a string to download it from the Hub.
             Or a previously initialized config can be passed.
+        bf16_full_eval (bool, defaults to `False`):
+            Whether to use full bfloat16 evaluation instead of 32-bit.
+            This will be faster and save memory compared to fp32/mixed precision but can harm generated images.
     """
 
     def __init__(
         self,
         use_habana: bool = False,
         use_hpu_graphs: bool = False,
         gaudi_config: Union[str, GaudiConfig] = None,
+        bf16_full_eval: bool = False,
     ):
         super().__init__()
 
         self.use_habana = use_habana
         if self.use_habana:
             self.use_hpu_graphs = use_hpu_graphs
             if self.use_hpu_graphs:
@@ -99,14 +104,55 @@
                 # Config already initialized
                 self.gaudi_config = copy.deepcopy(gaudi_config)
             else:
                 raise ValueError(
                     f"`gaudi_config` must be a string or a GaudiConfig object but is {type(gaudi_config)}."
                 )
 
+            if self.gaudi_config.use_habana_mixed_precision or self.gaudi_config.use_torch_autocast:
+                if bf16_full_eval:
+                    logger.warning(
+                        "`use_habana_mixed_precision` or `use_torch_autocast` is True in the given Gaudi configuration but "
+                        "`torch_dtype=torch.blfloat16` was given. Disabling mixed precision and continuing in bf16 only."
+                    )
+                elif self.gaudi_config.use_torch_autocast:
+                    # Open temporary files to write mixed-precision ops
+                    with tempfile.NamedTemporaryFile() as hmp_bf16_file:
+                        with tempfile.NamedTemporaryFile() as hmp_fp32_file:
+                            self.gaudi_config.write_bf16_fp32_ops_to_text_files(
+                                hmp_bf16_file.name,
+                                hmp_fp32_file.name,
+                            )
+                            os.environ["LOWER_LIST"] = str(hmp_bf16_file)
+                            os.environ["FP32_LIST"] = str(hmp_fp32_file)
+
+                            import habana_frameworks.torch.core  # noqa
+
+                elif self.gaudi_config.use_habana_mixed_precision:
+                    try:
+                        from habana_frameworks.torch.hpex import hmp
+                    except ImportError as error:
+                        error.msg = f"Could not import habana_frameworks.torch.hpex. {error.msg}."
+                        raise error
+
+                    # Open temporary files to write mixed-precision ops
+                    with tempfile.NamedTemporaryFile() as hmp_bf16_file:
+                        with tempfile.NamedTemporaryFile() as hmp_fp32_file:
+                            # hmp.convert needs ops to be written in text files
+                            self.gaudi_config.write_bf16_fp32_ops_to_text_files(
+                                hmp_bf16_file.name,
+                                hmp_fp32_file.name,
+                            )
+                            hmp.convert(
+                                opt_level=self.gaudi_config.hmp_opt_level,
+                                bf16_file_path=hmp_bf16_file.name,
+                                fp32_file_path=hmp_fp32_file.name,
+                                isVerbose=self.gaudi_config.hmp_is_verbose,
+                            )
+
             if self.use_hpu_graphs:
                 try:
                     import habana_frameworks.torch as ht
                 except ImportError as error:
                     error.msg = f"Could not import habana_frameworks.torch. {error.msg}."
                     raise error
                 self.ht = ht
@@ -115,37 +161,14 @@
             else:
                 try:
                     import habana_frameworks.torch.core as htcore
                 except ImportError as error:
                     error.msg = f"Could not import habana_frameworks.torch.core. {error.msg}."
                     raise error
                 self.htcore = htcore
-
-            if self.gaudi_config.use_habana_mixed_precision:
-                try:
-                    from habana_frameworks.torch.hpex import hmp
-                except ImportError as error:
-                    error.msg = f"Could not import habana_frameworks.torch.hpex. {error.msg}."
-                    raise error
-                self.hmp = hmp
-
-                # Open temporary files to mixed-precision write ops
-                with tempfile.NamedTemporaryFile() as hmp_bf16_file:
-                    with tempfile.NamedTemporaryFile() as hmp_fp32_file:
-                        # hmp.convert needs ops to be written in text files
-                        self.gaudi_config.write_bf16_fp32_ops_to_text_files(
-                            hmp_bf16_file.name,
-                            hmp_fp32_file.name,
-                        )
-                        self.hmp.convert(
-                            opt_level=self.gaudi_config.hmp_opt_level,
-                            bf16_file_path=hmp_bf16_file.name,
-                            fp32_file_path=hmp_fp32_file.name,
-                            isVerbose=self.gaudi_config.hmp_is_verbose,
-                        )
         else:
             if use_hpu_graphs:
                 raise ValueError(
                     "`use_hpu_graphs` is True but `use_habana` is False, please set `use_habana=True` to use HPU"
                     " graphs."
                 )
             if gaudi_config is not None:
@@ -209,21 +232,17 @@
             save_directory (`str` or `os.PathLike`):
                 Directory to which to save. Will be created if it doesn't exist.
             safe_serialization (`bool`, *optional*, defaults to `False`):
                 Whether to save the model using `safetensors` or the traditional PyTorch way (that uses `pickle`).
             variant (`str`, *optional*):
                 If specified, weights are saved in the format pytorch_model.<variant>.bin.
         """
-        self.save_config(save_directory)
-        if hasattr(self, "gaudi_config"):
-            self.gaudi_config.save_pretrained(save_directory)
-
         model_index_dict = dict(self.config)
-        model_index_dict.pop("_class_name")
-        model_index_dict.pop("_diffusers_version")
+        model_index_dict.pop("_class_name", None)
+        model_index_dict.pop("_diffusers_version", None)
         model_index_dict.pop("_module", None)
 
         expected_modules, optional_kwargs = self._get_signature_keys(self)
 
         def is_saveable_module(name, value):
             if name not in expected_modules:
                 return False
@@ -242,24 +261,36 @@
             if is_compiled_module(sub_model):
                 sub_model = sub_model._orig_mod
                 model_cls = sub_model.__class__
 
             save_method_name = None
             # search for the model's base class in GAUDI_LOADABLE_CLASSES
             for library_name, library_classes in GAUDI_LOADABLE_CLASSES.items():
-                library = importlib.import_module(library_name)
+                if library_name in sys.modules:
+                    library = importlib.import_module(library_name)
+                else:
+                    logger.info(
+                        f"{library_name} is not installed. Cannot save {pipeline_component_name} as {library_classes} from {library_name}"
+                    )
+
                 for base_class, save_load_methods in library_classes.items():
                     class_candidate = getattr(library, base_class, None)
                     if class_candidate is not None and issubclass(model_cls, class_candidate):
                         # if we found a suitable base class in GAUDI_LOADABLE_CLASSES then grab its save method
                         save_method_name = save_load_methods[0]
                         break
                 if save_method_name is not None:
                     break
 
+            if save_method_name is None:
+                logger.warn(f"self.{pipeline_component_name}={sub_model} of type {type(sub_model)} cannot be saved.")
+                # make sure that unsaveable components are not tried to be loaded afterward
+                self.register_to_config(**{pipeline_component_name: (None, None)})
+                continue
+
             save_method = getattr(sub_model, save_method_name)
 
             # Call the save method with the argument safe_serialization only if it's supported
             save_method_signature = inspect.signature(save_method)
             save_method_accept_safe = "safe_serialization" in save_method_signature.parameters
             save_method_accept_variant = "variant" in save_method_signature.parameters
 
@@ -267,14 +298,19 @@
             if save_method_accept_safe:
                 save_kwargs["safe_serialization"] = safe_serialization
             if save_method_accept_variant:
                 save_kwargs["variant"] = variant
 
             save_method(os.path.join(save_directory, pipeline_component_name), **save_kwargs)
 
+        # finally save the config
+        self.save_config(save_directory)
+        if hasattr(self, "gaudi_config"):
+            self.gaudi_config.save_pretrained(save_directory)
+
     @classmethod
     def from_pretrained(cls, pretrained_model_name_or_path: Optional[Union[str, os.PathLike]], **kwargs):
         """
         More information [here](https://huggingface.co/docs/diffusers/api/diffusion_pipeline#diffusers.DiffusionPipeline.from_pretrained).
         """
 
         # Set the correct log level depending on the node
@@ -288,11 +324,15 @@
 
         # Import diffusers.pipelines.pipeline_utils to override the values of LOADABLE_CLASSES and ALL_IMPORTABLE_CLASSES
         import diffusers.pipelines.pipeline_utils
 
         diffusers.pipelines.pipeline_utils.LOADABLE_CLASSES = GAUDI_LOADABLE_CLASSES
         diffusers.pipelines.pipeline_utils.ALL_IMPORTABLE_CLASSES = GAUDI_ALL_IMPORTABLE_CLASSES
 
+        # Define a new kwarg here to know in the __init__ whether to use mixed precision or not
+        bf16_full_eval = kwargs.get("torch_dtype", None) == torch.bfloat16
+        kwargs["bf16_full_eval"] = bf16_full_eval
+
         return super().from_pretrained(
             pretrained_model_name_or_path,
             **kwargs,
         )
```

### Comparing `optimum-habana-1.5.1/optimum/habana/diffusers/pipelines/stable_diffusion/pipeline_stable_diffusion.py` & `optimum-habana-1.6.0/optimum/habana/diffusers/pipelines/stable_diffusion/pipeline_stable_diffusion.py`

 * *Files 3% similar despite different names*

```diff
@@ -19,14 +19,15 @@
 from math import ceil
 from typing import Any, Callable, Dict, List, Optional, Union
 
 import numpy as np
 import PIL
 import torch
 from diffusers.configuration_utils import FrozenDict
+from diffusers.loaders import FromCkptMixin, LoraLoaderMixin, TextualInversionLoaderMixin
 from diffusers.models import AutoencoderKL, UNet2DConditionModel
 from diffusers.pipelines.stable_diffusion import StableDiffusionSafetyChecker
 from diffusers.schedulers import KarrasDiffusionSchedulers
 from diffusers.utils import BaseOutput, deprecate
 from packaging import version
 from transformers import CLIPImageProcessor, CLIPTextModel, CLIPTokenizer
 
@@ -43,15 +44,17 @@
 @dataclass
 class GaudiStableDiffusionPipelineOutput(BaseOutput):
     images: Union[List[PIL.Image.Image], np.ndarray]
     nsfw_content_detected: Optional[List[bool]]
     throughput: float
 
 
-class GaudiStableDiffusionPipeline(GaudiDiffusionPipeline):
+class GaudiStableDiffusionPipeline(
+    GaudiDiffusionPipeline, TextualInversionLoaderMixin, LoraLoaderMixin, FromCkptMixin
+):
     """
     Extends the [`StableDiffusionPipeline`](https://huggingface.co/docs/diffusers/api/pipelines/stable_diffusion#diffusers.StableDiffusionPipeline) class:
     - Generation is performed by batches
     - Two `mark_step()` were added to add support for lazy mode
     - Added support for HPU graphs
 
     Args:
@@ -76,14 +79,17 @@
         use_habana (bool, defaults to `False`):
             Whether to use Gaudi (`True`) or CPU (`False`).
         use_hpu_graphs (bool, defaults to `False`):
             Whether to use HPU graphs or not.
         gaudi_config (Union[str, [`GaudiConfig`]], defaults to `None`):
             Gaudi configuration to use. Can be a string to download it from the Hub.
             Or a previously initialized config can be passed.
+        bf16_full_eval (bool, defaults to `False`):
+            Whether to use full bfloat16 evaluation instead of 32-bit.
+            This will be faster and save memory compared to fp32/mixed precision but can harm generated images.
     """
 
     _optional_components = ["safety_checker", "feature_extractor"]
 
     def __init__(
         self,
         vae: AutoencoderKL,
@@ -93,19 +99,21 @@
         scheduler: KarrasDiffusionSchedulers,
         safety_checker: StableDiffusionSafetyChecker,
         feature_extractor: CLIPImageProcessor,
         requires_safety_checker: bool = True,
         use_habana: bool = False,
         use_hpu_graphs: bool = False,
         gaudi_config: Union[str, GaudiConfig] = None,
+        bf16_full_eval: bool = False,
     ):
         super().__init__(
             use_habana,
             use_hpu_graphs,
             gaudi_config,
+            bf16_full_eval,
         )
 
         if hasattr(scheduler.config, "steps_offset") and scheduler.config.steps_offset != 1:
             deprecation_message = (
                 f"The configuration file of this scheduler: {scheduler} is outdated. `steps_offset`"
                 f" should be set to 1 instead of {scheduler.config.steps_offset}. Please make sure "
                 "to update the config accordingly as leaving `steps_offset` might led to incorrect results"
@@ -238,14 +246,18 @@
             num_prompts = 1
         elif prompt is not None and isinstance(prompt, list):
             num_prompts = len(prompt)
         else:
             num_prompts = prompt_embeds.shape[0]
 
         if prompt_embeds is None:
+            # textual inversion: procecss multi-vector tokens if necessary
+            if isinstance(self, TextualInversionLoaderMixin):
+                prompt = self.maybe_convert_prompt(prompt, self.tokenizer)
+
             text_inputs = self.tokenizer(
                 prompt,
                 padding="max_length",
                 max_length=self.tokenizer.model_max_length,
                 truncation=True,
                 return_tensors="pt",
             )
@@ -298,14 +310,18 @@
                     f"`negative_prompt`: {negative_prompt} has {len(negative_prompt)} elements, but `prompt`:"
                     f" {prompt} has {num_prompts}. Please make sure that passed `negative_prompt` matches"
                     " the batch size of `prompt`."
                 )
             else:
                 uncond_tokens = negative_prompt
 
+            # textual inversion: procecss multi-vector tokens if necessary
+            if isinstance(self, TextualInversionLoaderMixin):
+                uncond_tokens = self.maybe_convert_prompt(uncond_tokens, self.tokenizer)
+
             max_length = prompt_embeds.shape[1]
             uncond_input = self.tokenizer(
                 uncond_tokens,
                 padding="max_length",
                 max_length=max_length,
                 truncation=True,
                 return_tensors="pt",
@@ -574,192 +590,195 @@
         Returns:
             [`~diffusers.pipelines.stable_diffusion.pipeline_stable_diffusion.GaudiStableDiffusionPipelineOutput`] or `tuple`:
             [`~diffusers.pipelines.stable_diffusion.pipeline_stable_diffusion.GaudiStableDiffusionPipelineOutput`] if `return_dict` is True, otherwise a `tuple`.
             When returning a tuple, the first element is a list with the generated images, and the second element is a
             list of `bool`s denoting whether the corresponding generated image likely represents "not-safe-for-work"
             (nsfw) content, according to the `safety_checker`.
         """
-        # 0. Default height and width to unet
-        height = height or self.unet.config.sample_size * self.vae_scale_factor
-        width = width or self.unet.config.sample_size * self.vae_scale_factor
-
-        # 1. Check inputs. Raise error if not correct
-        self.check_inputs(
-            prompt, height, width, callback_steps, negative_prompt, prompt_embeds, negative_prompt_embeds
-        )
-
-        # 2. Define call parameters
-        if prompt is not None and isinstance(prompt, str):
-            num_prompts = 1
-        elif prompt is not None and isinstance(prompt, list):
-            num_prompts = len(prompt)
-        else:
-            num_prompts = prompt_embeds.shape[0]
-        num_batches = ceil((num_images_per_prompt * num_prompts) / batch_size)
-        logger.info(
-            f"{num_prompts} prompt(s) received, {num_images_per_prompt} generation(s) per prompt,"
-            f" {batch_size} sample(s) per batch, {num_batches} total batch(es)."
-        )
-        if num_batches < 3:
-            logger.warning("The first two iterations are slower so it is recommended to feed more batches.")
-        device = self._execution_device
-        # here `guidance_scale` is defined analog to the guidance weight `w` of equation (2)
-        # of the Imagen paper: https://arxiv.org/pdf/2205.11487.pdf . `guidance_scale = 1`
-        # corresponds to doing no classifier free guidance.
-        do_classifier_free_guidance = guidance_scale > 1.0
-
-        # 3. Encode input prompt
-        prompt_embeds, negative_prompt_embeds = self._encode_prompt(
-            prompt,
-            device,
-            num_images_per_prompt,
-            do_classifier_free_guidance,
-            negative_prompt,
-            prompt_embeds=prompt_embeds,
-            negative_prompt_embeds=negative_prompt_embeds,
-        )
-
-        # 4. Prepare timesteps
-        self.scheduler.set_timesteps(num_inference_steps, device="cpu")
-        timesteps = self.scheduler.timesteps.to(device)
-
-        # 5. Prepare latent variables
-        num_channels_latents = self.unet.config.in_channels
-        latents = self.prepare_latents(
-            num_prompts * num_images_per_prompt,
-            num_channels_latents,
-            height,
-            width,
-            prompt_embeds.dtype,
-            device,
-            generator,
-            latents,
-        )
-
-        # 6. Prepare extra step kwargs. TODO: Logic should ideally just be moved out of the pipeline
-        extra_step_kwargs = self.prepare_extra_step_kwargs(generator, eta)
-
-        # 7. Split into batches (HPU-specific step)
-        latents_batches, text_embeddings_batches, num_dummy_samples = self._split_inputs_into_batches(
-            batch_size,
-            latents,
-            prompt_embeds,
-            negative_prompt_embeds,
-        )
+        with torch.autocast(device_type="hpu", dtype=torch.bfloat16, enabled=self.gaudi_config.use_torch_autocast):
+            # 0. Default height and width to unet
+            height = height or self.unet.config.sample_size * self.vae_scale_factor
+            width = width or self.unet.config.sample_size * self.vae_scale_factor
+
+            # 1. Check inputs. Raise error if not correct
+            self.check_inputs(
+                prompt, height, width, callback_steps, negative_prompt, prompt_embeds, negative_prompt_embeds
+            )
 
-        outputs = {
-            "images": [],
-            "has_nsfw_concept": [],
-        }
-        t0 = time.time()
-        t1 = t0
-
-        # 8. Denoising loop
-        for j in self.progress_bar(range(num_batches)):
-            # The throughput is calculated from the 3rd iteration
-            # because compilation occurs in the first two iterations
-            if j == 2:
-                t1 = time.time()
-
-            latents_batch = latents_batches[0]
-            latents_batches = torch.roll(latents_batches, shifts=-1, dims=0)
-            text_embeddings_batch = text_embeddings_batches[0]
-            text_embeddings_batches = torch.roll(text_embeddings_batches, shifts=-1, dims=0)
-
-            for i in range(num_inference_steps):
-                timestep = timesteps[0]
-                timesteps = torch.roll(timesteps, shifts=-1, dims=0)
-
-                capture = True if self.use_hpu_graphs and i < 2 else False
-
-                # expand the latents if we are doing classifier free guidance
-                latent_model_input = torch.cat([latents_batch] * 2) if do_classifier_free_guidance else latents_batch
-                # latent_model_input = self.scheduler.scale_model_input(latent_model_input, timestep)
-
-                # predict the noise residual
-                noise_pred = self.unet_hpu(
-                    latent_model_input,
-                    timestep,
-                    text_embeddings_batch,
-                    cross_attention_kwargs,
-                    capture,
-                )
+            # 2. Define call parameters
+            if prompt is not None and isinstance(prompt, str):
+                num_prompts = 1
+            elif prompt is not None and isinstance(prompt, list):
+                num_prompts = len(prompt)
+            else:
+                num_prompts = prompt_embeds.shape[0]
+            num_batches = ceil((num_images_per_prompt * num_prompts) / batch_size)
+            logger.info(
+                f"{num_prompts} prompt(s) received, {num_images_per_prompt} generation(s) per prompt,"
+                f" {batch_size} sample(s) per batch, {num_batches} total batch(es)."
+            )
+            if num_batches < 3:
+                logger.warning("The first two iterations are slower so it is recommended to feed more batches.")
+            device = self._execution_device
+            # here `guidance_scale` is defined analog to the guidance weight `w` of equation (2)
+            # of the Imagen paper: https://arxiv.org/pdf/2205.11487.pdf . `guidance_scale = 1`
+            # corresponds to doing no classifier free guidance.
+            do_classifier_free_guidance = guidance_scale > 1.0
 
-                # perform guidance
-                if do_classifier_free_guidance:
-                    noise_pred_uncond, noise_pred_text = noise_pred.chunk(2)
-                    noise_pred = noise_pred_uncond + guidance_scale * (noise_pred_text - noise_pred_uncond)
+            # 3. Encode input prompt
+            prompt_embeds, negative_prompt_embeds = self._encode_prompt(
+                prompt,
+                device,
+                num_images_per_prompt,
+                do_classifier_free_guidance,
+                negative_prompt,
+                prompt_embeds=prompt_embeds,
+                negative_prompt_embeds=negative_prompt_embeds,
+            )
+
+            # 4. Prepare timesteps
+            self.scheduler.set_timesteps(num_inference_steps, device="cpu")
+            timesteps = self.scheduler.timesteps.to(device)
+
+            # 5. Prepare latent variables
+            num_channels_latents = self.unet.config.in_channels
+            latents = self.prepare_latents(
+                num_prompts * num_images_per_prompt,
+                num_channels_latents,
+                height,
+                width,
+                prompt_embeds.dtype,
+                device,
+                generator,
+                latents,
+            )
+
+            # 6. Prepare extra step kwargs. TODO: Logic should ideally just be moved out of the pipeline
+            extra_step_kwargs = self.prepare_extra_step_kwargs(generator, eta)
+
+            # 7. Split into batches (HPU-specific step)
+            latents_batches, text_embeddings_batches, num_dummy_samples = self._split_inputs_into_batches(
+                batch_size,
+                latents,
+                prompt_embeds,
+                negative_prompt_embeds,
+            )
+
+            outputs = {
+                "images": [],
+                "has_nsfw_concept": [],
+            }
+            t0 = time.time()
+            t1 = t0
+
+            # 8. Denoising loop
+            for j in self.progress_bar(range(num_batches)):
+                # The throughput is calculated from the 3rd iteration
+                # because compilation occurs in the first two iterations
+                if j == 2:
+                    t1 = time.time()
+
+                latents_batch = latents_batches[0]
+                latents_batches = torch.roll(latents_batches, shifts=-1, dims=0)
+                text_embeddings_batch = text_embeddings_batches[0]
+                text_embeddings_batches = torch.roll(text_embeddings_batches, shifts=-1, dims=0)
+
+                for i in range(num_inference_steps):
+                    timestep = timesteps[0]
+                    timesteps = torch.roll(timesteps, shifts=-1, dims=0)
+
+                    capture = True if self.use_hpu_graphs and i < 2 else False
+
+                    # expand the latents if we are doing classifier free guidance
+                    latent_model_input = (
+                        torch.cat([latents_batch] * 2) if do_classifier_free_guidance else latents_batch
+                    )
+                    # latent_model_input = self.scheduler.scale_model_input(latent_model_input, timestep)
+
+                    # predict the noise residual
+                    noise_pred = self.unet_hpu(
+                        latent_model_input,
+                        timestep,
+                        text_embeddings_batch,
+                        cross_attention_kwargs,
+                        capture,
+                    )
+
+                    # perform guidance
+                    if do_classifier_free_guidance:
+                        noise_pred_uncond, noise_pred_text = noise_pred.chunk(2)
+                        noise_pred = noise_pred_uncond + guidance_scale * (noise_pred_text - noise_pred_uncond)
+
+                    # compute the previous noisy sample x_t -> x_t-1
+                    latents_batch = self.scheduler.step(noise_pred, latents_batch, **extra_step_kwargs).prev_sample
+
+                    if not self.use_hpu_graphs:
+                        self.htcore.mark_step()
+
+                    # call the callback, if provided
+                    if callback is not None and i % callback_steps == 0:
+                        callback(i, timestep, latents_batch)
+
+                if output_type == "latent":
+                    image = latents_batch
+                else:
+                    # 8. Post-processing
+                    image = self.decode_latents(latents_batch)
+                outputs["images"].append(image)
 
-                # compute the previous noisy sample x_t -> x_t-1
-                latents_batch = self.scheduler.step(noise_pred, latents_batch, **extra_step_kwargs).prev_sample
+                self.scheduler.reset_timestep_dependent_params()
 
                 if not self.use_hpu_graphs:
                     self.htcore.mark_step()
 
-                # call the callback, if provided
-                if callback is not None and i % callback_steps == 0:
-                    callback(i, timestep, latents_batch)
-
-            if output_type == "latent":
-                image = latents_batch
-            else:
-                # 8. Post-processing
-                image = self.decode_latents(latents_batch)
-            outputs["images"].append(image)
-
-            self.scheduler.reset_timestep_dependent_params()
-
-            if not self.use_hpu_graphs:
-                self.htcore.mark_step()
-
-        speed_metrics_prefix = "generation"
-        speed_measures = speed_metrics(
-            split=speed_metrics_prefix,
-            start_time=t0,
-            num_samples=num_batches * batch_size if t1 == t0 else (num_batches - 2) * batch_size,
-            num_steps=num_batches,
-            start_time_after_warmup=t1,
-        )
-        logger.info(f"Speed metrics: {speed_measures}")
-
-        # Remove dummy generations if needed
-        if num_dummy_samples > 0:
-            outputs["images"][-1] = outputs["images"][-1][:-num_dummy_samples]
-
-        # Process generated images
-        for i, image in enumerate(outputs["images"][:]):
-            if output_type == "latent":
-                has_nsfw_concept = None
-            else:
-                # 9. Run safety checker
-                image, has_nsfw_concept = self.run_safety_checker(image, device, prompt_embeds.dtype)
-
-            if i == 0:
-                outputs["images"].clear()
-
-            # 10. Convert to PIL
-            if output_type == "pil":
-                image = self.numpy_to_pil(image)
-                outputs["images"] += image
-            else:
-                outputs["images"] += [*image]
-
-            if has_nsfw_concept is not None:
-                outputs["has_nsfw_concept"] += has_nsfw_concept
-            else:
-                outputs["has_nsfw_concept"] = None
-
-        if not return_dict:
-            return (outputs["images"], outputs["has_nsfw_concept"])
-
-        return GaudiStableDiffusionPipelineOutput(
-            images=outputs["images"],
-            nsfw_content_detected=outputs["has_nsfw_concept"],
-            throughput=speed_measures[f"{speed_metrics_prefix}_samples_per_second"],
-        )
+            speed_metrics_prefix = "generation"
+            speed_measures = speed_metrics(
+                split=speed_metrics_prefix,
+                start_time=t0,
+                num_samples=num_batches * batch_size if t1 == t0 else (num_batches - 2) * batch_size,
+                num_steps=num_batches,
+                start_time_after_warmup=t1,
+            )
+            logger.info(f"Speed metrics: {speed_measures}")
+
+            # Remove dummy generations if needed
+            if num_dummy_samples > 0:
+                outputs["images"][-1] = outputs["images"][-1][:-num_dummy_samples]
+
+            # Process generated images
+            for i, image in enumerate(outputs["images"][:]):
+                if output_type == "latent":
+                    has_nsfw_concept = None
+                else:
+                    # 9. Run safety checker
+                    image, has_nsfw_concept = self.run_safety_checker(image, device, prompt_embeds.dtype)
+
+                if i == 0:
+                    outputs["images"].clear()
+
+                # 10. Convert to PIL
+                if output_type == "pil":
+                    image = self.numpy_to_pil(image)
+                    outputs["images"] += image
+                else:
+                    outputs["images"] += [*image]
+
+                if has_nsfw_concept is not None:
+                    outputs["has_nsfw_concept"] += has_nsfw_concept
+                else:
+                    outputs["has_nsfw_concept"] = None
+
+            if not return_dict:
+                return (outputs["images"], outputs["has_nsfw_concept"])
+
+            return GaudiStableDiffusionPipelineOutput(
+                images=outputs["images"],
+                nsfw_content_detected=outputs["has_nsfw_concept"],
+                throughput=speed_measures[f"{speed_metrics_prefix}_samples_per_second"],
+            )
 
     @torch.no_grad()
     def unet_hpu(self, latent_model_input, timestep, encoder_hidden_states, cross_attention_kwargs, capture):
         if self.use_hpu_graphs:
             return self.capture_replay(latent_model_input, timestep, encoder_hidden_states, capture)
         else:
             return self.unet(latent_model_input, timestep, encoder_hidden_states, cross_attention_kwargs).sample
```

### Comparing `optimum-habana-1.5.1/optimum/habana/diffusers/schedulers/scheduling_ddim.py` & `optimum-habana-1.6.0/optimum/habana/diffusers/schedulers/scheduling_ddim.py`

 * *Files identical despite different names*

### Comparing `optimum-habana-1.5.1/optimum/habana/distributed/distributed_runner.py` & `optimum-habana-1.6.0/optimum/habana/distributed/distributed_runner.py`

 * *Files identical despite different names*

### Comparing `optimum-habana-1.5.1/optimum/habana/transformers/__init__.py` & `optimum-habana-1.6.0/optimum/habana/transformers/__init__.py`

 * *Files identical despite different names*

### Comparing `optimum-habana-1.5.1/optimum/habana/transformers/deepspeed.py` & `optimum-habana-1.6.0/optimum/habana/transformers/deepspeed.py`

 * *Files 2% similar despite different names*

```diff
@@ -115,16 +115,15 @@
     config = hf_deepspeed_config.config
 
     # set the Deepspeed log level consistent with the Trainer
     ds_logger.setLevel(args.get_process_log_level())
 
     # TODO: temporary workaround
     # To remove when it is solved, see https://github.com/HabanaAI/Model-References/blob/17fbab7ceebca15b1560ffb2c4e15a3888bb5f33/PyTorch/nlp/pretraining/deepspeed-bert/run_pretraining.py#L527
-    if trainer.gaudi_config.use_habana_mixed_precision:
-        model.to(dtype=torch.bfloat16, device="hpu")
+    model.to(dtype=hf_deepspeed_config._dtype, device="hpu")
 
     if inference:
         # only Z3 makes sense for the inference
         if not hf_deepspeed_config.is_zero3():
             raise ValueError("ZeRO inference only makes sense with ZeRO Stage 3 - please adjust your config")
 
         # in case the training config is re-used for inference
```

### Comparing `optimum-habana-1.5.1/optimum/habana/transformers/gaudi_configuration.py` & `optimum-habana-1.6.0/optimum/habana/transformers/gaudi_configuration.py`

 * *Files 13% similar despite different names*

```diff
@@ -53,14 +53,21 @@
 
     def __init__(self, **kwargs):
         # Habana Mixed Precision (MHP) configuration
         self.use_habana_mixed_precision = kwargs.pop("use_habana_mixed_precision", False)
         self.hmp_bf16_ops = kwargs.pop("hmp_bf16_ops", DEFAULT_BF16_OPS)
         self.hmp_fp32_ops = kwargs.pop("hmp_fp32_ops", DEFAULT_FP32_OPS)
         self.hmp_is_verbose = kwargs.pop("hmp_is_verbose", False)
+        # Torch Autocast
+        self.use_torch_autocast = kwargs.pop("use_torch_autocast", False)
+
+        if self.use_habana_mixed_precision and self.use_torch_autocast:
+            raise ValueError(
+                "`use_habana_mixed_precision` and `use_torch_autocast` cannot be both `True` in your Gaudi configuration, you must choose one or the other to perform mixed-precision training."
+            )
 
         # Use Habana's custom AdamW implementation
         self.use_fused_adam = kwargs.pop("use_fused_adam", False)
         # Use Habana's custom fused clip norm implementation
         self.use_fused_clip_norm = kwargs.pop("use_fused_clip_norm", False)
 
         # TODO: to remove in a future version
```

### Comparing `optimum-habana-1.5.1/optimum/habana/transformers/generation/utils.py` & `optimum-habana-1.6.0/optimum/habana/transformers/generation/utils.py`

 * *Files 2% similar despite different names*

```diff
@@ -13,15 +13,15 @@
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
 import copy
 import inspect
 import warnings
-from typing import TYPE_CHECKING, Any, Callable, Dict, List, Optional, Union
+from typing import TYPE_CHECKING, Any, Callable, Dict, List, Optional, Tuple, Union
 
 import torch
 import torch.distributed as dist
 from transformers.deepspeed import is_deepspeed_zero3_enabled
 from transformers.generation.beam_constraints import DisjunctiveConstraint, PhrasalConstraint
 from transformers.generation.beam_search import BeamScorer, BeamSearchScorer, ConstrainedBeamSearchScorer
 from transformers.generation.configuration_utils import GenerationConfig
@@ -46,14 +46,16 @@
     SampleEncoderDecoderOutput,
     SampleOutput,
 )
 from transformers.utils import ModelOutput
 
 from optimum.utils import logging
 
+from ...utils import HabanaProfile
+
 
 if TYPE_CHECKING:
     from .streamers import BaseStreamer
 
 
 logger = logging.get_logger(__name__)
 
@@ -72,21 +74,62 @@
     """
     This class enables to perform fast generation in lazy mode and with HPU graphs.
     The only difference with GenerationMixin is that the various generation
     methods will generate sequences whose size is max_length. Having constant
     sizes allows to make the most of lazy mode and HPU graphs.
     """
 
+    @staticmethod
+    def _expand_inputs_for_generation(
+        expand_size: int = 1,
+        is_encoder_decoder: bool = False,
+        input_ids: Optional[torch.LongTensor] = None,
+        **model_kwargs,
+    ) -> Tuple[torch.LongTensor, Dict[str, Any]]:
+        """
+        Expands tensors from [batch_size, ...] to [batch_size * expand_size, ...].
+
+        Copied from Transformers: https://github.com/huggingface/transformers/blob/527ab894e59b6582578008e3b47648a65063f73d/src/transformers/generation/utils.py#L704
+        The tensor `token_idx` is not expanded.
+        """
+
+        def _expand_dict_for_generation(dict_to_expand):
+            for key in dict_to_expand:
+                if (
+                    dict_to_expand[key] is not None
+                    and key != "token_idx"
+                    and isinstance(dict_to_expand[key], torch.Tensor)
+                ):
+                    dict_to_expand[key] = dict_to_expand[key].repeat_interleave(expand_size, dim=0)
+            return dict_to_expand
+
+        if input_ids is not None:
+            input_ids = input_ids.repeat_interleave(expand_size, dim=0)
+
+        model_kwargs = _expand_dict_for_generation(model_kwargs)
+
+        if is_encoder_decoder:
+            if model_kwargs.get("encoder_outputs") is None:
+                raise ValueError("If `is_encoder_decoder` is True, make sure that `encoder_outputs` is defined.")
+            model_kwargs["encoder_outputs"] = _expand_dict_for_generation(model_kwargs["encoder_outputs"])
+
+        return input_ids, model_kwargs
+
     def _update_model_kwargs_for_generation(
         self,
         outputs: ModelOutput,
         model_kwargs: Dict[str, Any],
         is_encoder_decoder: bool = False,
         standardize_cache_format: bool = False,
     ) -> Dict[str, Any]:
+        """
+        Copied from Transformers: https://github.com/huggingface/transformers/blob/527ab894e59b6582578008e3b47648a65063f73d/src/transformers/generation/utils.py#L745
+
+        Adds support for `token_idx`, which is necessary for using static shapes.
+        """
         # update past_key_values
         model_kwargs["past_key_values"] = self._extract_past_from_model_output(
             outputs, standardize_cache_format=standardize_cache_format
         )
 
         # update token_type_ids with last value
         if "token_type_ids" in model_kwargs:
@@ -136,14 +179,16 @@
         stopping_criteria: Optional[StoppingCriteriaList] = None,
         prefix_allowed_tokens_fn: Optional[Callable[[int, torch.Tensor], List[int]]] = None,
         synced_gpus: Optional[bool] = None,
         streamer: Optional["BaseStreamer"] = None,
         lazy_mode: Optional[bool] = False,
         hpu_graphs: Optional[bool] = False,
         ignore_eos: Optional[bool] = None,
+        profiling_warmup_steps: Optional[int] = 0,
+        profiling_steps: Optional[int] = 0,
         **kwargs,
     ) -> Union[GenerateOutput, torch.LongTensor]:
         r"""
         Generates sequences of token ids for models with a language modeling head.
 
         <Tip warning={true}>
 
@@ -486,14 +531,16 @@
                 eos_token_id=generation_config.eos_token_id,
                 output_scores=generation_config.output_scores,
                 return_dict_in_generate=generation_config.return_dict_in_generate,
                 synced_gpus=synced_gpus,
                 streamer=streamer,
                 lazy_mode=lazy_mode,
                 ignore_eos=ignore_eos,
+                profiling_warmup_steps=profiling_warmup_steps,
+                profiling_steps=profiling_steps,
                 **model_kwargs,
             )
 
         elif is_contrastive_search_gen_mode:
             if generation_config.num_return_sequences > 1:
                 raise ValueError(
                     f"num_return_sequences has to be 1, but is {generation_config.num_return_sequences} when doing"
@@ -508,14 +555,16 @@
                 stopping_criteria=stopping_criteria,
                 pad_token_id=generation_config.pad_token_id,
                 eos_token_id=generation_config.eos_token_id,
                 output_scores=generation_config.output_scores,
                 return_dict_in_generate=generation_config.return_dict_in_generate,
                 synced_gpus=synced_gpus,
                 streamer=streamer,
+                profiling_warmup_steps=profiling_warmup_steps,
+                profiling_steps=profiling_steps,
                 **model_kwargs,
             )
 
         elif is_sample_gen_mode:
             # 11. prepare logits warper
             logits_warper = self._get_logits_warper(generation_config)
 
@@ -536,14 +585,17 @@
                 pad_token_id=generation_config.pad_token_id,
                 eos_token_id=generation_config.eos_token_id,
                 output_scores=generation_config.output_scores,
                 return_dict_in_generate=generation_config.return_dict_in_generate,
                 synced_gpus=synced_gpus,
                 streamer=streamer,
                 lazy_mode=lazy_mode,
+                ignore_eos=ignore_eos,
+                profiling_warmup_steps=profiling_warmup_steps,
+                profiling_steps=profiling_steps,
                 **model_kwargs,
             )
 
         elif is_beam_gen_mode:
             if generation_config.num_return_sequences > generation_config.num_beams:
                 raise ValueError("`num_return_sequences` has to be smaller or equal to `num_beams`.")
 
@@ -575,14 +627,16 @@
                 stopping_criteria=stopping_criteria,
                 pad_token_id=generation_config.pad_token_id,
                 eos_token_id=generation_config.eos_token_id,
                 output_scores=generation_config.output_scores,
                 return_dict_in_generate=generation_config.return_dict_in_generate,
                 synced_gpus=synced_gpus,
                 lazy_mode=lazy_mode,
+                profiling_warmup_steps=profiling_warmup_steps,
+                profiling_steps=profiling_steps,
                 **model_kwargs,
             )
 
         elif is_beam_sample_gen_mode:
             # 11. prepare logits warper
             logits_warper = self._get_logits_warper(generation_config)
 
@@ -615,14 +669,16 @@
                 stopping_criteria=stopping_criteria,
                 pad_token_id=generation_config.pad_token_id,
                 eos_token_id=generation_config.eos_token_id,
                 output_scores=generation_config.output_scores,
                 return_dict_in_generate=generation_config.return_dict_in_generate,
                 synced_gpus=synced_gpus,
                 lazy_mode=lazy_mode,
+                profiling_warmup_steps=profiling_warmup_steps,
+                profiling_steps=profiling_steps,
                 **model_kwargs,
             )
 
         elif is_group_beam_gen_mode:
             if generation_config.num_return_sequences > generation_config.num_beams:
                 raise ValueError("`num_return_sequences` has to be smaller or equal to `num_beams`.")
 
@@ -662,14 +718,16 @@
                 stopping_criteria=stopping_criteria,
                 pad_token_id=generation_config.pad_token_id,
                 eos_token_id=generation_config.eos_token_id,
                 output_scores=generation_config.output_scores,
                 return_dict_in_generate=generation_config.return_dict_in_generate,
                 synced_gpus=synced_gpus,
                 lazy_mode=lazy_mode,
+                profiling_warmup_steps=profiling_warmup_steps,
+                profiling_steps=profiling_steps,
                 **model_kwargs,
             )
 
         elif is_constraint_gen_mode:
             if generation_config.num_return_sequences > generation_config.num_beams:
                 raise ValueError("`num_return_sequences` has to be smaller or equal to `num_beams`.")
 
@@ -751,14 +809,16 @@
                 stopping_criteria=stopping_criteria,
                 pad_token_id=generation_config.pad_token_id,
                 eos_token_id=generation_config.eos_token_id,
                 output_scores=generation_config.output_scores,
                 return_dict_in_generate=generation_config.return_dict_in_generate,
                 synced_gpus=synced_gpus,
                 lazy_mode=lazy_mode,
+                profiling_warmup_steps=profiling_warmup_steps,
+                profiling_steps=profiling_steps,
                 **model_kwargs,
             )
 
     @torch.no_grad()
     def contrastive_search(
         self,
         input_ids: torch.LongTensor,
@@ -772,14 +832,16 @@
         output_attentions: Optional[bool] = None,
         output_hidden_states: Optional[bool] = None,
         output_scores: Optional[bool] = None,
         return_dict_in_generate: Optional[bool] = None,
         synced_gpus: Optional[bool] = False,
         streamer: Optional["BaseStreamer"] = None,
         lazy_mode: Optional[bool] = False,
+        profiling_warmup_steps: Optional[int] = 0,
+        profiling_steps: Optional[int] = 0,
         **model_kwargs,
     ) -> Union[ContrastiveSearchOutput, torch.LongTensor]:
         r"""
         Generates sequences of token ids for models with a language modeling head using **contrastive search** and can
         be used for text-decoder, text-to-text, speech-to-text, and vision-to-text models.
 
         <Tip warning={true}>
@@ -877,14 +939,16 @@
         output_hidden_states: Optional[bool] = None,
         output_scores: Optional[bool] = None,
         return_dict_in_generate: Optional[bool] = None,
         synced_gpus: Optional[bool] = False,
         streamer: Optional["BaseStreamer"] = None,
         lazy_mode: Optional[bool] = False,
         ignore_eos: Optional[bool] = None,
+        profiling_warmup_steps: Optional[int] = 0,
+        profiling_steps: Optional[int] = 0,
         **model_kwargs,
     ) -> Union[GreedySearchOutput, torch.LongTensor]:
         r"""
         Generates sequences of token ids for models with a language modeling head using **greedy decoding** and can be
         used for text-decoder, text-to-text, speech-to-text, and vision-to-text models.
 
         <Tip warning={true}>
@@ -1021,14 +1085,16 @@
                 model_kwargs["encoder_outputs"].get("hidden_states") if output_hidden_states else None
             )
 
         # keep track of which sequences are already finished
         if not ignore_eos:
             unfinished_sequences = torch.ones(input_ids.shape[0], dtype=torch.long, device=input_ids.device)
 
+        hb_profer = HabanaProfile(warmup=profiling_warmup_steps, active=profiling_steps)
+        hb_profer.start()
         this_peer_finished = False  # used by synced_gpus only
         while True:
             if lazy_mode:
                 self.htcore_generation.mark_step()
 
             if synced_gpus:
                 # Under synced_gpus the `forward` call must continue until all gpus complete their sequence.
@@ -1105,21 +1171,22 @@
 
             # if eos_token was found in one sentence, set sentence to finished
             if not ignore_eos and eos_token_id_tensor is not None:
                 unfinished_sequences = unfinished_sequences.mul(
                     next_tokens.tile(eos_token_id_tensor.shape[0], 1).ne(eos_token_id_tensor.unsqueeze(1)).prod(dim=0)
                 )
 
+            hb_profer.step()
             # stop if we exceed the maximum length, or when each sentence is finished (eager mode only)
             if (not ignore_eos and unfinished_sequences.max() == 0) or stopping_criteria(input_ids, scores):
                 if not synced_gpus:
                     break
                 else:
                     this_peer_finished = True
-
+        hb_profer.stop()
         if streamer is not None:
             streamer.end()
 
         if return_dict_in_generate:
             if self.config.is_encoder_decoder:
                 return GreedySearchEncoderDecoderOutput(
                     sequences=input_ids,
@@ -1152,14 +1219,17 @@
         output_attentions: Optional[bool] = None,
         output_hidden_states: Optional[bool] = None,
         output_scores: Optional[bool] = None,
         return_dict_in_generate: Optional[bool] = None,
         synced_gpus: Optional[bool] = False,
         streamer: Optional["BaseStreamer"] = None,
         lazy_mode: Optional[bool] = False,
+        ignore_eos: Optional[bool] = None,
+        profiling_warmup_steps: Optional[int] = 0,
+        profiling_steps: Optional[int] = 0,
         **model_kwargs,
     ) -> Union[SampleOutput, torch.LongTensor]:
         r"""
         Generates sequences of token ids for models with a language modeling head using **multinomial sampling** and
         can be used for text-decoder, text-to-text, speech-to-text, and vision-to-text models.
 
         <Tip warning={true}>
@@ -1203,14 +1273,16 @@
             synced_gpus (`bool`, *optional*, defaults to `False`):
                 Whether to continue running the while loop until max_length (needed for ZeRO stage 3)
             streamer (`BaseStreamer`, *optional*):
                 Streamer object that will be used to stream the generated sequences. Generated tokens are passed
                 through `streamer.put(token_ids)` and the streamer is responsible for any further processing.
             lazy_mode (`bool`, *optional*, defaults to `False`):
                 Whether the run is executed in lazy mode or not (i.e. eager mode).
+            ignore_eos (`bool`, *optional*):
+                Whether to ignore finished sequences (faster in lazy mode and with HPU graphs) or not (eager mode).
             model_kwargs:
                 Additional model specific kwargs will be forwarded to the `forward` function of the model. If model is
                 an encoder-decoder model the kwargs should include `encoder_outputs`.
 
         Return:
             [`transformers.generation.SampleDecoderOnlyOutput`], [`transformers.generation.SampleEncoderDecoderOutput`] or
             `torch.LongTensor`: A `torch.LongTensor` containing the generated tokens (default behaviour) or a
@@ -1267,16 +1339,14 @@
         ...     stopping_criteria=stopping_criteria,
         ... )
 
         >>> tokenizer.batch_decode(outputs, skip_special_tokens=True)
         ['Today is a beautiful day, and we must do everything possible to make it a day of celebration.']
         ```"""
 
-        logger.warning("Sampling is slow in lazy mode, eager mode should be preferred at the moment.")
-
         # init values
         logits_processor = logits_processor if logits_processor is not None else LogitsProcessorList()
         stopping_criteria = stopping_criteria if stopping_criteria is not None else StoppingCriteriaList()
         if max_length is not None:
             warnings.warn(
                 (
                     "`max_length` is deprecated in this function, use"
@@ -1314,16 +1384,18 @@
         if return_dict_in_generate and self.config.is_encoder_decoder:
             encoder_attentions = model_kwargs["encoder_outputs"].get("attentions") if output_attentions else None
             encoder_hidden_states = (
                 model_kwargs["encoder_outputs"].get("hidden_states") if output_hidden_states else None
             )
 
         # keep track of which sequences are already finished
+        # TODO: no ignore_eos check here since there is a compilation error, will add ignore_eos here if fixed
         unfinished_sequences = torch.ones(input_ids.shape[0], dtype=torch.long, device=input_ids.device)
-
+        hb_profer = HabanaProfile(warmup=profiling_warmup_steps, active=profiling_steps)
+        hb_profer.start()
         this_peer_finished = False  # used by synced_gpus only
         # auto-regressive generation
         while True:
             if lazy_mode:
                 self.htcore_generation.mark_step()
 
             if synced_gpus:
@@ -1379,14 +1451,15 @@
                     )
 
             # sample
             probs = torch.nn.functional.softmax(next_token_scores, dim=-1)
             next_tokens = torch.multinomial(probs, num_samples=1).squeeze(1)
 
             # finished sentences should have their next token be a padding token
+            # TODO: no ignore_eos check here since there is a compilation error, will add ignore_eos here if fixed
             if eos_token_id is not None:
                 if pad_token_id is None:
                     raise ValueError("If `eos_token_id` is defined, make sure that `pad_token_id` is defined.")
                 next_tokens = next_tokens * unfinished_sequences + pad_token_id * (1 - unfinished_sequences)
 
             # update generated ids, model inputs, and length for next step
             if token_idx is not None:
@@ -1398,29 +1471,29 @@
             if streamer is not None:
                 streamer.put(next_tokens.cpu())
             model_kwargs = self._update_model_kwargs_for_generation(
                 outputs, model_kwargs, is_encoder_decoder=self.config.is_encoder_decoder
             )
 
             # if eos_token was found in one sentence, set sentence to finished
-            if eos_token_id_tensor is not None:
+            if not ignore_eos and eos_token_id_tensor is not None:
                 unfinished_sequences = unfinished_sequences.mul(
                     next_tokens.tile(eos_token_id_tensor.shape[0], 1).ne(eos_token_id_tensor.unsqueeze(1)).prod(dim=0)
                 )
 
             # if lazy_mode and not hpu_graphs:
             #     self.htcore_generation.mark_step()
-
+            hb_profer.step()
             # stop if we exceed the maximum length, or when each sentence is finished (eager mode only)
-            if stopping_criteria(input_ids, scores) or (unfinished_sequences.max() == 0 and not lazy_mode):
+            if (not ignore_eos and unfinished_sequences.max() == 0) or stopping_criteria(input_ids, scores):
                 if not synced_gpus:
                     break
                 else:
                     this_peer_finished = True
-
+        hb_profer.stop()
         if streamer is not None:
             streamer.end()
 
         if return_dict_in_generate:
             if self.config.is_encoder_decoder:
                 return SampleEncoderDecoderOutput(
                     sequences=input_ids,
@@ -1452,14 +1525,16 @@
         eos_token_id: Optional[Union[int, List[int]]] = None,
         output_attentions: Optional[bool] = None,
         output_hidden_states: Optional[bool] = None,
         output_scores: Optional[bool] = None,
         return_dict_in_generate: Optional[bool] = None,
         synced_gpus: Optional[bool] = False,
         lazy_mode: Optional[bool] = False,
+        profiling_warmup_steps: Optional[int] = 0,
+        profiling_steps: Optional[int] = 0,
         **model_kwargs,
     ) -> Union[BeamSearchOutput, torch.LongTensor]:
         r"""
         Generates sequences of token ids for models with a language modeling head using **beam search decoding** and
         can be used for text-decoder, text-to-text, speech-to-text, and vision-to-text models.
 
         <Tip warning={true}>
@@ -1622,15 +1697,16 @@
             )
 
         # initialise score of first beam with 0 and the rest with -1e9. This makes sure that only tokens
         # of the first beam are considered to avoid sampling the exact same tokens across all beams.
         beam_scores = torch.zeros((batch_size, num_beams), dtype=torch.float, device=input_ids.device)
         beam_scores[:, 1:] = -1e9
         beam_scores = beam_scores.view((batch_size * num_beams,))
-
+        hb_profer = HabanaProfile(warmup=profiling_warmup_steps, active=profiling_steps)
+        hb_profer.start()
         this_peer_finished = False  # used by synced_gpus only
         while True:
             if synced_gpus:
                 # Under synced_gpus the `forward` call must continue until all gpus complete their sequence.
                 # The following logic allows an early break if all peers finished generating their sequence
                 this_peer_finished_flag = torch.tensor(0.0 if this_peer_finished else 1.0).to(input_ids.device)
                 # send 0.0 if we finished, 1.0 otherwise
@@ -1648,15 +1724,20 @@
                 output_hidden_states=output_hidden_states,
             )
 
             if synced_gpus and this_peer_finished:
                 cur_len = cur_len + 1
                 continue  # don't waste resources running the code we don't need
 
-            next_token_logits = outputs.logits[:, -1, :]
+            token_idx = model_kwargs.get("token_idx", None)
+            if token_idx is not None and outputs.logits.shape[-2] > 1:
+                next_token_logits = torch.index_select(outputs.logits, -2, token_idx - 1).squeeze(-2)
+            else:
+                next_token_logits = outputs.logits[:, -1, :]
+
             # hack: adjust tokens for Marian. For Marian we have to make sure that the `pad_token_id`
             # cannot be generated both before and after the `torch.nn.functional.log_softmax` operation.
             next_token_logits = self.adjust_logits_during_generation(next_token_logits, cur_len=cur_len)
             next_token_scores = torch.nn.functional.log_softmax(
                 next_token_logits, dim=-1
             )  # (batch_size * num_beams, vocab_size)
 
@@ -1704,15 +1785,20 @@
                 beam_indices=beam_indices,
             )
 
             beam_scores = beam_outputs["next_beam_scores"]
             beam_next_tokens = beam_outputs["next_beam_tokens"]
             beam_idx = beam_outputs["next_beam_indices"]
 
-            input_ids = torch.cat([input_ids[beam_idx, :], beam_next_tokens.unsqueeze(-1)], dim=-1)
+            if token_idx is not None:
+                input_ids.index_copy_(
+                    1, token_idx, beam_next_tokens.unsqueeze(-1) if beam_next_tokens.dim() == 1 else beam_next_tokens
+                )
+            else:
+                input_ids = torch.cat([input_ids[beam_idx, :], beam_next_tokens.unsqueeze(-1)], dim=-1)
 
             model_kwargs = self._update_model_kwargs_for_generation(
                 outputs, model_kwargs, is_encoder_decoder=self.config.is_encoder_decoder
             )
             if model_kwargs["past_key_values"] is not None:
                 model_kwargs["past_key_values"] = self._reorder_cache(model_kwargs["past_key_values"], beam_idx)
 
@@ -1720,20 +1806,21 @@
                 beam_indices = tuple((beam_indices[beam_idx[i]] + (beam_idx[i],) for i in range(len(beam_indices))))
 
             # increase cur_len
             cur_len = cur_len + 1
 
             # if lazy_mode and not hpu_graphs:
             #     self.htcore_generation.mark_step()
-
+            hb_profer.step()
             if stopping_criteria(input_ids, scores) or (beam_scorer.is_done and not lazy_mode):
                 if not synced_gpus:
                     break
                 else:
                     this_peer_finished = True
+        hb_profer.stop()
 
         sequence_outputs = beam_scorer.finalize(
             input_ids,
             beam_scores,
             next_tokens,
             next_indices,
             pad_token_id=pad_token_id,
@@ -1782,14 +1869,16 @@
         eos_token_id: Optional[Union[int, List[int]]] = None,
         output_attentions: Optional[bool] = None,
         output_hidden_states: Optional[bool] = None,
         output_scores: Optional[bool] = None,
         return_dict_in_generate: Optional[bool] = None,
         synced_gpus: Optional[bool] = False,
         lazy_mode: Optional[bool] = False,
+        profiling_warmup_steps: Optional[int] = 0,
+        profiling_steps: Optional[int] = 0,
         **model_kwargs,
     ) -> Union[BeamSampleOutput, torch.LongTensor]:
         r"""
         Generates sequences of token ids for models with a language modeling head using **beam search multinomial
         sampling** and can be used for text-decoder, text-to-text, speech-to-text, and vision-to-text models.
 
         <Tip warning={true}>
@@ -1923,14 +2012,16 @@
         output_attentions: Optional[bool] = None,
         output_hidden_states: Optional[bool] = None,
         output_scores: Optional[bool] = None,
         return_dict_in_generate: Optional[bool] = None,
         synced_gpus: Optional[bool] = False,
         lazy_mode: Optional[bool] = False,
         hpuy_graphs: Optional[bool] = False,
+        profiling_warmup_steps: Optional[int] = 0,
+        profiling_steps: Optional[int] = 0,
         **model_kwargs,
     ):
         r"""
         Generates sequences of token ids for models with a language modeling head using **diverse beam search
         decoding** and can be used for text-decoder, text-to-text, speech-to-text, and vision-to-text models.
 
         <Tip warning={true}>
@@ -2055,14 +2146,16 @@
         eos_token_id: Optional[Union[int, List[int]]] = None,
         output_attentions: Optional[bool] = None,
         output_hidden_states: Optional[bool] = None,
         output_scores: Optional[bool] = None,
         return_dict_in_generate: Optional[bool] = None,
         synced_gpus: Optional[bool] = None,
         lazy_mode: Optional[bool] = False,
+        profiling_warmup_steps: Optional[int] = 0,
+        profiling_steps: Optional[int] = 0,
         **model_kwargs,
     ) -> Union[BeamSearchOutput, torch.LongTensor]:
         r"""
         Generates sequences of token ids for models with a language modeling head using **constrained beam search
         decoding** and can be used for text-decoder, text-to-text, speech-to-text, and vision-to-text models.
 
         <Tip warning={true}>
```

### Comparing `optimum-habana-1.5.1/optimum/habana/transformers/gradient_checkpointing.py` & `optimum-habana-1.6.0/optimum/habana/transformers/gradient_checkpointing.py`

 * *Files identical despite different names*

### Comparing `optimum-habana-1.5.1/optimum/habana/transformers/models/albert/modeling_albert.py` & `optimum-habana-1.6.0/optimum/habana/transformers/models/albert/modeling_albert.py`

 * *Files identical despite different names*

### Comparing `optimum-habana-1.5.1/optimum/habana/transformers/models/bloom/modeling_bloom.py` & `optimum-habana-1.6.0/optimum/habana/transformers/models/gptj/modeling_gptj.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,502 +1,450 @@
-import math
-import os
-import warnings
 from typing import Optional, Tuple, Union
 
 import torch
 from torch.nn import CrossEntropyLoss
-from torch.nn import functional as F
-from transformers.modeling_outputs import BaseModelOutputWithPastAndCrossAttentions, CausalLMOutputWithCrossAttentions
-from transformers.models.bloom.modeling_bloom import BloomForCausalLM, BloomMLP, BloomModel
-from transformers.utils import logging
+from transformers.modeling_outputs import BaseModelOutputWithPast, CausalLMOutputWithPast
+from transformers.models.gptj.modeling_gptj import GPTJForCausalLM, apply_rotary_pos_emb, logger
 
 
-logger = logging.get_logger(__name__)
-
+def gaudi_gptj_attention_forward(
+    self,
+    hidden_states: torch.FloatTensor,
+    layer_past: Optional[Tuple[torch.Tensor]] = None,
+    attention_mask: Optional[torch.FloatTensor] = None,
+    position_ids: Optional[torch.LongTensor] = None,
+    head_mask: Optional[torch.FloatTensor] = None,
+    use_cache: Optional[bool] = False,
+    output_attentions: Optional[bool] = False,
+    token_idx: Optional[torch.Tensor] = None,
+) -> Union[
+    Tuple[torch.Tensor, Tuple[torch.Tensor]],
+    Optional[Tuple[torch.Tensor, Tuple[torch.Tensor], Tuple[torch.Tensor, ...]]],
+]:
+    """
+    Copied from GPTJAttention.forward: https://github.com/huggingface/transformers/blob/main/src/transformers/models/gptj/modeling_gptj.py
+    The only differences are:
+    - add new args token_idx
+    - remove is_torch_fx_proxy
+    - optimize KV cache
+    """
+    query = self.q_proj(hidden_states)
+    key = self.k_proj(hidden_states)
+    value = self.v_proj(hidden_states)
 
-def build_alibi_slope_tensor(n_head: int) -> torch.Tensor:
-    closest_power_of_2 = 2 ** math.floor(math.log2(n_head))
-    base = torch.tensor(2 ** (-(2 ** -(math.log2(closest_power_of_2) - 3))), dtype=torch.float32)
-    powers = torch.arange(1, 1 + closest_power_of_2, dtype=torch.int32)
-    slopes = torch.pow(base, powers)
+    query = self._split_heads(query, self.num_attention_heads, self.head_dim, True)
+    key = self._split_heads(key, self.num_attention_heads, self.head_dim, True)
+    value = self._split_heads(value, self.num_attention_heads, self.head_dim, False)
 
-    if closest_power_of_2 != n_head:
-        extra_base = torch.tensor(2 ** (-(2 ** -(math.log2(2 * closest_power_of_2) - 3))), dtype=torch.float32)
-        num_remaining_heads = min(closest_power_of_2, n_head - closest_power_of_2)
-        extra_powers = torch.arange(1, 1 + 2 * num_remaining_heads, 2, dtype=torch.int32)
-        slopes = torch.cat([slopes, torch.pow(extra_base, extra_powers)], dim=0)
-    return slopes
+    embed_positions = self._get_embed_positions(position_ids)
 
+    repeated_position_ids = position_ids.unsqueeze(-1).repeat(1, 1, embed_positions.shape[-1])
+    sincos = torch.gather(embed_positions, 1, repeated_position_ids)
+    sin, cos = torch.split(sincos, sincos.shape[-1] // 2, dim=-1)
 
-def gaudi_bloom_build_alibi_tensor(
-    attention_mask: torch.Tensor, slopes: torch.Tensor, num_heads: int, dtype: torch.dtype
-) -> torch.Tensor:
-    """
-    Link to paper: https://arxiv.org/abs/2108.12409 Alibi tensor is not causal as the original paper mentions, it
-    relies on a translation invariance of softmax for quick implementation: with l being a tensor, and a fixed value
-    `softmax(l+a) = softmax(l)`. Based on
-    https://github.com/ofirpress/attention_with_linear_biases/blob/a35aaca144e0eb6b789dfcb46784c4b8e31b7983/fairseq/models/transformer.py#L742
-    TODO @thomasw21 this doesn't work as nicely due to the masking strategy, and so masking varies slightly.
-
-    Args:
-    Returns tensor shaped (batch_size * num_heads, 1, max_seq_len)
-        attention_mask (`torch.Tensor`):
-            Token-wise attention mask, this should be of shape (batch_size, max_seq_len).
-        num_heads (`int`, *required*):
-            number of heads
-        dtype (`torch.dtype`, *optional*, default=`torch.bfloat16`):
-            dtype of the output tensor
-    """
-    batch_size = attention_mask.size()[0]
-    max_seq_len = attention_mask.size()[1]
-    alibi = slopes.unsqueeze(1).unsqueeze(1) * torch.arange(max_seq_len, device=attention_mask.device).unsqueeze(
-        0
-    ).unsqueeze(0).expand(num_heads, -1, -1)
-
-    # Select the part of the tensor that corresponds to our tensor parallel index.
-    tp_world_size = int(os.environ.get("WORLD_SIZE", 1))
-    tp_index = int(os.environ.get("RANK", 0))
-    alibi = alibi.reshape((tp_world_size, -1, *alibi.shape[1:]))[tp_index]
+    if self.rotary_dim is not None:
+        k_rot = key[:, :, :, : self.rotary_dim]
+        k_pass = key[:, :, :, self.rotary_dim :]
 
-    alibi = alibi.repeat(batch_size, 1, 1)
-    return alibi.to(dtype)
+        q_rot = query[:, :, :, : self.rotary_dim]
+        q_pass = query[:, :, :, self.rotary_dim :]
 
+        k_rot = apply_rotary_pos_emb(k_rot, sin, cos)
+        q_rot = apply_rotary_pos_emb(q_rot, sin, cos)
 
-def gaudi_dropout_add(x: torch.Tensor, residual: torch.Tensor, prob: float, training: bool) -> torch.Tensor:
-    """
-    Dropout add function
-    Args:
-        x (`torch.tensor`, *required*):
-            input tensor
-        residual (`torch.tensor`, *required*):
-            esidual tensor
-        prob (`float`, *required*):
-            dropout probability
-        training (`bool`, *required*):
-            training mode
-    """
-    out = F.dropout(x, p=prob, training=training) if training else x
-    out = residual + out
-    return out
+        key = torch.cat([k_rot, k_pass], dim=-1)
+        query = torch.cat([q_rot, q_pass], dim=-1)
+    else:
+        key = apply_rotary_pos_emb(key, sin, cos)
+        query = apply_rotary_pos_emb(query, sin, cos)
 
+    key = key.permute(0, 2, 1, 3)
+    query = query.permute(0, 2, 1, 3)
 
-def gaudi_bloom_attention_forward(
-    self,
-    hidden_states: torch.Tensor,
-    residual: torch.Tensor,
-    alibi: torch.Tensor,
-    attention_mask: torch.Tensor,
-    layer_past: Optional[Tuple[torch.Tensor, torch.Tensor]] = None,
-    head_mask: Optional[torch.Tensor] = None,
-    use_cache: bool = False,
-    output_attentions: bool = False,
-    token_idx=None,
-):
-    fused_qkv = self.query_key_value(hidden_states)  # [batch_size, seq_length, 3 x hidden_size]
-
-    # 3 x [batch_size, seq_length, num_heads, head_dim]
-    (query_layer, key_layer, value_layer) = self._split_heads(fused_qkv)
-
-    batch_size, q_length, _, _ = query_layer.shape
-
-    query_layer = query_layer.transpose(1, 2).reshape(batch_size * self.num_heads, q_length, self.head_dim)
-    key_layer = (
-        key_layer.permute(0, 2, 3, 1).reshape(batch_size * self.num_heads, self.head_dim, q_length).contiguous()
-    )
-    value_layer = value_layer.transpose(1, 2).reshape(batch_size * self.num_heads, q_length, self.head_dim)
     if layer_past is not None:
-        past_key, past_value = layer_past
-        # concatenate along seq_length dimension:
-        #  - key: [batch_size * self.num_heads, head_dim, kv_length]
-        #  - value: [batch_size * self.num_heads, kv_length, head_dim]
+        past_key = layer_past[0]
+        past_value = layer_past[1]
+
         if token_idx is not None:
             # HPU bug WA
-            past_key.index_add_(2, token_idx - 1, key_layer - torch.index_select(past_key, 2, token_idx - 1))
-            past_value.index_add_(1, token_idx - 1, value_layer - torch.index_select(past_value, 1, token_idx - 1))
-            key_layer = past_key
-            value_layer = past_value
+            past_key.index_add_(2, token_idx - 1, key - torch.index_select(past_key, 2, token_idx - 1))
+            past_value.index_add_(2, token_idx - 1, value - torch.index_select(past_value, 2, token_idx - 1))
+            key = past_key
+            value = past_value
         else:
-            key_layer = torch.cat((past_key, key_layer), dim=2)
-            value_layer = torch.cat((past_value, value_layer), dim=1)
-
-    _, _, kv_length = key_layer.shape
+            key = torch.cat([past_key, key], dim=-2)
+            value = torch.cat([past_value, value], dim=-2)
 
     if use_cache is True:
-        present = (key_layer, value_layer)
+        present = (key, value)
     else:
         present = None
 
-    # [batch_size * num_heads, q_length, kv_length]
-    # we use `torch.Tensor.baddbmm` instead of `torch.baddbmm` as the latter isn't supported by TorchScript v1.11
-    matmul_result = alibi.baddbmm(
-        batch1=query_layer,
-        batch2=key_layer,
-        beta=self.beta,
-        alpha=self.inv_norm_factor,
-    )
+    # compute self-attention: V x Softmax(QK^T)
+    attn_output, attn_weights = self._attn(query, key, value, attention_mask, head_mask)
 
-    # change view to [batch_size, num_heads, q_length, kv_length]
-    attention_scores = matmul_result.view(batch_size, self.num_heads, q_length, kv_length)
+    attn_output = self._merge_heads(attn_output, self.num_attention_heads, self.head_dim)
+    attn_output = self.out_proj(attn_output)
+    attn_output = self.resid_dropout(attn_output)
 
-    # cast attention scores to fp32, compute scaled softmax and cast back to initial dtype - [batch_size, num_heads, q_length, kv_length]
-    input_dtype = attention_scores.dtype
-    attn_weights = torch.masked_fill(attention_scores, attention_mask, torch.finfo(attention_scores.dtype).min)
-    attention_probs = F.softmax(attn_weights, dim=-1, dtype=torch.float32).to(input_dtype)
-
-    # [batch_size, num_heads, q_length, kv_length]
-    if self.training:
-        attention_probs = self.attention_dropout(attention_probs)
-
-    if head_mask is not None:
-        attention_probs = attention_probs * head_mask
-
-    # change view [batch_size x num_heads, q_length, kv_length]
-    attention_probs_reshaped = attention_probs.view(batch_size * self.num_heads, q_length, kv_length)
-
-    # matmul: [batch_size * num_heads, q_length, head_dim]
-    context_layer = torch.bmm(attention_probs_reshaped, value_layer)
-
-    # change view [batch_size, num_heads, q_length, head_dim]
-    context_layer = self._merge_heads(context_layer)
-
-    # aggregate results across tp ranks. See here: https://github.com/pytorch/pytorch/issues/76232
-    if self.pretraining_tp > 1 and self.slow_but_exact:
-        slices = self.hidden_size / self.pretraining_tp
-        output_tensor = torch.zeros_like(context_layer)
-        for i in range(self.pretraining_tp):
-            output_tensor = output_tensor + F.linear(
-                context_layer[:, :, int(i * slices) : int((i + 1) * slices)],
-                self.dense.weight[:, int(i * slices) : int((i + 1) * slices)],
-            )
-    else:
-        output_tensor = self.dense(context_layer)
-
-    output_tensor = gaudi_dropout_add(output_tensor, residual, self.hidden_dropout, self.training)
-
-    outputs = (output_tensor, present)
+    outputs = (attn_output, present)
     if output_attentions:
-        outputs += (attention_probs,)
-
-    return outputs
+        outputs += (attn_weights,)
 
+    return outputs  # a, present, (attentions)
 
-class GaudiBloomMLP(BloomMLP):
-    def __init__(self, config):
-        super().__init__(config)
-        self.gelu_impl = torch.nn.GELU(approximate="tanh")
 
-
-def gaudi_bloom_block_forward(
+def gaudi_gptj_block_forward(
     self,
-    hidden_states: torch.Tensor,
-    alibi: torch.Tensor,
-    attention_mask: torch.Tensor,
-    layer_past: Optional[Tuple[torch.Tensor, torch.Tensor]] = None,
-    head_mask: Optional[torch.Tensor] = None,
-    use_cache: bool = False,
-    output_attentions: bool = False,
-    token_idx=None,
-):
-    # hidden_states: [batch_size, seq_length, hidden_size]
-
-    # Layer norm at the beginning of the transformer layer.
-    layernorm_output = self.input_layernorm(hidden_states)
-
-    # Layer norm post the self attention.
-    if self.apply_residual_connection_post_layernorm:
-        residual = layernorm_output
-    else:
-        residual = hidden_states
-
-    # Self attention.
-    attn_outputs = self.self_attention(
-        layernorm_output,
-        residual,
+    hidden_states: Optional[torch.FloatTensor],
+    layer_past: Optional[Tuple[torch.Tensor]] = None,
+    attention_mask: Optional[torch.FloatTensor] = None,
+    position_ids: Optional[torch.LongTensor] = None,
+    head_mask: Optional[torch.FloatTensor] = None,
+    use_cache: Optional[bool] = False,
+    output_attentions: Optional[bool] = False,
+    token_idx: Optional[torch.Tensor] = None,
+) -> Union[Tuple[torch.Tensor], Optional[Tuple[torch.Tensor, Tuple[torch.FloatTensor, ...]]]]:
+    """
+    Copied from GPTJBlock.forward: https://github.com/huggingface/transformers/blob/main/src/transformers/models/gptj/modeling_gptj.py
+    The only differences are:
+    - add new args token_idx
+    """
+    residual = hidden_states
+    hidden_states = self.ln_1(hidden_states)
+    attn_outputs = self.attn(
+        hidden_states=hidden_states,
         layer_past=layer_past,
         attention_mask=attention_mask,
-        alibi=alibi,
+        position_ids=position_ids,
         head_mask=head_mask,
         use_cache=use_cache,
         output_attentions=output_attentions,
         token_idx=token_idx,
     )
-
-    attention_output = attn_outputs[0]
-
+    attn_output = attn_outputs[0]  # output_attn: a, present, (attentions)
     outputs = attn_outputs[1:]
 
-    layernorm_output = self.post_attention_layernorm(attention_output)
-
-    # Get residual
-    if self.apply_residual_connection_post_layernorm:
-        residual = layernorm_output
-    else:
-        residual = attention_output
-
-    # MLP.
-    output = self.mlp(layernorm_output, residual)
+    feed_forward_hidden_states = self.mlp(hidden_states)
+    hidden_states = attn_output + feed_forward_hidden_states + residual
 
     if use_cache:
-        outputs = (output,) + outputs
+        outputs = (hidden_states,) + outputs
     else:
-        outputs = (output,) + outputs[1:]
+        outputs = (hidden_states,) + outputs[1:]
 
-    return outputs  # hidden_states, present, attentions
+    return outputs  # hidden_states, present, (attentions)
 
 
-class GaudiBloomModel(BloomModel):
-    def __init__(self, config):
-        super().__init__(config)
-        self.register_buffer("alibi_slope", build_alibi_slope_tensor(self.num_heads), persistent=False)
-
-    def forward(
-        self,
-        input_ids: Optional[torch.LongTensor] = None,
-        past_key_values: Optional[Tuple[Tuple[torch.Tensor, torch.Tensor], ...]] = None,
-        attention_mask: Optional[torch.Tensor] = None,
-        head_mask: Optional[torch.LongTensor] = None,
-        inputs_embeds: Optional[torch.LongTensor] = None,
-        use_cache: Optional[bool] = None,
-        output_attentions: Optional[bool] = None,
-        output_hidden_states: Optional[bool] = None,
-        return_dict: Optional[bool] = None,
-        token_idx=None,
-        **deprecated_arguments,
-    ) -> Union[Tuple[torch.Tensor, ...], BaseModelOutputWithPastAndCrossAttentions]:
-        if deprecated_arguments.pop("position_ids", False) is not False:
-            # `position_ids` could have been `torch.Tensor` or `None` so defaulting pop to `False` allows to detect if users were passing explicitly `None`
-            warnings.warn(
-                "`position_ids` have no functionality in BLOOM and will be removed in v5.0.0. You can safely ignore"
-                " passing `position_ids`.",
-                FutureWarning,
-            )
-        if len(deprecated_arguments) > 0:
-            raise ValueError(f"Got unexpected arguments: {deprecated_arguments}")
-
-        output_attentions = output_attentions if output_attentions is not None else self.config.output_attentions
-        output_hidden_states = (
-            output_hidden_states if output_hidden_states is not None else self.config.output_hidden_states
-        )
-        use_cache = use_cache if use_cache is not None else self.config.use_cache
-        return_dict = return_dict if return_dict is not None else self.config.use_return_dict
-
-        if input_ids is not None and inputs_embeds is not None:
-            raise ValueError("You cannot specify both input_ids and inputs_embeds at the same time")
-        elif input_ids is not None:
-            batch_size, seq_length = input_ids.shape
-        elif inputs_embeds is not None:
-            batch_size, seq_length, _ = inputs_embeds.shape
-        else:
-            raise ValueError("You have to specify either input_ids or inputs_embeds")
-
-        if past_key_values is None:
-            past_key_values = tuple([None] * len(self.h))
+def gaudi_gptj_model_forward(
+    self,
+    input_ids: Optional[torch.LongTensor] = None,
+    past_key_values: Optional[Tuple[Tuple[torch.Tensor]]] = None,
+    attention_mask: Optional[torch.FloatTensor] = None,
+    token_type_ids: Optional[torch.LongTensor] = None,
+    position_ids: Optional[torch.LongTensor] = None,
+    head_mask: Optional[torch.FloatTensor] = None,
+    inputs_embeds: Optional[torch.FloatTensor] = None,
+    use_cache: Optional[bool] = None,
+    output_attentions: Optional[bool] = None,
+    output_hidden_states: Optional[bool] = None,
+    return_dict: Optional[bool] = None,
+    token_idx: Optional[torch.Tensor] = None,
+) -> Union[Tuple, BaseModelOutputWithPast]:
+    """
+    Copied from GPTJModel.forward: https://github.com/huggingface/transformers/blob/main/src/transformers/models/gptj/modeling_gptj.py
+    The only differences are:
+    - add new args token_idx
+    """
+    output_attentions = output_attentions if output_attentions is not None else self.config.output_attentions
+    output_hidden_states = (
+        output_hidden_states if output_hidden_states is not None else self.config.output_hidden_states
+    )
+    use_cache = use_cache if use_cache is not None else self.config.use_cache
+    return_dict = return_dict if return_dict is not None else self.config.use_return_dict
 
-        # Prepare head mask if needed
-        # 1.0 in head_mask indicate we keep the head
-        # attention_probs has shape batch_size x num_heads x N x N
-        # head_mask has shape n_layer x batch x num_heads x N x N
-        head_mask = self.get_head_mask(head_mask, self.config.n_layer)
-
-        if inputs_embeds is None:
-            inputs_embeds = self.word_embeddings(input_ids)
-
-        hidden_states = self.word_embeddings_layernorm(inputs_embeds)
-
-        presents = () if use_cache else None
-        all_self_attentions = () if output_attentions else None
-        all_hidden_states = () if output_hidden_states else None
-
-        # Compute alibi tensor: check gaudi_bloom_build_alibi_tensor
-        seq_length_with_past = seq_length
-        past_key_values_length = 0
-        if past_key_values[0] is not None:
-            past_key_values_length = past_key_values[0][0].shape[2]
-            seq_length_with_past = seq_length_with_past + past_key_values_length
-        if attention_mask is None:
-            attention_mask = torch.ones((batch_size, seq_length_with_past), device=hidden_states.device)
-        else:
-            attention_mask = attention_mask.to(hidden_states.device)
+    if input_ids is not None and inputs_embeds is not None:
+        raise ValueError("You cannot specify both input_ids and inputs_embeds at the same time")
+    elif input_ids is not None:
+        input_shape = input_ids.size()
+        input_ids = input_ids.view(-1, input_shape[-1])
+        batch_size = input_ids.shape[0]
+    elif inputs_embeds is not None:
+        input_shape = inputs_embeds.size()[:-1]
+        batch_size = inputs_embeds.shape[0]
+    else:
+        raise ValueError("You have to specify either input_ids or inputs_embeds")
 
-        alibi = gaudi_bloom_build_alibi_tensor(attention_mask, self.alibi_slope, self.num_heads, hidden_states.dtype)
+    device = input_ids.device if input_ids is not None else inputs_embeds.device
 
-        causal_mask = self._prepare_attn_mask(
-            attention_mask,
-            input_shape=(batch_size, seq_length),
-            past_key_values_length=past_key_values_length,
-        )
+    if token_type_ids is not None:
+        token_type_ids = token_type_ids.view(-1, input_shape[-1])
 
-        for i, (block, layer_past) in enumerate(zip(self.h, past_key_values)):
-            if output_hidden_states:
-                all_hidden_states = all_hidden_states + (hidden_states,)
-
-            if self.gradient_checkpointing and self.training:
-                if use_cache:
-                    logger.warning(
-                        "`use_cache=True` is incompatible with gradient checkpointing. Setting `use_cache=False`..."
-                    )
-                    use_cache = False
-
-                def create_custom_forward(module):
-                    def custom_forward(*inputs):
-                        # None for past_key_value
-                        return module(*inputs, use_cache=use_cache, output_attentions=output_attentions)
-
-                    return custom_forward
-
-                outputs = torch.utils.checkpoint.checkpoint(
-                    create_custom_forward(block),
-                    hidden_states,
-                    alibi,
-                    causal_mask,
-                    head_mask[i],
-                )
-            else:
-                outputs = block(
-                    hidden_states,
-                    layer_past=layer_past,
-                    attention_mask=causal_mask,
-                    head_mask=head_mask[i],
-                    use_cache=use_cache,
-                    output_attentions=output_attentions,
-                    alibi=alibi,
-                    token_idx=token_idx,
-                )
-
-            hidden_states = outputs[0]
-            if use_cache is True:
-                presents = presents + (outputs[1],)
+    if position_ids is not None:
+        position_ids = position_ids.view(-1, input_shape[-1]).long()
 
-            if output_attentions:
-                all_self_attentions = all_self_attentions + (outputs[2 if use_cache else 1],)
+    if past_key_values is None:
+        past_length = 0
+        past_key_values = tuple([None] * len(self.h))
+    else:
+        past_length = past_key_values[0][0].size(-2)
 
-        # Add last hidden state
-        hidden_states = self.ln_f(hidden_states)
+    if position_ids is None:
+        position_ids = torch.arange(past_length, input_shape[-1] + past_length, dtype=torch.long, device=device)
+        position_ids = position_ids.unsqueeze(0).view(-1, input_shape[-1])
+
+    # Attention mask.
+    if attention_mask is not None:
+        if batch_size <= 0:
+            raise ValueError("batch_size has to be defined and > 0")
+        attention_mask = attention_mask.view(batch_size, -1)
+        # We create a 3D attention mask from a 2D tensor mask.
+        # Sizes are [batch_size, 1, 1, to_seq_length]
+        # So we can broadcast to [batch_size, num_heads, from_seq_length, to_seq_length]
+        # this attention mask is more simple than the triangular masking of causal attention
+        # used in OpenAI GPT, we just need to prepare the broadcast dimension here.
+        attention_mask = attention_mask[:, None, None, :]
+
+        # Since attention_mask is 1.0 for positions we want to attend and 0.0 for
+        # masked positions, this operation will create a tensor which is 0.0 for
+        # positions we want to attend and the dtype's smallest value for masked positions.
+        # Since we are adding it to the raw scores before the softmax, this is
+        # effectively the same as removing these entirely.
+        attention_mask = attention_mask.to(dtype=self.dtype)  # fp16 compatibility
+        attention_mask = (1.0 - attention_mask) * torch.finfo(self.dtype).min
+
+    # Prepare head mask if needed
+    # 1.0 in head_mask indicate we keep the head
+    # attention_probs has shape bsz x num_attention_heads x N x N
+    # head_mask has shape n_layer x batch x num_attention_heads x N x N
+    head_mask = self.get_head_mask(head_mask, self.config.n_layer)
+
+    if inputs_embeds is None:
+        inputs_embeds = self.wte(input_ids)
+
+    hidden_states = inputs_embeds
+
+    if token_type_ids is not None:
+        token_type_embeds = self.wte(token_type_ids)
+        hidden_states = hidden_states + token_type_embeds
+
+    hidden_states = self.drop(hidden_states)
+
+    output_shape = input_shape + (hidden_states.size(-1),)
+
+    if self.gradient_checkpointing and self.training:
+        if use_cache:
+            logger.warning_once(
+                "`use_cache=True` is incompatible with gradient checkpointing. Setting `use_cache=False`..."
+            )
+            use_cache = False
 
+    presents = () if use_cache else None
+    all_self_attentions = () if output_attentions else None
+    all_hidden_states = () if output_hidden_states else None
+    for i, (block, layer_past) in enumerate(zip(self.h, past_key_values)):
+        # Model parallel
+        if self.model_parallel:
+            torch.cuda.set_device(hidden_states.device)
+            # Ensure layer_past is on same device as hidden_states (might not be correct)
+            if layer_past is not None:
+                layer_past = tuple(past_state.to(hidden_states.device) for past_state in layer_past)
+            # Ensure that attention_mask is always on the same device as hidden_states
+            if attention_mask is not None:
+                attention_mask = attention_mask.to(hidden_states.device)
+            if isinstance(head_mask, torch.Tensor):
+                head_mask = head_mask.to(hidden_states.device)
         if output_hidden_states:
             all_hidden_states = all_hidden_states + (hidden_states,)
 
-        if not return_dict:
-            return tuple(v for v in [hidden_states, presents, all_hidden_states, all_self_attentions] if v is not None)
+        if self.gradient_checkpointing and self.training:
 
-        return BaseModelOutputWithPastAndCrossAttentions(
-            last_hidden_state=hidden_states,
-            past_key_values=presents,
-            hidden_states=all_hidden_states,
-            attentions=all_self_attentions,
-        )
+            def create_custom_forward(module):
+                def custom_forward(*inputs):
+                    # None for past_key_value
+                    return module(*inputs, use_cache, output_attentions)
+
+                return custom_forward
+
+            outputs = torch.utils.checkpoint.checkpoint(
+                create_custom_forward(block),
+                hidden_states,
+                None,
+                attention_mask,
+                position_ids,
+                head_mask[i],
+            )
+        else:
+            outputs = block(
+                hidden_states=hidden_states,
+                layer_past=layer_past,
+                attention_mask=attention_mask,
+                position_ids=position_ids,
+                head_mask=head_mask[i],
+                use_cache=use_cache,
+                output_attentions=output_attentions,
+                token_idx=token_idx,
+            )
 
+        hidden_states = outputs[0]
+        if use_cache is True:
+            presents = presents + (outputs[1],)
+
+        if output_attentions:
+            all_self_attentions = all_self_attentions + (outputs[2 if use_cache else 1],)
+
+        # Model Parallel: If it's the last layer for that device, put things on the next device
+        if self.model_parallel:
+            for k, v in self.device_map.items():
+                if i == v[-1] and "cuda:" + str(k) != self.last_device:
+                    hidden_states = hidden_states.to("cuda:" + str(k + 1))
+
+    hidden_states = self.ln_f(hidden_states)
+
+    hidden_states = hidden_states.view(output_shape)
+    # Add last hidden state
+    if output_hidden_states:
+        all_hidden_states = all_hidden_states + (hidden_states,)
+
+    if not return_dict:
+        return tuple(v for v in [hidden_states, presents, all_hidden_states, all_self_attentions] if v is not None)
+
+    return BaseModelOutputWithPast(
+        last_hidden_state=hidden_states,
+        past_key_values=presents,
+        hidden_states=all_hidden_states,
+        attentions=all_self_attentions,
+    )
 
-class GaudiBloomForCausalLM(BloomForCausalLM):
-    def __init__(self, config):
-        super().__init__(config)
-        self.lm_head_chunks = []
-
-    def split_lm_head(self):
-        N = 2
-        self.lm_head_chunks = [c.t() for c in self.lm_head.weight.chunk(N, dim=0)]
+
+class GaudiGPTJForCausalLM(GPTJForCausalLM):
+    """
+    Inherits from GPTJForCausalLM: https://github.com/huggingface/transformers/blob/main/src/transformers/models/gptj/modeling_gptj.py
+    The only differences are:
+    - add new args token_idx
+    - add token_idx into model_inputs
+    - from step2 when enable KV cache, slice next_input_ids from input_ids base on the token_idx
+    - from step2 when enable KV cache, slice next_position_ids from position_ids base on the token_idx
+    - from step2 when enable KV cache, slice next_token_type_ids from token_type_ids base on the token_idx
+    """
 
     def prepare_inputs_for_generation(
-        self,
-        input_ids: torch.LongTensor,
-        past_key_values: Optional[torch.Tensor] = None,
-        attention_mask: Optional[torch.Tensor] = None,
-        token_idx: Optional[torch.Tensor] = None,
-        **kwargs,
-    ) -> dict:
-        # only last token for input_ids if past is not None
+        self, input_ids, past_key_values=None, inputs_embeds=None, token_idx=None, **kwargs
+    ):
+        token_type_ids = kwargs.get("token_type_ids", None)
+        # only last token for inputs_ids if past is defined in kwargs
         if past_key_values:
             if token_idx is not None:
                 input_ids = torch.index_select(input_ids, 1, token_idx - 1)
             else:
                 input_ids = input_ids[:, -1].unsqueeze(-1)
 
-            # the cache may be in the stardard format (e.g. in contrastive search), convert to bloom's format if needed
-            if past_key_values[0][0].shape[0] == input_ids.shape[0]:
-                past_key_values = self._convert_to_bloom_cache(past_key_values)
-
-        return {
-            "input_ids": input_ids,
-            "past_key_values": past_key_values,
-            "use_cache": kwargs.get("use_cache"),
-            "attention_mask": attention_mask,
-            "token_idx": token_idx,
-        }
+            if token_type_ids is not None:
+                if token_idx is not None:
+                    token_type_ids = torch.index_select(token_type_ids, 1, token_idx - 1)
+                else:
+                    token_type_ids = token_type_ids[:, -1].unsqueeze(-1)
+
+        attention_mask = kwargs.get("attention_mask", None)
+        position_ids = kwargs.get("position_ids", None)
+
+        if attention_mask is not None and position_ids is None:
+            # create position_ids on the fly for batch generation
+            position_ids = attention_mask.long().cumsum(-1) - 1
+            position_ids.masked_fill_(attention_mask == 0, 1)
+            if past_key_values:
+                if token_idx is not None:
+                    position_ids = torch.index_select(position_ids, 1, token_idx - 1)
+                else:
+                    position_ids = position_ids[:, -1].unsqueeze(-1)
+
+        # if `inputs_embeds` are passed, we only want to use them in the 1st generation step
+        if inputs_embeds is not None and past_key_values is None:
+            model_inputs = {"inputs_embeds": inputs_embeds}
+        else:
+            model_inputs = {"input_ids": input_ids}
+
+        model_inputs.update(
+            {
+                "past_key_values": past_key_values,
+                "use_cache": kwargs.get("use_cache"),
+                "position_ids": position_ids,
+                "attention_mask": attention_mask,
+                "token_type_ids": token_type_ids,
+                "token_idx": token_idx,
+            }
+        )
+
+        return model_inputs
 
     def forward(
         self,
         input_ids: Optional[torch.LongTensor] = None,
-        past_key_values: Optional[Tuple[Tuple[torch.Tensor, torch.Tensor], ...]] = None,
-        attention_mask: Optional[torch.Tensor] = None,
-        head_mask: Optional[torch.Tensor] = None,
-        inputs_embeds: Optional[torch.Tensor] = None,
-        labels: Optional[torch.Tensor] = None,
+        past_key_values: Optional[Tuple[Tuple[torch.Tensor]]] = None,
+        attention_mask: Optional[torch.FloatTensor] = None,
+        token_type_ids: Optional[torch.LongTensor] = None,
+        position_ids: Optional[torch.LongTensor] = None,
+        head_mask: Optional[torch.FloatTensor] = None,
+        inputs_embeds: Optional[torch.FloatTensor] = None,
+        labels: Optional[torch.LongTensor] = None,
         use_cache: Optional[bool] = None,
         output_attentions: Optional[bool] = None,
         output_hidden_states: Optional[bool] = None,
         return_dict: Optional[bool] = None,
-        token_idx: Optional[bool] = None,
-        **deprecated_arguments,
-    ) -> Union[Tuple[torch.Tensor], CausalLMOutputWithCrossAttentions]:
+        token_idx: Optional[torch.Tensor] = None,
+    ) -> Union[Tuple, CausalLMOutputWithPast]:
         r"""
         labels (`torch.LongTensor` of shape `(batch_size, sequence_length)`, *optional*):
             Labels for language modeling. Note that the labels **are shifted** inside the model, i.e. you can set
             `labels = input_ids` Indices are selected in `[-100, 0, ..., config.vocab_size]` All labels set to `-100`
             are ignored (masked), the loss is only computed for labels in `[0, ..., config.vocab_size]`
         """
-        if deprecated_arguments.pop("position_ids", False) is not False:
-            # `position_ids` could have been `torch.Tensor` or `None` so defaulting pop to `False` allows to detect if users were passing explicitly `None`
-            warnings.warn(
-                "`position_ids` have no functionality in BLOOM and will be removed in v5.0.0. You can safely ignore"
-                " passing `position_ids`.",
-                FutureWarning,
-            )
-        if len(deprecated_arguments) > 0:
-            raise ValueError(f"Got unexpected arguments: {deprecated_arguments}")
-
         return_dict = return_dict if return_dict is not None else self.config.use_return_dict
 
         transformer_outputs = self.transformer(
             input_ids,
             past_key_values=past_key_values,
             attention_mask=attention_mask,
+            token_type_ids=token_type_ids,
+            position_ids=position_ids,
             head_mask=head_mask,
             inputs_embeds=inputs_embeds,
             use_cache=use_cache,
             output_attentions=output_attentions,
             output_hidden_states=output_hidden_states,
             return_dict=return_dict,
             token_idx=token_idx,
         )
         hidden_states = transformer_outputs[0]
 
-        if len(self.lm_head_chunks) > 0:
-            lm_logits = torch.cat([torch.matmul(hidden_states, c) for c in self.lm_head_chunks], dim=-1)
-        else:
-            lm_logits = self.lm_head(hidden_states)
+        # Set device for model parallelism
+        if self.model_parallel:
+            torch.cuda.set_device(self.transformer.first_device)
+            hidden_states = hidden_states.to(self.lm_head.weight.device)
+
+        # make sure sampling in fp16 works correctly and
+        # compute loss in fp32 to match with mesh-tf version
+        # https://github.com/EleutherAI/gpt-neo/blob/89ce74164da2fb16179106f54e2269b5da8db333/models/gpt2/gpt2.py#L179
+        lm_logits = self.lm_head(hidden_states).to(torch.float32)
 
         loss = None
         if labels is not None:
-            # move labels to correct device to enable model parallelism
-            labels = labels.to(lm_logits.device)
             # Shift so that tokens < n predict n
             shift_logits = lm_logits[..., :-1, :].contiguous()
             shift_labels = labels[..., 1:].contiguous()
-            batch_size, seq_length, vocab_size = shift_logits.shape
             # Flatten the tokens
             loss_fct = CrossEntropyLoss()
-            loss = loss_fct(
-                shift_logits.view(batch_size * seq_length, vocab_size), shift_labels.view(batch_size * seq_length)
-            )
+            loss = loss_fct(shift_logits.view(-1, shift_logits.size(-1)), shift_labels.view(-1))
+
+            loss = loss.to(hidden_states.dtype)
 
         if not return_dict:
             output = (lm_logits,) + transformer_outputs[1:]
             return ((loss,) + output) if loss is not None else output
 
-        return CausalLMOutputWithCrossAttentions(
+        return CausalLMOutputWithPast(
             loss=loss,
             logits=lm_logits,
             past_key_values=transformer_outputs.past_key_values,
             hidden_states=transformer_outputs.hidden_states,
             attentions=transformer_outputs.attentions,
         )
```

### Comparing `optimum-habana-1.5.1/optimum/habana/transformers/models/modeling_all_models.py` & `optimum-habana-1.6.0/optimum/habana/transformers/models/modeling_all_models.py`

 * *Files 10% similar despite different names*

```diff
@@ -89,7 +89,22 @@
     # effectively the same as removing these entirely.
     # torch.finfo must take the dtype of encoder_extended_attention_mask
     extended_attention_mask = extended_attention_mask.to(dtype=dtype)  # bf16 compatibility
     extended_attention_mask = 1.0 - extended_attention_mask
     extended_attention_mask = extended_attention_mask * torch.finfo(extended_attention_mask.dtype).min
 
     return extended_attention_mask
+
+
+def gaudi_conv1d_forward(self, x):
+    """
+    Same as https://github.com/huggingface/transformers/blob/3335724376319a0c453049d0cd883504f530ff52/src/transformers/pytorch_utils.py#L100
+    but moves reshape before view for tpc auto fusion.
+    """
+    size_out = x.size()[:-1] + (self.nf,)
+    x = torch.mm(x.view(-1, x.size(-1)), self.weight)
+    x = x.view(size_out)
+    bias_shape = [1 for _ in x.shape]
+    bias_shape[-1] = self.nf
+    bias = self.bias.view(bias_shape)
+    x = x + bias
+    return x
```

### Comparing `optimum-habana-1.5.1/optimum/habana/transformers/models/vit/modeling_vit.py` & `optimum-habana-1.6.0/optimum/habana/transformers/models/vit/modeling_vit.py`

 * *Files identical despite different names*

### Comparing `optimum-habana-1.5.1/optimum/habana/transformers/models/wav2vec2/modeling_wav2vec2.py` & `optimum-habana-1.6.0/optimum/habana/transformers/models/wav2vec2/modeling_wav2vec2.py`

 * *Files identical despite different names*

### Comparing `optimum-habana-1.5.1/optimum/habana/transformers/trainer.py` & `optimum-habana-1.6.0/optimum/habana/transformers/trainer.py`

 * *Files 3% similar despite different names*

```diff
@@ -18,14 +18,15 @@
 import os
 import random
 import shutil
 import sys
 import tempfile
 import time
 import warnings
+from collections.abc import Mapping
 from typing import TYPE_CHECKING, Any, Callable, Dict, List, Optional, Tuple, Union
 
 import numpy as np
 import torch
 from packaging import version
 from torch.utils.data import DataLoader, Dataset, RandomSampler
 from torch.utils.data.distributed import DistributedSampler
@@ -74,17 +75,19 @@
     CONFIG_NAME,
     SAFE_WEIGHTS_NAME,
     WEIGHTS_NAME,
     is_datasets_available,
     is_safetensors_available,
 )
 
+from optimum.habana.distributed import all_reduce_gradients
 from optimum.utils import logging
 
 from ..utils import (
+    HabanaProfile,
     get_hpu_memory_stats,
     set_seed,
     speed_metrics,
     to_device_dtype,
 )
 from .deepspeed import deepspeed_init
 from .gaudi_configuration import GAUDI_CONFIG_NAME, GaudiConfig
@@ -137,14 +140,26 @@
         preprocess_logits_for_metrics: Optional[Callable[[torch.Tensor, torch.Tensor], torch.Tensor]] = None,
     ):
         if args is None:
             output_dir = "tmp_trainer"
             logger.info(f"No `GaudiTrainingArguments` passed, using `output_dir={output_dir}`.")
             args = GaudiTrainingArguments(output_dir=output_dir)
 
+        self.use_hpu_amp = False
+        self.use_cpu_amp = False
+        if args.bf16 and not args.deepspeed:
+            if args.half_precision_backend == "hpu_amp":
+                self.use_hpu_amp = True
+            else:
+                self.use_cpu_amp = True
+
+            # Workaround to not set amp backend again when calling super().__init__(...)
+            # args.bf16 is not used after the __init__ anyway
+            args.bf16 = False
+
         super().__init__(
             model,
             args,
             data_collator,
             train_dataset,
             eval_dataset,
             tokenizer,
@@ -165,26 +180,40 @@
                 try:
                     import habana_frameworks.torch.core as htcore
                 except ImportError as error:
                     error.msg = f"Could not import habana_frameworks.torch.core. {error.msg}."
                     raise error
                 self.htcore = htcore
 
-            if self.args.use_hpu_graphs:
+            if self.args.use_hpu_graphs_for_inference:
                 self.already_wrapped_for_hpu_graphs = False
 
             if self.args.deepspeed:
-                # Habana's fused ADAM is not compatible with DeepSpeed yet
-                self.gaudi_config.use_fused_adam = False
-                # HMP must be set to True when using DeepSpeed
-                self.gaudi_config.use_habana_mixed_precision = True
+                # Mixed-precision backends are turned off when using DeepSpeed since it manages this itself
+                self.gaudi_config.use_habana_mixed_precision = False
+                self.gaudi_config.use_torch_autocast = False
+                self.use_hpu_amp = False
+
+            if self.args.deepspeed or self.args.dataloader_num_workers >= 1:
                 # To avoid warnings about parallelism in tokenizers
                 os.environ["TOKENIZERS_PARALLELISM"] = "false"
 
-            if self.gaudi_config.use_habana_mixed_precision:
+            if self.gaudi_config.use_torch_autocast:
+                if not self.use_hpu_amp and not self.use_cpu_amp:
+                    self.use_hpu_amp = True
+                    logger.warning(
+                        "The argument `--bf16` was not given but `use_torch_autocast` is True in the Gaudi configuration so mixed-precision training with Torch Autocast is enabled."
+                    )
+            elif self.gaudi_config.use_habana_mixed_precision and self.use_hpu_amp:
+                self.gaudi_config.use_habana_mixed_precision = False
+                logger.warning(
+                    "`--bf16` was given and `use_habana_mixed_precision` is True in the Gaudi configuration. Using Torch Autocast as mixed-precision backend."
+                )
+
+            if self.gaudi_config.use_habana_mixed_precision and not (self.use_hpu_amp or self.use_cpu_amp):
                 try:
                     from habana_frameworks.torch.hpex import hmp
                 except ImportError as error:
                     error.msg = f"Could not import habana_frameworks.torch.hpex. {error.msg}."
                     raise error
                 self.hmp = hmp
 
@@ -381,15 +410,15 @@
             return model
 
         # Note: in torch.distributed mode, there's no point in wrapping the model
         # inside a DistributedDataParallel as we'll be under `no_grad` anyways.
         if not training:
             return model
 
-        if self.args.local_rank != -1:
+        if self.args.local_rank != -1 and self.args.distribution_strategy == "ddp":
             kwargs = {}
 
             kwargs["find_unused_parameters"] = self.args.ddp_find_unused_parameters
             if self.args.ddp_find_unused_parameters and self.args.gradient_checkpointing:
                 logger.warning(
                     "ddp_find_unused_parameters and gradient_checkpointing are both True, which may lead to an error:"
                     " https://github.com/huggingface/transformers/pull/4659#issuecomment-643356021"
@@ -402,21 +431,69 @@
             model = torch.nn.parallel.DistributedDataParallel(
                 model,
                 device_ids=[self.args.local_rank] if self.args._n_gpu != 0 and not self.args.use_habana else None,
                 output_device=self.args.local_rank if self.args._n_gpu != 0 and not self.args.use_habana else None,
                 **kwargs,
             )
 
+        if self.args.use_hpu_graphs_for_training:
+            import habana_frameworks.torch as ht
+
+            ht.hpu.ModuleCacher()(model=model, inplace=True)
+
         # torch.compile() needs to be called after wrapping the model with FSDP or DDP
         # to ensure that it accounts for the graph breaks required by those wrappers
         if self.args.torch_compile:
             model = torch.compile(model, backend=self.args.torch_compile_backend, mode=self.args.torch_compile_mode)
 
         return model
 
+    def _maybe_log_save_evaluate(self, tr_loss, model, trial, epoch, ignore_keys_for_eval):
+        if self.args.adjust_throughput:
+            save_start = time.perf_counter()
+
+        if self.control.should_log:
+            logs: Dict[str, float] = {}
+
+            # all_gather + mean() to get average loss over all processes
+            tr_loss_scalar = self._nested_gather(tr_loss).mean().item()
+
+            # reset tr_loss to zero
+            tr_loss -= tr_loss
+            logs["loss"] = round(tr_loss_scalar / (self.state.global_step - self._globalstep_last_logged), 4)
+            logs["learning_rate"] = self._get_learning_rate()
+
+            self._total_loss_scalar += tr_loss_scalar
+            self._globalstep_last_logged = self.state.global_step
+            self.store_flos()
+
+            self.log(logs)
+
+        metrics = None
+        if self.control.should_evaluate:
+            if isinstance(self.eval_dataset, dict):
+                metrics = {}
+                for eval_dataset_name, eval_dataset in self.eval_dataset.items():
+                    dataset_metrics = self.evaluate(
+                        eval_dataset=eval_dataset,
+                        ignore_keys=ignore_keys_for_eval,
+                        metric_key_prefix=f"eval_{eval_dataset_name}",
+                    )
+                    metrics.update(dataset_metrics)
+            else:
+                metrics = self.evaluate(ignore_keys=ignore_keys_for_eval)
+            self._report_to_hp_search(trial, self.state.global_step, metrics)
+
+        if self.control.should_save:
+            self._save_checkpoint(model, trial, metrics=metrics)
+            self.control = self.callback_handler.on_save(self.args, self.state, self.control)
+
+        if self.args.adjust_throughput:
+            self.log_evaluate_save_time += time.perf_counter() - save_start
+
     def train(
         self,
         resume_from_checkpoint: Optional[Union[str, bool]] = None,
         trial: Union["optuna.Trial", Dict[str, Any]] = None,
         ignore_keys_for_eval: Optional[List[str]] = None,
         **kwargs,
     ):
@@ -495,14 +572,36 @@
         return inner_training_loop(
             args=args,
             resume_from_checkpoint=resume_from_checkpoint,
             trial=trial,
             ignore_keys_for_eval=ignore_keys_for_eval,
         )
 
+    def _prepare_input(self, data: Union[torch.Tensor, Any]) -> Union[torch.Tensor, Any]:
+        """
+        Prepares one `data` before feeding it to the model, be it a tensor or a nested list/dictionary of tensors.
+        Compared to Transformers, it is also possible to enable non-blocking data copy.
+        """
+        if isinstance(data, Mapping):
+            return type(data)({k: self._prepare_input(v) for k, v in data.items()})
+        elif isinstance(data, (tuple, list)):
+            return type(data)(self._prepare_input(v) for v in data)
+        elif isinstance(data, torch.Tensor):
+            kwargs = {"device": self.args.device}
+            if self.deepspeed and (torch.is_floating_point(data) or torch.is_complex(data)):
+                # NLP models inputs are int/uint and those get adjusted to the right dtype of the
+                # embedding. Other models such as wav2vec2's inputs are already float and thus
+                # may need special handling to match the dtypes of the model
+                kwargs.update({"dtype": self.args.hf_deepspeed_config.dtype()})
+            if self.args.non_blocking_data_copy:
+                return data.to(**kwargs, non_blocking=True)
+            else:
+                return data.to(**kwargs)
+        return data
+
     def training_step(self, model: torch.nn.Module, inputs: Dict[str, Union[torch.Tensor, Any]]) -> torch.Tensor:
         """
         Perform a training step on a batch of inputs.
 
         Subclass and override to inject custom behavior.
 
         Args:
@@ -628,14 +727,23 @@
 
                 torch.utils.checkpoint.checkpoint = hpu_deepspeed_checkpointing
             elif args.use_lazy_mode:
                 from .gradient_checkpointing import checkpoint as lazy_mode_checkpointing
 
                 torch.utils.checkpoint.checkpoint = lazy_mode_checkpointing
 
+            # HACK for gradient checkpointing with T5
+            # For T5, checkpointing is imported with `from torch.utils.checkpoint import checkpoint`: https://github.com/huggingface/transformers/blob/04ab5605fbb4ef207b10bf2772d88c53fc242e83/src/transformers/models/t5/modeling_t5.py#L27
+            # Whereas for other models we do `import torch.utils.checkpoint`
+            # So monkey patching at Torch's level does not work
+            if self.model.config.model_type == "t5":
+                import transformers.models.t5.modeling_t5 as modeling_t5
+
+                modeling_t5.checkpoint = torch.utils.checkpoint.checkpoint
+
         model = self._wrap_model(self.model_wrapped)
 
         # for the rest of this function `model` is the outside model, whether it was wrapped or not
         if model is not self.model:
             self.model_wrapped = model
 
         # Check if saved optimizer or scheduler states exist
@@ -696,14 +804,23 @@
                     "batches in the first epoch. If this takes a lot of time, you can add the `--ignore_data_skip` "
                     "flag to your launch command, but you will resume the training on data already seen by your model."
                 )
                 if self.is_local_process_zero() and not args.disable_tqdm:
                     steps_trained_progress_bar = tqdm(total=steps_trained_in_current_epoch)
                     steps_trained_progress_bar.set_description("Skipping the first batches")
 
+        # In multi-worker training: broadcast model parameters from worker:0 to all the others.
+        # This must be done manually unless DistributedDataParallel is used.
+        if self.args.local_rank != -1 and self.args.distribution_strategy == "fast_ddp":
+            logger.debug(
+                f"Broadcasting the model parameters to assure that each of {self.args.world_size} workers start the training from the same point."
+            )
+            for param in model.parameters():
+                torch.distributed.broadcast(param.data, src=0)
+
         # Update the references
         self.callback_handler.model = self.model
         self.callback_handler.optimizer = self.optimizer
         self.callback_handler.lr_scheduler = self.lr_scheduler
         self.callback_handler.train_dataloader = train_dataloader
         if self.hp_name is not None and self._trial is not None:
             # use self._trial because the SigOpt/Optuna hpo only call `_hp_search_setup(trial)` instead of passing trial
@@ -723,19 +840,15 @@
 
         # tr_loss is a tensor to avoid synchronization of TPUs through .item()
         tr_loss = torch.tensor(0.0).to(args.device)
         # _total_loss_scalar is updated everytime .item() has to be called on tr_loss and stores the sum of all losses
         self._total_loss_scalar = 0.0
         self._globalstep_last_logged = self.state.global_step
 
-        # set_to_none is not implemented for some optimizers
-        try:
-            model.zero_grad(set_to_none=True)
-        except TypeError:
-            model.zero_grad()
+        self._zero_model_grad(model)
 
         self.control = self.callback_handler.on_train_begin(args, self.state, self.control)
 
         # Skip the first epochs_trained epochs to get the random state of the dataloader at the right point.
         if not args.ignore_data_skip:
             for epoch in range(epochs_trained):
                 is_random_sampler = hasattr(train_dataloader, "sampler") and isinstance(
@@ -747,14 +860,22 @@
                     for _ in train_dataloader:
                         break
                 else:
                     # Otherwise we need to call the whooooole sampler cause there is some random operation added
                     # AT THE VERY END!
                     _ = list(train_dataloader.sampler)
 
+        if self.args.adjust_throughput:
+            self.log_evaluate_save_time = 0
+        else:
+            self.log_evaluate_save_time = None
+
+        hb_profiler = HabanaProfile(warmup=self.args.profiling_warmup_steps, active=self.args.profiling_steps)
+        hb_profiler.start()
+
         for epoch in range(epochs_trained, num_train_epochs):
             if isinstance(train_dataloader, DataLoader) and isinstance(train_dataloader.sampler, DistributedSampler):
                 train_dataloader.sampler.set_epoch(epoch)
             elif hasattr(train_dataloader, "dataset") and isinstance(train_dataloader.dataset, IterableDatasetShard):
                 train_dataloader.dataset.set_epoch(epoch)
 
             epoch_iterator = train_dataloader
@@ -770,14 +891,15 @@
             )
             self.control = self.callback_handler.on_epoch_begin(args, self.state, self.control)
 
             if epoch == epochs_trained and resume_from_checkpoint is not None and steps_trained_in_current_epoch == 0:
                 self._load_rng_state(resume_from_checkpoint)
 
             step = -1
+
             for step, inputs in enumerate(epoch_iterator):
                 if (
                     args.throughput_warmup_steps > 0
                     and (args.throughput_warmup_steps * args.gradient_accumulation_steps)
                     == epoch * steps_in_epoch + step
                 ):
                     start_time_after_warmup = time.time()
@@ -793,59 +915,72 @@
                 elif steps_trained_progress_bar is not None:
                     steps_trained_progress_bar.close()
                     steps_trained_progress_bar = None
 
                 if step % args.gradient_accumulation_steps == 0:
                     self.control = self.callback_handler.on_step_begin(args, self.state, self.control)
 
+                # Proceed with forward and backward passes.
                 if (
-                    ((step + 1) % args.gradient_accumulation_steps != 0)
+                    args.distribution_strategy == "ddp"
+                    and ((step + 1) % args.gradient_accumulation_steps != 0)
                     and args.local_rank != -1
                     and args._no_sync_in_gradient_accumulation
                 ):
                     # Avoid unnecessary DDP synchronization since there will be no backward pass on this example.
                     with model.no_sync():
                         tr_loss_step = self.training_step(model, inputs)
                 else:
                     tr_loss_step = self.training_step(model, inputs)
 
+                is_optimization_step = (step + 1) % args.gradient_accumulation_steps == 0 or (
+                    # last step in epoch but step is always smaller than gradient_accumulation_steps
+                    steps_in_epoch <= args.gradient_accumulation_steps
+                    and (step + 1) == steps_in_epoch
+                )
+
+                if args.local_rank != -1 and args.distribution_strategy == "fast_ddp" and is_optimization_step:
+                    all_reduce_gradients(
+                        model, use_hpu_graph=True
+                    )  # use HPU graphs for gradient fusion regardless of args.use_hpu_graphs_for_training setting
+
                 if args.logging_nan_inf_filter and (torch.isnan(tr_loss_step) or torch.isinf(tr_loss_step)):
                     # if loss is nan or inf simply add the average of previous logged losses
                     tr_loss += tr_loss / (1 + self.state.global_step - self._globalstep_last_logged)
                 else:
                     tr_loss += tr_loss_step
 
                 self.current_flos += float(self.floating_point_ops(inputs))
                 if args.use_lazy_mode:
                     self.htcore.mark_step()
 
                 # Optimizer step for deepspeed must be called on every step regardless of the value of gradient_accumulation_steps
                 if self.deepspeed:
                     self.deepspeed.step()
 
-                if (step + 1) % args.gradient_accumulation_steps == 0 or (
-                    # last step in epoch but step is always smaller than gradient_accumulation_steps
-                    steps_in_epoch <= args.gradient_accumulation_steps
-                    and (step + 1) == steps_in_epoch
-                ):
+                if is_optimization_step:
                     # Gradient clipping
                     if args.max_grad_norm is not None and args.max_grad_norm > 0 and not self.deepspeed:
                         # deepspeed does its own clipping
 
                         if hasattr(self.optimizer, "clip_grad_norm"):
                             # Some optimizers (like the sharded optimizer) have a specific way to do gradient clipping
                             self.optimizer.clip_grad_norm(args.max_grad_norm)
                         elif hasattr(model, "clip_grad_norm_"):
                             # Some models (like FullyShardedDDP) have a specific way to do gradient clipping
                             model.clip_grad_norm_(args.max_grad_norm)
                         elif self.gaudi_config.use_fused_clip_norm and args.use_habana:
                             self.FusedNorm.clip_norm(model.parameters())
                         else:
                             # Revert to normal clipping otherwise
-                            if args.use_habana and self.gaudi_config.use_habana_mixed_precision:
+                            if (
+                                args.use_habana
+                                and (not (self.use_hpu_amp or self.use_cpu_amp))
+                                and self.gaudi_config.use_habana_mixed_precision
+                            ):
                                 with self.hmp.disable_casts():
                                     torch.nn.utils.clip_grad_norm_(model.parameters(), args.max_grad_norm)
                             else:
                                 torch.nn.utils.clip_grad_norm_(
                                     model.parameters(),
                                     args.max_grad_norm,
                                 )
@@ -853,40 +988,38 @@
                     # Optimizer step
                     optimizer_was_run = True
                     if self.deepspeed:
                         pass  # called outside the loop
                     elif (
                         args.use_habana
                         and self.gaudi_config.use_habana_mixed_precision
-                        and not (self.gaudi_config.use_fused_adam)
+                        and (not self.gaudi_config.use_fused_adam)
+                        and (not (self.use_hpu_amp or self.use_cpu_amp))
                     ):
                         with self.hmp.disable_casts():
                             self.optimizer.step()
                     else:
                         self.optimizer.step()
 
                     if optimizer_was_run and not self.deepspeed:
                         self.lr_scheduler.step()
 
-                    # set_to_none is not implemented for some optimizers
-                    try:
-                        model.zero_grad(set_to_none=True)
-                    except TypeError:
-                        model.zero_grad()
+                    self._zero_model_grad(model)
 
                     self.state.global_step += 1
                     self.state.epoch = epoch + (step + 1) / steps_in_epoch
                     if args.use_lazy_mode:
                         self.htcore.mark_step()
                     self.control = self.callback_handler.on_step_end(args, self.state, self.control)
 
                     self._maybe_log_save_evaluate(tr_loss, model, trial, epoch, ignore_keys_for_eval)
                 else:
                     self.control = self.callback_handler.on_substep_end(args, self.state, self.control)
 
+                hb_profiler.step()
                 if self.control.should_epoch_stop or self.control.should_training_stop:
                     break
             if step < 0:
                 logger.warning(
                     "There seems to be not a single sample in your epoch_iterator, stopping training at step"
                     f" {self.state.global_step}! This is expected if you're using an IterableDataset and set"
                     f" num_steps ({max_steps}) higher than the number of available samples."
@@ -895,14 +1028,16 @@
 
             self.control = self.callback_handler.on_epoch_end(args, self.state, self.control)
             self._maybe_log_save_evaluate(tr_loss, model, trial, epoch, ignore_keys_for_eval)
 
             if self.control.should_training_stop:
                 break
 
+        hb_profiler.stop()
+
         if args.past_index and hasattr(self, "_past"):
             # Clean the state at the end of training
             delattr(self, "_past")
 
         logger.info("\n\nTraining completed. Do not forget to share your model on huggingface.co/models =)\n\n")
         if args.load_best_model_at_end and self.state.best_model_checkpoint is not None:
             # Wait for everyone to get here so we are sure the model has been saved by process 0.
@@ -920,14 +1055,15 @@
         num_steps_for_speed_metrics = self.state.max_steps - args.throughput_warmup_steps
         metrics = speed_metrics(
             "train",
             start_time,
             num_samples=num_samples_for_speed_metrics,
             num_steps=num_steps_for_speed_metrics,
             start_time_after_warmup=start_time_after_warmup,
+            log_evaluate_save_time=self.log_evaluate_save_time,
         )
         self.store_flos()
         metrics["total_flos"] = self.state.total_flos
         metrics["train_loss"] = train_loss
 
         self.is_in_train = False
 
@@ -1145,15 +1281,15 @@
             self.model_wrapped = deepspeed_engine
             self.deepspeed = deepspeed_engine
 
         model = self._wrap_model(self.model, training=False, dataloader=dataloader)
         model.eval()
 
         # Do not use HPU graphs if the training is ongoing because it detaches gradients
-        if args.use_hpu_graphs and not self.is_in_train:
+        if args.use_hpu_graphs_for_inference and not self.is_in_train:
             logger.info("Using HPU graphs for inference.")
             # Do not wrap the model in HPU graphs if it has already been done
             if not self.already_wrapped_for_hpu_graphs:
                 from habana_frameworks.torch.hpu import wrap_in_hpu_graph
 
                 model = wrap_in_hpu_graph(model)
                 self.already_wrapped_for_hpu_graphs = True
@@ -1412,19 +1548,19 @@
                         logits = outputs
                     # TODO: this needs to be fixed and made cleaner later.
                     if self.args.past_index >= 0:
                         self._past = outputs[self.args.past_index - 1]
             except RuntimeError as error:
                 if "cpu fallback is not supported during hpu graph capturing" in str(error):
                     error.args = (
-                        f"{error}. You should run inference in lazy mode only with `use_lazy_mode=True` and `use_hpu_graphs=False`.",
+                        f"{error}. You should run inference in lazy mode only with `use_lazy_mode=True` and `use_hpu_graphs_for_inference=False`.",
                     )
                 raise error
 
-        if self.args.use_lazy_mode and not (self.args.use_hpu_graphs and not self.is_in_train):
+        if self.args.use_lazy_mode and not (self.args.use_hpu_graphs_for_inference and not self.is_in_train):
             self.htcore.mark_step()
 
         if prediction_loss_only:
             return (loss, None, None)
 
         logits = nested_detach(logits)
         if len(logits) == 1:
@@ -1467,15 +1603,15 @@
             deepspeed_engine.optimizer.optimizer = None
             deepspeed_engine.lr_scheduler = None
 
         model = self._wrap_model(self.model, training=False, dataloader=dataloader)
         model.eval()
 
         # Do not use HPU graphs if the training is ongoing because it detaches gradients
-        if args.use_hpu_graphs and not self.is_in_train:
+        if args.use_hpu_graphs_for_inference and not self.is_in_train:
             logger.info("Using HPU graphs for inference.")
             # Do not wrap the model in HPU graphs if it has already been done
             if not self.already_wrapped_for_hpu_graphs:
                 from habana_frameworks.torch.hpu import wrap_in_hpu_graph
 
                 model = wrap_in_hpu_graph(model)
                 self.already_wrapped_for_hpu_graphs = True
@@ -1763,7 +1899,39 @@
         self.control = self.callback_handler.on_log(self.args, self.state, self.control, logs)
 
     def _move_model_to_device(self, model, device):
         model = model.to(device)
         # Moving a model to HPU disconnects the tied weights, so we have to retie them.
         if self.args.use_habana and hasattr(model, "tie_weights"):
             model.tie_weights()
+
+    def autocast_smart_context_manager(self, cache_enabled: Optional[bool] = True):
+        """
+        A helper wrapper that creates an appropriate context manager for `autocast` while feeding it the desired
+        arguments, depending on the situation. Modified by Habana to enable using `autocast` on Gaudi devices.
+        """
+        if self.use_cpu_amp:
+            ctx_manager = torch.cpu.amp.autocast(cache_enabled=cache_enabled, dtype=torch.bfloat16)
+        elif self.use_hpu_amp:
+            ctx_manager = torch.autocast(device_type="hpu", dtype=torch.bfloat16, enabled=True)
+        else:
+            import contextlib
+
+            ctx_manager = contextlib.nullcontext() if sys.version_info >= (3, 7) else contextlib.suppress()
+        return ctx_manager
+
+    def _zero_model_grad(self, model):
+        if hasattr(model, "_zero_grad_kwargs"):
+            model.zero_grad(**model._zero_grad_kwargs)
+        else:
+            # Optimization based on setting gradients to None (instead of zeroing them out) may only be used when gradients are not recorded using HPU graphs.
+            # HPU graphs rely on fixed tensors - setting gradients to None will enforce their re-allocation during the backward pass each step.
+            set_to_none = (
+                self.args.local_rank == -1 or self.args.distribution_strategy == "ddp"
+            ) and not self.args.use_hpu_graphs_for_training
+
+            try:
+                model.zero_grad(set_to_none=set_to_none)
+                model._zero_grad_kwargs = {"set_to_none": set_to_none}
+            except TypeError:
+                model.zero_grad()
+                model._zero_grad_kwargs = {}
```

### Comparing `optimum-habana-1.5.1/optimum/habana/transformers/trainer_seq2seq.py` & `optimum-habana-1.6.0/optimum/habana/transformers/trainer_seq2seq.py`

 * *Files 2% similar despite different names*

```diff
@@ -203,22 +203,14 @@
         if gen_kwargs.get("max_length") is None and gen_kwargs.get("max_new_tokens") is None:
             gen_kwargs["max_length"] = self.args.generation_max_length
         gen_kwargs["num_beams"] = (
             gen_kwargs["num_beams"] if gen_kwargs.get("num_beams") is not None else self.args.generation_num_beams
         )
         self._gen_kwargs = gen_kwargs
 
-        if self.args.use_hpu_graphs:
-            # Disable HPU graphs as generation needs to be fixed
-            self.args.use_hpu_graphs = False
-            logger.warning(
-                "HPU graphs have not been validated for generation yet. Disabling it, generation will be"
-                " performed in lazy mode."
-            )
-
         return super().predict(test_dataset, ignore_keys=ignore_keys, metric_key_prefix=metric_key_prefix)
 
     def prediction_step(
         self,
         model: torch.nn.Module,
         inputs: Dict[str, Union[torch.Tensor, Any]],
         prediction_loss_only: bool,
@@ -263,26 +255,28 @@
             gen_kwargs["synced_gpus"] if gen_kwargs.get("synced_gpus") is not None else default_synced_gpus
         )
         # pad batches to max_length on-the-fly in lazy mode
         gen_kwargs["lazy_mode"] = (
             gen_kwargs["lazy_mode"] if gen_kwargs.get("lazy_mode") is not None else self.args.use_lazy_mode
         )
         gen_kwargs["hpu_graphs"] = (
-            gen_kwargs["hpu_graphs"] if gen_kwargs.get("hpu_graphs") is not None else self.args.use_hpu_graphs
+            gen_kwargs["hpu_graphs"]
+            if gen_kwargs.get("hpu_graphs") is not None
+            else self.args.use_hpu_graphs_for_inference
         )
 
         # TODO (Joao): the following line is needed to keep a consistent result on SQUAD. Ideally, we should not block
         # users from preparing a dataset with `decoder_input_ids`.
         inputs = {k: v for k, v in inputs.items() if k != "decoder_input_ids"}
         try:
             generated_tokens = self.model.generate(**inputs, **gen_kwargs)
         except RuntimeError as error:
             if "cpu fallback is not supported during hpu graph capturing" in str(error):
                 error.args = (
-                    f"{error}. You should run inference in lazy mode only with `use_lazy_mode=True` and `use_hpu_graphs=False`.",
+                    f"{error}. You should run inference in lazy mode only with `use_lazy_mode=True` and `use_hpu_graphs_for_inference=False`.",
                 )
             raise error
 
         # Temporary hack to ensure the generation config is not initialized for each iteration of the evaluation loop
         # TODO: remove this hack when the legacy code that initializes generation_config from a model config is
         # removed in https://github.com/huggingface/transformers/blob/98d88b23f54e5a23e741833f1e973fdf600cc2c5/src/transformers/generation/utils.py#L1183
         if self.model.generation_config._from_model_config:
@@ -310,19 +304,19 @@
                     else:
                         loss = (outputs["loss"] if isinstance(outputs, dict) else outputs[0]).mean().detach()
                 else:
                     loss = None
             except RuntimeError as error:
                 if "cpu fallback is not supported during hpu graph capturing" in str(error):
                     error.args = (
-                        f"{error}. You should run inference in lazy mode only with `use_lazy_mode=True` and `use_hpu_graphs=False`.",
+                        f"{error}. You should run inference in lazy mode only with `use_lazy_mode=True` and `use_hpu_graphs_for_inference=False`.",
                     )
                 raise error
 
-        if self.args.use_lazy_mode and not (self.args.use_hpu_graphs and not self.is_in_train):
+        if self.args.use_lazy_mode and not (self.args.use_hpu_graphs_for_inference and not self.is_in_train):
             self.htcore.mark_step()
 
         if self.args.prediction_loss_only:
             return loss, None, None
 
         if has_labels:
             labels = inputs["labels"]
```

### Comparing `optimum-habana-1.5.1/optimum/habana/transformers/trainer_utils.py` & `optimum-habana-1.6.0/optimum/habana/transformers/trainer_utils.py`

 * *Files identical despite different names*

### Comparing `optimum-habana-1.5.1/optimum/habana/transformers/training_args.py` & `optimum-habana-1.6.0/optimum/habana/transformers/training_args.py`

 * *Files 16% similar despite different names*

```diff
@@ -46,135 +46,245 @@
 
 
 logger = logging.get_logger(__name__)
 
 
 # List of arguments that are not supported by optimum-habana
 UNSUPPORTED_ARGUMENTS = [
-    "bf16",  # bf16 for CUDA devices
-    "bf16_full_eval",  # bf16 for CUDA devices
+    "bf16_full_eval",
     "fp16",
     "fp16_backend",
     "fp16_full_eval",
     "fp16_opt_level",
     "fsdp",
-    "half_precision_backend",  # not supported, Habana Mixed Precision should be used and specified in Gaudi configuration
     "mp_parameters",
     "sharded_ddp",
     "tf32",
     "tpu_metrics_debug",
     "tpu_num_cores",
 ]
 
 
+# List of supported distribution strategies
+SUPPORTED_DISTRIBUTION_STRATEGIES = [
+    "ddp",  # default
+    "fast_ddp",
+]
+
+
 @dataclass
 class GaudiTrainingArguments(TrainingArguments):
     """
-    GaudiTrainingArguments is built on top of the tranformers' TrainingArguments
+    GaudiTrainingArguments is built on top of the Tranformers' [TrainingArguments](https://huggingface.co/docs/transformers/main_classes/trainer#transformers.TrainingArguments)
     to enable deployment on Habana's Gaudi.
+
+    Args:
+        use_habana (`bool`, *optional*, defaults to `False`):
+            Whether to use Habana's HPU for running the model.
+        gaudi_config_name (`str`, *optional*):
+            Pretrained Gaudi config name or path.
+        use_lazy_mode (`bool`, *optional*, defaults to `False`):
+            Whether to use lazy mode for running the model.
+        use_hpu_graphs (`bool`, *optional*, defaults to `False`):
+            Deprecated, use `use_hpu_graphs_for_inference` instead. Whether to use HPU graphs for performing inference.
+        use_hpu_graphs_for_inference (`bool`, *optional*, defaults to `False`):
+            Whether to use HPU graphs for performing inference. It will speed up latency but may not be compatible with some operations.
+        use_hpu_graphs_for_training (`bool`, *optional*, defaults to `False`):
+            Whether to use HPU graphs for performing inference. It will speed up training but may not be compatible with some operations.
+        distribution_strategy (`str`, *optional*, defaults to `ddp`):
+            Determines how data parallel distributed training is achieved. May be: `ddp` or `fast_ddp`.
+        throughput_warmup_steps (`int`, *optional*, defaults to 0):
+            Number of steps to ignore for throughput calculation. For example, with `throughput_warmup_steps=N`,
+            the first N steps will not be considered in the calculation of the throughput. This is especially
+            useful in lazy mode where the first two or three iterations typically take longer.
+        adjust_throughput ('bool', *optional*, defaults to `False`):
+            Whether to remove the time taken for logging, evaluating and saving from throughput calculation.
+        pipelining_fwd_bwd (`bool`, *optional*, defaults to `False`):
+            Whether to add an additional `mark_step` between forward and backward for pipelining
+            host backward building and HPU forward computing.
+        non_blocking_data_copy (`bool`, *optional*, defaults to `False`):
+            Whether to enable async data copy when preparing inputs.
+        profiling_warmup_steps (`int`, *optional*, defaults to 0):
+            Number of steps to ignore for profling.
+        profiling_steps (`int`, *optional*, defaults to 0):
+            Number of steps to be captured when enabling profiling.
     """
 
     use_habana: Optional[bool] = field(
         default=False,
-        metadata={"help": "Whether to use Habana's HPU for training the model."},
+        metadata={"help": "Whether to use Habana's HPU for running the model."},
     )
 
     gaudi_config_name: Optional[str] = field(
         default=None,
-        metadata={"help": "Pretrained Gaudi config name or path if not the same as model_name."},
+        metadata={"help": "Pretrained Gaudi config name or path."},
+    )
+
+    use_lazy_mode: Optional[bool] = field(
+        default=False,
+        metadata={"help": "Whether to use lazy mode for running the model."},
+    )
+
+    use_hpu_graphs: Optional[bool] = field(
+        default=False,
+        metadata={
+            "help": "Deprecated, use `use_hpu_graphs_for_inference` instead. Whether to use HPU graphs for performing inference."
+        },
     )
 
-    use_lazy_mode: bool = field(
+    use_hpu_graphs_for_inference: Optional[bool] = field(
         default=False,
-        metadata={"help": "Whether to use lazy mode for training the model."},
+        metadata={
+            "help": "Whether to use HPU graphs for performing inference. It will speed up latency but may not be compatible with some operations."
+        },
     )
 
-    use_hpu_graphs: bool = field(
+    use_hpu_graphs_for_training: Optional[bool] = field(
         default=False,
-        metadata={"help": "Whether to use HPU graphs for performing inference."},
+        metadata={
+            "help": "Whether to use HPU graphs for performing training. It will speed up training but may not be compatible with some operations."
+        },
     )
 
-    throughput_warmup_steps: int = field(
+    distribution_strategy: Optional[str] = field(
+        default="ddp",
+        metadata={
+            "help": "Determines how distributed data parallel training is achieved. "
+            "Can be either `ddp` (i.e. using `DistributedDataParallel`) or "
+            "`fast_ddp` (i.e. using `optimum.habana.distributed.all_reduce_gradients`).",
+            "choices": ["ddp", "fast_ddp"],
+        },
+    )
+
+    throughput_warmup_steps: Optional[int] = field(
         default=0,
         metadata={
             "help": (
-                "Number of steps to ignore for throughput calculation. For example, with throughput_warmup_steps=N,"
+                "Number of steps to ignore for throughput calculation. For example, with `throughput_warmup_steps=N`,"
                 " the first N steps will not be considered in the calculation of the throughput. This is especially"
-                " useful in lazy mode where the first two or three training iterations typically take longer."
+                " useful in lazy mode where the first two or three iterations typically take longer."
             )
         },
     )
 
+    adjust_throughput: bool = field(
+        default=False,
+        metadata={
+            "help": "Whether to remove the time taken for logging, evaluating and saving from throughput calculation."
+        },
+    )
+
+    pipelining_fwd_bwd: Optional[bool] = field(
+        default=False,
+        metadata={
+            "help": (
+                "Whether to add an additional `mark_step` between forward and backward for pipelining "
+                "host backward building and HPU forward computing."
+            )
+        },
+    )
+
+    non_blocking_data_copy: Optional[bool] = field(
+        default=False,
+        metadata={"help": ("Whether to enable async data copy when preparing inputs.")},
+    )
+
+    profiling_warmup_steps: Optional[int] = field(
+        default=0,
+        metadata={"help": ("Number of steps to ignore for profling.")},
+    )
+
+    profiling_steps: Optional[int] = field(
+        default=0,
+        metadata={"help": ("Number of steps to be captured when enabling profiling.")},
+    )
+
     # Overriding the default value of optim because 'adamw_hf' is deprecated
-    optim: Union[OptimizerNames, str] = field(
+    optim: Optional[Union[OptimizerNames, str]] = field(
         default="adamw_torch",
         metadata={"help": "The optimizer to use."},
     )
 
-    # Override the default value of epsilon to be consistent with Habana FusedAdamW
-    adam_epsilon: float = field(
+    # Overriding the default value of epsilon to be consistent with Habana FusedAdamW
+    adam_epsilon: Optional[float] = field(
         default=1e-6,
         metadata={"help": "Epsilon for AdamW optimizer."},
     )
 
-    # Override logging_nan_inf_filter to make False the default value
-    logging_nan_inf_filter: bool = field(
+    # Overriding logging_nan_inf_filter to make False the default value
+    logging_nan_inf_filter: Optional[bool] = field(
         default=False,
         metadata={"help": "Filter nan and inf losses for logging."},
     )
 
+    # Overriding ddp_bucket_cap_mb to make 230 the default value
     ddp_bucket_cap_mb: Optional[int] = field(
         default=230,
         metadata={
             "help": (
                 "When using distributed training, the value of the flag `bucket_cap_mb` passed to "
                 "`DistributedDataParallel`."
             )
         },
     )
 
+    # Overriding ddp_find_unused_parameters to make False the default value
     ddp_find_unused_parameters: Optional[bool] = field(
         default=False,
         metadata={
             "help": (
                 "When using distributed training, the value of the flag `find_unused_parameters` passed to "
                 "`DistributedDataParallel`."
             )
         },
     )
 
-    pipelining_fwd_bwd: Optional[bool] = field(
-        default=False,
+    # Overriding half_precision_backend to allow only CPU and HPU as possible mixed-precision backends for Torch Autocast.
+    half_precision_backend: str = field(
+        default="hpu_amp",
         metadata={
-            "help": (
-                "Whether to add an additional mark_step between forward and backward for pipelining "
-                "host BWD building and HPU FWD computing."
-            )
+            "help": "The backend to use for half precision.",
+            "choices": ["cpu_amp", "hpu_amp"],
         },
     )
 
     def __post_init__(self):
-        if (self.use_lazy_mode or self.use_hpu_graphs or self.gaudi_config_name) and not self.use_habana:
+        if self.use_hpu_graphs:
+            warnings.warn(
+                (
+                    "`--use_hpu_graphs` is deprecated and will be removed in a future version of 🤗 Optimum Habana. Use "
+                    "`--use_hpu_graphs_for_inference` instead."
+                ),
+                FutureWarning,
+            )
+
+        use_hpu_graphs = self.use_hpu_graphs or self.use_hpu_graphs_for_inference or self.use_hpu_graphs_for_training
+
+        if (self.use_lazy_mode or use_hpu_graphs or self.gaudi_config_name) and not self.use_habana:
             raise ValueError(
-                "--use_lazy_mode, --use_hpu_graphs and --gaudi_config_name cannot be used without --use_habana"
+                "`--use_lazy_mode`, `--use_hpu_graphs_for_inference`, `--use_hpu_graphs_for_training` and `--gaudi_config_name` cannot be used without `--use_habana`."
             )
 
-        if self.use_hpu_graphs and not self.use_lazy_mode:
-            raise ValueError("--use_hpu_graphs cannot be used in eager mode. Please set --use_lazy_mode to True.")
+        if use_hpu_graphs and not self.use_lazy_mode:
+            raise ValueError(
+                "`--use_hpu_graphs_for_inference` and `--use_hpu_graphs_for_training` cannot be used in eager mode. Please set `--use_lazy_mode` to True."
+            )
 
-        # Raise errors for arguments that are not supported by optimum-habana
-        if self.bf16 or self.bf16_full_eval:
+        if self.distribution_strategy not in SUPPORTED_DISTRIBUTION_STRATEGIES:
             raise ValueError(
-                "--bf16 and --bf16_full_eval are not supported by optimum-habana. You should turn on Habana Mixed"
-                " Precision in your Gaudi configuration to enable bf16."
+                f"`--distribution_strategy` is {self.distribution_strategy} which is an invalid or unsupported value. Possible choices are: {', '.join(SUPPORTED_DISTRIBUTION_STRATEGIES)}."
             )
+
+        # Raise errors for arguments that are not supported by optimum-habana
+        if self.bf16_full_eval:
+            raise ValueError("--bf16_full_eval is not supported by optimum-habana.")
         if self.fp16 or self.fp16_full_eval:
             raise ValueError(
-                "--fp16, --fp16_backend, --fp16_full_eval, --fp16_opt_level and --half_precision_backend are not"
-                " supported by optimum-habana. Mixed-precision training can be enabled in your Gaudi configuration."
+                "--fp16, --fp16_backend, --fp16_full_eval and --fp16_opt_level are not"
+                " supported by optimum-habana. Mixed-precision can be enabled in your Gaudi configuration."
             )
         if self.fsdp:
             raise ValueError("--fsdp is not supported by optimum-habana.")
         if self.tpu_num_cores or self.tpu_metrics_debug:
             raise ValueError("TPUs are not supported by optimum-habana.")
         if self.mp_parameters:
             raise ValueError("--mp_parameters is not supported by optimum-habana.")
@@ -188,14 +298,19 @@
 
         # Handle --use_env option in torch.distributed.launch (local_rank not passed as an arg then).
         # This needs to happen before any call to self.device or self.n_gpu.
         env_local_rank = int(os.environ.get("LOCAL_RANK", -1))
         if env_local_rank != -1 and env_local_rank != self.local_rank:
             self.local_rank = env_local_rank
 
+        if self.local_rank != -1 and self.use_hpu_graphs_for_training and self.distribution_strategy != "fast_ddp":
+            raise ValueError(
+                "`--use_hpu_graphs_for_training` may only be used with `--distribution_strategy fast_ddp`"
+            )
+
         # expand paths, if not os.makedirs("~/bar") will make directory
         # in the current directory instead of the actual home
         # see https://github.com/huggingface/transformers/issues/10628
         if self.output_dir is not None:
             self.output_dir = os.path.expanduser(self.output_dir)
         if self.logging_dir is None and self.output_dir is not None:
             self.logging_dir = os.path.join(self.output_dir, default_logdir())
@@ -489,15 +604,15 @@
             if self.deepspeed:
                 # deepspeed inits torch.distributed internally
                 from transformers.deepspeed import is_deepspeed_available
 
                 if not is_deepspeed_available():
                     raise ImportError(
                         "--deepspeed requires deepspeed: `pip install"
-                        " git+https://github.com/HabanaAI/DeepSpeed.git@1.9.0`."
+                        " git+https://github.com/HabanaAI/DeepSpeed.git@1.10.0`."
                     )
                 import deepspeed
 
                 if world_size > 1:
                     os.environ["HLS_MODULE_ID"] = str(self.local_rank)
                     os.environ["ID"] = str(rank)
```

### Comparing `optimum-habana-1.5.1/optimum/habana/transformers/training_args_seq2seq.py` & `optimum-habana-1.6.0/optimum/habana/transformers/training_args_seq2seq.py`

 * *Files 10% similar despite different names*

```diff
@@ -14,51 +14,52 @@
 # limitations under the License.
 
 from dataclasses import dataclass, field
 from pathlib import Path
 from typing import Optional, Union
 
 from transformers.generation.configuration_utils import GenerationConfig
-from transformers.utils import add_start_docstrings
 
 from optimum.utils import logging
 
 from .training_args import GaudiTrainingArguments
 
 
 logger = logging.get_logger(__name__)
 
 
 @dataclass
-@add_start_docstrings(GaudiTrainingArguments.__doc__)
 class GaudiSeq2SeqTrainingArguments(GaudiTrainingArguments):
     """
+    GaudiSeq2SeqTrainingArguments is built on top of the Tranformers' [Seq2SeqTrainingArguments](https://huggingface.co/docs/transformers/main_classes/trainer#transformers.Seq2SeqTrainingArguments)
+    to enable deployment on Habana's Gaudi.
+
     Args:
         sortish_sampler (`bool`, *optional*, defaults to `False`):
             Whether to use a *sortish sampler* or not. Only possible if the underlying datasets are *Seq2SeqDataset*
             for now but will become generally available in the near future.
             It sorts the inputs according to lengths in order to minimize the padding size, with a bit of randomness
             for the training set.
         predict_with_generate (`bool`, *optional*, defaults to `False`):
             Whether to use generate to calculate generative metrics (ROUGE, BLEU).
         generation_max_length (`int`, *optional*):
             The `max_length` to use on each evaluation loop when `predict_with_generate=True`. Will default to the
             `max_length` value of the model configuration.
         generation_num_beams (`int`, *optional*):
             The `num_beams` to use on each evaluation loop when `predict_with_generate=True`. Will default to the
             `num_beams` value of the model configuration.
-        generation_config (`str` or `Path` or [`~generation.GenerationConfig`], *optional*):
-            Allows to load a [`~generation.GenerationConfig`] from the `from_pretrained` method. This can be either:
+        generation_config (`str` or `Path` or [`transformers.generation.GenerationConfig`], *optional*):
+            Allows to load a [`transformers.generation.GenerationConfig`] from the `from_pretrained` method. This can be either:
 
             - a string, the *model id* of a pretrained model configuration hosted inside a model repo on
               huggingface.co. Valid model ids can be located at the root-level, like `bert-base-uncased`, or namespaced
               under a user or organization name, like `dbmdz/bert-base-german-cased`.
             - a path to a *directory* containing a configuration file saved using the
-              [`~GenerationConfig.save_pretrained`] method, e.g., `./my_model_directory/`.
-            - a [`~generation.GenerationConfig`] object.
+              [`transformers.GenerationConfig.save_pretrained`] method, e.g., `./my_model_directory/`.
+            - a [`transformers.generation.GenerationConfig`] object.
     """
 
     sortish_sampler: bool = field(default=False, metadata={"help": "Whether to use SortishSampler or not."})
     predict_with_generate: bool = field(
         default=False, metadata={"help": "Whether to use generate to calculate generative metrics (ROUGE, BLEU)."}
     )
     generation_max_length: Optional[int] = field(
```

### Comparing `optimum-habana-1.5.1/optimum/habana/version.py` & `optimum-habana-1.6.0/optimum/habana/version.py`

 * *Files 2% similar despite different names*

```diff
@@ -9,8 +9,8 @@
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
-__version__ = "1.5.1"
+__version__ = "1.6.0"
```

### Comparing `optimum-habana-1.5.1/optimum_habana.egg-info/SOURCES.txt` & `optimum-habana-1.6.0/optimum_habana.egg-info/SOURCES.txt`

 * *Files 19% similar despite different names*

```diff
@@ -10,14 +10,15 @@
 optimum/habana/diffusers/__init__.py
 optimum/habana/diffusers/pipelines/pipeline_utils.py
 optimum/habana/diffusers/pipelines/stable_diffusion/pipeline_stable_diffusion.py
 optimum/habana/diffusers/schedulers/__init__.py
 optimum/habana/diffusers/schedulers/scheduling_ddim.py
 optimum/habana/distributed/__init__.py
 optimum/habana/distributed/distributed_runner.py
+optimum/habana/distributed/fast_ddp.py
 optimum/habana/transformers/__init__.py
 optimum/habana/transformers/deepspeed.py
 optimum/habana/transformers/gaudi_configuration.py
 optimum/habana/transformers/gradient_checkpointing.py
 optimum/habana/transformers/modeling_utils.py
 optimum/habana/transformers/trainer.py
 optimum/habana/transformers/trainer_seq2seq.py
@@ -28,16 +29,27 @@
 optimum/habana/transformers/generation/utils.py
 optimum/habana/transformers/models/__init__.py
 optimum/habana/transformers/models/modeling_all_models.py
 optimum/habana/transformers/models/albert/__init__.py
 optimum/habana/transformers/models/albert/modeling_albert.py
 optimum/habana/transformers/models/bloom/__init__.py
 optimum/habana/transformers/models/bloom/modeling_bloom.py
+optimum/habana/transformers/models/esm/__init__.py
+optimum/habana/transformers/models/esm/modeling_esm.py
+optimum/habana/transformers/models/esm/modeling_esmfold.py
 optimum/habana/transformers/models/gpt2/__init__.py
 optimum/habana/transformers/models/gpt2/modeling_gpt2.py
+optimum/habana/transformers/models/gpt_neox/__init__.py
+optimum/habana/transformers/models/gpt_neox/modeling_gpt_neox.py
+optimum/habana/transformers/models/gptj/__init__.py
+optimum/habana/transformers/models/gptj/modeling_gptj.py
+optimum/habana/transformers/models/opt/__init__.py
+optimum/habana/transformers/models/opt/modeling_opt.py
+optimum/habana/transformers/models/t5/__init__.py
+optimum/habana/transformers/models/t5/modeling_t5.py
 optimum/habana/transformers/models/vit/__init__.py
 optimum/habana/transformers/models/vit/modeling_vit.py
 optimum/habana/transformers/models/wav2vec2/__init__.py
 optimum/habana/transformers/models/wav2vec2/modeling_wav2vec2.py
 optimum_habana.egg-info/PKG-INFO
 optimum_habana.egg-info/SOURCES.txt
 optimum_habana.egg-info/dependency_links.txt
```

### Comparing `optimum-habana-1.5.1/pyproject.toml` & `optimum-habana-1.6.0/pyproject.toml`

 * *Files identical despite different names*

### Comparing `optimum-habana-1.5.1/setup.py` & `optimum-habana-1.6.0/setup.py`

 * *Files identical despite different names*

### Comparing `optimum-habana-1.5.1/tests/test_diffusers.py` & `optimum-habana-1.6.0/tests/test_diffusers.py`

 * *Files 4% similar despite different names*

```diff
@@ -27,15 +27,17 @@
 from transformers.testing_utils import slow
 
 from optimum.habana import GaudiConfig
 from optimum.habana.diffusers import GaudiDDIMScheduler, GaudiDiffusionPipeline, GaudiStableDiffusionPipeline
 from optimum.habana.utils import set_seed
 
 
-THROUGHPUT_BASELINE = 0.277
+THROUGHPUT_BASELINE_HMP = 0.287
+THROUGHPUT_BASELINE_BF16 = 0.302
+THROUGHPUT_BASELINE_AUTOCAST = 0.108
 
 
 class GaudiPipelineUtilsTester(TestCase):
     """
     Tests the features added on top of diffusers/pipeline_utils.py.
     """
 
@@ -94,26 +96,14 @@
             gaudi_config=GaudiConfig(),
         )
 
         self.assertTrue(hasattr(pipeline, "ht"))
         self.assertTrue(hasattr(pipeline, "hpu_stream"))
         self.assertTrue(hasattr(pipeline, "cache"))
 
-    def test_habana_mixed_precision(self):
-        gaudi_config = GaudiConfig(
-            use_habana_mixed_precision=True,
-        )
-
-        pipeline = GaudiDiffusionPipeline(
-            use_habana=True,
-            gaudi_config=gaudi_config,
-        )
-
-        self.assertTrue(hasattr(pipeline, "hmp"))
-
     def test_save_pretrained(self):
         model_name = "hf-internal-testing/tiny-stable-diffusion-torch"
         scheduler = GaudiDDIMScheduler.from_pretrained(model_name, subfolder="scheduler")
         pipeline = GaudiStableDiffusionPipeline.from_pretrained(
             model_name,
             scheduler=scheduler,
             use_habana=True,
@@ -505,15 +495,42 @@
             num_images_per_prompt=5,
         ).images
 
         self.assertEqual(len(images), 10)
         self.assertEqual(images[-1].shape, (64, 64, 3))
 
     @slow
-    def test_no_throughput_regression(self):
+    def test_no_throughput_regression_hmp(self):
+        prompts = [
+            "An image of a squirrel in Picasso style",
+            "High quality photo of an astronaut riding a horse in space",
+        ]
+        num_images_per_prompt = 11
+        batch_size = 4
+        model_name = "runwayml/stable-diffusion-v1-5"
+        scheduler = GaudiDDIMScheduler.from_pretrained(model_name, subfolder="scheduler")
+
+        pipeline = GaudiStableDiffusionPipeline.from_pretrained(
+            model_name,
+            scheduler=scheduler,
+            use_habana=True,
+            use_hpu_graphs=True,
+            gaudi_config=GaudiConfig.from_pretrained("Habana/stable-diffusion"),
+        )
+        set_seed(27)
+        outputs = pipeline(
+            prompt=prompts,
+            num_images_per_prompt=num_images_per_prompt,
+            batch_size=batch_size,
+        )
+        self.assertEqual(len(outputs.images), num_images_per_prompt * len(prompts))
+        self.assertGreaterEqual(outputs.throughput, 0.95 * THROUGHPUT_BASELINE_HMP)
+
+    @slow
+    def test_no_throughput_regression_bf16(self):
         prompts = [
             "An image of a squirrel in Picasso style",
             "High quality photo of an astronaut riding a horse in space",
         ]
         num_images_per_prompt = 11
         batch_size = 4
         model_name = "runwayml/stable-diffusion-v1-5"
@@ -521,23 +538,53 @@
 
         pipeline = GaudiStableDiffusionPipeline.from_pretrained(
             model_name,
             scheduler=scheduler,
             use_habana=True,
             use_hpu_graphs=True,
             gaudi_config=GaudiConfig.from_pretrained("Habana/stable-diffusion"),
+            torch_dtype=torch.bfloat16,
+        )
+        set_seed(27)
+        outputs = pipeline(
+            prompt=prompts,
+            num_images_per_prompt=num_images_per_prompt,
+            batch_size=batch_size,
+        )
+        self.assertEqual(len(outputs.images), num_images_per_prompt * len(prompts))
+        self.assertGreaterEqual(outputs.throughput, 0.95 * THROUGHPUT_BASELINE_BF16)
+
+    @slow
+    def test_no_throughput_regression_autocast(self):
+        prompts = [
+            "An image of a squirrel in Picasso style",
+            "High quality photo of an astronaut riding a horse in space",
+        ]
+        num_images_per_prompt = 11
+        batch_size = 4
+        model_name = "stabilityai/stable-diffusion-2-1"
+        scheduler = GaudiDDIMScheduler.from_pretrained(model_name, subfolder="scheduler")
+
+        pipeline = GaudiStableDiffusionPipeline.from_pretrained(
+            model_name,
+            scheduler=scheduler,
+            use_habana=True,
+            use_hpu_graphs=True,
+            gaudi_config=GaudiConfig.from_pretrained("Habana/stable-diffusion-2"),
         )
         set_seed(27)
         outputs = pipeline(
             prompt=prompts,
             num_images_per_prompt=num_images_per_prompt,
             batch_size=batch_size,
+            height=768,
+            width=768,
         )
         self.assertEqual(len(outputs.images), num_images_per_prompt * len(prompts))
-        self.assertGreaterEqual(outputs.throughput, 0.95 * THROUGHPUT_BASELINE)
+        self.assertGreaterEqual(outputs.throughput, 0.95 * THROUGHPUT_BASELINE_AUTOCAST)
 
     @slow
     def test_no_generation_regression(self):
         model_name = "CompVis/stable-diffusion-v1-4"
         # fp32
         with hmp.disable_casts():
             scheduler = GaudiDDIMScheduler.from_pretrained(model_name, subfolder="scheduler")
```

### Comparing `optimum-habana-1.5.1/tests/test_examples.py` & `optimum-habana-1.6.0/tests/test_examples.py`

 * *Files 4% similar despite different names*

```diff
@@ -33,23 +33,23 @@
     MODEL_FOR_QUESTION_ANSWERING_MAPPING,
     MODEL_FOR_SEQ_TO_SEQ_CAUSAL_LM_MAPPING,
     MODEL_FOR_SEQUENCE_CLASSIFICATION_MAPPING,
 )
 from transformers.testing_utils import slow
 
 from .utils import (
+    MODELS_TO_TEST_FOR_AUDIO_CLASSIFICATION,
+    MODELS_TO_TEST_FOR_CAUSAL_LANGUAGE_MODELING,
+    MODELS_TO_TEST_FOR_IMAGE_CLASSIFICATION,
+    MODELS_TO_TEST_FOR_MASKED_LANGUAGE_MODELING,
+    MODELS_TO_TEST_FOR_QUESTION_ANSWERING,
+    MODELS_TO_TEST_FOR_SEQ2SEQ,
+    MODELS_TO_TEST_FOR_SEQUENCE_CLASSIFICATION,
+    MODELS_TO_TEST_FOR_SPEECH_RECOGNITION,
     MODELS_TO_TEST_MAPPING,
-    VALID_MODELS_FOR_AUDIO_CLASSIFICATION,
-    VALID_MODELS_FOR_CAUSAL_LANGUAGE_MODELING,
-    VALID_MODELS_FOR_IMAGE_CLASSIFICATION,
-    VALID_MODELS_FOR_MASKED_LANGUAGE_MODELING,
-    VALID_MODELS_FOR_QUESTION_ANSWERING,
-    VALID_MODELS_FOR_SEQUENCE_CLASSIFICATION,
-    VALID_MODELS_FOR_SPEECH_RECOGNITION,
-    VALID_SEQ2SEQ_MODELS,
 )
 
 
 BASELINE_DIRECTORY = Path(__file__).parent.resolve() / Path("baselines")
 # Models should reach at least 99% of their baseline accuracy
 ACCURACY_PERF_FACTOR = 0.99
 # Trainings should last at most 5% longer than the baseline
@@ -62,15 +62,15 @@
     valid_models_for_task: List[str],
 ) -> List[Tuple[str]]:
     """
     Filter models that can perform the task from models_to_test.
     Args:
         models_to_test: mapping between a model type and a tuple (model_name_or_path, gaudi_config_name).
         task_mapping: mapping between a model config and a model class.
-        valid_models_for_task: list of supported models for a specific task.
+        valid_models_for_task: list of models to test for a specific task.
     Returns:
         A list of models that are supported for the task.
         Each element of the list follows the same format: (model_type, (model_name_or_path, gaudi_config_name)).
     """
 
     def is_valid_model_type(model_type: str) -> bool:
         in_task_mapping = CONFIG_MAPPING[model_type] in task_mapping
@@ -84,50 +84,55 @@
     ]
 
 
 _SCRIPT_TO_MODEL_MAPPING = {
     "run_qa": _get_supported_models_for_script(
         MODELS_TO_TEST_MAPPING,
         MODEL_FOR_QUESTION_ANSWERING_MAPPING,
-        VALID_MODELS_FOR_QUESTION_ANSWERING,
+        MODELS_TO_TEST_FOR_QUESTION_ANSWERING,
     ),
     "run_glue": _get_supported_models_for_script(
         MODELS_TO_TEST_MAPPING,
         MODEL_FOR_SEQUENCE_CLASSIFICATION_MAPPING,
-        VALID_MODELS_FOR_SEQUENCE_CLASSIFICATION,
+        MODELS_TO_TEST_FOR_SEQUENCE_CLASSIFICATION,
     ),
     "run_clm": _get_supported_models_for_script(
         MODELS_TO_TEST_MAPPING,
         MODEL_FOR_CAUSAL_LM_MAPPING,
-        VALID_MODELS_FOR_CAUSAL_LANGUAGE_MODELING,
+        MODELS_TO_TEST_FOR_CAUSAL_LANGUAGE_MODELING,
     ),
     "run_summarization": _get_supported_models_for_script(
         MODELS_TO_TEST_MAPPING,
         MODEL_FOR_SEQ_TO_SEQ_CAUSAL_LM_MAPPING,
-        VALID_SEQ2SEQ_MODELS,
+        MODELS_TO_TEST_FOR_SEQ2SEQ,
     ),
     "run_image_classification": _get_supported_models_for_script(
         MODELS_TO_TEST_MAPPING,
         MODEL_FOR_IMAGE_CLASSIFICATION_MAPPING,
-        VALID_MODELS_FOR_IMAGE_CLASSIFICATION,
+        MODELS_TO_TEST_FOR_IMAGE_CLASSIFICATION,
     ),
     "run_mlm": _get_supported_models_for_script(
         MODELS_TO_TEST_MAPPING,
         MODEL_FOR_MASKED_LM_MAPPING,
-        VALID_MODELS_FOR_MASKED_LANGUAGE_MODELING,
+        MODELS_TO_TEST_FOR_MASKED_LANGUAGE_MODELING,
     ),
     "run_audio_classification": _get_supported_models_for_script(
         MODELS_TO_TEST_MAPPING,
         MODEL_FOR_AUDIO_CLASSIFICATION_MAPPING,
-        VALID_MODELS_FOR_AUDIO_CLASSIFICATION,
+        MODELS_TO_TEST_FOR_AUDIO_CLASSIFICATION,
     ),
     "run_speech_recognition_ctc": _get_supported_models_for_script(
         MODELS_TO_TEST_MAPPING,
         MODEL_FOR_CTC_MAPPING,
-        VALID_MODELS_FOR_SPEECH_RECOGNITION,
+        MODELS_TO_TEST_FOR_SPEECH_RECOGNITION,
+    ),
+    "run_seq2seq_qa": _get_supported_models_for_script(
+        MODELS_TO_TEST_MAPPING,
+        MODEL_FOR_SEQ_TO_SEQ_CAUSAL_LM_MAPPING,
+        MODELS_TO_TEST_FOR_SEQ2SEQ,
     ),
 }
 
 
 class ExampleTestMeta(type):
     """
     Metaclass that takes care of creating the proper example tests for a given task.
@@ -313,15 +318,15 @@
             "--overwrite_output_dir",
             f"--learning_rate {lr}",
             f"--per_device_train_batch_size {train_batch_size}",
             f"--per_device_eval_batch_size {eval_batch_size}",
             f" --num_train_epochs {num_epochs}",
             "--use_habana",
             "--use_lazy_mode",
-            "--use_hpu_graphs",
+            "--use_hpu_graphs_for_inference",
             "--throughput_warmup_steps 3",
         ]
 
         if extra_command_line_arguments is not None:
             cmd_line += extra_command_line_arguments
 
         pattern = re.compile(r"([\"\'].+?[\"\'])|\s")
@@ -440,17 +445,27 @@
 
 class MultiCardAudioClassificationExampleTester(
     ExampleTesterBase, metaclass=ExampleTestMeta, example_name="run_audio_classification", multi_card=True
 ):
     TASK_NAME = "common_language"
 
 
+# class SpeechRecognitionExampleTester(ExampleTesterBase, metaclass=ExampleTestMeta, example_name="run_speech_recognition_ctc"):
+#     TASK_NAME = "librispeech_asr"
+
+
 # class MultiCardSpeechRecognitionExampleTester(
 #     ExampleTesterBase, metaclass=ExampleTestMeta, example_name="run_speech_recognition_ctc", multi_card=True
 # ):
 #     TASK_NAME = "librispeech_asr"
 
 
 class MultiCardSummarizationExampleTester(
     ExampleTesterBase, metaclass=ExampleTestMeta, example_name="run_summarization", multi_card=True
 ):
     TASK_NAME = "cnn_dailymail"
+
+
+class MultiCardSeq2SeqQuestionAnsweringExampleTester(
+    ExampleTesterBase, metaclass=ExampleTestMeta, example_name="run_seq2seq_qa", multi_card=True
+):
+    TASK_NAME = "squad_v2"
```

### Comparing `optimum-habana-1.5.1/tests/test_examples_match_transformers.py` & `optimum-habana-1.6.0/tests/test_examples_match_transformers.py`

 * *Files identical despite different names*

### Comparing `optimum-habana-1.5.1/tests/test_gaudi_configuration.py` & `optimum-habana-1.6.0/tests/test_gaudi_configuration.py`

 * *Files 2% similar despite different names*

```diff
@@ -50,14 +50,15 @@
     def test_default_parameter_types(self):
         gaudi_config = GaudiConfig()
 
         self.assertIsInstance(gaudi_config.use_habana_mixed_precision, bool)
         self.assertIsInstance(gaudi_config.hmp_is_verbose, bool)
         self.assertIsInstance(gaudi_config.use_fused_adam, bool)
         self.assertIsInstance(gaudi_config.use_fused_clip_norm, bool)
+        self.assertIsInstance(gaudi_config.use_torch_autocast, bool)
 
         self.assertTrue(is_list_of_strings(gaudi_config.hmp_bf16_ops))
         self.assertTrue(is_list_of_strings(gaudi_config.hmp_fp32_ops))
 
     def test_write_bf16_fp32_ops_to_text_files(self):
         gaudi_config = GaudiConfig()
```

### Comparing `optimum-habana-1.5.1/tests/test_trainer.py` & `optimum-habana-1.6.0/tests/test_trainer.py`

 * *Files 2% similar despite different names*

```diff
@@ -424,19 +424,23 @@
         trainer.train()
         self.default_trained_model = (trainer.model.a, trainer.model.b)
 
         trainer = get_regression_trainer(learning_rate=0.1, seed=314)
         trainer.train()
         self.alternate_trained_model = (trainer.model.a, trainer.model.b)
 
-    def check_trained_model(self, model, alternate_seed=False):
+    def check_trained_model(self, model, alternate_seed=False, bf16=False):
         # Checks a training seeded with learning_rate = 0.1
         (a, b) = self.alternate_trained_model if alternate_seed else self.default_trained_model
-        self.assertTrue(torch.allclose(model.a, a))
-        self.assertTrue(torch.allclose(model.b, b))
+        if not bf16:
+            self.assertTrue(torch.allclose(model.a, a))
+            self.assertTrue(torch.allclose(model.b, b))
+        else:
+            self.assertTrue(torch.allclose(model.a, a, atol=1e-03, rtol=0))
+            self.assertTrue(torch.allclose(model.b, b, atol=1e-03, rtol=0))
 
     def test_reproducible_training(self):
         # Checks that training worked, model trained and seed made a reproducible training.
         trainer = get_regression_trainer(learning_rate=0.1)
         trainer.train()
         self.check_trained_model(trainer.model)
 
@@ -562,23 +566,19 @@
 
         (a, b) = self.default_trained_model
         self.assertFalse(torch.allclose(trainer.model.a, a))
         self.assertFalse(torch.allclose(trainer.model.b, b))
         self.assertGreater(trainer.optimizer.state_dict()["param_groups"][0]["lr"], 0)
 
     def test_mixed_bf16(self):
-        # TODO: test HMP when it is easily possible to undo hmp.convert
-        # # very basic test
-        # trainer = get_regression_trainer(learning_rate=0.1, bf16=True)
-        # trainer.train()
-        # self.check_trained_model(trainer.model)
-
-        # --bf16 is not supported and should raise an error
-        with self.assertRaises(ValueError):
-            get_regression_trainer(learning_rate=0.1, bf16=True)
+        # very basic test
+        trainer = get_regression_trainer(learning_rate=0.1, bf16=True)
+        self.assertTrue(trainer.use_hpu_amp)
+        trainer.train()
+        self.check_trained_model(trainer.model, bf16=True)
 
 
 @require_torch
 @require_sentencepiece
 @require_tokenizers
 class GaudiTrainerIntegrationTest(TestCasePlus, GaudiTrainerIntegrationCommon):
     def setUp(self):
@@ -599,15 +599,21 @@
         _ = trainer.predict(eval_dataset)
 
     def test_hpu_graphs(self):
         train_dataset = RegressionDataset()
         eval_dataset = RegressionDataset()
         model = RegressionModel()
         gaudi_config = get_gaudi_config()
-        args = GaudiTrainingArguments("./regression", use_habana=True, use_lazy_mode=True, use_hpu_graphs=True)
+        args = GaudiTrainingArguments(
+            "./regression",
+            use_habana=True,
+            use_lazy_mode=True,
+            use_hpu_graphs_for_training=True,
+            use_hpu_graphs_for_inference=True,
+        )
         trainer = GaudiTrainer(model, gaudi_config, args, train_dataset=train_dataset, eval_dataset=eval_dataset)
         trainer.train()
         _ = trainer.evaluate()
         _ = trainer.predict(eval_dataset)
 
     def test_trainer_works_with_dict(self):
         train_dataset = RegressionDataset()
@@ -1605,14 +1611,19 @@
         wd_names = ['0.linear1.weight', '0.linear2.weight', '1.0.linear1.weight', '1.0.linear2.weight', '1.1.linear1.weight', '1.1.linear2.weight']
         # fmt: on
         wd_params = [p for n, p in model.named_parameters() if n in wd_names]
         no_wd_params = [p for n, p in model.named_parameters() if n not in wd_names]
         self.assertListEqual(trainer.optimizer.param_groups[0]["params"], wd_params)
         self.assertListEqual(trainer.optimizer.param_groups[1]["params"], no_wd_params)
 
+    def test_profiling(self):
+        # 24 total steps and compilation takes place during the 1st three steps
+        trainer = get_regression_trainer(profiling_warmup_steps=3, profiling_steps=21)
+        trainer.train()
+
 
 @require_torch
 @is_staging_test
 class GaudiTrainerIntegrationWithHubTester(unittest.TestCase):
     @classmethod
     def setUpClass(cls):
         cls._token = TOKEN
```

### Comparing `optimum-habana-1.5.1/tests/test_trainer_distributed.py` & `optimum-habana-1.6.0/tests/test_trainer_distributed.py`

 * *Files 7% similar despite different names*

```diff
@@ -58,36 +58,49 @@
             if labels is not None:
                 return torch.tensor(0.0, device=input_ids.device), input_ids
             else:
                 return input_ids
 
 
 class TestGaudiTrainerDistributed(TestCasePlus):
-    def test_gaudi_trainer_distributed(self):
+    def _test_gaudi_trainer_distributed(self, kwargs={}):
         output_dir = self.get_auto_remove_tmp_dir()
 
         command_list = [f"{self.test_file_dir}/test_trainer_distributed.py"]
         command_list += ["--output_dir"]
         command_list += [output_dir]
         command_list += ["--use_habana"]
         command_list += ["--use_lazy_mode"]
-        command_list += ["--use_hpu_graphs"]
+        for key, value in kwargs.items():
+            command_list += [f"--{key} {value}"]
         command = [" ".join(command_list)]
 
         distributed_runner = DistributedRunner(
             command_list=command,
             world_size=8,
             use_mpi=True,
         )
 
         ret_code = distributed_runner.run()
 
         # ret_code equals 0 or None if successful run
         self.assertTrue(ret_code == 0 or ret_code is None)
 
+    def test_gaudi_trainer_distributed(self):
+        self._test_gaudi_trainer_distributed()
+
+    def test_gaudi_trainer_distributed_hpu_graphs(self):
+        self._test_gaudi_trainer_distributed(
+            {
+                "use_hpu_graphs_for_training": "",
+                "use_hpu_graphs_for_inference": "",
+                "distribution_strategy": "fast_ddp",
+            }
+        )
+
 
 if __name__ == "__main__":
     # The script below is meant to be run under mpirun, on a machine with multiple HPUs:
     #
     # PYTHONPATH="src" python optimum-habana/examples/gaudi_spawn.py --world_size 8 --use_mpi --output_dir output_dir ./tests/test_trainer_distributed.py
 
     parser = HfArgumentParser((GaudiTrainingArguments,))
```

### Comparing `optimum-habana-1.5.1/tests/test_trainer_seq2seq.py` & `optimum-habana-1.6.0/tests/test_trainer_seq2seq.py`

 * *Files 2% similar despite different names*

```diff
@@ -47,16 +47,16 @@
             batch["input_ids"] = inputs.input_ids
             batch["attention_mask"] = inputs.attention_mask
 
             batch["decoder_input_ids"] = outputs.input_ids
             batch["labels"] = outputs.input_ids.copy()
             batch["decoder_attention_mask"] = outputs.attention_mask
 
-            assert all([len(x) == 512 for x in inputs.input_ids])
-            assert all([len(x) == 128 for x in outputs.input_ids])
+            assert all(len(x) == 512 for x in inputs.input_ids)
+            assert all(len(x) == 128 for x in outputs.input_ids)
 
             return batch
 
         def _compute_metrics(pred):
             labels_ids = pred.label_ids
             pred_ids = pred.predictions
 
@@ -100,15 +100,15 @@
             per_device_train_batch_size=batch_size,
             per_device_eval_batch_size=batch_size,
             predict_with_generate=True,
             do_train=True,
             do_eval=True,
             use_habana=True,
             use_lazy_mode=True,
-            use_hpu_graphs=True,
+            use_hpu_graphs_for_inference=True,
         )
 
         # instantiate trainer
         trainer = GaudiSeq2SeqTrainer(
             model=model,
             args=training_args,
             compute_metrics=_compute_metrics,
```

