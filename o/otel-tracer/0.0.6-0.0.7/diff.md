# Comparing `tmp/otel_tracer-0.0.6-py3-none-any.whl.zip` & `tmp/otel_tracer-0.0.7-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,15 +1,15 @@
-Zip file size: 4776 bytes, number of entries: 13
--rw-r--r--  2.0 unx        0 b- defN 23-Jun-26 08:22 otel_tracer/__init__.py
--rw-r--r--  2.0 unx        0 b- defN 23-Jun-26 08:22 otel_tracer/tracing/__init__.py
--rw-r--r--  2.0 unx     1744 b- defN 23-Jun-26 08:22 otel_tracer/tracing/tracer.py
--rw-r--r--  2.0 unx     1524 b- defN 23-Jun-26 08:22 otel_tracer/tracing/queue_instrumentor/__init__.py
--rw-r--r--  2.0 unx       45 b- defN 23-Jun-26 08:22 otel_tracer/tracing/queue_instrumentor/package.py
--rw-r--r--  2.0 unx       26 b- defN 23-Jun-26 08:22 otel_tracer/tracing/queue_instrumentor/version.py
--rw-r--r--  2.0 unx     2311 b- defN 23-Jun-26 08:22 otel_tracer/tracing/threading_instrumentor/__init__.py
--rw-r--r--  2.0 unx       45 b- defN 23-Jun-26 08:22 otel_tracer/tracing/threading_instrumentor/package.py
--rw-r--r--  2.0 unx       26 b- defN 23-Jun-26 08:22 otel_tracer/tracing/threading_instrumentor/version.py
--rw-r--r--  2.0 unx      670 b- defN 23-Jun-26 08:24 otel_tracer-0.0.6.dist-info/METADATA
--rw-r--r--  2.0 unx       92 b- defN 23-Jun-26 08:24 otel_tracer-0.0.6.dist-info/WHEEL
--rw-r--r--  2.0 unx       12 b- defN 23-Jun-26 08:24 otel_tracer-0.0.6.dist-info/top_level.txt
-?rw-rw-r--  2.0 unx     1203 b- defN 23-Jun-26 08:24 otel_tracer-0.0.6.dist-info/RECORD
-13 files, 7698 bytes uncompressed, 2696 bytes compressed:  65.0%
+Zip file size: 4915 bytes, number of entries: 13
+-rw-r--r--  2.0 unx        0 b- defN 23-Jun-26 08:47 otel_tracer/__init__.py
+-rw-r--r--  2.0 unx        0 b- defN 23-Jun-26 08:47 otel_tracer/tracing/__init__.py
+-rw-r--r--  2.0 unx     1744 b- defN 23-Jun-26 08:47 otel_tracer/tracing/tracer.py
+-rw-r--r--  2.0 unx     1946 b- defN 23-Jun-26 08:47 otel_tracer/tracing/queue_instrumentor/__init__.py
+-rw-r--r--  2.0 unx       45 b- defN 23-Jun-26 08:47 otel_tracer/tracing/queue_instrumentor/package.py
+-rw-r--r--  2.0 unx       26 b- defN 23-Jun-26 08:47 otel_tracer/tracing/queue_instrumentor/version.py
+-rw-r--r--  2.0 unx     2311 b- defN 23-Jun-26 08:47 otel_tracer/tracing/threading_instrumentor/__init__.py
+-rw-r--r--  2.0 unx       45 b- defN 23-Jun-26 08:47 otel_tracer/tracing/threading_instrumentor/package.py
+-rw-r--r--  2.0 unx       26 b- defN 23-Jun-26 08:47 otel_tracer/tracing/threading_instrumentor/version.py
+-rw-r--r--  2.0 unx      670 b- defN 23-Jun-26 08:47 otel_tracer-0.0.7.dist-info/METADATA
+-rw-r--r--  2.0 unx       92 b- defN 23-Jun-26 08:47 otel_tracer-0.0.7.dist-info/WHEEL
+-rw-r--r--  2.0 unx       12 b- defN 23-Jun-26 08:47 otel_tracer-0.0.7.dist-info/top_level.txt
+?rw-rw-r--  2.0 unx     1203 b- defN 23-Jun-26 08:47 otel_tracer-0.0.7.dist-info/RECORD
+13 files, 8120 bytes uncompressed, 2835 bytes compressed:  65.1%
```

## zipnote {}

```diff
@@ -21,20 +21,20 @@
 
 Filename: otel_tracer/tracing/threading_instrumentor/package.py
 Comment: 
 
 Filename: otel_tracer/tracing/threading_instrumentor/version.py
 Comment: 
 
-Filename: otel_tracer-0.0.6.dist-info/METADATA
+Filename: otel_tracer-0.0.7.dist-info/METADATA
 Comment: 
 
-Filename: otel_tracer-0.0.6.dist-info/WHEEL
+Filename: otel_tracer-0.0.7.dist-info/WHEEL
 Comment: 
 
-Filename: otel_tracer-0.0.6.dist-info/top_level.txt
+Filename: otel_tracer-0.0.7.dist-info/top_level.txt
 Comment: 
 
-Filename: otel_tracer-0.0.6.dist-info/RECORD
+Filename: otel_tracer-0.0.7.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## otel_tracer/tracing/queue_instrumentor/__init__.py

```diff
@@ -1,33 +1,43 @@
 import queue
 from typing import Collection
 from opentelemetry import context, trace
+from opentelemetry.context import attach, detach
 from opentelemetry.instrumentation.instrumentor import BaseInstrumentor
 from opentelemetry.trace import get_current_span, get_tracer, get_tracer_provider
 
 from .package import _instruments
 from .version import __version__
 
 
 class _InstrumentedQueue(queue.Queue):
     def __init__(self, *args, **kwargs):
         super().__init__(*args, **kwargs)
-        self._parent_span = None
+        self._tracer = get_tracer(__name__, __version__)
 
     def put(self, item, *args, **kwargs):
-        with self._tracer.start_as_current_span("Queue put"):
-            self._parent_span = get_current_span()
-            super().put(item, *args, **kwargs)
+        item["_parent_span"] = get_current_span()
+        super().put(item, *args, **kwargs)
 
     def get(self, *args, **kwargs):
-        parent_span = self._parent_span or get_current_span()
-        ctx = trace.set_span_in_context(parent_span)
-        context.attach(ctx)
-        with self._tracer.start_as_current_span("Queue get"):
-            return super().get(*args, **kwargs)
+        item = super().get(*args, **kwargs)
+
+        # Start a new span for the get operation
+        with self._tracer.start_as_current_span("queue.get") as span:
+            # Get the parent span context from the item, if it exists
+            parent_span = item.get("_parent_span")
+            if parent_span is not None:
+                # Set the parent span context for this thread
+                ctx = trace.set_span_in_context(parent_span)
+                token = attach(ctx)
+                try:
+                    # Call the original function
+                    return super().get(*args, **kwargs)
+                finally:
+                    detach(token)
 
 
 class QueueInstrumentor(BaseInstrumentor):
     original_queuecls = queue.Queue
 
     def instrumentation_dependencies(self) -> Collection[str]:
         return _instruments
```

## Comparing `otel_tracer-0.0.6.dist-info/RECORD` & `otel_tracer-0.0.7.dist-info/RECORD`

 * *Files 13% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 otel_tracer/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
 otel_tracer/tracing/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
 otel_tracer/tracing/tracer.py,sha256=NdPjLbjRFKpsTgQX0u2OgeiCjLmfiyYzZ_5NI5KyKWE,1744
-otel_tracer/tracing/queue_instrumentor/__init__.py,sha256=PEyKfmJa1ihIFTkaZLrAuR7G900znTAP8UJasYftn94,1524
+otel_tracer/tracing/queue_instrumentor/__init__.py,sha256=6FgjutGVTLB4BaKXzKjDAMtDFWlsjaHeR33wQkmqp7g,1946
 otel_tracer/tracing/queue_instrumentor/package.py,sha256=wJz15DWx9uQD1CmDQGwybppEIjvBfdvY-DCAFy9APdo,45
 otel_tracer/tracing/queue_instrumentor/version.py,sha256=vF0WxJ9A0bfePfBELWD9nFqFKXxJUgm6PBpoldirS8g,26
 otel_tracer/tracing/threading_instrumentor/__init__.py,sha256=WiDsbWKvP43CJ8H8Q6SrUV4fofZqF7qfLlHbs0fYyMY,2311
 otel_tracer/tracing/threading_instrumentor/package.py,sha256=wJz15DWx9uQD1CmDQGwybppEIjvBfdvY-DCAFy9APdo,45
 otel_tracer/tracing/threading_instrumentor/version.py,sha256=vF0WxJ9A0bfePfBELWD9nFqFKXxJUgm6PBpoldirS8g,26
-otel_tracer-0.0.6.dist-info/METADATA,sha256=BXDNo_5gy42gIZXDaaLXnPH2qfYFxoYexuy3uHCfiZM,670
-otel_tracer-0.0.6.dist-info/WHEEL,sha256=g4nMs7d-Xl9-xC9XovUrsDHGXt-FT0E17Yqo92DEfvY,92
-otel_tracer-0.0.6.dist-info/top_level.txt,sha256=llJBDjZB1BQSEOpLnQesdrfISu_CEXguxypv2CGx0aY,12
-otel_tracer-0.0.6.dist-info/RECORD,,
+otel_tracer-0.0.7.dist-info/METADATA,sha256=I6jTzpe4ZFwZywsGfUi9ha-AEcpCydiTOdSLm9lPP04,670
+otel_tracer-0.0.7.dist-info/WHEEL,sha256=g4nMs7d-Xl9-xC9XovUrsDHGXt-FT0E17Yqo92DEfvY,92
+otel_tracer-0.0.7.dist-info/top_level.txt,sha256=llJBDjZB1BQSEOpLnQesdrfISu_CEXguxypv2CGx0aY,12
+otel_tracer-0.0.7.dist-info/RECORD,,
```

