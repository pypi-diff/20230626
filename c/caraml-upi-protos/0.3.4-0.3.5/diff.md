# Comparing `tmp/caraml-upi-protos-0.3.4.tar.gz` & `tmp/caraml-upi-protos-0.3.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/caraml-upi-protos-0.3.4.tar", last modified: Fri Feb  3 04:20:55 2023, max compression
+gzip compressed data, was "dist/caraml-upi-protos-0.3.5.tar", last modified: Mon Jun 26 02:44:52 2023, max compression
```

## Comparing `caraml-upi-protos-0.3.4.tar` & `caraml-upi-protos-0.3.5.tar`

### file list

```diff
@@ -1,51 +1,51 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-03 04:20:55.000000 caraml-upi-protos-0.3.4/
--rw-r--r--   0 runner    (1001) docker     (123)     4736 2023-02-03 04:20:55.000000 caraml-upi-protos-0.3.4/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     3616 2023-02-03 04:20:42.000000 caraml-upi-protos-0.3.4/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-03 04:20:55.000000 caraml-upi-protos-0.3.4/caraml/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-02-03 04:20:42.000000 caraml-upi-protos-0.3.4/caraml/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-03 04:20:55.000000 caraml-upi-protos-0.3.4/caraml/upi/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-02-03 04:20:42.000000 caraml-upi-protos-0.3.4/caraml/upi/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3839 2023-02-03 04:20:42.000000 caraml-upi-protos-0.3.4/caraml/upi/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-03 04:20:55.000000 caraml-upi-protos-0.3.4/caraml/upi/v1/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-02-03 04:20:42.000000 caraml-upi-protos-0.3.4/caraml/upi/v1/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1813 2023-02-03 04:20:42.000000 caraml-upi-protos-0.3.4/caraml/upi/v1/header_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)      725 2023-02-03 04:20:42.000000 caraml-upi-protos-0.3.4/caraml/upi/v1/header_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      159 2023-02-03 04:20:42.000000 caraml-upi-protos-0.3.4/caraml/upi/v1/header_pb2_grpc.py
--rw-r--r--   0 runner    (1001) docker     (123)       76 2023-02-03 04:20:42.000000 caraml-upi-protos-0.3.4/caraml/upi/v1/header_pb2_grpc.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     5232 2023-02-03 04:20:42.000000 caraml-upi-protos-0.3.4/caraml/upi/v1/observation_log_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)     5814 2023-02-03 04:20:42.000000 caraml-upi-protos-0.3.4/caraml/upi/v1/observation_log_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     2793 2023-02-03 04:20:42.000000 caraml-upi-protos-0.3.4/caraml/upi/v1/observation_log_pb2_grpc.py
--rw-r--r--   0 runner    (1001) docker     (123)      918 2023-02-03 04:20:42.000000 caraml-upi-protos-0.3.4/caraml/upi/v1/observation_log_pb2_grpc.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     4644 2023-02-03 04:20:42.000000 caraml-upi-protos-0.3.4/caraml/upi/v1/prediction_log_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)     7920 2023-02-03 04:20:42.000000 caraml-upi-protos-0.3.4/caraml/upi/v1/prediction_log_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      159 2023-02-03 04:20:42.000000 caraml-upi-protos-0.3.4/caraml/upi/v1/prediction_log_pb2_grpc.py
--rw-r--r--   0 runner    (1001) docker     (123)       76 2023-02-03 04:20:42.000000 caraml-upi-protos-0.3.4/caraml/upi/v1/prediction_log_pb2_grpc.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     5586 2023-02-03 04:20:42.000000 caraml-upi-protos-0.3.4/caraml/upi/v1/router_log_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)    10249 2023-02-03 04:20:42.000000 caraml-upi-protos-0.3.4/caraml/upi/v1/router_log_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      159 2023-02-03 04:20:42.000000 caraml-upi-protos-0.3.4/caraml/upi/v1/router_log_pb2_grpc.py
--rw-r--r--   0 runner    (1001) docker     (123)       76 2023-02-03 04:20:42.000000 caraml-upi-protos-0.3.4/caraml/upi/v1/router_log_pb2_grpc.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     3590 2023-02-03 04:20:42.000000 caraml-upi-protos-0.3.4/caraml/upi/v1/table_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)     4236 2023-02-03 04:20:42.000000 caraml-upi-protos-0.3.4/caraml/upi/v1/table_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      159 2023-02-03 04:20:42.000000 caraml-upi-protos-0.3.4/caraml/upi/v1/table_pb2_grpc.py
--rw-r--r--   0 runner    (1001) docker     (123)       76 2023-02-03 04:20:42.000000 caraml-upi-protos-0.3.4/caraml/upi/v1/table_pb2_grpc.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     1762 2023-02-03 04:20:42.000000 caraml-upi-protos-0.3.4/caraml/upi/v1/type_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)     1161 2023-02-03 04:20:42.000000 caraml-upi-protos-0.3.4/caraml/upi/v1/type_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      159 2023-02-03 04:20:42.000000 caraml-upi-protos-0.3.4/caraml/upi/v1/type_pb2_grpc.py
--rw-r--r--   0 runner    (1001) docker     (123)       76 2023-02-03 04:20:42.000000 caraml-upi-protos-0.3.4/caraml/upi/v1/type_pb2_grpc.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     6837 2023-02-03 04:20:42.000000 caraml-upi-protos-0.3.4/caraml/upi/v1/upi_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)    11543 2023-02-03 04:20:42.000000 caraml-upi-protos-0.3.4/caraml/upi/v1/upi_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     2741 2023-02-03 04:20:42.000000 caraml-upi-protos-0.3.4/caraml/upi/v1/upi_pb2_grpc.py
--rw-r--r--   0 runner    (1001) docker     (123)      892 2023-02-03 04:20:42.000000 caraml-upi-protos-0.3.4/caraml/upi/v1/upi_pb2_grpc.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     2161 2023-02-03 04:20:42.000000 caraml-upi-protos-0.3.4/caraml/upi/v1/variable_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)     1771 2023-02-03 04:20:42.000000 caraml-upi-protos-0.3.4/caraml/upi/v1/variable_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      159 2023-02-03 04:20:42.000000 caraml-upi-protos-0.3.4/caraml/upi/v1/variable_pb2_grpc.py
--rw-r--r--   0 runner    (1001) docker     (123)       76 2023-02-03 04:20:42.000000 caraml-upi-protos-0.3.4/caraml/upi/v1/variable_pb2_grpc.pyi
--rw-r--r--   0 runner    (1001) docker     (123)       18 2023-02-03 04:20:53.000000 caraml-upi-protos-0.3.4/caraml/upi/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-03 04:20:55.000000 caraml-upi-protos-0.3.4/caraml_upi_protos.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     4736 2023-02-03 04:20:54.000000 caraml-upi-protos-0.3.4/caraml_upi_protos.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1419 2023-02-03 04:20:55.000000 caraml-upi-protos-0.3.4/caraml_upi_protos.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-02-03 04:20:54.000000 caraml-upi-protos-0.3.4/caraml_upi_protos.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      107 2023-02-03 04:20:54.000000 caraml-upi-protos-0.3.4/caraml_upi_protos.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        7 2023-02-03 04:20:54.000000 caraml-upi-protos-0.3.4/caraml_upi_protos.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       83 2023-02-03 04:20:55.000000 caraml-upi-protos-0.3.4/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1002 2023-02-03 04:20:42.000000 caraml-upi-protos-0.3.4/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 02:44:52.000000 caraml-upi-protos-0.3.5/
+-rw-r--r--   0 runner    (1001) docker     (123)     4736 2023-06-26 02:44:52.000000 caraml-upi-protos-0.3.5/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3616 2023-06-26 02:44:36.000000 caraml-upi-protos-0.3.5/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 02:44:52.000000 caraml-upi-protos-0.3.5/caraml/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-26 02:44:36.000000 caraml-upi-protos-0.3.5/caraml/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 02:44:52.000000 caraml-upi-protos-0.3.5/caraml/upi/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-26 02:44:36.000000 caraml-upi-protos-0.3.5/caraml/upi/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6889 2023-06-26 02:44:36.000000 caraml-upi-protos-0.3.5/caraml/upi/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 02:44:52.000000 caraml-upi-protos-0.3.5/caraml/upi/v1/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-26 02:44:36.000000 caraml-upi-protos-0.3.5/caraml/upi/v1/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1813 2023-06-26 02:44:36.000000 caraml-upi-protos-0.3.5/caraml/upi/v1/header_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)      725 2023-06-26 02:44:36.000000 caraml-upi-protos-0.3.5/caraml/upi/v1/header_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      159 2023-06-26 02:44:36.000000 caraml-upi-protos-0.3.5/caraml/upi/v1/header_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (123)       76 2023-06-26 02:44:36.000000 caraml-upi-protos-0.3.5/caraml/upi/v1/header_pb2_grpc.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     5232 2023-06-26 02:44:36.000000 caraml-upi-protos-0.3.5/caraml/upi/v1/observation_log_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5814 2023-06-26 02:44:36.000000 caraml-upi-protos-0.3.5/caraml/upi/v1/observation_log_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     2793 2023-06-26 02:44:36.000000 caraml-upi-protos-0.3.5/caraml/upi/v1/observation_log_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (123)      918 2023-06-26 02:44:36.000000 caraml-upi-protos-0.3.5/caraml/upi/v1/observation_log_pb2_grpc.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     4644 2023-06-26 02:44:36.000000 caraml-upi-protos-0.3.5/caraml/upi/v1/prediction_log_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7920 2023-06-26 02:44:36.000000 caraml-upi-protos-0.3.5/caraml/upi/v1/prediction_log_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      159 2023-06-26 02:44:36.000000 caraml-upi-protos-0.3.5/caraml/upi/v1/prediction_log_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (123)       76 2023-06-26 02:44:36.000000 caraml-upi-protos-0.3.5/caraml/upi/v1/prediction_log_pb2_grpc.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     5586 2023-06-26 02:44:36.000000 caraml-upi-protos-0.3.5/caraml/upi/v1/router_log_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10249 2023-06-26 02:44:36.000000 caraml-upi-protos-0.3.5/caraml/upi/v1/router_log_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      159 2023-06-26 02:44:36.000000 caraml-upi-protos-0.3.5/caraml/upi/v1/router_log_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (123)       76 2023-06-26 02:44:36.000000 caraml-upi-protos-0.3.5/caraml/upi/v1/router_log_pb2_grpc.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     3590 2023-06-26 02:44:36.000000 caraml-upi-protos-0.3.5/caraml/upi/v1/table_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4236 2023-06-26 02:44:36.000000 caraml-upi-protos-0.3.5/caraml/upi/v1/table_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      159 2023-06-26 02:44:36.000000 caraml-upi-protos-0.3.5/caraml/upi/v1/table_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (123)       76 2023-06-26 02:44:36.000000 caraml-upi-protos-0.3.5/caraml/upi/v1/table_pb2_grpc.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     1762 2023-06-26 02:44:36.000000 caraml-upi-protos-0.3.5/caraml/upi/v1/type_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1161 2023-06-26 02:44:36.000000 caraml-upi-protos-0.3.5/caraml/upi/v1/type_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      159 2023-06-26 02:44:36.000000 caraml-upi-protos-0.3.5/caraml/upi/v1/type_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (123)       76 2023-06-26 02:44:36.000000 caraml-upi-protos-0.3.5/caraml/upi/v1/type_pb2_grpc.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     6837 2023-06-26 02:44:36.000000 caraml-upi-protos-0.3.5/caraml/upi/v1/upi_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11543 2023-06-26 02:44:36.000000 caraml-upi-protos-0.3.5/caraml/upi/v1/upi_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     2741 2023-06-26 02:44:36.000000 caraml-upi-protos-0.3.5/caraml/upi/v1/upi_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (123)      892 2023-06-26 02:44:36.000000 caraml-upi-protos-0.3.5/caraml/upi/v1/upi_pb2_grpc.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     2161 2023-06-26 02:44:36.000000 caraml-upi-protos-0.3.5/caraml/upi/v1/variable_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1771 2023-06-26 02:44:36.000000 caraml-upi-protos-0.3.5/caraml/upi/v1/variable_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      159 2023-06-26 02:44:36.000000 caraml-upi-protos-0.3.5/caraml/upi/v1/variable_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (123)       76 2023-06-26 02:44:36.000000 caraml-upi-protos-0.3.5/caraml/upi/v1/variable_pb2_grpc.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)       18 2023-06-26 02:44:50.000000 caraml-upi-protos-0.3.5/caraml/upi/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 02:44:52.000000 caraml-upi-protos-0.3.5/caraml_upi_protos.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     4736 2023-06-26 02:44:52.000000 caraml-upi-protos-0.3.5/caraml_upi_protos.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1419 2023-06-26 02:44:52.000000 caraml-upi-protos-0.3.5/caraml_upi_protos.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-26 02:44:52.000000 caraml-upi-protos-0.3.5/caraml_upi_protos.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      107 2023-06-26 02:44:52.000000 caraml-upi-protos-0.3.5/caraml_upi_protos.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        7 2023-06-26 02:44:52.000000 caraml-upi-protos-0.3.5/caraml_upi_protos.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       83 2023-06-26 02:44:52.000000 caraml-upi-protos-0.3.5/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1002 2023-06-26 02:44:36.000000 caraml-upi-protos-0.3.5/setup.py
```

### Comparing `caraml-upi-protos-0.3.4/PKG-INFO` & `caraml-upi-protos-0.3.5/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: caraml-upi-protos
-Version: 0.3.4
+Version: 0.3.5
 Summary: Generated Python code from caraml-dev/universal-prediction-interface
 Home-page: UNKNOWN
 Author: CaraML Developer
 Author-email: dsp@gojek.com
 License: UNKNOWN
 Description: # CaraML UPI Protos
```

### Comparing `caraml-upi-protos-0.3.4/README.md` & `caraml-upi-protos-0.3.5/README.md`

 * *Files identical despite different names*

### Comparing `caraml-upi-protos-0.3.4/caraml/upi/v1/header_pb2.py` & `caraml-upi-protos-0.3.5/caraml/upi/v1/header_pb2.py`

 * *Files identical despite different names*

### Comparing `caraml-upi-protos-0.3.4/caraml/upi/v1/header_pb2.pyi` & `caraml-upi-protos-0.3.5/caraml/upi/v1/header_pb2.pyi`

 * *Files identical despite different names*

### Comparing `caraml-upi-protos-0.3.4/caraml/upi/v1/observation_log_pb2.py` & `caraml-upi-protos-0.3.5/caraml/upi/v1/observation_log_pb2.py`

 * *Files identical despite different names*

### Comparing `caraml-upi-protos-0.3.4/caraml/upi/v1/observation_log_pb2.pyi` & `caraml-upi-protos-0.3.5/caraml/upi/v1/observation_log_pb2.pyi`

 * *Files identical despite different names*

### Comparing `caraml-upi-protos-0.3.4/caraml/upi/v1/observation_log_pb2_grpc.py` & `caraml-upi-protos-0.3.5/caraml/upi/v1/observation_log_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `caraml-upi-protos-0.3.4/caraml/upi/v1/observation_log_pb2_grpc.pyi` & `caraml-upi-protos-0.3.5/caraml/upi/v1/observation_log_pb2_grpc.pyi`

 * *Files identical despite different names*

### Comparing `caraml-upi-protos-0.3.4/caraml/upi/v1/prediction_log_pb2.py` & `caraml-upi-protos-0.3.5/caraml/upi/v1/prediction_log_pb2.py`

 * *Files identical despite different names*

### Comparing `caraml-upi-protos-0.3.4/caraml/upi/v1/prediction_log_pb2.pyi` & `caraml-upi-protos-0.3.5/caraml/upi/v1/prediction_log_pb2.pyi`

 * *Files identical despite different names*

### Comparing `caraml-upi-protos-0.3.4/caraml/upi/v1/router_log_pb2.py` & `caraml-upi-protos-0.3.5/caraml/upi/v1/router_log_pb2.py`

 * *Files identical despite different names*

### Comparing `caraml-upi-protos-0.3.4/caraml/upi/v1/router_log_pb2.pyi` & `caraml-upi-protos-0.3.5/caraml/upi/v1/router_log_pb2.pyi`

 * *Files identical despite different names*

### Comparing `caraml-upi-protos-0.3.4/caraml/upi/v1/table_pb2.py` & `caraml-upi-protos-0.3.5/caraml/upi/v1/table_pb2.py`

 * *Files identical despite different names*

### Comparing `caraml-upi-protos-0.3.4/caraml/upi/v1/table_pb2.pyi` & `caraml-upi-protos-0.3.5/caraml/upi/v1/table_pb2.pyi`

 * *Files identical despite different names*

### Comparing `caraml-upi-protos-0.3.4/caraml/upi/v1/type_pb2.py` & `caraml-upi-protos-0.3.5/caraml/upi/v1/type_pb2.py`

 * *Files identical despite different names*

### Comparing `caraml-upi-protos-0.3.4/caraml/upi/v1/type_pb2.pyi` & `caraml-upi-protos-0.3.5/caraml/upi/v1/type_pb2.pyi`

 * *Files identical despite different names*

### Comparing `caraml-upi-protos-0.3.4/caraml/upi/v1/upi_pb2.py` & `caraml-upi-protos-0.3.5/caraml/upi/v1/upi_pb2.py`

 * *Files identical despite different names*

### Comparing `caraml-upi-protos-0.3.4/caraml/upi/v1/upi_pb2.pyi` & `caraml-upi-protos-0.3.5/caraml/upi/v1/upi_pb2.pyi`

 * *Files identical despite different names*

### Comparing `caraml-upi-protos-0.3.4/caraml/upi/v1/upi_pb2_grpc.py` & `caraml-upi-protos-0.3.5/caraml/upi/v1/upi_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `caraml-upi-protos-0.3.4/caraml/upi/v1/upi_pb2_grpc.pyi` & `caraml-upi-protos-0.3.5/caraml/upi/v1/upi_pb2_grpc.pyi`

 * *Files identical despite different names*

### Comparing `caraml-upi-protos-0.3.4/caraml/upi/v1/variable_pb2.py` & `caraml-upi-protos-0.3.5/caraml/upi/v1/variable_pb2.py`

 * *Files identical despite different names*

### Comparing `caraml-upi-protos-0.3.4/caraml/upi/v1/variable_pb2.pyi` & `caraml-upi-protos-0.3.5/caraml/upi/v1/variable_pb2.pyi`

 * *Files identical despite different names*

### Comparing `caraml-upi-protos-0.3.4/caraml_upi_protos.egg-info/PKG-INFO` & `caraml-upi-protos-0.3.5/caraml_upi_protos.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: caraml-upi-protos
-Version: 0.3.4
+Version: 0.3.5
 Summary: Generated Python code from caraml-dev/universal-prediction-interface
 Home-page: UNKNOWN
 Author: CaraML Developer
 Author-email: dsp@gojek.com
 License: UNKNOWN
 Description: # CaraML UPI Protos
```

### Comparing `caraml-upi-protos-0.3.4/caraml_upi_protos.egg-info/SOURCES.txt` & `caraml-upi-protos-0.3.5/caraml_upi_protos.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `caraml-upi-protos-0.3.4/setup.py` & `caraml-upi-protos-0.3.5/setup.py`

 * *Files identical despite different names*

