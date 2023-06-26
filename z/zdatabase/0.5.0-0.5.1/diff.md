# Comparing `tmp/zdatabase-0.5.0.tar.gz` & `tmp/zdatabase-0.5.1.tar.gz`

## Comparing `zdatabase-0.5.0.tar` & `zdatabase-0.5.1.tar`

### file list

```diff
@@ -1,8 +1,8 @@
--rw-r--r--   0        0        0      707 2020-02-02 00:00:00.000000 zdatabase-0.5.0/src/zdatabase/__init__.py
--rw-r--r--   0        0        0     2625 2020-02-02 00:00:00.000000 zdatabase-0.5.0/src/zdatabase/model.py
--rw-r--r--   0        0        0     5897 2020-02-02 00:00:00.000000 zdatabase-0.5.0/src/zdatabase/utility.py
--rw-r--r--   0        0        0       10 2020-02-02 00:00:00.000000 zdatabase-0.5.0/.gitignore
--rw-r--r--   0        0        0     1091 2020-02-02 00:00:00.000000 zdatabase-0.5.0/LICENSE
--rw-r--r--   0        0        0       31 2020-02-02 00:00:00.000000 zdatabase-0.5.0/README.md
--rw-r--r--   0        0        0      669 2020-02-02 00:00:00.000000 zdatabase-0.5.0/pyproject.toml
--rw-r--r--   0        0        0      624 2020-02-02 00:00:00.000000 zdatabase-0.5.0/PKG-INFO
+-rw-r--r--   0        0        0      707 2020-02-02 00:00:00.000000 zdatabase-0.5.1/src/zdatabase/__init__.py
+-rw-r--r--   0        0        0     2625 2020-02-02 00:00:00.000000 zdatabase-0.5.1/src/zdatabase/model.py
+-rw-r--r--   0        0        0     5049 2020-02-02 00:00:00.000000 zdatabase-0.5.1/src/zdatabase/utility.py
+-rw-r--r--   0        0        0       10 2020-02-02 00:00:00.000000 zdatabase-0.5.1/.gitignore
+-rw-r--r--   0        0        0     1091 2020-02-02 00:00:00.000000 zdatabase-0.5.1/LICENSE
+-rw-r--r--   0        0        0       31 2020-02-02 00:00:00.000000 zdatabase-0.5.1/README.md
+-rw-r--r--   0        0        0      669 2020-02-02 00:00:00.000000 zdatabase-0.5.1/pyproject.toml
+-rw-r--r--   0        0        0      624 2020-02-02 00:00:00.000000 zdatabase-0.5.1/PKG-INFO
```

### Comparing `zdatabase-0.5.0/src/zdatabase/__init__.py` & `zdatabase-0.5.1/src/zdatabase/__init__.py`

 * *Files identical despite different names*

### Comparing `zdatabase-0.5.0/src/zdatabase/model.py` & `zdatabase-0.5.1/src/zdatabase/model.py`

 * *Files identical despite different names*

### Comparing `zdatabase-0.5.0/src/zdatabase/utility.py` & `zdatabase-0.5.1/src/zdatabase/utility.py`

 * *Files 16% similar despite different names*

```diff
@@ -27,97 +27,68 @@
     def select(cls, params, conds):
         """ 筛选(模糊匹配）
         ?name=1&asset_sn=2019-BG-5453
         """
         flts = []
         for cond in conds:
             value = params.get(cond)
-            if value:
-                flts.append(getattr(cls, cond).like(f'%{value}%'))
+            flts += [getattr(cls, cond).like(f'%{value}%')] if value else []
         return flts
 
     @classmethod
     def select_(cls, params, conds):
         """ 筛选(精确匹配）
         ?name=1&asset_sn=2019-BG-5453
         """
         flts = []
         for cond in conds:
             value = params.get(cond)
-            if value:
-                flts.append(getattr(cls, cond) == value)
+            flts += [getattr(cls, cond) == value] if value else []
         return flts
 
     @classmethod
     def select_date(cls, attr_name, params):
         """ 日期筛选"""
         flts = []
         start_date = params.get('start_date')
         end_date = params.get('end_date')
-        if start_date:
-            flts.append(getattr(cls, attr_name) >= start_date)
-        if end_date:
-            flts.append(getattr(cls, attr_name) <= end_date)
+        flts += [getattr(cls, attr_name) >= start_date] if start_date else []
+        flts += [getattr(cls, attr_name) <= end_date] if end_date else []
         return flts
 
     @staticmethod
     def all(cls, query, method='to_json'):
         """返回全部记录
         """
         items = query.all()
         return [getattr(item, method)() for item in items]
 
     @staticmethod
     def paginate(query, params, method='to_json'):
         """分页
         page_size=100&page_num=1
         """
-        page_num = params.get('page_num')
-        page_size = params.get('page_size')
-        page_num = int(page_num) if page_num else 1
-        page_size = int(page_size) if page_size else 10
-        offset_num = (page_num - 1) * page_size
-        items = query.offset(offset_num).limit(page_size).all()
-        total = query.count()
+        page_num = int(params.get('page_num', '1'))
+        page_size = int(params.get('page_size', '10'))
+        pagination = query.paginate(page_num, per_page=page_size)  
         rst = {
-            'items': [getattr(item, method)() for item in items],
-            'total': total
-        }
-        return rst
-
-    @staticmethod
-    def paginate2(cls, query, params, method):
-        """分页
-        page_size=100&page_num=1
-        """
-        page_num = params.get('page_num')
-        page_size = params.get('page_size')
-        page_num = int(page_num) if page_num else 1
-        page_size = int(page_size) if page_size else 10
-        offset_num = (page_num - 1) * page_size
-        rst = query.offset(offset_num).limit(page_size).all()
-        total = query.count()
-        rst = {
-            'items': [method(item) for item in rst],
-            'total': total
+            'items': [getattr(item, method)() for item in pagination.items],
+            'total': pagination.total
         }
         return rst
 
 
 class MapperUtility:
     @staticmethod
     def jsonlize(items):
         return [item.to_json() for item in items]
 
     @classmethod
     def make_flts(cls, **kwargs):
-        flts = []
-        for k, v in kwargs.items():
-            flts += [getattr(cls, k) == v]
-        return flts
+        return [getattr(cls, k) == v for k, v in kwargs.items()]
 
     @classmethod
     def make_query(cls, **kwargs):
         flts = cls.make_flts(**kwargs)
         return cls.filter(*flts)
 
     @classmethod
```

### Comparing `zdatabase-0.5.0/LICENSE` & `zdatabase-0.5.1/LICENSE`

 * *Files identical despite different names*

### Comparing `zdatabase-0.5.0/pyproject.toml` & `zdatabase-0.5.1/pyproject.toml`

 * *Files 15% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["hatchling"]
 build-backend = "hatchling.build"
 
 [project]
 name = "zdatabase"
-version = "0.5.0"
+version = "0.5.1"
 authors = [
   { name="inspirare6", email="inspirare6@163.com" },
 ]
 description = "zen database library"
 readme = "README.md"
 requires-python = ">=3.7"
 dependencies = [
```

### Comparing `zdatabase-0.5.0/PKG-INFO` & `zdatabase-0.5.1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: zdatabase
-Version: 0.5.0
+Version: 0.5.1
 Summary: zen database library
 Project-URL: Homepage, https://github.com/inspirare6/zdatabase
 Project-URL: Bug Tracker, https://github.com/inspirare6/zdatabase/issues
 Author-email: inspirare6 <inspirare6@163.com>
 License-File: LICENSE
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

