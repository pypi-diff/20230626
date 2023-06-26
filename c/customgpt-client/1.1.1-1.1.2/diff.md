# Comparing `tmp/customgpt_client-1.1.1-py3-none-any.whl.zip` & `tmp/customgpt_client-1.1.2-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,18 +1,18 @@
-Zip file size: 304608 bytes, number of entries: 376
+Zip file size: 304733 bytes, number of entries: 376
 -rw-r--r--  2.0 unx      105 b- defN 80-Jan-01 00:00 customgpt_client/__init__.py
 -rw-r--r--  2.0 unx       47 b- defN 80-Jan-01 00:00 customgpt_client/api/__init__.py
 -rw-r--r--  2.0 unx        0 b- defN 80-Jan-01 00:00 customgpt_client/api/citations/__init__.py
 -rw-r--r--  2.0 unx     6513 b- defN 80-Jan-01 00:00 customgpt_client/api/citations/get_open_graph_data_for_citation.py
 -rw-r--r--  2.0 unx        0 b- defN 80-Jan-01 00:00 customgpt_client/api/conversations/__init__.py
 -rw-r--r--  2.0 unx     7370 b- defN 80-Jan-01 00:00 customgpt_client/api/conversations/create_project_conversation.py
 -rw-r--r--  2.0 unx     6970 b- defN 80-Jan-01 00:00 customgpt_client/api/conversations/delete_project_conversation.py
 -rw-r--r--  2.0 unx     8648 b- defN 80-Jan-01 00:00 customgpt_client/api/conversations/get_project_conversations.py
 -rw-r--r--  2.0 unx     8015 b- defN 80-Jan-01 00:00 customgpt_client/api/conversations/messages.py
--rw-r--r--  2.0 unx    12279 b- defN 80-Jan-01 00:00 customgpt_client/api/conversations/send_message_to_conversation.py
+-rw-r--r--  2.0 unx    12846 b- defN 80-Jan-01 00:00 customgpt_client/api/conversations/send_message_to_conversation.py
 -rw-r--r--  2.0 unx     7725 b- defN 80-Jan-01 00:00 customgpt_client/api/conversations/update_project_conversation.py
 -rw-r--r--  2.0 unx        0 b- defN 80-Jan-01 00:00 customgpt_client/api/pages/__init__.py
 -rw-r--r--  2.0 unx     6716 b- defN 80-Jan-01 00:00 customgpt_client/api/pages/delete_project_page.py
 -rw-r--r--  2.0 unx     8458 b- defN 80-Jan-01 00:00 customgpt_client/api/pages/get_project_pages.py
 -rw-r--r--  2.0 unx     4706 b- defN 80-Jan-01 00:00 customgpt_client/api/pages/preview.py
 -rw-r--r--  2.0 unx        0 b- defN 80-Jan-01 00:00 customgpt_client/api/project_settings/__init__.py
 -rw-r--r--  2.0 unx     6233 b- defN 80-Jan-01 00:00 customgpt_client/api/project_settings/get_project_settings.py
@@ -368,11 +368,11 @@
 -rw-r--r--  2.0 unx     3189 b- defN 80-Jan-01 00:00 customgpt_client/models/update_user_profile_response_500.py
 -rw-r--r--  2.0 unx     2351 b- defN 80-Jan-01 00:00 customgpt_client/models/update_user_profile_response_500_data.py
 -rw-r--r--  2.0 unx      262 b- defN 80-Jan-01 00:00 customgpt_client/models/update_user_profile_response_500_data_code.py
 -rw-r--r--  2.0 unx      183 b- defN 80-Jan-01 00:00 customgpt_client/models/update_user_profile_response_500_status.py
 -rw-r--r--  2.0 unx     3791 b- defN 80-Jan-01 00:00 customgpt_client/models/user.py
 -rw-r--r--  2.0 unx       25 b- defN 80-Jan-01 00:00 customgpt_client/py.typed
 -rw-r--r--  2.0 unx      993 b- defN 80-Jan-01 00:00 customgpt_client/types.py
--rw-r--r--  2.0 unx     1226 b- defN 80-Jan-01 00:00 customgpt_client-1.1.1.dist-info/METADATA
--rw-r--r--  2.0 unx       88 b- defN 80-Jan-01 00:00 customgpt_client-1.1.1.dist-info/WHEEL
-?rw-r--r--  2.0 unx    44509 b- defN 16-Jan-01 00:00 customgpt_client-1.1.1.dist-info/RECORD
-376 files, 887676 bytes uncompressed, 229372 bytes compressed:  74.2%
+-rw-r--r--  2.0 unx     1226 b- defN 80-Jan-01 00:00 customgpt_client-1.1.2.dist-info/METADATA
+-rw-r--r--  2.0 unx       88 b- defN 80-Jan-01 00:00 customgpt_client-1.1.2.dist-info/WHEEL
+?rw-r--r--  2.0 unx    44509 b- defN 16-Jan-01 00:00 customgpt_client-1.1.2.dist-info/RECORD
+376 files, 888243 bytes uncompressed, 229497 bytes compressed:  74.2%
```

## zipnote {}

```diff
@@ -1113,17 +1113,17 @@
 
 Filename: customgpt_client/py.typed
 Comment: 
 
 Filename: customgpt_client/types.py
 Comment: 
 
-Filename: customgpt_client-1.1.1.dist-info/METADATA
+Filename: customgpt_client-1.1.2.dist-info/METADATA
 Comment: 
 
-Filename: customgpt_client-1.1.1.dist-info/WHEEL
+Filename: customgpt_client-1.1.2.dist-info/WHEEL
 Comment: 
 
-Filename: customgpt_client-1.1.1.dist-info/RECORD
+Filename: customgpt_client-1.1.2.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## customgpt_client/api/conversations/send_message_to_conversation.py

```diff
@@ -1,10 +1,12 @@
 import inspect
+import json
+import re
 from http import HTTPStatus
-from typing import Any, Dict, Generator, Optional, Union
+from typing import Any, Dict, Optional, Union
 
 import httpx
 
 from ... import errors
 from ...models.send_message_to_conversation_json_body import SendMessageToConversationJsonBody
 from ...models.send_message_to_conversation_response_200 import SendMessageToConversationResponse200
 from ...models.send_message_to_conversation_response_401 import SendMessageToConversationResponse401
@@ -148,22 +150,23 @@
         client=client,
         json_body=json_body,
         stream=stream,
         lang=lang,
     )
 
     response = httpx.request(**kwargs)
-
-    lines = response.iter_lines()
-    while True:
-        try:
-            line = next(lines)
-            yield _build_response(client=client, response=response, content=line)
-        except StopIteration:
-            break
+    with httpx.stream(**kwargs) as response:
+        response_text = ""
+        for chunk in response.iter_text():
+            response_text += chunk
+
+        json_objects = re.findall(r"\{.*?\}", response_text)
+        for json_str in json_objects:
+            json_data = json.loads(json_str)
+            yield _build_response(client=client, response=response, content=json_data)
 
 
 async def astream_detailed(
     project_id: int,
     session_id: str,
     *,
     client: {},
@@ -177,72 +180,77 @@
         client=client,
         json_body=json_body,
         stream=stream,
         lang=lang,
     )
     async with httpx.AsyncClient() as client:
         async with client.stream(**kwargs) as response:
-            async for chunk in response.aiter_raw():
-                yield _build_response(client=client, response=response, content=chunk)
+            response_text = ""
+            async for chunk in response.aiter_text():
+                response_text += chunk
+
+            json_objects = re.findall(r"\{.*?\}", response_text)
+            for json_str in json_objects:
+                json_data = json.loads(json_str)
+                yield _build_response(client=client, response=response, content=json_data)
 
 
 def sync_detailed(
     project_id: int,
     session_id: str,
     *,
     client: {},
     json_body: SendMessageToConversationJsonBody,
     stream: Union[Unset, None, bool] = False,
     lang: Union[Unset, None, str] = "en",
 ):
     if stream:
-        return Generator(
-            stream_detailed(
-                project_id=project_id,
-                session_id=session_id,
-                client=client,
-                json_body=json_body,
-                stream=stream,
-                lang=lang,
-            )
+        yield from stream_detailed(
+            project_id=project_id,
+            session_id=session_id,
+            client=client,
+            json_body=json_body,
+            stream=stream,
+            lang=lang,
         )
-    """ Send a message to a conversation.
+    else:
+        """Send a message to a conversation.
 
-     Send a message to a conversation by `projectId` and `sessionId`.
+         Send a message to a conversation by `projectId` and `sessionId`.
 
-    Args:
-        project_id (int):  Example: 1.
-        session_id (str):  Example: 1.
-        stream (Union[Unset, None, bool]):
-        lang (Union[Unset, None, str]):  Default: 'en'.
-        json_body (SendMessageToConversationJsonBody):
+        Args:
+            project_id (int):  Example: 1.
+            session_id (str):  Example: 1.
+            stream (Union[Unset, None, bool]):
+            lang (Union[Unset, None, str]):  Default: 'en'.
+            json_body (SendMessageToConversationJsonBody):
+
+        Raises:
+            errors.UnexpectedStatus: If the server returns an undocumented status code and Client.raise_on_unexpected_status is True.
+            httpx.TimeoutException: If the request takes longer than Client.timeout.
+
+        Returns:
+            Response[Union[SendMessageToConversationResponse200, SendMessageToConversationResponse401, SendMessageToConversationResponse404, SendMessageToConversationResponse500]]
+        """
 
-    Raises:
-        errors.UnexpectedStatus: If the server returns an undocumented status code and Client.raise_on_unexpected_status is True.
-        httpx.TimeoutException: If the request takes longer than Client.timeout.
-
-    Returns:
-        Response[Union[SendMessageToConversationResponse200, SendMessageToConversationResponse401, SendMessageToConversationResponse404, SendMessageToConversationResponse500]]
-     """
-
-    kwargs = _get_kwargs(
-        project_id=project_id,
-        session_id=session_id,
-        client=client,
-        json_body=json_body,
-        stream=stream,
-        lang=lang,
-    )
+        kwargs = _get_kwargs(
+            project_id=project_id,
+            session_id=session_id,
+            client=client,
+            json_body=json_body,
+            stream=stream,
+            lang=lang,
+        )
 
-    response = httpx.request(
-        verify=client.verify_ssl,
-        **kwargs,
-    )
+        response = httpx.request(
+            verify=client.verify_ssl,
+            **kwargs,
+        )
 
-    return _build_response(client=client, response=response)
+        return _build_response(client=client, response=response)
 
 
 def sync(
     project_id: int,
     session_id: str,
     *,
     client: {},
@@ -307,46 +315,47 @@
             project_id=project_id,
             session_id=session_id,
             client=client,
             json_body=json_body,
             stream=stream,
             lang=lang,
         )
-    """ Send a message to a conversation.
-
-     Send a message to a conversation by `projectId` and `sessionId`.
-
-    Args:
-        project_id (int):  Example: 1.
-        session_id (str):  Example: 1.
-        stream (Union[Unset, None, bool]):
-        lang (Union[Unset, None, str]):  Default: 'en'.
-        json_body (SendMessageToConversationJsonBody):
+    else:
+        """Send a message to a conversation.
 
-    Raises:
-        errors.UnexpectedStatus: If the server returns an undocumented status code and Client.raise_on_unexpected_status is True.
-        httpx.TimeoutException: If the request takes longer than Client.timeout.
+         Send a message to a conversation by `projectId` and `sessionId`.
 
-    Returns:
-        Response[Union[SendMessageToConversationResponse200, SendMessageToConversationResponse401, SendMessageToConversationResponse404, SendMessageToConversationResponse500]]
-     """
+        Args:
+            project_id (int):  Example: 1.
+            session_id (str):  Example: 1.
+            stream (Union[Unset, None, bool]):
+            lang (Union[Unset, None, str]):  Default: 'en'.
+            json_body (SendMessageToConversationJsonBody):
+
+        Raises:
+            errors.UnexpectedStatus: If the server returns an undocumented status code and Client.raise_on_unexpected_status is True.
+            httpx.TimeoutException: If the request takes longer than Client.timeout.
+
+        Returns:
+            Response[Union[SendMessageToConversationResponse200, SendMessageToConversationResponse401, SendMessageToConversationResponse404, SendMessageToConversationResponse500]]
+        """
 
-    kwargs = _get_kwargs(
-        project_id=project_id,
-        session_id=session_id,
-        client=client,
-        json_body=json_body,
-        stream=stream,
-        lang=lang,
-    )
+        kwargs = _get_kwargs(
+            project_id=project_id,
+            session_id=session_id,
+            client=client,
+            json_body=json_body,
+            stream=stream,
+            lang=lang,
+        )
 
-    async with httpx.AsyncClient(verify=client.verify_ssl) as _client:
-        response = await _client.request(**kwargs)
+        async with httpx.AsyncClient(verify=client.verify_ssl) as _client:
+            response = await _client.request(**kwargs)
 
-    return _build_response(client=client, response=response)
+        return _build_response(client=client, response=response)
 
 
 async def asyncio(
     project_id: int,
     session_id: str,
     *,
     client: {},
```

## Comparing `customgpt_client-1.1.1.dist-info/METADATA` & `customgpt_client-1.1.2.dist-info/METADATA`

 * *Files 15% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: customgpt-client
-Version: 1.1.1
+Version: 1.1.2
 Summary: A client library for accessing customgpt
 Requires-Python: >=3.8,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
```

## Comparing `customgpt_client-1.1.1.dist-info/RECORD` & `customgpt_client-1.1.2.dist-info/RECORD`

 * *Files 0% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 customgpt_client/api/citations/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
 customgpt_client/api/citations/get_open_graph_data_for_citation.py,sha256=LEqhCbvID3yLZcATz958exB2l_GCbHlqMOGuD7HNTp8,6513
 customgpt_client/api/conversations/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
 customgpt_client/api/conversations/create_project_conversation.py,sha256=JLvtGNfBxHGwLiphetuBbQMzDCwM6r_7OzGu3y525tQ,7370
 customgpt_client/api/conversations/delete_project_conversation.py,sha256=jCoilmEkPFBKCf3aUAFw08oMGHwHjmVAzPIQqYLVqbU,6970
 customgpt_client/api/conversations/get_project_conversations.py,sha256=o4fXGDnZhbHxUK5zXCPNYetYUH1t8RuSf4IoU87k5OE,8648
 customgpt_client/api/conversations/messages.py,sha256=moepVvCLdm87tQgoRq6snDI--FN115qiRrAwcxuQhY0,8015
-customgpt_client/api/conversations/send_message_to_conversation.py,sha256=JgnVtp1-oEGXq9fWz-DvCTVY-EetKXPdU-CtpSZjYcU,12279
+customgpt_client/api/conversations/send_message_to_conversation.py,sha256=_WQO4SKSMc5RdZ0eFQlJKBPYPQZX5sBDRGrG4NLRaMQ,12846
 customgpt_client/api/conversations/update_project_conversation.py,sha256=vEueOTUh86Mz2DfPrAmBC1UBI-9ho7OYTJrYxWZeEoE,7725
 customgpt_client/api/pages/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
 customgpt_client/api/pages/delete_project_page.py,sha256=p0_lLDjGvn8P3Y4vbWSamMYxl7ySxM_HX4-IYnVsK1w,6716
 customgpt_client/api/pages/get_project_pages.py,sha256=FQNZVyRLYe7WGOYeN-MAxxjpld1uuApj-jxrMNne9_g,8458
 customgpt_client/api/pages/preview.py,sha256=f5hCz1niwbG9ysYXfbTW49iiJOVPUmLaduX8pdjzevU,4706
 customgpt_client/api/project_settings/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
 customgpt_client/api/project_settings/get_project_settings.py,sha256=ufuGyw4PWvE1mAYxgZl2022hswaSq62oman6k_RhQzc,6233
@@ -367,10 +367,10 @@
 customgpt_client/models/update_user_profile_response_500.py,sha256=vE_fP4yX8UVMMbO-96_tctsZ8YsdS1D2AF7q5mFsRNk,3189
 customgpt_client/models/update_user_profile_response_500_data.py,sha256=MAg1i8t243owgdIi0NdEPNLAPxypRLrVIiWb_iuSpBc,2351
 customgpt_client/models/update_user_profile_response_500_data_code.py,sha256=o-GDpigGzvI3qFGG1HstdR5Lx5p508fuGNvkauwP9s8,262
 customgpt_client/models/update_user_profile_response_500_status.py,sha256=sX5mpQWL7wNrEpdCiSpvQgsm1f6kaNvLlPmfSkzW-I8,183
 customgpt_client/models/user.py,sha256=Wlz5CcnbrVuJswNviFnkEthU9gCAV8GvPfnEE5DTKhI,3791
 customgpt_client/py.typed,sha256=8ZJUsxZiuOy1oJeVhsTWQhTG_6pTVHVXk5hJL79ebTk,25
 customgpt_client/types.py,sha256=4xaUIOliefW-5jz_p-JT2LO7-V0wKWaniHGtjPBQfvQ,993
-customgpt_client-1.1.1.dist-info/METADATA,sha256=7IJeXKmfgN0aobVZkYMdqqcSBAHPbTsR2UdcKPxr59k,1226
-customgpt_client-1.1.1.dist-info/WHEEL,sha256=Zb28QaM1gQi8f4VCBhsUklF61CTlNYfs9YAZn-TOGFk,88
-customgpt_client-1.1.1.dist-info/RECORD,,
+customgpt_client-1.1.2.dist-info/METADATA,sha256=iyRSM5Ut5mGOJnOvj86mkvWYK4QqdRpO30WTnjdYIzU,1226
+customgpt_client-1.1.2.dist-info/WHEEL,sha256=Zb28QaM1gQi8f4VCBhsUklF61CTlNYfs9YAZn-TOGFk,88
+customgpt_client-1.1.2.dist-info/RECORD,,
```

