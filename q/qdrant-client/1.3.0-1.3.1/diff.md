# Comparing `tmp/qdrant_client-1.3.0.tar.gz` & `tmp/qdrant_client-1.3.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "qdrant_client-1.3.0.tar", max compression
+gzip compressed data, was "qdrant_client-1.3.1.tar", max compression
```

## Comparing `qdrant_client-1.3.0.tar` & `qdrant_client-1.3.1.tar`

### file list

```diff
@@ -1,70 +1,70 @@
--rw-r--r--   0        0        0    11357 2023-06-23 13:38:56.175043 qdrant_client-1.3.0/LICENSE
--rw-r--r--   0        0        0     6250 2023-06-23 13:38:56.175043 qdrant_client-1.3.0/README.md
--rw-r--r--   0        0        0     1417 2023-06-23 13:38:56.179044 qdrant_client-1.3.0/pyproject.toml
--rw-r--r--   0        0        0       56 2023-06-23 13:38:56.179044 qdrant_client-1.3.0/qdrant_client/__init__.py
--rw-r--r--   0        0        0    10034 2023-06-23 13:38:56.179044 qdrant_client-1.3.0/qdrant_client/client_base.py
--rw-r--r--   0        0        0     9742 2023-06-23 13:38:56.179044 qdrant_client-1.3.0/qdrant_client/connection.py
--rw-r--r--   0        0        0        0 2023-06-23 13:38:56.179044 qdrant_client-1.3.0/qdrant_client/conversions/__init__.py
--rw-r--r--   0        0        0     3447 2023-06-23 13:38:56.179044 qdrant_client-1.3.0/qdrant_client/conversions/common_types.py
--rw-r--r--   0        0        0    72811 2023-06-23 13:38:56.179044 qdrant_client-1.3.0/qdrant_client/conversions/conversion.py
--rw-r--r--   0        0        0      252 2023-06-23 13:38:56.179044 qdrant_client-1.3.0/qdrant_client/grpc/__init__.py
--rw-r--r--   0        0        0    36463 2023-06-23 13:38:56.179044 qdrant_client-1.3.0/qdrant_client/grpc/collections_pb2.py
--rw-r--r--   0        0        0      159 2023-06-23 13:38:56.179044 qdrant_client-1.3.0/qdrant_client/grpc/collections_pb2_grpc.py
--rw-r--r--   0        0        0     2063 2023-06-23 13:38:56.179044 qdrant_client-1.3.0/qdrant_client/grpc/collections_service_pb2.py
--rw-r--r--   0        0        0    16916 2023-06-23 13:38:56.179044 qdrant_client-1.3.0/qdrant_client/grpc/collections_service_pb2_grpc.py
--rw-r--r--   0        0        0     3395 2023-06-23 13:38:56.179044 qdrant_client-1.3.0/qdrant_client/grpc/json_with_int_pb2.py
--rw-r--r--   0        0        0      159 2023-06-23 13:38:56.179044 qdrant_client-1.3.0/qdrant_client/grpc/json_with_int_pb2_grpc.py
--rw-r--r--   0        0        0    54119 2023-06-23 13:38:56.179044 qdrant_client-1.3.0/qdrant_client/grpc/points_pb2.py
--rw-r--r--   0        0        0      159 2023-06-23 13:38:56.179044 qdrant_client-1.3.0/qdrant_client/grpc/points_pb2_grpc.py
--rw-r--r--   0        0        0     2907 2023-06-23 13:38:56.179044 qdrant_client-1.3.0/qdrant_client/grpc/points_service_pb2.py
--rw-r--r--   0        0        0    30011 2023-06-23 13:38:56.179044 qdrant_client-1.3.0/qdrant_client/grpc/points_service_pb2_grpc.py
--rw-r--r--   0        0        0     2254 2023-06-23 13:38:56.179044 qdrant_client-1.3.0/qdrant_client/grpc/qdrant_pb2.py
--rw-r--r--   0        0        0     2411 2023-06-23 13:38:56.179044 qdrant_client-1.3.0/qdrant_client/grpc/qdrant_pb2_grpc.py
--rw-r--r--   0        0        0     7768 2023-06-23 13:38:56.179044 qdrant_client-1.3.0/qdrant_client/grpc/snapshots_service_pb2.py
--rw-r--r--   0        0        0    10406 2023-06-23 13:38:56.179044 qdrant_client-1.3.0/qdrant_client/grpc/snapshots_service_pb2_grpc.py
--rw-r--r--   0        0        0      505 2023-06-23 13:38:56.179044 qdrant_client-1.3.0/qdrant_client/http/__init__.py
--rw-r--r--   0        0        0        0 2023-06-23 13:38:56.179044 qdrant_client-1.3.0/qdrant_client/http/api/__init__.py
--rw-r--r--   0        0        0    10437 2023-06-23 13:38:56.179044 qdrant_client-1.3.0/qdrant_client/http/api/cluster_api.py
--rw-r--r--   0        0        0    30407 2023-06-23 13:38:56.179044 qdrant_client-1.3.0/qdrant_client/http/api/collections_api.py
--rw-r--r--   0        0        0    38894 2023-06-23 13:38:56.179044 qdrant_client-1.3.0/qdrant_client/http/api/points_api.py
--rw-r--r--   0        0        0     9499 2023-06-23 13:38:56.179044 qdrant_client-1.3.0/qdrant_client/http/api/service_api.py
--rw-r--r--   0        0        0    18850 2023-06-23 13:38:56.179044 qdrant_client-1.3.0/qdrant_client/http/api/snapshots_api.py
--rw-r--r--   0        0        0     7577 2023-06-23 13:38:56.179044 qdrant_client-1.3.0/qdrant_client/http/api_client.py
--rw-r--r--   0        0        0      233 2023-06-23 13:38:56.179044 qdrant_client-1.3.0/qdrant_client/http/configuration.py
--rw-r--r--   0        0        0     1616 2023-06-23 13:38:56.179044 qdrant_client-1.3.0/qdrant_client/http/exceptions.py
--rw-r--r--   0        0        0       22 2023-06-23 13:38:56.179044 qdrant_client-1.3.0/qdrant_client/http/models/__init__.py
--rw-r--r--   0        0        0    67870 2023-06-23 13:38:56.179044 qdrant_client-1.3.0/qdrant_client/http/models/models.py
--rw-r--r--   0        0        0        0 2023-06-23 13:38:56.179044 qdrant_client-1.3.0/qdrant_client/local/__init__.py
--rw-r--r--   0        0        0     2979 2023-06-23 13:38:56.179044 qdrant_client-1.3.0/qdrant_client/local/distances.py
--rw-r--r--   0        0        0     1446 2023-06-23 13:38:56.179044 qdrant_client-1.3.0/qdrant_client/local/geo.py
--rw-r--r--   0        0        0    29728 2023-06-23 13:38:56.179044 qdrant_client-1.3.0/qdrant_client/local/local_collection.py
--rw-r--r--   0        0        0     6371 2023-06-23 13:38:56.183044 qdrant_client-1.3.0/qdrant_client/local/payload_filters.py
--rw-r--r--   0        0        0     2922 2023-06-23 13:38:56.183044 qdrant_client-1.3.0/qdrant_client/local/payload_value_extractor.py
--rw-r--r--   0        0        0     4388 2023-06-23 13:38:56.183044 qdrant_client-1.3.0/qdrant_client/local/persistence.py
--rw-r--r--   0        0        0    23964 2023-06-23 13:38:56.183044 qdrant_client-1.3.0/qdrant_client/local/qdrant_local.py
--rw-r--r--   0        0        0        0 2023-06-23 13:38:56.183044 qdrant_client-1.3.0/qdrant_client/local/tests/__init__.py
--rw-r--r--   0        0        0     4210 2023-06-23 13:38:56.183044 qdrant_client-1.3.0/qdrant_client/local/tests/test_payload_filters.py
--rw-r--r--   0        0        0       40 2023-06-23 13:38:56.183044 qdrant_client-1.3.0/qdrant_client/models/__init__.py
--rw-r--r--   0        0        0     7034 2023-06-23 13:38:56.183044 qdrant_client-1.3.0/qdrant_client/parallel_processor.py
--rw-r--r--   0        0        0    13786 2023-06-23 13:38:56.183044 qdrant_client-1.3.0/qdrant_client/proto/collections.proto
--rw-r--r--   0        0        0     1496 2023-06-23 13:38:56.183044 qdrant_client-1.3.0/qdrant_client/proto/collections_service.proto
--rw-r--r--   0        0        0     1936 2023-06-23 13:38:56.183044 qdrant_client-1.3.0/qdrant_client/proto/json_with_int.proto
--rw-r--r--   0        0        0    19848 2023-06-23 13:38:56.183044 qdrant_client-1.3.0/qdrant_client/proto/points.proto
--rw-r--r--   0        0        0     2873 2023-06-23 13:38:56.183044 qdrant_client-1.3.0/qdrant_client/proto/points_service.proto
--rw-r--r--   0        0        0      331 2023-06-23 13:38:56.183044 qdrant_client-1.3.0/qdrant_client/proto/qdrant.proto
--rw-r--r--   0        0        0     1895 2023-06-23 13:38:56.183044 qdrant_client-1.3.0/qdrant_client/proto/snapshots_service.proto
--rw-r--r--   0        0        0        8 2023-06-23 13:38:56.183044 qdrant_client-1.3.0/qdrant_client/py.typed
--rw-r--r--   0        0        0    72285 2023-06-23 13:38:56.183044 qdrant_client-1.3.0/qdrant_client/qdrant_client.py
--rw-r--r--   0        0        0    81209 2023-06-23 13:38:56.183044 qdrant_client-1.3.0/qdrant_client/qdrant_remote.py
--rw-r--r--   0        0        0        0 2023-06-23 13:38:56.183044 qdrant_client-1.3.0/qdrant_client/uploader/__init__.py
--rw-r--r--   0        0        0     2758 2023-06-23 13:38:56.183044 qdrant_client-1.3.0/qdrant_client/uploader/grpc_uploader.py
--rw-r--r--   0        0        0     2160 2023-06-23 13:38:56.183044 qdrant_client-1.3.0/qdrant_client/uploader/rest_uploader.py
--rw-r--r--   0        0        0     3200 2023-06-23 13:38:56.183044 qdrant_client-1.3.0/qdrant_client/uploader/uploader.py
--rw-r--r--   0        0        0      267 2023-06-23 13:38:56.183044 qdrant_client-1.3.0/qdrant_openapi_client/__init__.py
--rw-r--r--   0        0        0       37 2023-06-23 13:38:56.183044 qdrant_client-1.3.0/qdrant_openapi_client/api/__init__.py
--rw-r--r--   0        0        0       53 2023-06-23 13:38:56.183044 qdrant_client-1.3.0/qdrant_openapi_client/api/collections_api.py
--rw-r--r--   0        0        0       48 2023-06-23 13:38:56.183044 qdrant_client-1.3.0/qdrant_openapi_client/api/points_api.py
--rw-r--r--   0        0        0       44 2023-06-23 13:38:56.183044 qdrant_client-1.3.0/qdrant_openapi_client/exceptions.py
--rw-r--r--   0        0        0       47 2023-06-23 13:38:56.183044 qdrant_client-1.3.0/qdrant_openapi_client/models/__init__.py
--rw-r--r--   0        0        0       47 2023-06-23 13:38:56.183044 qdrant_client-1.3.0/qdrant_openapi_client/models/models.py
--rw-r--r--   0        0        0     7353 1970-01-01 00:00:00.000000 qdrant_client-1.3.0/PKG-INFO
+-rw-r--r--   0        0        0    11357 2023-06-26 12:13:26.011897 qdrant_client-1.3.1/LICENSE
+-rw-r--r--   0        0        0     6250 2023-06-26 12:13:26.011897 qdrant_client-1.3.1/README.md
+-rw-r--r--   0        0        0     1440 2023-06-26 12:13:26.015897 qdrant_client-1.3.1/pyproject.toml
+-rw-r--r--   0        0        0       56 2023-06-26 12:13:26.015897 qdrant_client-1.3.1/qdrant_client/__init__.py
+-rw-r--r--   0        0        0    10034 2023-06-26 12:13:26.015897 qdrant_client-1.3.1/qdrant_client/client_base.py
+-rw-r--r--   0        0        0     9742 2023-06-26 12:13:26.015897 qdrant_client-1.3.1/qdrant_client/connection.py
+-rw-r--r--   0        0        0        0 2023-06-26 12:13:26.015897 qdrant_client-1.3.1/qdrant_client/conversions/__init__.py
+-rw-r--r--   0        0        0     3447 2023-06-26 12:13:26.015897 qdrant_client-1.3.1/qdrant_client/conversions/common_types.py
+-rw-r--r--   0        0        0    72811 2023-06-26 12:13:26.015897 qdrant_client-1.3.1/qdrant_client/conversions/conversion.py
+-rw-r--r--   0        0        0      252 2023-06-26 12:13:26.015897 qdrant_client-1.3.1/qdrant_client/grpc/__init__.py
+-rw-r--r--   0        0        0    36463 2023-06-26 12:13:26.015897 qdrant_client-1.3.1/qdrant_client/grpc/collections_pb2.py
+-rw-r--r--   0        0        0      159 2023-06-26 12:13:26.015897 qdrant_client-1.3.1/qdrant_client/grpc/collections_pb2_grpc.py
+-rw-r--r--   0        0        0     2063 2023-06-26 12:13:26.015897 qdrant_client-1.3.1/qdrant_client/grpc/collections_service_pb2.py
+-rw-r--r--   0        0        0    16916 2023-06-26 12:13:26.015897 qdrant_client-1.3.1/qdrant_client/grpc/collections_service_pb2_grpc.py
+-rw-r--r--   0        0        0     3395 2023-06-26 12:13:26.015897 qdrant_client-1.3.1/qdrant_client/grpc/json_with_int_pb2.py
+-rw-r--r--   0        0        0      159 2023-06-26 12:13:26.015897 qdrant_client-1.3.1/qdrant_client/grpc/json_with_int_pb2_grpc.py
+-rw-r--r--   0        0        0    54119 2023-06-26 12:13:26.015897 qdrant_client-1.3.1/qdrant_client/grpc/points_pb2.py
+-rw-r--r--   0        0        0      159 2023-06-26 12:13:26.015897 qdrant_client-1.3.1/qdrant_client/grpc/points_pb2_grpc.py
+-rw-r--r--   0        0        0     2907 2023-06-26 12:13:26.015897 qdrant_client-1.3.1/qdrant_client/grpc/points_service_pb2.py
+-rw-r--r--   0        0        0    30011 2023-06-26 12:13:26.015897 qdrant_client-1.3.1/qdrant_client/grpc/points_service_pb2_grpc.py
+-rw-r--r--   0        0        0     2254 2023-06-26 12:13:26.015897 qdrant_client-1.3.1/qdrant_client/grpc/qdrant_pb2.py
+-rw-r--r--   0        0        0     2411 2023-06-26 12:13:26.015897 qdrant_client-1.3.1/qdrant_client/grpc/qdrant_pb2_grpc.py
+-rw-r--r--   0        0        0     7768 2023-06-26 12:13:26.015897 qdrant_client-1.3.1/qdrant_client/grpc/snapshots_service_pb2.py
+-rw-r--r--   0        0        0    10406 2023-06-26 12:13:26.015897 qdrant_client-1.3.1/qdrant_client/grpc/snapshots_service_pb2_grpc.py
+-rw-r--r--   0        0        0      505 2023-06-26 12:13:26.015897 qdrant_client-1.3.1/qdrant_client/http/__init__.py
+-rw-r--r--   0        0        0        0 2023-06-26 12:13:26.015897 qdrant_client-1.3.1/qdrant_client/http/api/__init__.py
+-rw-r--r--   0        0        0    10437 2023-06-26 12:13:26.015897 qdrant_client-1.3.1/qdrant_client/http/api/cluster_api.py
+-rw-r--r--   0        0        0    30407 2023-06-26 12:13:26.019898 qdrant_client-1.3.1/qdrant_client/http/api/collections_api.py
+-rw-r--r--   0        0        0    38894 2023-06-26 12:13:26.019898 qdrant_client-1.3.1/qdrant_client/http/api/points_api.py
+-rw-r--r--   0        0        0     9499 2023-06-26 12:13:26.019898 qdrant_client-1.3.1/qdrant_client/http/api/service_api.py
+-rw-r--r--   0        0        0    18850 2023-06-26 12:13:26.019898 qdrant_client-1.3.1/qdrant_client/http/api/snapshots_api.py
+-rw-r--r--   0        0        0     7577 2023-06-26 12:13:26.019898 qdrant_client-1.3.1/qdrant_client/http/api_client.py
+-rw-r--r--   0        0        0      233 2023-06-26 12:13:26.019898 qdrant_client-1.3.1/qdrant_client/http/configuration.py
+-rw-r--r--   0        0        0     1616 2023-06-26 12:13:26.019898 qdrant_client-1.3.1/qdrant_client/http/exceptions.py
+-rw-r--r--   0        0        0       22 2023-06-26 12:13:26.019898 qdrant_client-1.3.1/qdrant_client/http/models/__init__.py
+-rw-r--r--   0        0        0    67870 2023-06-26 12:13:26.019898 qdrant_client-1.3.1/qdrant_client/http/models/models.py
+-rw-r--r--   0        0        0        0 2023-06-26 12:13:26.019898 qdrant_client-1.3.1/qdrant_client/local/__init__.py
+-rw-r--r--   0        0        0     2979 2023-06-26 12:13:26.019898 qdrant_client-1.3.1/qdrant_client/local/distances.py
+-rw-r--r--   0        0        0     1446 2023-06-26 12:13:26.019898 qdrant_client-1.3.1/qdrant_client/local/geo.py
+-rw-r--r--   0        0        0    29728 2023-06-26 12:13:26.019898 qdrant_client-1.3.1/qdrant_client/local/local_collection.py
+-rw-r--r--   0        0        0     6371 2023-06-26 12:13:26.019898 qdrant_client-1.3.1/qdrant_client/local/payload_filters.py
+-rw-r--r--   0        0        0     2922 2023-06-26 12:13:26.019898 qdrant_client-1.3.1/qdrant_client/local/payload_value_extractor.py
+-rw-r--r--   0        0        0     4388 2023-06-26 12:13:26.019898 qdrant_client-1.3.1/qdrant_client/local/persistence.py
+-rw-r--r--   0        0        0    23964 2023-06-26 12:13:26.019898 qdrant_client-1.3.1/qdrant_client/local/qdrant_local.py
+-rw-r--r--   0        0        0        0 2023-06-26 12:13:26.019898 qdrant_client-1.3.1/qdrant_client/local/tests/__init__.py
+-rw-r--r--   0        0        0     4210 2023-06-26 12:13:26.019898 qdrant_client-1.3.1/qdrant_client/local/tests/test_payload_filters.py
+-rw-r--r--   0        0        0       40 2023-06-26 12:13:26.019898 qdrant_client-1.3.1/qdrant_client/models/__init__.py
+-rw-r--r--   0        0        0     7034 2023-06-26 12:13:26.019898 qdrant_client-1.3.1/qdrant_client/parallel_processor.py
+-rw-r--r--   0        0        0    13786 2023-06-26 12:13:26.019898 qdrant_client-1.3.1/qdrant_client/proto/collections.proto
+-rw-r--r--   0        0        0     1496 2023-06-26 12:13:26.019898 qdrant_client-1.3.1/qdrant_client/proto/collections_service.proto
+-rw-r--r--   0        0        0     1936 2023-06-26 12:13:26.019898 qdrant_client-1.3.1/qdrant_client/proto/json_with_int.proto
+-rw-r--r--   0        0        0    19848 2023-06-26 12:13:26.019898 qdrant_client-1.3.1/qdrant_client/proto/points.proto
+-rw-r--r--   0        0        0     2873 2023-06-26 12:13:26.019898 qdrant_client-1.3.1/qdrant_client/proto/points_service.proto
+-rw-r--r--   0        0        0      331 2023-06-26 12:13:26.019898 qdrant_client-1.3.1/qdrant_client/proto/qdrant.proto
+-rw-r--r--   0        0        0     1895 2023-06-26 12:13:26.019898 qdrant_client-1.3.1/qdrant_client/proto/snapshots_service.proto
+-rw-r--r--   0        0        0        8 2023-06-26 12:13:26.019898 qdrant_client-1.3.1/qdrant_client/py.typed
+-rw-r--r--   0        0        0    72285 2023-06-26 12:13:26.019898 qdrant_client-1.3.1/qdrant_client/qdrant_client.py
+-rw-r--r--   0        0        0    81209 2023-06-26 12:13:26.019898 qdrant_client-1.3.1/qdrant_client/qdrant_remote.py
+-rw-r--r--   0        0        0        0 2023-06-26 12:13:26.019898 qdrant_client-1.3.1/qdrant_client/uploader/__init__.py
+-rw-r--r--   0        0        0     2758 2023-06-26 12:13:26.019898 qdrant_client-1.3.1/qdrant_client/uploader/grpc_uploader.py
+-rw-r--r--   0        0        0     2160 2023-06-26 12:13:26.019898 qdrant_client-1.3.1/qdrant_client/uploader/rest_uploader.py
+-rw-r--r--   0        0        0     3200 2023-06-26 12:13:26.019898 qdrant_client-1.3.1/qdrant_client/uploader/uploader.py
+-rw-r--r--   0        0        0      267 2023-06-26 12:13:26.019898 qdrant_client-1.3.1/qdrant_openapi_client/__init__.py
+-rw-r--r--   0        0        0       37 2023-06-26 12:13:26.019898 qdrant_client-1.3.1/qdrant_openapi_client/api/__init__.py
+-rw-r--r--   0        0        0       53 2023-06-26 12:13:26.019898 qdrant_client-1.3.1/qdrant_openapi_client/api/collections_api.py
+-rw-r--r--   0        0        0       48 2023-06-26 12:13:26.019898 qdrant_client-1.3.1/qdrant_openapi_client/api/points_api.py
+-rw-r--r--   0        0        0       44 2023-06-26 12:13:26.019898 qdrant_client-1.3.1/qdrant_openapi_client/exceptions.py
+-rw-r--r--   0        0        0       47 2023-06-26 12:13:26.019898 qdrant_client-1.3.1/qdrant_openapi_client/models/__init__.py
+-rw-r--r--   0        0        0       47 2023-06-26 12:13:26.019898 qdrant_client-1.3.1/qdrant_openapi_client/models/models.py
+-rw-r--r--   0        0        0     7436 1970-01-01 00:00:00.000000 qdrant_client-1.3.1/PKG-INFO
```

### Comparing `qdrant_client-1.3.0/LICENSE` & `qdrant_client-1.3.1/LICENSE`

 * *Files identical despite different names*

### Comparing `qdrant_client-1.3.0/README.md` & `qdrant_client-1.3.1/README.md`

 * *Files identical despite different names*

### Comparing `qdrant_client-1.3.0/pyproject.toml` & `qdrant_client-1.3.1/pyproject.toml`

 * *Files 8% similar despite different names*

```diff
@@ -1,16 +1,17 @@
 [tool.poetry]
 name = "qdrant-client"
-version = "1.3.0"
+version = "1.3.1"
 description = "Client library for the Qdrant vector search engine"
 authors = ["Andrey Vasnetsov <andrey@qdrant.tech>"]
 packages = [
     {include = "qdrant_client"},
     {include = "qdrant_openapi_client"}
 ]
+license = "Apache-2.0"
 readme = "README.md"
 homepage = "https://github.com/qdrant/qdrant-client"
 repository = "https://github.com/qdrant/qdrant-client"
 keywords = ["vector", "search", "neural", "matching", "client"]
 
 [tool.poetry.dependencies]
 python = ">=3.7,<3.12"
```

### Comparing `qdrant_client-1.3.0/qdrant_client/client_base.py` & `qdrant_client-1.3.1/qdrant_client/client_base.py`

 * *Files identical despite different names*

### Comparing `qdrant_client-1.3.0/qdrant_client/connection.py` & `qdrant_client-1.3.1/qdrant_client/connection.py`

 * *Files identical despite different names*

### Comparing `qdrant_client-1.3.0/qdrant_client/conversions/common_types.py` & `qdrant_client-1.3.1/qdrant_client/conversions/common_types.py`

 * *Files identical despite different names*

### Comparing `qdrant_client-1.3.0/qdrant_client/conversions/conversion.py` & `qdrant_client-1.3.1/qdrant_client/conversions/conversion.py`

 * *Files identical despite different names*

### Comparing `qdrant_client-1.3.0/qdrant_client/grpc/collections_pb2.py` & `qdrant_client-1.3.1/qdrant_client/grpc/collections_pb2.py`

 * *Files identical despite different names*

### Comparing `qdrant_client-1.3.0/qdrant_client/grpc/collections_service_pb2.py` & `qdrant_client-1.3.1/qdrant_client/grpc/collections_service_pb2.py`

 * *Files identical despite different names*

### Comparing `qdrant_client-1.3.0/qdrant_client/grpc/collections_service_pb2_grpc.py` & `qdrant_client-1.3.1/qdrant_client/grpc/collections_service_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `qdrant_client-1.3.0/qdrant_client/grpc/json_with_int_pb2.py` & `qdrant_client-1.3.1/qdrant_client/grpc/json_with_int_pb2.py`

 * *Files identical despite different names*

### Comparing `qdrant_client-1.3.0/qdrant_client/grpc/points_pb2.py` & `qdrant_client-1.3.1/qdrant_client/grpc/points_pb2.py`

 * *Files identical despite different names*

### Comparing `qdrant_client-1.3.0/qdrant_client/grpc/points_service_pb2.py` & `qdrant_client-1.3.1/qdrant_client/grpc/points_service_pb2.py`

 * *Files identical despite different names*

### Comparing `qdrant_client-1.3.0/qdrant_client/grpc/points_service_pb2_grpc.py` & `qdrant_client-1.3.1/qdrant_client/grpc/points_service_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `qdrant_client-1.3.0/qdrant_client/grpc/qdrant_pb2.py` & `qdrant_client-1.3.1/qdrant_client/grpc/qdrant_pb2.py`

 * *Files identical despite different names*

### Comparing `qdrant_client-1.3.0/qdrant_client/grpc/qdrant_pb2_grpc.py` & `qdrant_client-1.3.1/qdrant_client/grpc/qdrant_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `qdrant_client-1.3.0/qdrant_client/grpc/snapshots_service_pb2.py` & `qdrant_client-1.3.1/qdrant_client/grpc/snapshots_service_pb2.py`

 * *Files identical despite different names*

### Comparing `qdrant_client-1.3.0/qdrant_client/grpc/snapshots_service_pb2_grpc.py` & `qdrant_client-1.3.1/qdrant_client/grpc/snapshots_service_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `qdrant_client-1.3.0/qdrant_client/http/api/cluster_api.py` & `qdrant_client-1.3.1/qdrant_client/http/api/cluster_api.py`

 * *Files identical despite different names*

### Comparing `qdrant_client-1.3.0/qdrant_client/http/api/collections_api.py` & `qdrant_client-1.3.1/qdrant_client/http/api/collections_api.py`

 * *Files identical despite different names*

### Comparing `qdrant_client-1.3.0/qdrant_client/http/api/points_api.py` & `qdrant_client-1.3.1/qdrant_client/http/api/points_api.py`

 * *Files identical despite different names*

### Comparing `qdrant_client-1.3.0/qdrant_client/http/api/service_api.py` & `qdrant_client-1.3.1/qdrant_client/http/api/service_api.py`

 * *Files identical despite different names*

### Comparing `qdrant_client-1.3.0/qdrant_client/http/api/snapshots_api.py` & `qdrant_client-1.3.1/qdrant_client/http/api/snapshots_api.py`

 * *Files identical despite different names*

### Comparing `qdrant_client-1.3.0/qdrant_client/http/api_client.py` & `qdrant_client-1.3.1/qdrant_client/http/api_client.py`

 * *Files identical despite different names*

### Comparing `qdrant_client-1.3.0/qdrant_client/http/exceptions.py` & `qdrant_client-1.3.1/qdrant_client/http/exceptions.py`

 * *Files identical despite different names*

### Comparing `qdrant_client-1.3.0/qdrant_client/http/models/models.py` & `qdrant_client-1.3.1/qdrant_client/http/models/models.py`

 * *Files identical despite different names*

### Comparing `qdrant_client-1.3.0/qdrant_client/local/distances.py` & `qdrant_client-1.3.1/qdrant_client/local/distances.py`

 * *Files identical despite different names*

### Comparing `qdrant_client-1.3.0/qdrant_client/local/geo.py` & `qdrant_client-1.3.1/qdrant_client/local/geo.py`

 * *Files identical despite different names*

### Comparing `qdrant_client-1.3.0/qdrant_client/local/local_collection.py` & `qdrant_client-1.3.1/qdrant_client/local/local_collection.py`

 * *Files identical despite different names*

### Comparing `qdrant_client-1.3.0/qdrant_client/local/payload_filters.py` & `qdrant_client-1.3.1/qdrant_client/local/payload_filters.py`

 * *Files identical despite different names*

### Comparing `qdrant_client-1.3.0/qdrant_client/local/payload_value_extractor.py` & `qdrant_client-1.3.1/qdrant_client/local/payload_value_extractor.py`

 * *Files identical despite different names*

### Comparing `qdrant_client-1.3.0/qdrant_client/local/persistence.py` & `qdrant_client-1.3.1/qdrant_client/local/persistence.py`

 * *Files identical despite different names*

### Comparing `qdrant_client-1.3.0/qdrant_client/local/qdrant_local.py` & `qdrant_client-1.3.1/qdrant_client/local/qdrant_local.py`

 * *Files identical despite different names*

### Comparing `qdrant_client-1.3.0/qdrant_client/local/tests/test_payload_filters.py` & `qdrant_client-1.3.1/qdrant_client/local/tests/test_payload_filters.py`

 * *Files identical despite different names*

### Comparing `qdrant_client-1.3.0/qdrant_client/parallel_processor.py` & `qdrant_client-1.3.1/qdrant_client/parallel_processor.py`

 * *Files identical despite different names*

### Comparing `qdrant_client-1.3.0/qdrant_client/proto/collections.proto` & `qdrant_client-1.3.1/qdrant_client/proto/collections.proto`

 * *Files identical despite different names*

### Comparing `qdrant_client-1.3.0/qdrant_client/proto/collections_service.proto` & `qdrant_client-1.3.1/qdrant_client/proto/collections_service.proto`

 * *Files identical despite different names*

### Comparing `qdrant_client-1.3.0/qdrant_client/proto/json_with_int.proto` & `qdrant_client-1.3.1/qdrant_client/proto/json_with_int.proto`

 * *Files identical despite different names*

### Comparing `qdrant_client-1.3.0/qdrant_client/proto/points.proto` & `qdrant_client-1.3.1/qdrant_client/proto/points.proto`

 * *Files identical despite different names*

### Comparing `qdrant_client-1.3.0/qdrant_client/proto/points_service.proto` & `qdrant_client-1.3.1/qdrant_client/proto/points_service.proto`

 * *Files identical despite different names*

### Comparing `qdrant_client-1.3.0/qdrant_client/proto/snapshots_service.proto` & `qdrant_client-1.3.1/qdrant_client/proto/snapshots_service.proto`

 * *Files identical despite different names*

### Comparing `qdrant_client-1.3.0/qdrant_client/qdrant_client.py` & `qdrant_client-1.3.1/qdrant_client/qdrant_client.py`

 * *Files identical despite different names*

### Comparing `qdrant_client-1.3.0/qdrant_client/qdrant_remote.py` & `qdrant_client-1.3.1/qdrant_client/qdrant_remote.py`

 * *Files identical despite different names*

### Comparing `qdrant_client-1.3.0/qdrant_client/uploader/grpc_uploader.py` & `qdrant_client-1.3.1/qdrant_client/uploader/grpc_uploader.py`

 * *Files identical despite different names*

### Comparing `qdrant_client-1.3.0/qdrant_client/uploader/rest_uploader.py` & `qdrant_client-1.3.1/qdrant_client/uploader/rest_uploader.py`

 * *Files identical despite different names*

### Comparing `qdrant_client-1.3.0/qdrant_client/uploader/uploader.py` & `qdrant_client-1.3.1/qdrant_client/uploader/uploader.py`

 * *Files identical despite different names*

### Comparing `qdrant_client-1.3.0/PKG-INFO` & `qdrant_client-1.3.1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,16 +1,18 @@
 Metadata-Version: 2.1
 Name: qdrant-client
-Version: 1.3.0
+Version: 1.3.1
 Summary: Client library for the Qdrant vector search engine
 Home-page: https://github.com/qdrant/qdrant-client
+License: Apache-2.0
 Keywords: vector,search,neural,matching,client
 Author: Andrey Vasnetsov
 Author-email: andrey@qdrant.tech
 Requires-Python: >=3.7,<3.12
+Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Requires-Dist: grpcio (>=1.41.0)
```

#### html2text {}

```diff
@@ -1,22 +1,23 @@
-Metadata-Version: 2.1 Name: qdrant-client Version: 1.3.0 Summary: Client
+Metadata-Version: 2.1 Name: qdrant-client Version: 1.3.1 Summary: Client
 library for the Qdrant vector search engine Home-page: https://github.com/
-qdrant/qdrant-client Keywords: vector,search,neural,matching,client Author:
-Andrey Vasnetsov Author-email: andrey@qdrant.tech Requires-Python: >=3.7,<3.12
-Classifier: Programming Language :: Python :: 3 Classifier: Programming
-Language :: Python :: 3.7 Classifier: Programming Language :: Python :: 3.8
-Classifier: Programming Language :: Python :: 3.9 Classifier: Programming
-Language :: Python :: 3.10 Classifier: Programming Language :: Python :: 3.11
-Requires-Dist: grpcio (>=1.41.0) Requires-Dist: grpcio-tools (>=1.41.0)
-Requires-Dist: httpx[http2] (>=0.14.0) Requires-Dist: numpy (<1.21) ;
-python_version < "3.8" Requires-Dist: numpy (>=1.21) ; python_version >= "3.8"
-Requires-Dist: portalocker (>=2.7.0,<3.0.0) Requires-Dist: pydantic
-(>=1.8,<2.0) Requires-Dist: typing-extensions (>=4.0.0,<4.6.0) Requires-Dist:
-urllib3 (>=1.26.14,<2.0.0) Project-URL: Repository, https://github.com/qdrant/
-qdrant-client Description-Content-Type: text/markdown
+qdrant/qdrant-client License: Apache-2.0 Keywords:
+vector,search,neural,matching,client Author: Andrey Vasnetsov Author-email:
+andrey@qdrant.tech Requires-Python: >=3.7,<3.12 Classifier: License :: OSI
+Approved :: Apache Software License Classifier: Programming Language :: Python
+:: 3 Classifier: Programming Language :: Python :: 3.7 Classifier: Programming
+Language :: Python :: 3.8 Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10 Classifier: Programming
+Language :: Python :: 3.11 Requires-Dist: grpcio (>=1.41.0) Requires-Dist:
+grpcio-tools (>=1.41.0) Requires-Dist: httpx[http2] (>=0.14.0) Requires-Dist:
+numpy (<1.21) ; python_version < "3.8" Requires-Dist: numpy (>=1.21) ;
+python_version >= "3.8" Requires-Dist: portalocker (>=2.7.0,<3.0.0) Requires-
+Dist: pydantic (>=1.8,<2.0) Requires-Dist: typing-extensions (>=4.0.0,<4.6.0)
+Requires-Dist: urllib3 (>=1.26.14,<2.0.0) Project-URL: Repository, https://
+github.com/qdrant/qdrant-client Description-Content-Type: text/markdown
                                    [Qdrant]
           Python Client library for the Qdrant vector search engine.
   [PyPI_version] [OpenAPI_Docs] [Apache_2.0_License] [Discord] [Roadmap_2023]
 # Python Qdrant Client Client library and SDK for the [Qdrant](https://
 github.com/qdrant/qdrant) vector search engine. Library contains type
 definitions for all Qdrant API and allows to make both Sync and Async requests.
 Client allows calls for all [Qdrant API methods](https://qdrant.github.io/
```

