# Comparing `tmp/playmolecule-1.9.0.tar.gz` & `tmp/playmolecule-1.9.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "playmolecule-1.9.0.tar", last modified: Fri Jun  2 08:58:06 2023, max compression
+gzip compressed data, was "playmolecule-1.9.1.tar", last modified: Mon Jun 26 12:57:27 2023, max compression
```

## Comparing `playmolecule-1.9.0.tar` & `playmolecule-1.9.1.tar`

### file list

```diff
@@ -1,34 +1,34 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 08:58:06.371062 playmolecule-1.9.0/
--rw-r--r--   0 runner    (1001) docker     (123)     2852 2023-06-02 08:57:38.000000 playmolecule-1.9.0/LICENSE.md
--rw-r--r--   0 runner    (1001) docker     (123)       93 2023-06-02 08:57:38.000000 playmolecule-1.9.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)      666 2023-06-02 08:58:06.371062 playmolecule-1.9.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      189 2023-06-02 08:57:38.000000 playmolecule-1.9.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 08:58:06.371062 playmolecule-1.9.0/playmolecule/
--rw-r--r--   0 runner    (1001) docker     (123)      870 2023-06-02 08:57:38.000000 playmolecule-1.9.0/playmolecule/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      744 2023-06-02 08:57:38.000000 playmolecule-1.9.0/playmolecule/_test_funcs.py
--rw-r--r--   0 runner    (1001) docker     (123)      497 2023-06-02 08:58:06.371062 playmolecule-1.9.0/playmolecule/_version.py
--rw-r--r--   0 runner    (1001) docker     (123)       87 2023-06-02 08:57:38.000000 playmolecule-1.9.0/playmolecule/config.ini
--rw-r--r--   0 runner    (1001) docker     (123)      711 2023-06-02 08:57:38.000000 playmolecule-1.9.0/playmolecule/config.py
--rw-r--r--   0 runner    (1001) docker     (123)    24631 2023-06-02 08:57:38.000000 playmolecule-1.9.0/playmolecule/datacenter.py
--rw-r--r--   0 runner    (1001) docker     (123)    33556 2023-06-02 08:57:38.000000 playmolecule-1.9.0/playmolecule/devutils.py
--rw-r--r--   0 runner    (1001) docker     (123)    32171 2023-06-02 08:57:38.000000 playmolecule-1.9.0/playmolecule/job.py
--rw-r--r--   0 runner    (1001) docker     (123)     9766 2023-06-02 08:57:38.000000 playmolecule-1.9.0/playmolecule/jsonlogger.py
--rw-r--r--   0 runner    (1001) docker     (123)     6392 2023-06-02 08:57:38.000000 playmolecule-1.9.0/playmolecule/local.py
--rw-r--r--   0 runner    (1001) docker     (123)      431 2023-06-02 08:57:38.000000 playmolecule-1.9.0/playmolecule/logging.ini
--rw-r--r--   0 runner    (1001) docker     (123)     3797 2023-06-02 08:57:38.000000 playmolecule-1.9.0/playmolecule/playqueue.py
--rw-r--r--   0 runner    (1001) docker     (123)    33414 2023-06-02 08:57:38.000000 playmolecule-1.9.0/playmolecule/session.py
--rw-r--r--   0 runner    (1001) docker     (123)     3707 2023-06-02 08:57:38.000000 playmolecule-1.9.0/playmolecule/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 08:58:06.371062 playmolecule-1.9.0/playmolecule.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      666 2023-06-02 08:58:06.000000 playmolecule-1.9.0/playmolecule.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      678 2023-06-02 08:58:06.000000 playmolecule-1.9.0/playmolecule.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-02 08:58:06.000000 playmolecule-1.9.0/playmolecule.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-02 08:58:06.000000 playmolecule-1.9.0/playmolecule.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       64 2023-06-02 08:58:06.000000 playmolecule-1.9.0/playmolecule.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       13 2023-06-02 08:58:06.000000 playmolecule-1.9.0/playmolecule.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      983 2023-06-02 08:57:38.000000 playmolecule-1.9.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-02 08:58:06.371062 playmolecule-1.9.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      155 2023-06-02 08:57:38.000000 playmolecule-1.9.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 08:58:06.371062 playmolecule-1.9.0/tests/
--rw-r--r--   0 runner    (1001) docker     (123)     1601 2023-06-02 08:57:38.000000 playmolecule-1.9.0/tests/test.py
--rw-r--r--   0 runner    (1001) docker     (123)     4665 2023-06-02 08:57:38.000000 playmolecule-1.9.0/tests/test_app_wrapper.py
--rw-r--r--   0 runner    (1001) docker     (123)     4083 2023-06-02 08:57:38.000000 playmolecule-1.9.0/tests/test_datacenter.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 12:57:27.920272 playmolecule-1.9.1/
+-rw-r--r--   0 runner    (1001) docker     (123)     2852 2023-06-26 12:57:01.000000 playmolecule-1.9.1/LICENSE.md
+-rw-r--r--   0 runner    (1001) docker     (123)       93 2023-06-26 12:57:01.000000 playmolecule-1.9.1/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)      666 2023-06-26 12:57:27.920272 playmolecule-1.9.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      189 2023-06-26 12:57:01.000000 playmolecule-1.9.1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 12:57:27.920272 playmolecule-1.9.1/playmolecule/
+-rw-r--r--   0 runner    (1001) docker     (123)      870 2023-06-26 12:57:01.000000 playmolecule-1.9.1/playmolecule/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      744 2023-06-26 12:57:01.000000 playmolecule-1.9.1/playmolecule/_test_funcs.py
+-rw-r--r--   0 runner    (1001) docker     (123)      497 2023-06-26 12:57:27.920272 playmolecule-1.9.1/playmolecule/_version.py
+-rw-r--r--   0 runner    (1001) docker     (123)       87 2023-06-26 12:57:01.000000 playmolecule-1.9.1/playmolecule/config.ini
+-rw-r--r--   0 runner    (1001) docker     (123)      711 2023-06-26 12:57:01.000000 playmolecule-1.9.1/playmolecule/config.py
+-rw-r--r--   0 runner    (1001) docker     (123)    24631 2023-06-26 12:57:01.000000 playmolecule-1.9.1/playmolecule/datacenter.py
+-rw-r--r--   0 runner    (1001) docker     (123)    33556 2023-06-26 12:57:01.000000 playmolecule-1.9.1/playmolecule/devutils.py
+-rw-r--r--   0 runner    (1001) docker     (123)    32370 2023-06-26 12:57:01.000000 playmolecule-1.9.1/playmolecule/job.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9766 2023-06-26 12:57:01.000000 playmolecule-1.9.1/playmolecule/jsonlogger.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6392 2023-06-26 12:57:01.000000 playmolecule-1.9.1/playmolecule/local.py
+-rw-r--r--   0 runner    (1001) docker     (123)      431 2023-06-26 12:57:01.000000 playmolecule-1.9.1/playmolecule/logging.ini
+-rw-r--r--   0 runner    (1001) docker     (123)     3797 2023-06-26 12:57:01.000000 playmolecule-1.9.1/playmolecule/playqueue.py
+-rw-r--r--   0 runner    (1001) docker     (123)    33414 2023-06-26 12:57:01.000000 playmolecule-1.9.1/playmolecule/session.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3707 2023-06-26 12:57:01.000000 playmolecule-1.9.1/playmolecule/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 12:57:27.920272 playmolecule-1.9.1/playmolecule.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      666 2023-06-26 12:57:27.000000 playmolecule-1.9.1/playmolecule.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      678 2023-06-26 12:57:27.000000 playmolecule-1.9.1/playmolecule.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-26 12:57:27.000000 playmolecule-1.9.1/playmolecule.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-26 12:57:27.000000 playmolecule-1.9.1/playmolecule.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       64 2023-06-26 12:57:27.000000 playmolecule-1.9.1/playmolecule.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       13 2023-06-26 12:57:27.000000 playmolecule-1.9.1/playmolecule.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      983 2023-06-26 12:57:01.000000 playmolecule-1.9.1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-26 12:57:27.920272 playmolecule-1.9.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      155 2023-06-26 12:57:01.000000 playmolecule-1.9.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 12:57:27.920272 playmolecule-1.9.1/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     1601 2023-06-26 12:57:01.000000 playmolecule-1.9.1/tests/test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4665 2023-06-26 12:57:01.000000 playmolecule-1.9.1/tests/test_app_wrapper.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4083 2023-06-26 12:57:01.000000 playmolecule-1.9.1/tests/test_datacenter.py
```

### Comparing `playmolecule-1.9.0/LICENSE.md` & `playmolecule-1.9.1/LICENSE.md`

 * *Files identical despite different names*

### Comparing `playmolecule-1.9.0/PKG-INFO` & `playmolecule-1.9.1/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: playmolecule
-Version: 1.9.0
+Version: 1.9.1
 Summary: PlayMolecule python API
 Author-email: Acellera <info@acellera.com>
 Project-URL: Homepage, https://github.com/Acellera/playmolecule-python-api
 Project-URL: Bug Tracker, https://github.com/Acellera/playmolecule-python-api/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: POSIX :: Linux
 Requires-Python: >=3.8
```

### Comparing `playmolecule-1.9.0/playmolecule/__init__.py` & `playmolecule-1.9.1/playmolecule/__init__.py`

 * *Files identical despite different names*

### Comparing `playmolecule-1.9.0/playmolecule/_test_funcs.py` & `playmolecule-1.9.1/playmolecule/_test_funcs.py`

 * *Files identical despite different names*

### Comparing `playmolecule-1.9.0/playmolecule/config.py` & `playmolecule-1.9.1/playmolecule/config.py`

 * *Files identical despite different names*

### Comparing `playmolecule-1.9.0/playmolecule/datacenter.py` & `playmolecule-1.9.1/playmolecule/datacenter.py`

 * *Files identical despite different names*

### Comparing `playmolecule-1.9.0/playmolecule/devutils.py` & `playmolecule-1.9.1/playmolecule/devutils.py`

 * *Files identical despite different names*

### Comparing `playmolecule-1.9.0/playmolecule/job.py` & `playmolecule-1.9.1/playmolecule/job.py`

 * *Files 1% similar despite different names*

```diff
@@ -310,14 +310,15 @@
             "params": [],
         }
         if pm_options is not None:
             if not isinstance(pm_options, dict):
                 raise RuntimeError("pm_options only accepts dict arguments")
             out_config["pm_options"] = pm_options
 
+        sources = {}
         for param in self._params:
             name = param["name"]
             value = getattr(self, name)
             datatype = self._commands[name]["datatype"]
 
             newvals = []
             for val in ensurelist(value):
@@ -344,22 +345,23 @@
                             _throwError(
                                 f"File or folder does not exist: {val}", _logger
                             )
                             return
                     else:
                         filename = os.path.basename(os.path.normpath(val))
                         dest = os.path.join(inputpath, filename)
-                        if os.path.exists(dest):
-                            raise AssertionError(
-                                f"File {dest} already exists. Cannot overwrite"
-                            )
-                        if os.path.isfile(val):
-                            shutil.copy(val, os.path.join(inputpath, filename))
-                        else:
-                            shutil.copytree(val, os.path.join(inputpath, filename))
+                        if dest in sources and sources[dest] != os.path.normpath(val):
+                            raise RuntimeError(f"Two different files have the same name {sources['dest']} vs {val}. Please rename one of them.")
+                        
+                        if dest not in sources:
+                            if os.path.isfile(val):
+                                shutil.copy(val, os.path.join(inputpath, filename))
+                            else:
+                                shutil.copytree(val, os.path.join(inputpath, filename))
+                            sources[dest] = os.path.normpath(val)
                 else:
                     if type(val) == bool and isinstance(param["value"], str):
                         # TODO: Deprecate this once all apps have generated new style manifests
                         val = str(val)
                 newvals.append(val)
 
             out_config["params"].append(
```

### Comparing `playmolecule-1.9.0/playmolecule/jsonlogger.py` & `playmolecule-1.9.1/playmolecule/jsonlogger.py`

 * *Files identical despite different names*

### Comparing `playmolecule-1.9.0/playmolecule/local.py` & `playmolecule-1.9.1/playmolecule/local.py`

 * *Files identical despite different names*

### Comparing `playmolecule-1.9.0/playmolecule/playqueue.py` & `playmolecule-1.9.1/playmolecule/playqueue.py`

 * *Files identical despite different names*

### Comparing `playmolecule-1.9.0/playmolecule/session.py` & `playmolecule-1.9.1/playmolecule/session.py`

 * *Files identical despite different names*

### Comparing `playmolecule-1.9.0/playmolecule/utils.py` & `playmolecule-1.9.1/playmolecule/utils.py`

 * *Files identical despite different names*

### Comparing `playmolecule-1.9.0/playmolecule.egg-info/PKG-INFO` & `playmolecule-1.9.1/playmolecule.egg-info/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: playmolecule
-Version: 1.9.0
+Version: 1.9.1
 Summary: PlayMolecule python API
 Author-email: Acellera <info@acellera.com>
 Project-URL: Homepage, https://github.com/Acellera/playmolecule-python-api
 Project-URL: Bug Tracker, https://github.com/Acellera/playmolecule-python-api/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: POSIX :: Linux
 Requires-Python: >=3.8
```

### Comparing `playmolecule-1.9.0/playmolecule.egg-info/SOURCES.txt` & `playmolecule-1.9.1/playmolecule.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `playmolecule-1.9.0/pyproject.toml` & `playmolecule-1.9.1/pyproject.toml`

 * *Files identical despite different names*

### Comparing `playmolecule-1.9.0/tests/test.py` & `playmolecule-1.9.1/tests/test.py`

 * *Files identical despite different names*

### Comparing `playmolecule-1.9.0/tests/test_app_wrapper.py` & `playmolecule-1.9.1/tests/test_app_wrapper.py`

 * *Files identical despite different names*

### Comparing `playmolecule-1.9.0/tests/test_datacenter.py` & `playmolecule-1.9.1/tests/test_datacenter.py`

 * *Files identical despite different names*

