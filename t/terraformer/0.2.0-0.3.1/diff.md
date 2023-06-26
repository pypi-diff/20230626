# Comparing `tmp/terraformer-0.2.0.tar.gz` & `tmp/terraformer-0.3.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "terraformer-0.2.0.tar", last modified: Sat Feb 25 18:47:43 2023, max compression
+gzip compressed data, was "terraformer-0.3.1.tar", last modified: Mon Jun 26 14:50:47 2023, max compression
```

## Comparing `terraformer-0.2.0.tar` & `terraformer-0.3.1.tar`

### file list

```diff
@@ -1,33 +1,63 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-25 18:47:43.723213 terraformer-0.2.0/
--rw-r--r--   0 runner    (1001) docker     (123)     1097 2023-02-25 18:46:57.000000 terraformer-0.2.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     1661 2023-02-25 18:47:43.723213 terraformer-0.2.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1460 2023-02-25 18:46:57.000000 terraformer-0.2.0/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      532 2023-02-25 18:46:57.000000 terraformer-0.2.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)      653 2023-02-25 18:47:43.723213 terraformer-0.2.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      395 2023-02-25 18:46:57.000000 terraformer-0.2.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-25 18:47:43.723213 terraformer-0.2.0/terraformer/
--rw-r--r--   0 runner    (1001) docker     (123)      360 2023-02-25 18:46:57.000000 terraformer-0.2.0/terraformer/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      497 2023-02-25 18:47:43.723213 terraformer-0.2.0/terraformer/_version.py
--rw-r--r--   0 runner    (1001) docker     (123)     7944 2023-02-25 18:46:57.000000 terraformer-0.2.0/terraformer/apply_log.py
--rw-r--r--   0 runner    (1001) docker     (123)       40 2023-02-25 18:46:57.000000 terraformer-0.2.0/terraformer/authentication.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-25 18:47:43.723213 terraformer-0.2.0/terraformer/conf/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-02-25 18:46:57.000000 terraformer-0.2.0/terraformer/conf/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      128 2023-02-25 18:46:57.000000 terraformer-0.2.0/terraformer/conf/settings.py
--rw-r--r--   0 runner    (1001) docker     (123)      519 2023-02-25 18:46:57.000000 terraformer-0.2.0/terraformer/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (123)     3003 2023-02-25 18:46:57.000000 terraformer-0.2.0/terraformer/mixins.py
--rw-r--r--   0 runner    (1001) docker     (123)     2374 2023-02-25 18:46:57.000000 terraformer-0.2.0/terraformer/plan.py
--rw-r--r--   0 runner    (1001) docker     (123)       26 2023-02-25 18:46:57.000000 terraformer-0.2.0/terraformer/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)       59 2023-02-25 18:46:57.000000 terraformer-0.2.0/terraformer/settings.py
--rw-r--r--   0 runner    (1001) docker     (123)     4777 2023-02-25 18:46:57.000000 terraformer-0.2.0/terraformer/workspace.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-25 18:47:43.723213 terraformer-0.2.0/terraformer.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1661 2023-02-25 18:47:43.000000 terraformer-0.2.0/terraformer.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      628 2023-02-25 18:47:43.000000 terraformer-0.2.0/terraformer.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-02-25 18:47:43.000000 terraformer-0.2.0/terraformer.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      109 2023-02-25 18:47:43.000000 terraformer-0.2.0/terraformer.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       18 2023-02-25 18:47:43.000000 terraformer-0.2.0/terraformer.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-25 18:47:43.723213 terraformer-0.2.0/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-02-25 18:46:57.000000 terraformer-0.2.0/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      774 2023-02-25 18:46:57.000000 terraformer-0.2.0/tests/conftest.py
--rw-r--r--   0 runner    (1001) docker     (123)     1108 2023-02-25 18:46:57.000000 terraformer-0.2.0/tests/test_apply_logs.py
--rw-r--r--   0 runner    (1001) docker     (123)      774 2023-02-25 18:46:57.000000 terraformer-0.2.0/tests/test_plan.py
--rw-r--r--   0 runner    (1001) docker     (123)     2482 2023-02-25 18:46:57.000000 terraformer-0.2.0/tests/test_workspace.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 14:50:47.188364 terraformer-0.3.1/
+-rw-r--r--   0 runner    (1001) docker     (123)       37 2023-06-26 14:50:11.000000 terraformer-0.3.1/.gitattributes
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 14:50:47.180364 terraformer-0.3.1/.github/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 14:50:47.184364 terraformer-0.3.1/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)      363 2023-06-26 14:50:11.000000 terraformer-0.3.1/.github/workflows/black.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      386 2023-06-26 14:50:11.000000 terraformer-0.3.1/.github/workflows/dapperdata.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      361 2023-06-26 14:50:11.000000 terraformer-0.3.1/.github/workflows/isort.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      353 2023-06-26 14:50:11.000000 terraformer-0.3.1/.github/workflows/mypy.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      730 2023-06-26 14:50:11.000000 terraformer-0.3.1/.github/workflows/pypi.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      364 2023-06-26 14:50:11.000000 terraformer-0.3.1/.github/workflows/pytest.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      364 2023-06-26 14:50:11.000000 terraformer-0.3.1/.github/workflows/tomlsort.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     3103 2023-06-26 14:50:11.000000 terraformer-0.3.1/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)        7 2023-06-26 14:50:11.000000 terraformer-0.3.1/.python-version
+-rw-r--r--   0 runner    (1001) docker     (123)     1097 2023-06-26 14:50:11.000000 terraformer-0.3.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     3501 2023-06-26 14:50:47.188364 terraformer-0.3.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1982 2023-06-26 14:50:11.000000 terraformer-0.3.1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 14:50:47.180364 terraformer-0.3.1/docs/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 14:50:47.184364 terraformer-0.3.1/docs/dev/
+-rw-r--r--   0 runner    (1001) docker     (123)      141 2023-06-26 14:50:11.000000 terraformer-0.3.1/docs/dev/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)        9 2023-06-26 14:50:11.000000 terraformer-0.3.1/docs/dev/github.md
+-rw-r--r--   0 runner    (1001) docker     (123)        7 2023-06-26 14:50:11.000000 terraformer-0.3.1/docs/dev/pypi.md
+-rw-r--r--   0 runner    (1001) docker     (123)      284 2023-06-26 14:50:11.000000 terraformer-0.3.1/docs/dev/settings.md
+-rw-r--r--   0 runner    (1001) docker     (123)     2336 2023-06-26 14:50:11.000000 terraformer-0.3.1/makefile
+-rw-r--r--   0 runner    (1001) docker     (123)     1301 2023-06-26 14:50:11.000000 terraformer-0.3.1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-26 14:50:47.188364 terraformer-0.3.1/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 14:50:47.184364 terraformer-0.3.1/terraformer/
+-rw-r--r--   0 runner    (1001) docker     (123)      398 2023-06-26 14:50:11.000000 terraformer-0.3.1/terraformer/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      160 2023-06-26 14:50:47.000000 terraformer-0.3.1/terraformer/_version.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7944 2023-06-26 14:50:11.000000 terraformer-0.3.1/terraformer/apply_log.py
+-rw-r--r--   0 runner    (1001) docker     (123)       40 2023-06-26 14:50:11.000000 terraformer-0.3.1/terraformer/authentication.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 14:50:47.188364 terraformer-0.3.1/terraformer/conf/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-26 14:50:11.000000 terraformer-0.3.1/terraformer/conf/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      255 2023-06-26 14:50:11.000000 terraformer-0.3.1/terraformer/conf/settings.py
+-rw-r--r--   0 runner    (1001) docker     (123)      519 2023-06-26 14:50:11.000000 terraformer-0.3.1/terraformer/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3003 2023-06-26 14:50:11.000000 terraformer-0.3.1/terraformer/mixins.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5108 2023-06-26 14:50:11.000000 terraformer-0.3.1/terraformer/plan.py
+-rw-r--r--   0 runner    (1001) docker     (123)       26 2023-06-26 14:50:11.000000 terraformer-0.3.1/terraformer/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)       59 2023-06-26 14:50:11.000000 terraformer-0.3.1/terraformer/settings.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4777 2023-06-26 14:50:11.000000 terraformer-0.3.1/terraformer/workspace.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 14:50:47.188364 terraformer-0.3.1/terraformer.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     3501 2023-06-26 14:50:47.000000 terraformer-0.3.1/terraformer.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1212 2023-06-26 14:50:47.000000 terraformer-0.3.1/terraformer.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-26 14:50:47.000000 terraformer-0.3.1/terraformer.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      119 2023-06-26 14:50:47.000000 terraformer-0.3.1/terraformer.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       28 2023-06-26 14:50:47.000000 terraformer-0.3.1/terraformer.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 14:50:47.188364 terraformer-0.3.1/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-26 14:50:11.000000 terraformer-0.3.1/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      774 2023-06-26 14:50:11.000000 terraformer-0.3.1/tests/conftest.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 14:50:47.184364 terraformer-0.3.1/tests/terraform/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 14:50:47.188364 terraformer-0.3.1/tests/terraform/applies/
+-rw-r--r--   0 runner    (1001) docker     (123)    59416 2023-06-26 14:50:11.000000 terraformer-0.3.1/tests/terraform/applies/vpc.jsonl
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 14:50:47.188364 terraformer-0.3.1/tests/terraform/destroys/
+-rw-r--r--   0 runner    (1001) docker     (123)    97583 2023-06-26 14:50:11.000000 terraformer-0.3.1/tests/terraform/destroys/vpc.jsonl
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 14:50:47.188364 terraformer-0.3.1/tests/terraform/plans/
+-rw-r--r--   0 runner    (1001) docker     (123)      640 2023-06-26 14:50:11.000000 terraformer-0.3.1/tests/terraform/plans/sensitive_plan.json
+-rw-r--r--   0 runner    (1001) docker     (123)    14906 2023-06-26 14:50:11.000000 terraformer-0.3.1/tests/terraform/plans/test.plan
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 14:50:47.188364 terraformer-0.3.1/tests/terraform/workspace/
+-rw-r--r--   0 runner    (1001) docker     (123)      733 2023-06-26 14:50:11.000000 terraformer-0.3.1/tests/terraform/workspace/main.tf
+-rw-r--r--   0 runner    (1001) docker     (123)       39 2023-06-26 14:50:11.000000 terraformer-0.3.1/tests/terraform/workspace/mock.tfbackend
+-rw-r--r--   0 runner    (1001) docker     (123)       43 2023-06-26 14:50:11.000000 terraformer-0.3.1/tests/terraform/workspace/test.auto.tfvars.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1108 2023-06-26 14:50:11.000000 terraformer-0.3.1/tests/test_apply_logs.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1867 2023-06-26 14:50:11.000000 terraformer-0.3.1/tests/test_plan.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2482 2023-06-26 14:50:11.000000 terraformer-0.3.1/tests/test_workspace.py
```

### Comparing `terraformer-0.2.0/LICENSE` & `terraformer-0.3.1/LICENSE`

 * *Files identical despite different names*

### Comparing `terraformer-0.2.0/PKG-INFO` & `terraformer-0.3.1/README.md`

 * *Files 15% similar despite different names*

```diff
@@ -1,17 +1,7 @@
-Metadata-Version: 2.1
-Name: terraformer
-Version: 0.2.0
-Summary: A python library
-License: MIT
-Requires-Python: >=3.10
-Description-Content-Type: text/markdown
-Provides-Extra: dev
-License-File: LICENSE
-
 # terraformer
 
 terraformer is a Python wrapper around the Terraform CLI.
 
 ## Usage
 
 ### Quick Start
@@ -52,14 +42,28 @@
 from terraformer import Workspace
 
 workspace = Workspace(path="./")
 workspace.init()
 results, apply_log = workspace.apply(auto_approve=True)
 ```
 
+There is also the capability to parse an existing plan JSON and create a plan object with the sensitive and unknown attributes sanitized
+in the output.
+
+```python
+  import json
+
+  plan_from_json = TerraformPlan("", "tests/terraform/plans/sensitive_plan.json", False)
+  for address, resource_change in plan_from_json.changes:
+    print(f"address: {address}\n")
+    print("before:\n")
+    print(json.dumps(resource_change.before_sanitized))
+    print("\nafter:\n")
+    print(json.dumps(resource_change.after_sanitized))
+```
 
 ### Installation
 
 terraformer can be installed with pip.
 
 ```bash
 pip install terraformer
```

### Comparing `terraformer-0.2.0/terraformer/apply_log.py` & `terraformer-0.3.1/terraformer/apply_log.py`

 * *Files identical despite different names*

### Comparing `terraformer-0.2.0/terraformer/exceptions.py` & `terraformer-0.3.1/terraformer/exceptions.py`

 * *Files identical despite different names*

### Comparing `terraformer-0.2.0/terraformer/mixins.py` & `terraformer-0.3.1/terraformer/mixins.py`

 * *Files identical despite different names*

### Comparing `terraformer-0.2.0/terraformer/workspace.py` & `terraformer-0.3.1/terraformer/workspace.py`

 * *Files identical despite different names*

### Comparing `terraformer-0.2.0/tests/conftest.py` & `terraformer-0.3.1/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `terraformer-0.2.0/tests/test_apply_logs.py` & `terraformer-0.3.1/tests/test_apply_logs.py`

 * *Files identical despite different names*

### Comparing `terraformer-0.2.0/tests/test_workspace.py` & `terraformer-0.3.1/tests/test_workspace.py`

 * *Files identical despite different names*

