# Comparing `tmp/esg_coverage-0.2.0.tar.gz` & `tmp/esg_coverage-0.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "esg_coverage-0.2.0.tar", max compression
+gzip compressed data, was "esg_coverage-0.2.1.tar", max compression
```

## Comparing `esg_coverage-0.2.0.tar` & `esg_coverage-0.2.1.tar`

### file list

```diff
@@ -1,37 +1,49 @@
--rw-r--r--   0        0        0     1071 2023-06-23 21:03:21.257344 esg_coverage-0.2.0/LICENSE
--rw-r--r--   0        0        0     2873 2023-06-23 21:03:21.257344 esg_coverage-0.2.0/README.md
--rw-r--r--   0        0        0     2996 2023-06-23 21:03:44.650091 esg_coverage-0.2.0/pyproject.toml
--rw-r--r--   0        0        0      287 2023-06-23 21:03:21.261344 esg_coverage-0.2.0/src/esgcov/__cli__.py
--rw-r--r--   0        0        0      379 2023-06-23 21:03:21.261344 esg_coverage-0.2.0/src/esgcov/__init__.py
--rw-r--r--   0        0        0       22 2023-06-23 21:03:44.598091 esg_coverage-0.2.0/src/esgcov/_version.py
--rw-r--r--   0        0        0        0 2023-06-23 21:03:21.261344 esg_coverage-0.2.0/src/esgcov/conf/__init__.py
--rw-r--r--   0        0        0      288 2023-06-23 21:03:44.598091 esg_coverage-0.2.0/src/esgcov/conf/about/__init__.yaml
--rw-r--r--   0        0        0      435 2023-06-23 21:03:21.261344 esg_coverage-0.2.0/src/esgcov/conf/batch/__init__.yaml
--rw-r--r--   0        0        0       49 2023-06-23 21:03:21.261344 esg_coverage-0.2.0/src/esgcov/conf/cmd/about.yaml
--rw-r--r--   0        0        0      141 2023-06-23 21:03:21.261344 esg_coverage-0.2.0/src/esgcov/conf/cmd/copy_conf.yaml
--rw-r--r--   0        0        0      167 2023-06-23 21:03:21.261344 esg_coverage-0.2.0/src/esgcov/conf/cmd/cpcfg.yaml
--rw-r--r--   0        0        0       83 2023-06-23 21:03:21.261344 esg_coverage-0.2.0/src/esgcov/conf/cmd/run_task.yaml
--rw-r--r--   0        0        0      320 2023-06-23 21:03:21.261344 esg_coverage-0.2.0/src/esgcov/conf/config.yaml
--rw-r--r--   0        0        0      559 2023-06-23 21:03:21.261344 esg_coverage-0.2.0/src/esgcov/conf/copier/conf.yaml
--rw-r--r--   0        0        0      725 2023-06-23 21:03:21.261344 esg_coverage-0.2.0/src/esgcov/conf/dotenv/__init__.yaml
--rw-r--r--   0        0        0      319 2023-06-23 21:03:21.261344 esg_coverage-0.2.0/src/esgcov/conf/hconf.yaml
--rw-r--r--   0        0        0     1128 2023-06-23 21:03:21.261344 esg_coverage-0.2.0/src/esgcov/conf/hydra/help/help.yaml
--rw-r--r--   0        0        0      264 2023-06-23 21:03:21.261344 esg_coverage-0.2.0/src/esgcov/conf/hydra/job_logging/custom.yaml
--rw-r--r--   0        0        0      291 2023-06-23 21:03:21.261344 esg_coverage-0.2.0/src/esgcov/conf/joblib/__init__.yaml
--rw-r--r--   0        0        0      217 2023-06-23 21:03:21.261344 esg_coverage-0.2.0/src/esgcov/conf/mode/__debug__.yaml
--rw-r--r--   0        0        0      921 2023-06-23 21:03:21.261344 esg_coverage-0.2.0/src/esgcov/conf/mode/__init__.yaml
--rw-r--r--   0        0        0      231 2023-06-23 21:03:21.261344 esg_coverage-0.2.0/src/esgcov/conf/mode/debug.yaml
--rw-r--r--   0        0        0       61 2023-06-23 21:03:21.261344 esg_coverage-0.2.0/src/esgcov/conf/module/__init__.yaml
--rw-r--r--   0        0        0       96 2023-06-23 21:03:21.261344 esg_coverage-0.2.0/src/esgcov/conf/path/__batch__.yaml
--rw-r--r--   0        0        0      582 2023-06-23 21:03:21.261344 esg_coverage-0.2.0/src/esgcov/conf/path/__default__.yaml
--rw-r--r--   0        0        0     1719 2023-06-23 21:03:21.261344 esg_coverage-0.2.0/src/esgcov/conf/path/__init__.yaml
--rw-r--r--   0        0        0      396 2023-06-23 21:03:21.261344 esg_coverage-0.2.0/src/esgcov/conf/path/__task__.yaml
--rw-r--r--   0        0        0       85 2023-06-23 21:03:21.261344 esg_coverage-0.2.0/src/esgcov/conf/pipe/__external__.yaml
--rw-r--r--   0        0        0      113 2023-06-23 21:03:21.261344 esg_coverage-0.2.0/src/esgcov/conf/pipe/__init__.yaml
--rw-r--r--   0        0        0       51 2023-06-23 21:03:21.261344 esg_coverage-0.2.0/src/esgcov/conf/pipe/__instance__.yaml
--rw-r--r--   0        0        0       49 2023-06-23 21:03:21.261344 esg_coverage-0.2.0/src/esgcov/conf/pipe/__lambda__.yaml
--rw-r--r--   0        0        0      806 2023-06-23 21:03:21.261344 esg_coverage-0.2.0/src/esgcov/conf/project/__init__.yaml
--rw-r--r--   0        0        0      153 2023-06-23 21:03:21.261344 esg_coverage-0.2.0/src/esgcov/conf/task/__batch__.yaml
--rw-r--r--   0        0        0      195 2023-06-23 21:03:21.261344 esg_coverage-0.2.0/src/esgcov/conf/task/__init__.yaml
--rw-r--r--   0        0        0        0 2023-06-23 21:03:21.261344 esg_coverage-0.2.0/src/esgcov/py.typed
--rw-r--r--   0        0        0     3612 1970-01-01 00:00:00.000000 esg_coverage-0.2.0/PKG-INFO
+-rw-r--r--   0        0        0     1071 2023-06-26 18:49:16.807337 esg_coverage-0.2.1/LICENSE
+-rw-r--r--   0        0        0     2873 2023-06-26 18:49:16.807337 esg_coverage-0.2.1/README.md
+-rw-r--r--   0        0        0     2996 2023-06-26 18:49:41.415559 esg_coverage-0.2.1/pyproject.toml
+-rw-r--r--   0        0        0      287 2023-06-26 18:49:16.811337 esg_coverage-0.2.1/src/esgcov/__cli__.py
+-rw-r--r--   0        0        0      379 2023-06-26 18:49:16.811337 esg_coverage-0.2.1/src/esgcov/__init__.py
+-rw-r--r--   0        0        0       22 2023-06-26 18:49:41.359558 esg_coverage-0.2.1/src/esgcov/_version.py
+-rw-r--r--   0        0        0        0 2023-06-26 18:49:16.811337 esg_coverage-0.2.1/src/esgcov/conf/__init__.py
+-rw-r--r--   0        0        0      288 2023-06-26 18:49:41.359558 esg_coverage-0.2.1/src/esgcov/conf/about/__init__.yaml
+-rw-r--r--   0        0        0      435 2023-06-26 18:49:16.811337 esg_coverage-0.2.1/src/esgcov/conf/batch/__init__.yaml
+-rw-r--r--   0        0        0        0 2023-06-26 18:49:16.811337 esg_coverage-0.2.1/src/esgcov/conf/cmd/__init__.yaml
+-rw-r--r--   0        0        0       49 2023-06-26 18:49:16.811337 esg_coverage-0.2.1/src/esgcov/conf/cmd/about.yaml
+-rw-r--r--   0        0        0      155 2023-06-26 18:49:16.811337 esg_coverage-0.2.1/src/esgcov/conf/cmd/copy_conf.yaml
+-rw-r--r--   0        0        0      167 2023-06-26 18:49:16.811337 esg_coverage-0.2.1/src/esgcov/conf/cmd/cpcfg.yaml
+-rw-r--r--   0        0        0       83 2023-06-26 18:49:16.811337 esg_coverage-0.2.1/src/esgcov/conf/cmd/run_task.yaml
+-rw-r--r--   0        0        0      320 2023-06-26 18:49:16.811337 esg_coverage-0.2.1/src/esgcov/conf/config.yaml
+-rw-r--r--   0        0        0      569 2023-06-26 18:49:16.811337 esg_coverage-0.2.1/src/esgcov/conf/copier/conf.yaml
+-rw-r--r--   0        0        0      709 2023-06-26 18:49:16.811337 esg_coverage-0.2.1/src/esgcov/conf/dotenv/__init__.yaml
+-rw-r--r--   0        0        0      319 2023-06-26 18:49:16.811337 esg_coverage-0.2.1/src/esgcov/conf/hconf.yaml
+-rw-r--r--   0        0        0     1128 2023-06-26 18:49:16.811337 esg_coverage-0.2.1/src/esgcov/conf/hydra/help/help.yaml
+-rw-r--r--   0        0        0      264 2023-06-26 18:49:16.811337 esg_coverage-0.2.1/src/esgcov/conf/hydra/job_logging/custom.yaml
+-rw-r--r--   0        0        0      291 2023-06-26 18:49:16.811337 esg_coverage-0.2.1/src/esgcov/conf/joblib/__init__.yaml
+-rw-r--r--   0        0        0      217 2023-06-26 18:49:16.811337 esg_coverage-0.2.1/src/esgcov/conf/mode/__debug__.yaml
+-rw-r--r--   0        0        0      921 2023-06-26 18:49:16.811337 esg_coverage-0.2.1/src/esgcov/conf/mode/__init__.yaml
+-rw-r--r--   0        0        0      231 2023-06-26 18:49:16.811337 esg_coverage-0.2.1/src/esgcov/conf/mode/debug.yaml
+-rw-r--r--   0        0        0       61 2023-06-26 18:49:16.811337 esg_coverage-0.2.1/src/esgcov/conf/module/__init__.yaml
+-rw-r--r--   0        0        0       96 2023-06-26 18:49:16.811337 esg_coverage-0.2.1/src/esgcov/conf/path/__batch__.yaml
+-rw-r--r--   0        0        0      582 2023-06-26 18:49:16.811337 esg_coverage-0.2.1/src/esgcov/conf/path/__default__.yaml
+-rw-r--r--   0        0        0     1719 2023-06-26 18:49:16.811337 esg_coverage-0.2.1/src/esgcov/conf/path/__init__.yaml
+-rw-r--r--   0        0        0      412 2023-06-26 18:49:16.811337 esg_coverage-0.2.1/src/esgcov/conf/path/__task__.yaml
+-rw-r--r--   0        0        0       76 2023-06-26 18:49:16.811337 esg_coverage-0.2.1/src/esgcov/conf/pipe/__dataframe__.yaml
+-rw-r--r--   0        0        0       72 2023-06-26 18:49:16.811337 esg_coverage-0.2.1/src/esgcov/conf/pipe/__dataframe_external_funcs__.yaml
+-rw-r--r--   0        0        0       74 2023-06-26 18:49:16.811337 esg_coverage-0.2.1/src/esgcov/conf/pipe/__dataframe_instance_methods__.yaml
+-rw-r--r--   0        0        0       85 2023-06-26 18:49:16.811337 esg_coverage-0.2.1/src/esgcov/conf/pipe/__external__.yaml
+-rw-r--r--   0        0        0       77 2023-06-26 18:49:16.811337 esg_coverage-0.2.1/src/esgcov/conf/pipe/__init__.yaml
+-rw-r--r--   0        0        0       51 2023-06-26 18:49:16.811337 esg_coverage-0.2.1/src/esgcov/conf/pipe/__instance__.yaml
+-rw-r--r--   0        0        0       49 2023-06-26 18:49:16.811337 esg_coverage-0.2.1/src/esgcov/conf/pipe/__lambda__.yaml
+-rw-r--r--   0        0        0      217 2023-06-26 18:49:16.811337 esg_coverage-0.2.1/src/esgcov/conf/pipe/load_dataframes.yaml
+-rw-r--r--   0        0        0      220 2023-06-26 18:49:16.811337 esg_coverage-0.2.1/src/esgcov/conf/pipe/save_dataframes.yaml
+-rw-r--r--   0        0        0       92 2023-06-26 18:49:16.811337 esg_coverage-0.2.1/src/esgcov/conf/pipe/test_preprocessing.yaml
+-rw-r--r--   0        0        0       19 2023-06-26 18:49:16.811337 esg_coverage-0.2.1/src/esgcov/conf/pipeline/__init__.yaml
+-rw-r--r--   0        0        0      388 2023-06-26 18:49:16.811337 esg_coverage-0.2.1/src/esgcov/conf/pipeline/__test__.yaml
+-rw-r--r--   0        0        0      720 2023-06-26 18:49:16.811337 esg_coverage-0.2.1/src/esgcov/conf/project/__init__.yaml
+-rw-r--r--   0        0        0       36 2023-06-26 18:49:16.811337 esg_coverage-0.2.1/src/esgcov/conf/running/__init__.yaml
+-rw-r--r--   0        0        0      176 2023-06-26 18:49:16.811337 esg_coverage-0.2.1/src/esgcov/conf/task/__batch__.yaml
+-rw-r--r--   0        0        0      319 2023-06-26 18:49:16.811337 esg_coverage-0.2.1/src/esgcov/conf/task/__init__.yaml
+-rw-r--r--   0        0        0      311 2023-06-26 18:49:16.811337 esg_coverage-0.2.1/src/esgcov/conf/task/__test__.yaml
+-rw-r--r--   0        0        0       59 2023-06-26 18:49:16.811337 esg_coverage-0.2.1/src/esgcov/conf/workflow/__init__.yaml
+-rw-r--r--   0        0        0        0 2023-06-26 18:49:16.811337 esg_coverage-0.2.1/src/esgcov/py.typed
+-rw-r--r--   0        0        0     3612 1970-01-01 00:00:00.000000 esg_coverage-0.2.1/PKG-INFO
```

### Comparing `esg_coverage-0.2.0/LICENSE` & `esg_coverage-0.2.1/LICENSE`

 * *Files identical despite different names*

### Comparing `esg_coverage-0.2.0/README.md` & `esg_coverage-0.2.1/README.md`

 * *Files identical despite different names*

### Comparing `esg_coverage-0.2.0/pyproject.toml` & `esg_coverage-0.2.1/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,24 +1,24 @@
 [tool.poetry]
 name = "esg-coverage"
-version = "0.2.0"
+version = "0.2.1"
 description = "The Role of Analyst Coverage in Translating ESG Ratings into Stock Performance"
 authors = ["Young Joon Lee <entelecheia@hotmail.com>"]
 license = "MIT"
 homepage = "https://esg-coverage.entelecheia.ai"
 repository = "https://github.com/entelecheia/esg-coverage"
 readme = "README.md"
 packages = [{ include = "esgcov", from = "src" }]
 
 [tool.poetry.scripts]
 esgcov = 'esgcov.__cli__:main'
 
 [tool.poetry.dependencies]
 python = ">=3.8.1,<3.12"
-hyfi = "^0.12.2"
+hyfi = "^0.14.1"
 tabulate = "^0.9.0"
 
 [tool.poetry.group.dev]
 optional = true
 
 [tool.poetry.group.dev.dependencies]
 python-semantic-release = "^7.33.1"
```

### Comparing `esg_coverage-0.2.0/src/esgcov/conf/copier/conf.yaml` & `esg_coverage-0.2.1/src/esgcov/conf/copier/conf.yaml`

 * *Files 4% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 # Source path where to find the template.
 src_path: conf
 # Destination path where to render the template.
-dst_path: tmp/conf
+dst_path: workspace/tmp/conf
 # Filetypes to copy.
 filetypes:
   - yaml
   - yml
   - py
 # User-chosen additional file exclusion patterns.
 exclude:
```

### Comparing `esg_coverage-0.2.0/src/esgcov/conf/dotenv/__init__.yaml` & `esg_coverage-0.2.1/src/esgcov/conf/dotenv/__init__.yaml`

 * *Files 18% similar despite different names*

```diff
@@ -2,15 +2,14 @@
 DOTENV_DIR: ${oc.select:..path.runtime,.}
 DOTENV_PATH: ${.DOTENV_DIR}/${.DOTENV_FILENAME}
 # Internal
 HYFI_RESOURCE_DIR:
 HYFI_GLOBAL_ROOT:
 HYFI_GLOBAL_WORKSPACE_NAME:
 HYFI_PROJECT_NAME:
-HYFI_TASK_NAME:
 HYFI_PROJECT_DESC:
 HYFI_PROJECT_ROOT:
 HYFI_PROJECT_WORKSPACE_NAME:
 HYFI_LOG_LEVEL: WARNING
 HYFI_VERBOSE: false
 HYFI_NUM_WORKERS:
 CACHED_PATH_CACHE_ROOT:
```

### Comparing `esg_coverage-0.2.0/src/esgcov/conf/hydra/help/help.yaml` & `esg_coverage-0.2.1/src/esgcov/conf/hydra/help/help.yaml`

 * *Files identical despite different names*

### Comparing `esg_coverage-0.2.0/src/esgcov/conf/mode/__init__.yaml` & `esg_coverage-0.2.1/src/esgcov/conf/mode/__init__.yaml`

 * *Files identical despite different names*

### Comparing `esg_coverage-0.2.0/src/esgcov/conf/path/__default__.yaml` & `esg_coverage-0.2.1/src/esgcov/conf/path/__default__.yaml`

 * *Files identical despite different names*

### Comparing `esg_coverage-0.2.0/src/esgcov/conf/path/__init__.yaml` & `esg_coverage-0.2.1/src/esgcov/conf/path/__init__.yaml`

 * *Files identical despite different names*

### Comparing `esg_coverage-0.2.0/src/esgcov/conf/project/__init__.yaml` & `esg_coverage-0.2.1/src/esgcov/conf/project/__init__.yaml`

 * *Files 20% similar despite different names*

```diff
@@ -1,14 +1,13 @@
 defaults:
   - /dotenv: __init__
   - /joblib: __init__
   - /path: __init__
 
 project_name: ${alt:${oc.env:HYFI_PROJECT_NAME,null},hyfi-project}
-task_name: ${oc.select:..task_name,${alt:${oc.env:HYFI_TASK_NAME,null},default-task}}
 project_description: ${oc.env:HYFI_PROJECT_DESC,""}
 project_root: ${alt:${oc.env:HYFI_PROJECT_ROOT,null},${.global_hyfi_root}/${.global_workspace_name}/projects/${.project_name}}
 project_workspace_name: ${alt:${oc.env:HYFI_PROJECT_WORKSPACE_NAME,null},${.global_workspace_name}}
 global_hyfi_root: ${alt:${oc.env:HYFI_GLOBAL_ROOT,null},${__home_path__:}/.hyfi}
 global_workspace_name: ${alt:${oc.env:HYFI_GLOBAL_WORKSPACE_NAME,null},workspace}
 num_workers: ${oc.env:HYFI_NUM_WORKERS,1}
 use_huggingface_hub: false
```

### Comparing `esg_coverage-0.2.0/PKG-INFO` & `esg_coverage-0.2.1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,22 +1,22 @@
 Metadata-Version: 2.1
 Name: esg-coverage
-Version: 0.2.0
+Version: 0.2.1
 Summary: The Role of Analyst Coverage in Translating ESG Ratings into Stock Performance
 Home-page: https://esg-coverage.entelecheia.ai
 License: MIT
 Author: Young Joon Lee
 Author-email: entelecheia@hotmail.com
 Requires-Python: >=3.8.1,<3.12
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
-Requires-Dist: hyfi (>=0.12.2,<0.13.0)
+Requires-Dist: hyfi (>=0.14.1,<0.15.0)
 Requires-Dist: tabulate (>=0.9.0,<0.10.0)
 Project-URL: Repository, https://github.com/entelecheia/esg-coverage
 Description-Content-Type: text/markdown
 
 # The Analyst Pathway in ESG
 
 [![pypi-image]][pypi-url]
```

