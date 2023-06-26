# Comparing `tmp/sev-snp-measure-0.0.6.tar.gz` & `tmp/sev-snp-measure-0.0.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sev-snp-measure-0.0.6.tar", last modified: Mon Jun 12 05:30:37 2023, max compression
+gzip compressed data, was "sev-snp-measure-0.0.7.tar", last modified: Mon Jun 26 21:04:18 2023, max compression
```

## Comparing `sev-snp-measure-0.0.6.tar` & `sev-snp-measure-0.0.7.tar`

### file list

```diff
@@ -1,29 +1,29 @@
-drwxr-xr-x   0 dubek     (1000) dubek     (1000)        0 2023-06-12 05:30:37.365026 sev-snp-measure-0.0.6/
--rw-r--r--   0 dubek     (1000) dubek     (1000)    11358 2022-03-09 13:11:47.000000 sev-snp-measure-0.0.6/LICENSE
--rw-r--r--   0 dubek     (1000) dubek     (1000)     7370 2023-06-12 05:30:37.365026 sev-snp-measure-0.0.6/PKG-INFO
--rw-r--r--   0 dubek     (1000) dubek     (1000)     6625 2023-06-09 08:37:27.000000 sev-snp-measure-0.0.6/README.md
--rw-r--r--   0 dubek     (1000) dubek     (1000)       85 2022-04-11 09:47:58.000000 sev-snp-measure-0.0.6/pyproject.toml
--rw-r--r--   0 dubek     (1000) dubek     (1000)      973 2023-06-12 05:30:37.365026 sev-snp-measure-0.0.6/setup.cfg
-drwxr-xr-x   0 dubek     (1000) dubek     (1000)        0 2023-06-12 05:30:37.365026 sev-snp-measure-0.0.6/sev_snp_measure.egg-info/
--rw-r--r--   0 dubek     (1000) dubek     (1000)     7370 2023-06-12 05:30:37.000000 sev-snp-measure-0.0.6/sev_snp_measure.egg-info/PKG-INFO
--rw-r--r--   0 dubek     (1000) dubek     (1000)      617 2023-06-12 05:30:37.000000 sev-snp-measure-0.0.6/sev_snp_measure.egg-info/SOURCES.txt
--rw-r--r--   0 dubek     (1000) dubek     (1000)        1 2023-06-12 05:30:37.000000 sev-snp-measure-0.0.6/sev_snp_measure.egg-info/dependency_links.txt
--rw-r--r--   0 dubek     (1000) dubek     (1000)      109 2023-06-12 05:30:37.000000 sev-snp-measure-0.0.6/sev_snp_measure.egg-info/entry_points.txt
--rw-r--r--   0 dubek     (1000) dubek     (1000)       40 2023-06-12 05:30:37.000000 sev-snp-measure-0.0.6/sev_snp_measure.egg-info/requires.txt
--rw-r--r--   0 dubek     (1000) dubek     (1000)       14 2023-06-12 05:30:37.000000 sev-snp-measure-0.0.6/sev_snp_measure.egg-info/top_level.txt
-drwxr-xr-x   0 dubek     (1000) dubek     (1000)        0 2023-06-12 05:30:37.365026 sev-snp-measure-0.0.6/sevsnpmeasure/
--rw-r--r--   0 dubek     (1000) dubek     (1000)       89 2022-03-09 13:11:47.000000 sev-snp-measure-0.0.6/sevsnpmeasure/__init__.py
--rw-r--r--   0 dubek     (1000) dubek     (1000)     4647 2023-06-12 05:25:14.000000 sev-snp-measure-0.0.6/sevsnpmeasure/cli.py
--rw-r--r--   0 dubek     (1000) dubek     (1000)     2462 2023-04-10 12:16:34.000000 sev-snp-measure-0.0.6/sevsnpmeasure/gctx.py
--rw-r--r--   0 dubek     (1000) dubek     (1000)     5303 2023-06-08 08:08:31.000000 sev-snp-measure-0.0.6/sevsnpmeasure/guest.py
--rw-r--r--   0 dubek     (1000) dubek     (1000)     5638 2023-06-08 05:52:47.000000 sev-snp-measure-0.0.6/sevsnpmeasure/id_block.py
--rw-r--r--   0 dubek     (1000) dubek     (1000)     5078 2023-06-08 08:08:31.000000 sev-snp-measure-0.0.6/sevsnpmeasure/ovmf.py
--rw-r--r--   0 dubek     (1000) dubek     (1000)     3488 2023-06-08 09:35:10.000000 sev-snp-measure-0.0.6/sevsnpmeasure/sev_hashes.py
--rw-r--r--   0 dubek     (1000) dubek     (1000)      600 2022-04-24 09:17:37.000000 sev-snp-measure-0.0.6/sevsnpmeasure/sev_mode.py
--rw-r--r--   0 dubek     (1000) dubek     (1000)     1732 2023-05-28 09:56:41.000000 sev-snp-measure-0.0.6/sevsnpmeasure/vcpu_types.py
--rw-r--r--   0 dubek     (1000) dubek     (1000)       70 2023-05-22 17:48:16.000000 sev-snp-measure-0.0.6/sevsnpmeasure/vmm_types.py
--rw-r--r--   0 dubek     (1000) dubek     (1000)     6338 2023-05-22 17:48:16.000000 sev-snp-measure-0.0.6/sevsnpmeasure/vmsa.py
-drwxr-xr-x   0 dubek     (1000) dubek     (1000)        0 2023-06-12 05:30:37.365026 sev-snp-measure-0.0.6/tests/
--rw-r--r--   0 dubek     (1000) dubek     (1000)     8260 2023-06-09 08:37:27.000000 sev-snp-measure-0.0.6/tests/test_guest.py
--rw-r--r--   0 dubek     (1000) dubek     (1000)     1149 2023-04-13 07:47:31.000000 sev-snp-measure-0.0.6/tests/test_id_block.py
--rw-r--r--   0 dubek     (1000) dubek     (1000)      480 2022-06-08 12:42:41.000000 sev-snp-measure-0.0.6/tests/test_vcpu_types.py
+drwxr-xr-x   0 dubek     (1000) dubek     (1000)        0 2023-06-26 21:04:18.384427 sev-snp-measure-0.0.7/
+-rw-r--r--   0 dubek     (1000) dubek     (1000)    11358 2023-06-26 06:28:50.000000 sev-snp-measure-0.0.7/LICENSE
+-rw-r--r--   0 dubek     (1000) dubek     (1000)     7393 2023-06-26 21:04:18.384427 sev-snp-measure-0.0.7/PKG-INFO
+-rw-r--r--   0 dubek     (1000) dubek     (1000)     6631 2023-06-26 20:59:58.000000 sev-snp-measure-0.0.7/README.md
+-rw-r--r--   0 dubek     (1000) dubek     (1000)       85 2023-06-26 06:28:50.000000 sev-snp-measure-0.0.7/pyproject.toml
+-rw-r--r--   0 dubek     (1000) dubek     (1000)      990 2023-06-26 21:04:18.384427 sev-snp-measure-0.0.7/setup.cfg
+drwxr-xr-x   0 dubek     (1000) dubek     (1000)        0 2023-06-26 21:04:18.384427 sev-snp-measure-0.0.7/sev_snp_measure.egg-info/
+-rw-r--r--   0 dubek     (1000) dubek     (1000)     7393 2023-06-26 21:04:18.000000 sev-snp-measure-0.0.7/sev_snp_measure.egg-info/PKG-INFO
+-rw-r--r--   0 dubek     (1000) dubek     (1000)      617 2023-06-26 21:04:18.000000 sev-snp-measure-0.0.7/sev_snp_measure.egg-info/SOURCES.txt
+-rw-r--r--   0 dubek     (1000) dubek     (1000)        1 2023-06-26 21:04:18.000000 sev-snp-measure-0.0.7/sev_snp_measure.egg-info/dependency_links.txt
+-rw-r--r--   0 dubek     (1000) dubek     (1000)      109 2023-06-26 21:04:18.000000 sev-snp-measure-0.0.7/sev_snp_measure.egg-info/entry_points.txt
+-rw-r--r--   0 dubek     (1000) dubek     (1000)       40 2023-06-26 21:04:18.000000 sev-snp-measure-0.0.7/sev_snp_measure.egg-info/requires.txt
+-rw-r--r--   0 dubek     (1000) dubek     (1000)       14 2023-06-26 21:04:18.000000 sev-snp-measure-0.0.7/sev_snp_measure.egg-info/top_level.txt
+drwxr-xr-x   0 dubek     (1000) dubek     (1000)        0 2023-06-26 21:04:18.384427 sev-snp-measure-0.0.7/sevsnpmeasure/
+-rw-r--r--   0 dubek     (1000) dubek     (1000)       89 2023-06-26 06:28:50.000000 sev-snp-measure-0.0.7/sevsnpmeasure/__init__.py
+-rw-r--r--   0 dubek     (1000) dubek     (1000)     4647 2023-06-26 21:01:31.000000 sev-snp-measure-0.0.7/sevsnpmeasure/cli.py
+-rw-r--r--   0 dubek     (1000) dubek     (1000)     2462 2023-06-26 06:28:50.000000 sev-snp-measure-0.0.7/sevsnpmeasure/gctx.py
+-rw-r--r--   0 dubek     (1000) dubek     (1000)     5303 2023-06-26 06:28:50.000000 sev-snp-measure-0.0.7/sevsnpmeasure/guest.py
+-rw-r--r--   0 dubek     (1000) dubek     (1000)     5638 2023-06-26 06:28:50.000000 sev-snp-measure-0.0.7/sevsnpmeasure/id_block.py
+-rw-r--r--   0 dubek     (1000) dubek     (1000)     5078 2023-06-26 06:28:50.000000 sev-snp-measure-0.0.7/sevsnpmeasure/ovmf.py
+-rw-r--r--   0 dubek     (1000) dubek     (1000)     3488 2023-06-26 06:28:50.000000 sev-snp-measure-0.0.7/sevsnpmeasure/sev_hashes.py
+-rw-r--r--   0 dubek     (1000) dubek     (1000)      600 2023-06-26 06:28:50.000000 sev-snp-measure-0.0.7/sevsnpmeasure/sev_mode.py
+-rw-r--r--   0 dubek     (1000) dubek     (1000)     1732 2023-06-26 06:28:50.000000 sev-snp-measure-0.0.7/sevsnpmeasure/vcpu_types.py
+-rw-r--r--   0 dubek     (1000) dubek     (1000)       70 2023-06-26 06:28:50.000000 sev-snp-measure-0.0.7/sevsnpmeasure/vmm_types.py
+-rw-r--r--   0 dubek     (1000) dubek     (1000)     6338 2023-06-26 06:28:50.000000 sev-snp-measure-0.0.7/sevsnpmeasure/vmsa.py
+drwxr-xr-x   0 dubek     (1000) dubek     (1000)        0 2023-06-26 21:04:18.384427 sev-snp-measure-0.0.7/tests/
+-rw-r--r--   0 dubek     (1000) dubek     (1000)     8260 2023-06-26 06:28:50.000000 sev-snp-measure-0.0.7/tests/test_guest.py
+-rw-r--r--   0 dubek     (1000) dubek     (1000)     1149 2023-06-26 06:28:50.000000 sev-snp-measure-0.0.7/tests/test_id_block.py
+-rw-r--r--   0 dubek     (1000) dubek     (1000)      480 2023-06-26 06:28:50.000000 sev-snp-measure-0.0.7/tests/test_vcpu_types.py
```

### Comparing `sev-snp-measure-0.0.6/LICENSE` & `sev-snp-measure-0.0.7/LICENSE`

 * *Files identical despite different names*

### Comparing `sev-snp-measure-0.0.6/PKG-INFO` & `sev-snp-measure-0.0.7/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 Metadata-Version: 2.1
 Name: sev-snp-measure
-Version: 0.0.6
-Summary: Calculate expected measurement of an AMD SEV-SNP guest VM for confidential computing
-Home-page: https://github.com/IBM/sev-snp-measure
+Version: 0.0.7
+Summary: Calculate expected measurement of an AMD SEV/SEV-ES/SEV-SNP guest VM for confidential computing
+Home-page: https://github.com/virtee/sev-snp-measure
 Author: Dov Murik
 Author-email: dov.murik1@il.ibm.com
-Project-URL: Bug Tracker, https://github.com/IBM/sev-snp-measure/issues
+Project-URL: Bug Tracker, https://github.com/virtee/sev-snp-measure/issues
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: OS Independent
 Classifier: Topic :: Security
 Classifier: Topic :: Software Development :: Libraries
@@ -35,15 +35,15 @@
 This installs the `sevsnpmeasure` package and the `sev-snp-measure`
 command-line script.
 
 ### From Github
 
 Clone the Github repo and run the script directly from the local directory:
 
-    git clone https://github.com/IBM/sev-snp-measure.git
+    git clone https://github.com/virtee/sev-snp-measure.git
     cd sev-snp-measure
     ./sev-snp-measure.py --help
 
 ## Command-line usage
 
 ### sev-snp-measure
 ```
@@ -185,14 +185,14 @@
 
     pip install flake8
     make lint
 
 ## Notes
 
 If you have any questions or issues you can create a new [issue
-here](https://github.com/IBM/sev-snp-measure/issues/new)
+here](https://github.com/virtee/sev-snp-measure/issues/new)
 
 Pull requests are welcome!
 
 ## License
 
 Apache 2.0 license.
```

### Comparing `sev-snp-measure-0.0.6/README.md` & `sev-snp-measure-0.0.7/README.md`

 * *Files 3% similar despite different names*

```diff
@@ -16,15 +16,15 @@
 This installs the `sevsnpmeasure` package and the `sev-snp-measure`
 command-line script.
 
 ### From Github
 
 Clone the Github repo and run the script directly from the local directory:
 
-    git clone https://github.com/IBM/sev-snp-measure.git
+    git clone https://github.com/virtee/sev-snp-measure.git
     cd sev-snp-measure
     ./sev-snp-measure.py --help
 
 ## Command-line usage
 
 ### sev-snp-measure
 ```
@@ -166,14 +166,14 @@
 
     pip install flake8
     make lint
 
 ## Notes
 
 If you have any questions or issues you can create a new [issue
-here](https://github.com/IBM/sev-snp-measure/issues/new)
+here](https://github.com/virtee/sev-snp-measure/issues/new)
 
 Pull requests are welcome!
 
 ## License
 
 Apache 2.0 license.
```

### Comparing `sev-snp-measure-0.0.6/setup.cfg` & `sev-snp-measure-0.0.7/setup.cfg`

 * *Files 24% similar despite different names*

```diff
@@ -1,18 +1,18 @@
 [metadata]
 name = sev-snp-measure
-version = 0.0.6
+version = 0.0.7
 author = Dov Murik
 author_email = dov.murik1@il.ibm.com
-description = Calculate expected measurement of an AMD SEV-SNP guest VM for confidential computing
+description = Calculate expected measurement of an AMD SEV/SEV-ES/SEV-SNP guest VM for confidential computing
 long_description = file: README.md
 long_description_content_type = text/markdown
-url = https://github.com/IBM/sev-snp-measure
+url = https://github.com/virtee/sev-snp-measure
 project_urls = 
-	Bug Tracker = https://github.com/IBM/sev-snp-measure/issues
+	Bug Tracker = https://github.com/virtee/sev-snp-measure/issues
 classifiers = 
 	Development Status :: 4 - Beta
 	Intended Audience :: Developers
 	License :: OSI Approved :: Apache Software License
 	Programming Language :: Python :: 3
 	Operating System :: OS Independent
 	Topic :: Security
```

### Comparing `sev-snp-measure-0.0.6/sev_snp_measure.egg-info/PKG-INFO` & `sev-snp-measure-0.0.7/sev_snp_measure.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 Metadata-Version: 2.1
 Name: sev-snp-measure
-Version: 0.0.6
-Summary: Calculate expected measurement of an AMD SEV-SNP guest VM for confidential computing
-Home-page: https://github.com/IBM/sev-snp-measure
+Version: 0.0.7
+Summary: Calculate expected measurement of an AMD SEV/SEV-ES/SEV-SNP guest VM for confidential computing
+Home-page: https://github.com/virtee/sev-snp-measure
 Author: Dov Murik
 Author-email: dov.murik1@il.ibm.com
-Project-URL: Bug Tracker, https://github.com/IBM/sev-snp-measure/issues
+Project-URL: Bug Tracker, https://github.com/virtee/sev-snp-measure/issues
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: OS Independent
 Classifier: Topic :: Security
 Classifier: Topic :: Software Development :: Libraries
@@ -35,15 +35,15 @@
 This installs the `sevsnpmeasure` package and the `sev-snp-measure`
 command-line script.
 
 ### From Github
 
 Clone the Github repo and run the script directly from the local directory:
 
-    git clone https://github.com/IBM/sev-snp-measure.git
+    git clone https://github.com/virtee/sev-snp-measure.git
     cd sev-snp-measure
     ./sev-snp-measure.py --help
 
 ## Command-line usage
 
 ### sev-snp-measure
 ```
@@ -185,14 +185,14 @@
 
     pip install flake8
     make lint
 
 ## Notes
 
 If you have any questions or issues you can create a new [issue
-here](https://github.com/IBM/sev-snp-measure/issues/new)
+here](https://github.com/virtee/sev-snp-measure/issues/new)
 
 Pull requests are welcome!
 
 ## License
 
 Apache 2.0 license.
```

### Comparing `sev-snp-measure-0.0.6/sev_snp_measure.egg-info/SOURCES.txt` & `sev-snp-measure-0.0.7/sev_snp_measure.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `sev-snp-measure-0.0.6/sevsnpmeasure/cli.py` & `sev-snp-measure-0.0.7/sevsnpmeasure/cli.py`

 * *Files 0% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 import sys
 
 from sevsnpmeasure import guest
 from sevsnpmeasure import vcpu_types
 from sevsnpmeasure import vmm_types
 from .sev_mode import SevMode
 
-VERSION = '0.0.6'
+VERSION = '0.0.7'
 
 
 def auto_base_int(s: str) -> int:
     return int(s, 0)
 
 
 def print_measurement(ld: bytes, sev_mode: SevMode, output_format: str, verbose: bool):
```

### Comparing `sev-snp-measure-0.0.6/sevsnpmeasure/gctx.py` & `sev-snp-measure-0.0.7/sevsnpmeasure/gctx.py`

 * *Files identical despite different names*

### Comparing `sev-snp-measure-0.0.6/sevsnpmeasure/guest.py` & `sev-snp-measure-0.0.7/sevsnpmeasure/guest.py`

 * *Files identical despite different names*

### Comparing `sev-snp-measure-0.0.6/sevsnpmeasure/id_block.py` & `sev-snp-measure-0.0.7/sevsnpmeasure/id_block.py`

 * *Files identical despite different names*

### Comparing `sev-snp-measure-0.0.6/sevsnpmeasure/ovmf.py` & `sev-snp-measure-0.0.7/sevsnpmeasure/ovmf.py`

 * *Files identical despite different names*

### Comparing `sev-snp-measure-0.0.6/sevsnpmeasure/sev_hashes.py` & `sev-snp-measure-0.0.7/sevsnpmeasure/sev_hashes.py`

 * *Files identical despite different names*

### Comparing `sev-snp-measure-0.0.6/sevsnpmeasure/sev_mode.py` & `sev-snp-measure-0.0.7/sevsnpmeasure/sev_mode.py`

 * *Files identical despite different names*

### Comparing `sev-snp-measure-0.0.6/sevsnpmeasure/vcpu_types.py` & `sev-snp-measure-0.0.7/sevsnpmeasure/vcpu_types.py`

 * *Files identical despite different names*

### Comparing `sev-snp-measure-0.0.6/sevsnpmeasure/vmsa.py` & `sev-snp-measure-0.0.7/sevsnpmeasure/vmsa.py`

 * *Files identical despite different names*

### Comparing `sev-snp-measure-0.0.6/tests/test_guest.py` & `sev-snp-measure-0.0.7/tests/test_guest.py`

 * *Files identical despite different names*

### Comparing `sev-snp-measure-0.0.6/tests/test_id_block.py` & `sev-snp-measure-0.0.7/tests/test_id_block.py`

 * *Files identical despite different names*

