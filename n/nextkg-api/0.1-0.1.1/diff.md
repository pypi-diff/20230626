# Comparing `tmp/nextkg-api-0.1.tar.gz` & `tmp/nextkg-api-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nextkg-api-0.1.tar", last modified: Mon Aug 22 03:33:38 2022, max compression
+gzip compressed data, was "nextkg-api-0.1.1.tar", last modified: Sun Jun 25 23:28:53 2023, max compression
```

## Comparing `nextkg-api-0.1.tar` & `nextkg-api-0.1.1.tar`

### file list

```diff
@@ -1,22 +1,22 @@
-drwxr-xr-x   0 jadbin     (501) staff       (20)        0 2022-08-22 03:33:38.105712 nextkg-api-0.1/
--rw-r--r--   0 jadbin     (501) staff       (20)      109 2022-08-22 00:35:55.000000 nextkg-api-0.1/MANIFEST.in
--rw-r--r--   0 jadbin     (501) staff       (20)      186 2022-08-22 03:33:38.105389 nextkg-api-0.1/PKG-INFO
--rw-r--r--   0 jadbin     (501) staff       (20)       34 2022-08-22 03:33:35.000000 nextkg-api-0.1/README.rst
-drwxr-xr-x   0 jadbin     (501) staff       (20)        0 2022-08-22 03:33:38.101183 nextkg-api-0.1/nextkg_api/
--rw-r--r--   0 jadbin     (501) staff       (20)       20 2022-08-22 02:54:57.000000 nextkg-api-0.1/nextkg_api/__init__.py
--rw-r--r--   0 jadbin     (501) staff       (20)     6473 2022-08-22 03:08:32.000000 nextkg-api-0.1/nextkg_api/client.py
--rw-r--r--   0 jadbin     (501) staff       (20)      928 2022-08-22 03:00:44.000000 nextkg-api-0.1/nextkg_api/data_models.py
--rw-r--r--   0 jadbin     (501) staff       (20)     1361 2022-08-04 06:44:21.000000 nextkg-api-0.1/nextkg_api/utils.py
-drwxr-xr-x   0 jadbin     (501) staff       (20)        0 2022-08-22 03:33:38.103974 nextkg-api-0.1/nextkg_api.egg-info/
--rw-r--r--   0 jadbin     (501) staff       (20)      186 2022-08-22 03:33:38.000000 nextkg-api-0.1/nextkg_api.egg-info/PKG-INFO
--rw-r--r--   0 jadbin     (501) staff       (20)      363 2022-08-22 03:33:38.000000 nextkg-api-0.1/nextkg_api.egg-info/SOURCES.txt
--rw-r--r--   0 jadbin     (501) staff       (20)        1 2022-08-22 03:33:38.000000 nextkg-api-0.1/nextkg_api.egg-info/dependency_links.txt
--rw-r--r--   0 jadbin     (501) staff       (20)        1 2022-08-22 02:50:15.000000 nextkg-api-0.1/nextkg_api.egg-info/not-zip-safe
--rw-r--r--   0 jadbin     (501) staff       (20)       58 2022-08-22 03:33:38.000000 nextkg-api-0.1/nextkg_api.egg-info/requires.txt
--rw-r--r--   0 jadbin     (501) staff       (20)       11 2022-08-22 03:33:38.000000 nextkg-api-0.1/nextkg_api.egg-info/top_level.txt
-drwxr-xr-x   0 jadbin     (501) staff       (20)        0 2022-08-22 03:33:38.104318 nextkg-api-0.1/requirements/
--rw-r--r--   0 jadbin     (501) staff       (20)       32 2021-03-11 04:09:29.000000 nextkg-api-0.1/requirements/docs.txt
--rw-r--r--   0 jadbin     (501) staff       (20)       38 2022-08-22 03:33:38.105815 nextkg-api-0.1/setup.cfg
--rw-r--r--   0 jadbin     (501) staff       (20)     1040 2022-08-22 00:36:53.000000 nextkg-api-0.1/setup.py
-drwxr-xr-x   0 jadbin     (501) staff       (20)        0 2022-08-22 03:33:38.105053 nextkg-api-0.1/tests/
--rw-r--r--   0 jadbin     (501) staff       (20)        0 2021-03-12 10:28:04.000000 nextkg-api-0.1/tests/__init__.py
+drwxrwxrwx   0 root         (0) root         (0)        0 2023-06-25 23:28:53.474034 nextkg-api-0.1.1/
+-rwxrwxrwx   0 root         (0) root         (0)      109 2023-06-20 00:40:36.000000 nextkg-api-0.1.1/MANIFEST.in
+-rwxrwxrwx   0 root         (0) root         (0)      132 2023-06-25 23:28:53.474034 nextkg-api-0.1.1/PKG-INFO
+-rwxrwxrwx   0 root         (0) root         (0)       34 2023-06-20 00:40:36.000000 nextkg-api-0.1.1/README.rst
+drwxrwxrwx   0 root         (0) root         (0)        0 2023-06-25 23:28:53.207984 nextkg-api-0.1.1/nextkg_api/
+-rwxrwxrwx   0 root         (0) root         (0)       22 2023-06-25 23:28:10.000000 nextkg-api-0.1.1/nextkg_api/__init__.py
+-rwxrwxrwx   0 root         (0) root         (0)     6579 2023-06-20 02:40:07.000000 nextkg-api-0.1.1/nextkg_api/client.py
+-rwxrwxrwx   0 root         (0) root         (0)      981 2023-06-20 02:34:09.000000 nextkg-api-0.1.1/nextkg_api/data_models.py
+-rwxrwxrwx   0 root         (0) root         (0)     1361 2023-06-20 00:40:36.000000 nextkg-api-0.1.1/nextkg_api/utils.py
+drwxrwxrwx   0 root         (0) root         (0)        0 2023-06-25 23:28:53.379851 nextkg-api-0.1.1/nextkg_api.egg-info/
+-rwxrwxrwx   0 root         (0) root         (0)      132 2023-06-25 23:28:52.000000 nextkg-api-0.1.1/nextkg_api.egg-info/PKG-INFO
+-rwxrwxrwx   0 root         (0) root         (0)      363 2023-06-25 23:28:53.000000 nextkg-api-0.1.1/nextkg_api.egg-info/SOURCES.txt
+-rwxrwxrwx   0 root         (0) root         (0)        1 2023-06-25 23:28:52.000000 nextkg-api-0.1.1/nextkg_api.egg-info/dependency_links.txt
+-rwxrwxrwx   0 root         (0) root         (0)        1 2023-06-25 23:28:52.000000 nextkg-api-0.1.1/nextkg_api.egg-info/not-zip-safe
+-rwxrwxrwx   0 root         (0) root         (0)       33 2023-06-25 23:28:52.000000 nextkg-api-0.1.1/nextkg_api.egg-info/requires.txt
+-rwxrwxrwx   0 root         (0) root         (0)       11 2023-06-25 23:28:52.000000 nextkg-api-0.1.1/nextkg_api.egg-info/top_level.txt
+drwxrwxrwx   0 root         (0) root         (0)        0 2023-06-25 23:28:53.411508 nextkg-api-0.1.1/requirements/
+-rwxrwxrwx   0 root         (0) root         (0)       32 2023-06-20 00:40:36.000000 nextkg-api-0.1.1/requirements/docs.txt
+-rwxrwxrwx   0 root         (0) root         (0)       38 2023-06-25 23:28:53.474034 nextkg-api-0.1.1/setup.cfg
+-rwxrwxrwx   0 root         (0) root         (0)     1008 2023-06-20 01:47:19.000000 nextkg-api-0.1.1/setup.py
+drwxrwxrwx   0 root         (0) root         (0)        0 2023-06-25 23:28:53.442844 nextkg-api-0.1.1/tests/
+-rwxrwxrwx   0 root         (0) root         (0)        0 2023-06-20 00:40:36.000000 nextkg-api-0.1.1/tests/__init__.py
```

### Comparing `nextkg-api-0.1/nextkg_api/client.py` & `nextkg-api-0.1.1/nextkg_api/client.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,30 +1,30 @@
 import json
 from typing import List, Union, Tuple, Optional
 
-from requests_toolbelt.sessions import BaseUrlSession
+import requests
 
 from nextkg_api.data_models import Entity, Neighbor
 
 
 class NextKGClient:
     def __init__(self, host: str, kg_id: str):
         if '://' not in host:
             endpoint = f'http://{host}'
         else:
             endpoint = host
         if not endpoint.endswith('/'):
             endpoint += '/'
         self.endpoint = endpoint
-        self.session = BaseUrlSession(endpoint)
+        self.session = requests.Session()
         self.kg_id = kg_id
 
     def ping(self, raise_error=False) -> bool:
         try:
-            resp = self.session.get('/health')
+            resp = self.session.get(f'{self.endpoint}health')
             resp.raise_for_status()
         except Exception:
             if raise_error:
                 raise
             return False
         return True
 
@@ -35,15 +35,15 @@
         :param entity:
         :param strict:
         :return:
         """
         if isinstance(entity, Entity):
             entity = json.loads(entity.json())
         resp = self.session.post(
-            '/api/entities/link',
+            f'{self.endpoint}api/entities/link',
             json=dict(
                 entity=entity,
                 strict=strict,
             ),
             params=dict(
                 kg_id=self.kg_id,
             )
@@ -60,15 +60,15 @@
         :param entity:
         :param refresh:
         :return:
         """
         if isinstance(entity, Entity):
             entity = json.loads(entity.json())
         resp = self.session.put(
-            f'/api/entities/{entity_id}',
+            f'{self.endpoint}api/entities/{entity_id}',
             json=dict(
                 entity=entity,
                 refresh=refresh,
             ),
             params=dict(
                 kg_id=self.kg_id,
                 entity_id=entity_id,
@@ -87,15 +87,15 @@
         :param refresh:
         :return:
         """
 
         if isinstance(entity, Entity):
             entity = json.loads(entity.json())
         resp = self.session.post(
-            f'/api/entities/{entity_id}/update',
+            f'{self.endpoint}api/entities/{entity_id}/update',
             json=dict(
                 entity=entity,
                 refresh=refresh,
             ),
             params=dict(
                 kg_id=self.kg_id,
                 entity_id=entity_id,
@@ -110,15 +110,15 @@
         根据id获取实体
 
         :param entity_id:
         :return:
         """
 
         resp = self.session.get(
-            f'/api/entities/{entity_id}',
+            f'{self.endpoint}api/entities/{entity_id}',
             params=dict(
                 kg_id=self.kg_id,
                 entity_id=entity_id,
             )
         )
         if resp.status_code == 404:
             return
@@ -156,15 +156,15 @@
         :param refresh:
         :return:
         """
 
         if isinstance(entity, Entity):
             entity = json.loads(entity.json())
         resp = self.session.post(
-            '/api/entities',
+            f'{self.endpoint}api/entities',
             json=dict(
                 entity=entity,
                 refresh=refresh,
             ),
             params=dict(
                 kg_id=self.kg_id,
             )
@@ -180,15 +180,15 @@
         :param start_entity_id:
         :param end_entity_id:
         :param relation_type:
         :return:
         """
 
         resp = self.session.post(
-            '/api/relations',
+            f'{self.endpoint}api/relations',
             json=dict(
                 start_entity_id=start_entity_id,
                 end_entity_id=end_entity_id,
                 relation_type=relation_type,
             ),
             params=dict(
                 kg_id=self.kg_id,
@@ -201,42 +201,42 @@
         获取邻居
 
         :param entity_id:
         :return:
         """
 
         resp = self.session.post(
-            '/api/entities/find-neighbors',
+            f'{self.endpoint}api/entities/find-neighbors',
             params=dict(
                 kg_id=self.kg_id,
                 entity_id=entity_id,
             )
         )
         resp.raise_for_status()
         data = resp.json()['data']
         children = [Neighbor(**i) for i in data['children']]
         parents = [Neighbor(**i) for i in data['parents']]
         return children, parents
 
-    def _search_by_dsl(self, **params):
+    def _search_by_dsl(self, **params) -> List[Entity]:
         resp = self.session.post(
-            '/api/entities/search/by-dsl',
+            f'{self.endpoint}api/entities/search/by-dsl',
             params=dict(
                 kg_id=self.kg_id,
             ),
             json=dict(
                 params=params,
             )
         )
         resp.raise_for_status()
         data = resp.json()['data']
         return [Entity(**d) for d in data]
 
     def remove_entity(self, entity_id: str, refresh: bool = False):
         resp = self.session.delete(
-            f'/api/entities/{entity_id}',
+            f'{self.endpoint}api/entities/{entity_id}',
             params=dict(
                 kg_id=self.kg_id,
-                refresh=1 if refresh else 0,
+                refresh=refresh,
             )
         )
         resp.raise_for_status()
```

### Comparing `nextkg-api-0.1/nextkg_api/data_models.py` & `nextkg-api-0.1.1/nextkg_api/data_models.py`

 * *Files 5% similar despite different names*

```diff
@@ -8,27 +8,28 @@
     name: str
     value: Any = None
     json_value: Union[str, List[str]] = None
 
 
 class EntityMeta(BaseModel):
     pv: int = None
-    ts: dt.datetime = None
     origin_id: str = None
     md5: str = None
     edit_user: str = None
     audit_user: str = None
     domain: Union[str, List[str]] = None
+    operation_domain: Union[str, List[str]] = None
 
 
 class Entity(BaseModel):
     id: str = None
     entity_name: str
     entity_type: str = None
     entity_tags: Union[str, List[str]] = None
+    entity_title: str = None
     properties: List[Property] = None
     create_time: dt.datetime = None
     meta: EntityMeta = None
     version: str = None
 
 
 class PartialEntity(Entity):
```

### Comparing `nextkg-api-0.1/nextkg_api/utils.py` & `nextkg-api-0.1.1/nextkg_api/utils.py`

 * *Files identical despite different names*

### Comparing `nextkg-api-0.1/setup.py` & `nextkg-api-0.1.1/setup.py`

 * *Files 6% similar despite different names*

```diff
@@ -14,15 +14,14 @@
         return re.search(r"__version__ = '([^']+)'", f.read()).group(1)
 
 
 version = read_version()
 
 install_requires = [
     'requests>=2.25.1',
-    'requests-toolbelt>=0.9.1',
     'pydantic>=1.8.1',
 ]
 
 
 def main():
     if sys.version_info < (3, 6):
         raise RuntimeError('The minimal supported Python version is 3.6')
```

