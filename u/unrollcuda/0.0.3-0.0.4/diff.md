# Comparing `tmp/unrollcuda-0.0.3.tar.gz` & `tmp/unrollcuda-0.0.4.tar.gz`

## Comparing `unrollcuda-0.0.3.tar` & `unrollcuda-0.0.4.tar`

### file list

```diff
@@ -1,17 +1,21 @@
--rw-r--r--   0        0        0       17 2020-02-02 00:00:00.000000 unrollcuda-0.0.3/build.sh
--rw-r--r--   0        0        0      225 2020-02-02 00:00:00.000000 unrollcuda-0.0.3/df
--rw-r--r--   0        0        0       46 2020-02-02 00:00:00.000000 unrollcuda-0.0.3/requirements.txt
--rw-r--r--   0        0        0       75 2020-02-02 00:00:00.000000 unrollcuda-0.0.3/upload.sh
--rw-r--r--   0        0        0      804 2020-02-02 00:00:00.000000 unrollcuda-0.0.3/docker/Dockerfile
--rw-r--r--   0        0        0       39 2020-02-02 00:00:00.000000 unrollcuda-0.0.3/docker/build.sh
--rw-r--r--   0        0        0       50 2020-02-02 00:00:00.000000 unrollcuda-0.0.3/docker/requirements.txt
--rw-r--r--   0        0        0      191 2020-02-02 00:00:00.000000 unrollcuda-0.0.3/docker/run.sh
--rw-r--r--   0        0        0      201 2020-02-02 00:00:00.000000 unrollcuda-0.0.3/docker/stop.sh
--rw-r--r--   0        0        0     1655 2020-02-02 00:00:00.000000 unrollcuda-0.0.3/examples/cross.cu
--rw-r--r--   0        0        0      991 2020-02-02 00:00:00.000000 unrollcuda-0.0.3/examples/cross.py
--rw-r--r--   0        0        0       34 2020-02-02 00:00:00.000000 unrollcuda-0.0.3/src/unrollcuda/__init__.py
--rw-r--r--   0        0        0     3220 2020-02-02 00:00:00.000000 unrollcuda-0.0.3/src/unrollcuda/unrollcuda.py
--rw-r--r--   0        0        0      590 2020-02-02 00:00:00.000000 unrollcuda-0.0.3/LICENSE
--rw-r--r--   0        0        0      314 2020-02-02 00:00:00.000000 unrollcuda-0.0.3/README.md
--rw-r--r--   0        0        0      640 2020-02-02 00:00:00.000000 unrollcuda-0.0.3/pyproject.toml
--rw-r--r--   0        0        0      886 2020-02-02 00:00:00.000000 unrollcuda-0.0.3/PKG-INFO
+-rw-r--r--   0        0        0       17 2020-02-02 00:00:00.000000 unrollcuda-0.0.4/build.sh
+-rw-r--r--   0        0        0      225 2020-02-02 00:00:00.000000 unrollcuda-0.0.4/df
+-rw-r--r--   0        0        0       46 2020-02-02 00:00:00.000000 unrollcuda-0.0.4/requirements.txt
+-rw-r--r--   0        0        0       75 2020-02-02 00:00:00.000000 unrollcuda-0.0.4/upload.sh
+-rw-r--r--   0        0        0      454 2020-02-02 00:00:00.000000 unrollcuda-0.0.4/docker/Dockerfile
+-rw-r--r--   0        0        0       40 2020-02-02 00:00:00.000000 unrollcuda-0.0.4/docker/build.sh
+-rw-r--r--   0        0        0       80 2020-02-02 00:00:00.000000 unrollcuda-0.0.4/docker/check_gpu.sh
+-rw-r--r--   0        0        0       28 2020-02-02 00:00:00.000000 unrollcuda-0.0.4/docker/requirements.txt
+-rw-r--r--   0        0        0      129 2020-02-02 00:00:00.000000 unrollcuda-0.0.4/docker/run.sh
+-rw-r--r--   0        0        0      201 2020-02-02 00:00:00.000000 unrollcuda-0.0.4/docker/stop.sh
+-rw-r--r--   0        0        0     1655 2020-02-02 00:00:00.000000 unrollcuda-0.0.4/examples/cross.cu
+-rw-r--r--   0        0        0      991 2020-02-02 00:00:00.000000 unrollcuda-0.0.4/examples/cross.py
+-rw-r--r--   0        0        0     1584 2020-02-02 00:00:00.000000 unrollcuda-0.0.4/examples/invert.cu
+-rw-r--r--   0        0        0      801 2020-02-02 00:00:00.000000 unrollcuda-0.0.4/examples/invert.py
+-rw-r--r--   0        0        0     4256 2020-02-02 00:00:00.000000 unrollcuda-0.0.4/examples/unrollcuda_test.py
+-rw-r--r--   0        0        0     1410 2020-02-02 00:00:00.000000 unrollcuda-0.0.4/src/unrollcuda/__init__.py
+-rw-r--r--   0        0        0     4240 2020-02-02 00:00:00.000000 unrollcuda-0.0.4/src/unrollcuda/unrollcuda.py
+-rw-r--r--   0        0        0      590 2020-02-02 00:00:00.000000 unrollcuda-0.0.4/LICENSE
+-rw-r--r--   0        0        0     2996 2020-02-02 00:00:00.000000 unrollcuda-0.0.4/README.md
+-rw-r--r--   0        0        0      640 2020-02-02 00:00:00.000000 unrollcuda-0.0.4/pyproject.toml
+-rw-r--r--   0        0        0     3568 2020-02-02 00:00:00.000000 unrollcuda-0.0.4/PKG-INFO
```

### Comparing `unrollcuda-0.0.3/examples/cross.cu` & `unrollcuda-0.0.4/examples/cross.cu`

 * *Files identical despite different names*

### Comparing `unrollcuda-0.0.3/examples/cross.py` & `unrollcuda-0.0.4/examples/cross.py`

 * *Files identical despite different names*

### Comparing `unrollcuda-0.0.3/src/unrollcuda/unrollcuda.py` & `unrollcuda-0.0.4/src/unrollcuda/unrollcuda.py`

 * *Files 17% similar despite different names*

```diff
@@ -5,32 +5,38 @@
 ####################################################################################################
 
 import pycuda.driver as drv
 from pycuda import gpuarray
 from pycuda.compiler import SourceModule
 import numpy as np
 import logging
+import pkg_resources
 
+try:
+    __version__ = pkg_resources.get_distribution("unrollcuda").version
+except pkg_resources.DistributionNotFound:
+    # Package is not installed
+    pass
 
 logging.basicConfig(level=logging.INFO)
 
 
-class unrollcuda:
+class kernel:
     def __init__(
             self, 
             kernel_code,
             gpu_id=0, 
             reshape_order='C',
             max_block_x=0, 
             max_grid_x=0,
             batch_size=0,
             verbose=False
             ):
         self.verbose = verbose
-        if self.verbose:            
+        if self.verbose:
             self.logger = logging.getLogger(__name__)
 
         self.gpu_id = gpu_id        
         drv.init()
         self.dev = drv.Device(self.gpu_id)
         self.ctx = self.dev.make_context()
         self.kernel_code = kernel_code
@@ -46,16 +52,28 @@
                 )
 
     def log(self, msg):
         if self.verbose:
             self.logger.info(' '+msg)
         
     def inference(self, arr):
+        """
+        Perform computations on a provided array using the CUDA kernel specified in the `unrollcuda` instance.
+        
+        This method uses loop unrolling and batching techniques to efficiently handle array sizes larger than GPU memory. The computations are performed in batches, if needed, and the resulting array is reshaped back to the original shape before it is returned.
+        
+        Arguments:
+            arr (numpy.ndarray, required): The input array on which the computations will be performed. This can be a multi-dimensional array of any size.
+            
+        Returns:
+            numpy.ndarray: The resulting array after performing computations. The shape of this array will be the same as the input array `arr`.
+        """
         shape = arr.shape
-        self.result_array = np.zeros(arr.size, dtype=np.bool_, order=self.reshape_order)
+        # self.result_array = np.zeros(arr.size, dtype=np.bool_, order=self.reshape_order)
+        self.result_array = np.zeros(arr.size, dtype=arr.dtype, order=self.reshape_order)
         if self.batch_size == 0:
             self.batch_size = arr.size
         arr = arr.reshape(-1, order=self.reshape_order)
         total_elements = arr.size
 
         batch_start = 0
         while batch_start < total_elements:
```

### Comparing `unrollcuda-0.0.3/LICENSE` & `unrollcuda-0.0.4/LICENSE`

 * *Files identical despite different names*

### Comparing `unrollcuda-0.0.3/pyproject.toml` & `unrollcuda-0.0.4/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["hatchling","numpy","pycuda"]
 build-backend = "hatchling.build"
 
 [project]
 name = "unrollcuda"
-version = "0.0.3"
+version = "0.0.4"
 authors = [
   { name="Aleksei Iurasov", email="format37@gmail.com" },
 ]
 description = "Loop unrolling and batching for CUDA"
 readme = "README.md"
 requires-python = ">=3.8"
 classifiers = [
```

