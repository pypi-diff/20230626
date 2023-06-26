# Comparing `tmp/HawaData-0.7.4.tar.gz` & `tmp/HawaData-0.7.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "HawaData-0.7.4.tar", last modified: Mon Jun 26 01:37:44 2023, max compression
+gzip compressed data, was "HawaData-0.7.5.tar", last modified: Mon Jun 26 01:40:10 2023, max compression
```

## Comparing `HawaData-0.7.4.tar` & `HawaData-0.7.5.tar`

### file list

```diff
@@ -1,37 +1,37 @@
-drwxr-xr-x   0 wangzhou   (501) staff       (20)        0 2023-06-26 01:37:44.871918 HawaData-0.7.4/
-drwxr-xr-x   0 wangzhou   (501) staff       (20)        0 2023-06-26 01:37:44.857112 HawaData-0.7.4/HawaData.egg-info/
--rw-r--r--   0 wangzhou   (501) staff       (20)     3111 2023-06-26 01:37:44.000000 HawaData-0.7.4/HawaData.egg-info/PKG-INFO
--rw-r--r--   0 wangzhou   (501) staff       (20)      562 2023-06-26 01:37:44.000000 HawaData-0.7.4/HawaData.egg-info/SOURCES.txt
--rw-r--r--   0 wangzhou   (501) staff       (20)        1 2023-06-26 01:37:44.000000 HawaData-0.7.4/HawaData.egg-info/dependency_links.txt
--rw-r--r--   0 wangzhou   (501) staff       (20)        5 2023-06-26 01:37:44.000000 HawaData-0.7.4/HawaData.egg-info/top_level.txt
--rw-r--r--   0 wangzhou   (501) staff       (20)     3111 2023-06-26 01:37:44.871612 HawaData-0.7.4/PKG-INFO
--rw-r--r--   0 wangzhou   (501) staff       (20)      669 2022-12-02 07:10:45.000000 HawaData-0.7.4/README.md
-drwxr-xr-x   0 wangzhou   (501) staff       (20)        0 2023-06-26 01:37:44.858002 HawaData-0.7.4/hawa/
--rw-r--r--   0 wangzhou   (501) staff       (20)        0 2022-11-30 09:39:05.000000 HawaData-0.7.4/hawa/__init__.py
-drwxr-xr-x   0 wangzhou   (501) staff       (20)        0 2023-06-26 01:37:44.861171 HawaData-0.7.4/hawa/base/
--rw-r--r--   0 wangzhou   (501) staff       (20)        0 2022-12-01 05:35:03.000000 HawaData-0.7.4/hawa/base/__init__.py
--rw-r--r--   0 wangzhou   (501) staff       (20)     2627 2023-06-19 08:54:42.000000 HawaData-0.7.4/hawa/base/db.py
--rw-r--r--   0 wangzhou   (501) staff       (20)      173 2022-12-01 06:05:08.000000 HawaData-0.7.4/hawa/base/decos.py
--rw-r--r--   0 wangzhou   (501) staff       (20)       98 2023-05-24 07:06:51.000000 HawaData-0.7.4/hawa/base/errors.py
--rw-r--r--   0 wangzhou   (501) staff       (20)      845 2022-12-02 03:09:07.000000 HawaData-0.7.4/hawa/base/init.py
-drwxr-xr-x   0 wangzhou   (501) staff       (20)        0 2023-06-26 01:37:44.863655 HawaData-0.7.4/hawa/common/
--rw-r--r--   0 wangzhou   (501) staff       (20)        0 2022-11-30 09:40:41.000000 HawaData-0.7.4/hawa/common/__init__.py
--rw-r--r--   0 wangzhou   (501) staff       (20)    12444 2023-06-21 13:26:47.000000 HawaData-0.7.4/hawa/common/data.py
--rw-r--r--   0 wangzhou   (501) staff       (20)     5868 2023-06-19 08:57:17.000000 HawaData-0.7.4/hawa/common/query.py
--rw-r--r--   0 wangzhou   (501) staff       (20)     3098 2023-06-19 08:54:42.000000 HawaData-0.7.4/hawa/common/utils.py
--rw-r--r--   0 wangzhou   (501) staff       (20)     2552 2023-06-25 09:15:05.000000 HawaData-0.7.4/hawa/config.py
-drwxr-xr-x   0 wangzhou   (501) staff       (20)        0 2023-06-26 01:37:44.867978 HawaData-0.7.4/hawa/data/
--rw-r--r--   0 wangzhou   (501) staff       (20)        0 2022-12-01 08:59:59.000000 HawaData-0.7.4/hawa/data/__init__.py
--rw-r--r--   0 wangzhou   (501) staff       (20)      311 2023-05-22 06:36:14.000000 HawaData-0.7.4/hawa/data/city.py
--rw-r--r--   0 wangzhou   (501) staff       (20)      432 2023-05-22 06:36:14.000000 HawaData-0.7.4/hawa/data/district.py
--rw-r--r--   0 wangzhou   (501) staff       (20)     1592 2023-05-23 08:41:21.000000 HawaData-0.7.4/hawa/data/klass.py
--rw-r--r--   0 wangzhou   (501) staff       (20)      946 2023-06-21 13:09:45.000000 HawaData-0.7.4/hawa/data/school.py
--rw-r--r--   0 wangzhou   (501) staff       (20)     1197 2023-06-13 03:42:10.000000 HawaData-0.7.4/hawa/data/student.py
-drwxr-xr-x   0 wangzhou   (501) staff       (20)        0 2023-06-26 01:37:44.869883 HawaData-0.7.4/hawa/paper/
--rw-r--r--   0 wangzhou   (501) staff       (20)        0 2022-12-01 09:27:31.000000 HawaData-0.7.4/hawa/paper/__init__.py
--rw-r--r--   0 wangzhou   (501) staff       (20)    28401 2023-06-26 01:36:37.000000 HawaData-0.7.4/hawa/paper/health.py
--rw-r--r--   0 wangzhou   (501) staff       (20)     5273 2023-06-19 03:19:29.000000 HawaData-0.7.4/hawa/paper/mht.py
--rw-r--r--   0 wangzhou   (501) staff       (20)       38 2023-06-26 01:37:44.872004 HawaData-0.7.4/setup.cfg
--rw-r--r--   0 wangzhou   (501) staff       (20)      879 2023-05-05 08:13:11.000000 HawaData-0.7.4/setup.py
-drwxr-xr-x   0 wangzhou   (501) staff       (20)        0 2023-06-26 01:37:44.870791 HawaData-0.7.4/test/
--rw-r--r--   0 wangzhou   (501) staff       (20)     2208 2022-12-08 07:17:34.000000 HawaData-0.7.4/test/test_query.py
+drwxr-xr-x   0 wangzhou   (501) staff       (20)        0 2023-06-26 01:40:10.324671 HawaData-0.7.5/
+drwxr-xr-x   0 wangzhou   (501) staff       (20)        0 2023-06-26 01:40:10.317195 HawaData-0.7.5/HawaData.egg-info/
+-rw-r--r--   0 wangzhou   (501) staff       (20)     3149 2023-06-26 01:40:10.000000 HawaData-0.7.5/HawaData.egg-info/PKG-INFO
+-rw-r--r--   0 wangzhou   (501) staff       (20)      562 2023-06-26 01:40:10.000000 HawaData-0.7.5/HawaData.egg-info/SOURCES.txt
+-rw-r--r--   0 wangzhou   (501) staff       (20)        1 2023-06-26 01:40:10.000000 HawaData-0.7.5/HawaData.egg-info/dependency_links.txt
+-rw-r--r--   0 wangzhou   (501) staff       (20)        5 2023-06-26 01:40:10.000000 HawaData-0.7.5/HawaData.egg-info/top_level.txt
+-rw-r--r--   0 wangzhou   (501) staff       (20)     3149 2023-06-26 01:40:10.324391 HawaData-0.7.5/PKG-INFO
+-rw-r--r--   0 wangzhou   (501) staff       (20)      669 2022-12-02 07:10:45.000000 HawaData-0.7.5/README.md
+drwxr-xr-x   0 wangzhou   (501) staff       (20)        0 2023-06-26 01:40:10.318223 HawaData-0.7.5/hawa/
+-rw-r--r--   0 wangzhou   (501) staff       (20)        0 2022-11-30 09:39:05.000000 HawaData-0.7.5/hawa/__init__.py
+drwxr-xr-x   0 wangzhou   (501) staff       (20)        0 2023-06-26 01:40:10.319588 HawaData-0.7.5/hawa/base/
+-rw-r--r--   0 wangzhou   (501) staff       (20)        0 2022-12-01 05:35:03.000000 HawaData-0.7.5/hawa/base/__init__.py
+-rw-r--r--   0 wangzhou   (501) staff       (20)     2627 2023-06-19 08:54:42.000000 HawaData-0.7.5/hawa/base/db.py
+-rw-r--r--   0 wangzhou   (501) staff       (20)      173 2022-12-01 06:05:08.000000 HawaData-0.7.5/hawa/base/decos.py
+-rw-r--r--   0 wangzhou   (501) staff       (20)       98 2023-05-24 07:06:51.000000 HawaData-0.7.5/hawa/base/errors.py
+-rw-r--r--   0 wangzhou   (501) staff       (20)      845 2022-12-02 03:09:07.000000 HawaData-0.7.5/hawa/base/init.py
+drwxr-xr-x   0 wangzhou   (501) staff       (20)        0 2023-06-26 01:40:10.320766 HawaData-0.7.5/hawa/common/
+-rw-r--r--   0 wangzhou   (501) staff       (20)        0 2022-11-30 09:40:41.000000 HawaData-0.7.5/hawa/common/__init__.py
+-rw-r--r--   0 wangzhou   (501) staff       (20)    12444 2023-06-21 13:26:47.000000 HawaData-0.7.5/hawa/common/data.py
+-rw-r--r--   0 wangzhou   (501) staff       (20)     5868 2023-06-19 08:57:17.000000 HawaData-0.7.5/hawa/common/query.py
+-rw-r--r--   0 wangzhou   (501) staff       (20)     3098 2023-06-19 08:54:42.000000 HawaData-0.7.5/hawa/common/utils.py
+-rw-r--r--   0 wangzhou   (501) staff       (20)     2640 2023-06-26 01:39:47.000000 HawaData-0.7.5/hawa/config.py
+drwxr-xr-x   0 wangzhou   (501) staff       (20)        0 2023-06-26 01:40:10.322777 HawaData-0.7.5/hawa/data/
+-rw-r--r--   0 wangzhou   (501) staff       (20)        0 2022-12-01 08:59:59.000000 HawaData-0.7.5/hawa/data/__init__.py
+-rw-r--r--   0 wangzhou   (501) staff       (20)      311 2023-05-22 06:36:14.000000 HawaData-0.7.5/hawa/data/city.py
+-rw-r--r--   0 wangzhou   (501) staff       (20)      432 2023-05-22 06:36:14.000000 HawaData-0.7.5/hawa/data/district.py
+-rw-r--r--   0 wangzhou   (501) staff       (20)     1592 2023-05-23 08:41:21.000000 HawaData-0.7.5/hawa/data/klass.py
+-rw-r--r--   0 wangzhou   (501) staff       (20)      946 2023-06-21 13:09:45.000000 HawaData-0.7.5/hawa/data/school.py
+-rw-r--r--   0 wangzhou   (501) staff       (20)     1197 2023-06-13 03:42:10.000000 HawaData-0.7.5/hawa/data/student.py
+drwxr-xr-x   0 wangzhou   (501) staff       (20)        0 2023-06-26 01:40:10.323737 HawaData-0.7.5/hawa/paper/
+-rw-r--r--   0 wangzhou   (501) staff       (20)        0 2022-12-01 09:27:31.000000 HawaData-0.7.5/hawa/paper/__init__.py
+-rw-r--r--   0 wangzhou   (501) staff       (20)    28407 2023-06-26 01:39:47.000000 HawaData-0.7.5/hawa/paper/health.py
+-rw-r--r--   0 wangzhou   (501) staff       (20)     5273 2023-06-19 03:19:29.000000 HawaData-0.7.5/hawa/paper/mht.py
+-rw-r--r--   0 wangzhou   (501) staff       (20)       38 2023-06-26 01:40:10.324749 HawaData-0.7.5/setup.cfg
+-rw-r--r--   0 wangzhou   (501) staff       (20)      879 2023-05-05 08:13:11.000000 HawaData-0.7.5/setup.py
+drwxr-xr-x   0 wangzhou   (501) staff       (20)        0 2023-06-26 01:40:10.324022 HawaData-0.7.5/test/
+-rw-r--r--   0 wangzhou   (501) staff       (20)     2208 2022-12-08 07:17:34.000000 HawaData-0.7.5/test/test_query.py
```

### Comparing `HawaData-0.7.4/HawaData.egg-info/PKG-INFO` & `HawaData-0.7.5/HawaData.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: HawaData
-Version: 0.7.4
+Version: 0.7.5
 Summary: Use For Unified Hawa Data.
 Home-page: https://github.com/StevenLianaL/HawaData
 Author: Steven Wang
 Author-email: brightstar8284@icloud.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Description-Content-Type: text/markdown
@@ -106,7 +106,8 @@
 - 0.6.4 count dim field rank
 - 0.6.5 count sub unit ids
 - 0.7.0 use contextmanager to connect db
 - 0.7.1 count score rank with gender
 - 0.7.2 add cascade students
 - 0.7.3 add is_leaf to cascade students
 - 0.7.4 add ch key for dim_field data
+- 0.7.5 add ch key for dim_field data
```

### Comparing `HawaData-0.7.4/HawaData.egg-info/SOURCES.txt` & `HawaData-0.7.5/HawaData.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `HawaData-0.7.4/PKG-INFO` & `HawaData-0.7.5/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: HawaData
-Version: 0.7.4
+Version: 0.7.5
 Summary: Use For Unified Hawa Data.
 Home-page: https://github.com/StevenLianaL/HawaData
 Author: Steven Wang
 Author-email: brightstar8284@icloud.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Description-Content-Type: text/markdown
@@ -106,7 +106,8 @@
 - 0.6.4 count dim field rank
 - 0.6.5 count sub unit ids
 - 0.7.0 use contextmanager to connect db
 - 0.7.1 count score rank with gender
 - 0.7.2 add cascade students
 - 0.7.3 add is_leaf to cascade students
 - 0.7.4 add ch key for dim_field data
+- 0.7.5 add ch key for dim_field data
```

### Comparing `HawaData-0.7.4/README.md` & `HawaData-0.7.5/README.md`

 * *Files identical despite different names*

### Comparing `HawaData-0.7.4/hawa/base/db.py` & `HawaData-0.7.5/hawa/base/db.py`

 * *Files identical despite different names*

### Comparing `HawaData-0.7.4/hawa/base/init.py` & `HawaData-0.7.5/hawa/base/init.py`

 * *Files identical despite different names*

### Comparing `HawaData-0.7.4/hawa/common/data.py` & `HawaData-0.7.5/hawa/common/data.py`

 * *Files identical despite different names*

### Comparing `HawaData-0.7.4/hawa/common/query.py` & `HawaData-0.7.5/hawa/common/query.py`

 * *Files identical despite different names*

### Comparing `HawaData-0.7.4/hawa/common/utils.py` & `HawaData-0.7.5/hawa/common/utils.py`

 * *Files identical despite different names*

### Comparing `HawaData-0.7.4/hawa/config.py` & `HawaData-0.7.5/hawa/config.py`

 * *Files 3% similar despite different names*

```diff
@@ -49,14 +49,18 @@
     min_join_number = 10
     min_alone_numger = 5
 
     gender_map = {
         'total': '总体', 'M': '男生', "F": "女生"
     }
 
+    total_gender_map = {
+        'total': '全部', 'M': '男生', "F": "女生"
+    }
+
     # rank
     ranks = {
         'RANK_LABEL': {'A': '优秀', 'B': '良好', 'C': '达标', 'D': '待达标'},
         'FEEDBACK_LEVEL': {'A': '优秀', 'B': '良好', 'C': '中等', 'D': '待提高'}
     }
     reverse_ranks = {
         'RANK_LABEL': {k: v for v, k in ranks['RANK_LABEL'].items()},
```

### Comparing `HawaData-0.7.4/hawa/data/klass.py` & `HawaData-0.7.5/hawa/data/klass.py`

 * *Files identical despite different names*

### Comparing `HawaData-0.7.4/hawa/data/school.py` & `HawaData-0.7.5/hawa/data/school.py`

 * *Files identical despite different names*

### Comparing `HawaData-0.7.4/hawa/data/student.py` & `HawaData-0.7.5/hawa/data/student.py`

 * *Files identical despite different names*

### Comparing `HawaData-0.7.4/hawa/paper/health.py` & `HawaData-0.7.5/hawa/paper/health.py`

 * *Files 0% similar despite different names*

```diff
@@ -88,15 +88,15 @@
             res[gender_k] = self.count_dim_or_field_scores_by_answers(
                 answers=gender_v, item_code=item_code, res_format='dict'
             )
         codes = answers[item_code].unique().tolist()
         gender_box = []
         for gender_k, gender_data in res.items():
             row_data = {
-                "name": gender_k if key_format == 'en' else project.gender_map[gender_k],
+                "name": gender_k if key_format == 'en' else project.total_gender_map[gender_k],
                 "value": []
             }
             for c in codes:
                 row_data["value"].append(res[gender_k][c])
             gender_box.append(row_data)
 
         return {
```

### Comparing `HawaData-0.7.4/hawa/paper/mht.py` & `HawaData-0.7.5/hawa/paper/mht.py`

 * *Files identical despite different names*

### Comparing `HawaData-0.7.4/setup.py` & `HawaData-0.7.5/setup.py`

 * *Files identical despite different names*

### Comparing `HawaData-0.7.4/test/test_query.py` & `HawaData-0.7.5/test/test_query.py`

 * *Files identical despite different names*

