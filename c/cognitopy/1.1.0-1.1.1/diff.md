# Comparing `tmp/cognitopy-1.1.0.tar.gz` & `tmp/cognitopy-1.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cognitopy-1.1.0.tar", last modified: Sat Jun 24 19:51:17 2023, max compression
+gzip compressed data, was "cognitopy-1.1.1.tar", last modified: Mon Jun 26 18:12:01 2023, max compression
```

## Comparing `cognitopy-1.1.0.tar` & `cognitopy-1.1.1.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-24 19:51:17.768737 cognitopy-1.1.0/
--rw-r--r--   0 runner    (1001) docker     (123)     1073 2023-06-24 19:51:06.000000 cognitopy-1.1.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     8972 2023-06-24 19:51:17.768737 cognitopy-1.1.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     8437 2023-06-24 19:51:06.000000 cognitopy-1.1.0/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      640 2023-06-24 19:51:06.000000 cognitopy-1.1.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-24 19:51:17.768737 cognitopy-1.1.0/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-24 19:51:17.768737 cognitopy-1.1.0/src/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-24 19:51:06.000000 cognitopy-1.1.0/src/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-24 19:51:17.768737 cognitopy-1.1.0/src/cognitopy/
--rw-r--r--   0 runner    (1001) docker     (123)       48 2023-06-24 19:51:06.000000 cognitopy-1.1.0/src/cognitopy/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    24001 2023-06-24 19:51:06.000000 cognitopy-1.1.0/src/cognitopy/cognitopy.py
--rw-r--r--   0 runner    (1001) docker     (123)      520 2023-06-24 19:51:06.000000 cognitopy-1.1.0/src/cognitopy/enums.py
--rw-r--r--   0 runner    (1001) docker     (123)      204 2023-06-24 19:51:06.000000 cognitopy-1.1.0/src/cognitopy/exceptions.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-24 19:51:17.768737 cognitopy-1.1.0/src/cognitopy.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     8972 2023-06-24 19:51:17.000000 cognitopy-1.1.0/src/cognitopy.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      300 2023-06-24 19:51:17.000000 cognitopy-1.1.0/src/cognitopy.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-24 19:51:17.000000 cognitopy-1.1.0/src/cognitopy.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       19 2023-06-24 19:51:17.000000 cognitopy-1.1.0/src/cognitopy.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 18:12:01.859013 cognitopy-1.1.1/
+-rw-r--r--   0 runner    (1001) docker     (123)     1073 2023-06-26 18:11:48.000000 cognitopy-1.1.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     8997 2023-06-26 18:12:01.859013 cognitopy-1.1.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     8462 2023-06-26 18:11:48.000000 cognitopy-1.1.1/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      640 2023-06-26 18:11:48.000000 cognitopy-1.1.1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-26 18:12:01.859013 cognitopy-1.1.1/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 18:12:01.855013 cognitopy-1.1.1/src/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-26 18:11:48.000000 cognitopy-1.1.1/src/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 18:12:01.859013 cognitopy-1.1.1/src/cognitopy/
+-rw-r--r--   0 runner    (1001) docker     (123)       48 2023-06-26 18:11:48.000000 cognitopy-1.1.1/src/cognitopy/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    24046 2023-06-26 18:11:48.000000 cognitopy-1.1.1/src/cognitopy/cognitopy.py
+-rw-r--r--   0 runner    (1001) docker     (123)      520 2023-06-26 18:11:48.000000 cognitopy-1.1.1/src/cognitopy/enums.py
+-rw-r--r--   0 runner    (1001) docker     (123)      204 2023-06-26 18:11:48.000000 cognitopy-1.1.1/src/cognitopy/exceptions.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 18:12:01.859013 cognitopy-1.1.1/src/cognitopy.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     8997 2023-06-26 18:12:01.000000 cognitopy-1.1.1/src/cognitopy.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      300 2023-06-26 18:12:01.000000 cognitopy-1.1.1/src/cognitopy.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-26 18:12:01.000000 cognitopy-1.1.1/src/cognitopy.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       19 2023-06-26 18:12:01.000000 cognitopy-1.1.1/src/cognitopy.egg-info/top_level.txt
```

### Comparing `cognitopy-1.1.0/LICENSE` & `cognitopy-1.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `cognitopy-1.1.0/PKG-INFO` & `cognitopy-1.1.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cognitopy
-Version: 1.1.0
+Version: 1.1.1
 Summary: Python package to use aws cognito in a simple way
 Author-email: Daniel Muñoz Gonzalez <dani16595@gmail.com>
 Project-URL: Homepage, https://github.com/DaniMG95/cognitopy
 Project-URL: Bug Tracker, https://github.com/DaniMG95/cognitopy/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
@@ -61,15 +61,16 @@
                client_secret=COGNITO_APP_CLIENTE_SECRET) as cognito:
     cognito.register(username="XXXXX@mail.to", password="XXXXXXX8", user_attributes={})
 ```
 
 ### Register a new user
 It will register a user in our cognito service and send us a confirmation message.
 ```python
-cognito.register(username='XXXXX@mail.to', password='XXXXXXX8', user_attributes={})
+id_user = cognito.register(username='XXXXX@mail.to', password='XXXXXXX8', user_attributes={})
+print(id_user)
 ```
 
 ### Confirm a new user
 It is responsible for confirming the user from the number received by mail.
 ```python
 cognito.confirm_register(username='XXXXX@mail.to', confirmation_code='820850')
 ```
```

### Comparing `cognitopy-1.1.0/README.md` & `cognitopy-1.1.1/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -47,15 +47,16 @@
                client_secret=COGNITO_APP_CLIENTE_SECRET) as cognito:
     cognito.register(username="XXXXX@mail.to", password="XXXXXXX8", user_attributes={})
 ```
 
 ### Register a new user
 It will register a user in our cognito service and send us a confirmation message.
 ```python
-cognito.register(username='XXXXX@mail.to', password='XXXXXXX8', user_attributes={})
+id_user = cognito.register(username='XXXXX@mail.to', password='XXXXXXX8', user_attributes={})
+print(id_user)
 ```
 
 ### Confirm a new user
 It is responsible for confirming the user from the number received by mail.
 ```python
 cognito.confirm_register(username='XXXXX@mail.to', confirmation_code='820850')
 ```
```

### Comparing `cognitopy-1.1.0/pyproject.toml` & `cognitopy-1.1.1/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 build-backend = "setuptools.build_meta"
 
 [tool.black]
 line-length = 120
 
 [project]
 name = "cognitopy"
-version = "1.1.0"
+version = "1.1.1"
 authors = [
   { name="Daniel Muñoz Gonzalez", email="dani16595@gmail.com" },
 ]
 description = "Python package to use aws cognito in a simple way"
 readme = "README.md"
 requires-python = ">=3.7"
 classifiers = [
```

### Comparing `cognitopy-1.1.0/src/cognitopy/cognitopy.py` & `cognitopy-1.1.1/src/cognitopy/cognitopy.py`

 * *Files 1% similar despite different names*

```diff
@@ -183,30 +183,31 @@
                 f"{response['ChallengeName']}, the session is {response['Session']}."
             )
         return {
             self.__ACCESS_TOKEN_KEY: response[self.__AUTHENTICATION_RESULT][self.__ACCESS_TOKEN],
             self.__REFRESH_TOKEN_KEY: response[self.__AUTHENTICATION_RESULT][self.__REFRESH_TOKEN],
         }
 
-    def register(self, username: str, user_attributes: dict, password: str) -> None:
+    def register(self, username: str, user_attributes: dict, password: str) -> str:
         if not isinstance(username, str) or not isinstance(user_attributes, dict) or not isinstance(password, str):
             raise ValueError("The username, password should be strings and user_attributes should be a dict.")
         cognito_attributes = self.__dict_to_cognito(user_attributes)
         arg_secret_hash = {}
         self.__check_need_secret_hash(username=username, data=arg_secret_hash, key_secret_hash=self.__SECRET_HASH_ARG)
         try:
-            self.__client.sign_up(
+            response = self.__client.sign_up(
                 ClientId=self.__client_id,
                 Username=username,
                 Password=password,
                 UserAttributes=cognito_attributes,
                 **arg_secret_hash,
             )
         except ClientError as e:
             raise ExceptionAuthCognito(e.response[self.__ERROR][self.__MESSAGE])
+        return response["UserSub"]
 
     def resend_confirmation_code(self, username: str) -> None:
         if not isinstance(username, str):
             raise ValueError("The username should be a string.")
         arg_secret_hash = {}
         self.__check_need_secret_hash(username=username, data=arg_secret_hash, key_secret_hash=self.__SECRET_HASH_ARG)
         try:
```

### Comparing `cognitopy-1.1.0/src/cognitopy/enums.py` & `cognitopy-1.1.1/src/cognitopy/enums.py`

 * *Files identical despite different names*

### Comparing `cognitopy-1.1.0/src/cognitopy.egg-info/PKG-INFO` & `cognitopy-1.1.1/src/cognitopy.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cognitopy
-Version: 1.1.0
+Version: 1.1.1
 Summary: Python package to use aws cognito in a simple way
 Author-email: Daniel Muñoz Gonzalez <dani16595@gmail.com>
 Project-URL: Homepage, https://github.com/DaniMG95/cognitopy
 Project-URL: Bug Tracker, https://github.com/DaniMG95/cognitopy/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
@@ -61,15 +61,16 @@
                client_secret=COGNITO_APP_CLIENTE_SECRET) as cognito:
     cognito.register(username="XXXXX@mail.to", password="XXXXXXX8", user_attributes={})
 ```
 
 ### Register a new user
 It will register a user in our cognito service and send us a confirmation message.
 ```python
-cognito.register(username='XXXXX@mail.to', password='XXXXXXX8', user_attributes={})
+id_user = cognito.register(username='XXXXX@mail.to', password='XXXXXXX8', user_attributes={})
+print(id_user)
 ```
 
 ### Confirm a new user
 It is responsible for confirming the user from the number received by mail.
 ```python
 cognito.confirm_register(username='XXXXX@mail.to', confirmation_code='820850')
 ```
```

