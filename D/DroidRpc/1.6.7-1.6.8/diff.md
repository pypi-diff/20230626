# Comparing `tmp/DroidRpc-1.6.7.tar.gz` & `tmp/DroidRpc-1.6.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "DroidRpc-1.6.7.tar", last modified: Fri Jun  9 01:37:03 2023, max compression
+gzip compressed data, was "DroidRpc-1.6.8.tar", last modified: Fri Jun 16 07:33:26 2023, max compression
```

## Comparing `DroidRpc-1.6.7.tar` & `DroidRpc-1.6.8.tar`

### file list

```diff
@@ -1,25 +1,25 @@
-drwxrwxr-x   0 loratech  (1000) loratech  (1000)        0 2023-06-09 01:37:03.444829 DroidRpc-1.6.7/
--rwxrwxr-x   0 loratech  (1000) loratech  (1000)       25 2023-05-05 03:50:53.000000 DroidRpc-1.6.7/MANIFEST.in
--rw-rw-r--   0 loratech  (1000) loratech  (1000)      539 2023-06-09 01:37:03.444829 DroidRpc-1.6.7/PKG-INFO
--rwxrwxr-x   0 loratech  (1000) loratech  (1000)      274 2023-05-05 03:50:53.000000 DroidRpc-1.6.7/README.md
--rwxrwxr-x   0 loratech  (1000) loratech  (1000)      132 2023-05-05 03:50:53.000000 DroidRpc-1.6.7/requirements.txt
--rw-rw-r--   0 loratech  (1000) loratech  (1000)       38 2023-06-09 01:37:03.444829 DroidRpc-1.6.7/setup.cfg
--rwxrwxr-x   0 loratech  (1000) loratech  (1000)      777 2023-06-09 01:36:58.000000 DroidRpc-1.6.7/setup.py
-drwxrwxr-x   0 loratech  (1000) loratech  (1000)        0 2023-06-09 01:37:03.440829 DroidRpc-1.6.7/src/
-drwxrwxr-x   0 loratech  (1000) loratech  (1000)        0 2023-06-09 01:37:03.444829 DroidRpc-1.6.7/src/DroidRpc/
--rw-rw-r--   0 loratech  (1000) loratech  (1000)       25 2023-05-05 03:50:53.000000 DroidRpc-1.6.7/src/DroidRpc/__init__.py
--rw-rw-r--   0 loratech  (1000) loratech  (1000)     1767 2023-06-08 10:44:37.000000 DroidRpc-1.6.7/src/DroidRpc/droid_grpc.py
--rw-rw-r--   0 loratech  (1000) loratech  (1000)     5572 2023-06-08 10:44:37.000000 DroidRpc-1.6.7/src/DroidRpc/droid_pb2.py
-drwxrwxr-x   0 loratech  (1000) loratech  (1000)        0 2023-06-09 01:37:03.444829 DroidRpc-1.6.7/src/DroidRpc/formatting/
--rw-rw-r--   0 loratech  (1000) loratech  (1000)      388 2023-05-05 03:50:53.000000 DroidRpc-1.6.7/src/DroidRpc/formatting/__init__.py
--rw-rw-r--   0 loratech  (1000) loratech  (1000)    12910 2023-06-08 10:44:23.000000 DroidRpc-1.6.7/src/DroidRpc/formatting/converter.py
--rw-rw-r--   0 loratech  (1000) loratech  (1000)      398 2023-05-05 03:50:53.000000 DroidRpc-1.6.7/src/DroidRpc/formatting/datetime.py
--rw-rw-r--   0 loratech  (1000) loratech  (1000)    16801 2023-06-08 11:33:24.000000 DroidRpc-1.6.7/src/DroidRpc/main.py
--rw-rw-r--   0 loratech  (1000) loratech  (1000)     4446 2023-05-05 03:50:53.000000 DroidRpc-1.6.7/src/DroidRpc/raw_client_example.py
-drwxrwxr-x   0 loratech  (1000) loratech  (1000)        0 2023-06-09 01:37:03.444829 DroidRpc-1.6.7/src/DroidRpc.egg-info/
--rw-rw-r--   0 loratech  (1000) loratech  (1000)      539 2023-06-09 01:37:03.000000 DroidRpc-1.6.7/src/DroidRpc.egg-info/PKG-INFO
--rw-rw-r--   0 loratech  (1000) loratech  (1000)      504 2023-06-09 01:37:03.000000 DroidRpc-1.6.7/src/DroidRpc.egg-info/SOURCES.txt
--rw-rw-r--   0 loratech  (1000) loratech  (1000)        1 2023-06-09 01:37:03.000000 DroidRpc-1.6.7/src/DroidRpc.egg-info/dependency_links.txt
--rw-rw-r--   0 loratech  (1000) loratech  (1000)        1 2023-06-08 10:50:42.000000 DroidRpc-1.6.7/src/DroidRpc.egg-info/not-zip-safe
--rw-rw-r--   0 loratech  (1000) loratech  (1000)      132 2023-06-09 01:37:03.000000 DroidRpc-1.6.7/src/DroidRpc.egg-info/requires.txt
--rw-rw-r--   0 loratech  (1000) loratech  (1000)        9 2023-06-09 01:37:03.000000 DroidRpc-1.6.7/src/DroidRpc.egg-info/top_level.txt
+drwxrwxr-x   0 loratech  (1000) loratech  (1000)        0 2023-06-16 07:33:26.549226 DroidRpc-1.6.8/
+-rwxrwxr-x   0 loratech  (1000) loratech  (1000)       25 2023-05-05 03:50:53.000000 DroidRpc-1.6.8/MANIFEST.in
+-rw-rw-r--   0 loratech  (1000) loratech  (1000)      539 2023-06-16 07:33:26.549226 DroidRpc-1.6.8/PKG-INFO
+-rwxrwxr-x   0 loratech  (1000) loratech  (1000)      274 2023-05-05 03:50:53.000000 DroidRpc-1.6.8/README.md
+-rwxrwxr-x   0 loratech  (1000) loratech  (1000)      132 2023-05-05 03:50:53.000000 DroidRpc-1.6.8/requirements.txt
+-rw-rw-r--   0 loratech  (1000) loratech  (1000)       38 2023-06-16 07:33:26.549226 DroidRpc-1.6.8/setup.cfg
+-rwxrwxr-x   0 loratech  (1000) loratech  (1000)      777 2023-06-12 02:49:20.000000 DroidRpc-1.6.8/setup.py
+drwxrwxr-x   0 loratech  (1000) loratech  (1000)        0 2023-06-16 07:33:26.545226 DroidRpc-1.6.8/src/
+drwxrwxr-x   0 loratech  (1000) loratech  (1000)        0 2023-06-16 07:33:26.549226 DroidRpc-1.6.8/src/DroidRpc/
+-rw-rw-r--   0 loratech  (1000) loratech  (1000)       25 2023-05-05 03:50:53.000000 DroidRpc-1.6.8/src/DroidRpc/__init__.py
+-rw-rw-r--   0 loratech  (1000) loratech  (1000)     1767 2023-06-12 02:43:44.000000 DroidRpc-1.6.8/src/DroidRpc/droid_grpc.py
+-rw-rw-r--   0 loratech  (1000) loratech  (1000)     5572 2023-06-12 02:43:44.000000 DroidRpc-1.6.8/src/DroidRpc/droid_pb2.py
+drwxrwxr-x   0 loratech  (1000) loratech  (1000)        0 2023-06-16 07:33:26.549226 DroidRpc-1.6.8/src/DroidRpc/formatting/
+-rw-rw-r--   0 loratech  (1000) loratech  (1000)      388 2023-05-05 03:50:53.000000 DroidRpc-1.6.8/src/DroidRpc/formatting/__init__.py
+-rw-rw-r--   0 loratech  (1000) loratech  (1000)    12910 2023-06-13 10:42:31.000000 DroidRpc-1.6.8/src/DroidRpc/formatting/converter.py
+-rw-rw-r--   0 loratech  (1000) loratech  (1000)      398 2023-05-05 03:50:53.000000 DroidRpc-1.6.8/src/DroidRpc/formatting/datetime.py
+-rw-rw-r--   0 loratech  (1000) loratech  (1000)    18858 2023-06-13 10:42:17.000000 DroidRpc-1.6.8/src/DroidRpc/main.py
+-rw-rw-r--   0 loratech  (1000) loratech  (1000)     4446 2023-05-05 03:50:53.000000 DroidRpc-1.6.8/src/DroidRpc/raw_client_example.py
+drwxrwxr-x   0 loratech  (1000) loratech  (1000)        0 2023-06-16 07:33:26.549226 DroidRpc-1.6.8/src/DroidRpc.egg-info/
+-rw-rw-r--   0 loratech  (1000) loratech  (1000)      539 2023-06-16 07:33:26.000000 DroidRpc-1.6.8/src/DroidRpc.egg-info/PKG-INFO
+-rw-rw-r--   0 loratech  (1000) loratech  (1000)      504 2023-06-16 07:33:26.000000 DroidRpc-1.6.8/src/DroidRpc.egg-info/SOURCES.txt
+-rw-rw-r--   0 loratech  (1000) loratech  (1000)        1 2023-06-16 07:33:26.000000 DroidRpc-1.6.8/src/DroidRpc.egg-info/dependency_links.txt
+-rw-rw-r--   0 loratech  (1000) loratech  (1000)        1 2023-06-08 10:50:42.000000 DroidRpc-1.6.8/src/DroidRpc.egg-info/not-zip-safe
+-rw-rw-r--   0 loratech  (1000) loratech  (1000)      132 2023-06-16 07:33:26.000000 DroidRpc-1.6.8/src/DroidRpc.egg-info/requires.txt
+-rw-rw-r--   0 loratech  (1000) loratech  (1000)        9 2023-06-16 07:33:26.000000 DroidRpc-1.6.8/src/DroidRpc.egg-info/top_level.txt
```

### Comparing `DroidRpc-1.6.7/PKG-INFO` & `DroidRpc-1.6.8/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: DroidRpc
-Version: 1.6.7
+Version: 1.6.8
 Summary: Python client for connecting to LORA Technologies' bot services.
 Home-page: https://asklora.ai
 Author: LORA Tech
 Author-email: asklora@loratechai.com
 License: MIT
 Description-Content-Type: text/markdown
```

### Comparing `DroidRpc-1.6.7/setup.py` & `DroidRpc-1.6.8/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -6,15 +6,15 @@
     long_description = f.read()
 
 with open("requirements.txt", "r", encoding="utf-8") as f:
     required = f.read().splitlines()
 
 setuptools.setup(
     name="DroidRpc",
-    version="1.6.7",
+    version="1.6.8",
     description="Python client for connecting to LORA Technologies' bot services.",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://asklora.ai",
     license="MIT",
     install_requires=required,
     author="LORA Tech",
```

### Comparing `DroidRpc-1.6.7/src/DroidRpc/droid_grpc.py` & `DroidRpc-1.6.8/src/DroidRpc/droid_grpc.py`

 * *Files identical despite different names*

### Comparing `DroidRpc-1.6.7/src/DroidRpc/droid_pb2.py` & `DroidRpc-1.6.8/src/DroidRpc/droid_pb2.py`

 * *Files identical despite different names*

### Comparing `DroidRpc-1.6.7/src/DroidRpc/formatting/converter.py` & `DroidRpc-1.6.8/src/DroidRpc/formatting/converter.py`

 * *Files identical despite different names*

### Comparing `DroidRpc-1.6.7/src/DroidRpc/main.py` & `DroidRpc-1.6.8/src/DroidRpc/main.py`

 * *Files 11% similar despite different names*

```diff
@@ -22,16 +22,26 @@
     array_to_bytes,
     bytes_to_array,
     create_request_dict_to_proto,
     hedge_request_dict_to_proto,
     create_response_proto_to_dict,
     hedge_response_proto_to_dict
 )
+from grpclib import GRPCError
 
 
+class BatchInvalidError(Exception):
+    pass
+
+class ArrayToBytesError(Exception):
+    pass
+
+class ConnectFailedError(Exception):
+    pass
+
 class Client:
     """
     This is a thick client, and wraps the raw gRPC client.
     It implements different calling methods for creating and hedging bots, as 
     well as client-side load balancing to accommodate horizontal scaling of the 
     droid server.
 
@@ -179,17 +189,23 @@
 
         Returns:
             dict: A dictionary of bot properties.
         """
         inputs = locals().copy()
         inputs.pop('self')
         inputs = {k: np.array([v]) for k, v in inputs.items() if v is not None}
-        resp = await self.create_bots(**inputs)
-        return {k: v[0] for k, v in resp.items() if v is not None}
-    
+        try:
+            resp = await self.create_bots(**inputs)
+            return {k: v[0] for k, v in resp.items() if v is not None}
+        except BatchInvalidError as e:
+            raise BatchInvalidError(e.message)
+        except ConnectFailedError as e:
+            raise ConnectFailedError(e.message)
+        except Exception as e:
+            raise BatchInvalidError(e.message)
     async def create_bots(
             self,
             ticker: NDArray[str],
             spot_date: NDArray[np.datetime64],
             bot_id: NDArray[str],
             investment_amount: NDArray[np.float32],
             price: NDArray[np.float32],
@@ -220,34 +236,42 @@
             q: Dividend yields.
 
         Returns:
             dict: A dictionary of bot properties.
         """
         inputs = locals().copy()
         inputs.pop('self')
-        inputs = {k: array_to_bytes(v) for k, v in inputs.items() \
-            if v is not None}
+        try:
+            inputs = {k: array_to_bytes(v) for k, v in inputs.items() \
+                if v is not None}
+        except:
+            raise ArrayToBytesError("In valid input. Cannot convert to bytes.")
         assert len(inputs['ticker']) <= self.max_batch_size, \
             f"Max batch size ({self.max_batch_size}) exceeded."
 
         conn_err = False
         for _ in range(self.max_retries):
             try:
                 resp = await next(self._pool_itr)["stub"].CreateBots(
                     BatchCreateRequest(**inputs))
                 break
             except ConnectionRefusedError:
                 print('DROID connection error. Retrying...')
                 self._remove_dead_subclients()
                 conn_err = True
+            except GRPCError as e:
+                raise BatchInvalidError(e.message)
         if conn_err:
             # TODO: Schedule renewing of subclients
             pass
+        try:
+            return create_response_proto_to_dict(resp)
+        except Exception as e:
+            raise ConnectFailedError('DROID connection error after multiple tries')
 
-        return create_response_proto_to_dict(resp)
 
     async def hedge_bot(
         self,
         ticker: NDArray[str],
             spot_date: NDArray[np.datetime64],
             bot_id: NDArray[str],
             investment_amount: NDArray[np.float32],
@@ -284,16 +308,23 @@
 
         Returns:
             Dict[str, NDArray]: A dictionary of bot properties.
         """
         inputs = locals().copy()
         inputs.pop('self')
         inputs = {k: np.array([v]) for k, v in inputs.items() if v is not None}
-        resp = await self.hedge_bots(**inputs)
-        return {k: v[0] for k, v in resp.items() if v is not None}
+        try:
+            resp = await self.hedge_bots(**inputs)
+            return {k: v[0] for k, v in resp.items() if v is not None}
+        except BatchInvalidError as e:
+            raise BatchInvalidError(e.message)
+        except ConnectFailedError as e:
+            raise ConnectFailedError(e.message)
+        except Exception as e:
+            raise BatchInvalidError(e.message)
 
     async def hedge_bots(
             self,
             ticker: NDArray[str],
             spot_date: NDArray[np.datetime64],
             bot_id: NDArray[str],
             investment_amount: NDArray[np.float32],
@@ -330,35 +361,42 @@
             q: Dividend yields.
 
         Returns:
             Dict[str, NDArray]: A dictionary of bot properties.
         """
         inputs = locals().copy()
         inputs.pop('self')
-        inputs = {k: array_to_bytes(v) for k, v in inputs.items() \
-            if v is not None}
+        try:
+            inputs = {k: array_to_bytes(v) for k, v in inputs.items() \
+                if v is not None}
+        except:
+            raise ArrayToBytesError("In valid input. Cannot convert to bytes.")
         assert len(inputs['ticker']) <= self.max_batch_size, \
             f"Max batch size ({self.max_batch_size}) exceeded."
         
         conn_err = False
         for _ in range(self.max_retries):
             try:
                 resp = await next(self._pool_itr)["stub"].HedgeBots(
                     BatchHedgeRequest(**inputs))
             except ConnectionRefusedError:
                 print('DROID connection error. Retrying...')
                 self._remove_dead_subclients()
                 # TODO: Schedule renewal of subclients
                 resp = await next(self._pool_itr)["stub"].HedgeBots(
                     BatchHedgeRequest(**inputs))
+            except GRPCError as e:
+                raise BatchInvalidError(e.message)
         if conn_err:
             # TODO: Schedule renewal of subclients
             pass
-
-        return hedge_response_proto_to_dict(resp)
+        try:
+            return hedge_response_proto_to_dict(resp)
+        except Exception as e:
+            raise ConnectFailedError('DROID connection error after multiple tries')
     
     async def create_bots_from_dataframe(
             self,
             inputs: pd.DataFrame,
         ) -> pd.DataFrame:
         """
         Creates a batch of bots from a dataframe containing inputs.
@@ -368,38 +406,44 @@
         """
         # Convert to dict of numpy arrays
         inputs = inputs.to_dict(orient='list')
         assert len(inputs['ticker']) <= self.max_batch_size, \
             f"Max batch size ({self.max_batch_size}) exceeded."
         spot_dates = pd.to_datetime(inputs["spot_date"]).date.astype(str)
         del inputs["spot_date"] # Because this breaks below dict comprehension
-        inputs = {k: array_to_bytes(np.array(v)) \
+        try:
+            inputs = {k: array_to_bytes(np.array(v)) \
             for k, v in inputs.items() \
             if v is not None}
-        inputs["spot_date"] = array_to_bytes(spot_dates)
-
+            inputs["spot_date"] = array_to_bytes(spot_dates)
+        except:
+            raise ArrayToBytesError("In valid input. Cannot convert to bytes.")
         # Call DROID
         # TODO: Use self.create_bots() instead, reduce code duplication
         conn_err = False
         for _ in range(self.max_retries):
             try:
                 resp = await next(self._pool_itr)["stub"].CreateBots(
                     BatchCreateRequest(**inputs))
                 break
             # TODO: better error handling here (e.g. for TimeoutError)
             except ConnectionRefusedError:
                 print('DROID connection error. Retrying...')
                 self._remove_dead_subclients()
                 conn_err = True
+            except GRPCError as e:
+                raise BatchInvalidError(e.message)
         if conn_err:
             self.renew_pool()
             # TODO: Schedule renewing of subclients
             pass
-
-        resp = create_response_proto_to_dict(resp)
+        try:
+            resp = create_response_proto_to_dict(resp)
+        except Exception as e:
+            raise ConnectFailedError('DROID connection error after multiple tries')
         return pd.DataFrame.from_dict(resp)
 
     async def hedge_bots_from_dataframe(
             self,
             inputs: pd.DataFrame,
         ) -> pd.DataFrame:
         """
@@ -414,32 +458,38 @@
         assert len(inputs['ticker']) <= self.max_batch_size, \
             f"Max batch size ({self.max_batch_size}) exceeded."
         spot_dates = pd.to_datetime(inputs["spot_date"]).date.astype(str)
         expire_dates = pd.to_datetime(inputs["expire_date"]).date.astype(str)
         del inputs["spot_date"] # Because these break below dict comprehension
         del inputs["expire_date"]
         
-        inputs = {k: array_to_bytes(np.array(v)) \
-            for k, v in inputs.items() \
-            if v is not None}
-        inputs["spot_date"] = array_to_bytes(spot_dates)
-        inputs["expire_date"] = array_to_bytes(expire_dates)
-
+        try:
+            inputs = {k: array_to_bytes(np.array(v)) \
+                for k, v in inputs.items() \
+                if v is not None}
+            inputs["spot_date"] = array_to_bytes(spot_dates)
+            inputs["expire_date"] = array_to_bytes(expire_dates)
+        except:
+            raise ArrayToBytesError("In valid input. Cannot convert to bytes.")
         conn_err = False
         for _ in range(self.max_retries):
             try:
                 resp = await next(self._pool_itr)["stub"].HedgeBots(
                     BatchHedgeRequest(**inputs))
                 break
             except ConnectionRefusedError:
                 print('DROID connection error. Retrying...')
                 self._remove_dead_subclients()
                 conn_err = True
             except TimeoutError:
                 conn_err = True
+            except GRPCError as e:
+                raise BatchInvalidError(e.message)
         if conn_err:
             self.renew_pool()
             # TODO: Schedule renewing of subclients
             pass
-
-        resp = hedge_response_proto_to_dict(resp)
+        try:
+            resp = hedge_response_proto_to_dict(resp)
+        except Exception as e:
+            raise ConnectFailedError('DROID connection error after multiple tries')
         return pd.DataFrame.from_dict(resp)
```

### Comparing `DroidRpc-1.6.7/src/DroidRpc/raw_client_example.py` & `DroidRpc-1.6.8/src/DroidRpc/raw_client_example.py`

 * *Files identical despite different names*

### Comparing `DroidRpc-1.6.7/src/DroidRpc.egg-info/PKG-INFO` & `DroidRpc-1.6.8/src/DroidRpc.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: DroidRpc
-Version: 1.6.7
+Version: 1.6.8
 Summary: Python client for connecting to LORA Technologies' bot services.
 Home-page: https://asklora.ai
 Author: LORA Tech
 Author-email: asklora@loratechai.com
 License: MIT
 Description-Content-Type: text/markdown
```

