# Comparing `tmp/pysquril-0.2.2.tar.gz` & `tmp/pysquril-0.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pysquril-0.2.2.tar", max compression
+gzip compressed data, was "pysquril-0.3.0.tar", max compression
```

## Comparing `pysquril-0.2.2.tar` & `pysquril-0.3.0.tar`

### file list

```diff
@@ -1,10 +1,9 @@
--rw-r--r--   0        0        0      477 2023-02-17 09:07:38.215673 pysquril-0.2.2/pyproject.toml
--rw-r--r--   0        0        0        0 2023-02-02 16:22:52.725280 pysquril-0.2.2/pysquril/__init__.py
--rw-r--r--   0        0        0    15247 2023-02-10 13:33:00.691300 pysquril-0.2.2/pysquril/backends.py
--rw-r--r--   0        0        0       39 2023-02-03 08:50:40.059099 pysquril-0.2.2/pysquril/exc.py
--rw-r--r--   0        0        0    21254 2023-02-10 13:33:00.691913 pysquril-0.2.2/pysquril/generator.py
--rw-r--r--   0        0        0     9452 2023-02-03 08:50:40.060339 pysquril-0.2.2/pysquril/parser.py
--rw-r--r--   0        0        0     1997 2023-02-02 16:22:52.726626 pysquril-0.2.2/pysquril/test_data.py
--rw-r--r--   0        0        0    18059 2023-02-10 13:33:00.692504 pysquril-0.2.2/pysquril/tests.py
--rw-r--r--   0        0        0      690 1970-01-01 00:00:00.000000 pysquril-0.2.2/setup.py
--rw-r--r--   0        0        0      658 1970-01-01 00:00:00.000000 pysquril-0.2.2/PKG-INFO
+-rw-r--r--   0        0        0      524 2023-06-26 08:48:57.055407 pysquril-0.3.0/pyproject.toml
+-rw-r--r--   0        0        0        0 2022-06-22 08:13:57.003868 pysquril-0.3.0/pysquril/__init__.py
+-rw-r--r--   0        0        0    24504 2023-06-26 08:26:43.181491 pysquril-0.3.0/pysquril/backends.py
+-rw-r--r--   0        0        0      136 2023-06-22 13:54:05.278837 pysquril-0.3.0/pysquril/exc.py
+-rw-r--r--   0        0        0    21254 2023-06-20 11:11:42.555715 pysquril-0.3.0/pysquril/generator.py
+-rw-r--r--   0        0        0     9452 2023-01-27 11:51:39.899603 pysquril-0.3.0/pysquril/parser.py
+-rw-r--r--   0        0        0     1997 2022-11-21 13:00:47.589558 pysquril-0.3.0/pysquril/test_data.py
+-rw-r--r--   0        0        0    20442 2023-06-25 19:23:30.096636 pysquril-0.3.0/pysquril/tests.py
+-rw-r--r--   0        0        0      658 1970-01-01 00:00:00.000000 pysquril-0.3.0/PKG-INFO
```

### Comparing `pysquril-0.2.2/pysquril/generator.py` & `pysquril-0.3.0/pysquril/generator.py`

 * *Files identical despite different names*

### Comparing `pysquril-0.2.2/pysquril/parser.py` & `pysquril-0.3.0/pysquril/parser.py`

 * *Files identical despite different names*

### Comparing `pysquril-0.2.2/pysquril/test_data.py` & `pysquril-0.3.0/pysquril/test_data.py`

 * *Files identical despite different names*

### Comparing `pysquril-0.2.2/pysquril/tests.py` & `pysquril-0.3.0/pysquril/tests.py`

 * *Files 7% similar despite different names*

```diff
@@ -62,63 +62,46 @@
         ) -> list:
             out = []
             if verbose:
                 print(colored(uri_query, 'magenta'))
             q = SqlGeneratorCls(table, uri_query)
             if verbose:
                 print(colored(q.select_query, 'yellow'))
-            with session_func(engine) as session:
-                session.execute(q.select_query)
-                resp = session.fetchall()
-            for row in resp:
-                target = row[0]
-                if isinstance(target, dict) or isinstance(target, list):
-                    _in = target
-                else:
-                    _in = json.loads(target)
-                out.append(_in)
+            db = DbBackendCls(engine)
+            out = list(db.table_select(table, uri_query))
             if verbose:
                 print(out)
             return out
 
         def run_update_query(
             uri_query: str,
             table: str = 'test_table',
             engine: Union[sqlite3.Connection, psycopg2.pool.SimpleConnectionPool] = engine,
             verbose: bool = verbose,
             data: list = data,
         ) -> list:
             q = SqlGeneratorCls(table, uri_query, data=data)
             if verbose:
                 print(colored(q.update_query, 'cyan'))
-            with session_func(engine) as session:
-                session.execute(q.update_query)
-            with session_func(engine) as session:
-                session.execute(f'select * from {table}')
-                resp = session.fetchall()
-            for row in resp:
-                target = row[0]
-                if isinstance(target, dict):
-                    _in = target
-                else:
-                    _in = json.loads(target)
-                out.append(_in)
+            db = DbBackendCls(engine)
+            db.table_update(table, uri_query, data)
+            out = list(db.table_select(table, ""))
             return out
 
         def run_delete_query(
             uri_query: str,
             table: str = 'test_table',
             engine: Union[sqlite3.Connection, psycopg2.pool.SimpleConnectionPool] = engine,
             verbose: bool = verbose,
         ) -> bool:
             q = SqlGeneratorCls(table, uri_query)
             if verbose:
                 print(q.delete_query)
-            with session_func(engine) as session:
-                session.execute(q.delete_query)
+            db = DbBackendCls(engine)
+            db.table_delete(table, uri_query)
             return True
 
         db = DbBackendCls(engine)
         try:
             db.table_delete('test_table', '')
         except Exception as e:
             pass
@@ -355,15 +338,15 @@
         assert out == []
         out = run_delete_query('')
         with pytest.raises(Exception):
             out = run_delete_query('')
 
 
 
-    def test_sqlite(self):
+    def sqlite(self):
         engine = sqlite_init('/tmp', name='api-test.db')
         self.run_backend_tests(
             self.data,
             engine,
             sqlite_session,
             SqliteQueryGenerator,
             SqliteBackend,
@@ -401,50 +384,117 @@
     
     backend: Union[SqliteBackend, PostgresBackend]
     engine: Union[sqlite3.Connection, psycopg2.pool.SimpleConnectionPool]
 
     def test_audit(self) -> bool:
         test_table = "just_an_average_audit_test_table"
 
+        pkey = "id"
+
         key_to_update = "key1"
         original_value = 5
 
-        data = {key_to_update: original_value, "key2": "a"}
+        data = {pkey: 1, key_to_update: original_value, "key2": "a"}
+        more_data = {pkey: 2, key_to_update: original_value, "key3": {"moar": "things"}}
+
         self.backend.table_insert(table_name=test_table, data=data)
-        update_data = {key_to_update: original_value+1}
+        self.backend.table_insert(table_name=test_table, data=more_data)
 
         # update the table with the new data
-        self.backend.table_update(table_name=test_table, uri_query=f"set={key_to_update}&where={key_to_update}=eq.{original_value}", data=update_data)
+        new_data = {key_to_update: original_value+1}
+
+        self.backend.table_update(
+            table_name=test_table,
+            uri_query=f"set={key_to_update}&where={key_to_update}=eq.{original_value}",
+            data=new_data,
+        )
         result = list(self.backend.table_select(table_name=test_table, uri_query=""))
         self.assertTrue(result)
-        retrieved_data = result[-1]
-        self.assertEqual(retrieved_data, {**data, **update_data})
+        retrieved_data = result[0]
+        self.assertEqual(retrieved_data, {**data, **new_data})
         self.assertNotEqual(retrieved_data[key_to_update], original_value)
-        self.assertEqual(retrieved_data[key_to_update], update_data[key_to_update])
+        self.assertEqual(retrieved_data[key_to_update], new_data[key_to_update])
 
         # view update audit data
-        result = list(self.backend.table_select(table_name=f"{test_table}_audit", uri_query=""))
+        result = list(self.backend.table_select(
+            table_name=f"{test_table}_audit", uri_query="order=timestamp.asc")
+        )
         self.assertTrue(result)
-        audit_event = result[-1]
+        audit_event = result[0]
         self.assertEqual(audit_event["previous"], data)
-        self.assertEqual(audit_event["diff"], update_data)
+        self.assertEqual(audit_event["diff"], new_data)
+        self.assertEqual(audit_event["event"], "update")
+        self.assertTrue(audit_event["transaction_id"] is not None)
+        self.assertTrue(audit_event["event_id"] is not None)
+        self.assertTrue(audit_event["timestamp"] is not None)
+
+        # rollback updates
+        with self.assertRaises(ParseError): # missing rollback directive
+            self.backend.table_restore(table_name=test_table, uri_query="")
+        with self.assertRaises(ParseError): # missing primary key
+            self.backend.table_restore(table_name=test_table, uri_query="rollback")
+        with self.assertRaises(ParseError): # still missing primary key
+            self.backend.table_restore(table_name=test_table, uri_query="rollback&primary_key=")
+
+        # rollback to a specific state, for a specific row
+        result = self.backend.table_restore(
+            table_name=test_table,
+            uri_query=f"rollback&primary_key={pkey}&where=event_id=eq.{audit_event.get('event_id')}"
+        )
+        self.assertEqual(len(result.get("updates")), 1)
+        self.assertEqual(len(result.get("restores")), 0)
+        result = list(self.backend.table_select(table_name=test_table, uri_query="where=id=eq.1"))
+        self.assertEqual(result[0].get(key_to_update), original_value)
+
+        # delete a specific entry
+        self.backend.table_delete(table_name=test_table, uri_query="where=key3=not.is.null")
+        result = list(self.backend.table_select(table_name=f"{test_table}_audit", uri_query=""))
+        self.assertEqual(len(result), 4)
+
+        # restore the deleted entry
+        result = self.backend.table_restore(
+            table_name=test_table,
+            uri_query=f"rollback&primary_key={pkey}&where=event=eq.delete"
+        )
+        self.assertEqual(len(result.get("updates")), 0)
+        self.assertEqual(len(result.get("restores")), 1)
+        result = list(self.backend.table_select(table_name=test_table, uri_query="where=id=eq.2"))
+        self.assertTrue(result[0] is not None)
 
         # delete the table
         self.backend.table_delete(table_name=test_table, uri_query="")
 
+        # check that the deletes are in the audit
+        result = list(self.backend.table_select(table_name=f"{test_table}_audit", uri_query=""))
+        self.assertEqual(len(result), 7)
+
+        # restore everything TODO
+        result = self.backend.table_restore(table_name=test_table, uri_query=f"rollback&primary_key={pkey}")
+        self.assertTrue(result is not None)
+        result = list(self.backend.table_select(table_name=test_table, uri_query="order=id.asc"))
+        self.assertEqual(result[0], data)
+        self.assertEqual(result[1], more_data)
+
+        # delete the table (again)
+        self.backend.table_delete(table_name=test_table, uri_query="")
+
         # try to retrieve deleted table
         select = self.backend.table_select(table_name=test_table, uri_query="")
         with self.assertRaises((sqlite3.OperationalError, psycopg2.errors.UndefinedTable)):
             next(select)
+
+        # delete the audit table
+        self.backend.table_delete(table_name=f"{test_table}_audit", uri_query="")
         
         # try to retrieve deleted table's audit table
         select = self.backend.table_select(table_name=f"{test_table}_audit", uri_query="")
         with self.assertRaises((sqlite3.OperationalError, psycopg2.errors.UndefinedTable)):
             next(select)
 
+
 class TestSqliteBackend(TestSqlBackend):
     __test__ = True
 
     def setUp(self) -> None:
         self.directory = tempfile.gettempdir()
         self.file = f"{__package__}_test.db"
         self.engine = sqlite_init(self.directory, name=self.file)
```

### Comparing `pysquril-0.2.2/PKG-INFO` & `pysquril-0.3.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pysquril
-Version: 0.2.2
+Version: 0.3.0
 Summary: Python implementation of structured URI query language
 Home-page: https://github.com/unioslo/pysquril
 Author: Leon du Toit
 Author-email: l.c.d.toit@usit.uio.no
 Requires-Python: >=3.7,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.7
```

