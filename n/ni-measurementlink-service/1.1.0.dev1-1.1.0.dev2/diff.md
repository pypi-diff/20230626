# Comparing `tmp/ni_measurementlink_service-1.1.0.dev1.tar.gz` & `tmp/ni_measurementlink_service-1.1.0.dev2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ni_measurementlink_service-1.1.0.dev1.tar", max compression
+gzip compressed data, was "ni_measurementlink_service-1.1.0.dev2.tar", max compression
```

## Comparing `ni_measurementlink_service-1.1.0.dev1.tar` & `ni_measurementlink_service-1.1.0.dev2.tar`

### file list

```diff
@@ -1,61 +1,68 @@
--rw-r--r--   0        0        0     1071 2023-05-18 21:55:42.165839 ni_measurementlink_service-1.1.0.dev1/LICENSE
--rw-r--r--   0        0        0    16415 2023-05-18 21:55:42.165839 ni_measurementlink_service-1.1.0.dev1/README.md
--rw-r--r--   0        0        0      513 2023-05-18 21:55:42.209840 ni_measurementlink_service-1.1.0.dev1/ni_measurementlink_service/__init__.py
--rw-r--r--   0        0        0       62 2023-05-18 21:55:42.209840 ni_measurementlink_service-1.1.0.dev1/ni_measurementlink_service/_internal/__init__.py
--rw-r--r--   0        0        0    10404 2023-05-18 21:55:42.209840 ni_measurementlink_service-1.1.0.dev1/ni_measurementlink_service/_internal/discovery_client.py
--rw-r--r--   0        0        0    16735 2023-05-18 21:55:42.209840 ni_measurementlink_service-1.1.0.dev1/ni_measurementlink_service/_internal/grpc_servicer.py
--rw-r--r--   0        0        0       58 2023-05-18 21:55:42.209840 ni_measurementlink_service-1.1.0.dev1/ni_measurementlink_service/_internal/parameter/__init__.py
--rw-r--r--   0        0        0     2236 2023-05-18 21:55:42.209840 ni_measurementlink_service-1.1.0.dev1/ni_measurementlink_service/_internal/parameter/metadata.py
--rw-r--r--   0        0        0     9062 2023-05-18 21:55:42.209840 ni_measurementlink_service-1.1.0.dev1/ni_measurementlink_service/_internal/parameter/serialization_strategy.py
--rw-r--r--   0        0        0     6182 2023-05-18 21:55:42.209840 ni_measurementlink_service-1.1.0.dev1/ni_measurementlink_service/_internal/parameter/serializer.py
--rw-r--r--   0        0        0     3933 2023-05-18 21:55:42.209840 ni_measurementlink_service-1.1.0.dev1/ni_measurementlink_service/_internal/service_manager.py
--rw-r--r--   0        0        0       33 2023-05-18 21:55:42.209840 ni_measurementlink_service-1.1.0.dev1/ni_measurementlink_service/_internal/stubs/__init__.py
--rw-r--r--   0        0        0       33 2023-05-18 21:55:42.209840 ni_measurementlink_service-1.1.0.dev1/ni_measurementlink_service/_internal/stubs/ni/__init__.py
--rw-r--r--   0        0        0       33 2023-05-18 21:55:42.209840 ni_measurementlink_service-1.1.0.dev1/ni_measurementlink_service/_internal/stubs/ni/measurementlink/__init__.py
--rw-r--r--   0        0        0       33 2023-05-18 21:55:42.209840 ni_measurementlink_service-1.1.0.dev1/ni_measurementlink_service/_internal/stubs/ni/measurementlink/discovery/__init__.py
--rw-r--r--   0        0        0       33 2023-05-18 21:55:42.213840 ni_measurementlink_service-1.1.0.dev1/ni_measurementlink_service/_internal/stubs/ni/measurementlink/discovery/v1/__init__.py
--rw-r--r--   0        0        0     4264 2023-05-18 21:55:42.213840 ni_measurementlink_service-1.1.0.dev1/ni_measurementlink_service/_internal/stubs/ni/measurementlink/discovery/v1/discovery_service_pb2.py
--rw-r--r--   0        0        0     8921 2023-05-18 21:55:42.213840 ni_measurementlink_service-1.1.0.dev1/ni_measurementlink_service/_internal/stubs/ni/measurementlink/discovery/v1/discovery_service_pb2.pyi
--rw-r--r--   0        0        0    10817 2023-05-18 21:55:42.213840 ni_measurementlink_service-1.1.0.dev1/ni_measurementlink_service/_internal/stubs/ni/measurementlink/discovery/v1/discovery_service_pb2_grpc.py
--rw-r--r--   0        0        0       33 2023-05-18 21:55:42.213840 ni_measurementlink_service-1.1.0.dev1/ni_measurementlink_service/_internal/stubs/ni/measurementlink/measurement/__init__.py
--rw-r--r--   0        0        0       33 2023-05-18 21:55:42.213840 ni_measurementlink_service-1.1.0.dev1/ni_measurementlink_service/_internal/stubs/ni/measurementlink/measurement/v1/__init__.py
--rw-r--r--   0        0        0     5345 2023-05-18 21:55:42.213840 ni_measurementlink_service-1.1.0.dev1/ni_measurementlink_service/_internal/stubs/ni/measurementlink/measurement/v1/measurement_service_pb2.py
--rw-r--r--   0        0        0    13593 2023-05-18 21:55:42.213840 ni_measurementlink_service-1.1.0.dev1/ni_measurementlink_service/_internal/stubs/ni/measurementlink/measurement/v1/measurement_service_pb2.pyi
--rw-r--r--   0        0        0     5546 2023-05-18 21:55:42.213840 ni_measurementlink_service-1.1.0.dev1/ni_measurementlink_service/_internal/stubs/ni/measurementlink/measurement/v1/measurement_service_pb2_grpc.py
--rw-r--r--   0        0        0       33 2023-05-18 21:55:42.213840 ni_measurementlink_service-1.1.0.dev1/ni_measurementlink_service/_internal/stubs/ni/measurementlink/measurement/v2/__init__.py
--rw-r--r--   0        0        0     5777 2023-05-18 21:55:42.213840 ni_measurementlink_service-1.1.0.dev1/ni_measurementlink_service/_internal/stubs/ni/measurementlink/measurement/v2/measurement_service_pb2.py
--rw-r--r--   0        0        0    15001 2023-05-18 21:55:42.213840 ni_measurementlink_service-1.1.0.dev1/ni_measurementlink_service/_internal/stubs/ni/measurementlink/measurement/v2/measurement_service_pb2.pyi
--rw-r--r--   0        0        0     5549 2023-05-18 21:55:42.213840 ni_measurementlink_service-1.1.0.dev1/ni_measurementlink_service/_internal/stubs/ni/measurementlink/measurement/v2/measurement_service_pb2_grpc.py
--rw-r--r--   0        0        0     1532 2023-05-18 21:55:42.213840 ni_measurementlink_service-1.1.0.dev1/ni_measurementlink_service/_internal/stubs/ni/measurementlink/pin_map_context_pb2.py
--rw-r--r--   0        0        0     1314 2023-05-18 21:55:42.213840 ni_measurementlink_service-1.1.0.dev1/ni_measurementlink_service/_internal/stubs/ni/measurementlink/pin_map_context_pb2.pyi
--rw-r--r--   0        0        0      159 2023-05-18 21:55:42.213840 ni_measurementlink_service-1.1.0.dev1/ni_measurementlink_service/_internal/stubs/ni/measurementlink/pin_map_context_pb2_grpc.py
--rw-r--r--   0        0        0       33 2023-05-18 21:55:42.213840 ni_measurementlink_service-1.1.0.dev1/ni_measurementlink_service/_internal/stubs/ni/measurementlink/pinmap/__init__.py
--rw-r--r--   0        0        0       33 2023-05-18 21:55:42.213840 ni_measurementlink_service-1.1.0.dev1/ni_measurementlink_service/_internal/stubs/ni/measurementlink/pinmap/v1/__init__.py
--rw-r--r--   0        0        0     6202 2023-05-18 21:55:42.213840 ni_measurementlink_service-1.1.0.dev1/ni_measurementlink_service/_internal/stubs/ni/measurementlink/pinmap/v1/pin_map_service_pb2.py
--rw-r--r--   0        0        0    18188 2023-05-18 21:55:42.213840 ni_measurementlink_service-1.1.0.dev1/ni_measurementlink_service/_internal/stubs/ni/measurementlink/pinmap/v1/pin_map_service_pb2.pyi
--rw-r--r--   0        0        0    14078 2023-05-18 21:55:42.213840 ni_measurementlink_service-1.1.0.dev1/ni_measurementlink_service/_internal/stubs/ni/measurementlink/pinmap/v1/pin_map_service_pb2_grpc.py
--rw-r--r--   0        0        0       33 2023-05-18 21:55:42.213840 ni_measurementlink_service-1.1.0.dev1/ni_measurementlink_service/_internal/stubs/ni/measurementlink/sessionmanagement/__init__.py
--rw-r--r--   0        0        0       33 2023-05-18 21:55:42.213840 ni_measurementlink_service-1.1.0.dev1/ni_measurementlink_service/_internal/stubs/ni/measurementlink/sessionmanagement/v1/__init__.py
--rw-r--r--   0        0        0     5955 2023-05-18 21:55:42.213840 ni_measurementlink_service-1.1.0.dev1/ni_measurementlink_service/_internal/stubs/ni/measurementlink/sessionmanagement/v1/session_management_service_pb2.py
--rw-r--r--   0        0        0    13237 2023-05-18 21:55:42.213840 ni_measurementlink_service-1.1.0.dev1/ni_measurementlink_service/_internal/stubs/ni/measurementlink/sessionmanagement/v1/session_management_service_pb2.pyi
--rw-r--r--   0        0        0    13882 2023-05-18 21:55:42.213840 ni_measurementlink_service-1.1.0.dev1/ni_measurementlink_service/_internal/stubs/ni/measurementlink/sessionmanagement/v1/session_management_service_pb2_grpc.py
--rw-r--r--   0        0        0      709 2023-05-18 21:55:42.213840 ni_measurementlink_service-1.1.0.dev1/ni_measurementlink_service/_internal/stubs/proto/README.md
--rw-r--r--   0        0        0     6052 2023-05-18 21:55:42.213840 ni_measurementlink_service-1.1.0.dev1/ni_measurementlink_service/_internal/stubs/proto/ni/measurementlink/discovery/v1/discovery_service.proto
--rw-r--r--   0        0        0     6650 2023-05-18 21:55:42.213840 ni_measurementlink_service-1.1.0.dev1/ni_measurementlink_service/_internal/stubs/proto/ni/measurementlink/measurement/v1/measurement_service.proto
--rw-r--r--   0        0        0     7228 2023-05-18 21:55:42.213840 ni_measurementlink_service-1.1.0.dev1/ni_measurementlink_service/_internal/stubs/proto/ni/measurementlink/measurement/v2/measurement_service.proto
--rw-r--r--   0        0        0      712 2023-05-18 21:55:42.213840 ni_measurementlink_service-1.1.0.dev1/ni_measurementlink_service/_internal/stubs/proto/ni/measurementlink/pin_map_context.proto
--rw-r--r--   0        0        0     9622 2023-05-18 21:55:42.213840 ni_measurementlink_service-1.1.0.dev1/ni_measurementlink_service/_internal/stubs/proto/ni/measurementlink/pinmap/v1/pin_map_service.proto
--rw-r--r--   0        0        0     8468 2023-05-18 21:55:42.213840 ni_measurementlink_service-1.1.0.dev1/ni_measurementlink_service/_internal/stubs/proto/ni/measurementlink/sessionmanagement/v1/session_management_service.proto
--rw-r--r--   0        0        0     2426 2023-05-18 21:55:42.213840 ni_measurementlink_service-1.1.0.dev1/ni_measurementlink_service/_internal/stubs/proto/session.proto
--rw-r--r--   0        0        0     4196 2023-05-18 21:55:42.213840 ni_measurementlink_service-1.1.0.dev1/ni_measurementlink_service/_internal/stubs/session_pb2.py
--rw-r--r--   0        0        0     8735 2023-05-18 21:55:42.213840 ni_measurementlink_service-1.1.0.dev1/ni_measurementlink_service/_internal/stubs/session_pb2.pyi
--rw-r--r--   0        0        0     8948 2023-05-18 21:55:42.213840 ni_measurementlink_service-1.1.0.dev1/ni_measurementlink_service/_internal/stubs/session_pb2_grpc.py
--rw-r--r--   0        0        0       35 2023-05-18 21:55:42.213840 ni_measurementlink_service-1.1.0.dev1/ni_measurementlink_service/_internal/utilities/__init__.py
--rw-r--r--   0        0        0       37 2023-05-18 21:55:42.213840 ni_measurementlink_service-1.1.0.dev1/ni_measurementlink_service/measurement/__init__.py
--rw-r--r--   0        0        0     3021 2023-05-18 21:55:42.213840 ni_measurementlink_service-1.1.0.dev1/ni_measurementlink_service/measurement/info.py
--rw-r--r--   0        0        0    13261 2023-05-18 21:55:42.213840 ni_measurementlink_service-1.1.0.dev1/ni_measurementlink_service/measurement/service.py
--rw-r--r--   0        0        0        0 2023-05-18 21:55:42.213840 ni_measurementlink_service-1.1.0.dev1/ni_measurementlink_service/py.typed
--rw-r--r--   0        0        0    14466 2023-05-18 21:55:42.213840 ni_measurementlink_service-1.1.0.dev1/ni_measurementlink_service/session_management.py
--rw-r--r--   0        0        0     2650 2023-05-18 21:57:24.107064 ni_measurementlink_service-1.1.0.dev1/pyproject.toml
--rw-r--r--   0        0        0    19283 1970-01-01 00:00:00.000000 ni_measurementlink_service-1.1.0.dev1/setup.py
--rw-r--r--   0        0        0    17629 1970-01-01 00:00:00.000000 ni_measurementlink_service-1.1.0.dev1/PKG-INFO
+-rw-r--r--   0        0        0     1071 2023-06-26 21:34:54.060588 ni_measurementlink_service-1.1.0.dev2/LICENSE
+-rw-r--r--   0        0        0    16723 2023-06-26 21:34:54.060588 ni_measurementlink_service-1.1.0.dev2/README.md
+-rw-r--r--   0        0        0      513 2023-06-26 21:34:54.108589 ni_measurementlink_service-1.1.0.dev2/ni_measurementlink_service/__init__.py
+-rw-r--r--   0        0        0       62 2023-06-26 21:34:54.108589 ni_measurementlink_service-1.1.0.dev2/ni_measurementlink_service/_internal/__init__.py
+-rw-r--r--   0        0        0    10247 2023-06-26 21:34:54.108589 ni_measurementlink_service-1.1.0.dev2/ni_measurementlink_service/_internal/discovery_client.py
+-rw-r--r--   0        0        0    17484 2023-06-26 21:34:54.108589 ni_measurementlink_service-1.1.0.dev2/ni_measurementlink_service/_internal/grpc_servicer.py
+-rw-r--r--   0        0        0       58 2023-06-26 21:34:54.108589 ni_measurementlink_service-1.1.0.dev2/ni_measurementlink_service/_internal/parameter/__init__.py
+-rw-r--r--   0        0        0     5400 2023-06-26 21:34:54.108589 ni_measurementlink_service-1.1.0.dev2/ni_measurementlink_service/_internal/parameter/metadata.py
+-rw-r--r--   0        0        0     9237 2023-06-26 21:34:54.108589 ni_measurementlink_service-1.1.0.dev2/ni_measurementlink_service/_internal/parameter/serialization_strategy.py
+-rw-r--r--   0        0        0     8298 2023-06-26 21:34:54.108589 ni_measurementlink_service-1.1.0.dev2/ni_measurementlink_service/_internal/parameter/serializer.py
+-rw-r--r--   0        0        0     3933 2023-06-26 21:34:54.108589 ni_measurementlink_service-1.1.0.dev2/ni_measurementlink_service/_internal/service_manager.py
+-rw-r--r--   0        0        0       33 2023-06-26 21:34:54.108589 ni_measurementlink_service-1.1.0.dev2/ni_measurementlink_service/_internal/stubs/__init__.py
+-rw-r--r--   0        0        0       33 2023-06-26 21:34:54.108589 ni_measurementlink_service-1.1.0.dev2/ni_measurementlink_service/_internal/stubs/ni/__init__.py
+-rw-r--r--   0        0        0       33 2023-06-26 21:34:54.108589 ni_measurementlink_service-1.1.0.dev2/ni_measurementlink_service/_internal/stubs/ni/measurementlink/__init__.py
+-rw-r--r--   0        0        0       33 2023-06-26 21:34:54.108589 ni_measurementlink_service-1.1.0.dev2/ni_measurementlink_service/_internal/stubs/ni/measurementlink/discovery/__init__.py
+-rw-r--r--   0        0        0       33 2023-06-26 21:34:54.108589 ni_measurementlink_service-1.1.0.dev2/ni_measurementlink_service/_internal/stubs/ni/measurementlink/discovery/v1/__init__.py
+-rw-r--r--   0        0        0     4264 2023-06-26 21:34:54.108589 ni_measurementlink_service-1.1.0.dev2/ni_measurementlink_service/_internal/stubs/ni/measurementlink/discovery/v1/discovery_service_pb2.py
+-rw-r--r--   0        0        0     8921 2023-06-26 21:34:54.108589 ni_measurementlink_service-1.1.0.dev2/ni_measurementlink_service/_internal/stubs/ni/measurementlink/discovery/v1/discovery_service_pb2.pyi
+-rw-r--r--   0        0        0    10817 2023-06-26 21:34:54.108589 ni_measurementlink_service-1.1.0.dev2/ni_measurementlink_service/_internal/stubs/ni/measurementlink/discovery/v1/discovery_service_pb2_grpc.py
+-rw-r--r--   0        0        0     6348 2023-06-26 21:34:54.108589 ni_measurementlink_service-1.1.0.dev2/ni_measurementlink_service/_internal/stubs/ni/measurementlink/discovery/v1/discovery_service_pb2_grpc.pyi
+-rw-r--r--   0        0        0       33 2023-06-26 21:34:54.108589 ni_measurementlink_service-1.1.0.dev2/ni_measurementlink_service/_internal/stubs/ni/measurementlink/measurement/__init__.py
+-rw-r--r--   0        0        0       33 2023-06-26 21:34:54.108589 ni_measurementlink_service-1.1.0.dev2/ni_measurementlink_service/_internal/stubs/ni/measurementlink/measurement/v1/__init__.py
+-rw-r--r--   0        0        0     5345 2023-06-26 21:34:54.108589 ni_measurementlink_service-1.1.0.dev2/ni_measurementlink_service/_internal/stubs/ni/measurementlink/measurement/v1/measurement_service_pb2.py
+-rw-r--r--   0        0        0    13678 2023-06-26 21:34:54.108589 ni_measurementlink_service-1.1.0.dev2/ni_measurementlink_service/_internal/stubs/ni/measurementlink/measurement/v1/measurement_service_pb2.pyi
+-rw-r--r--   0        0        0     5546 2023-06-26 21:34:54.108589 ni_measurementlink_service-1.1.0.dev2/ni_measurementlink_service/_internal/stubs/ni/measurementlink/measurement/v1/measurement_service_pb2_grpc.py
+-rw-r--r--   0        0        0     2362 2023-06-26 21:34:54.108589 ni_measurementlink_service-1.1.0.dev2/ni_measurementlink_service/_internal/stubs/ni/measurementlink/measurement/v1/measurement_service_pb2_grpc.pyi
+-rw-r--r--   0        0        0       33 2023-06-26 21:34:54.108589 ni_measurementlink_service-1.1.0.dev2/ni_measurementlink_service/_internal/stubs/ni/measurementlink/measurement/v2/__init__.py
+-rw-r--r--   0        0        0     5777 2023-06-26 21:34:54.108589 ni_measurementlink_service-1.1.0.dev2/ni_measurementlink_service/_internal/stubs/ni/measurementlink/measurement/v2/measurement_service_pb2.py
+-rw-r--r--   0        0        0    15086 2023-06-26 21:34:54.108589 ni_measurementlink_service-1.1.0.dev2/ni_measurementlink_service/_internal/stubs/ni/measurementlink/measurement/v2/measurement_service_pb2.pyi
+-rw-r--r--   0        0        0     5549 2023-06-26 21:34:54.108589 ni_measurementlink_service-1.1.0.dev2/ni_measurementlink_service/_internal/stubs/ni/measurementlink/measurement/v2/measurement_service_pb2_grpc.py
+-rw-r--r--   0        0        0     2412 2023-06-26 21:34:54.108589 ni_measurementlink_service-1.1.0.dev2/ni_measurementlink_service/_internal/stubs/ni/measurementlink/measurement/v2/measurement_service_pb2_grpc.pyi
+-rw-r--r--   0        0        0     1532 2023-06-26 21:34:54.108589 ni_measurementlink_service-1.1.0.dev2/ni_measurementlink_service/_internal/stubs/ni/measurementlink/pin_map_context_pb2.py
+-rw-r--r--   0        0        0     1314 2023-06-26 21:34:54.108589 ni_measurementlink_service-1.1.0.dev2/ni_measurementlink_service/_internal/stubs/ni/measurementlink/pin_map_context_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-06-26 21:34:54.108589 ni_measurementlink_service-1.1.0.dev2/ni_measurementlink_service/_internal/stubs/ni/measurementlink/pin_map_context_pb2_grpc.py
+-rw-r--r--   0        0        0       76 2023-06-26 21:34:54.108589 ni_measurementlink_service-1.1.0.dev2/ni_measurementlink_service/_internal/stubs/ni/measurementlink/pin_map_context_pb2_grpc.pyi
+-rw-r--r--   0        0        0       33 2023-06-26 21:34:54.108589 ni_measurementlink_service-1.1.0.dev2/ni_measurementlink_service/_internal/stubs/ni/measurementlink/pinmap/__init__.py
+-rw-r--r--   0        0        0       33 2023-06-26 21:34:54.108589 ni_measurementlink_service-1.1.0.dev2/ni_measurementlink_service/_internal/stubs/ni/measurementlink/pinmap/v1/__init__.py
+-rw-r--r--   0        0        0     6202 2023-06-26 21:34:54.108589 ni_measurementlink_service-1.1.0.dev2/ni_measurementlink_service/_internal/stubs/ni/measurementlink/pinmap/v1/pin_map_service_pb2.py
+-rw-r--r--   0        0        0    18188 2023-06-26 21:34:54.108589 ni_measurementlink_service-1.1.0.dev2/ni_measurementlink_service/_internal/stubs/ni/measurementlink/pinmap/v1/pin_map_service_pb2.pyi
+-rw-r--r--   0        0        0    14078 2023-06-26 21:34:54.108589 ni_measurementlink_service-1.1.0.dev2/ni_measurementlink_service/_internal/stubs/ni/measurementlink/pinmap/v1/pin_map_service_pb2_grpc.py
+-rw-r--r--   0        0        0     6880 2023-06-26 21:34:54.108589 ni_measurementlink_service-1.1.0.dev2/ni_measurementlink_service/_internal/stubs/ni/measurementlink/pinmap/v1/pin_map_service_pb2_grpc.pyi
+-rw-r--r--   0        0        0       33 2023-06-26 21:34:54.108589 ni_measurementlink_service-1.1.0.dev2/ni_measurementlink_service/_internal/stubs/ni/measurementlink/sessionmanagement/__init__.py
+-rw-r--r--   0        0        0       33 2023-06-26 21:34:54.108589 ni_measurementlink_service-1.1.0.dev2/ni_measurementlink_service/_internal/stubs/ni/measurementlink/sessionmanagement/v1/__init__.py
+-rw-r--r--   0        0        0     5955 2023-06-26 21:34:54.108589 ni_measurementlink_service-1.1.0.dev2/ni_measurementlink_service/_internal/stubs/ni/measurementlink/sessionmanagement/v1/session_management_service_pb2.py
+-rw-r--r--   0        0        0    13370 2023-06-26 21:34:54.108589 ni_measurementlink_service-1.1.0.dev2/ni_measurementlink_service/_internal/stubs/ni/measurementlink/sessionmanagement/v1/session_management_service_pb2.pyi
+-rw-r--r--   0        0        0    13882 2023-06-26 21:34:54.108589 ni_measurementlink_service-1.1.0.dev2/ni_measurementlink_service/_internal/stubs/ni/measurementlink/sessionmanagement/v1/session_management_service_pb2_grpc.py
+-rw-r--r--   0        0        0     7537 2023-06-26 21:34:54.108589 ni_measurementlink_service-1.1.0.dev2/ni_measurementlink_service/_internal/stubs/ni/measurementlink/sessionmanagement/v1/session_management_service_pb2_grpc.pyi
+-rw-r--r--   0        0        0      709 2023-06-26 21:34:54.108589 ni_measurementlink_service-1.1.0.dev2/ni_measurementlink_service/_internal/stubs/proto/README.md
+-rw-r--r--   0        0        0     6052 2023-06-26 21:34:54.108589 ni_measurementlink_service-1.1.0.dev2/ni_measurementlink_service/_internal/stubs/proto/ni/measurementlink/discovery/v1/discovery_service.proto
+-rw-r--r--   0        0        0     6650 2023-06-26 21:34:54.108589 ni_measurementlink_service-1.1.0.dev2/ni_measurementlink_service/_internal/stubs/proto/ni/measurementlink/measurement/v1/measurement_service.proto
+-rw-r--r--   0        0        0     7228 2023-06-26 21:34:54.108589 ni_measurementlink_service-1.1.0.dev2/ni_measurementlink_service/_internal/stubs/proto/ni/measurementlink/measurement/v2/measurement_service.proto
+-rw-r--r--   0        0        0      712 2023-06-26 21:34:54.108589 ni_measurementlink_service-1.1.0.dev2/ni_measurementlink_service/_internal/stubs/proto/ni/measurementlink/pin_map_context.proto
+-rw-r--r--   0        0        0     9622 2023-06-26 21:34:54.108589 ni_measurementlink_service-1.1.0.dev2/ni_measurementlink_service/_internal/stubs/proto/ni/measurementlink/pinmap/v1/pin_map_service.proto
+-rw-r--r--   0        0        0     8468 2023-06-26 21:34:54.108589 ni_measurementlink_service-1.1.0.dev2/ni_measurementlink_service/_internal/stubs/proto/ni/measurementlink/sessionmanagement/v1/session_management_service.proto
+-rw-r--r--   0        0        0     2426 2023-06-26 21:34:54.108589 ni_measurementlink_service-1.1.0.dev2/ni_measurementlink_service/_internal/stubs/proto/session.proto
+-rw-r--r--   0        0        0     4196 2023-06-26 21:34:54.112589 ni_measurementlink_service-1.1.0.dev2/ni_measurementlink_service/_internal/stubs/session_pb2.py
+-rw-r--r--   0        0        0     8735 2023-06-26 21:34:54.112589 ni_measurementlink_service-1.1.0.dev2/ni_measurementlink_service/_internal/stubs/session_pb2.pyi
+-rw-r--r--   0        0        0     8948 2023-06-26 21:34:54.112589 ni_measurementlink_service-1.1.0.dev2/ni_measurementlink_service/_internal/stubs/session_pb2_grpc.py
+-rw-r--r--   0        0        0     2873 2023-06-26 21:34:54.112589 ni_measurementlink_service-1.1.0.dev2/ni_measurementlink_service/_internal/stubs/session_pb2_grpc.pyi
+-rw-r--r--   0        0        0       35 2023-06-26 21:34:54.112589 ni_measurementlink_service-1.1.0.dev2/ni_measurementlink_service/_internal/utilities/__init__.py
+-rw-r--r--   0        0        0       37 2023-06-26 21:34:54.112589 ni_measurementlink_service-1.1.0.dev2/ni_measurementlink_service/measurement/__init__.py
+-rw-r--r--   0        0        0     3520 2023-06-26 21:34:54.112589 ni_measurementlink_service-1.1.0.dev2/ni_measurementlink_service/measurement/info.py
+-rw-r--r--   0        0        0    15001 2023-06-26 21:34:54.112589 ni_measurementlink_service-1.1.0.dev2/ni_measurementlink_service/measurement/service.py
+-rw-r--r--   0        0        0        0 2023-06-26 21:34:54.112589 ni_measurementlink_service-1.1.0.dev2/ni_measurementlink_service/py.typed
+-rw-r--r--   0        0        0    19771 2023-06-26 21:34:54.112589 ni_measurementlink_service-1.1.0.dev2/ni_measurementlink_service/session_management.py
+-rw-r--r--   0        0        0     2831 2023-06-26 21:35:52.329345 ni_measurementlink_service-1.1.0.dev2/pyproject.toml
+-rw-r--r--   0        0        0    19614 1970-01-01 00:00:00.000000 ni_measurementlink_service-1.1.0.dev2/setup.py
+-rw-r--r--   0        0        0    17972 1970-01-01 00:00:00.000000 ni_measurementlink_service-1.1.0.dev2/PKG-INFO
```

### Comparing `ni_measurementlink_service-1.1.0.dev1/LICENSE` & `ni_measurementlink_service-1.1.0.dev2/LICENSE`

 * *Files identical despite different names*

### Comparing `ni_measurementlink_service-1.1.0.dev1/README.md` & `ni_measurementlink_service-1.1.0.dev2/README.md`

 * *Files 3% similar despite different names*

```diff
@@ -60,14 +60,15 @@
 ## Examples
 
 The `examples` directory contains example measurements for MeasurementLink 2023 Q3 or later. If
 you are using a previous version of MeasurementLink, download the appropriate examples:
 
 - MeasurementLink 2023 Q1: [measurementlink-python-examples-1.0.1.zip](https://github.com/ni/measurementlink-python/releases/download/1.0.1/measurementlink-python-examples-1.0.1.zip)
 - MeasurementLink 2023 Q2: [measurementlink-python-examples-1.0.1.zip](https://github.com/ni/measurementlink-python/releases/download/1.0.1/measurementlink-python-examples-1.0.1.zip)
+- MeasurementLink 2023 Q3: [measurementlink-python-examples-1.1.0.zip](https://github.com/ni/measurementlink-python/releases/download/1.1.0/measurementlink-python-examples-1.1.0.zip)
 
 For more information on setting up and running the example measurements, see the included `README.md` file.
 
 For best results, use the example measurements corresponding to the version of MeasurementLink
 that you are using. Newer examples may demonstrate features that are not available in older
 versions of MeasurementLink.
 
@@ -187,15 +188,17 @@
 
 To statically register a measurement service with the MeasurementLink discovery service, do the following:
 
 1. Create a [startup batch file](#create-a-batch-file-that-runs-a-python-measurement) or [executable](#create-executable-for-python-scripts) for the measurement service.
 
 2. Edit the measurement service's `.serviceconfig` file and set the `path` value to the filename of the startup batch file or executable.
 
-3. Copy the measurement service's directory (including the `.venv` subdirectory if present, `.serviceconfig` file, and startup batch file) to a subdirectory of `C:\ProgramData\National Instruments\MeasurementLink\Services`. 
+3. Copy the measurement service's directory (including the `.serviceconfig` file and startup batch file) to a subdirectory of `C:\ProgramData\National Instruments\MeasurementLink\Services`.
+> **Note**
+> If you are using a virtual environment, do not copy the `.venv` subdirectory&mdash;the virtual environment must be re-created in the new location.
 
 Once your measurement service is statically registered, the MeasurementLink discovery service makes it visible in supported NI applications.
 
 ### Create a batch file that runs a Python measurement
 
 The batch file used for static registration is responsible for starting the Python Scripts.
```

### Comparing `ni_measurementlink_service-1.1.0.dev1/ni_measurementlink_service/__init__.py` & `ni_measurementlink_service-1.1.0.dev2/ni_measurementlink_service/__init__.py`

 * *Files identical despite different names*

### Comparing `ni_measurementlink_service-1.1.0.dev1/ni_measurementlink_service/_internal/discovery_client.py` & `ni_measurementlink_service-1.1.0.dev2/ni_measurementlink_service/_internal/discovery_client.py`

 * *Files 3% similar despite different names*

```diff
@@ -20,20 +20,14 @@
     import errno
     import msvcrt
 
     import win32con
     import win32file
     import winerror
 
-
-_PROVIDED_MEASUREMENT_SERVICES = [
-    "ni.measurementlink.measurement.v1.MeasurementService",
-    "ni.measurementlink.measurement.v2.MeasurementService",
-]
-
 _logger = logging.getLogger(__name__)
 
 
 class ServiceLocation(typing.NamedTuple):
     """Represents the location of a service."""
 
     location: str
@@ -107,15 +101,15 @@
             service_location.location = "localhost"
             service_location.insecure_port = service_port
             # Service Descriptor
             service_descriptor = discovery_service_pb2.ServiceDescriptor()
             service_descriptor.display_name = measurement_info.display_name
             service_descriptor.service_class = service_info.service_class
             service_descriptor.description_url = service_info.description_url
-            service_descriptor.provided_interfaces.extend(_PROVIDED_MEASUREMENT_SERVICES)
+            service_descriptor.provided_interfaces.extend(service_info.provided_interfaces)
 
             # Registration Request Creation
             request = discovery_service_pb2.RegisterServiceRequest(
                 location=service_location, service_description=service_descriptor
             )
             # Registration RPC Call
             register_response = self.stub.RegisterService(request)
```

### Comparing `ni_measurementlink_service-1.1.0.dev1/ni_measurementlink_service/_internal/grpc_servicer.py` & `ni_measurementlink_service-1.1.0.dev2/ni_measurementlink_service/_internal/grpc_servicer.py`

 * *Files 7% similar despite different names*

```diff
@@ -20,70 +20,85 @@
     measurement_service_pb2_grpc as v1_measurement_service_pb2_grpc,
 )
 from ni_measurementlink_service._internal.stubs.ni.measurementlink.measurement.v2 import (
     measurement_service_pb2 as v2_measurement_service_pb2,
     measurement_service_pb2_grpc as v2_measurement_service_pb2_grpc,
 )
 from ni_measurementlink_service.measurement.info import MeasurementInfo
+from ni_measurementlink_service.session_management import PinMapContext
 
 
 class MeasurementServiceContext:
     """Accessor for the Measurement Service's context-local state."""
 
     def __init__(
-        self, grpc_context: grpc.ServicerContext, pin_map_context: pin_map_context_pb2.PinMapContext
-    ):
+        self,
+        grpc_context: grpc.ServicerContext,
+        pin_map_context: PinMapContext,
+    ) -> None:
         """Initialize the Measurement Service Context."""
         self._grpc_context: grpc.ServicerContext = grpc_context
-        self._pin_map_context: pin_map_context_pb2.PinMapContext = pin_map_context
+        self._pin_map_context: PinMapContext = pin_map_context
         self._is_complete: bool = False
 
-    def mark_complete(self):
+    def mark_complete(self) -> None:
         """Mark the current RPC as complete."""
         self._is_complete = True
 
     @property
-    def grpc_context(self):
+    def grpc_context(self) -> grpc.ServicerContext:
         """Get the context for the RPC."""
         return self._grpc_context
 
     @property
-    def pin_map_context(self):
+    def pin_map_context(self) -> PinMapContext:
         """Get the pin map context for the RPC."""
         return self._pin_map_context
 
-    def add_cancel_callback(self, cancel_callback: Callable):
+    def add_cancel_callback(self, cancel_callback: Callable[[], None]) -> None:
         """Add a callback that is invoked when the RPC is canceled."""
 
         def grpc_callback():
             if not self._is_complete:
                 cancel_callback()
 
         self._grpc_context.add_callback(grpc_callback)
 
-    def cancel(self):
+    def cancel(self) -> None:
         """Cancel the RPC."""
         if not self._is_complete:
             self._grpc_context.cancel()
 
     @property
-    def time_remaining(self):
+    def time_remaining(self) -> float:
         """Get the time remaining for the RPC."""
         return self._grpc_context.time_remaining()
 
-    def abort(self, code, details):
+    def abort(self, code: grpc.StatusCode, details: str) -> None:
         """Aborts the RPC."""
         self._grpc_context.abort(code, details)
 
 
 measurement_service_context: ContextVar[MeasurementServiceContext] = ContextVar(
     "measurement_service_context"
 )
 
 
+def _convert_pin_map_context_from_grpc(
+    grpc_pin_map_context: pin_map_context_pb2.PinMapContext,
+) -> PinMapContext:
+    # The protobuf PinMapContext sites field is a RepeatedScalarContainer, not a list.
+    # Constructing a protobuf PinMapContext with sites=None sets sites to an empty
+    # RepeatedScalarContainer, not None.
+    return PinMapContext(
+        pin_map_id=grpc_pin_map_context.pin_map_id,
+        sites=list(grpc_pin_map_context.sites),
+    )
+
+
 def _get_mapping_by_parameter_name(
     mapping_by_id: Dict[int, Any], measure_function: Callable[[], None]
 ) -> Dict[str, Any]:
     """Transform the mapping by id to mapping by parameter names of the measurement function.
 
     Args
     ----
@@ -227,17 +242,16 @@
             self.configuration_metadata, request.configuration_parameters.value
         )
 
         # Calling the registered measurement
         mapping_by_variable_name = _get_mapping_by_parameter_name(
             mapping_by_id, self.measure_function
         )
-        token = measurement_service_context.set(
-            MeasurementServiceContext(context, request.pin_map_context)
-        )
+        pin_map_context = _convert_pin_map_context_from_grpc(request.pin_map_context)
+        token = measurement_service_context.set(MeasurementServiceContext(context, pin_map_context))
         try:
             return_value = self.measure_function(**mapping_by_variable_name)
             if isinstance(return_value, collections.abc.Generator):
                 with contextlib.closing(return_value) as output_iter:
                     outputs = None
                     try:
                         while True:
@@ -371,17 +385,16 @@
             self.configuration_metadata, request.configuration_parameters.value
         )
 
         # Calling the registered measurement
         mapping_by_variable_name = _get_mapping_by_parameter_name(
             mapping_by_id, self.measure_function
         )
-        token = measurement_service_context.set(
-            MeasurementServiceContext(context, request.pin_map_context)
-        )
+        pin_map_context = _convert_pin_map_context_from_grpc(request.pin_map_context)
+        token = measurement_service_context.set(MeasurementServiceContext(context, pin_map_context))
         try:
             return_value = self.measure_function(**mapping_by_variable_name)
             if isinstance(return_value, collections.abc.Generator):
                 with contextlib.closing(return_value) as output_iter:
                     try:
                         while True:
                             outputs = next(output_iter)
```

### Comparing `ni_measurementlink_service-1.1.0.dev1/ni_measurementlink_service/_internal/parameter/serialization_strategy.py` & `ni_measurementlink_service-1.1.0.dev2/ni_measurementlink_service/_internal/parameter/serialization_strategy.py`

 * *Files 1% similar despite different names*

```diff
@@ -149,36 +149,39 @@
         type_pb2.Field.TYPE_DOUBLE: (DoubleEncoder, DoubleArrayEncoder),
         type_pb2.Field.TYPE_INT32: (IntEncoder, IntArrayEncoder),
         type_pb2.Field.TYPE_INT64: (IntEncoder, IntArrayEncoder),
         type_pb2.Field.TYPE_UINT32: (UIntEncoder, UIntArrayEncoder),
         type_pb2.Field.TYPE_UINT64: (UIntEncoder, UIntArrayEncoder),
         type_pb2.Field.TYPE_BOOL: (BoolEncoder, BoolArrayEncoder),
         type_pb2.Field.TYPE_STRING: (StringEncoder, StringArrayEncoder),
+        type_pb2.Field.TYPE_ENUM: (IntEncoder, IntArrayEncoder),
     }
 
     _FIELD_TYPE_TO_DECODER_MAPPING = {
         type_pb2.Field.TYPE_FLOAT: (FloatDecoder, FloatArrayDecoder),
         type_pb2.Field.TYPE_DOUBLE: (DoubleDecoder, DoubleArrayDecoder),
         type_pb2.Field.TYPE_INT32: (Int32Decoder, Int32ArrayDecoder),
         type_pb2.Field.TYPE_INT64: (Int64Decoder, Int64ArrayDecoder),
         type_pb2.Field.TYPE_UINT32: (UInt32Decoder, UInt32ArrayDecoder),
         type_pb2.Field.TYPE_UINT64: (UInt64Decoder, UInt64ArrayDecoder),
         type_pb2.Field.TYPE_BOOL: (BoolDecoder, BoolArrayDecoder),
         type_pb2.Field.TYPE_STRING: (StringDecoder, StringArrayDecoder),
+        type_pb2.Field.TYPE_ENUM: (Int32Decoder, Int32ArrayDecoder),
     }
 
     _TYPE_DEFAULT_MAPPING = {
         type_pb2.Field.TYPE_FLOAT: float(),
         type_pb2.Field.TYPE_DOUBLE: float(),
         type_pb2.Field.TYPE_INT32: int(),
         type_pb2.Field.TYPE_INT64: int(),
         type_pb2.Field.TYPE_UINT32: int(),
         type_pb2.Field.TYPE_UINT64: int(),
         type_pb2.Field.TYPE_BOOL: bool(),
         type_pb2.Field.TYPE_STRING: str(),
+        type_pb2.Field.TYPE_ENUM: int(),
     }
 
     @staticmethod
     def get_encoder(
         type: type_pb2.Field.Kind.ValueType, repeated: bool
     ) -> Callable[[int], Callable]:
         """Get the Scalar Encoder or Vector Encoder for the specified type based on repeated bool.
```

### Comparing `ni_measurementlink_service-1.1.0.dev1/ni_measurementlink_service/_internal/parameter/serializer.py` & `ni_measurementlink_service-1.1.0.dev2/ni_measurementlink_service/_internal/parameter/serializer.py`

 * *Files 16% similar despite different names*

```diff
@@ -2,15 +2,19 @@
 
 from io import BytesIO
 from typing import Any, Dict, Sequence
 
 from google.protobuf.internal import encoder
 
 from ni_measurementlink_service._internal.parameter import serialization_strategy
-from ni_measurementlink_service._internal.parameter.metadata import ParameterMetadata
+from ni_measurementlink_service._internal.parameter.metadata import (
+    ParameterMetadata,
+    get_enum_values_annotation,
+)
+from ni_measurementlink_service.measurement.info import TypeSpecialization
 
 _GRPC_WIRE_TYPE_BIT_WIDTH = 3
 
 
 def deserialize_parameters(
     parameter_metadata_dict: Dict[int, ParameterMetadata], parameter_bytes: bytes
 ) -> Dict[int, Any]:
@@ -27,14 +31,18 @@
         Dict[int, Any]: Deserialized parameters by ID
 
     """
     # Getting overlapping parameters
     overlapping_parameter_by_id = _get_overlapping_parameters(
         parameter_metadata_dict, parameter_bytes
     )
+
+    # Deserialization enum parameters to their user-defined type
+    _deserialize_enum_parameters(parameter_metadata_dict, overlapping_parameter_by_id)
+
     # Adding missing parameters with type defaults
     missing_parameters = _get_missing_parameters(
         parameter_metadata_dict, overlapping_parameter_by_id
     )
     overlapping_parameter_by_id.update(missing_parameters)
     return overlapping_parameter_by_id
 
@@ -63,14 +71,23 @@
             parameter_metadata.type,
             parameter_metadata.repeated,
         )
         type_default_value = serialization_strategy.Context.get_type_default(
             parameter_metadata.type,
             parameter_metadata.repeated,
         )
+        # Convert enum parameters to their underlying value.
+        if (
+            parameter_metadata.annotations.get("ni/type_specialization")
+            == TypeSpecialization.Enum.value
+        ):
+            if parameter_metadata.repeated:
+                parameter = [x.value for x in parameter]
+            else:
+                parameter = parameter.value
         # Skipping serialization if the value is None or if its a type default value.
         if parameter is not None and parameter != type_default_value:
             inner_encoder = encoder(i + 1)
             inner_encoder(serialize_buffer.write, parameter, None)
     return serialize_buffer.getvalue()
 
 
@@ -172,11 +189,50 @@
     -------
         Dict[int, Any]: Missing parameter(as type defaults) by ID.
 
     """
     missing_parameters = {}
     for key, value in parameter_metadata_dict.items():
         if key not in parameter_by_id:
-            missing_parameters[key] = serialization_strategy.Context.get_type_default(
-                value.type, value.repeated
-            )
+            enum_annotations = get_enum_values_annotation(value)
+            if enum_annotations and not value.repeated:
+                enum_type = _get_enum_type(value)
+                missing_parameters[key] = enum_type(0)
+            else:
+                missing_parameters[key] = serialization_strategy.Context.get_type_default(
+                    value.type, value.repeated
+                )
     return missing_parameters
+
+
+def _deserialize_enum_parameters(
+    parameter_metadata_dict: Dict[int, ParameterMetadata], parameter_by_id: Dict[int, Any]
+) -> None:
+    """Converts all enums in `parameter_by_id` to the user defined enum type.
+
+    Args
+    ----
+        parameter_metadata_dict (Dict[int, ParameterMetadata]): Parameter metadata by id.
+
+        parameter_by_id (Dict[int, Any]): Parameters by ID to compare the metadata with.
+
+    Returns
+    -------
+        None: No return value.
+
+    """
+    for id, value in parameter_by_id.items():
+        parameter_metadata = parameter_metadata_dict[id]
+        if get_enum_values_annotation(parameter_metadata):
+            enum_type = _get_enum_type(parameter_metadata)
+            if parameter_metadata.repeated:
+                for index, member_value in enumerate(value):
+                    parameter_by_id[id][index] = enum_type(member_value)
+            else:
+                parameter_by_id[id] = enum_type(value)
+
+
+def _get_enum_type(parameter_metadata: ParameterMetadata) -> type:
+    if parameter_metadata.repeated and len(parameter_metadata.default_value) > 0:
+        return type(parameter_metadata.default_value[0])
+    else:
+        return type(parameter_metadata.default_value)
```

### Comparing `ni_measurementlink_service-1.1.0.dev1/ni_measurementlink_service/_internal/service_manager.py` & `ni_measurementlink_service-1.1.0.dev2/ni_measurementlink_service/_internal/service_manager.py`

 * *Files identical despite different names*

### Comparing `ni_measurementlink_service-1.1.0.dev1/ni_measurementlink_service/_internal/stubs/ni/measurementlink/discovery/v1/discovery_service_pb2.py` & `ni_measurementlink_service-1.1.0.dev2/ni_measurementlink_service/_internal/stubs/ni/measurementlink/discovery/v1/discovery_service_pb2.py`

 * *Files identical despite different names*

### Comparing `ni_measurementlink_service-1.1.0.dev1/ni_measurementlink_service/_internal/stubs/ni/measurementlink/discovery/v1/discovery_service_pb2.pyi` & `ni_measurementlink_service-1.1.0.dev2/ni_measurementlink_service/_internal/stubs/ni/measurementlink/discovery/v1/discovery_service_pb2.pyi`

 * *Files identical despite different names*

### Comparing `ni_measurementlink_service-1.1.0.dev1/ni_measurementlink_service/_internal/stubs/ni/measurementlink/discovery/v1/discovery_service_pb2_grpc.py` & `ni_measurementlink_service-1.1.0.dev2/ni_measurementlink_service/_internal/stubs/ni/measurementlink/discovery/v1/discovery_service_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `ni_measurementlink_service-1.1.0.dev1/ni_measurementlink_service/_internal/stubs/ni/measurementlink/measurement/v1/measurement_service_pb2.py` & `ni_measurementlink_service-1.1.0.dev2/ni_measurementlink_service/_internal/stubs/ni/measurementlink/measurement/v1/measurement_service_pb2.py`

 * *Files identical despite different names*

### Comparing `ni_measurementlink_service-1.1.0.dev1/ni_measurementlink_service/_internal/stubs/ni/measurementlink/measurement/v1/measurement_service_pb2.pyi` & `ni_measurementlink_service-1.1.0.dev2/ni_measurementlink_service/_internal/stubs/ni/measurementlink/measurement/v1/measurement_service_pb2.pyi`

 * *Files 0% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 import builtins
 import collections.abc
 import google.protobuf.any_pb2
 import google.protobuf.descriptor
 import google.protobuf.internal.containers
 import google.protobuf.message
 import google.protobuf.type_pb2
-import ni.measurementlink.pin_map_context_pb2
+import ni_measurementlink_service._internal.stubs.ni.measurementlink.pin_map_context_pb2 as ni_measurementlink_pin_map_context_pb2
 import sys
 
 if sys.version_info >= (3, 8):
     import typing as typing_extensions
 else:
     import typing_extensions
 
@@ -68,24 +68,24 @@
     @property
     def configuration_parameters(self) -> google.protobuf.any_pb2.Any:
         """Required. Specifies the configuration to be used for the measurement. Each measurement will define its own set
         of required and optional parameters and generate errors as appropriate if the configuration does not conform
         to valid input ranges.
         """
     @property
-    def pin_map_context(self) -> ni.measurementlink.pin_map_context_pb2.PinMapContext:
+    def pin_map_context(self) -> ni_measurementlink_pin_map_context_pb2.PinMapContext:
         """Optional. Specifies the pin map context for the measurement, if any. This field is optional in that callers
         may not always have a pin map context available to include in the request message. Each measurement will
         define if a valid pin map context is required in order to run or not and generate errors appropriately.
         """
     def __init__(
         self,
         *,
         configuration_parameters: google.protobuf.any_pb2.Any | None = ...,
-        pin_map_context: ni.measurementlink.pin_map_context_pb2.PinMapContext | None = ...,
+        pin_map_context: ni_measurementlink_pin_map_context_pb2.PinMapContext | None = ...,
     ) -> None: ...
     def HasField(self, field_name: typing_extensions.Literal["configuration_parameters", b"configuration_parameters", "pin_map_context", b"pin_map_context"]) -> builtins.bool: ...
     def ClearField(self, field_name: typing_extensions.Literal["configuration_parameters", b"configuration_parameters", "pin_map_context", b"pin_map_context"]) -> None: ...
 
 global___MeasureRequest = MeasureRequest
 
 @typing_extensions.final
```

### Comparing `ni_measurementlink_service-1.1.0.dev1/ni_measurementlink_service/_internal/stubs/ni/measurementlink/measurement/v1/measurement_service_pb2_grpc.py` & `ni_measurementlink_service-1.1.0.dev2/ni_measurementlink_service/_internal/stubs/ni/measurementlink/measurement/v1/measurement_service_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `ni_measurementlink_service-1.1.0.dev1/ni_measurementlink_service/_internal/stubs/ni/measurementlink/measurement/v2/measurement_service_pb2.py` & `ni_measurementlink_service-1.1.0.dev2/ni_measurementlink_service/_internal/stubs/ni/measurementlink/measurement/v2/measurement_service_pb2.py`

 * *Files identical despite different names*

### Comparing `ni_measurementlink_service-1.1.0.dev1/ni_measurementlink_service/_internal/stubs/ni/measurementlink/measurement/v2/measurement_service_pb2.pyi` & `ni_measurementlink_service-1.1.0.dev2/ni_measurementlink_service/_internal/stubs/ni/measurementlink/measurement/v2/measurement_service_pb2.pyi`

 * *Files 1% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 import builtins
 import collections.abc
 import google.protobuf.any_pb2
 import google.protobuf.descriptor
 import google.protobuf.internal.containers
 import google.protobuf.message
 import google.protobuf.type_pb2
-import ni.measurementlink.pin_map_context_pb2
+import ni_measurementlink_service._internal.stubs.ni.measurementlink.pin_map_context_pb2 as ni_measurementlink_pin_map_context_pb2
 import sys
 
 if sys.version_info >= (3, 8):
     import typing as typing_extensions
 else:
     import typing_extensions
 
@@ -68,24 +68,24 @@
     @property
     def configuration_parameters(self) -> google.protobuf.any_pb2.Any:
         """Required. Specifies the configuration to be used for the measurement. Each measurement will define its own set
         of required and optional parameters and generate errors as appropriate if the configuration does not conform
         to valid input ranges.
         """
     @property
-    def pin_map_context(self) -> ni.measurementlink.pin_map_context_pb2.PinMapContext:
+    def pin_map_context(self) -> ni_measurementlink_pin_map_context_pb2.PinMapContext:
         """Optional. Specifies the pin map context for the measurement, if any. This field is optional in that callers
         may not always have a pin map context available to include in the request message. Each measurement will
         define if a valid pin map context is required in order to run or not and generate errors appropriately.
         """
     def __init__(
         self,
         *,
         configuration_parameters: google.protobuf.any_pb2.Any | None = ...,
-        pin_map_context: ni.measurementlink.pin_map_context_pb2.PinMapContext | None = ...,
+        pin_map_context: ni_measurementlink_pin_map_context_pb2.PinMapContext | None = ...,
     ) -> None: ...
     def HasField(self, field_name: typing_extensions.Literal["configuration_parameters", b"configuration_parameters", "pin_map_context", b"pin_map_context"]) -> builtins.bool: ...
     def ClearField(self, field_name: typing_extensions.Literal["configuration_parameters", b"configuration_parameters", "pin_map_context", b"pin_map_context"]) -> None: ...
 
 global___MeasureRequest = MeasureRequest
 
 @typing_extensions.final
```

### Comparing `ni_measurementlink_service-1.1.0.dev1/ni_measurementlink_service/_internal/stubs/ni/measurementlink/measurement/v2/measurement_service_pb2_grpc.py` & `ni_measurementlink_service-1.1.0.dev2/ni_measurementlink_service/_internal/stubs/ni/measurementlink/measurement/v2/measurement_service_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `ni_measurementlink_service-1.1.0.dev1/ni_measurementlink_service/_internal/stubs/ni/measurementlink/pin_map_context_pb2.py` & `ni_measurementlink_service-1.1.0.dev2/ni_measurementlink_service/_internal/stubs/ni/measurementlink/pin_map_context_pb2.py`

 * *Files identical despite different names*

### Comparing `ni_measurementlink_service-1.1.0.dev1/ni_measurementlink_service/_internal/stubs/ni/measurementlink/pin_map_context_pb2.pyi` & `ni_measurementlink_service-1.1.0.dev2/ni_measurementlink_service/_internal/stubs/ni/measurementlink/pin_map_context_pb2.pyi`

 * *Files identical despite different names*

### Comparing `ni_measurementlink_service-1.1.0.dev1/ni_measurementlink_service/_internal/stubs/ni/measurementlink/pinmap/v1/pin_map_service_pb2.py` & `ni_measurementlink_service-1.1.0.dev2/ni_measurementlink_service/_internal/stubs/ni/measurementlink/pinmap/v1/pin_map_service_pb2.py`

 * *Files identical despite different names*

### Comparing `ni_measurementlink_service-1.1.0.dev1/ni_measurementlink_service/_internal/stubs/ni/measurementlink/pinmap/v1/pin_map_service_pb2.pyi` & `ni_measurementlink_service-1.1.0.dev2/ni_measurementlink_service/_internal/stubs/ni/measurementlink/pinmap/v1/pin_map_service_pb2.pyi`

 * *Files identical despite different names*

### Comparing `ni_measurementlink_service-1.1.0.dev1/ni_measurementlink_service/_internal/stubs/ni/measurementlink/pinmap/v1/pin_map_service_pb2_grpc.py` & `ni_measurementlink_service-1.1.0.dev2/ni_measurementlink_service/_internal/stubs/ni/measurementlink/pinmap/v1/pin_map_service_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `ni_measurementlink_service-1.1.0.dev1/ni_measurementlink_service/_internal/stubs/ni/measurementlink/sessionmanagement/v1/session_management_service_pb2.py` & `ni_measurementlink_service-1.1.0.dev2/ni_measurementlink_service/_internal/stubs/ni/measurementlink/sessionmanagement/v1/session_management_service_pb2.py`

 * *Files identical despite different names*

### Comparing `ni_measurementlink_service-1.1.0.dev1/ni_measurementlink_service/_internal/stubs/ni/measurementlink/sessionmanagement/v1/session_management_service_pb2.pyi` & `ni_measurementlink_service-1.1.0.dev2/ni_measurementlink_service/_internal/stubs/ni/measurementlink/sessionmanagement/v1/session_management_service_pb2.pyi`

 * *Files 1% similar despite different names*

```diff
@@ -3,16 +3,16 @@
 isort:skip_file
 """
 import builtins
 import collections.abc
 import google.protobuf.descriptor
 import google.protobuf.internal.containers
 import google.protobuf.message
-import ni.measurementlink.pin_map_context_pb2
-import session_pb2
+import ni_measurementlink_service._internal.stubs.ni.measurementlink.pin_map_context_pb2 as ni_measurementlink_pin_map_context_pb2
+from ni_measurementlink_service._internal.stubs import session_pb2
 import sys
 
 if sys.version_info >= (3, 8):
     import typing as typing_extensions
 else:
     import typing_extensions
 
@@ -112,15 +112,15 @@
     DESCRIPTOR: google.protobuf.descriptor.Descriptor
 
     PIN_MAP_CONTEXT_FIELD_NUMBER: builtins.int
     PIN_OR_RELAY_NAMES_FIELD_NUMBER: builtins.int
     INSTRUMENT_TYPE_ID_FIELD_NUMBER: builtins.int
     TIMEOUT_IN_MILLISECONDS_FIELD_NUMBER: builtins.int
     @property
-    def pin_map_context(self) -> ni.measurementlink.pin_map_context_pb2.PinMapContext:
+    def pin_map_context(self) -> ni_measurementlink_pin_map_context_pb2.PinMapContext:
         """Required. Includes the pin map ID for the pin map in the Pin Map Service, as well as the list of sites for the measurement."""
     @property
     def pin_or_relay_names(self) -> google.protobuf.internal.containers.RepeatedScalarFieldContainer[builtins.str]:
         """Optional. List of pins, pin groups, relays, or relay groups to use for the measurement. If unspecified, reserve sessions for all pins and relays in the registered pin map resource."""
     instrument_type_id: builtins.str
     """Optional. Instrument type ID for the measurement. If unspecified, reserve sessions for all instrument types connected in the registered pin map resource.
     Pin maps have built in instrument definitions using the following NI driver based instrument type ids:
@@ -136,15 +136,15 @@
     timeout_in_milliseconds: builtins.int
     """Optional. Timeout for the reservation request.
     Allowed values: 0 (non-blocking, fails immediately if resources cannot be reserved), -1 (infinite timeout), or any other positive numeric value (wait for that number of milliseconds)
     """
     def __init__(
         self,
         *,
-        pin_map_context: ni.measurementlink.pin_map_context_pb2.PinMapContext | None = ...,
+        pin_map_context: ni_measurementlink_pin_map_context_pb2.PinMapContext | None = ...,
         pin_or_relay_names: collections.abc.Iterable[builtins.str] | None = ...,
         instrument_type_id: builtins.str = ...,
         timeout_in_milliseconds: builtins.int = ...,
     ) -> None: ...
     def HasField(self, field_name: typing_extensions.Literal["pin_map_context", b"pin_map_context"]) -> builtins.bool: ...
     def ClearField(self, field_name: typing_extensions.Literal["instrument_type_id", b"instrument_type_id", "pin_map_context", b"pin_map_context", "pin_or_relay_names", b"pin_or_relay_names", "timeout_in_milliseconds", b"timeout_in_milliseconds"]) -> None: ...
```

### Comparing `ni_measurementlink_service-1.1.0.dev1/ni_measurementlink_service/_internal/stubs/ni/measurementlink/sessionmanagement/v1/session_management_service_pb2_grpc.py` & `ni_measurementlink_service-1.1.0.dev2/ni_measurementlink_service/_internal/stubs/ni/measurementlink/sessionmanagement/v1/session_management_service_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `ni_measurementlink_service-1.1.0.dev1/ni_measurementlink_service/_internal/stubs/proto/README.md` & `ni_measurementlink_service-1.1.0.dev2/ni_measurementlink_service/_internal/stubs/proto/README.md`

 * *Files identical despite different names*

### Comparing `ni_measurementlink_service-1.1.0.dev1/ni_measurementlink_service/_internal/stubs/proto/ni/measurementlink/discovery/v1/discovery_service.proto` & `ni_measurementlink_service-1.1.0.dev2/ni_measurementlink_service/_internal/stubs/proto/ni/measurementlink/discovery/v1/discovery_service.proto`

 * *Files identical despite different names*

### Comparing `ni_measurementlink_service-1.1.0.dev1/ni_measurementlink_service/_internal/stubs/proto/ni/measurementlink/measurement/v1/measurement_service.proto` & `ni_measurementlink_service-1.1.0.dev2/ni_measurementlink_service/_internal/stubs/proto/ni/measurementlink/measurement/v1/measurement_service.proto`

 * *Files identical despite different names*

### Comparing `ni_measurementlink_service-1.1.0.dev1/ni_measurementlink_service/_internal/stubs/proto/ni/measurementlink/measurement/v2/measurement_service.proto` & `ni_measurementlink_service-1.1.0.dev2/ni_measurementlink_service/_internal/stubs/proto/ni/measurementlink/measurement/v2/measurement_service.proto`

 * *Files identical despite different names*

### Comparing `ni_measurementlink_service-1.1.0.dev1/ni_measurementlink_service/_internal/stubs/proto/ni/measurementlink/pin_map_context.proto` & `ni_measurementlink_service-1.1.0.dev2/ni_measurementlink_service/_internal/stubs/proto/ni/measurementlink/pin_map_context.proto`

 * *Files identical despite different names*

### Comparing `ni_measurementlink_service-1.1.0.dev1/ni_measurementlink_service/_internal/stubs/proto/ni/measurementlink/pinmap/v1/pin_map_service.proto` & `ni_measurementlink_service-1.1.0.dev2/ni_measurementlink_service/_internal/stubs/proto/ni/measurementlink/pinmap/v1/pin_map_service.proto`

 * *Files identical despite different names*

### Comparing `ni_measurementlink_service-1.1.0.dev1/ni_measurementlink_service/_internal/stubs/proto/ni/measurementlink/sessionmanagement/v1/session_management_service.proto` & `ni_measurementlink_service-1.1.0.dev2/ni_measurementlink_service/_internal/stubs/proto/ni/measurementlink/sessionmanagement/v1/session_management_service.proto`

 * *Files identical despite different names*

### Comparing `ni_measurementlink_service-1.1.0.dev1/ni_measurementlink_service/_internal/stubs/proto/session.proto` & `ni_measurementlink_service-1.1.0.dev2/ni_measurementlink_service/_internal/stubs/proto/session.proto`

 * *Files identical despite different names*

### Comparing `ni_measurementlink_service-1.1.0.dev1/ni_measurementlink_service/_internal/stubs/session_pb2.py` & `ni_measurementlink_service-1.1.0.dev2/ni_measurementlink_service/_internal/stubs/session_pb2.py`

 * *Files identical despite different names*

### Comparing `ni_measurementlink_service-1.1.0.dev1/ni_measurementlink_service/_internal/stubs/session_pb2.pyi` & `ni_measurementlink_service-1.1.0.dev2/ni_measurementlink_service/_internal/stubs/session_pb2.pyi`

 * *Files identical despite different names*

### Comparing `ni_measurementlink_service-1.1.0.dev1/ni_measurementlink_service/_internal/stubs/session_pb2_grpc.py` & `ni_measurementlink_service-1.1.0.dev2/ni_measurementlink_service/_internal/stubs/session_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `ni_measurementlink_service-1.1.0.dev1/ni_measurementlink_service/measurement/info.py` & `ni_measurementlink_service-1.1.0.dev2/ni_measurementlink_service/measurement/info.py`

 * *Files 12% similar despite different names*

```diff
@@ -33,28 +33,35 @@
 
     Attributes
     ----------
         service_class (str): Service class that the measurement belongs to.
         Measurements under same service class expected to perform same logic.
         For e.g., different version of measurement can come under same service class.
 
+
         description_url (str): Description URL of the measurement.
 
+        provided_interfaces (List[str]): List of interfaces the service provides.
+        For e.g., ni.measurementlink.measurement.v2.MeasurementService.
+        Defaults to ["ni.measurementlink.measurement.v1.MeasurementService"].
+
     """
 
     service_class: str
     description_url: str
+    provided_interfaces: typing.List[str] = ["ni.measurementlink.measurement.v1.MeasurementService"]
 
 
 class TypeSpecialization(enum.Enum):
     """Enum that represents the type specializations for measurement parameters."""
 
     NoType = ""
     Pin = "pin"
     Path = "path"
+    Enum = "enum"
 
 
 class DataType(enum.Enum):
     """Enum that represents the supported data types."""
 
     Int32 = (type_pb2.Field.TYPE_INT32, False, TypeSpecialization.NoType)
     Int64 = (type_pb2.Field.TYPE_INT64, False, TypeSpecialization.NoType)
@@ -62,18 +69,20 @@
     UInt64 = (type_pb2.Field.TYPE_UINT64, False, TypeSpecialization.NoType)
     Float = (type_pb2.Field.TYPE_FLOAT, False, TypeSpecialization.NoType)
     Double = (type_pb2.Field.TYPE_DOUBLE, False, TypeSpecialization.NoType)
     Boolean = (type_pb2.Field.TYPE_BOOL, False, TypeSpecialization.NoType)
     String = (type_pb2.Field.TYPE_STRING, False, TypeSpecialization.NoType)
     Pin = (type_pb2.Field.TYPE_STRING, False, TypeSpecialization.Pin)
     Path = (type_pb2.Field.TYPE_STRING, False, TypeSpecialization.Path)
+    Enum = (type_pb2.Field.TYPE_ENUM, False, TypeSpecialization.Enum)
 
     Int32Array1D = (type_pb2.Field.TYPE_INT32, True, TypeSpecialization.NoType)
     Int64Array1D = (type_pb2.Field.TYPE_INT64, True, TypeSpecialization.NoType)
     UInt32Array1D = (type_pb2.Field.TYPE_UINT32, True, TypeSpecialization.NoType)
     UInt64Array1D = (type_pb2.Field.TYPE_UINT64, True, TypeSpecialization.NoType)
     FloatArray1D = (type_pb2.Field.TYPE_FLOAT, True, TypeSpecialization.NoType)
     DoubleArray1D = (type_pb2.Field.TYPE_DOUBLE, True, TypeSpecialization.NoType)
     BooleanArray1D = (type_pb2.Field.TYPE_BOOL, True, TypeSpecialization.NoType)
     StringArray1D = (type_pb2.Field.TYPE_STRING, True, TypeSpecialization.NoType)
     PinArray1D = (type_pb2.Field.TYPE_STRING, True, TypeSpecialization.Pin)
     PathArray1D = (type_pb2.Field.TYPE_STRING, True, TypeSpecialization.Path)
+    EnumArray1D = (type_pb2.Field.TYPE_ENUM, True, TypeSpecialization.Enum)
```

### Comparing `ni_measurementlink_service-1.1.0.dev1/ni_measurementlink_service/measurement/service.py` & `ni_measurementlink_service-1.1.0.dev2/ni_measurementlink_service/measurement/service.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,16 +1,17 @@
 """Framework to host measurement service."""
 
 from __future__ import annotations
 
 import json
+from enum import Enum
 from os import path
 from pathlib import Path
 from threading import Lock
-from typing import Any, Callable, Dict, List, Optional, TypeVar
+from typing import Any, Callable, Dict, List, Optional, Type, TypeVar
 
 import grpc
 
 from ni_measurementlink_service._internal import grpc_servicer
 from ni_measurementlink_service._internal.discovery_client import DiscoveryClient
 from ni_measurementlink_service._internal.parameter import (
     metadata as parameter_metadata,
@@ -18,43 +19,44 @@
 from ni_measurementlink_service._internal.service_manager import GrpcService
 from ni_measurementlink_service.measurement.info import (
     DataType,
     MeasurementInfo,
     ServiceInfo,
     TypeSpecialization,
 )
+from ni_measurementlink_service.session_management import PinMapContext
 
 
 class MeasurementContext:
     """Proxy for the Measurement Service's context-local state."""
 
     @property
-    def grpc_context(self):
+    def grpc_context(self) -> grpc.ServicerContext:
         """Get the context for the RPC."""
         return grpc_servicer.measurement_service_context.get().grpc_context
 
     @property
-    def pin_map_context(self):
+    def pin_map_context(self) -> PinMapContext:
         """Get the pin map context for the RPC."""
         return grpc_servicer.measurement_service_context.get().pin_map_context
 
-    def add_cancel_callback(self, cancel_callback: Callable):
+    def add_cancel_callback(self, cancel_callback: Callable[[], None]) -> None:
         """Add a callback which is invoked when the RPC is canceled."""
         grpc_servicer.measurement_service_context.get().add_cancel_callback(cancel_callback)
 
-    def cancel(self):
+    def cancel(self) -> None:
         """Cancel the RPC."""
         grpc_servicer.measurement_service_context.get().cancel()
 
     @property
-    def time_remaining(self):
+    def time_remaining(self) -> float:
         """Get the time remaining for the RPC."""
         return grpc_servicer.measurement_service_context.get().time_remaining
 
-    def abort(self, code, details):
+    def abort(self, code: grpc.StatusCode, details: str) -> None:
         """Aborts the RPC."""
         grpc_servicer.measurement_service_context.get().abort(code, details)
 
 
 # Eventually, these can be replaced with typing.Self (Python >= 3.11).
 _TGrpcChannelPool = TypeVar("_TGrpcChannelPool", bound="GrpcChannelPool")
 _TMeasurementService = TypeVar("_TMeasurementService", bound="MeasurementService")
@@ -178,14 +180,15 @@
             version=version,
             ui_file_paths=ui_file_paths,
         )
 
         self.service_info = ServiceInfo(
             service_class=service["serviceClass"],
             description_url=service["descriptionUrl"],
+            provided_interfaces=service["providedInterfaces"],
         )
 
         self.configuration_parameter_list: list = []
         self.output_parameter_list: list = []
         self.grpc_service = GrpcService()
         self.context: MeasurementContext = MeasurementContext()
         self.discovery_client: DiscoveryClient = self.grpc_service.discovery_client
@@ -209,15 +212,21 @@
 
         See also: :func:`.configuration`, :func:`.output`
         """
         self.measure_function = measurement_function
         return measurement_function
 
     def configuration(
-        self, display_name: str, type: DataType, default_value: Any, *, instrument_type: str = ""
+        self,
+        display_name: str,
+        type: DataType,
+        default_value: Any,
+        *,
+        instrument_type: str = "",
+        enum_type: Optional[Type[Enum]] = None,
     ) -> Callable:
         """Add a configuration parameter to a measurement function.
 
         This decorator maps the measurement service's configuration parameters
         to Python positional parameters. To add multiple configuration parameters
         to the same measurement function, use this decorator multiple times.
         The order of decorator calls must match the order of positional parameters.
@@ -228,69 +237,82 @@
         ----
             display_name (str): Display name of the configuration.
 
             type (DataType): Data type of the configuration.
 
             default_value (Any): Default value of the configuration.
 
-            instrument_type (str): Optional.
+            instrument_type (Optional[str]):
             Filter pins by instrument type. This is only supported when configuration type
             is DataType.Pin. Pin maps have built in instrument definitions using the
             NI driver based instrument type ids. These can be found as constants
             in `nims.session_management`. For example, for an NI DCPower instrument
             the instrument type is `nims.session_management.INSTRUMENT_TYPE_NI_DCPOWER`.
             For custom instruments the user defined instrument type id is defined in the
             pin map file.
 
+            enum_type (Optional[Type[Enum]]):
+            Defines the enum type associated with this configuration parameter. This is only
+            supported when configuration type is DataType.Enum or DataType.EnumArray1D.
+
         Returns
         -------
             Callable: Callable that takes in Any Python Function
             and returns the same python function.
 
         """
         grpc_field_type, repeated, type_specialization = type.value
-        annotations = self._get_annotations(type_specialization, instrument_type)
+        annotations = self._make_annotations_dict(
+            type_specialization, instrument_type=instrument_type, enum_type=enum_type
+        )
         parameter = parameter_metadata.ParameterMetadata(
             display_name, grpc_field_type, repeated, default_value, annotations
         )
         parameter_metadata.validate_default_value_type(parameter)
         self.configuration_parameter_list.append(parameter)
 
         def _configuration(func):
             return func
 
         return _configuration
 
-    def output(self, display_name: str, type: DataType) -> Callable:
-        """Add a output parameter to a measurement function.
+    def output(
+        self, display_name: str, type: DataType, *, enum_type: Optional[Type[Enum]] = None
+    ) -> Callable:
+        """Add an output parameter to a measurement function.
 
         This decorator maps the measurement service's output parameters to
         the elements of the tuple returned by the measurement function.
         To add multiple output parameters to the same measurement function,
         use this decorator multiple times.
         The order of decorator calls must match the order of elements
-        returned by the measurement fuction.
+        returned by the measurement function.
 
         See also: :func:`.register_measurement`
 
         Args
         ----
             display_name (str): Display name of the output.
 
             type (DataType): Data type of the output.
 
+            enum_type (Optional[Type[Enum]]):
+            Defines the enum type associated with this configuration parameter. This is only
+            supported when configuration type is DataType.Enum or DataType.EnumArray1D.
+
         Returns
         -------
             Callable: Callable that takes in Any Python Function and
             returns the same python function.
 
         """
         grpc_field_type, repeated, type_specialization = type.value
+        annotations = self._make_annotations_dict(type_specialization, enum_type=enum_type)
         parameter = parameter_metadata.ParameterMetadata(
-            display_name, grpc_field_type, repeated, default_value=None, annotations={}
+            display_name, grpc_field_type, repeated, None, annotations
         )
         self.output_parameter_list.append(parameter)
 
         def _output(func):
             return func
 
         return _output
@@ -315,28 +337,45 @@
             self.service_info,
             self.configuration_parameter_list,
             self.output_parameter_list,
             self.measure_function,
         )
         return self
 
-    def _get_annotations(
-        self, type_specialization: TypeSpecialization, instrument_type: str
+    def _make_annotations_dict(
+        self,
+        type_specialization: TypeSpecialization,
+        *,
+        instrument_type: str = "",
+        enum_type: Optional[Type[Enum]] = None,
     ) -> Dict[str, str]:
         annotations: Dict[str, str] = {}
         if type_specialization == TypeSpecialization.NoType:
             return annotations
 
         annotations["ni/type_specialization"] = type_specialization.value
         if type_specialization == TypeSpecialization.Pin:
             if instrument_type != "" or instrument_type is not None:
                 annotations["ni/pin.instrument_type"] = instrument_type
+        if type_specialization == TypeSpecialization.Enum:
+            if enum_type is not None:
+                annotations["ni/enum.values"] = self._enum_to_annotations_value(enum_type)
+            else:
+                raise ValueError("enum_type is required for enum parameters.")
 
         return annotations
 
+    def _enum_to_annotations_value(self, enum_type: Type[Enum]) -> str:
+        if not any(member.value == 0 for member in enum_type):
+            raise ValueError("The enum does not have a value for 0.")
+        enum_values = {}
+        for member in enum_type:
+            enum_values[member.name] = member.value
+        return json.dumps(enum_values)
+
     def close_service(self) -> None:
         """Close the Service after un-registering with discovery service and cleanups."""
         self.grpc_service.stop()
         self.channel_pool.close()
 
     def __enter__(self: _TMeasurementService) -> _TMeasurementService:
         """Enter the runtime context related to the measurement service."""
```

### Comparing `ni_measurementlink_service-1.1.0.dev1/ni_measurementlink_service/session_management.py` & `ni_measurementlink_service-1.1.0.dev2/ni_measurementlink_service/session_management.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,12 +1,25 @@
 """Contains methods related to managing driver sessions."""
+from __future__ import annotations
+
+import abc
+import warnings
 from functools import cached_property
-from typing import Iterable, List, NamedTuple, Optional, TypeVar
+from typing import (
+    Any,
+    Iterable,
+    List,
+    NamedTuple,
+    Optional,
+    Sequence,
+    TypeVar,
+)
 
 import grpc
+from deprecation import DeprecatedWarning
 
 from ni_measurementlink_service._internal.stubs import session_pb2
 from ni_measurementlink_service._internal.stubs.ni.measurementlink import (
     pin_map_context_pb2,
 )
 from ni_measurementlink_service._internal.stubs.ni.measurementlink.sessionmanagement.v1 import (
     session_management_service_pb2,
@@ -36,18 +49,18 @@
 
 
 class PinMapContext(NamedTuple):
     """Container for the pin map and sites.
 
     Attributes
     ----------
-        pin_map_id (str): The resource id of the pin map in the Pin Map service that should be used
-            for the call.
+        pin_map_id: The resource id of the pin map in the Pin Map service that should be used for
+            the call.
 
-        sites (list): List of site numbers being used for the call. If None, use all sites in the
+        sites: List of site numbers being used for the call. If None or empty, use all sites in the
             pin map.
 
     """
 
     pin_map_id: str
     sites: Optional[List[int]]
 
@@ -105,25 +118,75 @@
     resource_name: str
     channel_list: str
     instrument_type_id: str
     session_exists: bool
     channel_mappings: Iterable[ChannelMapping]
 
 
+def _convert_channel_mapping_from_grpc(
+    channel_mapping: session_management_service_pb2.ChannelMapping,
+) -> ChannelMapping:
+    return ChannelMapping(
+        pin_or_relay_name=channel_mapping.pin_or_relay_name,
+        site=channel_mapping.site,
+        channel=channel_mapping.channel,
+    )
+
+
+def _convert_channel_mapping_to_grpc(
+    channel_mapping: ChannelMapping,
+) -> session_management_service_pb2.ChannelMapping:
+    return session_management_service_pb2.ChannelMapping(
+        pin_or_relay_name=channel_mapping.pin_or_relay_name,
+        site=channel_mapping.site,
+        channel=channel_mapping.channel,
+    )
+
+
+def _convert_session_info_from_grpc(
+    session_info: session_management_service_pb2.SessionInformation,
+) -> SessionInformation:
+    return SessionInformation(
+        session_name=session_info.session.name,
+        resource_name=session_info.resource_name,
+        channel_list=session_info.channel_list,
+        instrument_type_id=session_info.instrument_type_id,
+        session_exists=session_info.session_exists,
+        channel_mappings=[
+            _convert_channel_mapping_from_grpc(m) for m in session_info.channel_mappings
+        ],
+    )
+
+
+def _convert_session_info_to_grpc(
+    session_info: SessionInformation,
+) -> session_management_service_pb2.SessionInformation:
+    return session_management_service_pb2.SessionInformation(
+        session=session_pb2.Session(name=session_info.session_name),
+        resource_name=session_info.resource_name,
+        channel_list=session_info.channel_list,
+        instrument_type_id=session_info.instrument_type_id,
+        session_exists=session_info.session_exists,
+        channel_mappings=[
+            _convert_channel_mapping_to_grpc(m) for m in session_info.channel_mappings
+        ],
+    )
+
+
 # Eventually, this can be replaced with typing.Self (Python >= 3.11).
-_TReservation = TypeVar("_TReservation", bound="Reservation")
+_TReservation = TypeVar("_TReservation", bound="BaseReservation")
 
 
-class Reservation(object):
-    """Manage session reservation."""
+class BaseReservation(abc.ABC):
+    """Manages session reservation."""
 
     def __init__(
         self,
-        session_manager: "Client",
-        session_info: Iterable[session_management_service_pb2.SessionInformation],
+        session_manager: Client,
+        session_info: Sequence[session_management_service_pb2.SessionInformation],
     ):
         """Initialize reservation object."""
         self._session_manager = session_manager
         self._session_info = session_info
 
     def __enter__(self: _TReservation) -> _TReservation:
         """Context management protocol. Returns self."""
@@ -134,56 +197,69 @@
         self.unreserve()
         return False
 
     def unreserve(self):
         """Unreserve sessions."""
         self._session_manager._unreserve_sessions(self._session_info)
 
+
+class SingleSessionReservation(BaseReservation):
+    """Manages reservation for a single session."""
+
+    @cached_property
+    def session_info(self) -> SessionInformation:
+        """Single session information object."""
+        assert len(self._session_info) == 1
+        return _convert_session_info_from_grpc(self._session_info[0])
+
+
+class MultiSessionReservation(BaseReservation):
+    """Manages reservation for multiple sessions."""
+
     @cached_property
     def session_info(self) -> List[SessionInformation]:
-        """Return session information."""
-        return [
-            SessionInformation(
-                session_name=info.session.name,
-                resource_name=info.resource_name,
-                channel_list=info.channel_list,
-                instrument_type_id=info.instrument_type_id,
-                session_exists=info.session_exists,
-                channel_mappings=[
-                    ChannelMapping(
-                        pin_or_relay_name=channel_mapping.pin_or_relay_name,
-                        site=channel_mapping.site,
-                        channel=channel_mapping.channel,
-                    )
-                    for channel_mapping in info.channel_mappings
-                ],
-            )
-            for info in self._session_info
-        ]
+        """Multiple session information objects."""
+        return [_convert_session_info_from_grpc(info) for info in self._session_info]
+
+
+def __getattr__(name: str) -> Any:
+    if name == "Reservation":
+        warnings.warn(
+            DeprecatedWarning(
+                name,
+                deprecated_in="1.1.0",
+                removed_in=None,
+                details="Use MultiSessionReservation instead.",
+            ),
+            stacklevel=2,
+        )
+        return MultiSessionReservation
+    else:
+        raise AttributeError(f"module {__name__} has no attribute {name}")
 
 
 class Client(object):
     """Class that manages driver sessions."""
 
     def __init__(self, *, grpc_channel: grpc.Channel):
         """Initialize session manangement client."""
         self._client: session_management_service_pb2_grpc.SessionManagementServiceStub = (
             session_management_service_pb2_grpc.SessionManagementServiceStub(grpc_channel)
         )
 
-    def reserve_sessions(
+    def reserve_session(
         self,
         context: PinMapContext,
         pin_or_relay_names: Optional[Iterable[str]] = None,
         instrument_type_id: Optional[str] = None,
         timeout: Optional[float] = None,
-    ) -> Reservation:
-        """Reserve session(s).
+    ) -> SingleSessionReservation:
+        """Reserve a single session.
 
-        Reserve session(s) for the given pins, sites, and instrument type ID and returns the
+        Reserve the session matching the given pins, sites, and instrument type ID and return the
         information needed to create or access the session.
 
         Args
         ----
             context (PinMapContext): Includes the pin map ID for the pin map in the Pin Map Service,
                 as well as the list of sites for the measurement.
 
@@ -208,18 +284,89 @@
             timeout (float): Timeout in seconds. Allowed values,
                 0 (non-blocking, fails immediately if resources cannot be reserved),
                 -1 or negative (infinite timeout), or
                 any positive numeric value (wait for that number of second).
 
         Returns
         -------
-            Reservation: Context manager that can be used with a with-statement to unreserve the
-            sessions.
+            SingleSessionReservation: Context manager that can be used with a with-statement to
+            unreserve the session.
+
+        """
+        session_info = self._reserve_sessions(
+            context, pin_or_relay_names, instrument_type_id, timeout
+        )
+        if len(session_info) == 0:
+            raise ValueError("No sessions reserved. Expected single session, got 0 sessions.")
+        elif len(session_info) > 1:
+            raise ValueError(
+                "Too many sessions reserved. Expected single session, got "
+                f"{len(session_info)} sessions."
+            )
+        else:
+            return SingleSessionReservation(session_manager=self, session_info=session_info)
+
+    def reserve_sessions(
+        self,
+        context: PinMapContext,
+        pin_or_relay_names: Optional[Iterable[str]] = None,
+        instrument_type_id: Optional[str] = None,
+        timeout: Optional[float] = None,
+    ) -> MultiSessionReservation:
+        """Reserve multiple sessions.
+
+        Reserve sessions matching the given pins, sites, and instrument type ID and return the
+        information needed to create or access the sessions.
+
+        Args
+        ----
+            context (PinMapContext): Includes the pin map ID for the pin map in the Pin Map Service,
+                as well as the list of sites for the measurement.
+
+            pin_or_relay_names (Iterable[str]): List of pins, pin groups, relays, or relay groups to
+                use for the measurement. If unspecified, reserve sessions for all pins and relays in
+                the registered pin map resource.
+
+            instrument_type_id (str): Instrument type ID for the measurement. If unspecified,
+                reserve sessions for all instrument types connected in the registered pin map
+                resource. Pin maps have built in instrument definitions using the following NI
+                driver based instrument type ids:
+                    "niDCPower"
+                    "niDigitalPattern"
+                    "niScope"
+                    "niDMM"
+                    "niDAQmx"
+                    "niFGen"
+                    "niRelayDriver"
+                For custom instruments the user defined instrument type id is defined in the pin
+                map file.
+
+            timeout (float): Timeout in seconds. Allowed values,
+                0 (non-blocking, fails immediately if resources cannot be reserved),
+                -1 or negative (infinite timeout), or
+                any positive numeric value (wait for that number of second).
+
+        Returns
+        -------
+            MultiSessionReservation: Context manager that can be used with a with-statement to
+            unreserve the sessions.
 
         """
+        session_info = self._reserve_sessions(
+            context, pin_or_relay_names, instrument_type_id, timeout
+        )
+        return MultiSessionReservation(session_manager=self, session_info=session_info)
+
+    def _reserve_sessions(
+        self,
+        context: PinMapContext,
+        pin_or_relay_names: Optional[Iterable[str]] = None,
+        instrument_type_id: Optional[str] = None,
+        timeout: Optional[float] = None,
+    ) -> Sequence[session_management_service_pb2.SessionInformation]:
         pin_map_context = pin_map_context_pb2.PinMapContext(
             pin_map_id=context.pin_map_id, sites=context.sites
         )
 
         request = session_management_service_pb2.ReserveSessionsRequest(
             pin_map_context=pin_map_context
         )
@@ -233,18 +380,15 @@
                 timeout_in_ms = -1
             request.timeout_in_milliseconds = timeout_in_ms
 
         response: session_management_service_pb2.ReserveSessionsResponse = (
             self._client.ReserveSessions(request)
         )
 
-        return Reservation(
-            session_manager=self,
-            session_info=response.sessions,
-        )
+        return response.sessions
 
     def _unreserve_sessions(
         self, session_info: Iterable[session_management_service_pb2.SessionInformation]
     ):
         """Unreserves sessions so they can be accessed by other clients."""
         request = session_management_service_pb2.UnreserveSessionsRequest(sessions=session_info)
         self._client.UnreserveSessions(request)
@@ -316,15 +460,15 @@
                 for info in session_info
             )
         )
         self._client.UnregisterSessions(request)
 
     def reserve_all_registered_sessions(
         self, instrument_type_id: Optional[str] = None, timeout: Optional[float] = None
-    ) -> Reservation:
+    ) -> MultiSessionReservation:
         """Reserves and gets all sessions currently registered in the Session Manager.
 
         Args
         ----
             instrument_type_id (str): Instrument type ID for the measurement. If unspecified,
                 reserve sessions for all instrument types connected in the registered pin map
                 resource. Pin maps have built in instrument definitions using the following NI
@@ -342,24 +486,24 @@
             timeout (float): Timeout in seconds. Allowed values,
                 0 (non-blocking, fails immediately if resources cannot be reserved),
                 -1 or negative (infinite timeout), or
                 any positive numeric value (wait for that number of second).
 
         Returns
         -------
-            Reservation: Context manager that can be used with a with-statement to unreserve the
-            sessions.
+            MultiSessionReservation: Context manager that can be used with a with-statement to
+            unreserve the sessions.
 
         """
         request = session_management_service_pb2.ReserveAllRegisteredSessionsRequest()
         if instrument_type_id is not None:
             request.instrument_type_id = instrument_type_id
         if timeout is not None:
             timeout_in_ms = round(timeout * 1000)
             if timeout_in_ms < 0:
                 timeout_in_ms = -1
             request.timeout_in_milliseconds = timeout_in_ms
 
         response: session_management_service_pb2.ReserveAllRegisteredSessionsResponse = (
             self._client.ReserveAllRegisteredSessions(request)
         )
-        return Reservation(session_manager=self, session_info=response.sessions)
+        return MultiSessionReservation(session_manager=self, session_info=response.sessions)
```

### Comparing `ni_measurementlink_service-1.1.0.dev1/pyproject.toml` & `ni_measurementlink_service-1.1.0.dev2/pyproject.toml`

 * *Files 9% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 | \.venv
 | venv
 )
 '''
 
 [tool.poetry]
 name = "ni_measurementlink_service"
-version = "1.1.0-dev1"
+version = "1.1.0-dev2"
 description = "MeasurementLink Support for Python"
 authors = ["NI <opensource@ni.com>"]
 readme = "README.md" # apply the repo readme to the package as well
 repository = "https://github.com/ni/measurementlink-python/"
 license = "MIT"
 classifiers = [
     "Development Status :: 5 - Production/Stable",
@@ -33,27 +33,30 @@
 python = "^3.8"
 # This package includes gRPC stubs that were generated with the version of grpcio-tools specified
 # below. Please keep the minimum grpcio version in sync with the grpcio-tools version. Otherwise,
 # the generated gRPC stubs may not work with the minimum grpcio version.
 grpcio = "^1.49.1"
 protobuf = "^4.21"
 pywin32 = {version = ">=303", platform = "win32"}
+deprecation = ">=2.1"
 
 [tool.poetry.group.dev.dependencies]
 pytest = ">=7.2.0"
 ni-python-styleguide = ">=0.4.1"
 # When you update the grpcio-tools version, you should update the minimum grpcio version
 # and regenerate gRPC stubs.
 grpcio-tools = "1.49.1"
 pytest-cov = ">=3.0.0"
+pytest-mock = ">=3.0"
 mypy = ">=1.0"
 mypy-protobuf = ">=3.4"
 types-protobuf = "^4.21"
 types-pkg-resources = "*"
 types-pywin32 = {version = ">=304", platform = "win32"}
+grpc-stubs = "^1.53"
 
 [tool.poetry.group.docs]
 optional = true
 
 [tool.poetry.group.docs.dependencies]
 Sphinx = "^5.0.1"
 sphinx-rtd-theme = "^1.0.0"
@@ -72,17 +75,20 @@
 
 [tool.pytest.ini_options]
 addopts = "--doctest-modules --strict-markers"
 filterwarnings = ["always::ImportWarning", "always::ResourceWarning"]
 testpaths = ["tests"]
 
 [tool.mypy]
-exclude = ["stubs"]
 warn_unused_configs = true
 namespace_packages = true
 check_untyped_defs = true
 warn_redundant_casts = true
 warn_unused_ignores = true
 
 [[tool.mypy.overrides]]
-module = "grpc.*"
+module = [
+  # https://github.com/briancurtin/deprecation/issues/56 - Add type information (PEP 561)
+  "deprecation.*",
+  "grpc.framework.foundation.*"
+]
 ignore_missing_imports = true
```

### Comparing `ni_measurementlink_service-1.1.0.dev1/setup.py` & `ni_measurementlink_service-1.1.0.dev2/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -27,24 +27,24 @@
                                                 'proto/ni/measurementlink/discovery/v1/*',
                                                 'proto/ni/measurementlink/measurement/v1/*',
                                                 'proto/ni/measurementlink/measurement/v2/*',
                                                 'proto/ni/measurementlink/pinmap/v1/*',
                                                 'proto/ni/measurementlink/sessionmanagement/v1/*']}
 
 install_requires = \
-['grpcio>=1.49.1,<2.0.0', 'protobuf>=4.21,<5.0']
+['deprecation>=2.1', 'grpcio>=1.49.1,<2.0.0', 'protobuf>=4.21,<5.0']
 
 extras_require = \
 {':sys_platform == "win32"': ['pywin32>=303']}
 
 setup_kwargs = {
     'name': 'ni-measurementlink-service',
-    'version': '1.1.0.dev1',
+    'version': '1.1.0.dev2',
     'description': 'MeasurementLink Support for Python',
-    'long_description': '# MeasurementLink™ Support for Python\n\n- [MeasurementLink™ Support for Python](#measurementlink--support-for-python)\n  - [Introduction](#introduction)\n  - [Dependencies](#dependencies)\n  - [Documentation](#documentation)\n  - [Examples](#examples)\n  - [Developing Measurements: Quick Start](#developing-measurements-quick-start)\n    - [Installation](#installation)\n    - [Developing a minimal python measurement](#developing-a-minimal-python-measurement)\n  - [Steps to run/debug the measurement service](#steps-to-rundebug-the-measurement-service)\n  - [Static Registration of Python Measurements](#static-registration-of-python-measurements)\n    - [Create a batch file that runs a python measurement](#create-a-batch-file-that-runs-a-python-measurement)\n    - [Create Executable for Python Scripts](#create-executable-for-python-scripts)\n  - [Appendix: Managing Measurement as Python Package (Project)](#appendix-managing-measurement-as-python-package-project)\n    - [Create and Manage Python Measurement Package using Poetry](#create-and-manage-python-measurement-package-using-poetry)\n    - [Create and Manage Python Measurement Package using `venv`](#create-and-manage-python-measurement-package-using-venv)\n    - [Create and Manage Python Measurement Package by directly installing `ni-measurementlink-service` as a system-level package](#create-and-manage-python-measurement-package-by-directly-installing-ni-measurementlink-service-as-a-system-level-package)\n\n---\n\n## Introduction\n\nMeasurementLink Support for Python (`ni-measurementlink-service`) is a Python framework that enables measurement developers to quickly create Python measurements and run them as a service (gRPC).\n\n---\n\n## Dependencies\n\n- Python >= 3.8 [(3.9 recommended)](https://www.python.org/downloads/release/python-3913/)\n- [grpcio >= 1.49.1, < 2.x](https://pypi.org/project/grpcio/1.49.1/)\n- [protobuf >= 4.21, < 5.x](https://pypi.org/project/protobuf/4.21.0/)\n- [pywin32 >= 303 (Only for Windows)](https://pypi.org/project/pywin32/303/)\n\n---\n\n## Documentation\n\n- [MeasurementLink Manual](https://www.ni.com/docs/en-US/bundle/measurementlink)\n- [API Reference](https://ni.github.io/measurementlink-python/)\n\n---\n\n## System Configuration\n\n### Enable Win32 Long Paths\n\nBy default, Windows has a path length limit of 260 characters. NI recommends enabling support for long paths when developing and deploying Python measurement services. \n\nThere are three ways to do this:\n- When installing Python using the Python for Windows installer, click `Disable path length limit` at the end of the installation.\n- Set the `Enable Win32 long paths` group policy:\n  - Run `gpedit.msc`.\n  - Expand `Computer Configuration` » `Administrative Templates` » `All Settings`.\n  - Find `Enable Win32 long paths` in the list, double-click it, and set it to `Enabled`.\n- In the Windows registry, set `HKEY_LOCAL_MACHINE\\SYSTEM\\CurrentControlSet\\Control\\FileSystem\\LongPathsEnabled` (type: `REG_DWORD`) to 1. For more details, see [Maximum Path Length Limitation](https://learn.microsoft.com/en-us/windows/win32/fileio/maximum-file-path-limitation).\n\n---\n\n## Examples\n\nThe `examples` directory contains example measurements for MeasurementLink 2023 Q3 or later. If\nyou are using a previous version of MeasurementLink, download the appropriate examples:\n\n- MeasurementLink 2023 Q1: [measurementlink-python-examples-1.0.1.zip](https://github.com/ni/measurementlink-python/releases/download/1.0.1/measurementlink-python-examples-1.0.1.zip)\n- MeasurementLink 2023 Q2: [measurementlink-python-examples-1.0.1.zip](https://github.com/ni/measurementlink-python/releases/download/1.0.1/measurementlink-python-examples-1.0.1.zip)\n\nFor more information on setting up and running the example measurements, see the included `README.md` file.\n\nFor best results, use the example measurements corresponding to the version of MeasurementLink\nthat you are using. Newer examples may demonstrate features that are not available in older\nversions of MeasurementLink.\n\n---\n\n## Developing Measurements: Quick Start\n\nThis section provides instructions to develop custom measurement services in Python using MeasurementLink Support for Python.\n\n### Installation\n\nMake sure the system has the recommended Python version is installed. Install MeasurementLink Support for Python using [pip](https://pip.pypa.io/).\n\n``` cmd\nREM Activate the required virtual environment if any.\npip install ni-measurementlink-service\n```\n\nCheck if you have installed the expected version of MeasurementLink Support for Python installed by running the below command:\n\n```cmd\npip show ni-measurementlink-service\n```\n\n### Developing a minimal Python measurement\n\n1. Install the `ni-measurementlink-generator` package.\n\n``` cmd\nREM Activate the required virtual environment if any.\npip install ni-measurementlink-generator\n```\n\n2. Run the `ni-measurementlink-generator` tool. Use command line arguments to specify the `display-name` and optionally the `version`, `measurement-type`, and `product-type`.\n\n    1. Running `ni-measurementlink-generator` without optional arguments:\n\n    `ni-measurementlink-generator SampleMeasurement`\n\n    \'SampleMeasurement\' is the display name of your measurement service. Without the optional arguments,\n    the other arguments are generated for you based on the display name.\n\n    2. Running `ni-measurementlink-generator` with optional arguments for `measurement-version`, `ui-file`,\n    `service-class`, and `description-url`:\n\n    `ni-measurementlink-generator SampleMeasurement --measurement-version 0.1.0.0 --ui-file MeasurementUI.measui --service-class SampleMeasurement_Python --description-url https://www.example.com/SampleMeasurement.html`\n\n    3. Running `ni-measurementlink-generator` with optional argument for `directory-out`\n\n    `ni-measurementlink-generator SampleMeasurement --directory-out <new_path_for_created_files>`\n\n    If no output directory is specified, the files will\n    be placed in a new folder under the current directory\n    named after the display name without spaces.\n\n3. To customize the created measurement, provide metadata of the measurement\'s configuration (input parameters) and outputs (output parameters) in `measurement.py`.\n    1. Use the `configuration()` decorator to provide metadata about the configurations.**The order of the configuration decorator must match with the order of the parameters defined in the function signature.**\n\n        ``` python\n        @foo_measurement_service.register_measurement\n        #Display Names can not contains backslash or front slash.\n        @foo_measurement_service.configuration("DisplayNameForInput1", DataType.String, "DefaultValueForInput1")\n        @foo_measurement_service.configuration("DisplayNameForInput2", DataType.String, "DefaultValueForInput2")\n        def measure(input_1, input_2):\n            \'\'\' A simple Measurement method\'\'\'\n            return ["foo", "bar"]\n        ```\n\n    2. Use the `output()` decorator to provide metadata about the output.**The order of the output decorators from top to bottom must match the order of the values of the list returned by the function.**\n\n        ``` python\n        @foo_measurement_service.register_measurement\n        @foo_measurement_service.configuration("DisplayNameForInput1", nims.DataType.String, "DefaultValueForInput1")\n        @foo_measurement_service.configuration("DisplayNameForInput2", nims.DataType.String, "DefaultValueForInput2")\n        @foo_measurement_service.output("DisplayNameForOutput1", nims.DataType.String)\n        @foo_measurement_service.output("DisplayNameForOutput2", nims.DataType.String)\n        def measure(input_1, input_2):\n            return ["foo", "bar"]\n        ```\n\n4. Run/Debug the created measurement by following the steps discussed in the section ["Steps to run/debug the measurement service".](#steps-to-rundebug-the-measurement-service)\n\n---\n\n## Steps to run/debug the measurement service\n\n1. Start the discovery service if not already started.\n\n2. (Optional) Activate related virtual environments. Measurement developers can skip this step if they are not using any [virtual environments](#create-and-manage-python-measurement-package-using-venv) or [poetry-based projects.](#create-and-manage-python-measurement-package-using-poetry)\n\n    ```cmd\n    .venv\\scripts\\activate\n    ```\n\n    - After successful activation, you can see the name of the environment, `(.venv)` is added to the command prompt.\n    - If you face an access issue when trying to activate, retry after allowing scripts to run as Administrator by executing the below command in Windows PowerShell:\n\n        ```cmd\n        Set-ExecutionPolicy RemoteSigned \n        ```\n\n3. [Run](https://code.visualstudio.com/docs/python/python-tutorial#_run-hello-world)/[Debug](https://code.visualstudio.com/docs/python/debugging#_basic-debugging) the measurement Python file.\n\n4. To stop the running measurement service, press `Enter` in the terminal to properly close the service.\n\n5. (Optional) After the usage of measurement, deactivate the virtual environment. Measurement developers can skip this step if they are not using any [virtual environments](#create-and-manage-python-measurement-package-using-venv) or [poetry-based projects.](#create-and-manage-python-measurement-package-using-poetry)\n\n    ```cmd\n    deactivate\n    ```\n\n---\n\n## Static Registration of Python Measurements\n\nThe MeasurementLink discovery service provides a registry of other services, and can discover and activate other services on the system. These features allow the discovery service to distinguish, manage, and describe measurement services on the system.\n\nTo statically register a measurement service with the MeasurementLink discovery service, do the following:\n\n1. Create a [startup batch file](#create-a-batch-file-that-runs-a-python-measurement) or [executable](#create-executable-for-python-scripts) for the measurement service.\n\n2. Edit the measurement service\'s `.serviceconfig` file and set the `path` value to the filename of the startup batch file or executable.\n\n3. Copy the measurement service\'s directory (including the `.venv` subdirectory if present, `.serviceconfig` file, and startup batch file) to a subdirectory of `C:\\ProgramData\\National Instruments\\MeasurementLink\\Services`. \n\nOnce your measurement service is statically registered, the MeasurementLink discovery service makes it visible in supported NI applications.\n\n### Create a batch file that runs a Python measurement\n\nThe batch file used for static registration is responsible for starting the Python Scripts.\n\nTypical Batch File:\n\n``` cmd\n"<path_to_python_exe>" "<path_to_measurement_file>"\n```\n\nExamples to start the fictitious file named `foo_measurement.py`:\n\n1. Using the Python system distribution\n\n    ```cmd\n    python foo_measurement.py\n    ```\n\n2. Using the virtual environment\n\n    ```cmd\n    REM Windows\n    .\\.venv\\Scripts\\python.exe foo_measurement.py\n\n    REM Linux \n    .venv/bin/python foo_measurement.py\n    ```\n\n### Create Executable for Python Scripts\n\nTo create an executable from a measurement, measurement authors can use the [pyinstaller](https://www.pyinstaller.org/) tooling. During the executable creation, the user can also embed the User Interface file using the `--add-data "<path_of_the_UI_File>;."`.\n\nTypical Pyinstaller command to build executable.\n\n```cmd\npyinstaller --onefile --console --add-data "<path_of_the_UI_File>;." --paths .venv\\Lib\\site-packages\\ <path_of_the_measurement_script>\n```\n\n## Troubleshooting\n\n### "File not found" or "No such file or directory" errors when copying or running a measurement service\n\nIf copying or running a measurement service produces "File not found" or "No such file or directory" errors, make sure to [enable Win32 long paths](#enable-win32-long-paths). If you are unable to enable Win32 long paths, consider deploying the measurement service to a directory with a shorter path.\n\n## Appendix: Managing Measurement as Python Package (Project)\n\nMeasurement and its related files can be maintained as a Python package. The basic components of any Python measurement package are:\n\n1. Measurement Python module (`.py` file)\n    - This file contains all the details related to the measurement and also contains the logic for the measurement execution.\n    - This file is run to start the measurement as a service.\n\n2. UI File\n    - UI file for the measurement. Types of supported UI files are:\n        - Measurement UI (`.measui`): created using the **MeasurementLink UI Editor** application.\n        - LabVIEW UI (`.vi`)\n    - The path of this file is configured by `ui_file_path` in `measurement_info` variable definition in measurement Python module (`.py`).\n\nPython communities have different ways of managing Python packages and their dependencies. It is up to the measurement developer to decide how to maintain the package and dependencies. Measurement developers can choose from a few common approaches discussed below based on their requirements.\n\n### Create and Manage Python Measurement Package using Poetry\n\n1. Install `poetry` (one-time setup)\n\n    1. Make sure the system has the recommended Python version installed.\n\n    2. Install `poetry` using the installation steps given in <https://python-poetry.org/docs/#installation>.\n\n2. Create a new Python project and add `ni-measurementlink-service` as a dependency to the project.\n\n    1. Open a command prompt, and change the working directory to the directory of your choice where you want to create the project.\n\n        ``` cmd\n        cd <path_of_directory_of_your_choice>\n        ```\n\n    2. Create a Python package (project) using the `poetry new` command. Poetry will create boilerplate files and folders that are commonly needed for a Python project.\n\n        ``` cmd\n        poetry new <name_of_the_project>\n        ```\n\n    3. Add the `ni-measurementlink-service` package as a dependency using the [`poetry add`](https://python-poetry.org/docs/cli/#add) command.\n\n        ``` cmd\n        cd <name_of_the_project>\n        poetry add ni-measurementlink-service\n        ```\n\n    4. The virtual environment will be auto-created by poetry.\n\n    5. Create measurement modules as described in ["Developing a minimal Python measurement"](#developing-a-minimal-python-measurement)\n        - Any additional dependencies required by measurement can be added using [add command](https://python-poetry.org/docs/cli/#add).\n\n            ``` cmd\n            poetry add <dependency_package_name>\n            ```\n\nFor detailed info on managing projects using poetry [refer to the official documentation](https://python-poetry.org/docs/cli/).\n\n### Create and Manage Python Measurement Package using `venv`\n\n1. Make sure the system has the recommended Python version installed.\n\n2. Open a command prompt, and change the working directory to the directory of your choice where you want to create a project.\n\n    ``` cmd\n    cd <path_of_directory_of_your_choice>\n    ```\n\n3. Create a virtual environment.\n\n    ``` cmd\n    REM This creates a virtual environment named .venv\n    python -m venv .venv\n    ```\n\n4. Activate the virtual environment. After successful activation\n\n    ``` cmd\n    .venv\\scripts\\activate\n    REM Optionally upgrade the pip within the venv by executing the command\n    python -m pip install -U pip\n    ```\n\n5. Install the `ni-measurementlink-service` package into the virtual environment.\n\n    ``` cmd\n    pip install ni-measurementlink-service\n    ```\n\n6. Create measurement modules as described in ["Developing a minimal Python measurement"](#developing-a-minimal-python-measurement)\n    - Any additional dependencies required by measurement can be added pip install.\n\n        ``` cmd\n        pip install <dependency_package_name>\n        ```\n\nFor detailed info on managing projects with a virtual environment, refer to the [official documentation](https://docs.python.org/3/tutorial/venv.html).\n\n### Create and Manage Python Measurement Package by directly installing `ni-measurementlink-service` as a system-level package\n\nMeasurement developers can also install `ni-measurementlink-service` as a system package if necessary.\n\n1. Install the `ni-measurementlink-service` package from the command prompt\n\n    ``` cmd\n    pip install ni-measurementlink-service\n    ```\n\n2. Create measurement modules as described in ["Developing a minimal Python measurement"](#developing-a-minimal-python-measurement)\n\n---\n',
+    'long_description': '# MeasurementLink™ Support for Python\n\n- [MeasurementLink™ Support for Python](#measurementlink--support-for-python)\n  - [Introduction](#introduction)\n  - [Dependencies](#dependencies)\n  - [Documentation](#documentation)\n  - [Examples](#examples)\n  - [Developing Measurements: Quick Start](#developing-measurements-quick-start)\n    - [Installation](#installation)\n    - [Developing a minimal python measurement](#developing-a-minimal-python-measurement)\n  - [Steps to run/debug the measurement service](#steps-to-rundebug-the-measurement-service)\n  - [Static Registration of Python Measurements](#static-registration-of-python-measurements)\n    - [Create a batch file that runs a python measurement](#create-a-batch-file-that-runs-a-python-measurement)\n    - [Create Executable for Python Scripts](#create-executable-for-python-scripts)\n  - [Appendix: Managing Measurement as Python Package (Project)](#appendix-managing-measurement-as-python-package-project)\n    - [Create and Manage Python Measurement Package using Poetry](#create-and-manage-python-measurement-package-using-poetry)\n    - [Create and Manage Python Measurement Package using `venv`](#create-and-manage-python-measurement-package-using-venv)\n    - [Create and Manage Python Measurement Package by directly installing `ni-measurementlink-service` as a system-level package](#create-and-manage-python-measurement-package-by-directly-installing-ni-measurementlink-service-as-a-system-level-package)\n\n---\n\n## Introduction\n\nMeasurementLink Support for Python (`ni-measurementlink-service`) is a Python framework that enables measurement developers to quickly create Python measurements and run them as a service (gRPC).\n\n---\n\n## Dependencies\n\n- Python >= 3.8 [(3.9 recommended)](https://www.python.org/downloads/release/python-3913/)\n- [grpcio >= 1.49.1, < 2.x](https://pypi.org/project/grpcio/1.49.1/)\n- [protobuf >= 4.21, < 5.x](https://pypi.org/project/protobuf/4.21.0/)\n- [pywin32 >= 303 (Only for Windows)](https://pypi.org/project/pywin32/303/)\n\n---\n\n## Documentation\n\n- [MeasurementLink Manual](https://www.ni.com/docs/en-US/bundle/measurementlink)\n- [API Reference](https://ni.github.io/measurementlink-python/)\n\n---\n\n## System Configuration\n\n### Enable Win32 Long Paths\n\nBy default, Windows has a path length limit of 260 characters. NI recommends enabling support for long paths when developing and deploying Python measurement services. \n\nThere are three ways to do this:\n- When installing Python using the Python for Windows installer, click `Disable path length limit` at the end of the installation.\n- Set the `Enable Win32 long paths` group policy:\n  - Run `gpedit.msc`.\n  - Expand `Computer Configuration` » `Administrative Templates` » `All Settings`.\n  - Find `Enable Win32 long paths` in the list, double-click it, and set it to `Enabled`.\n- In the Windows registry, set `HKEY_LOCAL_MACHINE\\SYSTEM\\CurrentControlSet\\Control\\FileSystem\\LongPathsEnabled` (type: `REG_DWORD`) to 1. For more details, see [Maximum Path Length Limitation](https://learn.microsoft.com/en-us/windows/win32/fileio/maximum-file-path-limitation).\n\n---\n\n## Examples\n\nThe `examples` directory contains example measurements for MeasurementLink 2023 Q3 or later. If\nyou are using a previous version of MeasurementLink, download the appropriate examples:\n\n- MeasurementLink 2023 Q1: [measurementlink-python-examples-1.0.1.zip](https://github.com/ni/measurementlink-python/releases/download/1.0.1/measurementlink-python-examples-1.0.1.zip)\n- MeasurementLink 2023 Q2: [measurementlink-python-examples-1.0.1.zip](https://github.com/ni/measurementlink-python/releases/download/1.0.1/measurementlink-python-examples-1.0.1.zip)\n- MeasurementLink 2023 Q3: [measurementlink-python-examples-1.1.0.zip](https://github.com/ni/measurementlink-python/releases/download/1.1.0/measurementlink-python-examples-1.1.0.zip)\n\nFor more information on setting up and running the example measurements, see the included `README.md` file.\n\nFor best results, use the example measurements corresponding to the version of MeasurementLink\nthat you are using. Newer examples may demonstrate features that are not available in older\nversions of MeasurementLink.\n\n---\n\n## Developing Measurements: Quick Start\n\nThis section provides instructions to develop custom measurement services in Python using MeasurementLink Support for Python.\n\n### Installation\n\nMake sure the system has the recommended Python version is installed. Install MeasurementLink Support for Python using [pip](https://pip.pypa.io/).\n\n``` cmd\nREM Activate the required virtual environment if any.\npip install ni-measurementlink-service\n```\n\nCheck if you have installed the expected version of MeasurementLink Support for Python installed by running the below command:\n\n```cmd\npip show ni-measurementlink-service\n```\n\n### Developing a minimal Python measurement\n\n1. Install the `ni-measurementlink-generator` package.\n\n``` cmd\nREM Activate the required virtual environment if any.\npip install ni-measurementlink-generator\n```\n\n2. Run the `ni-measurementlink-generator` tool. Use command line arguments to specify the `display-name` and optionally the `version`, `measurement-type`, and `product-type`.\n\n    1. Running `ni-measurementlink-generator` without optional arguments:\n\n    `ni-measurementlink-generator SampleMeasurement`\n\n    \'SampleMeasurement\' is the display name of your measurement service. Without the optional arguments,\n    the other arguments are generated for you based on the display name.\n\n    2. Running `ni-measurementlink-generator` with optional arguments for `measurement-version`, `ui-file`,\n    `service-class`, and `description-url`:\n\n    `ni-measurementlink-generator SampleMeasurement --measurement-version 0.1.0.0 --ui-file MeasurementUI.measui --service-class SampleMeasurement_Python --description-url https://www.example.com/SampleMeasurement.html`\n\n    3. Running `ni-measurementlink-generator` with optional argument for `directory-out`\n\n    `ni-measurementlink-generator SampleMeasurement --directory-out <new_path_for_created_files>`\n\n    If no output directory is specified, the files will\n    be placed in a new folder under the current directory\n    named after the display name without spaces.\n\n3. To customize the created measurement, provide metadata of the measurement\'s configuration (input parameters) and outputs (output parameters) in `measurement.py`.\n    1. Use the `configuration()` decorator to provide metadata about the configurations.**The order of the configuration decorator must match with the order of the parameters defined in the function signature.**\n\n        ``` python\n        @foo_measurement_service.register_measurement\n        #Display Names can not contains backslash or front slash.\n        @foo_measurement_service.configuration("DisplayNameForInput1", DataType.String, "DefaultValueForInput1")\n        @foo_measurement_service.configuration("DisplayNameForInput2", DataType.String, "DefaultValueForInput2")\n        def measure(input_1, input_2):\n            \'\'\' A simple Measurement method\'\'\'\n            return ["foo", "bar"]\n        ```\n\n    2. Use the `output()` decorator to provide metadata about the output.**The order of the output decorators from top to bottom must match the order of the values of the list returned by the function.**\n\n        ``` python\n        @foo_measurement_service.register_measurement\n        @foo_measurement_service.configuration("DisplayNameForInput1", nims.DataType.String, "DefaultValueForInput1")\n        @foo_measurement_service.configuration("DisplayNameForInput2", nims.DataType.String, "DefaultValueForInput2")\n        @foo_measurement_service.output("DisplayNameForOutput1", nims.DataType.String)\n        @foo_measurement_service.output("DisplayNameForOutput2", nims.DataType.String)\n        def measure(input_1, input_2):\n            return ["foo", "bar"]\n        ```\n\n4. Run/Debug the created measurement by following the steps discussed in the section ["Steps to run/debug the measurement service".](#steps-to-rundebug-the-measurement-service)\n\n---\n\n## Steps to run/debug the measurement service\n\n1. Start the discovery service if not already started.\n\n2. (Optional) Activate related virtual environments. Measurement developers can skip this step if they are not using any [virtual environments](#create-and-manage-python-measurement-package-using-venv) or [poetry-based projects.](#create-and-manage-python-measurement-package-using-poetry)\n\n    ```cmd\n    .venv\\scripts\\activate\n    ```\n\n    - After successful activation, you can see the name of the environment, `(.venv)` is added to the command prompt.\n    - If you face an access issue when trying to activate, retry after allowing scripts to run as Administrator by executing the below command in Windows PowerShell:\n\n        ```cmd\n        Set-ExecutionPolicy RemoteSigned \n        ```\n\n3. [Run](https://code.visualstudio.com/docs/python/python-tutorial#_run-hello-world)/[Debug](https://code.visualstudio.com/docs/python/debugging#_basic-debugging) the measurement Python file.\n\n4. To stop the running measurement service, press `Enter` in the terminal to properly close the service.\n\n5. (Optional) After the usage of measurement, deactivate the virtual environment. Measurement developers can skip this step if they are not using any [virtual environments](#create-and-manage-python-measurement-package-using-venv) or [poetry-based projects.](#create-and-manage-python-measurement-package-using-poetry)\n\n    ```cmd\n    deactivate\n    ```\n\n---\n\n## Static Registration of Python Measurements\n\nThe MeasurementLink discovery service provides a registry of other services, and can discover and activate other services on the system. These features allow the discovery service to distinguish, manage, and describe measurement services on the system.\n\nTo statically register a measurement service with the MeasurementLink discovery service, do the following:\n\n1. Create a [startup batch file](#create-a-batch-file-that-runs-a-python-measurement) or [executable](#create-executable-for-python-scripts) for the measurement service.\n\n2. Edit the measurement service\'s `.serviceconfig` file and set the `path` value to the filename of the startup batch file or executable.\n\n3. Copy the measurement service\'s directory (including the `.serviceconfig` file and startup batch file) to a subdirectory of `C:\\ProgramData\\National Instruments\\MeasurementLink\\Services`.\n> **Note**\n> If you are using a virtual environment, do not copy the `.venv` subdirectory&mdash;the virtual environment must be re-created in the new location.\n\nOnce your measurement service is statically registered, the MeasurementLink discovery service makes it visible in supported NI applications.\n\n### Create a batch file that runs a Python measurement\n\nThe batch file used for static registration is responsible for starting the Python Scripts.\n\nTypical Batch File:\n\n``` cmd\n"<path_to_python_exe>" "<path_to_measurement_file>"\n```\n\nExamples to start the fictitious file named `foo_measurement.py`:\n\n1. Using the Python system distribution\n\n    ```cmd\n    python foo_measurement.py\n    ```\n\n2. Using the virtual environment\n\n    ```cmd\n    REM Windows\n    .\\.venv\\Scripts\\python.exe foo_measurement.py\n\n    REM Linux \n    .venv/bin/python foo_measurement.py\n    ```\n\n### Create Executable for Python Scripts\n\nTo create an executable from a measurement, measurement authors can use the [pyinstaller](https://www.pyinstaller.org/) tooling. During the executable creation, the user can also embed the User Interface file using the `--add-data "<path_of_the_UI_File>;."`.\n\nTypical Pyinstaller command to build executable.\n\n```cmd\npyinstaller --onefile --console --add-data "<path_of_the_UI_File>;." --paths .venv\\Lib\\site-packages\\ <path_of_the_measurement_script>\n```\n\n## Troubleshooting\n\n### "File not found" or "No such file or directory" errors when copying or running a measurement service\n\nIf copying or running a measurement service produces "File not found" or "No such file or directory" errors, make sure to [enable Win32 long paths](#enable-win32-long-paths). If you are unable to enable Win32 long paths, consider deploying the measurement service to a directory with a shorter path.\n\n## Appendix: Managing Measurement as Python Package (Project)\n\nMeasurement and its related files can be maintained as a Python package. The basic components of any Python measurement package are:\n\n1. Measurement Python module (`.py` file)\n    - This file contains all the details related to the measurement and also contains the logic for the measurement execution.\n    - This file is run to start the measurement as a service.\n\n2. UI File\n    - UI file for the measurement. Types of supported UI files are:\n        - Measurement UI (`.measui`): created using the **MeasurementLink UI Editor** application.\n        - LabVIEW UI (`.vi`)\n    - The path of this file is configured by `ui_file_path` in `measurement_info` variable definition in measurement Python module (`.py`).\n\nPython communities have different ways of managing Python packages and their dependencies. It is up to the measurement developer to decide how to maintain the package and dependencies. Measurement developers can choose from a few common approaches discussed below based on their requirements.\n\n### Create and Manage Python Measurement Package using Poetry\n\n1. Install `poetry` (one-time setup)\n\n    1. Make sure the system has the recommended Python version installed.\n\n    2. Install `poetry` using the installation steps given in <https://python-poetry.org/docs/#installation>.\n\n2. Create a new Python project and add `ni-measurementlink-service` as a dependency to the project.\n\n    1. Open a command prompt, and change the working directory to the directory of your choice where you want to create the project.\n\n        ``` cmd\n        cd <path_of_directory_of_your_choice>\n        ```\n\n    2. Create a Python package (project) using the `poetry new` command. Poetry will create boilerplate files and folders that are commonly needed for a Python project.\n\n        ``` cmd\n        poetry new <name_of_the_project>\n        ```\n\n    3. Add the `ni-measurementlink-service` package as a dependency using the [`poetry add`](https://python-poetry.org/docs/cli/#add) command.\n\n        ``` cmd\n        cd <name_of_the_project>\n        poetry add ni-measurementlink-service\n        ```\n\n    4. The virtual environment will be auto-created by poetry.\n\n    5. Create measurement modules as described in ["Developing a minimal Python measurement"](#developing-a-minimal-python-measurement)\n        - Any additional dependencies required by measurement can be added using [add command](https://python-poetry.org/docs/cli/#add).\n\n            ``` cmd\n            poetry add <dependency_package_name>\n            ```\n\nFor detailed info on managing projects using poetry [refer to the official documentation](https://python-poetry.org/docs/cli/).\n\n### Create and Manage Python Measurement Package using `venv`\n\n1. Make sure the system has the recommended Python version installed.\n\n2. Open a command prompt, and change the working directory to the directory of your choice where you want to create a project.\n\n    ``` cmd\n    cd <path_of_directory_of_your_choice>\n    ```\n\n3. Create a virtual environment.\n\n    ``` cmd\n    REM This creates a virtual environment named .venv\n    python -m venv .venv\n    ```\n\n4. Activate the virtual environment. After successful activation\n\n    ``` cmd\n    .venv\\scripts\\activate\n    REM Optionally upgrade the pip within the venv by executing the command\n    python -m pip install -U pip\n    ```\n\n5. Install the `ni-measurementlink-service` package into the virtual environment.\n\n    ``` cmd\n    pip install ni-measurementlink-service\n    ```\n\n6. Create measurement modules as described in ["Developing a minimal Python measurement"](#developing-a-minimal-python-measurement)\n    - Any additional dependencies required by measurement can be added pip install.\n\n        ``` cmd\n        pip install <dependency_package_name>\n        ```\n\nFor detailed info on managing projects with a virtual environment, refer to the [official documentation](https://docs.python.org/3/tutorial/venv.html).\n\n### Create and Manage Python Measurement Package by directly installing `ni-measurementlink-service` as a system-level package\n\nMeasurement developers can also install `ni-measurementlink-service` as a system package if necessary.\n\n1. Install the `ni-measurementlink-service` package from the command prompt\n\n    ``` cmd\n    pip install ni-measurementlink-service\n    ```\n\n2. Create measurement modules as described in ["Developing a minimal Python measurement"](#developing-a-minimal-python-measurement)\n\n---\n',
     'author': 'NI',
     'author_email': 'opensource@ni.com',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'https://github.com/ni/measurementlink-python/',
     'packages': packages,
     'package_data': package_data,
```

### Comparing `ni_measurementlink_service-1.1.0.dev1/PKG-INFO` & `ni_measurementlink_service-1.1.0.dev2/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ni-measurementlink-service
-Version: 1.1.0.dev1
+Version: 1.1.0.dev2
 Summary: MeasurementLink Support for Python
 Home-page: https://github.com/ni/measurementlink-python/
 License: MIT
 Author: NI
 Author-email: opensource@ni.com
 Requires-Python: >=3.8,<4.0
 Classifier: Development Status :: 5 - Production/Stable
@@ -17,14 +17,15 @@
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Classifier: Topic :: Scientific/Engineering
 Classifier: Topic :: System :: Hardware
+Requires-Dist: deprecation (>=2.1)
 Requires-Dist: grpcio (>=1.49.1,<2.0.0)
 Requires-Dist: protobuf (>=4.21,<5.0)
 Requires-Dist: pywin32 (>=303); sys_platform == "win32"
 Project-URL: Repository, https://github.com/ni/measurementlink-python/
 Description-Content-Type: text/markdown
 
 # MeasurementLink™ Support for Python
@@ -89,14 +90,15 @@
 ## Examples
 
 The `examples` directory contains example measurements for MeasurementLink 2023 Q3 or later. If
 you are using a previous version of MeasurementLink, download the appropriate examples:
 
 - MeasurementLink 2023 Q1: [measurementlink-python-examples-1.0.1.zip](https://github.com/ni/measurementlink-python/releases/download/1.0.1/measurementlink-python-examples-1.0.1.zip)
 - MeasurementLink 2023 Q2: [measurementlink-python-examples-1.0.1.zip](https://github.com/ni/measurementlink-python/releases/download/1.0.1/measurementlink-python-examples-1.0.1.zip)
+- MeasurementLink 2023 Q3: [measurementlink-python-examples-1.1.0.zip](https://github.com/ni/measurementlink-python/releases/download/1.1.0/measurementlink-python-examples-1.1.0.zip)
 
 For more information on setting up and running the example measurements, see the included `README.md` file.
 
 For best results, use the example measurements corresponding to the version of MeasurementLink
 that you are using. Newer examples may demonstrate features that are not available in older
 versions of MeasurementLink.
 
@@ -216,15 +218,17 @@
 
 To statically register a measurement service with the MeasurementLink discovery service, do the following:
 
 1. Create a [startup batch file](#create-a-batch-file-that-runs-a-python-measurement) or [executable](#create-executable-for-python-scripts) for the measurement service.
 
 2. Edit the measurement service's `.serviceconfig` file and set the `path` value to the filename of the startup batch file or executable.
 
-3. Copy the measurement service's directory (including the `.venv` subdirectory if present, `.serviceconfig` file, and startup batch file) to a subdirectory of `C:\ProgramData\National Instruments\MeasurementLink\Services`. 
+3. Copy the measurement service's directory (including the `.serviceconfig` file and startup batch file) to a subdirectory of `C:\ProgramData\National Instruments\MeasurementLink\Services`.
+> **Note**
+> If you are using a virtual environment, do not copy the `.venv` subdirectory&mdash;the virtual environment must be re-created in the new location.
 
 Once your measurement service is statically registered, the MeasurementLink discovery service makes it visible in supported NI applications.
 
 ### Create a batch file that runs a Python measurement
 
 The batch file used for static registration is responsible for starting the Python Scripts.
```

