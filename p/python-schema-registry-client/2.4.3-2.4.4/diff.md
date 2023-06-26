# Comparing `tmp/python-schema-registry-client-2.4.3.tar.gz` & `tmp/python_schema_registry_client-2.4.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "python-schema-registry-client-2.4.3.tar", last modified: Wed Apr 19 13:45:02 2023, max compression
+gzip compressed data, was "python_schema_registry_client-2.4.4.tar", max compression
```

## Comparing `python-schema-registry-client-2.4.3.tar` & `python_schema_registry_client-2.4.4.tar`

### file list

```diff
@@ -1,59 +1,19 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 13:45:02.476534 python-schema-registry-client-2.4.3/
--rw-r--r--   0 runner    (1001) docker     (123)     1079 2023-04-19 13:44:50.000000 python-schema-registry-client-2.4.3/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    12413 2023-04-19 13:45:02.476534 python-schema-registry-client-2.4.3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    11507 2023-04-19 13:44:50.000000 python-schema-registry-client-2.4.3/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      247 2023-04-19 13:44:50.000000 python-schema-registry-client-2.4.3/pyproject.toml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 13:45:02.476534 python-schema-registry-client-2.4.3/python_schema_registry_client.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    12413 2023-04-19 13:45:02.000000 python-schema-registry-client-2.4.3/python_schema_registry_client.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1856 2023-04-19 13:45:02.000000 python-schema-registry-client-2.4.3/python_schema_registry_client.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-19 13:45:02.000000 python-schema-registry-client-2.4.3/python_schema_registry_client.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      278 2023-04-19 13:45:02.000000 python-schema-registry-client-2.4.3/python_schema_registry_client.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       22 2023-04-19 13:45:02.000000 python-schema-registry-client-2.4.3/python_schema_registry_client.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 13:45:02.476534 python-schema-registry-client-2.4.3/schema_registry/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-19 13:44:50.000000 python-schema-registry-client-2.4.3/schema_registry/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 13:45:02.476534 python-schema-registry-client-2.4.3/schema_registry/client/
--rw-r--r--   0 runner    (1001) docker     (123)      215 2023-04-19 13:44:50.000000 python-schema-registry-client-2.4.3/schema_registry/client/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)       92 2023-04-19 13:44:50.000000 python-schema-registry-client-2.4.3/schema_registry/client/auth_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)    55077 2023-04-19 13:44:50.000000 python-schema-registry-client-2.4.3/schema_registry/client/client.py
--rw-r--r--   0 runner    (1001) docker     (123)      471 2023-04-19 13:44:50.000000 python-schema-registry-client-2.4.3/schema_registry/client/errors.py
--rw-r--r--   0 runner    (1001) docker     (123)      801 2023-04-19 13:44:50.000000 python-schema-registry-client-2.4.3/schema_registry/client/paths.py
--rw-r--r--   0 runner    (1001) docker     (123)     4701 2023-04-19 13:44:50.000000 python-schema-registry-client-2.4.3/schema_registry/client/schema.py
--rw-r--r--   0 runner    (1001) docker     (123)     2328 2023-04-19 13:44:50.000000 python-schema-registry-client-2.4.3/schema_registry/client/status.py
--rw-r--r--   0 runner    (1001) docker     (123)     1419 2023-04-19 13:44:50.000000 python-schema-registry-client-2.4.3/schema_registry/client/urls.py
--rw-r--r--   0 runner    (1001) docker     (123)     1039 2023-04-19 13:44:50.000000 python-schema-registry-client-2.4.3/schema_registry/client/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-19 13:44:50.000000 python-schema-registry-client-2.4.3/schema_registry/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 13:45:02.476534 python-schema-registry-client-2.4.3/schema_registry/serializers/
--rw-r--r--   0 runner    (1001) docker     (123)      541 2023-04-19 13:44:50.000000 python-schema-registry-client-2.4.3/schema_registry/serializers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      351 2023-04-19 13:44:50.000000 python-schema-registry-client-2.4.3/schema_registry/serializers/errors.py
--rw-r--r--   0 runner    (1001) docker     (123)     3773 2023-04-19 13:44:50.000000 python-schema-registry-client-2.4.3/schema_registry/serializers/faust.py
--rw-r--r--   0 runner    (1001) docker     (123)    14841 2023-04-19 13:44:50.000000 python-schema-registry-client-2.4.3/schema_registry/serializers/message_serializer.py
--rw-r--r--   0 runner    (1001) docker     (123)      380 2023-04-19 13:45:02.480533 python-schema-registry-client-2.4.3/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2116 2023-04-19 13:44:50.000000 python-schema-registry-client-2.4.3/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 13:45:02.476534 python-schema-registry-client-2.4.3/tests/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 13:45:02.476534 python-schema-registry-client-2.4.3/tests/client/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-19 13:44:50.000000 python-schema-registry-client-2.4.3/tests/client/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 13:45:02.476534 python-schema-registry-client-2.4.3/tests/client/async_client/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-19 13:44:50.000000 python-schema-registry-client-2.4.3/tests/client/async_client/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     4850 2023-04-19 13:44:50.000000 python-schema-registry-client-2.4.3/tests/client/async_client/test_http_client.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1258 2023-04-19 13:44:50.000000 python-schema-registry-client-2.4.3/tests/client/async_client/test_schema.py
--rw-r--r--   0 runner    (1001) docker     (123)     5269 2023-04-19 13:44:50.000000 python-schema-registry-client-2.4.3/tests/client/async_client/test_schema_compatibility.py
--rw-r--r--   0 runner    (1001) docker     (123)     1003 2023-04-19 13:44:50.000000 python-schema-registry-client-2.4.3/tests/client/async_client/test_schema_delete.py
--rw-r--r--   0 runner    (1001) docker     (123)     2325 2023-04-19 13:44:50.000000 python-schema-registry-client-2.4.3/tests/client/async_client/test_schema_getters.py
--rw-r--r--   0 runner    (1001) docker     (123)     9025 2023-04-19 13:44:50.000000 python-schema-registry-client-2.4.3/tests/client/async_client/test_schema_registration.py
--rw-r--r--   0 runner    (1001) docker     (123)     4452 2023-04-19 13:44:50.000000 python-schema-registry-client-2.4.3/tests/client/async_client/test_schema_version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 13:45:02.476534 python-schema-registry-client-2.4.3/tests/client/sync_client/
--rwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 13:44:50.000000 python-schema-registry-client-2.4.3/tests/client/sync_client/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     5798 2023-04-19 13:44:50.000000 python-schema-registry-client-2.4.3/tests/client/sync_client/test_http_client.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     3497 2023-04-19 13:44:50.000000 python-schema-registry-client-2.4.3/tests/client/sync_client/test_schema.py
--rw-r--r--   0 runner    (1001) docker     (123)     4508 2023-04-19 13:44:50.000000 python-schema-registry-client-2.4.3/tests/client/sync_client/test_schema_compatibility.py
--rw-r--r--   0 runner    (1001) docker     (123)      829 2023-04-19 13:44:50.000000 python-schema-registry-client-2.4.3/tests/client/sync_client/test_schema_delete.py
--rw-r--r--   0 runner    (1001) docker     (123)     1962 2023-04-19 13:44:50.000000 python-schema-registry-client-2.4.3/tests/client/sync_client/test_schema_getters.py
--rw-r--r--   0 runner    (1001) docker     (123)     7957 2023-04-19 13:44:50.000000 python-schema-registry-client-2.4.3/tests/client/sync_client/test_schema_registration.py
--rw-r--r--   0 runner    (1001) docker     (123)     3611 2023-04-19 13:44:50.000000 python-schema-registry-client-2.4.3/tests/client/sync_client/test_schema_version.py
--rw-r--r--   0 runner    (1001) docker     (123)     1620 2023-04-19 13:44:50.000000 python-schema-registry-client-2.4.3/tests/client/test_urls.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 13:45:02.476534 python-schema-registry-client-2.4.3/tests/serializer/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-19 13:44:50.000000 python-schema-registry-client-2.4.3/tests/serializer/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     8284 2023-04-19 13:44:50.000000 python-schema-registry-client-2.4.3/tests/serializer/test_async_message_serializer.py
--rw-r--r--   0 runner    (1001) docker     (123)     9806 2023-04-19 13:44:50.000000 python-schema-registry-client-2.4.3/tests/serializer/test_faust_serializer.py
--rw-r--r--   0 runner    (1001) docker     (123)     5131 2023-04-19 13:44:50.000000 python-schema-registry-client-2.4.3/tests/serializer/test_faust_serializer_clean_payload.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     7624 2023-04-19 13:44:50.000000 python-schema-registry-client-2.4.3/tests/serializer/test_message_serializer.py
+-rw-r--r--   0        0        0     1080 2023-06-26 09:17:27.976526 python_schema_registry_client-2.4.4/LICENSE
+-rw-r--r--   0        0        0    11607 2023-06-26 09:17:27.976526 python_schema_registry_client-2.4.4/README.md
+-rw-r--r--   0        0        0     2246 2023-06-26 09:17:27.976526 python_schema_registry_client-2.4.4/pyproject.toml
+-rw-r--r--   0        0        0        0 2023-06-26 09:17:27.976526 python_schema_registry_client-2.4.4/schema_registry/__init__.py
+-rw-r--r--   0        0        0      215 2023-06-26 09:17:27.976526 python_schema_registry_client-2.4.4/schema_registry/client/__init__.py
+-rw-r--r--   0        0        0       92 2023-06-26 09:17:27.976526 python_schema_registry_client-2.4.4/schema_registry/client/auth_utils.py
+-rw-r--r--   0        0        0    55631 2023-06-26 09:17:27.976526 python_schema_registry_client-2.4.4/schema_registry/client/client.py
+-rw-r--r--   0        0        0      535 2023-06-26 09:17:27.976526 python_schema_registry_client-2.4.4/schema_registry/client/errors.py
+-rw-r--r--   0        0        0      801 2023-06-26 09:17:27.976526 python_schema_registry_client-2.4.4/schema_registry/client/paths.py
+-rw-r--r--   0        0        0     4701 2023-06-26 09:17:27.976526 python_schema_registry_client-2.4.4/schema_registry/client/schema.py
+-rw-r--r--   0        0        0     2328 2023-06-26 09:17:27.976526 python_schema_registry_client-2.4.4/schema_registry/client/status.py
+-rw-r--r--   0        0        0     1419 2023-06-26 09:17:27.976526 python_schema_registry_client-2.4.4/schema_registry/client/urls.py
+-rw-r--r--   0        0        0     1039 2023-06-26 09:17:27.976526 python_schema_registry_client-2.4.4/schema_registry/client/utils.py
+-rw-r--r--   0        0        0        0 2023-06-26 09:17:27.976526 python_schema_registry_client-2.4.4/schema_registry/py.typed
+-rw-r--r--   0        0        0      541 2023-06-26 09:17:27.976526 python_schema_registry_client-2.4.4/schema_registry/serializers/__init__.py
+-rw-r--r--   0        0        0      351 2023-06-26 09:17:27.976526 python_schema_registry_client-2.4.4/schema_registry/serializers/errors.py
+-rw-r--r--   0        0        0     3770 2023-06-26 09:17:27.976526 python_schema_registry_client-2.4.4/schema_registry/serializers/faust.py
+-rw-r--r--   0        0        0    18116 2023-06-26 09:17:27.976526 python_schema_registry_client-2.4.4/schema_registry/serializers/message_serializer.py
+-rw-r--r--   0        0        0    12509 1970-01-01 00:00:00.000000 python_schema_registry_client-2.4.4/PKG-INFO
```

### Comparing `python-schema-registry-client-2.4.3/LICENSE` & `python_schema_registry_client-2.4.4/LICENSE`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
 The MIT License (MIT)
-Copyright (c) 2021, Marcos Schroh
+Copyright (c) 2023, Marcos Schroh
 
 Permission is hereby granted, free of charge, to any person obtaining a copy of this software and associated documentation files (the "Software"), to deal in the Software without restriction, including without limitation the rights to use, copy, modify, merge, publish, distribute, sublicense, and/or sell copies of the Software, and to permit persons to whom the Software is furnished to do so, subject to the following conditions:
 
 The above copyright notice and this permission notice shall be included in all copies or substantial portions of the Software.
 
-THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY, FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM, OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE SOFTWARE.
+THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY, FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM, OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE SOFTWARE.
```

### Comparing `python-schema-registry-client-2.4.3/PKG-INFO` & `python_schema_registry_client-2.4.4/README.md`

 * *Files 6% similar despite different names*

```diff
@@ -1,33 +1,10 @@
-Metadata-Version: 2.1
-Name: python-schema-registry-client
-Version: 2.4.3
-Summary: Python Rest Client to interact against Schema Registry Confluent Server to manage Avro Schemas
-Home-page: https://github.com/marcosschroh/python-schema-registry-client
-Author: Marcos Schroh
-Author-email: schrohm@gmail.com
-License: MIT
-Download-URL: https://pypi.org/project/python-schema-registry-client/#files
-Keywords: Schema Registry,Python,Avro,Apache,Apache Avro,JSON,JSON Schema
-Platform: UNKNOWN
-Classifier: Intended Audience :: Developers
-Classifier: License :: OSI Approved :: MIT License
-Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.7
-Classifier: Programming Language :: Python :: 3 :: Only
-Classifier: Topic :: Software Development
-Description-Content-Type: text/markdown
-Provides-Extra: docs
-Provides-Extra: faust
-Provides-Extra: tests
-License-File: LICENSE
-
 # Python Rest Client Schema Registry
 
-[![Build Status](https://img.shields.io/endpoint.svg?url=https%3A%2F%2Factions-badge.atrox.dev%2Fmarcosschroh%2Fpython-schema-registry-client%2Fbadge%3Fref%3Dmaster&style=flat)](https://actions-badge.atrox.dev/marcosschroh/python-schema-registry-client/goto?ref=master)
+[![Python package](https://github.com/marcosschroh/python-schema-registry-client/actions/workflows/python-package.yml/badge.svg)](https://github.com/marcosschroh/python-schema-registry-client/actions/workflows/python-package.yml)
 [![GitHub license](https://img.shields.io/github/license/marcosschroh/python-schema-registry-client.svg)](https://github.com/marcosschroh/python-schema-registry-client/blob/master/LICENSE)
 [![codecov](https://codecov.io/gh/marcosschroh/python-schema-registry-client/branch/master/graph/badge.svg)](https://codecov.io/gh/marcosschroh/python-schema-registry-client)
 [![Python Version](https://img.shields.io/badge/python-3.7+-blue.svg)](https://img.shields.io/badge/python-3.7+-blue.svg)
 
 Python Rest Client to interact against [schema-registry](https://docs.confluent.io/current/schema-registry/index.html) confluent server to manage [Avro](https://docs.oracle.com/database/nosql-12.1.3.1/GettingStartedGuide/avroschemas.html) and [JSON](https://json-schema.org/) schemas resources.
 
 ## Requirements
@@ -337,51 +314,44 @@
 
 So, our producers/consumers have to serialize/deserialize messages every time that they send/receive from Kafka topics. In this picture, we can imagine a `Faust` application receiving messages (encoded with an Avro schema) and we want to deserialize them, so we can ask the `schema server` to do that for us. In this scenario, the `MessageSerializer` is perfect.
 
 Also, could be a use case that we would like to have an Application only to administrate `Avro Schemas` (register, update compatibilities, delete old schemas, etc.), so the `SchemaRegistryClient` is perfect.
 
 ## Development
 
-Install the project and development utilities in edit mode:
+[Poetry](https://python-poetry.org/docs/) is needed to install the dependencies and develope locally
 
-```bash
-pip3 install -e ".[tests,docs,faust]"
-```
+1. Install dependencies: `poetry install --all-extras`
+2. Code linting: `./scripts/format`
+3. Run tests: `./scripts/test`
 
-The tests are run against the `Schema Server` using `docker compose`, so you will need
-`Docker` and `Docker Compose` installed.
+For commit messages we use [commitizen](https://commitizen-tools.github.io/commitizen/) in order to standardize a way of committing rules
 
-```bash
-./scripts/test
-```
+*Note*: The tests are run against the `Schema Server` using `docker compose`, so you will need
+`Docker` and `Docker Compose` installed.
 
-You can run tests with arbitrary python version by:
+In a terminal run `docker-compose up`. Then in a different terminal run the tests:
 
 ```bash
-./scripts/test --python-version 3.x
+./scripts/test
 ```
 
 All additional args will be passed to pytest, for example:
 
 ```bash
-./scripts/test ./tests/client/ --maxfail=1 
+./scripts/test ./tests/client/
 ```
 
-Run code linting:
-
-```bash
-./scripts/lint
-```
+### Tests usind the python shell
 
 To perform tests using the python shell you can run the project using `docker-compose`.
 
-1. Build: `docker-compose build --build-arg PYTHON_VERSION=$PYTHON_VERSION`
-2. Execute `docker-compose up`. Then, the `schema registry server` will run on `http://127.0.0.1:8081`, then you can interact against it using the `SchemaRegistryClient`:
-3. Use the python interpreter (get a python shell typing `python` in your command line)
-4. Play with the `schema server`
+1. Execute `docker-compose up`. Then, the `schema registry server` will run on `http://127.0.0.1:8081`, then you can interact against it using the `SchemaRegistryClient`:
+1. Use the python interpreter (get a python shell typing `python` in your command line)
+1. Play with the `schema server`
 
 ```python
 from schema_registry.client import SchemaRegistryClient, schema
 
 client = SchemaRegistryClient(url="http://127.0.0.1:8081")
 
 # do some operations with the client...
@@ -398,9 +368,7 @@
 
 avro_schema = schema.AvroSchema(deployment_schema)
 client.register("test-deployment", avro_schema)
 # >>>> Out[5]: 1
 ```
 
 Then, you can check the schema using your browser going to the url `http://127.0.0.1:8081/schemas/ids/1`
-
-
```

### Comparing `python-schema-registry-client-2.4.3/README.md` & `python_schema_registry_client-2.4.4/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,33 @@
+Metadata-Version: 2.1
+Name: python-schema-registry-client
+Version: 2.4.4
+Summary: Python Rest Client to interact against Schema Registry confluent server
+License: MIT
+Author: Marcos Schroh
+Author-email: schrohm@gmail.com
+Requires-Python: >=3.7,<4.0
+Classifier: License :: OSI Approved :: MIT License
+Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.7
+Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
+Provides-Extra: faust
+Requires-Dist: aiofiles (>=23.1.0,<24.0.0)
+Requires-Dist: fastavro (>=1.7.3,<2.0.0)
+Requires-Dist: faust-streaming (>=0.10.11,<0.11.0) ; extra == "faust"
+Requires-Dist: httpx (>=0.24.0,<0.25.0)
+Requires-Dist: jsonschema (>=4.17.3,<5.0.0)
+Description-Content-Type: text/markdown
+
 # Python Rest Client Schema Registry
 
-[![Build Status](https://img.shields.io/endpoint.svg?url=https%3A%2F%2Factions-badge.atrox.dev%2Fmarcosschroh%2Fpython-schema-registry-client%2Fbadge%3Fref%3Dmaster&style=flat)](https://actions-badge.atrox.dev/marcosschroh/python-schema-registry-client/goto?ref=master)
+[![Python package](https://github.com/marcosschroh/python-schema-registry-client/actions/workflows/python-package.yml/badge.svg)](https://github.com/marcosschroh/python-schema-registry-client/actions/workflows/python-package.yml)
 [![GitHub license](https://img.shields.io/github/license/marcosschroh/python-schema-registry-client.svg)](https://github.com/marcosschroh/python-schema-registry-client/blob/master/LICENSE)
 [![codecov](https://codecov.io/gh/marcosschroh/python-schema-registry-client/branch/master/graph/badge.svg)](https://codecov.io/gh/marcosschroh/python-schema-registry-client)
 [![Python Version](https://img.shields.io/badge/python-3.7+-blue.svg)](https://img.shields.io/badge/python-3.7+-blue.svg)
 
 Python Rest Client to interact against [schema-registry](https://docs.confluent.io/current/schema-registry/index.html) confluent server to manage [Avro](https://docs.oracle.com/database/nosql-12.1.3.1/GettingStartedGuide/avroschemas.html) and [JSON](https://json-schema.org/) schemas resources.
 
 ## Requirements
@@ -314,51 +337,44 @@
 
 So, our producers/consumers have to serialize/deserialize messages every time that they send/receive from Kafka topics. In this picture, we can imagine a `Faust` application receiving messages (encoded with an Avro schema) and we want to deserialize them, so we can ask the `schema server` to do that for us. In this scenario, the `MessageSerializer` is perfect.
 
 Also, could be a use case that we would like to have an Application only to administrate `Avro Schemas` (register, update compatibilities, delete old schemas, etc.), so the `SchemaRegistryClient` is perfect.
 
 ## Development
 
-Install the project and development utilities in edit mode:
+[Poetry](https://python-poetry.org/docs/) is needed to install the dependencies and develope locally
 
-```bash
-pip3 install -e ".[tests,docs,faust]"
-```
+1. Install dependencies: `poetry install --all-extras`
+2. Code linting: `./scripts/format`
+3. Run tests: `./scripts/test`
 
-The tests are run against the `Schema Server` using `docker compose`, so you will need
-`Docker` and `Docker Compose` installed.
+For commit messages we use [commitizen](https://commitizen-tools.github.io/commitizen/) in order to standardize a way of committing rules
 
-```bash
-./scripts/test
-```
+*Note*: The tests are run against the `Schema Server` using `docker compose`, so you will need
+`Docker` and `Docker Compose` installed.
 
-You can run tests with arbitrary python version by:
+In a terminal run `docker-compose up`. Then in a different terminal run the tests:
 
 ```bash
-./scripts/test --python-version 3.x
+./scripts/test
 ```
 
 All additional args will be passed to pytest, for example:
 
 ```bash
-./scripts/test ./tests/client/ --maxfail=1 
+./scripts/test ./tests/client/
 ```
 
-Run code linting:
-
-```bash
-./scripts/lint
-```
+### Tests usind the python shell
 
 To perform tests using the python shell you can run the project using `docker-compose`.
 
-1. Build: `docker-compose build --build-arg PYTHON_VERSION=$PYTHON_VERSION`
-2. Execute `docker-compose up`. Then, the `schema registry server` will run on `http://127.0.0.1:8081`, then you can interact against it using the `SchemaRegistryClient`:
-3. Use the python interpreter (get a python shell typing `python` in your command line)
-4. Play with the `schema server`
+1. Execute `docker-compose up`. Then, the `schema registry server` will run on `http://127.0.0.1:8081`, then you can interact against it using the `SchemaRegistryClient`:
+1. Use the python interpreter (get a python shell typing `python` in your command line)
+1. Play with the `schema server`
 
 ```python
 from schema_registry.client import SchemaRegistryClient, schema
 
 client = SchemaRegistryClient(url="http://127.0.0.1:8081")
 
 # do some operations with the client...
@@ -375,7 +391,8 @@
 
 avro_schema = schema.AvroSchema(deployment_schema)
 client.register("test-deployment", avro_schema)
 # >>>> Out[5]: 1
 ```
 
 Then, you can check the schema using your browser going to the url `http://127.0.0.1:8081/schemas/ids/1`
+
```

### Comparing `python-schema-registry-client-2.4.3/schema_registry/client/client.py` & `python_schema_registry_client-2.4.4/schema_registry/client/client.py`

 * *Files 9% similar despite different names*

```diff
@@ -36,42 +36,40 @@
     )
 
 
 class BaseClient:
     """
     A client that talks to a Schema Registry over HTTP
 
-    **Parameters:**
-
-    * **url** - (str|dict) url: Url to schema registry or dictionary containing client configuration.
-    * **ca_location** - *(optional str)* File or directory path to CA certificate(s)
-        for verifying the Schema Registry key.
-    * **cert_location** - *(optional str)* Path to public key used for authentication.
-    * **key_location** - *(optional str)* Path to private key used for authentication.
-    * **key_password** - *(optional str)* Key password
-    * **extra_headers** - *(optional dict)* Extra headers to add on every requests.
-    * **timeout** - *(optional)* (httpx._client.TimeoutTypes) The timeout configuration to use when sending requests.
-    * **pool_limits** - *(optional)* (httpx.Limits) The connection pool configuration to use when
-        determining the maximum number of concurrently open HTTP connections.
-    * **auth** - *(optional)* (schema_registry.client.Auth) Auth credentials.
+    Attributes:
+        url str | typing.Dict: Url to schema registry or dictionary containing client configuration.
+        ca_location str | None: File or directory path to CA certificate(s)
+            for verifying the Schema Registry key.
+        cert_location str | None: Path to public key used for authentication.
+        key_location str | None: Path to private key used for authentication.
+        key_password str | None: Key password
+        extra_headers str | None: Extra headers to add on every requests.
+        timeout httpx.Timeout | None: The timeout configuration to use when sending requests.
+        pool_limits httpx.Limits | None: The connection pool configuration to use when
+            determining the maximum number of concurrently open HTTP connections.
+        auth auth_utils.Auth | None: Auth credentials.
     """
 
     def __init__(
         self,
-        url: typing.Union[str, dict],
-        ca_location: str = None,
-        cert_location: str = None,
-        key_location: str = None,
-        key_password: str = None,
-        extra_headers: dict = None,
+        url: typing.Union[str, typing.Dict],
+        ca_location: typing.Optional[str] = None,
+        cert_location: typing.Optional[str] = None,
+        key_location: typing.Optional[str] = None,
+        key_password: typing.Optional[str] = None,
+        extra_headers: typing.Optional[typing.Dict] = None,
         timeout: typing.Optional[httpx.Timeout] = None,
         pool_limits: typing.Optional[httpx.Limits] = None,
         auth: typing.Optional[auth_utils.Auth] = None,
     ) -> None:
-
         if isinstance(url, str):
             conf = {
                 utils.URL: url,
                 utils.SSL_CA_LOCATION: ca_location,
                 utils.SSL_CERTIFICATE_LOCATION: cert_location,
                 utils.SSL_KEY_LOCATION: key_location,
                 utils.SSL_KEY_PASSWORD: key_password,
@@ -96,18 +94,17 @@
         self.id_to_schema: dict = defaultdict(dict)
         # Cache Schemas: subj => { schema => version }
         self.subject_to_schema_versions: dict = defaultdict(dict)
 
     def __eq__(self, obj: typing.Any) -> bool:
         return self.conf == obj.conf and self.extra_headers == obj.extra_headers
 
-
     @staticmethod
-    def _schema_from_result(result: dict) -> typing.Union[JsonSchema, AvroSchema]:
-        schema = result.get("schema")
+    def _schema_from_result(result: typing.Dict) -> typing.Union[JsonSchema, AvroSchema]:
+        schema: str = result["schema"]
         schema_type = result.get("schemaType", utils.AVRO_SCHEMA_TYPE)
         return SchemaFactory.create_schema(schema, schema_type)
 
     def _configure_auth(self) -> typing.Tuple[str, str]:
         # Check first if the credentials are sent in Auth
         if self.auth is not None:
             return (
@@ -180,15 +177,17 @@
         if self.timeout is not None:
             client_kwargs["timeout"] = self.timeout  # type:ignore
 
         if self.pool_limits is not None:
             client_kwargs["limits"] = self.pool_limits  # type:ignore
         return client_kwargs
 
-    def prepare_headers(self, body: dict = None, headers: dict = None) -> dict:
+    def prepare_headers(
+        self, body: typing.Optional[typing.Dict] = None, headers: typing.Optional[typing.Dict] = None
+    ) -> dict:
         _headers = {"Accept": utils.ACCEPT_HEADERS}
 
         if body:
             _headers["Content-Type"] = utils.HEADERS
 
         if headers:
             _headers.update(headers)
@@ -202,16 +201,16 @@
         sub_cache = cache[subject]
         sub_cache[schema] = value
 
     def _cache_schema(
         self,
         schema: typing.Union[BaseSchema, str],
         schema_id: int,
-        subject: str = None,
-        version: typing.Union[str, int] = None,
+        subject: typing.Optional[str] = None,
+        version: typing.Union[str, int, None] = None,
     ) -> None:
         if schema_id in self.id_to_schema:
             schema = self.id_to_schema[schema_id]
         else:
             self.id_to_schema[schema_id] = schema
 
         if subject:
@@ -220,90 +219,108 @@
                 self._add_to_cache(self.subject_to_schema_versions, subject, schema, version)
 
     @abstractmethod
     def request(
         self,
         url: str,
         method: str = "GET",
-        body: dict = None,
-        headers: dict = None,
+        body: typing.Optional[typing.Dict] = None,
+        headers: typing.Optional[typing.Dict] = None,
         timeout: typing.Union[TimeoutTypes, UseClientDefault] = USE_CLIENT_DEFAULT,
     ) -> typing.Union[tuple, httpx.Response, typing.Coroutine[typing.Any, typing.Any, typing.Any]]:
         _headers = self.prepare_headers(body=body, headers=headers)
         with httpx.Client(**self.client_kwargs) as client:
             response = client.request(method, url, headers=_headers, json=body, timeout=timeout)
         return response
 
 
 class SchemaRegistryClient(BaseClient):
     """
     A client that talks to a Schema Registry over HTTP
 
-    **Parameters:**
+    !!! Examlple
+        ```python title="Usage"
+        from schema_registry.client import SchemaRegistryClient, schema
+
+        client = SchemaRegistryClient(url="http://127.0.0.1:8081")
+
+        deployment_schema = {
+            "type": "record",
+            "namespace": "com.kubertenes",
+            "name": "AvroDeployment",
+            "fields": [
+                {"name": "image", "type": "string"},
+                {"name": "replicas", "type": "int"},
+                {"name": "port", "type": "int"},
+            ],
+        }
 
-    * **url** - *(Union[str, Dict]*: Url to schema registry or dictionary containing client configuration.
-    * **ca_location** - *Optional[str]*: File or directory path to CA certificate(s) for
-        verifying the Schema Registry key.
-    * **cert_location** - *Optional[str]*: Path to public key used for authentication.
-    * **key_location** - *Optional[str]*: Path to private key used for authentication.
-    * **key_password** - *Optional[str]*: Key password.
-    * **extra_headers** - *Optional[Dict[str, str]]*: Extra headers to add on every requests.
-    * **timeout** - *Optional[httpx._client.TimeoutTypes]*  The timeout configuration to use when sending requests.
-    * **pool_limits** - *Optional[httpx.Limits])* The connection pool configuration to use when
-        determining the maximum number of concurrently open HTTP connections.
-    * **auth** - *(optional)* (schema_registry.client.Auth) Auth credentials.
+        avro_schema = schema.AvroSchema(deployment_schema)
+        schema_id = client.register("test-deployment", avro_schema)
+        ```
+
+    Attributes:
+        url str | typing.Dict: Url to schema registry or dictionary containing client configuration.
+        ca_location str | None: File or directory path to CA certificate(s)
+            for verifying the Schema Registry key.
+        cert_location str | None: Path to public key used for authentication.
+        key_location str | None: Path to private key used for authentication.
+        key_password str | None: Key password
+        extra_headers str | None: Extra headers to add on every requests.
+        timeout httpx.Timeout | None: The timeout configuration to use when sending requests.
+        pool_limits httpx.Limits | None: The connection pool configuration to use when
+            determining the maximum number of concurrently open HTTP connections.
+        auth auth_utils.Auth | None: Auth credentials.
     """
 
     def request(
         self,
         url: str,
         method: str = "GET",
-        body: dict = None,
-        headers: dict = None,
+        body: typing.Optional[typing.Dict] = None,
+        headers: typing.Optional[typing.Dict] = None,
         timeout: typing.Union[TimeoutTypes, UseClientDefault] = USE_CLIENT_DEFAULT,
     ) -> httpx.Response:
         if method not in utils.VALID_METHODS:
             raise ClientError(f"Method {method} is invalid; valid methods include {utils.VALID_METHODS}")
 
         _headers = self.prepare_headers(body=body, headers=headers)
         with httpx.Client(**self.client_kwargs) as client:
             response = client.request(method, url, headers=_headers, json=body, timeout=timeout)
         return response
 
     def register(
         self,
         subject: str,
         schema: typing.Union[BaseSchema, str],
-        headers: dict = None,
+        headers: typing.Optional[typing.Dict] = None,
         timeout: typing.Union[TimeoutTypes, UseClientDefault] = USE_CLIENT_DEFAULT,
         schema_type: str = utils.AVRO_SCHEMA_TYPE,
     ) -> int:
         """
         Register a schema for a subject
 
         Schema can be avro or json, and can be presented as a parsed schema or a string.
         If schema is a string, the `schema_type` kwarg must be used to indicate
-        what type of schema the string is ("AVRO" by default).
+        what type of schema the string is (`AVRO` by default).
         If the schema is already parsed, the schema_type is inferred directly from the parsed schema.
         Multiple instances of the same schema will result in cache misses.
 
-        **Parameters:**
-
-        * **subject** - str: subject name
-        * **schema** - typing.Union[client.schema.BaseSchema, str]: Avro or JSON
-            schema to be registered
-        * **headers** - Dict: Extra headers to add on the requests
-        * **timeout** - Union[TimeoutTypes, UseClientDefault]: The timeout configuration
-            to use when sending requests. Default USE_CLIENT_DEFAULT
-        * **schema_type** - typing.Union["AVRO", "JSON"]: The type of schema to
-            parse if `schema` is a string. Default "AVRO"
-
-        **Returns:**
+        Attributes:
+            subject str: subject name
+            schema typing.Union[client.schema.BaseSchema, str]: Avro or JSON
+                schema to be registered
+            headers Dict: Extra headers to add on the requests
+            timeout Union[TimeoutTypes, UseClientDefault]: The timeout configuration
+                to use when sending requests. Default USE_CLIENT_DEFAULT
+            schema_type typing.Union[AVRO, JSON]: The type of schema to
+                parse if `schema` is a string. Default "AVRO"
 
-        * **int** - schema_id
+        Returns:
+            schema_id
         """
         schemas_to_id = self.subject_to_schema_ids[subject]
 
         if isinstance(schema, str):
             schema = SchemaFactory.create_schema(schema, schema_type)
 
         schema_id = schemas_to_id.get(schema)
@@ -342,87 +359,88 @@
 
         schema_id = result["id"]
         self._cache_schema(schema, schema_id, subject)
 
         return schema_id
 
     def get_subjects(
-        self, headers: dict = None, timeout: typing.Union[TimeoutTypes, UseClientDefault] = USE_CLIENT_DEFAULT
+        self,
+        headers: typing.Optional[typing.Dict] = None,
+        timeout: typing.Union[TimeoutTypes, UseClientDefault] = USE_CLIENT_DEFAULT,
     ) -> list:
         """
         GET /subjects/(string: subject)
         Get list of all registered subjects in your Schema Registry.
 
-        Args:
-            subject (str): subject name
-            headers (dict): Extra headers to add on the requests
-            timeout (httpx._client.TimeoutTypes): The timeout configuration to use when sending requests.
+        Attributes:
+            subject str: subject name
+            headers typing.Dict: Extra headers to add on the requests
+            timeout httpx._client.TimeoutTypes: The timeout configuration to use when sending requests.
                     Default USE_CLIENT_DEFAULT
 
-
         Returns:
-            list [str]: list of registered subjects.
+            List of registered subjects.
         """
         url, method = self.url_manager.url_for("get_subjects")
         result, code = get_response_and_status_code(self.request(url, method=method, headers=headers, timeout=timeout))
 
         if status.is_success(code):
             return result
 
         raise ClientError("Unable to get subjects", http_code=code, server_traceback=result)
 
     def delete_subject(
         self,
         subject: str,
-        headers: dict = None,
+        headers: typing.Optional[typing.Dict] = None,
         timeout: typing.Union[TimeoutTypes, UseClientDefault] = USE_CLIENT_DEFAULT,
     ) -> list:
         """
         DELETE /subjects/(string: subject)
         Deletes the specified subject and its associated compatibility level if registered.
         It is recommended to use this API only when a topic needs to be
         recycled or in development environments.
 
-        Args:
-            subject (str): subject name
-            headers (dict): Extra headers to add on the requests
-            timeout (httpx._client.TimeoutTypes): The timeout configuration to use when sending requests.
+        Attributes:
+            subject str: subject name
+            headers dict: Extra headers to add on the requests
+            timeout httpx._client.TimeoutTypes: The timeout configuration to use when sending requests.
              Default USE_CLIENT_DEFAULT
 
         Returns:
-            list (int): version of the schema deleted under this subject
+            List version of the schema deleted under this subject
         """
         url, method = self.url_manager.url_for("delete_subject", subject=subject)
         result, code = get_response_and_status_code(self.request(url, method=method, headers=headers, timeout=timeout))
 
         if status.is_success(code):
             return result
         elif code == status.HTTP_404_NOT_FOUND:
             return []
 
         raise ClientError("Unable to delete subject", http_code=code, server_traceback=result)
 
     def get_by_id(
         self,
         schema_id: int,
-        headers: dict = None,
+        headers: typing.Optional[typing.Dict] = None,
         timeout: typing.Union[TimeoutTypes, UseClientDefault] = USE_CLIENT_DEFAULT,
     ) -> typing.Optional[typing.Union[AvroSchema, JsonSchema]]:
         """
         GET /schemas/ids/{int: id}
         Retrieve a parsed avro schema by id or None if not found
 
-        Args:
-            schema_id (int): Schema Id
-            headers (dict): Extra headers to add on the requests
-            timeout (httpx._client.TimeoutTypes): The timeout configuration to use when sending requests.
-            Default USE_CLIENT_DEFAULT
+        Attributes:
+            schema_id int: Schema Id
+            headers dict: Extra headers to add on the requests
+            timeout httpx._client.TimeoutTypes: The timeout configuration to use when sending requests.
+                Default USE_CLIENT_DEFAULT
 
         Returns:
-            typing.Union[client.schema.AvroSchema, client.schema.JsonSchema]: Avro or JSON Record schema
+            Avro or JSON schema
         """
         if schema_id in self.id_to_schema:
             return self.id_to_schema[schema_id]
 
         url, method = self.url_manager.url_for("get_by_id", schema_id=schema_id)
 
         result, code = get_response_and_status_code(self.request(url, method=method, headers=headers, timeout=timeout))
@@ -435,29 +453,29 @@
             return schema
 
         raise ClientError(f"Received bad schema (id {schema_id})", http_code=code, server_traceback=result)
 
     def get_schema_subject_versions(
         self,
         schema_id: int,
-        headers: dict = None,
+        headers: typing.Optional[typing.Dict] = None,
         timeout: typing.Union[TimeoutTypes, UseClientDefault] = USE_CLIENT_DEFAULT,
     ) -> typing.Optional[typing.List[SubjectVersion]]:
         """
         GET /schemas/ids/{int: id}/versions
         Get the subject-version pairs identified by the input ID.
 
-        Args:
-            schema_id (int): Schema Id
-            headers (dict): Extra headers to add on the requests
-            timeout (httpx._client.TimeoutTypes): The timeout configuration to use when sending requests.
+        Attributes:
+            schema_id int: Schema Id
+            headers dict: Extra headers to add on the requests
+            timeout httpx._client.TimeoutTypes: The timeout configuration to use when sending requests.
                     Default USE_CLIENT_DEFAULT
 
         Returns:
-            typing.List[SubjectVersion]: List of Subject/Version pairs where Schema Id is registered
+            List of Subject/Version pairs where Schema Id is registered
         """
         url, method = self.url_manager.url_for("get_schema_subject_versions", schema_id=schema_id)
         result, code = get_response_and_status_code(self.request(url, method=method, headers=headers, timeout=timeout))
         if code == status.HTTP_404_NOT_FOUND:
             logger.warning(f"Schema {schema_id} not found: {code}")
             return None
         elif status.is_success(code):
@@ -468,35 +486,30 @@
 
         raise ClientError(f"Received bad schema (id {schema_id})", http_code=code, server_traceback=result)
 
     def get_schema(
         self,
         subject: str,
         version: typing.Union[int, str] = "latest",
-        headers: dict = None,
+        headers: typing.Optional[typing.Dict] = None,
         timeout: typing.Union[TimeoutTypes, UseClientDefault] = USE_CLIENT_DEFAULT,
     ) -> typing.Optional[utils.SchemaVersion]:
         """
         GET /subjects/(string: subject)/versions/(versionId: version)
         Get a specific version of the schema registered under this subject
 
-        Args:
-            subject (str): subject name
-            version (int, optional): version id. If is None, the latest schema is returned
-            headers (dict): Extra headers to add on the requests
-            timeout (httpx._client.TimeoutTypes): The timeout configuration to use when sending requests.
+        Attributes:
+            subject str: subject name
+            version int, optional: version id. If is None, the latest schema is returned
+            headers dict: Extra headers to add on the requests
+            timeout httpx._client.TimeoutTypes: The timeout configuration to use when sending requests.
              Default USE_CLIENT_DEFAULT
 
         Returns:
-            SchemaVersion (nametupled): (subject, schema_id, schema, version)
-
-            None: If server returns a not success response:
-                404: Schema not found
-                422: Unprocessable entity
-                ~ (200 - 299): Not success
+            The SchemaVersion utils.SchemaVersion if response was succeded
         """
         url, method = self.url_manager.url_for("get_schema", subject=subject, version=version)
 
         result, code = get_response_and_status_code(self.request(url, method=method, headers=headers, timeout=timeout))
         if code == status.HTTP_404_NOT_FOUND:
             logger.info(f"Schema version {version} under subjet {subject} not found: {code}")
             return None
@@ -517,29 +530,29 @@
         self._cache_schema(schema, schema_id, subject, version)
 
         return utils.SchemaVersion(subject, schema_id, schema, version)
 
     def get_versions(
         self,
         subject: str,
-        headers: dict = None,
+        headers: typing.Optional[typing.Dict] = None,
         timeout: typing.Union[TimeoutTypes, UseClientDefault] = USE_CLIENT_DEFAULT,
     ) -> list:
         """
         GET subjects/{subject}/versions
         Get a list of versions registered under the specified subject.
 
-        Args:
-            subject (str): subject name
-            headers (dict): Extra headers to add on the requests
-            timeout (httpx._client.TimeoutTypes): The timeout configuration to use when sending requests.
+        Attributes:
+            subject str: subject name
+            headers dict: Extra headers to add on the requests
+            timeout httpx._client.TimeoutTypes: The timeout configuration to use when sending requests.
                 Default USE_CLIENT_DEFAULT
 
         Returns:
-            list (str): version of the schema registered under this subject
+            List  version of the schema registered under this subject
         """
         url, method = self.url_manager.url_for("get_versions", subject=subject)
 
         result, code = get_response_and_status_code(self.request(url, method=method, headers=headers, timeout=timeout))
         if status.is_success(code):
             return result
         elif code == status.HTTP_404_NOT_FOUND:
@@ -548,38 +561,37 @@
 
         raise ClientError(f"Unable to get the versions for subject {subject}", http_code=code, server_traceback=result)
 
     def delete_version(
         self,
         subject: str,
         version: typing.Union[int, str] = "latest",
-        headers: dict = None,
+        headers: typing.Optional[typing.Dict] = None,
         timeout: typing.Union[TimeoutTypes, UseClientDefault] = USE_CLIENT_DEFAULT,
     ) -> typing.Optional[int]:
         """
         DELETE /subjects/(string: subject)/versions/(versionId: version)
         Deletes a specific version of the schema registered under this subject.
         This only deletes the version and the schema ID remains intact making
         it still possible to decode data using the schema ID.
         This API is recommended to be used only in development environments or
         under extreme circumstances where-in, its required to delete a previously
         registered schema for compatibility purposes or re-register previously registered schema.
 
-        Args:
-            subject (str): subject name
-            version (str): Version of the schema to be deleted.
+        Attributes:
+            subject str: subject name
+            version str: Version of the schema to be deleted.
                 Valid values for versionId are between [1,2^31-1] or the string "latest".
                 "latest" deletes the last registered schema under the specified subject.
-            headers (dict): Extra headers to add on the requests
-            timeout (httpx._client.TimeoutTypes): The timeout configuration to use when sending requests.
+            headers typing.Dict: Extra headers to add on the requests
+            timeout httpx._client.TimeoutTypes: The timeout configuration to use when sending requests.
                     Default USE_CLIENT_DEFAULT
 
         Returns:
-            int: version of the schema deleted
-            None: If the subject or version does not exist.
+            Version of the schema deleted. If the subject or version does not exist.
         """
         url, method = self.url_manager.url_for("delete_version", subject=subject, version=version)
 
         result, code = get_response_and_status_code(self.request(url, method=method, headers=headers, timeout=timeout))
 
         if status.is_success(code):
             return result
@@ -588,39 +600,35 @@
 
         raise ClientError("Unable to delete the version", http_code=code, server_traceback=result)
 
     def check_version(
         self,
         subject: str,
         schema: typing.Union[BaseSchema, str],
-        headers: dict = None,
+        headers: typing.Optional[typing.Dict] = None,
         timeout: typing.Union[TimeoutTypes, UseClientDefault] = USE_CLIENT_DEFAULT,
         schema_type: str = utils.AVRO_SCHEMA_TYPE,
     ) -> typing.Optional[utils.SchemaVersion]:
         """
         POST /subjects/(string: subject)
         Check if a schema has already been registered under the specified subject.
         If so, this returns the schema string along with its globally unique identifier,
         its version under this subject and the subject name.
 
-        Args:
-            subject (str):
-                subject name
-            schema typing.Union[client.schema.BaseSchema, str]:
-                Avro or JSON schema
-            headers (dict):
-                Extra headers to add on the requests
-            timeout (httpx._client.TimeoutTypes):
+        Attributes:
+            subject str: subject name
+            schema typing.Union[client.schema.BaseSchema, str]: Avro or JSON schema
+            headers typing.Dict: Extra headers to add on the requests
+            timeout httpx._client.TimeoutTypes:
                 The timeout configuration to use when sending requests. Default USE_CLIENT_DEFAULT
-            schema_type typing.Union["AVRO", "JSON"]:
+            schema_type typing.Union[AVRO, JSON]:
                 The type of schema to parse if `schema` is a string. Default "AVRO"
 
         Returns:
-            SchemaVersion (nametupled): (subject, schema_id, schema, version)
-            None: If schema not found.
+            SchemaVersion If schema exist
         """
         schemas_to_version = self.subject_to_schema_versions[subject]
 
         if isinstance(schema, str):
             schema = SchemaFactory.create_schema(schema, schema_type)
 
         version = schemas_to_version.get(schema)
@@ -649,37 +657,35 @@
         raise ClientError("Unable to get version of a schema", http_code=code, server_traceback=result)
 
     def test_compatibility(
         self,
         subject: str,
         schema: typing.Union[AvroSchema, JsonSchema, str],
         version: typing.Union[int, str] = "latest",
-        headers: dict = None,
+        headers: typing.Optional[typing.Dict] = None,
         timeout: typing.Union[TimeoutTypes, UseClientDefault] = USE_CLIENT_DEFAULT,
         schema_type: str = utils.AVRO_SCHEMA_TYPE,
     ) -> bool:
         """
         POST /compatibility/subjects/(string: subject)/versions/(versionId: version)
         Test the compatibility of a candidate parsed schema for a given subject.
         By default the latest version is checked against.
 
-        Args:
-            subject (str):
-                subject name
+        Attributes:
+            subject str: subject name
             schema typing.Union[client.schema.AvroSchema, client.schema.JsonSchema, str]:
                 Avro or JSON schema
-            headers (dict):
-                Extra headers to add on the requests
-            timeout (httpx._client.TimeoutTypes):
+            headers typing.Dict: Extra headers to add on the requests
+            timeout httpx._client.TimeoutTypes:
                 The timeout configuration to use when sending requests. Default USE_CLIENT_DEFAULT
-            schema_type typing.Union["AVRO", "JSON"]:
+            schema_type typing.Union[AVRO, JSON]:
                 The type of schema to parse if `schema` is a string. Default "AVRO"
 
         Returns:
-            bool: True if schema given compatible, False otherwise
+            Wether the schema is compatible with the latest version for a subject
         """
         url, method = self.url_manager.url_for("test_compatibility", subject=subject, version=version)
 
         if isinstance(schema, str):
             schema = SchemaFactory.create_schema(schema, schema_type)
 
         body = {"schema": json.dumps(schema.raw_schema), "schemaType": schema.schema_type}
@@ -696,33 +702,33 @@
             return result.get("is_compatible")
 
         raise ClientError("Unable to check the compatibility", http_code=code, server_traceback=result)
 
     def update_compatibility(
         self,
         level: str,
-        subject: str = None,
-        headers: dict = None,
+        subject: typing.Optional[str] = None,
+        headers: typing.Optional[typing.Dict] = None,
         timeout: typing.Union[TimeoutTypes, UseClientDefault] = USE_CLIENT_DEFAULT,
     ) -> bool:
         """
         PUT /config/(string: subject)
         Update the compatibility level.
         If subject is None, the compatibility level is global.
 
-        Args:
-            level (str): one of BACKWARD, BACKWARD_TRANSITIVE, FORWARD, FORWARD_TRANSITIVE,
+        Attributes:
+            level str: one of BACKWARD, BACKWARD_TRANSITIVE, FORWARD, FORWARD_TRANSITIVE,
                 FULL, FULL_TRANSITIVE, NONE
-            subject (str): Option subject
-            headers (dict): Extra headers to add on the requests
-            timeout (httpx._client.TimeoutTypes): The timeout configuration to use when sending requests.
+            subject str: Option subject
+            headers typing.Dict: Extra headers to add on the requests
+            timeout httpx._client.TimeoutTypes: The timeout configuration to use when sending requests.
                     Default USE_CLIENT_DEFAULT
 
         Returns:
-            bool: True if compatibility was updated
+            Whether the compatibility was updated
 
         Raises:
             ClientError: if the request was unsuccessful or an invalid
         """
         if level not in utils.VALID_LEVELS:
             raise ClientError(f"Invalid level specified: {level}")
 
@@ -736,34 +742,34 @@
         if status.is_success(code):
             return True
 
         raise ClientError(f"Unable to update level: {level}.", http_code=code, server_traceback=result)
 
     def get_compatibility(
         self,
-        subject: str = None,
-        headers: dict = None,
+        subject: typing.Optional[str] = None,
+        headers: typing.Optional[typing.Dict] = None,
         timeout: typing.Union[TimeoutTypes, UseClientDefault] = USE_CLIENT_DEFAULT,
     ) -> str:
         """
         Get the current compatibility level for a subject.
 
-        Args:
-            subject (str): subject name
-            headers (dict): Extra headers to add on the requests
-            timeout (httpx._client.TimeoutTypes): The timeout configuration to use when sending requests.
+        Attributes:
+            subject str: subject name
+            headers typing.Dict: Extra headers to add on the requests
+            timeout httpx._client.TimeoutTypes: The timeout configuration to use when sending requests.
                     Default USE_CLIENT_DEFAULT
 
         Returns:
-            str: one of BACKWARD, BACKWARD_TRANSITIVE, FORWARD, FORWARD_TRANSITIVE,
+            One of BACKWARD, BACKWARD_TRANSITIVE, FORWARD, FORWARD_TRANSITIVE,
                 FULL, FULL_TRANSITIVE, NONE
 
         Raises:
             ClientError: if the request was unsuccessful or an invalid
-            compatibility level was returned
+                compatibility level was returned
         """
         url, method = self.url_manager.url_for("get_compatibility", subject=subject)
         result, code = get_response_and_status_code(self.request(url, method=method, headers=headers, timeout=timeout))
 
         if status.is_success(code):
             compatibility = result.get("compatibilityLevel")
             if compatibility not in utils.VALID_LEVELS:
@@ -782,35 +788,34 @@
         )
 
 
 class AsyncSchemaRegistryClient(BaseClient):
     """
     A client that talks to a Schema Registry over HTTP
 
-    **Parameters:**
-
-    * **url** - *(Union[str, Dict]*: Url to schema registry or dictionary containing client configuration.
-    * **ca_location** - *Optional[str]*: File or directory path to CA certificate(s)
-        for verifying the Schema Registry key.
-    * **cert_location** - *Optional[str]*: Path to public key used for authentication.
-    * **key_location** - *Optional[str]*: Path to private key used for authentication.
-    * **key_password** - *Optional[str]*: Key password
-    * **extra_headers** - *Optional[Dict[str, str]]*: Extra headers to add on every requests.
-    * **timeout** - *Optional[httpx._client.TimeoutTypes]*  The timeout configuration to use when sending requests.
-    * **pool_limits** - *Optional[httpx.Limits])* The connection pool configuration to use when
-        determining the maximum number of concurrently open HTTP connections.
-    * **auth** - *(optional)* (schema_registry.client.Auth) Auth credentials.
+    Attributes:
+        url str | typing.Dict: Url to schema registry or dictionary containing client configuration.
+        ca_location str | None: File or directory path to CA certificate(s)
+            for verifying the Schema Registry key.
+        cert_location str | None: Path to public key used for authentication.
+        key_location str | None: Path to private key used for authentication.
+        key_password str | None: Key password
+        extra_headers str | None: Extra headers to add on every requests.
+        timeout httpx.Timeout | None: The timeout configuration to use when sending requests.
+        pool_limits httpx.Limits | None: The connection pool configuration to use when
+            determining the maximum number of concurrently open HTTP connections.
+        auth auth_utils.Auth | None: Auth credentials.
     """
 
     async def request(
         self,
         url: str,
         method: str = "GET",
-        body: dict = None,
-        headers: dict = None,
+        body: typing.Optional[typing.Dict] = None,
+        headers: typing.Optional[typing.Dict] = None,
         timeout: typing.Union[TimeoutTypes, UseClientDefault] = USE_CLIENT_DEFAULT,
     ) -> httpx.Response:
         if method not in utils.VALID_METHODS:
             raise ClientError(f"Method {method} is invalid; valid methods include {utils.VALID_METHODS}")
 
         _headers = self.prepare_headers(body=body, headers=headers)
         async with httpx.AsyncClient(**self.client_kwargs) as client:
@@ -818,43 +823,40 @@
 
         return response
 
     async def register(
         self,
         subject: str,
         schema: typing.Union[BaseSchema, str],
-        headers: dict = None,
+        headers: typing.Optional[typing.Dict] = None,
         timeout: typing.Union[TimeoutTypes, UseClientDefault] = USE_CLIENT_DEFAULT,
         schema_type: str = utils.AVRO_SCHEMA_TYPE,
     ) -> int:
         """
         POST /subjects/(string: subject)/versions
         Register a schema with the registry under the given subject
         and receive a schema id.
         Schema can be avro or json, and can be presented as a parsed schema or a string.
         If schema is a string, the `schema_type` kwarg must be used to indicate
         what type of schema the string is ("AVRO" by default).
         If the schema is already parsed, the schema_type is inferred directly from the parsed schema.
         Multiple instances of the same schema will result in cache misses.
 
-
-        Args:
-            subject (str):
-                subject name
-            schema typing.Union[client.schema.AvroSchema, client.schema.JsonSchema, str]:
-                Avro or JSON schema
-            headers (dict):
-                Extra headers to add on the requests
-            timeout (httpx._client.TimeoutTypes):
-                The timeout configuration to use when sending requests. Default USE_CLIENT_DEFAULT
-            schema_type typing.Union["AVRO", "JSON"]:
-                The type of schema to parse if `schema` is a string. Default "AVRO"
+        Attributes:
+            subject str: subject name
+            schema typing.Union[client.schema.BaseSchema, str]: Avro or JSON
+                schema to be registered
+            headers Dict: Extra headers to add on the requests
+            timeout Union[TimeoutTypes, UseClientDefault]: The timeout configuration
+                to use when sending requests. Default USE_CLIENT_DEFAULT
+            schema_type typing.Union[AVRO, JSON]: The type of schema to
+                parse if `schema` is a string. Default "AVRO"
 
         Returns:
-            int: schema_id
+            schema_id
         """
         schemas_to_id = self.subject_to_schema_ids[subject]
 
         if isinstance(schema, str):
             schema = SchemaFactory.create_schema(schema, schema_type)
 
         schema_id = schemas_to_id.get(schema)
@@ -894,59 +896,61 @@
 
         schema_id = result["id"]
         self._cache_schema(schema, schema_id, subject)
 
         return schema_id
 
     async def get_subjects(
-        self, headers: dict = None, timeout: typing.Union[TimeoutTypes, UseClientDefault] = USE_CLIENT_DEFAULT
+        self,
+        headers: typing.Optional[typing.Dict] = None,
+        timeout: typing.Union[TimeoutTypes, UseClientDefault] = USE_CLIENT_DEFAULT,
     ) -> list:
         """
         GET /subjects/(string: subject)
         Get list of all registered subjects in your Schema Registry.
 
-        Args:
-            subject (str): subject name
-            headers (dict): Extra headers to add on the requests
-            timeout (httpx._client.TimeoutTypes): The timeout configuration to use when sending requests.
+        Attributes:
+            subject str: subject name
+            headers typing.Dict: Extra headers to add on the requests
+            timeout httpx._client.TimeoutTypes: The timeout configuration to use when sending requests.
                     Default USE_CLIENT_DEFAULT
 
         Returns:
-            list [str]: list of registered subjects.
+            List of registered subjects.
         """
         url, method = self.url_manager.url_for("get_subjects")
         result, code = get_response_and_status_code(
             await self.request(url, method=method, headers=headers, timeout=timeout)
         )
 
         if status.is_success(code):
             return result
 
         raise ClientError("Unable to get subjects", http_code=code, server_traceback=result)
 
     async def delete_subject(
         self,
         subject: str,
-        headers: dict = None,
+        headers: typing.Optional[typing.Dict] = None,
         timeout: typing.Union[TimeoutTypes, UseClientDefault] = USE_CLIENT_DEFAULT,
     ) -> list:
         """
         DELETE /subjects/(string: subject)
         Deletes the specified subject and its associated compatibility level if registered.
         It is recommended to use this API only when a topic needs to be
         recycled or in development environments.
 
-        Args:
-            subject (str): subject name
-            headers (dict): Extra headers to add on the requests
-            timeout (httpx._client.TimeoutTypes): The timeout configuration to use when sending requests.
-                Default USE_CLIENT_DEFAULT
+        Attributes:
+            subject str: subject name
+            headers dict: Extra headers to add on the requests
+            timeout httpx._client.TimeoutTypes: The timeout configuration to use when sending requests.
+             Default USE_CLIENT_DEFAULT
 
         Returns:
-            list (int): version of the schema deleted under this subject
+            List version of the schema deleted under this subject
         """
         url, method = self.url_manager.url_for("delete_subject", subject=subject)
         result, code = get_response_and_status_code(
             await self.request(url, method=method, headers=headers, timeout=timeout)
         )
 
         if status.is_success(code):
@@ -955,29 +959,29 @@
             return []
 
         raise ClientError("Unable to delete subject", http_code=code, server_traceback=result)
 
     async def get_by_id(
         self,
         schema_id: int,
-        headers: dict = None,
+        headers: typing.Optional[typing.Dict] = None,
         timeout: typing.Union[TimeoutTypes, UseClientDefault] = USE_CLIENT_DEFAULT,
     ) -> typing.Optional[typing.Union[AvroSchema, JsonSchema]]:
         """
         GET /schemas/ids/{int: id}
         Retrieve a parsed avro schema by id or None if not found
 
-        Args:
-            schema_id (int): Schema Id
-            headers (dict): Extra headers to add on the requests
-            timeout (httpx._client.TimeoutTypes): The timeout configuration to use when sending requests.
+        Attributes:
+            schema_id int: Schema Id
+            headers dict: Extra headers to add on the requests
+            timeout httpx._client.TimeoutTypes: The timeout configuration to use when sending requests.
                 Default USE_CLIENT_DEFAULT
 
         Returns:
-            typing.Union[client.schema.AvroSchema, client.schema.JsonSchema]: Avro or JSON Record schema
+            Avro or JSON schema
         """
         if schema_id in self.id_to_schema:
             return self.id_to_schema[schema_id]
 
         url, method = self.url_manager.url_for("get_by_id", schema_id=schema_id)
 
         result, code = get_response_and_status_code(
@@ -993,15 +997,15 @@
 
         raise ClientError(f"Received bad schema (id {schema_id})", http_code=code, server_traceback=result)
 
     async def get_schema(
         self,
         subject: str,
         version: typing.Union[int, str] = "latest",
-        headers: dict = None,
+        headers: typing.Optional[typing.Dict] = None,
         timeout: typing.Union[TimeoutTypes, UseClientDefault] = USE_CLIENT_DEFAULT,
     ) -> typing.Optional[utils.SchemaVersion]:
         """
         GET /subjects/(string: subject)/versions/(versionId: version)
         Get a specific version of the schema registered under this subject
 
         Args:
@@ -1045,29 +1049,29 @@
         self._cache_schema(schema, schema_id, subject, version)
 
         return utils.SchemaVersion(subject, schema_id, schema, version)
 
     async def get_schema_subject_versions(
         self,
         schema_id: int,
-        headers: dict = None,
+        headers: typing.Optional[typing.Dict] = None,
         timeout: typing.Union[TimeoutTypes, UseClientDefault] = USE_CLIENT_DEFAULT,
     ) -> typing.Optional[typing.List[SubjectVersion]]:
         """
         GET /schemas/ids/{int: id}/versions
         Get the subject-version pairs identified by the input ID.
 
-        Args:
-            schema_id (int): Schema Id
-            headers (dict): Extra headers to add on the requests
-            timeout (httpx._client.TimeoutTypes): The timeout configuration to use when sending requests.
+        Attributes:
+            schema_id int: Schema Id
+            headers dict: Extra headers to add on the requests
+            timeout httpx._client.TimeoutTypes: The timeout configuration to use when sending requests.
                     Default USE_CLIENT_DEFAULT
 
         Returns:
-            typing.List[SubjectVersion]: List of Subject/Version pairs where Schema Id is registered
+            List of Subject/Version pairs where Schema Id is registered
         """
         url, method = self.url_manager.url_for("get_schema_subject_versions", schema_id=schema_id)
         result, code = get_response_and_status_code(
             await self.request(url, method=method, headers=headers, timeout=timeout)
         )
 
         if code == status.HTTP_404_NOT_FOUND:
@@ -1080,29 +1084,29 @@
             return ret
 
         raise ClientError(f"Received bad schema (id {schema_id})", http_code=code, server_traceback=result)
 
     async def get_versions(
         self,
         subject: str,
-        headers: dict = None,
+        headers: typing.Optional[typing.Dict] = None,
         timeout: typing.Union[TimeoutTypes, UseClientDefault] = USE_CLIENT_DEFAULT,
     ) -> list:
         """
         GET subjects/{subject}/versions
         Get a list of versions registered under the specified subject.
 
-        Args:
-            subject (str): subject name
-            headers (dict): Extra headers to add on the requests
-            timeout (httpx._client.TimeoutTypes): The timeout configuration to use when sending requests.
-                    Default USE_CLIENT_DEFAULT
+        Attributes:
+            subject str: subject name
+            headers dict: Extra headers to add on the requests
+            timeout httpx._client.TimeoutTypes: The timeout configuration to use when sending requests.
+                Default USE_CLIENT_DEFAULT
 
         Returns:
-            list (str): version of the schema registered under this subject
+            List  version of the schema registered under this subject
         """
         url, method = self.url_manager.url_for("get_versions", subject=subject)
 
         result, code = get_response_and_status_code(
             await self.request(url, method=method, headers=headers, timeout=timeout)
         )
         if status.is_success(code):
@@ -1113,38 +1117,37 @@
 
         raise ClientError(f"Unable to get the versions for subject {subject}", http_code=code, server_traceback=result)
 
     async def delete_version(
         self,
         subject: str,
         version: typing.Union[int, str] = "latest",
-        headers: dict = None,
+        headers: typing.Optional[typing.Dict] = None,
         timeout: typing.Union[TimeoutTypes, UseClientDefault] = USE_CLIENT_DEFAULT,
     ) -> typing.Optional[int]:
         """
         DELETE /subjects/(string: subject)/versions/(versionId: version)
         Deletes a specific version of the schema registered under this subject.
         This only deletes the version and the schema ID remains intact making
         it still possible to decode data using the schema ID.
         This API is recommended to be used only in development environments or
         under extreme circumstances where-in, its required to delete a previously
         registered schema for compatibility purposes or re-register previously registered schema.
 
-        Args:
-            subject (str): subject name
-            version (str): Version of the schema to be deleted.
+        Attributes:
+            subject str: subject name
+            version str: Version of the schema to be deleted.
                 Valid values for versionId are between [1,2^31-1] or the string "latest".
                 "latest" deletes the last registered schema under the specified subject.
-            headers (dict): Extra headers to add on the requests
-            timeout (httpx._client.TimeoutTypes): The timeout configuration to use when sending requests.
+            headers typing.Dict: Extra headers to add on the requests
+            timeout httpx._client.TimeoutTypes: The timeout configuration to use when sending requests.
                     Default USE_CLIENT_DEFAULT
 
         Returns:
-            int: version of the schema deleted
-            None: If the subject or version does not exist.
+            Version of the schema deleted. If the subject or version does not exist.
         """
         url, method = self.url_manager.url_for("delete_version", subject=subject, version=version)
 
         result, code = get_response_and_status_code(
             await self.request(url, method=method, headers=headers, timeout=timeout)
         )
 
@@ -1155,39 +1158,35 @@
 
         raise ClientError("Unable to delete the version", http_code=code, server_traceback=result)
 
     async def check_version(
         self,
         subject: str,
         schema: typing.Union[BaseSchema, str],
-        headers: dict = None,
+        headers: typing.Optional[typing.Dict] = None,
         timeout: typing.Union[TimeoutTypes, UseClientDefault] = USE_CLIENT_DEFAULT,
         schema_type: str = utils.AVRO_SCHEMA_TYPE,
     ) -> typing.Optional[utils.SchemaVersion]:
         """
         POST /subjects/(string: subject)
         Check if a schema has already been registered under the specified subject.
         If so, this returns the schema string along with its globally unique identifier,
         its version under this subject and the subject name.
 
-        Args:
-            subject (str):
-                subject name
-            schema typing.Union[client.schema.AvroSchema, client.schema.JsonSchema, str]:
-                Avro or JSON schema
-            headers (dict):
-                Extra headers to add on the requests
-            timeout (httpx._client.TimeoutTypes):
+        Attributes:
+            subject str: subject name
+            schema typing.Union[client.schema.BaseSchema, str]: Avro or JSON schema
+            headers typing.Dict: Extra headers to add on the requests
+            timeout httpx._client.TimeoutTypes:
                 The timeout configuration to use when sending requests. Default USE_CLIENT_DEFAULT
-            schema_type typing.Union["AVRO", "JSON"]:
+            schema_type typing.Union[AVRO, JSON]:
                 The type of schema to parse if `schema` is a string. Default "AVRO"
 
         Returns:
-            SchemaVersion (nametupled): (subject, schema_id, schema, version)
-            None: If schema not found.
+            SchemaVersion If schema exist
         """
         schemas_to_version = self.subject_to_schema_versions[subject]
 
         if isinstance(schema, str):
             schema = SchemaFactory.create_schema(schema, schema_type)
 
         version = schemas_to_version.get(schema)
@@ -1217,37 +1216,35 @@
         raise ClientError("Unable to get version of a schema", http_code=code, server_traceback=result)
 
     async def test_compatibility(
         self,
         subject: str,
         schema: typing.Union[AvroSchema, JsonSchema, str],
         version: typing.Union[int, str] = "latest",
-        headers: dict = None,
+        headers: typing.Optional[typing.Dict] = None,
         timeout: typing.Union[TimeoutTypes, UseClientDefault] = USE_CLIENT_DEFAULT,
         schema_type: str = utils.AVRO_SCHEMA_TYPE,
     ) -> bool:
         """
         POST /compatibility/subjects/(string: subject)/versions/(versionId: version)
         Test the compatibility of a candidate parsed schema for a given subject.
         By default the latest version is checked against.
 
-        Args:
-            subject (str):
-                subject name
+        Attributes:
+            subject str: subject name
             schema typing.Union[client.schema.AvroSchema, client.schema.JsonSchema, str]:
                 Avro or JSON schema
-            headers (dict):
-                Extra headers to add on the requests
-            timeout (httpx._client.TimeoutTypes):
+            headers typing.Dict: Extra headers to add on the requests
+            timeout httpx._client.TimeoutTypes:
                 The timeout configuration to use when sending requests. Default USE_CLIENT_DEFAULT
-            schema_type typing.Union["AVRO", "JSON"]:
+            schema_type typing.Union[AVRO, JSON]:
                 The type of schema to parse if `schema` is a string. Default "AVRO"
 
         Returns:
-            bool: True if schema given compatible, False otherwise
+            Wether the schema is compatible with the latest version for a subject
         """
         url, method = self.url_manager.url_for("test_compatibility", subject=subject, version=version)
 
         if isinstance(schema, str):
             schema = SchemaFactory.create_schema(schema, schema_type)
 
         body = {"schema": json.dumps(schema.raw_schema), "schemaType": schema.schema_type}
@@ -1265,33 +1262,33 @@
             return result.get("is_compatible")
 
         raise ClientError("Unable to check the compatibility", http_code=code, server_traceback=result)
 
     async def update_compatibility(
         self,
         level: str,
-        subject: str = None,
-        headers: dict = None,
+        subject: typing.Optional[str] = None,
+        headers: typing.Optional[typing.Dict] = None,
         timeout: typing.Union[TimeoutTypes, UseClientDefault] = USE_CLIENT_DEFAULT,
     ) -> bool:
         """
         PUT /config/(string: subject)
         Update the compatibility level.
         If subject is None, the compatibility level is global.
 
-        Args:
-            level (str): one of BACKWARD, BACKWARD_TRANSITIVE, FORWARD, FORWARD_TRANSITIVE,
+        Attributes:
+            level str: one of BACKWARD, BACKWARD_TRANSITIVE, FORWARD, FORWARD_TRANSITIVE,
                 FULL, FULL_TRANSITIVE, NONE
-            subject (str): Option subject
-            headers (dict): Extra headers to add on the requests
-            timeout (httpx._client.TimeoutTypes): The timeout configuration to use when sending requests.
-            Default USE_CLIENT_DEFAULT
+            subject str: Option subject
+            headers typing.Dict: Extra headers to add on the requests
+            timeout httpx._client.TimeoutTypes: The timeout configuration to use when sending requests.
+                    Default USE_CLIENT_DEFAULT
 
         Returns:
-            bool: True if compatibility was updated
+            Whether the compatibility was updated
 
         Raises:
             ClientError: if the request was unsuccessful or an invalid
         """
         if level not in utils.VALID_LEVELS:
             raise ClientError(f"Invalid level specified: {level}")
 
@@ -1305,34 +1302,34 @@
         if status.is_success(code):
             return True
 
         raise ClientError(f"Unable to update level: {level}.", http_code=code, server_traceback=result)
 
     async def get_compatibility(
         self,
-        subject: str = None,
-        headers: dict = None,
+        subject: typing.Optional[str] = None,
+        headers: typing.Optional[typing.Dict] = None,
         timeout: typing.Union[TimeoutTypes, UseClientDefault] = USE_CLIENT_DEFAULT,
     ) -> str:
         """
         Get the current compatibility level for a subject.
 
-        Args:
-            subject (str): subject name
-            headers (dict): Extra headers to add on the requests
-            timeout (httpx._client.TimeoutTypes): The timeout configuration to use when sending requests.
+        Attributes:
+            subject str: subject name
+            headers typing.Dict: Extra headers to add on the requests
+            timeout httpx._client.TimeoutTypes: The timeout configuration to use when sending requests.
                     Default USE_CLIENT_DEFAULT
 
         Returns:
-            str: one of BACKWARD, BACKWARD_TRANSITIVE, FORWARD, FORWARD_TRANSITIVE,
+            One of BACKWARD, BACKWARD_TRANSITIVE, FORWARD, FORWARD_TRANSITIVE,
                 FULL, FULL_TRANSITIVE, NONE
 
         Raises:
             ClientError: if the request was unsuccessful or an invalid
-            compatibility level was returned
+                compatibility level was returned
         """
         url, method = self.url_manager.url_for("get_compatibility", subject=subject)
         result, code = get_response_and_status_code(
             await self.request(url, method=method, headers=headers, timeout=timeout)
         )
 
         if status.is_success(code):
```

### Comparing `python-schema-registry-client-2.4.3/schema_registry/client/paths.py` & `python_schema_registry_client-2.4.4/schema_registry/client/paths.py`

 * *Files identical despite different names*

### Comparing `python-schema-registry-client-2.4.3/schema_registry/client/schema.py` & `python_schema_registry_client-2.4.4/schema_registry/client/schema.py`

 * *Files identical despite different names*

### Comparing `python-schema-registry-client-2.4.3/schema_registry/client/status.py` & `python_schema_registry_client-2.4.4/schema_registry/client/status.py`

 * *Files identical despite different names*

### Comparing `python-schema-registry-client-2.4.3/schema_registry/client/urls.py` & `python_schema_registry_client-2.4.4/schema_registry/client/urls.py`

 * *Files identical despite different names*

### Comparing `python-schema-registry-client-2.4.3/schema_registry/client/utils.py` & `python_schema_registry_client-2.4.4/schema_registry/client/utils.py`

 * *Files identical despite different names*

### Comparing `python-schema-registry-client-2.4.3/schema_registry/serializers/__init__.py` & `python_schema_registry_client-2.4.4/schema_registry/serializers/__init__.py`

 * *Files identical despite different names*

### Comparing `python-schema-registry-client-2.4.3/schema_registry/serializers/faust.py` & `python_schema_registry_client-2.4.4/schema_registry/serializers/faust.py`

 * *Files 0% similar despite different names*

```diff
@@ -21,15 +21,14 @@
         self.schema_subject = schema_subject
         self.schema = schema
         self.message_serializer = message_serializer
 
         Codec.__init__(self)
 
     def _loads(self, event: bytes) -> typing.Optional[typing.Dict]:
-
         return self.message_serializer.decode_message(event)
 
     def _dumps(self, payload: typing.Dict[str, typing.Any]) -> bytes:
         """
         Given a parsed avro schema, encode a record for the given topic.  The
         record is expected to be a dictionary.
         The schema is registered with the subject of 'topic-value'
@@ -72,30 +71,28 @@
 
 def avro_serializer_factory(
     schema_registry_client: SchemaRegistryClient,
     schema_subject: str,
     schema: AvroSchema,
     return_record_name: bool = False,
 ) -> "Serializer":  # type: ignore # noqa: F821
-
     if isinstance(schema, str):
         schema = AvroSchema(schema)
 
     return Serializer(
         schema_subject, schema, AvroMessageSerializer(schema_registry_client, return_record_name=return_record_name)
     )
 
 
 def json_serializer_factory(
     schema_registry_client: SchemaRegistryClient,
     schema_subject: str,
     schema: JsonSchema,
     return_record_name: bool = False,
 ) -> "Serializer":  # type: ignore # noqa: F821
-
     if isinstance(schema, str):
         schema = JsonSchema(schema)
 
     return Serializer(
         schema_subject, schema, JsonMessageSerializer(schema_registry_client, return_record_name=return_record_name)
     )
```

### Comparing `python-schema-registry-client-2.4.3/schema_registry/serializers/message_serializer.py` & `python_schema_registry_client-2.4.4/schema_registry/serializers/message_serializer.py`

 * *Files 13% similar despite different names*

```diff
@@ -33,19 +33,18 @@
         self.close()
 
 
 class MessageSerializer(ABC):
     """
     A helper class that can serialize and deserialize messages asynchronously
 
-    **Parameters:**
-
-    * **schemaregistry_client** - schema_registry.client.AsyncSchemaRegistryClient: Http Client
-    * **reader_schema** - schema_registry.schema.AvroSchema: Specify a schema to decode the message
-    * **return_record_name** - bool: If the record name should be returned
+    Attributes:
+        schemaregistry_client schema_registry.client.AsyncSchemaRegistryClient: Http Client
+        reader_schema schema_registry.schema.AvroSchema: Specify a schema to decode the message
+        return_record_name bool: If the record name should be returned
     """
 
     def __init__(
         self,
         schemaregistry_client: SchemaRegistryClient,
         reader_schema: typing.Optional[schema.AvroSchema] = None,
         return_record_name: bool = False,
@@ -70,39 +69,43 @@
         ...
 
     def encode_record_with_schema(self, subject: str, schema: typing.Union[BaseSchema], record: dict) -> bytes:
         """
         Given a parsed avro schema, encode a record for the given subject.
         The record is expected to be a dictionary.
         The schema is registered with the subject of 'topic-value'
-        Args:
-            subject (str): Subject name
-            schema (avro.schema.RecordSchema): Avro Schema
-            record (dict): An object to serialize
+
+        Attributes:
+            subject str: Subject name
+            schema avro.schema.RecordSchema: Avro Schema
+            record typing.Dict: An object to serialize
+
         Returns:
-            bytes: Encoded record with schema ID as bytes
+            Encoded record with schema ID as bytes
         """
         # Try to register the schema
         schema_id = self.schemaregistry_client.register(subject, schema, schema_type=self._serializer_schema_type)
 
         # cache writer
         if not self.id_to_writers.get(schema_id):
             self.id_to_writers[schema_id] = self._get_encoder_func(schema)
 
         return self.encode_record_with_schema_id(schema_id, record)
 
     def encode_record_with_schema_id(self, schema_id: int, record: dict) -> bytes:
         """
         Encode a record with a given schema id.  The record must
         be a python dictionary.
-        Args:
-            schema_id (int): integer ID
-            record (dict): An object to serialize
+
+        Attributes:
+            schema_id int: integer ID
+            record typing.Dict: An object to serialize
+
         Returns:
-            func: decoder function
+            Decoder function
         """
         # use slow avro
         if schema_id not in self.id_to_writers:
             try:
                 schema = self.schemaregistry_client.get_by_id(schema_id)
                 if not schema:
                     raise SerializerError("Schema does not exist")
@@ -121,16 +124,17 @@
 
             return outf.getvalue()
 
     def decode_message(self, message: typing.Optional[bytes]) -> typing.Optional[dict]:
         """
         Decode a message from kafka that has been encoded for use with
         the schema registry.
-        Args:
-            message (bytes or None): message key or value to be decoded
+        Attributes:
+            message bytes: message key or value to be decoded
+
         Returns:
             dict: Decoded message contents.
         """
 
         if message is None:
             return None
 
@@ -159,19 +163,71 @@
             return decoder_func(payload)
 
 
 class AvroMessageSerializer(MessageSerializer):
     """
     AvroMessageSerializer to serialize and deserialize messages
 
-    **Parameters:**
-
-    * **schemaregistry_client** - schema_registry.client.AsyncSchemaRegistryClient: Http Client
-    * **reader_schema** - schema_registry.schema.AvroSchema: Specify a schema to decode the message
-    * **return_record_name** - bool: If the record name should be returned
+    !!! Example
+        ```python
+        from schema_registry.client import SchemaRegistryClient, schema
+        from schema_registry.serializers import AvroMessageSerializer
+
+
+        client = SchemaRegistryClient("http://127.0.0.1:8081")
+        avro_message_serializer = AvroMessageSerializer(client)
+
+        avro_user_schema = schema.AvroSchema({
+            "type": "record",
+            "namespace": "com.example",
+            "name": "AvroUsers",
+            "fields": [
+                {"name": "first_name", "type": "string"},
+                {"name": "last_name", "type": "string"},
+                {"name": "age", "type": "int"},
+
+            ],
+        })
+
+        # We want to encode the user_record with avro_user_schema
+        user_record = {
+            "first_name": "my_first_name",
+            "last_name": "my_last_name",
+            "age": 20,
+        }
+
+        # Encode the record
+        message_encoded = avro_message_serializer.encode_record_with_schema(
+            "user", avro_user_schema, user_record)
+
+        # this is because the message encoded reserved 5 bytes for the schema_id
+        assert len(message_encoded) > 5
+        assert isinstance(message_encoded, bytes)
+
+        # Decode the message
+        message_decoded = avro_message_serializer.decode_message(message_encoded)
+        assert message_decoded == user_record
+
+        # Now if we send a bad record
+        bad_record = {
+            "first_name": "my_first_name",
+            "last_name": "my_last_name",
+            "age": "my_age"
+        }
+
+        avro_message_serializer.encode_record_with_schema(
+            "user", avro_user_schema, bad_record)
+
+        # >>> TypeError: an integer is required on field age
+        ```
+
+    Attributes:
+        schemaregistry_client schema_registry.client.AsyncSchemaRegistryClient: Http Client
+        reader_schema schema_registry.schema.AvroSchema: Specify a schema to decode the message
+        return_record_name bool: If the record name should be returned
     """
 
     @property
     def _serializer_schema_type(self) -> str:
         return utils.AVRO_SCHEMA_TYPE
 
     def _get_encoder_func(self, schema: typing.Union[BaseSchema]) -> typing.Callable:
@@ -183,19 +239,71 @@
         )  # type: ignore
 
 
 class JsonMessageSerializer(MessageSerializer):
     """
     JsonMessageSerializer to serialize and deserialize messages
 
-    **Parameters:**
+    !!! Example
 
-    * **schemaregistry_client** - schema_registry.client.AsyncSchemaRegistryClient: Http Client
-    * **reader_schema** - schema_registry.schema.AvroSchema: Specify a schema to decode the message
-    * **return_record_name** - bool: If the record name should be returned
+        ```python
+        from schema_registry.client import SchemaRegistryClient, schema
+        from schema_registry.serializers import JsonMessageSerializer
+
+
+        client = SchemaRegistryClient("http://127.0.0.1:8081")
+        json_message_serializer = JsonMessageSerializer(client)
+
+        json_schema = schema.JsonSchema({
+        "definitions" : {
+            "record:python.test.basic.basic" : {
+            "description" : "basic schema for tests",
+            "type" : "object",
+            "required" : [ "number", "name" ],
+            "properties" : {
+                "number" : {
+                "oneOf" : [ {
+                    "type" : "integer"
+                }, {
+                    "type" : "null"
+                } ]
+                },
+                "name" : {
+                "oneOf" : [ {
+                    "type" : "string"
+                } ]
+                }
+            }
+            }
+        },
+        "$ref" : "#/definitions/record:python.test.basic.basic"
+        })
+
+        # Encode the record
+        basic_record = {
+            "number": 10,
+            "name": "a_name",
+        }
+
+        message_encoded = json_message_serializer.encode_record_with_schema(
+            "basic", json_schema, basic_record)
+
+        # this is because the message encoded reserved 5 bytes for the schema_id
+        assert len(message_encoded) > 5
+        assert isinstance(message_encoded, bytes)
+
+        # Decode the message
+        message_decoded = json_message_serializer.decode_message(message_encoded)
+        assert message_decoded == basic_record
+        ```
+
+    Attributes:
+        schemaregistry_client schema_registry.client.AsyncSchemaRegistryClient: Http Client
+        reader_schema schema_registry.schema.AvroSchema: Specify a schema to decode the message
+        return_record_name bool: If the record name should be returned
     """
 
     @property
     def _serializer_schema_type(self) -> str:
         return utils.JSON_SCHEMA_TYPE
 
     def _get_encoder_func(self, schema: typing.Union[BaseSchema]) -> typing.Callable:
@@ -214,19 +322,18 @@
         return json_decoder_func
 
 
 class AsyncMessageSerializer(ABC):
     """
     AsyncMessageSerializer to serialize and deserialize messages asynchronously
 
-    **Parameters:**
-
-    * **schemaregistry_client** - schema_registry.client.AsyncSchemaRegistryClient: Http Client
-    * **reader_schema** - schema_registry.schema.AvroSchema: Specify a schema to decode the message
-    * **return_record_name** - bool: If the record name should be returned
+    Attributes:
+        schemaregistry_client schema_registry.client.AsyncSchemaRegistryClient: Http Client
+        reader_schema schema_registry.schema.AvroSchema: Specify a schema to decode the message
+        return_record_name bool: If the record name should be returned
     """
 
     def __init__(
         self,
         schemaregistry_client: AsyncSchemaRegistryClient,
         reader_schema: typing.Optional[schema.AvroSchema] = None,
         return_record_name: bool = False,
@@ -251,44 +358,49 @@
         ...
 
     async def encode_record_with_schema(self, subject: str, schema: typing.Union[BaseSchema], record: dict) -> bytes:
         """
         Given a parsed avro schema, encode a record for the given subject.
         The record is expected to be a dictionary.
         The schema is registered with the subject of 'topic-value'
-        Args:
-            subject (str): Subject name
-            schema (avro.schema.RecordSchema): Avro Schema
-            record (dict): An object to serialize
+
+        Attributes:
+            subject str: Subject name
+            schema avro.schema.RecordSchema: Avro Schema
+            record dict: An object to serialize
+
         Returns:
-            bytes: Encoded record with schema ID as bytes
+            Encoded record with schema ID
         """
         # Try to register the schema
         schema_id = await self.schemaregistry_client.register(subject, schema, schema_type=self._serializer_schema_type)
 
         # cache writer
         if not self.id_to_writers.get(schema_id):
             self.id_to_writers[schema_id] = self._get_encoder_func(schema)
 
         return await self.encode_record_with_schema_id(schema_id, record)
 
     async def encode_record_with_schema_id(self, schema_id: int, record: dict) -> bytes:
         """
         Encode a record with a given schema id.  The record must
         be a python dictionary.
-        Args:
-            schema_id (int): integer ID
-            record (dict): An object to serialize
+
+        Attributes:
+            schema_id int: integer ID
+            record typing.Dict: An object to serialize
+
         Returns:
-            func: decoder function
+            Decoder function
         """
         # use slow avro
         if schema_id not in self.id_to_writers:
             try:
                 schema = await self.schemaregistry_client.get_by_id(schema_id)
+
                 if not schema:
                     raise SerializerError("Schema does not exist")
                 self.id_to_writers[schema_id] = self._get_encoder_func(schema)
             except ClientError:
                 exc_type, exc_value, exc_traceback = sys.exc_info()
                 raise SerializerError(repr(traceback.format_exception(exc_type, exc_value, exc_traceback)))
 
@@ -302,18 +414,20 @@
 
             return outf.getvalue()
 
     async def decode_message(self, message: typing.Optional[bytes]) -> typing.Optional[dict]:
         """
         Decode a message from kafka that has been encoded for use with
         the schema registry.
-        Args:
-            message (bytes or None): message key or value to be decoded
+
+        Attributes:
+            message bytes: message key or value to be decoded
+
         Returns:
-            dict: Decoded message contents.
+            Decoded message
         """
 
         if message is None:
             return None
 
         if len(message) <= 5:
             raise SerializerError("message is too small to decode")
@@ -324,14 +438,15 @@
                 raise SerializerError("message does not start with magic byte")
 
             if schema_id in self.id_to_decoder_func:
                 return self.id_to_decoder_func[schema_id](payload)
 
             try:
                 writer_schema = await self.schemaregistry_client.get_by_id(schema_id)
+                print(writer_schema, "holis...")
             except ClientError as e:
                 raise SerializerError(f"unable to fetch schema with id {schema_id}: {e}")
 
             if writer_schema is None:
                 raise SerializerError(f"unable to fetch schema with id {schema_id}")
 
             decoder_func = self._get_decoder_func(payload, writer_schema)
@@ -340,19 +455,18 @@
             return decoder_func(payload)
 
 
 class AsyncAvroMessageSerializer(AsyncMessageSerializer):
     """
     AsyncAvroMessageSerializer to serialize and deserialize messages asynchronously
 
-    **Parameters:**
-
-    * **schemaregistry_client** - schema_registry.client.AsyncSchemaRegistryClient: Http Client
-    * **reader_schema** - schema_registry.schema.AvroSchema: Specify a schema to decode the message
-    * **return_record_name** - bool: If the record name should be returned
+    Attributes:
+        schemaregistry_client schema_registry.client.AsyncSchemaRegistryClient: Http Client
+        reader_schema schema_registry.schema.AvroSchema: Specify a schema to decode the message
+        return_record_name bool: If the record name should be returned
     """
 
     @property
     def _serializer_schema_type(self) -> str:
         return utils.AVRO_SCHEMA_TYPE
 
     def _get_encoder_func(self, schema: typing.Union[BaseSchema]) -> typing.Callable:
@@ -364,19 +478,18 @@
         )  # type: ignore
 
 
 class AsyncJsonMessageSerializer(AsyncMessageSerializer):
     """
     AsyncJsonMessageSerializer to serialize and deserialize messages asynchronously
 
-    **Parameters:**
-
-    * **schemaregistry_client** - schema_registry.client.AsyncSchemaRegistryClient: Http Client
-    * **reader_schema** - schema_registry.schema.AvroSchema: Specify a schema to decode the message
-    * **return_record_name** - bool: If the record name should be returned
+    Attributes:
+        schemaregistry_client schema_registry.client.AsyncSchemaRegistryClient: Http Client
+        reader_schema schema_registry.schema.AvroSchema: Specify a schema to decode the message
+        return_record_name bool: If the record name should be returned
     """
 
     @property
     def _serializer_schema_type(self) -> str:
         return utils.JSON_SCHEMA_TYPE
 
     def _get_encoder_func(self, schema: typing.Union[BaseSchema]) -> typing.Callable:
```

