# Comparing `tmp/snapchat-dlp-1.5.8.tar.gz` & `tmp/snapchat-dlp-1.5.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "snapchat-dlp-1.5.8.tar", last modified: Tue Jun 20 07:31:29 2023, max compression
+gzip compressed data, was "snapchat-dlp-1.5.9.tar", last modified: Wed Jun 21 07:09:11 2023, max compression
```

## Comparing `snapchat-dlp-1.5.8.tar` & `snapchat-dlp-1.5.9.tar`

### file list

```diff
@@ -1,55 +1,55 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 07:31:29.482376 snapchat-dlp-1.5.8/
--rw-r--r--   0 runner    (1001) docker     (123)      157 2023-06-20 07:31:18.000000 snapchat-dlp-1.5.8/AUTHORS.rst
--rw-r--r--   0 runner    (1001) docker     (123)     1071 2023-06-20 07:31:18.000000 snapchat-dlp-1.5.8/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      305 2023-06-20 07:31:18.000000 snapchat-dlp-1.5.8/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     5682 2023-06-20 07:31:29.482376 snapchat-dlp-1.5.8/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     3642 2023-06-20 07:31:18.000000 snapchat-dlp-1.5.8/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 07:31:29.478376 snapchat-dlp-1.5.8/docs/
--rw-r--r--   0 runner    (1001) docker     (123)      613 2023-06-20 07:31:18.000000 snapchat-dlp-1.5.8/docs/Makefile
--rw-r--r--   0 runner    (1001) docker     (123)       28 2023-06-20 07:31:18.000000 snapchat-dlp-1.5.8/docs/authors.rst
--rw-r--r--   0 runner    (1001) docker     (123)     4932 2023-06-20 07:31:18.000000 snapchat-dlp-1.5.8/docs/conf.py
--rw-r--r--   0 runner    (1001) docker     (123)       33 2023-06-20 07:31:18.000000 snapchat-dlp-1.5.8/docs/contributing.rst
--rw-r--r--   0 runner    (1001) docker     (123)       28 2023-06-20 07:31:18.000000 snapchat-dlp-1.5.8/docs/history.rst
--rw-r--r--   0 runner    (1001) docker     (123)      325 2023-06-20 07:31:18.000000 snapchat-dlp-1.5.8/docs/index.rst
--rw-r--r--   0 runner    (1001) docker     (123)     1171 2023-06-20 07:31:18.000000 snapchat-dlp-1.5.8/docs/installation.rst
--rw-r--r--   0 runner    (1001) docker     (123)      774 2023-06-20 07:31:18.000000 snapchat-dlp-1.5.8/docs/make.bat
--rw-r--r--   0 runner    (1001) docker     (123)       72 2023-06-20 07:31:18.000000 snapchat-dlp-1.5.8/docs/modules.rst
--rw-r--r--   0 runner    (1001) docker     (123)       27 2023-06-20 07:31:18.000000 snapchat-dlp-1.5.8/docs/readme.rst
--rw-r--r--   0 runner    (1001) docker     (123)      493 2023-06-20 07:31:18.000000 snapchat-dlp-1.5.8/docs/snapchat_dl.rst
--rw-r--r--   0 runner    (1001) docker     (123)       86 2023-06-20 07:31:18.000000 snapchat-dlp-1.5.8/docs/usage.rst
--rw-r--r--   0 runner    (1001) docker     (123)       25 2023-06-20 07:31:18.000000 snapchat-dlp-1.5.8/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)      467 2023-06-20 07:31:29.482376 snapchat-dlp-1.5.8/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2072 2023-06-20 07:31:18.000000 snapchat-dlp-1.5.8/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 07:31:29.478376 snapchat-dlp-1.5.8/snapchat_dlp/
--rw-r--r--   0 runner    (1001) docker     (123)      214 2023-06-20 07:31:18.000000 snapchat-dlp-1.5.8/snapchat_dlp/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2747 2023-06-20 07:31:18.000000 snapchat-dlp-1.5.8/snapchat_dlp/app.py
--rw-r--r--   0 runner    (1001) docker     (123)     3105 2023-06-20 07:31:18.000000 snapchat-dlp-1.5.8/snapchat_dlp/cli.py
--rw-r--r--   0 runner    (1001) docker     (123)     1515 2023-06-20 07:31:18.000000 snapchat-dlp-1.5.8/snapchat_dlp/downloader.py
--rw-r--r--   0 runner    (1001) docker     (123)     5295 2023-06-20 07:31:18.000000 snapchat-dlp-1.5.8/snapchat_dlp/snapchat_dlp.py
--rw-r--r--   0 runner    (1001) docker     (123)     3908 2023-06-20 07:31:18.000000 snapchat-dlp-1.5.8/snapchat_dlp/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)       22 2023-06-20 07:31:18.000000 snapchat-dlp-1.5.8/snapchat_dlp/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 07:31:29.478376 snapchat-dlp-1.5.8/snapchat_dlp.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     5682 2023-06-20 07:31:29.000000 snapchat-dlp-1.5.8/snapchat_dlp.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1073 2023-06-20 07:31:29.000000 snapchat-dlp-1.5.8/snapchat_dlp.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-20 07:31:29.000000 snapchat-dlp-1.5.8/snapchat_dlp.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       56 2023-06-20 07:31:29.000000 snapchat-dlp-1.5.8/snapchat_dlp.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-20 07:31:29.000000 snapchat-dlp-1.5.8/snapchat_dlp.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       26 2023-06-20 07:31:29.000000 snapchat-dlp-1.5.8/snapchat_dlp.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       13 2023-06-20 07:31:29.000000 snapchat-dlp-1.5.8/snapchat_dlp.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 07:31:29.478376 snapchat-dlp-1.5.8/tests/
--rw-r--r--   0 runner    (1001) docker     (123)       42 2023-06-20 07:31:18.000000 snapchat-dlp-1.5.8/tests/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 07:31:29.482376 snapchat-dlp-1.5.8/tests/mock_data/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 07:31:29.482376 snapchat-dlp-1.5.8/tests/mock_data/23/
--rw-r--r--   0 runner    (1001) docker     (123)       71 2023-06-20 07:31:18.000000 snapchat-dlp-1.5.8/tests/mock_data/23/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)    37542 2023-06-20 07:31:18.000000 snapchat-dlp-1.5.8/tests/mock_data/api-error.html
--rw-r--r--   0 runner    (1001) docker     (123)       34 2023-06-20 07:31:18.000000 snapchat-dlp-1.5.8/tests/mock_data/batch_file.txt
--rw-r--r--   0 runner    (1001) docker     (123)    36072 2023-06-20 07:31:18.000000 snapchat-dlp-1.5.8/tests/mock_data/invalidusername-nostories.html
--rw-r--r--   0 runner    (1001) docker     (123)    37543 2023-06-20 07:31:18.000000 snapchat-dlp-1.5.8/tests/mock_data/invalidusername.html
--rw-r--r--   0 runner    (1001) docker     (123)     2133 2023-06-20 07:31:18.000000 snapchat-dlp-1.5.8/tests/mock_data/invalidusername.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 07:31:29.482376 snapchat-dlp-1.5.8/tests/mock_data/user.1name/
--rw-r--r--   0 runner    (1001) docker     (123)       71 2023-06-20 07:31:18.000000 snapchat-dlp-1.5.8/tests/mock_data/user.1name/.gitignore
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 07:31:29.482376 snapchat-dlp-1.5.8/tests/mock_data/user1/
--rw-r--r--   0 runner    (1001) docker     (123)       71 2023-06-20 07:31:18.000000 snapchat-dlp-1.5.8/tests/mock_data/user1/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)     1201 2023-06-20 07:31:18.000000 snapchat-dlp-1.5.8/tests/test_downlaoder.py
--rw-r--r--   0 runner    (1001) docker     (123)     2459 2023-06-20 07:31:18.000000 snapchat-dlp-1.5.8/tests/test_snapchat_dl.py
--rw-r--r--   0 runner    (1001) docker     (123)     1883 2023-06-20 07:31:18.000000 snapchat-dlp-1.5.8/tests/test_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 07:09:11.137795 snapchat-dlp-1.5.9/
+-rw-r--r--   0 runner    (1001) docker     (123)      157 2023-06-21 07:08:57.000000 snapchat-dlp-1.5.9/AUTHORS.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1071 2023-06-21 07:08:57.000000 snapchat-dlp-1.5.9/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      305 2023-06-21 07:08:57.000000 snapchat-dlp-1.5.9/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     5682 2023-06-21 07:09:11.137795 snapchat-dlp-1.5.9/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3642 2023-06-21 07:08:57.000000 snapchat-dlp-1.5.9/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 07:09:11.133795 snapchat-dlp-1.5.9/docs/
+-rw-r--r--   0 runner    (1001) docker     (123)      613 2023-06-21 07:08:57.000000 snapchat-dlp-1.5.9/docs/Makefile
+-rw-r--r--   0 runner    (1001) docker     (123)       28 2023-06-21 07:08:57.000000 snapchat-dlp-1.5.9/docs/authors.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     4932 2023-06-21 07:08:57.000000 snapchat-dlp-1.5.9/docs/conf.py
+-rw-r--r--   0 runner    (1001) docker     (123)       33 2023-06-21 07:08:57.000000 snapchat-dlp-1.5.9/docs/contributing.rst
+-rw-r--r--   0 runner    (1001) docker     (123)       28 2023-06-21 07:08:57.000000 snapchat-dlp-1.5.9/docs/history.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      325 2023-06-21 07:08:57.000000 snapchat-dlp-1.5.9/docs/index.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1171 2023-06-21 07:08:57.000000 snapchat-dlp-1.5.9/docs/installation.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      774 2023-06-21 07:08:57.000000 snapchat-dlp-1.5.9/docs/make.bat
+-rw-r--r--   0 runner    (1001) docker     (123)       72 2023-06-21 07:08:57.000000 snapchat-dlp-1.5.9/docs/modules.rst
+-rw-r--r--   0 runner    (1001) docker     (123)       27 2023-06-21 07:08:57.000000 snapchat-dlp-1.5.9/docs/readme.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      493 2023-06-21 07:08:57.000000 snapchat-dlp-1.5.9/docs/snapchat_dl.rst
+-rw-r--r--   0 runner    (1001) docker     (123)       86 2023-06-21 07:08:57.000000 snapchat-dlp-1.5.9/docs/usage.rst
+-rw-r--r--   0 runner    (1001) docker     (123)       25 2023-06-21 07:08:57.000000 snapchat-dlp-1.5.9/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      467 2023-06-21 07:09:11.137795 snapchat-dlp-1.5.9/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2072 2023-06-21 07:08:57.000000 snapchat-dlp-1.5.9/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 07:09:11.133795 snapchat-dlp-1.5.9/snapchat_dlp/
+-rw-r--r--   0 runner    (1001) docker     (123)      214 2023-06-21 07:08:57.000000 snapchat-dlp-1.5.9/snapchat_dlp/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2747 2023-06-21 07:08:57.000000 snapchat-dlp-1.5.9/snapchat_dlp/app.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3105 2023-06-21 07:08:57.000000 snapchat-dlp-1.5.9/snapchat_dlp/cli.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1515 2023-06-21 07:08:57.000000 snapchat-dlp-1.5.9/snapchat_dlp/downloader.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5314 2023-06-21 07:08:57.000000 snapchat-dlp-1.5.9/snapchat_dlp/snapchat_dlp.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3908 2023-06-21 07:08:57.000000 snapchat-dlp-1.5.9/snapchat_dlp/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)       22 2023-06-21 07:08:57.000000 snapchat-dlp-1.5.9/snapchat_dlp/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 07:09:11.133795 snapchat-dlp-1.5.9/snapchat_dlp.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     5682 2023-06-21 07:09:10.000000 snapchat-dlp-1.5.9/snapchat_dlp.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1073 2023-06-21 07:09:11.000000 snapchat-dlp-1.5.9/snapchat_dlp.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-21 07:09:10.000000 snapchat-dlp-1.5.9/snapchat_dlp.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       56 2023-06-21 07:09:10.000000 snapchat-dlp-1.5.9/snapchat_dlp.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-21 07:09:10.000000 snapchat-dlp-1.5.9/snapchat_dlp.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       26 2023-06-21 07:09:10.000000 snapchat-dlp-1.5.9/snapchat_dlp.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       13 2023-06-21 07:09:10.000000 snapchat-dlp-1.5.9/snapchat_dlp.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 07:09:11.133795 snapchat-dlp-1.5.9/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)       42 2023-06-21 07:08:57.000000 snapchat-dlp-1.5.9/tests/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 07:09:11.133795 snapchat-dlp-1.5.9/tests/mock_data/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 07:09:11.133795 snapchat-dlp-1.5.9/tests/mock_data/23/
+-rw-r--r--   0 runner    (1001) docker     (123)       71 2023-06-21 07:08:57.000000 snapchat-dlp-1.5.9/tests/mock_data/23/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)    37542 2023-06-21 07:08:57.000000 snapchat-dlp-1.5.9/tests/mock_data/api-error.html
+-rw-r--r--   0 runner    (1001) docker     (123)       34 2023-06-21 07:08:57.000000 snapchat-dlp-1.5.9/tests/mock_data/batch_file.txt
+-rw-r--r--   0 runner    (1001) docker     (123)    36072 2023-06-21 07:08:57.000000 snapchat-dlp-1.5.9/tests/mock_data/invalidusername-nostories.html
+-rw-r--r--   0 runner    (1001) docker     (123)    37543 2023-06-21 07:08:57.000000 snapchat-dlp-1.5.9/tests/mock_data/invalidusername.html
+-rw-r--r--   0 runner    (1001) docker     (123)     2133 2023-06-21 07:08:57.000000 snapchat-dlp-1.5.9/tests/mock_data/invalidusername.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 07:09:11.137795 snapchat-dlp-1.5.9/tests/mock_data/user.1name/
+-rw-r--r--   0 runner    (1001) docker     (123)       71 2023-06-21 07:08:57.000000 snapchat-dlp-1.5.9/tests/mock_data/user.1name/.gitignore
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 07:09:11.137795 snapchat-dlp-1.5.9/tests/mock_data/user1/
+-rw-r--r--   0 runner    (1001) docker     (123)       71 2023-06-21 07:08:57.000000 snapchat-dlp-1.5.9/tests/mock_data/user1/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)     1201 2023-06-21 07:08:57.000000 snapchat-dlp-1.5.9/tests/test_downlaoder.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2459 2023-06-21 07:08:57.000000 snapchat-dlp-1.5.9/tests/test_snapchat_dl.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1883 2023-06-21 07:08:57.000000 snapchat-dlp-1.5.9/tests/test_utils.py
```

### Comparing `snapchat-dlp-1.5.8/LICENSE` & `snapchat-dlp-1.5.9/LICENSE`

 * *Files identical despite different names*

### Comparing `snapchat-dlp-1.5.8/PKG-INFO` & `snapchat-dlp-1.5.9/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: snapchat-dlp
-Version: 1.5.8
+Version: 1.5.9
 Summary: An update to snapchat-dlp, a Snapchat Public Stories Downloader.
 Home-page: https://github.com/Walmann/snapchat-dlp
 Author: Aakash Gajjar
 Author-email: skyqutip@gmail.com
 Maintainer: Walmann
 License: MIT license
 Project-URL: Original, https://github.com/skyme5/snapchat-dlp
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: snapchat-dlp Version: 1.5.8 Summary: An update to
+Metadata-Version: 2.1 Name: snapchat-dlp Version: 1.5.9 Summary: An update to
 snapchat-dlp, a Snapchat Public Stories Downloader. Home-page: https://
 github.com/Walmann/snapchat-dlp Author: Aakash Gajjar Author-email:
 skyqutip@gmail.com Maintainer: Walmann License: MIT license Project-URL:
 Original, https://github.com/skyme5/snapchat-dlp Project-URL: Source, https://
 github.com/Walmann/snapchat-dlp Description:
                    ****** Snapchat Public Stories Downloader
```

### Comparing `snapchat-dlp-1.5.8/README.md` & `snapchat-dlp-1.5.9/README.md`

 * *Files identical despite different names*

### Comparing `snapchat-dlp-1.5.8/docs/Makefile` & `snapchat-dlp-1.5.9/docs/Makefile`

 * *Files identical despite different names*

### Comparing `snapchat-dlp-1.5.8/docs/conf.py` & `snapchat-dlp-1.5.9/docs/conf.py`

 * *Files identical despite different names*

### Comparing `snapchat-dlp-1.5.8/docs/installation.rst` & `snapchat-dlp-1.5.9/docs/installation.rst`

 * *Files identical despite different names*

### Comparing `snapchat-dlp-1.5.8/docs/make.bat` & `snapchat-dlp-1.5.9/docs/make.bat`

 * *Files identical despite different names*

### Comparing `snapchat-dlp-1.5.8/setup.py` & `snapchat-dlp-1.5.9/setup.py`

 * *Files identical despite different names*

### Comparing `snapchat-dlp-1.5.8/snapchat_dlp/app.py` & `snapchat-dlp-1.5.9/snapchat_dlp/app.py`

 * *Files identical despite different names*

### Comparing `snapchat-dlp-1.5.8/snapchat_dlp/cli.py` & `snapchat-dlp-1.5.9/snapchat_dlp/cli.py`

 * *Files identical despite different names*

### Comparing `snapchat-dlp-1.5.8/snapchat_dlp/downloader.py` & `snapchat-dlp-1.5.9/snapchat_dlp/downloader.py`

 * *Files identical despite different names*

### Comparing `snapchat-dlp-1.5.8/snapchat_dlp/snapchat_dlp.py` & `snapchat-dlp-1.5.9/snapchat_dlp/snapchat_dlp.py`

 * *Files 0% similar despite different names*

```diff
@@ -78,15 +78,16 @@
             user_info = util_web_user_info(response_json)
             stories = util_web_story(response_json)
             return stories, user_info
         except (IndexError, KeyError, ValueError):
             raise APIResponseError
         except UserNotFoundError as e:
             print(f"User {username} not found. Check the spelling, or that it is a public profile.")
-            print(e)
+            # print(e)
+            pass
 
     def download(self, username):
         """Download Snapchat Story for `username`.
 
         Args:
             username (str): Snapchat `username`
```

### Comparing `snapchat-dlp-1.5.8/snapchat_dlp/utils.py` & `snapchat-dlp-1.5.9/snapchat_dlp/utils.py`

 * *Files identical despite different names*

### Comparing `snapchat-dlp-1.5.8/snapchat_dlp.egg-info/PKG-INFO` & `snapchat-dlp-1.5.9/snapchat_dlp.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: snapchat-dlp
-Version: 1.5.8
+Version: 1.5.9
 Summary: An update to snapchat-dlp, a Snapchat Public Stories Downloader.
 Home-page: https://github.com/Walmann/snapchat-dlp
 Author: Aakash Gajjar
 Author-email: skyqutip@gmail.com
 Maintainer: Walmann
 License: MIT license
 Project-URL: Original, https://github.com/skyme5/snapchat-dlp
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: snapchat-dlp Version: 1.5.8 Summary: An update to
+Metadata-Version: 2.1 Name: snapchat-dlp Version: 1.5.9 Summary: An update to
 snapchat-dlp, a Snapchat Public Stories Downloader. Home-page: https://
 github.com/Walmann/snapchat-dlp Author: Aakash Gajjar Author-email:
 skyqutip@gmail.com Maintainer: Walmann License: MIT license Project-URL:
 Original, https://github.com/skyme5/snapchat-dlp Project-URL: Source, https://
 github.com/Walmann/snapchat-dlp Description:
                    ****** Snapchat Public Stories Downloader
```

### Comparing `snapchat-dlp-1.5.8/snapchat_dlp.egg-info/SOURCES.txt` & `snapchat-dlp-1.5.9/snapchat_dlp.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `snapchat-dlp-1.5.8/tests/mock_data/api-error.html` & `snapchat-dlp-1.5.9/tests/mock_data/api-error.html`

 * *Files identical despite different names*

### Comparing `snapchat-dlp-1.5.8/tests/mock_data/invalidusername-nostories.html` & `snapchat-dlp-1.5.9/tests/mock_data/invalidusername-nostories.html`

 * *Files identical despite different names*

### Comparing `snapchat-dlp-1.5.8/tests/mock_data/invalidusername.html` & `snapchat-dlp-1.5.9/tests/mock_data/invalidusername.html`

 * *Files identical despite different names*

### Comparing `snapchat-dlp-1.5.8/tests/mock_data/invalidusername.json` & `snapchat-dlp-1.5.9/tests/mock_data/invalidusername.json`

 * *Files identical despite different names*

### Comparing `snapchat-dlp-1.5.8/tests/test_downlaoder.py` & `snapchat-dlp-1.5.9/tests/test_downlaoder.py`

 * *Files identical despite different names*

### Comparing `snapchat-dlp-1.5.8/tests/test_snapchat_dl.py` & `snapchat-dlp-1.5.9/tests/test_snapchat_dl.py`

 * *Files identical despite different names*

### Comparing `snapchat-dlp-1.5.8/tests/test_utils.py` & `snapchat-dlp-1.5.9/tests/test_utils.py`

 * *Files identical despite different names*

