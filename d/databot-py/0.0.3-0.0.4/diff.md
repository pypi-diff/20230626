# Comparing `tmp/databot-py-0.0.3.tar.gz` & `tmp/databot-py-0.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "databot-py-0.0.3.tar", last modified: Fri Jun 23 18:52:45 2023, max compression
+gzip compressed data, was "databot-py-0.0.4.tar", last modified: Mon Jun 26 20:22:36 2023, max compression
```

## Comparing `databot-py-0.0.3.tar` & `databot-py-0.0.4.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxrwxrwx   0        0        0        0 2023-06-23 18:52:45.877489 databot-py-0.0.3/
--rw-rw-rw-   0        0        0     1092 2023-02-14 16:33:12.000000 databot-py-0.0.3/LICENSE
--rw-rw-rw-   0        0        0     2249 2023-06-23 18:52:45.875479 databot-py-0.0.3/PKG-INFO
--rw-rw-rw-   0        0        0     1937 2023-06-23 18:24:34.000000 databot-py-0.0.3/README.md
-drwxrwxrwx   0        0        0        0 2023-06-23 18:52:45.852479 databot-py-0.0.3/databot/
--rw-rw-rw-   0        0        0    10969 2023-06-23 18:24:34.000000 databot-py-0.0.3/databot/PyDatabot.py
--rw-rw-rw-   0        0        0        0 2023-06-18 13:23:36.000000 databot-py-0.0.3/databot/__init__.py
-drwxrwxrwx   0        0        0        0 2023-06-23 18:52:45.873479 databot-py-0.0.3/databot_py.egg-info/
--rw-rw-rw-   0        0        0     2249 2023-06-23 18:52:45.000000 databot-py-0.0.3/databot_py.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      251 2023-06-23 18:52:45.000000 databot-py-0.0.3/databot_py.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-23 18:52:45.000000 databot-py-0.0.3/databot_py.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       14 2023-06-23 18:52:45.000000 databot-py-0.0.3/databot_py.egg-info/requires.txt
--rw-rw-rw-   0        0        0        8 2023-06-23 18:52:45.000000 databot-py-0.0.3/databot_py.egg-info/top_level.txt
--rw-rw-rw-   0        0        0      108 2023-06-23 18:24:07.000000 databot-py-0.0.3/pyproject.toml
--rw-rw-rw-   0        0        0       42 2023-06-23 18:52:45.879483 databot-py-0.0.3/setup.cfg
--rw-rw-rw-   0        0        0      765 2023-06-23 18:51:59.000000 databot-py-0.0.3/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-26 20:22:36.604505 databot-py-0.0.4/
+-rw-rw-rw-   0        0        0     1092 2023-02-14 16:33:12.000000 databot-py-0.0.4/LICENSE
+-rw-rw-rw-   0        0        0     2249 2023-06-26 20:22:36.603502 databot-py-0.0.4/PKG-INFO
+-rw-rw-rw-   0        0        0     1937 2023-06-23 18:24:34.000000 databot-py-0.0.4/README.md
+drwxrwxrwx   0        0        0        0 2023-06-26 20:22:36.572505 databot-py-0.0.4/databot/
+-rw-rw-rw-   0        0        0    10969 2023-06-23 18:24:34.000000 databot-py-0.0.4/databot/PyDatabot.py
+-rw-rw-rw-   0        0        0        0 2023-06-18 13:23:36.000000 databot-py-0.0.4/databot/__init__.py
+drwxrwxrwx   0        0        0        0 2023-06-26 20:22:36.601504 databot-py-0.0.4/databot_py.egg-info/
+-rw-rw-rw-   0        0        0     2249 2023-06-26 20:22:36.000000 databot-py-0.0.4/databot_py.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      251 2023-06-26 20:22:36.000000 databot-py-0.0.4/databot_py.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-26 20:22:36.000000 databot-py-0.0.4/databot_py.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       14 2023-06-26 20:22:36.000000 databot-py-0.0.4/databot_py.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        8 2023-06-26 20:22:36.000000 databot-py-0.0.4/databot_py.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0      108 2023-06-23 18:24:07.000000 databot-py-0.0.4/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2023-06-26 20:22:36.604505 databot-py-0.0.4/setup.cfg
+-rw-rw-rw-   0        0        0      765 2023-06-26 20:21:42.000000 databot-py-0.0.4/setup.py
```

### Comparing `databot-py-0.0.3/LICENSE` & `databot-py-0.0.4/LICENSE`

 * *Files identical despite different names*

### Comparing `databot-py-0.0.3/PKG-INFO` & `databot-py-0.0.4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: databot-py
-Version: 0.0.3
+Version: 0.0.4
 Summary: databot Python Library
 Home-page: https://github.com/dbaldwin/databot-py
 Author: Pat Ryan, Dennis Baldwin
 Author-email: theyoungsoul@gmail.com, db@droneblocks.io
 License: MIT
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

### Comparing `databot-py-0.0.3/README.md` & `databot-py-0.0.4/README.md`

 * *Files identical despite different names*

### Comparing `databot-py-0.0.3/databot/PyDatabot.py` & `databot-py-0.0.4/databot/PyDatabot.py`

 * *Files identical despite different names*

### Comparing `databot-py-0.0.3/databot_py.egg-info/PKG-INFO` & `databot-py-0.0.4/databot_py.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: databot-py
-Version: 0.0.3
+Version: 0.0.4
 Summary: databot Python Library
 Home-page: https://github.com/dbaldwin/databot-py
 Author: Pat Ryan, Dennis Baldwin
 Author-email: theyoungsoul@gmail.com, db@droneblocks.io
 License: MIT
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

### Comparing `databot-py-0.0.3/setup.py` & `databot-py-0.0.4/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 from glob import glob
 
 with open("README.md", "r", encoding="utf-8") as fh:
     long_description = fh.read()
 
 setup(
     name='databot-py',
-    version='0.0.3',
+    version='0.0.4',
     packages=['databot'],
     include_package_data=True,
     package_data={
         'media': glob('media/*'),
         'data': glob('data/*'),
         'web': glob('web/*')
     },
@@ -18,10 +18,10 @@
     license='MIT',
     author='Pat Ryan, Dennis Baldwin',
     author_email='theyoungsoul@gmail.com, db@droneblocks.io',
     description='databot Python Library',
     long_description=long_description,
     long_description_content_type="text/markdown",
     install_requires=[
-        'bleak==0.19.1'
+        'bleak==0.19.5'
     ]
 )
```

