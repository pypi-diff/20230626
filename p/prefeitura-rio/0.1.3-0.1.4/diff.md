# Comparing `tmp/prefeitura_rio-0.1.3.tar.gz` & `tmp/prefeitura_rio-0.1.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "prefeitura_rio-0.1.3.tar", max compression
+gzip compressed data, was "prefeitura_rio-0.1.4.tar", max compression
```

## Comparing `prefeitura_rio-0.1.3.tar` & `prefeitura_rio-0.1.4.tar`

### file list

```diff
@@ -1,13 +1,13 @@
--rw-r--r--   0        0        0    35149 2023-06-21 17:11:48.819069 prefeitura_rio-0.1.3/LICENSE
--rw-r--r--   0        0        0       83 2023-06-21 17:11:48.819069 prefeitura_rio-0.1.3/README.md
--rw-r--r--   0        0        0      124 2023-06-21 17:11:48.819069 prefeitura_rio-0.1.3/prefeitura_rio/__init__.py
--rw-r--r--   0        0        0     2397 2023-06-21 17:11:48.819069 prefeitura_rio-0.1.3/prefeitura_rio/core.py
--rw-r--r--   0        0        0        0 2023-06-21 17:11:48.819069 prefeitura_rio-0.1.3/prefeitura_rio/integrations/__init__.py
--rw-r--r--   0        0        0    18392 2023-06-21 17:11:48.819069 prefeitura_rio-0.1.3/prefeitura_rio/integrations/sgrc/__init__.py
--rw-r--r--   0        0        0      455 2023-06-21 17:11:48.819069 prefeitura_rio-0.1.3/prefeitura_rio/integrations/sgrc/exceptions.py
--rw-r--r--   0        0        0    11646 2023-06-21 17:11:48.819069 prefeitura_rio-0.1.3/prefeitura_rio/integrations/sgrc/models.py
--rw-r--r--   0        0        0     2082 2023-06-21 17:11:48.819069 prefeitura_rio-0.1.3/prefeitura_rio/integrations/sgrc/utils.py
--rw-r--r--   0        0        0     1749 2023-06-21 17:11:48.819069 prefeitura_rio-0.1.3/prefeitura_rio/metrics/__init__.py
--rw-r--r--   0        0        0     7642 2023-06-21 17:11:48.819069 prefeitura_rio-0.1.3/prefeitura_rio/metrics/agnostic.py
--rw-r--r--   0        0        0      958 2023-06-21 17:11:48.819069 prefeitura_rio-0.1.3/pyproject.toml
--rw-r--r--   0        0        0     1019 1970-01-01 00:00:00.000000 prefeitura_rio-0.1.3/PKG-INFO
+-rw-r--r--   0        0        0    35149 2023-06-26 18:55:31.592541 prefeitura_rio-0.1.4/LICENSE
+-rw-r--r--   0        0        0       83 2023-06-26 18:55:31.592541 prefeitura_rio-0.1.4/README.md
+-rw-r--r--   0        0        0      124 2023-06-26 18:55:31.592541 prefeitura_rio-0.1.4/prefeitura_rio/__init__.py
+-rw-r--r--   0        0        0     2397 2023-06-26 18:55:31.592541 prefeitura_rio-0.1.4/prefeitura_rio/core.py
+-rw-r--r--   0        0        0        0 2023-06-26 18:55:31.592541 prefeitura_rio-0.1.4/prefeitura_rio/integrations/__init__.py
+-rw-r--r--   0        0        0    18356 2023-06-26 18:55:31.592541 prefeitura_rio-0.1.4/prefeitura_rio/integrations/sgrc/__init__.py
+-rw-r--r--   0        0        0      455 2023-06-26 18:55:31.592541 prefeitura_rio-0.1.4/prefeitura_rio/integrations/sgrc/exceptions.py
+-rw-r--r--   0        0        0    11646 2023-06-26 18:55:31.592541 prefeitura_rio-0.1.4/prefeitura_rio/integrations/sgrc/models.py
+-rw-r--r--   0        0        0     2082 2023-06-26 18:55:31.592541 prefeitura_rio-0.1.4/prefeitura_rio/integrations/sgrc/utils.py
+-rw-r--r--   0        0        0     1749 2023-06-26 18:55:31.592541 prefeitura_rio-0.1.4/prefeitura_rio/metrics/__init__.py
+-rw-r--r--   0        0        0     7642 2023-06-26 18:55:31.592541 prefeitura_rio-0.1.4/prefeitura_rio/metrics/agnostic.py
+-rw-r--r--   0        0        0      958 2023-06-26 18:55:31.592541 prefeitura_rio-0.1.4/pyproject.toml
+-rw-r--r--   0        0        0     1019 1970-01-01 00:00:00.000000 prefeitura_rio-0.1.4/PKG-INFO
```

### Comparing `prefeitura_rio-0.1.3/LICENSE` & `prefeitura_rio-0.1.4/LICENSE`

 * *Files identical despite different names*

### Comparing `prefeitura_rio-0.1.3/prefeitura_rio/core.py` & `prefeitura_rio-0.1.4/prefeitura_rio/core.py`

 * *Files identical despite different names*

### Comparing `prefeitura_rio-0.1.3/prefeitura_rio/integrations/sgrc/__init__.py` & `prefeitura_rio-0.1.4/prefeitura_rio/integrations/sgrc/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -32,30 +32,30 @@
 
 def new_ticket(
     classification_code: str,
     description: str,
     address: Address,
     date_time: Union[datetime, str] = None,
     requester: Requester = None,
-    occurrence_origin_code: str = "13",  # TODO: review this in the future.
+    occurrence_origin_code: str = "28",
 ) -> NewTicket:
     """
     Creates a new ticket.
 
     Args:
         classification_code (str): The classification code.
         description (str): The description of the occurrence.
         address (Address): The address of the occurrence.
         date_time (Union[datetime, str], optional): The date and time of the occurrence. When
             converted to string, it must be in the following format: "%Y-%m-%dT%H:%M:%S". Defaults
             to `None`, which will be replaced by the current date and time.
         requester (Requester, optional): The requester information. Defaults to `None`, which will
             be replaced by an empty `Requester` object.
         occurrence_origin_code (str, optional): The occurrence origin code (e.g. "13" for
-            "Web App"). Defaults to "13".
+            "Web App"). Defaults to "28".
 
     Returns:
         NewTicket: The new ticket.
 
     Raises:
         BaseSGRCException: If an unexpected exception occurs.
         SGRCBusinessRuleException: If the request violates a business rule.
```

### Comparing `prefeitura_rio-0.1.3/prefeitura_rio/integrations/sgrc/models.py` & `prefeitura_rio-0.1.4/prefeitura_rio/integrations/sgrc/models.py`

 * *Files identical despite different names*

### Comparing `prefeitura_rio-0.1.3/prefeitura_rio/integrations/sgrc/utils.py` & `prefeitura_rio-0.1.4/prefeitura_rio/integrations/sgrc/utils.py`

 * *Files identical despite different names*

### Comparing `prefeitura_rio-0.1.3/prefeitura_rio/metrics/__init__.py` & `prefeitura_rio-0.1.4/prefeitura_rio/metrics/__init__.py`

 * *Files identical despite different names*

### Comparing `prefeitura_rio-0.1.3/prefeitura_rio/metrics/agnostic.py` & `prefeitura_rio-0.1.4/prefeitura_rio/metrics/agnostic.py`

 * *Files identical despite different names*

### Comparing `prefeitura_rio-0.1.3/pyproject.toml` & `prefeitura_rio-0.1.4/pyproject.toml`

 * *Files 16% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "prefeitura-rio"
-version = "0.1.3"
+version = "0.1.4"
 description = "Pacote Python que implementa utilidades para nossos projetos!"
 authors = ["Gabriel Gazola Milan <gabriel.gazola@poli.ufrj.br>"]
 license = "GPL-3.0-only"
 readme = "README.md"
 homepage = "https://github.com/prefeitura-rio/prefeitura-rio"
 repository = "https://github.com/prefeitura-rio/prefeitura-rio"
 keywords = ["python", "utilities", "government"]
```

### Comparing `prefeitura_rio-0.1.3/PKG-INFO` & `prefeitura_rio-0.1.4/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: prefeitura-rio
-Version: 0.1.3
+Version: 0.1.4
 Summary: Pacote Python que implementa utilidades para nossos projetos!
 Home-page: https://github.com/prefeitura-rio/prefeitura-rio
 License: GPL-3.0-only
 Keywords: python,utilities,government
 Author: Gabriel Gazola Milan
 Author-email: gabriel.gazola@poli.ufrj.br
 Requires-Python: >=3.9,<3.11
```

