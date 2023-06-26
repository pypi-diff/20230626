# Comparing `tmp/hydrusvideodeduplicator-0.1.7.tar.gz` & `tmp/hydrusvideodeduplicator-0.1.8.tar.gz`

## Comparing `hydrusvideodeduplicator-0.1.7.tar` & `hydrusvideodeduplicator-0.1.8.tar`

### file list

```diff
@@ -1,22 +1,22 @@
--rw-r--r--   0        0        0     4891 2020-02-02 00:00:00.000000 hydrusvideodeduplicator-0.1.7/src/hydrusvideodeduplicator/README.md
--rw-r--r--   0        0        0      119 2020-02-02 00:00:00.000000 hydrusvideodeduplicator-0.1.7/src/hydrusvideodeduplicator/__about__.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 hydrusvideodeduplicator-0.1.7/src/hydrusvideodeduplicator/__init__.py
--rw-r--r--   0        0        0     4852 2020-02-02 00:00:00.000000 hydrusvideodeduplicator-0.1.7/src/hydrusvideodeduplicator/__main__.py
--rw-r--r--   0        0        0     1106 2020-02-02 00:00:00.000000 hydrusvideodeduplicator-0.1.7/src/hydrusvideodeduplicator/config.py
--rw-r--r--   0        0        0    13565 2020-02-02 00:00:00.000000 hydrusvideodeduplicator-0.1.7/src/hydrusvideodeduplicator/dedup.py
--rw-r--r--   0        0        0     4036 2020-02-02 00:00:00.000000 hydrusvideodeduplicator-0.1.7/src/hydrusvideodeduplicator/dedup_util.py
--rw-r--r--   0        0        0     1663 2020-02-02 00:00:00.000000 hydrusvideodeduplicator-0.1.7/src/hydrusvideodeduplicator/pdq_utils.py
--rw-r--r--   0        0        0     2632 2020-02-02 00:00:00.000000 hydrusvideodeduplicator-0.1.7/src/hydrusvideodeduplicator/vpdq.py
--rw-r--r--   0        0        0     2350 2020-02-02 00:00:00.000000 hydrusvideodeduplicator-0.1.7/src/hydrusvideodeduplicator/vpdq_brute_matcher.py
--rw-r--r--   0        0        0     3638 2020-02-02 00:00:00.000000 hydrusvideodeduplicator-0.1.7/src/hydrusvideodeduplicator/vpdq_faiss.py
--rw-r--r--   0        0        0     5565 2020-02-02 00:00:00.000000 hydrusvideodeduplicator-0.1.7/src/hydrusvideodeduplicator/vpdq_util.py
--rw-r--r--   0        0        0    34519 2020-02-02 00:00:00.000000 hydrusvideodeduplicator-0.1.7/src/hydrusvideodeduplicator/hydrus_api/LICENSE
--rw-r--r--   0        0        0      160 2020-02-02 00:00:00.000000 hydrusvideodeduplicator-0.1.7/src/hydrusvideodeduplicator/hydrus_api/README.md
--rw-r--r--   0        0        0    36568 2020-02-02 00:00:00.000000 hydrusvideodeduplicator-0.1.7/src/hydrusvideodeduplicator/hydrus_api/__init__.py
--rw-r--r--   0        0        0     5261 2020-02-02 00:00:00.000000 hydrusvideodeduplicator-0.1.7/src/hydrusvideodeduplicator/hydrus_api/utils.py
--rw-r--r--   0        0        0       97 2020-02-02 00:00:00.000000 hydrusvideodeduplicator-0.1.7/tests/__init__.py
--rw-r--r--   0        0        0     3127 2020-02-02 00:00:00.000000 hydrusvideodeduplicator-0.1.7/.gitignore
--rw-r--r--   0        0        0     1078 2020-02-02 00:00:00.000000 hydrusvideodeduplicator-0.1.7/LICENSE
--rw-r--r--   0        0        0     2348 2020-02-02 00:00:00.000000 hydrusvideodeduplicator-0.1.7/README.md
--rw-r--r--   0        0        0     3496 2020-02-02 00:00:00.000000 hydrusvideodeduplicator-0.1.7/pyproject.toml
--rw-r--r--   0        0        0     3378 2020-02-02 00:00:00.000000 hydrusvideodeduplicator-0.1.7/PKG-INFO
+-rw-r--r--   0        0        0     4891 2020-02-02 00:00:00.000000 hydrusvideodeduplicator-0.1.8/src/hydrusvideodeduplicator/README.md
+-rw-r--r--   0        0        0      119 2020-02-02 00:00:00.000000 hydrusvideodeduplicator-0.1.8/src/hydrusvideodeduplicator/__about__.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 hydrusvideodeduplicator-0.1.8/src/hydrusvideodeduplicator/__init__.py
+-rw-r--r--   0        0        0     4852 2020-02-02 00:00:00.000000 hydrusvideodeduplicator-0.1.8/src/hydrusvideodeduplicator/__main__.py
+-rw-r--r--   0        0        0     1106 2020-02-02 00:00:00.000000 hydrusvideodeduplicator-0.1.8/src/hydrusvideodeduplicator/config.py
+-rw-r--r--   0        0        0    13565 2020-02-02 00:00:00.000000 hydrusvideodeduplicator-0.1.8/src/hydrusvideodeduplicator/dedup.py
+-rw-r--r--   0        0        0     4036 2020-02-02 00:00:00.000000 hydrusvideodeduplicator-0.1.8/src/hydrusvideodeduplicator/dedup_util.py
+-rw-r--r--   0        0        0     1663 2020-02-02 00:00:00.000000 hydrusvideodeduplicator-0.1.8/src/hydrusvideodeduplicator/pdq_utils.py
+-rw-r--r--   0        0        0     2632 2020-02-02 00:00:00.000000 hydrusvideodeduplicator-0.1.8/src/hydrusvideodeduplicator/vpdq.py
+-rw-r--r--   0        0        0     2497 2020-02-02 00:00:00.000000 hydrusvideodeduplicator-0.1.8/src/hydrusvideodeduplicator/vpdq_brute_matcher.py
+-rw-r--r--   0        0        0     3638 2020-02-02 00:00:00.000000 hydrusvideodeduplicator-0.1.8/src/hydrusvideodeduplicator/vpdq_faiss.py
+-rw-r--r--   0        0        0     5565 2020-02-02 00:00:00.000000 hydrusvideodeduplicator-0.1.8/src/hydrusvideodeduplicator/vpdq_util.py
+-rw-r--r--   0        0        0    34519 2020-02-02 00:00:00.000000 hydrusvideodeduplicator-0.1.8/src/hydrusvideodeduplicator/hydrus_api/LICENSE
+-rw-r--r--   0        0        0      160 2020-02-02 00:00:00.000000 hydrusvideodeduplicator-0.1.8/src/hydrusvideodeduplicator/hydrus_api/README.md
+-rw-r--r--   0        0        0    36568 2020-02-02 00:00:00.000000 hydrusvideodeduplicator-0.1.8/src/hydrusvideodeduplicator/hydrus_api/__init__.py
+-rw-r--r--   0        0        0     5261 2020-02-02 00:00:00.000000 hydrusvideodeduplicator-0.1.8/src/hydrusvideodeduplicator/hydrus_api/utils.py
+-rw-r--r--   0        0        0       97 2020-02-02 00:00:00.000000 hydrusvideodeduplicator-0.1.8/tests/__init__.py
+-rw-r--r--   0        0        0     3127 2020-02-02 00:00:00.000000 hydrusvideodeduplicator-0.1.8/.gitignore
+-rw-r--r--   0        0        0     1078 2020-02-02 00:00:00.000000 hydrusvideodeduplicator-0.1.8/LICENSE
+-rw-r--r--   0        0        0     2348 2020-02-02 00:00:00.000000 hydrusvideodeduplicator-0.1.8/README.md
+-rw-r--r--   0        0        0     3496 2020-02-02 00:00:00.000000 hydrusvideodeduplicator-0.1.8/pyproject.toml
+-rw-r--r--   0        0        0     3378 2020-02-02 00:00:00.000000 hydrusvideodeduplicator-0.1.8/PKG-INFO
```

### Comparing `hydrusvideodeduplicator-0.1.7/src/hydrusvideodeduplicator/README.md` & `hydrusvideodeduplicator-0.1.8/src/hydrusvideodeduplicator/README.md`

 * *Files identical despite different names*

### Comparing `hydrusvideodeduplicator-0.1.7/src/hydrusvideodeduplicator/__main__.py` & `hydrusvideodeduplicator-0.1.8/src/hydrusvideodeduplicator/__main__.py`

 * *Files identical despite different names*

### Comparing `hydrusvideodeduplicator-0.1.7/src/hydrusvideodeduplicator/config.py` & `hydrusvideodeduplicator-0.1.8/src/hydrusvideodeduplicator/config.py`

 * *Files identical despite different names*

### Comparing `hydrusvideodeduplicator-0.1.7/src/hydrusvideodeduplicator/dedup.py` & `hydrusvideodeduplicator-0.1.8/src/hydrusvideodeduplicator/dedup.py`

 * *Files identical despite different names*

### Comparing `hydrusvideodeduplicator-0.1.7/src/hydrusvideodeduplicator/dedup_util.py` & `hydrusvideodeduplicator-0.1.8/src/hydrusvideodeduplicator/dedup_util.py`

 * *Files identical despite different names*

### Comparing `hydrusvideodeduplicator-0.1.7/src/hydrusvideodeduplicator/pdq_utils.py` & `hydrusvideodeduplicator-0.1.8/src/hydrusvideodeduplicator/pdq_utils.py`

 * *Files identical despite different names*

### Comparing `hydrusvideodeduplicator-0.1.7/src/hydrusvideodeduplicator/vpdq.py` & `hydrusvideodeduplicator-0.1.8/src/hydrusvideodeduplicator/vpdq.py`

 * *Files identical despite different names*

### Comparing `hydrusvideodeduplicator-0.1.7/src/hydrusvideodeduplicator/vpdq_brute_matcher.py` & `hydrusvideodeduplicator-0.1.8/src/hydrusvideodeduplicator/vpdq_brute_matcher.py`

 * *Files 5% similar despite different names*

```diff
@@ -57,11 +57,16 @@
     filtered_compared = quality_filter(dedupe(compared_hash), quality_tolerance)
     query_match_cnt = match_VPDQ_in_another(
         filtered_query, filtered_compared, distance_tolerance
     )
     compared_match_cnt = match_VPDQ_in_another(
         filtered_compared, filtered_query, distance_tolerance
     )
+
+    # TODO: Why does this sometimes happen?
+    if len(filtered_query) == 0 or len(filtered_compared) == 0:
+        return VPDQMatchResult(0, 0)
+
     return VPDQMatchResult(
         query_match_cnt * 100 / len(filtered_query),
         compared_match_cnt * 100 / len(filtered_compared),
     )
```

### Comparing `hydrusvideodeduplicator-0.1.7/src/hydrusvideodeduplicator/vpdq_faiss.py` & `hydrusvideodeduplicator-0.1.8/src/hydrusvideodeduplicator/vpdq_faiss.py`

 * *Files identical despite different names*

### Comparing `hydrusvideodeduplicator-0.1.7/src/hydrusvideodeduplicator/vpdq_util.py` & `hydrusvideodeduplicator-0.1.8/src/hydrusvideodeduplicator/vpdq_util.py`

 * *Files identical despite different names*

### Comparing `hydrusvideodeduplicator-0.1.7/src/hydrusvideodeduplicator/hydrus_api/LICENSE` & `hydrusvideodeduplicator-0.1.8/src/hydrusvideodeduplicator/hydrus_api/LICENSE`

 * *Files identical despite different names*

### Comparing `hydrusvideodeduplicator-0.1.7/src/hydrusvideodeduplicator/hydrus_api/__init__.py` & `hydrusvideodeduplicator-0.1.8/src/hydrusvideodeduplicator/hydrus_api/__init__.py`

 * *Files identical despite different names*

### Comparing `hydrusvideodeduplicator-0.1.7/src/hydrusvideodeduplicator/hydrus_api/utils.py` & `hydrusvideodeduplicator-0.1.8/src/hydrusvideodeduplicator/hydrus_api/utils.py`

 * *Files identical despite different names*

### Comparing `hydrusvideodeduplicator-0.1.7/.gitignore` & `hydrusvideodeduplicator-0.1.8/.gitignore`

 * *Files identical despite different names*

### Comparing `hydrusvideodeduplicator-0.1.7/LICENSE` & `hydrusvideodeduplicator-0.1.8/LICENSE`

 * *Files identical despite different names*

### Comparing `hydrusvideodeduplicator-0.1.7/README.md` & `hydrusvideodeduplicator-0.1.8/README.md`

 * *Files identical despite different names*

### Comparing `hydrusvideodeduplicator-0.1.7/pyproject.toml` & `hydrusvideodeduplicator-0.1.8/pyproject.toml`

 * *Files identical despite different names*

### Comparing `hydrusvideodeduplicator-0.1.7/PKG-INFO` & `hydrusvideodeduplicator-0.1.8/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: hydrusvideodeduplicator
-Version: 0.1.7
+Version: 0.1.8
 Summary: Video deduplicator utility for Hydrus Network
 Project-URL: Documentation, https://github.com/appleappleapplenanner/hydrus-video-deduplicator#readme
 Project-URL: Issues, https://github.com/appleappleapplenanner/hydrus-video-deduplicator/issues
 Project-URL: Source, https://github.com/appleappleapplenanner/hydrus-video-deduplicator
 Author: appleappleapplenanner
 License-Expression: MIT
 License-File: LICENSE
```

