# Comparing `tmp/pysquril-0.3.0.tar.gz` & `tmp/pysquril-0.3.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pysquril-0.3.0.tar", max compression
+gzip compressed data, was "pysquril-0.3.1.tar", max compression
```

## Comparing `pysquril-0.3.0.tar` & `pysquril-0.3.1.tar`

### file list

```diff
@@ -1,9 +1,9 @@
--rw-r--r--   0        0        0      524 2023-06-26 08:48:57.055407 pysquril-0.3.0/pyproject.toml
--rw-r--r--   0        0        0        0 2022-06-22 08:13:57.003868 pysquril-0.3.0/pysquril/__init__.py
--rw-r--r--   0        0        0    24504 2023-06-26 08:26:43.181491 pysquril-0.3.0/pysquril/backends.py
--rw-r--r--   0        0        0      136 2023-06-22 13:54:05.278837 pysquril-0.3.0/pysquril/exc.py
--rw-r--r--   0        0        0    21254 2023-06-20 11:11:42.555715 pysquril-0.3.0/pysquril/generator.py
--rw-r--r--   0        0        0     9452 2023-01-27 11:51:39.899603 pysquril-0.3.0/pysquril/parser.py
--rw-r--r--   0        0        0     1997 2022-11-21 13:00:47.589558 pysquril-0.3.0/pysquril/test_data.py
--rw-r--r--   0        0        0    20442 2023-06-25 19:23:30.096636 pysquril-0.3.0/pysquril/tests.py
--rw-r--r--   0        0        0      658 1970-01-01 00:00:00.000000 pysquril-0.3.0/PKG-INFO
+-rw-r--r--   0        0        0      524 2023-06-26 11:29:09.624724 pysquril-0.3.1/pyproject.toml
+-rw-r--r--   0        0        0        0 2022-06-22 08:13:57.003868 pysquril-0.3.1/pysquril/__init__.py
+-rw-r--r--   0        0        0    24898 2023-06-26 11:27:37.766727 pysquril-0.3.1/pysquril/backends.py
+-rw-r--r--   0        0        0      136 2023-06-22 13:54:05.278837 pysquril-0.3.1/pysquril/exc.py
+-rw-r--r--   0        0        0    21254 2023-06-20 11:11:42.555715 pysquril-0.3.1/pysquril/generator.py
+-rw-r--r--   0        0        0     9452 2023-01-27 11:51:39.899603 pysquril-0.3.1/pysquril/parser.py
+-rw-r--r--   0        0        0     1997 2022-11-21 13:00:47.589558 pysquril-0.3.1/pysquril/test_data.py
+-rw-r--r--   0        0        0    20942 2023-06-26 11:20:09.459378 pysquril-0.3.1/pysquril/tests.py
+-rw-r--r--   0        0        0      658 1970-01-01 00:00:00.000000 pysquril-0.3.1/PKG-INFO
```

### Comparing `pysquril-0.3.0/pyproject.toml` & `pysquril-0.3.1/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "pysquril"
-version = "0.3.0"
+version = "0.3.1"
 description = "Python implementation of structured URI query language"
 repository = "https://github.com/unioslo/pysquril"
 authors = [
     "Leon du Toit <l.c.d.toit@usit.uio.no>",
     "Eirik Haatveit <haatveit@uio.no>",
 ]
```

### Comparing `pysquril-0.3.0/pysquril/backends.py` & `pysquril-0.3.1/pysquril/backends.py`

 * *Files 2% similar despite different names*

```diff
@@ -457,14 +457,15 @@
         tsc = AuditTransaction(self.requestor)
         for row in self.table_select(table_name, uri_query):
             audit_data.append(tsc.event_delete(diff=None, previous=row))
         sql = self.generator_class(f'"{self.schema}{self.sep}{table_name}"', uri_query)
         with sqlite_session(self.engine) as session:
             session.execute(sql.delete_query)
             if not table_name.endswith("_audit"):
+                self.table_create(f'{table_name}_audit', session)
                 self.table_insert(f'{table_name}_audit', audit_data, session)
         return True
 
     def _union_queries(self, uri_query: str, tables: list) -> str:
         queries = []
         for table_name in tables:
             sql = self.generator_class(f'"{self.schema}{self.sep}{table_name}"', uri_query)
@@ -559,17 +560,22 @@
     ) -> bool:
         table_create = f'create table if not exists {self.schema}{self.sep}"{table_name}"{self.table_definition}'
         trigger_create = f"""
             create trigger ensure_unique_data before insert
             on {self.schema}{self.sep}"{table_name}"
             for each row execute procedure unique_data()
         """ # change to create if not exists when pg ^v11
-        session.execute(f'create schema if not exists {self.schema}')
-        session.execute(table_create)
-        session.execute(trigger_create)
+        session.execute( # need to check if table exists
+            f"select exists(select from pg_tables where schemaname = '{self.schema}' and tablename = '{table_name}')"
+        )
+        exists = session.fetchall()[0][0]
+        if not exists:
+            session.execute(f'create schema if not exists {self.schema}')
+            session.execute(table_create)
+            session.execute(trigger_create)
 
 
     def table_insert(
         self,
         table_name: str,
         data: Union[dict, list],
         session: Optional[psycopg2.extensions.cursor] = None,
@@ -639,14 +645,15 @@
         tsc = AuditTransaction(self.requestor)
         for row in self.table_select(table_name, uri_query):
             audit_data.append(tsc.event_delete(diff=None, previous=row))
         sql = self.generator_class(f'{self.schema}{self.sep}"{table_name}"', uri_query)
         with postgres_session(self.engine) as session:
             session.execute(sql.delete_query)
             if not table_name.endswith("_audit"):
+                self.table_create(f'{table_name}_audit', session)
                 self.table_insert(f'{table_name}_audit', audit_data, session)
         return True
 
     def _union_queries(self, uri_query: str, tables: list) -> str:
         queries = []
         for table_name in tables:
             sql = self.generator_class(f'{self.schema}{self.sep}"{table_name}"', uri_query)
```

### Comparing `pysquril-0.3.0/pysquril/generator.py` & `pysquril-0.3.1/pysquril/generator.py`

 * *Files identical despite different names*

### Comparing `pysquril-0.3.0/pysquril/parser.py` & `pysquril-0.3.1/pysquril/parser.py`

 * *Files identical despite different names*

### Comparing `pysquril-0.3.0/pysquril/test_data.py` & `pysquril-0.3.1/pysquril/test_data.py`

 * *Files identical despite different names*

### Comparing `pysquril-0.3.0/pysquril/tests.py` & `pysquril-0.3.1/pysquril/tests.py`

 * *Files 4% similar despite different names*

```diff
@@ -486,14 +486,23 @@
         self.backend.table_delete(table_name=f"{test_table}_audit", uri_query="")
         
         # try to retrieve deleted table's audit table
         select = self.backend.table_select(table_name=f"{test_table}_audit", uri_query="")
         with self.assertRaises((sqlite3.OperationalError, psycopg2.errors.UndefinedTable)):
             next(select)
 
+        # test deleting an entire table, without any updates
+        # automatic audit table creation on delete
+        some_data = {"id": 0, "lol": None, "cat": [1, 2]}
+        some_table = "yay"
+        self.backend.table_insert(table_name=some_table, data=some_data)
+        self.backend.table_delete(table_name=some_table, uri_query="")
+        audit = list(self.backend.table_select(table_name=f"{some_table}_audit", uri_query=""))
+        self.assertEqual(audit[0].get("previous"), some_data)
+
 
 class TestSqliteBackend(TestSqlBackend):
     __test__ = True
 
     def setUp(self) -> None:
         self.directory = tempfile.gettempdir()
         self.file = f"{__package__}_test.db"
```

### Comparing `pysquril-0.3.0/PKG-INFO` & `pysquril-0.3.1/PKG-INFO`

 * *Files 16% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pysquril
-Version: 0.3.0
+Version: 0.3.1
 Summary: Python implementation of structured URI query language
 Home-page: https://github.com/unioslo/pysquril
 Author: Leon du Toit
 Author-email: l.c.d.toit@usit.uio.no
 Requires-Python: >=3.7,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.7
```

