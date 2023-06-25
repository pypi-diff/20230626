# Comparing `tmp/UpyTest-3.1.2.tar.gz` & `tmp/UpyTest-3.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "UpyTest-3.1.2.tar", last modified: Sun Jun 25 22:08:24 2023, max compression
+gzip compressed data, was "UpyTest-3.1.3.tar", last modified: Sun Jun 25 22:27:11 2023, max compression
```

## Comparing `UpyTest-3.1.2.tar` & `UpyTest-3.1.3.tar`

### file list

```diff
@@ -1,72 +1,72 @@
-drwxrwxr-x   0 idtaleb   (1000) idtaleb   (1000)        0 2023-06-25 22:08:24.033028 UpyTest-3.1.2/
--rw-rw-r--   0 idtaleb   (1000) idtaleb   (1000)      694 2023-06-25 22:08:24.029028 UpyTest-3.1.2/PKG-INFO
-drwxrwxr-x   0 idtaleb   (1000) idtaleb   (1000)        0 2023-06-25 22:08:24.021028 UpyTest-3.1.2/UpyTest.egg-info/
--rw-rw-r--   0 idtaleb   (1000) idtaleb   (1000)      694 2023-06-25 22:08:23.000000 UpyTest-3.1.2/UpyTest.egg-info/PKG-INFO
--rw-rw-r--   0 idtaleb   (1000) idtaleb   (1000)     2351 2023-06-25 22:08:23.000000 UpyTest-3.1.2/UpyTest.egg-info/SOURCES.txt
--rw-rw-r--   0 idtaleb   (1000) idtaleb   (1000)        1 2023-06-25 22:08:23.000000 UpyTest-3.1.2/UpyTest.egg-info/dependency_links.txt
--rw-rw-r--   0 idtaleb   (1000) idtaleb   (1000)       14 2023-06-25 22:08:23.000000 UpyTest-3.1.2/UpyTest.egg-info/requires.txt
--rw-rw-r--   0 idtaleb   (1000) idtaleb   (1000)       14 2023-06-25 22:08:23.000000 UpyTest-3.1.2/UpyTest.egg-info/top_level.txt
--rw-rw-r--   0 idtaleb   (1000) idtaleb   (1000)       38 2023-06-25 22:08:24.033028 UpyTest-3.1.2/setup.cfg
--rw-rw-r--   0 idtaleb   (1000) idtaleb   (1000)     1985 2023-06-25 22:08:20.000000 UpyTest-3.1.2/setup.py
-drwxrwxr-x   0 idtaleb   (1000) idtaleb   (1000)        0 2023-06-25 22:08:24.025028 UpyTest-3.1.2/thonnycontrib/
--rw-rw-r--   0 idtaleb   (1000) idtaleb   (1000)      947 2023-06-24 22:43:54.000000 UpyTest-3.1.2/thonnycontrib/ThonnyLogsGenerator.py
--rw-rw-r--   0 idtaleb   (1000) idtaleb   (1000)        0 2023-06-24 22:52:20.000000 UpyTest-3.1.2/thonnycontrib/__init__.py
-drwxrwxr-x   0 idtaleb   (1000) idtaleb   (1000)        0 2023-06-25 22:08:24.025028 UpyTest-3.1.2/thonnycontrib/backend/
--rw-rw-r--   0 idtaleb   (1000) idtaleb   (1000)        0 2023-03-15 10:38:40.000000 UpyTest-3.1.2/thonnycontrib/backend/__init__.py
--rw-rw-r--   0 idtaleb   (1000) idtaleb   (1000)    16304 2023-06-24 19:59:14.000000 UpyTest-3.1.2/thonnycontrib/backend/ast_parser.py
--rw-rw-r--   0 idtaleb   (1000) idtaleb   (1000)    35328 2023-06-25 21:33:06.000000 UpyTest-3.1.2/thonnycontrib/backend/doctest_parser.py
--rw-rw-r--   0 idtaleb   (1000) idtaleb   (1000)     5028 2023-06-24 15:10:56.000000 UpyTest-3.1.2/thonnycontrib/backend/evaluator.py
--rw-rw-r--   0 idtaleb   (1000) idtaleb   (1000)     4503 2023-06-25 22:01:28.000000 UpyTest-3.1.2/thonnycontrib/backend/l1test_backend.py
--rw-rw-r--   0 idtaleb   (1000) idtaleb   (1000)     6541 2023-06-24 18:11:15.000000 UpyTest-3.1.2/thonnycontrib/backend/test_finder.py
-drwxrwxr-x   0 idtaleb   (1000) idtaleb   (1000)        0 2023-06-25 22:08:24.025028 UpyTest-3.1.2/thonnycontrib/backend/verdicts/
--rw-rw-r--   0 idtaleb   (1000) idtaleb   (1000)     2057 2023-06-24 19:29:56.000000 UpyTest-3.1.2/thonnycontrib/backend/verdicts/ExampleVerdict.py
--rw-rw-r--   0 idtaleb   (1000) idtaleb   (1000)      496 2023-06-24 18:12:47.000000 UpyTest-3.1.2/thonnycontrib/backend/verdicts/ExceptionVerdict.py
--rw-rw-r--   0 idtaleb   (1000) idtaleb   (1000)      733 2023-06-24 18:13:06.000000 UpyTest-3.1.2/thonnycontrib/backend/verdicts/FailedVerdict.py
--rw-rw-r--   0 idtaleb   (1000) idtaleb   (1000)      637 2023-06-24 19:25:27.000000 UpyTest-3.1.2/thonnycontrib/backend/verdicts/FailedWhenExceptionExpectedVerdict.py
--rw-rw-r--   0 idtaleb   (1000) idtaleb   (1000)      450 2023-06-24 18:12:56.000000 UpyTest-3.1.2/thonnycontrib/backend/verdicts/PassedVerdict.py
--rw-rw-r--   0 idtaleb   (1000) idtaleb   (1000)      377 2023-06-24 18:13:00.000000 UpyTest-3.1.2/thonnycontrib/backend/verdicts/SetupVerdict.py
--rw-rw-r--   0 idtaleb   (1000) idtaleb   (1000)        0 2023-06-24 02:35:02.000000 UpyTest-3.1.2/thonnycontrib/backend/verdicts/__init__.py
-drwxrwxr-x   0 idtaleb   (1000) idtaleb   (1000)        0 2023-06-25 22:08:24.025028 UpyTest-3.1.2/thonnycontrib/docs/
--rw-rw-r--   0 idtaleb   (1000) idtaleb   (1000)        0 2023-03-15 10:38:40.000000 UpyTest-3.1.2/thonnycontrib/docs/__init__.py
-drwxrwxr-x   0 idtaleb   (1000) idtaleb   (1000)        0 2023-06-25 22:08:24.029028 UpyTest-3.1.2/thonnycontrib/docs/res/
--rw-rw-r--   0 idtaleb   (1000) idtaleb   (1000)      912 2023-06-21 22:17:10.000000 UpyTest-3.1.2/thonnycontrib/docs/res/error_icon.png
--rw-rw-r--   0 idtaleb   (1000) idtaleb   (1000)     1275 2023-03-15 10:38:40.000000 UpyTest-3.1.2/thonnycontrib/docs/res/failed.png
--rw-rw-r--   0 idtaleb   (1000) idtaleb   (1000)     1468 2023-06-25 02:50:15.000000 UpyTest-3.1.2/thonnycontrib/docs/res/l1test_debug.png
--rw-rw-r--   0 idtaleb   (1000) idtaleb   (1000)     2130 2023-03-15 10:38:40.000000 UpyTest-3.1.2/thonnycontrib/docs/res/l1test_icon.png
--rw-rw-r--   0 idtaleb   (1000) idtaleb   (1000)     2086 2023-03-15 10:38:40.000000 UpyTest-3.1.2/thonnycontrib/docs/res/l1test_icon_old.png
--rw-rw-r--   0 idtaleb   (1000) idtaleb   (1000)      628 2023-04-23 12:41:34.000000 UpyTest-3.1.2/thonnycontrib/docs/res/outline_class.png
--rw-rw-r--   0 idtaleb   (1000) idtaleb   (1000)      578 2023-04-23 12:41:32.000000 UpyTest-3.1.2/thonnycontrib/docs/res/outline_method.gif
--rw-rw-r--   0 idtaleb   (1000) idtaleb   (1000)     1213 2023-03-15 10:38:40.000000 UpyTest-3.1.2/thonnycontrib/docs/res/passed.png
--rw-rw-r--   0 idtaleb   (1000) idtaleb   (1000)     1531 2023-03-15 10:38:40.000000 UpyTest-3.1.2/thonnycontrib/docs/res/pending_icon.png
--rw-rw-r--   0 idtaleb   (1000) idtaleb   (1000)      997 2023-06-21 22:19:21.000000 UpyTest-3.1.2/thonnycontrib/docs/res/restart_icon.png
--rw-rw-r--   0 idtaleb   (1000) idtaleb   (1000)     2282 2023-03-15 10:38:40.000000 UpyTest-3.1.2/thonnycontrib/docs/res/test_only_btn.png
--rw-rw-r--   0 idtaleb   (1000) idtaleb   (1000)     1073 2023-03-15 10:38:40.000000 UpyTest-3.1.2/thonnycontrib/docs/res/warning.png
-drwxrwxr-x   0 idtaleb   (1000) idtaleb   (1000)        0 2023-06-25 22:08:24.029028 UpyTest-3.1.2/thonnycontrib/docstring_generator/
--rw-rw-r--   0 idtaleb   (1000) idtaleb   (1000)        0 2023-03-15 10:38:40.000000 UpyTest-3.1.2/thonnycontrib/docstring_generator/__init__.py
--rw-rw-r--   0 idtaleb   (1000) idtaleb   (1000)     8660 2023-06-24 13:42:03.000000 UpyTest-3.1.2/thonnycontrib/docstring_generator/doc_generator.py
--rw-rw-r--   0 idtaleb   (1000) idtaleb   (1000)     7134 2023-03-15 10:38:40.000000 UpyTest-3.1.2/thonnycontrib/docstring_generator/doc_template.py
--rw-rw-r--   0 idtaleb   (1000) idtaleb   (1000)     1315 2023-06-25 20:12:20.000000 UpyTest-3.1.2/thonnycontrib/environement_vars.py
--rw-rw-r--   0 idtaleb   (1000) idtaleb   (1000)     3756 2023-06-23 23:49:24.000000 UpyTest-3.1.2/thonnycontrib/exceptions.py
-drwxrwxr-x   0 idtaleb   (1000) idtaleb   (1000)        0 2023-06-25 22:08:24.029028 UpyTest-3.1.2/thonnycontrib/l1test_configuration/
--rw-rw-r--   0 idtaleb   (1000) idtaleb   (1000)        0 2023-03-15 10:38:40.000000 UpyTest-3.1.2/thonnycontrib/l1test_configuration/__init__.py
--rw-rw-r--   0 idtaleb   (1000) idtaleb   (1000)     2575 2023-04-02 02:23:42.000000 UpyTest-3.1.2/thonnycontrib/l1test_configuration/l1test_options.py
-drwxrwxr-x   0 idtaleb   (1000) idtaleb   (1000)        0 2023-06-25 22:08:24.029028 UpyTest-3.1.2/thonnycontrib/l1test_frontend/
--rw-rw-r--   0 idtaleb   (1000) idtaleb   (1000)      708 2023-06-24 22:52:29.000000 UpyTest-3.1.2/thonnycontrib/l1test_frontend/__init__.py
--rw-rw-r--   0 idtaleb   (1000) idtaleb   (1000)     2507 2023-06-25 03:08:15.000000 UpyTest-3.1.2/thonnycontrib/l1test_frontend/l1test_error_view.py
--rw-rw-r--   0 idtaleb   (1000) idtaleb   (1000)     2756 2023-06-25 13:23:15.000000 UpyTest-3.1.2/thonnycontrib/l1test_frontend/l1test_reporter.py
--rw-rw-r--   0 idtaleb   (1000) idtaleb   (1000)    23408 2023-06-25 22:07:30.000000 UpyTest-3.1.2/thonnycontrib/l1test_frontend/l1test_runner.py
--rw-rw-r--   0 idtaleb   (1000) idtaleb   (1000)    36550 2023-06-25 20:32:06.000000 UpyTest-3.1.2/thonnycontrib/l1test_frontend/l1test_treeview.py
--rw-rw-r--   0 idtaleb   (1000) idtaleb   (1000)     3523 2023-06-25 21:48:20.000000 UpyTest-3.1.2/thonnycontrib/l1test_frontend/outlines.py
--rw-rw-r--   0 idtaleb   (1000) idtaleb   (1000)     7310 2023-06-25 21:56:55.000000 UpyTest-3.1.2/thonnycontrib/plugin_loader.py
--rw-rw-r--   0 idtaleb   (1000) idtaleb   (1000)     2432 2023-06-25 02:35:31.000000 UpyTest-3.1.2/thonnycontrib/properties.py
-drwxrwxr-x   0 idtaleb   (1000) idtaleb   (1000)        0 2023-06-25 22:08:24.029028 UpyTest-3.1.2/thonnycontrib/tests/
--rw-rw-r--   0 idtaleb   (1000) idtaleb   (1000)        0 2023-03-15 10:38:42.000000 UpyTest-3.1.2/thonnycontrib/tests/__init__.py
--rw-rw-r--   0 idtaleb   (1000) idtaleb   (1000)      348 2023-03-15 10:38:42.000000 UpyTest-3.1.2/thonnycontrib/tests/backend_mock.py
--rw-rw-r--   0 idtaleb   (1000) idtaleb   (1000)     1980 2023-03-15 10:38:42.000000 UpyTest-3.1.2/thonnycontrib/tests/test_doc_generator.py
--rw-rw-r--   0 idtaleb   (1000) idtaleb   (1000)     4848 2023-06-24 02:33:48.000000 UpyTest-3.1.2/thonnycontrib/tests/tests_example_no_expected.py
--rw-rw-r--   0 idtaleb   (1000) idtaleb   (1000)    14741 2023-06-24 02:34:31.000000 UpyTest-3.1.2/thonnycontrib/tests/tests_example_with_exception.py
--rw-rw-r--   0 idtaleb   (1000) idtaleb   (1000)    18496 2023-06-24 02:34:31.000000 UpyTest-3.1.2/thonnycontrib/tests/tests_example_with_expected.py
--rw-rw-r--   0 idtaleb   (1000) idtaleb   (1000)     9799 2023-06-25 13:23:15.000000 UpyTest-3.1.2/thonnycontrib/tests/tests_l1TestRunner.py
--rw-rw-r--   0 idtaleb   (1000) idtaleb   (1000)     6392 2023-06-23 23:27:45.000000 UpyTest-3.1.2/thonnycontrib/tests/tests_test_finder.py
--rw-rw-r--   0 idtaleb   (1000) idtaleb   (1000)    12629 2023-06-24 02:34:31.000000 UpyTest-3.1.2/thonnycontrib/tests/tests_view.py
--rw-rw-r--   0 idtaleb   (1000) idtaleb   (1000)    18919 2023-06-25 22:06:41.000000 UpyTest-3.1.2/thonnycontrib/utils.py
+drwxrwxr-x   0 idtaleb   (1000) idtaleb   (1000)        0 2023-06-25 22:27:11.231478 UpyTest-3.1.3/
+-rw-rw-r--   0 idtaleb   (1000) idtaleb   (1000)      694 2023-06-25 22:27:11.231478 UpyTest-3.1.3/PKG-INFO
+drwxrwxr-x   0 idtaleb   (1000) idtaleb   (1000)        0 2023-06-25 22:27:11.223478 UpyTest-3.1.3/UpyTest.egg-info/
+-rw-rw-r--   0 idtaleb   (1000) idtaleb   (1000)      694 2023-06-25 22:27:11.000000 UpyTest-3.1.3/UpyTest.egg-info/PKG-INFO
+-rw-rw-r--   0 idtaleb   (1000) idtaleb   (1000)     2351 2023-06-25 22:27:11.000000 UpyTest-3.1.3/UpyTest.egg-info/SOURCES.txt
+-rw-rw-r--   0 idtaleb   (1000) idtaleb   (1000)        1 2023-06-25 22:27:11.000000 UpyTest-3.1.3/UpyTest.egg-info/dependency_links.txt
+-rw-rw-r--   0 idtaleb   (1000) idtaleb   (1000)       14 2023-06-25 22:27:11.000000 UpyTest-3.1.3/UpyTest.egg-info/requires.txt
+-rw-rw-r--   0 idtaleb   (1000) idtaleb   (1000)       14 2023-06-25 22:27:11.000000 UpyTest-3.1.3/UpyTest.egg-info/top_level.txt
+-rw-rw-r--   0 idtaleb   (1000) idtaleb   (1000)       38 2023-06-25 22:27:11.231478 UpyTest-3.1.3/setup.cfg
+-rw-rw-r--   0 idtaleb   (1000) idtaleb   (1000)     1985 2023-06-25 22:23:46.000000 UpyTest-3.1.3/setup.py
+drwxrwxr-x   0 idtaleb   (1000) idtaleb   (1000)        0 2023-06-25 22:27:11.223478 UpyTest-3.1.3/thonnycontrib/
+-rw-rw-r--   0 idtaleb   (1000) idtaleb   (1000)      947 2023-06-24 22:43:54.000000 UpyTest-3.1.3/thonnycontrib/ThonnyLogsGenerator.py
+-rw-rw-r--   0 idtaleb   (1000) idtaleb   (1000)        0 2023-06-24 22:52:20.000000 UpyTest-3.1.3/thonnycontrib/__init__.py
+drwxrwxr-x   0 idtaleb   (1000) idtaleb   (1000)        0 2023-06-25 22:27:11.223478 UpyTest-3.1.3/thonnycontrib/backend/
+-rw-rw-r--   0 idtaleb   (1000) idtaleb   (1000)        0 2023-03-15 10:38:40.000000 UpyTest-3.1.3/thonnycontrib/backend/__init__.py
+-rw-rw-r--   0 idtaleb   (1000) idtaleb   (1000)    16304 2023-06-24 19:59:14.000000 UpyTest-3.1.3/thonnycontrib/backend/ast_parser.py
+-rw-rw-r--   0 idtaleb   (1000) idtaleb   (1000)    35328 2023-06-25 21:33:06.000000 UpyTest-3.1.3/thonnycontrib/backend/doctest_parser.py
+-rw-rw-r--   0 idtaleb   (1000) idtaleb   (1000)     5028 2023-06-24 15:10:56.000000 UpyTest-3.1.3/thonnycontrib/backend/evaluator.py
+-rw-rw-r--   0 idtaleb   (1000) idtaleb   (1000)     4503 2023-06-25 22:01:28.000000 UpyTest-3.1.3/thonnycontrib/backend/l1test_backend.py
+-rw-rw-r--   0 idtaleb   (1000) idtaleb   (1000)     6541 2023-06-24 18:11:15.000000 UpyTest-3.1.3/thonnycontrib/backend/test_finder.py
+drwxrwxr-x   0 idtaleb   (1000) idtaleb   (1000)        0 2023-06-25 22:27:11.223478 UpyTest-3.1.3/thonnycontrib/backend/verdicts/
+-rw-rw-r--   0 idtaleb   (1000) idtaleb   (1000)     2057 2023-06-24 19:29:56.000000 UpyTest-3.1.3/thonnycontrib/backend/verdicts/ExampleVerdict.py
+-rw-rw-r--   0 idtaleb   (1000) idtaleb   (1000)      496 2023-06-24 18:12:47.000000 UpyTest-3.1.3/thonnycontrib/backend/verdicts/ExceptionVerdict.py
+-rw-rw-r--   0 idtaleb   (1000) idtaleb   (1000)      733 2023-06-24 18:13:06.000000 UpyTest-3.1.3/thonnycontrib/backend/verdicts/FailedVerdict.py
+-rw-rw-r--   0 idtaleb   (1000) idtaleb   (1000)      637 2023-06-24 19:25:27.000000 UpyTest-3.1.3/thonnycontrib/backend/verdicts/FailedWhenExceptionExpectedVerdict.py
+-rw-rw-r--   0 idtaleb   (1000) idtaleb   (1000)      450 2023-06-24 18:12:56.000000 UpyTest-3.1.3/thonnycontrib/backend/verdicts/PassedVerdict.py
+-rw-rw-r--   0 idtaleb   (1000) idtaleb   (1000)      377 2023-06-24 18:13:00.000000 UpyTest-3.1.3/thonnycontrib/backend/verdicts/SetupVerdict.py
+-rw-rw-r--   0 idtaleb   (1000) idtaleb   (1000)        0 2023-06-24 02:35:02.000000 UpyTest-3.1.3/thonnycontrib/backend/verdicts/__init__.py
+drwxrwxr-x   0 idtaleb   (1000) idtaleb   (1000)        0 2023-06-25 22:27:11.223478 UpyTest-3.1.3/thonnycontrib/docs/
+-rw-rw-r--   0 idtaleb   (1000) idtaleb   (1000)        0 2023-03-15 10:38:40.000000 UpyTest-3.1.3/thonnycontrib/docs/__init__.py
+drwxrwxr-x   0 idtaleb   (1000) idtaleb   (1000)        0 2023-06-25 22:27:11.227478 UpyTest-3.1.3/thonnycontrib/docs/res/
+-rw-rw-r--   0 idtaleb   (1000) idtaleb   (1000)      912 2023-06-21 22:17:10.000000 UpyTest-3.1.3/thonnycontrib/docs/res/error_icon.png
+-rw-rw-r--   0 idtaleb   (1000) idtaleb   (1000)     1275 2023-03-15 10:38:40.000000 UpyTest-3.1.3/thonnycontrib/docs/res/failed.png
+-rw-rw-r--   0 idtaleb   (1000) idtaleb   (1000)     1468 2023-06-25 02:50:15.000000 UpyTest-3.1.3/thonnycontrib/docs/res/l1test_debug.png
+-rw-rw-r--   0 idtaleb   (1000) idtaleb   (1000)     2130 2023-03-15 10:38:40.000000 UpyTest-3.1.3/thonnycontrib/docs/res/l1test_icon.png
+-rw-rw-r--   0 idtaleb   (1000) idtaleb   (1000)     2086 2023-03-15 10:38:40.000000 UpyTest-3.1.3/thonnycontrib/docs/res/l1test_icon_old.png
+-rw-rw-r--   0 idtaleb   (1000) idtaleb   (1000)      628 2023-04-23 12:41:34.000000 UpyTest-3.1.3/thonnycontrib/docs/res/outline_class.png
+-rw-rw-r--   0 idtaleb   (1000) idtaleb   (1000)      578 2023-04-23 12:41:32.000000 UpyTest-3.1.3/thonnycontrib/docs/res/outline_method.gif
+-rw-rw-r--   0 idtaleb   (1000) idtaleb   (1000)     1213 2023-03-15 10:38:40.000000 UpyTest-3.1.3/thonnycontrib/docs/res/passed.png
+-rw-rw-r--   0 idtaleb   (1000) idtaleb   (1000)     1531 2023-03-15 10:38:40.000000 UpyTest-3.1.3/thonnycontrib/docs/res/pending_icon.png
+-rw-rw-r--   0 idtaleb   (1000) idtaleb   (1000)      997 2023-06-21 22:19:21.000000 UpyTest-3.1.3/thonnycontrib/docs/res/restart_icon.png
+-rw-rw-r--   0 idtaleb   (1000) idtaleb   (1000)     2282 2023-03-15 10:38:40.000000 UpyTest-3.1.3/thonnycontrib/docs/res/test_only_btn.png
+-rw-rw-r--   0 idtaleb   (1000) idtaleb   (1000)     1073 2023-03-15 10:38:40.000000 UpyTest-3.1.3/thonnycontrib/docs/res/warning.png
+drwxrwxr-x   0 idtaleb   (1000) idtaleb   (1000)        0 2023-06-25 22:27:11.227478 UpyTest-3.1.3/thonnycontrib/docstring_generator/
+-rw-rw-r--   0 idtaleb   (1000) idtaleb   (1000)        0 2023-03-15 10:38:40.000000 UpyTest-3.1.3/thonnycontrib/docstring_generator/__init__.py
+-rw-rw-r--   0 idtaleb   (1000) idtaleb   (1000)     8660 2023-06-24 13:42:03.000000 UpyTest-3.1.3/thonnycontrib/docstring_generator/doc_generator.py
+-rw-rw-r--   0 idtaleb   (1000) idtaleb   (1000)     7134 2023-03-15 10:38:40.000000 UpyTest-3.1.3/thonnycontrib/docstring_generator/doc_template.py
+-rw-rw-r--   0 idtaleb   (1000) idtaleb   (1000)     1315 2023-06-25 20:12:20.000000 UpyTest-3.1.3/thonnycontrib/environement_vars.py
+-rw-rw-r--   0 idtaleb   (1000) idtaleb   (1000)     3756 2023-06-23 23:49:24.000000 UpyTest-3.1.3/thonnycontrib/exceptions.py
+drwxrwxr-x   0 idtaleb   (1000) idtaleb   (1000)        0 2023-06-25 22:27:11.227478 UpyTest-3.1.3/thonnycontrib/l1test_configuration/
+-rw-rw-r--   0 idtaleb   (1000) idtaleb   (1000)        0 2023-03-15 10:38:40.000000 UpyTest-3.1.3/thonnycontrib/l1test_configuration/__init__.py
+-rw-rw-r--   0 idtaleb   (1000) idtaleb   (1000)     2575 2023-04-02 02:23:42.000000 UpyTest-3.1.3/thonnycontrib/l1test_configuration/l1test_options.py
+drwxrwxr-x   0 idtaleb   (1000) idtaleb   (1000)        0 2023-06-25 22:27:11.227478 UpyTest-3.1.3/thonnycontrib/l1test_frontend/
+-rw-rw-r--   0 idtaleb   (1000) idtaleb   (1000)      708 2023-06-24 22:52:29.000000 UpyTest-3.1.3/thonnycontrib/l1test_frontend/__init__.py
+-rw-rw-r--   0 idtaleb   (1000) idtaleb   (1000)     2507 2023-06-25 03:08:15.000000 UpyTest-3.1.3/thonnycontrib/l1test_frontend/l1test_error_view.py
+-rw-rw-r--   0 idtaleb   (1000) idtaleb   (1000)     2756 2023-06-25 13:23:15.000000 UpyTest-3.1.3/thonnycontrib/l1test_frontend/l1test_reporter.py
+-rw-rw-r--   0 idtaleb   (1000) idtaleb   (1000)    23428 2023-06-25 22:26:48.000000 UpyTest-3.1.3/thonnycontrib/l1test_frontend/l1test_runner.py
+-rw-rw-r--   0 idtaleb   (1000) idtaleb   (1000)    36550 2023-06-25 20:32:06.000000 UpyTest-3.1.3/thonnycontrib/l1test_frontend/l1test_treeview.py
+-rw-rw-r--   0 idtaleb   (1000) idtaleb   (1000)     3523 2023-06-25 21:48:20.000000 UpyTest-3.1.3/thonnycontrib/l1test_frontend/outlines.py
+-rw-rw-r--   0 idtaleb   (1000) idtaleb   (1000)     7310 2023-06-25 21:56:55.000000 UpyTest-3.1.3/thonnycontrib/plugin_loader.py
+-rw-rw-r--   0 idtaleb   (1000) idtaleb   (1000)     2432 2023-06-25 02:35:31.000000 UpyTest-3.1.3/thonnycontrib/properties.py
+drwxrwxr-x   0 idtaleb   (1000) idtaleb   (1000)        0 2023-06-25 22:27:11.231478 UpyTest-3.1.3/thonnycontrib/tests/
+-rw-rw-r--   0 idtaleb   (1000) idtaleb   (1000)        0 2023-03-15 10:38:42.000000 UpyTest-3.1.3/thonnycontrib/tests/__init__.py
+-rw-rw-r--   0 idtaleb   (1000) idtaleb   (1000)      348 2023-03-15 10:38:42.000000 UpyTest-3.1.3/thonnycontrib/tests/backend_mock.py
+-rw-rw-r--   0 idtaleb   (1000) idtaleb   (1000)     1980 2023-03-15 10:38:42.000000 UpyTest-3.1.3/thonnycontrib/tests/test_doc_generator.py
+-rw-rw-r--   0 idtaleb   (1000) idtaleb   (1000)     4848 2023-06-24 02:33:48.000000 UpyTest-3.1.3/thonnycontrib/tests/tests_example_no_expected.py
+-rw-rw-r--   0 idtaleb   (1000) idtaleb   (1000)    14741 2023-06-24 02:34:31.000000 UpyTest-3.1.3/thonnycontrib/tests/tests_example_with_exception.py
+-rw-rw-r--   0 idtaleb   (1000) idtaleb   (1000)    18496 2023-06-24 02:34:31.000000 UpyTest-3.1.3/thonnycontrib/tests/tests_example_with_expected.py
+-rw-rw-r--   0 idtaleb   (1000) idtaleb   (1000)     9799 2023-06-25 13:23:15.000000 UpyTest-3.1.3/thonnycontrib/tests/tests_l1TestRunner.py
+-rw-rw-r--   0 idtaleb   (1000) idtaleb   (1000)     6392 2023-06-23 23:27:45.000000 UpyTest-3.1.3/thonnycontrib/tests/tests_test_finder.py
+-rw-rw-r--   0 idtaleb   (1000) idtaleb   (1000)    12629 2023-06-24 02:34:31.000000 UpyTest-3.1.3/thonnycontrib/tests/tests_view.py
+-rw-rw-r--   0 idtaleb   (1000) idtaleb   (1000)    18919 2023-06-25 22:06:41.000000 UpyTest-3.1.3/thonnycontrib/utils.py
```

### Comparing `UpyTest-3.1.2/PKG-INFO` & `UpyTest-3.1.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: UpyTest
-Version: 3.1.2
+Version: 3.1.3
 Summary: A plug-in which adds a test framework
 Home-page: https://gitlab.univ-lille.fr/reda.idtaleb.etu/thonny_test_framework
 Author: Réda Id-taleb
 Platform: Windows
 Platform: macOS
 Platform: Linux
 Classifier: Topic :: Education :: Testing
```

### Comparing `UpyTest-3.1.2/UpyTest.egg-info/PKG-INFO` & `UpyTest-3.1.3/UpyTest.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: UpyTest
-Version: 3.1.2
+Version: 3.1.3
 Summary: A plug-in which adds a test framework
 Home-page: https://gitlab.univ-lille.fr/reda.idtaleb.etu/thonny_test_framework
 Author: Réda Id-taleb
 Platform: Windows
 Platform: macOS
 Platform: Linux
 Classifier: Topic :: Education :: Testing
```

### Comparing `UpyTest-3.1.2/UpyTest.egg-info/SOURCES.txt` & `UpyTest-3.1.3/UpyTest.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `UpyTest-3.1.2/setup.py` & `UpyTest-3.1.3/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -27,15 +27,15 @@
     return py_packs | other_packs
 
 setupdir = os.path.dirname(__file__)
 
 
 setup(
     name="UpyTest",
-    version="3.1.2",
+    version="3.1.3",
     author="Réda Id-taleb",
     description="A plug-in which adds a test framework",
     long_description="""A plug-in for Thonny which allows you to test your doc examples
  
 More info: https://gitlab.univ-lille.fr/reda.idtaleb.etu/thonny_test_framework""",
     url="https://gitlab.univ-lille.fr/reda.idtaleb.etu/thonny_test_framework",
 #    keywords="IDE education programming tests in documentation",
```

### Comparing `UpyTest-3.1.2/thonnycontrib/ThonnyLogsGenerator.py` & `UpyTest-3.1.3/thonnycontrib/ThonnyLogsGenerator.py`

 * *Files identical despite different names*

### Comparing `UpyTest-3.1.2/thonnycontrib/backend/ast_parser.py` & `UpyTest-3.1.3/thonnycontrib/backend/ast_parser.py`

 * *Files identical despite different names*

### Comparing `UpyTest-3.1.2/thonnycontrib/backend/doctest_parser.py` & `UpyTest-3.1.3/thonnycontrib/backend/doctest_parser.py`

 * *Files identical despite different names*

### Comparing `UpyTest-3.1.2/thonnycontrib/backend/evaluator.py` & `UpyTest-3.1.3/thonnycontrib/backend/evaluator.py`

 * *Files identical despite different names*

### Comparing `UpyTest-3.1.2/thonnycontrib/backend/l1test_backend.py` & `UpyTest-3.1.3/thonnycontrib/backend/l1test_backend.py`

 * *Files identical despite different names*

### Comparing `UpyTest-3.1.2/thonnycontrib/backend/test_finder.py` & `UpyTest-3.1.3/thonnycontrib/backend/test_finder.py`

 * *Files identical despite different names*

### Comparing `UpyTest-3.1.2/thonnycontrib/backend/verdicts/ExampleVerdict.py` & `UpyTest-3.1.3/thonnycontrib/backend/verdicts/ExampleVerdict.py`

 * *Files identical despite different names*

### Comparing `UpyTest-3.1.2/thonnycontrib/backend/verdicts/FailedVerdict.py` & `UpyTest-3.1.3/thonnycontrib/backend/verdicts/FailedVerdict.py`

 * *Files identical despite different names*

### Comparing `UpyTest-3.1.2/thonnycontrib/backend/verdicts/FailedWhenExceptionExpectedVerdict.py` & `UpyTest-3.1.3/thonnycontrib/backend/verdicts/FailedWhenExceptionExpectedVerdict.py`

 * *Files identical despite different names*

### Comparing `UpyTest-3.1.2/thonnycontrib/docs/res/error_icon.png` & `UpyTest-3.1.3/thonnycontrib/docs/res/error_icon.png`

 * *Files identical despite different names*

### Comparing `UpyTest-3.1.2/thonnycontrib/docs/res/failed.png` & `UpyTest-3.1.3/thonnycontrib/docs/res/failed.png`

 * *Files identical despite different names*

### Comparing `UpyTest-3.1.2/thonnycontrib/docs/res/l1test_debug.png` & `UpyTest-3.1.3/thonnycontrib/docs/res/l1test_debug.png`

 * *Files identical despite different names*

### Comparing `UpyTest-3.1.2/thonnycontrib/docs/res/l1test_icon.png` & `UpyTest-3.1.3/thonnycontrib/docs/res/l1test_icon.png`

 * *Files identical despite different names*

### Comparing `UpyTest-3.1.2/thonnycontrib/docs/res/l1test_icon_old.png` & `UpyTest-3.1.3/thonnycontrib/docs/res/l1test_icon_old.png`

 * *Files identical despite different names*

### Comparing `UpyTest-3.1.2/thonnycontrib/docs/res/outline_class.png` & `UpyTest-3.1.3/thonnycontrib/docs/res/outline_class.png`

 * *Files identical despite different names*

### Comparing `UpyTest-3.1.2/thonnycontrib/docs/res/outline_method.gif` & `UpyTest-3.1.3/thonnycontrib/docs/res/outline_method.gif`

 * *Files identical despite different names*

### Comparing `UpyTest-3.1.2/thonnycontrib/docs/res/passed.png` & `UpyTest-3.1.3/thonnycontrib/docs/res/passed.png`

 * *Files identical despite different names*

### Comparing `UpyTest-3.1.2/thonnycontrib/docs/res/pending_icon.png` & `UpyTest-3.1.3/thonnycontrib/docs/res/pending_icon.png`

 * *Files identical despite different names*

### Comparing `UpyTest-3.1.2/thonnycontrib/docs/res/restart_icon.png` & `UpyTest-3.1.3/thonnycontrib/docs/res/restart_icon.png`

 * *Files identical despite different names*

### Comparing `UpyTest-3.1.2/thonnycontrib/docs/res/test_only_btn.png` & `UpyTest-3.1.3/thonnycontrib/docs/res/test_only_btn.png`

 * *Files identical despite different names*

### Comparing `UpyTest-3.1.2/thonnycontrib/docs/res/warning.png` & `UpyTest-3.1.3/thonnycontrib/docs/res/warning.png`

 * *Files identical despite different names*

### Comparing `UpyTest-3.1.2/thonnycontrib/docstring_generator/doc_generator.py` & `UpyTest-3.1.3/thonnycontrib/docstring_generator/doc_generator.py`

 * *Files identical despite different names*

### Comparing `UpyTest-3.1.2/thonnycontrib/docstring_generator/doc_template.py` & `UpyTest-3.1.3/thonnycontrib/docstring_generator/doc_template.py`

 * *Files identical despite different names*

### Comparing `UpyTest-3.1.2/thonnycontrib/environement_vars.py` & `UpyTest-3.1.3/thonnycontrib/environement_vars.py`

 * *Files identical despite different names*

### Comparing `UpyTest-3.1.2/thonnycontrib/exceptions.py` & `UpyTest-3.1.3/thonnycontrib/exceptions.py`

 * *Files identical despite different names*

### Comparing `UpyTest-3.1.2/thonnycontrib/l1test_configuration/l1test_options.py` & `UpyTest-3.1.3/thonnycontrib/l1test_configuration/l1test_options.py`

 * *Files identical despite different names*

### Comparing `UpyTest-3.1.2/thonnycontrib/l1test_frontend/__init__.py` & `UpyTest-3.1.3/thonnycontrib/l1test_frontend/__init__.py`

 * *Files identical despite different names*

### Comparing `UpyTest-3.1.2/thonnycontrib/l1test_frontend/l1test_error_view.py` & `UpyTest-3.1.3/thonnycontrib/l1test_frontend/l1test_error_view.py`

 * *Files identical despite different names*

### Comparing `UpyTest-3.1.2/thonnycontrib/l1test_frontend/l1test_reporter.py` & `UpyTest-3.1.3/thonnycontrib/l1test_frontend/l1test_reporter.py`

 * *Files identical despite different names*

### Comparing `UpyTest-3.1.2/thonnycontrib/l1test_frontend/l1test_runner.py` & `UpyTest-3.1.3/thonnycontrib/l1test_frontend/l1test_runner.py`

 * *Files 0% similar despite different names*

```diff
@@ -139,16 +139,16 @@
         try:
             self.set_is_running()
             self.__request_backend(selected_line=selected_line)
         except:
             self.set_is_running(False)
             treeview.insert_in_header("Coudn't restart the backend.\nPlease restart with the 'Stop' button !", 
                                       clear=True, tags=("red"), image="error_icon.png")
-
-        clear_env_vars(IMPORT_MODULE_VAR, SELECTED_LINE_VAR)
+        finally:
+            clear_env_vars(IMPORT_MODULE_VAR, SELECTED_LINE_VAR)
         
     def __request_backend(self, command_name=BACKEND_COMMAND, selected_line:int=None):
         """
         Sends a command to the Thonny's backend to execute the current script.
         The name of the command must starts with a uppercase.    
         
         Please note that `thonny.get_runner.execute_current()` will consider
```

### Comparing `UpyTest-3.1.2/thonnycontrib/l1test_frontend/l1test_treeview.py` & `UpyTest-3.1.3/thonnycontrib/l1test_frontend/l1test_treeview.py`

 * *Files identical despite different names*

### Comparing `UpyTest-3.1.2/thonnycontrib/l1test_frontend/outlines.py` & `UpyTest-3.1.3/thonnycontrib/l1test_frontend/outlines.py`

 * *Files identical despite different names*

### Comparing `UpyTest-3.1.2/thonnycontrib/plugin_loader.py` & `UpyTest-3.1.3/thonnycontrib/plugin_loader.py`

 * *Files identical despite different names*

### Comparing `UpyTest-3.1.2/thonnycontrib/properties.py` & `UpyTest-3.1.3/thonnycontrib/properties.py`

 * *Files identical despite different names*

### Comparing `UpyTest-3.1.2/thonnycontrib/tests/test_doc_generator.py` & `UpyTest-3.1.3/thonnycontrib/tests/test_doc_generator.py`

 * *Files identical despite different names*

### Comparing `UpyTest-3.1.2/thonnycontrib/tests/tests_example_no_expected.py` & `UpyTest-3.1.3/thonnycontrib/tests/tests_example_no_expected.py`

 * *Files identical despite different names*

### Comparing `UpyTest-3.1.2/thonnycontrib/tests/tests_example_with_exception.py` & `UpyTest-3.1.3/thonnycontrib/tests/tests_example_with_exception.py`

 * *Files identical despite different names*

### Comparing `UpyTest-3.1.2/thonnycontrib/tests/tests_example_with_expected.py` & `UpyTest-3.1.3/thonnycontrib/tests/tests_example_with_expected.py`

 * *Files identical despite different names*

### Comparing `UpyTest-3.1.2/thonnycontrib/tests/tests_l1TestRunner.py` & `UpyTest-3.1.3/thonnycontrib/tests/tests_l1TestRunner.py`

 * *Files identical despite different names*

### Comparing `UpyTest-3.1.2/thonnycontrib/tests/tests_test_finder.py` & `UpyTest-3.1.3/thonnycontrib/tests/tests_test_finder.py`

 * *Files identical despite different names*

### Comparing `UpyTest-3.1.2/thonnycontrib/tests/tests_view.py` & `UpyTest-3.1.3/thonnycontrib/tests/tests_view.py`

 * *Files identical despite different names*

### Comparing `UpyTest-3.1.2/thonnycontrib/utils.py` & `UpyTest-3.1.3/thonnycontrib/utils.py`

 * *Files identical despite different names*

