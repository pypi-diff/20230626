# Comparing `tmp/octodns-dnsmadeeasy-0.0.2.tar.gz` & `tmp/octodns-dnsmadeeasy-0.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "octodns-dnsmadeeasy-0.0.2.tar", last modified: Wed Mar 29 20:09:52 2023, max compression
+gzip compressed data, was "octodns-dnsmadeeasy-0.0.3.tar", last modified: Mon Jun 26 17:53:59 2023, max compression
```

## Comparing `octodns-dnsmadeeasy-0.0.2.tar` & `octodns-dnsmadeeasy-0.0.3.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxr-xr-x   0 ross       (501) staff       (20)        0 2023-03-29 20:09:52.775184 octodns-dnsmadeeasy-0.0.2/
--rw-r--r--   0 ross       (501) staff       (20)     2193 2023-03-29 20:09:52.774795 octodns-dnsmadeeasy-0.0.2/PKG-INFO
--rw-r--r--   0 ross       (501) staff       (20)     1854 2022-10-26 15:20:10.000000 octodns-dnsmadeeasy-0.0.2/README.md
-drwxr-xr-x   0 ross       (501) staff       (20)        0 2023-03-29 20:09:52.771776 octodns-dnsmadeeasy-0.0.2/octodns_dnsmadeeasy/
--rw-r--r--   0 ross       (501) staff       (20)    13404 2023-03-29 20:09:38.000000 octodns-dnsmadeeasy-0.0.2/octodns_dnsmadeeasy/__init__.py
-drwxr-xr-x   0 ross       (501) staff       (20)        0 2023-03-29 20:09:52.773505 octodns-dnsmadeeasy-0.0.2/octodns_dnsmadeeasy.egg-info/
--rw-r--r--   0 ross       (501) staff       (20)     2193 2023-03-29 20:09:52.000000 octodns-dnsmadeeasy-0.0.2/octodns_dnsmadeeasy.egg-info/PKG-INFO
--rw-r--r--   0 ross       (501) staff       (20)      322 2023-03-29 20:09:52.000000 octodns-dnsmadeeasy-0.0.2/octodns_dnsmadeeasy.egg-info/SOURCES.txt
--rw-r--r--   0 ross       (501) staff       (20)        1 2023-03-29 20:09:52.000000 octodns-dnsmadeeasy-0.0.2/octodns_dnsmadeeasy.egg-info/dependency_links.txt
--rw-r--r--   0 ross       (501) staff       (20)      238 2023-03-29 20:09:52.000000 octodns-dnsmadeeasy-0.0.2/octodns_dnsmadeeasy.egg-info/requires.txt
--rw-r--r--   0 ross       (501) staff       (20)       20 2023-03-29 20:09:52.000000 octodns-dnsmadeeasy-0.0.2/octodns_dnsmadeeasy.egg-info/top_level.txt
--rw-r--r--   0 ross       (501) staff       (20)      312 2023-02-04 19:18:43.000000 octodns-dnsmadeeasy-0.0.2/pyproject.toml
--rw-r--r--   0 ross       (501) staff       (20)       38 2023-03-29 20:09:52.775285 octodns-dnsmadeeasy-0.0.2/setup.cfg
--rw-r--r--   0 ross       (501) staff       (20)     1830 2023-02-04 19:18:43.000000 octodns-dnsmadeeasy-0.0.2/setup.py
-drwxr-xr-x   0 ross       (501) staff       (20)        0 2023-03-29 20:09:52.773898 octodns-dnsmadeeasy-0.0.2/tests/
--rw-r--r--   0 ross       (501) staff       (20)     8831 2023-02-04 19:18:43.000000 octodns-dnsmadeeasy-0.0.2/tests/test_octodns_provider_dnsmadeeasy.py
+drwxr-xr-x   0 yzguy      (501) staff       (20)        0 2023-06-26 17:53:59.284079 octodns-dnsmadeeasy-0.0.3/
+-rw-r--r--   0 yzguy      (501) staff       (20)     2193 2023-06-26 17:53:59.283924 octodns-dnsmadeeasy-0.0.3/PKG-INFO
+-rw-r--r--   0 yzguy      (501) staff       (20)     1854 2023-06-22 18:01:26.000000 octodns-dnsmadeeasy-0.0.3/README.md
+drwxr-xr-x   0 yzguy      (501) staff       (20)        0 2023-06-26 17:53:59.282984 octodns-dnsmadeeasy-0.0.3/octodns_dnsmadeeasy/
+-rw-r--r--   0 yzguy      (501) staff       (20)    14740 2023-06-26 17:47:00.000000 octodns-dnsmadeeasy-0.0.3/octodns_dnsmadeeasy/__init__.py
+drwxr-xr-x   0 yzguy      (501) staff       (20)        0 2023-06-26 17:53:59.283503 octodns-dnsmadeeasy-0.0.3/octodns_dnsmadeeasy.egg-info/
+-rw-r--r--   0 yzguy      (501) staff       (20)     2193 2023-06-26 17:53:59.000000 octodns-dnsmadeeasy-0.0.3/octodns_dnsmadeeasy.egg-info/PKG-INFO
+-rw-r--r--   0 yzguy      (501) staff       (20)      322 2023-06-26 17:53:59.000000 octodns-dnsmadeeasy-0.0.3/octodns_dnsmadeeasy.egg-info/SOURCES.txt
+-rw-r--r--   0 yzguy      (501) staff       (20)        1 2023-06-26 17:53:59.000000 octodns-dnsmadeeasy-0.0.3/octodns_dnsmadeeasy.egg-info/dependency_links.txt
+-rw-r--r--   0 yzguy      (501) staff       (20)      238 2023-06-26 17:53:59.000000 octodns-dnsmadeeasy-0.0.3/octodns_dnsmadeeasy.egg-info/requires.txt
+-rw-r--r--   0 yzguy      (501) staff       (20)       20 2023-06-26 17:53:59.000000 octodns-dnsmadeeasy-0.0.3/octodns_dnsmadeeasy.egg-info/top_level.txt
+-rw-r--r--   0 yzguy      (501) staff       (20)      312 2023-06-22 18:01:26.000000 octodns-dnsmadeeasy-0.0.3/pyproject.toml
+-rw-r--r--   0 yzguy      (501) staff       (20)       38 2023-06-26 17:53:59.284114 octodns-dnsmadeeasy-0.0.3/setup.cfg
+-rw-r--r--   0 yzguy      (501) staff       (20)     1830 2023-06-22 18:01:26.000000 octodns-dnsmadeeasy-0.0.3/setup.py
+drwxr-xr-x   0 yzguy      (501) staff       (20)        0 2023-06-26 17:53:59.283607 octodns-dnsmadeeasy-0.0.3/tests/
+-rw-r--r--   0 yzguy      (501) staff       (20)    16135 2023-06-26 17:37:39.000000 octodns-dnsmadeeasy-0.0.3/tests/test_octodns_provider_dnsmadeeasy.py
```

### Comparing `octodns-dnsmadeeasy-0.0.2/PKG-INFO` & `octodns-dnsmadeeasy-0.0.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: octodns-dnsmadeeasy
-Version: 0.0.2
+Version: 0.0.3
 Summary:  DNS Made Easy provider for octoDNS
 Home-page: https://github.com/octodns/octodns-dnsmadeeasy
 Author: Ross McFarland
 Author-email: rwmcfa1@gmail.com
 License: MIT
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
```

### Comparing `octodns-dnsmadeeasy-0.0.2/README.md` & `octodns-dnsmadeeasy-0.0.3/README.md`

 * *Files identical despite different names*

### Comparing `octodns-dnsmadeeasy-0.0.2/octodns_dnsmadeeasy/__init__.py` & `octodns-dnsmadeeasy-0.0.3/octodns_dnsmadeeasy/__init__.py`

 * *Files 8% similar despite different names*

```diff
@@ -11,15 +11,15 @@
 from requests import Session
 
 from octodns import __VERSION__ as octodns_version
 from octodns.provider import ProviderException
 from octodns.provider.base import BaseProvider
 from octodns.record import Record
 
-__VERSION__ = '0.0.2'
+__VERSION__ = '0.0.3'
 
 
 class DnsMadeEasyClientException(ProviderException):
     pass
 
 
 class DnsMadeEasyClientBadRequest(DnsMadeEasyClientException):
@@ -98,18 +98,22 @@
         return self._domains
 
     def domain(self, name):
         path = f'/id/{name}'
         return self._request('GET', path).json()
 
     def domain_create(self, name):
-        self._request('POST', '/', data={'name': name})
+        response = self._request('POST', '/', data={'name': name}).json()
+        # Add our newly created domain to the cache
+        self.domains[f'{name}.'] = response['id']
 
     def records(self, zone_name):
         zone_id = self.domains.get(zone_name, False)
+        if not zone_id:
+            return []
         path = f'/{zone_id}/records'
         ret = []
 
         # has pages in resp, do we need paging?
         resp = self._request('GET', path).json()
         ret += resp['data']
 
@@ -124,28 +128,29 @@
                 if value == '':
                     record['value'] = zone_name
                 elif not value.endswith('.'):
                     record['value'] = f'{value}.{zone_name}'
 
         return ret
 
-    def record_create(self, zone_name, params):
+    def record_multi_delete(self, zone_name, record_ids):
         zone_id = self.domains.get(zone_name, False)
         path = f'/{zone_id}/records'
+        self._request('DELETE', path, params={'ids': record_ids})
 
-        # change ALIAS records to ANAME
-        if params['type'] == 'ALIAS':
-            params['type'] = 'ANAME'
-
-        self._request('POST', path, data=params)
-
-    def record_delete(self, zone_name, record_id):
+    def record_multi_create(self, zone_name, records):
         zone_id = self.domains.get(zone_name, False)
-        path = f'/{zone_id}/records/{record_id}'
-        self._request('DELETE', path)
+        path = f'/{zone_id}/records/createMulti'
+
+        # Change ALIAS records to ANAME
+        for record in records:
+            if record['type'] == 'ALIAS':
+                record['type'] = 'ANAME'
+            record['gtdLocation'] = 'DEFAULT'
+        self._request('POST', path, data=records)
 
 
 class DnsMadeEasyProvider(BaseProvider):
     SUPPORTS_GEO = False
     SUPPORTS_DYNAMIC = False
     SUPPORTS_ROOT_NS = True
     SUPPORTS = set(
@@ -243,18 +248,15 @@
                     'weight': record['weight'],
                 }
             )
         return {'type': _type, 'ttl': records[0]['ttl'], 'values': values}
 
     def zone_records(self, zone):
         if zone.name not in self._zone_records:
-            try:
-                self._zone_records[zone.name] = self._client.records(zone.name)
-            except DnsMadeEasyClientNotFound:
-                return []
+            self._zone_records[zone.name] = self._client.records(zone.name)
 
         return self._zone_records[zone.name]
 
     def populate(self, zone, target=False, lenient=False):
         self.log.debug(
             'populate: name=%s, target=%s, lenient=%s',
             zone.name,
@@ -388,33 +390,38 @@
                 'issuerCritical': value.flags,
                 'name': record.name,
                 'caaType': value.tag,
                 'ttl': record.ttl,
                 'type': record._type,
             }
 
-    def _apply_Create(self, change):
+    def _mod_Create(self, change):
+        creations = []
         new = change.new
         params_for = getattr(self, f'_params_for_{new._type}')
         for params in params_for(new):
-            self._client.record_create(new.zone.name, params)
+            creations.append(params)
+        return new.zone, [], creations
 
-    def _apply_Update(self, change):
-        self._apply_Delete(change)
-        self._apply_Create(change)
-
-    def _apply_Delete(self, change):
+    def _mod_Delete(self, change):
+        deletions = []
         existing = change.existing
         zone = existing.zone
         for record in self.zone_records(zone):
             if (
                 existing.name == record['name']
                 and existing._type == record['type']
             ):
-                self._client.record_delete(zone.name, record['id'])
+                deletions.append(record['id'])
+        return zone, deletions, []
+
+    def _mod_Update(self, change):
+        _, deletions, _ = self._mod_Delete(change)
+        zone, _, creations = self._mod_Create(change)
+        return zone, deletions, creations
 
     def _apply(self, plan):
         desired = plan.desired
         changes = plan.changes
         self.log.debug(
             '_apply: zone=%s, len(changes)=%d', desired.name, len(changes)
         )
@@ -422,13 +429,38 @@
         domain_name = desired.name[:-1]
         try:
             self._client.domain(domain_name)
         except DnsMadeEasyClientNotFound:
             self.log.debug('_apply:   no matching zone, creating domain')
             self._client.domain_create(domain_name)
 
+        zone_operations = {}
+
+        # Optimise our changes into a single set of creates/delete operations for each zone
         for change in changes:
             class_name = change.__class__.__name__
-            getattr(self, f'_apply_{class_name}')(change)
+            zone, mod_del, mod_create = getattr(self, f'_mod_{class_name}')(
+                change
+            )
+            if zone.name in zone_operations:
+                zone_operations[zone.name]['deletions'].extend(mod_del)
+                zone_operations[zone.name]['creations'].extend(mod_create)
+            else:
+                zone_operations[zone.name] = {
+                    'zone': zone,
+                    'deletions': mod_del,
+                    'creations': mod_create,
+                }
+
+        # Perform our operations
+        for zone_name, operation in zone_operations.items():
+            if operation['deletions']:
+                self._client.record_multi_delete(
+                    zone_name, operation['deletions']
+                )
+            if operation['creations']:
+                self._client.record_multi_create(
+                    zone_name, operation['creations']
+                )
 
         # Clear out the cache if any
         self._zone_records.pop(desired.name, None)
```

### Comparing `octodns-dnsmadeeasy-0.0.2/octodns_dnsmadeeasy.egg-info/PKG-INFO` & `octodns-dnsmadeeasy-0.0.3/octodns_dnsmadeeasy.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: octodns-dnsmadeeasy
-Version: 0.0.2
+Version: 0.0.3
 Summary:  DNS Made Easy provider for octoDNS
 Home-page: https://github.com/octodns/octodns-dnsmadeeasy
 Author: Ross McFarland
 Author-email: rwmcfa1@gmail.com
 License: MIT
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
```

### Comparing `octodns-dnsmadeeasy-0.0.2/setup.py` & `octodns-dnsmadeeasy-0.0.3/setup.py`

 * *Files identical despite different names*

