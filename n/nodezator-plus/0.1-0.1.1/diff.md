# Comparing `tmp/nodezator_plus-0.1.tar.gz` & `tmp/nodezator_plus-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nodezator_plus-0.1.tar", last modified: Mon Jun 26 16:48:59 2023, max compression
+gzip compressed data, was "nodezator_plus-0.1.1.tar", last modified: Mon Jun 26 21:33:05 2023, max compression
```

## Comparing `nodezator_plus-0.1.tar` & `nodezator_plus-0.1.1.tar`

### file list

```diff
@@ -1,18 +1,24 @@
-drwxrwxrwx   0        0        0        0 2023-06-26 16:48:59.261057 nodezator_plus-0.1/
--rw-rw-rw-   0        0        0      126 2023-06-26 16:48:59.261057 nodezator_plus-0.1/PKG-INFO
-drwxrwxrwx   0        0        0        0 2023-06-26 16:48:59.183713 nodezator_plus-0.1/nodezator_plus/
--rw-rw-rw-   0        0        0       91 2023-06-26 16:21:11.000000 nodezator_plus-0.1/nodezator_plus/__init__.py
--rw-rw-rw-   0        0        0      169 2023-06-26 15:55:20.000000 nodezator_plus-0.1/nodezator_plus/__main__.py
--rw-rw-rw-   0        0        0      583 2023-06-26 14:55:13.000000 nodezator_plus-0.1/nodezator_plus/anim.py
--rw-rw-rw-   0        0        0      521 2023-06-26 15:49:03.000000 nodezator_plus-0.1/nodezator_plus/cli.py
--rw-rw-rw-   0        0        0     4668 2023-06-26 14:53:13.000000 nodezator_plus-0.1/nodezator_plus/double_translation.py
--rw-rw-rw-   0        0        0    14215 2023-06-26 14:53:30.000000 nodezator_plus-0.1/nodezator_plus/menu1.py
--rw-rw-rw-   0        0        0     1284 2023-06-26 16:00:33.000000 nodezator_plus-0.1/nodezator_plus/translate.py
-drwxrwxrwx   0        0        0        0 2023-06-26 16:48:59.258057 nodezator_plus-0.1/nodezator_plus.egg-info/
--rw-rw-rw-   0        0        0      126 2023-06-26 16:48:58.000000 nodezator_plus-0.1/nodezator_plus.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      395 2023-06-26 16:48:58.000000 nodezator_plus-0.1/nodezator_plus.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-26 16:48:58.000000 nodezator_plus-0.1/nodezator_plus.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        2 2023-06-26 16:48:58.000000 nodezator_plus-0.1/nodezator_plus.egg-info/not-zip-safe
--rw-rw-rw-   0        0        0       15 2023-06-26 16:48:58.000000 nodezator_plus-0.1/nodezator_plus.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-06-26 16:48:59.264060 nodezator_plus-0.1/setup.cfg
--rw-rw-rw-   0        0        0      228 2023-06-26 16:39:24.000000 nodezator_plus-0.1/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-26 21:33:05.739275 nodezator_plus-0.1.1/
+-rw-rw-rw-   0        0        0     1635 2023-06-26 21:33:05.740255 nodezator_plus-0.1.1/PKG-INFO
+drwxrwxrwx   0        0        0        0 2023-06-26 21:33:05.671715 nodezator_plus-0.1.1/nodezator_plus/
+-rw-rw-rw-   0        0        0        0 2023-06-26 20:57:32.000000 nodezator_plus-0.1.1/nodezator_plus/__init__.py
+-rw-rw-rw-   0        0        0      273 2023-06-26 21:18:06.000000 nodezator_plus-0.1.1/nodezator_plus/__main__.py
+-rw-rw-rw-   0        0        0   213202 2023-06-26 13:57:58.000000 nodezator_plus-0.1.1/nodezator_plus/anim.mp4
+-rw-rw-rw-   0        0        0      583 2023-06-26 14:55:13.000000 nodezator_plus-0.1.1/nodezator_plus/anim.py
+-rw-rw-rw-   0        0        0      563 2023-06-26 21:18:38.000000 nodezator_plus-0.1.1/nodezator_plus/cli.py
+-rw-rw-rw-   0        0        0     4668 2023-06-26 14:53:13.000000 nodezator_plus-0.1.1/nodezator_plus/double_translation.py
+-rw-rw-rw-   0        0        0    14215 2023-06-26 14:53:30.000000 nodezator_plus-0.1.1/nodezator_plus/menu1.py
+drwxrwxrwx   0        0        0        0 2023-06-26 21:33:05.731609 nodezator_plus-0.1.1/nodezator_plus/ru/
+-rw-rw-rw-   0        0        0     3594 2023-06-23 13:45:39.000000 nodezator_plus-0.1.1/nodezator_plus/ru/dialogs_map.pyl
+-rw-rw-rw-   0        0        0        4 2023-06-23 11:15:50.000000 nodezator_plus-0.1.1/nodezator_plus/ru/status_messages_map.pyl
+-rw-rw-rw-   0        0        0     9011 2023-06-25 10:32:56.000000 nodezator_plus-0.1.1/nodezator_plus/ru/translations_map.pyl
+-rw-rw-rw-   0        0        0     1284 2023-06-26 16:00:33.000000 nodezator_plus-0.1.1/nodezator_plus/translate.py
+drwxrwxrwx   0        0        0        0 2023-06-26 21:33:05.716552 nodezator_plus-0.1.1/nodezator_plus.egg-info/
+-rw-rw-rw-   0        0        0     1635 2023-06-26 21:33:05.000000 nodezator_plus-0.1.1/nodezator_plus.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      571 2023-06-26 21:33:05.000000 nodezator_plus-0.1.1/nodezator_plus.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-26 21:33:05.000000 nodezator_plus-0.1.1/nodezator_plus.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        2 2023-06-26 21:33:05.000000 nodezator_plus-0.1.1/nodezator_plus.egg-info/not-zip-safe
+-rw-rw-rw-   0        0        0       23 2023-06-26 21:33:05.000000 nodezator_plus-0.1.1/nodezator_plus.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       15 2023-06-26 21:33:05.000000 nodezator_plus-0.1.1/nodezator_plus.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0     1554 2023-06-26 21:33:05.761078 nodezator_plus-0.1.1/setup.cfg
+-rw-rw-rw-   0        0        0      411 2023-06-26 21:28:44.000000 nodezator_plus-0.1.1/setup.py
```

### Comparing `nodezator_plus-0.1/nodezator_plus/anim.py` & `nodezator_plus-0.1.1/nodezator_plus/anim.py`

 * *Files identical despite different names*

### Comparing `nodezator_plus-0.1/nodezator_plus/double_translation.py` & `nodezator_plus-0.1.1/nodezator_plus/double_translation.py`

 * *Files identical despite different names*

### Comparing `nodezator_plus-0.1/nodezator_plus/menu1.py` & `nodezator_plus-0.1.1/nodezator_plus/menu1.py`

 * *Files identical despite different names*

### Comparing `nodezator_plus-0.1/nodezator_plus/translate.py` & `nodezator_plus-0.1.1/nodezator_plus/translate.py`

 * *Files identical despite different names*

