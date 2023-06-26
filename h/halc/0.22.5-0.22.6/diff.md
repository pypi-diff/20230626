# Comparing `tmp/halc-0.22.5.tar.gz` & `tmp/halc-0.22.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "halc-0.22.5.tar", last modified: Sun Jun 25 21:38:02 2023, max compression
+gzip compressed data, was "halc-0.22.6.tar", last modified: Mon Jun 26 02:24:46 2023, max compression
```

## Comparing `halc-0.22.5.tar` & `halc-0.22.6.tar`

### file list

```diff
@@ -1,42 +1,42 @@
-drwxrwxr-x   0 lpaarup   (1001) lpaarup   (1001)        0 2023-06-25 21:38:02.614587 halc-0.22.5/
--rw-rw-r--   0 lpaarup   (1001) lpaarup   (1001)     1061 2023-06-14 16:42:42.000000 halc-0.22.5/LICENSE
--rw-rw-r--   0 lpaarup   (1001) lpaarup   (1001)      858 2023-06-25 21:38:02.614587 halc-0.22.5/PKG-INFO
--rw-rw-r--   0 lpaarup   (1001) lpaarup   (1001)      328 2023-06-14 16:36:58.000000 halc-0.22.5/README.md
-drwxrwxr-x   0 lpaarup   (1001) lpaarup   (1001)        0 2023-06-25 21:38:02.610587 halc-0.22.5/halc/
--rw-rw-r--   0 lpaarup   (1001) lpaarup   (1001)      227 2023-06-25 21:37:55.000000 halc-0.22.5/halc/__about__.py
--rw-rw-r--   0 lpaarup   (1001) lpaarup   (1001)      183 2023-06-22 04:12:24.000000 halc-0.22.5/halc/__init__.py
-drwxrwxr-x   0 lpaarup   (1001) lpaarup   (1001)        0 2023-06-25 21:38:02.610587 halc-0.22.5/halc/coco/
--rw-rw-r--   0 lpaarup   (1001) lpaarup   (1001)       23 2023-06-22 04:12:24.000000 halc-0.22.5/halc/coco/__init__.py
--rw-rw-r--   0 lpaarup   (1001) lpaarup   (1001)      343 2023-06-22 04:12:24.000000 halc-0.22.5/halc/coco/parse.py
-drwxrwxr-x   0 lpaarup   (1001) lpaarup   (1001)        0 2023-06-25 21:38:02.610587 halc-0.22.5/halc/images/
--rw-rw-r--   0 lpaarup   (1001) lpaarup   (1001)       42 2023-06-21 23:09:44.000000 halc-0.22.5/halc/images/__init__.py
--rw-rw-r--   0 lpaarup   (1001) lpaarup   (1001)     1246 2023-06-21 23:19:20.000000 halc-0.22.5/halc/images/get.py
--rw-rw-r--   0 lpaarup   (1001) lpaarup   (1001)     5773 2023-06-21 22:47:19.000000 halc-0.22.5/halc/initialize.py
-drwxrwxr-x   0 lpaarup   (1001) lpaarup   (1001)        0 2023-06-25 21:38:02.610587 halc-0.22.5/halc/projects/
--rw-rw-r--   0 lpaarup   (1001) lpaarup   (1001)      127 2023-06-18 04:01:46.000000 halc-0.22.5/halc/projects/__init__.py
--rw-rw-r--   0 lpaarup   (1001) lpaarup   (1001)     1388 2023-06-18 05:35:04.000000 halc-0.22.5/halc/projects/create.py
--rw-rw-r--   0 lpaarup   (1001) lpaarup   (1001)      538 2023-06-18 05:11:14.000000 halc-0.22.5/halc/projects/delete.py
--rw-rw-r--   0 lpaarup   (1001) lpaarup   (1001)     1015 2023-06-18 04:06:48.000000 halc-0.22.5/halc/projects/get.py
-drwxrwxr-x   0 lpaarup   (1001) lpaarup   (1001)        0 2023-06-25 21:38:02.610587 halc-0.22.5/halc/storage/
--rw-rw-r--   0 lpaarup   (1001) lpaarup   (1001)      164 2023-06-18 17:18:21.000000 halc-0.22.5/halc/storage/__init__.py
--rw-rw-r--   0 lpaarup   (1001) lpaarup   (1001)     2494 2023-06-18 18:06:19.000000 halc-0.22.5/halc/storage/create.py
--rw-rw-r--   0 lpaarup   (1001) lpaarup   (1001)      706 2023-06-18 17:21:10.000000 halc-0.22.5/halc/storage/delete.py
--rw-rw-r--   0 lpaarup   (1001) lpaarup   (1001)      617 2023-06-18 17:17:06.000000 halc-0.22.5/halc/storage/get.py
-drwxrwxr-x   0 lpaarup   (1001) lpaarup   (1001)        0 2023-06-25 21:38:02.610587 halc-0.22.5/halc/upload/
--rw-rw-r--   0 lpaarup   (1001) lpaarup   (1001)      133 2023-06-25 21:37:38.000000 halc-0.22.5/halc/upload/__init__.py
--rw-rw-r--   0 lpaarup   (1001) lpaarup   (1001)     6951 2023-06-22 02:52:05.000000 halc-0.22.5/halc/upload/images.py
--rw-rw-r--   0 lpaarup   (1001) lpaarup   (1001)     7000 2023-06-22 04:12:24.000000 halc-0.22.5/halc/upload/labels.py
--rw-rw-r--   0 lpaarup   (1001) lpaarup   (1001)     1379 2023-06-22 04:12:24.000000 halc-0.22.5/halc/utils.py
-drwxrwxr-x   0 lpaarup   (1001) lpaarup   (1001)        0 2023-06-25 21:38:02.614587 halc-0.22.5/halc/versions/
--rw-rw-r--   0 lpaarup   (1001) lpaarup   (1001)      157 2023-06-18 05:17:09.000000 halc-0.22.5/halc/versions/__init__.py
--rw-rw-r--   0 lpaarup   (1001) lpaarup   (1001)     1186 2023-06-18 05:37:02.000000 halc-0.22.5/halc/versions/create.py
--rw-rw-r--   0 lpaarup   (1001) lpaarup   (1001)      707 2023-06-18 05:26:55.000000 halc-0.22.5/halc/versions/delete.py
--rw-rw-r--   0 lpaarup   (1001) lpaarup   (1001)     1596 2023-06-18 05:37:38.000000 halc-0.22.5/halc/versions/get.py
-drwxrwxr-x   0 lpaarup   (1001) lpaarup   (1001)        0 2023-06-25 21:38:02.610587 halc-0.22.5/halc.egg-info/
--rw-rw-r--   0 lpaarup   (1001) lpaarup   (1001)      858 2023-06-25 21:38:02.000000 halc-0.22.5/halc.egg-info/PKG-INFO
--rw-rw-r--   0 lpaarup   (1001) lpaarup   (1001)      676 2023-06-25 21:38:02.000000 halc-0.22.5/halc.egg-info/SOURCES.txt
--rw-rw-r--   0 lpaarup   (1001) lpaarup   (1001)        1 2023-06-25 21:38:02.000000 halc-0.22.5/halc.egg-info/dependency_links.txt
--rw-rw-r--   0 lpaarup   (1001) lpaarup   (1001)      121 2023-06-25 21:38:02.000000 halc-0.22.5/halc.egg-info/requires.txt
--rw-rw-r--   0 lpaarup   (1001) lpaarup   (1001)        5 2023-06-25 21:38:02.000000 halc-0.22.5/halc.egg-info/top_level.txt
--rw-rw-r--   0 lpaarup   (1001) lpaarup   (1001)       79 2023-06-25 21:38:02.614587 halc-0.22.5/setup.cfg
--rw-rw-r--   0 lpaarup   (1001) lpaarup   (1001)     1437 2023-06-22 05:02:03.000000 halc-0.22.5/setup.py
+drwxrwxr-x   0 lpaarup   (1001) lpaarup   (1001)        0 2023-06-26 02:24:46.642684 halc-0.22.6/
+-rw-rw-r--   0 lpaarup   (1001) lpaarup   (1001)     1061 2023-06-14 16:42:42.000000 halc-0.22.6/LICENSE
+-rw-rw-r--   0 lpaarup   (1001) lpaarup   (1001)      858 2023-06-26 02:24:46.642684 halc-0.22.6/PKG-INFO
+-rw-rw-r--   0 lpaarup   (1001) lpaarup   (1001)      328 2023-06-14 16:36:58.000000 halc-0.22.6/README.md
+drwxrwxr-x   0 lpaarup   (1001) lpaarup   (1001)        0 2023-06-26 02:24:46.642684 halc-0.22.6/halc/
+-rw-rw-r--   0 lpaarup   (1001) lpaarup   (1001)      227 2023-06-26 02:24:37.000000 halc-0.22.6/halc/__about__.py
+-rw-rw-r--   0 lpaarup   (1001) lpaarup   (1001)      183 2023-06-22 04:12:24.000000 halc-0.22.6/halc/__init__.py
+drwxrwxr-x   0 lpaarup   (1001) lpaarup   (1001)        0 2023-06-26 02:24:46.642684 halc-0.22.6/halc/coco/
+-rw-rw-r--   0 lpaarup   (1001) lpaarup   (1001)       23 2023-06-22 04:12:24.000000 halc-0.22.6/halc/coco/__init__.py
+-rw-rw-r--   0 lpaarup   (1001) lpaarup   (1001)      343 2023-06-22 04:12:24.000000 halc-0.22.6/halc/coco/parse.py
+drwxrwxr-x   0 lpaarup   (1001) lpaarup   (1001)        0 2023-06-26 02:24:46.642684 halc-0.22.6/halc/images/
+-rw-rw-r--   0 lpaarup   (1001) lpaarup   (1001)       42 2023-06-21 23:09:44.000000 halc-0.22.6/halc/images/__init__.py
+-rw-rw-r--   0 lpaarup   (1001) lpaarup   (1001)     1246 2023-06-21 23:19:20.000000 halc-0.22.6/halc/images/get.py
+-rw-rw-r--   0 lpaarup   (1001) lpaarup   (1001)     5773 2023-06-21 22:47:19.000000 halc-0.22.6/halc/initialize.py
+drwxrwxr-x   0 lpaarup   (1001) lpaarup   (1001)        0 2023-06-26 02:24:46.642684 halc-0.22.6/halc/projects/
+-rw-rw-r--   0 lpaarup   (1001) lpaarup   (1001)      127 2023-06-18 04:01:46.000000 halc-0.22.6/halc/projects/__init__.py
+-rw-rw-r--   0 lpaarup   (1001) lpaarup   (1001)     1388 2023-06-18 05:35:04.000000 halc-0.22.6/halc/projects/create.py
+-rw-rw-r--   0 lpaarup   (1001) lpaarup   (1001)      538 2023-06-18 05:11:14.000000 halc-0.22.6/halc/projects/delete.py
+-rw-rw-r--   0 lpaarup   (1001) lpaarup   (1001)     1015 2023-06-18 04:06:48.000000 halc-0.22.6/halc/projects/get.py
+drwxrwxr-x   0 lpaarup   (1001) lpaarup   (1001)        0 2023-06-26 02:24:46.642684 halc-0.22.6/halc/storage/
+-rw-rw-r--   0 lpaarup   (1001) lpaarup   (1001)      164 2023-06-18 17:18:21.000000 halc-0.22.6/halc/storage/__init__.py
+-rw-rw-r--   0 lpaarup   (1001) lpaarup   (1001)     2494 2023-06-18 18:06:19.000000 halc-0.22.6/halc/storage/create.py
+-rw-rw-r--   0 lpaarup   (1001) lpaarup   (1001)      706 2023-06-18 17:21:10.000000 halc-0.22.6/halc/storage/delete.py
+-rw-rw-r--   0 lpaarup   (1001) lpaarup   (1001)      617 2023-06-18 17:17:06.000000 halc-0.22.6/halc/storage/get.py
+drwxrwxr-x   0 lpaarup   (1001) lpaarup   (1001)        0 2023-06-26 02:24:46.642684 halc-0.22.6/halc/upload/
+-rw-rw-r--   0 lpaarup   (1001) lpaarup   (1001)      133 2023-06-25 21:37:38.000000 halc-0.22.6/halc/upload/__init__.py
+-rw-rw-r--   0 lpaarup   (1001) lpaarup   (1001)     6951 2023-06-22 02:52:05.000000 halc-0.22.6/halc/upload/images.py
+-rw-rw-r--   0 lpaarup   (1001) lpaarup   (1001)     7168 2023-06-25 21:47:15.000000 halc-0.22.6/halc/upload/labels.py
+-rw-rw-r--   0 lpaarup   (1001) lpaarup   (1001)     1379 2023-06-22 04:12:24.000000 halc-0.22.6/halc/utils.py
+drwxrwxr-x   0 lpaarup   (1001) lpaarup   (1001)        0 2023-06-26 02:24:46.642684 halc-0.22.6/halc/versions/
+-rw-rw-r--   0 lpaarup   (1001) lpaarup   (1001)      157 2023-06-18 05:17:09.000000 halc-0.22.6/halc/versions/__init__.py
+-rw-rw-r--   0 lpaarup   (1001) lpaarup   (1001)     1186 2023-06-18 05:37:02.000000 halc-0.22.6/halc/versions/create.py
+-rw-rw-r--   0 lpaarup   (1001) lpaarup   (1001)      707 2023-06-18 05:26:55.000000 halc-0.22.6/halc/versions/delete.py
+-rw-rw-r--   0 lpaarup   (1001) lpaarup   (1001)     1596 2023-06-18 05:37:38.000000 halc-0.22.6/halc/versions/get.py
+drwxrwxr-x   0 lpaarup   (1001) lpaarup   (1001)        0 2023-06-26 02:24:46.642684 halc-0.22.6/halc.egg-info/
+-rw-rw-r--   0 lpaarup   (1001) lpaarup   (1001)      858 2023-06-26 02:24:46.000000 halc-0.22.6/halc.egg-info/PKG-INFO
+-rw-rw-r--   0 lpaarup   (1001) lpaarup   (1001)      676 2023-06-26 02:24:46.000000 halc-0.22.6/halc.egg-info/SOURCES.txt
+-rw-rw-r--   0 lpaarup   (1001) lpaarup   (1001)        1 2023-06-26 02:24:46.000000 halc-0.22.6/halc.egg-info/dependency_links.txt
+-rw-rw-r--   0 lpaarup   (1001) lpaarup   (1001)      121 2023-06-26 02:24:46.000000 halc-0.22.6/halc.egg-info/requires.txt
+-rw-rw-r--   0 lpaarup   (1001) lpaarup   (1001)        5 2023-06-26 02:24:46.000000 halc-0.22.6/halc.egg-info/top_level.txt
+-rw-rw-r--   0 lpaarup   (1001) lpaarup   (1001)       79 2023-06-26 02:24:46.642684 halc-0.22.6/setup.cfg
+-rw-rw-r--   0 lpaarup   (1001) lpaarup   (1001)     1437 2023-06-22 05:02:03.000000 halc-0.22.6/setup.py
```

### Comparing `halc-0.22.5/LICENSE` & `halc-0.22.6/LICENSE`

 * *Files identical despite different names*

### Comparing `halc-0.22.5/PKG-INFO` & `halc-0.22.6/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: halc
-Version: 0.22.5
+Version: 0.22.6
 Summary: Python SDK for Happyrobot's HALC
 Home-page: https://happyrobot.ai
 Author: Happyrobot
 Author-email: luis.paarup@happyrobot.ai
 License: MIT
 Keywords: happyrobot computer vision artificial intelligence foundation models large vision
 Classifier: Development Status :: 3 - Alpha
```

### Comparing `halc-0.22.5/halc/images/get.py` & `halc-0.22.6/halc/images/get.py`

 * *Files identical despite different names*

### Comparing `halc-0.22.5/halc/initialize.py` & `halc-0.22.6/halc/initialize.py`

 * *Files identical despite different names*

### Comparing `halc-0.22.5/halc/projects/create.py` & `halc-0.22.6/halc/projects/create.py`

 * *Files identical despite different names*

### Comparing `halc-0.22.5/halc/projects/delete.py` & `halc-0.22.6/halc/projects/delete.py`

 * *Files identical despite different names*

### Comparing `halc-0.22.5/halc/projects/get.py` & `halc-0.22.6/halc/projects/get.py`

 * *Files identical despite different names*

### Comparing `halc-0.22.5/halc/storage/create.py` & `halc-0.22.6/halc/storage/create.py`

 * *Files identical despite different names*

### Comparing `halc-0.22.5/halc/storage/delete.py` & `halc-0.22.6/halc/storage/delete.py`

 * *Files identical despite different names*

### Comparing `halc-0.22.5/halc/storage/get.py` & `halc-0.22.6/halc/storage/get.py`

 * *Files identical despite different names*

### Comparing `halc-0.22.5/halc/upload/images.py` & `halc-0.22.6/halc/upload/images.py`

 * *Files identical despite different names*

### Comparing `halc-0.22.5/halc/upload/labels.py` & `halc-0.22.6/halc/upload/labels.py`

 * *Files 2% similar despite different names*

```diff
@@ -171,14 +171,17 @@
                     # RLE is a list of ints
                     if len(seg["counts"]) < 2:
                         # Discard RLEs with less than 2 elements
                         continue
                     rle = seg["counts"]
                 else:
                     # Rle is coco compressed string. Convert to list of ints.
+                    if isinstance(seg["counts"], str):
+                        # Convert to bytes
+                        seg["counts"] = seg["counts"].encode("ascii")
                     rle = compressed_rle_to_list(seg["counts"])
                 annotation["segmentation"] = {"rle": rle}
 
         # Add annotation to list
         image_with_annotations["annotations"].append(annotation)
         cls["count"] += 1
```

### Comparing `halc-0.22.5/halc/utils.py` & `halc-0.22.6/halc/utils.py`

 * *Files identical despite different names*

### Comparing `halc-0.22.5/halc/versions/create.py` & `halc-0.22.6/halc/versions/create.py`

 * *Files identical despite different names*

### Comparing `halc-0.22.5/halc/versions/delete.py` & `halc-0.22.6/halc/versions/delete.py`

 * *Files identical despite different names*

### Comparing `halc-0.22.5/halc/versions/get.py` & `halc-0.22.6/halc/versions/get.py`

 * *Files identical despite different names*

### Comparing `halc-0.22.5/halc.egg-info/PKG-INFO` & `halc-0.22.6/halc.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: halc
-Version: 0.22.5
+Version: 0.22.6
 Summary: Python SDK for Happyrobot's HALC
 Home-page: https://happyrobot.ai
 Author: Happyrobot
 Author-email: luis.paarup@happyrobot.ai
 License: MIT
 Keywords: happyrobot computer vision artificial intelligence foundation models large vision
 Classifier: Development Status :: 3 - Alpha
```

### Comparing `halc-0.22.5/halc.egg-info/SOURCES.txt` & `halc-0.22.6/halc.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `halc-0.22.5/setup.py` & `halc-0.22.6/setup.py`

 * *Files identical despite different names*

