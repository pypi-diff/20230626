# Comparing `tmp/KafkaMetricsExporter-0.0.2.tar.gz` & `tmp/KafkaMetricsExporter-0.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "KafkaMetricsExporter-0.0.2.tar", last modified: Mon Jun 26 14:32:07 2023, max compression
+gzip compressed data, was "KafkaMetricsExporter-0.0.3.tar", last modified: Mon Jun 26 15:15:54 2023, max compression
```

## Comparing `KafkaMetricsExporter-0.0.2.tar` & `KafkaMetricsExporter-0.0.3.tar`

### file list

```diff
@@ -1,11 +1,11 @@
-drwxr-xr-x   0 rachana_hpe   (502) staff       (20)        0 2023-06-26 14:32:07.877971 KafkaMetricsExporter-0.0.2/
-drwxr-xr-x   0 rachana_hpe   (502) staff       (20)        0 2023-06-26 14:32:07.874922 KafkaMetricsExporter-0.0.2/KafkaMetricsExporter/
--rw-r--r--   0 rachana_hpe   (502) staff       (20)    20892 2023-06-26 13:42:29.000000 KafkaMetricsExporter-0.0.2/KafkaMetricsExporter/__init__.py
--rw-r--r--   0 rachana_hpe   (502) staff       (20)     1057 2023-06-26 14:31:25.000000 KafkaMetricsExporter-0.0.2/KafkaMetricsExporter/setup.py
-drwxr-xr-x   0 rachana_hpe   (502) staff       (20)        0 2023-06-26 14:32:07.876743 KafkaMetricsExporter-0.0.2/KafkaMetricsExporter.egg-info/
--rw-r--r--   0 rachana_hpe   (502) staff       (20)      538 2023-06-26 14:32:07.000000 KafkaMetricsExporter-0.0.2/KafkaMetricsExporter.egg-info/PKG-INFO
--rw-r--r--   0 rachana_hpe   (502) staff       (20)      238 2023-06-26 14:32:07.000000 KafkaMetricsExporter-0.0.2/KafkaMetricsExporter.egg-info/SOURCES.txt
--rw-r--r--   0 rachana_hpe   (502) staff       (20)        1 2023-06-26 14:32:07.000000 KafkaMetricsExporter-0.0.2/KafkaMetricsExporter.egg-info/dependency_links.txt
--rw-r--r--   0 rachana_hpe   (502) staff       (20)       21 2023-06-26 14:32:07.000000 KafkaMetricsExporter-0.0.2/KafkaMetricsExporter.egg-info/top_level.txt
--rw-r--r--   0 rachana_hpe   (502) staff       (20)      538 2023-06-26 14:32:07.877421 KafkaMetricsExporter-0.0.2/PKG-INFO
--rw-r--r--   0 rachana_hpe   (502) staff       (20)       38 2023-06-26 14:32:07.878072 KafkaMetricsExporter-0.0.2/setup.cfg
+drwxr-xr-x   0 rachana_hpe   (502) staff       (20)        0 2023-06-26 15:15:54.718361 KafkaMetricsExporter-0.0.3/
+drwxr-xr-x   0 rachana_hpe   (502) staff       (20)        0 2023-06-26 15:15:54.715130 KafkaMetricsExporter-0.0.3/KafkaMetricsExporter/
+-rw-r--r--   0 rachana_hpe   (502) staff       (20)    20892 2023-06-26 13:42:29.000000 KafkaMetricsExporter-0.0.3/KafkaMetricsExporter/__init__.py
+drwxr-xr-x   0 rachana_hpe   (502) staff       (20)        0 2023-06-26 15:15:54.717638 KafkaMetricsExporter-0.0.3/KafkaMetricsExporter.egg-info/
+-rw-r--r--   0 rachana_hpe   (502) staff       (20)      538 2023-06-26 15:15:54.000000 KafkaMetricsExporter-0.0.3/KafkaMetricsExporter.egg-info/PKG-INFO
+-rw-r--r--   0 rachana_hpe   (502) staff       (20)      217 2023-06-26 15:15:54.000000 KafkaMetricsExporter-0.0.3/KafkaMetricsExporter.egg-info/SOURCES.txt
+-rw-r--r--   0 rachana_hpe   (502) staff       (20)        1 2023-06-26 15:15:54.000000 KafkaMetricsExporter-0.0.3/KafkaMetricsExporter.egg-info/dependency_links.txt
+-rw-r--r--   0 rachana_hpe   (502) staff       (20)       21 2023-06-26 15:15:54.000000 KafkaMetricsExporter-0.0.3/KafkaMetricsExporter.egg-info/top_level.txt
+-rw-r--r--   0 rachana_hpe   (502) staff       (20)      538 2023-06-26 15:15:54.718063 KafkaMetricsExporter-0.0.3/PKG-INFO
+-rw-r--r--   0 rachana_hpe   (502) staff       (20)       38 2023-06-26 15:15:54.718460 KafkaMetricsExporter-0.0.3/setup.cfg
+-rw-r--r--   0 rachana_hpe   (502) staff       (20)     1057 2023-06-26 15:15:30.000000 KafkaMetricsExporter-0.0.3/setup.py
```

### Comparing `KafkaMetricsExporter-0.0.2/KafkaMetricsExporter/__init__.py` & `KafkaMetricsExporter-0.0.3/KafkaMetricsExporter/__init__.py`

 * *Files identical despite different names*

### Comparing `KafkaMetricsExporter-0.0.2/KafkaMetricsExporter/setup.py` & `KafkaMetricsExporter-0.0.3/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,18 +1,18 @@
 from setuptools import setup, find_packages
 
-VERSION = '0.0.2' 
+VERSION = '0.0.3' 
 DESCRIPTION = 'My first Python package'
 LONG_DESCRIPTION = 'My first Python package on Opentelemetry Kafka metrics exporter'
 
 # Setting up
 setup(
        # the name must match the folder name 'KafkaMetricsExporter'
         name="KafkaMetricsExporter", 
-        version="0.0.2",
+        version=VERSION,
         author="Rachana Gupta",
         author_email="<rachana.gupta@hpe.com>",
         description=DESCRIPTION,
         long_description=LONG_DESCRIPTION,
         packages=find_packages(),
         install_requires=[], # add any additional packages that 
         # needs to be installed along with your package. Eg: 'caer'
```

### Comparing `KafkaMetricsExporter-0.0.2/KafkaMetricsExporter.egg-info/PKG-INFO` & `KafkaMetricsExporter-0.0.3/KafkaMetricsExporter.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: KafkaMetricsExporter
-Version: 0.0.2
+Version: 0.0.3
 Summary: My first Python package
 Author: Rachana Gupta
 Author-email: <rachana.gupta@hpe.com>
 Keywords: python,first package
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Education
 Classifier: Programming Language :: Python :: 2
```

### Comparing `KafkaMetricsExporter-0.0.2/PKG-INFO` & `KafkaMetricsExporter-0.0.3/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: KafkaMetricsExporter
-Version: 0.0.2
+Version: 0.0.3
 Summary: My first Python package
 Author: Rachana Gupta
 Author-email: <rachana.gupta@hpe.com>
 Keywords: python,first package
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Education
 Classifier: Programming Language :: Python :: 2
```

