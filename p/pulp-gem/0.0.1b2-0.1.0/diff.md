# Comparing `tmp/pulp-gem-0.0.1b2.tar.gz` & `tmp/pulp-gem-0.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/pulp-gem-0.0.1b2.tar", last modified: Wed Dec 19 10:05:01 2018, max compression
+gzip compressed data, was "pulp-gem-0.1.0.tar", last modified: Mon Jun 26 19:17:57 2023, max compression
```

## Comparing `pulp-gem-0.0.1b2.tar` & `pulp-gem-0.1.0.tar`

### file list

```diff
@@ -1,47 +1,68 @@
-drwxr-xr-x   0 matthiasd  (1000) matthiasd  (1000)        0 2018-12-19 10:05:01.000000 pulp-gem-0.0.1b2/
--rw-r--r--   0 matthiasd  (1000) matthiasd  (1000)      657 2018-02-21 08:44:39.000000 pulp-gem-0.0.1b2/COPYRIGHT
--rw-r--r--   0 matthiasd  (1000) matthiasd  (1000)    18046 2018-12-18 14:47:48.000000 pulp-gem-0.0.1b2/LICENSE
--rw-r--r--   0 matthiasd  (1000) matthiasd  (1000)       26 2018-05-31 16:00:57.000000 pulp-gem-0.0.1b2/MANIFEST.in
--rw-r--r--   0 matthiasd  (1000) matthiasd  (1000)     6092 2018-12-19 10:05:01.000000 pulp-gem-0.0.1b2/PKG-INFO
--rw-r--r--   0 matthiasd  (1000) matthiasd  (1000)     4347 2018-12-19 09:58:47.000000 pulp-gem-0.0.1b2/README.rst
-drwxr-xr-x   0 matthiasd  (1000) matthiasd  (1000)        0 2018-12-19 10:05:01.000000 pulp-gem-0.0.1b2/pulp_gem/
--rw-r--r--   0 matthiasd  (1000) matthiasd  (1000)       59 2018-02-15 14:19:07.000000 pulp-gem-0.0.1b2/pulp_gem/__init__.py
-drwxr-xr-x   0 matthiasd  (1000) matthiasd  (1000)        0 2018-12-19 10:05:01.000000 pulp-gem-0.0.1b2/pulp_gem/app/
--rw-r--r--   0 matthiasd  (1000) matthiasd  (1000)      205 2018-12-03 17:32:33.000000 pulp-gem-0.0.1b2/pulp_gem/app/__init__.py
-drwxr-xr-x   0 matthiasd  (1000) matthiasd  (1000)        0 2018-12-19 10:05:01.000000 pulp-gem-0.0.1b2/pulp_gem/app/migrations/
--rw-rw-r--   0 matthiasd  (1000) matthiasd  (1000)     1690 2018-12-17 10:20:35.000000 pulp-gem-0.0.1b2/pulp_gem/app/migrations/0001_initial.py
--rw-r--r--   0 matthiasd  (1000) matthiasd  (1000)        0 2018-07-01 07:54:41.000000 pulp-gem-0.0.1b2/pulp_gem/app/migrations/__init__.py
--rw-r--r--   0 matthiasd  (1000) matthiasd  (1000)      817 2018-12-18 14:47:48.000000 pulp-gem-0.0.1b2/pulp_gem/app/models.py
--rw-r--r--   0 matthiasd  (1000) matthiasd  (1000)     1056 2018-12-18 14:47:48.000000 pulp-gem-0.0.1b2/pulp_gem/app/serializers.py
-drwxr-xr-x   0 matthiasd  (1000) matthiasd  (1000)        0 2018-12-19 10:05:01.000000 pulp-gem-0.0.1b2/pulp_gem/app/tasks/
--rw-r--r--   0 matthiasd  (1000) matthiasd  (1000)       87 2018-05-03 19:36:34.000000 pulp-gem-0.0.1b2/pulp_gem/app/tasks/__init__.py
--rw-r--r--   0 matthiasd  (1000) matthiasd  (1000)     3346 2018-12-18 14:47:48.000000 pulp-gem-0.0.1b2/pulp_gem/app/tasks/publishing.py
--rw-r--r--   0 matthiasd  (1000) matthiasd  (1000)     5823 2018-12-18 14:47:48.000000 pulp-gem-0.0.1b2/pulp_gem/app/tasks/synchronizing.py
--rw-r--r--   0 matthiasd  (1000) matthiasd  (1000)     5968 2018-12-19 09:48:35.000000 pulp-gem-0.0.1b2/pulp_gem/app/viewsets.py
--rw-r--r--   0 matthiasd  (1000) matthiasd  (1000)     1836 2018-12-04 14:35:08.000000 pulp-gem-0.0.1b2/pulp_gem/specs.py
-drwxr-xr-x   0 matthiasd  (1000) matthiasd  (1000)        0 2018-12-19 10:05:01.000000 pulp-gem-0.0.1b2/pulp_gem/tests/
--rw-r--r--   0 matthiasd  (1000) matthiasd  (1000)        0 2018-12-03 17:32:33.000000 pulp-gem-0.0.1b2/pulp_gem/tests/__init__.py
-drwxr-xr-x   0 matthiasd  (1000) matthiasd  (1000)        0 2018-12-19 10:05:01.000000 pulp-gem-0.0.1b2/pulp_gem/tests/functional/
--rw-r--r--   0 matthiasd  (1000) matthiasd  (1000)       43 2018-12-03 17:32:33.000000 pulp-gem-0.0.1b2/pulp_gem/tests/functional/__init__.py
-drwxr-xr-x   0 matthiasd  (1000) matthiasd  (1000)        0 2018-12-19 10:05:01.000000 pulp-gem-0.0.1b2/pulp_gem/tests/functional/api/
--rw-r--r--   0 matthiasd  (1000) matthiasd  (1000)       76 2018-12-03 17:32:33.000000 pulp-gem-0.0.1b2/pulp_gem/tests/functional/api/__init__.py
--rw-r--r--   0 matthiasd  (1000) matthiasd  (1000)     3948 2018-12-18 14:47:48.000000 pulp-gem-0.0.1b2/pulp_gem/tests/functional/api/test_crud_content_unit.py
--rw-r--r--   0 matthiasd  (1000) matthiasd  (1000)     3665 2018-12-03 17:32:33.000000 pulp-gem-0.0.1b2/pulp_gem/tests/functional/api/test_crud_publishers.py
--rw-r--r--   0 matthiasd  (1000) matthiasd  (1000)     4689 2018-12-18 14:47:48.000000 pulp-gem-0.0.1b2/pulp_gem/tests/functional/api/test_crud_remotes.py
--rw-r--r--   0 matthiasd  (1000) matthiasd  (1000)     3601 2018-12-04 15:14:05.000000 pulp-gem-0.0.1b2/pulp_gem/tests/functional/api/test_download_content.py
--rw-r--r--   0 matthiasd  (1000) matthiasd  (1000)     3358 2018-12-18 14:47:48.000000 pulp-gem-0.0.1b2/pulp_gem/tests/functional/api/test_publish.py
--rw-r--r--   0 matthiasd  (1000) matthiasd  (1000)     4532 2018-12-18 14:47:48.000000 pulp-gem-0.0.1b2/pulp_gem/tests/functional/api/test_sync.py
--rw-r--r--   0 matthiasd  (1000) matthiasd  (1000)     1017 2018-12-18 14:47:48.000000 pulp-gem-0.0.1b2/pulp_gem/tests/functional/constants.py
--rw-r--r--   0 matthiasd  (1000) matthiasd  (1000)     3378 2018-12-18 14:47:48.000000 pulp-gem-0.0.1b2/pulp_gem/tests/functional/utils.py
-drwxr-xr-x   0 matthiasd  (1000) matthiasd  (1000)        0 2018-12-19 10:05:01.000000 pulp-gem-0.0.1b2/pulp_gem/tests/unit/
--rw-r--r--   0 matthiasd  (1000) matthiasd  (1000)        0 2018-12-03 17:32:33.000000 pulp-gem-0.0.1b2/pulp_gem/tests/unit/__init__.py
--rw-r--r--   0 matthiasd  (1000) matthiasd  (1000)      229 2018-12-03 17:32:33.000000 pulp-gem-0.0.1b2/pulp_gem/tests/unit/test_models.py
-drwxr-xr-x   0 matthiasd  (1000) matthiasd  (1000)        0 2018-12-19 10:05:01.000000 pulp-gem-0.0.1b2/pulp_gem.egg-info/
--rw-r--r--   0 matthiasd  (1000) matthiasd  (1000)     6092 2018-12-19 10:05:01.000000 pulp-gem-0.0.1b2/pulp_gem.egg-info/PKG-INFO
--rw-r--r--   0 matthiasd  (1000) matthiasd  (1000)     1112 2018-12-19 10:05:01.000000 pulp-gem-0.0.1b2/pulp_gem.egg-info/SOURCES.txt
--rw-r--r--   0 matthiasd  (1000) matthiasd  (1000)        1 2018-12-19 10:05:01.000000 pulp-gem-0.0.1b2/pulp_gem.egg-info/dependency_links.txt
--rw-r--r--   0 matthiasd  (1000) matthiasd  (1000)       58 2018-12-19 10:05:01.000000 pulp-gem-0.0.1b2/pulp_gem.egg-info/entry_points.txt
--rw-r--r--   0 matthiasd  (1000) matthiasd  (1000)       38 2018-12-19 10:05:01.000000 pulp-gem-0.0.1b2/pulp_gem.egg-info/requires.txt
--rw-r--r--   0 matthiasd  (1000) matthiasd  (1000)        9 2018-12-19 10:05:01.000000 pulp-gem-0.0.1b2/pulp_gem.egg-info/top_level.txt
--rw-r--r--   0 matthiasd  (1000) matthiasd  (1000)       38 2018-12-19 10:05:01.000000 pulp-gem-0.0.1b2/setup.cfg
--rwxr-xr-x   0 matthiasd  (1000) matthiasd  (1000)     1146 2018-12-19 09:37:39.000000 pulp-gem-0.0.1b2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 19:17:57.242227 pulp-gem-0.1.0/
+-rw-r--r--   0 runner    (1001) docker     (123)     2097 2023-06-26 19:17:43.000000 pulp-gem-0.1.0/CHANGES.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     2095 2023-06-26 19:17:43.000000 pulp-gem-0.1.0/COMMITMENT
+-rw-r--r--   0 runner    (1001) docker     (123)      657 2023-06-26 19:17:43.000000 pulp-gem-0.1.0/COPYRIGHT
+-rw-r--r--   0 runner    (1001) docker     (123)    18046 2023-06-26 19:17:43.000000 pulp-gem-0.1.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      237 2023-06-26 19:17:43.000000 pulp-gem-0.1.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     1089 2023-06-26 19:17:57.242227 pulp-gem-0.1.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      183 2023-06-26 19:17:43.000000 pulp-gem-0.1.0/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      122 2023-06-26 19:17:43.000000 pulp-gem-0.1.0/functest_requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 19:17:57.238227 pulp-gem-0.1.0/pulp_gem/
+-rw-r--r--   0 runner    (1001) docker     (123)       59 2023-06-26 19:17:43.000000 pulp-gem-0.1.0/pulp_gem/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 19:17:57.242227 pulp-gem-0.1.0/pulp_gem/app/
+-rw-r--r--   0 runner    (1001) docker     (123)      247 2023-06-26 19:17:55.000000 pulp-gem-0.1.0/pulp_gem/app/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 19:17:57.242227 pulp-gem-0.1.0/pulp_gem/app/management/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-26 19:17:43.000000 pulp-gem-0.1.0/pulp_gem/app/management/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 19:17:57.242227 pulp-gem-0.1.0/pulp_gem/app/management/commands/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-26 19:17:43.000000 pulp-gem-0.1.0/pulp_gem/app/management/commands/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2226 2023-06-26 19:17:43.000000 pulp-gem-0.1.0/pulp_gem/app/management/commands/datarepair-shallow-gems.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 19:17:57.242227 pulp-gem-0.1.0/pulp_gem/app/migrations/
+-rw-r--r--   0 runner    (1001) docker     (123)     2569 2023-06-26 19:17:43.000000 pulp-gem-0.1.0/pulp_gem/app/migrations/0001_initial.py
+-rw-r--r--   0 runner    (1001) docker     (123)      807 2023-06-26 19:17:43.000000 pulp-gem-0.1.0/pulp_gem/app/migrations/0002_gemrepository.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3162 2023-06-26 19:17:43.000000 pulp-gem-0.1.0/pulp_gem/app/migrations/0003_move_data_to_new_master_distribution_model.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1833 2023-06-26 19:17:43.000000 pulp-gem-0.1.0/pulp_gem/app/migrations/0004_alter_gemcontent_content_ptr_and_more.py
+-rw-r--r--   0 runner    (1001) docker     (123)      804 2023-06-26 19:17:43.000000 pulp-gem-0.1.0/pulp_gem/app/migrations/0005_rename_gemcontent_shallowgemcontent.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2068 2023-06-26 19:17:43.000000 pulp-gem-0.1.0/pulp_gem/app/migrations/0006_gemremote_excludes_gemremote_includes_and_more.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-26 19:17:43.000000 pulp-gem-0.1.0/pulp_gem/app/migrations/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4661 2023-06-26 19:17:43.000000 pulp-gem-0.1.0/pulp_gem/app/models.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7355 2023-06-26 19:17:43.000000 pulp-gem-0.1.0/pulp_gem/app/serializers.py
+-rw-r--r--   0 runner    (1001) docker     (123)      165 2023-06-26 19:17:43.000000 pulp-gem-0.1.0/pulp_gem/app/settings.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 19:17:57.242227 pulp-gem-0.1.0/pulp_gem/app/tasks/
+-rw-r--r--   0 runner    (1001) docker     (123)       87 2023-06-26 19:17:43.000000 pulp-gem-0.1.0/pulp_gem/app/tasks/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7052 2023-06-26 19:17:43.000000 pulp-gem-0.1.0/pulp_gem/app/tasks/publishing.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6169 2023-06-26 19:17:43.000000 pulp-gem-0.1.0/pulp_gem/app/tasks/synchronizing.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4584 2023-06-26 19:17:43.000000 pulp-gem-0.1.0/pulp_gem/app/viewsets.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7287 2023-06-26 19:17:43.000000 pulp-gem-0.1.0/pulp_gem/specs.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 19:17:57.242227 pulp-gem-0.1.0/pulp_gem/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-26 19:17:43.000000 pulp-gem-0.1.0/pulp_gem/tests/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 19:17:57.242227 pulp-gem-0.1.0/pulp_gem/tests/functional/
+-rw-r--r--   0 runner    (1001) docker     (123)       43 2023-06-26 19:17:43.000000 pulp-gem-0.1.0/pulp_gem/tests/functional/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 19:17:57.242227 pulp-gem-0.1.0/pulp_gem/tests/functional/api/
+-rw-r--r--   0 runner    (1001) docker     (123)       76 2023-06-26 19:17:43.000000 pulp-gem-0.1.0/pulp_gem/tests/functional/api/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1800 2023-06-26 19:17:43.000000 pulp-gem-0.1.0/pulp_gem/tests/functional/api/test_crud_content_unit.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2732 2023-06-26 19:17:43.000000 pulp-gem-0.1.0/pulp_gem/tests/functional/api/test_crud_remotes.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1969 2023-06-26 19:17:43.000000 pulp-gem-0.1.0/pulp_gem/tests/functional/api/test_download_content.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2659 2023-06-26 19:17:43.000000 pulp-gem-0.1.0/pulp_gem/tests/functional/api/test_full_mirror.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2153 2023-06-26 19:17:43.000000 pulp-gem-0.1.0/pulp_gem/tests/functional/api/test_publish.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3545 2023-06-26 19:17:43.000000 pulp-gem-0.1.0/pulp_gem/tests/functional/api/test_sync.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3234 2023-06-26 19:17:43.000000 pulp-gem-0.1.0/pulp_gem/tests/functional/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1830 2023-06-26 19:17:43.000000 pulp-gem-0.1.0/pulp_gem/tests/functional/constants.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4061 2023-06-26 19:17:43.000000 pulp-gem-0.1.0/pulp_gem/tests/functional/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 19:17:57.242227 pulp-gem-0.1.0/pulp_gem/tests/unit/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-26 19:17:43.000000 pulp-gem-0.1.0/pulp_gem/tests/unit/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      229 2023-06-26 19:17:43.000000 pulp-gem-0.1.0/pulp_gem/tests/unit/test_models.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2520 2023-06-26 19:17:43.000000 pulp-gem-0.1.0/pulp_gem/tests/unit/test_serializers.py
+-rw-r--r--   0 runner    (1001) docker     (123)      829 2023-06-26 19:17:43.000000 pulp-gem-0.1.0/pulp_gem/tests/unit/test_spec.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 19:17:57.238227 pulp-gem-0.1.0/pulp_gem.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1089 2023-06-26 19:17:56.000000 pulp-gem-0.1.0/pulp_gem.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1851 2023-06-26 19:17:57.000000 pulp-gem-0.1.0/pulp_gem.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-26 19:17:56.000000 pulp-gem-0.1.0/pulp_gem.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       58 2023-06-26 19:17:56.000000 pulp-gem-0.1.0/pulp_gem.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       42 2023-06-26 19:17:56.000000 pulp-gem-0.1.0/pulp_gem.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        9 2023-06-26 19:17:56.000000 pulp-gem-0.1.0/pulp_gem.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      787 2023-06-26 19:17:43.000000 pulp-gem-0.1.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       42 2023-06-26 19:17:43.000000 pulp-gem-0.1.0/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-26 19:17:57.242227 pulp-gem-0.1.0/setup.cfg
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1378 2023-06-26 19:17:55.000000 pulp-gem-0.1.0/setup.py
+-rw-r--r--   0 runner    (1001) docker     (123)      150 2023-06-26 19:17:43.000000 pulp-gem-0.1.0/test_requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       19 2023-06-26 19:17:43.000000 pulp-gem-0.1.0/unittest_requirements.txt
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive (GNU)
+POSIX tar archive
```

### Comparing `pulp-gem-0.0.1b2/COPYRIGHT` & `pulp-gem-0.1.0/COPYRIGHT`

 * *Files identical despite different names*

### Comparing `pulp-gem-0.0.1b2/LICENSE` & `pulp-gem-0.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `pulp-gem-0.0.1b2/pulp_gem/app/migrations/0001_initial.py` & `pulp-gem-0.1.0/pulp_gem/app/migrations/0004_alter_gemcontent_content_ptr_and_more.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,49 +1,40 @@
-# Generated by Django 2.1.4 on 2018-12-17 10:20
+# Generated by Django 4.2.1 on 2023-05-15 20:04
 
 from django.db import migrations, models
 import django.db.models.deletion
 
 
 class Migration(migrations.Migration):
 
-    initial = True
-
     dependencies = [
-        ('pulp_app', '0001_initial'),
+        ('core', '0106_alter_artifactdistribution_distribution_ptr_and_more'),
+        ('gem', '0003_move_data_to_new_master_distribution_model'),
     ]
 
     operations = [
-        migrations.CreateModel(
-            name='GemContent',
-            fields=[
-                ('content_ptr', models.OneToOneField(auto_created=True, on_delete=django.db.models.deletion.CASCADE, parent_link=True, primary_key=True, serialize=False, to='pulp_app.Content')),
-                ('name', models.TextField()),
-                ('version', models.TextField()),
-            ],
-            bases=('pulp_app.content',),
+        migrations.AlterField(
+            model_name='gemcontent',
+            name='content_ptr',
+            field=models.OneToOneField(auto_created=True, on_delete=django.db.models.deletion.CASCADE, parent_link=True, primary_key=True, serialize=False, to='core.content'),
+        ),
+        migrations.AlterField(
+            model_name='gemdistribution',
+            name='distribution_ptr',
+            field=models.OneToOneField(auto_created=True, on_delete=django.db.models.deletion.CASCADE, parent_link=True, primary_key=True, serialize=False, to='core.distribution'),
         ),
-        migrations.CreateModel(
-            name='GemPublisher',
-            fields=[
-                ('publisher_ptr', models.OneToOneField(auto_created=True, on_delete=django.db.models.deletion.CASCADE, parent_link=True, primary_key=True, serialize=False, to='pulp_app.Publisher')),
-            ],
-            options={
-                'abstract': False,
-            },
-            bases=('pulp_app.publisher',),
+        migrations.AlterField(
+            model_name='gempublication',
+            name='publication_ptr',
+            field=models.OneToOneField(auto_created=True, on_delete=django.db.models.deletion.CASCADE, parent_link=True, primary_key=True, serialize=False, to='core.publication'),
         ),
-        migrations.CreateModel(
-            name='GemRemote',
-            fields=[
-                ('remote_ptr', models.OneToOneField(auto_created=True, on_delete=django.db.models.deletion.CASCADE, parent_link=True, primary_key=True, serialize=False, to='pulp_app.Remote')),
-            ],
-            options={
-                'abstract': False,
-            },
-            bases=('pulp_app.remote',),
+        migrations.AlterField(
+            model_name='gemremote',
+            name='remote_ptr',
+            field=models.OneToOneField(auto_created=True, on_delete=django.db.models.deletion.CASCADE, parent_link=True, primary_key=True, serialize=False, to='core.remote'),
         ),
-        migrations.AlterUniqueTogether(
-            name='gemcontent',
-            unique_together={('name', 'version')},
+        migrations.AlterField(
+            model_name='gemrepository',
+            name='repository_ptr',
+            field=models.OneToOneField(auto_created=True, on_delete=django.db.models.deletion.CASCADE, parent_link=True, primary_key=True, serialize=False, to='core.repository'),
         ),
     ]
```

### Comparing `pulp-gem-0.0.1b2/pulp_gem/app/tasks/synchronizing.py` & `pulp-gem-0.1.0/pulp_gem/app/tasks/synchronizing.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,65 +1,37 @@
 import logging
-import os
 
 from gettext import gettext as _
-from urllib.parse import urlparse, urlunparse
+from urllib.parse import urljoin
 
-from pulpcore.plugin.models import Artifact, ProgressBar, Remote, Repository
+from django.conf import settings
+
+from pulpcore.plugin.models import Artifact, ProgressReport, Remote, Repository
 from pulpcore.plugin.stages import (
     DeclarativeArtifact,
     DeclarativeContent,
     DeclarativeVersion,
     Stage,
-    ArtifactDownloader,
-    ArtifactSaver,
-    QueryExistingContentUnits,
-    ContentUnitSaver,
 )
 
 from pulp_gem.app.models import GemContent, GemRemote
-from pulp_gem.specs import read_specs
+from pulp_gem.specs import (
+    NAME_REGEX,
+    VERSION_REGEX,
+    PRERELEASE_VERSION_REGEX,
+    read_versions,
+    read_info,
+    ruby_ver_includes,
+)
 
 
 log = logging.getLogger(__name__)
 
 
-class ExistingContentNeedsNoArtifacts(Stage):
-    """
-    Stage to remove declarative_artifacts from existing content.
-
-    A Stages API stage that removes all
-    :class:`~pulpcore.plugin.stages.DeclarativeArtifact` instances from
-    :class:`~pulpcore.plugin.stages.DeclarativeContent` units if the respective
-    :class:`~pulpcore.plugin.models.Content` is already existing.
-    """
-
-    async def __call__(self, in_q, out_q):
-        """
-        The coroutine for this stage.
-
-        Args:
-            in_q (:class:`asyncio.Queue`): The queue to receive
-                :class:`~pulpcore.plugin.stages.DeclarativeContent` objects from.
-            out_q (:class:`asyncio.Queue`): The queue to put
-                :class:`~pulpcore.plugin.stages.DeclarativeContent` into.
-
-        Returns:
-            The coroutine for this stage.
-
-        """
-        async for batch in self.batches(in_q):
-            for declarative_content in batch:
-                if declarative_content.content.pk is not None:
-                    declarative_content.d_artifacts = []
-                await out_q.put(declarative_content)
-        await out_q.put(None)
-
-
-def synchronize(remote_pk, repository_pk, mirror):
+def synchronize(remote_pk, repository_pk, mirror=False):
     """
     Create a new version of the repository that is synchronized with the remote as specified.
 
     Args:
         remote_pk (str): The remote PK.
         repository_pk (str): The repository PK.
         mirror (bool): True for mirror mode, False for additive.
@@ -68,25 +40,18 @@
         ValueError: If the remote does not specify a URL to sync.
 
     """
     remote = GemRemote.objects.get(pk=remote_pk)
     repository = Repository.objects.get(pk=repository_pk)
 
     if not remote.url:
-        raise ValueError(_('A remote must have a url specified to synchronize.'))
+        raise ValueError(_("A remote must have a url specified to synchronize."))
 
-    # Interpret policy to download Artifacts or not
-    download_artifacts = (remote.policy == Remote.IMMEDIATE)
     first_stage = GemFirstStage(remote)
-    dv = GemDeclarativeVersion(
-        first_stage,
-        repository,
-        mirror=mirror,
-        download_artifacts=download_artifacts,
-    )
+    dv = DeclarativeVersion(first_stage, repository, mirror=mirror)
     dv.create()
 
 
 class GemFirstStage(Stage):
     """
     The first stage of a pulp_gem sync pipeline.
     """
@@ -97,75 +62,92 @@
 
         Args:
             remote (GemRemote): The remote data to be used when syncing
 
         """
         self.remote = remote
 
-    async def __call__(self, in_q, out_q):
+    async def run(self):
         """
         Build and emit `DeclarativeContent` from the Spec data.
-
-        Args:
-            in_q (asyncio.Queue): Unused because the first stage doesn't read from an input queue.
-            out_q (asyncio.Queue): The out_q to send `DeclarativeContent` objects to
-
-        """
-        with ProgressBar(message='Downloading Metadata') as pb:
-            parsed_url = urlparse(self.remote.url)
-            root_dir = parsed_url.path
-            specs_path = os.path.join(root_dir, 'specs.4.8.gz')
-            specs_url = urlunparse(parsed_url._replace(path=specs_path))
-            downloader = self.remote.get_downloader(url=specs_url)
-            result = await downloader.run()
-            pb.increment()
-
-        with ProgressBar(message='Parsing Metadata') as pb:
-            for key in read_specs(result.path):
-                relative_path = os.path.join('gems', key.name + '-' + key.version + '.gem')
-                path = os.path.join(root_dir, relative_path)
-                url = urlunparse(parsed_url._replace(path=path))
-
-                spec_relative_path = os.path.join('quick/Marshal.4.8',
-                                                  key.name + '-' + key.version + '.gemspec.rz')
-                spec_path = os.path.join(root_dir, spec_relative_path)
-                spec_url = urlunparse(parsed_url._replace(path=spec_path))
-                gem = GemContent(name=key.name, version=key.version)
-                da_gem = DeclarativeArtifact(Artifact(), url, relative_path, self.remote)
-                da_spec = DeclarativeArtifact(Artifact(), spec_url, spec_relative_path, self.remote)
-                dc = DeclarativeContent(content=gem, d_artifacts=[da_gem, da_spec])
-                pb.increment()
-                await out_q.put(dc)
-        await out_q.put(None)
-
-
-class GemDeclarativeVersion(DeclarativeVersion):
-    """
-    Custom implementation of Declarative version.
-    """
-
-    def pipeline_stages(self, new_version):
         """
-        Build the list of pipeline stages feeding into the ContentUnitAssociation stage.
-
-        If the `self.download_artifacts` is False the pipeline will not include Artifact downloading
-        and saving stages.
+        # Interpret policy to download Artifacts or not
+        deferred_download = self.remote.policy != Remote.IMMEDIATE
 
-        This is overwritten to create a custom pipeline.
-
-        Args:
-            new_version (:class:`~pulpcore.plugin.models.RepositoryVersion`): The
-                new repository version that is going to be built.
-
-        Returns:
-            list: List of :class:`~pulpcore.plugin.stages.Stage` instances
-
-        """
-        pipeline = [
-            self.first_stage,
-            QueryExistingContentUnits(),
-            ExistingContentNeedsNoArtifacts(),
-        ]
-        if self.download_artifacts:
-            pipeline.extend([ArtifactDownloader(), ArtifactSaver()])
-        pipeline.append(ContentUnitSaver())
-        return pipeline
+        async with ProgressReport(
+            message="Downloading versions list", total=1
+        ) as pr_download_versions:
+            versions_url = urljoin(self.remote.url, "versions")
+            versions_downloader = self.remote.get_downloader(url=versions_url)
+            versions_result = await versions_downloader.run()
+            await pr_download_versions.aincrement()
+
+        async with ProgressReport(message="Parsing versions list") as pr_parse_versions:
+            async with ProgressReport(message="Parsing versions info") as pr_parse_info:
+                async for name, versions, md5_sum in read_versions(versions_result.path):
+                    await pr_parse_versions.aincrement()
+                    if not NAME_REGEX.match(name):
+                        log.warn(f"Skipping invalid gem name: '{name}'.")
+                        continue
+                    if not self.remote.prereleases:
+                        versions = [version for version in versions if VERSION_REGEX.match(version)]
+                    else:
+                        versions = [
+                            version
+                            for version in versions
+                            if PRERELEASE_VERSION_REGEX.match(version)
+                        ]
+                    if self.remote.includes:
+                        if name not in self.remote.includes:
+                            continue
+                        version_requirements = self.remote.includes[name]
+                        if version_requirements is not None:
+                            versions = [
+                                version
+                                for version in versions
+                                if ruby_ver_includes(version_requirements, version)
+                            ]
+                    if self.remote.excludes:
+                        if name in self.remote.excludes:
+                            version_requirements = self.remote.excludes[name]
+                            if version_requirements is None:
+                                continue
+                            versions = [
+                                version
+                                for version in versions
+                                if not ruby_ver_includes(version_requirements, version)
+                            ]
+                    if not versions:
+                        continue
+                    info_url = urljoin(urljoin(self.remote.url, "info/"), name)
+                    if "md5" in settings.ALLOWED_CONTENT_CHECKSUMS:
+                        extra_kwargs = {"expected_digests": {"md5": md5_sum}}
+                    else:
+                        extra_kwargs = {}
+                        log.warn(f"Checksum of info file for '{name}' could not be validated.")
+                    info_downloader = self.remote.get_downloader(url=info_url, **extra_kwargs)
+                    info_result = await info_downloader.run()
+                    async for gem_info in read_info(info_result.path, versions):
+                        gem_info["name"] = name
+                        gem = GemContent(**gem_info)
+                        gem_path = gem.relative_path
+                        gem_url = urljoin(self.remote.url, gem_path)
+                        gemspec_path = gem.gemspec_path
+                        gemspec_url = urljoin(self.remote.url, gemspec_path)
+
+                        da_gem = DeclarativeArtifact(
+                            artifact=Artifact(sha256=gem_info["checksum"]),
+                            url=gem_url,
+                            relative_path=gem_path,
+                            remote=self.remote,
+                            deferred_download=deferred_download,
+                        )
+                        da_gemspec = DeclarativeArtifact(
+                            artifact=Artifact(),
+                            url=gemspec_url,
+                            relative_path=gemspec_path,
+                            remote=self.remote,
+                            deferred_download=deferred_download,
+                        )
+                        dc = DeclarativeContent(content=gem, d_artifacts=[da_gem, da_gemspec])
+                        await pr_parse_info.aincrement()
+                        await self.put(dc)
```

