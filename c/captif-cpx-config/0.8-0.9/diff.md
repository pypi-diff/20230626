# Comparing `tmp/captif_cpx_config-0.8.tar.gz` & `tmp/captif_cpx_config-0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "captif_cpx_config-0.8.tar", max compression
+gzip compressed data, was "captif_cpx_config-0.9.tar", max compression
```

## Comparing `captif_cpx_config-0.8.tar` & `captif_cpx_config-0.9.tar`

### file list

```diff
@@ -1,6 +1,6 @@
--rw-r--r--   0        0        0     1084 2023-06-21 22:49:45.223392 captif_cpx_config-0.8/LICENSE
--rw-r--r--   0        0        0       19 2023-06-21 22:49:45.223392 captif_cpx_config-0.8/README.md
--rw-r--r--   0        0        0       44 2023-06-21 22:49:45.223392 captif_cpx_config-0.8/captif_cpx_config/__init__.py
--rw-r--r--   0        0        0     4185 2023-06-21 22:49:45.223392 captif_cpx_config-0.8/captif_cpx_config/metadata.py
--rw-r--r--   0        0        0      522 2023-06-21 22:49:45.223392 captif_cpx_config-0.8/pyproject.toml
--rw-r--r--   0        0        0      519 1970-01-01 00:00:00.000000 captif_cpx_config-0.8/PKG-INFO
+-rw-r--r--   0        0        0     1084 2023-06-23 02:06:00.030631 captif_cpx_config-0.9/LICENSE
+-rw-r--r--   0        0        0       19 2023-06-23 02:06:00.030631 captif_cpx_config-0.9/README.md
+-rw-r--r--   0        0        0       44 2023-06-23 02:06:00.030631 captif_cpx_config-0.9/captif_cpx_config/__init__.py
+-rw-r--r--   0        0        0     4335 2023-06-23 02:06:00.030631 captif_cpx_config-0.9/captif_cpx_config/metadata.py
+-rw-r--r--   0        0        0      523 2023-06-23 02:06:00.030631 captif_cpx_config-0.9/pyproject.toml
+-rw-r--r--   0        0        0      519 1970-01-01 00:00:00.000000 captif_cpx_config-0.9/PKG-INFO
```

### Comparing `captif_cpx_config-0.8/LICENSE` & `captif_cpx_config-0.9/LICENSE`

 * *Files identical despite different names*

### Comparing `captif_cpx_config-0.8/captif_cpx_config/metadata.py` & `captif_cpx_config-0.9/captif_cpx_config/metadata.py`

 * *Files 2% similar despite different names*

```diff
@@ -115,14 +115,18 @@
             "to convert the data back into volts."
         ),
     )
     notes: Optional[str] = Field(
         default=None,
         description="any additional notes",
     )
+    gis_check_complete: Optional[bool] = Field(
+        default=False,
+        description="tracks whether the manual GIS check has been done",
+    )
 
     wheel_bay_details: list["WheelBayDetails"] = []
 
     def write(self, path: str):
         with open(path, "w") as f:
             f.write(self.json(indent=4))
```

### Comparing `captif_cpx_config-0.8/pyproject.toml` & `captif_cpx_config-0.9/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "captif-cpx-config"
-version = "0.8"
+version = "0.9"
 description = ""
 authors = ["John Bull <john.bull@nzta.govt.nz>"]
 license = "MIT"
 readme = "README.md"
 packages = [{include = "captif_cpx_config"}]
 
 [tool.poetry.dependencies]
@@ -14,12 +14,12 @@
 
 [tool.poetry.group.dev.dependencies]
 pytest = "^7.3.1"
 pytest-cov = "^4.1.0"
 pytest-randomly = "^3.12.0"
 black = "^23.3.0"
 flake8 = "^6.0.0"
-captif-cpx-db = ">=0.8"
+captif-cpx-db = ">=0.10"
 
 [build-system]
 requires = ["poetry-core"]
 build-backend = "poetry.core.masonry.api"
```

### Comparing `captif_cpx_config-0.8/PKG-INFO` & `captif_cpx_config-0.9/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: captif-cpx-config
-Version: 0.8
+Version: 0.9
 Summary: 
 License: MIT
 Author: John Bull
 Author-email: john.bull@nzta.govt.nz
 Requires-Python: >=3.9,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
```

