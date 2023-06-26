# Comparing `tmp/pypomes-0.1.7.tar.gz` & `tmp/pypomes-0.1.8.tar.gz`

## Comparing `pypomes-0.1.7.tar` & `pypomes-0.1.8.tar`

### file list

```diff
@@ -1,23 +1,23 @@
--rw-r--r--   0        0        0      360 2020-02-02 00:00:00.000000 pypomes-0.1.7/requirements.txt
--rw-r--r--   0        0        0     4209 2020-02-02 00:00:00.000000 pypomes-0.1.7/src/pypomes/__init__.py
--rw-r--r--   0        0        0     7707 2020-02-02 00:00:00.000000 pypomes-0.1.7/src/pypomes/azure_pomes.py
--rw-r--r--   0        0        0     1402 2020-02-02 00:00:00.000000 pypomes-0.1.7/src/pypomes/crypto_pomes.py
--rw-r--r--   0        0        0     2314 2020-02-02 00:00:00.000000 pypomes-0.1.7/src/pypomes/datetime_pomes.py
--rw-r--r--   0        0        0    12079 2020-02-02 00:00:00.000000 pypomes-0.1.7/src/pypomes/db_pomes.py
--rw-r--r--   0        0        0    27585 2020-02-02 00:00:00.000000 pypomes-0.1.7/src/pypomes/dict_pomes.py
--rw-r--r--   0        0        0     4503 2020-02-02 00:00:00.000000 pypomes-0.1.7/src/pypomes/encoding_pomes.py
--rw-r--r--   0        0        0     2109 2020-02-02 00:00:00.000000 pypomes-0.1.7/src/pypomes/env_pomes.py
--rw-r--r--   0        0        0     1098 2020-02-02 00:00:00.000000 pypomes-0.1.7/src/pypomes/exception_pomes.py
--rw-r--r--   0        0        0      770 2020-02-02 00:00:00.000000 pypomes-0.1.7/src/pypomes/file_pomes.py
--rw-r--r--   0        0        0     1912 2020-02-02 00:00:00.000000 pypomes-0.1.7/src/pypomes/json_pomes.py
--rw-r--r--   0        0        0     6257 2020-02-02 00:00:00.000000 pypomes-0.1.7/src/pypomes/list_pomes.py
--rw-r--r--   0        0        0     4882 2020-02-02 00:00:00.000000 pypomes-0.1.7/src/pypomes/logging_pomes.py
--rw-r--r--   0        0        0    10498 2020-02-02 00:00:00.000000 pypomes-0.1.7/src/pypomes/minio_pomes.py
--rw-r--r--   0        0        0     7454 2020-02-02 00:00:00.000000 pypomes-0.1.7/src/pypomes/soap_pomes.py
--rw-r--r--   0        0        0     2026 2020-02-02 00:00:00.000000 pypomes-0.1.7/src/pypomes/str_pomes.py
--rw-r--r--   0        0        0     2564 2020-02-02 00:00:00.000000 pypomes-0.1.7/src/pypomes/xml_pomes.py
--rw-r--r--   0        0        0       85 2020-02-02 00:00:00.000000 pypomes-0.1.7/.gitignore
--rw-r--r--   0        0        0     1086 2020-02-02 00:00:00.000000 pypomes-0.1.7/LICENSE
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 pypomes-0.1.7/README.md
--rw-r--r--   0        0        0     1102 2020-02-02 00:00:00.000000 pypomes-0.1.7/pyproject.toml
--rw-r--r--   0        0        0      475 2020-02-02 00:00:00.000000 pypomes-0.1.7/PKG-INFO
+-rw-r--r--   0        0        0      360 2020-02-02 00:00:00.000000 pypomes-0.1.8/requirements.txt
+-rw-r--r--   0        0        0     4209 2020-02-02 00:00:00.000000 pypomes-0.1.8/src/pypomes/__init__.py
+-rw-r--r--   0        0        0     7707 2020-02-02 00:00:00.000000 pypomes-0.1.8/src/pypomes/azure_pomes.py
+-rw-r--r--   0        0        0     1402 2020-02-02 00:00:00.000000 pypomes-0.1.8/src/pypomes/crypto_pomes.py
+-rw-r--r--   0        0        0     2314 2020-02-02 00:00:00.000000 pypomes-0.1.8/src/pypomes/datetime_pomes.py
+-rw-r--r--   0        0        0    12079 2020-02-02 00:00:00.000000 pypomes-0.1.8/src/pypomes/db_pomes.py
+-rw-r--r--   0        0        0    27585 2020-02-02 00:00:00.000000 pypomes-0.1.8/src/pypomes/dict_pomes.py
+-rw-r--r--   0        0        0     4503 2020-02-02 00:00:00.000000 pypomes-0.1.8/src/pypomes/encoding_pomes.py
+-rw-r--r--   0        0        0     2125 2020-02-02 00:00:00.000000 pypomes-0.1.8/src/pypomes/env_pomes.py
+-rw-r--r--   0        0        0     1098 2020-02-02 00:00:00.000000 pypomes-0.1.8/src/pypomes/exception_pomes.py
+-rw-r--r--   0        0        0      770 2020-02-02 00:00:00.000000 pypomes-0.1.8/src/pypomes/file_pomes.py
+-rw-r--r--   0        0        0     1912 2020-02-02 00:00:00.000000 pypomes-0.1.8/src/pypomes/json_pomes.py
+-rw-r--r--   0        0        0     6257 2020-02-02 00:00:00.000000 pypomes-0.1.8/src/pypomes/list_pomes.py
+-rw-r--r--   0        0        0     4882 2020-02-02 00:00:00.000000 pypomes-0.1.8/src/pypomes/logging_pomes.py
+-rw-r--r--   0        0        0    10498 2020-02-02 00:00:00.000000 pypomes-0.1.8/src/pypomes/minio_pomes.py
+-rw-r--r--   0        0        0     7454 2020-02-02 00:00:00.000000 pypomes-0.1.8/src/pypomes/soap_pomes.py
+-rw-r--r--   0        0        0     2026 2020-02-02 00:00:00.000000 pypomes-0.1.8/src/pypomes/str_pomes.py
+-rw-r--r--   0        0        0     2564 2020-02-02 00:00:00.000000 pypomes-0.1.8/src/pypomes/xml_pomes.py
+-rw-r--r--   0        0        0       85 2020-02-02 00:00:00.000000 pypomes-0.1.8/.gitignore
+-rw-r--r--   0        0        0     1086 2020-02-02 00:00:00.000000 pypomes-0.1.8/LICENSE
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 pypomes-0.1.8/README.md
+-rw-r--r--   0        0        0     1102 2020-02-02 00:00:00.000000 pypomes-0.1.8/pyproject.toml
+-rw-r--r--   0        0        0      475 2020-02-02 00:00:00.000000 pypomes-0.1.8/PKG-INFO
```

### Comparing `pypomes-0.1.7/src/pypomes/__init__.py` & `pypomes-0.1.8/src/pypomes/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -100,9 +100,9 @@
     soap_post, soap_post_zeep, soap_get_attachment, soap_get_dict, soap_get_cids, soap_build_envelope,
     # str_pomes
     str_between, str_split_on_mark, str_find_whitespace,
     # xml_pomes
     xml_to_dict, xml_normalize_keys
 ]
 
-__version__ = "0.1.7"
-__version_info__ = (0, 1, 7)
+__version__ = "0.1.8"
+__version_info__ = (0, 1, 8)
```

### Comparing `pypomes-0.1.7/src/pypomes/azure_pomes.py` & `pypomes-0.1.8/src/pypomes/azure_pomes.py`

 * *Files identical despite different names*

### Comparing `pypomes-0.1.7/src/pypomes/crypto_pomes.py` & `pypomes-0.1.8/src/pypomes/crypto_pomes.py`

 * *Files identical despite different names*

### Comparing `pypomes-0.1.7/src/pypomes/datetime_pomes.py` & `pypomes-0.1.8/src/pypomes/datetime_pomes.py`

 * *Files identical despite different names*

### Comparing `pypomes-0.1.7/src/pypomes/db_pomes.py` & `pypomes-0.1.8/src/pypomes/db_pomes.py`

 * *Files identical despite different names*

### Comparing `pypomes-0.1.7/src/pypomes/dict_pomes.py` & `pypomes-0.1.8/src/pypomes/dict_pomes.py`

 * *Files identical despite different names*

### Comparing `pypomes-0.1.7/src/pypomes/encoding_pomes.py` & `pypomes-0.1.8/src/pypomes/encoding_pomes.py`

 * *Files identical despite different names*

### Comparing `pypomes-0.1.7/src/pypomes/env_pomes.py` & `pypomes-0.1.8/src/pypomes/env_pomes.py`

 * *Files 17% similar despite different names*

```diff
@@ -8,15 +8,15 @@
     :param key: The key the value is associated with.
     :param def_value: The default value to return, if the key has not been defined.
     :return: The int value associated with the key.
     """
     result: str
     try:
         result = os.environ[key]
-    except KeyError:
+    except (KeyError, TypeError):
         result = def_value
 
     return result
 
 
 def env_get_bool(key: str, def_value: bool = None) -> bool:
     """
@@ -25,15 +25,15 @@
     :param key: The key the value is associated with.
     :param def_value: The default value to return, if the key has not been defined.
     :return: The boolean value associated with the key.
     """
     result: bool
     try:
         result = bool(os.environ[key])
-    except KeyError | TypeError:
+    except (KeyError, TypeError):
         result = def_value
 
     return result
 
 
 def env_get_int(key: str, def_value: int = None) -> int:
     """
@@ -42,15 +42,15 @@
     :param key: The key the value is associated with.
     :param def_value: The default value to return, if the key has not been defined.
     :return: The int value associated with the key.
     """
     result: int
     try:
         result = int(os.environ[key])
-    except KeyError | TypeError:
+    except (KeyError, TypeError):
         result = def_value
 
     return result
 
 
 def env_get_float(key: str, def_value: float = None) -> float:
     """
@@ -59,14 +59,14 @@
     :param key: The key the value is associated with.
     :param def_value: The default value to return, if the key has not been defined.
     :return: The float value associated with the key.
     """
     result: float
     try:
         result = int(os.environ[key])
-    except KeyError | TypeError:
+    except (KeyError, TypeError):
         result = def_value
 
     return result
 
 
 APP_PREFIX = env_get_str("PYPOMES_APP_PREFIX", "PYPOMES")
```

### Comparing `pypomes-0.1.7/src/pypomes/exception_pomes.py` & `pypomes-0.1.8/src/pypomes/exception_pomes.py`

 * *Files identical despite different names*

### Comparing `pypomes-0.1.7/src/pypomes/file_pomes.py` & `pypomes-0.1.8/src/pypomes/file_pomes.py`

 * *Files identical despite different names*

### Comparing `pypomes-0.1.7/src/pypomes/json_pomes.py` & `pypomes-0.1.8/src/pypomes/json_pomes.py`

 * *Files identical despite different names*

### Comparing `pypomes-0.1.7/src/pypomes/list_pomes.py` & `pypomes-0.1.8/src/pypomes/list_pomes.py`

 * *Files identical despite different names*

### Comparing `pypomes-0.1.7/src/pypomes/logging_pomes.py` & `pypomes-0.1.8/src/pypomes/logging_pomes.py`

 * *Files identical despite different names*

### Comparing `pypomes-0.1.7/src/pypomes/minio_pomes.py` & `pypomes-0.1.8/src/pypomes/minio_pomes.py`

 * *Files identical despite different names*

### Comparing `pypomes-0.1.7/src/pypomes/soap_pomes.py` & `pypomes-0.1.8/src/pypomes/soap_pomes.py`

 * *Files identical despite different names*

### Comparing `pypomes-0.1.7/src/pypomes/str_pomes.py` & `pypomes-0.1.8/src/pypomes/str_pomes.py`

 * *Files identical despite different names*

### Comparing `pypomes-0.1.7/src/pypomes/xml_pomes.py` & `pypomes-0.1.8/src/pypomes/xml_pomes.py`

 * *Files identical despite different names*

### Comparing `pypomes-0.1.7/LICENSE` & `pypomes-0.1.8/LICENSE`

 * *Files identical despite different names*

### Comparing `pypomes-0.1.7/pyproject.toml` & `pypomes-0.1.8/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -21,15 +21,15 @@
     "xmltodict3>=0.0.4",
     "zeep>=4.2.1"
 ]
 build-backend = "hatchling.build"
 
 [project]
 name = "pypomes"
-version = "0.1.7"
+version = "0.1.8"
 authors = [
   { name="GT Nunes", email="wisecoder01@gmail.com" },
 ]
 description = "A collection of Python pomes, pennyeach"
 readme = "README.md"
 requires-python = ">=3.10"
 classifiers = [
```

