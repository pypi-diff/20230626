# Comparing `tmp/chatgpt_functions-0.0.2.tar.gz` & `tmp/chatgpt_functions-0.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, last modified: Sun Feb  2 00:00:00 2020, max compression
+gzip compressed data, was "chatgpt_functions-0.0.3.tar", last modified: Mon Jun 26 14:38:11 2023, max compression
```

## Comparing `chatgpt_functions-0.0.2.tar` & `chatgpt_functions-0.0.3.tar`

### file list

```diff
@@ -1,14 +1,14 @@
--rw-r--r--   0        0        0      144 2020-02-02 00:00:00.000000 chatgpt_functions-0.0.2/config.py
--rw-r--r--   0        0        0     2278 2020-02-02 00:00:00.000000 chatgpt_functions-0.0.2/main.py
--rw-r--r--   0        0        0       78 2020-02-02 00:00:00.000000 chatgpt_functions-0.0.2/requirements.txt
--rw-r--r--   0        0        0       83 2020-02-02 00:00:00.000000 chatgpt_functions-0.0.2/src/chatgpt_functions/__init__.py
--rw-r--r--   0        0        0     2060 2020-02-02 00:00:00.000000 chatgpt_functions-0.0.2/src/chatgpt_functions/chatgpt.py
--rw-r--r--   0        0        0      722 2020-02-02 00:00:00.000000 chatgpt_functions-0.0.2/src/chatgpt_functions/chatgpt_function.py
--rw-r--r--   0        0        0      448 2020-02-02 00:00:00.000000 chatgpt_functions-0.0.2/src/chatgpt_functions/chatgpt_types.py
--rw-r--r--   0        0        0     1319 2020-02-02 00:00:00.000000 chatgpt_functions-0.0.2/src/chatgpt_functions/function_parameters.py
--rw-r--r--   0        0        0       30 2020-02-02 00:00:00.000000 chatgpt_functions-0.0.2/test/hello.py
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 chatgpt_functions-0.0.2/.gitignore
--rw-r--r--   0        0        0     1091 2020-02-02 00:00:00.000000 chatgpt_functions-0.0.2/LICENSE
--rw-r--r--   0        0        0     1374 2020-02-02 00:00:00.000000 chatgpt_functions-0.0.2/README.md
--rw-r--r--   0        0        0      639 2020-02-02 00:00:00.000000 chatgpt_functions-0.0.2/pyproject.toml
--rw-r--r--   0        0        0     1883 2020-02-02 00:00:00.000000 chatgpt_functions-0.0.2/PKG-INFO
+drwxrwxrwx   0        0        0        0 2023-06-26 14:38:11.228014 chatgpt_functions-0.0.3/
+-rw-rw-rw-   0        0        0     1091 2023-06-26 13:13:15.000000 chatgpt_functions-0.0.3/LICENSE
+-rw-rw-rw-   0        0        0     1865 2023-06-26 14:38:11.228014 chatgpt_functions-0.0.3/PKG-INFO
+-rw-rw-rw-   0        0        0     1374 2023-06-26 12:54:41.000000 chatgpt_functions-0.0.3/README.md
+drwxrwxrwx   0        0        0        0 2023-06-26 14:38:11.226008 chatgpt_functions-0.0.3/chatgpt_functions.egg-info/
+-rw-rw-rw-   0        0        0     1865 2023-06-26 14:38:11.000000 chatgpt_functions-0.0.3/chatgpt_functions.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      291 2023-06-26 14:38:11.000000 chatgpt_functions-0.0.3/chatgpt_functions.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-26 14:38:11.000000 chatgpt_functions-0.0.3/chatgpt_functions.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       36 2023-06-26 14:38:11.000000 chatgpt_functions-0.0.3/chatgpt_functions.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        1 2023-06-26 14:38:11.000000 chatgpt_functions-0.0.3/chatgpt_functions.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0        2 2023-06-26 14:38:11.000000 chatgpt_functions-0.0.3/chatgpt_functions.egg-info/zip-safe
+-rw-rw-rw-   0        0        0      682 2023-06-26 14:36:57.000000 chatgpt_functions-0.0.3/pyproject.toml
+-rw-rw-rw-   0        0        0      690 2023-06-26 14:38:11.230015 chatgpt_functions-0.0.3/setup.cfg
+-rw-rw-rw-   0        0        0       39 2023-06-26 14:27:24.000000 chatgpt_functions-0.0.3/setup.py
```

### Comparing `chatgpt_functions-0.0.2/LICENSE` & `chatgpt_functions-0.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `chatgpt_functions-0.0.2/README.md` & `chatgpt_functions-0.0.3/README.md`

 * *Files identical despite different names*

