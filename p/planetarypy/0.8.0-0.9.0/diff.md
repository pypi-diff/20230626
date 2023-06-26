# Comparing `tmp/planetarypy-0.8.0.tar.gz` & `tmp/planetarypy-0.9.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/planetarypy-0.8.0.tar", last modified: Thu Jul 16 08:39:56 2020, max compression
+gzip compressed data, was "dist/planetarypy-0.9.0.tar", last modified: Fri Jul 24 13:10:43 2020, max compression
```

## Comparing `planetarypy-0.8.0.tar` & `planetarypy-0.9.0.tar`

### file list

```diff
@@ -1,65 +1,65 @@
-drwxrwxr-x   0 maye      (1000) maye      (1000)        0 2020-07-16 08:39:56.000000 planetarypy-0.8.0/
--rw-r--r--   0 maye      (1000) maye      (1000)      162 2015-07-11 04:02:26.000000 planetarypy-0.8.0/AUTHORS.rst
--rw-r--r--   0 maye      (1000) maye      (1000)     3210 2019-07-11 05:41:09.000000 planetarypy-0.8.0/CONTRIBUTING.rst
--rw-r--r--   0 maye      (1000) maye      (1000)      156 2016-12-20 10:16:51.000000 planetarypy-0.8.0/HISTORY.rst
--rw-r--r--   0 maye      (1000) maye      (1000)     1483 2019-07-11 05:41:41.000000 planetarypy-0.8.0/LICENSE
--rw-r--r--   0 maye      (1000) maye      (1000)      285 2019-07-11 05:41:41.000000 planetarypy-0.8.0/MANIFEST.in
--rw-rw-r--   0 maye      (1000) maye      (1000)     1813 2020-07-16 08:39:56.000000 planetarypy-0.8.0/PKG-INFO
--rw-r--r--   0 maye      (1000) maye      (1000)      625 2019-07-11 05:41:41.000000 planetarypy-0.8.0/README.rst
-drwxrwxr-x   0 maye      (1000) maye      (1000)        0 2020-07-16 08:39:56.000000 planetarypy-0.8.0/docs/
--rw-r--r--   0 maye      (1000) maye      (1000)     6782 2019-07-11 05:41:33.000000 planetarypy-0.8.0/docs/Makefile
--rw-r--r--   0 maye      (1000) maye      (1000)       28 2015-07-11 04:02:26.000000 planetarypy-0.8.0/docs/authors.rst
--rwxr--r--   0 maye      (1000) maye      (1000)     8447 2019-07-11 05:41:23.000000 planetarypy-0.8.0/docs/conf.py
--rw-r--r--   0 maye      (1000) maye      (1000)       33 2015-07-11 04:02:26.000000 planetarypy-0.8.0/docs/contributing.rst
--rw-r--r--   0 maye      (1000) maye      (1000)       28 2015-07-11 04:02:26.000000 planetarypy-0.8.0/docs/history.rst
--rw-r--r--   0 maye      (1000) maye      (1000)      509 2019-07-11 05:41:26.000000 planetarypy-0.8.0/docs/index.rst
--rw-r--r--   0 maye      (1000) maye      (1000)      203 2019-07-11 05:41:27.000000 planetarypy-0.8.0/docs/installation.rst
--rw-r--r--   0 maye      (1000) maye      (1000)     6469 2019-07-11 05:41:30.000000 planetarypy-0.8.0/docs/make.bat
--rw-r--r--   0 maye      (1000) maye      (1000)       27 2015-07-11 04:02:26.000000 planetarypy-0.8.0/docs/readme.rst
--rw-r--r--   0 maye      (1000) maye      (1000)       83 2019-07-11 05:41:41.000000 planetarypy-0.8.0/docs/usage.rst
-drwxrwxr-x   0 maye      (1000) maye      (1000)        0 2020-07-16 08:39:56.000000 planetarypy-0.8.0/planetarypy/
--rw-r--r--   0 maye      (1000) maye      (1000)      213 2020-07-16 08:39:27.000000 planetarypy-0.8.0/planetarypy/__init__.py
--rw-r--r--   0 maye      (1000) maye      (1000)     2073 2020-07-16 06:07:30.000000 planetarypy-0.8.0/planetarypy/_config.py
--rw-r--r--   0 maye      (1000) maye      (1000)      572 2015-04-20 16:52:14.000000 planetarypy-0.8.0/planetarypy/constants.py
--rw-r--r--   0 maye      (1000) maye      (1000)       30 2020-07-16 06:15:05.000000 planetarypy-0.8.0/planetarypy/dbmanager.py
--rw-r--r--   0 maye      (1000) maye      (1000)     1196 2020-07-16 07:01:58.000000 planetarypy-0.8.0/planetarypy/exceptions.py
--rw-r--r--   0 maye      (1000) maye      (1000)     2211 2015-04-20 19:31:33.000000 planetarypy-0.8.0/planetarypy/factsheet_parse.py
--rwxrwxr-x   0 maye      (1000) maye      (1000)    23089 2020-07-16 08:31:14.000000 planetarypy-0.8.0/planetarypy/geotools.py
--rwxrwxr-x   0 maye      (1000) maye      (1000)    23406 2020-07-16 06:05:48.000000 planetarypy-0.8.0/planetarypy/mars.py
-drwxrwxr-x   0 maye      (1000) maye      (1000)        0 2020-07-16 08:39:56.000000 planetarypy-0.8.0/planetarypy/pdstools/
--rw-r--r--   0 maye      (1000) maye      (1000)        0 2020-03-10 06:17:22.000000 planetarypy-0.8.0/planetarypy/pdstools/__init__.py
--rw-r--r--   0 maye      (1000) maye      (1000)       48 2019-07-11 05:44:16.000000 planetarypy-0.8.0/planetarypy/pdstools/atlas.py
--rw-r--r--   0 maye      (1000) maye      (1000)     3131 2020-03-10 00:02:05.000000 planetarypy-0.8.0/planetarypy/pdstools/cassini.py
--rw-r--r--   0 maye      (1000) maye      (1000)      907 2019-07-11 05:44:16.000000 planetarypy-0.8.0/planetarypy/pdstools/cli.py
-drwxrwxr-x   0 maye      (1000) maye      (1000)        0 2020-07-16 08:39:56.000000 planetarypy-0.8.0/planetarypy/pdstools/data/
--rw-r--r--   0 maye      (1000) maye      (1000)        0 2018-05-23 04:31:56.000000 planetarypy-0.8.0/planetarypy/pdstools/data/__init__.py
--rw-rw-r--   0 maye      (1000) maye      (1000)     2547 2020-07-16 05:45:51.000000 planetarypy-0.8.0/planetarypy/pdstools/data/pds_indices_db.toml
--rw-r--r--   0 maye      (1000) maye      (1000)    17914 2020-07-16 06:07:30.000000 planetarypy-0.8.0/planetarypy/pdstools/indices.py
--rw-r--r--   0 maye      (1000) maye      (1000)    12487 2018-04-27 02:05:23.000000 planetarypy-0.8.0/planetarypy/pdstools/opusapi.py
--rw-r--r--   0 maye      (1000) maye      (1000)     1477 2020-07-16 06:07:30.000000 planetarypy-0.8.0/planetarypy/pdstools/scraper.py
-drwxrwxr-x   0 maye      (1000) maye      (1000)        0 2020-07-16 08:39:56.000000 planetarypy-0.8.0/planetarypy/spicekernels/
--rw-r--r--   0 maye      (1000) maye      (1000)        0 2017-05-16 19:12:17.000000 planetarypy-0.8.0/planetarypy/spicekernels/__init__.py
--rw-r--r--   0 maye      (1000) maye      (1000)     8582 2017-05-17 01:31:10.000000 planetarypy-0.8.0/planetarypy/spicekernels/cassini.py
--rw-r--r--   0 maye      (1000) maye      (1000)      954 2017-05-16 19:26:45.000000 planetarypy-0.8.0/planetarypy/spicekernels/general.py
--rw-rw-r--   0 maye      (1000) maye      (1000)     5696 2020-07-16 06:05:48.000000 planetarypy-0.8.0/planetarypy/utils.py
-drwxrwxr-x   0 maye      (1000) maye      (1000)        0 2020-07-16 08:39:56.000000 planetarypy-0.8.0/planetarypy.egg-info/
--rw-rw-r--   0 maye      (1000) maye      (1000)     1813 2020-07-16 08:39:56.000000 planetarypy-0.8.0/planetarypy.egg-info/PKG-INFO
--rw-rw-r--   0 maye      (1000) maye      (1000)     1494 2020-07-16 08:39:56.000000 planetarypy-0.8.0/planetarypy.egg-info/SOURCES.txt
--rw-rw-r--   0 maye      (1000) maye      (1000)        1 2020-07-16 08:39:56.000000 planetarypy-0.8.0/planetarypy.egg-info/dependency_links.txt
--rw-rw-r--   0 maye      (1000) maye      (1000)      134 2020-07-16 08:39:56.000000 planetarypy-0.8.0/planetarypy.egg-info/entry_points.txt
--rw-rw-r--   0 maye      (1000) maye      (1000)        1 2020-07-16 08:39:56.000000 planetarypy-0.8.0/planetarypy.egg-info/not-zip-safe
--rw-rw-r--   0 maye      (1000) maye      (1000)      123 2020-07-16 08:39:56.000000 planetarypy-0.8.0/planetarypy.egg-info/requires.txt
--rw-rw-r--   0 maye      (1000) maye      (1000)       12 2020-07-16 08:39:56.000000 planetarypy-0.8.0/planetarypy.egg-info/top_level.txt
--rw-rw-r--   0 maye      (1000) maye      (1000)      198 2020-07-16 08:39:56.000000 planetarypy-0.8.0/setup.cfg
--rw-rw-r--   0 maye      (1000) maye      (1000)     1667 2020-07-16 08:39:27.000000 planetarypy-0.8.0/setup.py
-drwxrwxr-x   0 maye      (1000) maye      (1000)        0 2020-07-16 08:39:56.000000 planetarypy-0.8.0/tests/
-drwxrwxr-x   0 maye      (1000) maye      (1000)        0 2020-07-16 08:39:56.000000 planetarypy-0.8.0/tests/.ipynb_checkpoints/
--rw-r--r--   0 maye      (1000) maye      (1000)     7008 2018-08-10 20:33:31.000000 planetarypy-0.8.0/tests/.ipynb_checkpoints/test_io-checkpoint.ipynb
--rw-r--r--   0 maye      (1000) maye      (1000)     7681 2020-03-09 20:11:44.000000 planetarypy-0.8.0/tests/.ipynb_checkpoints/test_pds_tools_Index-checkpoint.ipynb
--rw-r--r--   0 maye      (1000) maye      (1000)    15129 2019-09-05 01:50:35.000000 planetarypy-0.8.0/tests/.ipynb_checkpoints/test_pdstools-checkpoint.ipynb
--rw-r--r--   0 maye      (1000) maye      (1000)     5375 2018-11-28 19:45:11.000000 planetarypy-0.8.0/tests/.ipynb_checkpoints/test_retrievers-checkpoint.ipynb
--rw-r--r--   0 maye      (1000) maye      (1000)     7121 2020-07-16 06:07:30.000000 planetarypy-0.8.0/tests/test_config.ipynb
--rw-r--r--   0 maye      (1000) maye      (1000)      179 2019-07-11 05:41:41.000000 planetarypy-0.8.0/tests/test_constants.py
--rw-r--r--   0 maye      (1000) maye      (1000)     7392 2020-07-16 06:07:30.000000 planetarypy-0.8.0/tests/test_pds_tools_Index.ipynb
--rw-r--r--   0 maye      (1000) maye      (1000)    18446 2020-07-16 06:07:30.000000 planetarypy-0.8.0/tests/test_pdstools.ipynb
--rw-r--r--   0 maye      (1000) maye      (1000)     5184 2020-07-16 06:07:30.000000 planetarypy-0.8.0/tests/test_retrievers.ipynb
+drwxrwxr-x   0 maye      (1000) maye      (1000)        0 2020-07-24 13:10:43.000000 planetarypy-0.9.0/
+-rw-r--r--   0 maye      (1000) maye      (1000)      162 2015-07-11 04:02:26.000000 planetarypy-0.9.0/AUTHORS.rst
+-rw-r--r--   0 maye      (1000) maye      (1000)     3210 2019-07-11 05:41:09.000000 planetarypy-0.9.0/CONTRIBUTING.rst
+-rw-r--r--   0 maye      (1000) maye      (1000)      156 2016-12-20 10:16:51.000000 planetarypy-0.9.0/HISTORY.rst
+-rw-r--r--   0 maye      (1000) maye      (1000)     1483 2019-07-11 05:41:41.000000 planetarypy-0.9.0/LICENSE
+-rw-r--r--   0 maye      (1000) maye      (1000)      285 2019-07-11 05:41:41.000000 planetarypy-0.9.0/MANIFEST.in
+-rw-rw-r--   0 maye      (1000) maye      (1000)     1813 2020-07-24 13:10:43.000000 planetarypy-0.9.0/PKG-INFO
+-rw-r--r--   0 maye      (1000) maye      (1000)      625 2019-07-11 05:41:41.000000 planetarypy-0.9.0/README.rst
+drwxrwxr-x   0 maye      (1000) maye      (1000)        0 2020-07-24 13:10:43.000000 planetarypy-0.9.0/docs/
+-rw-r--r--   0 maye      (1000) maye      (1000)     6782 2019-07-11 05:41:33.000000 planetarypy-0.9.0/docs/Makefile
+-rw-r--r--   0 maye      (1000) maye      (1000)       28 2015-07-11 04:02:26.000000 planetarypy-0.9.0/docs/authors.rst
+-rwxr--r--   0 maye      (1000) maye      (1000)     8447 2019-07-11 05:41:23.000000 planetarypy-0.9.0/docs/conf.py
+-rw-r--r--   0 maye      (1000) maye      (1000)       33 2015-07-11 04:02:26.000000 planetarypy-0.9.0/docs/contributing.rst
+-rw-r--r--   0 maye      (1000) maye      (1000)       28 2015-07-11 04:02:26.000000 planetarypy-0.9.0/docs/history.rst
+-rw-r--r--   0 maye      (1000) maye      (1000)      509 2019-07-11 05:41:26.000000 planetarypy-0.9.0/docs/index.rst
+-rw-r--r--   0 maye      (1000) maye      (1000)      203 2019-07-11 05:41:27.000000 planetarypy-0.9.0/docs/installation.rst
+-rw-r--r--   0 maye      (1000) maye      (1000)     6469 2019-07-11 05:41:30.000000 planetarypy-0.9.0/docs/make.bat
+-rw-r--r--   0 maye      (1000) maye      (1000)       27 2015-07-11 04:02:26.000000 planetarypy-0.9.0/docs/readme.rst
+-rw-r--r--   0 maye      (1000) maye      (1000)       83 2019-07-11 05:41:41.000000 planetarypy-0.9.0/docs/usage.rst
+drwxrwxr-x   0 maye      (1000) maye      (1000)        0 2020-07-24 13:10:43.000000 planetarypy-0.9.0/planetarypy/
+-rw-r--r--   0 maye      (1000) maye      (1000)      213 2020-07-24 13:10:22.000000 planetarypy-0.9.0/planetarypy/__init__.py
+-rw-r--r--   0 maye      (1000) maye      (1000)     2073 2020-07-16 06:07:30.000000 planetarypy-0.9.0/planetarypy/_config.py
+-rw-r--r--   0 maye      (1000) maye      (1000)      572 2015-04-20 16:52:14.000000 planetarypy-0.9.0/planetarypy/constants.py
+-rw-r--r--   0 maye      (1000) maye      (1000)       30 2020-07-16 06:15:05.000000 planetarypy-0.9.0/planetarypy/dbmanager.py
+-rw-r--r--   0 maye      (1000) maye      (1000)     1196 2020-07-16 07:01:58.000000 planetarypy-0.9.0/planetarypy/exceptions.py
+-rw-r--r--   0 maye      (1000) maye      (1000)     2211 2015-04-20 19:31:33.000000 planetarypy-0.9.0/planetarypy/factsheet_parse.py
+-rwxrwxr-x   0 maye      (1000) maye      (1000)    24912 2020-07-24 08:11:48.000000 planetarypy-0.9.0/planetarypy/geotools.py
+-rwxrwxr-x   0 maye      (1000) maye      (1000)    23406 2020-07-16 06:05:48.000000 planetarypy-0.9.0/planetarypy/mars.py
+drwxrwxr-x   0 maye      (1000) maye      (1000)        0 2020-07-24 13:10:43.000000 planetarypy-0.9.0/planetarypy/pdstools/
+-rw-r--r--   0 maye      (1000) maye      (1000)        0 2020-03-10 06:17:22.000000 planetarypy-0.9.0/planetarypy/pdstools/__init__.py
+-rw-r--r--   0 maye      (1000) maye      (1000)       48 2019-07-11 05:44:16.000000 planetarypy-0.9.0/planetarypy/pdstools/atlas.py
+-rw-r--r--   0 maye      (1000) maye      (1000)     3131 2020-03-10 00:02:05.000000 planetarypy-0.9.0/planetarypy/pdstools/cassini.py
+-rw-r--r--   0 maye      (1000) maye      (1000)      907 2019-07-11 05:44:16.000000 planetarypy-0.9.0/planetarypy/pdstools/cli.py
+drwxrwxr-x   0 maye      (1000) maye      (1000)        0 2020-07-24 13:10:43.000000 planetarypy-0.9.0/planetarypy/pdstools/data/
+-rw-r--r--   0 maye      (1000) maye      (1000)        0 2018-05-23 04:31:56.000000 planetarypy-0.9.0/planetarypy/pdstools/data/__init__.py
+-rw-rw-r--   0 maye      (1000) maye      (1000)     2547 2020-07-16 05:45:51.000000 planetarypy-0.9.0/planetarypy/pdstools/data/pds_indices_db.toml
+-rw-r--r--   0 maye      (1000) maye      (1000)    17914 2020-07-16 06:07:30.000000 planetarypy-0.9.0/planetarypy/pdstools/indices.py
+-rw-r--r--   0 maye      (1000) maye      (1000)    12487 2018-04-27 02:05:23.000000 planetarypy-0.9.0/planetarypy/pdstools/opusapi.py
+-rw-r--r--   0 maye      (1000) maye      (1000)     1477 2020-07-16 06:07:30.000000 planetarypy-0.9.0/planetarypy/pdstools/scraper.py
+drwxrwxr-x   0 maye      (1000) maye      (1000)        0 2020-07-24 13:10:43.000000 planetarypy-0.9.0/planetarypy/spicekernels/
+-rw-r--r--   0 maye      (1000) maye      (1000)        0 2017-05-16 19:12:17.000000 planetarypy-0.9.0/planetarypy/spicekernels/__init__.py
+-rw-r--r--   0 maye      (1000) maye      (1000)     8582 2017-05-17 01:31:10.000000 planetarypy-0.9.0/planetarypy/spicekernels/cassini.py
+-rw-r--r--   0 maye      (1000) maye      (1000)      954 2017-05-16 19:26:45.000000 planetarypy-0.9.0/planetarypy/spicekernels/general.py
+-rw-rw-r--   0 maye      (1000) maye      (1000)     5696 2020-07-24 13:08:14.000000 planetarypy-0.9.0/planetarypy/utils.py
+drwxrwxr-x   0 maye      (1000) maye      (1000)        0 2020-07-24 13:10:43.000000 planetarypy-0.9.0/planetarypy.egg-info/
+-rw-rw-r--   0 maye      (1000) maye      (1000)     1813 2020-07-24 13:10:43.000000 planetarypy-0.9.0/planetarypy.egg-info/PKG-INFO
+-rw-rw-r--   0 maye      (1000) maye      (1000)     1494 2020-07-24 13:10:43.000000 planetarypy-0.9.0/planetarypy.egg-info/SOURCES.txt
+-rw-rw-r--   0 maye      (1000) maye      (1000)        1 2020-07-24 13:10:43.000000 planetarypy-0.9.0/planetarypy.egg-info/dependency_links.txt
+-rw-rw-r--   0 maye      (1000) maye      (1000)      134 2020-07-24 13:10:43.000000 planetarypy-0.9.0/planetarypy.egg-info/entry_points.txt
+-rw-rw-r--   0 maye      (1000) maye      (1000)        1 2020-07-24 13:10:43.000000 planetarypy-0.9.0/planetarypy.egg-info/not-zip-safe
+-rw-rw-r--   0 maye      (1000) maye      (1000)      123 2020-07-24 13:10:43.000000 planetarypy-0.9.0/planetarypy.egg-info/requires.txt
+-rw-rw-r--   0 maye      (1000) maye      (1000)       12 2020-07-24 13:10:43.000000 planetarypy-0.9.0/planetarypy.egg-info/top_level.txt
+-rw-rw-r--   0 maye      (1000) maye      (1000)      198 2020-07-24 13:10:43.000000 planetarypy-0.9.0/setup.cfg
+-rw-rw-r--   0 maye      (1000) maye      (1000)     1667 2020-07-24 13:10:22.000000 planetarypy-0.9.0/setup.py
+drwxrwxr-x   0 maye      (1000) maye      (1000)        0 2020-07-24 13:10:43.000000 planetarypy-0.9.0/tests/
+drwxrwxr-x   0 maye      (1000) maye      (1000)        0 2020-07-24 13:10:43.000000 planetarypy-0.9.0/tests/.ipynb_checkpoints/
+-rw-r--r--   0 maye      (1000) maye      (1000)     7008 2018-08-10 20:33:31.000000 planetarypy-0.9.0/tests/.ipynb_checkpoints/test_io-checkpoint.ipynb
+-rw-r--r--   0 maye      (1000) maye      (1000)     7681 2020-03-09 20:11:44.000000 planetarypy-0.9.0/tests/.ipynb_checkpoints/test_pds_tools_Index-checkpoint.ipynb
+-rw-r--r--   0 maye      (1000) maye      (1000)    15129 2019-09-05 01:50:35.000000 planetarypy-0.9.0/tests/.ipynb_checkpoints/test_pdstools-checkpoint.ipynb
+-rw-r--r--   0 maye      (1000) maye      (1000)     5375 2018-11-28 19:45:11.000000 planetarypy-0.9.0/tests/.ipynb_checkpoints/test_retrievers-checkpoint.ipynb
+-rw-r--r--   0 maye      (1000) maye      (1000)     7121 2020-07-16 06:07:30.000000 planetarypy-0.9.0/tests/test_config.ipynb
+-rw-r--r--   0 maye      (1000) maye      (1000)      179 2019-07-11 05:41:41.000000 planetarypy-0.9.0/tests/test_constants.py
+-rw-r--r--   0 maye      (1000) maye      (1000)     7392 2020-07-16 06:07:30.000000 planetarypy-0.9.0/tests/test_pds_tools_Index.ipynb
+-rw-r--r--   0 maye      (1000) maye      (1000)    18446 2020-07-16 06:07:30.000000 planetarypy-0.9.0/tests/test_pdstools.ipynb
+-rw-r--r--   0 maye      (1000) maye      (1000)     5184 2020-07-16 06:07:30.000000 planetarypy-0.9.0/tests/test_retrievers.ipynb
```

### Comparing `planetarypy-0.8.0/CONTRIBUTING.rst` & `planetarypy-0.9.0/CONTRIBUTING.rst`

 * *Files identical despite different names*

### Comparing `planetarypy-0.8.0/LICENSE` & `planetarypy-0.9.0/LICENSE`

 * *Files identical despite different names*

### Comparing `planetarypy-0.8.0/PKG-INFO` & `planetarypy-0.9.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.2
 Name: planetarypy
-Version: 0.8.0
+Version: 0.9.0
 Summary: Python module to support analysis of planetary data.
 Home-page: https://github.com/michaelaye/planetarypy
 Author: K.-Michael Aye
 Author-email: kmichael.aye@gmail.com
 License: ISC
 Description: ===============================
         planetarypy
```

### Comparing `planetarypy-0.8.0/README.rst` & `planetarypy-0.9.0/README.rst`

 * *Files identical despite different names*

### Comparing `planetarypy-0.8.0/docs/Makefile` & `planetarypy-0.9.0/docs/Makefile`

 * *Files identical despite different names*

### Comparing `planetarypy-0.8.0/docs/conf.py` & `planetarypy-0.9.0/docs/conf.py`

 * *Files identical despite different names*

### Comparing `planetarypy-0.8.0/docs/make.bat` & `planetarypy-0.9.0/docs/make.bat`

 * *Files identical despite different names*

### Comparing `planetarypy-0.8.0/planetarypy/_config.py` & `planetarypy-0.9.0/planetarypy/_config.py`

 * *Files identical despite different names*

### Comparing `planetarypy-0.8.0/planetarypy/constants.py` & `planetarypy-0.9.0/planetarypy/constants.py`

 * *Files identical despite different names*

### Comparing `planetarypy-0.8.0/planetarypy/exceptions.py` & `planetarypy-0.9.0/planetarypy/exceptions.py`

 * *Files identical despite different names*

### Comparing `planetarypy-0.8.0/planetarypy/factsheet_parse.py` & `planetarypy-0.9.0/planetarypy/factsheet_parse.py`

 * *Files identical despite different names*

### Comparing `planetarypy-0.8.0/planetarypy/geotools.py` & `planetarypy-0.9.0/planetarypy/geotools.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,12 @@
 # encoding: utf-8
 """
 Some tools to work with geo data.
+GDAL required!
+
 Abbreviations:
 ul = Upper Left
 lr = LowerRight
 
 Copyright (c) 2011 Klaus-Michael Aye. All rights reserved.
 """
 
@@ -23,41 +25,90 @@
 
 gdal.UseExceptions()
 
 
 def calculate_image_azimuth(origPoint, newPoint, zero="right"):
     """Calculate azimuth angle between 2 image points.
 
+    Beware that this function calculates trigonometric angles.
+    If the points are from an image that has (0, 0) in the upper left, this means
+    that the angles increase clockwise.
+    That is why, for example, for an HiRISE image, the return of this function
+    matches the angle rotation definition for HiRISE data.
+
     Parameters
     ==========
     origPoint, newPoint: <mars.Point> objects
     zero: <string>
         right' or 'top' to indicate where zero is.
 
     Returns
     =======
-    azimuth: <float> azimuth angle
+    azimuth: <float>
+        Azimuth angle
     """
     deltaSample = newPoint.sample - origPoint.sample
     deltaLine = newPoint.line - origPoint.line
 
-    azimuth = degrees(atan2(deltaLine, deltaSample))
+    azimuth = np.degrees(np.arctan2(deltaLine, deltaSample))
 
     if azimuth < 0.0:
         azimuth += 360.0
     if azimuth > 360.0:
         azimuth -= 360.0
     if zero == "top":
         azimuth += 90.0
         if azimuth > 360.0:
             azimuth -= 360.0
 
     return azimuth
 
 
+def get_north_shifted_point(img, offset=0.001):
+    "Increasing the latitude is a sure way of getting north."
+    newPoint = Point(lon=img.center.lon, lat=img.center.lat + offset)
+    newPoint.lonlat_to_pixel(img.geotrans, img.projection)
+    return newPoint
+
+
+def calculate_image_north_azimuth(img, zero="right"):
+    newPoint = get_north_shifted_point(img)
+    return img.center.calculate_azimuth(newPoint, zero=zero)
+
+
+def get_sun_angles(spicer, img):
+    """Calculate solar azimuth and incidence.
+    
+    By requiring a spicer object for this function, it becomes independent from the
+    solar system object where the calculations are made.
+
+    Parameters
+    ----------
+    spicer : spicer.Spicer
+        needs to be setup for time, but spoint is set from img.center in here.
+    img : geotools.ImgData
+        The image data of which the center point serves as the start point.
+    
+    Returns
+    -------
+    tuple(float, float)
+        Solar azimuth, incidence [degrees]
+    """
+    p = img.center
+    spicer.set_spoint_by(lat=p.lat, lon=p.lon)
+    p2lon, p2lat = spicer.point_towards_sun(pixel_res=1)
+    p2 = Point.copy_geodata(p, lat=p2lat.value, lon=p2lon.value)
+    p2.lonlat_to_pixel()
+    # remember, this calculates CCW angles, but if image is "origin='upper'",
+    # it becomes CW
+    sun_az = p.calculate_azimuth(p2)
+    sun_inc = spicer.illum_angles.dsolar
+    return sun_az, sun_inc.value
+
+
 def debug_srs(projection):
     """Correct wrong scale_factor in PolarStereographic data.
 
     Some PolarStereographic data have a 0 as a scale_factor in the
     projection (mostly MOLA), which is being corrected here.
     TODO: Check for being PolarStereographic before doing this!
     """
@@ -668,39 +719,39 @@
 #                              min(ulY,lrY),
 #                              max(ulY,lrY)),
 #                      origin='image' )
 #     plt.clabel(CS,fontsize=9, inline=1)
 #     plt.show()
 
 
-def main(argv=None):
-    """docstring for main"""
-    from mayavi import mlab
-
-    if argv is None:
-        argv = sys.argv
-
-    x1 = x2 = y1 = y2 = 0
-    fname = ""
-    try:
-        fname = argv[1]
-        x1, x2, y1, y2 = [int(i) for i in argv[2:]]
-    except:
-        print("Usage: {0} fname x1 x2 y1 y2".format(argv[0]))
-
-    print(x1, x2, y1, y2)
-    ds = gdal.Open(fname)
-    band = ds.GetRasterBand(1)
-    STORED_VALUE = band.ReadAsArray(x1, y1, x2 - x1, y2 - y1)
-    ds = 0
-
-    # PDS label infos:
-    SCALING_FACTOR = 0.25
-    OFFSET = -8000
-    topo = (STORED_VALUE * SCALING_FACTOR) + OFFSET
-    mlab.surf(topo, warp_scale=1 / 115.0, vmin=1700)
-    mlab.colorbar(orientation="vertical", title="Height [m]", label_fmt="%4.0f")
-    mlab.show()
+# def main(argv=None):
+#     """docstring for main"""
+#     from mayavi import mlab
+
+#     if argv is None:
+#         argv = sys.argv
+
+#     x1 = x2 = y1 = y2 = 0
+#     fname = ""
+#     try:
+#         fname = argv[1]
+#         x1, x2, y1, y2 = [int(i) for i in argv[2:]]
+#     except:
+#         print("Usage: {0} fname x1 x2 y1 y2".format(argv[0]))
+
+#     print(x1, x2, y1, y2)
+#     ds = gdal.Open(fname)
+#     band = ds.GetRasterBand(1)
+#     STORED_VALUE = band.ReadAsArray(x1, y1, x2 - x1, y2 - y1)
+#     ds = 0
+
+#     # PDS label infos:
+#     SCALING_FACTOR = 0.25
+#     OFFSET = -8000
+#     topo = (STORED_VALUE * SCALING_FACTOR) + OFFSET
+#     mlab.surf(topo, warp_scale=1 / 115.0, vmin=1700)
+#     mlab.colorbar(orientation="vertical", title="Height [m]", label_fmt="%4.0f")
+#     mlab.show()
 
 
-if __name__ == "__main__":
-    sys.exit(main())
+# if __name__ == "__main__":
+#     sys.exit(main())
```

### Comparing `planetarypy-0.8.0/planetarypy/mars.py` & `planetarypy-0.9.0/planetarypy/mars.py`

 * *Files identical despite different names*

### Comparing `planetarypy-0.8.0/planetarypy/pdstools/cassini.py` & `planetarypy-0.9.0/planetarypy/pdstools/cassini.py`

 * *Files identical despite different names*

### Comparing `planetarypy-0.8.0/planetarypy/pdstools/cli.py` & `planetarypy-0.9.0/planetarypy/pdstools/cli.py`

 * *Files identical despite different names*

### Comparing `planetarypy-0.8.0/planetarypy/pdstools/data/pds_indices_db.toml` & `planetarypy-0.9.0/planetarypy/pdstools/data/pds_indices_db.toml`

 * *Files identical despite different names*

### Comparing `planetarypy-0.8.0/planetarypy/pdstools/indices.py` & `planetarypy-0.9.0/planetarypy/pdstools/indices.py`

 * *Files identical despite different names*

### Comparing `planetarypy-0.8.0/planetarypy/pdstools/opusapi.py` & `planetarypy-0.9.0/planetarypy/pdstools/opusapi.py`

 * *Files identical despite different names*

### Comparing `planetarypy-0.8.0/planetarypy/pdstools/scraper.py` & `planetarypy-0.9.0/planetarypy/pdstools/scraper.py`

 * *Files identical despite different names*

### Comparing `planetarypy-0.8.0/planetarypy/spicekernels/cassini.py` & `planetarypy-0.9.0/planetarypy/spicekernels/cassini.py`

 * *Files identical despite different names*

### Comparing `planetarypy-0.8.0/planetarypy/spicekernels/general.py` & `planetarypy-0.9.0/planetarypy/spicekernels/general.py`

 * *Files identical despite different names*

### Comparing `planetarypy-0.8.0/planetarypy/utils.py` & `planetarypy-0.9.0/planetarypy/utils.py`

 * *Files identical despite different names*

### Comparing `planetarypy-0.8.0/planetarypy.egg-info/PKG-INFO` & `planetarypy-0.9.0/planetarypy.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.2
 Name: planetarypy
-Version: 0.8.0
+Version: 0.9.0
 Summary: Python module to support analysis of planetary data.
 Home-page: https://github.com/michaelaye/planetarypy
 Author: K.-Michael Aye
 Author-email: kmichael.aye@gmail.com
 License: ISC
 Description: ===============================
         planetarypy
```

### Comparing `planetarypy-0.8.0/planetarypy.egg-info/SOURCES.txt` & `planetarypy-0.9.0/planetarypy.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `planetarypy-0.8.0/setup.py` & `planetarypy-0.9.0/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -11,15 +11,15 @@
     readme = readme_file.read()
 
 with open("HISTORY.rst") as history_file:
     history = history_file.read().replace(".. :changelog:", "")
 
 setup(
     name="planetarypy",
-    version="0.8.0",
+    version="0.9.0",
     description="Python module to support analysis of planetary data.",
     long_description=readme + "\n\n" + history,
     author="K.-Michael Aye",
     author_email="kmichael.aye@gmail.com",
     url="https://github.com/michaelaye/planetarypy",
     packages=find_packages(),
     include_package_data=True,
```

### Comparing `planetarypy-0.8.0/tests/.ipynb_checkpoints/test_io-checkpoint.ipynb` & `planetarypy-0.9.0/tests/.ipynb_checkpoints/test_io-checkpoint.ipynb`

 * *Files identical despite different names*

### Comparing `planetarypy-0.8.0/tests/.ipynb_checkpoints/test_pds_tools_Index-checkpoint.ipynb` & `planetarypy-0.9.0/tests/.ipynb_checkpoints/test_pds_tools_Index-checkpoint.ipynb`

 * *Files identical despite different names*

### Comparing `planetarypy-0.8.0/tests/.ipynb_checkpoints/test_pdstools-checkpoint.ipynb` & `planetarypy-0.9.0/tests/.ipynb_checkpoints/test_pdstools-checkpoint.ipynb`

 * *Files identical despite different names*

### Comparing `planetarypy-0.8.0/tests/.ipynb_checkpoints/test_retrievers-checkpoint.ipynb` & `planetarypy-0.9.0/tests/.ipynb_checkpoints/test_retrievers-checkpoint.ipynb`

 * *Files identical despite different names*

### Comparing `planetarypy-0.8.0/tests/test_config.ipynb` & `planetarypy-0.9.0/tests/test_config.ipynb`

 * *Files identical despite different names*

### Comparing `planetarypy-0.8.0/tests/test_pds_tools_Index.ipynb` & `planetarypy-0.9.0/tests/test_pds_tools_Index.ipynb`

 * *Files identical despite different names*

### Comparing `planetarypy-0.8.0/tests/test_pdstools.ipynb` & `planetarypy-0.9.0/tests/test_pdstools.ipynb`

 * *Files identical despite different names*

### Comparing `planetarypy-0.8.0/tests/test_retrievers.ipynb` & `planetarypy-0.9.0/tests/test_retrievers.ipynb`

 * *Files identical despite different names*

