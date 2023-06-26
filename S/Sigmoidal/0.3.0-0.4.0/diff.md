# Comparing `tmp/Sigmoidal-0.3.0.tar.gz` & `tmp/Sigmoidal-0.4.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "Sigmoidal-0.3.0.tar", last modified: Thu Jun  1 18:46:45 2023, max compression
+gzip compressed data, was "Sigmoidal-0.4.0.tar", last modified: Mon Jun 26 19:54:36 2023, max compression
```

## Comparing `Sigmoidal-0.3.0.tar` & `Sigmoidal-0.4.0.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxr-xr-x   0 jade       (502) staff       (20)        0 2023-06-01 18:46:45.887342 Sigmoidal-0.3.0/
--rw-r--r--   0 jade       (502) staff       (20)     1063 2023-05-22 21:09:43.000000 Sigmoidal-0.3.0/LICENSE
--rw-r--r--   0 jade       (502) staff       (20)        0 2023-05-22 21:14:28.000000 Sigmoidal-0.3.0/MANIFEST.in
--rw-r--r--   0 jade       (502) staff       (20)     1542 2023-06-01 18:46:45.886799 Sigmoidal-0.3.0/PKG-INFO
--rw-r--r--   0 jade       (502) staff       (20)     1057 2023-05-23 02:43:17.000000 Sigmoidal-0.3.0/README.md
-drwxr-xr-x   0 jade       (502) staff       (20)        0 2023-06-01 18:46:45.886232 Sigmoidal-0.3.0/Sigmoidal.egg-info/
--rw-r--r--   0 jade       (502) staff       (20)     1542 2023-06-01 18:46:45.000000 Sigmoidal-0.3.0/Sigmoidal.egg-info/PKG-INFO
--rw-r--r--   0 jade       (502) staff       (20)      388 2023-06-01 18:46:45.000000 Sigmoidal-0.3.0/Sigmoidal.egg-info/SOURCES.txt
--rw-r--r--   0 jade       (502) staff       (20)        1 2023-06-01 18:46:45.000000 Sigmoidal-0.3.0/Sigmoidal.egg-info/dependency_links.txt
--rw-r--r--   0 jade       (502) staff       (20)       28 2023-06-01 18:46:45.000000 Sigmoidal-0.3.0/Sigmoidal.egg-info/requires.txt
--rw-r--r--   0 jade       (502) staff       (20)       10 2023-06-01 18:46:45.000000 Sigmoidal-0.3.0/Sigmoidal.egg-info/top_level.txt
--rw-r--r--   0 jade       (502) staff       (20)       38 2023-06-01 18:46:45.887377 Sigmoidal-0.3.0/setup.cfg
--rw-r--r--   0 jade       (502) staff       (20)      723 2023-06-01 18:10:41.000000 Sigmoidal-0.3.0/setup.py
-drwxr-xr-x   0 jade       (502) staff       (20)        0 2023-06-01 18:46:45.886333 Sigmoidal-0.3.0/sigmoidal/
--rw-r--r--   0 jade       (502) staff       (20)     4993 2023-06-01 18:46:08.000000 Sigmoidal-0.3.0/sigmoidal/__init__.py
+drwxr-xr-x   0 jade       (502) staff       (20)        0 2023-06-26 19:54:36.814554 Sigmoidal-0.4.0/
+-rw-r--r--   0 jade       (502) staff       (20)     1063 2023-05-22 21:09:43.000000 Sigmoidal-0.4.0/LICENSE
+-rw-r--r--   0 jade       (502) staff       (20)        0 2023-05-22 21:14:28.000000 Sigmoidal-0.4.0/MANIFEST.in
+-rw-r--r--   0 jade       (502) staff       (20)     1542 2023-06-26 19:54:36.813911 Sigmoidal-0.4.0/PKG-INFO
+-rw-r--r--   0 jade       (502) staff       (20)     1057 2023-05-23 02:43:17.000000 Sigmoidal-0.4.0/README.md
+drwxr-xr-x   0 jade       (502) staff       (20)        0 2023-06-26 19:54:36.813428 Sigmoidal-0.4.0/Sigmoidal.egg-info/
+-rw-r--r--   0 jade       (502) staff       (20)     1542 2023-06-26 19:54:36.000000 Sigmoidal-0.4.0/Sigmoidal.egg-info/PKG-INFO
+-rw-r--r--   0 jade       (502) staff       (20)      388 2023-06-26 19:54:36.000000 Sigmoidal-0.4.0/Sigmoidal.egg-info/SOURCES.txt
+-rw-r--r--   0 jade       (502) staff       (20)        1 2023-06-26 19:54:36.000000 Sigmoidal-0.4.0/Sigmoidal.egg-info/dependency_links.txt
+-rw-r--r--   0 jade       (502) staff       (20)       28 2023-06-26 19:54:36.000000 Sigmoidal-0.4.0/Sigmoidal.egg-info/requires.txt
+-rw-r--r--   0 jade       (502) staff       (20)       10 2023-06-26 19:54:36.000000 Sigmoidal-0.4.0/Sigmoidal.egg-info/top_level.txt
+-rw-r--r--   0 jade       (502) staff       (20)       38 2023-06-26 19:54:36.814597 Sigmoidal-0.4.0/setup.cfg
+-rw-r--r--   0 jade       (502) staff       (20)      723 2023-06-26 19:53:11.000000 Sigmoidal-0.4.0/setup.py
+drwxr-xr-x   0 jade       (502) staff       (20)        0 2023-06-26 19:54:36.813523 Sigmoidal-0.4.0/sigmoidal/
+-rw-r--r--   0 jade       (502) staff       (20)     4405 2023-06-26 19:49:58.000000 Sigmoidal-0.4.0/sigmoidal/__init__.py
```

### Comparing `Sigmoidal-0.3.0/LICENSE` & `Sigmoidal-0.4.0/LICENSE`

 * *Files identical despite different names*

### Comparing `Sigmoidal-0.3.0/PKG-INFO` & `Sigmoidal-0.4.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: Sigmoidal
-Version: 0.3.0
+Version: 0.4.0
 Summary: Sigmoidal is a small library to allow you to fit and evaluate sigmoid functions in a way that works like the Numpy Polynomial class.
 Home-page: https://github.com/HelloSleuth/sigmoid
 Author: Jade Glaze, Sleuth
 Author-email: jade@hellosleuth.com
 License: MIT
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3.10
```

### Comparing `Sigmoidal-0.3.0/README.md` & `Sigmoidal-0.4.0/README.md`

 * *Files identical despite different names*

### Comparing `Sigmoidal-0.3.0/Sigmoidal.egg-info/PKG-INFO` & `Sigmoidal-0.4.0/Sigmoidal.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: Sigmoidal
-Version: 0.3.0
+Version: 0.4.0
 Summary: Sigmoidal is a small library to allow you to fit and evaluate sigmoid functions in a way that works like the Numpy Polynomial class.
 Home-page: https://github.com/HelloSleuth/sigmoid
 Author: Jade Glaze, Sleuth
 Author-email: jade@hellosleuth.com
 License: MIT
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3.10
```

### Comparing `Sigmoidal-0.3.0/setup.py` & `Sigmoidal-0.4.0/setup.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup
 
 setup(
     name='Sigmoidal',
-    version='0.3.0',
+    version='0.4.0',
     author='Jade Glaze, Sleuth',
     author_email='jade@hellosleuth.com',
     url='https://github.com/HelloSleuth/sigmoid',
     license='MIT',
     description='Sigmoidal is a small library to allow you to fit and evaluate sigmoid functions in a way that works like the Numpy Polynomial class.',
     long_description=open('README.md').read(),
     long_description_content_type='text/markdown',
```

### Comparing `Sigmoidal-0.3.0/sigmoidal/__init__.py` & `Sigmoidal-0.4.0/sigmoidal/__init__.py`

 * *Files 8% similar despite different names*

```diff
@@ -101,38 +101,20 @@
     @staticmethod
     def _negative_scaled_sigmoid(x, L):
         e_ = np.exp(x)
         return (L * e_) / (1 + e_)
 
     @staticmethod
     def _sigmoid(x, L, x0, k, b):
-        x_ = k * (x - x0)
-
-        if isinstance(x_, np.ndarray):
-            positive_mask = x_ >= 0
-            negative_mask = ~positive_mask
-
-            y = np.empty_like(x_, dtype=np.float64)
-            y[positive_mask] = Sigmoid._positive_scaled_sigmoid(x_[positive_mask], L)
-            y[negative_mask] = Sigmoid._negative_scaled_sigmoid(x_[negative_mask], L)
-        else:
-            if x_ >= 0:
-                y = Sigmoid._positive_scaled_sigmoid(x_, L)
-            else:
-                y = Sigmoid._negative_scaled_sigmoid(x_, L)
-        y = y + b
-
-        # naive implementation
-        # y = L / (1 + np.exp(-k*(x-x0))) + b
-        return y
+        return L * scipy.special.expit(k * (x - x0)) + b
 
     @staticmethod
     def _derivative_1(x, L, x0, k, *args):
-        e_ = np.exp(-k*(x-x0))
-        y = (k*L*e_)/((1+e_)**2)
+        E = scipy.special.expit(k * (x - x0))
+        y = k * L * E * (1 - E)
         return y
 
     @staticmethod
     def _derivative_2(x, L, x0, k, *args):
         e_kxx0 = np.exp(k*(x+x0))
         e_kx0 = np.exp(k*x0)
         e_kx = np.exp(k*x)
```

