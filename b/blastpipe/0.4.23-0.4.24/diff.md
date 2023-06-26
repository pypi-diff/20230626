# Comparing `tmp/blastpipe-0.4.23.tar.gz` & `tmp/blastpipe-0.4.24.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "blastpipe-0.4.23.tar", last modified: Sun Jun 25 02:16:18 2023, max compression
+gzip compressed data, was "blastpipe-0.4.24.tar", last modified: Mon Jun 26 03:54:53 2023, max compression
```

## Comparing `blastpipe-0.4.23.tar` & `blastpipe-0.4.24.tar`

### file list

```diff
@@ -1,42 +1,42 @@
-drwxrwxr-x   0 ross      (1000) ross      (1000)        0 2023-06-25 02:16:18.607188 blastpipe-0.4.23/
--rw-rw-r--   0 ross      (1000) ross      (1000)     3723 2023-06-25 02:16:18.000000 blastpipe-0.4.23/.gitignore
--rw-rw-r--   0 ross      (1000) ross      (1000)       56 2023-06-25 02:16:18.000000 blastpipe-0.4.23/.markdownlint.json
--rw-rw-r--   0 ross      (1000) ross      (1000)    12099 2023-06-25 02:16:18.000000 blastpipe-0.4.23/CHANGELOG.md
--rw-rw-r--   0 ross      (1000) ross      (1000)    11358 2023-06-25 02:16:18.000000 blastpipe-0.4.23/LICENSE.txt
--rw-rw-r--   0 ross      (1000) ross      (1000)     4612 2023-06-25 02:16:18.000000 blastpipe-0.4.23/NOTICE.md
--rw-rw-r--   0 ross      (1000) ross      (1000)     5097 2023-06-25 02:16:18.000000 blastpipe-0.4.23/PKG-INFO
--rw-rw-r--   0 ross      (1000) ross      (1000)     4204 2023-06-25 02:16:18.000000 blastpipe-0.4.23/README.rst
-drwxrwxr-x   0 ross      (1000) ross      (1000)        0 2023-06-25 02:16:18.000000 blastpipe-0.4.23/blastpipe/
--rw-rw-r--   0 ross      (1000) ross      (1000)     1629 2023-06-25 02:16:18.000000 blastpipe-0.4.23/blastpipe/__init__.py
--rw-rw-r--   0 ross      (1000) ross      (1000)     3234 2023-06-25 02:16:18.000000 blastpipe-0.4.23/blastpipe/backports.py
--rw-rw-r--   0 ross      (1000) ross      (1000)     1811 2023-06-25 02:16:18.000000 blastpipe-0.4.23/blastpipe/buffer.py
--rw-rw-r--   0 ross      (1000) ross      (1000)     1666 2023-06-25 02:16:18.000000 blastpipe-0.4.23/blastpipe/loop.py
--rw-rw-r--   0 ross      (1000) ross      (1000)     2867 2023-06-25 02:16:18.000000 blastpipe-0.4.23/blastpipe/malloc.py
--rw-rw-r--   0 ross      (1000) ross      (1000)      971 2023-06-25 02:16:18.000000 blastpipe-0.4.23/blastpipe/meson.build
--rw-rw-r--   0 ross      (1000) ross      (1000)     1351 2023-06-25 02:16:18.000000 blastpipe-0.4.23/blastpipe/mixin.py
--rw-rw-r--   0 ross      (1000) ross      (1000)     1808 2023-06-25 02:16:18.000000 blastpipe-0.4.23/blastpipe/sequence.py
--rw-rw-r--   0 ross      (1000) ross      (1000)     1408 2023-06-25 02:16:18.000000 blastpipe-0.4.23/blastpipe/tailcall.py
--rw-rw-r--   0 ross      (1000) ross      (1000)     3043 2023-06-25 02:16:18.000000 blastpipe-0.4.23/meson.build
--rw-rw-r--   0 ross      (1000) ross      (1000)     5580 2023-06-25 02:16:18.000000 blastpipe-0.4.23/meson.options
--rw-rw-r--   0 ross      (1000) ross      (1000)    11474 2023-06-25 02:16:18.000000 blastpipe-0.4.23/pyproject.toml
-drwxrwxr-x   0 ross      (1000) ross      (1000)        0 2023-06-25 02:16:18.000000 blastpipe-0.4.23/subprojects/
--rw-rw-r--   0 ross      (1000) ross      (1000)      739 2023-06-25 02:16:18.000000 blastpipe-0.4.23/subprojects/dev.wrap
-drwxrwxr-x   0 ross      (1000) ross      (1000)        0 2023-06-25 02:16:18.000000 blastpipe-0.4.23/subprojects/docs/
--rw-rw-r--   0 ross      (1000) ross      (1000)    11358 2023-06-25 02:16:18.000000 blastpipe-0.4.23/subprojects/docs/LICENSE.txt
-drwxrwxr-x   0 ross      (1000) ross      (1000)        0 2023-06-25 02:16:18.000000 blastpipe-0.4.23/subprojects/docs/_static/
-drwxrwxr-x   0 ross      (1000) ross      (1000)        0 2023-06-25 02:16:18.000000 blastpipe-0.4.23/subprojects/docs/_static/css/
--rw-rw-r--   0 ross      (1000) ross      (1000)      767 2023-06-25 02:16:18.000000 blastpipe-0.4.23/subprojects/docs/_static/css/custom.css
--rw-rw-r--   0 ross      (1000) ross      (1000)      693 2023-06-25 02:16:18.000000 blastpipe-0.4.23/subprojects/docs/_static/css/meson.build
--rw-rw-r--   0 ross      (1000) ross      (1000)      633 2023-06-25 02:16:18.000000 blastpipe-0.4.23/subprojects/docs/_static/meson.build
-drwxrwxr-x   0 ross      (1000) ross      (1000)        0 2023-06-25 02:16:18.000000 blastpipe-0.4.23/subprojects/docs/_templates/
--rw-rw-r--   0 ross      (1000) ross      (1000)     1033 2023-06-25 02:16:18.000000 blastpipe-0.4.23/subprojects/docs/_templates/layout.html
--rw-rw-r--   0 ross      (1000) ross      (1000)      694 2023-06-25 02:16:18.000000 blastpipe-0.4.23/subprojects/docs/_templates/meson.build
--rw-rw-r--   0 ross      (1000) ross      (1000)      860 2023-06-25 02:16:18.000000 blastpipe-0.4.23/subprojects/docs/conf.cfg
--rw-rw-r--   0 ross      (1000) ross      (1000)     1751 2023-06-25 02:16:18.000000 blastpipe-0.4.23/subprojects/docs/index.rst
--rw-rw-r--   0 ross      (1000) ross      (1000)     2680 2023-06-25 02:16:18.000000 blastpipe-0.4.23/subprojects/docs/meson.build
--rw-rw-r--   0 ross      (1000) ross      (1000)     2058 2023-06-25 02:16:18.000000 blastpipe-0.4.23/subprojects/docs/meson.options
-drwxrwxr-x   0 ross      (1000) ross      (1000)        0 2023-06-25 02:16:18.000000 blastpipe-0.4.23/tests/
--rw-rw-r--   0 ross      (1000) ross      (1000)     2350 2023-06-25 02:16:18.000000 blastpipe-0.4.23/tests/meson.build
--rw-rw-r--   0 ross      (1000) ross      (1000)     1173 2023-06-25 02:16:18.000000 blastpipe-0.4.23/tests/test_backports.py
--rw-rw-r--   0 ross      (1000) ross      (1000)     2503 2023-06-25 02:16:18.000000 blastpipe-0.4.23/tests/test_fuzz.py
--rw-rw-r--   0 ross      (1000) ross      (1000)     1689 2023-06-25 02:16:18.000000 blastpipe-0.4.23/tests/test_tailcall.py
+drwxrwxr-x   0 ross      (1000) ross      (1000)        0 2023-06-26 03:54:53.533516 blastpipe-0.4.24/
+-rw-rw-r--   0 ross      (1000) ross      (1000)     3723 2023-06-26 03:54:53.000000 blastpipe-0.4.24/.gitignore
+-rw-rw-r--   0 ross      (1000) ross      (1000)       56 2023-06-26 03:54:53.000000 blastpipe-0.4.24/.markdownlint.json
+-rw-rw-r--   0 ross      (1000) ross      (1000)    12252 2023-06-26 03:54:53.000000 blastpipe-0.4.24/CHANGELOG.md
+-rw-rw-r--   0 ross      (1000) ross      (1000)    11358 2023-06-26 03:54:53.000000 blastpipe-0.4.24/LICENSE.txt
+-rw-rw-r--   0 ross      (1000) ross      (1000)     4612 2023-06-26 03:54:53.000000 blastpipe-0.4.24/NOTICE.md
+-rw-rw-r--   0 ross      (1000) ross      (1000)     5099 2023-06-26 03:54:53.000000 blastpipe-0.4.24/PKG-INFO
+-rw-rw-r--   0 ross      (1000) ross      (1000)     4206 2023-06-26 03:54:53.000000 blastpipe-0.4.24/README.rst
+drwxrwxr-x   0 ross      (1000) ross      (1000)        0 2023-06-26 03:54:53.000000 blastpipe-0.4.24/blastpipe/
+-rw-rw-r--   0 ross      (1000) ross      (1000)     1629 2023-06-26 03:54:53.000000 blastpipe-0.4.24/blastpipe/__init__.py
+-rw-rw-r--   0 ross      (1000) ross      (1000)     3234 2023-06-26 03:54:53.000000 blastpipe-0.4.24/blastpipe/backports.py
+-rw-rw-r--   0 ross      (1000) ross      (1000)     1811 2023-06-26 03:54:53.000000 blastpipe-0.4.24/blastpipe/buffer.py
+-rw-rw-r--   0 ross      (1000) ross      (1000)     1666 2023-06-26 03:54:53.000000 blastpipe-0.4.24/blastpipe/loop.py
+-rw-rw-r--   0 ross      (1000) ross      (1000)     2867 2023-06-26 03:54:53.000000 blastpipe-0.4.24/blastpipe/malloc.py
+-rw-rw-r--   0 ross      (1000) ross      (1000)      971 2023-06-26 03:54:53.000000 blastpipe-0.4.24/blastpipe/meson.build
+-rw-rw-r--   0 ross      (1000) ross      (1000)     1351 2023-06-26 03:54:53.000000 blastpipe-0.4.24/blastpipe/mixin.py
+-rw-rw-r--   0 ross      (1000) ross      (1000)     1808 2023-06-26 03:54:53.000000 blastpipe-0.4.24/blastpipe/sequence.py
+-rw-rw-r--   0 ross      (1000) ross      (1000)     1408 2023-06-26 03:54:53.000000 blastpipe-0.4.24/blastpipe/tailcall.py
+-rw-rw-r--   0 ross      (1000) ross      (1000)     3043 2023-06-26 03:54:53.000000 blastpipe-0.4.24/meson.build
+-rw-rw-r--   0 ross      (1000) ross      (1000)     5580 2023-06-26 03:54:53.000000 blastpipe-0.4.24/meson.options
+-rw-rw-r--   0 ross      (1000) ross      (1000)    11676 2023-06-26 03:54:53.000000 blastpipe-0.4.24/pyproject.toml
+drwxrwxr-x   0 ross      (1000) ross      (1000)        0 2023-06-26 03:54:53.000000 blastpipe-0.4.24/subprojects/
+-rw-rw-r--   0 ross      (1000) ross      (1000)      739 2023-06-26 03:54:53.000000 blastpipe-0.4.24/subprojects/dev.wrap
+drwxrwxr-x   0 ross      (1000) ross      (1000)        0 2023-06-26 03:54:53.000000 blastpipe-0.4.24/subprojects/docs/
+-rw-rw-r--   0 ross      (1000) ross      (1000)    11358 2023-06-26 03:54:53.000000 blastpipe-0.4.24/subprojects/docs/LICENSE.txt
+drwxrwxr-x   0 ross      (1000) ross      (1000)        0 2023-06-26 03:54:53.000000 blastpipe-0.4.24/subprojects/docs/_static/
+drwxrwxr-x   0 ross      (1000) ross      (1000)        0 2023-06-26 03:54:53.000000 blastpipe-0.4.24/subprojects/docs/_static/css/
+-rw-rw-r--   0 ross      (1000) ross      (1000)      767 2023-06-26 03:54:53.000000 blastpipe-0.4.24/subprojects/docs/_static/css/custom.css
+-rw-rw-r--   0 ross      (1000) ross      (1000)      693 2023-06-26 03:54:53.000000 blastpipe-0.4.24/subprojects/docs/_static/css/meson.build
+-rw-rw-r--   0 ross      (1000) ross      (1000)      633 2023-06-26 03:54:53.000000 blastpipe-0.4.24/subprojects/docs/_static/meson.build
+drwxrwxr-x   0 ross      (1000) ross      (1000)        0 2023-06-26 03:54:53.000000 blastpipe-0.4.24/subprojects/docs/_templates/
+-rw-rw-r--   0 ross      (1000) ross      (1000)     1033 2023-06-26 03:54:53.000000 blastpipe-0.4.24/subprojects/docs/_templates/layout.html
+-rw-rw-r--   0 ross      (1000) ross      (1000)      694 2023-06-26 03:54:53.000000 blastpipe-0.4.24/subprojects/docs/_templates/meson.build
+-rw-rw-r--   0 ross      (1000) ross      (1000)      860 2023-06-26 03:54:53.000000 blastpipe-0.4.24/subprojects/docs/conf.cfg
+-rw-rw-r--   0 ross      (1000) ross      (1000)     1751 2023-06-26 03:54:53.000000 blastpipe-0.4.24/subprojects/docs/index.rst
+-rw-rw-r--   0 ross      (1000) ross      (1000)     2680 2023-06-26 03:54:53.000000 blastpipe-0.4.24/subprojects/docs/meson.build
+-rw-rw-r--   0 ross      (1000) ross      (1000)     2058 2023-06-26 03:54:53.000000 blastpipe-0.4.24/subprojects/docs/meson.options
+drwxrwxr-x   0 ross      (1000) ross      (1000)        0 2023-06-26 03:54:53.000000 blastpipe-0.4.24/tests/
+-rw-rw-r--   0 ross      (1000) ross      (1000)     2350 2023-06-26 03:54:53.000000 blastpipe-0.4.24/tests/meson.build
+-rw-rw-r--   0 ross      (1000) ross      (1000)     1173 2023-06-26 03:54:53.000000 blastpipe-0.4.24/tests/test_backports.py
+-rw-rw-r--   0 ross      (1000) ross      (1000)     2503 2023-06-26 03:54:53.000000 blastpipe-0.4.24/tests/test_fuzz.py
+-rw-rw-r--   0 ross      (1000) ross      (1000)     1689 2023-06-26 03:54:53.000000 blastpipe-0.4.24/tests/test_tailcall.py
```

### Comparing `blastpipe-0.4.23/.gitignore` & `blastpipe-0.4.24/.gitignore`

 * *Files identical despite different names*

### Comparing `blastpipe-0.4.23/CHANGELOG.md` & `blastpipe-0.4.24/CHANGELOG.md`

 * *Files 1% similar despite different names*

```diff
@@ -13,14 +13,18 @@
    specific language governing permissions and limitations
    under the License. -->
 
 # Changelog
 
 <!--next-version-placeholder-->
 
+## v0.4.23 (2023-06-24)
+### Other
+* PKG-INFO Updated ([`f80b3da`](https://github.com/rjdbcm/blastpipe/commit/f80b3da157f4a083922832e621b949a477238972))
+
 ## v0.4.21 (2023-06-23)
 ### Other
 * PKG-INFO Updated ([`5c84048`](https://github.com/rjdbcm/blastpipe/commit/5c840485844fabc70b91c5be67d7b60ab4b864b0))
 
 ## v0.4.6 (2023-06-21)
```

### Comparing `blastpipe-0.4.23/LICENSE.txt` & `blastpipe-0.4.24/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `blastpipe-0.4.23/NOTICE.md` & `blastpipe-0.4.24/NOTICE.md`

 * *Files identical despite different names*

### Comparing `blastpipe-0.4.23/PKG-INFO` & `blastpipe-0.4.24/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: blastpipe
-Version: 0.4.23
+Version: 0.4.24
 Summary: Packaged with OZI.
 Classifier: Development Status :: 2 - Pre-Alpha
 Classifier: Natural Language :: English
 Classifier: Intended Audience :: Developers
 Classifier: Operating System :: MacOS :: MacOS X
 Classifier: Operating System :: Microsoft :: Windows
 Classifier: Operating System :: POSIX :: Linux
@@ -50,15 +50,15 @@
  :target: https://www.sigstore.dev/
 
 License
 ^^^^^^^
 
 blastpipe is released under the terms of the 2.0 version of the Apache License,
 approved by the Apache Software Foundation. blastpipe meets the Open Source Initiative's definition of
-open source software, and the Free Software Foundation's definition of GPL-compatible open 
+open source software, and the Free Software Foundation's definition of GPLv3-compatible open 
 source software.
 
 |osi-logo| |asf-logo| |fsf-logo|
 
 .. note::
    The OSI logo trademark is the trademark of Open Source Initiative.
    The blastpipe project is not affiliated with or endorsed by the Open Source Initiative.
```

### Comparing `blastpipe-0.4.23/README.rst` & `blastpipe-0.4.24/README.rst`

 * *Files 1% similar despite different names*

```diff
@@ -30,15 +30,15 @@
  :target: https://www.sigstore.dev/
 
 License
 ^^^^^^^
 
 blastpipe is released under the terms of the 2.0 version of the Apache License,
 approved by the Apache Software Foundation. blastpipe meets the Open Source Initiative's definition of
-open source software, and the Free Software Foundation's definition of GPL-compatible open 
+open source software, and the Free Software Foundation's definition of GPLv3-compatible open 
 source software.
 
 |osi-logo| |asf-logo| |fsf-logo|
 
 .. note::
    The OSI logo trademark is the trademark of Open Source Initiative.
    The blastpipe project is not affiliated with or endorsed by the Open Source Initiative.
```

### Comparing `blastpipe-0.4.23/blastpipe/__init__.py` & `blastpipe-0.4.24/blastpipe/__init__.py`

 * *Files identical despite different names*

### Comparing `blastpipe-0.4.23/blastpipe/backports.py` & `blastpipe-0.4.24/blastpipe/backports.py`

 * *Files identical despite different names*

### Comparing `blastpipe-0.4.23/blastpipe/buffer.py` & `blastpipe-0.4.24/blastpipe/buffer.py`

 * *Files identical despite different names*

### Comparing `blastpipe-0.4.23/blastpipe/loop.py` & `blastpipe-0.4.24/blastpipe/loop.py`

 * *Files identical despite different names*

### Comparing `blastpipe-0.4.23/blastpipe/malloc.py` & `blastpipe-0.4.24/blastpipe/malloc.py`

 * *Files identical despite different names*

### Comparing `blastpipe-0.4.23/blastpipe/meson.build` & `blastpipe-0.4.24/blastpipe/meson.build`

 * *Files identical despite different names*

### Comparing `blastpipe-0.4.23/blastpipe/mixin.py` & `blastpipe-0.4.24/blastpipe/mixin.py`

 * *Files identical despite different names*

### Comparing `blastpipe-0.4.23/blastpipe/sequence.py` & `blastpipe-0.4.24/blastpipe/sequence.py`

 * *Files identical despite different names*

### Comparing `blastpipe-0.4.23/blastpipe/tailcall.py` & `blastpipe-0.4.24/blastpipe/tailcall.py`

 * *Files identical despite different names*

### Comparing `blastpipe-0.4.23/meson.build` & `blastpipe-0.4.24/meson.build`

 * *Files identical despite different names*

### Comparing `blastpipe-0.4.23/meson.options` & `blastpipe-0.4.24/meson.options`

 * *Files identical despite different names*

### Comparing `blastpipe-0.4.23/pyproject.toml` & `blastpipe-0.4.24/pyproject.toml`

 * *Files 3% similar despite different names*

```diff
@@ -14,15 +14,15 @@
 # under the License.
 [project]
 authors = [{name = "Ross J. Duff MSc", email = "rjdbcm@github.com"}]
 dynamic = ["version"]
 license = {file = "LICENSE.txt"}
 readme  = "README.rst"
 
-[project.optional_dependencies] # also meson test suite names
+[project.optional_dependencies] # also OZI meson test suite names
 # Default OZI test setup
 dev  = ["[dist,docs,lint,test]"]
 ## Packaging Setup
 dist = ["pyc_wheel", "python-semantic-release", "sigstore"]
 ## Documentation Setup
 docs = ["doc8", "pydocstyle[toml]", "Pygments", "pyparsing", "sphinx",
         "sphinx-design", "sphinxawesome-codelinter", "sphinxawesome-theme ~= 5.0.0b2"]
@@ -30,22 +30,24 @@
 lint = ["bandit[toml]", "black", "flake8", "Flake8-pyproject", "isort", "pylint", "pyright",
         "restructuredtext-lint"]
 ## Testing Setup
 test = ["coverage[toml]", "hypothesis[all]", "pytest", "pytest-asyncio", "pytest-cov", 
         "pytest-tcpclient", "pytest-randomly", "pytest-xdist"]
 
 [tool.mesonpep517.metadata]
+# We let setuptools_scm write version metadata to a PKG-INFO template
 summary         = "Packaged with OZI."
 pkg-info-file   = "PKG-INFO"
 
 [build-system]
 requires      = ["mesonpep517","ninja","setuptools>=64","setuptools_scm[toml]>=6.2","tomli"]
 build-backend = "mesonpep517.buildapi"
 
 [tool.bandit]
+# We allow bandit to also scan meson build directory but not virtual environments
 exclude_dirs = ["venv", "build-env-*"]
 verbose = true
 format = "txt"
 
 [tool.black]
 line-length = 93
 
@@ -138,14 +140,15 @@
 #                         build/meson-dist/*.sig,\
 #                         build/meson-dist/*.crt,\
 #                         build/meson-dist/*.sigstore"""
 major_on_zero            = false
 patch_without_tag        = false
 prerelease_tag           = "beta"
 pre_commit_command       = """
+                        git clean -dfX && \
                         meson setup build-dist-checkpoint --reconfigure -Ddev=enabled && \
                         meson test -C build-dist-checkpoint --setup=test --setup=lint && \
                         git stash -- PKG-INFO && \
                         git stash drop"""
 remove_dist              = false
 repository               = "pypi"
 tag_format               = "{version}"
@@ -208,15 +211,15 @@
  :target: https://www.sigstore.dev/
 
 License
 ^^^^^^^
 
 blastpipe is released under the terms of the 2.0 version of the Apache License,
 approved by the Apache Software Foundation. blastpipe meets the Open Source Initiative's definition of
-open source software, and the Free Software Foundation's definition of GPL-compatible open 
+open source software, and the Free Software Foundation's definition of GPLv3-compatible open 
 source software.
 
 |osi-logo| |asf-logo| |fsf-logo|
 
 .. note::
    The OSI logo trademark is the trademark of Open Source Initiative.
    The blastpipe project is not affiliated with or endorsed by the Open Source Initiative.
```

### Comparing `blastpipe-0.4.23/subprojects/dev.wrap` & `blastpipe-0.4.24/subprojects/dev.wrap`

 * *Files identical despite different names*

### Comparing `blastpipe-0.4.23/subprojects/docs/LICENSE.txt` & `blastpipe-0.4.24/subprojects/docs/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `blastpipe-0.4.23/subprojects/docs/_static/css/custom.css` & `blastpipe-0.4.24/subprojects/docs/_static/css/custom.css`

 * *Files identical despite different names*

### Comparing `blastpipe-0.4.23/subprojects/docs/_static/css/meson.build` & `blastpipe-0.4.24/subprojects/docs/_static/css/meson.build`

 * *Files identical despite different names*

### Comparing `blastpipe-0.4.23/subprojects/docs/_static/meson.build` & `blastpipe-0.4.24/subprojects/docs/_static/meson.build`

 * *Files identical despite different names*

### Comparing `blastpipe-0.4.23/subprojects/docs/_templates/layout.html` & `blastpipe-0.4.24/subprojects/docs/_templates/layout.html`

 * *Files identical despite different names*

### Comparing `blastpipe-0.4.23/subprojects/docs/_templates/meson.build` & `blastpipe-0.4.24/subprojects/docs/_templates/meson.build`

 * *Files identical despite different names*

### Comparing `blastpipe-0.4.23/subprojects/docs/conf.cfg` & `blastpipe-0.4.24/subprojects/docs/conf.cfg`

 * *Files identical despite different names*

### Comparing `blastpipe-0.4.23/subprojects/docs/index.rst` & `blastpipe-0.4.24/subprojects/docs/index.rst`

 * *Files identical despite different names*

### Comparing `blastpipe-0.4.23/subprojects/docs/meson.build` & `blastpipe-0.4.24/subprojects/docs/meson.build`

 * *Files identical despite different names*

### Comparing `blastpipe-0.4.23/subprojects/docs/meson.options` & `blastpipe-0.4.24/subprojects/docs/meson.options`

 * *Files identical despite different names*

### Comparing `blastpipe-0.4.23/tests/meson.build` & `blastpipe-0.4.24/tests/meson.build`

 * *Files identical despite different names*

### Comparing `blastpipe-0.4.23/tests/test_backports.py` & `blastpipe-0.4.24/tests/test_backports.py`

 * *Files identical despite different names*

### Comparing `blastpipe-0.4.23/tests/test_fuzz.py` & `blastpipe-0.4.24/tests/test_fuzz.py`

 * *Files identical despite different names*

### Comparing `blastpipe-0.4.23/tests/test_tailcall.py` & `blastpipe-0.4.24/tests/test_tailcall.py`

 * *Files identical despite different names*

