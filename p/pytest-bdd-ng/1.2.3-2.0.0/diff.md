# Comparing `tmp/pytest-bdd-ng-1.2.3.tar.gz` & `tmp/pytest-bdd-ng-2.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pytest-bdd-ng-1.2.3.tar", last modified: Thu Oct  6 16:47:20 2022, max compression
+gzip compressed data, was "pytest-bdd-ng-2.0.0.tar", last modified: Mon Jun 26 09:57:43 2023, max compression
```

## Comparing `pytest-bdd-ng-1.2.3.tar` & `pytest-bdd-ng-2.0.0.tar`

### file list

```diff
@@ -1,56 +1,69 @@
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-06 16:47:20.019213 pytest-bdd-ng-1.2.3/
--rw-r--r--   0 runner    (1001) docker     (121)     1088 2022-10-06 16:47:02.000000 pytest-bdd-ng-1.2.3/AUTHORS.rst
--rw-r--r--   0 runner    (1001) docker     (121)    13725 2022-10-06 16:47:02.000000 pytest-bdd-ng-1.2.3/CHANGES.rst
--rw-r--r--   0 runner    (1001) docker     (121)     1092 2022-10-06 16:47:02.000000 pytest-bdd-ng-1.2.3/LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (121)       80 2022-10-06 16:47:02.000000 pytest-bdd-ng-1.2.3/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (121)    50964 2022-10-06 16:47:20.019213 pytest-bdd-ng-1.2.3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)    48771 2022-10-06 16:47:02.000000 pytest-bdd-ng-1.2.3/README.rst
--rw-r--r--   0 runner    (1001) docker     (121)      823 2022-10-06 16:47:02.000000 pytest-bdd-ng-1.2.3/pyproject.toml
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-06 16:47:20.015213 pytest-bdd-ng-1.2.3/pytest_bdd/
--rw-r--r--   0 runner    (1001) docker     (121)      523 2022-10-06 16:47:02.000000 pytest-bdd-ng-1.2.3/pytest_bdd/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     4847 2022-10-06 16:47:02.000000 pytest-bdd-ng-1.2.3/pytest_bdd/allure_logging.py
--rw-r--r--   0 runner    (1001) docker     (121)    10288 2022-10-06 16:47:02.000000 pytest-bdd-ng-1.2.3/pytest_bdd/ast.py
--rw-r--r--   0 runner    (1001) docker     (121)     1179 2022-10-06 16:47:02.000000 pytest-bdd-ng-1.2.3/pytest_bdd/collector.py
--rw-r--r--   0 runner    (1001) docker     (121)     1547 2022-10-06 16:47:02.000000 pytest-bdd-ng-1.2.3/pytest_bdd/const.py
--rw-r--r--   0 runner    (1001) docker     (121)     5821 2022-10-06 16:47:02.000000 pytest-bdd-ng-1.2.3/pytest_bdd/cucumber_json.py
--rw-r--r--   0 runner    (1001) docker     (121)     1068 2022-10-06 16:47:02.000000 pytest-bdd-ng-1.2.3/pytest_bdd/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (121)     8114 2022-10-06 16:47:02.000000 pytest-bdd-ng-1.2.3/pytest_bdd/generation.py
--rw-r--r--   0 runner    (1001) docker     (121)     3395 2022-10-06 16:47:02.000000 pytest-bdd-ng-1.2.3/pytest_bdd/gherkin_terminal_reporter.py
--rw-r--r--   0 runner    (1001) docker     (121)     2426 2022-10-06 16:47:02.000000 pytest-bdd-ng-1.2.3/pytest_bdd/hooks.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-06 16:47:20.015213 pytest-bdd-ng-1.2.3/pytest_bdd/model/
--rw-r--r--   0 runner    (1001) docker     (121)      175 2022-10-06 16:47:02.000000 pytest-bdd-ng-1.2.3/pytest_bdd/model/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     2369 2022-10-06 16:47:02.000000 pytest-bdd-ng-1.2.3/pytest_bdd/model/feature.py
--rw-r--r--   0 runner    (1001) docker     (121)     7027 2022-10-06 16:47:02.000000 pytest-bdd-ng-1.2.3/pytest_bdd/model/scenario.py
--rw-r--r--   0 runner    (1001) docker     (121)      719 2022-10-06 16:47:02.000000 pytest-bdd-ng-1.2.3/pytest_bdd/packaging.py
--rw-r--r--   0 runner    (1001) docker     (121)    30695 2022-10-06 16:47:02.000000 pytest-bdd-ng-1.2.3/pytest_bdd/parser.py
--rw-r--r--   0 runner    (1001) docker     (121)     4368 2022-10-06 16:47:02.000000 pytest-bdd-ng-1.2.3/pytest_bdd/parsers.py
--rw-r--r--   0 runner    (1001) docker     (121)     5503 2022-10-06 16:47:02.000000 pytest-bdd-ng-1.2.3/pytest_bdd/plugin.py
--rw-r--r--   0 runner    (1001) docker     (121)     5640 2022-10-06 16:47:02.000000 pytest-bdd-ng-1.2.3/pytest_bdd/reporting.py
--rw-r--r--   0 runner    (1001) docker     (121)     7369 2022-10-06 16:47:02.000000 pytest-bdd-ng-1.2.3/pytest_bdd/runner.py
--rw-r--r--   0 runner    (1001) docker     (121)    12685 2022-10-06 16:47:02.000000 pytest-bdd-ng-1.2.3/pytest_bdd/scenario.py
--rw-r--r--   0 runner    (1001) docker     (121)     2519 2022-10-06 16:47:02.000000 pytest-bdd-ng-1.2.3/pytest_bdd/scripts.py
--rw-r--r--   0 runner    (1001) docker     (121)    17009 2022-10-06 16:47:02.000000 pytest-bdd-ng-1.2.3/pytest_bdd/steps.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-06 16:47:20.015213 pytest-bdd-ng-1.2.3/pytest_bdd/struct_bdd/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-10-06 16:47:02.000000 pytest-bdd-ng-1.2.3/pytest_bdd/struct_bdd/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     7421 2022-10-06 16:47:02.000000 pytest-bdd-ng-1.2.3/pytest_bdd/struct_bdd/ast_builder.py
--rw-r--r--   0 runner    (1001) docker     (121)    13399 2022-10-06 16:47:02.000000 pytest-bdd-ng-1.2.3/pytest_bdd/struct_bdd/model.py
--rw-r--r--   0 runner    (1001) docker     (121)     3116 2022-10-06 16:47:02.000000 pytest-bdd-ng-1.2.3/pytest_bdd/struct_bdd/parser.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-06 16:47:20.015213 pytest-bdd-ng-1.2.3/pytest_bdd/templates/
--rw-r--r--   0 runner    (1001) docker     (121)      621 2022-10-06 16:47:02.000000 pytest-bdd-ng-1.2.3/pytest_bdd/templates/test.py.mak
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-06 16:47:20.019213 pytest-bdd-ng-1.2.3/pytest_bdd/typing/
--rw-r--r--   0 runner    (1001) docker     (121)      304 2022-10-06 16:47:02.000000 pytest-bdd-ng-1.2.3/pytest_bdd/typing/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)      139 2022-10-06 16:47:02.000000 pytest-bdd-ng-1.2.3/pytest_bdd/typing/allure.py
--rw-r--r--   0 runner    (1001) docker     (121)      453 2022-10-06 16:47:02.000000 pytest-bdd-ng-1.2.3/pytest_bdd/typing/parser.py
--rw-r--r--   0 runner    (1001) docker     (121)     1880 2022-10-06 16:47:02.000000 pytest-bdd-ng-1.2.3/pytest_bdd/typing/pytest.py
--rw-r--r--   0 runner    (1001) docker     (121)      157 2022-10-06 16:47:02.000000 pytest-bdd-ng-1.2.3/pytest_bdd/typing/struct_bdd.py
--rw-r--r--   0 runner    (1001) docker     (121)     8353 2022-10-06 16:47:02.000000 pytest-bdd-ng-1.2.3/pytest_bdd/utils.py
--rw-r--r--   0 runner    (1001) docker     (121)     1101 2022-10-06 16:47:02.000000 pytest-bdd-ng-1.2.3/pytest_bdd/warning_types.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-06 16:47:20.019213 pytest-bdd-ng-1.2.3/pytest_bdd_ng.egg-info/
--rw-r--r--   0 runner    (1001) docker     (121)    50964 2022-10-06 16:47:19.000000 pytest-bdd-ng-1.2.3/pytest_bdd_ng.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)     1213 2022-10-06 16:47:20.000000 pytest-bdd-ng-1.2.3/pytest_bdd_ng.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2022-10-06 16:47:19.000000 pytest-bdd-ng-1.2.3/pytest_bdd_ng.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (121)       98 2022-10-06 16:47:19.000000 pytest-bdd-ng-1.2.3/pytest_bdd_ng.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (121)      417 2022-10-06 16:47:19.000000 pytest-bdd-ng-1.2.3/pytest_bdd_ng.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (121)       11 2022-10-06 16:47:20.000000 pytest-bdd-ng-1.2.3/pytest_bdd_ng.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (121)     1702 2022-10-06 16:47:20.019213 pytest-bdd-ng-1.2.3/setup.cfg
--rwxr-xr-x   0 runner    (1001) docker     (121)       38 2022-10-06 16:47:02.000000 pytest-bdd-ng-1.2.3/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 09:57:43.129619 pytest-bdd-ng-2.0.0/
+-rw-r--r--   0 runner    (1001) docker     (123)     1098 2023-06-26 09:57:26.000000 pytest-bdd-ng-2.0.0/AUTHORS.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1092 2023-06-26 09:57:26.000000 pytest-bdd-ng-2.0.0/LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     7650 2023-06-26 09:57:43.129619 pytest-bdd-ng-2.0.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     4589 2023-06-26 09:57:26.000000 pytest-bdd-ng-2.0.0/README.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     3628 2023-06-26 09:57:26.000000 pytest-bdd-ng-2.0.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      714 2023-06-26 09:57:43.129619 pytest-bdd-ng-2.0.0/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 09:57:43.121619 pytest-bdd-ng-2.0.0/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 09:57:43.125619 pytest-bdd-ng-2.0.0/src/pytest_bdd/
+-rw-r--r--   0 runner    (1001) docker     (123)      495 2023-06-26 09:57:26.000000 pytest-bdd-ng-2.0.0/src/pytest_bdd/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6172 2023-06-26 09:57:26.000000 pytest-bdd-ng-2.0.0/src/pytest_bdd/allure_logging.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3166 2023-06-26 09:57:26.000000 pytest-bdd-ng-2.0.0/src/pytest_bdd/collector.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 09:57:43.125619 pytest-bdd-ng-2.0.0/src/pytest_bdd/compatibility/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-26 09:57:26.000000 pytest-bdd-ng-2.0.0/src/pytest_bdd/compatibility/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      139 2023-06-26 09:57:26.000000 pytest-bdd-ng-2.0.0/src/pytest_bdd/compatibility/allure.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 09:57:43.125619 pytest-bdd-ng-2.0.0/src/pytest_bdd/compatibility/importlib/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-26 09:57:26.000000 pytest-bdd-ng-2.0.0/src/pytest_bdd/compatibility/importlib/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      233 2023-06-26 09:57:26.000000 pytest-bdd-ng-2.0.0/src/pytest_bdd/compatibility/importlib/metadata.py
+-rw-r--r--   0 runner    (1001) docker     (123)      296 2023-06-26 09:57:26.000000 pytest-bdd-ng-2.0.0/src/pytest_bdd/compatibility/importlib/resources.py
+-rw-r--r--   0 runner    (1001) docker     (123)      761 2023-06-26 09:57:26.000000 pytest-bdd-ng-2.0.0/src/pytest_bdd/compatibility/parser.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4165 2023-06-26 09:57:26.000000 pytest-bdd-ng-2.0.0/src/pytest_bdd/compatibility/pytest.py
+-rw-r--r--   0 runner    (1001) docker     (123)      157 2023-06-26 09:57:26.000000 pytest-bdd-ng-2.0.0/src/pytest_bdd/compatibility/struct_bdd.py
+-rw-r--r--   0 runner    (1001) docker     (123)      183 2023-06-26 09:57:26.000000 pytest-bdd-ng-2.0.0/src/pytest_bdd/compatibility/tomllib.py
+-rw-r--r--   0 runner    (1001) docker     (123)      314 2023-06-26 09:57:26.000000 pytest-bdd-ng-2.0.0/src/pytest_bdd/compatibility/typing.py
+-rw-r--r--   0 runner    (1001) docker     (123)      106 2023-06-26 09:57:26.000000 pytest-bdd-ng-2.0.0/src/pytest_bdd/const.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5864 2023-06-26 09:57:26.000000 pytest-bdd-ng-2.0.0/src/pytest_bdd/cucumber_json.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1033 2023-06-26 09:57:26.000000 pytest-bdd-ng-2.0.0/src/pytest_bdd/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10912 2023-06-26 09:57:26.000000 pytest-bdd-ng-2.0.0/src/pytest_bdd/generation.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3366 2023-06-26 09:57:26.000000 pytest-bdd-ng-2.0.0/src/pytest_bdd/gherkin_terminal_reporter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3040 2023-06-26 09:57:26.000000 pytest-bdd-ng-2.0.0/src/pytest_bdd/hooks.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10179 2023-06-26 09:57:26.000000 pytest-bdd-ng-2.0.0/src/pytest_bdd/message_plugin.py
+-rw-r--r--   0 runner    (1001) docker     (123)      478 2023-06-26 09:57:26.000000 pytest-bdd-ng-2.0.0/src/pytest_bdd/mimetypes.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 09:57:43.125619 pytest-bdd-ng-2.0.0/src/pytest_bdd/model/
+-rw-r--r--   0 runner    (1001) docker     (123)      237 2023-06-26 09:57:26.000000 pytest-bdd-ng-2.0.0/src/pytest_bdd/model/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7291 2023-06-26 09:57:26.000000 pytest-bdd-ng-2.0.0/src/pytest_bdd/model/gherkin_document.py
+-rw-r--r--   0 runner    (1001) docker     (123)    23640 2023-06-26 09:57:26.000000 pytest-bdd-ng-2.0.0/src/pytest_bdd/model/messages.py
+-rw-r--r--   0 runner    (1001) docker     (123)      610 2023-06-26 09:57:26.000000 pytest-bdd-ng-2.0.0/src/pytest_bdd/packaging.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5147 2023-06-26 09:57:26.000000 pytest-bdd-ng-2.0.0/src/pytest_bdd/parser.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11549 2023-06-26 09:57:26.000000 pytest-bdd-ng-2.0.0/src/pytest_bdd/parsers.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11339 2023-06-26 09:57:26.000000 pytest-bdd-ng-2.0.0/src/pytest_bdd/plugin.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5874 2023-06-26 09:57:26.000000 pytest-bdd-ng-2.0.0/src/pytest_bdd/reporting.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8500 2023-06-26 09:57:26.000000 pytest-bdd-ng-2.0.0/src/pytest_bdd/runner.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13591 2023-06-26 09:57:26.000000 pytest-bdd-ng-2.0.0/src/pytest_bdd/scenario.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 09:57:43.129619 pytest-bdd-ng-2.0.0/src/pytest_bdd/script/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-26 09:57:26.000000 pytest-bdd-ng-2.0.0/src/pytest_bdd/script/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3516 2023-06-26 09:57:26.000000 pytest-bdd-ng-2.0.0/src/pytest_bdd/script/bdd_tree_to_rst.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19536 2023-06-26 09:57:26.000000 pytest-bdd-ng-2.0.0/src/pytest_bdd/steps.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 09:57:43.129619 pytest-bdd-ng-2.0.0/src/pytest_bdd/struct_bdd/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-26 09:57:26.000000 pytest-bdd-ng-2.0.0/src/pytest_bdd/struct_bdd/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14996 2023-06-26 09:57:26.000000 pytest-bdd-ng-2.0.0/src/pytest_bdd/struct_bdd/model.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9835 2023-06-26 09:57:26.000000 pytest-bdd-ng-2.0.0/src/pytest_bdd/struct_bdd/model_builder.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3497 2023-06-26 09:57:26.000000 pytest-bdd-ng-2.0.0/src/pytest_bdd/struct_bdd/parser.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2475 2023-06-26 09:57:26.000000 pytest-bdd-ng-2.0.0/src/pytest_bdd/struct_bdd/plugin.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 09:57:43.129619 pytest-bdd-ng-2.0.0/src/pytest_bdd/template/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-26 09:57:26.000000 pytest-bdd-ng-2.0.0/src/pytest_bdd/template/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      704 2023-06-26 09:57:26.000000 pytest-bdd-ng-2.0.0/src/pytest_bdd/template/test.py.mak
+-rw-r--r--   0 runner    (1001) docker     (123)     9515 2023-06-26 09:57:26.000000 pytest-bdd-ng-2.0.0/src/pytest_bdd/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1101 2023-06-26 09:57:26.000000 pytest-bdd-ng-2.0.0/src/pytest_bdd/warning_types.py
+-rw-r--r--   0 runner    (1001) docker     (123)      569 2023-06-26 09:57:26.000000 pytest-bdd-ng-2.0.0/src/pytest_bdd/webloc.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 09:57:43.129619 pytest-bdd-ng-2.0.0/src/pytest_bdd_ng.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     7650 2023-06-26 09:57:43.000000 pytest-bdd-ng-2.0.0/src/pytest_bdd_ng.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1843 2023-06-26 09:57:43.000000 pytest-bdd-ng-2.0.0/src/pytest_bdd_ng.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-26 09:57:43.000000 pytest-bdd-ng-2.0.0/src/pytest_bdd_ng.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      118 2023-06-26 09:57:43.000000 pytest-bdd-ng-2.0.0/src/pytest_bdd_ng.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      775 2023-06-26 09:57:43.000000 pytest-bdd-ng-2.0.0/src/pytest_bdd_ng.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       11 2023-06-26 09:57:43.000000 pytest-bdd-ng-2.0.0/src/pytest_bdd_ng.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 09:57:43.129619 pytest-bdd-ng-2.0.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     1810 2023-06-26 09:57:26.000000 pytest-bdd-ng-2.0.0/tests/test_hooks.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4704 2023-06-26 09:57:26.000000 pytest-bdd-ng-2.0.0/tests/test_utils.py
```

### Comparing `pytest-bdd-ng-1.2.3/AUTHORS.rst` & `pytest-bdd-ng-2.0.0/AUTHORS.rst`

 * *Files 2% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 `Anatoly Bubenkov <bubenkoff@gmail.com>`_
     key implementation idea and realization, many new features and improvements
 
 These people have contributed to `pytest-bdd`, in alphabetical order:
 
 * `Adam Coddington <me@adamcoddington.net>`_
 * `Albert-Jan Nijburg <albertjan@curit.com>`_
-* `Alessio Bogon <youtux>`_
+* `Alessio Bogon <youtux@gmail.com>`_
 * `Andrey Makhnach <andrey.makhnach@gmail.com>`_
 * `Aron Curzon <curzona@gmail.com>`_
 * `Dmitrijs Milajevs <dimazest@gmail.com>`_
 * `Dmitry Kolyagin <pauk-slon>`_
 * `Florian Bruhin <me@the-compiler.org>`_
 * `Floris Bruynooghe <flub@devork.be>`_
 * `Harro van der Klauw <hvdklauw@gmail.com>`_
```

### Comparing `pytest-bdd-ng-1.2.3/LICENSE.txt` & `pytest-bdd-ng-2.0.0/LICENSE.txt`

 * *Files 11% similar despite different names*

```diff
@@ -1,7 +1,7 @@
-Copyright (C) 2013-2022 Oleg Pidsadnyi, Anatoly Bubenkov and others
+Copyright (C) 2013-2023 Oleg Pidsadnyi, Anatoly Bubenkov and others
 
 Permission is hereby granted, free of charge, to any person obtaining a copy of this software and associated documentation files (the "Software"), to deal in the Software without restriction, including without limitation the rights to use, copy, modify, merge, publish, distribute, sublicense, and/or sell copies of the Software, and to permit persons to whom the Software is furnished to do so, subject to the following conditions:
 
 The above copyright notice and this permission notice shall be included in all copies or substantial portions of the Software.
 
 THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY, FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM, OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE SOFTWARE.
```

### Comparing `pytest-bdd-ng-1.2.3/pytest_bdd/allure_logging.py` & `pytest-bdd-ng-2.0.0/src/pytest_bdd/allure_logging.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,17 +1,18 @@
-from __future__ import annotations
-
+import json
 import os
+from unittest.mock import patch
 
 import pytest
 from attr import asdict
+from attr.exceptions import NotAnAttrsClassError
 from pluggy import HookimplMarker
+from pydantic import BaseModel as PydanticBaseModel
 
-from pytest_bdd.model import Feature, Scenario, Step, Tag
-from pytest_bdd.typing.allure import ALLURE_INSTALLED
+from pytest_bdd.compatibility.allure import ALLURE_INSTALLED
 
 if ALLURE_INSTALLED:
     from allure_commons import hookimpl
     from allure_commons import plugin_manager as allure_plugin_manager
     from allure_commons._allure import StepContext
     from allure_commons.model2 import Label, Parameter, Status, TestStepResult
     from allure_commons.types import LabelType
@@ -22,55 +23,75 @@
 
 
 class AllurePytestBDD:
     def __init__(self, allure_logger, allure_cache):
         self.allure_logger = allure_logger
         self._cache = allure_cache
 
+        self.allure_plugin_name = None
+        self.pytest_plugin_name = None
+
     @classmethod
     def register_if_allure_accessible(cls, config):
         pluginmanager = config.pluginmanager
         allure_accessible = pluginmanager.hasplugin("allure_pytest") and config.option.allure_report_dir
         if allure_accessible:
             allure_plugin_manager.get_plugins()
 
             listener = next(
                 filter(lambda plugin: isinstance(plugin, AllureListener), allure_plugin_manager.get_plugins())
             )
 
             bdd_listener = cls(listener.allure_logger, listener._cache)
-            allure_plugin_manager.register(bdd_listener)
-            pluginmanager.register(bdd_listener)
+            bdd_listener.allure_plugin_name = allure_plugin_manager.register(bdd_listener)
+            bdd_listener.pytest_plugin_name = pluginmanager.register(bdd_listener)
+            return bdd_listener
 
     @hookimpl(hookwrapper=True)
     def report_result(self, result):
-        recomposable_features = []
+        def patched_asdict(*args, recurse=True, value_serializer=None, **kwargs):
+            def patched_value_serializer(instance, field, value):
+                if isinstance(value, PydanticBaseModel):
+                    # Maybe possible to speedup; Some values are not serialized when used value.dict()
+                    return json.loads(value.json())
+                elif value_serializer is not patched_value_serializer:
+                    return value_serializer(instance, field, value)
+                else:
+                    if recurse:
+                        try:
+                            return patched_asdict(
+                                value, *args[1:], recurse=True, value_serializer=patched_value_serializer, **kwargs
+                            )
+                        except NotAnAttrsClassError:
+                            return value
+                    else:
+                        return value
+
+            if value_serializer is None:
+                value_serializer = patched_value_serializer
 
-        def decompose_scenario_or_feature(attr, value):
-            if isinstance(value, (Tag, Step, Scenario, Feature)):
-                if isinstance(value, Feature):
-                    recomposable_features.append(value)
-                value.decompose()
-            return True
+            return asdict(*args, value_serializer=patched_value_serializer, **kwargs)
 
-        asdict(result, filter=decompose_scenario_or_feature)
+        with patch("allure_commons.logger.asdict", new=patched_asdict):
+            yield
 
-        yield
-
-        while recomposable_features:
-            recomposable_features.pop().compose()
+    def unregister(self, config):
+        pluginmanager = config.pluginmanager
+        allure_accessible = pluginmanager.hasplugin("allure_pytest") and config.option.allure_report_dir
+        if allure_accessible:
+            allure_plugin_manager.unregister(name=self.allure_plugin_name)
+            pluginmanager.unregister(name=self.pytest_plugin_name)
 
     @pytest.hookimpl
     def pytest_bdd_before_step_call(self, request, feature, scenario, step, step_func, step_func_args, step_definition):
         """Called before step function is set up."""
-        step_definition.func = StepContext(f"{step.keyword} {step.name}", step_func_args)(step_func)
+        step_definition.func = StepContext(f"{step.keyword} {step.text}", step_func_args)(step_func)
 
     @pytest.hookimpl
     def pytest_bdd_before_scenario(self, request, feature, scenario):
-
         scenario_result_uuid = self._cache.get(scenario)
         test_result_uuid = self._cache.get(request.node.nodeid)
 
         if not scenario_result_uuid:
             scenario_result_uuid = self._cache.push(scenario)
 
         self.allure_logger.start_step(test_result_uuid, scenario_result_uuid, TestStepResult())
```

### Comparing `pytest-bdd-ng-1.2.3/pytest_bdd/cucumber_json.py` & `pytest-bdd-ng-2.0.0/src/pytest_bdd/cucumber_json.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,32 +1,29 @@
 """Cucumber json output formatter."""
-from __future__ import annotations
-
 import json
 import math
 import os
 import time
-from typing import TYPE_CHECKING, Any, cast
+from typing import TYPE_CHECKING, Any, Dict, Sequence, Union, cast
 
-from pytest_bdd.typing import Protocol, runtime_checkable
-from pytest_bdd.typing.pytest import Parser, TerminalReporter, TestReport
+from pytest_bdd.compatibility.pytest import Parser, TerminalReporter, TestReport
+from pytest_bdd.compatibility.typing import Protocol, runtime_checkable
 
 if TYPE_CHECKING:  # pragma: no cover
-
-    from pytest_bdd.typing.pytest import Config as BaseConfig
+    from pytest_bdd.compatibility.pytest import Config as BaseConfig
 
     @runtime_checkable
     class LogBDDCucumberJSONProtocol(Protocol):
-        _bddcucumberjson: LogBDDCucumberJSON
+        _bddcucumberjson: "LogBDDCucumberJSON"
 
     class Config(BaseConfig, LogBDDCucumberJSONProtocol):  # type: ignore[misc]
         pass
 
 else:
-    from pytest_bdd.typing.pytest import Config
+    from pytest_bdd.compatibility.pytest import Config
 
 
 def add_options(parser: Parser) -> None:
     """Add pytest-bdd options."""
     group = parser.getgroup("bdd", "Cucumber JSON")
     group.addoption(
         "--cucumberjson",
@@ -35,57 +32,57 @@
         dest="cucumber_json_path",
         metavar="path",
         default=None,
         help="create cucumber json style report file at given path.",
     )
 
 
-def configure(config: Config | BaseConfig) -> None:
+def configure(config: Union[Config, "BaseConfig"]) -> None:
     cucumber_json_path = config.option.cucumber_json_path
     # prevent opening json log on worker nodes (xdist)
     if cucumber_json_path and not hasattr(config, "workerinput"):
         cast(Config, config)._bddcucumberjson = LogBDDCucumberJSON(cucumber_json_path)
         config.pluginmanager.register(cast(Config, config)._bddcucumberjson)
 
 
-def unconfigure(config: Config | BaseConfig) -> None:
+def unconfigure(config: Union[Config, "BaseConfig"]) -> None:
     xml = getattr(config, "_bddcucumberjson", None)
     if xml is not None:
         _config = cast(Config, config)
         del _config._bddcucumberjson
         config.pluginmanager.unregister(xml)
 
 
 class LogBDDCucumberJSON:
 
     """Logging plugin for cucumber like json output."""
 
     def __init__(self, logfile: str) -> None:
         logfile = os.path.expanduser(os.path.expandvars(logfile))
         self.logfile = os.path.normpath(os.path.abspath(logfile))
-        self.features: dict[str, dict] = {}
+        self.features: Dict[str, dict] = {}
 
-    def _get_result(self, step: dict[str, Any], report: TestReport, error_message: bool = False) -> dict[str, Any]:
+    def _get_result(self, step: Dict[str, Any], report: TestReport, error_message: bool = False) -> Dict[str, Any]:
         """Get scenario test run result.
 
         :param step: `StepHandler` step we get result for
         :param report: pytest `Report` object
         :return: `dict` in form {"status": "<passed|failed|skipped>", ["error_message": "<error_message>"]}
         """
-        result: dict[str, Any] = {}
+        result: Dict[str, Any] = {}
         if report.passed or not step["failed"]:  # ignore setup/teardown
             result = {"status": "passed"}
         elif report.failed and step["failed"]:
             result = {"status": "failed", "error_message": str(report.longrepr) if error_message else ""}
         elif report.skipped:
             result = {"status": "skipped"}
         result["duration"] = int(math.floor((10**9) * step["duration"]))  # nanosec
         return result
 
-    def _serialize_tags(self, item: dict[str, Any]) -> list[dict[str, Any]]:
+    def _serialize_tags(self, item: Dict[str, Any]) -> Sequence[Dict[str, Any]]:
         """Serialize item's tags.
 
         :param item: json-serialized `Scenario` or `Feature`.
         :return: `list` of `dict` in the form of:
             [
                 {
                     "name": "<tag>",
@@ -102,15 +99,15 @@
             # skip reporting for non-bdd tests
             return
 
         if not scenario["steps"] or report.when != "call":
             # skip if there isn't a result or scenario has no steps
             return
 
-        def stepmap(step: dict[str, Any]) -> dict[str, Any]:
+        def stepmap(step: Dict[str, Any]) -> Dict[str, Any]:
             error_message = False
             if step["failed"] and not scenario.setdefault("failed", False):
                 scenario["failed"] = True
                 error_message = True
 
             step_name = step["name"]
```

### Comparing `pytest-bdd-ng-1.2.3/pytest_bdd/exceptions.py` & `pytest-bdd-ng-2.0.0/src/pytest_bdd/exceptions.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,9 +1,8 @@
 """pytest-bdd Exceptions."""
-from __future__ import annotations
 
 
 class ScenarioIsDecoratorOnly(Exception):
     """Scenario can be only used as decorator."""
 
 
 class ScenarioValidationError(Exception):
```

### Comparing `pytest-bdd-ng-1.2.3/pytest_bdd/gherkin_terminal_reporter.py` & `pytest-bdd-ng-2.0.0/src/pytest_bdd/gherkin_terminal_reporter.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,10 @@
-from __future__ import annotations
-
 from typing import Any
 
-from pytest_bdd.typing.pytest import Config, Parser, TerminalReporter, TestReport
+from pytest_bdd.compatibility.pytest import Config, Parser, TerminalReporter, TestReport
 
 
 def add_options(parser: Parser) -> None:
     group = parser.getgroup("terminal reporting", "reporting", after="general")
     group._addoption(
         "--gherkin-terminal-reporter",
         action="store_true",
```

### Comparing `pytest-bdd-ng-1.2.3/pytest_bdd/packaging.py` & `pytest-bdd-ng-2.0.0/src/pytest_bdd/packaging.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,28 +1,22 @@
-from __future__ import annotations
-
-import sys
 from functools import lru_cache
 from operator import eq
 from typing import Any, Callable
 
 from packaging.utils import Version
 
-if sys.version_info >= (3, 10):
-    from importlib.metadata import version
-else:
-    from importlib_metadata import version
+from pytest_bdd.compatibility.importlib.metadata import version
 
 
 def get_distribution_version(distribution_name: str) -> Version:
     return Version(version(distribution_name))
 
 
 def parse_version(version: str) -> Version:
     return Version(version)
 
 
-@lru_cache()
+@lru_cache
 def compare_distribution_version(
     distribution_name: str, version: str, operator: Callable[[Any, Any], bool] = eq
 ) -> bool:
     return operator(get_distribution_version(distribution_name), parse_version(version))
```

### Comparing `pytest-bdd-ng-1.2.3/pytest_bdd/reporting.py` & `pytest-bdd-ng-2.0.0/src/pytest_bdd/reporting.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,49 +1,48 @@
 """Reporting functionality.
 
 Collection of the scenario execution statuses, timing and other information
 that enriches the pytest test reporting.
 """
-from __future__ import annotations
-
 import time
-from typing import Any, Callable
+from typing import Any, Callable, Dict, List, Sequence
 
 import pytest
 from attr import Factory, attrib, attrs
 
-from pytest_bdd.model import Feature, Scenario, Step
-from pytest_bdd.typing.pytest import CallInfo, FixtureRequest, Item
+from pytest_bdd.compatibility.pytest import CallInfo, FixtureRequest, Item
+from pytest_bdd.model import Feature
+from pytest_bdd.model.messages import Pickle, PickleStep
 
 
 class StepReport:
     """StepHandler execution report."""
 
     failed = False
     stopped = None
 
-    def __init__(self, step: Step) -> None:
+    def __init__(self, step: PickleStep) -> None:
         """StepHandler report constructor.
 
         :param StepHandler step: StepHandler.
         """
         self.step = step
         self.started = time.perf_counter()
 
-    def serialize(self) -> dict[str, Any]:
+    def serialize(self, feature: Feature) -> Dict[str, Any]:
         """Serialize the step execution report.
 
         :return: Serialized step execution report.
         :rtype: dict
         """
         return {
-            "name": self.step.name,
-            "type": self.step.prefix,
-            "keyword": self.step.keyword,
-            "line_number": self.step.line_number,
+            "name": self.step.text,
+            "type": feature._get_step_prefix(self.step),
+            "keyword": feature._get_step_keyword(self.step),
+            "line_number": feature._get_step_line_number(self.step),
             "failed": self.failed,
             "duration": self.duration,
         }
 
     def finalize(self, failed: bool) -> None:
         """Stop collecting information and finalize the report.
 
@@ -63,19 +62,19 @@
             return 0
 
         return self.stopped - self.started
 
 
 @attrs
 class ScenarioReport:
-    """Scenario execution report."""
+    """Pickle execution report."""
 
     feature: Feature = attrib()
-    scenario: Scenario = attrib()
-    step_reports: list[StepReport] = attrib(default=Factory(list))
+    scenario: Pickle = attrib()
+    step_reports: List[StepReport] = attrib(default=Factory(list))
 
     @property
     def current_step_report(self) -> StepReport:
         """Get current step report.
 
         :return: Last or current step report.
         :rtype: pytest_bdd.reporting.StepReport
@@ -86,28 +85,28 @@
         """Add new step report.
 
         :param step_report: New current step report.
         :type step_report: pytest_bdd.reporting.StepReport
         """
         self.step_reports.append(step_report)
 
-    def serialize(self) -> dict[str, Any]:
+    def serialize(self) -> Dict[str, Any]:
         """Serialize scenario execution report in order to transfer reporting from nodes in the distributed mode.
 
         :return: Serialized report.
         :rtype: dict
         """
         pickle = self.scenario
-        feature = self.feature
+        feature: Feature = self.feature
 
         return {
-            "steps": [step_report.serialize() for step_report in self.step_reports],
+            "steps": [step_report.serialize(self.feature) for step_report in self.step_reports],
             "name": pickle.name,
-            "line_number": pickle.line_number,
-            "tags": sorted(set(pickle.tag_names).difference(feature.tag_names)),
+            "line_number": feature._get_pickle_line_number(pickle),
+            "tags": sorted(set(feature._get_pickle_tag_names(pickle)).difference(feature.tag_names)),
             "feature": {
                 "name": feature.name,
                 "filename": feature.filename,
                 "rel_filename": feature.rel_filename,
                 "line_number": feature.line_number,
                 "description": feature.description,
                 "tags": feature.tag_names,
@@ -126,57 +125,57 @@
             self.add_step_report(report)
 
 
 class ScenarioReporterPlugin:
     def __init__(self):
         self.current_report = None
 
-    @pytest.mark.hookwrapper
+    @pytest.hookimpl(hookwrapper=True)
     def pytest_runtest_makereport(self, item: Item, call: CallInfo):
         outcome = yield
         if call.when != "setup":
             rep = outcome.get_result()
             """Store item in the report object."""
             scenario_report: ScenarioReport = self.current_report
 
             if scenario_report is not None:
                 rep.scenario = scenario_report.serialize()
                 rep.item = {"name": item.name}
 
-    @pytest.mark.tryfirst
-    def pytest_bdd_before_scenario(self, request: FixtureRequest, feature: Feature, scenario: Scenario) -> None:
+    @pytest.hookimpl(tryfirst=True)
+    def pytest_bdd_before_scenario(self, request: FixtureRequest, feature: Feature, scenario: Pickle) -> None:
         """Create scenario report for the item."""
         self.current_report = ScenarioReport(feature=feature, scenario=scenario)  # type: ignore[call-arg]
 
-    @pytest.mark.tryfirst
+    @pytest.hookimpl(tryfirst=True)
     def pytest_bdd_step_error(
         self,
         request: FixtureRequest,
         feature: Feature,
-        scenario: Scenario,
-        step: Step,
+        scenario: Pickle,
+        step: PickleStep,
         step_func: Callable,
         step_func_args: dict,
         exception: Exception,
     ) -> None:
         """Finalize the step report as failed."""
         self.current_report.fail()
 
-    @pytest.mark.tryfirst
+    @pytest.hookimpl(tryfirst=True)
     def pytest_bdd_before_step(
-        self, request: FixtureRequest, feature: Feature, scenario: Scenario, step: Step, step_func: Callable
+        self, request: FixtureRequest, feature: Feature, scenario: Pickle, step: PickleStep, step_func: Callable
     ) -> None:
         """Store step start time."""
         self.current_report.add_step_report(StepReport(step=step))
 
-    @pytest.mark.tryfirst
+    @pytest.hookimpl(tryfirst=True)
     def pytest_bdd_after_step(
         self,
         request: FixtureRequest,
         feature: Feature,
-        scenario: Scenario,
-        step: Step,
+        scenario: Pickle,
+        step: PickleStep,
         step_func: Callable,
         step_func_args: dict,
     ) -> None:
         """Finalize the step report as successful."""
         self.current_report.current_step_report.finalize(failed=False)
```

### Comparing `pytest-bdd-ng-1.2.3/pytest_bdd/runner.py` & `pytest-bdd-ng-2.0.0/src/pytest_bdd/runner.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,30 +1,32 @@
-from __future__ import annotations
-
 from collections import deque
-from contextlib import suppress
+from contextlib import contextmanager, suppress
 from functools import partial
 from itertools import zip_longest
 from operator import attrgetter
+from typing import Optional
 
+from pluggy import PluginManager
 from pytest import hookimpl
 
 from pytest_bdd import exceptions
-from pytest_bdd.model import Feature, Scenario
+from pytest_bdd.compatibility.pytest import FixtureRequest, Item, call_fixture_func
+from pytest_bdd.model import Feature
+from pytest_bdd.model import Pickle as Scenario
+from pytest_bdd.model.messages import PickleStep
 from pytest_bdd.steps import StepHandler
-from pytest_bdd.typing.pytest import FixtureRequest, Item, call_fixture_func
 from pytest_bdd.utils import DefaultMapping, get_args, inject_fixture
 
 
 class ScenarioRunner:
-    def __init__(self):
-        self.request: FixtureRequest | None = None
-        self.feature = None
+    def __init__(self) -> None:
+        self.request: Optional[FixtureRequest] = None
+        self.feature: Optional[Feature] = None
         self.scenario = None
-        self.plugin_manager = None
+        self.plugin_manager: Optional[PluginManager] = None
 
     def pytest_runtest_call(self, item: Item):
         if "pytest_bdd_scenario" in list(map(attrgetter("name"), item.iter_markers())):
             self.request = item._request
             self.feature = self.request.getfixturevalue("feature")
             self.scenario = self.request.getfixturevalue("scenario")
             self.plugin_manager = self.request.config.hook
@@ -67,64 +69,82 @@
                 self.plugin_manager.pytest_bdd_run_step(
                     request=request, feature=feature, scenario=scenario, step=step, previous_step=previous_step
                 )  # type: ignore[call-arg]
                 previous_step = step
 
         return dispatcher
 
-    def pytest_bdd_run_step(self, request, feature, scenario, step, previous_step):
-        hook_kwargs = dict(
-            request=request,
-            feature=feature,
-            scenario=scenario,
-            step=step,
-            previous_step=previous_step,
-        )
-
-        try:
-            step_definition = self._match_to_step(step, previous_step)
-        except exceptions.StepDefinitionNotFoundError as exception:
-            hook_kwargs["exception"] = exception
-            self.request.config.hook.pytest_bdd_step_func_lookup_error(**hook_kwargs)
-            raise
+    @contextmanager
+    def extended_step_context(self, feature: Feature, scenario, step):
+        if isinstance(step, PickleStep):
+            try:
+                step.__dict__["doc_string"] = feature._get_step_doc_string(step)
+                step.__dict__["data_table"] = feature._get_step_data_table(step)
+                step.__dict__["keyword"] = feature._get_step_keyword(step)
+                step.__dict__["line_number"] = feature._get_step_line_number(step)
+                yield
+            finally:
+                step.__dict__.pop("doc_string", None)
+                step.__dict__.pop("data_table", None)
+                step.__dict__.pop("keyword", None)
+                step.__dict__.pop("line_number", None)
         else:
-            hook_kwargs["step_func"] = step_definition.func
-            hook_kwargs["step_definition"] = step_definition
+            yield
 
-        self.request.config.hook.pytest_bdd_before_step(**hook_kwargs)
-
-        hook_kwargs["step_func_args"] = {}
-        step_params = step_definition.get_parameters(step)
-        try:
-            self._inject_step_parameters_as_fixtures(
-                step_params=step_params, params_fixtures_mapping=step_definition.params_fixtures_mapping
+    def pytest_bdd_run_step(self, request, feature: Feature, scenario, step, previous_step):
+        with self.extended_step_context(feature, scenario, step):
+            hook_kwargs = dict(
+                request=request,
+                feature=feature,
+                scenario=scenario,
+                step=step,
+                previous_step=previous_step,
             )
 
-            step_function_kwargs = dict(self._get_step_function_kwargs(step, step_definition, step_params))
-            hook_kwargs["step_func_args"] = step_function_kwargs
+            try:
+                step_definition = self._match_to_step(step, previous_step)
+            except exceptions.StepDefinitionNotFoundError as exception:
+                hook_kwargs["exception"] = exception
+                request.config.hook.pytest_bdd_step_func_lookup_error(**hook_kwargs)
+                raise
+            else:
+                hook_kwargs["step_func"] = step_definition.func
+                hook_kwargs["step_definition"] = step_definition
+
+            request.config.hook.pytest_bdd_before_step(**hook_kwargs)
+
+            hook_kwargs["step_func_args"] = {}
+            step_params = step_definition.get_parameters(step)
+            try:
+                self._inject_step_parameters_as_fixtures(
+                    step_params=step_params, params_fixtures_mapping=step_definition.params_fixtures_mapping
+                )
+
+                step_function_kwargs = dict(self._get_step_function_kwargs(step, step_definition, step_params))
+                hook_kwargs["step_func_args"] = step_function_kwargs
 
-            self.request.config.hook.pytest_bdd_before_step_call(**hook_kwargs)
+                request.config.hook.pytest_bdd_before_step_call(**hook_kwargs)
 
-            step_caller = self.request.config.hook.pytest_bdd_get_step_caller(**hook_kwargs)
-            step_result = step_caller()
+                step_caller = request.config.hook.pytest_bdd_get_step_caller(**hook_kwargs)
+                step_result = step_caller()
 
-            self._inject_target_fixtures(step_definition, step_result)
-            self.request.config.hook.pytest_bdd_after_step(**hook_kwargs)
-        except Exception as exception:
-            hook_kwargs["exception"] = exception
-            self.request.config.hook.pytest_bdd_step_error(**hook_kwargs)
-            raise
+                self._inject_target_fixtures(step_definition, step_result)
+                request.config.hook.pytest_bdd_after_step(**hook_kwargs)
+            except Exception as exception:
+                hook_kwargs["exception"] = exception
+                request.config.hook.pytest_bdd_step_error(**hook_kwargs)
+                raise
 
     @hookimpl(trylast=True)
     def pytest_bdd_get_step_caller(self, request, feature, scenario, step, step_func, step_func_args, step_definition):
         # Execute the step as if it was a pytest fixture, so that we can allow "yield" statements in it
         return partial(call_fixture_func, fixturefunc=step_definition.func, request=request, kwargs=step_func_args)
 
     def _inject_step_parameters_as_fixtures(
-        self, step_params: dict | None = None, params_fixtures_mapping: dict | None = None
+        self, step_params: Optional[dict] = None, params_fixtures_mapping: Optional[dict] = None
     ):
         step_params = step_params or {}
         params_fixtures_mapping = (
             DefaultMapping.instantiate_from_collection_or_bool(
                 params_fixtures_mapping or {}, warm_up_keys=step_params.keys()
             )
             or {}
@@ -163,13 +183,13 @@
                 feature=self.feature,
                 scenario=self.scenario,
                 step=step,
                 previous_step=previous_step,
             )
         except StepHandler.Matcher.MatchNotFoundError as e:
             raise exceptions.StepDefinitionNotFoundError(
-                f'Step definition is not found: "{step.name}". '
+                f'Step definition is not found: "{step.text}". '
                 f'Step keyword: "{step.keyword}". '
                 f"Line {step.line_number} "
                 f'in scenario "{self.scenario.name}" '
-                f'in the feature "{self.feature.filename}"'
+                f'in the feature "{self.feature.uri}"'
             ) from e
```

### Comparing `pytest-bdd-ng-1.2.3/pytest_bdd/scenario.py` & `pytest-bdd-ng-2.0.0/src/pytest_bdd/scenario.py`

 * *Files 22% similar despite different names*

```diff
@@ -6,223 +6,246 @@
 Example:
 
 test_publish_article = scenario(
     feature_name="publish_article.feature",
     scenario_name="Publishing the article",
 )
 """
-from __future__ import annotations
-
+import asyncio
 import collections
-from functools import reduce
-from operator import truediv
-from os.path import commonpath, dirname
+import os
+import ssl
+from contextlib import suppress
+from enum import Enum
+from functools import partial, reduce
+from operator import methodcaller, truediv
+from os.path import commonpath
 from pathlib import Path
-from typing import Callable, Iterable, Sequence, cast
+from tempfile import NamedTemporaryFile
+from typing import Callable, Iterable, Optional, Tuple, Type, Union, cast
+from urllib.parse import urljoin
 
-import pytest
+import aiohttp
+import certifi
 from attr import Factory, attrib, attrs
+from pytest import mark
 
-from pytest_bdd.model import Feature, Scenario
+from pytest_bdd.compatibility.parser import ParserProtocol
+from pytest_bdd.compatibility.pytest import Config, Parser, get_config_root_path
+from pytest_bdd.mimetypes import Mimetype
+from pytest_bdd.model import Feature
+from pytest_bdd.model.messages import Pickle
 from pytest_bdd.parser import GherkinParser
-from pytest_bdd.typing.parser import ParserProtocol
-from pytest_bdd.typing.pytest import Config, Metafunc, Parser
-from pytest_bdd.utils import get_caller_module_locals, get_caller_module_path, make_python_name
+from pytest_bdd.utils import PytestBDDIdGeneratorHandler, compose, make_python_name
 
 Args = collections.namedtuple("Args", ["args", "kwargs"])
 
 
 def add_options(parser: Parser):
     """Add pytest-bdd options."""
     group = parser.getgroup("bdd", "Scenario")
     group.addoption(
-        "--feature-autoload",
-        action="store_true",
+        "--disable-feature-autoload",
+        action="store_false",
         dest="feature_autoload",
-        default=None,
-        help="Turn on feature files autoload",
+        default=True,
+        help="Turn off feature files autoload",
     )
     parser.addini(
-        "feature_autoload",
-        default=False,
+        "disable_feature_autoload",
+        default=True,
         type="bool",
-        help="Turn on feature files autoload",
+        help="Turn off feature files autoload",
     )
 
 
 @attrs
-class FileScenarioLocator:
-    feature_paths = attrib(default=Factory(list))
-    scenario_filter = attrib(default=None)
-    encoding = attrib(default="utf-8")
-    features_base_dir = attrib(default=None)
-    parser: ParserProtocol = attrib(default=Factory(GherkinParser))
-    parse_args: Args = attrib(default=Factory(lambda: Args((), {})))
-
-    @property
-    def glob(self):
-        return self.parser.glob
-
-    def resolve(self):
-        features_base_dir = (
-            self.features_base_dir() if isinstance(self.features_base_dir, Callable) else self.features_base_dir
+class UrlScenarioLocator:
+    url_paths = attrib()
+    filter_ = attrib()
+    encoding = attrib()
+    features_base_url = attrib()
+    mimetype = attrib()
+    parser_type = attrib()
+    parse_args = attrib()
+
+    async def fetch(self, session: aiohttp.ClientSession, url):
+        sslcontext = ssl.create_default_context(cafile=certifi.where())
+        async with session.get(url, ssl=sslcontext) as response:
+            return response.content_type, await response.text(encoding=self.encoding)
+
+    async def fetch_all(self, urls):
+        async with aiohttp.ClientSession() as session:
+            return await asyncio.gather(*[self.fetch(session, url) for url in urls], return_exceptions=True)
+
+    def resolve(self, config: Union[Config, PytestBDDIdGeneratorHandler]):
+        urls = list(
+            self.url_paths
+            if self.features_base_url is None
+            else map(partial(urljoin, self.features_base_url), self.url_paths)
         )
-        features_base_dir = (Path.cwd() / Path(features_base_dir)).resolve()
-
-        already_resolved = set()
-
-        def feature_paths_gen():
-            for feature_path in map(Path, self.feature_paths):
-                if feature_path.is_dir():
-                    yield from iter(self.glob(feature_path))
-                else:
-                    yield feature_path
-
-        for feature_path in feature_paths_gen():
-            if feature_path.is_absolute():
-                try:
-                    common_path = Path(commonpath([feature_path, features_base_dir]))
-                except ValueError:
-                    rel_feature_path = feature_path
-                else:
-                    sub_levels = len(features_base_dir.relative_to(common_path).parts)
-                    sub_path = reduce(truediv, [".."] * sub_levels, Path())
-                    rel_feature_path = sub_path / feature_path.relative_to(common_path)
+        if not urls:
+            return
+        loop = asyncio.new_event_loop()
+        responses = loop.run_until_complete(self.fetch_all(urls))
+
+        # Wait 250 ms for the underlying SSL connections to close
+        loop.run_until_complete(asyncio.sleep(0.250))
+        loop.close()
+
+        hook_handler = cast(Config, config).hook
+        encoding = self.encoding
+
+        for url, response in zip(urls, responses):
+            if isinstance(response, Exception):
+                continue
+
+            mimetype, feature_content = response
+
+            if self.mimetype is not None:
+                mimetype = self.mimetype
+
+                if isinstance(mimetype, Mimetype):
+                    mimetype = mimetype.value
+
+            if self.parser_type is None:
+                parser_type = hook_handler.pytest_bdd_get_parser(
+                    config=config,
+                    mimetype=mimetype,
+                )
             else:
-                rel_feature_path = feature_path
+                parser_type = self.parser_type
 
-            uri = str(rel_feature_path.as_posix())
-            absolute_feature_path = (Path(features_base_dir) / rel_feature_path).resolve()
+            if parser_type is None:
+                break
 
-            if absolute_feature_path not in already_resolved:
-                already_resolved.add(absolute_feature_path)
+            parser = parser_type(id_generator=cast(PytestBDDIdGeneratorHandler, config).pytest_bdd_id_generator)
 
-                feature = self.parser.parse(
-                    absolute_feature_path,
-                    uri,
+            try:
+                filename = None
+                with NamedTemporaryFile(mode="w", delete=False) as f:
+                    filename = f.name
+                    f.write(feature_content)
+
+                feature = parser.parse(
+                    config,
+                    Path(filename),
+                    url,
                     *self.parse_args.args,
-                    **{**dict(encoding=self.encoding), **self.parse_args.kwargs},
+                    **{**dict(encoding=encoding), **self.parse_args.kwargs},
                 )
 
-                for scenario in feature.scenarios:
-                    if self.scenario_filter is None or self.scenario_filter(feature, scenario):
-                        yield feature, scenario
+                for pickle in feature.pickles:
+                    if self.filter_ is None or self.filter_(config, feature, pickle):  # type: ignore
+                        yield feature, pickle
+            finally:
+                if filename is not None:
+                    with suppress(Exception):
+                        os.unlink(filename)
 
 
 @attrs
-class ModuleScenarioRegistry:
-
-    caller_locals = attrib()
-    caller_module_path = attrib()
-    locator_registry: list[tuple] = attrib(default=Factory(list))
-    resolved_locator_registry: dict = attrib(default=Factory(dict))
-    resolved = attrib(default=False)
-    config = attrib(default=None)
-
-    @classmethod
-    def get(
-        cls,
-        caller_locals: dict | None = None,
-        caller_module_path: str = None,
-    ) -> ModuleScenarioRegistry:
-        caller_locals = cast(
-            dict, caller_locals if caller_locals is not None else get_caller_module_locals(stacklevel=2)
-        )
-        caller_module_path = cast(
-            str, caller_module_path if caller_module_path is not None else get_caller_module_path(stacklevel=2)
-        )
-        if "__pytest_bdd_scenario_registry__" not in caller_locals.keys():
-            caller_locals["__pytest_bdd_scenario_registry__"] = ModuleScenarioRegistry(  # type: ignore[call-arg]
-                caller_locals=caller_locals, caller_module_path=caller_module_path
-            )
-        return cast(ModuleScenarioRegistry, caller_locals["__pytest_bdd_scenario_registry__"])
-
-    def add(self, locator, test_func):
-        test_func.__pytest_bdd_scenario_registry__ = self
-        self.locator_registry.append((locator, test_func))
-        if test_func.__name__ not in self.caller_locals.keys():
-            self.caller_locals[test_func.__name__] = test_func
-
-    def update(self, locator, updatable, test_func):
-        for index, (registry_locator, registry_test_func) in enumerate(self.locator_registry):
-            if locator == registry_locator:
-                del self.caller_locals[updatable.__name__]
-                self.add(locator, test_func)
-                break
+class FileScenarioLocator:
+    feature_paths = attrib(default=Factory(list))
+    filter_: Optional[Callable[[Config, Feature, Pickle], Tuple[Feature, Pickle]]] = attrib(default=None)
+    encoding = attrib(default="utf-8")
+    features_base_dir: Optional[Union[str, Path]] = attrib(default=None)
+    mimetype: Optional[str] = attrib(default=None)
+    parser_type: Optional[Type[ParserProtocol]] = attrib(default=GherkinParser)
+    parse_args: Args = attrib(default=Factory(lambda: Args((), {})))
 
-    @property
-    def resolved_locators(self):
-        if not self.resolved:
-            self.resolved = True
-            for locator, test_func in self.locator_registry:
-                for feature, scenario in locator.resolve():
-                    self.resolved_locator_registry[(feature.uri, scenario.id)] = test_func, feature, scenario
-        return self.resolved_locator_registry
-
-    def parametrize(self, metafunc: Metafunc):
-        test_func = metafunc.function
-        self.config = metafunc.config
-
-        parametrizations = [
-            (feature, scenario) for _, (func, feature, scenario) in self.resolved_locators.items() if func is test_func
-        ]
-
-        metafunc.parametrize(
-            "feature, scenario",
-            [self._build_scenario_param(feature, scenario, self.config) for feature, scenario in parametrizations],
-        )
+    def _resolve_features_base_dir(self, config: Union[Config, PytestBDDIdGeneratorHandler]):
+        try:
+            if self.features_base_dir is None:
+                features_base_dir = cast(Config, config).getini("bdd_features_base_dir")
+            else:
+                features_base_dir = self.features_base_dir
+        except (ValueError, KeyError):
+            features_base_dir = get_config_root_path(cast(Config, config))
+        else:
+            if callable(features_base_dir):
+                features_base_dir = features_base_dir(config)
+
+            features_base_dir = (get_config_root_path(cast(Config, config)) / Path(features_base_dir)).resolve()
+
+        return features_base_dir
+
+    def _gen_feature_paths(self, features_base_dir):
+        for feature_pathlike in self.feature_paths:
+            if isinstance(feature_pathlike, Path):
+                feature_path = features_base_dir / feature_pathlike
+                if feature_path.is_dir():
+                    yield from filter(methodcaller("is_file"), feature_path.glob("**/*"))
+                else:
+                    yield feature_path
+            else:
+                try:
+                    yield from filter(methodcaller("is_file"), features_base_dir.glob(str(feature_pathlike)))
+                except IndexError:
+                    yield from filter(methodcaller("is_file"), features_base_dir.glob("**/*"))
 
     @staticmethod
-    def _build_scenario_param(feature: Feature, scenario: Scenario, config: Config):
-        marks = []
-        for tag in scenario.tag_names:
-            tag_marks = config.hook.pytest_bdd_convert_tag_to_marks(feature=feature, scenario=scenario, tag=tag)
-            if tag_marks is not None:
-                marks.extend(tag_marks)
-        return pytest.param(
-            feature,
-            scenario,
-            id=f"{feature.uri}-{feature.name}-{scenario.name}{scenario.table_rows_breadcrumb}",
-            marks=marks,
-        )
+    def _build_file_uri(features_base_dir: Path, feature_path: Path):
+        if feature_path.is_absolute():
+            try:
+                common_path = Path(commonpath([feature_path, features_base_dir]))
+            except ValueError:
+                rel_feature_path = feature_path
+            else:
+                sub_levels = len(features_base_dir.relative_to(common_path).parts)
+                sub_path = reduce(truediv, [".."] * sub_levels, Path())
+                rel_feature_path = sub_path / feature_path.relative_to(common_path)
+        else:
+            rel_feature_path = feature_path
+
+        return "file:" + str(rel_feature_path.as_posix())
+
+    def resolve(self, config: Union[Config, PytestBDDIdGeneratorHandler]):
+        features_base_dir = self._resolve_features_base_dir(config)
+        already_resolved_feature_paths = set()
+
+        for feature_path in self._gen_feature_paths(features_base_dir=features_base_dir):
+            feature_path_key = str(feature_path)
+            if feature_path_key in already_resolved_feature_paths:
+                break
 
-    @property
-    def features_base_dir(self) -> Path:
-        default_base_dir = dirname(self.caller_module_path)
-        return Path(self.get_from_config_ini("bdd_features_base_dir", default_base_dir))
-
-    def get_from_config_ini(self, key: str, default: str) -> str:
-        """Get value from ini config. Return default if value has not been set.
-
-        Use if the default value is dynamic. Otherwise set default on addini call.
-        """
-        value = self.config.getini(key)
-        if not isinstance(value, str):
-            raise TypeError(f"Expected a string for configuration option {value!r}, got a {type(value)} instead")
-        return value if value != "" else default
-
-    def build_bound_locator_test_function(self, locator):
-        @pytest.mark.pytest_bdd_scenario
-        @pytest.mark.usefixtures("feature", "scenario")
-        def test():
-            ...
+            uri = self._build_file_uri(features_base_dir, feature_path)
+            already_resolved_feature_paths.add(feature_path_key)
+            hook_handler = cast(Config, config).hook
+            encoding = self.encoding
+
+            if self.parser_type is None:
+                if self.mimetype is None:
+                    mimetype = hook_handler.pytest_bdd_get_mimetype(config=config, path=feature_path)
+                else:
+                    mimetype = self.mimetype
 
-        test.__name__ = next(iter(test_names))
+                parser_type = hook_handler.pytest_bdd_get_parser(
+                    config=config,
+                    mimetype=mimetype,
+                )
+            else:
+                parser_type = self.parser_type
 
-        self.add(locator, test)
+            if parser_type is None:
+                break
 
-        return test
+            parser = parser_type(id_generator=cast(PytestBDDIdGeneratorHandler, config).pytest_bdd_id_generator)
 
-    def build_bound_locator_test_decorator(self, locator):
-        def decorator(func):
-            updated_func = pytest.mark.pytest_bdd_scenario(pytest.mark.usefixtures("feature", "scenario")(func))
-            self.update(locator, self.build_bound_locator_test_function(locator), updated_func)
-            return updated_func
+            feature = parser.parse(
+                config,
+                feature_path,
+                uri,
+                *self.parse_args.args,
+                **{**dict(encoding=encoding), **self.parse_args.kwargs},
+            )
 
-        return decorator
+            for pickle in feature.pickles:
+                if self.filter_ is None or self.filter_(config, feature, pickle):  # type: ignore
+                    yield feature, pickle
 
 
 def get_python_name_generator(name: str) -> Iterable[str]:
     """Generate a sequence of suitable python names out of given arbitrary string name."""
     python_name = make_python_name(name)
     suffix = ""
     index = 0
@@ -235,115 +258,115 @@
         index += 1
         suffix = f"{index}"
 
 
 test_names = get_python_name_generator("")
 
 
+class FeaturePathType(Enum):
+    PATH = "path"
+    URL = "url"
+    UNDEFINED = "undefined"
+
+
 def scenario(
-    feature_name: Path | str = Path(),
-    scenario_name: str | None = None,
+    feature_name: Optional[Union[Path, str]] = None,
+    scenario_name: Optional[str] = None,
     encoding: str = "utf-8",
-    features_base_dir: Path | str | None = None,
+    features_base_dir: Optional[Union[Path, str]] = None,
+    features_base_url=None,
+    features_path_type: Optional[Union[FeaturePathType, str]] = None,
+    features_mimetype: Optional[Mimetype] = None,
     return_test_decorator=True,
-    parser: ParserProtocol | None = None,
+    parser_type: Optional[Type[ParserProtocol]] = None,
     parse_args=Args((), {}),
-    _caller_module_locals=None,
-    _caller_module_path=None,
+    locators=(),
 ):
     """
     Scenario decorator.
 
     :param feature_name: Feature file name. Absolute or relative to the configured feature base path.
     :param scenario_name: Scenario name.
     :param encoding: Feature file encoding.
     :param features_base_dir: Feature base directory from where features will be searched
+    :param features_base_url: Feature base url from where features will be loaded
+    :param features_path_type: If feature path is not absolute helps to select if filepath or url will be used
+    :param features_mimetype: Helps to select appropriate parser if non-standard file extension is used
     :param return_test_decorator; Return test decorator or generated test
-    :param parser: Parser used to parse feature-like file
+    :param parser_type: Parser used to parse feature-like file
     :param parse_args: args consumed by parser during parsing
+    :param locators: Feature locators to load Features; Could be custom
     """
-    return _scenarios(
-        feature_paths=[feature_name],
-        scenario_filter_or_scenario_name=scenario_name,
+    return scenarios(
+        *([feature_name] if feature_name is not None else []),
+        filter_=scenario_name,
         encoding=encoding,
         features_base_dir=features_base_dir,
+        features_base_url=features_base_url,
+        features_path_type=features_path_type,
+        features_mimetype=features_mimetype,
         return_test_decorator=return_test_decorator,
-        _caller_module_locals=_caller_module_locals or get_caller_module_locals(stacklevel=2),
-        _caller_module_path=_caller_module_path or get_caller_module_path(stacklevel=2),
-        parser=parser,
+        locators=locators,
+        parser_type=parser_type,
         parse_args=parse_args,
     )
 
 
 def scenarios(
-    *feature_paths: Path | str,
-    encoding: str = "utf-8",
-    features_base_dir: Path | str | None = None,
+    *feature_paths: Union[Path, str],
+    filter_: Optional[Union[str, Callable]] = None,
     return_test_decorator=False,
-    parser: ParserProtocol | None = None,
+    encoding: str = "utf-8",
+    features_base_dir: Optional[Union[Path, str]] = None,
+    features_base_url: Optional[str] = None,
+    features_path_type: Optional[Union[FeaturePathType, str]] = None,
+    features_mimetype: Optional[Mimetype] = None,
+    parser_type: Optional[Type[ParserProtocol]] = None,
     parse_args=Args((), {}),
-    _caller_module_locals=None,
-    _caller_module_path=None,
+    locators=(),
 ):
     """
-    Scenario decorator.
+    Function to bind feature files to pytest runtime
 
     :param feature_paths: Features file names. Absolute or relative to the configured feature base path.
+    :param filter_: Callable to filter scenarios
     :param encoding: Feature file encoding.
     :param features_base_dir: Feature base directory from where features will be searched
+    :param features_base_url: Feature base url from where features will be loaded
+    :param features_path_type: If feature path is not absolute helps to select if filepath or url will be used
+    :param features_mimetype: Helps to select appropriate parser if non-standard file extension is used
+    :param return_test_decorator; Return test decorator or generated test
+    :param parser_type: Parser used to parse feature-like file
+    :param parser_type: Parser used to parse feature-like file
+    :param parse_args: args consumed by parser during parsing
     :param return_test_decorator; Return test decorator or generated test
+    :param locators: Feature locators to load Features; Could be custom
     """
-    return _scenarios(
-        feature_paths=feature_paths,
-        scenario_filter_or_scenario_name=None,
-        encoding=encoding,
-        features_base_dir=features_base_dir,
-        return_test_decorator=return_test_decorator,
-        parser=parser,
-        parse_args=parse_args,
-        _caller_module_locals=_caller_module_locals or get_caller_module_locals(stacklevel=2),
-        _caller_module_path=_caller_module_path or get_caller_module_path(stacklevel=2),
+
+    decorator = compose(
+        mark.pytest_bdd_scenario,
+        mark.usefixtures("feature", "scenario"),
+        mark.scenarios(
+            *feature_paths,
+            filter_=filter_,
+            encoding=encoding,
+            features_base_dir=features_base_dir,
+            features_base_url=features_base_url,
+            features_path_type=features_path_type,
+            features_mimetype=features_mimetype,
+            parser_type=parser_type,
+            parse_args=parse_args,
+            locators=locators,
+        ),
     )
 
+    if return_test_decorator:
+        return decorator
+    else:
 
-def _scenarios(
-    feature_paths: Sequence[Path | str],
-    scenario_filter_or_scenario_name: str | Callable | None,
-    return_test_decorator=True,
-    encoding: str = "utf-8",
-    features_base_dir: Path | str | None = None,
-    parser: ParserProtocol | None = None,
-    parse_args=Args((), {}),
-    _caller_module_locals=None,
-    _caller_module_path=None,
-):
-    if parser is None:
-        parser = GherkinParser()
-    module_scenario_registry = ModuleScenarioRegistry.get(
-        caller_locals=_caller_module_locals,
-        caller_module_path=_caller_module_path,
-    )
+        @decorator
+        def test():
+            ...
 
-    scenario_filter_kwarg = {}
-    if isinstance(scenario_filter_or_scenario_name, str):
-        scenario_filter_kwarg = {
-            "scenario_filter": lambda feature, scenario: scenario.name == scenario_filter_or_scenario_name
-        }
-    if callable(scenario_filter_or_scenario_name):
-        scenario_filter_kwarg = {"scenario_filter": scenario_filter_or_scenario_name}
-
-    scenario_locator = FileScenarioLocator(  # type: ignore[call-arg]
-        feature_paths=feature_paths,
-        **scenario_filter_kwarg,
-        encoding=encoding,
-        features_base_dir=(
-            features_base_dir if features_base_dir is not None else lambda: module_scenario_registry.features_base_dir
-        ),  # known only after start of pytest runtime
-        parser=parser,
-        parse_args=parse_args,
-    )
+        test.__name__ = next(iter(test_names))
 
-    return (
-        module_scenario_registry.build_bound_locator_test_decorator
-        if return_test_decorator
-        else module_scenario_registry.build_bound_locator_test_function
-    )(scenario_locator)
+        return test
```

### Comparing `pytest-bdd-ng-1.2.3/pytest_bdd/steps.py` & `pytest-bdd-ng-2.0.0/src/pytest_bdd/steps.py`

 * *Files 14% similar despite different names*

```diff
@@ -30,31 +30,38 @@
 
 
 @given("I have a beautiful article")
 def given_beautiful_article(article):
     pass
 
 """
-from __future__ import annotations
-
+import os
 import warnings
 from contextlib import suppress
-from typing import Any, Callable, Iterable, Iterator, Sequence, cast
+from inspect import getfile, getsourcelines
+from typing import Any, Callable, Dict, Iterable, Iterator, Optional, Sequence, Set, Union, cast
 from uuid import uuid4
 from warnings import warn
 
 import pytest
 from attr import Factory, attrib, attrs
 from ordered_set import OrderedSet
 
-from pytest_bdd.const import StepType
-from pytest_bdd.model import Feature, Scenario, Step
-from pytest_bdd.parsers import StepParser, get_parser
-from pytest_bdd.typing.pytest import Config, Parser, TypeAlias
-from pytest_bdd.utils import convert_str_to_python_name, get_caller_module_locals, setdefaultattr
+from pytest_bdd.compatibility.pytest import Config, Parser, TypeAlias, get_config_root_path
+from pytest_bdd.model import Feature, StepType
+from pytest_bdd.model.messages import Location, Pickle
+from pytest_bdd.model.messages import PickleStep as Step
+from pytest_bdd.model.messages import SourceReference, StepDefinition, StepDefinitionPattern
+from pytest_bdd.parsers import StepParser
+from pytest_bdd.utils import (
+    PytestBDDIdGeneratorHandler,
+    convert_str_to_python_name,
+    get_caller_module_locals,
+    setdefaultattr,
+)
 from pytest_bdd.warning_types import PytestBDDStepDefinitionWarning
 
 
 def add_options(parser: Parser):
     """Add pytest-bdd options."""
     group = parser.getgroup("bdd", "Steps")
     group.addoption(
@@ -70,151 +77,163 @@
         type="bool",
         help="Allow use different keywords with same step definition",
     )
 
 
 def given(
     parserlike: Any,
-    converters: dict[str, Callable] | None = None,
-    target_fixture: str | None = None,
-    target_fixtures: list[str] = None,
-    params_fixtures_mapping: set[str] | dict[str, str] | Any = True,
-    param_defaults: dict | None = None,
-    liberal: bool | None = None,
+    anonymous_group_names: Optional[Iterable[str]] = None,
+    converters: Optional[Dict[str, Callable]] = None,
+    target_fixture: Optional[str] = None,
+    target_fixtures: Optional[Sequence[str]] = None,
+    params_fixtures_mapping: Union[Set[str], Dict[str, str], Any] = True,
+    param_defaults: Optional[dict] = None,
+    liberal: Optional[bool] = None,
     stacklevel=1,
 ) -> Callable:
     """Given step decorator.
 
     :param parserlike: StepHandler name or a parser object.
+    :param anonymous_group_names: Grant names for anonymous groups of parserlike
     :param converters: Optional `dict` of the argument or parameter converters in form
                        {<param_name>: <converter function>}.
     :param target_fixture: Target fixture name to replace by steps definition function.
     :param target_fixtures: Target fixture names to be replaced by steps definition function.
     :param params_fixtures_mapping: StepHandler parameters would be injected as fixtures
     :param param_defaults: Default parameters for step definition
     :param liberal: Could step definition be used with other keywords
     :param stacklevel: Stack level to find the caller frame. This is used when injecting the step definition fixture.
 
 
     :return: Decorator function for the step.
     """
     return StepHandler.decorator_builder(
-        StepType.CONTEXT,
+        StepType.context,
         parserlike,
+        anonymous_group_names=anonymous_group_names,
         converters=converters,
         target_fixture=target_fixture,
         target_fixtures=target_fixtures,
         params_fixtures_mapping=params_fixtures_mapping,
         param_defaults=param_defaults,
         liberal=liberal,
         stacklevel=stacklevel + 1,
     )
 
 
 def when(
     parserlike: Any,
-    converters: dict[str, Callable] | None = None,
-    target_fixture: str | None = None,
-    target_fixtures: list[str] = None,
-    params_fixtures_mapping: set[str] | dict[str, str] | Any = True,
-    param_defaults: dict | None = None,
-    liberal: bool | None = None,
+    anonymous_group_names: Optional[Iterable[str]] = None,
+    converters: Optional[Dict[str, Callable]] = None,
+    target_fixture: Optional[str] = None,
+    target_fixtures: Optional[Sequence[str]] = None,
+    params_fixtures_mapping: Union[Set[str], Dict[str, str], Any] = True,
+    param_defaults: Optional[dict] = None,
+    liberal: Optional[bool] = None,
     stacklevel=1,
 ) -> Callable:
     """When step decorator.
 
     :param parserlike: StepHandler name or a parser object.
+    :param anonymous_group_names: Grant names for anonymous groups of parserlike
     :param converters: Optional `dict` of the argument or parameter converters in form
                        {<param_name>: <converter function>}.
     :param target_fixture: Target fixture name to replace by steps definition function.
     :param target_fixtures: Target fixture names to be replaced by steps definition function.
     :param params_fixtures_mapping: StepHandler parameters would be injected as fixtures
     :param param_defaults: Default parameters for step definition
     :param liberal: Could step definition be used with other keywords
     :param stacklevel: Stack level to find the caller frame. This is used when injecting the step definition fixture.
 
     :return: Decorator function for the step.
     """
     return StepHandler.decorator_builder(
-        StepType.ACTION,
+        StepType.action,
         parserlike,
+        anonymous_group_names=anonymous_group_names,
         converters=converters,
         target_fixture=target_fixture,
         target_fixtures=target_fixtures,
         params_fixtures_mapping=params_fixtures_mapping,
         param_defaults=param_defaults,
         liberal=liberal,
         stacklevel=stacklevel + 1,
     )
 
 
 def then(
     parserlike: Any,
-    converters: dict[str, Callable] | None = None,
-    target_fixture: str | None = None,
-    target_fixtures: list[str] = None,
-    params_fixtures_mapping: set[str] | dict[str, str] | Any = True,
-    param_defaults: dict | None = None,
-    liberal: bool | None = None,
+    anonymous_group_names: Optional[Iterable[str]] = None,
+    converters: Optional[Dict[str, Callable]] = None,
+    target_fixture: Optional[str] = None,
+    target_fixtures: Optional[Sequence[str]] = None,
+    params_fixtures_mapping: Union[Set[str], Dict[str, str], Any] = True,
+    param_defaults: Optional[dict] = None,
+    liberal: Optional[bool] = None,
     stacklevel=1,
 ) -> Callable:
     """Then step decorator.
 
     :param parserlike: StepHandler name or a parser object.
+    :param anonymous_group_names: Grant names for anonymous groups of parserlike
     :param converters: Optional `dict` of the argument or parameter converters in form
                        {<param_name>: <converter function>}.
     :param target_fixture: Target fixture name to replace by steps definition function.
     :param target_fixtures: Target fixture names to be replaced by steps definition function.
     :param params_fixtures_mapping: StepHandler parameters would be injected as fixtures
     :param param_defaults: Default parameters for step definition
     :param liberal: Could step definition be used with other keywords
     :param stacklevel: Stack level to find the caller frame. This is used when injecting the step definition fixture.
 
     :return: Decorator function for the step.
     """
     return StepHandler.decorator_builder(
-        StepType.OUTCOME,
+        StepType.outcome,
         parserlike,
+        anonymous_group_names=anonymous_group_names,
         converters=converters,
         target_fixture=target_fixture,
         target_fixtures=target_fixtures,
         params_fixtures_mapping=params_fixtures_mapping,
         param_defaults=param_defaults,
         liberal=liberal,
         stacklevel=stacklevel + 1,
     )
 
 
 def step(
     parserlike: Any,
-    converters: dict[str, Callable] | None = None,
-    target_fixture: str | None = None,
-    target_fixtures: list[str] = None,
-    params_fixtures_mapping: set[str] | dict[str, str] | Any = True,
-    param_defaults: dict | None = None,
-    liberal: bool | None = None,
+    anonymous_group_names: Optional[Iterable[str]] = None,
+    converters: Optional[Dict[str, Callable]] = None,
+    target_fixture: Optional[str] = None,
+    target_fixtures: Optional[Sequence[str]] = None,
+    params_fixtures_mapping: Union[Set[str], Dict[str, str], Any] = True,
+    param_defaults: Optional[dict] = None,
+    liberal: Optional[bool] = None,
     stacklevel=1,
 ):
     """Liberal step decorator which could be used with any keyword.
 
     :param parserlike: StepHandler name or a parser object.
+    :param anonymous_group_names: Grant names for anonymous groups of parserlike
     :param converters: Optional `dict` of the argument or parameter converters in form
                        {<param_name>: <converter function>}.
     :param target_fixture: Target fixture name to replace by steps definition function.
     :param target_fixtures: Target fixture names to be replaced by steps definition function.
     :param params_fixtures_mapping: StepHandler parameters would be injected as fixtures
     :param param_defaults: Default parameters for step definition
     :param liberal: Could step definition be used with other keywords
     :param stacklevel: Stack level to find the caller frame. This is used when injecting the step definition fixture.
 
     :return: Decorator function for the step.
     """
     return StepHandler.decorator_builder(
-        StepType.UNSPECIFIED if liberal else StepType.UNKNOWN,
+        StepType.unknown,
         parserlike,
+        anonymous_group_names=anonymous_group_names,
         converters=converters,
         target_fixture=target_fixture,
         target_fixtures=target_fixtures,
         params_fixtures_mapping=params_fixtures_mapping,
         param_defaults=param_defaults,
         liberal=liberal,
         stacklevel=stacklevel + 1,
@@ -224,65 +243,63 @@
 class StepHandler:
     Model: TypeAlias = "Step"
 
     @attrs
     class Matcher:
         config: Config = attrib()
         feature: Feature = attrib(init=False)
-        pickle: Scenario = attrib(init=False)
+        pickle: Pickle = attrib(init=False)
         step: Step = attrib(init=False)
-        previous_step: Step | None = attrib(init=False)
-        step_registry: StepHandler.Registry = attrib(init=False)
+        previous_step: Optional[Step] = attrib(init=False)
+        step_registry: "StepHandler.Registry" = attrib(init=False)
         step_type_context = attrib(default=None)
 
         class MatchNotFoundError(RuntimeError):
             pass
 
         def __call__(
             self,
             feature: Feature,
-            pickle: Scenario,
+            pickle: Pickle,
             step: Step,
-            previous_step: Step | None,
-            step_registry: StepHandler.Registry,
-        ) -> StepHandler.Definition:
+            previous_step: Optional[Step],
+            step_registry: "StepHandler.Registry",
+        ) -> "StepHandler.Definition":
             self.feature = feature
             self.pickle = pickle
             self.step = step
             self.previous_step = previous_step
             self.step_registry = step_registry
 
             self.step_type_context = (
                 self.step_type_context
-                if self.step.type in (StepType.CONJUNCTION, StepType.UNKNOWN) and self.step_type_context is not None
+                if self.step.type is StepType.unknown and self.step_type_context is not None
                 else self.step.type
             )
-            if self.step_type_context == StepType.CONJUNCTION:
-                self.step_type_context = StepType.UNKNOWN
 
             step_definitions = list(
                 self.find_step_definition_matches(
                     self.step_registry, (self.strict_matcher, self.unspecified_matcher, self.liberal_matcher)
                 )
             )
 
             if len(step_definitions) > 0:
                 if len(step_definitions) > 1:
                     warn(PytestBDDStepDefinitionWarning(f"Alternative step definitions are found: {step_definitions}"))
                 return step_definitions[0]
-            raise self.MatchNotFoundError
+            raise self.MatchNotFoundError(self.step.text)
 
         def strict_matcher(self, step_definition):
             return step_definition.type_ == self.step_type_context and step_definition.parser.is_matching(
                 self.step.text
             )
 
         def unspecified_matcher(self, step_definition):
             return (
-                self.step_type_context == StepType.UNSPECIFIED or step_definition.type_ == StepType.UNSPECIFIED
+                self.step_type_context == StepType.unknown or step_definition.type_ == StepType.unknown
             ) and step_definition.parser.is_matching(self.step.text)
 
         def liberal_matcher(self, step_definition):
             if step_definition.liberal is None:
                 if self.config.option.liberal_steps is not None:
                     is_step_definition_liberal = self.config.option.liberal_steps
                 else:
@@ -297,51 +314,76 @@
                     step_definition.type_ != self.step_type_context,
                     step_definition.parser.is_matching(self.step.text),
                 )
             )
 
         @staticmethod
         def find_step_definition_matches(
-            registry: StepHandler.Registry | None, matchers: Sequence[Callable[[StepHandler.Definition], bool]]
-        ) -> Iterable[StepHandler.Definition]:
+            registry: Optional["StepHandler.Registry"], matchers: Sequence[Callable[["StepHandler.Definition"], bool]]
+        ) -> Iterable["StepHandler.Definition"]:
             if registry:
                 found_matches = False
                 for matcher in matchers:
                     for step_definition in registry:
                         if matcher(step_definition):
                             found_matches = True
                             yield step_definition
                     if found_matches:
                         break
                 if not found_matches:
                     with suppress(AttributeError):
                         yield from StepHandler.Matcher.find_step_definition_matches(registry.parent, matchers)
 
-    @attrs(auto_attribs=True, eq=False)
+    @attrs(eq=False)
     class Definition:
-        func: Callable
-        type_: str | None
-        parser: StepParser
-        converters: dict[str, Callable]
-        params_fixtures_mapping: set[str] | dict[str, str] | Any
-        param_defaults: dict
-        target_fixtures: list[str]
-        liberal: Any | None
+        func: Callable = attrib()
+        type_: Optional[Union[str, StepType]] = attrib()
+        parser: StepParser = attrib()
+        anonymous_group_names: Optional[Iterable[str]] = attrib()
+        converters: Dict[str, Callable] = attrib()
+        params_fixtures_mapping: Union[Set[str], Dict[str, str], Any] = attrib()
+        param_defaults: dict = attrib()
+        target_fixtures: Sequence[str] = attrib()
+        liberal: Optional[Any] = attrib()
+
+        id = attrib(init=False)
+        __cached_message = attrib(init=False)
+
+        def as_message(self, config: Union[Config, PytestBDDIdGeneratorHandler]):
+            try:
+                message = self.__cached_message
+            except AttributeError:
+                self.id = cast(PytestBDDIdGeneratorHandler, config).pytest_bdd_id_generator.get_next_id()
+                self.__cached_message = StepDefinition(
+                    id=self.id,
+                    pattern=StepDefinitionPattern(source=str(self.parser), type=self.parser.type),
+                    source_reference=SourceReference(
+                        uri=os.path.relpath(
+                            getfile(self.func),
+                            str(get_config_root_path(cast(Config, config))),
+                        ),
+                        location=Location(line=getsourcelines(self.func)[1]),
+                    ),
+                )
+                message = self.__cached_message
+            return message
 
         def get_parameters(self, step: Step):
-            parsed_arguments = self.parser.parse_arguments(step.name) or {}
+            parsed_arguments = (
+                self.parser.parse_arguments(step.text, anonymous_group_names=self.anonymous_group_names) or {}
+            )
             return {
                 **self.param_defaults,
                 **{arg: self.converters.get(arg, lambda _: _)(value) for arg, value in parsed_arguments.items()},
             }
 
     @attrs
     class Registry:
-        registry: set[StepHandler.Definition] = attrib(default=Factory(set))
-        parent: StepHandler.Registry = attrib(default=None, init=False)
+        registry: Set["StepHandler.Definition"] = attrib(default=Factory(set))
+        parent: "StepHandler.Registry" = attrib(default=None, init=False)
 
         @classmethod
         def inject_registry_fixture_and_register_steps(cls, obj):
             steps = [
                 step_candidate
                 for step_candidate in obj.__dict__.values()
                 if hasattr(step_candidate, "__pytest_bdd_step_definitions__")
@@ -364,33 +406,35 @@
             def step_registry(step_registry):
                 self.parent = step_registry
                 return self
 
             step_registry.__registry__ = self
             return step_registry
 
-        def __iter__(self) -> Iterator[StepHandler.Definition]:
+        def __iter__(self) -> Iterator["StepHandler.Definition"]:
             return iter(self.registry)
 
     @staticmethod
     def decorator_builder(
-        step_type: str | None,
+        step_type: Optional[Union[str, StepType]],
         step_parserlike: Any,
-        converters: dict[str, Callable] | None = None,
-        target_fixture: str | None = None,
-        target_fixtures: list[str] | None = None,
-        params_fixtures_mapping: set[str] | dict[str, str] | Any = True,
-        param_defaults: dict | None = None,
-        liberal: Any | None = None,
+        anonymous_group_names: Optional[Iterable[str]] = None,
+        converters: Optional[Dict[str, Callable]] = None,
+        target_fixture: Optional[str] = None,
+        target_fixtures: Optional[Sequence[str]] = None,
+        params_fixtures_mapping: Union[Set[str], Dict[str, str], Any] = True,
+        param_defaults: Optional[dict] = None,
+        liberal: Optional[Any] = None,
         stacklevel=2,
     ) -> Callable:
         """StepHandler decorator for the type and the name.
 
         :param step_type: StepHandler type (CONTEXT, ACTION or OUTCOME).
         :param step_parserlike: StepHandler name as in the feature file.
+        :param anonymous_group_names: Grant names for anonymous groups of parserlike
         :param converters: Optional step arguments converters mapping
         :param target_fixture: Optional fixture name to replace by step definition
         :param target_fixtures: Target fixture names to be replaced by steps definition function.
         :param params_fixtures_mapping: StepHandler parameters would be injected as fixtures
         :param param_defaults: Default parameters for step definition
         :param liberal: Could step definition be used with other keywords
         :param stacklevel: Stack level to find the caller frame. This is used when injecting the step definition fixture
@@ -417,15 +461,16 @@
 
             :param function step_func: StepHandler definition function
             """
 
             step_definition = StepHandler.Definition(  # type: ignore[call-arg]
                 func=step_func,
                 type_=step_type,
-                parser=get_parser(step_parserlike),
+                parser=StepParser.build(step_parserlike),
+                anonymous_group_names=anonymous_group_names,
                 converters=cast(dict, converters),
                 params_fixtures_mapping=params_fixtures_mapping,
                 param_defaults=cast(dict, param_defaults),
                 target_fixtures=cast(list, target_fixtures),
                 liberal=liberal,
             )
```

### Comparing `pytest-bdd-ng-1.2.3/pytest_bdd/struct_bdd/ast_builder.py` & `pytest-bdd-ng-2.0.0/src/pytest_bdd/struct_bdd/model_builder.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,176 +1,240 @@
-from __future__ import annotations
-
-from itertools import count
+from itertools import filterfalse
+from json import loads as json_loads
 from operator import attrgetter
-from typing import Any
+from typing import Any, Union, cast
 
-from attr import Factory, attrib, attrs
+from attr import attrib, attrs
+from gherkin.pickles.compiler import Compiler
 
-import pytest_bdd.ast as ast
-from pytest_bdd.struct_bdd.model import Join, Step, Table
+from pytest_bdd.model.gherkin_document import Feature as GherkinDocumentFeature
+from pytest_bdd.model.messages import (
+    DataTable,
+    DocString,
+    Examples,
+    Feature,
+    FeatureChild,
+    GherkinDocument,
+    KeywordType,
+    Location,
+    Scenario,
+    Step,
+    TableCell,
+    TableRow,
+    Tag,
+    Type,
+)
+from pytest_bdd.struct_bdd.model import Join as StructJoin
+from pytest_bdd.struct_bdd.model import StepPrototype as StructStep
+from pytest_bdd.struct_bdd.model import Table as StructTable
 
 
 @attrs
 class _ASTBuilder:
     model: Any
-    id_generator = attrib(default=Factory(lambda: map(str, count())), kw_only=True)
 
     def build(self, *args, **kwargs):  # pragma: no cover
         raise NotImplementedError
 
 
 @attrs
-class DocumentASTBuilder(_ASTBuilder):
-    model: Step = attrib()
+class GherkinDocumentBuilder(_ASTBuilder):
+    model: StructStep = attrib()
+
+    def build(self, id_generator):
+        return GherkinDocument(
+            comments=[], uri=None, feature=StepToFeatureASTBuilder(self.model).build(id_generator=id_generator)
+        )
 
-    def build(self):
-        return ast.AST(
-            gherkin_document=ast.GherkinDocument(comments=[], uri=None).setattrs(
-                feature=StepToFeatureASTBuilder(self.model, id_generator=self.id_generator).build()
-            )
+    def build_feature(self, filename, uri, id_generator):
+        gherkin_document = self.build(id_generator=id_generator)
+        gherkin_document.uri = uri
+
+        gherkin_document_serialized = gherkin_document.json(by_alias=True, exclude_none=True)
+
+        scenarios_data = Compiler().compile(json_loads(gherkin_document_serialized))
+        pickles = GherkinDocumentFeature.load_pickles(scenarios_data)
+
+        feature = GherkinDocumentFeature(  # type: ignore[call-arg]
+            gherkin_document=gherkin_document,
+            uri=uri,
+            pickles=pickles,
+            filename=filename,
         )
 
+        feature.fill_registry()
+
+        return feature
+
 
 @attrs
 class StepToFeatureASTBuilder(_ASTBuilder):
-    model: Step = attrib()
+    model: StructStep = attrib()
 
-    def build(self):
-        return ast.Feature(
-            children=self._build_children(),
+    def build(self, id_generator):
+        return Feature(
+            children=self._build_children(id_generator=id_generator),
             description=self.model.description or "",
             language="EN",
-            location=ast.Location(column=0, line=0),
+            location=Location(column=0, line=0),
             tags=[],
             name=self.model.name or "",
-        ).setattrs(keyword="Feature")
+            keyword="Feature",
+        )
 
-    def _build_children(self):
+    def _build_children(self, id_generator):
         def _():
             for route in self.model.routes:
                 if route.steps:
-                    yield ast.NodeContainerChild().setattrs(
-                        scenario=ast.Scenario(
+
+                    def steps_gen(steps):
+                        previous_step_keyword_type = None
+                        for step in steps:
+                            step_keyword_type = (
+                                previous_step_keyword_type
+                                if step.keyword_type is KeywordType.conjunction
+                                else step.keyword_type
+                            )
+                            yield Step(
+                                id=next(id_generator),
+                                keyword=step.type if isinstance(step.type, str) else cast(Type, step.type).value,
+                                location=Location(column=0, line=0),
+                                text=step.action,
+                                keyword_type=step_keyword_type.value,
+                                **(
+                                    (
+                                        lambda rows: dict(
+                                            data_table=DataTable(
+                                                rows=rows,
+                                                location=Location(column=0, line=0),  # type: ignore[call-arg]
+                                            )  # type: ignore[call-arg]
+                                        )
+                                        if rows
+                                        else {}
+                                    )(
+                                        [
+                                            *filterfalse(
+                                                lambda row: row is None,
+                                                map(
+                                                    lambda row_values: (
+                                                        (
+                                                            lambda cells: TableRow(
+                                                                id=next(id_generator),
+                                                                location=Location(column=0, line=0),  # type: ignore[call-arg]
+                                                                cells=cells,
+                                                            )  # type: ignore[call-arg]
+                                                            if cells
+                                                            else None
+                                                        )(
+                                                            [
+                                                                *map(
+                                                                    lambda parameter: TableCell(
+                                                                        location=Location(column=0, line=0),
+                                                                        value=parameter,
+                                                                    ),
+                                                                    row_values,
+                                                                )
+                                                            ]
+                                                        )
+                                                    ),
+                                                    StructJoin(tables=step.data).rowed_values,
+                                                ),
+                                            )
+                                        ]
+                                    )
+                                ),
+                                **(
+                                    dict(
+                                        doc_string=DocString(
+                                            content=step.description,
+                                            delimiter="\n",
+                                            location=Location(column=0, line=0),
+                                        )
+                                    )
+                                    if step.description
+                                    else dict()
+                                ),
+                            )
+                            previous_step_keyword_type = step_keyword_type
+
+                    steps = [*steps_gen(filter(lambda step: step.action is not None, route.steps))]
+
+                    yield FeatureChild(
+                        scenario=Scenario(
                             description=route.steps[0].description or "",
-                            examples=[ExampleASTBuilder(route.example_table, id_generator=self.id_generator).build()]
+                            examples=[ExampleASTBuilder(route.example_table).build(id_generator=id_generator)]
                             if route.example_table.values
                             else [],
-                            identifier=next(self.id_generator),
+                            id=next(id_generator),
                             keyword="Scenario",
-                            location=ast.Location(column=0, line=0),
+                            location=Location(column=0, line=0),
                             name=next(filter(bool, map(attrgetter("name"), reversed(route.steps))), ""),
                             tags=[
                                 *map(
-                                    lambda tag_name: ast.Tag(
-                                        identifier=next(self.id_generator),
-                                        location=ast.Location(column=0, line=0),
+                                    lambda tag_name: Tag(
+                                        id=next(id_generator),
+                                        location=Location(column=0, line=0),
                                         name=tag_name,
                                     ),
                                     route.tags,
                                 )
                             ],
-                            steps=[
-                                *map(
-                                    lambda step: ast.Step(
-                                        identifier=next(self.id_generator),
-                                        keyword=step.type,
-                                        location=ast.Location(column=0, line=0),
-                                        text=step.action,
-                                        keyword_type=step.keyword_type,
-                                    ).setattrs(
-                                        data_table=ast.DataTable(
-                                            rows=[
-                                                *map(
-                                                    lambda row_values: ast.TableRow(
-                                                        identifier=next(self.id_generator),
-                                                        location=ast.Location(column=0, line=0),
-                                                        cells=[
-                                                            *map(
-                                                                lambda parameter: ast.TableCell(
-                                                                    location=ast.Location(column=0, line=0),
-                                                                    value=parameter,
-                                                                ),
-                                                                row_values,
-                                                            )
-                                                        ],
-                                                    ),
-                                                    Join(tables=step.data).rowed_values,
-                                                )
-                                            ],
-                                            location=ast.Location(column=0, line=0),
-                                        ),
-                                        **(
-                                            {
-                                                "doc_string": ast.DocString(
-                                                    content=step.description,
-                                                    delimiter="\n",
-                                                    location=ast.Location(column=0, line=0),
-                                                )
-                                            }
-                                            if step.description
-                                            else {}
-                                        ),
-                                    ),
-                                    filter(lambda step: step.action is not None, route.steps),
-                                )
-                            ],
+                            steps=steps,
                         )
                     )
 
         return list(_())
 
 
 @attrs
 class ExampleASTBuilder(_ASTBuilder):
-    model: Table | Join = attrib()
+    model: Union[StructJoin, StructTable] = attrib()
 
-    def build(self):
-        return ast.Example(
+    def build(self, id_generator):
+        return Examples(
             description=self.model.description,
-            identifier=next(self.id_generator),
+            id=next(id_generator),
             keyword="Examples",
-            location=ast.Location(column=0, line=0),
+            location=Location(column=0, line=0),
             name=self.model.name,
             table_body=[
                 *map(
-                    lambda row_values: ast.TableRow(
-                        identifier=next(self.id_generator),
-                        location=ast.Location(column=0, line=0),
+                    lambda row_values: TableRow(
+                        id=next(id_generator),
+                        location=Location(column=0, line=0),
                         cells=[
                             *map(
-                                lambda parameter: ast.TableCell(
-                                    location=ast.Location(column=0, line=0),
+                                lambda parameter: TableCell(
+                                    location=Location(column=0, line=0),
                                     value=parameter,
                                 ),
                                 row_values,
                             )
                         ],
                     ),
                     self.model.rowed_values,
                 )
             ],
             tags=[
                 *map(
-                    lambda tag_name: ast.Tag(
-                        identifier=next(self.id_generator),
-                        location=ast.Location(column=0, line=0),
+                    lambda tag_name: Tag(
+                        id=next(id_generator),
+                        location=Location(column=0, line=0),
                         name=tag_name,
                     ),
                     self.model.tags,
                 )
             ],
-        ).setattrs(
-            table_header=ast.ExampleTableHeader(
-                identifier=next(self.id_generator),
-                location=ast.Location(column=0, line=0),
+            table_header=TableRow(
+                id=next(id_generator),
+                location=Location(column=0, line=0),
                 cells=[
                     *map(
-                        lambda parameter: ast.TableCell(
-                            location=ast.Location(column=0, line=0),
+                        lambda parameter: TableCell(
+                            location=Location(column=0, line=0),
                             value=parameter,
                         ),
                         self.model.parameters,
                     )
                 ],
             ),
         )
```

### Comparing `pytest-bdd-ng-1.2.3/pytest_bdd/struct_bdd/parser.py` & `pytest-bdd-ng-2.0.0/src/pytest_bdd/struct_bdd/parser.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,63 +1,67 @@
 from enum import Enum
 from functools import partial
 from operator import methodcaller
 from pathlib import Path
-from typing import cast
+from typing import Union
 
 from attr import attrib, attrs
 
-from pytest_bdd.struct_bdd.model import Step, StepSchema
-from pytest_bdd.typing.parser import ParserProtocol
+from pytest_bdd.compatibility.parser import ParserProtocol
+from pytest_bdd.compatibility.pytest import Config
+from pytest_bdd.struct_bdd.model import Step
+from pytest_bdd.struct_bdd.model_builder import GherkinDocumentBuilder
+from pytest_bdd.utils import PytestBDDIdGeneratorHandler
 
 
 @attrs
 class StructBDDParser(ParserProtocol):
     class KIND(Enum):
         HOCON = "hocon"
         HJSON = "hjson"
         JSON = "json"
         JSON5 = "json5"
         TOML = "toml"
         YAML = "yaml"
 
+    id_generator = attrib()
     kind = attrib(kw_only=True)
     glob = attrib(kw_only=True)
     loader = attrib(kw_only=True)
 
     @kind.default
     def kind_default(self):
         return self.KIND.YAML.value if getattr(self, "loader", None) is None else None
 
     @glob.default
     def glob_default(self):
-        return methodcaller("rglob", "*" if self.kind is None else f"*.bdd.{self.kind}")
+        return methodcaller("glob", "*" if self.kind is None else f"*.bdd.{self.kind}")
 
     @loader.default
     def loader_default(self):
         return self.build_loader()
 
-    def parse(self, path: Path, uri: str, *args, **kwargs):
+    def parse(self, config: Union[Config, PytestBDDIdGeneratorHandler], path: Path, uri: str, *args, **kwargs):
         encoding = kwargs.pop("encoding", "utf-8")
         mode = kwargs.pop("mode", "r")
         with path.open(mode=mode, encoding=encoding) as feature_file:
             content = feature_file.read()
-
-        return cast(Step, StepSchema().load(self.loader(content, *args, **kwargs))).build_feature(
-            filename=str(path.as_posix()), uri=uri
-        )
+        filename = str(path.as_posix())
+        raw_step = self.loader(content, *args, **kwargs)
+        step = Step.parse_obj(raw_step)
+        return GherkinDocumentBuilder(model=step).build_feature(filename, uri, self.id_generator)  # type: ignore[call-arg]
 
     def build_loader(self):
         if self.kind == self.KIND.YAML.value:
             from yaml import FullLoader
             from yaml import load as load_yaml
 
             return partial(load_yaml, Loader=FullLoader)
         elif self.kind == self.KIND.TOML.value:
-            from tomli import loads as load_toml
+            from pytest_bdd.compatibility.tomllib import loads as load_toml
 
             return load_toml
         elif self.kind == self.KIND.JSON.value:
             from json import loads as load_json
 
             return load_json
         elif self.kind == self.KIND.JSON5.value:
```

### Comparing `pytest-bdd-ng-1.2.3/pytest_bdd/utils.py` & `pytest-bdd-ng-2.0.0/src/pytest_bdd/utils.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,47 +1,63 @@
 """Various utility functions."""
-from __future__ import annotations
-
 import base64
 import pickle
 import re
+import sys
 from collections import defaultdict
-from contextlib import nullcontext, suppress
+from contextlib import contextmanager, nullcontext, suppress
 from enum import Enum
-from functools import partial
+from functools import reduce
 from inspect import getframeinfo, signature
 from itertools import tee
 from operator import attrgetter, getitem, itemgetter
 from sys import _getframe
-from typing import TYPE_CHECKING, Any, Callable, Collection, Mapping, cast
+from typing import (
+    TYPE_CHECKING,
+    Any,
+    Callable,
+    Collection,
+    Dict,
+    Mapping,
+    Optional,
+    Pattern,
+    Sequence,
+    Type,
+    Union,
+    cast,
+)
 
-from attr import Factory, attrib, attrs
-from marshmallow import post_load
+from pytest import raises
 
+from pytest_bdd.compatibility.pytest import FixtureDef, fail
+from pytest_bdd.compatibility.typing import Literal, Protocol, runtime_checkable
 from pytest_bdd.const import ALPHA_REGEX, PYTHON_REPLACE_REGEX
-from pytest_bdd.typing import Literal
-from pytest_bdd.typing.pytest import FixtureDef
 
 if TYPE_CHECKING:  # pragma: no cover
-    from pytest_bdd.typing.pytest import RunResult
+    from pytest_bdd.compatibility.pytest import RunResult
+
+
+@runtime_checkable
+class PytestBDDIdGeneratorHandler(Protocol):
+    pytest_bdd_id_generator: Union["IdGenerator", Any]
 
 
-def get_args(func: Callable) -> list[str]:
+def get_args(func: Callable) -> Sequence[str]:
     """Get a list of argument names for a function.
 
     :param func: The function to inspect.
 
     :return: A list of argument names.
     :rtype: list
     """
     params = signature(func).parameters.values()
     return [param.name for param in params if param.kind == param.POSITIONAL_OR_KEYWORD]
 
 
-def get_caller_module_locals(stacklevel: int = 1) -> dict[str, Any]:
+def get_caller_module_locals(stacklevel: int = 1) -> Dict[str, Any]:
     """Get the caller module locals dictionary.
 
     We use sys._getframe instead of inspect.stack(0) because the latter is way slower, since it iterates over
     all the frames in the stack.
     """
     return _getframe(stacklevel).f_locals
 
@@ -76,39 +92,25 @@
     """Dump objects to stdout so that they can be inspected by the test suite."""
     for obj in objects:
         dump = pickle.dumps(obj, protocol=pickle.HIGHEST_PROTOCOL)
         encoded = base64.b64encode(dump).decode("ascii")
         print(f"{_DUMP_START}{encoded}{_DUMP_END}")
 
 
-def collect_dumped_objects(result: RunResult):
+def collect_dumped_objects(result: "RunResult"):
     """Parse all the objects dumped with `dump_object` from the result.
 
     Note: You must run the result with output to stdout enabled.
     For example, using ``testdir.runpytest("-s")``.
     """
     stdout = result.stdout.str()  # pytest < 6.2, otherwise we could just do str(result.stdout)
     payloads = re.findall(rf"{_DUMP_START}(.*?){_DUMP_END}", stdout)
     return [pickle.loads(base64.b64decode(payload)) for payload in payloads]
 
 
-@attrs
-class SimpleMapping(Mapping):
-    _dict: dict = attrib(default=Factory(dict), kw_only=True)
-
-    def __getitem__(self, item):
-        return self._dict[item]
-
-    def __iter__(self):
-        return iter(self._dict)
-
-    def __len__(self):
-        return len(self._dict)
-
-
 class DefaultMapping(defaultdict):
     Skip = object()
 
     def __init__(self, *args, default_factory=None, warm_up_keys=(), **kwargs):
         super().__init__(default_factory, *args, **kwargs)
         self.warm_up(*warm_up_keys)
 
@@ -131,15 +133,15 @@
     def warm_up(self, *items):
         for item in items:
             with suppress(KeyError):
                 getitem(self, item)
 
     @classmethod
     def instantiate_from_collection_or_bool(
-        cls, bool_or_items: Collection[str] | dict[str, Any] | Any = True, *, warm_up_keys=()
+        cls, bool_or_items: Union[Collection[str], Dict[str, Any], Any] = True, *, warm_up_keys=()
     ):
         if isinstance(bool_or_items, Collection):
             if not isinstance(bool_or_items, Mapping):
                 bool_or_items = zip(*tee(iter(bool_or_items)))
         else:
             bool_or_items = cast(dict, {...: ...} if bool_or_items else {...: DefaultMapping.Skip})
         return cls(bool_or_items, warm_up_keys=warm_up_keys)
@@ -179,45 +181,14 @@
     request._fixturemanager._arg2fixturedefs.setdefault(arg, []).insert(0, fd)
     # inject fixture value in request cache
     request._fixture_defs[arg] = fd
     if add_fixturename:
         request._pyfuncitem._fixtureinfo.names_closure.append(arg)
 
 
-class ModelSchemaPostLoadable:
-    postbuild_attrs: list[str] = []
-
-    @staticmethod
-    def build_from_schema(cls, data, many, **kwargs):
-        return cls.postbuild_attr_builder(cls, data, cls.postbuild_attrs)
-
-    @classmethod
-    def schema_post_loader(cls):
-        return post_load(partial(cls.build_from_schema, cls))
-
-    @staticmethod
-    def postbuild_attr_builder(cls, data, postbuild_args):
-        _data = {**data}
-        empty = object()
-        postbuildable_args = []
-        for argument in postbuild_args:
-            value = _data.pop(argument, empty)
-            if value is not empty:
-                postbuildable_args.append((argument, value))
-        instance = cls(**_data)
-        for argument, value in postbuildable_args:
-            setattr(instance, argument, value)
-        return instance
-
-    def setattrs(self, **kwargs):
-        for key, value in kwargs.items():
-            setattr(self, key, value)
-        return self
-
-
 def _itemgetter(*items):
     def func(obj):
         if len(items) == 0:
             return []
         elif len(items) == 1:
             return [obj[items[0]]]
         else:
@@ -226,14 +197,39 @@
     return func
 
 
 class _NoneException(Exception):
     ...
 
 
+class Empty(Enum):
+    empty = None
+
+
+def getitemdefault(
+    obj, index, default=Empty.empty, default_factory: Optional[Callable] = None, treat_as_empty=Empty.empty
+):
+    if default is not Empty.empty:
+        if default_factory is not None:
+            raise ValueError("Both 'default' and 'default_factory' were specified")
+        else:
+            default_factory = lambda: default
+    try:
+        item = getitem(obj, index)
+    except KeyError:
+        if default_factory is None:
+            raise
+        else:
+            item = default_factory()
+    if item is not treat_as_empty:
+        return item
+    else:
+        raise KeyError(f"{index}")
+
+
 def deepattrgetter(*attrs, **kwargs):
     empty = object()
     default = kwargs.pop("default", empty)
     default_exception_type = AttributeError if default is not empty else _NoneException
     skip_missing = kwargs.pop("skip_missing", False)
     skip_missing_context = suppress(AttributeError) if skip_missing else nullcontext()
     if default is not empty and skip_missing:
@@ -249,26 +245,79 @@
                     yield default
 
         return tuple(_())
 
     return fn
 
 
-class EMPTY(Enum):
-    EMPTY = 1
-
-
-def setdefaultattr(obj, key, value: Literal[EMPTY.EMPTY] | Any = EMPTY.EMPTY, value_factory: None | Callable = None):
-    if value is not EMPTY.EMPTY and value_factory is not None:
+def setdefaultattr(
+    obj, key, value: Union[Literal[Empty.empty], Any] = Empty.empty, value_factory: Optional[Callable] = None
+):
+    if value is not Empty.empty and value_factory is not None:
         raise ValueError("Both 'value' and 'value_factory' were specified")
     with suppress(AttributeError):
         return getattr(obj, key)
     if value_factory is not None:
         value = value_factory()
     setattr(obj, key, value)
     return value
 
 
+def compose(*funcs):
+    return reduce(lambda f, g: lambda *args, **kwargs: f(g(*args, **kwargs)), funcs)
+
+
 def make_python_name(string: str) -> str:
     """Make python attribute name out of a given string."""
     string = re.sub(PYTHON_REPLACE_REGEX, "", string.replace(" ", "_"))
     return re.sub(ALPHA_REGEX, "", string).lower()
+
+
+@runtime_checkable
+class StringableProtocol(Protocol):
+    def __str__(self) -> str:
+        ...  # pragma: no cover
+
+
+def stringify(value: Union[StringableProtocol, str, bytes]) -> str:
+    return str(value, **({"encoding": "utf-8"} if isinstance(value, bytes) else {}))
+
+
+class IdGenerator:
+    def __init__(self):
+        self._id_counter = 0
+
+    def __next__(self):
+        try:
+            return str(self._id_counter)
+        finally:
+            self._id_counter += 1
+
+    get_next_id = __next__
+
+
+@contextmanager
+def doesnt_raise(
+    expected_exception: Union[Type[Exception], Sequence[Type[Exception]]],
+    *,
+    match: Optional[Union[str, Pattern[str]]] = None,
+    suppress_not_matched=True,
+):
+    """
+
+    :param expected_exception: Expected exception/s which don't have to be raised; If it raised - test fails
+    :param match: Message which will be count as failing test. If message is not matched - function passes
+    :param suppress_not_matched: If specified - all non-matched exceptions will be suppressed
+    :return:
+    """
+
+    try:
+        yield
+    except expected_exception:  # type:ignore[misc]
+        ex_type, ex_value, ex_traceback = sys.exc_info()
+        is_matched = True
+        if match is not None:
+            is_matched = bool(re.search(match, f"{ex_value}"))
+        if is_matched:
+            fail(f"{ex_value}")
+        elif not suppress_not_matched:
+            raise
```

### Comparing `pytest-bdd-ng-1.2.3/pytest_bdd/warning_types.py` & `pytest-bdd-ng-2.0.0/src/pytest_bdd/warning_types.py`

 * *Files identical despite different names*

