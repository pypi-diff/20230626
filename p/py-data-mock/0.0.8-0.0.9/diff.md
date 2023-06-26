# Comparing `tmp/py-data-mock-0.0.8.tar.gz` & `tmp/py-data-mock-0.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "py-data-mock-0.0.8.tar", last modified: Sat Jun 24 21:02:46 2023, max compression
+gzip compressed data, was "py-data-mock-0.0.9.tar", last modified: Mon Jun 26 16:05:45 2023, max compression
```

## Comparing `py-data-mock-0.0.8.tar` & `py-data-mock-0.0.9.tar`

### file list

```diff
@@ -1,45 +1,48 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-24 21:02:46.562688 py-data-mock-0.0.8/
--rw-r--r--   0 root         (0) root         (0)    35149 2023-06-24 21:01:57.000000 py-data-mock-0.0.8/LICENSE
--rw-r--r--   0 root         (0) root         (0)      363 2023-06-24 21:02:46.562688 py-data-mock-0.0.8/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     4391 2023-06-24 21:01:57.000000 py-data-mock-0.0.8/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-24 21:02:46.558688 py-data-mock-0.0.8/data_mock/
--rw-r--r--   0 root         (0) root         (0)       53 2023-06-24 21:01:57.000000 py-data-mock-0.0.8/data_mock/__init__.py
--rw-r--r--   0 root         (0) root         (0)       85 2023-06-24 21:01:57.000000 py-data-mock-0.0.8/data_mock/exceptions.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-24 21:02:46.554687 py-data-mock-0.0.8/data_mock/google/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-24 21:02:46.554687 py-data-mock-0.0.8/data_mock/google/cloud/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-24 21:02:46.558688 py-data-mock-0.0.8/data_mock/google/cloud/bigquery/
--rw-r--r--   0 root         (0) root         (0)      827 2023-06-24 21:01:57.000000 py-data-mock-0.0.8/data_mock/google/cloud/bigquery/__init__.py
--rw-r--r--   0 root         (0) root         (0)     6784 2023-06-24 21:01:57.000000 py-data-mock-0.0.8/data_mock/google/cloud/bigquery/client.py
--rw-r--r--   0 root         (0) root         (0)      301 2023-06-24 21:01:57.000000 py-data-mock-0.0.8/data_mock/google/cloud/bigquery/dataset.py
--rw-r--r--   0 root         (0) root         (0)     1427 2023-06-24 21:01:57.000000 py-data-mock-0.0.8/data_mock/google/cloud/bigquery/enums.py
--rw-r--r--   0 root         (0) root         (0)       85 2023-06-24 21:01:57.000000 py-data-mock-0.0.8/data_mock/google/cloud/bigquery/exceptions.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-24 21:02:46.558688 py-data-mock-0.0.8/data_mock/google/cloud/bigquery/job/
--rw-r--r--   0 root         (0) root         (0)      329 2023-06-24 21:01:57.000000 py-data-mock-0.0.8/data_mock/google/cloud/bigquery/job/__init__.py
--rw-r--r--   0 root         (0) root         (0)      350 2023-06-24 21:01:57.000000 py-data-mock-0.0.8/data_mock/google/cloud/bigquery/job/load.py
--rw-r--r--   0 root         (0) root         (0)       80 2023-06-24 21:01:57.000000 py-data-mock-0.0.8/data_mock/google/cloud/bigquery/job/query.py
--rw-r--r--   0 root         (0) root         (0)       22 2023-06-24 21:01:57.000000 py-data-mock-0.0.8/data_mock/google/cloud/bigquery/retry.py
--rw-r--r--   0 root         (0) root         (0)      728 2023-06-24 21:01:57.000000 py-data-mock-0.0.8/data_mock/google/cloud/bigquery/schema.py
--rw-r--r--   0 root         (0) root         (0)     3013 2023-06-24 21:01:57.000000 py-data-mock-0.0.8/data_mock/google/cloud/bigquery/table.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-24 21:02:46.558688 py-data-mock-0.0.8/data_mock/google/cloud/storage/
--rw-r--r--   0 root         (0) root         (0)      110 2023-06-24 21:01:57.000000 py-data-mock-0.0.8/data_mock/google/cloud/storage/__init__.py
--rw-r--r--   0 root         (0) root         (0)     1228 2023-06-24 21:01:57.000000 py-data-mock-0.0.8/data_mock/google/cloud/storage/blob.py
--rw-r--r--   0 root         (0) root         (0)      522 2023-06-24 21:01:57.000000 py-data-mock-0.0.8/data_mock/google/cloud/storage/bucket.py
--rw-r--r--   0 root         (0) root         (0)      445 2023-06-24 21:01:57.000000 py-data-mock-0.0.8/data_mock/google/cloud/storage/client.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-24 21:02:46.562688 py-data-mock-0.0.8/data_mock/mock_helpers/
--rw-r--r--   0 root         (0) root         (0)     8025 2023-06-24 21:01:57.000000 py-data-mock-0.0.8/data_mock/mock_helpers/generate_data.py
--rw-r--r--   0 root         (0) root         (0)     2704 2023-06-24 21:01:57.000000 py-data-mock-0.0.8/data_mock/mock_helpers/provider.py
--rw-r--r--   0 root         (0) root         (0)      116 2023-06-24 21:01:57.000000 py-data-mock-0.0.8/data_mock/mock_helpers/writer.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-24 21:02:46.562688 py-data-mock-0.0.8/data_mock/psycopg2/
--rw-r--r--   0 root         (0) root         (0)       84 2023-06-24 21:01:57.000000 py-data-mock-0.0.8/data_mock/psycopg2/__init__.py
--rw-r--r--   0 root         (0) root         (0)     5039 2023-06-24 21:01:57.000000 py-data-mock-0.0.8/data_mock/psycopg2/connect.py
--rw-r--r--   0 root         (0) root         (0)     5360 2023-06-24 21:01:57.000000 py-data-mock-0.0.8/data_mock/psycopg2/cursor.py
--rw-r--r--   0 root         (0) root         (0)       44 2023-06-24 21:01:57.000000 py-data-mock-0.0.8/data_mock/psycopg2/exceptions.py
--rw-r--r--   0 root         (0) root         (0)      417 2023-06-24 21:01:57.000000 py-data-mock-0.0.8/data_mock/psycopg2/extras.py
--rw-r--r--   0 root         (0) root         (0)       99 2023-06-24 21:01:57.000000 py-data-mock-0.0.8/data_mock/requests.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-24 21:02:46.562688 py-data-mock-0.0.8/py_data_mock.egg-info/
--rw-r--r--   0 root         (0) root         (0)      363 2023-06-24 21:02:46.000000 py-data-mock-0.0.8/py_data_mock.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     1139 2023-06-24 21:02:46.000000 py-data-mock-0.0.8/py_data_mock.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-06-24 21:02:46.000000 py-data-mock-0.0.8/py_data_mock.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      152 2023-06-24 21:02:46.000000 py-data-mock-0.0.8/py_data_mock.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)       38 2023-06-24 21:02:46.562688 py-data-mock-0.0.8/setup.cfg
--rw-r--r--   0 root         (0) root         (0)      635 2023-06-24 21:01:57.000000 py-data-mock-0.0.8/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-26 16:05:45.840340 py-data-mock-0.0.9/
+-rw-r--r--   0 root         (0) root         (0)    35149 2023-06-26 16:05:07.000000 py-data-mock-0.0.9/LICENSE
+-rw-r--r--   0 root         (0) root         (0)      363 2023-06-26 16:05:45.840340 py-data-mock-0.0.9/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     4391 2023-06-26 16:05:07.000000 py-data-mock-0.0.9/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-26 16:05:45.832340 py-data-mock-0.0.9/data_mock/
+-rw-r--r--   0 root         (0) root         (0)       53 2023-06-26 16:05:07.000000 py-data-mock-0.0.9/data_mock/__init__.py
+-rw-r--r--   0 root         (0) root         (0)       85 2023-06-26 16:05:07.000000 py-data-mock-0.0.9/data_mock/exceptions.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-26 16:05:45.832340 py-data-mock-0.0.9/data_mock/google/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-26 16:05:45.832340 py-data-mock-0.0.9/data_mock/google/cloud/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-26 16:05:45.836341 py-data-mock-0.0.9/data_mock/google/cloud/bigquery/
+-rw-r--r--   0 root         (0) root         (0)      827 2023-06-26 16:05:07.000000 py-data-mock-0.0.9/data_mock/google/cloud/bigquery/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     6784 2023-06-26 16:05:07.000000 py-data-mock-0.0.9/data_mock/google/cloud/bigquery/client.py
+-rw-r--r--   0 root         (0) root         (0)      301 2023-06-26 16:05:07.000000 py-data-mock-0.0.9/data_mock/google/cloud/bigquery/dataset.py
+-rw-r--r--   0 root         (0) root         (0)     1427 2023-06-26 16:05:07.000000 py-data-mock-0.0.9/data_mock/google/cloud/bigquery/enums.py
+-rw-r--r--   0 root         (0) root         (0)       85 2023-06-26 16:05:07.000000 py-data-mock-0.0.9/data_mock/google/cloud/bigquery/exceptions.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-26 16:05:45.836341 py-data-mock-0.0.9/data_mock/google/cloud/bigquery/job/
+-rw-r--r--   0 root         (0) root         (0)      329 2023-06-26 16:05:07.000000 py-data-mock-0.0.9/data_mock/google/cloud/bigquery/job/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      350 2023-06-26 16:05:07.000000 py-data-mock-0.0.9/data_mock/google/cloud/bigquery/job/load.py
+-rw-r--r--   0 root         (0) root         (0)       80 2023-06-26 16:05:07.000000 py-data-mock-0.0.9/data_mock/google/cloud/bigquery/job/query.py
+-rw-r--r--   0 root         (0) root         (0)       22 2023-06-26 16:05:07.000000 py-data-mock-0.0.9/data_mock/google/cloud/bigquery/retry.py
+-rw-r--r--   0 root         (0) root         (0)      728 2023-06-26 16:05:07.000000 py-data-mock-0.0.9/data_mock/google/cloud/bigquery/schema.py
+-rw-r--r--   0 root         (0) root         (0)     3013 2023-06-26 16:05:07.000000 py-data-mock-0.0.9/data_mock/google/cloud/bigquery/table.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-26 16:05:45.836341 py-data-mock-0.0.9/data_mock/google/cloud/storage/
+-rw-r--r--   0 root         (0) root         (0)      110 2023-06-26 16:05:07.000000 py-data-mock-0.0.9/data_mock/google/cloud/storage/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     1228 2023-06-26 16:05:07.000000 py-data-mock-0.0.9/data_mock/google/cloud/storage/blob.py
+-rw-r--r--   0 root         (0) root         (0)      522 2023-06-26 16:05:07.000000 py-data-mock-0.0.9/data_mock/google/cloud/storage/bucket.py
+-rw-r--r--   0 root         (0) root         (0)      445 2023-06-26 16:05:07.000000 py-data-mock-0.0.9/data_mock/google/cloud/storage/client.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-26 16:05:45.836341 py-data-mock-0.0.9/data_mock/mock_helpers/
+-rw-r--r--   0 root         (0) root         (0)     8025 2023-06-26 16:05:07.000000 py-data-mock-0.0.9/data_mock/mock_helpers/generate_data.py
+-rw-r--r--   0 root         (0) root         (0)     2704 2023-06-26 16:05:07.000000 py-data-mock-0.0.9/data_mock/mock_helpers/provider.py
+-rw-r--r--   0 root         (0) root         (0)      116 2023-06-26 16:05:07.000000 py-data-mock-0.0.9/data_mock/mock_helpers/writer.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-26 16:05:45.836341 py-data-mock-0.0.9/data_mock/psycopg2/
+-rw-r--r--   0 root         (0) root         (0)       84 2023-06-26 16:05:07.000000 py-data-mock-0.0.9/data_mock/psycopg2/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     5039 2023-06-26 16:05:07.000000 py-data-mock-0.0.9/data_mock/psycopg2/connect.py
+-rw-r--r--   0 root         (0) root         (0)     5360 2023-06-26 16:05:07.000000 py-data-mock-0.0.9/data_mock/psycopg2/cursor.py
+-rw-r--r--   0 root         (0) root         (0)       44 2023-06-26 16:05:07.000000 py-data-mock-0.0.9/data_mock/psycopg2/exceptions.py
+-rw-r--r--   0 root         (0) root         (0)      417 2023-06-26 16:05:07.000000 py-data-mock-0.0.9/data_mock/psycopg2/extras.py
+-rw-r--r--   0 root         (0) root         (0)       99 2023-06-26 16:05:07.000000 py-data-mock-0.0.9/data_mock/requests.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-26 16:05:45.836341 py-data-mock-0.0.9/data_mock/requests_lib/
+-rw-r--r--   0 root         (0) root         (0)        2 2023-06-26 16:05:07.000000 py-data-mock-0.0.9/data_mock/requests_lib/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     2636 2023-06-26 16:05:07.000000 py-data-mock-0.0.9/data_mock/requests_lib/main.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-26 16:05:45.840340 py-data-mock-0.0.9/py_data_mock.egg-info/
+-rw-r--r--   0 root         (0) root         (0)      363 2023-06-26 16:05:45.000000 py-data-mock-0.0.9/py_data_mock.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     1205 2023-06-26 16:05:45.000000 py-data-mock-0.0.9/py_data_mock.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-06-26 16:05:45.000000 py-data-mock-0.0.9/py_data_mock.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      176 2023-06-26 16:05:45.000000 py-data-mock-0.0.9/py_data_mock.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)       38 2023-06-26 16:05:45.840340 py-data-mock-0.0.9/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)      662 2023-06-26 16:05:07.000000 py-data-mock-0.0.9/setup.py
```

### Comparing `py-data-mock-0.0.8/LICENSE` & `py-data-mock-0.0.9/LICENSE`

 * *Files identical despite different names*

### Comparing `py-data-mock-0.0.8/README.md` & `py-data-mock-0.0.9/README.md`

 * *Files identical despite different names*

### Comparing `py-data-mock-0.0.8/data_mock/google/cloud/bigquery/__init__.py` & `py-data-mock-0.0.9/data_mock/google/cloud/bigquery/__init__.py`

 * *Files identical despite different names*

### Comparing `py-data-mock-0.0.8/data_mock/google/cloud/bigquery/client.py` & `py-data-mock-0.0.9/data_mock/google/cloud/bigquery/client.py`

 * *Files identical despite different names*

### Comparing `py-data-mock-0.0.8/data_mock/google/cloud/bigquery/enums.py` & `py-data-mock-0.0.9/data_mock/google/cloud/bigquery/enums.py`

 * *Files identical despite different names*

### Comparing `py-data-mock-0.0.8/data_mock/google/cloud/bigquery/schema.py` & `py-data-mock-0.0.9/data_mock/google/cloud/bigquery/schema.py`

 * *Files identical despite different names*

### Comparing `py-data-mock-0.0.8/data_mock/google/cloud/bigquery/table.py` & `py-data-mock-0.0.9/data_mock/google/cloud/bigquery/table.py`

 * *Files identical despite different names*

### Comparing `py-data-mock-0.0.8/data_mock/google/cloud/storage/blob.py` & `py-data-mock-0.0.9/data_mock/google/cloud/storage/blob.py`

 * *Files identical despite different names*

### Comparing `py-data-mock-0.0.8/data_mock/google/cloud/storage/bucket.py` & `py-data-mock-0.0.9/data_mock/google/cloud/storage/bucket.py`

 * *Files identical despite different names*

### Comparing `py-data-mock-0.0.8/data_mock/mock_helpers/generate_data.py` & `py-data-mock-0.0.9/data_mock/mock_helpers/generate_data.py`

 * *Files identical despite different names*

### Comparing `py-data-mock-0.0.8/data_mock/mock_helpers/provider.py` & `py-data-mock-0.0.9/data_mock/mock_helpers/provider.py`

 * *Files identical despite different names*

### Comparing `py-data-mock-0.0.8/data_mock/psycopg2/connect.py` & `py-data-mock-0.0.9/data_mock/psycopg2/connect.py`

 * *Files identical despite different names*

### Comparing `py-data-mock-0.0.8/data_mock/psycopg2/cursor.py` & `py-data-mock-0.0.9/data_mock/psycopg2/cursor.py`

 * *Files identical despite different names*

### Comparing `py-data-mock-0.0.8/py_data_mock.egg-info/SOURCES.txt` & `py-data-mock-0.0.9/py_data_mock.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -23,11 +23,13 @@
 data_mock/mock_helpers/provider.py
 data_mock/mock_helpers/writer.py
 data_mock/psycopg2/__init__.py
 data_mock/psycopg2/connect.py
 data_mock/psycopg2/cursor.py
 data_mock/psycopg2/exceptions.py
 data_mock/psycopg2/extras.py
+data_mock/requests_lib/__init__.py
+data_mock/requests_lib/main.py
 py_data_mock.egg-info/PKG-INFO
 py_data_mock.egg-info/SOURCES.txt
 py_data_mock.egg-info/dependency_links.txt
 py_data_mock.egg-info/top_level.txt
```

### Comparing `py-data-mock-0.0.8/setup.py` & `py-data-mock-0.0.9/setup.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,19 +1,19 @@
 from setuptools import setup
 
 setup(
     name='py-data-mock',
-    version='0.0.8',    
+    version='0.0.9',    
     description='Mock Data',
     url='https://github.com/paulhtremblay/py-data-mock',
     author='Henry Tremblay',
     author_email='paulhtremblay@gmail.com',
     license='GNU GENERAL PUBLIC LICENSE',
     packages=['data_mock/google/cloud/bigquery/job', 'data_mock/google/cloud/bigquery',
         'data_mock/google/cloud/storage','data_mock/mock_helpers', 'data_mock',
-        'data_mock/psycopg2/',
+        'data_mock/psycopg2/', 'data_mock/requests_lib/',
         ],
      classifiers=[
         'Programming Language :: Python :: 3',
         'Topic :: Software Development :: Testing :: Mocking'
     ],
 )
```

