# Comparing `tmp/uedition-0.3.1.tar.gz` & `tmp/uedition-0.4.0.tar.gz`

## Comparing `uedition-0.3.1.tar` & `uedition-0.4.0.tar`

### file list

```diff
@@ -1,64 +1,67 @@
--rw-r--r--   0        0        0      299 2020-02-02 00:00:00.000000 uedition-0.3.1/.pre-commit-config.yaml
--rw-r--r--   0        0        0       29 2020-02-02 00:00:00.000000 uedition-0.3.1/tox.ini
--rw-r--r--   0        0        0      295 2020-02-02 00:00:00.000000 uedition-0.3.1/.github/dependabot.yml
--rw-r--r--   0        0        0     1334 2020-02-02 00:00:00.000000 uedition-0.3.1/.github/workflows/coverage.yml
--rw-r--r--   0        0        0      758 2020-02-02 00:00:00.000000 uedition-0.3.1/.github/workflows/release.yml
--rw-r--r--   0        0        0      686 2020-02-02 00:00:00.000000 uedition-0.3.1/.github/workflows/tests.yml
--rw-r--r--   0        0        0      127 2020-02-02 00:00:00.000000 uedition-0.3.1/tests/__init__.py
--rw-r--r--   0        0        0     3414 2020-02-02 00:00:00.000000 uedition-0.3.1/tests/conftest.py
--rw-r--r--   0        0        0      459 2020-02-02 00:00:00.000000 uedition-0.3.1/tests/test_about.py
--rw-r--r--   0        0        0      596 2020-02-02 00:00:00.000000 uedition-0.3.1/tests/test_build.py
--rw-r--r--   0        0        0     2476 2020-02-02 00:00:00.000000 uedition-0.3.1/tests/test_check.py
--rw-r--r--   0        0        0      547 2020-02-02 00:00:00.000000 uedition-0.3.1/tests/test_settings.py
--rw-r--r--   0        0        0       11 2020-02-02 00:00:00.000000 uedition-0.3.1/tests/fixtures/basic/uEdition.yml
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 uedition-0.3.1/tests/fixtures/empty/.gitkeep
--rw-r--r--   0        0        0       67 2020-02-02 00:00:00.000000 uedition-0.3.1/tests/fixtures/invalid_core_files/uEdition.yaml
--rw-r--r--   0        0        0       34 2020-02-02 00:00:00.000000 uedition-0.3.1/tests/fixtures/invalid_core_files/en/_config.yml
--rw-r--r--   0        0        0       34 2020-02-02 00:00:00.000000 uedition-0.3.1/tests/fixtures/invalid_core_files/en/_toc.yml
--rw-r--r--   0        0        0       67 2020-02-02 00:00:00.000000 uedition-0.3.1/tests/fixtures/missing_core_files/uEdition.yaml
--rw-r--r--   0        0        0       12 2020-02-02 00:00:00.000000 uedition-0.3.1/tests/fixtures/missing_files/.gitignore
--rw-r--r--   0        0        0     5524 2020-02-02 00:00:00.000000 uedition-0.3.1/tests/fixtures/missing_files/references.bib
--rw-r--r--   0        0        0       67 2020-02-02 00:00:00.000000 uedition-0.3.1/tests/fixtures/missing_files/uEdition.yaml
--rw-r--r--   0        0        0      987 2020-02-02 00:00:00.000000 uedition-0.3.1/tests/fixtures/missing_files/en/_config.yml
--rw-r--r--   0        0        0      154 2020-02-02 00:00:00.000000 uedition-0.3.1/tests/fixtures/missing_files/en/_toc.yml
--rw-r--r--   0        0        0       96 2020-02-02 00:00:00.000000 uedition-0.3.1/tests/fixtures/missing_files/en/intro.md
--rw-r--r--   0        0        0       67 2020-02-02 00:00:00.000000 uedition-0.3.1/tests/fixtures/missing_toc_root/uEdition.yaml
--rw-r--r--   0        0        0       34 2020-02-02 00:00:00.000000 uedition-0.3.1/tests/fixtures/missing_toc_root/en/_config.yml
--rw-r--r--   0        0        0       96 2020-02-02 00:00:00.000000 uedition-0.3.1/tests/fixtures/missing_toc_root/en/_toc.yml
--rw-r--r--   0        0        0       67 2020-02-02 00:00:00.000000 uedition-0.3.1/tests/fixtures/missing_toc_root_file/uEdition.yaml
--rw-r--r--   0        0        0       34 2020-02-02 00:00:00.000000 uedition-0.3.1/tests/fixtures/missing_toc_root_file/en/_config.yml
--rw-r--r--   0        0        0      110 2020-02-02 00:00:00.000000 uedition-0.3.1/tests/fixtures/missing_toc_root_file/en/_toc.yml
--rw-r--r--   0        0        0       12 2020-02-02 00:00:00.000000 uedition-0.3.1/tests/fixtures/multilang/.gitignore
--rw-r--r--   0        0        0     5524 2020-02-02 00:00:00.000000 uedition-0.3.1/tests/fixtures/multilang/references.bib
--rw-r--r--   0        0        0      112 2020-02-02 00:00:00.000000 uedition-0.3.1/tests/fixtures/multilang/uEdition.yaml
--rw-r--r--   0        0        0      987 2020-02-02 00:00:00.000000 uedition-0.3.1/tests/fixtures/multilang/de/_config.yml
--rw-r--r--   0        0        0      297 2020-02-02 00:00:00.000000 uedition-0.3.1/tests/fixtures/multilang/de/_toc.yml
--rw-r--r--   0        0        0       59 2020-02-02 00:00:00.000000 uedition-0.3.1/tests/fixtures/multilang/de/a-1-page.md
--rw-r--r--   0        0        0       59 2020-02-02 00:00:00.000000 uedition-0.3.1/tests/fixtures/multilang/de/a-2-page.md
--rw-r--r--   0        0        0       46 2020-02-02 00:00:00.000000 uedition-0.3.1/tests/fixtures/multilang/de/a-page.md
--rw-r--r--   0        0        0       46 2020-02-02 00:00:00.000000 uedition-0.3.1/tests/fixtures/multilang/de/b-page.md
--rw-r--r--   0        0        0       98 2020-02-02 00:00:00.000000 uedition-0.3.1/tests/fixtures/multilang/de/intro.md
--rw-r--r--   0        0        0      987 2020-02-02 00:00:00.000000 uedition-0.3.1/tests/fixtures/multilang/en/_config.yml
--rw-r--r--   0        0        0      297 2020-02-02 00:00:00.000000 uedition-0.3.1/tests/fixtures/multilang/en/_toc.yml
--rw-r--r--   0        0        0       54 2020-02-02 00:00:00.000000 uedition-0.3.1/tests/fixtures/multilang/en/a-1-page.md
--rw-r--r--   0        0        0       54 2020-02-02 00:00:00.000000 uedition-0.3.1/tests/fixtures/multilang/en/a-2-page.md
--rw-r--r--   0        0        0       41 2020-02-02 00:00:00.000000 uedition-0.3.1/tests/fixtures/multilang/en/a-page.md
--rw-r--r--   0        0        0       41 2020-02-02 00:00:00.000000 uedition-0.3.1/tests/fixtures/multilang/en/b-page.md
--rw-r--r--   0        0        0       96 2020-02-02 00:00:00.000000 uedition-0.3.1/tests/fixtures/multilang/en/intro.md
--rw-r--r--   0        0        0       11 2020-02-02 00:00:00.000000 uedition-0.3.1/tests/fixtures/yaml/uEdition.yaml
--rw-r--r--   0        0        0      157 2020-02-02 00:00:00.000000 uedition-0.3.1/uedition/__about__.py
--rw-r--r--   0        0        0      285 2020-02-02 00:00:00.000000 uedition-0.3.1/uedition/__init__.py
--rw-r--r--   0        0        0      182 2020-02-02 00:00:00.000000 uedition-0.3.1/uedition/__main__.py
--rw-r--r--   0        0        0     1945 2020-02-02 00:00:00.000000 uedition-0.3.1/uedition/settings.py
--rw-r--r--   0        0        0      864 2020-02-02 00:00:00.000000 uedition-0.3.1/uedition/cli/__init__.py
--rw-r--r--   0        0        0     2796 2020-02-02 00:00:00.000000 uedition-0.3.1/uedition/cli/build.py
--rw-r--r--   0        0        0     6970 2020-02-02 00:00:00.000000 uedition-0.3.1/uedition/cli/check.py
--rw-r--r--   0        0        0     1174 2020-02-02 00:00:00.000000 uedition-0.3.1/uedition/cli/serve.py
--rw-r--r--   0        0        0      206 2020-02-02 00:00:00.000000 uedition-0.3.1/uedition/ext/__init__.py
--rw-r--r--   0        0        0     5452 2020-02-02 00:00:00.000000 uedition-0.3.1/uedition/ext/config.py
--rw-r--r--   0        0        0    10625 2020-02-02 00:00:00.000000 uedition-0.3.1/uedition/ext/tei.py
--rw-r--r--   0        0        0       71 2020-02-02 00:00:00.000000 uedition-0.3.1/.gitignore
--rw-r--r--   0        0        0     1101 2020-02-02 00:00:00.000000 uedition-0.3.1/LICENSE.txt
--rw-r--r--   0        0        0      982 2020-02-02 00:00:00.000000 uedition-0.3.1/README.md
--rw-r--r--   0        0        0     1631 2020-02-02 00:00:00.000000 uedition-0.3.1/pyproject.toml
--rw-r--r--   0        0        0     1938 2020-02-02 00:00:00.000000 uedition-0.3.1/PKG-INFO
+-rw-r--r--   0        0        0      249 2020-02-02 00:00:00.000000 uedition-0.4.0/.pre-commit-config.yaml
+-rw-r--r--   0        0        0       29 2020-02-02 00:00:00.000000 uedition-0.4.0/tox.ini
+-rw-r--r--   0        0        0      295 2020-02-02 00:00:00.000000 uedition-0.4.0/.github/dependabot.yml
+-rw-r--r--   0        0        0      213 2020-02-02 00:00:00.000000 uedition-0.4.0/.github/workflows/codestyle.yml
+-rw-r--r--   0        0        0     1334 2020-02-02 00:00:00.000000 uedition-0.4.0/.github/workflows/coverage.yml
+-rw-r--r--   0        0        0      758 2020-02-02 00:00:00.000000 uedition-0.4.0/.github/workflows/release.yml
+-rw-r--r--   0        0        0      686 2020-02-02 00:00:00.000000 uedition-0.4.0/.github/workflows/tests.yml
+-rw-r--r--   0        0        0      127 2020-02-02 00:00:00.000000 uedition-0.4.0/tests/__init__.py
+-rw-r--r--   0        0        0     3423 2020-02-02 00:00:00.000000 uedition-0.4.0/tests/conftest.py
+-rw-r--r--   0        0        0      459 2020-02-02 00:00:00.000000 uedition-0.4.0/tests/test_about.py
+-rw-r--r--   0        0        0      596 2020-02-02 00:00:00.000000 uedition-0.4.0/tests/test_build.py
+-rw-r--r--   0        0        0     2494 2020-02-02 00:00:00.000000 uedition-0.4.0/tests/test_check.py
+-rw-r--r--   0        0        0      547 2020-02-02 00:00:00.000000 uedition-0.4.0/tests/test_settings.py
+-rw-r--r--   0        0        0       11 2020-02-02 00:00:00.000000 uedition-0.4.0/tests/fixtures/basic/uEdition.yml
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 uedition-0.4.0/tests/fixtures/empty/.gitkeep
+-rw-r--r--   0        0        0       67 2020-02-02 00:00:00.000000 uedition-0.4.0/tests/fixtures/invalid_core_files/uEdition.yaml
+-rw-r--r--   0        0        0       34 2020-02-02 00:00:00.000000 uedition-0.4.0/tests/fixtures/invalid_core_files/en/_config.yml
+-rw-r--r--   0        0        0       34 2020-02-02 00:00:00.000000 uedition-0.4.0/tests/fixtures/invalid_core_files/en/_toc.yml
+-rw-r--r--   0        0        0       67 2020-02-02 00:00:00.000000 uedition-0.4.0/tests/fixtures/missing_core_files/uEdition.yaml
+-rw-r--r--   0        0        0       12 2020-02-02 00:00:00.000000 uedition-0.4.0/tests/fixtures/missing_files/.gitignore
+-rw-r--r--   0        0        0     5524 2020-02-02 00:00:00.000000 uedition-0.4.0/tests/fixtures/missing_files/references.bib
+-rw-r--r--   0        0        0       67 2020-02-02 00:00:00.000000 uedition-0.4.0/tests/fixtures/missing_files/uEdition.yaml
+-rw-r--r--   0        0        0      987 2020-02-02 00:00:00.000000 uedition-0.4.0/tests/fixtures/missing_files/en/_config.yml
+-rw-r--r--   0        0        0      154 2020-02-02 00:00:00.000000 uedition-0.4.0/tests/fixtures/missing_files/en/_toc.yml
+-rw-r--r--   0        0        0       96 2020-02-02 00:00:00.000000 uedition-0.4.0/tests/fixtures/missing_files/en/intro.md
+-rw-r--r--   0        0        0       67 2020-02-02 00:00:00.000000 uedition-0.4.0/tests/fixtures/missing_toc_root/uEdition.yaml
+-rw-r--r--   0        0        0       34 2020-02-02 00:00:00.000000 uedition-0.4.0/tests/fixtures/missing_toc_root/en/_config.yml
+-rw-r--r--   0        0        0       96 2020-02-02 00:00:00.000000 uedition-0.4.0/tests/fixtures/missing_toc_root/en/_toc.yml
+-rw-r--r--   0        0        0       67 2020-02-02 00:00:00.000000 uedition-0.4.0/tests/fixtures/missing_toc_root_file/uEdition.yaml
+-rw-r--r--   0        0        0       34 2020-02-02 00:00:00.000000 uedition-0.4.0/tests/fixtures/missing_toc_root_file/en/_config.yml
+-rw-r--r--   0        0        0      110 2020-02-02 00:00:00.000000 uedition-0.4.0/tests/fixtures/missing_toc_root_file/en/_toc.yml
+-rw-r--r--   0        0        0       12 2020-02-02 00:00:00.000000 uedition-0.4.0/tests/fixtures/multilang/.gitignore
+-rw-r--r--   0        0        0     5524 2020-02-02 00:00:00.000000 uedition-0.4.0/tests/fixtures/multilang/references.bib
+-rw-r--r--   0        0        0      112 2020-02-02 00:00:00.000000 uedition-0.4.0/tests/fixtures/multilang/uEdition.yaml
+-rw-r--r--   0        0        0      987 2020-02-02 00:00:00.000000 uedition-0.4.0/tests/fixtures/multilang/de/_config.yml
+-rw-r--r--   0        0        0      297 2020-02-02 00:00:00.000000 uedition-0.4.0/tests/fixtures/multilang/de/_toc.yml
+-rw-r--r--   0        0        0       59 2020-02-02 00:00:00.000000 uedition-0.4.0/tests/fixtures/multilang/de/a-1-page.md
+-rw-r--r--   0        0        0       59 2020-02-02 00:00:00.000000 uedition-0.4.0/tests/fixtures/multilang/de/a-2-page.md
+-rw-r--r--   0        0        0       46 2020-02-02 00:00:00.000000 uedition-0.4.0/tests/fixtures/multilang/de/a-page.md
+-rw-r--r--   0        0        0       46 2020-02-02 00:00:00.000000 uedition-0.4.0/tests/fixtures/multilang/de/b-page.md
+-rw-r--r--   0        0        0       98 2020-02-02 00:00:00.000000 uedition-0.4.0/tests/fixtures/multilang/de/intro.md
+-rw-r--r--   0        0        0      987 2020-02-02 00:00:00.000000 uedition-0.4.0/tests/fixtures/multilang/en/_config.yml
+-rw-r--r--   0        0        0      297 2020-02-02 00:00:00.000000 uedition-0.4.0/tests/fixtures/multilang/en/_toc.yml
+-rw-r--r--   0        0        0       54 2020-02-02 00:00:00.000000 uedition-0.4.0/tests/fixtures/multilang/en/a-1-page.md
+-rw-r--r--   0        0        0       54 2020-02-02 00:00:00.000000 uedition-0.4.0/tests/fixtures/multilang/en/a-2-page.md
+-rw-r--r--   0        0        0       41 2020-02-02 00:00:00.000000 uedition-0.4.0/tests/fixtures/multilang/en/a-page.md
+-rw-r--r--   0        0        0       41 2020-02-02 00:00:00.000000 uedition-0.4.0/tests/fixtures/multilang/en/b-page.md
+-rw-r--r--   0        0        0       96 2020-02-02 00:00:00.000000 uedition-0.4.0/tests/fixtures/multilang/en/intro.md
+-rw-r--r--   0        0        0       11 2020-02-02 00:00:00.000000 uedition-0.4.0/tests/fixtures/yaml/uEdition.yaml
+-rw-r--r--   0        0        0      157 2020-02-02 00:00:00.000000 uedition-0.4.0/uedition/__about__.py
+-rw-r--r--   0        0        0      285 2020-02-02 00:00:00.000000 uedition-0.4.0/uedition/__init__.py
+-rw-r--r--   0        0        0      182 2020-02-02 00:00:00.000000 uedition-0.4.0/uedition/__main__.py
+-rw-r--r--   0        0        0     2070 2020-02-02 00:00:00.000000 uedition-0.4.0/uedition/settings.py
+-rw-r--r--   0        0        0      864 2020-02-02 00:00:00.000000 uedition-0.4.0/uedition/cli/__init__.py
+-rw-r--r--   0        0        0     3002 2020-02-02 00:00:00.000000 uedition-0.4.0/uedition/cli/build.py
+-rw-r--r--   0        0        0     7295 2020-02-02 00:00:00.000000 uedition-0.4.0/uedition/cli/check.py
+-rw-r--r--   0        0        0     1192 2020-02-02 00:00:00.000000 uedition-0.4.0/uedition/cli/serve.py
+-rw-r--r--   0        0        0      286 2020-02-02 00:00:00.000000 uedition-0.4.0/uedition/ext/__init__.py
+-rw-r--r--   0        0        0     6083 2020-02-02 00:00:00.000000 uedition-0.4.0/uedition/ext/config.py
+-rw-r--r--   0        0        0     2426 2020-02-02 00:00:00.000000 uedition-0.4.0/uedition/ext/language_switcher.js
+-rw-r--r--   0        0        0     1091 2020-02-02 00:00:00.000000 uedition-0.4.0/uedition/ext/language_switcher.py
+-rw-r--r--   0        0        0    11271 2020-02-02 00:00:00.000000 uedition-0.4.0/uedition/ext/tei.py
+-rw-r--r--   0        0        0       71 2020-02-02 00:00:00.000000 uedition-0.4.0/.gitignore
+-rw-r--r--   0        0        0     1101 2020-02-02 00:00:00.000000 uedition-0.4.0/LICENSE.txt
+-rw-r--r--   0        0        0      982 2020-02-02 00:00:00.000000 uedition-0.4.0/README.md
+-rw-r--r--   0        0        0     1741 2020-02-02 00:00:00.000000 uedition-0.4.0/pyproject.toml
+-rw-r--r--   0        0        0     1938 2020-02-02 00:00:00.000000 uedition-0.4.0/PKG-INFO
```

### Comparing `uedition-0.3.1/.github/workflows/coverage.yml` & `uedition-0.4.0/.github/workflows/coverage.yml`

 * *Files identical despite different names*

### Comparing `uedition-0.3.1/.github/workflows/release.yml` & `uedition-0.4.0/.github/workflows/release.yml`

 * *Files identical despite different names*

### Comparing `uedition-0.3.1/.github/workflows/tests.yml` & `uedition-0.4.0/.github/workflows/tests.yml`

 * *Files identical despite different names*

### Comparing `uedition-0.3.1/tests/conftest.py` & `uedition-0.4.0/tests/conftest.py`

 * *Files 8% similar despite different names*

```diff
@@ -13,115 +13,124 @@
     yield runner
 
 
 @fixture
 def empty_app() -> None:
     """Yield a uEdition application with no configuration set."""
     cwd = os.getcwd()
-    os.chdir('tests/fixtures/empty')
+    os.chdir("tests/fixtures/empty")
     from uedition.cli import app
     from uedition.settings import reload_settings
+
     reload_settings()
     yield app
     os.chdir(cwd)
 
 
 @fixture
 def basic_app() -> None:
     """Yield a basic uEdition application."""
     cwd = os.getcwd()
-    os.chdir('tests/fixtures/basic')
+    os.chdir("tests/fixtures/basic")
     from uedition.cli import app
     from uedition.settings import reload_settings
+
     reload_settings()
     yield app
     os.chdir(cwd)
 
 
 @fixture
 def yaml_app() -> None:
     """Yield a basic application initiated from a folder with a .yaml file."""
     cwd = os.getcwd()
-    os.chdir('tests/fixtures/yaml')
+    os.chdir("tests/fixtures/yaml")
     from uedition.cli import app
     from uedition.settings import reload_settings
+
     reload_settings()
     yield app
     os.chdir(cwd)
 
 
 @fixture
 def multilang_app() -> None:
     """Yield a fully featured application with multiple languages configured."""
     cwd = os.getcwd()
-    os.chdir('tests/fixtures/multilang')
-    if os.path.exists('docs'):  # noqa: cov
-        rmtree('docs')
-    if os.path.exists('en/_build'):  # noqa: cov
-        rmtree('en/_build')
-    if os.path.exists('de/_build'):  # noqa: cov
-        rmtree('de/_build')
+    os.chdir("tests/fixtures/multilang")
+    if os.path.exists("docs"):  # noqa: cov
+        rmtree("docs")
+    if os.path.exists("en/_build"):  # noqa: cov
+        rmtree("en/_build")
+    if os.path.exists("de/_build"):  # noqa: cov
+        rmtree("de/_build")
     from uedition.cli import app
     from uedition.settings import reload_settings
+
     reload_settings()
     yield app
     os.chdir(cwd)
 
 
 @fixture
 def missing_core_files_app() -> None:
     """Yield a basic application where the core _config.yml and _toc.yml files are missing."""
     cwd = os.getcwd()
-    os.chdir('tests/fixtures/missing_core_files')
+    os.chdir("tests/fixtures/missing_core_files")
     from uedition.cli import app
     from uedition.settings import reload_settings
+
     reload_settings()
     yield app
     os.chdir(cwd)
 
 
 @fixture
 def invalid_core_files_app() -> None:
     """Yield a basic application where the core _config.yml and _toc.yml files are invalid YAML."""
     cwd = os.getcwd()
-    os.chdir('tests/fixtures/invalid_core_files')
+    os.chdir("tests/fixtures/invalid_core_files")
     from uedition.cli import app
     from uedition.settings import reload_settings
+
     reload_settings()
     yield app
     os.chdir(cwd)
 
 
 @fixture
 def missing_toc_root_app() -> None:
     """Yield a basic application where the _toc.yml file is missing the root entry."""
     cwd = os.getcwd()
-    os.chdir('tests/fixtures/missing_toc_root')
+    os.chdir("tests/fixtures/missing_toc_root")
     from uedition.cli import app
     from uedition.settings import reload_settings
+
     reload_settings()
     yield app
     os.chdir(cwd)
 
 
 @fixture
 def missing_toc_root_file_app() -> None:
     """Yield a basic application where the _toc.yml file points to a missing root file."""
     cwd = os.getcwd()
-    os.chdir('tests/fixtures/missing_toc_root_file')
+    os.chdir("tests/fixtures/missing_toc_root_file")
     from uedition.cli import app
     from uedition.settings import reload_settings
+
     reload_settings()
     yield app
     os.chdir(cwd)
 
 
 @fixture
 def missing_files_app() -> None:
     """Yield a basic application where some files are missing root file."""
     cwd = os.getcwd()
-    os.chdir('tests/fixtures/missing_files')
+    os.chdir("tests/fixtures/missing_files")
     from uedition.cli import app
     from uedition.settings import reload_settings
+
     reload_settings()
     yield app
     os.chdir(cwd)
```

### Comparing `uedition-0.3.1/tests/test_build.py` & `uedition-0.4.0/tests/test_build.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,17 +1,17 @@
 """Tests for the 'build' functionality."""
 from typer import Typer
 from typer.testing import CliRunner
 
 
 def test_basic_build(runner: CliRunner, multilang_app: Typer) -> None:
     """Test that the basic build works."""
-    result = runner.invoke(multilang_app, ['build'])
+    result = runner.invoke(multilang_app, ["build"])
     assert result.exit_code == 0
 
 
 def test_basic_build_rebuild(runner: CliRunner, multilang_app: Typer) -> None:
     """Test that rebuilding works."""
-    result = runner.invoke(multilang_app, ['build'])
+    result = runner.invoke(multilang_app, ["build"])
     assert result.exit_code == 0
-    result = runner.invoke(multilang_app, ['build'])
+    result = runner.invoke(multilang_app, ["build"])
     assert result.exit_code == 0
```

### Comparing `uedition-0.3.1/tests/test_check.py` & `uedition-0.4.0/tests/test_check.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,53 +1,59 @@
 """Tests for the check functionality."""
 from typer import Typer
 from typer.testing import CliRunner
 
 
 def test_check_multilang(runner: CliRunner, multilang_app: Typer) -> None:
     """Test that a correctly setup uEdition throws no errors."""
-    result = runner.invoke(multilang_app, ['check'])
+    result = runner.invoke(multilang_app, ["check"])
     assert result.exit_code == 0
-    assert 'All checks successfully passed' in result.stdout
+    assert "All checks successfully passed" in result.stdout
 
 
-def test_check_missing_core_files(runner: CliRunner, missing_core_files_app: Typer) -> None:
+def test_check_missing_core_files(
+    runner: CliRunner, missing_core_files_app: Typer
+) -> None:
     """Test that missing core files (_config.yml, _toc.yml) are correctly reported."""
-    result = runner.invoke(missing_core_files_app, ['check'])
+    result = runner.invoke(missing_core_files_app, ["check"])
     assert result.exit_code == 1
-    assert 'The following errors were found' in result.stdout
-    assert 'Missing configuration file en/_config.yml' in result.stdout
-    assert 'Missing toc file en/_toc.yml' in result.stdout
+    assert "The following errors were found" in result.stdout
+    assert "Missing configuration file en/_config.yml" in result.stdout
+    assert "Missing toc file en/_toc.yml" in result.stdout
 
 
-def test_check_invalid_core_files_app(runner: CliRunner, invalid_core_files_app: Typer) -> None:
+def test_check_invalid_core_files_app(
+    runner: CliRunner, invalid_core_files_app: Typer
+) -> None:
     """Test that missing core files (_config.yml, _toc.yml) are correctly reported."""
-    result = runner.invoke(invalid_core_files_app, ['check'])
+    result = runner.invoke(invalid_core_files_app, ["check"])
     assert result.exit_code == 1
-    assert 'The following errors were found' in result.stdout
-    assert 'en/_config.yml' in result.stdout
-    assert 'en/_toc.yml' in result.stdout
-    assert 'mapping values are not allowed here' in result.stdout
+    assert "The following errors were found" in result.stdout
+    assert "en/_config.yml" in result.stdout
+    assert "en/_toc.yml" in result.stdout
+    assert "mapping values are not allowed here" in result.stdout
 
 
 def test_missing_toc_root(runner: CliRunner, missing_toc_root_app: Typer) -> None:
     """Test that a missing toc root entry is correctly reported."""
-    result = runner.invoke(missing_toc_root_app, ['check'])
+    result = runner.invoke(missing_toc_root_app, ["check"])
     assert result.exit_code == 1
-    assert 'The following errors were found' in result.stdout
-    assert 'No root in en/_toc.yml' in result.stdout
+    assert "The following errors were found" in result.stdout
+    assert "No root in en/_toc.yml" in result.stdout
 
 
-def test_missing_toc_root_file(runner: CliRunner, missing_toc_root_file_app: Typer) -> None:
+def test_missing_toc_root_file(
+    runner: CliRunner, missing_toc_root_file_app: Typer
+) -> None:
     """Test that a missing root file is correctly reported."""
-    result = runner.invoke(missing_toc_root_file_app, ['check'])
+    result = runner.invoke(missing_toc_root_file_app, ["check"])
     assert result.exit_code == 1
-    assert 'The following errors were found' in result.stdout
-    assert 'Root in en/_toc.yml points to missing file missing.md' in result.stdout
+    assert "The following errors were found" in result.stdout
+    assert "Root in en/_toc.yml points to missing file missing.md" in result.stdout
 
 
 def test_missing_files(runner: CliRunner, missing_files_app: Typer) -> None:
     """Test that missing files are correctly reported."""
-    result = runner.invoke(missing_files_app, ['check'])
+    result = runner.invoke(missing_files_app, ["check"])
     assert result.exit_code == 1
-    assert 'The following errors were found' in result.stdout
-    assert 'File a-page.md missing in en/_toc.yml' in result.stdout
+    assert "The following errors were found" in result.stdout
+    assert "File a-page.md missing in en/_toc.yml" in result.stdout
```

### Comparing `uedition-0.3.1/tests/test_settings.py` & `uedition-0.4.0/tests/test_settings.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 """Tests for the core settings functionality."""
 from typer import Typer
 from typer.testing import CliRunner
 
 
 def test_empty_defaults(runner: CliRunner, empty_app: Typer) -> None:
     """Test that running in an empty directory works."""
-    result = runner.invoke(empty_app, ['version'])
+    result = runner.invoke(empty_app, ["version"])
     assert result.exit_code == 0
 
 
 def test_load_from_yaml(runner: CliRunner, yaml_app: Typer) -> None:
     """Test that loading the configuration from a .yaml file works."""
-    result = runner.invoke(yaml_app, ['version'])
+    result = runner.invoke(yaml_app, ["version"])
     assert result.exit_code == 0
```

### Comparing `uedition-0.3.1/tests/fixtures/missing_files/references.bib` & `uedition-0.4.0/tests/fixtures/missing_files/references.bib`

 * *Files identical despite different names*

### Comparing `uedition-0.3.1/tests/fixtures/missing_files/en/_config.yml` & `uedition-0.4.0/tests/fixtures/missing_files/en/_config.yml`

 * *Files identical despite different names*

### Comparing `uedition-0.3.1/tests/fixtures/multilang/references.bib` & `uedition-0.4.0/tests/fixtures/multilang/references.bib`

 * *Files identical despite different names*

### Comparing `uedition-0.3.1/tests/fixtures/multilang/de/_config.yml` & `uedition-0.4.0/tests/fixtures/multilang/de/_config.yml`

 * *Files identical despite different names*

### Comparing `uedition-0.3.1/tests/fixtures/multilang/en/_config.yml` & `uedition-0.4.0/tests/fixtures/multilang/en/_config.yml`

 * *Files identical despite different names*

### Comparing `uedition-0.3.1/uedition/settings.py` & `uedition-0.4.0/uedition/settings.py`

 * *Files 13% similar despite different names*

```diff
@@ -8,19 +8,23 @@
 from pydantic.env_settings import SettingsSourceCallable
 from yaml import safe_load
 from typing import Any
 
 
 def uedition_yaml_settings(settings: BaseSettings) -> dict[str, Any]:
     """Load the settings from a uEdition.yaml or uEdition.yml file."""
-    if os.path.exists('uEdition.yaml'):
-        with open('uEdition.yaml', encoding=settings.__config__.env_file_encoding) as in_f:
+    if os.path.exists("uEdition.yaml"):
+        with open(
+            "uEdition.yaml", encoding=settings.__config__.env_file_encoding
+        ) as in_f:
             return safe_load(in_f)
-    elif os.path.exists('uEdition.yml'):
-        with open('uEdition.yml', encoding=settings.__config__.env_file_encoding) as in_f:
+    elif os.path.exists("uEdition.yml"):
+        with open(
+            "uEdition.yml", encoding=settings.__config__.env_file_encoding
+        ) as in_f:
             return safe_load(in_f)
     return dict()
 
 
 class LanguageSetting(BaseModel):
     """Settings for a single language."""
 
@@ -31,33 +35,38 @@
     path: str
     """The path the language's content is at."""
 
 
 class Settings(BaseSettings):
     """Application settings."""
 
-    version: str = '1'
+    version: str = "1"
     """The configuration file version."""
     languages: list[LanguageSetting] = []
     """The configured languages."""
-    output: str = 'docs'
+    output: str = "docs"
     """The output directory."""
 
     class Config:
         """Configuration overrides."""
 
         @classmethod
         def customise_sources(
             cls,  # noqa: ANN102
             init_settings: SettingsSourceCallable,
             env_settings: SettingsSourceCallable,
             file_secret_settings: SettingsSourceCallable,
         ) -> tuple[SettingsSourceCallable, ...]:
             """Add the YAMl loading functionality."""
-            return env_settings, init_settings, file_secret_settings, uedition_yaml_settings
+            return (
+                env_settings,
+                init_settings,
+                file_secret_settings,
+                uedition_yaml_settings,
+            )
 
 
 settings = Settings().dict()
 
 
 def reload_settings() -> None:
     """Reload the settings."""
```

### Comparing `uedition-0.3.1/uedition/cli/__init__.py` & `uedition-0.4.0/uedition/cli/__init__.py`

 * *Files 8% similar despite different names*

```diff
@@ -31,9 +31,9 @@
     """Check that the μEdition is set up correctly."""
     check_module.run()
 
 
 @app.command()
 def version() -> None:
     """Output the current μEdition version."""
-    print_cli(f'μEdition: {__version__}')
+    print_cli(f"μEdition: {__version__}")
     print_cli(f'Configuration: {settings["version"]}')
```

### Comparing `uedition-0.3.1/uedition/cli/build.py` & `uedition-0.4.0/uedition/cli/build.py`

 * *Files 12% similar despite different names*

```diff
@@ -6,20 +6,21 @@
 from shutil import rmtree, copytree
 
 from ..settings import settings
 
 
 def landing_build() -> None:
     """Build the landing page."""
-    if not path.exists(settings['output']):
-        makedirs(settings['output'], exist_ok=True)
-    with open(path.join(settings['output'], 'config.json'), 'w') as out_f:
+    if not path.exists(settings["output"]):
+        makedirs(settings["output"], exist_ok=True)
+    with open(path.join(settings["output"], "config.json"), "w") as out_f:
         json.dump(settings, out_f)
-    with open(path.join(settings['output'], 'index.html'), 'w') as out_f:
-        out_f.write('''\
+    with open(path.join(settings["output"], "index.html"), "w") as out_f:
+        out_f.write(
+            """\
 <!DOCTYPE html>
 <html>
   <head>
     <meta name="charset" value="utf-8">
     <title>Redirecting... Please wait...</title>
   </head>
   <body>
@@ -55,38 +56,56 @@
           window.location = window.location.href + config.languages[0].path;
         }
       }
       redirect();
     </script>
   </body>
 </html>
-''')
+"""
+        )
 
 
 def full_build(lang: dict) -> None:
     """Run the full build process for a single language."""
     landing_build()
-    subprocess.run(['jupyter-book', 'build', '--all', '--path-output', path.join('_build', lang['code']), lang['path']])
+    subprocess.run(
+        [
+            "jupyter-book",
+            "build",
+            "--all",
+            "--path-output",
+            path.join("_build", lang["code"]),
+            lang["path"],
+        ]
+    )
     copytree(
-        path.join('_build', lang['code'], '_build', 'html'),
-        path.join(settings['output'], lang['code']),
-        dirs_exist_ok=True
+        path.join("_build", lang["code"], "_build", "html"),
+        path.join(settings["output"], lang["code"]),
+        dirs_exist_ok=True,
     )
 
 
 def partial_build(lang: dict) -> None:
     """Run the as-needed build process for a single language."""
     landing_build()
-    subprocess.run(['jupyter-book', 'build', '--path-output', path.join('_build', lang['code']), lang['path']])
+    subprocess.run(
+        [
+            "jupyter-book",
+            "build",
+            "--path-output",
+            path.join("_build", lang["code"]),
+            lang["path"],
+        ]
+    )
     copytree(
-        path.join('_build', lang['code'], '_build', 'html'),
-        path.join(settings['output'], lang['code']),
-        dirs_exist_ok=True
+        path.join("_build", lang["code"], "_build", "html"),
+        path.join(settings["output"], lang["code"]),
+        dirs_exist_ok=True,
     )
 
 
 def run() -> None:
     """Build the full uEdition."""
-    if path.exists(settings['output']):
-        rmtree(settings['output'])
-    for lang in settings['languages']:
+    if path.exists(settings["output"]):
+        rmtree(settings["output"])
+    for lang in settings["languages"]:
         full_build(lang)
```

### Comparing `uedition-0.3.1/uedition/cli/check.py` & `uedition-0.4.0/uedition/cli/check.py`

 * *Files 19% similar despite different names*

```diff
@@ -12,177 +12,191 @@
 
 from ..settings import settings
 
 
 def collect_files(toc: dict) -> list[str]:
     """Collect all files from a TOC."""
     files = []
-    if 'parts' in toc:
-        for part in toc['parts']:
+    if "parts" in toc:
+        for part in toc["parts"]:
             files.extend(collect_files(part))
-    elif 'chapters' in toc:
-        for chapter in toc['chapters']:
-            files.append(chapter['file'])
+    elif "chapters" in toc:
+        for chapter in toc["chapters"]:
+            files.append(chapter["file"])
             files.extend(collect_files(chapter))
-    elif 'sections' in toc:
-        for sections in toc['sections']:
-            files.append(sections['file'])
+    elif "sections" in toc:
+        for sections in toc["sections"]:
+            files.append(sections["file"])
     return files
 
 
-def compare_tocs(prefix: str, toc_a: dict, toc_b: dict) -> list[tuple[str | None, str | None]]:
+def compare_tocs(
+    prefix: str, toc_a: dict, toc_b: dict
+) -> list[tuple[str | None, str | None]]:
     """Recursively compare the structure of two TOCs."""
     mismatches = []
-    if 'parts' in toc_a and 'parts' in toc_b:
+    if "parts" in toc_a and "parts" in toc_b:
         pass
-    elif 'chapters' in toc_a and 'chapters' in toc_b:
+    elif "chapters" in toc_a and "chapters" in toc_b:
         pass
-    elif 'sections' in toc_a and 'sections' in toc_b:
+    elif "sections" in toc_a and "sections" in toc_b:
         pass
-    elif 'parts' in toc_a:
-        mismatches.append((f'{prefix}has parts, which are missing from'))
-    elif 'chapters' in toc_a:
-        mismatches.append((f'{prefix}has chapters, which are missing from'))
-    elif 'sections' in toc_b:
-        mismatches.append((f'{prefix}has sections, which are missing from'))
+    elif "parts" in toc_a:
+        mismatches.append((f"{prefix}has parts, which are missing from"))
+    elif "chapters" in toc_a:
+        mismatches.append((f"{prefix}has chapters, which are missing from"))
+    elif "sections" in toc_b:
+        mismatches.append((f"{prefix}has sections, which are missing from"))
     return mismatches
 
 
 class ConfigurationFileChecks(Thread):
     """Basic configuration file checks."""
 
-    def __init__(self: 'ConfigurationFileChecks', progress: Progress, task: int) -> None:
+    def __init__(
+        self: "ConfigurationFileChecks", progress: Progress, task: int
+    ) -> None:
         """Initialise the thread."""
         super().__init__(group=None)
         self._progress = progress
         self._task = task
         self.errors = []
 
-    def run(self: 'ConfigurationFileChecks') -> None:
+    def run(self: "ConfigurationFileChecks") -> None:
         """Run the checks."""
-        for lang in settings['languages']:
-            yaml_path = os.path.join(lang['path'], '_config.yml')
+        for lang in settings["languages"]:
+            yaml_path = os.path.join(lang["path"], "_config.yml")
             if os.path.exists(yaml_path):
                 with open(yaml_path) as in_f:
                     try:
                         safe_load(in_f)
                     except Exception as e:
                         self.errors.append(str(e))
             else:
-                self.errors.append(f'Missing configuration file {yaml_path}')
+                self.errors.append(f"Missing configuration file {yaml_path}")
             self._progress.update(self._task, advance=1)
 
 
 class TocFileChecks(Thread):
     """TOC file checks."""
 
-    def __init__(self: 'TocFileChecks', progress: Progress, task: int) -> None:
+    def __init__(self: "TocFileChecks", progress: Progress, task: int) -> None:
         """Initialise the thread."""
         super().__init__(group=None)
         self._progress = progress
         self._task = task
         self.errors = []
 
-    def run(self: 'TocFileChecks') -> None:
+    def run(self: "TocFileChecks") -> None:
         """Run the checks."""
-        for lang in settings['languages']:
-            yaml_path = os.path.join(lang['path'], '_toc.yml')
+        for lang in settings["languages"]:
+            yaml_path = os.path.join(lang["path"], "_toc.yml")
             if os.path.exists(yaml_path):
                 with open(yaml_path) as in_f:
                     try:
                         toc = safe_load(in_f)
-                        if 'root' in toc:
-                            root_path = os.path.join(lang['path'], f'{toc["root"]}.md')
+                        if "root" in toc:
+                            root_path = os.path.join(lang["path"], f'{toc["root"]}.md')
                             if not os.path.exists(root_path):
-                                self.errors.append(f'Root in {yaml_path} points to missing file {toc["root"]}.md')
+                                self.errors.append(
+                                    f'Root in {yaml_path} points to missing file {toc["root"]}.md'
+                                )
                             root_base = os.path.dirname(root_path)
                             for filename in collect_files(toc):
-                                if not os.path.exists(os.path.join(root_base, f'{filename}.md')):
-                                    self.errors.append(f'File {filename}.md missing in {yaml_path}')
+                                if not os.path.exists(
+                                    os.path.join(root_base, f"{filename}.md")
+                                ):
+                                    self.errors.append(
+                                        f"File {filename}.md missing in {yaml_path}"
+                                    )
                         else:
-                            self.errors.append(f'No root in {yaml_path}')
+                            self.errors.append(f"No root in {yaml_path}")
                     except Exception as e:
                         self.errors.append(str(e))
             else:
-                self.errors.append(f'Missing toc file {yaml_path}')
+                self.errors.append(f"Missing toc file {yaml_path}")
             self._progress.update(self._task, advance=1)
 
 
 class LanguageConsistencyChecks(Thread):
     """Multi-language consistency checks."""
 
-    def __init__(self: 'LanguageConsistencyChecks', progress: Progress, task: int) -> None:
+    def __init__(
+        self: "LanguageConsistencyChecks", progress: Progress, task: int
+    ) -> None:
         """Initialise the thread."""
         super().__init__(group=None)
         self._progress = progress
         self._task = task
         self.errors = []
 
-    def run(self: 'LanguageConsistencyChecks') -> None:
+    def run(self: "LanguageConsistencyChecks") -> None:
         """Run the checks."""
-        if len(settings['languages']) == 0:
+        if len(settings["languages"]) == 0:
             return
-        base_toc_path = os.path.join(settings['languages'][0]['path'], '_toc.yml')
+        base_toc_path = os.path.join(settings["languages"][0]["path"], "_toc.yml")
         if not os.path.exists(base_toc_path):
             return
         with open(base_toc_path) as in_f:
             try:
                 base_toc = safe_load(in_f)
             except Exception:
                 return
-        for lang in settings['languages'][1:]:
-            lang_toc_path = os.path.join(lang['path'], '_toc.yml')
+        for lang in settings["languages"][1:]:
+            lang_toc_path = os.path.join(lang["path"], "_toc.yml")
             if not os.path.exists(lang_toc_path):
                 continue
             try:
                 with open(lang_toc_path) as in_f:
                     lang_toc = safe_load(in_f)
             except Exception:
                 continue
-            missmatches = compare_tocs('', base_toc, lang_toc)
+            missmatches = compare_tocs("", base_toc, lang_toc)
             if len(missmatches) > 0:
                 for mismatch in missmatches:
                     if mismatch[0] is None:
-                        self.errors.append(f'{base_toc_path} {mismatch[1]} {lang_toc_path}')
+                        self.errors.append(
+                            f"{base_toc_path} {mismatch[1]} {lang_toc_path}"
+                        )
                     elif mismatch[0] is None:
-                        self.errors.append(f'{lang_toc_path} {mismatch[0]} {base_toc_path}')
+                        self.errors.append(
+                            f"{lang_toc_path} {mismatch[0]} {base_toc_path}"
+                        )
 
 
 def run() -> None:
     """Check that the μEdition is correctly set up."""
     errors = []
     with Progress() as progress:
         threads = [
             ConfigurationFileChecks(
                 progress,
                 progress.add_task(
-                    '[green]Configuration file checks',
-                    total=len(settings['languages'])
-                )
+                    "[green]Configuration file checks", total=len(settings["languages"])
+                ),
             ),
             TocFileChecks(
                 progress,
                 progress.add_task(
-                    '[green]TOC file checks',
-                    total=len(settings['languages'])
-                )
+                    "[green]TOC file checks", total=len(settings["languages"])
+                ),
             ),
             LanguageConsistencyChecks(
                 progress,
                 progress.add_task(
-                    '[green]Language consistency checks',
-                    total=len(settings['languages']) - 1
-                )
-            )
+                    "[green]Language consistency checks",
+                    total=len(settings["languages"]) - 1,
+                ),
+            ),
         ]
         for thread in threads:
             thread.start()
         for thread in threads:
             thread.join()
             errors.extend(thread.errors)
     if len(errors) > 0:
-        print_cli('[red]:bug: The following errors were found:')
+        print_cli("[red]:bug: The following errors were found:")
         for error in errors:
-            print_cli(f'[red]* {error}')
+            print_cli(f"[red]* {error}")
         raise typer.Exit(code=1)
     else:
-        print_cli('[green]:+1: All checks successfully passed')
+        print_cli("[green]:+1: All checks successfully passed")
```

### Comparing `uedition-0.3.1/uedition/cli/serve.py` & `uedition-0.4.0/uedition/cli/serve.py`

 * *Files 13% similar despite different names*

```diff
@@ -6,28 +6,34 @@
 from .build import full_build, partial_build
 from ..settings import settings
 
 
 def build_cmd(lang: dict, full: bool = True) -> Callable[[], None]:
     """Create a function that (re-)builds one of the sub-sites."""
     if full:
+
         def cmd() -> None:
             full_build(lang)
+
         return cmd
     else:
+
         def cmd() -> None:
             partial_build(lang)
+
         return cmd
 
 
 def run() -> None:
     """Run the development server."""
-    full_rebuilds = [build_cmd(lang, full=True) for lang in settings['languages']]
-    partial_rebuilds = [build_cmd(lang, full=False) for lang in settings['languages']]
+    full_rebuilds = [build_cmd(lang, full=True) for lang in settings["languages"]]
+    partial_rebuilds = [build_cmd(lang, full=False) for lang in settings["languages"]]
     for cmd in full_rebuilds:
         cmd()
     server = Server()
-    for lang, full_cmd, partial_cmd in zip(settings['languages'], full_rebuilds, partial_rebuilds):
-        server.watch(path.join(lang['path'], '*.yml'), full_cmd)
-        server.watch(path.join(lang['path'], '**', '*.*'), partial_cmd)
-    server.watch('uEdition.*', lambda: [cmd() for cmd in full_rebuilds])
-    server.serve(root='site', port=8000)
+    for lang, full_cmd, partial_cmd in zip(
+        settings["languages"], full_rebuilds, partial_rebuilds
+    ):
+        server.watch(path.join(lang["path"], "*.yml"), full_cmd)
+        server.watch(path.join(lang["path"], "**", "*.*"), partial_cmd)
+    server.watch("uEdition.*", lambda: [cmd() for cmd in full_rebuilds])
+    server.serve(root="site", port=8000)
```

### Comparing `uedition-0.3.1/uedition/ext/config.py` & `uedition-0.4.0/uedition/ext/config.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,15 +1,14 @@
 """uEdition configuration handling.
 
 This module handles reading the uEdition-specific configuration settings, validating them and
 adding any required default values.
 """
 from pydantic import BaseModel, validator, ValidationError
 from sphinx.application import Sphinx
-from sphinx.config import Config
 from sphinx.util import logging
 from typing import Union, Literal, Optional
 
 
 logger = logging.getLogger(__name__)
 
 
@@ -22,102 +21,111 @@
 
 class RuleSelector(BaseModel):
     """Validation rule for the selector for matching a TEI tag."""
 
     tag: str
     attributes: list[RuleSelectorAttribute] = []
 
-    @validator('tag', pre=True)
-    def expand_tag_namespace(cls, v, values, **kwargs) -> str:
-        """Expand any ```tei:``` namespace prefixes. """
-        return v.replace('tei:', '{http://www.tei-c.org/ns/1.0}')
-
-    @validator('attributes', pre=True)
-    def convert_dict_attributes_to_list(cls, v, values, **kwargs) -> list[dict]:
+    @validator("tag", pre=True)
+    def expand_tag_namespace(
+        cls: "RuleSelector", v: str, values: dict, **kwargs: dict
+    ) -> str:
+        """Expand any ```tei:``` namespace prefixes."""
+        return v.replace("tei:", "{http://www.tei-c.org/ns/1.0}")
+
+    @validator("attributes", pre=True)
+    def convert_dict_attributes_to_list(
+        cls: "RuleSelector", v: dict | list, values: dict, **kwargs: dict
+    ) -> list[dict]:
         """Convert a single attributes dictionary to a list with that dictionary."""
         if isinstance(v, dict):
             return [v]
         return v
 
 
 class RuleText(BaseModel):
     """Validation rule for retrieving the text content from an attribute."""
 
-    action: Literal['from-attribute']
+    action: Literal["from-attribute"]
     attr: str
 
 
 class RuleAttributeCopy(BaseModel):
     """Validation rule for copying and attribute."""
 
-    action: Literal['copy'] = 'copy'
+    action: Literal["copy"] = "copy"
     attr: str
     source: str
 
 
 class RuleAttributeSet(BaseModel):
     """Validation rule for settings an attribute to a specific value."""
 
-    action: Literal['set']
+    action: Literal["set"]
     attr: str
     value: str
 
 
 class RuleAttributeDelete(BaseModel):
     """Validation rule for deleting an attribute."""
 
-    action: Literal['delete']
+    action: Literal["delete"]
     attr: str
 
 
 class Rule(BaseModel):
     """Validation model for a rule transforming a TEI tag into a HTML tag."""
 
     selector: RuleSelector
-    tag: Union[str, None] = 'div'
+    tag: Union[str, None] = "div"
     text: Union[RuleText, None] = None
-    attributes: list[Union[RuleAttributeCopy, RuleAttributeSet, RuleAttributeDelete]] = []
-
-    @validator('selector', pre=True)
-    def convert_str_selector_to_dict(cls, v, values, **kwargs) -> dict:
+    attributes: list[
+        Union[RuleAttributeCopy, RuleAttributeSet, RuleAttributeDelete]
+    ] = []
+
+    @validator("selector", pre=True)
+    def convert_str_selector_to_dict(
+        cls: "Rule", v: str | dict, values: dict, **kwargs: dict
+    ) -> dict:
+        """Convert a simple string selector into the dictionary representation."""
         if isinstance(v, str):
-            return {'tag': v}
+            return {"tag": v}
         return v
 
 
 class TextSection(BaseModel):
     """Validation model for a TEI text section."""
 
     title: str
-    type: Literal['text'] = 'text'
+    type: Literal["text"] = "text"
     content: str
     mappings: list[Rule] = []
 
 
 class SingleFieldRule(BaseModel):
     """Validation model for a TEI field rule."""
 
     title: str
-    type: Literal['single'] = 'single'
+    type: Literal["single"] = "single"
     content: str
 
 
 class ListFieldRule(BaseModel):
     """Validation model for a TEI field rule."""
 
     title: str
-    type: Literal['list']
+    type: Literal["list"]
     content: str
 
 
 class FieldsSection(BaseModel):
     """Validation model for a TEI fields section."""
 
     title: str
-    type: Literal['fields']
+    type: Literal["fields"]
     fields: list[SingleFieldRule | ListFieldRule]
 
 
 class TEIConfig(BaseModel):
     """Validation model for the TEI-specific settings."""
 
     text_only_in_leaf_nodes: bool = False
@@ -128,56 +136,68 @@
 class Config(BaseModel):
     """Configuration validation model."""
 
     tei: Optional[TEIConfig]
 
 
 BASE_RULES = [
-    {'selector': 'tei:body', 'tag': 'section'},
-    {'selector': 'tei:head', 'tag': 'h1'},
-    {'selector': 'tei:p', 'tag': 'p'},
-
-    {'selector': 'tei:seg', 'tag': 'span'},
-    {'selector': 'tei:pb', 'tag': 'span'},
-    {'selector': 'tei:hi', 'tag': 'span'},
+    {"selector": "tei:body", "tag": "section"},
+    {"selector": "tei:head", "tag": "h1"},
+    {"selector": "tei:p", "tag": "p"},
+    {"selector": "tei:seg", "tag": "span"},
+    {"selector": "tei:pb", "tag": "span"},
+    {"selector": "tei:hi", "tag": "span"},
     {
-        'selector': 'tei:ref',
-        'tag': 'a',
-        'attributes': [
-            {'attr': 'href', 'source': 'target'}
-        ]
+        "selector": "tei:ref",
+        "tag": "a",
+        "attributes": [{"attr": "href", "source": "target"}],
     },
-    {'selector': 'tei:citedRange', 'tag': 'span'},
-    {'selector': 'tei:q', 'tag': 'span'},
-    {'selector': 'tei:hi', 'tag': 'span'},
-    {'selector': 'tei:foreign', 'tag': 'span'},
-    {'selector': 'tei:speaker', 'tag': 'span'},
-    {'selector': 'tei:stage', 'tag': 'span'},
-    {'selector': 'tei:lem', 'tag': 'span'},
-    {'selector': 'tei:sic', 'tag': 'span'},
+    {"selector": "tei:citedRange", "tag": "span"},
+    {"selector": "tei:q", "tag": "span"},
+    {"selector": "tei:hi", "tag": "span"},
+    {"selector": "tei:foreign", "tag": "span"},
+    {"selector": "tei:speaker", "tag": "span"},
+    {"selector": "tei:stage", "tag": "span"},
+    {"selector": "tei:lem", "tag": "span"},
+    {"selector": "tei:sic", "tag": "span"},
 ]
 """Base mapping rules for mapping TEI tags to default HTML elements."""
 
 
 def validate_config(app: Sphinx, config: Config) -> None:
     """Validate the configuration and add any default values."""
-    if 'tei' in config.uEdition:
-        if 'sections' in config.uEdition['tei'] and isinstance(config.uEdition['tei']['sections'], list):
-            if 'mappings' in config.uEdition['tei'] and isinstance(config.uEdition['tei']['mappings'], list):
-                for section in config.uEdition['tei']['sections']:
-                    if 'mappings' in section and isinstance(section['mappings'], list):
-                        section['mappings'] = section['mappings'] + config.uEdition['tei']['mappings'] + BASE_RULES
-                    else:
-                        section['mappings'] = config.uEdition['tei']['mappings'] + BASE_RULES
-    try:
-        config.uEdition = Config(**config.uEdition).dict()
-    except ValidationError as e:
-        for error in e.errors():
-            logger.error(' -> '.join([str(l) for l in error['loc']]))
-            logger.error(f'  {error["msg"]}')
+    if config.uEdition:
+        if "tei" in config.uEdition:
+            if "sections" in config.uEdition["tei"] and isinstance(
+                config.uEdition["tei"]["sections"], list
+            ):
+                if "mappings" in config.uEdition["tei"] and isinstance(
+                    config.uEdition["tei"]["mappings"], list
+                ):
+                    for section in config.uEdition["tei"]["sections"]:
+                        if "mappings" in section and isinstance(
+                            section["mappings"], list
+                        ):
+                            section["mappings"] = (
+                                section["mappings"]
+                                + config.uEdition["tei"]["mappings"]
+                                + BASE_RULES
+                            )
+                        else:
+                            section["mappings"] = (
+                                config.uEdition["tei"]["mappings"] + BASE_RULES
+                            )
+        try:
+            config.uEdition = Config(**config.uEdition).dict()
+        except ValidationError as e:
+            for error in e.errors():
+                logger.error(" -> ".join([str(loc) for loc in error["loc"]]))
+                logger.error(f'  {error["msg"]}')
+            config.uEdition = {}
+    else:
         config.uEdition = {}
 
 
 def setup(app: Sphinx) -> None:
-    """Setup the Sphinx configuration handling for the uEdition."""
-    app.add_config_value('uEdition', default=None, rebuild='html', types=[dict])
-    app.connect('config-inited', validate_config)
+    """Set up the Sphinx configuration handling for the uEdition."""
+    app.add_config_value("uEdition", default=None, rebuild="html", types=[dict])
+    app.connect("config-inited", validate_config)
```

### Comparing `uedition-0.3.1/uedition/ext/tei.py` & `uedition-0.4.0/uedition/ext/tei.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,156 +1,180 @@
+"""TEI parsing extension for Sphinx."""
 from docutils import nodes
-from docutils.parsers.rst import Parser as RstParser
 from lxml import etree
 from sphinx.application import Sphinx
 from sphinx.parsers import Parser as SphinxParser
-from sphinx.util import logging
-from sphinx_design.shared import create_component
+from sphinx.writers.html import HTMLWriter
 
 
-namespaces = {'tei': 'http://www.tei-c.org/ns/1.0'}
+namespaces = {"tei": "http://www.tei-c.org/ns/1.0"}
 
 
-class TeiElement(nodes.Element): pass
+class TeiElement(nodes.Element):
+    """An abstract TEI element for HTML rendering."""
 
+    pass
 
-def tei_element_html_enter(self, node: TeiElement) -> None:
-    if node.get('html_tag') is not None:
+
+def tei_element_html_enter(self: "HTMLWriter", node: TeiElement) -> None:
+    """Visit a TeiElement and generate the correct HTML."""
+    if node.get("html_tag") is not None:
         buffer = [f'<{node.get("html_tag")} data-tei-tag="{node.get("tei_tag")[29:]}"']
-        if node.get('ids'):
+        if node.get("ids"):
             buffer.append(f' id="{node.get("ids")[0]}"')
-        for key, value in node.get('tei_attributes').items():
+        for key, value in node.get("tei_attributes").items():
             buffer.append(f' {key}="{value}"')
         self.body.append(f'{"".join(buffer)}>')
 
 
-def tei_element_html_exit(self, node: TeiElement) -> None:
-    if node.get('html_tag') is not None:
+def tei_element_html_exit(self: "HTMLWriter", node: TeiElement) -> None:
+    """Close the HTML tag."""
+    if node.get("html_tag") is not None:
         self.body.append(f'</{node.get("html_tag")}>')
 
 
 class TEIParser(SphinxParser):
     """Sphinx parser for Text Encoding Initiative XML."""
 
-    supported: tuple[str, ...] = ('tei',)
+    supported: tuple[str, ...] = ("tei",)
     """Specify that only .tei files are parsed"""
 
-    def parse(self: 'TEIParser', inputstring: str, document: nodes.document) -> None:
+    def parse(self: "TEIParser", inputstring: str, document: nodes.document) -> None:
         """Parse source TEI text.
 
         This function creates the basic structure and then the :func:`~uEdition.extensions.tei.TEIParser._walk_tree`
         function is used to actually process the XML.
 
         :param inputstring: The TEI XML string to parse
         :type inputstring: str
         :param document: The root docutils node to add AST elements to
         :type document: :class:`~docutils.nodes.document`
         """
-        root = etree.fromstring(inputstring.encode('UTF-8'))
-        title = root.xpath('string(/tei:TEI/tei:teiHeader/tei:fileDesc/tei:titleStmt/tei:title)', namespaces=namespaces)
-        doc_section = nodes.section(ids=['document'])
+        root = etree.fromstring(inputstring.encode("UTF-8"))
+        title = root.xpath(
+            "string(/tei:TEI/tei:teiHeader/tei:fileDesc/tei:titleStmt/tei:title)",
+            namespaces=namespaces,
+        )
+        doc_section = nodes.section(ids=["document"])
         doc_title = nodes.title()
-        doc_title.append(nodes.Text(title if title else '[Untitled]'))
+        doc_title.append(nodes.Text(title if title else "[Untitled]"))
         doc_section.append(doc_title)
-        if 'tei' in self.config.uEdition and 'sections' in self.config.uEdition['tei']:
-            for conf_section in self.config.uEdition['tei']['sections']:
-                section = nodes.section(ids=[nodes.make_id(conf_section['title'])])
+        if "tei" in self.config.uEdition and "sections" in self.config.uEdition["tei"]:
+            for conf_section in self.config.uEdition["tei"]["sections"]:
+                section = nodes.section(ids=[nodes.make_id(conf_section["title"])])
                 section_title = nodes.title()
-                section_title.append(nodes.Text(conf_section['title']))
+                section_title.append(nodes.Text(conf_section["title"]))
                 section.append(section_title)
-                if conf_section['type'] == 'text':
-                    source = root.xpath(conf_section['content'], namespaces=namespaces)
+                if conf_section["type"] == "text":
+                    source = root.xpath(conf_section["content"], namespaces=namespaces)
                     if len(source) > 0:
                         doc_section.append(section)
                         tmp = nodes.section()
                         for child in source:
-                            self._walk_tree(child, tmp, conf_section['mappings'])
+                            self._walk_tree(child, tmp, conf_section["mappings"])
                         self._wrap_sections(section, tmp)
-                elif conf_section['type'] == 'fields':
+                elif conf_section["type"] == "fields":
                     doc_section.append(section)
                     fields = nodes.definition_list()
                     section.append(fields)
-                    for field in conf_section['fields']:
-                        if field['type'] == 'single':
+                    for field in conf_section["fields"]:
+                        if field["type"] == "single":
                             self._parse_single_field(fields, field, root)
-                        elif field['type'] == 'list':
+                        elif field["type"] == "list":
                             self._parse_list_field(fields, field, root)
         document.append(doc_section)
 
-    def _walk_tree(self: 'TEIParser', node: etree.Element, parent: nodes.Element, rules) -> None:
+    def _walk_tree(
+        self: "TEIParser", node: etree.Element, parent: nodes.Element, rules: list
+    ) -> None:
         """Walk the XML tree and create the appropriate AST nodes.
 
         Uses the mapping rules defined in :mod:`~uEdition.extensions.config` to determine what to
         map the XML to.
         """
         is_leaf = len(node) == 0
-        text_only_in_leaf_nodes = self.config.uEdition['tei']['text_only_in_leaf_nodes'] \
-            if 'tei' in self.config.uEdition else False
+        text_only_in_leaf_nodes = (
+            self.config.uEdition["tei"]["text_only_in_leaf_nodes"]
+            if "tei" in self.config.uEdition
+            else False
+        )
         attributes = {}
         # Get the first matching rule for the current node
         rule = self._rule_for_node(node, rules)
         # Loop over the XML node attributes and apply any attribute transforms defined in the matching rule
         for key, value in node.attrib.items():
             # Always strip the namespace from the `id` attribute
-            if key == '{http://www.w3.org/XML/1998/namespace}id':
-                key = 'id'
-            if rule and 'attributes' in rule:
+            if key == "{http://www.w3.org/XML/1998/namespace}id":
+                key = "id"
+            if rule and "attributes" in rule:
                 processed = False
-                for attr_rule in rule['attributes']:
-                    if attr_rule['action'] == 'copy':
-                        if key == attr_rule['source']:
+                for attr_rule in rule["attributes"]:
+                    if attr_rule["action"] == "copy":
+                        if key == attr_rule["source"]:
                             # Copied attributes are added without a `data-` prefix
-                            attributes[attr_rule['attr']] = value
-                    elif attr_rule['action'] == 'delete':
-                        if key == attr_rule['attr']:
+                            attributes[attr_rule["attr"]] = value
+                    elif attr_rule["action"] == "delete":
+                        if key == attr_rule["attr"]:
                             processed = True
-                    elif attr_rule['action'] == 'set':
-                        if key == attr_rule['attr']:
-                            value = attr_rule['value']
+                    elif attr_rule["action"] == "set":
+                        if key == attr_rule["attr"]:
+                            value = attr_rule["value"]
                 # if the attribute did not match any attribute transform
                 if not processed:
                     # The id attribute is always output as is, all other attributes are prefixed with `data-`
-                    if key == 'id':
-                        attributes['id'] = value
+                    if key == "id":
+                        attributes["id"] = value
                     else:
-                        attributes[f'data-{key}'] = value
+                        attributes[f"data-{key}"] = value
             else:
                 # The id attribute is always output as is, all other attributes are prefixed with `data-`
-                if key == 'id':
-                    attributes['id'] = value
+                if key == "id":
+                    attributes["id"] = value
                 else:
-                    attributes[f'data-{key}'] = value
+                    attributes[f"data-{key}"] = value
         # Create the docutils AST element
         new_element = TeiElement(
-            html_tag=rule['tag'] if rule is not None and 'tag' in rule else 'div',
+            html_tag=rule["tag"] if rule is not None and "tag" in rule else "div",
             tei_tag=node.tag,
             tei_attributes=attributes,
         )
         parent.append(new_element)
-        if rule is not None and 'text' in rule and rule['text']:
+        if rule is not None and "text" in rule and rule["text"]:
             # If there is a `text` key in the rule, use that to set the text
-            if rule['text']['action'] == 'from-attribute' and rule['text']['attr'] in node.attrib:
-                new_element.append(nodes.Text(node.attrib[rule['text']['attr']]))
+            if (
+                rule["text"]["action"] == "from-attribute"
+                and rule["text"]["attr"] in node.attrib
+            ):
+                new_element.append(nodes.Text(node.attrib[rule["text"]["attr"]]))
         else:
             if node.text and (is_leaf or not text_only_in_leaf_nodes):
                 # Only create text content if there is text and we either are in a leaf node or are adding all text
                 new_element.append(nodes.Text(node.text))
         # Process any children
         for child in node:
             self._walk_tree(child, new_element, rules)
         # If there is text after this XML node and we are adding all text, then add text content to the parent
         if node.tail and not text_only_in_leaf_nodes:
             parent.append(nodes.Text(node.tail))
 
-    def _wrap_sections(self: 'TEIParser', section: nodes.Element, tmp: nodes.Element) -> None:
+    def _wrap_sections(
+        self: "TEIParser", section: nodes.Element, tmp: nodes.Element
+    ) -> None:
         """Ensure that sections are correctly wrapped."""
         section_stack = [(0, section)]
         for node in tmp.children:
-            if isinstance(node, TeiElement) and node.attributes['html_tag'] in ['h1', 'h2', 'h3', 'h4', 'h5', 'h6']:
-                section_level = int(node.attributes['html_tag'][1])
+            if isinstance(node, TeiElement) and node.attributes["html_tag"] in [
+                "h1",
+                "h2",
+                "h3",
+                "h4",
+                "h5",
+                "h6",
+            ]:
+                section_level = int(node.attributes["html_tag"][1])
                 while section_level <= section_stack[-1][0]:
                     section_stack.pop()
                 new_section = nodes.section(ids=[nodes.make_id(node.astext())])
                 title = nodes.title()
                 title.children = node.children
                 new_section.append(title)
                 section_stack[-1][1].append(new_section)
@@ -158,68 +182,82 @@
             elif isinstance(node, nodes.section):
                 pass
             else:
                 # Need to check that the
                 in_heading = False
                 tmp = node
                 while tmp.parent is not None and isinstance(tmp.parent, TeiElement):
-                    if tmp.parent.attributes['html_tag'] in ['h1', 'h2', 'h3', 'h4', 'h5', 'h6']:
+                    if tmp.parent.attributes["html_tag"] in [
+                        "h1",
+                        "h2",
+                        "h3",
+                        "h4",
+                        "h5",
+                        "h6",
+                    ]:
                         in_heading = True
                         break
                     tmp = tmp.parent
                 if not in_heading:
                     section_stack[-1][1].append(node)
 
-    def _rule_for_node(self: 'TEIParser', node: etree.Element, rules: list[dict]) -> dict:
+    def _rule_for_node(
+        self: "TEIParser", node: etree.Element, rules: list[dict]
+    ) -> dict:
         """Determine the first matching mapping rule for the node from the configured rules."""
         tei_tag = node.tag
         for rule in rules:
-            if rule['selector']['tag'] == tei_tag:
-                if 'attributes' in rule['selector']:
+            if rule["selector"]["tag"] == tei_tag:
+                if "attributes" in rule["selector"]:
                     attr_match = True
-                    for attr_rule in rule['selector']['attributes']:
-                        if attr_rule['attr'] not in node.attrib or \
-                                node.attrib[attr_rule['attr']] != attr_rule['value']:
+                    for attr_rule in rule["selector"]["attributes"]:
+                        if (
+                            attr_rule["attr"] not in node.attrib
+                            or node.attrib[attr_rule["attr"]] != attr_rule["value"]
+                        ):
                             attr_match = False
                             break
                     if not attr_match:
                         continue
                 return rule
         return None
 
-    def _parse_single_field(self: 'TEIParser', parent: etree.Element, field: dict, root: etree.Element) -> None:
-        content = root.xpath(field['content'], namespaces=namespaces)
+    def _parse_single_field(
+        self: "TEIParser", parent: etree.Element, field: dict, root: etree.Element
+    ) -> None:
+        content = root.xpath(field["content"], namespaces=namespaces)
         if len(content) > 0:
             content = content[0]
             li = nodes.definition_list_item()
             dt = nodes.term()
-            dt.append(nodes.Text(field['title']))
+            dt.append(nodes.Text(field["title"]))
             li.append(dt)
             dd = nodes.definition()
             dd.append(nodes.Text(content))
             li.append(dd)
             parent.append(li)
 
-    def _parse_list_field(self: 'TEIParser', parent: etree.Element, field: dict, root: etree.Element) -> None:
-        content = root.xpath(field['content'], namespaces=namespaces)
+    def _parse_list_field(
+        self: "TEIParser", parent: etree.Element, field: dict, root: etree.Element
+    ) -> None:
+        content = root.xpath(field["content"], namespaces=namespaces)
         if len(content) > 0:
             li = nodes.definition_list_item()
             dt = nodes.term()
-            dt.append(nodes.Text(field['title']))
+            dt.append(nodes.Text(field["title"]))
             li.append(dt)
             dd = nodes.definition()
             values = nodes.enumerated_list()
             for value in content:
                 item = nodes.list_item()
                 item.append(nodes.Text(value))
                 values.append(item)
             dd.append(values)
             li.append(dd)
             parent.append(li)
 
 
-
 def setup(app: Sphinx) -> None:
-    """Setup the TEI Sphinx extension."""
+    """Set up the TEI Sphinx extension."""
     app.add_node(TeiElement, html=(tei_element_html_enter, tei_element_html_exit))
-    app.add_source_suffix('.tei', 'tei')
+    app.add_source_suffix(".tei", "tei")
     app.add_source_parser(TEIParser)
```

### Comparing `uedition-0.3.1/LICENSE.txt` & `uedition-0.4.0/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `uedition-0.3.1/README.md` & `uedition-0.4.0/README.md`

 * *Files identical despite different names*

### Comparing `uedition-0.3.1/pyproject.toml` & `uedition-0.4.0/pyproject.toml`

 * *Files 12% similar despite different names*

```diff
@@ -37,14 +37,21 @@
 Documentation = "https://github.com/unknown/uedition#readme"
 Issues = "https://github.com/unknown/uedition/issues"
 Source = "https://github.com/unknown/uedition"
 
 [tool.hatch.version]
 path = "uedition/__about__.py"
 
+[tool.hatch.envs.dev]
+extra-dependencies = [
+  "black"
+]
+[tool.hatch.envs.dev.scripts]
+codestyle = "black ."
+
 [tool.hatch.envs.test]
 extra-dependencies = [
   "pytest",
   "pytest-cov",
 ]
 [tool.hatch.envs.test.scripts]
 cov = "pytest --cov-report=term-missing --cov-config=pyproject.toml --cov=uedition --cov=tests --cov-branch {args}"
```

### Comparing `uedition-0.3.1/PKG-INFO` & `uedition-0.4.0/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: uEdition
-Version: 0.3.1
+Version: 0.4.0
 Project-URL: Documentation, https://github.com/unknown/uedition#readme
 Project-URL: Issues, https://github.com/unknown/uedition/issues
 Project-URL: Source, https://github.com/unknown/uedition
 Author-email: Mark Hall <mark.hall@work.room3b.eu>
 License-Expression: MIT
 License-File: LICENSE.txt
 Classifier: Development Status :: 4 - Beta
```

