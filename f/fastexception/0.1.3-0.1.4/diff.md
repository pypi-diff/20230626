# Comparing `tmp/fastexception-0.1.3.tar.gz` & `tmp/fastexception-0.1.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "fastexception-0.1.3.tar", last modified: Mon Jun 26 08:57:12 2023, max compression
+gzip compressed data, was "fastexception-0.1.4.tar", last modified: Mon Jun 26 10:37:51 2023, max compression
```

## Comparing `fastexception-0.1.3.tar` & `fastexception-0.1.4.tar`

### file list

```diff
@@ -1,12 +1,15 @@
-drwxrwxr-x   0 mojtaba   (1000) mojtaba   (1000)        0 2023-06-26 08:57:12.713100 fastexception-0.1.3/
--rw-rw-r--   0 mojtaba   (1000) mojtaba   (1000)     1062 2023-06-25 19:31:43.000000 fastexception-0.1.3/LICENSE.txt
--rw-rw-r--   0 mojtaba   (1000) mojtaba   (1000)     1300 2023-06-26 08:57:12.713100 fastexception-0.1.3/PKG-INFO
--rw-rw-r--   0 mojtaba   (1000) mojtaba   (1000)     1015 2023-06-26 07:08:25.000000 fastexception-0.1.3/README.md
-drwxrwxr-x   0 mojtaba   (1000) mojtaba   (1000)        0 2023-06-26 08:57:12.713100 fastexception-0.1.3/fastexception.egg-info/
--rw-rw-r--   0 mojtaba   (1000) mojtaba   (1000)     1300 2023-06-26 08:57:12.000000 fastexception-0.1.3/fastexception.egg-info/PKG-INFO
--rw-rw-r--   0 mojtaba   (1000) mojtaba   (1000)      214 2023-06-26 08:57:12.000000 fastexception-0.1.3/fastexception.egg-info/SOURCES.txt
--rw-rw-r--   0 mojtaba   (1000) mojtaba   (1000)        1 2023-06-26 08:57:12.000000 fastexception-0.1.3/fastexception.egg-info/dependency_links.txt
--rw-rw-r--   0 mojtaba   (1000) mojtaba   (1000)       10 2023-06-26 08:57:12.000000 fastexception-0.1.3/fastexception.egg-info/requires.txt
--rw-rw-r--   0 mojtaba   (1000) mojtaba   (1000)        1 2023-06-26 08:57:12.000000 fastexception-0.1.3/fastexception.egg-info/top_level.txt
--rw-rw-r--   0 mojtaba   (1000) mojtaba   (1000)       38 2023-06-26 08:57:12.713100 fastexception-0.1.3/setup.cfg
--rw-rw-r--   0 mojtaba   (1000) mojtaba   (1000)      581 2023-06-26 08:57:07.000000 fastexception-0.1.3/setup.py
+drwxrwxr-x   0 mojtaba   (1000) mojtaba   (1000)        0 2023-06-26 10:37:51.695723 fastexception-0.1.4/
+-rw-rw-r--   0 mojtaba   (1000) mojtaba   (1000)     1056 2023-06-26 09:37:50.000000 fastexception-0.1.4/LICENSE
+-rw-rw-r--   0 mojtaba   (1000) mojtaba   (1000)     1442 2023-06-26 10:37:51.695723 fastexception-0.1.4/PKG-INFO
+-rw-rw-r--   0 mojtaba   (1000) mojtaba   (1000)     1015 2023-06-26 07:08:25.000000 fastexception-0.1.4/README.md
+drwxrwxr-x   0 mojtaba   (1000) mojtaba   (1000)        0 2023-06-26 10:37:51.695723 fastexception-0.1.4/fastexception/
+-rw-rw-r--   0 mojtaba   (1000) mojtaba   (1000)       23 2023-06-26 09:38:39.000000 fastexception-0.1.4/fastexception/__init__.py
+-rw-rw-r--   0 mojtaba   (1000) mojtaba   (1000)     5348 2023-06-25 19:01:41.000000 fastexception-0.1.4/fastexception/fastexception.py
+drwxrwxr-x   0 mojtaba   (1000) mojtaba   (1000)        0 2023-06-26 10:37:51.695723 fastexception-0.1.4/fastexception.egg-info/
+-rw-rw-r--   0 mojtaba   (1000) mojtaba   (1000)     1442 2023-06-26 10:37:51.000000 fastexception-0.1.4/fastexception.egg-info/PKG-INFO
+-rw-rw-r--   0 mojtaba   (1000) mojtaba   (1000)      267 2023-06-26 10:37:51.000000 fastexception-0.1.4/fastexception.egg-info/SOURCES.txt
+-rw-rw-r--   0 mojtaba   (1000) mojtaba   (1000)        1 2023-06-26 10:37:51.000000 fastexception-0.1.4/fastexception.egg-info/dependency_links.txt
+-rw-rw-r--   0 mojtaba   (1000) mojtaba   (1000)       10 2023-06-26 10:37:51.000000 fastexception-0.1.4/fastexception.egg-info/requires.txt
+-rw-rw-r--   0 mojtaba   (1000) mojtaba   (1000)       14 2023-06-26 10:37:51.000000 fastexception-0.1.4/fastexception.egg-info/top_level.txt
+-rw-rw-r--   0 mojtaba   (1000) mojtaba   (1000)       38 2023-06-26 10:37:51.695723 fastexception-0.1.4/setup.cfg
+-rw-rw-r--   0 mojtaba   (1000) mojtaba   (1000)      776 2023-06-26 10:37:37.000000 fastexception-0.1.4/setup.py
```

### Comparing `fastexception-0.1.3/LICENSE.txt` & `fastexception-0.1.4/LICENSE`

 * *Files 5% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-Copyright (c) 2021 Giorgos Myrianthous
+Copyright (c) 2023 Mojtaba Ataei
 
 Permission is hereby granted, free of charge, to any person obtaining
 a copy of this software and associated documentation files (the
 "Software"), to deal in the Software without restriction, including
 without limitation the rights to use, copy, modify, merge, publish,
 distribute, sublicense, and/or sell copies of the Software, and to
 permit persons to whom the Software is furnished to do so, subject to
```

### Comparing `fastexception-0.1.3/PKG-INFO` & `fastexception-0.1.4/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,17 +1,20 @@
 Metadata-Version: 2.1
 Name: fastexception
-Version: 0.1.3
+Version: 0.1.4
 Home-page: https://github.com/mojtabapaso/fastexception
 Author: Mojtaba
 Author-email: mojtabapaso@gamil.com
 License: MIT
 Keywords: FastAPI Tools Fast Exception
+Classifier: Programming Language :: Python :: 3
+Classifier: License :: OSI Approved :: MIT License
+Classifier: Operating System :: OS Independent
 Description-Content-Type: text/markdown
-License-File: LICENSE.txt
+License-File: LICENSE
 
 fast exception
 ===================
 This package is a plugin for easier handling of Exception and sending HTTP status code.
 
 Installing
 ============
```

### Comparing `fastexception-0.1.3/README.md` & `fastexception-0.1.4/README.md`

 * *Files identical despite different names*

### Comparing `fastexception-0.1.3/fastexception.egg-info/PKG-INFO` & `fastexception-0.1.4/fastexception.egg-info/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,17 +1,20 @@
 Metadata-Version: 2.1
 Name: fastexception
-Version: 0.1.3
+Version: 0.1.4
 Home-page: https://github.com/mojtabapaso/fastexception
 Author: Mojtaba
 Author-email: mojtabapaso@gamil.com
 License: MIT
 Keywords: FastAPI Tools Fast Exception
+Classifier: Programming Language :: Python :: 3
+Classifier: License :: OSI Approved :: MIT License
+Classifier: Operating System :: OS Independent
 Description-Content-Type: text/markdown
-License-File: LICENSE.txt
+License-File: LICENSE
 
 fast exception
 ===================
 This package is a plugin for easier handling of Exception and sending HTTP status code.
 
 Installing
 ============
```

