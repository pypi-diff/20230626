# Comparing `tmp/pypnusershub-1.6.7.tar.gz` & `tmp/pypnusershub-1.6.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pypnusershub-1.6.7.tar", last modified: Wed Jun  7 08:42:08 2023, max compression
+gzip compressed data, was "pypnusershub-1.6.8.tar", last modified: Mon Jun 26 14:39:58 2023, max compression
```

## Comparing `pypnusershub-1.6.7.tar` & `pypnusershub-1.6.8.tar`

### file list

```diff
@@ -1,56 +1,57 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 08:42:08.426686 pypnusershub-1.6.7/
--rw-r--r--   0 runner    (1001) docker     (123)    35141 2023-06-07 08:41:58.000000 pypnusershub-1.6.7/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      146 2023-06-07 08:41:58.000000 pypnusershub-1.6.7/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     8282 2023-06-07 08:42:08.426686 pypnusershub-1.6.7/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     7355 2023-06-07 08:41:58.000000 pypnusershub-1.6.7/README.md
--rw-r--r--   0 runner    (1001) docker     (123)        5 2023-06-07 08:41:58.000000 pypnusershub-1.6.7/VERSION
--rw-r--r--   0 runner    (1001) docker     (123)      176 2023-06-07 08:41:58.000000 pypnusershub-1.6.7/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)      124 2023-06-07 08:41:58.000000 pypnusershub-1.6.7/requirements-common.in
--rw-r--r--   0 runner    (1001) docker     (123)       35 2023-06-07 08:41:58.000000 pypnusershub-1.6.7/requirements-dependencies.in
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-07 08:42:08.426686 pypnusershub-1.6.7/setup.cfg
--rwxr-xr-x   0 runner    (1001) docker     (123)     1754 2023-06-07 08:41:58.000000 pypnusershub-1.6.7/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 08:42:08.410686 pypnusershub-1.6.7/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 08:42:08.418686 pypnusershub-1.6.7/src/pypnusershub/
--rw-r--r--   0 runner    (1001) docker     (123)       43 2023-06-07 08:41:58.000000 pypnusershub-1.6.7/src/pypnusershub/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2818 2023-06-07 08:41:58.000000 pypnusershub-1.6.7/src/pypnusershub/__main__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 08:42:08.422686 pypnusershub-1.6.7/src/pypnusershub/db/
--rw-r--r--   0 runner    (1001) docker     (123)       30 2023-06-07 08:41:58.000000 pypnusershub-1.6.7/src/pypnusershub/db/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4424 2023-06-07 08:41:58.000000 pypnusershub-1.6.7/src/pypnusershub/db/fixtures.sql
--rw-r--r--   0 runner    (1001) docker     (123)    13545 2023-06-07 08:41:58.000000 pypnusershub-1.6.7/src/pypnusershub/db/models.py
--rw-r--r--   0 runner    (1001) docker     (123)     4781 2023-06-07 08:41:58.000000 pypnusershub-1.6.7/src/pypnusershub/db/models_register.py
--rw-r--r--   0 runner    (1001) docker     (123)     3842 2023-06-07 08:41:58.000000 pypnusershub-1.6.7/src/pypnusershub/db/tools.py
--rw-r--r--   0 runner    (1001) docker     (123)      788 2023-06-07 08:41:58.000000 pypnusershub-1.6.7/src/pypnusershub/env.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 08:42:08.422686 pypnusershub-1.6.7/src/pypnusershub/migrations/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-07 08:41:58.000000 pypnusershub-1.6.7/src/pypnusershub/migrations/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 08:42:08.422686 pypnusershub-1.6.7/src/pypnusershub/migrations/data/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-07 08:41:58.000000 pypnusershub-1.6.7/src/pypnusershub/migrations/data/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3605 2023-06-07 08:41:58.000000 pypnusershub-1.6.7/src/pypnusershub/migrations/data/utilisateurs-samples.sql
--rw-r--r--   0 runner    (1001) docker     (123)    15812 2023-06-07 08:41:58.000000 pypnusershub-1.6.7/src/pypnusershub/migrations/data/utilisateurs.sql
--rw-r--r--   0 runner    (1001) docker     (123)     2180 2023-06-07 08:41:58.000000 pypnusershub-1.6.7/src/pypnusershub/migrations/env.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 08:42:08.426686 pypnusershub-1.6.7/src/pypnusershub/migrations/versions/
--rw-r--r--   0 runner    (1001) docker     (123)      806 2023-06-07 08:41:58.000000 pypnusershub-1.6.7/src/pypnusershub/migrations/versions/10e87bc144cd_get_id_role_by_name.py
--rw-r--r--   0 runner    (1001) docker     (123)      547 2023-06-07 08:41:58.000000 pypnusershub-1.6.7/src/pypnusershub/migrations/versions/112ccf1024ce_add_unique_constraint_on_t_roles_uuid.py
--rw-r--r--   0 runner    (1001) docker     (123)     5854 2023-06-07 08:41:58.000000 pypnusershub-1.6.7/src/pypnusershub/migrations/versions/5b334b77f5f5_fix_v_roleslist_forall_applications.py
--rw-r--r--   0 runner    (1001) docker     (123)      988 2023-06-07 08:41:58.000000 pypnusershub-1.6.7/src/pypnusershub/migrations/versions/72f227e37bdf_utilisateurs_sample_data.py
--rw-r--r--   0 runner    (1001) docker     (123)      668 2023-06-07 08:41:58.000000 pypnusershub-1.6.7/src/pypnusershub/migrations/versions/830cc8f4daef_add_additional_data_field_to_organism.py
--rw-r--r--   0 runner    (1001) docker     (123)      573 2023-06-07 08:41:58.000000 pypnusershub-1.6.7/src/pypnusershub/migrations/versions/951b8270a1cf_add_unique_constraint_on_uuid_organisme.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-07 08:41:58.000000 pypnusershub-1.6.7/src/pypnusershub/migrations/versions/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      530 2023-06-07 08:41:58.000000 pypnusershub-1.6.7/src/pypnusershub/migrations/versions/fa35dfe5ff27_create_utilisateurs_schema.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    10925 2023-06-07 08:41:58.000000 pypnusershub-1.6.7/src/pypnusershub/routes.py
--rw-r--r--   0 runner    (1001) docker     (123)     6677 2023-06-07 08:41:58.000000 pypnusershub-1.6.7/src/pypnusershub/routes_register.py
--rw-r--r--   0 runner    (1001) docker     (123)      953 2023-06-07 08:41:58.000000 pypnusershub-1.6.7/src/pypnusershub/schemas.py
--rw-r--r--   0 runner    (1001) docker     (123)       78 2023-06-07 08:41:58.000000 pypnusershub-1.6.7/src/pypnusershub/test_settings.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 08:42:08.426686 pypnusershub-1.6.7/src/pypnusershub/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-07 08:41:58.000000 pypnusershub-1.6.7/src/pypnusershub/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      558 2023-06-07 08:41:58.000000 pypnusershub-1.6.7/src/pypnusershub/tests/conftest.py
--rw-r--r--   0 runner    (1001) docker     (123)     2033 2023-06-07 08:41:58.000000 pypnusershub-1.6.7/src/pypnusershub/tests/fixtures.py
--rw-r--r--   0 runner    (1001) docker     (123)     2262 2023-06-07 08:41:58.000000 pypnusershub-1.6.7/src/pypnusershub/tests/test_utilisateurs.py
--rw-r--r--   0 runner    (1001) docker     (123)     1035 2023-06-07 08:41:58.000000 pypnusershub-1.6.7/src/pypnusershub/tests/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     2777 2023-06-07 08:41:58.000000 pypnusershub-1.6.7/src/pypnusershub/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 08:42:08.418686 pypnusershub-1.6.7/src/pypnusershub.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     8282 2023-06-07 08:42:08.000000 pypnusershub-1.6.7/src/pypnusershub.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1804 2023-06-07 08:42:08.000000 pypnusershub-1.6.7/src/pypnusershub.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-07 08:42:08.000000 pypnusershub-1.6.7/src/pypnusershub.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       56 2023-06-07 08:42:08.000000 pypnusershub-1.6.7/src/pypnusershub.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)      188 2023-06-07 08:42:08.000000 pypnusershub-1.6.7/src/pypnusershub.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       13 2023-06-07 08:42:08.000000 pypnusershub-1.6.7/src/pypnusershub.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 14:39:58.839547 pypnusershub-1.6.8/
+-rw-r--r--   0 runner    (1001) docker     (123)    35141 2023-06-26 14:39:44.000000 pypnusershub-1.6.8/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      146 2023-06-26 14:39:44.000000 pypnusershub-1.6.8/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     8282 2023-06-26 14:39:58.839547 pypnusershub-1.6.8/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     7355 2023-06-26 14:39:44.000000 pypnusershub-1.6.8/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)        5 2023-06-26 14:39:44.000000 pypnusershub-1.6.8/VERSION
+-rw-r--r--   0 runner    (1001) docker     (123)      176 2023-06-26 14:39:44.000000 pypnusershub-1.6.8/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      124 2023-06-26 14:39:44.000000 pypnusershub-1.6.8/requirements-common.in
+-rw-r--r--   0 runner    (1001) docker     (123)       35 2023-06-26 14:39:44.000000 pypnusershub-1.6.8/requirements-dependencies.in
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-26 14:39:58.839547 pypnusershub-1.6.8/setup.cfg
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1754 2023-06-26 14:39:44.000000 pypnusershub-1.6.8/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 14:39:58.827547 pypnusershub-1.6.8/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 14:39:58.831548 pypnusershub-1.6.8/src/pypnusershub/
+-rw-r--r--   0 runner    (1001) docker     (123)       43 2023-06-26 14:39:44.000000 pypnusershub-1.6.8/src/pypnusershub/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2818 2023-06-26 14:39:44.000000 pypnusershub-1.6.8/src/pypnusershub/__main__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 14:39:58.835548 pypnusershub-1.6.8/src/pypnusershub/db/
+-rw-r--r--   0 runner    (1001) docker     (123)       30 2023-06-26 14:39:44.000000 pypnusershub-1.6.8/src/pypnusershub/db/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4424 2023-06-26 14:39:44.000000 pypnusershub-1.6.8/src/pypnusershub/db/fixtures.sql
+-rw-r--r--   0 runner    (1001) docker     (123)    13545 2023-06-26 14:39:44.000000 pypnusershub-1.6.8/src/pypnusershub/db/models.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4781 2023-06-26 14:39:44.000000 pypnusershub-1.6.8/src/pypnusershub/db/models_register.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3842 2023-06-26 14:39:44.000000 pypnusershub-1.6.8/src/pypnusershub/db/tools.py
+-rw-r--r--   0 runner    (1001) docker     (123)      788 2023-06-26 14:39:44.000000 pypnusershub-1.6.8/src/pypnusershub/env.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 14:39:58.835548 pypnusershub-1.6.8/src/pypnusershub/migrations/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-26 14:39:44.000000 pypnusershub-1.6.8/src/pypnusershub/migrations/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 14:39:58.835548 pypnusershub-1.6.8/src/pypnusershub/migrations/data/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-26 14:39:44.000000 pypnusershub-1.6.8/src/pypnusershub/migrations/data/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3605 2023-06-26 14:39:44.000000 pypnusershub-1.6.8/src/pypnusershub/migrations/data/utilisateurs-samples.sql
+-rw-r--r--   0 runner    (1001) docker     (123)    15812 2023-06-26 14:39:44.000000 pypnusershub-1.6.8/src/pypnusershub/migrations/data/utilisateurs.sql
+-rw-r--r--   0 runner    (1001) docker     (123)     2180 2023-06-26 14:39:44.000000 pypnusershub-1.6.8/src/pypnusershub/migrations/env.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 14:39:58.835548 pypnusershub-1.6.8/src/pypnusershub/migrations/versions/
+-rw-r--r--   0 runner    (1001) docker     (123)      806 2023-06-26 14:39:44.000000 pypnusershub-1.6.8/src/pypnusershub/migrations/versions/10e87bc144cd_get_id_role_by_name.py
+-rw-r--r--   0 runner    (1001) docker     (123)      547 2023-06-26 14:39:44.000000 pypnusershub-1.6.8/src/pypnusershub/migrations/versions/112ccf1024ce_add_unique_constraint_on_t_roles_uuid.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5854 2023-06-26 14:39:44.000000 pypnusershub-1.6.8/src/pypnusershub/migrations/versions/5b334b77f5f5_fix_v_roleslist_forall_applications.py
+-rw-r--r--   0 runner    (1001) docker     (123)      988 2023-06-26 14:39:44.000000 pypnusershub-1.6.8/src/pypnusershub/migrations/versions/72f227e37bdf_utilisateurs_sample_data.py
+-rw-r--r--   0 runner    (1001) docker     (123)      668 2023-06-26 14:39:44.000000 pypnusershub-1.6.8/src/pypnusershub/migrations/versions/830cc8f4daef_add_additional_data_field_to_organism.py
+-rw-r--r--   0 runner    (1001) docker     (123)      573 2023-06-26 14:39:44.000000 pypnusershub-1.6.8/src/pypnusershub/migrations/versions/951b8270a1cf_add_unique_constraint_on_uuid_organisme.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-26 14:39:44.000000 pypnusershub-1.6.8/src/pypnusershub/migrations/versions/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      530 2023-06-26 14:39:44.000000 pypnusershub-1.6.8/src/pypnusershub/migrations/versions/fa35dfe5ff27_create_utilisateurs_schema.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    11397 2023-06-26 14:39:44.000000 pypnusershub-1.6.8/src/pypnusershub/routes.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6677 2023-06-26 14:39:44.000000 pypnusershub-1.6.8/src/pypnusershub/routes_register.py
+-rw-r--r--   0 runner    (1001) docker     (123)      953 2023-06-26 14:39:44.000000 pypnusershub-1.6.8/src/pypnusershub/schemas.py
+-rw-r--r--   0 runner    (1001) docker     (123)       78 2023-06-26 14:39:44.000000 pypnusershub-1.6.8/src/pypnusershub/test_settings.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 14:39:58.835548 pypnusershub-1.6.8/src/pypnusershub/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-26 14:39:44.000000 pypnusershub-1.6.8/src/pypnusershub/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      558 2023-06-26 14:39:44.000000 pypnusershub-1.6.8/src/pypnusershub/tests/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2033 2023-06-26 14:39:44.000000 pypnusershub-1.6.8/src/pypnusershub/tests/fixtures.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2262 2023-06-26 14:39:44.000000 pypnusershub-1.6.8/src/pypnusershub/tests/test_utilisateurs.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1256 2023-06-26 14:39:44.000000 pypnusershub-1.6.8/src/pypnusershub/tests/test_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1035 2023-06-26 14:39:44.000000 pypnusershub-1.6.8/src/pypnusershub/tests/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3455 2023-06-26 14:39:44.000000 pypnusershub-1.6.8/src/pypnusershub/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 14:39:58.831548 pypnusershub-1.6.8/src/pypnusershub.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     8282 2023-06-26 14:39:58.000000 pypnusershub-1.6.8/src/pypnusershub.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1841 2023-06-26 14:39:58.000000 pypnusershub-1.6.8/src/pypnusershub.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-26 14:39:58.000000 pypnusershub-1.6.8/src/pypnusershub.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       56 2023-06-26 14:39:58.000000 pypnusershub-1.6.8/src/pypnusershub.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      188 2023-06-26 14:39:58.000000 pypnusershub-1.6.8/src/pypnusershub.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       13 2023-06-26 14:39:58.000000 pypnusershub-1.6.8/src/pypnusershub.egg-info/top_level.txt
```

### Comparing `pypnusershub-1.6.7/LICENSE` & `pypnusershub-1.6.8/LICENSE`

 * *Files identical despite different names*

### Comparing `pypnusershub-1.6.7/PKG-INFO` & `pypnusershub-1.6.8/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pypnusershub
-Version: 1.6.7
+Version: 1.6.8
 Summary: Python lib to authenticate using PN's UsersHub
 Home-page: https://github.com/PnX-SI/UsersHub-authentification-module
 Maintainer: Parcs nationaux des Écrins et des Cévennes
 Maintainer-email: geonature@ecrins-parcnational.fr
 Classifier: Development Status :: 1 - Planning
 Classifier: Intended Audience :: Developers
 Classifier: Natural Language :: English
```

### Comparing `pypnusershub-1.6.7/README.md` & `pypnusershub-1.6.8/README.md`

 * *Files identical despite different names*

### Comparing `pypnusershub-1.6.7/setup.py` & `pypnusershub-1.6.8/setup.py`

 * *Files identical despite different names*

### Comparing `pypnusershub-1.6.7/src/pypnusershub/__main__.py` & `pypnusershub-1.6.8/src/pypnusershub/__main__.py`

 * *Files identical despite different names*

### Comparing `pypnusershub-1.6.7/src/pypnusershub/db/fixtures.sql` & `pypnusershub-1.6.8/src/pypnusershub/db/fixtures.sql`

 * *Files identical despite different names*

### Comparing `pypnusershub-1.6.7/src/pypnusershub/db/models.py` & `pypnusershub-1.6.8/src/pypnusershub/db/models.py`

 * *Files identical despite different names*

### Comparing `pypnusershub-1.6.7/src/pypnusershub/db/models_register.py` & `pypnusershub-1.6.8/src/pypnusershub/db/models_register.py`

 * *Files identical despite different names*

### Comparing `pypnusershub-1.6.7/src/pypnusershub/db/tools.py` & `pypnusershub-1.6.8/src/pypnusershub/db/tools.py`

 * *Files identical despite different names*

### Comparing `pypnusershub-1.6.7/src/pypnusershub/env.py` & `pypnusershub-1.6.8/src/pypnusershub/env.py`

 * *Files identical despite different names*

### Comparing `pypnusershub-1.6.7/src/pypnusershub/migrations/data/utilisateurs-samples.sql` & `pypnusershub-1.6.8/src/pypnusershub/migrations/data/utilisateurs-samples.sql`

 * *Files identical despite different names*

### Comparing `pypnusershub-1.6.7/src/pypnusershub/migrations/data/utilisateurs.sql` & `pypnusershub-1.6.8/src/pypnusershub/migrations/data/utilisateurs.sql`

 * *Files identical despite different names*

### Comparing `pypnusershub-1.6.7/src/pypnusershub/migrations/env.py` & `pypnusershub-1.6.8/src/pypnusershub/migrations/env.py`

 * *Files identical despite different names*

### Comparing `pypnusershub-1.6.7/src/pypnusershub/migrations/versions/10e87bc144cd_get_id_role_by_name.py` & `pypnusershub-1.6.8/src/pypnusershub/migrations/versions/10e87bc144cd_get_id_role_by_name.py`

 * *Files identical despite different names*

### Comparing `pypnusershub-1.6.7/src/pypnusershub/migrations/versions/112ccf1024ce_add_unique_constraint_on_t_roles_uuid.py` & `pypnusershub-1.6.8/src/pypnusershub/migrations/versions/112ccf1024ce_add_unique_constraint_on_t_roles_uuid.py`

 * *Files identical despite different names*

### Comparing `pypnusershub-1.6.7/src/pypnusershub/migrations/versions/5b334b77f5f5_fix_v_roleslist_forall_applications.py` & `pypnusershub-1.6.8/src/pypnusershub/migrations/versions/5b334b77f5f5_fix_v_roleslist_forall_applications.py`

 * *Files identical despite different names*

### Comparing `pypnusershub-1.6.7/src/pypnusershub/migrations/versions/72f227e37bdf_utilisateurs_sample_data.py` & `pypnusershub-1.6.8/src/pypnusershub/migrations/versions/72f227e37bdf_utilisateurs_sample_data.py`

 * *Files identical despite different names*

### Comparing `pypnusershub-1.6.7/src/pypnusershub/migrations/versions/830cc8f4daef_add_additional_data_field_to_organism.py` & `pypnusershub-1.6.8/src/pypnusershub/migrations/versions/830cc8f4daef_add_additional_data_field_to_organism.py`

 * *Files identical despite different names*

### Comparing `pypnusershub-1.6.7/src/pypnusershub/migrations/versions/951b8270a1cf_add_unique_constraint_on_uuid_organisme.py` & `pypnusershub-1.6.8/src/pypnusershub/migrations/versions/951b8270a1cf_add_unique_constraint_on_uuid_organisme.py`

 * *Files identical despite different names*

### Comparing `pypnusershub-1.6.7/src/pypnusershub/migrations/versions/fa35dfe5ff27_create_utilisateurs_schema.py` & `pypnusershub-1.6.8/src/pypnusershub/migrations/versions/fa35dfe5ff27_create_utilisateurs_schema.py`

 * *Files identical despite different names*

### Comparing `pypnusershub-1.6.7/src/pypnusershub/routes.py` & `pypnusershub-1.6.8/src/pypnusershub/routes.py`

 * *Files 4% similar despite different names*

```diff
@@ -25,15 +25,15 @@
     session,
 )
 
 from sqlalchemy.orm import exc
 import sqlalchemy as sa
 from werkzeug.exceptions import BadRequest, Forbidden
 
-from pypnusershub.utils import get_current_app_id
+from pypnusershub.utils import get_current_app_id, set_cookie
 from pypnusershub.db import models, db
 from pypnusershub.db.tools import (
     user_to_token,
     user_from_token,
     UnreadableAccessRightsError,
     AccessRightsExpiredError,
 )
@@ -76,28 +76,24 @@
         app.config["PASS_METHOD"] = app.config.get("PASS_METHOD", "hash")
 
         if cookie_autorenew:
 
             @app.after_request
             def after_request(response):
                 try:
-                    set_cookie = response.headers.get("Set-Cookie", "")
-                    is_setting_token = set_cookie.startswith("token=")
+                    cookie_set = response.headers.get("Set-Cookie", "")
+                    is_setting_token = cookie_set.startswith("token=")
                     is_token_set = request.cookies.get("token")
                     if is_token_set and not is_setting_token:
                         cookie_exp = datetime.datetime.utcnow()
                         cookie_exp += datetime.timedelta(seconds=expiration)
-                        response.set_cookie(
-                            "token", request.cookies["token"], expires=cookie_exp
-                        )
-                        response.set_cookie(
-                            "currentUser",
-                            request.cookies["currentUser"],
-                            expires=cookie_exp,
-                        )
+                        set_cookie(response=response, application_url=current_app.config.get("URL_APPLICATION"),
+                                   key="token", value=request.cookies["token"], expires=cookie_exp)
+                        set_cookie(response=response, application_url=current_app.config.get("URL_APPLICATION"),
+                                   key="currentUser", value=request.cookies["currentUser"], expires=cookie_exp)
                     return response
                 # TODO: replace the generic exception by a specific one
                 except Exception:
                     return response
 
         parent = super(ConfigurableBlueprint, self)
         parent.register(app, *args, **kwargs)
@@ -135,15 +131,16 @@
                 return fn(*args, **kwargs)
 
             except AccessRightsExpiredError:
                 if redirect_on_expiration:
                     res = redirect(redirect_on_expiration, code=302)
                 else:
                     res = Response("Token Expired", 403)
-                res.set_cookie("token", "", expires=0)
+                set_cookie(response=res, application_url=current_app.config.get("URL_APPLICATION"),
+                   key="token", value="", expires=0)
                 return res
 
             except KeyError as e:
                 if "token" not in e.args:
                     raise
                 if redirect_on_expiration:
                     return redirect(redirect_on_expiration, code=302)
@@ -154,15 +151,16 @@
                 # invalid token
                 if redirect_on_invalid_token:
                     res = redirect(redirect_on_invalid_token, code=302)
                 else:
                     res = Response(
                         "Token BadSignature or token not coresponding to the app", 403
                     )
-                res.set_cookie("token", "", expires=0)
+                set_cookie(response=res, application_url=current_app.config.get("URL_APPLICATION"),
+                            key="token", value="", expires=0)
                 return res
 
             except Exception as e:
                 trap_all_exceptions = current_app.config.get(
                     "TRAP_ALL_EXCEPTIONS", True
                 )
                 if not trap_all_exceptions:
@@ -239,15 +237,16 @@
         # Génération d'un token
         token = user_to_token(user)
         cookie_exp = datetime.datetime.utcnow()
         cookie_exp += datetime.timedelta(
             seconds=current_app.config["COOKIE_EXPIRATION"]
         )
         resp = Response(json.dumps({"user": user_dict, "expires": str(cookie_exp)}))
-        resp.set_cookie("token", token, expires=cookie_exp)
+        set_cookie(response=resp, application_url=current_app.config.get("URL_APPLICATION"),
+                   key="token", value=token, expires=cookie_exp)
 
         return resp
     except Exception as e:
         msg = json.dumps({"login": False, "msg": repr(e)})
         return Response(msg, status=403)
 
 @routes.route("/public_login", methods=["POST"])
@@ -265,15 +264,16 @@
     # Génération d'un token
     token = user_to_token(user)
     cookie_exp = datetime.datetime.utcnow()
     cookie_exp += datetime.timedelta(
         seconds=current_app.config["COOKIE_EXPIRATION"]
     )
     resp = Response(json.dumps({"user": user_dict, "expires": str(cookie_exp)}))
-    resp.set_cookie("token", token, expires=cookie_exp)
+    set_cookie(response=resp, application_url=current_app.config.get("URL_APPLICATION"),
+               key="token", value=token, expires=cookie_exp)
 
     return resp
 
 @routes.route("/logout", methods=["GET", "POST"])
 def logout():
     params = request.args
     if "redirect" in params:
```

### Comparing `pypnusershub-1.6.7/src/pypnusershub/routes_register.py` & `pypnusershub-1.6.8/src/pypnusershub/routes_register.py`

 * *Files identical despite different names*

### Comparing `pypnusershub-1.6.7/src/pypnusershub/schemas.py` & `pypnusershub-1.6.8/src/pypnusershub/schemas.py`

 * *Files identical despite different names*

### Comparing `pypnusershub-1.6.7/src/pypnusershub/tests/conftest.py` & `pypnusershub-1.6.8/src/pypnusershub/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `pypnusershub-1.6.7/src/pypnusershub/tests/fixtures.py` & `pypnusershub-1.6.8/src/pypnusershub/tests/fixtures.py`

 * *Files identical despite different names*

### Comparing `pypnusershub-1.6.7/src/pypnusershub/tests/test_utilisateurs.py` & `pypnusershub-1.6.8/src/pypnusershub/tests/test_utilisateurs.py`

 * *Files identical despite different names*

### Comparing `pypnusershub-1.6.7/src/pypnusershub/tests/utils.py` & `pypnusershub-1.6.8/src/pypnusershub/tests/utils.py`

 * *Files identical despite different names*

### Comparing `pypnusershub-1.6.7/src/pypnusershub/utils.py` & `pypnusershub-1.6.8/src/pypnusershub/utils.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,21 +1,22 @@
 # coding: utf8
 
-from __future__ import (unicode_literals, print_function,
-                        absolute_import, division)
+from __future__ import unicode_literals, print_function, absolute_import, division
 
 """
     Collections of utilities unrelated to the main module purpose.
 """
 
 import os
 import io
 from types import ModuleType
+from typing import Optional
+from urllib.parse import urlsplit
 
-from flask import current_app
+from flask import current_app, Response
 
 
 class RessourceError(EnvironmentError):
 
     def __init__(self, msg, errors):
         super(RessourceError, self).__init__(msg)
         self.errors = errors
@@ -80,7 +81,28 @@
                 code_application=current_app.config['CODE_APPLICATION'],
             )
             .one()
             .id_application
         )
     else:
         return None
+
+
+def get_cookie_path(application_url: Optional[str] = None) -> str:
+    """
+    Returns the cookie path computed from the application_url
+    """
+    if application_url is None:
+        return "/"
+    split_url = urlsplit(application_url)
+    return split_url.path if split_url.path else "/"
+
+
+def set_cookie(response: Response, application_url: Optional[str] = None, **kwargs):
+    """
+    Set automatically a Path on a cookie.
+    All kwargs are passed to Response.set_cookie()
+    """
+    cookie_path = get_cookie_path(application_url=application_url)
+    response.set_cookie(**kwargs, path=cookie_path)
+    return response
+
```

### Comparing `pypnusershub-1.6.7/src/pypnusershub.egg-info/PKG-INFO` & `pypnusershub-1.6.8/src/pypnusershub.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pypnusershub
-Version: 1.6.7
+Version: 1.6.8
 Summary: Python lib to authenticate using PN's UsersHub
 Home-page: https://github.com/PnX-SI/UsersHub-authentification-module
 Maintainer: Parcs nationaux des Écrins et des Cévennes
 Maintainer-email: geonature@ecrins-parcnational.fr
 Classifier: Development Status :: 1 - Planning
 Classifier: Intended Audience :: Developers
 Classifier: Natural Language :: English
```

### Comparing `pypnusershub-1.6.7/src/pypnusershub.egg-info/SOURCES.txt` & `pypnusershub-1.6.8/src/pypnusershub.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -38,8 +38,9 @@
 src/pypnusershub/migrations/versions/951b8270a1cf_add_unique_constraint_on_uuid_organisme.py
 src/pypnusershub/migrations/versions/__init__.py
 src/pypnusershub/migrations/versions/fa35dfe5ff27_create_utilisateurs_schema.py
 src/pypnusershub/tests/__init__.py
 src/pypnusershub/tests/conftest.py
 src/pypnusershub/tests/fixtures.py
 src/pypnusershub/tests/test_utilisateurs.py
+src/pypnusershub/tests/test_utils.py
 src/pypnusershub/tests/utils.py
```

