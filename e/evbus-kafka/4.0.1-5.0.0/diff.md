# Comparing `tmp/evbus-kafka-4.0.1.tar.gz` & `tmp/evbus-kafka-5.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "evbus-kafka-4.0.1.tar", last modified: Mon Jun 13 18:07:39 2022, max compression
+gzip compressed data, was "evbus-kafka-5.0.0.tar", last modified: Mon Jun 26 15:26:34 2023, max compression
```

## Comparing `evbus-kafka-4.0.1.tar` & `evbus-kafka-5.0.0.tar`

### file list

```diff
@@ -1,22 +1,22 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-06-13 18:07:39.853458 evbus-kafka-4.0.1/
--rw-r--r--   0 root         (0) root         (0)    11341 2022-01-19 21:19:26.000000 evbus-kafka-4.0.1/LICENSE
--rw-r--r--   0 root         (0) root         (0)     4590 2022-06-13 18:07:39.853458 evbus-kafka-4.0.1/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     3724 2022-02-24 15:38:38.000000 evbus-kafka-4.0.1/README.rst
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-06-13 18:07:39.853458 evbus-kafka-4.0.1/evbus_kafka/
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-06-13 18:07:39.853458 evbus-kafka-4.0.1/evbus_kafka/acct/
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-06-13 18:07:39.853458 evbus-kafka-4.0.1/evbus_kafka/acct/kafka/
--rw-r--r--   0 root         (0) root         (0)     1147 2022-05-11 22:01:14.000000 evbus-kafka-4.0.1/evbus_kafka/acct/kafka/extras.py
--rw-r--r--   0 root         (0) root         (0)     1768 2022-05-11 22:15:33.000000 evbus-kafka-4.0.1/evbus_kafka/acct/kafka/ssl.py
--rw-r--r--   0 root         (0) root         (0)       94 2022-05-11 22:01:14.000000 evbus-kafka-4.0.1/evbus_kafka/conf.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-06-13 18:07:39.853458 evbus-kafka-4.0.1/evbus_kafka/ingress/
--rw-r--r--   0 root         (0) root         (0)     1665 2022-06-13 17:27:54.000000 evbus-kafka-4.0.1/evbus_kafka/ingress/kakfa_queue.py
--rw-r--r--   0 root         (0) root         (0)       18 2022-06-13 18:07:38.000000 evbus-kafka-4.0.1/evbus_kafka/version.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-06-13 18:07:39.853458 evbus-kafka-4.0.1/evbus_kafka.egg-info/
--rw-r--r--   0 root         (0) root         (0)     4590 2022-06-13 18:07:39.000000 evbus-kafka-4.0.1/evbus_kafka.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      367 2022-06-13 18:07:39.000000 evbus-kafka-4.0.1/evbus_kafka.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2022-06-13 18:07:39.000000 evbus-kafka-4.0.1/evbus_kafka.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       46 2022-06-13 18:07:39.000000 evbus-kafka-4.0.1/evbus_kafka.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       12 2022-06-13 18:07:39.000000 evbus-kafka-4.0.1/evbus_kafka.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)      255 2022-01-19 21:19:26.000000 evbus-kafka-4.0.1/pyproject.toml
--rw-r--r--   0 root         (0) root         (0)       73 2022-06-13 18:07:39.853458 evbus-kafka-4.0.1/setup.cfg
--rw-r--r--   0 root         (0) root         (0)     2747 2022-01-19 21:31:13.000000 evbus-kafka-4.0.1/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-26 15:26:34.700991 evbus-kafka-5.0.0/
+-rw-r--r--   0 root         (0) root         (0)    11341 2023-06-26 15:26:20.000000 evbus-kafka-5.0.0/LICENSE
+-rw-r--r--   0 root         (0) root         (0)     4591 2023-06-26 15:26:34.700991 evbus-kafka-5.0.0/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     3724 2023-06-26 15:26:20.000000 evbus-kafka-5.0.0/README.rst
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-26 15:26:34.700991 evbus-kafka-5.0.0/evbus_kafka/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-26 15:26:34.700991 evbus-kafka-5.0.0/evbus_kafka/acct/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-26 15:26:34.700991 evbus-kafka-5.0.0/evbus_kafka/acct/kafka/
+-rw-r--r--   0 root         (0) root         (0)     1147 2023-06-26 15:26:20.000000 evbus-kafka-5.0.0/evbus_kafka/acct/kafka/extras.py
+-rw-r--r--   0 root         (0) root         (0)     1768 2023-06-26 15:26:20.000000 evbus-kafka-5.0.0/evbus_kafka/acct/kafka/ssl.py
+-rw-r--r--   0 root         (0) root         (0)       94 2023-06-26 15:26:20.000000 evbus-kafka-5.0.0/evbus_kafka/conf.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-26 15:26:34.700991 evbus-kafka-5.0.0/evbus_kafka/ingress/
+-rw-r--r--   0 root         (0) root         (0)     1665 2023-06-26 15:26:20.000000 evbus-kafka-5.0.0/evbus_kafka/ingress/kakfa_queue.py
+-rw-r--r--   0 root         (0) root         (0)       18 2023-06-26 15:26:34.000000 evbus-kafka-5.0.0/evbus_kafka/version.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-26 15:26:34.700991 evbus-kafka-5.0.0/evbus_kafka.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     4591 2023-06-26 15:26:34.000000 evbus-kafka-5.0.0/evbus_kafka.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      367 2023-06-26 15:26:34.000000 evbus-kafka-5.0.0/evbus_kafka.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-06-26 15:26:34.000000 evbus-kafka-5.0.0/evbus_kafka.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       46 2023-06-26 15:26:34.000000 evbus-kafka-5.0.0/evbus_kafka.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       12 2023-06-26 15:26:34.000000 evbus-kafka-5.0.0/evbus_kafka.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)      265 2023-06-26 15:26:20.000000 evbus-kafka-5.0.0/pyproject.toml
+-rw-r--r--   0 root         (0) root         (0)       73 2023-06-26 15:26:34.700991 evbus-kafka-5.0.0/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)     2748 2023-06-26 15:26:20.000000 evbus-kafka-5.0.0/setup.py
```

### Comparing `evbus-kafka-4.0.1/LICENSE` & `evbus-kafka-5.0.0/LICENSE`

 * *Files identical despite different names*

### Comparing `evbus-kafka-4.0.1/PKG-INFO` & `evbus-kafka-5.0.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,28 +1,28 @@
 Metadata-Version: 2.1
 Name: evbus-kafka
-Version: 4.0.1
+Version: 5.0.0
 Summary: evbus app-merge components for kafka queues
 Home-page: https://gitlab.com/idem/evbus-kafka
 Author: Joseph Hall
 Author-email: perlhoser@gmail.com
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Environment :: Console
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: Information Technology
 Classifier: Intended Audience :: System Administrators
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python
-Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
 Classifier: Development Status :: 5 - Production/Stable
-Requires-Python: >=3.7
+Requires-Python: >=3.8
 Description-Content-Type: text/x-rst
 License-File: LICENSE
 
 ===========
 evbus-kafka
 ===========
 
@@ -38,15 +38,15 @@
 
 Getting Started
 ===============
 
 Prerequisites
 -------------
 
-* Python 3.7+
+* Python 3.8+
 * git *(if installing from source, or contributing to the project)*
 
 Installation
 ------------
 
 .. note::
```

### Comparing `evbus-kafka-4.0.1/README.rst` & `evbus-kafka-5.0.0/README.rst`

 * *Files 1% similar despite different names*

```diff
@@ -14,15 +14,15 @@
 
 Getting Started
 ===============
 
 Prerequisites
 -------------
 
-* Python 3.7+
+* Python 3.8+
 * git *(if installing from source, or contributing to the project)*
 
 Installation
 ------------
 
 .. note::
```

### Comparing `evbus-kafka-4.0.1/evbus_kafka/acct/kafka/extras.py` & `evbus-kafka-5.0.0/evbus_kafka/acct/kafka/extras.py`

 * *Files identical despite different names*

### Comparing `evbus-kafka-4.0.1/evbus_kafka/acct/kafka/ssl.py` & `evbus-kafka-5.0.0/evbus_kafka/acct/kafka/ssl.py`

 * *Files identical despite different names*

### Comparing `evbus-kafka-4.0.1/evbus_kafka/ingress/kakfa_queue.py` & `evbus-kafka-5.0.0/evbus_kafka/ingress/kakfa_queue.py`

 * *Files identical despite different names*

### Comparing `evbus-kafka-4.0.1/evbus_kafka.egg-info/PKG-INFO` & `evbus-kafka-5.0.0/evbus_kafka.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,28 +1,28 @@
 Metadata-Version: 2.1
 Name: evbus-kafka
-Version: 4.0.1
+Version: 5.0.0
 Summary: evbus app-merge components for kafka queues
 Home-page: https://gitlab.com/idem/evbus-kafka
 Author: Joseph Hall
 Author-email: perlhoser@gmail.com
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Environment :: Console
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: Information Technology
 Classifier: Intended Audience :: System Administrators
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python
-Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
 Classifier: Development Status :: 5 - Production/Stable
-Requires-Python: >=3.7
+Requires-Python: >=3.8
 Description-Content-Type: text/x-rst
 License-File: LICENSE
 
 ===========
 evbus-kafka
 ===========
 
@@ -38,15 +38,15 @@
 
 Getting Started
 ===============
 
 Prerequisites
 -------------
 
-* Python 3.7+
+* Python 3.8+
 * git *(if installing from source, or contributing to the project)*
 
 Installation
 ------------
 
 .. note::
```

### Comparing `evbus-kafka-4.0.1/setup.py` & `evbus-kafka-5.0.0/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -71,24 +71,24 @@
     url="https://gitlab.com/idem/evbus-kafka",
     version=VERSION,
     install_requires=REQUIREMENTS,
     extras_require=REQUIREMENTS_EXTRA,
     description=DESC,
     long_description=LONG_DESC,
     long_description_content_type="text/x-rst",
-    python_requires=">=3.7",
+    python_requires=">=3.8",
     classifiers=[
         "Environment :: Console",
         "Intended Audience :: Developers",
         "Intended Audience :: Information Technology",
         "Intended Audience :: System Administrators",
         "Operating System :: OS Independent",
         "Programming Language :: Python",
-        "Programming Language :: Python :: 3.7",
         "Programming Language :: Python :: 3.8",
         "Programming Language :: Python :: 3.9",
         "Programming Language :: Python :: 3.10",
+        "Programming Language :: Python :: 3.11",
         "Development Status :: 5 - Production/Stable",
     ],
     packages=discover_packages(),
     cmdclass={"clean": Clean},
 )
```

