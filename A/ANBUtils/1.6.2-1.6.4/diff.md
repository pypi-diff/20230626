# Comparing `tmp/ANBUtils-1.6.2.tar.gz` & `tmp/ANBUtils-1.6.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/ANBUtils-1.6.2.tar", last modified: Tue Jun 20 12:52:37 2023, max compression
+gzip compressed data, was "dist/ANBUtils-1.6.4.tar", last modified: Mon Jun 26 08:04:37 2023, max compression
```

## Comparing `ANBUtils-1.6.2.tar` & `ANBUtils-1.6.4.tar`

### file list

```diff
@@ -1,21 +1,20 @@
-drwxr-xr-x   0 redbson    (501) staff       (20)        0 2023-06-20 12:52:37.094656 ANBUtils-1.6.2/
-drwxr-xr-x   0 redbson    (501) staff       (20)        0 2023-06-20 12:52:37.090532 ANBUtils-1.6.2/ANBUtils/
--rw-r--r--   0 redbson    (501) staff       (20)      157 2023-06-20 12:51:49.000000 ANBUtils-1.6.2/ANBUtils/__info__.py
--rw-r--r--   0 redbson    (501) staff       (20)      829 2023-06-20 12:48:41.000000 ANBUtils-1.6.2/ANBUtils/__init__.py
--rw-r--r--   0 redbson    (501) staff       (20)     3129 2023-06-20 12:35:47.000000 ANBUtils-1.6.2/ANBUtils/a.py
--rw-r--r--   0 redbson    (501) staff       (20)    12409 2023-06-16 06:57:29.000000 ANBUtils-1.6.2/ANBUtils/db_worker.py
--rw-r--r--   0 redbson    (501) staff       (20)      932 2023-06-06 05:14:52.000000 ANBUtils-1.6.2/ANBUtils/easy_pickle.py
--rw-r--r--   0 redbson    (501) staff       (20)      890 2023-06-13 10:59:29.000000 ANBUtils-1.6.2/ANBUtils/environ_cheker.py
--rw-r--r--   0 redbson    (501) staff       (20)     3520 2023-06-13 11:04:14.000000 ANBUtils-1.6.2/ANBUtils/id_work.py
--rw-r--r--   0 redbson    (501) staff       (20)     1954 2023-06-13 04:36:50.000000 ANBUtils-1.6.2/ANBUtils/messenger.py
--rw-r--r--   0 redbson    (501) staff       (20)     4021 2023-06-06 05:17:20.000000 ANBUtils-1.6.2/ANBUtils/tbox.py
-drwxr-xr-x   0 redbson    (501) staff       (20)        0 2023-06-20 12:52:37.094204 ANBUtils-1.6.2/ANBUtils.egg-info/
--rw-r--r--   0 redbson    (501) staff       (20)     5322 2023-06-20 12:52:37.000000 ANBUtils-1.6.2/ANBUtils.egg-info/PKG-INFO
--rw-r--r--   0 redbson    (501) staff       (20)      365 2023-06-20 12:52:37.000000 ANBUtils-1.6.2/ANBUtils.egg-info/SOURCES.txt
--rw-r--r--   0 redbson    (501) staff       (20)        1 2023-06-20 12:52:37.000000 ANBUtils-1.6.2/ANBUtils.egg-info/dependency_links.txt
--rw-r--r--   0 redbson    (501) staff       (20)      108 2023-06-20 12:52:37.000000 ANBUtils-1.6.2/ANBUtils.egg-info/requires.txt
--rw-r--r--   0 redbson    (501) staff       (20)        9 2023-06-20 12:52:37.000000 ANBUtils-1.6.2/ANBUtils.egg-info/top_level.txt
--rw-r--r--   0 redbson    (501) staff       (20)     5322 2023-06-20 12:52:37.094475 ANBUtils-1.6.2/PKG-INFO
--rw-r--r--   0 redbson    (501) staff       (20)     4894 2023-06-13 11:16:05.000000 ANBUtils-1.6.2/README.md
--rw-r--r--   0 redbson    (501) staff       (20)       38 2023-06-20 12:52:37.094728 ANBUtils-1.6.2/setup.cfg
--rw-r--r--   0 redbson    (501) staff       (20)      869 2023-06-20 12:52:13.000000 ANBUtils-1.6.2/setup.py
+drwxr-xr-x   0 redbson    (501) staff       (20)        0 2023-06-26 08:04:37.237027 ANBUtils-1.6.4/
+drwxr-xr-x   0 redbson    (501) staff       (20)        0 2023-06-26 08:04:37.235877 ANBUtils-1.6.4/ANBUtils/
+-rw-r--r--   0 redbson    (501) staff       (20)      817 2023-06-20 13:05:30.000000 ANBUtils-1.6.4/ANBUtils/__init__.py
+-rw-r--r--   0 redbson    (501) staff       (20)     3129 2023-06-20 12:35:47.000000 ANBUtils-1.6.4/ANBUtils/a.py
+-rw-r--r--   0 redbson    (501) staff       (20)    12409 2023-06-16 06:57:29.000000 ANBUtils-1.6.4/ANBUtils/db_worker.py
+-rw-r--r--   0 redbson    (501) staff       (20)      932 2023-06-06 05:14:52.000000 ANBUtils-1.6.4/ANBUtils/easy_pickle.py
+-rw-r--r--   0 redbson    (501) staff       (20)      890 2023-06-13 10:59:29.000000 ANBUtils-1.6.4/ANBUtils/environ_cheker.py
+-rw-r--r--   0 redbson    (501) staff       (20)     3520 2023-06-13 11:04:14.000000 ANBUtils-1.6.4/ANBUtils/id_work.py
+-rw-r--r--   0 redbson    (501) staff       (20)     1954 2023-06-13 04:36:50.000000 ANBUtils-1.6.4/ANBUtils/messenger.py
+-rw-r--r--   0 redbson    (501) staff       (20)     4021 2023-06-06 05:17:20.000000 ANBUtils-1.6.4/ANBUtils/tbox.py
+drwxr-xr-x   0 redbson    (501) staff       (20)        0 2023-06-26 08:04:37.236637 ANBUtils-1.6.4/ANBUtils.egg-info/
+-rw-r--r--   0 redbson    (501) staff       (20)     5286 2023-06-26 08:04:37.000000 ANBUtils-1.6.4/ANBUtils.egg-info/PKG-INFO
+-rw-r--r--   0 redbson    (501) staff       (20)      344 2023-06-26 08:04:37.000000 ANBUtils-1.6.4/ANBUtils.egg-info/SOURCES.txt
+-rw-r--r--   0 redbson    (501) staff       (20)        1 2023-06-26 08:04:37.000000 ANBUtils-1.6.4/ANBUtils.egg-info/dependency_links.txt
+-rw-r--r--   0 redbson    (501) staff       (20)      108 2023-06-26 08:04:37.000000 ANBUtils-1.6.4/ANBUtils.egg-info/requires.txt
+-rw-r--r--   0 redbson    (501) staff       (20)        9 2023-06-26 08:04:37.000000 ANBUtils-1.6.4/ANBUtils.egg-info/top_level.txt
+-rw-r--r--   0 redbson    (501) staff       (20)     5286 2023-06-26 08:04:37.236853 ANBUtils-1.6.4/PKG-INFO
+-rw-r--r--   0 redbson    (501) staff       (20)     4894 2023-06-13 11:16:05.000000 ANBUtils-1.6.4/README.md
+-rw-r--r--   0 redbson    (501) staff       (20)       38 2023-06-26 08:04:37.237083 ANBUtils-1.6.4/setup.cfg
+-rw-r--r--   0 redbson    (501) staff       (20)      844 2023-06-26 08:04:19.000000 ANBUtils-1.6.4/setup.py
```

### Comparing `ANBUtils-1.6.2/ANBUtils/__init__.py` & `ANBUtils-1.6.4/ANBUtils/__init__.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,18 +1,15 @@
 
-from .__info__ import *
-
-
 from .environ_cheker import environment_checker as _checker
 _checker()
 
 
 
 from .a import (
-    print_rate_progress, set_date_index, digit, count, value, count2int
+    print_rate_progress, set_date_index, digit, count, value, count2int, data_browser
 )
 
 from .db_worker import (
     DBWorker, crawler_starter, log_db, read_log, dblink, dblink_add, dblink_remove, dblink_update, collection_show,
     df2mongo, mongo2df, get_db_info, get_mongodb, dblink_help, get_token,
     in_severs
 )
```

### Comparing `ANBUtils-1.6.2/ANBUtils/a.py` & `ANBUtils-1.6.4/ANBUtils/a.py`

 * *Files identical despite different names*

### Comparing `ANBUtils-1.6.2/ANBUtils/db_worker.py` & `ANBUtils-1.6.4/ANBUtils/db_worker.py`

 * *Files identical despite different names*

### Comparing `ANBUtils-1.6.2/ANBUtils/easy_pickle.py` & `ANBUtils-1.6.4/ANBUtils/easy_pickle.py`

 * *Files identical despite different names*

### Comparing `ANBUtils-1.6.2/ANBUtils/environ_cheker.py` & `ANBUtils-1.6.4/ANBUtils/environ_cheker.py`

 * *Files identical despite different names*

### Comparing `ANBUtils-1.6.2/ANBUtils/id_work.py` & `ANBUtils-1.6.4/ANBUtils/id_work.py`

 * *Files identical despite different names*

### Comparing `ANBUtils-1.6.2/ANBUtils/messenger.py` & `ANBUtils-1.6.4/ANBUtils/messenger.py`

 * *Files identical despite different names*

### Comparing `ANBUtils-1.6.2/ANBUtils/tbox.py` & `ANBUtils-1.6.4/ANBUtils/tbox.py`

 * *Files identical despite different names*

### Comparing `ANBUtils-1.6.2/ANBUtils.egg-info/PKG-INFO` & `ANBUtils-1.6.4/ANBUtils.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,17 +1,15 @@
 Metadata-Version: 2.1
 Name: ANBUtils
-Version: 1.6.2
+Version: 1.6.4
 Summary: ANBUilts is a versatile Python package that offers a comprehensive set of utility functions and tools for data analysis, database operations, and messaging integration.
 Home-page: https://github.com/redbson/ANBUtils
 Author: Yafei Hou
 Author-email: redbson@gmail.com
-License: UNKNOWN
-Platform: UNKNOWN
-Requires-Python: >=3.8
+Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 
 # ANBUtils
 
 ANBUtils is a Python package that provides various utility functions for common tasks in data analysis and database operations. It includes functions for working with MongoDB, sending messages via DingTalk, and handling date and time operations.
 
 
@@ -145,8 +143,7 @@
 ANBUtils is an open-source project, and contributions are welcome. If you encounter any issues or have suggestions for improvements, please feel free to open an issue on the [GitHub repository](https://github.com/example-user/ANBUtils).
 
 For support or general questions, you can reach out to the project maintainers or the community through the GitHub repository.
 
 ## License
 
 ANBUtils is released under the [MIT License](https://opensource.org/licenses/MIT). Please refer to the LICENSE file for more details.
-
```

### Comparing `ANBUtils-1.6.2/PKG-INFO` & `ANBUtils-1.6.4/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,17 +1,15 @@
 Metadata-Version: 2.1
 Name: ANBUtils
-Version: 1.6.2
+Version: 1.6.4
 Summary: ANBUilts is a versatile Python package that offers a comprehensive set of utility functions and tools for data analysis, database operations, and messaging integration.
 Home-page: https://github.com/redbson/ANBUtils
 Author: Yafei Hou
 Author-email: redbson@gmail.com
-License: UNKNOWN
-Platform: UNKNOWN
-Requires-Python: >=3.8
+Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 
 # ANBUtils
 
 ANBUtils is a Python package that provides various utility functions for common tasks in data analysis and database operations. It includes functions for working with MongoDB, sending messages via DingTalk, and handling date and time operations.
 
 
@@ -145,8 +143,7 @@
 ANBUtils is an open-source project, and contributions are welcome. If you encounter any issues or have suggestions for improvements, please feel free to open an issue on the [GitHub repository](https://github.com/example-user/ANBUtils).
 
 For support or general questions, you can reach out to the project maintainers or the community through the GitHub repository.
 
 ## License
 
 ANBUtils is released under the [MIT License](https://opensource.org/licenses/MIT). Please refer to the LICENSE file for more details.
-
```

### Comparing `ANBUtils-1.6.2/README.md` & `ANBUtils-1.6.4/README.md`

 * *Files identical despite different names*

### Comparing `ANBUtils-1.6.2/setup.py` & `ANBUtils-1.6.4/setup.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,26 +1,23 @@
 from setuptools import setup, find_packages
-import ANBUtils.__info__ as info
-
 
 with open('README.md', 'r', encoding='utf-8') as f:
     long_description = f.read()
 
-
 setup(
     name="ANBUtils",
-    version=info.__version__,
+    version='1.6.4',
     packages=find_packages(),
-    author=info.__author__,
-    author_email=info.__author_email__,
-    url= info.__url__,
+    author='Yafei Hou',
+    author_email='redbson@gmail.com',
+    url= 'https://github.com/redbson/ANBUtils',
     description = "ANBUilts is a versatile Python package that offers a comprehensive set of utility functions and tools for data analysis, database operations, and messaging integration.",
     long_description=long_description,
     long_description_content_type='text/markdown',
-    python_requires='>=3.8',
+    python_requires='>=3.6',
     install_requires=[
         "matplotlib>=3.0.0",
         "numpy>=1.0.0",
         "pandas>=1.0.0",
         "pymongo>=4.0.2",
         "requests>=2.0.0",
         "matplotlib>=3.0.0",
```

