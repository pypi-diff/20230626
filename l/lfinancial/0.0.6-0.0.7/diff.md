# Comparing `tmp/lfinancial-0.0.6.tar.gz` & `tmp/lfinancial-0.0.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "lfinancial-0.0.6.tar", last modified: Mon Jun 26 14:01:25 2023, max compression
+gzip compressed data, was "lfinancial-0.0.7.tar", last modified: Mon Jun 26 15:42:16 2023, max compression
```

## Comparing `lfinancial-0.0.6.tar` & `lfinancial-0.0.7.tar`

### file list

```diff
@@ -1,13 +1,16 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 14:01:25.272941 lfinancial-0.0.6/
--rw-r--r--   0 runner    (1001) docker     (123)     1063 2023-06-26 14:01:25.272941 lfinancial-0.0.6/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      732 2023-06-26 14:01:15.000000 lfinancial-0.0.6/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 14:01:25.272941 lfinancial-0.0.6/lfinancial/
--rw-r--r--   0 runner    (1001) docker     (123)       33 2023-06-26 14:01:15.000000 lfinancial-0.0.6/lfinancial/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      604 2023-06-26 14:01:15.000000 lfinancial-0.0.6/lfinancial/financial.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 14:01:25.272941 lfinancial-0.0.6/lfinancial.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1063 2023-06-26 14:01:25.000000 lfinancial-0.0.6/lfinancial.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      201 2023-06-26 14:01:25.000000 lfinancial-0.0.6/lfinancial.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-26 14:01:25.000000 lfinancial-0.0.6/lfinancial.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       11 2023-06-26 14:01:25.000000 lfinancial-0.0.6/lfinancial.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-26 14:01:25.272941 lfinancial-0.0.6/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      667 2023-06-26 14:01:15.000000 lfinancial-0.0.6/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 15:42:16.056700 lfinancial-0.0.7/
+-rw-r--r--   0 runner    (1001) docker     (123)    18092 2023-06-26 15:42:02.000000 lfinancial-0.0.7/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     1111 2023-06-26 15:42:16.056700 lfinancial-0.0.7/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      732 2023-06-26 15:42:02.000000 lfinancial-0.0.7/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 15:42:16.056700 lfinancial-0.0.7/lfinancial/
+-rw-r--r--   0 runner    (1001) docker     (123)       33 2023-06-26 15:42:02.000000 lfinancial-0.0.7/lfinancial/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      604 2023-06-26 15:42:02.000000 lfinancial-0.0.7/lfinancial/financial.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 15:42:16.056700 lfinancial-0.0.7/lfinancial.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1111 2023-06-26 15:42:16.000000 lfinancial-0.0.7/lfinancial.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      237 2023-06-26 15:42:16.000000 lfinancial-0.0.7/lfinancial.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-26 15:42:16.000000 lfinancial-0.0.7/lfinancial.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       11 2023-06-26 15:42:16.000000 lfinancial-0.0.7/lfinancial.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-26 15:42:16.056700 lfinancial-0.0.7/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      693 2023-06-26 15:42:02.000000 lfinancial-0.0.7/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 15:42:16.056700 lfinancial-0.0.7/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)      308 2023-06-26 15:42:02.000000 lfinancial-0.0.7/tests/test_document_type.py
```

### Comparing `lfinancial-0.0.6/PKG-INFO` & `lfinancial-0.0.7/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,17 +1,18 @@
 Metadata-Version: 2.1
 Name: lfinancial
-Version: 0.0.6
+Version: 0.0.7
 Summary: Generate financial test data
 Author: zaneliu
 Author-email: lzy291980138@163.com
 Classifier: Programming Language :: Python :: 3
-Classifier: License :: OSI Approved :: MIT License
+Classifier: License :: OSI Approved :: GNU General Public License v2 (GPLv2)
 Classifier: Operating System :: OS Independent
 Description-Content-Type: text/markdown
+License-File: LICENSE
 
 LFinancial is a Python package that generates financial fake data.
 
 ---
 ```
 .-.    .----. .-. .-. .-.   .--.   .-. .-. .----. .-.   .--.   .-.    
 } |    } |__} { | |  \{ |  / {} \  |  \{ | | }`-' { |  / {} \  } |
```

### Comparing `lfinancial-0.0.6/README.md` & `lfinancial-0.0.7/README.md`

 * *Files identical despite different names*

### Comparing `lfinancial-0.0.6/lfinancial/financial.py` & `lfinancial-0.0.7/lfinancial/financial.py`

 * *Files identical despite different names*

### Comparing `lfinancial-0.0.6/lfinancial.egg-info/PKG-INFO` & `lfinancial-0.0.7/lfinancial.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,17 +1,18 @@
 Metadata-Version: 2.1
 Name: lfinancial
-Version: 0.0.6
+Version: 0.0.7
 Summary: Generate financial test data
 Author: zaneliu
 Author-email: lzy291980138@163.com
 Classifier: Programming Language :: Python :: 3
-Classifier: License :: OSI Approved :: MIT License
+Classifier: License :: OSI Approved :: GNU General Public License v2 (GPLv2)
 Classifier: Operating System :: OS Independent
 Description-Content-Type: text/markdown
+License-File: LICENSE
 
 LFinancial is a Python package that generates financial fake data.
 
 ---
 ```
 .-.    .----. .-. .-. .-.   .--.   .-. .-. .----. .-.   .--.   .-.    
 } |    } |__} { | |  \{ |  / {} \  |  \{ | | }`-' { |  / {} \  } |
```

