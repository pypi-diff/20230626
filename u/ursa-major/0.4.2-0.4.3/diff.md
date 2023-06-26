# Comparing `tmp/ursa-major-0.4.2.tar.gz` & `tmp/ursa-major-0.4.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/ursa-major-0.4.2.tar", last modified: Wed Mar 10 16:32:04 2021, max compression
+gzip compressed data, was "ursa-major-0.4.3.tar", last modified: Mon Jun 26 16:10:19 2023, max compression
```

## Comparing `ursa-major-0.4.2.tar` & `ursa-major-0.4.3.tar`

### file list

```diff
@@ -1,61 +1,61 @@
-drwxrwxr-x   0 yzhu       (501) games       (20)        0 2021-03-10 16:32:04.498007 ursa-major-0.4.2/
--rw-rw-r--   0 yzhu       (501) games       (20)     1799 2021-03-10 15:56:17.000000 ursa-major-0.4.2/CHANGELOG.rst
--rw-r--r--   0 yzhu       (501) games       (20)     1057 2020-05-11 07:53:55.000000 ursa-major-0.4.2/LICENSE
--rw-r--r--   0 yzhu       (501) games       (20)      230 2020-05-11 07:53:55.000000 ursa-major-0.4.2/MANIFEST.in
--rw-rw-r--   0 yzhu       (501) games       (20)    16976 2021-03-10 16:32:04.495891 ursa-major-0.4.2/PKG-INFO
--rw-r--r--   0 yzhu       (501) games       (20)    11272 2020-05-11 07:53:55.000000 ursa-major-0.4.2/README.rst
-drwxrwxr-x   0 yzhu       (501) games       (20)        0 2021-03-10 16:32:04.345064 ursa-major-0.4.2/conf/
--rw-r--r--   0 yzhu       (501) games       (20)      493 2020-05-11 07:53:55.000000 ursa-major-0.4.2/conf/ursa-major-stage.conf
--rw-r--r--   0 yzhu       (501) games       (20)      484 2020-05-11 07:53:55.000000 ursa-major-0.4.2/conf/ursa-major.conf
--rw-rw-r--   0 yzhu       (501) games       (20)       62 2021-03-10 05:57:48.000000 ursa-major-0.4.2/requirements.txt
--rw-rw-r--   0 yzhu       (501) games       (20)       38 2021-03-10 16:32:04.498544 ursa-major-0.4.2/setup.cfg
--rw-rw-r--   0 yzhu       (501) games       (20)     2115 2021-03-10 15:55:36.000000 ursa-major-0.4.2/setup.py
--rw-rw-r--   0 yzhu       (501) games       (20)       48 2021-03-10 15:47:53.000000 ursa-major-0.4.2/test-requirements.txt
-drwxrwxr-x   0 yzhu       (501) games       (20)        0 2021-03-10 16:32:04.406842 ursa-major-0.4.2/tests/
--rw-rw-r--   0 yzhu       (501) games       (20)     5494 2021-03-10 05:57:48.000000 ursa-major-0.4.2/tests/__init__.py
--rw-rw-r--   0 yzhu       (501) games       (20)    13350 2021-03-10 11:48:04.000000 ursa-major-0.4.2/tests/test_add_module.py
--rw-rw-r--   0 yzhu       (501) games       (20)    16023 2021-03-10 05:57:48.000000 ursa-major-0.4.2/tests/test_add_tag_handler.py
--rw-rw-r--   0 yzhu       (501) games       (20)     7008 2021-03-10 11:48:04.000000 ursa-major-0.4.2/tests/test_check_config.py
--rw-r--r--   0 yzhu       (501) games       (20)     4349 2020-05-11 07:53:55.000000 ursa-major-0.4.2/tests/test_cli.py
-drwxrwxr-x   0 yzhu       (501) games       (20)        0 2021-03-10 16:32:04.427235 ursa-major-0.4.2/tests/test_data/
--rw-r--r--   0 yzhu       (501) games       (20)   126163 2020-05-11 07:53:55.000000 ursa-major-0.4.2/tests/test_data/mbs_modules_testmodule_all_in_one_page.json
--rw-r--r--   0 yzhu       (501) games       (20)     4122 2020-05-11 07:53:55.000000 ursa-major-0.4.2/tests/test_data/mbs_testmodule_604_verbose.json
--rw-r--r--   0 yzhu       (501) games       (20)     6486 2020-05-11 07:53:55.000000 ursa-major-0.4.2/tests/test_data/test_get_modules_with_requires.json
--rw-r--r--   0 yzhu       (501) games       (20)     3853 2020-05-11 07:53:55.000000 ursa-major-0.4.2/tests/test_data/testmodule_ready_message.json
--rw-r--r--   0 yzhu       (501) games       (20)     3966 2020-05-11 07:53:55.000000 ursa-major-0.4.2/tests/test_data/testmodule_with_requires_ready_message.json
--rw-r--r--   0 yzhu       (501) games       (20)      382 2020-05-11 07:53:55.000000 ursa-major-0.4.2/tests/test_data/ursa-major-test.conf
--rw-r--r--   0 yzhu       (501) games       (20)    21530 2020-05-11 07:53:55.000000 ursa-major-0.4.2/tests/test_koji_service.py
--rw-rw-r--   0 yzhu       (501) games       (20)     6257 2021-03-10 05:57:48.000000 ursa-major-0.4.2/tests/test_mbs.py
--rw-rw-r--   0 yzhu       (501) games       (20)    11685 2021-03-10 11:48:04.000000 ursa-major-0.4.2/tests/test_remove_module.py
--rw-rw-r--   0 yzhu       (501) games       (20)     8717 2021-03-10 15:55:25.000000 ursa-major-0.4.2/tests/test_update_tag.py
--rw-r--r--   0 yzhu       (501) games       (20)     4241 2020-05-11 07:53:55.000000 ursa-major-0.4.2/tests/test_utils.py
-drwxrwxr-x   0 yzhu       (501) games       (20)        0 2021-03-10 16:32:04.444558 ursa-major-0.4.2/ursa_major/
--rw-r--r--   0 yzhu       (501) games       (20)     2962 2020-05-11 07:53:55.000000 ursa-major-0.4.2/ursa_major/__init__.py
--rw-r--r--   0 yzhu       (501) games       (20)    10364 2020-05-11 07:53:55.000000 ursa-major-0.4.2/ursa_major/cli.py
-drwxrwxr-x   0 yzhu       (501) games       (20)        0 2021-03-10 16:32:04.484181 ursa-major-0.4.2/ursa_major/handlers/
--rw-r--r--   0 yzhu       (501) games       (20)        0 2020-05-11 07:53:55.000000 ursa-major-0.4.2/ursa_major/handlers/__init__.py
--rw-r--r--   0 yzhu       (501) games       (20)     7158 2020-05-11 07:53:55.000000 ursa-major-0.4.2/ursa_major/handlers/add_module.py
--rw-rw-r--   0 yzhu       (501) games       (20)    10745 2021-03-10 05:57:48.000000 ursa-major-0.4.2/ursa_major/handlers/add_tag.py
--rw-r--r--   0 yzhu       (501) games       (20)     4770 2020-05-11 07:53:55.000000 ursa-major-0.4.2/ursa_major/handlers/base.py
--rw-r--r--   0 yzhu       (501) games       (20)     6292 2020-05-11 07:53:55.000000 ursa-major-0.4.2/ursa_major/handlers/check_config.py
--rw-r--r--   0 yzhu       (501) games       (20)     4416 2020-05-11 07:53:55.000000 ursa-major-0.4.2/ursa_major/handlers/remove_module.py
--rw-r--r--   0 yzhu       (501) games       (20)     1899 2020-05-11 07:53:55.000000 ursa-major-0.4.2/ursa_major/handlers/show_config.py
--rw-r--r--   0 yzhu       (501) games       (20)     8533 2021-03-10 14:33:31.000000 ursa-major-0.4.2/ursa_major/handlers/update_tag.py
--rw-r--r--   0 yzhu       (501) games       (20)    19366 2020-05-11 07:53:55.000000 ursa-major-0.4.2/ursa_major/koji_service.py
--rw-r--r--   0 yzhu       (501) games       (20)     2058 2020-05-11 07:53:55.000000 ursa-major-0.4.2/ursa_major/logger.py
--rw-r--r--   0 yzhu       (501) games       (20)     9568 2020-05-11 07:53:55.000000 ursa-major-0.4.2/ursa_major/mail.py
--rw-r--r--   0 yzhu       (501) games       (20)     5176 2020-05-11 07:53:55.000000 ursa-major-0.4.2/ursa_major/mbs.py
-drwxrwxr-x   0 yzhu       (501) games       (20)        0 2021-03-10 16:32:04.314046 ursa-major-0.4.2/ursa_major/templates/
-drwxrwxr-x   0 yzhu       (501) games       (20)        0 2021-03-10 16:32:04.493170 ursa-major-0.4.2/ursa_major/templates/mail/
--rw-r--r--   0 yzhu       (501) games       (20)      250 2020-05-11 07:53:55.000000 ursa-major-0.4.2/ursa_major/templates/mail/add-tag-error.txt.j2
--rw-r--r--   0 yzhu       (501) games       (20)      384 2020-05-11 07:53:55.000000 ursa-major-0.4.2/ursa_major/templates/mail/add-tag.txt.j2
--rw-r--r--   0 yzhu       (501) games       (20)      159 2020-05-11 07:53:55.000000 ursa-major-0.4.2/ursa_major/templates/mail/base.txt.j2
--rw-rw-r--   0 yzhu       (501) games       (20)     6899 2021-03-10 05:57:48.000000 ursa-major-0.4.2/ursa_major/utils.py
-drwxrwxr-x   0 yzhu       (501) games       (20)        0 2021-03-10 16:32:04.463719 ursa-major-0.4.2/ursa_major.egg-info/
--rw-rw-r--   0 yzhu       (501) games       (20)    16976 2021-03-10 16:32:04.000000 ursa-major-0.4.2/ursa_major.egg-info/PKG-INFO
--rw-rw-r--   0 yzhu       (501) games       (20)     1457 2021-03-10 16:32:04.000000 ursa-major-0.4.2/ursa_major.egg-info/SOURCES.txt
--rw-rw-r--   0 yzhu       (501) games       (20)        1 2021-03-10 16:32:04.000000 ursa-major-0.4.2/ursa_major.egg-info/dependency_links.txt
--rw-rw-r--   0 yzhu       (501) games       (20)       91 2021-03-10 16:32:04.000000 ursa-major-0.4.2/ursa_major.egg-info/entry_points.txt
--rw-rw-r--   0 yzhu       (501) games       (20)        1 2021-03-08 13:13:55.000000 ursa-major-0.4.2/ursa_major.egg-info/not-zip-safe
--rw-rw-r--   0 yzhu       (501) games       (20)       68 2021-03-10 16:32:04.000000 ursa-major-0.4.2/ursa_major.egg-info/requires.txt
--rw-rw-r--   0 yzhu       (501) games       (20)       11 2021-03-10 16:32:04.000000 ursa-major-0.4.2/ursa_major.egg-info/top_level.txt
+drwxr-xr-x   0 yzhu       (501) staff       (20)        0 2023-06-26 16:10:19.780806 ursa-major-0.4.3/
+-rw-r--r--   0 yzhu       (501) staff       (20)     1914 2023-06-26 16:09:08.000000 ursa-major-0.4.3/CHANGELOG.rst
+-rw-r--r--   0 yzhu       (501) staff       (20)     1057 2020-05-11 07:53:55.000000 ursa-major-0.4.3/LICENSE
+-rw-r--r--   0 yzhu       (501) staff       (20)      230 2020-05-11 07:53:55.000000 ursa-major-0.4.3/MANIFEST.in
+-rw-r--r--   0 yzhu       (501) staff       (20)    13642 2023-06-26 16:10:19.780485 ursa-major-0.4.3/PKG-INFO
+-rw-r--r--   0 yzhu       (501) staff       (20)    11272 2020-05-11 07:53:55.000000 ursa-major-0.4.3/README.rst
+drwxr-xr-x   0 yzhu       (501) staff       (20)        0 2023-06-26 16:10:19.768371 ursa-major-0.4.3/conf/
+-rw-r--r--   0 yzhu       (501) staff       (20)      493 2020-05-11 07:53:55.000000 ursa-major-0.4.3/conf/ursa-major-stage.conf
+-rw-r--r--   0 yzhu       (501) staff       (20)      484 2020-05-11 07:53:55.000000 ursa-major-0.4.3/conf/ursa-major.conf
+-rw-rw-r--   0 yzhu       (501) staff       (20)       62 2021-03-10 05:57:48.000000 ursa-major-0.4.3/requirements.txt
+-rw-r--r--   0 yzhu       (501) staff       (20)       38 2023-06-26 16:10:19.780875 ursa-major-0.4.3/setup.cfg
+-rw-r--r--   0 yzhu       (501) staff       (20)     2115 2023-06-26 16:09:08.000000 ursa-major-0.4.3/setup.py
+-rw-rw-r--   0 yzhu       (501) staff       (20)       48 2021-03-10 15:47:53.000000 ursa-major-0.4.3/test-requirements.txt
+drwxr-xr-x   0 yzhu       (501) staff       (20)        0 2023-06-26 16:10:19.771184 ursa-major-0.4.3/tests/
+-rw-rw-r--   0 yzhu       (501) staff       (20)     5494 2021-03-10 05:57:48.000000 ursa-major-0.4.3/tests/__init__.py
+-rw-rw-r--   0 yzhu       (501) staff       (20)    13350 2021-03-10 11:48:04.000000 ursa-major-0.4.3/tests/test_add_module.py
+-rw-rw-r--   0 yzhu       (501) staff       (20)    16023 2021-03-10 05:57:48.000000 ursa-major-0.4.3/tests/test_add_tag_handler.py
+-rw-rw-r--   0 yzhu       (501) staff       (20)     7008 2021-03-10 11:48:04.000000 ursa-major-0.4.3/tests/test_check_config.py
+-rw-r--r--   0 yzhu       (501) staff       (20)     4349 2020-05-11 07:53:55.000000 ursa-major-0.4.3/tests/test_cli.py
+drwxr-xr-x   0 yzhu       (501) staff       (20)        0 2023-06-26 16:10:19.773672 ursa-major-0.4.3/tests/test_data/
+-rw-r--r--   0 yzhu       (501) staff       (20)   126163 2020-05-11 07:53:55.000000 ursa-major-0.4.3/tests/test_data/mbs_modules_testmodule_all_in_one_page.json
+-rw-r--r--   0 yzhu       (501) staff       (20)     4122 2020-05-11 07:53:55.000000 ursa-major-0.4.3/tests/test_data/mbs_testmodule_604_verbose.json
+-rw-r--r--   0 yzhu       (501) staff       (20)     6486 2020-05-11 07:53:55.000000 ursa-major-0.4.3/tests/test_data/test_get_modules_with_requires.json
+-rw-r--r--   0 yzhu       (501) staff       (20)     3853 2020-05-11 07:53:55.000000 ursa-major-0.4.3/tests/test_data/testmodule_ready_message.json
+-rw-r--r--   0 yzhu       (501) staff       (20)     3966 2020-05-11 07:53:55.000000 ursa-major-0.4.3/tests/test_data/testmodule_with_requires_ready_message.json
+-rw-r--r--   0 yzhu       (501) staff       (20)      382 2020-05-11 07:53:55.000000 ursa-major-0.4.3/tests/test_data/ursa-major-test.conf
+-rw-r--r--   0 yzhu       (501) staff       (20)    21515 2023-06-26 16:07:21.000000 ursa-major-0.4.3/tests/test_koji_service.py
+-rw-rw-r--   0 yzhu       (501) staff       (20)     6257 2021-03-10 05:57:48.000000 ursa-major-0.4.3/tests/test_mbs.py
+-rw-rw-r--   0 yzhu       (501) staff       (20)    11685 2021-03-10 11:48:04.000000 ursa-major-0.4.3/tests/test_remove_module.py
+-rw-rw-r--   0 yzhu       (501) staff       (20)     8717 2021-03-10 15:55:25.000000 ursa-major-0.4.3/tests/test_update_tag.py
+-rw-r--r--   0 yzhu       (501) staff       (20)     4241 2020-05-11 07:53:55.000000 ursa-major-0.4.3/tests/test_utils.py
+drwxr-xr-x   0 yzhu       (501) staff       (20)        0 2023-06-26 16:10:19.775448 ursa-major-0.4.3/ursa_major/
+-rw-r--r--   0 yzhu       (501) staff       (20)     2962 2020-05-11 07:53:55.000000 ursa-major-0.4.3/ursa_major/__init__.py
+-rw-r--r--   0 yzhu       (501) staff       (20)    10364 2020-05-11 07:53:55.000000 ursa-major-0.4.3/ursa_major/cli.py
+drwxr-xr-x   0 yzhu       (501) staff       (20)        0 2023-06-26 16:10:19.779353 ursa-major-0.4.3/ursa_major/handlers/
+-rw-r--r--   0 yzhu       (501) staff       (20)        0 2020-05-11 07:53:55.000000 ursa-major-0.4.3/ursa_major/handlers/__init__.py
+-rw-r--r--   0 yzhu       (501) staff       (20)     7158 2020-05-11 07:53:55.000000 ursa-major-0.4.3/ursa_major/handlers/add_module.py
+-rw-rw-r--   0 yzhu       (501) staff       (20)    10745 2021-03-10 05:57:48.000000 ursa-major-0.4.3/ursa_major/handlers/add_tag.py
+-rw-r--r--   0 yzhu       (501) staff       (20)     4770 2020-05-11 07:53:55.000000 ursa-major-0.4.3/ursa_major/handlers/base.py
+-rw-r--r--   0 yzhu       (501) staff       (20)     6292 2020-05-11 07:53:55.000000 ursa-major-0.4.3/ursa_major/handlers/check_config.py
+-rw-r--r--   0 yzhu       (501) staff       (20)     4416 2020-05-11 07:53:55.000000 ursa-major-0.4.3/ursa_major/handlers/remove_module.py
+-rw-r--r--   0 yzhu       (501) staff       (20)     1899 2020-05-11 07:53:55.000000 ursa-major-0.4.3/ursa_major/handlers/show_config.py
+-rw-r--r--   0 yzhu       (501) staff       (20)     8533 2021-03-10 14:33:31.000000 ursa-major-0.4.3/ursa_major/handlers/update_tag.py
+-rw-r--r--   0 yzhu       (501) staff       (20)    19369 2023-06-26 16:07:21.000000 ursa-major-0.4.3/ursa_major/koji_service.py
+-rw-r--r--   0 yzhu       (501) staff       (20)     2058 2020-05-11 07:53:55.000000 ursa-major-0.4.3/ursa_major/logger.py
+-rw-r--r--   0 yzhu       (501) staff       (20)     9568 2020-05-11 07:53:55.000000 ursa-major-0.4.3/ursa_major/mail.py
+-rw-r--r--   0 yzhu       (501) staff       (20)     5176 2020-05-11 07:53:55.000000 ursa-major-0.4.3/ursa_major/mbs.py
+drwxr-xr-x   0 yzhu       (501) staff       (20)        0 2023-06-26 16:10:19.766033 ursa-major-0.4.3/ursa_major/templates/
+drwxr-xr-x   0 yzhu       (501) staff       (20)        0 2023-06-26 16:10:19.780103 ursa-major-0.4.3/ursa_major/templates/mail/
+-rw-r--r--   0 yzhu       (501) staff       (20)      250 2020-05-11 07:53:55.000000 ursa-major-0.4.3/ursa_major/templates/mail/add-tag-error.txt.j2
+-rw-r--r--   0 yzhu       (501) staff       (20)      384 2020-05-11 07:53:55.000000 ursa-major-0.4.3/ursa_major/templates/mail/add-tag.txt.j2
+-rw-r--r--   0 yzhu       (501) staff       (20)      159 2020-05-11 07:53:55.000000 ursa-major-0.4.3/ursa_major/templates/mail/base.txt.j2
+-rw-rw-r--   0 yzhu       (501) staff       (20)     6899 2021-03-10 05:57:48.000000 ursa-major-0.4.3/ursa_major/utils.py
+drwxr-xr-x   0 yzhu       (501) staff       (20)        0 2023-06-26 16:10:19.777296 ursa-major-0.4.3/ursa_major.egg-info/
+-rw-rw-r--   0 yzhu       (501) staff       (20)    13642 2023-06-26 16:10:19.000000 ursa-major-0.4.3/ursa_major.egg-info/PKG-INFO
+-rw-rw-r--   0 yzhu       (501) staff       (20)     1457 2023-06-26 16:10:19.000000 ursa-major-0.4.3/ursa_major.egg-info/SOURCES.txt
+-rw-rw-r--   0 yzhu       (501) staff       (20)        1 2023-06-26 16:10:19.000000 ursa-major-0.4.3/ursa_major.egg-info/dependency_links.txt
+-rw-rw-r--   0 yzhu       (501) staff       (20)       90 2023-06-26 16:10:19.000000 ursa-major-0.4.3/ursa_major.egg-info/entry_points.txt
+-rw-rw-r--   0 yzhu       (501) staff       (20)        1 2021-03-08 13:13:55.000000 ursa-major-0.4.3/ursa_major.egg-info/not-zip-safe
+-rw-rw-r--   0 yzhu       (501) staff       (20)       68 2023-06-26 16:10:19.000000 ursa-major-0.4.3/ursa_major.egg-info/requires.txt
+-rw-rw-r--   0 yzhu       (501) staff       (20)       11 2023-06-26 16:10:19.000000 ursa-major-0.4.3/ursa_major.egg-info/top_level.txt
```

### Comparing `ursa-major-0.4.2/CHANGELOG.rst` & `ursa-major-0.4.3/CHANGELOG.rst`

 * *Files 6% similar despite different names*

```diff
@@ -1,9 +1,13 @@
 Change Logs
 ===========
+0.4.2 (2023-06-27)
+------------------
+* Use gssapi_login instead of krb_login for koji kerberos auth (Yuming Zhu)
+
 0.4.2 (2021-03-10)
 ------------------
 * Use old tuple syntax for mock.call.call_args of old mock release (Yuming Zhu)
 * Fix unittests for missing koji profile (Yuming Zhu)
 * Using libmodulemd v2 API (Yuming Zhu)
 
 0.4.1 (2020-02-11)
```

### Comparing `ursa-major-0.4.2/LICENSE` & `ursa-major-0.4.3/LICENSE`

 * *Files identical despite different names*

### Comparing `ursa-major-0.4.2/PKG-INFO` & `ursa-major-0.4.3/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,444 +1,448 @@
-Metadata-Version: 1.1
+Metadata-Version: 2.1
 Name: ursa-major
-Version: 0.4.2
+Version: 0.4.3
 Summary: A utility for managing module tags in Koji's tag inheritance
 Home-page: https://pagure.io/ursa-major/
 Author: The Factory 2.0 Team
 Author-email: ursa-major-owner@fedoraproject.org
 License: MIT
-Description: Ursa-Major
-        ==========
-        
-        .. image:: https://img.shields.io/pypi/v/ursa-major.svg
-           :alt: PyPI
-        
-        .. image:: https://img.shields.io/pypi/l/ursa-major.svg
-           :alt: PyPI - License
-        
-        .. image:: https://img.shields.io/pypi/pyversions/ursa-major.svg
-           :alt: PyPI - Python Version
-        
-        Ursa-Major is a utility to help managing module's koji tags in koji's
-        inheritance. It reads configuration for tags from a tag config file, then
-        update koji's inheritance accordingly.
-        
-        Tag Config File
-        ---------------
-        
-        The tag config file used by Ursa-Major is in json format, the top level keys
-        are koji tags which we should add module tags into their inheritance. For each
-        tag, it contains a list of modules, owners can also be set for a tag.
-        
-        An example tag config file is:
-        
-        .. code-block:: json
-        
-            {
-                "fedora-30-buildroot-modules": {
-                    "modules": [
-                        {
-                            "name": "httpd",
-                            "priority": 10,
-                            "buildrequires": {
-                                "platform": "f30"
-                            },
-                            "requires": {
-                                "platform": "f30"
-                            },
-                            "stream": "2.4"
-                        },
-                        {
-                            "name": "ruby",
-                            "priority": 40,
-                            "requires": {
-                                "platform": "f30"
-                            },
-                            "stream": "2.5"
-                        }
-                    ],
-                    "owners": [
-                        "foo@example.com"
-                    ]
-                },
-                "fedora-30-test-build": {
-                    "modules": [
-                        {
-                            "name": "testmodule",
-                            "priority": 150,
-                            "stream": "f30"
-                        }
-                    ],
-                    "owners": [
-                        "bar@example.com"
-                    ]
-                }
-            }
-        
-        
-        A valid module config should contains:
-        
-        * ``name`` (required): module name
-        * ``stream`` (required): module stream
-        * ``priority`` (required): add module's tag to tag inheritance with this priority
-        * ``requires`` (optional): module's runtime dependencies.
-        * ``buildrequires`` (optional): module's build time dependencies.
-        
-        For each tag, ``owners`` can be set with email addresses.
-        
-        The default tag config file used by Ursa-Major is ``ursa-major.json`` in current
-        working directory. You can change it with ``--tag-config-file``.
-        
-        
-        Koji and MBS
-        ------------
-        
-        Tags in tag config file are koji tags, Ursa-Major connects to koji hub and
-        update tag inheritance per config, and connects to MBS to query module's
-        information, especially the modulemd data.
-        
-        Koji and MBS servers are set in Ursa-Major's config files, the global config
-        file is ``/etc/ursa-major/ursa-major`` by default, and can be changed by
-        ``--config`` argument. The user config file is
-        ``~/.config/ursa-major/ursa-major.conf``, and can be changed by
-        ``--user-config``. User config file is optional, and values in global config
-        file will be overrided by user config file.
-        
-        An example config file:
-        
-        .. code-block:: bash
-        
-            $ cat /etc/ursa-major/ursa-major.conf
-        
-            [main]
-            # See https://docs.python.org/3/library/logging.html#logging-levels
-            log_level = info
-        
-            [koji]
-            profile = koji
-        
-            [mbs]
-            server_url = https://mbs.fedoraproject.org/
-        
-            [mail]
-            mail_processing = true
-            mail_log_level = info
-            mail_server = smtp.example.com
-            mail_from = ursa-major@example.com
-            mail_replyto = ursa-major@example.com
-            # email addresses seperated by ','
-            mail_always_cc = ursa-major-admin@example.com
-            mail_always_bcc =
-            mail_subject_prefix = [ursa-major]
-        
-        
-        Sub Commands
-        ============
-        
-        Global arguments of ``ursa-major``:
-        
-        * ``--debug`` (optional): print debug messages
-        
-        * ``--dry-run`` (optional): run in dry-run mode, not do any real change
-        
-        * ``--config`` (optional): default if ``/etc/ursa-major/ursa-major.conf``
-        
-        * ``--user-config`` (optional): default is ``~/.config/ursa-major/ursa-major.conf``
-        
-        * ``--tag-config-file`` (optional): default is ``$PWD/ursa-major.json``
-        
-        
-        show-config
-        -----------
-        
-        This just show the content of tag config file, or the content of a specified
-        tag.
-        
-        Arguments:
-        
-        * ``--tag`` (optional): only show config content under this tag
-        
-        Example:
-        
-        .. code-block:: bash
-        
-            $ ursa-major show-config --tag-config-file ~/fedora-prod-ursa-major.json --tag fedora-30-test-build
-        
-        check-config
-        ------------
-        
-        Check the tag config file to detect any invalid configuration:
-        
-        .. code-block:: bash
-        
-            $ ursa-major check-config --tag-config-file ~/fedora-prod-ursa-major.json
-        
-        Checks include:
-        
-        * ``name``, ``stream`` and ``priority`` are required for a module
-        * ``priority`` value should not conflict with other parent tags which not belong
-          to this module in tag's inheritance
-        * ...
-        
-        remove-module
-        -------------
-        
-        Remove a module from the tag config file.
-        
-        Arguments:
-        
-        * ``--tag`` (required): remove module from this tag
-        
-        * ``--name`` (required): module name
-        
-        * ``--stream`` (required): module stream
-        
-        * ``--require`` (optional): module's runtime requires, can be specified multiple times
-        
-        * ``--buildrequire`` (optional): module's buildrequires, can be specified multiple times
-        
-        
-        Example:
-        
-        .. code-block:: bash
-        
-            $ ursa-major remove-module --tag fedora-30-test-build --name testmodule --stream f30
-        
-        This will remove the module of ``testmodule:f30`` from tag config file if it's
-        s present under tag ``fedora-30-test-build``.
-        
-        add-module
-        ----------
-        
-        Add a module to tag config file under the specified tag.
-        
-        Arguments:
-        
-        * ``--tag`` (required): add module to this tag
-        
-        * ``--name`` (required): module name
-        
-        * ``--stream`` (required): module stream
-        
-        * ``--priority`` (required): priority value when add tag to inheritance
-        
-        * ``--require`` (optional): module's runtime requires, can be specified multiple times
-        
-        * ``--buildrequire`` (optional): module's buildrequires, can be specified multiple times
-        
-        Example:
-        
-        .. code-block:: bash
-        
-            $ ursa-major add-module --tag fedora-30-test-build --name testmodule --stream f30 --priority 100
-        
-        If the specified module with that ``name`` and ``stream`` already exists in tag
-        config file, Ursa-Major will check whether ``requires`` or ``priority`` is
-        different from the value specified in command line, if true, the tag config
-        file will be updated to use the values specified.
-        
-        update-tag
-        ----------
-        
-        Update a tag's inheritance data with all latest module build tags of the
-        modules in tag's config.
-        
-        Arguments:
-        
-        * ``--tag`` (required): the tag to update
-        * ``--wait-regen-repo`` (optional): wait for regen-repo task to finish
-        
-        Example:
-        
-        .. code-block:: bash
-        
-            $ ursa-major update-tag --tag fedora-30-test-build --wait-regen-repo
-        
-        This will check the latest builds in MBS for all modules in config of tag
-        'fedora-30-test-build', if there is any build's tag is missing from tag's
-        inheritance data, the tag will be added into inheritance, and old tags
-        will be removed at the same time for the module.
-        
-        add-tag
-        -------
-        
-        Reads module state change message from an environment variable and then add
-        the module's koji tag tag inheritance according to tag config file if the
-        module build state is 'ready', and remove old tags of the module at the same
-        time. The module's state change message is generated by MBS.
-        
-        Arguments:
-        
-        * ``--module-from-env`` (optional): the environment variable Ursa-Major read the
-          module state change message from, by default it's ``CI_MESSAGE``
-        
-        * ``--wait-regen-repo`` (optinal): wait for regen-repo tasks to finish, default is ``False``
-        
-        * ``--send-mail`` (optional): send mail to tag owners, default is ``False``
-        
-        Example:
-        
-        .. code-block:: bash
-        
-            $ cat $CI_MESSAGE
-            {
-              "state_reason": null,
-              "component_builds": [
-                108146,
-                108145
-              ],
-              "name": "testmodule",
-              "stream": "master",
-              "time_submitted": "2018-10-26T16:59:06Z",
-              "version": "20181026165847",
-              "time_modified": "2018-10-26T16:59:27Z",
-              "state_name": "ready",
-              "scmurl": "https://src.fedoraproject.org/modules/testmodule.git?#3f262deef9d79160ea229142aeb51eedcc956929",
-              "state": 5,
-              "time_completed": "2018-10-26T16:59:15Z",
-              "koji_tag": "module-testmodule-master-20181026165847-a5b0195c",
-              "context": "a5b0195c",
-              "owner": "foobar",
-              "siblings": [],
-              "id": 2321,
-              "rebuild_strategy": "only-changed"
-            }
-        
-            $ cat $PWD/ursa-major.json
-            {
-                "fedora-30-test-build": {
-                    "modules": [
-                        {
-                            "name": "testmodule",
-                            "priority": 150,
-                            "stream": "master"
-                        }
-                    ],
-                    "owners": [
-                        "foobar@example.com"
-                    ]
-                }
-            }
-        
-            $ ursa-major add-tag --wait-regen-repo --send-mail
-        
-        In this example, Ursa-Major reads the module state change message from
-        enviroment variable ``CI_MESSAGE``, the module build state name is "ready" and
-        module is present under a tag "fedora-30-test-build" in tag config file.
-        Ursa-Major will add the koji tag "module-testmodule-master-20181026165847-a5b0195c"
-        into "fedora-30-test-build"'s inheritance, and then regen-repo for build tags
-        in "fedora-30-test-build"'s inheritance.
-        
-        When a tag is added to tag inheritance, Ursa-Major also submit ``regen-repo``
-        tasks for the build tags in inheritance data. If the specified tag is a build
-        tag, it's the only one build tag Ursa-Major will regen-repo for. Or Ursa-Major
-        will check the tag's inheritance data, if it reaches the first build tag in
-        each inheritant path, it returns that build tag. And it stops at any tag that
-        name starts with 'module-'.
-        
-        For example, if we have tag inheritance data as below (tags with
-        '*' marks are build tags):
-        
-        Example #1:
-        
-        ::
-        
-                my-example-tag
-                  └─product-foo-temp-override
-                     └─product-foo-override
-                        └─product-foo-build (*)
-                           ├─tmp-product-foo-build (*)
-                           └─alt-product-foo-build (*)
-        
-        In this case, there is one build tag found for 'my-example-tag', it is:
-        ``product-foo-build``. Ursa-Major stops at 'product-foo-build', so
-        'tmp-product-foo-build' and 'alt-product-foo-build' are not checked at all.
-        
-        Example #2:
-        
-        ::
-        
-            my-example-tag
-              ├─module-345678-build
-              ├─module-234567-build
-              ├─module-123456-build
-              │  └─product-foo-module-hotfix
-              │     └─product-foo-module-hotfix-build (*)
-              ├─tmp-product-foo-python-candidate
-              │  └─tmp-product-foo-python-override
-              │     └─tmp-product-foo-python-build (*)
-              ├─product-foo-container-build (*)
-              └─product-foo-temp-override
-                 └─product-foo-override
-                    └─product-foo-build (*)
-                       ├─tmp-product-foo-build (*)
-                       └─alt-product-foo-build (*)
-        
-        In this case, there are 3 build tags found for ``my-example-tag``, they are:
-        ``tmp-product-foo-python-build``, ``product-foo-container-build`` and
-        ``product-foo-build``. ``product-foo-module-hotfix-build`` is a build tag, but
-        Ursa-Major doesn't count it in, because it stops at tag 'module-123456-build'
-        which name starts with 'module-'.
-        
-        Ursa-Major will send mail to tag owners if run with "--send-mail", mail
-        configuration can be configured in global config file or user config file,
-        under the section of "mail".
-        
-        
-        Change Logs
-        ===========
-        0.4.2 (2021-03-10)
-        ------------------
-        * Use old tuple syntax for mock.call.call_args of old mock release (Yuming Zhu)
-        * Fix unittests for missing koji profile (Yuming Zhu)
-        * Using libmodulemd v2 API (Yuming Zhu)
-        
-        0.4.1 (2020-02-11)
-        ------------------
-        * Remove updating koji inheritance ability from add-module and remove-module (Qixiang Wan)
-        
-        0.3.3 (2019-08-23)
-        ------------------
-        * Add new sub command update-tag (Qixiang Wan)
-        
-        0.3.2 (2019-06-26)
-        ------------------
-        * Include garbaged module builds while checking existing module build tags (Qixiang Wan)
-        * Refactor get_modules (Qixiang Wan)
-        
-        0.3.1 (2019-05-21)
-        ------------------
-        
-        * Not check requires/buildrequires for existing koji tags (Qixiang Wan)
-        * Updating existing inheritance instead of removing and adding (Qixiang Wan)
-        
-        0.2.2 (2019-03-26)
-        ------------------
-        
-        * For adding tag, allow filtering on buildrequires to find out koji_tags from
-          tag inheritance (Chenxiong Qi)
-        
-        0.2.1 (2019-03-20)
-        ------------------
-        
-        * Make setup_method/teardown_method compatible with newer version of pytest (Chenxiong Qi)
-        * Add missing file CHANGELOG.rst to sdist package (Chenxiong Qi)
-        
-        0.2.0 (2019-03-20)
-        ------------------
-        
-        * Add tests for AddModuleHandler methods (Chenxiong Qi)
-        * Avoid long modulemd embedded into fake data for tests (Chenxiong Qi)
-        * Fixes according to review comments (Chenxiong Qi)
-        * Command check-config supports filtering modules on buildrequires (Chenxiong Qi)
-        * Command add-module supports buildrequires now (Chenxiong Qi)
-        * Command remove-module supports filtering modules on buildrequires (Chenxiong Qi)
-        * Allow passing buildrequires to MBS.get_modules_with_requires (Chenxiong Qi)
-        * Reword remove-module help and --tag option help text (Chenxiong Qi)
-        * Allow filtering on buildrequires (Chenxiong Qi)
-        
-        
 Keywords: ursa-major modularity koji fedora
-Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 2.7
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Topic :: Utilities
+License-File: LICENSE
+
+Ursa-Major
+==========
+
+.. image:: https://img.shields.io/pypi/v/ursa-major.svg
+   :alt: PyPI
+
+.. image:: https://img.shields.io/pypi/l/ursa-major.svg
+   :alt: PyPI - License
+
+.. image:: https://img.shields.io/pypi/pyversions/ursa-major.svg
+   :alt: PyPI - Python Version
+
+Ursa-Major is a utility to help managing module's koji tags in koji's
+inheritance. It reads configuration for tags from a tag config file, then
+update koji's inheritance accordingly.
+
+Tag Config File
+---------------
+
+The tag config file used by Ursa-Major is in json format, the top level keys
+are koji tags which we should add module tags into their inheritance. For each
+tag, it contains a list of modules, owners can also be set for a tag.
+
+An example tag config file is:
+
+.. code-block:: json
+
+    {
+        "fedora-30-buildroot-modules": {
+            "modules": [
+                {
+                    "name": "httpd",
+                    "priority": 10,
+                    "buildrequires": {
+                        "platform": "f30"
+                    },
+                    "requires": {
+                        "platform": "f30"
+                    },
+                    "stream": "2.4"
+                },
+                {
+                    "name": "ruby",
+                    "priority": 40,
+                    "requires": {
+                        "platform": "f30"
+                    },
+                    "stream": "2.5"
+                }
+            ],
+            "owners": [
+                "foo@example.com"
+            ]
+        },
+        "fedora-30-test-build": {
+            "modules": [
+                {
+                    "name": "testmodule",
+                    "priority": 150,
+                    "stream": "f30"
+                }
+            ],
+            "owners": [
+                "bar@example.com"
+            ]
+        }
+    }
+
+
+A valid module config should contains:
+
+* ``name`` (required): module name
+* ``stream`` (required): module stream
+* ``priority`` (required): add module's tag to tag inheritance with this priority
+* ``requires`` (optional): module's runtime dependencies.
+* ``buildrequires`` (optional): module's build time dependencies.
+
+For each tag, ``owners`` can be set with email addresses.
+
+The default tag config file used by Ursa-Major is ``ursa-major.json`` in current
+working directory. You can change it with ``--tag-config-file``.
+
+
+Koji and MBS
+------------
+
+Tags in tag config file are koji tags, Ursa-Major connects to koji hub and
+update tag inheritance per config, and connects to MBS to query module's
+information, especially the modulemd data.
+
+Koji and MBS servers are set in Ursa-Major's config files, the global config
+file is ``/etc/ursa-major/ursa-major`` by default, and can be changed by
+``--config`` argument. The user config file is
+``~/.config/ursa-major/ursa-major.conf``, and can be changed by
+``--user-config``. User config file is optional, and values in global config
+file will be overrided by user config file.
+
+An example config file:
+
+.. code-block:: bash
+
+    $ cat /etc/ursa-major/ursa-major.conf
+
+    [main]
+    # See https://docs.python.org/3/library/logging.html#logging-levels
+    log_level = info
+
+    [koji]
+    profile = koji
+
+    [mbs]
+    server_url = https://mbs.fedoraproject.org/
+
+    [mail]
+    mail_processing = true
+    mail_log_level = info
+    mail_server = smtp.example.com
+    mail_from = ursa-major@example.com
+    mail_replyto = ursa-major@example.com
+    # email addresses seperated by ','
+    mail_always_cc = ursa-major-admin@example.com
+    mail_always_bcc =
+    mail_subject_prefix = [ursa-major]
+
+
+Sub Commands
+============
+
+Global arguments of ``ursa-major``:
+
+* ``--debug`` (optional): print debug messages
+
+* ``--dry-run`` (optional): run in dry-run mode, not do any real change
+
+* ``--config`` (optional): default if ``/etc/ursa-major/ursa-major.conf``
+
+* ``--user-config`` (optional): default is ``~/.config/ursa-major/ursa-major.conf``
+
+* ``--tag-config-file`` (optional): default is ``$PWD/ursa-major.json``
+
+
+show-config
+-----------
+
+This just show the content of tag config file, or the content of a specified
+tag.
+
+Arguments:
+
+* ``--tag`` (optional): only show config content under this tag
+
+Example:
+
+.. code-block:: bash
+
+    $ ursa-major show-config --tag-config-file ~/fedora-prod-ursa-major.json --tag fedora-30-test-build
+
+check-config
+------------
+
+Check the tag config file to detect any invalid configuration:
+
+.. code-block:: bash
+
+    $ ursa-major check-config --tag-config-file ~/fedora-prod-ursa-major.json
+
+Checks include:
+
+* ``name``, ``stream`` and ``priority`` are required for a module
+* ``priority`` value should not conflict with other parent tags which not belong
+  to this module in tag's inheritance
+* ...
+
+remove-module
+-------------
+
+Remove a module from the tag config file.
+
+Arguments:
+
+* ``--tag`` (required): remove module from this tag
+
+* ``--name`` (required): module name
+
+* ``--stream`` (required): module stream
+
+* ``--require`` (optional): module's runtime requires, can be specified multiple times
+
+* ``--buildrequire`` (optional): module's buildrequires, can be specified multiple times
+
+
+Example:
+
+.. code-block:: bash
+
+    $ ursa-major remove-module --tag fedora-30-test-build --name testmodule --stream f30
+
+This will remove the module of ``testmodule:f30`` from tag config file if it's
+s present under tag ``fedora-30-test-build``.
+
+add-module
+----------
+
+Add a module to tag config file under the specified tag.
+
+Arguments:
+
+* ``--tag`` (required): add module to this tag
+
+* ``--name`` (required): module name
+
+* ``--stream`` (required): module stream
+
+* ``--priority`` (required): priority value when add tag to inheritance
+
+* ``--require`` (optional): module's runtime requires, can be specified multiple times
+
+* ``--buildrequire`` (optional): module's buildrequires, can be specified multiple times
+
+Example:
+
+.. code-block:: bash
+
+    $ ursa-major add-module --tag fedora-30-test-build --name testmodule --stream f30 --priority 100
+
+If the specified module with that ``name`` and ``stream`` already exists in tag
+config file, Ursa-Major will check whether ``requires`` or ``priority`` is
+different from the value specified in command line, if true, the tag config
+file will be updated to use the values specified.
+
+update-tag
+----------
+
+Update a tag's inheritance data with all latest module build tags of the
+modules in tag's config.
+
+Arguments:
+
+* ``--tag`` (required): the tag to update
+* ``--wait-regen-repo`` (optional): wait for regen-repo task to finish
+
+Example:
+
+.. code-block:: bash
+
+    $ ursa-major update-tag --tag fedora-30-test-build --wait-regen-repo
+
+This will check the latest builds in MBS for all modules in config of tag
+'fedora-30-test-build', if there is any build's tag is missing from tag's
+inheritance data, the tag will be added into inheritance, and old tags
+will be removed at the same time for the module.
+
+add-tag
+-------
+
+Reads module state change message from an environment variable and then add
+the module's koji tag tag inheritance according to tag config file if the
+module build state is 'ready', and remove old tags of the module at the same
+time. The module's state change message is generated by MBS.
+
+Arguments:
+
+* ``--module-from-env`` (optional): the environment variable Ursa-Major read the
+  module state change message from, by default it's ``CI_MESSAGE``
+
+* ``--wait-regen-repo`` (optinal): wait for regen-repo tasks to finish, default is ``False``
+
+* ``--send-mail`` (optional): send mail to tag owners, default is ``False``
+
+Example:
+
+.. code-block:: bash
+
+    $ cat $CI_MESSAGE
+    {
+      "state_reason": null,
+      "component_builds": [
+        108146,
+        108145
+      ],
+      "name": "testmodule",
+      "stream": "master",
+      "time_submitted": "2018-10-26T16:59:06Z",
+      "version": "20181026165847",
+      "time_modified": "2018-10-26T16:59:27Z",
+      "state_name": "ready",
+      "scmurl": "https://src.fedoraproject.org/modules/testmodule.git?#3f262deef9d79160ea229142aeb51eedcc956929",
+      "state": 5,
+      "time_completed": "2018-10-26T16:59:15Z",
+      "koji_tag": "module-testmodule-master-20181026165847-a5b0195c",
+      "context": "a5b0195c",
+      "owner": "foobar",
+      "siblings": [],
+      "id": 2321,
+      "rebuild_strategy": "only-changed"
+    }
+
+    $ cat $PWD/ursa-major.json
+    {
+        "fedora-30-test-build": {
+            "modules": [
+                {
+                    "name": "testmodule",
+                    "priority": 150,
+                    "stream": "master"
+                }
+            ],
+            "owners": [
+                "foobar@example.com"
+            ]
+        }
+    }
+
+    $ ursa-major add-tag --wait-regen-repo --send-mail
+
+In this example, Ursa-Major reads the module state change message from
+enviroment variable ``CI_MESSAGE``, the module build state name is "ready" and
+module is present under a tag "fedora-30-test-build" in tag config file.
+Ursa-Major will add the koji tag "module-testmodule-master-20181026165847-a5b0195c"
+into "fedora-30-test-build"'s inheritance, and then regen-repo for build tags
+in "fedora-30-test-build"'s inheritance.
+
+When a tag is added to tag inheritance, Ursa-Major also submit ``regen-repo``
+tasks for the build tags in inheritance data. If the specified tag is a build
+tag, it's the only one build tag Ursa-Major will regen-repo for. Or Ursa-Major
+will check the tag's inheritance data, if it reaches the first build tag in
+each inheritant path, it returns that build tag. And it stops at any tag that
+name starts with 'module-'.
+
+For example, if we have tag inheritance data as below (tags with
+'*' marks are build tags):
+
+Example #1:
+
+::
+
+        my-example-tag
+          └─product-foo-temp-override
+             └─product-foo-override
+                └─product-foo-build (*)
+                   ├─tmp-product-foo-build (*)
+                   └─alt-product-foo-build (*)
+
+In this case, there is one build tag found for 'my-example-tag', it is:
+``product-foo-build``. Ursa-Major stops at 'product-foo-build', so
+'tmp-product-foo-build' and 'alt-product-foo-build' are not checked at all.
+
+Example #2:
+
+::
+
+    my-example-tag
+      ├─module-345678-build
+      ├─module-234567-build
+      ├─module-123456-build
+      │  └─product-foo-module-hotfix
+      │     └─product-foo-module-hotfix-build (*)
+      ├─tmp-product-foo-python-candidate
+      │  └─tmp-product-foo-python-override
+      │     └─tmp-product-foo-python-build (*)
+      ├─product-foo-container-build (*)
+      └─product-foo-temp-override
+         └─product-foo-override
+            └─product-foo-build (*)
+               ├─tmp-product-foo-build (*)
+               └─alt-product-foo-build (*)
+
+In this case, there are 3 build tags found for ``my-example-tag``, they are:
+``tmp-product-foo-python-build``, ``product-foo-container-build`` and
+``product-foo-build``. ``product-foo-module-hotfix-build`` is a build tag, but
+Ursa-Major doesn't count it in, because it stops at tag 'module-123456-build'
+which name starts with 'module-'.
+
+Ursa-Major will send mail to tag owners if run with "--send-mail", mail
+configuration can be configured in global config file or user config file,
+under the section of "mail".
+
+
+Change Logs
+===========
+0.4.2 (2023-06-27)
+------------------
+* Use gssapi_login instead of krb_login for koji kerberos auth (Yuming Zhu)
+
+0.4.2 (2021-03-10)
+------------------
+* Use old tuple syntax for mock.call.call_args of old mock release (Yuming Zhu)
+* Fix unittests for missing koji profile (Yuming Zhu)
+* Using libmodulemd v2 API (Yuming Zhu)
+
+0.4.1 (2020-02-11)
+------------------
+* Remove updating koji inheritance ability from add-module and remove-module (Qixiang Wan)
+
+0.3.3 (2019-08-23)
+------------------
+* Add new sub command update-tag (Qixiang Wan)
+
+0.3.2 (2019-06-26)
+------------------
+* Include garbaged module builds while checking existing module build tags (Qixiang Wan)
+* Refactor get_modules (Qixiang Wan)
+
+0.3.1 (2019-05-21)
+------------------
+
+* Not check requires/buildrequires for existing koji tags (Qixiang Wan)
+* Updating existing inheritance instead of removing and adding (Qixiang Wan)
+
+0.2.2 (2019-03-26)
+------------------
+
+* For adding tag, allow filtering on buildrequires to find out koji_tags from
+  tag inheritance (Chenxiong Qi)
+
+0.2.1 (2019-03-20)
+------------------
+
+* Make setup_method/teardown_method compatible with newer version of pytest (Chenxiong Qi)
+* Add missing file CHANGELOG.rst to sdist package (Chenxiong Qi)
+
+0.2.0 (2019-03-20)
+------------------
+
+* Add tests for AddModuleHandler methods (Chenxiong Qi)
+* Avoid long modulemd embedded into fake data for tests (Chenxiong Qi)
+* Fixes according to review comments (Chenxiong Qi)
+* Command check-config supports filtering modules on buildrequires (Chenxiong Qi)
+* Command add-module supports buildrequires now (Chenxiong Qi)
+* Command remove-module supports filtering modules on buildrequires (Chenxiong Qi)
+* Allow passing buildrequires to MBS.get_modules_with_requires (Chenxiong Qi)
+* Reword remove-module help and --tag option help text (Chenxiong Qi)
+* Allow filtering on buildrequires (Chenxiong Qi)
+
```

### Comparing `ursa-major-0.4.2/README.rst` & `ursa-major-0.4.3/README.rst`

 * *Files identical despite different names*

### Comparing `ursa-major-0.4.2/setup.py` & `ursa-major-0.4.3/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -36,15 +36,15 @@
     deps_links.extend(_)
 
 
 setup(
     name='ursa-major',
     description="A utility for managing module tags in Koji's tag inheritance",
     long_description=get_long_description(),
-    version='0.4.2',
+    version='0.4.3',
     classifiers=[
         'Programming Language :: Python :: 2.7',
         'Programming Language :: Python :: 3.6',
         'Topic :: Utilities',
     ],
     keywords='ursa-major modularity koji fedora',
     author='The Factory 2.0 Team',
```

### Comparing `ursa-major-0.4.2/tests/__init__.py` & `ursa-major-0.4.3/tests/__init__.py`

 * *Files identical despite different names*

### Comparing `ursa-major-0.4.2/tests/test_add_module.py` & `ursa-major-0.4.3/tests/test_add_module.py`

 * *Files identical despite different names*

### Comparing `ursa-major-0.4.2/tests/test_add_tag_handler.py` & `ursa-major-0.4.3/tests/test_add_tag_handler.py`

 * *Files identical despite different names*

### Comparing `ursa-major-0.4.2/tests/test_check_config.py` & `ursa-major-0.4.3/tests/test_check_config.py`

 * *Files identical despite different names*

### Comparing `ursa-major-0.4.2/tests/test_cli.py` & `ursa-major-0.4.3/tests/test_cli.py`

 * *Files identical despite different names*

### Comparing `ursa-major-0.4.2/tests/test_data/mbs_modules_testmodule_all_in_one_page.json` & `ursa-major-0.4.3/tests/test_data/mbs_modules_testmodule_all_in_one_page.json`

 * *Files identical despite different names*

### Comparing `ursa-major-0.4.2/tests/test_data/mbs_testmodule_604_verbose.json` & `ursa-major-0.4.3/tests/test_data/mbs_testmodule_604_verbose.json`

 * *Files identical despite different names*

### Comparing `ursa-major-0.4.2/tests/test_data/test_get_modules_with_requires.json` & `ursa-major-0.4.3/tests/test_data/test_get_modules_with_requires.json`

 * *Files identical despite different names*

### Comparing `ursa-major-0.4.2/tests/test_data/testmodule_ready_message.json` & `ursa-major-0.4.3/tests/test_data/testmodule_ready_message.json`

 * *Files identical despite different names*

### Comparing `ursa-major-0.4.2/tests/test_data/testmodule_with_requires_ready_message.json` & `ursa-major-0.4.3/tests/test_data/testmodule_with_requires_ready_message.json`

 * *Files identical despite different names*

### Comparing `ursa-major-0.4.2/tests/test_koji_service.py` & `ursa-major-0.4.3/tests/test_koji_service.py`

 * *Files 0% similar despite different names*

```diff
@@ -28,36 +28,38 @@
 from ursa_major.koji_service import KojiService
 
 
 class KojiServiceTestCase(unittest.TestCase):
     def setUp(self):
         self.koji_profile = mock.Mock()
         with mock.patch('ursa_major.koji_service.koji') as koji:
-            koji.krb_login = mock.Mock()
+            koji.gssapi_login = mock.Mock()
             koji.get_profile_module = mock.Mock(
                 return_value=mock.Mock(
                     config=mock.Mock(
                         server='koji.example.com',
                         weburl='koji.example.com',
                         authtype='kerberos',
                         krb_rdns=False,
                         cert=''),
                 )
             )
             self.koji_profile = koji.get_profile_module.return_value
             self.koji = KojiService('dummy-koji')
             self.koji.koji_proxy.logged_in = False
 
-    def test_krb_login(self):
+    def test_gssapi_login(self):
         self.koji.koji_module.config.keytab = 'testkeytab'
         self.koji.koji_module.config.principal = 'testprincipal'
         self.assertEqual(self.koji.koji_module.config.krb_rdns, False)
         self.koji.login()
-        self.koji.koji_proxy.krb_login.assert_called_with('testprincipal',
-                                                          'testkeytab')
+        self.koji.koji_proxy.gssapi_login.assert_called_with(
+            'testprincipal',
+            'testkeytab'
+        )
 
     def test_get_inheritance_data(self):
         self.koji.koji_proxy = mock.Mock(
             getTag=mock.Mock(),
             getInheritanceData=mock.Mock(),
         )
         self.koji.get_inheritance_data(1)
```

### Comparing `ursa-major-0.4.2/tests/test_mbs.py` & `ursa-major-0.4.3/tests/test_mbs.py`

 * *Files identical despite different names*

### Comparing `ursa-major-0.4.2/tests/test_remove_module.py` & `ursa-major-0.4.3/tests/test_remove_module.py`

 * *Files identical despite different names*

### Comparing `ursa-major-0.4.2/tests/test_update_tag.py` & `ursa-major-0.4.3/tests/test_update_tag.py`

 * *Files identical despite different names*

### Comparing `ursa-major-0.4.2/tests/test_utils.py` & `ursa-major-0.4.3/tests/test_utils.py`

 * *Files identical despite different names*

### Comparing `ursa-major-0.4.2/ursa_major/__init__.py` & `ursa-major-0.4.3/ursa_major/__init__.py`

 * *Files identical despite different names*

### Comparing `ursa-major-0.4.2/ursa_major/cli.py` & `ursa-major-0.4.3/ursa_major/cli.py`

 * *Files identical despite different names*

### Comparing `ursa-major-0.4.2/ursa_major/handlers/add_module.py` & `ursa-major-0.4.3/ursa_major/handlers/add_module.py`

 * *Files identical despite different names*

### Comparing `ursa-major-0.4.2/ursa_major/handlers/add_tag.py` & `ursa-major-0.4.3/ursa_major/handlers/add_tag.py`

 * *Files identical despite different names*

### Comparing `ursa-major-0.4.2/ursa_major/handlers/base.py` & `ursa-major-0.4.3/ursa_major/handlers/base.py`

 * *Files identical despite different names*

### Comparing `ursa-major-0.4.2/ursa_major/handlers/check_config.py` & `ursa-major-0.4.3/ursa_major/handlers/check_config.py`

 * *Files identical despite different names*

### Comparing `ursa-major-0.4.2/ursa_major/handlers/remove_module.py` & `ursa-major-0.4.3/ursa_major/handlers/remove_module.py`

 * *Files identical despite different names*

### Comparing `ursa-major-0.4.2/ursa_major/handlers/show_config.py` & `ursa-major-0.4.3/ursa_major/handlers/show_config.py`

 * *Files identical despite different names*

### Comparing `ursa-major-0.4.2/ursa_major/handlers/update_tag.py` & `ursa-major-0.4.3/ursa_major/handlers/update_tag.py`

 * *Files identical despite different names*

### Comparing `ursa-major-0.4.2/ursa_major/koji_service.py` & `ursa-major-0.4.3/ursa_major/koji_service.py`

 * *Files 0% similar despite different names*

```diff
@@ -96,15 +96,15 @@
         if auth_type == 'ssl' or has_cert:
             self.koji_proxy.ssl_login(
                 os.path.expanduser(self.koji_module.config.cert),
                 os.path.expanduser(self.koji_module.config.ca),
                 os.path.expanduser(self.koji_module.config.serverca))
 
         elif auth_type == 'kerberos':
-            self.koji_proxy.krb_login(
+            self.koji_proxy.gssapi_login(
                 getattr(self.koji_module.config, 'principal', None),
                 getattr(self.koji_module.config, 'keytab', None))
         else:
             raise RuntimeError('Unsupported authentication type in Koji')
 
     def logout(self):
         """ expire the login session"""
```

### Comparing `ursa-major-0.4.2/ursa_major/logger.py` & `ursa-major-0.4.3/ursa_major/logger.py`

 * *Files identical despite different names*

### Comparing `ursa-major-0.4.2/ursa_major/mail.py` & `ursa-major-0.4.3/ursa_major/mail.py`

 * *Files identical despite different names*

### Comparing `ursa-major-0.4.2/ursa_major/mbs.py` & `ursa-major-0.4.3/ursa_major/mbs.py`

 * *Files identical despite different names*

### Comparing `ursa-major-0.4.2/ursa_major/utils.py` & `ursa-major-0.4.3/ursa_major/utils.py`

 * *Files identical despite different names*

### Comparing `ursa-major-0.4.2/ursa_major.egg-info/PKG-INFO` & `ursa-major-0.4.3/ursa_major.egg-info/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,444 +1,448 @@
-Metadata-Version: 1.1
+Metadata-Version: 2.1
 Name: ursa-major
-Version: 0.4.2
+Version: 0.4.3
 Summary: A utility for managing module tags in Koji's tag inheritance
 Home-page: https://pagure.io/ursa-major/
 Author: The Factory 2.0 Team
 Author-email: ursa-major-owner@fedoraproject.org
 License: MIT
-Description: Ursa-Major
-        ==========
-        
-        .. image:: https://img.shields.io/pypi/v/ursa-major.svg
-           :alt: PyPI
-        
-        .. image:: https://img.shields.io/pypi/l/ursa-major.svg
-           :alt: PyPI - License
-        
-        .. image:: https://img.shields.io/pypi/pyversions/ursa-major.svg
-           :alt: PyPI - Python Version
-        
-        Ursa-Major is a utility to help managing module's koji tags in koji's
-        inheritance. It reads configuration for tags from a tag config file, then
-        update koji's inheritance accordingly.
-        
-        Tag Config File
-        ---------------
-        
-        The tag config file used by Ursa-Major is in json format, the top level keys
-        are koji tags which we should add module tags into their inheritance. For each
-        tag, it contains a list of modules, owners can also be set for a tag.
-        
-        An example tag config file is:
-        
-        .. code-block:: json
-        
-            {
-                "fedora-30-buildroot-modules": {
-                    "modules": [
-                        {
-                            "name": "httpd",
-                            "priority": 10,
-                            "buildrequires": {
-                                "platform": "f30"
-                            },
-                            "requires": {
-                                "platform": "f30"
-                            },
-                            "stream": "2.4"
-                        },
-                        {
-                            "name": "ruby",
-                            "priority": 40,
-                            "requires": {
-                                "platform": "f30"
-                            },
-                            "stream": "2.5"
-                        }
-                    ],
-                    "owners": [
-                        "foo@example.com"
-                    ]
-                },
-                "fedora-30-test-build": {
-                    "modules": [
-                        {
-                            "name": "testmodule",
-                            "priority": 150,
-                            "stream": "f30"
-                        }
-                    ],
-                    "owners": [
-                        "bar@example.com"
-                    ]
-                }
-            }
-        
-        
-        A valid module config should contains:
-        
-        * ``name`` (required): module name
-        * ``stream`` (required): module stream
-        * ``priority`` (required): add module's tag to tag inheritance with this priority
-        * ``requires`` (optional): module's runtime dependencies.
-        * ``buildrequires`` (optional): module's build time dependencies.
-        
-        For each tag, ``owners`` can be set with email addresses.
-        
-        The default tag config file used by Ursa-Major is ``ursa-major.json`` in current
-        working directory. You can change it with ``--tag-config-file``.
-        
-        
-        Koji and MBS
-        ------------
-        
-        Tags in tag config file are koji tags, Ursa-Major connects to koji hub and
-        update tag inheritance per config, and connects to MBS to query module's
-        information, especially the modulemd data.
-        
-        Koji and MBS servers are set in Ursa-Major's config files, the global config
-        file is ``/etc/ursa-major/ursa-major`` by default, and can be changed by
-        ``--config`` argument. The user config file is
-        ``~/.config/ursa-major/ursa-major.conf``, and can be changed by
-        ``--user-config``. User config file is optional, and values in global config
-        file will be overrided by user config file.
-        
-        An example config file:
-        
-        .. code-block:: bash
-        
-            $ cat /etc/ursa-major/ursa-major.conf
-        
-            [main]
-            # See https://docs.python.org/3/library/logging.html#logging-levels
-            log_level = info
-        
-            [koji]
-            profile = koji
-        
-            [mbs]
-            server_url = https://mbs.fedoraproject.org/
-        
-            [mail]
-            mail_processing = true
-            mail_log_level = info
-            mail_server = smtp.example.com
-            mail_from = ursa-major@example.com
-            mail_replyto = ursa-major@example.com
-            # email addresses seperated by ','
-            mail_always_cc = ursa-major-admin@example.com
-            mail_always_bcc =
-            mail_subject_prefix = [ursa-major]
-        
-        
-        Sub Commands
-        ============
-        
-        Global arguments of ``ursa-major``:
-        
-        * ``--debug`` (optional): print debug messages
-        
-        * ``--dry-run`` (optional): run in dry-run mode, not do any real change
-        
-        * ``--config`` (optional): default if ``/etc/ursa-major/ursa-major.conf``
-        
-        * ``--user-config`` (optional): default is ``~/.config/ursa-major/ursa-major.conf``
-        
-        * ``--tag-config-file`` (optional): default is ``$PWD/ursa-major.json``
-        
-        
-        show-config
-        -----------
-        
-        This just show the content of tag config file, or the content of a specified
-        tag.
-        
-        Arguments:
-        
-        * ``--tag`` (optional): only show config content under this tag
-        
-        Example:
-        
-        .. code-block:: bash
-        
-            $ ursa-major show-config --tag-config-file ~/fedora-prod-ursa-major.json --tag fedora-30-test-build
-        
-        check-config
-        ------------
-        
-        Check the tag config file to detect any invalid configuration:
-        
-        .. code-block:: bash
-        
-            $ ursa-major check-config --tag-config-file ~/fedora-prod-ursa-major.json
-        
-        Checks include:
-        
-        * ``name``, ``stream`` and ``priority`` are required for a module
-        * ``priority`` value should not conflict with other parent tags which not belong
-          to this module in tag's inheritance
-        * ...
-        
-        remove-module
-        -------------
-        
-        Remove a module from the tag config file.
-        
-        Arguments:
-        
-        * ``--tag`` (required): remove module from this tag
-        
-        * ``--name`` (required): module name
-        
-        * ``--stream`` (required): module stream
-        
-        * ``--require`` (optional): module's runtime requires, can be specified multiple times
-        
-        * ``--buildrequire`` (optional): module's buildrequires, can be specified multiple times
-        
-        
-        Example:
-        
-        .. code-block:: bash
-        
-            $ ursa-major remove-module --tag fedora-30-test-build --name testmodule --stream f30
-        
-        This will remove the module of ``testmodule:f30`` from tag config file if it's
-        s present under tag ``fedora-30-test-build``.
-        
-        add-module
-        ----------
-        
-        Add a module to tag config file under the specified tag.
-        
-        Arguments:
-        
-        * ``--tag`` (required): add module to this tag
-        
-        * ``--name`` (required): module name
-        
-        * ``--stream`` (required): module stream
-        
-        * ``--priority`` (required): priority value when add tag to inheritance
-        
-        * ``--require`` (optional): module's runtime requires, can be specified multiple times
-        
-        * ``--buildrequire`` (optional): module's buildrequires, can be specified multiple times
-        
-        Example:
-        
-        .. code-block:: bash
-        
-            $ ursa-major add-module --tag fedora-30-test-build --name testmodule --stream f30 --priority 100
-        
-        If the specified module with that ``name`` and ``stream`` already exists in tag
-        config file, Ursa-Major will check whether ``requires`` or ``priority`` is
-        different from the value specified in command line, if true, the tag config
-        file will be updated to use the values specified.
-        
-        update-tag
-        ----------
-        
-        Update a tag's inheritance data with all latest module build tags of the
-        modules in tag's config.
-        
-        Arguments:
-        
-        * ``--tag`` (required): the tag to update
-        * ``--wait-regen-repo`` (optional): wait for regen-repo task to finish
-        
-        Example:
-        
-        .. code-block:: bash
-        
-            $ ursa-major update-tag --tag fedora-30-test-build --wait-regen-repo
-        
-        This will check the latest builds in MBS for all modules in config of tag
-        'fedora-30-test-build', if there is any build's tag is missing from tag's
-        inheritance data, the tag will be added into inheritance, and old tags
-        will be removed at the same time for the module.
-        
-        add-tag
-        -------
-        
-        Reads module state change message from an environment variable and then add
-        the module's koji tag tag inheritance according to tag config file if the
-        module build state is 'ready', and remove old tags of the module at the same
-        time. The module's state change message is generated by MBS.
-        
-        Arguments:
-        
-        * ``--module-from-env`` (optional): the environment variable Ursa-Major read the
-          module state change message from, by default it's ``CI_MESSAGE``
-        
-        * ``--wait-regen-repo`` (optinal): wait for regen-repo tasks to finish, default is ``False``
-        
-        * ``--send-mail`` (optional): send mail to tag owners, default is ``False``
-        
-        Example:
-        
-        .. code-block:: bash
-        
-            $ cat $CI_MESSAGE
-            {
-              "state_reason": null,
-              "component_builds": [
-                108146,
-                108145
-              ],
-              "name": "testmodule",
-              "stream": "master",
-              "time_submitted": "2018-10-26T16:59:06Z",
-              "version": "20181026165847",
-              "time_modified": "2018-10-26T16:59:27Z",
-              "state_name": "ready",
-              "scmurl": "https://src.fedoraproject.org/modules/testmodule.git?#3f262deef9d79160ea229142aeb51eedcc956929",
-              "state": 5,
-              "time_completed": "2018-10-26T16:59:15Z",
-              "koji_tag": "module-testmodule-master-20181026165847-a5b0195c",
-              "context": "a5b0195c",
-              "owner": "foobar",
-              "siblings": [],
-              "id": 2321,
-              "rebuild_strategy": "only-changed"
-            }
-        
-            $ cat $PWD/ursa-major.json
-            {
-                "fedora-30-test-build": {
-                    "modules": [
-                        {
-                            "name": "testmodule",
-                            "priority": 150,
-                            "stream": "master"
-                        }
-                    ],
-                    "owners": [
-                        "foobar@example.com"
-                    ]
-                }
-            }
-        
-            $ ursa-major add-tag --wait-regen-repo --send-mail
-        
-        In this example, Ursa-Major reads the module state change message from
-        enviroment variable ``CI_MESSAGE``, the module build state name is "ready" and
-        module is present under a tag "fedora-30-test-build" in tag config file.
-        Ursa-Major will add the koji tag "module-testmodule-master-20181026165847-a5b0195c"
-        into "fedora-30-test-build"'s inheritance, and then regen-repo for build tags
-        in "fedora-30-test-build"'s inheritance.
-        
-        When a tag is added to tag inheritance, Ursa-Major also submit ``regen-repo``
-        tasks for the build tags in inheritance data. If the specified tag is a build
-        tag, it's the only one build tag Ursa-Major will regen-repo for. Or Ursa-Major
-        will check the tag's inheritance data, if it reaches the first build tag in
-        each inheritant path, it returns that build tag. And it stops at any tag that
-        name starts with 'module-'.
-        
-        For example, if we have tag inheritance data as below (tags with
-        '*' marks are build tags):
-        
-        Example #1:
-        
-        ::
-        
-                my-example-tag
-                  └─product-foo-temp-override
-                     └─product-foo-override
-                        └─product-foo-build (*)
-                           ├─tmp-product-foo-build (*)
-                           └─alt-product-foo-build (*)
-        
-        In this case, there is one build tag found for 'my-example-tag', it is:
-        ``product-foo-build``. Ursa-Major stops at 'product-foo-build', so
-        'tmp-product-foo-build' and 'alt-product-foo-build' are not checked at all.
-        
-        Example #2:
-        
-        ::
-        
-            my-example-tag
-              ├─module-345678-build
-              ├─module-234567-build
-              ├─module-123456-build
-              │  └─product-foo-module-hotfix
-              │     └─product-foo-module-hotfix-build (*)
-              ├─tmp-product-foo-python-candidate
-              │  └─tmp-product-foo-python-override
-              │     └─tmp-product-foo-python-build (*)
-              ├─product-foo-container-build (*)
-              └─product-foo-temp-override
-                 └─product-foo-override
-                    └─product-foo-build (*)
-                       ├─tmp-product-foo-build (*)
-                       └─alt-product-foo-build (*)
-        
-        In this case, there are 3 build tags found for ``my-example-tag``, they are:
-        ``tmp-product-foo-python-build``, ``product-foo-container-build`` and
-        ``product-foo-build``. ``product-foo-module-hotfix-build`` is a build tag, but
-        Ursa-Major doesn't count it in, because it stops at tag 'module-123456-build'
-        which name starts with 'module-'.
-        
-        Ursa-Major will send mail to tag owners if run with "--send-mail", mail
-        configuration can be configured in global config file or user config file,
-        under the section of "mail".
-        
-        
-        Change Logs
-        ===========
-        0.4.2 (2021-03-10)
-        ------------------
-        * Use old tuple syntax for mock.call.call_args of old mock release (Yuming Zhu)
-        * Fix unittests for missing koji profile (Yuming Zhu)
-        * Using libmodulemd v2 API (Yuming Zhu)
-        
-        0.4.1 (2020-02-11)
-        ------------------
-        * Remove updating koji inheritance ability from add-module and remove-module (Qixiang Wan)
-        
-        0.3.3 (2019-08-23)
-        ------------------
-        * Add new sub command update-tag (Qixiang Wan)
-        
-        0.3.2 (2019-06-26)
-        ------------------
-        * Include garbaged module builds while checking existing module build tags (Qixiang Wan)
-        * Refactor get_modules (Qixiang Wan)
-        
-        0.3.1 (2019-05-21)
-        ------------------
-        
-        * Not check requires/buildrequires for existing koji tags (Qixiang Wan)
-        * Updating existing inheritance instead of removing and adding (Qixiang Wan)
-        
-        0.2.2 (2019-03-26)
-        ------------------
-        
-        * For adding tag, allow filtering on buildrequires to find out koji_tags from
-          tag inheritance (Chenxiong Qi)
-        
-        0.2.1 (2019-03-20)
-        ------------------
-        
-        * Make setup_method/teardown_method compatible with newer version of pytest (Chenxiong Qi)
-        * Add missing file CHANGELOG.rst to sdist package (Chenxiong Qi)
-        
-        0.2.0 (2019-03-20)
-        ------------------
-        
-        * Add tests for AddModuleHandler methods (Chenxiong Qi)
-        * Avoid long modulemd embedded into fake data for tests (Chenxiong Qi)
-        * Fixes according to review comments (Chenxiong Qi)
-        * Command check-config supports filtering modules on buildrequires (Chenxiong Qi)
-        * Command add-module supports buildrequires now (Chenxiong Qi)
-        * Command remove-module supports filtering modules on buildrequires (Chenxiong Qi)
-        * Allow passing buildrequires to MBS.get_modules_with_requires (Chenxiong Qi)
-        * Reword remove-module help and --tag option help text (Chenxiong Qi)
-        * Allow filtering on buildrequires (Chenxiong Qi)
-        
-        
 Keywords: ursa-major modularity koji fedora
-Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 2.7
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Topic :: Utilities
+License-File: LICENSE
+
+Ursa-Major
+==========
+
+.. image:: https://img.shields.io/pypi/v/ursa-major.svg
+   :alt: PyPI
+
+.. image:: https://img.shields.io/pypi/l/ursa-major.svg
+   :alt: PyPI - License
+
+.. image:: https://img.shields.io/pypi/pyversions/ursa-major.svg
+   :alt: PyPI - Python Version
+
+Ursa-Major is a utility to help managing module's koji tags in koji's
+inheritance. It reads configuration for tags from a tag config file, then
+update koji's inheritance accordingly.
+
+Tag Config File
+---------------
+
+The tag config file used by Ursa-Major is in json format, the top level keys
+are koji tags which we should add module tags into their inheritance. For each
+tag, it contains a list of modules, owners can also be set for a tag.
+
+An example tag config file is:
+
+.. code-block:: json
+
+    {
+        "fedora-30-buildroot-modules": {
+            "modules": [
+                {
+                    "name": "httpd",
+                    "priority": 10,
+                    "buildrequires": {
+                        "platform": "f30"
+                    },
+                    "requires": {
+                        "platform": "f30"
+                    },
+                    "stream": "2.4"
+                },
+                {
+                    "name": "ruby",
+                    "priority": 40,
+                    "requires": {
+                        "platform": "f30"
+                    },
+                    "stream": "2.5"
+                }
+            ],
+            "owners": [
+                "foo@example.com"
+            ]
+        },
+        "fedora-30-test-build": {
+            "modules": [
+                {
+                    "name": "testmodule",
+                    "priority": 150,
+                    "stream": "f30"
+                }
+            ],
+            "owners": [
+                "bar@example.com"
+            ]
+        }
+    }
+
+
+A valid module config should contains:
+
+* ``name`` (required): module name
+* ``stream`` (required): module stream
+* ``priority`` (required): add module's tag to tag inheritance with this priority
+* ``requires`` (optional): module's runtime dependencies.
+* ``buildrequires`` (optional): module's build time dependencies.
+
+For each tag, ``owners`` can be set with email addresses.
+
+The default tag config file used by Ursa-Major is ``ursa-major.json`` in current
+working directory. You can change it with ``--tag-config-file``.
+
+
+Koji and MBS
+------------
+
+Tags in tag config file are koji tags, Ursa-Major connects to koji hub and
+update tag inheritance per config, and connects to MBS to query module's
+information, especially the modulemd data.
+
+Koji and MBS servers are set in Ursa-Major's config files, the global config
+file is ``/etc/ursa-major/ursa-major`` by default, and can be changed by
+``--config`` argument. The user config file is
+``~/.config/ursa-major/ursa-major.conf``, and can be changed by
+``--user-config``. User config file is optional, and values in global config
+file will be overrided by user config file.
+
+An example config file:
+
+.. code-block:: bash
+
+    $ cat /etc/ursa-major/ursa-major.conf
+
+    [main]
+    # See https://docs.python.org/3/library/logging.html#logging-levels
+    log_level = info
+
+    [koji]
+    profile = koji
+
+    [mbs]
+    server_url = https://mbs.fedoraproject.org/
+
+    [mail]
+    mail_processing = true
+    mail_log_level = info
+    mail_server = smtp.example.com
+    mail_from = ursa-major@example.com
+    mail_replyto = ursa-major@example.com
+    # email addresses seperated by ','
+    mail_always_cc = ursa-major-admin@example.com
+    mail_always_bcc =
+    mail_subject_prefix = [ursa-major]
+
+
+Sub Commands
+============
+
+Global arguments of ``ursa-major``:
+
+* ``--debug`` (optional): print debug messages
+
+* ``--dry-run`` (optional): run in dry-run mode, not do any real change
+
+* ``--config`` (optional): default if ``/etc/ursa-major/ursa-major.conf``
+
+* ``--user-config`` (optional): default is ``~/.config/ursa-major/ursa-major.conf``
+
+* ``--tag-config-file`` (optional): default is ``$PWD/ursa-major.json``
+
+
+show-config
+-----------
+
+This just show the content of tag config file, or the content of a specified
+tag.
+
+Arguments:
+
+* ``--tag`` (optional): only show config content under this tag
+
+Example:
+
+.. code-block:: bash
+
+    $ ursa-major show-config --tag-config-file ~/fedora-prod-ursa-major.json --tag fedora-30-test-build
+
+check-config
+------------
+
+Check the tag config file to detect any invalid configuration:
+
+.. code-block:: bash
+
+    $ ursa-major check-config --tag-config-file ~/fedora-prod-ursa-major.json
+
+Checks include:
+
+* ``name``, ``stream`` and ``priority`` are required for a module
+* ``priority`` value should not conflict with other parent tags which not belong
+  to this module in tag's inheritance
+* ...
+
+remove-module
+-------------
+
+Remove a module from the tag config file.
+
+Arguments:
+
+* ``--tag`` (required): remove module from this tag
+
+* ``--name`` (required): module name
+
+* ``--stream`` (required): module stream
+
+* ``--require`` (optional): module's runtime requires, can be specified multiple times
+
+* ``--buildrequire`` (optional): module's buildrequires, can be specified multiple times
+
+
+Example:
+
+.. code-block:: bash
+
+    $ ursa-major remove-module --tag fedora-30-test-build --name testmodule --stream f30
+
+This will remove the module of ``testmodule:f30`` from tag config file if it's
+s present under tag ``fedora-30-test-build``.
+
+add-module
+----------
+
+Add a module to tag config file under the specified tag.
+
+Arguments:
+
+* ``--tag`` (required): add module to this tag
+
+* ``--name`` (required): module name
+
+* ``--stream`` (required): module stream
+
+* ``--priority`` (required): priority value when add tag to inheritance
+
+* ``--require`` (optional): module's runtime requires, can be specified multiple times
+
+* ``--buildrequire`` (optional): module's buildrequires, can be specified multiple times
+
+Example:
+
+.. code-block:: bash
+
+    $ ursa-major add-module --tag fedora-30-test-build --name testmodule --stream f30 --priority 100
+
+If the specified module with that ``name`` and ``stream`` already exists in tag
+config file, Ursa-Major will check whether ``requires`` or ``priority`` is
+different from the value specified in command line, if true, the tag config
+file will be updated to use the values specified.
+
+update-tag
+----------
+
+Update a tag's inheritance data with all latest module build tags of the
+modules in tag's config.
+
+Arguments:
+
+* ``--tag`` (required): the tag to update
+* ``--wait-regen-repo`` (optional): wait for regen-repo task to finish
+
+Example:
+
+.. code-block:: bash
+
+    $ ursa-major update-tag --tag fedora-30-test-build --wait-regen-repo
+
+This will check the latest builds in MBS for all modules in config of tag
+'fedora-30-test-build', if there is any build's tag is missing from tag's
+inheritance data, the tag will be added into inheritance, and old tags
+will be removed at the same time for the module.
+
+add-tag
+-------
+
+Reads module state change message from an environment variable and then add
+the module's koji tag tag inheritance according to tag config file if the
+module build state is 'ready', and remove old tags of the module at the same
+time. The module's state change message is generated by MBS.
+
+Arguments:
+
+* ``--module-from-env`` (optional): the environment variable Ursa-Major read the
+  module state change message from, by default it's ``CI_MESSAGE``
+
+* ``--wait-regen-repo`` (optinal): wait for regen-repo tasks to finish, default is ``False``
+
+* ``--send-mail`` (optional): send mail to tag owners, default is ``False``
+
+Example:
+
+.. code-block:: bash
+
+    $ cat $CI_MESSAGE
+    {
+      "state_reason": null,
+      "component_builds": [
+        108146,
+        108145
+      ],
+      "name": "testmodule",
+      "stream": "master",
+      "time_submitted": "2018-10-26T16:59:06Z",
+      "version": "20181026165847",
+      "time_modified": "2018-10-26T16:59:27Z",
+      "state_name": "ready",
+      "scmurl": "https://src.fedoraproject.org/modules/testmodule.git?#3f262deef9d79160ea229142aeb51eedcc956929",
+      "state": 5,
+      "time_completed": "2018-10-26T16:59:15Z",
+      "koji_tag": "module-testmodule-master-20181026165847-a5b0195c",
+      "context": "a5b0195c",
+      "owner": "foobar",
+      "siblings": [],
+      "id": 2321,
+      "rebuild_strategy": "only-changed"
+    }
+
+    $ cat $PWD/ursa-major.json
+    {
+        "fedora-30-test-build": {
+            "modules": [
+                {
+                    "name": "testmodule",
+                    "priority": 150,
+                    "stream": "master"
+                }
+            ],
+            "owners": [
+                "foobar@example.com"
+            ]
+        }
+    }
+
+    $ ursa-major add-tag --wait-regen-repo --send-mail
+
+In this example, Ursa-Major reads the module state change message from
+enviroment variable ``CI_MESSAGE``, the module build state name is "ready" and
+module is present under a tag "fedora-30-test-build" in tag config file.
+Ursa-Major will add the koji tag "module-testmodule-master-20181026165847-a5b0195c"
+into "fedora-30-test-build"'s inheritance, and then regen-repo for build tags
+in "fedora-30-test-build"'s inheritance.
+
+When a tag is added to tag inheritance, Ursa-Major also submit ``regen-repo``
+tasks for the build tags in inheritance data. If the specified tag is a build
+tag, it's the only one build tag Ursa-Major will regen-repo for. Or Ursa-Major
+will check the tag's inheritance data, if it reaches the first build tag in
+each inheritant path, it returns that build tag. And it stops at any tag that
+name starts with 'module-'.
+
+For example, if we have tag inheritance data as below (tags with
+'*' marks are build tags):
+
+Example #1:
+
+::
+
+        my-example-tag
+          └─product-foo-temp-override
+             └─product-foo-override
+                └─product-foo-build (*)
+                   ├─tmp-product-foo-build (*)
+                   └─alt-product-foo-build (*)
+
+In this case, there is one build tag found for 'my-example-tag', it is:
+``product-foo-build``. Ursa-Major stops at 'product-foo-build', so
+'tmp-product-foo-build' and 'alt-product-foo-build' are not checked at all.
+
+Example #2:
+
+::
+
+    my-example-tag
+      ├─module-345678-build
+      ├─module-234567-build
+      ├─module-123456-build
+      │  └─product-foo-module-hotfix
+      │     └─product-foo-module-hotfix-build (*)
+      ├─tmp-product-foo-python-candidate
+      │  └─tmp-product-foo-python-override
+      │     └─tmp-product-foo-python-build (*)
+      ├─product-foo-container-build (*)
+      └─product-foo-temp-override
+         └─product-foo-override
+            └─product-foo-build (*)
+               ├─tmp-product-foo-build (*)
+               └─alt-product-foo-build (*)
+
+In this case, there are 3 build tags found for ``my-example-tag``, they are:
+``tmp-product-foo-python-build``, ``product-foo-container-build`` and
+``product-foo-build``. ``product-foo-module-hotfix-build`` is a build tag, but
+Ursa-Major doesn't count it in, because it stops at tag 'module-123456-build'
+which name starts with 'module-'.
+
+Ursa-Major will send mail to tag owners if run with "--send-mail", mail
+configuration can be configured in global config file or user config file,
+under the section of "mail".
+
+
+Change Logs
+===========
+0.4.2 (2023-06-27)
+------------------
+* Use gssapi_login instead of krb_login for koji kerberos auth (Yuming Zhu)
+
+0.4.2 (2021-03-10)
+------------------
+* Use old tuple syntax for mock.call.call_args of old mock release (Yuming Zhu)
+* Fix unittests for missing koji profile (Yuming Zhu)
+* Using libmodulemd v2 API (Yuming Zhu)
+
+0.4.1 (2020-02-11)
+------------------
+* Remove updating koji inheritance ability from add-module and remove-module (Qixiang Wan)
+
+0.3.3 (2019-08-23)
+------------------
+* Add new sub command update-tag (Qixiang Wan)
+
+0.3.2 (2019-06-26)
+------------------
+* Include garbaged module builds while checking existing module build tags (Qixiang Wan)
+* Refactor get_modules (Qixiang Wan)
+
+0.3.1 (2019-05-21)
+------------------
+
+* Not check requires/buildrequires for existing koji tags (Qixiang Wan)
+* Updating existing inheritance instead of removing and adding (Qixiang Wan)
+
+0.2.2 (2019-03-26)
+------------------
+
+* For adding tag, allow filtering on buildrequires to find out koji_tags from
+  tag inheritance (Chenxiong Qi)
+
+0.2.1 (2019-03-20)
+------------------
+
+* Make setup_method/teardown_method compatible with newer version of pytest (Chenxiong Qi)
+* Add missing file CHANGELOG.rst to sdist package (Chenxiong Qi)
+
+0.2.0 (2019-03-20)
+------------------
+
+* Add tests for AddModuleHandler methods (Chenxiong Qi)
+* Avoid long modulemd embedded into fake data for tests (Chenxiong Qi)
+* Fixes according to review comments (Chenxiong Qi)
+* Command check-config supports filtering modules on buildrequires (Chenxiong Qi)
+* Command add-module supports buildrequires now (Chenxiong Qi)
+* Command remove-module supports filtering modules on buildrequires (Chenxiong Qi)
+* Allow passing buildrequires to MBS.get_modules_with_requires (Chenxiong Qi)
+* Reword remove-module help and --tag option help text (Chenxiong Qi)
+* Allow filtering on buildrequires (Chenxiong Qi)
+
```

### Comparing `ursa-major-0.4.2/ursa_major.egg-info/SOURCES.txt` & `ursa-major-0.4.3/ursa_major.egg-info/SOURCES.txt`

 * *Files identical despite different names*

