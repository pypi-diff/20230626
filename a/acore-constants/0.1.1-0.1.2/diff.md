# Comparing `tmp/acore_constants-0.1.1.tar.gz` & `tmp/acore_constants-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "acore_constants-0.1.1.tar", last modified: Mon Jun 26 05:07:14 2023, max compression
+gzip compressed data, was "acore_constants-0.1.2.tar", last modified: Mon Jun 26 05:45:26 2023, max compression
```

## Comparing `acore_constants-0.1.1.tar` & `acore_constants-0.1.2.tar`

### file list

```diff
@@ -1,30 +1,30 @@
-drwxr-xr-x   0 sanhehu    (501) staff       (20)        0 2023-06-26 05:07:14.326328 acore_constants-0.1.1/
--rw-r--r--   0 sanhehu    (501) staff       (20)      670 2023-06-26 04:53:26.000000 acore_constants-0.1.1/AUTHORS.rst
--rw-r--r--   0 sanhehu    (501) staff       (20)     1126 2023-06-26 04:53:26.000000 acore_constants-0.1.1/LICENSE.txt
--rw-r--r--   0 sanhehu    (501) staff       (20)      323 2023-06-26 04:53:26.000000 acore_constants-0.1.1/MANIFEST.in
--rw-r--r--   0 sanhehu    (501) staff       (20)     4224 2023-06-26 05:07:14.326177 acore_constants-0.1.1/PKG-INFO
--rw-r--r--   0 sanhehu    (501) staff       (20)     3081 2023-06-26 05:06:56.000000 acore_constants-0.1.1/README.rst
-drwxr-xr-x   0 sanhehu    (501) staff       (20)        0 2023-06-26 05:07:14.324944 acore_constants-0.1.1/acore_constants/
--rw-r--r--   0 sanhehu    (501) staff       (20)      415 2023-06-26 05:06:03.000000 acore_constants-0.1.1/acore_constants/__init__.py
--rw-r--r--   0 sanhehu    (501) staff       (20)       93 2023-06-26 04:53:26.000000 acore_constants-0.1.1/acore_constants/_version.py
--rw-r--r--   0 sanhehu    (501) staff       (20)       56 2023-06-26 05:01:13.000000 acore_constants-0.1.1/acore_constants/api.py
--rw-r--r--   0 sanhehu    (501) staff       (20)      800 2023-06-26 05:01:01.000000 acore_constants-0.1.1/acore_constants/constants.py
-drwxr-xr-x   0 sanhehu    (501) staff       (20)        0 2023-06-26 05:07:14.325767 acore_constants-0.1.1/acore_constants/docs/
--rw-r--r--   0 sanhehu    (501) staff       (20)        0 2023-06-26 04:57:16.000000 acore_constants-0.1.1/acore_constants/docs/__init__.py
--rw-r--r--   0 sanhehu    (501) staff       (20)      642 2023-06-26 04:53:26.000000 acore_constants-0.1.1/acore_constants/paths.py
-drwxr-xr-x   0 sanhehu    (501) staff       (20)        0 2023-06-26 05:07:14.325644 acore_constants-0.1.1/acore_constants.egg-info/
--rw-r--r--   0 sanhehu    (501) staff       (20)     4224 2023-06-26 05:07:14.000000 acore_constants-0.1.1/acore_constants.egg-info/PKG-INFO
--rw-r--r--   0 sanhehu    (501) staff       (20)      562 2023-06-26 05:07:14.000000 acore_constants-0.1.1/acore_constants.egg-info/SOURCES.txt
--rw-r--r--   0 sanhehu    (501) staff       (20)        1 2023-06-26 05:07:14.000000 acore_constants-0.1.1/acore_constants.egg-info/dependency_links.txt
--rw-r--r--   0 sanhehu    (501) staff       (20)      139 2023-06-26 05:07:14.000000 acore_constants-0.1.1/acore_constants.egg-info/requires.txt
--rw-r--r--   0 sanhehu    (501) staff       (20)       16 2023-06-26 05:07:14.000000 acore_constants-0.1.1/acore_constants.egg-info/top_level.txt
--rw-r--r--   0 sanhehu    (501) staff       (20)      743 2023-06-26 05:04:56.000000 acore_constants-0.1.1/release-history.rst
--rw-r--r--   0 sanhehu    (501) staff       (20)      102 2023-06-26 04:53:26.000000 acore_constants-0.1.1/requirements-automation.txt
--rw-r--r--   0 sanhehu    (501) staff       (20)      353 2023-06-26 04:53:26.000000 acore_constants-0.1.1/requirements-dev.txt
--rw-r--r--   0 sanhehu    (501) staff       (20)      563 2023-06-26 04:53:26.000000 acore_constants-0.1.1/requirements-doc.txt
--rw-r--r--   0 sanhehu    (501) staff       (20)      183 2023-06-26 04:53:26.000000 acore_constants-0.1.1/requirements-test.txt
--rw-r--r--   0 sanhehu    (501) staff       (20)       30 2023-06-26 04:53:26.000000 acore_constants-0.1.1/requirements.txt
--rw-r--r--   0 sanhehu    (501) staff       (20)       38 2023-06-26 05:07:14.326374 acore_constants-0.1.1/setup.cfg
--rw-r--r--   0 sanhehu    (501) staff       (20)     7564 2023-06-26 04:53:26.000000 acore_constants-0.1.1/setup.py
-drwxr-xr-x   0 sanhehu    (501) staff       (20)        0 2023-06-26 05:07:14.325868 acore_constants-0.1.1/tests/
--rw-r--r--   0 sanhehu    (501) staff       (20)      357 2023-06-26 05:01:33.000000 acore_constants-0.1.1/tests/test_api.py
+drwxr-xr-x   0 sanhehu    (501) staff       (20)        0 2023-06-26 05:45:26.474619 acore_constants-0.1.2/
+-rw-r--r--   0 sanhehu    (501) staff       (20)      670 2023-06-26 04:53:26.000000 acore_constants-0.1.2/AUTHORS.rst
+-rw-r--r--   0 sanhehu    (501) staff       (20)     1126 2023-06-26 04:53:26.000000 acore_constants-0.1.2/LICENSE.txt
+-rw-r--r--   0 sanhehu    (501) staff       (20)      323 2023-06-26 04:53:26.000000 acore_constants-0.1.2/MANIFEST.in
+-rw-r--r--   0 sanhehu    (501) staff       (20)     4224 2023-06-26 05:45:26.474492 acore_constants-0.1.2/PKG-INFO
+-rw-r--r--   0 sanhehu    (501) staff       (20)     3081 2023-06-26 05:06:56.000000 acore_constants-0.1.2/README.rst
+drwxr-xr-x   0 sanhehu    (501) staff       (20)        0 2023-06-26 05:45:26.473564 acore_constants-0.1.2/acore_constants/
+-rw-r--r--   0 sanhehu    (501) staff       (20)      415 2023-06-26 05:06:03.000000 acore_constants-0.1.2/acore_constants/__init__.py
+-rw-r--r--   0 sanhehu    (501) staff       (20)       93 2023-06-26 05:43:21.000000 acore_constants-0.1.2/acore_constants/_version.py
+-rw-r--r--   0 sanhehu    (501) staff       (20)       56 2023-06-26 05:01:13.000000 acore_constants-0.1.2/acore_constants/api.py
+-rw-r--r--   0 sanhehu    (501) staff       (20)      784 2023-06-26 05:43:06.000000 acore_constants-0.1.2/acore_constants/constants.py
+drwxr-xr-x   0 sanhehu    (501) staff       (20)        0 2023-06-26 05:45:26.474250 acore_constants-0.1.2/acore_constants/docs/
+-rw-r--r--   0 sanhehu    (501) staff       (20)        0 2023-06-26 04:57:16.000000 acore_constants-0.1.2/acore_constants/docs/__init__.py
+-rw-r--r--   0 sanhehu    (501) staff       (20)      642 2023-06-26 04:53:26.000000 acore_constants-0.1.2/acore_constants/paths.py
+drwxr-xr-x   0 sanhehu    (501) staff       (20)        0 2023-06-26 05:45:26.474144 acore_constants-0.1.2/acore_constants.egg-info/
+-rw-r--r--   0 sanhehu    (501) staff       (20)     4224 2023-06-26 05:45:26.000000 acore_constants-0.1.2/acore_constants.egg-info/PKG-INFO
+-rw-r--r--   0 sanhehu    (501) staff       (20)      562 2023-06-26 05:45:26.000000 acore_constants-0.1.2/acore_constants.egg-info/SOURCES.txt
+-rw-r--r--   0 sanhehu    (501) staff       (20)        1 2023-06-26 05:45:26.000000 acore_constants-0.1.2/acore_constants.egg-info/dependency_links.txt
+-rw-r--r--   0 sanhehu    (501) staff       (20)      139 2023-06-26 05:45:26.000000 acore_constants-0.1.2/acore_constants.egg-info/requires.txt
+-rw-r--r--   0 sanhehu    (501) staff       (20)       16 2023-06-26 05:45:26.000000 acore_constants-0.1.2/acore_constants.egg-info/top_level.txt
+-rw-r--r--   0 sanhehu    (501) staff       (20)      983 2023-06-26 05:44:16.000000 acore_constants-0.1.2/release-history.rst
+-rw-r--r--   0 sanhehu    (501) staff       (20)      102 2023-06-26 04:53:26.000000 acore_constants-0.1.2/requirements-automation.txt
+-rw-r--r--   0 sanhehu    (501) staff       (20)      353 2023-06-26 04:53:26.000000 acore_constants-0.1.2/requirements-dev.txt
+-rw-r--r--   0 sanhehu    (501) staff       (20)      563 2023-06-26 04:53:26.000000 acore_constants-0.1.2/requirements-doc.txt
+-rw-r--r--   0 sanhehu    (501) staff       (20)      183 2023-06-26 04:53:26.000000 acore_constants-0.1.2/requirements-test.txt
+-rw-r--r--   0 sanhehu    (501) staff       (20)       30 2023-06-26 04:53:26.000000 acore_constants-0.1.2/requirements.txt
+-rw-r--r--   0 sanhehu    (501) staff       (20)       38 2023-06-26 05:45:26.474670 acore_constants-0.1.2/setup.cfg
+-rw-r--r--   0 sanhehu    (501) staff       (20)     7564 2023-06-26 04:53:26.000000 acore_constants-0.1.2/setup.py
+drwxr-xr-x   0 sanhehu    (501) staff       (20)        0 2023-06-26 05:45:26.474349 acore_constants-0.1.2/tests/
+-rw-r--r--   0 sanhehu    (501) staff       (20)      341 2023-06-26 05:43:15.000000 acore_constants-0.1.2/tests/test_api.py
```

### Comparing `acore_constants-0.1.1/AUTHORS.rst` & `acore_constants-0.1.2/AUTHORS.rst`

 * *Files identical despite different names*

### Comparing `acore_constants-0.1.1/LICENSE.txt` & `acore_constants-0.1.2/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `acore_constants-0.1.1/PKG-INFO` & `acore_constants-0.1.2/acore_constants.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 Metadata-Version: 2.1
-Name: acore_constants
-Version: 0.1.1
+Name: acore-constants
+Version: 0.1.2
 Summary: AzerothCore World of Warcraft server project constants variables.
 Home-page: https://github.com/MacHu-GWU/acore_constants-project
-Download-URL: https://pypi.python.org/pypi/acore_constants/0.1.1#downloads
+Download-URL: https://pypi.python.org/pypi/acore_constants/0.1.2#downloads
 Author: Sanhe Hu
 Author-email: husanhe@gmail.com
 Maintainer: Sanhe Hu
 Maintainer-email: husanhe@gmail.com
 License: MIT
 Platform: Windows
 Platform: MacOS
```

### Comparing `acore_constants-0.1.1/README.rst` & `acore_constants-0.1.2/README.rst`

 * *Files identical despite different names*

### Comparing `acore_constants-0.1.1/acore_constants/constants.py` & `acore_constants-0.1.2/acore_constants/constants.py`

 * *Files 20% similar despite different names*

```diff
@@ -10,9 +10,9 @@
         "stopped", 如果在线, 则显示 "N players" 其中 N 是一个整数. 注意这个 value
         的格式也很重要, 他会被其他项目的代码解析.
     :param WOW_STATUS_MEASURE_TIME: 这个 tag 用来记录 WOW_STATUS 的测量时间. 值为
         ISO 格式的 datetime.
     """
 
     SERVER_ID = "wserver:server_id"
-    WOW_STATUS_MEASURE_TIME_TAG_KEY = "wserver:wow_status_measure_time"
-    WOW_STATUS_TAG_KEY = "wserver:wow_status"
+    WOW_STATUS = "wserver:wow_status"
+    WOW_STATUS_MEASURE_TIME = "wserver:wow_status_measure_time"
```

### Comparing `acore_constants-0.1.1/acore_constants/paths.py` & `acore_constants-0.1.2/acore_constants/paths.py`

 * *Files identical despite different names*

### Comparing `acore_constants-0.1.1/acore_constants.egg-info/PKG-INFO` & `acore_constants-0.1.2/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 Metadata-Version: 2.1
-Name: acore-constants
-Version: 0.1.1
+Name: acore_constants
+Version: 0.1.2
 Summary: AzerothCore World of Warcraft server project constants variables.
 Home-page: https://github.com/MacHu-GWU/acore_constants-project
-Download-URL: https://pypi.python.org/pypi/acore_constants/0.1.1#downloads
+Download-URL: https://pypi.python.org/pypi/acore_constants/0.1.2#downloads
 Author: Sanhe Hu
 Author-email: husanhe@gmail.com
 Maintainer: Sanhe Hu
 Maintainer-email: husanhe@gmail.com
 License: MIT
 Platform: Windows
 Platform: MacOS
```

### Comparing `acore_constants-0.1.1/acore_constants.egg-info/SOURCES.txt` & `acore_constants-0.1.2/acore_constants.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `acore_constants-0.1.1/release-history.rst` & `acore_constants-0.1.2/release-history.rst`

 * *Files 17% similar despite different names*

```diff
@@ -11,14 +11,22 @@
 **Minor Improvements**
 
 **Bugfixes**
 
 **Miscellaneous**
 
 
+0.1.2 (2023-06-26)
+~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~
+**Bugfixes**
+
+- rename ``WOW_STATUS_TAG_KEY`` to ``WOW_STATUS``
+- rename ``WOW_STATUS_MEASURE_TIME_TAG_KEY`` to ``WOW_STATUS_MEASURE_TIME``
+
+
 0.1.1 (2023-06-26)
 ~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~
 **Features and Improvements**
 
 - First release
 - Add the following constant:
     - ``acore_constants.api.TagKey.SERVER_ID = "wserver:server_id"``
```

### Comparing `acore_constants-0.1.1/requirements-doc.txt` & `acore_constants-0.1.2/requirements-doc.txt`

 * *Files identical despite different names*

### Comparing `acore_constants-0.1.1/setup.py` & `acore_constants-0.1.2/setup.py`

 * *Files identical despite different names*

