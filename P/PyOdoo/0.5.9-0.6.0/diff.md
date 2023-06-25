# Comparing `tmp/PyOdoo-0.5.9.tar.gz` & `tmp/PyOdoo-0.6.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "PyOdoo-0.5.9.tar", last modified: Wed May 17 21:33:39 2023, max compression
+gzip compressed data, was "PyOdoo-0.6.0.tar", last modified: Sun Jun 25 21:58:28 2023, max compression
```

## Comparing `PyOdoo-0.5.9.tar` & `PyOdoo-0.6.0.tar`

### file list

```diff
@@ -1,31 +1,35 @@
-drwxr-xr-x   0 muflone   (1000) users      (985)        0 2023-05-17 21:33:39.663660 PyOdoo-0.5.9/
--rw-r--r--   0 muflone   (1000) users      (985)      613 2021-05-09 18:22:23.000000 PyOdoo-0.5.9/LICENSE
--rw-r--r--   0 muflone   (1000) users      (985)     1762 2023-05-17 21:33:39.663660 PyOdoo-0.5.9/PKG-INFO
-drwxr-xr-x   0 muflone   (1000) users      (985)        0 2023-05-17 21:33:39.660327 PyOdoo-0.5.9/PyOdoo.egg-info/
--rw-r--r--   0 muflone   (1000) users      (985)     1762 2023-05-17 21:33:39.000000 PyOdoo-0.5.9/PyOdoo.egg-info/PKG-INFO
--rw-r--r--   0 muflone   (1000) users      (985)      552 2023-05-17 21:33:39.000000 PyOdoo-0.5.9/PyOdoo.egg-info/SOURCES.txt
--rw-r--r--   0 muflone   (1000) users      (985)        1 2023-05-17 21:33:39.000000 PyOdoo-0.5.9/PyOdoo.egg-info/dependency_links.txt
--rw-r--r--   0 muflone   (1000) users      (985)        7 2023-05-17 21:33:39.000000 PyOdoo-0.5.9/PyOdoo.egg-info/top_level.txt
--rw-r--r--   0 muflone   (1000) users      (985)     1014 2023-02-05 04:31:04.000000 PyOdoo-0.5.9/README.md
-drwxr-xr-x   0 muflone   (1000) users      (985)        0 2023-05-17 21:33:39.660327 PyOdoo-0.5.9/pyodoo/
--rw-r--r--   0 muflone   (1000) users      (985)     1306 2023-02-05 04:31:04.000000 PyOdoo-0.5.9/pyodoo/__init__.py
--rw-r--r--   0 muflone   (1000) users      (985)     1004 2023-02-05 04:31:04.000000 PyOdoo-0.5.9/pyodoo/active_status_choice.py
--rw-r--r--   0 muflone   (1000) users      (985)      956 2023-02-05 04:31:04.000000 PyOdoo-0.5.9/pyodoo/boolean_operator.py
--rw-r--r--   0 muflone   (1000) users      (985)     1365 2023-05-15 23:49:57.000000 PyOdoo-0.5.9/pyodoo/compare_type.py
--rw-r--r--   0 muflone   (1000) users      (985)     1227 2023-05-17 21:21:43.000000 PyOdoo-0.5.9/pyodoo/constants.py
--rw-r--r--   0 muflone   (1000) users      (985)     1502 2023-02-05 04:31:04.000000 PyOdoo-0.5.9/pyodoo/filter.py
--rw-r--r--   0 muflone   (1000) users      (985)     1008 2023-02-05 04:31:04.000000 PyOdoo-0.5.9/pyodoo/message_subtype.py
-drwxr-xr-x   0 muflone   (1000) users      (985)        0 2023-05-17 21:33:39.663660 PyOdoo-0.5.9/pyodoo/samples/
--rw-r--r--   0 muflone   (1000) users      (985)        0 2022-09-23 22:59:11.000000 PyOdoo-0.5.9/pyodoo/samples/__init__.py
--rw-r--r--   0 muflone   (1000) users      (985)     1345 2023-02-05 04:31:04.000000 PyOdoo-0.5.9/pyodoo/samples/awaitable.py
--rw-r--r--   0 muflone   (1000) users      (985)     5169 2023-03-19 10:57:46.000000 PyOdoo-0.5.9/pyodoo/samples/contacts.py
--rw-r--r--   0 muflone   (1000) users      (985)     3666 2023-02-05 16:20:33.000000 PyOdoo-0.5.9/pyodoo/samples/contacts_async.py
-drwxr-xr-x   0 muflone   (1000) users      (985)        0 2023-05-17 21:33:39.663660 PyOdoo-0.5.9/pyodoo/v12/
--rw-r--r--   0 muflone   (1000) users      (985)      986 2023-02-05 04:31:04.000000 PyOdoo-0.5.9/pyodoo/v12/__init__.py
--rw-r--r--   0 muflone   (1000) users      (985)    11089 2023-02-05 18:02:47.000000 PyOdoo-0.5.9/pyodoo/v12/api.py
--rw-r--r--   0 muflone   (1000) users      (985)    31145 2023-05-17 21:27:30.000000 PyOdoo-0.5.9/pyodoo/v12/model.py
--rw-r--r--   0 muflone   (1000) users      (985)       90 2022-01-06 22:44:31.000000 PyOdoo-0.5.9/pyproject.toml
--rw-r--r--   0 muflone   (1000) users      (985)      883 2023-05-17 21:33:39.663660 PyOdoo-0.5.9/setup.cfg
-drwxr-xr-x   0 muflone   (1000) users      (985)        0 2023-05-17 21:33:39.663660 PyOdoo-0.5.9/tests/
--rw-r--r--   0 muflone   (1000) users      (985)    16600 2023-05-15 23:49:57.000000 PyOdoo-0.5.9/tests/test_compare_types.py
--rw-r--r--   0 muflone   (1000) users      (985)    33179 2023-05-17 21:28:14.000000 PyOdoo-0.5.9/tests/test_contacts.py
+drwxr-xr-x   0 muflone   (1000) users      (985)        0 2023-06-25 21:58:28.008923 PyOdoo-0.6.0/
+-rw-r--r--   0 muflone   (1000) users      (985)      613 2021-05-09 18:22:23.000000 PyOdoo-0.6.0/LICENSE
+-rw-r--r--   0 muflone   (1000) users      (985)     1863 2023-06-25 21:58:28.012256 PyOdoo-0.6.0/PKG-INFO
+drwxr-xr-x   0 muflone   (1000) users      (985)        0 2023-06-25 21:58:28.005590 PyOdoo-0.6.0/PyOdoo.egg-info/
+-rw-r--r--   0 muflone   (1000) users      (985)     1863 2023-06-25 21:58:27.000000 PyOdoo-0.6.0/PyOdoo.egg-info/PKG-INFO
+-rw-r--r--   0 muflone   (1000) users      (985)      675 2023-06-25 21:58:28.000000 PyOdoo-0.6.0/PyOdoo.egg-info/SOURCES.txt
+-rw-r--r--   0 muflone   (1000) users      (985)        1 2023-06-25 21:58:27.000000 PyOdoo-0.6.0/PyOdoo.egg-info/dependency_links.txt
+-rw-r--r--   0 muflone   (1000) users      (985)       12 2023-06-25 21:58:27.000000 PyOdoo-0.6.0/PyOdoo.egg-info/requires.txt
+-rw-r--r--   0 muflone   (1000) users      (985)        7 2023-06-25 21:58:27.000000 PyOdoo-0.6.0/PyOdoo.egg-info/top_level.txt
+-rw-r--r--   0 muflone   (1000) users      (985)     1115 2023-06-25 21:47:00.000000 PyOdoo-0.6.0/README.md
+drwxr-xr-x   0 muflone   (1000) users      (985)        0 2023-06-25 21:58:28.008923 PyOdoo-0.6.0/pyodoo/
+-rw-r--r--   0 muflone   (1000) users      (985)     1306 2023-02-05 04:31:04.000000 PyOdoo-0.6.0/pyodoo/__init__.py
+-rw-r--r--   0 muflone   (1000) users      (985)     1004 2023-02-05 04:31:04.000000 PyOdoo-0.6.0/pyodoo/active_status_choice.py
+-rw-r--r--   0 muflone   (1000) users      (985)      956 2023-02-05 04:31:04.000000 PyOdoo-0.6.0/pyodoo/boolean_operator.py
+-rw-r--r--   0 muflone   (1000) users      (985)     1365 2023-05-15 23:49:57.000000 PyOdoo-0.6.0/pyodoo/compare_type.py
+-rw-r--r--   0 muflone   (1000) users      (985)     1227 2023-06-20 00:48:59.000000 PyOdoo-0.6.0/pyodoo/constants.py
+-rw-r--r--   0 muflone   (1000) users      (985)     1502 2023-02-05 04:31:04.000000 PyOdoo-0.6.0/pyodoo/filter.py
+-rw-r--r--   0 muflone   (1000) users      (985)     1008 2023-02-05 04:31:04.000000 PyOdoo-0.6.0/pyodoo/message_subtype.py
+drwxr-xr-x   0 muflone   (1000) users      (985)        0 2023-06-25 21:58:28.008923 PyOdoo-0.6.0/pyodoo/samples/
+-rw-r--r--   0 muflone   (1000) users      (985)        0 2022-09-23 22:59:11.000000 PyOdoo-0.6.0/pyodoo/samples/__init__.py
+-rw-r--r--   0 muflone   (1000) users      (985)     1345 2023-02-05 04:31:04.000000 PyOdoo-0.6.0/pyodoo/samples/awaitable.py
+-rw-r--r--   0 muflone   (1000) users      (985)     5169 2023-03-19 10:57:46.000000 PyOdoo-0.6.0/pyodoo/samples/contacts.py
+-rw-r--r--   0 muflone   (1000) users      (985)     3666 2023-02-05 16:20:33.000000 PyOdoo-0.6.0/pyodoo/samples/contacts_async.py
+-rw-r--r--   0 muflone   (1000) users      (985)     2477 2023-06-25 19:15:22.000000 PyOdoo-0.6.0/pyodoo/samples/sql_excel_query.py
+drwxr-xr-x   0 muflone   (1000) users      (985)        0 2023-06-25 21:58:28.008923 PyOdoo-0.6.0/pyodoo/v12/
+-rw-r--r--   0 muflone   (1000) users      (985)     1066 2023-06-20 23:32:16.000000 PyOdoo-0.6.0/pyodoo/v12/__init__.py
+-rw-r--r--   0 muflone   (1000) users      (985)    11089 2023-02-05 18:02:47.000000 PyOdoo-0.6.0/pyodoo/v12/api.py
+-rw-r--r--   0 muflone   (1000) users      (985)    31424 2023-06-02 23:09:47.000000 PyOdoo-0.6.0/pyodoo/v12/model.py
+-rw-r--r--   0 muflone   (1000) users      (985)    10269 2023-06-25 18:56:12.000000 PyOdoo-0.6.0/pyodoo/v12/sql_excel_query.py
+-rw-r--r--   0 muflone   (1000) users      (985)       90 2022-01-06 22:44:31.000000 PyOdoo-0.6.0/pyproject.toml
+-rw-r--r--   0 muflone   (1000) users      (985)      916 2023-06-25 21:58:28.012256 PyOdoo-0.6.0/setup.cfg
+drwxr-xr-x   0 muflone   (1000) users      (985)        0 2023-06-25 21:58:28.008923 PyOdoo-0.6.0/tests/
+-rw-r--r--   0 muflone   (1000) users      (985)    16600 2023-05-15 23:49:57.000000 PyOdoo-0.6.0/tests/test_compare_types.py
+-rw-r--r--   0 muflone   (1000) users      (985)    34030 2023-06-02 23:11:58.000000 PyOdoo-0.6.0/tests/test_contacts.py
+-rw-r--r--   0 muflone   (1000) users      (985)     8073 2023-06-25 19:16:26.000000 PyOdoo-0.6.0/tests/test_sql_excel_query.py
```

### Comparing `PyOdoo-0.5.9/LICENSE` & `PyOdoo-0.6.0/LICENSE`

 * *Files identical despite different names*

### Comparing `PyOdoo-0.5.9/PKG-INFO` & `PyOdoo-0.6.0/PKG-INFO`

 * *Files 20% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: PyOdoo
-Version: 0.5.9
+Version: 0.6.0
 Summary: API for Odoo
 Home-page: http://www.muflone.com/pyodoo/
 Author: Fabio Castelli
 Author-email: muflone@muflone.com
 License: GPLv3+
 Classifier: Development Status :: 1 - Planning
 Classifier: Intended Audience :: Developers
@@ -40,11 +40,13 @@
 PyOdoo is an attempt to build a common API to interact with any
 [**Odoo**](https://www.odoo.com/) server in order to operate using
 its XML RPC API.
 
 # System Requirements
 
 * Python 3.x
+* xlrd 2.0.x (https://pypi.org/project/xlrd/)
+* requests 2.31.x (https://pypi.org/project/requests/)
 
 # Usage
 
 Please see the **samples** and the **tests** folders for some usage examples.
```

### Comparing `PyOdoo-0.5.9/PyOdoo.egg-info/PKG-INFO` & `PyOdoo-0.6.0/PyOdoo.egg-info/PKG-INFO`

 * *Files 20% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: PyOdoo
-Version: 0.5.9
+Version: 0.6.0
 Summary: API for Odoo
 Home-page: http://www.muflone.com/pyodoo/
 Author: Fabio Castelli
 Author-email: muflone@muflone.com
 License: GPLv3+
 Classifier: Development Status :: 1 - Planning
 Classifier: Intended Audience :: Developers
@@ -40,11 +40,13 @@
 PyOdoo is an attempt to build a common API to interact with any
 [**Odoo**](https://www.odoo.com/) server in order to operate using
 its XML RPC API.
 
 # System Requirements
 
 * Python 3.x
+* xlrd 2.0.x (https://pypi.org/project/xlrd/)
+* requests 2.31.x (https://pypi.org/project/requests/)
 
 # Usage
 
 Please see the **samples** and the **tests** folders for some usage examples.
```

### Comparing `PyOdoo-0.5.9/PyOdoo.egg-info/SOURCES.txt` & `PyOdoo-0.6.0/PyOdoo.egg-info/SOURCES.txt`

 * *Files 22% similar despite different names*

```diff
@@ -1,24 +1,28 @@
 LICENSE
 README.md
 pyproject.toml
 setup.cfg
 PyOdoo.egg-info/PKG-INFO
 PyOdoo.egg-info/SOURCES.txt
 PyOdoo.egg-info/dependency_links.txt
+PyOdoo.egg-info/requires.txt
 PyOdoo.egg-info/top_level.txt
 pyodoo/__init__.py
 pyodoo/active_status_choice.py
 pyodoo/boolean_operator.py
 pyodoo/compare_type.py
 pyodoo/constants.py
 pyodoo/filter.py
 pyodoo/message_subtype.py
 pyodoo/samples/__init__.py
 pyodoo/samples/awaitable.py
 pyodoo/samples/contacts.py
 pyodoo/samples/contacts_async.py
+pyodoo/samples/sql_excel_query.py
 pyodoo/v12/__init__.py
 pyodoo/v12/api.py
 pyodoo/v12/model.py
+pyodoo/v12/sql_excel_query.py
 tests/test_compare_types.py
-tests/test_contacts.py
+tests/test_contacts.py
+tests/test_sql_excel_query.py
```

### Comparing `PyOdoo-0.5.9/README.md` & `PyOdoo-0.6.0/README.md`

 * *Files 25% similar despite different names*

```diff
@@ -20,11 +20,13 @@
 PyOdoo is an attempt to build a common API to interact with any
 [**Odoo**](https://www.odoo.com/) server in order to operate using
 its XML RPC API.
 
 # System Requirements
 
 * Python 3.x
+* xlrd 2.0.x (https://pypi.org/project/xlrd/)
+* requests 2.31.x (https://pypi.org/project/requests/)
 
 # Usage
 
 Please see the **samples** and the **tests** folders for some usage examples.
```

### Comparing `PyOdoo-0.5.9/pyodoo/__init__.py` & `PyOdoo-0.6.0/pyodoo/__init__.py`

 * *Files identical despite different names*

### Comparing `PyOdoo-0.5.9/pyodoo/active_status_choice.py` & `PyOdoo-0.6.0/pyodoo/active_status_choice.py`

 * *Files identical despite different names*

### Comparing `PyOdoo-0.5.9/pyodoo/boolean_operator.py` & `PyOdoo-0.6.0/pyodoo/boolean_operator.py`

 * *Files identical despite different names*

### Comparing `PyOdoo-0.5.9/pyodoo/compare_type.py` & `PyOdoo-0.6.0/pyodoo/compare_type.py`

 * *Files identical despite different names*

### Comparing `PyOdoo-0.5.9/pyodoo/constants.py` & `PyOdoo-0.6.0/pyodoo/constants.py`

 * *Files 8% similar despite different names*

```diff
@@ -15,15 +15,15 @@
 #  GNU General Public License for more details.
 #
 #  You should have received a copy of the GNU General Public License
 #  along with this program.  If not, see <https://www.gnu.org/licenses/>.
 ##
 
 APP_NAME = 'PyOdoo'
-APP_VERSION = '0.5.9'
+APP_VERSION = '0.6.0'
 APP_DESCRIPTION = 'API for Odoo'
 APP_DOMAIN = 'pyodoo'
 APP_ID = f'{APP_DOMAIN}.muflone.com'
 APP_AUTHOR = 'Fabio Castelli'
 APP_AUTHOR_EMAIL = 'muflone@muflone.com'
 APP_COPYRIGHT = f'Copyright 2021-2023 {APP_AUTHOR}'
 URL_AUTHOR = 'http://www.muflone.com/'
```

### Comparing `PyOdoo-0.5.9/pyodoo/filter.py` & `PyOdoo-0.6.0/pyodoo/filter.py`

 * *Files identical despite different names*

### Comparing `PyOdoo-0.5.9/pyodoo/message_subtype.py` & `PyOdoo-0.6.0/pyodoo/message_subtype.py`

 * *Files identical despite different names*

### Comparing `PyOdoo-0.5.9/pyodoo/samples/awaitable.py` & `PyOdoo-0.6.0/pyodoo/samples/awaitable.py`

 * *Files identical despite different names*

### Comparing `PyOdoo-0.5.9/pyodoo/samples/contacts.py` & `PyOdoo-0.6.0/pyodoo/samples/contacts.py`

 * *Files identical despite different names*

### Comparing `PyOdoo-0.5.9/pyodoo/samples/contacts_async.py` & `PyOdoo-0.6.0/pyodoo/samples/contacts_async.py`

 * *Files identical despite different names*

### Comparing `PyOdoo-0.5.9/pyodoo/v12/__init__.py` & `PyOdoo-0.6.0/pyodoo/v12/__init__.py`

 * *Files 6% similar despite different names*

```diff
@@ -16,7 +16,8 @@
 #
 #  You should have received a copy of the GNU General Public License
 #  along with this program.  If not, see <https://www.gnu.org/licenses/>.
 ##
 
 from .api import Api                                               # noqa: F401
 from .model import Model                                           # noqa: F401
+from .sql_excel_query import SqlExcelQuery                         # noqa: F401
```

### Comparing `PyOdoo-0.5.9/pyodoo/v12/api.py` & `PyOdoo-0.6.0/pyodoo/v12/api.py`

 * *Files identical despite different names*

### Comparing `PyOdoo-0.5.9/pyodoo/v12/model.py` & `PyOdoo-0.6.0/pyodoo/v12/model.py`

 * *Files 1% similar despite different names*

```diff
@@ -88,28 +88,34 @@
 
         :return: The user ID for the authenticated user
         """
         return self.api.authenticate()
 
     def get_model(self,
                   model_name: str,
-                  authenticate: bool = False) -> 'Model':
+                  authenticate: bool = False,
+                  use_existing_uid: bool = False) -> 'Model':
         """
         Get a Model object for another model name
         :param model_name: Model name
         :param authenticate: Automatically authenticate user
+        :param use_existing_uid: Use the existing UID if not authenticated
         :return: Model object
         """
-        return Model(model_name=model_name,
-                     endpoint=self.api.endpoint,
-                     database=self.api.database,
-                     username=self.api.username,
-                     password=self.api.password,
-                     language=self.api.language,
-                     authenticate=authenticate)
+        model = Model(model_name=model_name,
+                      endpoint=self.api.endpoint,
+                      database=self.api.database,
+                      username=self.api.username,
+                      password=self.api.password,
+                      language=self.api.language,
+                      authenticate=authenticate)
+        if not authenticate and use_existing_uid:
+            # Use the existing UID
+            model.api.uid = self.api.uid
+        return model
 
     def get_model_data_reference(self,
                                  module_name: str,
                                  value: str):
         """
         Get a reference row from ir.module.data
```

### Comparing `PyOdoo-0.5.9/setup.cfg` & `PyOdoo-0.6.0/setup.cfg`

 * *Files 22% similar despite different names*

```diff
@@ -21,14 +21,16 @@
 	Topic :: Software Development :: Libraries :: Python Modules
 
 [options]
 packages = 
 	pyodoo
 	pyodoo.v12
 include_package_data = False
+install_requires = 
+	xlrd==2.0.1
 
 [options.package_data]
 pyodoo = samples/*
 
 [egg_info]
 tag_build = 
 tag_date = 0
```

### Comparing `PyOdoo-0.5.9/tests/test_compare_types.py` & `PyOdoo-0.6.0/tests/test_compare_types.py`

 * *Files identical despite different names*

### Comparing `PyOdoo-0.5.9/tests/test_contacts.py` & `PyOdoo-0.6.0/tests/test_contacts.py`

 * *Files 2% similar despite different names*

```diff
@@ -780,18 +780,39 @@
         self.assertIsNotNone(results)
         # Check if we have 2 fields
         field_name = results['name']
         self.assertEqual(len(field_name), 2)
         self.assertIn('string', field_name)
         self.assertIn('type', field_name)
 
-    def test_41_get_model(self) -> None:
+    def test_41_get_model_authenticate(self) -> None:
         """
         Get a new Model object
         """
         model_name = 'res.users'
-        results = self.model.get_model(model_name=model_name,
-                                       authenticate=False)
+        model = self.model.get_model(model_name=model_name,
+                                     authenticate=True,
+                                     use_existing_uid=False)
+        results = model.count(filters=[])
         # Check if we have results
+        self.assertIsNotNone(model)
+        self.assertIsInstance(model, Model)
+        self.assertEqual(model.model_name, model_name)
         self.assertIsNotNone(results)
-        self.assertIsInstance(results, Model)
-        self.assertEqual(results.model_name, model_name)
+        self.assertGreater(results, 0)
+
+    def test_42_get_model_no_authenticate(self) -> None:
+        """
+        Get a new Model object using the existing UID
+        """
+        self.model.authenticate()
+        model_name = 'res.users'
+        model = self.model.get_model(model_name=model_name,
+                                     authenticate=False,
+                                     use_existing_uid=True)
+        results = model.count(filters=[])
+        # Check if we have results
+        self.assertIsNotNone(model)
+        self.assertIsInstance(model, Model)
+        self.assertEqual(model.model_name, model_name)
+        self.assertIsNotNone(results)
+        self.assertGreater(results, 0)
```

