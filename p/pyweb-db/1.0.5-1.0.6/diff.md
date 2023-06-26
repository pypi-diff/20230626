# Comparing `tmp/pyweb_db-1.0.5.tar.gz` & `tmp/pyweb_db-1.0.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyweb_db-1.0.5.tar", last modified: Sun Jun 25 20:13:40 2023, max compression
+gzip compressed data, was "pyweb_db-1.0.6.tar", last modified: Mon Jun 26 11:46:40 2023, max compression
```

## Comparing `pyweb_db-1.0.5.tar` & `pyweb_db-1.0.6.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxrwxrwx   0        0        0        0 2023-06-25 20:13:40.230163 pyweb_db-1.0.5/
--rw-rw-rw-   0        0        0     1059 2023-06-24 13:11:04.000000 pyweb_db-1.0.5/LICENSE
--rw-rw-rw-   0        0        0      590 2023-06-25 20:13:40.231431 pyweb_db-1.0.5/PKG-INFO
--rw-rw-rw-   0        0        0      143 2023-06-25 10:35:20.000000 pyweb_db-1.0.5/README.md
-drwxrwxrwx   0        0        0        0 2023-06-25 20:13:40.188022 pyweb_db-1.0.5/pyweb_db/
--rw-rw-rw-   0        0        0     8573 2023-06-25 20:13:23.000000 pyweb_db-1.0.5/pyweb_db/__init__.py
--rw-rw-rw-   0        0        0     4707 2023-06-25 19:54:48.000000 pyweb_db-1.0.5/pyweb_db/main.py
-drwxrwxrwx   0        0        0        0 2023-06-25 20:13:40.228080 pyweb_db-1.0.5/pyweb_db.egg-info/
--rw-rw-rw-   0        0        0      590 2023-06-25 20:13:39.000000 pyweb_db-1.0.5/pyweb_db.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      233 2023-06-25 20:13:40.000000 pyweb_db-1.0.5/pyweb_db.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-25 20:13:39.000000 pyweb_db-1.0.5/pyweb_db.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        9 2023-06-25 20:13:39.000000 pyweb_db-1.0.5/pyweb_db.egg-info/requires.txt
--rw-rw-rw-   0        0        0        9 2023-06-25 20:13:39.000000 pyweb_db-1.0.5/pyweb_db.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       84 2023-06-25 20:13:40.234382 pyweb_db-1.0.5/setup.cfg
--rw-rw-rw-   0        0        0      686 2023-06-25 19:55:06.000000 pyweb_db-1.0.5/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-26 11:46:40.751739 pyweb_db-1.0.6/
+-rw-rw-rw-   0        0        0     1059 2023-06-24 13:11:04.000000 pyweb_db-1.0.6/LICENSE
+-rw-rw-rw-   0        0        0      590 2023-06-26 11:46:40.751739 pyweb_db-1.0.6/PKG-INFO
+-rw-rw-rw-   0        0        0      143 2023-06-25 10:35:20.000000 pyweb_db-1.0.6/README.md
+drwxrwxrwx   0        0        0        0 2023-06-26 11:46:40.726791 pyweb_db-1.0.6/pyweb_db/
+-rw-rw-rw-   0        0        0    10204 2023-06-26 11:45:52.000000 pyweb_db-1.0.6/pyweb_db/__init__.py
+-rw-rw-rw-   0        0        0     4707 2023-06-26 11:45:20.000000 pyweb_db-1.0.6/pyweb_db/main.py
+drwxrwxrwx   0        0        0        0 2023-06-26 11:46:40.749744 pyweb_db-1.0.6/pyweb_db.egg-info/
+-rw-rw-rw-   0        0        0      590 2023-06-26 11:46:40.000000 pyweb_db-1.0.6/pyweb_db.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      233 2023-06-26 11:46:40.000000 pyweb_db-1.0.6/pyweb_db.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-26 11:46:40.000000 pyweb_db-1.0.6/pyweb_db.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        9 2023-06-26 11:46:40.000000 pyweb_db-1.0.6/pyweb_db.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        9 2023-06-26 11:46:40.000000 pyweb_db-1.0.6/pyweb_db.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       84 2023-06-26 11:46:40.753733 pyweb_db-1.0.6/setup.cfg
+-rw-rw-rw-   0        0        0      686 2023-06-26 11:46:00.000000 pyweb_db-1.0.6/setup.py
```

### Comparing `pyweb_db-1.0.5/LICENSE` & `pyweb_db-1.0.6/LICENSE`

 * *Files identical despite different names*

### Comparing `pyweb_db-1.0.5/PKG-INFO` & `pyweb_db-1.0.6/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyweb_db
-Version: 1.0.5
+Version: 1.0.6
 Summary: This is a simple JSON-based database library
 Author: PyWebSol
 Author-email: pywebsol@gmail.com
 Keywords: database python json pywebsol
 Classifier: Programming Language :: Python :: 3.11
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `pyweb_db-1.0.5/pyweb_db/__init__.py` & `pyweb_db-1.0.6/pyweb_db/__init__.py`

 * *Files 7% similar despite different names*

```diff
@@ -54,14 +54,30 @@
         if table_name in db_content:
             for data in datas:
                 if (not data in db_content[table_name] and unique == True):
                     db_content[table_name].append(data)
                 elif unique == False:
                     db_content[table_name].append(data)
             await self.save_data(db_content)
+    
+    async def insert_datas_into_tables(self, table_names: list, datas: list, unique: bool = False):
+        db_content = await self.load_data()
+        if not type(datas) == list:
+            print(f'INCORRECT TYPE!\n{datas}')
+            return
+        if not type(table_names) == list:
+            print(f'INCORRECT TYPE!\n{table_names}')
+            return
+        for table_name, data in zip(table_names, datas):
+            if table_name in db_content:
+                if (not data in db_content[table_name] and unique == True):
+                    db_content[table_name].append(data)
+                elif unique == False:
+                    db_content[table_name].append(data)
+            await self.save_data(db_content)
 
     async def delete_from_table(self, table_name: str, data):
         db_content = await self.load_data()
         if table_name in db_content:
             if data in db_content[table_name]:
                 db_content[table_name].remove(data)
                 await self.save_data(db_content)
@@ -148,14 +164,32 @@
                 for data in datas:
                     if (not data in db_content[table_name] and unique == True):
                         db_content[table_name].append(data)
                     elif unique == False:
                         db_content[table_name].append(data)
                 file.seek(0)
                 json.dump(db_content, file)
+    
+    def insert_datas_into_tables(self, table_names: list, datas: list, unique: bool = False):
+        with open(self.path, 'r+', encoding='utf-8') as file:
+            db_content = json.load(file)
+            if not type(datas) == list:
+                print(f'INCORRECT TYPE!\n{datas}')
+                return
+            if not type(table_names) == list:
+                print(f'INCORRECT TYPE!\n{table_names}')
+                return
+            for table_name, data in zip(table_names, datas):
+                if table_name in db_content:
+                    if (not data in db_content[table_name] and unique == True):
+                        db_content[table_name].append(data)
+                    elif unique == False:
+                        db_content[table_name].append(data)
+                file.seek(0)
+                json.dump(db_content, file)
 
     def delete_from_table(self, table_name: str, data):
         with open(self.path, 'r+', encoding='utf-8') as file:
             db_content = json.load(file)
             if table_name in db_content:
                 if data in db_content[table_name]:
                     db_content[table_name].remove(data)
```

### Comparing `pyweb_db-1.0.5/pyweb_db/main.py` & `pyweb_db-1.0.6/pyweb_db/main.py`

 * *Files identical despite different names*

### Comparing `pyweb_db-1.0.5/pyweb_db.egg-info/PKG-INFO` & `pyweb_db-1.0.6/pyweb_db.egg-info/PKG-INFO`

 * *Files 20% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyweb-db
-Version: 1.0.5
+Version: 1.0.6
 Summary: This is a simple JSON-based database library
 Author: PyWebSol
 Author-email: pywebsol@gmail.com
 Keywords: database python json pywebsol
 Classifier: Programming Language :: Python :: 3.11
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `pyweb_db-1.0.5/setup.py` & `pyweb_db-1.0.6/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 
 def readme():
   with open('README.md', 'r', encoding='utf-8') as f:
     return f.read()
 
 setup(
   name='pyweb_db',
-  version='1.0.5',
+  version='1.0.6',
   author='PyWebSol',
   author_email='pywebsol@gmail.com',
   description='This is a simple JSON-based database library',
   long_description=readme(),
   long_description_content_type='text/markdown',
   packages=find_packages(),
   install_requires=['aiofiles'],
```

