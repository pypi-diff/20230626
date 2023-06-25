# Comparing `tmp/framegrab-0.1.1.tar.gz` & `tmp/framegrab-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "framegrab-0.1.1.tar", max compression
+gzip compressed data, was "framegrab-0.1.2.tar", max compression
```

## Comparing `framegrab-0.1.1.tar` & `framegrab-0.1.2.tar`

### file list

```diff
@@ -1,6 +1,7 @@
--rw-r--r--   0        0        0     1071 2023-06-16 19:22:23.911251 framegrab-0.1.1/LICENSE.txt
--rw-r--r--   0        0        0     2906 2023-06-16 19:22:23.911372 framegrab-0.1.1/README.md
--rw-r--r--   0        0        0      471 2023-06-25 18:57:35.749379 framegrab-0.1.1/pyproject.toml
--rw-r--r--   0        0        0    10360 2023-06-16 19:22:23.911782 framegrab-0.1.1/src/framegrab/grabber.py
--rw-r--r--   0        0        0     2456 2023-06-24 01:53:17.596683 framegrab-0.1.1/src/framegrab/motion.py
--rw-r--r--   0        0        0     3641 1970-01-01 00:00:00.000000 framegrab-0.1.1/PKG-INFO
+-rw-r--r--   0        0        0     1071 2023-06-16 19:22:23.911251 framegrab-0.1.2/LICENSE.txt
+-rw-r--r--   0        0        0     2906 2023-06-16 19:22:23.911372 framegrab-0.1.2/README.md
+-rw-r--r--   0        0        0      487 2023-06-25 22:41:55.703134 framegrab-0.1.2/pyproject.toml
+-rw-r--r--   0        0        0      388 2023-06-25 22:41:55.703396 framegrab-0.1.2/src/framegrab/__init__.py
+-rw-r--r--   0        0        0    10360 2023-06-16 19:22:23.911782 framegrab-0.1.2/src/framegrab/grabber.py
+-rw-r--r--   0        0        0     2456 2023-06-24 01:53:17.596683 framegrab-0.1.2/src/framegrab/motion.py
+-rw-r--r--   0        0        0     3678 1970-01-01 00:00:00.000000 framegrab-0.1.2/PKG-INFO
```

### Comparing `framegrab-0.1.1/LICENSE.txt` & `framegrab-0.1.2/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `framegrab-0.1.1/README.md` & `framegrab-0.1.2/README.md`

 * *Files identical despite different names*

### Comparing `framegrab-0.1.1/src/framegrab/grabber.py` & `framegrab-0.1.2/src/framegrab/grabber.py`

 * *Files identical despite different names*

### Comparing `framegrab-0.1.1/src/framegrab/motion.py` & `framegrab-0.1.2/src/framegrab/motion.py`

 * *Files identical despite different names*

### Comparing `framegrab-0.1.1/PKG-INFO` & `framegrab-0.1.2/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,23 +1,24 @@
 Metadata-Version: 2.1
 Name: framegrab
-Version: 0.1.1
+Version: 0.1.2
 Summary: Easily grab frames from cameras or streams
 License: MIT
 Author: Groundlight
 Author-email: info@groundlight.ai
 Requires-Python: >=3.7,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Requires-Dist: opencv-python (>=4.7.0.72,<5.0.0.0)
+Requires-Dist: pafy (>=0.5.5,<0.6.0)
 Requires-Dist: pillow (>=9.5.0,<10.0.0)
 Requires-Dist: youtube-dl (>=2021.12.17,<2022.0.0)
 Description-Content-Type: text/markdown
 
 # FrameGrab by Groundlight
 ## A user-friendly library for grabbing images from cameras or streams
```

