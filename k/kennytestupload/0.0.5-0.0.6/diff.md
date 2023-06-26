# Comparing `tmp/kennytestupload-0.0.5.macosx-10.9-x86_64.tar.gz` & `tmp/kennytestupload-0.0.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "/Users/kenny/Desktop/GitHub/PythonClassContent/Pygame/dist/kennytestupload-0.0.5.macosx-10.9-x86_64.tar", last modified: Mon Jun 26 20:59:30 2023, max compression
+gzip compressed data, was "dist/kennytestupload-0.0.6.tar", last modified: Mon Jun 26 21:01:42 2023, max compression
```

## Comparing `kennytestupload-0.0.5.macosx-10.9-x86_64.tar` & `kennytestupload-0.0.6.tar`

### file list

```diff
@@ -1,53 +1,19 @@
-drwxr-xr-x   0 kenny      (501) staff       (20)        0 2023-06-26 20:59:30.380799 ./
-drwxr-xr-x   0 kenny      (501) staff       (20)        0 2023-06-26 20:59:30.380856 ./Users/
-drwxr-xr-x   0 kenny      (501) staff       (20)        0 2023-06-26 20:59:30.380912 ./Users/kenny/
-drwxr-xr-x   0 kenny      (501) staff       (20)        0 2023-06-26 20:59:30.380966 ./Users/kenny/Desktop/
-drwxr-xr-x   0 kenny      (501) staff       (20)        0 2023-06-26 20:59:30.381025 ./Users/kenny/Desktop/GitHub/
-drwxr-xr-x   0 kenny      (501) staff       (20)        0 2023-06-26 20:59:30.381080 ./Users/kenny/Desktop/GitHub/PythonClassContent/
-drwxr-xr-x   0 kenny      (501) staff       (20)        0 2023-06-26 20:59:30.381135 ./Users/kenny/Desktop/GitHub/PythonClassContent/PythonAlgo/
-drwxr-xr-x   0 kenny      (501) staff       (20)        0 2023-06-26 20:59:30.381190 ./Users/kenny/Desktop/GitHub/PythonClassContent/PythonAlgo/PythonDS/
-drwxr-xr-x   0 kenny      (501) staff       (20)        0 2023-06-26 20:59:30.381245 ./Users/kenny/Desktop/GitHub/PythonClassContent/PythonAlgo/PythonDS/venv/
-drwxr-xr-x   0 kenny      (501) staff       (20)        0 2023-06-26 20:59:30.381354 ./Users/kenny/Desktop/GitHub/PythonClassContent/PythonAlgo/PythonDS/venv/lib/
-drwxr-xr-x   0 kenny      (501) staff       (20)        0 2023-06-26 20:59:30.381412 ./Users/kenny/Desktop/GitHub/PythonClassContent/PythonAlgo/PythonDS/venv/lib/python3.8/
-drwxr-xr-x   0 kenny      (501) staff       (20)        0 2023-06-26 20:59:30.439325 ./Users/kenny/Desktop/GitHub/PythonClassContent/PythonAlgo/PythonDS/venv/lib/python3.8/site-packages/
-drwxr-xr-x   0 kenny      (501) staff       (20)        0 2023-06-26 20:59:30.387414 ./Users/kenny/Desktop/GitHub/PythonClassContent/PythonAlgo/PythonDS/venv/lib/python3.8/site-packages/kennytestupload/
--rw-r--r--   0 kenny      (501) staff       (20)      582 2023-06-12 20:55:20.000000 ./Users/kenny/Desktop/GitHub/PythonClassContent/PythonAlgo/PythonDS/venv/lib/python3.8/site-packages/kennytestupload/BasicDemo.py
--rw-r--r--   0 kenny      (501) staff       (20)     1543 2023-06-12 21:21:01.000000 ./Users/kenny/Desktop/GitHub/PythonClassContent/PythonAlgo/PythonDS/venv/lib/python3.8/site-packages/kennytestupload/ClassUsage.py
--rw-r--r--   0 kenny      (501) staff       (20)     1895 2023-06-20 00:05:55.000000 ./Users/kenny/Desktop/GitHub/PythonClassContent/PythonAlgo/PythonDS/venv/lib/python3.8/site-packages/kennytestupload/Collision.py
--rw-r--r--   0 kenny      (501) staff       (20)      989 2023-06-12 23:31:16.000000 ./Users/kenny/Desktop/GitHub/PythonClassContent/PythonAlgo/PythonDS/venv/lib/python3.8/site-packages/kennytestupload/Features.py
--rw-r--r--   0 kenny      (501) staff       (20)    11451 2023-06-26 19:31:00.000000 ./Users/kenny/Desktop/GitHub/PythonClassContent/PythonAlgo/PythonDS/venv/lib/python3.8/site-packages/kennytestupload/Main.py
--rw-r--r--   0 kenny      (501) staff       (20)     3018 2023-06-26 20:29:08.000000 ./Users/kenny/Desktop/GitHub/PythonClassContent/PythonAlgo/PythonDS/venv/lib/python3.8/site-packages/kennytestupload/SpaceInvader.py
--rw-r--r--   0 kenny      (501) staff       (20)     1613 2023-06-13 00:24:31.000000 ./Users/kenny/Desktop/GitHub/PythonClassContent/PythonAlgo/PythonDS/venv/lib/python3.8/site-packages/kennytestupload/Tets.py
--rw-r--r--   0 kenny      (501) staff       (20)      131 2023-06-26 20:29:08.000000 ./Users/kenny/Desktop/GitHub/PythonClassContent/PythonAlgo/PythonDS/venv/lib/python3.8/site-packages/kennytestupload/__init__.py
-drwxr-xr-x   0 kenny      (501) staff       (20)        0 2023-06-26 20:59:30.402061 ./Users/kenny/Desktop/GitHub/PythonClassContent/PythonAlgo/PythonDS/venv/lib/python3.8/site-packages/kennytestupload/__pycache__/
--rw-r--r--   0 kenny      (501) staff       (20)      639 2023-06-26 20:59:30.387956 ./Users/kenny/Desktop/GitHub/PythonClassContent/PythonAlgo/PythonDS/venv/lib/python3.8/site-packages/kennytestupload/__pycache__/BasicDemo.cpython-38.pyc
--rw-r--r--   0 kenny      (501) staff       (20)     1775 2023-06-26 20:59:30.389326 ./Users/kenny/Desktop/GitHub/PythonClassContent/PythonAlgo/PythonDS/venv/lib/python3.8/site-packages/kennytestupload/__pycache__/ClassUsage.cpython-38.pyc
--rw-r--r--   0 kenny      (501) staff       (20)     1944 2023-06-26 20:59:30.390923 ./Users/kenny/Desktop/GitHub/PythonClassContent/PythonAlgo/PythonDS/venv/lib/python3.8/site-packages/kennytestupload/__pycache__/Collision.cpython-38.pyc
--rw-r--r--   0 kenny      (501) staff       (20)      218 2023-06-26 20:59:30.389912 ./Users/kenny/Desktop/GitHub/PythonClassContent/PythonAlgo/PythonDS/venv/lib/python3.8/site-packages/kennytestupload/__pycache__/Features.cpython-38.pyc
--rw-r--r--   0 kenny      (501) staff       (20)     9399 2023-06-26 20:59:30.401946 ./Users/kenny/Desktop/GitHub/PythonClassContent/PythonAlgo/PythonDS/venv/lib/python3.8/site-packages/kennytestupload/__pycache__/Main.cpython-38.pyc
--rw-r--r--   0 kenny      (501) staff       (20)     2945 2023-06-26 20:59:30.388762 ./Users/kenny/Desktop/GitHub/PythonClassContent/PythonAlgo/PythonDS/venv/lib/python3.8/site-packages/kennytestupload/__pycache__/SpaceInvader.cpython-38.pyc
--rw-r--r--   0 kenny      (501) staff       (20)     1645 2023-06-26 20:59:30.391641 ./Users/kenny/Desktop/GitHub/PythonClassContent/PythonAlgo/PythonDS/venv/lib/python3.8/site-packages/kennytestupload/__pycache__/Tets.cpython-38.pyc
--rw-r--r--   0 kenny      (501) staff       (20)      307 2023-06-26 20:59:30.389679 ./Users/kenny/Desktop/GitHub/PythonClassContent/PythonAlgo/PythonDS/venv/lib/python3.8/site-packages/kennytestupload/__pycache__/__init__.cpython-38.pyc
-drwxr-xr-x   0 kenny      (501) staff       (20)        0 2023-06-26 20:59:30.445820 ./Users/kenny/Desktop/GitHub/PythonClassContent/PythonAlgo/PythonDS/venv/lib/python3.8/site-packages/kennytestupload-0.0.5-py3.8.egg-info/
--rw-r--r--   0 kenny      (501) staff       (20)      385 2023-06-26 20:59:30.435870 ./Users/kenny/Desktop/GitHub/PythonClassContent/PythonAlgo/PythonDS/venv/lib/python3.8/site-packages/kennytestupload-0.0.5-py3.8.egg-info/PKG-INFO
--rw-r--r--   0 kenny      (501) staff       (20)      395 2023-06-26 20:59:30.439123 ./Users/kenny/Desktop/GitHub/PythonClassContent/PythonAlgo/PythonDS/venv/lib/python3.8/site-packages/kennytestupload-0.0.5-py3.8.egg-info/SOURCES.txt
--rw-r--r--   0 kenny      (501) staff       (20)        1 2023-06-26 20:59:30.437345 ./Users/kenny/Desktop/GitHub/PythonClassContent/PythonAlgo/PythonDS/venv/lib/python3.8/site-packages/kennytestupload-0.0.5-py3.8.egg-info/dependency_links.txt
--rw-r--r--   0 kenny      (501) staff       (20)       16 2023-06-26 20:59:30.437575 ./Users/kenny/Desktop/GitHub/PythonClassContent/PythonAlgo/PythonDS/venv/lib/python3.8/site-packages/kennytestupload-0.0.5-py3.8.egg-info/top_level.txt
-drwxr-xr-x   0 kenny      (501) staff       (20)        0 2023-06-26 20:59:30.402763 ./Users/kenny/Desktop/GitHub/PythonClassContent/PythonAlgo/PythonDS/venv/lib/python3.8/site-packages/testupload/
--rw-r--r--   0 kenny      (501) staff       (20)      582 2023-06-12 20:55:20.000000 ./Users/kenny/Desktop/GitHub/PythonClassContent/PythonAlgo/PythonDS/venv/lib/python3.8/site-packages/testupload/BasicDemo.py
--rw-r--r--   0 kenny      (501) staff       (20)     1543 2023-06-12 21:21:01.000000 ./Users/kenny/Desktop/GitHub/PythonClassContent/PythonAlgo/PythonDS/venv/lib/python3.8/site-packages/testupload/ClassUsage.py
--rw-r--r--   0 kenny      (501) staff       (20)     1895 2023-06-20 00:05:55.000000 ./Users/kenny/Desktop/GitHub/PythonClassContent/PythonAlgo/PythonDS/venv/lib/python3.8/site-packages/testupload/Collision.py
--rw-r--r--   0 kenny      (501) staff       (20)      989 2023-06-12 23:31:16.000000 ./Users/kenny/Desktop/GitHub/PythonClassContent/PythonAlgo/PythonDS/venv/lib/python3.8/site-packages/testupload/Features.py
--rw-r--r--   0 kenny      (501) staff       (20)    11451 2023-06-26 19:31:00.000000 ./Users/kenny/Desktop/GitHub/PythonClassContent/PythonAlgo/PythonDS/venv/lib/python3.8/site-packages/testupload/Main.py
--rw-r--r--   0 kenny      (501) staff       (20)     3018 2023-06-26 20:29:08.000000 ./Users/kenny/Desktop/GitHub/PythonClassContent/PythonAlgo/PythonDS/venv/lib/python3.8/site-packages/testupload/SpaceInvader.py
--rw-r--r--   0 kenny      (501) staff       (20)     1613 2023-06-13 00:24:31.000000 ./Users/kenny/Desktop/GitHub/PythonClassContent/PythonAlgo/PythonDS/venv/lib/python3.8/site-packages/testupload/Tets.py
--rw-r--r--   0 kenny      (501) staff       (20)      131 2023-06-26 20:29:08.000000 ./Users/kenny/Desktop/GitHub/PythonClassContent/PythonAlgo/PythonDS/venv/lib/python3.8/site-packages/testupload/__init__.py
-drwxr-xr-x   0 kenny      (501) staff       (20)        0 2023-06-26 20:59:30.408195 ./Users/kenny/Desktop/GitHub/PythonClassContent/PythonAlgo/PythonDS/venv/lib/python3.8/site-packages/testupload/__pycache__/
--rw-r--r--   0 kenny      (501) staff       (20)      634 2023-06-26 20:59:30.402881 ./Users/kenny/Desktop/GitHub/PythonClassContent/PythonAlgo/PythonDS/venv/lib/python3.8/site-packages/testupload/__pycache__/BasicDemo.cpython-38.pyc
--rw-r--r--   0 kenny      (501) staff       (20)     1770 2023-06-26 20:59:30.404226 ./Users/kenny/Desktop/GitHub/PythonClassContent/PythonAlgo/PythonDS/venv/lib/python3.8/site-packages/testupload/__pycache__/ClassUsage.cpython-38.pyc
--rw-r--r--   0 kenny      (501) staff       (20)     1939 2023-06-26 20:59:30.405464 ./Users/kenny/Desktop/GitHub/PythonClassContent/PythonAlgo/PythonDS/venv/lib/python3.8/site-packages/testupload/__pycache__/Collision.cpython-38.pyc
--rw-r--r--   0 kenny      (501) staff       (20)      213 2023-06-26 20:59:30.404752 ./Users/kenny/Desktop/GitHub/PythonClassContent/PythonAlgo/PythonDS/venv/lib/python3.8/site-packages/testupload/__pycache__/Features.cpython-38.pyc
--rw-r--r--   0 kenny      (501) staff       (20)     9394 2023-06-26 20:59:30.408112 ./Users/kenny/Desktop/GitHub/PythonClassContent/PythonAlgo/PythonDS/venv/lib/python3.8/site-packages/testupload/__pycache__/Main.cpython-38.pyc
--rw-r--r--   0 kenny      (501) staff       (20)     2940 2023-06-26 20:59:30.403666 ./Users/kenny/Desktop/GitHub/PythonClassContent/PythonAlgo/PythonDS/venv/lib/python3.8/site-packages/testupload/__pycache__/SpaceInvader.cpython-38.pyc
--rw-r--r--   0 kenny      (501) staff       (20)     1640 2023-06-26 20:59:30.406033 ./Users/kenny/Desktop/GitHub/PythonClassContent/PythonAlgo/PythonDS/venv/lib/python3.8/site-packages/testupload/__pycache__/Tets.cpython-38.pyc
--rw-r--r--   0 kenny      (501) staff       (20)      302 2023-06-26 20:59:30.404474 ./Users/kenny/Desktop/GitHub/PythonClassContent/PythonAlgo/PythonDS/venv/lib/python3.8/site-packages/testupload/__pycache__/__init__.cpython-38.pyc
+drwxr-xr-x   0 kenny      (501) staff       (20)        0 2023-06-26 21:01:42.990807 kennytestupload-0.0.6/
+-rw-r--r--   0 kenny      (501) staff       (20)      385 2023-06-26 21:01:42.990619 kennytestupload-0.0.6/PKG-INFO
+-rw-r--r--   0 kenny      (501) staff       (20)       22 2023-06-26 19:38:53.000000 kennytestupload-0.0.6/README
+drwxr-xr-x   0 kenny      (501) staff       (20)        0 2023-06-26 21:01:42.989622 kennytestupload-0.0.6/kennytestupload/
+-rw-r--r--   0 kenny      (501) staff       (20)      582 2023-06-12 20:55:20.000000 kennytestupload-0.0.6/kennytestupload/BasicDemo.py
+-rw-r--r--   0 kenny      (501) staff       (20)     1543 2023-06-12 21:21:01.000000 kennytestupload-0.0.6/kennytestupload/ClassUsage.py
+-rw-r--r--   0 kenny      (501) staff       (20)     1895 2023-06-20 00:05:55.000000 kennytestupload-0.0.6/kennytestupload/Collision.py
+-rw-r--r--   0 kenny      (501) staff       (20)      989 2023-06-12 23:31:16.000000 kennytestupload-0.0.6/kennytestupload/Features.py
+-rw-r--r--   0 kenny      (501) staff       (20)    11451 2023-06-26 19:31:00.000000 kennytestupload-0.0.6/kennytestupload/Main.py
+-rw-r--r--   0 kenny      (501) staff       (20)     3018 2023-06-26 20:29:08.000000 kennytestupload-0.0.6/kennytestupload/SpaceInvader.py
+-rw-r--r--   0 kenny      (501) staff       (20)     1613 2023-06-13 00:24:31.000000 kennytestupload-0.0.6/kennytestupload/Tets.py
+-rw-r--r--   0 kenny      (501) staff       (20)      131 2023-06-26 20:29:08.000000 kennytestupload-0.0.6/kennytestupload/__init__.py
+drwxr-xr-x   0 kenny      (501) staff       (20)        0 2023-06-26 21:01:42.990285 kennytestupload-0.0.6/kennytestupload.egg-info/
+-rw-r--r--   0 kenny      (501) staff       (20)      385 2023-06-26 21:01:42.000000 kennytestupload-0.0.6/kennytestupload.egg-info/PKG-INFO
+-rw-r--r--   0 kenny      (501) staff       (20)      395 2023-06-26 21:01:42.000000 kennytestupload-0.0.6/kennytestupload.egg-info/SOURCES.txt
+-rw-r--r--   0 kenny      (501) staff       (20)        1 2023-06-26 21:01:42.000000 kennytestupload-0.0.6/kennytestupload.egg-info/dependency_links.txt
+-rw-r--r--   0 kenny      (501) staff       (20)       16 2023-06-26 21:01:42.000000 kennytestupload-0.0.6/kennytestupload.egg-info/top_level.txt
+-rw-r--r--   0 kenny      (501) staff       (20)       38 2023-06-26 21:01:42.990867 kennytestupload-0.0.6/setup.cfg
+-rw-r--r--   0 kenny      (501) staff       (20)      874 2023-06-26 21:01:38.000000 kennytestupload-0.0.6/setup.py
```

### Comparing `./Users/kenny/Desktop/GitHub/PythonClassContent/PythonAlgo/PythonDS/venv/lib/python3.8/site-packages/kennytestupload/BasicDemo.py` & `kennytestupload-0.0.6/kennytestupload/BasicDemo.py`

 * *Files identical despite different names*

### Comparing `./Users/kenny/Desktop/GitHub/PythonClassContent/PythonAlgo/PythonDS/venv/lib/python3.8/site-packages/kennytestupload/ClassUsage.py` & `kennytestupload-0.0.6/kennytestupload/ClassUsage.py`

 * *Files identical despite different names*

### Comparing `./Users/kenny/Desktop/GitHub/PythonClassContent/PythonAlgo/PythonDS/venv/lib/python3.8/site-packages/kennytestupload/Collision.py` & `kennytestupload-0.0.6/kennytestupload/Collision.py`

 * *Files identical despite different names*

### Comparing `./Users/kenny/Desktop/GitHub/PythonClassContent/PythonAlgo/PythonDS/venv/lib/python3.8/site-packages/kennytestupload/Features.py` & `kennytestupload-0.0.6/kennytestupload/Features.py`

 * *Files identical despite different names*

### Comparing `./Users/kenny/Desktop/GitHub/PythonClassContent/PythonAlgo/PythonDS/venv/lib/python3.8/site-packages/kennytestupload/Main.py` & `kennytestupload-0.0.6/kennytestupload/Main.py`

 * *Files identical despite different names*

### Comparing `./Users/kenny/Desktop/GitHub/PythonClassContent/PythonAlgo/PythonDS/venv/lib/python3.8/site-packages/kennytestupload/SpaceInvader.py` & `kennytestupload-0.0.6/kennytestupload/SpaceInvader.py`

 * *Files identical despite different names*

### Comparing `./Users/kenny/Desktop/GitHub/PythonClassContent/PythonAlgo/PythonDS/venv/lib/python3.8/site-packages/kennytestupload/Tets.py` & `kennytestupload-0.0.6/kennytestupload/Tets.py`

 * *Files identical despite different names*

