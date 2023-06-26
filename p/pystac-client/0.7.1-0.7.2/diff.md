# Comparing `tmp/pystac-client-0.7.1.tar.gz` & `tmp/pystac-client-0.7.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pystac-client-0.7.1.tar", last modified: Tue Jun 13 12:48:18 2023, max compression
+gzip compressed data, was "pystac-client-0.7.2.tar", last modified: Mon Jun 26 13:40:42 2023, max compression
```

## Comparing `pystac-client-0.7.1.tar` & `pystac-client-0.7.2.tar`

### file list

```diff
@@ -1,35 +1,35 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 12:48:18.773177 pystac-client-0.7.1/
--rw-r--r--   0 runner    (1001) docker     (123)      553 2023-06-13 12:48:04.000000 pystac-client-0.7.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)       23 2023-06-13 12:48:04.000000 pystac-client-0.7.1/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     3164 2023-06-13 12:48:18.773177 pystac-client-0.7.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1581 2023-06-13 12:48:04.000000 pystac-client-0.7.1/README.md
--rw-r--r--   0 runner    (1001) docker     (123)     3483 2023-06-13 12:48:04.000000 pystac-client-0.7.1/pyproject.toml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 12:48:18.773177 pystac-client-0.7.1/pystac_client/
--rw-r--r--   0 runner    (1001) docker     (123)      431 2023-06-13 12:48:04.000000 pystac-client-0.7.1/pystac_client/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      806 2023-06-13 12:48:04.000000 pystac-client-0.7.1/pystac_client/_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)    11237 2023-06-13 12:48:04.000000 pystac-client-0.7.1/pystac_client/cli.py
--rw-r--r--   0 runner    (1001) docker     (123)    26027 2023-06-13 12:48:04.000000 pystac-client-0.7.1/pystac_client/client.py
--rw-r--r--   0 runner    (1001) docker     (123)     7170 2023-06-13 12:48:04.000000 pystac-client-0.7.1/pystac_client/collection_client.py
--rw-r--r--   0 runner    (1001) docker     (123)     1324 2023-06-13 12:48:04.000000 pystac-client-0.7.1/pystac_client/conformance.py
--rw-r--r--   0 runner    (1001) docker     (123)      246 2023-06-13 12:48:04.000000 pystac-client-0.7.1/pystac_client/errors.py
--rw-r--r--   0 runner    (1001) docker     (123)      449 2023-06-13 12:48:04.000000 pystac-client-0.7.1/pystac_client/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (123)    32409 2023-06-13 12:48:04.000000 pystac-client-0.7.1/pystac_client/item_search.py
--rw-r--r--   0 runner    (1001) docker     (123)     2217 2023-06-13 12:48:04.000000 pystac-client-0.7.1/pystac_client/mixins.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-13 12:48:04.000000 pystac-client-0.7.1/pystac_client/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)    12350 2023-06-13 12:48:04.000000 pystac-client-0.7.1/pystac_client/stac_api_io.py
--rw-r--r--   0 runner    (1001) docker     (123)       22 2023-06-13 12:48:04.000000 pystac-client-0.7.1/pystac_client/version.py
--rw-r--r--   0 runner    (1001) docker     (123)     2767 2023-06-13 12:48:04.000000 pystac-client-0.7.1/pystac_client/warnings.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 12:48:18.773177 pystac-client-0.7.1/pystac_client.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     3164 2023-06-13 12:48:18.000000 pystac-client-0.7.1/pystac_client.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      758 2023-06-13 12:48:18.000000 pystac-client-0.7.1/pystac_client.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-13 12:48:18.000000 pystac-client-0.7.1/pystac_client.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       54 2023-06-13 12:48:18.000000 pystac-client-0.7.1/pystac_client.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)      743 2023-06-13 12:48:18.000000 pystac-client-0.7.1/pystac_client.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       14 2023-06-13 12:48:18.000000 pystac-client-0.7.1/pystac_client.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-13 12:48:18.773177 pystac-client-0.7.1/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 12:48:18.773177 pystac-client-0.7.1/tests/
--rw-r--r--   0 runner    (1001) docker     (123)     2679 2023-06-13 12:48:04.000000 pystac-client-0.7.1/tests/test_cli.py
--rw-r--r--   0 runner    (1001) docker     (123)    25263 2023-06-13 12:48:04.000000 pystac-client-0.7.1/tests/test_client.py
--rw-r--r--   0 runner    (1001) docker     (123)     2810 2023-06-13 12:48:04.000000 pystac-client-0.7.1/tests/test_collection_client.py
--rw-r--r--   0 runner    (1001) docker     (123)    29284 2023-06-13 12:48:04.000000 pystac-client-0.7.1/tests/test_item_search.py
--rw-r--r--   0 runner    (1001) docker     (123)     9118 2023-06-13 12:48:04.000000 pystac-client-0.7.1/tests/test_stac_api_io.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 13:40:42.529092 pystac-client-0.7.2/
+-rw-r--r--   0 runner    (1001) docker     (123)      553 2023-06-26 13:40:22.000000 pystac-client-0.7.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       23 2023-06-26 13:40:22.000000 pystac-client-0.7.2/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     3164 2023-06-26 13:40:42.529092 pystac-client-0.7.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1581 2023-06-26 13:40:22.000000 pystac-client-0.7.2/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)     3477 2023-06-26 13:40:22.000000 pystac-client-0.7.2/pyproject.toml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 13:40:42.529092 pystac-client-0.7.2/pystac_client/
+-rw-r--r--   0 runner    (1001) docker     (123)      431 2023-06-26 13:40:22.000000 pystac-client-0.7.2/pystac_client/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      806 2023-06-26 13:40:22.000000 pystac-client-0.7.2/pystac_client/_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11237 2023-06-26 13:40:22.000000 pystac-client-0.7.2/pystac_client/cli.py
+-rw-r--r--   0 runner    (1001) docker     (123)    26027 2023-06-26 13:40:22.000000 pystac-client-0.7.2/pystac_client/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7170 2023-06-26 13:40:22.000000 pystac-client-0.7.2/pystac_client/collection_client.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1324 2023-06-26 13:40:22.000000 pystac-client-0.7.2/pystac_client/conformance.py
+-rw-r--r--   0 runner    (1001) docker     (123)      246 2023-06-26 13:40:22.000000 pystac-client-0.7.2/pystac_client/errors.py
+-rw-r--r--   0 runner    (1001) docker     (123)      449 2023-06-26 13:40:22.000000 pystac-client-0.7.2/pystac_client/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)    32409 2023-06-26 13:40:22.000000 pystac-client-0.7.2/pystac_client/item_search.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2217 2023-06-26 13:40:22.000000 pystac-client-0.7.2/pystac_client/mixins.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-26 13:40:22.000000 pystac-client-0.7.2/pystac_client/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)    12285 2023-06-26 13:40:22.000000 pystac-client-0.7.2/pystac_client/stac_api_io.py
+-rw-r--r--   0 runner    (1001) docker     (123)       22 2023-06-26 13:40:22.000000 pystac-client-0.7.2/pystac_client/version.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2767 2023-06-26 13:40:22.000000 pystac-client-0.7.2/pystac_client/warnings.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 13:40:42.529092 pystac-client-0.7.2/pystac_client.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     3164 2023-06-26 13:40:42.000000 pystac-client-0.7.2/pystac_client.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      758 2023-06-26 13:40:42.000000 pystac-client-0.7.2/pystac_client.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-26 13:40:42.000000 pystac-client-0.7.2/pystac_client.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       54 2023-06-26 13:40:42.000000 pystac-client-0.7.2/pystac_client.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      737 2023-06-26 13:40:42.000000 pystac-client-0.7.2/pystac_client.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       14 2023-06-26 13:40:42.000000 pystac-client-0.7.2/pystac_client.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-26 13:40:42.529092 pystac-client-0.7.2/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 13:40:42.529092 pystac-client-0.7.2/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     2679 2023-06-26 13:40:22.000000 pystac-client-0.7.2/tests/test_cli.py
+-rw-r--r--   0 runner    (1001) docker     (123)    25649 2023-06-26 13:40:22.000000 pystac-client-0.7.2/tests/test_client.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2810 2023-06-26 13:40:22.000000 pystac-client-0.7.2/tests/test_collection_client.py
+-rw-r--r--   0 runner    (1001) docker     (123)    29284 2023-06-26 13:40:22.000000 pystac-client-0.7.2/tests/test_item_search.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9118 2023-06-26 13:40:22.000000 pystac-client-0.7.2/tests/test_stac_api_io.py
```

### Comparing `pystac-client-0.7.1/LICENSE` & `pystac-client-0.7.2/LICENSE`

 * *Files identical despite different names*

### Comparing `pystac-client-0.7.1/PKG-INFO` & `pystac-client-0.7.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pystac-client
-Version: 0.7.1
+Version: 0.7.2
 Summary: Python library for working with SpatioTemporal Asset Catalog (STAC) APIs.
 Author-email: Jon Duckworth <duckontheweb@gmail.com>, Matthew Hanson <matt.a.hanson@gmail.com>
 Maintainer-email: Pete Gadomski <pete.gadomski@gmail.com>
 License: Apache-2.0
 Project-URL: homepage, https://github.com/stac-utils/pystac-client
 Project-URL: documentation, https://pystac-client.readthedocs.io
 Project-URL: repository, https://github.com/stac-utils/pystac-client.git
```

### Comparing `pystac-client-0.7.1/README.md` & `pystac-client-0.7.2/README.md`

 * *Files identical despite different names*

### Comparing `pystac-client-0.7.1/pyproject.toml` & `pystac-client-0.7.2/pyproject.toml`

 * *Files 5% similar despite different names*

```diff
@@ -38,26 +38,26 @@
 
 [project.optional-dependencies]
 dev = [
     "black~=23.3.0",
     "codespell~=2.2.4",
     "coverage~=7.2",
     "doc8~=1.1.1",
-    "importlib-metadata~=6.6.0",
+    "importlib-metadata~=6.7",
     "mypy~=1.2",
     "orjson~=3.8",
     "pre-commit~=3.2",
     "pytest-benchmark~=4.0.0",
     "pytest-console-scripts~=1.4.0",
     "pytest-cov~=4.1.0",
     "pytest-recording~=0.12.2",
-    "pytest~=7.3.1",
+    "pytest~=7.4",
     "recommonmark~=0.7.1",
     "requests-mock~=1.11.0",
-    "ruff==0.0.272",
+    "ruff==0.0.275",
     "tomli~=2.0; python_version<'3.11'",
     "types-python-dateutil~=2.8.19",
     "types-requests~=2.31.0",
     "urllib3<2",  # temporary pin https://github.com/stac-utils/pystac-client/issues/509
 ]
 docs = [
     "Sphinx~=6.2",
@@ -67,15 +67,15 @@
     "geopandas~=0.13.0",
     "geoviews~=1.9",
     "hvplot~=0.8.3",
     "ipykernel~=6.22",
     "ipython~=8.12",
     "jinja2<4.0",
     "matplotlib~=3.7.1",
-    "myst-parser~=1.0.0",
+    "myst-parser~=2.0",
     "nbsphinx~=0.9",
     "pydata-sphinx-theme~=0.13",
     "pygeoif~=1.0",
     "scipy~=1.10",
     "sphinxcontrib-fulltoc~=1.2",
 ]
```

### Comparing `pystac-client-0.7.1/pystac_client/_utils.py` & `pystac-client-0.7.2/pystac_client/_utils.py`

 * *Files identical despite different names*

### Comparing `pystac-client-0.7.1/pystac_client/cli.py` & `pystac-client-0.7.2/pystac_client/cli.py`

 * *Files identical despite different names*

### Comparing `pystac-client-0.7.1/pystac_client/client.py` & `pystac-client-0.7.2/pystac_client/client.py`

 * *Files identical despite different names*

### Comparing `pystac-client-0.7.1/pystac_client/collection_client.py` & `pystac-client-0.7.2/pystac_client/collection_client.py`

 * *Files identical despite different names*

### Comparing `pystac-client-0.7.1/pystac_client/conformance.py` & `pystac-client-0.7.2/pystac_client/conformance.py`

 * *Files identical despite different names*

### Comparing `pystac-client-0.7.1/pystac_client/item_search.py` & `pystac-client-0.7.2/pystac_client/item_search.py`

 * *Files identical despite different names*

### Comparing `pystac-client-0.7.1/pystac_client/mixins.py` & `pystac-client-0.7.2/pystac_client/mixins.py`

 * *Files identical despite different names*

### Comparing `pystac-client-0.7.1/pystac_client/stac_api_io.py` & `pystac-client-0.7.2/pystac_client/stac_api_io.py`

 * *Files 2% similar despite different names*

```diff
@@ -263,15 +263,14 @@
             result = pystac_client.client.Client.from_dict(
                 d, href=str(href), root=root, migrate=False, preserve_dict=preserve_dict
             )
             result._stac_io = self
             return result
 
         if info.object_type == pystac.STACObjectType.COLLECTION:
-            assert isinstance(root, pystac_client.client.Client)
             return pystac_client.collection_client.CollectionClient.from_dict(
                 d, href=str(href), root=root, migrate=False, preserve_dict=preserve_dict
             )
 
         if info.object_type == pystac.STACObjectType.ITEM:
             return pystac.Item.from_dict(
                 d, href=str(href), root=root, migrate=False, preserve_dict=preserve_dict
```

### Comparing `pystac-client-0.7.1/pystac_client/warnings.py` & `pystac-client-0.7.2/pystac_client/warnings.py`

 * *Files identical despite different names*

### Comparing `pystac-client-0.7.1/pystac_client.egg-info/PKG-INFO` & `pystac-client-0.7.2/pystac_client.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pystac-client
-Version: 0.7.1
+Version: 0.7.2
 Summary: Python library for working with SpatioTemporal Asset Catalog (STAC) APIs.
 Author-email: Jon Duckworth <duckontheweb@gmail.com>, Matthew Hanson <matt.a.hanson@gmail.com>
 Maintainer-email: Pete Gadomski <pete.gadomski@gmail.com>
 License: Apache-2.0
 Project-URL: homepage, https://github.com/stac-utils/pystac-client
 Project-URL: documentation, https://pystac-client.readthedocs.io
 Project-URL: repository, https://github.com/stac-utils/pystac-client.git
```

### Comparing `pystac-client-0.7.1/pystac_client.egg-info/SOURCES.txt` & `pystac-client-0.7.2/pystac_client.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `pystac-client-0.7.1/pystac_client.egg-info/requires.txt` & `pystac-client-0.7.2/pystac_client.egg-info/requires.txt`

 * *Files 4% similar despite different names*

```diff
@@ -3,26 +3,26 @@
 python-dateutil>=2.8.2
 
 [dev]
 black~=23.3.0
 codespell~=2.2.4
 coverage~=7.2
 doc8~=1.1.1
-importlib-metadata~=6.6.0
+importlib-metadata~=6.7
 mypy~=1.2
 orjson~=3.8
 pre-commit~=3.2
 pytest-benchmark~=4.0.0
 pytest-console-scripts~=1.4.0
 pytest-cov~=4.1.0
 pytest-recording~=0.12.2
-pytest~=7.3.1
+pytest~=7.4
 recommonmark~=0.7.1
 requests-mock~=1.11.0
-ruff==0.0.272
+ruff==0.0.275
 types-python-dateutil~=2.8.19
 types-requests~=2.31.0
 urllib3<2
 
 [dev:python_version < "3.11"]
 tomli~=2.0
 
@@ -34,13 +34,13 @@
 geopandas~=0.13.0
 geoviews~=1.9
 hvplot~=0.8.3
 ipykernel~=6.22
 ipython~=8.12
 jinja2<4.0
 matplotlib~=3.7.1
-myst-parser~=1.0.0
+myst-parser~=2.0
 nbsphinx~=0.9
 pydata-sphinx-theme~=0.13
 pygeoif~=1.0
 scipy~=1.10
 sphinxcontrib-fulltoc~=1.2
```

### Comparing `pystac-client-0.7.1/tests/test_cli.py` & `pystac-client-0.7.2/tests/test_cli.py`

 * *Files identical despite different names*

### Comparing `pystac-client-0.7.1/tests/test_client.py` & `pystac-client-0.7.2/tests/test_client.py`

 * *Files 0% similar despite different names*

```diff
@@ -678,7 +678,20 @@
         with pytest.warns(FallbackToPystac):
             next(client.get_collections())
 
         client.add_conforms_to("COLLECTIONS")
 
         with pytest.warns(MissingLink, match="rel='data'"):
             next(client.get_collections())
+
+
+@pytest.mark.vcr
+def test_collections_are_clients() -> None:
+    # https://github.com/stac-utils/pystac-client/issues/548
+    catalog = Client.open(
+        "https://planetarycomputer.microsoft.com/api/stac/v1/",
+    )
+    item = catalog.get_collection("cil-gdpcir-cc-by").get_item(
+        "cil-gdpcir-NUIST-NESM3-ssp585-r1i1p1f1-day"
+    )
+    assert item
+    item.get_collection()
```

### Comparing `pystac-client-0.7.1/tests/test_collection_client.py` & `pystac-client-0.7.2/tests/test_collection_client.py`

 * *Files identical despite different names*

### Comparing `pystac-client-0.7.1/tests/test_item_search.py` & `pystac-client-0.7.2/tests/test_item_search.py`

 * *Files identical despite different names*

### Comparing `pystac-client-0.7.1/tests/test_stac_api_io.py` & `pystac-client-0.7.2/tests/test_stac_api_io.py`

 * *Files identical despite different names*

