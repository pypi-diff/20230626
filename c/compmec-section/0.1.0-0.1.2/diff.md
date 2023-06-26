# Comparing `tmp/compmec_section-0.1.0.tar.gz` & `tmp/compmec_section-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "compmec_section-0.1.0.tar", max compression
+gzip compressed data, was "compmec_section-0.1.2.tar", max compression
```

## Comparing `compmec_section-0.1.0.tar` & `compmec_section-0.1.2.tar`

### file list

```diff
@@ -1,5 +1,8 @@
--rw-r--r--   0        0        0     1079 2023-06-26 09:35:56.600163 compmec_section-0.1.0/LICENSE.md
--rw-r--r--   0        0        0      517 2023-06-26 10:26:47.944235 compmec_section-0.1.0/pyproject.toml
--rw-r--r--   0        0        0        0 2023-06-26 09:29:15.430541 compmec_section-0.1.0/README.md
--rw-r--r--   0        0        0        0 2023-06-26 09:29:15.430541 compmec_section-0.1.0/src/compmec/section/__init__.py
--rw-r--r--   0        0        0      352 1970-01-01 00:00:00.000000 compmec_section-0.1.0/PKG-INFO
+-rw-r--r--   0        0        0     1079 2023-06-26 09:35:56.600163 compmec_section-0.1.2/LICENSE.md
+-rw-r--r--   0        0        0      680 2023-06-26 18:11:41.074743 compmec_section-0.1.2/pyproject.toml
+-rw-r--r--   0        0        0     1778 2023-06-26 18:11:41.075736 compmec_section-0.1.2/README.md
+-rw-r--r--   0        0        0      295 2023-06-26 17:14:35.445886 compmec_section-0.1.2/src/compmec/section/__init__.py
+-rw-r--r--   0        0        0     3049 2023-06-26 18:11:41.076737 compmec_section-0.1.2/src/compmec/section/material.py
+-rw-r--r--   0        0        0        0 2023-06-26 17:14:35.431349 compmec_section-0.1.2/src/compmec/section/profile.py
+-rw-r--r--   0        0        0     5339 2023-06-26 17:14:35.453481 compmec_section-0.1.2/src/compmec/section/shape.py
+-rw-r--r--   0        0        0     2339 1970-01-01 00:00:00.000000 compmec_section-0.1.2/PKG-INFO
```

### Comparing `compmec_section-0.1.0/LICENSE.md` & `compmec_section-0.1.2/LICENSE.md`

 * *Files identical despite different names*

### Comparing `compmec_section-0.1.0/pyproject.toml` & `compmec_section-0.1.2/pyproject.toml`

 * *Files 11% similar despite different names*

```diff
@@ -1,21 +1,25 @@
 [tool.poetry]
 name = "compmec-section"
-version = "0.1.0"
-description = ""
+version = "0.1.2"
+description = "Compute characteristics of an arbitrary cross-section in python"
 authors = ["Carlos Adir <carlos.adir.leite@gmail.com>"]
 readme = "README.md"
 packages = [{ include = "compmec/section", from = "src" }]
 
 [tool.poetry.dependencies]
-python = "^3.10"
+numpy = "^1.0.0"
+python = "^3.7"
 
 [tool.poetry.dev-dependencies]
 pytest = "^5.2"
 
 [tool.poetry.group.dev.dependencies]
 pre-commit = "^3.3.3"
 scriv = {extras = ["toml"], version = "^1.3.1"}
 
 [build-system]
 requires = ["poetry-core"]
 build-backend = "poetry.core.masonry.api"
+
+[tool.scriv]
+version = "literal: src/compmec/section/__init__.py: __version__"
```

