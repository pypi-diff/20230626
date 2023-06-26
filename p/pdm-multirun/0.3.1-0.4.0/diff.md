# Comparing `tmp/pdm_multirun-0.3.1.tar.gz` & `tmp/pdm_multirun-0.4.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pdm_multirun-0.3.1.tar", last modified: Tue Jun 13 13:14:06 2023, max compression
+gzip compressed data, was "pdm_multirun-0.4.0.tar", last modified: Mon Jun 26 12:47:07 2023, max compression
```

## Comparing `pdm_multirun-0.3.1.tar` & `pdm_multirun-0.4.0.tar`

### file list

```diff
@@ -1,10 +1,10 @@
--rw-r--r--   0        0        0      754 2023-06-08 13:02:32.508182 pdm_multirun-0.3.1/LICENSE
--rw-r--r--   0        0        0     2353 2023-06-08 13:02:35.261493 pdm_multirun-0.3.1/README.md
--rw-r--r--   0        0        0     2595 2023-06-13 13:14:06.400693 pdm_multirun-0.3.1/pyproject.toml
--rw-r--r--   0        0        0      150 2023-06-08 13:02:32.381516 pdm_multirun-0.3.1/src/pdm_multirun/__init__.py
--rw-r--r--   0        0        0     3240 2023-06-13 10:35:41.322821 pdm_multirun-0.3.1/src/pdm_multirun/plugin.py
--rw-r--r--   0        0        0        0 2023-06-08 13:02:32.378183 pdm_multirun-0.3.1/src/pdm_multirun/py.typed
--rw-r--r--   0        0        0      165 2023-06-08 13:02:32.371516 pdm_multirun-0.3.1/tests/__init__.py
--rw-r--r--   0        0        0       47 2023-06-08 13:02:32.368183 pdm_multirun-0.3.1/tests/conftest.py
--rw-r--r--   0        0        0      155 2023-06-08 13:53:36.229321 pdm_multirun-0.3.1/tests/test_plugin.py
--rw-r--r--   0        0        0     3784 1970-01-01 00:00:00.000000 pdm_multirun-0.3.1/PKG-INFO
+-rw-r--r--   0        0        0      754 2023-06-26 12:37:27.982105 pdm_multirun-0.4.0/LICENSE
+-rw-r--r--   0        0        0     3217 2023-06-26 12:39:57.149892 pdm_multirun-0.4.0/README.md
+-rw-r--r--   0        0        0     2550 2023-06-26 12:47:07.037097 pdm_multirun-0.4.0/pyproject.toml
+-rw-r--r--   0        0        0      150 2023-06-26 12:37:27.875440 pdm_multirun-0.4.0/src/pdm_multirun/__init__.py
+-rw-r--r--   0        0        0     3531 2023-06-26 12:17:30.368118 pdm_multirun-0.4.0/src/pdm_multirun/plugin.py
+-rw-r--r--   0        0        0        0 2023-06-26 12:37:27.875440 pdm_multirun-0.4.0/src/pdm_multirun/py.typed
+-rw-r--r--   0        0        0      165 2023-06-26 12:37:27.868774 pdm_multirun-0.4.0/tests/__init__.py
+-rw-r--r--   0        0        0       47 2023-06-26 12:37:27.868774 pdm_multirun-0.4.0/tests/conftest.py
+-rw-r--r--   0        0        0      155 2023-06-08 13:53:36.229321 pdm_multirun-0.4.0/tests/test_plugin.py
+-rw-r--r--   0        0        0     4598 1970-01-01 00:00:00.000000 pdm_multirun-0.4.0/PKG-INFO
```

### Comparing `pdm_multirun-0.3.1/LICENSE` & `pdm_multirun-0.4.0/LICENSE`

 * *Files identical despite different names*

### Comparing `pdm_multirun-0.3.1/README.md` & `pdm_multirun-0.4.0/README.md`

 * *Files 23% similar despite different names*

```diff
@@ -19,14 +19,28 @@
 
 With [PDM](https://github.com/pdm-project/pdm):
 
 ```bash
 pdm self add pdm-multirun
 ```
 
+As a local-only plugin:
+
+```toml
+# pyproject.toml
+[tool.pdm]
+plugins = [
+    "pdm-multirun",
+]
+```
+
+```bash
+pdm install --plugins
+```
+
 ## Usage
 
 This plugin adds a `multirun` command to PDM.
 The command accepts the same parameters as the `run` command,
 with an additional `-i`, `--interpreters`, `--versions` parameter
 that allows to specify the interpreters to use.
 
@@ -37,21 +51,38 @@
 To specify interpreters, pass a comma-separated string
 of Python versions:
 
 ```bash
 pdm multirun -i 3.10,3.11 pytest tests/
 ```
 
-By default, PDM Multirun reads Python versions from the
-`PDM_MULTIRUN_VERSIONS` environment variable.
-It is a string of `{major}.{minor}` versions,
+If you use virtual environments instead,
+pass their names to the `--interpreters` option
+and add the `-e`, `--venvs` flag:
+
+```bash
+pdm multirun -ei 3.10,3.11 pytest tests/
+```
+
+```bash
+pdm multirun -ei tests38,tests39 pytest tests/
+```
+
+By default, PDM Multirun reads Python versions (or venv names)
+from the `PDM_MULTIRUN_VERSIONS` environment variable.
+It is a string of `{major}.{minor}` versions (or venv names),
 separated by spaces, that can be found and called by PDM.
 
 ```bash
-export PDM_MULTIRUN_VERSIONS="3.7 3.8 3.9 3.10 3.11"
+export PDM_MULTIRUN_VERSIONS="3.8 3.9 3.10 3.11 3.12"
+pdm multirun pytest tests/
+```
+
+```bash
+export PDM_MULTIRUN_VERSIONS="tests38 tests39 tests310"
 pdm multirun pytest tests/
 ```
 
 PDM Multirun sets the `PDM_MULTIRUN=1` environment variable
 when running the specified command.
 You can use it to decide if you should, for example,
 print the current Python version in the output
@@ -67,10 +98,24 @@
     py = f"{sys.version_info[0]}.{sys.version_info[1]}"  # 3.8, 3.9, etc.
     ...  # use `py` string accordingly
 ```
 
 ---
 
 PDM Multirun successively runs the `pdm use` then `pdm run` internal actions.
-If the command fails on a Python version, PDM Multirun stops there.
-It any case, PDM Multirun will restore the Python version
-saved in `.pdm.toml` (through the `pdm use` command) before exiting.
+By default, if PDM cannot "use" an interpreter/venv, it continues with the next.
+
+```bash
+# will continue with 3.8 even if 3.7 is not available
+pdm multirun -i 3.7,3.8 pytest tests/
+```
+
+You can tell it to fail instead with the `-f`, `--fail-fast` flag:
+
+```bash
+# will stop at 3.7 if it's not available
+pdm multirun -fi 3.7,3.8 pytest tests/
+```
+
+If the command you run fails on a Python version, PDM Multirun stops there.
+In any case, PDM Multirun will restore the Python interpreter
+saved in `.pdm-python` (through the `pdm use` command) before exiting.
```

### Comparing `pdm_multirun-0.3.1/pyproject.toml` & `pdm_multirun-0.4.0/pyproject.toml`

 * *Files 5% similar despite different names*

```diff
@@ -7,37 +7,36 @@
 [project]
 name = "pdm-multirun"
 description = "A PDM plugin to run a command on multiple Python versions."
 authors = [
     { name = "Timothée Mazzucotelli", email = "pawamoy@pm.me" },
 ]
 readme = "README.md"
-requires-python = ">=3.7"
+requires-python = ">=3.8"
 keywords = []
 dynamic = []
 classifiers = [
     "Development Status :: 4 - Beta",
     "Intended Audience :: Developers",
     "Programming Language :: Python",
     "Programming Language :: Python :: 3",
     "Programming Language :: Python :: 3 :: Only",
-    "Programming Language :: Python :: 3.7",
     "Programming Language :: Python :: 3.8",
     "Programming Language :: Python :: 3.9",
     "Programming Language :: Python :: 3.10",
     "Programming Language :: Python :: 3.11",
     "Topic :: Documentation",
     "Topic :: Software Development",
     "Topic :: Utilities",
     "Typing :: Typed",
 ]
 dependencies = [
     "pdm>=2",
 ]
-version = "0.3.1"
+version = "0.4.0"
 
 [project.license]
 text = "ISC"
 
 [project.urls]
 Homepage = "https://pawamoy.github.io/pdm-multirun"
 Documentation = "https://pawamoy.github.io/pdm-multirun"
```

### Comparing `pdm_multirun-0.3.1/src/pdm_multirun/plugin.py` & `pdm_multirun-0.4.0/src/pdm_multirun/plugin.py`

 * *Files 20% similar despite different names*

```diff
@@ -12,74 +12,83 @@
 from pdm.cli.hooks import HookManager
 
 if TYPE_CHECKING:
     import argparse
 
     from pdm.core import Core
 
-PYTHON_VERSIONS = os.getenv("PDM_MULTIRUN_VERSIONS", "").split()
-PYTHON_VERSIONS = PYTHON_VERSIONS or [f"python3.{minor}" for minor in range(7, 12)]
+PYTHON_VERSIONS = os.getenv("PDM_MULTIRUN_VERSIONS", "").split() or [f"3.{minor}" for minor in range(8, 13)]
 
 
-def _interpreters(versions: str) -> list[str]:
-    return [f"python{version.strip()}" for version in versions.split(",")]
+def _comma_separated_list(value: str) -> list[str]:
+    return value.split(",")
 
 
 class MultirunCommand(RunCommand):
     """Run a command under multiple Python versions."""
 
     def add_arguments(self, parser: argparse.ArgumentParser) -> None:  # noqa: D102
         super().add_arguments(parser)
         parser.add_argument(
             "-f",
             "--fail-fast",
-            help="Exit as soon as an interpreter cannot be found or used",
+            help="Exit as soon as an interpreter/venv cannot be found or used",
             action="store_true",
             default=False,
         )
         parser.add_argument(
             "-i",
             "--interpreters",
             "--versions",
-            help="Comma-separated list of Python versions to run the command with",
-            type=_interpreters,
+            "--names",
+            help="Comma-separated list of Python versions or virtual environment names to run the command with",
+            type=_comma_separated_list,
+        )
+        parser.add_argument(
+            "-e",
+            "--venvs",
+            action="store_true",
+            default=False,
+            help="Use virtual environments",
         )
 
     def handle(self, project: Project, options: argparse.Namespace) -> None:  # noqa: D102
         os.environ["PDM_MULTIRUN"] = "1"
         old_python = str(project.environment.interpreter.path)
         project.core.ui.echo(f"Current interpreter: {old_python}", verbosity=termui.Verbosity.DETAIL)
-        for python_version in options.interpreters or PYTHON_VERSIONS:
+        for selected in options.interpreters or PYTHON_VERSIONS:
+            use_kwargs = {"venv" if options.venvs else "python": selected}
             try:
-                self._use(project, options, python_version)
+                self._use(project, options, **use_kwargs)
             except Exception:  # noqa: BLE001
                 if options.fail_fast:
                     raise
-                project.core.ui.echo(f"Skipped interpreter: {python_version}", verbosity=termui.Verbosity.DETAIL)
+                project.core.ui.echo(f"Skipped interpreter/venv: {selected}", verbosity=termui.Verbosity.DETAIL)
                 continue
             try:
                 super().handle(project, options)
             except SystemExit as exit:
                 if exit.code:
                     self._use(project, options, old_python)
                     raise
         project.core.ui.echo(f"Restoring interpreter: {old_python}", verbosity=termui.Verbosity.DETAIL)
         self._use(project, options, old_python)
         os.environ.pop("PDM_MULTIRUN", None)
 
-    def _use(self, project: Project, options: argparse.Namespace, python: str) -> None:
+    def _use(self, project: Project, options: argparse.Namespace, python: str = "", venv: str | None = None) -> None:
         old_echo = project.core.ui.echo
         if not options.verbose:
             project.core.ui.echo = lambda *args, **kwargs: None  # type: ignore[method-assign]
         # unset cached environment
         project.environment = None  # type: ignore[assignment]
         try:
             UseCommand().do_use(
                 project,
                 python=python,
+                venv=venv,
                 first=True,
                 ignore_remembered=False,
                 hooks=HookManager(project, skip=options.skip),
             )
         finally:
             project.core.ui.echo = old_echo  # type: ignore[method-assign]
```

### Comparing `pdm_multirun-0.3.1/PKG-INFO` & `pdm_multirun-0.4.0/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,19 +1,18 @@
 Metadata-Version: 2.1
 Name: pdm-multirun
-Version: 0.3.1
+Version: 0.4.0
 Summary: A PDM plugin to run a command on multiple Python versions.
 Author-Email: Timothée Mazzucotelli <pawamoy@pm.me>
 License: ISC
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3 :: Only
-Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Topic :: Documentation
 Classifier: Topic :: Software Development
 Classifier: Topic :: Utilities
@@ -22,15 +21,15 @@
 Project-URL: Documentation, https://pawamoy.github.io/pdm-multirun
 Project-URL: Changelog, https://pawamoy.github.io/pdm-multirun/changelog
 Project-URL: Repository, https://github.com/pawamoy/pdm-multirun
 Project-URL: Issues, https://github.com/pawamoy/pdm-multirun/issues
 Project-URL: Discussions, https://github.com/pawamoy/pdm-multirun/discussions
 Project-URL: Gitter, https://gitter.im/pdm-multirun/community
 Project-URL: Funding, https://github.com/sponsors/pawamoy
-Requires-Python: >=3.7
+Requires-Python: >=3.8
 Requires-Dist: pdm>=2
 Description-Content-Type: text/markdown
 
 # PDM Multirun
 
 [![ci](https://github.com/pawamoy/pdm-multirun/workflows/ci/badge.svg)](https://github.com/pawamoy/pdm-multirun/actions?query=workflow%3Aci)
 [![documentation](https://img.shields.io/badge/docs-mkdocs%20material-blue.svg?style=flat)](https://pawamoy.github.io/pdm-multirun/)
@@ -51,14 +50,28 @@
 
 With [PDM](https://github.com/pdm-project/pdm):
 
 ```bash
 pdm self add pdm-multirun
 ```
 
+As a local-only plugin:
+
+```toml
+# pyproject.toml
+[tool.pdm]
+plugins = [
+    "pdm-multirun",
+]
+```
+
+```bash
+pdm install --plugins
+```
+
 ## Usage
 
 This plugin adds a `multirun` command to PDM.
 The command accepts the same parameters as the `run` command,
 with an additional `-i`, `--interpreters`, `--versions` parameter
 that allows to specify the interpreters to use.
 
@@ -69,21 +82,38 @@
 To specify interpreters, pass a comma-separated string
 of Python versions:
 
 ```bash
 pdm multirun -i 3.10,3.11 pytest tests/
 ```
 
-By default, PDM Multirun reads Python versions from the
-`PDM_MULTIRUN_VERSIONS` environment variable.
-It is a string of `{major}.{minor}` versions,
+If you use virtual environments instead,
+pass their names to the `--interpreters` option
+and add the `-e`, `--venvs` flag:
+
+```bash
+pdm multirun -ei 3.10,3.11 pytest tests/
+```
+
+```bash
+pdm multirun -ei tests38,tests39 pytest tests/
+```
+
+By default, PDM Multirun reads Python versions (or venv names)
+from the `PDM_MULTIRUN_VERSIONS` environment variable.
+It is a string of `{major}.{minor}` versions (or venv names),
 separated by spaces, that can be found and called by PDM.
 
 ```bash
-export PDM_MULTIRUN_VERSIONS="3.7 3.8 3.9 3.10 3.11"
+export PDM_MULTIRUN_VERSIONS="3.8 3.9 3.10 3.11 3.12"
+pdm multirun pytest tests/
+```
+
+```bash
+export PDM_MULTIRUN_VERSIONS="tests38 tests39 tests310"
 pdm multirun pytest tests/
 ```
 
 PDM Multirun sets the `PDM_MULTIRUN=1` environment variable
 when running the specified command.
 You can use it to decide if you should, for example,
 print the current Python version in the output
@@ -99,10 +129,24 @@
     py = f"{sys.version_info[0]}.{sys.version_info[1]}"  # 3.8, 3.9, etc.
     ...  # use `py` string accordingly
 ```
 
 ---
 
 PDM Multirun successively runs the `pdm use` then `pdm run` internal actions.
-If the command fails on a Python version, PDM Multirun stops there.
-It any case, PDM Multirun will restore the Python version
-saved in `.pdm.toml` (through the `pdm use` command) before exiting.
+By default, if PDM cannot "use" an interpreter/venv, it continues with the next.
+
+```bash
+# will continue with 3.8 even if 3.7 is not available
+pdm multirun -i 3.7,3.8 pytest tests/
+```
+
+You can tell it to fail instead with the `-f`, `--fail-fast` flag:
+
+```bash
+# will stop at 3.7 if it's not available
+pdm multirun -fi 3.7,3.8 pytest tests/
+```
+
+If the command you run fails on a Python version, PDM Multirun stops there.
+In any case, PDM Multirun will restore the Python interpreter
+saved in `.pdm-python` (through the `pdm use` command) before exiting.
```

