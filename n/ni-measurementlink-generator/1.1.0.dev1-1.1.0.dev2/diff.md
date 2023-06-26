# Comparing `tmp/ni_measurementlink_generator-1.1.0.dev1.tar.gz` & `tmp/ni_measurementlink_generator-1.1.0.dev2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ni_measurementlink_generator-1.1.0.dev1.tar", max compression
+gzip compressed data, was "ni_measurementlink_generator-1.1.0.dev2.tar", max compression
```

## Comparing `ni_measurementlink_generator-1.1.0.dev1.tar` & `ni_measurementlink_generator-1.1.0.dev2.tar`

### file list

```diff
@@ -1,12 +1,13 @@
--rw-r--r--   0        0        0      593 2023-05-18 21:55:42.209840 ni_measurementlink_generator-1.1.0.dev1/README.md
--rw-r--r--   0        0        0      148 2023-05-18 21:55:42.209840 ni_measurementlink_generator-1.1.0.dev1/ni_measurementlink_generator/__main__.py
--rw-r--r--   0        0        0        0 2023-05-18 21:55:42.209840 ni_measurementlink_generator-1.1.0.dev1/ni_measurementlink_generator/py.typed
--rw-r--r--   0        0        0     5599 2023-05-18 21:55:42.209840 ni_measurementlink_generator-1.1.0.dev1/ni_measurementlink_generator/template.py
--rw-r--r--   0        0        0     1690 2023-05-18 21:55:42.209840 ni_measurementlink_generator-1.1.0.dev1/ni_measurementlink_generator/templates/measurement.measproj.mako
--rw-r--r--   0        0        0     5143 2023-05-18 21:55:42.209840 ni_measurementlink_generator-1.1.0.dev1/ni_measurementlink_generator/templates/measurement.measui.mako
--rw-r--r--   0        0        0     1472 2023-05-18 21:55:42.209840 ni_measurementlink_generator-1.1.0.dev1/ni_measurementlink_generator/templates/measurement.py.mako
--rw-r--r--   0        0        0      341 2023-05-18 21:55:42.209840 ni_measurementlink_generator-1.1.0.dev1/ni_measurementlink_generator/templates/measurement.serviceconfig.mako
--rw-r--r--   0        0        0      241 2023-05-18 21:55:42.209840 ni_measurementlink_generator-1.1.0.dev1/ni_measurementlink_generator/templates/start.bat.mako
--rw-r--r--   0        0        0     1602 2023-05-18 21:57:24.107064 ni_measurementlink_generator-1.1.0.dev1/pyproject.toml
--rw-r--r--   0        0        0     1567 1970-01-01 00:00:00.000000 ni_measurementlink_generator-1.1.0.dev1/setup.py
--rw-r--r--   0        0        0     1750 1970-01-01 00:00:00.000000 ni_measurementlink_generator-1.1.0.dev1/PKG-INFO
+-rw-r--r--   0        0        0      593 2023-06-26 21:34:54.108589 ni_measurementlink_generator-1.1.0.dev2/README.md
+-rw-r--r--   0        0        0      148 2023-06-26 21:34:54.108589 ni_measurementlink_generator-1.1.0.dev2/ni_measurementlink_generator/__main__.py
+-rw-r--r--   0        0        0        0 2023-06-26 21:34:54.108589 ni_measurementlink_generator-1.1.0.dev2/ni_measurementlink_generator/py.typed
+-rw-r--r--   0        0        0     5671 2023-06-26 21:34:54.108589 ni_measurementlink_generator-1.1.0.dev2/ni_measurementlink_generator/template.py
+-rw-r--r--   0        0        0    10343 2023-06-26 21:34:54.108589 ni_measurementlink_generator-1.1.0.dev2/ni_measurementlink_generator/templates/_helpers.py.mako
+-rw-r--r--   0        0        0     1690 2023-06-26 21:34:54.108589 ni_measurementlink_generator-1.1.0.dev2/ni_measurementlink_generator/templates/measurement.measproj.mako
+-rw-r--r--   0        0        0     5143 2023-06-26 21:34:54.108589 ni_measurementlink_generator-1.1.0.dev2/ni_measurementlink_generator/templates/measurement.measui.mako
+-rw-r--r--   0        0        0     1472 2023-06-26 21:34:54.108589 ni_measurementlink_generator-1.1.0.dev2/ni_measurementlink_generator/templates/measurement.py.mako
+-rw-r--r--   0        0        0      341 2023-06-26 21:34:54.108589 ni_measurementlink_generator-1.1.0.dev2/ni_measurementlink_generator/templates/measurement.serviceconfig.mako
+-rw-r--r--   0        0        0      241 2023-06-26 21:34:54.108589 ni_measurementlink_generator-1.1.0.dev2/ni_measurementlink_generator/templates/start.bat.mako
+-rw-r--r--   0        0        0     1602 2023-06-26 21:36:36.225855 ni_measurementlink_generator-1.1.0.dev2/pyproject.toml
+-rw-r--r--   0        0        0     1567 1970-01-01 00:00:00.000000 ni_measurementlink_generator-1.1.0.dev2/setup.py
+-rw-r--r--   0        0        0     1750 1970-01-01 00:00:00.000000 ni_measurementlink_generator-1.1.0.dev2/PKG-INFO
```

### Comparing `ni_measurementlink_generator-1.1.0.dev1/README.md` & `ni_measurementlink_generator-1.1.0.dev2/README.md`

 * *Files identical despite different names*

### Comparing `ni_measurementlink_generator-1.1.0.dev1/ni_measurementlink_generator/template.py` & `ni_measurementlink_generator-1.1.0.dev2/ni_measurementlink_generator/template.py`

 * *Files 2% similar despite different names*

```diff
@@ -178,7 +178,8 @@
         _create_file(
             "measurement.measproj.mako",
             f"{display_name_for_filenames}.measproj",
             directory_out_path,
             ui_file=ui_file,
         )
     _create_file("start.bat.mako", "start.bat", directory_out_path)
+    _create_file("_helpers.py.mako", "_helpers.py", directory_out_path)
```

### Comparing `ni_measurementlink_generator-1.1.0.dev1/ni_measurementlink_generator/templates/measurement.measproj.mako` & `ni_measurementlink_generator-1.1.0.dev2/ni_measurementlink_generator/templates/measurement.measproj.mako`

 * *Files identical despite different names*

### Comparing `ni_measurementlink_generator-1.1.0.dev1/ni_measurementlink_generator/templates/measurement.measui.mako` & `ni_measurementlink_generator-1.1.0.dev2/ni_measurementlink_generator/templates/measurement.measui.mako`

 * *Files identical despite different names*

### Comparing `ni_measurementlink_generator-1.1.0.dev1/ni_measurementlink_generator/templates/measurement.py.mako` & `ni_measurementlink_generator-1.1.0.dev2/ni_measurementlink_generator/templates/measurement.py.mako`

 * *Files identical despite different names*

### Comparing `ni_measurementlink_generator-1.1.0.dev1/pyproject.toml` & `ni_measurementlink_generator-1.1.0.dev2/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "ni_measurementlink_generator"
-version = "1.1.0-dev1"
+version = "1.1.0-dev2"
 description = "MeasurementLink Code Generator for Python"
 authors = ["NI <opensource@ni.com>"]
 readme = "README.md"
 repository = "https://github.com/ni/measurementlink-python/"
 license = "MIT"
 classifiers = [
     "Development Status :: 5 - Production/Stable",
```

### Comparing `ni_measurementlink_generator-1.1.0.dev1/setup.py` & `ni_measurementlink_generator-1.1.0.dev2/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -12,15 +12,15 @@
 
 entry_points = \
 {'console_scripts': ['ni-measurementlink-generator = '
                      'ni_measurementlink_generator.template:create_measurement']}
 
 setup_kwargs = {
     'name': 'ni-measurementlink-generator',
-    'version': '1.1.0.dev1',
+    'version': '1.1.0.dev2',
     'description': 'MeasurementLink Code Generator for Python',
     'long_description': '# MeasurementLink™ Code Generator for Python\n\n---\n\n## Introduction\n\nMeasurementLink Code Generator for Python (`ni-measurementlink-generator`) is a tool for generating measurement plugins.\n\nFor installation and usage, see [MeasurementLink Support for Python (`ni-measurementlink-service`)](https://pypi.org/project/ni-measurementlink-service/).\n\n---\n\n## Dependencies\n\n- Python >= 3.8 [(3.9 recommended)](https://www.python.org/downloads/release/python-3913/)\n- [mako >= 1.2.1, < 2.x](https://pypi.org/project/Mako/1.2.1/)\n- [click >= 8.1.3, < 9.x](https://pypi.org/project/click/8.1.3/)\n\n---',
     'author': 'NI',
     'author_email': 'opensource@ni.com',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'https://github.com/ni/measurementlink-python/',
```

### Comparing `ni_measurementlink_generator-1.1.0.dev1/PKG-INFO` & `ni_measurementlink_generator-1.1.0.dev2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ni-measurementlink-generator
-Version: 1.1.0.dev1
+Version: 1.1.0.dev2
 Summary: MeasurementLink Code Generator for Python
 Home-page: https://github.com/ni/measurementlink-python/
 License: MIT
 Author: NI
 Author-email: opensource@ni.com
 Requires-Python: >=3.8,<4.0
 Classifier: Development Status :: 5 - Production/Stable
```

