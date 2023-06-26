# Comparing `tmp/flook-0.1.4.tar.gz` & `tmp/flook-0.1.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "flook-0.1.4.tar", last modified: Sun Jun 25 23:59:01 2023, max compression
+gzip compressed data, was "flook-0.1.5.tar", last modified: Mon Jun 26 00:43:09 2023, max compression
```

## Comparing `flook-0.1.4.tar` & `flook-0.1.5.tar`

### file list

```diff
@@ -1,68 +1,68 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-25 23:59:01.437313 flook-0.1.4/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-25 23:59:01.433313 flook-0.1.4/.github/
--rw-r--r--   0 runner    (1001) docker     (123)      120 2023-06-25 23:58:41.000000 flook-0.1.4/.github/CODEOWNERS
--rw-r--r--   0 runner    (1001) docker     (123)       47 2023-06-25 23:58:41.000000 flook-0.1.4/.github/FUNDING.yml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-25 23:59:01.433313 flook-0.1.4/.github/ISSUE_TEMPLATE/
--rw-r--r--   0 runner    (1001) docker     (123)      329 2023-06-25 23:58:41.000000 flook-0.1.4/.github/ISSUE_TEMPLATE/bug_report.md
--rw-r--r--   0 runner    (1001) docker     (123)      458 2023-06-25 23:58:41.000000 flook-0.1.4/.github/ISSUE_TEMPLATE/feature_request.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-25 23:59:01.433313 flook-0.1.4/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)      494 2023-06-25 23:58:41.000000 flook-0.1.4/.github/workflows/ci.yml
--rw-r--r--   0 runner    (1001) docker     (123)      573 2023-06-25 23:58:41.000000 flook-0.1.4/.github/workflows/release.yml
--rw-r--r--   0 runner    (1001) docker     (123)      564 2023-06-25 23:58:41.000000 flook-0.1.4/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)       68 2023-06-25 23:58:41.000000 flook-0.1.4/AUTHORS.rst
--rw-r--r--   0 runner    (1001) docker     (123)       79 2023-06-25 23:58:41.000000 flook-0.1.4/CHANGELOG.rst
--rw-r--r--   0 runner    (1001) docker     (123)     5219 2023-06-25 23:58:41.000000 flook-0.1.4/CODE_OF_CONDUCT.md
--rw-r--r--   0 runner    (1001) docker     (123)      742 2023-06-25 23:58:41.000000 flook-0.1.4/CONTRIBUTING.rst
--rw-r--r--   0 runner    (1001) docker     (123)     1074 2023-06-25 23:58:41.000000 flook-0.1.4/LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (123)      939 2023-06-25 23:58:41.000000 flook-0.1.4/Makefile
--rw-r--r--   0 runner    (1001) docker     (123)     1569 2023-06-25 23:59:01.437313 flook-0.1.4/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      792 2023-06-25 23:58:41.000000 flook-0.1.4/README.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-25 23:59:01.433313 flook-0.1.4/cache/
--rw-r--r--   0 runner    (1001) docker     (123)       13 2023-06-25 23:58:41.000000 flook-0.1.4/cache/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)      250 2023-06-25 23:58:41.000000 flook-0.1.4/pyproject.toml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-25 23:59:01.429313 flook-0.1.4/recipe/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-25 23:59:01.433313 flook-0.1.4/recipe/nginx/
--rw-r--r--   0 runner    (1001) docker     (123)      454 2023-06-25 23:58:41.000000 flook-0.1.4/recipe/nginx/motd.j2
--rw-r--r--   0 runner    (1001) docker     (123)      546 2023-06-25 23:58:41.000000 flook-0.1.4/recipe/nginx/recipe.yml
--rw-r--r--   0 runner    (1001) docker     (123)       41 2023-06-25 23:58:41.000000 flook-0.1.4/renovate.json
--rw-r--r--   0 runner    (1001) docker     (123)     1494 2023-06-25 23:59:01.437313 flook-0.1.4/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1553 2023-06-25 23:58:41.000000 flook-0.1.4/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-25 23:59:01.429313 flook-0.1.4/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-25 23:59:01.433313 flook-0.1.4/src/flook/
--rw-r--r--   0 runner    (1001) docker     (123)     1681 2023-06-25 23:58:41.000000 flook-0.1.4/src/flook/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6039 2023-06-25 23:58:41.000000 flook-0.1.4/src/flook/cli.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-25 23:59:01.433313 flook-0.1.4/src/flook/command/
--rw-r--r--   0 runner    (1001) docker     (123)     1102 2023-06-25 23:58:41.000000 flook-0.1.4/src/flook/command/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3150 2023-06-25 23:58:41.000000 flook-0.1.4/src/flook/command/configs.py
--rw-r--r--   0 runner    (1001) docker     (123)     3821 2023-06-25 23:58:41.000000 flook-0.1.4/src/flook/command/hosts.py
--rw-r--r--   0 runner    (1001) docker     (123)     5051 2023-06-25 23:58:41.000000 flook-0.1.4/src/flook/command/recipes.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-25 23:59:01.433313 flook-0.1.4/src/flook/exception/
--rw-r--r--   0 runner    (1001) docker     (123)     1102 2023-06-25 23:58:41.000000 flook-0.1.4/src/flook/exception/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-25 23:59:01.433313 flook-0.1.4/src/flook/model/
--rw-r--r--   0 runner    (1001) docker     (123)     1102 2023-06-25 23:58:41.000000 flook-0.1.4/src/flook/model/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2750 2023-06-25 23:58:41.000000 flook-0.1.4/src/flook/model/host.py
--rw-r--r--   0 runner    (1001) docker     (123)     2131 2023-06-25 23:58:41.000000 flook-0.1.4/src/flook/model/recipe.py
--rw-r--r--   0 runner    (1001) docker     (123)     1986 2023-06-25 23:58:41.000000 flook-0.1.4/src/flook/model/task.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-25 23:59:01.437313 flook-0.1.4/src/flook/module/
--rw-r--r--   0 runner    (1001) docker     (123)     1102 2023-06-25 23:58:41.000000 flook-0.1.4/src/flook/module/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2005 2023-06-25 23:58:41.000000 flook-0.1.4/src/flook/module/ansible.py
--rw-r--r--   0 runner    (1001) docker     (123)     1571 2023-06-25 23:58:41.000000 flook-0.1.4/src/flook/module/config.py
--rw-r--r--   0 runner    (1001) docker     (123)     7049 2023-06-25 23:58:41.000000 flook-0.1.4/src/flook/module/database.py
--rw-r--r--   0 runner    (1001) docker     (123)     3440 2023-06-25 23:58:41.000000 flook-0.1.4/src/flook/module/file_system.py
--rw-r--r--   0 runner    (1001) docker     (123)     1548 2023-06-25 23:58:41.000000 flook-0.1.4/src/flook/module/logger.py
--rw-r--r--   0 runner    (1001) docker     (123)     2145 2023-06-25 23:58:41.000000 flook-0.1.4/src/flook/module/output.py
--rw-r--r--   0 runner    (1001) docker     (123)     1476 2023-06-25 23:58:41.000000 flook-0.1.4/src/flook/module/playbook.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-25 23:59:01.433313 flook-0.1.4/src/flook.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1569 2023-06-25 23:59:01.000000 flook-0.1.4/src/flook.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1214 2023-06-25 23:59:01.000000 flook-0.1.4/src/flook.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-25 23:59:01.000000 flook-0.1.4/src/flook.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       41 2023-06-25 23:59:01.000000 flook-0.1.4/src/flook.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-25 23:59:01.000000 flook-0.1.4/src/flook.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)      126 2023-06-25 23:59:01.000000 flook-0.1.4/src/flook.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        6 2023-06-25 23:59:01.000000 flook-0.1.4/src/flook.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-25 23:59:01.437313 flook-0.1.4/tests/
--rw-r--r--   0 runner    (1001) docker     (123)     1102 2023-06-25 23:58:41.000000 flook-0.1.4/tests/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-25 23:59:01.437313 flook-0.1.4/tests/module/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-25 23:58:41.000000 flook-0.1.4/tests/module/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1325 2023-06-25 23:58:41.000000 flook-0.1.4/tests/module/test_logger.py
--rw-r--r--   0 runner    (1001) docker     (123)      719 2023-06-25 23:58:41.000000 flook-0.1.4/tox.ini
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 00:43:09.628960 flook-0.1.5/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 00:43:09.624959 flook-0.1.5/.github/
+-rw-r--r--   0 runner    (1001) docker     (123)      120 2023-06-26 00:42:41.000000 flook-0.1.5/.github/CODEOWNERS
+-rw-r--r--   0 runner    (1001) docker     (123)       47 2023-06-26 00:42:41.000000 flook-0.1.5/.github/FUNDING.yml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 00:43:09.624959 flook-0.1.5/.github/ISSUE_TEMPLATE/
+-rw-r--r--   0 runner    (1001) docker     (123)      329 2023-06-26 00:42:41.000000 flook-0.1.5/.github/ISSUE_TEMPLATE/bug_report.md
+-rw-r--r--   0 runner    (1001) docker     (123)      458 2023-06-26 00:42:41.000000 flook-0.1.5/.github/ISSUE_TEMPLATE/feature_request.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 00:43:09.624959 flook-0.1.5/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)      494 2023-06-26 00:42:41.000000 flook-0.1.5/.github/workflows/ci.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      573 2023-06-26 00:42:41.000000 flook-0.1.5/.github/workflows/release.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      564 2023-06-26 00:42:41.000000 flook-0.1.5/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)       68 2023-06-26 00:42:41.000000 flook-0.1.5/AUTHORS.rst
+-rw-r--r--   0 runner    (1001) docker     (123)       79 2023-06-26 00:42:41.000000 flook-0.1.5/CHANGELOG.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     5219 2023-06-26 00:42:41.000000 flook-0.1.5/CODE_OF_CONDUCT.md
+-rw-r--r--   0 runner    (1001) docker     (123)      742 2023-06-26 00:42:41.000000 flook-0.1.5/CONTRIBUTING.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1074 2023-06-26 00:42:41.000000 flook-0.1.5/LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      939 2023-06-26 00:42:41.000000 flook-0.1.5/Makefile
+-rw-r--r--   0 runner    (1001) docker     (123)     1569 2023-06-26 00:43:09.628960 flook-0.1.5/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      792 2023-06-26 00:42:41.000000 flook-0.1.5/README.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 00:43:09.624959 flook-0.1.5/cache/
+-rw-r--r--   0 runner    (1001) docker     (123)       13 2023-06-26 00:42:41.000000 flook-0.1.5/cache/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)      250 2023-06-26 00:42:41.000000 flook-0.1.5/pyproject.toml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 00:43:09.620959 flook-0.1.5/recipe/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 00:43:09.624959 flook-0.1.5/recipe/nginx/
+-rw-r--r--   0 runner    (1001) docker     (123)      454 2023-06-26 00:42:41.000000 flook-0.1.5/recipe/nginx/motd.j2
+-rw-r--r--   0 runner    (1001) docker     (123)      546 2023-06-26 00:42:41.000000 flook-0.1.5/recipe/nginx/recipe.yml
+-rw-r--r--   0 runner    (1001) docker     (123)       41 2023-06-26 00:42:41.000000 flook-0.1.5/renovate.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1494 2023-06-26 00:43:09.628960 flook-0.1.5/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1553 2023-06-26 00:42:41.000000 flook-0.1.5/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 00:43:09.620959 flook-0.1.5/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 00:43:09.624959 flook-0.1.5/src/flook/
+-rw-r--r--   0 runner    (1001) docker     (123)     1681 2023-06-26 00:42:41.000000 flook-0.1.5/src/flook/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6039 2023-06-26 00:42:41.000000 flook-0.1.5/src/flook/cli.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 00:43:09.628960 flook-0.1.5/src/flook/command/
+-rw-r--r--   0 runner    (1001) docker     (123)     1102 2023-06-26 00:42:41.000000 flook-0.1.5/src/flook/command/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3150 2023-06-26 00:42:41.000000 flook-0.1.5/src/flook/command/configs.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3821 2023-06-26 00:42:41.000000 flook-0.1.5/src/flook/command/hosts.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5754 2023-06-26 00:42:41.000000 flook-0.1.5/src/flook/command/recipes.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 00:43:09.628960 flook-0.1.5/src/flook/exception/
+-rw-r--r--   0 runner    (1001) docker     (123)     1102 2023-06-26 00:42:41.000000 flook-0.1.5/src/flook/exception/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 00:43:09.628960 flook-0.1.5/src/flook/model/
+-rw-r--r--   0 runner    (1001) docker     (123)     1102 2023-06-26 00:42:41.000000 flook-0.1.5/src/flook/model/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2750 2023-06-26 00:42:41.000000 flook-0.1.5/src/flook/model/host.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2131 2023-06-26 00:42:41.000000 flook-0.1.5/src/flook/model/recipe.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1986 2023-06-26 00:42:41.000000 flook-0.1.5/src/flook/model/task.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 00:43:09.628960 flook-0.1.5/src/flook/module/
+-rw-r--r--   0 runner    (1001) docker     (123)     1102 2023-06-26 00:42:41.000000 flook-0.1.5/src/flook/module/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2005 2023-06-26 00:42:41.000000 flook-0.1.5/src/flook/module/ansible.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1571 2023-06-26 00:42:41.000000 flook-0.1.5/src/flook/module/config.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7049 2023-06-26 00:42:41.000000 flook-0.1.5/src/flook/module/database.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3440 2023-06-26 00:42:41.000000 flook-0.1.5/src/flook/module/file_system.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1548 2023-06-26 00:42:41.000000 flook-0.1.5/src/flook/module/logger.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2145 2023-06-26 00:42:41.000000 flook-0.1.5/src/flook/module/output.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1476 2023-06-26 00:42:41.000000 flook-0.1.5/src/flook/module/playbook.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 00:43:09.624959 flook-0.1.5/src/flook.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1569 2023-06-26 00:43:09.000000 flook-0.1.5/src/flook.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1214 2023-06-26 00:43:09.000000 flook-0.1.5/src/flook.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-26 00:43:09.000000 flook-0.1.5/src/flook.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       41 2023-06-26 00:43:09.000000 flook-0.1.5/src/flook.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-26 00:43:09.000000 flook-0.1.5/src/flook.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)      126 2023-06-26 00:43:09.000000 flook-0.1.5/src/flook.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        6 2023-06-26 00:43:09.000000 flook-0.1.5/src/flook.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 00:43:09.628960 flook-0.1.5/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     1102 2023-06-26 00:42:41.000000 flook-0.1.5/tests/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 00:43:09.628960 flook-0.1.5/tests/module/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-26 00:42:41.000000 flook-0.1.5/tests/module/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1325 2023-06-26 00:42:41.000000 flook-0.1.5/tests/module/test_logger.py
+-rw-r--r--   0 runner    (1001) docker     (123)      719 2023-06-26 00:42:41.000000 flook-0.1.5/tox.ini
```

### Comparing `flook-0.1.4/.github/workflows/release.yml` & `flook-0.1.5/.github/workflows/release.yml`

 * *Files identical despite different names*

### Comparing `flook-0.1.4/.gitignore` & `flook-0.1.5/.gitignore`

 * *Files identical despite different names*

### Comparing `flook-0.1.4/CODE_OF_CONDUCT.md` & `flook-0.1.5/CODE_OF_CONDUCT.md`

 * *Files identical despite different names*

### Comparing `flook-0.1.4/CONTRIBUTING.rst` & `flook-0.1.5/CONTRIBUTING.rst`

 * *Files identical despite different names*

### Comparing `flook-0.1.4/LICENSE.txt` & `flook-0.1.5/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `flook-0.1.4/Makefile` & `flook-0.1.5/Makefile`

 * *Files identical despite different names*

### Comparing `flook-0.1.4/PKG-INFO` & `flook-0.1.5/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: flook
-Version: 0.1.4
+Version: 0.1.5
 Summary: A Lightweight and Flexible Ansible Command Line Tool.
 Home-page: https://github.com/norwik/flook/
 Author: Clivern
 Author-email: hello@clivern.com
 License: MIT
 Project-URL: Documentation, https://github.com/norwik/flook/
 Project-URL: Source, https://github.com/norwik/flook/
```

### Comparing `flook-0.1.4/README.rst` & `flook-0.1.5/README.rst`

 * *Files identical despite different names*

### Comparing `flook-0.1.4/recipe/nginx/recipe.yml` & `flook-0.1.5/recipe/nginx/recipe.yml`

 * *Files identical despite different names*

### Comparing `flook-0.1.4/setup.cfg` & `flook-0.1.5/setup.cfg`

 * *Files identical despite different names*

### Comparing `flook-0.1.4/setup.py` & `flook-0.1.5/setup.py`

 * *Files identical despite different names*

### Comparing `flook-0.1.4/src/flook/__init__.py` & `flook-0.1.5/src/flook/__init__.py`

 * *Files identical despite different names*

### Comparing `flook-0.1.4/src/flook/cli.py` & `flook-0.1.5/src/flook/cli.py`

 * *Files identical despite different names*

### Comparing `flook-0.1.4/src/flook/command/__init__.py` & `flook-0.1.5/src/flook/command/__init__.py`

 * *Files identical despite different names*

### Comparing `flook-0.1.4/src/flook/command/configs.py` & `flook-0.1.5/src/flook/command/configs.py`

 * *Files identical despite different names*

### Comparing `flook-0.1.4/src/flook/command/hosts.py` & `flook-0.1.5/src/flook/command/hosts.py`

 * *Files identical despite different names*

### Comparing `flook-0.1.4/src/flook/command/recipes.py` & `flook-0.1.5/src/flook/command/recipes.py`

 * *Files 15% similar despite different names*

```diff
@@ -139,13 +139,37 @@
 
     def delete(self, name):
         """Delete a Recipe"""
         self.database.delete_recipe(name)
 
         click.echo(f"Recipe with name {name} got deleted")
 
-    def run(self, name, host, tag):
+    def run(self, name, host_name, tag):
         """Run a Recipe towards a host"""
-        # name is a recipe name
-        # host is the host name
-        # tag is the tag for hosts
-        pass
+        hosts = []
+        found = ""
+        recipe = self.database.get_recipe(name)
+
+        if recipe is None:
+            raise click.ClickException(f"Recipe with name {recipe.name} not found")
+
+        if host_name != "":
+            host = self.database.get_host(host_name)
+
+            if host is None:
+                raise click.ClickException(f"Host with name {name} not found")
+
+            found = host.id
+            hosts.append(host)
+
+        if tag != "":
+            items = self.database.list_hosts()
+            for item in items:
+                if tag not in item.tags or found == item.id:
+                    continue
+                hosts.append(item)
+
+        if len(hosts) == 0:
+            raise click.ClickException(f"No hosts matching!")
+
+        print(hosts)
+        print(recipe)
```

### Comparing `flook-0.1.4/src/flook/exception/__init__.py` & `flook-0.1.5/src/flook/exception/__init__.py`

 * *Files identical despite different names*

### Comparing `flook-0.1.4/src/flook/model/__init__.py` & `flook-0.1.5/src/flook/model/__init__.py`

 * *Files identical despite different names*

### Comparing `flook-0.1.4/src/flook/model/host.py` & `flook-0.1.5/src/flook/model/host.py`

 * *Files identical despite different names*

### Comparing `flook-0.1.4/src/flook/model/recipe.py` & `flook-0.1.5/src/flook/model/recipe.py`

 * *Files identical despite different names*

### Comparing `flook-0.1.4/src/flook/model/task.py` & `flook-0.1.5/src/flook/model/task.py`

 * *Files identical despite different names*

### Comparing `flook-0.1.4/src/flook/module/__init__.py` & `flook-0.1.5/src/flook/module/__init__.py`

 * *Files identical despite different names*

### Comparing `flook-0.1.4/src/flook/module/ansible.py` & `flook-0.1.5/src/flook/module/ansible.py`

 * *Files identical despite different names*

### Comparing `flook-0.1.4/src/flook/module/config.py` & `flook-0.1.5/src/flook/module/config.py`

 * *Files identical despite different names*

### Comparing `flook-0.1.4/src/flook/module/database.py` & `flook-0.1.5/src/flook/module/database.py`

 * *Files identical despite different names*

### Comparing `flook-0.1.4/src/flook/module/file_system.py` & `flook-0.1.5/src/flook/module/file_system.py`

 * *Files identical despite different names*

### Comparing `flook-0.1.4/src/flook/module/logger.py` & `flook-0.1.5/src/flook/module/logger.py`

 * *Files identical despite different names*

### Comparing `flook-0.1.4/src/flook/module/output.py` & `flook-0.1.5/src/flook/module/output.py`

 * *Files 0% similar despite different names*

```diff
@@ -62,8 +62,8 @@
 
         return self._table(data)
 
     def camel_case(self, value):
         """Change string into camel case"""
         value = sub(r"(_|-)+", " ", value).title().replace(" ", "")
 
-        return ''.join([value[0].lower(), value[1:]])
+        return "".join([value[0].lower(), value[1:]])
```

### Comparing `flook-0.1.4/src/flook/module/playbook.py` & `flook-0.1.5/src/flook/module/playbook.py`

 * *Files identical despite different names*

### Comparing `flook-0.1.4/src/flook.egg-info/PKG-INFO` & `flook-0.1.5/src/flook.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: flook
-Version: 0.1.4
+Version: 0.1.5
 Summary: A Lightweight and Flexible Ansible Command Line Tool.
 Home-page: https://github.com/norwik/flook/
 Author: Clivern
 Author-email: hello@clivern.com
 License: MIT
 Project-URL: Documentation, https://github.com/norwik/flook/
 Project-URL: Source, https://github.com/norwik/flook/
```

### Comparing `flook-0.1.4/src/flook.egg-info/SOURCES.txt` & `flook-0.1.5/src/flook.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `flook-0.1.4/tests/__init__.py` & `flook-0.1.5/tests/__init__.py`

 * *Files identical despite different names*

### Comparing `flook-0.1.4/tests/module/test_logger.py` & `flook-0.1.5/tests/module/test_logger.py`

 * *Files identical despite different names*

### Comparing `flook-0.1.4/tox.ini` & `flook-0.1.5/tox.ini`

 * *Files identical despite different names*

