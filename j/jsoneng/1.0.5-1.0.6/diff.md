# Comparing `tmp/jsoneng-1.0.5.tar.gz` & `tmp/jsoneng-1.0.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "jsoneng-1.0.5.tar", last modified: Tue Jun 13 18:43:56 2023, max compression
+gzip compressed data, was "jsoneng-1.0.6.tar", last modified: Mon Jun 26 00:34:09 2023, max compression
```

## Comparing `jsoneng-1.0.5.tar` & `jsoneng-1.0.6.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxrwxrwx   0        0        0        0 2023-06-13 18:43:56.380214 jsoneng-1.0.5/
--rw-rw-rw-   0        0        0     1091 2023-05-13 03:44:08.000000 jsoneng-1.0.5/LICENSE
--rw-rw-rw-   0        0        0     2021 2023-06-13 18:43:56.381135 jsoneng-1.0.5/PKG-INFO
--rw-rw-rw-   0        0        0     1478 2023-05-13 03:44:08.000000 jsoneng-1.0.5/README.md
--rw-rw-rw-   0        0        0      108 2023-05-13 03:44:08.000000 jsoneng-1.0.5/pyproject.toml
--rw-rw-rw-   0        0        0      682 2023-06-13 18:43:56.381135 jsoneng-1.0.5/setup.cfg
-drwxrwxrwx   0        0        0        0 2023-06-13 18:43:56.350785 jsoneng-1.0.5/src/
-drwxrwxrwx   0        0        0        0 2023-06-13 18:43:56.366494 jsoneng-1.0.5/src/jsoneng/
--rw-rw-rw-   0        0        0     7904 2023-06-13 18:40:04.000000 jsoneng-1.0.5/src/jsoneng/__init__.py
-drwxrwxrwx   0        0        0        0 2023-06-13 18:43:56.380214 jsoneng-1.0.5/src/jsoneng.egg-info/
--rw-rw-rw-   0        0        0     2021 2023-06-13 18:43:56.000000 jsoneng-1.0.5/src/jsoneng.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      206 2023-06-13 18:43:56.000000 jsoneng-1.0.5/src/jsoneng.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-13 18:43:56.000000 jsoneng-1.0.5/src/jsoneng.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        8 2023-06-13 18:43:56.000000 jsoneng-1.0.5/src/jsoneng.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-06-26 00:34:09.471504 jsoneng-1.0.6/
+-rw-rw-rw-   0        0        0     1091 2023-05-13 03:44:08.000000 jsoneng-1.0.6/LICENSE
+-rw-rw-rw-   0        0        0     2021 2023-06-26 00:34:09.471504 jsoneng-1.0.6/PKG-INFO
+-rw-rw-rw-   0        0        0     1478 2023-05-13 03:44:08.000000 jsoneng-1.0.6/README.md
+-rw-rw-rw-   0        0        0      108 2023-05-13 03:44:08.000000 jsoneng-1.0.6/pyproject.toml
+-rw-rw-rw-   0        0        0      682 2023-06-26 00:34:09.473586 jsoneng-1.0.6/setup.cfg
+drwxrwxrwx   0        0        0        0 2023-06-26 00:34:09.393917 jsoneng-1.0.6/src/
+drwxrwxrwx   0        0        0        0 2023-06-26 00:34:09.446826 jsoneng-1.0.6/src/jsoneng/
+-rw-rw-rw-   0        0        0     4244 2023-06-26 00:31:47.000000 jsoneng-1.0.6/src/jsoneng/__init__.py
+drwxrwxrwx   0        0        0        0 2023-06-26 00:34:09.466069 jsoneng-1.0.6/src/jsoneng.egg-info/
+-rw-rw-rw-   0        0        0     2021 2023-06-26 00:34:09.000000 jsoneng-1.0.6/src/jsoneng.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      206 2023-06-26 00:34:09.000000 jsoneng-1.0.6/src/jsoneng.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-26 00:34:09.000000 jsoneng-1.0.6/src/jsoneng.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        8 2023-06-26 00:34:09.000000 jsoneng-1.0.6/src/jsoneng.egg-info/top_level.txt
```

### Comparing `jsoneng-1.0.5/LICENSE` & `jsoneng-1.0.6/LICENSE`

 * *Files identical despite different names*

### Comparing `jsoneng-1.0.5/PKG-INFO` & `jsoneng-1.0.6/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: jsoneng
-Version: 1.0.5
+Version: 1.0.6
 Summary: A package for a python JSON database CRUD engine
 Home-page: https://github.com/youhengzhou/jsoneng
 Author: YouHeng Zhou
 Author-email: youhengzhou@cmail.carleton.ca
 Project-URL: Bug Tracker, https://github.com/youhengzhou/jsoneng/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `jsoneng-1.0.5/README.md` & `jsoneng-1.0.6/README.md`

 * *Files identical despite different names*

### Comparing `jsoneng-1.0.5/setup.cfg` & `jsoneng-1.0.6/setup.cfg`

 * *Files 17% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 00000000: 5b6d 6574 6164 6174 615d 0d0a 6e61 6d65  [metadata]..name
 00000010: 203d 206a 736f 6e65 6e67 0d0a 7665 7273   = jsoneng..vers
-00000020: 696f 6e20 3d20 312e 302e 350d 0a61 7574  ion = 1.0.5..aut
+00000020: 696f 6e20 3d20 312e 302e 360d 0a61 7574  ion = 1.0.6..aut
 00000030: 686f 7220 3d20 596f 7548 656e 6720 5a68  hor = YouHeng Zh
 00000040: 6f75 0d0a 6175 7468 6f72 5f65 6d61 696c  ou..author_email
 00000050: 203d 2079 6f75 6865 6e67 7a68 6f75 4063   = youhengzhou@c
 00000060: 6d61 696c 2e63 6172 6c65 746f 6e2e 6361  mail.carleton.ca
 00000070: 0d0a 6465 7363 7269 7074 696f 6e20 3d20  ..description = 
 00000080: 4120 7061 636b 6167 6520 666f 7220 6120  A package for a 
 00000090: 7079 7468 6f6e 204a 534f 4e20 6461 7461  python JSON data
```

### Comparing `jsoneng-1.0.5/src/jsoneng.egg-info/PKG-INFO` & `jsoneng-1.0.6/src/jsoneng.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: jsoneng
-Version: 1.0.5
+Version: 1.0.6
 Summary: A package for a python JSON database CRUD engine
 Home-page: https://github.com/youhengzhou/jsoneng
 Author: YouHeng Zhou
 Author-email: youhengzhou@cmail.carleton.ca
 Project-URL: Bug Tracker, https://github.com/youhengzhou/jsoneng/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

