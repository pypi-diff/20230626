# Comparing `tmp/nano-autograds-0.0.1.tar.gz` & `tmp/nano-autograds-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nano-autograds-0.0.1.tar", last modified: Sun Jun 25 22:48:56 2023, max compression
+gzip compressed data, was "nano-autograds-0.1.1.tar", last modified: Sun Jun 25 22:46:48 2023, max compression
```

## Comparing `nano-autograds-0.0.1.tar` & `nano-autograds-0.1.1.tar`

### file list

```diff
@@ -1,34 +1,34 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-25 22:48:56.189541 nano-autograds-0.0.1/
--rw-r--r--   0 runner    (1001) docker     (123)     4885 2023-06-25 22:48:56.189541 nano-autograds-0.0.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     4320 2023-06-25 22:48:42.000000 nano-autograds-0.0.1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-25 22:48:56.185541 nano-autograds-0.0.1/autograd/
--rw-r--r--   0 runner    (1001) docker     (123)      316 2023-06-25 22:48:42.000000 nano-autograds-0.0.1/autograd/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-25 22:48:56.185541 nano-autograds-0.0.1/autograd/core/
--rw-r--r--   0 runner    (1001) docker     (123)     1491 2023-06-25 22:48:42.000000 nano-autograds-0.0.1/autograd/core/Graph.py
--rw-r--r--   0 runner    (1001) docker     (123)     4957 2023-06-25 22:48:42.000000 nano-autograds-0.0.1/autograd/core/Spares_nn.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-25 22:48:42.000000 nano-autograds-0.0.1/autograd/core/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5855 2023-06-25 22:48:42.000000 nano-autograds-0.0.1/autograd/core/engine.py
--rw-r--r--   0 runner    (1001) docker     (123)     3474 2023-06-25 22:48:42.000000 nano-autograds-0.0.1/autograd/core/nn.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-25 22:48:56.185541 nano-autograds-0.0.1/autograd/torch/
--rw-r--r--   0 runner    (1001) docker     (123)      119 2023-06-25 22:48:42.000000 nano-autograds-0.0.1/autograd/torch/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      241 2023-06-25 22:48:42.000000 nano-autograds-0.0.1/autograd/torch/init.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-25 22:48:56.185541 nano-autograds-0.0.1/autograd/torch/nn/
--rw-r--r--   0 runner    (1001) docker     (123)       59 2023-06-25 22:48:42.000000 nano-autograds-0.0.1/autograd/torch/nn/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3047 2023-06-25 22:48:42.000000 nano-autograds-0.0.1/autograd/torch/nn/functional.py
--rw-r--r--   0 runner    (1001) docker     (123)     3918 2023-06-25 22:48:42.000000 nano-autograds-0.0.1/autograd/torch/nn/module.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-25 22:48:56.185541 nano-autograds-0.0.1/autograd/torch/optim/
--rw-r--r--   0 runner    (1001) docker     (123)       64 2023-06-25 22:48:42.000000 nano-autograds-0.0.1/autograd/torch/optim/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1886 2023-06-25 22:48:42.000000 nano-autograds-0.0.1/autograd/torch/optim/lr_scheduler.py
--rw-r--r--   0 runner    (1001) docker     (123)     1373 2023-06-25 22:48:42.000000 nano-autograds-0.0.1/autograd/torch/optim/optimizer.py
--rw-r--r--   0 runner    (1001) docker     (123)    19876 2023-06-25 22:48:42.000000 nano-autograds-0.0.1/autograd/torch/tensor.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-25 22:48:56.185541 nano-autograds-0.0.1/nano_autograds.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     4885 2023-06-25 22:48:56.000000 nano-autograds-0.0.1/nano_autograds.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      634 2023-06-25 22:48:56.000000 nano-autograds-0.0.1/nano_autograds.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-25 22:48:56.000000 nano-autograds-0.0.1/nano_autograds.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       14 2023-06-25 22:48:56.000000 nano-autograds-0.0.1/nano_autograds.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-25 22:48:56.189541 nano-autograds-0.0.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      932 2023-06-25 22:48:42.000000 nano-autograds-0.0.1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-25 22:48:56.185541 nano-autograds-0.0.1/test/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-25 22:48:42.000000 nano-autograds-0.0.1/test/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2787 2023-06-25 22:48:42.000000 nano-autograds-0.0.1/test/autograd.py
--rw-r--r--   0 runner    (1001) docker     (123)     2602 2023-06-25 22:48:42.000000 nano-autograds-0.0.1/test/test_engine.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-25 22:46:48.198803 nano-autograds-0.1.1/
+-rw-r--r--   0 runner    (1001) docker     (123)     4875 2023-06-25 22:46:48.198803 nano-autograds-0.1.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     4320 2023-06-25 22:46:28.000000 nano-autograds-0.1.1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-25 22:46:48.194803 nano-autograds-0.1.1/autograd/
+-rw-r--r--   0 runner    (1001) docker     (123)      316 2023-06-25 22:46:28.000000 nano-autograds-0.1.1/autograd/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-25 22:46:48.194803 nano-autograds-0.1.1/autograd/core/
+-rw-r--r--   0 runner    (1001) docker     (123)     1491 2023-06-25 22:46:28.000000 nano-autograds-0.1.1/autograd/core/Graph.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4957 2023-06-25 22:46:28.000000 nano-autograds-0.1.1/autograd/core/Spares_nn.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-25 22:46:28.000000 nano-autograds-0.1.1/autograd/core/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5855 2023-06-25 22:46:28.000000 nano-autograds-0.1.1/autograd/core/engine.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3474 2023-06-25 22:46:28.000000 nano-autograds-0.1.1/autograd/core/nn.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-25 22:46:48.194803 nano-autograds-0.1.1/autograd/torch/
+-rw-r--r--   0 runner    (1001) docker     (123)      119 2023-06-25 22:46:28.000000 nano-autograds-0.1.1/autograd/torch/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      241 2023-06-25 22:46:28.000000 nano-autograds-0.1.1/autograd/torch/init.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-25 22:46:48.194803 nano-autograds-0.1.1/autograd/torch/nn/
+-rw-r--r--   0 runner    (1001) docker     (123)       59 2023-06-25 22:46:28.000000 nano-autograds-0.1.1/autograd/torch/nn/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3047 2023-06-25 22:46:28.000000 nano-autograds-0.1.1/autograd/torch/nn/functional.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3918 2023-06-25 22:46:28.000000 nano-autograds-0.1.1/autograd/torch/nn/module.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-25 22:46:48.194803 nano-autograds-0.1.1/autograd/torch/optim/
+-rw-r--r--   0 runner    (1001) docker     (123)       64 2023-06-25 22:46:28.000000 nano-autograds-0.1.1/autograd/torch/optim/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1886 2023-06-25 22:46:28.000000 nano-autograds-0.1.1/autograd/torch/optim/lr_scheduler.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1373 2023-06-25 22:46:28.000000 nano-autograds-0.1.1/autograd/torch/optim/optimizer.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19876 2023-06-25 22:46:28.000000 nano-autograds-0.1.1/autograd/torch/tensor.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-25 22:46:48.194803 nano-autograds-0.1.1/nano_autograds.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     4875 2023-06-25 22:46:48.000000 nano-autograds-0.1.1/nano_autograds.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      634 2023-06-25 22:46:48.000000 nano-autograds-0.1.1/nano_autograds.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-25 22:46:48.000000 nano-autograds-0.1.1/nano_autograds.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       14 2023-06-25 22:46:48.000000 nano-autograds-0.1.1/nano_autograds.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-25 22:46:48.198803 nano-autograds-0.1.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      922 2023-06-25 22:46:28.000000 nano-autograds-0.1.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-25 22:46:48.198803 nano-autograds-0.1.1/test/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-25 22:46:28.000000 nano-autograds-0.1.1/test/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2787 2023-06-25 22:46:28.000000 nano-autograds-0.1.1/test/autograd.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2602 2023-06-25 22:46:28.000000 nano-autograds-0.1.1/test/test_engine.py
```

### Comparing `nano-autograds-0.0.1/PKG-INFO` & `nano-autograds-0.1.1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 Metadata-Version: 2.1
 Name: nano-autograds
-Version: 0.0.1
+Version: 0.1.1
 Summary: A tinyTroch scalar-Engine Nano-autograd a Micro-Framework with a small PyTorch-like neural network library on top.
-Home-page: https://github.com/deep-matter/Nano-AutoGrad/tree/main/autograd
+Home-page: https://github.com/deep-matter/Nano-AutoGrad/autograd
 Author: Youness EL BRAG
 Author-email: younsselbrag@gmail.com
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `nano-autograds-0.0.1/README.md` & `nano-autograds-0.1.1/README.md`

 * *Files identical despite different names*

### Comparing `nano-autograds-0.0.1/autograd/core/Graph.py` & `nano-autograds-0.1.1/autograd/core/Graph.py`

 * *Files identical despite different names*

### Comparing `nano-autograds-0.0.1/autograd/core/Spares_nn.py` & `nano-autograds-0.1.1/autograd/core/Spares_nn.py`

 * *Files identical despite different names*

### Comparing `nano-autograds-0.0.1/autograd/core/engine.py` & `nano-autograds-0.1.1/autograd/core/engine.py`

 * *Files identical despite different names*

### Comparing `nano-autograds-0.0.1/autograd/core/nn.py` & `nano-autograds-0.1.1/autograd/core/nn.py`

 * *Files identical despite different names*

### Comparing `nano-autograds-0.0.1/autograd/torch/nn/functional.py` & `nano-autograds-0.1.1/autograd/torch/nn/functional.py`

 * *Files identical despite different names*

### Comparing `nano-autograds-0.0.1/autograd/torch/nn/module.py` & `nano-autograds-0.1.1/autograd/torch/nn/module.py`

 * *Files identical despite different names*

### Comparing `nano-autograds-0.0.1/autograd/torch/optim/lr_scheduler.py` & `nano-autograds-0.1.1/autograd/torch/optim/lr_scheduler.py`

 * *Files identical despite different names*

### Comparing `nano-autograds-0.0.1/autograd/torch/optim/optimizer.py` & `nano-autograds-0.1.1/autograd/torch/optim/optimizer.py`

 * *Files identical despite different names*

### Comparing `nano-autograds-0.0.1/autograd/torch/tensor.py` & `nano-autograds-0.1.1/autograd/torch/tensor.py`

 * *Files identical despite different names*

### Comparing `nano-autograds-0.0.1/nano_autograds.egg-info/PKG-INFO` & `nano-autograds-0.1.1/nano_autograds.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 Metadata-Version: 2.1
 Name: nano-autograds
-Version: 0.0.1
+Version: 0.1.1
 Summary: A tinyTroch scalar-Engine Nano-autograd a Micro-Framework with a small PyTorch-like neural network library on top.
-Home-page: https://github.com/deep-matter/Nano-AutoGrad/tree/main/autograd
+Home-page: https://github.com/deep-matter/Nano-AutoGrad/autograd
 Author: Youness EL BRAG
 Author-email: younsselbrag@gmail.com
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `nano-autograds-0.0.1/nano_autograds.egg-info/SOURCES.txt` & `nano-autograds-0.1.1/nano_autograds.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `nano-autograds-0.0.1/setup.py` & `nano-autograds-0.1.1/setup.py`

 * *Files 12% similar despite different names*

```diff
@@ -7,21 +7,21 @@
 sys.path.insert(0, target_dir)
 
 with open(target_dir +"/README.md", "r") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="nano-autograds",
-    version="0.0.1",
+    version="0.1.1",
     author="Youness EL BRAG",
     author_email="younsselbrag@gmail.com",
     description="A tinyTroch scalar-Engine Nano-autograd a Micro-Framework with a small PyTorch-like neural network library on top.",
     long_description=long_description,
     long_description_content_type="text/markdown",
-    url="https://github.com/deep-matter/Nano-AutoGrad/tree/main/autograd",
+    url="https://github.com/deep-matter/Nano-AutoGrad/autograd",
     packages=setuptools.find_packages(),
     classifiers=[
         "Programming Language :: Python :: 3",
         "License :: OSI Approved :: MIT License",
         "Operating System :: OS Independent",
     ],
     python_requires='>=3.7',
```

### Comparing `nano-autograds-0.0.1/test/autograd.py` & `nano-autograds-0.1.1/test/autograd.py`

 * *Files identical despite different names*

### Comparing `nano-autograds-0.0.1/test/test_engine.py` & `nano-autograds-0.1.1/test/test_engine.py`

 * *Files identical despite different names*

