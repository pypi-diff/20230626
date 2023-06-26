# Comparing `tmp/th2_grpc_common-4.3.0.dev5346797023.tar.gz` & `tmp/th2_grpc_common-4.3.0.dev5374522280.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/th2_grpc_common-4.3.0.dev5346797023.tar", last modified: Thu Jun 22 14:29:57 2023, max compression
+gzip compressed data, was "dist/th2_grpc_common-4.3.0.dev5374522280.tar", last modified: Mon Jun 26 06:24:00 2023, max compression
```

## Comparing `th2_grpc_common-4.3.0.dev5346797023.tar` & `th2_grpc_common-4.3.0.dev5374522280.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-22 14:29:57.000000 th2_grpc_common-4.3.0.dev5346797023/
--rw-r--r--   0 runner    (1001) docker     (122)     6568 2023-06-22 14:29:57.000000 th2_grpc_common-4.3.0.dev5346797023/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (122)     5001 2023-06-22 14:29:02.000000 th2_grpc_common-4.3.0.dev5346797023/README.md
--rw-r--r--   0 runner    (1001) docker     (122)       83 2023-06-22 14:29:02.000000 th2_grpc_common-4.3.0.dev5346797023/package_info.json
--rw-r--r--   0 runner    (1001) docker     (122)       38 2023-06-22 14:29:57.000000 th2_grpc_common-4.3.0.dev5346797023/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (122)     4491 2023-06-22 14:29:02.000000 th2_grpc_common-4.3.0.dev5346797023/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-22 14:29:57.000000 th2_grpc_common-4.3.0.dev5346797023/th2_grpc_common/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-06-22 14:29:56.000000 th2_grpc_common-4.3.0.dev5346797023/th2_grpc_common/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     8610 2023-06-22 14:29:02.000000 th2_grpc_common-4.3.0.dev5346797023/th2_grpc_common/common.proto
--rw-r--r--   0 runner    (1001) docker     (122)    14802 2023-06-22 14:29:56.000000 th2_grpc_common-4.3.0.dev5346797023/th2_grpc_common/common_pb2.py
--rw-r--r--   0 runner    (1001) docker     (122)    45617 2023-06-22 14:29:56.000000 th2_grpc_common-4.3.0.dev5346797023/th2_grpc_common/common_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (122)      159 2023-06-22 14:29:56.000000 th2_grpc_common-4.3.0.dev5346797023/th2_grpc_common/common_pb2_grpc.py
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-06-22 14:29:56.000000 th2_grpc_common-4.3.0.dev5346797023/th2_grpc_common/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-22 14:29:57.000000 th2_grpc_common-4.3.0.dev5346797023/th2_grpc_common.egg-info/
--rw-r--r--   0 runner    (1001) docker     (122)     6568 2023-06-22 14:29:56.000000 th2_grpc_common-4.3.0.dev5346797023/th2_grpc_common.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (122)      408 2023-06-22 14:29:57.000000 th2_grpc_common-4.3.0.dev5346797023/th2_grpc_common.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (122)        1 2023-06-22 14:29:56.000000 th2_grpc_common-4.3.0.dev5346797023/th2_grpc_common.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (122)       40 2023-06-22 14:29:56.000000 th2_grpc_common-4.3.0.dev5346797023/th2_grpc_common.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (122)       17 2023-06-22 14:29:56.000000 th2_grpc_common-4.3.0.dev5346797023/th2_grpc_common.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-26 06:24:00.000000 th2_grpc_common-4.3.0.dev5374522280/
+-rw-r--r--   0 runner    (1001) docker     (122)     6568 2023-06-26 06:24:00.000000 th2_grpc_common-4.3.0.dev5374522280/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (122)     5001 2023-06-26 06:23:01.000000 th2_grpc_common-4.3.0.dev5374522280/README.md
+-rw-r--r--   0 runner    (1001) docker     (122)       83 2023-06-26 06:23:02.000000 th2_grpc_common-4.3.0.dev5374522280/package_info.json
+-rw-r--r--   0 runner    (1001) docker     (122)       38 2023-06-26 06:24:00.000000 th2_grpc_common-4.3.0.dev5374522280/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (122)     4491 2023-06-26 06:23:01.000000 th2_grpc_common-4.3.0.dev5374522280/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-26 06:24:00.000000 th2_grpc_common-4.3.0.dev5374522280/th2_grpc_common/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-06-26 06:24:00.000000 th2_grpc_common-4.3.0.dev5374522280/th2_grpc_common/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     8610 2023-06-26 06:23:01.000000 th2_grpc_common-4.3.0.dev5374522280/th2_grpc_common/common.proto
+-rw-r--r--   0 runner    (1001) docker     (122)    15925 2023-06-26 06:24:00.000000 th2_grpc_common-4.3.0.dev5374522280/th2_grpc_common/common_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (122)    45617 2023-06-26 06:24:00.000000 th2_grpc_common-4.3.0.dev5374522280/th2_grpc_common/common_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (122)      159 2023-06-26 06:24:00.000000 th2_grpc_common-4.3.0.dev5374522280/th2_grpc_common/common_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-06-26 06:24:00.000000 th2_grpc_common-4.3.0.dev5374522280/th2_grpc_common/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-26 06:24:00.000000 th2_grpc_common-4.3.0.dev5374522280/th2_grpc_common.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (122)     6568 2023-06-26 06:24:00.000000 th2_grpc_common-4.3.0.dev5374522280/th2_grpc_common.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (122)      408 2023-06-26 06:24:00.000000 th2_grpc_common-4.3.0.dev5374522280/th2_grpc_common.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (122)        1 2023-06-26 06:24:00.000000 th2_grpc_common-4.3.0.dev5374522280/th2_grpc_common.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (122)       40 2023-06-26 06:24:00.000000 th2_grpc_common-4.3.0.dev5374522280/th2_grpc_common.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (122)       17 2023-06-26 06:24:00.000000 th2_grpc_common-4.3.0.dev5374522280/th2_grpc_common.egg-info/top_level.txt
```

### Comparing `th2_grpc_common-4.3.0.dev5346797023/PKG-INFO` & `th2_grpc_common-4.3.0.dev5374522280/th2_grpc_common.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
-Name: th2_grpc_common
-Version: 4.3.0.dev5346797023
+Name: th2-grpc-common
+Version: 4.3.0.dev5374522280
 Summary: th2_grpc_common
 Home-page: https://github.com/th2-net/th2-grpc-common
 Author: TH2-devs
 Author-email: th2-devs@exactprosystems.com
 License: Apache License 2.0
 Description: # th2 gRPC common library (4.3.0)
         
@@ -56,15 +56,15 @@
         ## Release notes
         
         ### 4.3.0
         
         + Added golang specific properties
         + Updated bom:4.4.0
         + Updated grpc-service-generator:3.4.0
-        + Updated grpcio-tools:1.54.2
+        + Updated grpcio-tools:1.56.0
         + Updated mypy-protobuf:3.4
         
         ### 4.2.0
         
         + Added vulnerability check
         + Updated bom:4.2.0
         + Updated protoc:3.21.7
```

### Comparing `th2_grpc_common-4.3.0.dev5346797023/README.md` & `th2_grpc_common-4.3.0.dev5374522280/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -48,15 +48,15 @@
 ## Release notes
 
 ### 4.3.0
 
 + Added golang specific properties
 + Updated bom:4.4.0
 + Updated grpc-service-generator:3.4.0
-+ Updated grpcio-tools:1.54.2
++ Updated grpcio-tools:1.56.0
 + Updated mypy-protobuf:3.4
 
 ### 4.2.0
 
 + Added vulnerability check
 + Updated bom:4.2.0
 + Updated protoc:3.21.7
```

### Comparing `th2_grpc_common-4.3.0.dev5346797023/setup.py` & `th2_grpc_common-4.3.0.dev5374522280/setup.py`

 * *Files identical despite different names*

### Comparing `th2_grpc_common-4.3.0.dev5346797023/th2_grpc_common/common.proto` & `th2_grpc_common-4.3.0.dev5374522280/th2_grpc_common/common.proto`

 * *Files identical despite different names*

### Comparing `th2_grpc_common-4.3.0.dev5346797023/th2_grpc_common/common_pb2.py` & `th2_grpc_common-4.3.0.dev5374522280/th2_grpc_common/common_pb2.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,29 +1,30 @@
 # -*- coding: utf-8 -*-
 # Generated by the protocol buffer compiler.  DO NOT EDIT!
 # source: th2_grpc_common/common.proto
 """Generated protocol buffer code."""
-from google.protobuf.internal import builder as _builder
 from google.protobuf import descriptor as _descriptor
 from google.protobuf import descriptor_pool as _descriptor_pool
 from google.protobuf import symbol_database as _symbol_database
+from google.protobuf.internal import builder as _builder
 # @@protoc_insertion_point(imports)
 
 _sym_db = _symbol_database.Default()
 
 
 from google.protobuf import timestamp_pb2 as google_dot_protobuf_dot_timestamp__pb2
 from google.protobuf import duration_pb2 as google_dot_protobuf_dot_duration__pb2
 from google.protobuf import wrappers_pb2 as google_dot_protobuf_dot_wrappers__pb2
 
 
 DESCRIPTOR = _descriptor_pool.Default().AddSerializedFile(b'\n\x1cth2_grpc_common/common.proto\x1a\x1fgoogle/protobuf/timestamp.proto\x1a\x1egoogle/protobuf/duration.proto\x1a\x1egoogle/protobuf/wrappers.proto\"<\n\x0c\x43onnectionID\x12\x15\n\rsession_alias\x18\x01 \x01(\t\x12\x15\n\rsession_group\x18\x02 \x01(\t\"\xb9\x01\n\tMessageID\x12$\n\rconnection_id\x18\x01 \x01(\x0b\x32\r.ConnectionID\x12\x1d\n\tdirection\x18\x02 \x01(\x0e\x32\n.Direction\x12\x10\n\x08sequence\x18\x03 \x01(\x03\x12\x13\n\x0bsubsequence\x18\x04 \x03(\r\x12\x11\n\tbook_name\x18\x05 \x01(\t\x12-\n\ttimestamp\x18\x06 \x01(\x0b\x32\x1a.google.protobuf.Timestamp\",\n\x12\x45ventBatchMetadata\x12\x16\n\x0e\x65xternal_queue\x18\x01 \x01(\t\"3\n\x19MessageGroupBatchMetadata\x12\x16\n\x0e\x65xternal_queue\x18\x01 \x01(\t\"\xc0\x01\n\x0fMessageMetadata\x12\x16\n\x02id\x18\x01 \x01(\x0b\x32\n.MessageID\x12\x14\n\x0cmessage_type\x18\x03 \x01(\t\x12\x34\n\nproperties\x18\x04 \x03(\x0b\x32 .MessageMetadata.PropertiesEntry\x12\x10\n\x08protocol\x18\x05 \x01(\t\x1a\x31\n\x0fPropertiesEntry\x12\x0b\n\x03key\x18\x01 \x01(\t\x12\r\n\x05value\x18\x02 \x01(\t:\x02\x38\x01J\x04\x08\x02\x10\x03\"\xb0\x01\n\x12RawMessageMetadata\x12\x16\n\x02id\x18\x01 \x01(\x0b\x32\n.MessageID\x12\x37\n\nproperties\x18\x03 \x03(\x0b\x32#.RawMessageMetadata.PropertiesEntry\x12\x10\n\x08protocol\x18\x04 \x01(\t\x1a\x31\n\x0fPropertiesEntry\x12\x0b\n\x03key\x18\x01 \x01(\t\x12\r\n\x05value\x18\x02 \x01(\t:\x02\x38\x01J\x04\x08\x02\x10\x03\"\x8e\x01\n\x05Value\x12 \n\nnull_value\x18\x01 \x01(\x0e\x32\n.NullValueH\x00\x12\x16\n\x0csimple_value\x18\x02 \x01(\tH\x00\x12!\n\rmessage_value\x18\x03 \x01(\x0b\x32\x08.MessageH\x00\x12 \n\nlist_value\x18\x04 \x01(\x0b\x32\n.ListValueH\x00\x42\x06\n\x04kind\"#\n\tListValue\x12\x16\n\x06values\x18\x01 \x03(\x0b\x32\x06.Value\"\xad\x01\n\x07Message\x12!\n\x0fparent_event_id\x18\x03 \x01(\x0b\x32\x08.EventID\x12\"\n\x08metadata\x18\x01 \x01(\x0b\x32\x10.MessageMetadata\x12$\n\x06\x66ields\x18\x02 \x03(\x0b\x32\x14.Message.FieldsEntry\x1a\x35\n\x0b\x46ieldsEntry\x12\x0b\n\x03key\x18\x01 \x01(\t\x12\x15\n\x05value\x18\x02 \x01(\x0b\x32\x06.Value:\x02\x38\x01\"d\n\nRawMessage\x12!\n\x0fparent_event_id\x18\x03 \x01(\x0b\x32\x08.EventID\x12%\n\x08metadata\x18\x01 \x01(\x0b\x32\x13.RawMessageMetadata\x12\x0c\n\x04\x62ody\x18\x02 \x01(\x0c\"U\n\nAnyMessage\x12\x1b\n\x07message\x18\x01 \x01(\x0b\x32\x08.MessageH\x00\x12\"\n\x0braw_message\x18\x02 \x01(\x0b\x32\x0b.RawMessageH\x00\x42\x06\n\x04kind\"-\n\x0cMessageGroup\x12\x1d\n\x08messages\x18\x01 \x03(\x0b\x32\x0b.AnyMessage\"*\n\x0cMessageBatch\x12\x1a\n\x08messages\x18\x01 \x03(\x0b\x32\x08.Message\"0\n\x0fRawMessageBatch\x12\x1d\n\x08messages\x18\x01 \x03(\x0b\x32\x0b.RawMessage\"`\n\x11MessageGroupBatch\x12,\n\x08metadata\x18\x02 \x01(\x0b\x32\x1a.MessageGroupBatchMetadata\x12\x1d\n\x06groups\x18\x01 \x03(\x0b\x32\r.MessageGroup\"i\n\rRequestStatus\x12%\n\x06status\x18\x01 \x01(\x0e\x32\x15.RequestStatus.Status\x12\x0f\n\x07message\x18\x02 \x01(\t\" \n\x06Status\x12\x0b\n\x07SUCCESS\x10\x00\x12\t\n\x05\x45RROR\x10\x01\"D\n\x12\x43omparisonSettings\x12(\n\x0f\x66\x61il_unexpected\x18\x02 \x01(\x0e\x32\x0f.FailUnexpectedJ\x04\x08\x01\x10\x02\"\xa2\x01\n\x16RootComparisonSettings\x12\x15\n\rignore_fields\x18\x01 \x03(\t\x12#\n\x1b\x63heck_repeating_group_order\x18\x02 \x01(\x08\x12\x31\n\x0etime_precision\x18\x03 \x01(\x0b\x32\x19.google.protobuf.Duration\x12\x19\n\x11\x64\x65\x63imal_precision\x18\x04 \x01(\t\"\xf9\x01\n\x0bValueFilter\x12#\n\toperation\x18\x01 \x01(\x0e\x32\x10.FilterOperation\x12\x0b\n\x03key\x18\x02 \x01(\x08\x12\x17\n\rsimple_filter\x18\x03 \x01(\tH\x00\x12(\n\x0emessage_filter\x18\x04 \x01(\x0b\x32\x0e.MessageFilterH\x00\x12\'\n\x0blist_filter\x18\x05 \x01(\x0b\x32\x10.ListValueFilterH\x00\x12\"\n\x0bsimple_list\x18\x06 \x01(\x0b\x32\x0b.SimpleListH\x00\x12 \n\nnull_value\x18\x07 \x01(\x0e\x32\n.NullValueH\x00\x42\x06\n\x04kind\"/\n\x0fListValueFilter\x12\x1c\n\x06values\x18\x01 \x03(\x0b\x32\x0c.ValueFilter\"#\n\nSimpleList\x12\x15\n\rsimple_values\x18\x01 \x03(\t\"\xb6\x01\n\rMessageFilter\x12*\n\x06\x66ields\x18\x03 \x03(\x0b\x32\x1a.MessageFilter.FieldsEntry\x12\x30\n\x13\x63omparison_settings\x18\x04 \x01(\x0b\x32\x13.ComparisonSettings\x1a;\n\x0b\x46ieldsEntry\x12\x0b\n\x03key\x18\x01 \x01(\t\x12\x1b\n\x05value\x18\x02 \x01(\x0b\x32\x0c.ValueFilter:\x02\x38\x01J\x04\x08\x01\x10\x02J\x04\x08\x02\x10\x03\"\xae\x02\n\x0eMetadataFilter\x12>\n\x10property_filters\x18\x01 \x03(\x0b\x32$.MetadataFilter.PropertyFiltersEntry\x1a\x85\x01\n\x0cSimpleFilter\x12#\n\toperation\x18\x01 \x01(\x0e\x32\x10.FilterOperation\x12\x0b\n\x03key\x18\x02 \x01(\x08\x12\x0f\n\x05value\x18\x03 \x01(\tH\x00\x12\"\n\x0bsimple_list\x18\x04 \x01(\x0b\x32\x0b.SimpleListH\x00\x42\x0e\n\x0c\x66ilter_value\x1aT\n\x14PropertyFiltersEntry\x12\x0b\n\x03key\x18\x01 \x01(\t\x12+\n\x05value\x18\x02 \x01(\x0b\x32\x1c.MetadataFilter.SimpleFilter:\x02\x38\x01\"\xe3\x01\n\x11RootMessageFilter\x12\x13\n\x0bmessageType\x18\x01 \x01(\t\x12&\n\x0emessage_filter\x18\x02 \x01(\x0b\x32\x0e.MessageFilter\x12(\n\x0fmetadata_filter\x18\x03 \x01(\x0b\x32\x0f.MetadataFilter\x12\x34\n\x13\x63omparison_settings\x18\x04 \x01(\x0b\x32\x17.RootComparisonSettings\x12\x31\n\x0b\x64\x65scription\x18\x05 \x01(\x0b\x32\x1c.google.protobuf.StringValue\"\xe8\x06\n\nCheckpoint\x12\n\n\x02id\x18\x01 \x01(\t\x12x\n2book_name_to_session_alias_to_direction_checkpoint\x18\x03 \x03(\x0b\x32<.Checkpoint.BookNameToSessionAliasToDirectionCheckpointEntry\x1a\x81\x01\n0BookNameToSessionAliasToDirectionCheckpointEntry\x12\x0b\n\x03key\x18\x01 \x01(\t\x12<\n\x05value\x18\x02 \x01(\x0b\x32-.Checkpoint.SessionAliasToDirectionCheckpoint:\x02\x38\x01\x1a\x94\x02\n!SessionAliasToDirectionCheckpoint\x12\x83\x01\n%session_alias_to_direction_checkpoint\x18\x01 \x03(\x0b\x32T.Checkpoint.SessionAliasToDirectionCheckpoint.SessionAliasToDirectionCheckpointEntry\x1ai\n&SessionAliasToDirectionCheckpointEntry\x12\x0b\n\x03key\x18\x01 \x01(\t\x12.\n\x05value\x18\x02 \x01(\x0b\x32\x1f.Checkpoint.DirectionCheckpoint:\x02\x38\x01\x1a\xdf\x01\n\x13\x44irectionCheckpoint\x12\x64\n\x1c\x64irection_to_checkpoint_data\x18\x02 \x03(\x0b\x32>.Checkpoint.DirectionCheckpoint.DirectionToCheckpointDataEntry\x1a\\\n\x1e\x44irectionToCheckpointDataEntry\x12\x0b\n\x03key\x18\x01 \x01(\x05\x12)\n\x05value\x18\x02 \x01(\x0b\x32\x1a.Checkpoint.CheckpointData:\x02\x38\x01J\x04\x08\x01\x10\x02\x1aQ\n\x0e\x43heckpointData\x12\x10\n\x08sequence\x18\x01 \x01(\x03\x12-\n\ttimestamp\x18\x02 \x01(\x0b\x32\x1a.google.protobuf.TimestampJ\x04\x08\x02\x10\x03\"l\n\x07\x45ventID\x12\n\n\x02id\x18\x01 \x01(\t\x12\x11\n\tbook_name\x18\x02 \x01(\t\x12\r\n\x05scope\x18\x03 \x01(\t\x12\x33\n\x0fstart_timestamp\x18\x04 \x01(\x0b\x32\x1a.google.protobuf.Timestamp\"\xe5\x01\n\x05\x45vent\x12\x14\n\x02id\x18\x01 \x01(\x0b\x32\x08.EventID\x12\x1b\n\tparent_id\x18\x02 \x01(\x0b\x32\x08.EventID\x12\x31\n\rend_timestamp\x18\x04 \x01(\x0b\x32\x1a.google.protobuf.Timestamp\x12\x1c\n\x06status\x18\x05 \x01(\x0e\x32\x0c.EventStatus\x12\x0c\n\x04name\x18\x06 \x01(\t\x12\x0c\n\x04type\x18\x07 \x01(\t\x12\x0c\n\x04\x62ody\x18\x08 \x01(\x0c\x12(\n\x14\x61ttached_message_ids\x18\t \x03(\x0b\x32\n.MessageIDJ\x04\x08\x03\x10\x04\"n\n\nEventBatch\x12%\n\x08metadata\x18\x03 \x01(\x0b\x32\x13.EventBatchMetadata\x12!\n\x0fparent_event_id\x18\x01 \x01(\x0b\x32\x08.EventID\x12\x16\n\x06\x65vents\x18\x02 \x03(\x0b\x32\x06.Event*\"\n\tDirection\x12\t\n\x05\x46IRST\x10\x00\x12\n\n\x06SECOND\x10\x01*\x1b\n\tNullValue\x12\x0e\n\nNULL_VALUE\x10\x00*=\n\x0e\x46\x61ilUnexpected\x12\x06\n\x02NO\x10\x00\x12\n\n\x06\x46IELDS\x10\x01\x12\x17\n\x13\x46IELDS_AND_MESSAGES\x10\x02*\xf2\x01\n\x0f\x46ilterOperation\x12\t\n\x05\x45QUAL\x10\x00\x12\r\n\tNOT_EQUAL\x10\x01\x12\t\n\x05\x45MPTY\x10\x02\x12\r\n\tNOT_EMPTY\x10\x03\x12\x06\n\x02IN\x10\x04\x12\n\n\x06NOT_IN\x10\x05\x12\x08\n\x04LIKE\x10\x06\x12\x0c\n\x08NOT_LIKE\x10\x07\x12\x08\n\x04MORE\x10\x08\x12\x0c\n\x08NOT_MORE\x10\t\x12\x08\n\x04LESS\x10\n\x12\x0c\n\x08NOT_LESS\x10\x0b\x12\x0c\n\x08WILDCARD\x10\x0c\x12\x10\n\x0cNOT_WILDCARD\x10\r\x12\x15\n\x11\x45Q_TIME_PRECISION\x10\x0e\x12\x18\n\x14\x45Q_DECIMAL_PRECISION\x10\x0f*&\n\x0b\x45ventStatus\x12\x0b\n\x07SUCCESS\x10\x00\x12\n\n\x06\x46\x41ILED\x10\x01\x42:\n\x1c\x63om.exactpro.th2.common.grpcP\x01Z\x18th2-grpc/th2_grpc_commonb\x06proto3')
 
-_builder.BuildMessageAndEnumDescriptors(DESCRIPTOR, globals())
-_builder.BuildTopDescriptorsAndMessages(DESCRIPTOR, 'th2_grpc_common.common_pb2', globals())
+_globals = globals()
+_builder.BuildMessageAndEnumDescriptors(DESCRIPTOR, _globals)
+_builder.BuildTopDescriptorsAndMessages(DESCRIPTOR, 'th2_grpc_common.common_pb2', _globals)
 if _descriptor._USE_C_DESCRIPTORS == False:
 
   DESCRIPTOR._options = None
   DESCRIPTOR._serialized_options = b'\n\034com.exactpro.th2.common.grpcP\001Z\030th2-grpc/th2_grpc_common'
   _MESSAGEMETADATA_PROPERTIESENTRY._options = None
   _MESSAGEMETADATA_PROPERTIESENTRY._serialized_options = b'8\001'
   _RAWMESSAGEMETADATA_PROPERTIESENTRY._options = None
@@ -36,100 +37,100 @@
   _METADATAFILTER_PROPERTYFILTERSENTRY._serialized_options = b'8\001'
   _CHECKPOINT_BOOKNAMETOSESSIONALIASTODIRECTIONCHECKPOINTENTRY._options = None
   _CHECKPOINT_BOOKNAMETOSESSIONALIASTODIRECTIONCHECKPOINTENTRY._serialized_options = b'8\001'
   _CHECKPOINT_SESSIONALIASTODIRECTIONCHECKPOINT_SESSIONALIASTODIRECTIONCHECKPOINTENTRY._options = None
   _CHECKPOINT_SESSIONALIASTODIRECTIONCHECKPOINT_SESSIONALIASTODIRECTIONCHECKPOINTENTRY._serialized_options = b'8\001'
   _CHECKPOINT_DIRECTIONCHECKPOINT_DIRECTIONTOCHECKPOINTDATAENTRY._options = None
   _CHECKPOINT_DIRECTIONCHECKPOINT_DIRECTIONTOCHECKPOINTDATAENTRY._serialized_options = b'8\001'
-  _DIRECTION._serialized_start=4367
-  _DIRECTION._serialized_end=4401
-  _NULLVALUE._serialized_start=4403
-  _NULLVALUE._serialized_end=4430
-  _FAILUNEXPECTED._serialized_start=4432
-  _FAILUNEXPECTED._serialized_end=4493
-  _FILTEROPERATION._serialized_start=4496
-  _FILTEROPERATION._serialized_end=4738
-  _EVENTSTATUS._serialized_start=4740
-  _EVENTSTATUS._serialized_end=4778
-  _CONNECTIONID._serialized_start=129
-  _CONNECTIONID._serialized_end=189
-  _MESSAGEID._serialized_start=192
-  _MESSAGEID._serialized_end=377
-  _EVENTBATCHMETADATA._serialized_start=379
-  _EVENTBATCHMETADATA._serialized_end=423
-  _MESSAGEGROUPBATCHMETADATA._serialized_start=425
-  _MESSAGEGROUPBATCHMETADATA._serialized_end=476
-  _MESSAGEMETADATA._serialized_start=479
-  _MESSAGEMETADATA._serialized_end=671
-  _MESSAGEMETADATA_PROPERTIESENTRY._serialized_start=616
-  _MESSAGEMETADATA_PROPERTIESENTRY._serialized_end=665
-  _RAWMESSAGEMETADATA._serialized_start=674
-  _RAWMESSAGEMETADATA._serialized_end=850
-  _RAWMESSAGEMETADATA_PROPERTIESENTRY._serialized_start=616
-  _RAWMESSAGEMETADATA_PROPERTIESENTRY._serialized_end=665
-  _VALUE._serialized_start=853
-  _VALUE._serialized_end=995
-  _LISTVALUE._serialized_start=997
-  _LISTVALUE._serialized_end=1032
-  _MESSAGE._serialized_start=1035
-  _MESSAGE._serialized_end=1208
-  _MESSAGE_FIELDSENTRY._serialized_start=1155
-  _MESSAGE_FIELDSENTRY._serialized_end=1208
-  _RAWMESSAGE._serialized_start=1210
-  _RAWMESSAGE._serialized_end=1310
-  _ANYMESSAGE._serialized_start=1312
-  _ANYMESSAGE._serialized_end=1397
-  _MESSAGEGROUP._serialized_start=1399
-  _MESSAGEGROUP._serialized_end=1444
-  _MESSAGEBATCH._serialized_start=1446
-  _MESSAGEBATCH._serialized_end=1488
-  _RAWMESSAGEBATCH._serialized_start=1490
-  _RAWMESSAGEBATCH._serialized_end=1538
-  _MESSAGEGROUPBATCH._serialized_start=1540
-  _MESSAGEGROUPBATCH._serialized_end=1636
-  _REQUESTSTATUS._serialized_start=1638
-  _REQUESTSTATUS._serialized_end=1743
-  _REQUESTSTATUS_STATUS._serialized_start=1711
-  _REQUESTSTATUS_STATUS._serialized_end=1743
-  _COMPARISONSETTINGS._serialized_start=1745
-  _COMPARISONSETTINGS._serialized_end=1813
-  _ROOTCOMPARISONSETTINGS._serialized_start=1816
-  _ROOTCOMPARISONSETTINGS._serialized_end=1978
-  _VALUEFILTER._serialized_start=1981
-  _VALUEFILTER._serialized_end=2230
-  _LISTVALUEFILTER._serialized_start=2232
-  _LISTVALUEFILTER._serialized_end=2279
-  _SIMPLELIST._serialized_start=2281
-  _SIMPLELIST._serialized_end=2316
-  _MESSAGEFILTER._serialized_start=2319
-  _MESSAGEFILTER._serialized_end=2501
-  _MESSAGEFILTER_FIELDSENTRY._serialized_start=2430
-  _MESSAGEFILTER_FIELDSENTRY._serialized_end=2489
-  _METADATAFILTER._serialized_start=2504
-  _METADATAFILTER._serialized_end=2806
-  _METADATAFILTER_SIMPLEFILTER._serialized_start=2587
-  _METADATAFILTER_SIMPLEFILTER._serialized_end=2720
-  _METADATAFILTER_PROPERTYFILTERSENTRY._serialized_start=2722
-  _METADATAFILTER_PROPERTYFILTERSENTRY._serialized_end=2806
-  _ROOTMESSAGEFILTER._serialized_start=2809
-  _ROOTMESSAGEFILTER._serialized_end=3036
-  _CHECKPOINT._serialized_start=3039
-  _CHECKPOINT._serialized_end=3911
-  _CHECKPOINT_BOOKNAMETOSESSIONALIASTODIRECTIONCHECKPOINTENTRY._serialized_start=3188
-  _CHECKPOINT_BOOKNAMETOSESSIONALIASTODIRECTIONCHECKPOINTENTRY._serialized_end=3317
-  _CHECKPOINT_SESSIONALIASTODIRECTIONCHECKPOINT._serialized_start=3320
-  _CHECKPOINT_SESSIONALIASTODIRECTIONCHECKPOINT._serialized_end=3596
-  _CHECKPOINT_SESSIONALIASTODIRECTIONCHECKPOINT_SESSIONALIASTODIRECTIONCHECKPOINTENTRY._serialized_start=3491
-  _CHECKPOINT_SESSIONALIASTODIRECTIONCHECKPOINT_SESSIONALIASTODIRECTIONCHECKPOINTENTRY._serialized_end=3596
-  _CHECKPOINT_DIRECTIONCHECKPOINT._serialized_start=3599
-  _CHECKPOINT_DIRECTIONCHECKPOINT._serialized_end=3822
-  _CHECKPOINT_DIRECTIONCHECKPOINT_DIRECTIONTOCHECKPOINTDATAENTRY._serialized_start=3724
-  _CHECKPOINT_DIRECTIONCHECKPOINT_DIRECTIONTOCHECKPOINTDATAENTRY._serialized_end=3816
-  _CHECKPOINT_CHECKPOINTDATA._serialized_start=3824
-  _CHECKPOINT_CHECKPOINTDATA._serialized_end=3905
-  _EVENTID._serialized_start=3913
-  _EVENTID._serialized_end=4021
-  _EVENT._serialized_start=4024
-  _EVENT._serialized_end=4253
-  _EVENTBATCH._serialized_start=4255
-  _EVENTBATCH._serialized_end=4365
+  _globals['_DIRECTION']._serialized_start=4367
+  _globals['_DIRECTION']._serialized_end=4401
+  _globals['_NULLVALUE']._serialized_start=4403
+  _globals['_NULLVALUE']._serialized_end=4430
+  _globals['_FAILUNEXPECTED']._serialized_start=4432
+  _globals['_FAILUNEXPECTED']._serialized_end=4493
+  _globals['_FILTEROPERATION']._serialized_start=4496
+  _globals['_FILTEROPERATION']._serialized_end=4738
+  _globals['_EVENTSTATUS']._serialized_start=4740
+  _globals['_EVENTSTATUS']._serialized_end=4778
+  _globals['_CONNECTIONID']._serialized_start=129
+  _globals['_CONNECTIONID']._serialized_end=189
+  _globals['_MESSAGEID']._serialized_start=192
+  _globals['_MESSAGEID']._serialized_end=377
+  _globals['_EVENTBATCHMETADATA']._serialized_start=379
+  _globals['_EVENTBATCHMETADATA']._serialized_end=423
+  _globals['_MESSAGEGROUPBATCHMETADATA']._serialized_start=425
+  _globals['_MESSAGEGROUPBATCHMETADATA']._serialized_end=476
+  _globals['_MESSAGEMETADATA']._serialized_start=479
+  _globals['_MESSAGEMETADATA']._serialized_end=671
+  _globals['_MESSAGEMETADATA_PROPERTIESENTRY']._serialized_start=616
+  _globals['_MESSAGEMETADATA_PROPERTIESENTRY']._serialized_end=665
+  _globals['_RAWMESSAGEMETADATA']._serialized_start=674
+  _globals['_RAWMESSAGEMETADATA']._serialized_end=850
+  _globals['_RAWMESSAGEMETADATA_PROPERTIESENTRY']._serialized_start=616
+  _globals['_RAWMESSAGEMETADATA_PROPERTIESENTRY']._serialized_end=665
+  _globals['_VALUE']._serialized_start=853
+  _globals['_VALUE']._serialized_end=995
+  _globals['_LISTVALUE']._serialized_start=997
+  _globals['_LISTVALUE']._serialized_end=1032
+  _globals['_MESSAGE']._serialized_start=1035
+  _globals['_MESSAGE']._serialized_end=1208
+  _globals['_MESSAGE_FIELDSENTRY']._serialized_start=1155
+  _globals['_MESSAGE_FIELDSENTRY']._serialized_end=1208
+  _globals['_RAWMESSAGE']._serialized_start=1210
+  _globals['_RAWMESSAGE']._serialized_end=1310
+  _globals['_ANYMESSAGE']._serialized_start=1312
+  _globals['_ANYMESSAGE']._serialized_end=1397
+  _globals['_MESSAGEGROUP']._serialized_start=1399
+  _globals['_MESSAGEGROUP']._serialized_end=1444
+  _globals['_MESSAGEBATCH']._serialized_start=1446
+  _globals['_MESSAGEBATCH']._serialized_end=1488
+  _globals['_RAWMESSAGEBATCH']._serialized_start=1490
+  _globals['_RAWMESSAGEBATCH']._serialized_end=1538
+  _globals['_MESSAGEGROUPBATCH']._serialized_start=1540
+  _globals['_MESSAGEGROUPBATCH']._serialized_end=1636
+  _globals['_REQUESTSTATUS']._serialized_start=1638
+  _globals['_REQUESTSTATUS']._serialized_end=1743
+  _globals['_REQUESTSTATUS_STATUS']._serialized_start=1711
+  _globals['_REQUESTSTATUS_STATUS']._serialized_end=1743
+  _globals['_COMPARISONSETTINGS']._serialized_start=1745
+  _globals['_COMPARISONSETTINGS']._serialized_end=1813
+  _globals['_ROOTCOMPARISONSETTINGS']._serialized_start=1816
+  _globals['_ROOTCOMPARISONSETTINGS']._serialized_end=1978
+  _globals['_VALUEFILTER']._serialized_start=1981
+  _globals['_VALUEFILTER']._serialized_end=2230
+  _globals['_LISTVALUEFILTER']._serialized_start=2232
+  _globals['_LISTVALUEFILTER']._serialized_end=2279
+  _globals['_SIMPLELIST']._serialized_start=2281
+  _globals['_SIMPLELIST']._serialized_end=2316
+  _globals['_MESSAGEFILTER']._serialized_start=2319
+  _globals['_MESSAGEFILTER']._serialized_end=2501
+  _globals['_MESSAGEFILTER_FIELDSENTRY']._serialized_start=2430
+  _globals['_MESSAGEFILTER_FIELDSENTRY']._serialized_end=2489
+  _globals['_METADATAFILTER']._serialized_start=2504
+  _globals['_METADATAFILTER']._serialized_end=2806
+  _globals['_METADATAFILTER_SIMPLEFILTER']._serialized_start=2587
+  _globals['_METADATAFILTER_SIMPLEFILTER']._serialized_end=2720
+  _globals['_METADATAFILTER_PROPERTYFILTERSENTRY']._serialized_start=2722
+  _globals['_METADATAFILTER_PROPERTYFILTERSENTRY']._serialized_end=2806
+  _globals['_ROOTMESSAGEFILTER']._serialized_start=2809
+  _globals['_ROOTMESSAGEFILTER']._serialized_end=3036
+  _globals['_CHECKPOINT']._serialized_start=3039
+  _globals['_CHECKPOINT']._serialized_end=3911
+  _globals['_CHECKPOINT_BOOKNAMETOSESSIONALIASTODIRECTIONCHECKPOINTENTRY']._serialized_start=3188
+  _globals['_CHECKPOINT_BOOKNAMETOSESSIONALIASTODIRECTIONCHECKPOINTENTRY']._serialized_end=3317
+  _globals['_CHECKPOINT_SESSIONALIASTODIRECTIONCHECKPOINT']._serialized_start=3320
+  _globals['_CHECKPOINT_SESSIONALIASTODIRECTIONCHECKPOINT']._serialized_end=3596
+  _globals['_CHECKPOINT_SESSIONALIASTODIRECTIONCHECKPOINT_SESSIONALIASTODIRECTIONCHECKPOINTENTRY']._serialized_start=3491
+  _globals['_CHECKPOINT_SESSIONALIASTODIRECTIONCHECKPOINT_SESSIONALIASTODIRECTIONCHECKPOINTENTRY']._serialized_end=3596
+  _globals['_CHECKPOINT_DIRECTIONCHECKPOINT']._serialized_start=3599
+  _globals['_CHECKPOINT_DIRECTIONCHECKPOINT']._serialized_end=3822
+  _globals['_CHECKPOINT_DIRECTIONCHECKPOINT_DIRECTIONTOCHECKPOINTDATAENTRY']._serialized_start=3724
+  _globals['_CHECKPOINT_DIRECTIONCHECKPOINT_DIRECTIONTOCHECKPOINTDATAENTRY']._serialized_end=3816
+  _globals['_CHECKPOINT_CHECKPOINTDATA']._serialized_start=3824
+  _globals['_CHECKPOINT_CHECKPOINTDATA']._serialized_end=3905
+  _globals['_EVENTID']._serialized_start=3913
+  _globals['_EVENTID']._serialized_end=4021
+  _globals['_EVENT']._serialized_start=4024
+  _globals['_EVENT']._serialized_end=4253
+  _globals['_EVENTBATCH']._serialized_start=4255
+  _globals['_EVENTBATCH']._serialized_end=4365
 # @@protoc_insertion_point(module_scope)
```

### Comparing `th2_grpc_common-4.3.0.dev5346797023/th2_grpc_common/common_pb2.pyi` & `th2_grpc_common-4.3.0.dev5374522280/th2_grpc_common/common_pb2.pyi`

 * *Files identical despite different names*

### Comparing `th2_grpc_common-4.3.0.dev5346797023/th2_grpc_common.egg-info/PKG-INFO` & `th2_grpc_common-4.3.0.dev5374522280/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
-Name: th2-grpc-common
-Version: 4.3.0.dev5346797023
+Name: th2_grpc_common
+Version: 4.3.0.dev5374522280
 Summary: th2_grpc_common
 Home-page: https://github.com/th2-net/th2-grpc-common
 Author: TH2-devs
 Author-email: th2-devs@exactprosystems.com
 License: Apache License 2.0
 Description: # th2 gRPC common library (4.3.0)
         
@@ -56,15 +56,15 @@
         ## Release notes
         
         ### 4.3.0
         
         + Added golang specific properties
         + Updated bom:4.4.0
         + Updated grpc-service-generator:3.4.0
-        + Updated grpcio-tools:1.54.2
+        + Updated grpcio-tools:1.56.0
         + Updated mypy-protobuf:3.4
         
         ### 4.2.0
         
         + Added vulnerability check
         + Updated bom:4.2.0
         + Updated protoc:3.21.7
```

