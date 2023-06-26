# Comparing `tmp/adafruit-circuitpython-macropad-2.2.0.tar.gz` & `tmp/adafruit-circuitpython-macropad-2.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "adafruit-circuitpython-macropad-2.2.0.tar", last modified: Mon May  1 22:24:10 2023, max compression
+gzip compressed data, was "adafruit-circuitpython-macropad-2.2.1.tar", last modified: Mon Jun 26 18:03:25 2023, max compression
```

## Comparing `adafruit-circuitpython-macropad-2.2.0.tar` & `adafruit-circuitpython-macropad-2.2.1.tar`

### file list

```diff
@@ -1,71 +1,71 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 22:24:10.928958 adafruit-circuitpython-macropad-2.2.0/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 22:24:10.916957 adafruit-circuitpython-macropad-2.2.0/.github/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 22:24:10.920958 adafruit-circuitpython-macropad-2.2.0/.github/PULL_REQUEST_TEMPLATE/
--rw-r--r--   0 runner    (1001) docker     (123)      880 2023-05-01 22:23:45.000000 adafruit-circuitpython-macropad-2.2.0/.github/PULL_REQUEST_TEMPLATE/adafruit_circuitpython_pr.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 22:24:10.920958 adafruit-circuitpython-macropad-2.2.0/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)      303 2023-05-01 22:23:45.000000 adafruit-circuitpython-macropad-2.2.0/.github/workflows/build.yml
--rw-r--r--   0 runner    (1001) docker     (123)      479 2023-05-01 22:23:45.000000 adafruit-circuitpython-macropad-2.2.0/.github/workflows/failure-help-text.yml
--rw-r--r--   0 runner    (1001) docker     (123)      482 2023-05-01 22:23:45.000000 adafruit-circuitpython-macropad-2.2.0/.github/workflows/release_gh.yml
--rw-r--r--   0 runner    (1001) docker     (123)      475 2023-05-01 22:23:45.000000 adafruit-circuitpython-macropad-2.2.0/.github/workflows/release_pypi.yml
--rw-r--r--   0 runner    (1001) docker     (123)     1654 2023-05-01 22:23:45.000000 adafruit-circuitpython-macropad-2.2.0/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)     1239 2023-05-01 22:23:45.000000 adafruit-circuitpython-macropad-2.2.0/.pre-commit-config.yaml
--rw-r--r--   0 runner    (1001) docker     (123)    13069 2023-05-01 22:23:45.000000 adafruit-circuitpython-macropad-2.2.0/.pylintrc
--rw-r--r--   0 runner    (1001) docker     (123)      388 2023-05-01 22:23:45.000000 adafruit-circuitpython-macropad-2.2.0/.readthedocs.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     6753 2023-05-01 22:23:45.000000 adafruit-circuitpython-macropad-2.2.0/CODE_OF_CONDUCT.md
--rw-r--r--   0 runner    (1001) docker     (123)     1104 2023-05-01 22:23:45.000000 adafruit-circuitpython-macropad-2.2.0/LICENSE
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 22:24:10.920958 adafruit-circuitpython-macropad-2.2.0/LICENSES/
--rw-r--r--   0 runner    (1001) docker     (123)    16814 2023-05-01 22:23:45.000000 adafruit-circuitpython-macropad-2.2.0/LICENSES/CC-BY-4.0.txt
--rw-r--r--   0 runner    (1001) docker     (123)    18375 2023-05-01 22:23:45.000000 adafruit-circuitpython-macropad-2.2.0/LICENSES/CC-BY-SA-4.0.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1108 2023-05-01 22:23:45.000000 adafruit-circuitpython-macropad-2.2.0/LICENSES/MIT.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1211 2023-05-01 22:23:45.000000 adafruit-circuitpython-macropad-2.2.0/LICENSES/Unlicense.txt
--rw-r--r--   0 runner    (1001) docker     (123)     4818 2023-05-01 22:24:10.928958 adafruit-circuitpython-macropad-2.2.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     4042 2023-05-01 22:23:45.000000 adafruit-circuitpython-macropad-2.2.0/README.rst
--rw-r--r--   0 runner    (1001) docker     (123)      188 2023-05-01 22:23:45.000000 adafruit-circuitpython-macropad-2.2.0/README.rst.license
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 22:24:10.924958 adafruit-circuitpython-macropad-2.2.0/adafruit_circuitpython_macropad.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     4818 2023-05-01 22:24:10.000000 adafruit-circuitpython-macropad-2.2.0/adafruit_circuitpython_macropad.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1805 2023-05-01 22:24:10.000000 adafruit-circuitpython-macropad-2.2.0/adafruit_circuitpython_macropad.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-01 22:24:10.000000 adafruit-circuitpython-macropad-2.2.0/adafruit_circuitpython_macropad.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      227 2023-05-01 22:24:10.000000 adafruit-circuitpython-macropad-2.2.0/adafruit_circuitpython_macropad.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       18 2023-05-01 22:24:10.000000 adafruit-circuitpython-macropad-2.2.0/adafruit_circuitpython_macropad.egg-info/top_level.txt
--rwxr-xr-x   0 runner    (1001) docker     (123)    38207 2023-05-01 22:24:01.000000 adafruit-circuitpython-macropad-2.2.0/adafruit_macropad.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 22:24:10.924958 adafruit-circuitpython-macropad-2.2.0/docs/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 22:24:10.924958 adafruit-circuitpython-macropad-2.2.0/docs/_static/
--rw-r--r--   0 runner    (1001) docker     (123)     4414 2023-05-01 22:23:45.000000 adafruit-circuitpython-macropad-2.2.0/docs/_static/favicon.ico
--rw-r--r--   0 runner    (1001) docker     (123)      105 2023-05-01 22:23:45.000000 adafruit-circuitpython-macropad-2.2.0/docs/_static/favicon.ico.license
--rw-r--r--   0 runner    (1001) docker     (123)      431 2023-05-01 22:23:45.000000 adafruit-circuitpython-macropad-2.2.0/docs/api.rst
--rw-r--r--   0 runner    (1001) docker     (123)      189 2023-05-01 22:23:45.000000 adafruit-circuitpython-macropad-2.2.0/docs/api.rst.license
--rw-r--r--   0 runner    (1001) docker     (123)     6168 2023-05-01 22:23:45.000000 adafruit-circuitpython-macropad-2.2.0/docs/conf.py
--rw-r--r--   0 runner    (1001) docker     (123)      308 2023-05-01 22:23:45.000000 adafruit-circuitpython-macropad-2.2.0/docs/examples.rst
--rw-r--r--   0 runner    (1001) docker     (123)      189 2023-05-01 22:23:45.000000 adafruit-circuitpython-macropad-2.2.0/docs/examples.rst.license
--rw-r--r--   0 runner    (1001) docker     (123)     1123 2023-05-01 22:23:45.000000 adafruit-circuitpython-macropad-2.2.0/docs/index.rst
--rw-r--r--   0 runner    (1001) docker     (123)      189 2023-05-01 22:23:45.000000 adafruit-circuitpython-macropad-2.2.0/docs/index.rst.license
--rw-r--r--   0 runner    (1001) docker     (123)      186 2023-05-01 22:23:45.000000 adafruit-circuitpython-macropad-2.2.0/docs/requirements.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 22:24:10.928958 adafruit-circuitpython-macropad-2.2.0/examples/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 22:24:10.928958 adafruit-circuitpython-macropad-2.2.0/examples/macropad_display_image/
--rw-r--r--   0 runner    (1001) docker     (123)     1088 2023-05-01 22:23:45.000000 adafruit-circuitpython-macropad-2.2.0/examples/macropad_display_image/blinka.bmp
--rw-r--r--   0 runner    (1001) docker     (123)      122 2023-05-01 22:23:45.000000 adafruit-circuitpython-macropad-2.2.0/examples/macropad_display_image/blinka.bmp.license
--rw-r--r--   0 runner    (1001) docker     (123)      330 2023-05-01 22:24:01.000000 adafruit-circuitpython-macropad-2.2.0/examples/macropad_display_image/macropad_display_image.py
--rw-r--r--   0 runner    (1001) docker     (123)     1294 2023-05-01 22:24:01.000000 adafruit-circuitpython-macropad-2.2.0/examples/macropad_grid_layout.py
--rw-r--r--   0 runner    (1001) docker     (123)     1127 2023-05-01 22:24:01.000000 adafruit-circuitpython-macropad-2.2.0/examples/macropad_keyboard_layout.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1713 2023-05-01 22:24:01.000000 adafruit-circuitpython-macropad-2.2.0/examples/macropad_keyboard_mouse.py
--rw-r--r--   0 runner    (1001) docker     (123)      413 2023-05-01 22:24:01.000000 adafruit-circuitpython-macropad-2.2.0/examples/macropad_led_animation_example.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 22:24:10.928958 adafruit-circuitpython-macropad-2.2.0/examples/macropad_mp3/
--rw-r--r--   0 runner    (1001) docker     (123)    13920 2023-05-01 22:23:45.000000 adafruit-circuitpython-macropad-2.2.0/examples/macropad_mp3/beats.mp3
--rw-r--r--   0 runner    (1001) docker     (123)      123 2023-05-01 22:23:45.000000 adafruit-circuitpython-macropad-2.2.0/examples/macropad_mp3/beats.mp3.license
--rw-r--r--   0 runner    (1001) docker     (123)    24648 2023-05-01 22:23:45.000000 adafruit-circuitpython-macropad-2.2.0/examples/macropad_mp3/happy.mp3
--rw-r--r--   0 runner    (1001) docker     (123)      123 2023-05-01 22:23:45.000000 adafruit-circuitpython-macropad-2.2.0/examples/macropad_mp3/happy.mp3.license
--rw-r--r--   0 runner    (1001) docker     (123)     1107 2023-05-01 22:24:01.000000 adafruit-circuitpython-macropad-2.2.0/examples/macropad_mp3/macropad_mp3.py
--rw-r--r--   0 runner    (1001) docker     (123)    12696 2023-05-01 22:23:45.000000 adafruit-circuitpython-macropad-2.2.0/examples/macropad_mp3/slow.mp3
--rw-r--r--   0 runner    (1001) docker     (123)      123 2023-05-01 22:23:45.000000 adafruit-circuitpython-macropad-2.2.0/examples/macropad_mp3/slow.mp3.license
--rw-r--r--   0 runner    (1001) docker     (123)    35609 2023-05-01 22:23:45.000000 adafruit-circuitpython-macropad-2.2.0/examples/macropad_mp3/upbeats.mp3
--rw-r--r--   0 runner    (1001) docker     (123)      123 2023-05-01 22:23:45.000000 adafruit-circuitpython-macropad-2.2.0/examples/macropad_mp3/upbeats.mp3.license
--rw-r--r--   0 runner    (1001) docker     (123)     1938 2023-05-01 22:24:01.000000 adafruit-circuitpython-macropad-2.2.0/examples/macropad_rainbow_keys.py
--rw-r--r--   0 runner    (1001) docker     (123)      991 2023-05-01 22:24:01.000000 adafruit-circuitpython-macropad-2.2.0/examples/macropad_rotation.py
--rw-r--r--   0 runner    (1001) docker     (123)      661 2023-05-01 22:24:01.000000 adafruit-circuitpython-macropad-2.2.0/examples/macropad_simpletest.py
--rw-r--r--   0 runner    (1001) docker     (123)      833 2023-05-01 22:24:01.000000 adafruit-circuitpython-macropad-2.2.0/examples/macropad_simpletest_display.py
--rw-r--r--   0 runner    (1001) docker     (123)      801 2023-05-01 22:24:01.000000 adafruit-circuitpython-macropad-2.2.0/examples/macropad_tone_keypad.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     3535 2023-05-01 22:24:01.000000 adafruit-circuitpython-macropad-2.2.0/examples/macropad_tone_keypad_extended.py
--rw-r--r--   0 runner    (1001) docker     (123)      108 2023-05-01 22:23:45.000000 adafruit-circuitpython-macropad-2.2.0/optional_requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1238 2023-05-01 22:24:01.000000 adafruit-circuitpython-macropad-2.2.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)      324 2023-05-01 22:23:45.000000 adafruit-circuitpython-macropad-2.2.0/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-01 22:24:10.928958 adafruit-circuitpython-macropad-2.2.0/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 18:03:25.344708 adafruit-circuitpython-macropad-2.2.1/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 18:03:25.336708 adafruit-circuitpython-macropad-2.2.1/.github/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 18:03:25.336708 adafruit-circuitpython-macropad-2.2.1/.github/PULL_REQUEST_TEMPLATE/
+-rw-r--r--   0 runner    (1001) docker     (123)      880 2023-06-26 18:03:10.000000 adafruit-circuitpython-macropad-2.2.1/.github/PULL_REQUEST_TEMPLATE/adafruit_circuitpython_pr.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 18:03:25.336708 adafruit-circuitpython-macropad-2.2.1/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)      303 2023-06-26 18:03:10.000000 adafruit-circuitpython-macropad-2.2.1/.github/workflows/build.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      479 2023-06-26 18:03:10.000000 adafruit-circuitpython-macropad-2.2.1/.github/workflows/failure-help-text.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      482 2023-06-26 18:03:10.000000 adafruit-circuitpython-macropad-2.2.1/.github/workflows/release_gh.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      475 2023-06-26 18:03:10.000000 adafruit-circuitpython-macropad-2.2.1/.github/workflows/release_pypi.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1654 2023-06-26 18:03:10.000000 adafruit-circuitpython-macropad-2.2.1/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)     1238 2023-06-26 18:03:10.000000 adafruit-circuitpython-macropad-2.2.1/.pre-commit-config.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)    13078 2023-06-26 18:03:10.000000 adafruit-circuitpython-macropad-2.2.1/.pylintrc
+-rw-r--r--   0 runner    (1001) docker     (123)      388 2023-06-26 18:03:10.000000 adafruit-circuitpython-macropad-2.2.1/.readthedocs.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     6753 2023-06-26 18:03:10.000000 adafruit-circuitpython-macropad-2.2.1/CODE_OF_CONDUCT.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1104 2023-06-26 18:03:10.000000 adafruit-circuitpython-macropad-2.2.1/LICENSE
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 18:03:25.340708 adafruit-circuitpython-macropad-2.2.1/LICENSES/
+-rw-r--r--   0 runner    (1001) docker     (123)    16814 2023-06-26 18:03:10.000000 adafruit-circuitpython-macropad-2.2.1/LICENSES/CC-BY-4.0.txt
+-rw-r--r--   0 runner    (1001) docker     (123)    18375 2023-06-26 18:03:10.000000 adafruit-circuitpython-macropad-2.2.1/LICENSES/CC-BY-SA-4.0.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1108 2023-06-26 18:03:10.000000 adafruit-circuitpython-macropad-2.2.1/LICENSES/MIT.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1211 2023-06-26 18:03:10.000000 adafruit-circuitpython-macropad-2.2.1/LICENSES/Unlicense.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     4818 2023-06-26 18:03:25.344708 adafruit-circuitpython-macropad-2.2.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     4042 2023-06-26 18:03:10.000000 adafruit-circuitpython-macropad-2.2.1/README.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      188 2023-06-26 18:03:10.000000 adafruit-circuitpython-macropad-2.2.1/README.rst.license
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 18:03:25.340708 adafruit-circuitpython-macropad-2.2.1/adafruit_circuitpython_macropad.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     4818 2023-06-26 18:03:25.000000 adafruit-circuitpython-macropad-2.2.1/adafruit_circuitpython_macropad.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1805 2023-06-26 18:03:25.000000 adafruit-circuitpython-macropad-2.2.1/adafruit_circuitpython_macropad.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-26 18:03:25.000000 adafruit-circuitpython-macropad-2.2.1/adafruit_circuitpython_macropad.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      227 2023-06-26 18:03:25.000000 adafruit-circuitpython-macropad-2.2.1/adafruit_circuitpython_macropad.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       18 2023-06-26 18:03:25.000000 adafruit-circuitpython-macropad-2.2.1/adafruit_circuitpython_macropad.egg-info/top_level.txt
+-rwxr-xr-x   0 runner    (1001) docker     (123)    38355 2023-06-26 18:03:17.000000 adafruit-circuitpython-macropad-2.2.1/adafruit_macropad.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 18:03:25.340708 adafruit-circuitpython-macropad-2.2.1/docs/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 18:03:25.340708 adafruit-circuitpython-macropad-2.2.1/docs/_static/
+-rw-r--r--   0 runner    (1001) docker     (123)     4414 2023-06-26 18:03:10.000000 adafruit-circuitpython-macropad-2.2.1/docs/_static/favicon.ico
+-rw-r--r--   0 runner    (1001) docker     (123)      105 2023-06-26 18:03:10.000000 adafruit-circuitpython-macropad-2.2.1/docs/_static/favicon.ico.license
+-rw-r--r--   0 runner    (1001) docker     (123)      431 2023-06-26 18:03:10.000000 adafruit-circuitpython-macropad-2.2.1/docs/api.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      189 2023-06-26 18:03:10.000000 adafruit-circuitpython-macropad-2.2.1/docs/api.rst.license
+-rw-r--r--   0 runner    (1001) docker     (123)     6196 2023-06-26 18:03:10.000000 adafruit-circuitpython-macropad-2.2.1/docs/conf.py
+-rw-r--r--   0 runner    (1001) docker     (123)      308 2023-06-26 18:03:10.000000 adafruit-circuitpython-macropad-2.2.1/docs/examples.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      189 2023-06-26 18:03:10.000000 adafruit-circuitpython-macropad-2.2.1/docs/examples.rst.license
+-rw-r--r--   0 runner    (1001) docker     (123)     1123 2023-06-26 18:03:10.000000 adafruit-circuitpython-macropad-2.2.1/docs/index.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      189 2023-06-26 18:03:10.000000 adafruit-circuitpython-macropad-2.2.1/docs/index.rst.license
+-rw-r--r--   0 runner    (1001) docker     (123)      207 2023-06-26 18:03:10.000000 adafruit-circuitpython-macropad-2.2.1/docs/requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 18:03:25.340708 adafruit-circuitpython-macropad-2.2.1/examples/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 18:03:25.340708 adafruit-circuitpython-macropad-2.2.1/examples/macropad_display_image/
+-rw-r--r--   0 runner    (1001) docker     (123)     1088 2023-06-26 18:03:10.000000 adafruit-circuitpython-macropad-2.2.1/examples/macropad_display_image/blinka.bmp
+-rw-r--r--   0 runner    (1001) docker     (123)      122 2023-06-26 18:03:10.000000 adafruit-circuitpython-macropad-2.2.1/examples/macropad_display_image/blinka.bmp.license
+-rw-r--r--   0 runner    (1001) docker     (123)      330 2023-06-26 18:03:17.000000 adafruit-circuitpython-macropad-2.2.1/examples/macropad_display_image/macropad_display_image.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1294 2023-06-26 18:03:17.000000 adafruit-circuitpython-macropad-2.2.1/examples/macropad_grid_layout.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1127 2023-06-26 18:03:17.000000 adafruit-circuitpython-macropad-2.2.1/examples/macropad_keyboard_layout.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1713 2023-06-26 18:03:17.000000 adafruit-circuitpython-macropad-2.2.1/examples/macropad_keyboard_mouse.py
+-rw-r--r--   0 runner    (1001) docker     (123)      413 2023-06-26 18:03:17.000000 adafruit-circuitpython-macropad-2.2.1/examples/macropad_led_animation_example.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 18:03:25.344708 adafruit-circuitpython-macropad-2.2.1/examples/macropad_mp3/
+-rw-r--r--   0 runner    (1001) docker     (123)    13920 2023-06-26 18:03:10.000000 adafruit-circuitpython-macropad-2.2.1/examples/macropad_mp3/beats.mp3
+-rw-r--r--   0 runner    (1001) docker     (123)      123 2023-06-26 18:03:10.000000 adafruit-circuitpython-macropad-2.2.1/examples/macropad_mp3/beats.mp3.license
+-rw-r--r--   0 runner    (1001) docker     (123)    24648 2023-06-26 18:03:10.000000 adafruit-circuitpython-macropad-2.2.1/examples/macropad_mp3/happy.mp3
+-rw-r--r--   0 runner    (1001) docker     (123)      123 2023-06-26 18:03:10.000000 adafruit-circuitpython-macropad-2.2.1/examples/macropad_mp3/happy.mp3.license
+-rw-r--r--   0 runner    (1001) docker     (123)     1107 2023-06-26 18:03:17.000000 adafruit-circuitpython-macropad-2.2.1/examples/macropad_mp3/macropad_mp3.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12696 2023-06-26 18:03:10.000000 adafruit-circuitpython-macropad-2.2.1/examples/macropad_mp3/slow.mp3
+-rw-r--r--   0 runner    (1001) docker     (123)      123 2023-06-26 18:03:10.000000 adafruit-circuitpython-macropad-2.2.1/examples/macropad_mp3/slow.mp3.license
+-rw-r--r--   0 runner    (1001) docker     (123)    35609 2023-06-26 18:03:10.000000 adafruit-circuitpython-macropad-2.2.1/examples/macropad_mp3/upbeats.mp3
+-rw-r--r--   0 runner    (1001) docker     (123)      123 2023-06-26 18:03:10.000000 adafruit-circuitpython-macropad-2.2.1/examples/macropad_mp3/upbeats.mp3.license
+-rw-r--r--   0 runner    (1001) docker     (123)     1938 2023-06-26 18:03:17.000000 adafruit-circuitpython-macropad-2.2.1/examples/macropad_rainbow_keys.py
+-rw-r--r--   0 runner    (1001) docker     (123)      991 2023-06-26 18:03:17.000000 adafruit-circuitpython-macropad-2.2.1/examples/macropad_rotation.py
+-rw-r--r--   0 runner    (1001) docker     (123)      661 2023-06-26 18:03:17.000000 adafruit-circuitpython-macropad-2.2.1/examples/macropad_simpletest.py
+-rw-r--r--   0 runner    (1001) docker     (123)      833 2023-06-26 18:03:17.000000 adafruit-circuitpython-macropad-2.2.1/examples/macropad_simpletest_display.py
+-rw-r--r--   0 runner    (1001) docker     (123)      801 2023-06-26 18:03:17.000000 adafruit-circuitpython-macropad-2.2.1/examples/macropad_tone_keypad.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     3536 2023-06-26 18:03:17.000000 adafruit-circuitpython-macropad-2.2.1/examples/macropad_tone_keypad_extended.py
+-rw-r--r--   0 runner    (1001) docker     (123)      108 2023-06-26 18:03:10.000000 adafruit-circuitpython-macropad-2.2.1/optional_requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1238 2023-06-26 18:03:17.000000 adafruit-circuitpython-macropad-2.2.1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      324 2023-06-26 18:03:10.000000 adafruit-circuitpython-macropad-2.2.1/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-26 18:03:25.344708 adafruit-circuitpython-macropad-2.2.1/setup.cfg
```

### Comparing `adafruit-circuitpython-macropad-2.2.0/.github/PULL_REQUEST_TEMPLATE/adafruit_circuitpython_pr.md` & `adafruit-circuitpython-macropad-2.2.1/.github/PULL_REQUEST_TEMPLATE/adafruit_circuitpython_pr.md`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-macropad-2.2.0/.gitignore` & `adafruit-circuitpython-macropad-2.2.1/.gitignore`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-macropad-2.2.0/.pre-commit-config.yaml` & `adafruit-circuitpython-macropad-2.2.1/.pre-commit-config.yaml`

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

### Comparing `adafruit-circuitpython-macropad-2.2.0/.pylintrc` & `adafruit-circuitpython-macropad-2.2.1/.pylintrc`

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

### Comparing `adafruit-circuitpython-macropad-2.2.0/CODE_OF_CONDUCT.md` & `adafruit-circuitpython-macropad-2.2.1/CODE_OF_CONDUCT.md`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-macropad-2.2.0/LICENSE` & `adafruit-circuitpython-macropad-2.2.1/LICENSE`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-macropad-2.2.0/LICENSES/CC-BY-4.0.txt` & `adafruit-circuitpython-macropad-2.2.1/LICENSES/CC-BY-4.0.txt`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-macropad-2.2.0/LICENSES/CC-BY-SA-4.0.txt` & `adafruit-circuitpython-macropad-2.2.1/LICENSES/CC-BY-SA-4.0.txt`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-macropad-2.2.0/LICENSES/MIT.txt` & `adafruit-circuitpython-macropad-2.2.1/LICENSES/MIT.txt`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-macropad-2.2.0/LICENSES/Unlicense.txt` & `adafruit-circuitpython-macropad-2.2.1/LICENSES/Unlicense.txt`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-macropad-2.2.0/PKG-INFO` & `adafruit-circuitpython-macropad-2.2.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: adafruit-circuitpython-macropad
-Version: 2.2.0
+Version: 2.2.1
 Summary: A helper library for the Adafruit MacroPad RP2040
 Author-email: Adafruit Industries <circuitpython@adafruit.com>
 License: MIT
 Project-URL: Homepage, https://github.com/adafruit/Adafruit_CircuitPython_MacroPad
 Keywords: adafruit,macropad,rp2040,mechanical,keyboard,breakout,hardwaremicropython,circuitpython
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Software Development :: Libraries
```

### Comparing `adafruit-circuitpython-macropad-2.2.0/README.rst` & `adafruit-circuitpython-macropad-2.2.1/README.rst`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-macropad-2.2.0/adafruit_circuitpython_macropad.egg-info/PKG-INFO` & `adafruit-circuitpython-macropad-2.2.1/adafruit_circuitpython_macropad.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: adafruit-circuitpython-macropad
-Version: 2.2.0
+Version: 2.2.1
 Summary: A helper library for the Adafruit MacroPad RP2040
 Author-email: Adafruit Industries <circuitpython@adafruit.com>
 License: MIT
 Project-URL: Homepage, https://github.com/adafruit/Adafruit_CircuitPython_MacroPad
 Keywords: adafruit,macropad,rp2040,mechanical,keyboard,breakout,hardwaremicropython,circuitpython
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Software Development :: Libraries
```

### Comparing `adafruit-circuitpython-macropad-2.2.0/adafruit_circuitpython_macropad.egg-info/SOURCES.txt` & `adafruit-circuitpython-macropad-2.2.1/adafruit_circuitpython_macropad.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-macropad-2.2.0/adafruit_macropad.py` & `adafruit-circuitpython-macropad-2.2.1/adafruit_macropad.py`

 * *Files 1% similar despite different names*

```diff
@@ -81,22 +81,25 @@
     from typing import Tuple, Optional, Union, Iterator
     from neopixel import NeoPixel
     from keypad import Keys
     import adafruit_hid  # pylint:disable=ungrouped-imports
 except ImportError:
     pass
 
-__version__ = "2.2.0"
+__version__ = "2.2.1"
 __repo__ = "https://github.com/adafruit/Adafruit_CircuitPython_MacroPad.git"
 
 ROTATED_KEYMAP_0 = (0, 1, 2, 3, 4, 5, 6, 7, 8, 9, 10, 11)
 ROTATED_KEYMAP_90 = (2, 5, 8, 11, 1, 4, 7, 10, 0, 3, 6, 9)
 ROTATED_KEYMAP_180 = (11, 10, 9, 8, 7, 6, 5, 4, 3, 2, 1, 0)
 ROTATED_KEYMAP_270 = (9, 6, 3, 0, 10, 7, 4, 1, 11, 8, 5, 2)
 
+# See https://cdn-shop.adafruit.com/product-files/5228/5223-ds.pdf#page=13
+_DISPLAY_SLEEP_COMMAND = 0xAE
+_DISPLAY_WAKE_COMMAND = 0xAF
 
 keycodes = Keycode
 """Module level Keycode class, to be changed when initing Macropad with a different language"""
 
 
 class _PixelMapLite:
     """Generate a pixel map based on a specified order. Designed to work with a set of 12 pixels,
@@ -286,14 +289,15 @@
         self._encoder_switch.switch_to_input(pull=digitalio.Pull.UP)
         self._debounced_switch = Debouncer(self._encoder_switch)
 
         # Define display:
         if not isinstance(board.DISPLAY, type(None)):
             self.display = board.DISPLAY
             self.display.rotation = rotation
+            self.display.bus.send(_DISPLAY_WAKE_COMMAND, b"")
         self._display_sleep = False
 
         # Define audio:
         self._speaker_enable = digitalio.DigitalInOut(board.SPEAKER_ENABLE)
         self._speaker_enable.switch_to_output(value=False)
         self._sample = None
         self._sine_wave = None
@@ -336,19 +340,18 @@
         """
         return self._display_sleep
 
     @display_sleep.setter
     def display_sleep(self, sleep: bool) -> None:
         if self._display_sleep == sleep:
             return
-        # See https://cdn-shop.adafruit.com/product-files/5228/5223-ds.pdf#page=13
         if sleep:
-            command = 0xAE
+            command = _DISPLAY_SLEEP_COMMAND
         else:
-            command = 0xAF
+            command = _DISPLAY_WAKE_COMMAND
         self.display.bus.send(command, b"")
         self._display_sleep = sleep
 
     @property
     def pixels(self) -> Optional[_PixelMapLite]:
         """Sequence-like object representing the twelve NeoPixel LEDs in a 3 x 4 grid on the
         MacroPad. Each pixel is at a certain index in the sequence, numbered 0-11. Colors can be an
```

### Comparing `adafruit-circuitpython-macropad-2.2.0/docs/_static/favicon.ico` & `adafruit-circuitpython-macropad-2.2.1/docs/_static/favicon.ico`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-macropad-2.2.0/docs/conf.py` & `adafruit-circuitpython-macropad-2.2.1/docs/conf.py`

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

### Comparing `adafruit-circuitpython-macropad-2.2.0/docs/index.rst` & `adafruit-circuitpython-macropad-2.2.1/docs/index.rst`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-macropad-2.2.0/examples/macropad_display_image/blinka.bmp` & `adafruit-circuitpython-macropad-2.2.1/examples/macropad_display_image/blinka.bmp`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-macropad-2.2.0/examples/macropad_grid_layout.py` & `adafruit-circuitpython-macropad-2.2.1/examples/macropad_grid_layout.py`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-macropad-2.2.0/examples/macropad_keyboard_layout.py` & `adafruit-circuitpython-macropad-2.2.1/examples/macropad_keyboard_layout.py`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-macropad-2.2.0/examples/macropad_keyboard_mouse.py` & `adafruit-circuitpython-macropad-2.2.1/examples/macropad_keyboard_mouse.py`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-macropad-2.2.0/examples/macropad_mp3/beats.mp3` & `adafruit-circuitpython-macropad-2.2.1/examples/macropad_mp3/beats.mp3`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-macropad-2.2.0/examples/macropad_mp3/happy.mp3` & `adafruit-circuitpython-macropad-2.2.1/examples/macropad_mp3/happy.mp3`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-macropad-2.2.0/examples/macropad_mp3/macropad_mp3.py` & `adafruit-circuitpython-macropad-2.2.1/examples/macropad_mp3/macropad_mp3.py`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-macropad-2.2.0/examples/macropad_mp3/slow.mp3` & `adafruit-circuitpython-macropad-2.2.1/examples/macropad_mp3/slow.mp3`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-macropad-2.2.0/examples/macropad_mp3/upbeats.mp3` & `adafruit-circuitpython-macropad-2.2.1/examples/macropad_mp3/upbeats.mp3`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-macropad-2.2.0/examples/macropad_rainbow_keys.py` & `adafruit-circuitpython-macropad-2.2.1/examples/macropad_rainbow_keys.py`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-macropad-2.2.0/examples/macropad_rotation.py` & `adafruit-circuitpython-macropad-2.2.1/examples/macropad_rotation.py`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-macropad-2.2.0/examples/macropad_simpletest.py` & `adafruit-circuitpython-macropad-2.2.1/examples/macropad_simpletest.py`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-macropad-2.2.0/examples/macropad_simpletest_display.py` & `adafruit-circuitpython-macropad-2.2.1/examples/macropad_simpletest_display.py`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-macropad-2.2.0/examples/macropad_tone_keypad.py` & `adafruit-circuitpython-macropad-2.2.1/examples/macropad_tone_keypad.py`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-macropad-2.2.0/examples/macropad_tone_keypad_extended.py` & `adafruit-circuitpython-macropad-2.2.1/examples/macropad_tone_keypad_extended.py`

 * *Files 0% similar despite different names*

```diff
@@ -24,14 +24,15 @@
 # the order they were pressed.
 key_pressed_stack = []
 
 # When at least one key is pressed, this will
 # be the index of the currently playing note.
 playing_index = None
 
+
 # Helper to convert an integer to an rgb value.
 def rgb_from_int(rgb):
     blue = rgb & 255
     green = (rgb >> 8) & 255
     red = (rgb >> 16) & 255
     return red, green, blue
```

### Comparing `adafruit-circuitpython-macropad-2.2.0/pyproject.toml` & `adafruit-circuitpython-macropad-2.2.1/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -8,15 +8,15 @@
     "wheel",
     "setuptools-scm",
 ]
 
 [project]
 name = "adafruit-circuitpython-macropad"
 description = "A helper library for the Adafruit MacroPad RP2040"
-version = "2.2.0"
+version = "2.2.1"
 readme = "README.rst"
 authors = [
     {name = "Adafruit Industries", email = "circuitpython@adafruit.com"}
 ]
 urls = {Homepage = "https://github.com/adafruit/Adafruit_CircuitPython_MacroPad"}
 keywords = [
     "adafruit",
```

