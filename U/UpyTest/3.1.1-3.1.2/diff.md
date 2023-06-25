# Comparing `tmp/UpyTest-3.1.1.tar.gz` & `tmp/UpyTest-3.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "UpyTest-3.1.1.tar", last modified: Sat Jun 24 23:05:20 2023, max compression
+gzip compressed data, was "UpyTest-3.1.2.tar", last modified: Sun Jun 25 22:08:24 2023, max compression
```

## Comparing `UpyTest-3.1.1.tar` & `UpyTest-3.1.2.tar`

### file list

```diff
@@ -1,71 +1,72 @@
-drwxrwxr-x   0 idtaleb   (1000) idtaleb   (1000)        0 2023-06-24 23:05:20.409857 UpyTest-3.1.1/
--rw-rw-r--   0 idtaleb   (1000) idtaleb   (1000)      694 2023-06-24 23:05:20.409857 UpyTest-3.1.1/PKG-INFO
-drwxrwxr-x   0 idtaleb   (1000) idtaleb   (1000)        0 2023-06-24 23:05:20.401857 UpyTest-3.1.1/UpyTest.egg-info/
--rw-rw-r--   0 idtaleb   (1000) idtaleb   (1000)      694 2023-06-24 23:05:20.000000 UpyTest-3.1.1/UpyTest.egg-info/PKG-INFO
--rw-rw-r--   0 idtaleb   (1000) idtaleb   (1000)     2311 2023-06-24 23:05:20.000000 UpyTest-3.1.1/UpyTest.egg-info/SOURCES.txt
--rw-rw-r--   0 idtaleb   (1000) idtaleb   (1000)        1 2023-06-24 23:05:20.000000 UpyTest-3.1.1/UpyTest.egg-info/dependency_links.txt
--rw-rw-r--   0 idtaleb   (1000) idtaleb   (1000)       14 2023-06-24 23:05:20.000000 UpyTest-3.1.1/UpyTest.egg-info/requires.txt
--rw-rw-r--   0 idtaleb   (1000) idtaleb   (1000)       14 2023-06-24 23:05:20.000000 UpyTest-3.1.1/UpyTest.egg-info/top_level.txt
--rw-rw-r--   0 idtaleb   (1000) idtaleb   (1000)       38 2023-06-24 23:05:20.409857 UpyTest-3.1.1/setup.cfg
--rw-rw-r--   0 idtaleb   (1000) idtaleb   (1000)     1985 2023-06-24 23:04:31.000000 UpyTest-3.1.1/setup.py
-drwxrwxr-x   0 idtaleb   (1000) idtaleb   (1000)        0 2023-06-24 23:05:20.401857 UpyTest-3.1.1/thonnycontrib/
--rw-rw-r--   0 idtaleb   (1000) idtaleb   (1000)      947 2023-06-24 22:43:54.000000 UpyTest-3.1.1/thonnycontrib/ThonnyLogsGenerator.py
--rw-rw-r--   0 idtaleb   (1000) idtaleb   (1000)        0 2023-06-24 22:52:20.000000 UpyTest-3.1.1/thonnycontrib/__init__.py
-drwxrwxr-x   0 idtaleb   (1000) idtaleb   (1000)        0 2023-06-24 23:05:20.401857 UpyTest-3.1.1/thonnycontrib/backend/
--rw-rw-r--   0 idtaleb   (1000) idtaleb   (1000)        0 2023-03-15 10:38:40.000000 UpyTest-3.1.1/thonnycontrib/backend/__init__.py
--rw-rw-r--   0 idtaleb   (1000) idtaleb   (1000)    16304 2023-06-24 19:59:14.000000 UpyTest-3.1.1/thonnycontrib/backend/ast_parser.py
--rw-rw-r--   0 idtaleb   (1000) idtaleb   (1000)    35341 2023-06-24 19:19:49.000000 UpyTest-3.1.1/thonnycontrib/backend/doctest_parser.py
--rw-rw-r--   0 idtaleb   (1000) idtaleb   (1000)     5028 2023-06-24 15:10:56.000000 UpyTest-3.1.1/thonnycontrib/backend/evaluator.py
--rw-rw-r--   0 idtaleb   (1000) idtaleb   (1000)     4560 2023-06-24 00:10:31.000000 UpyTest-3.1.1/thonnycontrib/backend/l1test_backend.py
--rw-rw-r--   0 idtaleb   (1000) idtaleb   (1000)     6541 2023-06-24 18:11:15.000000 UpyTest-3.1.1/thonnycontrib/backend/test_finder.py
-drwxrwxr-x   0 idtaleb   (1000) idtaleb   (1000)        0 2023-06-24 23:05:20.405857 UpyTest-3.1.1/thonnycontrib/backend/verdicts/
--rw-rw-r--   0 idtaleb   (1000) idtaleb   (1000)     2057 2023-06-24 19:29:56.000000 UpyTest-3.1.1/thonnycontrib/backend/verdicts/ExampleVerdict.py
--rw-rw-r--   0 idtaleb   (1000) idtaleb   (1000)      496 2023-06-24 18:12:47.000000 UpyTest-3.1.1/thonnycontrib/backend/verdicts/ExceptionVerdict.py
--rw-rw-r--   0 idtaleb   (1000) idtaleb   (1000)      733 2023-06-24 18:13:06.000000 UpyTest-3.1.1/thonnycontrib/backend/verdicts/FailedVerdict.py
--rw-rw-r--   0 idtaleb   (1000) idtaleb   (1000)      637 2023-06-24 19:25:27.000000 UpyTest-3.1.1/thonnycontrib/backend/verdicts/FailedWhenExceptionExpectedVerdict.py
--rw-rw-r--   0 idtaleb   (1000) idtaleb   (1000)      450 2023-06-24 18:12:56.000000 UpyTest-3.1.1/thonnycontrib/backend/verdicts/PassedVerdict.py
--rw-rw-r--   0 idtaleb   (1000) idtaleb   (1000)      377 2023-06-24 18:13:00.000000 UpyTest-3.1.1/thonnycontrib/backend/verdicts/SetupVerdict.py
--rw-rw-r--   0 idtaleb   (1000) idtaleb   (1000)        0 2023-06-24 02:35:02.000000 UpyTest-3.1.1/thonnycontrib/backend/verdicts/__init__.py
-drwxrwxr-x   0 idtaleb   (1000) idtaleb   (1000)        0 2023-06-24 23:05:20.405857 UpyTest-3.1.1/thonnycontrib/docs/
--rw-rw-r--   0 idtaleb   (1000) idtaleb   (1000)        0 2023-03-15 10:38:40.000000 UpyTest-3.1.1/thonnycontrib/docs/__init__.py
-drwxrwxr-x   0 idtaleb   (1000) idtaleb   (1000)        0 2023-06-24 23:05:20.405857 UpyTest-3.1.1/thonnycontrib/docs/res/
--rw-rw-r--   0 idtaleb   (1000) idtaleb   (1000)      912 2023-06-21 22:17:10.000000 UpyTest-3.1.1/thonnycontrib/docs/res/error_icon.png
--rw-rw-r--   0 idtaleb   (1000) idtaleb   (1000)     1275 2023-03-15 10:38:40.000000 UpyTest-3.1.1/thonnycontrib/docs/res/failed.png
--rw-rw-r--   0 idtaleb   (1000) idtaleb   (1000)     2130 2023-03-15 10:38:40.000000 UpyTest-3.1.1/thonnycontrib/docs/res/l1test_icon.png
--rw-rw-r--   0 idtaleb   (1000) idtaleb   (1000)     2086 2023-03-15 10:38:40.000000 UpyTest-3.1.1/thonnycontrib/docs/res/l1test_icon_old.png
--rw-rw-r--   0 idtaleb   (1000) idtaleb   (1000)      628 2023-04-23 12:41:34.000000 UpyTest-3.1.1/thonnycontrib/docs/res/outline_class.png
--rw-rw-r--   0 idtaleb   (1000) idtaleb   (1000)      578 2023-04-23 12:41:32.000000 UpyTest-3.1.1/thonnycontrib/docs/res/outline_method.gif
--rw-rw-r--   0 idtaleb   (1000) idtaleb   (1000)     1213 2023-03-15 10:38:40.000000 UpyTest-3.1.1/thonnycontrib/docs/res/passed.png
--rw-rw-r--   0 idtaleb   (1000) idtaleb   (1000)     1531 2023-03-15 10:38:40.000000 UpyTest-3.1.1/thonnycontrib/docs/res/pending_icon.png
--rw-rw-r--   0 idtaleb   (1000) idtaleb   (1000)      997 2023-06-21 22:19:21.000000 UpyTest-3.1.1/thonnycontrib/docs/res/restart_icon.png
--rw-rw-r--   0 idtaleb   (1000) idtaleb   (1000)     2282 2023-03-15 10:38:40.000000 UpyTest-3.1.1/thonnycontrib/docs/res/test_only_btn.png
--rw-rw-r--   0 idtaleb   (1000) idtaleb   (1000)     1073 2023-03-15 10:38:40.000000 UpyTest-3.1.1/thonnycontrib/docs/res/warning.png
-drwxrwxr-x   0 idtaleb   (1000) idtaleb   (1000)        0 2023-06-24 23:05:20.405857 UpyTest-3.1.1/thonnycontrib/docstring_generator/
--rw-rw-r--   0 idtaleb   (1000) idtaleb   (1000)        0 2023-03-15 10:38:40.000000 UpyTest-3.1.1/thonnycontrib/docstring_generator/__init__.py
--rw-rw-r--   0 idtaleb   (1000) idtaleb   (1000)     8660 2023-06-24 13:42:03.000000 UpyTest-3.1.1/thonnycontrib/docstring_generator/doc_generator.py
--rw-rw-r--   0 idtaleb   (1000) idtaleb   (1000)     7134 2023-03-15 10:38:40.000000 UpyTest-3.1.1/thonnycontrib/docstring_generator/doc_template.py
--rw-rw-r--   0 idtaleb   (1000) idtaleb   (1000)     1469 2023-06-23 23:48:13.000000 UpyTest-3.1.1/thonnycontrib/environement_vars.py
--rw-rw-r--   0 idtaleb   (1000) idtaleb   (1000)     3756 2023-06-23 23:49:24.000000 UpyTest-3.1.1/thonnycontrib/exceptions.py
-drwxrwxr-x   0 idtaleb   (1000) idtaleb   (1000)        0 2023-06-24 23:05:20.405857 UpyTest-3.1.1/thonnycontrib/l1test_configuration/
--rw-rw-r--   0 idtaleb   (1000) idtaleb   (1000)        0 2023-03-15 10:38:40.000000 UpyTest-3.1.1/thonnycontrib/l1test_configuration/__init__.py
--rw-rw-r--   0 idtaleb   (1000) idtaleb   (1000)     2575 2023-04-02 02:23:42.000000 UpyTest-3.1.1/thonnycontrib/l1test_configuration/l1test_options.py
-drwxrwxr-x   0 idtaleb   (1000) idtaleb   (1000)        0 2023-06-24 23:05:20.405857 UpyTest-3.1.1/thonnycontrib/l1test_frontend/
--rw-rw-r--   0 idtaleb   (1000) idtaleb   (1000)      708 2023-06-24 22:52:29.000000 UpyTest-3.1.1/thonnycontrib/l1test_frontend/__init__.py
--rw-rw-r--   0 idtaleb   (1000) idtaleb   (1000)     2504 2023-03-15 10:38:40.000000 UpyTest-3.1.1/thonnycontrib/l1test_frontend/l1test_error_view.py
--rw-rw-r--   0 idtaleb   (1000) idtaleb   (1000)     2768 2023-06-24 15:25:01.000000 UpyTest-3.1.1/thonnycontrib/l1test_frontend/l1test_reporter.py
--rw-rw-r--   0 idtaleb   (1000) idtaleb   (1000)    17790 2023-06-24 18:09:36.000000 UpyTest-3.1.1/thonnycontrib/l1test_frontend/l1test_runner.py
--rw-rw-r--   0 idtaleb   (1000) idtaleb   (1000)    36633 2023-06-24 19:59:14.000000 UpyTest-3.1.1/thonnycontrib/l1test_frontend/l1test_treeview.py
--rw-rw-r--   0 idtaleb   (1000) idtaleb   (1000)     3544 2023-06-24 22:57:49.000000 UpyTest-3.1.1/thonnycontrib/l1test_frontend/outlines.py
--rw-rw-r--   0 idtaleb   (1000) idtaleb   (1000)     9423 2023-06-24 22:56:36.000000 UpyTest-3.1.1/thonnycontrib/plugin_loader.py
--rw-rw-r--   0 idtaleb   (1000) idtaleb   (1000)     2401 2023-06-24 04:10:46.000000 UpyTest-3.1.1/thonnycontrib/properties.py
-drwxrwxr-x   0 idtaleb   (1000) idtaleb   (1000)        0 2023-06-24 23:05:20.409857 UpyTest-3.1.1/thonnycontrib/tests/
--rw-rw-r--   0 idtaleb   (1000) idtaleb   (1000)        0 2023-03-15 10:38:42.000000 UpyTest-3.1.1/thonnycontrib/tests/__init__.py
--rw-rw-r--   0 idtaleb   (1000) idtaleb   (1000)      348 2023-03-15 10:38:42.000000 UpyTest-3.1.1/thonnycontrib/tests/backend_mock.py
--rw-rw-r--   0 idtaleb   (1000) idtaleb   (1000)     1980 2023-03-15 10:38:42.000000 UpyTest-3.1.1/thonnycontrib/tests/test_doc_generator.py
--rw-rw-r--   0 idtaleb   (1000) idtaleb   (1000)     4848 2023-06-24 02:33:48.000000 UpyTest-3.1.1/thonnycontrib/tests/tests_example_no_expected.py
--rw-rw-r--   0 idtaleb   (1000) idtaleb   (1000)    14741 2023-06-24 02:34:31.000000 UpyTest-3.1.1/thonnycontrib/tests/tests_example_with_exception.py
--rw-rw-r--   0 idtaleb   (1000) idtaleb   (1000)    18496 2023-06-24 02:34:31.000000 UpyTest-3.1.1/thonnycontrib/tests/tests_example_with_expected.py
--rw-rw-r--   0 idtaleb   (1000) idtaleb   (1000)     9827 2023-03-15 10:38:42.000000 UpyTest-3.1.1/thonnycontrib/tests/tests_l1TestRunner.py
--rw-rw-r--   0 idtaleb   (1000) idtaleb   (1000)     6392 2023-06-23 23:27:45.000000 UpyTest-3.1.1/thonnycontrib/tests/tests_test_finder.py
--rw-rw-r--   0 idtaleb   (1000) idtaleb   (1000)    12629 2023-06-24 02:34:31.000000 UpyTest-3.1.1/thonnycontrib/tests/tests_view.py
--rw-rw-r--   0 idtaleb   (1000) idtaleb   (1000)    21712 2023-06-24 03:26:11.000000 UpyTest-3.1.1/thonnycontrib/utils.py
+drwxrwxr-x   0 idtaleb   (1000) idtaleb   (1000)        0 2023-06-25 22:08:24.033028 UpyTest-3.1.2/
+-rw-rw-r--   0 idtaleb   (1000) idtaleb   (1000)      694 2023-06-25 22:08:24.029028 UpyTest-3.1.2/PKG-INFO
+drwxrwxr-x   0 idtaleb   (1000) idtaleb   (1000)        0 2023-06-25 22:08:24.021028 UpyTest-3.1.2/UpyTest.egg-info/
+-rw-rw-r--   0 idtaleb   (1000) idtaleb   (1000)      694 2023-06-25 22:08:23.000000 UpyTest-3.1.2/UpyTest.egg-info/PKG-INFO
+-rw-rw-r--   0 idtaleb   (1000) idtaleb   (1000)     2351 2023-06-25 22:08:23.000000 UpyTest-3.1.2/UpyTest.egg-info/SOURCES.txt
+-rw-rw-r--   0 idtaleb   (1000) idtaleb   (1000)        1 2023-06-25 22:08:23.000000 UpyTest-3.1.2/UpyTest.egg-info/dependency_links.txt
+-rw-rw-r--   0 idtaleb   (1000) idtaleb   (1000)       14 2023-06-25 22:08:23.000000 UpyTest-3.1.2/UpyTest.egg-info/requires.txt
+-rw-rw-r--   0 idtaleb   (1000) idtaleb   (1000)       14 2023-06-25 22:08:23.000000 UpyTest-3.1.2/UpyTest.egg-info/top_level.txt
+-rw-rw-r--   0 idtaleb   (1000) idtaleb   (1000)       38 2023-06-25 22:08:24.033028 UpyTest-3.1.2/setup.cfg
+-rw-rw-r--   0 idtaleb   (1000) idtaleb   (1000)     1985 2023-06-25 22:08:20.000000 UpyTest-3.1.2/setup.py
+drwxrwxr-x   0 idtaleb   (1000) idtaleb   (1000)        0 2023-06-25 22:08:24.025028 UpyTest-3.1.2/thonnycontrib/
+-rw-rw-r--   0 idtaleb   (1000) idtaleb   (1000)      947 2023-06-24 22:43:54.000000 UpyTest-3.1.2/thonnycontrib/ThonnyLogsGenerator.py
+-rw-rw-r--   0 idtaleb   (1000) idtaleb   (1000)        0 2023-06-24 22:52:20.000000 UpyTest-3.1.2/thonnycontrib/__init__.py
+drwxrwxr-x   0 idtaleb   (1000) idtaleb   (1000)        0 2023-06-25 22:08:24.025028 UpyTest-3.1.2/thonnycontrib/backend/
+-rw-rw-r--   0 idtaleb   (1000) idtaleb   (1000)        0 2023-03-15 10:38:40.000000 UpyTest-3.1.2/thonnycontrib/backend/__init__.py
+-rw-rw-r--   0 idtaleb   (1000) idtaleb   (1000)    16304 2023-06-24 19:59:14.000000 UpyTest-3.1.2/thonnycontrib/backend/ast_parser.py
+-rw-rw-r--   0 idtaleb   (1000) idtaleb   (1000)    35328 2023-06-25 21:33:06.000000 UpyTest-3.1.2/thonnycontrib/backend/doctest_parser.py
+-rw-rw-r--   0 idtaleb   (1000) idtaleb   (1000)     5028 2023-06-24 15:10:56.000000 UpyTest-3.1.2/thonnycontrib/backend/evaluator.py
+-rw-rw-r--   0 idtaleb   (1000) idtaleb   (1000)     4503 2023-06-25 22:01:28.000000 UpyTest-3.1.2/thonnycontrib/backend/l1test_backend.py
+-rw-rw-r--   0 idtaleb   (1000) idtaleb   (1000)     6541 2023-06-24 18:11:15.000000 UpyTest-3.1.2/thonnycontrib/backend/test_finder.py
+drwxrwxr-x   0 idtaleb   (1000) idtaleb   (1000)        0 2023-06-25 22:08:24.025028 UpyTest-3.1.2/thonnycontrib/backend/verdicts/
+-rw-rw-r--   0 idtaleb   (1000) idtaleb   (1000)     2057 2023-06-24 19:29:56.000000 UpyTest-3.1.2/thonnycontrib/backend/verdicts/ExampleVerdict.py
+-rw-rw-r--   0 idtaleb   (1000) idtaleb   (1000)      496 2023-06-24 18:12:47.000000 UpyTest-3.1.2/thonnycontrib/backend/verdicts/ExceptionVerdict.py
+-rw-rw-r--   0 idtaleb   (1000) idtaleb   (1000)      733 2023-06-24 18:13:06.000000 UpyTest-3.1.2/thonnycontrib/backend/verdicts/FailedVerdict.py
+-rw-rw-r--   0 idtaleb   (1000) idtaleb   (1000)      637 2023-06-24 19:25:27.000000 UpyTest-3.1.2/thonnycontrib/backend/verdicts/FailedWhenExceptionExpectedVerdict.py
+-rw-rw-r--   0 idtaleb   (1000) idtaleb   (1000)      450 2023-06-24 18:12:56.000000 UpyTest-3.1.2/thonnycontrib/backend/verdicts/PassedVerdict.py
+-rw-rw-r--   0 idtaleb   (1000) idtaleb   (1000)      377 2023-06-24 18:13:00.000000 UpyTest-3.1.2/thonnycontrib/backend/verdicts/SetupVerdict.py
+-rw-rw-r--   0 idtaleb   (1000) idtaleb   (1000)        0 2023-06-24 02:35:02.000000 UpyTest-3.1.2/thonnycontrib/backend/verdicts/__init__.py
+drwxrwxr-x   0 idtaleb   (1000) idtaleb   (1000)        0 2023-06-25 22:08:24.025028 UpyTest-3.1.2/thonnycontrib/docs/
+-rw-rw-r--   0 idtaleb   (1000) idtaleb   (1000)        0 2023-03-15 10:38:40.000000 UpyTest-3.1.2/thonnycontrib/docs/__init__.py
+drwxrwxr-x   0 idtaleb   (1000) idtaleb   (1000)        0 2023-06-25 22:08:24.029028 UpyTest-3.1.2/thonnycontrib/docs/res/
+-rw-rw-r--   0 idtaleb   (1000) idtaleb   (1000)      912 2023-06-21 22:17:10.000000 UpyTest-3.1.2/thonnycontrib/docs/res/error_icon.png
+-rw-rw-r--   0 idtaleb   (1000) idtaleb   (1000)     1275 2023-03-15 10:38:40.000000 UpyTest-3.1.2/thonnycontrib/docs/res/failed.png
+-rw-rw-r--   0 idtaleb   (1000) idtaleb   (1000)     1468 2023-06-25 02:50:15.000000 UpyTest-3.1.2/thonnycontrib/docs/res/l1test_debug.png
+-rw-rw-r--   0 idtaleb   (1000) idtaleb   (1000)     2130 2023-03-15 10:38:40.000000 UpyTest-3.1.2/thonnycontrib/docs/res/l1test_icon.png
+-rw-rw-r--   0 idtaleb   (1000) idtaleb   (1000)     2086 2023-03-15 10:38:40.000000 UpyTest-3.1.2/thonnycontrib/docs/res/l1test_icon_old.png
+-rw-rw-r--   0 idtaleb   (1000) idtaleb   (1000)      628 2023-04-23 12:41:34.000000 UpyTest-3.1.2/thonnycontrib/docs/res/outline_class.png
+-rw-rw-r--   0 idtaleb   (1000) idtaleb   (1000)      578 2023-04-23 12:41:32.000000 UpyTest-3.1.2/thonnycontrib/docs/res/outline_method.gif
+-rw-rw-r--   0 idtaleb   (1000) idtaleb   (1000)     1213 2023-03-15 10:38:40.000000 UpyTest-3.1.2/thonnycontrib/docs/res/passed.png
+-rw-rw-r--   0 idtaleb   (1000) idtaleb   (1000)     1531 2023-03-15 10:38:40.000000 UpyTest-3.1.2/thonnycontrib/docs/res/pending_icon.png
+-rw-rw-r--   0 idtaleb   (1000) idtaleb   (1000)      997 2023-06-21 22:19:21.000000 UpyTest-3.1.2/thonnycontrib/docs/res/restart_icon.png
+-rw-rw-r--   0 idtaleb   (1000) idtaleb   (1000)     2282 2023-03-15 10:38:40.000000 UpyTest-3.1.2/thonnycontrib/docs/res/test_only_btn.png
+-rw-rw-r--   0 idtaleb   (1000) idtaleb   (1000)     1073 2023-03-15 10:38:40.000000 UpyTest-3.1.2/thonnycontrib/docs/res/warning.png
+drwxrwxr-x   0 idtaleb   (1000) idtaleb   (1000)        0 2023-06-25 22:08:24.029028 UpyTest-3.1.2/thonnycontrib/docstring_generator/
+-rw-rw-r--   0 idtaleb   (1000) idtaleb   (1000)        0 2023-03-15 10:38:40.000000 UpyTest-3.1.2/thonnycontrib/docstring_generator/__init__.py
+-rw-rw-r--   0 idtaleb   (1000) idtaleb   (1000)     8660 2023-06-24 13:42:03.000000 UpyTest-3.1.2/thonnycontrib/docstring_generator/doc_generator.py
+-rw-rw-r--   0 idtaleb   (1000) idtaleb   (1000)     7134 2023-03-15 10:38:40.000000 UpyTest-3.1.2/thonnycontrib/docstring_generator/doc_template.py
+-rw-rw-r--   0 idtaleb   (1000) idtaleb   (1000)     1315 2023-06-25 20:12:20.000000 UpyTest-3.1.2/thonnycontrib/environement_vars.py
+-rw-rw-r--   0 idtaleb   (1000) idtaleb   (1000)     3756 2023-06-23 23:49:24.000000 UpyTest-3.1.2/thonnycontrib/exceptions.py
+drwxrwxr-x   0 idtaleb   (1000) idtaleb   (1000)        0 2023-06-25 22:08:24.029028 UpyTest-3.1.2/thonnycontrib/l1test_configuration/
+-rw-rw-r--   0 idtaleb   (1000) idtaleb   (1000)        0 2023-03-15 10:38:40.000000 UpyTest-3.1.2/thonnycontrib/l1test_configuration/__init__.py
+-rw-rw-r--   0 idtaleb   (1000) idtaleb   (1000)     2575 2023-04-02 02:23:42.000000 UpyTest-3.1.2/thonnycontrib/l1test_configuration/l1test_options.py
+drwxrwxr-x   0 idtaleb   (1000) idtaleb   (1000)        0 2023-06-25 22:08:24.029028 UpyTest-3.1.2/thonnycontrib/l1test_frontend/
+-rw-rw-r--   0 idtaleb   (1000) idtaleb   (1000)      708 2023-06-24 22:52:29.000000 UpyTest-3.1.2/thonnycontrib/l1test_frontend/__init__.py
+-rw-rw-r--   0 idtaleb   (1000) idtaleb   (1000)     2507 2023-06-25 03:08:15.000000 UpyTest-3.1.2/thonnycontrib/l1test_frontend/l1test_error_view.py
+-rw-rw-r--   0 idtaleb   (1000) idtaleb   (1000)     2756 2023-06-25 13:23:15.000000 UpyTest-3.1.2/thonnycontrib/l1test_frontend/l1test_reporter.py
+-rw-rw-r--   0 idtaleb   (1000) idtaleb   (1000)    23408 2023-06-25 22:07:30.000000 UpyTest-3.1.2/thonnycontrib/l1test_frontend/l1test_runner.py
+-rw-rw-r--   0 idtaleb   (1000) idtaleb   (1000)    36550 2023-06-25 20:32:06.000000 UpyTest-3.1.2/thonnycontrib/l1test_frontend/l1test_treeview.py
+-rw-rw-r--   0 idtaleb   (1000) idtaleb   (1000)     3523 2023-06-25 21:48:20.000000 UpyTest-3.1.2/thonnycontrib/l1test_frontend/outlines.py
+-rw-rw-r--   0 idtaleb   (1000) idtaleb   (1000)     7310 2023-06-25 21:56:55.000000 UpyTest-3.1.2/thonnycontrib/plugin_loader.py
+-rw-rw-r--   0 idtaleb   (1000) idtaleb   (1000)     2432 2023-06-25 02:35:31.000000 UpyTest-3.1.2/thonnycontrib/properties.py
+drwxrwxr-x   0 idtaleb   (1000) idtaleb   (1000)        0 2023-06-25 22:08:24.029028 UpyTest-3.1.2/thonnycontrib/tests/
+-rw-rw-r--   0 idtaleb   (1000) idtaleb   (1000)        0 2023-03-15 10:38:42.000000 UpyTest-3.1.2/thonnycontrib/tests/__init__.py
+-rw-rw-r--   0 idtaleb   (1000) idtaleb   (1000)      348 2023-03-15 10:38:42.000000 UpyTest-3.1.2/thonnycontrib/tests/backend_mock.py
+-rw-rw-r--   0 idtaleb   (1000) idtaleb   (1000)     1980 2023-03-15 10:38:42.000000 UpyTest-3.1.2/thonnycontrib/tests/test_doc_generator.py
+-rw-rw-r--   0 idtaleb   (1000) idtaleb   (1000)     4848 2023-06-24 02:33:48.000000 UpyTest-3.1.2/thonnycontrib/tests/tests_example_no_expected.py
+-rw-rw-r--   0 idtaleb   (1000) idtaleb   (1000)    14741 2023-06-24 02:34:31.000000 UpyTest-3.1.2/thonnycontrib/tests/tests_example_with_exception.py
+-rw-rw-r--   0 idtaleb   (1000) idtaleb   (1000)    18496 2023-06-24 02:34:31.000000 UpyTest-3.1.2/thonnycontrib/tests/tests_example_with_expected.py
+-rw-rw-r--   0 idtaleb   (1000) idtaleb   (1000)     9799 2023-06-25 13:23:15.000000 UpyTest-3.1.2/thonnycontrib/tests/tests_l1TestRunner.py
+-rw-rw-r--   0 idtaleb   (1000) idtaleb   (1000)     6392 2023-06-23 23:27:45.000000 UpyTest-3.1.2/thonnycontrib/tests/tests_test_finder.py
+-rw-rw-r--   0 idtaleb   (1000) idtaleb   (1000)    12629 2023-06-24 02:34:31.000000 UpyTest-3.1.2/thonnycontrib/tests/tests_view.py
+-rw-rw-r--   0 idtaleb   (1000) idtaleb   (1000)    18919 2023-06-25 22:06:41.000000 UpyTest-3.1.2/thonnycontrib/utils.py
```

### Comparing `UpyTest-3.1.1/PKG-INFO` & `UpyTest-3.1.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: UpyTest
-Version: 3.1.1
+Version: 3.1.2
 Summary: A plug-in which adds a test framework
 Home-page: https://gitlab.univ-lille.fr/reda.idtaleb.etu/thonny_test_framework
 Author: Réda Id-taleb
 Platform: Windows
 Platform: macOS
 Platform: Linux
 Classifier: Topic :: Education :: Testing
```

### Comparing `UpyTest-3.1.1/UpyTest.egg-info/PKG-INFO` & `UpyTest-3.1.2/UpyTest.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: UpyTest
-Version: 3.1.1
+Version: 3.1.2
 Summary: A plug-in which adds a test framework
 Home-page: https://gitlab.univ-lille.fr/reda.idtaleb.etu/thonny_test_framework
 Author: Réda Id-taleb
 Platform: Windows
 Platform: macOS
 Platform: Linux
 Classifier: Topic :: Education :: Testing
```

### Comparing `UpyTest-3.1.1/UpyTest.egg-info/SOURCES.txt` & `UpyTest-3.1.2/UpyTest.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -23,14 +23,15 @@
 thonnycontrib/backend/verdicts/FailedWhenExceptionExpectedVerdict.py
 thonnycontrib/backend/verdicts/PassedVerdict.py
 thonnycontrib/backend/verdicts/SetupVerdict.py
 thonnycontrib/backend/verdicts/__init__.py
 thonnycontrib/docs/__init__.py
 thonnycontrib/docs/res/error_icon.png
 thonnycontrib/docs/res/failed.png
+thonnycontrib/docs/res/l1test_debug.png
 thonnycontrib/docs/res/l1test_icon.png
 thonnycontrib/docs/res/l1test_icon_old.png
 thonnycontrib/docs/res/outline_class.png
 thonnycontrib/docs/res/outline_method.gif
 thonnycontrib/docs/res/passed.png
 thonnycontrib/docs/res/pending_icon.png
 thonnycontrib/docs/res/restart_icon.png
```

### Comparing `UpyTest-3.1.1/setup.py` & `UpyTest-3.1.2/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -27,15 +27,15 @@
     return py_packs | other_packs
 
 setupdir = os.path.dirname(__file__)
 
 
 setup(
     name="UpyTest",
-    version="3.1.1",
+    version="3.1.2",
     author="Réda Id-taleb",
     description="A plug-in which adds a test framework",
     long_description="""A plug-in for Thonny which allows you to test your doc examples
  
 More info: https://gitlab.univ-lille.fr/reda.idtaleb.etu/thonny_test_framework""",
     url="https://gitlab.univ-lille.fr/reda.idtaleb.etu/thonny_test_framework",
 #    keywords="IDE education programming tests in documentation",
```

### Comparing `UpyTest-3.1.1/thonnycontrib/ThonnyLogsGenerator.py` & `UpyTest-3.1.2/thonnycontrib/ThonnyLogsGenerator.py`

 * *Files identical despite different names*

### Comparing `UpyTest-3.1.1/thonnycontrib/backend/ast_parser.py` & `UpyTest-3.1.2/thonnycontrib/backend/ast_parser.py`

 * *Files identical despite different names*

### Comparing `UpyTest-3.1.1/thonnycontrib/backend/doctest_parser.py` & `UpyTest-3.1.2/thonnycontrib/backend/doctest_parser.py`

 * *Files 0% similar despite different names*

```diff
@@ -356,18 +356,18 @@
                                     expected_result=want, lineno=self.lineno)   
             else: # forcément une erreur de compilation ou encore une erreur de runtime
                 # si c'est une erreur `CompilationError` alors on récupère seulement sa représentation      
                 if isinstance(e, CompilationError):   # if CompilationError -> ExceptionTest verdict
                     return ExceptionVerdict(self.filename, tested_line=self.source.strip(), 
                                             expected_result=want, lineno=self.lineno, error_details=str(e))
                 else: # sinon on doit chercher la dernière exception. 
-                    failure_msg = "Instead, it raises :\n%s" % (get_last_exception(sys.exc_info())) 
+                    failure_msg = "Instead, it raises : %s()" % (e.__class__.__name__) 
                     return FailedWhenExceptionExpectedVerdict(self.filename, tested_line=self.source.strip(), 
-                                expected_result=want,lineno=self.lineno, failure_message=failure_msg) 
-    
+                                expected_result=want,lineno=self.lineno, failure_message=failure_msg)     
+
     def __build_exception_verdict(self, exception_msg, want):
         """
         Returns an exception verdict with the given exception message. 
 
         Args:
             exception_msg (str): The exception message
             want (str): The want of the Example.
```

### Comparing `UpyTest-3.1.1/thonnycontrib/backend/evaluator.py` & `UpyTest-3.1.2/thonnycontrib/backend/evaluator.py`

 * *Files identical despite different names*

### Comparing `UpyTest-3.1.1/thonnycontrib/backend/l1test_backend.py` & `UpyTest-3.1.2/thonnycontrib/backend/l1test_backend.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,77 +1,61 @@
 import os
 from types import ModuleType
 
 from .test_finder import FindSelectedL1DoctestStrategy
 from ..exceptions import BackendException
 from ..environement_vars import *
 from .evaluator import Evaluator 
-from thonny.common import ToplevelCommand, ToplevelResponse
+from thonny.common import ToplevelCommand, ToplevelResponse, InlineCommand
 from ..properties import BACKEND_COMMAND, L1TEST_EXCEPTION, VERDICTS
-# Ce n'est pas une API publique
 from thonny.plugins.cpython_backend.cp_back import (
     Executor,
     MainCPythonBackend
 )
 import thonny.plugins.cpython_backend.cp_back
 import pickle
 
 BACKEND: MainCPythonBackend = thonny.plugins.cpython_backend.cp_back.get_backend()
-
-def _cmd_l1test(cmd: ToplevelCommand) -> ToplevelResponse:   
-    """
-    Cette fonction est invoquée lorsque un événement de type `ToplevelCommand` (associé 
-    à la commande L1test) est récupéré.
-    
-    Args: 
-        cmd(ToplevelCommand): L'événement `ToplevelCommand` associé à la commande L1test.
-        
-    Returns:
-        ToplevelResponse: un événement de type ToplveleResponse qui contiendra la réponse
-        renvoyé par `L1TestExecutor.execute_source()`.
-    """ 
-    response: ToplevelResponse = BACKEND._execute_file(cmd, L1TestExecutor)
-    return response  
  
 class L1TestExecutor(Executor):
     def execute_source(self, source:str, filename:str, mode:str, ast_postprocessors):  
         """Cette fonction est invoquée par la méthode `BACKEND._execute_file(cmd, L1TestExecutor)`
         située en haut de ce fichier.
 
         Returns:
             dict: doit retourner, obligatoirement, un dictionnaire dont les données sont séralisées.
         """
         assert mode == "exec"
         try:
             evaluator = Evaluator(filename, source)
-            
-            is_selected = eval(os.environ.get(IS_SELECTED_VAR))
-            if is_selected: # si un seul test a été ciblé
-                selected_line: int = int(os.environ.get(SELECTED_LINE_VAR))
+            selected_line: int = os.environ.get(SELECTED_LINE_VAR)
+            if selected_line: # si un seul test a été ciblé
+                selected_line = int(selected_line)
                 evaluator.set_finder_strategy(FindSelectedL1DoctestStrategy(selected_line))
             
             verdicts = evaluator.evaluate()
             
             # on récupère la valeur de l'option qui indique si on doit importer le module dans le shell
             import_module_option = eval(os.environ.get(IMPORT_MODULE_VAR)) 
             # importation du module dans le shell.
             if import_module_option: 
                 # importation du module dans le shell.
                 self._import_module_in_shell(evaluator.get_module())                                                
             
             # Sérialiser les données en binaires. 
             serialized_data = pickle.dumps(verdicts)
-            
             # The serialized data should necessary be a dictionary and the returned statement should
             # also be a dictionary
             return {VERDICTS: serialized_data}
         except BaseException as e:
             # pas besoin de sérialiser la valeur du dictionaire car il conteint que des types primitifs.
             return {L1TEST_EXCEPTION: self._build_backend_exception(e, str(e))}
     
+
+    
     def _import_module_in_shell(self, module:ModuleType):
         """
         Imports the given `module` into Thonny's shell.
         
         Args:
             module (ModuleType): the module to be imported into the shell.
         """
@@ -93,15 +77,30 @@
         """
         return {
                 "type_name": exception.__class__.__name__,
                 "message": message, 
                 "prefix": exception.get_prefix_message() if isinstance(exception, BackendException) \
                                                          else None
             }
+ 
+def _cmd_l1test(cmd: ToplevelCommand) -> ToplevelResponse:   
+    """
+    Cette fonction est invoquée lorsque un événement de type `ToplevelCommand` (associé 
+    à la commande L1test) est récupéré.
     
+    Args: 
+        cmd(ToplevelCommand): L'événement `ToplevelCommand` associé à la commande L1test.
+        
+    Returns:
+        ToplevelResponse: un événement de type ToplveleResponse qui contiendra la réponse
+        renvoyé par `L1TestExecutor.execute_source()`.
+    """ 
+    response: ToplevelResponse = BACKEND._execute_file(cmd, L1TestExecutor)
+    return response  
+   
 def load_plugin(): 
     """
         Cette fonction est importante car il est appelée par Thonny à son intialisation.
         
         Cette fonction doit déclarer les commandes magiques et leurs handlers.
     """
     BACKEND.add_command(BACKEND_COMMAND, _cmd_l1test)
```

### Comparing `UpyTest-3.1.1/thonnycontrib/backend/test_finder.py` & `UpyTest-3.1.2/thonnycontrib/backend/test_finder.py`

 * *Files identical despite different names*

### Comparing `UpyTest-3.1.1/thonnycontrib/backend/verdicts/ExampleVerdict.py` & `UpyTest-3.1.2/thonnycontrib/backend/verdicts/ExampleVerdict.py`

 * *Files identical despite different names*

### Comparing `UpyTest-3.1.1/thonnycontrib/backend/verdicts/FailedVerdict.py` & `UpyTest-3.1.2/thonnycontrib/backend/verdicts/FailedVerdict.py`

 * *Files identical despite different names*

### Comparing `UpyTest-3.1.1/thonnycontrib/backend/verdicts/FailedWhenExceptionExpectedVerdict.py` & `UpyTest-3.1.2/thonnycontrib/backend/verdicts/FailedWhenExceptionExpectedVerdict.py`

 * *Files identical despite different names*

### Comparing `UpyTest-3.1.1/thonnycontrib/docs/res/error_icon.png` & `UpyTest-3.1.2/thonnycontrib/docs/res/error_icon.png`

 * *Files identical despite different names*

### Comparing `UpyTest-3.1.1/thonnycontrib/docs/res/failed.png` & `UpyTest-3.1.2/thonnycontrib/docs/res/failed.png`

 * *Files identical despite different names*

### Comparing `UpyTest-3.1.1/thonnycontrib/docs/res/l1test_icon.png` & `UpyTest-3.1.2/thonnycontrib/docs/res/l1test_icon.png`

 * *Files identical despite different names*

### Comparing `UpyTest-3.1.1/thonnycontrib/docs/res/l1test_icon_old.png` & `UpyTest-3.1.2/thonnycontrib/docs/res/l1test_icon_old.png`

 * *Files identical despite different names*

### Comparing `UpyTest-3.1.1/thonnycontrib/docs/res/outline_class.png` & `UpyTest-3.1.2/thonnycontrib/docs/res/outline_class.png`

 * *Files identical despite different names*

### Comparing `UpyTest-3.1.1/thonnycontrib/docs/res/outline_method.gif` & `UpyTest-3.1.2/thonnycontrib/docs/res/outline_method.gif`

 * *Files identical despite different names*

### Comparing `UpyTest-3.1.1/thonnycontrib/docs/res/passed.png` & `UpyTest-3.1.2/thonnycontrib/docs/res/passed.png`

 * *Files identical despite different names*

### Comparing `UpyTest-3.1.1/thonnycontrib/docs/res/pending_icon.png` & `UpyTest-3.1.2/thonnycontrib/docs/res/pending_icon.png`

 * *Files identical despite different names*

### Comparing `UpyTest-3.1.1/thonnycontrib/docs/res/restart_icon.png` & `UpyTest-3.1.2/thonnycontrib/docs/res/restart_icon.png`

 * *Files identical despite different names*

### Comparing `UpyTest-3.1.1/thonnycontrib/docs/res/test_only_btn.png` & `UpyTest-3.1.2/thonnycontrib/docs/res/test_only_btn.png`

 * *Files identical despite different names*

### Comparing `UpyTest-3.1.1/thonnycontrib/docs/res/warning.png` & `UpyTest-3.1.2/thonnycontrib/docs/res/warning.png`

 * *Files identical despite different names*

### Comparing `UpyTest-3.1.1/thonnycontrib/docstring_generator/doc_generator.py` & `UpyTest-3.1.2/thonnycontrib/docstring_generator/doc_generator.py`

 * *Files identical despite different names*

### Comparing `UpyTest-3.1.1/thonnycontrib/docstring_generator/doc_template.py` & `UpyTest-3.1.2/thonnycontrib/docstring_generator/doc_template.py`

 * *Files identical despite different names*

### Comparing `UpyTest-3.1.1/thonnycontrib/environement_vars.py` & `UpyTest-3.1.2/thonnycontrib/environement_vars.py`

 * *Files 5% similar despite different names*

```diff
@@ -11,18 +11,14 @@
 """
 
 # `IMPORT_MODULE_VAR` est une variable d'environnment qui stocke la valeur de l'option
 # `l1test_options.IMPORT_MODULE` qui indique si oui(`True`) ou non(`False`) qu'il faut
 # importer le module executé dans le shell.
 IMPORT_MODULE_VAR = "import_module"
 
-# `IS_SELECTED_VAR` est une variable d'environnment qui stocke si oui(`True`) ou non(`False`)
-# on a ciblé un seul test
-IS_SELECTED_VAR = "is_selected"
-
 # `SELECTED_LINE_VAR` est une variable d'environnment qui stocke le numéro de ligne de 
 # la fonction séléctionnée si `IS_SELECTED_VAR` est à True, sinon elle stocke `None`.
 SELECTED_LINE_VAR = "selected_line"
 
 # `TEST_ONLY_VAR` est une variable d'environnment qui stocke si oui(`True`) ou non(`False`)
 # on a cliqué sur le button qui lancent les fonction qui possède le `@test_only`
 TEST_ONLY_VAR = "test_only"
```

### Comparing `UpyTest-3.1.1/thonnycontrib/exceptions.py` & `UpyTest-3.1.2/thonnycontrib/exceptions.py`

 * *Files identical despite different names*

### Comparing `UpyTest-3.1.1/thonnycontrib/l1test_configuration/l1test_options.py` & `UpyTest-3.1.2/thonnycontrib/l1test_configuration/l1test_options.py`

 * *Files identical despite different names*

### Comparing `UpyTest-3.1.1/thonnycontrib/l1test_frontend/__init__.py` & `UpyTest-3.1.2/thonnycontrib/l1test_frontend/__init__.py`

 * *Files identical despite different names*

### Comparing `UpyTest-3.1.1/thonnycontrib/l1test_frontend/l1test_error_view.py` & `UpyTest-3.1.2/thonnycontrib/l1test_frontend/l1test_error_view.py`

 * *Files 9% similar despite different names*

```diff
@@ -13,26 +13,24 @@
             horizontal_scrollbar_style=scrollbar_style("Horizontal"),
             horizontal_scrollbar_class=ui_utils.AutoScrollbar,
             read_only=True,
             wrap="word",
             font="TkDefaultFont",
         )
         self.workbench = thonny.get_workbench()
-        font = tk_font.Font(
-                    family=get_font_family_option(),
-                    size=get_font_size_option()+3,
-                    weight="bold"
-                )
+        title_font = tk_font.Font(family=get_font_family_option(),
+                                  size=get_font_size_option(),
+                                  weight="bold")
         
         self.text.tag_config("green", foreground="darkgreen")
         self.text.tag_config("red", foreground="red")
         self.text.tag_config("darkred", foreground="#d41919")
         self.text.tag_config("yellow", foreground="yellow")  
         
-        self.text.tag_configure("title", font=font)              
+        self.text.tag_configure("title", font=title_font)              
     
     def append_text(self, chars, tags=()):
         self.text.direct_insert("end", chars, tags=tags)
         self._update_font(font_family_opt="io_font_family")
 
     def write(self, data):
         self.text.set_content(data)
@@ -57,13 +55,13 @@
 class AssistantRstText(rst_utils.RstText):
     def configure_tags(self):
         super().configure_tags()
         self.workbench = thonny.get_workbench()
         font = tk_font.Font(
                     family=get_font_family_option(option="io_font_family"),
                     size=get_font_size_option(),
-                    underline=1
+                    underline=True
                 )
         
         self.tag_configure("url", font=font)
 
         self.tag_raise("sel")
```

### Comparing `UpyTest-3.1.1/thonnycontrib/l1test_frontend/l1test_reporter.py` & `UpyTest-3.1.2/thonnycontrib/l1test_frontend/l1test_reporter.py`

 * *Files 1% similar despite different names*

```diff
@@ -27,15 +27,15 @@
             prefix_info (str, optional): the title preceding the error message. 
             Defaults to CANNOT_RUN_TESTS_MSG.
             color (str, optional): the color of the whole content. Defaults to "red".
         """
         self.__error_view.clear()
         if title:
             title = title if title.endswith("\n") else title + "\n"
-            self.__error_view.append_text(title+"\n", tags=("darkred", "title"))
+            self.__error_view.append_text(title, tags=("darkred", "title"))
 
         hyperlink_error = format_filename_to_hyperlink(error_msg)
 
         if hyperlink_error: 
             self.__error_view.append_rst(hyperlink_error) # hyperlink doit être ajouté en mode RST
             error_msg = remove_url_part(error_msg) 
             self.__error_view.append_text(error_msg, tags=color) # le reste du message est ajouté en mode texte
@@ -53,13 +53,13 @@
     
     def set_treeview_class(self, treeview_class):
         self.__treeview_class = treeview_class   
     
     def get_error_view_class(self, error_view_class):
         self.__error_view_class = error_view_class      
     
-    def get_l1test_treeview(self) -> L1TestTreeView:
+    def get_treeview(self) -> L1TestTreeView:
         return self.__treeview    
     
     def get_l1test_error_view(self) -> L1TestErrorView:
         return self.__error_view
```

### Comparing `UpyTest-3.1.1/thonnycontrib/l1test_frontend/l1test_runner.py` & `UpyTest-3.1.2/thonnycontrib/l1test_frontend/l1test_runner.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,21 +1,26 @@
 from collections import namedtuple
 from typing import List
+
+from ..utils import clear_env_vars
 from ..backend.ast_parser import L1DocTest
-from thonny.workbench import WorkbenchEvent
-from ..utils import send_to_backend
-from ..backend.verdicts.ExampleVerdict import ExampleVerdict
-from ..environement_vars import IS_SELECTED_VAR
 from ..exceptions import *
+from ..environement_vars import *
 from .l1test_reporter import *
 from ..properties import *
 from thonny.common import ToplevelResponse, InlineResponse
+from thonny.workbench import WorkbenchEvent
 from thonnycontrib import l1test_frontend 
+from thonny.editors import EditorNotebook
+from thonny import editors
+import thonny
 from ..ThonnyLogsGenerator import log_in_thonny
-import pickle, inspect, thonny, ast, time
+import pickle, inspect, thonny, time
+from ..l1test_configuration import l1test_options 
+
 
 # ErrorMsg déclare deux champs : le préfixe et le message d'erreur
 # le préfix est juste le titre qui précède le message d'erreur sur la Error view
 ErrorMsg = namedtuple("ErrorMsg", "title msg")
 
 # Le nom de l'event qui lance le redémarrage du backend thonny
 BACKEND_RESTART_EVENT = "BackendRestart"
@@ -51,144 +56,235 @@
         
         thonny.get_workbench().bind(L1TREE_VIEW_EVENT, self.show_right_view, True)
         
         # Quand le backend est redémarré en thonny nous invoquons la méthode 
         # `self._on_restart_backend()`
         thonny.get_workbench().bind(BACKEND_RESTART_EVENT, self._on_restart_backend, True)
     
+    def run_l1test(self, selected_line: int=None):
+        """
+        Run the L1Test plugin by sending a command to the l1test_backend. This method checks
+        if the file is saved and if the editor is empty. If the file is not saved or the editor
+        then it will display an error message on the ErrorView. Otherwise, it will send a command 
+        to the backend to run the tests.
+        Args:
+            is_selected (bool): Set as True if only one method is selected to run
+                            it's tests.
+            selected_line (int): The number of the selected line. 
+            Default is 0 if no line is selected.
+        """
+        try:
+            editor: EditorNotebook = get_workbench().get_editor_notebook()
+            # si aucun editeur n'est ouvert sur le workbench
+            if not editor.get_current_editor():
+                raise NoEditorFoundException("No editor found !\n\nPlease open an editor before running the tests.")
+            
+            # cette ligne demande de sauver le fichier s'il n'a pas encore été sauvé sur
+            # la machine. Si le fichier est déjà sauvé, il va permettre d'enregistrer la nouvelle
+            # version du fichier.
+            filename = editors.get_saved_current_script_filename(force=True)
+            
+            # si le filename est null alors le fichier n'a  pas été sauvé sur machine.  
+            # Ce cas survient quand l'utilisatur quitte la fenetre de sauvegarde sans sauver le fichier.
+            if not filename: 
+                msg = "The file is not saved.\n\nConsider to save the file before running the tests."
+                raise NotSavedFileException(msg)
+
+            if not editor.get_current_editor_content().strip():  # L'éditeur est vide. 
+                # on a pas envie d'envoyer une commande au backend si le fichier est vide.
+                # Dans tous les cas y a rien à tester.
+                raise EmptyEditorException("The editor is empty!\n")
+            
+            # si on est là alors le fichier est bien sauvegardé et contient quelque chose.
+            self.request_backend(selected_line)         
+        except FrontendException as e: # on catche que les exception coté view
+            self.terminate_running()
+            self.set_has_exception(True) 
+            self.clean_error_view()
+            self.show_right_view(error_msg=str(e))
+    
+    def request_backend(self, selected_line:int):
+        """Allows to execute the `L1test` magic command. 
+        
+        There's two cases : 
+        1. if the `L1test` is invoked for the first so the command is sent to 
+        backend to be executed by the thonny's runner. 
+        2. if the `L1test` is invoked while it's always running, so the L1TestRunner
+        will force to stop the backend before resending the command to the thonny's 
+        runner. 
+        
+        Note: there's a delay of 1 second after the backend is restarted to allow 
+        the proxy to be initialized.
+
+        Args:
+            is_selected (bool): Set as True if only one method is selected to run
+                            it's tests.
+            selected_line (int): The number of the selected line.
+        """
+        treeview = self._reporter.get_treeview()
+        if self.is_running(): # si le plugin est en cours d'execution et pas encore terminé
+            thonny.get_runner().cmd_stop_restart() # invoke le restart backend
+            
+            # on affiche sur la treeview comme quoi un restart backend forcé est en cours
+            treeview.insert_in_header("Force to restart backend ...", 
+                                      clear=True, tags=("red"), image="restart_icon.png")
+            
+            # on indique que l'état du plugin n'est plus en execution
+            self.set_is_running(False)
+            
+            # On donne un peu du temps au proxy pour se réinitialiser.
+            # La valeur choisit n'affecte pas le temps d'execution du plugin.
+            time.sleep(1) 
+            
+        # On invoque la commande magique L1test
+        try:
+            self.set_is_running()
+            self.__request_backend(selected_line=selected_line)
+        except:
+            self.set_is_running(False)
+            treeview.insert_in_header("Coudn't restart the backend.\nPlease restart with the 'Stop' button !", 
+                                      clear=True, tags=("red"), image="error_icon.png")
+
+        clear_env_vars(IMPORT_MODULE_VAR, SELECTED_LINE_VAR)
+        
+    def __request_backend(self, command_name=BACKEND_COMMAND, selected_line:int=None):
+        """
+        Sends a command to the Thonny's backend to execute the current script.
+        The name of the command must starts with a uppercase.    
+        
+        Please note that `thonny.get_runner.execute_current()` will consider 
+        all the current script, and it builds a `ToplevelCommand` automatically. 
+        So in the case if you don't want to consider all the script but only a 
+        selected method, you should set the number of the selected line. 
+        
+        The value of the selected line is stored in an environnement variable to be
+        shared with the backend. The handler of the command(l1test_backend) can access 
+        this environnement variables to decide if the `Evaluator` should run all the 
+        tests or only for the selected line.
+
+        Note: the value of the environnement variable should be a string.
+        For example : 
+        ```py
+        os.environ["is_selected"] = str(is_selected) # the value should always be a string 
+        ```
+        
+        In the handler of the command :
+        ```py
+        def _cmd_l1test(cmd: ToplevelCommand):         
+            is_selected: bool = eval(os.environ.get("is_selected"))
+        ```
+                    
+        Note : when a new command is called in Thonny it triggers a partial 
+        "restart" of the backend before processing the new command. Thonny does 
+        this to force stop the current process and start a new process for the 
+        new command.
+            
+        Args:
+            command_name (str): A command name , should starts with a upper case. 
+            Defaults to BACKEND_COMMAND.
+            selected_line (int, optional): The number of the selected line. Defaults to None
+            if no line is selected.
+        """ 
+        # on stocke dans une variable d'environnment la valeur de l'option `import_module in shell`.
+        # le l1test backend retrouvera cette valeur pour décider d'importer ou non le module dans le shell.
+        os.environ[IMPORT_MODULE_VAR] = str(l1test_options.get_option(l1test_options.IMPORT_MODULE))
+        
+        if selected_line:
+            os.environ[SELECTED_LINE_VAR] = str(selected_line)
+        
+        # Une fois que execute_current() est executée un restart backend partiel est invoqué
+        # pour un nouveau processus pour la commande passé en paramètre.
+        thonny.get_runner().execute_current(command_name)
+    
     def show_execution_state(self, msg: InlineResponse):
         """
         This function is called when an event of type InlineResponse is received. 
         This function verfies the source of the event. If the source is L1Test so it will access to the 
         received response and then it will show the state of the execution.
         """
-        if msg.get("command_name") == BACKEND_COMMAND:
+        if self._is_relevant_response(msg):
             self.clean_error_view()
 
             state:str = msg.get("state")
 
-            treeview:L1TestTreeView = self._reporter.get_l1test_treeview()
+            treeview:L1TestTreeView = self._reporter.get_treeview()
             treeview.disable_menu()
-             
-            treeview.insert_in_header(L1TEST_IN_PROGRESS, clear=True, tags="blue", image="pending_icon.png")
             
+            treeview.insert_in_header(L1TEST_IN_PROGRESS, clear=True, tags="blue", image="pending_icon.png")
+        
             if state == PENDING_STATE:
                 self.set_pending(True)
                 self.clean_treeview(all=False)
                 source, invite, lineno = msg.get("source"), msg.get("invite"), msg.get("lineno") 
 
                 row_content = "%s for line %s, %s %s" % (state, lineno, invite, source)
                 self.row = treeview.insert_row(text=row_content, open=True, tags=("clickable",), values=lineno)
                 treeview.insert_row(parent=self.row, 
-                                           text="Interrompez avec 'ctrl+c', si ce test prend plus de temps.", 
-                                           tags=("nonClickable", "orange"))
+                                    text="Interrompez avec 'ctrl+c', si ce test prend plus de temps.", 
+                                    tags=("nonClickable", "orange"))
             elif state == EXECUTED_STATE: 
                 treeview.insert_row(parent=self.row, text=state, tags=("nonClickable", "green"))  
             else: # si le state == FINISHED_STATE
-                self.set_pending(False)     
+                self.set_pending(False) 
     
     def report_verdicts(self, msg: ToplevelResponse):     
         """
-            This method is binded to the `TopLevelResponse` event sent by the backend.
-            
-            If this method is triggered so the `msg` parameter will contain the response received 
-            from the backend. Please note that the `TopLevelResponse` event is not necessary sent 
-            by the l1test_backend, but it can be also sent by the Shell. The shell contains an 
-            internal infinite loop that waits for commands and sends the responses periodically.
-            
-            This method verify the source of the `TopLevelResponse` event. If the source is 
-            l1test_backend so it checks the recieved response if it contains exception or not. 
-            If the response contains an exception so the according error will be displayed in 
-            error view. Otherwise the response contains the verdicts of the tests and will be shown 
-            on the treeview.
-            
-            Note: The data is deserialized before displaying it on the view.
+        This method is binded to the `TopLevelResponse` event sent by the backend.
+        
+        If this method is triggered so the `msg` parameter will contain the response received 
+        from the backend. Please note that the `TopLevelResponse` event is not necessary sent 
+        by the l1test_backend, but it can be also sent by the Shell. The shell contains an 
+        internal infinite loop that waits for commands and sends the responses periodically.
+        
+        This method verify the source of the `TopLevelResponse` event. If the source is 
+        l1test_backend so it checks the recieved response if it contains exception or not. 
+        If the response contains an exception so the according error will be displayed in 
+        error view. Otherwise the response contains the verdicts of the tests and will be shown 
+        on the treeview.
+        
+        Note: The data is deserialized before displaying it on the view.
         """   
        
         # On vérifie si le TopLevelRespone reçu est envoyé par le l1test_backend 
-        if msg.get("command_name") == BACKEND_COMMAND:
-            verdicts, error_msg = None, ErrorMsg(title=None, msg=None)
-           
-            self.clean_error_view()         
-            # We check if the backend encountered an exception
-            if msg.get(L1TEST_EXCEPTION):
-                error_msg = self.__handle_raised_exception(msg.get(L1TEST_EXCEPTION))
-            
-            if not self.is_pending() and self.is_running():
-                self.clean_treeview()
-                
-                l1test_treeview:L1TestTreeView = self._reporter.get_l1test_treeview()
-                l1test_treeview.enable_menu()    
-                
-                if msg.get(VERDICTS): # We check if the response contains the "verdicts" attribute 
-                    self.set_has_exception(False)
-                    received_verdicts = msg.get(VERDICTS)
-
-                    # deserialization of the data
-                    verdicts: List[L1DocTest] = pickle.loads(received_verdicts)                    
-                    log_in_thonny(verdicts, eval(os.environ.get(IS_SELECTED_VAR)))
+        if self._is_relevant_response(msg):
+            verdicts, error_msg = self.__get_verdicts_and_error(msg)
             self.show_right_view(verdicts=verdicts, error_msg=error_msg.msg, error_title=error_msg.title)
         else:
             # Le TopLevelReponse reçu ne nous intéresse pas.
             return 
         # On indique l'état de l'execution du la commande comme terminée
         self.terminate_running()
     
-    def show_verdicts(self, test_results:List[L1DocTest]):
+    def __get_verdicts_and_error(self, msg:ToplevelResponse):
         """
-        Report the verdicts on the view.
-
-        Args:
-            test_results (dict): The recieved verdicts from the backend.
-        """
-        self._reporter.display_tests_results(test_results) 
-    
-    def send_to_backend(self, is_selected, selected_line):
-        """Allows to execute the `L1test` magic command. 
+        Returns the l1doctests and the error message from the received response. 
+        If the response contains an exception so the error message will be returned. In this
+        case the l1doctests will be None. Reverse is true, if the response does not contain the
+        error message so the l1doctests will be returned and the error message will be None.
         
-        There's two cases : 
-        1. if the `L1test` is invoked for the first so the command is sent to 
-        backend to be executed by the thonny's runner. 
-        2. if the `L1test` is invoked while it's always running, so the L1TestRunner
-        will force to stop the backend before resending the command to the thonny's 
-        runner. Note: there's a delay of 0.3 second after the backend is restarted to allow 
-        the proxy to be initialized.
-
         Args:
-            is_selected (bool): Set as True if only one method is selected to run
-                            it's tests.
-            selected_line (int): The number of the selected line.
+            msg (ToplevelResponse): The received response from the backend.
+
+        Returns:
+            a tuple of (l1doctests, error_msg)
         """
-        treeview = self._reporter.get_l1test_treeview()
-        if self.is_running(): # si le plugin est en cours d'execution et pas encore terminé
-            thonny.get_runner().cmd_stop_restart() # invoke le restart backend
-            
-            # on affiche sur la treeview comme quoi un restart backend forcé est en cours
-            treeview.insert_in_header("Force to restart backend ...", 
-                                      clear=True, tags=("red"), image="restart_icon.png")
-            
-            # on indique que l'état du plugin n'est plus en execution
-            self.set_is_running(False)
-            
-            # On donne un peu du temps au proxy pour se réinitialiser.
-            # La valeur choisit n'affecte pas le temps d'execution du plugin.
-            time.sleep(1) 
-            
-        # On invoque la commande magique L1test
-        try:
-            self.__send_to_backend(is_selected, selected_line)
-        except:
-            self.set_is_running(False)
-            treeview.insert_in_header("Coudn't restart the backend.\nPlease restart with the 'Stop' button !", 
-                                      clear=True, tags=("red"), image="error_icon.png")
+        l1doctests, error_msg = None, ErrorMsg(title=None, msg=None)
+        self.clean_error_view()
+        if msg.get(L1TEST_EXCEPTION):
+            error_msg = self.__handle_raised_exception(msg.get(L1TEST_EXCEPTION))
+        if not self.is_pending() and self.is_running():
+            self.clean_treeview()
+            self._reporter.get_treeview().enable_menu()
+            if msg.get(VERDICTS):
+                self.set_has_exception(False)
+                received_verdicts = msg.get(VERDICTS)
+                l1doctests: List[L1DocTest] = pickle.loads(received_verdicts)                    
+                log_in_thonny(l1doctests, os.environ.get(SELECTED_LINE_VAR) != None)
+        return l1doctests, error_msg
     
-    def __send_to_backend(self, is_selected, selected_line):
-        self.set_is_running()
-        send_to_backend(is_selected=is_selected, selected_line=selected_line)
-        
     def __handle_raised_exception(self, exception: dict) -> ErrorMsg:
         """
         This function handles the raised exception by returning a tuple containing
         a prefix message and the exception message.
 
         The prefix refers to the title shown on the ErrorView. If you want to remove 
         the title, you should specify the prefix as an empty string. If you don't 
@@ -232,19 +328,15 @@
             list[BackendException]: Returns a list of the backend exception classes.
         """
         import thonnycontrib.exceptions as exceptions
         backend_exceptions = []
         for name, obj in inspect.getmembers(exceptions):
             if inspect.isclass(obj) and issubclass(obj, exceptions.BackendException):
                 backend_exceptions.append(obj)
-        return backend_exceptions
-    
-    def show_errors(self, exception_msg, title=None):
-        title = CANNOT_RUN_TESTS_MSG if title is None else title
-        self._reporter.display_error_msg(exception_msg, title=title)    
+        return backend_exceptions   
     
     def _on_restart_backend(self, event: WorkbenchEvent):
         """
         This function is called when the backend of thonny is restared. The restarting
         of the backend generates a `BackendRestart` event and this event can 
         be generated either by  the red `Stop/Restart backend` button in Thonny's 
         toolbar or by invoking a new command. 
@@ -280,65 +372,89 @@
             if event.get("full"):
                 self.terminate_running()
                 self.clean_treeview()          
             else:       
                 # on vérifie si le l1test a été invoqué
                 if self.is_running(): 
                     self.clean_treeview()
-                    treeview:L1TestTreeView = self._reporter.get_l1test_treeview()
+                    treeview:L1TestTreeView = self._reporter.get_treeview()
                     treeview.insert_in_header("Starting executing tests ...", clear=True, tags="blue", 
                                               image="pending_icon.png")
                 else: # probablement une autre commande a déclenché le Restart du backend -> on fait rien
                     pass
         self.show_right_view()
-     
+    
     def show_right_view(self, event:WorkbenchEvent=None, verdicts=None, error_msg:str=None, error_title:str=None, both=False):
         """
             Displays either the L1TestTreeView or the L1TestErrorView. 
             It depends on the execution state of the l1test plugin. 
             
             If an error was raised by the plugin then only the Error view will be displayed.
         """
+        exception_details = False
         if event and event.get("sequence") == L1TREE_VIEW_EVENT:
-            possible_keys = ["sequence", "has_exception", "both", "verdicts", "error_msg", "error_title"]
+            possible_keys = ["sequence", "exception_details", "both", "verdicts", "error_msg", "error_title"]
             assert any(key in possible_keys for key in event.__dict__.keys())
-            if event.get("has_exception") != None:
-                has_exception = event.has_exception
-                self._has_exception = has_exception
+            if event.get("exception_details") != None:
+                exception_details = event.exception_details
             if event.get("verdicts") != None:
                 verdicts = event.verdicts
             if event.get("error_msg") != None:
                 error_msg = event.error_msg 
             if event.get("error_title") != None: 
                 error_title = event.error_title
             if event.get("both") != None: 
                 both = event.both
-        if (self._has_exception):
+        if (self._has_exception or exception_details):
             if error_msg:
                 self.show_errors(exception_msg=error_msg, title=error_title)
             if not both:
-                self._reporter.get_l1test_treeview().hide_view()
+                self._reporter.get_treeview().hide_view()
             else:
-                self._reporter.get_l1test_treeview().show_view()
+                self._reporter.get_treeview().show_view()
             self._reporter.get_l1test_error_view().show_view()
         else:
             self.clean_error_view()
             if verdicts:
                 self.show_verdicts(verdicts)
             if not both:
                 self._reporter.get_l1test_error_view().hide_view()
             else:
                 self._reporter.get_l1test_error_view().show_view()
-            self._reporter.get_l1test_treeview().show_view()
-       
+            self._reporter.get_treeview().show_view()
+    
+    def show_verdicts(self, test_results:List[L1DocTest]):
+        """
+        Report the verdicts on the view.
+
+        Args:
+            test_results (dict): The recieved verdicts from the backend.
+        """
+        self._reporter.display_tests_results(test_results) 
+    
+    def show_errors(self, exception_msg, title=None):
+        """
+        Report the error message on the error view.
+        
+        Args:
+            exception_msg (str): The error message to display.
+            title (str, optional): The title of the error message. Defaults to None.
+        """
+        title = CANNOT_RUN_TESTS_MSG if title is None else title
+        self._reporter.display_error_msg(exception_msg, title=title) 
+    
+    def _is_relevant_response(self, msg: ToplevelResponse, cmd_name:str=BACKEND_COMMAND):
+       """Returns True if the TopLevelResponse is relevant to the l1test plugin."""         
+       return msg.get("command_name") == cmd_name
+    
     def clean_error_view(self):
         self._reporter.get_l1test_error_view().clear()
                
     def clean_treeview(self, all=True): 
-        self._reporter.get_l1test_treeview().clear_tree(clear_all=all)
+        self._reporter.get_treeview().clear_tree(clear_all=all)
          
     def set_is_running(self, value=True):
         self._is_l1test_running = value
     
     def is_running(self):
         return self._is_l1test_running
```

### Comparing `UpyTest-3.1.1/thonnycontrib/l1test_frontend/l1test_treeview.py` & `UpyTest-3.1.2/thonnycontrib/l1test_frontend/l1test_treeview.py`

 * *Files 1% similar despite different names*

```diff
@@ -696,32 +696,32 @@
             if focus == self.selected_item:
                 # Item is already selected, so toggle the selection state
                 if self.treeview.selection():
                     self.selected_item = None
                     self._remove_highlight_selection_effect()
                     self._highlight_line_on_editor(-1, code_view)
                     if get_option(EXCEPTION_DETAIL):
-                        self.workbench.event_generate(L1TREE_VIEW_EVENT, has_exception=False)
+                        self.workbench.event_generate(L1TREE_VIEW_EVENT, exception_details=False)
                 else:
                     self._show_highlight_selection_effect()
             else:
                 # Item is not selected, so select it and remove the previous selection
                 if self.selected_item:
                     self.selected_item = None
                     self._remove_highlight_selection_effect()
                     self._highlight_line_on_editor(-1, code_view)
                     if get_option(EXCEPTION_DETAIL):
-                        self.workbench.event_generate(L1TREE_VIEW_EVENT, has_exception=False)
+                        self.workbench.event_generate(L1TREE_VIEW_EVENT, exception_details=False)
                 
                 self._show_highlight_selection_effect()
                 self.selected_item = focus 
                 
                 if get_option(EXCEPTION_DETAIL): 
                     if ExceptionVerdict.__name__ in values:
-                        self.workbench.event_generate(L1TREE_VIEW_EVENT, has_exception=True, both=True,
+                        self.workbench.event_generate(L1TREE_VIEW_EVENT, exception_details=True, both=True,
                                                     error_msg=values[-1], error_title=item["text"])
                            
                 lineno = values[0]
                 self._highlight_line_on_editor(lineno, code_view)
                 self.workbench.event_generate(
                     "OutlineDoubleClick", item_text=self.treeview.item(self.treeview.focus(), option="text")
                 )
@@ -746,15 +746,14 @@
         """
         if clear:
             self.header_bar.direct_delete("1.0", tk.END)
         if image:
             if isinstance(image, str):
                 image = self.get_icon(image)
             self.header_bar.image_create(tk.END, image=image)
-            #setattr(self, get_basename(image), photo_image)  # save the image in the treeview
             text = " " + text
         self.header_bar.direct_insert(tk.END, text, tags=tags)
         self.resize_header_bar()
            
     def is_treeview_cleared(self):
         return len(self.treeview.get_children()) == 0
```

### Comparing `UpyTest-3.1.1/thonnycontrib/l1test_frontend/outlines.py` & `UpyTest-3.1.2/thonnycontrib/l1test_frontend/outlines.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 from typing import List
 import re
 from thonny import get_workbench
 from functools import partial
 from ..properties import PLUGIN_NAME
 import tkinter as tk
-from ..utils import get_basename, get_photoImage 
+from ..utils import  get_photoImage 
 from thonnycontrib import l1test_frontend 
 
 _OUTLINE_REGEX = r"\s*(?P<type>def|class)[ ]+(?P<name>[\w]+)"
 
 class OutlinedNode():
     def __init__(self, type:str, name:str, lineno:int) -> None:
         self.__type = type
@@ -85,13 +85,12 @@
 
 def run_outlined_test(lineno:int):
     """
     Cette fonction est invoquée quand le button `Run test for selected function`
     suite à un clique droit sur une ligne du fichier.
     Cette fonction permet d'envoyer au l1test_backend la commande L1test avec en argument
     is_selected=True.
-    
     """
-    from ..plugin_loader import _send_to_l1test_backend
-    _send_to_l1test_backend(is_selected=True, selected_line=lineno)
+    from thonnycontrib.l1test_frontend import get_l1test_runner
+    get_l1test_runner().run_l1test(selected_line=lineno)
```

### Comparing `UpyTest-3.1.1/thonnycontrib/plugin_loader.py` & `UpyTest-3.1.2/thonnycontrib/plugin_loader.py`

 * *Files 22% similar despite different names*

```diff
@@ -3,93 +3,54 @@
 from thonny.editors import  EditorNotebook
 from thonny import editors
 from thonny.ui_utils import select_sequence
 from .l1test_frontend.outlines import run_outlined_test
 from .docstring_generator.doc_generator import DocGenerator
 from .l1test_frontend.l1test_reporter import L1TestErrorView, L1TestTreeView
 from .exceptions import *
-from .properties import  ERROR_VIEW_LABEL, PLUGIN_NAME, CANNOT_GENERATE_THE_DOCSTRING
+from .properties import  (
+    ERROR_VIEW_LABEL, 
+    DEBUG_NAME, 
+    PLUGIN_NAME, 
+    CANNOT_GENERATE_THE_DOCSTRING
+)
 from .utils import (
     get_focused_writable_text,
     get_selected_line, 
-    assert_one_line_is_selected
+    assert_one_line_is_selected,
+    get_image_path
 )
 from .l1test_configuration import l1test_options
 from .l1test_frontend import get_l1test_runner
 from .l1test_frontend import get_outliner
 from .environement_vars import *
 from thonny.editors import EditorCodeViewText
-
+from thonny.plugins.debugger import Debugger, get_current_debugger
+    
 def run_all_tests():
     """
     Cette fonction est invoquée quand le button `l1test` est cliqué.
     Cette fonction permet d'envoyer au l1test_backend la commande L1test.
     """
-    _send_to_l1test_backend()
-
+    get_l1test_runner().run_l1test()
+ 
 def run_selected_test():
     """
     Cette fonction est invoquée quand le button `Run test for selected function`
     suite à un clique droit sur une ligne du fichier.
     Cette fonction permet d'envoyer au l1test_backend la commande L1test avec en argument
     is_selected=True.
-    
-    Raises:
-        CannotSelectSeveralLines: si plusieurs lignes sont séléctionnées.
     """
     try:
         assert_one_line_is_selected()
         lineno = get_selected_line(get_focused_writable_text())
-        _send_to_l1test_backend(is_selected=True, selected_line=lineno)
+        get_l1test_runner().run_l1test(selected_line=lineno)
     except CannotSelectSeveralLines as e:
-        l1test_runner = get_l1test_runner()
-        l1test_runner.set_has_exception(True) 
-        l1test_runner.clean_error_view()
-        l1test_runner.show_right_view(error_msg=str(e))
-
-def _send_to_l1test_backend(is_selected: bool=False, selected_line: int=0):
-    """
-        Send a command to the l1test_backend.
-        Args:
-            is_selected (bool): Set as True if only one method is selected to run
-                            it's tests.
-            selected_line (int): The number of the selected line.
-    """
-    l1test_runner = get_l1test_runner()
-    try:
-        editor: EditorNotebook = get_workbench().get_editor_notebook()
-        # si aucun editeur n'est ouvert sur le workbench
-        if not editor.get_current_editor():
-            raise NoEditorFoundException("No editor found !\n\nPlease open an editor before running the tests.")
-        
-        # cette ligne demande de sauver le fichier s'il n'a pas encore été sauvé sur
-        # la machine. Si le fichier est déjà sauvé, il va permettre d'enregistrer la nouvelle
-        # version du fichier.
-        filename = editors.get_saved_current_script_filename(force=True)
-        
-        # si le filename est null alors le fichier n'a  pas été sauvé sur machine.  
-        # Ce cas survient quand l'utilisatur quitte la fenetre de sauvegarde sans sauver le fichier.
-        if not filename: 
-            msg = "The file is not saved.\n\nConsider to save the file before running the tests."
-            raise NotSavedFileException(msg)
-
-        if not editor.get_current_editor_content().strip():  # L'éditeur est vide. 
-            # on a pas envie d'envoyer une commande au backend si le fichier est vide.
-            # Dans tous les cas y a rien à tester.
-            raise EmptyEditorException("The editor is empty!\n")
-        
-         # si on est là alors le fichier est bien sauvegardé et contient quelque chose.
-        l1test_runner.send_to_backend(is_selected, selected_line)
-        
-    except FrontendException as e: # on catche que les exception coté view
-        l1test_runner.terminate_running()
-        l1test_runner.set_has_exception(True) 
-        l1test_runner.clean_error_view()
-        l1test_runner.show_right_view(error_msg=str(e))
-       
+        pass # Do nothing here. It's not relevant to show an error message.
+      
 def generate_auto_docstring(event): 
     if _writable_text_is_focused(): # on vérifie si la zone séléctionnée est une zone de l'éditeur
         if l1test_options.get_option(l1test_options.AUTO_GENERATON_DOC): 
             text_widget = get_focused_writable_text()
             lineno = get_selected_line(text_widget) - 1
             __generate_docstring(lineno, text_widget)
             
@@ -157,22 +118,23 @@
 def __init_l1test_commands():
     # Création du button l1test au niveau de la barre des commandes
     get_workbench().add_command(command_id=PLUGIN_NAME,
                                 menu_name=PLUGIN_NAME,  
                                 command_label="Run all tests",
                                 handler=run_all_tests,
                                 include_in_toolbar=True, #j'inclue ici ce bouton dans la toolbar 
-                                image=os.path.join(os.path.dirname(__file__), "docs/res", "l1test_icon.png"),
+                                image=get_image_path("l1test_icon.png"),
                                 caption=PLUGIN_NAME)
     
     # Création du button L1Test dans la barre de menu en haut.  
     get_workbench().add_command(command_id="Run one test",
                                 menu_name=PLUGIN_NAME,  
                                 command_label="Run tests for ...",
                                 handler=run_outlined_test, 
+                                image=get_image_path("l1test_icon.png"),
                                 submenu=get_outliner().get_menu()
     )
     
     # Création du bouton dans le menu 'Edit' pour lancer un seul test d'une seul foncton
     get_workbench().add_command(command_id="function test",
                                 menu_name="edit",  
                                 command_label="Run test for selected function",
```

### Comparing `UpyTest-3.1.1/thonnycontrib/properties.py` & `UpyTest-3.1.2/thonnycontrib/properties.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 PLUGIN_NAME = "L1Test"
+DEBUG_NAME = "L1Test debugger"
 ERROR_VIEW_LABEL = '%s errors' % PLUGIN_NAME
 
 # ici vous pouvez changer la syntaxe du doctest. 
 # version 2022 PJI : Actuellement on garde la syntaxe `$py`.
 L1TEST_SYMBOL = "[$]py"
 # version 2022 avant la rentrée
 L1TEST_SYMBOL1 = "[$][$][$]"
```

### Comparing `UpyTest-3.1.1/thonnycontrib/tests/test_doc_generator.py` & `UpyTest-3.1.2/thonnycontrib/tests/test_doc_generator.py`

 * *Files identical despite different names*

### Comparing `UpyTest-3.1.1/thonnycontrib/tests/tests_example_no_expected.py` & `UpyTest-3.1.2/thonnycontrib/tests/tests_example_no_expected.py`

 * *Files identical despite different names*

### Comparing `UpyTest-3.1.1/thonnycontrib/tests/tests_example_with_exception.py` & `UpyTest-3.1.2/thonnycontrib/tests/tests_example_with_exception.py`

 * *Files identical despite different names*

### Comparing `UpyTest-3.1.1/thonnycontrib/tests/tests_example_with_expected.py` & `UpyTest-3.1.2/thonnycontrib/tests/tests_example_with_expected.py`

 * *Files identical despite different names*

### Comparing `UpyTest-3.1.1/thonnycontrib/tests/tests_l1TestRunner.py` & `UpyTest-3.1.2/thonnycontrib/tests/tests_l1TestRunner.py`

 * *Files 1% similar despite different names*

```diff
@@ -76,15 +76,15 @@
         l1test_runner = L1TestRunner()
         
         # on s'assure que le mock_get_workbench est appelée lors de l'instantiation de L1TestRunner
         mock_get_workbench.assert_called()
         
         # On doit ajouter du faux contenus à la treeview, pour vérifier qu'elle
         # sera vraiment nettoyée après le restart_backend.
-        l1test_treeview = l1test_runner.get_reporter().get_l1test_treeview()
+        l1test_treeview = l1test_runner.get_reporter().get_treeview()
         treeview = self.__add_fake_row_in_treeview(l1test_treeview)
         
         self.workbench_event.full = True # on suppose que c'est un redémarrage complet
         l1test_runner._on_restart_backend(self.workbench_event)
 
         # on s'assure qu'après le redémarrage complet du backend l'état du `L1TestRunner` est déclaré 
         # comme terminé.
@@ -115,15 +115,15 @@
         l1test_runner.set_is_running()
         # On s'assure que le `L1TestRunner` est en execution.
         self.assertTrue(l1test_runner.is_running())
         
         self.workbench_event.full = False # on suppose que c'est un redémarrage partiel
         l1test_runner._on_restart_backend(self.workbench_event)
 
-        treeview = l1test_runner.get_reporter().get_l1test_treeview().get_treeview()
+        treeview = l1test_runner.get_reporter().get_treeview().get_treeview()
         # on s'assure qu'il existe rien dans la treeview
         self.assertTrue(len(treeview.get_children()) == 0)
 
     @patch("thonny.get_workbench", return_value=MockWorkbench())
     def test_restart_backend_event_when_partial_restart_and_when_l1test_is_invoked_case2(self,  
         mock_get_workbench: MagicMock
     ):
@@ -144,15 +144,15 @@
         # on suppose que la commande L1test a été invoquée
         l1test_runner.set_is_running()
         # On s'assure que le `L1TestRunner` est en execution.
         self.assertTrue(l1test_runner.is_running())
         
         # On doit ajouter du faux contenus à la treeview, pour vérifier que son contenue
         # sera effacée et que le message "Executing tests in progress ..." apparaîtera à la place
-        l1test_treeview = l1test_runner.get_reporter().get_l1test_treeview()
+        l1test_treeview = l1test_runner.get_reporter().get_treeview()
         treeview = self.__add_fake_row_in_treeview(l1test_treeview)
         
         self.workbench_event.full = False # on suppose que c'est un redémarrage partiel
         l1test_runner._on_restart_backend(self.workbench_event)
         
         # On s'assure qu'il y a rien dans la treeview
         self.assertTrue(len(treeview.get_children()) == 0)
@@ -174,15 +174,15 @@
         mock_get_workbench.assert_called()
         
         # On s'assure que le `L1TestRunner` n'est pas en execution.
         self.assertFalse(l1test_runner.is_running())
         
         # On doit ajouter du faux contenus à la treeview, pour vérifier que le contenu
         # de la treeview ne sera pas du tout effacée.
-        l1test_treeview = l1test_runner.get_reporter().get_l1test_treeview()
+        l1test_treeview = l1test_runner.get_reporter().get_treeview()
         row_text = "A fake content"
         treeview = self.__add_fake_row_in_treeview(l1test_treeview, row_text=row_text)
         
         self.workbench_event.full = False # on suppose que c'est un redémarrage partiel
         l1test_runner._on_restart_backend(self.workbench_event)
         
         # on s'assure que le contenu de la treeview reste le même
```

### Comparing `UpyTest-3.1.1/thonnycontrib/tests/tests_test_finder.py` & `UpyTest-3.1.2/thonnycontrib/tests/tests_test_finder.py`

 * *Files identical despite different names*

### Comparing `UpyTest-3.1.1/thonnycontrib/tests/tests_view.py` & `UpyTest-3.1.2/thonnycontrib/tests/tests_view.py`

 * *Files identical despite different names*

### Comparing `UpyTest-3.1.1/thonnycontrib/utils.py` & `UpyTest-3.1.2/thonnycontrib/utils.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,87 +1,27 @@
 from io import StringIO
 from tkinter import Text, ttk
 from types import ModuleType
-from thonny import rst_utils, get_runner, get_workbench
+from thonny import rst_utils, get_workbench
 from setuptools import find_packages
 from thonnycontrib.exceptions import CannotImportModuleException, CannotSelectSeveralLines, CompilationError
 from .properties import BACKEND_COMMAND 
-from .l1test_configuration import l1test_options 
 from .environement_vars import *
 import os, re, ast, traceback, textwrap, tkinter as tk
 import thonny
-
-def send_to_backend(command_name=BACKEND_COMMAND, is_selected=False, selected_line:int=0):
-    """
-        Sends a command to the Thonny's shell to execute the current script.
-        The name of the command must starts with a uppercase.    
-
-        When the `is_selected` parameter is False so the `runner` of Thonny is 
-        invoked to use it's method `execute_current()` that takes the name of the 
-        command. 
-        
-        Please note that `execute_current()` will consider all the current script, 
-        and it builds a `ToplevelCommand` automatically. So in the case if you don't 
-        want to consider all the script but only a selected method, you should set 
-        the `is_selected` parameter to True. If setted to True, we set two environement
-        variables containing the value of the `is_selected` parameter and the number 
-        of the selected line so that the `Evaluator` can retrieve this values and it will 
-        recognize if only one test is selected. 
-        
-        Note: the value of the environnement varaible should be a string.
-              
-        The handler of the command(l1test_backend) can access this environnement variables
-        to decide if the `Evaluator` should run all the tests or only for the selected line.
-     
-        For example : 
-        ```py
-        os.environ["is_selected"] = str(is_selected) # the value should always be a string 
-        ```
-         
-        In the handler of the command :
-        ```py
-        def _cmd_l1test(cmd: ToplevelCommand):         
-            is_selected: bool = eval(os.environ.get("is_selected"))
-        ```
-        --------------
-        Note : when a new command is called in Thonny it triggers a partial 
-        "restart" of the backend before processing the new command. Thonny does 
-        this to force stop the current process and start a new process for the 
-        new command.
-        
-    Args:
-        command_name (str): A command name , should starts with a upper case. 
-                        Defaults to BACKEND_COMMAND.
-        is_selected (bool): Set to True if one method is selected to run its tests. 
-                        Defaults to False, so all the tests of the script will be run
-
-    Raises:
-        CannotSelectSeveralLines: if several lines are selected.
-    """ 
-    # on stocke dans une variable d'environnment la valeur de l'option `import_module in shell`.
-    # le l1test backend retrouvera cette valeur pour décider d'importer ou non le module dans le shell.
-    os.environ[IMPORT_MODULE_VAR] = str(l1test_options.get_option(l1test_options.IMPORT_MODULE))
-    
-    os.environ[IS_SELECTED_VAR] = str(is_selected)
-    if (is_selected):
-        os.environ[SELECTED_LINE_VAR] = str(selected_line)
-    
-    # Une fois que execute_current() est executée un restart backend partiel est invoqué
-    # pour un nouveau processus pour la commande passé en paramètre.
-    get_runner().execute_current(command_name)
     
-def wrap(string:str, length=8, break_long_words=False):   
+def wrap(string:str, length=8, break_long_words=False, separator=os.sep):   
     """Wrap a text using the `wraptext` module.
 
     Args:
         string (str): the string to wrap.
         length (int, optional): the min length from which the string will be wrapped. Defaults to 8.
         break_long_words (bool, optional): if False the entire words will not be wrapped
                                         if the words lentgh is more that the given length. Defaults to False.
-
+        separator (str, optional): the separator around which to wrap the filenames.
     Returns:
         str: the wrapped string.
     """
     return '\n'.join(textwrap.wrap(string, length, break_long_words=break_long_words))
 
 def get_all_tree_childrens(tree: ttk.Treeview, node=None):
     """Gets recursivly all the childrens of the given node of the treeview. 
@@ -538,8 +478,15 @@
     Raises:
         AssertionError: If the backend is not initialized.
     """
     from thonny.common import InlineResponse
     import thonnycontrib.backend.l1test_backend
     backend = thonnycontrib.backend.l1test_backend.BACKEND
     assert backend != None
-    backend.send_message(InlineResponse(command_name=command_name, state=state, **options))
+    backend.send_message(InlineResponse(command_name=command_name, state=state, **options))
+
+def clear_env_vars(*vars):
+    """
+    Clears the environnement variables.
+    """
+    for var in vars:
+        os.environ.pop(var, None)
```

