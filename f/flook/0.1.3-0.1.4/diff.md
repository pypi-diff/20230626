# Comparing `tmp/flook-0.1.3.tar.gz` & `tmp/flook-0.1.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "flook-0.1.3.tar", last modified: Sun Jun 25 11:40:42 2023, max compression
+gzip compressed data, was "flook-0.1.4.tar", last modified: Sun Jun 25 23:59:01 2023, max compression
```

## Comparing `flook-0.1.3.tar` & `flook-0.1.4.tar`

### file list

```diff
@@ -1,65 +1,68 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-25 11:40:42.983288 flook-0.1.3/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-25 11:40:42.979288 flook-0.1.3/.github/
--rw-r--r--   0 runner    (1001) docker     (123)      120 2023-06-25 11:40:20.000000 flook-0.1.3/.github/CODEOWNERS
--rw-r--r--   0 runner    (1001) docker     (123)       47 2023-06-25 11:40:20.000000 flook-0.1.3/.github/FUNDING.yml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-25 11:40:42.979288 flook-0.1.3/.github/ISSUE_TEMPLATE/
--rw-r--r--   0 runner    (1001) docker     (123)      329 2023-06-25 11:40:20.000000 flook-0.1.3/.github/ISSUE_TEMPLATE/bug_report.md
--rw-r--r--   0 runner    (1001) docker     (123)      458 2023-06-25 11:40:20.000000 flook-0.1.3/.github/ISSUE_TEMPLATE/feature_request.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-25 11:40:42.979288 flook-0.1.3/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)      494 2023-06-25 11:40:20.000000 flook-0.1.3/.github/workflows/ci.yml
--rw-r--r--   0 runner    (1001) docker     (123)      573 2023-06-25 11:40:20.000000 flook-0.1.3/.github/workflows/release.yml
--rw-r--r--   0 runner    (1001) docker     (123)      564 2023-06-25 11:40:20.000000 flook-0.1.3/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)       68 2023-06-25 11:40:20.000000 flook-0.1.3/AUTHORS.rst
--rw-r--r--   0 runner    (1001) docker     (123)       79 2023-06-25 11:40:20.000000 flook-0.1.3/CHANGELOG.rst
--rw-r--r--   0 runner    (1001) docker     (123)     5219 2023-06-25 11:40:20.000000 flook-0.1.3/CODE_OF_CONDUCT.md
--rw-r--r--   0 runner    (1001) docker     (123)      742 2023-06-25 11:40:20.000000 flook-0.1.3/CONTRIBUTING.rst
--rw-r--r--   0 runner    (1001) docker     (123)     1074 2023-06-25 11:40:20.000000 flook-0.1.3/LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (123)      939 2023-06-25 11:40:20.000000 flook-0.1.3/Makefile
--rw-r--r--   0 runner    (1001) docker     (123)     1569 2023-06-25 11:40:42.983288 flook-0.1.3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      792 2023-06-25 11:40:20.000000 flook-0.1.3/README.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-25 11:40:42.979288 flook-0.1.3/cache/
--rw-r--r--   0 runner    (1001) docker     (123)       13 2023-06-25 11:40:20.000000 flook-0.1.3/cache/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)      250 2023-06-25 11:40:20.000000 flook-0.1.3/pyproject.toml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-25 11:40:42.979288 flook-0.1.3/recipe/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-25 11:40:42.979288 flook-0.1.3/recipe/nginx/
--rw-r--r--   0 runner    (1001) docker     (123)      454 2023-06-25 11:40:20.000000 flook-0.1.3/recipe/nginx/motd.j2
--rw-r--r--   0 runner    (1001) docker     (123)      546 2023-06-25 11:40:20.000000 flook-0.1.3/recipe/nginx/recipe.yml
--rw-r--r--   0 runner    (1001) docker     (123)       41 2023-06-25 11:40:20.000000 flook-0.1.3/renovate.json
--rw-r--r--   0 runner    (1001) docker     (123)     1494 2023-06-25 11:40:42.983288 flook-0.1.3/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1553 2023-06-25 11:40:20.000000 flook-0.1.3/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-25 11:40:42.979288 flook-0.1.3/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-25 11:40:42.979288 flook-0.1.3/src/flook/
--rw-r--r--   0 runner    (1001) docker     (123)     1681 2023-06-25 11:40:20.000000 flook-0.1.3/src/flook/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5669 2023-06-25 11:40:20.000000 flook-0.1.3/src/flook/cli.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-25 11:40:42.983288 flook-0.1.3/src/flook/command/
--rw-r--r--   0 runner    (1001) docker     (123)     1102 2023-06-25 11:40:20.000000 flook-0.1.3/src/flook/command/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3150 2023-06-25 11:40:20.000000 flook-0.1.3/src/flook/command/configs.py
--rw-r--r--   0 runner    (1001) docker     (123)     3849 2023-06-25 11:40:20.000000 flook-0.1.3/src/flook/command/hosts.py
--rw-r--r--   0 runner    (1001) docker     (123)     4670 2023-06-25 11:40:20.000000 flook-0.1.3/src/flook/command/recipes.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-25 11:40:42.983288 flook-0.1.3/src/flook/exception/
--rw-r--r--   0 runner    (1001) docker     (123)     1102 2023-06-25 11:40:20.000000 flook-0.1.3/src/flook/exception/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-25 11:40:42.983288 flook-0.1.3/src/flook/module/
--rw-r--r--   0 runner    (1001) docker     (123)     1102 2023-06-25 11:40:20.000000 flook-0.1.3/src/flook/module/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2005 2023-06-25 11:40:20.000000 flook-0.1.3/src/flook/module/ansible.py
--rw-r--r--   0 runner    (1001) docker     (123)     1571 2023-06-25 11:40:20.000000 flook-0.1.3/src/flook/module/config.py
--rw-r--r--   0 runner    (1001) docker     (123)     4764 2023-06-25 11:40:20.000000 flook-0.1.3/src/flook/module/database.py
--rw-r--r--   0 runner    (1001) docker     (123)     3440 2023-06-25 11:40:20.000000 flook-0.1.3/src/flook/module/file_system.py
--rw-r--r--   0 runner    (1001) docker     (123)     1548 2023-06-25 11:40:20.000000 flook-0.1.3/src/flook/module/logger.py
--rw-r--r--   0 runner    (1001) docker     (123)     1808 2023-06-25 11:40:20.000000 flook-0.1.3/src/flook/module/output.py
--rw-r--r--   0 runner    (1001) docker     (123)     1292 2023-06-25 11:40:20.000000 flook-0.1.3/src/flook/module/playbook.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-25 11:40:42.983288 flook-0.1.3/src/flook.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1569 2023-06-25 11:40:42.000000 flook-0.1.3/src/flook.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1170 2023-06-25 11:40:42.000000 flook-0.1.3/src/flook.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-25 11:40:42.000000 flook-0.1.3/src/flook.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       41 2023-06-25 11:40:42.000000 flook-0.1.3/src/flook.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-25 11:40:42.000000 flook-0.1.3/src/flook.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)      126 2023-06-25 11:40:42.000000 flook-0.1.3/src/flook.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        6 2023-06-25 11:40:42.000000 flook-0.1.3/src/flook.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-25 11:40:42.983288 flook-0.1.3/tests/
--rw-r--r--   0 runner    (1001) docker     (123)     1102 2023-06-25 11:40:20.000000 flook-0.1.3/tests/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-25 11:40:42.983288 flook-0.1.3/tests/module/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-25 11:40:20.000000 flook-0.1.3/tests/module/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1511 2023-06-25 11:40:20.000000 flook-0.1.3/tests/module/test_database.py
--rw-r--r--   0 runner    (1001) docker     (123)     1325 2023-06-25 11:40:20.000000 flook-0.1.3/tests/module/test_logger.py
--rw-r--r--   0 runner    (1001) docker     (123)     1501 2023-06-25 11:40:20.000000 flook-0.1.3/tests/module/test_output.py
--rw-r--r--   0 runner    (1001) docker     (123)      719 2023-06-25 11:40:20.000000 flook-0.1.3/tox.ini
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-25 23:59:01.437313 flook-0.1.4/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-25 23:59:01.433313 flook-0.1.4/.github/
+-rw-r--r--   0 runner    (1001) docker     (123)      120 2023-06-25 23:58:41.000000 flook-0.1.4/.github/CODEOWNERS
+-rw-r--r--   0 runner    (1001) docker     (123)       47 2023-06-25 23:58:41.000000 flook-0.1.4/.github/FUNDING.yml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-25 23:59:01.433313 flook-0.1.4/.github/ISSUE_TEMPLATE/
+-rw-r--r--   0 runner    (1001) docker     (123)      329 2023-06-25 23:58:41.000000 flook-0.1.4/.github/ISSUE_TEMPLATE/bug_report.md
+-rw-r--r--   0 runner    (1001) docker     (123)      458 2023-06-25 23:58:41.000000 flook-0.1.4/.github/ISSUE_TEMPLATE/feature_request.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-25 23:59:01.433313 flook-0.1.4/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)      494 2023-06-25 23:58:41.000000 flook-0.1.4/.github/workflows/ci.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      573 2023-06-25 23:58:41.000000 flook-0.1.4/.github/workflows/release.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      564 2023-06-25 23:58:41.000000 flook-0.1.4/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)       68 2023-06-25 23:58:41.000000 flook-0.1.4/AUTHORS.rst
+-rw-r--r--   0 runner    (1001) docker     (123)       79 2023-06-25 23:58:41.000000 flook-0.1.4/CHANGELOG.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     5219 2023-06-25 23:58:41.000000 flook-0.1.4/CODE_OF_CONDUCT.md
+-rw-r--r--   0 runner    (1001) docker     (123)      742 2023-06-25 23:58:41.000000 flook-0.1.4/CONTRIBUTING.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1074 2023-06-25 23:58:41.000000 flook-0.1.4/LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      939 2023-06-25 23:58:41.000000 flook-0.1.4/Makefile
+-rw-r--r--   0 runner    (1001) docker     (123)     1569 2023-06-25 23:59:01.437313 flook-0.1.4/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      792 2023-06-25 23:58:41.000000 flook-0.1.4/README.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-25 23:59:01.433313 flook-0.1.4/cache/
+-rw-r--r--   0 runner    (1001) docker     (123)       13 2023-06-25 23:58:41.000000 flook-0.1.4/cache/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)      250 2023-06-25 23:58:41.000000 flook-0.1.4/pyproject.toml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-25 23:59:01.429313 flook-0.1.4/recipe/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-25 23:59:01.433313 flook-0.1.4/recipe/nginx/
+-rw-r--r--   0 runner    (1001) docker     (123)      454 2023-06-25 23:58:41.000000 flook-0.1.4/recipe/nginx/motd.j2
+-rw-r--r--   0 runner    (1001) docker     (123)      546 2023-06-25 23:58:41.000000 flook-0.1.4/recipe/nginx/recipe.yml
+-rw-r--r--   0 runner    (1001) docker     (123)       41 2023-06-25 23:58:41.000000 flook-0.1.4/renovate.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1494 2023-06-25 23:59:01.437313 flook-0.1.4/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1553 2023-06-25 23:58:41.000000 flook-0.1.4/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-25 23:59:01.429313 flook-0.1.4/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-25 23:59:01.433313 flook-0.1.4/src/flook/
+-rw-r--r--   0 runner    (1001) docker     (123)     1681 2023-06-25 23:58:41.000000 flook-0.1.4/src/flook/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6039 2023-06-25 23:58:41.000000 flook-0.1.4/src/flook/cli.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-25 23:59:01.433313 flook-0.1.4/src/flook/command/
+-rw-r--r--   0 runner    (1001) docker     (123)     1102 2023-06-25 23:58:41.000000 flook-0.1.4/src/flook/command/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3150 2023-06-25 23:58:41.000000 flook-0.1.4/src/flook/command/configs.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3821 2023-06-25 23:58:41.000000 flook-0.1.4/src/flook/command/hosts.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5051 2023-06-25 23:58:41.000000 flook-0.1.4/src/flook/command/recipes.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-25 23:59:01.433313 flook-0.1.4/src/flook/exception/
+-rw-r--r--   0 runner    (1001) docker     (123)     1102 2023-06-25 23:58:41.000000 flook-0.1.4/src/flook/exception/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-25 23:59:01.433313 flook-0.1.4/src/flook/model/
+-rw-r--r--   0 runner    (1001) docker     (123)     1102 2023-06-25 23:58:41.000000 flook-0.1.4/src/flook/model/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2750 2023-06-25 23:58:41.000000 flook-0.1.4/src/flook/model/host.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2131 2023-06-25 23:58:41.000000 flook-0.1.4/src/flook/model/recipe.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1986 2023-06-25 23:58:41.000000 flook-0.1.4/src/flook/model/task.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-25 23:59:01.437313 flook-0.1.4/src/flook/module/
+-rw-r--r--   0 runner    (1001) docker     (123)     1102 2023-06-25 23:58:41.000000 flook-0.1.4/src/flook/module/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2005 2023-06-25 23:58:41.000000 flook-0.1.4/src/flook/module/ansible.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1571 2023-06-25 23:58:41.000000 flook-0.1.4/src/flook/module/config.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7049 2023-06-25 23:58:41.000000 flook-0.1.4/src/flook/module/database.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3440 2023-06-25 23:58:41.000000 flook-0.1.4/src/flook/module/file_system.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1548 2023-06-25 23:58:41.000000 flook-0.1.4/src/flook/module/logger.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2145 2023-06-25 23:58:41.000000 flook-0.1.4/src/flook/module/output.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1476 2023-06-25 23:58:41.000000 flook-0.1.4/src/flook/module/playbook.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-25 23:59:01.433313 flook-0.1.4/src/flook.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1569 2023-06-25 23:59:01.000000 flook-0.1.4/src/flook.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1214 2023-06-25 23:59:01.000000 flook-0.1.4/src/flook.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-25 23:59:01.000000 flook-0.1.4/src/flook.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       41 2023-06-25 23:59:01.000000 flook-0.1.4/src/flook.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-25 23:59:01.000000 flook-0.1.4/src/flook.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)      126 2023-06-25 23:59:01.000000 flook-0.1.4/src/flook.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        6 2023-06-25 23:59:01.000000 flook-0.1.4/src/flook.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-25 23:59:01.437313 flook-0.1.4/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     1102 2023-06-25 23:58:41.000000 flook-0.1.4/tests/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-25 23:59:01.437313 flook-0.1.4/tests/module/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-25 23:58:41.000000 flook-0.1.4/tests/module/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1325 2023-06-25 23:58:41.000000 flook-0.1.4/tests/module/test_logger.py
+-rw-r--r--   0 runner    (1001) docker     (123)      719 2023-06-25 23:58:41.000000 flook-0.1.4/tox.ini
```

### Comparing `flook-0.1.3/.github/workflows/release.yml` & `flook-0.1.4/.github/workflows/release.yml`

 * *Files identical despite different names*

### Comparing `flook-0.1.3/.gitignore` & `flook-0.1.4/.gitignore`

 * *Files identical despite different names*

### Comparing `flook-0.1.3/CODE_OF_CONDUCT.md` & `flook-0.1.4/CODE_OF_CONDUCT.md`

 * *Files identical despite different names*

### Comparing `flook-0.1.3/CONTRIBUTING.rst` & `flook-0.1.4/CONTRIBUTING.rst`

 * *Files identical despite different names*

### Comparing `flook-0.1.3/LICENSE.txt` & `flook-0.1.4/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `flook-0.1.3/Makefile` & `flook-0.1.4/Makefile`

 * *Files identical despite different names*

### Comparing `flook-0.1.3/PKG-INFO` & `flook-0.1.4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: flook
-Version: 0.1.3
+Version: 0.1.4
 Summary: A Lightweight and Flexible Ansible Command Line Tool.
 Home-page: https://github.com/norwik/flook/
 Author: Clivern
 Author-email: hello@clivern.com
 License: MIT
 Project-URL: Documentation, https://github.com/norwik/flook/
 Project-URL: Source, https://github.com/norwik/flook/
```

### Comparing `flook-0.1.3/README.rst` & `flook-0.1.4/README.rst`

 * *Files identical despite different names*

### Comparing `flook-0.1.3/recipe/nginx/recipe.yml` & `flook-0.1.4/recipe/nginx/recipe.yml`

 * *Files identical despite different names*

### Comparing `flook-0.1.3/setup.cfg` & `flook-0.1.4/setup.cfg`

 * *Files identical despite different names*

### Comparing `flook-0.1.3/setup.py` & `flook-0.1.4/setup.py`

 * *Files identical despite different names*

### Comparing `flook-0.1.3/src/flook/__init__.py` & `flook-0.1.4/src/flook/__init__.py`

 * *Files identical despite different names*

### Comparing `flook-0.1.3/src/flook/cli.py` & `flook-0.1.4/src/flook/cli.py`

 * *Files 6% similar despite different names*

```diff
@@ -16,20 +16,22 @@
 # IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
 # FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
 # AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
 # LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
 # OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
 # SOFTWARE.
 
+import uuid
 import click
 import logging, json, sys
 from flook import __version__
 from flook.command.configs import Configs
 from flook.command.hosts import Hosts
 from flook.command.recipes import Recipes
+from flook.model.host import Host
 
 
 @click.group(help="🐺 A Lightweight and Flexible Ansible Command Line Tool")
 @click.version_option(version=__version__, help="Show the current version")
 def main():
     pass
 
@@ -58,20 +60,20 @@
     "--connection",
     "connection",
     type=click.STRING,
     default="ssh",
     help="Connection type to the host",
 )
 @click.option(
-    "-h",
-    "--host",
-    "host",
+    "-i",
+    "--ip",
+    "ip",
     type=click.STRING,
     default="",
-    help="The name of the host to connect to",
+    help="The IP or hostname to connect to",
 )
 @click.option(
     "-p",
     "--port",
     "port",
     type=click.INT,
     default=22,
@@ -98,32 +100,31 @@
     "--ssh_private_key_file",
     "ssh_private_key_file",
     type=click.File(),
     default="",
     help="Private key file used by ssh",
 )
 @click.option("-t", "--tags", "tags", type=click.STRING, default="", help="Host tags")
-def add(name, connection, host, port, user, password, ssh_private_key_file, tags):
-    return (
-        Hosts()
-        .init()
-        .add(
-            name,
-            {
-                "connection": connection,
-                "host": host,
-                "port": port,
-                "user": user,
-                "password": password,
-                "ssh_private_key_file": ssh_private_key_file,
-                "tags": tags.split(",") if "," in tags else [],
-            },
-        )
+def add(name, connection, ip, port, user, password, ssh_private_key_file, tags):
+    host = Host(
+        str(uuid.uuid4()),
+        name,
+        connection,
+        ip,
+        port,
+        user,
+        password,
+        ssh_private_key_file.read(),
+        tags.split(",") if "," in tags else [],
+        None,
+        None,
     )
 
+    return Hosts().init().add(host)
+
 
 # Get host sub command
 @host.command(help="Get a host")
 @click.argument("name")
 @click.option(
     "-o", "--output", "output", type=click.STRING, default="", help="Output format"
 )
@@ -187,14 +188,37 @@
 # Delete recipe sub command
 @recipe.command(help="Delete a recipe")
 @click.argument("name")
 def delete(name):
     return Recipes().init().delete(name)
 
 
+# Run recipe sub command
+@recipe.command(help="Run a recipe towards hosts")
+@click.argument("name")
+@click.option(
+    "-h",
+    "--host",
+    "host",
+    type=click.STRING,
+    default="",
+    help="The name of the host to run recipe towards",
+)
+@click.option(
+    "-t",
+    "--tag",
+    "tag",
+    type=click.STRING,
+    default="",
+    help="Hosts tag to run recipe towards",
+)
+def run(name, host, tag):
+    return Recipes().init().run(name, host, tag)
+
+
 # Manage configs command
 @click.group(help="Manage configs")
 def config():
     pass
 
 
 # Init configs sub command
```

### Comparing `flook-0.1.3/src/flook/command/__init__.py` & `flook-0.1.4/src/flook/command/__init__.py`

 * *Files identical despite different names*

### Comparing `flook-0.1.3/src/flook/command/configs.py` & `flook-0.1.4/src/flook/command/configs.py`

 * *Files identical despite different names*

### Comparing `flook-0.1.3/src/flook/command/hosts.py` & `flook-0.1.4/src/flook/command/hosts.py`

 * *Files 10% similar despite different names*

```diff
@@ -18,14 +18,15 @@
 # AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
 # LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
 # OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
 # SOFTWARE.
 
 import click
 
+from flook.model.host import Host
 from flook.module.logger import Logger
 from flook.module.database import Database
 from flook.module.output import Output
 from flook.module.config import Config
 
 
 class Hosts:
@@ -40,74 +41,76 @@
     def init(self):
         """Init database and configs"""
         self._configs = self.config.load()
         self.database.connect(self._configs["database"]["path"])
         self.database.migrate()
         return self
 
-    def add(self, name, configs):
+    def add(self, host):
         """Add a new host"""
-        configs["ssh_private_key_file"] = configs["ssh_private_key_file"].read()
+        if self.database.get_host(host.name) is not None:
+            raise click.ClickException(f"Host with name {host.name} exists")
 
-        if self.database.get_host(name) is not None:
-            raise click.ClickException(f"Host with name {name} exists")
+        self.database.insert_host(host)
 
-        self.database.insert_host(name, configs)
-        click.echo(f"Host with name {name} got created")
+        click.echo(f"Host with name {host.name} got created")
 
     def list(self, tag, output):
         """List hosts"""
         data = []
-        result = self.database.list_hosts()
+        hosts = self.database.list_hosts()
 
-        for item in result:
-            if tag != "" and tag not in item["config"]["tags"]:
+        for host in hosts:
+            if tag != "" and tag not in host.tags:
                 continue
 
             data.append(
                 {
-                    "Name": item["name"],
-                    "Host": item["config"]["host"],
-                    "Connection": item["config"]["connection"].upper(),
-                    "Tags": ", ".join(item["config"]["tags"])
-                    if len(item["config"]["tags"]) > 0
-                    else "-",
-                    "Created at": item["createdAt"],
+                    "ID": host.id,
+                    "Name": host.name,
+                    "IP": host.ip,
+                    "Connection": host.connection.upper(),
+                    "Tags": ", ".join(host.tags) if len(host.tags) > 0 else "-",
+                    "Created at": host.created_at,
+                    "Updated at": host.updated_at,
                 }
             )
 
         if len(data) == 0:
             raise click.ClickException(f"No hosts found!")
 
         print(
             self.output.render(
                 data, Output.JSON if output.lower() == "json" else Output.DEFAULT
             )
         )
 
     def get(self, name, output):
         """Get a host"""
-        result = self.database.get_host(name)
+        host = self.database.get_host(name)
 
-        if result is None:
+        if host is None:
             raise click.ClickException(f"Host with name {name} not found")
 
         data = [
             {
-                "Name": name,
-                "Host": result["host"],
-                "Connection": result["connection"].upper(),
-                "Tags": ", ".join(result["tags"]) if len(result["tags"]) > 0 else "-",
-                "Created at": result["createdAt"],
+                "ID": host.id,
+                "Name": host.name,
+                "IP": host.ip,
+                "Connection": host.connection.upper(),
+                "Tags": ", ".join(host.tags) if len(host.tags) > 0 else "-",
+                "Created at": host.created_at,
+                "Updated at": host.updated_at,
             }
         ]
 
         print(
             self.output.render(
                 data, Output.JSON if output.lower() == "json" else Output.DEFAULT
             )
         )
 
     def delete(self, name):
         """Delete a host"""
         self.database.delete_host(name)
+
         click.echo(f"Host with name {name} got deleted")
```

### Comparing `flook-0.1.3/src/flook/command/recipes.py` & `flook-0.1.4/src/flook/command/recipes.py`

 * *Files 8% similar despite different names*

```diff
@@ -16,17 +16,19 @@
 # IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
 # FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
 # AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
 # LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
 # OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
 # SOFTWARE.
 
+import uuid
 import click
 import yaml
 
+from flook.model.recipe import Recipe
 from flook.module.logger import Logger
 from flook.module.database import Database
 from flook.module.output import Output
 from flook.module.config import Config
 from flook.module.file_system import FileSystem
 
 
@@ -72,66 +74,78 @@
                         {
                             k: self.file_system.read_file(
                                 "{}/{}".format(configs["path"], v)
                             )
                         }
                     )
 
-        self.database.insert_recipe(
-            name, {"recipe": recipe, "templates": templates, "tags": configs["tags"]}
+        recipe = Recipe(
+            str(uuid.uuid4()), name, recipe, templates, configs["tags"], None, None
         )
 
+        self.database.insert_recipe(recipe)
+
         click.echo(f"Recipe with name {name} got created")
 
     def list(self, tag, output):
         """List Recipes"""
         data = []
-        result = self.database.list_recipes()
+        recipes = self.database.list_recipes()
 
-        for item in result:
-            if tag != "" and tag not in item["config"]["tags"]:
+        for recipe in recipes:
+            if tag != "" and tag not in recipe.tags:
                 continue
 
             data.append(
                 {
-                    "Name": item["name"],
-                    "Tags": ", ".join(item["config"]["tags"])
-                    if len(item["config"]["tags"]) > 0
-                    else "-",
-                    "Created at": item["createdAt"],
+                    "ID": recipe.id,
+                    "Name": recipe.name,
+                    "Tags": ", ".join(recipe.tags) if len(recipe.tags) > 0 else "-",
+                    "Created at": recipe.created_at,
+                    "Updated at": recipe.updated_at,
                 }
             )
 
         if len(data) == 0:
             raise click.ClickException(f"No recipes found!")
 
         print(
             self.output.render(
                 data, Output.JSON if output.lower() == "json" else Output.DEFAULT
             )
         )
 
     def get(self, name, output):
         """Get Recipe"""
-        result = self.database.get_recipe(name)
+        recipe = self.database.get_recipe(name)
 
-        if result is None:
-            raise click.ClickException(f"Recipe with name {name} not found")
+        if recipe is None:
+            raise click.ClickException(f"Recipe with name {recipe.name} not found")
 
         data = [
             {
-                "Name": name,
-                "Tags": ", ".join(result["tags"]) if len(result["tags"]) > 0 else "-",
-                "Created at": result["createdAt"],
+                "ID": recipe.id,
+                "Name": recipe.name,
+                "Tags": ", ".join(recipe.tags) if len(recipe.tags) > 0 else "-",
+                "Created at": recipe.created_at,
+                "Updated at": recipe.updated_at,
             }
         ]
 
         print(
             self.output.render(
                 data, Output.JSON if output.lower() == "json" else Output.DEFAULT
             )
         )
 
     def delete(self, name):
         """Delete a Recipe"""
         self.database.delete_recipe(name)
+
         click.echo(f"Recipe with name {name} got deleted")
+
+    def run(self, name, host, tag):
+        """Run a Recipe towards a host"""
+        # name is a recipe name
+        # host is the host name
+        # tag is the tag for hosts
+        pass
```

### Comparing `flook-0.1.3/src/flook/exception/__init__.py` & `flook-0.1.4/src/flook/exception/__init__.py`

 * *Files identical despite different names*

### Comparing `flook-0.1.3/src/flook/module/__init__.py` & `flook-0.1.4/src/flook/model/__init__.py`

 * *Files identical despite different names*

### Comparing `flook-0.1.3/src/flook/module/ansible.py` & `flook-0.1.4/src/flook/module/ansible.py`

 * *Files identical despite different names*

### Comparing `flook-0.1.3/src/flook/module/config.py` & `flook-0.1.4/src/flook/module/config.py`

 * *Files identical despite different names*

### Comparing `flook-0.1.3/src/flook/module/file_system.py` & `flook-0.1.4/src/flook/module/file_system.py`

 * *Files identical despite different names*

### Comparing `flook-0.1.3/src/flook/module/logger.py` & `flook-0.1.4/src/flook/module/logger.py`

 * *Files identical despite different names*

### Comparing `flook-0.1.3/src/flook/module/output.py` & `flook-0.1.4/src/flook/module/output.py`

 * *Files 15% similar despite different names*

```diff
@@ -17,14 +17,15 @@
 # FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
 # AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
 # LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
 # OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
 # SOFTWARE.
 
 import json
+from re import sub
 from prettytable import PrettyTable
 
 
 class Output:
     """Output Class"""
 
     JSON = "JSON"
@@ -43,15 +44,26 @@
         x.field_names = headers
         x.add_rows(rows)
 
         return x
 
     def _json(self, data):
         """Output data as JSON"""
-        return json.dumps(data)
+        new = []
+
+        for item in data:
+            new.append({self.camel_case(k): v for k, v in item.items()})
+
+        return json.dumps(new)
 
     def render(self, data, typ):
         """Render Data to the Console"""
         if typ == Output.JSON:
             return self._json(data)
 
         return self._table(data)
+
+    def camel_case(self, value):
+        """Change string into camel case"""
+        value = sub(r"(_|-)+", " ", value).title().replace(" ", "")
+
+        return ''.join([value[0].lower(), value[1:]])
```

### Comparing `flook-0.1.3/src/flook/module/playbook.py` & `flook-0.1.4/src/flook/module/__init__.py`

 * *Files 9% similar despite different names*

```diff
@@ -15,15 +15,7 @@
 # THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
 # IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
 # FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
 # AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
 # LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
 # OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
 # SOFTWARE.
-
-# @TODO this class should create a dir & create all the required
-# files for ansible to run against the host.
-class Playbook:
-    """Playbook Class"""
-
-    def __init__(self):
-        pass
```

### Comparing `flook-0.1.3/src/flook.egg-info/PKG-INFO` & `flook-0.1.4/src/flook.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: flook
-Version: 0.1.3
+Version: 0.1.4
 Summary: A Lightweight and Flexible Ansible Command Line Tool.
 Home-page: https://github.com/norwik/flook/
 Author: Clivern
 Author-email: hello@clivern.com
 License: MIT
 Project-URL: Documentation, https://github.com/norwik/flook/
 Project-URL: Source, https://github.com/norwik/flook/
```

### Comparing `flook-0.1.3/src/flook.egg-info/SOURCES.txt` & `flook-0.1.4/src/flook.egg-info/SOURCES.txt`

 * *Files 12% similar despite different names*

```diff
@@ -30,20 +30,22 @@
 src/flook.egg-info/requires.txt
 src/flook.egg-info/top_level.txt
 src/flook/command/__init__.py
 src/flook/command/configs.py
 src/flook/command/hosts.py
 src/flook/command/recipes.py
 src/flook/exception/__init__.py
+src/flook/model/__init__.py
+src/flook/model/host.py
+src/flook/model/recipe.py
+src/flook/model/task.py
 src/flook/module/__init__.py
 src/flook/module/ansible.py
 src/flook/module/config.py
 src/flook/module/database.py
 src/flook/module/file_system.py
 src/flook/module/logger.py
 src/flook/module/output.py
 src/flook/module/playbook.py
 tests/__init__.py
 tests/module/__init__.py
-tests/module/test_database.py
-tests/module/test_logger.py
-tests/module/test_output.py
+tests/module/test_logger.py
```

### Comparing `flook-0.1.3/tests/__init__.py` & `flook-0.1.4/tests/__init__.py`

 * *Files identical despite different names*

### Comparing `flook-0.1.3/tests/module/test_database.py` & `flook-0.1.4/src/flook/module/playbook.py`

 * *Files 26% similar despite different names*

```diff
@@ -16,23 +16,27 @@
 # IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
 # FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
 # AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
 # LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
 # OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
 # SOFTWARE.
 
-import pytest
-from flook.module.database import Database
 
+# @TODO this class should create a dir & create all the required
+# files for ansible to run against the host.
+class Playbook:
+    """Playbook Class"""
 
-def test_database():
-    """Database Tests"""
-    db = Database()
-    assert db.connect("cache/flook.db") == 0
-
-    db.migrate()
-    db.delete_host("c.com")
-
-    assert db.insert_host("c.com", {"ip": "127.0.0.1"}) == 1
-    assert db.get_host("c.com")["ip"] == "127.0.0.1"
-    assert db.get_host("f.com") == None
-    assert len(db.list_hosts()) == 1
+    def __init__(self):
+        pass
+
+    def set_cache_dir(self, cache_dir):
+        pass
+
+    def set_hosts(self, hosts):
+        pass
+
+    def set_recipe(self, recipe):
+        pass
+
+    def build(self):
+        pass
```

### Comparing `flook-0.1.3/tests/module/test_logger.py` & `flook-0.1.4/tests/module/test_logger.py`

 * *Files identical despite different names*

### Comparing `flook-0.1.3/tox.ini` & `flook-0.1.4/tox.ini`

 * *Files identical despite different names*

