# Comparing `tmp/mesh_common-0.0.3.tar.gz` & `tmp/mesh_common-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mesh_common-0.0.3.tar", max compression
+gzip compressed data, was "mesh_common-0.1.1.tar", max compression
```

## Comparing `mesh_common-0.0.3.tar` & `mesh_common-0.1.1.tar`

### file list

```diff
@@ -1,30 +1,30 @@
--rw-r--r--   0        0        0     1078 2023-06-25 21:16:51.577757 mesh_common-0.0.3/LICENSE.md
--rw-r--r--   0        0        0      352 2023-06-25 21:16:51.577757 mesh_common-0.0.3/README.md
--rw-r--r--   0        0        0     7521 2023-06-25 21:16:51.577757 mesh_common-0.0.3/mesh_common/__init__.py
--rw-r--r--   0        0        0     1810 2023-06-25 21:16:51.577757 mesh_common-0.0.3/mesh_common/aws.py
--rw-r--r--   0        0        0     2976 2023-06-25 21:16:51.577757 mesh_common-0.0.3/mesh_common/concurrency.py
--rw-r--r--   0        0        0     2106 2023-06-25 21:16:51.577757 mesh_common-0.0.3/mesh_common/constants.py
--rw-r--r--   0        0        0    10606 2023-06-25 21:16:51.577757 mesh_common-0.0.3/mesh_common/encoding.py
--rw-r--r--   0        0        0     2139 2023-06-25 21:16:51.577757 mesh_common-0.0.3/mesh_common/env_config.py
--rw-r--r--   0        0        0      745 2023-06-25 21:16:51.577757 mesh_common-0.0.3/mesh_common/fernet.py
--rw-r--r--   0        0        0     1258 2023-06-25 21:16:51.577757 mesh_common-0.0.3/mesh_common/fixtures.py
--rw-r--r--   0        0        0     4671 2023-06-25 21:16:51.577757 mesh_common-0.0.3/mesh_common/httpx_retry_transport.py
--rw-r--r--   0        0        0     1937 2023-06-25 21:16:51.577757 mesh_common-0.0.3/mesh_common/lambdas.py
--rw-r--r--   0        0        0     3537 2023-06-25 21:16:51.577757 mesh_common-0.0.3/mesh_common/oas.py
--rw-r--r--   0        0        0        0 2023-06-25 21:16:51.577757 mesh_common-0.0.3/mesh_common/py.typed
--rw-r--r--   0        0        0     3306 2023-06-25 21:16:51.577757 mesh_common-0.0.3/mesh_common/singletons.py
--rw-r--r--   0        0        0     1565 2023-06-25 21:16:51.577757 mesh_common-0.0.3/mesh_common/sqs_helper.py
--rw-r--r--   0        0        0     6909 2023-06-25 21:16:51.577757 mesh_common-0.0.3/mesh_common/test_helpers.py
--rw-r--r--   0        0        0    10117 2023-06-25 21:16:51.577757 mesh_common-0.0.3/mesh_common/test_helpers_logs.py
--rw-r--r--   0        0        0      732 2023-06-25 21:16:51.577757 mesh_common-0.0.3/mesh_common/text.py
--rw-r--r--   0        0        0     2765 2023-06-25 21:17:14.378035 mesh_common-0.0.3/pyproject.toml
--rw-r--r--   0        0        0        0 2023-06-25 21:16:51.577757 mesh_common-0.0.3/tests/__init__.py
--rw-r--r--   0        0        0     2404 2023-06-25 21:16:51.577757 mesh_common-0.0.3/tests/common_tests.py
--rw-r--r--   0        0        0     6014 2023-06-25 21:16:51.577757 mesh_common-0.0.3/tests/concurrency_tests.py
--rw-r--r--   0        0        0      673 2023-06-25 21:16:51.577757 mesh_common-0.0.3/tests/conftest.py
--rw-r--r--   0        0        0     8775 2023-06-25 21:16:51.577757 mesh_common-0.0.3/tests/encoding_tests.py
--rw-r--r--   0        0        0     1711 2023-06-25 21:16:51.577757 mesh_common-0.0.3/tests/env_config_tests.py
--rw-r--r--   0        0        0     4329 2023-06-25 21:16:51.577757 mesh_common-0.0.3/tests/httpx_retry_transport_tests.py
--rw-r--r--   0        0        0     5638 2023-06-25 21:16:51.577757 mesh_common-0.0.3/tests/singletons_tests.py
--rw-r--r--   0        0        0     1128 2023-06-25 21:16:51.577757 mesh_common-0.0.3/tests/test_helpers_tests.py
--rw-r--r--   0        0        0     1178 1970-01-01 00:00:00.000000 mesh_common-0.0.3/PKG-INFO
+-rw-r--r--   0        0        0     1078 2023-06-26 09:37:47.405002 mesh_common-0.1.1/LICENSE.md
+-rw-r--r--   0        0        0      352 2023-06-26 09:37:47.405002 mesh_common-0.1.1/README.md
+-rw-r--r--   0        0        0     7521 2023-06-26 09:37:47.405002 mesh_common-0.1.1/mesh_common/__init__.py
+-rw-r--r--   0        0        0     1810 2023-06-26 09:37:47.405002 mesh_common-0.1.1/mesh_common/aws.py
+-rw-r--r--   0        0        0     2976 2023-06-26 09:37:47.405002 mesh_common-0.1.1/mesh_common/concurrency.py
+-rw-r--r--   0        0        0     2106 2023-06-26 09:37:47.405002 mesh_common-0.1.1/mesh_common/constants.py
+-rw-r--r--   0        0        0    10606 2023-06-26 09:37:47.405002 mesh_common-0.1.1/mesh_common/encoding.py
+-rw-r--r--   0        0        0     2139 2023-06-26 09:37:47.405002 mesh_common-0.1.1/mesh_common/env_config.py
+-rw-r--r--   0        0        0      745 2023-06-26 09:37:47.405002 mesh_common-0.1.1/mesh_common/fernet.py
+-rw-r--r--   0        0        0     1258 2023-06-26 09:37:47.405002 mesh_common-0.1.1/mesh_common/fixtures.py
+-rw-r--r--   0        0        0     4671 2023-06-26 09:37:47.405002 mesh_common-0.1.1/mesh_common/httpx_retry_transport.py
+-rw-r--r--   0        0        0     1937 2023-06-26 09:37:47.405002 mesh_common-0.1.1/mesh_common/lambdas.py
+-rw-r--r--   0        0        0     3537 2023-06-26 09:37:47.405002 mesh_common-0.1.1/mesh_common/oas.py
+-rw-r--r--   0        0        0        0 2023-06-26 09:37:47.405002 mesh_common-0.1.1/mesh_common/py.typed
+-rw-r--r--   0        0        0     3306 2023-06-26 09:37:47.405002 mesh_common-0.1.1/mesh_common/singletons.py
+-rw-r--r--   0        0        0     1565 2023-06-26 09:37:47.405002 mesh_common-0.1.1/mesh_common/sqs_helper.py
+-rw-r--r--   0        0        0     6909 2023-06-26 09:37:47.405002 mesh_common-0.1.1/mesh_common/test_helpers.py
+-rw-r--r--   0        0        0    10117 2023-06-26 09:37:47.405002 mesh_common-0.1.1/mesh_common/test_helpers_logs.py
+-rw-r--r--   0        0        0      732 2023-06-26 09:37:47.405002 mesh_common-0.1.1/mesh_common/text.py
+-rw-r--r--   0        0        0     2764 2023-06-26 09:38:09.797105 mesh_common-0.1.1/pyproject.toml
+-rw-r--r--   0        0        0        0 2023-06-26 09:37:47.409002 mesh_common-0.1.1/tests/__init__.py
+-rw-r--r--   0        0        0     2404 2023-06-26 09:37:47.409002 mesh_common-0.1.1/tests/common_tests.py
+-rw-r--r--   0        0        0     6014 2023-06-26 09:37:47.409002 mesh_common-0.1.1/tests/concurrency_tests.py
+-rw-r--r--   0        0        0      673 2023-06-26 09:37:47.409002 mesh_common-0.1.1/tests/conftest.py
+-rw-r--r--   0        0        0     8775 2023-06-26 09:37:47.409002 mesh_common-0.1.1/tests/encoding_tests.py
+-rw-r--r--   0        0        0     1711 2023-06-26 09:37:47.409002 mesh_common-0.1.1/tests/env_config_tests.py
+-rw-r--r--   0        0        0     4329 2023-06-26 09:37:47.409002 mesh_common-0.1.1/tests/httpx_retry_transport_tests.py
+-rw-r--r--   0        0        0     5638 2023-06-26 09:37:47.409002 mesh_common-0.1.1/tests/singletons_tests.py
+-rw-r--r--   0        0        0     1128 2023-06-26 09:37:47.409002 mesh_common-0.1.1/tests/test_helpers_tests.py
+-rw-r--r--   0        0        0     1176 1970-01-01 00:00:00.000000 mesh_common-0.1.1/PKG-INFO
```

### Comparing `mesh_common-0.0.3/LICENSE.md` & `mesh_common-0.1.1/LICENSE.md`

 * *Files identical despite different names*

### Comparing `mesh_common-0.0.3/mesh_common/__init__.py` & `mesh_common-0.1.1/mesh_common/__init__.py`

 * *Files identical despite different names*

### Comparing `mesh_common-0.0.3/mesh_common/aws.py` & `mesh_common-0.1.1/mesh_common/aws.py`

 * *Files identical despite different names*

### Comparing `mesh_common-0.0.3/mesh_common/concurrency.py` & `mesh_common-0.1.1/mesh_common/concurrency.py`

 * *Files identical despite different names*

### Comparing `mesh_common-0.0.3/mesh_common/constants.py` & `mesh_common-0.1.1/mesh_common/constants.py`

 * *Files identical despite different names*

### Comparing `mesh_common-0.0.3/mesh_common/encoding.py` & `mesh_common-0.1.1/mesh_common/encoding.py`

 * *Files identical despite different names*

### Comparing `mesh_common-0.0.3/mesh_common/env_config.py` & `mesh_common-0.1.1/mesh_common/env_config.py`

 * *Files identical despite different names*

### Comparing `mesh_common-0.0.3/mesh_common/fernet.py` & `mesh_common-0.1.1/mesh_common/fernet.py`

 * *Files identical despite different names*

### Comparing `mesh_common-0.0.3/mesh_common/fixtures.py` & `mesh_common-0.1.1/mesh_common/fixtures.py`

 * *Files identical despite different names*

### Comparing `mesh_common-0.0.3/mesh_common/httpx_retry_transport.py` & `mesh_common-0.1.1/mesh_common/httpx_retry_transport.py`

 * *Files identical despite different names*

### Comparing `mesh_common-0.0.3/mesh_common/lambdas.py` & `mesh_common-0.1.1/mesh_common/lambdas.py`

 * *Files identical despite different names*

### Comparing `mesh_common-0.0.3/mesh_common/oas.py` & `mesh_common-0.1.1/mesh_common/oas.py`

 * *Files identical despite different names*

### Comparing `mesh_common-0.0.3/mesh_common/singletons.py` & `mesh_common-0.1.1/mesh_common/singletons.py`

 * *Files identical despite different names*

### Comparing `mesh_common-0.0.3/mesh_common/sqs_helper.py` & `mesh_common-0.1.1/mesh_common/sqs_helper.py`

 * *Files identical despite different names*

### Comparing `mesh_common-0.0.3/mesh_common/test_helpers.py` & `mesh_common-0.1.1/mesh_common/test_helpers.py`

 * *Files identical despite different names*

### Comparing `mesh_common-0.0.3/mesh_common/test_helpers_logs.py` & `mesh_common-0.1.1/mesh_common/test_helpers_logs.py`

 * *Files identical despite different names*

### Comparing `mesh_common-0.0.3/mesh_common/text.py` & `mesh_common-0.1.1/mesh_common/text.py`

 * *Files identical despite different names*

### Comparing `mesh_common-0.0.3/pyproject.toml` & `mesh_common-0.1.1/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "mesh_common"
-version = "0.0.3"
+version = "0.1.1"
 description = ""
 authors = ["spinecore"]
 license = "MIT"
 packages = [
     { include = "mesh_common" },
     { include = "tests", format = "sdist" },
 ]
@@ -15,16 +15,16 @@
 python = ">=3.10,<4.0"
 boto3 = "^1.26.159"
 boto3-stubs = {extras = ["s3", "ssm", "secretsmanager", "dynamodb", "sqs", "lambda", "logs", "sns", "events"], version = "^1.26.159"}
 httpx = "^0.24.1"
 types-urllib3 = "^1.26.25.13"
 types-cryptography = "^3.3.23.2"
 types-python-dateutil = "^2.8.19.13"
-nhs-aws-helpers = "^0.0.16"
 nhs-context-logging = "^0.2.3"
+nhs-aws-helpers = "^0.1.1"
 
 [tool.setuptools.package-data]
 "mesh_common" = ["py.typed"]
 
 [tool.poetry.group.dev.dependencies]
 # ci / testing dependencies
 petname = "^2.6"
```

### Comparing `mesh_common-0.0.3/tests/common_tests.py` & `mesh_common-0.1.1/tests/common_tests.py`

 * *Files identical despite different names*

### Comparing `mesh_common-0.0.3/tests/concurrency_tests.py` & `mesh_common-0.1.1/tests/concurrency_tests.py`

 * *Files identical despite different names*

### Comparing `mesh_common-0.0.3/tests/conftest.py` & `mesh_common-0.1.1/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `mesh_common-0.0.3/tests/encoding_tests.py` & `mesh_common-0.1.1/tests/encoding_tests.py`

 * *Files identical despite different names*

### Comparing `mesh_common-0.0.3/tests/env_config_tests.py` & `mesh_common-0.1.1/tests/env_config_tests.py`

 * *Files identical despite different names*

### Comparing `mesh_common-0.0.3/tests/httpx_retry_transport_tests.py` & `mesh_common-0.1.1/tests/httpx_retry_transport_tests.py`

 * *Files identical despite different names*

### Comparing `mesh_common-0.0.3/tests/singletons_tests.py` & `mesh_common-0.1.1/tests/singletons_tests.py`

 * *Files identical despite different names*

### Comparing `mesh_common-0.0.3/tests/test_helpers_tests.py` & `mesh_common-0.1.1/tests/test_helpers_tests.py`

 * *Files identical despite different names*

### Comparing `mesh_common-0.0.3/PKG-INFO` & `mesh_common-0.1.1/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,22 +1,22 @@
 Metadata-Version: 2.1
 Name: mesh-common
-Version: 0.0.3
+Version: 0.1.1
 Summary: 
 License: MIT
 Author: spinecore
 Requires-Python: >=3.10,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Requires-Dist: boto3 (>=1.26.159,<2.0.0)
 Requires-Dist: boto3-stubs[dynamodb,events,lambda,logs,s3,secretsmanager,sns,sqs,ssm] (>=1.26.159,<2.0.0)
 Requires-Dist: httpx (>=0.24.1,<0.25.0)
-Requires-Dist: nhs-aws-helpers (>=0.0.16,<0.0.17)
+Requires-Dist: nhs-aws-helpers (>=0.1.1,<0.2.0)
 Requires-Dist: nhs-context-logging (>=0.2.3,<0.3.0)
 Requires-Dist: types-cryptography (>=3.3.23.2,<4.0.0.0)
 Requires-Dist: types-python-dateutil (>=2.8.19.13,<3.0.0.0)
 Requires-Dist: types-urllib3 (>=1.26.25.13,<2.0.0.0)
 Description-Content-Type: text/markdown
 
 # MESH Common
```

