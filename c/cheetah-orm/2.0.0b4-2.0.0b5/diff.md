# Comparing `tmp/cheetah_orm-2.0.0b4-py3-none-any.whl.zip` & `tmp/cheetah_orm-2.0.0b5-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,15 +1,15 @@
-Zip file size: 13886 bytes, number of entries: 13
--rw-rw-rw-  2.0 fat      211 b- defN 23-Jun-25 18:07 cheetah_orm/__init__.py
+Zip file size: 13768 bytes, number of entries: 13
+-rw-rw-rw-  2.0 fat      211 b- defN 23-Jun-26 21:02 cheetah_orm/__init__.py
 -rw-rw-rw-  2.0 fat      849 b- defN 23-Jun-08 21:21 cheetah_orm/constants.py
 -rw-rw-rw-  2.0 fat      483 b- defN 23-Jun-08 20:36 cheetah_orm/error.py
 -rw-rw-rw-  2.0 fat     7695 b- defN 23-Jun-25 04:32 cheetah_orm/fields.py
 -rw-rw-rw-  2.0 fat     2526 b- defN 23-Jun-25 17:24 cheetah_orm/indexes.py
--rw-rw-rw-  2.0 fat    30178 b- defN 23-Jun-25 18:06 cheetah_orm/mappers.py
--rw-rw-rw-  2.0 fat    14124 b- defN 23-Jun-22 17:25 cheetah_orm/migrators.py
+-rw-rw-rw-  2.0 fat    28604 b- defN 23-Jun-26 21:00 cheetah_orm/mappers.py
+-rw-rw-rw-  2.0 fat    14130 b- defN 23-Jun-26 21:08 cheetah_orm/migrators.py
 -rw-rw-rw-  2.0 fat     1898 b- defN 23-Jun-20 03:51 cheetah_orm/model.py
--rw-rw-rw-  2.0 fat     1092 b- defN 23-Jun-25 18:10 cheetah_orm-2.0.0b4.dist-info/LICENSE
--rw-rw-rw-  2.0 fat     6754 b- defN 23-Jun-25 18:10 cheetah_orm-2.0.0b4.dist-info/METADATA
--rw-rw-rw-  2.0 fat       92 b- defN 23-Jun-25 18:10 cheetah_orm-2.0.0b4.dist-info/WHEEL
--rw-rw-rw-  2.0 fat       12 b- defN 23-Jun-25 18:10 cheetah_orm-2.0.0b4.dist-info/top_level.txt
--rw-rw-r--  2.0 fat     1047 b- defN 23-Jun-25 18:10 cheetah_orm-2.0.0b4.dist-info/RECORD
-13 files, 66961 bytes uncompressed, 12146 bytes compressed:  81.9%
+-rw-rw-rw-  2.0 fat     1092 b- defN 23-Jun-26 21:12 cheetah_orm-2.0.0b5.dist-info/LICENSE
+-rw-rw-rw-  2.0 fat     6765 b- defN 23-Jun-26 21:12 cheetah_orm-2.0.0b5.dist-info/METADATA
+-rw-rw-rw-  2.0 fat       92 b- defN 23-Jun-26 21:12 cheetah_orm-2.0.0b5.dist-info/WHEEL
+-rw-rw-rw-  2.0 fat       12 b- defN 23-Jun-26 21:12 cheetah_orm-2.0.0b5.dist-info/top_level.txt
+-rw-rw-r--  2.0 fat     1047 b- defN 23-Jun-26 21:12 cheetah_orm-2.0.0b5.dist-info/RECORD
+13 files, 65404 bytes uncompressed, 12028 bytes compressed:  81.6%
```

## zipnote {}

```diff
@@ -18,23 +18,23 @@
 
 Filename: cheetah_orm/migrators.py
 Comment: 
 
 Filename: cheetah_orm/model.py
 Comment: 
 
-Filename: cheetah_orm-2.0.0b4.dist-info/LICENSE
+Filename: cheetah_orm-2.0.0b5.dist-info/LICENSE
 Comment: 
 
-Filename: cheetah_orm-2.0.0b4.dist-info/METADATA
+Filename: cheetah_orm-2.0.0b5.dist-info/METADATA
 Comment: 
 
-Filename: cheetah_orm-2.0.0b4.dist-info/WHEEL
+Filename: cheetah_orm-2.0.0b5.dist-info/WHEEL
 Comment: 
 
-Filename: cheetah_orm-2.0.0b4.dist-info/top_level.txt
+Filename: cheetah_orm-2.0.0b5.dist-info/top_level.txt
 Comment: 
 
-Filename: cheetah_orm-2.0.0b4.dist-info/RECORD
+Filename: cheetah_orm-2.0.0b5.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## cheetah_orm/__init__.py

```diff
@@ -1,6 +1,6 @@
 """A lightweight and high-performance object-relational mapper for Python."""
 
 __author__    = "Cybermals"
 __copyright__ = "Copyright (c) 2023 by Cybermals"
 __license__   = "MIT"
-__version__   = "2.0.0b4"
+__version__   = "2.0.0b5"
```

## cheetah_orm/mappers.py

```diff
@@ -295,25 +295,14 @@
         """Delete the given model from the database."""
         self._cur.execute(self._cache[model.__class__]["delete"], (model.id,))
 
     def filter(self, model, condition="", *args, **kwargs):
         """Filter data in the database."""
         sql = self._cache[model]["select"]
 
-        # Enclose field names in the condition with backticks
-        parts = condition.split(" ")
-
-        for i, part in enumerate(parts):
-            # Skip operators
-            if "=?" not in part:
-                continue
-
-            part = "`" + part.replace("=?", "`=?")
-            parts[i] = part
-
         # Is there a condition?
         if condition != "":
             sql += f" WHERE {condition}"
 
         # Are there columns to order by?
         if "order_by" in kwargs:
             direction = kwargs.get("order", "ASC")
@@ -335,25 +324,14 @@
         results = [model(**dict(row)) for row in self._cur.fetchall()]
         return results
     
     def count(self, model, condition="", *args, **kwargs):
         """Count data in the database."""
         sql = self._cache[model]["count"]
 
-        # Enclose field names in the condition with backticks
-        parts = condition.split(" ")
-
-        for i, part in enumerate(parts):
-            # Skip operators
-            if "=?" not in part:
-                continue
-
-            part = "`" + part.replace("=?", "`=?")
-            parts[i] = part
-
         # Is there a condition?
         if condition != "":
             sql += f" WHERE {condition}"
 
         sql += ";"
 
         # Execute query and fetch results
@@ -575,27 +553,16 @@
         """Delete the given model from the database."""
         self._cur.execute(self._cache[model.__class__]["delete"], (model.id,))
 
     def filter(self, model, condition="", *args, **kwargs):
         """Filter data in the database."""
         sql = self._cache[model]["select"]
 
-        # Replace "=?" with "=%s" in the condition for MySQL/MariaDB compatibility and enclose field names
-        # in backticks
-        parts = condition.split(" ")
-
-        for i, part in enumerate(parts):
-            # Skip operators
-            if "=?" not in part:
-                continue
-
-            part = "`" + part.replace("=?", "`=%s")
-            parts[i] = part
-
-        condition = " ".join(parts)
+        # Replace "=?" placeholders with "=%s" placeholders in the condition format string
+        condition = condition.replace("=?", "=%s")
 
         # Is there a condition?
         if condition != "":
             sql += f" WHERE {condition}"
 
         # Are there columns to order by?
         if "order_by" in kwargs:
@@ -618,27 +585,16 @@
         results = [model(**dict(row)) for row in self._cur.fetchall()]
         return results
     
     def count(self, model, condition="", *args, **kwargs):
         """Count data in the database."""
         sql = self._cache[model]["count"]
 
-        # Replace "=?" with "=%s" in the condition for MySQL/MariaDB compatibility and enclose field names
-        # in backticks
-        parts = condition.split(" ")
-
-        for i, part in enumerate(parts):
-            # Skip operators
-            if "=?" not in part:
-                continue
-
-            part = "`" + part.replace("=?", "`=%s")
-            parts[i] = part
-
-        condition = " ".join(parts)
+        # Replace "=?" placeholders with "=%s" placeholders in the condition format string
+        condition = condition.replace("=?", "=%s")
 
         # Is there a condition?
         if condition != "":
             sql += f" WHERE {condition}"
 
         sql += ";"
 
@@ -865,26 +821,17 @@
         """Delete the given model from the database."""
         self._cur.execute(self._cache[model.__class__]["delete"], (model.id,))
 
     def filter(self, model, condition="", *args, **kwargs):
         """Filter data in the database."""
         sql = self._cache[model]["select"]
 
-        # Replace "=?" with "=%s" in the condition for PostgreSQL compatibility and quote column names
-        parts = condition.split(" ")
-
-        for i, part in enumerate(parts):
-            # Skip operators
-            if "=?" not in part:
-                continue
-
-            part = '"' + part.replace("=?", '"=%s')
-            parts[i] = part
-
-        condition = " ".join(parts)
+        # Replace "=?" placeholders with "=%s" placeholders and replace backticks with double quotes in the 
+        # condition format string
+        condition = condition.replace("=?", "=%s").replace("`", '"')
 
         # Is there a condition?
         if condition != "":
             sql += f" WHERE {condition}"
 
         # Are there columns to order by?
         if "order_by" in kwargs:
@@ -907,26 +854,17 @@
         results = [model(**dict(row)) for row in self._cur.fetchall()]
         return results
     
     def count(self, model, condition="", *args, **kwargs):
         """Count data in the database."""
         sql = self._cache[model]["count"]
 
-        # Replace "=?" with "=%s" in the condition for PostgreSQL compatibility and quote column names
-        parts = condition.split(" ")
-
-        for i, part in enumerate(parts):
-            # Skip operators
-            if "=?" not in part:
-                continue
-
-            part = '"' + part.replace("=?", '"=%s')
-            parts[i] = part
-
-        condition = " ".join(parts)
+        # Replace "=?" placeholders with "=%s" placeholders and replace backticks with double quotes in the 
+        # condition format string
+        condition = condition.replace("=?", "=%s").replace("`", '"')
 
         # Is there a condition?
         if condition != "":
             sql += f" WHERE {condition}"
 
         sql += ";"
```

## cheetah_orm/migrators.py

```diff
@@ -37,15 +37,15 @@
 
 
 class SQLiteMigrator(Migrator):
     """An SQLite migrator."""
     def migrate(self, model):
         """Migrate a data model if necessary."""
         # Does migration metadata for the given data model exist?
-        records = self._mapper.filter(MigrationMetadata, "name=?", model.table)
+        records = self._mapper.filter(MigrationMetadata, "`name`=?", model.table)
 
         if len(records):
             # Fetch migration metadata and import it
             metadata = records[0]
             fields = json.loads(metadata.fields)
             indexes = json.loads(metadata.indexes)
 
@@ -89,15 +89,15 @@
 
 
 class MySQLMigrator(Migrator):
     """A MySQL migrator."""
     def migrate(self, model):
         """Migrate a data model if necessary."""
         # Does migration metadata for the given data model exist?
-        records = self._mapper.filter(MigrationMetadata, "name=?", model.table)
+        records = self._mapper.filter(MigrationMetadata, "`name`=?", model.table)
 
         if len(records):
             # Fetch migration metadata and import it
             metadata = records[0]
             fields = json.loads(metadata.fields)
             indexes = json.loads(metadata.indexes)
 
@@ -235,15 +235,15 @@
 
 
 class PostgreSQLMigrator(Migrator):
     """A PostgreSQL migrator."""
     def migrate(self, model):
         """Migrate a data model if necessary."""
         # Does migration metadata for the given data model exist?
-        records = self._mapper.filter(MigrationMetadata, "name=?", model.table)
+        records = self._mapper.filter(MigrationMetadata, "`name`=?", model.table)
 
         if len(records):
             # Fetch migration metadata and import it
             metadata = records[0]
             fields = json.loads(metadata.fields)
             indexes = json.loads(metadata.indexes)
```

## Comparing `cheetah_orm-2.0.0b4.dist-info/LICENSE` & `cheetah_orm-2.0.0b5.dist-info/LICENSE`

 * *Files identical despite different names*

## Comparing `cheetah_orm-2.0.0b4.dist-info/METADATA` & `cheetah_orm-2.0.0b5.dist-info/METADATA`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cheetah-orm
-Version: 2.0.0b4
+Version: 2.0.0b5
 Summary: A lightweight and high-performance object-relational mapper for Python.
 Author-email: Cybermals <cybermals@googlegroups.com>
 License: MIT
 Keywords: object-relational mapper
 Classifier: Development Status :: 4 - Beta
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
@@ -43,18 +43,15 @@
 # Features
 * support for sqlite3, MariaDB/MySQL, and PostgreSQL
 * high-level database-neutral API written in pure Python
 * automatically generates the needed SQL statements for whichever database system you prefer to
   use
 * rich filtering API supports any conditional statement that is supported by the underlying database
   system plus sorting, offsets, and limits
-
-
-# Known Bugs
-none
+* result set counting
 
 
 # Usage
 ```python
 #!/usr/bin/python3
 """Cheetah ORM - Demo"""
 
@@ -193,42 +190,42 @@
 
 for user in users:
     print(user)
 
 print()
 
 # Fetch Daniel
-users = mapper.filter(User, "name=?", "Daniel")
+users = mapper.filter(User, "`name`=?", "Daniel")
 print("Users Named 'Daniel':")
 
 for user in users:
     print(user)
 
 print()
 
 # Fetch Leila and Abby
-users = mapper.filter(User, "name=? OR name=?", "Leila", "Abby")
+users = mapper.filter(User, "`name`=? OR `name`=?", "Leila", "Abby")
 print("Users Named 'Leila' or 'Abby':")
 
 for user in users:
     print(user)
 
 print()
 
 # Fetch all users with "Favorite animal?" as their security question ordered by username
-users = mapper.filter(User, "question=?", "Favorite animal?", order_by=["name"])
+users = mapper.filter(User, "`question`=?", "Favorite animal?", order_by=["name"])
 print("Users with the Security Question 'Favorite animal?' Ordered by Username:")
 
 for user in users:
     print(user)
 
 print()
 
 # The middle 2 users
-users = mapper.filter(User, "question=?", "Favorite animal?", order_by=["name"], offset=1, limit=2)
+users = mapper.filter(User, "`question`=?", "Favorite animal?", order_by=["name"], offset=1, limit=2)
 print("The Middle 2 Users:")
 
 for user in users:
     print(user)
 
 print()
 
@@ -276,13 +273,13 @@
 mapper.save_model(post)
 
 # Now delete a user
 mapper.delete_model(fiona)
 mapper.commit()
 
 # Verify that the user's posts were deleted too
-posts = mapper.filter(Post, "user=?", 5)
-print(f"Fiona has {len(posts)} post(s).")
+post_cnt = mapper.count(Post, "`user`=?", 5)
+print(f"Fiona has {post_cnt} post(s).")
 
 # Disconnect from the database
 mapper.disconnect()
 ```
```

