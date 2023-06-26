# Comparing `tmp/unrollcuda-0.0.4.tar.gz` & `tmp/unrollcuda-0.0.5.tar.gz`

## Comparing `unrollcuda-0.0.4.tar` & `unrollcuda-0.0.5.tar`

### file list

```diff
@@ -1,21 +1,21 @@
--rw-r--r--   0        0        0       17 2020-02-02 00:00:00.000000 unrollcuda-0.0.4/build.sh
--rw-r--r--   0        0        0      225 2020-02-02 00:00:00.000000 unrollcuda-0.0.4/df
--rw-r--r--   0        0        0       46 2020-02-02 00:00:00.000000 unrollcuda-0.0.4/requirements.txt
--rw-r--r--   0        0        0       75 2020-02-02 00:00:00.000000 unrollcuda-0.0.4/upload.sh
--rw-r--r--   0        0        0      454 2020-02-02 00:00:00.000000 unrollcuda-0.0.4/docker/Dockerfile
--rw-r--r--   0        0        0       40 2020-02-02 00:00:00.000000 unrollcuda-0.0.4/docker/build.sh
--rw-r--r--   0        0        0       80 2020-02-02 00:00:00.000000 unrollcuda-0.0.4/docker/check_gpu.sh
--rw-r--r--   0        0        0       28 2020-02-02 00:00:00.000000 unrollcuda-0.0.4/docker/requirements.txt
--rw-r--r--   0        0        0      129 2020-02-02 00:00:00.000000 unrollcuda-0.0.4/docker/run.sh
--rw-r--r--   0        0        0      201 2020-02-02 00:00:00.000000 unrollcuda-0.0.4/docker/stop.sh
--rw-r--r--   0        0        0     1655 2020-02-02 00:00:00.000000 unrollcuda-0.0.4/examples/cross.cu
--rw-r--r--   0        0        0      991 2020-02-02 00:00:00.000000 unrollcuda-0.0.4/examples/cross.py
--rw-r--r--   0        0        0     1584 2020-02-02 00:00:00.000000 unrollcuda-0.0.4/examples/invert.cu
--rw-r--r--   0        0        0      801 2020-02-02 00:00:00.000000 unrollcuda-0.0.4/examples/invert.py
--rw-r--r--   0        0        0     4256 2020-02-02 00:00:00.000000 unrollcuda-0.0.4/examples/unrollcuda_test.py
--rw-r--r--   0        0        0     1410 2020-02-02 00:00:00.000000 unrollcuda-0.0.4/src/unrollcuda/__init__.py
--rw-r--r--   0        0        0     4240 2020-02-02 00:00:00.000000 unrollcuda-0.0.4/src/unrollcuda/unrollcuda.py
--rw-r--r--   0        0        0      590 2020-02-02 00:00:00.000000 unrollcuda-0.0.4/LICENSE
--rw-r--r--   0        0        0     2996 2020-02-02 00:00:00.000000 unrollcuda-0.0.4/README.md
--rw-r--r--   0        0        0      640 2020-02-02 00:00:00.000000 unrollcuda-0.0.4/pyproject.toml
--rw-r--r--   0        0        0     3568 2020-02-02 00:00:00.000000 unrollcuda-0.0.4/PKG-INFO
+-rw-r--r--   0        0        0       17 2020-02-02 00:00:00.000000 unrollcuda-0.0.5/build.sh
+-rw-r--r--   0        0        0      225 2020-02-02 00:00:00.000000 unrollcuda-0.0.5/df
+-rw-r--r--   0        0        0       46 2020-02-02 00:00:00.000000 unrollcuda-0.0.5/requirements.txt
+-rw-r--r--   0        0        0       92 2020-02-02 00:00:00.000000 unrollcuda-0.0.5/upload.sh
+-rw-r--r--   0        0        0      454 2020-02-02 00:00:00.000000 unrollcuda-0.0.5/docker/Dockerfile
+-rw-r--r--   0        0        0       40 2020-02-02 00:00:00.000000 unrollcuda-0.0.5/docker/build.sh
+-rw-r--r--   0        0        0       80 2020-02-02 00:00:00.000000 unrollcuda-0.0.5/docker/check_gpu.sh
+-rw-r--r--   0        0        0       28 2020-02-02 00:00:00.000000 unrollcuda-0.0.5/docker/requirements.txt
+-rw-r--r--   0        0        0      129 2020-02-02 00:00:00.000000 unrollcuda-0.0.5/docker/run.sh
+-rw-r--r--   0        0        0      201 2020-02-02 00:00:00.000000 unrollcuda-0.0.5/docker/stop.sh
+-rw-r--r--   0        0        0     1655 2020-02-02 00:00:00.000000 unrollcuda-0.0.5/examples/cross.cu
+-rw-r--r--   0        0        0      991 2020-02-02 00:00:00.000000 unrollcuda-0.0.5/examples/cross.py
+-rw-r--r--   0        0        0     1584 2020-02-02 00:00:00.000000 unrollcuda-0.0.5/examples/invert.cu
+-rw-r--r--   0        0        0      801 2020-02-02 00:00:00.000000 unrollcuda-0.0.5/examples/invert.py
+-rw-r--r--   0        0        0     4256 2020-02-02 00:00:00.000000 unrollcuda-0.0.5/examples/unrollcuda_test.py
+-rw-r--r--   0        0        0     1580 2020-02-02 00:00:00.000000 unrollcuda-0.0.5/src/unrollcuda/__init__.py
+-rw-r--r--   0        0        0     4059 2020-02-02 00:00:00.000000 unrollcuda-0.0.5/src/unrollcuda/unrollcuda.py
+-rw-r--r--   0        0        0      590 2020-02-02 00:00:00.000000 unrollcuda-0.0.5/LICENSE
+-rw-r--r--   0        0        0     2996 2020-02-02 00:00:00.000000 unrollcuda-0.0.5/README.md
+-rw-r--r--   0        0        0      640 2020-02-02 00:00:00.000000 unrollcuda-0.0.5/pyproject.toml
+-rw-r--r--   0        0        0     3568 2020-02-02 00:00:00.000000 unrollcuda-0.0.5/PKG-INFO
```

### Comparing `unrollcuda-0.0.4/examples/cross.cu` & `unrollcuda-0.0.5/examples/cross.cu`

 * *Files identical despite different names*

### Comparing `unrollcuda-0.0.4/examples/cross.py` & `unrollcuda-0.0.5/examples/cross.py`

 * *Files identical despite different names*

### Comparing `unrollcuda-0.0.4/examples/invert.cu` & `unrollcuda-0.0.5/examples/invert.cu`

 * *Files identical despite different names*

### Comparing `unrollcuda-0.0.4/examples/invert.py` & `unrollcuda-0.0.5/examples/invert.py`

 * *Files identical despite different names*

### Comparing `unrollcuda-0.0.4/examples/unrollcuda_test.py` & `unrollcuda-0.0.5/examples/unrollcuda_test.py`

 * *Files identical despite different names*

### Comparing `unrollcuda-0.0.4/src/unrollcuda/__init__.py` & `unrollcuda-0.0.5/src/unrollcuda/__init__.py`

 * *Files 18% similar despite different names*

```diff
@@ -13,8 +13,15 @@
     batch_size (int, optional): Size of the batch used when the array can't be fitted into GPU memory at once. If 0, the batch size will be equal to the array size. Defaults to 0.
     verbose (bool, optional): If True, verbose logging is enabled. Defaults to False.
 
 Project Links:
     PyPI: https://pypi.org/project/unrollcuda
     GitHub: https://github.com/format37/unrollcuda
 """
-from .unrollcuda import kernel, inference
+from .unrollcuda import kernel
+import pkg_resources
+
+try:
+    __version__ = pkg_resources.get_distribution("unrollcuda").version
+except pkg_resources.DistributionNotFound:
+    # Package is not installed
+    pass
```

### Comparing `unrollcuda-0.0.4/src/unrollcuda/unrollcuda.py` & `unrollcuda-0.0.5/src/unrollcuda/unrollcuda.py`

 * *Files 8% similar despite different names*

```diff
@@ -5,21 +5,14 @@
 ####################################################################################################
 
 import pycuda.driver as drv
 from pycuda import gpuarray
 from pycuda.compiler import SourceModule
 import numpy as np
 import logging
-import pkg_resources
-
-try:
-    __version__ = pkg_resources.get_distribution("unrollcuda").version
-except pkg_resources.DistributionNotFound:
-    # Package is not installed
-    pass
 
 logging.basicConfig(level=logging.INFO)
 
 
 class kernel:
     def __init__(
             self,
```

### Comparing `unrollcuda-0.0.4/LICENSE` & `unrollcuda-0.0.5/LICENSE`

 * *Files identical despite different names*

### Comparing `unrollcuda-0.0.4/README.md` & `unrollcuda-0.0.5/README.md`

 * *Files identical despite different names*

### Comparing `unrollcuda-0.0.4/pyproject.toml` & `unrollcuda-0.0.5/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["hatchling","numpy","pycuda"]
 build-backend = "hatchling.build"
 
 [project]
 name = "unrollcuda"
-version = "0.0.4"
+version = "0.0.5"
 authors = [
   { name="Aleksei Iurasov", email="format37@gmail.com" },
 ]
 description = "Loop unrolling and batching for CUDA"
 readme = "README.md"
 requires-python = ">=3.8"
 classifiers = [
```

### Comparing `unrollcuda-0.0.4/PKG-INFO` & `unrollcuda-0.0.5/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: unrollcuda
-Version: 0.0.4
+Version: 0.0.5
 Summary: Loop unrolling and batching for CUDA
 Project-URL: Homepage, https://github.com/format37/unrollcuda
 Project-URL: Bug Tracker, https://github.com/format37/unrollcuda/issues
 Author-email: Aleksei Iurasov <format37@gmail.com>
 License-File: LICENSE
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: OS Independent
```

