# Comparing `tmp/vcrpy-4.4.0.tar.gz` & `tmp/vcrpy-5.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "vcrpy-4.4.0.tar", last modified: Mon Jun 26 14:20:09 2023, max compression
+gzip compressed data, was "vcrpy-5.0.0.tar", last modified: Mon Jun 26 21:26:54 2023, max compression
```

## Comparing `vcrpy-4.4.0.tar` & `vcrpy-5.0.0.tar`

### file list

```diff
@@ -1,108 +1,108 @@
-drwxr-xr-x   0 kevin     (1000) kevin     (1000)        0 2023-06-26 14:20:09.906139 vcrpy-4.4.0/
--rw-r--r--   0 kevin     (1000) kevin     (1000)     1063 2023-06-26 14:02:48.000000 vcrpy-4.4.0/LICENSE.txt
--rw-r--r--   0 kevin     (1000) kevin     (1000)      142 2023-06-26 14:02:48.000000 vcrpy-4.4.0/MANIFEST.in
--rw-r--r--   0 kevin     (1000) kevin     (1000)     3925 2023-06-26 14:20:09.906139 vcrpy-4.4.0/PKG-INFO
--rw-r--r--   0 kevin     (1000) kevin     (1000)     2767 2023-06-26 14:02:48.000000 vcrpy-4.4.0/README.rst
--rw-r--r--   0 kevin     (1000) kevin     (1000)      325 2023-06-26 14:02:48.000000 vcrpy-4.4.0/pyproject.toml
--rw-r--r--   0 kevin     (1000) kevin     (1000)       67 2023-06-26 14:20:09.906139 vcrpy-4.4.0/setup.cfg
--rw-r--r--   0 kevin     (1000) kevin     (1000)     3557 2023-06-26 14:02:48.000000 vcrpy-4.4.0/setup.py
-drwxr-xr-x   0 kevin     (1000) kevin     (1000)        0 2023-06-26 14:20:09.906139 vcrpy-4.4.0/tests/
--rw-r--r--   0 kevin     (1000) kevin     (1000)      354 2023-06-26 14:02:48.000000 vcrpy-4.4.0/tests/assertions.py
-drwxr-xr-x   0 kevin     (1000) kevin     (1000)        0 2023-06-26 14:20:09.906139 vcrpy-4.4.0/tests/fixtures/
-drwxr-xr-x   0 kevin     (1000) kevin     (1000)        0 2023-06-26 14:20:09.906139 vcrpy-4.4.0/tests/fixtures/migration/
--rw-r--r--   0 kevin     (1000) kevin     (1000)     1115 2023-06-26 14:02:48.000000 vcrpy-4.4.0/tests/fixtures/migration/new_cassette.json
--rw-r--r--   0 kevin     (1000) kevin     (1000)      599 2023-06-26 14:02:48.000000 vcrpy-4.4.0/tests/fixtures/migration/new_cassette.yaml
--rw-r--r--   0 kevin     (1000) kevin     (1000)       23 2023-06-26 14:02:48.000000 vcrpy-4.4.0/tests/fixtures/migration/not_cassette.txt
--rw-r--r--   0 kevin     (1000) kevin     (1000)     1031 2023-06-26 14:02:48.000000 vcrpy-4.4.0/tests/fixtures/migration/old_cassette.json
--rw-r--r--   0 kevin     (1000) kevin     (1000)      869 2023-06-26 14:02:48.000000 vcrpy-4.4.0/tests/fixtures/migration/old_cassette.yaml
-drwxr-xr-x   0 kevin     (1000) kevin     (1000)        0 2023-06-26 14:20:09.906139 vcrpy-4.4.0/tests/fixtures/wild/
--rw-r--r--   0 kevin     (1000) kevin     (1000)     9705 2023-06-26 14:02:48.000000 vcrpy-4.4.0/tests/fixtures/wild/domain_redirect.yaml
-drwxr-xr-x   0 kevin     (1000) kevin     (1000)        0 2023-06-26 14:20:09.906139 vcrpy-4.4.0/tests/integration/
--rw-r--r--   0 kevin     (1000) kevin     (1000)        0 2023-06-26 14:02:48.000000 vcrpy-4.4.0/tests/integration/__init__.py
--rw-r--r--   0 kevin     (1000) kevin     (1000)     1214 2023-06-26 14:02:48.000000 vcrpy-4.4.0/tests/integration/aiohttp_utils.py
-drwxr-xr-x   0 kevin     (1000) kevin     (1000)        0 2023-06-26 14:20:09.906139 vcrpy-4.4.0/tests/integration/cassettes/
--rw-r--r--   0 kevin     (1000) kevin     (1000)     1017 2023-06-26 14:02:48.000000 vcrpy-4.4.0/tests/integration/cassettes/test_httpx_test_test_behind_proxy.yml
--rw-r--r--   0 kevin     (1000) kevin     (1000)      781 2023-06-26 14:02:48.000000 vcrpy-4.4.0/tests/integration/conftest.py
--rw-r--r--   0 kevin     (1000) kevin     (1000)    16816 2023-06-26 14:02:48.000000 vcrpy-4.4.0/tests/integration/test_aiohttp.py
--rw-r--r--   0 kevin     (1000) kevin     (1000)     2766 2023-06-26 14:02:48.000000 vcrpy-4.4.0/tests/integration/test_basic.py
--rw-r--r--   0 kevin     (1000) kevin     (1000)     2951 2023-06-26 14:02:48.000000 vcrpy-4.4.0/tests/integration/test_boto.py
--rw-r--r--   0 kevin     (1000) kevin     (1000)     3589 2023-06-26 14:02:48.000000 vcrpy-4.4.0/tests/integration/test_boto3.py
--rw-r--r--   0 kevin     (1000) kevin     (1000)     2626 2023-06-26 14:02:48.000000 vcrpy-4.4.0/tests/integration/test_config.py
--rw-r--r--   0 kevin     (1000) kevin     (1000)     1618 2023-06-26 14:02:48.000000 vcrpy-4.4.0/tests/integration/test_disksaver.py
--rw-r--r--   0 kevin     (1000) kevin     (1000)     6402 2023-06-26 14:02:48.000000 vcrpy-4.4.0/tests/integration/test_filter.py
--rw-r--r--   0 kevin     (1000) kevin     (1000)     1030 2023-06-26 14:02:48.000000 vcrpy-4.4.0/tests/integration/test_http
--rw-r--r--   0 kevin     (1000) kevin     (1000)     4946 2023-06-26 14:02:48.000000 vcrpy-4.4.0/tests/integration/test_httplib2.py
--rw-r--r--   0 kevin     (1000) kevin     (1000)    10635 2023-06-26 14:02:48.000000 vcrpy-4.4.0/tests/integration/test_httpx.py
--rw-r--r--   0 kevin     (1000) kevin     (1000)     2621 2023-06-26 14:02:48.000000 vcrpy-4.4.0/tests/integration/test_ignore.py
--rw-r--r--   0 kevin     (1000) kevin     (1000)     4000 2023-06-26 14:02:48.000000 vcrpy-4.4.0/tests/integration/test_matchers.py
--rw-r--r--   0 kevin     (1000) kevin     (1000)      878 2023-06-26 14:02:48.000000 vcrpy-4.4.0/tests/integration/test_multiple.py
--rw-r--r--   0 kevin     (1000) kevin     (1000)     1779 2023-06-26 14:02:48.000000 vcrpy-4.4.0/tests/integration/test_proxy.py
--rw-r--r--   0 kevin     (1000) kevin     (1000)     5170 2023-06-26 14:02:48.000000 vcrpy-4.4.0/tests/integration/test_record_mode.py
--rw-r--r--   0 kevin     (1000) kevin     (1000)     1222 2023-06-26 14:02:48.000000 vcrpy-4.4.0/tests/integration/test_register_matcher.py
--rw-r--r--   0 kevin     (1000) kevin     (1000)     1844 2023-06-26 14:02:48.000000 vcrpy-4.4.0/tests/integration/test_register_persister.py
--rw-r--r--   0 kevin     (1000) kevin     (1000)      962 2023-06-26 14:02:48.000000 vcrpy-4.4.0/tests/integration/test_register_serializer.py
--rw-r--r--   0 kevin     (1000) kevin     (1000)      739 2023-06-26 14:02:48.000000 vcrpy-4.4.0/tests/integration/test_request.py
--rw-r--r--   0 kevin     (1000) kevin     (1000)    13174 2023-06-26 14:02:48.000000 vcrpy-4.4.0/tests/integration/test_requests.py
--rw-r--r--   0 kevin     (1000) kevin     (1000)     5040 2023-06-26 14:02:48.000000 vcrpy-4.4.0/tests/integration/test_stubs.py
--rw-r--r--   0 kevin     (1000) kevin     (1000)    12599 2023-06-26 14:02:48.000000 vcrpy-4.4.0/tests/integration/test_tornado.py
--rw-r--r--   0 kevin     (1000) kevin     (1000)     1387 2023-06-26 14:02:48.000000 vcrpy-4.4.0/tests/integration/test_tornado_exception_can_be_caught.yaml
--rw-r--r--   0 kevin     (1000) kevin     (1000)     1566 2023-06-26 14:02:48.000000 vcrpy-4.4.0/tests/integration/test_tornado_with_decorator_use_cassette.yaml
--rw-r--r--   0 kevin     (1000) kevin     (1000)     5109 2023-06-26 14:02:48.000000 vcrpy-4.4.0/tests/integration/test_urllib2.py
--rw-r--r--   0 kevin     (1000) kevin     (1000)     6384 2023-06-26 14:02:48.000000 vcrpy-4.4.0/tests/integration/test_urllib3.py
--rw-r--r--   0 kevin     (1000) kevin     (1000)     3538 2023-06-26 14:02:48.000000 vcrpy-4.4.0/tests/integration/test_wild.py
-drwxr-xr-x   0 kevin     (1000) kevin     (1000)        0 2023-06-26 14:20:09.906139 vcrpy-4.4.0/tests/unit/
--rw-r--r--   0 kevin     (1000) kevin     (1000)    13163 2023-06-26 14:02:48.000000 vcrpy-4.4.0/tests/unit/test_cassettes.py
--rw-r--r--   0 kevin     (1000) kevin     (1000)     2669 2023-06-26 14:02:48.000000 vcrpy-4.4.0/tests/unit/test_errors.py
--rw-r--r--   0 kevin     (1000) kevin     (1000)    12401 2023-06-26 14:02:48.000000 vcrpy-4.4.0/tests/unit/test_filters.py
--rw-r--r--   0 kevin     (1000) kevin     (1000)      611 2023-06-26 14:02:48.000000 vcrpy-4.4.0/tests/unit/test_json_serializer.py
--rw-r--r--   0 kevin     (1000) kevin     (1000)     9990 2023-06-26 14:02:48.000000 vcrpy-4.4.0/tests/unit/test_matchers.py
--rw-r--r--   0 kevin     (1000) kevin     (1000)     1588 2023-06-26 14:02:48.000000 vcrpy-4.4.0/tests/unit/test_migration.py
--rw-r--r--   0 kevin     (1000) kevin     (1000)     1067 2023-06-26 14:02:48.000000 vcrpy-4.4.0/tests/unit/test_persist.py
--rw-r--r--   0 kevin     (1000) kevin     (1000)     2471 2023-06-26 14:02:48.000000 vcrpy-4.4.0/tests/unit/test_request.py
--rw-r--r--   0 kevin     (1000) kevin     (1000)     3629 2023-06-26 14:02:48.000000 vcrpy-4.4.0/tests/unit/test_response.py
--rw-r--r--   0 kevin     (1000) kevin     (1000)     4038 2023-06-26 14:02:48.000000 vcrpy-4.4.0/tests/unit/test_serialize.py
--rw-r--r--   0 kevin     (1000) kevin     (1000)      840 2023-06-26 14:02:48.000000 vcrpy-4.4.0/tests/unit/test_stubs.py
--rw-r--r--   0 kevin     (1000) kevin     (1000)     5580 2023-06-26 14:02:48.000000 vcrpy-4.4.0/tests/unit/test_unittest.py
--rw-r--r--   0 kevin     (1000) kevin     (1000)    12082 2023-06-26 14:02:48.000000 vcrpy-4.4.0/tests/unit/test_vcr.py
--rw-r--r--   0 kevin     (1000) kevin     (1000)      395 2023-06-26 14:02:48.000000 vcrpy-4.4.0/tests/unit/test_vcr_import.py
--rw-r--r--   0 kevin     (1000) kevin     (1000)     3281 2023-06-26 14:02:48.000000 vcrpy-4.4.0/tox.ini
-drwxr-xr-x   0 kevin     (1000) kevin     (1000)        0 2023-06-26 14:20:09.906139 vcrpy-4.4.0/vcr/
--rw-r--r--   0 kevin     (1000) kevin     (1000)      296 2023-06-26 14:17:30.000000 vcrpy-4.4.0/vcr/__init__.py
--rw-r--r--   0 kevin     (1000) kevin     (1000)      125 2023-06-26 14:02:48.000000 vcrpy-4.4.0/vcr/_handle_coroutine.py
--rw-r--r--   0 kevin     (1000) kevin     (1000)    13892 2023-06-26 14:02:48.000000 vcrpy-4.4.0/vcr/cassette.py
--rw-r--r--   0 kevin     (1000) kevin     (1000)    10834 2023-06-26 14:02:48.000000 vcrpy-4.4.0/vcr/config.py
--rw-r--r--   0 kevin     (1000) kevin     (1000)     1976 2023-06-26 14:02:48.000000 vcrpy-4.4.0/vcr/errors.py
--rw-r--r--   0 kevin     (1000) kevin     (1000)     6911 2023-06-26 14:02:48.000000 vcrpy-4.4.0/vcr/filters.py
--rw-r--r--   0 kevin     (1000) kevin     (1000)     4365 2023-06-26 14:02:48.000000 vcrpy-4.4.0/vcr/matchers.py
--rw-r--r--   0 kevin     (1000) kevin     (1000)     4662 2023-06-26 14:02:48.000000 vcrpy-4.4.0/vcr/migration.py
--rw-r--r--   0 kevin     (1000) kevin     (1000)    17948 2023-06-26 14:02:48.000000 vcrpy-4.4.0/vcr/patch.py
-drwxr-xr-x   0 kevin     (1000) kevin     (1000)        0 2023-06-26 14:20:09.906139 vcrpy-4.4.0/vcr/persisters/
--rw-r--r--   0 kevin     (1000) kevin     (1000)        0 2023-06-26 14:02:48.000000 vcrpy-4.4.0/vcr/persisters/__init__.py
--rw-r--r--   0 kevin     (1000) kevin     (1000)     1095 2023-06-26 14:02:48.000000 vcrpy-4.4.0/vcr/persisters/filesystem.py
--rw-r--r--   0 kevin     (1000) kevin     (1000)      630 2023-06-26 14:02:48.000000 vcrpy-4.4.0/vcr/record_mode.py
--rw-r--r--   0 kevin     (1000) kevin     (1000)     3782 2023-06-26 14:02:48.000000 vcrpy-4.4.0/vcr/request.py
--rw-r--r--   0 kevin     (1000) kevin     (1000)     2124 2023-06-26 14:02:48.000000 vcrpy-4.4.0/vcr/serialize.py
-drwxr-xr-x   0 kevin     (1000) kevin     (1000)        0 2023-06-26 14:20:09.906139 vcrpy-4.4.0/vcr/serializers/
--rw-r--r--   0 kevin     (1000) kevin     (1000)        0 2023-06-26 14:02:48.000000 vcrpy-4.4.0/vcr/serializers/__init__.py
--rw-r--r--   0 kevin     (1000) kevin     (1000)     2513 2023-06-26 14:02:48.000000 vcrpy-4.4.0/vcr/serializers/compat.py
--rw-r--r--   0 kevin     (1000) kevin     (1000)      778 2023-06-26 14:02:48.000000 vcrpy-4.4.0/vcr/serializers/jsonserializer.py
--rw-r--r--   0 kevin     (1000) kevin     (1000)      363 2023-06-26 14:02:48.000000 vcrpy-4.4.0/vcr/serializers/yamlserializer.py
-drwxr-xr-x   0 kevin     (1000) kevin     (1000)        0 2023-06-26 14:20:09.906139 vcrpy-4.4.0/vcr/stubs/
--rw-r--r--   0 kevin     (1000) kevin     (1000)    13682 2023-06-26 14:02:48.000000 vcrpy-4.4.0/vcr/stubs/__init__.py
--rw-r--r--   0 kevin     (1000) kevin     (1000)     9954 2023-06-26 14:02:48.000000 vcrpy-4.4.0/vcr/stubs/aiohttp_stubs.py
--rw-r--r--   0 kevin     (1000) kevin     (1000)     1202 2023-06-26 14:02:48.000000 vcrpy-4.4.0/vcr/stubs/boto3_stubs.py
--rw-r--r--   0 kevin     (1000) kevin     (1000)      235 2023-06-26 14:02:48.000000 vcrpy-4.4.0/vcr/stubs/boto_stubs.py
--rw-r--r--   0 kevin     (1000) kevin     (1000)      578 2023-06-26 14:02:48.000000 vcrpy-4.4.0/vcr/stubs/compat.py
--rw-r--r--   0 kevin     (1000) kevin     (1000)     2166 2023-06-26 14:02:48.000000 vcrpy-4.4.0/vcr/stubs/httplib2_stubs.py
--rw-r--r--   0 kevin     (1000) kevin     (1000)     5579 2023-06-26 14:02:48.000000 vcrpy-4.4.0/vcr/stubs/httpx_stubs.py
--rw-r--r--   0 kevin     (1000) kevin     (1000)      558 2023-06-26 14:02:48.000000 vcrpy-4.4.0/vcr/stubs/requests_stubs.py
--rw-r--r--   0 kevin     (1000) kevin     (1000)     3407 2023-06-26 14:02:48.000000 vcrpy-4.4.0/vcr/stubs/tornado_stubs.py
--rw-r--r--   0 kevin     (1000) kevin     (1000)      504 2023-06-26 14:02:48.000000 vcrpy-4.4.0/vcr/stubs/urllib3_stubs.py
--rw-r--r--   0 kevin     (1000) kevin     (1000)     1086 2023-06-26 14:02:48.000000 vcrpy-4.4.0/vcr/unittest.py
--rw-r--r--   0 kevin     (1000) kevin     (1000)     3882 2023-06-26 14:02:48.000000 vcrpy-4.4.0/vcr/util.py
-drwxr-xr-x   0 kevin     (1000) kevin     (1000)        0 2023-06-26 14:20:09.906139 vcrpy-4.4.0/vcrpy.egg-info/
--rw-r--r--   0 kevin     (1000) kevin     (1000)     3925 2023-06-26 14:20:09.000000 vcrpy-4.4.0/vcrpy.egg-info/PKG-INFO
--rw-r--r--   0 kevin     (1000) kevin     (1000)     2694 2023-06-26 14:20:09.000000 vcrpy-4.4.0/vcrpy.egg-info/SOURCES.txt
--rw-r--r--   0 kevin     (1000) kevin     (1000)        1 2023-06-26 14:20:09.000000 vcrpy-4.4.0/vcrpy.egg-info/dependency_links.txt
--rw-r--r--   0 kevin     (1000) kevin     (1000)       65 2023-06-26 14:20:09.000000 vcrpy-4.4.0/vcrpy.egg-info/requires.txt
--rw-r--r--   0 kevin     (1000) kevin     (1000)        4 2023-06-26 14:20:09.000000 vcrpy-4.4.0/vcrpy.egg-info/top_level.txt
+drwxr-xr-x   0 kevin     (1000) kevin     (1000)        0 2023-06-26 21:26:54.761739 vcrpy-5.0.0/
+-rw-r--r--   0 kevin     (1000) kevin     (1000)     1063 2023-06-26 14:02:48.000000 vcrpy-5.0.0/LICENSE.txt
+-rw-r--r--   0 kevin     (1000) kevin     (1000)      142 2023-06-26 14:02:48.000000 vcrpy-5.0.0/MANIFEST.in
+-rw-r--r--   0 kevin     (1000) kevin     (1000)     3875 2023-06-26 21:26:54.761739 vcrpy-5.0.0/PKG-INFO
+-rw-r--r--   0 kevin     (1000) kevin     (1000)     2767 2023-06-26 14:02:48.000000 vcrpy-5.0.0/README.rst
+-rw-r--r--   0 kevin     (1000) kevin     (1000)      325 2023-06-26 14:02:48.000000 vcrpy-5.0.0/pyproject.toml
+-rw-r--r--   0 kevin     (1000) kevin     (1000)       67 2023-06-26 21:26:54.761739 vcrpy-5.0.0/setup.cfg
+-rw-r--r--   0 kevin     (1000) kevin     (1000)     3503 2023-06-26 17:41:10.000000 vcrpy-5.0.0/setup.py
+drwxr-xr-x   0 kevin     (1000) kevin     (1000)        0 2023-06-26 21:26:54.761739 vcrpy-5.0.0/tests/
+-rw-r--r--   0 kevin     (1000) kevin     (1000)      385 2023-06-26 17:41:10.000000 vcrpy-5.0.0/tests/assertions.py
+drwxr-xr-x   0 kevin     (1000) kevin     (1000)        0 2023-06-26 21:26:54.761739 vcrpy-5.0.0/tests/fixtures/
+drwxr-xr-x   0 kevin     (1000) kevin     (1000)        0 2023-06-26 21:26:54.761739 vcrpy-5.0.0/tests/fixtures/migration/
+-rw-r--r--   0 kevin     (1000) kevin     (1000)     1115 2023-06-26 14:02:48.000000 vcrpy-5.0.0/tests/fixtures/migration/new_cassette.json
+-rw-r--r--   0 kevin     (1000) kevin     (1000)      599 2023-06-26 14:02:48.000000 vcrpy-5.0.0/tests/fixtures/migration/new_cassette.yaml
+-rw-r--r--   0 kevin     (1000) kevin     (1000)       23 2023-06-26 14:02:48.000000 vcrpy-5.0.0/tests/fixtures/migration/not_cassette.txt
+-rw-r--r--   0 kevin     (1000) kevin     (1000)     1031 2023-06-26 14:02:48.000000 vcrpy-5.0.0/tests/fixtures/migration/old_cassette.json
+-rw-r--r--   0 kevin     (1000) kevin     (1000)      869 2023-06-26 14:02:48.000000 vcrpy-5.0.0/tests/fixtures/migration/old_cassette.yaml
+drwxr-xr-x   0 kevin     (1000) kevin     (1000)        0 2023-06-26 21:26:54.761739 vcrpy-5.0.0/tests/fixtures/wild/
+-rw-r--r--   0 kevin     (1000) kevin     (1000)     9705 2023-06-26 14:02:48.000000 vcrpy-5.0.0/tests/fixtures/wild/domain_redirect.yaml
+drwxr-xr-x   0 kevin     (1000) kevin     (1000)        0 2023-06-26 21:26:54.761739 vcrpy-5.0.0/tests/integration/
+-rw-r--r--   0 kevin     (1000) kevin     (1000)        0 2023-06-26 14:02:48.000000 vcrpy-5.0.0/tests/integration/__init__.py
+-rw-r--r--   0 kevin     (1000) kevin     (1000)     1214 2023-06-26 14:02:48.000000 vcrpy-5.0.0/tests/integration/aiohttp_utils.py
+drwxr-xr-x   0 kevin     (1000) kevin     (1000)        0 2023-06-26 21:26:54.761739 vcrpy-5.0.0/tests/integration/cassettes/
+-rw-r--r--   0 kevin     (1000) kevin     (1000)     1017 2023-06-26 14:02:48.000000 vcrpy-5.0.0/tests/integration/cassettes/test_httpx_test_test_behind_proxy.yml
+-rw-r--r--   0 kevin     (1000) kevin     (1000)      781 2023-06-26 14:02:48.000000 vcrpy-5.0.0/tests/integration/conftest.py
+-rw-r--r--   0 kevin     (1000) kevin     (1000)    16808 2023-06-26 17:41:10.000000 vcrpy-5.0.0/tests/integration/test_aiohttp.py
+-rw-r--r--   0 kevin     (1000) kevin     (1000)     2742 2023-06-26 17:41:10.000000 vcrpy-5.0.0/tests/integration/test_basic.py
+-rw-r--r--   0 kevin     (1000) kevin     (1000)     2951 2023-06-26 14:02:48.000000 vcrpy-5.0.0/tests/integration/test_boto.py
+-rw-r--r--   0 kevin     (1000) kevin     (1000)     3559 2023-06-26 17:41:10.000000 vcrpy-5.0.0/tests/integration/test_boto3.py
+-rw-r--r--   0 kevin     (1000) kevin     (1000)     2626 2023-06-26 14:02:48.000000 vcrpy-5.0.0/tests/integration/test_config.py
+-rw-r--r--   0 kevin     (1000) kevin     (1000)     1594 2023-06-26 17:41:10.000000 vcrpy-5.0.0/tests/integration/test_disksaver.py
+-rw-r--r--   0 kevin     (1000) kevin     (1000)     6426 2023-06-26 17:41:10.000000 vcrpy-5.0.0/tests/integration/test_filter.py
+-rw-r--r--   0 kevin     (1000) kevin     (1000)     1030 2023-06-26 14:02:48.000000 vcrpy-5.0.0/tests/integration/test_http
+-rw-r--r--   0 kevin     (1000) kevin     (1000)     4922 2023-06-26 17:41:10.000000 vcrpy-5.0.0/tests/integration/test_httplib2.py
+-rw-r--r--   0 kevin     (1000) kevin     (1000)    10635 2023-06-26 14:02:48.000000 vcrpy-5.0.0/tests/integration/test_httpx.py
+-rw-r--r--   0 kevin     (1000) kevin     (1000)     2541 2023-06-26 17:41:10.000000 vcrpy-5.0.0/tests/integration/test_ignore.py
+-rw-r--r--   0 kevin     (1000) kevin     (1000)     4000 2023-06-26 14:02:48.000000 vcrpy-5.0.0/tests/integration/test_matchers.py
+-rw-r--r--   0 kevin     (1000) kevin     (1000)      878 2023-06-26 14:02:48.000000 vcrpy-5.0.0/tests/integration/test_multiple.py
+-rw-r--r--   0 kevin     (1000) kevin     (1000)     1755 2023-06-26 17:41:10.000000 vcrpy-5.0.0/tests/integration/test_proxy.py
+-rw-r--r--   0 kevin     (1000) kevin     (1000)     5170 2023-06-26 14:02:48.000000 vcrpy-5.0.0/tests/integration/test_record_mode.py
+-rw-r--r--   0 kevin     (1000) kevin     (1000)     1222 2023-06-26 14:02:48.000000 vcrpy-5.0.0/tests/integration/test_register_matcher.py
+-rw-r--r--   0 kevin     (1000) kevin     (1000)     2825 2023-06-26 17:41:10.000000 vcrpy-5.0.0/tests/integration/test_register_persister.py
+-rw-r--r--   0 kevin     (1000) kevin     (1000)      962 2023-06-26 14:02:48.000000 vcrpy-5.0.0/tests/integration/test_register_serializer.py
+-rw-r--r--   0 kevin     (1000) kevin     (1000)      739 2023-06-26 14:02:48.000000 vcrpy-5.0.0/tests/integration/test_request.py
+-rw-r--r--   0 kevin     (1000) kevin     (1000)    12531 2023-06-26 17:41:10.000000 vcrpy-5.0.0/tests/integration/test_requests.py
+-rw-r--r--   0 kevin     (1000) kevin     (1000)     5052 2023-06-26 17:41:10.000000 vcrpy-5.0.0/tests/integration/test_stubs.py
+-rw-r--r--   0 kevin     (1000) kevin     (1000)    12593 2023-06-26 17:41:10.000000 vcrpy-5.0.0/tests/integration/test_tornado.py
+-rw-r--r--   0 kevin     (1000) kevin     (1000)     1387 2023-06-26 14:02:48.000000 vcrpy-5.0.0/tests/integration/test_tornado_exception_can_be_caught.yaml
+-rw-r--r--   0 kevin     (1000) kevin     (1000)     1566 2023-06-26 14:02:48.000000 vcrpy-5.0.0/tests/integration/test_tornado_with_decorator_use_cassette.yaml
+-rw-r--r--   0 kevin     (1000) kevin     (1000)     5085 2023-06-26 17:41:10.000000 vcrpy-5.0.0/tests/integration/test_urllib2.py
+-rw-r--r--   0 kevin     (1000) kevin     (1000)     6402 2023-06-26 17:41:10.000000 vcrpy-5.0.0/tests/integration/test_urllib3.py
+-rw-r--r--   0 kevin     (1000) kevin     (1000)     3538 2023-06-26 14:02:48.000000 vcrpy-5.0.0/tests/integration/test_wild.py
+drwxr-xr-x   0 kevin     (1000) kevin     (1000)        0 2023-06-26 21:26:54.761739 vcrpy-5.0.0/tests/unit/
+-rw-r--r--   0 kevin     (1000) kevin     (1000)    13542 2023-06-26 17:41:10.000000 vcrpy-5.0.0/tests/unit/test_cassettes.py
+-rw-r--r--   0 kevin     (1000) kevin     (1000)     2669 2023-06-26 14:02:48.000000 vcrpy-5.0.0/tests/unit/test_errors.py
+-rw-r--r--   0 kevin     (1000) kevin     (1000)    12401 2023-06-26 14:02:48.000000 vcrpy-5.0.0/tests/unit/test_filters.py
+-rw-r--r--   0 kevin     (1000) kevin     (1000)      611 2023-06-26 14:02:48.000000 vcrpy-5.0.0/tests/unit/test_json_serializer.py
+-rw-r--r--   0 kevin     (1000) kevin     (1000)     9990 2023-06-26 14:02:48.000000 vcrpy-5.0.0/tests/unit/test_matchers.py
+-rw-r--r--   0 kevin     (1000) kevin     (1000)     1568 2023-06-26 17:41:10.000000 vcrpy-5.0.0/tests/unit/test_migration.py
+-rw-r--r--   0 kevin     (1000) kevin     (1000)     1067 2023-06-26 14:02:48.000000 vcrpy-5.0.0/tests/unit/test_persist.py
+-rw-r--r--   0 kevin     (1000) kevin     (1000)     2471 2023-06-26 14:02:48.000000 vcrpy-5.0.0/tests/unit/test_request.py
+-rw-r--r--   0 kevin     (1000) kevin     (1000)     3613 2023-06-26 17:41:10.000000 vcrpy-5.0.0/tests/unit/test_response.py
+-rw-r--r--   0 kevin     (1000) kevin     (1000)     3992 2023-06-26 17:41:10.000000 vcrpy-5.0.0/tests/unit/test_serialize.py
+-rw-r--r--   0 kevin     (1000) kevin     (1000)      840 2023-06-26 14:02:48.000000 vcrpy-5.0.0/tests/unit/test_stubs.py
+-rw-r--r--   0 kevin     (1000) kevin     (1000)     5580 2023-06-26 14:02:48.000000 vcrpy-5.0.0/tests/unit/test_unittest.py
+-rw-r--r--   0 kevin     (1000) kevin     (1000)    12082 2023-06-26 14:02:48.000000 vcrpy-5.0.0/tests/unit/test_vcr.py
+-rw-r--r--   0 kevin     (1000) kevin     (1000)      395 2023-06-26 14:02:48.000000 vcrpy-5.0.0/tests/unit/test_vcr_import.py
+-rw-r--r--   0 kevin     (1000) kevin     (1000)     3115 2023-06-26 17:41:10.000000 vcrpy-5.0.0/tox.ini
+drwxr-xr-x   0 kevin     (1000) kevin     (1000)        0 2023-06-26 21:26:54.761739 vcrpy-5.0.0/vcr/
+-rw-r--r--   0 kevin     (1000) kevin     (1000)      296 2023-06-26 17:44:58.000000 vcrpy-5.0.0/vcr/__init__.py
+-rw-r--r--   0 kevin     (1000) kevin     (1000)      125 2023-06-26 14:02:48.000000 vcrpy-5.0.0/vcr/_handle_coroutine.py
+-rw-r--r--   0 kevin     (1000) kevin     (1000)    13958 2023-06-26 17:41:10.000000 vcrpy-5.0.0/vcr/cassette.py
+-rw-r--r--   0 kevin     (1000) kevin     (1000)    10818 2023-06-26 17:41:10.000000 vcrpy-5.0.0/vcr/config.py
+-rw-r--r--   0 kevin     (1000) kevin     (1000)     1976 2023-06-26 14:02:48.000000 vcrpy-5.0.0/vcr/errors.py
+-rw-r--r--   0 kevin     (1000) kevin     (1000)     6911 2023-06-26 14:02:48.000000 vcrpy-5.0.0/vcr/filters.py
+-rw-r--r--   0 kevin     (1000) kevin     (1000)     4267 2023-06-26 17:41:10.000000 vcrpy-5.0.0/vcr/matchers.py
+-rw-r--r--   0 kevin     (1000) kevin     (1000)     4639 2023-06-26 17:41:10.000000 vcrpy-5.0.0/vcr/migration.py
+-rw-r--r--   0 kevin     (1000) kevin     (1000)    17916 2023-06-26 17:41:10.000000 vcrpy-5.0.0/vcr/patch.py
+drwxr-xr-x   0 kevin     (1000) kevin     (1000)        0 2023-06-26 21:26:54.761739 vcrpy-5.0.0/vcr/persisters/
+-rw-r--r--   0 kevin     (1000) kevin     (1000)        0 2023-06-26 14:02:48.000000 vcrpy-5.0.0/vcr/persisters/__init__.py
+-rw-r--r--   0 kevin     (1000) kevin     (1000)     1203 2023-06-26 17:41:10.000000 vcrpy-5.0.0/vcr/persisters/filesystem.py
+-rw-r--r--   0 kevin     (1000) kevin     (1000)      630 2023-06-26 14:02:48.000000 vcrpy-5.0.0/vcr/record_mode.py
+-rw-r--r--   0 kevin     (1000) kevin     (1000)     3772 2023-06-26 17:41:10.000000 vcrpy-5.0.0/vcr/request.py
+-rw-r--r--   0 kevin     (1000) kevin     (1000)     2124 2023-06-26 14:02:48.000000 vcrpy-5.0.0/vcr/serialize.py
+drwxr-xr-x   0 kevin     (1000) kevin     (1000)        0 2023-06-26 21:26:54.761739 vcrpy-5.0.0/vcr/serializers/
+-rw-r--r--   0 kevin     (1000) kevin     (1000)        0 2023-06-26 14:02:48.000000 vcrpy-5.0.0/vcr/serializers/__init__.py
+-rw-r--r--   0 kevin     (1000) kevin     (1000)     2513 2023-06-26 14:02:48.000000 vcrpy-5.0.0/vcr/serializers/compat.py
+-rw-r--r--   0 kevin     (1000) kevin     (1000)      778 2023-06-26 14:02:48.000000 vcrpy-5.0.0/vcr/serializers/jsonserializer.py
+-rw-r--r--   0 kevin     (1000) kevin     (1000)      363 2023-06-26 14:02:48.000000 vcrpy-5.0.0/vcr/serializers/yamlserializer.py
+drwxr-xr-x   0 kevin     (1000) kevin     (1000)        0 2023-06-26 21:26:54.761739 vcrpy-5.0.0/vcr/stubs/
+-rw-r--r--   0 kevin     (1000) kevin     (1000)    13616 2023-06-26 17:41:10.000000 vcrpy-5.0.0/vcr/stubs/__init__.py
+-rw-r--r--   0 kevin     (1000) kevin     (1000)     9946 2023-06-26 17:41:10.000000 vcrpy-5.0.0/vcr/stubs/aiohttp_stubs.py
+-rw-r--r--   0 kevin     (1000) kevin     (1000)     1202 2023-06-26 14:02:48.000000 vcrpy-5.0.0/vcr/stubs/boto3_stubs.py
+-rw-r--r--   0 kevin     (1000) kevin     (1000)      235 2023-06-26 14:02:48.000000 vcrpy-5.0.0/vcr/stubs/boto_stubs.py
+-rw-r--r--   0 kevin     (1000) kevin     (1000)      578 2023-06-26 14:02:48.000000 vcrpy-5.0.0/vcr/stubs/compat.py
+-rw-r--r--   0 kevin     (1000) kevin     (1000)     2166 2023-06-26 14:02:48.000000 vcrpy-5.0.0/vcr/stubs/httplib2_stubs.py
+-rw-r--r--   0 kevin     (1000) kevin     (1000)     5579 2023-06-26 14:02:48.000000 vcrpy-5.0.0/vcr/stubs/httpx_stubs.py
+-rw-r--r--   0 kevin     (1000) kevin     (1000)      558 2023-06-26 14:02:48.000000 vcrpy-5.0.0/vcr/stubs/requests_stubs.py
+-rw-r--r--   0 kevin     (1000) kevin     (1000)     3407 2023-06-26 14:02:48.000000 vcrpy-5.0.0/vcr/stubs/tornado_stubs.py
+-rw-r--r--   0 kevin     (1000) kevin     (1000)      504 2023-06-26 14:02:48.000000 vcrpy-5.0.0/vcr/stubs/urllib3_stubs.py
+-rw-r--r--   0 kevin     (1000) kevin     (1000)     1074 2023-06-26 17:41:10.000000 vcrpy-5.0.0/vcr/unittest.py
+-rw-r--r--   0 kevin     (1000) kevin     (1000)     3800 2023-06-26 17:41:10.000000 vcrpy-5.0.0/vcr/util.py
+drwxr-xr-x   0 kevin     (1000) kevin     (1000)        0 2023-06-26 21:26:54.761739 vcrpy-5.0.0/vcrpy.egg-info/
+-rw-r--r--   0 kevin     (1000) kevin     (1000)     3875 2023-06-26 21:26:54.000000 vcrpy-5.0.0/vcrpy.egg-info/PKG-INFO
+-rw-r--r--   0 kevin     (1000) kevin     (1000)     2694 2023-06-26 21:26:54.000000 vcrpy-5.0.0/vcrpy.egg-info/SOURCES.txt
+-rw-r--r--   0 kevin     (1000) kevin     (1000)        1 2023-06-26 21:26:54.000000 vcrpy-5.0.0/vcrpy.egg-info/dependency_links.txt
+-rw-r--r--   0 kevin     (1000) kevin     (1000)       65 2023-06-26 21:26:54.000000 vcrpy-5.0.0/vcrpy.egg-info/requires.txt
+-rw-r--r--   0 kevin     (1000) kevin     (1000)        4 2023-06-26 21:26:54.000000 vcrpy-5.0.0/vcrpy.egg-info/top_level.txt
```

### Comparing `vcrpy-4.4.0/LICENSE.txt` & `vcrpy-5.0.0/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `vcrpy-4.4.0/PKG-INFO` & `vcrpy-5.0.0/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,32 +1,31 @@
 Metadata-Version: 2.1
 Name: vcrpy
-Version: 4.4.0
+Version: 5.0.0
 Summary: Automatically mock your HTTP interactions to simplify and speed up testing
 Home-page: https://github.com/kevin1024/vcrpy
 Author: Kevin McCarthy
 Author-email: me@kevinmccarthy.org
 License: MIT
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Environment :: Console
 Classifier: Intended Audience :: Developers
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3 :: Only
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Classifier: Programming Language :: Python :: Implementation :: PyPy
 Classifier: Topic :: Software Development :: Testing
 Classifier: Topic :: Internet :: WWW/HTTP
 Classifier: License :: OSI Approved :: MIT License
-Requires-Python: >=3.7
+Requires-Python: >=3.8
 Description-Content-Type: text/x-rst
 License-File: LICENSE.txt
 
 
 ###########
 VCR.py 📼
 ###########
```

### Comparing `vcrpy-4.4.0/README.rst` & `vcrpy-5.0.0/README.rst`

 * *Files identical despite different names*

### Comparing `vcrpy-4.4.0/setup.py` & `vcrpy-5.0.0/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 import os
 import re
 import sys
 
 from setuptools import find_packages, setup
 from setuptools.command.test import test as TestCommand
 
-long_description = open("README.rst", "r").read()
+long_description = open("README.rst").read()
 here = os.path.abspath(os.path.dirname(__file__))
 
 
 def read(*parts):
     # intentionally *not* adding an encoding option to open, See:
     #   https://github.com/pypa/virtualenv/issues/201#issuecomment-3145690
     with codecs.open(os.path.join(here, *parts), "r") as fp:
@@ -81,25 +81,24 @@
     description=("Automatically mock your HTTP interactions to simplify and speed up testing"),
     long_description=long_description,
     long_description_content_type="text/x-rst",
     author="Kevin McCarthy",
     author_email="me@kevinmccarthy.org",
     url="https://github.com/kevin1024/vcrpy",
     packages=find_packages(exclude=["tests*"]),
-    python_requires=">=3.7",
+    python_requires=">=3.8",
     install_requires=install_requires,
     license="MIT",
     tests_require=tests_require,
     classifiers=[
         "Development Status :: 5 - Production/Stable",
         "Environment :: Console",
         "Intended Audience :: Developers",
         "Programming Language :: Python",
         "Programming Language :: Python :: 3",
-        "Programming Language :: Python :: 3.7",
         "Programming Language :: Python :: 3.8",
         "Programming Language :: Python :: 3.9",
         "Programming Language :: Python :: 3.10",
         "Programming Language :: Python :: 3.11",
         "Programming Language :: Python :: 3 :: Only",
         "Programming Language :: Python :: Implementation :: CPython",
         "Programming Language :: Python :: Implementation :: PyPy",
```

### Comparing `vcrpy-4.4.0/tests/fixtures/migration/new_cassette.json` & `vcrpy-5.0.0/tests/fixtures/migration/new_cassette.json`

 * *Files identical despite different names*

### Comparing `vcrpy-4.4.0/tests/fixtures/migration/new_cassette.yaml` & `vcrpy-5.0.0/tests/fixtures/migration/new_cassette.yaml`

 * *Files identical despite different names*

### Comparing `vcrpy-4.4.0/tests/fixtures/migration/old_cassette.json` & `vcrpy-5.0.0/tests/fixtures/migration/old_cassette.json`

 * *Files identical despite different names*

### Comparing `vcrpy-4.4.0/tests/fixtures/migration/old_cassette.yaml` & `vcrpy-5.0.0/tests/fixtures/migration/old_cassette.yaml`

 * *Files identical despite different names*

### Comparing `vcrpy-4.4.0/tests/fixtures/wild/domain_redirect.yaml` & `vcrpy-5.0.0/tests/fixtures/wild/domain_redirect.yaml`

 * *Files identical despite different names*

### Comparing `vcrpy-4.4.0/tests/integration/aiohttp_utils.py` & `vcrpy-5.0.0/tests/integration/aiohttp_utils.py`

 * *Files identical despite different names*

### Comparing `vcrpy-4.4.0/tests/integration/cassettes/test_httpx_test_test_behind_proxy.yml` & `vcrpy-5.0.0/tests/integration/cassettes/test_httpx_test_test_behind_proxy.yml`

 * *Files identical despite different names*

### Comparing `vcrpy-4.4.0/tests/integration/conftest.py` & `vcrpy-5.0.0/tests/integration/conftest.py`

 * *Files identical despite different names*

### Comparing `vcrpy-4.4.0/tests/integration/test_aiohttp.py` & `vcrpy-5.0.0/tests/integration/test_aiohttp.py`

 * *Files 1% similar despite different names*

```diff
@@ -147,15 +147,15 @@
         assert cassette_response_json == response_json
         assert cassette.play_count == 1
 
     assert next(
         (
             log
             for log in caplog.records
-            if log.getMessage() == "<Request (POST) {}> not in cassette, sending to real server".format(url)
+            if log.getMessage() == f"<Request (POST) {url}> not in cassette, sending to real server"
         ),
         None,
     ), "Log message not found."
 
 
 @pytest.mark.online
 def test_params(tmpdir, mockbin_request_url):
```

### Comparing `vcrpy-4.4.0/tests/integration/test_basic.py` & `vcrpy-5.0.0/tests/integration/test_basic.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,7 @@
-# -*- coding: utf-8 -*-
 """Basic tests for cassettes"""
 
 # External imports
 import os
 from urllib.request import urlopen
 
 # Internal imports
```

### Comparing `vcrpy-4.4.0/tests/integration/test_boto.py` & `vcrpy-5.0.0/tests/integration/test_boto.py`

 * *Files identical despite different names*

### Comparing `vcrpy-4.4.0/tests/integration/test_boto3.py` & `vcrpy-5.0.0/tests/integration/test_boto3.py`

 * *Files 3% similar despite different names*

```diff
@@ -16,20 +16,20 @@
 except ImportError:
     botocore_awsrequest = False
 
 # skip tests if boto does not use vendored requests anymore
 # https://github.com/boto/botocore/pull/1495
 boto3_skip_vendored_requests = pytest.mark.skipif(
     botocore_awsrequest,
-    reason="botocore version {ver} does not use vendored requests anymore.".format(ver=botocore.__version__),
+    reason=f"botocore version {botocore.__version__} does not use vendored requests anymore.",
 )
 
 boto3_skip_awsrequest = pytest.mark.skipif(
     not botocore_awsrequest,
-    reason="botocore version {ver} still uses vendored requests.".format(ver=botocore.__version__),
+    reason=f"botocore version {botocore.__version__} still uses vendored requests.",
 )
 
 IAM_USER_NAME = "vcrpy"
 
 
 @pytest.fixture
 def iam_client():
```

### Comparing `vcrpy-4.4.0/tests/integration/test_config.py` & `vcrpy-5.0.0/tests/integration/test_config.py`

 * *Files identical despite different names*

### Comparing `vcrpy-4.4.0/tests/integration/test_disksaver.py` & `vcrpy-5.0.0/tests/integration/test_disksaver.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,8 +1,7 @@
-# -*- coding: utf-8 -*-
 """Basic tests about save behavior"""
 
 # External imports
 import os
 import time
 from urllib.request import urlopen
```

### Comparing `vcrpy-4.4.0/tests/integration/test_filter.py` & `vcrpy-5.0.0/tests/integration/test_filter.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import base64
 import json
 from urllib.error import HTTPError
 from urllib.parse import urlencode
 from urllib.request import Request, urlopen
 
 import pytest
-from assertions import assert_cassette_has_one_response, assert_is_json
+from assertions import assert_cassette_has_one_response, assert_is_json_bytes
 
 import vcr
 
 
 def _request_with_auth(url, username, password):
     request = Request(url)
     base64string = base64.b64encode(username.encode("ascii") + b":" + password.encode("ascii"))
@@ -101,15 +101,15 @@
     request = Request(url, headers={"Accept-Encoding": ["gzip, deflate"]})
     cass_file = str(tmpdir.join("gzip_response.yaml"))
     with vcr.use_cassette(cass_file, decode_compressed_response=True):
         urlopen(request)
     with vcr.use_cassette(cass_file) as cass:
         decoded_response = urlopen(url).read()
         assert_cassette_has_one_response(cass)
-    assert_is_json(decoded_response)
+    assert_is_json_bytes(decoded_response)
 
 
 def test_decomptess_empty_body(tmpdir, httpbin):
     url = httpbin.url + "/gzip"
     request = Request(url, headers={"Accept-Encoding": ["gzip, deflate"]}, method="HEAD")
     cass_file = str(tmpdir.join("gzip_empty_response.yaml"))
     with vcr.use_cassette(cass_file, decode_compressed_response=True):
@@ -125,27 +125,27 @@
     request = Request(url, headers={"Accept-Encoding": ["gzip, deflate"]})
     cass_file = str(tmpdir.join("deflate_response.yaml"))
     with vcr.use_cassette(cass_file, decode_compressed_response=True):
         urlopen(request)
     with vcr.use_cassette(cass_file) as cass:
         decoded_response = urlopen(url).read()
         assert_cassette_has_one_response(cass)
-    assert_is_json(decoded_response)
+    assert_is_json_bytes(decoded_response)
 
 
 def test_decompress_regular(tmpdir, httpbin):
     """Test that it doesn't try to decompress content that isn't compressed"""
     url = httpbin.url + "/get"
     cass_file = str(tmpdir.join("noncompressed_response.yaml"))
     with vcr.use_cassette(cass_file, decode_compressed_response=True):
         urlopen(url)
     with vcr.use_cassette(cass_file) as cass:
         resp = urlopen(url).read()
         assert_cassette_has_one_response(cass)
-    assert_is_json(resp)
+    assert_is_json_bytes(resp)
 
 
 def test_before_record_request_corruption(tmpdir, httpbin):
     """Modifying request in before_record_request should not affect outgoing request"""
 
     def before_record(request):
         request.headers.clear()
```

### Comparing `vcrpy-4.4.0/tests/integration/test_http` & `vcrpy-5.0.0/tests/integration/test_http`

 * *Files identical despite different names*

### Comparing `vcrpy-4.4.0/tests/integration/test_httplib2.py` & `vcrpy-5.0.0/tests/integration/test_httplib2.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,7 @@
-# -*- coding: utf-8 -*-
 """Integration tests with httplib2"""
 from urllib.parse import urlencode
 
 import pytest
 import pytest_httpbin.certs
 from assertions import assert_cassette_has_one_response
```

### Comparing `vcrpy-4.4.0/tests/integration/test_httpx.py` & `vcrpy-5.0.0/tests/integration/test_httpx.py`

 * *Files identical despite different names*

### Comparing `vcrpy-4.4.0/tests/integration/test_ignore.py` & `vcrpy-5.0.0/tests/integration/test_ignore.py`

 * *Files 19% similar despite different names*

```diff
@@ -24,45 +24,45 @@
     socket.getaddrinfo = real_getaddrinfo
 
 
 def test_ignore_localhost(tmpdir, httpbin):
     with overridden_dns({"httpbin.org": "127.0.0.1"}):
         cass_file = str(tmpdir.join("filter_qs.yaml"))
         with vcr.use_cassette(cass_file, ignore_localhost=True) as cass:
-            urlopen("http://localhost:{}/".format(httpbin.port))
+            urlopen(f"http://localhost:{httpbin.port}/")
             assert len(cass) == 0
-            urlopen("http://httpbin.org:{}/".format(httpbin.port))
+            urlopen(f"http://httpbin.org:{httpbin.port}/")
             assert len(cass) == 1
 
 
 def test_ignore_httpbin(tmpdir, httpbin):
     with overridden_dns({"httpbin.org": "127.0.0.1"}):
         cass_file = str(tmpdir.join("filter_qs.yaml"))
         with vcr.use_cassette(cass_file, ignore_hosts=["httpbin.org"]) as cass:
-            urlopen("http://httpbin.org:{}/".format(httpbin.port))
+            urlopen(f"http://httpbin.org:{httpbin.port}/")
             assert len(cass) == 0
-            urlopen("http://localhost:{}/".format(httpbin.port))
+            urlopen(f"http://localhost:{httpbin.port}/")
             assert len(cass) == 1
 
 
 def test_ignore_localhost_and_httpbin(tmpdir, httpbin):
     with overridden_dns({"httpbin.org": "127.0.0.1"}):
         cass_file = str(tmpdir.join("filter_qs.yaml"))
         with vcr.use_cassette(cass_file, ignore_hosts=["httpbin.org"], ignore_localhost=True) as cass:
-            urlopen("http://httpbin.org:{}".format(httpbin.port))
-            urlopen("http://localhost:{}".format(httpbin.port))
+            urlopen(f"http://httpbin.org:{httpbin.port}")
+            urlopen(f"http://localhost:{httpbin.port}")
             assert len(cass) == 0
 
 
 def test_ignore_localhost_twice(tmpdir, httpbin):
     with overridden_dns({"httpbin.org": "127.0.0.1"}):
         cass_file = str(tmpdir.join("filter_qs.yaml"))
         with vcr.use_cassette(cass_file, ignore_localhost=True) as cass:
-            urlopen("http://localhost:{}".format(httpbin.port))
+            urlopen(f"http://localhost:{httpbin.port}")
             assert len(cass) == 0
-            urlopen("http://httpbin.org:{}".format(httpbin.port))
+            urlopen(f"http://httpbin.org:{httpbin.port}")
             assert len(cass) == 1
         with vcr.use_cassette(cass_file, ignore_localhost=True) as cass:
             assert len(cass) == 1
-            urlopen("http://localhost:{}".format(httpbin.port))
-            urlopen("http://httpbin.org:{}".format(httpbin.port))
+            urlopen(f"http://localhost:{httpbin.port}")
+            urlopen(f"http://httpbin.org:{httpbin.port}")
             assert len(cass) == 1
```

### Comparing `vcrpy-4.4.0/tests/integration/test_matchers.py` & `vcrpy-5.0.0/tests/integration/test_matchers.py`

 * *Files identical despite different names*

### Comparing `vcrpy-4.4.0/tests/integration/test_multiple.py` & `vcrpy-5.0.0/tests/integration/test_multiple.py`

 * *Files identical despite different names*

### Comparing `vcrpy-4.4.0/tests/integration/test_proxy.py` & `vcrpy-5.0.0/tests/integration/test_proxy.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,7 @@
-# -*- coding: utf-8 -*-
 """Test using a proxy."""
 
 import http.server
 import multiprocessing
 import socketserver
 from urllib.request import urlopen
```

### Comparing `vcrpy-4.4.0/tests/integration/test_record_mode.py` & `vcrpy-5.0.0/tests/integration/test_record_mode.py`

 * *Files identical despite different names*

### Comparing `vcrpy-4.4.0/tests/integration/test_register_matcher.py` & `vcrpy-5.0.0/tests/integration/test_register_matcher.py`

 * *Files identical despite different names*

### Comparing `vcrpy-4.4.0/tests/integration/test_register_persister.py` & `vcrpy-5.0.0/tests/integration/test_register_persister.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,17 +1,18 @@
-# -*- coding: utf-8 -*-
 """Tests for cassettes with custom persistence"""
 
 # External imports
 import os
 from urllib.request import urlopen
 
+import pytest
+
 # Internal imports
 import vcr
-from vcr.persisters.filesystem import FilesystemPersister
+from vcr.persisters.filesystem import CassetteDecodeError, CassetteNotFoundError, FilesystemPersister
 
 
 class CustomFilesystemPersister:
     """Behaves just like default FilesystemPersister but adds .test extension
     to the cassette file"""
 
     @staticmethod
@@ -21,14 +22,27 @@
 
     @staticmethod
     def save_cassette(cassette_path, cassette_dict, serializer):
         cassette_path += ".test"
         FilesystemPersister.save_cassette(cassette_path, cassette_dict, serializer)
 
 
+class BadPersister(FilesystemPersister):
+    """A bad persister that raises different errors."""
+
+    @staticmethod
+    def load_cassette(cassette_path, serializer):
+        if "nonexistent" in cassette_path:
+            raise CassetteNotFoundError()
+        elif "encoding" in cassette_path:
+            raise CassetteDecodeError()
+        else:
+            raise ValueError("buggy persister")
+
+
 def test_save_cassette_with_custom_persister(tmpdir, httpbin):
     """Ensure you can save a cassette using custom persister"""
     my_vcr = vcr.VCR()
     my_vcr.register_persister(CustomFilesystemPersister)
 
     # Check to make sure directory doesn't exist
     assert not os.path.exists(str(tmpdir.join("nonexistent")))
@@ -49,7 +63,26 @@
     my_vcr.register_persister(CustomFilesystemPersister)
 
     test_fixture = str(tmpdir.join("synopsis.json.test"))
 
     with my_vcr.use_cassette(test_fixture, serializer="json"):
         response = urlopen(httpbin.url).read()
         assert b"difficult sometimes" in response
+
+
+def test_load_cassette_persister_exception_handling(tmpdir, httpbin):
+    """
+    Ensure expected errors from persister are swallowed while unexpected ones
+    are passed up the call stack.
+    """
+    my_vcr = vcr.VCR()
+    my_vcr.register_persister(BadPersister)
+
+    with my_vcr.use_cassette("bad/nonexistent") as cass:
+        assert len(cass) == 0
+
+    with my_vcr.use_cassette("bad/encoding") as cass:
+        assert len(cass) == 0
+
+    with pytest.raises(ValueError):
+        with my_vcr.use_cassette("bad/buggy") as cass:
+            pass
```

### Comparing `vcrpy-4.4.0/tests/integration/test_register_serializer.py` & `vcrpy-5.0.0/tests/integration/test_register_serializer.py`

 * *Files identical despite different names*

### Comparing `vcrpy-4.4.0/tests/integration/test_request.py` & `vcrpy-5.0.0/tests/integration/test_request.py`

 * *Files identical despite different names*

### Comparing `vcrpy-4.4.0/tests/integration/test_requests.py` & `vcrpy-5.0.0/tests/integration/test_requests.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 """Test requests' interaction with vcr"""
 import pytest
-from assertions import assert_cassette_empty, assert_is_json
+from assertions import assert_cassette_empty, assert_is_json_bytes
 
 import vcr
 
 requests = pytest.importorskip("requests")
 from requests.exceptions import ConnectionError  # noqa E402
 
 
@@ -110,30 +110,14 @@
 
     with vcr.use_cassette(str(tmpdir.join("requests.yaml"))):
         req2 = requests.post(url, data2).content
 
     assert req1 == req2
 
 
-@pytest.mark.skipif("sys.version_info >= (3, 6)", strict=True, raises=ConnectionError)
-def test_post_chunked_binary_secure(tmpdir, httpbin_secure):
-    """Ensure that we can send chunked binary without breaking while trying to concatenate bytes with str."""
-    data1 = iter([b"data", b"to", b"send"])
-    data2 = iter([b"data", b"to", b"send"])
-    url = httpbin_secure.url + "/post"
-    with vcr.use_cassette(str(tmpdir.join("requests.yaml"))):
-        req1 = requests.post(url, data1).content
-        print(req1)
-
-    with vcr.use_cassette(str(tmpdir.join("requests.yaml"))):
-        req2 = requests.post(url, data2).content
-
-    assert req1 == req2
-
-
 def test_redirects(tmpdir, httpbin_both):
     """Ensure that we can handle redirects"""
     url = httpbin_both + "/redirect-to?url=bytes/1024"
     with vcr.use_cassette(str(tmpdir.join("requests.yaml"))):
         content = requests.get(url).content
 
     with vcr.use_cassette(str(tmpdir.join("requests.yaml"))) as cass:
@@ -172,15 +156,15 @@
     Ensure that requests (actually urllib3) is able to automatically decompress
     the response body
     """
     for _ in range(2):  # one for recording, one for re-playing
         with vcr.use_cassette(str(tmpdir.join("gzip.yaml"))):
             response = requests.get(httpbin_both + "/gzip")
             assert response.headers["content-encoding"] == "gzip"  # i.e. not removed
-            assert_is_json(response.content)  # i.e. uncompressed bytes
+            assert_is_json_bytes(response.content)  # i.e. uncompressed bytes
 
 
 def test_gzip__decode_compressed_response_true(tmpdir, httpbin_both):
     url = httpbin_both + "/gzip"
 
     expected_response = requests.get(url)
     expected_content = expected_response.content
```

### Comparing `vcrpy-4.4.0/tests/integration/test_stubs.py` & `vcrpy-5.0.0/tests/integration/test_stubs.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 import http.client as httplib
 import json
 import zlib
 
-from assertions import assert_is_json
+from assertions import assert_is_json_bytes
 
 import vcr
 
 
 def _headers_are_case_insensitive(host, port):
     conn = httplib.HTTPConnection(host, port)
     conn.request("GET", "/cookies/set?k1=v1")
@@ -80,15 +80,15 @@
     # decoded and saved to the cassette.
     with vcr.use_cassette(testfile):
         conn = httplib.HTTPConnection(host, port)
         conn.request("GET", "/gzip")
         inside = conn.getresponse()
 
         assert "content-encoding" not in inside.headers
-        assert_is_json(inside.read())
+        assert_is_json_bytes(inside.read())
 
 
 def _make_before_record_response(fields, replacement="[REDACTED]"):
     def before_record_response(response):
         string_body = response["body"]["string"].decode("utf8")
         body = json.loads(string_body)
```

### Comparing `vcrpy-4.4.0/tests/integration/test_tornado.py` & `vcrpy-5.0.0/tests/integration/test_tornado.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,13 @@
-# -*- coding: utf-8 -*-
 """Test requests' interaction with vcr"""
 
 import json
 
 import pytest
-from assertions import assert_cassette_empty, assert_is_json
+from assertions import assert_cassette_empty, assert_is_json_bytes
 
 import vcr
 from vcr.errors import CannotOverwriteExistingCassetteException
 
 tornado = pytest.importorskip("tornado")
 http = pytest.importorskip("tornado.httpclient")
 
@@ -191,19 +190,19 @@
     if tornado.version_info < (4,):
         kwargs["use_gzip"] = True
     else:
         kwargs["decompress_response"] = True
 
     with vcr.use_cassette(str(tmpdir.join("gzip.yaml"))):
         response = yield get(get_client(), url, **kwargs)
-        assert_is_json(response.body)
+        assert_is_json_bytes(response.body)
 
     with vcr.use_cassette(str(tmpdir.join("gzip.yaml"))) as cass:
         response = yield get(get_client(), url, **kwargs)
-        assert_is_json(response.body)
+        assert_is_json_bytes(response.body)
         assert 1 == cass.play_count
 
 
 @pytest.mark.gen_test
 def test_https_with_cert_validation_disabled(get_client, tmpdir):
     cass_path = str(tmpdir.join("cert_validation_disabled.yaml"))
```

### Comparing `vcrpy-4.4.0/tests/integration/test_tornado_exception_can_be_caught.yaml` & `vcrpy-5.0.0/tests/integration/test_tornado_exception_can_be_caught.yaml`

 * *Files identical despite different names*

### Comparing `vcrpy-4.4.0/tests/integration/test_tornado_with_decorator_use_cassette.yaml` & `vcrpy-5.0.0/tests/integration/test_tornado_with_decorator_use_cassette.yaml`

 * *Files identical despite different names*

### Comparing `vcrpy-4.4.0/tests/integration/test_urllib2.py` & `vcrpy-5.0.0/tests/integration/test_urllib2.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,7 @@
-# -*- coding: utf-8 -*-
 """Integration tests with urllib2"""
 
 import ssl
 from urllib.parse import urlencode
 from urllib.request import urlopen
 
 import pytest_httpbin.certs
```

### Comparing `vcrpy-4.4.0/tests/integration/test_urllib3.py` & `vcrpy-5.0.0/tests/integration/test_urllib3.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 """Integration tests with urllib3"""
 
 # coding=utf-8
 
 import pytest
 import pytest_httpbin
-from assertions import assert_cassette_empty, assert_is_json
+from assertions import assert_cassette_empty, assert_is_json_bytes
 
 import vcr
 from vcr.patch import force_reset
 from vcr.stubs.compat import get_headers
 
 urllib3 = pytest.importorskip("urllib3")
 
@@ -132,18 +132,18 @@
     the response body
     """
     url = httpbin_both.url + "/gzip"
     response = verify_pool_mgr.request("GET", url)
 
     with vcr.use_cassette(str(tmpdir.join("gzip.yaml"))):
         response = verify_pool_mgr.request("GET", url)
-        assert_is_json(response.data)
+        assert_is_json_bytes(response.data)
 
     with vcr.use_cassette(str(tmpdir.join("gzip.yaml"))):
-        assert_is_json(response.data)
+        assert_is_json_bytes(response.data)
 
 
 def test_https_with_cert_validation_disabled(tmpdir, httpbin_secure, pool_mgr):
     with vcr.use_cassette(str(tmpdir.join("cert_validation_disabled.yaml"))):
         pool_mgr.request("GET", httpbin_secure.url)
```

### Comparing `vcrpy-4.4.0/tests/integration/test_wild.py` & `vcrpy-5.0.0/tests/integration/test_wild.py`

 * *Files identical despite different names*

### Comparing `vcrpy-4.4.0/tests/unit/test_cassettes.py` & `vcrpy-5.0.0/tests/unit/test_cassettes.py`

 * *Files 2% similar despite different names*

```diff
@@ -25,14 +25,27 @@
             }
         )
     )
     a_cassette = Cassette.load(path=str(a_file))
     assert len(a_cassette) == 1
 
 
+def test_cassette_load_nonexistent():
+    a_cassette = Cassette.load(path="something/nonexistent.yml")
+    assert len(a_cassette) == 0
+
+
+def test_cassette_load_invalid_encoding(tmpdir):
+    a_file = tmpdir.join("invalid_encoding.yml")
+    with open(a_file, "wb") as fd:
+        fd.write(b"\xda")
+    a_cassette = Cassette.load(path=str(a_file))
+    assert len(a_cassette) == 0
+
+
 def test_cassette_not_played():
     a = Cassette("test")
     assert not a.play_count
 
 
 def test_cassette_append():
     a = Cassette("test")
```

### Comparing `vcrpy-4.4.0/tests/unit/test_errors.py` & `vcrpy-5.0.0/tests/unit/test_errors.py`

 * *Files identical despite different names*

### Comparing `vcrpy-4.4.0/tests/unit/test_filters.py` & `vcrpy-5.0.0/tests/unit/test_filters.py`

 * *Files identical despite different names*

### Comparing `vcrpy-4.4.0/tests/unit/test_json_serializer.py` & `vcrpy-5.0.0/tests/unit/test_json_serializer.py`

 * *Files identical despite different names*

### Comparing `vcrpy-4.4.0/tests/unit/test_matchers.py` & `vcrpy-5.0.0/tests/unit/test_matchers.py`

 * *Files identical despite different names*

### Comparing `vcrpy-4.4.0/tests/unit/test_migration.py` & `vcrpy-5.0.0/tests/unit/test_migration.py`

 * *Files 4% similar despite different names*

```diff
@@ -13,28 +13,28 @@
     from yaml import Loader
 
 
 def test_try_migrate_with_json(tmpdir):
     cassette = tmpdir.join("cassette.json").strpath
     shutil.copy("tests/fixtures/migration/old_cassette.json", cassette)
     assert vcr.migration.try_migrate(cassette)
-    with open("tests/fixtures/migration/new_cassette.json", "r") as f:
+    with open("tests/fixtures/migration/new_cassette.json") as f:
         expected_json = json.load(f)
-    with open(cassette, "r") as f:
+    with open(cassette) as f:
         actual_json = json.load(f)
     assert actual_json == expected_json
 
 
 def test_try_migrate_with_yaml(tmpdir):
     cassette = tmpdir.join("cassette.yaml").strpath
     shutil.copy("tests/fixtures/migration/old_cassette.yaml", cassette)
     assert vcr.migration.try_migrate(cassette)
-    with open("tests/fixtures/migration/new_cassette.yaml", "r") as f:
+    with open("tests/fixtures/migration/new_cassette.yaml") as f:
         expected_yaml = yaml.load(f, Loader=Loader)
-    with open(cassette, "r") as f:
+    with open(cassette) as f:
         actual_yaml = yaml.load(f, Loader=Loader)
     assert actual_yaml == expected_yaml
 
 
 def test_try_migrate_with_invalid_or_new_cassettes(tmpdir):
     cassette = tmpdir.join("cassette").strpath
     files = [
```

### Comparing `vcrpy-4.4.0/tests/unit/test_persist.py` & `vcrpy-5.0.0/tests/unit/test_persist.py`

 * *Files identical despite different names*

### Comparing `vcrpy-4.4.0/tests/unit/test_request.py` & `vcrpy-5.0.0/tests/unit/test_request.py`

 * *Files identical despite different names*

### Comparing `vcrpy-4.4.0/tests/unit/test_response.py` & `vcrpy-5.0.0/tests/unit/test_response.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,7 @@
-# coding: UTF-8
 import io
 
 from vcr.stubs import VCRHTTPResponse
 
 
 def test_response_should_have_headers_field():
     recorded_response = {
```

### Comparing `vcrpy-4.4.0/tests/unit/test_serialize.py` & `vcrpy-5.0.0/tests/unit/test_serialize.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,36 +1,35 @@
-# -*- encoding: utf-8 -*-
 from unittest import mock
 
 import pytest
 
 from vcr.request import Request
 from vcr.serialize import deserialize, serialize
 from vcr.serializers import compat, jsonserializer, yamlserializer
 
 
 def test_deserialize_old_yaml_cassette():
-    with open("tests/fixtures/migration/old_cassette.yaml", "r") as f:
+    with open("tests/fixtures/migration/old_cassette.yaml") as f:
         with pytest.raises(ValueError):
             deserialize(f.read(), yamlserializer)
 
 
 def test_deserialize_old_json_cassette():
-    with open("tests/fixtures/migration/old_cassette.json", "r") as f:
+    with open("tests/fixtures/migration/old_cassette.json") as f:
         with pytest.raises(ValueError):
             deserialize(f.read(), jsonserializer)
 
 
 def test_deserialize_new_yaml_cassette():
-    with open("tests/fixtures/migration/new_cassette.yaml", "r") as f:
+    with open("tests/fixtures/migration/new_cassette.yaml") as f:
         deserialize(f.read(), yamlserializer)
 
 
 def test_deserialize_new_json_cassette():
-    with open("tests/fixtures/migration/new_cassette.json", "r") as f:
+    with open("tests/fixtures/migration/new_cassette.json") as f:
         deserialize(f.read(), jsonserializer)
 
 
 REQBODY_TEMPLATE = """\
 interactions:
 - request:
     body: {req_body}
```

### Comparing `vcrpy-4.4.0/tests/unit/test_stubs.py` & `vcrpy-5.0.0/tests/unit/test_stubs.py`

 * *Files identical despite different names*

### Comparing `vcrpy-4.4.0/tests/unit/test_unittest.py` & `vcrpy-5.0.0/tests/unit/test_unittest.py`

 * *Files identical despite different names*

### Comparing `vcrpy-4.4.0/tests/unit/test_vcr.py` & `vcrpy-5.0.0/tests/unit/test_vcr.py`

 * *Files identical despite different names*

### Comparing `vcrpy-4.4.0/tox.ini` & `vcrpy-5.0.0/tox.ini`

 * *Files 16% similar despite different names*

```diff
@@ -1,22 +1,21 @@
 [tox]
 skip_missing_interpreters=true
 envlist =
   cov-clean,
   lint,
-  {py37,py38,py39,py310,py311}-{requests-urllib3-1,httplib2,urllib3-1,tornado4,boto3,aiohttp,httpx},
+  {py38,py39,py310,py311}-{requests-urllib3-1,httplib2,urllib3-1,tornado4,boto3,aiohttp,httpx},
   {py310,py311}-{requests-urllib3-2,urllib3-2},
   {pypy3}-{requests-urllib3-1,httplib2,urllib3-1,tornado4,boto3},
   {py310}-httpx019,
   cov-report
 
 
 [gh-actions]
 python =
-    3.7: py37
     3.8: py38
     3.9: py39
     3.10: py310, lint
     3.11: py311
     pypy-3: pypy3
 
 # Coverage environment tasks: cov-clean and cov-report
@@ -62,17 +61,17 @@
 deps =
     sphinx
     sphinx_rtd_theme
 # This is the sphinx command to generate HTML.
 # In other circumstances, we might want to generate a PDF or an ebook
 commands =
     sphinx-build -W -b html -d {envtmpdir}/doctrees . {envtmpdir}/html
-# We use Python 3.7. Tox sometimes tries to autodetect it based on the name of
+# We use Python 3.8. Tox sometimes tries to autodetect it based on the name of
 # the testenv, but "docs" does not give useful clues so we have to be explicit.
-basepython = python3.7
+basepython = python3.8
 
 [testenv]
 # Need to use develop install so that paths
 # for aggregate code coverage combine
 usedevelop=true
 commands =
     ./runtests.sh --cov=./vcr --cov-branch --cov-report=xml --cov-append {posargs}
@@ -90,23 +89,22 @@
     urllib3-1: urllib3<2
     urllib3-2: urllib3<3
     boto3: boto3
     aiohttp: aiohttp
     aiohttp: pytest-asyncio
     aiohttp: pytest-aiohttp
     httpx: httpx
-    {py37,py38,py39,py310}-{httpx}: httpx
-    {py37,py38,py39,py310}-{httpx}: pytest-asyncio
+    {py38,py39,py310}-{httpx}: httpx
+    {py38,py39,py310}-{httpx}: pytest-asyncio
     httpx: httpx>0.19
-    # httpx==0.19 is the latest version that supports allow_redirects, newer versions use follow_redirects
     httpx019: httpx==0.19
-    {py37,py38,py39,py310}-{httpx}: pytest-asyncio
+    {py38,py39,py310}-{httpx}: pytest-asyncio
 depends =
-  lint,{py37,py38,py39,py310,py311,pypy3}-{requests-urllib3-1,httplib2,urllib3-1,tornado4,boto3},{py310,py311}-{requests-urllib3-2,urllib3-2},{py37,py38,py39,py310,py311}-{aiohttp},{py37,py38,py39,py310,py311}-{httpx}: cov-clean
-  cov-report: lint,{py37,py38,py39,py310,py311,pypy3}-{requests-urllib3-1,httplib2,urllib3-1,tornado4,boto3},{py310,py311}-{requests-urllib3-2,urllib3-2},{py37,py38,py39,py310,py311}-{aiohttp}
+  lint,{py38,py39,py310,py311,pypy3}-{requests-urllib3-1,httplib2,urllib3-1,tornado4,boto3},{py310,py311}-{requests-urllib3-2,urllib3-2},{py38,py39,py310,py311}-{aiohttp},{py38,py39,py310,py311}-{httpx}: cov-clean
+  cov-report: lint,{py38,py39,py310,py311,pypy3}-{requests-urllib3-1,httplib2,urllib3-1,tornado4,boto3},{py310,py311}-{requests-urllib3-2,urllib3-2},{py38,py39,py310,py311}-{aiohttp}
 passenv =
     AWS_ACCESS_KEY_ID
     AWS_DEFAULT_REGION
     AWS_SECRET_ACCESS_KEY
 
 [flake8]
 max_line_length = 110
```

### Comparing `vcrpy-4.4.0/vcr/cassette.py` & `vcrpy-5.0.0/vcr/cassette.py`

 * *Files 2% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 
 import wrapt
 
 from ._handle_coroutine import handle_coroutine
 from .errors import UnhandledHTTPRequestError
 from .matchers import get_matchers_results, method, requests_match, uri
 from .patch import CassettePatcherBuilder
-from .persisters.filesystem import FilesystemPersister
+from .persisters.filesystem import CassetteDecodeError, CassetteNotFoundError, FilesystemPersister
 from .record_mode import RecordMode
 from .serializers import yamlserializer
 from .util import partition_dict
 
 try:
     from asyncio import iscoroutinefunction
 except ImportError:
@@ -276,30 +276,30 @@
         """
         for index, response in self._responses(request):
             if self.play_counts[index] == 0 or self.allow_playback_repeats:
                 self.play_counts[index] += 1
                 return response
         # The cassette doesn't contain the request asked for.
         raise UnhandledHTTPRequestError(
-            "The cassette (%r) doesn't contain the request (%r) asked for" % (self._path, request)
+            f"The cassette ({self._path!r}) doesn't contain the request ({request!r}) asked for"
         )
 
     def responses_of(self, request):
         """
         Find the responses corresponding to a request.
         This function isn't actually used by VCR internally, but is
         provided as an external API.
         """
         responses = [response for index, response in self._responses(request)]
 
         if responses:
             return responses
         # The cassette doesn't contain the request asked for.
         raise UnhandledHTTPRequestError(
-            "The cassette (%r) doesn't contain the request (%r) asked for" % (self._path, request)
+            f"The cassette ({self._path!r}) doesn't contain the request ({request!r}) asked for"
         )
 
     def rewind(self):
         self.play_counts = collections.Counter()
 
     def find_requests_with_most_matches(self, request):
         """
@@ -348,19 +348,19 @@
     def _load(self):
         try:
             requests, responses = self._persister.load_cassette(self._path, serializer=self._serializer)
             for request, response in zip(requests, responses):
                 self.append(request, response)
             self.dirty = False
             self.rewound = True
-        except ValueError:
+        except (CassetteDecodeError, CassetteNotFoundError):
             pass
 
     def __str__(self):
-        return "<Cassette containing {} recorded response(s)>".format(len(self))
+        return f"<Cassette containing {len(self)} recorded response(s)>"
 
     def __len__(self):
         """Return the number of request,response pairs stored in here"""
         return len(self.data)
 
     def __contains__(self, request):
         """Return whether or not a request has been stored"""
```

### Comparing `vcrpy-4.4.0/vcr/config.py` & `vcrpy-5.0.0/vcr/config.py`

 * *Files 1% similar despite different names*

```diff
@@ -84,24 +84,24 @@
         self.record_on_exception = record_on_exception
         self._custom_patches = tuple(custom_patches)
 
     def _get_serializer(self, serializer_name):
         try:
             serializer = self.serializers[serializer_name]
         except KeyError:
-            raise KeyError("Serializer {} doesn't exist or isn't registered".format(serializer_name))
+            raise KeyError(f"Serializer {serializer_name} doesn't exist or isn't registered")
         return serializer
 
     def _get_matchers(self, matcher_names):
         matchers = []
         try:
             for m in matcher_names:
                 matchers.append(self.matchers[m])
         except KeyError:
-            raise KeyError("Matcher {} doesn't exist or isn't registered".format(m))
+            raise KeyError(f"Matcher {m} doesn't exist or isn't registered")
         return matchers
 
     def use_cassette(self, path=None, **kwargs):
         if path is not None and not isinstance(path, (str, Path)):
             function = path
             # Assume this is an attempt to decorate a function
             return self._use_cassette(**kwargs)(function)
```

### Comparing `vcrpy-4.4.0/vcr/errors.py` & `vcrpy-5.0.0/vcr/errors.py`

 * *Files identical despite different names*

### Comparing `vcrpy-4.4.0/vcr/filters.py` & `vcrpy-5.0.0/vcr/filters.py`

 * *Files identical despite different names*

### Comparing `vcrpy-4.4.0/vcr/matchers.py` & `vcrpy-5.0.0/vcr/matchers.py`

 * *Files 17% similar despite different names*

```diff
@@ -6,45 +6,45 @@
 from .util import read_body
 
 log = logging.getLogger(__name__)
 
 
 def method(r1, r2):
     if r1.method != r2.method:
-        raise AssertionError("{} != {}".format(r1.method, r2.method))
+        raise AssertionError(f"{r1.method} != {r2.method}")
 
 
 def uri(r1, r2):
     if r1.uri != r2.uri:
-        raise AssertionError("{} != {}".format(r1.uri, r2.uri))
+        raise AssertionError(f"{r1.uri} != {r2.uri}")
 
 
 def host(r1, r2):
     if r1.host != r2.host:
-        raise AssertionError("{} != {}".format(r1.host, r2.host))
+        raise AssertionError(f"{r1.host} != {r2.host}")
 
 
 def scheme(r1, r2):
     if r1.scheme != r2.scheme:
-        raise AssertionError("{} != {}".format(r1.scheme, r2.scheme))
+        raise AssertionError(f"{r1.scheme} != {r2.scheme}")
 
 
 def port(r1, r2):
     if r1.port != r2.port:
-        raise AssertionError("{} != {}".format(r1.port, r2.port))
+        raise AssertionError(f"{r1.port} != {r2.port}")
 
 
 def path(r1, r2):
     if r1.path != r2.path:
-        raise AssertionError("{} != {}".format(r1.path, r2.path))
+        raise AssertionError(f"{r1.path} != {r2.path}")
 
 
 def query(r1, r2):
     if r1.query != r2.query:
-        raise AssertionError("{} != {}".format(r1.query, r2.query))
+        raise AssertionError(f"{r1.query} != {r2.query}")
 
 
 def raw_body(r1, r2):
     if read_body(r1) != read_body(r2):
         raise AssertionError
 
 
@@ -55,15 +55,15 @@
         transformer = _identity
     if transformer(read_body(r1)) != transformer(read_body(r2)):
         raise AssertionError
 
 
 def headers(r1, r2):
     if r1.headers != r2.headers:
-        raise AssertionError("{} != {}".format(r1.headers, r2.headers))
+        raise AssertionError(f"{r1.headers} != {r2.headers}")
 
 
 def _header_checker(value, header="Content-Type"):
     def checker(headers):
         _header = headers.get(header, "")
         if isinstance(_header, bytes):
             _header = _header.decode("utf-8")
@@ -103,15 +103,15 @@
     else:
         return _identity
 
 
 def requests_match(r1, r2, matchers):
     successes, failures = get_matchers_results(r1, r2, matchers)
     if failures:
-        log.debug("Requests {} and {} differ.\n" "Failure details:\n" "{}".format(r1, r2, failures))
+        log.debug(f"Requests {r1} and {r2} differ.\nFailure details:\n{failures}")
     return len(failures) == 0
 
 
 def _evaluate_matcher(matcher_function, *args):
     """
     Evaluate the result of a given matcher as a boolean with an assertion error message if any.
     It handles two types of matcher :
```

### Comparing `vcrpy-4.4.0/vcr/migration.py` & `vcrpy-5.0.0/vcr/migration.py`

 * *Files 2% similar despite different names*

```diff
@@ -51,15 +51,15 @@
 PARTS = ["protocol", "host", "port", "path"]
 
 
 def build_uri(**parts):
     port = parts["port"]
     scheme = parts["protocol"]
     default_port = {"https": 443, "http": 80}[scheme]
-    parts["port"] = ":{}".format(port) if port != default_port else ""
+    parts["port"] = f":{port}" if port != default_port else ""
     return "{protocol}://{host}{port}{path}".format(**parts)
 
 
 def _migrate(data):
     interactions = []
     for item in data:
         req = item["request"]
@@ -114,15 +114,15 @@
     return True
 
 
 def migrate(file_path, migration_fn):
     # because we assume that original files can be reverted
     # we will try to copy the content. (os.rename not needed)
     with tempfile.TemporaryFile(mode="w+") as out_fp:
-        with open(file_path, "r") as in_fp:
+        with open(file_path) as in_fp:
             if not migration_fn(in_fp, out_fp):
                 return False
         with open(file_path, "w") as in_fp:
             out_fp.seek(0)
             shutil.copyfileobj(out_fp, in_fp)
         return True
 
@@ -146,13 +146,13 @@
         path = os.path.abspath(path)
     files = [path]
     if os.path.isdir(path):
         files = (os.path.join(root, name) for (root, dirs, files) in os.walk(path) for name in files)
     for file_path in files:
         migrated = try_migrate(file_path)
         status = "OK" if migrated else "FAIL"
-        sys.stderr.write("[{}] {}\n".format(status, file_path))
+        sys.stderr.write(f"[{status}] {file_path}\n")
     sys.stderr.write("Done.\n")
 
 
 if __name__ == "__main__":
     main()
```

### Comparing `vcrpy-4.4.0/vcr/patch.py` & `vcrpy-5.0.0/vcr/patch.py`

 * *Files 1% similar despite different names*

```diff
@@ -182,17 +182,15 @@
             self._class_to_cassette_subclass[klass] = subclass
         return self._class_to_cassette_subclass[klass]
 
     def _build_cassette_subclass(self, base_class):
         bases = (base_class,)
         if not issubclass(base_class, object):  # Check for old style class
             bases += (object,)
-        return type(
-            "{}{}".format(base_class.__name__, self._cassette._path), bases, dict(cassette=self._cassette)
-        )
+        return type(f"{base_class.__name__}{self._cassette._path}", bases, dict(cassette=self._cassette))
 
     @_build_patchers_from_mock_triples_decorator
     def _httplib(self):
         yield httplib, "HTTPConnection", VCRHTTPConnection
         yield httplib, "HTTPSConnection", VCRHTTPSConnection
 
     def _requests(self):
```

### Comparing `vcrpy-4.4.0/vcr/persisters/filesystem.py` & `vcrpy-5.0.0/vcr/persisters/filesystem.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,25 +1,33 @@
 # .. _persister_example:
 
 from pathlib import Path
 
 from ..serialize import deserialize, serialize
 
 
+class CassetteNotFoundError(FileNotFoundError):
+    pass
+
+
+class CassetteDecodeError(ValueError):
+    pass
+
+
 class FilesystemPersister:
     @classmethod
     def load_cassette(cls, cassette_path, serializer):
         cassette_path = Path(cassette_path)  # if cassette path is already Path this is no operation
         if not cassette_path.is_file():
-            raise ValueError("Cassette not found.")
+            raise CassetteNotFoundError()
         try:
             with cassette_path.open() as f:
                 data = f.read()
-        except UnicodeEncodeError as err:
-            raise ValueError("Can't read Cassette, Encoding is broken") from err
+        except UnicodeDecodeError as err:
+            raise CassetteDecodeError("Can't read Cassette, Encoding is broken") from err
 
         return deserialize(data, serializer)
 
     @staticmethod
     def save_cassette(cassette_path, cassette_dict, serializer):
         data = serialize(cassette_dict, serializer)
         cassette_path = Path(cassette_path)  # if cassette path is already Path this is no operation
```

### Comparing `vcrpy-4.4.0/vcr/record_mode.py` & `vcrpy-5.0.0/vcr/record_mode.py`

 * *Files identical despite different names*

### Comparing `vcrpy-4.4.0/vcr/request.py` & `vcrpy-5.0.0/vcr/request.py`

 * *Files 3% similar despite different names*

```diff
@@ -86,15 +86,15 @@
 
     # alias for backwards compatibility
     @property
     def protocol(self):
         return self.scheme
 
     def __str__(self):
-        return "<Request ({}) {}>".format(self.method, self.uri)
+        return f"<Request ({self.method}) {self.uri}>"
 
     def __repr__(self):
         return self.__str__()
 
     def _to_dict(self):
         return {
             "method": self.method,
```

### Comparing `vcrpy-4.4.0/vcr/serialize.py` & `vcrpy-5.0.0/vcr/serialize.py`

 * *Files identical despite different names*

### Comparing `vcrpy-4.4.0/vcr/serializers/compat.py` & `vcrpy-5.0.0/vcr/serializers/compat.py`

 * *Files identical despite different names*

### Comparing `vcrpy-4.4.0/vcr/serializers/jsonserializer.py` & `vcrpy-5.0.0/vcr/serializers/jsonserializer.py`

 * *Files identical despite different names*

### Comparing `vcrpy-4.4.0/vcr/stubs/__init__.py` & `vcrpy-5.0.0/vcr/stubs/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -184,34 +184,34 @@
 
     def _port_postfix(self):
         """
         Returns empty string for the default port and ':port' otherwise
         """
         port = self.real_connection.port
         default_port = {"https": 443, "http": 80}[self._protocol]
-        return ":{}".format(port) if port != default_port else ""
+        return f":{port}" if port != default_port else ""
 
     def _uri(self, url):
         """Returns request absolute URI"""
         if url and not url.startswith("/"):
             # Then this must be a proxy request.
             return url
-        uri = "{}://{}{}{}".format(self._protocol, self.real_connection.host, self._port_postfix(), url)
+        uri = f"{self._protocol}://{self.real_connection.host}{self._port_postfix()}{url}"
         log.debug("Absolute URI: %s", uri)
         return uri
 
     def _url(self, uri):
         """Returns request selector url from absolute URI"""
-        prefix = "{}://{}{}".format(self._protocol, self.real_connection.host, self._port_postfix())
+        prefix = f"{self._protocol}://{self.real_connection.host}{self._port_postfix()}"
         return uri.replace(prefix, "", 1)
 
     def request(self, method, url, body=None, headers=None, *args, **kwargs):
         """Persist the request metadata in self._vcr_request"""
         self._vcr_request = Request(method=method, uri=self._uri(url), body=body, headers=headers or {})
-        log.debug("Got {}".format(self._vcr_request))
+        log.debug(f"Got {self._vcr_request}")
 
         # Note: The request may not actually be finished at this point, so
         # I'm not sending the actual request until getresponse().  This
         # allows me to compare the entire length of the response to see if it
         # exists in the cassette.
 
         self._sock = VCRFakeSocket()
@@ -219,15 +219,15 @@
     def putrequest(self, method, url, *args, **kwargs):
         """
         httplib gives you more than one way to do it.  This is a way
         to start building up a request.  Usually followed by a bunch
         of putheader() calls.
         """
         self._vcr_request = Request(method=method, uri=self._uri(url), body="", headers={})
-        log.debug("Got {}".format(self._vcr_request))
+        log.debug(f"Got {self._vcr_request}")
 
     def putheader(self, header, *values):
         self._vcr_request.headers[header] = values
 
     def send(self, data):
         """
         This method is called after request(), to add additional data to the
@@ -251,27 +251,27 @@
             self._vcr_request.body = message_body
 
     def getresponse(self, _=False, **kwargs):
         """Retrieve the response"""
         # Check to see if the cassette has a response for this request. If so,
         # then return it
         if self.cassette.can_play_response_for(self._vcr_request):
-            log.info("Playing response for {} from cassette".format(self._vcr_request))
+            log.info(f"Playing response for {self._vcr_request} from cassette")
             response = self.cassette.play_response(self._vcr_request)
             return VCRHTTPResponse(response)
         else:
             if self.cassette.write_protected and self.cassette.filter_request(self._vcr_request):
                 raise CannotOverwriteExistingCassetteException(
                     cassette=self.cassette, failed_request=self._vcr_request
                 )
 
             # Otherwise, we should send the request, then get the response
             # and return it.
 
-            log.info("{} not in cassette, sending to real server".format(self._vcr_request))
+            log.info(f"{self._vcr_request} not in cassette, sending to real server")
             # This is imported here to avoid circular import.
             # TODO(@IvanMalison): Refactor to allow normal import.
             from vcr.patch import force_reset
 
             with force_reset():
                 self.real_connection.request(
                     method=self._vcr_request.method,
```

### Comparing `vcrpy-4.4.0/vcr/stubs/aiohttp_stubs.py` & `vcrpy-5.0.0/vcr/stubs/aiohttp_stubs.py`

 * *Files 2% similar despite different names*

```diff
@@ -257,15 +257,15 @@
         cookie_header = _build_cookie_header(self, cookies, c_header, request_url)
         if cookie_header:
             headers[hdrs.COOKIE] = cookie_header
 
         vcr_request = Request(method, str(request_url), data, _serialize_headers(headers))
 
         if cassette.can_play_response_for(vcr_request):
-            log.info("Playing response for {} from cassette".format(vcr_request))
+            log.info(f"Playing response for {vcr_request} from cassette")
             response = play_responses(cassette, vcr_request, kwargs)
             for redirect in response.history:
                 self._cookie_jar.update_cookies(redirect.cookies, redirect.url)
             self._cookie_jar.update_cookies(response.cookies, response.url)
             return response
 
         if cassette.write_protected and cassette.filter_request(vcr_request):
```

### Comparing `vcrpy-4.4.0/vcr/stubs/boto3_stubs.py` & `vcrpy-5.0.0/vcr/stubs/boto3_stubs.py`

 * *Files identical despite different names*

### Comparing `vcrpy-4.4.0/vcr/stubs/compat.py` & `vcrpy-5.0.0/vcr/stubs/compat.py`

 * *Files identical despite different names*

### Comparing `vcrpy-4.4.0/vcr/stubs/httplib2_stubs.py` & `vcrpy-5.0.0/vcr/stubs/httplib2_stubs.py`

 * *Files identical despite different names*

### Comparing `vcrpy-4.4.0/vcr/stubs/httpx_stubs.py` & `vcrpy-5.0.0/vcr/stubs/httpx_stubs.py`

 * *Files identical despite different names*

### Comparing `vcrpy-4.4.0/vcr/stubs/requests_stubs.py` & `vcrpy-5.0.0/vcr/stubs/requests_stubs.py`

 * *Files identical despite different names*

### Comparing `vcrpy-4.4.0/vcr/stubs/tornado_stubs.py` & `vcrpy-5.0.0/vcr/stubs/tornado_stubs.py`

 * *Files identical despite different names*

### Comparing `vcrpy-4.4.0/vcr/unittest.py` & `vcrpy-5.0.0/vcr/unittest.py`

 * *Files 11% similar despite different names*

```diff
@@ -28,12 +28,12 @@
         return kwargs
 
     def _get_cassette_library_dir(self):
         testdir = os.path.dirname(inspect.getfile(self.__class__))
         return os.path.join(testdir, "cassettes")
 
     def _get_cassette_name(self):
-        return "{0}.{1}.yaml".format(self.__class__.__name__, self._testMethodName)
+        return f"{self.__class__.__name__}.{self._testMethodName}.yaml"
 
 
 class VCRTestCase(VCRMixin, unittest.TestCase):
     pass
```

### Comparing `vcrpy-4.4.0/vcr/util.py` & `vcrpy-5.0.0/vcr/util.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,13 +1,9 @@
 import types
-
-try:
-    from collections.abc import Mapping, MutableMapping
-except ImportError:
-    from collections import Mapping, MutableMapping
+from collections.abc import Mapping, MutableMapping
 
 
 # Shamelessly stolen from https://github.com/kennethreitz/requests/blob/master/requests/structures.py
 class CaseInsensitiveDict(MutableMapping):
     """
     A case-insensitive ``dict``-like object.
     Implements all methods and operations of
```

### Comparing `vcrpy-4.4.0/vcrpy.egg-info/PKG-INFO` & `vcrpy-5.0.0/vcrpy.egg-info/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,32 +1,31 @@
 Metadata-Version: 2.1
 Name: vcrpy
-Version: 4.4.0
+Version: 5.0.0
 Summary: Automatically mock your HTTP interactions to simplify and speed up testing
 Home-page: https://github.com/kevin1024/vcrpy
 Author: Kevin McCarthy
 Author-email: me@kevinmccarthy.org
 License: MIT
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Environment :: Console
 Classifier: Intended Audience :: Developers
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3 :: Only
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Classifier: Programming Language :: Python :: Implementation :: PyPy
 Classifier: Topic :: Software Development :: Testing
 Classifier: Topic :: Internet :: WWW/HTTP
 Classifier: License :: OSI Approved :: MIT License
-Requires-Python: >=3.7
+Requires-Python: >=3.8
 Description-Content-Type: text/x-rst
 License-File: LICENSE.txt
 
 
 ###########
 VCR.py 📼
 ###########
```

### Comparing `vcrpy-4.4.0/vcrpy.egg-info/SOURCES.txt` & `vcrpy-5.0.0/vcrpy.egg-info/SOURCES.txt`

 * *Files identical despite different names*

