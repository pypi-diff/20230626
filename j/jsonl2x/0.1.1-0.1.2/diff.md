# Comparing `tmp/jsonl2x-0.1.1.tar.gz` & `tmp/jsonl2x-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "jsonl2x-0.1.1.tar", last modified: Mon Jun 26 12:02:23 2023, max compression
+gzip compressed data, was "jsonl2x-0.1.2.tar", last modified: Mon Jun 26 12:26:27 2023, max compression
```

## Comparing `jsonl2x-0.1.1.tar` & `jsonl2x-0.1.2.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxr-xr-x   0 wh         (501) staff       (20)        0 2023-06-26 12:02:23.684596 jsonl2x-0.1.1/
--rw-r--r--   0 wh         (501) staff       (20)      667 2023-06-26 12:02:23.684326 jsonl2x-0.1.1/PKG-INFO
--rw-r--r--   0 wh         (501) staff       (20)       35 2023-06-26 12:01:47.000000 jsonl2x-0.1.1/README.md
-drwxr-xr-x   0 wh         (501) staff       (20)        0 2023-06-26 12:02:23.681941 jsonl2x-0.1.1/jsonl2x/
--rw-r--r--   0 wh         (501) staff       (20)       63 2023-06-26 12:02:20.000000 jsonl2x-0.1.1/jsonl2x/__init__.py
--rw-r--r--   0 wh         (501) staff       (20)      713 2023-06-26 11:49:32.000000 jsonl2x-0.1.1/jsonl2x/main.py
-drwxr-xr-x   0 wh         (501) staff       (20)        0 2023-06-26 12:02:23.683915 jsonl2x-0.1.1/jsonl2x.egg-info/
--rw-r--r--   0 wh         (501) staff       (20)      667 2023-06-26 12:02:23.000000 jsonl2x-0.1.1/jsonl2x.egg-info/PKG-INFO
--rw-r--r--   0 wh         (501) staff       (20)      242 2023-06-26 12:02:23.000000 jsonl2x-0.1.1/jsonl2x.egg-info/SOURCES.txt
--rw-r--r--   0 wh         (501) staff       (20)        1 2023-06-26 12:02:23.000000 jsonl2x-0.1.1/jsonl2x.egg-info/dependency_links.txt
--rw-r--r--   0 wh         (501) staff       (20)       47 2023-06-26 12:02:23.000000 jsonl2x-0.1.1/jsonl2x.egg-info/entry_points.txt
--rw-r--r--   0 wh         (501) staff       (20)        7 2023-06-26 12:02:23.000000 jsonl2x-0.1.1/jsonl2x.egg-info/requires.txt
--rw-r--r--   0 wh         (501) staff       (20)        8 2023-06-26 12:02:23.000000 jsonl2x-0.1.1/jsonl2x.egg-info/top_level.txt
--rw-r--r--   0 wh         (501) staff       (20)       38 2023-06-26 12:02:23.684678 jsonl2x-0.1.1/setup.cfg
--rw-r--r--   0 wh         (501) staff       (20)     3845 2023-06-26 11:56:49.000000 jsonl2x-0.1.1/setup.py
+drwxr-xr-x   0 wh         (501) staff       (20)        0 2023-06-26 12:26:27.497525 jsonl2x-0.1.2/
+-rw-r--r--   0 wh         (501) staff       (20)      667 2023-06-26 12:26:27.497280 jsonl2x-0.1.2/PKG-INFO
+-rw-r--r--   0 wh         (501) staff       (20)       35 2023-06-26 12:01:47.000000 jsonl2x-0.1.2/README.md
+drwxr-xr-x   0 wh         (501) staff       (20)        0 2023-06-26 12:26:27.495279 jsonl2x-0.1.2/jsonl2x/
+-rw-r--r--   0 wh         (501) staff       (20)       63 2023-06-26 12:26:02.000000 jsonl2x-0.1.2/jsonl2x/__init__.py
+-rw-r--r--   0 wh         (501) staff       (20)      980 2023-06-26 12:24:22.000000 jsonl2x-0.1.2/jsonl2x/main.py
+drwxr-xr-x   0 wh         (501) staff       (20)        0 2023-06-26 12:26:27.496928 jsonl2x-0.1.2/jsonl2x.egg-info/
+-rw-r--r--   0 wh         (501) staff       (20)      667 2023-06-26 12:26:27.000000 jsonl2x-0.1.2/jsonl2x.egg-info/PKG-INFO
+-rw-r--r--   0 wh         (501) staff       (20)      242 2023-06-26 12:26:27.000000 jsonl2x-0.1.2/jsonl2x.egg-info/SOURCES.txt
+-rw-r--r--   0 wh         (501) staff       (20)        1 2023-06-26 12:26:27.000000 jsonl2x-0.1.2/jsonl2x.egg-info/dependency_links.txt
+-rw-r--r--   0 wh         (501) staff       (20)       47 2023-06-26 12:26:27.000000 jsonl2x-0.1.2/jsonl2x.egg-info/entry_points.txt
+-rw-r--r--   0 wh         (501) staff       (20)        7 2023-06-26 12:26:27.000000 jsonl2x-0.1.2/jsonl2x.egg-info/requires.txt
+-rw-r--r--   0 wh         (501) staff       (20)        8 2023-06-26 12:26:27.000000 jsonl2x-0.1.2/jsonl2x.egg-info/top_level.txt
+-rw-r--r--   0 wh         (501) staff       (20)       38 2023-06-26 12:26:27.497604 jsonl2x-0.1.2/setup.cfg
+-rw-r--r--   0 wh         (501) staff       (20)     3845 2023-06-26 11:56:49.000000 jsonl2x-0.1.2/setup.py
```

### Comparing `jsonl2x-0.1.1/PKG-INFO` & `jsonl2x-0.1.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: jsonl2x
-Version: 0.1.1
+Version: 0.1.2
 Summary: 用来找含有大文件目录的工具
 Home-page: https://gitee.com/WenHao0804/jsonl2x
 Author: WenHao
 Author-email: wh.wenhao@foxmail.com
 License: MIT
 Platform: UNKNOWN
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `jsonl2x-0.1.1/jsonl2x.egg-info/PKG-INFO` & `jsonl2x-0.1.2/jsonl2x.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: jsonl2x
-Version: 0.1.1
+Version: 0.1.2
 Summary: 用来找含有大文件目录的工具
 Home-page: https://gitee.com/WenHao0804/jsonl2x
 Author: WenHao
 Author-email: wh.wenhao@foxmail.com
 License: MIT
 Platform: UNKNOWN
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `jsonl2x-0.1.1/setup.py` & `jsonl2x-0.1.2/setup.py`

 * *Files identical despite different names*

