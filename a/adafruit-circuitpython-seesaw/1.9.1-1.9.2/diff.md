# Comparing `tmp/adafruit-circuitpython-seesaw-1.9.1.tar.gz` & `tmp/adafruit-circuitpython-seesaw-1.9.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "adafruit-circuitpython-seesaw-1.9.1.tar", last modified: Fri Jun 11 15:28:17 2021, max compression
+gzip compressed data, was "adafruit-circuitpython-seesaw-1.9.2.tar", last modified: Mon Jun 14 19:28:32 2021, max compression
```

## Comparing `adafruit-circuitpython-seesaw-1.9.1.tar` & `adafruit-circuitpython-seesaw-1.9.2.tar`

### file list

```diff
@@ -1,62 +1,62 @@
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-06-11 15:28:17.741288 adafruit-circuitpython-seesaw-1.9.1/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-06-11 15:28:17.733287 adafruit-circuitpython-seesaw-1.9.1/.github/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-06-11 15:28:17.737287 adafruit-circuitpython-seesaw-1.9.1/.github/PULL_REQUEST_TEMPLATE/
--rw-r--r--   0 runner    (1001) docker     (121)      886 2021-06-11 15:28:08.000000 adafruit-circuitpython-seesaw-1.9.1/.github/PULL_REQUEST_TEMPLATE/adafruit_circuitpython_pr.md
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-06-11 15:28:17.737287 adafruit-circuitpython-seesaw-1.9.1/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (121)     2437 2021-06-11 15:28:08.000000 adafruit-circuitpython-seesaw-1.9.1/.github/workflows/build.yml
--rw-r--r--   0 runner    (1001) docker     (121)      479 2021-06-11 15:28:08.000000 adafruit-circuitpython-seesaw-1.9.1/.github/workflows/failure-help-text.yml
--rw-r--r--   0 runner    (1001) docker     (121)     2712 2021-06-11 15:28:08.000000 adafruit-circuitpython-seesaw-1.9.1/.github/workflows/release.yml
--rw-r--r--   0 runner    (1001) docker     (121)      189 2021-06-11 15:28:08.000000 adafruit-circuitpython-seesaw-1.9.1/.gitignore
--rw-r--r--   0 runner    (1001) docker     (121)     1020 2021-06-11 15:28:08.000000 adafruit-circuitpython-seesaw-1.9.1/.pre-commit-config.yaml
--rw-r--r--   0 runner    (1001) docker     (121)    16223 2021-06-11 15:28:08.000000 adafruit-circuitpython-seesaw-1.9.1/.pylintrc
--rw-r--r--   0 runner    (1001) docker     (121)      162 2021-06-11 15:28:08.000000 adafruit-circuitpython-seesaw-1.9.1/.readthedocs.yml
--rw-r--r--   0 runner    (1001) docker     (121)     6147 2021-06-11 15:28:08.000000 adafruit-circuitpython-seesaw-1.9.1/CODE_OF_CONDUCT.md
--rw-r--r--   0 runner    (1001) docker     (121)     1102 2021-06-11 15:28:08.000000 adafruit-circuitpython-seesaw-1.9.1/LICENSE
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-06-11 15:28:17.737287 adafruit-circuitpython-seesaw-1.9.1/LICENSES/
--rw-r--r--   0 runner    (1001) docker     (121)    16814 2021-06-11 15:28:08.000000 adafruit-circuitpython-seesaw-1.9.1/LICENSES/CC-BY-4.0.txt
--rw-r--r--   0 runner    (1001) docker     (121)     1108 2021-06-11 15:28:08.000000 adafruit-circuitpython-seesaw-1.9.1/LICENSES/MIT.txt
--rw-r--r--   0 runner    (1001) docker     (121)     1211 2021-06-11 15:28:08.000000 adafruit-circuitpython-seesaw-1.9.1/LICENSES/Unlicense.txt
--rw-r--r--   0 runner    (1001) docker     (121)     3635 2021-06-11 15:28:17.741288 adafruit-circuitpython-seesaw-1.9.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)     2270 2021-06-11 15:28:08.000000 adafruit-circuitpython-seesaw-1.9.1/README.rst
--rw-r--r--   0 runner    (1001) docker     (121)      108 2021-06-11 15:28:08.000000 adafruit-circuitpython-seesaw-1.9.1/README.rst.license
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-06-11 15:28:17.737287 adafruit-circuitpython-seesaw-1.9.1/adafruit_circuitpython_seesaw.egg-info/
--rw-r--r--   0 runner    (1001) docker     (121)     3635 2021-06-11 15:28:17.000000 adafruit-circuitpython-seesaw-1.9.1/adafruit_circuitpython_seesaw.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)     1391 2021-06-11 15:28:17.000000 adafruit-circuitpython-seesaw-1.9.1/adafruit_circuitpython_seesaw.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2021-06-11 15:28:17.000000 adafruit-circuitpython-seesaw-1.9.1/adafruit_circuitpython_seesaw.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (121)       49 2021-06-11 15:28:17.000000 adafruit-circuitpython-seesaw-1.9.1/adafruit_circuitpython_seesaw.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (121)       16 2021-06-11 15:28:17.000000 adafruit-circuitpython-seesaw-1.9.1/adafruit_circuitpython_seesaw.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-06-11 15:28:17.737287 adafruit-circuitpython-seesaw-1.9.1/adafruit_seesaw/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2021-06-11 15:28:08.000000 adafruit-circuitpython-seesaw-1.9.1/adafruit_seesaw/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     1060 2021-06-11 15:28:08.000000 adafruit-circuitpython-seesaw-1.9.1/adafruit_seesaw/analoginput.py
--rw-r--r--   0 runner    (1001) docker     (121)     3140 2021-06-11 15:28:08.000000 adafruit-circuitpython-seesaw-1.9.1/adafruit_seesaw/crickit.py
--rw-r--r--   0 runner    (1001) docker     (121)     3484 2021-06-11 15:28:08.000000 adafruit-circuitpython-seesaw-1.9.1/adafruit_seesaw/digitalio.py
--rw-r--r--   0 runner    (1001) docker     (121)     3477 2021-06-11 15:28:08.000000 adafruit-circuitpython-seesaw-1.9.1/adafruit_seesaw/keypad.py
--rw-r--r--   0 runner    (1001) docker     (121)     4885 2021-06-11 15:28:08.000000 adafruit-circuitpython-seesaw-1.9.1/adafruit_seesaw/neopixel.py
--rw-r--r--   0 runner    (1001) docker     (121)     1759 2021-06-11 15:28:08.000000 adafruit-circuitpython-seesaw-1.9.1/adafruit_seesaw/pwmout.py
--rw-r--r--   0 runner    (1001) docker     (121)     3210 2021-06-11 15:28:08.000000 adafruit-circuitpython-seesaw-1.9.1/adafruit_seesaw/robohat.py
--rw-r--r--   0 runner    (1001) docker     (121)     1059 2021-06-11 15:28:08.000000 adafruit-circuitpython-seesaw-1.9.1/adafruit_seesaw/rotaryio.py
--rw-r--r--   0 runner    (1001) docker     (121)     1435 2021-06-11 15:28:08.000000 adafruit-circuitpython-seesaw-1.9.1/adafruit_seesaw/samd09.py
--rw-r--r--   0 runner    (1001) docker     (121)    15343 2021-06-11 15:28:08.000000 adafruit-circuitpython-seesaw-1.9.1/adafruit_seesaw/seesaw.py
--rwxr-xr-x   0 runner    (1001) docker     (121)     3519 2021-06-11 15:28:08.000000 adafruit-circuitpython-seesaw-1.9.1/adafruit_seesaw/tftshield18.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-06-11 15:28:17.741288 adafruit-circuitpython-seesaw-1.9.1/docs/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-06-11 15:28:17.741288 adafruit-circuitpython-seesaw-1.9.1/docs/_static/
--rw-r--r--   0 runner    (1001) docker     (121)     4414 2021-06-11 15:28:08.000000 adafruit-circuitpython-seesaw-1.9.1/docs/_static/favicon.ico
--rw-r--r--   0 runner    (1001) docker     (121)      105 2021-06-11 15:28:08.000000 adafruit-circuitpython-seesaw-1.9.1/docs/_static/favicon.ico.license
--rw-r--r--   0 runner    (1001) docker     (121)      782 2021-06-11 15:28:08.000000 adafruit-circuitpython-seesaw-1.9.1/docs/api.rst
--rw-r--r--   0 runner    (1001) docker     (121)       96 2021-06-11 15:28:08.000000 adafruit-circuitpython-seesaw-1.9.1/docs/api.rst.license
--rwxr-xr-x   0 runner    (1001) docker     (121)     5805 2021-06-11 15:28:08.000000 adafruit-circuitpython-seesaw-1.9.1/docs/conf.py
--rw-r--r--   0 runner    (1001) docker     (121)     1011 2021-06-11 15:28:08.000000 adafruit-circuitpython-seesaw-1.9.1/docs/examples.rst
--rw-r--r--   0 runner    (1001) docker     (121)       96 2021-06-11 15:28:08.000000 adafruit-circuitpython-seesaw-1.9.1/docs/examples.rst.license
--rw-r--r--   0 runner    (1001) docker     (121)     2263 2021-06-11 15:28:08.000000 adafruit-circuitpython-seesaw-1.9.1/docs/index.rst
--rw-r--r--   0 runner    (1001) docker     (121)       96 2021-06-11 15:28:08.000000 adafruit-circuitpython-seesaw-1.9.1/docs/index.rst.license
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-06-11 15:28:17.741288 adafruit-circuitpython-seesaw-1.9.1/examples/
--rw-r--r--   0 runner    (1001) docker     (121)     5034 2021-06-11 15:28:08.000000 adafruit-circuitpython-seesaw-1.9.1/examples/seesaw_crickit_test.py
--rwxr-xr-x   0 runner    (1001) docker     (121)     1199 2021-06-11 15:28:08.000000 adafruit-circuitpython-seesaw-1.9.1/examples/seesaw_joy_featherwing.py
--rw-r--r--   0 runner    (1001) docker     (121)     1257 2021-06-11 15:28:08.000000 adafruit-circuitpython-seesaw-1.9.1/examples/seesaw_minitft_featherwing.py
--rw-r--r--   0 runner    (1001) docker     (121)     1584 2021-06-11 15:28:08.000000 adafruit-circuitpython-seesaw-1.9.1/examples/seesaw_rotary_neopixel.py
--rw-r--r--   0 runner    (1001) docker     (121)      995 2021-06-11 15:28:08.000000 adafruit-circuitpython-seesaw-1.9.1/examples/seesaw_rotary_simpletest.py
--rw-r--r--   0 runner    (1001) docker     (121)      669 2021-06-11 15:28:08.000000 adafruit-circuitpython-seesaw-1.9.1/examples/seesaw_simpletest.py
--rw-r--r--   0 runner    (1001) docker     (121)      477 2021-06-11 15:28:08.000000 adafruit-circuitpython-seesaw-1.9.1/examples/seesaw_soil_simpletest.py
--rwxr-xr-x   0 runner    (1001) docker     (121)      152 2021-06-11 15:28:08.000000 adafruit-circuitpython-seesaw-1.9.1/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (121)       38 2021-06-11 15:28:17.741288 adafruit-circuitpython-seesaw-1.9.1/setup.cfg
--rwxr-xr-x   0 runner    (1001) docker     (121)     1929 2021-06-11 15:28:08.000000 adafruit-circuitpython-seesaw-1.9.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-06-14 19:28:32.826600 adafruit-circuitpython-seesaw-1.9.2/
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-06-14 19:28:32.822600 adafruit-circuitpython-seesaw-1.9.2/.github/
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-06-14 19:28:32.822600 adafruit-circuitpython-seesaw-1.9.2/.github/PULL_REQUEST_TEMPLATE/
+-rw-r--r--   0 runner    (1001) docker     (121)      886 2021-06-14 19:28:25.000000 adafruit-circuitpython-seesaw-1.9.2/.github/PULL_REQUEST_TEMPLATE/adafruit_circuitpython_pr.md
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-06-14 19:28:32.822600 adafruit-circuitpython-seesaw-1.9.2/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (121)     2437 2021-06-14 19:28:25.000000 adafruit-circuitpython-seesaw-1.9.2/.github/workflows/build.yml
+-rw-r--r--   0 runner    (1001) docker     (121)      479 2021-06-14 19:28:25.000000 adafruit-circuitpython-seesaw-1.9.2/.github/workflows/failure-help-text.yml
+-rw-r--r--   0 runner    (1001) docker     (121)     2712 2021-06-14 19:28:25.000000 adafruit-circuitpython-seesaw-1.9.2/.github/workflows/release.yml
+-rw-r--r--   0 runner    (1001) docker     (121)      189 2021-06-14 19:28:25.000000 adafruit-circuitpython-seesaw-1.9.2/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (121)     1020 2021-06-14 19:28:25.000000 adafruit-circuitpython-seesaw-1.9.2/.pre-commit-config.yaml
+-rw-r--r--   0 runner    (1001) docker     (121)    16223 2021-06-14 19:28:25.000000 adafruit-circuitpython-seesaw-1.9.2/.pylintrc
+-rw-r--r--   0 runner    (1001) docker     (121)      162 2021-06-14 19:28:25.000000 adafruit-circuitpython-seesaw-1.9.2/.readthedocs.yml
+-rw-r--r--   0 runner    (1001) docker     (121)     6147 2021-06-14 19:28:25.000000 adafruit-circuitpython-seesaw-1.9.2/CODE_OF_CONDUCT.md
+-rw-r--r--   0 runner    (1001) docker     (121)     1102 2021-06-14 19:28:25.000000 adafruit-circuitpython-seesaw-1.9.2/LICENSE
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-06-14 19:28:32.822600 adafruit-circuitpython-seesaw-1.9.2/LICENSES/
+-rw-r--r--   0 runner    (1001) docker     (121)    16814 2021-06-14 19:28:25.000000 adafruit-circuitpython-seesaw-1.9.2/LICENSES/CC-BY-4.0.txt
+-rw-r--r--   0 runner    (1001) docker     (121)     1108 2021-06-14 19:28:25.000000 adafruit-circuitpython-seesaw-1.9.2/LICENSES/MIT.txt
+-rw-r--r--   0 runner    (1001) docker     (121)     1211 2021-06-14 19:28:25.000000 adafruit-circuitpython-seesaw-1.9.2/LICENSES/Unlicense.txt
+-rw-r--r--   0 runner    (1001) docker     (121)     3635 2021-06-14 19:28:32.826600 adafruit-circuitpython-seesaw-1.9.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (121)     2270 2021-06-14 19:28:25.000000 adafruit-circuitpython-seesaw-1.9.2/README.rst
+-rw-r--r--   0 runner    (1001) docker     (121)      108 2021-06-14 19:28:25.000000 adafruit-circuitpython-seesaw-1.9.2/README.rst.license
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-06-14 19:28:32.822600 adafruit-circuitpython-seesaw-1.9.2/adafruit_circuitpython_seesaw.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (121)     3635 2021-06-14 19:28:32.000000 adafruit-circuitpython-seesaw-1.9.2/adafruit_circuitpython_seesaw.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (121)     1391 2021-06-14 19:28:32.000000 adafruit-circuitpython-seesaw-1.9.2/adafruit_circuitpython_seesaw.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (121)        1 2021-06-14 19:28:32.000000 adafruit-circuitpython-seesaw-1.9.2/adafruit_circuitpython_seesaw.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (121)       49 2021-06-14 19:28:32.000000 adafruit-circuitpython-seesaw-1.9.2/adafruit_circuitpython_seesaw.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (121)       16 2021-06-14 19:28:32.000000 adafruit-circuitpython-seesaw-1.9.2/adafruit_circuitpython_seesaw.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-06-14 19:28:32.826600 adafruit-circuitpython-seesaw-1.9.2/adafruit_seesaw/
+-rw-r--r--   0 runner    (1001) docker     (121)        0 2021-06-14 19:28:25.000000 adafruit-circuitpython-seesaw-1.9.2/adafruit_seesaw/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1060 2021-06-14 19:28:25.000000 adafruit-circuitpython-seesaw-1.9.2/adafruit_seesaw/analoginput.py
+-rw-r--r--   0 runner    (1001) docker     (121)     3140 2021-06-14 19:28:25.000000 adafruit-circuitpython-seesaw-1.9.2/adafruit_seesaw/crickit.py
+-rw-r--r--   0 runner    (1001) docker     (121)     3484 2021-06-14 19:28:25.000000 adafruit-circuitpython-seesaw-1.9.2/adafruit_seesaw/digitalio.py
+-rw-r--r--   0 runner    (1001) docker     (121)     3477 2021-06-14 19:28:25.000000 adafruit-circuitpython-seesaw-1.9.2/adafruit_seesaw/keypad.py
+-rw-r--r--   0 runner    (1001) docker     (121)     4885 2021-06-14 19:28:25.000000 adafruit-circuitpython-seesaw-1.9.2/adafruit_seesaw/neopixel.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1759 2021-06-14 19:28:25.000000 adafruit-circuitpython-seesaw-1.9.2/adafruit_seesaw/pwmout.py
+-rw-r--r--   0 runner    (1001) docker     (121)     3210 2021-06-14 19:28:25.000000 adafruit-circuitpython-seesaw-1.9.2/adafruit_seesaw/robohat.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1059 2021-06-14 19:28:25.000000 adafruit-circuitpython-seesaw-1.9.2/adafruit_seesaw/rotaryio.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1435 2021-06-14 19:28:25.000000 adafruit-circuitpython-seesaw-1.9.2/adafruit_seesaw/samd09.py
+-rw-r--r--   0 runner    (1001) docker     (121)    15343 2021-06-14 19:28:25.000000 adafruit-circuitpython-seesaw-1.9.2/adafruit_seesaw/seesaw.py
+-rwxr-xr-x   0 runner    (1001) docker     (121)     3519 2021-06-14 19:28:25.000000 adafruit-circuitpython-seesaw-1.9.2/adafruit_seesaw/tftshield18.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-06-14 19:28:32.826600 adafruit-circuitpython-seesaw-1.9.2/docs/
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-06-14 19:28:32.826600 adafruit-circuitpython-seesaw-1.9.2/docs/_static/
+-rw-r--r--   0 runner    (1001) docker     (121)     4414 2021-06-14 19:28:25.000000 adafruit-circuitpython-seesaw-1.9.2/docs/_static/favicon.ico
+-rw-r--r--   0 runner    (1001) docker     (121)      105 2021-06-14 19:28:25.000000 adafruit-circuitpython-seesaw-1.9.2/docs/_static/favicon.ico.license
+-rw-r--r--   0 runner    (1001) docker     (121)      782 2021-06-14 19:28:25.000000 adafruit-circuitpython-seesaw-1.9.2/docs/api.rst
+-rw-r--r--   0 runner    (1001) docker     (121)       96 2021-06-14 19:28:25.000000 adafruit-circuitpython-seesaw-1.9.2/docs/api.rst.license
+-rwxr-xr-x   0 runner    (1001) docker     (121)     5805 2021-06-14 19:28:25.000000 adafruit-circuitpython-seesaw-1.9.2/docs/conf.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1011 2021-06-14 19:28:25.000000 adafruit-circuitpython-seesaw-1.9.2/docs/examples.rst
+-rw-r--r--   0 runner    (1001) docker     (121)       96 2021-06-14 19:28:25.000000 adafruit-circuitpython-seesaw-1.9.2/docs/examples.rst.license
+-rw-r--r--   0 runner    (1001) docker     (121)     2263 2021-06-14 19:28:25.000000 adafruit-circuitpython-seesaw-1.9.2/docs/index.rst
+-rw-r--r--   0 runner    (1001) docker     (121)       96 2021-06-14 19:28:25.000000 adafruit-circuitpython-seesaw-1.9.2/docs/index.rst.license
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-06-14 19:28:32.826600 adafruit-circuitpython-seesaw-1.9.2/examples/
+-rw-r--r--   0 runner    (1001) docker     (121)     5034 2021-06-14 19:28:25.000000 adafruit-circuitpython-seesaw-1.9.2/examples/seesaw_crickit_test.py
+-rwxr-xr-x   0 runner    (1001) docker     (121)     1199 2021-06-14 19:28:25.000000 adafruit-circuitpython-seesaw-1.9.2/examples/seesaw_joy_featherwing.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1257 2021-06-14 19:28:25.000000 adafruit-circuitpython-seesaw-1.9.2/examples/seesaw_minitft_featherwing.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1689 2021-06-14 19:28:25.000000 adafruit-circuitpython-seesaw-1.9.2/examples/seesaw_rotary_neopixel.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1168 2021-06-14 19:28:25.000000 adafruit-circuitpython-seesaw-1.9.2/examples/seesaw_rotary_simpletest.py
+-rw-r--r--   0 runner    (1001) docker     (121)      669 2021-06-14 19:28:25.000000 adafruit-circuitpython-seesaw-1.9.2/examples/seesaw_simpletest.py
+-rw-r--r--   0 runner    (1001) docker     (121)      477 2021-06-14 19:28:25.000000 adafruit-circuitpython-seesaw-1.9.2/examples/seesaw_soil_simpletest.py
+-rwxr-xr-x   0 runner    (1001) docker     (121)      152 2021-06-14 19:28:25.000000 adafruit-circuitpython-seesaw-1.9.2/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (121)       38 2021-06-14 19:28:32.826600 adafruit-circuitpython-seesaw-1.9.2/setup.cfg
+-rwxr-xr-x   0 runner    (1001) docker     (121)     1929 2021-06-14 19:28:25.000000 adafruit-circuitpython-seesaw-1.9.2/setup.py
```

### Comparing `adafruit-circuitpython-seesaw-1.9.1/.github/PULL_REQUEST_TEMPLATE/adafruit_circuitpython_pr.md` & `adafruit-circuitpython-seesaw-1.9.2/.github/PULL_REQUEST_TEMPLATE/adafruit_circuitpython_pr.md`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-seesaw-1.9.1/.github/workflows/build.yml` & `adafruit-circuitpython-seesaw-1.9.2/.github/workflows/build.yml`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-seesaw-1.9.1/.github/workflows/release.yml` & `adafruit-circuitpython-seesaw-1.9.2/.github/workflows/release.yml`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-seesaw-1.9.1/.pre-commit-config.yaml` & `adafruit-circuitpython-seesaw-1.9.2/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-seesaw-1.9.1/.pylintrc` & `adafruit-circuitpython-seesaw-1.9.2/.pylintrc`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-seesaw-1.9.1/CODE_OF_CONDUCT.md` & `adafruit-circuitpython-seesaw-1.9.2/CODE_OF_CONDUCT.md`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-seesaw-1.9.1/LICENSE` & `adafruit-circuitpython-seesaw-1.9.2/LICENSE`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-seesaw-1.9.1/LICENSES/CC-BY-4.0.txt` & `adafruit-circuitpython-seesaw-1.9.2/LICENSES/CC-BY-4.0.txt`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-seesaw-1.9.1/LICENSES/MIT.txt` & `adafruit-circuitpython-seesaw-1.9.2/LICENSES/MIT.txt`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-seesaw-1.9.1/LICENSES/Unlicense.txt` & `adafruit-circuitpython-seesaw-1.9.2/LICENSES/Unlicense.txt`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-seesaw-1.9.1/PKG-INFO` & `adafruit-circuitpython-seesaw-1.9.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: adafruit-circuitpython-seesaw
-Version: 1.9.1
+Version: 1.9.2
 Summary: CircuitPython library for controlling a SeeSaw helper chip.
 Home-page: https://github.com/adafruit/Adafruit_CircuitPython_seesaw
 Author: Adafruit Industries
 Author-email: circuitpython@adafruit.com
 License: MIT
 Description: 
         Introduction
```

### Comparing `adafruit-circuitpython-seesaw-1.9.1/README.rst` & `adafruit-circuitpython-seesaw-1.9.2/README.rst`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-seesaw-1.9.1/adafruit_circuitpython_seesaw.egg-info/PKG-INFO` & `adafruit-circuitpython-seesaw-1.9.2/adafruit_circuitpython_seesaw.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: adafruit-circuitpython-seesaw
-Version: 1.9.1
+Version: 1.9.2
 Summary: CircuitPython library for controlling a SeeSaw helper chip.
 Home-page: https://github.com/adafruit/Adafruit_CircuitPython_seesaw
 Author: Adafruit Industries
 Author-email: circuitpython@adafruit.com
 License: MIT
 Description: 
         Introduction
```

### Comparing `adafruit-circuitpython-seesaw-1.9.1/adafruit_circuitpython_seesaw.egg-info/SOURCES.txt` & `adafruit-circuitpython-seesaw-1.9.2/adafruit_circuitpython_seesaw.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-seesaw-1.9.1/adafruit_seesaw/analoginput.py` & `adafruit-circuitpython-seesaw-1.9.2/adafruit_seesaw/analoginput.py`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-seesaw-1.9.1/adafruit_seesaw/crickit.py` & `adafruit-circuitpython-seesaw-1.9.2/adafruit_seesaw/crickit.py`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-seesaw-1.9.1/adafruit_seesaw/digitalio.py` & `adafruit-circuitpython-seesaw-1.9.2/adafruit_seesaw/digitalio.py`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-seesaw-1.9.1/adafruit_seesaw/keypad.py` & `adafruit-circuitpython-seesaw-1.9.2/adafruit_seesaw/keypad.py`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-seesaw-1.9.1/adafruit_seesaw/neopixel.py` & `adafruit-circuitpython-seesaw-1.9.2/adafruit_seesaw/neopixel.py`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-seesaw-1.9.1/adafruit_seesaw/pwmout.py` & `adafruit-circuitpython-seesaw-1.9.2/adafruit_seesaw/pwmout.py`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-seesaw-1.9.1/adafruit_seesaw/robohat.py` & `adafruit-circuitpython-seesaw-1.9.2/adafruit_seesaw/robohat.py`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-seesaw-1.9.1/adafruit_seesaw/rotaryio.py` & `adafruit-circuitpython-seesaw-1.9.2/adafruit_seesaw/rotaryio.py`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-seesaw-1.9.1/adafruit_seesaw/samd09.py` & `adafruit-circuitpython-seesaw-1.9.2/adafruit_seesaw/samd09.py`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-seesaw-1.9.1/adafruit_seesaw/seesaw.py` & `adafruit-circuitpython-seesaw-1.9.2/adafruit_seesaw/seesaw.py`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-seesaw-1.9.1/adafruit_seesaw/tftshield18.py` & `adafruit-circuitpython-seesaw-1.9.2/adafruit_seesaw/tftshield18.py`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-seesaw-1.9.1/docs/_static/favicon.ico` & `adafruit-circuitpython-seesaw-1.9.2/docs/_static/favicon.ico`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-seesaw-1.9.1/docs/api.rst` & `adafruit-circuitpython-seesaw-1.9.2/docs/api.rst`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-seesaw-1.9.1/docs/conf.py` & `adafruit-circuitpython-seesaw-1.9.2/docs/conf.py`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-seesaw-1.9.1/docs/examples.rst` & `adafruit-circuitpython-seesaw-1.9.2/docs/examples.rst`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-seesaw-1.9.1/docs/index.rst` & `adafruit-circuitpython-seesaw-1.9.2/docs/index.rst`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-seesaw-1.9.1/examples/seesaw_crickit_test.py` & `adafruit-circuitpython-seesaw-1.9.2/examples/seesaw_crickit_test.py`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-seesaw-1.9.1/examples/seesaw_joy_featherwing.py` & `adafruit-circuitpython-seesaw-1.9.2/examples/seesaw_joy_featherwing.py`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-seesaw-1.9.1/examples/seesaw_minitft_featherwing.py` & `adafruit-circuitpython-seesaw-1.9.2/examples/seesaw_minitft_featherwing.py`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-seesaw-1.9.1/examples/seesaw_rotary_neopixel.py` & `adafruit-circuitpython-seesaw-1.9.2/examples/seesaw_rotary_neopixel.py`

 * *Files 5% similar despite different names*

```diff
@@ -14,24 +14,27 @@
 # import busio
 # i2c = busio.I2C(board.SCL1, board.SDA1)
 # seesaw = seesaw.Seesaw(i2c, 0x36)
 
 seesaw = seesaw.Seesaw(board.I2C(), 0x36)
 
 encoder = rotaryio.IncrementalEncoder(seesaw)
+seesaw.pin_mode(24, seesaw.INPUT_PULLUP)
 switch = digitalio.DigitalIO(seesaw, 24)
 
 pixel = neopixel.NeoPixel(seesaw, 6, 1)
 pixel.brightness = 0.5
 
 last_position = -1
 color = 0  # start at red
 
 while True:
-    position = encoder.position
+
+    # negate the position to make clockwise rotation positive
+    position = -encoder.position
 
     if position != last_position:
         print(position)
 
         if switch.value:
             # Change the LED color.
             if position > last_position:  # Advance forward through the colorwheel.
```

### Comparing `adafruit-circuitpython-seesaw-1.9.1/examples/seesaw_simpletest.py` & `adafruit-circuitpython-seesaw-1.9.2/examples/seesaw_simpletest.py`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-seesaw-1.9.1/setup.py` & `adafruit-circuitpython-seesaw-1.9.2/setup.py`

 * *Files identical despite different names*

