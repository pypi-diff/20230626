# Comparing `tmp/airflow-provider-duckdb-0.1.1a9.tar.gz` & `tmp/airflow-provider-duckdb-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "airflow-provider-duckdb-0.1.1a9.tar", last modified: Mon Jun 26 20:30:58 2023, max compression
+gzip compressed data, was "airflow-provider-duckdb-0.2.0.tar", last modified: Mon Jun 26 21:02:51 2023, max compression
```

## Comparing `airflow-provider-duckdb-0.1.1a9.tar` & `airflow-provider-duckdb-0.2.0.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxr-xr-x   0 julian     (502) staff       (20)        0 2023-06-26 20:30:58.099434 airflow-provider-duckdb-0.1.1a9/
--rw-r--r--   0 julian     (502) staff       (20)    11357 2022-10-30 21:15:10.000000 airflow-provider-duckdb-0.1.1a9/LICENSE
--rw-r--r--   0 julian     (502) staff       (20)     3077 2023-06-26 20:30:58.099232 airflow-provider-duckdb-0.1.1a9/PKG-INFO
--rw-r--r--   0 julian     (502) staff       (20)     2655 2023-06-21 17:25:11.000000 airflow-provider-duckdb-0.1.1a9/README.md
-drwxr-xr-x   0 julian     (502) staff       (20)        0 2023-06-26 20:30:58.098394 airflow-provider-duckdb-0.1.1a9/airflow_provider_duckdb.egg-info/
--rw-r--r--   0 julian     (502) staff       (20)     3077 2023-06-26 20:30:58.000000 airflow-provider-duckdb-0.1.1a9/airflow_provider_duckdb.egg-info/PKG-INFO
--rw-r--r--   0 julian     (502) staff       (20)      409 2023-06-26 20:30:58.000000 airflow-provider-duckdb-0.1.1a9/airflow_provider_duckdb.egg-info/SOURCES.txt
--rw-r--r--   0 julian     (502) staff       (20)        1 2023-06-26 20:30:58.000000 airflow-provider-duckdb-0.1.1a9/airflow_provider_duckdb.egg-info/dependency_links.txt
--rw-r--r--   0 julian     (502) staff       (20)       85 2023-06-26 20:30:58.000000 airflow-provider-duckdb-0.1.1a9/airflow_provider_duckdb.egg-info/entry_points.txt
--rw-r--r--   0 julian     (502) staff       (20)       48 2023-06-26 20:30:58.000000 airflow-provider-duckdb-0.1.1a9/airflow_provider_duckdb.egg-info/requires.txt
--rw-r--r--   0 julian     (502) staff       (20)       16 2023-06-26 20:30:58.000000 airflow-provider-duckdb-0.1.1a9/airflow_provider_duckdb.egg-info/top_level.txt
-drwxr-xr-x   0 julian     (502) staff       (20)        0 2023-06-26 20:30:58.098577 airflow-provider-duckdb-0.1.1a9/duckdb_provider/
--rw-r--r--   0 julian     (502) staff       (20)      471 2023-05-02 14:52:15.000000 airflow-provider-duckdb-0.1.1a9/duckdb_provider/__init__.py
-drwxr-xr-x   0 julian     (502) staff       (20)        0 2023-06-26 20:30:58.099005 airflow-provider-duckdb-0.1.1a9/duckdb_provider/hooks/
--rw-r--r--   0 julian     (502) staff       (20)        0 2022-10-30 21:28:31.000000 airflow-provider-duckdb-0.1.1a9/duckdb_provider/hooks/__init__.py
--rw-r--r--   0 julian     (502) staff       (20)     2782 2023-06-26 20:30:48.000000 airflow-provider-duckdb-0.1.1a9/duckdb_provider/hooks/duckdb_hook.py
--rw-r--r--   0 julian     (502) staff       (20)       38 2023-06-26 20:30:58.099485 airflow-provider-duckdb-0.1.1a9/setup.cfg
--rw-r--r--   0 julian     (502) staff       (20)      946 2023-06-26 20:30:51.000000 airflow-provider-duckdb-0.1.1a9/setup.py
+drwxr-xr-x   0 julian     (502) staff       (20)        0 2023-06-26 21:02:51.569235 airflow-provider-duckdb-0.2.0/
+-rw-r--r--   0 julian     (502) staff       (20)    11357 2022-10-30 21:15:10.000000 airflow-provider-duckdb-0.2.0/LICENSE
+-rw-r--r--   0 julian     (502) staff       (20)     4280 2023-06-26 21:02:51.569020 airflow-provider-duckdb-0.2.0/PKG-INFO
+-rw-r--r--   0 julian     (502) staff       (20)     3860 2023-06-26 21:01:50.000000 airflow-provider-duckdb-0.2.0/README.md
+drwxr-xr-x   0 julian     (502) staff       (20)        0 2023-06-26 21:02:51.567089 airflow-provider-duckdb-0.2.0/airflow_provider_duckdb.egg-info/
+-rw-r--r--   0 julian     (502) staff       (20)     4280 2023-06-26 21:02:51.000000 airflow-provider-duckdb-0.2.0/airflow_provider_duckdb.egg-info/PKG-INFO
+-rw-r--r--   0 julian     (502) staff       (20)      409 2023-06-26 21:02:51.000000 airflow-provider-duckdb-0.2.0/airflow_provider_duckdb.egg-info/SOURCES.txt
+-rw-r--r--   0 julian     (502) staff       (20)        1 2023-06-26 21:02:51.000000 airflow-provider-duckdb-0.2.0/airflow_provider_duckdb.egg-info/dependency_links.txt
+-rw-r--r--   0 julian     (502) staff       (20)       85 2023-06-26 21:02:51.000000 airflow-provider-duckdb-0.2.0/airflow_provider_duckdb.egg-info/entry_points.txt
+-rw-r--r--   0 julian     (502) staff       (20)       48 2023-06-26 21:02:51.000000 airflow-provider-duckdb-0.2.0/airflow_provider_duckdb.egg-info/requires.txt
+-rw-r--r--   0 julian     (502) staff       (20)       16 2023-06-26 21:02:51.000000 airflow-provider-duckdb-0.2.0/airflow_provider_duckdb.egg-info/top_level.txt
+drwxr-xr-x   0 julian     (502) staff       (20)        0 2023-06-26 21:02:51.567459 airflow-provider-duckdb-0.2.0/duckdb_provider/
+-rw-r--r--   0 julian     (502) staff       (20)      471 2023-05-02 14:52:15.000000 airflow-provider-duckdb-0.2.0/duckdb_provider/__init__.py
+drwxr-xr-x   0 julian     (502) staff       (20)        0 2023-06-26 21:02:51.568567 airflow-provider-duckdb-0.2.0/duckdb_provider/hooks/
+-rw-r--r--   0 julian     (502) staff       (20)        0 2022-10-30 21:28:31.000000 airflow-provider-duckdb-0.2.0/duckdb_provider/hooks/__init__.py
+-rw-r--r--   0 julian     (502) staff       (20)     2782 2023-06-26 20:55:58.000000 airflow-provider-duckdb-0.2.0/duckdb_provider/hooks/duckdb_hook.py
+-rw-r--r--   0 julian     (502) staff       (20)       38 2023-06-26 21:02:51.569288 airflow-provider-duckdb-0.2.0/setup.cfg
+-rw-r--r--   0 julian     (502) staff       (20)      944 2023-06-26 20:54:03.000000 airflow-provider-duckdb-0.2.0/setup.py
```

### Comparing `airflow-provider-duckdb-0.1.1a9/LICENSE` & `airflow-provider-duckdb-0.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `airflow-provider-duckdb-0.1.1a9/duckdb_provider/hooks/duckdb_hook.py` & `airflow-provider-duckdb-0.2.0/duckdb_provider/hooks/duckdb_hook.py`

 * *Files identical despite different names*

### Comparing `airflow-provider-duckdb-0.1.1a9/setup.py` & `airflow-provider-duckdb-0.2.0/setup.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from setuptools import find_packages, setup
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 setup(
     name="airflow-provider-duckdb",
-    version="0.1.1a9",
+    version="0.2.0",
     description="DuckDB (duckdb.org) provider for Apache Airflow",
     long_description=long_description,
     long_description_content_type="text/markdown",
     entry_points={
         "apache_airflow_provider": [
             "provider_info=duckdb_provider.__init__:get_provider_info"
         ]
```

