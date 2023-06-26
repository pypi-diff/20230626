# Comparing `tmp/zep_python-0.31.tar.gz` & `tmp/zep_python-0.32.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "zep_python-0.31.tar", max compression
+gzip compressed data, was "zep_python-0.32.tar", max compression
```

## Comparing `zep_python-0.31.tar` & `zep_python-0.32.tar`

### file list

```diff
@@ -1,9 +1,9 @@
--rw-r--r--   0        0        0    11357 2023-06-05 15:48:33.601814 zep_python-0.31/LICENSE
--rw-r--r--   0        0        0     2402 2023-06-05 15:48:33.605814 zep_python-0.31/README.md
--rw-r--r--   0        0        0      872 2023-06-05 15:48:33.605814 zep_python-0.31/pyproject.toml
--rw-r--r--   0        0        0      389 2023-06-05 15:48:33.605814 zep_python-0.31/zep_python/__init__.py
--rw-r--r--   0        0        0     1685 2023-06-05 15:48:33.605814 zep_python-0.31/zep_python/exceptions.py
--rw-r--r--   0        0        0     4882 2023-06-05 15:48:33.605814 zep_python-0.31/zep_python/models.py
--rw-r--r--   0        0        0        0 2023-06-05 15:48:33.605814 zep_python-0.31/zep_python/py.typed
--rw-r--r--   0        0        0    13286 2023-06-05 15:48:33.605814 zep_python-0.31/zep_python/zep_client.py
--rw-r--r--   0        0        0     3081 1970-01-01 00:00:00.000000 zep_python-0.31/PKG-INFO
+-rw-r--r--   0        0        0    11357 2023-06-26 21:22:44.926598 zep_python-0.32/LICENSE
+-rw-r--r--   0        0        0     2402 2023-06-26 21:22:44.926598 zep_python-0.32/README.md
+-rw-r--r--   0        0        0      872 2023-06-26 21:22:44.930598 zep_python-0.32/pyproject.toml
+-rw-r--r--   0        0        0      389 2023-06-26 21:22:44.930598 zep_python-0.32/zep_python/__init__.py
+-rw-r--r--   0        0        0     2234 2023-06-26 21:22:44.930598 zep_python-0.32/zep_python/exceptions.py
+-rw-r--r--   0        0        0     4882 2023-06-26 21:22:44.930598 zep_python-0.32/zep_python/models.py
+-rw-r--r--   0        0        0        0 2023-06-26 21:22:44.930598 zep_python-0.32/zep_python/py.typed
+-rw-r--r--   0        0        0    13149 2023-06-26 21:22:44.930598 zep_python-0.32/zep_python/zep_client.py
+-rw-r--r--   0        0        0     3081 1970-01-01 00:00:00.000000 zep_python-0.32/PKG-INFO
```

### Comparing `zep_python-0.31/LICENSE` & `zep_python-0.32/LICENSE`

 * *Files identical despite different names*

### Comparing `zep_python-0.31/README.md` & `zep_python-0.32/README.md`

 * *Files identical despite different names*

### Comparing `zep_python-0.31/pyproject.toml` & `zep_python-0.32/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "zep-python"
-version = "0.31"
+version = "0.32"
 description = "Zep stores, manages, enriches, indexes, and searches long-term memory for conversational AI applications. This is the Python client for the Zep service."
 authors = ["Daniel Chalef <daniel.chalef@private.org>"]
 readme = "README.md"
 
 [tool.poetry.dependencies]
 python = "^3.8"
 httpx = "^0.24.0"
```

### Comparing `zep_python-0.31/zep_python/exceptions.py` & `zep_python-0.32/zep_python/exceptions.py`

 * *Files 6% similar despite different names*

```diff
@@ -51,14 +51,36 @@
                 "message": response.text,
             }
         else:
             response_data = None
         super().__init__(message=message, response_data=response_data)
 
 
+class AuthError(ZepClientError):
+    """
+    Raised when API authentication fails.
+
+    Inherits from APIError.
+    """
+
+    def __init__(
+        self,
+        response: Union[httpx.Response, None] = None,
+        message: str = "Authentication error",
+    ) -> None:
+        if response:
+            response_data = {
+                "status_code": response.status_code,
+                "message": response.text,
+            }
+        else:
+            response_data = None
+        super().__init__(message=message, response_data=response_data)
+
+
 class NotFoundError(ZepClientError):
     """
     Raised when the API response contains no results.
 
     Inherits from ZepClientError.
     """
```

### Comparing `zep_python-0.31/zep_python/models.py` & `zep_python-0.32/zep_python/models.py`

 * *Files identical despite different names*

### Comparing `zep_python-0.31/zep_python/zep_client.py` & `zep_python-0.32/zep_python/zep_client.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from __future__ import annotations
 
 from types import TracebackType
 from typing import Any, Dict, List, Optional, Type
 
 import httpx
 
-from zep_python.exceptions import APIError, NotFoundError
+from zep_python.exceptions import APIError, AuthError, NotFoundError
 from zep_python.models import (
     Memory,
     MemorySearchPayload,
     MemorySearchResult,
     Message,
     Summary,
 )
@@ -39,26 +39,34 @@
     search_memory(session_id: str, search_payload: SearchPayload,
                   limit: Optional[int] = None) -> List[SearchResult]:
         Search memory for the specified session.
     close() -> None:
         Close the HTTP client.
     """
 
-    def __init__(self, base_url: str) -> None:
+    def __init__(self, base_url: str, api_key: Optional[str] = None) -> None:
         """
         Initialize the ZepClient with the specified base URL.
 
         Parameters
         ----------
         base_url : str
             The base URL of the API.
+
+        api_key : Optional[str]
+            The API key to use for authentication. (optional)
         """
+
+        headers: Dict[str, str] = {}
+        if api_key is not None:
+            headers["Authorization"] = f"Bearer {api_key}"
+
         self.base_url = f"{base_url}{API_BASE_PATH}"
-        self.aclient = httpx.AsyncClient(base_url=self.base_url)
-        self.client = httpx.Client(base_url=self.base_url)
+        self.aclient = httpx.AsyncClient(base_url=self.base_url, headers=headers)
+        self.client = httpx.Client(base_url=self.base_url, headers=headers)
 
     async def __aenter__(self) -> "ZepClient":
         """Asynchronous context manager entry point"""
         return self
 
     async def __aexit__(
         self,
@@ -78,14 +86,27 @@
         exc_type: Type[Exception],
         exc_val: Exception,
         exc_tb: TracebackType,
     ) -> None:
         """Sync context manager exit point"""
         self.close()
 
+    def _handle_response(
+        self, response: httpx.Response, missing_message: Optional[str] = None
+    ) -> None:
+        missing_message = missing_message or "No query results found"
+        if response.status_code == 404:
+            raise NotFoundError(missing_message)
+
+        if response.status_code == 401:
+            raise AuthError(response)
+
+        if response.status_code != 200:
+            raise APIError(response)
+
     def _parse_get_memory_response(self, response_data: Any) -> Memory:
         """Parse the response from the get_memory API call."""
         messages: List[Message]
         try:
             messages = [
                 Message.parse_obj(m) for m in response_data.get("messages", None)
             ]
@@ -139,19 +160,15 @@
         if session_id is None or session_id == "":
             raise ValueError("session_id must be provided")
 
         url = f"/sessions/{session_id}/memory"
         params = self._gen_get_params(lastn)
         response = self.client.get(url, params=params)
 
-        if response.status_code == 404:
-            raise NotFoundError(f"No memory found for session {session_id}")
-
-        if response.status_code != 200:
-            raise APIError(response)
+        self._handle_response(response, f"No memory found for session {session_id}")
 
         response_data = response.json()
 
         return self._parse_get_memory_response(response_data)
 
     async def aget_memory(self, session_id: str, lastn: Optional[int] = None) -> Memory:
         """
@@ -178,19 +195,15 @@
         if session_id is None or session_id == "":
             raise ValueError("session_id must be provided")
 
         url = f"/sessions/{session_id}/memory"
         params = self._gen_get_params(lastn)
         response = await self.aclient.get(url, params=params)
 
-        if response.status_code == 404:
-            raise NotFoundError(f"No memory found for session {session_id}")
-
-        if response.status_code != 200:
-            raise APIError(response)
+        self._handle_response(response, f"No memory found for session {session_id}")
 
         response_data = response.json()
 
         return self._parse_get_memory_response(response_data)
 
     def add_memory(self, session_id: str, memory_messages: Memory) -> str:
         """
@@ -216,16 +229,16 @@
         if session_id is None or session_id == "":
             raise ValueError("session_id must be provided")
 
         response = self.client.post(
             f"/sessions/{session_id}/memory",
             json=memory_messages.dict(exclude_none=True),
         )
-        if response.status_code != 200:
-            raise APIError(response)
+
+        self._handle_response(response)
 
         return response.text
 
     async def aadd_memory(self, session_id: str, memory_messages: Memory) -> str:
         """
         Asynchronously add memory to the specified session.
 
@@ -249,16 +262,16 @@
         if session_id is None or session_id == "":
             raise ValueError("session_id must be provided")
 
         response = await self.aclient.post(
             f"/sessions/{session_id}/memory",
             json=memory_messages.dict(exclude_none=True),
         )
-        if response.status_code != 200:
-            raise APIError(response)
+
+        self._handle_response(response)
 
         return response.text
 
     def delete_memory(self, session_id: str) -> str:
         """
         Delete memory for the specified session.
 
@@ -277,19 +290,15 @@
         APIError
             If the API response format is unexpected.
         """
         if session_id is None or session_id == "":
             raise ValueError("session_id must be provided")
 
         response = self.client.delete(f"/sessions/{session_id}/memory")
-        if response.status_code == 404:
-            raise NotFoundError(f"No session found for session {session_id}")
-
-        if response.status_code != 200:
-            raise APIError(response)
+        self._handle_response(response)
         return response.text
 
     async def adelete_memory(self, session_id: str) -> str:
         """
         Asynchronously delete memory for the specified session.
 
         Parameters
@@ -307,19 +316,15 @@
         APIError
             If the API response format is unexpected.
         """
         if session_id is None or session_id == "":
             raise ValueError("session_id must be provided")
 
         response = await self.aclient.delete(f"/sessions/{session_id}/memory")
-        if response.status_code == 404:
-            raise NotFoundError(f"No session found for session {session_id}")
-
-        if response.status_code != 200:
-            raise APIError(response)
+        self._handle_response(response)
         return response.text
 
     def search_memory(
         self,
         session_id: str,
         search_payload: MemorySearchPayload,
         limit: Optional[int] = None,
@@ -354,18 +359,15 @@
 
         params = {"limit": limit} if limit is not None else {}
         response = self.client.post(
             f"/sessions/{session_id}/search",
             json=search_payload.dict(),
             params=params,
         )
-        if response.status_code == 404:
-            raise NotFoundError("No query results found")
-        if response.status_code != 200:
-            raise APIError(response)
+        self._handle_response(response)
         return [
             MemorySearchResult(**search_result) for search_result in response.json()
         ]
 
     async def asearch_memory(
         self,
         session_id: str,
@@ -402,18 +404,15 @@
 
         params = {"limit": limit} if limit is not None else {}
         response = await self.aclient.post(
             f"/sessions/{session_id}/search",
             json=search_payload.dict(),
             params=params,
         )
-        if response.status_code == 404:
-            raise NotFoundError("No query results found")
-        if response.status_code != 200:
-            raise APIError(response)
+        self._handle_response(response)
         return [
             MemorySearchResult(**search_result) for search_result in response.json()
         ]
 
     async def aclose(self) -> None:
         """
         Asynchronously close the HTTP client.
```

### Comparing `zep_python-0.31/PKG-INFO` & `zep_python-0.32/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: zep-python
-Version: 0.31
+Version: 0.32
 Summary: Zep stores, manages, enriches, indexes, and searches long-term memory for conversational AI applications. This is the Python client for the Zep service.
 Author: Daniel Chalef
 Author-email: daniel.chalef@private.org
 Requires-Python: >=3.8,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
```

