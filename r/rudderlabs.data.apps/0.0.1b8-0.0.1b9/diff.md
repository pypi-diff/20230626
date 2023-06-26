# Comparing `tmp/rudderlabs.data.apps-0.0.1b8.tar.gz` & `tmp/rudderlabs.data.apps-0.0.1b9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "/home/runner/work/rudderlabs.data.apps/rudderlabs.data.apps/dist/tmpa8gzhc5b/rudderlabs.data.apps-0.0.1b8.tar", last modified: Thu Jul 21 03:06:40 2022, max compression
+gzip compressed data, was "/home/runner/work/rudderlabs.data.apps/rudderlabs.data.apps/dist/tmptoo6ld37/rudderlabs.data.apps-0.0.1b9.tar", last modified: Thu Jul 21 03:12:59 2022, max compression
```

## Comparing `rudderlabs.data.apps-0.0.1b8.tar` & `rudderlabs.data.apps-0.0.1b9.tar`

### file list

```diff
@@ -1,79 +1,80 @@
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-07-21 03:06:40.000000 rudderlabs.data.apps-0.0.1b8/
--rw-r--r--   0 runner    (1001) docker     (121)    35147 2022-07-21 03:06:24.000000 rudderlabs.data.apps-0.0.1b8/COPYING
--rw-r--r--   0 runner    (1001) docker     (121)      225 2022-07-21 03:06:24.000000 rudderlabs.data.apps-0.0.1b8/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (121)     1869 2022-07-21 03:06:40.000000 rudderlabs.data.apps-0.0.1b8/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)     1312 2022-07-21 03:06:24.000000 rudderlabs.data.apps-0.0.1b8/README.rst
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-07-21 03:06:40.000000 rudderlabs.data.apps-0.0.1b8/docs/
--rwxr-xr-x   0 runner    (1001) docker     (121)     1421 2022-07-21 03:06:24.000000 rudderlabs.data.apps-0.0.1b8/docs/api.rst
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-07-21 03:06:40.000000 rudderlabs.data.apps-0.0.1b8/docs/img/
--rw-r--r--   0 runner    (1001) docker     (121)    15406 2022-07-21 03:06:24.000000 rudderlabs.data.apps-0.0.1b8/docs/img/favicon.ico
--rw-r--r--   0 runner    (1001) docker     (121)    21769 2022-07-21 03:06:24.000000 rudderlabs.data.apps-0.0.1b8/docs/img/logo.png
--rw-r--r--   0 runner    (1001) docker     (121)    43455 2022-07-21 03:06:24.000000 rudderlabs.data.apps-0.0.1b8/docs/img/run_pipeline_flow_diagram.png
--rw-r--r--   0 runner    (1001) docker     (121)      479 2022-07-21 03:06:24.000000 rudderlabs.data.apps-0.0.1b8/docs/index.rst
--rw-r--r--   0 runner    (1001) docker     (121)      908 2022-07-21 03:06:24.000000 rudderlabs.data.apps-0.0.1b8/docs/install.rst
--rwxr-xr-x   0 runner    (1001) docker     (121)      288 2022-07-21 03:06:24.000000 rudderlabs.data.apps-0.0.1b8/docs/links.rst
--rw-r--r--   0 runner    (1001) docker     (121)     3008 2022-07-21 03:06:24.000000 rudderlabs.data.apps-0.0.1b8/docs/new_data_app_repo.rst
--rw-r--r--   0 runner    (1001) docker     (121)     2177 2022-07-21 03:06:24.000000 rudderlabs.data.apps-0.0.1b8/docs/sagemaker.rst
--rwxr-xr-x   0 runner    (1001) docker     (121)      243 2022-07-21 03:06:24.000000 rudderlabs.data.apps-0.0.1b8/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (121)       47 2022-07-21 03:06:24.000000 rudderlabs.data.apps-0.0.1b8/requirements.txt
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-07-21 03:06:40.000000 rudderlabs.data.apps-0.0.1b8/rudderlabs/
--rw-r--r--   0 runner    (1001) docker     (121)      129 2022-07-21 03:06:24.000000 rudderlabs.data.apps-0.0.1b8/rudderlabs/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-07-21 03:06:40.000000 rudderlabs.data.apps-0.0.1b8/rudderlabs/data/
--rw-r--r--   0 runner    (1001) docker     (121)      129 2022-07-21 03:06:24.000000 rudderlabs.data.apps-0.0.1b8/rudderlabs/data/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-07-21 03:06:40.000000 rudderlabs.data.apps-0.0.1b8/rudderlabs/data/apps/
--rw-r--r--   0 runner    (1001) docker     (121)      129 2022-07-21 03:06:24.000000 rudderlabs.data.apps-0.0.1b8/rudderlabs/data/apps/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-07-21 03:06:40.000000 rudderlabs.data.apps-0.0.1b8/rudderlabs/data/apps/aws/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-07-21 03:06:24.000000 rudderlabs.data.apps-0.0.1b8/rudderlabs/data/apps/aws/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     1400 2022-07-21 03:06:24.000000 rudderlabs.data.apps-0.0.1b8/rudderlabs/data/apps/aws/processing.py
--rw-r--r--   0 runner    (1001) docker     (121)     3855 2022-07-21 03:06:24.000000 rudderlabs.data.apps-0.0.1b8/rudderlabs/data/apps/aws/s3.py
--rw-r--r--   0 runner    (1001) docker     (121)     1307 2022-07-21 03:06:24.000000 rudderlabs.data.apps-0.0.1b8/rudderlabs/data/apps/aws/session.py
--rwxr-xr-x   0 runner    (1001) docker     (121)      801 2022-07-21 03:06:24.000000 rudderlabs.data.apps-0.0.1b8/rudderlabs/data/apps/config.py
--rwxr-xr-x   0 runner    (1001) docker     (121)      747 2022-07-21 03:06:24.000000 rudderlabs.data.apps-0.0.1b8/rudderlabs/data/apps/constants.py
--rwxr-xr-x   0 runner    (1001) docker     (121)     7577 2022-07-21 03:06:24.000000 rudderlabs.data.apps-0.0.1b8/rudderlabs/data/apps/log.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-07-21 03:06:40.000000 rudderlabs.data.apps-0.0.1b8/rudderlabs/data/apps/scripts/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-07-21 03:06:24.000000 rudderlabs.data.apps-0.0.1b8/rudderlabs/data/apps/scripts/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (121)      321 2022-07-21 03:06:24.000000 rudderlabs.data.apps-0.0.1b8/rudderlabs/data/apps/scripts/aws.py
--rwxr-xr-x   0 runner    (1001) docker     (121)     3315 2022-07-21 03:06:24.000000 rudderlabs.data.apps-0.0.1b8/rudderlabs/data/apps/scripts/new.py
--rwxr-xr-x   0 runner    (1001) docker     (121)     1854 2022-07-21 03:06:24.000000 rudderlabs.data.apps-0.0.1b8/rudderlabs/data/apps/scripts/rudderlabs.py
--rw-r--r--   0 runner    (1001) docker     (121)     8325 2022-07-21 03:06:24.000000 rudderlabs.data.apps-0.0.1b8/rudderlabs/data/apps/scripts/run_pipeline.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-07-21 03:06:40.000000 rudderlabs.data.apps-0.0.1b8/rudderlabs/data/apps/templates/
--rw-r--r--   0 runner    (1001) docker     (121)       37 2022-07-21 03:06:24.000000 rudderlabs.data.apps-0.0.1b8/rudderlabs/data/apps/templates/.gitattributes
--rw-r--r--   0 runner    (1001) docker     (121)     1816 2022-07-21 03:06:24.000000 rudderlabs.data.apps-0.0.1b8/rudderlabs/data/apps/templates/.gitignore
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-07-21 03:06:24.000000 rudderlabs.data.apps-0.0.1b8/rudderlabs/data/apps/templates/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-07-21 03:06:40.000000 rudderlabs.data.apps-0.0.1b8/rudderlabs/data/apps/templates/conda/
--rw-r--r--   0 runner    (1001) docker     (121)      110 2022-07-21 03:06:24.000000 rudderlabs.data.apps-0.0.1b8/rudderlabs/data/apps/templates/conda/environment.yaml
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-07-21 03:06:40.000000 rudderlabs.data.apps-0.0.1b8/rudderlabs/data/apps/templates/config/
--rw-r--r--   0 runner    (1001) docker     (121)      660 2022-07-21 03:06:24.000000 rudderlabs.data.apps-0.0.1b8/rudderlabs/data/apps/templates/config/sample.yaml
--rw-r--r--   0 runner    (1001) docker     (121)     1271 2022-07-21 03:06:24.000000 rudderlabs.data.apps-0.0.1b8/rudderlabs/data/apps/templates/credentials_template.yaml
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-07-21 03:06:40.000000 rudderlabs.data.apps-0.0.1b8/rudderlabs/data/apps/templates/data/
--rw-r--r--   0 runner    (1001) docker     (121)       14 2022-07-21 03:06:24.000000 rudderlabs.data.apps-0.0.1b8/rudderlabs/data/apps/templates/data/.gitignore
--rw-r--r--   0 runner    (1001) docker     (121)     6809 2022-07-21 03:06:24.000000 rudderlabs.data.apps-0.0.1b8/rudderlabs/data/apps/templates/data_loader.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-07-21 03:06:40.000000 rudderlabs.data.apps-0.0.1b8/rudderlabs/data/apps/templates/notebooks/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-07-21 03:06:24.000000 rudderlabs.data.apps-0.0.1b8/rudderlabs/data/apps/templates/notebooks/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     5969 2022-07-21 03:06:24.000000 rudderlabs.data.apps-0.0.1b8/rudderlabs/data/apps/templates/notebooks/sample_notebook.ipynb
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-07-21 03:06:40.000000 rudderlabs.data.apps-0.0.1b8/rudderlabs/data/apps/templates/pipelines/
--rw-r--r--   0 runner    (1001) docker     (121)      713 2022-07-21 03:06:24.000000 rudderlabs.data.apps-0.0.1b8/rudderlabs/data/apps/templates/pipelines/sample_pipeline.yaml
--rw-r--r--   0 runner    (1001) docker     (121)       27 2022-07-21 03:06:24.000000 rudderlabs.data.apps-0.0.1b8/rudderlabs/data/apps/templates/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (121)     5628 2022-07-21 03:06:24.000000 rudderlabs.data.apps-0.0.1b8/rudderlabs/data/apps/templates/run_notebook_wrapper.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-07-21 03:06:40.000000 rudderlabs.data.apps-0.0.1b8/rudderlabs/data/apps/utils/
--rw-r--r--   0 runner    (1001) docker     (121)     1754 2022-07-21 03:06:24.000000 rudderlabs.data.apps-0.0.1b8/rudderlabs/data/apps/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     1505 2022-07-21 03:06:24.000000 rudderlabs.data.apps-0.0.1b8/rudderlabs/data/apps/utils/data.py
--rw-r--r--   0 runner    (1001) docker     (121)     1748 2022-07-21 03:06:24.000000 rudderlabs.data.apps-0.0.1b8/rudderlabs/data/apps/utils/notebook.py
--rw-r--r--   0 runner    (1001) docker     (121)     2710 2022-07-21 03:06:24.000000 rudderlabs.data.apps-0.0.1b8/rudderlabs/data/apps/utils/zip.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-07-21 03:06:40.000000 rudderlabs.data.apps-0.0.1b8/rudderlabs/data/apps/wh/
--rw-r--r--   0 runner    (1001) docker     (121)     1098 2022-07-21 03:06:24.000000 rudderlabs.data.apps-0.0.1b8/rudderlabs/data/apps/wh/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     2327 2022-07-21 03:06:24.000000 rudderlabs.data.apps-0.0.1b8/rudderlabs/data/apps/wh/connector_base.py
--rw-r--r--   0 runner    (1001) docker     (121)     1586 2022-07-21 03:06:24.000000 rudderlabs.data.apps-0.0.1b8/rudderlabs/data/apps/wh/query_utils.py
--rw-r--r--   0 runner    (1001) docker     (121)     2450 2022-07-21 03:06:24.000000 rudderlabs.data.apps-0.0.1b8/rudderlabs/data/apps/wh/redshift_connector.py
--rw-r--r--   0 runner    (1001) docker     (121)     1511 2022-07-21 03:06:24.000000 rudderlabs.data.apps-0.0.1b8/rudderlabs/data/apps/wh/snowflake_connector.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-07-21 03:06:40.000000 rudderlabs.data.apps-0.0.1b8/rudderlabs.data.apps.egg-info/
--rw-r--r--   0 runner    (1001) docker     (121)     1869 2022-07-21 03:06:40.000000 rudderlabs.data.apps-0.0.1b8/rudderlabs.data.apps.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)     2120 2022-07-21 03:06:40.000000 rudderlabs.data.apps-0.0.1b8/rudderlabs.data.apps.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2022-07-21 03:06:40.000000 rudderlabs.data.apps-0.0.1b8/rudderlabs.data.apps.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (121)      257 2022-07-21 03:06:40.000000 rudderlabs.data.apps-0.0.1b8/rudderlabs.data.apps.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2022-07-21 03:06:40.000000 rudderlabs.data.apps-0.0.1b8/rudderlabs.data.apps.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (121)      316 2022-07-21 03:06:40.000000 rudderlabs.data.apps-0.0.1b8/rudderlabs.data.apps.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (121)       11 2022-07-21 03:06:40.000000 rudderlabs.data.apps-0.0.1b8/rudderlabs.data.apps.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (121)       38 2022-07-21 03:06:40.000000 rudderlabs.data.apps-0.0.1b8/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (121)     2316 2022-07-21 03:06:24.000000 rudderlabs.data.apps-0.0.1b8/setup.py
--rw-r--r--   0 runner    (1001) docker     (121)        8 2022-07-21 03:06:24.000000 rudderlabs.data.apps-0.0.1b8/version.txt
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-07-21 03:12:59.000000 rudderlabs.data.apps-0.0.1b9/
+-rw-r--r--   0 runner    (1001) docker     (121)    35147 2022-07-21 03:12:39.000000 rudderlabs.data.apps-0.0.1b9/COPYING
+-rw-r--r--   0 runner    (1001) docker     (121)      140 2022-07-21 03:12:39.000000 rudderlabs.data.apps-0.0.1b9/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (121)     1869 2022-07-21 03:12:59.000000 rudderlabs.data.apps-0.0.1b9/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (121)     1312 2022-07-21 03:12:39.000000 rudderlabs.data.apps-0.0.1b9/README.rst
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-07-21 03:12:59.000000 rudderlabs.data.apps-0.0.1b9/docs/
+-rwxr-xr-x   0 runner    (1001) docker     (121)     1421 2022-07-21 03:12:39.000000 rudderlabs.data.apps-0.0.1b9/docs/api.rst
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-07-21 03:12:59.000000 rudderlabs.data.apps-0.0.1b9/docs/img/
+-rw-r--r--   0 runner    (1001) docker     (121)    15406 2022-07-21 03:12:39.000000 rudderlabs.data.apps-0.0.1b9/docs/img/favicon.ico
+-rw-r--r--   0 runner    (1001) docker     (121)    21769 2022-07-21 03:12:39.000000 rudderlabs.data.apps-0.0.1b9/docs/img/logo.png
+-rw-r--r--   0 runner    (1001) docker     (121)    43455 2022-07-21 03:12:39.000000 rudderlabs.data.apps-0.0.1b9/docs/img/run_pipeline_flow_diagram.png
+-rw-r--r--   0 runner    (1001) docker     (121)      479 2022-07-21 03:12:39.000000 rudderlabs.data.apps-0.0.1b9/docs/index.rst
+-rw-r--r--   0 runner    (1001) docker     (121)      908 2022-07-21 03:12:39.000000 rudderlabs.data.apps-0.0.1b9/docs/install.rst
+-rwxr-xr-x   0 runner    (1001) docker     (121)      288 2022-07-21 03:12:39.000000 rudderlabs.data.apps-0.0.1b9/docs/links.rst
+-rw-r--r--   0 runner    (1001) docker     (121)     3008 2022-07-21 03:12:39.000000 rudderlabs.data.apps-0.0.1b9/docs/new_data_app_repo.rst
+-rw-r--r--   0 runner    (1001) docker     (121)     2177 2022-07-21 03:12:39.000000 rudderlabs.data.apps-0.0.1b9/docs/sagemaker.rst
+-rwxr-xr-x   0 runner    (1001) docker     (121)      243 2022-07-21 03:12:39.000000 rudderlabs.data.apps-0.0.1b9/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (121)       47 2022-07-21 03:12:39.000000 rudderlabs.data.apps-0.0.1b9/requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-07-21 03:12:59.000000 rudderlabs.data.apps-0.0.1b9/rudderlabs/
+-rw-r--r--   0 runner    (1001) docker     (121)      129 2022-07-21 03:12:39.000000 rudderlabs.data.apps-0.0.1b9/rudderlabs/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-07-21 03:12:59.000000 rudderlabs.data.apps-0.0.1b9/rudderlabs/data/
+-rw-r--r--   0 runner    (1001) docker     (121)      129 2022-07-21 03:12:39.000000 rudderlabs.data.apps-0.0.1b9/rudderlabs/data/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-07-21 03:12:59.000000 rudderlabs.data.apps-0.0.1b9/rudderlabs/data/apps/
+-rw-r--r--   0 runner    (1001) docker     (121)      129 2022-07-21 03:12:39.000000 rudderlabs.data.apps-0.0.1b9/rudderlabs/data/apps/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-07-21 03:12:59.000000 rudderlabs.data.apps-0.0.1b9/rudderlabs/data/apps/aws/
+-rw-r--r--   0 runner    (1001) docker     (121)        0 2022-07-21 03:12:39.000000 rudderlabs.data.apps-0.0.1b9/rudderlabs/data/apps/aws/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1400 2022-07-21 03:12:39.000000 rudderlabs.data.apps-0.0.1b9/rudderlabs/data/apps/aws/processing.py
+-rw-r--r--   0 runner    (1001) docker     (121)     3855 2022-07-21 03:12:39.000000 rudderlabs.data.apps-0.0.1b9/rudderlabs/data/apps/aws/s3.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1307 2022-07-21 03:12:39.000000 rudderlabs.data.apps-0.0.1b9/rudderlabs/data/apps/aws/session.py
+-rwxr-xr-x   0 runner    (1001) docker     (121)      801 2022-07-21 03:12:39.000000 rudderlabs.data.apps-0.0.1b9/rudderlabs/data/apps/config.py
+-rwxr-xr-x   0 runner    (1001) docker     (121)      747 2022-07-21 03:12:39.000000 rudderlabs.data.apps-0.0.1b9/rudderlabs/data/apps/constants.py
+-rwxr-xr-x   0 runner    (1001) docker     (121)     7577 2022-07-21 03:12:39.000000 rudderlabs.data.apps-0.0.1b9/rudderlabs/data/apps/log.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-07-21 03:12:59.000000 rudderlabs.data.apps-0.0.1b9/rudderlabs/data/apps/scripts/
+-rw-r--r--   0 runner    (1001) docker     (121)        0 2022-07-21 03:12:39.000000 rudderlabs.data.apps-0.0.1b9/rudderlabs/data/apps/scripts/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (121)      321 2022-07-21 03:12:39.000000 rudderlabs.data.apps-0.0.1b9/rudderlabs/data/apps/scripts/aws.py
+-rwxr-xr-x   0 runner    (1001) docker     (121)     3315 2022-07-21 03:12:39.000000 rudderlabs.data.apps-0.0.1b9/rudderlabs/data/apps/scripts/new.py
+-rwxr-xr-x   0 runner    (1001) docker     (121)     1854 2022-07-21 03:12:39.000000 rudderlabs.data.apps-0.0.1b9/rudderlabs/data/apps/scripts/rudderlabs.py
+-rw-r--r--   0 runner    (1001) docker     (121)     8325 2022-07-21 03:12:39.000000 rudderlabs.data.apps-0.0.1b9/rudderlabs/data/apps/scripts/run_pipeline.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-07-21 03:12:59.000000 rudderlabs.data.apps-0.0.1b9/rudderlabs/data/apps/templates/
+-rw-r--r--   0 runner    (1001) docker     (121)       37 2022-07-21 03:12:39.000000 rudderlabs.data.apps-0.0.1b9/rudderlabs/data/apps/templates/.gitattributes
+-rw-r--r--   0 runner    (1001) docker     (121)     1816 2022-07-21 03:12:39.000000 rudderlabs.data.apps-0.0.1b9/rudderlabs/data/apps/templates/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (121)      415 2022-07-21 03:12:39.000000 rudderlabs.data.apps-0.0.1b9/rudderlabs/data/apps/templates/README.md
+-rw-r--r--   0 runner    (1001) docker     (121)        0 2022-07-21 03:12:39.000000 rudderlabs.data.apps-0.0.1b9/rudderlabs/data/apps/templates/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-07-21 03:12:59.000000 rudderlabs.data.apps-0.0.1b9/rudderlabs/data/apps/templates/conda/
+-rw-r--r--   0 runner    (1001) docker     (121)      110 2022-07-21 03:12:39.000000 rudderlabs.data.apps-0.0.1b9/rudderlabs/data/apps/templates/conda/environment.yaml
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-07-21 03:12:59.000000 rudderlabs.data.apps-0.0.1b9/rudderlabs/data/apps/templates/config/
+-rw-r--r--   0 runner    (1001) docker     (121)      660 2022-07-21 03:12:39.000000 rudderlabs.data.apps-0.0.1b9/rudderlabs/data/apps/templates/config/sample.yaml
+-rw-r--r--   0 runner    (1001) docker     (121)     1271 2022-07-21 03:12:39.000000 rudderlabs.data.apps-0.0.1b9/rudderlabs/data/apps/templates/credentials_template.yaml
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-07-21 03:12:59.000000 rudderlabs.data.apps-0.0.1b9/rudderlabs/data/apps/templates/data/
+-rw-r--r--   0 runner    (1001) docker     (121)       14 2022-07-21 03:12:39.000000 rudderlabs.data.apps-0.0.1b9/rudderlabs/data/apps/templates/data/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (121)     6809 2022-07-21 03:12:39.000000 rudderlabs.data.apps-0.0.1b9/rudderlabs/data/apps/templates/data_loader.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-07-21 03:12:59.000000 rudderlabs.data.apps-0.0.1b9/rudderlabs/data/apps/templates/notebooks/
+-rw-r--r--   0 runner    (1001) docker     (121)        0 2022-07-21 03:12:39.000000 rudderlabs.data.apps-0.0.1b9/rudderlabs/data/apps/templates/notebooks/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)     5969 2022-07-21 03:12:39.000000 rudderlabs.data.apps-0.0.1b9/rudderlabs/data/apps/templates/notebooks/sample_notebook.ipynb
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-07-21 03:12:59.000000 rudderlabs.data.apps-0.0.1b9/rudderlabs/data/apps/templates/pipelines/
+-rw-r--r--   0 runner    (1001) docker     (121)      713 2022-07-21 03:12:39.000000 rudderlabs.data.apps-0.0.1b9/rudderlabs/data/apps/templates/pipelines/sample_pipeline.yaml
+-rw-r--r--   0 runner    (1001) docker     (121)       27 2022-07-21 03:12:39.000000 rudderlabs.data.apps-0.0.1b9/rudderlabs/data/apps/templates/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (121)     5628 2022-07-21 03:12:39.000000 rudderlabs.data.apps-0.0.1b9/rudderlabs/data/apps/templates/run_notebook_wrapper.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-07-21 03:12:59.000000 rudderlabs.data.apps-0.0.1b9/rudderlabs/data/apps/utils/
+-rw-r--r--   0 runner    (1001) docker     (121)     1754 2022-07-21 03:12:39.000000 rudderlabs.data.apps-0.0.1b9/rudderlabs/data/apps/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1505 2022-07-21 03:12:39.000000 rudderlabs.data.apps-0.0.1b9/rudderlabs/data/apps/utils/data.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1748 2022-07-21 03:12:39.000000 rudderlabs.data.apps-0.0.1b9/rudderlabs/data/apps/utils/notebook.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2710 2022-07-21 03:12:39.000000 rudderlabs.data.apps-0.0.1b9/rudderlabs/data/apps/utils/zip.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-07-21 03:12:59.000000 rudderlabs.data.apps-0.0.1b9/rudderlabs/data/apps/wh/
+-rw-r--r--   0 runner    (1001) docker     (121)     1098 2022-07-21 03:12:39.000000 rudderlabs.data.apps-0.0.1b9/rudderlabs/data/apps/wh/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2327 2022-07-21 03:12:39.000000 rudderlabs.data.apps-0.0.1b9/rudderlabs/data/apps/wh/connector_base.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1586 2022-07-21 03:12:39.000000 rudderlabs.data.apps-0.0.1b9/rudderlabs/data/apps/wh/query_utils.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2450 2022-07-21 03:12:39.000000 rudderlabs.data.apps-0.0.1b9/rudderlabs/data/apps/wh/redshift_connector.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1511 2022-07-21 03:12:39.000000 rudderlabs.data.apps-0.0.1b9/rudderlabs/data/apps/wh/snowflake_connector.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-07-21 03:12:59.000000 rudderlabs.data.apps-0.0.1b9/rudderlabs.data.apps.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (121)     1869 2022-07-21 03:12:59.000000 rudderlabs.data.apps-0.0.1b9/rudderlabs.data.apps.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (121)     2161 2022-07-21 03:12:59.000000 rudderlabs.data.apps-0.0.1b9/rudderlabs.data.apps.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (121)        1 2022-07-21 03:12:59.000000 rudderlabs.data.apps-0.0.1b9/rudderlabs.data.apps.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (121)      257 2022-07-21 03:12:59.000000 rudderlabs.data.apps-0.0.1b9/rudderlabs.data.apps.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (121)        1 2022-07-21 03:12:59.000000 rudderlabs.data.apps-0.0.1b9/rudderlabs.data.apps.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (121)      316 2022-07-21 03:12:59.000000 rudderlabs.data.apps-0.0.1b9/rudderlabs.data.apps.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (121)       11 2022-07-21 03:12:59.000000 rudderlabs.data.apps-0.0.1b9/rudderlabs.data.apps.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (121)       38 2022-07-21 03:12:59.000000 rudderlabs.data.apps-0.0.1b9/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (121)     2316 2022-07-21 03:12:39.000000 rudderlabs.data.apps-0.0.1b9/setup.py
+-rw-r--r--   0 runner    (1001) docker     (121)        8 2022-07-21 03:12:39.000000 rudderlabs.data.apps-0.0.1b9/version.txt
```

### Comparing `rudderlabs.data.apps-0.0.1b8/COPYING` & `rudderlabs.data.apps-0.0.1b9/COPYING`

 * *Files identical despite different names*

### Comparing `rudderlabs.data.apps-0.0.1b8/PKG-INFO` & `rudderlabs.data.apps-0.0.1b9/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: rudderlabs.data.apps
-Version: 0.0.1b8
+Version: 0.0.1b9
 Summary: Rudderlabs data apps library
 Home-page: https://github.com/rudderlabs1/rudderlabs.data.apps
 Author: Srinivas
 Author-email: cnu.1439@gmail.com
 License: GPLv3
 Keywords: rudderlabs
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
```

### Comparing `rudderlabs.data.apps-0.0.1b8/README.rst` & `rudderlabs.data.apps-0.0.1b9/README.rst`

 * *Files identical despite different names*

### Comparing `rudderlabs.data.apps-0.0.1b8/docs/api.rst` & `rudderlabs.data.apps-0.0.1b9/docs/api.rst`

 * *Files identical despite different names*

### Comparing `rudderlabs.data.apps-0.0.1b8/docs/img/favicon.ico` & `rudderlabs.data.apps-0.0.1b9/docs/img/favicon.ico`

 * *Files identical despite different names*

### Comparing `rudderlabs.data.apps-0.0.1b8/docs/img/logo.png` & `rudderlabs.data.apps-0.0.1b9/docs/img/logo.png`

 * *Files identical despite different names*

### Comparing `rudderlabs.data.apps-0.0.1b8/docs/img/run_pipeline_flow_diagram.png` & `rudderlabs.data.apps-0.0.1b9/docs/img/run_pipeline_flow_diagram.png`

 * *Files identical despite different names*

### Comparing `rudderlabs.data.apps-0.0.1b8/docs/install.rst` & `rudderlabs.data.apps-0.0.1b9/docs/install.rst`

 * *Files identical despite different names*

### Comparing `rudderlabs.data.apps-0.0.1b8/docs/new_data_app_repo.rst` & `rudderlabs.data.apps-0.0.1b9/docs/new_data_app_repo.rst`

 * *Files identical despite different names*

### Comparing `rudderlabs.data.apps-0.0.1b8/docs/sagemaker.rst` & `rudderlabs.data.apps-0.0.1b9/docs/sagemaker.rst`

 * *Files identical despite different names*

### Comparing `rudderlabs.data.apps-0.0.1b8/rudderlabs/data/apps/aws/processing.py` & `rudderlabs.data.apps-0.0.1b9/rudderlabs/data/apps/aws/processing.py`

 * *Files identical despite different names*

### Comparing `rudderlabs.data.apps-0.0.1b8/rudderlabs/data/apps/aws/s3.py` & `rudderlabs.data.apps-0.0.1b9/rudderlabs/data/apps/aws/s3.py`

 * *Files identical despite different names*

### Comparing `rudderlabs.data.apps-0.0.1b8/rudderlabs/data/apps/aws/session.py` & `rudderlabs.data.apps-0.0.1b9/rudderlabs/data/apps/aws/session.py`

 * *Files identical despite different names*

### Comparing `rudderlabs.data.apps-0.0.1b8/rudderlabs/data/apps/config.py` & `rudderlabs.data.apps-0.0.1b9/rudderlabs/data/apps/config.py`

 * *Files identical despite different names*

### Comparing `rudderlabs.data.apps-0.0.1b8/rudderlabs/data/apps/constants.py` & `rudderlabs.data.apps-0.0.1b9/rudderlabs/data/apps/constants.py`

 * *Files identical despite different names*

### Comparing `rudderlabs.data.apps-0.0.1b8/rudderlabs/data/apps/log.py` & `rudderlabs.data.apps-0.0.1b9/rudderlabs/data/apps/log.py`

 * *Files identical despite different names*

### Comparing `rudderlabs.data.apps-0.0.1b8/rudderlabs/data/apps/scripts/new.py` & `rudderlabs.data.apps-0.0.1b9/rudderlabs/data/apps/scripts/new.py`

 * *Files identical despite different names*

### Comparing `rudderlabs.data.apps-0.0.1b8/rudderlabs/data/apps/scripts/rudderlabs.py` & `rudderlabs.data.apps-0.0.1b9/rudderlabs/data/apps/scripts/rudderlabs.py`

 * *Files identical despite different names*

### Comparing `rudderlabs.data.apps-0.0.1b8/rudderlabs/data/apps/scripts/run_pipeline.py` & `rudderlabs.data.apps-0.0.1b9/rudderlabs/data/apps/scripts/run_pipeline.py`

 * *Files identical despite different names*

### Comparing `rudderlabs.data.apps-0.0.1b8/rudderlabs/data/apps/templates/.gitignore` & `rudderlabs.data.apps-0.0.1b9/rudderlabs/data/apps/templates/.gitignore`

 * *Files identical despite different names*

### Comparing `rudderlabs.data.apps-0.0.1b8/rudderlabs/data/apps/templates/config/sample.yaml` & `rudderlabs.data.apps-0.0.1b9/rudderlabs/data/apps/templates/config/sample.yaml`

 * *Files identical despite different names*

### Comparing `rudderlabs.data.apps-0.0.1b8/rudderlabs/data/apps/templates/credentials_template.yaml` & `rudderlabs.data.apps-0.0.1b9/rudderlabs/data/apps/templates/credentials_template.yaml`

 * *Files identical despite different names*

### Comparing `rudderlabs.data.apps-0.0.1b8/rudderlabs/data/apps/templates/data_loader.py` & `rudderlabs.data.apps-0.0.1b9/rudderlabs/data/apps/templates/data_loader.py`

 * *Files identical despite different names*

### Comparing `rudderlabs.data.apps-0.0.1b8/rudderlabs/data/apps/templates/notebooks/sample_notebook.ipynb` & `rudderlabs.data.apps-0.0.1b9/rudderlabs/data/apps/templates/notebooks/sample_notebook.ipynb`

 * *Files identical despite different names*

### Comparing `rudderlabs.data.apps-0.0.1b8/rudderlabs/data/apps/templates/pipelines/sample_pipeline.yaml` & `rudderlabs.data.apps-0.0.1b9/rudderlabs/data/apps/templates/pipelines/sample_pipeline.yaml`

 * *Files identical despite different names*

### Comparing `rudderlabs.data.apps-0.0.1b8/rudderlabs/data/apps/templates/run_notebook_wrapper.py` & `rudderlabs.data.apps-0.0.1b9/rudderlabs/data/apps/templates/run_notebook_wrapper.py`

 * *Files identical despite different names*

### Comparing `rudderlabs.data.apps-0.0.1b8/rudderlabs/data/apps/utils/__init__.py` & `rudderlabs.data.apps-0.0.1b9/rudderlabs/data/apps/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `rudderlabs.data.apps-0.0.1b8/rudderlabs/data/apps/utils/data.py` & `rudderlabs.data.apps-0.0.1b9/rudderlabs/data/apps/utils/data.py`

 * *Files identical despite different names*

### Comparing `rudderlabs.data.apps-0.0.1b8/rudderlabs/data/apps/utils/notebook.py` & `rudderlabs.data.apps-0.0.1b9/rudderlabs/data/apps/utils/notebook.py`

 * *Files identical despite different names*

### Comparing `rudderlabs.data.apps-0.0.1b8/rudderlabs/data/apps/utils/zip.py` & `rudderlabs.data.apps-0.0.1b9/rudderlabs/data/apps/utils/zip.py`

 * *Files identical despite different names*

### Comparing `rudderlabs.data.apps-0.0.1b8/rudderlabs/data/apps/wh/__init__.py` & `rudderlabs.data.apps-0.0.1b9/rudderlabs/data/apps/wh/__init__.py`

 * *Files identical despite different names*

### Comparing `rudderlabs.data.apps-0.0.1b8/rudderlabs/data/apps/wh/connector_base.py` & `rudderlabs.data.apps-0.0.1b9/rudderlabs/data/apps/wh/connector_base.py`

 * *Files identical despite different names*

### Comparing `rudderlabs.data.apps-0.0.1b8/rudderlabs/data/apps/wh/query_utils.py` & `rudderlabs.data.apps-0.0.1b9/rudderlabs/data/apps/wh/query_utils.py`

 * *Files identical despite different names*

### Comparing `rudderlabs.data.apps-0.0.1b8/rudderlabs/data/apps/wh/redshift_connector.py` & `rudderlabs.data.apps-0.0.1b9/rudderlabs/data/apps/wh/redshift_connector.py`

 * *Files identical despite different names*

### Comparing `rudderlabs.data.apps-0.0.1b8/rudderlabs/data/apps/wh/snowflake_connector.py` & `rudderlabs.data.apps-0.0.1b9/rudderlabs/data/apps/wh/snowflake_connector.py`

 * *Files identical despite different names*

### Comparing `rudderlabs.data.apps-0.0.1b8/rudderlabs.data.apps.egg-info/PKG-INFO` & `rudderlabs.data.apps-0.0.1b9/rudderlabs.data.apps.egg-info/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: rudderlabs.data.apps
-Version: 0.0.1b8
+Version: 0.0.1b9
 Summary: Rudderlabs data apps library
 Home-page: https://github.com/rudderlabs1/rudderlabs.data.apps
 Author: Srinivas
 Author-email: cnu.1439@gmail.com
 License: GPLv3
 Keywords: rudderlabs
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
```

### Comparing `rudderlabs.data.apps-0.0.1b8/rudderlabs.data.apps.egg-info/SOURCES.txt` & `rudderlabs.data.apps-0.0.1b9/rudderlabs.data.apps.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -34,14 +34,15 @@
 rudderlabs/data/apps/scripts/__init__.py
 rudderlabs/data/apps/scripts/aws.py
 rudderlabs/data/apps/scripts/new.py
 rudderlabs/data/apps/scripts/rudderlabs.py
 rudderlabs/data/apps/scripts/run_pipeline.py
 rudderlabs/data/apps/templates/.gitattributes
 rudderlabs/data/apps/templates/.gitignore
+rudderlabs/data/apps/templates/README.md
 rudderlabs/data/apps/templates/__init__.py
 rudderlabs/data/apps/templates/credentials_template.yaml
 rudderlabs/data/apps/templates/data_loader.py
 rudderlabs/data/apps/templates/requirements.txt
 rudderlabs/data/apps/templates/run_notebook_wrapper.py
 rudderlabs/data/apps/templates/conda/environment.yaml
 rudderlabs/data/apps/templates/config/sample.yaml
```

### Comparing `rudderlabs.data.apps-0.0.1b8/setup.py` & `rudderlabs.data.apps-0.0.1b9/setup.py`

 * *Files identical despite different names*

