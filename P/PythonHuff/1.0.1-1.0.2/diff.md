# Comparing `tmp/PythonHuff-1.0.1.tar.gz` & `tmp/PythonHuff-1.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist\PythonHuff-1.0.1.tar", last modified: Mon Jun 26 13:59:21 2023, max compression
+gzip compressed data, was "dist\PythonHuff-1.0.2.tar", last modified: Mon Jun 26 14:00:49 2023, max compression
```

## Comparing `PythonHuff-1.0.1.tar` & `PythonHuff-1.0.2.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxrwxrwx   0        0        0        0 2023-06-26 13:59:21.590782 PythonHuff-1.0.1/
--rw-rw-rw-   0        0        0     1480 2023-06-26 13:59:21.575117 PythonHuff-1.0.1/PKG-INFO
-drwxrwxrwx   0        0        0        0 2023-06-26 13:59:21.575117 PythonHuff-1.0.1/PythonHuff.egg-info/
--rw-rw-rw-   0        0        0     1480 2023-06-26 13:59:21.000000 PythonHuff-1.0.1/PythonHuff.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      228 2023-06-26 13:59:21.000000 PythonHuff-1.0.1/PythonHuff.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-26 13:59:21.000000 PythonHuff-1.0.1/PythonHuff.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       43 2023-06-26 13:59:21.000000 PythonHuff-1.0.1/PythonHuff.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0        7 2023-06-26 13:59:21.000000 PythonHuff-1.0.1/PythonHuff.egg-info/top_level.txt
--rw-rw-rw-   0        0        0      864 2023-06-26 09:45:17.000000 PythonHuff-1.0.1/README.md
-drwxrwxrwx   0        0        0        0 2023-06-26 13:59:21.575117 PythonHuff-1.0.1/pyhuff/
--rw-rw-rw-   0        0        0     4183 2023-06-26 13:58:21.000000 PythonHuff-1.0.1/pyhuff/__init__.py
--rw-rw-rw-   0        0        0     2452 2023-06-26 08:39:21.000000 PythonHuff-1.0.1/pyhuff/classes.py
--rw-rw-rw-   0        0        0       42 2023-06-26 13:59:21.590782 PythonHuff-1.0.1/setup.cfg
--rw-rw-rw-   0        0        0      697 2023-06-26 13:59:15.000000 PythonHuff-1.0.1/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-26 14:00:49.181289 PythonHuff-1.0.2/
+-rw-rw-rw-   0        0        0     1480 2023-06-26 14:00:49.181289 PythonHuff-1.0.2/PKG-INFO
+drwxrwxrwx   0        0        0        0 2023-06-26 14:00:49.181289 PythonHuff-1.0.2/PythonHuff.egg-info/
+-rw-rw-rw-   0        0        0     1480 2023-06-26 14:00:49.000000 PythonHuff-1.0.2/PythonHuff.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      228 2023-06-26 14:00:49.000000 PythonHuff-1.0.2/PythonHuff.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-26 14:00:49.000000 PythonHuff-1.0.2/PythonHuff.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       43 2023-06-26 14:00:49.000000 PythonHuff-1.0.2/PythonHuff.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0        7 2023-06-26 14:00:49.000000 PythonHuff-1.0.2/PythonHuff.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0      864 2023-06-26 09:45:17.000000 PythonHuff-1.0.2/README.md
+drwxrwxrwx   0        0        0        0 2023-06-26 14:00:49.181289 PythonHuff-1.0.2/pyhuff/
+-rw-rw-rw-   0        0        0     4183 2023-06-26 13:58:21.000000 PythonHuff-1.0.2/pyhuff/__init__.py
+-rw-rw-rw-   0        0        0     2452 2023-06-26 08:39:21.000000 PythonHuff-1.0.2/pyhuff/classes.py
+-rw-rw-rw-   0        0        0       42 2023-06-26 14:00:49.181289 PythonHuff-1.0.2/setup.cfg
+-rw-rw-rw-   0        0        0      697 2023-06-26 14:00:46.000000 PythonHuff-1.0.2/setup.py
```

### Comparing `PythonHuff-1.0.1/PKG-INFO` & `PythonHuff-1.0.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: PythonHuff
-Version: 1.0.1
+Version: 1.0.2
 Summary: Huffman compression and decompression (Pure Python implementation)
 Home-page: UNKNOWN
 License: UNKNOWN
 Description: <p><span><span style="font-family:Verdana, Arial, Helvetica, sans-serif;line-height:19px;text-indent:26px;"><span style="font-size:14px;"><span style="font-family:Arial;line-height:26px;"><br></span></span></span></span></p>
         
         ### Usage
         ```python
```

### Comparing `PythonHuff-1.0.1/PythonHuff.egg-info/PKG-INFO` & `PythonHuff-1.0.2/PythonHuff.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: PythonHuff
-Version: 1.0.1
+Version: 1.0.2
 Summary: Huffman compression and decompression (Pure Python implementation)
 Home-page: UNKNOWN
 License: UNKNOWN
 Description: <p><span><span style="font-family:Verdana, Arial, Helvetica, sans-serif;line-height:19px;text-indent:26px;"><span style="font-size:14px;"><span style="font-family:Arial;line-height:26px;"><br></span></span></span></span></p>
         
         ### Usage
         ```python
```

### Comparing `PythonHuff-1.0.1/README.md` & `PythonHuff-1.0.2/README.md`

 * *Files identical despite different names*

### Comparing `PythonHuff-1.0.1/pyhuff/__init__.py` & `PythonHuff-1.0.2/pyhuff/__init__.py`

 * *Files identical despite different names*

### Comparing `PythonHuff-1.0.1/pyhuff/classes.py` & `PythonHuff-1.0.2/pyhuff/classes.py`

 * *Files identical despite different names*

### Comparing `PythonHuff-1.0.1/setup.py` & `PythonHuff-1.0.2/setup.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,22 +1,22 @@
 from setuptools import setup
 def readme():
     with open('README.md','r') as f:
         return f.read()
 setup(
     name='PythonHuff',
-    version='1.0.1',
+    version='1.0.2',
     packages=['pyhuff'],
     description='Huffman compression and decompression (Pure Python implementation)',
     long_description=readme(),
     long_description_content_type='text/markdown',
     keywords=['huffman','compression','decompression','algorithm'],
     classifiers=[
         'Programming Language :: Python :: 3',
         'Programming Language :: Python :: 2',
         'Operating System :: OS Independent',
     ],entry_points={
         'console_scripts':[
-            'pyhuff=pyhuff._script'
+            'pyhuff=pyhuff:_script'
         ]
     }
 )
```

