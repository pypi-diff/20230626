# Comparing `tmp/cmem_plugin_kafka-1.3.0rc1.tar.gz` & `tmp/cmem_plugin_kafka-1.3.1rc1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cmem_plugin_kafka-1.3.0rc1.tar", max compression
+gzip compressed data, was "cmem_plugin_kafka-1.3.1rc1.tar", max compression
```

## Comparing `cmem_plugin_kafka-1.3.0rc1.tar` & `cmem_plugin_kafka-1.3.1rc1.tar`

### file list

```diff
@@ -1,11 +1,11 @@
--rw-r--r--   0        0        0    11334 2023-06-20 07:14:18.923375 cmem_plugin_kafka-1.3.0rc1/LICENSE
--rw-r--r--   0        0        0     3733 2023-06-20 07:14:18.923375 cmem_plugin_kafka-1.3.0rc1/README-public.md
--rw-r--r--   0        0        0        0 2023-06-20 07:14:18.923375 cmem_plugin_kafka-1.3.0rc1/cmem_plugin_kafka/__init__.py
--rw-r--r--   0        0        0     4331 2023-06-20 07:14:18.923375 cmem_plugin_kafka-1.3.0rc1/cmem_plugin_kafka/constants.py
--rw-r--r--   0        0        0    14787 2023-06-20 07:14:18.923375 cmem_plugin_kafka-1.3.0rc1/cmem_plugin_kafka/kafka_handlers.py
--rw-r--r--   0        0        0    12053 2023-06-20 07:14:18.923375 cmem_plugin_kafka-1.3.0rc1/cmem_plugin_kafka/utils.py
--rw-r--r--   0        0        0        0 2023-06-20 07:14:18.923375 cmem_plugin_kafka-1.3.0rc1/cmem_plugin_kafka/workflow/__init__.py
--rw-r--r--   0        0        0    11646 2023-06-20 07:14:18.923375 cmem_plugin_kafka-1.3.0rc1/cmem_plugin_kafka/workflow/consumer.py
--rw-r--r--   0        0        0     9739 2023-06-20 07:14:18.923375 cmem_plugin_kafka-1.3.0rc1/cmem_plugin_kafka/workflow/producer.py
--rw-r--r--   0        0        0     2206 2023-06-20 07:14:46.663061 cmem_plugin_kafka-1.3.0rc1/pyproject.toml
--rw-r--r--   0        0        0     4792 1970-01-01 00:00:00.000000 cmem_plugin_kafka-1.3.0rc1/PKG-INFO
+-rw-r--r--   0        0        0    11334 2023-06-26 06:54:32.897262 cmem_plugin_kafka-1.3.1rc1/LICENSE
+-rw-r--r--   0        0        0     3733 2023-06-26 06:54:32.897262 cmem_plugin_kafka-1.3.1rc1/README-public.md
+-rw-r--r--   0        0        0        0 2023-06-26 06:54:32.901262 cmem_plugin_kafka-1.3.1rc1/cmem_plugin_kafka/__init__.py
+-rw-r--r--   0        0        0     4331 2023-06-26 06:54:32.901262 cmem_plugin_kafka-1.3.1rc1/cmem_plugin_kafka/constants.py
+-rw-r--r--   0        0        0    14787 2023-06-26 06:54:32.901262 cmem_plugin_kafka-1.3.1rc1/cmem_plugin_kafka/kafka_handlers.py
+-rw-r--r--   0        0        0    12053 2023-06-26 06:54:32.901262 cmem_plugin_kafka-1.3.1rc1/cmem_plugin_kafka/utils.py
+-rw-r--r--   0        0        0        0 2023-06-26 06:54:32.901262 cmem_plugin_kafka-1.3.1rc1/cmem_plugin_kafka/workflow/__init__.py
+-rw-r--r--   0        0        0    11646 2023-06-26 06:54:32.901262 cmem_plugin_kafka-1.3.1rc1/cmem_plugin_kafka/workflow/consumer.py
+-rw-r--r--   0        0        0     9739 2023-06-26 06:54:32.901262 cmem_plugin_kafka-1.3.1rc1/cmem_plugin_kafka/workflow/producer.py
+-rw-r--r--   0        0        0     2242 2023-06-26 06:54:59.489295 cmem_plugin_kafka-1.3.1rc1/pyproject.toml
+-rw-r--r--   0        0        0     4843 1970-01-01 00:00:00.000000 cmem_plugin_kafka-1.3.1rc1/PKG-INFO
```

### Comparing `cmem_plugin_kafka-1.3.0rc1/LICENSE` & `cmem_plugin_kafka-1.3.1rc1/LICENSE`

 * *Files identical despite different names*

### Comparing `cmem_plugin_kafka-1.3.0rc1/README-public.md` & `cmem_plugin_kafka-1.3.1rc1/README-public.md`

 * *Files identical despite different names*

### Comparing `cmem_plugin_kafka-1.3.0rc1/cmem_plugin_kafka/constants.py` & `cmem_plugin_kafka-1.3.1rc1/cmem_plugin_kafka/constants.py`

 * *Files identical despite different names*

### Comparing `cmem_plugin_kafka-1.3.0rc1/cmem_plugin_kafka/kafka_handlers.py` & `cmem_plugin_kafka-1.3.1rc1/cmem_plugin_kafka/kafka_handlers.py`

 * *Files identical despite different names*

### Comparing `cmem_plugin_kafka-1.3.0rc1/cmem_plugin_kafka/utils.py` & `cmem_plugin_kafka-1.3.1rc1/cmem_plugin_kafka/utils.py`

 * *Files identical despite different names*

### Comparing `cmem_plugin_kafka-1.3.0rc1/cmem_plugin_kafka/workflow/consumer.py` & `cmem_plugin_kafka-1.3.1rc1/cmem_plugin_kafka/workflow/consumer.py`

 * *Files identical despite different names*

### Comparing `cmem_plugin_kafka-1.3.0rc1/cmem_plugin_kafka/workflow/producer.py` & `cmem_plugin_kafka-1.3.1rc1/cmem_plugin_kafka/workflow/producer.py`

 * *Files identical despite different names*

### Comparing `cmem_plugin_kafka-1.3.0rc1/pyproject.toml` & `cmem_plugin_kafka-1.3.1rc1/pyproject.toml`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "cmem-plugin-kafka"
-version = "1.3.0rc1"
+version = "1.3.1rc1"
 license = "Apache-2.0"
 description = "Send and receive messages from Apache Kafka."
 authors = ["eccenca GmbH <cmempy-developer@eccenca.com>"]
 classifiers = [
     "Development Status :: 5 - Production/Stable",
     "Environment :: Plugins",
     "Topic :: Software Development :: Libraries :: Python Modules",
@@ -18,20 +18,21 @@
 homepage = "https://github.com/eccenca/cmem-plugin-kafka"
 
 
 [tool.poetry.dependencies]
 python = "^3.9"
 cmem-plugin-base = "^3.1.0"
 confluent-kafka = [
-    { version = "1.9.2" },
+    { version = "2.1.1" },
     # before you publish, comment out this next line
     # { markers = "sys_platform == 'darwin'", url = "https://files.pythonhosted.org/packages/fb/16/d04dded73439266a3dbcd585f1128483dcf509e039bacd93642ac5de97d4/confluent-kafka-1.8.2.tar.gz"}
 ]
 defusedxml = "^0.7.1"
 json-stream = "2.3.0"
+json-stream-rs-tokenizer = "0.4.17"
 
 [tool.poetry.group.dev.dependencies]
 bandit = "^1.7.5"
 black = "^23.3.0"
 coverage = "^7.2.3"
 defusedxml = "^0.7.1"
 flake8-formatter-junit-xml = "^0.0.6"
```

### Comparing `cmem_plugin_kafka-1.3.0rc1/PKG-INFO` & `cmem_plugin_kafka-1.3.1rc1/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cmem-plugin-kafka
-Version: 1.3.0rc1
+Version: 1.3.1rc1
 Summary: Send and receive messages from Apache Kafka.
 Home-page: https://github.com/eccenca/cmem-plugin-kafka
 License: Apache-2.0
 Keywords: eccenca Corporate Memory,plugin,kafka,kafka-producer,kafka-consumer
 Author: eccenca GmbH
 Author-email: cmempy-developer@eccenca.com
 Requires-Python: >=3.9,<4.0
@@ -14,17 +14,18 @@
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Requires-Dist: cmem-plugin-base (>=3.1.0,<4.0.0)
-Requires-Dist: confluent-kafka (==1.9.2)
+Requires-Dist: confluent-kafka (==2.1.1)
 Requires-Dist: defusedxml (>=0.7.1,<0.8.0)
 Requires-Dist: json-stream (==2.3.0)
+Requires-Dist: json-stream-rs-tokenizer (==0.4.17)
 Description-Content-Type: text/markdown
 
 # cmem-plugin-kafka
 
 Send and receive messages from Apache Kafka.
 
 This is a plugin for [eccenca](https://eccenca.com) [Corporate Memory](https://documentation.eccenca.com).
```

