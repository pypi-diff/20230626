# Comparing `tmp/pytest-fluent-0.0.0.tar.gz` & `tmp/pytest-fluent-0.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pytest-fluent-0.0.0.tar", last modified: Mon Jun 26 08:57:01 2023, max compression
+gzip compressed data, was "pytest-fluent-0.1.0.tar", last modified: Tue Jul 12 10:36:20 2022, max compression
```

## Comparing `pytest-fluent-0.0.0.tar` & `pytest-fluent-0.1.0.tar`

### file list

```diff
@@ -1,23 +1,43 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 08:57:01.256390 pytest-fluent-0.0.0/
--rw-r--r--   0 runner    (1001) docker     (123)     1086 2023-06-26 08:56:49.000000 pytest-fluent-0.0.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    11908 2023-06-26 08:57:01.256390 pytest-fluent-0.0.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    10529 2023-06-26 08:56:49.000000 pytest-fluent-0.0.0/README.md
--rw-r--r--   0 runner    (1001) docker     (123)     2148 2023-06-26 08:56:49.000000 pytest-fluent-0.0.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)      387 2023-06-26 08:57:01.256390 pytest-fluent-0.0.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-26 08:56:49.000000 pytest-fluent-0.0.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 08:57:01.252390 pytest-fluent-0.0.0/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 08:57:01.256390 pytest-fluent-0.0.0/src/pytest_fluent/
--rw-r--r--   0 runner    (1001) docker     (123)      630 2023-06-26 08:56:49.000000 pytest-fluent-0.0.0/src/pytest_fluent/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2315 2023-06-26 08:56:49.000000 pytest-fluent-0.0.0/src/pytest_fluent/additional_information.py
--rw-r--r--   0 runner    (1001) docker     (123)     7708 2023-06-26 08:56:49.000000 pytest-fluent-0.0.0/src/pytest_fluent/content_patcher.py
--rw-r--r--   0 runner    (1001) docker     (123)     1564 2023-06-26 08:56:49.000000 pytest-fluent-0.0.0/src/pytest_fluent/event.py
--rw-r--r--   0 runner    (1001) docker     (123)    15746 2023-06-26 08:56:49.000000 pytest-fluent-0.0.0/src/pytest_fluent/plugin.py
--rw-r--r--   0 runner    (1001) docker     (123)     1465 2023-06-26 08:56:49.000000 pytest-fluent-0.0.0/src/pytest_fluent/setting_file_loader_action.py
--rw-r--r--   0 runner    (1001) docker     (123)     4750 2023-06-26 08:56:49.000000 pytest-fluent-0.0.0/src/pytest_fluent/test_report.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 08:57:01.256390 pytest-fluent-0.0.0/src/pytest_fluent.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    11908 2023-06-26 08:57:01.000000 pytest-fluent-0.0.0/src/pytest_fluent.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      546 2023-06-26 08:57:01.000000 pytest-fluent-0.0.0/src/pytest_fluent.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-26 08:57:01.000000 pytest-fluent-0.0.0/src/pytest_fluent.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       49 2023-06-26 08:57:01.000000 pytest-fluent-0.0.0/src/pytest_fluent.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)      173 2023-06-26 08:57:01.000000 pytest-fluent-0.0.0/src/pytest_fluent.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       14 2023-06-26 08:57:01.000000 pytest-fluent-0.0.0/src/pytest_fluent.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2022-07-12 10:36:20.328379 pytest-fluent-0.1.0/
+drwxrwxrwx   0        0        0        0 2022-07-12 10:36:20.138777 pytest-fluent-0.1.0/.github/
+drwxrwxrwx   0        0        0        0 2022-07-12 10:36:20.231380 pytest-fluent-0.1.0/.github/workflow/
+-rw-rw-rw-   0        0        0      956 2022-07-12 06:21:54.000000 pytest-fluent-0.1.0/.github/workflow/python-publish.yml
+-rw-rw-rw-   0        0        0     1222 2022-07-12 06:45:48.000000 pytest-fluent-0.1.0/.github/workflow/tests.yml
+-rw-rw-rw-   0        0        0     2256 2022-02-16 11:31:14.000000 pytest-fluent-0.1.0/.gitignore
+-rw-rw-rw-   0        0        0     1107 2022-07-12 06:17:08.000000 pytest-fluent-0.1.0/LICENSE
+-rw-rw-rw-   0        0        0     8122 2022-07-12 10:36:20.329380 pytest-fluent-0.1.0/PKG-INFO
+-rw-rw-rw-   0        0        0     6708 2022-07-12 06:45:02.000000 pytest-fluent-0.1.0/README.md
+drwxrwxrwx   0        0        0        0 2022-07-12 10:36:20.255380 pytest-fluent-0.1.0/docs/
+-rw-rw-rw-   0        0        0       90 2022-02-22 07:33:27.000000 pytest-fluent-0.1.0/docs/api.md
+-rw-rw-rw-   0        0        0      110 2022-02-16 11:31:14.000000 pytest-fluent-0.1.0/docs/changelog.md
+-rw-rw-rw-   0        0        0      883 2022-07-12 06:47:47.000000 pytest-fluent-0.1.0/docs/conf.py
+-rw-rw-rw-   0        0        0       84 2022-02-16 11:31:14.000000 pytest-fluent-0.1.0/docs/contributing.md
+-rw-rw-rw-   0        0        0      151 2022-02-16 11:31:14.000000 pytest-fluent-0.1.0/docs/index.md
+-rw-rw-rw-   0        0        0      111 2022-02-16 11:31:14.000000 pytest-fluent-0.1.0/docs/installation.md
+-rw-rw-rw-   0        0        0       99 2022-02-16 11:31:14.000000 pytest-fluent-0.1.0/docs/usage.md
+-rw-rw-rw-   0        0        0      491 2022-07-12 06:57:43.000000 pytest-fluent-0.1.0/pyproject.toml
+-rw-rw-rw-   0        0        0       15 2022-02-16 11:31:14.000000 pytest-fluent-0.1.0/requirements-dev.txt
+-rw-rw-rw-   0        0        0     1836 2022-07-12 10:36:20.332380 pytest-fluent-0.1.0/setup.cfg
+-rw-rw-rw-   0        0        0       41 2022-02-16 11:31:14.000000 pytest-fluent-0.1.0/setup.py
+drwxrwxrwx   0        0        0        0 2022-07-12 10:36:20.142777 pytest-fluent-0.1.0/src/
+drwxrwxrwx   0        0        0        0 2022-07-12 10:36:20.273379 pytest-fluent-0.1.0/src/pytest_fluent/
+-rw-rw-rw-   0        0        0      766 2022-07-12 07:12:47.000000 pytest-fluent-0.1.0/src/pytest_fluent/__init__.py
+-rw-rw-rw-   0        0        0      868 2022-02-16 11:31:14.000000 pytest-fluent-0.1.0/src/pytest_fluent/additional_information.py
+-rw-rw-rw-   0        0        0    11095 2022-07-12 06:58:06.000000 pytest-fluent-0.1.0/src/pytest_fluent/plugin.py
+-rw-rw-rw-   0        0        0     4886 2022-07-12 07:04:52.000000 pytest-fluent-0.1.0/src/pytest_fluent/test_report.py
+drwxrwxrwx   0        0        0        0 2022-07-12 10:36:20.294380 pytest-fluent-0.1.0/src/pytest_fluent.egg-info/
+-rw-rw-rw-   0        0        0     8122 2022-07-12 10:36:19.000000 pytest-fluent-0.1.0/src/pytest_fluent.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      812 2022-07-12 10:36:20.000000 pytest-fluent-0.1.0/src/pytest_fluent.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2022-07-12 10:36:19.000000 pytest-fluent-0.1.0/src/pytest_fluent.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       49 2022-07-12 10:36:19.000000 pytest-fluent-0.1.0/src/pytest_fluent.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0      189 2022-07-12 10:36:19.000000 pytest-fluent-0.1.0/src/pytest_fluent.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       14 2022-07-12 10:36:19.000000 pytest-fluent-0.1.0/src/pytest_fluent.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2022-07-12 10:36:20.325379 pytest-fluent-0.1.0/tests/
+-rw-rw-rw-   0        0        0        0 2022-02-16 11:31:14.000000 pytest-fluent-0.1.0/tests/__init__.py
+-rw-rw-rw-   0        0        0     1571 2022-07-12 06:37:06.000000 pytest-fluent-0.1.0/tests/conftest.py
+-rw-rw-rw-   0        0        0      851 2022-02-16 11:31:14.000000 pytest-fluent-0.1.0/tests/test_additional_information.py
+-rw-rw-rw-   0        0        0     1779 2022-07-12 06:58:05.000000 pytest-fluent-0.1.0/tests/test_addoptions.py
+-rw-rw-rw-   0        0        0     1364 2022-07-12 07:00:18.000000 pytest-fluent-0.1.0/tests/test_fixtures.py
+-rw-rw-rw-   0        0        0     4456 2022-07-12 07:02:21.000000 pytest-fluent-0.1.0/tests/test_reporting.py
+-rw-rw-rw-   0        0        0      245 2022-02-16 11:31:14.000000 pytest-fluent-0.1.0/tests/utility.py
+-rw-rw-rw-   0        0        0     4123 2022-07-12 07:03:08.000000 pytest-fluent-0.1.0/tox.ini
```

### Comparing `pytest-fluent-0.0.0/LICENSE` & `pytest-fluent-0.1.0/LICENSE`

 * *Ordering differences only*

 * *Files 16% similar despite different names*

```diff
@@ -1,21 +1,21 @@
-MIT License
-
-Copyright (c) 2022 Rohde & Schwarz GmbH & Co. KG
-
-Permission is hereby granted, free of charge, to any person obtaining a copy
-of this software and associated documentation files (the "Software"), to deal
-in the Software without restriction, including without limitation the rights
-to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
-copies of the Software, and to permit persons to whom the Software is
-furnished to do so, subject to the following conditions:
-
-The above copyright notice and this permission notice shall be included in all
-copies or substantial portions of the Software.
-
-THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
-IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
-FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
-AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
-LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
-OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
-SOFTWARE.
+MIT License
+
+Copyright (c) 2022 Rohde & Schwarz GmbH & Co. KG
+
+Permission is hereby granted, free of charge, to any person obtaining a copy
+of this software and associated documentation files (the "Software"), to deal
+in the Software without restriction, including without limitation the rights
+to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
+copies of the Software, and to permit persons to whom the Software is
+furnished to do so, subject to the following conditions:
+
+The above copyright notice and this permission notice shall be included in all
+copies or substantial portions of the Software.
+
+THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
+IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
+FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
+AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
+LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
+OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
+SOFTWARE.
```

### Comparing `pytest-fluent-0.0.0/src/pytest_fluent/__init__.py` & `pytest-fluent-0.1.0/src/pytest_fluent/__init__.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,26 +1,29 @@
-"""pytest-fluent-logging."""
-
-from importlib.metadata import PackageNotFoundError, version
-
-from .additional_information import (
-    additional_information_callback,
-    additional_session_information_callback,
-    additional_test_information_callback,
-)
-from .plugin import get_session_uid, get_test_uid
-
-__version__ = "unknown"
-try:
-    __version__ = version(__name__)
-except PackageNotFoundError:
-    # package is not installed
-    pass
-
-
-__all__ = [
-    "additional_session_information_callback",
-    "additional_test_information_callback",
-    "additional_information_callback",
-    "get_session_uid",
-    "get_test_uid",
-]
+"""pytest-fluent-logging."""
+import sys
+
+if sys.version_info >= (3, 8):
+    from importlib.metadata import PackageNotFoundError, version
+else:
+    from importlib_metadata import PackageNotFoundError  # type: ignore
+    from importlib_metadata import version  # type: ignore
+
+__version__ = "unknown"
+try:
+    __version__ = version(__name__)
+except PackageNotFoundError:
+    # package is not installed
+    pass
+
+
+from .additional_information import (
+    additional_session_information_callback,
+    additional_test_information_callback,
+)
+from .plugin import get_session_uid, get_test_uid
+
+__all__ = [
+    "additional_session_information_callback",
+    "additional_test_information_callback",
+    "get_session_uid",
+    "get_test_uid",
+]
```

### Comparing `pytest-fluent-0.0.0/src/pytest_fluent/test_report.py` & `pytest-fluent-0.1.0/src/pytest_fluent/test_report.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,134 +1,135 @@
-"""Extract result information."""
-# The MIT License (MIT)
-
-# Copyright (c) 2019 Israel Fruchter
-
-# Permission is hereby granted, free of charge, to any person obtaining a copy
-# of this software and associated documentation files (the "Software"), to deal
-# in the Software without restriction, including without limitation the rights
-# to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
-# copies of the Software, and to permit persons to whom the Software is
-# furnished to do so, subject to the following conditions:
-
-# The above copyright notice and this permission notice shall be included in
-# all copies or substantial portions of the Software.
-
-# THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
-# IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
-# FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
-# AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
-# LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
-# OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN
-# THE SOFTWARE.
-#
-# Adopted from https://github.com/fruch/pytest-elk-reporter
-
-import typing
-
-import pytest
-import six
-
-
-class LogReport(object):
-    def __init__(self, config):
-        self.config = config
-        super(LogReport, self).__init__()
-
-    def __call__(self, report: pytest.TestReport):
-        """Prepare result report for broadcasting."""
-        # pylint: disable=too-many-branches
-        results: typing.Dict[typing.Any, typing.Any] = {}
-
-        worker_id = self.get_worker_id()
-        # wait until workers are senting back their results.
-        # See https://pytest-xdist.readthedocs.io/en/latest/how-it-works.html
-        if worker_id not in ["master", "default"]:
-            return results
-        data = None
-
-        if report.passed:
-            if report.when == "call":
-                data = self.create_report_with_verdict(
-                    report,
-                    lambda x: hasattr(x, "wasxfail"),
-                    "xpassed",
-                    "passed",
-                )
-        elif report.failed:
-            if report.when == "call":
-                verdict = "failed"
-                if hasattr(report, "longrepr"):
-                    import _pytest
-
-                    if isinstance(
-                        report.longrepr, _pytest._code.code.ExceptionChainRepr
-                    ):
-                        verdict = "error"
-                data = self.create_report(report, verdict)
-            elif report.when == "setup":
-                data = self.create_report(report, "error")
-        elif report.skipped:
-            data = self.create_report_with_verdict(
-                report, lambda x: hasattr(x, "wasxfail"), "xfailed", "skipped"
-            )
-
-        if data:
-            results.update(data)
-        return results
-
-    def create_report_with_verdict(
-        self,
-        report: pytest.TestReport,
-        predicate: typing.Callable,
-        if_val: str,
-        else_val: str,
-    ) -> dict:
-        if predicate(report):
-            return self.create_report(report, if_val)
-        else:
-            return self.create_report(report, else_val)
-
-    def create_report(
-        self,
-        item_report: pytest.TestReport,
-        verdict: str,
-    ):
-        """Create test report dataset."""
-        test_data = dict(
-            item_report.user_properties,
-            name=item_report.nodeid,
-            outcome=verdict,
-            duration=item_report.duration,
-            markers=item_report.keywords,
-        )
-        message = self.get_failure_messge(item_report)
-        if message:
-            test_data.update(failure_message=message)
-        return test_data
-
-    def get_worker_id(self):
-        """Extract the worker id"""
-        worker_id = "default"
-        if hasattr(self.config, "workerinput"):
-            worker_id = self.config.workerinput["workerid"]
-        if (
-            not hasattr(self.config, "workerinput")
-            and getattr(self.config.option, "dist", "no") != "no"
-        ):
-            worker_id = "master"
-        return worker_id
-
-    @staticmethod
-    def get_failure_messge(item_report):
-        """Extract error message."""
-        if item_report.passed:
-            return ""
-        if hasattr(item_report, "longreprtext"):
-            message = item_report.longreprtext
-        elif hasattr(item_report.longrepr, "reprcrash"):
-            message = item_report.longrepr.reprcrash.message
-        elif isinstance(item_report.longrepr, six.string_types):
-            message = item_report.longrepr
-        else:
-            message = str(item_report.longrepr)
-        return message
+"""Extract result information."""
+# The MIT License (MIT)
+
+# Copyright (c) 2019 Israel Fruchter
+
+# Permission is hereby granted, free of charge, to any person obtaining a copy
+# of this software and associated documentation files (the "Software"), to deal
+# in the Software without restriction, including without limitation the rights
+# to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
+# copies of the Software, and to permit persons to whom the Software is
+# furnished to do so, subject to the following conditions:
+
+# The above copyright notice and this permission notice shall be included in
+# all copies or substantial portions of the Software.
+
+# THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
+# IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
+# FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
+# AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
+# LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
+# OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN
+# THE SOFTWARE.
+#
+# Adopted from https://github.com/fruch/pytest-elk-reporter
+
+import typing
+
+import pytest
+import six
+
+
+class LogReport(object):
+    def __init__(self, config):
+        self.config = config
+        super(LogReport, self).__init__()
+
+    def __call__(self, report: pytest.TestReport):
+        """Prepare result report for broadcasting."""
+        # pylint: disable=too-many-branches
+        results: typing.Dict[typing.Any, typing.Any] = {}
+
+        worker_id = self.get_worker_id()
+        # wait until workers are senting back their results.
+        # See https://pytest-xdist.readthedocs.io/en/latest/how-it-works.html
+        if worker_id not in ["master", "default"]:
+            return results
+        data = None
+
+        if report.passed:
+            if report.when == "call":
+                data = self.create_report_with_verdict(
+                    report,
+                    lambda x: hasattr(x, "wasxfail"),
+                    "xpassed",
+                    "passed",
+                )
+        elif report.failed:
+            if report.when == "call":
+
+                verdict = "failed"
+                if hasattr(report, "longrepr"):
+                    import _pytest
+
+                    if isinstance(
+                        report.longrepr, _pytest._code.code.ExceptionChainRepr
+                    ):
+                        verdict = "error"
+                data = self.create_report(report, verdict)
+            elif report.when == "setup":
+                data = self.create_report(report, "error")
+        elif report.skipped:
+            data = self.create_report_with_verdict(
+                report, lambda x: hasattr(x, "wasxfail"), "xfailed", "skipped"
+            )
+
+        if data:
+            results.update(data)
+        return results
+
+    def create_report_with_verdict(
+        self,
+        report: pytest.TestReport,
+        predicate: typing.Callable,
+        if_val: str,
+        else_val: str,
+    ) -> dict:
+        if predicate(report):
+            return self.create_report(report, if_val)
+        else:
+            return self.create_report(report, else_val)
+
+    def create_report(
+        self,
+        item_report: pytest.TestReport,
+        verdict: str,
+    ):
+        """Create test report dataset."""
+        test_data = dict(
+            item_report.user_properties,
+            name=item_report.nodeid,
+            outcome=verdict,
+            duration=item_report.duration,
+            markers=item_report.keywords,
+        )
+        message = self.get_failure_messge(item_report)
+        if message:
+            test_data.update(failure_message=message)
+        return test_data
+
+    def get_worker_id(self):
+        """Extract the worker id"""
+        worker_id = "default"
+        if hasattr(self.config, "workerinput"):
+            worker_id = self.config.workerinput["workerid"]
+        if (
+            not hasattr(self.config, "workerinput")
+            and getattr(self.config.option, "dist", "no") != "no"
+        ):
+            worker_id = "master"
+        return worker_id
+
+    @staticmethod
+    def get_failure_messge(item_report):
+        """Extract error message."""
+        if item_report.passed:
+            return ""
+        if hasattr(item_report, "longreprtext"):
+            message = item_report.longreprtext
+        elif hasattr(item_report.longrepr, "reprcrash"):
+            message = item_report.longrepr.reprcrash.message
+        elif isinstance(item_report.longrepr, six.string_types):
+            message = item_report.longrepr
+        else:
+            message = str(item_report.longrepr)
+        return message
```

### Comparing `pytest-fluent-0.0.0/src/pytest_fluent.egg-info/SOURCES.txt` & `pytest-fluent-0.1.0/src/pytest_fluent.egg-info/SOURCES.txt`

 * *Files 17% similar despite different names*

```diff
@@ -1,18 +1,34 @@
+.gitignore
 LICENSE
 README.md
 pyproject.toml
+requirements-dev.txt
 setup.cfg
 setup.py
+tox.ini
+.github/workflow/python-publish.yml
+.github/workflow/tests.yml
+docs/api.md
+docs/changelog.md
+docs/conf.py
+docs/contributing.md
+docs/index.md
+docs/installation.md
+docs/usage.md
 src/pytest_fluent/__init__.py
 src/pytest_fluent/additional_information.py
-src/pytest_fluent/content_patcher.py
-src/pytest_fluent/event.py
 src/pytest_fluent/plugin.py
-src/pytest_fluent/setting_file_loader_action.py
 src/pytest_fluent/test_report.py
 src/pytest_fluent.egg-info/PKG-INFO
 src/pytest_fluent.egg-info/SOURCES.txt
 src/pytest_fluent.egg-info/dependency_links.txt
 src/pytest_fluent.egg-info/entry_points.txt
 src/pytest_fluent.egg-info/requires.txt
-src/pytest_fluent.egg-info/top_level.txt
+src/pytest_fluent.egg-info/top_level.txt
+tests/__init__.py
+tests/conftest.py
+tests/test_additional_information.py
+tests/test_addoptions.py
+tests/test_fixtures.py
+tests/test_reporting.py
+tests/utility.py
```

