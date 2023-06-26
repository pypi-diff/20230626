# Comparing `tmp/navigation_with_image_language_model-0.1.tar.gz` & `tmp/navigation_with_image_language_model-1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "navigation_with_image_language_model-0.1.tar", last modified: Mon Jun 26 09:27:03 2023, max compression
+gzip compressed data, was "navigation_with_image_language_model-1.0.tar", last modified: Mon Jun 26 09:14:44 2023, max compression
```

## Comparing `navigation_with_image_language_model-0.1.tar` & `navigation_with_image_language_model-1.0.tar`

### file list

```diff
@@ -1,26 +1,26 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-26 09:27:03.204295 navigation_with_image_language_model-0.1/
--rw-r--r--   0 root         (0) root         (0)      235 2023-06-26 09:27:03.204295 navigation_with_image_language_model-0.1/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)       38 2023-04-07 14:02:00.000000 navigation_with_image_language_model-0.1/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-26 09:27:03.204295 navigation_with_image_language_model-0.1/navigation_with_image_language_model.egg-info/
--rw-r--r--   0 root         (0) root         (0)      235 2023-06-26 09:27:03.000000 navigation_with_image_language_model-0.1/navigation_with_image_language_model.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      621 2023-06-26 09:27:03.000000 navigation_with_image_language_model-0.1/navigation_with_image_language_model.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-06-26 09:27:03.000000 navigation_with_image_language_model-0.1/navigation_with_image_language_model.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)     1419 2023-06-26 09:27:03.000000 navigation_with_image_language_model-0.1/navigation_with_image_language_model.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       17 2023-06-26 09:27:03.000000 navigation_with_image_language_model-0.1/navigation_with_image_language_model.egg-info/top_level.txt
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-26 09:27:03.204295 navigation_with_image_language_model-0.1/pipeline/
--rw-r--r--   0 root         (0) root         (0)        0 2023-06-25 10:24:00.000000 navigation_with_image_language_model-0.1/pipeline/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-26 09:27:03.204295 navigation_with_image_language_model-0.1/pipeline/clipseg/
--rw-r--r--   0 root         (0) root         (0)        0 2023-06-25 11:27:29.000000 navigation_with_image_language_model-0.1/pipeline/clipseg/__init__.py
--rwxr-xr-x   0 root         (0) root         (0)     9281 2023-04-07 14:23:59.000000 navigation_with_image_language_model-0.1/pipeline/clipseg/evaluation_utils.py
--rwxr-xr-x   0 root         (0) root         (0)     9288 2023-04-07 14:23:59.000000 navigation_with_image_language_model-0.1/pipeline/clipseg/general_utils.py
--rwxr-xr-x   0 root         (0) root         (0)    10606 2023-04-07 14:23:59.000000 navigation_with_image_language_model-0.1/pipeline/clipseg/metrics.py
--rw-r--r--   0 root         (0) root         (0)    16896 2023-04-07 14:23:59.000000 navigation_with_image_language_model-0.1/pipeline/clipseg/score.py
--rw-r--r--   0 root         (0) root         (0)      787 2023-04-07 14:23:59.000000 navigation_with_image_language_model-0.1/pipeline/clipseg/setup.py
--rw-r--r--   0 root         (0) root         (0)    10397 2023-04-07 14:23:59.000000 navigation_with_image_language_model-0.1/pipeline/clipseg/training.py
--rw-r--r--   0 root         (0) root         (0)     2874 2023-06-25 11:33:40.000000 navigation_with_image_language_model-0.1/pipeline/eval.py
--rw-r--r--   0 root         (0) root         (0)    14016 2023-06-25 11:32:21.000000 navigation_with_image_language_model-0.1/pipeline/models.py
--rw-r--r--   0 root         (0) root         (0)     6236 2023-06-25 10:09:53.000000 navigation_with_image_language_model-0.1/pipeline/utils.py
--rw-r--r--   0 root         (0) root         (0)       38 2023-06-26 09:27:03.208295 navigation_with_image_language_model-0.1/setup.cfg
--rw-r--r--   0 root         (0) root         (0)     2571 2023-06-26 09:26:55.000000 navigation_with_image_language_model-0.1/setup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-26 09:27:03.204295 navigation_with_image_language_model-0.1/weights/
--rw-r--r--   0 root         (0) root         (0)        0 2023-06-25 11:27:44.000000 navigation_with_image_language_model-0.1/weights/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-26 09:14:44.671362 navigation_with_image_language_model-1.0/
+-rw-r--r--   0 root         (0) root         (0)      203 2023-06-26 09:14:44.671362 navigation_with_image_language_model-1.0/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)       38 2023-04-07 14:02:00.000000 navigation_with_image_language_model-1.0/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-26 09:14:44.671362 navigation_with_image_language_model-1.0/navigation_with_image_language_model.egg-info/
+-rw-r--r--   0 root         (0) root         (0)      203 2023-06-26 09:14:44.000000 navigation_with_image_language_model-1.0/navigation_with_image_language_model.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      621 2023-06-26 09:14:44.000000 navigation_with_image_language_model-1.0/navigation_with_image_language_model.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-06-26 09:14:44.000000 navigation_with_image_language_model-1.0/navigation_with_image_language_model.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)     1419 2023-06-26 09:14:44.000000 navigation_with_image_language_model-1.0/navigation_with_image_language_model.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       17 2023-06-26 09:14:44.000000 navigation_with_image_language_model-1.0/navigation_with_image_language_model.egg-info/top_level.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-26 09:14:44.671362 navigation_with_image_language_model-1.0/pipeline/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-06-25 10:24:00.000000 navigation_with_image_language_model-1.0/pipeline/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-26 09:14:44.671362 navigation_with_image_language_model-1.0/pipeline/clipseg/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-06-25 11:27:29.000000 navigation_with_image_language_model-1.0/pipeline/clipseg/__init__.py
+-rwxr-xr-x   0 root         (0) root         (0)     9281 2023-04-07 14:23:59.000000 navigation_with_image_language_model-1.0/pipeline/clipseg/evaluation_utils.py
+-rwxr-xr-x   0 root         (0) root         (0)     9288 2023-04-07 14:23:59.000000 navigation_with_image_language_model-1.0/pipeline/clipseg/general_utils.py
+-rwxr-xr-x   0 root         (0) root         (0)    10606 2023-04-07 14:23:59.000000 navigation_with_image_language_model-1.0/pipeline/clipseg/metrics.py
+-rw-r--r--   0 root         (0) root         (0)    16896 2023-04-07 14:23:59.000000 navigation_with_image_language_model-1.0/pipeline/clipseg/score.py
+-rw-r--r--   0 root         (0) root         (0)      787 2023-04-07 14:23:59.000000 navigation_with_image_language_model-1.0/pipeline/clipseg/setup.py
+-rw-r--r--   0 root         (0) root         (0)    10397 2023-04-07 14:23:59.000000 navigation_with_image_language_model-1.0/pipeline/clipseg/training.py
+-rw-r--r--   0 root         (0) root         (0)     2874 2023-06-25 11:33:40.000000 navigation_with_image_language_model-1.0/pipeline/eval.py
+-rw-r--r--   0 root         (0) root         (0)    14016 2023-06-25 11:32:21.000000 navigation_with_image_language_model-1.0/pipeline/models.py
+-rw-r--r--   0 root         (0) root         (0)     6236 2023-06-25 10:09:53.000000 navigation_with_image_language_model-1.0/pipeline/utils.py
+-rw-r--r--   0 root         (0) root         (0)       38 2023-06-26 09:14:44.671362 navigation_with_image_language_model-1.0/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)     2539 2023-06-25 10:49:02.000000 navigation_with_image_language_model-1.0/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-26 09:14:44.671362 navigation_with_image_language_model-1.0/weights/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-06-25 11:27:44.000000 navigation_with_image_language_model-1.0/weights/__init__.py
```

### Comparing `navigation_with_image_language_model-0.1/navigation_with_image_language_model.egg-info/SOURCES.txt` & `navigation_with_image_language_model-1.0/navigation_with_image_language_model.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `navigation_with_image_language_model-0.1/navigation_with_image_language_model.egg-info/requires.txt` & `navigation_with_image_language_model-1.0/navigation_with_image_language_model.egg-info/requires.txt`

 * *Files identical despite different names*

### Comparing `navigation_with_image_language_model-0.1/pipeline/clipseg/evaluation_utils.py` & `navigation_with_image_language_model-1.0/pipeline/clipseg/evaluation_utils.py`

 * *Files identical despite different names*

### Comparing `navigation_with_image_language_model-0.1/pipeline/clipseg/general_utils.py` & `navigation_with_image_language_model-1.0/pipeline/clipseg/general_utils.py`

 * *Files identical despite different names*

### Comparing `navigation_with_image_language_model-0.1/pipeline/clipseg/metrics.py` & `navigation_with_image_language_model-1.0/pipeline/clipseg/metrics.py`

 * *Files identical despite different names*

### Comparing `navigation_with_image_language_model-0.1/pipeline/clipseg/score.py` & `navigation_with_image_language_model-1.0/pipeline/clipseg/score.py`

 * *Files identical despite different names*

### Comparing `navigation_with_image_language_model-0.1/pipeline/clipseg/setup.py` & `navigation_with_image_language_model-1.0/pipeline/clipseg/setup.py`

 * *Files identical despite different names*

### Comparing `navigation_with_image_language_model-0.1/pipeline/clipseg/training.py` & `navigation_with_image_language_model-1.0/pipeline/clipseg/training.py`

 * *Files identical despite different names*

### Comparing `navigation_with_image_language_model-0.1/pipeline/eval.py` & `navigation_with_image_language_model-1.0/pipeline/eval.py`

 * *Files identical despite different names*

### Comparing `navigation_with_image_language_model-0.1/pipeline/models.py` & `navigation_with_image_language_model-1.0/pipeline/models.py`

 * *Files identical despite different names*

### Comparing `navigation_with_image_language_model-0.1/pipeline/utils.py` & `navigation_with_image_language_model-1.0/pipeline/utils.py`

 * *Files identical despite different names*

### Comparing `navigation_with_image_language_model-0.1/setup.py` & `navigation_with_image_language_model-1.0/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 from setuptools import setup, find_packages
 
 setup(
     name='navigation_with_image_language_model',
-    version='0.1',
-    description='The package provides a pipeline that utilizes models like ClipSeg and StableDiffusion or ClipSeg and SegmentAnything to prompt an image for a path.',
+    version='1.0',
+    description='ClipSeg and StableDiffusion or ClipSeg and SegmentAnything are utilized in a pipeline to prompt an image for a path',
     packages=find_packages(),
     install_requires=[
         'accelerate==0.18.0',
         'aiohttp==3.8.4',
         'aiosignal==1.3.1',
         'asttokens==2.2.1',
         'async-timeout==4.0.2',
```

