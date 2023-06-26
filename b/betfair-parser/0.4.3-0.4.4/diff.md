# Comparing `tmp/betfair_parser-0.4.3.tar.gz` & `tmp/betfair_parser-0.4.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "betfair_parser-0.4.3.tar", max compression
+gzip compressed data, was "betfair_parser-0.4.4.tar", max compression
```

## Comparing `betfair_parser-0.4.3.tar` & `betfair_parser-0.4.4.tar`

### file list

```diff
@@ -1,33 +1,33 @@
--rw-r--r--   0        0        0     1286 2023-06-21 01:47:50.300462 betfair_parser-0.4.3/LICENSE.txt
--rw-r--r--   0        0        0     3277 2023-06-21 01:47:50.300462 betfair_parser-0.4.3/README.md
--rw-r--r--   0        0        0        0 2023-06-21 01:47:50.300462 betfair_parser-0.4.3/betfair_parser/__init__.py
--rw-r--r--   0        0        0     2054 2023-06-21 01:47:50.300462 betfair_parser-0.4.3/betfair_parser/client.py
--rw-r--r--   0        0        0     2417 2023-06-21 01:47:50.300462 betfair_parser-0.4.3/betfair_parser/endpoints.py
--rw-r--r--   0        0        0      741 2023-06-21 01:47:50.300462 betfair_parser-0.4.3/betfair_parser/exceptions.py
--rw-r--r--   0        0        0        0 2023-06-21 01:47:50.300462 betfair_parser-0.4.3/betfair_parser/spec/__init__.py
--rw-r--r--   0        0        0       85 2023-06-21 01:47:50.300462 betfair_parser-0.4.3/betfair_parser/spec/accounts/__init__.py
--rw-r--r--   0        0        0     2929 2023-06-21 01:47:50.300462 betfair_parser-0.4.3/betfair_parser/spec/accounts/enums.py
--rw-r--r--   0        0        0     3278 2023-06-21 01:47:50.300462 betfair_parser-0.4.3/betfair_parser/spec/accounts/operations.py
--rw-r--r--   0        0        0    11161 2023-06-21 01:47:50.300462 betfair_parser-0.4.3/betfair_parser/spec/accounts/type_definitions.py
--rw-r--r--   0        0        0       84 2023-06-21 01:47:50.300462 betfair_parser-0.4.3/betfair_parser/spec/betting/__init__.py
--rw-r--r--   0        0        0    21951 2023-06-21 01:47:50.300462 betfair_parser-0.4.3/betfair_parser/spec/betting/enums.py
--rw-r--r--   0        0        0     9634 2023-06-21 01:47:50.300462 betfair_parser-0.4.3/betfair_parser/spec/betting/listings.py
--rw-r--r--   0        0        0      134 2023-06-21 01:47:50.300462 betfair_parser-0.4.3/betfair_parser/spec/betting/operations.py
--rw-r--r--   0        0        0     8860 2023-06-21 01:47:50.300462 betfair_parser-0.4.3/betfair_parser/spec/betting/orders.py
--rw-r--r--   0        0        0    32923 2023-06-21 01:47:50.304462 betfair_parser-0.4.3/betfair_parser/spec/betting/type_definitions.py
--rw-r--r--   0        0        0      238 2023-06-21 01:47:50.304462 betfair_parser-0.4.3/betfair_parser/spec/common/__init__.py
--rw-r--r--   0        0        0     9771 2023-06-21 01:47:50.304462 betfair_parser-0.4.3/betfair_parser/spec/common/enums.py
--rw-r--r--   0        0        0     4740 2023-06-21 01:47:50.304462 betfair_parser-0.4.3/betfair_parser/spec/common/messages.py
--rw-r--r--   0        0        0     1493 2023-06-21 01:47:50.304462 betfair_parser-0.4.3/betfair_parser/spec/common/type_definitions.py
--rw-r--r--   0        0        0     2773 2023-06-21 01:47:50.304462 betfair_parser-0.4.3/betfair_parser/spec/heartbeat.py
--rw-r--r--   0        0        0     8653 2023-06-21 01:47:50.304462 betfair_parser-0.4.3/betfair_parser/spec/identity.py
--rw-r--r--   0        0        0     3645 2023-06-21 01:47:50.304462 betfair_parser-0.4.3/betfair_parser/spec/navigation.py
--rw-r--r--   0        0        0     3172 2023-06-21 01:47:50.304462 betfair_parser-0.4.3/betfair_parser/spec/race_status.py
--rw-r--r--   0        0        0      399 2023-06-21 01:47:50.304462 betfair_parser-0.4.3/betfair_parser/spec/streaming/__init__.py
--rw-r--r--   0        0        0     5989 2023-06-21 01:47:50.304462 betfair_parser-0.4.3/betfair_parser/spec/streaming/mcm.py
--rw-r--r--   0        0        0     2247 2023-06-21 01:47:50.304462 betfair_parser-0.4.3/betfair_parser/spec/streaming/ocm.py
--rw-r--r--   0        0        0     2507 2023-06-21 01:47:50.304462 betfair_parser-0.4.3/betfair_parser/spec/streaming/status.py
--rw-r--r--   0        0        0     2319 2023-06-21 01:47:50.304462 betfair_parser-0.4.3/betfair_parser/strenums.py
--rw-r--r--   0        0        0      902 2023-06-21 01:47:50.304462 betfair_parser-0.4.3/betfair_parser/util.py
--rw-r--r--   0        0        0     1731 2023-06-21 01:48:07.032525 betfair_parser-0.4.3/pyproject.toml
--rw-r--r--   0        0        0     3767 1970-01-01 00:00:00.000000 betfair_parser-0.4.3/PKG-INFO
+-rw-r--r--   0        0        0     1286 2023-06-26 20:38:03.031096 betfair_parser-0.4.4/LICENSE.txt
+-rw-r--r--   0        0        0     3277 2023-06-26 20:38:03.031096 betfair_parser-0.4.4/README.md
+-rw-r--r--   0        0        0        0 2023-06-26 20:38:03.031096 betfair_parser-0.4.4/betfair_parser/__init__.py
+-rw-r--r--   0        0        0     2090 2023-06-26 20:38:03.031096 betfair_parser-0.4.4/betfair_parser/client.py
+-rw-r--r--   0        0        0     2417 2023-06-26 20:38:03.031096 betfair_parser-0.4.4/betfair_parser/endpoints.py
+-rw-r--r--   0        0        0      741 2023-06-26 20:38:03.035096 betfair_parser-0.4.4/betfair_parser/exceptions.py
+-rw-r--r--   0        0        0        0 2023-06-26 20:38:03.035096 betfair_parser-0.4.4/betfair_parser/spec/__init__.py
+-rw-r--r--   0        0        0       85 2023-06-26 20:38:03.035096 betfair_parser-0.4.4/betfair_parser/spec/accounts/__init__.py
+-rw-r--r--   0        0        0     2929 2023-06-26 20:38:03.035096 betfair_parser-0.4.4/betfair_parser/spec/accounts/enums.py
+-rw-r--r--   0        0        0     3278 2023-06-26 20:38:03.035096 betfair_parser-0.4.4/betfair_parser/spec/accounts/operations.py
+-rw-r--r--   0        0        0    11161 2023-06-26 20:38:03.035096 betfair_parser-0.4.4/betfair_parser/spec/accounts/type_definitions.py
+-rw-r--r--   0        0        0       84 2023-06-26 20:38:03.035096 betfair_parser-0.4.4/betfair_parser/spec/betting/__init__.py
+-rw-r--r--   0        0        0    21951 2023-06-26 20:38:03.035096 betfair_parser-0.4.4/betfair_parser/spec/betting/enums.py
+-rw-r--r--   0        0        0     9634 2023-06-26 20:38:03.035096 betfair_parser-0.4.4/betfair_parser/spec/betting/listings.py
+-rw-r--r--   0        0        0      134 2023-06-26 20:38:03.035096 betfair_parser-0.4.4/betfair_parser/spec/betting/operations.py
+-rw-r--r--   0        0        0     8860 2023-06-26 20:38:03.035096 betfair_parser-0.4.4/betfair_parser/spec/betting/orders.py
+-rw-r--r--   0        0        0    32923 2023-06-26 20:38:03.035096 betfair_parser-0.4.4/betfair_parser/spec/betting/type_definitions.py
+-rw-r--r--   0        0        0      238 2023-06-26 20:38:03.035096 betfair_parser-0.4.4/betfair_parser/spec/common/__init__.py
+-rw-r--r--   0        0        0     9771 2023-06-26 20:38:03.035096 betfair_parser-0.4.4/betfair_parser/spec/common/enums.py
+-rw-r--r--   0        0        0     4829 2023-06-26 20:38:03.035096 betfair_parser-0.4.4/betfair_parser/spec/common/messages.py
+-rw-r--r--   0        0        0     1493 2023-06-26 20:38:03.035096 betfair_parser-0.4.4/betfair_parser/spec/common/type_definitions.py
+-rw-r--r--   0        0        0     2773 2023-06-26 20:38:03.035096 betfair_parser-0.4.4/betfair_parser/spec/heartbeat.py
+-rw-r--r--   0        0        0     8653 2023-06-26 20:38:03.035096 betfair_parser-0.4.4/betfair_parser/spec/identity.py
+-rw-r--r--   0        0        0     3645 2023-06-26 20:38:03.035096 betfair_parser-0.4.4/betfair_parser/spec/navigation.py
+-rw-r--r--   0        0        0     3172 2023-06-26 20:38:03.035096 betfair_parser-0.4.4/betfair_parser/spec/race_status.py
+-rw-r--r--   0        0        0      399 2023-06-26 20:38:03.035096 betfair_parser-0.4.4/betfair_parser/spec/streaming/__init__.py
+-rw-r--r--   0        0        0     5989 2023-06-26 20:38:03.035096 betfair_parser-0.4.4/betfair_parser/spec/streaming/mcm.py
+-rw-r--r--   0        0        0     2247 2023-06-26 20:38:03.035096 betfair_parser-0.4.4/betfair_parser/spec/streaming/ocm.py
+-rw-r--r--   0        0        0     2507 2023-06-26 20:38:03.035096 betfair_parser-0.4.4/betfair_parser/spec/streaming/status.py
+-rw-r--r--   0        0        0     2319 2023-06-26 20:38:03.035096 betfair_parser-0.4.4/betfair_parser/strenums.py
+-rw-r--r--   0        0        0      902 2023-06-26 20:38:03.035096 betfair_parser-0.4.4/betfair_parser/util.py
+-rw-r--r--   0        0        0     1731 2023-06-26 20:38:23.011106 betfair_parser-0.4.4/pyproject.toml
+-rw-r--r--   0        0        0     3767 1970-01-01 00:00:00.000000 betfair_parser-0.4.4/PKG-INFO
```

### Comparing `betfair_parser-0.4.3/LICENSE.txt` & `betfair_parser-0.4.4/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `betfair_parser-0.4.3/README.md` & `betfair_parser-0.4.4/README.md`

 * *Files identical despite different names*

### Comparing `betfair_parser-0.4.3/betfair_parser/client.py` & `betfair_parser-0.4.4/betfair_parser/client.py`

 * *Files 8% similar despite different names*

```diff
@@ -55,9 +55,11 @@
         CertLogin.with_params(username=username, password=password),
         endpoints=endpoints,
     )
     session.headers.update({"X-Authentication": resp.token})
 
 
 def logout(session, endpoints=ENDPOINTS):
-    request(session, Logout(), endpoints=endpoints)
-    del session.headers["X-Authentication"]
+    try:
+        request(session, Logout(), endpoints=endpoints)
+    finally:
+        session.headers.pop("X-Authentication", None)
```

### Comparing `betfair_parser-0.4.3/betfair_parser/endpoints.py` & `betfair_parser-0.4.4/betfair_parser/endpoints.py`

 * *Files identical despite different names*

### Comparing `betfair_parser-0.4.3/betfair_parser/exceptions.py` & `betfair_parser-0.4.4/betfair_parser/exceptions.py`

 * *Files identical despite different names*

### Comparing `betfair_parser-0.4.3/betfair_parser/spec/accounts/enums.py` & `betfair_parser-0.4.4/betfair_parser/spec/accounts/enums.py`

 * *Files identical despite different names*

### Comparing `betfair_parser-0.4.3/betfair_parser/spec/accounts/operations.py` & `betfair_parser-0.4.4/betfair_parser/spec/accounts/operations.py`

 * *Files identical despite different names*

### Comparing `betfair_parser-0.4.3/betfair_parser/spec/accounts/type_definitions.py` & `betfair_parser-0.4.4/betfair_parser/spec/accounts/type_definitions.py`

 * *Files identical despite different names*

### Comparing `betfair_parser-0.4.3/betfair_parser/spec/betting/enums.py` & `betfair_parser-0.4.4/betfair_parser/spec/betting/enums.py`

 * *Files identical despite different names*

### Comparing `betfair_parser-0.4.3/betfair_parser/spec/betting/listings.py` & `betfair_parser-0.4.4/betfair_parser/spec/betting/listings.py`

 * *Files identical despite different names*

### Comparing `betfair_parser-0.4.3/betfair_parser/spec/betting/orders.py` & `betfair_parser-0.4.4/betfair_parser/spec/betting/orders.py`

 * *Files identical despite different names*

### Comparing `betfair_parser-0.4.3/betfair_parser/spec/betting/type_definitions.py` & `betfair_parser-0.4.4/betfair_parser/spec/betting/type_definitions.py`

 * *Files identical despite different names*

### Comparing `betfair_parser-0.4.3/betfair_parser/spec/common/enums.py` & `betfair_parser-0.4.4/betfair_parser/spec/common/enums.py`

 * *Files identical despite different names*

### Comparing `betfair_parser-0.4.3/betfair_parser/spec/common/messages.py` & `betfair_parser-0.4.4/betfair_parser/spec/common/messages.py`

 * *Files 3% similar despite different names*

```diff
@@ -32,14 +32,17 @@
 
     def validate(self):
         return bool(decode(encode(self), type=type(self)))
 
     def to_dict(self):
         return msgspec.structs.asdict(self)
 
+    def replace(self, **kwargs):
+        return msgspec.structs.replace(self, **kwargs)
+
 
 class Params(BaseMessage, omit_defaults=True, frozen=True):
     """By default, don't send None and other default values in operation parameters."""
 
 
 class BaseResponse(BaseMessage, frozen=True):
     """Base class for Response, ErrorResponse and identity responses."""
```

### Comparing `betfair_parser-0.4.3/betfair_parser/spec/common/type_definitions.py` & `betfair_parser-0.4.4/betfair_parser/spec/common/type_definitions.py`

 * *Files identical despite different names*

### Comparing `betfair_parser-0.4.3/betfair_parser/spec/heartbeat.py` & `betfair_parser-0.4.4/betfair_parser/spec/heartbeat.py`

 * *Files identical despite different names*

### Comparing `betfair_parser-0.4.3/betfair_parser/spec/identity.py` & `betfair_parser-0.4.4/betfair_parser/spec/identity.py`

 * *Files identical despite different names*

### Comparing `betfair_parser-0.4.3/betfair_parser/spec/navigation.py` & `betfair_parser-0.4.4/betfair_parser/spec/navigation.py`

 * *Files identical despite different names*

### Comparing `betfair_parser-0.4.3/betfair_parser/spec/race_status.py` & `betfair_parser-0.4.4/betfair_parser/spec/race_status.py`

 * *Files identical despite different names*

### Comparing `betfair_parser-0.4.3/betfair_parser/spec/streaming/mcm.py` & `betfair_parser-0.4.4/betfair_parser/spec/streaming/mcm.py`

 * *Files identical despite different names*

### Comparing `betfair_parser-0.4.3/betfair_parser/spec/streaming/ocm.py` & `betfair_parser-0.4.4/betfair_parser/spec/streaming/ocm.py`

 * *Files identical despite different names*

### Comparing `betfair_parser-0.4.3/betfair_parser/spec/streaming/status.py` & `betfair_parser-0.4.4/betfair_parser/spec/streaming/status.py`

 * *Files identical despite different names*

### Comparing `betfair_parser-0.4.3/betfair_parser/strenums.py` & `betfair_parser-0.4.4/betfair_parser/strenums.py`

 * *Files identical despite different names*

### Comparing `betfair_parser-0.4.3/betfair_parser/util.py` & `betfair_parser-0.4.4/betfair_parser/util.py`

 * *Files identical despite different names*

### Comparing `betfair_parser-0.4.3/pyproject.toml` & `betfair_parser-0.4.4/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -37,15 +37,15 @@
 
 [build-system]
 requires = ["poetry-core>=1.0.0"]
 build-backend = "poetry.core.masonry.api"
 
 [tool.poetry]
 name = "betfair_parser"
-version = "0.4.3"
+version = "0.4.4"
 description = "A betfair parser"
 readme = "README.md"
 authors = ["Bradley McElroy <bradley.mcelroy@live.com>"]
 
 [tool.poetry.dependencies]
 python = ">=3.9,<4.0"
 msgspec = "^0.16.0"
```

### Comparing `betfair_parser-0.4.3/PKG-INFO` & `betfair_parser-0.4.4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: betfair-parser
-Version: 0.4.3
+Version: 0.4.4
 Summary: A betfair parser
 Author: Bradley McElroy
 Author-email: bradley.mcelroy@live.com
 Requires-Python: >=3.9,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
```

