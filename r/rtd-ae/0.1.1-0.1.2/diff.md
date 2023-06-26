# Comparing `tmp/rtd_ae-0.1.1.tar.gz` & `tmp/rtd_ae-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "rtd_ae-0.1.1.tar", max compression
+gzip compressed data, was "rtd_ae-0.1.2.tar", max compression
```

## Comparing `rtd_ae-0.1.1.tar` & `rtd_ae-0.1.2.tar`

### file list

```diff
@@ -1,11 +1,11 @@
--rw-r--r--   0        0        0      798 2023-06-26 08:03:14.256951 rtd_ae-0.1.1/pyproject.toml
--rw-r--r--   0        0        0     1989 2023-06-23 08:13:48.129881 rtd_ae-0.1.1/README.md
--rw-r--r--   0        0        0        0 2023-06-23 08:13:48.135878 rtd_ae-0.1.1/rtd_ae/__init__.py
--rw-r--r--   0        0        0     7360 2023-06-23 11:23:06.543266 rtd_ae-0.1.1/rtd_ae/autoencoder.py
--rw-r--r--   0        0        0     4741 2023-06-23 11:23:06.506276 rtd_ae-0.1.1/rtd_ae/custom_shapes.py
--rw-r--r--   0        0        0     7697 2023-06-23 11:23:06.553264 rtd_ae-0.1.1/rtd_ae/rtd.py
--rw-r--r--   0        0        0     1724 2023-06-23 11:23:06.517268 rtd_ae-0.1.1/rtd_ae/spheres.py
--rw-r--r--   0        0        0    10198 2023-06-23 11:23:06.497278 rtd_ae-0.1.1/rtd_ae/top_ae.py
--rw-r--r--   0        0        0     4817 2023-06-23 11:23:06.532270 rtd_ae-0.1.1/rtd_ae/topology.py
--rw-r--r--   0        0        0    13896 2023-06-26 06:58:44.873538 rtd_ae-0.1.1/rtd_ae/utils.py
--rw-r--r--   0        0        0     2958 1970-01-01 00:00:00.000000 rtd_ae-0.1.1/PKG-INFO
+-rw-r--r--   0        0        0      762 2023-06-26 11:11:27.877596 rtd_ae-0.1.2/pyproject.toml
+-rw-r--r--   0        0        0     1989 2023-06-23 08:13:48.129881 rtd_ae-0.1.2/README.md
+-rw-r--r--   0        0        0        0 2023-06-23 08:13:48.135878 rtd_ae-0.1.2/rtd_ae/__init__.py
+-rw-r--r--   0        0        0     7360 2023-06-23 11:23:06.543266 rtd_ae-0.1.2/rtd_ae/autoencoder.py
+-rw-r--r--   0        0        0     4741 2023-06-23 11:23:06.506276 rtd_ae-0.1.2/rtd_ae/custom_shapes.py
+-rw-r--r--   0        0        0     7697 2023-06-23 11:23:06.553264 rtd_ae-0.1.2/rtd_ae/rtd.py
+-rw-r--r--   0        0        0     1724 2023-06-23 11:23:06.517268 rtd_ae-0.1.2/rtd_ae/spheres.py
+-rw-r--r--   0        0        0    10198 2023-06-23 11:23:06.497278 rtd_ae-0.1.2/rtd_ae/top_ae.py
+-rw-r--r--   0        0        0     4817 2023-06-23 11:23:06.532270 rtd_ae-0.1.2/rtd_ae/topology.py
+-rw-r--r--   0        0        0    13896 2023-06-26 06:58:44.873538 rtd_ae-0.1.2/rtd_ae/utils.py
+-rw-r--r--   0        0        0     2938 1970-01-01 00:00:00.000000 rtd_ae-0.1.2/PKG-INFO
```

### Comparing `rtd_ae-0.1.1/pyproject.toml` & `rtd_ae-0.1.2/pyproject.toml`

 * *Files 12% similar despite different names*

```diff
@@ -1,32 +1,32 @@
 [tool.poetry]
 name = "rtd-ae"
-version = "0.1.1"
+version = "0.1.2"
 description = ""
 authors = ["Daniil Cherniavskii <danchern97@mail.ru>", "AndreyBychkov <abychkov_edu@proton.me>"]
 readme = "README.md"
 packages = [{include = "rtd_ae"}]
 
 [tool.poetry.dependencies]
-python = ">=3.10,<3.13"
-tqdm = "^4.65.0"
-torch = "^2.0.1"
-scikit-learn = "^1.2.2"
+python = ">=3.9,<3.13"
+tqdm = "^4.60.0"
+torch = "^2"
+scikit-learn = "^1.1"
 POT = "^0.9.0"
-matplotlib = "^3.7.1"
-gudhi = "^3.8.0"
-pytorch-lightning = "^2.0.4"
-pandas = "^2.0.2"
-numpy = "^1.25.0"
-notebook = "^6.5.4"
-scipy = "^1.10.1"
-Pillow = "^9.5.0"
-giotto-ph = "^0.2.2"
+matplotlib = "^3.6"
+gudhi = "^3.6"
+pytorch-lightning = "^2"
+pandas = "^2"
+numpy = "^1.19.0"
+notebook = "^6"
+scipy = "^1.9"
+Pillow = "^9.0.0"
+giotto-ph = "^0.2"
 #ripserplusplus = {git = "https://github.com/ArGintum/RipserZeros.git", platform = "linux"}
-ipywidgets = "^8.0.6"
+ipywidgets = "^8"
 iprogress = "^0.4"
-tensorboardx = "^2.6.1"
+tensorboardx = "^2"
 
 
 [build-system]
 requires = ["poetry-core"]
 build-backend = "poetry.core.masonry.api"
```

### Comparing `rtd_ae-0.1.1/README.md` & `rtd_ae-0.1.2/README.md`

 * *Files identical despite different names*

### Comparing `rtd_ae-0.1.1/rtd_ae/autoencoder.py` & `rtd_ae-0.1.2/rtd_ae/autoencoder.py`

 * *Files identical despite different names*

### Comparing `rtd_ae-0.1.1/rtd_ae/custom_shapes.py` & `rtd_ae-0.1.2/rtd_ae/custom_shapes.py`

 * *Files identical despite different names*

### Comparing `rtd_ae-0.1.1/rtd_ae/rtd.py` & `rtd_ae-0.1.2/rtd_ae/rtd.py`

 * *Files identical despite different names*

### Comparing `rtd_ae-0.1.1/rtd_ae/spheres.py` & `rtd_ae-0.1.2/rtd_ae/spheres.py`

 * *Files identical despite different names*

### Comparing `rtd_ae-0.1.1/rtd_ae/top_ae.py` & `rtd_ae-0.1.2/rtd_ae/top_ae.py`

 * *Files identical despite different names*

### Comparing `rtd_ae-0.1.1/rtd_ae/topology.py` & `rtd_ae-0.1.2/rtd_ae/topology.py`

 * *Files identical despite different names*

### Comparing `rtd_ae-0.1.1/rtd_ae/utils.py` & `rtd_ae-0.1.2/rtd_ae/utils.py`

 * *Files identical despite different names*

### Comparing `rtd_ae-0.1.1/PKG-INFO` & `rtd_ae-0.1.2/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,33 +1,34 @@
 Metadata-Version: 2.1
 Name: rtd-ae
-Version: 0.1.1
+Version: 0.1.2
 Summary: 
 Author: Daniil Cherniavskii
 Author-email: danchern97@mail.ru
-Requires-Python: >=3.10,<3.13
+Requires-Python: >=3.9,<3.13
 Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Requires-Dist: POT (>=0.9.0,<0.10.0)
-Requires-Dist: Pillow (>=9.5.0,<10.0.0)
-Requires-Dist: giotto-ph (>=0.2.2,<0.3.0)
-Requires-Dist: gudhi (>=3.8.0,<4.0.0)
+Requires-Dist: Pillow (>=9.0.0,<10.0.0)
+Requires-Dist: giotto-ph (>=0.2,<0.3)
+Requires-Dist: gudhi (>=3.6,<4.0)
 Requires-Dist: iprogress (>=0.4,<0.5)
-Requires-Dist: ipywidgets (>=8.0.6,<9.0.0)
-Requires-Dist: matplotlib (>=3.7.1,<4.0.0)
-Requires-Dist: notebook (>=6.5.4,<7.0.0)
-Requires-Dist: numpy (>=1.25.0,<2.0.0)
-Requires-Dist: pandas (>=2.0.2,<3.0.0)
-Requires-Dist: pytorch-lightning (>=2.0.4,<3.0.0)
-Requires-Dist: scikit-learn (>=1.2.2,<2.0.0)
-Requires-Dist: scipy (>=1.10.1,<2.0.0)
-Requires-Dist: tensorboardx (>=2.6.1,<3.0.0)
-Requires-Dist: torch (>=2.0.1,<3.0.0)
-Requires-Dist: tqdm (>=4.65.0,<5.0.0)
+Requires-Dist: ipywidgets (>=8,<9)
+Requires-Dist: matplotlib (>=3.6,<4.0)
+Requires-Dist: notebook (>=6,<7)
+Requires-Dist: numpy (>=1.19.0,<2.0.0)
+Requires-Dist: pandas (>=2,<3)
+Requires-Dist: pytorch-lightning (>=2,<3)
+Requires-Dist: scikit-learn (>=1.1,<2.0)
+Requires-Dist: scipy (>=1.9,<2.0)
+Requires-Dist: tensorboardx (>=2,<3)
+Requires-Dist: torch (>=2,<3)
+Requires-Dist: tqdm (>=4.60.0,<5.0.0)
 Description-Content-Type: text/markdown
 
 # Learning topology-preserving data representations (ICLR 2023)
 
 This repository contains code base for the paper which introduces a novel method for global structure preserving dimensionality rediction based on Topological Data Analysis (TDA), specifically Representation Topology Divergence (RTD).
 
 ## Description
```

