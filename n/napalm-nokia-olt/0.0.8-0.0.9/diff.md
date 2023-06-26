# Comparing `tmp/napalm_nokia_olt-0.0.8.tar.gz` & `tmp/napalm_nokia_olt-0.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "/Users/nahanga/Desktop/NOKIA/napalm_nokia_olt/dist/.tmp-psyrtioo/napalm_nokia_olt-0.0.8.tar", last modified: Mon Jun 26 13:04:46 2023, max compression
+gzip compressed data, was "/Users/nahanga/Desktop/NOKIA/napalm_nokia_olt/dist/.tmp-lmupyogh/napalm_nokia_olt-0.0.9.tar", last modified: Mon Jun 26 13:55:29 2023, max compression
```

## Comparing `napalm_nokia_olt-0.0.8.tar` & `napalm_nokia_olt-0.0.9.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxr-xr-x   0 nahanga    (501) staff       (20)        0 2023-06-26 13:04:46.668252 napalm_nokia_olt-0.0.8/
--rw-r--r--   0 nahanga    (501) staff       (20)    11324 2022-08-16 08:37:40.000000 napalm_nokia_olt-0.0.8/LICENSE.md
--rw-r--r--   0 nahanga    (501) staff       (20)      687 2023-06-26 13:04:46.668446 napalm_nokia_olt-0.0.8/PKG-INFO
--rw-r--r--   0 nahanga    (501) staff       (20)      167 2023-02-10 17:17:02.000000 napalm_nokia_olt-0.0.8/README.md
-drwxr-xr-x   0 nahanga    (501) staff       (20)        0 2023-06-26 13:04:46.654223 napalm_nokia_olt-0.0.8/napalm_nokia_olt/
--rw-r--r--   0 nahanga    (501) staff       (20)      115 2023-02-10 17:39:46.000000 napalm_nokia_olt-0.0.8/napalm_nokia_olt/__init__.py
--rw-r--r--   0 nahanga    (501) staff       (20)     5596 2023-06-26 13:02:53.000000 napalm_nokia_olt-0.0.8/napalm_nokia_olt/nokia_olt.py
-drwxr-xr-x   0 nahanga    (501) staff       (20)        0 2023-06-26 13:04:46.667874 napalm_nokia_olt-0.0.8/napalm_nokia_olt.egg-info/
--rw-r--r--   0 nahanga    (501) staff       (20)      687 2023-06-26 13:04:46.000000 napalm_nokia_olt-0.0.8/napalm_nokia_olt.egg-info/PKG-INFO
--rw-r--r--   0 nahanga    (501) staff       (20)      297 2023-06-26 13:04:46.000000 napalm_nokia_olt-0.0.8/napalm_nokia_olt.egg-info/SOURCES.txt
--rw-r--r--   0 nahanga    (501) staff       (20)        1 2023-06-26 13:04:46.000000 napalm_nokia_olt-0.0.8/napalm_nokia_olt.egg-info/dependency_links.txt
--rw-r--r--   0 nahanga    (501) staff       (20)       10 2023-06-26 13:04:46.000000 napalm_nokia_olt-0.0.8/napalm_nokia_olt.egg-info/requires.txt
--rw-r--r--   0 nahanga    (501) staff       (20)       17 2023-06-26 13:04:46.000000 napalm_nokia_olt-0.0.8/napalm_nokia_olt.egg-info/top_level.txt
--rw-r--r--   0 nahanga    (501) staff       (20)       38 2023-06-26 13:04:46.669395 napalm_nokia_olt-0.0.8/setup.cfg
--rw-r--r--   0 nahanga    (501) staff       (20)      927 2023-06-26 13:03:03.000000 napalm_nokia_olt-0.0.8/setup.py
+drwxr-xr-x   0 nahanga    (501) staff       (20)        0 2023-06-26 13:55:29.129327 napalm_nokia_olt-0.0.9/
+-rw-r--r--   0 nahanga    (501) staff       (20)    11324 2022-08-16 08:37:40.000000 napalm_nokia_olt-0.0.9/LICENSE.md
+-rw-r--r--   0 nahanga    (501) staff       (20)      687 2023-06-26 13:55:29.129487 napalm_nokia_olt-0.0.9/PKG-INFO
+-rw-r--r--   0 nahanga    (501) staff       (20)      167 2023-02-10 17:17:02.000000 napalm_nokia_olt-0.0.9/README.md
+drwxr-xr-x   0 nahanga    (501) staff       (20)        0 2023-06-26 13:55:29.107558 napalm_nokia_olt-0.0.9/napalm_nokia_olt/
+-rw-r--r--   0 nahanga    (501) staff       (20)      115 2023-02-10 17:39:46.000000 napalm_nokia_olt-0.0.9/napalm_nokia_olt/__init__.py
+-rw-r--r--   0 nahanga    (501) staff       (20)     9686 2023-06-26 13:54:50.000000 napalm_nokia_olt-0.0.9/napalm_nokia_olt/nokia_olt.py
+drwxr-xr-x   0 nahanga    (501) staff       (20)        0 2023-06-26 13:55:29.128942 napalm_nokia_olt-0.0.9/napalm_nokia_olt.egg-info/
+-rw-r--r--   0 nahanga    (501) staff       (20)      687 2023-06-26 13:55:29.000000 napalm_nokia_olt-0.0.9/napalm_nokia_olt.egg-info/PKG-INFO
+-rw-r--r--   0 nahanga    (501) staff       (20)      297 2023-06-26 13:55:29.000000 napalm_nokia_olt-0.0.9/napalm_nokia_olt.egg-info/SOURCES.txt
+-rw-r--r--   0 nahanga    (501) staff       (20)        1 2023-06-26 13:55:29.000000 napalm_nokia_olt-0.0.9/napalm_nokia_olt.egg-info/dependency_links.txt
+-rw-r--r--   0 nahanga    (501) staff       (20)       10 2023-06-26 13:55:29.000000 napalm_nokia_olt-0.0.9/napalm_nokia_olt.egg-info/requires.txt
+-rw-r--r--   0 nahanga    (501) staff       (20)       17 2023-06-26 13:55:29.000000 napalm_nokia_olt-0.0.9/napalm_nokia_olt.egg-info/top_level.txt
+-rw-r--r--   0 nahanga    (501) staff       (20)       38 2023-06-26 13:55:29.130809 napalm_nokia_olt-0.0.9/setup.cfg
+-rw-r--r--   0 nahanga    (501) staff       (20)      927 2023-06-26 13:55:00.000000 napalm_nokia_olt-0.0.9/setup.py
```

### Comparing `napalm_nokia_olt-0.0.8/LICENSE.md` & `napalm_nokia_olt-0.0.9/LICENSE.md`

 * *Files identical despite different names*

### Comparing `napalm_nokia_olt-0.0.8/PKG-INFO` & `napalm_nokia_olt-0.0.9/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: napalm_nokia_olt
-Version: 0.0.8
+Version: 0.0.9
 Summary: Network Automation and Programmability Abstraction Layer driver for NOKIA OLT 
 Home-page: https://github.com/davama/napalm-nokia_olt
 Author: Dave Macias
 Author-email: davama@gmail.com
 Keywords: napalm driver
 Classifier: Topic :: Utilities
 Classifier: Programming Language :: Python :: 3
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: napalm_nokia_olt Version: 0.0.8 Summary: Network
+Metadata-Version: 2.1 Name: napalm_nokia_olt Version: 0.0.9 Summary: Network
 Automation and Programmability Abstraction Layer driver for NOKIA OLT Home-
 page: https://github.com/davama/napalm-nokia_olt Author: Dave Macias Author-
 email: davama@gmail.com Keywords: napalm driver Classifier: Topic :: Utilities
 Classifier: Programming Language :: Python :: 3 Classifier: Operating System ::
 OS Independent Classifier: License :: OSI Approved :: BSD License Description-
 Content-Type: text/markdown License-File: LICENSE.md
 ***** napalm-nokia_olt *****
```

### Comparing `napalm_nokia_olt-0.0.8/napalm_nokia_olt.egg-info/PKG-INFO` & `napalm_nokia_olt-0.0.9/napalm_nokia_olt.egg-info/PKG-INFO`

 * *Files 23% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: napalm-nokia-olt
-Version: 0.0.8
+Version: 0.0.9
 Summary: Network Automation and Programmability Abstraction Layer driver for NOKIA OLT 
 Home-page: https://github.com/davama/napalm-nokia_olt
 Author: Dave Macias
 Author-email: davama@gmail.com
 Keywords: napalm driver
 Classifier: Topic :: Utilities
 Classifier: Programming Language :: Python :: 3
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: napalm-nokia-olt Version: 0.0.8 Summary: Network
+Metadata-Version: 2.1 Name: napalm-nokia-olt Version: 0.0.9 Summary: Network
 Automation and Programmability Abstraction Layer driver for NOKIA OLT Home-
 page: https://github.com/davama/napalm-nokia_olt Author: Dave Macias Author-
 email: davama@gmail.com Keywords: napalm driver Classifier: Topic :: Utilities
 Classifier: Programming Language :: Python :: 3 Classifier: Operating System ::
 OS Independent Classifier: License :: OSI Approved :: BSD License Description-
 Content-Type: text/markdown License-File: LICENSE.md
 ***** napalm-nokia_olt *****
```

### Comparing `napalm_nokia_olt-0.0.8/setup.py` & `napalm_nokia_olt-0.0.9/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 
 # read the contents of your README file
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="napalm_nokia_olt",
-    version="0.0.8",
+    version="0.0.9",
     author="Dave Macias",
     author_email = "davama@gmail.com",
     description=("Network Automation and Programmability Abstraction "
                  "Layer driver for NOKIA OLT "),
     keywords="napalm driver",
     url = "https://github.com/davama/napalm-nokia_olt",
     packages=find_packages(),
```

