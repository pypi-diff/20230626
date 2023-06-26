# Comparing `tmp/jsonablr-0.1.0.tar.gz` & `tmp/jsonablr-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "jsonablr-0.1.0.tar", max compression
+gzip compressed data, was "jsonablr-0.1.1.tar", max compression
```

## Comparing `jsonablr-0.1.0.tar` & `jsonablr-0.1.1.tar`

### file list

```diff
@@ -1,6 +1,6 @@
--rw-r--r--   0        0        0     1076 2023-06-26 17:24:04.431422 jsonablr-0.1.0/LICENSE
--rw-r--r--   0        0        0     1907 2023-06-26 17:24:04.437195 jsonablr-0.1.0/README.md
--rw-r--r--   0        0        0      182 2023-06-26 17:24:04.437373 jsonablr-0.1.0/jsonablr/__init__.py
--rw-r--r--   0        0        0     5957 2023-06-26 17:24:04.437555 jsonablr-0.1.0/jsonablr/main.py
--rw-r--r--   0        0        0      530 2023-06-26 17:29:24.082000 jsonablr-0.1.0/pyproject.toml
--rw-r--r--   0        0        0     2538 1970-01-01 00:00:00.000000 jsonablr-0.1.0/PKG-INFO
+-rw-r--r--   0        0        0     1076 2023-06-26 17:24:04.431422 jsonablr-0.1.1/LICENSE
+-rw-r--r--   0        0        0     1907 2023-06-26 17:24:04.437195 jsonablr-0.1.1/README.md
+-rw-r--r--   0        0        0      182 2023-06-26 17:24:04.437373 jsonablr-0.1.1/jsonablr/__init__.py
+-rw-r--r--   0        0        0     6038 2023-06-26 18:57:40.127262 jsonablr-0.1.1/jsonablr/main.py
+-rw-r--r--   0        0        0      530 2023-06-26 19:00:42.088367 jsonablr-0.1.1/pyproject.toml
+-rw-r--r--   0        0        0     2538 1970-01-01 00:00:00.000000 jsonablr-0.1.1/PKG-INFO
```

### Comparing `jsonablr-0.1.0/LICENSE` & `jsonablr-0.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `jsonablr-0.1.0/README.md` & `jsonablr-0.1.1/README.md`

 * *Files identical despite different names*

### Comparing `jsonablr-0.1.0/jsonablr/main.py` & `jsonablr-0.1.1/jsonablr/main.py`

 * *Files 6% similar despite different names*

```diff
@@ -170,22 +170,24 @@
 
         if self.options.include is not None:
             allowed_keys &= set(self.options.include)
         if self.options.exclude is not None:
             allowed_keys -= set(self.options.exclude)
 
         encoder = self.__class__(
-            options=Options.parse_obj(self.options.dict(include={
-                'by_alias',
-                'exclude_unset',
-                'exclude_none',
-                'exclude_defaults',
-                'sqlalchemy_safe',
-                'preserve_set'
-            }))
+            options=Options.parse_obj(self.options.dict(
+                include={
+                    'by_alias',
+                    'exclude_unset',
+                    'exclude_none',
+                    'exclude_defaults',
+                    'sqlalchemy_safe',
+                    'preserve_set'
+                })),
+            encoders=self.encoders
         )
 
         for key, value in obj.items():
             if (
                 (
                     not self.options.sqlalchemy_safe
                     or (not isinstance(key, str))
```

### Comparing `jsonablr-0.1.0/pyproject.toml` & `jsonablr-0.1.1/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [tool.poetry]
 authors = ["Bernard van Niekerk <bernard.van.niekerk@icloud.com>"]
 description = "Serialize Pydantic models and non-JSONable types into a JSONable variable."
 name = "jsonablr"
 readme = "README.md"
 repository = "https://github.com/frizzy/jsonablr.git"
-version = "0.1.0"
+version = "0.1.1"
 
 [tool.poetry.dependencies]
 pydantic = "^1.10"
 python = "^3.9"
 
 [tool.poetry.group.test]
 optional = true
```

### Comparing `jsonablr-0.1.0/PKG-INFO` & `jsonablr-0.1.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: jsonablr
-Version: 0.1.0
+Version: 0.1.1
 Summary: Serialize Pydantic models and non-JSONable types into a JSONable variable.
 Home-page: https://github.com/frizzy/jsonablr.git
 Author: Bernard van Niekerk
 Author-email: bernard.van.niekerk@icloud.com
 Requires-Python: >=3.9,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
```

