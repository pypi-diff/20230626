# Comparing `tmp/acore_server_metadata-0.5.1.tar.gz` & `tmp/acore_server_metadata-0.5.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "acore_server_metadata-0.5.1.tar", last modified: Thu Jun 22 16:35:01 2023, max compression
+gzip compressed data, was "acore_server_metadata-0.5.2.tar", last modified: Mon Jun 26 05:28:01 2023, max compression
```

## Comparing `acore_server_metadata-0.5.1.tar` & `acore_server_metadata-0.5.2.tar`

### file list

```diff
@@ -1,48 +1,48 @@
-drwxr-xr-x   0 sanhehu    (501) staff       (20)        0 2023-06-22 16:35:01.214875 acore_server_metadata-0.5.1/
--rw-r--r--   0 sanhehu    (501) staff       (20)      670 2023-06-15 16:37:48.000000 acore_server_metadata-0.5.1/AUTHORS.rst
--rw-r--r--   0 sanhehu    (501) staff       (20)     1132 2023-06-15 16:37:48.000000 acore_server_metadata-0.5.1/LICENSE.txt
--rw-r--r--   0 sanhehu    (501) staff       (20)      329 2023-06-15 16:37:48.000000 acore_server_metadata-0.5.1/MANIFEST.in
--rw-r--r--   0 sanhehu    (501) staff       (20)     7028 2023-06-22 16:35:01.214724 acore_server_metadata-0.5.1/PKG-INFO
--rw-r--r--   0 sanhehu    (501) staff       (20)     5879 2023-06-19 18:57:43.000000 acore_server_metadata-0.5.1/README.rst
-drwxr-xr-x   0 sanhehu    (501) staff       (20)        0 2023-06-22 16:35:01.209445 acore_server_metadata-0.5.1/acore_server_metadata/
--rw-r--r--   0 sanhehu    (501) staff       (20)      391 2023-06-16 02:28:42.000000 acore_server_metadata-0.5.1/acore_server_metadata/__init__.py
--rw-r--r--   0 sanhehu    (501) staff       (20)       93 2023-06-22 16:18:48.000000 acore_server_metadata-0.5.1/acore_server_metadata/_version.py
--rw-r--r--   0 sanhehu    (501) staff       (20)      105 2023-06-22 16:18:25.000000 acore_server_metadata-0.5.1/acore_server_metadata/api.py
-drwxr-xr-x   0 sanhehu    (501) staff       (20)        0 2023-06-22 16:35:01.210413 acore_server_metadata-0.5.1/acore_server_metadata/docs/
--rw-r--r--   0 sanhehu    (501) staff       (20)       43 2023-06-15 16:37:48.000000 acore_server_metadata-0.5.1/acore_server_metadata/docs/__init__.py
--rw-r--r--   0 sanhehu    (501) staff       (20)      496 2023-06-16 15:11:12.000000 acore_server_metadata-0.5.1/acore_server_metadata/exc.py
--rw-r--r--   0 sanhehu    (501) staff       (20)      642 2023-06-15 16:37:48.000000 acore_server_metadata-0.5.1/acore_server_metadata/paths.py
-drwxr-xr-x   0 sanhehu    (501) staff       (20)        0 2023-06-22 16:35:01.211853 acore_server_metadata-0.5.1/acore_server_metadata/server/
--rw-r--r--   0 sanhehu    (501) staff       (20)       25 2023-06-22 14:16:00.000000 acore_server_metadata-0.5.1/acore_server_metadata/server/__init__.py
--rw-r--r--   0 sanhehu    (501) staff       (20)      171 2023-06-22 15:54:39.000000 acore_server_metadata-0.5.1/acore_server_metadata/server/api.py
--rw-r--r--   0 sanhehu    (501) staff       (20)    12199 2023-06-22 15:59:52.000000 acore_server_metadata-0.5.1/acore_server_metadata/server/server.py
--rw-r--r--   0 sanhehu    (501) staff       (20)    17224 2023-06-22 16:17:47.000000 acore_server_metadata-0.5.1/acore_server_metadata/server/server_operation.py
--rw-r--r--   0 sanhehu    (501) staff       (20)     1665 2023-06-22 15:56:21.000000 acore_server_metadata-0.5.1/acore_server_metadata/server/server_status.py
--rw-r--r--   0 sanhehu    (501) staff       (20)       89 2023-06-15 20:16:40.000000 acore_server_metadata-0.5.1/acore_server_metadata/settings.py
-drwxr-xr-x   0 sanhehu    (501) staff       (20)        0 2023-06-22 16:35:01.212638 acore_server_metadata-0.5.1/acore_server_metadata/tests/
--rw-r--r--   0 sanhehu    (501) staff       (20)       58 2023-06-15 16:37:48.000000 acore_server_metadata-0.5.1/acore_server_metadata/tests/__init__.py
--rw-r--r--   0 sanhehu    (501) staff       (20)      447 2023-06-15 16:37:48.000000 acore_server_metadata-0.5.1/acore_server_metadata/tests/helper.py
--rw-r--r--   0 sanhehu    (501) staff       (20)     2169 2023-06-16 01:30:10.000000 acore_server_metadata-0.5.1/acore_server_metadata/tests/mock_aws.py
--rw-r--r--   0 sanhehu    (501) staff       (20)      479 2023-06-22 15:28:39.000000 acore_server_metadata-0.5.1/acore_server_metadata/utils.py
-drwxr-xr-x   0 sanhehu    (501) staff       (20)        0 2023-06-22 16:35:01.213645 acore_server_metadata-0.5.1/acore_server_metadata/vendor/
--rw-r--r--   0 sanhehu    (501) staff       (20)       25 2023-06-15 16:37:48.000000 acore_server_metadata-0.5.1/acore_server_metadata/vendor/__init__.py
--rw-r--r--   0 sanhehu    (501) staff       (20)     7553 2023-06-19 14:26:47.000000 acore_server_metadata-0.5.1/acore_server_metadata/vendor/hashes.py
--rw-r--r--   0 sanhehu    (501) staff       (20)     3572 2023-06-15 16:37:48.000000 acore_server_metadata-0.5.1/acore_server_metadata/vendor/pytest_cov_helper.py
-drwxr-xr-x   0 sanhehu    (501) staff       (20)        0 2023-06-22 16:35:01.210288 acore_server_metadata-0.5.1/acore_server_metadata.egg-info/
--rw-r--r--   0 sanhehu    (501) staff       (20)     7028 2023-06-22 16:35:01.000000 acore_server_metadata-0.5.1/acore_server_metadata.egg-info/PKG-INFO
--rw-r--r--   0 sanhehu    (501) staff       (20)     1187 2023-06-22 16:35:01.000000 acore_server_metadata-0.5.1/acore_server_metadata.egg-info/SOURCES.txt
--rw-r--r--   0 sanhehu    (501) staff       (20)        1 2023-06-22 16:35:01.000000 acore_server_metadata-0.5.1/acore_server_metadata.egg-info/dependency_links.txt
--rw-r--r--   0 sanhehu    (501) staff       (20)      242 2023-06-22 16:35:01.000000 acore_server_metadata-0.5.1/acore_server_metadata.egg-info/requires.txt
--rw-r--r--   0 sanhehu    (501) staff       (20)       22 2023-06-22 16:35:01.000000 acore_server_metadata-0.5.1/acore_server_metadata.egg-info/top_level.txt
--rw-r--r--   0 sanhehu    (501) staff       (20)     4218 2023-06-22 16:21:54.000000 acore_server_metadata-0.5.1/release-history.rst
--rw-r--r--   0 sanhehu    (501) staff       (20)      102 2023-06-15 16:37:48.000000 acore_server_metadata-0.5.1/requirements-automation.txt
--rw-r--r--   0 sanhehu    (501) staff       (20)      353 2023-06-15 16:37:48.000000 acore_server_metadata-0.5.1/requirements-dev.txt
--rw-r--r--   0 sanhehu    (501) staff       (20)      563 2023-06-15 16:37:48.000000 acore_server_metadata-0.5.1/requirements-doc.txt
--rw-r--r--   0 sanhehu    (501) staff       (20)      228 2023-06-16 01:31:27.000000 acore_server_metadata-0.5.1/requirements-test.txt
--rw-r--r--   0 sanhehu    (501) staff       (20)       88 2023-06-19 18:46:02.000000 acore_server_metadata-0.5.1/requirements.txt
--rw-r--r--   0 sanhehu    (501) staff       (20)       38 2023-06-22 16:35:01.214916 acore_server_metadata-0.5.1/setup.cfg
--rw-r--r--   0 sanhehu    (501) staff       (20)     7570 2023-06-15 16:37:48.000000 acore_server_metadata-0.5.1/setup.py
-drwxr-xr-x   0 sanhehu    (501) staff       (20)        0 2023-06-22 16:35:01.214314 acore_server_metadata-0.5.1/tests/
--rw-r--r--   0 sanhehu    (501) staff       (20)     1157 2023-06-19 18:53:48.000000 acore_server_metadata-0.5.1/tests/test_api.py
--rw-r--r--   0 sanhehu    (501) staff       (20)     8010 2023-06-22 16:18:04.000000 acore_server_metadata-0.5.1/tests/test_server.py
--rw-r--r--   0 sanhehu    (501) staff       (20)      923 2023-06-22 15:33:22.000000 acore_server_metadata-0.5.1/tests/test_utils.py
+drwxr-xr-x   0 sanhehu    (501) staff       (20)        0 2023-06-26 05:28:01.087415 acore_server_metadata-0.5.2/
+-rw-r--r--   0 sanhehu    (501) staff       (20)      670 2023-06-15 16:37:48.000000 acore_server_metadata-0.5.2/AUTHORS.rst
+-rw-r--r--   0 sanhehu    (501) staff       (20)     1132 2023-06-15 16:37:48.000000 acore_server_metadata-0.5.2/LICENSE.txt
+-rw-r--r--   0 sanhehu    (501) staff       (20)      329 2023-06-15 16:37:48.000000 acore_server_metadata-0.5.2/MANIFEST.in
+-rw-r--r--   0 sanhehu    (501) staff       (20)     7052 2023-06-26 05:28:01.087251 acore_server_metadata-0.5.2/PKG-INFO
+-rw-r--r--   0 sanhehu    (501) staff       (20)     5903 2023-06-26 05:13:50.000000 acore_server_metadata-0.5.2/README.rst
+drwxr-xr-x   0 sanhehu    (501) staff       (20)        0 2023-06-26 05:28:01.081349 acore_server_metadata-0.5.2/acore_server_metadata/
+-rw-r--r--   0 sanhehu    (501) staff       (20)      391 2023-06-16 02:28:42.000000 acore_server_metadata-0.5.2/acore_server_metadata/__init__.py
+-rw-r--r--   0 sanhehu    (501) staff       (20)       93 2023-06-26 05:13:00.000000 acore_server_metadata-0.5.2/acore_server_metadata/_version.py
+-rw-r--r--   0 sanhehu    (501) staff       (20)      105 2023-06-22 16:18:25.000000 acore_server_metadata-0.5.2/acore_server_metadata/api.py
+drwxr-xr-x   0 sanhehu    (501) staff       (20)        0 2023-06-26 05:28:01.082321 acore_server_metadata-0.5.2/acore_server_metadata/docs/
+-rw-r--r--   0 sanhehu    (501) staff       (20)       43 2023-06-15 16:37:48.000000 acore_server_metadata-0.5.2/acore_server_metadata/docs/__init__.py
+-rw-r--r--   0 sanhehu    (501) staff       (20)      496 2023-06-16 15:11:12.000000 acore_server_metadata-0.5.2/acore_server_metadata/exc.py
+-rw-r--r--   0 sanhehu    (501) staff       (20)      642 2023-06-15 16:37:48.000000 acore_server_metadata-0.5.2/acore_server_metadata/paths.py
+drwxr-xr-x   0 sanhehu    (501) staff       (20)        0 2023-06-26 05:28:01.083968 acore_server_metadata-0.5.2/acore_server_metadata/server/
+-rw-r--r--   0 sanhehu    (501) staff       (20)       25 2023-06-22 14:16:00.000000 acore_server_metadata-0.5.2/acore_server_metadata/server/__init__.py
+-rw-r--r--   0 sanhehu    (501) staff       (20)      171 2023-06-22 15:54:39.000000 acore_server_metadata-0.5.2/acore_server_metadata/server/api.py
+-rw-r--r--   0 sanhehu    (501) staff       (20)    12104 2023-06-26 05:15:51.000000 acore_server_metadata-0.5.2/acore_server_metadata/server/server.py
+-rw-r--r--   0 sanhehu    (501) staff       (20)    17223 2023-06-26 05:15:47.000000 acore_server_metadata-0.5.2/acore_server_metadata/server/server_operation.py
+-rw-r--r--   0 sanhehu    (501) staff       (20)     1665 2023-06-22 15:56:21.000000 acore_server_metadata-0.5.2/acore_server_metadata/server/server_status.py
+-rw-r--r--   0 sanhehu    (501) staff       (20)      270 2023-06-26 05:12:13.000000 acore_server_metadata-0.5.2/acore_server_metadata/settings.py
+drwxr-xr-x   0 sanhehu    (501) staff       (20)        0 2023-06-26 05:28:01.084709 acore_server_metadata-0.5.2/acore_server_metadata/tests/
+-rw-r--r--   0 sanhehu    (501) staff       (20)       58 2023-06-15 16:37:48.000000 acore_server_metadata-0.5.2/acore_server_metadata/tests/__init__.py
+-rw-r--r--   0 sanhehu    (501) staff       (20)      447 2023-06-15 16:37:48.000000 acore_server_metadata-0.5.2/acore_server_metadata/tests/helper.py
+-rw-r--r--   0 sanhehu    (501) staff       (20)     2169 2023-06-16 01:30:10.000000 acore_server_metadata-0.5.2/acore_server_metadata/tests/mock_aws.py
+-rw-r--r--   0 sanhehu    (501) staff       (20)      479 2023-06-22 15:28:39.000000 acore_server_metadata-0.5.2/acore_server_metadata/utils.py
+drwxr-xr-x   0 sanhehu    (501) staff       (20)        0 2023-06-26 05:28:01.085964 acore_server_metadata-0.5.2/acore_server_metadata/vendor/
+-rw-r--r--   0 sanhehu    (501) staff       (20)       25 2023-06-15 16:37:48.000000 acore_server_metadata-0.5.2/acore_server_metadata/vendor/__init__.py
+-rw-r--r--   0 sanhehu    (501) staff       (20)     7553 2023-06-19 14:26:47.000000 acore_server_metadata-0.5.2/acore_server_metadata/vendor/hashes.py
+-rw-r--r--   0 sanhehu    (501) staff       (20)     3572 2023-06-15 16:37:48.000000 acore_server_metadata-0.5.2/acore_server_metadata/vendor/pytest_cov_helper.py
+drwxr-xr-x   0 sanhehu    (501) staff       (20)        0 2023-06-26 05:28:01.082191 acore_server_metadata-0.5.2/acore_server_metadata.egg-info/
+-rw-r--r--   0 sanhehu    (501) staff       (20)     7052 2023-06-26 05:28:01.000000 acore_server_metadata-0.5.2/acore_server_metadata.egg-info/PKG-INFO
+-rw-r--r--   0 sanhehu    (501) staff       (20)     1187 2023-06-26 05:28:01.000000 acore_server_metadata-0.5.2/acore_server_metadata.egg-info/SOURCES.txt
+-rw-r--r--   0 sanhehu    (501) staff       (20)        1 2023-06-26 05:28:01.000000 acore_server_metadata-0.5.2/acore_server_metadata.egg-info/dependency_links.txt
+-rw-r--r--   0 sanhehu    (501) staff       (20)      272 2023-06-26 05:28:01.000000 acore_server_metadata-0.5.2/acore_server_metadata.egg-info/requires.txt
+-rw-r--r--   0 sanhehu    (501) staff       (20)       22 2023-06-26 05:28:01.000000 acore_server_metadata-0.5.2/acore_server_metadata.egg-info/top_level.txt
+-rw-r--r--   0 sanhehu    (501) staff       (20)     4747 2023-06-26 05:15:20.000000 acore_server_metadata-0.5.2/release-history.rst
+-rw-r--r--   0 sanhehu    (501) staff       (20)      102 2023-06-15 16:37:48.000000 acore_server_metadata-0.5.2/requirements-automation.txt
+-rw-r--r--   0 sanhehu    (501) staff       (20)      353 2023-06-15 16:37:48.000000 acore_server_metadata-0.5.2/requirements-dev.txt
+-rw-r--r--   0 sanhehu    (501) staff       (20)      563 2023-06-15 16:37:48.000000 acore_server_metadata-0.5.2/requirements-doc.txt
+-rw-r--r--   0 sanhehu    (501) staff       (20)      228 2023-06-16 01:31:27.000000 acore_server_metadata-0.5.2/requirements-test.txt
+-rw-r--r--   0 sanhehu    (501) staff       (20)      118 2023-06-26 05:08:10.000000 acore_server_metadata-0.5.2/requirements.txt
+-rw-r--r--   0 sanhehu    (501) staff       (20)       38 2023-06-26 05:28:01.087469 acore_server_metadata-0.5.2/setup.cfg
+-rw-r--r--   0 sanhehu    (501) staff       (20)     7570 2023-06-15 16:37:48.000000 acore_server_metadata-0.5.2/setup.py
+drwxr-xr-x   0 sanhehu    (501) staff       (20)        0 2023-06-26 05:28:01.086785 acore_server_metadata-0.5.2/tests/
+-rw-r--r--   0 sanhehu    (501) staff       (20)     1157 2023-06-19 18:53:48.000000 acore_server_metadata-0.5.2/tests/test_api.py
+-rw-r--r--   0 sanhehu    (501) staff       (20)     8043 2023-06-26 05:11:16.000000 acore_server_metadata-0.5.2/tests/test_server.py
+-rw-r--r--   0 sanhehu    (501) staff       (20)      923 2023-06-22 15:33:22.000000 acore_server_metadata-0.5.2/tests/test_utils.py
```

### Comparing `acore_server_metadata-0.5.1/AUTHORS.rst` & `acore_server_metadata-0.5.2/AUTHORS.rst`

 * *Files identical despite different names*

### Comparing `acore_server_metadata-0.5.1/LICENSE.txt` & `acore_server_metadata-0.5.2/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `acore_server_metadata-0.5.1/PKG-INFO` & `acore_server_metadata-0.5.2/acore_server_metadata.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 Metadata-Version: 2.1
-Name: acore_server_metadata
-Version: 0.5.1
+Name: acore-server-metadata
+Version: 0.5.2
 Summary: Azerothcore WOW server metadata for Fleet management.
 Home-page: https://github.com/MacHu-GWU/acore_server_metadata-project
-Download-URL: https://pypi.python.org/pypi/acore_server_metadata/0.5.1#downloads
+Download-URL: https://pypi.python.org/pypi/acore_server_metadata/0.5.2#downloads
 Author: Sanhe Hu
 Author-email: husanhe@gmail.com
 Maintainer: Sanhe Hu
 Maintainer-email: husanhe@gmail.com
 License: MIT
 Platform: Windows
 Platform: MacOS
@@ -104,21 +104,21 @@
     >>> server
     Server(
         id='prod-1',
         ec2_inst=Ec2Instance(
             id='i-1a2b3c4d',
             status='running',
             ...
-            tags={'realm': 'prod'},
+            tags={'wserver:server_id': 'prod'},
             data=...
         ),
         rds_inst=RDSDBInstance(
             id='db-inst-1',
             status='available',
-            tags={'realm': 'prod'},
+            tags={'wserver:server_id': 'prod'},
             data=...
         ),
     )
 
     # 检查服务器的状态
     >>> server.is_exists()
     >>> server.is_running()
```

### Comparing `acore_server_metadata-0.5.1/README.rst` & `acore_server_metadata-0.5.2/README.rst`

 * *Files 2% similar despite different names*

```diff
@@ -72,21 +72,21 @@
     >>> server
     Server(
         id='prod-1',
         ec2_inst=Ec2Instance(
             id='i-1a2b3c4d',
             status='running',
             ...
-            tags={'realm': 'prod'},
+            tags={'wserver:server_id': 'prod'},
             data=...
         ),
         rds_inst=RDSDBInstance(
             id='db-inst-1',
             status='available',
-            tags={'realm': 'prod'},
+            tags={'wserver:server_id': 'prod'},
             data=...
         ),
     )
 
     # 检查服务器的状态
     >>> server.is_exists()
     >>> server.is_running()
```

### Comparing `acore_server_metadata-0.5.1/acore_server_metadata/paths.py` & `acore_server_metadata-0.5.2/acore_server_metadata/paths.py`

 * *Files identical despite different names*

### Comparing `acore_server_metadata-0.5.1/acore_server_metadata/server/server.py` & `acore_server_metadata-0.5.2/acore_server_metadata/server/server.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,23 +1,20 @@
 # -*- coding: utf-8 -*-
 
 import typing as T
 import dataclasses
 
 from simple_aws_ec2.api import Ec2Instance, EC2InstanceStatusEnum
 from simple_aws_rds.api import RDSDBInstance, RDSDBInstanceStatusEnum
+from acore_constants.api import TagKey
 
 from ..utils import group_by
-from ..vendor.hashes import hashes
 from ..exc import (
-    ServerNotFoundError,
     ServerNotUniqueError,
-    ServerAlreadyExistsError,
 )
-from ..settings import settings
 
 from .server_status import ServerStatusMixin
 from .server_operation import ServerOperationMixin
 
 
 @dataclasses.dataclass
 class BaseServer:
@@ -103,15 +100,15 @@
         """
         内部方法, 根据指定 server_id 列表, 批量获得获得所有包含该 Tag 的 EC2 实例.
         常用于用 Batch 的方式批量获得信息, 以减少 API 调用次数.
         """
         return Ec2Instance.query(
             ec2_client=ec2_client,
             filters=[
-                dict(Name=f"tag:{settings.ID_TAG_KEY}", Values=ids),
+                dict(Name=f"tag:{TagKey.SERVER_ID}", Values=ids),
                 # we don't count terminated instances as existing
                 dict(
                     Name="instance-state-name",
                     Values=[
                         EC2InstanceStatusEnum.pending.value,
                         EC2InstanceStatusEnum.running.value,
                         EC2InstanceStatusEnum.stopping.value,
@@ -145,15 +142,15 @@
                         RDSDBInstanceStatusEnum.deleting.value,
                         RDSDBInstanceStatusEnum.failed.value,
                         RDSDBInstanceStatusEnum.restore_error.value,
                     ]
                 )
                 and (
                     rds_inst.tags.get(
-                        settings.ID_TAG_KEY,
+                        TagKey.SERVER_ID,
                         "THIS_IS_IMPOSSIBLE_TO_MATCH",
                     )
                     in ids
                 )
             )
         ]
 
@@ -278,18 +275,18 @@
         """
         # batch get data
         ec2_inst_list = cls._get_existing_ec2(ec2_client=ec2_client, ids=ids)
         rds_inst_list = cls._get_existing_rds(rds_client=rds_client, ids=ids)
 
         # group by server id
         ec2_inst_mapper = group_by(
-            ec2_inst_list, key=lambda inst: inst.tags[settings.ID_TAG_KEY]
+            ec2_inst_list, key=lambda inst: inst.tags[TagKey.SERVER_ID]
         )
         rds_inst_mapper = group_by(
-            rds_inst_list, key=lambda inst: inst.tags[settings.ID_TAG_KEY]
+            rds_inst_list, key=lambda inst: inst.tags[TagKey.SERVER_ID]
         )
 
         # merge data
         def get_inst(key: str, mapper: T.Dict[str, list]):
             if key not in mapper:
                 return None
             items = mapper[key]
```

### Comparing `acore_server_metadata-0.5.1/acore_server_metadata/server/server_operation.py` & `acore_server_metadata-0.5.2/acore_server_metadata/server/server_operation.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,18 +1,19 @@
 # -*- coding: utf-8 -*-
 
 import typing as T
 from datetime import timezone
 
+from acore_constants.api import TagKey
+
 from ..utils import get_utc_now
 from ..exc import (
     ServerNotFoundError,
     ServerAlreadyExistsError,
 )
-from ..settings import settings
 from ..vendor.hashes import hashes
 
 if T.TYPE_CHECKING:  # pragma: no cover
     from .server import Server
     from mypy_boto3_ec2 import EC2Client
     from mypy_boto3_rds import RDSClient
 
@@ -75,15 +76,15 @@
             if ec2_inst is not None:  # pragma: no cover
                 raise ServerAlreadyExistsError(
                     f"EC2 instance {self.id!r} already exists"
                 )
         if tags is None:
             tags = dict()
         tags["Name"] = self.id
-        tags[settings.ID_TAG_KEY] = self.id  # the realm tag indicator has to match
+        tags[TagKey.SERVER_ID] = self.id  # the realm tag indicator has to match
         tags["tech:machine_creator"] = "acore_server_metadata"
         return ec2_client.run_instances(
             ImageId=ami_id,
             InstanceType=instance_type,
             # only launch one instance for each realm
             MinCount=1,
             MaxCount=1,
@@ -143,15 +144,15 @@
             rds_inst = self.get_rds(rds_client, id=self.id)
             if rds_inst is not None:  # pragma: no cover
                 raise ServerAlreadyExistsError(
                     f"RDS DB instance {self.id!r} already exists"
                 )
         if tags is None:
             tags = dict()
-        tags[settings.ID_TAG_KEY] = self.id
+        tags[TagKey.SERVER_ID] = self.id
         tags["tech:machine_creator"] = "acore_server_metadata"
 
         res = rds_client.describe_db_snapshots(
             DBSnapshotIdentifier=db_snapshot_identifier,
         )
         db_snapshot_list = res.get("DBSnapshots", [])
         if len(db_snapshot_list):
@@ -372,15 +373,15 @@
             rds_inst = self.rds_inst
 
         snapshot_id = self._get_db_snapshot_id()
         return rds_client.create_db_snapshot(
             DBSnapshotIdentifier=snapshot_id,
             DBInstanceIdentifier=rds_inst.id,
             Tags=[
-                dict(Key=settings.ID_TAG_KEY, Value=rds_inst.id),
+                dict(Key=TagKey.SERVER_ID, Value=rds_inst.id),
                 dict(Key="tech:machine_creator", Value="acore_server_metadata"),
             ],
         )
 
     def cleanup_db_snapshot(
         self: "Server",
         rds_client: "RDSClient",
```

### Comparing `acore_server_metadata-0.5.1/acore_server_metadata/server/server_status.py` & `acore_server_metadata-0.5.2/acore_server_metadata/server/server_status.py`

 * *Files identical despite different names*

### Comparing `acore_server_metadata-0.5.1/acore_server_metadata/tests/mock_aws.py` & `acore_server_metadata-0.5.2/acore_server_metadata/tests/mock_aws.py`

 * *Files identical despite different names*

### Comparing `acore_server_metadata-0.5.1/acore_server_metadata/vendor/hashes.py` & `acore_server_metadata-0.5.2/acore_server_metadata/vendor/hashes.py`

 * *Files identical despite different names*

### Comparing `acore_server_metadata-0.5.1/acore_server_metadata/vendor/pytest_cov_helper.py` & `acore_server_metadata-0.5.2/acore_server_metadata/vendor/pytest_cov_helper.py`

 * *Files identical despite different names*

### Comparing `acore_server_metadata-0.5.1/acore_server_metadata.egg-info/PKG-INFO` & `acore_server_metadata-0.5.2/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 Metadata-Version: 2.1
-Name: acore-server-metadata
-Version: 0.5.1
+Name: acore_server_metadata
+Version: 0.5.2
 Summary: Azerothcore WOW server metadata for Fleet management.
 Home-page: https://github.com/MacHu-GWU/acore_server_metadata-project
-Download-URL: https://pypi.python.org/pypi/acore_server_metadata/0.5.1#downloads
+Download-URL: https://pypi.python.org/pypi/acore_server_metadata/0.5.2#downloads
 Author: Sanhe Hu
 Author-email: husanhe@gmail.com
 Maintainer: Sanhe Hu
 Maintainer-email: husanhe@gmail.com
 License: MIT
 Platform: Windows
 Platform: MacOS
@@ -104,21 +104,21 @@
     >>> server
     Server(
         id='prod-1',
         ec2_inst=Ec2Instance(
             id='i-1a2b3c4d',
             status='running',
             ...
-            tags={'realm': 'prod'},
+            tags={'wserver:server_id': 'prod'},
             data=...
         ),
         rds_inst=RDSDBInstance(
             id='db-inst-1',
             status='available',
-            tags={'realm': 'prod'},
+            tags={'wserver:server_id': 'prod'},
             data=...
         ),
     )
 
     # 检查服务器的状态
     >>> server.is_exists()
     >>> server.is_running()
```

### Comparing `acore_server_metadata-0.5.1/acore_server_metadata.egg-info/SOURCES.txt` & `acore_server_metadata-0.5.2/acore_server_metadata.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `acore_server_metadata-0.5.1/release-history.rst` & `acore_server_metadata-0.5.2/release-history.rst`

 * *Files 7% similar despite different names*

```diff
@@ -11,14 +11,32 @@
 **Minor Improvements**
 
 **Bugfixes**
 
 **Miscellaneous**
 
 
+x.y.z (Backlog)
+~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~
+**Features and Improvements**
+
+**Minor Improvements**
+
+**Bugfixes**
+
+**Miscellaneous**
+
+
+0.5.2 (2023-06-26)
+~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~
+**Minor Improvements**
+
+- ``acore_server_metadata.settings`` module is not in used anymore. It is kept for backward compatibility. Now we use `acore_constants <https://github.com/MacHu-GWU/acore_constants-project>`_ library to define constants.
+
+
 0.5.1 (2023-06-22)
 ~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~
 **Features and Improvements**
 
 - Now the ``acore_server_metadata.api.Server.get_server()`` method will always return a ``Server`` object. If the ec2 or rds doesn't not exists, then the ``ec2_inst`` or ``rds_inst`` attribure of the ``Server`` object will be ``None``. This behavior was returning ``None`` before.
 - Similarly the ``acore_server_metadata.api.Server.batch_get_server()`` method will always return a ``Server`` object for specific id.
```

### Comparing `acore_server_metadata-0.5.1/requirements-doc.txt` & `acore_server_metadata-0.5.2/requirements-doc.txt`

 * *Files identical despite different names*

### Comparing `acore_server_metadata-0.5.1/setup.py` & `acore_server_metadata-0.5.2/setup.py`

 * *Files identical despite different names*

### Comparing `acore_server_metadata-0.5.1/tests/test_api.py` & `acore_server_metadata-0.5.2/tests/test_api.py`

 * *Files identical despite different names*

### Comparing `acore_server_metadata-0.5.1/tests/test_server.py` & `acore_server_metadata-0.5.2/tests/test_server.py`

 * *Files 2% similar despite different names*

```diff
@@ -3,14 +3,15 @@
 import typing as T
 import moto
 import time
 import pytest
 
 from simple_aws_ec2.api import Ec2Instance
 from simple_aws_rds.api import RDSDBInstance
+from acore_constants.api import TagKey
 
 from acore_server_metadata.tests.mock_aws import BaseMockTest
 from acore_server_metadata.settings import settings
 from acore_server_metadata.server.api import (
     Server,
     ServerNotUniqueError,
 )
@@ -49,15 +50,15 @@
             MinCount=1,
             MaxCount=1,
             ImageId=self.ami_id,
             TagSpecifications=[
                 {
                     "ResourceType": "instance",
                     "Tags": [
-                        {"Key": settings.ID_TAG_KEY, "Value": id},
+                        {"Key": TagKey.SERVER_ID, "Value": id},
                     ],
                 },
             ],
         )["Instances"][0]["InstanceId"]
         return ec2_id
 
     def launch_rds(self, id: str) -> str:
@@ -66,15 +67,15 @@
         :return: db  instance id
         """
         rds_id = self.rds_client.create_db_instance(
             DBInstanceIdentifier=id,
             DBInstanceClass="db.t2.micro",
             Engine="mysql",
             Tags=[
-                {"Key": settings.ID_TAG_KEY, "Value": id},
+                {"Key": TagKey.SERVER_ID, "Value": id},
             ],
         )["DBInstance"]["DBInstanceIdentifier"]
         return rds_id
 
     def delete_all_ec2(self):
         for ec2_inst in Ec2Instance.query(self.ec2_client):
             ec2_inst.terminate_instance(self.ec2_client)
```

### Comparing `acore_server_metadata-0.5.1/tests/test_utils.py` & `acore_server_metadata-0.5.2/tests/test_utils.py`

 * *Files identical despite different names*

