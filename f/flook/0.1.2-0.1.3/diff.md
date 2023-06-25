# Comparing `tmp/flook-0.1.2.tar.gz` & `tmp/flook-0.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "flook-0.1.2.tar", last modified: Sun Jun 25 11:25:24 2023, max compression
+gzip compressed data, was "flook-0.1.3.tar", last modified: Sun Jun 25 11:40:42 2023, max compression
```

## Comparing `flook-0.1.2.tar` & `flook-0.1.3.tar`

### file list

```diff
@@ -1,65 +1,65 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-25 11:25:24.969176 flook-0.1.2/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-25 11:25:24.957176 flook-0.1.2/.github/
--rw-r--r--   0 runner    (1001) docker     (123)      120 2023-06-25 11:25:03.000000 flook-0.1.2/.github/CODEOWNERS
--rw-r--r--   0 runner    (1001) docker     (123)       47 2023-06-25 11:25:03.000000 flook-0.1.2/.github/FUNDING.yml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-25 11:25:24.957176 flook-0.1.2/.github/ISSUE_TEMPLATE/
--rw-r--r--   0 runner    (1001) docker     (123)      329 2023-06-25 11:25:03.000000 flook-0.1.2/.github/ISSUE_TEMPLATE/bug_report.md
--rw-r--r--   0 runner    (1001) docker     (123)      458 2023-06-25 11:25:03.000000 flook-0.1.2/.github/ISSUE_TEMPLATE/feature_request.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-25 11:25:24.957176 flook-0.1.2/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)      494 2023-06-25 11:25:03.000000 flook-0.1.2/.github/workflows/ci.yml
--rw-r--r--   0 runner    (1001) docker     (123)      573 2023-06-25 11:25:03.000000 flook-0.1.2/.github/workflows/release.yml
--rw-r--r--   0 runner    (1001) docker     (123)      564 2023-06-25 11:25:03.000000 flook-0.1.2/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)       68 2023-06-25 11:25:03.000000 flook-0.1.2/AUTHORS.rst
--rw-r--r--   0 runner    (1001) docker     (123)       79 2023-06-25 11:25:03.000000 flook-0.1.2/CHANGELOG.rst
--rw-r--r--   0 runner    (1001) docker     (123)     5219 2023-06-25 11:25:03.000000 flook-0.1.2/CODE_OF_CONDUCT.md
--rw-r--r--   0 runner    (1001) docker     (123)      742 2023-06-25 11:25:03.000000 flook-0.1.2/CONTRIBUTING.rst
--rw-r--r--   0 runner    (1001) docker     (123)     1074 2023-06-25 11:25:03.000000 flook-0.1.2/LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (123)      939 2023-06-25 11:25:03.000000 flook-0.1.2/Makefile
--rw-r--r--   0 runner    (1001) docker     (123)     1569 2023-06-25 11:25:24.969176 flook-0.1.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      792 2023-06-25 11:25:03.000000 flook-0.1.2/README.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-25 11:25:24.961176 flook-0.1.2/cache/
--rw-r--r--   0 runner    (1001) docker     (123)       13 2023-06-25 11:25:03.000000 flook-0.1.2/cache/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)      250 2023-06-25 11:25:03.000000 flook-0.1.2/pyproject.toml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-25 11:25:24.949175 flook-0.1.2/recipe/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-25 11:25:24.961176 flook-0.1.2/recipe/nginx/
--rw-r--r--   0 runner    (1001) docker     (123)      454 2023-06-25 11:25:03.000000 flook-0.1.2/recipe/nginx/motd.j2
--rw-r--r--   0 runner    (1001) docker     (123)      546 2023-06-25 11:25:03.000000 flook-0.1.2/recipe/nginx/recipe.yml
--rw-r--r--   0 runner    (1001) docker     (123)       41 2023-06-25 11:25:03.000000 flook-0.1.2/renovate.json
--rw-r--r--   0 runner    (1001) docker     (123)     1494 2023-06-25 11:25:24.969176 flook-0.1.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1553 2023-06-25 11:25:03.000000 flook-0.1.2/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-25 11:25:24.953175 flook-0.1.2/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-25 11:25:24.961176 flook-0.1.2/src/flook/
--rw-r--r--   0 runner    (1001) docker     (123)     1681 2023-06-25 11:25:03.000000 flook-0.1.2/src/flook/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5706 2023-06-25 11:25:03.000000 flook-0.1.2/src/flook/cli.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-25 11:25:24.965175 flook-0.1.2/src/flook/command/
--rw-r--r--   0 runner    (1001) docker     (123)     1102 2023-06-25 11:25:03.000000 flook-0.1.2/src/flook/command/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3150 2023-06-25 11:25:03.000000 flook-0.1.2/src/flook/command/configs.py
--rw-r--r--   0 runner    (1001) docker     (123)     3849 2023-06-25 11:25:03.000000 flook-0.1.2/src/flook/command/hosts.py
--rw-r--r--   0 runner    (1001) docker     (123)     4670 2023-06-25 11:25:03.000000 flook-0.1.2/src/flook/command/recipes.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-25 11:25:24.965175 flook-0.1.2/src/flook/exception/
--rw-r--r--   0 runner    (1001) docker     (123)     1102 2023-06-25 11:25:03.000000 flook-0.1.2/src/flook/exception/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-25 11:25:24.965175 flook-0.1.2/src/flook/module/
--rw-r--r--   0 runner    (1001) docker     (123)     1102 2023-06-25 11:25:03.000000 flook-0.1.2/src/flook/module/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2005 2023-06-25 11:25:03.000000 flook-0.1.2/src/flook/module/ansible.py
--rw-r--r--   0 runner    (1001) docker     (123)     1571 2023-06-25 11:25:03.000000 flook-0.1.2/src/flook/module/config.py
--rw-r--r--   0 runner    (1001) docker     (123)     4764 2023-06-25 11:25:03.000000 flook-0.1.2/src/flook/module/database.py
--rw-r--r--   0 runner    (1001) docker     (123)     3440 2023-06-25 11:25:03.000000 flook-0.1.2/src/flook/module/file_system.py
--rw-r--r--   0 runner    (1001) docker     (123)     1548 2023-06-25 11:25:03.000000 flook-0.1.2/src/flook/module/logger.py
--rw-r--r--   0 runner    (1001) docker     (123)     1808 2023-06-25 11:25:03.000000 flook-0.1.2/src/flook/module/output.py
--rw-r--r--   0 runner    (1001) docker     (123)     1292 2023-06-25 11:25:03.000000 flook-0.1.2/src/flook/module/playbook.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-25 11:25:24.961176 flook-0.1.2/src/flook.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1569 2023-06-25 11:25:24.000000 flook-0.1.2/src/flook.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1170 2023-06-25 11:25:24.000000 flook-0.1.2/src/flook.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-25 11:25:24.000000 flook-0.1.2/src/flook.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       41 2023-06-25 11:25:24.000000 flook-0.1.2/src/flook.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-25 11:25:24.000000 flook-0.1.2/src/flook.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)      126 2023-06-25 11:25:24.000000 flook-0.1.2/src/flook.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        6 2023-06-25 11:25:24.000000 flook-0.1.2/src/flook.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-25 11:25:24.965175 flook-0.1.2/tests/
--rw-r--r--   0 runner    (1001) docker     (123)     1102 2023-06-25 11:25:03.000000 flook-0.1.2/tests/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-25 11:25:24.969176 flook-0.1.2/tests/module/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-25 11:25:03.000000 flook-0.1.2/tests/module/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1511 2023-06-25 11:25:03.000000 flook-0.1.2/tests/module/test_database.py
--rw-r--r--   0 runner    (1001) docker     (123)     1325 2023-06-25 11:25:03.000000 flook-0.1.2/tests/module/test_logger.py
--rw-r--r--   0 runner    (1001) docker     (123)     1501 2023-06-25 11:25:03.000000 flook-0.1.2/tests/module/test_output.py
--rw-r--r--   0 runner    (1001) docker     (123)      719 2023-06-25 11:25:03.000000 flook-0.1.2/tox.ini
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-25 11:40:42.983288 flook-0.1.3/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-25 11:40:42.979288 flook-0.1.3/.github/
+-rw-r--r--   0 runner    (1001) docker     (123)      120 2023-06-25 11:40:20.000000 flook-0.1.3/.github/CODEOWNERS
+-rw-r--r--   0 runner    (1001) docker     (123)       47 2023-06-25 11:40:20.000000 flook-0.1.3/.github/FUNDING.yml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-25 11:40:42.979288 flook-0.1.3/.github/ISSUE_TEMPLATE/
+-rw-r--r--   0 runner    (1001) docker     (123)      329 2023-06-25 11:40:20.000000 flook-0.1.3/.github/ISSUE_TEMPLATE/bug_report.md
+-rw-r--r--   0 runner    (1001) docker     (123)      458 2023-06-25 11:40:20.000000 flook-0.1.3/.github/ISSUE_TEMPLATE/feature_request.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-25 11:40:42.979288 flook-0.1.3/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)      494 2023-06-25 11:40:20.000000 flook-0.1.3/.github/workflows/ci.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      573 2023-06-25 11:40:20.000000 flook-0.1.3/.github/workflows/release.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      564 2023-06-25 11:40:20.000000 flook-0.1.3/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)       68 2023-06-25 11:40:20.000000 flook-0.1.3/AUTHORS.rst
+-rw-r--r--   0 runner    (1001) docker     (123)       79 2023-06-25 11:40:20.000000 flook-0.1.3/CHANGELOG.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     5219 2023-06-25 11:40:20.000000 flook-0.1.3/CODE_OF_CONDUCT.md
+-rw-r--r--   0 runner    (1001) docker     (123)      742 2023-06-25 11:40:20.000000 flook-0.1.3/CONTRIBUTING.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1074 2023-06-25 11:40:20.000000 flook-0.1.3/LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      939 2023-06-25 11:40:20.000000 flook-0.1.3/Makefile
+-rw-r--r--   0 runner    (1001) docker     (123)     1569 2023-06-25 11:40:42.983288 flook-0.1.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      792 2023-06-25 11:40:20.000000 flook-0.1.3/README.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-25 11:40:42.979288 flook-0.1.3/cache/
+-rw-r--r--   0 runner    (1001) docker     (123)       13 2023-06-25 11:40:20.000000 flook-0.1.3/cache/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)      250 2023-06-25 11:40:20.000000 flook-0.1.3/pyproject.toml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-25 11:40:42.979288 flook-0.1.3/recipe/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-25 11:40:42.979288 flook-0.1.3/recipe/nginx/
+-rw-r--r--   0 runner    (1001) docker     (123)      454 2023-06-25 11:40:20.000000 flook-0.1.3/recipe/nginx/motd.j2
+-rw-r--r--   0 runner    (1001) docker     (123)      546 2023-06-25 11:40:20.000000 flook-0.1.3/recipe/nginx/recipe.yml
+-rw-r--r--   0 runner    (1001) docker     (123)       41 2023-06-25 11:40:20.000000 flook-0.1.3/renovate.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1494 2023-06-25 11:40:42.983288 flook-0.1.3/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1553 2023-06-25 11:40:20.000000 flook-0.1.3/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-25 11:40:42.979288 flook-0.1.3/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-25 11:40:42.979288 flook-0.1.3/src/flook/
+-rw-r--r--   0 runner    (1001) docker     (123)     1681 2023-06-25 11:40:20.000000 flook-0.1.3/src/flook/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5669 2023-06-25 11:40:20.000000 flook-0.1.3/src/flook/cli.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-25 11:40:42.983288 flook-0.1.3/src/flook/command/
+-rw-r--r--   0 runner    (1001) docker     (123)     1102 2023-06-25 11:40:20.000000 flook-0.1.3/src/flook/command/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3150 2023-06-25 11:40:20.000000 flook-0.1.3/src/flook/command/configs.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3849 2023-06-25 11:40:20.000000 flook-0.1.3/src/flook/command/hosts.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4670 2023-06-25 11:40:20.000000 flook-0.1.3/src/flook/command/recipes.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-25 11:40:42.983288 flook-0.1.3/src/flook/exception/
+-rw-r--r--   0 runner    (1001) docker     (123)     1102 2023-06-25 11:40:20.000000 flook-0.1.3/src/flook/exception/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-25 11:40:42.983288 flook-0.1.3/src/flook/module/
+-rw-r--r--   0 runner    (1001) docker     (123)     1102 2023-06-25 11:40:20.000000 flook-0.1.3/src/flook/module/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2005 2023-06-25 11:40:20.000000 flook-0.1.3/src/flook/module/ansible.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1571 2023-06-25 11:40:20.000000 flook-0.1.3/src/flook/module/config.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4764 2023-06-25 11:40:20.000000 flook-0.1.3/src/flook/module/database.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3440 2023-06-25 11:40:20.000000 flook-0.1.3/src/flook/module/file_system.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1548 2023-06-25 11:40:20.000000 flook-0.1.3/src/flook/module/logger.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1808 2023-06-25 11:40:20.000000 flook-0.1.3/src/flook/module/output.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1292 2023-06-25 11:40:20.000000 flook-0.1.3/src/flook/module/playbook.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-25 11:40:42.983288 flook-0.1.3/src/flook.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1569 2023-06-25 11:40:42.000000 flook-0.1.3/src/flook.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1170 2023-06-25 11:40:42.000000 flook-0.1.3/src/flook.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-25 11:40:42.000000 flook-0.1.3/src/flook.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       41 2023-06-25 11:40:42.000000 flook-0.1.3/src/flook.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-25 11:40:42.000000 flook-0.1.3/src/flook.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)      126 2023-06-25 11:40:42.000000 flook-0.1.3/src/flook.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        6 2023-06-25 11:40:42.000000 flook-0.1.3/src/flook.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-25 11:40:42.983288 flook-0.1.3/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     1102 2023-06-25 11:40:20.000000 flook-0.1.3/tests/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-25 11:40:42.983288 flook-0.1.3/tests/module/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-25 11:40:20.000000 flook-0.1.3/tests/module/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1511 2023-06-25 11:40:20.000000 flook-0.1.3/tests/module/test_database.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1325 2023-06-25 11:40:20.000000 flook-0.1.3/tests/module/test_logger.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1501 2023-06-25 11:40:20.000000 flook-0.1.3/tests/module/test_output.py
+-rw-r--r--   0 runner    (1001) docker     (123)      719 2023-06-25 11:40:20.000000 flook-0.1.3/tox.ini
```

### Comparing `flook-0.1.2/.github/workflows/release.yml` & `flook-0.1.3/.github/workflows/release.yml`

 * *Files identical despite different names*

### Comparing `flook-0.1.2/.gitignore` & `flook-0.1.3/.gitignore`

 * *Files identical despite different names*

### Comparing `flook-0.1.2/CODE_OF_CONDUCT.md` & `flook-0.1.3/CODE_OF_CONDUCT.md`

 * *Files identical despite different names*

### Comparing `flook-0.1.2/CONTRIBUTING.rst` & `flook-0.1.3/CONTRIBUTING.rst`

 * *Files identical despite different names*

### Comparing `flook-0.1.2/LICENSE.txt` & `flook-0.1.3/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `flook-0.1.2/Makefile` & `flook-0.1.3/Makefile`

 * *Files identical despite different names*

### Comparing `flook-0.1.2/PKG-INFO` & `flook-0.1.3/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: flook
-Version: 0.1.2
+Version: 0.1.3
 Summary: A Lightweight and Flexible Ansible Command Line Tool.
 Home-page: https://github.com/norwik/flook/
 Author: Clivern
 Author-email: hello@clivern.com
 License: MIT
 Project-URL: Documentation, https://github.com/norwik/flook/
 Project-URL: Source, https://github.com/norwik/flook/
```

### Comparing `flook-0.1.2/README.rst` & `flook-0.1.3/README.rst`

 * *Files identical despite different names*

### Comparing `flook-0.1.2/recipe/nginx/recipe.yml` & `flook-0.1.3/recipe/nginx/recipe.yml`

 * *Files identical despite different names*

### Comparing `flook-0.1.2/setup.cfg` & `flook-0.1.3/setup.cfg`

 * *Files identical despite different names*

### Comparing `flook-0.1.2/setup.py` & `flook-0.1.3/setup.py`

 * *Files identical despite different names*

### Comparing `flook-0.1.2/src/flook/__init__.py` & `flook-0.1.3/src/flook/__init__.py`

 * *Files identical despite different names*

### Comparing `flook-0.1.2/src/flook/cli.py` & `flook-0.1.3/src/flook/cli.py`

 * *Files 2% similar despite different names*

```diff
@@ -22,15 +22,14 @@
 
 import click
 import logging, json, sys
 from flook import __version__
 from flook.command.configs import Configs
 from flook.command.hosts import Hosts
 from flook.command.recipes import Recipes
-from flook.module.table import Table
 
 
 @click.group(help="🐺 A Lightweight and Flexible Ansible Command Line Tool")
 @click.version_option(version=__version__, help="Show the current version")
 def main():
     pass
```

### Comparing `flook-0.1.2/src/flook/command/__init__.py` & `flook-0.1.3/src/flook/command/__init__.py`

 * *Files identical despite different names*

### Comparing `flook-0.1.2/src/flook/command/configs.py` & `flook-0.1.3/src/flook/command/configs.py`

 * *Files identical despite different names*

### Comparing `flook-0.1.2/src/flook/command/hosts.py` & `flook-0.1.3/src/flook/command/hosts.py`

 * *Files identical despite different names*

### Comparing `flook-0.1.2/src/flook/command/recipes.py` & `flook-0.1.3/src/flook/command/recipes.py`

 * *Files identical despite different names*

### Comparing `flook-0.1.2/src/flook/exception/__init__.py` & `flook-0.1.3/src/flook/exception/__init__.py`

 * *Files identical despite different names*

### Comparing `flook-0.1.2/src/flook/module/__init__.py` & `flook-0.1.3/src/flook/module/__init__.py`

 * *Files identical despite different names*

### Comparing `flook-0.1.2/src/flook/module/ansible.py` & `flook-0.1.3/src/flook/module/ansible.py`

 * *Files identical despite different names*

### Comparing `flook-0.1.2/src/flook/module/config.py` & `flook-0.1.3/src/flook/module/config.py`

 * *Files identical despite different names*

### Comparing `flook-0.1.2/src/flook/module/database.py` & `flook-0.1.3/src/flook/module/database.py`

 * *Files identical despite different names*

### Comparing `flook-0.1.2/src/flook/module/file_system.py` & `flook-0.1.3/src/flook/module/file_system.py`

 * *Files identical despite different names*

### Comparing `flook-0.1.2/src/flook/module/logger.py` & `flook-0.1.3/src/flook/module/logger.py`

 * *Files identical despite different names*

### Comparing `flook-0.1.2/src/flook/module/output.py` & `flook-0.1.3/src/flook/module/output.py`

 * *Files identical despite different names*

### Comparing `flook-0.1.2/src/flook/module/playbook.py` & `flook-0.1.3/src/flook/module/playbook.py`

 * *Files identical despite different names*

### Comparing `flook-0.1.2/src/flook.egg-info/PKG-INFO` & `flook-0.1.3/src/flook.egg-info/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: flook
-Version: 0.1.2
+Version: 0.1.3
 Summary: A Lightweight and Flexible Ansible Command Line Tool.
 Home-page: https://github.com/norwik/flook/
 Author: Clivern
 Author-email: hello@clivern.com
 License: MIT
 Project-URL: Documentation, https://github.com/norwik/flook/
 Project-URL: Source, https://github.com/norwik/flook/
```

### Comparing `flook-0.1.2/src/flook.egg-info/SOURCES.txt` & `flook-0.1.3/src/flook.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `flook-0.1.2/tests/__init__.py` & `flook-0.1.3/tests/__init__.py`

 * *Files identical despite different names*

### Comparing `flook-0.1.2/tests/module/test_database.py` & `flook-0.1.3/tests/module/test_database.py`

 * *Files identical despite different names*

### Comparing `flook-0.1.2/tests/module/test_logger.py` & `flook-0.1.3/tests/module/test_logger.py`

 * *Files identical despite different names*

### Comparing `flook-0.1.2/tests/module/test_output.py` & `flook-0.1.3/tests/module/test_output.py`

 * *Files identical despite different names*

### Comparing `flook-0.1.2/tox.ini` & `flook-0.1.3/tox.ini`

 * *Files identical despite different names*

