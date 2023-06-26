# Comparing `tmp/jobbergate_api-3.5.0a5.tar.gz` & `tmp/jobbergate_api-3.5.0a6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "jobbergate_api-3.5.0a5.tar", max compression
+gzip compressed data, was "jobbergate_api-3.5.0a6.tar", max compression
```

## Comparing `jobbergate_api-3.5.0a5.tar` & `jobbergate_api-3.5.0a6.tar`

### file list

```diff
@@ -1,61 +1,61 @@
--rw-r--r--   0        0        0     1082 2023-06-22 17:40:37.483250 jobbergate_api-3.5.0a5/LICENSE
--rw-r--r--   0        0        0      738 2023-06-22 17:40:37.483250 jobbergate_api-3.5.0a5/README.rst
--rw-r--r--   0        0        0      169 2023-06-22 17:40:37.483250 jobbergate_api-3.5.0a5/jobbergate_api/__init__.py
--rw-r--r--   0        0        0       30 2023-06-22 17:40:37.483250 jobbergate_api-3.5.0a5/jobbergate_api/apps/__init__.py
--rw-r--r--   0        0        0       41 2023-06-22 17:40:37.483250 jobbergate_api-3.5.0a5/jobbergate_api/apps/applications/__init__.py
--rw-r--r--   0        0        0     5655 2023-06-22 17:40:37.483250 jobbergate_api-3.5.0a5/jobbergate_api/apps/applications/application_files.py
--rw-r--r--   0        0        0      234 2023-06-22 17:40:37.483250 jobbergate_api-3.5.0a5/jobbergate_api/apps/applications/constants.py
--rw-r--r--   0        0        0     9408 2023-06-22 17:40:37.483250 jobbergate_api-3.5.0a5/jobbergate_api/apps/applications/file_validation.py
--rw-r--r--   0        0        0     1474 2023-06-22 17:40:37.483250 jobbergate_api-3.5.0a5/jobbergate_api/apps/applications/models.py
--rw-r--r--   0        0        0    14123 2023-06-22 17:40:37.483250 jobbergate_api-3.5.0a5/jobbergate_api/apps/applications/routers.py
--rw-r--r--   0        0        0     7421 2023-06-22 17:40:37.483250 jobbergate_api-3.5.0a5/jobbergate_api/apps/applications/schemas.py
--rw-r--r--   0        0        0       40 2023-06-22 17:40:37.483250 jobbergate_api-3.5.0a5/jobbergate_api/apps/job_scripts/__init__.py
--rw-r--r--   0        0        0    12639 2023-06-22 17:40:37.487250 jobbergate_api-3.5.0a5/jobbergate_api/apps/job_scripts/job_script_files.py
--rw-r--r--   0        0        0     1287 2023-06-22 17:40:37.487250 jobbergate_api-3.5.0a5/jobbergate_api/apps/job_scripts/models.py
--rw-r--r--   0        0        0    17426 2023-06-22 17:40:37.487250 jobbergate_api-3.5.0a5/jobbergate_api/apps/job_scripts/routers.py
--rw-r--r--   0        0        0     3800 2023-06-22 17:40:37.487250 jobbergate_api-3.5.0a5/jobbergate_api/apps/job_scripts/schemas.py
--rw-r--r--   0        0        0       44 2023-06-22 17:40:37.487250 jobbergate_api-3.5.0a5/jobbergate_api/apps/job_submissions/__init__.py
--rw-r--r--   0        0        0      529 2023-06-22 17:40:37.487250 jobbergate_api-3.5.0a5/jobbergate_api/apps/job_submissions/constants.py
--rw-r--r--   0        0        0     1909 2023-06-22 17:40:37.487250 jobbergate_api-3.5.0a5/jobbergate_api/apps/job_submissions/models.py
--rw-r--r--   0        0        0    12331 2023-06-22 17:40:37.487250 jobbergate_api-3.5.0a5/jobbergate_api/apps/job_submissions/properties_parser.py
--rw-r--r--   0        0        0    18431 2023-06-22 17:40:37.487250 jobbergate_api-3.5.0a5/jobbergate_api/apps/job_submissions/routers.py
--rw-r--r--   0        0        0    15946 2023-06-22 17:40:37.487250 jobbergate_api-3.5.0a5/jobbergate_api/apps/job_submissions/schemas.py
--rw-r--r--   0        0        0      554 2023-06-22 17:40:37.487250 jobbergate_api-3.5.0a5/jobbergate_api/apps/permissions.py
--rw-r--r--   0        0        0     3621 2023-06-22 17:40:37.487250 jobbergate_api-3.5.0a5/jobbergate_api/config.py
--rw-r--r--   0        0        0     2466 2023-06-22 17:40:37.487250 jobbergate_api-3.5.0a5/jobbergate_api/email_notification.py
--rw-r--r--   0        0        0     3268 2023-06-22 17:40:37.487250 jobbergate_api-3.5.0a5/jobbergate_api/main.py
--rw-r--r--   0        0        0     3433 2023-06-22 17:40:37.487250 jobbergate_api-3.5.0a5/jobbergate_api/meta_mapper.py
--rw-r--r--   0        0        0       96 2023-06-22 17:40:37.487250 jobbergate_api-3.5.0a5/jobbergate_api/metadata.py
--rw-r--r--   0        0        0     3470 2023-06-22 17:40:37.487250 jobbergate_api-3.5.0a5/jobbergate_api/pagination.py
--rw-r--r--   0        0        0     2284 2023-06-22 17:40:37.487250 jobbergate_api-3.5.0a5/jobbergate_api/s3_manager.py
--rw-r--r--   0        0        0     2166 2023-06-22 17:40:37.487250 jobbergate_api-3.5.0a5/jobbergate_api/security.py
--rw-r--r--   0        0        0     5580 2023-06-22 17:40:37.487250 jobbergate_api-3.5.0a5/jobbergate_api/storage.py
--rw-r--r--   0        0        0       40 2023-06-22 17:40:37.487250 jobbergate_api-3.5.0a5/jobbergate_api/tests/__init__.py
--rw-r--r--   0        0        0       28 2023-06-22 17:40:37.487250 jobbergate_api-3.5.0a5/jobbergate_api/tests/apps/__init__.py
--rw-r--r--   0        0        0       44 2023-06-22 17:40:37.487250 jobbergate_api-3.5.0a5/jobbergate_api/tests/apps/applications/__init__.py
--rw-r--r--   0        0        0    10634 2023-06-22 17:40:37.487250 jobbergate_api-3.5.0a5/jobbergate_api/tests/apps/applications/test_application_files.py
--rw-r--r--   0        0        0     1967 2023-06-22 17:40:37.487250 jobbergate_api-3.5.0a5/jobbergate_api/tests/apps/applications/test_file_validation.py
--rw-r--r--   0        0        0    44032 2023-06-22 17:40:37.487250 jobbergate_api-3.5.0a5/jobbergate_api/tests/apps/applications/test_routers.py
--rw-r--r--   0        0        0     5180 2023-06-22 17:40:37.487250 jobbergate_api-3.5.0a5/jobbergate_api/tests/apps/applications/test_schemas.py
--rw-r--r--   0        0        0     2756 2023-06-22 17:40:37.487250 jobbergate_api-3.5.0a5/jobbergate_api/tests/apps/conftest.py
--rw-r--r--   0        0        0       42 2023-06-22 17:40:37.487250 jobbergate_api-3.5.0a5/jobbergate_api/tests/apps/job_scripts/__init__.py
--rw-r--r--   0        0        0     1376 2023-06-22 17:40:37.487250 jobbergate_api-3.5.0a5/jobbergate_api/tests/apps/job_scripts/conftest.py
--rw-r--r--   0        0        0    11518 2023-06-22 17:40:37.487250 jobbergate_api-3.5.0a5/jobbergate_api/tests/apps/job_scripts/test_job_script_files.py
--rw-r--r--   0        0        0    53958 2023-06-22 17:40:37.487250 jobbergate_api-3.5.0a5/jobbergate_api/tests/apps/job_scripts/test_routers.py
--rw-r--r--   0        0        0       46 2023-06-22 17:40:37.487250 jobbergate_api-3.5.0a5/jobbergate_api/tests/apps/job_submissions/__init__.py
--rw-r--r--   0        0        0    24706 2023-06-22 17:40:37.487250 jobbergate_api-3.5.0a5/jobbergate_api/tests/apps/job_submissions/test_properties_parser.py
--rw-r--r--   0        0        0    78149 2023-06-22 17:40:37.487250 jobbergate_api-3.5.0a5/jobbergate_api/tests/apps/job_submissions/test_routers.py
--rw-r--r--   0        0        0      511 2023-06-22 17:40:37.487250 jobbergate_api-3.5.0a5/jobbergate_api/tests/apps/test_main.py
--rw-r--r--   0        0        0     8900 2023-06-22 17:40:37.487250 jobbergate_api-3.5.0a5/jobbergate_api/tests/conftest.py
--rw-r--r--   0        0        0     4503 2023-06-22 17:40:37.487250 jobbergate_api-3.5.0a5/jobbergate_api/tests/integration/draft_test_jobbergate_slurm_job_properties.py
--rw-r--r--   0        0        0     3215 2023-06-22 17:40:37.487250 jobbergate_api-3.5.0a5/jobbergate_api/tests/test_config.py
--rw-r--r--   0        0        0     4974 2023-06-22 17:40:37.487250 jobbergate_api-3.5.0a5/jobbergate_api/tests/test_email_notification.py
--rw-r--r--   0        0        0     3177 2023-06-22 17:40:37.487250 jobbergate_api-3.5.0a5/jobbergate_api/tests/test_meta_mapper.py
--rw-r--r--   0        0        0     3959 2023-06-22 17:40:37.487250 jobbergate_api-3.5.0a5/jobbergate_api/tests/test_pagination.py
--rw-r--r--   0        0        0     1146 2023-06-22 17:40:37.487250 jobbergate_api-3.5.0a5/jobbergate_api/tests/test_s3_manager.py
--rw-r--r--   0        0        0     2718 2023-06-22 17:40:37.487250 jobbergate_api-3.5.0a5/jobbergate_api/tests/test_security.py
--rw-r--r--   0        0        0     4512 2023-06-22 17:40:37.487250 jobbergate_api-3.5.0a5/jobbergate_api/tests/test_storage.py
--rw-r--r--   0        0        0     2777 2023-06-22 17:40:37.487250 jobbergate_api-3.5.0a5/jobbergate_api/tests/test_version.py
--rw-r--r--   0        0        0     1102 2023-06-22 17:40:37.487250 jobbergate_api-3.5.0a5/jobbergate_api/version.py
--rw-r--r--   0        0        0     2898 2023-06-22 17:40:37.487250 jobbergate_api-3.5.0a5/pyproject.toml
--rw-r--r--   0        0        0     2756 1970-01-01 00:00:00.000000 jobbergate_api-3.5.0a5/PKG-INFO
+-rw-r--r--   0        0        0     1082 2023-06-26 17:06:40.203826 jobbergate_api-3.5.0a6/LICENSE
+-rw-r--r--   0        0        0      738 2023-06-26 17:06:40.203826 jobbergate_api-3.5.0a6/README.rst
+-rw-r--r--   0        0        0      169 2023-06-26 17:06:40.203826 jobbergate_api-3.5.0a6/jobbergate_api/__init__.py
+-rw-r--r--   0        0        0       30 2023-06-26 17:06:40.203826 jobbergate_api-3.5.0a6/jobbergate_api/apps/__init__.py
+-rw-r--r--   0        0        0       41 2023-06-26 17:06:40.203826 jobbergate_api-3.5.0a6/jobbergate_api/apps/applications/__init__.py
+-rw-r--r--   0        0        0     5655 2023-06-26 17:06:40.203826 jobbergate_api-3.5.0a6/jobbergate_api/apps/applications/application_files.py
+-rw-r--r--   0        0        0      234 2023-06-26 17:06:40.203826 jobbergate_api-3.5.0a6/jobbergate_api/apps/applications/constants.py
+-rw-r--r--   0        0        0     9408 2023-06-26 17:06:40.203826 jobbergate_api-3.5.0a6/jobbergate_api/apps/applications/file_validation.py
+-rw-r--r--   0        0        0     1474 2023-06-26 17:06:40.203826 jobbergate_api-3.5.0a6/jobbergate_api/apps/applications/models.py
+-rw-r--r--   0        0        0    15910 2023-06-26 17:06:40.203826 jobbergate_api-3.5.0a6/jobbergate_api/apps/applications/routers.py
+-rw-r--r--   0        0        0     7421 2023-06-26 17:06:40.203826 jobbergate_api-3.5.0a6/jobbergate_api/apps/applications/schemas.py
+-rw-r--r--   0        0        0       40 2023-06-26 17:06:40.207826 jobbergate_api-3.5.0a6/jobbergate_api/apps/job_scripts/__init__.py
+-rw-r--r--   0        0        0    12639 2023-06-26 17:06:40.207826 jobbergate_api-3.5.0a6/jobbergate_api/apps/job_scripts/job_script_files.py
+-rw-r--r--   0        0        0     1287 2023-06-26 17:06:40.207826 jobbergate_api-3.5.0a6/jobbergate_api/apps/job_scripts/models.py
+-rw-r--r--   0        0        0    17785 2023-06-26 17:06:40.207826 jobbergate_api-3.5.0a6/jobbergate_api/apps/job_scripts/routers.py
+-rw-r--r--   0        0        0     3800 2023-06-26 17:06:40.207826 jobbergate_api-3.5.0a6/jobbergate_api/apps/job_scripts/schemas.py
+-rw-r--r--   0        0        0       44 2023-06-26 17:06:40.207826 jobbergate_api-3.5.0a6/jobbergate_api/apps/job_submissions/__init__.py
+-rw-r--r--   0        0        0      529 2023-06-26 17:06:40.207826 jobbergate_api-3.5.0a6/jobbergate_api/apps/job_submissions/constants.py
+-rw-r--r--   0        0        0     1909 2023-06-26 17:06:40.207826 jobbergate_api-3.5.0a6/jobbergate_api/apps/job_submissions/models.py
+-rw-r--r--   0        0        0    12331 2023-06-26 17:06:40.207826 jobbergate_api-3.5.0a6/jobbergate_api/apps/job_submissions/properties_parser.py
+-rw-r--r--   0        0        0    19227 2023-06-26 17:06:40.207826 jobbergate_api-3.5.0a6/jobbergate_api/apps/job_submissions/routers.py
+-rw-r--r--   0        0        0    15946 2023-06-26 17:06:40.207826 jobbergate_api-3.5.0a6/jobbergate_api/apps/job_submissions/schemas.py
+-rw-r--r--   0        0        0     1313 2023-06-26 17:06:40.207826 jobbergate_api-3.5.0a6/jobbergate_api/apps/permissions.py
+-rw-r--r--   0        0        0     3621 2023-06-26 17:06:40.207826 jobbergate_api-3.5.0a6/jobbergate_api/config.py
+-rw-r--r--   0        0        0     2466 2023-06-26 17:06:40.207826 jobbergate_api-3.5.0a6/jobbergate_api/email_notification.py
+-rw-r--r--   0        0        0     3268 2023-06-26 17:06:40.207826 jobbergate_api-3.5.0a6/jobbergate_api/main.py
+-rw-r--r--   0        0        0     3433 2023-06-26 17:06:40.207826 jobbergate_api-3.5.0a6/jobbergate_api/meta_mapper.py
+-rw-r--r--   0        0        0       96 2023-06-26 17:06:40.207826 jobbergate_api-3.5.0a6/jobbergate_api/metadata.py
+-rw-r--r--   0        0        0     3470 2023-06-26 17:06:40.207826 jobbergate_api-3.5.0a6/jobbergate_api/pagination.py
+-rw-r--r--   0        0        0     2284 2023-06-26 17:06:40.207826 jobbergate_api-3.5.0a6/jobbergate_api/s3_manager.py
+-rw-r--r--   0        0        0     2166 2023-06-26 17:06:40.207826 jobbergate_api-3.5.0a6/jobbergate_api/security.py
+-rw-r--r--   0        0        0     5580 2023-06-26 17:06:40.207826 jobbergate_api-3.5.0a6/jobbergate_api/storage.py
+-rw-r--r--   0        0        0       40 2023-06-26 17:06:40.207826 jobbergate_api-3.5.0a6/jobbergate_api/tests/__init__.py
+-rw-r--r--   0        0        0       28 2023-06-26 17:06:40.207826 jobbergate_api-3.5.0a6/jobbergate_api/tests/apps/__init__.py
+-rw-r--r--   0        0        0       44 2023-06-26 17:06:40.207826 jobbergate_api-3.5.0a6/jobbergate_api/tests/apps/applications/__init__.py
+-rw-r--r--   0        0        0    10634 2023-06-26 17:06:40.207826 jobbergate_api-3.5.0a6/jobbergate_api/tests/apps/applications/test_application_files.py
+-rw-r--r--   0        0        0     1967 2023-06-26 17:06:40.207826 jobbergate_api-3.5.0a6/jobbergate_api/tests/apps/applications/test_file_validation.py
+-rw-r--r--   0        0        0    50586 2023-06-26 17:06:40.211826 jobbergate_api-3.5.0a6/jobbergate_api/tests/apps/applications/test_routers.py
+-rw-r--r--   0        0        0     5180 2023-06-26 17:06:40.211826 jobbergate_api-3.5.0a6/jobbergate_api/tests/apps/applications/test_schemas.py
+-rw-r--r--   0        0        0     2756 2023-06-26 17:06:40.211826 jobbergate_api-3.5.0a6/jobbergate_api/tests/apps/conftest.py
+-rw-r--r--   0        0        0       42 2023-06-26 17:06:40.211826 jobbergate_api-3.5.0a6/jobbergate_api/tests/apps/job_scripts/__init__.py
+-rw-r--r--   0        0        0     1376 2023-06-26 17:06:40.211826 jobbergate_api-3.5.0a6/jobbergate_api/tests/apps/job_scripts/conftest.py
+-rw-r--r--   0        0        0    11518 2023-06-26 17:06:40.211826 jobbergate_api-3.5.0a6/jobbergate_api/tests/apps/job_scripts/test_job_script_files.py
+-rw-r--r--   0        0        0    57121 2023-06-26 17:06:40.211826 jobbergate_api-3.5.0a6/jobbergate_api/tests/apps/job_scripts/test_routers.py
+-rw-r--r--   0        0        0       46 2023-06-26 17:06:40.211826 jobbergate_api-3.5.0a6/jobbergate_api/tests/apps/job_submissions/__init__.py
+-rw-r--r--   0        0        0    24706 2023-06-26 17:06:40.211826 jobbergate_api-3.5.0a6/jobbergate_api/tests/apps/job_submissions/test_properties_parser.py
+-rw-r--r--   0        0        0    80706 2023-06-26 17:06:40.211826 jobbergate_api-3.5.0a6/jobbergate_api/tests/apps/job_submissions/test_routers.py
+-rw-r--r--   0        0        0      511 2023-06-26 17:06:40.211826 jobbergate_api-3.5.0a6/jobbergate_api/tests/apps/test_main.py
+-rw-r--r--   0        0        0     8900 2023-06-26 17:06:40.211826 jobbergate_api-3.5.0a6/jobbergate_api/tests/conftest.py
+-rw-r--r--   0        0        0     4503 2023-06-26 17:06:40.211826 jobbergate_api-3.5.0a6/jobbergate_api/tests/integration/draft_test_jobbergate_slurm_job_properties.py
+-rw-r--r--   0        0        0     3215 2023-06-26 17:06:40.211826 jobbergate_api-3.5.0a6/jobbergate_api/tests/test_config.py
+-rw-r--r--   0        0        0     4974 2023-06-26 17:06:40.211826 jobbergate_api-3.5.0a6/jobbergate_api/tests/test_email_notification.py
+-rw-r--r--   0        0        0     3177 2023-06-26 17:06:40.211826 jobbergate_api-3.5.0a6/jobbergate_api/tests/test_meta_mapper.py
+-rw-r--r--   0        0        0     3959 2023-06-26 17:06:40.211826 jobbergate_api-3.5.0a6/jobbergate_api/tests/test_pagination.py
+-rw-r--r--   0        0        0     1146 2023-06-26 17:06:40.211826 jobbergate_api-3.5.0a6/jobbergate_api/tests/test_s3_manager.py
+-rw-r--r--   0        0        0     2718 2023-06-26 17:06:40.211826 jobbergate_api-3.5.0a6/jobbergate_api/tests/test_security.py
+-rw-r--r--   0        0        0     4512 2023-06-26 17:06:40.211826 jobbergate_api-3.5.0a6/jobbergate_api/tests/test_storage.py
+-rw-r--r--   0        0        0     2777 2023-06-26 17:06:40.211826 jobbergate_api-3.5.0a6/jobbergate_api/tests/test_version.py
+-rw-r--r--   0        0        0     1102 2023-06-26 17:06:40.211826 jobbergate_api-3.5.0a6/jobbergate_api/version.py
+-rw-r--r--   0        0        0     2898 2023-06-26 17:06:40.211826 jobbergate_api-3.5.0a6/pyproject.toml
+-rw-r--r--   0        0        0     2756 1970-01-01 00:00:00.000000 jobbergate_api-3.5.0a6/PKG-INFO
```

### Comparing `jobbergate_api-3.5.0a5/LICENSE` & `jobbergate_api-3.5.0a6/LICENSE`

 * *Files identical despite different names*

### Comparing `jobbergate_api-3.5.0a5/README.rst` & `jobbergate_api-3.5.0a6/README.rst`

 * *Files identical despite different names*

### Comparing `jobbergate_api-3.5.0a5/jobbergate_api/apps/applications/application_files.py` & `jobbergate_api-3.5.0a6/jobbergate_api/apps/applications/application_files.py`

 * *Files identical despite different names*

### Comparing `jobbergate_api-3.5.0a5/jobbergate_api/apps/applications/file_validation.py` & `jobbergate_api-3.5.0a6/jobbergate_api/apps/applications/file_validation.py`

 * *Files identical despite different names*

### Comparing `jobbergate_api-3.5.0a5/jobbergate_api/apps/applications/models.py` & `jobbergate_api-3.5.0a6/jobbergate_api/apps/applications/models.py`

 * *Files identical despite different names*

### Comparing `jobbergate_api-3.5.0a5/jobbergate_api/apps/applications/routers.py` & `jobbergate_api-3.5.0a6/jobbergate_api/apps/applications/routers.py`

 * *Files 14% similar despite different names*

```diff
@@ -16,29 +16,44 @@
 from jobbergate_api.apps.applications.schemas import (
     ApplicationCreateRequest,
     ApplicationPartialResponse,
     ApplicationResponse,
     ApplicationUpdateRequest,
 )
 from jobbergate_api.apps.job_scripts.models import job_scripts_table
-from jobbergate_api.apps.permissions import Permissions
+from jobbergate_api.apps.permissions import Permissions, check_owner
 from jobbergate_api.config import settings
 from jobbergate_api.pagination import Pagination, ok_response, package_response
 from jobbergate_api.security import IdentityClaims, guard
 from jobbergate_api.storage import (
     INTEGRITY_CHECK_EXCEPTIONS,
     database,
     render_sql,
     search_clause,
     sort_clause,
 )
 
 router = APIRouter()
 
 
+async def _fetch_application_by_id(application_id: int) -> ApplicationPartialResponse:
+    """
+    Fetch an application from the database by its id.
+    """
+    select_query = applications_table.select().where(applications_table.c.id == application_id)
+    raw_application = await database.fetch_one(select_query)
+
+    if not raw_application:
+        message = f"Application {application_id=} not found."
+        logger.error(message)
+        raise HTTPException(status_code=status.HTTP_404_NOT_FOUND, detail=message)
+
+    return ApplicationPartialResponse.parse_obj(raw_application)
+
+
 @router.post(
     "/applications",
     status_code=status.HTTP_201_CREATED,
     response_model=ApplicationPartialResponse,
     description="Endpoint for application creation",
 )
 async def applications_create(
@@ -72,34 +87,38 @@
     return application_data
 
 
 @router.post(
     "/applications/{application_id}/upload",
     status_code=status.HTTP_201_CREATED,
     description="Endpoint for uploading application files.",
-    dependencies=[Depends(guard.lockdown(Permissions.APPLICATIONS_EDIT))],
 )
 async def applications_upload(
     application_id: int = Query(..., description="id of the application for which to upload a file"),
     upload_files: List[UploadFile] = File(..., description="The application files to be uploaded"),
     content_length: int = Header(...),
+    token_payload: TokenPayload = Depends(guard.lockdown(Permissions.APPLICATIONS_EDIT)),
 ):
     """
     Upload application files using an authenticated user token.
     """
     logger.debug(f"Preparing to receive upload files for {application_id=}")
 
     if content_length > settings.MAX_UPLOAD_FILE_SIZE:
         message = f"Uploaded files cannot exceed {settings.MAX_UPLOAD_FILE_SIZE} bytes."
         logger.warning(message)
         raise HTTPException(
             status_code=status.HTTP_413_REQUEST_ENTITY_TOO_LARGE,
             detail=message,
         )
 
+    identity_claims = IdentityClaims.from_token_payload(token_payload)
+    application = await _fetch_application_by_id(application_id)
+    check_owner(application.application_owner_email, identity_claims.email, application_id, "application")
+
     ApplicationFiles.get_from_upload_files(upload_files).write_to_s3(application_id)
 
     update_query = (
         applications_table.update()
         .where(applications_table.c.id == application_id)
         .values(dict(application_uploaded=True))
     )
@@ -107,24 +126,31 @@
     logger.trace(f"update_query = {render_sql(update_query)}")
     await database.execute(update_query)
 
 
 @router.patch(
     "/applications/{application_id}/upload/individually",
     status_code=status.HTTP_204_NO_CONTENT,
-    responses={204: {"description": "File(s) was(were) patched successfully"}},
-    dependencies=[Depends(guard.lockdown(Permissions.APPLICATIONS_EDIT))],
+    responses={
+        204: {"description": "File(s) was(were) patched successfully"},
+        403: {"description": "User does not own application"},
+    },
 )
 async def update_application_source_file(
     application_id: int = Query(..., description="id of the application for which to upload a file"),
     source_file: Union[UploadFile, None] = File(default=None),
     config_file: Union[UploadFile, None] = File(default=None),
     template_files: Union[List[UploadFile], None] = None,
+    token_payload: TokenPayload = Depends(guard.lockdown(Permissions.APPLICATIONS_EDIT)),
 ):
     """Update the application files individually."""
+    identity_claims = IdentityClaims.from_token_payload(token_payload)
+    application = await _fetch_application_by_id(application_id)
+    check_owner(application.application_owner_email, identity_claims.email, application_id, "application")
+
     # TODO: limit by file size
     ApplicationFiles(
         application_config=config_file.file.read().decode("utf-8") if config_file is not None else None,
         application_source_file=source_file.file.read().decode("utf-8") if source_file is not None else None,
         application_templates={
             PurePath(template_file.filename).name: template_file.file.read().decode("utf-8")
             for template_file in template_files
@@ -136,33 +162,27 @@
     return FastAPIResponse(status_code=status.HTTP_204_NO_CONTENT)
 
 
 @router.delete(
     "/applications/{application_id}/upload",
     status_code=status.HTTP_204_NO_CONTENT,
     description="Endpoint for deleting application files",
-    dependencies=[Depends(guard.lockdown(Permissions.APPLICATIONS_EDIT))],
 )
 async def applications_delete_upload(
     application_id: int = Query(..., description="id of the application for which to delete the file"),
+    token_payload: TokenPayload = Depends(guard.lockdown(Permissions.APPLICATIONS_EDIT)),
 ):
     """
     Delete application files using an authenticated user token.
     """
     logger.debug(f"Preparing to delete files for {application_id=}")
 
-    select_query = applications_table.select().where(applications_table.c.id == application_id)
-    raw_application = await database.fetch_one(select_query)
-
-    if not raw_application:
-        message = f"Application {application_id=} not found."
-        logger.warning(message)
-        raise HTTPException(status_code=status.HTTP_404_NOT_FOUND, detail=message)
-
-    application = ApplicationPartialResponse.parse_obj(raw_application)
+    identity_claims = IdentityClaims.from_token_payload(token_payload)
+    application = await _fetch_application_by_id(application_id)
+    check_owner(application.application_owner_email, identity_claims.email, application_id, "application")
 
     if not application.application_uploaded:
         logger.debug(f"Trying to delete an applications that was not uploaded ({application_id=})")
         return FastAPIResponse(status_code=status.HTTP_204_NO_CONTENT)
 
     ApplicationFiles.delete_from_s3(application_id)
 
@@ -178,22 +198,26 @@
     return FastAPIResponse(status_code=status.HTTP_204_NO_CONTENT)
 
 
 @router.delete(
     "/applications/{application_id}",
     status_code=status.HTTP_204_NO_CONTENT,
     description="Endpoint to delete application",
-    dependencies=[Depends(guard.lockdown(Permissions.APPLICATIONS_EDIT))],
 )
 async def application_delete(
     application_id: int = Query(..., description="id of the application to delete"),
+    token_payload: TokenPayload = Depends(guard.lockdown(Permissions.APPLICATIONS_EDIT)),
 ):
     """
     Delete application from the database and S3 given its id.
     """
+    identity_claims = IdentityClaims.from_token_payload(token_payload)
+    application = await _fetch_application_by_id(application_id)
+    check_owner(application.application_owner_email, identity_claims.email, application_id, "application")
+
     logger.debug(f"Orphaning job_scripts rendered from application {application_id=}")
     update_query = (
         job_scripts_table.update()
         .where(job_scripts_table.c.application_id == application_id)
         .values(dict(application_id=None))
     )
 
@@ -225,18 +249,18 @@
     return FastAPIResponse(status_code=status.HTTP_204_NO_CONTENT)
 
 
 @router.delete(
     "/applications",
     status_code=status.HTTP_204_NO_CONTENT,
     description="Endpoint to delete application by identifier",
-    dependencies=[Depends(guard.lockdown(Permissions.APPLICATIONS_EDIT))],
 )
 async def application_delete_by_identifier(
     identifier: str = Query(..., description="identifier of the application to delete"),
+    token_payload: TokenPayload = Depends(guard.lockdown(Permissions.APPLICATIONS_EDIT)),
 ):
     """
     Delete application from the database and S3 given it's identifier.
     """
     logger.debug(f"Preparing to delete {identifier=} from the database and S3")
 
     where_stmt = applications_table.c.application_identifier == identifier
@@ -247,22 +271,25 @@
     if not raw_application:
         message = f"Application {identifier=} not found."
         logger.warning(message)
         raise HTTPException(
             status_code=status.HTTP_404_NOT_FOUND,
             detail=message,
         )
+    application = ApplicationPartialResponse.parse_obj(raw_application)
+
+    identity_claims = IdentityClaims.from_token_payload(token_payload)
+    check_owner(application.application_owner_email, identity_claims.email, application.id, "application")
 
-    id_ = raw_application["id"]
     delete_query = applications_table.delete().where(where_stmt)
     logger.trace(f"delete_query = {render_sql(delete_query)}")
 
     await database.execute(delete_query)
 
-    ApplicationFiles.delete_from_s3(id_)
+    ApplicationFiles.delete_from_s3(application.id)
 
     return FastAPIResponse(status_code=status.HTTP_204_NO_CONTENT)
 
 
 @router.get(
     "/applications",
     description="Endpoint to list applications",
@@ -355,24 +382,27 @@
 
 
 @router.put(
     "/applications/{application_id}",
     status_code=status.HTTP_200_OK,
     description="Endpoint to update an application given the id",
     response_model=ApplicationPartialResponse,
-    dependencies=[Depends(guard.lockdown(Permissions.APPLICATIONS_EDIT))],
 )
 async def application_update(
     application_id: int,
     application: ApplicationUpdateRequest,
+    token_payload: TokenPayload = Depends(guard.lockdown(Permissions.APPLICATIONS_EDIT)),
 ):
     """
     Update an application given it's id.
     """
     logger.debug(f"Preparing to update {application_id=}")
+    identity_claims = IdentityClaims.from_token_payload(token_payload)
+    old_application = await _fetch_application_by_id(application_id)
+    check_owner(old_application.application_owner_email, identity_claims.email, application_id, "application")
 
     update_query = (
         applications_table.update()
         .where(applications_table.c.id == application_id)
         .values(application.dict(exclude_unset=True))
         .returning(applications_table)
     )
```

### Comparing `jobbergate_api-3.5.0a5/jobbergate_api/apps/applications/schemas.py` & `jobbergate_api-3.5.0a6/jobbergate_api/apps/applications/schemas.py`

 * *Files identical despite different names*

### Comparing `jobbergate_api-3.5.0a5/jobbergate_api/apps/job_scripts/job_script_files.py` & `jobbergate_api-3.5.0a6/jobbergate_api/apps/job_scripts/job_script_files.py`

 * *Files identical despite different names*

### Comparing `jobbergate_api-3.5.0a5/jobbergate_api/apps/job_scripts/models.py` & `jobbergate_api-3.5.0a6/jobbergate_api/apps/job_scripts/models.py`

 * *Files identical despite different names*

### Comparing `jobbergate_api-3.5.0a5/jobbergate_api/apps/job_scripts/routers.py` & `jobbergate_api-3.5.0a6/jobbergate_api/apps/job_scripts/routers.py`

 * *Files 8% similar despite different names*

```diff
@@ -19,28 +19,43 @@
 from jobbergate_api.apps.job_scripts.models import job_scripts_table, searchable_fields, sortable_fields
 from jobbergate_api.apps.job_scripts.schemas import (
     JobScriptCreateRequest,
     JobScriptResponse,
     JobScriptUpdateRequest,
 )
 from jobbergate_api.apps.job_submissions.models import job_submissions_table
-from jobbergate_api.apps.permissions import Permissions
+from jobbergate_api.apps.permissions import Permissions, check_owner
 from jobbergate_api.pagination import Pagination, ok_response, package_response
 from jobbergate_api.security import IdentityClaims, guard
 from jobbergate_api.storage import (
     INTEGRITY_CHECK_EXCEPTIONS,
     database,
     render_sql,
     search_clause,
     sort_clause,
 )
 
 router = APIRouter()
 
 
+async def _fetch_job_script_by_id(job_script_id: int) -> JobScriptResponse:
+    """
+    Fetch a job_script from the database by its id.
+    """
+    select_query = job_scripts_table.select().where(job_scripts_table.c.id == job_script_id)
+    raw_job_script = await database.fetch_one(select_query)
+
+    if not raw_job_script:
+        message = f"Job Script with {job_script_id=} was not found."
+        logger.error(message)
+        raise HTTPException(status_code=status.HTTP_404_NOT_FOUND, detail=message)
+
+    return JobScriptResponse.parse_obj(raw_job_script)
+
+
 @router.post(
     "/job-scripts",
     status_code=status.HTTP_201_CREATED,
     response_model=JobScriptResponse,
     description="Endpoint for job_script creation",
 )
 async def job_script_create(
@@ -188,77 +203,67 @@
     return response
 
 
 @router.post(
     "/job-scripts/{job_script_id}/upload",
     status_code=status.HTTP_200_OK,
     description="Endpoint to upload a new job script file.",
-    dependencies=[Depends(guard.lockdown(Permissions.JOB_SCRIPTS_EDIT))],
 )
 async def job_script_create_file_content(
     job_script_id: int = Query(...),
     job_script_file: UploadFile = File(...),
+    token_payload: TokenPayload = Depends(guard.lockdown(Permissions.JOB_SCRIPTS_EDIT)),
 ):
     """Create a job script file (only if the job script has none)."""
     logger.debug(f"Creating the main file for {job_script_id=}")
 
-    query = job_scripts_table.select().where(job_scripts_table.c.id == job_script_id)
-    logger.trace(f"get_query = {render_sql(query)}")
-    job_script = await database.fetch_one(query)
-
-    if not job_script:
-        message = f"JobScript with id={job_script_id} was not found."
-        logger.warning(message)
-        raise HTTPException(status_code=status.HTTP_404_NOT_FOUND, detail=message)
+    identity_claims = IdentityClaims.from_token_payload(token_payload)
+    job_script = await _fetch_job_script_by_id(job_script_id)
+    check_owner(job_script.job_script_owner_email, identity_claims.email, job_script_id, "job_script")
 
     jobscript_files = JobScriptFiles.get_from_single_upload_file(job_script_file)
     jobscript_files.write_to_s3(job_script_id, remove_previous_files=True)
 
     update_query = (
         job_scripts_table.update()
-        .where(job_scripts_table.c.id == job_script["id"])
+        .where(job_scripts_table.c.id == job_script_id)
         .values(updated_at=func.now())
     )
     await database.execute(update_query)
     logger.debug(f"Success creating job script files from single upload file for {job_script_id=}")
     return dict(message=f"Successfully uploaded {job_script_file.filename} for {job_script_id=}")
 
 
 @router.patch(
     "/job-scripts/{job_script_id}/upload",
     status_code=status.HTTP_204_NO_CONTENT,
     description="Endpoint to replace a job script file.",
-    dependencies=[Depends(guard.lockdown(Permissions.JOB_SCRIPTS_EDIT))],
 )
 async def job_script_replace_file_content(
     job_script_id: int = Query(...),
     job_script_file: UploadFile = File(...),
+    token_payload: TokenPayload = Depends(guard.lockdown(Permissions.JOB_SCRIPTS_EDIT)),
 ):
     """Replace the content on a job script file."""
     logger.debug(f"Replacing the main file from {job_script_id=}")
 
-    query = job_scripts_table.select().where(job_scripts_table.c.id == job_script_id)
-    logger.trace(f"get_query = {render_sql(query)}")
-    job_script = await database.fetch_one(query)
-
-    if not job_script:
-        message = f"JobScript with id={job_script_id} was not found."
-        logger.warning(message)
-        raise HTTPException(status_code=status.HTTP_404_NOT_FOUND, detail=message)
+    identity_claims = IdentityClaims.from_token_payload(token_payload)
+    job_script = await _fetch_job_script_by_id(job_script_id)
+    check_owner(job_script.job_script_owner_email, identity_claims.email, job_script_id, "job_script")
 
     file_manager = JobScriptFiles.file_manager_factory(job_script_id)
     file_content = job_script_file.file.read().decode("utf-8")
 
     for s3_path in file_manager.keys():
         root_dir = s3_path.parts[0]
         if root_dir == JOBSCRIPTS_MAIN_FILE_FOLDER:
             file_manager[s3_path] = file_content
             update_query = (
                 job_scripts_table.update()
-                .where(job_scripts_table.c.id == job_script["id"])
+                .where(job_scripts_table.c.id == job_script_id)
                 .values(updated_at=func.now())
             )
             await database.execute(update_query)
             logger.debug(f"Success replacing the main file from {job_script_id=}")
             return None
 
     message = f"Main file from {job_script_id=} was not found."
@@ -354,46 +359,37 @@
     return await package_response(JobScriptResponse, query, pagination)
 
 
 @router.delete(
     "/job-scripts/{job_script_id}",
     status_code=status.HTTP_204_NO_CONTENT,
     description="Endpoint to delete job script",
-    dependencies=[Depends(guard.lockdown(Permissions.JOB_SCRIPTS_EDIT))],
 )
-async def job_script_delete(job_script_id: int = Query(..., description="id of the job script to delete")):
+async def job_script_delete(
+    job_script_id: int = Query(..., description="id of the job script to delete"),
+    token_payload: TokenPayload = Depends(guard.lockdown(Permissions.JOB_SCRIPTS_EDIT)),
+):
     """
     Delete job_script given its id.
     """
+    identity_claims = IdentityClaims.from_token_payload(token_payload)
+    job_script = await _fetch_job_script_by_id(job_script_id)
+    check_owner(job_script.job_script_owner_email, identity_claims.email, job_script_id, "job_script")
+
     logger.debug(f"Orphaning job_submissions submitted from job_script {job_script_id=}")
     update_query = (
         job_submissions_table.update()
         .where(job_submissions_table.c.job_script_id == job_script_id)
         .values(dict(job_script_id=None))
     )
     logger.trace(f"update_query = {render_sql(update_query)}")
     await database.execute(update_query)
 
     logger.debug(f"Preparing to delete {job_script_id=}")
-    where_stmt = job_scripts_table.c.id == job_script_id
-
-    get_query = job_scripts_table.select().where(where_stmt)
-    logger.trace(f"get_query = {render_sql(get_query)}")
-
-    raw_job_script = await database.fetch_one(get_query)
-    if not raw_job_script:
-
-        message = f"JobScript with id={job_script_id} not found."
-        logger.warning(message)
-        raise HTTPException(
-            status_code=status.HTTP_404_NOT_FOUND,
-            detail=message,
-        )
-
-    delete_query = job_scripts_table.delete().where(where_stmt)
+    delete_query = job_scripts_table.delete().where(job_scripts_table.c.id == job_script_id)
     logger.trace(f"delete_query = {render_sql(delete_query)}")
     await database.execute(delete_query)
 
     try:
         JobScriptFiles.delete_from_s3(job_script_id)
     except KeyError:
         # There is no need to raise an error if we try to delete a file that does not exist
@@ -401,21 +397,27 @@
 
 
 @router.put(
     "/job-scripts/{job_script_id}",
     status_code=status.HTTP_200_OK,
     description="Endpoint to update a job_script given the id",
     response_model=JobScriptResponse,
-    dependencies=[Depends(guard.lockdown(Permissions.JOB_SCRIPTS_EDIT))],
 )
-async def job_script_update(job_script_id: int, job_script: JobScriptUpdateRequest):
+async def job_script_update(
+    job_script_id: int,
+    job_script: JobScriptUpdateRequest,
+    token_payload: TokenPayload = Depends(guard.lockdown(Permissions.JOB_SCRIPTS_EDIT)),
+):
     """
     Update a job_script given its id.
     """
     logger.debug(f"Updating {job_script_id=}")
+    identity_claims = IdentityClaims.from_token_payload(token_payload)
+    old_job_script = await _fetch_job_script_by_id(job_script_id)
+    check_owner(old_job_script.job_script_owner_email, identity_claims.email, job_script_id, "job_script")
 
     update_query = (
         job_scripts_table.update()
         .where(job_scripts_table.c.id == job_script_id)
         .values(
             job_script.dict(exclude_unset=True, exclude={"job_script_files"}),
         )
```

### Comparing `jobbergate_api-3.5.0a5/jobbergate_api/apps/job_scripts/schemas.py` & `jobbergate_api-3.5.0a6/jobbergate_api/apps/job_scripts/schemas.py`

 * *Files identical despite different names*

### Comparing `jobbergate_api-3.5.0a5/jobbergate_api/apps/job_submissions/constants.py` & `jobbergate_api-3.5.0a6/jobbergate_api/apps/job_submissions/constants.py`

 * *Files identical despite different names*

### Comparing `jobbergate_api-3.5.0a5/jobbergate_api/apps/job_submissions/models.py` & `jobbergate_api-3.5.0a6/jobbergate_api/apps/job_submissions/models.py`

 * *Files identical despite different names*

### Comparing `jobbergate_api-3.5.0a5/jobbergate_api/apps/job_submissions/properties_parser.py` & `jobbergate_api-3.5.0a6/jobbergate_api/apps/job_submissions/properties_parser.py`

 * *Files identical despite different names*

### Comparing `jobbergate_api-3.5.0a5/jobbergate_api/apps/job_submissions/routers.py` & `jobbergate_api-3.5.0a6/jobbergate_api/apps/job_submissions/routers.py`

 * *Files 22% similar despite different names*

```diff
@@ -21,29 +21,44 @@
 from jobbergate_api.apps.job_submissions.schemas import (
     ActiveJobSubmission,
     JobSubmissionCreateRequest,
     JobSubmissionResponse,
     JobSubmissionUpdateRequest,
     PendingJobSubmission,
 )
-from jobbergate_api.apps.permissions import Permissions
+from jobbergate_api.apps.permissions import Permissions, check_owner
 from jobbergate_api.email_notification import notify_submission_rejected
 from jobbergate_api.pagination import Pagination, ok_response, package_response
 from jobbergate_api.security import IdentityClaims, guard
 from jobbergate_api.storage import (
     INTEGRITY_CHECK_EXCEPTIONS,
     database,
     render_sql,
     search_clause,
     sort_clause,
 )
 
 router = APIRouter()
 
 
+async def _fetch_job_submission_by_id(job_submission_id: int) -> JobSubmissionResponse:
+    """
+    Fetch a job_submission from the database by its id.
+    """
+    select_query = job_submissions_table.select().where(job_submissions_table.c.id == job_submission_id)
+    raw_job_submission = await database.fetch_one(select_query)
+
+    if not raw_job_submission:
+        message = f"Job Submission with {job_submission_id=} was not found."
+        logger.error(message)
+        raise HTTPException(status_code=status.HTTP_404_NOT_FOUND, detail=message)
+
+    return JobSubmissionResponse.parse_obj(raw_job_submission)
+
+
 @router.post(
     "/job-submissions",
     status_code=201,
     description="Endpoint for job_submission creation",
     response_model=JobSubmissionResponse,
 )
 async def job_submission_create(
@@ -234,54 +249,60 @@
     return response
 
 
 @router.delete(
     "/job-submissions/{job_submission_id}",
     status_code=status.HTTP_204_NO_CONTENT,
     description="Endpoint to delete job submission",
-    dependencies=[Depends(guard.lockdown(Permissions.JOB_SUBMISSIONS_EDIT))],
 )
 async def job_submission_delete(
     job_submission_id: int = Query(..., description="id of the job submission to delete"),
+    token_payload: TokenPayload = Depends(guard.lockdown(Permissions.JOB_SUBMISSIONS_EDIT)),
 ):
     """
     Delete job_submission given its id.
     """
     logger.debug(f"Deleting {job_submission_id=}")
-    where_stmt = job_submissions_table.c.id == job_submission_id
 
-    get_query = job_submissions_table.select().where(where_stmt)
-    logger.trace(f"get_query = {render_sql(get_query)}")
-    raw_job_submission = await database.fetch_one(get_query)
-    if not raw_job_submission:
-        message = f"JobSubmission with id={job_submission_id} not found"
-        logger.warning(message)
-        raise HTTPException(
-            status_code=status.HTTP_404_NOT_FOUND,
-            detail=message,
-        )
+    identity_claims = IdentityClaims.from_token_payload(token_payload)
+    job_submission = await _fetch_job_submission_by_id(job_submission_id)
+    check_owner(
+        job_submission.job_submission_owner_email, identity_claims.email, job_submission_id, "job_submission"
+    )
 
-    delete_query = job_submissions_table.delete().where(where_stmt)
+    delete_query = job_submissions_table.delete().where(job_submissions_table.c.id == job_submission_id)
     logger.trace(f"delete_query = {render_sql(delete_query)}")
     await database.execute(delete_query)
 
 
 @router.put(
     "/job-submissions/{job_submission_id}",
     status_code=status.HTTP_200_OK,
     description="Endpoint to update a job_submission given the id",
     response_model=JobSubmissionResponse,
-    dependencies=[Depends(guard.lockdown(Permissions.JOB_SUBMISSIONS_EDIT))],
 )
-async def job_submission_update(job_submission_id: int, job_submission: JobSubmissionUpdateRequest):
+async def job_submission_update(
+    job_submission_id: int,
+    job_submission: JobSubmissionUpdateRequest,
+    token_payload: TokenPayload = Depends(guard.lockdown(Permissions.JOB_SUBMISSIONS_EDIT)),
+):
     """
     Update a job_submission given its id.
     """
     logger.debug(f"Updating {job_submission_id=}")
 
+    identity_claims = IdentityClaims.from_token_payload(token_payload)
+    old_job_submission = await _fetch_job_submission_by_id(job_submission_id)
+    check_owner(
+        old_job_submission.job_submission_owner_email,
+        identity_claims.email,
+        job_submission_id,
+        "job_submission",
+    )
+
     update_dict = job_submission.dict(exclude_unset=True)
     exec_dir = update_dict.pop("execution_directory", None)
     if exec_dir is not None:
         update_dict.update(execution_directory=str(exec_dir))
 
     update_query = (
         job_submissions_table.update()
```

### Comparing `jobbergate_api-3.5.0a5/jobbergate_api/apps/job_submissions/schemas.py` & `jobbergate_api-3.5.0a6/jobbergate_api/apps/job_submissions/schemas.py`

 * *Files identical despite different names*

### Comparing `jobbergate_api-3.5.0a5/jobbergate_api/config.py` & `jobbergate_api-3.5.0a6/jobbergate_api/config.py`

 * *Files identical despite different names*

### Comparing `jobbergate_api-3.5.0a5/jobbergate_api/email_notification.py` & `jobbergate_api-3.5.0a6/jobbergate_api/email_notification.py`

 * *Files identical despite different names*

### Comparing `jobbergate_api-3.5.0a5/jobbergate_api/main.py` & `jobbergate_api-3.5.0a6/jobbergate_api/main.py`

 * *Files identical despite different names*

### Comparing `jobbergate_api-3.5.0a5/jobbergate_api/meta_mapper.py` & `jobbergate_api-3.5.0a6/jobbergate_api/meta_mapper.py`

 * *Files identical despite different names*

### Comparing `jobbergate_api-3.5.0a5/jobbergate_api/pagination.py` & `jobbergate_api-3.5.0a6/jobbergate_api/pagination.py`

 * *Files identical despite different names*

### Comparing `jobbergate_api-3.5.0a5/jobbergate_api/s3_manager.py` & `jobbergate_api-3.5.0a6/jobbergate_api/s3_manager.py`

 * *Files identical despite different names*

### Comparing `jobbergate_api-3.5.0a5/jobbergate_api/security.py` & `jobbergate_api-3.5.0a6/jobbergate_api/security.py`

 * *Files identical despite different names*

### Comparing `jobbergate_api-3.5.0a5/jobbergate_api/storage.py` & `jobbergate_api-3.5.0a6/jobbergate_api/storage.py`

 * *Files identical despite different names*

### Comparing `jobbergate_api-3.5.0a5/jobbergate_api/tests/apps/applications/test_application_files.py` & `jobbergate_api-3.5.0a6/jobbergate_api/tests/apps/applications/test_application_files.py`

 * *Files identical despite different names*

### Comparing `jobbergate_api-3.5.0a5/jobbergate_api/tests/apps/applications/test_file_validation.py` & `jobbergate_api-3.5.0a6/jobbergate_api/tests/apps/applications/test_file_validation.py`

 * *Files identical despite different names*

### Comparing `jobbergate_api-3.5.0a5/jobbergate_api/tests/apps/applications/test_routers.py` & `jobbergate_api-3.5.0a6/jobbergate_api/tests/apps/applications/test_routers.py`

 * *Files 17% similar despite different names*

```diff
@@ -109,26 +109,28 @@
     count = await database.fetch_all("SELECT COUNT(*) FROM applications")
     assert count[0][0] == 0
 
 
 @pytest.mark.asyncio
 @mock.patch("jobbergate_api.apps.applications.routers.ApplicationFiles.delete_from_s3")
 async def test_delete_application_no_file_uploaded(
-    mocked_application_deleter, client, application_data, inject_security_header
+    mocked_application_deleter, client, fill_application_data, inject_security_header
 ):
     """
     Test DELETE /applications/<id> correctly deletes an application.
 
     This test proves that an application is successfully deleted via a DELETE request to the
     /applications/<id> endpoint. We show this by asserting that the application no longer exists in the
     database after the delete request is made and the correct status code is returned.
     """
     inserted_id = await database.execute(
         query=applications_table.insert(),
-        values=application_data,
+        values=fill_application_data(
+            application_owner_email="owner1@org.com",
+        ),
     )
     count = await database.fetch_all("SELECT COUNT(*) FROM applications")
     assert count[0][0] == 1
 
     inject_security_header("owner1@org.com", Permissions.APPLICATIONS_EDIT)
     response = await client.delete(f"/jobbergate/applications/{inserted_id}")
 
@@ -138,27 +140,29 @@
 
     mocked_application_deleter.assert_called_once_with(inserted_id)
 
 
 @pytest.mark.asyncio
 @mock.patch("jobbergate_api.apps.applications.routers.ApplicationFiles.delete_from_s3")
 async def test_delete_application_with_uploaded_file(
-    mocked_application_deleter, client, application_data, inject_security_header
+    mocked_application_deleter, client, fill_application_data, inject_security_header
 ):
     """
     Test DELETE /applications/<id> correctly deletes an application and it's file.
 
     This test proves that an application is successfully deleted via a DELETE request to the
     /applications/<id> endpoint. We show this by asserting that the application no longer exists in the
     database after the delete request is made, the correct status code is returned and the correct boto3
     method was called.
     """
     inserted_id = await database.execute(
         query=applications_table.insert(),
-        values=application_data,
+        values=fill_application_data(
+            application_owner_email="owner1@org.com",
+        ),
     )
     count = await database.fetch_all("SELECT COUNT(*) FROM applications")
     assert count[0][0] == 1
 
     inject_security_header("owner1@org.com", Permissions.APPLICATIONS_EDIT)
     response = await client.delete(f"/jobbergate/applications/{inserted_id}")
 
@@ -201,39 +205,71 @@
 
     mocked_application_deleter.assert_called_once_with(inserted_id)
 
 
 @pytest.mark.asyncio
 async def test_delete_application_bad_permission(
     client,
-    application_data,
+    fill_application_data,
     inject_security_header,
 ):
     """
     Test that it is not possible to delete application without proper permission.
 
     This test proves that an application is not deleted via a DELETE request to the /applications/<id>
     endpoint. We show this by asserting that the application still exists in the database after the delete
     request is made and the correct status code is returned.
     """
     inserted_id = await database.execute(
         query=applications_table.insert(),
-        values=application_data,
+        values=fill_application_data(
+            application_owner_email="owner1@org.com",
+        ),
     )
     count = await database.fetch_all("SELECT COUNT(*) FROM applications")
     assert count[0][0] == 1
 
     inject_security_header("owner1@org.com", "INVALID_PERMISSION")
     response = await client.delete(f"/jobbergate/applications/{inserted_id}")
     assert response.status_code == status.HTTP_403_FORBIDDEN
     count = await database.fetch_all("SELECT COUNT(*) FROM applications")
     assert count[0][0] == 1
 
 
 @pytest.mark.asyncio
+async def test_delete_application_non_owner(
+    client,
+    fill_application_data,
+    inject_security_header,
+):
+    """
+    Test that it is not possible to delete application if you are not the owner.
+
+    This test proves that an application is not deleted via a DELETE request to the /applications/<id>
+    endpoint. We show this by asserting that the application still exists in the database after the delete
+    request is made and the correct status code is returned.
+    """
+    inserted_id = await database.execute(
+        query=applications_table.insert(),
+        values=fill_application_data(
+            application_owner_email="owner1@org.com",
+        ),
+    )
+    count = await database.fetch_all("SELECT COUNT(*) FROM applications")
+    assert count[0][0] == 1
+
+    inject_security_header("other-owner@other.com", Permissions.APPLICATIONS_EDIT)
+    response = await client.delete(f"/jobbergate/applications/{inserted_id}")
+    assert response.status_code == status.HTTP_403_FORBIDDEN
+    assert "does not own" in response.text
+    count = await database.fetch_all("SELECT COUNT(*) FROM applications")
+    assert count[0][0] == 1
+
+
+@pytest.mark.asyncio
 async def test_delete_application_not_found(client, inject_security_header):
     """
     Test DELETE /applications/<id> the correct response code when the application doesn't exist.
 
     This test proves that DELETE /applications/<id> returns the correct response code (404)
     when the application id does not exist in the database. We show this by asserting that a 404 response
     code is returned for a request made with an application id that doesn't exist.
@@ -244,26 +280,28 @@
 
 
 @pytest.mark.asyncio
 @mock.patch("jobbergate_api.apps.applications.routers.ApplicationFiles.delete_from_s3")
 async def test_delete_application__unlinks_job_scripts(
     mocked_application_deleter,
     client,
-    application_data,
+    fill_application_data,
     job_script_data,
     inject_security_header,
 ):
     """
     Test DELETE /applications/<id> correctly deletes an application linked to a job_script.
 
     Test that a the application_id field for connected job_scripts is set to null.
     """
     inserted_id = await database.execute(
         query=applications_table.insert(),
-        values=application_data,
+        values=fill_application_data(
+            application_owner_email="owner1@org.com",
+        ),
     )
     count = await database.fetch_all("SELECT COUNT(*) FROM applications")
     assert count[0][0] == 1
 
     await database.execute(
         query=job_scripts_table.insert(),
         values=dict(
@@ -958,14 +996,60 @@
     assert result is not None
     assert result["application_name"] == "old-name"
     assert result["application_identifier"] == "old_identifier"
     assert result["application_description"] == "old description"
 
 
 @pytest.mark.asyncio
+async def test_update_application_non_owner(
+    client,
+    fill_application_data,
+    inject_security_header,
+):
+    """
+    Test that it is not possible to update applications if you are not the owner.
+
+    This test proves that an application's values are not updated following a PUT request to the
+    /application/<id> endpoint by a user without permission. We show this by asserting that the status code
+    403 is returned and that the application_data is still the same as before.
+    """
+    inserted_id = await database.execute(
+        query=applications_table.insert(),
+        values=fill_application_data(
+            application_name="old-name",
+            application_identifier="old_identifier",
+            application_owner_email="owner1@org.com",
+            application_description="old description",
+        ),
+    )
+    count = await database.fetch_all("SELECT COUNT(*) FROM applications")
+    assert count[0][0] == 1
+
+    inject_security_header("other-owner@org.com", Permissions.APPLICATIONS_EDIT)
+    response = await client.put(
+        f"/jobbergate/applications/{inserted_id}",
+        json=dict(
+            application_name="new_name",
+            application_identifier="new_identifier",
+            application_description="new_description",
+        ),
+    )
+    assert response.status_code == status.HTTP_403_FORBIDDEN
+    assert "does not own" in response.text
+
+    query = applications_table.select(applications_table.c.id == inserted_id)
+    result = await database.fetch_one(query)
+
+    assert result is not None
+    assert result["application_name"] == "old-name"
+    assert result["application_identifier"] == "old_identifier"
+    assert result["application_description"] == "old description"
+
+
+@pytest.mark.asyncio
 @mock.patch("jobbergate_api.apps.applications.routers.ApplicationFiles.write_to_s3")
 @mock.patch(
     "jobbergate_api.apps.applications.routers.ApplicationFiles.get_from_upload_files",
     return_value=ApplicationFiles(),
 )
 async def test_upload_file__works_with_small_file(
     mocked_application_writer,
@@ -1003,20 +1087,53 @@
             )
 
     assert response.status_code == status.HTTP_201_CREATED
     mocked_application_writer.assert_called_once()
     mocked_application_get_upload.assert_called_once()
 
     application = await fetch_instance(inserted_id, applications_table, ApplicationPartialResponse)
-    assert application.application_uploaded
+
+
+@pytest.mark.asyncio
+async def test_upload_file__fails_for_non_owner(
+    client,
+    inject_security_header,
+    fill_application_data,
+    tweak_settings,
+    make_dummy_file,
+    dummy_application_config,
+    make_files_param,
+):
+    """
+    Test that a file cannot be uploaded by a non-owner.
+    """
+    inserted_id = await database.execute(
+        query=applications_table.insert(),
+        values=fill_application_data(application_owner_email="owner1@org.com"),
+    )
+    application = await fetch_instance(inserted_id, applications_table, ApplicationPartialResponse)
+    assert not application.application_uploaded
+
+    dummy_file = make_dummy_file("jobbergate.yaml", content=dummy_application_config)
+    inject_security_header("non-owner@org.com", Permissions.APPLICATIONS_EDIT)
+    with tweak_settings(MAX_UPLOAD_FILE_SIZE=600):
+        with make_files_param(dummy_file) as files_param:
+            response = await client.post(
+                f"/jobbergate/applications/{inserted_id}/upload",
+                files=files_param,
+            )
+
+    assert response.status_code == status.HTTP_403_FORBIDDEN
+    assert "does not own" in response.text
+    assert not application.application_uploaded
 
 
 @pytest.mark.asyncio
 @mock.patch("jobbergate_api.apps.applications.routers.ApplicationFiles.write_to_s3")
-async def test_upload_file_individually(
+async def test_upload_file_individually__success(
     mocked_application_writer,
     client,
     inject_security_header,
     fill_application_data,
     tweak_settings,
     make_dummy_file,
     dummy_application_config,
@@ -1111,14 +1228,45 @@
 
     mocked_application_writer.assert_has_calls(
         [mock.call(inserted_id, remove_previous_files=False) for _ in range(7)]
     )
 
 
 @pytest.mark.asyncio
+async def test_upload_file_individually__fails_on_non_owner(
+    client,
+    inject_security_header,
+    fill_application_data,
+    make_dummy_file,
+    dummy_application_source_file,
+):
+    """
+    Test that the application files cannot be patched individually by a non-owner.
+    """
+    inserted_id = await database.execute(
+        query=applications_table.insert(),
+        values=fill_application_data(application_owner_email="owner1@org.com"),
+    )
+    application = await fetch_instance(inserted_id, applications_table, ApplicationPartialResponse)
+    assert not application.application_uploaded
+
+    dummy_source_file = make_dummy_file("jobbergate.py", content=dummy_application_source_file)
+
+    inject_security_header("non-owner@org.com", Permissions.APPLICATIONS_EDIT)
+
+    response = await client.patch(
+        f"/jobbergate/applications/{inserted_id}/upload/individually",
+        files={"source_file": open(dummy_source_file, "rb")},
+    )
+
+    assert response.status_code == status.HTTP_403_FORBIDDEN
+    assert "does not own" in response.text
+
+
+@pytest.mark.asyncio
 @mock.patch("jobbergate_api.apps.applications.routers.ApplicationFiles.write_to_s3")
 async def test_upload_file__fails_with_413_on_large_file(
     mocked_application_writer,
     client,
     inject_security_header,
     tweak_settings,
     make_dummy_file,
@@ -1139,15 +1287,17 @@
     assert response.status_code == status.HTTP_413_REQUEST_ENTITY_TOO_LARGE
 
     mocked_application_writer.assert_not_called()
 
 
 @pytest.mark.asyncio
 @mock.patch("jobbergate_api.apps.applications.routers.ApplicationFiles.delete_from_s3")
-async def test_delete_file(mocked_application_deleter, client, inject_security_header, fill_application_data):
+async def test_delete_file_success(
+    mocked_application_deleter, client, inject_security_header, fill_application_data
+):
     """
     Test that a file is deleted.
 
     This test proves that an application's file is deleted by making sure that the boto3 put_object method
     is called once and a 201 status code is returned.
     """
     inserted_id = await database.execute(
@@ -1163,7 +1313,32 @@
     response = await client.delete(f"/jobbergate/applications/{inserted_id}/upload")
 
     assert response.status_code == status.HTTP_204_NO_CONTENT
     mocked_application_deleter.assert_called_once_with(inserted_id)
 
     application = await fetch_instance(inserted_id, applications_table, ApplicationPartialResponse)
     assert not application.application_uploaded
+
+
+@pytest.mark.asyncio
+@mock.patch("jobbergate_api.apps.applications.routers.ApplicationFiles.delete_from_s3")
+async def test_delete_file__fails_with_403_for_non_owner(
+    mocked_application_deleter, client, inject_security_header, fill_application_data
+):
+    """
+    Test that a file is not deleted if the requester is not the owner.
+    """
+    inserted_id = await database.execute(
+        query=applications_table.insert(),
+        values=fill_application_data(application_owner_email="owner1@org.com", application_uploaded=True),
+    )
+    application: ApplicationPartialResponse = await fetch_instance(
+        inserted_id, applications_table, ApplicationPartialResponse
+    )
+    assert application.application_uploaded
+
+    inject_security_header("non-owner@org.com", Permissions.APPLICATIONS_EDIT)
+    response = await client.delete(f"/jobbergate/applications/{inserted_id}/upload")
+
+    assert response.status_code == status.HTTP_403_FORBIDDEN
+    assert "does not own" in response.text
+    mocked_application_deleter.assert_not_called()
```

### Comparing `jobbergate_api-3.5.0a5/jobbergate_api/tests/apps/applications/test_schemas.py` & `jobbergate_api-3.5.0a6/jobbergate_api/tests/apps/applications/test_schemas.py`

 * *Files identical despite different names*

### Comparing `jobbergate_api-3.5.0a5/jobbergate_api/tests/apps/conftest.py` & `jobbergate_api-3.5.0a6/jobbergate_api/tests/apps/conftest.py`

 * *Files identical despite different names*

### Comparing `jobbergate_api-3.5.0a5/jobbergate_api/tests/apps/job_scripts/conftest.py` & `jobbergate_api-3.5.0a6/jobbergate_api/tests/apps/job_scripts/conftest.py`

 * *Files identical despite different names*

### Comparing `jobbergate_api-3.5.0a5/jobbergate_api/tests/apps/job_scripts/test_job_script_files.py` & `jobbergate_api-3.5.0a6/jobbergate_api/tests/apps/job_scripts/test_job_script_files.py`

 * *Files identical despite different names*

### Comparing `jobbergate_api-3.5.0a5/jobbergate_api/tests/apps/job_scripts/test_routers.py` & `jobbergate_api-3.5.0a6/jobbergate_api/tests/apps/job_scripts/test_routers.py`

 * *Files 2% similar despite different names*

```diff
@@ -583,15 +583,15 @@
 
     response = await client.patch(
         "/jobbergate/job-scripts/1/upload",
         files={"job_script_file": open(new_job_script_file, "rb")},
     )
 
     assert response.status_code == status.HTTP_404_NOT_FOUND
-    assert "JobScript with id=1 was not found." in response.text
+    assert "Job Script with job_script_id=1 was not found." in response.text
 
 
 @pytest.mark.asyncio
 @database.transaction(force_rollback=True)
 async def test_upload_job_script_file_by_id__job_script_file_not_found(
     client,
     fill_job_script_data,
@@ -626,14 +626,50 @@
 
     assert response.status_code == status.HTTP_404_NOT_FOUND
     assert f"Main file from job_script_id={inserted_job_script_id} was not found." in response.text
 
 
 @pytest.mark.asyncio
 @database.transaction(force_rollback=True)
+async def test_upload_job_script_file_by_id__fails_for_non_owner(
+    client,
+    fill_job_script_data,
+    inject_security_header,
+    make_dummy_file,
+):
+    """Test that a job script file can not be uploaded by a non owner."""
+    inserted_job_script_id = await database.execute(
+        query=job_scripts_table.insert(),
+        values=fill_job_script_data(
+            job_script_owner_email="owner1@org.com",
+        ),
+    )
+
+    main_file_path = pathlib.Path("jobbergate.py")
+
+    new_file_content = "I'm the new content"
+
+    count = await database.fetch_all("SELECT COUNT(*) FROM job_scripts")
+    assert count[0][0] == 1
+
+    new_job_script_file = make_dummy_file(main_file_path, content=new_file_content)
+
+    inject_security_header("non-owner@org.com", Permissions.JOB_SCRIPTS_EDIT)
+
+    response = await client.patch(
+        f"/jobbergate/job-scripts/{inserted_job_script_id}/upload",
+        files={"job_script_file": open(new_job_script_file, "rb")},
+    )
+
+    assert response.status_code == status.HTTP_403_FORBIDDEN
+    assert "does not own" in response.text
+
+
+@pytest.mark.asyncio
+@database.transaction(force_rollback=True)
 async def test_get_job_script_by_id_file_not_found_at_s3(
     client,
     fill_application_data,
     fill_job_script_data,
     inject_security_header,
     mocked_file_manager_factory,
 ):
@@ -1350,14 +1386,43 @@
 
     assert job_script_row is not None
     assert job_script_row["job_script_name"] == "target-js"
 
 
 @pytest.mark.asyncio
 @database.transaction(force_rollback=True)
+async def test_update_job_script_non_owner(
+    client,
+    fill_application_data,
+    fill_job_script_data,
+    inject_security_header,
+):
+    """
+    Test that it is not possible to update a job_script if the user is not the owner.
+    """
+    inserted_application_id = await database.execute(
+        query=applications_table.insert(),
+        values=fill_application_data(application_owner_email="owner1@org.com"),
+    )
+    job_script_id = await database.execute(
+        query=job_scripts_table.insert(),
+        values=fill_job_script_data(job_script_name="target-js", application_id=inserted_application_id),
+    )
+
+    inject_security_header("non-owner@org.com", Permissions.JOB_SCRIPTS_EDIT)
+    response = await client.put(
+        f"/jobbergate/job-scripts/{job_script_id}", json={"job_script_name": "new name"}
+    )
+
+    assert response.status_code == status.HTTP_403_FORBIDDEN
+    assert "does not own" in response.text
+
+
+@pytest.mark.asyncio
+@database.transaction(force_rollback=True)
 async def test_delete_job_script(
     client,
     fill_application_data,
     fill_job_script_data,
     inject_security_header,
 ):
     """
@@ -1442,14 +1507,44 @@
 
     count = await database.fetch_all("SELECT COUNT(*) FROM job_scripts")
     assert count[0][0] == 1
 
 
 @pytest.mark.asyncio
 @database.transaction(force_rollback=True)
+async def test_delete_job_script_non_owner(
+    client,
+    fill_application_data,
+    fill_job_script_data,
+    inject_security_header,
+):
+    """
+    Test that it is not possible to delete a job_script when the user is not the owner.
+    """
+    inserted_application_id = await database.execute(
+        query=applications_table.insert(),
+        values=fill_application_data(),
+    )
+    inserted_job_script_id = await database.execute(
+        query=job_scripts_table.insert(),
+        values=fill_job_script_data(application_id=inserted_application_id),
+    )
+
+    count = await database.fetch_all("SELECT COUNT(*) FROM job_scripts")
+    assert count[0][0] == 1
+
+    inject_security_header("non-owner@org.com", Permissions.JOB_SCRIPTS_EDIT)
+    response = await client.delete(f"/jobbergate/job-scripts/{inserted_job_script_id}")
+
+    assert response.status_code == status.HTTP_403_FORBIDDEN
+    assert "does not own" in response.text
+
+
+@pytest.mark.asyncio
+@database.transaction(force_rollback=True)
 async def test_delete_job_script__unlinks_job_submissions(
     client,
     fill_application_data,
     fill_job_script_data,
     fill_job_submission_data,
     inject_security_header,
 ):
```

### Comparing `jobbergate_api-3.5.0a5/jobbergate_api/tests/apps/job_submissions/test_properties_parser.py` & `jobbergate_api-3.5.0a6/jobbergate_api/tests/apps/job_submissions/test_properties_parser.py`

 * *Files identical despite different names*

### Comparing `jobbergate_api-3.5.0a5/jobbergate_api/tests/apps/job_submissions/test_routers.py` & `jobbergate_api-3.5.0a6/jobbergate_api/tests/apps/job_submissions/test_routers.py`

 * *Files 1% similar despite different names*

```diff
@@ -1455,14 +1455,52 @@
     job_submission = JobSubmissionResponse.parse_obj(await database.fetch_one(query))
 
     assert job_submission is not None
     assert job_submission.job_submission_name == "old name"
 
 
 @pytest.mark.asyncio
+async def test_update_job_submission_non_owner(
+    client,
+    fill_application_data,
+    fill_job_script_data,
+    fill_job_submission_data,
+    inject_security_header,
+):
+    """
+    Test that it is not possible to update a job_submission if you are not the owner.
+    """
+    inserted_application_id = await database.execute(
+        query=applications_table.insert(),
+        values=fill_application_data(),
+    )
+    inserted_job_script_id = await database.execute(
+        query=job_scripts_table.insert(),
+        values=fill_job_script_data(application_id=inserted_application_id),
+    )
+    inserted_job_submission_id = await database.execute(
+        query=job_submissions_table.insert(),
+        values=fill_job_submission_data(
+            job_script_id=inserted_job_script_id,
+            job_submission_name="old name",
+            job_submission_owner_email="owner1@org.com",
+        ),
+    )
+
+    inject_security_header("non-owner@org.com", Permissions.JOB_SUBMISSIONS_EDIT)
+    response = await client.put(
+        f"/jobbergate/job-submissions/{inserted_job_submission_id}",
+        json=dict(job_submission_name="new name"),
+    )
+
+    assert response.status_code == status.HTTP_403_FORBIDDEN
+    assert "does not own" in response.text
+
+
+@pytest.mark.asyncio
 async def test_delete_job_submission(
     client,
     fill_application_data,
     fill_job_script_data,
     fill_job_submission_data,
     inject_security_header,
 ):
@@ -1555,14 +1593,51 @@
     assert response.status_code == status.HTTP_403_FORBIDDEN
 
     count = await database.fetch_all("SELECT COUNT(*) FROM job_submissions")
     assert count[0][0] == 1
 
 
 @pytest.mark.asyncio
+async def test_delete_job_submission_non_owner(
+    client,
+    fill_application_data,
+    fill_job_script_data,
+    fill_job_submission_data,
+    inject_security_header,
+):
+    """
+    Test that it is not possible to delete a job_submission if you are not the owner.
+    """
+    inserted_application_id = await database.execute(
+        query=applications_table.insert(),
+        values=fill_application_data(),
+    )
+    inserted_job_script_id = await database.execute(
+        query=job_scripts_table.insert(),
+        values=fill_job_script_data(application_id=inserted_application_id),
+    )
+    inserted_job_submission_id = await database.execute(
+        query=job_submissions_table.insert(),
+        values=fill_job_submission_data(
+            job_script_id=inserted_job_script_id,
+            job_submission_owner_email="owner1@org.com",
+        ),
+    )
+
+    count = await database.fetch_all("SELECT COUNT(*) FROM job_submissions")
+    assert count[0][0] == 1
+
+    inject_security_header("non-owner@org.com", Permissions.JOB_SUBMISSIONS_EDIT)
+    response = await client.delete(f"/jobbergate/job-submissions/{inserted_job_submission_id}")
+
+    assert response.status_code == status.HTTP_403_FORBIDDEN
+    assert "does not own" in response.text
+
+
+@pytest.mark.asyncio
 async def test_job_submissions_agent_pending__success(
     client,
     fill_application_data,
     fill_job_script_data,
     fill_all_job_submission_data,
     inject_security_header,
     mocked_file_manager_factory,
```

### Comparing `jobbergate_api-3.5.0a5/jobbergate_api/tests/conftest.py` & `jobbergate_api-3.5.0a6/jobbergate_api/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `jobbergate_api-3.5.0a5/jobbergate_api/tests/integration/draft_test_jobbergate_slurm_job_properties.py` & `jobbergate_api-3.5.0a6/jobbergate_api/tests/integration/draft_test_jobbergate_slurm_job_properties.py`

 * *Files identical despite different names*

### Comparing `jobbergate_api-3.5.0a5/jobbergate_api/tests/test_config.py` & `jobbergate_api-3.5.0a6/jobbergate_api/tests/test_config.py`

 * *Files identical despite different names*

### Comparing `jobbergate_api-3.5.0a5/jobbergate_api/tests/test_email_notification.py` & `jobbergate_api-3.5.0a6/jobbergate_api/tests/test_email_notification.py`

 * *Files identical despite different names*

### Comparing `jobbergate_api-3.5.0a5/jobbergate_api/tests/test_meta_mapper.py` & `jobbergate_api-3.5.0a6/jobbergate_api/tests/test_meta_mapper.py`

 * *Files identical despite different names*

### Comparing `jobbergate_api-3.5.0a5/jobbergate_api/tests/test_pagination.py` & `jobbergate_api-3.5.0a6/jobbergate_api/tests/test_pagination.py`

 * *Files identical despite different names*

### Comparing `jobbergate_api-3.5.0a5/jobbergate_api/tests/test_s3_manager.py` & `jobbergate_api-3.5.0a6/jobbergate_api/tests/test_s3_manager.py`

 * *Files identical despite different names*

### Comparing `jobbergate_api-3.5.0a5/jobbergate_api/tests/test_security.py` & `jobbergate_api-3.5.0a6/jobbergate_api/tests/test_security.py`

 * *Files identical despite different names*

### Comparing `jobbergate_api-3.5.0a5/jobbergate_api/tests/test_storage.py` & `jobbergate_api-3.5.0a6/jobbergate_api/tests/test_storage.py`

 * *Files identical despite different names*

### Comparing `jobbergate_api-3.5.0a5/jobbergate_api/tests/test_version.py` & `jobbergate_api-3.5.0a6/jobbergate_api/tests/test_version.py`

 * *Files identical despite different names*

### Comparing `jobbergate_api-3.5.0a5/jobbergate_api/version.py` & `jobbergate_api-3.5.0a6/jobbergate_api/version.py`

 * *Files identical despite different names*

### Comparing `jobbergate_api-3.5.0a5/pyproject.toml` & `jobbergate_api-3.5.0a6/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "jobbergate-api"
-version = "3.5.0a5"
+version = "3.5.0a6"
 description = "Jobbergate API"
 authors = ["Omnivector Solutions <info@omnivector.solutions>"]
 license = "MIT"
 readme = "README.rst"
 repository = "https://github.com/omnivector-solutions/jobbergate"
 classifiers = [
     "License :: OSI Approved :: MIT License",
```

### Comparing `jobbergate_api-3.5.0a5/PKG-INFO` & `jobbergate_api-3.5.0a6/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: jobbergate-api
-Version: 3.5.0a5
+Version: 3.5.0a6
 Summary: Jobbergate API
 Home-page: https://github.com/omnivector-solutions/jobbergate
 License: MIT
 Author: Omnivector Solutions
 Author-email: info@omnivector.solutions
 Requires-Python: >=3.8,<4.0
 Classifier: Development Status :: 5 - Production/Stable
```

