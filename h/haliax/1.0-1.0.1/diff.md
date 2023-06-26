# Comparing `tmp/haliax-1.0.tar.gz` & `tmp/haliax-1.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, last modified: Sun Feb  2 00:00:00 2020, max compression
+gzip compressed data, was "haliax-1.0.1.tar", last modified: Mon Jun 26 19:23:59 2023, max compression
```

## Comparing `haliax-1.0.tar` & `haliax-1.0.1.tar`

### file list

```diff
@@ -1,39 +1,42 @@
--rw-r--r--   0        0        0      157 2020-02-02 00:00:00.000000 haliax-1.0/.flake8
--rw-r--r--   0        0        0      893 2020-02-02 00:00:00.000000 haliax-1.0/.pre-commit-config.yaml
--rw-r--r--   0        0        0     4191 2020-02-02 00:00:00.000000 haliax-1.0/CONTRIBUTING.md
--rw-r--r--   0        0        0     1450 2020-02-02 00:00:00.000000 haliax-1.0/mkdocs.yml
--rw-r--r--   0        0        0     1090 2020-02-02 00:00:00.000000 haliax-1.0/.github/workflows/run_tests.yaml
--rw-r--r--   0        0        0      325 2020-02-02 00:00:00.000000 haliax-1.0/docs/index.md
--rw-r--r--   0        0        0     4090 2020-02-02 00:00:00.000000 haliax-1.0/docs/indexing.md
--rw-r--r--   0        0        0    12092 2020-02-02 00:00:00.000000 haliax-1.0/haliax/__init__.py
--rw-r--r--   0        0        0    46624 2020-02-02 00:00:00.000000 haliax-1.0/haliax/core.py
--rw-r--r--   0        0        0    15410 2020-02-02 00:00:00.000000 haliax-1.0/haliax/hof.py
--rw-r--r--   0        0        0     4678 2020-02-02 00:00:00.000000 haliax-1.0/haliax/jax_utils.py
--rw-r--r--   0        0        0     4398 2020-02-02 00:00:00.000000 haliax-1.0/haliax/ops.py
--rw-r--r--   0        0        0    16809 2020-02-02 00:00:00.000000 haliax-1.0/haliax/partitioning.py
--rw-r--r--   0        0        0    12653 2020-02-02 00:00:00.000000 haliax-1.0/haliax/random.py
--rw-r--r--   0        0        0     1738 2020-02-02 00:00:00.000000 haliax-1.0/haliax/tree_util.py
--rw-r--r--   0        0        0     1082 2020-02-02 00:00:00.000000 haliax-1.0/haliax/types.py
--rw-r--r--   0        0        0     1689 2020-02-02 00:00:00.000000 haliax-1.0/haliax/util.py
--rw-r--r--   0        0        0     5273 2020-02-02 00:00:00.000000 haliax-1.0/haliax/wrap.py
--rw-r--r--   0        0        0     4398 2020-02-02 00:00:00.000000 haliax-1.0/haliax/nn/__init__.py
--rw-r--r--   0        0        0     8383 2020-02-02 00:00:00.000000 haliax-1.0/haliax/nn/attention.py
--rw-r--r--   0        0        0     3316 2020-02-02 00:00:00.000000 haliax-1.0/haliax/nn/dropout.py
--rw-r--r--   0        0        0      869 2020-02-02 00:00:00.000000 haliax-1.0/haliax/nn/embedding.py
--rw-r--r--   0        0        0     1022 2020-02-02 00:00:00.000000 haliax-1.0/haliax/nn/linear.py
--rw-r--r--   0        0        0     1166 2020-02-02 00:00:00.000000 haliax-1.0/haliax/nn/normalization.py
--rw-r--r--   0        0        0     3972 2020-02-02 00:00:00.000000 haliax-1.0/haliax/nn/scan.py
--rw-r--r--   0        0        0    21465 2020-02-02 00:00:00.000000 haliax-1.0/tests/core_test.py
--rw-r--r--   0        0        0     2290 2020-02-02 00:00:00.000000 haliax-1.0/tests/test_attention.py
--rw-r--r--   0        0        0     6575 2020-02-02 00:00:00.000000 haliax-1.0/tests/test_hof.py
--rw-r--r--   0        0        0     3614 2020-02-02 00:00:00.000000 haliax-1.0/tests/test_nn.py
--rw-r--r--   0        0        0     6523 2020-02-02 00:00:00.000000 haliax-1.0/tests/test_ops.py
--rw-r--r--   0        0        0     7300 2020-02-02 00:00:00.000000 haliax-1.0/tests/test_partitioning.py
--rw-r--r--   0        0        0    11235 2020-02-02 00:00:00.000000 haliax-1.0/tests/test_random.py
--rw-r--r--   0        0        0      926 2020-02-02 00:00:00.000000 haliax-1.0/tests/test_tree_util.py
--rw-r--r--   0        0        0     3480 2020-02-02 00:00:00.000000 haliax-1.0/tests/test_utils.py
--rw-r--r--   0        0        0     1958 2020-02-02 00:00:00.000000 haliax-1.0/.gitignore
--rw-r--r--   0        0        0    11349 2020-02-02 00:00:00.000000 haliax-1.0/LICENSE
--rw-r--r--   0        0        0     4182 2020-02-02 00:00:00.000000 haliax-1.0/README.md
--rw-r--r--   0        0        0     1771 2020-02-02 00:00:00.000000 haliax-1.0/pyproject.toml
--rw-r--r--   0        0        0     5528 2020-02-02 00:00:00.000000 haliax-1.0/PKG-INFO
+drwxr-xr-x   0 dlwh       (501) staff       (20)        0 2023-06-26 19:23:59.235540 haliax-1.0.1/
+-rw-r--r--   0 dlwh       (501) staff       (20)    11349 2023-06-26 17:49:29.000000 haliax-1.0.1/LICENSE
+-rw-r--r--   0 dlwh       (501) staff       (20)     4880 2023-06-26 19:23:59.235391 haliax-1.0.1/PKG-INFO
+-rw-r--r--   0 dlwh       (501) staff       (20)     4182 2023-06-26 18:58:48.000000 haliax-1.0.1/README.md
+-rw-r--r--   0 dlwh       (501) staff       (20)     1405 2023-06-26 19:23:42.000000 haliax-1.0.1/pyproject.toml
+-rw-r--r--   0 dlwh       (501) staff       (20)       38 2023-06-26 19:23:59.235592 haliax-1.0.1/setup.cfg
+drwxr-xr-x   0 dlwh       (501) staff       (20)        0 2023-06-26 19:23:59.229393 haliax-1.0.1/src/
+drwxr-xr-x   0 dlwh       (501) staff       (20)        0 2023-06-26 19:23:59.231920 haliax-1.0.1/src/haliax/
+-rw-r--r--   0 dlwh       (501) staff       (20)    12092 2023-06-26 17:49:29.000000 haliax-1.0.1/src/haliax/__init__.py
+-rw-r--r--   0 dlwh       (501) staff       (20)    46624 2023-06-26 17:49:29.000000 haliax-1.0.1/src/haliax/core.py
+-rw-r--r--   0 dlwh       (501) staff       (20)    15410 2023-06-26 17:49:29.000000 haliax-1.0.1/src/haliax/hof.py
+-rw-r--r--   0 dlwh       (501) staff       (20)     4678 2023-06-26 17:49:29.000000 haliax-1.0.1/src/haliax/jax_utils.py
+drwxr-xr-x   0 dlwh       (501) staff       (20)        0 2023-06-26 19:23:59.233731 haliax-1.0.1/src/haliax/nn/
+-rw-r--r--   0 dlwh       (501) staff       (20)     4398 2023-06-26 17:49:29.000000 haliax-1.0.1/src/haliax/nn/__init__.py
+-rw-r--r--   0 dlwh       (501) staff       (20)     8383 2023-06-26 17:49:29.000000 haliax-1.0.1/src/haliax/nn/attention.py
+-rw-r--r--   0 dlwh       (501) staff       (20)     3316 2023-06-26 17:49:29.000000 haliax-1.0.1/src/haliax/nn/dropout.py
+-rw-r--r--   0 dlwh       (501) staff       (20)      869 2023-06-26 17:49:29.000000 haliax-1.0.1/src/haliax/nn/embedding.py
+-rw-r--r--   0 dlwh       (501) staff       (20)     1022 2023-06-26 17:49:29.000000 haliax-1.0.1/src/haliax/nn/linear.py
+-rw-r--r--   0 dlwh       (501) staff       (20)     1166 2023-06-26 17:49:29.000000 haliax-1.0.1/src/haliax/nn/normalization.py
+-rw-r--r--   0 dlwh       (501) staff       (20)     3972 2023-06-26 17:49:29.000000 haliax-1.0.1/src/haliax/nn/scan.py
+-rw-r--r--   0 dlwh       (501) staff       (20)     4398 2023-06-26 17:49:29.000000 haliax-1.0.1/src/haliax/ops.py
+-rw-r--r--   0 dlwh       (501) staff       (20)    16809 2023-06-26 17:49:29.000000 haliax-1.0.1/src/haliax/partitioning.py
+-rw-r--r--   0 dlwh       (501) staff       (20)    12653 2023-06-26 17:49:29.000000 haliax-1.0.1/src/haliax/random.py
+-rw-r--r--   0 dlwh       (501) staff       (20)     1738 2023-06-26 17:49:29.000000 haliax-1.0.1/src/haliax/tree_util.py
+-rw-r--r--   0 dlwh       (501) staff       (20)     1082 2023-06-26 17:49:29.000000 haliax-1.0.1/src/haliax/types.py
+-rw-r--r--   0 dlwh       (501) staff       (20)     1689 2023-06-26 17:49:29.000000 haliax-1.0.1/src/haliax/util.py
+-rw-r--r--   0 dlwh       (501) staff       (20)     5273 2023-06-26 17:49:29.000000 haliax-1.0.1/src/haliax/wrap.py
+drwxr-xr-x   0 dlwh       (501) staff       (20)        0 2023-06-26 19:23:59.232691 haliax-1.0.1/src/haliax.egg-info/
+-rw-r--r--   0 dlwh       (501) staff       (20)     4880 2023-06-26 19:23:59.000000 haliax-1.0.1/src/haliax.egg-info/PKG-INFO
+-rw-r--r--   0 dlwh       (501) staff       (20)      784 2023-06-26 19:23:59.000000 haliax-1.0.1/src/haliax.egg-info/SOURCES.txt
+-rw-r--r--   0 dlwh       (501) staff       (20)        1 2023-06-26 19:23:59.000000 haliax-1.0.1/src/haliax.egg-info/dependency_links.txt
+-rw-r--r--   0 dlwh       (501) staff       (20)      271 2023-06-26 19:23:59.000000 haliax-1.0.1/src/haliax.egg-info/requires.txt
+-rw-r--r--   0 dlwh       (501) staff       (20)        7 2023-06-26 19:23:59.000000 haliax-1.0.1/src/haliax.egg-info/top_level.txt
+drwxr-xr-x   0 dlwh       (501) staff       (20)        0 2023-06-26 19:23:59.235193 haliax-1.0.1/tests/
+-rw-r--r--   0 dlwh       (501) staff       (20)     2290 2023-06-26 17:49:35.000000 haliax-1.0.1/tests/test_attention.py
+-rw-r--r--   0 dlwh       (501) staff       (20)     6575 2023-06-26 17:49:35.000000 haliax-1.0.1/tests/test_hof.py
+-rw-r--r--   0 dlwh       (501) staff       (20)     3614 2023-06-26 17:49:35.000000 haliax-1.0.1/tests/test_nn.py
+-rw-r--r--   0 dlwh       (501) staff       (20)     6523 2023-06-26 17:49:35.000000 haliax-1.0.1/tests/test_ops.py
+-rw-r--r--   0 dlwh       (501) staff       (20)     7300 2023-06-26 17:49:35.000000 haliax-1.0.1/tests/test_partitioning.py
+-rw-r--r--   0 dlwh       (501) staff       (20)    11235 2023-06-26 17:49:35.000000 haliax-1.0.1/tests/test_random.py
+-rw-r--r--   0 dlwh       (501) staff       (20)      926 2023-06-26 17:49:35.000000 haliax-1.0.1/tests/test_tree_util.py
+-rw-r--r--   0 dlwh       (501) staff       (20)     3480 2023-06-26 18:00:17.000000 haliax-1.0.1/tests/test_utils.py
```

### Comparing `haliax-1.0/haliax/__init__.py` & `haliax-1.0.1/src/haliax/__init__.py`

 * *Files identical despite different names*

### Comparing `haliax-1.0/haliax/core.py` & `haliax-1.0.1/src/haliax/core.py`

 * *Files identical despite different names*

### Comparing `haliax-1.0/haliax/hof.py` & `haliax-1.0.1/src/haliax/hof.py`

 * *Files identical despite different names*

### Comparing `haliax-1.0/haliax/jax_utils.py` & `haliax-1.0.1/src/haliax/jax_utils.py`

 * *Files identical despite different names*

### Comparing `haliax-1.0/haliax/ops.py` & `haliax-1.0.1/src/haliax/ops.py`

 * *Files identical despite different names*

### Comparing `haliax-1.0/haliax/partitioning.py` & `haliax-1.0.1/src/haliax/partitioning.py`

 * *Files identical despite different names*

### Comparing `haliax-1.0/haliax/random.py` & `haliax-1.0.1/src/haliax/random.py`

 * *Files identical despite different names*

### Comparing `haliax-1.0/haliax/tree_util.py` & `haliax-1.0.1/src/haliax/tree_util.py`

 * *Files identical despite different names*

### Comparing `haliax-1.0/haliax/types.py` & `haliax-1.0.1/src/haliax/types.py`

 * *Files identical despite different names*

### Comparing `haliax-1.0/haliax/util.py` & `haliax-1.0.1/src/haliax/util.py`

 * *Files identical despite different names*

### Comparing `haliax-1.0/haliax/wrap.py` & `haliax-1.0.1/src/haliax/wrap.py`

 * *Files identical despite different names*

### Comparing `haliax-1.0/haliax/nn/__init__.py` & `haliax-1.0.1/src/haliax/nn/__init__.py`

 * *Files identical despite different names*

### Comparing `haliax-1.0/haliax/nn/attention.py` & `haliax-1.0.1/src/haliax/nn/attention.py`

 * *Files identical despite different names*

### Comparing `haliax-1.0/haliax/nn/dropout.py` & `haliax-1.0.1/src/haliax/nn/dropout.py`

 * *Files identical despite different names*

### Comparing `haliax-1.0/haliax/nn/embedding.py` & `haliax-1.0.1/src/haliax/nn/embedding.py`

 * *Files identical despite different names*

### Comparing `haliax-1.0/haliax/nn/linear.py` & `haliax-1.0.1/src/haliax/nn/linear.py`

 * *Files identical despite different names*

### Comparing `haliax-1.0/haliax/nn/normalization.py` & `haliax-1.0.1/src/haliax/nn/normalization.py`

 * *Files identical despite different names*

### Comparing `haliax-1.0/haliax/nn/scan.py` & `haliax-1.0.1/src/haliax/nn/scan.py`

 * *Files identical despite different names*

### Comparing `haliax-1.0/tests/test_attention.py` & `haliax-1.0.1/tests/test_attention.py`

 * *Files identical despite different names*

### Comparing `haliax-1.0/tests/test_hof.py` & `haliax-1.0.1/tests/test_hof.py`

 * *Files identical despite different names*

### Comparing `haliax-1.0/tests/test_nn.py` & `haliax-1.0.1/tests/test_nn.py`

 * *Files identical despite different names*

### Comparing `haliax-1.0/tests/test_ops.py` & `haliax-1.0.1/tests/test_ops.py`

 * *Files identical despite different names*

### Comparing `haliax-1.0/tests/test_partitioning.py` & `haliax-1.0.1/tests/test_partitioning.py`

 * *Files identical despite different names*

### Comparing `haliax-1.0/tests/test_random.py` & `haliax-1.0.1/tests/test_random.py`

 * *Files identical despite different names*

### Comparing `haliax-1.0/tests/test_tree_util.py` & `haliax-1.0.1/tests/test_tree_util.py`

 * *Files identical despite different names*

### Comparing `haliax-1.0/tests/test_utils.py` & `haliax-1.0.1/tests/test_utils.py`

 * *Files identical despite different names*

### Comparing `haliax-1.0/LICENSE` & `haliax-1.0.1/LICENSE`

 * *Files identical despite different names*

### Comparing `haliax-1.0/README.md` & `haliax-1.0.1/README.md`

 * *Files identical despite different names*

### Comparing `haliax-1.0/pyproject.toml` & `haliax-1.0.1/pyproject.toml`

 * *Files 24% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
-requires = ["hatchling"]
-build-backend = "hatchling.build"
+requires = ["setuptools>=58.0.4", "wheel"]
+build-backend = "setuptools.build_meta"
 
 [project]
 name = "haliax"
-version = "1.0"
+version = "1.0.1"
 authors = [
   { name="David Hall", email="dlwh@cs.stanford.edu" },
 ]
 description = "Named Tensors for Legible Deep Learning in JAX"
 readme = "README.md"
 requires-python = ">=3.10"
 classifiers = [
@@ -32,40 +32,17 @@
     "mkdocs-literate-nav >= 0.6.0", "mkdocs-macros-plugin >= 0.7.0", "mkdocstrings-python >= 1.1.2",
     "mkdocs-include-markdown-plugin",
     "pymdown-extensions",
     "pygments",
     "pymdown-extensions",
 ]
 
+[options]
+packages = ["haliax", "haliax.*"]
 
-[tool.hatch.build.sources]
-"src/haliax" = "haliax"
+[options.package_data]
+haliax = ["src/haliax/*"]
 
 
-[tool.hatch.build.targets.wheel]
-packages = ["src/haliax"]
-
 [project.urls]
 "Homepage" = "https://github.com/stanford-crfm/haliax"
 "Bug Tracker" = "https://github.com/stanford-crfm/haliax/issues/"
-
-
-[tool.black]
-line-length = 119
-target-version = ["py310"]
-preview = true
-
-[tool.isort]
-profile = "black"
-multi_line_output = 3
-lines_after_imports = 2
-include_trailing_comma = true
-force_grid_wrap = 0
-use_parentheses = true
-ensure_newline_before_comments = true
-line_length = 119
-
-[tool.mypy]
-python_version = "3.10"
-
-[tool.mypy-haliax.core]
-ignore_missing_imports = true
```

