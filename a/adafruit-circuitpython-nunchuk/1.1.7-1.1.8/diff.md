# Comparing `tmp/adafruit-circuitpython-nunchuk-1.1.7.tar.gz` & `tmp/adafruit-circuitpython-nunchuk-1.1.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "adafruit-circuitpython-nunchuk-1.1.7.tar", last modified: Mon Dec  5 19:10:08 2022, max compression
+gzip compressed data, was "adafruit-circuitpython-nunchuk-1.1.8.tar", last modified: Mon Jun 26 17:58:16 2023, max compression
```

## Comparing `adafruit-circuitpython-nunchuk-1.1.7.tar` & `adafruit-circuitpython-nunchuk-1.1.8.tar`

### file list

```diff
@@ -1,49 +1,49 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-05 19:10:08.154249 adafruit-circuitpython-nunchuk-1.1.7/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-05 19:10:08.146248 adafruit-circuitpython-nunchuk-1.1.7/.github/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-05 19:10:08.150248 adafruit-circuitpython-nunchuk-1.1.7/.github/PULL_REQUEST_TEMPLATE/
--rw-r--r--   0 runner    (1001) docker     (123)      880 2022-12-05 19:09:52.000000 adafruit-circuitpython-nunchuk-1.1.7/.github/PULL_REQUEST_TEMPLATE/adafruit_circuitpython_pr.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-05 19:10:08.150248 adafruit-circuitpython-nunchuk-1.1.7/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)      303 2022-12-05 19:09:52.000000 adafruit-circuitpython-nunchuk-1.1.7/.github/workflows/build.yml
--rw-r--r--   0 runner    (1001) docker     (123)      479 2022-12-05 19:09:52.000000 adafruit-circuitpython-nunchuk-1.1.7/.github/workflows/failure-help-text.yml
--rw-r--r--   0 runner    (1001) docker     (123)      423 2022-12-05 19:09:52.000000 adafruit-circuitpython-nunchuk-1.1.7/.github/workflows/release_gh.yml
--rw-r--r--   0 runner    (1001) docker     (123)      475 2022-12-05 19:09:52.000000 adafruit-circuitpython-nunchuk-1.1.7/.github/workflows/release_pypi.yml
--rw-r--r--   0 runner    (1001) docker     (123)     1654 2022-12-05 19:09:52.000000 adafruit-circuitpython-nunchuk-1.1.7/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)     1239 2022-12-05 19:09:52.000000 adafruit-circuitpython-nunchuk-1.1.7/.pre-commit-config.yaml
--rw-r--r--   0 runner    (1001) docker     (123)    13069 2022-12-05 19:09:52.000000 adafruit-circuitpython-nunchuk-1.1.7/.pylintrc
--rw-r--r--   0 runner    (1001) docker     (123)      388 2022-12-05 19:09:52.000000 adafruit-circuitpython-nunchuk-1.1.7/.readthedocs.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     6147 2022-12-05 19:09:52.000000 adafruit-circuitpython-nunchuk-1.1.7/CODE_OF_CONDUCT.md
--rw-r--r--   0 runner    (1001) docker     (123)     1104 2022-12-05 19:09:52.000000 adafruit-circuitpython-nunchuk-1.1.7/LICENSE
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-05 19:10:08.150248 adafruit-circuitpython-nunchuk-1.1.7/LICENSES/
--rw-r--r--   0 runner    (1001) docker     (123)    16814 2022-12-05 19:09:52.000000 adafruit-circuitpython-nunchuk-1.1.7/LICENSES/CC-BY-4.0.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1108 2022-12-05 19:09:52.000000 adafruit-circuitpython-nunchuk-1.1.7/LICENSES/MIT.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1211 2022-12-05 19:09:52.000000 adafruit-circuitpython-nunchuk-1.1.7/LICENSES/Unlicense.txt
--rw-r--r--   0 runner    (1001) docker     (123)     4113 2022-12-05 19:10:08.154249 adafruit-circuitpython-nunchuk-1.1.7/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     3340 2022-12-05 19:09:52.000000 adafruit-circuitpython-nunchuk-1.1.7/README.rst
--rw-r--r--   0 runner    (1001) docker     (123)      108 2022-12-05 19:09:52.000000 adafruit-circuitpython-nunchuk-1.1.7/README.rst.license
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-05 19:10:08.150248 adafruit-circuitpython-nunchuk-1.1.7/adafruit_circuitpython_nunchuk.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     4113 2022-12-05 19:10:08.000000 adafruit-circuitpython-nunchuk-1.1.7/adafruit_circuitpython_nunchuk.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1029 2022-12-05 19:10:08.000000 adafruit-circuitpython-nunchuk-1.1.7/adafruit_circuitpython_nunchuk.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2022-12-05 19:10:08.000000 adafruit-circuitpython-nunchuk-1.1.7/adafruit_circuitpython_nunchuk.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       61 2022-12-05 19:10:08.000000 adafruit-circuitpython-nunchuk-1.1.7/adafruit_circuitpython_nunchuk.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       17 2022-12-05 19:10:08.000000 adafruit-circuitpython-nunchuk-1.1.7/adafruit_circuitpython_nunchuk.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)     4204 2022-12-05 19:10:00.000000 adafruit-circuitpython-nunchuk-1.1.7/adafruit_nunchuk.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-05 19:10:08.154249 adafruit-circuitpython-nunchuk-1.1.7/docs/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-05 19:10:08.154249 adafruit-circuitpython-nunchuk-1.1.7/docs/_static/
--rw-r--r--   0 runner    (1001) docker     (123)     4414 2022-12-05 19:09:52.000000 adafruit-circuitpython-nunchuk-1.1.7/docs/_static/favicon.ico
--rw-r--r--   0 runner    (1001) docker     (123)      105 2022-12-05 19:09:52.000000 adafruit-circuitpython-nunchuk-1.1.7/docs/_static/favicon.ico.license
--rw-r--r--   0 runner    (1001) docker     (123)      266 2022-12-05 19:09:52.000000 adafruit-circuitpython-nunchuk-1.1.7/docs/api.rst
--rw-r--r--   0 runner    (1001) docker     (123)       96 2022-12-05 19:09:52.000000 adafruit-circuitpython-nunchuk-1.1.7/docs/api.rst.license
--rw-r--r--   0 runner    (1001) docker     (123)     5763 2022-12-05 19:09:52.000000 adafruit-circuitpython-nunchuk-1.1.7/docs/conf.py
--rw-r--r--   0 runner    (1001) docker     (123)      188 2022-12-05 19:09:52.000000 adafruit-circuitpython-nunchuk-1.1.7/docs/examples.rst
--rw-r--r--   0 runner    (1001) docker     (123)       96 2022-12-05 19:09:52.000000 adafruit-circuitpython-nunchuk-1.1.7/docs/examples.rst.license
--rw-r--r--   0 runner    (1001) docker     (123)      972 2022-12-05 19:09:52.000000 adafruit-circuitpython-nunchuk-1.1.7/docs/index.rst
--rw-r--r--   0 runner    (1001) docker     (123)       96 2022-12-05 19:09:52.000000 adafruit-circuitpython-nunchuk-1.1.7/docs/index.rst.license
--rw-r--r--   0 runner    (1001) docker     (123)      123 2022-12-05 19:09:52.000000 adafruit-circuitpython-nunchuk-1.1.7/docs/requirements.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-05 19:10:08.154249 adafruit-circuitpython-nunchuk-1.1.7/examples/
--rw-r--r--   0 runner    (1001) docker     (123)     1717 2022-12-05 19:10:00.000000 adafruit-circuitpython-nunchuk-1.1.7/examples/nunchuk_accel_mouse.py
--rw-r--r--   0 runner    (1001) docker     (123)     1580 2022-12-05 19:10:00.000000 adafruit-circuitpython-nunchuk-1.1.7/examples/nunchuk_analog_mouse.py
--rw-r--r--   0 runner    (1001) docker     (123)      481 2022-12-05 19:10:00.000000 adafruit-circuitpython-nunchuk-1.1.7/examples/nunchuk_simpletest.py
--rw-r--r--   0 runner    (1001) docker     (123)      108 2022-12-05 19:09:52.000000 adafruit-circuitpython-nunchuk-1.1.7/optional_requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1234 2022-12-05 19:10:00.000000 adafruit-circuitpython-nunchuk-1.1.7/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)      158 2022-12-05 19:09:52.000000 adafruit-circuitpython-nunchuk-1.1.7/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2022-12-05 19:10:08.154249 adafruit-circuitpython-nunchuk-1.1.7/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 17:58:16.286054 adafruit-circuitpython-nunchuk-1.1.8/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 17:58:16.278053 adafruit-circuitpython-nunchuk-1.1.8/.github/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 17:58:16.282054 adafruit-circuitpython-nunchuk-1.1.8/.github/PULL_REQUEST_TEMPLATE/
+-rw-r--r--   0 runner    (1001) docker     (123)      880 2023-06-26 17:57:57.000000 adafruit-circuitpython-nunchuk-1.1.8/.github/PULL_REQUEST_TEMPLATE/adafruit_circuitpython_pr.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 17:58:16.282054 adafruit-circuitpython-nunchuk-1.1.8/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)      303 2023-06-26 17:57:57.000000 adafruit-circuitpython-nunchuk-1.1.8/.github/workflows/build.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      479 2023-06-26 17:57:57.000000 adafruit-circuitpython-nunchuk-1.1.8/.github/workflows/failure-help-text.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      482 2023-06-26 17:57:57.000000 adafruit-circuitpython-nunchuk-1.1.8/.github/workflows/release_gh.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      475 2023-06-26 17:57:57.000000 adafruit-circuitpython-nunchuk-1.1.8/.github/workflows/release_pypi.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1654 2023-06-26 17:57:57.000000 adafruit-circuitpython-nunchuk-1.1.8/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)     1238 2023-06-26 17:57:57.000000 adafruit-circuitpython-nunchuk-1.1.8/.pre-commit-config.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)    13078 2023-06-26 17:57:57.000000 adafruit-circuitpython-nunchuk-1.1.8/.pylintrc
+-rw-r--r--   0 runner    (1001) docker     (123)      388 2023-06-26 17:57:57.000000 adafruit-circuitpython-nunchuk-1.1.8/.readthedocs.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     6147 2023-06-26 17:57:57.000000 adafruit-circuitpython-nunchuk-1.1.8/CODE_OF_CONDUCT.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1104 2023-06-26 17:57:57.000000 adafruit-circuitpython-nunchuk-1.1.8/LICENSE
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 17:58:16.282054 adafruit-circuitpython-nunchuk-1.1.8/LICENSES/
+-rw-r--r--   0 runner    (1001) docker     (123)    16814 2023-06-26 17:57:57.000000 adafruit-circuitpython-nunchuk-1.1.8/LICENSES/CC-BY-4.0.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1108 2023-06-26 17:57:57.000000 adafruit-circuitpython-nunchuk-1.1.8/LICENSES/MIT.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1211 2023-06-26 17:57:57.000000 adafruit-circuitpython-nunchuk-1.1.8/LICENSES/Unlicense.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     4113 2023-06-26 17:58:16.286054 adafruit-circuitpython-nunchuk-1.1.8/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3340 2023-06-26 17:57:57.000000 adafruit-circuitpython-nunchuk-1.1.8/README.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      108 2023-06-26 17:57:57.000000 adafruit-circuitpython-nunchuk-1.1.8/README.rst.license
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 17:58:16.282054 adafruit-circuitpython-nunchuk-1.1.8/adafruit_circuitpython_nunchuk.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     4113 2023-06-26 17:58:16.000000 adafruit-circuitpython-nunchuk-1.1.8/adafruit_circuitpython_nunchuk.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1029 2023-06-26 17:58:16.000000 adafruit-circuitpython-nunchuk-1.1.8/adafruit_circuitpython_nunchuk.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-26 17:58:16.000000 adafruit-circuitpython-nunchuk-1.1.8/adafruit_circuitpython_nunchuk.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       61 2023-06-26 17:58:16.000000 adafruit-circuitpython-nunchuk-1.1.8/adafruit_circuitpython_nunchuk.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       17 2023-06-26 17:58:16.000000 adafruit-circuitpython-nunchuk-1.1.8/adafruit_circuitpython_nunchuk.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     4499 2023-06-26 17:58:07.000000 adafruit-circuitpython-nunchuk-1.1.8/adafruit_nunchuk.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 17:58:16.286054 adafruit-circuitpython-nunchuk-1.1.8/docs/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 17:58:16.286054 adafruit-circuitpython-nunchuk-1.1.8/docs/_static/
+-rw-r--r--   0 runner    (1001) docker     (123)     4414 2023-06-26 17:57:57.000000 adafruit-circuitpython-nunchuk-1.1.8/docs/_static/favicon.ico
+-rw-r--r--   0 runner    (1001) docker     (123)      105 2023-06-26 17:57:57.000000 adafruit-circuitpython-nunchuk-1.1.8/docs/_static/favicon.ico.license
+-rw-r--r--   0 runner    (1001) docker     (123)      266 2023-06-26 17:57:57.000000 adafruit-circuitpython-nunchuk-1.1.8/docs/api.rst
+-rw-r--r--   0 runner    (1001) docker     (123)       96 2023-06-26 17:57:57.000000 adafruit-circuitpython-nunchuk-1.1.8/docs/api.rst.license
+-rw-r--r--   0 runner    (1001) docker     (123)     5791 2023-06-26 17:57:57.000000 adafruit-circuitpython-nunchuk-1.1.8/docs/conf.py
+-rw-r--r--   0 runner    (1001) docker     (123)      188 2023-06-26 17:57:57.000000 adafruit-circuitpython-nunchuk-1.1.8/docs/examples.rst
+-rw-r--r--   0 runner    (1001) docker     (123)       96 2023-06-26 17:57:57.000000 adafruit-circuitpython-nunchuk-1.1.8/docs/examples.rst.license
+-rw-r--r--   0 runner    (1001) docker     (123)      972 2023-06-26 17:57:57.000000 adafruit-circuitpython-nunchuk-1.1.8/docs/index.rst
+-rw-r--r--   0 runner    (1001) docker     (123)       96 2023-06-26 17:57:57.000000 adafruit-circuitpython-nunchuk-1.1.8/docs/index.rst.license
+-rw-r--r--   0 runner    (1001) docker     (123)      144 2023-06-26 17:57:57.000000 adafruit-circuitpython-nunchuk-1.1.8/docs/requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 17:58:16.286054 adafruit-circuitpython-nunchuk-1.1.8/examples/
+-rw-r--r--   0 runner    (1001) docker     (123)     1716 2023-06-26 17:58:07.000000 adafruit-circuitpython-nunchuk-1.1.8/examples/nunchuk_accel_mouse.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1579 2023-06-26 17:58:07.000000 adafruit-circuitpython-nunchuk-1.1.8/examples/nunchuk_analog_mouse.py
+-rw-r--r--   0 runner    (1001) docker     (123)      481 2023-06-26 17:58:07.000000 adafruit-circuitpython-nunchuk-1.1.8/examples/nunchuk_simpletest.py
+-rw-r--r--   0 runner    (1001) docker     (123)      108 2023-06-26 17:57:57.000000 adafruit-circuitpython-nunchuk-1.1.8/optional_requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1234 2023-06-26 17:58:07.000000 adafruit-circuitpython-nunchuk-1.1.8/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      158 2023-06-26 17:57:57.000000 adafruit-circuitpython-nunchuk-1.1.8/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-26 17:58:16.286054 adafruit-circuitpython-nunchuk-1.1.8/setup.cfg
```

### Comparing `adafruit-circuitpython-nunchuk-1.1.7/.github/PULL_REQUEST_TEMPLATE/adafruit_circuitpython_pr.md` & `adafruit-circuitpython-nunchuk-1.1.8/.github/PULL_REQUEST_TEMPLATE/adafruit_circuitpython_pr.md`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-nunchuk-1.1.7/.gitignore` & `adafruit-circuitpython-nunchuk-1.1.8/.gitignore`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-nunchuk-1.1.7/.pre-commit-config.yaml` & `adafruit-circuitpython-nunchuk-1.1.8/.pre-commit-config.yaml`

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

### Comparing `adafruit-circuitpython-nunchuk-1.1.7/.pylintrc` & `adafruit-circuitpython-nunchuk-1.1.8/.pylintrc`

 * *Files 1% similar despite different names*

```diff
@@ -392,8 +392,8 @@
 min-public-methods=1
 
 
 [EXCEPTIONS]
 
 # Exceptions that will emit a warning when being caught. Defaults to
 # "Exception"
-overgeneral-exceptions=Exception
+overgeneral-exceptions=builtins.Exception
```

### Comparing `adafruit-circuitpython-nunchuk-1.1.7/CODE_OF_CONDUCT.md` & `adafruit-circuitpython-nunchuk-1.1.8/CODE_OF_CONDUCT.md`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-nunchuk-1.1.7/LICENSE` & `adafruit-circuitpython-nunchuk-1.1.8/LICENSE`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-nunchuk-1.1.7/LICENSES/CC-BY-4.0.txt` & `adafruit-circuitpython-nunchuk-1.1.8/LICENSES/CC-BY-4.0.txt`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-nunchuk-1.1.7/LICENSES/MIT.txt` & `adafruit-circuitpython-nunchuk-1.1.8/LICENSES/MIT.txt`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-nunchuk-1.1.7/LICENSES/Unlicense.txt` & `adafruit-circuitpython-nunchuk-1.1.8/LICENSES/Unlicense.txt`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-nunchuk-1.1.7/PKG-INFO` & `adafruit-circuitpython-nunchuk-1.1.8/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: adafruit-circuitpython-nunchuk
-Version: 1.1.7
+Version: 1.1.8
 Summary: CircuitPython library for Nintendo Nunchuk controller
 Author-email: Adafruit Industries <circuitpython@adafruit.com>
 License: MIT
 Project-URL: Homepage, https://github.com/adafruit/Adafruit_CircuitPython_Nunchuk.git
 Keywords: adafruit,blinka,circuitpython,micropython,nunchuk,nunchuck,nintendo,controller
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Software Development :: Libraries
```

### Comparing `adafruit-circuitpython-nunchuk-1.1.7/README.rst` & `adafruit-circuitpython-nunchuk-1.1.8/README.rst`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-nunchuk-1.1.7/adafruit_circuitpython_nunchuk.egg-info/PKG-INFO` & `adafruit-circuitpython-nunchuk-1.1.8/adafruit_circuitpython_nunchuk.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: adafruit-circuitpython-nunchuk
-Version: 1.1.7
+Version: 1.1.8
 Summary: CircuitPython library for Nintendo Nunchuk controller
 Author-email: Adafruit Industries <circuitpython@adafruit.com>
 License: MIT
 Project-URL: Homepage, https://github.com/adafruit/Adafruit_CircuitPython_Nunchuk.git
 Keywords: adafruit,blinka,circuitpython,micropython,nunchuk,nunchuck,nintendo,controller
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Software Development :: Libraries
```

### Comparing `adafruit-circuitpython-nunchuk-1.1.7/adafruit_circuitpython_nunchuk.egg-info/SOURCES.txt` & `adafruit-circuitpython-nunchuk-1.1.8/adafruit_circuitpython_nunchuk.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-nunchuk-1.1.7/adafruit_nunchuk.py` & `adafruit-circuitpython-nunchuk-1.1.8/adafruit_nunchuk.py`

 * *Files 5% similar despite different names*

```diff
@@ -31,15 +31,15 @@
 
 try:
     import typing  # pylint: disable=unused-import
     from busio import I2C
 except ImportError:
     pass
 
-__version__ = "1.1.7"
+__version__ = "1.1.8"
 __repo__ = "https://github.com/adafruit/Adafruit_CircuitPython_Nunchuk.git"
 
 _I2C_INIT_DELAY = 0.1
 
 
 class Nunchuk:
     """Class which provides interface to Nintendo Nunchuk controller.
@@ -57,14 +57,21 @@
     _Buttons = namedtuple("Buttons", ("C", "Z"))
     _Acceleration = namedtuple("Acceleration", ("x", "y", "z"))
 
     def __init__(
         self, i2c: I2C, address: int = 0x52, i2c_read_delay: float = 0.002
     ) -> None:
         self.buffer = bytearray(8)
+        # -| HACK |---------------------------------------------------
+        # fixes quirk with RP2040 + 3rd party controllers
+        while not i2c.try_lock():
+            pass
+        _ = i2c.scan()
+        i2c.unlock()
+        # ------------------------------------------------------------
         self.i2c_device = I2CDevice(i2c, address)
         self._i2c_read_delay = i2c_read_delay
         time.sleep(_I2C_INIT_DELAY)
         with self.i2c_device as i2c_dev:
             # turn off encrypted data
             # http://wiibrew.org/wiki/Wiimote/Extension_Controllers
             i2c_dev.write(b"\xF0\x55")
```

### Comparing `adafruit-circuitpython-nunchuk-1.1.7/docs/_static/favicon.ico` & `adafruit-circuitpython-nunchuk-1.1.8/docs/_static/favicon.ico`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-nunchuk-1.1.7/docs/conf.py` & `adafruit-circuitpython-nunchuk-1.1.8/docs/conf.py`

 * *Files 1% similar despite different names*

```diff
@@ -13,14 +13,15 @@
 # -- General configuration ------------------------------------------------
 
 # Add any Sphinx extension module names here, as strings. They can be
 # extensions coming with Sphinx (named 'sphinx.ext.*') or your custom
 # ones.
 extensions = [
     "sphinx.ext.autodoc",
+    "sphinxcontrib.jquery",
     "sphinx.ext.intersphinx",
     "sphinx.ext.napoleon",
     "sphinx.ext.todo",
 ]
 
 # TODO: Please Read!
 # Uncomment the below if you use native CircuitPython modules such as
```

### Comparing `adafruit-circuitpython-nunchuk-1.1.7/docs/index.rst` & `adafruit-circuitpython-nunchuk-1.1.8/docs/index.rst`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-nunchuk-1.1.7/examples/nunchuk_accel_mouse.py` & `adafruit-circuitpython-nunchuk-1.1.8/examples/nunchuk_accel_mouse.py`

 * *Files 1% similar despite different names*

```diff
@@ -23,15 +23,14 @@
 
 
 # This is just to show that we're getting back data - uncomment it and hold down the buttons
 # while True:
 #    print((0 if nc.button_C else 1, 0 if nc.button_Z else 1))
 
 while True:
-
     accel = nc.acceleration
     #    print(accel)
     #    x, y = nc.joystick
     #    print((x,y))
     x = accel[0] / 4
     y = accel[1] / 4
     print((x, y))
```

### Comparing `adafruit-circuitpython-nunchuk-1.1.7/examples/nunchuk_analog_mouse.py` & `adafruit-circuitpython-nunchuk-1.1.8/examples/nunchuk_analog_mouse.py`

 * *Files 0% similar despite different names*

```diff
@@ -23,15 +23,14 @@
 
 
 # This is just to show that we're getting back data - uncomment it and hold down the buttons
 # while True:
 #    print((0 if nc.button_C else 1, 0 if nc.button_Z else 1))
 
 while True:
-
     x, y = nc.joystick
     # Eliminate spurious reads
     if x == 255 or y == 255:
         continue
     relX = x - centerX
     relY = centerY - y
```

### Comparing `adafruit-circuitpython-nunchuk-1.1.7/pyproject.toml` & `adafruit-circuitpython-nunchuk-1.1.8/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -8,15 +8,15 @@
     "wheel",
     "setuptools-scm",
 ]
 
 [project]
 name = "adafruit-circuitpython-nunchuk"
 description = "CircuitPython library for Nintendo Nunchuk controller"
-version = "1.1.7"
+version = "1.1.8"
 readme = "README.rst"
 authors = [
     {name = "Adafruit Industries", email = "circuitpython@adafruit.com"}
 ]
 urls = {Homepage = "https://github.com/adafruit/Adafruit_CircuitPython_Nunchuk.git"}
 keywords = [
     "adafruit",
```

