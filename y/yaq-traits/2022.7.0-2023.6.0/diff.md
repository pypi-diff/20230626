# Comparing `tmp/yaq-traits-2022.7.0.tar.gz` & `tmp/yaq_traits-2023.6.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "yaq-traits-2022.7.0.tar", last modified: Tue Jul 12 20:21:19 2022, max compression
+gzip compressed data, was "yaq_traits-2023.6.0.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
```

## Comparing `yaq-traits-2022.7.0.tar` & `yaq_traits-2023.6.0.tar`

### file list

```diff
@@ -1,35 +1,35 @@
--rw-r--r--   0        0        0       20 2022-07-12 20:21:00.774928 yaq-traits-2022.7.0/.github/CODEOWNERS
--rw-r--r--   0        0        0      825 2022-07-12 20:21:00.774928 yaq-traits-2022.7.0/.github/workflows/python-publish.yml
--rw-r--r--   0        0        0      638 2022-07-12 20:21:00.774928 yaq-traits-2022.7.0/.github/workflows/run-entry-points.yml
--rw-r--r--   0        0        0      447 2022-07-12 20:21:00.774928 yaq-traits-2022.7.0/.gitignore
--rw-r--r--   0        0        0      589 2022-07-12 20:21:00.774928 yaq-traits-2022.7.0/.pre-commit-config.yaml
--rw-r--r--   0        0        0      407 2022-07-12 20:21:00.774928 yaq-traits-2022.7.0/.pre-commit-hooks.yaml
--rw-r--r--   0        0        0     5640 2022-07-12 20:21:00.774928 yaq-traits-2022.7.0/CHANGELOG.md
--rw-r--r--   0        0        0     7652 2022-07-12 20:21:00.774928 yaq-traits-2022.7.0/LICENSE
--rw-r--r--   0        0        0     1003 2022-07-12 20:21:00.774928 yaq-traits-2022.7.0/README.md
--rw-r--r--   0        0        0       14 2022-07-12 20:21:00.774928 yaq-traits-2022.7.0/docs/CNAME
--rw-r--r--   0        0        0    12598 2022-07-12 20:21:00.774928 yaq-traits-2022.7.0/docs/index.html
--rw-r--r--   0        0        0      737 2022-07-12 20:21:00.774928 yaq-traits-2022.7.0/docs/style.css
--rw-r--r--   0        0        0     1278 2022-07-12 20:21:00.774928 yaq-traits-2022.7.0/pyproject.toml
--rw-r--r--   0        0        0        9 2022-07-12 20:21:00.774928 yaq-traits-2022.7.0/yaq_traits/VERSION
--rw-r--r--   0        0        0       86 2022-07-12 20:21:00.774928 yaq-traits-2022.7.0/yaq_traits/__init__.py
--rw-r--r--   0        0        0     4087 2022-07-12 20:21:00.774928 yaq-traits-2022.7.0/yaq_traits/__main__.py
--rw-r--r--   0        0        0      252 2022-07-12 20:21:00.774928 yaq-traits-2022.7.0/yaq_traits/__traits__.py
--rw-r--r--   0        0        0      493 2022-07-12 20:21:00.774928 yaq-traits-2022.7.0/yaq_traits/__version__.py
--rw-r--r--   0        0        0     1374 2022-07-12 20:21:00.774928 yaq-traits-2022.7.0/yaq_traits/_check.py
--rw-r--r--   0        0        0     5418 2022-07-12 20:21:00.774928 yaq-traits-2022.7.0/yaq_traits/_compose.py
--rw-r--r--   0        0        0      510 2022-07-12 20:21:00.774928 yaq-traits-2022.7.0/yaq_traits/has-dependents.toml
--rw-r--r--   0        0        0     1156 2022-07-12 20:21:00.774928 yaq-traits-2022.7.0/yaq_traits/has-limits.toml
--rw-r--r--   0        0        0      906 2022-07-12 20:21:00.774928 yaq-traits-2022.7.0/yaq_traits/has-mapping.toml
--rw-r--r--   0        0        0      556 2022-07-12 20:21:00.774928 yaq-traits-2022.7.0/yaq_traits/has-measure-trigger.toml
--rw-r--r--   0        0        0     1831 2022-07-12 20:21:00.774928 yaq-traits-2022.7.0/yaq_traits/has-position.toml
--rw-r--r--   0        0        0     2389 2022-07-12 20:21:00.774928 yaq-traits-2022.7.0/yaq_traits/has-transformed-position.toml
--rw-r--r--   0        0        0      794 2022-07-12 20:21:00.774928 yaq-traits-2022.7.0/yaq_traits/has-turret.toml
--rw-r--r--   0        0        0     1737 2022-07-12 20:21:00.774928 yaq-traits-2022.7.0/yaq_traits/is-daemon.toml
--rw-r--r--   0        0        0     1664 2022-07-12 20:21:00.778928 yaq-traits-2022.7.0/yaq_traits/is-discrete.toml
--rw-r--r--   0        0        0      312 2022-07-12 20:21:00.778928 yaq-traits-2022.7.0/yaq_traits/is-homeable.toml
--rw-r--r--   0        0        0     1043 2022-07-12 20:21:00.778928 yaq-traits-2022.7.0/yaq_traits/is-sensor.toml
--rw-r--r--   0        0        0      184 2022-07-12 20:21:00.778928 yaq-traits-2022.7.0/yaq_traits/uses-i2c.toml
--rw-r--r--   0        0        0      684 2022-07-12 20:21:00.778928 yaq-traits-2022.7.0/yaq_traits/uses-serial.toml
--rw-r--r--   0        0        0      269 2022-07-12 20:21:00.778928 yaq-traits-2022.7.0/yaq_traits/uses-uart.toml
--rw-r--r--   0        0        0     2050 1970-01-01 00:00:00.000000 yaq-traits-2022.7.0/PKG-INFO
+-rw-r--r--   0        0        0       20 2023-06-26 21:00:16.993633 yaq_traits-2023.6.0/.github/CODEOWNERS
+-rw-r--r--   0        0        0      825 2023-06-26 21:00:16.993633 yaq_traits-2023.6.0/.github/workflows/python-publish.yml
+-rw-r--r--   0        0        0      638 2023-06-26 21:00:16.993633 yaq_traits-2023.6.0/.github/workflows/run-entry-points.yml
+-rw-r--r--   0        0        0      447 2023-06-26 21:00:16.993633 yaq_traits-2023.6.0/.gitignore
+-rw-r--r--   0        0        0      589 2023-06-26 21:00:16.993633 yaq_traits-2023.6.0/.pre-commit-config.yaml
+-rw-r--r--   0        0        0      407 2023-06-26 21:00:16.993633 yaq_traits-2023.6.0/.pre-commit-hooks.yaml
+-rw-r--r--   0        0        0     6102 2023-06-26 21:00:16.993633 yaq_traits-2023.6.0/CHANGELOG.md
+-rw-r--r--   0        0        0     7652 2023-06-26 21:00:16.993633 yaq_traits-2023.6.0/LICENSE
+-rw-r--r--   0        0        0     1003 2023-06-26 21:00:16.993633 yaq_traits-2023.6.0/README.md
+-rw-r--r--   0        0        0       14 2023-06-26 21:00:16.993633 yaq_traits-2023.6.0/docs/CNAME
+-rw-r--r--   0        0        0    12598 2023-06-26 21:00:16.993633 yaq_traits-2023.6.0/docs/index.html
+-rw-r--r--   0        0        0      737 2023-06-26 21:00:16.993633 yaq_traits-2023.6.0/docs/style.css
+-rw-r--r--   0        0        0     1278 2023-06-26 21:00:16.993633 yaq_traits-2023.6.0/pyproject.toml
+-rw-r--r--   0        0        0        9 2023-06-26 21:00:16.993633 yaq_traits-2023.6.0/yaq_traits/VERSION
+-rw-r--r--   0        0        0       86 2023-06-26 21:00:16.993633 yaq_traits-2023.6.0/yaq_traits/__init__.py
+-rw-r--r--   0        0        0     4087 2023-06-26 21:00:16.993633 yaq_traits-2023.6.0/yaq_traits/__main__.py
+-rw-r--r--   0        0        0      252 2023-06-26 21:00:16.997633 yaq_traits-2023.6.0/yaq_traits/__traits__.py
+-rw-r--r--   0        0        0      493 2023-06-26 21:00:16.997633 yaq_traits-2023.6.0/yaq_traits/__version__.py
+-rw-r--r--   0        0        0     1374 2023-06-26 21:00:16.997633 yaq_traits-2023.6.0/yaq_traits/_check.py
+-rw-r--r--   0        0        0     5418 2023-06-26 21:00:16.997633 yaq_traits-2023.6.0/yaq_traits/_compose.py
+-rw-r--r--   0        0        0      510 2023-06-26 21:00:16.997633 yaq_traits-2023.6.0/yaq_traits/has-dependents.toml
+-rw-r--r--   0        0        0     1156 2023-06-26 21:00:16.997633 yaq_traits-2023.6.0/yaq_traits/has-limits.toml
+-rw-r--r--   0        0        0      906 2023-06-26 21:00:16.997633 yaq_traits-2023.6.0/yaq_traits/has-mapping.toml
+-rw-r--r--   0        0        0      556 2023-06-26 21:00:16.997633 yaq_traits-2023.6.0/yaq_traits/has-measure-trigger.toml
+-rw-r--r--   0        0        0     1831 2023-06-26 21:00:16.997633 yaq_traits-2023.6.0/yaq_traits/has-position.toml
+-rw-r--r--   0        0        0     2713 2023-06-26 21:00:16.997633 yaq_traits-2023.6.0/yaq_traits/has-transformed-position.toml
+-rw-r--r--   0        0        0      794 2023-06-26 21:00:16.997633 yaq_traits-2023.6.0/yaq_traits/has-turret.toml
+-rw-r--r--   0        0        0     1737 2023-06-26 21:00:16.997633 yaq_traits-2023.6.0/yaq_traits/is-daemon.toml
+-rw-r--r--   0        0        0     1664 2023-06-26 21:00:16.997633 yaq_traits-2023.6.0/yaq_traits/is-discrete.toml
+-rw-r--r--   0        0        0      312 2023-06-26 21:00:16.997633 yaq_traits-2023.6.0/yaq_traits/is-homeable.toml
+-rw-r--r--   0        0        0     1043 2023-06-26 21:00:16.997633 yaq_traits-2023.6.0/yaq_traits/is-sensor.toml
+-rw-r--r--   0        0        0      184 2023-06-26 21:00:16.997633 yaq_traits-2023.6.0/yaq_traits/uses-i2c.toml
+-rw-r--r--   0        0        0      684 2023-06-26 21:00:16.997633 yaq_traits-2023.6.0/yaq_traits/uses-serial.toml
+-rw-r--r--   0        0        0      269 2023-06-26 21:00:16.997633 yaq_traits-2023.6.0/yaq_traits/uses-uart.toml
+-rw-r--r--   0        0        0     2050 1970-01-01 00:00:00.000000 yaq_traits-2023.6.0/PKG-INFO
```

### Comparing `yaq-traits-2022.7.0/.github/workflows/python-publish.yml` & `yaq_traits-2023.6.0/.github/workflows/python-publish.yml`

 * *Files identical despite different names*

### Comparing `yaq-traits-2022.7.0/.github/workflows/run-entry-points.yml` & `yaq_traits-2023.6.0/.github/workflows/run-entry-points.yml`

 * *Files identical despite different names*

### Comparing `yaq-traits-2022.7.0/.pre-commit-config.yaml` & `yaq_traits-2023.6.0/.pre-commit-config.yaml`

 * *Files 4% similar despite different names*

```diff
@@ -1,26 +1,26 @@
 repos:
   - repo: https://github.com/pre-commit/pre-commit-hooks
-    rev: v4.3.0
+    rev: v4.4.0
     hooks:
     -   id: trailing-whitespace
     -   id: no-commit-to-branch
         args: [-b main]
 
   - repo: https://github.com/psf/black
-    rev: 22.6.0
+    rev: 23.3.0
     hooks:
       - id: black
         name: black
         entry: black
         require_serial: true
         types: [python]
 
   - repo: https://github.com/pre-commit/mirrors-mypy
-    rev: v0.961
+    rev: v1.3.0
     hooks:
       - id: mypy
         exclude: ^docs/conf.py
         additional_dependencies:
           - types-toml
 
 default_language_version:
```

### Comparing `yaq-traits-2022.7.0/CHANGELOG.md` & `yaq_traits-2023.6.0/CHANGELOG.md`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,25 @@
  Changelog
 All notable changes to this project will be documented in this file.
 
 The format is based on [Keep a Changelog](https://keepachangelog.com/).
 
 ## Unreleased
 
+## [2023.6.0]
+
+### Added
+- config native_limits for `has-transformed-position` trait
+
+## [2022.11.0]
+
+### Fixed
+- `has-transformed-position` accepts null type for native units (like `has-position`)
+- fixed bug in `has-transformed-position` where `get_native_destination` was not a message
+
 ## [2022.7.0]
 
 ### Added
 - has-transformed-position trait for using non-native coordinates to address position
 - has-dependents trait for informing clients about relationships between daemons
 
 ## [2022.5.0]
@@ -156,15 +167,17 @@
 - general fixes for all traits
 
 ## [2020.06.0]
 
 ### Added
 - initial release
 
-[Unreleased]: https://github.com/yaq-project/yaq-traits/compare/v2022.7.0...main
+[Unreleased]: https://github.com/yaq-project/yaq-traits/compare/v2023.6.0...main
+[2023.06.0]: https://github.com/yaq-project/yaq-traits/compare/v2022.11.0...v2023.6.0
+[2022.11.0]: https://github.com/yaq-project/yaq-traits/compare/v2022.7.0...v2022.11.0
 [2022.7.0]: https://github.com/yaq-project/yaq-traits/compare/v2022.5.0...v2022.7.0
 [2022.5.0]: https://github.com/yaq-project/yaq-traits/compare/v2022.3.0...v2022.5.0
 [2022.3.0]: https://github.com/yaq-project/yaq-traits/compare/v2021.10.0...v2022.3.0
 [2021.10.0]: https://github.com/yaq-project/yaq-traits/compare/v2021.4.0...v2021.10.0
 [2021.4.0]: https://github.com/yaq-project/yaq-traits/compare/v2021.3.2...v2021.4.0
 [2021.3.2]: https://github.com/yaq-project/yaq-traits/compare/v2021.3.1...v2021.3.2
 [2021.3.1]: https://github.com/yaq-project/yaq-traits/compare/v2021.3.0...v2021.3.1
```

### Comparing `yaq-traits-2022.7.0/LICENSE` & `yaq_traits-2023.6.0/LICENSE`

 * *Files identical despite different names*

### Comparing `yaq-traits-2022.7.0/README.md` & `yaq_traits-2023.6.0/README.md`

 * *Files identical despite different names*

### Comparing `yaq-traits-2022.7.0/docs/index.html` & `yaq_traits-2023.6.0/docs/index.html`

 * *Files identical despite different names*

### Comparing `yaq-traits-2022.7.0/docs/style.css` & `yaq_traits-2023.6.0/docs/style.css`

 * *Files identical despite different names*

### Comparing `yaq-traits-2022.7.0/pyproject.toml` & `yaq_traits-2023.6.0/pyproject.toml`

 * *Files identical despite different names*

### Comparing `yaq-traits-2022.7.0/yaq_traits/__main__.py` & `yaq_traits-2023.6.0/yaq_traits/__main__.py`

 * *Files identical despite different names*

### Comparing `yaq-traits-2022.7.0/yaq_traits/_check.py` & `yaq_traits-2023.6.0/yaq_traits/_check.py`

 * *Files identical despite different names*

### Comparing `yaq-traits-2022.7.0/yaq_traits/_compose.py` & `yaq_traits-2023.6.0/yaq_traits/_compose.py`

 * *Files identical despite different names*

### Comparing `yaq-traits-2022.7.0/yaq_traits/has-limits.toml` & `yaq_traits-2023.6.0/yaq_traits/has-limits.toml`

 * *Files identical despite different names*

### Comparing `yaq-traits-2022.7.0/yaq_traits/has-mapping.toml` & `yaq_traits-2023.6.0/yaq_traits/has-mapping.toml`

 * *Files identical despite different names*

### Comparing `yaq-traits-2022.7.0/yaq_traits/has-measure-trigger.toml` & `yaq_traits-2023.6.0/yaq_traits/has-measure-trigger.toml`

 * *Files identical despite different names*

### Comparing `yaq-traits-2022.7.0/yaq_traits/has-position.toml` & `yaq_traits-2023.6.0/yaq_traits/has-position.toml`

 * *Files identical despite different names*

### Comparing `yaq-traits-2022.7.0/yaq_traits/has-transformed-position.toml` & `yaq_traits-2023.6.0/yaq_traits/has-transformed-position.toml`

 * *Files 3% similar despite different names*

```diff
@@ -4,14 +4,23 @@
 two coordinate systems. One frame (the "transformed" frame) is for common
 client control. The other frame (the "native" frame) reports position in terms
 of low-level motor control.
 """
 requires = ["has-limits"]
 
 
+[config]
+
+[config.native_limits]
+type = "array"
+items = "double"
+default = [-inf, +inf]
+doc = "Bounds of motion specified in native coordinates.  To specify bounds in transformed coordinates, use `limits`."
+
+
 [state]
 
 [state.native_reference_position]
 doc = """The reference position, expressed in native coordinates.
 Default is `0.0`"""
 type = "double"
 default = 0.0
@@ -58,16 +67,19 @@
 
 [messages.get_native_limits]
 doc = "Returns limits in the relative coordinate system."
 response = {"type"="array", "items"="double"}
 
 [messages.get_native_units]
 doc = "Get the units of native coordinates."
-response = "string"
+response = ["null", "string"]
 
+[messages.get_native_destination]
+doc = "Get the destination in native coordinates."
+response = "double"
 
 [properties]
 
 [properties.native_reference_position]
 getter = "get_native_reference"
 setter = "set_native_reference"
 units_getter = "get_native_units"
```

### Comparing `yaq-traits-2022.7.0/yaq_traits/has-turret.toml` & `yaq_traits-2023.6.0/yaq_traits/has-turret.toml`

 * *Files identical despite different names*

### Comparing `yaq-traits-2022.7.0/yaq_traits/is-daemon.toml` & `yaq_traits-2023.6.0/yaq_traits/is-daemon.toml`

 * *Files identical despite different names*

### Comparing `yaq-traits-2022.7.0/yaq_traits/is-discrete.toml` & `yaq_traits-2023.6.0/yaq_traits/is-discrete.toml`

 * *Files identical despite different names*

### Comparing `yaq-traits-2022.7.0/yaq_traits/is-sensor.toml` & `yaq_traits-2023.6.0/yaq_traits/is-sensor.toml`

 * *Files identical despite different names*

### Comparing `yaq-traits-2022.7.0/yaq_traits/uses-serial.toml` & `yaq_traits-2023.6.0/yaq_traits/uses-serial.toml`

 * *Files identical despite different names*

### Comparing `yaq-traits-2022.7.0/PKG-INFO` & `yaq_traits-2023.6.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: yaq-traits
-Version: 2022.7.0
+Version: 2023.6.0
 Summary: package defining yaq traits
 Home-page: https://traits.yaq.fyi
 Author: yaq Developers
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Science/Research
```

