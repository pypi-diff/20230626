# Comparing `tmp/tendril-utils-db-0.5.1.tar.gz` & `tmp/tendril-utils-db-0.5.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tendril-utils-db-0.5.1.tar", last modified: Wed Apr 12 17:42:18 2023, max compression
+gzip compressed data, was "tendril-utils-db-0.5.2.tar", last modified: Mon Jun 26 15:16:59 2023, max compression
```

## Comparing `tendril-utils-db-0.5.1.tar` & `tendril-utils-db-0.5.2.tar`

### file list

```diff
@@ -1,62 +1,62 @@
-drwxrwxr-x   0 chintal   (1000) chintal   (1000)        0 2023-04-12 17:42:18.514977 tendril-utils-db-0.5.1/
--rw-rw-r--   0 chintal   (1000) chintal   (1000)     2122 2020-08-18 06:57:07.000000 tendril-utils-db-0.5.1/.gitignore
--rw-rw-r--   0 chintal   (1000) chintal   (1000)      638 2020-08-18 06:57:07.000000 tendril-utils-db-0.5.1/.readthedocs.yml
--rw-rw-r--   0 chintal   (1000) chintal   (1000)      629 2020-08-18 06:57:07.000000 tendril-utils-db-0.5.1/.travis.yml
--rw-rw-r--   0 chintal   (1000) chintal   (1000)        0 2020-08-18 06:57:07.000000 tendril-utils-db-0.5.1/CHANGELOG.rst
--rw-rw-r--   0 chintal   (1000) chintal   (1000)    34520 2020-08-18 06:57:07.000000 tendril-utils-db-0.5.1/LICENSE
--rw-rw-r--   0 chintal   (1000) chintal   (1000)      173 2020-08-18 06:57:07.000000 tendril-utils-db-0.5.1/MANIFEST.in
--rw-rw-r--   0 chintal   (1000) chintal   (1000)     3495 2023-04-12 17:42:18.514977 tendril-utils-db-0.5.1/PKG-INFO
--rw-rw-r--   0 chintal   (1000) chintal   (1000)     2205 2020-08-18 06:57:07.000000 tendril-utils-db-0.5.1/README.rst
--rw-rw-r--   0 chintal   (1000) chintal   (1000)     2109 2022-12-08 14:04:07.000000 tendril-utils-db-0.5.1/alembic.ini
-drwxrwxr-x   0 chintal   (1000) chintal   (1000)        0 2023-04-12 17:42:18.506977 tendril-utils-db-0.5.1/docs/
--rw-rw-r--   0 chintal   (1000) chintal   (1000)     7660 2020-08-18 06:57:07.000000 tendril-utils-db-0.5.1/docs/Makefile
-drwxrwxr-x   0 chintal   (1000) chintal   (1000)        0 2023-04-12 17:42:18.510977 tendril-utils-db-0.5.1/docs/_static/
--rw-rw-r--   0 chintal   (1000) chintal   (1000)     2727 2020-08-18 06:57:07.000000 tendril-utils-db-0.5.1/docs/_static/custom.css
--rw-rw-r--   0 chintal   (1000) chintal   (1000)   128918 2020-08-18 06:57:07.000000 tendril-utils-db-0.5.1/docs/_static/favicon.ico
--rw-rw-r--   0 chintal   (1000) chintal   (1000)    96804 2020-08-18 06:57:07.000000 tendril-utils-db-0.5.1/docs/_static/logo.png
--rw-rw-r--   0 chintal   (1000) chintal   (1000)     9889 2020-08-18 06:57:07.000000 tendril-utils-db-0.5.1/docs/_static/logo_packed.png
-drwxrwxr-x   0 chintal   (1000) chintal   (1000)        0 2023-04-12 17:42:18.510977 tendril-utils-db-0.5.1/docs/_templates/
--rw-rw-r--   0 chintal   (1000) chintal   (1000)     1713 2020-08-18 06:57:07.000000 tendril-utils-db-0.5.1/docs/_templates/about.html
-drwxrwxr-x   0 chintal   (1000) chintal   (1000)        0 2023-04-12 17:42:18.510977 tendril-utils-db-0.5.1/docs/api/
--rw-rw-r--   0 chintal   (1000) chintal   (1000)      128 2020-08-18 06:57:07.000000 tendril-utils-db-0.5.1/docs/api/index.rst
--rw-rw-r--   0 chintal   (1000) chintal   (1000)    13493 2020-08-18 06:57:07.000000 tendril-utils-db-0.5.1/docs/conf.py
--rw-rw-r--   0 chintal   (1000) chintal   (1000)      869 2020-08-18 06:57:07.000000 tendril-utils-db-0.5.1/docs/index.rst
--rw-rw-r--   0 chintal   (1000) chintal   (1000)     1643 2020-08-18 06:57:07.000000 tendril-utils-db-0.5.1/docs/installation.rst
-drwxrwxr-x   0 chintal   (1000) chintal   (1000)        0 2023-04-12 17:42:18.510977 tendril-utils-db-0.5.1/docs/usage/
--rw-rw-r--   0 chintal   (1000) chintal   (1000)       35 2020-08-18 06:57:07.000000 tendril-utils-db-0.5.1/docs/usage/standalone.rst
--rw-rw-r--   0 chintal   (1000) chintal   (1000)       49 2020-08-18 06:57:07.000000 tendril-utils-db-0.5.1/docs/usage/tendril.rst
--rw-rw-r--   0 chintal   (1000) chintal   (1000)      131 2023-04-12 17:42:18.514977 tendril-utils-db-0.5.1/setup.cfg
--rwxrwxr-x   0 chintal   (1000) chintal   (1000)     3310 2022-12-15 17:03:18.000000 tendril-utils-db-0.5.1/setup.py
-drwxrwxr-x   0 chintal   (1000) chintal   (1000)        0 2023-04-12 17:42:18.502977 tendril-utils-db-0.5.1/src/
-drwxrwxr-x   0 chintal   (1000) chintal   (1000)        0 2023-04-12 17:42:18.510977 tendril-utils-db-0.5.1/src/tendril/
--rw-rw-r--   0 chintal   (1000) chintal   (1000)       65 2020-11-29 17:49:40.000000 tendril-utils-db-0.5.1/src/tendril/__init__.py
-drwxrwxr-x   0 chintal   (1000) chintal   (1000)        0 2023-04-12 17:42:18.510977 tendril-utils-db-0.5.1/src/tendril/config/
--rw-rw-r--   0 chintal   (1000) chintal   (1000)     1112 2020-08-18 06:57:07.000000 tendril-utils-db-0.5.1/src/tendril/config/__init__.py
--rw-rw-r--   0 chintal   (1000) chintal   (1000)     2812 2023-03-28 18:11:09.000000 tendril-utils-db-0.5.1/src/tendril/config/db.py
--rw-rw-r--   0 chintal   (1000) chintal   (1000)     1599 2022-12-08 13:59:11.000000 tendril-utils-db-0.5.1/src/tendril/config/db_core.py
-drwxrwxr-x   0 chintal   (1000) chintal   (1000)        0 2023-04-12 17:42:18.510977 tendril-utils-db-0.5.1/src/tendril/db/
--rw-rw-r--   0 chintal   (1000) chintal   (1000)       65 2022-12-08 13:59:11.000000 tendril-utils-db-0.5.1/src/tendril/db/__init__.py
-drwxrwxr-x   0 chintal   (1000) chintal   (1000)        0 2023-04-12 17:42:18.510977 tendril-utils-db-0.5.1/src/tendril/db/controllers/
--rw-rw-r--   0 chintal   (1000) chintal   (1000)       65 2022-12-15 17:03:18.000000 tendril-utils-db-0.5.1/src/tendril/db/controllers/__init__.py
-drwxrwxr-x   0 chintal   (1000) chintal   (1000)        0 2023-04-12 17:42:18.514977 tendril-utils-db-0.5.1/src/tendril/db/migration/
--rw-rw-r--   0 chintal   (1000) chintal   (1000)       38 2022-12-08 13:59:11.000000 tendril-utils-db-0.5.1/src/tendril/db/migration/README
--rw-rw-r--   0 chintal   (1000) chintal   (1000)        0 2022-12-08 13:59:11.000000 tendril-utils-db-0.5.1/src/tendril/db/migration/__init__.py
--rw-rw-r--   0 chintal   (1000) chintal   (1000)     2206 2022-12-08 13:59:11.000000 tendril-utils-db-0.5.1/src/tendril/db/migration/env.py
--rw-rw-r--   0 chintal   (1000) chintal   (1000)      494 2022-12-08 13:59:11.000000 tendril-utils-db-0.5.1/src/tendril/db/migration/script.py.mako
-drwxrwxr-x   0 chintal   (1000) chintal   (1000)        0 2023-04-12 17:42:18.514977 tendril-utils-db-0.5.1/src/tendril/db/migration/versions/
--rw-rw-r--   0 chintal   (1000) chintal   (1000)        0 2022-12-08 13:59:11.000000 tendril-utils-db-0.5.1/src/tendril/db/migration/versions/__init__.py
-drwxrwxr-x   0 chintal   (1000) chintal   (1000)        0 2023-04-12 17:42:18.514977 tendril-utils-db-0.5.1/src/tendril/db/models/
--rw-rw-r--   0 chintal   (1000) chintal   (1000)       65 2022-12-15 17:03:18.000000 tendril-utils-db-0.5.1/src/tendril/db/models/__init__.py
-drwxrwxr-x   0 chintal   (1000) chintal   (1000)        0 2023-04-12 17:42:18.514977 tendril-utils-db-0.5.1/src/tendril/utils/
--rw-rw-r--   0 chintal   (1000) chintal   (1000)       65 2020-11-29 17:49:49.000000 tendril-utils-db-0.5.1/src/tendril/utils/__init__.py
--rw-rw-r--   0 chintal   (1000) chintal   (1000)    10197 2023-04-12 17:41:29.000000 tendril-utils-db-0.5.1/src/tendril/utils/db.py
-drwxrwxr-x   0 chintal   (1000) chintal   (1000)        0 2023-04-12 17:42:18.514977 tendril-utils-db-0.5.1/src/tendril_utils_db.egg-info/
--rw-rw-r--   0 chintal   (1000) chintal   (1000)     3495 2023-04-12 17:42:18.000000 tendril-utils-db-0.5.1/src/tendril_utils_db.egg-info/PKG-INFO
--rw-rw-r--   0 chintal   (1000) chintal   (1000)     1089 2023-04-12 17:42:18.000000 tendril-utils-db-0.5.1/src/tendril_utils_db.egg-info/SOURCES.txt
--rw-rw-r--   0 chintal   (1000) chintal   (1000)        1 2023-04-12 17:42:18.000000 tendril-utils-db-0.5.1/src/tendril_utils_db.egg-info/dependency_links.txt
--rw-rw-r--   0 chintal   (1000) chintal   (1000)      763 2023-04-12 17:42:18.000000 tendril-utils-db-0.5.1/src/tendril_utils_db.egg-info/requires.txt
--rw-rw-r--   0 chintal   (1000) chintal   (1000)        8 2023-04-12 17:42:18.000000 tendril-utils-db-0.5.1/src/tendril_utils_db.egg-info/top_level.txt
-drwxrwxr-x   0 chintal   (1000) chintal   (1000)        0 2023-04-12 17:42:18.514977 tendril-utils-db-0.5.1/tests/
--rw-rw-r--   0 chintal   (1000) chintal   (1000)        0 2020-08-18 06:57:07.000000 tendril-utils-db-0.5.1/tests/__init__.py
--rw-rw-r--   0 chintal   (1000) chintal   (1000)     1060 2020-08-18 06:57:07.000000 tendril-utils-db-0.5.1/tests/coveralls.py
--rw-rw-r--   0 chintal   (1000) chintal   (1000)      858 2020-08-18 06:57:07.000000 tendril-utils-db-0.5.1/tox.ini
+drwxrwxr-x   0 chintal   (1000) chintal   (1000)        0 2023-06-26 15:16:59.471393 tendril-utils-db-0.5.2/
+-rw-rw-r--   0 chintal   (1000) chintal   (1000)     2122 2020-08-18 06:57:07.000000 tendril-utils-db-0.5.2/.gitignore
+-rw-rw-r--   0 chintal   (1000) chintal   (1000)      638 2020-08-18 06:57:07.000000 tendril-utils-db-0.5.2/.readthedocs.yml
+-rw-rw-r--   0 chintal   (1000) chintal   (1000)      629 2020-08-18 06:57:07.000000 tendril-utils-db-0.5.2/.travis.yml
+-rw-rw-r--   0 chintal   (1000) chintal   (1000)        0 2020-08-18 06:57:07.000000 tendril-utils-db-0.5.2/CHANGELOG.rst
+-rw-rw-r--   0 chintal   (1000) chintal   (1000)    34520 2020-08-18 06:57:07.000000 tendril-utils-db-0.5.2/LICENSE
+-rw-rw-r--   0 chintal   (1000) chintal   (1000)      173 2020-08-18 06:57:07.000000 tendril-utils-db-0.5.2/MANIFEST.in
+-rw-rw-r--   0 chintal   (1000) chintal   (1000)     3495 2023-06-26 15:16:59.471393 tendril-utils-db-0.5.2/PKG-INFO
+-rw-rw-r--   0 chintal   (1000) chintal   (1000)     2205 2020-08-18 06:57:07.000000 tendril-utils-db-0.5.2/README.rst
+-rw-rw-r--   0 chintal   (1000) chintal   (1000)     2109 2022-12-08 14:04:07.000000 tendril-utils-db-0.5.2/alembic.ini
+drwxrwxr-x   0 chintal   (1000) chintal   (1000)        0 2023-06-26 15:16:59.463393 tendril-utils-db-0.5.2/docs/
+-rw-rw-r--   0 chintal   (1000) chintal   (1000)     7660 2020-08-18 06:57:07.000000 tendril-utils-db-0.5.2/docs/Makefile
+drwxrwxr-x   0 chintal   (1000) chintal   (1000)        0 2023-06-26 15:16:59.467393 tendril-utils-db-0.5.2/docs/_static/
+-rw-rw-r--   0 chintal   (1000) chintal   (1000)     2727 2020-08-18 06:57:07.000000 tendril-utils-db-0.5.2/docs/_static/custom.css
+-rw-rw-r--   0 chintal   (1000) chintal   (1000)   128918 2020-08-18 06:57:07.000000 tendril-utils-db-0.5.2/docs/_static/favicon.ico
+-rw-rw-r--   0 chintal   (1000) chintal   (1000)    96804 2020-08-18 06:57:07.000000 tendril-utils-db-0.5.2/docs/_static/logo.png
+-rw-rw-r--   0 chintal   (1000) chintal   (1000)     9889 2020-08-18 06:57:07.000000 tendril-utils-db-0.5.2/docs/_static/logo_packed.png
+drwxrwxr-x   0 chintal   (1000) chintal   (1000)        0 2023-06-26 15:16:59.467393 tendril-utils-db-0.5.2/docs/_templates/
+-rw-rw-r--   0 chintal   (1000) chintal   (1000)     1713 2020-08-18 06:57:07.000000 tendril-utils-db-0.5.2/docs/_templates/about.html
+drwxrwxr-x   0 chintal   (1000) chintal   (1000)        0 2023-06-26 15:16:59.467393 tendril-utils-db-0.5.2/docs/api/
+-rw-rw-r--   0 chintal   (1000) chintal   (1000)      128 2020-08-18 06:57:07.000000 tendril-utils-db-0.5.2/docs/api/index.rst
+-rw-rw-r--   0 chintal   (1000) chintal   (1000)    13493 2020-08-18 06:57:07.000000 tendril-utils-db-0.5.2/docs/conf.py
+-rw-rw-r--   0 chintal   (1000) chintal   (1000)      869 2020-08-18 06:57:07.000000 tendril-utils-db-0.5.2/docs/index.rst
+-rw-rw-r--   0 chintal   (1000) chintal   (1000)     1643 2020-08-18 06:57:07.000000 tendril-utils-db-0.5.2/docs/installation.rst
+drwxrwxr-x   0 chintal   (1000) chintal   (1000)        0 2023-06-26 15:16:59.467393 tendril-utils-db-0.5.2/docs/usage/
+-rw-rw-r--   0 chintal   (1000) chintal   (1000)       35 2020-08-18 06:57:07.000000 tendril-utils-db-0.5.2/docs/usage/standalone.rst
+-rw-rw-r--   0 chintal   (1000) chintal   (1000)       49 2020-08-18 06:57:07.000000 tendril-utils-db-0.5.2/docs/usage/tendril.rst
+-rw-rw-r--   0 chintal   (1000) chintal   (1000)      131 2023-06-26 15:16:59.471393 tendril-utils-db-0.5.2/setup.cfg
+-rwxrwxr-x   0 chintal   (1000) chintal   (1000)     3310 2022-12-15 17:03:18.000000 tendril-utils-db-0.5.2/setup.py
+drwxrwxr-x   0 chintal   (1000) chintal   (1000)        0 2023-06-26 15:16:59.455393 tendril-utils-db-0.5.2/src/
+drwxrwxr-x   0 chintal   (1000) chintal   (1000)        0 2023-06-26 15:16:59.467393 tendril-utils-db-0.5.2/src/tendril/
+-rw-rw-r--   0 chintal   (1000) chintal   (1000)       65 2020-11-29 17:49:40.000000 tendril-utils-db-0.5.2/src/tendril/__init__.py
+drwxrwxr-x   0 chintal   (1000) chintal   (1000)        0 2023-06-26 15:16:59.467393 tendril-utils-db-0.5.2/src/tendril/config/
+-rw-rw-r--   0 chintal   (1000) chintal   (1000)     1112 2020-08-18 06:57:07.000000 tendril-utils-db-0.5.2/src/tendril/config/__init__.py
+-rw-rw-r--   0 chintal   (1000) chintal   (1000)     2812 2023-03-28 18:11:09.000000 tendril-utils-db-0.5.2/src/tendril/config/db.py
+-rw-rw-r--   0 chintal   (1000) chintal   (1000)     1599 2022-12-08 13:59:11.000000 tendril-utils-db-0.5.2/src/tendril/config/db_core.py
+drwxrwxr-x   0 chintal   (1000) chintal   (1000)        0 2023-06-26 15:16:59.467393 tendril-utils-db-0.5.2/src/tendril/db/
+-rw-rw-r--   0 chintal   (1000) chintal   (1000)       65 2022-12-08 13:59:11.000000 tendril-utils-db-0.5.2/src/tendril/db/__init__.py
+drwxrwxr-x   0 chintal   (1000) chintal   (1000)        0 2023-06-26 15:16:59.467393 tendril-utils-db-0.5.2/src/tendril/db/controllers/
+-rw-rw-r--   0 chintal   (1000) chintal   (1000)       65 2022-12-15 17:03:18.000000 tendril-utils-db-0.5.2/src/tendril/db/controllers/__init__.py
+drwxrwxr-x   0 chintal   (1000) chintal   (1000)        0 2023-06-26 15:16:59.471393 tendril-utils-db-0.5.2/src/tendril/db/migration/
+-rw-rw-r--   0 chintal   (1000) chintal   (1000)       38 2022-12-08 13:59:11.000000 tendril-utils-db-0.5.2/src/tendril/db/migration/README
+-rw-rw-r--   0 chintal   (1000) chintal   (1000)        0 2022-12-08 13:59:11.000000 tendril-utils-db-0.5.2/src/tendril/db/migration/__init__.py
+-rw-rw-r--   0 chintal   (1000) chintal   (1000)     2206 2022-12-08 13:59:11.000000 tendril-utils-db-0.5.2/src/tendril/db/migration/env.py
+-rw-rw-r--   0 chintal   (1000) chintal   (1000)      494 2022-12-08 13:59:11.000000 tendril-utils-db-0.5.2/src/tendril/db/migration/script.py.mako
+drwxrwxr-x   0 chintal   (1000) chintal   (1000)        0 2023-06-26 15:16:59.471393 tendril-utils-db-0.5.2/src/tendril/db/migration/versions/
+-rw-rw-r--   0 chintal   (1000) chintal   (1000)        0 2022-12-08 13:59:11.000000 tendril-utils-db-0.5.2/src/tendril/db/migration/versions/__init__.py
+drwxrwxr-x   0 chintal   (1000) chintal   (1000)        0 2023-06-26 15:16:59.471393 tendril-utils-db-0.5.2/src/tendril/db/models/
+-rw-rw-r--   0 chintal   (1000) chintal   (1000)       65 2022-12-15 17:03:18.000000 tendril-utils-db-0.5.2/src/tendril/db/models/__init__.py
+drwxrwxr-x   0 chintal   (1000) chintal   (1000)        0 2023-06-26 15:16:59.471393 tendril-utils-db-0.5.2/src/tendril/utils/
+-rw-rw-r--   0 chintal   (1000) chintal   (1000)       65 2020-11-29 17:49:49.000000 tendril-utils-db-0.5.2/src/tendril/utils/__init__.py
+-rw-rw-r--   0 chintal   (1000) chintal   (1000)    10347 2023-06-26 15:16:17.000000 tendril-utils-db-0.5.2/src/tendril/utils/db.py
+drwxrwxr-x   0 chintal   (1000) chintal   (1000)        0 2023-06-26 15:16:59.471393 tendril-utils-db-0.5.2/src/tendril_utils_db.egg-info/
+-rw-rw-r--   0 chintal   (1000) chintal   (1000)     3495 2023-06-26 15:16:59.000000 tendril-utils-db-0.5.2/src/tendril_utils_db.egg-info/PKG-INFO
+-rw-rw-r--   0 chintal   (1000) chintal   (1000)     1089 2023-06-26 15:16:59.000000 tendril-utils-db-0.5.2/src/tendril_utils_db.egg-info/SOURCES.txt
+-rw-rw-r--   0 chintal   (1000) chintal   (1000)        1 2023-06-26 15:16:59.000000 tendril-utils-db-0.5.2/src/tendril_utils_db.egg-info/dependency_links.txt
+-rw-rw-r--   0 chintal   (1000) chintal   (1000)      763 2023-06-26 15:16:59.000000 tendril-utils-db-0.5.2/src/tendril_utils_db.egg-info/requires.txt
+-rw-rw-r--   0 chintal   (1000) chintal   (1000)        8 2023-06-26 15:16:59.000000 tendril-utils-db-0.5.2/src/tendril_utils_db.egg-info/top_level.txt
+drwxrwxr-x   0 chintal   (1000) chintal   (1000)        0 2023-06-26 15:16:59.471393 tendril-utils-db-0.5.2/tests/
+-rw-rw-r--   0 chintal   (1000) chintal   (1000)        0 2020-08-18 06:57:07.000000 tendril-utils-db-0.5.2/tests/__init__.py
+-rw-rw-r--   0 chintal   (1000) chintal   (1000)     1060 2020-08-18 06:57:07.000000 tendril-utils-db-0.5.2/tests/coveralls.py
+-rw-rw-r--   0 chintal   (1000) chintal   (1000)      858 2020-08-18 06:57:07.000000 tendril-utils-db-0.5.2/tox.ini
```

### Comparing `tendril-utils-db-0.5.1/.gitignore` & `tendril-utils-db-0.5.2/.gitignore`

 * *Files identical despite different names*

### Comparing `tendril-utils-db-0.5.1/.readthedocs.yml` & `tendril-utils-db-0.5.2/.readthedocs.yml`

 * *Files identical despite different names*

### Comparing `tendril-utils-db-0.5.1/.travis.yml` & `tendril-utils-db-0.5.2/.travis.yml`

 * *Files identical despite different names*

### Comparing `tendril-utils-db-0.5.1/LICENSE` & `tendril-utils-db-0.5.2/LICENSE`

 * *Files identical despite different names*

### Comparing `tendril-utils-db-0.5.1/PKG-INFO` & `tendril-utils-db-0.5.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tendril-utils-db
-Version: 0.5.1
+Version: 0.5.2
 Summary: Database utilities for tendril
 Home-page: https://github.com/tendril-framework/tendril-utils-db
 Author: Chintalagiri Shashank
 Author-email: shashank@chintal.in
 Project-URL: Documentation, https://tendril-utils-db.readthedocs.io/en/latest
 Project-URL: Bug Tracker, https://github.com/tendril-framework/tendril-utils-db/issues
 Project-URL: Source Repository, https://github.com/tendril-framework/tendril-utils-db
```

### Comparing `tendril-utils-db-0.5.1/README.rst` & `tendril-utils-db-0.5.2/README.rst`

 * *Files identical despite different names*

### Comparing `tendril-utils-db-0.5.1/alembic.ini` & `tendril-utils-db-0.5.2/alembic.ini`

 * *Files identical despite different names*

### Comparing `tendril-utils-db-0.5.1/docs/Makefile` & `tendril-utils-db-0.5.2/docs/Makefile`

 * *Files identical despite different names*

### Comparing `tendril-utils-db-0.5.1/docs/_static/custom.css` & `tendril-utils-db-0.5.2/docs/_static/custom.css`

 * *Files identical despite different names*

### Comparing `tendril-utils-db-0.5.1/docs/_static/favicon.ico` & `tendril-utils-db-0.5.2/docs/_static/favicon.ico`

 * *Files identical despite different names*

### Comparing `tendril-utils-db-0.5.1/docs/_static/logo.png` & `tendril-utils-db-0.5.2/docs/_static/logo.png`

 * *Files identical despite different names*

### Comparing `tendril-utils-db-0.5.1/docs/_static/logo_packed.png` & `tendril-utils-db-0.5.2/docs/_static/logo_packed.png`

 * *Files identical despite different names*

### Comparing `tendril-utils-db-0.5.1/docs/_templates/about.html` & `tendril-utils-db-0.5.2/docs/_templates/about.html`

 * *Files identical despite different names*

### Comparing `tendril-utils-db-0.5.1/docs/conf.py` & `tendril-utils-db-0.5.2/docs/conf.py`

 * *Files identical despite different names*

### Comparing `tendril-utils-db-0.5.1/docs/index.rst` & `tendril-utils-db-0.5.2/docs/index.rst`

 * *Files identical despite different names*

### Comparing `tendril-utils-db-0.5.1/docs/installation.rst` & `tendril-utils-db-0.5.2/docs/installation.rst`

 * *Files identical despite different names*

### Comparing `tendril-utils-db-0.5.1/setup.py` & `tendril-utils-db-0.5.2/setup.py`

 * *Files identical despite different names*

### Comparing `tendril-utils-db-0.5.1/src/tendril/config/__init__.py` & `tendril-utils-db-0.5.2/src/tendril/config/__init__.py`

 * *Files identical despite different names*

### Comparing `tendril-utils-db-0.5.1/src/tendril/config/db.py` & `tendril-utils-db-0.5.2/src/tendril/config/db.py`

 * *Files identical despite different names*

### Comparing `tendril-utils-db-0.5.1/src/tendril/config/db_core.py` & `tendril-utils-db-0.5.2/src/tendril/config/db_core.py`

 * *Files identical despite different names*

### Comparing `tendril-utils-db-0.5.1/src/tendril/db/migration/env.py` & `tendril-utils-db-0.5.2/src/tendril/db/migration/env.py`

 * *Files identical despite different names*

### Comparing `tendril-utils-db-0.5.1/src/tendril/utils/db.py` & `tendril-utils-db-0.5.2/src/tendril/utils/db.py`

 * *Files 3% similar despite different names*

```diff
@@ -39,14 +39,16 @@
 from contextlib import contextmanager
 import functools
 import arrow
 
 from tendril.utils.versions import get_namespace_package_names
 
 from tendril.config import DATABASE_URI
+from tendril.config import DATABASE_HOST
+from tendril.config import DATABASE_DB
 from tendril.config import DATABASE_PACKAGE_PREFIXES
 
 from tendril.utils import log
 logger = log.get_logger(__name__, log.DEBUG)
 log.logging.getLogger('sqlalchemy.engine').setLevel(log.WARNING)
 
 try:
@@ -283,7 +285,9 @@
 #: a complete ER diagram.
 #:
 #: Rendered by :mod:`sqlalchemyviz` into the following ER diagram.
 #:
 #: .. sqlaviz::
 #:     :metadataobject: tendril.utils.db.metadata
 metadata = get_metadata()
+
+logger.info(f"Using Database {DATABASE_DB} on Host {DATABASE_HOST}")
```

### Comparing `tendril-utils-db-0.5.1/src/tendril_utils_db.egg-info/PKG-INFO` & `tendril-utils-db-0.5.2/src/tendril_utils_db.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tendril-utils-db
-Version: 0.5.1
+Version: 0.5.2
 Summary: Database utilities for tendril
 Home-page: https://github.com/tendril-framework/tendril-utils-db
 Author: Chintalagiri Shashank
 Author-email: shashank@chintal.in
 Project-URL: Documentation, https://tendril-utils-db.readthedocs.io/en/latest
 Project-URL: Bug Tracker, https://github.com/tendril-framework/tendril-utils-db/issues
 Project-URL: Source Repository, https://github.com/tendril-framework/tendril-utils-db
```

### Comparing `tendril-utils-db-0.5.1/src/tendril_utils_db.egg-info/SOURCES.txt` & `tendril-utils-db-0.5.2/src/tendril_utils_db.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `tendril-utils-db-0.5.1/src/tendril_utils_db.egg-info/requires.txt` & `tendril-utils-db-0.5.2/src/tendril_utils_db.egg-info/requires.txt`

 * *Files identical despite different names*

### Comparing `tendril-utils-db-0.5.1/tests/coveralls.py` & `tendril-utils-db-0.5.2/tests/coveralls.py`

 * *Files identical despite different names*

### Comparing `tendril-utils-db-0.5.1/tox.ini` & `tendril-utils-db-0.5.2/tox.ini`

 * *Files identical despite different names*

