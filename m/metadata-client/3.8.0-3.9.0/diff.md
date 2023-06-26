# Comparing `tmp/metadata_client-3.8.0.tar.gz` & `tmp/metadata_client-3.9.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "metadata_client-3.8.0.tar", last modified: Fri May 13 14:41:40 2022, max compression
+gzip compressed data, was "metadata_client-3.9.0.tar", last modified: Fri Jul  1 10:12:12 2022, max compression
```

## Comparing `metadata_client-3.8.0.tar` & `metadata_client-3.9.0.tar`

### file list

```diff
@@ -1,113 +1,113 @@
-drwxr-xr-x   0 maial      (501) staff       (20)        0 2022-05-13 14:41:40.437237 metadata_client-3.8.0/
--rw-r--r--   0 maial      (501) staff       (20)       48 2021-12-14 20:32:26.000000 metadata_client-3.8.0/AUTHORS.rst
--rw-r--r--   0 maial      (501) staff       (20)     6011 2022-05-13 12:22:51.000000 metadata_client-3.8.0/HISTORY.rst
--rw-r--r--   0 maial      (501) staff       (20)      779 2021-12-14 20:32:26.000000 metadata_client-3.8.0/LICENSE
--rw-r--r--   0 maial      (501) staff       (20)       89 2021-12-14 20:32:26.000000 metadata_client-3.8.0/MANIFEST.in
--rw-r--r--   0 maial      (501) staff       (20)    15044 2022-05-13 14:41:40.436840 metadata_client-3.8.0/PKG-INFO
--rw-r--r--   0 maial      (501) staff       (20)    13987 2022-05-13 12:22:51.000000 metadata_client-3.8.0/README.rst
-drwxr-xr-x   0 maial      (501) staff       (20)        0 2022-05-13 14:41:40.388136 metadata_client-3.8.0/metadata_client/
--rw-r--r--   0 maial      (501) staff       (20)      216 2022-05-13 12:22:51.000000 metadata_client-3.8.0/metadata_client/__init__.py
-drwxr-xr-x   0 maial      (501) staff       (20)        0 2022-05-13 14:41:40.401794 metadata_client-3.8.0/metadata_client/apis/
--rw-r--r--   0 maial      (501) staff       (20)      833 2021-12-14 20:30:26.000000 metadata_client-3.8.0/metadata_client/apis/__init__.py
--rw-r--r--   0 maial      (501) staff       (20)     1791 2022-05-05 17:15:05.000000 metadata_client-3.8.0/metadata_client/apis/dark_run_api.py
--rw-r--r--   0 maial      (501) staff       (20)     1683 2022-05-05 17:15:05.000000 metadata_client-3.8.0/metadata_client/apis/data_file_api.py
--rw-r--r--   0 maial      (501) staff       (20)     1767 2022-05-05 17:15:05.000000 metadata_client-3.8.0/metadata_client/apis/data_group_api.py
--rw-r--r--   0 maial      (501) staff       (20)     2041 2022-05-05 17:15:05.000000 metadata_client-3.8.0/metadata_client/apis/data_group_repository_api.py
--rw-r--r--   0 maial      (501) staff       (20)     1740 2022-05-05 17:15:05.000000 metadata_client-3.8.0/metadata_client/apis/data_group_type_api.py
--rw-r--r--   0 maial      (501) staff       (20)      473 2022-05-05 17:15:05.000000 metadata_client-3.8.0/metadata_client/apis/data_source_group_api.py
--rw-r--r--   0 maial      (501) staff       (20)      848 2022-05-05 17:15:05.000000 metadata_client-3.8.0/metadata_client/apis/data_source_group_version_api.py
--rw-r--r--   0 maial      (501) staff       (20)     1293 2022-05-05 17:15:05.000000 metadata_client-3.8.0/metadata_client/apis/data_type_api.py
--rw-r--r--   0 maial      (501) staff       (20)     1773 2022-05-05 17:15:05.000000 metadata_client-3.8.0/metadata_client/apis/experiment_api.py
--rw-r--r--   0 maial      (501) staff       (20)     1452 2022-05-05 17:15:05.000000 metadata_client-3.8.0/metadata_client/apis/experiment_type_api.py
--rw-r--r--   0 maial      (501) staff       (20)     2241 2022-05-05 17:15:05.000000 metadata_client-3.8.0/metadata_client/apis/instrument_api.py
--rw-r--r--   0 maial      (501) staff       (20)     1772 2022-05-05 17:15:05.000000 metadata_client-3.8.0/metadata_client/apis/parameter_api.py
--rw-r--r--   0 maial      (501) staff       (20)     1432 2022-05-05 17:15:05.000000 metadata_client-3.8.0/metadata_client/apis/parameter_type_api.py
--rw-r--r--   0 maial      (501) staff       (20)     2241 2022-05-05 17:15:05.000000 metadata_client-3.8.0/metadata_client/apis/proposal_api.py
--rw-r--r--   0 maial      (501) staff       (20)     1536 2022-05-05 17:15:05.000000 metadata_client-3.8.0/metadata_client/apis/repostory_api.py
--rwxr-xr-x   0 maial      (501) staff       (20)     2345 2022-05-05 17:15:05.000000 metadata_client-3.8.0/metadata_client/apis/run_api.py
--rw-r--r--   0 maial      (501) staff       (20)     1742 2022-05-05 17:15:05.000000 metadata_client-3.8.0/metadata_client/apis/sample_api.py
--rw-r--r--   0 maial      (501) staff       (20)      615 2022-05-05 17:15:05.000000 metadata_client-3.8.0/metadata_client/apis/user_api.py
-drwxr-xr-x   0 maial      (501) staff       (20)        0 2022-05-13 14:41:40.403934 metadata_client-3.8.0/metadata_client/common/
--rw-r--r--   0 maial      (501) staff       (20)       46 2021-12-14 20:30:57.000000 metadata_client-3.8.0/metadata_client/common/__init__.py
--rw-r--r--   0 maial      (501) staff       (20)     9438 2022-05-13 12:22:51.000000 metadata_client-3.8.0/metadata_client/common/base.py
--rw-r--r--   0 maial      (501) staff       (20)     3413 2022-05-05 17:15:05.000000 metadata_client-3.8.0/metadata_client/common/config.py
--rw-r--r--   0 maial      (501) staff       (20)     1136 2021-12-14 20:30:57.000000 metadata_client-3.8.0/metadata_client/common/util.py
--rw-r--r--   0 maial      (501) staff       (20)    31396 2022-05-05 17:15:05.000000 metadata_client-3.8.0/metadata_client/metadata_client.py
--rw-r--r--   0 maial      (501) staff       (20)      353 2021-12-14 20:32:42.000000 metadata_client-3.8.0/metadata_client/metadata_client_api.py
-drwxr-xr-x   0 maial      (501) staff       (20)        0 2022-05-13 14:41:40.412762 metadata_client-3.8.0/metadata_client/modules/
--rw-r--r--   0 maial      (501) staff       (20)      708 2021-12-14 20:30:50.000000 metadata_client-3.8.0/metadata_client/modules/__init__.py
--rw-r--r--   0 maial      (501) staff       (20)     4831 2022-05-05 17:15:05.000000 metadata_client-3.8.0/metadata_client/modules/dark_run.py
--rw-r--r--   0 maial      (501) staff       (20)     3506 2022-05-05 17:15:05.000000 metadata_client-3.8.0/metadata_client/modules/data_file.py
--rw-r--r--   0 maial      (501) staff       (20)     5680 2022-05-05 17:15:05.000000 metadata_client-3.8.0/metadata_client/modules/data_group.py
--rw-r--r--   0 maial      (501) staff       (20)     4927 2022-05-05 17:15:05.000000 metadata_client-3.8.0/metadata_client/modules/data_group_repository.py
--rw-r--r--   0 maial      (501) staff       (20)     3292 2022-05-05 17:15:05.000000 metadata_client-3.8.0/metadata_client/modules/data_group_type.py
--rw-r--r--   0 maial      (501) staff       (20)      771 2021-12-14 20:30:50.000000 metadata_client-3.8.0/metadata_client/modules/data_source_group.py
--rw-r--r--   0 maial      (501) staff       (20)     1225 2021-12-14 20:30:50.000000 metadata_client-3.8.0/metadata_client/modules/data_source_group_version.py
--rw-r--r--   0 maial      (501) staff       (20)     2849 2022-05-05 17:15:05.000000 metadata_client-3.8.0/metadata_client/modules/data_type.py
--rw-r--r--   0 maial      (501) staff       (20)     4038 2022-05-05 17:15:05.000000 metadata_client-3.8.0/metadata_client/modules/experiment.py
--rw-r--r--   0 maial      (501) staff       (20)     2933 2022-05-05 17:15:05.000000 metadata_client-3.8.0/metadata_client/modules/experiment_type.py
--rw-r--r--   0 maial      (501) staff       (20)     3396 2022-05-05 17:15:05.000000 metadata_client-3.8.0/metadata_client/modules/instrument.py
--rw-r--r--   0 maial      (501) staff       (20)     5303 2022-05-05 17:15:05.000000 metadata_client-3.8.0/metadata_client/modules/parameter.py
--rw-r--r--   0 maial      (501) staff       (20)     2919 2022-05-05 17:15:05.000000 metadata_client-3.8.0/metadata_client/modules/parameter_type.py
--rw-r--r--   0 maial      (501) staff       (20)     6792 2022-05-05 17:15:05.000000 metadata_client-3.8.0/metadata_client/modules/proposal.py
--rw-r--r--   0 maial      (501) staff       (20)     3874 2022-05-05 17:15:05.000000 metadata_client-3.8.0/metadata_client/modules/repository.py
--rw-r--r--   0 maial      (501) staff       (20)     6406 2022-05-05 17:15:05.000000 metadata_client-3.8.0/metadata_client/modules/run.py
--rw-r--r--   0 maial      (501) staff       (20)     5091 2022-05-05 17:15:05.000000 metadata_client-3.8.0/metadata_client/modules/sample.py
--rw-r--r--   0 maial      (501) staff       (20)     1082 2021-12-14 20:31:10.000000 metadata_client-3.8.0/metadata_client/modules/user.py
-drwxr-xr-x   0 maial      (501) staff       (20)        0 2022-05-13 14:41:40.414708 metadata_client-3.8.0/metadata_client/tests/
--rw-r--r--   0 maial      (501) staff       (20)       85 2021-12-14 20:32:12.000000 metadata_client-3.8.0/metadata_client/tests/__init__.py
-drwxr-xr-x   0 maial      (501) staff       (20)        0 2022-05-13 14:41:40.423271 metadata_client-3.8.0/metadata_client/tests/apis/
--rw-r--r--   0 maial      (501) staff       (20)       85 2021-12-14 20:31:39.000000 metadata_client-3.8.0/metadata_client/tests/apis/__init__.py
--rw-r--r--   0 maial      (501) staff       (20)     1893 2021-12-14 20:31:39.000000 metadata_client-3.8.0/metadata_client/tests/apis/api_base.py
--rw-r--r--   0 maial      (501) staff       (20)     4239 2021-12-14 20:31:39.000000 metadata_client-3.8.0/metadata_client/tests/apis/dark_run_api_test.py
--rw-r--r--   0 maial      (501) staff       (20)     5169 2021-12-14 20:31:39.000000 metadata_client-3.8.0/metadata_client/tests/apis/data_file_api_test.py
--rw-r--r--   0 maial      (501) staff       (20)     8048 2021-12-14 20:31:39.000000 metadata_client-3.8.0/metadata_client/tests/apis/data_group_api_test.py
--rw-r--r--   0 maial      (501) staff       (20)     6309 2021-12-14 20:31:39.000000 metadata_client-3.8.0/metadata_client/tests/apis/data_group_repository_api_test.py
--rw-r--r--   0 maial      (501) staff       (20)     5488 2021-12-14 20:31:39.000000 metadata_client-3.8.0/metadata_client/tests/apis/data_group_type_api_test.py
--rw-r--r--   0 maial      (501) staff       (20)     5329 2021-12-14 20:31:39.000000 metadata_client-3.8.0/metadata_client/tests/apis/data_type_api_test.py
--rw-r--r--   0 maial      (501) staff       (20)     6791 2021-12-14 20:31:39.000000 metadata_client-3.8.0/metadata_client/tests/apis/experiment_api_test.py
--rw-r--r--   0 maial      (501) staff       (20)     5491 2021-12-14 20:31:39.000000 metadata_client-3.8.0/metadata_client/tests/apis/experiment_type_api_test.py
--rw-r--r--   0 maial      (501) staff       (20)     3730 2021-12-14 20:31:39.000000 metadata_client-3.8.0/metadata_client/tests/apis/instrument_api_test.py
--rw-r--r--   0 maial      (501) staff       (20)     6759 2021-12-14 20:31:39.000000 metadata_client-3.8.0/metadata_client/tests/apis/parameter_api_test.py
--rw-r--r--   0 maial      (501) staff       (20)     5464 2021-12-14 20:31:39.000000 metadata_client-3.8.0/metadata_client/tests/apis/parameter_type_api_test.py
--rw-r--r--   0 maial      (501) staff       (20)    14173 2022-05-05 17:15:05.000000 metadata_client-3.8.0/metadata_client/tests/apis/proposal_api_test.py
--rw-r--r--   0 maial      (501) staff       (20)     6879 2021-12-14 20:31:39.000000 metadata_client-3.8.0/metadata_client/tests/apis/repository_api_test.py
--rw-r--r--   0 maial      (501) staff       (20)     8955 2022-05-05 17:15:05.000000 metadata_client-3.8.0/metadata_client/tests/apis/run_api_test.py
--rw-r--r--   0 maial      (501) staff       (20)     6919 2022-05-05 17:15:05.000000 metadata_client-3.8.0/metadata_client/tests/apis/sample_api_test.py
--rw-r--r--   0 maial      (501) staff       (20)     2002 2021-12-14 20:31:39.000000 metadata_client-3.8.0/metadata_client/tests/apis/user_api_test.py
-drwxr-xr-x   0 maial      (501) staff       (20)        0 2022-05-13 14:41:40.427676 metadata_client-3.8.0/metadata_client/tests/common/
--rw-r--r--   0 maial      (501) staff       (20)       85 2021-12-14 20:31:33.000000 metadata_client-3.8.0/metadata_client/tests/common/__init__.py
--rw-r--r--   0 maial      (501) staff       (20)     4432 2022-05-13 12:22:51.000000 metadata_client-3.8.0/metadata_client/tests/common/base_test.py
--rw-r--r--   0 maial      (501) staff       (20)     3353 2022-05-05 17:15:06.000000 metadata_client-3.8.0/metadata_client/tests/common/config_test.py
--rw-r--r--   0 maial      (501) staff       (20)     2117 2021-12-14 20:31:33.000000 metadata_client-3.8.0/metadata_client/tests/common/generators.py
--rwxr-xr-x   0 maial      (501) staff       (20)     2824 2022-05-05 17:15:10.000000 metadata_client-3.8.0/metadata_client/tests/common/secrets.py
--rw-r--r--   0 maial      (501) staff       (20)     5003 2021-12-14 20:31:50.000000 metadata_client-3.8.0/metadata_client/tests/common/util.py
--rw-r--r--   0 maial      (501) staff       (20)     1813 2021-12-14 20:31:50.000000 metadata_client-3.8.0/metadata_client/tests/common/util_datetime.py
--rw-r--r--   0 maial      (501) staff       (20)     2373 2021-12-14 20:31:50.000000 metadata_client-3.8.0/metadata_client/tests/common/util_test.py
--rw-r--r--   0 maial      (501) staff       (20)     1579 2022-05-05 17:15:06.000000 metadata_client-3.8.0/metadata_client/tests/metadata_client_connection_test.py
--rw-r--r--   0 maial      (501) staff       (20)    56026 2022-05-05 17:15:06.000000 metadata_client-3.8.0/metadata_client/tests/metadata_client_test.py
-drwxr-xr-x   0 maial      (501) staff       (20)        0 2022-05-13 14:41:40.436022 metadata_client-3.8.0/metadata_client/tests/modules/
--rw-r--r--   0 maial      (501) staff       (20)       85 2021-12-14 20:32:03.000000 metadata_client-3.8.0/metadata_client/tests/modules/__init__.py
--rw-r--r--   0 maial      (501) staff       (20)     8729 2022-05-05 17:15:06.000000 metadata_client-3.8.0/metadata_client/tests/modules/dark_run_test.py
--rw-r--r--   0 maial      (501) staff       (20)     6105 2022-05-05 17:15:06.000000 metadata_client-3.8.0/metadata_client/tests/modules/data_file_test.py
--rw-r--r--   0 maial      (501) staff       (20)     5156 2022-05-05 17:15:06.000000 metadata_client-3.8.0/metadata_client/tests/modules/data_group_repository_test.py
--rw-r--r--   0 maial      (501) staff       (20)    11675 2022-05-05 17:15:06.000000 metadata_client-3.8.0/metadata_client/tests/modules/data_group_test.py
--rw-r--r--   0 maial      (501) staff       (20)     6370 2022-05-05 17:15:06.000000 metadata_client-3.8.0/metadata_client/tests/modules/data_group_type_test.py
--rw-r--r--   0 maial      (501) staff       (20)     4973 2021-12-14 20:32:03.000000 metadata_client-3.8.0/metadata_client/tests/modules/data_type_test.py
--rw-r--r--   0 maial      (501) staff       (20)     7136 2021-12-14 20:32:03.000000 metadata_client-3.8.0/metadata_client/tests/modules/experiment_test.py
--rw-r--r--   0 maial      (501) staff       (20)     5078 2021-12-14 20:32:03.000000 metadata_client-3.8.0/metadata_client/tests/modules/experiment_type_test.py
--rw-r--r--   0 maial      (501) staff       (20)     4607 2021-12-14 20:32:03.000000 metadata_client-3.8.0/metadata_client/tests/modules/module_base.py
--rw-r--r--   0 maial      (501) staff       (20)     9271 2022-05-05 17:15:06.000000 metadata_client-3.8.0/metadata_client/tests/modules/parameter_test.py
--rw-r--r--   0 maial      (501) staff       (20)     5059 2021-12-14 20:32:03.000000 metadata_client-3.8.0/metadata_client/tests/modules/parameter_type_test.py
--rw-r--r--   0 maial      (501) staff       (20)    14605 2022-05-03 12:44:12.000000 metadata_client-3.8.0/metadata_client/tests/modules/proposal_test.py
--rw-r--r--   0 maial      (501) staff       (20)     6643 2021-12-14 20:32:03.000000 metadata_client-3.8.0/metadata_client/tests/modules/repository_test.py
--rw-r--r--   0 maial      (501) staff       (20)    10473 2021-12-14 20:32:03.000000 metadata_client-3.8.0/metadata_client/tests/modules/run_test.py
--rw-r--r--   0 maial      (501) staff       (20)     8838 2022-05-05 17:15:06.000000 metadata_client-3.8.0/metadata_client/tests/modules/sample_test.py
-drwxr-xr-x   0 maial      (501) staff       (20)        0 2022-05-13 14:41:40.390354 metadata_client-3.8.0/metadata_client.egg-info/
--rw-r--r--   0 maial      (501) staff       (20)    15044 2022-05-13 14:41:39.000000 metadata_client-3.8.0/metadata_client.egg-info/PKG-INFO
--rw-r--r--   0 maial      (501) staff       (20)     4120 2022-05-13 14:41:39.000000 metadata_client-3.8.0/metadata_client.egg-info/SOURCES.txt
--rw-r--r--   0 maial      (501) staff       (20)        1 2022-05-13 14:41:39.000000 metadata_client-3.8.0/metadata_client.egg-info/dependency_links.txt
--rw-r--r--   0 maial      (501) staff       (20)      124 2022-05-13 14:41:39.000000 metadata_client-3.8.0/metadata_client.egg-info/requires.txt
--rw-r--r--   0 maial      (501) staff       (20)       16 2022-05-13 14:41:39.000000 metadata_client-3.8.0/metadata_client.egg-info/top_level.txt
--rw-r--r--   0 maial      (501) staff       (20)       38 2022-05-13 14:41:40.437331 metadata_client-3.8.0/setup.cfg
--rw-r--r--   0 maial      (501) staff       (20)     2313 2022-05-05 17:15:06.000000 metadata_client-3.8.0/setup.py
+drwxr-xr-x   0 maial      (501) staff       (20)        0 2022-07-01 10:12:12.961401 metadata_client-3.9.0/
+-rw-r--r--   0 maial      (501) staff       (20)       48 2021-12-14 20:32:26.000000 metadata_client-3.9.0/AUTHORS.rst
+-rw-r--r--   0 maial      (501) staff       (20)     6238 2022-06-24 11:54:57.000000 metadata_client-3.9.0/HISTORY.rst
+-rw-r--r--   0 maial      (501) staff       (20)      779 2021-12-14 20:32:26.000000 metadata_client-3.9.0/LICENSE
+-rw-r--r--   0 maial      (501) staff       (20)       89 2021-12-14 20:32:26.000000 metadata_client-3.9.0/MANIFEST.in
+-rw-r--r--   0 maial      (501) staff       (20)    15042 2022-07-01 10:12:12.961017 metadata_client-3.9.0/PKG-INFO
+-rw-r--r--   0 maial      (501) staff       (20)    13987 2022-06-24 11:54:57.000000 metadata_client-3.9.0/README.rst
+drwxr-xr-x   0 maial      (501) staff       (20)        0 2022-07-01 10:12:12.891679 metadata_client-3.9.0/metadata_client/
+-rw-r--r--   0 maial      (501) staff       (20)      216 2022-06-24 11:54:57.000000 metadata_client-3.9.0/metadata_client/__init__.py
+drwxr-xr-x   0 maial      (501) staff       (20)        0 2022-07-01 10:12:12.908379 metadata_client-3.9.0/metadata_client/apis/
+-rw-r--r--   0 maial      (501) staff       (20)      833 2021-12-14 20:30:26.000000 metadata_client-3.9.0/metadata_client/apis/__init__.py
+-rw-r--r--   0 maial      (501) staff       (20)     1791 2022-05-05 17:15:05.000000 metadata_client-3.9.0/metadata_client/apis/dark_run_api.py
+-rw-r--r--   0 maial      (501) staff       (20)     1683 2022-05-05 17:15:05.000000 metadata_client-3.9.0/metadata_client/apis/data_file_api.py
+-rw-r--r--   0 maial      (501) staff       (20)     1767 2022-05-05 17:15:05.000000 metadata_client-3.9.0/metadata_client/apis/data_group_api.py
+-rw-r--r--   0 maial      (501) staff       (20)     2041 2022-05-05 17:15:05.000000 metadata_client-3.9.0/metadata_client/apis/data_group_repository_api.py
+-rw-r--r--   0 maial      (501) staff       (20)     1740 2022-05-05 17:15:05.000000 metadata_client-3.9.0/metadata_client/apis/data_group_type_api.py
+-rw-r--r--   0 maial      (501) staff       (20)      473 2022-05-05 17:15:05.000000 metadata_client-3.9.0/metadata_client/apis/data_source_group_api.py
+-rw-r--r--   0 maial      (501) staff       (20)      848 2022-05-05 17:15:05.000000 metadata_client-3.9.0/metadata_client/apis/data_source_group_version_api.py
+-rw-r--r--   0 maial      (501) staff       (20)     1293 2022-05-05 17:15:05.000000 metadata_client-3.9.0/metadata_client/apis/data_type_api.py
+-rw-r--r--   0 maial      (501) staff       (20)     1773 2022-05-05 17:15:05.000000 metadata_client-3.9.0/metadata_client/apis/experiment_api.py
+-rw-r--r--   0 maial      (501) staff       (20)     1452 2022-05-05 17:15:05.000000 metadata_client-3.9.0/metadata_client/apis/experiment_type_api.py
+-rw-r--r--   0 maial      (501) staff       (20)     2241 2022-05-05 17:15:05.000000 metadata_client-3.9.0/metadata_client/apis/instrument_api.py
+-rw-r--r--   0 maial      (501) staff       (20)     1772 2022-05-05 17:15:05.000000 metadata_client-3.9.0/metadata_client/apis/parameter_api.py
+-rw-r--r--   0 maial      (501) staff       (20)     1432 2022-05-05 17:15:05.000000 metadata_client-3.9.0/metadata_client/apis/parameter_type_api.py
+-rw-r--r--   0 maial      (501) staff       (20)     2241 2022-05-05 17:15:05.000000 metadata_client-3.9.0/metadata_client/apis/proposal_api.py
+-rw-r--r--   0 maial      (501) staff       (20)     1536 2022-05-05 17:15:05.000000 metadata_client-3.9.0/metadata_client/apis/repostory_api.py
+-rwxr-xr-x   0 maial      (501) staff       (20)     2345 2022-05-05 17:15:05.000000 metadata_client-3.9.0/metadata_client/apis/run_api.py
+-rw-r--r--   0 maial      (501) staff       (20)     1742 2022-05-05 17:15:05.000000 metadata_client-3.9.0/metadata_client/apis/sample_api.py
+-rw-r--r--   0 maial      (501) staff       (20)      615 2022-05-05 17:15:05.000000 metadata_client-3.9.0/metadata_client/apis/user_api.py
+drwxr-xr-x   0 maial      (501) staff       (20)        0 2022-07-01 10:12:12.911533 metadata_client-3.9.0/metadata_client/common/
+-rw-r--r--   0 maial      (501) staff       (20)       46 2021-12-14 20:30:57.000000 metadata_client-3.9.0/metadata_client/common/__init__.py
+-rw-r--r--   0 maial      (501) staff       (20)     9438 2022-05-13 12:22:51.000000 metadata_client-3.9.0/metadata_client/common/base.py
+-rw-r--r--   0 maial      (501) staff       (20)     3413 2022-05-05 17:15:05.000000 metadata_client-3.9.0/metadata_client/common/config.py
+-rw-r--r--   0 maial      (501) staff       (20)     1136 2021-12-14 20:30:57.000000 metadata_client-3.9.0/metadata_client/common/util.py
+-rw-r--r--   0 maial      (501) staff       (20)    31396 2022-05-05 17:15:05.000000 metadata_client-3.9.0/metadata_client/metadata_client.py
+-rw-r--r--   0 maial      (501) staff       (20)      353 2021-12-14 20:32:42.000000 metadata_client-3.9.0/metadata_client/metadata_client_api.py
+drwxr-xr-x   0 maial      (501) staff       (20)        0 2022-07-01 10:12:12.927359 metadata_client-3.9.0/metadata_client/modules/
+-rw-r--r--   0 maial      (501) staff       (20)      708 2021-12-14 20:30:50.000000 metadata_client-3.9.0/metadata_client/modules/__init__.py
+-rw-r--r--   0 maial      (501) staff       (20)     4831 2022-05-05 17:15:05.000000 metadata_client-3.9.0/metadata_client/modules/dark_run.py
+-rw-r--r--   0 maial      (501) staff       (20)     3506 2022-05-05 17:15:05.000000 metadata_client-3.9.0/metadata_client/modules/data_file.py
+-rw-r--r--   0 maial      (501) staff       (20)     5680 2022-05-05 17:15:05.000000 metadata_client-3.9.0/metadata_client/modules/data_group.py
+-rw-r--r--   0 maial      (501) staff       (20)     4927 2022-05-05 17:15:05.000000 metadata_client-3.9.0/metadata_client/modules/data_group_repository.py
+-rw-r--r--   0 maial      (501) staff       (20)     3292 2022-05-05 17:15:05.000000 metadata_client-3.9.0/metadata_client/modules/data_group_type.py
+-rw-r--r--   0 maial      (501) staff       (20)      771 2021-12-14 20:30:50.000000 metadata_client-3.9.0/metadata_client/modules/data_source_group.py
+-rw-r--r--   0 maial      (501) staff       (20)     1225 2021-12-14 20:30:50.000000 metadata_client-3.9.0/metadata_client/modules/data_source_group_version.py
+-rw-r--r--   0 maial      (501) staff       (20)     2849 2022-05-05 17:15:05.000000 metadata_client-3.9.0/metadata_client/modules/data_type.py
+-rw-r--r--   0 maial      (501) staff       (20)     4038 2022-05-05 17:15:05.000000 metadata_client-3.9.0/metadata_client/modules/experiment.py
+-rw-r--r--   0 maial      (501) staff       (20)     2933 2022-05-05 17:15:05.000000 metadata_client-3.9.0/metadata_client/modules/experiment_type.py
+-rw-r--r--   0 maial      (501) staff       (20)     3396 2022-05-05 17:15:05.000000 metadata_client-3.9.0/metadata_client/modules/instrument.py
+-rw-r--r--   0 maial      (501) staff       (20)     5303 2022-05-05 17:15:05.000000 metadata_client-3.9.0/metadata_client/modules/parameter.py
+-rw-r--r--   0 maial      (501) staff       (20)     2919 2022-05-05 17:15:05.000000 metadata_client-3.9.0/metadata_client/modules/parameter_type.py
+-rw-r--r--   0 maial      (501) staff       (20)     6792 2022-05-05 17:15:05.000000 metadata_client-3.9.0/metadata_client/modules/proposal.py
+-rw-r--r--   0 maial      (501) staff       (20)     3874 2022-05-05 17:15:05.000000 metadata_client-3.9.0/metadata_client/modules/repository.py
+-rw-r--r--   0 maial      (501) staff       (20)     6406 2022-05-05 17:15:05.000000 metadata_client-3.9.0/metadata_client/modules/run.py
+-rw-r--r--   0 maial      (501) staff       (20)     5091 2022-05-05 17:15:05.000000 metadata_client-3.9.0/metadata_client/modules/sample.py
+-rw-r--r--   0 maial      (501) staff       (20)     1082 2021-12-14 20:31:10.000000 metadata_client-3.9.0/metadata_client/modules/user.py
+drwxr-xr-x   0 maial      (501) staff       (20)        0 2022-07-01 10:12:12.929621 metadata_client-3.9.0/metadata_client/tests/
+-rw-r--r--   0 maial      (501) staff       (20)       85 2021-12-14 20:32:12.000000 metadata_client-3.9.0/metadata_client/tests/__init__.py
+drwxr-xr-x   0 maial      (501) staff       (20)        0 2022-07-01 10:12:12.942142 metadata_client-3.9.0/metadata_client/tests/apis/
+-rw-r--r--   0 maial      (501) staff       (20)       85 2021-12-14 20:31:39.000000 metadata_client-3.9.0/metadata_client/tests/apis/__init__.py
+-rw-r--r--   0 maial      (501) staff       (20)     1893 2021-12-14 20:31:39.000000 metadata_client-3.9.0/metadata_client/tests/apis/api_base.py
+-rw-r--r--   0 maial      (501) staff       (20)     4239 2021-12-14 20:31:39.000000 metadata_client-3.9.0/metadata_client/tests/apis/dark_run_api_test.py
+-rw-r--r--   0 maial      (501) staff       (20)     5169 2021-12-14 20:31:39.000000 metadata_client-3.9.0/metadata_client/tests/apis/data_file_api_test.py
+-rw-r--r--   0 maial      (501) staff       (20)     8048 2021-12-14 20:31:39.000000 metadata_client-3.9.0/metadata_client/tests/apis/data_group_api_test.py
+-rw-r--r--   0 maial      (501) staff       (20)     6309 2021-12-14 20:31:39.000000 metadata_client-3.9.0/metadata_client/tests/apis/data_group_repository_api_test.py
+-rw-r--r--   0 maial      (501) staff       (20)     5488 2021-12-14 20:31:39.000000 metadata_client-3.9.0/metadata_client/tests/apis/data_group_type_api_test.py
+-rw-r--r--   0 maial      (501) staff       (20)     5329 2021-12-14 20:31:39.000000 metadata_client-3.9.0/metadata_client/tests/apis/data_type_api_test.py
+-rw-r--r--   0 maial      (501) staff       (20)     6791 2021-12-14 20:31:39.000000 metadata_client-3.9.0/metadata_client/tests/apis/experiment_api_test.py
+-rw-r--r--   0 maial      (501) staff       (20)     5491 2021-12-14 20:31:39.000000 metadata_client-3.9.0/metadata_client/tests/apis/experiment_type_api_test.py
+-rw-r--r--   0 maial      (501) staff       (20)     3730 2021-12-14 20:31:39.000000 metadata_client-3.9.0/metadata_client/tests/apis/instrument_api_test.py
+-rw-r--r--   0 maial      (501) staff       (20)     6759 2021-12-14 20:31:39.000000 metadata_client-3.9.0/metadata_client/tests/apis/parameter_api_test.py
+-rw-r--r--   0 maial      (501) staff       (20)     5464 2021-12-14 20:31:39.000000 metadata_client-3.9.0/metadata_client/tests/apis/parameter_type_api_test.py
+-rw-r--r--   0 maial      (501) staff       (20)    14173 2022-05-05 17:15:05.000000 metadata_client-3.9.0/metadata_client/tests/apis/proposal_api_test.py
+-rw-r--r--   0 maial      (501) staff       (20)     6879 2021-12-14 20:31:39.000000 metadata_client-3.9.0/metadata_client/tests/apis/repository_api_test.py
+-rw-r--r--   0 maial      (501) staff       (20)     8955 2022-05-05 17:15:05.000000 metadata_client-3.9.0/metadata_client/tests/apis/run_api_test.py
+-rw-r--r--   0 maial      (501) staff       (20)     6919 2022-05-05 17:15:05.000000 metadata_client-3.9.0/metadata_client/tests/apis/sample_api_test.py
+-rw-r--r--   0 maial      (501) staff       (20)     2002 2021-12-14 20:31:39.000000 metadata_client-3.9.0/metadata_client/tests/apis/user_api_test.py
+drwxr-xr-x   0 maial      (501) staff       (20)        0 2022-07-01 10:12:12.948017 metadata_client-3.9.0/metadata_client/tests/common/
+-rw-r--r--   0 maial      (501) staff       (20)       85 2021-12-14 20:31:33.000000 metadata_client-3.9.0/metadata_client/tests/common/__init__.py
+-rw-r--r--   0 maial      (501) staff       (20)     4432 2022-05-13 12:22:51.000000 metadata_client-3.9.0/metadata_client/tests/common/base_test.py
+-rw-r--r--   0 maial      (501) staff       (20)     3353 2022-05-05 17:15:06.000000 metadata_client-3.9.0/metadata_client/tests/common/config_test.py
+-rw-r--r--   0 maial      (501) staff       (20)     2117 2021-12-14 20:31:33.000000 metadata_client-3.9.0/metadata_client/tests/common/generators.py
+-rwxr-xr-x   0 maial      (501) staff       (20)     2824 2022-05-05 17:15:10.000000 metadata_client-3.9.0/metadata_client/tests/common/secrets.py
+-rw-r--r--   0 maial      (501) staff       (20)     5003 2021-12-14 20:31:50.000000 metadata_client-3.9.0/metadata_client/tests/common/util.py
+-rw-r--r--   0 maial      (501) staff       (20)     1813 2021-12-14 20:31:50.000000 metadata_client-3.9.0/metadata_client/tests/common/util_datetime.py
+-rw-r--r--   0 maial      (501) staff       (20)     2373 2021-12-14 20:31:50.000000 metadata_client-3.9.0/metadata_client/tests/common/util_test.py
+-rw-r--r--   0 maial      (501) staff       (20)     1579 2022-05-05 17:15:06.000000 metadata_client-3.9.0/metadata_client/tests/metadata_client_connection_test.py
+-rw-r--r--   0 maial      (501) staff       (20)    56026 2022-05-05 17:15:06.000000 metadata_client-3.9.0/metadata_client/tests/metadata_client_test.py
+drwxr-xr-x   0 maial      (501) staff       (20)        0 2022-07-01 10:12:12.960413 metadata_client-3.9.0/metadata_client/tests/modules/
+-rw-r--r--   0 maial      (501) staff       (20)       85 2021-12-14 20:32:03.000000 metadata_client-3.9.0/metadata_client/tests/modules/__init__.py
+-rw-r--r--   0 maial      (501) staff       (20)     8729 2022-05-05 17:15:06.000000 metadata_client-3.9.0/metadata_client/tests/modules/dark_run_test.py
+-rw-r--r--   0 maial      (501) staff       (20)     6105 2022-05-05 17:15:06.000000 metadata_client-3.9.0/metadata_client/tests/modules/data_file_test.py
+-rw-r--r--   0 maial      (501) staff       (20)     5156 2022-05-05 17:15:06.000000 metadata_client-3.9.0/metadata_client/tests/modules/data_group_repository_test.py
+-rw-r--r--   0 maial      (501) staff       (20)    11675 2022-05-05 17:15:06.000000 metadata_client-3.9.0/metadata_client/tests/modules/data_group_test.py
+-rw-r--r--   0 maial      (501) staff       (20)     6370 2022-05-05 17:15:06.000000 metadata_client-3.9.0/metadata_client/tests/modules/data_group_type_test.py
+-rw-r--r--   0 maial      (501) staff       (20)     4973 2021-12-14 20:32:03.000000 metadata_client-3.9.0/metadata_client/tests/modules/data_type_test.py
+-rw-r--r--   0 maial      (501) staff       (20)     7136 2021-12-14 20:32:03.000000 metadata_client-3.9.0/metadata_client/tests/modules/experiment_test.py
+-rw-r--r--   0 maial      (501) staff       (20)     5078 2021-12-14 20:32:03.000000 metadata_client-3.9.0/metadata_client/tests/modules/experiment_type_test.py
+-rw-r--r--   0 maial      (501) staff       (20)     4607 2021-12-14 20:32:03.000000 metadata_client-3.9.0/metadata_client/tests/modules/module_base.py
+-rw-r--r--   0 maial      (501) staff       (20)     9271 2022-05-05 17:15:06.000000 metadata_client-3.9.0/metadata_client/tests/modules/parameter_test.py
+-rw-r--r--   0 maial      (501) staff       (20)     5059 2021-12-14 20:32:03.000000 metadata_client-3.9.0/metadata_client/tests/modules/parameter_type_test.py
+-rw-r--r--   0 maial      (501) staff       (20)    14605 2022-05-03 12:44:12.000000 metadata_client-3.9.0/metadata_client/tests/modules/proposal_test.py
+-rw-r--r--   0 maial      (501) staff       (20)     6643 2021-12-14 20:32:03.000000 metadata_client-3.9.0/metadata_client/tests/modules/repository_test.py
+-rw-r--r--   0 maial      (501) staff       (20)    10473 2021-12-14 20:32:03.000000 metadata_client-3.9.0/metadata_client/tests/modules/run_test.py
+-rw-r--r--   0 maial      (501) staff       (20)     8838 2022-05-05 17:15:06.000000 metadata_client-3.9.0/metadata_client/tests/modules/sample_test.py
+drwxr-xr-x   0 maial      (501) staff       (20)        0 2022-07-01 10:12:12.894713 metadata_client-3.9.0/metadata_client.egg-info/
+-rw-r--r--   0 maial      (501) staff       (20)    15042 2022-07-01 10:12:12.000000 metadata_client-3.9.0/metadata_client.egg-info/PKG-INFO
+-rw-r--r--   0 maial      (501) staff       (20)     4120 2022-07-01 10:12:12.000000 metadata_client-3.9.0/metadata_client.egg-info/SOURCES.txt
+-rw-r--r--   0 maial      (501) staff       (20)        1 2022-07-01 10:12:12.000000 metadata_client-3.9.0/metadata_client.egg-info/dependency_links.txt
+-rw-r--r--   0 maial      (501) staff       (20)      124 2022-07-01 10:12:12.000000 metadata_client-3.9.0/metadata_client.egg-info/requires.txt
+-rw-r--r--   0 maial      (501) staff       (20)       16 2022-07-01 10:12:12.000000 metadata_client-3.9.0/metadata_client.egg-info/top_level.txt
+-rw-r--r--   0 maial      (501) staff       (20)       38 2022-07-01 10:12:12.961503 metadata_client-3.9.0/setup.cfg
+-rw-r--r--   0 maial      (501) staff       (20)     2313 2022-06-24 11:54:57.000000 metadata_client-3.9.0/setup.py
```

### Comparing `metadata_client-3.8.0/HISTORY.rst` & `metadata_client-3.9.0/HISTORY.rst`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,16 @@
 History
 -------
 
+v3.9.0 (24 June 2022)
++++++++++++++++++++++
+- Update dependencies certifi and requests
+- Drop support for python 3.6 (latest requests tag dropped support to python 3.6)
+- Add CI tests to python latest (currently version 3.11)
+
 v3.8.0 (13 May 2022)
 ++++++++++++++++++++
 - Remove replace_expired_token method work-around since oauth2_xfel_client version 6.1+ should have it handled
 - Add pagination headers to the response object from metadata_client
 
 v3.7.0 (5 May 2022)
 +++++++++++++++++++
```

### Comparing `metadata_client-3.8.0/LICENSE` & `metadata_client-3.9.0/LICENSE`

 * *Files identical despite different names*

### Comparing `metadata_client-3.8.0/PKG-INFO` & `metadata_client-3.9.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: metadata_client
-Version: 3.8.0
+Version: 3.9.0
 Summary: Python Client for European XFEL Metadata Catalogue Web App available at https://in.xfel.eu/metadata
 Home-page: https://git.xfel.eu/gitlab/ITDM/metadata_client
 Author: Luís Maia
 Author-email: luis.maia@xfel.eu
 Maintainer: Luís Maia
 Maintainer-email: luis.maia@xfel.eu
 License: MIT
@@ -17,15 +17,15 @@
 Classifier: Natural Language :: English
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: OS Independent
 Classifier: Topic :: Scientific/Engineering :: Information Analysis
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
-Requires-Python: >=3.6
+Requires-Python: >=3.7
 Provides-Extra: test
 License-File: LICENSE
 License-File: AUTHORS.rst
 
 Metadata Catalogue Client
 =========================
 
@@ -89,15 +89,15 @@
     # Force re-installation of packages
     pip install --ignore-installed
 
  Installing it will place two folders under the current Python installation
  site-packages folder:
 
  - `metadata_client` with the sources;
- - `metadata_client-3.8.0.dist-info/` with Wheels configuration files.
+ - `metadata_client-3.9.0.dist-info/` with Wheels configuration files.
 
  To identify your Python site-packages folder run::
 
     python -c "from distutils.sysconfig import get_python_lib; print(get_python_lib())"
 
 
 Usage
@@ -371,9 +371,7 @@
     python setup.py bdist_wheel
 
     # Upload new version .egg and .whl files
     twine upload dist/*
 
     # In case a test is necessary, it is possible to test it against test.pypi.org
     twine upload --repository-url https://test.pypi.org/legacy/ dist/* --verbose
-
-
```

### Comparing `metadata_client-3.8.0/README.rst` & `metadata_client-3.9.0/README.rst`

 * *Files 0% similar despite different names*

```diff
@@ -61,15 +61,15 @@
     # Force re-installation of packages
     pip install --ignore-installed
 
  Installing it will place two folders under the current Python installation
  site-packages folder:
 
  - `metadata_client` with the sources;
- - `metadata_client-3.8.0.dist-info/` with Wheels configuration files.
+ - `metadata_client-3.9.0.dist-info/` with Wheels configuration files.
 
  To identify your Python site-packages folder run::
 
     python -c "from distutils.sysconfig import get_python_lib; print(get_python_lib())"
 
 
 Usage
```

### Comparing `metadata_client-3.8.0/metadata_client/apis/__init__.py` & `metadata_client-3.9.0/metadata_client/apis/__init__.py`

 * *Files identical despite different names*

### Comparing `metadata_client-3.8.0/metadata_client/apis/dark_run_api.py` & `metadata_client-3.9.0/metadata_client/apis/dark_run_api.py`

 * *Files identical despite different names*

### Comparing `metadata_client-3.8.0/metadata_client/apis/data_file_api.py` & `metadata_client-3.9.0/metadata_client/apis/data_file_api.py`

 * *Files identical despite different names*

### Comparing `metadata_client-3.8.0/metadata_client/apis/data_group_api.py` & `metadata_client-3.9.0/metadata_client/apis/data_group_api.py`

 * *Files identical despite different names*

### Comparing `metadata_client-3.8.0/metadata_client/apis/data_group_repository_api.py` & `metadata_client-3.9.0/metadata_client/apis/data_group_repository_api.py`

 * *Files identical despite different names*

### Comparing `metadata_client-3.8.0/metadata_client/apis/data_group_type_api.py` & `metadata_client-3.9.0/metadata_client/apis/data_group_type_api.py`

 * *Files identical despite different names*

### Comparing `metadata_client-3.8.0/metadata_client/apis/data_source_group_version_api.py` & `metadata_client-3.9.0/metadata_client/apis/data_source_group_version_api.py`

 * *Files identical despite different names*

### Comparing `metadata_client-3.8.0/metadata_client/apis/data_type_api.py` & `metadata_client-3.9.0/metadata_client/apis/data_type_api.py`

 * *Files identical despite different names*

### Comparing `metadata_client-3.8.0/metadata_client/apis/experiment_api.py` & `metadata_client-3.9.0/metadata_client/apis/experiment_api.py`

 * *Files identical despite different names*

### Comparing `metadata_client-3.8.0/metadata_client/apis/experiment_type_api.py` & `metadata_client-3.9.0/metadata_client/apis/experiment_type_api.py`

 * *Files identical despite different names*

### Comparing `metadata_client-3.8.0/metadata_client/apis/instrument_api.py` & `metadata_client-3.9.0/metadata_client/apis/instrument_api.py`

 * *Files identical despite different names*

### Comparing `metadata_client-3.8.0/metadata_client/apis/parameter_api.py` & `metadata_client-3.9.0/metadata_client/apis/parameter_api.py`

 * *Files identical despite different names*

### Comparing `metadata_client-3.8.0/metadata_client/apis/parameter_type_api.py` & `metadata_client-3.9.0/metadata_client/apis/parameter_type_api.py`

 * *Files identical despite different names*

### Comparing `metadata_client-3.8.0/metadata_client/apis/proposal_api.py` & `metadata_client-3.9.0/metadata_client/apis/proposal_api.py`

 * *Files identical despite different names*

### Comparing `metadata_client-3.8.0/metadata_client/apis/repostory_api.py` & `metadata_client-3.9.0/metadata_client/apis/repostory_api.py`

 * *Files identical despite different names*

### Comparing `metadata_client-3.8.0/metadata_client/apis/run_api.py` & `metadata_client-3.9.0/metadata_client/apis/run_api.py`

 * *Files identical despite different names*

### Comparing `metadata_client-3.8.0/metadata_client/apis/sample_api.py` & `metadata_client-3.9.0/metadata_client/apis/sample_api.py`

 * *Files identical despite different names*

### Comparing `metadata_client-3.8.0/metadata_client/apis/user_api.py` & `metadata_client-3.9.0/metadata_client/apis/user_api.py`

 * *Files identical despite different names*

### Comparing `metadata_client-3.8.0/metadata_client/common/base.py` & `metadata_client-3.9.0/metadata_client/common/base.py`

 * *Files identical despite different names*

### Comparing `metadata_client-3.8.0/metadata_client/common/config.py` & `metadata_client-3.9.0/metadata_client/common/config.py`

 * *Files identical despite different names*

### Comparing `metadata_client-3.8.0/metadata_client/common/util.py` & `metadata_client-3.9.0/metadata_client/common/util.py`

 * *Files identical despite different names*

### Comparing `metadata_client-3.8.0/metadata_client/metadata_client.py` & `metadata_client-3.9.0/metadata_client/metadata_client.py`

 * *Files identical despite different names*

### Comparing `metadata_client-3.8.0/metadata_client/modules/__init__.py` & `metadata_client-3.9.0/metadata_client/modules/__init__.py`

 * *Files identical despite different names*

### Comparing `metadata_client-3.8.0/metadata_client/modules/dark_run.py` & `metadata_client-3.9.0/metadata_client/modules/dark_run.py`

 * *Files identical despite different names*

### Comparing `metadata_client-3.8.0/metadata_client/modules/data_file.py` & `metadata_client-3.9.0/metadata_client/modules/data_file.py`

 * *Files identical despite different names*

### Comparing `metadata_client-3.8.0/metadata_client/modules/data_group.py` & `metadata_client-3.9.0/metadata_client/modules/data_group.py`

 * *Files identical despite different names*

### Comparing `metadata_client-3.8.0/metadata_client/modules/data_group_repository.py` & `metadata_client-3.9.0/metadata_client/modules/data_group_repository.py`

 * *Files identical despite different names*

### Comparing `metadata_client-3.8.0/metadata_client/modules/data_group_type.py` & `metadata_client-3.9.0/metadata_client/modules/data_group_type.py`

 * *Files identical despite different names*

### Comparing `metadata_client-3.8.0/metadata_client/modules/data_source_group.py` & `metadata_client-3.9.0/metadata_client/modules/data_source_group.py`

 * *Files identical despite different names*

### Comparing `metadata_client-3.8.0/metadata_client/modules/data_source_group_version.py` & `metadata_client-3.9.0/metadata_client/modules/data_source_group_version.py`

 * *Files identical despite different names*

### Comparing `metadata_client-3.8.0/metadata_client/modules/data_type.py` & `metadata_client-3.9.0/metadata_client/modules/data_type.py`

 * *Files identical despite different names*

### Comparing `metadata_client-3.8.0/metadata_client/modules/experiment.py` & `metadata_client-3.9.0/metadata_client/modules/experiment.py`

 * *Files identical despite different names*

### Comparing `metadata_client-3.8.0/metadata_client/modules/experiment_type.py` & `metadata_client-3.9.0/metadata_client/modules/experiment_type.py`

 * *Files identical despite different names*

### Comparing `metadata_client-3.8.0/metadata_client/modules/instrument.py` & `metadata_client-3.9.0/metadata_client/modules/instrument.py`

 * *Files identical despite different names*

### Comparing `metadata_client-3.8.0/metadata_client/modules/parameter.py` & `metadata_client-3.9.0/metadata_client/modules/parameter.py`

 * *Files identical despite different names*

### Comparing `metadata_client-3.8.0/metadata_client/modules/parameter_type.py` & `metadata_client-3.9.0/metadata_client/modules/parameter_type.py`

 * *Files identical despite different names*

### Comparing `metadata_client-3.8.0/metadata_client/modules/proposal.py` & `metadata_client-3.9.0/metadata_client/modules/proposal.py`

 * *Files identical despite different names*

### Comparing `metadata_client-3.8.0/metadata_client/modules/repository.py` & `metadata_client-3.9.0/metadata_client/modules/repository.py`

 * *Files identical despite different names*

### Comparing `metadata_client-3.8.0/metadata_client/modules/run.py` & `metadata_client-3.9.0/metadata_client/modules/run.py`

 * *Files identical despite different names*

### Comparing `metadata_client-3.8.0/metadata_client/modules/sample.py` & `metadata_client-3.9.0/metadata_client/modules/sample.py`

 * *Files identical despite different names*

### Comparing `metadata_client-3.8.0/metadata_client/modules/user.py` & `metadata_client-3.9.0/metadata_client/modules/user.py`

 * *Files identical despite different names*

### Comparing `metadata_client-3.8.0/metadata_client/tests/apis/api_base.py` & `metadata_client-3.9.0/metadata_client/tests/apis/api_base.py`

 * *Files identical despite different names*

### Comparing `metadata_client-3.8.0/metadata_client/tests/apis/dark_run_api_test.py` & `metadata_client-3.9.0/metadata_client/tests/apis/dark_run_api_test.py`

 * *Files identical despite different names*

### Comparing `metadata_client-3.8.0/metadata_client/tests/apis/data_file_api_test.py` & `metadata_client-3.9.0/metadata_client/tests/apis/data_file_api_test.py`

 * *Files identical despite different names*

### Comparing `metadata_client-3.8.0/metadata_client/tests/apis/data_group_api_test.py` & `metadata_client-3.9.0/metadata_client/tests/apis/data_group_api_test.py`

 * *Files identical despite different names*

### Comparing `metadata_client-3.8.0/metadata_client/tests/apis/data_group_repository_api_test.py` & `metadata_client-3.9.0/metadata_client/tests/apis/data_group_repository_api_test.py`

 * *Files identical despite different names*

### Comparing `metadata_client-3.8.0/metadata_client/tests/apis/data_group_type_api_test.py` & `metadata_client-3.9.0/metadata_client/tests/apis/data_group_type_api_test.py`

 * *Files identical despite different names*

### Comparing `metadata_client-3.8.0/metadata_client/tests/apis/data_type_api_test.py` & `metadata_client-3.9.0/metadata_client/tests/apis/data_type_api_test.py`

 * *Files identical despite different names*

### Comparing `metadata_client-3.8.0/metadata_client/tests/apis/experiment_api_test.py` & `metadata_client-3.9.0/metadata_client/tests/apis/experiment_api_test.py`

 * *Files identical despite different names*

### Comparing `metadata_client-3.8.0/metadata_client/tests/apis/experiment_type_api_test.py` & `metadata_client-3.9.0/metadata_client/tests/apis/experiment_type_api_test.py`

 * *Files identical despite different names*

### Comparing `metadata_client-3.8.0/metadata_client/tests/apis/instrument_api_test.py` & `metadata_client-3.9.0/metadata_client/tests/apis/instrument_api_test.py`

 * *Files identical despite different names*

### Comparing `metadata_client-3.8.0/metadata_client/tests/apis/parameter_api_test.py` & `metadata_client-3.9.0/metadata_client/tests/apis/parameter_api_test.py`

 * *Files identical despite different names*

### Comparing `metadata_client-3.8.0/metadata_client/tests/apis/parameter_type_api_test.py` & `metadata_client-3.9.0/metadata_client/tests/apis/parameter_type_api_test.py`

 * *Files identical despite different names*

### Comparing `metadata_client-3.8.0/metadata_client/tests/apis/proposal_api_test.py` & `metadata_client-3.9.0/metadata_client/tests/apis/proposal_api_test.py`

 * *Files identical despite different names*

### Comparing `metadata_client-3.8.0/metadata_client/tests/apis/repository_api_test.py` & `metadata_client-3.9.0/metadata_client/tests/apis/repository_api_test.py`

 * *Files identical despite different names*

### Comparing `metadata_client-3.8.0/metadata_client/tests/apis/run_api_test.py` & `metadata_client-3.9.0/metadata_client/tests/apis/run_api_test.py`

 * *Files identical despite different names*

### Comparing `metadata_client-3.8.0/metadata_client/tests/apis/sample_api_test.py` & `metadata_client-3.9.0/metadata_client/tests/apis/sample_api_test.py`

 * *Files identical despite different names*

### Comparing `metadata_client-3.8.0/metadata_client/tests/apis/user_api_test.py` & `metadata_client-3.9.0/metadata_client/tests/apis/user_api_test.py`

 * *Files identical despite different names*

### Comparing `metadata_client-3.8.0/metadata_client/tests/common/base_test.py` & `metadata_client-3.9.0/metadata_client/tests/common/base_test.py`

 * *Files identical despite different names*

### Comparing `metadata_client-3.8.0/metadata_client/tests/common/config_test.py` & `metadata_client-3.9.0/metadata_client/tests/common/config_test.py`

 * *Files identical despite different names*

### Comparing `metadata_client-3.8.0/metadata_client/tests/common/generators.py` & `metadata_client-3.9.0/metadata_client/tests/common/generators.py`

 * *Files identical despite different names*

### Comparing `metadata_client-3.8.0/metadata_client/tests/common/secrets.py` & `metadata_client-3.9.0/metadata_client/tests/common/secrets.py`

 * *Files identical despite different names*

### Comparing `metadata_client-3.8.0/metadata_client/tests/common/util.py` & `metadata_client-3.9.0/metadata_client/tests/common/util.py`

 * *Files identical despite different names*

### Comparing `metadata_client-3.8.0/metadata_client/tests/common/util_datetime.py` & `metadata_client-3.9.0/metadata_client/tests/common/util_datetime.py`

 * *Files identical despite different names*

### Comparing `metadata_client-3.8.0/metadata_client/tests/common/util_test.py` & `metadata_client-3.9.0/metadata_client/tests/common/util_test.py`

 * *Files identical despite different names*

### Comparing `metadata_client-3.8.0/metadata_client/tests/metadata_client_connection_test.py` & `metadata_client-3.9.0/metadata_client/tests/metadata_client_connection_test.py`

 * *Files identical despite different names*

### Comparing `metadata_client-3.8.0/metadata_client/tests/metadata_client_test.py` & `metadata_client-3.9.0/metadata_client/tests/metadata_client_test.py`

 * *Files identical despite different names*

### Comparing `metadata_client-3.8.0/metadata_client/tests/modules/dark_run_test.py` & `metadata_client-3.9.0/metadata_client/tests/modules/dark_run_test.py`

 * *Files identical despite different names*

### Comparing `metadata_client-3.8.0/metadata_client/tests/modules/data_file_test.py` & `metadata_client-3.9.0/metadata_client/tests/modules/data_file_test.py`

 * *Files identical despite different names*

### Comparing `metadata_client-3.8.0/metadata_client/tests/modules/data_group_repository_test.py` & `metadata_client-3.9.0/metadata_client/tests/modules/data_group_repository_test.py`

 * *Files identical despite different names*

### Comparing `metadata_client-3.8.0/metadata_client/tests/modules/data_group_test.py` & `metadata_client-3.9.0/metadata_client/tests/modules/data_group_test.py`

 * *Files identical despite different names*

### Comparing `metadata_client-3.8.0/metadata_client/tests/modules/data_group_type_test.py` & `metadata_client-3.9.0/metadata_client/tests/modules/data_group_type_test.py`

 * *Files identical despite different names*

### Comparing `metadata_client-3.8.0/metadata_client/tests/modules/data_type_test.py` & `metadata_client-3.9.0/metadata_client/tests/modules/data_type_test.py`

 * *Files identical despite different names*

### Comparing `metadata_client-3.8.0/metadata_client/tests/modules/experiment_test.py` & `metadata_client-3.9.0/metadata_client/tests/modules/experiment_test.py`

 * *Files identical despite different names*

### Comparing `metadata_client-3.8.0/metadata_client/tests/modules/experiment_type_test.py` & `metadata_client-3.9.0/metadata_client/tests/modules/experiment_type_test.py`

 * *Files identical despite different names*

### Comparing `metadata_client-3.8.0/metadata_client/tests/modules/module_base.py` & `metadata_client-3.9.0/metadata_client/tests/modules/module_base.py`

 * *Files identical despite different names*

### Comparing `metadata_client-3.8.0/metadata_client/tests/modules/parameter_test.py` & `metadata_client-3.9.0/metadata_client/tests/modules/parameter_test.py`

 * *Files identical despite different names*

### Comparing `metadata_client-3.8.0/metadata_client/tests/modules/parameter_type_test.py` & `metadata_client-3.9.0/metadata_client/tests/modules/parameter_type_test.py`

 * *Files identical despite different names*

### Comparing `metadata_client-3.8.0/metadata_client/tests/modules/proposal_test.py` & `metadata_client-3.9.0/metadata_client/tests/modules/proposal_test.py`

 * *Files identical despite different names*

### Comparing `metadata_client-3.8.0/metadata_client/tests/modules/repository_test.py` & `metadata_client-3.9.0/metadata_client/tests/modules/repository_test.py`

 * *Files identical despite different names*

### Comparing `metadata_client-3.8.0/metadata_client/tests/modules/run_test.py` & `metadata_client-3.9.0/metadata_client/tests/modules/run_test.py`

 * *Files identical despite different names*

### Comparing `metadata_client-3.8.0/metadata_client/tests/modules/sample_test.py` & `metadata_client-3.9.0/metadata_client/tests/modules/sample_test.py`

 * *Files identical despite different names*

### Comparing `metadata_client-3.8.0/metadata_client.egg-info/PKG-INFO` & `metadata_client-3.9.0/metadata_client.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: metadata-client
-Version: 3.8.0
+Version: 3.9.0
 Summary: Python Client for European XFEL Metadata Catalogue Web App available at https://in.xfel.eu/metadata
 Home-page: https://git.xfel.eu/gitlab/ITDM/metadata_client
 Author: Luís Maia
 Author-email: luis.maia@xfel.eu
 Maintainer: Luís Maia
 Maintainer-email: luis.maia@xfel.eu
 License: MIT
@@ -17,15 +17,15 @@
 Classifier: Natural Language :: English
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: OS Independent
 Classifier: Topic :: Scientific/Engineering :: Information Analysis
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
-Requires-Python: >=3.6
+Requires-Python: >=3.7
 Provides-Extra: test
 License-File: LICENSE
 License-File: AUTHORS.rst
 
 Metadata Catalogue Client
 =========================
 
@@ -89,15 +89,15 @@
     # Force re-installation of packages
     pip install --ignore-installed
 
  Installing it will place two folders under the current Python installation
  site-packages folder:
 
  - `metadata_client` with the sources;
- - `metadata_client-3.8.0.dist-info/` with Wheels configuration files.
+ - `metadata_client-3.9.0.dist-info/` with Wheels configuration files.
 
  To identify your Python site-packages folder run::
 
     python -c "from distutils.sysconfig import get_python_lib; print(get_python_lib())"
 
 
 Usage
@@ -371,9 +371,7 @@
     python setup.py bdist_wheel
 
     # Upload new version .egg and .whl files
     twine upload dist/*
 
     # In case a test is necessary, it is possible to test it against test.pypi.org
     twine upload --repository-url https://test.pypi.org/legacy/ dist/* --verbose
-
-
```

### Comparing `metadata_client-3.8.0/metadata_client.egg-info/SOURCES.txt` & `metadata_client-3.9.0/metadata_client.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `metadata_client-3.8.0/setup.py` & `metadata_client-3.9.0/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -48,15 +48,15 @@
     extras_require={'test': [
         'pytest',
         'pytest-cov',
         'python-dateutil',
         'pytz',
         'pycodestyle'
     ]},
-    python_requires='>=3.6',
+    python_requires='>=3.7',
     classifiers=[
         'Development Status :: 5 - Production/Stable',
         'Environment :: Web Environment',
         'Environment :: Console',
         'Intended Audience :: Developers',
         'Intended Audience :: Science/Research',
         'Natural Language :: English',
```

