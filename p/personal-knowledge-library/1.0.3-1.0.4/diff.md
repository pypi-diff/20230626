# Comparing `tmp/personal_knowledge_library-1.0.3.tar.gz` & `tmp/personal_knowledge_library-1.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "personal_knowledge_library-1.0.3.tar", last modified: Sun Jun 18 18:20:38 2023, max compression
+gzip compressed data, was "personal_knowledge_library-1.0.4.tar", last modified: Mon Jun 26 07:14:31 2023, max compression
```

## Comparing `personal_knowledge_library-1.0.3.tar` & `personal_knowledge_library-1.0.4.tar`

### file list

```diff
@@ -1,44 +1,44 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-18 18:20:38.984197 personal_knowledge_library-1.0.3/
--rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-06-18 18:20:26.000000 personal_knowledge_library-1.0.3/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    44039 2023-06-18 18:20:38.984197 personal_knowledge_library-1.0.3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    43169 2023-06-18 18:20:26.000000 personal_knowledge_library-1.0.3/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-18 18:20:38.984197 personal_knowledge_library-1.0.3/knowledge/
--rw-r--r--   0 runner    (1001) docker     (123)     1417 2023-06-18 18:20:26.000000 personal_knowledge_library-1.0.3/knowledge/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-18 18:20:38.984197 personal_knowledge_library-1.0.3/knowledge/base/
--rw-r--r--   0 runner    (1001) docker     (123)      890 2023-06-18 18:20:26.000000 personal_knowledge_library-1.0.3/knowledge/base/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4429 2023-06-18 18:20:26.000000 personal_knowledge_library-1.0.3/knowledge/base/access.py
--rw-r--r--   0 runner    (1001) docker     (123)     7995 2023-06-18 18:20:26.000000 personal_knowledge_library-1.0.3/knowledge/base/entity.py
--rw-r--r--   0 runner    (1001) docker     (123)    79715 2023-06-18 18:20:26.000000 personal_knowledge_library-1.0.3/knowledge/base/ontology.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-18 18:20:38.984197 personal_knowledge_library-1.0.3/knowledge/nel/
--rw-r--r--   0 runner    (1001) docker     (123)      327 2023-06-18 18:20:26.000000 personal_knowledge_library-1.0.3/knowledge/nel/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    14503 2023-06-18 18:20:26.000000 personal_knowledge_library-1.0.3/knowledge/nel/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     5435 2023-06-18 18:20:26.000000 personal_knowledge_library-1.0.3/knowledge/nel/engine.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-18 18:20:38.984197 personal_knowledge_library-1.0.3/knowledge/ontomapping/
--rw-r--r--   0 runner    (1001) docker     (123)    17105 2023-06-18 18:20:26.000000 personal_knowledge_library-1.0.3/knowledge/ontomapping/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    11310 2023-06-18 18:20:26.000000 personal_knowledge_library-1.0.3/knowledge/ontomapping/manager.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-18 18:20:38.984197 personal_knowledge_library-1.0.3/knowledge/public/
--rw-r--r--   0 runner    (1001) docker     (123)      852 2023-06-18 18:20:26.000000 personal_knowledge_library-1.0.3/knowledge/public/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2831 2023-06-18 18:20:26.000000 personal_knowledge_library-1.0.3/knowledge/public/cache.py
--rw-r--r--   0 runner    (1001) docker     (123)    12240 2023-06-18 18:20:26.000000 personal_knowledge_library-1.0.3/knowledge/public/helper.py
--rw-r--r--   0 runner    (1001) docker     (123)     3006 2023-06-18 18:20:26.000000 personal_knowledge_library-1.0.3/knowledge/public/relations.py
--rw-r--r--   0 runner    (1001) docker     (123)    44912 2023-06-18 18:20:26.000000 personal_knowledge_library-1.0.3/knowledge/public/wikidata.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-18 18:20:38.984197 personal_knowledge_library-1.0.3/knowledge/services/
--rw-r--r--   0 runner    (1001) docker     (123)      531 2023-06-18 18:20:26.000000 personal_knowledge_library-1.0.3/knowledge/services/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     9002 2023-06-18 18:20:26.000000 personal_knowledge_library-1.0.3/knowledge/services/base.py
--rw-r--r--   0 runner    (1001) docker     (123)    52672 2023-06-18 18:20:26.000000 personal_knowledge_library-1.0.3/knowledge/services/graph.py
--rw-r--r--   0 runner    (1001) docker     (123)    20193 2023-06-18 18:20:26.000000 personal_knowledge_library-1.0.3/knowledge/services/group.py
--rw-r--r--   0 runner    (1001) docker     (123)    29652 2023-06-18 18:20:26.000000 personal_knowledge_library-1.0.3/knowledge/services/ontology.py
--rw-r--r--   0 runner    (1001) docker     (123)     4439 2023-06-18 18:20:26.000000 personal_knowledge_library-1.0.3/knowledge/services/tenant.py
--rw-r--r--   0 runner    (1001) docker     (123)    12696 2023-06-18 18:20:26.000000 personal_knowledge_library-1.0.3/knowledge/services/users.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-18 18:20:38.984197 personal_knowledge_library-1.0.3/knowledge/utils/
--rw-r--r--   0 runner    (1001) docker     (123)      192 2023-06-18 18:20:26.000000 personal_knowledge_library-1.0.3/knowledge/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6092 2023-06-18 18:20:26.000000 personal_knowledge_library-1.0.3/knowledge/utils/rdf.py
--rw-r--r--   0 runner    (1001) docker     (123)     5191 2023-06-18 18:20:26.000000 personal_knowledge_library-1.0.3/knowledge/utils/wikipedia.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-18 18:20:38.984197 personal_knowledge_library-1.0.3/personal_knowledge_library.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    44039 2023-06-18 18:20:38.000000 personal_knowledge_library-1.0.3/personal_knowledge_library.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      973 2023-06-18 18:20:38.000000 personal_knowledge_library-1.0.3/personal_knowledge_library.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-18 18:20:38.000000 personal_knowledge_library-1.0.3/personal_knowledge_library.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      110 2023-06-18 18:20:38.000000 personal_knowledge_library-1.0.3/personal_knowledge_library.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       10 2023-06-18 18:20:38.000000 personal_knowledge_library-1.0.3/personal_knowledge_library.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       79 2023-06-18 18:20:38.988197 personal_knowledge_library-1.0.3/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2446 2023-06-18 18:20:26.000000 personal_knowledge_library-1.0.3/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 07:14:31.745282 personal_knowledge_library-1.0.4/
+-rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-06-26 07:14:14.000000 personal_knowledge_library-1.0.4/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    44039 2023-06-26 07:14:31.745282 personal_knowledge_library-1.0.4/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    43169 2023-06-26 07:14:14.000000 personal_knowledge_library-1.0.4/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 07:14:31.741282 personal_knowledge_library-1.0.4/knowledge/
+-rw-r--r--   0 runner    (1001) docker     (123)     1417 2023-06-26 07:14:14.000000 personal_knowledge_library-1.0.4/knowledge/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 07:14:31.741282 personal_knowledge_library-1.0.4/knowledge/base/
+-rw-r--r--   0 runner    (1001) docker     (123)      890 2023-06-26 07:14:14.000000 personal_knowledge_library-1.0.4/knowledge/base/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4429 2023-06-26 07:14:14.000000 personal_knowledge_library-1.0.4/knowledge/base/access.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7995 2023-06-26 07:14:14.000000 personal_knowledge_library-1.0.4/knowledge/base/entity.py
+-rw-r--r--   0 runner    (1001) docker     (123)    80585 2023-06-26 07:14:14.000000 personal_knowledge_library-1.0.4/knowledge/base/ontology.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 07:14:31.741282 personal_knowledge_library-1.0.4/knowledge/nel/
+-rw-r--r--   0 runner    (1001) docker     (123)      327 2023-06-26 07:14:14.000000 personal_knowledge_library-1.0.4/knowledge/nel/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14503 2023-06-26 07:14:14.000000 personal_knowledge_library-1.0.4/knowledge/nel/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5435 2023-06-26 07:14:14.000000 personal_knowledge_library-1.0.4/knowledge/nel/engine.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 07:14:31.741282 personal_knowledge_library-1.0.4/knowledge/ontomapping/
+-rw-r--r--   0 runner    (1001) docker     (123)    17105 2023-06-26 07:14:14.000000 personal_knowledge_library-1.0.4/knowledge/ontomapping/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11310 2023-06-26 07:14:14.000000 personal_knowledge_library-1.0.4/knowledge/ontomapping/manager.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 07:14:31.741282 personal_knowledge_library-1.0.4/knowledge/public/
+-rw-r--r--   0 runner    (1001) docker     (123)      852 2023-06-26 07:14:14.000000 personal_knowledge_library-1.0.4/knowledge/public/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2831 2023-06-26 07:14:14.000000 personal_knowledge_library-1.0.4/knowledge/public/cache.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12240 2023-06-26 07:14:14.000000 personal_knowledge_library-1.0.4/knowledge/public/helper.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3006 2023-06-26 07:14:14.000000 personal_knowledge_library-1.0.4/knowledge/public/relations.py
+-rw-r--r--   0 runner    (1001) docker     (123)    44912 2023-06-26 07:14:14.000000 personal_knowledge_library-1.0.4/knowledge/public/wikidata.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 07:14:31.745282 personal_knowledge_library-1.0.4/knowledge/services/
+-rw-r--r--   0 runner    (1001) docker     (123)      531 2023-06-26 07:14:14.000000 personal_knowledge_library-1.0.4/knowledge/services/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9002 2023-06-26 07:14:14.000000 personal_knowledge_library-1.0.4/knowledge/services/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)    52734 2023-06-26 07:14:14.000000 personal_knowledge_library-1.0.4/knowledge/services/graph.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20193 2023-06-26 07:14:14.000000 personal_knowledge_library-1.0.4/knowledge/services/group.py
+-rw-r--r--   0 runner    (1001) docker     (123)    29652 2023-06-26 07:14:14.000000 personal_knowledge_library-1.0.4/knowledge/services/ontology.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4439 2023-06-26 07:14:14.000000 personal_knowledge_library-1.0.4/knowledge/services/tenant.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12696 2023-06-26 07:14:14.000000 personal_knowledge_library-1.0.4/knowledge/services/users.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 07:14:31.745282 personal_knowledge_library-1.0.4/knowledge/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)      192 2023-06-26 07:14:14.000000 personal_knowledge_library-1.0.4/knowledge/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6092 2023-06-26 07:14:14.000000 personal_knowledge_library-1.0.4/knowledge/utils/rdf.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5191 2023-06-26 07:14:14.000000 personal_knowledge_library-1.0.4/knowledge/utils/wikipedia.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 07:14:31.745282 personal_knowledge_library-1.0.4/personal_knowledge_library.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    44039 2023-06-26 07:14:31.000000 personal_knowledge_library-1.0.4/personal_knowledge_library.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      973 2023-06-26 07:14:31.000000 personal_knowledge_library-1.0.4/personal_knowledge_library.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-26 07:14:31.000000 personal_knowledge_library-1.0.4/personal_knowledge_library.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      110 2023-06-26 07:14:31.000000 personal_knowledge_library-1.0.4/personal_knowledge_library.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       10 2023-06-26 07:14:31.000000 personal_knowledge_library-1.0.4/personal_knowledge_library.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       79 2023-06-26 07:14:31.745282 personal_knowledge_library-1.0.4/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2446 2023-06-26 07:14:14.000000 personal_knowledge_library-1.0.4/setup.py
```

### Comparing `personal_knowledge_library-1.0.3/LICENSE` & `personal_knowledge_library-1.0.4/LICENSE`

 * *Files identical despite different names*

### Comparing `personal_knowledge_library-1.0.3/PKG-INFO` & `personal_knowledge_library-1.0.4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: personal_knowledge_library
-Version: 1.0.3
+Version: 1.0.4
 Summary: Library to access Wacom's Personal Knowledge graph.
 Home-page: https://github.com/Wacom-Developer/personal-knowledge-library
 Author: Markus Weber
 Author-email: markus.weber@wacom.com
 License: Apache 2.0 License
 Keywords: semantic-knowledge;knowledge-graph
 Platform: UNKNOWN
```

### Comparing `personal_knowledge_library-1.0.3/README.md` & `personal_knowledge_library-1.0.4/README.md`

 * *Files identical despite different names*

### Comparing `personal_knowledge_library-1.0.3/knowledge/__init__.py` & `personal_knowledge_library-1.0.4/knowledge/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -12,15 +12,15 @@
 __author__ = "Markus Weber"
 __copyright__ = "Copyright 2021-2023 Wacom. All rights reserved."
 __credits__ = ["Markus Weber"]
 __license__ = "Wacom"
 __maintainer__ = ["Markus Weber"]
 __email__ = "markus.weber@wacom.com"
 __status__ = "beta"
-__version__ = "1.0.3"
+__version__ = "1.0.4"
 
 # Create the Logger
 logger: Union[logging.Logger, None] = None
 
 if logger is None:
     logger = logging.getLogger(__name__)
     logger.setLevel(logging.DEBUG)
```

### Comparing `personal_knowledge_library-1.0.3/knowledge/base/__init__.py` & `personal_knowledge_library-1.0.4/knowledge/base/__init__.py`

 * *Files identical despite different names*

### Comparing `personal_knowledge_library-1.0.3/knowledge/base/access.py` & `personal_knowledge_library-1.0.4/knowledge/base/access.py`

 * *Files identical despite different names*

### Comparing `personal_knowledge_library-1.0.3/knowledge/base/entity.py` & `personal_knowledge_library-1.0.4/knowledge/base/entity.py`

 * *Files identical despite different names*

### Comparing `personal_knowledge_library-1.0.3/knowledge/base/ontology.py` & `personal_knowledge_library-1.0.4/knowledge/base/ontology.py`

 * *Files 1% similar despite different names*

```diff
@@ -1982,21 +1982,39 @@
         -------
         instance: ThingObject
             ThingObject that is created from the dict
         """
         labels: List[Label] = []
         alias: List[Label] = []
         descriptions: List[Description] = []
-
+        main_labels: Dict[str, bool] = {}
         for label in entity[LABELS_TAG]:
             if label[LOCALE_TAG] in SUPPORTED_LOCALES:
                 if label[IS_MAIN_TAG]:
-                    labels.append(Label.create_from_dict(label))
+                    main_label: Label = Label.create_from_dict(label)
+                    main_labels[label[LOCALE_TAG]] = True
+                    labels.append(main_label)
                 else:
-                    alias.append(Label.create_from_dict(label))
+                    alias_label: Label = Label.create_from_dict(label)
+                    if alias_label.language_code not in main_labels:
+                        main_labels[alias_label.language_code] = False
+                    alias.append(alias_label)
+        for lang_code, is_main in main_labels.items():
+            if not is_main:
+                la_idx: int = 0
+                while la_idx < len(alias):
+                    # Fix things where there is no main label
+                    if alias[la_idx].language_code == lang_code:
+                        al: Label = alias[la_idx]
+                        labels.append(Label(al.content, al.language_code, main=True))
+                        del alias[la_idx]
+                    else:
+                        la_idx += 1
+
+
 
         for desc in entity[DESCRIPTIONS_TAG]:
             if desc[LOCALE_TAG] in SUPPORTED_LOCALES:
                 descriptions.append(Description.create_from_dict(desc))
 
         use_nel: bool = entity.get(USE_NEL_TAG, True)
```

### Comparing `personal_knowledge_library-1.0.3/knowledge/nel/base.py` & `personal_knowledge_library-1.0.4/knowledge/nel/base.py`

 * *Files identical despite different names*

### Comparing `personal_knowledge_library-1.0.3/knowledge/nel/engine.py` & `personal_knowledge_library-1.0.4/knowledge/nel/engine.py`

 * *Files identical despite different names*

### Comparing `personal_knowledge_library-1.0.3/knowledge/ontomapping/__init__.py` & `personal_knowledge_library-1.0.4/knowledge/ontomapping/__init__.py`

 * *Files identical despite different names*

### Comparing `personal_knowledge_library-1.0.3/knowledge/ontomapping/manager.py` & `personal_knowledge_library-1.0.4/knowledge/ontomapping/manager.py`

 * *Files identical despite different names*

### Comparing `personal_knowledge_library-1.0.3/knowledge/public/__init__.py` & `personal_knowledge_library-1.0.4/knowledge/public/__init__.py`

 * *Files identical despite different names*

### Comparing `personal_knowledge_library-1.0.3/knowledge/public/cache.py` & `personal_knowledge_library-1.0.4/knowledge/public/cache.py`

 * *Files identical despite different names*

### Comparing `personal_knowledge_library-1.0.3/knowledge/public/helper.py` & `personal_knowledge_library-1.0.4/knowledge/public/helper.py`

 * *Files identical despite different names*

### Comparing `personal_knowledge_library-1.0.3/knowledge/public/relations.py` & `personal_knowledge_library-1.0.4/knowledge/public/relations.py`

 * *Files identical despite different names*

### Comparing `personal_knowledge_library-1.0.3/knowledge/public/wikidata.py` & `personal_knowledge_library-1.0.4/knowledge/public/wikidata.py`

 * *Files identical despite different names*

### Comparing `personal_knowledge_library-1.0.3/knowledge/services/__init__.py` & `personal_knowledge_library-1.0.4/knowledge/services/__init__.py`

 * *Files identical despite different names*

### Comparing `personal_knowledge_library-1.0.3/knowledge/services/base.py` & `personal_knowledge_library-1.0.4/knowledge/services/base.py`

 * *Files identical despite different names*

### Comparing `personal_knowledge_library-1.0.3/knowledge/services/graph.py` & `personal_knowledge_library-1.0.4/knowledge/services/graph.py`

 * *Files 0% similar despite different names*

```diff
@@ -183,14 +183,15 @@
             # Create ThingObject
             thing: ThingObject = ThingObject(label=pref_label, icon=e[IMAGE_TAG],
                                              description=[Description.create_from_dict(d) for d in e[DESCRIPTIONS_TAG]],
                                              concept_type=OntologyClassReference.parse(e[TYPE_TAG]),
                                              uri=e[URI_TAG])
             thing.group_ids = e.get(GROUP_IDS_TAG, [])
             thing.owner_id = e.get(OWNER_ID_TAG)
+            thing.use_for_nel = e.get(SEND_TO_NEL_TAG, False)
             # Set the alias
             thing.alias = aliases
             # Configure data properties
             if DATA_PROPERTIES_TAG in e:
                 for data_property in e[DATA_PROPERTIES_TAG]:
                     data_property_type: OntologyPropertyReference = \
                         OntologyPropertyReference.parse(data_property[DATA_PROPERTY_TAG])
```

### Comparing `personal_knowledge_library-1.0.3/knowledge/services/group.py` & `personal_knowledge_library-1.0.4/knowledge/services/group.py`

 * *Files identical despite different names*

### Comparing `personal_knowledge_library-1.0.3/knowledge/services/ontology.py` & `personal_knowledge_library-1.0.4/knowledge/services/ontology.py`

 * *Files identical despite different names*

### Comparing `personal_knowledge_library-1.0.3/knowledge/services/tenant.py` & `personal_knowledge_library-1.0.4/knowledge/services/tenant.py`

 * *Files identical despite different names*

### Comparing `personal_knowledge_library-1.0.3/knowledge/services/users.py` & `personal_knowledge_library-1.0.4/knowledge/services/users.py`

 * *Files identical despite different names*

### Comparing `personal_knowledge_library-1.0.3/knowledge/utils/rdf.py` & `personal_knowledge_library-1.0.4/knowledge/utils/rdf.py`

 * *Files identical despite different names*

### Comparing `personal_knowledge_library-1.0.3/knowledge/utils/wikipedia.py` & `personal_knowledge_library-1.0.4/knowledge/utils/wikipedia.py`

 * *Files identical despite different names*

### Comparing `personal_knowledge_library-1.0.3/personal_knowledge_library.egg-info/PKG-INFO` & `personal_knowledge_library-1.0.4/personal_knowledge_library.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: personal-knowledge-library
-Version: 1.0.3
+Version: 1.0.4
 Summary: Library to access Wacom's Personal Knowledge graph.
 Home-page: https://github.com/Wacom-Developer/personal-knowledge-library
 Author: Markus Weber
 Author-email: markus.weber@wacom.com
 License: Apache 2.0 License
 Keywords: semantic-knowledge;knowledge-graph
 Platform: UNKNOWN
```

### Comparing `personal_knowledge_library-1.0.3/personal_knowledge_library.egg-info/SOURCES.txt` & `personal_knowledge_library-1.0.4/personal_knowledge_library.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `personal_knowledge_library-1.0.3/setup.py` & `personal_knowledge_library-1.0.4/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -22,15 +22,15 @@
 an older version of knowledge-service-lib :
     $ python -m pip install personal-knowledge-library
 """)
     sys.exit(1)
 
 # The directory containing this file
 HERE = pathlib.Path(__file__).parent
-__version__ = "1.0.3"
+__version__ = "1.0.4"
 
 # The text of the README file
 README = (HERE / "README.md").read_text()
 
 # the setup
 setup(
     name='personal_knowledge_library',
```

