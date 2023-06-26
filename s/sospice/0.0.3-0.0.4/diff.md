# Comparing `tmp/sospice-0.0.3.tar.gz` & `tmp/sospice-0.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sospice-0.0.3.tar", last modified: Thu Jun 22 21:36:06 2023, max compression
+gzip compressed data, was "sospice-0.0.4.tar", last modified: Mon Jun 26 14:44:13 2023, max compression
```

## Comparing `sospice-0.0.3.tar` & `sospice-0.0.4.tar`

### file list

```diff
@@ -1,81 +1,96 @@
-drwxrwxr-x   0 eric      (1001) eric      (1001)        0 2023-06-22 21:36:06.199324 sospice-0.0.3/
--rw-rw-r--   0 eric      (1001) eric      (1001)      112 2023-06-22 21:35:39.000000 sospice-0.0.3/.flake8
-drwxrwxr-x   0 eric      (1001) eric      (1001)        0 2023-06-22 21:36:06.191320 sospice-0.0.3/.github/
-drwxrwxr-x   0 eric      (1001) eric      (1001)        0 2023-06-22 21:36:06.191320 sospice-0.0.3/.github/workflows/
--rw-rw-r--   0 eric      (1001) eric      (1001)     1313 2023-06-20 07:30:27.000000 sospice-0.0.3/.github/workflows/python-package.yml
--rw-rw-r--   0 eric      (1001) eric      (1001)     3130 2023-06-22 21:35:39.000000 sospice-0.0.3/.gitignore
--rw-rw-r--   0 eric      (1001) eric      (1001)      931 2023-06-03 17:29:19.000000 sospice-0.0.3/.pre-commit-config.yaml
--rw-rw-r--   0 eric      (1001) eric      (1001)     1483 2023-04-28 17:14:31.000000 sospice-0.0.3/LICENSE
--rw-rw-r--   0 eric      (1001) eric      (1001)      467 2023-06-22 21:35:39.000000 sospice-0.0.3/Makefile
--rw-rw-r--   0 eric      (1001) eric      (1001)     3313 2023-06-22 21:36:06.199324 sospice-0.0.3/PKG-INFO
--rw-rw-r--   0 eric      (1001) eric      (1001)     2461 2023-06-22 21:35:39.000000 sospice-0.0.3/README.rst
-drwxrwxr-x   0 eric      (1001) eric      (1001)        0 2023-06-22 21:36:06.191320 sospice-0.0.3/docs/
--rw-rw-r--   0 eric      (1001) eric      (1001)      638 2023-04-26 09:59:38.000000 sospice-0.0.3/docs/Makefile
--rw-rw-r--   0 eric      (1001) eric      (1001)      804 2023-04-26 09:59:38.000000 sospice-0.0.3/docs/make.bat
-drwxrwxr-x   0 eric      (1001) eric      (1001)        0 2023-06-22 21:36:06.195322 sospice-0.0.3/docs/source/
-drwxrwxr-x   0 eric      (1001) eric      (1001)        0 2023-06-22 21:36:06.191320 sospice-0.0.3/docs/source/_templates/
-drwxrwxr-x   0 eric      (1001) eric      (1001)        0 2023-06-22 21:36:06.195322 sospice-0.0.3/docs/source/_templates/autosummary/
--rw-rw-r--   0 eric      (1001) eric      (1001)       77 2023-06-22 21:35:39.000000 sospice-0.0.3/docs/source/_templates/autosummary/module.rst
--rw-rw-r--   0 eric      (1001) eric      (1001)      259 2023-06-22 21:35:39.000000 sospice-0.0.3/docs/source/api.rst
--rw-rw-r--   0 eric      (1001) eric      (1001)      201 2023-06-05 21:42:41.000000 sospice-0.0.3/docs/source/changelog.rst
--rw-rw-r--   0 eric      (1001) eric      (1001)       40 2023-06-05 21:42:41.000000 sospice-0.0.3/docs/source/citation.rst
--rw-rw-r--   0 eric      (1001) eric      (1001)     3465 2023-06-22 21:35:39.000000 sospice-0.0.3/docs/source/conf.py
--rw-rw-r--   0 eric      (1001) eric      (1001)     5558 2023-06-05 21:42:41.000000 sospice-0.0.3/docs/source/develop.rst
--rw-rw-r--   0 eric      (1001) eric      (1001)      394 2023-06-05 21:42:41.000000 sospice-0.0.3/docs/source/getting_started.rst
--rw-rw-r--   0 eric      (1001) eric      (1001)     1076 2023-06-22 09:32:46.000000 sospice-0.0.3/docs/source/index.rst
-drwxrwxr-x   0 eric      (1001) eric      (1001)        0 2023-06-22 21:36:06.195322 sospice-0.0.3/examples/
--rw-rw-r--   0 eric      (1001) eric      (1001)      104 2023-04-26 09:59:38.000000 sospice-0.0.3/examples/README.md
--rw-rw-r--   0 eric      (1001) eric      (1001)     1381 2023-06-22 21:35:39.000000 sospice-0.0.3/pyproject.toml
--rw-rw-r--   0 eric      (1001) eric      (1001)      254 2023-06-22 21:35:39.000000 sospice-0.0.3/requirements.txt
--rw-rw-r--   0 eric      (1001) eric      (1001)       38 2023-06-22 21:36:06.199324 sospice-0.0.3/setup.cfg
-drwxrwxr-x   0 eric      (1001) eric      (1001)        0 2023-06-22 21:36:06.195322 sospice-0.0.3/sospice/
--rw-rw-r--   0 eric      (1001) eric      (1001)      283 2023-06-13 15:46:15.000000 sospice-0.0.3/sospice/CITATION.rst
--rw-rw-r--   0 eric      (1001) eric      (1001)      100 2023-06-22 21:34:09.000000 sospice-0.0.3/sospice/__init__.py
-drwxrwxr-x   0 eric      (1001) eric      (1001)        0 2023-06-22 21:36:06.195322 sospice-0.0.3/sospice/calibrate/
--rw-rw-r--   0 eric      (1001) eric      (1001)       39 2023-05-29 22:03:18.000000 sospice-0.0.3/sospice/calibrate/__init__.py
-drwxrwxr-x   0 eric      (1001) eric      (1001)        0 2023-06-22 21:36:06.195322 sospice-0.0.3/sospice/calibrate/tests/
--rw-rw-r--   0 eric      (1001) eric      (1001)        0 2023-04-26 09:59:38.000000 sospice-0.0.3/sospice/calibrate/tests/__init__.py
--rw-rw-r--   0 eric      (1001) eric      (1001)     2228 2023-06-03 14:31:07.000000 sospice-0.0.3/sospice/calibrate/tests/test_uncertainties.py
--rw-rw-r--   0 eric      (1001) eric      (1001)     1525 2023-06-03 17:30:17.000000 sospice-0.0.3/sospice/calibrate/uncertainties.py
-drwxrwxr-x   0 eric      (1001) eric      (1001)        0 2023-06-22 21:36:06.195322 sospice-0.0.3/sospice/catalog/
--rw-rw-r--   0 eric      (1001) eric      (1001)       58 2023-06-22 21:35:39.000000 sospice-0.0.3/sospice/catalog/__init__.py
--rw-rw-r--   0 eric      (1001) eric      (1001)     5485 2023-06-22 21:35:39.000000 sospice-0.0.3/sospice/catalog/catalog.py
--rw-rw-r--   0 eric      (1001) eric      (1001)     1890 2023-06-22 21:35:39.000000 sospice-0.0.3/sospice/catalog/release.py
-drwxrwxr-x   0 eric      (1001) eric      (1001)        0 2023-06-22 21:36:06.195322 sospice-0.0.3/sospice/catalog/tests/
--rw-rw-r--   0 eric      (1001) eric      (1001)        0 2023-04-26 09:59:38.000000 sospice-0.0.3/sospice/catalog/tests/__init__.py
--rw-rw-r--   0 eric      (1001) eric      (1001)     3638 2023-06-22 21:35:39.000000 sospice-0.0.3/sospice/catalog/tests/test_catalog.py
--rw-rw-r--   0 eric      (1001) eric      (1001)      975 2023-06-22 21:35:39.000000 sospice-0.0.3/sospice/catalog/tests/test_release.py
-drwxrwxr-x   0 eric      (1001) eric      (1001)        0 2023-06-22 21:36:06.195322 sospice-0.0.3/sospice/data/
--rw-rw-r--   0 eric      (1001) eric      (1001)        0 2023-04-26 09:59:38.000000 sospice-0.0.3/sospice/data/__init__.py
-drwxrwxr-x   0 eric      (1001) eric      (1001)        0 2023-06-22 21:36:06.195322 sospice-0.0.3/sospice/data/calibration/
--rw-rw-r--   0 eric      (1001) eric      (1001)     2708 2023-05-12 20:53:10.000000 sospice-0.0.3/sospice/data/calibration/effective_area.sav
-drwxrwxr-x   0 eric      (1001) eric      (1001)        0 2023-06-22 21:36:06.195322 sospice-0.0.3/sospice/data/tests/
--rw-rw-r--   0 eric      (1001) eric      (1001)        0 2023-04-26 09:59:38.000000 sospice-0.0.3/sospice/data/tests/__init__.py
-drwxrwxr-x   0 eric      (1001) eric      (1001)        0 2023-06-22 21:36:06.195322 sospice-0.0.3/sospice/instrument_modelling/
--rw-rw-r--   0 eric      (1001) eric      (1001)       87 2023-06-14 09:12:07.000000 sospice-0.0.3/sospice/instrument_modelling/__init__.py
--rw-rw-r--   0 eric      (1001) eric      (1001)     5983 2023-05-31 21:34:22.000000 sospice-0.0.3/sospice/instrument_modelling/observation.py
--rw-rw-r--   0 eric      (1001) eric      (1001)     4801 2023-06-01 21:25:28.000000 sospice-0.0.3/sospice/instrument_modelling/spice.py
--rw-rw-r--   0 eric      (1001) eric      (1001)     1666 2023-05-30 07:01:03.000000 sospice-0.0.3/sospice/instrument_modelling/study.py
-drwxrwxr-x   0 eric      (1001) eric      (1001)        0 2023-06-22 21:36:06.199324 sospice-0.0.3/sospice/instrument_modelling/tests/
--rw-rw-r--   0 eric      (1001) eric      (1001)        0 2023-05-12 21:08:37.000000 sospice-0.0.3/sospice/instrument_modelling/tests/__init__.py
--rw-rw-r--   0 eric      (1001) eric      (1001)     2720 2023-05-31 22:03:33.000000 sospice-0.0.3/sospice/instrument_modelling/tests/test_observation.py
--rw-rw-r--   0 eric      (1001) eric      (1001)     3183 2023-05-30 07:01:03.000000 sospice-0.0.3/sospice/instrument_modelling/tests/test_spice.py
--rw-rw-r--   0 eric      (1001) eric      (1001)     1473 2023-05-30 07:01:03.000000 sospice-0.0.3/sospice/instrument_modelling/tests/test_study.py
-drwxrwxr-x   0 eric      (1001) eric      (1001)        0 2023-06-22 21:36:06.199324 sospice-0.0.3/sospice/psf/
--rw-rw-r--   0 eric      (1001) eric      (1001)        0 2023-04-26 09:59:38.000000 sospice-0.0.3/sospice/psf/__init__.py
-drwxrwxr-x   0 eric      (1001) eric      (1001)        0 2023-06-22 21:36:06.199324 sospice-0.0.3/sospice/psf/tests/
--rw-rw-r--   0 eric      (1001) eric      (1001)        0 2023-04-26 09:59:38.000000 sospice-0.0.3/sospice/psf/tests/__init__.py
-drwxrwxr-x   0 eric      (1001) eric      (1001)        0 2023-06-22 21:36:06.199324 sospice-0.0.3/sospice/tests/
--rw-rw-r--   0 eric      (1001) eric      (1001)        0 2023-04-26 14:38:35.000000 sospice-0.0.3/sospice/tests/__init__.py
-drwxrwxr-x   0 eric      (1001) eric      (1001)        0 2023-06-22 21:36:06.199324 sospice-0.0.3/sospice/util/
--rw-rw-r--   0 eric      (1001) eric      (1001)       21 2023-05-13 07:03:48.000000 sospice-0.0.3/sospice/util/__init__.py
--rw-rw-r--   0 eric      (1001) eric      (1001)      405 2023-05-30 06:42:04.000000 sospice-0.0.3/sospice/util/rss.py
-drwxrwxr-x   0 eric      (1001) eric      (1001)        0 2023-06-22 21:36:06.199324 sospice-0.0.3/sospice/util/tests/
--rw-rw-r--   0 eric      (1001) eric      (1001)        0 2023-04-26 09:59:38.000000 sospice-0.0.3/sospice/util/tests/__init__.py
--rw-rw-r--   0 eric      (1001) eric      (1001)      316 2023-06-01 22:04:59.000000 sospice-0.0.3/sospice/util/tests/test_rss.py
-drwxrwxr-x   0 eric      (1001) eric      (1001)        0 2023-06-22 21:36:06.195322 sospice-0.0.3/sospice.egg-info/
--rw-rw-r--   0 eric      (1001) eric      (1001)     3313 2023-06-22 21:36:06.000000 sospice-0.0.3/sospice.egg-info/PKG-INFO
--rw-rw-r--   0 eric      (1001) eric      (1001)     1583 2023-06-22 21:36:06.000000 sospice-0.0.3/sospice.egg-info/SOURCES.txt
--rw-rw-r--   0 eric      (1001) eric      (1001)        1 2023-06-22 21:36:06.000000 sospice-0.0.3/sospice.egg-info/dependency_links.txt
--rw-rw-r--   0 eric      (1001) eric      (1001)      254 2023-06-22 21:36:06.000000 sospice-0.0.3/sospice.egg-info/requires.txt
--rw-rw-r--   0 eric      (1001) eric      (1001)        8 2023-06-22 21:36:06.000000 sospice-0.0.3/sospice.egg-info/top_level.txt
+drwxrwxr-x   0 eric      (1001) eric      (1001)        0 2023-06-26 14:44:13.831052 sospice-0.0.4/
+-rw-rw-r--   0 eric      (1001) eric      (1001)      112 2023-06-22 21:53:26.000000 sospice-0.0.4/.flake8
+drwxrwxr-x   0 eric      (1001) eric      (1001)        0 2023-06-26 14:44:13.807052 sospice-0.0.4/.github/
+drwxrwxr-x   0 eric      (1001) eric      (1001)        0 2023-06-26 14:44:13.811052 sospice-0.0.4/.github/workflows/
+-rw-rw-r--   0 eric      (1001) eric      (1001)     1313 2023-06-20 07:30:27.000000 sospice-0.0.4/.github/workflows/python-package.yml
+-rw-rw-r--   0 eric      (1001) eric      (1001)     3152 2023-06-26 13:51:54.000000 sospice-0.0.4/.gitignore
+-rw-rw-r--   0 eric      (1001) eric      (1001)      931 2023-06-03 17:29:19.000000 sospice-0.0.4/.pre-commit-config.yaml
+-rw-rw-r--   0 eric      (1001) eric      (1001)     1483 2023-04-28 17:14:31.000000 sospice-0.0.4/LICENSE
+-rw-rw-r--   0 eric      (1001) eric      (1001)      473 2023-06-26 13:53:18.000000 sospice-0.0.4/Makefile
+-rw-rw-r--   0 eric      (1001) eric      (1001)     3310 2023-06-26 14:44:13.831052 sospice-0.0.4/PKG-INFO
+-rw-rw-r--   0 eric      (1001) eric      (1001)     2458 2023-06-22 21:53:26.000000 sospice-0.0.4/README.rst
+drwxrwxr-x   0 eric      (1001) eric      (1001)        0 2023-06-26 14:44:13.811052 sospice-0.0.4/docs/
+-rw-rw-r--   0 eric      (1001) eric      (1001)      638 2023-04-26 09:59:38.000000 sospice-0.0.4/docs/Makefile
+-rw-rw-r--   0 eric      (1001) eric      (1001)      804 2023-04-26 09:59:38.000000 sospice-0.0.4/docs/make.bat
+drwxrwxr-x   0 eric      (1001) eric      (1001)        0 2023-06-26 14:44:13.815052 sospice-0.0.4/docs/source/
+drwxrwxr-x   0 eric      (1001) eric      (1001)        0 2023-06-26 14:44:13.807052 sospice-0.0.4/docs/source/_templates/
+drwxrwxr-x   0 eric      (1001) eric      (1001)        0 2023-06-26 14:44:13.815052 sospice-0.0.4/docs/source/_templates/autosummary/
+-rw-rw-r--   0 eric      (1001) eric      (1001)       77 2023-06-22 21:53:26.000000 sospice-0.0.4/docs/source/_templates/autosummary/module.rst
+-rw-rw-r--   0 eric      (1001) eric      (1001)      259 2023-06-22 21:53:26.000000 sospice-0.0.4/docs/source/api.rst
+-rw-rw-r--   0 eric      (1001) eric      (1001)      201 2023-06-05 21:42:41.000000 sospice-0.0.4/docs/source/changelog.rst
+-rw-rw-r--   0 eric      (1001) eric      (1001)       40 2023-06-05 21:42:41.000000 sospice-0.0.4/docs/source/citation.rst
+-rw-rw-r--   0 eric      (1001) eric      (1001)     3465 2023-06-22 21:53:26.000000 sospice-0.0.4/docs/source/conf.py
+-rw-rw-r--   0 eric      (1001) eric      (1001)     5558 2023-06-05 21:42:41.000000 sospice-0.0.4/docs/source/develop.rst
+-rw-rw-r--   0 eric      (1001) eric      (1001)      389 2023-06-22 21:53:26.000000 sospice-0.0.4/docs/source/getting_started.rst
+-rw-rw-r--   0 eric      (1001) eric      (1001)     1076 2023-06-22 09:32:46.000000 sospice-0.0.4/docs/source/index.rst
+drwxrwxr-x   0 eric      (1001) eric      (1001)        0 2023-06-26 14:44:13.815052 sospice-0.0.4/examples/
+-rw-rw-r--   0 eric      (1001) eric      (1001)      104 2023-04-26 09:59:38.000000 sospice-0.0.4/examples/README.md
+-rw-rw-r--   0 eric      (1001) eric      (1001)     1467 2023-06-26 14:43:54.000000 sospice-0.0.4/pyproject.toml
+-rw-rw-r--   0 eric      (1001) eric      (1001)      254 2023-06-22 21:53:26.000000 sospice-0.0.4/requirements.txt
+-rw-rw-r--   0 eric      (1001) eric      (1001)       38 2023-06-26 14:44:13.831052 sospice-0.0.4/setup.cfg
+drwxrwxr-x   0 eric      (1001) eric      (1001)        0 2023-06-26 14:44:13.815052 sospice-0.0.4/sospice/
+-rw-rw-r--   0 eric      (1001) eric      (1001)      283 2023-06-13 15:46:15.000000 sospice-0.0.4/sospice/CITATION.rst
+-rw-rw-r--   0 eric      (1001) eric      (1001)      129 2023-06-26 13:51:37.000000 sospice-0.0.4/sospice/__init__.py
+-rw-rw-r--   0 eric      (1001) eric      (1001)      214 2023-06-26 14:44:13.000000 sospice-0.0.4/sospice/_version.py
+drwxrwxr-x   0 eric      (1001) eric      (1001)        0 2023-06-26 14:44:13.815052 sospice-0.0.4/sospice/calibrate/
+-rw-rw-r--   0 eric      (1001) eric      (1001)       39 2023-05-29 22:03:18.000000 sospice-0.0.4/sospice/calibrate/__init__.py
+drwxrwxr-x   0 eric      (1001) eric      (1001)        0 2023-06-26 14:44:13.815052 sospice-0.0.4/sospice/calibrate/tests/
+-rw-rw-r--   0 eric      (1001) eric      (1001)        0 2023-04-26 09:59:38.000000 sospice-0.0.4/sospice/calibrate/tests/__init__.py
+-rw-rw-r--   0 eric      (1001) eric      (1001)     2228 2023-06-03 14:31:07.000000 sospice-0.0.4/sospice/calibrate/tests/test_uncertainties.py
+-rw-rw-r--   0 eric      (1001) eric      (1001)     1525 2023-06-03 17:30:17.000000 sospice-0.0.4/sospice/calibrate/uncertainties.py
+drwxrwxr-x   0 eric      (1001) eric      (1001)        0 2023-06-26 14:44:13.819052 sospice-0.0.4/sospice/catalog/
+-rw-rw-r--   0 eric      (1001) eric      (1001)       58 2023-06-22 21:53:26.000000 sospice-0.0.4/sospice/catalog/__init__.py
+-rw-rw-r--   0 eric      (1001) eric      (1001)     5485 2023-06-22 21:53:26.000000 sospice-0.0.4/sospice/catalog/catalog.py
+-rw-rw-r--   0 eric      (1001) eric      (1001)     1890 2023-06-22 21:53:26.000000 sospice-0.0.4/sospice/catalog/release.py
+drwxrwxr-x   0 eric      (1001) eric      (1001)        0 2023-06-26 14:44:13.819052 sospice-0.0.4/sospice/catalog/tests/
+-rw-rw-r--   0 eric      (1001) eric      (1001)        0 2023-04-26 09:59:38.000000 sospice-0.0.4/sospice/catalog/tests/__init__.py
+-rw-rw-r--   0 eric      (1001) eric      (1001)     3638 2023-06-22 21:53:26.000000 sospice-0.0.4/sospice/catalog/tests/test_catalog.py
+-rw-rw-r--   0 eric      (1001) eric      (1001)      975 2023-06-22 21:53:26.000000 sospice-0.0.4/sospice/catalog/tests/test_release.py
+drwxrwxr-x   0 eric      (1001) eric      (1001)        0 2023-06-26 14:44:13.819052 sospice-0.0.4/sospice/data/
+-rw-rw-r--   0 eric      (1001) eric      (1001)        0 2023-04-26 09:59:38.000000 sospice-0.0.4/sospice/data/__init__.py
+drwxrwxr-x   0 eric      (1001) eric      (1001)        0 2023-06-26 14:44:13.819052 sospice-0.0.4/sospice/data/calibration/
+-rw-rw-r--   0 eric      (1001) eric      (1001)     2708 2023-05-12 20:53:10.000000 sospice-0.0.4/sospice/data/calibration/effective_area.sav
+drwxrwxr-x   0 eric      (1001) eric      (1001)        0 2023-06-26 14:44:13.819052 sospice-0.0.4/sospice/data/tests/
+-rw-rw-r--   0 eric      (1001) eric      (1001)        0 2023-04-26 09:59:38.000000 sospice-0.0.4/sospice/data/tests/__init__.py
+drwxrwxr-x   0 eric      (1001) eric      (1001)        0 2023-06-26 14:44:13.819052 sospice-0.0.4/sospice/instrument_modelling/
+-rw-rw-r--   0 eric      (1001) eric      (1001)       87 2023-06-14 09:12:07.000000 sospice-0.0.4/sospice/instrument_modelling/__init__.py
+-rw-rw-r--   0 eric      (1001) eric      (1001)     5983 2023-05-31 21:34:22.000000 sospice-0.0.4/sospice/instrument_modelling/observation.py
+-rw-rw-r--   0 eric      (1001) eric      (1001)     4801 2023-06-01 21:25:28.000000 sospice-0.0.4/sospice/instrument_modelling/spice.py
+-rw-rw-r--   0 eric      (1001) eric      (1001)     1666 2023-05-30 07:01:03.000000 sospice-0.0.4/sospice/instrument_modelling/study.py
+drwxrwxr-x   0 eric      (1001) eric      (1001)        0 2023-06-26 14:44:13.819052 sospice-0.0.4/sospice/instrument_modelling/tests/
+-rw-rw-r--   0 eric      (1001) eric      (1001)        0 2023-05-12 21:08:37.000000 sospice-0.0.4/sospice/instrument_modelling/tests/__init__.py
+-rw-rw-r--   0 eric      (1001) eric      (1001)     2720 2023-05-31 22:03:33.000000 sospice-0.0.4/sospice/instrument_modelling/tests/test_observation.py
+-rw-rw-r--   0 eric      (1001) eric      (1001)     3183 2023-05-30 07:01:03.000000 sospice-0.0.4/sospice/instrument_modelling/tests/test_spice.py
+-rw-rw-r--   0 eric      (1001) eric      (1001)     1473 2023-05-30 07:01:03.000000 sospice-0.0.4/sospice/instrument_modelling/tests/test_study.py
+drwxrwxr-x   0 eric      (1001) eric      (1001)        0 2023-06-26 14:44:13.819052 sospice-0.0.4/sospice/psf/
+-rw-rw-r--   0 eric      (1001) eric      (1001)        0 2023-04-26 09:59:38.000000 sospice-0.0.4/sospice/psf/__init__.py
+drwxrwxr-x   0 eric      (1001) eric      (1001)        0 2023-06-26 14:44:13.819052 sospice-0.0.4/sospice/psf/tests/
+-rw-rw-r--   0 eric      (1001) eric      (1001)        0 2023-04-26 09:59:38.000000 sospice-0.0.4/sospice/psf/tests/__init__.py
+drwxrwxr-x   0 eric      (1001) eric      (1001)        0 2023-06-26 14:44:13.819052 sospice-0.0.4/sospice/tests/
+-rw-rw-r--   0 eric      (1001) eric      (1001)        0 2023-04-26 14:38:35.000000 sospice-0.0.4/sospice/tests/__init__.py
+drwxrwxr-x   0 eric      (1001) eric      (1001)        0 2023-06-26 14:44:13.819052 sospice-0.0.4/sospice/util/
+-rw-rw-r--   0 eric      (1001) eric      (1001)       21 2023-05-13 07:03:48.000000 sospice-0.0.4/sospice/util/__init__.py
+-rw-rw-r--   0 eric      (1001) eric      (1001)      405 2023-05-30 06:42:04.000000 sospice-0.0.4/sospice/util/rss.py
+drwxrwxr-x   0 eric      (1001) eric      (1001)        0 2023-06-26 14:44:13.819052 sospice-0.0.4/sospice/util/tests/
+-rw-rw-r--   0 eric      (1001) eric      (1001)        0 2023-04-26 09:59:38.000000 sospice-0.0.4/sospice/util/tests/__init__.py
+-rw-rw-r--   0 eric      (1001) eric      (1001)      316 2023-06-01 22:04:59.000000 sospice-0.0.4/sospice/util/tests/test_rss.py
+drwxrwxr-x   0 eric      (1001) eric      (1001)        0 2023-06-26 14:44:13.815052 sospice-0.0.4/sospice.egg-info/
+-rw-rw-r--   0 eric      (1001) eric      (1001)     3310 2023-06-26 14:44:13.000000 sospice-0.0.4/sospice.egg-info/PKG-INFO
+-rw-rw-r--   0 eric      (1001) eric      (1001)     1872 2023-06-26 14:44:13.000000 sospice-0.0.4/sospice.egg-info/SOURCES.txt
+-rw-rw-r--   0 eric      (1001) eric      (1001)        1 2023-06-26 14:44:13.000000 sospice-0.0.4/sospice.egg-info/dependency_links.txt
+-rw-rw-r--   0 eric      (1001) eric      (1001)      254 2023-06-26 14:44:13.000000 sospice-0.0.4/sospice.egg-info/requires.txt
+-rw-rw-r--   0 eric      (1001) eric      (1001)       40 2023-06-26 14:44:13.000000 sospice-0.0.4/sospice.egg-info/top_level.txt
+drwxrwxr-x   0 eric      (1001) eric      (1001)        0 2023-06-26 14:44:13.811052 sospice-0.0.4/venv/
+drwxrwxr-x   0 eric      (1001) eric      (1001)        0 2023-06-26 14:44:13.831052 sospice-0.0.4/venv/bin/
+-rwxrwxr-x   0 eric      (1001) eric      (1001)      637 2023-04-26 09:14:39.000000 sospice-0.0.4/venv/bin/rst2html.py
+-rwxrwxr-x   0 eric      (1001) eric      (1001)      759 2023-04-26 09:14:39.000000 sospice-0.0.4/venv/bin/rst2html4.py
+-rwxrwxr-x   0 eric      (1001) eric      (1001)     1104 2023-04-26 09:14:39.000000 sospice-0.0.4/venv/bin/rst2html5.py
+-rwxrwxr-x   0 eric      (1001) eric      (1001)      836 2023-04-26 09:14:39.000000 sospice-0.0.4/venv/bin/rst2latex.py
+-rwxrwxr-x   0 eric      (1001) eric      (1001)      659 2023-04-26 09:14:39.000000 sospice-0.0.4/venv/bin/rst2man.py
+-rwxrwxr-x   0 eric      (1001) eric      (1001)      825 2023-04-26 09:14:39.000000 sospice-0.0.4/venv/bin/rst2odt.py
+-rwxrwxr-x   0 eric      (1001) eric      (1001)     1763 2023-04-26 09:14:39.000000 sospice-0.0.4/venv/bin/rst2odt_prepstyles.py
+-rwxrwxr-x   0 eric      (1001) eric      (1001)      644 2023-04-26 09:14:39.000000 sospice-0.0.4/venv/bin/rst2pseudoxml.py
+-rwxrwxr-x   0 eric      (1001) eric      (1001)      680 2023-04-26 09:14:39.000000 sospice-0.0.4/venv/bin/rst2s5.py
+-rwxrwxr-x   0 eric      (1001) eric      (1001)      916 2023-04-26 09:14:39.000000 sospice-0.0.4/venv/bin/rst2xetex.py
+-rwxrwxr-x   0 eric      (1001) eric      (1001)      645 2023-04-26 09:14:39.000000 sospice-0.0.4/venv/bin/rst2xml.py
+-rwxrwxr-x   0 eric      (1001) eric      (1001)      713 2023-04-26 09:14:39.000000 sospice-0.0.4/venv/bin/rstpep2html.py
```

### Comparing `sospice-0.0.3/.github/workflows/python-package.yml` & `sospice-0.0.4/.github/workflows/python-package.yml`

 * *Files identical despite different names*

### Comparing `sospice-0.0.3/.gitignore` & `sospice-0.0.4/.gitignore`

 * *Files 2% similar despite different names*

```diff
@@ -158,7 +158,10 @@
 #  be found at https://github.com/github/gitignore/blob/main/Global/JetBrains.gitignore
 #  and can be added to the global gitignore or merged into this file.  For a more nuclear
 #  option (not recommended) you can uncomment the following to ignore the entire idea folder.
 .idea/
 
 # Editors backup files
 *~
+
+# Local files
+local/
```

### Comparing `sospice-0.0.3/.pre-commit-config.yaml` & `sospice-0.0.4/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `sospice-0.0.3/LICENSE` & `sospice-0.0.4/LICENSE`

 * *Files identical despite different names*

### Comparing `sospice-0.0.3/PKG-INFO` & `sospice-0.0.4/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sospice
-Version: 0.0.3
+Version: 0.0.4
 Summary: Python data analysis tools for Solar Orbiter/SPICE
 Author-email: SPICE consortium <spice-github.ias@universite-paris-saclay.fr>
 Project-URL: Homepage, https://github.com/solo-spice/sospice/
 Project-URL: Bug Tracker, https://github.com/solo-spice/sospice/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
@@ -41,16 +41,16 @@
 -  Calibration: ``calibrate``
 
    -  ``spice_error``: Computation of uncertainties on data, coming from
       different noise components.
 
 - Catalog: ``catalog``
 
-   - ``Catalog``: access and read catalog, find files in catalog.
-   - ``Release```: find and access releases.
+   -  ``Catalog``: access and read catalog, find files in catalog.
+   -  ``Release```: find and access releases.
 
 -  Instrument modelling: ``instrument_modelling``
 
    -  ``Spice``: instrument calibration parameters, effective area,
       quantum efficiency…
    -  ``Study``: study parameters.
    -  ``Observation``: a SPICE observation with some study (including
@@ -58,15 +58,15 @@
       data).
 
 Package philosophy
 ------------------
 
 We want ``sospice`` to be:
 
--  Convenient to install. It is installable by ``pip`` and it will be
+-  Convenient to install. It is installable by ``pip`` and it is
    published on `PyPI <https://pypi.org/>`__
 -  Useful, providing a single package for all SPICE-specific steps of
    your data analysis.
 -  Easy to use, with simple interface functions to operations performed
    by lower-level functions.
 -  Well documented. We use ``sphinx`` to build documentation from the
    Python docstrings.
```

### Comparing `sospice-0.0.3/README.rst` & `sospice-0.0.4/README.rst`

 * *Files 1% similar despite different names*

```diff
@@ -21,16 +21,16 @@
 -  Calibration: ``calibrate``
 
    -  ``spice_error``: Computation of uncertainties on data, coming from
       different noise components.
 
 - Catalog: ``catalog``
 
-   - ``Catalog``: access and read catalog, find files in catalog.
-   - ``Release```: find and access releases.
+   -  ``Catalog``: access and read catalog, find files in catalog.
+   -  ``Release```: find and access releases.
 
 -  Instrument modelling: ``instrument_modelling``
 
    -  ``Spice``: instrument calibration parameters, effective area,
       quantum efficiency…
    -  ``Study``: study parameters.
    -  ``Observation``: a SPICE observation with some study (including
@@ -38,15 +38,15 @@
       data).
 
 Package philosophy
 ------------------
 
 We want ``sospice`` to be:
 
--  Convenient to install. It is installable by ``pip`` and it will be
+-  Convenient to install. It is installable by ``pip`` and it is
    published on `PyPI <https://pypi.org/>`__
 -  Useful, providing a single package for all SPICE-specific steps of
    your data analysis.
 -  Easy to use, with simple interface functions to operations performed
    by lower-level functions.
 -  Well documented. We use ``sphinx`` to build documentation from the
    Python docstrings.
```

### Comparing `sospice-0.0.3/docs/Makefile` & `sospice-0.0.4/docs/Makefile`

 * *Files identical despite different names*

### Comparing `sospice-0.0.3/docs/make.bat` & `sospice-0.0.4/docs/make.bat`

 * *Files identical despite different names*

### Comparing `sospice-0.0.3/docs/source/conf.py` & `sospice-0.0.4/docs/source/conf.py`

 * *Files identical despite different names*

### Comparing `sospice-0.0.3/docs/source/develop.rst` & `sospice-0.0.4/docs/source/develop.rst`

 * *Files identical despite different names*

### Comparing `sospice-0.0.3/docs/source/index.rst` & `sospice-0.0.4/docs/source/index.rst`

 * *Files identical despite different names*

### Comparing `sospice-0.0.3/pyproject.toml` & `sospice-0.0.4/pyproject.toml`

 * *Files 4% similar despite different names*

```diff
@@ -19,22 +19,26 @@
     "Operating System :: OS Independent",
     "Development Status :: 3 - Alpha",
     "Intended Audience :: Science/Research",
     "Topic :: Scientific/Engineering :: Astronomy",
 ]
 dynamic = ["version", "dependencies"]
 
+[tool.setuptools.packages.find]
+exclude = ["local"]
+
 [tool.setuptools.dynamic]
 version = {attr = "sospice.__version__"}
 dependencies = {file = ["requirements.txt"]}
 
 #[project.optional-dependencies]
 #docs = ["sphinx"]
 
 [tool.setuptools_scm]
+write_to = "sospice/_version.py"
 
 [project.urls]
 "Homepage" = "https://github.com/solo-spice/sospice/"
 "Bug Tracker" = "https://github.com/solo-spice/sospice/issues"
 
 [tool.black]
 include = '\.pyi?$'
```

### Comparing `sospice-0.0.3/sospice/calibrate/tests/test_uncertainties.py` & `sospice-0.0.4/sospice/calibrate/tests/test_uncertainties.py`

 * *Files identical despite different names*

### Comparing `sospice-0.0.3/sospice/calibrate/uncertainties.py` & `sospice-0.0.4/sospice/calibrate/uncertainties.py`

 * *Files identical despite different names*

### Comparing `sospice-0.0.3/sospice/catalog/catalog.py` & `sospice-0.0.4/sospice/catalog/catalog.py`

 * *Files identical despite different names*

### Comparing `sospice-0.0.3/sospice/catalog/release.py` & `sospice-0.0.4/sospice/catalog/release.py`

 * *Files identical despite different names*

### Comparing `sospice-0.0.3/sospice/catalog/tests/test_catalog.py` & `sospice-0.0.4/sospice/catalog/tests/test_catalog.py`

 * *Files identical despite different names*

### Comparing `sospice-0.0.3/sospice/catalog/tests/test_release.py` & `sospice-0.0.4/sospice/catalog/tests/test_release.py`

 * *Files identical despite different names*

### Comparing `sospice-0.0.3/sospice/data/calibration/effective_area.sav` & `sospice-0.0.4/sospice/data/calibration/effective_area.sav`

 * *Files identical despite different names*

### Comparing `sospice-0.0.3/sospice/instrument_modelling/observation.py` & `sospice-0.0.4/sospice/instrument_modelling/observation.py`

 * *Files identical despite different names*

### Comparing `sospice-0.0.3/sospice/instrument_modelling/spice.py` & `sospice-0.0.4/sospice/instrument_modelling/spice.py`

 * *Files identical despite different names*

### Comparing `sospice-0.0.3/sospice/instrument_modelling/study.py` & `sospice-0.0.4/sospice/instrument_modelling/study.py`

 * *Files identical despite different names*

### Comparing `sospice-0.0.3/sospice/instrument_modelling/tests/test_observation.py` & `sospice-0.0.4/sospice/instrument_modelling/tests/test_observation.py`

 * *Files identical despite different names*

### Comparing `sospice-0.0.3/sospice/instrument_modelling/tests/test_spice.py` & `sospice-0.0.4/sospice/instrument_modelling/tests/test_spice.py`

 * *Files identical despite different names*

### Comparing `sospice-0.0.3/sospice/instrument_modelling/tests/test_study.py` & `sospice-0.0.4/sospice/instrument_modelling/tests/test_study.py`

 * *Files identical despite different names*

### Comparing `sospice-0.0.3/sospice.egg-info/PKG-INFO` & `sospice-0.0.4/sospice.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sospice
-Version: 0.0.3
+Version: 0.0.4
 Summary: Python data analysis tools for Solar Orbiter/SPICE
 Author-email: SPICE consortium <spice-github.ias@universite-paris-saclay.fr>
 Project-URL: Homepage, https://github.com/solo-spice/sospice/
 Project-URL: Bug Tracker, https://github.com/solo-spice/sospice/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
@@ -41,16 +41,16 @@
 -  Calibration: ``calibrate``
 
    -  ``spice_error``: Computation of uncertainties on data, coming from
       different noise components.
 
 - Catalog: ``catalog``
 
-   - ``Catalog``: access and read catalog, find files in catalog.
-   - ``Release```: find and access releases.
+   -  ``Catalog``: access and read catalog, find files in catalog.
+   -  ``Release```: find and access releases.
 
 -  Instrument modelling: ``instrument_modelling``
 
    -  ``Spice``: instrument calibration parameters, effective area,
       quantum efficiency…
    -  ``Study``: study parameters.
    -  ``Observation``: a SPICE observation with some study (including
@@ -58,15 +58,15 @@
       data).
 
 Package philosophy
 ------------------
 
 We want ``sospice`` to be:
 
--  Convenient to install. It is installable by ``pip`` and it will be
+-  Convenient to install. It is installable by ``pip`` and it is
    published on `PyPI <https://pypi.org/>`__
 -  Useful, providing a single package for all SPICE-specific steps of
    your data analysis.
 -  Easy to use, with simple interface functions to operations performed
    by lower-level functions.
 -  Well documented. We use ``sphinx`` to build documentation from the
    Python docstrings.
```

### Comparing `sospice-0.0.3/sospice.egg-info/SOURCES.txt` & `sospice-0.0.4/sospice.egg-info/SOURCES.txt`

 * *Files 18% similar despite different names*

```diff
@@ -16,14 +16,15 @@
 docs/source/develop.rst
 docs/source/getting_started.rst
 docs/source/index.rst
 docs/source/_templates/autosummary/module.rst
 examples/README.md
 sospice/CITATION.rst
 sospice/__init__.py
+sospice/_version.py
 sospice.egg-info/PKG-INFO
 sospice.egg-info/SOURCES.txt
 sospice.egg-info/dependency_links.txt
 sospice.egg-info/requires.txt
 sospice.egg-info/top_level.txt
 sospice/calibrate/__init__.py
 sospice/calibrate/uncertainties.py
@@ -48,8 +49,20 @@
 sospice/instrument_modelling/tests/test_study.py
 sospice/psf/__init__.py
 sospice/psf/tests/__init__.py
 sospice/tests/__init__.py
 sospice/util/__init__.py
 sospice/util/rss.py
 sospice/util/tests/__init__.py
-sospice/util/tests/test_rss.py
+sospice/util/tests/test_rss.py
+venv/bin/rst2html.py
+venv/bin/rst2html4.py
+venv/bin/rst2html5.py
+venv/bin/rst2latex.py
+venv/bin/rst2man.py
+venv/bin/rst2odt.py
+venv/bin/rst2odt_prepstyles.py
+venv/bin/rst2pseudoxml.py
+venv/bin/rst2s5.py
+venv/bin/rst2xetex.py
+venv/bin/rst2xml.py
+venv/bin/rstpep2html.py
```

