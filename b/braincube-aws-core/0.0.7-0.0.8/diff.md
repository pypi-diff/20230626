# Comparing `tmp/braincube-aws-core-0.0.7.tar.gz` & `tmp/braincube-aws-core-0.0.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "braincube-aws-core-0.0.7.tar", last modified: Mon Jun 26 12:28:34 2023, max compression
+gzip compressed data, was "braincube-aws-core-0.0.8.tar", last modified: Mon Jun 26 12:59:48 2023, max compression
```

## Comparing `braincube-aws-core-0.0.7.tar` & `braincube-aws-core-0.0.8.tar`

### file list

```diff
@@ -1,43 +1,43 @@
-drwxr-xr-x   0 evangelosboudis   (501) staff       (20)        0 2023-06-26 12:28:34.497773 braincube-aws-core-0.0.7/
--rw-r--r--   0 evangelosboudis   (501) staff       (20)     1066 2023-05-10 08:49:09.000000 braincube-aws-core-0.0.7/LICENSE
--rw-r--r--   0 evangelosboudis   (501) staff       (20)     8755 2023-06-26 12:28:34.498060 braincube-aws-core-0.0.7/PKG-INFO
--rw-r--r--   0 evangelosboudis   (501) staff       (20)     8009 2023-06-21 20:23:04.000000 braincube-aws-core-0.0.7/README.md
--rw-r--r--   0 evangelosboudis   (501) staff       (20)      103 2023-05-10 08:49:09.000000 braincube-aws-core-0.0.7/pyproject.toml
--rw-r--r--   0 evangelosboudis   (501) staff       (20)      946 2023-06-26 12:28:34.499246 braincube-aws-core-0.0.7/setup.cfg
--rw-r--r--   0 evangelosboudis   (501) staff       (20)       38 2023-05-10 08:49:09.000000 braincube-aws-core-0.0.7/setup.py
-drwxr-xr-x   0 evangelosboudis   (501) staff       (20)        0 2023-06-26 12:28:34.474156 braincube-aws-core-0.0.7/src/
-drwxr-xr-x   0 evangelosboudis   (501) staff       (20)        0 2023-06-26 12:28:34.478923 braincube-aws-core-0.0.7/src/braincube_aws_core.egg-info/
--rw-r--r--   0 evangelosboudis   (501) staff       (20)     8755 2023-06-26 12:28:34.000000 braincube-aws-core-0.0.7/src/braincube_aws_core.egg-info/PKG-INFO
--rw-r--r--   0 evangelosboudis   (501) staff       (20)      932 2023-06-26 12:28:34.000000 braincube-aws-core-0.0.7/src/braincube_aws_core.egg-info/SOURCES.txt
--rw-r--r--   0 evangelosboudis   (501) staff       (20)        1 2023-06-26 12:28:34.000000 braincube-aws-core-0.0.7/src/braincube_aws_core.egg-info/dependency_links.txt
--rw-r--r--   0 evangelosboudis   (501) staff       (20)       67 2023-06-26 12:28:34.000000 braincube-aws-core-0.0.7/src/braincube_aws_core.egg-info/requires.txt
--rw-r--r--   0 evangelosboudis   (501) staff       (20)        5 2023-06-26 12:28:34.000000 braincube-aws-core-0.0.7/src/braincube_aws_core.egg-info/top_level.txt
-drwxr-xr-x   0 evangelosboudis   (501) staff       (20)        0 2023-06-26 12:28:34.479298 braincube-aws-core-0.0.7/src/core/
--rw-r--r--   0 evangelosboudis   (501) staff       (20)        0 2023-05-10 08:49:09.000000 braincube-aws-core-0.0.7/src/core/__init__.py
-drwxr-xr-x   0 evangelosboudis   (501) staff       (20)        0 2023-06-26 12:28:34.484925 braincube-aws-core-0.0.7/src/core/app/
--rw-r--r--   0 evangelosboudis   (501) staff       (20)        0 2023-05-10 08:49:09.000000 braincube-aws-core-0.0.7/src/core/app/__init__.py
--rw-r--r--   0 evangelosboudis   (501) staff       (20)     2971 2023-06-26 09:56:02.000000 braincube-aws-core-0.0.7/src/core/app/app_controller.py
--rw-r--r--   0 evangelosboudis   (501) staff       (20)     1872 2023-06-26 06:47:29.000000 braincube-aws-core-0.0.7/src/core/app/app_event.py
--rw-r--r--   0 evangelosboudis   (501) staff       (20)     5067 2023-06-26 12:26:27.000000 braincube-aws-core-0.0.7/src/core/app/app_module.py
--rw-r--r--   0 evangelosboudis   (501) staff       (20)      489 2023-06-26 06:58:32.000000 braincube-aws-core-0.0.7/src/core/app/app_processor.py
--rw-r--r--   0 evangelosboudis   (501) staff       (20)     5462 2023-06-26 08:24:01.000000 braincube-aws-core-0.0.7/src/core/app/data.py
--rw-r--r--   0 evangelosboudis   (501) staff       (20)      680 2023-06-26 08:19:40.000000 braincube-aws-core-0.0.7/src/core/app/http_exception_handler.py
-drwxr-xr-x   0 evangelosboudis   (501) staff       (20)        0 2023-06-26 12:28:34.490668 braincube-aws-core-0.0.7/src/core/dal/
--rw-r--r--   0 evangelosboudis   (501) staff       (20)        0 2023-05-10 08:49:09.000000 braincube-aws-core-0.0.7/src/core/dal/__init__.py
--rw-r--r--   0 evangelosboudis   (501) staff       (20)     1990 2023-06-14 20:23:51.000000 braincube-aws-core-0.0.7/src/core/dal/data.py
--rw-r--r--   0 evangelosboudis   (501) staff       (20)      241 2023-05-11 10:53:14.000000 braincube-aws-core-0.0.7/src/core/dal/database_errors.py
--rw-r--r--   0 evangelosboudis   (501) staff       (20)     6191 2023-06-15 06:23:48.000000 braincube-aws-core-0.0.7/src/core/dal/postgres_connection.py
--rw-r--r--   0 evangelosboudis   (501) staff       (20)    33246 2023-06-22 15:26:24.000000 braincube-aws-core-0.0.7/src/core/dal/postgres_repository.py
-drwxr-xr-x   0 evangelosboudis   (501) staff       (20)        0 2023-06-26 12:28:34.493049 braincube-aws-core-0.0.7/src/core/di/
--rw-r--r--   0 evangelosboudis   (501) staff       (20)        0 2023-05-10 08:49:09.000000 braincube-aws-core-0.0.7/src/core/di/__init__.py
--rw-r--r--   0 evangelosboudis   (501) staff       (20)      561 2023-05-11 10:50:19.000000 braincube-aws-core-0.0.7/src/core/di/data.py
--rw-r--r--   0 evangelosboudis   (501) staff       (20)     4122 2023-05-11 10:51:25.000000 braincube-aws-core-0.0.7/src/core/di/injector.py
-drwxr-xr-x   0 evangelosboudis   (501) staff       (20)        0 2023-06-26 12:28:34.495419 braincube-aws-core-0.0.7/src/core/rules_engine/
--rw-r--r--   0 evangelosboudis   (501) staff       (20)        0 2023-05-10 08:49:09.000000 braincube-aws-core-0.0.7/src/core/rules_engine/__init__.py
--rw-r--r--   0 evangelosboudis   (501) staff       (20)     1017 2023-06-01 06:45:52.000000 braincube-aws-core-0.0.7/src/core/rules_engine/data.py
--rw-r--r--   0 evangelosboudis   (501) staff       (20)      132 2023-06-01 06:45:21.000000 braincube-aws-core-0.0.7/src/core/rules_engine/exceptions.py
--rw-r--r--   0 evangelosboudis   (501) staff       (20)     2752 2023-06-01 07:59:06.000000 braincube-aws-core-0.0.7/src/core/rules_engine/rule_manager.py
-drwxr-xr-x   0 evangelosboudis   (501) staff       (20)        0 2023-06-26 12:28:34.497116 braincube-aws-core-0.0.7/src/core/utils/
--rw-r--r--   0 evangelosboudis   (501) staff       (20)        0 2023-05-10 08:49:09.000000 braincube-aws-core-0.0.7/src/core/utils/__init__.py
--rw-r--r--   0 evangelosboudis   (501) staff       (20)      738 2023-05-15 14:42:55.000000 braincube-aws-core-0.0.7/src/core/utils/convert.py
--rw-r--r--   0 evangelosboudis   (501) staff       (20)     1377 2023-05-11 10:53:41.000000 braincube-aws-core-0.0.7/src/core/utils/data.py
+drwxr-xr-x   0 evangelosboudis   (501) staff       (20)        0 2023-06-26 12:59:48.555010 braincube-aws-core-0.0.8/
+-rw-r--r--   0 evangelosboudis   (501) staff       (20)     1066 2023-05-10 08:49:09.000000 braincube-aws-core-0.0.8/LICENSE
+-rw-r--r--   0 evangelosboudis   (501) staff       (20)     8755 2023-06-26 12:59:48.555276 braincube-aws-core-0.0.8/PKG-INFO
+-rw-r--r--   0 evangelosboudis   (501) staff       (20)     8009 2023-06-21 20:23:04.000000 braincube-aws-core-0.0.8/README.md
+-rw-r--r--   0 evangelosboudis   (501) staff       (20)      103 2023-05-10 08:49:09.000000 braincube-aws-core-0.0.8/pyproject.toml
+-rw-r--r--   0 evangelosboudis   (501) staff       (20)      946 2023-06-26 12:59:48.556633 braincube-aws-core-0.0.8/setup.cfg
+-rw-r--r--   0 evangelosboudis   (501) staff       (20)       38 2023-05-10 08:49:09.000000 braincube-aws-core-0.0.8/setup.py
+drwxr-xr-x   0 evangelosboudis   (501) staff       (20)        0 2023-06-26 12:59:48.535639 braincube-aws-core-0.0.8/src/
+drwxr-xr-x   0 evangelosboudis   (501) staff       (20)        0 2023-06-26 12:59:48.541241 braincube-aws-core-0.0.8/src/braincube_aws_core.egg-info/
+-rw-r--r--   0 evangelosboudis   (501) staff       (20)     8755 2023-06-26 12:59:48.000000 braincube-aws-core-0.0.8/src/braincube_aws_core.egg-info/PKG-INFO
+-rw-r--r--   0 evangelosboudis   (501) staff       (20)      932 2023-06-26 12:59:48.000000 braincube-aws-core-0.0.8/src/braincube_aws_core.egg-info/SOURCES.txt
+-rw-r--r--   0 evangelosboudis   (501) staff       (20)        1 2023-06-26 12:59:48.000000 braincube-aws-core-0.0.8/src/braincube_aws_core.egg-info/dependency_links.txt
+-rw-r--r--   0 evangelosboudis   (501) staff       (20)       67 2023-06-26 12:59:48.000000 braincube-aws-core-0.0.8/src/braincube_aws_core.egg-info/requires.txt
+-rw-r--r--   0 evangelosboudis   (501) staff       (20)        5 2023-06-26 12:59:48.000000 braincube-aws-core-0.0.8/src/braincube_aws_core.egg-info/top_level.txt
+drwxr-xr-x   0 evangelosboudis   (501) staff       (20)        0 2023-06-26 12:59:48.541577 braincube-aws-core-0.0.8/src/core/
+-rw-r--r--   0 evangelosboudis   (501) staff       (20)        0 2023-05-10 08:49:09.000000 braincube-aws-core-0.0.8/src/core/__init__.py
+drwxr-xr-x   0 evangelosboudis   (501) staff       (20)        0 2023-06-26 12:59:48.546055 braincube-aws-core-0.0.8/src/core/app/
+-rw-r--r--   0 evangelosboudis   (501) staff       (20)        0 2023-05-10 08:49:09.000000 braincube-aws-core-0.0.8/src/core/app/__init__.py
+-rw-r--r--   0 evangelosboudis   (501) staff       (20)     2971 2023-06-26 09:56:02.000000 braincube-aws-core-0.0.8/src/core/app/app_controller.py
+-rw-r--r--   0 evangelosboudis   (501) staff       (20)     1872 2023-06-26 06:47:29.000000 braincube-aws-core-0.0.8/src/core/app/app_event.py
+-rw-r--r--   0 evangelosboudis   (501) staff       (20)     5067 2023-06-26 12:58:44.000000 braincube-aws-core-0.0.8/src/core/app/app_module.py
+-rw-r--r--   0 evangelosboudis   (501) staff       (20)      489 2023-06-26 06:58:32.000000 braincube-aws-core-0.0.8/src/core/app/app_processor.py
+-rw-r--r--   0 evangelosboudis   (501) staff       (20)     5462 2023-06-26 08:24:01.000000 braincube-aws-core-0.0.8/src/core/app/data.py
+-rw-r--r--   0 evangelosboudis   (501) staff       (20)      680 2023-06-26 08:19:40.000000 braincube-aws-core-0.0.8/src/core/app/http_exception_handler.py
+drwxr-xr-x   0 evangelosboudis   (501) staff       (20)        0 2023-06-26 12:59:48.549147 braincube-aws-core-0.0.8/src/core/dal/
+-rw-r--r--   0 evangelosboudis   (501) staff       (20)        0 2023-05-10 08:49:09.000000 braincube-aws-core-0.0.8/src/core/dal/__init__.py
+-rw-r--r--   0 evangelosboudis   (501) staff       (20)     1990 2023-06-14 20:23:51.000000 braincube-aws-core-0.0.8/src/core/dal/data.py
+-rw-r--r--   0 evangelosboudis   (501) staff       (20)      241 2023-05-11 10:53:14.000000 braincube-aws-core-0.0.8/src/core/dal/database_errors.py
+-rw-r--r--   0 evangelosboudis   (501) staff       (20)     6191 2023-06-15 06:23:48.000000 braincube-aws-core-0.0.8/src/core/dal/postgres_connection.py
+-rw-r--r--   0 evangelosboudis   (501) staff       (20)    33246 2023-06-22 15:26:24.000000 braincube-aws-core-0.0.8/src/core/dal/postgres_repository.py
+drwxr-xr-x   0 evangelosboudis   (501) staff       (20)        0 2023-06-26 12:59:48.550721 braincube-aws-core-0.0.8/src/core/di/
+-rw-r--r--   0 evangelosboudis   (501) staff       (20)        0 2023-05-10 08:49:09.000000 braincube-aws-core-0.0.8/src/core/di/__init__.py
+-rw-r--r--   0 evangelosboudis   (501) staff       (20)      561 2023-05-11 10:50:19.000000 braincube-aws-core-0.0.8/src/core/di/data.py
+-rw-r--r--   0 evangelosboudis   (501) staff       (20)     4122 2023-05-11 10:51:25.000000 braincube-aws-core-0.0.8/src/core/di/injector.py
+drwxr-xr-x   0 evangelosboudis   (501) staff       (20)        0 2023-06-26 12:59:48.552849 braincube-aws-core-0.0.8/src/core/rules_engine/
+-rw-r--r--   0 evangelosboudis   (501) staff       (20)        0 2023-05-10 08:49:09.000000 braincube-aws-core-0.0.8/src/core/rules_engine/__init__.py
+-rw-r--r--   0 evangelosboudis   (501) staff       (20)     1017 2023-06-01 06:45:52.000000 braincube-aws-core-0.0.8/src/core/rules_engine/data.py
+-rw-r--r--   0 evangelosboudis   (501) staff       (20)      132 2023-06-01 06:45:21.000000 braincube-aws-core-0.0.8/src/core/rules_engine/exceptions.py
+-rw-r--r--   0 evangelosboudis   (501) staff       (20)     2752 2023-06-01 07:59:06.000000 braincube-aws-core-0.0.8/src/core/rules_engine/rule_manager.py
+drwxr-xr-x   0 evangelosboudis   (501) staff       (20)        0 2023-06-26 12:59:48.554405 braincube-aws-core-0.0.8/src/core/utils/
+-rw-r--r--   0 evangelosboudis   (501) staff       (20)        0 2023-05-10 08:49:09.000000 braincube-aws-core-0.0.8/src/core/utils/__init__.py
+-rw-r--r--   0 evangelosboudis   (501) staff       (20)      738 2023-05-15 14:42:55.000000 braincube-aws-core-0.0.8/src/core/utils/convert.py
+-rw-r--r--   0 evangelosboudis   (501) staff       (20)     1377 2023-05-11 10:53:41.000000 braincube-aws-core-0.0.8/src/core/utils/data.py
```

### Comparing `braincube-aws-core-0.0.7/LICENSE` & `braincube-aws-core-0.0.8/LICENSE`

 * *Files identical despite different names*

### Comparing `braincube-aws-core-0.0.7/PKG-INFO` & `braincube-aws-core-0.0.8/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: braincube-aws-core
-Version: 0.0.7
+Version: 0.0.8
 Summary: Microframework for python aws lambdas
 Home-page: https://bitbucket.org/braincube-common/core-aws.git
 Author: Braincube
 Author-email: v.boudis@braincube.gr
 License: MIT
 Keywords: python,amazon,aws,lambda,routing,dal,injection
 Classifier: Intended Audience :: Developers
```

### Comparing `braincube-aws-core-0.0.7/README.md` & `braincube-aws-core-0.0.8/README.md`

 * *Files identical despite different names*

### Comparing `braincube-aws-core-0.0.7/setup.cfg` & `braincube-aws-core-0.0.8/setup.cfg`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = braincube-aws-core
-version = 0.0.7
+version = 0.0.8
 author = Braincube
 author_email = v.boudis@braincube.gr
 description = Microframework for python aws lambdas
 long_description = file: README.md
 long_description_content_type = text/markdown
 url = https://bitbucket.org/braincube-common/core-aws.git
 license = MIT
```

### Comparing `braincube-aws-core-0.0.7/src/braincube_aws_core.egg-info/PKG-INFO` & `braincube-aws-core-0.0.8/src/braincube_aws_core.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: braincube-aws-core
-Version: 0.0.7
+Version: 0.0.8
 Summary: Microframework for python aws lambdas
 Home-page: https://bitbucket.org/braincube-common/core-aws.git
 Author: Braincube
 Author-email: v.boudis@braincube.gr
 License: MIT
 Keywords: python,amazon,aws,lambda,routing,dal,injection
 Classifier: Intended Audience :: Developers
```

### Comparing `braincube-aws-core-0.0.7/src/braincube_aws_core.egg-info/SOURCES.txt` & `braincube-aws-core-0.0.8/src/braincube_aws_core.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `braincube-aws-core-0.0.7/src/core/app/app_controller.py` & `braincube-aws-core-0.0.8/src/core/app/app_controller.py`

 * *Files identical despite different names*

### Comparing `braincube-aws-core-0.0.7/src/core/app/app_event.py` & `braincube-aws-core-0.0.8/src/core/app/app_event.py`

 * *Files identical despite different names*

### Comparing `braincube-aws-core-0.0.7/src/core/app/app_module.py` & `braincube-aws-core-0.0.8/src/core/app/app_module.py`

 * *Files identical despite different names*

### Comparing `braincube-aws-core-0.0.7/src/core/app/data.py` & `braincube-aws-core-0.0.8/src/core/app/data.py`

 * *Files identical despite different names*

### Comparing `braincube-aws-core-0.0.7/src/core/app/http_exception_handler.py` & `braincube-aws-core-0.0.8/src/core/app/http_exception_handler.py`

 * *Files identical despite different names*

### Comparing `braincube-aws-core-0.0.7/src/core/dal/data.py` & `braincube-aws-core-0.0.8/src/core/dal/data.py`

 * *Files identical despite different names*

### Comparing `braincube-aws-core-0.0.7/src/core/dal/postgres_connection.py` & `braincube-aws-core-0.0.8/src/core/dal/postgres_connection.py`

 * *Files identical despite different names*

### Comparing `braincube-aws-core-0.0.7/src/core/dal/postgres_repository.py` & `braincube-aws-core-0.0.8/src/core/dal/postgres_repository.py`

 * *Files identical despite different names*

### Comparing `braincube-aws-core-0.0.7/src/core/di/data.py` & `braincube-aws-core-0.0.8/src/core/di/data.py`

 * *Files identical despite different names*

### Comparing `braincube-aws-core-0.0.7/src/core/di/injector.py` & `braincube-aws-core-0.0.8/src/core/di/injector.py`

 * *Files identical despite different names*

### Comparing `braincube-aws-core-0.0.7/src/core/rules_engine/data.py` & `braincube-aws-core-0.0.8/src/core/rules_engine/data.py`

 * *Files identical despite different names*

### Comparing `braincube-aws-core-0.0.7/src/core/rules_engine/rule_manager.py` & `braincube-aws-core-0.0.8/src/core/rules_engine/rule_manager.py`

 * *Files identical despite different names*

### Comparing `braincube-aws-core-0.0.7/src/core/utils/convert.py` & `braincube-aws-core-0.0.8/src/core/utils/convert.py`

 * *Files identical despite different names*

### Comparing `braincube-aws-core-0.0.7/src/core/utils/data.py` & `braincube-aws-core-0.0.8/src/core/utils/data.py`

 * *Files identical despite different names*

