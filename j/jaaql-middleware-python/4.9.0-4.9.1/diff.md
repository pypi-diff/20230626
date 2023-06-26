# Comparing `tmp/jaaql-middleware-python-4.9.0.tar.gz` & `tmp/jaaql-middleware-python-4.9.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "jaaql-middleware-python-4.9.0.tar", last modified: Sat May  6 14:31:55 2023, max compression
+gzip compressed data, was "jaaql-middleware-python-4.9.1.tar", last modified: Sat May  6 14:40:09 2023, max compression
```

## Comparing `jaaql-middleware-python-4.9.0.tar` & `jaaql-middleware-python-4.9.1.tar`

### file list

```diff
@@ -1,86 +1,86 @@
-drwxrwxrwx   0        0        0        0 2023-05-06 14:31:55.343793 jaaql-middleware-python-4.9.0/
--rw-rw-rw-   0        0        0    18134 2022-03-12 16:03:36.000000 jaaql-middleware-python-4.9.0/LICENSE.txt
--rw-rw-rw-   0        0        0      946 2023-05-06 14:31:55.343793 jaaql-middleware-python-4.9.0/PKG-INFO
--rw-rw-rw-   0        0        0      453 2023-04-26 22:40:37.000000 jaaql-middleware-python-4.9.0/README.md
-drwxrwxrwx   0        0        0        0 2023-05-06 14:31:55.280793 jaaql-middleware-python-4.9.0/jaaql/
--rw-rw-rw-   0        0        0        0 2022-03-12 16:03:36.000000 jaaql-middleware-python-4.9.0/jaaql/__init__.py
-drwxrwxrwx   0        0        0        0 2023-05-06 14:31:55.284795 jaaql-middleware-python-4.9.0/jaaql/config/
--rw-rw-rw-   0        0        0        0 2022-03-12 16:03:36.000000 jaaql-middleware-python-4.9.0/jaaql/config/__init__.py
--rw-rw-rw-   0        0        0      324 2023-04-26 22:40:37.000000 jaaql-middleware-python-4.9.0/jaaql/config/config-docker.ini
--rw-rw-rw-   0        0        0      253 2023-04-26 22:40:37.000000 jaaql-middleware-python-4.9.0/jaaql/config/config-test.ini
--rw-rw-rw-   0        0        0      291 2023-04-26 22:40:37.000000 jaaql-middleware-python-4.9.0/jaaql/config/config.ini
--rw-rw-rw-   0        0        0      470 2023-04-26 22:40:37.000000 jaaql-middleware-python-4.9.0/jaaql/config_constants.py
--rw-rw-rw-   0        0        0     4496 2023-05-06 14:31:29.000000 jaaql-middleware-python-4.9.0/jaaql/constants.py
-drwxrwxrwx   0        0        0        0 2023-05-06 14:31:55.289792 jaaql-middleware-python-4.9.0/jaaql/db/
--rw-rw-rw-   0        0        0        0 2022-05-19 20:40:08.000000 jaaql-middleware-python-4.9.0/jaaql/db/__init__.py
--rw-rw-rw-   0        0        0     6929 2023-05-02 18:15:39.000000 jaaql-middleware-python-4.9.0/jaaql/db/db_interface.py
--rw-rw-rw-   0        0        0    11198 2023-04-26 22:40:37.000000 jaaql-middleware-python-4.9.0/jaaql/db/db_pg_interface.py
--rw-rw-rw-   0        0        0     7062 2023-05-02 19:35:29.000000 jaaql-middleware-python-4.9.0/jaaql/db/db_utils.py
--rw-rw-rw-   0        0        0     2934 2023-05-02 18:45:07.000000 jaaql-middleware-python-4.9.0/jaaql/db/db_utils_no_circ.py
-drwxrwxrwx   0        0        0        0 2023-05-06 14:31:55.293792 jaaql-middleware-python-4.9.0/jaaql/documentation/
--rw-rw-rw-   0        0        0        0 2022-03-12 16:03:36.000000 jaaql-middleware-python-4.9.0/jaaql/documentation/__init__.py
--rw-rw-rw-   0        0        0     6592 2023-05-02 12:22:14.000000 jaaql-middleware-python-4.9.0/jaaql/documentation/documentation_internal.py
--rw-rw-rw-   0        0        0     8192 2023-04-26 22:40:37.000000 jaaql-middleware-python-4.9.0/jaaql/documentation/documentation_public.py
--rw-rw-rw-   0        0        0     3456 2023-04-26 22:40:37.000000 jaaql-middleware-python-4.9.0/jaaql/documentation/documentation_shared.py
-drwxrwxrwx   0        0        0        0 2023-05-06 14:31:55.297812 jaaql-middleware-python-4.9.0/jaaql/email/
--rw-rw-rw-   0        0        0        0 2022-05-05 10:44:50.000000 jaaql-middleware-python-4.9.0/jaaql/email/__init__.py
--rw-rw-rw-   0        0        0     7331 2023-05-03 00:21:37.000000 jaaql-middleware-python-4.9.0/jaaql/email/email_manager.py
--rw-rw-rw-   0        0        0    19242 2023-04-26 22:40:37.000000 jaaql-middleware-python-4.9.0/jaaql/email/email_manager_service.py
--rw-rw-rw-   0        0        0      234 2023-04-26 22:40:37.000000 jaaql-middleware-python-4.9.0/jaaql/email/patch_ems.py
-drwxrwxrwx   0        0        0        0 2023-05-06 14:31:55.302792 jaaql-middleware-python-4.9.0/jaaql/exceptions/
--rw-rw-rw-   0        0        0        0 2022-03-12 16:03:36.000000 jaaql-middleware-python-4.9.0/jaaql/exceptions/__init__.py
--rw-rw-rw-   0        0        0      401 2022-04-17 07:42:21.000000 jaaql-middleware-python-4.9.0/jaaql/exceptions/custom_http_status.py
--rw-rw-rw-   0        0        0      985 2022-05-20 15:36:28.000000 jaaql-middleware-python-4.9.0/jaaql/exceptions/http_status_exception.py
--rw-rw-rw-   0        0        0      321 2022-03-12 16:03:36.000000 jaaql-middleware-python-4.9.0/jaaql/exceptions/not_yet_implement_exception.py
-drwxrwxrwx   0        0        0        0 2023-05-06 14:31:55.303792 jaaql-middleware-python-4.9.0/jaaql/interpreter/
--rw-rw-rw-   0        0        0        0 2022-03-12 16:03:36.000000 jaaql-middleware-python-4.9.0/jaaql/interpreter/__init__.py
--rw-rw-rw-   0        0        0    23250 2023-05-02 18:09:24.000000 jaaql-middleware-python-4.9.0/jaaql/interpreter/interpret_jaaql.py
--rw-rw-rw-   0        0        0     5962 2023-05-02 12:06:24.000000 jaaql-middleware-python-4.9.0/jaaql/jaaql.py
-drwxrwxrwx   0        0        0        0 2023-05-06 14:31:55.306792 jaaql-middleware-python-4.9.0/jaaql/migrations/
--rw-rw-rw-   0        0        0        0 2022-03-12 16:03:36.000000 jaaql-middleware-python-4.9.0/jaaql/migrations/__init__.py
--rw-rw-rw-   0        0        0      683 2022-09-19 00:09:13.000000 jaaql-middleware-python-4.9.0/jaaql/migrations/migration_history.sql
--rw-rw-rw-   0        0        0     8620 2023-05-03 01:48:38.000000 jaaql-middleware-python-4.9.0/jaaql/migrations/migrations.py
-drwxrwxrwx   0        0        0        0 2023-05-06 14:31:55.318793 jaaql-middleware-python-4.9.0/jaaql/mvc/
--rw-rw-rw-   0        0        0        0 2022-03-12 16:03:36.000000 jaaql-middleware-python-4.9.0/jaaql/mvc/__init__.py
--rw-rw-rw-   0        0        0    32856 2023-05-04 13:15:14.000000 jaaql-middleware-python-4.9.0/jaaql/mvc/base_controller.py
--rw-rw-rw-   0        0        0    11591 2023-05-02 12:24:40.000000 jaaql-middleware-python-4.9.0/jaaql/mvc/base_model.py
--rw-rw-rw-   0        0        0     3928 2023-05-02 12:51:04.000000 jaaql-middleware-python-4.9.0/jaaql/mvc/controller.py
--rw-rw-rw-   0        0        0      274 2022-03-12 16:03:36.000000 jaaql-middleware-python-4.9.0/jaaql/mvc/controller_interface.py
--rw-rw-rw-   0        0        0     7494 2023-04-26 22:40:37.000000 jaaql-middleware-python-4.9.0/jaaql/mvc/exception_queries.py
--rw-rw-rw-   0        0        0    43043 2023-04-26 22:40:37.000000 jaaql-middleware-python-4.9.0/jaaql/mvc/generated_queries.py
--rw-rw-rw-   0        0        0      232 2023-04-26 22:40:37.000000 jaaql-middleware-python-4.9.0/jaaql/mvc/handmade_queries.py
--rw-rw-rw-   0        0        0    38055 2023-05-02 18:45:01.000000 jaaql-middleware-python-4.9.0/jaaql/mvc/model.py
--rw-rw-rw-   0        0        0      257 2022-05-07 20:33:26.000000 jaaql-middleware-python-4.9.0/jaaql/mvc/model_interface.py
--rw-rw-rw-   0        0        0      209 2023-04-26 22:40:37.000000 jaaql-middleware-python-4.9.0/jaaql/mvc/response.py
-drwxrwxrwx   0        0        0        0 2023-05-06 14:31:55.319807 jaaql-middleware-python-4.9.0/jaaql/openapi/
--rw-rw-rw-   0        0        0        0 2022-03-12 16:03:36.000000 jaaql-middleware-python-4.9.0/jaaql/openapi/__init__.py
--rw-rw-rw-   0        0        0    28821 2023-05-02 11:33:27.000000 jaaql-middleware-python-4.9.0/jaaql/openapi/swagger_documentation.py
--rw-rw-rw-   0        0        0      149 2022-06-11 20:45:39.000000 jaaql-middleware-python-4.9.0/jaaql/patch.py
-drwxrwxrwx   0        0        0        0 2023-05-06 14:31:55.326793 jaaql-middleware-python-4.9.0/jaaql/scripts/
--rw-rw-rw-   0        0        0     1379 2023-04-26 22:40:37.000000 jaaql-middleware-python-4.9.0/jaaql/scripts/01.install_domains.generated.sql
--rw-rw-rw-   0        0        0      939 2023-04-26 22:40:37.000000 jaaql-middleware-python-4.9.0/jaaql/scripts/02.install_super_user.exceptions.sql
--rw-rw-rw-   0        0        0     1960 2023-05-06 14:31:29.000000 jaaql-middleware-python-4.9.0/jaaql/scripts/03.install_super_user.handwritten.sql
--rw-rw-rw-   0        0        0     7492 2023-04-26 22:40:37.000000 jaaql-middleware-python-4.9.0/jaaql/scripts/04.install_jaaql_data_structures.generated.sql
--rw-rw-rw-   0        0        0      324 2023-04-26 22:40:37.000000 jaaql-middleware-python-4.9.0/jaaql/scripts/05.install_jaaql.exceptions.sql
--rw-rw-rw-   0        0        0      990 2023-04-26 22:40:37.000000 jaaql-middleware-python-4.9.0/jaaql/scripts/06.install_jaaql.handwritten.sql
--rw-rw-rw-   0        0        0     4105 2023-02-12 10:12:32.000000 jaaql-middleware-python-4.9.0/jaaql/scripts/swagger_template.html
-drwxrwxrwx   0        0        0        0 2023-05-06 14:31:55.330792 jaaql-middleware-python-4.9.0/jaaql/services/
--rw-rw-rw-   0        0        0        0 2022-07-10 13:56:37.000000 jaaql-middleware-python-4.9.0/jaaql/services/__init__.py
--rw-rw-rw-   0        0        0     2688 2023-04-26 22:40:37.000000 jaaql-middleware-python-4.9.0/jaaql/services/cached_canned_query_service.py
--rw-rw-rw-   0        0        0     2096 2023-05-03 01:33:07.000000 jaaql-middleware-python-4.9.0/jaaql/services/migrations_manager_service.py
--rw-rw-rw-   0        0        0      296 2023-05-03 01:25:04.000000 jaaql-middleware-python-4.9.0/jaaql/services/patch_mms.py
-drwxrwxrwx   0        0        0        0 2023-05-06 14:31:55.337792 jaaql-middleware-python-4.9.0/jaaql/utilities/
--rw-rw-rw-   0        0        0        0 2022-03-12 16:03:36.000000 jaaql-middleware-python-4.9.0/jaaql/utilities/__init__.py
--rw-rw-rw-   0        0        0     6698 2023-04-26 22:40:37.000000 jaaql-middleware-python-4.9.0/jaaql/utilities/crypt_utils.py
--rw-rw-rw-   0        0        0     5357 2023-05-02 10:06:52.000000 jaaql-middleware-python-4.9.0/jaaql/utilities/options.py
--rw-rw-rw-   0        0        0     5162 2023-05-02 17:32:54.000000 jaaql-middleware-python-4.9.0/jaaql/utilities/utils.py
--rw-rw-rw-   0        0        0     2636 2023-05-02 18:18:38.000000 jaaql-middleware-python-4.9.0/jaaql/utilities/utils_no_project_imports.py
--rw-rw-rw-   0        0        0     2160 2022-05-22 11:21:40.000000 jaaql-middleware-python-4.9.0/jaaql/utilities/vault.py
-drwxrwxrwx   0        0        0        0 2023-05-06 14:31:55.342792 jaaql-middleware-python-4.9.0/jaaql_middleware_python.egg-info/
--rw-rw-rw-   0        0        0      946 2023-05-06 14:31:55.000000 jaaql-middleware-python-4.9.0/jaaql_middleware_python.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     2221 2023-05-06 14:31:55.000000 jaaql-middleware-python-4.9.0/jaaql_middleware_python.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-06 14:31:55.000000 jaaql-middleware-python-4.9.0/jaaql_middleware_python.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      337 2023-05-06 14:31:55.000000 jaaql-middleware-python-4.9.0/jaaql_middleware_python.egg-info/requires.txt
--rw-rw-rw-   0        0        0        6 2023-05-06 14:31:55.000000 jaaql-middleware-python-4.9.0/jaaql_middleware_python.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-05-06 14:31:55.343793 jaaql-middleware-python-4.9.0/setup.cfg
--rw-rw-rw-   0        0        0      893 2022-03-12 16:03:36.000000 jaaql-middleware-python-4.9.0/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-06 14:40:09.164515 jaaql-middleware-python-4.9.1/
+-rw-rw-rw-   0        0        0    18134 2022-03-12 16:03:36.000000 jaaql-middleware-python-4.9.1/LICENSE.txt
+-rw-rw-rw-   0        0        0      946 2023-05-06 14:40:09.163529 jaaql-middleware-python-4.9.1/PKG-INFO
+-rw-rw-rw-   0        0        0      453 2023-04-26 22:40:37.000000 jaaql-middleware-python-4.9.1/README.md
+drwxrwxrwx   0        0        0        0 2023-05-06 14:40:09.106518 jaaql-middleware-python-4.9.1/jaaql/
+-rw-rw-rw-   0        0        0        0 2022-03-12 16:03:36.000000 jaaql-middleware-python-4.9.1/jaaql/__init__.py
+drwxrwxrwx   0        0        0        0 2023-05-06 14:40:09.110516 jaaql-middleware-python-4.9.1/jaaql/config/
+-rw-rw-rw-   0        0        0        0 2022-03-12 16:03:36.000000 jaaql-middleware-python-4.9.1/jaaql/config/__init__.py
+-rw-rw-rw-   0        0        0      324 2023-04-26 22:40:37.000000 jaaql-middleware-python-4.9.1/jaaql/config/config-docker.ini
+-rw-rw-rw-   0        0        0      253 2023-04-26 22:40:37.000000 jaaql-middleware-python-4.9.1/jaaql/config/config-test.ini
+-rw-rw-rw-   0        0        0      291 2023-04-26 22:40:37.000000 jaaql-middleware-python-4.9.1/jaaql/config/config.ini
+-rw-rw-rw-   0        0        0      470 2023-04-26 22:40:37.000000 jaaql-middleware-python-4.9.1/jaaql/config_constants.py
+-rw-rw-rw-   0        0        0     4496 2023-05-06 14:39:41.000000 jaaql-middleware-python-4.9.1/jaaql/constants.py
+drwxrwxrwx   0        0        0        0 2023-05-06 14:40:09.114513 jaaql-middleware-python-4.9.1/jaaql/db/
+-rw-rw-rw-   0        0        0        0 2022-05-19 20:40:08.000000 jaaql-middleware-python-4.9.1/jaaql/db/__init__.py
+-rw-rw-rw-   0        0        0     6929 2023-05-02 18:15:39.000000 jaaql-middleware-python-4.9.1/jaaql/db/db_interface.py
+-rw-rw-rw-   0        0        0    11198 2023-04-26 22:40:37.000000 jaaql-middleware-python-4.9.1/jaaql/db/db_pg_interface.py
+-rw-rw-rw-   0        0        0     7062 2023-05-02 19:35:29.000000 jaaql-middleware-python-4.9.1/jaaql/db/db_utils.py
+-rw-rw-rw-   0        0        0     2934 2023-05-02 18:45:07.000000 jaaql-middleware-python-4.9.1/jaaql/db/db_utils_no_circ.py
+drwxrwxrwx   0        0        0        0 2023-05-06 14:40:09.119517 jaaql-middleware-python-4.9.1/jaaql/documentation/
+-rw-rw-rw-   0        0        0        0 2022-03-12 16:03:36.000000 jaaql-middleware-python-4.9.1/jaaql/documentation/__init__.py
+-rw-rw-rw-   0        0        0     6592 2023-05-02 12:22:14.000000 jaaql-middleware-python-4.9.1/jaaql/documentation/documentation_internal.py
+-rw-rw-rw-   0        0        0     8192 2023-04-26 22:40:37.000000 jaaql-middleware-python-4.9.1/jaaql/documentation/documentation_public.py
+-rw-rw-rw-   0        0        0     3456 2023-04-26 22:40:37.000000 jaaql-middleware-python-4.9.1/jaaql/documentation/documentation_shared.py
+drwxrwxrwx   0        0        0        0 2023-05-06 14:40:09.122513 jaaql-middleware-python-4.9.1/jaaql/email/
+-rw-rw-rw-   0        0        0        0 2022-05-05 10:44:50.000000 jaaql-middleware-python-4.9.1/jaaql/email/__init__.py
+-rw-rw-rw-   0        0        0     7331 2023-05-03 00:21:37.000000 jaaql-middleware-python-4.9.1/jaaql/email/email_manager.py
+-rw-rw-rw-   0        0        0    19242 2023-04-26 22:40:37.000000 jaaql-middleware-python-4.9.1/jaaql/email/email_manager_service.py
+-rw-rw-rw-   0        0        0      234 2023-04-26 22:40:37.000000 jaaql-middleware-python-4.9.1/jaaql/email/patch_ems.py
+drwxrwxrwx   0        0        0        0 2023-05-06 14:40:09.126515 jaaql-middleware-python-4.9.1/jaaql/exceptions/
+-rw-rw-rw-   0        0        0        0 2022-03-12 16:03:36.000000 jaaql-middleware-python-4.9.1/jaaql/exceptions/__init__.py
+-rw-rw-rw-   0        0        0      401 2022-04-17 07:42:21.000000 jaaql-middleware-python-4.9.1/jaaql/exceptions/custom_http_status.py
+-rw-rw-rw-   0        0        0      985 2022-05-20 15:36:28.000000 jaaql-middleware-python-4.9.1/jaaql/exceptions/http_status_exception.py
+-rw-rw-rw-   0        0        0      321 2022-03-12 16:03:36.000000 jaaql-middleware-python-4.9.1/jaaql/exceptions/not_yet_implement_exception.py
+drwxrwxrwx   0        0        0        0 2023-05-06 14:40:09.128514 jaaql-middleware-python-4.9.1/jaaql/interpreter/
+-rw-rw-rw-   0        0        0        0 2022-03-12 16:03:36.000000 jaaql-middleware-python-4.9.1/jaaql/interpreter/__init__.py
+-rw-rw-rw-   0        0        0    23250 2023-05-02 18:09:24.000000 jaaql-middleware-python-4.9.1/jaaql/interpreter/interpret_jaaql.py
+-rw-rw-rw-   0        0        0     5962 2023-05-02 12:06:24.000000 jaaql-middleware-python-4.9.1/jaaql/jaaql.py
+drwxrwxrwx   0        0        0        0 2023-05-06 14:40:09.130515 jaaql-middleware-python-4.9.1/jaaql/migrations/
+-rw-rw-rw-   0        0        0        0 2022-03-12 16:03:36.000000 jaaql-middleware-python-4.9.1/jaaql/migrations/__init__.py
+-rw-rw-rw-   0        0        0      683 2022-09-19 00:09:13.000000 jaaql-middleware-python-4.9.1/jaaql/migrations/migration_history.sql
+-rw-rw-rw-   0        0        0     8620 2023-05-03 01:48:38.000000 jaaql-middleware-python-4.9.1/jaaql/migrations/migrations.py
+drwxrwxrwx   0        0        0        0 2023-05-06 14:40:09.141514 jaaql-middleware-python-4.9.1/jaaql/mvc/
+-rw-rw-rw-   0        0        0        0 2022-03-12 16:03:36.000000 jaaql-middleware-python-4.9.1/jaaql/mvc/__init__.py
+-rw-rw-rw-   0        0        0    32856 2023-05-04 13:15:14.000000 jaaql-middleware-python-4.9.1/jaaql/mvc/base_controller.py
+-rw-rw-rw-   0        0        0    11591 2023-05-02 12:24:40.000000 jaaql-middleware-python-4.9.1/jaaql/mvc/base_model.py
+-rw-rw-rw-   0        0        0     3928 2023-05-02 12:51:04.000000 jaaql-middleware-python-4.9.1/jaaql/mvc/controller.py
+-rw-rw-rw-   0        0        0      274 2022-03-12 16:03:36.000000 jaaql-middleware-python-4.9.1/jaaql/mvc/controller_interface.py
+-rw-rw-rw-   0        0        0     7494 2023-04-26 22:40:37.000000 jaaql-middleware-python-4.9.1/jaaql/mvc/exception_queries.py
+-rw-rw-rw-   0        0        0    43043 2023-04-26 22:40:37.000000 jaaql-middleware-python-4.9.1/jaaql/mvc/generated_queries.py
+-rw-rw-rw-   0        0        0      232 2023-04-26 22:40:37.000000 jaaql-middleware-python-4.9.1/jaaql/mvc/handmade_queries.py
+-rw-rw-rw-   0        0        0    38055 2023-05-02 18:45:01.000000 jaaql-middleware-python-4.9.1/jaaql/mvc/model.py
+-rw-rw-rw-   0        0        0      257 2022-05-07 20:33:26.000000 jaaql-middleware-python-4.9.1/jaaql/mvc/model_interface.py
+-rw-rw-rw-   0        0        0      209 2023-04-26 22:40:37.000000 jaaql-middleware-python-4.9.1/jaaql/mvc/response.py
+drwxrwxrwx   0        0        0        0 2023-05-06 14:40:09.143516 jaaql-middleware-python-4.9.1/jaaql/openapi/
+-rw-rw-rw-   0        0        0        0 2022-03-12 16:03:36.000000 jaaql-middleware-python-4.9.1/jaaql/openapi/__init__.py
+-rw-rw-rw-   0        0        0    28821 2023-05-02 11:33:27.000000 jaaql-middleware-python-4.9.1/jaaql/openapi/swagger_documentation.py
+-rw-rw-rw-   0        0        0      149 2022-06-11 20:45:39.000000 jaaql-middleware-python-4.9.1/jaaql/patch.py
+drwxrwxrwx   0        0        0        0 2023-05-06 14:40:09.149515 jaaql-middleware-python-4.9.1/jaaql/scripts/
+-rw-rw-rw-   0        0        0     1379 2023-04-26 22:40:37.000000 jaaql-middleware-python-4.9.1/jaaql/scripts/01.install_domains.generated.sql
+-rw-rw-rw-   0        0        0      939 2023-04-26 22:40:37.000000 jaaql-middleware-python-4.9.1/jaaql/scripts/02.install_super_user.exceptions.sql
+-rw-rw-rw-   0        0        0     2006 2023-05-06 14:39:26.000000 jaaql-middleware-python-4.9.1/jaaql/scripts/03.install_super_user.handwritten.sql
+-rw-rw-rw-   0        0        0     7492 2023-04-26 22:40:37.000000 jaaql-middleware-python-4.9.1/jaaql/scripts/04.install_jaaql_data_structures.generated.sql
+-rw-rw-rw-   0        0        0      324 2023-04-26 22:40:37.000000 jaaql-middleware-python-4.9.1/jaaql/scripts/05.install_jaaql.exceptions.sql
+-rw-rw-rw-   0        0        0      990 2023-04-26 22:40:37.000000 jaaql-middleware-python-4.9.1/jaaql/scripts/06.install_jaaql.handwritten.sql
+-rw-rw-rw-   0        0        0     4105 2023-02-12 10:12:32.000000 jaaql-middleware-python-4.9.1/jaaql/scripts/swagger_template.html
+drwxrwxrwx   0        0        0        0 2023-05-06 14:40:09.152543 jaaql-middleware-python-4.9.1/jaaql/services/
+-rw-rw-rw-   0        0        0        0 2022-07-10 13:56:37.000000 jaaql-middleware-python-4.9.1/jaaql/services/__init__.py
+-rw-rw-rw-   0        0        0     2688 2023-04-26 22:40:37.000000 jaaql-middleware-python-4.9.1/jaaql/services/cached_canned_query_service.py
+-rw-rw-rw-   0        0        0     2096 2023-05-03 01:33:07.000000 jaaql-middleware-python-4.9.1/jaaql/services/migrations_manager_service.py
+-rw-rw-rw-   0        0        0      296 2023-05-03 01:25:04.000000 jaaql-middleware-python-4.9.1/jaaql/services/patch_mms.py
+drwxrwxrwx   0        0        0        0 2023-05-06 14:40:09.158538 jaaql-middleware-python-4.9.1/jaaql/utilities/
+-rw-rw-rw-   0        0        0        0 2022-03-12 16:03:36.000000 jaaql-middleware-python-4.9.1/jaaql/utilities/__init__.py
+-rw-rw-rw-   0        0        0     6698 2023-04-26 22:40:37.000000 jaaql-middleware-python-4.9.1/jaaql/utilities/crypt_utils.py
+-rw-rw-rw-   0        0        0     5357 2023-05-02 10:06:52.000000 jaaql-middleware-python-4.9.1/jaaql/utilities/options.py
+-rw-rw-rw-   0        0        0     5162 2023-05-02 17:32:54.000000 jaaql-middleware-python-4.9.1/jaaql/utilities/utils.py
+-rw-rw-rw-   0        0        0     2636 2023-05-02 18:18:38.000000 jaaql-middleware-python-4.9.1/jaaql/utilities/utils_no_project_imports.py
+-rw-rw-rw-   0        0        0     2160 2022-05-22 11:21:40.000000 jaaql-middleware-python-4.9.1/jaaql/utilities/vault.py
+drwxrwxrwx   0        0        0        0 2023-05-06 14:40:09.162529 jaaql-middleware-python-4.9.1/jaaql_middleware_python.egg-info/
+-rw-rw-rw-   0        0        0      946 2023-05-06 14:40:09.000000 jaaql-middleware-python-4.9.1/jaaql_middleware_python.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     2221 2023-05-06 14:40:09.000000 jaaql-middleware-python-4.9.1/jaaql_middleware_python.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-06 14:40:09.000000 jaaql-middleware-python-4.9.1/jaaql_middleware_python.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      337 2023-05-06 14:40:09.000000 jaaql-middleware-python-4.9.1/jaaql_middleware_python.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        6 2023-05-06 14:40:09.000000 jaaql-middleware-python-4.9.1/jaaql_middleware_python.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-05-06 14:40:09.164515 jaaql-middleware-python-4.9.1/setup.cfg
+-rw-rw-rw-   0        0        0      893 2022-03-12 16:03:36.000000 jaaql-middleware-python-4.9.1/setup.py
```

### Comparing `jaaql-middleware-python-4.9.0/LICENSE.txt` & `jaaql-middleware-python-4.9.1/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `jaaql-middleware-python-4.9.0/PKG-INFO` & `jaaql-middleware-python-4.9.1/PKG-INFO`

 * *Files 17% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: jaaql-middleware-python
-Version: 4.9.0
+Version: 4.9.1
 Summary: The jaaql package, allowing for rapid development and deployment of RESTful HTTP applications
 Home-page: https://github.com/JAAQL/JAAQL-middleware-python
 Author: Software Quality Measurement and Improvement bv
 Author-email: aaron.tasker@sqmi.nl
 License: Mozilla Public License Version 2.0 with Commons Clause
 Platform: UNKNOWN
 Description-Content-Type: text/markdown
```

### Comparing `jaaql-middleware-python-4.9.0/jaaql/constants.py` & `jaaql-middleware-python-4.9.1/jaaql/constants.py`

 * *Files 0% similar despite different names*

```diff
@@ -125,9 +125,9 @@
 USERNAME__anonymous = "anonymous"
 PASSWORD__anonymous = "jaaql_public_password"
 ROLE__jaaql = "jaaql"
 ROLE__postgres = "postgres"
 
 PROTOCOL__postgres = "postgresql://"
 
-VERSION = "4.9.0"
+VERSION = "4.9.1"
```

### Comparing `jaaql-middleware-python-4.9.0/jaaql/db/db_interface.py` & `jaaql-middleware-python-4.9.1/jaaql/db/db_interface.py`

 * *Files identical despite different names*

### Comparing `jaaql-middleware-python-4.9.0/jaaql/db/db_pg_interface.py` & `jaaql-middleware-python-4.9.1/jaaql/db/db_pg_interface.py`

 * *Files identical despite different names*

### Comparing `jaaql-middleware-python-4.9.0/jaaql/db/db_utils.py` & `jaaql-middleware-python-4.9.1/jaaql/db/db_utils.py`

 * *Files identical despite different names*

### Comparing `jaaql-middleware-python-4.9.0/jaaql/db/db_utils_no_circ.py` & `jaaql-middleware-python-4.9.1/jaaql/db/db_utils_no_circ.py`

 * *Files identical despite different names*

### Comparing `jaaql-middleware-python-4.9.0/jaaql/documentation/documentation_internal.py` & `jaaql-middleware-python-4.9.1/jaaql/documentation/documentation_internal.py`

 * *Files identical despite different names*

### Comparing `jaaql-middleware-python-4.9.0/jaaql/documentation/documentation_public.py` & `jaaql-middleware-python-4.9.1/jaaql/documentation/documentation_public.py`

 * *Files identical despite different names*

### Comparing `jaaql-middleware-python-4.9.0/jaaql/documentation/documentation_shared.py` & `jaaql-middleware-python-4.9.1/jaaql/documentation/documentation_shared.py`

 * *Files identical despite different names*

### Comparing `jaaql-middleware-python-4.9.0/jaaql/email/email_manager.py` & `jaaql-middleware-python-4.9.1/jaaql/email/email_manager.py`

 * *Files identical despite different names*

### Comparing `jaaql-middleware-python-4.9.0/jaaql/email/email_manager_service.py` & `jaaql-middleware-python-4.9.1/jaaql/email/email_manager_service.py`

 * *Files identical despite different names*

### Comparing `jaaql-middleware-python-4.9.0/jaaql/exceptions/http_status_exception.py` & `jaaql-middleware-python-4.9.1/jaaql/exceptions/http_status_exception.py`

 * *Files identical despite different names*

### Comparing `jaaql-middleware-python-4.9.0/jaaql/interpreter/interpret_jaaql.py` & `jaaql-middleware-python-4.9.1/jaaql/interpreter/interpret_jaaql.py`

 * *Files identical despite different names*

### Comparing `jaaql-middleware-python-4.9.0/jaaql/jaaql.py` & `jaaql-middleware-python-4.9.1/jaaql/jaaql.py`

 * *Files identical despite different names*

### Comparing `jaaql-middleware-python-4.9.0/jaaql/migrations/migration_history.sql` & `jaaql-middleware-python-4.9.1/jaaql/migrations/migration_history.sql`

 * *Files identical despite different names*

### Comparing `jaaql-middleware-python-4.9.0/jaaql/migrations/migrations.py` & `jaaql-middleware-python-4.9.1/jaaql/migrations/migrations.py`

 * *Files identical despite different names*

### Comparing `jaaql-middleware-python-4.9.0/jaaql/mvc/base_controller.py` & `jaaql-middleware-python-4.9.1/jaaql/mvc/base_controller.py`

 * *Files identical despite different names*

### Comparing `jaaql-middleware-python-4.9.0/jaaql/mvc/base_model.py` & `jaaql-middleware-python-4.9.1/jaaql/mvc/base_model.py`

 * *Files identical despite different names*

### Comparing `jaaql-middleware-python-4.9.0/jaaql/mvc/controller.py` & `jaaql-middleware-python-4.9.1/jaaql/mvc/controller.py`

 * *Files identical despite different names*

### Comparing `jaaql-middleware-python-4.9.0/jaaql/mvc/exception_queries.py` & `jaaql-middleware-python-4.9.1/jaaql/mvc/exception_queries.py`

 * *Files identical despite different names*

### Comparing `jaaql-middleware-python-4.9.0/jaaql/mvc/generated_queries.py` & `jaaql-middleware-python-4.9.1/jaaql/mvc/generated_queries.py`

 * *Files identical despite different names*

### Comparing `jaaql-middleware-python-4.9.0/jaaql/mvc/model.py` & `jaaql-middleware-python-4.9.1/jaaql/mvc/model.py`

 * *Files identical despite different names*

### Comparing `jaaql-middleware-python-4.9.0/jaaql/openapi/swagger_documentation.py` & `jaaql-middleware-python-4.9.1/jaaql/openapi/swagger_documentation.py`

 * *Files identical despite different names*

### Comparing `jaaql-middleware-python-4.9.0/jaaql/scripts/01.install_domains.generated.sql` & `jaaql-middleware-python-4.9.1/jaaql/scripts/01.install_domains.generated.sql`

 * *Files identical despite different names*

### Comparing `jaaql-middleware-python-4.9.0/jaaql/scripts/02.install_super_user.exceptions.sql` & `jaaql-middleware-python-4.9.1/jaaql/scripts/02.install_super_user.exceptions.sql`

 * *Files identical despite different names*

### Comparing `jaaql-middleware-python-4.9.0/jaaql/scripts/03.install_super_user.handwritten.sql` & `jaaql-middleware-python-4.9.1/jaaql/scripts/03.install_super_user.handwritten.sql`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 CREATE EXTENSION IF NOT EXISTS pgcrypto;
 CREATE EXTENSION IF NOT EXISTS dblink;
 CREATE EXTENSION IF NOT EXISTS jaaql;
+CREATE EXTENSION IF NOT EXISTS plpgsql_check;
 
 create or replace function does_user_own_this_database(_user name, database object_name) returns boolean as
 $$
 DECLARE
     owner boolean;
 BEGIN
     SELECT (datdba::regrole)::text = _user::text into owner FROM pg_database WHERE datname = does_user_own_this_database.database;
```

### Comparing `jaaql-middleware-python-4.9.0/jaaql/scripts/04.install_jaaql_data_structures.generated.sql` & `jaaql-middleware-python-4.9.1/jaaql/scripts/04.install_jaaql_data_structures.generated.sql`

 * *Files identical despite different names*

### Comparing `jaaql-middleware-python-4.9.0/jaaql/scripts/06.install_jaaql.handwritten.sql` & `jaaql-middleware-python-4.9.1/jaaql/scripts/06.install_jaaql.handwritten.sql`

 * *Files identical despite different names*

### Comparing `jaaql-middleware-python-4.9.0/jaaql/scripts/swagger_template.html` & `jaaql-middleware-python-4.9.1/jaaql/scripts/swagger_template.html`

 * *Files identical despite different names*

### Comparing `jaaql-middleware-python-4.9.0/jaaql/services/cached_canned_query_service.py` & `jaaql-middleware-python-4.9.1/jaaql/services/cached_canned_query_service.py`

 * *Files identical despite different names*

### Comparing `jaaql-middleware-python-4.9.0/jaaql/services/migrations_manager_service.py` & `jaaql-middleware-python-4.9.1/jaaql/services/migrations_manager_service.py`

 * *Files identical despite different names*

### Comparing `jaaql-middleware-python-4.9.0/jaaql/utilities/crypt_utils.py` & `jaaql-middleware-python-4.9.1/jaaql/utilities/crypt_utils.py`

 * *Files identical despite different names*

### Comparing `jaaql-middleware-python-4.9.0/jaaql/utilities/options.py` & `jaaql-middleware-python-4.9.1/jaaql/utilities/options.py`

 * *Files identical despite different names*

### Comparing `jaaql-middleware-python-4.9.0/jaaql/utilities/utils.py` & `jaaql-middleware-python-4.9.1/jaaql/utilities/utils.py`

 * *Files identical despite different names*

### Comparing `jaaql-middleware-python-4.9.0/jaaql/utilities/utils_no_project_imports.py` & `jaaql-middleware-python-4.9.1/jaaql/utilities/utils_no_project_imports.py`

 * *Files identical despite different names*

### Comparing `jaaql-middleware-python-4.9.0/jaaql/utilities/vault.py` & `jaaql-middleware-python-4.9.1/jaaql/utilities/vault.py`

 * *Files identical despite different names*

### Comparing `jaaql-middleware-python-4.9.0/jaaql_middleware_python.egg-info/PKG-INFO` & `jaaql-middleware-python-4.9.1/jaaql_middleware_python.egg-info/PKG-INFO`

 * *Files 17% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: jaaql-middleware-python
-Version: 4.9.0
+Version: 4.9.1
 Summary: The jaaql package, allowing for rapid development and deployment of RESTful HTTP applications
 Home-page: https://github.com/JAAQL/JAAQL-middleware-python
 Author: Software Quality Measurement and Improvement bv
 Author-email: aaron.tasker@sqmi.nl
 License: Mozilla Public License Version 2.0 with Commons Clause
 Platform: UNKNOWN
 Description-Content-Type: text/markdown
```

### Comparing `jaaql-middleware-python-4.9.0/jaaql_middleware_python.egg-info/SOURCES.txt` & `jaaql-middleware-python-4.9.1/jaaql_middleware_python.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `jaaql-middleware-python-4.9.0/setup.py` & `jaaql-middleware-python-4.9.1/setup.py`

 * *Files identical despite different names*

