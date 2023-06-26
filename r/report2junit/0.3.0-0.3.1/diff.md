# Comparing `tmp/report2junit-0.3.0.tar.gz` & `tmp/report2junit-0.3.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "report2junit-0.3.0.tar", last modified: Mon Mar  6 09:30:12 2023, max compression
+gzip compressed data, was "report2junit-0.3.1.tar", max compression
```

## Comparing `report2junit-0.3.0.tar` & `report2junit-0.3.1.tar`

### file list

```diff
@@ -1,29 +1,11 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-06 09:30:12.130946 report2junit-0.3.0/
--rw-r--r--   0 runner    (1001) docker     (123)     1052 2023-03-06 09:29:43.000000 report2junit-0.3.0/LICENSE.md
--rw-r--r--   0 runner    (1001) docker     (123)     7273 2023-03-06 09:30:12.130946 report2junit-0.3.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     6573 2023-03-06 09:29:43.000000 report2junit-0.3.0/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      665 2023-03-06 09:29:43.000000 report2junit-0.3.0/pyproject.toml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-06 09:30:12.130946 report2junit-0.3.0/report2junit/
--rw-r--r--   0 runner    (1001) docker     (123)     1480 2023-03-06 09:29:43.000000 report2junit-0.3.0/report2junit/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1307 2023-03-06 09:29:43.000000 report2junit-0.3.0/report2junit/junit.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-06 09:30:12.130946 report2junit-0.3.0/report2junit/reports/
--rw-r--r--   0 runner    (1001) docker     (123)      886 2023-03-06 09:29:43.000000 report2junit-0.3.0/report2junit/reports/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1316 2023-03-06 09:29:43.000000 report2junit-0.3.0/report2junit/reports/cfn_guard.py
--rw-r--r--   0 runner    (1001) docker     (123)     1402 2023-03-06 09:29:43.000000 report2junit-0.3.0/report2junit/reports/cfn_nag.py
--rw-r--r--   0 runner    (1001) docker     (123)     1705 2023-03-06 09:29:43.000000 report2junit-0.3.0/report2junit/reports/junit.py
--rw-r--r--   0 runner    (1001) docker     (123)      328 2023-03-06 09:29:43.000000 report2junit-0.3.0/report2junit/reports/noreport.py
--rw-r--r--   0 runner    (1001) docker     (123)     1347 2023-03-06 09:29:43.000000 report2junit-0.3.0/report2junit/reports/report_factory.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-06 09:30:12.130946 report2junit-0.3.0/report2junit.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     7273 2023-03-06 09:30:11.000000 report2junit-0.3.0/report2junit.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      670 2023-03-06 09:30:12.000000 report2junit-0.3.0/report2junit.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-03-06 09:30:11.000000 report2junit-0.3.0/report2junit.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       51 2023-03-06 09:30:11.000000 report2junit-0.3.0/report2junit.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)       28 2023-03-06 09:30:11.000000 report2junit-0.3.0/report2junit.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       19 2023-03-06 09:30:11.000000 report2junit-0.3.0/report2junit.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      284 2023-03-06 09:30:12.134946 report2junit-0.3.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1219 2023-03-06 09:29:43.000000 report2junit-0.3.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-06 09:30:12.130946 report2junit-0.3.0/tests/
--rw-r--r--   0 runner    (1001) docker     (123)      330 2023-03-06 09:29:43.000000 report2junit-0.3.0/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      203 2023-03-06 09:29:43.000000 report2junit-0.3.0/tests/conftest.py
--rw-r--r--   0 runner    (1001) docker     (123)     2345 2023-03-06 09:29:43.000000 report2junit-0.3.0/tests/test_cli.py
--rw-r--r--   0 runner    (1001) docker     (123)     1989 2023-03-06 09:29:43.000000 report2junit-0.3.0/tests/test_report2junit.py
+-rw-r--r--   0        0        0     1052 2023-06-26 06:53:12.165052 report2junit-0.3.1/LICENSE.md
+-rw-r--r--   0        0        0      902 2023-06-26 06:53:13.145058 report2junit-0.3.1/pyproject.toml
+-rw-r--r--   0        0        0     1457 2023-06-26 06:53:13.145058 report2junit-0.3.1/report2junit/__init__.py
+-rw-r--r--   0        0        0     1307 2023-06-26 06:53:12.169052 report2junit-0.3.1/report2junit/junit.py
+-rw-r--r--   0        0        0      886 2023-06-26 06:53:12.169052 report2junit-0.3.1/report2junit/reports/__init__.py
+-rw-r--r--   0        0        0     1316 2023-06-26 06:53:12.169052 report2junit-0.3.1/report2junit/reports/cfn_guard.py
+-rw-r--r--   0        0        0     1402 2023-06-26 06:53:12.169052 report2junit-0.3.1/report2junit/reports/cfn_nag.py
+-rw-r--r--   0        0        0     1705 2023-06-26 06:53:12.169052 report2junit-0.3.1/report2junit/reports/junit.py
+-rw-r--r--   0        0        0      328 2023-06-26 06:53:12.169052 report2junit-0.3.1/report2junit/reports/noreport.py
+-rw-r--r--   0        0        0     1347 2023-06-26 06:53:12.169052 report2junit-0.3.1/report2junit/reports/report_factory.py
+-rw-r--r--   0        0        0      618 1970-01-01 00:00:00.000000 report2junit-0.3.1/PKG-INFO
```

### Comparing `report2junit-0.3.0/LICENSE.md` & `report2junit-0.3.1/LICENSE.md`

 * *Files identical despite different names*

### Comparing `report2junit-0.3.0/report2junit/__init__.py` & `report2junit-0.3.1/report2junit/__init__.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,16 +1,18 @@
 from typing import Optional, List
 import os.path
 import click
 
-from report2junit.reports import ReportFactory
 from report2junit.junit import JUnitOutput
 from report2junit.reports import AVAILABLE_REPORTS
 
 
+__version__ = "0.3.1"
+
+
 @click.command()
 @click.argument("source-files", nargs=-1)
 @click.option("--destination-file", required=False)
 @click.option("--fail-on-failures/--ignore-failures", default=True)
 def main(
     source_files: List[str], destination_file: Optional[str], fail_on_failures: bool
 ) -> None:
```

### Comparing `report2junit-0.3.0/report2junit/junit.py` & `report2junit-0.3.1/report2junit/junit.py`

 * *Files identical despite different names*

### Comparing `report2junit-0.3.0/report2junit/reports/__init__.py` & `report2junit-0.3.1/report2junit/reports/__init__.py`

 * *Files identical despite different names*

### Comparing `report2junit-0.3.0/report2junit/reports/cfn_guard.py` & `report2junit-0.3.1/report2junit/reports/cfn_guard.py`

 * *Files identical despite different names*

### Comparing `report2junit-0.3.0/report2junit/reports/cfn_nag.py` & `report2junit-0.3.1/report2junit/reports/cfn_nag.py`

 * *Files identical despite different names*

### Comparing `report2junit-0.3.0/report2junit/reports/junit.py` & `report2junit-0.3.1/report2junit/reports/junit.py`

 * *Files identical despite different names*

### Comparing `report2junit-0.3.0/report2junit/reports/report_factory.py` & `report2junit-0.3.1/report2junit/reports/report_factory.py`

 * *Files identical despite different names*

