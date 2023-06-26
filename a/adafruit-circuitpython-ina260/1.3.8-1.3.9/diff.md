# Comparing `tmp/adafruit-circuitpython-ina260-1.3.8.tar.gz` & `tmp/adafruit-circuitpython-ina260-1.3.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "adafruit-circuitpython-ina260-1.3.8.tar", last modified: Mon Aug 22 18:41:08 2022, max compression
+gzip compressed data, was "adafruit-circuitpython-ina260-1.3.9.tar", last modified: Fri Aug 26 02:21:35 2022, max compression
```

## Comparing `adafruit-circuitpython-ina260-1.3.8.tar` & `adafruit-circuitpython-ina260-1.3.9.tar`

### file list

```diff
@@ -1,49 +1,49 @@
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-22 18:41:08.610823 adafruit-circuitpython-ina260-1.3.8/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-22 18:41:08.606824 adafruit-circuitpython-ina260-1.3.8/.github/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-22 18:41:08.610823 adafruit-circuitpython-ina260-1.3.8/.github/PULL_REQUEST_TEMPLATE/
--rw-r--r--   0 runner    (1001) docker     (121)      880 2022-08-22 18:40:50.000000 adafruit-circuitpython-ina260-1.3.8/.github/PULL_REQUEST_TEMPLATE/adafruit_circuitpython_pr.md
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-22 18:41:08.610823 adafruit-circuitpython-ina260-1.3.8/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (121)     2535 2022-08-22 18:40:50.000000 adafruit-circuitpython-ina260-1.3.8/.github/workflows/build.yml
--rw-r--r--   0 runner    (1001) docker     (121)      479 2022-08-22 18:40:50.000000 adafruit-circuitpython-ina260-1.3.8/.github/workflows/failure-help-text.yml
--rw-r--r--   0 runner    (1001) docker     (121)     2966 2022-08-22 18:40:50.000000 adafruit-circuitpython-ina260-1.3.8/.github/workflows/release.yml
--rw-r--r--   0 runner    (1001) docker     (121)     1648 2022-08-22 18:40:50.000000 adafruit-circuitpython-ina260-1.3.8/.gitignore
--rw-r--r--   0 runner    (1001) docker     (121)     1239 2022-08-22 18:40:50.000000 adafruit-circuitpython-ina260-1.3.8/.pre-commit-config.yaml
--rw-r--r--   0 runner    (1001) docker     (121)    16248 2022-08-22 18:40:50.000000 adafruit-circuitpython-ina260-1.3.8/.pylintrc
--rw-r--r--   0 runner    (1001) docker     (121)      388 2022-08-22 18:40:50.000000 adafruit-circuitpython-ina260-1.3.8/.readthedocs.yaml
--rw-r--r--   0 runner    (1001) docker     (121)     6147 2022-08-22 18:40:50.000000 adafruit-circuitpython-ina260-1.3.8/CODE_OF_CONDUCT.md
--rw-r--r--   0 runner    (1001) docker     (121)     1104 2022-08-22 18:40:50.000000 adafruit-circuitpython-ina260-1.3.8/LICENSE
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-22 18:41:08.610823 adafruit-circuitpython-ina260-1.3.8/LICENSES/
--rw-r--r--   0 runner    (1001) docker     (121)    16814 2022-08-22 18:40:50.000000 adafruit-circuitpython-ina260-1.3.8/LICENSES/CC-BY-4.0.txt
--rw-r--r--   0 runner    (1001) docker     (121)     1108 2022-08-22 18:40:50.000000 adafruit-circuitpython-ina260-1.3.8/LICENSES/MIT.txt
--rw-r--r--   0 runner    (1001) docker     (121)     1211 2022-08-22 18:40:50.000000 adafruit-circuitpython-ina260-1.3.8/LICENSES/Unlicense.txt
--rw-r--r--   0 runner    (1001) docker     (121)     3907 2022-08-22 18:41:08.610823 adafruit-circuitpython-ina260-1.3.8/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)     3138 2022-08-22 18:40:50.000000 adafruit-circuitpython-ina260-1.3.8/README.rst
--rw-r--r--   0 runner    (1001) docker     (121)      108 2022-08-22 18:40:50.000000 adafruit-circuitpython-ina260-1.3.8/README.rst.license
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-22 18:41:08.610823 adafruit-circuitpython-ina260-1.3.8/adafruit_circuitpython_ina260.egg-info/
--rw-r--r--   0 runner    (1001) docker     (121)     3907 2022-08-22 18:41:08.000000 adafruit-circuitpython-ina260-1.3.8/adafruit_circuitpython_ina260.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)      998 2022-08-22 18:41:08.000000 adafruit-circuitpython-ina260-1.3.8/adafruit_circuitpython_ina260.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2022-08-22 18:41:08.000000 adafruit-circuitpython-ina260-1.3.8/adafruit_circuitpython_ina260.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (121)       93 2022-08-22 18:41:08.000000 adafruit-circuitpython-ina260-1.3.8/adafruit_circuitpython_ina260.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (121)       16 2022-08-22 18:41:08.000000 adafruit-circuitpython-ina260-1.3.8/adafruit_circuitpython_ina260.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (121)    13755 2022-08-22 18:40:59.000000 adafruit-circuitpython-ina260-1.3.8/adafruit_ina260.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-22 18:41:08.610823 adafruit-circuitpython-ina260-1.3.8/docs/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-22 18:41:08.610823 adafruit-circuitpython-ina260-1.3.8/docs/_static/
--rw-r--r--   0 runner    (1001) docker     (121)     4414 2022-08-22 18:40:50.000000 adafruit-circuitpython-ina260-1.3.8/docs/_static/favicon.ico
--rw-r--r--   0 runner    (1001) docker     (121)      105 2022-08-22 18:40:50.000000 adafruit-circuitpython-ina260-1.3.8/docs/_static/favicon.ico.license
--rw-r--r--   0 runner    (1001) docker     (121)      265 2022-08-22 18:40:50.000000 adafruit-circuitpython-ina260-1.3.8/docs/api.rst
--rw-r--r--   0 runner    (1001) docker     (121)       96 2022-08-22 18:40:50.000000 adafruit-circuitpython-ina260-1.3.8/docs/api.rst.license
--rw-r--r--   0 runner    (1001) docker     (121)     5708 2022-08-22 18:40:50.000000 adafruit-circuitpython-ina260-1.3.8/docs/conf.py
--rw-r--r--   0 runner    (1001) docker     (121)      186 2022-08-22 18:40:50.000000 adafruit-circuitpython-ina260-1.3.8/docs/examples.rst
--rw-r--r--   0 runner    (1001) docker     (121)       96 2022-08-22 18:40:50.000000 adafruit-circuitpython-ina260-1.3.8/docs/examples.rst.license
--rw-r--r--   0 runner    (1001) docker     (121)      971 2022-08-22 18:40:50.000000 adafruit-circuitpython-ina260-1.3.8/docs/index.rst
--rw-r--r--   0 runner    (1001) docker     (121)       96 2022-08-22 18:40:50.000000 adafruit-circuitpython-ina260-1.3.8/docs/index.rst.license
--rw-r--r--   0 runner    (1001) docker     (121)      123 2022-08-22 18:40:50.000000 adafruit-circuitpython-ina260-1.3.8/docs/requirements.txt
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-22 18:41:08.610823 adafruit-circuitpython-ina260-1.3.8/examples/
--rw-r--r--   0 runner    (1001) docker     (121)     1035 2022-08-22 18:40:59.000000 adafruit-circuitpython-ina260-1.3.8/examples/ina260_averaging.py
--rw-r--r--   0 runner    (1001) docker     (121)     1996 2022-08-22 18:40:59.000000 adafruit-circuitpython-ina260-1.3.8/examples/ina260_latch.py
--rw-r--r--   0 runner    (1001) docker     (121)     1475 2022-08-22 18:40:59.000000 adafruit-circuitpython-ina260-1.3.8/examples/ina260_modes.py
--rw-r--r--   0 runner    (1001) docker     (121)      360 2022-08-22 18:40:59.000000 adafruit-circuitpython-ina260-1.3.8/examples/ina260_simpletest.py
--rw-r--r--   0 runner    (1001) docker     (121)      108 2022-08-22 18:40:50.000000 adafruit-circuitpython-ina260-1.3.8/optional_requirements.txt
--rw-r--r--   0 runner    (1001) docker     (121)     1229 2022-08-22 18:40:59.000000 adafruit-circuitpython-ina260-1.3.8/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (121)      190 2022-08-22 18:40:50.000000 adafruit-circuitpython-ina260-1.3.8/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (121)       38 2022-08-22 18:41:08.610823 adafruit-circuitpython-ina260-1.3.8/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-26 02:21:35.116060 adafruit-circuitpython-ina260-1.3.9/
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-26 02:21:35.112060 adafruit-circuitpython-ina260-1.3.9/.github/
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-26 02:21:35.112060 adafruit-circuitpython-ina260-1.3.9/.github/PULL_REQUEST_TEMPLATE/
+-rw-r--r--   0 runner    (1001) docker     (121)      880 2022-08-26 02:21:15.000000 adafruit-circuitpython-ina260-1.3.9/.github/PULL_REQUEST_TEMPLATE/adafruit_circuitpython_pr.md
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-26 02:21:35.112060 adafruit-circuitpython-ina260-1.3.9/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (121)     2535 2022-08-26 02:21:15.000000 adafruit-circuitpython-ina260-1.3.9/.github/workflows/build.yml
+-rw-r--r--   0 runner    (1001) docker     (121)      479 2022-08-26 02:21:15.000000 adafruit-circuitpython-ina260-1.3.9/.github/workflows/failure-help-text.yml
+-rw-r--r--   0 runner    (1001) docker     (121)     2966 2022-08-26 02:21:15.000000 adafruit-circuitpython-ina260-1.3.9/.github/workflows/release.yml
+-rw-r--r--   0 runner    (1001) docker     (121)     1648 2022-08-26 02:21:15.000000 adafruit-circuitpython-ina260-1.3.9/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (121)     1239 2022-08-26 02:21:15.000000 adafruit-circuitpython-ina260-1.3.9/.pre-commit-config.yaml
+-rw-r--r--   0 runner    (1001) docker     (121)    16248 2022-08-26 02:21:15.000000 adafruit-circuitpython-ina260-1.3.9/.pylintrc
+-rw-r--r--   0 runner    (1001) docker     (121)      388 2022-08-26 02:21:15.000000 adafruit-circuitpython-ina260-1.3.9/.readthedocs.yaml
+-rw-r--r--   0 runner    (1001) docker     (121)     6147 2022-08-26 02:21:15.000000 adafruit-circuitpython-ina260-1.3.9/CODE_OF_CONDUCT.md
+-rw-r--r--   0 runner    (1001) docker     (121)     1104 2022-08-26 02:21:15.000000 adafruit-circuitpython-ina260-1.3.9/LICENSE
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-26 02:21:35.112060 adafruit-circuitpython-ina260-1.3.9/LICENSES/
+-rw-r--r--   0 runner    (1001) docker     (121)    16814 2022-08-26 02:21:15.000000 adafruit-circuitpython-ina260-1.3.9/LICENSES/CC-BY-4.0.txt
+-rw-r--r--   0 runner    (1001) docker     (121)     1108 2022-08-26 02:21:15.000000 adafruit-circuitpython-ina260-1.3.9/LICENSES/MIT.txt
+-rw-r--r--   0 runner    (1001) docker     (121)     1211 2022-08-26 02:21:15.000000 adafruit-circuitpython-ina260-1.3.9/LICENSES/Unlicense.txt
+-rw-r--r--   0 runner    (1001) docker     (121)     3907 2022-08-26 02:21:35.116060 adafruit-circuitpython-ina260-1.3.9/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (121)     3138 2022-08-26 02:21:15.000000 adafruit-circuitpython-ina260-1.3.9/README.rst
+-rw-r--r--   0 runner    (1001) docker     (121)      108 2022-08-26 02:21:15.000000 adafruit-circuitpython-ina260-1.3.9/README.rst.license
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-26 02:21:35.116060 adafruit-circuitpython-ina260-1.3.9/adafruit_circuitpython_ina260.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (121)     3907 2022-08-26 02:21:35.000000 adafruit-circuitpython-ina260-1.3.9/adafruit_circuitpython_ina260.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (121)      998 2022-08-26 02:21:35.000000 adafruit-circuitpython-ina260-1.3.9/adafruit_circuitpython_ina260.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (121)        1 2022-08-26 02:21:35.000000 adafruit-circuitpython-ina260-1.3.9/adafruit_circuitpython_ina260.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (121)       93 2022-08-26 02:21:35.000000 adafruit-circuitpython-ina260-1.3.9/adafruit_circuitpython_ina260.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (121)       16 2022-08-26 02:21:35.000000 adafruit-circuitpython-ina260-1.3.9/adafruit_circuitpython_ina260.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (121)    13755 2022-08-26 02:21:26.000000 adafruit-circuitpython-ina260-1.3.9/adafruit_ina260.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-26 02:21:35.116060 adafruit-circuitpython-ina260-1.3.9/docs/
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-26 02:21:35.116060 adafruit-circuitpython-ina260-1.3.9/docs/_static/
+-rw-r--r--   0 runner    (1001) docker     (121)     4414 2022-08-26 02:21:15.000000 adafruit-circuitpython-ina260-1.3.9/docs/_static/favicon.ico
+-rw-r--r--   0 runner    (1001) docker     (121)      105 2022-08-26 02:21:15.000000 adafruit-circuitpython-ina260-1.3.9/docs/_static/favicon.ico.license
+-rw-r--r--   0 runner    (1001) docker     (121)      265 2022-08-26 02:21:15.000000 adafruit-circuitpython-ina260-1.3.9/docs/api.rst
+-rw-r--r--   0 runner    (1001) docker     (121)       96 2022-08-26 02:21:15.000000 adafruit-circuitpython-ina260-1.3.9/docs/api.rst.license
+-rw-r--r--   0 runner    (1001) docker     (121)     5928 2022-08-26 02:21:15.000000 adafruit-circuitpython-ina260-1.3.9/docs/conf.py
+-rw-r--r--   0 runner    (1001) docker     (121)      186 2022-08-26 02:21:15.000000 adafruit-circuitpython-ina260-1.3.9/docs/examples.rst
+-rw-r--r--   0 runner    (1001) docker     (121)       96 2022-08-26 02:21:15.000000 adafruit-circuitpython-ina260-1.3.9/docs/examples.rst.license
+-rw-r--r--   0 runner    (1001) docker     (121)      971 2022-08-26 02:21:15.000000 adafruit-circuitpython-ina260-1.3.9/docs/index.rst
+-rw-r--r--   0 runner    (1001) docker     (121)       96 2022-08-26 02:21:15.000000 adafruit-circuitpython-ina260-1.3.9/docs/index.rst.license
+-rw-r--r--   0 runner    (1001) docker     (121)      123 2022-08-26 02:21:15.000000 adafruit-circuitpython-ina260-1.3.9/docs/requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-26 02:21:35.116060 adafruit-circuitpython-ina260-1.3.9/examples/
+-rw-r--r--   0 runner    (1001) docker     (121)     1035 2022-08-26 02:21:26.000000 adafruit-circuitpython-ina260-1.3.9/examples/ina260_averaging.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1996 2022-08-26 02:21:26.000000 adafruit-circuitpython-ina260-1.3.9/examples/ina260_latch.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1475 2022-08-26 02:21:26.000000 adafruit-circuitpython-ina260-1.3.9/examples/ina260_modes.py
+-rw-r--r--   0 runner    (1001) docker     (121)      360 2022-08-26 02:21:26.000000 adafruit-circuitpython-ina260-1.3.9/examples/ina260_simpletest.py
+-rw-r--r--   0 runner    (1001) docker     (121)      108 2022-08-26 02:21:15.000000 adafruit-circuitpython-ina260-1.3.9/optional_requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (121)     1229 2022-08-26 02:21:26.000000 adafruit-circuitpython-ina260-1.3.9/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (121)      190 2022-08-26 02:21:15.000000 adafruit-circuitpython-ina260-1.3.9/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (121)       38 2022-08-26 02:21:35.116060 adafruit-circuitpython-ina260-1.3.9/setup.cfg
```

### Comparing `adafruit-circuitpython-ina260-1.3.8/.github/PULL_REQUEST_TEMPLATE/adafruit_circuitpython_pr.md` & `adafruit-circuitpython-ina260-1.3.9/.github/PULL_REQUEST_TEMPLATE/adafruit_circuitpython_pr.md`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-ina260-1.3.8/.github/workflows/build.yml` & `adafruit-circuitpython-ina260-1.3.9/.github/workflows/build.yml`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-ina260-1.3.8/.github/workflows/release.yml` & `adafruit-circuitpython-ina260-1.3.9/.github/workflows/release.yml`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-ina260-1.3.8/.gitignore` & `adafruit-circuitpython-ina260-1.3.9/.gitignore`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-ina260-1.3.8/.pre-commit-config.yaml` & `adafruit-circuitpython-ina260-1.3.9/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-ina260-1.3.8/.pylintrc` & `adafruit-circuitpython-ina260-1.3.9/.pylintrc`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-ina260-1.3.8/CODE_OF_CONDUCT.md` & `adafruit-circuitpython-ina260-1.3.9/CODE_OF_CONDUCT.md`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-ina260-1.3.8/LICENSE` & `adafruit-circuitpython-ina260-1.3.9/LICENSE`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-ina260-1.3.8/LICENSES/CC-BY-4.0.txt` & `adafruit-circuitpython-ina260-1.3.9/LICENSES/CC-BY-4.0.txt`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-ina260-1.3.8/LICENSES/MIT.txt` & `adafruit-circuitpython-ina260-1.3.9/LICENSES/MIT.txt`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-ina260-1.3.8/LICENSES/Unlicense.txt` & `adafruit-circuitpython-ina260-1.3.9/LICENSES/Unlicense.txt`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-ina260-1.3.8/PKG-INFO` & `adafruit-circuitpython-ina260-1.3.9/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: adafruit-circuitpython-ina260
-Version: 1.3.8
+Version: 1.3.9
 Summary: CircuitPython driver for the TI INA260 current and power sensor
 Author-email: Adafruit Industries <circuitpython@adafruit.com>
 License: MIT
 Project-URL: Homepage, https://github.com/adafruit/Adafruit_CircuitPython_INA260
 Keywords: adafruit,blinka,circuitpython,micropython,ina260,power,current,voltage
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Software Development :: Libraries
```

### Comparing `adafruit-circuitpython-ina260-1.3.8/README.rst` & `adafruit-circuitpython-ina260-1.3.9/README.rst`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-ina260-1.3.8/adafruit_circuitpython_ina260.egg-info/PKG-INFO` & `adafruit-circuitpython-ina260-1.3.9/adafruit_circuitpython_ina260.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: adafruit-circuitpython-ina260
-Version: 1.3.8
+Version: 1.3.9
 Summary: CircuitPython driver for the TI INA260 current and power sensor
 Author-email: Adafruit Industries <circuitpython@adafruit.com>
 License: MIT
 Project-URL: Homepage, https://github.com/adafruit/Adafruit_CircuitPython_INA260
 Keywords: adafruit,blinka,circuitpython,micropython,ina260,power,current,voltage
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Software Development :: Libraries
```

### Comparing `adafruit-circuitpython-ina260-1.3.8/adafruit_circuitpython_ina260.egg-info/SOURCES.txt` & `adafruit-circuitpython-ina260-1.3.9/adafruit_circuitpython_ina260.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-ina260-1.3.8/adafruit_ina260.py` & `adafruit-circuitpython-ina260-1.3.9/adafruit_ina260.py`

 * *Files 0% similar despite different names*

```diff
@@ -16,15 +16,15 @@
 * https://github.com/adafruit/circuitpython/releases
 * Adafruit's Bus Device library: https://github.com/adafruit/Adafruit_CircuitPython_BusDevice
 * Adafruit's Register library: https://github.com/adafruit/Adafruit_CircuitPython_Register
 """
 
 # imports
 
-__version__ = "1.3.8"
+__version__ = "1.3.9"
 __repo__ = "https://github.com/adafruit/Adafruit_CircuitPython_INA260.git"
 
 from micropython import const
 import adafruit_bus_device.i2c_device as i2cdevice
 
 from adafruit_register.i2c_struct import ROUnaryStruct
 from adafruit_register.i2c_bits import ROBits, RWBits
```

### Comparing `adafruit-circuitpython-ina260-1.3.8/docs/_static/favicon.ico` & `adafruit-circuitpython-ina260-1.3.9/docs/_static/favicon.ico`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-ina260-1.3.8/docs/conf.py` & `adafruit-circuitpython-ina260-1.3.9/docs/conf.py`

 * *Files 8% similar despite different names*

```diff
@@ -2,14 +2,15 @@
 
 # SPDX-FileCopyrightText: 2021 ladyada for Adafruit Industries
 #
 # SPDX-License-Identifier: MIT
 
 import os
 import sys
+import datetime
 
 sys.path.insert(0, os.path.abspath(".."))
 
 # -- General configuration ------------------------------------------------
 
 # Add any Sphinx extension module names here, as strings. They can be
 # extensions coming with Sphinx (named 'sphinx.ext.*') or your custom
@@ -52,15 +53,22 @@
 source_suffix = ".rst"
 
 # The master toctree document.
 master_doc = "index"
 
 # General information about the project.
 project = "Adafruit INA260 Library"
-copyright = "2019 Bryan Siepert"
+creation_year = "2019"
+current_year = str(datetime.datetime.now().year)
+year_duration = (
+    current_year
+    if current_year == creation_year
+    else creation_year + " - " + current_year
+)
+copyright = year_duration + " Bryan Siepert"
 author = "Bryan Siepert"
 
 # The version info for the project you're documenting, acts as replacement for
 # |version| and |release|, also used in various other places throughout the
 # built documents.
 #
 # The short X.Y version.
```

### Comparing `adafruit-circuitpython-ina260-1.3.8/docs/index.rst` & `adafruit-circuitpython-ina260-1.3.9/docs/index.rst`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-ina260-1.3.8/examples/ina260_averaging.py` & `adafruit-circuitpython-ina260-1.3.9/examples/ina260_averaging.py`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-ina260-1.3.8/examples/ina260_latch.py` & `adafruit-circuitpython-ina260-1.3.9/examples/ina260_latch.py`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-ina260-1.3.8/examples/ina260_modes.py` & `adafruit-circuitpython-ina260-1.3.9/examples/ina260_modes.py`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-ina260-1.3.8/pyproject.toml` & `adafruit-circuitpython-ina260-1.3.9/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -8,15 +8,15 @@
     "wheel",
     "setuptools-scm",
 ]
 
 [project]
 name = "adafruit-circuitpython-ina260"
 description = "CircuitPython driver for the TI INA260 current and power sensor"
-version = "1.3.8"
+version = "1.3.9"
 readme = "README.rst"
 authors = [
     {name = "Adafruit Industries", email = "circuitpython@adafruit.com"}
 ]
 urls = {Homepage = "https://github.com/adafruit/Adafruit_CircuitPython_INA260"}
 keywords = [
     "adafruit",
```

