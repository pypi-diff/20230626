# Comparing `tmp/pygac-1.7.1.tar.gz` & `tmp/pygac-1.7.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pygac-1.7.1.tar", last modified: Fri Dec  9 10:50:41 2022, max compression
+gzip compressed data, was "pygac-1.7.2.tar", last modified: Mon Jun 26 11:06:11 2023, max compression
```

## Comparing `pygac-1.7.1.tar` & `pygac-1.7.2.tar`

### file list

```diff
@@ -1,92 +1,94 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-09 10:50:41.779014 pygac-1.7.1/
--rw-r--r--   0 runner    (1001) docker     (123)      100 2022-12-09 10:50:37.000000 pygac-1.7.1/.bumpversion.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-09 10:50:41.771014 pygac-1.7.1/.github/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-09 10:50:41.775014 pygac-1.7.1/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)     1256 2022-12-09 10:50:37.000000 pygac-1.7.1/.github/workflows/ci.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      496 2022-12-09 10:50:37.000000 pygac-1.7.1/.github/workflows/deploy-sdist.yaml
--rw-r--r--   0 runner    (1001) docker     (123)       93 2022-12-09 10:50:37.000000 pygac-1.7.1/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)      189 2022-12-09 10:50:37.000000 pygac-1.7.1/.landscape.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      223 2022-12-09 10:50:37.000000 pygac-1.7.1/.pre-commit-config.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      362 2022-12-09 10:50:37.000000 pygac-1.7.1/.readthedocs.yml
--rw-r--r--   0 runner    (1001) docker     (123)       94 2022-12-09 10:50:37.000000 pygac-1.7.1/.stickler.yml
--rw-r--r--   0 runner    (1001) docker     (123)    12217 2022-12-09 10:50:37.000000 pygac-1.7.1/CHANGELOG.md
--rw-r--r--   0 runner    (1001) docker     (123)    35147 2022-12-09 10:50:37.000000 pygac-1.7.1/LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (123)      122 2022-12-09 10:50:37.000000 pygac-1.7.1/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     1275 2022-12-09 10:50:41.779014 pygac-1.7.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      608 2022-12-09 10:50:37.000000 pygac-1.7.1/README.md
--rw-r--r--   0 runner    (1001) docker     (123)     1789 2022-12-09 10:50:37.000000 pygac-1.7.1/RELEASING.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-09 10:50:41.775014 pygac-1.7.1/bin/
--rwxr-xr-x   0 runner    (1001) docker     (123)    14019 2022-12-09 10:50:37.000000 pygac-1.7.1/bin/pygac-convert-patmosx-coefficients
--rwxr-xr-x   0 runner    (1001) docker     (123)     5921 2022-12-09 10:50:37.000000 pygac-1.7.1/bin/pygac-run
--rw-r--r--   0 runner    (1001) docker     (123)     8701 2022-12-09 10:50:37.000000 pygac-1.7.1/changelog.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-09 10:50:41.775014 pygac-1.7.1/continuous_integration/
--rw-r--r--   0 runner    (1001) docker     (123)      286 2022-12-09 10:50:37.000000 pygac-1.7.1/continuous_integration/environment.yaml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-09 10:50:41.775014 pygac-1.7.1/doc/
--rw-r--r--   0 runner    (1001) docker     (123)     4590 2022-12-09 10:50:37.000000 pygac-1.7.1/doc/Makefile
--rw-r--r--   0 runner    (1001) docker     (123)      452 2022-12-09 10:50:37.000000 pygac-1.7.1/doc/rtd_environment.yaml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-09 10:50:41.775014 pygac-1.7.1/doc/source/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-09 10:50:41.775014 pygac-1.7.1/doc/source/_static/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2022-12-09 10:50:37.000000 pygac-1.7.1/doc/source/_static/.gitkeep
--rw-r--r--   0 runner    (1001) docker     (123)     1455 2022-12-09 10:50:37.000000 pygac-1.7.1/doc/source/api.rst
--rw-r--r--   0 runner    (1001) docker     (123)     7171 2022-12-09 10:50:37.000000 pygac-1.7.1/doc/source/conf.py
--rw-r--r--   0 runner    (1001) docker     (123)      640 2022-12-09 10:50:37.000000 pygac-1.7.1/doc/source/index.rst
--rw-r--r--   0 runner    (1001) docker     (123)     1358 2022-12-09 10:50:37.000000 pygac-1.7.1/doc/source/installation.rst
--rw-r--r--   0 runner    (1001) docker     (123)     1338 2022-12-09 10:50:37.000000 pygac-1.7.1/doc/source/introduction.rst
--rw-r--r--   0 runner    (1001) docker     (123)    15455 2022-12-09 10:50:37.000000 pygac-1.7.1/doc/source/legacy.rst
--rw-r--r--   0 runner    (1001) docker     (123)     7318 2022-12-09 10:50:37.000000 pygac-1.7.1/doc/source/methods.rst
--rw-r--r--   0 runner    (1001) docker     (123)     3576 2022-12-09 10:50:37.000000 pygac-1.7.1/doc/source/usage.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-09 10:50:41.775014 pygac-1.7.1/etc/
--rw-r--r--   0 runner    (1001) docker     (123)      126 2022-12-09 10:50:37.000000 pygac-1.7.1/etc/pygac.cfg.template
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-09 10:50:41.775014 pygac-1.7.1/gapfilled_tles/
--rw-r--r--   0 runner    (1001) docker     (123)  1308955 2022-12-09 10:50:37.000000 pygac-1.7.1/gapfilled_tles/TLE_noaa16.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-09 10:50:41.779014 pygac-1.7.1/pygac/
--rw-r--r--   0 runner    (1001) docker     (123)     1567 2022-12-09 10:50:37.000000 pygac-1.7.1/pygac/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    26499 2022-12-09 10:50:37.000000 pygac-1.7.1/pygac/calibration.py
--rw-r--r--   0 runner    (1001) docker     (123)    11033 2022-12-09 10:50:37.000000 pygac-1.7.1/pygac/clock_offsets_converter.py
--rw-r--r--   0 runner    (1001) docker     (123)     3395 2022-12-09 10:50:37.000000 pygac-1.7.1/pygac/configuration.py
--rw-r--r--   0 runner    (1001) docker     (123)    20117 2022-12-09 10:50:37.000000 pygac-1.7.1/pygac/correct_tsm_issue.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-09 10:50:41.779014 pygac-1.7.1/pygac/data/
--rw-r--r--   0 runner    (1001) docker     (123)    40666 2022-12-09 10:50:37.000000 pygac-1.7.1/pygac/data/calibration.json
--rw-r--r--   0 runner    (1001) docker     (123)    20619 2022-12-09 10:50:37.000000 pygac-1.7.1/pygac/gac_calibration.py_old
--rw-r--r--   0 runner    (1001) docker     (123)    27380 2022-12-09 10:50:37.000000 pygac-1.7.1/pygac/gac_io.py
--rw-r--r--   0 runner    (1001) docker     (123)    19076 2022-12-09 10:50:37.000000 pygac-1.7.1/pygac/gac_io.py_old
--rw-r--r--   0 runner    (1001) docker     (123)    10529 2022-12-09 10:50:37.000000 pygac-1.7.1/pygac/gac_klm.py
--rw-r--r--   0 runner    (1001) docker     (123)     2623 2022-12-09 10:50:37.000000 pygac-1.7.1/pygac/gac_pod.py
--rw-r--r--   0 runner    (1001) docker     (123)     2069 2022-12-09 10:50:37.000000 pygac-1.7.1/pygac/gac_reader.py
--rw-r--r--   0 runner    (1001) docker     (123)      737 2022-12-09 10:50:37.000000 pygac-1.7.1/pygac/investigate_bts1.m
--rw-r--r--   0 runner    (1001) docker     (123)    48323 2022-12-09 10:50:37.000000 pygac-1.7.1/pygac/klm_reader.py
--rw-r--r--   0 runner    (1001) docker     (123)    10611 2022-12-09 10:50:37.000000 pygac-1.7.1/pygac/lac_klm.py
--rw-r--r--   0 runner    (1001) docker     (123)     2573 2022-12-09 10:50:37.000000 pygac-1.7.1/pygac/lac_pod.py
--rw-r--r--   0 runner    (1001) docker     (123)     2091 2022-12-09 10:50:37.000000 pygac-1.7.1/pygac/lac_reader.py
--rw-r--r--   0 runner    (1001) docker     (123)    25035 2022-12-09 10:50:37.000000 pygac-1.7.1/pygac/pod_reader.py
--rw-r--r--   0 runner    (1001) docker     (123)     2239 2022-12-09 10:50:37.000000 pygac-1.7.1/pygac/pygac_geotiepoints.py
--rw-r--r--   0 runner    (1001) docker     (123)    44708 2022-12-09 10:50:37.000000 pygac-1.7.1/pygac/reader.py
--rw-r--r--   0 runner    (1001) docker     (123)     4236 2022-12-09 10:50:37.000000 pygac-1.7.1/pygac/runner.py
--rw-r--r--   0 runner    (1001) docker     (123)     1543 2022-12-09 10:50:37.000000 pygac-1.7.1/pygac/slerp.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-09 10:50:41.779014 pygac-1.7.1/pygac/tests/
--rw-r--r--   0 runner    (1001) docker     (123)      859 2022-12-09 10:50:37.000000 pygac-1.7.1/pygac/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2752 2022-12-09 10:50:37.000000 pygac-1.7.1/pygac/tests/test_angles.py
--rw-r--r--   0 runner    (1001) docker     (123)     5284 2022-12-09 10:50:37.000000 pygac-1.7.1/pygac/tests/test_calibrate_klm.py
--rw-r--r--   0 runner    (1001) docker     (123)     5261 2022-12-09 10:50:37.000000 pygac-1.7.1/pygac/tests/test_calibrate_pod.py
--rw-r--r--   0 runner    (1001) docker     (123)     6750 2022-12-09 10:50:37.000000 pygac-1.7.1/pygac/tests/test_calibration_coefficients.py
--rw-r--r--   0 runner    (1001) docker     (123)     9622 2022-12-09 10:50:37.000000 pygac-1.7.1/pygac/tests/test_io.py
--rw-r--r--   0 runner    (1001) docker     (123)     7131 2022-12-09 10:50:37.000000 pygac-1.7.1/pygac/tests/test_klm.py
--rw-r--r--   0 runner    (1001) docker     (123)    13068 2022-12-09 10:50:37.000000 pygac-1.7.1/pygac/tests/test_pod.py
--rw-r--r--   0 runner    (1001) docker     (123)    30010 2022-12-09 10:50:37.000000 pygac-1.7.1/pygac/tests/test_reader.py
--rw-r--r--   0 runner    (1001) docker     (123)     4434 2022-12-09 10:50:37.000000 pygac-1.7.1/pygac/tests/test_slerp.py
--rw-r--r--   0 runner    (1001) docker     (123)     3145 2022-12-09 10:50:37.000000 pygac-1.7.1/pygac/tests/test_tsm.py
--rw-r--r--   0 runner    (1001) docker     (123)     3921 2022-12-09 10:50:37.000000 pygac-1.7.1/pygac/tests/test_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     1073 2022-12-09 10:50:37.000000 pygac-1.7.1/pygac/tests/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)    11310 2022-12-09 10:50:37.000000 pygac-1.7.1/pygac/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)      176 2022-12-09 10:50:41.000000 pygac-1.7.1/pygac/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-09 10:50:41.779014 pygac-1.7.1/pygac.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1275 2022-12-09 10:50:41.000000 pygac-1.7.1/pygac.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1704 2022-12-09 10:50:41.000000 pygac-1.7.1/pygac.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2022-12-09 10:50:41.000000 pygac-1.7.1/pygac.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2022-12-09 10:50:41.000000 pygac-1.7.1/pygac.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)      147 2022-12-09 10:50:41.000000 pygac-1.7.1/pygac.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        6 2022-12-09 10:50:41.000000 pygac-1.7.1/pygac.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      206 2022-12-09 10:50:37.000000 pygac-1.7.1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       67 2022-12-09 10:50:37.000000 pygac-1.7.1/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)      143 2022-12-09 10:50:41.783014 pygac-1.7.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2716 2022-12-09 10:50:37.000000 pygac-1.7.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 11:06:11.312225 pygac-1.7.2/
+-rw-r--r--   0 runner    (1001) docker     (123)      100 2023-06-26 11:06:06.000000 pygac-1.7.2/.bumpversion.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 11:06:11.296225 pygac-1.7.2/.github/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 11:06:11.300225 pygac-1.7.2/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)     1256 2023-06-26 11:06:06.000000 pygac-1.7.2/.github/workflows/ci.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      496 2023-06-26 11:06:06.000000 pygac-1.7.2/.github/workflows/deploy-sdist.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)       93 2023-06-26 11:06:06.000000 pygac-1.7.2/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)      189 2023-06-26 11:06:06.000000 pygac-1.7.2/.landscape.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      223 2023-06-26 11:06:06.000000 pygac-1.7.2/.pre-commit-config.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      362 2023-06-26 11:06:06.000000 pygac-1.7.2/.readthedocs.yml
+-rw-r--r--   0 runner    (1001) docker     (123)       94 2023-06-26 11:06:06.000000 pygac-1.7.2/.stickler.yml
+-rw-r--r--   0 runner    (1001) docker     (123)    12731 2023-06-26 11:06:06.000000 pygac-1.7.2/CHANGELOG.md
+-rw-r--r--   0 runner    (1001) docker     (123)    35147 2023-06-26 11:06:06.000000 pygac-1.7.2/LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      122 2023-06-26 11:06:06.000000 pygac-1.7.2/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     1275 2023-06-26 11:06:11.312225 pygac-1.7.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      608 2023-06-26 11:06:06.000000 pygac-1.7.2/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1789 2023-06-26 11:06:06.000000 pygac-1.7.2/RELEASING.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 11:06:11.300225 pygac-1.7.2/bin/
+-rwxr-xr-x   0 runner    (1001) docker     (123)    14019 2023-06-26 11:06:06.000000 pygac-1.7.2/bin/pygac-convert-patmosx-coefficients
+-rwxr-xr-x   0 runner    (1001) docker     (123)     5921 2023-06-26 11:06:06.000000 pygac-1.7.2/bin/pygac-run
+-rw-r--r--   0 runner    (1001) docker     (123)     8701 2023-06-26 11:06:06.000000 pygac-1.7.2/changelog.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 11:06:11.300225 pygac-1.7.2/continuous_integration/
+-rw-r--r--   0 runner    (1001) docker     (123)      300 2023-06-26 11:06:06.000000 pygac-1.7.2/continuous_integration/environment.yaml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 11:06:11.300225 pygac-1.7.2/doc/
+-rw-r--r--   0 runner    (1001) docker     (123)     4590 2023-06-26 11:06:06.000000 pygac-1.7.2/doc/Makefile
+-rw-r--r--   0 runner    (1001) docker     (123)      452 2023-06-26 11:06:06.000000 pygac-1.7.2/doc/rtd_environment.yaml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 11:06:11.304225 pygac-1.7.2/doc/source/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 11:06:11.304225 pygac-1.7.2/doc/source/_static/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-26 11:06:06.000000 pygac-1.7.2/doc/source/_static/.gitkeep
+-rw-r--r--   0 runner    (1001) docker     (123)     1455 2023-06-26 11:06:06.000000 pygac-1.7.2/doc/source/api.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     7171 2023-06-26 11:06:06.000000 pygac-1.7.2/doc/source/conf.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 11:06:11.304225 pygac-1.7.2/doc/source/images/
+-rw-r--r--   0 runner    (1001) docker     (123)    29292 2023-06-26 11:06:06.000000 pygac-1.7.2/doc/source/images/noaa_class_preferences.png
+-rw-r--r--   0 runner    (1001) docker     (123)      640 2023-06-26 11:06:06.000000 pygac-1.7.2/doc/source/index.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1358 2023-06-26 11:06:06.000000 pygac-1.7.2/doc/source/installation.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1619 2023-06-26 11:06:06.000000 pygac-1.7.2/doc/source/introduction.rst
+-rw-r--r--   0 runner    (1001) docker     (123)    15455 2023-06-26 11:06:06.000000 pygac-1.7.2/doc/source/legacy.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     7318 2023-06-26 11:06:06.000000 pygac-1.7.2/doc/source/methods.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     3576 2023-06-26 11:06:06.000000 pygac-1.7.2/doc/source/usage.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 11:06:11.304225 pygac-1.7.2/etc/
+-rw-r--r--   0 runner    (1001) docker     (123)      126 2023-06-26 11:06:06.000000 pygac-1.7.2/etc/pygac.cfg.template
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 11:06:11.304225 pygac-1.7.2/gapfilled_tles/
+-rw-r--r--   0 runner    (1001) docker     (123)  1308955 2023-06-26 11:06:06.000000 pygac-1.7.2/gapfilled_tles/TLE_noaa16.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 11:06:11.308225 pygac-1.7.2/pygac/
+-rw-r--r--   0 runner    (1001) docker     (123)     1567 2023-06-26 11:06:06.000000 pygac-1.7.2/pygac/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    26499 2023-06-26 11:06:06.000000 pygac-1.7.2/pygac/calibration.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11033 2023-06-26 11:06:06.000000 pygac-1.7.2/pygac/clock_offsets_converter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3395 2023-06-26 11:06:06.000000 pygac-1.7.2/pygac/configuration.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20117 2023-06-26 11:06:06.000000 pygac-1.7.2/pygac/correct_tsm_issue.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 11:06:11.312225 pygac-1.7.2/pygac/data/
+-rw-r--r--   0 runner    (1001) docker     (123)    40666 2023-06-26 11:06:06.000000 pygac-1.7.2/pygac/data/calibration.json
+-rw-r--r--   0 runner    (1001) docker     (123)    20619 2023-06-26 11:06:06.000000 pygac-1.7.2/pygac/gac_calibration.py_old
+-rw-r--r--   0 runner    (1001) docker     (123)    27380 2023-06-26 11:06:06.000000 pygac-1.7.2/pygac/gac_io.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19076 2023-06-26 11:06:06.000000 pygac-1.7.2/pygac/gac_io.py_old
+-rw-r--r--   0 runner    (1001) docker     (123)    10529 2023-06-26 11:06:06.000000 pygac-1.7.2/pygac/gac_klm.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2623 2023-06-26 11:06:06.000000 pygac-1.7.2/pygac/gac_pod.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2069 2023-06-26 11:06:06.000000 pygac-1.7.2/pygac/gac_reader.py
+-rw-r--r--   0 runner    (1001) docker     (123)      737 2023-06-26 11:06:06.000000 pygac-1.7.2/pygac/investigate_bts1.m
+-rw-r--r--   0 runner    (1001) docker     (123)    48323 2023-06-26 11:06:06.000000 pygac-1.7.2/pygac/klm_reader.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10611 2023-06-26 11:06:06.000000 pygac-1.7.2/pygac/lac_klm.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2573 2023-06-26 11:06:06.000000 pygac-1.7.2/pygac/lac_pod.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2091 2023-06-26 11:06:06.000000 pygac-1.7.2/pygac/lac_reader.py
+-rw-r--r--   0 runner    (1001) docker     (123)    25039 2023-06-26 11:06:06.000000 pygac-1.7.2/pygac/pod_reader.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2239 2023-06-26 11:06:06.000000 pygac-1.7.2/pygac/pygac_geotiepoints.py
+-rw-r--r--   0 runner    (1001) docker     (123)    44693 2023-06-26 11:06:06.000000 pygac-1.7.2/pygac/reader.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4236 2023-06-26 11:06:06.000000 pygac-1.7.2/pygac/runner.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1543 2023-06-26 11:06:06.000000 pygac-1.7.2/pygac/slerp.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 11:06:11.312225 pygac-1.7.2/pygac/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)      859 2023-06-26 11:06:06.000000 pygac-1.7.2/pygac/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2752 2023-06-26 11:06:06.000000 pygac-1.7.2/pygac/tests/test_angles.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5284 2023-06-26 11:06:06.000000 pygac-1.7.2/pygac/tests/test_calibrate_klm.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5261 2023-06-26 11:06:06.000000 pygac-1.7.2/pygac/tests/test_calibrate_pod.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6750 2023-06-26 11:06:06.000000 pygac-1.7.2/pygac/tests/test_calibration_coefficients.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9622 2023-06-26 11:06:06.000000 pygac-1.7.2/pygac/tests/test_io.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7131 2023-06-26 11:06:06.000000 pygac-1.7.2/pygac/tests/test_klm.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13068 2023-06-26 11:06:06.000000 pygac-1.7.2/pygac/tests/test_pod.py
+-rw-r--r--   0 runner    (1001) docker     (123)    30010 2023-06-26 11:06:06.000000 pygac-1.7.2/pygac/tests/test_reader.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4434 2023-06-26 11:06:06.000000 pygac-1.7.2/pygac/tests/test_slerp.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3145 2023-06-26 11:06:06.000000 pygac-1.7.2/pygac/tests/test_tsm.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3921 2023-06-26 11:06:06.000000 pygac-1.7.2/pygac/tests/test_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1073 2023-06-26 11:06:06.000000 pygac-1.7.2/pygac/tests/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11310 2023-06-26 11:06:06.000000 pygac-1.7.2/pygac/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)      160 2023-06-26 11:06:11.000000 pygac-1.7.2/pygac/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 11:06:11.312225 pygac-1.7.2/pygac.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1275 2023-06-26 11:06:11.000000 pygac-1.7.2/pygac.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1749 2023-06-26 11:06:11.000000 pygac-1.7.2/pygac.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-26 11:06:11.000000 pygac-1.7.2/pygac.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-26 11:06:11.000000 pygac-1.7.2/pygac.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)      147 2023-06-26 11:06:11.000000 pygac-1.7.2/pygac.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        6 2023-06-26 11:06:11.000000 pygac-1.7.2/pygac.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      206 2023-06-26 11:06:06.000000 pygac-1.7.2/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       83 2023-06-26 11:06:06.000000 pygac-1.7.2/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      143 2023-06-26 11:06:11.312225 pygac-1.7.2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2716 2023-06-26 11:06:06.000000 pygac-1.7.2/setup.py
```

### Comparing `pygac-1.7.1/.github/workflows/ci.yaml` & `pygac-1.7.2/.github/workflows/ci.yaml`

 * *Files identical despite different names*

### Comparing `pygac-1.7.1/CHANGELOG.md` & `pygac-1.7.2/CHANGELOG.md`

 * *Files 1% similar despite different names*

```diff
@@ -1,7 +1,27 @@
+## Version 1.7.2 (2023/06/26)
+
+
+### Pull Requests Merged
+
+#### Bugs fixed
+
+* [PR 120](https://github.com/pytroll/pygac/pull/120) - Compatibility with numpy v1.24
+
+#### Features added
+
+* [PR 122](https://github.com/pytroll/pygac/pull/122) - Don't use deprecated distutils module.
+
+#### Documentation changes
+
+* [PR 123](https://github.com/pytroll/pygac/pull/123) - Update supported data formats in documentation ([2494](https://github.com/pytroll/satpy/issues/2494))
+
+In this release 3 pull requests were closed.
+
+
 ## Version 1.7.1 (2022/12/09)
 
 
 ### Pull Requests Merged
 
 #### Bugs fixed
```

### Comparing `pygac-1.7.1/LICENSE.txt` & `pygac-1.7.2/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `pygac-1.7.1/PKG-INFO` & `pygac-1.7.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pygac
-Version: 1.7.1
+Version: 1.7.2
 Summary: NOAA AVHRR GAC/LAC reader and calibration
 Home-page: https://github.com/pytroll/pygac
 Author: The Pytroll Team
 Author-email: pytroll@googlegroups.com
 License: GPLv3
 Platform: UNKNOWN
 Classifier: Development Status :: 4 - Beta
```

### Comparing `pygac-1.7.1/README.md` & `pygac-1.7.2/README.md`

 * *Files identical despite different names*

### Comparing `pygac-1.7.1/RELEASING.md` & `pygac-1.7.2/RELEASING.md`

 * *Files identical despite different names*

### Comparing `pygac-1.7.1/bin/pygac-convert-patmosx-coefficients` & `pygac-1.7.2/bin/pygac-convert-patmosx-coefficients`

 * *Files identical despite different names*

### Comparing `pygac-1.7.1/bin/pygac-run` & `pygac-1.7.2/bin/pygac-run`

 * *Files identical despite different names*

### Comparing `pygac-1.7.1/changelog.rst` & `pygac-1.7.2/changelog.rst`

 * *Files identical despite different names*

### Comparing `pygac-1.7.1/doc/Makefile` & `pygac-1.7.2/doc/Makefile`

 * *Files identical despite different names*

### Comparing `pygac-1.7.1/doc/source/api.rst` & `pygac-1.7.2/doc/source/api.rst`

 * *Files identical despite different names*

### Comparing `pygac-1.7.1/doc/source/conf.py` & `pygac-1.7.2/doc/source/conf.py`

 * *Files identical despite different names*

### Comparing `pygac-1.7.1/doc/source/index.rst` & `pygac-1.7.2/doc/source/index.rst`

 * *Files identical despite different names*

### Comparing `pygac-1.7.1/doc/source/installation.rst` & `pygac-1.7.2/doc/source/installation.rst`

 * *Files identical despite different names*

### Comparing `pygac-1.7.1/doc/source/introduction.rst` & `pygac-1.7.2/doc/source/introduction.rst`

 * *Files 22% similar despite different names*

```diff
@@ -6,14 +6,22 @@
 
 Pygac reads AVHRR GAC (Global Area Coverage), LAC (Local Area Coverage) and FRAC
 (Full Resolution Area Coverage) level 1b data from NOAA, which is described in
 the `POD`_ (NOAA-14 and before) and `KLM`_ (NOAA-15 and following) user guides.
 The data can be obtained from `NOAA CLASS`_, where you can also find a
 comprehensive `introduction`_.
 
+.. note::
+
+    Pygac can only read AVHRR data with 10 bits/pixel. This can be specified in
+    your NOAA CLASS order or user preferences (see screenshot below).
+
+.. image:: images/noaa_class_preferences.png
+    :width: 350
+    :alt: Screenshot of AVHRR data extraction preferences
 
 .. _NOAA CLASS:
     https://www.class.noaa.gov/
 .. _POD:
     https://www.ncei.noaa.gov/pub/data/satellite/publications/podguides/TIROS-N%20thru%20N-14/
 .. _KLM:
     https://www.ncei.noaa.gov/pub/data/satellite/publications/podguides/N-15%20thru%20N-19/
```

### Comparing `pygac-1.7.1/doc/source/legacy.rst` & `pygac-1.7.2/doc/source/legacy.rst`

 * *Files identical despite different names*

### Comparing `pygac-1.7.1/doc/source/methods.rst` & `pygac-1.7.2/doc/source/methods.rst`

 * *Files identical despite different names*

### Comparing `pygac-1.7.1/doc/source/usage.rst` & `pygac-1.7.2/doc/source/usage.rst`

 * *Files identical despite different names*

### Comparing `pygac-1.7.1/gapfilled_tles/TLE_noaa16.txt` & `pygac-1.7.2/gapfilled_tles/TLE_noaa16.txt`

 * *Files identical despite different names*

### Comparing `pygac-1.7.1/pygac/__init__.py` & `pygac-1.7.2/pygac/__init__.py`

 * *Files identical despite different names*

### Comparing `pygac-1.7.1/pygac/calibration.py` & `pygac-1.7.2/pygac/calibration.py`

 * *Files identical despite different names*

### Comparing `pygac-1.7.1/pygac/clock_offsets_converter.py` & `pygac-1.7.2/pygac/clock_offsets_converter.py`

 * *Files identical despite different names*

### Comparing `pygac-1.7.1/pygac/configuration.py` & `pygac-1.7.2/pygac/configuration.py`

 * *Files identical despite different names*

### Comparing `pygac-1.7.1/pygac/correct_tsm_issue.py` & `pygac-1.7.2/pygac/correct_tsm_issue.py`

 * *Files identical despite different names*

### Comparing `pygac-1.7.1/pygac/data/calibration.json` & `pygac-1.7.2/pygac/data/calibration.json`

 * *Files identical despite different names*

### Comparing `pygac-1.7.1/pygac/gac_calibration.py_old` & `pygac-1.7.2/pygac/gac_calibration.py_old`

 * *Files identical despite different names*

### Comparing `pygac-1.7.1/pygac/gac_io.py` & `pygac-1.7.2/pygac/gac_io.py`

 * *Files identical despite different names*

### Comparing `pygac-1.7.1/pygac/gac_io.py_old` & `pygac-1.7.2/pygac/gac_io.py_old`

 * *Files identical despite different names*

### Comparing `pygac-1.7.1/pygac/gac_klm.py` & `pygac-1.7.2/pygac/gac_klm.py`

 * *Files identical despite different names*

### Comparing `pygac-1.7.1/pygac/gac_pod.py` & `pygac-1.7.2/pygac/gac_pod.py`

 * *Files identical despite different names*

### Comparing `pygac-1.7.1/pygac/gac_reader.py` & `pygac-1.7.2/pygac/gac_reader.py`

 * *Files identical despite different names*

### Comparing `pygac-1.7.1/pygac/investigate_bts1.m` & `pygac-1.7.2/pygac/investigate_bts1.m`

 * *Files identical despite different names*

### Comparing `pygac-1.7.1/pygac/klm_reader.py` & `pygac-1.7.2/pygac/klm_reader.py`

 * *Files identical despite different names*

### Comparing `pygac-1.7.1/pygac/lac_klm.py` & `pygac-1.7.2/pygac/lac_klm.py`

 * *Files identical despite different names*

### Comparing `pygac-1.7.1/pygac/lac_pod.py` & `pygac-1.7.2/pygac/lac_pod.py`

 * *Files identical despite different names*

### Comparing `pygac-1.7.1/pygac/lac_reader.py` & `pygac-1.7.2/pygac/lac_reader.py`

 * *Files identical despite different names*

### Comparing `pygac-1.7.1/pygac/pod_reader.py` & `pygac-1.7.2/pygac/pod_reader.py`

 * *Files 0% similar despite different names*

```diff
@@ -494,17 +494,17 @@
             return
 
         # create arrays of lons and lats for interpolation. The locations
         # correspond to not yet corrected utcs, i.e. the time difference from
         # one line to the other should be equal to the scan rate.
         pixels_per_line = self.lats.shape[1]
         complete_lons = np.full((num_lines, pixels_per_line), np.nan,
-                                dtype=np.float)
+                                dtype=np.float64)
         complete_lats = np.full((num_lines, pixels_per_line), np.nan,
-                                dtype=np.float)
+                                dtype=np.float64)
 
         complete_lons[scan_lines - min_line] = self.lons
         complete_lats[scan_lines - min_line] = self.lats
         complete_lons[missed_lines - min_line] = missed_lons
         complete_lats[missed_lines - min_line] = missed_lats
 
         # perform the slerp interpolation to the corrected utc times
```

### Comparing `pygac-1.7.1/pygac/pygac_geotiepoints.py` & `pygac-1.7.2/pygac/pygac_geotiepoints.py`

 * *Files identical despite different names*

### Comparing `pygac-1.7.1/pygac/reader.py` & `pygac-1.7.2/pygac/reader.py`

 * *Files 1% similar despite different names*

```diff
@@ -39,15 +39,15 @@
 from pygac.utils import (centered_modulus,
                          calculate_sun_earth_distance_correction,
                          get_absolute_azimuth_angle_diff)
 from pyorbital.orbital import Orbital
 from pyorbital import astronomy
 from pygac.calibration import Calibrator, calibrate_solar, calibrate_thermal
 from pygac import gac_io
-from distutils.version import LooseVersion
+from packaging.version import Version
 
 LOG = logging.getLogger(__name__)
 
 # rpy values from
 # here:http://yyy.rsmas.miami.edu/groups/rrsl/pathfinder/Processing/proc_app_a.html
 rpy_coeffs = {
     'noaa7': {'roll': 0.000,
@@ -766,15 +766,15 @@
             self.lons[:, mid_column][:, np.newaxis],
             self.lats[:, mid_column][:, np.newaxis],  # approximate satellite position
             sat_alt,  # approximate satellite altitude
             self.times[:, np.newaxis],
             self.lons, self.lats, 0)
         # Sometimes (pyorbital <= 1.6.1) the get_observer_look_not_tle returns nodata instead of 90.
         # Problem solved with https://github.com/pytroll/pyorbital/pull/77
-        if LooseVersion(pyorbital.__version__) <= LooseVersion('1.6.1'):
+        if Version(pyorbital.__version__) <= Version('1.6.1'):
             sat_elev[:, mid_column] = 90
         return sat_azi, sat_elev
 
     def get_angles(self):
         """Get azimuth and zenith angles.
 
         Azimuth angle definition is the same as in pyorbital, but with
```

### Comparing `pygac-1.7.1/pygac/runner.py` & `pygac-1.7.2/pygac/runner.py`

 * *Files identical despite different names*

### Comparing `pygac-1.7.1/pygac/slerp.py` & `pygac-1.7.2/pygac/slerp.py`

 * *Files identical despite different names*

### Comparing `pygac-1.7.1/pygac/tests/__init__.py` & `pygac-1.7.2/pygac/tests/__init__.py`

 * *Files identical despite different names*

### Comparing `pygac-1.7.1/pygac/tests/test_angles.py` & `pygac-1.7.2/pygac/tests/test_angles.py`

 * *Files identical despite different names*

### Comparing `pygac-1.7.1/pygac/tests/test_calibrate_klm.py` & `pygac-1.7.2/pygac/tests/test_calibrate_klm.py`

 * *Files identical despite different names*

### Comparing `pygac-1.7.1/pygac/tests/test_calibrate_pod.py` & `pygac-1.7.2/pygac/tests/test_calibrate_pod.py`

 * *Files identical despite different names*

### Comparing `pygac-1.7.1/pygac/tests/test_calibration_coefficients.py` & `pygac-1.7.2/pygac/tests/test_calibration_coefficients.py`

 * *Files identical despite different names*

### Comparing `pygac-1.7.1/pygac/tests/test_io.py` & `pygac-1.7.2/pygac/tests/test_io.py`

 * *Files identical despite different names*

### Comparing `pygac-1.7.1/pygac/tests/test_klm.py` & `pygac-1.7.2/pygac/tests/test_klm.py`

 * *Files identical despite different names*

### Comparing `pygac-1.7.1/pygac/tests/test_pod.py` & `pygac-1.7.2/pygac/tests/test_pod.py`

 * *Files identical despite different names*

### Comparing `pygac-1.7.1/pygac/tests/test_reader.py` & `pygac-1.7.2/pygac/tests/test_reader.py`

 * *Files identical despite different names*

### Comparing `pygac-1.7.1/pygac/tests/test_slerp.py` & `pygac-1.7.2/pygac/tests/test_slerp.py`

 * *Files identical despite different names*

### Comparing `pygac-1.7.1/pygac/tests/test_tsm.py` & `pygac-1.7.2/pygac/tests/test_tsm.py`

 * *Files identical despite different names*

### Comparing `pygac-1.7.1/pygac/tests/test_utils.py` & `pygac-1.7.2/pygac/tests/test_utils.py`

 * *Files identical despite different names*

### Comparing `pygac-1.7.1/pygac/tests/utils.py` & `pygac-1.7.2/pygac/tests/utils.py`

 * *Files identical despite different names*

### Comparing `pygac-1.7.1/pygac/utils.py` & `pygac-1.7.2/pygac/utils.py`

 * *Files identical despite different names*

### Comparing `pygac-1.7.1/pygac.egg-info/PKG-INFO` & `pygac-1.7.2/pygac.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pygac
-Version: 1.7.1
+Version: 1.7.2
 Summary: NOAA AVHRR GAC/LAC reader and calibration
 Home-page: https://github.com/pytroll/pygac
 Author: The Pytroll Team
 Author-email: pytroll@googlegroups.com
 License: GPLv3
 Platform: UNKNOWN
 Classifier: Development Status :: 4 - Beta
```

### Comparing `pygac-1.7.1/pygac.egg-info/SOURCES.txt` & `pygac-1.7.2/pygac.egg-info/SOURCES.txt`

 * *Files 8% similar despite different names*

```diff
@@ -26,14 +26,15 @@
 doc/source/index.rst
 doc/source/installation.rst
 doc/source/introduction.rst
 doc/source/legacy.rst
 doc/source/methods.rst
 doc/source/usage.rst
 doc/source/_static/.gitkeep
+doc/source/images/noaa_class_preferences.png
 etc/pygac.cfg.template
 gapfilled_tles/TLE_noaa16.txt
 pygac/__init__.py
 pygac/calibration.py
 pygac/clock_offsets_converter.py
 pygac/configuration.py
 pygac/correct_tsm_issue.py
```

### Comparing `pygac-1.7.1/setup.py` & `pygac-1.7.2/setup.py`

 * *Files identical despite different names*

