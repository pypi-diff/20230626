# Comparing `tmp/lf-metric-emitter-0.0.2.tar.gz` & `tmp/lf-metric-emitter-0.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "lf-metric-emitter-0.0.2.tar", last modified: Fri Jun 23 17:23:14 2023, max compression
+gzip compressed data, was "lf-metric-emitter-0.0.3.tar", last modified: Mon Jun 26 20:29:37 2023, max compression
```

## Comparing `lf-metric-emitter-0.0.2.tar` & `lf-metric-emitter-0.0.3.tar`

### file list

```diff
@@ -1,40 +1,41 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 17:23:14.297565 lf-metric-emitter-0.0.2/
--rw-r--r--   0 runner    (1001) docker     (123)      413 2023-06-23 17:23:00.000000 lf-metric-emitter-0.0.2/.copier-answers.yml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 17:23:14.293565 lf-metric-emitter-0.0.2/.github/
--rw-r--r--   0 runner    (1001) docker     (123)     3566 2023-06-23 17:23:00.000000 lf-metric-emitter-0.0.2/.github/pull_request_template.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 17:23:14.293565 lf-metric-emitter-0.0.2/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)      764 2023-06-23 17:23:00.000000 lf-metric-emitter-0.0.2/.github/workflows/build-documentation.yml
--rw-r--r--   0 runner    (1001) docker     (123)      958 2023-06-23 17:23:00.000000 lf-metric-emitter-0.0.2/.github/workflows/linting.yml
--rw-r--r--   0 runner    (1001) docker     (123)     1009 2023-06-23 17:23:00.000000 lf-metric-emitter-0.0.2/.github/workflows/publish-to-pypi.yml
--rw-r--r--   0 runner    (1001) docker     (123)      842 2023-06-23 17:23:00.000000 lf-metric-emitter-0.0.2/.github/workflows/smoke-test.yml
--rw-r--r--   0 runner    (1001) docker     (123)     1120 2023-06-23 17:23:00.000000 lf-metric-emitter-0.0.2/.github/workflows/testing-and-coverage.yml
--rw-r--r--   0 runner    (1001) docker     (123)     1893 2023-06-23 17:23:00.000000 lf-metric-emitter-0.0.2/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)     3570 2023-06-23 17:23:00.000000 lf-metric-emitter-0.0.2/.pre-commit-config.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      471 2023-06-23 17:23:00.000000 lf-metric-emitter-0.0.2/.readthedocs.yml
--rw-r--r--   0 runner    (1001) docker     (123)     1073 2023-06-23 17:23:00.000000 lf-metric-emitter-0.0.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     3448 2023-06-23 17:23:14.297565 lf-metric-emitter-0.0.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1729 2023-06-23 17:23:00.000000 lf-metric-emitter-0.0.2/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 17:23:14.293565 lf-metric-emitter-0.0.2/docs/
--rw-r--r--   0 runner    (1001) docker     (123)      787 2023-06-23 17:23:00.000000 lf-metric-emitter-0.0.2/docs/Makefile
--rw-r--r--   0 runner    (1001) docker     (123)     1625 2023-06-23 17:23:00.000000 lf-metric-emitter-0.0.2/docs/conf.py
--rw-r--r--   0 runner    (1001) docker     (123)      378 2023-06-23 17:23:00.000000 lf-metric-emitter-0.0.2/docs/index.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 17:23:14.293565 lf-metric-emitter-0.0.2/docs/notebooks/
--rw-r--r--   0 runner    (1001) docker     (123)       35 2023-06-23 17:23:00.000000 lf-metric-emitter-0.0.2/docs/notebooks/README.md
--rw-r--r--   0 runner    (1001) docker     (123)       60 2023-06-23 17:23:00.000000 lf-metric-emitter-0.0.2/docs/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1339 2023-06-23 17:23:00.000000 lf-metric-emitter-0.0.2/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-23 17:23:14.297565 lf-metric-emitter-0.0.2/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 17:23:14.293565 lf-metric-emitter-0.0.2/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 17:23:14.297565 lf-metric-emitter-0.0.2/src/lf_metric_emitter.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     3448 2023-06-23 17:23:14.000000 lf-metric-emitter-0.0.2/src/lf_metric_emitter.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      798 2023-06-23 17:23:14.000000 lf-metric-emitter-0.0.2/src/lf_metric_emitter.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-23 17:23:14.000000 lf-metric-emitter-0.0.2/src/lf_metric_emitter.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      102 2023-06-23 17:23:14.000000 lf-metric-emitter-0.0.2/src/lf_metric_emitter.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       15 2023-06-23 17:23:14.000000 lf-metric-emitter-0.0.2/src/lf_metric_emitter.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 17:23:14.297565 lf-metric-emitter-0.0.2/src/metric_emitter/
--rw-r--r--   0 runner    (1001) docker     (123)       29 2023-06-23 17:23:00.000000 lf-metric-emitter-0.0.2/src/metric_emitter/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      160 2023-06-23 17:23:14.000000 lf-metric-emitter-0.0.2/src/metric_emitter/_version.py
--rw-r--r--   0 runner    (1001) docker     (123)     5096 2023-06-23 17:23:00.000000 lf-metric-emitter-0.0.2/src/metric_emitter/emitter.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 17:23:14.293565 lf-metric-emitter-0.0.2/tests/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 17:23:14.297565 lf-metric-emitter-0.0.2/tests/metric_emitter/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-23 17:23:00.000000 lf-metric-emitter-0.0.2/tests/metric_emitter/conftest.py
--rw-r--r--   0 runner    (1001) docker     (123)      264 2023-06-23 17:23:00.000000 lf-metric-emitter-0.0.2/tests/metric_emitter/test_emitter.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 20:29:37.564478 lf-metric-emitter-0.0.3/
+-rw-r--r--   0 runner    (1001) docker     (123)      413 2023-06-26 20:29:25.000000 lf-metric-emitter-0.0.3/.copier-answers.yml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 20:29:37.564478 lf-metric-emitter-0.0.3/.github/
+-rw-r--r--   0 runner    (1001) docker     (123)      687 2023-06-26 20:29:25.000000 lf-metric-emitter-0.0.3/.github/dependabot.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     3566 2023-06-26 20:29:25.000000 lf-metric-emitter-0.0.3/.github/pull_request_template.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 20:29:37.564478 lf-metric-emitter-0.0.3/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)      764 2023-06-26 20:29:25.000000 lf-metric-emitter-0.0.3/.github/workflows/build-documentation.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      958 2023-06-26 20:29:25.000000 lf-metric-emitter-0.0.3/.github/workflows/linting.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1009 2023-06-26 20:29:25.000000 lf-metric-emitter-0.0.3/.github/workflows/publish-to-pypi.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      842 2023-06-26 20:29:25.000000 lf-metric-emitter-0.0.3/.github/workflows/smoke-test.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1120 2023-06-26 20:29:25.000000 lf-metric-emitter-0.0.3/.github/workflows/testing-and-coverage.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1893 2023-06-26 20:29:25.000000 lf-metric-emitter-0.0.3/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)     3570 2023-06-26 20:29:25.000000 lf-metric-emitter-0.0.3/.pre-commit-config.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      471 2023-06-26 20:29:25.000000 lf-metric-emitter-0.0.3/.readthedocs.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1073 2023-06-26 20:29:25.000000 lf-metric-emitter-0.0.3/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     3448 2023-06-26 20:29:37.564478 lf-metric-emitter-0.0.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1729 2023-06-26 20:29:25.000000 lf-metric-emitter-0.0.3/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 20:29:37.564478 lf-metric-emitter-0.0.3/docs/
+-rw-r--r--   0 runner    (1001) docker     (123)      787 2023-06-26 20:29:25.000000 lf-metric-emitter-0.0.3/docs/Makefile
+-rw-r--r--   0 runner    (1001) docker     (123)     1625 2023-06-26 20:29:25.000000 lf-metric-emitter-0.0.3/docs/conf.py
+-rw-r--r--   0 runner    (1001) docker     (123)      378 2023-06-26 20:29:25.000000 lf-metric-emitter-0.0.3/docs/index.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 20:29:37.564478 lf-metric-emitter-0.0.3/docs/notebooks/
+-rw-r--r--   0 runner    (1001) docker     (123)       35 2023-06-26 20:29:25.000000 lf-metric-emitter-0.0.3/docs/notebooks/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       60 2023-06-26 20:29:25.000000 lf-metric-emitter-0.0.3/docs/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1339 2023-06-26 20:29:25.000000 lf-metric-emitter-0.0.3/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-26 20:29:37.564478 lf-metric-emitter-0.0.3/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 20:29:37.560478 lf-metric-emitter-0.0.3/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 20:29:37.564478 lf-metric-emitter-0.0.3/src/lf_metric_emitter.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     3448 2023-06-26 20:29:37.000000 lf-metric-emitter-0.0.3/src/lf_metric_emitter.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      821 2023-06-26 20:29:37.000000 lf-metric-emitter-0.0.3/src/lf_metric_emitter.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-26 20:29:37.000000 lf-metric-emitter-0.0.3/src/lf_metric_emitter.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      102 2023-06-26 20:29:37.000000 lf-metric-emitter-0.0.3/src/lf_metric_emitter.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       15 2023-06-26 20:29:37.000000 lf-metric-emitter-0.0.3/src/lf_metric_emitter.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 20:29:37.564478 lf-metric-emitter-0.0.3/src/metric_emitter/
+-rw-r--r--   0 runner    (1001) docker     (123)       29 2023-06-26 20:29:25.000000 lf-metric-emitter-0.0.3/src/metric_emitter/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      160 2023-06-26 20:29:37.000000 lf-metric-emitter-0.0.3/src/metric_emitter/_version.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5302 2023-06-26 20:29:25.000000 lf-metric-emitter-0.0.3/src/metric_emitter/emitter.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 20:29:37.560478 lf-metric-emitter-0.0.3/tests/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 20:29:37.564478 lf-metric-emitter-0.0.3/tests/metric_emitter/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-26 20:29:25.000000 lf-metric-emitter-0.0.3/tests/metric_emitter/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (123)      264 2023-06-26 20:29:25.000000 lf-metric-emitter-0.0.3/tests/metric_emitter/test_emitter.py
```

### Comparing `lf-metric-emitter-0.0.2/.github/pull_request_template.md` & `lf-metric-emitter-0.0.3/.github/pull_request_template.md`

 * *Files identical despite different names*

### Comparing `lf-metric-emitter-0.0.2/.github/workflows/build-documentation.yml` & `lf-metric-emitter-0.0.3/.github/workflows/build-documentation.yml`

 * *Files identical despite different names*

### Comparing `lf-metric-emitter-0.0.2/.github/workflows/linting.yml` & `lf-metric-emitter-0.0.3/.github/workflows/linting.yml`

 * *Files identical despite different names*

### Comparing `lf-metric-emitter-0.0.2/.github/workflows/publish-to-pypi.yml` & `lf-metric-emitter-0.0.3/.github/workflows/publish-to-pypi.yml`

 * *Files identical despite different names*

### Comparing `lf-metric-emitter-0.0.2/.github/workflows/smoke-test.yml` & `lf-metric-emitter-0.0.3/.github/workflows/smoke-test.yml`

 * *Files identical despite different names*

### Comparing `lf-metric-emitter-0.0.2/.github/workflows/testing-and-coverage.yml` & `lf-metric-emitter-0.0.3/.github/workflows/testing-and-coverage.yml`

 * *Files identical despite different names*

### Comparing `lf-metric-emitter-0.0.2/.gitignore` & `lf-metric-emitter-0.0.3/.gitignore`

 * *Files identical despite different names*

### Comparing `lf-metric-emitter-0.0.2/.pre-commit-config.yaml` & `lf-metric-emitter-0.0.3/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `lf-metric-emitter-0.0.2/LICENSE` & `lf-metric-emitter-0.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `lf-metric-emitter-0.0.2/PKG-INFO` & `lf-metric-emitter-0.0.3/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: lf-metric-emitter
-Version: 0.0.2
+Version: 0.0.3
 Author-email: LINCC Frameworks <name@you.com>
 License: MIT License
         
         Copyright (c) 2023 LINCC Frameworks
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
         of this software and associated documentation files (the "Software"), to deal
```

### Comparing `lf-metric-emitter-0.0.2/README.md` & `lf-metric-emitter-0.0.3/README.md`

 * *Files identical despite different names*

### Comparing `lf-metric-emitter-0.0.2/docs/Makefile` & `lf-metric-emitter-0.0.3/docs/Makefile`

 * *Files identical despite different names*

### Comparing `lf-metric-emitter-0.0.2/docs/conf.py` & `lf-metric-emitter-0.0.3/docs/conf.py`

 * *Files identical despite different names*

### Comparing `lf-metric-emitter-0.0.2/pyproject.toml` & `lf-metric-emitter-0.0.3/pyproject.toml`

 * *Files identical despite different names*

### Comparing `lf-metric-emitter-0.0.2/src/lf_metric_emitter.egg-info/PKG-INFO` & `lf-metric-emitter-0.0.3/src/lf_metric_emitter.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: lf-metric-emitter
-Version: 0.0.2
+Version: 0.0.3
 Author-email: LINCC Frameworks <name@you.com>
 License: MIT License
         
         Copyright (c) 2023 LINCC Frameworks
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
         of this software and associated documentation files (the "Software"), to deal
```

### Comparing `lf-metric-emitter-0.0.2/src/lf_metric_emitter.egg-info/SOURCES.txt` & `lf-metric-emitter-0.0.3/src/lf_metric_emitter.egg-info/SOURCES.txt`

 * *Files 12% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 .copier-answers.yml
 .gitignore
 .pre-commit-config.yaml
 .readthedocs.yml
 LICENSE
 README.md
 pyproject.toml
+.github/dependabot.yml
 .github/pull_request_template.md
 .github/workflows/build-documentation.yml
 .github/workflows/linting.yml
 .github/workflows/publish-to-pypi.yml
 .github/workflows/smoke-test.yml
 .github/workflows/testing-and-coverage.yml
 docs/Makefile
```

### Comparing `lf-metric-emitter-0.0.2/src/metric_emitter/emitter.py` & `lf-metric-emitter-0.0.3/src/metric_emitter/emitter.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 import json
 import os
 import requests
 import time
 
 from collections.abc import Iterable
 from numbers import Number
+from urllib.parse import urljoin
 
 schema = {
     "namespace": "placholder",
     "type": "record",
     "name": "placeholder",
     "fields": [
         {
@@ -137,15 +138,20 @@
             "Accept": "application/vnd.kafka.v2+json",
         }
 
         base_url = os.environ.get("KAFKA_API_URL", None)
 
         if base_url is None or self.record["benchmark_env"] == "unknown":
             print(f"Base URL: {base_url}")
-            print(f"Benchmark environment: {self.record['benchmark_env']}")
             print(payload)
 
         else:
             # results in url like: `https://example.com/lsst.example.metric.name`
-            full_url = base_url + "/" + ".".join([self.schema["namespace"], self.schema["name"]])
+            metric_name = ".".join([self.schema["namespace"], self.schema["name"]])
+            full_url = urljoin(base_url, metric_name)
 
-            requests.post(full_url, json=payload, headers=headers)
+            response = requests.post(full_url, json=payload, headers=headers)
+
+            if response.status_code is not 200:
+                print(f"Response status code: {response.status_code}")
+                print(f"Full URL: {full_url}")
+                print(payload)
```

