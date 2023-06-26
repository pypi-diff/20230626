# Comparing `tmp/otel_tracer-0.0.5-py3-none-any.whl.zip` & `tmp/otel_tracer-0.0.6-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,12 +1,15 @@
-Zip file size: 3624 bytes, number of entries: 10
--rw-r--r--  2.0 unx        0 b- defN 23-Jun-15 03:17 otel_tracer/__init__.py
--rw-r--r--  2.0 unx        0 b- defN 23-Jun-15 03:17 otel_tracer/tracing/__init__.py
--rw-r--r--  2.0 unx     1639 b- defN 23-Jun-15 03:17 otel_tracer/tracing/tracer.py
--rw-r--r--  2.0 unx     2311 b- defN 23-Jun-15 03:17 otel_tracer/tracing/threading_instrumentor/__init__.py
--rw-r--r--  2.0 unx       45 b- defN 23-Jun-15 03:17 otel_tracer/tracing/threading_instrumentor/package.py
--rw-r--r--  2.0 unx       26 b- defN 23-Jun-15 03:17 otel_tracer/tracing/threading_instrumentor/version.py
--rw-r--r--  2.0 unx      670 b- defN 23-Jun-15 03:17 otel_tracer-0.0.5.dist-info/METADATA
--rw-r--r--  2.0 unx       92 b- defN 23-Jun-15 03:17 otel_tracer-0.0.5.dist-info/WHEEL
--rw-r--r--  2.0 unx       12 b- defN 23-Jun-15 03:17 otel_tracer-0.0.5.dist-info/top_level.txt
-?rw-rw-r--  2.0 unx      888 b- defN 23-Jun-15 03:17 otel_tracer-0.0.5.dist-info/RECORD
-10 files, 5683 bytes uncompressed, 2068 bytes compressed:  63.6%
+Zip file size: 4776 bytes, number of entries: 13
+-rw-r--r--  2.0 unx        0 b- defN 23-Jun-26 08:22 otel_tracer/__init__.py
+-rw-r--r--  2.0 unx        0 b- defN 23-Jun-26 08:22 otel_tracer/tracing/__init__.py
+-rw-r--r--  2.0 unx     1744 b- defN 23-Jun-26 08:22 otel_tracer/tracing/tracer.py
+-rw-r--r--  2.0 unx     1524 b- defN 23-Jun-26 08:22 otel_tracer/tracing/queue_instrumentor/__init__.py
+-rw-r--r--  2.0 unx       45 b- defN 23-Jun-26 08:22 otel_tracer/tracing/queue_instrumentor/package.py
+-rw-r--r--  2.0 unx       26 b- defN 23-Jun-26 08:22 otel_tracer/tracing/queue_instrumentor/version.py
+-rw-r--r--  2.0 unx     2311 b- defN 23-Jun-26 08:22 otel_tracer/tracing/threading_instrumentor/__init__.py
+-rw-r--r--  2.0 unx       45 b- defN 23-Jun-26 08:22 otel_tracer/tracing/threading_instrumentor/package.py
+-rw-r--r--  2.0 unx       26 b- defN 23-Jun-26 08:22 otel_tracer/tracing/threading_instrumentor/version.py
+-rw-r--r--  2.0 unx      670 b- defN 23-Jun-26 08:24 otel_tracer-0.0.6.dist-info/METADATA
+-rw-r--r--  2.0 unx       92 b- defN 23-Jun-26 08:24 otel_tracer-0.0.6.dist-info/WHEEL
+-rw-r--r--  2.0 unx       12 b- defN 23-Jun-26 08:24 otel_tracer-0.0.6.dist-info/top_level.txt
+?rw-rw-r--  2.0 unx     1203 b- defN 23-Jun-26 08:24 otel_tracer-0.0.6.dist-info/RECORD
+13 files, 7698 bytes uncompressed, 2696 bytes compressed:  65.0%
```

## zipnote {}

```diff
@@ -3,29 +3,38 @@
 
 Filename: otel_tracer/tracing/__init__.py
 Comment: 
 
 Filename: otel_tracer/tracing/tracer.py
 Comment: 
 
+Filename: otel_tracer/tracing/queue_instrumentor/__init__.py
+Comment: 
+
+Filename: otel_tracer/tracing/queue_instrumentor/package.py
+Comment: 
+
+Filename: otel_tracer/tracing/queue_instrumentor/version.py
+Comment: 
+
 Filename: otel_tracer/tracing/threading_instrumentor/__init__.py
 Comment: 
 
 Filename: otel_tracer/tracing/threading_instrumentor/package.py
 Comment: 
 
 Filename: otel_tracer/tracing/threading_instrumentor/version.py
 Comment: 
 
-Filename: otel_tracer-0.0.5.dist-info/METADATA
+Filename: otel_tracer-0.0.6.dist-info/METADATA
 Comment: 
 
-Filename: otel_tracer-0.0.5.dist-info/WHEEL
+Filename: otel_tracer-0.0.6.dist-info/WHEEL
 Comment: 
 
-Filename: otel_tracer-0.0.5.dist-info/top_level.txt
+Filename: otel_tracer-0.0.6.dist-info/top_level.txt
 Comment: 
 
-Filename: otel_tracer-0.0.5.dist-info/RECORD
+Filename: otel_tracer-0.0.6.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## otel_tracer/tracing/tracer.py

```diff
@@ -7,14 +7,15 @@
 from opentelemetry.instrumentation.redis import RedisInstrumentor
 from opentelemetry.instrumentation.requests import RequestsInstrumentor
 from opentelemetry.sdk.resources import Resource
 from opentelemetry.sdk.trace import TracerProvider
 from opentelemetry.sdk.trace.export import BatchSpanProcessor
 
 from .threading_instrumentor import ThreadingInstrumentor
+from .queue_instrumentor import QueueInstrumentor
 
 
 def init_flask(app, servicename, endpoint):
     FlaskInstrumentor().instrument_app(app)
 
     trace.set_tracer_provider(
         TracerProvider(
@@ -50,7 +51,10 @@
 
 
 def init_pika():
     PikaInstrumentor().instrument()
 
 def init_threading():
     ThreadingInstrumentor().instrument()
+
+def init_queue():
+    QueueInstrumentor().instrument()
```

## Comparing `otel_tracer-0.0.5.dist-info/METADATA` & `otel_tracer-0.0.6.dist-info/METADATA`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: otel-tracer
-Version: 0.0.5
+Version: 0.0.6
 Summary: common python utilities for VxRail
 Home-page: UNKNOWN
 Author: VxRail
 Author-email: UNKNOWN
 License: ToBeDone
 Platform: python3
 Requires-Dist: flask
```

## Comparing `otel_tracer-0.0.5.dist-info/RECORD` & `otel_tracer-0.0.6.dist-info/RECORD`

 * *Files 26% similar despite different names*

```diff
@@ -1,10 +1,13 @@
 otel_tracer/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
 otel_tracer/tracing/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
-otel_tracer/tracing/tracer.py,sha256=OIMDvxMP9CDDqIQfKj9fq8raNvvxY7vfcNmGooXK-nw,1639
+otel_tracer/tracing/tracer.py,sha256=NdPjLbjRFKpsTgQX0u2OgeiCjLmfiyYzZ_5NI5KyKWE,1744
+otel_tracer/tracing/queue_instrumentor/__init__.py,sha256=PEyKfmJa1ihIFTkaZLrAuR7G900znTAP8UJasYftn94,1524
+otel_tracer/tracing/queue_instrumentor/package.py,sha256=wJz15DWx9uQD1CmDQGwybppEIjvBfdvY-DCAFy9APdo,45
+otel_tracer/tracing/queue_instrumentor/version.py,sha256=vF0WxJ9A0bfePfBELWD9nFqFKXxJUgm6PBpoldirS8g,26
 otel_tracer/tracing/threading_instrumentor/__init__.py,sha256=WiDsbWKvP43CJ8H8Q6SrUV4fofZqF7qfLlHbs0fYyMY,2311
 otel_tracer/tracing/threading_instrumentor/package.py,sha256=wJz15DWx9uQD1CmDQGwybppEIjvBfdvY-DCAFy9APdo,45
 otel_tracer/tracing/threading_instrumentor/version.py,sha256=vF0WxJ9A0bfePfBELWD9nFqFKXxJUgm6PBpoldirS8g,26
-otel_tracer-0.0.5.dist-info/METADATA,sha256=NY5yorzRa9FqDxVpw3Z1p7UYWu1oroQv7QeysVKwWlc,670
-otel_tracer-0.0.5.dist-info/WHEEL,sha256=g4nMs7d-Xl9-xC9XovUrsDHGXt-FT0E17Yqo92DEfvY,92
-otel_tracer-0.0.5.dist-info/top_level.txt,sha256=llJBDjZB1BQSEOpLnQesdrfISu_CEXguxypv2CGx0aY,12
-otel_tracer-0.0.5.dist-info/RECORD,,
+otel_tracer-0.0.6.dist-info/METADATA,sha256=BXDNo_5gy42gIZXDaaLXnPH2qfYFxoYexuy3uHCfiZM,670
+otel_tracer-0.0.6.dist-info/WHEEL,sha256=g4nMs7d-Xl9-xC9XovUrsDHGXt-FT0E17Yqo92DEfvY,92
+otel_tracer-0.0.6.dist-info/top_level.txt,sha256=llJBDjZB1BQSEOpLnQesdrfISu_CEXguxypv2CGx0aY,12
+otel_tracer-0.0.6.dist-info/RECORD,,
```

