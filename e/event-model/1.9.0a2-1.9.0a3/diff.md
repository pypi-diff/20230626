# Comparing `tmp/event-model-1.9.0a2.tar.gz` & `tmp/event-model-1.9.0a3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/event-model-1.9.0a2.tar", last modified: Wed Apr  3 13:51:23 2019, max compression
+gzip compressed data, was "dist/event-model-1.9.0a3.tar", last modified: Wed Apr  3 14:46:05 2019, max compression
```

## Comparing `event-model-1.9.0a2.tar` & `event-model-1.9.0a3.tar`

### file list

```diff
@@ -1,42 +1,42 @@
-drwxr-xr-x   0 dallan    (1000) dallan    (1000)        0 2019-04-03 13:51:23.000000 event-model-1.9.0a2/
-drwxr-xr-x   0 dallan    (1000) dallan    (1000)        0 2019-04-03 13:51:23.000000 event-model-1.9.0a2/event_model.egg-info/
--rw-r--r--   0 dallan    (1000) dallan    (1000)        1 2019-04-03 13:51:22.000000 event-model-1.9.0a2/event_model.egg-info/dependency_links.txt
--rw-r--r--   0 dallan    (1000) dallan    (1000)       20 2019-04-03 13:51:22.000000 event-model-1.9.0a2/event_model.egg-info/entry_points.txt
--rw-r--r--   0 dallan    (1000) dallan    (1000)       17 2019-04-03 13:51:22.000000 event-model-1.9.0a2/event_model.egg-info/requires.txt
--rw-r--r--   0 dallan    (1000) dallan    (1000)     3419 2019-04-03 13:51:22.000000 event-model-1.9.0a2/event_model.egg-info/PKG-INFO
--rw-r--r--   0 dallan    (1000) dallan    (1000)       12 2019-04-03 13:51:22.000000 event-model-1.9.0a2/event_model.egg-info/top_level.txt
--rw-r--r--   0 dallan    (1000) dallan    (1000)      911 2019-04-03 13:51:22.000000 event-model-1.9.0a2/event_model.egg-info/SOURCES.txt
-drwxr-xr-x   0 dallan    (1000) dallan    (1000)        0 2019-04-03 13:51:23.000000 event-model-1.9.0a2/event_model/
--rw-r--r--   0 dallan    (1000) dallan    (1000)    41625 2019-04-03 13:50:19.000000 event-model-1.9.0a2/event_model/__init__.py
--rw-r--r--   0 dallan    (1000) dallan    (1000)      499 2019-04-03 13:51:23.000000 event-model-1.9.0a2/event_model/_version.py
-drwxr-xr-x   0 dallan    (1000) dallan    (1000)        0 2019-04-03 13:51:23.000000 event-model-1.9.0a2/event_model/schemas/
--rw-r--r--   0 dallan    (1000) dallan    (1000)     2974 2018-10-29 19:41:48.000000 event-model-1.9.0a2/event_model/schemas/run_start.json
--rw-r--r--   0 dallan    (1000) dallan    (1000)     2050 2019-01-09 14:29:05.000000 event-model-1.9.0a2/event_model/schemas/bulk_events.json
--rw-r--r--   0 dallan    (1000) dallan    (1000)     2163 2019-01-25 20:02:13.000000 event-model-1.9.0a2/event_model/schemas/event_page.json
--rw-r--r--   0 dallan    (1000) dallan    (1000)     5704 2019-03-25 15:33:57.000000 event-model-1.9.0a2/event_model/schemas/event_descriptor.json
--rw-r--r--   0 dallan    (1000) dallan    (1000)     1536 2019-01-16 20:07:07.000000 event-model-1.9.0a2/event_model/schemas/event.json
--rw-r--r--   0 dallan    (1000) dallan    (1000)      801 2018-10-29 19:41:48.000000 event-model-1.9.0a2/event_model/schemas/datum.json
--rw-r--r--   0 dallan    (1000) dallan    (1000)     1074 2019-01-09 14:29:05.000000 event-model-1.9.0a2/event_model/schemas/datum_page.json
--rw-r--r--   0 dallan    (1000) dallan    (1000)     1445 2018-10-29 19:41:48.000000 event-model-1.9.0a2/event_model/schemas/resource.json
--rw-r--r--   0 dallan    (1000) dallan    (1000)     1548 2018-10-29 19:41:48.000000 event-model-1.9.0a2/event_model/schemas/run_stop.json
--rw-r--r--   0 dallan    (1000) dallan    (1000)      912 2019-01-09 14:29:05.000000 event-model-1.9.0a2/event_model/schemas/bulk_datum.json
-drwxr-xr-x   0 dallan    (1000) dallan    (1000)        0 2019-04-03 13:51:23.000000 event-model-1.9.0a2/event_model/tests/
--rw-r--r--   0 dallan    (1000) dallan    (1000)    20620 2019-04-03 13:50:19.000000 event-model-1.9.0a2/event_model/tests/test_em.py
--rw-r--r--   0 dallan    (1000) dallan    (1000)        0 2019-02-13 22:08:11.000000 event-model-1.9.0a2/event_model/tests/__init__.py
--rw-r--r--   0 dallan    (1000) dallan    (1000)     3419 2019-04-03 13:51:23.000000 event-model-1.9.0a2/PKG-INFO
--rw-r--r--   0 dallan    (1000) dallan    (1000)    68611 2019-02-13 22:08:11.000000 event-model-1.9.0a2/versioneer.py
--rw-r--r--   0 dallan    (1000) dallan    (1000)      227 2019-04-03 13:51:23.000000 event-model-1.9.0a2/setup.cfg
--rw-r--r--   0 dallan    (1000) dallan    (1000)      374 2019-02-13 22:08:11.000000 event-model-1.9.0a2/MANIFEST.in
--rw-r--r--   0 dallan    (1000) dallan    (1000)     1584 2019-02-13 14:24:10.000000 event-model-1.9.0a2/LICENSE
-drwxr-xr-x   0 dallan    (1000) dallan    (1000)        0 2019-04-03 13:51:23.000000 event-model-1.9.0a2/docs/
-drwxr-xr-x   0 dallan    (1000) dallan    (1000)        0 2019-04-03 13:51:23.000000 event-model-1.9.0a2/docs/source/
--rw-r--r--   0 dallan    (1000) dallan    (1000)     1082 2019-02-13 22:08:11.000000 event-model-1.9.0a2/docs/source/api.rst
--rw-r--r--   0 dallan    (1000) dallan    (1000)       81 2019-02-13 22:08:11.000000 event-model-1.9.0a2/docs/source/installation.rst
--rw-r--r--   0 dallan    (1000) dallan    (1000)     1259 2019-04-01 16:32:07.000000 event-model-1.9.0a2/docs/source/release-history.rst
--rw-r--r--   0 dallan    (1000) dallan    (1000)     6417 2019-02-13 22:08:11.000000 event-model-1.9.0a2/docs/source/conf.py
--rw-r--r--   0 dallan    (1000) dallan    (1000)      599 2019-02-13 22:08:11.000000 event-model-1.9.0a2/docs/source/index.rst
--rw-r--r--   0 dallan    (1000) dallan    (1000)    11788 2019-03-05 20:43:21.000000 event-model-1.9.0a2/docs/source/data-model.rst
--rw-r--r--   0 dallan    (1000) dallan    (1000)      673 2019-02-13 22:08:11.000000 event-model-1.9.0a2/docs/Makefile
--rw-r--r--   0 dallan    (1000) dallan    (1000)      797 2019-02-13 22:08:11.000000 event-model-1.9.0a2/docs/make.bat
--rw-r--r--   0 dallan    (1000) dallan    (1000)     2474 2018-10-29 19:41:48.000000 event-model-1.9.0a2/README.md
--rw-r--r--   0 dallan    (1000) dallan    (1000)     2236 2019-04-03 13:50:19.000000 event-model-1.9.0a2/setup.py
+drwxr-xr-x   0 dallan    (1000) dallan    (1000)        0 2019-04-03 14:46:05.000000 event-model-1.9.0a3/
+drwxr-xr-x   0 dallan    (1000) dallan    (1000)        0 2019-04-03 14:46:05.000000 event-model-1.9.0a3/event_model.egg-info/
+-rw-r--r--   0 dallan    (1000) dallan    (1000)        1 2019-04-03 14:46:05.000000 event-model-1.9.0a3/event_model.egg-info/dependency_links.txt
+-rw-r--r--   0 dallan    (1000) dallan    (1000)       20 2019-04-03 14:46:05.000000 event-model-1.9.0a3/event_model.egg-info/entry_points.txt
+-rw-r--r--   0 dallan    (1000) dallan    (1000)       17 2019-04-03 14:46:05.000000 event-model-1.9.0a3/event_model.egg-info/requires.txt
+-rw-r--r--   0 dallan    (1000) dallan    (1000)     3419 2019-04-03 14:46:05.000000 event-model-1.9.0a3/event_model.egg-info/PKG-INFO
+-rw-r--r--   0 dallan    (1000) dallan    (1000)       12 2019-04-03 14:46:05.000000 event-model-1.9.0a3/event_model.egg-info/top_level.txt
+-rw-r--r--   0 dallan    (1000) dallan    (1000)      911 2019-04-03 14:46:05.000000 event-model-1.9.0a3/event_model.egg-info/SOURCES.txt
+drwxr-xr-x   0 dallan    (1000) dallan    (1000)        0 2019-04-03 14:46:05.000000 event-model-1.9.0a3/event_model/
+-rw-r--r--   0 dallan    (1000) dallan    (1000)    41669 2019-04-03 14:41:59.000000 event-model-1.9.0a3/event_model/__init__.py
+-rw-r--r--   0 dallan    (1000) dallan    (1000)      499 2019-04-03 14:46:05.000000 event-model-1.9.0a3/event_model/_version.py
+drwxr-xr-x   0 dallan    (1000) dallan    (1000)        0 2019-04-03 14:46:05.000000 event-model-1.9.0a3/event_model/schemas/
+-rw-r--r--   0 dallan    (1000) dallan    (1000)     2974 2018-10-29 19:41:48.000000 event-model-1.9.0a3/event_model/schemas/run_start.json
+-rw-r--r--   0 dallan    (1000) dallan    (1000)     2050 2019-01-09 14:29:05.000000 event-model-1.9.0a3/event_model/schemas/bulk_events.json
+-rw-r--r--   0 dallan    (1000) dallan    (1000)     2163 2019-01-25 20:02:13.000000 event-model-1.9.0a3/event_model/schemas/event_page.json
+-rw-r--r--   0 dallan    (1000) dallan    (1000)     5704 2019-03-25 15:33:57.000000 event-model-1.9.0a3/event_model/schemas/event_descriptor.json
+-rw-r--r--   0 dallan    (1000) dallan    (1000)     1536 2019-01-16 20:07:07.000000 event-model-1.9.0a3/event_model/schemas/event.json
+-rw-r--r--   0 dallan    (1000) dallan    (1000)      801 2018-10-29 19:41:48.000000 event-model-1.9.0a3/event_model/schemas/datum.json
+-rw-r--r--   0 dallan    (1000) dallan    (1000)     1074 2019-01-09 14:29:05.000000 event-model-1.9.0a3/event_model/schemas/datum_page.json
+-rw-r--r--   0 dallan    (1000) dallan    (1000)     1445 2018-10-29 19:41:48.000000 event-model-1.9.0a3/event_model/schemas/resource.json
+-rw-r--r--   0 dallan    (1000) dallan    (1000)     1548 2018-10-29 19:41:48.000000 event-model-1.9.0a3/event_model/schemas/run_stop.json
+-rw-r--r--   0 dallan    (1000) dallan    (1000)      912 2019-01-09 14:29:05.000000 event-model-1.9.0a3/event_model/schemas/bulk_datum.json
+drwxr-xr-x   0 dallan    (1000) dallan    (1000)        0 2019-04-03 14:46:05.000000 event-model-1.9.0a3/event_model/tests/
+-rw-r--r--   0 dallan    (1000) dallan    (1000)    21504 2019-04-03 14:41:59.000000 event-model-1.9.0a3/event_model/tests/test_em.py
+-rw-r--r--   0 dallan    (1000) dallan    (1000)        0 2019-02-13 22:08:11.000000 event-model-1.9.0a3/event_model/tests/__init__.py
+-rw-r--r--   0 dallan    (1000) dallan    (1000)     3419 2019-04-03 14:46:05.000000 event-model-1.9.0a3/PKG-INFO
+-rw-r--r--   0 dallan    (1000) dallan    (1000)    68611 2019-02-13 22:08:11.000000 event-model-1.9.0a3/versioneer.py
+-rw-r--r--   0 dallan    (1000) dallan    (1000)      227 2019-04-03 14:46:05.000000 event-model-1.9.0a3/setup.cfg
+-rw-r--r--   0 dallan    (1000) dallan    (1000)      374 2019-02-13 22:08:11.000000 event-model-1.9.0a3/MANIFEST.in
+-rw-r--r--   0 dallan    (1000) dallan    (1000)     1584 2019-02-13 14:24:10.000000 event-model-1.9.0a3/LICENSE
+drwxr-xr-x   0 dallan    (1000) dallan    (1000)        0 2019-04-03 14:46:05.000000 event-model-1.9.0a3/docs/
+drwxr-xr-x   0 dallan    (1000) dallan    (1000)        0 2019-04-03 14:46:05.000000 event-model-1.9.0a3/docs/source/
+-rw-r--r--   0 dallan    (1000) dallan    (1000)     1082 2019-02-13 22:08:11.000000 event-model-1.9.0a3/docs/source/api.rst
+-rw-r--r--   0 dallan    (1000) dallan    (1000)       81 2019-02-13 22:08:11.000000 event-model-1.9.0a3/docs/source/installation.rst
+-rw-r--r--   0 dallan    (1000) dallan    (1000)     1259 2019-04-01 16:32:07.000000 event-model-1.9.0a3/docs/source/release-history.rst
+-rw-r--r--   0 dallan    (1000) dallan    (1000)     6417 2019-02-13 22:08:11.000000 event-model-1.9.0a3/docs/source/conf.py
+-rw-r--r--   0 dallan    (1000) dallan    (1000)      599 2019-02-13 22:08:11.000000 event-model-1.9.0a3/docs/source/index.rst
+-rw-r--r--   0 dallan    (1000) dallan    (1000)    11788 2019-03-05 20:43:21.000000 event-model-1.9.0a3/docs/source/data-model.rst
+-rw-r--r--   0 dallan    (1000) dallan    (1000)      673 2019-02-13 22:08:11.000000 event-model-1.9.0a3/docs/Makefile
+-rw-r--r--   0 dallan    (1000) dallan    (1000)      797 2019-02-13 22:08:11.000000 event-model-1.9.0a3/docs/make.bat
+-rw-r--r--   0 dallan    (1000) dallan    (1000)     2474 2018-10-29 19:41:48.000000 event-model-1.9.0a3/README.md
+-rw-r--r--   0 dallan    (1000) dallan    (1000)     2236 2019-04-03 13:50:19.000000 event-model-1.9.0a3/setup.py
```

### Comparing `event-model-1.9.0a2/event_model.egg-info/PKG-INFO` & `event-model-1.9.0a3/event_model.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: event-model
-Version: 1.9.0a2
+Version: 1.9.0a3
 Summary: Data model used by the bluesky ecosystem
 Home-page: https://github.com/NSLS-II/event-model
 Author: Brookhaven National Lab
 Author-email: dallan@bnl.gov
 License: BSD (3-clause)
 Description: # Event Model
```

### Comparing `event-model-1.9.0a2/event_model.egg-info/SOURCES.txt` & `event-model-1.9.0a3/event_model.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `event-model-1.9.0a2/event_model/__init__.py` & `event-model-1.9.0a3/event_model/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -958,17 +958,18 @@
 
     Yields
     ------
     datum : dict
     """
     resource = datum_page['resource']
     datum_kwarg_list = _transpose_dict_of_lists(datum_page['datum_kwargs'])
-    for datum_id, datum_kwargs in zip(
+    for datum_id, datum_kwargs in itertools.zip_longest(
             datum_page['datum_id'],
-            datum_kwarg_list):
+            datum_kwarg_list,
+            fillvalue={}):
         datum = {'datum_id': datum_id, 'datum_kwargs': datum_kwargs,
                  'resource': resource}
         yield datum
 
 
 def bulk_events_to_event_pages(bulk_events):
     """
```

### Comparing `event-model-1.9.0a2/event_model/schemas/run_start.json` & `event-model-1.9.0a3/event_model/schemas/run_start.json`

 * *Files identical despite different names*

### Comparing `event-model-1.9.0a2/event_model/schemas/bulk_events.json` & `event-model-1.9.0a3/event_model/schemas/bulk_events.json`

 * *Files identical despite different names*

### Comparing `event-model-1.9.0a2/event_model/schemas/event_page.json` & `event-model-1.9.0a3/event_model/schemas/event_page.json`

 * *Files identical despite different names*

### Comparing `event-model-1.9.0a2/event_model/schemas/event_descriptor.json` & `event-model-1.9.0a3/event_model/schemas/event_descriptor.json`

 * *Files identical despite different names*

### Comparing `event-model-1.9.0a2/event_model/schemas/event.json` & `event-model-1.9.0a3/event_model/schemas/event.json`

 * *Files identical despite different names*

### Comparing `event-model-1.9.0a2/event_model/schemas/datum.json` & `event-model-1.9.0a3/event_model/schemas/datum.json`

 * *Files identical despite different names*

### Comparing `event-model-1.9.0a2/event_model/schemas/datum_page.json` & `event-model-1.9.0a3/event_model/schemas/datum_page.json`

 * *Files identical despite different names*

### Comparing `event-model-1.9.0a2/event_model/schemas/resource.json` & `event-model-1.9.0a3/event_model/schemas/resource.json`

 * *Files identical despite different names*

### Comparing `event-model-1.9.0a2/event_model/schemas/run_stop.json` & `event-model-1.9.0a3/event_model/schemas/run_stop.json`

 * *Files identical despite different names*

### Comparing `event-model-1.9.0a2/event_model/schemas/bulk_datum.json` & `event-model-1.9.0a3/event_model/schemas/bulk_datum.json`

 * *Files identical despite different names*

### Comparing `event-model-1.9.0a2/event_model/tests/test_em.py` & `event-model-1.9.0a3/event_model/tests/test_em.py`

 * *Files 7% similar despite different names*

```diff
@@ -131,14 +131,37 @@
 
     # Round trip three datum -> datum_page -> datum.
     expected = [datum_doc1, datum_doc2, datum_doc3]
     actual = list(event_model.unpack_datum_page(
         event_model.pack_datum_page(*expected)))
     assert actual == expected
 
+    # Check edge case where datum_kwargs are empty.
+    datum_doc1 = res_bundle.compose_datum(datum_kwargs={})
+    datum_doc2 = res_bundle.compose_datum(datum_kwargs={})
+    datum_doc3 = res_bundle.compose_datum(datum_kwargs={})
+
+    # Round trip one datum -> datum_page -> datum.
+    expected = datum_doc1
+    actual, = event_model.unpack_datum_page(
+        event_model.pack_datum_page(expected))
+    assert actual == expected
+
+    # Round trip two datum -> datum_page -> datum.
+    expected = [datum_doc1, datum_doc2]
+    actual = list(event_model.unpack_datum_page(
+        event_model.pack_datum_page(*expected)))
+    assert actual == expected
+
+    # Round trip three datum -> datum_page -> datum.
+    expected = [datum_doc1, datum_doc2, datum_doc3]
+    actual = list(event_model.unpack_datum_page(
+        event_model.pack_datum_page(*expected)))
+    assert actual == expected
+
 
 def test_bulk_events_to_event_page(tmp_path):
     run_bundle = event_model.compose_run()
     desc_bundle = run_bundle.compose_descriptor(
         data_keys={'motor': {'shape': [], 'dtype': 'number', 'source': '...'},
                    'image': {'shape': [512, 512], 'dtype': 'number',
                              'source': '...', 'external': 'FILESTORE:'}},
```

### Comparing `event-model-1.9.0a2/PKG-INFO` & `event-model-1.9.0a3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: event-model
-Version: 1.9.0a2
+Version: 1.9.0a3
 Summary: Data model used by the bluesky ecosystem
 Home-page: https://github.com/NSLS-II/event-model
 Author: Brookhaven National Lab
 Author-email: dallan@bnl.gov
 License: BSD (3-clause)
 Description: # Event Model
```

### Comparing `event-model-1.9.0a2/versioneer.py` & `event-model-1.9.0a3/versioneer.py`

 * *Files identical despite different names*

### Comparing `event-model-1.9.0a2/LICENSE` & `event-model-1.9.0a3/LICENSE`

 * *Files identical despite different names*

### Comparing `event-model-1.9.0a2/docs/source/api.rst` & `event-model-1.9.0a3/docs/source/api.rst`

 * *Files identical despite different names*

### Comparing `event-model-1.9.0a2/docs/source/release-history.rst` & `event-model-1.9.0a3/docs/source/release-history.rst`

 * *Files identical despite different names*

### Comparing `event-model-1.9.0a2/docs/source/conf.py` & `event-model-1.9.0a3/docs/source/conf.py`

 * *Files identical despite different names*

### Comparing `event-model-1.9.0a2/docs/source/index.rst` & `event-model-1.9.0a3/docs/source/index.rst`

 * *Files identical despite different names*

### Comparing `event-model-1.9.0a2/docs/source/data-model.rst` & `event-model-1.9.0a3/docs/source/data-model.rst`

 * *Files identical despite different names*

### Comparing `event-model-1.9.0a2/docs/Makefile` & `event-model-1.9.0a3/docs/Makefile`

 * *Files identical despite different names*

### Comparing `event-model-1.9.0a2/docs/make.bat` & `event-model-1.9.0a3/docs/make.bat`

 * *Files identical despite different names*

### Comparing `event-model-1.9.0a2/README.md` & `event-model-1.9.0a3/README.md`

 * *Files identical despite different names*

### Comparing `event-model-1.9.0a2/setup.py` & `event-model-1.9.0a3/setup.py`

 * *Files identical despite different names*

