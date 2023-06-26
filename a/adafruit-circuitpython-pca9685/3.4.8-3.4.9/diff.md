# Comparing `tmp/adafruit-circuitpython-pca9685-3.4.8.tar.gz` & `tmp/adafruit-circuitpython-pca9685-3.4.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "adafruit-circuitpython-pca9685-3.4.8.tar", last modified: Tue Feb 14 23:25:40 2023, max compression
+gzip compressed data, was "adafruit-circuitpython-pca9685-3.4.9.tar", last modified: Thu May 18 15:39:34 2023, max compression
```

## Comparing `adafruit-circuitpython-pca9685-3.4.8.tar` & `adafruit-circuitpython-pca9685-3.4.9.tar`

### file list

```diff
@@ -1,49 +1,49 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-14 23:25:40.111663 adafruit-circuitpython-pca9685-3.4.8/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-14 23:25:40.107663 adafruit-circuitpython-pca9685-3.4.8/.github/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-14 23:25:40.107663 adafruit-circuitpython-pca9685-3.4.8/.github/PULL_REQUEST_TEMPLATE/
--rw-r--r--   0 runner    (1001) docker     (123)      880 2023-02-14 23:25:23.000000 adafruit-circuitpython-pca9685-3.4.8/.github/PULL_REQUEST_TEMPLATE/adafruit_circuitpython_pr.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-14 23:25:40.107663 adafruit-circuitpython-pca9685-3.4.8/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)      303 2023-02-14 23:25:23.000000 adafruit-circuitpython-pca9685-3.4.8/.github/workflows/build.yml
--rw-r--r--   0 runner    (1001) docker     (123)      479 2023-02-14 23:25:23.000000 adafruit-circuitpython-pca9685-3.4.8/.github/workflows/failure-help-text.yml
--rw-r--r--   0 runner    (1001) docker     (123)      482 2023-02-14 23:25:23.000000 adafruit-circuitpython-pca9685-3.4.8/.github/workflows/release_gh.yml
--rw-r--r--   0 runner    (1001) docker     (123)      475 2023-02-14 23:25:23.000000 adafruit-circuitpython-pca9685-3.4.8/.github/workflows/release_pypi.yml
--rw-r--r--   0 runner    (1001) docker     (123)     1654 2023-02-14 23:25:23.000000 adafruit-circuitpython-pca9685-3.4.8/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)     1239 2023-02-14 23:25:23.000000 adafruit-circuitpython-pca9685-3.4.8/.pre-commit-config.yaml
--rw-r--r--   0 runner    (1001) docker     (123)    13069 2023-02-14 23:25:23.000000 adafruit-circuitpython-pca9685-3.4.8/.pylintrc
--rw-r--r--   0 runner    (1001) docker     (123)      388 2023-02-14 23:25:23.000000 adafruit-circuitpython-pca9685-3.4.8/.readthedocs.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     6147 2023-02-14 23:25:23.000000 adafruit-circuitpython-pca9685-3.4.8/CODE_OF_CONDUCT.md
--rw-r--r--   0 runner    (1001) docker     (123)     1119 2023-02-14 23:25:23.000000 adafruit-circuitpython-pca9685-3.4.8/LICENSE
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-14 23:25:40.111663 adafruit-circuitpython-pca9685-3.4.8/LICENSES/
--rw-r--r--   0 runner    (1001) docker     (123)    16814 2023-02-14 23:25:23.000000 adafruit-circuitpython-pca9685-3.4.8/LICENSES/CC-BY-4.0.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1108 2023-02-14 23:25:23.000000 adafruit-circuitpython-pca9685-3.4.8/LICENSES/MIT.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1211 2023-02-14 23:25:23.000000 adafruit-circuitpython-pca9685-3.4.8/LICENSES/Unlicense.txt
--rw-r--r--   0 runner    (1001) docker     (123)     3449 2023-02-14 23:25:40.111663 adafruit-circuitpython-pca9685-3.4.8/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2672 2023-02-14 23:25:23.000000 adafruit-circuitpython-pca9685-3.4.8/README.rst
--rw-r--r--   0 runner    (1001) docker     (123)      108 2023-02-14 23:25:23.000000 adafruit-circuitpython-pca9685-3.4.8/README.rst.license
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-14 23:25:40.111663 adafruit-circuitpython-pca9685-3.4.8/adafruit_circuitpython_pca9685.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     3449 2023-02-14 23:25:40.000000 adafruit-circuitpython-pca9685-3.4.8/adafruit_circuitpython_pca9685.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1022 2023-02-14 23:25:40.000000 adafruit-circuitpython-pca9685-3.4.8/adafruit_circuitpython_pca9685.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-02-14 23:25:40.000000 adafruit-circuitpython-pca9685-3.4.8/adafruit_circuitpython_pca9685.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       93 2023-02-14 23:25:40.000000 adafruit-circuitpython-pca9685-3.4.8/adafruit_circuitpython_pca9685.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       17 2023-02-14 23:25:40.000000 adafruit-circuitpython-pca9685-3.4.8/adafruit_circuitpython_pca9685.egg-info/top_level.txt
--rwxr-xr-x   0 runner    (1001) docker     (123)     6466 2023-02-14 23:25:32.000000 adafruit-circuitpython-pca9685-3.4.8/adafruit_pca9685.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-14 23:25:40.111663 adafruit-circuitpython-pca9685-3.4.8/docs/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-14 23:25:40.111663 adafruit-circuitpython-pca9685-3.4.8/docs/_static/
--rw-r--r--   0 runner    (1001) docker     (123)     4414 2023-02-14 23:25:23.000000 adafruit-circuitpython-pca9685-3.4.8/docs/_static/favicon.ico
--rw-r--r--   0 runner    (1001) docker     (123)      105 2023-02-14 23:25:23.000000 adafruit-circuitpython-pca9685-3.4.8/docs/_static/favicon.ico.license
--rw-r--r--   0 runner    (1001) docker     (123)      126 2023-02-14 23:25:23.000000 adafruit-circuitpython-pca9685-3.4.8/docs/api.rst
--rw-r--r--   0 runner    (1001) docker     (123)       96 2023-02-14 23:25:23.000000 adafruit-circuitpython-pca9685-3.4.8/docs/api.rst.license
--rw-r--r--   0 runner    (1001) docker     (123)     5591 2023-02-14 23:25:23.000000 adafruit-circuitpython-pca9685-3.4.8/docs/conf.py
--rw-r--r--   0 runner    (1001) docker     (123)      716 2023-02-14 23:25:23.000000 adafruit-circuitpython-pca9685-3.4.8/docs/examples.rst
--rw-r--r--   0 runner    (1001) docker     (123)       96 2023-02-14 23:25:23.000000 adafruit-circuitpython-pca9685-3.4.8/docs/examples.rst.license
--rw-r--r--   0 runner    (1001) docker     (123)     1086 2023-02-14 23:25:23.000000 adafruit-circuitpython-pca9685-3.4.8/docs/index.rst
--rw-r--r--   0 runner    (1001) docker     (123)       96 2023-02-14 23:25:23.000000 adafruit-circuitpython-pca9685-3.4.8/docs/index.rst.license
--rw-r--r--   0 runner    (1001) docker     (123)      123 2023-02-14 23:25:23.000000 adafruit-circuitpython-pca9685-3.4.8/docs/requirements.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-14 23:25:40.111663 adafruit-circuitpython-pca9685-3.4.8/examples/
--rw-r--r--   0 runner    (1001) docker     (123)     1703 2023-02-14 23:25:32.000000 adafruit-circuitpython-pca9685-3.4.8/examples/pca9685_calibration.py
--rw-r--r--   0 runner    (1001) docker     (123)     2404 2023-02-14 23:25:32.000000 adafruit-circuitpython-pca9685-3.4.8/examples/pca9685_servo.py
--rw-r--r--   0 runner    (1001) docker     (123)      774 2023-02-14 23:25:32.000000 adafruit-circuitpython-pca9685-3.4.8/examples/pca9685_simpletest.py
--rw-r--r--   0 runner    (1001) docker     (123)      108 2023-02-14 23:25:23.000000 adafruit-circuitpython-pca9685-3.4.8/optional_requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1238 2023-02-14 23:25:32.000000 adafruit-circuitpython-pca9685-3.4.8/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)      190 2023-02-14 23:25:23.000000 adafruit-circuitpython-pca9685-3.4.8/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-02-14 23:25:40.111663 adafruit-circuitpython-pca9685-3.4.8/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 15:39:34.887743 adafruit-circuitpython-pca9685-3.4.9/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 15:39:34.883743 adafruit-circuitpython-pca9685-3.4.9/.github/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 15:39:34.883743 adafruit-circuitpython-pca9685-3.4.9/.github/PULL_REQUEST_TEMPLATE/
+-rw-r--r--   0 runner    (1001) docker     (123)      880 2023-05-18 15:39:15.000000 adafruit-circuitpython-pca9685-3.4.9/.github/PULL_REQUEST_TEMPLATE/adafruit_circuitpython_pr.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 15:39:34.887743 adafruit-circuitpython-pca9685-3.4.9/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)      303 2023-05-18 15:39:15.000000 adafruit-circuitpython-pca9685-3.4.9/.github/workflows/build.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      479 2023-05-18 15:39:15.000000 adafruit-circuitpython-pca9685-3.4.9/.github/workflows/failure-help-text.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      482 2023-05-18 15:39:15.000000 adafruit-circuitpython-pca9685-3.4.9/.github/workflows/release_gh.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      475 2023-05-18 15:39:15.000000 adafruit-circuitpython-pca9685-3.4.9/.github/workflows/release_pypi.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1654 2023-05-18 15:39:15.000000 adafruit-circuitpython-pca9685-3.4.9/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)     1238 2023-05-18 15:39:15.000000 adafruit-circuitpython-pca9685-3.4.9/.pre-commit-config.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)    13069 2023-05-18 15:39:15.000000 adafruit-circuitpython-pca9685-3.4.9/.pylintrc
+-rw-r--r--   0 runner    (1001) docker     (123)      388 2023-05-18 15:39:15.000000 adafruit-circuitpython-pca9685-3.4.9/.readthedocs.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     6147 2023-05-18 15:39:15.000000 adafruit-circuitpython-pca9685-3.4.9/CODE_OF_CONDUCT.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1119 2023-05-18 15:39:15.000000 adafruit-circuitpython-pca9685-3.4.9/LICENSE
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 15:39:34.887743 adafruit-circuitpython-pca9685-3.4.9/LICENSES/
+-rw-r--r--   0 runner    (1001) docker     (123)    16814 2023-05-18 15:39:15.000000 adafruit-circuitpython-pca9685-3.4.9/LICENSES/CC-BY-4.0.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1108 2023-05-18 15:39:15.000000 adafruit-circuitpython-pca9685-3.4.9/LICENSES/MIT.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1211 2023-05-18 15:39:15.000000 adafruit-circuitpython-pca9685-3.4.9/LICENSES/Unlicense.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     3449 2023-05-18 15:39:34.887743 adafruit-circuitpython-pca9685-3.4.9/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2672 2023-05-18 15:39:15.000000 adafruit-circuitpython-pca9685-3.4.9/README.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      108 2023-05-18 15:39:15.000000 adafruit-circuitpython-pca9685-3.4.9/README.rst.license
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 15:39:34.887743 adafruit-circuitpython-pca9685-3.4.9/adafruit_circuitpython_pca9685.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     3449 2023-05-18 15:39:34.000000 adafruit-circuitpython-pca9685-3.4.9/adafruit_circuitpython_pca9685.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1022 2023-05-18 15:39:34.000000 adafruit-circuitpython-pca9685-3.4.9/adafruit_circuitpython_pca9685.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-18 15:39:34.000000 adafruit-circuitpython-pca9685-3.4.9/adafruit_circuitpython_pca9685.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       93 2023-05-18 15:39:34.000000 adafruit-circuitpython-pca9685-3.4.9/adafruit_circuitpython_pca9685.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       17 2023-05-18 15:39:34.000000 adafruit-circuitpython-pca9685-3.4.9/adafruit_circuitpython_pca9685.egg-info/top_level.txt
+-rwxr-xr-x   0 runner    (1001) docker     (123)     6475 2023-05-18 15:39:26.000000 adafruit-circuitpython-pca9685-3.4.9/adafruit_pca9685.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 15:39:34.887743 adafruit-circuitpython-pca9685-3.4.9/docs/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 15:39:34.887743 adafruit-circuitpython-pca9685-3.4.9/docs/_static/
+-rw-r--r--   0 runner    (1001) docker     (123)     4414 2023-05-18 15:39:15.000000 adafruit-circuitpython-pca9685-3.4.9/docs/_static/favicon.ico
+-rw-r--r--   0 runner    (1001) docker     (123)      105 2023-05-18 15:39:15.000000 adafruit-circuitpython-pca9685-3.4.9/docs/_static/favicon.ico.license
+-rw-r--r--   0 runner    (1001) docker     (123)      126 2023-05-18 15:39:15.000000 adafruit-circuitpython-pca9685-3.4.9/docs/api.rst
+-rw-r--r--   0 runner    (1001) docker     (123)       96 2023-05-18 15:39:15.000000 adafruit-circuitpython-pca9685-3.4.9/docs/api.rst.license
+-rw-r--r--   0 runner    (1001) docker     (123)     5591 2023-05-18 15:39:15.000000 adafruit-circuitpython-pca9685-3.4.9/docs/conf.py
+-rw-r--r--   0 runner    (1001) docker     (123)      716 2023-05-18 15:39:15.000000 adafruit-circuitpython-pca9685-3.4.9/docs/examples.rst
+-rw-r--r--   0 runner    (1001) docker     (123)       96 2023-05-18 15:39:15.000000 adafruit-circuitpython-pca9685-3.4.9/docs/examples.rst.license
+-rw-r--r--   0 runner    (1001) docker     (123)     1086 2023-05-18 15:39:15.000000 adafruit-circuitpython-pca9685-3.4.9/docs/index.rst
+-rw-r--r--   0 runner    (1001) docker     (123)       96 2023-05-18 15:39:15.000000 adafruit-circuitpython-pca9685-3.4.9/docs/index.rst.license
+-rw-r--r--   0 runner    (1001) docker     (123)      123 2023-05-18 15:39:15.000000 adafruit-circuitpython-pca9685-3.4.9/docs/requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 15:39:34.887743 adafruit-circuitpython-pca9685-3.4.9/examples/
+-rw-r--r--   0 runner    (1001) docker     (123)     1703 2023-05-18 15:39:26.000000 adafruit-circuitpython-pca9685-3.4.9/examples/pca9685_calibration.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2404 2023-05-18 15:39:26.000000 adafruit-circuitpython-pca9685-3.4.9/examples/pca9685_servo.py
+-rw-r--r--   0 runner    (1001) docker     (123)      774 2023-05-18 15:39:26.000000 adafruit-circuitpython-pca9685-3.4.9/examples/pca9685_simpletest.py
+-rw-r--r--   0 runner    (1001) docker     (123)      108 2023-05-18 15:39:15.000000 adafruit-circuitpython-pca9685-3.4.9/optional_requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1238 2023-05-18 15:39:26.000000 adafruit-circuitpython-pca9685-3.4.9/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      190 2023-05-18 15:39:15.000000 adafruit-circuitpython-pca9685-3.4.9/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-18 15:39:34.887743 adafruit-circuitpython-pca9685-3.4.9/setup.cfg
```

### Comparing `adafruit-circuitpython-pca9685-3.4.8/.github/PULL_REQUEST_TEMPLATE/adafruit_circuitpython_pr.md` & `adafruit-circuitpython-pca9685-3.4.9/.github/PULL_REQUEST_TEMPLATE/adafruit_circuitpython_pr.md`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-pca9685-3.4.8/.gitignore` & `adafruit-circuitpython-pca9685-3.4.9/.gitignore`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-pca9685-3.4.8/.pre-commit-config.yaml` & `adafruit-circuitpython-pca9685-3.4.9/.pre-commit-config.yaml`

 * *Files 3% similar despite different names*

```diff
@@ -1,28 +1,28 @@
 # SPDX-FileCopyrightText: 2020 Diego Elio Pettenò
 #
 # SPDX-License-Identifier: Unlicense
 
 repos:
   - repo: https://github.com/python/black
-    rev: 22.3.0
+    rev: 23.3.0
     hooks:
       - id: black
   - repo: https://github.com/fsfe/reuse-tool
-    rev: v0.14.0
+    rev: v1.1.2
     hooks:
       - id: reuse
   - repo: https://github.com/pre-commit/pre-commit-hooks
-    rev: v4.2.0
+    rev: v4.4.0
     hooks:
       - id: check-yaml
       - id: end-of-file-fixer
       - id: trailing-whitespace
   - repo: https://github.com/pycqa/pylint
-    rev: v2.15.5
+    rev: v2.17.4
     hooks:
       - id: pylint
         name: pylint (library code)
         types: [python]
         args:
           - --disable=consider-using-f-string
         exclude: "^(docs/|examples/|tests/|setup.py$)"
```

### Comparing `adafruit-circuitpython-pca9685-3.4.8/.pylintrc` & `adafruit-circuitpython-pca9685-3.4.9/.pylintrc`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-pca9685-3.4.8/CODE_OF_CONDUCT.md` & `adafruit-circuitpython-pca9685-3.4.9/CODE_OF_CONDUCT.md`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-pca9685-3.4.8/LICENSE` & `adafruit-circuitpython-pca9685-3.4.9/LICENSE`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-pca9685-3.4.8/LICENSES/CC-BY-4.0.txt` & `adafruit-circuitpython-pca9685-3.4.9/LICENSES/CC-BY-4.0.txt`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-pca9685-3.4.8/LICENSES/MIT.txt` & `adafruit-circuitpython-pca9685-3.4.9/LICENSES/MIT.txt`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-pca9685-3.4.8/LICENSES/Unlicense.txt` & `adafruit-circuitpython-pca9685-3.4.9/LICENSES/Unlicense.txt`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-pca9685-3.4.8/PKG-INFO` & `adafruit-circuitpython-pca9685-3.4.9/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: adafruit-circuitpython-pca9685
-Version: 3.4.8
+Version: 3.4.9
 Summary: CircuitPython driver for motor, stepper, and servo based on PCA9685.
 Author-email: Adafruit Industries <circuitpython@adafruit.com>
 License: MIT
 Project-URL: Homepage, https://github.com/adafruit/Adafruit_CircuitPython_PCA9685
 Keywords: adafruit,pca9685,motor,stepper,servo,hardware,micropython,circuitpython
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Software Development :: Libraries
```

### Comparing `adafruit-circuitpython-pca9685-3.4.8/README.rst` & `adafruit-circuitpython-pca9685-3.4.9/README.rst`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-pca9685-3.4.8/adafruit_circuitpython_pca9685.egg-info/PKG-INFO` & `adafruit-circuitpython-pca9685-3.4.9/adafruit_circuitpython_pca9685.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: adafruit-circuitpython-pca9685
-Version: 3.4.8
+Version: 3.4.9
 Summary: CircuitPython driver for motor, stepper, and servo based on PCA9685.
 Author-email: Adafruit Industries <circuitpython@adafruit.com>
 License: MIT
 Project-URL: Homepage, https://github.com/adafruit/Adafruit_CircuitPython_PCA9685
 Keywords: adafruit,pca9685,motor,stepper,servo,hardware,micropython,circuitpython
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Software Development :: Libraries
```

### Comparing `adafruit-circuitpython-pca9685-3.4.8/adafruit_circuitpython_pca9685.egg-info/SOURCES.txt` & `adafruit-circuitpython-pca9685-3.4.9/adafruit_circuitpython_pca9685.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-pca9685-3.4.8/adafruit_pca9685.py` & `adafruit-circuitpython-pca9685-3.4.9/adafruit_pca9685.py`

 * *Files 1% similar despite different names*

```diff
@@ -27,15 +27,15 @@
 
 * Adafruit CircuitPython firmware for the ESP8622 and M0-based boards:
   https://github.com/adafruit/circuitpython/releases
 * Adafruit's Bus Device library: https://github.com/adafruit/Adafruit_CircuitPython_BusDevice
 * Adafruit's Register library: https://github.com/adafruit/Adafruit_CircuitPython_Register
 """
 
-__version__ = "3.4.8"
+__version__ = "3.4.9"
 __repo__ = "https://github.com/adafruit/Adafruit_CircuitPython_PCA9685.git"
 
 import time
 
 from adafruit_register.i2c_struct import UnaryStruct
 from adafruit_register.i2c_struct_array import StructArray
 from adafruit_bus_device import i2c_device
@@ -69,15 +69,16 @@
     @frequency.setter
     def frequency(self, _):
         raise NotImplementedError("frequency cannot be set on individual channels")
 
     @property
     def duty_cycle(self) -> int:
         """16 bit value that dictates how much of one cycle is high (1) versus low (0). 0xffff will
-        always be high, 0 will always be low and 0x7fff will be half high and then half low."""
+        always be high, 0 will always be low and 0x7fff will be half high and then half low.
+        """
         pwm = self._pca.pwm_regs[self._index]
         if pwm[0] == 0x1000:
             return 0xFFFF
         return pwm[1] << 4
 
     @duty_cycle.setter
     def duty_cycle(self, value: int) -> None:
```

### Comparing `adafruit-circuitpython-pca9685-3.4.8/docs/_static/favicon.ico` & `adafruit-circuitpython-pca9685-3.4.9/docs/_static/favicon.ico`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-pca9685-3.4.8/docs/conf.py` & `adafruit-circuitpython-pca9685-3.4.9/docs/conf.py`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-pca9685-3.4.8/docs/examples.rst` & `adafruit-circuitpython-pca9685-3.4.9/docs/examples.rst`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-pca9685-3.4.8/docs/index.rst` & `adafruit-circuitpython-pca9685-3.4.9/docs/index.rst`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-pca9685-3.4.8/examples/pca9685_calibration.py` & `adafruit-circuitpython-pca9685-3.4.9/examples/pca9685_calibration.py`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-pca9685-3.4.8/examples/pca9685_servo.py` & `adafruit-circuitpython-pca9685-3.4.9/examples/pca9685_servo.py`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-pca9685-3.4.8/examples/pca9685_simpletest.py` & `adafruit-circuitpython-pca9685-3.4.9/examples/pca9685_simpletest.py`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-pca9685-3.4.8/pyproject.toml` & `adafruit-circuitpython-pca9685-3.4.9/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -8,15 +8,15 @@
     "wheel",
     "setuptools-scm",
 ]
 
 [project]
 name = "adafruit-circuitpython-pca9685"
 description = "CircuitPython driver for motor, stepper, and servo based on PCA9685."
-version = "3.4.8"
+version = "3.4.9"
 readme = "README.rst"
 authors = [
     {name = "Adafruit Industries", email = "circuitpython@adafruit.com"}
 ]
 urls = {Homepage = "https://github.com/adafruit/Adafruit_CircuitPython_PCA9685"}
 keywords = [
     "adafruit",
```

