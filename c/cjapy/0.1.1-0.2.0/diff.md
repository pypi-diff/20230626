# Comparing `tmp/cjapy-0.1.1.tar.gz` & `tmp/cjapy-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cjapy-0.1.1.tar", last modified: Wed Jan 11 19:58:06 2023, max compression
+gzip compressed data, was "cjapy-0.2.0.tar", last modified: Mon Jun 26 14:07:28 2023, max compression
```

## Comparing `cjapy-0.1.1.tar` & `cjapy-0.2.0.tar`

### file list

```diff
@@ -1,23 +1,35 @@
-drwxrwxrwx   0        0        0        0 2023-01-11 19:58:06.694197 cjapy-0.1.1/
--rw-rw-rw-   0        0        0    10337 2021-10-20 19:50:41.000000 cjapy-0.1.1/LICENSE
--rw-rw-rw-   0        0        0     3383 2023-01-11 19:58:06.693199 cjapy-0.1.1/PKG-INFO
--rw-rw-rw-   0        0        0     2469 2021-11-08 18:46:39.000000 cjapy-0.1.1/README.md
-drwxrwxrwx   0        0        0        0 2023-01-11 19:58:06.677242 cjapy-0.1.1/cjapy/
--rw-rw-rw-   0        0        0      107 2021-10-20 19:50:41.000000 cjapy-0.1.1/cjapy/__init__.py
--rw-rw-rw-   0        0        0       23 2023-01-11 19:57:16.000000 cjapy-0.1.1/cjapy/__version__.py
--rw-rw-rw-   0        0        0   109066 2023-01-11 19:05:51.000000 cjapy-0.1.1/cjapy/cjapy.py
--rw-rw-rw-   0        0        0      459 2021-10-20 19:50:41.000000 cjapy-0.1.1/cjapy/config.py
--rw-rw-rw-   0        0        0     6254 2021-10-20 19:50:41.000000 cjapy-0.1.1/cjapy/configs.py
--rw-rw-rw-   0        0        0    11796 2021-11-08 18:46:39.000000 cjapy-0.1.1/cjapy/connector.py
--rw-rw-rw-   0        0        0    12007 2021-11-08 18:46:39.000000 cjapy-0.1.1/cjapy/projects.py
--rw-rw-rw-   0        0        0    16716 2022-07-10 12:50:38.000000 cjapy-0.1.1/cjapy/requestCreator.py
--rw-rw-rw-   0        0        0     2366 2021-10-20 19:50:41.000000 cjapy-0.1.1/cjapy/token_provider.py
--rw-rw-rw-   0        0        0     9362 2022-12-01 11:30:08.000000 cjapy-0.1.1/cjapy/workspace.py
-drwxrwxrwx   0        0        0        0 2023-01-11 19:58:06.690214 cjapy-0.1.1/cjapy.egg-info/
--rw-rw-rw-   0        0        0     3383 2023-01-11 19:58:06.000000 cjapy-0.1.1/cjapy.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      361 2023-01-11 19:58:06.000000 cjapy-0.1.1/cjapy.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-01-11 19:58:06.000000 cjapy-0.1.1/cjapy.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       60 2023-01-11 19:58:06.000000 cjapy-0.1.1/cjapy.egg-info/requires.txt
--rw-rw-rw-   0        0        0        6 2023-01-11 19:58:06.000000 cjapy-0.1.1/cjapy.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-01-11 19:58:06.695195 cjapy-0.1.1/setup.cfg
--rw-rw-rw-   0        0        0     1871 2021-10-20 19:50:41.000000 cjapy-0.1.1/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-26 14:07:28.419361 cjapy-0.2.0/
+-rw-rw-rw-   0        0        0    10337 2021-10-20 19:50:41.000000 cjapy-0.2.0/LICENSE
+-rw-rw-rw-   0        0        0     3565 2023-06-26 14:07:28.416364 cjapy-0.2.0/PKG-INFO
+-rw-rw-rw-   0        0        0     2469 2021-11-08 18:46:39.000000 cjapy-0.2.0/README.md
+drwxrwxrwx   0        0        0        0 2023-06-26 14:07:28.148988 cjapy-0.2.0/cjapy/
+-rw-rw-rw-   0        0        0      107 2021-10-20 19:50:41.000000 cjapy-0.2.0/cjapy/__init__.py
+-rw-rw-rw-   0        0        0       23 2023-06-26 06:51:12.000000 cjapy-0.2.0/cjapy/__version__.py
+-rw-rw-rw-   0        0        0   109066 2023-05-11 12:56:12.000000 cjapy-0.2.0/cjapy/cjapy.py
+-rw-rw-rw-   0        0        0      566 2023-06-26 06:55:22.000000 cjapy-0.2.0/cjapy/config.py
+-rw-rw-rw-   0        0        0     7666 2023-06-26 06:48:55.000000 cjapy-0.2.0/cjapy/configs.py
+-rw-rw-rw-   0        0        0    12662 2023-06-26 09:12:19.000000 cjapy-0.2.0/cjapy/connector.py
+-rw-rw-rw-   0        0        0    12007 2021-11-08 18:46:39.000000 cjapy-0.2.0/cjapy/projects.py
+-rw-rw-rw-   0        0        0    16716 2023-05-11 12:56:12.000000 cjapy-0.2.0/cjapy/requestCreator.py
+-rw-rw-rw-   0        0        0     3463 2023-06-26 09:22:08.000000 cjapy-0.2.0/cjapy/token_provider.py
+-rw-rw-rw-   0        0        0     9362 2023-05-11 12:56:12.000000 cjapy-0.2.0/cjapy/workspace.py
+drwxrwxrwx   0        0        0        0 2023-06-26 14:07:28.213750 cjapy-0.2.0/cjapy.egg-info/
+-rw-rw-rw-   0        0        0     3565 2023-06-26 14:07:27.000000 cjapy-0.2.0/cjapy.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      576 2023-06-26 14:07:27.000000 cjapy-0.2.0/cjapy.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-26 14:07:27.000000 cjapy-0.2.0/cjapy.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       79 2023-06-26 14:07:27.000000 cjapy-0.2.0/cjapy.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        6 2023-06-26 14:07:27.000000 cjapy-0.2.0/cjapy.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-06-26 14:07:28.410864 cjapy-0.2.0/docs/
+-rw-rw-rw-   0        0        0     1805 2021-10-20 19:50:41.000000 cjapy-0.2.0/docs/authenticating_without_config_json.md
+-rw-rw-rw-   0        0        0    27971 2023-05-11 12:56:12.000000 cjapy-0.2.0/docs/cja.md
+-rw-rw-rw-   0        0        0     3664 2023-06-26 06:49:51.000000 cjapy-0.2.0/docs/getting_started.md
+-rw-rw-rw-   0        0        0     3934 2021-10-20 19:50:41.000000 cjapy-0.2.0/docs/logging.md
+-rw-rw-rw-   0        0        0     3335 2021-10-20 19:50:41.000000 cjapy-0.2.0/docs/main.md
+-rw-rw-rw-   0        0        0     8595 2021-11-08 18:46:39.000000 cjapy-0.2.0/docs/projects.md
+-rw-rw-rw-   0        0        0     1214 2023-06-26 14:06:41.000000 cjapy-0.2.0/docs/releases.md
+-rw-rw-rw-   0        0        0     6126 2021-11-08 18:46:39.000000 cjapy-0.2.0/docs/requestCreator.md
+-rw-rw-rw-   0        0        0     3348 2021-10-20 19:50:41.000000 cjapy-0.2.0/docs/workspace.md
+-rw-rw-rw-   0        0        0     1364 2023-06-26 13:49:26.000000 cjapy-0.2.0/pyproject.toml
+-rw-rw-rw-   0        0        0      100 2021-10-20 19:50:41.000000 cjapy-0.2.0/requirements.txt
+-rw-rw-rw-   0        0        0       42 2023-06-26 14:07:28.427339 cjapy-0.2.0/setup.cfg
+-rw-rw-rw-   0        0        0     1871 2021-10-20 19:50:41.000000 cjapy-0.2.0/setup.py
```

### Comparing `cjapy-0.1.1/LICENSE` & `cjapy-0.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `cjapy-0.1.1/PKG-INFO` & `cjapy-0.2.0/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,28 +1,31 @@
 Metadata-Version: 2.1
 Name: cjapy
-Version: 0.1.1
-Summary: Adobe Customer Journey Analytics API
+Version: 0.2.0
+Summary: Adobe Customer Journey Analytics (CJA) wrapper
 Home-page: https://github.com/pitchmuc/cjapy
 Author: Julien Piccini
-Author-email: piccini.julien@gmail.com
-License: GPL
-Keywords: adobe,analytics,API,python,Customer Journey Analytics,CJA
+Author-email: Julien Piccini <piccini.julien@gmail.com>
+License: Apache License 2.0
+Project-URL: homepage, https://github.com/pitchmuc/cjapy
+Project-URL: changelog, https://github.com/pitchmuc/cjapy/blob/master/docs/releases.md
+Keywords: adobe,analytics,API,python
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python
 Classifier: Topic :: Scientific/Engineering :: Information Analysis
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Development Status :: 4 - Beta
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
+Provides-Extra: dynamic
 License-File: LICENSE
 
 # Adobe Customer Journey API
 
 -----------------------
 
 This is a python wrapper for the Adobe Customer Journey API.\
```

### Comparing `cjapy-0.1.1/README.md` & `cjapy-0.2.0/README.md`

 * *Files identical despite different names*

### Comparing `cjapy-0.1.1/cjapy/cjapy.py` & `cjapy-0.2.0/cjapy/cjapy.py`

 * *Files identical despite different names*

### Comparing `cjapy-0.1.1/cjapy/configs.py` & `cjapy-0.2.0/cjapy/configs.py`

 * *Files 24% similar despite different names*

```diff
@@ -24,41 +24,55 @@
     elif path.startswith("\\") and Path("." + path).exists():
         return Path("." + path)
     else:
         return None
 
 
 def createConfigFile(
-    verbose: bool = False, filename: str = "config_analytics_template.json", **kwargs
+    filename: str = "config_analytics_template.json",
+    auth_type:str = "OauthV2",
+    verbose: bool = False, 
+     **kwargs
 ) -> None:
     """Creates a `config_admin.json` file with the pre-defined configuration format
     to store the access data in under the specified `destination`.
+    Parameters: 
+        filename : OPTIONAL : : name of the config file.
+        auth_type : OPTIONAL : type of authentication, either "jwt" or "oauthV2". Default is oauthV2
+        verbose : OPTIONAL : set to true, gives you a print stateent where is the location.
     """
     json_data = {
         "org_id": "<orgID>",
         "client_id": "<APIkey>",
-        "tech_id": "<something>@techacct.adobe.com",
         "secret": "<YourSecret>",
-        "pathToKey": "<path/to/your/privatekey.key>",
     }
+    if auth_type == 'jwt':
+        json_data["tech_id"] = "<something>@techacct.adobe.com"
+        json_data["pathToKey"] = "<path/to/your/privatekey.key>"
+    elif auth_type == 'OauthV2':
+        json_data["scopes"] = "<scopes>"
     with open(filename, "w") as cf:
         cf.write(json.dumps(json_data, indent=4))
     if verbose:
         print(
             f" file created at this location : {os.getcwd()}{os.sep}config_analytics.json"
         )
 
 
-def importConfigFile(path: str) -> None:
+def importConfigFile(
+        path: str = None,
+        auth_type: str = None,
+        )-> None:
     """Reads the file denoted by the supplied `path` and retrieves the configuration information
     from it.
 
     Arguments:
         path: REQUIRED : path to the configuration file. Can be either a fully-qualified or relative.
-
+        auth_type : OPTIONAL : type of authentication, either "jwt" or "oauthV2". Detected based on keys present in config file.
+    
     Example of path value.
     "config.json"
     "./config.json"
     "/my-folder/config.json"
     """
 
     config_file_path: Optional[Path] = find_path(path)
@@ -74,60 +88,71 @@
             client_id = provided_config["api_key"]
         elif "client_id" in provided_keys:
             client_id = provided_config["client_id"]
         else:
             raise RuntimeError(
                 f"Either an `api_key` or a `client_id` should be provided."
             )
-        configure(
-            org_id=provided_config["org_id"],
-            tech_id=provided_config["tech_id"],
-            secret=provided_config["secret"],
-            path_to_key=provided_config["pathToKey"],
-            client_id=client_id,
-        )
+        if auth_type is None:
+            if 'scopes' in provided_keys:
+                auth_type = 'oauthV2'
+            elif 'tech_id' in provided_keys and "pathToKey" in provided_keys:
+                auth_type = 'jwt'
+        args = {
+            "org_id": provided_config["org_id"],
+            "client_id": client_id,
+            "secret": provided_config["secret"],
+        }
+        if auth_type == "jwt":
+            args["tech_id"] = provided_config["tech_id"]
+            args["path_to_key"] = provided_config["pathToKey"]
+        elif auth_type == "oauthV2":
+            args["scopes"] = provided_config["scopes"].replace(' ','')
+        configure(**args)
 
 
 def configure(
     org_id: str = None,
     tech_id: str = None,
     secret: str = None,
     client_id: str = None,
     path_to_key: str = None,
     private_key: str = None,
+    scopes: str = None
 ):
     """Performs programmatic configuration of the API using provided values.
     Arguments:
         org_id : REQUIRED : Organization ID
         tech_id : REQUIRED : Technical Account ID
         secret : REQUIRED : secret generated for your connection
         client_id : REQUIRED : The client_id (old api_key) provided by the JWT connection.
         path_to_key : REQUIRED : If you have a file containing your private key value.
         private_key : REQUIRED : If you do not use a file but pass a variable directly.
+        scopes : OPTIONAL : The scope define in your project for your API connection. Oauth V2, for clients and customers.
     """
     if not org_id:
         raise ValueError("`org_id` must be specified in the configuration.")
     if not client_id:
         raise ValueError("`client_id` must be specified in the configuration.")
-    if not tech_id:
-        raise ValueError("`tech_id` must be specified in the configuration.")
+    if tech_id is None and (path_to_key is None and private_key is None) and scopes is None:
+        raise ValueError("either `scopes` needs to be specified or one of `private_key` or `path_to_key` with tech_id")
     if not secret:
         raise ValueError("`secret` must be specified in the configuration.")
-    if not path_to_key and not private_key:
-        raise ValueError(
-            "`pathToKey` or `private_key` must be specified in the configuration."
-        )
     config_object["org_id"] = org_id
     config_object["client_id"] = client_id
     header["x-api-key"] = client_id
     header["x-gw-ims-org-id"] = org_id
     config_object["tech_id"] = tech_id
     config_object["secret"] = secret
     config_object["pathToKey"] = path_to_key
     config_object["private_key"] = private_key
+    config_object["scopes"] = scopes
+    config_object["jwtTokenEndpoint"] = f"{config_object['imsEndpoint']}/ims/exchange/jwt"
+    config_object["oauthTokenEndpointV2"] = f"{config_object['imsEndpoint']}/ims/token/v2"
+
     # ensure the reset of the state by overwriting possible values from previous import.
     config_object["date_limit"] = 0
     config_object["token"] = ""
 
 
 def get_private_key_from_config(config: dict) -> str:
     """
@@ -142,27 +167,27 @@
             f'Unable to find the private key under path `{config["pathToKey"]}`.'
         )
     with open(Path(private_key_path), "r") as f:
         private_key = f.read()
     return private_key
 
 
-def generateLoggingObject() -> dict:
+def generateLoggingObject(level:str="WARNING",filename:str="cjapy.log") -> dict:
     """
     Generates a dictionary for the logging object with basic configuration.
     You can find the information for the different possible values on the logging documentation.
         https://docs.python.org/3/library/logging.html
     Output:
         level : Level of the logger to display information (NOTSET, DEBUG,INFO,WARNING,EROR,CRITICAL)
         stream : If the logger should display print statements
         file : If the logger should write the messages to a file
         filename : name of the file where log are written
         format : format of the logs
     """
     myObject = {
-        "level": "WARNING",
+        "level": level,
         "stream": True,
         "file": False,
         "format": "%(asctime)s::%(name)s::%(funcName)s::%(levelname)s::%(message)s::%(lineno)d",
-        "filename": "cjapy.log",
+        "filename": filename,
     }
     return myObject
```

### Comparing `cjapy-0.1.1/cjapy/connector.py` & `cjapy-0.2.0/cjapy/connector.py`

 * *Files 4% similar despite different names*

```diff
@@ -43,46 +43,61 @@
         self.config = deepcopy(config_object)
         self.header = deepcopy(header)
         self.loggingEnabled = loggingEnabled
         self.logger = logger
         self.restTime = 30
         self.retry = retry
         if self.config["token"] == "" or time.time() > self.config["date_limit"]:
-            token_and_expiry = token_provider.get_token_and_expiry_for_config(
-                config=self.config, verbose=verbose
-            )
+            if self.config["private_key"] is not None or self.config["pathToKey"] is not None:
+                self.connectionType = 'jwt'
+                token_and_expiry = token_provider.get_jwt_token_and_expiry_for_config(
+                    config=self.config, verbose=verbose
+                )
+                
+            elif self.config["scopes"] is not None:
+                self.connectionType = 'oauthV2'
+                token_and_expiry = token_provider.get_oauth_token_and_expiry_for_config(
+                    config=self.config,
+                    verbose=verbose
+                )
             token = token_and_expiry["token"]
             expiry = token_and_expiry["expiry"]
             if self.loggingEnabled:
-                self.logger.info(f"token retrieved : {token}")
+                self.logger.info(f"token retrieved: {token}")
             self.token = token
             self.config["token"] = token
-            self.config["date_limit"] = time.time() + expiry / 1000 - 500
+            self.config["date_limit"] = time.time() + expiry - 500
             self.header.update({"Authorization": f"Bearer {token}"})
 
     def _checkingDate(self) -> None:
         """
         Checking if the token is still valid
         """
         now = time.time()
         if now > self.config["date_limit"]:
             if self.loggingEnabled:
                 self.logger.warning("token expired. Trying to retrieve a new token")
-            token_with_expiry = token_provider.get_token_and_expiry_for_config(
-                config=self.config
-            )
+            if self.connectionType == 'jwt':
+                token_with_expiry = token_provider.get_jwt_token_and_expiry_for_config(
+                    config=self.config)
+            elif self.connectionType == 'oauthV2':
+                token_with_expiry = token_provider.get_oauth_token_and_expiry_for_config(
+                    config=self.config,
+                    connectionType=self.connectionType)
             token = token_with_expiry["token"]
+            expiry = token_with_expiry["expiry"]
             if self.loggingEnabled:
                 self.logger.info("new token retrieved : {token}")
             self.config["token"] = token
+            self.config["date_limit"] = time.time() + expiry - 500
+            self.header.update({"Authorization": f"Bearer {token}"})
             self.config["date_limit"] = (
-                time.time() + token_with_expiry["expiry"] / 1000 - 500
+                time.time() + (token_with_expiry["expiry"]) - 500
             )
-            self.header.update({"Authorization": f"Bearer {token}"})
-
+            
     def getData(
         self,
         endpoint: str,
         params: dict = None,
         data: dict = None,
         headers: dict = None,
         *args,
```

### Comparing `cjapy-0.1.1/cjapy/projects.py` & `cjapy-0.2.0/cjapy/projects.py`

 * *Files identical despite different names*

### Comparing `cjapy-0.1.1/cjapy/requestCreator.py` & `cjapy-0.2.0/cjapy/requestCreator.py`

 * *Files identical despite different names*

### Comparing `cjapy-0.1.1/cjapy/token_provider.py` & `cjapy-0.2.0/cjapy/token_provider.py`

 * *Files 20% similar despite different names*

```diff
@@ -2,17 +2,18 @@
 import time
 from typing import Dict, Union
 
 import jwt
 import requests
 
 from cjapy import configs
+import json
 
 
-def get_token_and_expiry_for_config(config: dict, verbose: bool = False, save: bool = False, *args, **kwargs) -> \
+def get_jwt_token_and_expiry_for_config(config: dict, verbose: bool = False, save: bool = False, *args, **kwargs) -> \
         Dict[str, str]:
     """
     Retrieve the token by using the information provided by the user during the import importConfigFile function.
     ArgumentS :
         verbose : OPTIONAL : Default False. If set to True, print information.
         save : OPTIONAL : Default False. If set to True, save the toke in the .
     """
@@ -33,32 +34,58 @@
     encoded_jwt = _get_jwt(payload=jwt_payload, private_key=private_key)
 
     payload = {
         'client_id': config['client_id'],
         'client_secret': config['secret'],
         'jwt_token': encoded_jwt
     }
-    response = requests.post(config['tokenEndpoint'], headers=header_jwt, data=payload)
+    response = requests.post(config['jwtTokenEndpoint'], headers=header_jwt, data=payload)
     json_response = response.json()
     try:
         token = json_response['access_token']
     except KeyError:
         print('Issue retrieving token')
         print(json_response)
-    expiry = json_response['expires_in']
+    expiry = json_response['expires_in'] / 1000
     if save:
         with open('token.txt', 'w') as f:
             f.write(token)
         print(f'token has been saved here: {os.getcwd()}{os.sep}token.txt')
     if verbose:
-        print('token valid till : ' + time.ctime(time.time() + expiry / 1000))
+        print('token valid till : ' + time.ctime(time.time() + expiry))
     return {'token': token, 'expiry': expiry}
 
 
 def _get_jwt(payload: dict, private_key: str) -> str:
     """
     Ensure that jwt enconding return the same type (str) as versions < 2.0.0 returned bytes and >2.0.0 return strings. 
     """
     token: Union[str, bytes] = jwt.encode(payload, private_key, algorithm='RS256')
     if isinstance(token, bytes):
         return token.decode('utf-8')
     return token
+
+def get_oauth_token_and_expiry_for_config(config: dict, 
+        verbose: bool = False,
+        save: bool = False
+    ) -> Dict[str, str]:
+        """
+        Retrieve the access token by using the OAuth information provided by the user
+        during the import importConfigFile function.
+        Arguments :
+            config : REQUIRED : Configuration object.
+            verbose : OPTIONAL : Default False. If set to True, print information.
+            save : OPTIONAL : Default False. If set to True, save the toke in the .
+        """
+        oauth_payload = {
+            "grant_type": "client_credentials",
+            "client_id": config["client_id"],
+            "client_secret": config["secret"],
+            "scope": config["scopes"]
+        }
+        response = requests.post(
+            config["oauthTokenEndpointV2"], data=oauth_payload
+        )
+        responseJson = response.json()
+        token = responseJson.get('access_token')
+        expiry = responseJson.get("expires_in")
+        return {'token': token, 'expiry': expiry}
```

### Comparing `cjapy-0.1.1/cjapy/workspace.py` & `cjapy-0.2.0/cjapy/workspace.py`

 * *Files identical despite different names*

### Comparing `cjapy-0.1.1/cjapy.egg-info/PKG-INFO` & `cjapy-0.2.0/cjapy.egg-info/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,28 +1,31 @@
 Metadata-Version: 2.1
 Name: cjapy
-Version: 0.1.1
-Summary: Adobe Customer Journey Analytics API
+Version: 0.2.0
+Summary: Adobe Customer Journey Analytics (CJA) wrapper
 Home-page: https://github.com/pitchmuc/cjapy
 Author: Julien Piccini
-Author-email: piccini.julien@gmail.com
-License: GPL
-Keywords: adobe,analytics,API,python,Customer Journey Analytics,CJA
+Author-email: Julien Piccini <piccini.julien@gmail.com>
+License: Apache License 2.0
+Project-URL: homepage, https://github.com/pitchmuc/cjapy
+Project-URL: changelog, https://github.com/pitchmuc/cjapy/blob/master/docs/releases.md
+Keywords: adobe,analytics,API,python
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python
 Classifier: Topic :: Scientific/Engineering :: Information Analysis
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Development Status :: 4 - Beta
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
+Provides-Extra: dynamic
 License-File: LICENSE
 
 # Adobe Customer Journey API
 
 -----------------------
 
 This is a python wrapper for the Adobe Customer Journey API.\
```

### Comparing `cjapy-0.1.1/setup.py` & `cjapy-0.2.0/setup.py`

 * *Files identical despite different names*

