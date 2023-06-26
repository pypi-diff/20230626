# Comparing `tmp/potato_tool-0.0.5.tar.gz` & `tmp/potato_tool-0.0.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "potato_tool-0.0.5.tar", last modified: Mon Jun 26 06:17:41 2023, max compression
+gzip compressed data, was "potato_tool-0.0.6.tar", last modified: Mon Jun 26 06:20:52 2023, max compression
```

## Comparing `potato_tool-0.0.5.tar` & `potato_tool-0.0.6.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxr-xr-x   0 a          (501) staff       (20)        0 2023-06-26 06:17:41.914114 potato_tool-0.0.5/
--rw-r--r--   0 a          (501) staff       (20)     3597 2023-06-26 06:17:41.913849 potato_tool-0.0.5/PKG-INFO
--rw-r--r--   0 a          (501) staff       (20)     3315 2023-06-26 05:51:28.000000 potato_tool-0.0.5/README.md
-drwxr-xr-x   0 a          (501) staff       (20)        0 2023-06-26 06:17:41.910849 potato_tool-0.0.5/potato_tool/
--rw-r--r--   0 a          (501) staff       (20)       30 2023-06-26 05:17:26.000000 potato_tool-0.0.5/potato_tool/__init__.py
--rwxr-xr-x   0 a          (501) staff       (20)    11209 2023-06-26 06:07:42.000000 potato_tool-0.0.5/potato_tool/font.py
-drwxr-xr-x   0 a          (501) staff       (20)        0 2023-06-26 06:17:41.913379 potato_tool-0.0.5/potato_tool.egg-info/
--rw-r--r--   0 a          (501) staff       (20)     3597 2023-06-26 06:17:41.000000 potato_tool-0.0.5/potato_tool.egg-info/PKG-INFO
--rw-r--r--   0 a          (501) staff       (20)      274 2023-06-26 06:17:41.000000 potato_tool-0.0.5/potato_tool.egg-info/SOURCES.txt
--rw-r--r--   0 a          (501) staff       (20)        1 2023-06-26 06:17:41.000000 potato_tool-0.0.5/potato_tool.egg-info/dependency_links.txt
--rw-r--r--   0 a          (501) staff       (20)     1026 2023-06-26 06:17:41.000000 potato_tool-0.0.5/potato_tool.egg-info/entry_points.txt
--rw-r--r--   0 a          (501) staff       (20)       25 2023-06-26 06:17:41.000000 potato_tool-0.0.5/potato_tool.egg-info/requires.txt
--rw-r--r--   0 a          (501) staff       (20)       12 2023-06-26 06:17:41.000000 potato_tool-0.0.5/potato_tool.egg-info/top_level.txt
--rw-r--r--   0 a          (501) staff       (20)       38 2023-06-26 06:17:41.914221 potato_tool-0.0.5/setup.cfg
--rw-r--r--   0 a          (501) staff       (20)     2164 2023-06-26 06:17:23.000000 potato_tool-0.0.5/setup.py
+drwxr-xr-x   0 a          (501) staff       (20)        0 2023-06-26 06:20:52.125267 potato_tool-0.0.6/
+-rw-r--r--   0 a          (501) staff       (20)     3597 2023-06-26 06:20:52.124999 potato_tool-0.0.6/PKG-INFO
+-rw-r--r--   0 a          (501) staff       (20)     3315 2023-06-26 05:51:28.000000 potato_tool-0.0.6/README.md
+drwxr-xr-x   0 a          (501) staff       (20)        0 2023-06-26 06:20:52.122348 potato_tool-0.0.6/potato_tool/
+-rw-r--r--   0 a          (501) staff       (20)       30 2023-06-26 05:17:26.000000 potato_tool-0.0.6/potato_tool/__init__.py
+-rwxr-xr-x   0 a          (501) staff       (20)    11199 2023-06-26 06:20:22.000000 potato_tool-0.0.6/potato_tool/font.py
+drwxr-xr-x   0 a          (501) staff       (20)        0 2023-06-26 06:20:52.124569 potato_tool-0.0.6/potato_tool.egg-info/
+-rw-r--r--   0 a          (501) staff       (20)     3597 2023-06-26 06:20:52.000000 potato_tool-0.0.6/potato_tool.egg-info/PKG-INFO
+-rw-r--r--   0 a          (501) staff       (20)      274 2023-06-26 06:20:52.000000 potato_tool-0.0.6/potato_tool.egg-info/SOURCES.txt
+-rw-r--r--   0 a          (501) staff       (20)        1 2023-06-26 06:20:52.000000 potato_tool-0.0.6/potato_tool.egg-info/dependency_links.txt
+-rw-r--r--   0 a          (501) staff       (20)     1026 2023-06-26 06:20:52.000000 potato_tool-0.0.6/potato_tool.egg-info/entry_points.txt
+-rw-r--r--   0 a          (501) staff       (20)       25 2023-06-26 06:20:52.000000 potato_tool-0.0.6/potato_tool.egg-info/requires.txt
+-rw-r--r--   0 a          (501) staff       (20)       12 2023-06-26 06:20:52.000000 potato_tool-0.0.6/potato_tool.egg-info/top_level.txt
+-rw-r--r--   0 a          (501) staff       (20)       38 2023-06-26 06:20:52.125378 potato_tool-0.0.6/setup.cfg
+-rw-r--r--   0 a          (501) staff       (20)     2164 2023-06-26 06:20:32.000000 potato_tool-0.0.6/setup.py
```

### Comparing `potato_tool-0.0.5/PKG-INFO` & `potato_tool-0.0.6/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: potato_tool
-Version: 0.0.5
+Version: 0.0.6
 Summary: 输出染色、前置符、格式化输出及表格输出
 Home-page: https://potato.gold
 Author: Potato
 Author-email: ljy1058318852@163.com
 License: UNKNOWN
 Platform: UNKNOWN
 Description-Content-Type: text/markdown
```

### Comparing `potato_tool-0.0.5/README.md` & `potato_tool-0.0.6/README.md`

 * *Files identical despite different names*

### Comparing `potato_tool-0.0.5/potato_tool/font.py` & `potato_tool-0.0.6/potato_tool/font.py`

 * *Files 1% similar despite different names*

```diff
@@ -295,10 +295,8 @@
                      __        __
         ____  ____ _/ /_____ _/ /_____
        / __ \/ __ `/ __/ __ `/ __/ __ \\
       / /_/ / /_/ / /_/ /_/ / /_/ /_/ / ''',end="")
     blueP('''
      / .___/\____/\__/\__,_/\__/\____/
     /_/
-''')
-
-logo_1()
+''')
```

### Comparing `potato_tool-0.0.5/potato_tool.egg-info/PKG-INFO` & `potato_tool-0.0.6/potato_tool.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: potato-tool
-Version: 0.0.5
+Version: 0.0.6
 Summary: 输出染色、前置符、格式化输出及表格输出
 Home-page: https://potato.gold
 Author: Potato
 Author-email: ljy1058318852@163.com
 License: UNKNOWN
 Platform: UNKNOWN
 Description-Content-Type: text/markdown
```

### Comparing `potato_tool-0.0.5/potato_tool.egg-info/entry_points.txt` & `potato_tool-0.0.6/potato_tool.egg-info/entry_points.txt`

 * *Files identical despite different names*

### Comparing `potato_tool-0.0.5/setup.py` & `potato_tool-0.0.6/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 import codecs
 
 with codecs.open("README.md", "r", encoding="utf-8") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name='potato_tool',
-    version='0.0.5',
+    version='0.0.6',
     author='Potato',
     author_email='ljy1058318852@163.com',
     url='https://potato.gold',
     description=u'输出染色、前置符、格式化输出及表格输出',
     long_description=long_description,
     long_description_content_type="text/markdown",
     packages=setuptools.find_packages(),
```

