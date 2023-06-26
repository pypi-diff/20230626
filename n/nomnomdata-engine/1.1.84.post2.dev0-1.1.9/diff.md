# Comparing `tmp/nomnomdata_engine-1.1.84.post2.dev0.tar.gz` & `tmp/nomnomdata-engine-1.1.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nomnomdata_engine-1.1.84.post2.dev0.tar", max compression
+gzip compressed data, was "nomnomdata-engine-1.1.9.tar", max compression
```

## Comparing `nomnomdata_engine-1.1.84.post2.dev0.tar` & `nomnomdata-engine-1.1.9.tar`

### file list

```diff
@@ -1,17 +1,18 @@
--rw-r--r--   0        0        0      702 2023-06-26 19:19:08.419372 nomnomdata_engine-1.1.84.post2.dev0/LICENSE
--rw-r--r--   0        0        0       37 2023-06-26 19:19:08.419372 nomnomdata_engine-1.1.84.post2.dev0/README.md
--rw-r--r--   0        0        0      432 2023-06-26 19:19:08.419372 nomnomdata_engine-1.1.84.post2.dev0/nomnomdata/engine/__init__.py
--rw-r--r--   0        0        0    10061 2023-06-26 19:19:08.419372 nomnomdata_engine-1.1.84.post2.dev0/nomnomdata/engine/components.py
--rw-r--r--   0        0        0    72521 2023-06-26 19:19:08.419372 nomnomdata_engine-1.1.84.post2.dev0/nomnomdata/engine/connections.py
--rw-r--r--   0        0        0     5598 2023-06-26 19:19:08.419372 nomnomdata_engine-1.1.84.post2.dev0/nomnomdata/engine/encoders.py
--rw-r--r--   0        0        0    14368 2023-06-26 19:19:08.420373 nomnomdata_engine-1.1.84.post2.dev0/nomnomdata/engine/engine.py
--rw-r--r--   0        0        0      516 2023-06-26 19:19:08.420373 nomnomdata_engine-1.1.84.post2.dev0/nomnomdata/engine/errors.py
--rw-r--r--   0        0        0      290 2023-06-26 19:19:08.420373 nomnomdata_engine-1.1.84.post2.dev0/nomnomdata/engine/globals.py
--rw-r--r--   0        0        0     2448 2023-06-26 19:19:08.420373 nomnomdata_engine-1.1.84.post2.dev0/nomnomdata/engine/logging.py
--rw-r--r--   0        0        0    11023 2023-06-26 19:19:08.420373 nomnomdata_engine-1.1.84.post2.dev0/nomnomdata/engine/nominode.py
--rw-r--r--   0        0        0     9574 2023-06-26 19:19:08.420373 nomnomdata_engine-1.1.84.post2.dev0/nomnomdata/engine/parameters.py
--rw-r--r--   0        0        0    35388 2023-06-26 19:19:08.420373 nomnomdata_engine-1.1.84.post2.dev0/nomnomdata/engine/shared_configs.py
--rw-r--r--   0        0        0     4357 2023-06-26 19:19:08.420373 nomnomdata_engine-1.1.84.post2.dev0/nomnomdata/engine/testing.py
--rw-r--r--   0        0        0      162 2023-06-26 19:19:08.420373 nomnomdata_engine-1.1.84.post2.dev0/nomnomdata/engine/util.py
--rw-r--r--   0        0        0     1302 2023-06-26 19:19:22.132170 nomnomdata_engine-1.1.84.post2.dev0/pyproject.toml
--rw-r--r--   0        0        0     1142 1970-01-01 00:00:00.000000 nomnomdata_engine-1.1.84.post2.dev0/PKG-INFO
+-rw-r--r--   0        0        0      702 2021-03-23 15:35:19.464848 nomnomdata-engine-1.1.9/LICENSE
+-rw-r--r--   0        0        0       40 2021-03-23 15:35:19.464848 nomnomdata-engine-1.1.9/README.md
+-rw-r--r--   0        0        0      432 2021-03-23 15:35:19.464848 nomnomdata-engine-1.1.9/nomnomdata/engine/__init__.py
+-rw-r--r--   0        0        0     9869 2021-03-23 15:35:19.464848 nomnomdata-engine-1.1.9/nomnomdata/engine/components.py
+-rw-r--r--   0        0        0    30556 2021-03-23 15:35:19.464848 nomnomdata-engine-1.1.9/nomnomdata/engine/connections.py
+-rw-r--r--   0        0        0     5426 2021-03-23 15:35:19.464848 nomnomdata-engine-1.1.9/nomnomdata/engine/encoders.py
+-rw-r--r--   0        0        0    14368 2021-03-23 15:35:19.464848 nomnomdata-engine-1.1.9/nomnomdata/engine/engine.py
+-rw-r--r--   0        0        0      516 2021-03-23 15:35:19.464848 nomnomdata-engine-1.1.9/nomnomdata/engine/errors.py
+-rw-r--r--   0        0        0      290 2021-03-23 15:35:19.464848 nomnomdata-engine-1.1.9/nomnomdata/engine/globals.py
+-rw-r--r--   0        0        0     2448 2021-03-23 15:35:19.464848 nomnomdata-engine-1.1.9/nomnomdata/engine/logging.py
+-rw-r--r--   0        0        0    11023 2021-03-23 15:35:19.464848 nomnomdata-engine-1.1.9/nomnomdata/engine/nominode.py
+-rw-r--r--   0        0        0     9574 2021-03-23 15:35:19.464848 nomnomdata-engine-1.1.9/nomnomdata/engine/parameters.py
+-rw-r--r--   0        0        0    15475 2021-03-23 15:35:19.464848 nomnomdata-engine-1.1.9/nomnomdata/engine/shared_configs.py
+-rw-r--r--   0        0        0     4357 2021-03-23 15:35:19.464848 nomnomdata-engine-1.1.9/nomnomdata/engine/testing.py
+-rw-r--r--   0        0        0      162 2021-03-23 15:35:19.464848 nomnomdata-engine-1.1.9/nomnomdata/engine/util.py
+-rw-r--r--   0        0        0     1269 2021-03-23 15:35:41.196843 nomnomdata-engine-1.1.9/pyproject.toml
+-rw-r--r--   0        0        0      907 2021-03-23 15:35:42.349421 nomnomdata-engine-1.1.9/setup.py
+-rw-r--r--   0        0        0      995 2021-03-23 15:35:42.349753 nomnomdata-engine-1.1.9/PKG-INFO
```

### Comparing `nomnomdata_engine-1.1.84.post2.dev0/LICENSE` & `nomnomdata-engine-1.1.9/LICENSE`

 * *Files identical despite different names*

### Comparing `nomnomdata_engine-1.1.84.post2.dev0/nomnomdata/engine/components.py` & `nomnomdata-engine-1.1.9/nomnomdata/engine/components.py`

 * *Files 5% similar despite different names*

```diff
@@ -31,20 +31,14 @@
     def dump(self, val):
         return val
 
     def load(self, val):
         return val
 
 
-class Rule:
-    def __init__(self, name: str = "", value: List[str] = [""]):
-        self.name = name
-        self.value = value
-
-
 class Parameter:
     """
     Parameter for use in a ParameterGroup, also contains options
     to control the look in the Nominode UI
 
     :param type:
         Set the type to allow validation of the parameter and
@@ -80,15 +74,14 @@
         help_header_id: str = None,
         help_md_path: str = None,
         required: bool = False,
         description: str = "",
         default: object = None,
         many: bool = False,
         categories: List[str] = None,
-        show_on: Rule = None,
     ):
         if (
             not isinstance(type, ParameterType)
             and type is not None
             and issubclass(type, ParameterType)
         ):
             raise ValueError(f"{type} is not an instance, perhaps a forgotten ()?")
@@ -114,15 +107,14 @@
         self.required = required
         self.description = description
         if default:
             type.validate(default)
         self.default = default
         self.many = many
         self.categories = [{"name": val} for val in categories] if categories else None
-        self.show_on = show_on
 
     def validate(self, value: Any):
         self._verify_required(value)
         if self.many and value is not None:
             for v in value:
                 self._validate(v)
         else:
```

### Comparing `nomnomdata_engine-1.1.84.post2.dev0/nomnomdata/engine/encoders.py` & `nomnomdata-engine-1.1.9/nomnomdata/engine/encoders.py`

 * *Files 2% similar despite different names*

```diff
@@ -115,19 +115,14 @@
             result["help"] = p.help
         if p.default:
             result["default"] = p.type.dump(p.default)
         if p.many:
             result["many"] = p.many
         if p.categories:
             result["categories"] = p.categories
-        if p.show_on:
-            result["show_on"] = {
-                "parameter_name": p.show_on.name,
-                "parameter_value": p.show_on.value,
-            }
         if isinstance(p.type, Connection):
             result.update(self.serialize_connection_parameter(p.type))
         elif isinstance(p.type, SharedConfig):
             result.update(self.serialize_shared_config_parameter(p.type))
         else:
             result.update(self.serialize_parameter_type(p.type))
         return result
```

### Comparing `nomnomdata_engine-1.1.84.post2.dev0/nomnomdata/engine/engine.py` & `nomnomdata-engine-1.1.9/nomnomdata/engine/engine.py`

 * *Files identical despite different names*

### Comparing `nomnomdata_engine-1.1.84.post2.dev0/nomnomdata/engine/errors.py` & `nomnomdata-engine-1.1.9/nomnomdata/engine/errors.py`

 * *Files identical despite different names*

### Comparing `nomnomdata_engine-1.1.84.post2.dev0/nomnomdata/engine/logging.py` & `nomnomdata-engine-1.1.9/nomnomdata/engine/logging.py`

 * *Files identical despite different names*

### Comparing `nomnomdata_engine-1.1.84.post2.dev0/nomnomdata/engine/nominode.py` & `nomnomdata-engine-1.1.9/nomnomdata/engine/nominode.py`

 * *Files identical despite different names*

### Comparing `nomnomdata_engine-1.1.84.post2.dev0/nomnomdata/engine/parameters.py` & `nomnomdata-engine-1.1.9/nomnomdata/engine/parameters.py`

 * *Files identical despite different names*

### Comparing `nomnomdata_engine-1.1.84.post2.dev0/nomnomdata/engine/testing.py` & `nomnomdata-engine-1.1.9/nomnomdata/engine/testing.py`

 * *Files identical despite different names*

### Comparing `nomnomdata_engine-1.1.84.post2.dev0/pyproject.toml` & `nomnomdata-engine-1.1.9/pyproject.toml`

 * *Files 24% similar despite different names*

```diff
@@ -4,25 +4,24 @@
 license = "LGPL-3.0-only"
 name = "nomnomdata-engine"
 packages = [
   {include = "nomnomdata"},
 ]
 readme = "README.md"
 repository = "https://gitlab.com/nomnomdata/tools/nomnomdata-engine"
-version = "1.1.84.post2.dev0"
+version = "1.1.9"
 
 [tool.poetry.dependencies]
 dunamai = "^1.1.0"
 httmock = "^1.3.0"
 nomnomdata-cli = "^0.1.7"
 python = "^3.7"
 pyyaml = "^5.3.1"
 requests = "^2.23.0"
 wrapt = "^1.12.1"
-MarkupSafe = "2.0.1"
 
 [tool.poetry.dev-dependencies]
 genson = "^1.2.1"
 pytest = "^6.0.1"
 pytest-cov = "^2.10.0"
 pytest-snapshot = "^0.4.2"
```

### Comparing `nomnomdata_engine-1.1.84.post2.dev0/PKG-INFO` & `nomnomdata-engine-1.1.9/PKG-INFO`

 * *Files 21% similar despite different names*

```diff
@@ -1,28 +1,25 @@
 Metadata-Version: 2.1
 Name: nomnomdata-engine
-Version: 1.1.84.post2.dev0
+Version: 1.1.9
 Summary: Package containing tooling for developing nominode engines
 Home-page: https://gitlab.com/nomnomdata/tools/nomnomdata-engine
 License: LGPL-3.0-only
 Author: Nom Nom Data Inc
 Author-email: info@nomnomdata.com
 Requires-Python: >=3.7,<4.0
 Classifier: License :: OSI Approved :: GNU Lesser General Public License v3 (LGPLv3)
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
-Classifier: Programming Language :: Python :: 3.10
-Classifier: Programming Language :: Python :: 3.11
-Requires-Dist: MarkupSafe (==2.0.1)
 Requires-Dist: dunamai (>=1.1.0,<2.0.0)
 Requires-Dist: httmock (>=1.3.0,<2.0.0)
 Requires-Dist: nomnomdata-cli (>=0.1.7,<0.2.0)
 Requires-Dist: pyyaml (>=5.3.1,<6.0.0)
 Requires-Dist: requests (>=2.23.0,<3.0.0)
 Requires-Dist: wrapt (>=1.12.1,<2.0.0)
 Project-URL: Repository, https://gitlab.com/nomnomdata/tools/nomnomdata-engine
 Description-Content-Type: text/markdown
 
-Package for developing Nominode apps
+Package for developing nominode engines
```

