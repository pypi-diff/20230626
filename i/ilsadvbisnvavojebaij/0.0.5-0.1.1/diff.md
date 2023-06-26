# Comparing `tmp/ilsadvbisnvavojebaij-0.0.5.tar.gz` & `tmp/ilsadvbisnvavojebaij-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ilsadvbisnvavojebaij-0.0.5.tar", last modified: Mon Jun 26 00:54:38 2023, max compression
+gzip compressed data, was "ilsadvbisnvavojebaij-0.1.1.tar", last modified: Mon Jun 26 04:52:15 2023, max compression
```

## Comparing `ilsadvbisnvavojebaij-0.0.5.tar` & `ilsadvbisnvavojebaij-0.1.1.tar`

### file list

```diff
@@ -1,21 +1,21 @@
-drwxr-xr-x   0 kiko       (501) staff       (20)        0 2023-06-26 00:54:38.022003 ilsadvbisnvavojebaij-0.0.5/
--rw-r--r--   0 kiko       (501) staff       (20)      516 2023-06-26 00:54:38.022174 ilsadvbisnvavojebaij-0.0.5/PKG-INFO
--rw-r--r--   0 kiko       (501) staff       (20)        0 2023-06-25 20:21:40.000000 ilsadvbisnvavojebaij-0.0.5/README.md
--rw-r--r--   0 kiko       (501) staff       (20)       89 2023-06-25 20:21:40.000000 ilsadvbisnvavojebaij-0.0.5/pyproject.toml
--rw-r--r--   0 kiko       (501) staff       (20)      740 2023-06-26 00:54:38.023082 ilsadvbisnvavojebaij-0.0.5/setup.cfg
-drwxr-xr-x   0 kiko       (501) staff       (20)        0 2023-06-26 00:54:37.979496 ilsadvbisnvavojebaij-0.0.5/src/
-drwxr-xr-x   0 kiko       (501) staff       (20)        0 2023-06-26 00:54:37.982241 ilsadvbisnvavojebaij-0.0.5/src/ilsadvbisnvavojebaij/
--rw-r--r--   0 kiko       (501) staff       (20)       22 2023-06-26 00:45:05.000000 ilsadvbisnvavojebaij-0.0.5/src/ilsadvbisnvavojebaij/__init__.py
-drwxr-xr-x   0 kiko       (501) staff       (20)        0 2023-06-26 00:54:38.020008 ilsadvbisnvavojebaij-0.0.5/src/ilsadvbisnvavojebaij/math/
--rw-r--r--   0 kiko       (501) staff       (20)        0 2023-06-25 20:21:40.000000 ilsadvbisnvavojebaij-0.0.5/src/ilsadvbisnvavojebaij/math/__init__.py
--rw-r--r--   0 kiko       (501) staff       (20)      499 2023-06-25 20:21:40.000000 ilsadvbisnvavojebaij-0.0.5/src/ilsadvbisnvavojebaij/math/scalars.py
--rw-r--r--   0 kiko       (501) staff       (20)      949 2023-06-25 20:21:40.000000 ilsadvbisnvavojebaij-0.0.5/src/ilsadvbisnvavojebaij/math/vectors.py
-drwxr-xr-x   0 kiko       (501) staff       (20)        0 2023-06-26 00:54:38.021422 ilsadvbisnvavojebaij-0.0.5/src/ilsadvbisnvavojebaij/utils/
--rw-r--r--   0 kiko       (501) staff       (20)        0 2023-06-25 20:21:40.000000 ilsadvbisnvavojebaij-0.0.5/src/ilsadvbisnvavojebaij/utils/__init__.py
--rw-r--r--   0 kiko       (501) staff       (20)     1245 2023-06-25 20:21:40.000000 ilsadvbisnvavojebaij-0.0.5/src/ilsadvbisnvavojebaij/utils/logging.py
-drwxr-xr-x   0 kiko       (501) staff       (20)        0 2023-06-26 00:54:37.985898 ilsadvbisnvavojebaij-0.0.5/src/ilsadvbisnvavojebaij.egg-info/
--rw-r--r--   0 kiko       (501) staff       (20)      516 2023-06-26 00:54:37.000000 ilsadvbisnvavojebaij-0.0.5/src/ilsadvbisnvavojebaij.egg-info/PKG-INFO
--rw-r--r--   0 kiko       (501) staff       (20)      519 2023-06-26 00:54:37.000000 ilsadvbisnvavojebaij-0.0.5/src/ilsadvbisnvavojebaij.egg-info/SOURCES.txt
--rw-r--r--   0 kiko       (501) staff       (20)        1 2023-06-26 00:54:37.000000 ilsadvbisnvavojebaij-0.0.5/src/ilsadvbisnvavojebaij.egg-info/dependency_links.txt
--rw-r--r--   0 kiko       (501) staff       (20)       14 2023-06-26 00:54:37.000000 ilsadvbisnvavojebaij-0.0.5/src/ilsadvbisnvavojebaij.egg-info/requires.txt
--rw-r--r--   0 kiko       (501) staff       (20)       21 2023-06-26 00:54:37.000000 ilsadvbisnvavojebaij-0.0.5/src/ilsadvbisnvavojebaij.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 04:52:15.721088 ilsadvbisnvavojebaij-0.1.1/
+-rw-r--r--   0 runner    (1001) docker     (123)      516 2023-06-26 04:52:15.721088 ilsadvbisnvavojebaij-0.1.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-26 04:51:38.000000 ilsadvbisnvavojebaij-0.1.1/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       89 2023-06-26 04:51:38.000000 ilsadvbisnvavojebaij-0.1.1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      740 2023-06-26 04:52:15.721088 ilsadvbisnvavojebaij-0.1.1/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 04:52:15.717087 ilsadvbisnvavojebaij-0.1.1/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 04:52:15.717087 ilsadvbisnvavojebaij-0.1.1/src/ilsadvbisnvavojebaij/
+-rw-r--r--   0 runner    (1001) docker     (123)       22 2023-06-26 04:51:38.000000 ilsadvbisnvavojebaij-0.1.1/src/ilsadvbisnvavojebaij/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 04:52:15.717087 ilsadvbisnvavojebaij-0.1.1/src/ilsadvbisnvavojebaij/math/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-26 04:51:38.000000 ilsadvbisnvavojebaij-0.1.1/src/ilsadvbisnvavojebaij/math/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      499 2023-06-26 04:51:38.000000 ilsadvbisnvavojebaij-0.1.1/src/ilsadvbisnvavojebaij/math/scalars.py
+-rw-r--r--   0 runner    (1001) docker     (123)      949 2023-06-26 04:51:38.000000 ilsadvbisnvavojebaij-0.1.1/src/ilsadvbisnvavojebaij/math/vectors.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 04:52:15.721088 ilsadvbisnvavojebaij-0.1.1/src/ilsadvbisnvavojebaij/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-26 04:51:38.000000 ilsadvbisnvavojebaij-0.1.1/src/ilsadvbisnvavojebaij/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1245 2023-06-26 04:51:38.000000 ilsadvbisnvavojebaij-0.1.1/src/ilsadvbisnvavojebaij/utils/logging.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 04:52:15.717087 ilsadvbisnvavojebaij-0.1.1/src/ilsadvbisnvavojebaij.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      516 2023-06-26 04:52:15.000000 ilsadvbisnvavojebaij-0.1.1/src/ilsadvbisnvavojebaij.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      519 2023-06-26 04:52:15.000000 ilsadvbisnvavojebaij-0.1.1/src/ilsadvbisnvavojebaij.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-26 04:52:15.000000 ilsadvbisnvavojebaij-0.1.1/src/ilsadvbisnvavojebaij.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       14 2023-06-26 04:52:15.000000 ilsadvbisnvavojebaij-0.1.1/src/ilsadvbisnvavojebaij.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       21 2023-06-26 04:52:15.000000 ilsadvbisnvavojebaij-0.1.1/src/ilsadvbisnvavojebaij.egg-info/top_level.txt
```

### Comparing `ilsadvbisnvavojebaij-0.0.5/PKG-INFO` & `ilsadvbisnvavojebaij-0.1.1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ilsadvbisnvavojebaij
-Version: 0.0.5
+Version: 0.1.1
 Summary: A randome placeholder package for CI testing
 Author: Francisco Castillo
 Author-email: fjcastillocarrasco@gmail.com
 Classifier: Development Status :: 1 - Planning
 Classifier: Intended Audience :: Developers
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
```

### Comparing `ilsadvbisnvavojebaij-0.0.5/setup.cfg` & `ilsadvbisnvavojebaij-0.1.1/setup.cfg`

 * *Files identical despite different names*

### Comparing `ilsadvbisnvavojebaij-0.0.5/src/ilsadvbisnvavojebaij/math/vectors.py` & `ilsadvbisnvavojebaij-0.1.1/src/ilsadvbisnvavojebaij/math/vectors.py`

 * *Files identical despite different names*

### Comparing `ilsadvbisnvavojebaij-0.0.5/src/ilsadvbisnvavojebaij/utils/logging.py` & `ilsadvbisnvavojebaij-0.1.1/src/ilsadvbisnvavojebaij/utils/logging.py`

 * *Files identical despite different names*

### Comparing `ilsadvbisnvavojebaij-0.0.5/src/ilsadvbisnvavojebaij.egg-info/PKG-INFO` & `ilsadvbisnvavojebaij-0.1.1/src/ilsadvbisnvavojebaij.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ilsadvbisnvavojebaij
-Version: 0.0.5
+Version: 0.1.1
 Summary: A randome placeholder package for CI testing
 Author: Francisco Castillo
 Author-email: fjcastillocarrasco@gmail.com
 Classifier: Development Status :: 1 - Planning
 Classifier: Intended Audience :: Developers
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
```

### Comparing `ilsadvbisnvavojebaij-0.0.5/src/ilsadvbisnvavojebaij.egg-info/SOURCES.txt` & `ilsadvbisnvavojebaij-0.1.1/src/ilsadvbisnvavojebaij.egg-info/SOURCES.txt`

 * *Files identical despite different names*

