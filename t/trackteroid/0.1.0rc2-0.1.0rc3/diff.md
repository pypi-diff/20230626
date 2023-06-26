# Comparing `tmp/trackteroid-0.1.0rc2.tar.gz` & `tmp/trackteroid-0.1.0rc3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "trackteroid-0.1.0rc2.tar", last modified: Tue Jun 20 16:01:03 2023, max compression
+gzip compressed data, was "trackteroid-0.1.0rc3.tar", last modified: Mon Jun 26 09:05:37 2023, max compression
```

## Comparing `trackteroid-0.1.0rc2.tar` & `trackteroid-0.1.0rc3.tar`

### file list

```diff
@@ -1,78 +1,79 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 16:01:03.187090 trackteroid-0.1.0rc2/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 16:01:03.175089 trackteroid-0.1.0rc2/.github/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 16:01:03.179089 trackteroid-0.1.0rc2/.github/ISSUE_TEMPLATE/
--rw-r--r--   0 runner    (1001) docker     (123)      913 2023-06-20 16:00:51.000000 trackteroid-0.1.0rc2/.github/ISSUE_TEMPLATE/issue--bug-report.md
--rw-r--r--   0 runner    (1001) docker     (123)      547 2023-06-20 16:00:51.000000 trackteroid-0.1.0rc2/.github/ISSUE_TEMPLATE/issue--feature-request.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 16:01:03.179089 trackteroid-0.1.0rc2/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)     1084 2023-06-20 16:00:51.000000 trackteroid-0.1.0rc2/.github/workflows/python-publish.yml
--rw-r--r--   0 runner    (1001) docker     (123)       51 2023-06-20 16:00:51.000000 trackteroid-0.1.0rc2/.gitignore
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 16:01:03.175089 trackteroid-0.1.0rc2/.graphics/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 16:01:03.179089 trackteroid-0.1.0rc2/.graphics/svg/
--rw-r--r--   0 runner    (1001) docker     (123)     3248 2023-06-20 16:00:51.000000 trackteroid-0.1.0rc2/.graphics/svg/logo_black.svg
--rw-r--r--   0 runner    (1001) docker     (123)     3208 2023-06-20 16:00:51.000000 trackteroid-0.1.0rc2/.graphics/svg/logo_white.svg
--rw-r--r--   0 runner    (1001) docker     (123)      830 2023-06-20 16:00:51.000000 trackteroid-0.1.0rc2/.readthedocs.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      297 2023-06-20 16:00:51.000000 trackteroid-0.1.0rc2/AUTHORS.md
--rw-r--r--   0 runner    (1001) docker     (123)       14 2023-06-20 16:00:51.000000 trackteroid-0.1.0rc2/CHANGELOG.md
--rw-r--r--   0 runner    (1001) docker     (123)     1494 2023-06-20 16:00:51.000000 trackteroid-0.1.0rc2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     3566 2023-06-20 16:01:03.187090 trackteroid-0.1.0rc2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      902 2023-06-20 16:00:51.000000 trackteroid-0.1.0rc2/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 16:01:03.179089 trackteroid-0.1.0rc2/doc/
--rw-r--r--   0 runner    (1001) docker     (123)       83 2023-06-20 16:00:51.000000 trackteroid-0.1.0rc2/doc/requirements.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 16:01:03.179089 trackteroid-0.1.0rc2/doc/sphinx_source/
--rw-r--r--   0 runner    (1001) docker     (123)      634 2023-06-20 16:00:51.000000 trackteroid-0.1.0rc2/doc/sphinx_source/Makefile
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 16:01:03.179089 trackteroid-0.1.0rc2/doc/sphinx_source/_static/
--rw-r--r--   0 runner    (1001) docker     (123)   170890 2023-06-20 16:00:51.000000 trackteroid-0.1.0rc2/doc/sphinx_source/_static/favicon.ico
--rw-r--r--   0 runner    (1001) docker     (123)     4385 2023-06-20 16:00:51.000000 trackteroid-0.1.0rc2/doc/sphinx_source/_static/logo_white.svg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 16:01:03.183089 trackteroid-0.1.0rc2/doc/sphinx_source/collections/
--rw-r--r--   0 runner    (1001) docker     (123)     2787 2023-06-20 16:00:51.000000 trackteroid-0.1.0rc2/doc/sphinx_source/collections/emptycollection.md
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-20 16:00:51.000000 trackteroid-0.1.0rc2/doc/sphinx_source/collections/entitycollection.md
--rw-r--r--   0 runner    (1001) docker     (123)     1097 2023-06-20 16:00:51.000000 trackteroid-0.1.0rc2/doc/sphinx_source/collections/overview.md
--rw-r--r--   0 runner    (1001) docker     (123)      194 2023-06-20 16:00:51.000000 trackteroid-0.1.0rc2/doc/sphinx_source/collections.md
--rw-r--r--   0 runner    (1001) docker     (123)     1341 2023-06-20 16:00:51.000000 trackteroid-0.1.0rc2/doc/sphinx_source/conf.py
--rw-r--r--   0 runner    (1001) docker     (123)     8271 2023-06-20 16:00:51.000000 trackteroid-0.1.0rc2/doc/sphinx_source/configuration.md
--rw-r--r--   0 runner    (1001) docker     (123)     4779 2023-06-20 16:00:51.000000 trackteroid-0.1.0rc2/doc/sphinx_source/index.md
--rw-r--r--   0 runner    (1001) docker     (123)      554 2023-06-20 16:00:51.000000 trackteroid-0.1.0rc2/doc/sphinx_source/installation.md
--rw-r--r--   0 runner    (1001) docker     (123)      765 2023-06-20 16:00:51.000000 trackteroid-0.1.0rc2/doc/sphinx_source/make.bat
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 16:01:03.183089 trackteroid-0.1.0rc2/doc/sphinx_source/query/
--rw-r--r--   0 runner    (1001) docker     (123)     7897 2023-06-20 16:00:51.000000 trackteroid-0.1.0rc2/doc/sphinx_source/query/overview.md
--rw-r--r--   0 runner    (1001) docker     (123)       43 2023-06-20 16:00:51.000000 trackteroid-0.1.0rc2/doc/sphinx_source/query.md
--rw-r--r--   0 runner    (1001) docker     (123)    12845 2023-06-20 16:00:51.000000 trackteroid-0.1.0rc2/doc/sphinx_source/quickstart.md
--rw-r--r--   0 runner    (1001) docker     (123)        9 2023-06-20 16:00:51.000000 trackteroid-0.1.0rc2/doc/sphinx_source/session.md
--rw-r--r--   0 runner    (1001) docker     (123)     1159 2023-06-20 16:00:51.000000 trackteroid-0.1.0rc2/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)      277 2023-06-20 16:00:51.000000 trackteroid-0.1.0rc2/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-20 16:01:03.187090 trackteroid-0.1.0rc2/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 16:01:03.175089 trackteroid-0.1.0rc2/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 16:01:03.183089 trackteroid-0.1.0rc2/src/trackteroid/
--rw-r--r--   0 runner    (1001) docker     (123)     1856 2023-06-20 16:00:51.000000 trackteroid-0.1.0rc2/src/trackteroid/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3911 2023-06-20 16:00:51.000000 trackteroid-0.1.0rc2/src/trackteroid/configuration.py
--rw-r--r--   0 runner    (1001) docker     (123)     1599 2023-06-20 16:00:51.000000 trackteroid-0.1.0rc2/src/trackteroid/constants.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 16:01:03.187090 trackteroid-0.1.0rc2/src/trackteroid/entities/
--rw-r--r--   0 runner    (1001) docker     (123)     1728 2023-06-20 16:00:51.000000 trackteroid-0.1.0rc2/src/trackteroid/entities/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    70322 2023-06-20 16:00:51.000000 trackteroid-0.1.0rc2/src/trackteroid/entities/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     1031 2023-06-20 16:00:51.000000 trackteroid-0.1.0rc2/src/trackteroid/entities/base.pyi
--rw-r--r--   0 runner    (1001) docker     (123)    10503 2023-06-20 16:00:51.000000 trackteroid-0.1.0rc2/src/trackteroid/entities/declarations.py
--rw-r--r--   0 runner    (1001) docker     (123)     4262 2023-06-20 16:00:51.000000 trackteroid-0.1.0rc2/src/trackteroid/entities/declarations.pyi
--rw-r--r--   0 runner    (1001) docker     (123)    31930 2023-06-20 16:00:51.000000 trackteroid-0.1.0rc2/src/trackteroid/entities/entities.py
--rwxr-xr-x   0 runner    (1001) docker     (123)   171659 2023-06-20 16:00:51.000000 trackteroid-0.1.0rc2/src/trackteroid/entities/entities.pyi
--rw-r--r--   0 runner    (1001) docker     (123)    12395 2023-06-20 16:00:51.000000 trackteroid-0.1.0rc2/src/trackteroid/entities/relationships_parser.py
--rw-r--r--   0 runner    (1001) docker     (123)     4287 2023-06-20 16:00:51.000000 trackteroid-0.1.0rc2/src/trackteroid/entities/schematypes.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 16:01:03.187090 trackteroid-0.1.0rc2/src/trackteroid/query/
--rw-r--r--   0 runner    (1001) docker     (123)     1759 2023-06-20 16:00:51.000000 trackteroid-0.1.0rc2/src/trackteroid/query/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6859 2023-06-20 16:00:51.000000 trackteroid-0.1.0rc2/src/trackteroid/query/criteria.py
--rw-r--r--   0 runner    (1001) docker     (123)     1884 2023-06-20 16:00:51.000000 trackteroid-0.1.0rc2/src/trackteroid/query/criteria.pyi
--rw-r--r--   0 runner    (1001) docker     (123)    16595 2023-06-20 16:00:51.000000 trackteroid-0.1.0rc2/src/trackteroid/query/query.py
--rw-r--r--   0 runner    (1001) docker     (123)      271 2023-06-20 16:00:51.000000 trackteroid-0.1.0rc2/src/trackteroid/query/query.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     3851 2023-06-20 16:00:51.000000 trackteroid-0.1.0rc2/src/trackteroid/query/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)    14066 2023-06-20 16:00:51.000000 trackteroid-0.1.0rc2/src/trackteroid/session.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 16:01:03.187090 trackteroid-0.1.0rc2/src/trackteroid/stubs/
--rw-r--r--   0 runner    (1001) docker     (123)     1574 2023-06-20 16:00:51.000000 trackteroid-0.1.0rc2/src/trackteroid/stubs/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    14184 2023-06-20 16:00:51.000000 trackteroid-0.1.0rc2/src/trackteroid/stubs/stubs.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 16:01:03.183089 trackteroid-0.1.0rc2/src/trackteroid.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     3566 2023-06-20 16:01:03.000000 trackteroid-0.1.0rc2/src/trackteroid.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1822 2023-06-20 16:01:03.000000 trackteroid-0.1.0rc2/src/trackteroid.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-20 16:01:03.000000 trackteroid-0.1.0rc2/src/trackteroid.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       24 2023-06-20 16:01:03.000000 trackteroid-0.1.0rc2/src/trackteroid.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       12 2023-06-20 16:01:03.000000 trackteroid-0.1.0rc2/src/trackteroid.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 16:01:03.187090 trackteroid-0.1.0rc2/tests/
--rw-r--r--   0 runner    (1001) docker     (123)       40 2023-06-20 16:00:51.000000 trackteroid-0.1.0rc2/tests/test_placeholder.py
--rw-r--r--   0 runner    (1001) docker     (123)      209 2023-06-20 16:00:51.000000 trackteroid-0.1.0rc2/tox.ini
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 09:05:37.357818 trackteroid-0.1.0rc3/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 09:05:37.337818 trackteroid-0.1.0rc3/.github/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 09:05:37.345818 trackteroid-0.1.0rc3/.github/ISSUE_TEMPLATE/
+-rw-r--r--   0 runner    (1001) docker     (123)      913 2023-06-26 09:05:11.000000 trackteroid-0.1.0rc3/.github/ISSUE_TEMPLATE/issue--bug-report.md
+-rw-r--r--   0 runner    (1001) docker     (123)      547 2023-06-26 09:05:11.000000 trackteroid-0.1.0rc3/.github/ISSUE_TEMPLATE/issue--feature-request.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 09:05:37.345818 trackteroid-0.1.0rc3/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)     1084 2023-06-26 09:05:11.000000 trackteroid-0.1.0rc3/.github/workflows/python-publish.yml
+-rw-r--r--   0 runner    (1001) docker     (123)       51 2023-06-26 09:05:11.000000 trackteroid-0.1.0rc3/.gitignore
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 09:05:37.337818 trackteroid-0.1.0rc3/.graphics/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 09:05:37.345818 trackteroid-0.1.0rc3/.graphics/svg/
+-rw-r--r--   0 runner    (1001) docker     (123)     3248 2023-06-26 09:05:11.000000 trackteroid-0.1.0rc3/.graphics/svg/logo_black.svg
+-rw-r--r--   0 runner    (1001) docker     (123)     3208 2023-06-26 09:05:11.000000 trackteroid-0.1.0rc3/.graphics/svg/logo_white.svg
+-rw-r--r--   0 runner    (1001) docker     (123)      830 2023-06-26 09:05:11.000000 trackteroid-0.1.0rc3/.readthedocs.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      297 2023-06-26 09:05:11.000000 trackteroid-0.1.0rc3/AUTHORS.md
+-rw-r--r--   0 runner    (1001) docker     (123)       14 2023-06-26 09:05:11.000000 trackteroid-0.1.0rc3/CHANGELOG.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1494 2023-06-26 09:05:11.000000 trackteroid-0.1.0rc3/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     3566 2023-06-26 09:05:37.357818 trackteroid-0.1.0rc3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      902 2023-06-26 09:05:11.000000 trackteroid-0.1.0rc3/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 09:05:37.345818 trackteroid-0.1.0rc3/doc/
+-rw-r--r--   0 runner    (1001) docker     (123)       83 2023-06-26 09:05:11.000000 trackteroid-0.1.0rc3/doc/requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 09:05:37.349818 trackteroid-0.1.0rc3/doc/sphinx_source/
+-rw-r--r--   0 runner    (1001) docker     (123)      634 2023-06-26 09:05:11.000000 trackteroid-0.1.0rc3/doc/sphinx_source/Makefile
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 09:05:37.349818 trackteroid-0.1.0rc3/doc/sphinx_source/_static/
+-rw-r--r--   0 runner    (1001) docker     (123)   170890 2023-06-26 09:05:11.000000 trackteroid-0.1.0rc3/doc/sphinx_source/_static/favicon.ico
+-rw-r--r--   0 runner    (1001) docker     (123)     4385 2023-06-26 09:05:11.000000 trackteroid-0.1.0rc3/doc/sphinx_source/_static/logo_white.svg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 09:05:37.349818 trackteroid-0.1.0rc3/doc/sphinx_source/collections/
+-rw-r--r--   0 runner    (1001) docker     (123)     1941 2023-06-26 09:05:11.000000 trackteroid-0.1.0rc3/doc/sphinx_source/collections/emptycollection.md
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-26 09:05:11.000000 trackteroid-0.1.0rc3/doc/sphinx_source/collections/entitycollection.md
+-rw-r--r--   0 runner    (1001) docker     (123)     7668 2023-06-26 09:05:11.000000 trackteroid-0.1.0rc3/doc/sphinx_source/collections/examples.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1097 2023-06-26 09:05:11.000000 trackteroid-0.1.0rc3/doc/sphinx_source/collections/overview.md
+-rw-r--r--   0 runner    (1001) docker     (123)      194 2023-06-26 09:05:11.000000 trackteroid-0.1.0rc3/doc/sphinx_source/collections.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1408 2023-06-26 09:05:11.000000 trackteroid-0.1.0rc3/doc/sphinx_source/conf.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8277 2023-06-26 09:05:11.000000 trackteroid-0.1.0rc3/doc/sphinx_source/configuration.md
+-rw-r--r--   0 runner    (1001) docker     (123)     4778 2023-06-26 09:05:11.000000 trackteroid-0.1.0rc3/doc/sphinx_source/index.md
+-rw-r--r--   0 runner    (1001) docker     (123)      554 2023-06-26 09:05:11.000000 trackteroid-0.1.0rc3/doc/sphinx_source/installation.md
+-rw-r--r--   0 runner    (1001) docker     (123)      765 2023-06-26 09:05:11.000000 trackteroid-0.1.0rc3/doc/sphinx_source/make.bat
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 09:05:37.349818 trackteroid-0.1.0rc3/doc/sphinx_source/query/
+-rw-r--r--   0 runner    (1001) docker     (123)     3726 2023-06-26 09:05:11.000000 trackteroid-0.1.0rc3/doc/sphinx_source/query/examples.md
+-rw-r--r--   0 runner    (1001) docker     (123)     5700 2023-06-26 09:05:11.000000 trackteroid-0.1.0rc3/doc/sphinx_source/query/overview.md
+-rw-r--r--   0 runner    (1001) docker     (123)      146 2023-06-26 09:05:11.000000 trackteroid-0.1.0rc3/doc/sphinx_source/query.md
+-rw-r--r--   0 runner    (1001) docker     (123)     8255 2023-06-26 09:05:11.000000 trackteroid-0.1.0rc3/doc/sphinx_source/quickstart.md
+-rw-r--r--   0 runner    (1001) docker     (123)        9 2023-06-26 09:05:11.000000 trackteroid-0.1.0rc3/doc/sphinx_source/session.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1159 2023-06-26 09:05:11.000000 trackteroid-0.1.0rc3/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      277 2023-06-26 09:05:11.000000 trackteroid-0.1.0rc3/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-26 09:05:37.357818 trackteroid-0.1.0rc3/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 09:05:37.341818 trackteroid-0.1.0rc3/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 09:05:37.349818 trackteroid-0.1.0rc3/src/trackteroid/
+-rw-r--r--   0 runner    (1001) docker     (123)     1856 2023-06-26 09:05:11.000000 trackteroid-0.1.0rc3/src/trackteroid/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5107 2023-06-26 09:05:11.000000 trackteroid-0.1.0rc3/src/trackteroid/configuration.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1599 2023-06-26 09:05:11.000000 trackteroid-0.1.0rc3/src/trackteroid/constants.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 09:05:37.353818 trackteroid-0.1.0rc3/src/trackteroid/entities/
+-rw-r--r--   0 runner    (1001) docker     (123)     1728 2023-06-26 09:05:11.000000 trackteroid-0.1.0rc3/src/trackteroid/entities/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    72524 2023-06-26 09:05:11.000000 trackteroid-0.1.0rc3/src/trackteroid/entities/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10503 2023-06-26 09:05:11.000000 trackteroid-0.1.0rc3/src/trackteroid/entities/declarations.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4262 2023-06-26 09:05:11.000000 trackteroid-0.1.0rc3/src/trackteroid/entities/declarations.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)    31930 2023-06-26 09:05:11.000000 trackteroid-0.1.0rc3/src/trackteroid/entities/entities.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)   171659 2023-06-26 09:05:11.000000 trackteroid-0.1.0rc3/src/trackteroid/entities/entities.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)    13329 2023-06-26 09:05:11.000000 trackteroid-0.1.0rc3/src/trackteroid/entities/relationships_parser.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4287 2023-06-26 09:05:11.000000 trackteroid-0.1.0rc3/src/trackteroid/entities/schematypes.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 09:05:37.353818 trackteroid-0.1.0rc3/src/trackteroid/query/
+-rw-r--r--   0 runner    (1001) docker     (123)     1759 2023-06-26 09:05:11.000000 trackteroid-0.1.0rc3/src/trackteroid/query/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6859 2023-06-26 09:05:11.000000 trackteroid-0.1.0rc3/src/trackteroid/query/criteria.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1884 2023-06-26 09:05:11.000000 trackteroid-0.1.0rc3/src/trackteroid/query/criteria.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)    16595 2023-06-26 09:05:11.000000 trackteroid-0.1.0rc3/src/trackteroid/query/query.py
+-rw-r--r--   0 runner    (1001) docker     (123)      271 2023-06-26 09:05:11.000000 trackteroid-0.1.0rc3/src/trackteroid/query/query.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     3851 2023-06-26 09:05:11.000000 trackteroid-0.1.0rc3/src/trackteroid/query/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14525 2023-06-26 09:05:11.000000 trackteroid-0.1.0rc3/src/trackteroid/session.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 09:05:37.353818 trackteroid-0.1.0rc3/src/trackteroid/stubs/
+-rw-r--r--   0 runner    (1001) docker     (123)     1574 2023-06-26 09:05:11.000000 trackteroid-0.1.0rc3/src/trackteroid/stubs/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14184 2023-06-26 09:05:11.000000 trackteroid-0.1.0rc3/src/trackteroid/stubs/stubs.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 09:05:37.349818 trackteroid-0.1.0rc3/src/trackteroid.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     3566 2023-06-26 09:05:37.000000 trackteroid-0.1.0rc3/src/trackteroid.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1866 2023-06-26 09:05:37.000000 trackteroid-0.1.0rc3/src/trackteroid.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-26 09:05:37.000000 trackteroid-0.1.0rc3/src/trackteroid.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       24 2023-06-26 09:05:37.000000 trackteroid-0.1.0rc3/src/trackteroid.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       12 2023-06-26 09:05:37.000000 trackteroid-0.1.0rc3/src/trackteroid.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 09:05:37.353818 trackteroid-0.1.0rc3/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)       40 2023-06-26 09:05:11.000000 trackteroid-0.1.0rc3/tests/test_placeholder.py
+-rw-r--r--   0 runner    (1001) docker     (123)      209 2023-06-26 09:05:11.000000 trackteroid-0.1.0rc3/tox.ini
```

### Comparing `trackteroid-0.1.0rc2/.github/ISSUE_TEMPLATE/issue--bug-report.md` & `trackteroid-0.1.0rc3/.github/ISSUE_TEMPLATE/issue--bug-report.md`

 * *Files identical despite different names*

### Comparing `trackteroid-0.1.0rc2/.github/ISSUE_TEMPLATE/issue--feature-request.md` & `trackteroid-0.1.0rc3/.github/ISSUE_TEMPLATE/issue--feature-request.md`

 * *Files identical despite different names*

### Comparing `trackteroid-0.1.0rc2/.github/workflows/python-publish.yml` & `trackteroid-0.1.0rc3/.github/workflows/python-publish.yml`

 * *Files identical despite different names*

### Comparing `trackteroid-0.1.0rc2/.graphics/svg/logo_black.svg` & `trackteroid-0.1.0rc3/.graphics/svg/logo_black.svg`

 * *Files identical despite different names*

### Comparing `trackteroid-0.1.0rc2/.graphics/svg/logo_white.svg` & `trackteroid-0.1.0rc3/.graphics/svg/logo_white.svg`

 * *Files identical despite different names*

### Comparing `trackteroid-0.1.0rc2/.readthedocs.yaml` & `trackteroid-0.1.0rc3/.readthedocs.yaml`

 * *Files identical despite different names*

### Comparing `trackteroid-0.1.0rc2/LICENSE` & `trackteroid-0.1.0rc3/LICENSE`

 * *Files identical despite different names*

### Comparing `trackteroid-0.1.0rc2/PKG-INFO` & `trackteroid-0.1.0rc3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: trackteroid
-Version: 0.1.0rc2
+Version: 0.1.0rc3
 Summary: Declarative, object-oriented wrapper for Ftrack queries. Powerful functional-style interactions with resulting collections.
 Author: Rico Koschmitzky, Dennis Weil
 License: BSD 3-Clause License
         
         Copyright (c) 2023, Trixter
         
         Redistribution and use in source and binary forms, with or without
```

### Comparing `trackteroid-0.1.0rc2/README.md` & `trackteroid-0.1.0rc3/README.md`

 * *Files identical despite different names*

### Comparing `trackteroid-0.1.0rc2/doc/sphinx_source/Makefile` & `trackteroid-0.1.0rc3/doc/sphinx_source/Makefile`

 * *Files identical despite different names*

### Comparing `trackteroid-0.1.0rc2/doc/sphinx_source/_static/favicon.ico` & `trackteroid-0.1.0rc3/doc/sphinx_source/_static/favicon.ico`

 * *Files identical despite different names*

### Comparing `trackteroid-0.1.0rc2/doc/sphinx_source/_static/logo_white.svg` & `trackteroid-0.1.0rc3/doc/sphinx_source/_static/logo_white.svg`

 * *Files identical despite different names*

### Comparing `trackteroid-0.1.0rc2/doc/sphinx_source/collections/overview.md` & `trackteroid-0.1.0rc3/doc/sphinx_source/collections/overview.md`

 * *Files identical despite different names*

### Comparing `trackteroid-0.1.0rc2/doc/sphinx_source/conf.py` & `trackteroid-0.1.0rc3/doc/sphinx_source/conf.py`

 * *Files 4% similar despite different names*

```diff
@@ -38,7 +38,12 @@
 # https://www.sphinx-doc.org/en/master/usage/configuration.html#options-for-html-output
 
 html_theme = 'sphinx_rtd_theme'
 html_static_path = ['_static']
 
 html_favicon = "_static/favicon.ico"
 html_logo = '_static/logo_white.svg'
+
+suppress_warnings = [
+    'myst.xref_missing',
+    'myst.header'
+]
```

### Comparing `trackteroid-0.1.0rc2/doc/sphinx_source/configuration.md` & `trackteroid-0.1.0rc3/doc/sphinx_source/configuration.md`

 * *Files 2% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 
 Configuration in Trackteroid is accomplished through a Python file, providing a high degree of flexibility and adjustability in a language you are already familiar with.
 
 To make your configuration file accessible, you can utilize the `TRACKTEROID_CONFIGURATION` environment variable.
 
 Here's an example for Linux with Bash:
 ```shell
-export TRACKTEROID_EXAMPLE=/path/to/my/trackteroid_user_config.py
+export TRACKTEROID_CONFIGURATION=/path/to/my/trackteroid_user_config.py
 ```
 
 The subsequent section outlines the available configuration options within Trackteroid and explains how to customize them according to your preferences.
 Configuration entries are defined in ALL_CAPS style and can store constant values or callables.
 
 
 ## ALLOWED_FOR_DELETION_RESOLVER
```

### Comparing `trackteroid-0.1.0rc2/doc/sphinx_source/index.md` & `trackteroid-0.1.0rc3/doc/sphinx_source/index.md`

 * *Files 0% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 
 
 **Declarative, object-oriented wrapper for Ftrack queries. Powerful functional-style interactions with resulting collections.**
 
 
 Welcome to Trackteroid’s documentation. Get started with [Installation](installation.md) and then get an overview with the [Quickstart](quickstart.md). 
 
-Trackteroid depends on [Ftrack](https://www.ftrack.com/en/) and it's [Python API](https://ftrack-python-api.readthedocs.io/) a project management and production tracking software specifically designed for the media and entertainment industry. It is commonly used in the fields of film, television, animation, visual effects, and gaming.
+Trackteroid depends on [Ftrack](https://www.ftrack.com/en/) and its [Python API](https://ftrack-python-api.readthedocs.io/) a project management and production tracking software specifically designed for the media and entertainment industry. It is commonly used in the fields of film, television, animation, visual effects, and gaming.
 
 
 ## Motivation
 
 We have decided to build a wrapping API around the Ftrack Python API to address several limitations and challenges that arise when directly interacting with the Python API. While the Ftrack Python API offers a lot of flexibility, there are certain aspects that can make development and maintenance more cumbersome and less intuitive. By creating a wrapping API, we aim to overcome these challenges and provide a more streamlined and developer-friendly experience. Here are the key reasons for this decision:
 
 - **Simplifying Querying**
```

### Comparing `trackteroid-0.1.0rc2/doc/sphinx_source/installation.md` & `trackteroid-0.1.0rc3/doc/sphinx_source/installation.md`

 * *Files identical despite different names*

### Comparing `trackteroid-0.1.0rc2/doc/sphinx_source/make.bat` & `trackteroid-0.1.0rc3/doc/sphinx_source/make.bat`

 * *Files identical despite different names*

### Comparing `trackteroid-0.1.0rc2/pyproject.toml` & `trackteroid-0.1.0rc3/pyproject.toml`

 * *Files identical despite different names*

### Comparing `trackteroid-0.1.0rc2/src/trackteroid/__init__.py` & `trackteroid-0.1.0rc3/src/trackteroid/__init__.py`

 * *Files identical despite different names*

### Comparing `trackteroid-0.1.0rc2/src/trackteroid/configuration.py` & `trackteroid-0.1.0rc3/src/trackteroid/configuration.py`

 * *Files 22% similar despite different names*

```diff
@@ -30,57 +30,97 @@
 
 import importlib
 import logging
 import os
 import traceback
 import sys
 
+import wrapt
+
+
+def _fallback_decorator(fallback_func, attribute):
+    """ fallback mechanism for the wrapped function on the associated config entry
+
+    Args:
+        fallback_func callable: function to wrap
+        attribute: name of the attribute the fallback will be applied to
+
+    Returns:
+        callable: function wrapper
+
+    """
+    @wrapt.decorator
+    def wrapper(wrapped, instance, args, kwargs):
+        try:
+            return wrapped(*args, **kwargs)
+        except:
+            _LOG.error(
+                f"Calling '{attribute}' raised an exception. Falling back to default implementation!",
+                exc_info=True
+            )
+            return fallback_func(*args, **kwargs)
+
+    return wrapper
 
 
 def _override_configuration():
-    """ idenfities and parses a user configuration and applies relevant attributes to this module
+    """ identifies and parses a user configuration and applies relevant attributes to this module
 
     """
     _custom_configuration = os.getenv("TRACKTEROID_CONFIGURATION", False)
     # try our best to source a custom configuration
     if _custom_configuration:
         if not os.path.exists(_custom_configuration):
-            raise OSError("Custom configuration `{}` doesn't exist.".format(_custom_configuration))
+            raise OSError(f"Custom configuration `{_custom_configuration}` doesn't exist.")
         if not os.path.splitext(_custom_configuration)[1] in [".py"]:
-            raise AssertionError("Custom configuration must `{}` be a .py file.".format(_custom_configuration))
+            raise AssertionError(f"Custom configuration must `{_custom_configuration}` be a .py file.")
 
-        _LOG.info("Custom configuration specified in `{}`. Trying to load...".format(_custom_configuration))
+        _LOG.info(f"Custom configuration specified in `{_custom_configuration}`. Trying to load...")
         try:
-            custom_configuration = importlib.load_source("configuration", _custom_configuration)
+            spec = importlib.util.spec_from_file_location("custom_configuration", _custom_configuration)
+            custom_configuration = importlib.util.module_from_spec(spec)
+            spec.loader.exec_module(custom_configuration)
         except:
             raise RuntimeError(
-                "Failed to load custom configuration.\n{}".format("\n".join(traceback.format_exception(*sys.exc_info())))
+                "Failed to load custom configuration.\n{}".format(
+                    "\n".join(traceback.format_exception(*sys.exc_info()))
+                )
             )
 
         relevant_attributes = [_ for _ in globals().keys() if _.isupper() and not _.startswith("_")]
         for attribute in relevant_attributes:
             if hasattr(custom_configuration, attribute):
-                _LOG.info("Adding '{}' from user configuration.".format(attribute))
-                globals()[attribute] = getattr(custom_configuration, attribute)
+                _LOG.info(f"Adding '{attribute}' from user configuration.")
+                if attribute in _CALLABLES_REQUIRE_FALLBACK:
+                    globals()[attribute] = _fallback_decorator(
+                        globals()[attribute],
+                        attribute
+                    )(getattr(custom_configuration, attribute))
+                else:
+                    globals()[attribute] = getattr(custom_configuration, attribute)
+
 
 # default entries - ALL upper variable names in here can be set in custom user configuration
 ############################################################################################
-# TODO: add example output
+
 # A functions that gets the current api version string and would return a custom entities
 # schema used for relationship resolutions.
 RELATIONSHIPS_RESOLVER = lambda api_version: {}
 
 # The primary logger
 LOGGING_NAMESPACE = "trackteroid"
 
 # A function that gets the current session and the type name that it requests a
 # deletion for and resolves to True or False.
 ALLOWED_FOR_DELETION_RESOLVER = lambda session, type_name: True
 
 WARN_ON_INJECT = False
 ############################################################################################
 
-_LOG = logging.getLogger("{}.configuration".format(LOGGING_NAMESPACE))
+_LOG = logging.getLogger(f"{LOGGING_NAMESPACE}.configuration")
+_CALLABLES_REQUIRE_FALLBACK = [
+    "RELATIONSHIPS_RESOLVER",
+]
 
 _override_configuration()
```

### Comparing `trackteroid-0.1.0rc2/src/trackteroid/constants.py` & `trackteroid-0.1.0rc3/src/trackteroid/constants.py`

 * *Files 8% similar despite different names*

```diff
@@ -24,8 +24,8 @@
 #  DAMAGES (INCLUDING, BUT NOT LIMITED TO, PROCUREMENT OF SUBSTITUTE GOODS OR
 #  SERVICES; LOSS OF USE, DATA, OR PROFITS; OR BUSINESS INTERRUPTION) HOWEVER
 #  CAUSED AND ON ANY THEORY OF LIABILITY, WHETHER IN CONTRACT, STRICT LIABILITY,
 #  OR TORT (INCLUDING NEGLIGENCE OR OTHERWISE) ARISING IN ANY WAY OUT OF THE USE
 #  OF THIS SOFTWARE, EVEN IF ADVISED OF THE POSSIBILITY OF SUCH DAMAGE.
 #
 
-__VERSION__ = "0.1.0rc2"
+__VERSION__ = "0.1.0rc3"
```

### Comparing `trackteroid-0.1.0rc2/src/trackteroid/entities/__init__.py` & `trackteroid-0.1.0rc3/src/trackteroid/entities/__init__.py`

 * *Files identical despite different names*

### Comparing `trackteroid-0.1.0rc2/src/trackteroid/entities/base.py` & `trackteroid-0.1.0rc3/src/trackteroid/entities/base.py`

 * *Files 1% similar despite different names*

```diff
@@ -39,30 +39,29 @@
 )
 from copy import copy
 import sys
 
 from ftrack_api.symbol import NOT_SET
 
 from .declarations import *
-from .relationships_parser import RelationshipsParser
+
 from .schematypes import (
     CUSTOM_ATTRIBUTE_TYPE_COMPATIBILITY,
     AttributeInfo
 )
 from ..query import (
     Criterion,
     Criteria,
     utils
 )
 from ..configuration import (
     LOGGING_NAMESPACE,
     ALLOWED_FOR_DELETION_RESOLVER,
     WARN_ON_INJECT
 )
-from ..session import SESSION
 
 
 LOG = logging.getLogger("{}.entities".format(LOGGING_NAMESPACE))
 
 _RELATIONSHIPS_CACHE = {}
 
 
@@ -170,34 +169,36 @@
             self._entity_type_name = entity_type.__name__
 
         # build a key for the cached based on used schema name and session server url
         key = self._cache_key
 
         # on initial request infer all relationships from database and custom schema
         if key not in _RELATIONSHIPS_CACHE:
-            # always do a copy of ourselve that will be added to the cache as a Relationship instance
+            # always do a copy of ourselves that will be added to the cache as a Relationship instance
             # is currently being used as a class attribute
             self._infer_from_session_schema(session)
 
             # TODO: warn if schema doesn't have entities set
             collection_attributes = session.parsed_relationships.array_attributes
             for target_entity_name, relation in schema.get("entities", {}).get(self._entity_type_name, {}).items():
                 collection = None
 
                 if not isinstance(relation, list):
                     _relation = [relation]
+                else:
+                    _relation = relation
 
                 for some_relation in _relation:
                     attribute_tokens = some_relation.split(".")
                     leaf_attribute = some_relation.split(".")[-1]
 
                     if len(attribute_tokens) > 1:
                         _collection = leaf_attribute in collection_attributes
                     else:
-                        _collection = bool(re.match("^(children|ancestors)(\[\w+\])?", attribute_tokens[0]))
+                        _collection = bool(re.match(r"^(children|ancestors)(\[\w+\])?", attribute_tokens[0]))
 
                     if collection is None:
                         collection = _collection
                     if collection != _collection:
                         raise AttributeError(
                             "Given relationships '{}' attribute array state is ambigious.".format(
                                 relation
@@ -257,31 +258,31 @@
 
     def __getattr__(self, item):
         current_depth = self.depth
         collection_copy = copy(self)
         # in case we use methods like .values() or .from_entities() etc
         # we need to take care to not increment the depth, as it doesn represent
         # an attribute/relation access
-        if item in [_ for _ in dir(EntityCollection) if not re.match("__\w+__|children", _)]:
+        if item in [_ for _ in dir(EntityCollection) if not re.match(r"__\w+__|children", _)]:
             collection_copy.depth = current_depth
         return collection_copy
 
     def __getitem__(self, item):
         # TEST: Maybe we should return somthing else when accessing POD
         #  attributes so we can avoid doing this:
         #  names.append(Query(Asset).by_name("test").get_all().name or [])
 
         if inspect.isclass(item) and issubclass(item, Entity):
             self._entity = item()
 
         return self
 
     def __iter__(self):
-       self._current_iter_index = 0
-       return self
+        self._current_iter_index = 0
+        return self
 
     def __len__(self):
         return 0
 
     def __next__(self):
         if self._current_iter_index == 0:
             self._current_iter_index += 1
@@ -301,19 +302,19 @@
 
     @property
     def entity_type(self):
         return self._entity
 
     def create(self, **kwargs):
         assert self.depth == 1, \
-        """
-        This attribute does not exist yet. The parent attribute also did not exist.
-        Create can only be called on existing attributes OR if at least the parent
-        exists.
-        """
+            """
+            This attribute does not exist yet. The parent attribute also did not exist.
+            Create can only be called on existing attributes OR if at least the parent
+            exists.
+            """
         entitycollection = EntityCollection._make_empty(self._entity.__class__, self._session)
         return entitycollection.create(empty=self, **kwargs)
 
     def create_batch(self, *attributes):
         """
 
         Args:
@@ -350,28 +351,34 @@
     MEMBERS = [
         "_entity",
         "_entities",
         "_query",
         "query",
         "_schema_types_map",
         "_current_iter_index",
-        "_session"
+        "_session",
+        "_source"
     ]
 
     def __init__(self, _cls=None, entities={}, session=None):
         super(EntityCollection, self).__init__()
         self._entity = _cls()
 
         self._entities = entities
         self._query = None
         self._current_iter_index = []
         self._session = session
 
+        # similar to the source attribute on EmptyCollection
+        # we sometimes need to keep track of what produced this
+        # current collection
+        self._source = (None, None)
+
         self._schema_types_map = {
-            "string": (str),
+            "string": (str,),
             "number": (float,),
             "boolean": (bool,),
             "integer": (int,),
             "mapped_array": (dict,)
         }
 
     def __contains__(self, other):
@@ -393,35 +400,37 @@
         # TODO: clean after we have tests for this functionality
         if self and item in list(self.values())[0].ftrack_entity.keys():
             entities = []
             values = []
             entity_type = None
             for entity in self.values():
                 value = entity[item]
-                # resolve entitites in collections
+                # resolve entities in collections
                 if value.__class__.__name__ == "Collection":
                     for _ in value:
                         # wrap ftrack entity
                         if hasattr(_, "entity_type"):
                             entities.append(Entity.from_entity_type(str(_.entity_type), ftrack_entity=_))
                         else:
                             values.append(_)
                     if not entities and not values and not entity_type:
-                        entity_type = Entity.from_entity_type(name=self._get_attribute_compatibility_types(item).types[0].__name__)
+                        entity_type = Entity.from_entity_type(
+                            name=self._get_attribute_compatibility_types(item).types[0].__name__
+                        )
                 elif value.__class__.__name__ == "KeyValueMappedCollectionProxy":
                     values.append(dict(entity.ftrack_entity["metadata"].items()))
 
                 # wrap ftrack entity
                 elif hasattr(value, "entity_type"):
                     entities.append(Entity.from_entity_type(str(value.entity_type), ftrack_entity=value))
                 else:
                     values.append(value)
 
             if entities:
-                return self.from_entities(entities)
+                return self.from_entities(entities, source=(item, self))
             elif entity_type:
                 return EmptyCollection(_type=entity_type, source=self, session=self._session)
             return values
 
         elif item == "get":
             return self._get_relatives
 
@@ -432,36 +441,40 @@
             for entity in self.values():
                 values.append(entity.ftrack_entity["custom_attributes"].get(attr))
             return values
 
         # handle collection.<type>
         elif item in globals():
             # if not already parsed and cached let's do it now
-            self._entity.relationship(session=self.query.session, schema=self.query.schema, entity_type=self._entity.__class__)
+            self._entity.relationship(
+                session=self.query.session,
+                schema=self.query.schema,
+                entity_type=self._entity.__class__
+            )
             if self._entity.relationship.get(globals()[item]):
                 relation = self._entity.relationship.get(globals()[item]).relation
 
                 result = None
 
                 if not isinstance(relation, list):
                     relation = [relation]
 
                 for some_relation in relation:
                     current = None
                     # tokenize the attribute chain
                     for token in some_relation.split("."):
                         _filter = None
                         # and also identify filters like with `parent[Shot]`
-                        _ = re.findall("\w+", token)
+                        _ = re.findall(r"\w+", token)
                         if len(_) == 2:
                             token, _filter = _
                         elif len(_) > 2:
                             raise ValueError("Unable to identify attribute and filter within token '{}'.".format(_))
 
-                        _collection = self if current == None else current
+                        _collection = self if current is None else current
                         current = getattr(_collection, token)
 
                         if NOT_SET in current:
                             self._entity.log.warning(
                                 "Was the attribute you're trying to access projected? "
                                 "A symbol.NOT_SET found on '{}' access. This would resolve to '{}'.".format(
                                     item,
@@ -469,25 +482,24 @@
                                 )
                             )
 
                         # TODO: check if the entity we need for filtering is in the globals
                         if _filter:
                             current = current[globals()[_filter]]
 
-                    if result == None:
+                    if result is None:
                         result = current
                     else:
                         result = result.union(current)
 
                 return result
 
         else:
             raise AttributeError("Attribute {} does not exist.".format(item))
 
-
     def __getitem__(self, item):
         if isinstance(item, (int, slice)):
             # no one needs to know that internally we store the id as the key!
             return self.from_entities(list(self.values())[item])
         elif isinstance(item, str):
             return self.from_entities(self._entities[item])
         elif issubclass(item, Entity):
@@ -533,54 +545,67 @@
 
     def __setattr__(self, key, value):
         # TODO: setting uses_versions and used_in_versions will not update bidirectionally
         #  Can we solve this in a generic way?
         # should we update this so we have the correct data locally?
         if key in self.MEMBERS:
             super(EntityCollection, self).__setattr__(key, value)
-        elif getattr(self, key, None) is not None:
-            compatible, reason = self._is_attribute_compatible_with_value(key, value)
-            if not compatible:
-                raise TypeError(reason)
-
-            if isinstance(value, (list, tuple, EntityCollection)) \
-                    and len(self) == 1 \
-                    and list(self._entities.values())[0].ftrack_entity[key].__class__.__name__ == "Collection":
-                if isinstance(value, EntityCollection):
-                    list(self.values())[0].ftrack_entity[key] = [_.ftrack_entity for _ in value.values()]
-            else:
-                for idx, entity in enumerate(self.values()):
-                    if key.startswith("custom_"):
-                        if isinstance(value, (list, tuple, EntityCollection)):
-                            entity.ftrack_entity["custom_attributes"][key.replace("custom_", "")] = value[idx]
-                        else:
-                            entity.ftrack_entity["custom_attributes"][key.replace("custom_", "")] = value
-                    elif entity.ftrack_entity[key].__class__.__name__ == "KeyValueMappedCollectionProxy":
-                        _should_capture = False
-                        if isinstance(value, (list, tuple)):
-                            if any(_ not in  value[idx].keys() for _ in entity.ftrack_entity[key]):
-                                _should_capture = True
-                            for _key, _value in value[idx].items():
-                                entity.ftrack_entity[key][_key] = _value
-                        else:
-                            if not len(value):
-                                entity.ftrack_entity[key] = value
+        else:
+            attribute_value = getattr(self, key, None)
+            if attribute_value is not None:
+                # If the attribute access produces a collection
+                # we potentially can not go by key as the attribute
+                # access can be a type based shortcut.
+                # Therefore we need to resolve the collections produced
+                # via the full attribute chain and retain the last attribute
+                # as our key.
+                if not isinstance(attribute_value, list):
+                    key, collection = attribute_value._source
+                else:
+                    collection = self
+
+                compatible, reason = collection._is_attribute_compatible_with_value(key, value)
+                if not compatible:
+                    raise TypeError(reason)
+
+                if isinstance(value, (list, tuple, EntityCollection)) \
+                        and len(collection) == 1 \
+                        and list(collection._entities.values())[0].ftrack_entity[key].__class__.__name__ == "Collection":
+                    if isinstance(value, EntityCollection):
+                        list(collection.values())[0].ftrack_entity[key] = [_.ftrack_entity for _ in value.values()]
+                else:
+                    for idx, entity in enumerate(collection.values()):
+                        if key.startswith("custom_"):
+                            if isinstance(value, (list, tuple, EntityCollection)):
+                                entity.ftrack_entity["custom_attributes"][key.replace("custom_", "")] = value[idx]
                             else:
-                                for _key, _value in value.items():
+                                entity.ftrack_entity["custom_attributes"][key.replace("custom_", "")] = value
+                        elif entity.ftrack_entity[key].__class__.__name__ == "KeyValueMappedCollectionProxy":
+                            _should_capture = False
+                            if isinstance(value, (list, tuple)):
+                                if any(_ not in  value[idx].keys() for _ in entity.ftrack_entity[key]):
+                                    _should_capture = True
+                                for _key, _value in value[idx].items():
                                     entity.ftrack_entity[key][_key] = _value
-                    else:
-                        if isinstance(value, EntityCollection):
-                            entity.ftrack_entity[key] = list(value.values())[idx].ftrack_entity
-                        elif isinstance(value, (list, tuple)):
-                            entity.ftrack_entity[key] = value[idx]
+                            else:
+                                if not len(value):
+                                    entity.ftrack_entity[key] = value
+                                else:
+                                    for _key, _value in value.items():
+                                        entity.ftrack_entity[key][_key] = _value
                         else:
-                            entity.ftrack_entity[key] = value
+                            if isinstance(value, EntityCollection):
+                                entity.ftrack_entity[key] = list(value.values())[idx].ftrack_entity
+                            elif isinstance(value, (list, tuple)):
+                                entity.ftrack_entity[key] = value[idx]
+                            else:
+                                entity.ftrack_entity[key] = value
 
-        else:
-            raise AttributeError("Attribute {} does not exist.".format(key))
+            else:
+                raise AttributeError("Attribute {} does not exist.".format(key))
 
     def __nonzero__(self):
         return len(self) > 0
 
     def _init_type_map(self, type_def):
         """ builds a dictionary with EmptyCollections, based on the given type definitions
 
@@ -780,32 +805,29 @@
         value_info = self._get_value_type(value)
         compatible, reason = True, ""
 
         # TODO: make sure we compare the actual types and not just the names
         # TEST: What happens if we naively do this. Adjust unittests to check!
         if value_info.types not in [_ for _ in attribute_info.types]:
             compatible, reason = False, \
-            (
-                "The given value '{}' does not have the correct type "
-                "for the receiver attribute '{}'. {} != {}".format(
-                    value,
-                    attribute_name,
-                    value_info.types,
-                    attribute_info.types
+                (
+                    "The given value '{}' does not have the correct type "
+                    "for the receiver attribute '{}'. {} != {}".format(
+                        value,
+                        attribute_name,
+                        value_info.types,
+                        attribute_info.types
+                    )
                 )
-            )
             return compatible, reason
 
-        # TODO: Allow assignment of single value to multiple receivers.
-        #  If is_array is true, we have to make sure, that the receiver either supports
-        #  a collection or we have to check if the value only contains a single value
         if isinstance(value, (EntityCollection, tuple, list)):
             _reason = (
                 "When setting an attribute on a receiver collection, "
-                "we expect the given value to have the same amount of alements as our collection has entities"
+                "we expect the given value to have the same amount of elements as our collection has entities "
                 "or in case it is an iterable to have the same length."
             )
             if attribute_info.array:
                 if len(self) > 1:
                     # we want to assign a value to multiple entities
                     if len(self) != len(value):
                         compatible, reason = False, _reason
@@ -817,19 +839,23 @@
                 "The given value is not a collection or array, but the receiver contains more than a single entity."
 
         return compatible, reason
 
     @staticmethod
     def _get_value_type(value):
         if isinstance(value, (EntityCollection, EmptyCollection)):
-            return AttributeInfo(types=type(value._entity),
-                                 array=True)
+            return AttributeInfo(
+                types=type(value._entity),
+                array=True
+            )
         elif isinstance(value, (tuple, list)):
-            return AttributeInfo(types=type(value[0]),
-                                 array=True)
+            return AttributeInfo(
+                types=type(value[0]),
+                array=True
+            )
         else:
             return AttributeInfo(types=type(value))
 
     def _get_attribute_compatibility_types(self, attribute_name):
         """ Returns an AttributeInfo object that encodes which values can
         potentially be assigned to self.[attribute_name]
             Args:
@@ -885,16 +911,18 @@
         self._query = copy(instance)
 
     def from_entities(self, entities, type_override=None, source=None):
         """ helper to create an EntityCollection from given entities
 
         Args:
             entities (Entity or list): Entity subclass or list of Entity subclasses
-            source (EntityCollection): In case entities is an empty list, it might be important
+            source (EntityCollection or tuple(str, EntityCollection)): store what source produced the new collection
             to preserve the source, from where the resulting EmptyCollection was generated from.
+            type_override: if given it will use the override as the type for the generated collection
+                and not determine it from the first entity automatically
 
         Returns:
             EntityCollection
         """
         if not entities:
             if type_override:
                 type_override = type_override()
@@ -928,14 +956,16 @@
             _cls=type_override or _entity_types[0],
             entities=_entities,
             session=self._session
         )
 
         entities.query = self.query
         entities.query.valid = False
+        entities._source = source
+
         return entities
 
     def group(self, predicate):
         """ Returns a dictionary with keys given by the predicate. All entities
         from the original collection will be mapped to their corresponding key.
 
         Examples:
@@ -1081,14 +1111,43 @@
                     filtered.append(entity)
 
         if filtered:
             return self.from_entities(filtered)
         else:
             return EmptyCollection(_type=self._entity, source=self._get_parent(self), session=self._session)
 
+    def apply(self, predicate, attribute_name=None):
+        """Applies a predicate function to each entity in the collection and
+        assigns the generated value to the specified attribute.
+        If no attribute name is provided, the value is directly assigned to the calling collection.
+
+        Examples:
+            >>> some_collection.apply(lambda c: c.another_attr[0] + "_edited", "some_attr")
+            >>> assetversion_collection.Task.Status.apply(status_collection)
+
+        Args:
+            predicate (callable): A callable function that receives a single entity collection.
+                The return value of the function will be applied to the specified attribute.
+            attribute_name (optional: str): The name of the attribute to which the generated value will be assigned
+                or None
+
+        Returns:
+            EntityCollection: the updated collection
+
+        """
+        if not attribute_name:
+            attribute_name, collection = self._source
+        else:
+            collection = self
+
+        for entitycollection in collection:
+            setattr(entitycollection, attribute_name, predicate(entitycollection))
+
+        return getattr(collection, attribute_name)
+
     @staticmethod
     def _get_parent(entitycollection):
         parent_relation = entitycollection._entity.relationship.parent or "parent"
         parents = getattr(entitycollection, parent_relation)
         if not isinstance(parents, (EntityCollection, EmptyCollection)):
             entitycollection.fetch_attributes(parent_relation)
             parents = getattr(entitycollection, parent_relation)
@@ -1125,15 +1184,15 @@
 
         return self.from_entities(positive), self.from_entities(negative)
 
     def union(self, *collections):
         """ Returns an EntityCollection with elements belonging to the current or the given collection or possibly both
 
         Args:
-            collection (EntityCollection): EntityCollection object of same type as the current one
+            collections (EntityCollection): EntityCollection object of same type as the current one
 
         Returns:
             EntityCollection:
 
         """
         entities = list(self.values())
         for collection in collections:
@@ -1146,15 +1205,15 @@
 
         return self.from_entities(entities)
 
     def intersection(self, *collections):
         """ Returns an EntityCollection with elements belonging to the current and the given collection
 
         Args:
-            collection (EntityCollection): EntityCollection object of same type as the current one
+            collections (EntityCollection): EntityCollection object of same type as the current one
 
         Returns:
             EntityCollection:
 
         """
         for collection in collections:
             self._validate_collection_type(collection)
@@ -1283,15 +1342,15 @@
         def _flatten(iterable):
             def __flatten(iterable, path=""):
                 flat = {}
                 if len(iterable.keys()) == 1:
                     # we are on a non branching level
                     key = list(iterable.keys())[0]
                     # append to the existing path as we don't need to branch
-                    path += "." + key if path else key # only insert dot in existing path
+                    path += "." + key if path else key  # only insert dot in existing path
                     # get the downstream dict recursively
                     if key.endswith("]"):
                         _ = __flatten(iterable[key], "")
                     else:
                         _ = __flatten(iterable[key], path)
                     # if the downstream level will not branch either, we move the dict
                     # up one level. this is also done if we split due to a type
@@ -1398,31 +1457,29 @@
             query.get_all()
         else:
             LOG.info("All requested attributes already set.")
 
     def commit(self):
         self._session.commit()
 
-    def _get_relatives(self, relative_type, *args, **kwargs):
+    def _get_relatives(self, relative_type, **kwargs):
         """ Get the relative entity based on the relationship.
 
         Args:
             relative_type (Entity): subclass of Entity
-            *args ():
             **kwargs ():
 
         Returns:
             Any: whatever the attributes holds, most likely another EntityCollection
         """
 
         relationship = self.query.entity_type.relationship.get(relative_type, default=TargetRelation()).relation
         if not relationship:
             raise ValueError("Unknown relationship for relative '{}'".format(relative_type))
 
-        relation_projections = []
         if not isinstance(relationship, list):
             relation_projections = [relationship]
         else:
             relation_projections = relationship
 
         outside_projections = kwargs.get("projections", [])
         constructed_projections = []
@@ -1591,23 +1648,20 @@
 
     def delete(self):
         """ Deletes all Entities in self from ftrack.
 
         Returns:
             The SESSION object so we can call commit() directly.
         """
-
-
-        if not ALLOWED_FOR_DELETION_RESOLVER(session=self._session, type_name=self.entity_type.__name__):
+        type_name = self.entity_type.__name__
+        if not ALLOWED_FOR_DELETION_RESOLVER(session=self._session, type_name=type_name):
             raise AssertionError(
-                "Current entity type '{}' for server '{}' is not allowed for deletion as it doesn't match against "
-                "any of these patterns: {}".format(
-                    self.entity_type.__name__,
-                    self._session.server_url,
-                    (", ".join(allowed_for_deletion_patterns) or "<no pattern given>")
+                "Current entity type '{}' for server '{}' is not allowed for deletion. ".format(
+                    type_name,
+                    self._session.server_url
                 )
             )
 
         for entity in self.values():
             ftrack_entity = entity.ftrack_entity
             LOG.info("Deleting Entity '{}'".format(ftrack_entity))
             self._session.delete(ftrack_entity)
@@ -1747,23 +1801,23 @@
     # this is how the query consolidates its criteria
     # having multiple filters allows us the inject criterion multiple times
     # Example:
     #   Query(Task).inject("parent.parent.name is 'library').by_name(Project, "Foobar").inject("parent.status.name is 'Approved').get_all()
     def inject(self, target, *filter):
         if any(re.search(r"^or\s*", _, flags=re.IGNORECASE) for _ in filter):
             raise ValueError(
-                "OR relationships are not supported accross multiple criteria or filter.\n"
-                "You can use an 'or' relatioship within a single filter string though."
+                "OR relationships are not supported across multiple criteria or filter.\n"
+                "You can use an 'or' relationship within a single filter string though."
             )
 
         # sanitize partial query
         sanitized_filters = [re.sub(r"^(and|where)\s*", "", _, flags=re.IGNORECASE) for _ in filter]
         partial_query = " and ".join(sanitized_filters)
         if WARN_ON_INJECT:
-            self.log.warning("`inject` crieria was used with partial query '{}'".format(partial_query))
+            self.log.warning("`inject` criteria was used with partial query '{}'".format(partial_query))
 
         return partial_query
 
 
 class Entity(_EntityBase):
 
     @Criteria.supported_targets(_EntityBase)
@@ -1784,7 +1838,8 @@
         query = query[:-4] + ")"
         return query
 
 
 class EntityCollectionOperationError(ValueError):
     pass
 
+
```

### Comparing `trackteroid-0.1.0rc2/src/trackteroid/entities/declarations.py` & `trackteroid-0.1.0rc3/src/trackteroid/entities/declarations.py`

 * *Files identical despite different names*

### Comparing `trackteroid-0.1.0rc2/src/trackteroid/entities/declarations.pyi` & `trackteroid-0.1.0rc3/src/trackteroid/entities/declarations.pyi`

 * *Files identical despite different names*

### Comparing `trackteroid-0.1.0rc2/src/trackteroid/entities/entities.py` & `trackteroid-0.1.0rc3/src/trackteroid/entities/entities.py`

 * *Files identical despite different names*

### Comparing `trackteroid-0.1.0rc2/src/trackteroid/entities/entities.pyi` & `trackteroid-0.1.0rc3/src/trackteroid/entities/entities.pyi`

 * *Files identical despite different names*

### Comparing `trackteroid-0.1.0rc2/src/trackteroid/entities/relationships_parser.py` & `trackteroid-0.1.0rc3/src/trackteroid/entities/relationships_parser.py`

 * *Files 4% similar despite different names*

```diff
@@ -80,29 +80,44 @@
                     if ref:
                         tmp_array_refs[prop] = ref
             self._entities[entity_id]["refs"] = tmp_refs
             self._entities[entity_id]["array_refs"] = tmp_array_refs
 
     def create_entity_network(self, ftrack_entity):
         self._tmp_exclude_types = set(self._exclude_types)
+        # entity type must be excluded, as finding it in one of its children would lead to an endless recursion
+        self._tmp_exclude_types.add(ftrack_entity)
         return self.recurse_entity_connections(ftrack_entity, ancestors=set())
 
     def recurse_entity_connections(self, ftrack_entity, ancestors=None):
+        # ancestors are the entities, in sequence, linking to the current entity
+        # the top entity of course has none
         if ancestors is None:
             ancestors = set()
+        # refs - reference type attributes on the current entity
+        # type - current entity's type
         network = {"refs": {}, "type": ftrack_entity}
+        # return otherwise recursion will be endless
         if ftrack_entity in ancestors:
             return network
+
+        # get all array or non-array reference attributes of the current entity
         refs = self._entities.get(ftrack_entity).get(self._ref_key)
         if refs:
+            # first iteration - validate props
+            valid_props = {}
             for prop_name, prop_type in refs.items():
-                if prop_name in self._attributes_blacklist or prop_type in self._tmp_exclude_types or prop_type == ftrack_entity:
-                    continue
+                if prop_name not in self._attributes_blacklist and prop_type not in self._tmp_exclude_types and prop_type != ftrack_entity:
+                    valid_props[prop_name] = prop_type
+            # add valid prop types to exclude list for deeper recursions
+            self._tmp_exclude_types.update(valid_props.values())
+
+            # second iteration, recurse all valid props
+            for prop_name, prop_type in valid_props.items():
                 if prop_type in self._entities:
-                    self._tmp_exclude_types.add(ftrack_entity)
                     ancestors.add(ftrack_entity)
                     network["refs"][prop_name] = self.recurse_entity_connections(prop_type, ancestors)
         return network
 
     def extract_entity_relations(self, network):
         self._tmp_relations = {}
         self.recurse_entity_relations(network)
@@ -120,23 +135,26 @@
                     self._tmp_relations[prop_type] = tmp_path
                     self.recurse_entity_relations(attr_data, tmp_path)
 
     def extract_all_entity_relations(self):
         for entity_name in self._entities:
             self._relationships[entity_name] = {}
 
+            # create network of non-array references
             self.use_array_refs = False
             asset_network = self.create_entity_network(entity_name)
 
             # extract non-collection relations
             self._relationships[entity_name]["non_collection"] = self.extract_entity_relations(asset_network)
 
-            # extract collection relations
+            # create network of array references
             self.use_array_refs = True
             asset_network = self.create_entity_network(entity_name)
+
+            # extract collection relations
             self._relationships[entity_name]["collection"] = self.extract_entity_relations(asset_network)
 
     def parse_project_structure(self, project):
         root_data = TreeData(project.entity_type, None)
         self._root_item = TreeItem(root_data)
         self._project_relations = {}
         self.recurse_project_structure(self._root_item, project)
```

### Comparing `trackteroid-0.1.0rc2/src/trackteroid/entities/schematypes.py` & `trackteroid-0.1.0rc3/src/trackteroid/entities/schematypes.py`

 * *Files identical despite different names*

### Comparing `trackteroid-0.1.0rc2/src/trackteroid/query/__init__.py` & `trackteroid-0.1.0rc3/src/trackteroid/query/__init__.py`

 * *Files identical despite different names*

### Comparing `trackteroid-0.1.0rc2/src/trackteroid/query/criteria.py` & `trackteroid-0.1.0rc3/src/trackteroid/query/criteria.py`

 * *Files identical despite different names*

### Comparing `trackteroid-0.1.0rc2/src/trackteroid/query/criteria.pyi` & `trackteroid-0.1.0rc3/src/trackteroid/query/criteria.pyi`

 * *Files identical despite different names*

### Comparing `trackteroid-0.1.0rc2/src/trackteroid/query/query.py` & `trackteroid-0.1.0rc3/src/trackteroid/query/query.py`

 * *Files identical despite different names*

### Comparing `trackteroid-0.1.0rc2/src/trackteroid/query/utils.py` & `trackteroid-0.1.0rc3/src/trackteroid/query/utils.py`

 * *Files 4% similar despite different names*

```diff
@@ -51,15 +51,15 @@
                 )
             else:
                 non_pattern_elements.append("\"{}\"".format(element))
 
         non_pattern_expressions = []
 
         # handle known id shortcuts like parent.id -> parent_id, version.id -> version_id
-        if attribute is "id" and target.relation and not target.collection:
+        if attribute == "id" and target.relation and not target.collection:
             relation_tokens = relation.split(".")
             if len(relation_tokens) > 1:
                 attribute = "{}_id".format(relation_tokens[-1])
                 relation = ".".join(relation_tokens[:-1])
             else:
                 attribute = "{}_id".format(relation_tokens[0])
                 relation = ""
```

### Comparing `trackteroid-0.1.0rc2/src/trackteroid/session.py` & `trackteroid-0.1.0rc3/src/trackteroid/session.py`

 * *Files 4% similar despite different names*

```diff
@@ -98,18 +98,23 @@
     def __ne__(self, other):
         return not self.__eq__(other)
 
     @property
     def parsed_relationships(self):
         if not self._session.server_url in _PARSED_RELATIONSHIPS_CACHE:
             relationship_parser = RelationshipsParser(ftrack_session=self._session)
-            # TODO: why do we have to exclude certain types?
+            # types such as "Context" are ambiguous and cannot be used to extract direct relationships
+            # example structure - Seq -> Folder -> Shot
+            # in this case, establishing a relationship from Seq to Shot is impossible as would any other
+            # that went through "parent" or "children" for example
             relationship_parser.exclude_types = {"Context"}
             relationship_parser.parse_session_schemas()
-            # TODO: why do we have to exclude certain attributes?
+            # attributes that group things cannot be used to extract relationships
+            # as an example, "descendants" lists all children and children of children and so on,
+            # so they are all flattened with their relationships removed
             relationship_parser.attributes_blacklist = {"descendants", "ancestors", "status_changes"}
             relationship_parser.extract_all_entity_relations()
             _PARSED_RELATIONSHIPS_CACHE[self._session.server_url] = relationship_parser
 
         return _PARSED_RELATIONSHIPS_CACHE[self._session.server_url]
 
     def get_cached_collections(self):
```

### Comparing `trackteroid-0.1.0rc2/src/trackteroid/stubs/__init__.py` & `trackteroid-0.1.0rc3/src/trackteroid/stubs/__init__.py`

 * *Files identical despite different names*

### Comparing `trackteroid-0.1.0rc2/src/trackteroid/stubs/stubs.py` & `trackteroid-0.1.0rc3/src/trackteroid/stubs/stubs.py`

 * *Files identical despite different names*

### Comparing `trackteroid-0.1.0rc2/src/trackteroid.egg-info/PKG-INFO` & `trackteroid-0.1.0rc3/src/trackteroid.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: trackteroid
-Version: 0.1.0rc2
+Version: 0.1.0rc3
 Summary: Declarative, object-oriented wrapper for Ftrack queries. Powerful functional-style interactions with resulting collections.
 Author: Rico Koschmitzky, Dennis Weil
 License: BSD 3-Clause License
         
         Copyright (c) 2023, Trixter
         
         Redistribution and use in source and binary forms, with or without
```

### Comparing `trackteroid-0.1.0rc2/src/trackteroid.egg-info/SOURCES.txt` & `trackteroid-0.1.0rc3/src/trackteroid.egg-info/SOURCES.txt`

 * *Files 5% similar despite different names*

```diff
@@ -23,28 +23,29 @@
 doc/sphinx_source/query.md
 doc/sphinx_source/quickstart.md
 doc/sphinx_source/session.md
 doc/sphinx_source/_static/favicon.ico
 doc/sphinx_source/_static/logo_white.svg
 doc/sphinx_source/collections/emptycollection.md
 doc/sphinx_source/collections/entitycollection.md
+doc/sphinx_source/collections/examples.md
 doc/sphinx_source/collections/overview.md
+doc/sphinx_source/query/examples.md
 doc/sphinx_source/query/overview.md
 src/trackteroid/__init__.py
 src/trackteroid/configuration.py
 src/trackteroid/constants.py
 src/trackteroid/session.py
 src/trackteroid.egg-info/PKG-INFO
 src/trackteroid.egg-info/SOURCES.txt
 src/trackteroid.egg-info/dependency_links.txt
 src/trackteroid.egg-info/requires.txt
 src/trackteroid.egg-info/top_level.txt
 src/trackteroid/entities/__init__.py
 src/trackteroid/entities/base.py
-src/trackteroid/entities/base.pyi
 src/trackteroid/entities/declarations.py
 src/trackteroid/entities/declarations.pyi
 src/trackteroid/entities/entities.py
 src/trackteroid/entities/entities.pyi
 src/trackteroid/entities/relationships_parser.py
 src/trackteroid/entities/schematypes.py
 src/trackteroid/query/__init__.py
```

