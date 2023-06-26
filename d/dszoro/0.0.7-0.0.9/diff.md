# Comparing `tmp/dszoro-0.0.7.tar.gz` & `tmp/dszoro-0.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dszoro-0.0.7.tar", last modified: Sun Jun 25 17:30:42 2023, max compression
+gzip compressed data, was "dszoro-0.0.9.tar", last modified: Mon Jun 26 03:07:19 2023, max compression
```

## Comparing `dszoro-0.0.7.tar` & `dszoro-0.0.9.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxrwxrwx   0        0        0        0 2023-06-25 17:30:42.403357 dszoro-0.0.7/
--rw-rw-rw-   0        0        0        0 2023-06-25 11:25:13.000000 dszoro-0.0.7/LICENSE
--rw-rw-rw-   0        0        0     3331 2023-06-25 17:30:42.404665 dszoro-0.0.7/PKG-INFO
--rw-rw-rw-   0        0        0     2883 2023-06-24 13:28:53.000000 dszoro-0.0.7/README.md
--rw-rw-rw-   0        0        0      108 2023-06-24 13:24:03.000000 dszoro-0.0.7/pyproject.toml
--rw-rw-rw-   0        0        0      590 2023-06-25 17:30:42.411742 dszoro-0.0.7/setup.cfg
-drwxrwxrwx   0        0        0        0 2023-06-25 17:30:42.385557 dszoro-0.0.7/src/
-drwxrwxrwx   0        0        0        0 2023-06-25 17:30:42.394478 dszoro-0.0.7/src/dszoro/
--rw-rw-rw-   0        0        0        0 2023-06-24 13:22:36.000000 dszoro-0.0.7/src/dszoro/__init__.py
--rw-rw-rw-   0        0        0    27455 2023-06-25 17:22:49.000000 dszoro-0.0.7/src/dszoro/codes.py
-drwxrwxrwx   0        0        0        0 2023-06-25 17:30:42.402304 dszoro-0.0.7/src/dszoro.egg-info/
--rw-rw-rw-   0        0        0     3331 2023-06-25 17:30:42.000000 dszoro-0.0.7/src/dszoro.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      221 2023-06-25 17:30:42.000000 dszoro-0.0.7/src/dszoro.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-25 17:30:42.000000 dszoro-0.0.7/src/dszoro.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        7 2023-06-25 17:30:42.000000 dszoro-0.0.7/src/dszoro.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-06-26 03:07:19.846239 dszoro-0.0.9/
+-rw-rw-rw-   0        0        0        0 2023-06-25 11:25:13.000000 dszoro-0.0.9/LICENSE
+-rw-rw-rw-   0        0        0     3331 2023-06-26 03:07:19.846239 dszoro-0.0.9/PKG-INFO
+-rw-rw-rw-   0        0        0     2883 2023-06-24 13:28:53.000000 dszoro-0.0.9/README.md
+-rw-rw-rw-   0        0        0      108 2023-06-24 13:24:03.000000 dszoro-0.0.9/pyproject.toml
+-rw-rw-rw-   0        0        0      590 2023-06-26 03:07:19.850512 dszoro-0.0.9/setup.cfg
+drwxrwxrwx   0        0        0        0 2023-06-26 03:07:19.794402 dszoro-0.0.9/src/
+drwxrwxrwx   0        0        0        0 2023-06-26 03:07:19.811316 dszoro-0.0.9/src/dszoro/
+-rw-rw-rw-   0        0        0        0 2023-06-24 13:22:36.000000 dszoro-0.0.9/src/dszoro/__init__.py
+-rw-rw-rw-   0        0        0    55351 2023-06-26 03:01:56.000000 dszoro-0.0.9/src/dszoro/program.py
+drwxrwxrwx   0        0        0        0 2023-06-26 03:07:19.843089 dszoro-0.0.9/src/dszoro.egg-info/
+-rw-rw-rw-   0        0        0     3331 2023-06-26 03:07:19.000000 dszoro-0.0.9/src/dszoro.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      223 2023-06-26 03:07:19.000000 dszoro-0.0.9/src/dszoro.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-26 03:07:19.000000 dszoro-0.0.9/src/dszoro.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        7 2023-06-26 03:07:19.000000 dszoro-0.0.9/src/dszoro.egg-info/top_level.txt
```

### Comparing `dszoro-0.0.7/PKG-INFO` & `dszoro-0.0.9/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dszoro
-Version: 0.0.7
+Version: 0.0.9
 Summary: A small example package
 Author: Zoro
 Author-email: author@example.com
 Project-URL: Bug Tracker, https://github.com/pypa/sampleproject/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `dszoro-0.0.7/README.md` & `dszoro-0.0.9/README.md`

 * *Files identical despite different names*

### Comparing `dszoro-0.0.7/setup.cfg` & `dszoro-0.0.9/setup.cfg`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 00000000: 5b6d 6574 6164 6174 615d 0d0a 6e61 6d65  [metadata]..name
 00000010: 203d 2064 737a 6f72 6f0d 0a76 6572 7369   = dszoro..versi
-00000020: 6f6e 203d 2030 2e30 2e37 0d0a 6175 7468  on = 0.0.7..auth
+00000020: 6f6e 203d 2030 2e30 2e39 0d0a 6175 7468  on = 0.0.9..auth
 00000030: 6f72 203d 205a 6f72 6f0d 0a61 7574 686f  or = Zoro..autho
 00000040: 725f 656d 6169 6c20 3d20 6175 7468 6f72  r_email = author
 00000050: 4065 7861 6d70 6c65 2e63 6f6d 0d0a 6465  @example.com..de
 00000060: 7363 7269 7074 696f 6e20 3d20 4120 736d  scription = A sm
 00000070: 616c 6c20 6578 616d 706c 6520 7061 636b  all example pack
 00000080: 6167 650d 0a6c 6f6e 675f 6465 7363 7269  age..long_descri
 00000090: 7074 696f 6e20 3d20 6669 6c65 3a20 5245  ption = file: RE
```

### Comparing `dszoro-0.0.7/src/dszoro.egg-info/PKG-INFO` & `dszoro-0.0.9/src/dszoro.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dszoro
-Version: 0.0.7
+Version: 0.0.9
 Summary: A small example package
 Author: Zoro
 Author-email: author@example.com
 Project-URL: Bug Tracker, https://github.com/pypa/sampleproject/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

