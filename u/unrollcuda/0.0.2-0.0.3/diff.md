# Comparing `tmp/unrollcuda-0.0.2.tar.gz` & `tmp/unrollcuda-0.0.3.tar.gz`

## Comparing `unrollcuda-0.0.2.tar` & `unrollcuda-0.0.3.tar`

### file list

```diff
@@ -1,15 +1,17 @@
--rw-r--r--   0        0        0      225 2020-02-02 00:00:00.000000 unrollcuda-0.0.2/df
--rw-r--r--   0        0        0       46 2020-02-02 00:00:00.000000 unrollcuda-0.0.2/requirements.txt
--rw-r--r--   0        0        0      722 2020-02-02 00:00:00.000000 unrollcuda-0.0.2/docker/Dockerfile
--rw-r--r--   0        0        0       39 2020-02-02 00:00:00.000000 unrollcuda-0.0.2/docker/build.sh
--rw-r--r--   0        0        0       50 2020-02-02 00:00:00.000000 unrollcuda-0.0.2/docker/requirements.txt
--rw-r--r--   0        0        0      191 2020-02-02 00:00:00.000000 unrollcuda-0.0.2/docker/run.sh
--rw-r--r--   0        0        0      201 2020-02-02 00:00:00.000000 unrollcuda-0.0.2/docker/stop.sh
--rw-r--r--   0        0        0     1655 2020-02-02 00:00:00.000000 unrollcuda-0.0.2/examples/cross.cu
--rw-r--r--   0        0        0      991 2020-02-02 00:00:00.000000 unrollcuda-0.0.2/examples/cross.py
--rw-r--r--   0        0        0       34 2020-02-02 00:00:00.000000 unrollcuda-0.0.2/src/unrollcuda/__init__.py
--rw-r--r--   0        0        0     3220 2020-02-02 00:00:00.000000 unrollcuda-0.0.2/src/unrollcuda/unrollcuda.py
--rw-r--r--   0        0        0      590 2020-02-02 00:00:00.000000 unrollcuda-0.0.2/LICENSE
--rw-r--r--   0        0        0      314 2020-02-02 00:00:00.000000 unrollcuda-0.0.2/README.md
--rw-r--r--   0        0        0      622 2020-02-02 00:00:00.000000 unrollcuda-0.0.2/pyproject.toml
--rw-r--r--   0        0        0      864 2020-02-02 00:00:00.000000 unrollcuda-0.0.2/PKG-INFO
+-rw-r--r--   0        0        0       17 2020-02-02 00:00:00.000000 unrollcuda-0.0.3/build.sh
+-rw-r--r--   0        0        0      225 2020-02-02 00:00:00.000000 unrollcuda-0.0.3/df
+-rw-r--r--   0        0        0       46 2020-02-02 00:00:00.000000 unrollcuda-0.0.3/requirements.txt
+-rw-r--r--   0        0        0       75 2020-02-02 00:00:00.000000 unrollcuda-0.0.3/upload.sh
+-rw-r--r--   0        0        0      804 2020-02-02 00:00:00.000000 unrollcuda-0.0.3/docker/Dockerfile
+-rw-r--r--   0        0        0       39 2020-02-02 00:00:00.000000 unrollcuda-0.0.3/docker/build.sh
+-rw-r--r--   0        0        0       50 2020-02-02 00:00:00.000000 unrollcuda-0.0.3/docker/requirements.txt
+-rw-r--r--   0        0        0      191 2020-02-02 00:00:00.000000 unrollcuda-0.0.3/docker/run.sh
+-rw-r--r--   0        0        0      201 2020-02-02 00:00:00.000000 unrollcuda-0.0.3/docker/stop.sh
+-rw-r--r--   0        0        0     1655 2020-02-02 00:00:00.000000 unrollcuda-0.0.3/examples/cross.cu
+-rw-r--r--   0        0        0      991 2020-02-02 00:00:00.000000 unrollcuda-0.0.3/examples/cross.py
+-rw-r--r--   0        0        0       34 2020-02-02 00:00:00.000000 unrollcuda-0.0.3/src/unrollcuda/__init__.py
+-rw-r--r--   0        0        0     3220 2020-02-02 00:00:00.000000 unrollcuda-0.0.3/src/unrollcuda/unrollcuda.py
+-rw-r--r--   0        0        0      590 2020-02-02 00:00:00.000000 unrollcuda-0.0.3/LICENSE
+-rw-r--r--   0        0        0      314 2020-02-02 00:00:00.000000 unrollcuda-0.0.3/README.md
+-rw-r--r--   0        0        0      640 2020-02-02 00:00:00.000000 unrollcuda-0.0.3/pyproject.toml
+-rw-r--r--   0        0        0      886 2020-02-02 00:00:00.000000 unrollcuda-0.0.3/PKG-INFO
```

### Comparing `unrollcuda-0.0.2/docker/Dockerfile` & `unrollcuda-0.0.3/docker/Dockerfile`

 * *Files 14% similar despite different names*

```diff
@@ -10,11 +10,12 @@
 # Set up symlinks for gcc and g++
 RUN rm /usr/bin/gcc && rm /usr/bin/g++ \
     && ln -s /usr/bin/gcc-9 /usr/bin/gcc \
     && ln -s /usr/bin/g++-9 /usr/bin/g++
 
 COPY requirements.txt /app/scripts/requirements.txt
 RUN python3 -m pip install -r requirements.txt --no-cache-dir
-RUN python3 -m pip install --index-url https://test.pypi.org/simple/ --no-deps unrollcuda
+# RUN python3 -m pip install --index-url https://test.pypi.org/simple/ --no-deps unrollcuda
+RUN python3 -m pip install --index-url https://test.pypi.org/simple/ unrollcuda
 # CMD ["python3", "sample.py"]
 # CMD ["nvprof -f -o ../prof.nvvp python3 test.py"]
 # CMD ["cuda-gdb --args python3 -m pycuda.debug test.py"]
```

### Comparing `unrollcuda-0.0.2/examples/cross.cu` & `unrollcuda-0.0.3/examples/cross.cu`

 * *Files identical despite different names*

### Comparing `unrollcuda-0.0.2/examples/cross.py` & `unrollcuda-0.0.3/examples/cross.py`

 * *Files identical despite different names*

### Comparing `unrollcuda-0.0.2/src/unrollcuda/unrollcuda.py` & `unrollcuda-0.0.3/src/unrollcuda/unrollcuda.py`

 * *Files identical despite different names*

### Comparing `unrollcuda-0.0.2/LICENSE` & `unrollcuda-0.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `unrollcuda-0.0.2/PKG-INFO` & `unrollcuda-0.0.3/PKG-INFO`

 * *Files 24% similar despite different names*

```diff
@@ -1,20 +1,21 @@
 Metadata-Version: 2.1
 Name: unrollcuda
-Version: 0.0.2
+Version: 0.0.3
 Summary: Loop unrolling and batching for CUDA
 Project-URL: Homepage, https://github.com/format37/unrollcuda
 Project-URL: Bug Tracker, https://github.com/format37/unrollcuda/issues
 Author-email: Aleksei Iurasov <format37@gmail.com>
 License-File: LICENSE
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
-Requires-Python: >=3.7
+Requires-Python: >=3.8
 Requires-Dist: numpy
+Requires-Dist: pycuda
 Description-Content-Type: text/markdown
 
 # unrollcuda
 Loop unrolling and batching for CUDA  
 The core idea of this solution is to give a way to solve the following tasks:  
 1. Use Loop unrolling to compute in CUDA any size and any count of dimensions array  
 2. Use Batching to compute any size array, even if it s big that can't be fitted in GPU memory
```

