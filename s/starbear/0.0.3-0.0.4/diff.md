# Comparing `tmp/starbear-0.0.3.tar.gz` & `tmp/starbear-0.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "starbear-0.0.3.tar", max compression
+gzip compressed data, was "starbear-0.0.4.tar", max compression
```

## Comparing `starbear-0.0.3.tar` & `starbear-0.0.4.tar`

### file list

```diff
@@ -1,11 +1,11 @@
--rw-r--r--   0        0        0      786 2023-05-31 17:00:55.345292 starbear-0.0.3/pyproject.toml
--rw-r--r--   0        0        0       95 2023-01-22 18:07:37.078561 starbear-0.0.3/starbear/__init__.py
--rw-r--r--   0        0        0     4988 2023-05-31 16:06:31.359436 starbear-0.0.3/starbear/base-lib.js
--rw-r--r--   0        0        0      552 2023-01-22 20:51:07.514209 starbear-0.0.3/starbear/base-template.html
--rw-r--r--   0        0        0     5075 2023-05-31 17:00:43.309664 starbear-0.0.3/starbear/page.py
--rw-r--r--   0        0        0     6759 2023-01-22 18:36:53.392128 starbear-0.0.3/starbear/repr.py
--rw-r--r--   0        0        0     9683 2023-05-31 17:00:43.309894 starbear-0.0.3/starbear/serve.py
--rw-r--r--   0        0        0     2525 2023-01-23 07:23:44.113526 starbear-0.0.3/starbear/utils.py
--rw-r--r--   0        0        0       18 2023-05-31 17:00:55.378845 starbear-0.0.3/starbear/version.py
--rw-r--r--   0        0        0      731 1970-01-01 00:00:00.000000 starbear-0.0.3/setup.py
--rw-r--r--   0        0        0      628 1970-01-01 00:00:00.000000 starbear-0.0.3/PKG-INFO
+-rw-r--r--   0        0        0      786 2023-06-26 19:37:39.133159 starbear-0.0.4/pyproject.toml
+-rw-r--r--   0        0        0       95 2023-01-22 18:07:37.078561 starbear-0.0.4/starbear/__init__.py
+-rw-r--r--   0        0        0     4988 2023-05-31 16:06:31.359436 starbear-0.0.4/starbear/base-lib.js
+-rw-r--r--   0        0        0      552 2023-01-22 20:51:07.514209 starbear-0.0.4/starbear/base-template.html
+-rw-r--r--   0        0        0     5126 2023-06-08 20:37:34.926744 starbear-0.0.4/starbear/page.py
+-rw-r--r--   0        0        0     6759 2023-01-22 18:36:53.392128 starbear-0.0.4/starbear/repr.py
+-rw-r--r--   0        0        0    10916 2023-06-26 19:28:58.244359 starbear-0.0.4/starbear/serve.py
+-rw-r--r--   0        0        0     2525 2023-01-23 07:23:44.113526 starbear-0.0.4/starbear/utils.py
+-rw-r--r--   0        0        0       18 2023-06-26 19:37:39.166090 starbear-0.0.4/starbear/version.py
+-rw-r--r--   0        0        0      731 1970-01-01 00:00:00.000000 starbear-0.0.4/setup.py
+-rw-r--r--   0        0        0      628 1970-01-01 00:00:00.000000 starbear-0.0.4/PKG-INFO
```

### Comparing `starbear-0.0.3/pyproject.toml` & `starbear-0.0.4/pyproject.toml`

 * *Files 15% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "starbear"
-version = "0.0.3"
+version = "0.0.4"
 description = "Framework for easy small local web apps or programs"
 authors = ["Olivier Breuleux <breuleux@gmail.com>"]
 license = "MIT"
 
 [tool.poetry.dependencies]
 python = "^3.9"
 uvicorn = "^0.17.6"
```

### Comparing `starbear-0.0.3/starbear/base-lib.js` & `starbear-0.0.4/starbear/base-lib.js`

 * *Files identical despite different names*

### Comparing `starbear-0.0.3/starbear/base-template.html` & `starbear-0.0.4/starbear/base-template.html`

 * *Files identical despite different names*

### Comparing `starbear-0.0.3/starbear/page.py` & `starbear-0.0.4/starbear/page.py`

 * *Files 5% similar despite different names*

```diff
@@ -9,21 +9,23 @@
     def __init__(
         self,
         iq,
         oq,
         representer,
         selector=None,
         query_params={},
+        session={},
         track_history=True,
         sent_resources=None,
     ):
         self.iq = iq
         self.oq = oq
         self.selector = selector
         self.query_params = query_params
+        self.session = session
         self.representer = representer
         self.track_history = track_history
         self.sent_resources = sent_resources or ResourceDeduplicator()
         self.tasks = set()
         self.js = JavaScriptOperation(self, [])
 
     def __getitem__(self, selector):
```

### Comparing `starbear-0.0.3/starbear/repr.py` & `starbear-0.0.4/starbear/repr.py`

 * *Files identical despite different names*

### Comparing `starbear-0.0.3/starbear/serve.py` & `starbear-0.0.4/starbear/serve.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,34 +1,36 @@
 import asyncio as aio
 import base64
 import inspect
 import json
 import traceback
 from functools import wraps
+from itertools import count
 from pathlib import Path
 from uuid import uuid4 as uuid
 
 from hrepr import Tag
 from starlette.exceptions import HTTPException
 from starlette.responses import (
     FileResponse,
     HTMLResponse,
     JSONResponse,
     RedirectResponse,
     Response,
 )
-from starlette.routing import Mount, Route, WebSocketRoute
+from starlette.routing import Route, WebSocketRoute
 from starlette.websockets import WebSocketDisconnect
 
 from .page import Page
 from .repr import Representer
 from .utils import keyword_decorator
 
 here = Path(__file__).parent
 
+_count = count()
 
 construct = {}
 
 
 def register_constructor(key):
     def deco(fn):
         construct[key] = fn
@@ -47,42 +49,46 @@
         self._queue.appendleft(entry)
         self._unfinished_tasks += 1
         self._finished.clear()
         self._wakeup_next(self._getters)
 
 
 class Cub:
-    def __init__(self, mother, session, query_params={}):
+    def __init__(self, mother, process, query_params={}, session={}):
         self.mother = mother
         self.fn = mother.fn
-        self.path = mother.path
-        self.session = session
+        self.process = process
         self.query_params = query_params
-        self.route = f"{self.path}/{self.session}"
+        self.session = session
+        self.route = self.mother.path_for("main", process=self.process).rstrip("/")
         self.methods = {}
         self.representer = Representer(self.route)
         self.iq = aio.Queue()
         self.oq = Queue2()
         self.history = []
         self.reset = False
         self.ws = None
         self.page = Page(
-            self.iq, self.oq, representer=self.representer, query_params=query_params
+            self.iq,
+            self.oq,
+            representer=self.representer,
+            query_params=query_params,
+            session=session,
         )
         self.coro = aio.create_task(self.run())
         self._sd_coro = None
 
     def schedule_selfdestruct(self):
         async def sd():
-            await aio.sleep(self.mother.session_timeout)
-            del self.mother.cubs[self.session]
+            await aio.sleep(self.mother.process_timeout)
+            del self.mother.cubs[self.process]
             self.coro.cancel()
-            print(f"Destroyed session: {self.session}")
+            print(f"Destroyed process: {self.process}")
 
-        if self.mother.session_timeout is not None:
+        if self.mother.process_timeout is not None:
             self._sd_coro = aio.create_task(sd())
 
     def unschedule_selfdestruct(self):
         if self._sd_coro:
             self._sd_coro.cancel()
             self._sd_coro = None
 
@@ -190,123 +196,158 @@
         self.representer.queue_registry.put(
             qid=data["reqid"],
             value=data["value"],
         )
         return JSONResponse({"status": "ok"})
 
 
-def get_session_from_request(request):
-    session_base = request.path_params.get("session", None)
-    if session_base is None:
-        session_base = base64.urlsafe_b64encode(uuid().bytes).decode("utf8").strip("=")
-    return session_base
+def get_process_from_request(request):
+    process_base = request.path_params.get("process", None)
+    if process_base is None:
+        process_base = base64.urlsafe_b64encode(uuid().bytes).decode("utf8").strip("=")
+    return process_base
 
 
 def forward_cub(fn):
     @wraps(fn)
     async def fwd(self, request):
-        session = get_session_from_request(request)
-        cub = self._get(session, query_params=request.query_params)
+        process = get_process_from_request(request)
+        cub = self._get(process, query_params=request.query_params)
         if cub is None:
-            print(f"Trying to access missing session: {session}")
-            return JSONResponse({"missing": session}, status_code=404)
+            print(f"Trying to access missing process: {process}")
+            return JSONResponse({"missing": process}, status_code=404)
         else:
             return await fn(self, request, cub)
 
     return fwd
 
 
 class MotherBear:
-    def __init__(self, fn, path, session_timeout=60, hide_sessions=True):
+    def __init__(self, fn, process_timeout=60, hide_processes=True):
         self.fn = fn
-        self.path = path.rstrip("/")
-        self.session_timeout = session_timeout
-        self.hide_sessions = hide_sessions
+        self.router = None
+        self.process_timeout = process_timeout
+        self.hide_processes = hide_processes
         self.cubs = {}
+        self.appid = next(_count)
 
-    def _get(self, sess, query_params={}, ensure=False):
-        if sess not in self.cubs:
+    def _get(self, proc, query_params={}, session={}, ensure=False):
+        if proc not in self.cubs:
             if ensure:
-                print(f"Creating session: {sess}")
-                self.cubs[sess] = Cub(self, sess, query_params=query_params)
+                print(f"Creating process: {proc}")
+                self.cubs[proc] = Cub(
+                    self, proc, query_params=query_params, session=session
+                )
             else:
                 return None
-        return self.cubs[sess]
+        return self.cubs[proc]
+
+    def path_for(self, name, **kwargs):
+        return self.router.url_path_for(self._mangle(name), **kwargs)
+
+    def _ensure_router(self, request):
+        router = request.scope["router"]
+        if self.router is None:
+            self.router = router
+        else:
+            assert self.router is router
 
     async def route_dispatch(self, request):
-        session = get_session_from_request(request)
-        if self.hide_sessions:
+        self._ensure_router(request)
+        process = get_process_from_request(request)
+        main_path = self.path_for("main", process=process)
+        if self.hide_processes:
+            try:
+                session = request.session
+            except AssertionError:
+                session = {}
             return await self._get(
-                session, query_params=request.query_params, ensure=True
+                process, query_params=request.query_params, session=session, ensure=True
             ).route_main(request)
         else:
-            url = f"{self.path}/{session}"
+            url = main_path
             if request.query_params:
                 url = f"{url}?{request.query_params}"
             return RedirectResponse(url=url)
 
     async def route_main(self, request):
-        session = get_session_from_request(request)
+        self._ensure_router(request)
+        process = get_process_from_request(request)
         return await self._get(
-            session, query_params=request.query_params, ensure=True
+            process, query_params=request.query_params, ensure=True
         ).route_main(request)
 
     @forward_cub
     async def route_socket(self, ws, cub):
+        self._ensure_router(ws)
         return await cub.route_socket(ws)
 
     @forward_cub
     async def route_method(self, request, cub):
+        self._ensure_router(request)
         return await cub.route_method(request)
 
     @forward_cub
     async def route_file(self, request, cub):
+        self._ensure_router(request)
         pth = cub.representer.file_registry.get_file_from_url(
             request.path_params["path"]
         )
         if pth is None:
             raise HTTPException(
                 status_code=404, detail="File not found or not available."
             )
         return FileResponse(pth, headers={"Cache-Control": "no-cache"})
 
     @forward_cub
     async def route_vfile(self, request, cub):
+        self._ensure_router(request)
         vf = cub.representer.vfile_registry.get(request.path_params["path"])
         return Response(content=vf.content, media_type=vf.type)
 
     @forward_cub
     async def route_post(self, request, cub):
+        self._ensure_router(request)
         return await cub.route_post(request)
 
     @forward_cub
     async def route_queue(self, request, cub):
+        self._ensure_router(request)
         return await cub.route_queue(request)
 
     async def route_static(self, request):
+        self._ensure_router(request)
         pth = here / request.path_params["path"]
         return FileResponse(pth, headers={"Cache-Control": "no-cache"})
 
-    def routes(self):
-        return Mount(
-            self.path,
-            routes=[
-                Route("/", self.route_dispatch),
-                Route("/{session:str}/static/{path:path}", self.route_static),
-                Route("/{session:str}/", self.route_main),
-                Route(
-                    "/{session:str}/method/{method:int}",
-                    self.route_method,
-                    methods=["GET", "POST"],
-                ),
-                Route("/{session:str}/file/{path:path}", self.route_file),
-                Route("/{session:str}/vfile/{path:path}", self.route_vfile),
-                Route("/{session:str}/post", self.route_post, methods=["POST"]),
-                Route("/{session:str}/queue", self.route_queue, methods=["POST"]),
-                WebSocketRoute("/{session:str}/socket", self.route_socket),
-            ],
+    def _mangle(self, name):
+        return f"app{self.appid}_{name}"
+
+    def _make_route(self, name, path, cls=Route, **kwargs):
+        return cls(
+            path,
+            getattr(self, f"route_{name}"),
+            name=self._mangle(name),
+            **kwargs,
         )
 
+    def routes(self):
+        return [
+            self._make_route("dispatch", "/"),
+            self._make_route("static", "/{process:str}/static/{path:path}"),
+            self._make_route("main", "/{process:str}/"),
+            self._make_route(
+                "method",
+                "/{process:str}/method/{method:int}",
+                methods=["GET", "POST"],
+            ),
+            self._make_route("file", "/{process:str}/file/{path:path}"),
+            self._make_route("vfile", "/{process:str}/vfile/{path:path}"),
+            self._make_route("post", "/{process:str}/post", methods=["POST"]),
+            self._make_route("queue", "/{process:str}/queue", methods=["POST"]),
+            self._make_route("socket", "/{process:str}/socket", cls=WebSocketRoute),
+        ]
+
 
 @keyword_decorator
-def bear(fn, path="", **kwargs):
-    return MotherBear(fn, path, **kwargs).routes()
+def bear(fn, **kwargs):
+    return MotherBear(fn, **kwargs)
```

### Comparing `starbear-0.0.3/starbear/utils.py` & `starbear-0.0.4/starbear/utils.py`

 * *Files identical despite different names*

### Comparing `starbear-0.0.3/setup.py` & `starbear-0.0.4/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -11,15 +11,15 @@
 ['hrepr>=0.5.0,<0.6.0',
  'starlette>=0.20.3,<0.21.0',
  'uvicorn>=0.17.6,<0.18.0',
  'websockets>=10.3,<11.0']
 
 setup_kwargs = {
     'name': 'starbear',
-    'version': '0.0.3',
+    'version': '0.0.4',
     'description': 'Framework for easy small local web apps or programs',
     'long_description': 'None',
     'author': 'Olivier Breuleux',
     'author_email': 'breuleux@gmail.com',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'None',
```

### Comparing `starbear-0.0.3/PKG-INFO` & `starbear-0.0.4/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: starbear
-Version: 0.0.3
+Version: 0.0.4
 Summary: Framework for easy small local web apps or programs
 License: MIT
 Author: Olivier Breuleux
 Author-email: breuleux@gmail.com
 Requires-Python: >=3.9,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
```

