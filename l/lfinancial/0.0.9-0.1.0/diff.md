# Comparing `tmp/lfinancial-0.0.9.tar.gz` & `tmp/lfinancial-0.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "lfinancial-0.0.9.tar", last modified: Mon Jun 26 16:11:56 2023, max compression
+gzip compressed data, was "lfinancial-0.1.0.tar", last modified: Mon Jun 26 17:03:12 2023, max compression
```

## Comparing `lfinancial-0.0.9.tar` & `lfinancial-0.1.0.tar`

### file list

```diff
@@ -1,16 +1,17 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 16:11:56.952864 lfinancial-0.0.9/
--rw-r--r--   0 runner    (1001) docker     (123)    18092 2023-06-26 16:11:42.000000 lfinancial-0.0.9/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     1305 2023-06-26 16:11:56.952864 lfinancial-0.0.9/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      926 2023-06-26 16:11:42.000000 lfinancial-0.0.9/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 16:11:56.948863 lfinancial-0.0.9/lfinancial/
--rw-r--r--   0 runner    (1001) docker     (123)       33 2023-06-26 16:11:42.000000 lfinancial-0.0.9/lfinancial/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      604 2023-06-26 16:11:42.000000 lfinancial-0.0.9/lfinancial/financial.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 16:11:56.948863 lfinancial-0.0.9/lfinancial.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1305 2023-06-26 16:11:56.000000 lfinancial-0.0.9/lfinancial.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      237 2023-06-26 16:11:56.000000 lfinancial-0.0.9/lfinancial.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-26 16:11:56.000000 lfinancial-0.0.9/lfinancial.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       11 2023-06-26 16:11:56.000000 lfinancial-0.0.9/lfinancial.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-26 16:11:56.952864 lfinancial-0.0.9/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      693 2023-06-26 16:11:42.000000 lfinancial-0.0.9/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 16:11:56.952864 lfinancial-0.0.9/tests/
--rw-r--r--   0 runner    (1001) docker     (123)      308 2023-06-26 16:11:42.000000 lfinancial-0.0.9/tests/test_document_type.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 17:03:12.892420 lfinancial-0.1.0/
+-rw-r--r--   0 runner    (1001) docker     (123)    18092 2023-06-26 17:02:55.000000 lfinancial-0.1.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     1311 2023-06-26 17:03:12.892420 lfinancial-0.1.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      932 2023-06-26 17:02:55.000000 lfinancial-0.1.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 17:03:12.888420 lfinancial-0.1.0/lfinancial/
+-rw-r--r--   0 runner    (1001) docker     (123)       33 2023-06-26 17:02:55.000000 lfinancial-0.1.0/lfinancial/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      626 2023-06-26 17:02:55.000000 lfinancial-0.1.0/lfinancial/factory.py
+-rw-r--r--   0 runner    (1001) docker     (123)      916 2023-06-26 17:02:55.000000 lfinancial-0.1.0/lfinancial/financial.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 17:03:12.888420 lfinancial-0.1.0/lfinancial.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1311 2023-06-26 17:03:12.000000 lfinancial-0.1.0/lfinancial.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      259 2023-06-26 17:03:12.000000 lfinancial-0.1.0/lfinancial.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-26 17:03:12.000000 lfinancial-0.1.0/lfinancial.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       11 2023-06-26 17:03:12.000000 lfinancial-0.1.0/lfinancial.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-26 17:03:12.892420 lfinancial-0.1.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      693 2023-06-26 17:02:55.000000 lfinancial-0.1.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 17:03:12.888420 lfinancial-0.1.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)      299 2023-06-26 17:02:55.000000 lfinancial-0.1.0/tests/test_document_type.py
```

### Comparing `lfinancial-0.0.9/LICENSE` & `lfinancial-0.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `lfinancial-0.0.9/PKG-INFO` & `lfinancial-0.1.0/PKG-INFO`

 * *Files 22% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: lfinancial
-Version: 0.0.9
+Version: 0.1.0
 Summary: Generate financial test data
 Author: zaneliu
 Author-email: lzy291980138@163.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: GNU General Public License v2 (GPLv2)
 Classifier: Operating System :: OS Independent
 Description-Content-Type: text/markdown
@@ -29,17 +29,24 @@
 pip install lfinancial
 ```
 
 #### How to use it? 
 ```python
 from lfinancial import Financial
 
-
 f = Financial()
 
-f.id_code('SSN')
-f.id_code('SSN', 'US')
-f.id_code('IDCard', 'CN')
-f.id_code('Passport')
-f.id_code('NRIC')
-f.id_code('MyNumber')
+f.ssn()
+# 582-94-2808
+
+f.id_card()
+# 488258196409087762
+
+f.passport()
+# EG4130431
+
+f.nric()
+# SD44949622
+
+f.my_number()
+# 399495927695
 ```
```

### Comparing `lfinancial-0.0.9/README.md` & `lfinancial-0.1.0/README.md`

 * *Files 16% similar despite different names*

```diff
@@ -17,17 +17,24 @@
 pip install lfinancial
 ```
 
 #### How to use it? 
 ```python
 from lfinancial import Financial
 
-
 f = Financial()
 
-f.id_code('SSN')
-f.id_code('SSN', 'US')
-f.id_code('IDCard', 'CN')
-f.id_code('Passport')
-f.id_code('NRIC')
-f.id_code('MyNumber')
+f.ssn()
+# 582-94-2808
+
+f.id_card()
+# 488258196409087762
+
+f.passport()
+# EG4130431
+
+f.nric()
+# SD44949622
+
+f.my_number()
+# 399495927695
 ```
```

### Comparing `lfinancial-0.0.9/lfinancial.egg-info/PKG-INFO` & `lfinancial-0.1.0/lfinancial.egg-info/PKG-INFO`

 * *Files 22% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: lfinancial
-Version: 0.0.9
+Version: 0.1.0
 Summary: Generate financial test data
 Author: zaneliu
 Author-email: lzy291980138@163.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: GNU General Public License v2 (GPLv2)
 Classifier: Operating System :: OS Independent
 Description-Content-Type: text/markdown
@@ -29,17 +29,24 @@
 pip install lfinancial
 ```
 
 #### How to use it? 
 ```python
 from lfinancial import Financial
 
-
 f = Financial()
 
-f.id_code('SSN')
-f.id_code('SSN', 'US')
-f.id_code('IDCard', 'CN')
-f.id_code('Passport')
-f.id_code('NRIC')
-f.id_code('MyNumber')
+f.ssn()
+# 582-94-2808
+
+f.id_card()
+# 488258196409087762
+
+f.passport()
+# EG4130431
+
+f.nric()
+# SD44949622
+
+f.my_number()
+# 399495927695
 ```
```

### Comparing `lfinancial-0.0.9/setup.py` & `lfinancial-0.1.0/setup.py`

 * *Files 18% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 excluded_packages = ["docs", "tests", "tests.*"]
 with open("README.md", "r", encoding="utf-8") as fh:
     long_description = fh.read()
 
 
 setup(
     name='lfinancial',
-    version='0.0.9',
+    version='0.1.0',
     author='zaneliu',
     description='Generate financial test data',
     long_description=long_description,
     long_description_content_type="text/markdown",
     readme="README.md",
     author_email='lzy291980138@163.com',
     packages=['lfinancial'],
```

