# Comparing `tmp/HawaData-0.7.5.tar.gz` & `tmp/HawaData-0.7.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "HawaData-0.7.5.tar", last modified: Mon Jun 26 01:40:10 2023, max compression
+gzip compressed data, was "HawaData-0.7.6.tar", last modified: Mon Jun 26 06:30:02 2023, max compression
```

## Comparing `HawaData-0.7.5.tar` & `HawaData-0.7.6.tar`

### file list

```diff
@@ -1,37 +1,38 @@
-drwxr-xr-x   0 wangzhou   (501) staff       (20)        0 2023-06-26 01:40:10.324671 HawaData-0.7.5/
-drwxr-xr-x   0 wangzhou   (501) staff       (20)        0 2023-06-26 01:40:10.317195 HawaData-0.7.5/HawaData.egg-info/
--rw-r--r--   0 wangzhou   (501) staff       (20)     3149 2023-06-26 01:40:10.000000 HawaData-0.7.5/HawaData.egg-info/PKG-INFO
--rw-r--r--   0 wangzhou   (501) staff       (20)      562 2023-06-26 01:40:10.000000 HawaData-0.7.5/HawaData.egg-info/SOURCES.txt
--rw-r--r--   0 wangzhou   (501) staff       (20)        1 2023-06-26 01:40:10.000000 HawaData-0.7.5/HawaData.egg-info/dependency_links.txt
--rw-r--r--   0 wangzhou   (501) staff       (20)        5 2023-06-26 01:40:10.000000 HawaData-0.7.5/HawaData.egg-info/top_level.txt
--rw-r--r--   0 wangzhou   (501) staff       (20)     3149 2023-06-26 01:40:10.324391 HawaData-0.7.5/PKG-INFO
--rw-r--r--   0 wangzhou   (501) staff       (20)      669 2022-12-02 07:10:45.000000 HawaData-0.7.5/README.md
-drwxr-xr-x   0 wangzhou   (501) staff       (20)        0 2023-06-26 01:40:10.318223 HawaData-0.7.5/hawa/
--rw-r--r--   0 wangzhou   (501) staff       (20)        0 2022-11-30 09:39:05.000000 HawaData-0.7.5/hawa/__init__.py
-drwxr-xr-x   0 wangzhou   (501) staff       (20)        0 2023-06-26 01:40:10.319588 HawaData-0.7.5/hawa/base/
--rw-r--r--   0 wangzhou   (501) staff       (20)        0 2022-12-01 05:35:03.000000 HawaData-0.7.5/hawa/base/__init__.py
--rw-r--r--   0 wangzhou   (501) staff       (20)     2627 2023-06-19 08:54:42.000000 HawaData-0.7.5/hawa/base/db.py
--rw-r--r--   0 wangzhou   (501) staff       (20)      173 2022-12-01 06:05:08.000000 HawaData-0.7.5/hawa/base/decos.py
--rw-r--r--   0 wangzhou   (501) staff       (20)       98 2023-05-24 07:06:51.000000 HawaData-0.7.5/hawa/base/errors.py
--rw-r--r--   0 wangzhou   (501) staff       (20)      845 2022-12-02 03:09:07.000000 HawaData-0.7.5/hawa/base/init.py
-drwxr-xr-x   0 wangzhou   (501) staff       (20)        0 2023-06-26 01:40:10.320766 HawaData-0.7.5/hawa/common/
--rw-r--r--   0 wangzhou   (501) staff       (20)        0 2022-11-30 09:40:41.000000 HawaData-0.7.5/hawa/common/__init__.py
--rw-r--r--   0 wangzhou   (501) staff       (20)    12444 2023-06-21 13:26:47.000000 HawaData-0.7.5/hawa/common/data.py
--rw-r--r--   0 wangzhou   (501) staff       (20)     5868 2023-06-19 08:57:17.000000 HawaData-0.7.5/hawa/common/query.py
--rw-r--r--   0 wangzhou   (501) staff       (20)     3098 2023-06-19 08:54:42.000000 HawaData-0.7.5/hawa/common/utils.py
--rw-r--r--   0 wangzhou   (501) staff       (20)     2640 2023-06-26 01:39:47.000000 HawaData-0.7.5/hawa/config.py
-drwxr-xr-x   0 wangzhou   (501) staff       (20)        0 2023-06-26 01:40:10.322777 HawaData-0.7.5/hawa/data/
--rw-r--r--   0 wangzhou   (501) staff       (20)        0 2022-12-01 08:59:59.000000 HawaData-0.7.5/hawa/data/__init__.py
--rw-r--r--   0 wangzhou   (501) staff       (20)      311 2023-05-22 06:36:14.000000 HawaData-0.7.5/hawa/data/city.py
--rw-r--r--   0 wangzhou   (501) staff       (20)      432 2023-05-22 06:36:14.000000 HawaData-0.7.5/hawa/data/district.py
--rw-r--r--   0 wangzhou   (501) staff       (20)     1592 2023-05-23 08:41:21.000000 HawaData-0.7.5/hawa/data/klass.py
--rw-r--r--   0 wangzhou   (501) staff       (20)      946 2023-06-21 13:09:45.000000 HawaData-0.7.5/hawa/data/school.py
--rw-r--r--   0 wangzhou   (501) staff       (20)     1197 2023-06-13 03:42:10.000000 HawaData-0.7.5/hawa/data/student.py
-drwxr-xr-x   0 wangzhou   (501) staff       (20)        0 2023-06-26 01:40:10.323737 HawaData-0.7.5/hawa/paper/
--rw-r--r--   0 wangzhou   (501) staff       (20)        0 2022-12-01 09:27:31.000000 HawaData-0.7.5/hawa/paper/__init__.py
--rw-r--r--   0 wangzhou   (501) staff       (20)    28407 2023-06-26 01:39:47.000000 HawaData-0.7.5/hawa/paper/health.py
--rw-r--r--   0 wangzhou   (501) staff       (20)     5273 2023-06-19 03:19:29.000000 HawaData-0.7.5/hawa/paper/mht.py
--rw-r--r--   0 wangzhou   (501) staff       (20)       38 2023-06-26 01:40:10.324749 HawaData-0.7.5/setup.cfg
--rw-r--r--   0 wangzhou   (501) staff       (20)      879 2023-05-05 08:13:11.000000 HawaData-0.7.5/setup.py
-drwxr-xr-x   0 wangzhou   (501) staff       (20)        0 2023-06-26 01:40:10.324022 HawaData-0.7.5/test/
--rw-r--r--   0 wangzhou   (501) staff       (20)     2208 2022-12-08 07:17:34.000000 HawaData-0.7.5/test/test_query.py
+drwxr-xr-x   0 wangzhou   (501) staff       (20)        0 2023-06-26 06:30:02.060936 HawaData-0.7.6/
+drwxr-xr-x   0 wangzhou   (501) staff       (20)        0 2023-06-26 06:30:02.049295 HawaData-0.7.6/HawaData.egg-info/
+-rw-r--r--   0 wangzhou   (501) staff       (20)     3207 2023-06-26 06:30:01.000000 HawaData-0.7.6/HawaData.egg-info/PKG-INFO
+-rw-r--r--   0 wangzhou   (501) staff       (20)      584 2023-06-26 06:30:02.000000 HawaData-0.7.6/HawaData.egg-info/SOURCES.txt
+-rw-r--r--   0 wangzhou   (501) staff       (20)        1 2023-06-26 06:30:01.000000 HawaData-0.7.6/HawaData.egg-info/dependency_links.txt
+-rw-r--r--   0 wangzhou   (501) staff       (20)        5 2023-06-26 06:30:01.000000 HawaData-0.7.6/HawaData.egg-info/top_level.txt
+-rw-r--r--   0 wangzhou   (501) staff       (20)     3207 2023-06-26 06:30:02.060658 HawaData-0.7.6/PKG-INFO
+-rw-r--r--   0 wangzhou   (501) staff       (20)      669 2022-12-02 07:10:45.000000 HawaData-0.7.6/README.md
+drwxr-xr-x   0 wangzhou   (501) staff       (20)        0 2023-06-26 06:30:02.049834 HawaData-0.7.6/hawa/
+-rw-r--r--   0 wangzhou   (501) staff       (20)        0 2022-11-30 09:39:05.000000 HawaData-0.7.6/hawa/__init__.py
+drwxr-xr-x   0 wangzhou   (501) staff       (20)        0 2023-06-26 06:30:02.052650 HawaData-0.7.6/hawa/base/
+-rw-r--r--   0 wangzhou   (501) staff       (20)        0 2022-12-01 05:35:03.000000 HawaData-0.7.6/hawa/base/__init__.py
+-rw-r--r--   0 wangzhou   (501) staff       (20)     2627 2023-06-19 08:54:42.000000 HawaData-0.7.6/hawa/base/db.py
+-rw-r--r--   0 wangzhou   (501) staff       (20)      173 2022-12-01 06:05:08.000000 HawaData-0.7.6/hawa/base/decos.py
+-rw-r--r--   0 wangzhou   (501) staff       (20)       98 2023-05-24 07:06:51.000000 HawaData-0.7.6/hawa/base/errors.py
+-rw-r--r--   0 wangzhou   (501) staff       (20)      845 2022-12-02 03:09:07.000000 HawaData-0.7.6/hawa/base/init.py
+drwxr-xr-x   0 wangzhou   (501) staff       (20)        0 2023-06-26 06:30:02.054354 HawaData-0.7.6/hawa/common/
+-rw-r--r--   0 wangzhou   (501) staff       (20)        0 2022-11-30 09:40:41.000000 HawaData-0.7.6/hawa/common/__init__.py
+-rw-r--r--   0 wangzhou   (501) staff       (20)    15442 2023-06-26 06:26:56.000000 HawaData-0.7.6/hawa/common/data.py
+-rw-r--r--   0 wangzhou   (501) staff       (20)     6169 2023-06-26 06:18:33.000000 HawaData-0.7.6/hawa/common/query.py
+-rw-r--r--   0 wangzhou   (501) staff       (20)     3098 2023-06-19 08:54:42.000000 HawaData-0.7.6/hawa/common/utils.py
+-rw-r--r--   0 wangzhou   (501) staff       (20)     2696 2023-06-26 02:08:50.000000 HawaData-0.7.6/hawa/config.py
+drwxr-xr-x   0 wangzhou   (501) staff       (20)        0 2023-06-26 06:30:02.057923 HawaData-0.7.6/hawa/data/
+-rw-r--r--   0 wangzhou   (501) staff       (20)        0 2022-12-01 08:59:59.000000 HawaData-0.7.6/hawa/data/__init__.py
+-rw-r--r--   0 wangzhou   (501) staff       (20)      311 2023-05-22 06:36:14.000000 HawaData-0.7.6/hawa/data/city.py
+-rw-r--r--   0 wangzhou   (501) staff       (20)      432 2023-05-22 06:36:14.000000 HawaData-0.7.6/hawa/data/district.py
+-rw-r--r--   0 wangzhou   (501) staff       (20)     1592 2023-05-23 08:41:21.000000 HawaData-0.7.6/hawa/data/klass.py
+-rw-r--r--   0 wangzhou   (501) staff       (20)      711 2023-06-26 06:27:54.000000 HawaData-0.7.6/hawa/data/province.py
+-rw-r--r--   0 wangzhou   (501) staff       (20)      946 2023-06-21 13:09:45.000000 HawaData-0.7.6/hawa/data/school.py
+-rw-r--r--   0 wangzhou   (501) staff       (20)     1197 2023-06-13 03:42:10.000000 HawaData-0.7.6/hawa/data/student.py
+drwxr-xr-x   0 wangzhou   (501) staff       (20)        0 2023-06-26 06:30:02.059306 HawaData-0.7.6/hawa/paper/
+-rw-r--r--   0 wangzhou   (501) staff       (20)        0 2022-12-01 09:27:31.000000 HawaData-0.7.6/hawa/paper/__init__.py
+-rw-r--r--   0 wangzhou   (501) staff       (20)    28407 2023-06-26 01:39:47.000000 HawaData-0.7.6/hawa/paper/health.py
+-rw-r--r--   0 wangzhou   (501) staff       (20)     5273 2023-06-19 03:19:29.000000 HawaData-0.7.6/hawa/paper/mht.py
+-rw-r--r--   0 wangzhou   (501) staff       (20)       38 2023-06-26 06:30:02.061024 HawaData-0.7.6/setup.cfg
+-rw-r--r--   0 wangzhou   (501) staff       (20)      879 2023-05-05 08:13:11.000000 HawaData-0.7.6/setup.py
+drwxr-xr-x   0 wangzhou   (501) staff       (20)        0 2023-06-26 06:30:02.060058 HawaData-0.7.6/test/
+-rw-r--r--   0 wangzhou   (501) staff       (20)     2208 2022-12-08 07:17:34.000000 HawaData-0.7.6/test/test_query.py
```

### Comparing `HawaData-0.7.5/HawaData.egg-info/PKG-INFO` & `HawaData-0.7.6/HawaData.egg-info/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: HawaData
-Version: 0.7.5
+Version: 0.7.6
 Summary: Use For Unified Hawa Data.
 Home-page: https://github.com/StevenLianaL/HawaData
 Author: Steven Wang
 Author-email: brightstar8284@icloud.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Description-Content-Type: text/markdown
@@ -107,7 +107,8 @@
 - 0.6.5 count sub unit ids
 - 0.7.0 use contextmanager to connect db
 - 0.7.1 count score rank with gender
 - 0.7.2 add cascade students
 - 0.7.3 add is_leaf to cascade students
 - 0.7.4 add ch key for dim_field data
 - 0.7.5 add ch key for dim_field data
+- 0.7.6 add ProvinceHealthApiDataLess for cascade schools
```

### Comparing `HawaData-0.7.5/HawaData.egg-info/SOURCES.txt` & `HawaData-0.7.6/HawaData.egg-info/SOURCES.txt`

 * *Files 16% similar despite different names*

```diff
@@ -15,13 +15,14 @@
 hawa/common/data.py
 hawa/common/query.py
 hawa/common/utils.py
 hawa/data/__init__.py
 hawa/data/city.py
 hawa/data/district.py
 hawa/data/klass.py
+hawa/data/province.py
 hawa/data/school.py
 hawa/data/student.py
 hawa/paper/__init__.py
 hawa/paper/health.py
 hawa/paper/mht.py
 test/test_query.py
```

### Comparing `HawaData-0.7.5/PKG-INFO` & `HawaData-0.7.6/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: HawaData
-Version: 0.7.5
+Version: 0.7.6
 Summary: Use For Unified Hawa Data.
 Home-page: https://github.com/StevenLianaL/HawaData
 Author: Steven Wang
 Author-email: brightstar8284@icloud.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Description-Content-Type: text/markdown
@@ -107,7 +107,8 @@
 - 0.6.5 count sub unit ids
 - 0.7.0 use contextmanager to connect db
 - 0.7.1 count score rank with gender
 - 0.7.2 add cascade students
 - 0.7.3 add is_leaf to cascade students
 - 0.7.4 add ch key for dim_field data
 - 0.7.5 add ch key for dim_field data
+- 0.7.6 add ProvinceHealthApiDataLess for cascade schools
```

### Comparing `HawaData-0.7.5/README.md` & `HawaData-0.7.6/README.md`

 * *Files identical despite different names*

### Comparing `HawaData-0.7.5/hawa/base/db.py` & `HawaData-0.7.6/hawa/base/db.py`

 * *Files identical despite different names*

### Comparing `HawaData-0.7.5/hawa/base/init.py` & `HawaData-0.7.6/hawa/base/init.py`

 * *Files identical despite different names*

### Comparing `HawaData-0.7.5/hawa/common/data.py` & `HawaData-0.7.6/hawa/common/data.py`

 * *Files 18% similar despite different names*

```diff
@@ -77,14 +77,15 @@
     last_year = None
     last_year_code_scores: Optional[pd.DataFrame] = field(default_factory=pd.DataFrame)
 
     def __post_init__(self):
         # 初始化数据
         init_functions = [i for i in dir(self) if i.startswith('_to_init_')]
         for func in init_functions:
+            print(f"{func=}")
             getattr(self, func)()
 
         # 构建辅助工具
         self._to_build_helper()
 
         # 计算数据
         count_functions = [i for i in dir(self) if i.startswith('_to_count_')]
@@ -133,14 +134,15 @@
             valid_to_start=start_stamp_str,
             valid_to_end=end_stamp_str,
         )
         if self.cases.empty:
             raise NoCasesError(f'no cases:{self.meta_unit} {self.school_ids}')
         self.case_ids = self.cases['id'].tolist()
         self.case_project_ids = Counter(self.cases['project_id'].tolist())
+        self.school_ids = self.cases['school_id'].unique().tolist()
         project.logger.debug(f'cases: {len(self.cases)}')
 
     def _to_init_e_answers(self):
         self.answers = self.query.query_answers(case_ids=self.case_ids)
         project.logger.debug(f'answers: {len(self.answers)}')
 
     def _to_init_f_students(self):
@@ -306,7 +308,70 @@
                 if not cls_row['children']:
                     cls_row['is_leaf'] = True
                 grade_row['children'].append(cls_row)
             if not grade_row['children']:
                 grade_row['is_leaf'] = True
             res.append(grade_row)
         return res
+
+    def get_cascade_schools_from_province(self):
+        """省-市-区县-学校的 cascade 数据"""
+        sch_ids = self.school_ids
+        province_ids = {i // (10 ** 8) * 10000 for i in sch_ids}
+        city_ids = {i // (10 ** 6) * 100 for i in sch_ids}
+        district_ids = {i // (10 ** 4) for i in sch_ids}
+        location_ids = province_ids | city_ids | district_ids
+        locations = self.query.query_locations(list(location_ids))
+        schools = self.schools
+        location_map = {lo['id']: lo for _, lo in locations.iterrows()}
+        school_map = {sch['id']: sch for _, sch in schools.iterrows()}
+        res = []
+        for p_id in province_ids:
+            p = location_map[p_id]
+            p_row = {
+                'label': p['name'], 'value': p['id'], 'children': [], "is_leaf": False
+            }
+            if p_id not in project.municipality_ids:
+                for c_id in city_ids:
+                    if c_id // 10000 * 10000 != p_id:
+                        continue
+                    c = location_map[c_id]
+                    c_row = {
+                        'label': c['name'], 'value': c['id'], 'children': [], "is_leaf": False
+                    }
+                    for d_id in district_ids:
+                        if d_id // 100 * 100 != c_id:
+                            continue
+                        d = location_map[d_id]
+                        d_row = {
+                            'label': d['name'], 'value': d['id'], 'children': [], "is_leaf": False
+                        }
+                        for s_id in sch_ids:
+                            if s_id // 10000 != d_id:
+                                continue
+                            s = school_map[s_id]
+                            s_row = {
+                                'label': s['name'], 'value': s['id'], "is_leaf": True
+                            }
+                            d_row['children'].append(s_row)
+                        c_row['children'].append(d_row)
+                    p_row['children'].append(c_row)
+                res.append(p_row)
+            else:
+                for d_id in district_ids:
+                    if d_id // 10000 * 10000 != p_id:
+                        continue
+                    d = location_map[d_id]
+                    d_row = {
+                        'label': d['name'], 'value': d['id'], 'children': [], "is_leaf": False
+                    }
+                    for s_id in sch_ids:
+                        if s_id // 10000 != d_id:
+                            continue
+                        s = school_map[s_id]
+                        s_row = {
+                            'label': s['name'], 'value': s['id'], "is_leaf": True
+                        }
+                        d_row['children'].append(s_row)
+                    p_row['children'].append(d_row)
+                res.append(p_row)
+        return res
```

### Comparing `HawaData-0.7.5/hawa/common/query.py` & `HawaData-0.7.6/hawa/common/query.py`

 * *Files 12% similar despite different names*

```diff
@@ -78,15 +78,15 @@
             return pd.DataFrame()
         elif len(school_ids) == 1:
             school_sql = f"and cs.school_id={school_ids[0]}"
         else:
             school_sql = f"and cs.school_id in {tuple(school_ids)}"
 
         sql = f"select c.id,c.name,c.valid_from,c.valid_to,c.client_id,c.created," \
-              f"c.paper_id,c.is_cleared, cp.name project_name, c.project_id " \
+              f"c.paper_id,c.is_cleared, cp.name project_name, c.project_id, cs.school_id " \
               f"from cases c " \
               f"inner join case_schools cs on c.id=cs.case_id " \
               f"inner join case_projects cp on c.project_id=cp.id " \
               f"where  is_cleared=1 and valid_to between '{valid_to_start}' and '{valid_to_end}'" \
               f" {school_sql} {paper_sql};"
         with self.db.engine_conn() as conn:
             cases = pd.read_sql(text(sql), conn).drop_duplicates(subset=['id'])
@@ -124,7 +124,13 @@
     def query_item_codes(self, item_ids: list[int]):
         item_code_sql = f'select ic.item_id,ic.code,ic.category,c.name ' \
                         f'from item_codes ic left join codebook c on ic.code = c.code ' \
                         f'where ic.item_id in {tuple(item_ids)};'
         with self.db.engine_conn() as conn:
             item_codes = pd.read_sql(text(item_code_sql), conn)
         return item_codes
+
+    def query_locations(self, location_ids: list[int]):
+        location_sql = f'select id, name, level from locations where id in {tuple(location_ids)};'
+        with self.db.engine_conn() as conn:
+            locations = pd.read_sql(text(location_sql), conn)
+        return locations
```

### Comparing `HawaData-0.7.5/hawa/common/utils.py` & `HawaData-0.7.6/hawa/common/utils.py`

 * *Files identical despite different names*

### Comparing `HawaData-0.7.5/hawa/config.py` & `HawaData-0.7.6/hawa/config.py`

 * *Files 9% similar despite different names*

```diff
@@ -81,14 +81,15 @@
 
     category_map = {
         'total': "学生", 'M': '男生', "F": "女生"
     }
 
     # other
     municipality = {11, 12, 31, 50}
+    municipality_ids = {110000, 120000, 310000, 500000}
 
     class Config:
         env_prefix = 'No_Env_'  # 不使用环境变量
 
     @property
     def grade_mapping(self):
         mappings = dict(zip(range(0, 13), '无 一 二 三 四 五 六 七 八 九 十 十一 十二'.split(' ')))
```

### Comparing `HawaData-0.7.5/hawa/data/klass.py` & `HawaData-0.7.6/hawa/data/klass.py`

 * *Files identical despite different names*

### Comparing `HawaData-0.7.5/hawa/data/school.py` & `HawaData-0.7.6/hawa/data/school.py`

 * *Files identical despite different names*

### Comparing `HawaData-0.7.5/hawa/data/student.py` & `HawaData-0.7.6/hawa/data/student.py`

 * *Files identical despite different names*

### Comparing `HawaData-0.7.5/hawa/paper/health.py` & `HawaData-0.7.6/hawa/paper/health.py`

 * *Files identical despite different names*

### Comparing `HawaData-0.7.5/hawa/paper/mht.py` & `HawaData-0.7.6/hawa/paper/mht.py`

 * *Files identical despite different names*

### Comparing `HawaData-0.7.5/setup.py` & `HawaData-0.7.6/setup.py`

 * *Files identical despite different names*

### Comparing `HawaData-0.7.5/test/test_query.py` & `HawaData-0.7.6/test/test_query.py`

 * *Files identical despite different names*

