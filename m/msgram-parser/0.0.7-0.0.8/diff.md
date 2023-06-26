# Comparing `tmp/msgram-parser-0.0.7.tar.gz` & `tmp/msgram-parser-0.0.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "msgram-parser-0.0.7.tar", last modified: Sun Jun 25 21:40:59 2023, max compression
+gzip compressed data, was "msgram-parser-0.0.8.tar", last modified: Mon Jun 26 18:47:32 2023, max compression
```

## Comparing `msgram-parser-0.0.7.tar` & `msgram-parser-0.0.8.tar`

### file list

```diff
@@ -1,30 +1,30 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-25 21:40:59.685420 msgram-parser-0.0.7/
--rw-r--r--   0 runner    (1001) docker     (123)    35149 2023-06-25 21:40:35.000000 msgram-parser-0.0.7/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    44750 2023-06-25 21:40:59.685420 msgram-parser-0.0.7/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     3411 2023-06-25 21:40:35.000000 msgram-parser-0.0.7/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-25 21:40:59.681420 msgram-parser-0.0.7/genericparser/
--rw-r--r--   0 runner    (1001) docker     (123)      109 2023-06-25 21:40:35.000000 msgram-parser-0.0.7/genericparser/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)       81 2023-06-25 21:40:35.000000 msgram-parser-0.0.7/genericparser/accept_plugins.py
--rw-r--r--   0 runner    (1001) docker     (123)     2024 2023-06-25 21:40:35.000000 msgram-parser-0.0.7/genericparser/genericparser.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-25 21:40:59.681420 msgram-parser-0.0.7/genericparser/plugins/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-25 21:40:35.000000 msgram-parser-0.0.7/genericparser/plugins/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-25 21:40:59.681420 msgram-parser-0.0.7/genericparser/plugins/dinamic/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-25 21:40:35.000000 msgram-parser-0.0.7/genericparser/plugins/dinamic/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-25 21:40:59.681420 msgram-parser-0.0.7/genericparser/plugins/domain/
--rw-r--r--   0 runner    (1001) docker     (123)     1921 2023-06-25 21:40:35.000000 msgram-parser-0.0.7/genericparser/plugins/domain/generic_class.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-25 21:40:59.685420 msgram-parser-0.0.7/genericparser/plugins/statics/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-25 21:40:35.000000 msgram-parser-0.0.7/genericparser/plugins/statics/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      697 2023-06-25 21:40:35.000000 msgram-parser-0.0.7/genericparser/plugins/statics/sonarqube.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-25 21:40:59.685420 msgram-parser-0.0.7/genericparser/services/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-25 21:40:35.000000 msgram-parser-0.0.7/genericparser/services/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-25 21:40:59.685420 msgram-parser-0.0.7/msgram_parser.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    44750 2023-06-25 21:40:59.000000 msgram-parser-0.0.7/msgram_parser.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      611 2023-06-25 21:40:59.000000 msgram-parser-0.0.7/msgram_parser.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-25 21:40:59.000000 msgram-parser-0.0.7/msgram_parser.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       87 2023-06-25 21:40:59.000000 msgram-parser-0.0.7/msgram_parser.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       14 2023-06-25 21:40:59.000000 msgram-parser-0.0.7/msgram_parser.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1129 2023-06-25 21:40:35.000000 msgram-parser-0.0.7/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-25 21:40:59.685420 msgram-parser-0.0.7/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-25 21:40:59.685420 msgram-parser-0.0.7/tests/
--rw-r--r--   0 runner    (1001) docker     (123)      391 2023-06-25 21:40:35.000000 msgram-parser-0.0.7/tests/test_extract_mettric_sonarqbe.py
--rw-r--r--   0 runner    (1001) docker     (123)      312 2023-06-25 21:40:35.000000 msgram-parser-0.0.7/tests/tests_main_file.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 18:47:32.436048 msgram-parser-0.0.8/
+-rw-r--r--   0 runner    (1001) docker     (123)    35149 2023-06-26 18:47:02.000000 msgram-parser-0.0.8/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    44750 2023-06-26 18:47:32.436048 msgram-parser-0.0.8/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3411 2023-06-26 18:47:02.000000 msgram-parser-0.0.8/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 18:47:32.432048 msgram-parser-0.0.8/genericparser/
+-rw-r--r--   0 runner    (1001) docker     (123)      109 2023-06-26 18:47:02.000000 msgram-parser-0.0.8/genericparser/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)       81 2023-06-26 18:47:02.000000 msgram-parser-0.0.8/genericparser/accept_plugins.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2024 2023-06-26 18:47:02.000000 msgram-parser-0.0.8/genericparser/genericparser.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 18:47:32.432048 msgram-parser-0.0.8/genericparser/plugins/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-26 18:47:02.000000 msgram-parser-0.0.8/genericparser/plugins/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 18:47:32.432048 msgram-parser-0.0.8/genericparser/plugins/dinamic/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-26 18:47:02.000000 msgram-parser-0.0.8/genericparser/plugins/dinamic/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 18:47:32.432048 msgram-parser-0.0.8/genericparser/plugins/domain/
+-rw-r--r--   0 runner    (1001) docker     (123)     1921 2023-06-26 18:47:02.000000 msgram-parser-0.0.8/genericparser/plugins/domain/generic_class.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 18:47:32.436048 msgram-parser-0.0.8/genericparser/plugins/statics/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-26 18:47:02.000000 msgram-parser-0.0.8/genericparser/plugins/statics/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      785 2023-06-26 18:47:02.000000 msgram-parser-0.0.8/genericparser/plugins/statics/sonarqube.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 18:47:32.436048 msgram-parser-0.0.8/genericparser/services/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-26 18:47:02.000000 msgram-parser-0.0.8/genericparser/services/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 18:47:32.436048 msgram-parser-0.0.8/msgram_parser.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    44750 2023-06-26 18:47:32.000000 msgram-parser-0.0.8/msgram_parser.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      611 2023-06-26 18:47:32.000000 msgram-parser-0.0.8/msgram_parser.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-26 18:47:32.000000 msgram-parser-0.0.8/msgram_parser.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       87 2023-06-26 18:47:32.000000 msgram-parser-0.0.8/msgram_parser.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       14 2023-06-26 18:47:32.000000 msgram-parser-0.0.8/msgram_parser.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1130 2023-06-26 18:47:02.000000 msgram-parser-0.0.8/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-26 18:47:32.436048 msgram-parser-0.0.8/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 18:47:32.436048 msgram-parser-0.0.8/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)      391 2023-06-26 18:47:02.000000 msgram-parser-0.0.8/tests/test_extract_mettric_sonarqbe.py
+-rw-r--r--   0 runner    (1001) docker     (123)      312 2023-06-26 18:47:02.000000 msgram-parser-0.0.8/tests/tests_main_file.py
```

### Comparing `msgram-parser-0.0.7/LICENSE` & `msgram-parser-0.0.8/LICENSE`

 * *Files identical despite different names*

### Comparing `msgram-parser-0.0.7/PKG-INFO` & `msgram-parser-0.0.8/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: msgram-parser
-Version: 0.0.7
+Version: 0.0.8
 Summary: The msgram Parser is a PyPI library that serves as a repository for parsing metrics, meaning that it provides a collection of tools, functions, and resources specifically designed to handle and extract information from metric data.
 Author-email: MeasureSoftGram <measuresoftgram@gmail.com>
 License:                     GNU GENERAL PUBLIC LICENSE
                                Version 3, 29 June 2007
         
          Copyright (C) 2007 Free Software Foundation, Inc. <https://fsf.org/>
          Everyone is permitted to copy and distribute verbatim copies
```

### Comparing `msgram-parser-0.0.7/README.md` & `msgram-parser-0.0.8/README.md`

 * *Files identical despite different names*

### Comparing `msgram-parser-0.0.7/genericparser/genericparser.py` & `msgram-parser-0.0.8/genericparser/genericparser.py`

 * *Files identical despite different names*

### Comparing `msgram-parser-0.0.7/genericparser/plugins/domain/generic_class.py` & `msgram-parser-0.0.8/genericparser/plugins/domain/generic_class.py`

 * *Files identical despite different names*

### Comparing `msgram-parser-0.0.7/genericparser/plugins/statics/sonarqube.py` & `msgram-parser-0.0.8/genericparser/plugins/statics/sonarqube.py`

 * *Files 24% similar despite different names*

```diff
@@ -5,18 +5,19 @@
     def extract(self, input_file):
         metrics = []
         keys = []
         values = []
         for entry in input_file:
             key = entry.get("key", {})
             measures = entry.get("measures", [])
-            for measure in measures:
-                metric = measure.get("metric", None)
-                value = measure.get("value", None)
-                metrics.append(metric)
-                keys.append(key)
-                values.append(value)
+            if entry.get("qualifier") in ["FIL", "UTS", "TRK"]:
+                for measure in measures:
+                    metric = measure.get("metric", None)
+                    value = measure.get("value", None)
+                    metrics.append(metric)
+                    keys.append(key)
+                    values.append(value)
         return {"file_paths": keys, "metrics": metrics, "values": values}
 
 
 def main():
     return ParserSonarQube()
```

### Comparing `msgram-parser-0.0.7/msgram_parser.egg-info/PKG-INFO` & `msgram-parser-0.0.8/msgram_parser.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: msgram-parser
-Version: 0.0.7
+Version: 0.0.8
 Summary: The msgram Parser is a PyPI library that serves as a repository for parsing metrics, meaning that it provides a collection of tools, functions, and resources specifically designed to handle and extract information from metric data.
 Author-email: MeasureSoftGram <measuresoftgram@gmail.com>
 License:                     GNU GENERAL PUBLIC LICENSE
                                Version 3, 29 June 2007
         
          Copyright (C) 2007 Free Software Foundation, Inc. <https://fsf.org/>
          Everyone is permitted to copy and distribute verbatim copies
```

### Comparing `msgram-parser-0.0.7/msgram_parser.egg-info/SOURCES.txt` & `msgram-parser-0.0.8/msgram_parser.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `msgram-parser-0.0.7/pyproject.toml` & `msgram-parser-0.0.8/pyproject.toml`

 * *Files 8% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "msgram-parser"
-version = "0.0.7"
+version = "0.0.8"
 description = "The msgram Parser is a PyPI library that serves as a repository for parsing metrics, meaning that it provides a collection of tools, functions, and resources specifically designed to handle and extract information from metric data."
 readme = "README.md"
 authors = [
     { name = "MeasureSoftGram", email = "measuresoftgram@gmail.com" }
 ]
 license = { file = "LICENSE" }
 classifiers = [
@@ -28,8 +28,8 @@
     ]
 
 
 [tool.mypy]
 strict = true
 
 [project.optional-dependencies]
-dev = ["pytest", "pytest-cov", "setuptools", "wheel"]
+dev = ["pytest", "pytest-cov", "setuptools", "wheel"]
```

