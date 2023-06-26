# Comparing `tmp/highlight_io-0.5.1.tar.gz` & `tmp/highlight_io-0.5.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "highlight_io-0.5.1.tar", max compression
+gzip compressed data, was "highlight_io-0.5.2.tar", max compression
```

## Comparing `highlight_io-0.5.1.tar` & `highlight_io-0.5.2.tar`

### file list

```diff
@@ -1,13 +1,13 @@
--rw-r--r--   0        0        0      350 2023-06-23 19:53:45.556355 highlight_io-0.5.1/README.md
--rw-r--r--   0        0        0       64 2023-06-23 19:53:45.556355 highlight_io-0.5.1/highlight_io/__init__.py
--rw-r--r--   0        0        0      155 2023-06-23 19:53:45.556355 highlight_io-0.5.1/highlight_io/integrations/__init__.py
--rw-r--r--   0        0        0      717 2023-06-23 19:53:45.556355 highlight_io-0.5.1/highlight_io/integrations/aws.py
--rw-r--r--   0        0        0      740 2023-06-23 19:53:45.556355 highlight_io-0.5.1/highlight_io/integrations/azure.py
--rw-r--r--   0        0        0     1631 2023-06-23 19:53:45.556355 highlight_io-0.5.1/highlight_io/integrations/django.py
--rw-r--r--   0        0        0      722 2023-06-23 19:53:45.556355 highlight_io-0.5.1/highlight_io/integrations/fastapi.py
--rw-r--r--   0        0        0     1519 2023-06-23 19:53:45.556355 highlight_io-0.5.1/highlight_io/integrations/flask.py
--rw-r--r--   0        0        0      747 2023-06-23 19:53:45.556355 highlight_io-0.5.1/highlight_io/integrations/gcp.py
--rw-r--r--   0        0        0     1072 2023-06-23 19:53:45.556355 highlight_io-0.5.1/highlight_io/integrations/serverless.py
--rw-r--r--   0        0        0     8916 2023-06-23 19:53:45.556355 highlight_io-0.5.1/highlight_io/sdk.py
--rw-r--r--   0        0        0     1716 2023-06-23 19:53:45.560356 highlight_io-0.5.1/pyproject.toml
--rw-r--r--   0        0        0     2118 1970-01-01 00:00:00.000000 highlight_io-0.5.1/PKG-INFO
+-rw-r--r--   0        0        0      350 2023-06-26 17:12:11.141541 highlight_io-0.5.2/README.md
+-rw-r--r--   0        0        0       64 2023-06-26 17:12:11.141541 highlight_io-0.5.2/highlight_io/__init__.py
+-rw-r--r--   0        0        0      155 2023-06-26 17:12:11.141541 highlight_io-0.5.2/highlight_io/integrations/__init__.py
+-rw-r--r--   0        0        0      717 2023-06-26 17:12:11.141541 highlight_io-0.5.2/highlight_io/integrations/aws.py
+-rw-r--r--   0        0        0      740 2023-06-26 17:12:11.141541 highlight_io-0.5.2/highlight_io/integrations/azure.py
+-rw-r--r--   0        0        0     1631 2023-06-26 17:12:11.141541 highlight_io-0.5.2/highlight_io/integrations/django.py
+-rw-r--r--   0        0        0     1799 2023-06-26 17:12:11.141541 highlight_io-0.5.2/highlight_io/integrations/fastapi.py
+-rw-r--r--   0        0        0     1519 2023-06-26 17:12:11.141541 highlight_io-0.5.2/highlight_io/integrations/flask.py
+-rw-r--r--   0        0        0      747 2023-06-26 17:12:11.141541 highlight_io-0.5.2/highlight_io/integrations/gcp.py
+-rw-r--r--   0        0        0     1072 2023-06-26 17:12:11.141541 highlight_io-0.5.2/highlight_io/integrations/serverless.py
+-rw-r--r--   0        0        0    11253 2023-06-26 17:12:11.141541 highlight_io-0.5.2/highlight_io/sdk.py
+-rw-r--r--   0        0        0     1716 2023-06-26 17:12:11.141541 highlight_io-0.5.2/pyproject.toml
+-rw-r--r--   0        0        0     2118 1970-01-01 00:00:00.000000 highlight_io-0.5.2/PKG-INFO
```

### Comparing `highlight_io-0.5.1/highlight_io/integrations/aws.py` & `highlight_io-0.5.2/highlight_io/integrations/aws.py`

 * *Files identical despite different names*

### Comparing `highlight_io-0.5.1/highlight_io/integrations/azure.py` & `highlight_io-0.5.2/highlight_io/integrations/azure.py`

 * *Files identical despite different names*

### Comparing `highlight_io-0.5.1/highlight_io/integrations/django.py` & `highlight_io-0.5.2/highlight_io/integrations/django.py`

 * *Files identical despite different names*

### Comparing `highlight_io-0.5.1/highlight_io/integrations/flask.py` & `highlight_io-0.5.2/highlight_io/integrations/flask.py`

 * *Files identical despite different names*

### Comparing `highlight_io-0.5.1/highlight_io/integrations/gcp.py` & `highlight_io-0.5.2/highlight_io/integrations/gcp.py`

 * *Files identical despite different names*

### Comparing `highlight_io-0.5.1/highlight_io/integrations/serverless.py` & `highlight_io-0.5.2/highlight_io/integrations/serverless.py`

 * *Files identical despite different names*

### Comparing `highlight_io-0.5.1/highlight_io/sdk.py` & `highlight_io-0.5.2/highlight_io/sdk.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,9 +1,12 @@
 import contextlib
+import http
+import json
 import logging
+import traceback
 import typing
 
 from opentelemetry import trace, _logs
 from opentelemetry._logs.severity import std_to_otel
 from opentelemetry.exporter.otlp.proto.http import Compression
 from opentelemetry.exporter.otlp.proto.http._log_exporter import OTLPLogExporter
 from opentelemetry.exporter.otlp.proto.http.trace_exporter import OTLPSpanExporter
@@ -145,14 +148,78 @@
             try:
                 yield span
             except Exception as e:
                 self.record_exception(e)
                 raise
 
     @staticmethod
+    def record_http_error(
+        status_code: int, detail: str, headers: typing.Dict[str, str]
+    ) -> None:
+        """
+        Record an http error from your app.
+
+        Example:
+            from fastapi import FastAPI, Request, HTTPException, APIRouter
+            import highlight_io
+
+            H = highlight_io.H('project_id', ...)
+
+            app = FastAPI()
+            app.add_middleware(FastAPIMiddleware)
+
+            router = APIRouter()
+
+
+            @router.get("/health")
+            def health_check():
+                with H.trace(session_id, request_id):
+                    logging.info('hello, world!')
+                    H.record_http_error(status_code=404)
+                    raise HTTPException(status_code=404, detail="Item not found")
+
+
+        :param status_code: the http status code to report
+        :param detail: the error status details
+        :param headers: the headers of the http request
+        :return: None
+        """
+        span = trace.get_current_span()
+        if not span:
+            raise RuntimeError("H.record_http_error called without a span context")
+
+        # try load json of the form `{"detail":"Item not found"}`
+        try:
+            body = json.loads(detail)
+            if "detail" in body:
+                detail = body["detail"]
+        except ValueError:
+            pass
+
+        if not detail:
+            detail = http.HTTPStatus(status_code).phrase
+
+        # we cannot use `span.record_exception()` here because that uses `traceback.format_exc()` which
+        # relies there being an exception raised. we manually `traceback.format_stack()` to get the current
+        # execution stack for recording an http exception.
+        attributes = {
+            "exception.type": "HTTPException",
+            "exception.message": detail,
+            "exception.stacktrace": "".join(traceback.format_stack()),
+            "http.status_code": status_code,
+        }
+        for k, v in headers.items():
+            if type(v) in [bool, str, bytes, int, float]:
+                attributes[f"http.headers.{k}"] = v
+        span.add_event(name="exception", attributes=attributes)
+        logging.exception(
+            f"Highlight caught an http error (status_code={status_code}, detail={detail})"
+        )
+
+    @staticmethod
     def record_exception(e: Exception) -> None:
         """
         Record arbitrary exceptions raised within your app.
 
         Example:
             import highlight_io
             H = highlight_io.H('project_id', ...)
```

### Comparing `highlight_io-0.5.1/pyproject.toml` & `highlight_io-0.5.2/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "highlight-io"
-version = "0.5.1"
+version = "0.5.2"
 description = "Session replay and error monitoring: stop guessing why bugs happen!"
 license = "Apache-2.0"
 authors = [
     "Vadim Korolik <vadim@highlight.io>",
     "Jay Khatri <jay@highlight.io>",
 ]
 readme = "README.md"
```

### Comparing `highlight_io-0.5.1/PKG-INFO` & `highlight_io-0.5.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: highlight-io
-Version: 0.5.1
+Version: 0.5.2
 Summary: Session replay and error monitoring: stop guessing why bugs happen!
 Home-page: https://www.highlight.io
 License: Apache-2.0
 Keywords: web,framework
 Author: Vadim Korolik
 Author-email: vadim@highlight.io
 Requires-Python: >=3.8,<4.0
```

