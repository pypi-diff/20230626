# Comparing `tmp/zhei-0.0.1.tar.gz` & `tmp/zhei-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "zhei-0.0.1.tar", last modified: Mon Jun 26 10:10:29 2023, max compression
+gzip compressed data, was "zhei-0.0.2.tar", last modified: Mon Jun 26 10:45:45 2023, max compression
```

## Comparing `zhei-0.0.1.tar` & `zhei-0.0.2.tar`

### file list

```diff
@@ -1,22 +1,21 @@
-drwxr-xr-x   0 dengyifan   (501) staff       (20)        0 2023-06-26 10:10:29.910856 zhei-0.0.1/
--rw-r--r--   0 dengyifan   (501) staff       (20)      175 2023-06-26 10:10:29.910607 zhei-0.0.1/PKG-INFO
-drwxr-xr-x   0 dengyifan   (501) staff       (20)        0 2023-06-26 10:10:29.906690 zhei-0.0.1/models/
--rw-r--r--   0 dengyifan   (501) staff       (20)        0 2023-06-26 09:58:31.000000 zhei-0.0.1/models/__init__.py
--rw-r--r--   0 dengyifan   (501) staff       (20)        0 2023-06-26 09:42:47.000000 zhei-0.0.1/models/lightning_model.py
--rw-r--r--   0 dengyifan   (501) staff       (20)       38 2023-06-26 10:10:29.910916 zhei-0.0.1/setup.cfg
--rw-r--r--   0 dengyifan   (501) staff       (20)      370 2023-06-26 10:10:25.000000 zhei-0.0.1/setup.py
-drwxr-xr-x   0 dengyifan   (501) staff       (20)        0 2023-06-26 10:10:29.909448 zhei-0.0.1/utils/
--rw-r--r--   0 dengyifan   (501) staff       (20)     4112 2023-06-26 05:12:15.000000 zhei-0.0.1/utils/__init__.py
--rw-r--r--   0 dengyifan   (501) staff       (20)      674 2023-06-26 07:36:31.000000 zhei-0.0.1/utils/catch_error.py
--rw-r--r--   0 dengyifan   (501) staff       (20)    21439 2023-06-26 08:26:20.000000 zhei-0.0.1/utils/eval_methods.py
--rw-r--r--   0 dengyifan   (501) staff       (20)    18295 2023-06-26 09:15:29.000000 zhei-0.0.1/utils/gpu.py
--rw-r--r--   0 dengyifan   (501) staff       (20)     3417 2023-06-26 07:41:13.000000 zhei-0.0.1/utils/io.py
--rw-r--r--   0 dengyifan   (501) staff       (20)      762 2023-06-26 07:31:23.000000 zhei-0.0.1/utils/log.py
--rw-r--r--   0 dengyifan   (501) staff       (20)      418 2023-06-26 09:20:53.000000 zhei-0.0.1/utils/notice.py
--rw-r--r--   0 dengyifan   (501) staff       (20)     4262 2023-06-26 07:25:55.000000 zhei-0.0.1/utils/result.py
--rw-r--r--   0 dengyifan   (501) staff       (20)      813 2023-06-26 09:15:08.000000 zhei-0.0.1/utils/tt.py
-drwxr-xr-x   0 dengyifan   (501) staff       (20)        0 2023-06-26 10:10:29.910262 zhei-0.0.1/zhei.egg-info/
--rw-r--r--   0 dengyifan   (501) staff       (20)      175 2023-06-26 10:10:29.000000 zhei-0.0.1/zhei.egg-info/PKG-INFO
--rw-r--r--   0 dengyifan   (501) staff       (20)      308 2023-06-26 10:10:29.000000 zhei-0.0.1/zhei.egg-info/SOURCES.txt
--rw-r--r--   0 dengyifan   (501) staff       (20)        1 2023-06-26 10:10:29.000000 zhei-0.0.1/zhei.egg-info/dependency_links.txt
--rw-r--r--   0 dengyifan   (501) staff       (20)       13 2023-06-26 10:10:29.000000 zhei-0.0.1/zhei.egg-info/top_level.txt
+drwxr-xr-x   0 dengyifan   (501) staff       (20)        0 2023-06-26 10:45:45.886592 zhei-0.0.2/
+-rw-r--r--   0 dengyifan   (501) staff       (20)      198 2023-06-26 10:45:45.886422 zhei-0.0.2/PKG-INFO
+drwxr-xr-x   0 dengyifan   (501) staff       (20)        0 2023-06-26 10:45:45.883010 zhei-0.0.2/models/
+-rw-r--r--   0 dengyifan   (501) staff       (20)        0 2023-06-26 09:58:31.000000 zhei-0.0.2/models/__init__.py
+-rw-r--r--   0 dengyifan   (501) staff       (20)        0 2023-06-26 09:42:47.000000 zhei-0.0.2/models/lightning_model.py
+-rw-r--r--   0 dengyifan   (501) staff       (20)       38 2023-06-26 10:45:45.886656 zhei-0.0.2/setup.cfg
+-rw-r--r--   0 dengyifan   (501) staff       (20)      459 2023-06-26 10:45:36.000000 zhei-0.0.2/setup.py
+drwxr-xr-x   0 dengyifan   (501) staff       (20)        0 2023-06-26 10:45:45.885471 zhei-0.0.2/utils/
+-rw-r--r--   0 dengyifan   (501) staff       (20)     4112 2023-06-26 05:12:15.000000 zhei-0.0.2/utils/__init__.py
+-rw-r--r--   0 dengyifan   (501) staff       (20)      674 2023-06-26 07:36:31.000000 zhei-0.0.2/utils/catch_error.py
+-rw-r--r--   0 dengyifan   (501) staff       (20)    21439 2023-06-26 08:26:20.000000 zhei-0.0.2/utils/eval_methods.py
+-rw-r--r--   0 dengyifan   (501) staff       (20)    18295 2023-06-26 09:15:29.000000 zhei-0.0.2/utils/gpu.py
+-rw-r--r--   0 dengyifan   (501) staff       (20)     3417 2023-06-26 07:41:13.000000 zhei-0.0.2/utils/io.py
+-rw-r--r--   0 dengyifan   (501) staff       (20)      762 2023-06-26 07:31:23.000000 zhei-0.0.2/utils/log.py
+-rw-r--r--   0 dengyifan   (501) staff       (20)      418 2023-06-26 09:20:53.000000 zhei-0.0.2/utils/notice.py
+-rw-r--r--   0 dengyifan   (501) staff       (20)     4262 2023-06-26 07:25:55.000000 zhei-0.0.2/utils/result.py
+drwxr-xr-x   0 dengyifan   (501) staff       (20)        0 2023-06-26 10:45:45.886192 zhei-0.0.2/zhei.egg-info/
+-rw-r--r--   0 dengyifan   (501) staff       (20)      198 2023-06-26 10:45:45.000000 zhei-0.0.2/zhei.egg-info/PKG-INFO
+-rw-r--r--   0 dengyifan   (501) staff       (20)      296 2023-06-26 10:45:45.000000 zhei-0.0.2/zhei.egg-info/SOURCES.txt
+-rw-r--r--   0 dengyifan   (501) staff       (20)        1 2023-06-26 10:45:45.000000 zhei-0.0.2/zhei.egg-info/dependency_links.txt
+-rw-r--r--   0 dengyifan   (501) staff       (20)       13 2023-06-26 10:45:45.000000 zhei-0.0.2/zhei.egg-info/top_level.txt
```

### Comparing `zhei-0.0.1/utils/__init__.py` & `zhei-0.0.2/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `zhei-0.0.1/utils/catch_error.py` & `zhei-0.0.2/utils/catch_error.py`

 * *Files identical despite different names*

### Comparing `zhei-0.0.1/utils/eval_methods.py` & `zhei-0.0.2/utils/eval_methods.py`

 * *Files identical despite different names*

### Comparing `zhei-0.0.1/utils/gpu.py` & `zhei-0.0.2/utils/gpu.py`

 * *Files identical despite different names*

### Comparing `zhei-0.0.1/utils/io.py` & `zhei-0.0.2/utils/io.py`

 * *Files identical despite different names*

### Comparing `zhei-0.0.1/utils/log.py` & `zhei-0.0.2/utils/log.py`

 * *Files identical despite different names*

### Comparing `zhei-0.0.1/utils/result.py` & `zhei-0.0.2/utils/result.py`

 * *Files identical despite different names*

