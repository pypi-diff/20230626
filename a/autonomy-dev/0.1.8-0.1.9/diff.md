# Comparing `tmp/autonomy_dev-0.1.8.tar.gz` & `tmp/autonomy_dev-0.1.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "autonomy_dev-0.1.8.tar", max compression
+gzip compressed data, was "autonomy_dev-0.1.9.tar", max compression
```

## Comparing `autonomy_dev-0.1.8.tar` & `autonomy_dev-0.1.9.tar`

### file list

```diff
@@ -1,21 +1,26 @@
--rw-r--r--   0        0        0      578 2023-06-25 14:08:44.021352 autonomy_dev-0.1.8/LICENSE
--rw-r--r--   0        0        0      368 2023-06-25 14:08:44.021352 autonomy_dev-0.1.8/README.md
--rw-r--r--   0        0        0        0 2023-06-25 14:08:44.021352 autonomy_dev-0.1.8/auto_dev/__init__.py
--rw-r--r--   0        0        0     2454 2023-06-25 14:08:44.021352 autonomy_dev-0.1.8/auto_dev/base.py
--rw-r--r--   0        0        0      242 2023-06-25 14:08:44.021352 autonomy_dev-0.1.8/auto_dev/cli.py
--rw-r--r--   0        0        0     2758 2023-06-25 14:08:44.021352 autonomy_dev-0.1.8/auto_dev/cli_executor.py
--rw-r--r--   0        0        0     4303 2023-06-25 14:08:44.021352 autonomy_dev-0.1.8/auto_dev/commands/augment.py
--rw-r--r--   0        0        0     1890 2023-06-25 14:08:44.021352 autonomy_dev-0.1.8/auto_dev/commands/fmt.py
--rw-r--r--   0        0        0     1984 2023-06-25 14:08:44.021352 autonomy_dev-0.1.8/auto_dev/commands/lint.py
--rw-r--r--   0        0        0     1457 2023-06-25 14:08:44.021352 autonomy_dev-0.1.8/auto_dev/commands/test.py
--rw-r--r--   0        0        0      369 2023-06-25 14:08:44.021352 autonomy_dev-0.1.8/auto_dev/constants.py
--rw-r--r--   0        0        0      173 2023-06-25 14:08:44.021352 autonomy_dev-0.1.8/auto_dev/data/mermaid.py
--rw-r--r--   0        0        0      642 2023-06-25 14:08:44.021352 autonomy_dev-0.1.8/auto_dev/data/pylama.ini
--rw-r--r--   0        0        0     2027 2023-06-25 14:08:44.021352 autonomy_dev-0.1.8/auto_dev/fmt.py
--rw-r--r--   0        0        0      464 2023-06-25 14:08:44.021352 autonomy_dev-0.1.8/auto_dev/lint.py
--rw-r--r--   0        0        0      438 2023-06-25 14:08:44.021352 autonomy_dev-0.1.8/auto_dev/test.py
--rw-r--r--   0        0        0     1585 2023-06-25 14:08:44.021352 autonomy_dev-0.1.8/auto_dev/utils.py
--rw-r--r--   0        0        0     2510 2023-06-25 14:08:44.025352 autonomy_dev-0.1.8/pyproject.toml
--rw-r--r--   0        0        0     1634 2023-06-25 14:08:44.025352 autonomy_dev-0.1.8/tests/test_augmenter.py
--rw-r--r--   0        0        0     1484 2023-06-25 14:08:44.025352 autonomy_dev-0.1.8/tests/test_cli.py
--rw-r--r--   0        0        0     2501 1970-01-01 00:00:00.000000 autonomy_dev-0.1.8/PKG-INFO
+-rw-r--r--   0        0        0      578 2023-06-26 02:33:37.494932 autonomy_dev-0.1.9/LICENSE
+-rw-r--r--   0        0        0      368 2023-06-26 02:33:37.494932 autonomy_dev-0.1.9/README.md
+-rw-r--r--   0        0        0        0 2023-06-26 02:33:37.494932 autonomy_dev-0.1.9/auto_dev/__init__.py
+-rw-r--r--   0        0        0     2569 2023-06-26 02:33:37.494932 autonomy_dev-0.1.9/auto_dev/base.py
+-rw-r--r--   0        0        0      242 2023-06-26 02:33:37.494932 autonomy_dev-0.1.9/auto_dev/cli.py
+-rw-r--r--   0        0        0     2758 2023-06-26 02:33:37.494932 autonomy_dev-0.1.9/auto_dev/cli_executor.py
+-rw-r--r--   0        0        0     3318 2023-06-26 02:33:37.494932 autonomy_dev-0.1.9/auto_dev/commands/augment.py
+-rw-r--r--   0        0        0     1890 2023-06-26 02:33:37.494932 autonomy_dev-0.1.9/auto_dev/commands/fmt.py
+-rw-r--r--   0        0        0     2151 2023-06-26 02:33:37.494932 autonomy_dev-0.1.9/auto_dev/commands/lint.py
+-rw-r--r--   0        0        0     5195 2023-06-26 02:33:37.494932 autonomy_dev-0.1.9/auto_dev/commands/repo.py
+-rw-r--r--   0        0        0    10945 2023-06-26 02:33:37.494932 autonomy_dev-0.1.9/auto_dev/commands/scaffold.py
+-rw-r--r--   0        0        0     1450 2023-06-26 02:33:37.494932 autonomy_dev-0.1.9/auto_dev/commands/test.py
+-rw-r--r--   0        0        0      515 2023-06-26 02:33:37.494932 autonomy_dev-0.1.9/auto_dev/constants.py
+-rw-r--r--   0        0        0      173 2023-06-26 02:33:37.494932 autonomy_dev-0.1.9/auto_dev/data/mermaid.py
+-rw-r--r--   0        0        0      642 2023-06-26 02:33:37.494932 autonomy_dev-0.1.9/auto_dev/data/pylama.ini
+-rw-r--r--   0        0        0      532 2023-06-26 02:33:37.494932 autonomy_dev-0.1.9/auto_dev/data/repo/templates/python/readme.py
+-rw-r--r--   0        0        0     2027 2023-06-26 02:33:37.494932 autonomy_dev-0.1.9/auto_dev/fmt.py
+-rw-r--r--   0        0        0      464 2023-06-26 02:33:37.494932 autonomy_dev-0.1.9/auto_dev/lint.py
+-rw-r--r--   0        0        0      438 2023-06-26 02:33:37.494932 autonomy_dev-0.1.9/auto_dev/test.py
+-rw-r--r--   0        0        0     1585 2023-06-26 02:33:37.494932 autonomy_dev-0.1.9/auto_dev/utils.py
+-rw-r--r--   0        0        0     2595 2023-06-26 02:33:37.498932 autonomy_dev-0.1.9/pyproject.toml
+-rw-r--r--   0        0        0      455 2023-06-26 02:33:37.498932 autonomy_dev-0.1.9/tests/conftest.py
+-rw-r--r--   0        0        0     1634 2023-06-26 02:33:37.498932 autonomy_dev-0.1.9/tests/test_augmenter.py
+-rw-r--r--   0        0        0     1108 2023-06-26 02:33:37.498932 autonomy_dev-0.1.9/tests/test_cli.py
+-rw-r--r--   0        0        0     2488 2023-06-26 02:33:37.498932 autonomy_dev-0.1.9/tests/test_contracts.py
+-rw-r--r--   0        0        0     2619 1970-01-01 00:00:00.000000 autonomy_dev-0.1.9/PKG-INFO
```

### Comparing `autonomy_dev-0.1.8/LICENSE` & `autonomy_dev-0.1.9/LICENSE`

 * *Files identical despite different names*

### Comparing `autonomy_dev-0.1.8/auto_dev/base.py` & `autonomy_dev-0.1.9/auto_dev/base.py`

 * *Files 4% similar despite different names*

```diff
@@ -59,14 +59,17 @@
     @click.option("-n", "--num-processes", default=1, help="Number of processes to use for linting", type=int)
     @click.pass_context
     def cli(ctx, log_level=False, verbose=False, num_processes=1):
         """Cli development tooling."""
         ctx.obj = {}
         ctx.obj["VERBOSE"] = verbose
         ctx.obj["LOGGER"] = get_logger(log_level=log_level)
+        if num_processes == 0:
+            # we use all available cores
+            num_processes = os.cpu_count()
         ctx.obj["NUM_PROCESSES"] = num_processes
         ctx.obj["LOGGER"].info("Starting Auto Dev...")
         if verbose:
             ctx.obj["LOGGER"].info("Verbose mode enabled")
         if num_processes > 1:
             ctx.obj["LOGGER"].info(f"Using {num_processes} processes for processing")
         if log_level:
```

### Comparing `autonomy_dev-0.1.8/auto_dev/cli_executor.py` & `autonomy_dev-0.1.9/auto_dev/cli_executor.py`

 * *Files identical despite different names*

### Comparing `autonomy_dev-0.1.8/auto_dev/commands/fmt.py` & `autonomy_dev-0.1.9/auto_dev/commands/fmt.py`

 * *Files identical despite different names*

### Comparing `autonomy_dev-0.1.8/auto_dev/commands/lint.py` & `autonomy_dev-0.1.9/auto_dev/commands/lint.py`

 * *Files 4% similar despite different names*

```diff
@@ -41,14 +41,18 @@
         results = multi_thread_lint(paths, verbose, num_processes)
     else:
         results = single_thread_lint(paths, verbose, logger)
     passed = sum(results.values())
     failed = len(results) - passed
     logger.info(f"Linting completed with {passed} passed and {failed} failed")
     if failed > 0:
+        for file_path, result in results.items():
+            if not result:
+                logger.error(f"Linting failed for {paths[file_path]}")
+    if failed > 0:
         raise click.ClickException("Linting failed!")
 
 
 def single_thread_lint(paths, verbose, logger):
     """Run the linting in a single thread."""
     results = {}
     for package in track(range(len(paths)), description="Linting..."):
```

### Comparing `autonomy_dev-0.1.8/auto_dev/commands/test.py` & `autonomy_dev-0.1.9/auto_dev/commands/test.py`

 * *Files 8% similar despite different names*

```diff
@@ -22,15 +22,15 @@
 @click.pass_context
 def test(ctx, path):
     """
     Runs the test tooling
     """
     verbose = ctx.obj["VERBOSE"]
     logger = ctx.obj["LOGGER"]
-    logger.info("Testing Open Autonomy Packages")
+    logger.info(f"Testing path: `{path}`")
     try:
         packages = get_packages() if not path else [path]
     except Exception as error:
         raise click.ClickException(f"Unable to get packages are you in the right directory? {error}")
     results = {}
     for package in track(range(len(packages)), description="Testing..."):
         result = test_path(str(packages[package]), verbose=verbose)
```

### Comparing `autonomy_dev-0.1.8/auto_dev/data/pylama.ini` & `autonomy_dev-0.1.9/auto_dev/data/pylama.ini`

 * *Files identical despite different names*

### Comparing `autonomy_dev-0.1.8/auto_dev/fmt.py` & `autonomy_dev-0.1.9/auto_dev/fmt.py`

 * *Files identical despite different names*

### Comparing `autonomy_dev-0.1.8/auto_dev/utils.py` & `autonomy_dev-0.1.9/auto_dev/utils.py`

 * *Files identical despite different names*

### Comparing `autonomy_dev-0.1.8/pyproject.toml` & `autonomy_dev-0.1.9/pyproject.toml`

 * *Files 8% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 [tool]
 [tool.poetry]
 name = "autonomy_dev"
-version = "0.1.8"
+version = "0.1.9"
 homepage = "https://github.com/8ball030/auto_dev"
 description = "A collection of tooling to enable open source development of autonomy tools"
 authors = ["8Baller <8ball030@gmail.com>"]
 readme = "README.md"
 license =  "Apache-2.0"
 classifiers=[
     'Development Status :: 2 - Pre-Alpha',
@@ -21,16 +21,16 @@
 packages = [
     { include = "auto_dev" },
     { include = "tests", format = "sdist" },
 ]
 
 
 [tool.poetry.dependencies]
-python = ">=3.7,<=3.11"
-click = ">=8.0.2"
+python = ">=3.7.2,<=3.11"
+click = "8.0.2"
 black = "^22.6.0"
 mypy = "^0.971"
 pytest-cov = "^3.0.0"
 tox = "^3.25.1"
 pip = "^22.2.2"
 mkdocs = "^1.3.1"
 mkdocs-include-markdown-plugin = "^3.6.1"
@@ -45,14 +45,18 @@
 GitPython = "^3.1.27"
 pylama = {extras = ["all"], version = "^8.4.1"}
 rich-click = "^1.5.2"
 install = "^1.3.5"
 mkdocstrings-python = "^0.10.0"
 isort = "~5"
 pylint = "~2"
+open-aea = "^1.35.0"
+open-aea-cli-ipfs = "^1.35.0"
+web3 = "~5"
+responses = "^0.23.1"
 
 [tool.poetry.dev-dependencies]
 
 
 [tool.poetry.extras]
 all = [
     "pytest",
```

### Comparing `autonomy_dev-0.1.8/tests/test_augmenter.py` & `autonomy_dev-0.1.9/tests/test_augmenter.py`

 * *Files identical despite different names*

### Comparing `autonomy_dev-0.1.8/PKG-INFO` & `autonomy_dev-0.1.9/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,51 +1,54 @@
 Metadata-Version: 2.1
 Name: autonomy-dev
-Version: 0.1.8
+Version: 0.1.9
 Summary: A collection of tooling to enable open source development of autonomy tools
 Home-page: https://github.com/8ball030/auto_dev
 License: Apache-2.0
 Author: 8Baller
 Author-email: 8ball030@gmail.com
-Requires-Python: >=3.7,<=3.11
+Requires-Python: >=3.7.2,<=3.11
 Classifier: Development Status :: 2 - Pre-Alpha
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Natural Language :: English
 Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Provides-Extra: all
 Provides-Extra: dev
 Provides-Extra: doc
 Requires-Dist: GitPython (>=3.1.27,<4.0.0)
 Requires-Dist: black (>=22.6.0,<23.0.0) ; extra == "all"
 Requires-Dist: bump2version (>=1.0.1,<2.0.0) ; extra == "dev"
-Requires-Dist: click (>=8.0.2)
+Requires-Dist: click (==8.0.2)
 Requires-Dist: install (>=1.3.5,<2.0.0)
 Requires-Dist: isort (>=5,<6) ; extra == "all"
 Requires-Dist: mkdocs (>=1.3.1,<2.0.0) ; extra == "doc"
 Requires-Dist: mkdocs-autorefs (>=0.4.1,<0.5.0) ; extra == "doc"
 Requires-Dist: mkdocs-include-markdown-plugin (>=3.6.1,<4.0.0) ; extra == "doc"
 Requires-Dist: mkdocs-material (>=8.4.0,<9.0.0) ; extra == "doc"
 Requires-Dist: mkdocs-material-extensions (>=1.0.3,<2.0.0)
 Requires-Dist: mkdocstrings-python (>=0.10.0,<0.11.0)
 Requires-Dist: mypy (>=0.971,<0.972) ; extra == "all"
+Requires-Dist: open-aea (>=1.35.0,<2.0.0)
+Requires-Dist: open-aea-cli-ipfs (>=1.35.0,<2.0.0)
 Requires-Dist: pip (>=22.2.2,<23.0.0) ; extra == "dev"
 Requires-Dist: pre-commit (>=2.20.0,<3.0.0) ; extra == "dev"
 Requires-Dist: pylama[all] (>=8.4.1,<9.0.0) ; extra == "all"
 Requires-Dist: pylint (>=2,<3) ; extra == "all"
 Requires-Dist: pytest-cov (>=3.0.0,<4.0.0) ; extra == "all"
+Requires-Dist: responses (>=0.23.1,<0.24.0)
 Requires-Dist: rich-click (>=1.5.2,<2.0.0)
 Requires-Dist: toml (>=0.10.2,<0.11.0) ; extra == "dev"
 Requires-Dist: tox (>=3.25.1,<4.0.0) ; extra == "dev"
 Requires-Dist: twine (>=4.0.1,<5.0.0) ; extra == "dev"
+Requires-Dist: web3 (>=5,<6)
 Requires-Dist: yamllint (>=1.27.1,<2.0.0)
 Description-Content-Type: text/markdown
 
 # Autonomy Dev
 
 Tooling to speed up autonomy development.
```

