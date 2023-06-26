# Comparing `tmp/vcrpy-4.3.1.tar.gz` & `tmp/vcrpy-4.4.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "vcrpy-4.3.1.tar", last modified: Fri May 26 16:04:05 2023, max compression
+gzip compressed data, was "vcrpy-4.4.0.tar", last modified: Mon Jun 26 14:20:09 2023, max compression
```

## Comparing `vcrpy-4.3.1.tar` & `vcrpy-4.4.0.tar`

### file list

```diff
@@ -1,106 +1,108 @@
-drwxr-xr-x   0 kevin      (501) staff       (20)        0 2023-05-26 16:04:05.109307 vcrpy-4.3.1/
--rw-r--r--   0 kevin      (501) staff       (20)     1063 2022-08-31 19:12:36.000000 vcrpy-4.3.1/LICENSE.txt
--rw-r--r--   0 kevin      (501) staff       (20)      142 2022-08-31 19:12:36.000000 vcrpy-4.3.1/MANIFEST.in
--rw-r--r--   0 kevin      (501) staff       (20)     3925 2023-05-26 16:04:05.109377 vcrpy-4.3.1/PKG-INFO
--rw-r--r--   0 kevin      (501) staff       (20)     2767 2022-08-31 19:12:36.000000 vcrpy-4.3.1/README.rst
--rw-r--r--   0 kevin      (501) staff       (20)      164 2023-05-24 18:36:09.000000 vcrpy-4.3.1/pyproject.toml
--rw-r--r--   0 kevin      (501) staff       (20)       67 2023-05-26 16:04:05.109567 vcrpy-4.3.1/setup.cfg
--rw-r--r--   0 kevin      (501) staff       (20)     3557 2023-05-26 15:56:05.000000 vcrpy-4.3.1/setup.py
-drwxr-xr-x   0 kevin      (501) staff       (20)        0 2023-05-26 16:04:05.097563 vcrpy-4.3.1/tests/
--rw-r--r--   0 kevin      (501) staff       (20)      354 2022-08-31 19:12:36.000000 vcrpy-4.3.1/tests/assertions.py
-drwxr-xr-x   0 kevin      (501) staff       (20)        0 2023-05-26 16:04:05.096258 vcrpy-4.3.1/tests/fixtures/
-drwxr-xr-x   0 kevin      (501) staff       (20)        0 2023-05-26 16:04:05.098448 vcrpy-4.3.1/tests/fixtures/migration/
--rw-r--r--   0 kevin      (501) staff       (20)     1115 2022-08-31 19:12:36.000000 vcrpy-4.3.1/tests/fixtures/migration/new_cassette.json
--rw-r--r--   0 kevin      (501) staff       (20)      599 2022-08-31 19:12:36.000000 vcrpy-4.3.1/tests/fixtures/migration/new_cassette.yaml
--rw-r--r--   0 kevin      (501) staff       (20)       23 2022-08-31 19:12:36.000000 vcrpy-4.3.1/tests/fixtures/migration/not_cassette.txt
--rw-r--r--   0 kevin      (501) staff       (20)     1031 2022-08-31 19:12:36.000000 vcrpy-4.3.1/tests/fixtures/migration/old_cassette.json
--rw-r--r--   0 kevin      (501) staff       (20)      869 2022-08-31 19:12:36.000000 vcrpy-4.3.1/tests/fixtures/migration/old_cassette.yaml
-drwxr-xr-x   0 kevin      (501) staff       (20)        0 2023-05-26 16:04:05.098579 vcrpy-4.3.1/tests/fixtures/wild/
--rw-r--r--   0 kevin      (501) staff       (20)     9705 2022-08-31 19:12:36.000000 vcrpy-4.3.1/tests/fixtures/wild/domain_redirect.yaml
-drwxr-xr-x   0 kevin      (501) staff       (20)        0 2023-05-26 16:04:05.103320 vcrpy-4.3.1/tests/integration/
--rw-r--r--   0 kevin      (501) staff       (20)        0 2022-08-31 19:12:36.000000 vcrpy-4.3.1/tests/integration/__init__.py
--rw-r--r--   0 kevin      (501) staff       (20)     1214 2023-05-24 18:36:09.000000 vcrpy-4.3.1/tests/integration/aiohttp_utils.py
-drwxr-xr-x   0 kevin      (501) staff       (20)        0 2023-05-26 16:04:05.103432 vcrpy-4.3.1/tests/integration/cassettes/
--rw-r--r--   0 kevin      (501) staff       (20)     1017 2023-05-24 18:36:09.000000 vcrpy-4.3.1/tests/integration/cassettes/test_httpx_test_test_behind_proxy.yml
--rw-r--r--   0 kevin      (501) staff       (20)      781 2023-05-26 15:56:05.000000 vcrpy-4.3.1/tests/integration/conftest.py
--rw-r--r--   0 kevin      (501) staff       (20)    16516 2023-05-26 15:56:05.000000 vcrpy-4.3.1/tests/integration/test_aiohttp.py
--rw-r--r--   0 kevin      (501) staff       (20)     2766 2022-08-31 19:12:36.000000 vcrpy-4.3.1/tests/integration/test_basic.py
--rw-r--r--   0 kevin      (501) staff       (20)     2951 2023-05-24 18:36:09.000000 vcrpy-4.3.1/tests/integration/test_boto.py
--rw-r--r--   0 kevin      (501) staff       (20)     3589 2023-05-24 18:36:09.000000 vcrpy-4.3.1/tests/integration/test_boto3.py
--rw-r--r--   0 kevin      (501) staff       (20)     2526 2023-05-24 18:36:09.000000 vcrpy-4.3.1/tests/integration/test_config.py
--rw-r--r--   0 kevin      (501) staff       (20)     1563 2023-05-24 18:36:09.000000 vcrpy-4.3.1/tests/integration/test_disksaver.py
--rw-r--r--   0 kevin      (501) staff       (20)     5714 2023-05-24 18:36:09.000000 vcrpy-4.3.1/tests/integration/test_filter.py
--rw-r--r--   0 kevin      (501) staff       (20)     1030 2022-08-31 19:12:36.000000 vcrpy-4.3.1/tests/integration/test_http
--rw-r--r--   0 kevin      (501) staff       (20)     4926 2023-05-24 18:36:09.000000 vcrpy-4.3.1/tests/integration/test_httplib2.py
--rw-r--r--   0 kevin      (501) staff       (20)    10415 2023-05-24 18:36:09.000000 vcrpy-4.3.1/tests/integration/test_httpx.py
--rw-r--r--   0 kevin      (501) staff       (20)     2621 2023-05-24 18:36:09.000000 vcrpy-4.3.1/tests/integration/test_ignore.py
--rw-r--r--   0 kevin      (501) staff       (20)     4000 2023-05-24 18:36:09.000000 vcrpy-4.3.1/tests/integration/test_matchers.py
--rw-r--r--   0 kevin      (501) staff       (20)      878 2023-05-24 18:36:09.000000 vcrpy-4.3.1/tests/integration/test_multiple.py
--rw-r--r--   0 kevin      (501) staff       (20)     1779 2023-05-24 18:36:09.000000 vcrpy-4.3.1/tests/integration/test_proxy.py
--rw-r--r--   0 kevin      (501) staff       (20)     5170 2023-05-24 18:36:09.000000 vcrpy-4.3.1/tests/integration/test_record_mode.py
--rw-r--r--   0 kevin      (501) staff       (20)     1167 2023-05-24 18:36:09.000000 vcrpy-4.3.1/tests/integration/test_register_matcher.py
--rw-r--r--   0 kevin      (501) staff       (20)     1852 2022-08-31 19:12:36.000000 vcrpy-4.3.1/tests/integration/test_register_persister.py
--rw-r--r--   0 kevin      (501) staff       (20)      962 2022-08-31 19:12:36.000000 vcrpy-4.3.1/tests/integration/test_register_serializer.py
--rw-r--r--   0 kevin      (501) staff       (20)      739 2023-05-24 18:36:09.000000 vcrpy-4.3.1/tests/integration/test_request.py
--rw-r--r--   0 kevin      (501) staff       (20)    11635 2023-05-24 18:36:09.000000 vcrpy-4.3.1/tests/integration/test_requests.py
--rw-r--r--   0 kevin      (501) staff       (20)     5040 2023-05-24 18:36:09.000000 vcrpy-4.3.1/tests/integration/test_stubs.py
--rw-r--r--   0 kevin      (501) staff       (20)    12599 2023-05-24 18:36:09.000000 vcrpy-4.3.1/tests/integration/test_tornado.py
--rw-r--r--   0 kevin      (501) staff       (20)     1387 2022-08-31 19:12:36.000000 vcrpy-4.3.1/tests/integration/test_tornado_exception_can_be_caught.yaml
--rw-r--r--   0 kevin      (501) staff       (20)     1566 2022-08-31 19:12:36.000000 vcrpy-4.3.1/tests/integration/test_tornado_with_decorator_use_cassette.yaml
--rw-r--r--   0 kevin      (501) staff       (20)     5072 2023-05-24 18:36:09.000000 vcrpy-4.3.1/tests/integration/test_urllib2.py
--rw-r--r--   0 kevin      (501) staff       (20)     6364 2023-05-26 15:56:05.000000 vcrpy-4.3.1/tests/integration/test_urllib3.py
--rw-r--r--   0 kevin      (501) staff       (20)     3498 2023-05-26 15:56:05.000000 vcrpy-4.3.1/tests/integration/test_wild.py
-drwxr-xr-x   0 kevin      (501) staff       (20)        0 2023-05-26 16:04:05.105452 vcrpy-4.3.1/tests/unit/
--rw-r--r--   0 kevin      (501) staff       (20)    13163 2023-05-24 18:36:09.000000 vcrpy-4.3.1/tests/unit/test_cassettes.py
--rw-r--r--   0 kevin      (501) staff       (20)     2669 2022-08-31 19:12:36.000000 vcrpy-4.3.1/tests/unit/test_errors.py
--rw-r--r--   0 kevin      (501) staff       (20)    11738 2023-05-24 18:36:09.000000 vcrpy-4.3.1/tests/unit/test_filters.py
--rw-r--r--   0 kevin      (501) staff       (20)      611 2023-05-24 18:36:09.000000 vcrpy-4.3.1/tests/unit/test_json_serializer.py
--rw-r--r--   0 kevin      (501) staff       (20)     9990 2023-05-24 18:36:09.000000 vcrpy-4.3.1/tests/unit/test_matchers.py
--rw-r--r--   0 kevin      (501) staff       (20)     1588 2023-05-24 18:36:09.000000 vcrpy-4.3.1/tests/unit/test_migration.py
--rw-r--r--   0 kevin      (501) staff       (20)     1067 2022-08-31 19:12:36.000000 vcrpy-4.3.1/tests/unit/test_persist.py
--rw-r--r--   0 kevin      (501) staff       (20)     2471 2023-05-24 18:36:09.000000 vcrpy-4.3.1/tests/unit/test_request.py
--rw-r--r--   0 kevin      (501) staff       (20)     3648 2022-08-31 19:12:36.000000 vcrpy-4.3.1/tests/unit/test_response.py
--rw-r--r--   0 kevin      (501) staff       (20)     4038 2023-05-24 18:36:09.000000 vcrpy-4.3.1/tests/unit/test_serialize.py
--rw-r--r--   0 kevin      (501) staff       (20)      798 2023-05-24 18:36:09.000000 vcrpy-4.3.1/tests/unit/test_stubs.py
--rw-r--r--   0 kevin      (501) staff       (20)    12082 2023-05-26 15:56:05.000000 vcrpy-4.3.1/tests/unit/test_vcr.py
--rw-r--r--   0 kevin      (501) staff       (20)      395 2023-05-24 18:36:09.000000 vcrpy-4.3.1/tests/unit/test_vcr_import.py
--rw-r--r--   0 kevin      (501) staff       (20)     3281 2023-05-26 15:56:05.000000 vcrpy-4.3.1/tox.ini
-drwxr-xr-x   0 kevin      (501) staff       (20)        0 2023-05-26 16:04:05.107080 vcrpy-4.3.1/vcr/
--rw-r--r--   0 kevin      (501) staff       (20)      296 2023-05-26 15:56:45.000000 vcrpy-4.3.1/vcr/__init__.py
--rw-r--r--   0 kevin      (501) staff       (20)      125 2022-08-31 19:12:36.000000 vcrpy-4.3.1/vcr/_handle_coroutine.py
--rw-r--r--   0 kevin      (501) staff       (20)    13892 2023-05-24 18:36:09.000000 vcrpy-4.3.1/vcr/cassette.py
--rw-r--r--   0 kevin      (501) staff       (20)    10830 2023-05-24 18:36:09.000000 vcrpy-4.3.1/vcr/config.py
--rw-r--r--   0 kevin      (501) staff       (20)     1976 2022-08-31 19:12:36.000000 vcrpy-4.3.1/vcr/errors.py
--rw-r--r--   0 kevin      (501) staff       (20)     6651 2023-05-24 18:36:09.000000 vcrpy-4.3.1/vcr/filters.py
--rw-r--r--   0 kevin      (501) staff       (20)     4105 2023-05-24 18:36:09.000000 vcrpy-4.3.1/vcr/matchers.py
--rw-r--r--   0 kevin      (501) staff       (20)     4660 2023-05-24 18:36:09.000000 vcrpy-4.3.1/vcr/migration.py
--rw-r--r--   0 kevin      (501) staff       (20)    17948 2023-05-26 15:56:05.000000 vcrpy-4.3.1/vcr/patch.py
-drwxr-xr-x   0 kevin      (501) staff       (20)        0 2023-05-26 16:04:05.107272 vcrpy-4.3.1/vcr/persisters/
--rw-r--r--   0 kevin      (501) staff       (20)        0 2022-08-31 19:12:36.000000 vcrpy-4.3.1/vcr/persisters/__init__.py
--rw-r--r--   0 kevin      (501) staff       (20)     1095 2023-05-24 18:36:09.000000 vcrpy-4.3.1/vcr/persisters/filesystem.py
--rw-r--r--   0 kevin      (501) staff       (20)      630 2022-08-31 19:12:36.000000 vcrpy-4.3.1/vcr/record_mode.py
--rw-r--r--   0 kevin      (501) staff       (20)     3782 2023-05-24 18:36:09.000000 vcrpy-4.3.1/vcr/request.py
--rw-r--r--   0 kevin      (501) staff       (20)     2124 2023-05-24 18:36:09.000000 vcrpy-4.3.1/vcr/serialize.py
-drwxr-xr-x   0 kevin      (501) staff       (20)        0 2023-05-26 16:04:05.107670 vcrpy-4.3.1/vcr/serializers/
--rw-r--r--   0 kevin      (501) staff       (20)        0 2022-08-31 19:12:36.000000 vcrpy-4.3.1/vcr/serializers/__init__.py
--rw-r--r--   0 kevin      (501) staff       (20)     2513 2022-08-31 19:12:36.000000 vcrpy-4.3.1/vcr/serializers/compat.py
--rw-r--r--   0 kevin      (501) staff       (20)      778 2022-08-31 19:12:36.000000 vcrpy-4.3.1/vcr/serializers/jsonserializer.py
--rw-r--r--   0 kevin      (501) staff       (20)      363 2023-05-24 18:36:09.000000 vcrpy-4.3.1/vcr/serializers/yamlserializer.py
-drwxr-xr-x   0 kevin      (501) staff       (20)        0 2023-05-26 16:04:05.108691 vcrpy-4.3.1/vcr/stubs/
--rw-r--r--   0 kevin      (501) staff       (20)    13412 2023-05-26 15:56:05.000000 vcrpy-4.3.1/vcr/stubs/__init__.py
--rw-r--r--   0 kevin      (501) staff       (20)     9954 2023-05-24 18:36:09.000000 vcrpy-4.3.1/vcr/stubs/aiohttp_stubs.py
--rw-r--r--   0 kevin      (501) staff       (20)     1202 2023-05-24 18:36:09.000000 vcrpy-4.3.1/vcr/stubs/boto3_stubs.py
--rw-r--r--   0 kevin      (501) staff       (20)      235 2023-05-24 18:36:09.000000 vcrpy-4.3.1/vcr/stubs/boto_stubs.py
--rw-r--r--   0 kevin      (501) staff       (20)      578 2023-05-24 18:36:09.000000 vcrpy-4.3.1/vcr/stubs/compat.py
--rw-r--r--   0 kevin      (501) staff       (20)     2166 2023-05-24 18:36:09.000000 vcrpy-4.3.1/vcr/stubs/httplib2_stubs.py
--rw-r--r--   0 kevin      (501) staff       (20)     5579 2023-05-24 18:36:09.000000 vcrpy-4.3.1/vcr/stubs/httpx_stubs.py
--rw-r--r--   0 kevin      (501) staff       (20)      558 2023-05-26 15:56:05.000000 vcrpy-4.3.1/vcr/stubs/requests_stubs.py
--rw-r--r--   0 kevin      (501) staff       (20)     3407 2022-08-31 19:12:36.000000 vcrpy-4.3.1/vcr/stubs/tornado_stubs.py
--rw-r--r--   0 kevin      (501) staff       (20)      504 2023-05-26 15:56:05.000000 vcrpy-4.3.1/vcr/stubs/urllib3_stubs.py
--rw-r--r--   0 kevin      (501) staff       (20)     3882 2022-08-31 19:12:36.000000 vcrpy-4.3.1/vcr/util.py
-drwxr-xr-x   0 kevin      (501) staff       (20)        0 2023-05-26 16:04:05.109201 vcrpy-4.3.1/vcrpy.egg-info/
--rw-r--r--   0 kevin      (501) staff       (20)     3925 2023-05-26 16:04:05.000000 vcrpy-4.3.1/vcrpy.egg-info/PKG-INFO
--rw-r--r--   0 kevin      (501) staff       (20)     2650 2023-05-26 16:04:05.000000 vcrpy-4.3.1/vcrpy.egg-info/SOURCES.txt
--rw-r--r--   0 kevin      (501) staff       (20)        1 2023-05-26 16:04:05.000000 vcrpy-4.3.1/vcrpy.egg-info/dependency_links.txt
--rw-r--r--   0 kevin      (501) staff       (20)       65 2023-05-26 16:04:05.000000 vcrpy-4.3.1/vcrpy.egg-info/requires.txt
--rw-r--r--   0 kevin      (501) staff       (20)        4 2023-05-26 16:04:05.000000 vcrpy-4.3.1/vcrpy.egg-info/top_level.txt
+drwxr-xr-x   0 kevin     (1000) kevin     (1000)        0 2023-06-26 14:20:09.906139 vcrpy-4.4.0/
+-rw-r--r--   0 kevin     (1000) kevin     (1000)     1063 2023-06-26 14:02:48.000000 vcrpy-4.4.0/LICENSE.txt
+-rw-r--r--   0 kevin     (1000) kevin     (1000)      142 2023-06-26 14:02:48.000000 vcrpy-4.4.0/MANIFEST.in
+-rw-r--r--   0 kevin     (1000) kevin     (1000)     3925 2023-06-26 14:20:09.906139 vcrpy-4.4.0/PKG-INFO
+-rw-r--r--   0 kevin     (1000) kevin     (1000)     2767 2023-06-26 14:02:48.000000 vcrpy-4.4.0/README.rst
+-rw-r--r--   0 kevin     (1000) kevin     (1000)      325 2023-06-26 14:02:48.000000 vcrpy-4.4.0/pyproject.toml
+-rw-r--r--   0 kevin     (1000) kevin     (1000)       67 2023-06-26 14:20:09.906139 vcrpy-4.4.0/setup.cfg
+-rw-r--r--   0 kevin     (1000) kevin     (1000)     3557 2023-06-26 14:02:48.000000 vcrpy-4.4.0/setup.py
+drwxr-xr-x   0 kevin     (1000) kevin     (1000)        0 2023-06-26 14:20:09.906139 vcrpy-4.4.0/tests/
+-rw-r--r--   0 kevin     (1000) kevin     (1000)      354 2023-06-26 14:02:48.000000 vcrpy-4.4.0/tests/assertions.py
+drwxr-xr-x   0 kevin     (1000) kevin     (1000)        0 2023-06-26 14:20:09.906139 vcrpy-4.4.0/tests/fixtures/
+drwxr-xr-x   0 kevin     (1000) kevin     (1000)        0 2023-06-26 14:20:09.906139 vcrpy-4.4.0/tests/fixtures/migration/
+-rw-r--r--   0 kevin     (1000) kevin     (1000)     1115 2023-06-26 14:02:48.000000 vcrpy-4.4.0/tests/fixtures/migration/new_cassette.json
+-rw-r--r--   0 kevin     (1000) kevin     (1000)      599 2023-06-26 14:02:48.000000 vcrpy-4.4.0/tests/fixtures/migration/new_cassette.yaml
+-rw-r--r--   0 kevin     (1000) kevin     (1000)       23 2023-06-26 14:02:48.000000 vcrpy-4.4.0/tests/fixtures/migration/not_cassette.txt
+-rw-r--r--   0 kevin     (1000) kevin     (1000)     1031 2023-06-26 14:02:48.000000 vcrpy-4.4.0/tests/fixtures/migration/old_cassette.json
+-rw-r--r--   0 kevin     (1000) kevin     (1000)      869 2023-06-26 14:02:48.000000 vcrpy-4.4.0/tests/fixtures/migration/old_cassette.yaml
+drwxr-xr-x   0 kevin     (1000) kevin     (1000)        0 2023-06-26 14:20:09.906139 vcrpy-4.4.0/tests/fixtures/wild/
+-rw-r--r--   0 kevin     (1000) kevin     (1000)     9705 2023-06-26 14:02:48.000000 vcrpy-4.4.0/tests/fixtures/wild/domain_redirect.yaml
+drwxr-xr-x   0 kevin     (1000) kevin     (1000)        0 2023-06-26 14:20:09.906139 vcrpy-4.4.0/tests/integration/
+-rw-r--r--   0 kevin     (1000) kevin     (1000)        0 2023-06-26 14:02:48.000000 vcrpy-4.4.0/tests/integration/__init__.py
+-rw-r--r--   0 kevin     (1000) kevin     (1000)     1214 2023-06-26 14:02:48.000000 vcrpy-4.4.0/tests/integration/aiohttp_utils.py
+drwxr-xr-x   0 kevin     (1000) kevin     (1000)        0 2023-06-26 14:20:09.906139 vcrpy-4.4.0/tests/integration/cassettes/
+-rw-r--r--   0 kevin     (1000) kevin     (1000)     1017 2023-06-26 14:02:48.000000 vcrpy-4.4.0/tests/integration/cassettes/test_httpx_test_test_behind_proxy.yml
+-rw-r--r--   0 kevin     (1000) kevin     (1000)      781 2023-06-26 14:02:48.000000 vcrpy-4.4.0/tests/integration/conftest.py
+-rw-r--r--   0 kevin     (1000) kevin     (1000)    16816 2023-06-26 14:02:48.000000 vcrpy-4.4.0/tests/integration/test_aiohttp.py
+-rw-r--r--   0 kevin     (1000) kevin     (1000)     2766 2023-06-26 14:02:48.000000 vcrpy-4.4.0/tests/integration/test_basic.py
+-rw-r--r--   0 kevin     (1000) kevin     (1000)     2951 2023-06-26 14:02:48.000000 vcrpy-4.4.0/tests/integration/test_boto.py
+-rw-r--r--   0 kevin     (1000) kevin     (1000)     3589 2023-06-26 14:02:48.000000 vcrpy-4.4.0/tests/integration/test_boto3.py
+-rw-r--r--   0 kevin     (1000) kevin     (1000)     2626 2023-06-26 14:02:48.000000 vcrpy-4.4.0/tests/integration/test_config.py
+-rw-r--r--   0 kevin     (1000) kevin     (1000)     1618 2023-06-26 14:02:48.000000 vcrpy-4.4.0/tests/integration/test_disksaver.py
+-rw-r--r--   0 kevin     (1000) kevin     (1000)     6402 2023-06-26 14:02:48.000000 vcrpy-4.4.0/tests/integration/test_filter.py
+-rw-r--r--   0 kevin     (1000) kevin     (1000)     1030 2023-06-26 14:02:48.000000 vcrpy-4.4.0/tests/integration/test_http
+-rw-r--r--   0 kevin     (1000) kevin     (1000)     4946 2023-06-26 14:02:48.000000 vcrpy-4.4.0/tests/integration/test_httplib2.py
+-rw-r--r--   0 kevin     (1000) kevin     (1000)    10635 2023-06-26 14:02:48.000000 vcrpy-4.4.0/tests/integration/test_httpx.py
+-rw-r--r--   0 kevin     (1000) kevin     (1000)     2621 2023-06-26 14:02:48.000000 vcrpy-4.4.0/tests/integration/test_ignore.py
+-rw-r--r--   0 kevin     (1000) kevin     (1000)     4000 2023-06-26 14:02:48.000000 vcrpy-4.4.0/tests/integration/test_matchers.py
+-rw-r--r--   0 kevin     (1000) kevin     (1000)      878 2023-06-26 14:02:48.000000 vcrpy-4.4.0/tests/integration/test_multiple.py
+-rw-r--r--   0 kevin     (1000) kevin     (1000)     1779 2023-06-26 14:02:48.000000 vcrpy-4.4.0/tests/integration/test_proxy.py
+-rw-r--r--   0 kevin     (1000) kevin     (1000)     5170 2023-06-26 14:02:48.000000 vcrpy-4.4.0/tests/integration/test_record_mode.py
+-rw-r--r--   0 kevin     (1000) kevin     (1000)     1222 2023-06-26 14:02:48.000000 vcrpy-4.4.0/tests/integration/test_register_matcher.py
+-rw-r--r--   0 kevin     (1000) kevin     (1000)     1844 2023-06-26 14:02:48.000000 vcrpy-4.4.0/tests/integration/test_register_persister.py
+-rw-r--r--   0 kevin     (1000) kevin     (1000)      962 2023-06-26 14:02:48.000000 vcrpy-4.4.0/tests/integration/test_register_serializer.py
+-rw-r--r--   0 kevin     (1000) kevin     (1000)      739 2023-06-26 14:02:48.000000 vcrpy-4.4.0/tests/integration/test_request.py
+-rw-r--r--   0 kevin     (1000) kevin     (1000)    13174 2023-06-26 14:02:48.000000 vcrpy-4.4.0/tests/integration/test_requests.py
+-rw-r--r--   0 kevin     (1000) kevin     (1000)     5040 2023-06-26 14:02:48.000000 vcrpy-4.4.0/tests/integration/test_stubs.py
+-rw-r--r--   0 kevin     (1000) kevin     (1000)    12599 2023-06-26 14:02:48.000000 vcrpy-4.4.0/tests/integration/test_tornado.py
+-rw-r--r--   0 kevin     (1000) kevin     (1000)     1387 2023-06-26 14:02:48.000000 vcrpy-4.4.0/tests/integration/test_tornado_exception_can_be_caught.yaml
+-rw-r--r--   0 kevin     (1000) kevin     (1000)     1566 2023-06-26 14:02:48.000000 vcrpy-4.4.0/tests/integration/test_tornado_with_decorator_use_cassette.yaml
+-rw-r--r--   0 kevin     (1000) kevin     (1000)     5109 2023-06-26 14:02:48.000000 vcrpy-4.4.0/tests/integration/test_urllib2.py
+-rw-r--r--   0 kevin     (1000) kevin     (1000)     6384 2023-06-26 14:02:48.000000 vcrpy-4.4.0/tests/integration/test_urllib3.py
+-rw-r--r--   0 kevin     (1000) kevin     (1000)     3538 2023-06-26 14:02:48.000000 vcrpy-4.4.0/tests/integration/test_wild.py
+drwxr-xr-x   0 kevin     (1000) kevin     (1000)        0 2023-06-26 14:20:09.906139 vcrpy-4.4.0/tests/unit/
+-rw-r--r--   0 kevin     (1000) kevin     (1000)    13163 2023-06-26 14:02:48.000000 vcrpy-4.4.0/tests/unit/test_cassettes.py
+-rw-r--r--   0 kevin     (1000) kevin     (1000)     2669 2023-06-26 14:02:48.000000 vcrpy-4.4.0/tests/unit/test_errors.py
+-rw-r--r--   0 kevin     (1000) kevin     (1000)    12401 2023-06-26 14:02:48.000000 vcrpy-4.4.0/tests/unit/test_filters.py
+-rw-r--r--   0 kevin     (1000) kevin     (1000)      611 2023-06-26 14:02:48.000000 vcrpy-4.4.0/tests/unit/test_json_serializer.py
+-rw-r--r--   0 kevin     (1000) kevin     (1000)     9990 2023-06-26 14:02:48.000000 vcrpy-4.4.0/tests/unit/test_matchers.py
+-rw-r--r--   0 kevin     (1000) kevin     (1000)     1588 2023-06-26 14:02:48.000000 vcrpy-4.4.0/tests/unit/test_migration.py
+-rw-r--r--   0 kevin     (1000) kevin     (1000)     1067 2023-06-26 14:02:48.000000 vcrpy-4.4.0/tests/unit/test_persist.py
+-rw-r--r--   0 kevin     (1000) kevin     (1000)     2471 2023-06-26 14:02:48.000000 vcrpy-4.4.0/tests/unit/test_request.py
+-rw-r--r--   0 kevin     (1000) kevin     (1000)     3629 2023-06-26 14:02:48.000000 vcrpy-4.4.0/tests/unit/test_response.py
+-rw-r--r--   0 kevin     (1000) kevin     (1000)     4038 2023-06-26 14:02:48.000000 vcrpy-4.4.0/tests/unit/test_serialize.py
+-rw-r--r--   0 kevin     (1000) kevin     (1000)      840 2023-06-26 14:02:48.000000 vcrpy-4.4.0/tests/unit/test_stubs.py
+-rw-r--r--   0 kevin     (1000) kevin     (1000)     5580 2023-06-26 14:02:48.000000 vcrpy-4.4.0/tests/unit/test_unittest.py
+-rw-r--r--   0 kevin     (1000) kevin     (1000)    12082 2023-06-26 14:02:48.000000 vcrpy-4.4.0/tests/unit/test_vcr.py
+-rw-r--r--   0 kevin     (1000) kevin     (1000)      395 2023-06-26 14:02:48.000000 vcrpy-4.4.0/tests/unit/test_vcr_import.py
+-rw-r--r--   0 kevin     (1000) kevin     (1000)     3281 2023-06-26 14:02:48.000000 vcrpy-4.4.0/tox.ini
+drwxr-xr-x   0 kevin     (1000) kevin     (1000)        0 2023-06-26 14:20:09.906139 vcrpy-4.4.0/vcr/
+-rw-r--r--   0 kevin     (1000) kevin     (1000)      296 2023-06-26 14:17:30.000000 vcrpy-4.4.0/vcr/__init__.py
+-rw-r--r--   0 kevin     (1000) kevin     (1000)      125 2023-06-26 14:02:48.000000 vcrpy-4.4.0/vcr/_handle_coroutine.py
+-rw-r--r--   0 kevin     (1000) kevin     (1000)    13892 2023-06-26 14:02:48.000000 vcrpy-4.4.0/vcr/cassette.py
+-rw-r--r--   0 kevin     (1000) kevin     (1000)    10834 2023-06-26 14:02:48.000000 vcrpy-4.4.0/vcr/config.py
+-rw-r--r--   0 kevin     (1000) kevin     (1000)     1976 2023-06-26 14:02:48.000000 vcrpy-4.4.0/vcr/errors.py
+-rw-r--r--   0 kevin     (1000) kevin     (1000)     6911 2023-06-26 14:02:48.000000 vcrpy-4.4.0/vcr/filters.py
+-rw-r--r--   0 kevin     (1000) kevin     (1000)     4365 2023-06-26 14:02:48.000000 vcrpy-4.4.0/vcr/matchers.py
+-rw-r--r--   0 kevin     (1000) kevin     (1000)     4662 2023-06-26 14:02:48.000000 vcrpy-4.4.0/vcr/migration.py
+-rw-r--r--   0 kevin     (1000) kevin     (1000)    17948 2023-06-26 14:02:48.000000 vcrpy-4.4.0/vcr/patch.py
+drwxr-xr-x   0 kevin     (1000) kevin     (1000)        0 2023-06-26 14:20:09.906139 vcrpy-4.4.0/vcr/persisters/
+-rw-r--r--   0 kevin     (1000) kevin     (1000)        0 2023-06-26 14:02:48.000000 vcrpy-4.4.0/vcr/persisters/__init__.py
+-rw-r--r--   0 kevin     (1000) kevin     (1000)     1095 2023-06-26 14:02:48.000000 vcrpy-4.4.0/vcr/persisters/filesystem.py
+-rw-r--r--   0 kevin     (1000) kevin     (1000)      630 2023-06-26 14:02:48.000000 vcrpy-4.4.0/vcr/record_mode.py
+-rw-r--r--   0 kevin     (1000) kevin     (1000)     3782 2023-06-26 14:02:48.000000 vcrpy-4.4.0/vcr/request.py
+-rw-r--r--   0 kevin     (1000) kevin     (1000)     2124 2023-06-26 14:02:48.000000 vcrpy-4.4.0/vcr/serialize.py
+drwxr-xr-x   0 kevin     (1000) kevin     (1000)        0 2023-06-26 14:20:09.906139 vcrpy-4.4.0/vcr/serializers/
+-rw-r--r--   0 kevin     (1000) kevin     (1000)        0 2023-06-26 14:02:48.000000 vcrpy-4.4.0/vcr/serializers/__init__.py
+-rw-r--r--   0 kevin     (1000) kevin     (1000)     2513 2023-06-26 14:02:48.000000 vcrpy-4.4.0/vcr/serializers/compat.py
+-rw-r--r--   0 kevin     (1000) kevin     (1000)      778 2023-06-26 14:02:48.000000 vcrpy-4.4.0/vcr/serializers/jsonserializer.py
+-rw-r--r--   0 kevin     (1000) kevin     (1000)      363 2023-06-26 14:02:48.000000 vcrpy-4.4.0/vcr/serializers/yamlserializer.py
+drwxr-xr-x   0 kevin     (1000) kevin     (1000)        0 2023-06-26 14:20:09.906139 vcrpy-4.4.0/vcr/stubs/
+-rw-r--r--   0 kevin     (1000) kevin     (1000)    13682 2023-06-26 14:02:48.000000 vcrpy-4.4.0/vcr/stubs/__init__.py
+-rw-r--r--   0 kevin     (1000) kevin     (1000)     9954 2023-06-26 14:02:48.000000 vcrpy-4.4.0/vcr/stubs/aiohttp_stubs.py
+-rw-r--r--   0 kevin     (1000) kevin     (1000)     1202 2023-06-26 14:02:48.000000 vcrpy-4.4.0/vcr/stubs/boto3_stubs.py
+-rw-r--r--   0 kevin     (1000) kevin     (1000)      235 2023-06-26 14:02:48.000000 vcrpy-4.4.0/vcr/stubs/boto_stubs.py
+-rw-r--r--   0 kevin     (1000) kevin     (1000)      578 2023-06-26 14:02:48.000000 vcrpy-4.4.0/vcr/stubs/compat.py
+-rw-r--r--   0 kevin     (1000) kevin     (1000)     2166 2023-06-26 14:02:48.000000 vcrpy-4.4.0/vcr/stubs/httplib2_stubs.py
+-rw-r--r--   0 kevin     (1000) kevin     (1000)     5579 2023-06-26 14:02:48.000000 vcrpy-4.4.0/vcr/stubs/httpx_stubs.py
+-rw-r--r--   0 kevin     (1000) kevin     (1000)      558 2023-06-26 14:02:48.000000 vcrpy-4.4.0/vcr/stubs/requests_stubs.py
+-rw-r--r--   0 kevin     (1000) kevin     (1000)     3407 2023-06-26 14:02:48.000000 vcrpy-4.4.0/vcr/stubs/tornado_stubs.py
+-rw-r--r--   0 kevin     (1000) kevin     (1000)      504 2023-06-26 14:02:48.000000 vcrpy-4.4.0/vcr/stubs/urllib3_stubs.py
+-rw-r--r--   0 kevin     (1000) kevin     (1000)     1086 2023-06-26 14:02:48.000000 vcrpy-4.4.0/vcr/unittest.py
+-rw-r--r--   0 kevin     (1000) kevin     (1000)     3882 2023-06-26 14:02:48.000000 vcrpy-4.4.0/vcr/util.py
+drwxr-xr-x   0 kevin     (1000) kevin     (1000)        0 2023-06-26 14:20:09.906139 vcrpy-4.4.0/vcrpy.egg-info/
+-rw-r--r--   0 kevin     (1000) kevin     (1000)     3925 2023-06-26 14:20:09.000000 vcrpy-4.4.0/vcrpy.egg-info/PKG-INFO
+-rw-r--r--   0 kevin     (1000) kevin     (1000)     2694 2023-06-26 14:20:09.000000 vcrpy-4.4.0/vcrpy.egg-info/SOURCES.txt
+-rw-r--r--   0 kevin     (1000) kevin     (1000)        1 2023-06-26 14:20:09.000000 vcrpy-4.4.0/vcrpy.egg-info/dependency_links.txt
+-rw-r--r--   0 kevin     (1000) kevin     (1000)       65 2023-06-26 14:20:09.000000 vcrpy-4.4.0/vcrpy.egg-info/requires.txt
+-rw-r--r--   0 kevin     (1000) kevin     (1000)        4 2023-06-26 14:20:09.000000 vcrpy-4.4.0/vcrpy.egg-info/top_level.txt
```

### Comparing `vcrpy-4.3.1/LICENSE.txt` & `vcrpy-4.4.0/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `vcrpy-4.3.1/PKG-INFO` & `vcrpy-4.4.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: vcrpy
-Version: 4.3.1
+Version: 4.4.0
 Summary: Automatically mock your HTTP interactions to simplify and speed up testing
 Home-page: https://github.com/kevin1024/vcrpy
 Author: Kevin McCarthy
 Author-email: me@kevinmccarthy.org
 License: MIT
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Environment :: Console
```

### Comparing `vcrpy-4.3.1/README.rst` & `vcrpy-4.4.0/README.rst`

 * *Files identical despite different names*

### Comparing `vcrpy-4.3.1/setup.py` & `vcrpy-4.4.0/setup.py`

 * *Files identical despite different names*

### Comparing `vcrpy-4.3.1/tests/fixtures/migration/new_cassette.json` & `vcrpy-4.4.0/tests/fixtures/migration/new_cassette.json`

 * *Files identical despite different names*

### Comparing `vcrpy-4.3.1/tests/fixtures/migration/new_cassette.yaml` & `vcrpy-4.4.0/tests/fixtures/migration/new_cassette.yaml`

 * *Files identical despite different names*

### Comparing `vcrpy-4.3.1/tests/fixtures/migration/old_cassette.json` & `vcrpy-4.4.0/tests/fixtures/migration/old_cassette.json`

 * *Files identical despite different names*

### Comparing `vcrpy-4.3.1/tests/fixtures/migration/old_cassette.yaml` & `vcrpy-4.4.0/tests/fixtures/migration/old_cassette.yaml`

 * *Files identical despite different names*

### Comparing `vcrpy-4.3.1/tests/fixtures/wild/domain_redirect.yaml` & `vcrpy-4.4.0/tests/fixtures/wild/domain_redirect.yaml`

 * *Files identical despite different names*

### Comparing `vcrpy-4.3.1/tests/integration/aiohttp_utils.py` & `vcrpy-4.4.0/tests/integration/aiohttp_utils.py`

 * *Files identical despite different names*

### Comparing `vcrpy-4.3.1/tests/integration/cassettes/test_httpx_test_test_behind_proxy.yml` & `vcrpy-4.4.0/tests/integration/cassettes/test_httpx_test_test_behind_proxy.yml`

 * *Files identical despite different names*

### Comparing `vcrpy-4.3.1/tests/integration/conftest.py` & `vcrpy-4.4.0/tests/integration/conftest.py`

 * *Files identical despite different names*

### Comparing `vcrpy-4.3.1/tests/integration/test_aiohttp.py` & `vcrpy-4.4.0/tests/integration/test_aiohttp.py`

 * *Files 7% similar despite different names*

```diff
@@ -30,26 +30,28 @@
     return request("GET", url, output=output, **kwargs)
 
 
 def post(url, output="text", **kwargs):
     return request("POST", url, output="text", **kwargs)
 
 
+@pytest.mark.online
 def test_status(tmpdir, mockbin_request_url):
     url = mockbin_request_url
 
     with vcr.use_cassette(str(tmpdir.join("status.yaml"))):
         response, _ = get(url)
 
     with vcr.use_cassette(str(tmpdir.join("status.yaml"))) as cassette:
         cassette_response, _ = get(url)
         assert cassette_response.status == response.status
         assert cassette.play_count == 1
 
 
+@pytest.mark.online
 @pytest.mark.parametrize("auth", [None, aiohttp.BasicAuth("vcrpy", "test")])
 def test_headers(tmpdir, auth, mockbin_request_url):
     url = mockbin_request_url
     with vcr.use_cassette(str(tmpdir.join("headers.yaml"))):
         response, _ = get(url, auth=auth)
 
     with vcr.use_cassette(str(tmpdir.join("headers.yaml"))) as cassette:
@@ -59,75 +61,81 @@
         cassette_response, _ = get(url, auth=auth)
         assert dict(cassette_response.headers) == dict(response.headers)
         assert cassette.play_count == 1
         assert "istr" not in cassette.data[0]
         assert "yarl.URL" not in cassette.data[0]
 
 
+@pytest.mark.online
 def test_case_insensitive_headers(tmpdir, mockbin_request_url):
     url = mockbin_request_url
 
     with vcr.use_cassette(str(tmpdir.join("whatever.yaml"))):
         _, _ = get(url)
 
     with vcr.use_cassette(str(tmpdir.join("whatever.yaml"))) as cassette:
         cassette_response, _ = get(url)
         assert "Content-Type" in cassette_response.headers
         assert "content-type" in cassette_response.headers
         assert cassette.play_count == 1
 
 
+@pytest.mark.online
 def test_text(tmpdir, mockbin_request_url):
     url = mockbin_request_url
 
     with vcr.use_cassette(str(tmpdir.join("text.yaml"))):
         _, response_text = get(url)
 
     with vcr.use_cassette(str(tmpdir.join("text.yaml"))) as cassette:
         _, cassette_response_text = get(url)
         assert cassette_response_text == response_text
         assert cassette.play_count == 1
 
 
+@pytest.mark.online
 def test_json(tmpdir, mockbin_request_url):
     url = mockbin_request_url
     headers = {"Content-Type": "application/json"}
 
     with vcr.use_cassette(str(tmpdir.join("json.yaml"))):
         _, response_json = get(url, output="json", headers=headers)
 
     with vcr.use_cassette(str(tmpdir.join("json.yaml"))) as cassette:
         _, cassette_response_json = get(url, output="json", headers=headers)
         assert cassette_response_json == response_json
         assert cassette.play_count == 1
 
 
+@pytest.mark.online
 def test_binary(tmpdir, mockbin_request_url):
     url = mockbin_request_url + "/image/png"
     with vcr.use_cassette(str(tmpdir.join("binary.yaml"))):
         _, response_binary = get(url, output="raw")
 
     with vcr.use_cassette(str(tmpdir.join("binary.yaml"))) as cassette:
         _, cassette_response_binary = get(url, output="raw")
         assert cassette_response_binary == response_binary
         assert cassette.play_count == 1
 
 
+@pytest.mark.online
 def test_stream(tmpdir, mockbin_request_url):
     url = mockbin_request_url
 
     with vcr.use_cassette(str(tmpdir.join("stream.yaml"))):
         _, body = get(url, output="raw")  # Do not use stream here, as the stream is exhausted by vcr
 
     with vcr.use_cassette(str(tmpdir.join("stream.yaml"))) as cassette:
         _, cassette_body = get(url, output="stream")
         assert cassette_body == body
         assert cassette.play_count == 1
 
 
+@pytest.mark.online
 @pytest.mark.parametrize("body", ["data", "json"])
 def test_post(tmpdir, body, caplog, mockbin_request_url):
     caplog.set_level(logging.INFO)
     data = {"key1": "value1", "key2": "value2"}
     url = mockbin_request_url
     with vcr.use_cassette(str(tmpdir.join("post.yaml"))):
         _, response_json = post(url, **{body: data})
@@ -145,14 +153,15 @@
             for log in caplog.records
             if log.getMessage() == "<Request (POST) {}> not in cassette, sending to real server".format(url)
         ),
         None,
     ), "Log message not found."
 
 
+@pytest.mark.online
 def test_params(tmpdir, mockbin_request_url):
     url = mockbin_request_url + "?d=d"
     headers = {"Content-Type": "application/json"}
     params = {"a": 1, "b": 2, "c": "c"}
 
     with vcr.use_cassette(str(tmpdir.join("get.yaml"))) as cassette:
         _, response_json = get(url, output="json", params=params, headers=headers)
@@ -160,14 +169,15 @@
 
     with vcr.use_cassette(str(tmpdir.join("get.yaml"))) as cassette:
         _, cassette_response_json = get(url, output="json", params=params, headers=headers)
         assert cassette_response_json == response_json
         assert cassette.play_count == 1
 
 
+@pytest.mark.online
 def test_params_same_url_distinct_params(tmpdir, mockbin_request_url):
     url = mockbin_request_url
     headers = {"Content-Type": "application/json"}
     params = {"a": 1, "b": 2, "c": "c"}
 
     with vcr.use_cassette(str(tmpdir.join("get.yaml"))) as cassette:
         _, response_json = get(url, output="json", params=params, headers=headers)
@@ -179,14 +189,15 @@
 
     other_params = {"other": "params"}
     with vcr.use_cassette(str(tmpdir.join("get.yaml"))) as cassette:
         with pytest.raises(vcr.errors.CannotOverwriteExistingCassetteException):
             get(url, output="text", params=other_params)
 
 
+@pytest.mark.online
 def test_params_on_url(tmpdir, mockbin_request_url):
     url = mockbin_request_url + "?a=1&b=foo"
     headers = {"Content-Type": "application/json"}
 
     with vcr.use_cassette(str(tmpdir.join("get.yaml"))) as cassette:
         _, response_json = get(url, output="json", headers=headers)
         request = cassette.requests[0]
@@ -244,14 +255,15 @@
     request = cassette.requests[0]
     assert request.url == str(client.make_url(url))
     response_json = loop.run_until_complete(response.json())
     assert response_json is None
     assert cassette.play_count == 1
 
 
+@pytest.mark.online
 def test_redirect(tmpdir, mockbin):
     url = mockbin + "/redirect/302/2"
 
     with vcr.use_cassette(str(tmpdir.join("redirect.yaml"))):
         response, _ = get(url)
 
     with vcr.use_cassette(str(tmpdir.join("redirect.yaml"))) as cassette:
@@ -268,14 +280,15 @@
     assert cassette_response.request_info.method == response.request_info.method
     assert {k: v for k, v in cassette_response.request_info.headers.items()} == {
         k: v for k, v in response.request_info.headers.items()
     }
     assert cassette_response.request_info.real_url == response.request_info.real_url
 
 
+@pytest.mark.online
 def test_not_modified(tmpdir, mockbin):
     """It doesn't try to redirect on 304"""
     url = mockbin + "/status/304"
 
     with vcr.use_cassette(str(tmpdir.join("not_modified.yaml"))):
         response, _ = get(url)
 
@@ -285,14 +298,15 @@
         assert cassette_response.status == 304
         assert response.status == 304
         assert len(cassette_response.history) == len(response.history)
         assert len(cassette) == 1
         assert cassette.play_count == 1
 
 
+@pytest.mark.online
 def test_double_requests(tmpdir, mockbin_request_url):
     """We should capture, record, and replay all requests and response chains,
     even if there are duplicate ones.
 
     We should replay in the order we saw them.
     """
     url = mockbin_request_url
@@ -400,14 +414,15 @@
                 assert not cookies_resp.cookies
                 cookies = session.cookie_jar.filter_cookies(cookies_url)
                 assert cookies["Cookie_1"].value == "Val_1"
 
     run_in_loop(run)
 
 
+@pytest.mark.online
 def test_not_allow_redirects(tmpdir, mockbin):
     url = mockbin + "/redirect/308/5"
     path = str(tmpdir.join("redirects.yaml"))
 
     with vcr.use_cassette(path):
         response, _ = get(url, allow_redirects=False)
         assert response.url.path == "/redirect/308/5"
```

### Comparing `vcrpy-4.3.1/tests/integration/test_basic.py` & `vcrpy-4.4.0/tests/integration/test_basic.py`

 * *Files identical despite different names*

### Comparing `vcrpy-4.3.1/tests/integration/test_boto.py` & `vcrpy-4.4.0/tests/integration/test_boto.py`

 * *Files identical despite different names*

### Comparing `vcrpy-4.3.1/tests/integration/test_boto3.py` & `vcrpy-4.4.0/tests/integration/test_boto3.py`

 * *Files identical despite different names*

### Comparing `vcrpy-4.3.1/tests/integration/test_config.py` & `vcrpy-4.4.0/tests/integration/test_config.py`

 * *Files 5% similar despite different names*

```diff
@@ -3,48 +3,52 @@
 from urllib.request import urlopen
 
 import pytest
 
 import vcr
 
 
+@pytest.mark.online
 def test_set_serializer_default_config(tmpdir, mockbin_request_url):
     my_vcr = vcr.VCR(serializer="json")
 
     with my_vcr.use_cassette(str(tmpdir.join("test.json"))):
         assert my_vcr.serializer == "json"
         urlopen(mockbin_request_url)
 
     with open(str(tmpdir.join("test.json"))) as f:
         file_content = f.read()
         assert file_content.endswith("\n")
         assert json.loads(file_content)
 
 
+@pytest.mark.online
 def test_default_set_cassette_library_dir(tmpdir, mockbin_request_url):
     my_vcr = vcr.VCR(cassette_library_dir=str(tmpdir.join("subdir")))
 
     with my_vcr.use_cassette("test.json"):
         urlopen(mockbin_request_url)
 
     assert os.path.exists(str(tmpdir.join("subdir").join("test.json")))
 
 
+@pytest.mark.online
 def test_override_set_cassette_library_dir(tmpdir, mockbin_request_url):
     my_vcr = vcr.VCR(cassette_library_dir=str(tmpdir.join("subdir")))
 
     cld = str(tmpdir.join("subdir2"))
 
     with my_vcr.use_cassette("test.json", cassette_library_dir=cld):
         urlopen(mockbin_request_url)
 
     assert os.path.exists(str(tmpdir.join("subdir2").join("test.json")))
     assert not os.path.exists(str(tmpdir.join("subdir").join("test.json")))
 
 
+@pytest.mark.online
 def test_override_match_on(tmpdir, mockbin_request_url):
     my_vcr = vcr.VCR(match_on=["method"])
 
     with my_vcr.use_cassette(str(tmpdir.join("test.json"))):
         urlopen(mockbin_request_url)
 
     with my_vcr.use_cassette(str(tmpdir.join("test.json"))) as cass:
@@ -58,14 +62,15 @@
     my_vcr = vcr.VCR()
     my_vcr.register_matcher("awesome", object)
     with pytest.raises(KeyError):
         with my_vcr.use_cassette("test.yaml", match_on=["notawesome"]):
             pass
 
 
+@pytest.mark.online
 def test_dont_record_on_exception(tmpdir, mockbin_request_url):
     my_vcr = vcr.VCR(record_on_exception=False)
 
     @my_vcr.use_cassette(str(tmpdir.join("dontsave.yml")))
     def some_test():
         assert b"Not in content" in urlopen(mockbin_request_url)
```

### Comparing `vcrpy-4.3.1/tests/integration/test_disksaver.py` & `vcrpy-4.4.0/tests/integration/test_disksaver.py`

 * *Files 10% similar despite different names*

```diff
@@ -2,18 +2,21 @@
 """Basic tests about save behavior"""
 
 # External imports
 import os
 import time
 from urllib.request import urlopen
 
+import pytest
+
 # Internal imports
 import vcr
 
 
+@pytest.mark.online
 def test_disk_saver_nowrite(tmpdir, mockbin_request_url):
     """
     Ensure that when you close a cassette without changing it it doesn't
     rewrite the file
     """
     fname = str(tmpdir.join("synopsis.yaml"))
     with vcr.use_cassette(fname) as cass:
@@ -26,14 +29,15 @@
         assert cass.play_count == 1
         assert cass.dirty is False
     last_mod2 = os.path.getmtime(fname)
 
     assert last_mod == last_mod2
 
 
+@pytest.mark.online
 def test_disk_saver_write(tmpdir, mockbin_request_url):
     """
     Ensure that when you close a cassette after changing it it does
     rewrite the file
     """
     fname = str(tmpdir.join("synopsis.yaml"))
     with vcr.use_cassette(fname) as cass:
```

### Comparing `vcrpy-4.3.1/tests/integration/test_filter.py` & `vcrpy-4.4.0/tests/integration/test_filter.py`

 * *Files 4% similar despite different names*

```diff
@@ -138,7 +138,28 @@
     cass_file = str(tmpdir.join("noncompressed_response.yaml"))
     with vcr.use_cassette(cass_file, decode_compressed_response=True):
         urlopen(url)
     with vcr.use_cassette(cass_file) as cass:
         resp = urlopen(url).read()
         assert_cassette_has_one_response(cass)
     assert_is_json(resp)
+
+
+def test_before_record_request_corruption(tmpdir, httpbin):
+    """Modifying request in before_record_request should not affect outgoing request"""
+
+    def before_record(request):
+        request.headers.clear()
+        request.body = b""
+        return request
+
+    req = Request(
+        httpbin.url + "/post",
+        data=urlencode({"test": "exists"}).encode(),
+        headers={"X-Test": "exists"},
+    )
+    cass_file = str(tmpdir.join("modified_response.yaml"))
+    with vcr.use_cassette(cass_file, before_record_request=before_record):
+        resp = json.loads(urlopen(req).read())
+
+    assert resp["headers"]["X-Test"] == "exists"
+    assert resp["form"]["test"] == "exists"
```

### Comparing `vcrpy-4.3.1/tests/integration/test_http` & `vcrpy-4.4.0/tests/integration/test_http`

 * *Files identical despite different names*

### Comparing `vcrpy-4.3.1/tests/integration/test_httplib2.py` & `vcrpy-4.4.0/tests/integration/test_httplib2.py`

 * *Files 1% similar despite different names*

```diff
@@ -52,14 +52,15 @@
         headers = resp.items()
 
     with vcr.use_cassette(str(tmpdir.join("headers.yaml"))):
         resp, _ = http().request(url)
         assert set(headers) == set(resp.items())
 
 
+@pytest.mark.online
 def test_effective_url(tmpdir):
     """Ensure that the effective_url is captured"""
     url = "http://mockbin.org/redirect/301"
 
     with vcr.use_cassette(str(tmpdir.join("headers.yaml"))):
         resp, _ = http().request(url)
         effective_url = resp["content-location"]
```

### Comparing `vcrpy-4.3.1/tests/integration/test_httpx.py` & `vcrpy-4.4.0/tests/integration/test_httpx.py`

 * *Files 5% similar despite different names*

```diff
@@ -83,65 +83,70 @@
 
 
 @pytest.fixture
 def yml(tmpdir, request):
     return str(tmpdir.join(request.function.__name__ + ".yaml"))
 
 
+@pytest.mark.online
 def test_status(tmpdir, mockbin, do_request):
     url = mockbin
 
     with vcr.use_cassette(str(tmpdir.join("status.yaml"))):
         response = do_request()("GET", url)
 
     with vcr.use_cassette(str(tmpdir.join("status.yaml"))) as cassette:
         cassette_response = do_request()("GET", url)
         assert cassette_response.status_code == response.status_code
         assert cassette.play_count == 1
 
 
+@pytest.mark.online
 def test_case_insensitive_headers(tmpdir, mockbin, do_request):
     url = mockbin
 
     with vcr.use_cassette(str(tmpdir.join("whatever.yaml"))):
         do_request()("GET", url)
 
     with vcr.use_cassette(str(tmpdir.join("whatever.yaml"))) as cassette:
         cassette_response = do_request()("GET", url)
         assert "Content-Type" in cassette_response.headers
         assert "content-type" in cassette_response.headers
         assert cassette.play_count == 1
 
 
+@pytest.mark.online
 def test_content(tmpdir, mockbin, do_request):
     url = mockbin
 
     with vcr.use_cassette(str(tmpdir.join("cointent.yaml"))):
         response = do_request()("GET", url)
 
     with vcr.use_cassette(str(tmpdir.join("cointent.yaml"))) as cassette:
         cassette_response = do_request()("GET", url)
         assert cassette_response.content == response.content
         assert cassette.play_count == 1
 
 
+@pytest.mark.online
 def test_json(tmpdir, mockbin, do_request):
     url = mockbin + "/request"
 
     headers = {"content-type": "application/json"}
 
     with vcr.use_cassette(str(tmpdir.join("json.yaml"))):
         response = do_request(headers=headers)("GET", url)
 
     with vcr.use_cassette(str(tmpdir.join("json.yaml"))) as cassette:
         cassette_response = do_request(headers=headers)("GET", url)
         assert cassette_response.json() == response.json()
         assert cassette.play_count == 1
 
 
+@pytest.mark.online
 def test_params_same_url_distinct_params(tmpdir, mockbin, do_request):
     url = mockbin + "/request"
     headers = {"Content-Type": "application/json"}
     params = {"a": 1, "b": False, "c": "c"}
 
     with vcr.use_cassette(str(tmpdir.join("get.yaml"))) as cassette:
         response = do_request()("GET", url, params=params, headers=headers)
@@ -154,14 +159,15 @@
 
     params = {"other": "params"}
     with vcr.use_cassette(str(tmpdir.join("get.yaml"))) as cassette:
         with pytest.raises(vcr.errors.CannotOverwriteExistingCassetteException):
             do_request()("GET", url, params=params, headers=headers)
 
 
+@pytest.mark.online
 def test_redirect(mockbin, yml, do_request):
     url = mockbin + "/redirect/303/2"
 
     redirect_kwargs = {HTTPX_REDIRECT_PARAM.name: True}
 
     response = do_request()("GET", url, **redirect_kwargs)
     with vcr.use_cassette(yml):
@@ -180,14 +186,15 @@
     assert cassette_response.request.url == response.request.url
     assert cassette_response.request.method == response.request.method
     assert {k: v for k, v in cassette_response.request.headers.items()} == {
         k: v for k, v in response.request.headers.items()
     }
 
 
+@pytest.mark.online
 def test_work_with_gzipped_data(mockbin, do_request, yml):
     url = mockbin + "/gzip?foo=bar"
     headers = {"accept-encoding": "deflate, gzip"}
 
     with vcr.use_cassette(yml):
         do_request(headers=headers)("GET", url)
 
@@ -195,14 +202,15 @@
         cassette_response = do_request(headers=headers)("GET", url)
 
         assert cassette_response.headers["content-encoding"] == "gzip"
         assert cassette_response.read()
         assert cassette.play_count == 1
 
 
+@pytest.mark.online
 @pytest.mark.parametrize("url", ["https://github.com/kevin1024/vcrpy/issues/" + str(i) for i in range(3, 6)])
 def test_simple_fetching(do_request, yml, url):
     with vcr.use_cassette(yml):
         do_request()("GET", url)
 
     with vcr.use_cassette(yml) as cassette:
         cassette_response = do_request()("GET", url)
@@ -227,14 +235,15 @@
         assert str(cassette_response.request.url) == url
         assert cassette.play_count == 1
 
         assert cassette_response.headers["Via"] == "my_own_proxy", str(cassette_response.headers)
         assert cassette_response.request.url == response.request.url
 
 
+@pytest.mark.online
 def test_cookies(tmpdir, mockbin, do_request):
     def client_cookies(client):
         return [c for c in client.client.cookies]
 
     def response_cookies(response):
         return [c for c in response.cookies]
 
@@ -264,14 +273,15 @@
             cassette_response = new_client("GET", url)
 
             assert cassette.play_count == 1
             assert response_cookies(cassette_response) == ["k1", "k2"]
             assert client_cookies(new_client) == ["k1", "k2"]
 
 
+@pytest.mark.online
 def test_relative_redirects(tmpdir, scheme, do_request, mockbin):
     redirect_kwargs = {HTTPX_REDIRECT_PARAM.name: True}
 
     url = mockbin + "/redirect/301?to=/redirect/301?to=/request"
     testfile = str(tmpdir.join("relative_redirects.yml"))
     with vcr.use_cassette(testfile):
         response = do_request()("GET", url, **redirect_kwargs)
@@ -282,14 +292,15 @@
         response = do_request()("GET", url, **redirect_kwargs)
         assert len(response.history) == 2
         assert response.json()["url"].endswith("request")
 
         assert cassette.play_count == 3
 
 
+@pytest.mark.online
 def test_redirect_wo_allow_redirects(do_request, mockbin, yml):
     url = mockbin + "/redirect/308/5"
 
     redirect_kwargs = {HTTPX_REDIRECT_PARAM.name: False}
 
     with vcr.use_cassette(yml):
         response = do_request()("GET", url, **redirect_kwargs)
```

### Comparing `vcrpy-4.3.1/tests/integration/test_ignore.py` & `vcrpy-4.4.0/tests/integration/test_ignore.py`

 * *Files identical despite different names*

### Comparing `vcrpy-4.3.1/tests/integration/test_matchers.py` & `vcrpy-4.4.0/tests/integration/test_matchers.py`

 * *Files identical despite different names*

### Comparing `vcrpy-4.3.1/tests/integration/test_multiple.py` & `vcrpy-4.4.0/tests/integration/test_multiple.py`

 * *Files identical despite different names*

### Comparing `vcrpy-4.3.1/tests/integration/test_proxy.py` & `vcrpy-4.4.0/tests/integration/test_proxy.py`

 * *Files identical despite different names*

### Comparing `vcrpy-4.3.1/tests/integration/test_record_mode.py` & `vcrpy-4.4.0/tests/integration/test_record_mode.py`

 * *Files identical despite different names*

### Comparing `vcrpy-4.3.1/tests/integration/test_register_matcher.py` & `vcrpy-4.4.0/tests/integration/test_register_matcher.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,20 +1,23 @@
 from urllib.request import urlopen
 
+import pytest
+
 import vcr
 
 
 def true_matcher(r1, r2):
     return True
 
 
 def false_matcher(r1, r2):
     return False
 
 
+@pytest.mark.online
 def test_registered_true_matcher(tmpdir, mockbin_request_url):
     my_vcr = vcr.VCR()
     my_vcr.register_matcher("true", true_matcher)
     testfile = str(tmpdir.join("test.yml"))
     with my_vcr.use_cassette(testfile, match_on=["true"]):
         # These 2 different urls are stored as the same request
         urlopen(mockbin_request_url)
@@ -22,14 +25,15 @@
 
     with my_vcr.use_cassette(testfile, match_on=["true"]):
         # I can get the response twice even though I only asked for it once
         urlopen(mockbin_request_url)
         urlopen(mockbin_request_url)
 
 
+@pytest.mark.online
 def test_registered_false_matcher(tmpdir, mockbin_request_url):
     my_vcr = vcr.VCR()
     my_vcr.register_matcher("false", false_matcher)
     testfile = str(tmpdir.join("test.yml"))
     with my_vcr.use_cassette(testfile, match_on=["false"]) as cass:
         # These 2 different urls are stored as different requests
         urlopen(mockbin_request_url)
```

### Comparing `vcrpy-4.3.1/tests/integration/test_register_persister.py` & `vcrpy-4.4.0/tests/integration/test_register_persister.py`

 * *Files 1% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 from urllib.request import urlopen
 
 # Internal imports
 import vcr
 from vcr.persisters.filesystem import FilesystemPersister
 
 
-class CustomFilesystemPersister(object):
+class CustomFilesystemPersister:
     """Behaves just like default FilesystemPersister but adds .test extension
     to the cassette file"""
 
     @staticmethod
     def load_cassette(cassette_path, serializer):
         cassette_path += ".test"
         return FilesystemPersister.load_cassette(cassette_path, serializer)
```

### Comparing `vcrpy-4.3.1/tests/integration/test_register_serializer.py` & `vcrpy-4.4.0/tests/integration/test_register_serializer.py`

 * *Files identical despite different names*

### Comparing `vcrpy-4.3.1/tests/integration/test_request.py` & `vcrpy-4.4.0/tests/integration/test_request.py`

 * *Files identical despite different names*

### Comparing `vcrpy-4.3.1/tests/integration/test_requests.py` & `vcrpy-4.4.0/tests/integration/test_requests.py`

 * *Files 10% similar despite different names*

```diff
@@ -140,40 +140,71 @@
         assert content == requests.get(url).content
         # Ensure that we've now cached *two* responses. One for the redirect
         # and one for the final fetch
         assert len(cass) == 2
         assert cass.play_count == 2
 
 
+def test_raw_stream(tmpdir, httpbin):
+    expected_response = requests.get(httpbin.url, stream=True)
+    expected_content = b"".join(expected_response.raw.stream())
+
+    for _ in range(2):  # one for recording, one for cassette reply
+        with vcr.use_cassette(str(tmpdir.join("raw_stream.yaml"))):
+            actual_response = requests.get(httpbin.url, stream=True)
+            actual_content = b"".join(actual_response.raw.stream())
+        assert actual_content == expected_content
+
+
 def test_cross_scheme(tmpdir, httpbin_secure, httpbin):
     """Ensure that requests between schemes are treated separately"""
     # First fetch a url under http, and then again under https and then
     # ensure that we haven't served anything out of cache, and we have two
     # requests / response pairs in the cassette
     with vcr.use_cassette(str(tmpdir.join("cross_scheme.yaml"))) as cass:
         requests.get(httpbin_secure + "/")
         requests.get(httpbin + "/")
         assert cass.play_count == 0
         assert len(cass) == 2
 
 
-def test_gzip(tmpdir, httpbin_both):
+def test_gzip__decode_compressed_response_false(tmpdir, httpbin_both):
     """
     Ensure that requests (actually urllib3) is able to automatically decompress
     the response body
     """
-    url = httpbin_both + "/gzip"
-    response = requests.get(url)
+    for _ in range(2):  # one for recording, one for re-playing
+        with vcr.use_cassette(str(tmpdir.join("gzip.yaml"))):
+            response = requests.get(httpbin_both + "/gzip")
+            assert response.headers["content-encoding"] == "gzip"  # i.e. not removed
+            assert_is_json(response.content)  # i.e. uncompressed bytes
 
-    with vcr.use_cassette(str(tmpdir.join("gzip.yaml"))):
-        response = requests.get(url)
-        assert_is_json(response.content)
 
-    with vcr.use_cassette(str(tmpdir.join("gzip.yaml"))):
-        assert_is_json(response.content)
+def test_gzip__decode_compressed_response_true(tmpdir, httpbin_both):
+    url = httpbin_both + "/gzip"
+
+    expected_response = requests.get(url)
+    expected_content = expected_response.content
+    assert expected_response.headers["content-encoding"] == "gzip"  # self-test
+
+    with vcr.use_cassette(
+        str(tmpdir.join("decode_compressed.yaml")), decode_compressed_response=True
+    ) as cassette:
+        r = requests.get(url)
+        assert r.headers["content-encoding"] == "gzip"  # i.e. not removed
+        assert r.content == expected_content
+
+    # Has the cassette body been decompressed?
+    cassette_response_body = cassette.responses[0]["body"]["string"]
+    assert isinstance(cassette_response_body, str)
+
+    with vcr.use_cassette(str(tmpdir.join("decode_compressed.yaml")), decode_compressed_response=True):
+        r = requests.get(url)
+        assert "content-encoding" not in r.headers  # i.e. removed
+        assert r.content == expected_content
 
 
 def test_session_and_connection_close(tmpdir, httpbin):
     """
     This tests the issue in https://github.com/kevin1024/vcrpy/issues/48
 
     If you use a requests.session and the connection is closed, then an
```

### Comparing `vcrpy-4.3.1/tests/integration/test_stubs.py` & `vcrpy-4.4.0/tests/integration/test_stubs.py`

 * *Files identical despite different names*

### Comparing `vcrpy-4.3.1/tests/integration/test_tornado.py` & `vcrpy-4.4.0/tests/integration/test_tornado.py`

 * *Files identical despite different names*

### Comparing `vcrpy-4.3.1/tests/integration/test_tornado_exception_can_be_caught.yaml` & `vcrpy-4.4.0/tests/integration/test_tornado_exception_can_be_caught.yaml`

 * *Files identical despite different names*

### Comparing `vcrpy-4.3.1/tests/integration/test_tornado_with_decorator_use_cassette.yaml` & `vcrpy-4.4.0/tests/integration/test_tornado_with_decorator_use_cassette.yaml`

 * *Files identical despite different names*

### Comparing `vcrpy-4.3.1/tests/integration/test_urllib2.py` & `vcrpy-4.4.0/tests/integration/test_urllib2.py`

 * *Files 2% similar despite different names*

```diff
@@ -3,14 +3,15 @@
 
 import ssl
 from urllib.parse import urlencode
 from urllib.request import urlopen
 
 import pytest_httpbin.certs
 from assertions import assert_cassette_has_one_response
+from pytest import mark
 
 # Internal imports
 import vcr
 
 
 def urlopen_with_cafile(*args, **kwargs):
     context = ssl.create_default_context(cafile=pytest_httpbin.certs.where())
@@ -52,14 +53,15 @@
 
     with vcr.use_cassette(str(tmpdir.join("headers.yaml"))):
         open2 = urlopen_with_cafile(url).info().items()
 
         assert sorted(open1) == sorted(open2)
 
 
+@mark.online
 def test_effective_url(tmpdir):
     """Ensure that the effective_url is captured"""
     url = "http://mockbin.org/redirect/301"
 
     with vcr.use_cassette(str(tmpdir.join("headers.yaml"))):
         effective_url = urlopen_with_cafile(url).geturl()
         assert effective_url == "http://mockbin.org/redirect/301/0"
```

### Comparing `vcrpy-4.3.1/tests/integration/test_urllib3.py` & `vcrpy-4.4.0/tests/integration/test_urllib3.py`

 * *Files 1% similar despite different names*

```diff
@@ -93,14 +93,15 @@
 
     with vcr.use_cassette(str(tmpdir.join("verify_pool_mgr.yaml"))):
         req2 = verify_pool_mgr.request("POST", url, data).data
 
     assert req1 == req2
 
 
+@pytest.mark.online
 def test_redirects(tmpdir, verify_pool_mgr):
     """Ensure that we can handle redirects"""
     url = "http://mockbin.org/redirect/301"
 
     with vcr.use_cassette(str(tmpdir.join("verify_pool_mgr.yaml"))):
         content = verify_pool_mgr.request("GET", url).data
```

### Comparing `vcrpy-4.3.1/tests/integration/test_wild.py` & `vcrpy-4.4.0/tests/integration/test_wild.py`

 * *Files 6% similar despite different names*

```diff
@@ -48,14 +48,15 @@
 
     with vcr.use_cassette(testfile) as cass:
         assert len(cass) == 1
         _pretend_to_be_flickr_library()
         assert cass.play_count == 1
 
 
+@pytest.mark.online
 def test_flickr_should_respond_with_200(tmpdir):
     testfile = str(tmpdir.join("flickr.yml"))
     with vcr.use_cassette(testfile):
         r = requests.post("https://api.flickr.com/services/upload", verify=False)
         assert r.status_code == 200
 
 
@@ -66,14 +67,15 @@
         s.get(httpbin.url + "/cookies/set?k1=v1&k2=v2")
         assert s.cookies.keys() == ["k1", "k2"]
 
         r2 = s.get(httpbin.url + "/cookies")
         assert sorted(r2.json()["cookies"].keys()) == ["k1", "k2"]
 
 
+@pytest.mark.online
 def test_amazon_doctype(tmpdir):
     # amazon gzips its homepage.  For some reason, in requests 2.7, it's not
     # getting gunzipped.
     with vcr.use_cassette(str(tmpdir.join("amz.yml"))):
         r = requests.get("http://www.amazon.com", verify=False)
     assert "html" in r.text
```

### Comparing `vcrpy-4.3.1/tests/unit/test_cassettes.py` & `vcrpy-4.4.0/tests/unit/test_cassettes.py`

 * *Files identical despite different names*

### Comparing `vcrpy-4.3.1/tests/unit/test_errors.py` & `vcrpy-4.4.0/tests/unit/test_errors.py`

 * *Files identical despite different names*

### Comparing `vcrpy-4.3.1/tests/unit/test_filters.py` & `vcrpy-4.4.0/tests/unit/test_filters.py`

 * *Files 10% similar despite different names*

```diff
@@ -294,14 +294,26 @@
         "status": {"code": 200, "message": "OK"},
     }
     decoded_response = decode_response(deflate_response)
     assert decoded_response["body"]["string"] == body
     assert decoded_response["headers"]["content-length"] == [str(len(body))]
 
 
+def test_decode_response_deflate_already_decompressed():
+    body = b"deflate message"
+    gzip_response = {
+        "body": {"string": body},
+        "headers": {
+            "content-encoding": ["deflate"],
+        },
+    }
+    decoded_response = decode_response(gzip_response)
+    assert decoded_response["body"]["string"] == body
+
+
 def test_decode_response_gzip():
     body = b"gzip message"
 
     buf = BytesIO()
     f = gzip.GzipFile("a", fileobj=buf, mode="wb")
     f.write(body)
     f.close()
@@ -321,7 +333,19 @@
             "server": ["nginx"],
         },
         "status": {"code": 200, "message": "OK"},
     }
     decoded_response = decode_response(gzip_response)
     assert decoded_response["body"]["string"] == body
     assert decoded_response["headers"]["content-length"] == [str(len(body))]
+
+
+def test_decode_response_gzip_already_decompressed():
+    body = b"gzip message"
+    gzip_response = {
+        "body": {"string": body},
+        "headers": {
+            "content-encoding": ["gzip"],
+        },
+    }
+    decoded_response = decode_response(gzip_response)
+    assert decoded_response["body"]["string"] == body
```

### Comparing `vcrpy-4.3.1/tests/unit/test_json_serializer.py` & `vcrpy-4.4.0/tests/unit/test_json_serializer.py`

 * *Files identical despite different names*

### Comparing `vcrpy-4.3.1/tests/unit/test_matchers.py` & `vcrpy-4.4.0/tests/unit/test_matchers.py`

 * *Files identical despite different names*

### Comparing `vcrpy-4.3.1/tests/unit/test_migration.py` & `vcrpy-4.4.0/tests/unit/test_migration.py`

 * *Files identical despite different names*

### Comparing `vcrpy-4.3.1/tests/unit/test_persist.py` & `vcrpy-4.4.0/tests/unit/test_persist.py`

 * *Files identical despite different names*

### Comparing `vcrpy-4.3.1/tests/unit/test_request.py` & `vcrpy-4.4.0/tests/unit/test_request.py`

 * *Files identical despite different names*

### Comparing `vcrpy-4.3.1/tests/unit/test_response.py` & `vcrpy-4.4.0/tests/unit/test_response.py`

 * *Files 5% similar despite different names*

```diff
@@ -89,11 +89,11 @@
             b"different types of cancer cells. Recently, the first HDACi was\n      "
             b"approved for the "
             b"treatment of cutaneous T cell lymphomas. Most HDACi currently in\n      "
             b"clinical "
         },
     }
     vcr_response = VCRHTTPResponse(recorded_response)
-    handle = io.TextIOWrapper(io.BufferedReader(vcr_response), encoding="utf-8")
+    handle = io.TextIOWrapper(vcr_response, encoding="utf-8")
     handle = iter(handle)
     articles = [line for line in handle]
     assert len(articles) > 1
```

### Comparing `vcrpy-4.3.1/tests/unit/test_serialize.py` & `vcrpy-4.4.0/tests/unit/test_serialize.py`

 * *Files identical despite different names*

### Comparing `vcrpy-4.3.1/tests/unit/test_stubs.py` & `vcrpy-4.4.0/tests/unit/test_stubs.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,19 +1,22 @@
 from unittest import mock
 
+from pytest import mark
+
 from vcr import mode
 from vcr.cassette import Cassette
 from vcr.stubs import VCRHTTPSConnection
 
 
 class TestVCRConnection:
     def test_setting_of_attributes_get_propagated_to_real_connection(self):
         vcr_connection = VCRHTTPSConnection("www.examplehost.com")
         vcr_connection.ssl_version = "example_ssl_version"
         assert vcr_connection.real_connection.ssl_version == "example_ssl_version"
 
+    @mark.online
     @mock.patch("vcr.cassette.Cassette.can_play_response_for", return_value=False)
     def testing_connect(*args):
         vcr_connection = VCRHTTPSConnection("www.google.com")
         vcr_connection.cassette = Cassette("test", record_mode=mode.ALL)
         vcr_connection.real_connection.connect()
         assert vcr_connection.real_connection.sock is not None
```

### Comparing `vcrpy-4.3.1/tests/unit/test_vcr.py` & `vcrpy-4.4.0/tests/unit/test_vcr.py`

 * *Files identical despite different names*

### Comparing `vcrpy-4.3.1/tox.ini` & `vcrpy-4.4.0/tox.ini`

 * *Files identical despite different names*

### Comparing `vcrpy-4.3.1/vcr/cassette.py` & `vcrpy-4.4.0/vcr/cassette.py`

 * *Files identical despite different names*

### Comparing `vcrpy-4.3.1/vcr/config.py` & `vcrpy-4.4.0/vcr/config.py`

 * *Files 0% similar despite different names*

```diff
@@ -215,15 +215,15 @@
 
         if before_record_request:
             if not isinstance(before_record_request, collections_abc.Iterable):
                 before_record_request = (before_record_request,)
             filter_functions.extend(before_record_request)
 
         def before_record_request(request):
-            request = copy.copy(request)
+            request = copy.deepcopy(request)
             for function in filter_functions:
                 if request is None:
                     break
                 request = function(request)
             return request
 
         return before_record_request
```

### Comparing `vcrpy-4.3.1/vcr/errors.py` & `vcrpy-4.4.0/vcr/errors.py`

 * *Files identical despite different names*

### Comparing `vcrpy-4.3.1/vcr/filters.py` & `vcrpy-4.4.0/vcr/filters.py`

 * *Files 2% similar despite different names*

```diff
@@ -149,17 +149,23 @@
     def decompress_body(body, encoding):
         """Returns decompressed body according to encoding using zlib.
         to (de-)compress gzip format, use wbits = zlib.MAX_WBITS | 16
         """
         if not body:
             return ""
         if encoding == "gzip":
-            return zlib.decompress(body, zlib.MAX_WBITS | 16)
+            try:
+                return zlib.decompress(body, zlib.MAX_WBITS | 16)
+            except zlib.error:
+                return body  # assumes that the data was already decompressed
         else:  # encoding == 'deflate'
-            return zlib.decompress(body)
+            try:
+                return zlib.decompress(body)
+            except zlib.error:
+                return body  # assumes that the data was already decompressed
 
     # Deepcopy here in case `headers` contain objects that could
     # be mutated by a shallow copy and corrupt the real response.
     response = copy.deepcopy(response)
     headers = CaseInsensitiveDict(response["headers"])
     if is_compressed(headers):
         encoding = headers["content-encoding"][0]
```

### Comparing `vcrpy-4.3.1/vcr/matchers.py` & `vcrpy-4.4.0/vcr/matchers.py`

 * *Files 17% similar despite different names*

```diff
@@ -5,55 +5,65 @@
 
 from .util import read_body
 
 log = logging.getLogger(__name__)
 
 
 def method(r1, r2):
-    assert r1.method == r2.method, "{} != {}".format(r1.method, r2.method)
+    if r1.method != r2.method:
+        raise AssertionError("{} != {}".format(r1.method, r2.method))
 
 
 def uri(r1, r2):
-    assert r1.uri == r2.uri, "{} != {}".format(r1.uri, r2.uri)
+    if r1.uri != r2.uri:
+        raise AssertionError("{} != {}".format(r1.uri, r2.uri))
 
 
 def host(r1, r2):
-    assert r1.host == r2.host, "{} != {}".format(r1.host, r2.host)
+    if r1.host != r2.host:
+        raise AssertionError("{} != {}".format(r1.host, r2.host))
 
 
 def scheme(r1, r2):
-    assert r1.scheme == r2.scheme, "{} != {}".format(r1.scheme, r2.scheme)
+    if r1.scheme != r2.scheme:
+        raise AssertionError("{} != {}".format(r1.scheme, r2.scheme))
 
 
 def port(r1, r2):
-    assert r1.port == r2.port, "{} != {}".format(r1.port, r2.port)
+    if r1.port != r2.port:
+        raise AssertionError("{} != {}".format(r1.port, r2.port))
 
 
 def path(r1, r2):
-    assert r1.path == r2.path, "{} != {}".format(r1.path, r2.path)
+    if r1.path != r2.path:
+        raise AssertionError("{} != {}".format(r1.path, r2.path))
 
 
 def query(r1, r2):
-    assert r1.query == r2.query, "{} != {}".format(r1.query, r2.query)
+    if r1.query != r2.query:
+        raise AssertionError("{} != {}".format(r1.query, r2.query))
 
 
 def raw_body(r1, r2):
-    assert read_body(r1) == read_body(r2)
+    if read_body(r1) != read_body(r2):
+        raise AssertionError
 
 
 def body(r1, r2):
     transformer = _get_transformer(r1)
     r2_transformer = _get_transformer(r2)
     if transformer != r2_transformer:
         transformer = _identity
-    assert transformer(read_body(r1)) == transformer(read_body(r2))
+    if transformer(read_body(r1)) != transformer(read_body(r2)):
+        raise AssertionError
 
 
 def headers(r1, r2):
-    assert r1.headers == r2.headers, "{} != {}".format(r1.headers, r2.headers)
+    if r1.headers != r2.headers:
+        raise AssertionError("{} != {}".format(r1.headers, r2.headers))
 
 
 def _header_checker(value, header="Content-Type"):
     def checker(headers):
         _header = headers.get(header, "")
         if isinstance(_header, bytes):
             _header = _header.decode("utf-8")
```

### Comparing `vcrpy-4.3.1/vcr/migration.py` & `vcrpy-4.4.0/vcr/migration.py`

 * *Files 2% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 
 .. warning:: Backup your cassettes files before migration.
 
 It merges and deletes the request obsolete keys (protocol, host, port, path)
 into new 'uri' key.
 Usage::
 
-    python -m vcr.migration PATH
+    python3 -m vcr.migration PATH
 
 The PATH can be path to the directory with cassettes or cassette itself
 """
 
 import json
 import os
 import shutil
@@ -134,15 +134,15 @@
         return migrate(path, migrate_yml)
     return False
 
 
 def main():
     if len(sys.argv) != 2:
         raise SystemExit(
-            "Please provide path to cassettes directory or file. " "Usage: python -m vcr.migration PATH"
+            "Please provide path to cassettes directory or file. " "Usage: python3 -m vcr.migration PATH"
         )
 
     path = sys.argv[1]
     if not os.path.isabs(path):
         path = os.path.abspath(path)
     files = [path]
     if os.path.isdir(path):
```

### Comparing `vcrpy-4.3.1/vcr/patch.py` & `vcrpy-4.4.0/vcr/patch.py`

 * *Files identical despite different names*

### Comparing `vcrpy-4.3.1/vcr/persisters/filesystem.py` & `vcrpy-4.4.0/vcr/persisters/filesystem.py`

 * *Files identical despite different names*

### Comparing `vcrpy-4.3.1/vcr/record_mode.py` & `vcrpy-4.4.0/vcr/record_mode.py`

 * *Files identical despite different names*

### Comparing `vcrpy-4.3.1/vcr/request.py` & `vcrpy-4.4.0/vcr/request.py`

 * *Files identical despite different names*

### Comparing `vcrpy-4.3.1/vcr/serialize.py` & `vcrpy-4.4.0/vcr/serialize.py`

 * *Files identical despite different names*

### Comparing `vcrpy-4.3.1/vcr/serializers/compat.py` & `vcrpy-4.4.0/vcr/serializers/compat.py`

 * *Files identical despite different names*

### Comparing `vcrpy-4.3.1/vcr/serializers/jsonserializer.py` & `vcrpy-4.4.0/vcr/serializers/jsonserializer.py`

 * *Files identical despite different names*

### Comparing `vcrpy-4.3.1/vcr/stubs/__init__.py` & `vcrpy-4.4.0/vcr/stubs/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -89,14 +89,17 @@
         # twiddling self._closed and using this property to shadow the real
         # self.closed from the superclass
         return self._closed
 
     def read(self, *args, **kwargs):
         return self._content.read(*args, **kwargs)
 
+    def read1(self, *args, **kwargs):
+        return self._content.read1(*args, **kwargs)
+
     def readall(self):
         return self._content.readall()
 
     def readinto(self, *args, **kwargs):
         return self._content.readinto(*args, **kwargs)
 
     def readline(self, *args, **kwargs):
@@ -163,14 +166,21 @@
     @property
     def data(self):
         return self._content.getbuffer().tobytes()
 
     def drain_conn(self):
         pass
 
+    def stream(self, amt=65536, decode_content=None):
+        while True:
+            b = self._content.read(amt)
+            yield b
+            if not b:
+                break
+
 
 class VCRConnection:
     # A reference to the cassette that's currently being patched in
     cassette = None
 
     def _port_postfix(self):
         """
```

### Comparing `vcrpy-4.3.1/vcr/stubs/aiohttp_stubs.py` & `vcrpy-4.4.0/vcr/stubs/aiohttp_stubs.py`

 * *Files identical despite different names*

### Comparing `vcrpy-4.3.1/vcr/stubs/boto3_stubs.py` & `vcrpy-4.4.0/vcr/stubs/boto3_stubs.py`

 * *Files identical despite different names*

### Comparing `vcrpy-4.3.1/vcr/stubs/compat.py` & `vcrpy-4.4.0/vcr/stubs/compat.py`

 * *Files identical despite different names*

### Comparing `vcrpy-4.3.1/vcr/stubs/httplib2_stubs.py` & `vcrpy-4.4.0/vcr/stubs/httplib2_stubs.py`

 * *Files identical despite different names*

### Comparing `vcrpy-4.3.1/vcr/stubs/httpx_stubs.py` & `vcrpy-4.4.0/vcr/stubs/httpx_stubs.py`

 * *Files identical despite different names*

### Comparing `vcrpy-4.3.1/vcr/stubs/requests_stubs.py` & `vcrpy-4.4.0/vcr/stubs/requests_stubs.py`

 * *Files identical despite different names*

### Comparing `vcrpy-4.3.1/vcr/stubs/tornado_stubs.py` & `vcrpy-4.4.0/vcr/stubs/tornado_stubs.py`

 * *Files identical despite different names*

### Comparing `vcrpy-4.3.1/vcr/util.py` & `vcrpy-4.4.0/vcr/util.py`

 * *Files identical despite different names*

### Comparing `vcrpy-4.3.1/vcrpy.egg-info/PKG-INFO` & `vcrpy-4.4.0/vcrpy.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: vcrpy
-Version: 4.3.1
+Version: 4.4.0
 Summary: Automatically mock your HTTP interactions to simplify and speed up testing
 Home-page: https://github.com/kevin1024/vcrpy
 Author: Kevin McCarthy
 Author-email: me@kevinmccarthy.org
 License: MIT
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Environment :: Console
```

### Comparing `vcrpy-4.3.1/vcrpy.egg-info/SOURCES.txt` & `vcrpy-4.4.0/vcrpy.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -50,28 +50,30 @@
 tests/unit/test_matchers.py
 tests/unit/test_migration.py
 tests/unit/test_persist.py
 tests/unit/test_request.py
 tests/unit/test_response.py
 tests/unit/test_serialize.py
 tests/unit/test_stubs.py
+tests/unit/test_unittest.py
 tests/unit/test_vcr.py
 tests/unit/test_vcr_import.py
 vcr/__init__.py
 vcr/_handle_coroutine.py
 vcr/cassette.py
 vcr/config.py
 vcr/errors.py
 vcr/filters.py
 vcr/matchers.py
 vcr/migration.py
 vcr/patch.py
 vcr/record_mode.py
 vcr/request.py
 vcr/serialize.py
+vcr/unittest.py
 vcr/util.py
 vcr/persisters/__init__.py
 vcr/persisters/filesystem.py
 vcr/serializers/__init__.py
 vcr/serializers/compat.py
 vcr/serializers/jsonserializer.py
 vcr/serializers/yamlserializer.py
```

