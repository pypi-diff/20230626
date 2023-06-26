# Comparing `tmp/geneabacus-0.3.1.tar.gz` & `tmp/geneabacus-0.3.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "geneabacus-0.3.1.tar", last modified: Thu Jun 22 18:43:22 2023, max compression
+gzip compressed data, was "geneabacus-0.3.2.tar", last modified: Mon Jun 26 19:58:01 2023, max compression
```

## Comparing `geneabacus-0.3.1.tar` & `geneabacus-0.3.2.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 build     (1000) build     (1001)        0 2023-06-22 18:43:22.002443 geneabacus-0.3.1/
--rw-r--r--   0 build     (1000) build     (1001)       17 2023-06-22 18:42:53.000000 geneabacus-0.3.1/.gitignore
-drwxr-xr-x   0 build     (1000) build     (1001)        0 2023-06-22 18:43:22.002443 geneabacus-0.3.1/.sourcehut/
--rw-r--r--   0 build     (1000) build     (1001)     1290 2023-06-22 18:42:53.000000 geneabacus-0.3.1/.sourcehut/arch.yml
--rw-r--r--   0 build     (1000) build     (1001)    16726 2023-06-22 18:42:53.000000 geneabacus-0.3.1/LICENSE
--rw-r--r--   0 build     (1000) build     (1001)     1448 2023-06-22 18:43:22.002443 geneabacus-0.3.1/PKG-INFO
--rw-r--r--   0 build     (1000) build     (1001)     1137 2023-06-22 18:42:53.000000 geneabacus-0.3.1/README.md
--rw-r--r--   0 build     (1000) build     (1001)      131 2023-06-22 18:42:53.000000 geneabacus-0.3.1/pyproject.toml
--rw-r--r--   0 build     (1000) build     (1001)      465 2023-06-22 18:43:22.002443 geneabacus-0.3.1/setup.cfg
-drwxr-xr-x   0 build     (1000) build     (1001)        0 2023-06-22 18:43:21.999108 geneabacus-0.3.1/src/
-drwxr-xr-x   0 build     (1000) build     (1001)        0 2023-06-22 18:43:22.002443 geneabacus-0.3.1/src/geneabacus/
--rw-r--r--   0 build     (1000) build     (1001)        0 2023-06-22 18:42:53.000000 geneabacus-0.3.1/src/geneabacus/__init__.py
--rw-r--r--   0 build     (1000) build     (1001)     5222 2023-06-22 18:42:53.000000 geneabacus-0.3.1/src/geneabacus/profileio.py
-drwxr-xr-x   0 build     (1000) build     (1001)        0 2023-06-22 18:43:22.002443 geneabacus-0.3.1/src/geneabacus.egg-info/
--rw-r--r--   0 build     (1000) build     (1001)     1448 2023-06-22 18:43:21.000000 geneabacus-0.3.1/src/geneabacus.egg-info/PKG-INFO
--rw-r--r--   0 build     (1000) build     (1001)      317 2023-06-22 18:43:21.000000 geneabacus-0.3.1/src/geneabacus.egg-info/SOURCES.txt
--rw-r--r--   0 build     (1000) build     (1001)        1 2023-06-22 18:43:21.000000 geneabacus-0.3.1/src/geneabacus.egg-info/dependency_links.txt
--rw-r--r--   0 build     (1000) build     (1001)       10 2023-06-22 18:43:21.000000 geneabacus-0.3.1/src/geneabacus.egg-info/requires.txt
--rw-r--r--   0 build     (1000) build     (1001)       11 2023-06-22 18:43:21.000000 geneabacus-0.3.1/src/geneabacus.egg-info/top_level.txt
+drwxr-xr-x   0 build     (1000) build     (1001)        0 2023-06-26 19:58:01.306877 geneabacus-0.3.2/
+-rw-r--r--   0 build     (1000) build     (1001)       17 2023-06-26 19:57:20.000000 geneabacus-0.3.2/.gitignore
+drwxr-xr-x   0 build     (1000) build     (1001)        0 2023-06-26 19:58:01.303543 geneabacus-0.3.2/.sourcehut/
+-rw-r--r--   0 build     (1000) build     (1001)     1290 2023-06-26 19:57:20.000000 geneabacus-0.3.2/.sourcehut/arch.yml
+-rw-r--r--   0 build     (1000) build     (1001)    16726 2023-06-26 19:57:20.000000 geneabacus-0.3.2/LICENSE
+-rw-r--r--   0 build     (1000) build     (1001)     1448 2023-06-26 19:58:01.306877 geneabacus-0.3.2/PKG-INFO
+-rw-r--r--   0 build     (1000) build     (1001)     1137 2023-06-26 19:57:20.000000 geneabacus-0.3.2/README.md
+-rw-r--r--   0 build     (1000) build     (1001)      131 2023-06-26 19:57:20.000000 geneabacus-0.3.2/pyproject.toml
+-rw-r--r--   0 build     (1000) build     (1001)      476 2023-06-26 19:58:01.306877 geneabacus-0.3.2/setup.cfg
+drwxr-xr-x   0 build     (1000) build     (1001)        0 2023-06-26 19:58:01.300210 geneabacus-0.3.2/src/
+drwxr-xr-x   0 build     (1000) build     (1001)        0 2023-06-26 19:58:01.303543 geneabacus-0.3.2/src/geneabacus/
+-rw-r--r--   0 build     (1000) build     (1001)        0 2023-06-26 19:57:20.000000 geneabacus-0.3.2/src/geneabacus/__init__.py
+-rw-r--r--   0 build     (1000) build     (1001)     5222 2023-06-26 19:57:20.000000 geneabacus-0.3.2/src/geneabacus/profileio.py
+drwxr-xr-x   0 build     (1000) build     (1001)        0 2023-06-26 19:58:01.306877 geneabacus-0.3.2/src/geneabacus.egg-info/
+-rw-r--r--   0 build     (1000) build     (1001)     1448 2023-06-26 19:58:01.000000 geneabacus-0.3.2/src/geneabacus.egg-info/PKG-INFO
+-rw-r--r--   0 build     (1000) build     (1001)      317 2023-06-26 19:58:01.000000 geneabacus-0.3.2/src/geneabacus.egg-info/SOURCES.txt
+-rw-r--r--   0 build     (1000) build     (1001)        1 2023-06-26 19:58:01.000000 geneabacus-0.3.2/src/geneabacus.egg-info/dependency_links.txt
+-rw-r--r--   0 build     (1000) build     (1001)       20 2023-06-26 19:58:01.000000 geneabacus-0.3.2/src/geneabacus.egg-info/requires.txt
+-rw-r--r--   0 build     (1000) build     (1001)       11 2023-06-26 19:58:01.000000 geneabacus-0.3.2/src/geneabacus.egg-info/top_level.txt
```

### Comparing `geneabacus-0.3.1/.sourcehut/arch.yml` & `geneabacus-0.3.2/.sourcehut/arch.yml`

 * *Files identical despite different names*

### Comparing `geneabacus-0.3.1/LICENSE` & `geneabacus-0.3.2/LICENSE`

 * *Files identical despite different names*

### Comparing `geneabacus-0.3.1/PKG-INFO` & `geneabacus-0.3.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: geneabacus
-Version: 0.3.1
+Version: 0.3.2
 Summary: Python IO functions for GeneAbacus
 Home-page: https://git.sr.ht/~vejnar/GeneAbacus-python
 Author: Charles E. Vejnar
 License: Mozilla Public License 2.0 (MPL 2.0)
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

### Comparing `geneabacus-0.3.1/README.md` & `geneabacus-0.3.2/README.md`

 * *Files identical despite different names*

### Comparing `geneabacus-0.3.1/src/geneabacus/profileio.py` & `geneabacus-0.3.2/src/geneabacus/profileio.py`

 * *Files identical despite different names*

### Comparing `geneabacus-0.3.1/src/geneabacus.egg-info/PKG-INFO` & `geneabacus-0.3.2/src/geneabacus.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: geneabacus
-Version: 0.3.1
+Version: 0.3.2
 Summary: Python IO functions for GeneAbacus
 Home-page: https://git.sr.ht/~vejnar/GeneAbacus-python
 Author: Charles E. Vejnar
 License: Mozilla Public License 2.0 (MPL 2.0)
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

