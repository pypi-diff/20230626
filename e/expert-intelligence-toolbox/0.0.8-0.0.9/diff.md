# Comparing `tmp/expert_intelligence_toolbox-0.0.8.tar.gz` & `tmp/expert_intelligence_toolbox-0.0.9.tar.gz`

## Comparing `expert_intelligence_toolbox-0.0.8.tar` & `expert_intelligence_toolbox-0.0.9.tar`

### file list

```diff
@@ -1,11 +1,11 @@
--rw-r--r--   0        0        0     3285 2020-02-02 00:00:00.000000 expert_intelligence_toolbox-0.0.8/instructions.md
--rw-r--r--   0        0        0      174 2020-02-02 00:00:00.000000 expert_intelligence_toolbox-0.0.8/requirements.txt
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 expert_intelligence_toolbox-0.0.8/src/expert_intelligence_toolbox/__init__.py
--rw-r--r--   0        0        0       64 2020-02-02 00:00:00.000000 expert_intelligence_toolbox-0.0.8/src/expert_intelligence_toolbox/example.py
--rw-r--r--   0        0        0     7319 2020-02-02 00:00:00.000000 expert_intelligence_toolbox-0.0.8/src/expert_intelligence_toolbox/geographic.py
--rw-r--r--   0        0        0     2625 2020-02-02 00:00:00.000000 expert_intelligence_toolbox-0.0.8/src/expert_intelligence_toolbox/snowflake_connector.py
--rw-r--r--   0        0        0       20 2020-02-02 00:00:00.000000 expert_intelligence_toolbox-0.0.8/.gitignore
--rw-r--r--   0        0        0     1068 2020-02-02 00:00:00.000000 expert_intelligence_toolbox-0.0.8/LICENSE
--rw-r--r--   0        0        0      372 2020-02-02 00:00:00.000000 expert_intelligence_toolbox-0.0.8/README.md
--rw-r--r--   0        0        0      718 2020-02-02 00:00:00.000000 expert_intelligence_toolbox-0.0.8/pyproject.toml
--rw-r--r--   0        0        0     1010 2020-02-02 00:00:00.000000 expert_intelligence_toolbox-0.0.8/PKG-INFO
+-rw-r--r--   0        0        0     3285 2020-02-02 00:00:00.000000 expert_intelligence_toolbox-0.0.9/instructions.md
+-rw-r--r--   0        0        0      185 2020-02-02 00:00:00.000000 expert_intelligence_toolbox-0.0.9/requirements.txt
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 expert_intelligence_toolbox-0.0.9/src/expert_intelligence_toolbox/__init__.py
+-rw-r--r--   0        0        0       64 2020-02-02 00:00:00.000000 expert_intelligence_toolbox-0.0.9/src/expert_intelligence_toolbox/example.py
+-rw-r--r--   0        0        0    11962 2020-02-02 00:00:00.000000 expert_intelligence_toolbox-0.0.9/src/expert_intelligence_toolbox/geographic.py
+-rw-r--r--   0        0        0     2625 2020-02-02 00:00:00.000000 expert_intelligence_toolbox-0.0.9/src/expert_intelligence_toolbox/snowflake_connector.py
+-rw-r--r--   0        0        0       20 2020-02-02 00:00:00.000000 expert_intelligence_toolbox-0.0.9/.gitignore
+-rw-r--r--   0        0        0     1068 2020-02-02 00:00:00.000000 expert_intelligence_toolbox-0.0.9/LICENSE
+-rw-r--r--   0        0        0      372 2020-02-02 00:00:00.000000 expert_intelligence_toolbox-0.0.9/README.md
+-rw-r--r--   0        0        0      718 2020-02-02 00:00:00.000000 expert_intelligence_toolbox-0.0.9/pyproject.toml
+-rw-r--r--   0        0        0     1010 2020-02-02 00:00:00.000000 expert_intelligence_toolbox-0.0.9/PKG-INFO
```

### Comparing `expert_intelligence_toolbox-0.0.8/instructions.md` & `expert_intelligence_toolbox-0.0.9/instructions.md`

 * *Files identical despite different names*

### Comparing `expert_intelligence_toolbox-0.0.8/src/expert_intelligence_toolbox/snowflake_connector.py` & `expert_intelligence_toolbox-0.0.9/src/expert_intelligence_toolbox/snowflake_connector.py`

 * *Files identical despite different names*

### Comparing `expert_intelligence_toolbox-0.0.8/LICENSE` & `expert_intelligence_toolbox-0.0.9/LICENSE`

 * *Files identical despite different names*

### Comparing `expert_intelligence_toolbox-0.0.8/pyproject.toml` & `expert_intelligence_toolbox-0.0.9/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["hatchling"]
 build-backend = "hatchling.build"
 
 [project]
 name = "expert_intelligence_toolbox"
-version = "0.0.8"
+version = "0.0.9"
 authors = [
   { name="Arnold Kuersteiner", email="arnold.kuersteiner@expert-intelligence.com" },
   { name="Pham Minh Ky", email="ky.pham@expert-intelligence.com" },
 ]
 description = "This is (for now) a test."
 readme = "README.md"
 requires-python = ">=3.7"
```

### Comparing `expert_intelligence_toolbox-0.0.8/PKG-INFO` & `expert_intelligence_toolbox-0.0.9/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: expert_intelligence_toolbox
-Version: 0.0.8
+Version: 0.0.9
 Summary: This is (for now) a test.
 Project-URL: Homepage, https://github.com/Point-Topic/expert_intelligence_toolbox
 Project-URL: Bug Tracker, https://github.com/Point-Topic/expert_intelligence_toolbox/issues
 Author-email: Arnold Kuersteiner <arnold.kuersteiner@expert-intelligence.com>, Pham Minh Ky <ky.pham@expert-intelligence.com>
 License-File: LICENSE
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

