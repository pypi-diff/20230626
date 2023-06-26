# Comparing `tmp/recon_lw-2.0.0.dev5347019501.tar.gz` & `tmp/recon_lw-2.0.0.dev5376000103.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/recon_lw-2.0.0.dev5347019501.tar", last modified: Thu Jun 22 14:51:29 2023, max compression
+gzip compressed data, was "dist/recon_lw-2.0.0.dev5376000103.tar", last modified: Mon Jun 26 08:40:13 2023, max compression
```

## Comparing `recon_lw-2.0.0.dev5347019501.tar` & `recon_lw-2.0.0.dev5376000103.tar`

### file list

```diff
@@ -1,28 +1,28 @@
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-22 14:51:29.000000 recon_lw-2.0.0.dev5347019501/
--rw-r--r--   0 runner    (1001) docker     (122)       69 2023-06-22 14:50:39.000000 recon_lw-2.0.0.dev5347019501/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (122)      294 2023-06-22 14:51:29.000000 recon_lw-2.0.0.dev5347019501/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (122)       10 2023-06-22 14:50:39.000000 recon_lw-2.0.0.dev5347019501/README.md
--rw-r--r--   0 runner    (1001) docker     (122)       76 2023-06-22 14:51:04.000000 recon_lw-2.0.0.dev5347019501/package_info.json
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-22 14:51:29.000000 recon_lw-2.0.0.dev5347019501/recon_lw/
--rw-r--r--   0 runner    (1001) docker     (122)     1908 2023-06-22 14:50:39.000000 recon_lw-2.0.0.dev5347019501/recon_lw/EventsSaver.py
--rw-r--r--   0 runner    (1001) docker     (122)     4937 2023-06-22 14:50:39.000000 recon_lw-2.0.0.dev5347019501/recon_lw/LastStateMatcher.py
--rw-r--r--   0 runner    (1001) docker     (122)     2507 2023-06-22 14:50:39.000000 recon_lw-2.0.0.dev5347019501/recon_lw/LiveObjectsCache.py
--rw-r--r--   0 runner    (1001) docker     (122)     2916 2023-06-22 14:50:39.000000 recon_lw-2.0.0.dev5347019501/recon_lw/SequenceCache.py
--rw-r--r--   0 runner    (1001) docker     (122)     1108 2023-06-22 14:50:39.000000 recon_lw-2.0.0.dev5347019501/recon_lw/StateSequenceGenerator.py
--rw-r--r--   0 runner    (1001) docker     (122)     3716 2023-06-22 14:50:39.000000 recon_lw-2.0.0.dev5347019501/recon_lw/TimeCacheMatcher.py
--rw-r--r--   0 runner    (1001) docker     (122)        5 2023-06-22 14:50:39.000000 recon_lw-2.0.0.dev5347019501/recon_lw/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)    13503 2023-06-22 14:50:39.000000 recon_lw-2.0.0.dev5347019501/recon_lw/recon_lw.py
--rw-r--r--   0 runner    (1001) docker     (122)    33393 2023-06-22 14:50:39.000000 recon_lw-2.0.0.dev5347019501/recon_lw/recon_ob.py
--rw-r--r--   0 runner    (1001) docker     (122)    22143 2023-06-22 14:50:39.000000 recon_lw-2.0.0.dev5347019501/recon_lw/recon_ob_cross_stream.py
--rw-r--r--   0 runner    (1001) docker     (122)     6293 2023-06-22 14:50:39.000000 recon_lw-2.0.0.dev5347019501/recon_lw/recon_ob_stats.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-22 14:51:29.000000 recon_lw-2.0.0.dev5347019501/recon_lw.egg-info/
--rw-r--r--   0 runner    (1001) docker     (122)      294 2023-06-22 14:51:29.000000 recon_lw-2.0.0.dev5347019501/recon_lw.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (122)      542 2023-06-22 14:51:29.000000 recon_lw-2.0.0.dev5347019501/recon_lw.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (122)        1 2023-06-22 14:51:29.000000 recon_lw-2.0.0.dev5347019501/recon_lw.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (122)      219 2023-06-22 14:51:29.000000 recon_lw-2.0.0.dev5347019501/recon_lw.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (122)        9 2023-06-22 14:51:29.000000 recon_lw-2.0.0.dev5347019501/recon_lw.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (122)      275 2023-06-22 14:50:39.000000 recon_lw-2.0.0.dev5347019501/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (122)       38 2023-06-22 14:51:29.000000 recon_lw-2.0.0.dev5347019501/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (122)     1582 2023-06-22 14:50:39.000000 recon_lw-2.0.0.dev5347019501/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-22 14:51:29.000000 recon_lw-2.0.0.dev5347019501/test/
--rw-r--r--   0 runner    (1001) docker     (122)     4050 2023-06-22 14:50:39.000000 recon_lw-2.0.0.dev5347019501/test/test_recon_ob.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-26 08:40:13.000000 recon_lw-2.0.0.dev5376000103/
+-rw-r--r--   0 runner    (1001) docker     (122)       69 2023-06-26 08:39:21.000000 recon_lw-2.0.0.dev5376000103/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (122)      294 2023-06-26 08:40:13.000000 recon_lw-2.0.0.dev5376000103/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (122)       10 2023-06-26 08:39:21.000000 recon_lw-2.0.0.dev5376000103/README.md
+-rw-r--r--   0 runner    (1001) docker     (122)       76 2023-06-26 08:39:47.000000 recon_lw-2.0.0.dev5376000103/package_info.json
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-26 08:40:13.000000 recon_lw-2.0.0.dev5376000103/recon_lw/
+-rw-r--r--   0 runner    (1001) docker     (122)     1908 2023-06-26 08:39:21.000000 recon_lw-2.0.0.dev5376000103/recon_lw/EventsSaver.py
+-rw-r--r--   0 runner    (1001) docker     (122)     4937 2023-06-26 08:39:21.000000 recon_lw-2.0.0.dev5376000103/recon_lw/LastStateMatcher.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2507 2023-06-26 08:39:21.000000 recon_lw-2.0.0.dev5376000103/recon_lw/LiveObjectsCache.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2916 2023-06-26 08:39:21.000000 recon_lw-2.0.0.dev5376000103/recon_lw/SequenceCache.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1108 2023-06-26 08:39:21.000000 recon_lw-2.0.0.dev5376000103/recon_lw/StateSequenceGenerator.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3716 2023-06-26 08:39:21.000000 recon_lw-2.0.0.dev5376000103/recon_lw/TimeCacheMatcher.py
+-rw-r--r--   0 runner    (1001) docker     (122)        5 2023-06-26 08:39:21.000000 recon_lw-2.0.0.dev5376000103/recon_lw/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)    13503 2023-06-26 08:39:21.000000 recon_lw-2.0.0.dev5376000103/recon_lw/recon_lw.py
+-rw-r--r--   0 runner    (1001) docker     (122)    33427 2023-06-26 08:39:21.000000 recon_lw-2.0.0.dev5376000103/recon_lw/recon_ob.py
+-rw-r--r--   0 runner    (1001) docker     (122)    22143 2023-06-26 08:39:21.000000 recon_lw-2.0.0.dev5376000103/recon_lw/recon_ob_cross_stream.py
+-rw-r--r--   0 runner    (1001) docker     (122)     6293 2023-06-26 08:39:21.000000 recon_lw-2.0.0.dev5376000103/recon_lw/recon_ob_stats.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-26 08:40:13.000000 recon_lw-2.0.0.dev5376000103/recon_lw.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (122)      294 2023-06-26 08:40:13.000000 recon_lw-2.0.0.dev5376000103/recon_lw.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (122)      542 2023-06-26 08:40:13.000000 recon_lw-2.0.0.dev5376000103/recon_lw.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (122)        1 2023-06-26 08:40:13.000000 recon_lw-2.0.0.dev5376000103/recon_lw.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (122)      219 2023-06-26 08:40:13.000000 recon_lw-2.0.0.dev5376000103/recon_lw.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (122)        9 2023-06-26 08:40:13.000000 recon_lw-2.0.0.dev5376000103/recon_lw.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (122)      275 2023-06-26 08:39:21.000000 recon_lw-2.0.0.dev5376000103/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (122)       38 2023-06-26 08:40:13.000000 recon_lw-2.0.0.dev5376000103/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (122)     1582 2023-06-26 08:39:21.000000 recon_lw-2.0.0.dev5376000103/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-26 08:40:13.000000 recon_lw-2.0.0.dev5376000103/test/
+-rw-r--r--   0 runner    (1001) docker     (122)     4050 2023-06-26 08:39:21.000000 recon_lw-2.0.0.dev5376000103/test/test_recon_ob.py
```

### Comparing `recon_lw-2.0.0.dev5347019501/recon_lw/EventsSaver.py` & `recon_lw-2.0.0.dev5376000103/recon_lw/EventsSaver.py`

 * *Files identical despite different names*

### Comparing `recon_lw-2.0.0.dev5347019501/recon_lw/LastStateMatcher.py` & `recon_lw-2.0.0.dev5376000103/recon_lw/LastStateMatcher.py`

 * *Files identical despite different names*

### Comparing `recon_lw-2.0.0.dev5347019501/recon_lw/LiveObjectsCache.py` & `recon_lw-2.0.0.dev5376000103/recon_lw/LiveObjectsCache.py`

 * *Files identical despite different names*

### Comparing `recon_lw-2.0.0.dev5347019501/recon_lw/SequenceCache.py` & `recon_lw-2.0.0.dev5376000103/recon_lw/SequenceCache.py`

 * *Files identical despite different names*

### Comparing `recon_lw-2.0.0.dev5347019501/recon_lw/StateSequenceGenerator.py` & `recon_lw-2.0.0.dev5376000103/recon_lw/StateSequenceGenerator.py`

 * *Files identical despite different names*

### Comparing `recon_lw-2.0.0.dev5347019501/recon_lw/TimeCacheMatcher.py` & `recon_lw-2.0.0.dev5376000103/recon_lw/TimeCacheMatcher.py`

 * *Files identical despite different names*

### Comparing `recon_lw-2.0.0.dev5347019501/recon_lw/recon_lw.py` & `recon_lw-2.0.0.dev5376000103/recon_lw/recon_lw.py`

 * *Files identical despite different names*

### Comparing `recon_lw-2.0.0.dev5347019501/recon_lw/recon_ob.py` & `recon_lw-2.0.0.dev5376000103/recon_lw/recon_ob.py`

 * *Files 1% similar despite different names*

```diff
@@ -500,18 +500,18 @@
     result_body = {}
     side_key = side + "_aggr"
     del_index = level - 1
     if not 0 <= del_index < len(order_book[side_key]):
         result_body["error"] = "Unexpected level {0}, against existing {1} levels on {2} side".format(level,
                                                                                                       len(order_book[side_key]),
                                                                                                       side_key)
-
+        return result_body, []
+    
     #is it purely implied
     order_book["implied_only"] = (order_book[side_key][del_index]["real_num_orders"] == 0)
-
     order_book[side_key].pop(del_index)
 
     order_book["aggr_seq"]["top_delta"] = (del_index == 0)
     update_time_and_version(str_time_of_event, order_book)
     order_book["aggr_seq"]["limit_delta"] = 1
 
     return {}, [copy.deepcopy(order_book)]
```

### Comparing `recon_lw-2.0.0.dev5347019501/recon_lw/recon_ob_cross_stream.py` & `recon_lw-2.0.0.dev5376000103/recon_lw/recon_ob_cross_stream.py`

 * *Files identical despite different names*

### Comparing `recon_lw-2.0.0.dev5347019501/recon_lw/recon_ob_stats.py` & `recon_lw-2.0.0.dev5376000103/recon_lw/recon_ob_stats.py`

 * *Files identical despite different names*

### Comparing `recon_lw-2.0.0.dev5347019501/recon_lw.egg-info/SOURCES.txt` & `recon_lw-2.0.0.dev5376000103/recon_lw.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `recon_lw-2.0.0.dev5347019501/setup.py` & `recon_lw-2.0.0.dev5376000103/setup.py`

 * *Files identical despite different names*

### Comparing `recon_lw-2.0.0.dev5347019501/test/test_recon_ob.py` & `recon_lw-2.0.0.dev5376000103/test/test_recon_ob.py`

 * *Files identical despite different names*

