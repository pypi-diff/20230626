# Comparing `tmp/dcentrapi-0.2.5.tar.gz` & `tmp/dcentrapi-0.2.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dcentrapi-0.2.5.tar", last modified: Mon Jun  5 07:36:54 2023, max compression
+gzip compressed data, was "dcentrapi-0.2.6.tar", last modified: Mon Jun 26 07:56:13 2023, max compression
```

## Comparing `dcentrapi-0.2.5.tar` & `dcentrapi-0.2.6.tar`

### file list

```diff
@@ -1,21 +1,23 @@
-drwxr-xr-x   0 nivshitrit   (501) staff       (20)        0 2023-06-05 07:36:54.163551 dcentrapi-0.2.5/
--rw-r--r--   0 nivshitrit   (501) staff       (20)     1073 2022-10-09 08:58:27.000000 dcentrapi-0.2.5/LICENSE.rst
--rw-r--r--   0 nivshitrit   (501) staff       (20)     6780 2023-06-05 07:36:54.163414 dcentrapi-0.2.5/PKG-INFO
--rw-r--r--   0 nivshitrit   (501) staff       (20)     6211 2022-10-09 08:58:27.000000 dcentrapi-0.2.5/README.md
-drwxr-xr-x   0 nivshitrit   (501) staff       (20)        0 2023-06-05 07:36:54.162538 dcentrapi-0.2.5/dcentrapi/
--rw-r--r--   0 nivshitrit   (501) staff       (20)      829 2023-05-24 09:45:16.000000 dcentrapi-0.2.5/dcentrapi/Base.py
--rw-r--r--   0 nivshitrit   (501) staff       (20)      280 2023-03-08 10:39:09.000000 dcentrapi-0.2.5/dcentrapi/__init__.py
--rw-r--r--   0 nivshitrit   (501) staff       (20)       63 2023-06-05 07:36:32.000000 dcentrapi-0.2.5/dcentrapi/common.py
--rw-r--r--   0 nivshitrit   (501) staff       (20)     8714 2023-06-05 07:36:17.000000 dcentrapi-0.2.5/dcentrapi/eventPolling.py
--rw-r--r--   0 nivshitrit   (501) staff       (20)      491 2023-03-02 14:02:13.000000 dcentrapi-0.2.5/dcentrapi/gasMonitor.py
--rw-r--r--   0 nivshitrit   (501) staff       (20)     3078 2022-11-22 15:13:50.000000 dcentrapi-0.2.5/dcentrapi/merkleTree.py
--rw-r--r--   0 nivshitrit   (501) staff       (20)     3059 2023-06-05 07:36:17.000000 dcentrapi-0.2.5/dcentrapi/rpcAggregation.py
--rw-r--r--   0 nivshitrit   (501) staff       (20)      804 2023-05-31 13:35:59.000000 dcentrapi-0.2.5/dcentrapi/web3Index.py
-drwxr-xr-x   0 nivshitrit   (501) staff       (20)        0 2023-06-05 07:36:54.163254 dcentrapi-0.2.5/dcentrapi.egg-info/
--rw-r--r--   0 nivshitrit   (501) staff       (20)     6780 2023-06-05 07:36:54.000000 dcentrapi-0.2.5/dcentrapi.egg-info/PKG-INFO
--rw-r--r--   0 nivshitrit   (501) staff       (20)      379 2023-06-05 07:36:54.000000 dcentrapi-0.2.5/dcentrapi.egg-info/SOURCES.txt
--rw-r--r--   0 nivshitrit   (501) staff       (20)        1 2023-06-05 07:36:54.000000 dcentrapi-0.2.5/dcentrapi.egg-info/dependency_links.txt
--rw-r--r--   0 nivshitrit   (501) staff       (20)        9 2023-06-05 07:36:54.000000 dcentrapi-0.2.5/dcentrapi.egg-info/requires.txt
--rw-r--r--   0 nivshitrit   (501) staff       (20)       10 2023-06-05 07:36:54.000000 dcentrapi-0.2.5/dcentrapi.egg-info/top_level.txt
--rw-r--r--   0 nivshitrit   (501) staff       (20)       38 2023-06-05 07:36:54.163613 dcentrapi-0.2.5/setup.cfg
--rw-r--r--   0 nivshitrit   (501) staff       (20)     1167 2023-04-09 07:57:53.000000 dcentrapi-0.2.5/setup.py
+drwxr-xr-x   0 oded       (502) staff       (20)        0 2023-06-26 07:56:13.505123 dcentrapi-0.2.6/
+-rw-r--r--   0 oded       (502) staff       (20)     1073 2022-09-29 14:45:59.000000 dcentrapi-0.2.6/LICENSE.rst
+-rw-r--r--   0 oded       (502) staff       (20)     6741 2023-06-26 07:56:13.504991 dcentrapi-0.2.6/PKG-INFO
+-rw-r--r--   0 oded       (502) staff       (20)     6211 2022-09-29 14:45:59.000000 dcentrapi-0.2.6/README.md
+drwxr-xr-x   0 oded       (502) staff       (20)        0 2023-06-26 07:56:13.504110 dcentrapi-0.2.6/dcentrapi/
+-rw-r--r--   0 oded       (502) staff       (20)      829 2023-06-26 05:46:25.000000 dcentrapi-0.2.6/dcentrapi/Base.py
+-rw-r--r--   0 oded       (502) staff       (20)      280 2023-06-26 05:46:25.000000 dcentrapi-0.2.6/dcentrapi/__init__.py
+-rw-r--r--   0 oded       (502) staff       (20)      195 2023-06-26 06:53:05.000000 dcentrapi-0.2.6/dcentrapi/common.py
+-rw-r--r--   0 oded       (502) staff       (20)     8714 2023-06-26 05:46:25.000000 dcentrapi-0.2.6/dcentrapi/eventPolling.py
+-rw-r--r--   0 oded       (502) staff       (20)      491 2023-06-26 05:46:25.000000 dcentrapi-0.2.6/dcentrapi/gasMonitor.py
+-rw-r--r--   0 oded       (502) staff       (20)      527 2023-06-26 06:53:05.000000 dcentrapi-0.2.6/dcentrapi/hackMitigation.py
+-rw-r--r--   0 oded       (502) staff       (20)     3078 2022-12-21 09:08:31.000000 dcentrapi-0.2.6/dcentrapi/merkleTree.py
+-rw-r--r--   0 oded       (502) staff       (20)     3059 2023-06-26 05:46:25.000000 dcentrapi-0.2.6/dcentrapi/rpcAggregation.py
+-rw-r--r--   0 oded       (502) staff       (20)      909 2022-11-10 13:20:43.000000 dcentrapi-0.2.6/dcentrapi/test.py
+-rw-r--r--   0 oded       (502) staff       (20)      804 2023-06-26 05:46:25.000000 dcentrapi-0.2.6/dcentrapi/web3Index.py
+drwxr-xr-x   0 oded       (502) staff       (20)        0 2023-06-26 07:56:13.504809 dcentrapi-0.2.6/dcentrapi.egg-info/
+-rw-r--r--   0 oded       (502) staff       (20)     6741 2023-06-26 07:56:13.000000 dcentrapi-0.2.6/dcentrapi.egg-info/PKG-INFO
+-rw-r--r--   0 oded       (502) staff       (20)      425 2023-06-26 07:56:13.000000 dcentrapi-0.2.6/dcentrapi.egg-info/SOURCES.txt
+-rw-r--r--   0 oded       (502) staff       (20)        1 2023-06-26 07:56:13.000000 dcentrapi-0.2.6/dcentrapi.egg-info/dependency_links.txt
+-rw-r--r--   0 oded       (502) staff       (20)        9 2023-06-26 07:56:13.000000 dcentrapi-0.2.6/dcentrapi.egg-info/requires.txt
+-rw-r--r--   0 oded       (502) staff       (20)       10 2023-06-26 07:56:13.000000 dcentrapi-0.2.6/dcentrapi.egg-info/top_level.txt
+-rw-r--r--   0 oded       (502) staff       (20)       38 2023-06-26 07:56:13.505161 dcentrapi-0.2.6/setup.cfg
+-rw-r--r--   0 oded       (502) staff       (20)     1167 2022-12-21 09:08:31.000000 dcentrapi-0.2.6/setup.py
```

### Comparing `dcentrapi-0.2.5/LICENSE.rst` & `dcentrapi-0.2.6/LICENSE.rst`

 * *Files identical despite different names*

### Comparing `dcentrapi-0.2.5/PKG-INFO` & `dcentrapi-0.2.6/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,17 +1,15 @@
 Metadata-Version: 2.1
 Name: dcentrapi
-Version: 0.2.5
+Version: 0.2.6
 Summary: Dcentralab Pypi packages
-Home-page: UNKNOWN
 Author: Dcentralab (Niv Shitrit)
 Author-email: <niv@dcentralab.com>
 License: MIT
 Keywords: python
-Platform: UNKNOWN
 Classifier: Development Status :: 1 - Planning
 Classifier: Intended Audience :: Developers
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: Unix
 Classifier: Operating System :: MacOS :: MacOS X
 Classifier: Operating System :: Microsoft :: Windows
 Description-Content-Type: text/markdown
@@ -105,9 +103,7 @@
 Show your appreciation to those who have contributed to the project.
 
 ## License
 For open source projects, say how it is licensed.
 
 ## Project status
 If you have run out of energy or time for your project, put a note at the top of the README saying that development has slowed down or stopped completely. Someone may choose to fork your project or volunteer to step in as a maintainer or owner, allowing your project to keep going. You can also make an explicit request for maintainers.
-
-
```

### Comparing `dcentrapi-0.2.5/README.md` & `dcentrapi-0.2.6/README.md`

 * *Files identical despite different names*

### Comparing `dcentrapi-0.2.5/dcentrapi/Base.py` & `dcentrapi-0.2.6/dcentrapi/Base.py`

 * *Files identical despite different names*

### Comparing `dcentrapi-0.2.5/dcentrapi/eventPolling.py` & `dcentrapi-0.2.6/dcentrapi/eventPolling.py`

 * *Files identical despite different names*

### Comparing `dcentrapi-0.2.5/dcentrapi/merkleTree.py` & `dcentrapi-0.2.6/dcentrapi/merkleTree.py`

 * *Files identical despite different names*

### Comparing `dcentrapi-0.2.5/dcentrapi/rpcAggregation.py` & `dcentrapi-0.2.6/dcentrapi/rpcAggregation.py`

 * *Files identical despite different names*

### Comparing `dcentrapi-0.2.5/dcentrapi/web3Index.py` & `dcentrapi-0.2.6/dcentrapi/web3Index.py`

 * *Files identical despite different names*

### Comparing `dcentrapi-0.2.5/dcentrapi.egg-info/PKG-INFO` & `dcentrapi-0.2.6/dcentrapi.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,17 +1,15 @@
 Metadata-Version: 2.1
 Name: dcentrapi
-Version: 0.2.5
+Version: 0.2.6
 Summary: Dcentralab Pypi packages
-Home-page: UNKNOWN
 Author: Dcentralab (Niv Shitrit)
 Author-email: <niv@dcentralab.com>
 License: MIT
 Keywords: python
-Platform: UNKNOWN
 Classifier: Development Status :: 1 - Planning
 Classifier: Intended Audience :: Developers
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: Unix
 Classifier: Operating System :: MacOS :: MacOS X
 Classifier: Operating System :: Microsoft :: Windows
 Description-Content-Type: text/markdown
@@ -105,9 +103,7 @@
 Show your appreciation to those who have contributed to the project.
 
 ## License
 For open source projects, say how it is licensed.
 
 ## Project status
 If you have run out of energy or time for your project, put a note at the top of the README saying that development has slowed down or stopped completely. Someone may choose to fork your project or volunteer to step in as a maintainer or owner, allowing your project to keep going. You can also make an explicit request for maintainers.
-
-
```

### Comparing `dcentrapi-0.2.5/setup.py` & `dcentrapi-0.2.6/setup.py`

 * *Files identical despite different names*

