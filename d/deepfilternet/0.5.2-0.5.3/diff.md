# Comparing `tmp/deepfilternet-0.5.2.tar.gz` & `tmp/deepfilternet-0.5.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "deepfilternet-0.5.2.tar", max compression
+gzip compressed data, was "deepfilternet-0.5.3.tar", max compression
```

## Comparing `deepfilternet-0.5.2.tar` & `deepfilternet-0.5.3.tar`

### file list

```diff
@@ -1,47 +1,47 @@
--rw-r--r--   0        0        0      495 2023-06-22 10:10:32.394557 deepfilternet-0.5.2/LICENSE
--rw-r--r--   0        0        0    10837 2023-06-22 10:10:32.394557 deepfilternet-0.5.2/LICENSE-APACHE
--rw-r--r--   0        0        0     1083 2023-06-22 10:10:32.394557 deepfilternet-0.5.2/LICENSE-MIT
--rw-r--r--   0        0        0      171 2023-06-22 10:10:32.394557 deepfilternet-0.5.2/df/__init__.py
--rw-r--r--   0        0        0     7976 2023-06-22 10:10:32.394557 deepfilternet-0.5.2/df/checkpoint.py
--rw-r--r--   0        0        0    10763 2023-06-22 10:10:32.394557 deepfilternet-0.5.2/df/config.py
--rw-r--r--   0        0        0    11383 2023-06-22 10:10:32.394557 deepfilternet-0.5.2/df/deepfilternet.py
--rw-r--r--   0        0        0    19236 2023-06-22 10:10:32.394557 deepfilternet-0.5.2/df/deepfilternet2.py
--rw-r--r--   0        0        0    16199 2023-06-22 10:10:32.394557 deepfilternet-0.5.2/df/deepfilternet3.py
--rw-r--r--   0        0        0    15869 2023-06-22 10:10:32.394557 deepfilternet-0.5.2/df/deepfilternetmf.py
--rw-r--r--   0        0        0    13830 2023-06-22 10:10:32.394557 deepfilternet-0.5.2/df/enhance.py
--rw-r--r--   0        0        0    23763 2023-06-22 10:10:32.394557 deepfilternet-0.5.2/df/evaluation_utils.py
--rw-r--r--   0        0        0     4105 2023-06-22 10:10:32.394557 deepfilternet-0.5.2/df/io.py
--rw-r--r--   0        0        0     7192 2023-06-22 10:10:32.394557 deepfilternet-0.5.2/df/logger.py
--rw-r--r--   0        0        0    33521 2023-06-22 10:10:32.394557 deepfilternet-0.5.2/df/loss.py
--rw-r--r--   0        0        0     1920 2023-06-22 10:10:32.394557 deepfilternet-0.5.2/df/lr.py
--rw-r--r--   0        0        0      779 2023-06-22 10:10:32.394557 deepfilternet-0.5.2/df/model.py
--rw-r--r--   0        0        0    36996 2023-06-22 10:10:32.394557 deepfilternet-0.5.2/df/modules.py
--rw-r--r--   0        0        0    24440 2023-06-22 10:10:32.394557 deepfilternet-0.5.2/df/multiframe.py
--rw-r--r--   0        0        0     8108 2023-06-22 10:10:32.394557 deepfilternet-0.5.2/df/scripts/dnsmos.py
--rw-r--r--   0        0        0     9722 2023-06-22 10:10:32.394557 deepfilternet-0.5.2/df/scripts/dnsmos_dns5.py
--rw-r--r--   0        0        0     3528 2023-06-22 10:10:32.394557 deepfilternet-0.5.2/df/scripts/dnsmos_v2.py
--rw-r--r--   0        0        0    10613 2023-06-22 10:10:32.394557 deepfilternet-0.5.2/df/scripts/export.py
--rw-r--r--   0        0        0     4376 2023-06-22 10:10:32.394557 deepfilternet-0.5.2/df/scripts/filter_dnsmos.py
--rw-r--r--   0        0        0     2267 2023-06-22 10:10:32.394557 deepfilternet-0.5.2/df/scripts/fix_n_samples_hdf5.py
--rw-r--r--   0        0        0      519 2023-06-22 10:10:32.394557 deepfilternet-0.5.2/df/scripts/list_attrs_in_hdf5.py
--rw-r--r--   0        0        0     1959 2023-06-22 10:10:32.394557 deepfilternet-0.5.2/df/scripts/model_summary.py
--rw-r--r--   0        0        0     2211 2023-06-22 10:10:32.394557 deepfilternet-0.5.2/df/scripts/plot_lrs.py
--rw-r--r--   0        0        0      636 2023-06-22 10:10:32.394557 deepfilternet-0.5.2/df/scripts/plot_spec.py
--rw-r--r--   0        0        0     4194 2023-06-22 10:10:32.394557 deepfilternet-0.5.2/df/scripts/plot_summaries.py
--rwxr-xr-x   0        0        0     8762 2023-06-22 10:10:32.394557 deepfilternet-0.5.2/df/scripts/prepare_data.py
--rw-r--r--   0        0        0      355 2023-06-22 10:10:32.394557 deepfilternet-0.5.2/df/scripts/print_model.py
--rw-r--r--   0        0        0     2423 2023-06-22 10:10:32.394557 deepfilternet-0.5.2/df/scripts/sample_from_hdf5.py
--rw-r--r--   0        0        0     2393 2023-06-22 10:10:32.394557 deepfilternet-0.5.2/df/scripts/split_hdf5.py
--rwxr-xr-x   0        0        0     4608 2023-06-22 10:10:32.394557 deepfilternet-0.5.2/df/scripts/test_df.py
--rw-r--r--   0        0        0     2535 2023-06-22 10:10:32.394557 deepfilternet-0.5.2/df/scripts/test_dns_2020.py
--rw-r--r--   0        0        0     2312 2023-06-22 10:10:32.394557 deepfilternet-0.5.2/df/scripts/test_noisy_dnsmos.py
--rw-r--r--   0        0        0     2592 2023-06-22 10:10:32.394557 deepfilternet-0.5.2/df/scripts/test_voicebank_demand.py
--rw-r--r--   0        0        0     3109 2023-06-22 10:10:32.394557 deepfilternet-0.5.2/df/scripts/trim_silence_hdf5.py
--rw-r--r--   0        0        0    17442 2023-06-22 10:10:32.394557 deepfilternet-0.5.2/df/sepm.py
--rw-r--r--   0        0        0     9474 2023-06-22 10:10:32.394557 deepfilternet-0.5.2/df/stoi.py
--rw-r--r--   0        0        0    23584 2023-06-22 10:10:32.394557 deepfilternet-0.5.2/df/train.py
--rw-r--r--   0        0        0     7430 2023-06-22 10:10:32.394557 deepfilternet-0.5.2/df/utils.py
--rw-r--r--   0        0        0      884 2023-06-22 10:10:32.394557 deepfilternet-0.5.2/df/version.py
--rw-r--r--   0        0        0     3566 2023-06-22 10:10:32.394557 deepfilternet-0.5.2/df/visualization.py
--rw-r--r--   0        0        0     2450 2023-06-22 10:10:32.398557 deepfilternet-0.5.2/pyproject.toml
--rw-r--r--   0        0        0     1707 1970-01-01 00:00:00.000000 deepfilternet-0.5.2/PKG-INFO
+-rw-r--r--   0        0        0      495 2023-06-26 10:29:39.157300 deepfilternet-0.5.3/LICENSE
+-rw-r--r--   0        0        0    10837 2023-06-26 10:29:39.157300 deepfilternet-0.5.3/LICENSE-APACHE
+-rw-r--r--   0        0        0     1083 2023-06-26 10:29:39.157300 deepfilternet-0.5.3/LICENSE-MIT
+-rw-r--r--   0        0        0      171 2023-06-26 10:29:39.157300 deepfilternet-0.5.3/df/__init__.py
+-rw-r--r--   0        0        0     7976 2023-06-26 10:29:39.157300 deepfilternet-0.5.3/df/checkpoint.py
+-rw-r--r--   0        0        0    10763 2023-06-26 10:29:39.157300 deepfilternet-0.5.3/df/config.py
+-rw-r--r--   0        0        0    11383 2023-06-26 10:29:39.157300 deepfilternet-0.5.3/df/deepfilternet.py
+-rw-r--r--   0        0        0    19236 2023-06-26 10:29:39.157300 deepfilternet-0.5.3/df/deepfilternet2.py
+-rw-r--r--   0        0        0    16199 2023-06-26 10:29:39.157300 deepfilternet-0.5.3/df/deepfilternet3.py
+-rw-r--r--   0        0        0    15869 2023-06-26 10:29:39.157300 deepfilternet-0.5.3/df/deepfilternetmf.py
+-rw-r--r--   0        0        0    13830 2023-06-26 10:29:39.157300 deepfilternet-0.5.3/df/enhance.py
+-rw-r--r--   0        0        0    23763 2023-06-26 10:29:39.157300 deepfilternet-0.5.3/df/evaluation_utils.py
+-rw-r--r--   0        0        0     4105 2023-06-26 10:29:39.157300 deepfilternet-0.5.3/df/io.py
+-rw-r--r--   0        0        0     7192 2023-06-26 10:29:39.157300 deepfilternet-0.5.3/df/logger.py
+-rw-r--r--   0        0        0    33521 2023-06-26 10:29:39.157300 deepfilternet-0.5.3/df/loss.py
+-rw-r--r--   0        0        0     1920 2023-06-26 10:29:39.157300 deepfilternet-0.5.3/df/lr.py
+-rw-r--r--   0        0        0      779 2023-06-26 10:29:39.157300 deepfilternet-0.5.3/df/model.py
+-rw-r--r--   0        0        0    36996 2023-06-26 10:29:39.157300 deepfilternet-0.5.3/df/modules.py
+-rw-r--r--   0        0        0    24440 2023-06-26 10:29:39.157300 deepfilternet-0.5.3/df/multiframe.py
+-rw-r--r--   0        0        0     8108 2023-06-26 10:29:39.157300 deepfilternet-0.5.3/df/scripts/dnsmos.py
+-rw-r--r--   0        0        0     9722 2023-06-26 10:29:39.157300 deepfilternet-0.5.3/df/scripts/dnsmos_dns5.py
+-rw-r--r--   0        0        0     3528 2023-06-26 10:29:39.157300 deepfilternet-0.5.3/df/scripts/dnsmos_v2.py
+-rw-r--r--   0        0        0    10613 2023-06-26 10:29:39.157300 deepfilternet-0.5.3/df/scripts/export.py
+-rw-r--r--   0        0        0     4376 2023-06-26 10:29:39.157300 deepfilternet-0.5.3/df/scripts/filter_dnsmos.py
+-rw-r--r--   0        0        0     2267 2023-06-26 10:29:39.157300 deepfilternet-0.5.3/df/scripts/fix_n_samples_hdf5.py
+-rw-r--r--   0        0        0      519 2023-06-26 10:29:39.157300 deepfilternet-0.5.3/df/scripts/list_attrs_in_hdf5.py
+-rw-r--r--   0        0        0     1959 2023-06-26 10:29:39.157300 deepfilternet-0.5.3/df/scripts/model_summary.py
+-rw-r--r--   0        0        0     2211 2023-06-26 10:29:39.157300 deepfilternet-0.5.3/df/scripts/plot_lrs.py
+-rw-r--r--   0        0        0      636 2023-06-26 10:29:39.157300 deepfilternet-0.5.3/df/scripts/plot_spec.py
+-rw-r--r--   0        0        0     4194 2023-06-26 10:29:39.157300 deepfilternet-0.5.3/df/scripts/plot_summaries.py
+-rwxr-xr-x   0        0        0     8762 2023-06-26 10:29:39.157300 deepfilternet-0.5.3/df/scripts/prepare_data.py
+-rw-r--r--   0        0        0      355 2023-06-26 10:29:39.157300 deepfilternet-0.5.3/df/scripts/print_model.py
+-rw-r--r--   0        0        0     2423 2023-06-26 10:29:39.157300 deepfilternet-0.5.3/df/scripts/sample_from_hdf5.py
+-rw-r--r--   0        0        0     2393 2023-06-26 10:29:39.157300 deepfilternet-0.5.3/df/scripts/split_hdf5.py
+-rwxr-xr-x   0        0        0     4608 2023-06-26 10:29:39.157300 deepfilternet-0.5.3/df/scripts/test_df.py
+-rw-r--r--   0        0        0     2535 2023-06-26 10:29:39.157300 deepfilternet-0.5.3/df/scripts/test_dns_2020.py
+-rw-r--r--   0        0        0     2312 2023-06-26 10:29:39.157300 deepfilternet-0.5.3/df/scripts/test_noisy_dnsmos.py
+-rw-r--r--   0        0        0     2592 2023-06-26 10:29:39.157300 deepfilternet-0.5.3/df/scripts/test_voicebank_demand.py
+-rw-r--r--   0        0        0     3109 2023-06-26 10:29:39.157300 deepfilternet-0.5.3/df/scripts/trim_silence_hdf5.py
+-rw-r--r--   0        0        0    17442 2023-06-26 10:29:39.157300 deepfilternet-0.5.3/df/sepm.py
+-rw-r--r--   0        0        0     9474 2023-06-26 10:29:39.161300 deepfilternet-0.5.3/df/stoi.py
+-rw-r--r--   0        0        0    23584 2023-06-26 10:29:39.161300 deepfilternet-0.5.3/df/train.py
+-rw-r--r--   0        0        0     7430 2023-06-26 10:29:39.161300 deepfilternet-0.5.3/df/utils.py
+-rw-r--r--   0        0        0      884 2023-06-26 10:29:39.161300 deepfilternet-0.5.3/df/version.py
+-rw-r--r--   0        0        0     3566 2023-06-26 10:29:39.161300 deepfilternet-0.5.3/df/visualization.py
+-rw-r--r--   0        0        0     2450 2023-06-26 10:29:39.161300 deepfilternet-0.5.3/pyproject.toml
+-rw-r--r--   0        0        0     1707 1970-01-01 00:00:00.000000 deepfilternet-0.5.3/PKG-INFO
```

### Comparing `deepfilternet-0.5.2/LICENSE-APACHE` & `deepfilternet-0.5.3/LICENSE-APACHE`

 * *Files identical despite different names*

### Comparing `deepfilternet-0.5.2/LICENSE-MIT` & `deepfilternet-0.5.3/LICENSE-MIT`

 * *Files identical despite different names*

### Comparing `deepfilternet-0.5.2/df/checkpoint.py` & `deepfilternet-0.5.3/df/checkpoint.py`

 * *Files identical despite different names*

### Comparing `deepfilternet-0.5.2/df/config.py` & `deepfilternet-0.5.3/df/config.py`

 * *Files identical despite different names*

### Comparing `deepfilternet-0.5.2/df/deepfilternet.py` & `deepfilternet-0.5.3/df/deepfilternet.py`

 * *Files identical despite different names*

### Comparing `deepfilternet-0.5.2/df/deepfilternet2.py` & `deepfilternet-0.5.3/df/deepfilternet2.py`

 * *Files identical despite different names*

### Comparing `deepfilternet-0.5.2/df/deepfilternet3.py` & `deepfilternet-0.5.3/df/deepfilternet3.py`

 * *Files identical despite different names*

### Comparing `deepfilternet-0.5.2/df/deepfilternetmf.py` & `deepfilternet-0.5.3/df/deepfilternetmf.py`

 * *Files identical despite different names*

### Comparing `deepfilternet-0.5.2/df/enhance.py` & `deepfilternet-0.5.3/df/enhance.py`

 * *Files identical despite different names*

### Comparing `deepfilternet-0.5.2/df/evaluation_utils.py` & `deepfilternet-0.5.3/df/evaluation_utils.py`

 * *Files identical despite different names*

### Comparing `deepfilternet-0.5.2/df/io.py` & `deepfilternet-0.5.3/df/io.py`

 * *Files identical despite different names*

### Comparing `deepfilternet-0.5.2/df/logger.py` & `deepfilternet-0.5.3/df/logger.py`

 * *Files identical despite different names*

### Comparing `deepfilternet-0.5.2/df/loss.py` & `deepfilternet-0.5.3/df/loss.py`

 * *Files identical despite different names*

### Comparing `deepfilternet-0.5.2/df/lr.py` & `deepfilternet-0.5.3/df/lr.py`

 * *Files identical despite different names*

### Comparing `deepfilternet-0.5.2/df/model.py` & `deepfilternet-0.5.3/df/model.py`

 * *Files identical despite different names*

### Comparing `deepfilternet-0.5.2/df/modules.py` & `deepfilternet-0.5.3/df/modules.py`

 * *Files identical despite different names*

### Comparing `deepfilternet-0.5.2/df/multiframe.py` & `deepfilternet-0.5.3/df/multiframe.py`

 * *Files identical despite different names*

### Comparing `deepfilternet-0.5.2/df/scripts/dnsmos.py` & `deepfilternet-0.5.3/df/scripts/dnsmos.py`

 * *Files identical despite different names*

### Comparing `deepfilternet-0.5.2/df/scripts/dnsmos_dns5.py` & `deepfilternet-0.5.3/df/scripts/dnsmos_dns5.py`

 * *Files identical despite different names*

### Comparing `deepfilternet-0.5.2/df/scripts/dnsmos_v2.py` & `deepfilternet-0.5.3/df/scripts/dnsmos_v2.py`

 * *Files identical despite different names*

### Comparing `deepfilternet-0.5.2/df/scripts/export.py` & `deepfilternet-0.5.3/df/scripts/export.py`

 * *Files identical despite different names*

### Comparing `deepfilternet-0.5.2/df/scripts/filter_dnsmos.py` & `deepfilternet-0.5.3/df/scripts/filter_dnsmos.py`

 * *Files identical despite different names*

### Comparing `deepfilternet-0.5.2/df/scripts/fix_n_samples_hdf5.py` & `deepfilternet-0.5.3/df/scripts/fix_n_samples_hdf5.py`

 * *Files identical despite different names*

### Comparing `deepfilternet-0.5.2/df/scripts/list_attrs_in_hdf5.py` & `deepfilternet-0.5.3/df/scripts/list_attrs_in_hdf5.py`

 * *Files identical despite different names*

### Comparing `deepfilternet-0.5.2/df/scripts/model_summary.py` & `deepfilternet-0.5.3/df/scripts/model_summary.py`

 * *Files identical despite different names*

### Comparing `deepfilternet-0.5.2/df/scripts/plot_lrs.py` & `deepfilternet-0.5.3/df/scripts/plot_lrs.py`

 * *Files identical despite different names*

### Comparing `deepfilternet-0.5.2/df/scripts/plot_spec.py` & `deepfilternet-0.5.3/df/scripts/plot_spec.py`

 * *Files identical despite different names*

### Comparing `deepfilternet-0.5.2/df/scripts/plot_summaries.py` & `deepfilternet-0.5.3/df/scripts/plot_summaries.py`

 * *Files identical despite different names*

### Comparing `deepfilternet-0.5.2/df/scripts/prepare_data.py` & `deepfilternet-0.5.3/df/scripts/prepare_data.py`

 * *Files identical despite different names*

### Comparing `deepfilternet-0.5.2/df/scripts/sample_from_hdf5.py` & `deepfilternet-0.5.3/df/scripts/sample_from_hdf5.py`

 * *Files identical despite different names*

### Comparing `deepfilternet-0.5.2/df/scripts/split_hdf5.py` & `deepfilternet-0.5.3/df/scripts/split_hdf5.py`

 * *Files identical despite different names*

### Comparing `deepfilternet-0.5.2/df/scripts/test_df.py` & `deepfilternet-0.5.3/df/scripts/test_df.py`

 * *Files identical despite different names*

### Comparing `deepfilternet-0.5.2/df/scripts/test_dns_2020.py` & `deepfilternet-0.5.3/df/scripts/test_dns_2020.py`

 * *Files identical despite different names*

### Comparing `deepfilternet-0.5.2/df/scripts/test_noisy_dnsmos.py` & `deepfilternet-0.5.3/df/scripts/test_noisy_dnsmos.py`

 * *Files identical despite different names*

### Comparing `deepfilternet-0.5.2/df/scripts/test_voicebank_demand.py` & `deepfilternet-0.5.3/df/scripts/test_voicebank_demand.py`

 * *Files identical despite different names*

### Comparing `deepfilternet-0.5.2/df/scripts/trim_silence_hdf5.py` & `deepfilternet-0.5.3/df/scripts/trim_silence_hdf5.py`

 * *Files identical despite different names*

### Comparing `deepfilternet-0.5.2/df/sepm.py` & `deepfilternet-0.5.3/df/sepm.py`

 * *Files identical despite different names*

### Comparing `deepfilternet-0.5.2/df/stoi.py` & `deepfilternet-0.5.3/df/stoi.py`

 * *Files identical despite different names*

### Comparing `deepfilternet-0.5.2/df/train.py` & `deepfilternet-0.5.3/df/train.py`

 * *Files identical despite different names*

### Comparing `deepfilternet-0.5.2/df/utils.py` & `deepfilternet-0.5.3/df/utils.py`

 * *Files identical despite different names*

### Comparing `deepfilternet-0.5.2/df/version.py` & `deepfilternet-0.5.3/df/version.py`

 * *Files identical despite different names*

### Comparing `deepfilternet-0.5.2/df/visualization.py` & `deepfilternet-0.5.3/df/visualization.py`

 * *Files identical despite different names*

### Comparing `deepfilternet-0.5.2/pyproject.toml` & `deepfilternet-0.5.3/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "DeepFilterNet"
-version = "0.5.2"
+version = "0.5.3"
 description = "Noise supression using deep filtering"
 authors = ["Hendrik Schröter"]
 repository = "https://github.com/Rikorose/DeepFilterNet"
 keywords = ["noise reduction", "neural network"]
 classifiers = [
   "Topic :: Multimedia :: Sound/Audio :: Speech",
   "Topic :: Software Development :: Libraries :: Python Modules",
@@ -19,16 +19,16 @@
   { path = "pretrained_models/DeepFilterNet/config.ini" },
   { path = "pretrained_models/DeepFilterNet/checkpoints/*" },
   { path = "pretrained_models/DeepFilterNet2/config.ini" },
   { path = "pretrained_models/DeepFilterNet2/checkpoints/*" },
 ]
 
 [tool.poetry.dependencies]
-deepfilterlib = "0.5.2"
-deepfilterdataloader = { version = "0.5.2", optional = true }
+deepfilterlib = "0.5.3"
+deepfilterdataloader = { version = "0.5.3", optional = true }
 python = ">=3.8,<4.0"
 numpy = ">=1.22,<2.0"
 loguru = ">=0.5"
 appdirs = "^1.4"
 requests = "^2.27"
 packaging = "^23.0"
 sympy = ">=1.6"
```

### Comparing `deepfilternet-0.5.2/PKG-INFO` & `deepfilternet-0.5.3/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: deepfilternet
-Version: 0.5.2
+Version: 0.5.3
 Summary: Noise supression using deep filtering
 Home-page: https://github.com/Rikorose/DeepFilterNet
 License: MIT
 Keywords: noise reduction,neural network
 Author: Hendrik Schröter
 Requires-Python: >=3.8,<4.0
 Classifier: License :: OSI Approved :: MIT License
@@ -20,16 +20,16 @@
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Classifier: Topic :: Utilities
 Provides-Extra: dnsmos-local
 Provides-Extra: eval
 Provides-Extra: soundfile
 Provides-Extra: train
 Requires-Dist: appdirs (>=1.4,<2.0)
-Requires-Dist: deepfilterdataloader (==0.5.2) ; extra == "train"
-Requires-Dist: deepfilterlib (==0.5.2)
+Requires-Dist: deepfilterdataloader (==0.5.3) ; extra == "train"
+Requires-Dist: deepfilterlib (==0.5.3)
 Requires-Dist: icecream (>=2,<3) ; extra == "train"
 Requires-Dist: loguru (>=0.5)
 Requires-Dist: numpy (>=1.22,<2.0)
 Requires-Dist: onnxruntime (>=1.15,<2.0) ; extra == "dnsmos-local"
 Requires-Dist: packaging (>=23.0,<24.0)
 Requires-Dist: pesq (>=0.0.3,<0.0.5) ; extra == "eval"
 Requires-Dist: pystoi (>=0.3,<0.4) ; extra == "eval"
```

