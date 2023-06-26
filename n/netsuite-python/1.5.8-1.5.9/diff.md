# Comparing `tmp/netsuite_python-1.5.8.tar.gz` & `tmp/netsuite_python-1.5.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "netsuite_python-1.5.8.tar", last modified: Fri May 19 19:17:08 2023, max compression
+gzip compressed data, was "netsuite_python-1.5.9.tar", last modified: Mon Jun 26 17:16:53 2023, max compression
```

## Comparing `netsuite_python-1.5.8.tar` & `netsuite_python-1.5.9.tar`

### file list

```diff
@@ -1,39 +1,39 @@
-drwxrwxrwx   0        0        0        0 2023-05-19 19:17:08.560851 netsuite_python-1.5.8/
--rw-rw-rw-   0        0        0     5438 2023-05-19 19:17:08.560851 netsuite_python-1.5.8/PKG-INFO
--rw-rw-rw-   0        0        0     5108 2023-04-25 19:14:38.000000 netsuite_python-1.5.8/README.md
-drwxrwxrwx   0        0        0        0 2023-05-19 19:17:08.541852 netsuite_python-1.5.8/netsuite/
--rw-rw-rw-   0        0        0    12072 2023-04-25 18:30:40.000000 netsuite_python-1.5.8/netsuite/Netsuite.py
--rw-rw-rw-   0        0        0      494 2023-02-12 19:28:31.000000 netsuite_python-1.5.8/netsuite/NetsuiteToken.py
--rw-rw-rw-   0        0        0       74 2023-02-12 19:28:31.000000 netsuite_python-1.5.8/netsuite/__init__.py
-drwxrwxrwx   0        0        0        0 2023-05-19 19:17:08.545854 netsuite_python-1.5.8/netsuite/api_clients/
--rw-rw-rw-   0        0        0      235 2023-04-09 19:43:22.000000 netsuite_python-1.5.8/netsuite/api_clients/__init__.py
-drwxrwxrwx   0        0        0        0 2023-05-19 19:17:08.547852 netsuite_python-1.5.8/netsuite/api_clients/api/
--rw-rw-rw-   0        0        0       59 2023-04-09 19:48:25.000000 netsuite_python-1.5.8/netsuite/api_clients/api/__init__.py
--rw-rw-rw-   0        0        0     5489 2023-04-09 19:49:23.000000 netsuite_python-1.5.8/netsuite/api_clients/api/query_api.py
--rw-rw-rw-   0        0        0     2518 2023-05-19 19:16:57.000000 netsuite_python-1.5.8/netsuite/api_clients/api/restlet_api.py
--rw-rw-rw-   0        0        0    25577 2023-04-09 19:51:26.000000 netsuite_python-1.5.8/netsuite/api_clients/api_client.py
--rw-rw-rw-   0        0        0     8466 2023-03-23 15:55:18.000000 netsuite_python-1.5.8/netsuite/api_clients/configuration.py
--rw-rw-rw-   0        0        0    13259 2023-04-06 18:39:08.000000 netsuite_python-1.5.8/netsuite/api_clients/rest.py
--rw-rw-rw-   0        0        0      243 2023-02-12 19:28:31.000000 netsuite_python-1.5.8/netsuite/exceptions.py
--rw-rw-rw-   0        0        0     3921 2023-02-12 19:28:31.000000 netsuite_python-1.5.8/netsuite/module_loading.py
-drwxrwxrwx   0        0        0        0 2023-05-19 19:17:08.549851 netsuite_python-1.5.8/netsuite/netsuite_rest_client/
--rw-rw-rw-   0        0        0        0 2023-04-25 17:05:59.000000 netsuite_python-1.5.8/netsuite/netsuite_rest_client/__init__.py
--rw-rw-rw-   0        0        0      463 2023-04-17 18:07:52.000000 netsuite_python-1.5.8/netsuite/netsuite_rest_client/rest_api_client.py
-drwxrwxrwx   0        0        0        0 2023-05-19 19:17:08.550852 netsuite_python-1.5.8/netsuite/scripts/
--rw-rw-rw-   0        0        0        0 2023-02-12 19:28:31.000000 netsuite_python-1.5.8/netsuite/scripts/__init__.py
--rw-rw-rw-   0        0        0    11634 2023-04-28 19:27:52.000000 netsuite_python-1.5.8/netsuite/scripts/cli.py
--rw-rw-rw-   0        0        0     6300 2023-04-17 18:30:20.000000 netsuite_python-1.5.8/netsuite/settings.py
-drwxrwxrwx   0        0        0        0 2023-05-19 19:17:08.554851 netsuite_python-1.5.8/netsuite/storages/
--rw-rw-rw-   0        0        0      324 2023-02-12 19:28:31.000000 netsuite_python-1.5.8/netsuite/storages/BaseStorage.py
--rw-rw-rw-   0        0        0      653 2023-02-12 19:28:31.000000 netsuite_python-1.5.8/netsuite/storages/InMemoryStorage.py
--rw-rw-rw-   0        0        0     1594 2023-02-12 19:28:31.000000 netsuite_python-1.5.8/netsuite/storages/JSONStorage.py
--rw-rw-rw-   0        0        0      119 2023-02-12 19:28:31.000000 netsuite_python-1.5.8/netsuite/storages/__init__.py
-drwxrwxrwx   0        0        0        0 2023-05-19 19:17:08.559852 netsuite_python-1.5.8/netsuite_python.egg-info/
--rw-rw-rw-   0        0        0     5438 2023-05-19 19:17:08.000000 netsuite_python-1.5.8/netsuite_python.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      920 2023-05-19 19:17:08.000000 netsuite_python-1.5.8/netsuite_python.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-19 19:17:08.000000 netsuite_python-1.5.8/netsuite_python.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       55 2023-05-19 19:17:08.000000 netsuite_python-1.5.8/netsuite_python.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0       81 2023-05-19 19:17:08.000000 netsuite_python-1.5.8/netsuite_python.egg-info/requires.txt
--rw-rw-rw-   0        0        0        9 2023-05-19 19:17:08.000000 netsuite_python-1.5.8/netsuite_python.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-05-19 19:17:08.560851 netsuite_python-1.5.8/setup.cfg
--rw-rw-rw-   0        0        0      961 2023-05-19 19:17:03.000000 netsuite_python-1.5.8/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-26 17:16:53.847256 netsuite_python-1.5.9/
+-rw-rw-rw-   0        0        0     5438 2023-06-26 17:16:53.847256 netsuite_python-1.5.9/PKG-INFO
+-rw-rw-rw-   0        0        0     5108 2023-04-25 19:14:38.000000 netsuite_python-1.5.9/README.md
+drwxrwxrwx   0        0        0        0 2023-06-26 17:16:53.814255 netsuite_python-1.5.9/netsuite/
+-rw-rw-rw-   0        0        0    12080 2023-06-26 17:14:03.000000 netsuite_python-1.5.9/netsuite/Netsuite.py
+-rw-rw-rw-   0        0        0      494 2023-02-12 19:28:31.000000 netsuite_python-1.5.9/netsuite/NetsuiteToken.py
+-rw-rw-rw-   0        0        0       74 2023-02-12 19:28:31.000000 netsuite_python-1.5.9/netsuite/__init__.py
+drwxrwxrwx   0        0        0        0 2023-06-26 17:16:53.823256 netsuite_python-1.5.9/netsuite/api_clients/
+-rw-rw-rw-   0        0        0      235 2023-04-09 19:43:22.000000 netsuite_python-1.5.9/netsuite/api_clients/__init__.py
+drwxrwxrwx   0        0        0        0 2023-06-26 17:16:53.828255 netsuite_python-1.5.9/netsuite/api_clients/api/
+-rw-rw-rw-   0        0        0       59 2023-04-09 19:48:25.000000 netsuite_python-1.5.9/netsuite/api_clients/api/__init__.py
+-rw-rw-rw-   0        0        0     5489 2023-04-09 19:49:23.000000 netsuite_python-1.5.9/netsuite/api_clients/api/query_api.py
+-rw-rw-rw-   0        0        0     2579 2023-05-19 19:55:49.000000 netsuite_python-1.5.9/netsuite/api_clients/api/restlet_api.py
+-rw-rw-rw-   0        0        0    25577 2023-04-09 19:51:26.000000 netsuite_python-1.5.9/netsuite/api_clients/api_client.py
+-rw-rw-rw-   0        0        0     8466 2023-03-23 15:55:18.000000 netsuite_python-1.5.9/netsuite/api_clients/configuration.py
+-rw-rw-rw-   0        0        0    13259 2023-04-06 18:39:08.000000 netsuite_python-1.5.9/netsuite/api_clients/rest.py
+-rw-rw-rw-   0        0        0      243 2023-02-12 19:28:31.000000 netsuite_python-1.5.9/netsuite/exceptions.py
+-rw-rw-rw-   0        0        0     3921 2023-02-12 19:28:31.000000 netsuite_python-1.5.9/netsuite/module_loading.py
+drwxrwxrwx   0        0        0        0 2023-06-26 17:16:53.831255 netsuite_python-1.5.9/netsuite/netsuite_rest_client/
+-rw-rw-rw-   0        0        0        0 2023-04-25 17:05:59.000000 netsuite_python-1.5.9/netsuite/netsuite_rest_client/__init__.py
+-rw-rw-rw-   0        0        0      463 2023-04-17 18:07:52.000000 netsuite_python-1.5.9/netsuite/netsuite_rest_client/rest_api_client.py
+drwxrwxrwx   0        0        0        0 2023-06-26 17:16:53.833255 netsuite_python-1.5.9/netsuite/scripts/
+-rw-rw-rw-   0        0        0        0 2023-02-12 19:28:31.000000 netsuite_python-1.5.9/netsuite/scripts/__init__.py
+-rw-rw-rw-   0        0        0    12245 2023-06-26 17:12:39.000000 netsuite_python-1.5.9/netsuite/scripts/cli.py
+-rw-rw-rw-   0        0        0     6300 2023-04-17 18:30:20.000000 netsuite_python-1.5.9/netsuite/settings.py
+drwxrwxrwx   0        0        0        0 2023-06-26 17:16:53.841255 netsuite_python-1.5.9/netsuite/storages/
+-rw-rw-rw-   0        0        0      324 2023-02-12 19:28:31.000000 netsuite_python-1.5.9/netsuite/storages/BaseStorage.py
+-rw-rw-rw-   0        0        0      653 2023-02-12 19:28:31.000000 netsuite_python-1.5.9/netsuite/storages/InMemoryStorage.py
+-rw-rw-rw-   0        0        0     1594 2023-02-12 19:28:31.000000 netsuite_python-1.5.9/netsuite/storages/JSONStorage.py
+-rw-rw-rw-   0        0        0      119 2023-02-12 19:28:31.000000 netsuite_python-1.5.9/netsuite/storages/__init__.py
+drwxrwxrwx   0        0        0        0 2023-06-26 17:16:53.846255 netsuite_python-1.5.9/netsuite_python.egg-info/
+-rw-rw-rw-   0        0        0     5438 2023-06-26 17:16:53.000000 netsuite_python-1.5.9/netsuite_python.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      920 2023-06-26 17:16:53.000000 netsuite_python-1.5.9/netsuite_python.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-26 17:16:53.000000 netsuite_python-1.5.9/netsuite_python.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       55 2023-06-26 17:16:53.000000 netsuite_python-1.5.9/netsuite_python.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0       81 2023-06-26 17:16:53.000000 netsuite_python-1.5.9/netsuite_python.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        9 2023-06-26 17:16:53.000000 netsuite_python-1.5.9/netsuite_python.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-06-26 17:16:53.847256 netsuite_python-1.5.9/setup.cfg
+-rw-rw-rw-   0        0        0      961 2023-06-26 17:15:56.000000 netsuite_python-1.5.9/setup.py
```

### Comparing `netsuite_python-1.5.8/PKG-INFO` & `netsuite_python-1.5.9/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: netsuite_python
-Version: 1.5.8
+Version: 1.5.9
 Summary: Python SDK for Netsuite API with Flask Integration
 Home-page: https://bitbucket.org/theapiguys/netsuite_python
 Author: Will @ TheAPIGuys
 Author-email: will@theapiguys.com
 License: UNKNOWN
 Platform: UNKNOWN
 Description-Content-Type: text/markdown
```

### Comparing `netsuite_python-1.5.8/README.md` & `netsuite_python-1.5.9/README.md`

 * *Files identical despite different names*

### Comparing `netsuite_python-1.5.8/netsuite/Netsuite.py` & `netsuite_python-1.5.9/netsuite/Netsuite.py`

 * *Files 1% similar despite different names*

```diff
@@ -213,24 +213,24 @@
         print('Extracting....')
         file = zipfile.ZipFile(BytesIO(req.content))
         file.extractall(path=self.api_settings.NETSUITE_CLIENT_PATH)
 
 
         client_src = Path.joinpath(Path(self.api_settings.NETSUITE_CLIENT_PATH), f'python-client/netsuite_rest_client')
         class_src = Path.joinpath(Path(netsuite.settings.PACKAGE_DIR), f'netsuite_rest_client/rest_api_client.py')
-        docs_src = Path.joinpath(Path(self.api_settings.NETSUITE_CLIENT_PATH), f'python-client/docs')
+        # docs_src = Path.joinpath(Path(self.api_settings.NETSUITE_CLIENT_PATH), f'python-client/docs')
         readme_src = Path.joinpath(Path(self.api_settings.NETSUITE_CLIENT_PATH), f'python-client/README.md')
 
         dst = Path(f'{self.api_settings.NETSUITE_CLIENT_PATH}')
-        docs_dst = Path.joinpath(Path(self.api_settings.NETSUITE_CLIENT_PATH), f'docs')
+        # docs_dst = Path.joinpath(Path(self.api_settings.NETSUITE_CLIENT_PATH), f'docs')
         print(f'Copying to: {dst}')
         shutil.copytree(client_src, dst, symlinks=True, ignore=None, ignore_dangling_symlinks=False,
                         dirs_exist_ok=True)
-        shutil.copytree(docs_src, docs_dst, symlinks=True, ignore=None, ignore_dangling_symlinks=False,
-                        dirs_exist_ok=True)
+        # shutil.copytree(docs_src, docs_dst, symlinks=True, ignore=None, ignore_dangling_symlinks=False,
+        #                 dirs_exist_ok=True)
 
         shutil.copy(class_src, dst)
         shutil.copy(readme_src, dst)
 
 
         shutil.rmtree(Path.joinpath(Path(self.api_settings.NETSUITE_CLIENT_PATH), 'python-client'))
         print('temp folder was removed.')
```

### Comparing `netsuite_python-1.5.8/netsuite/api_clients/api/query_api.py` & `netsuite_python-1.5.9/netsuite/api_clients/api/query_api.py`

 * *Files identical despite different names*

### Comparing `netsuite_python-1.5.8/netsuite/api_clients/api/restlet_api.py` & `netsuite_python-1.5.9/netsuite/api_clients/api/restlet_api.py`

 * *Files 6% similar despite different names*

```diff
@@ -68,8 +68,10 @@
                         if type(response.get("results")) is list:
                             return response.get("results")
                         else:
                             items = [response.get("results")]
                             return items
                 except ValueError:
                     pass
+                except TypeError:
+                    pass
         return response
```

### Comparing `netsuite_python-1.5.8/netsuite/api_clients/api_client.py` & `netsuite_python-1.5.9/netsuite/api_clients/api_client.py`

 * *Files identical despite different names*

### Comparing `netsuite_python-1.5.8/netsuite/api_clients/configuration.py` & `netsuite_python-1.5.9/netsuite/api_clients/configuration.py`

 * *Files identical despite different names*

### Comparing `netsuite_python-1.5.8/netsuite/api_clients/rest.py` & `netsuite_python-1.5.9/netsuite/api_clients/rest.py`

 * *Files identical despite different names*

### Comparing `netsuite_python-1.5.8/netsuite/module_loading.py` & `netsuite_python-1.5.9/netsuite/module_loading.py`

 * *Files identical despite different names*

### Comparing `netsuite_python-1.5.8/netsuite/scripts/cli.py` & `netsuite_python-1.5.9/netsuite/scripts/cli.py`

 * *Files 2% similar despite different names*

```diff
@@ -212,62 +212,71 @@
 def generate_rest_client():
     generate_netsuite_rest_client()
 
 def generate_netsuite_rest_client():
     ns_records_to_include = []
     print (" ----- Rest Client Generator -----")
     netsuite = Netsuite()
-    needs_other_recordtypes = prompt("Will you be using record types other than customer?", type=click.BOOL, default=True)
-
-
-    if needs_other_recordtypes:
-        display_ns_classes = prompt("List available Netsuite Records?", type=click.BOOL, default=True)
-        print("")
-        records = netsuite.get_netsuite_recordtypes()
-        if display_ns_classes:
-            display_custom = prompt("Display Custom records (probably not)?", type=click.BOOL, default=False)
-            print("\n   RECORDS")
-            print("-------------------")
-            if display_custom:
-                for record in records:
-                    print(record)
-            else:
-                for record in records:
-                    if "customrecord" not in record and "customlist" not in record:
+    use_record_wizard = prompt("Use Record Wizard?", type=click.BOOL, default=True)
+    if use_record_wizard:
+        needs_other_recordtypes = prompt("Will you be using record types other than customer?", type=click.BOOL, default=True)
+
+
+        if needs_other_recordtypes:
+
+            display_ns_classes = prompt("List available Netsuite Records?", type=click.BOOL, default=True)
+            print("")
+            print(" Getting Record Types... May take a minute...")
+            records = netsuite.get_netsuite_recordtypes()
+            if display_ns_classes:
+                display_custom = prompt("Display Custom records (probably not)?", type=click.BOOL, default=False)
+                print("\n   RECORDS")
+                print("-------------------")
+                if display_custom:
+                    for record in records:
                         print(record)
-
-        print("\n")
-        add_more_records = True
-        while add_more_records:
-            next_record = prompt("Which records do you need?", default='')
-            if next_record == '':
-                if prompt("Skip this step and use default (customer)?", type=click.BOOL, default=False):
-                    break
-            else:
-                if next_record not in records:
-                    print("That record is not available.")
-                elif next_record in ns_records_to_include:
-                    print("record already included.")
                 else:
-                     ns_records_to_include.append(next_record)
-                     print(f"Record Added: {next_record}")
-            add_more_records = prompt("Add another?", type=click.BOOL, default='yes', show_choices=True)
-
-
-    if len(ns_records_to_include) >> 0:
-        record_str = ''
-        index = 0
-        for record in ns_records_to_include:
-            if index == 0:
-                record_str += f'{record}'
-            else:
-                record_str += f',{record}'
+                    for record in records:
+                        if "customrecord" not in record and "customlist" not in record:
+                            print(record)
+
+            print("\n")
+            add_more_records = True
+            while add_more_records:
+                next_record = prompt("Which records do you need?", default='')
+                if next_record == '':
+                    if prompt("Skip this step and use default (customer)?", type=click.BOOL, default=False):
+                        break
+                else:
+                    if next_record not in records:
+                        print("That record is not available.")
+                    elif next_record in ns_records_to_include:
+                        print("record already included.")
+                    else:
+                         ns_records_to_include.append(next_record)
+                         print(f"Record Added: {next_record}")
+                add_more_records = prompt("Add another?", type=click.BOOL, default='yes', show_choices=True)
+
+
+        if len(ns_records_to_include) >> 0:
+            record_str = ''
+            index = 0
+            for record in ns_records_to_include:
+                print(len(ns_records_to_include))
+                if index == 0:
+                    print('index was 0')
+                    record_str += f'{record}'
+                    index += 1
+                else:
+                    record_str += f',{record}'
+        else:
+            record_str = 'customer'
     else:
-        record_str = 'customer'
-
+        record_str = prompt("Enter Record Types (comma separated)", default='customer')
+    print(f"Record STR: record_str")
     netsuite.generate_rest_client(record_types=record_str)
 
 
 @cli.command()
 @click.option('--credentials-file', '--f', type=click.File('r'), default=api_settings.CREDENTIALS_PATH,
               prompt="Path to Credentials File")
 @click.pass_context
```

### Comparing `netsuite_python-1.5.8/netsuite/settings.py` & `netsuite_python-1.5.9/netsuite/settings.py`

 * *Files identical despite different names*

### Comparing `netsuite_python-1.5.8/netsuite/storages/InMemoryStorage.py` & `netsuite_python-1.5.9/netsuite/storages/InMemoryStorage.py`

 * *Files identical despite different names*

### Comparing `netsuite_python-1.5.8/netsuite/storages/JSONStorage.py` & `netsuite_python-1.5.9/netsuite/storages/JSONStorage.py`

 * *Files identical despite different names*

### Comparing `netsuite_python-1.5.8/netsuite_python.egg-info/PKG-INFO` & `netsuite_python-1.5.9/netsuite_python.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: netsuite-python
-Version: 1.5.8
+Version: 1.5.9
 Summary: Python SDK for Netsuite API with Flask Integration
 Home-page: https://bitbucket.org/theapiguys/netsuite_python
 Author: Will @ TheAPIGuys
 Author-email: will@theapiguys.com
 License: UNKNOWN
 Platform: UNKNOWN
 Description-Content-Type: text/markdown
```

### Comparing `netsuite_python-1.5.8/netsuite_python.egg-info/SOURCES.txt` & `netsuite_python-1.5.9/netsuite_python.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `netsuite_python-1.5.8/setup.py` & `netsuite_python-1.5.9/setup.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from setuptools import setup, find_packages
 from pathlib import Path
 this_directory = Path(__file__).parent
 long_description = (this_directory / "README.md").read_text()
 
 setup(
     name='netsuite_python',
-    version='1.5.8',
+    version='1.5.9',
     description='Python SDK for Netsuite API with Flask Integration',
     long_description=long_description,
     long_description_content_type='text/markdown',
     url='https://bitbucket.org/theapiguys/netsuite_python',
     readme="README.md",
     author='Will @ TheAPIGuys',
     author_email='will@theapiguys.com',
```

