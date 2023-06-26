# Comparing `tmp/ibmpairs-0.2.8.tar.gz` & `tmp/ibmpairs-0.2.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ibmpairs-0.2.8.tar", last modified: Tue Jun 13 14:28:44 2023, max compression
+gzip compressed data, was "ibmpairs-0.2.9.tar", last modified: Mon Jun 26 13:15:29 2023, max compression
```

## Comparing `ibmpairs-0.2.8.tar` & `ibmpairs-0.2.9.tar`

### file list

```diff
@@ -1,35 +1,35 @@
-drwxr-xr-x   0 staylor    (501) staff       (20)        0 2023-06-13 14:28:44.599039 ibmpairs-0.2.8/
--rw-r--r--   0 staylor    (501) staff       (20)     6699 2023-06-13 14:21:21.000000 ibmpairs-0.2.8/CONTRIBUTING.md
--rw-r--r--   0 staylor    (501) staff       (20)     1488 2023-06-13 14:21:21.000000 ibmpairs-0.2.8/LICENSE
--rw-r--r--   0 staylor    (501) staff       (20)      335 2023-06-13 14:21:21.000000 ibmpairs-0.2.8/MAINTAINERS.md
--rw-r--r--   0 staylor    (501) staff       (20)      281 2023-06-13 14:21:21.000000 ibmpairs-0.2.8/MANIFEST.in
--rw-r--r--   0 staylor    (501) staff       (20)     3270 2023-06-13 14:28:44.599115 ibmpairs-0.2.8/PKG-INFO
--rw-r--r--   0 staylor    (501) staff       (20)     2520 2023-06-13 14:21:21.000000 ibmpairs-0.2.8/README.md
-drwxr-xr-x   0 staylor    (501) staff       (20)        0 2023-06-13 14:28:44.597690 ibmpairs-0.2.8/ibmpairs/
--rw-r--r--   0 staylor    (501) staff       (20)    63867 2023-06-13 13:01:01.000000 ibmpairs-0.2.8/ibmpairs/authentication.py
--rw-r--r--   0 staylor    (501) staff       (20)   412432 2023-05-17 14:56:54.000000 ibmpairs-0.2.8/ibmpairs/catalog.py
--rw-r--r--   0 staylor    (501) staff       (20)    40851 2023-06-13 08:16:26.000000 ibmpairs-0.2.8/ibmpairs/client.py
--rw-r--r--   0 staylor    (501) staff       (20)    13679 2023-06-09 08:29:50.000000 ibmpairs-0.2.8/ibmpairs/common.py
--rw-r--r--   0 staylor    (501) staff       (20)     1112 2023-05-17 14:56:54.000000 ibmpairs-0.2.8/ibmpairs/config.py
--rw-r--r--   0 staylor    (501) staff       (20)     5189 2023-06-08 14:13:08.000000 ibmpairs-0.2.8/ibmpairs/constants.py
--rw-r--r--   0 staylor    (501) staff       (20)    16020 2023-06-09 13:08:53.000000 ibmpairs-0.2.8/ibmpairs/dashboard.py
-drwxr-xr-x   0 staylor    (501) staff       (20)        0 2023-06-13 14:28:44.598803 ibmpairs-0.2.8/ibmpairs/external/
--rw-r--r--   0 staylor    (501) staff       (20)   102439 2023-05-17 14:56:54.000000 ibmpairs-0.2.8/ibmpairs/external/ibm.py
--rw-r--r--   0 staylor    (501) staff       (20)      391 2023-05-17 14:56:54.000000 ibmpairs-0.2.8/ibmpairs/logger.py
--rw-r--r--   0 staylor    (501) staff       (20)    26501 2023-06-13 09:33:56.000000 ibmpairs-0.2.8/ibmpairs/messages.py
--rw-r--r--   0 staylor    (501) staff       (20)   166380 2023-05-19 08:50:17.000000 ibmpairs-0.2.8/ibmpairs/paw.py
--rw-r--r--   0 staylor    (501) staff       (20)   357366 2023-05-18 11:15:15.000000 ibmpairs-0.2.8/ibmpairs/query.py
--rw-r--r--   0 staylor    (501) staff       (20)   164223 2023-05-18 11:15:34.000000 ibmpairs-0.2.8/ibmpairs/upload.py
--rw-r--r--   0 staylor    (501) staff       (20)    11334 2023-05-17 14:56:54.000000 ibmpairs-0.2.8/ibmpairs/utils.py
--rw-r--r--   0 staylor    (501) staff       (20)       42 2023-06-13 14:28:44.000000 ibmpairs-0.2.8/ibmpairs/version.py
-drwxr-xr-x   0 staylor    (501) staff       (20)        0 2023-06-13 14:28:44.598534 ibmpairs-0.2.8/ibmpairs.egg-info/
--rw-r--r--   0 staylor    (501) staff       (20)     3270 2023-06-13 14:28:44.000000 ibmpairs-0.2.8/ibmpairs.egg-info/PKG-INFO
--rw-r--r--   0 staylor    (501) staff       (20)      619 2023-06-13 14:28:44.000000 ibmpairs-0.2.8/ibmpairs.egg-info/SOURCES.txt
--rw-r--r--   0 staylor    (501) staff       (20)        1 2023-06-13 14:28:44.000000 ibmpairs-0.2.8/ibmpairs.egg-info/dependency_links.txt
--rw-r--r--   0 staylor    (501) staff       (20)        1 2023-06-13 14:28:44.000000 ibmpairs-0.2.8/ibmpairs.egg-info/not-zip-safe
--rw-r--r--   0 staylor    (501) staff       (20)      187 2023-06-13 14:28:44.000000 ibmpairs-0.2.8/ibmpairs.egg-info/requires.txt
--rw-r--r--   0 staylor    (501) staff       (20)        9 2023-06-13 14:28:44.000000 ibmpairs-0.2.8/ibmpairs.egg-info/top_level.txt
--rw-r--r--   0 staylor    (501) staff       (20)       60 2023-06-13 14:21:21.000000 ibmpairs-0.2.8/requirements-development.txt
--rw-r--r--   0 staylor    (501) staff       (20)      184 2023-06-13 14:21:21.000000 ibmpairs-0.2.8/requirements.txt
--rw-r--r--   0 staylor    (501) staff       (20)      103 2023-06-13 14:28:44.599427 ibmpairs-0.2.8/setup.cfg
--rwxr-xr-x   0 staylor    (501) staff       (20)     1838 2023-06-13 14:24:49.000000 ibmpairs-0.2.8/setup.py
+drwxr-xr-x   0 staylor    (501) staff       (20)        0 2023-06-26 13:15:29.039194 ibmpairs-0.2.9/
+-rw-r--r--   0 staylor    (501) staff       (20)     6699 2023-06-26 13:05:03.000000 ibmpairs-0.2.9/CONTRIBUTING.md
+-rw-r--r--   0 staylor    (501) staff       (20)     1488 2023-06-26 13:05:03.000000 ibmpairs-0.2.9/LICENSE
+-rw-r--r--   0 staylor    (501) staff       (20)      335 2023-06-26 13:05:03.000000 ibmpairs-0.2.9/MAINTAINERS.md
+-rw-r--r--   0 staylor    (501) staff       (20)      281 2023-06-26 13:05:03.000000 ibmpairs-0.2.9/MANIFEST.in
+-rw-r--r--   0 staylor    (501) staff       (20)     3270 2023-06-26 13:15:29.039255 ibmpairs-0.2.9/PKG-INFO
+-rw-r--r--   0 staylor    (501) staff       (20)     2520 2023-06-26 13:05:03.000000 ibmpairs-0.2.9/README.md
+drwxr-xr-x   0 staylor    (501) staff       (20)        0 2023-06-26 13:15:29.038104 ibmpairs-0.2.9/ibmpairs/
+-rw-r--r--   0 staylor    (501) staff       (20)    63825 2023-06-26 13:14:50.000000 ibmpairs-0.2.9/ibmpairs/authentication.py
+-rw-r--r--   0 staylor    (501) staff       (20)   412432 2023-06-26 13:05:03.000000 ibmpairs-0.2.9/ibmpairs/catalog.py
+-rw-r--r--   0 staylor    (501) staff       (20)    40899 2023-06-26 13:14:50.000000 ibmpairs-0.2.9/ibmpairs/client.py
+-rw-r--r--   0 staylor    (501) staff       (20)    15441 2023-06-26 13:14:50.000000 ibmpairs-0.2.9/ibmpairs/common.py
+-rw-r--r--   0 staylor    (501) staff       (20)     1112 2023-06-26 13:05:03.000000 ibmpairs-0.2.9/ibmpairs/config.py
+-rw-r--r--   0 staylor    (501) staff       (20)     5152 2023-06-26 13:14:50.000000 ibmpairs-0.2.9/ibmpairs/constants.py
+-rw-r--r--   0 staylor    (501) staff       (20)    16020 2023-06-26 13:05:03.000000 ibmpairs-0.2.9/ibmpairs/dashboard.py
+drwxr-xr-x   0 staylor    (501) staff       (20)        0 2023-06-26 13:15:29.039013 ibmpairs-0.2.9/ibmpairs/external/
+-rw-r--r--   0 staylor    (501) staff       (20)   102439 2023-06-26 13:05:03.000000 ibmpairs-0.2.9/ibmpairs/external/ibm.py
+-rw-r--r--   0 staylor    (501) staff       (20)      391 2023-06-26 13:05:03.000000 ibmpairs-0.2.9/ibmpairs/logger.py
+-rw-r--r--   0 staylor    (501) staff       (20)    26501 2023-06-26 13:05:03.000000 ibmpairs-0.2.9/ibmpairs/messages.py
+-rw-r--r--   0 staylor    (501) staff       (20)   166380 2023-06-26 13:05:03.000000 ibmpairs-0.2.9/ibmpairs/paw.py
+-rw-r--r--   0 staylor    (501) staff       (20)   357366 2023-06-26 13:05:03.000000 ibmpairs-0.2.9/ibmpairs/query.py
+-rw-r--r--   0 staylor    (501) staff       (20)   164223 2023-06-26 13:05:03.000000 ibmpairs-0.2.9/ibmpairs/upload.py
+-rw-r--r--   0 staylor    (501) staff       (20)    11334 2023-06-26 13:05:03.000000 ibmpairs-0.2.9/ibmpairs/utils.py
+-rw-r--r--   0 staylor    (501) staff       (20)       42 2023-06-26 13:15:28.000000 ibmpairs-0.2.9/ibmpairs/version.py
+drwxr-xr-x   0 staylor    (501) staff       (20)        0 2023-06-26 13:15:29.038889 ibmpairs-0.2.9/ibmpairs.egg-info/
+-rw-r--r--   0 staylor    (501) staff       (20)     3270 2023-06-26 13:15:29.000000 ibmpairs-0.2.9/ibmpairs.egg-info/PKG-INFO
+-rw-r--r--   0 staylor    (501) staff       (20)      619 2023-06-26 13:15:29.000000 ibmpairs-0.2.9/ibmpairs.egg-info/SOURCES.txt
+-rw-r--r--   0 staylor    (501) staff       (20)        1 2023-06-26 13:15:29.000000 ibmpairs-0.2.9/ibmpairs.egg-info/dependency_links.txt
+-rw-r--r--   0 staylor    (501) staff       (20)        1 2023-06-26 13:13:06.000000 ibmpairs-0.2.9/ibmpairs.egg-info/not-zip-safe
+-rw-r--r--   0 staylor    (501) staff       (20)      187 2023-06-26 13:15:29.000000 ibmpairs-0.2.9/ibmpairs.egg-info/requires.txt
+-rw-r--r--   0 staylor    (501) staff       (20)        9 2023-06-26 13:15:29.000000 ibmpairs-0.2.9/ibmpairs.egg-info/top_level.txt
+-rw-r--r--   0 staylor    (501) staff       (20)       60 2023-06-26 13:05:03.000000 ibmpairs-0.2.9/requirements-development.txt
+-rw-r--r--   0 staylor    (501) staff       (20)      184 2023-06-26 13:05:03.000000 ibmpairs-0.2.9/requirements.txt
+-rw-r--r--   0 staylor    (501) staff       (20)      103 2023-06-26 13:15:29.039538 ibmpairs-0.2.9/setup.cfg
+-rwxr-xr-x   0 staylor    (501) staff       (20)     1838 2023-06-26 13:14:50.000000 ibmpairs-0.2.9/setup.py
```

### Comparing `ibmpairs-0.2.8/CONTRIBUTING.md` & `ibmpairs-0.2.9/CONTRIBUTING.md`

 * *Files identical despite different names*

### Comparing `ibmpairs-0.2.8/LICENSE` & `ibmpairs-0.2.9/LICENSE`

 * *Files identical despite different names*

### Comparing `ibmpairs-0.2.8/PKG-INFO` & `ibmpairs-0.2.9/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ibmpairs
-Version: 0.2.8
+Version: 0.2.9
 Summary: open source Python modules for the IBM PAIRS Geoscope platform
 Home-page: https://ibmpairs.mybluemix.net
 Author: Physical Analytics, IBM Research
 Author-email: pairs@us.ibm.com
 Maintainer: cmalbrec
 License: BSD-Clause-3
 Project-URL: Documentation, https://pairs.res.ibm.com/tutorial
```

### Comparing `ibmpairs-0.2.8/README.md` & `ibmpairs-0.2.9/README.md`

 * *Files identical despite different names*

### Comparing `ibmpairs-0.2.8/ibmpairs/authentication.py` & `ibmpairs-0.2.9/ibmpairs/authentication.py`

 * *Files 1% similar despite different names*

```diff
@@ -113,31 +113,31 @@
         else:
             self._legacy = GLOBAL_LEGACY_ENVIRONMENT
         
         if host is not None:
             self._host = common.strip_protocol(host)
         else:
             if self._legacy is True:
-                self._host = common.strip_protocol(constants.CLIENT_LEGACY_URL)
+                self._host = common.ensure_api_path(common.strip_protocol(constants.CLIENT_LEGACY_URL))
             else:
-                self._host = common.strip_protocol(constants.CLIENT_URL)
+                self._host = common.ensure_api_path(common.strip_protocol(constants.CLIENT_URL))
         
         self._username      = username
         self._password      = password
         
         if password_file is not None:
             self._password_file = password_file
         else:
             self._password_file = "auth/basic.txt"
         
         if ((self._password is None) and (self._username is not None)):
             try:
-                self.set_credentials_from_file(self._username, self._password_file, self._host)
+                self.set_credentials_from_file(self._username, self._password_file, common.strip_api_path(self._host))
             except Exception as e:
-                msg = messages.INFO_AUTHENTICATION_PASSWORD_NOT_FOUND_IN_FILE.format(self._username, self._password_file, self._host)
+                msg = messages.INFO_AUTHENTICATION_PASSWORD_NOT_FOUND_IN_FILE.format(self._username, self._password_file, common.strip_api_path(self._host))
                 logger.info(msg)
         
         if (self._password is None) or (self._username is None):
             msg = messages.ERROR_AUTHENTICATION_FAILED.format('username and password')
             logger.error(msg)
             raise common.PAWException(msg)
             
@@ -807,17 +807,17 @@
         else:
             self._legacy = GLOBAL_LEGACY_ENVIRONMENT
         
         if host is not None:
             self._host = common.strip_protocol(host)
         else:
             if self._legacy is True:
-                self._host = common.strip_protocol(constants.CLIENT_LEGACY_URL)
+                self._host = common.ensure_api_path(common.strip_protocol(constants.CLIENT_LEGACY_URL))
             else:
-                self._host = common.strip_protocol(constants.CLIENT_URL)
+                self._host = common.ensure_api_path(common.strip_protocol(constants.CLIENT_URL))
         
         self._username      = username
         self._api_key       = api_key
         self._api_key_file  = api_key_file
         
         if self._legacy is True:
             if client_id is not None:
@@ -876,18 +876,18 @@
                 logger.error(msg)
                 raise common.PAWException(msg)
         
         if ((self._api_key is None) and (self._username is not None)):
             try:
                 self.set_credentials_from_file(self._username,
                                                self._api_key_file, 
-                                               self._host
+                                               common.strip_api_path(self._host)
                                               )
             except:
-                msg = messages.INFO_AUTHENTICATION_API_KEY_NOT_FOUND_IN_FILE.format(self._username, self._api_key_file, self._host)
+                msg = messages.INFO_AUTHENTICATION_API_KEY_NOT_FOUND_IN_FILE.format(self._username, self._api_key_file, common.strip_api_path(self._host))
                 logger.info(msg)
         
         if (self._api_key is not None):
             try:
                 self.get_auth_token(api_key      = self._api_key,
                                     client_id    = self._client_id, 
                                     endpoint     = self._endpoint,
@@ -1135,16 +1135,14 @@
         
         :param api_key:   An api key for the authentication system.
         :type api_key:    str
         :param client_id: A client id for the authentication system.
         :type client_id:  str
         :param endpoint:  The authentication endpoint.
         :type endpoint:   str
-        :param verify:    Verify ssl.
-        :type verify:     boolean
         """
         
         response               = None
         response_oauth2_return = None
         
         if api_key is not None:
             self.set_api_key(api_key)
@@ -1201,17 +1199,14 @@
     #
     def phoenix_refresh_auth_token(self,
                                    verify    = constants.GLOBAL_SSL_VERIFY
                                   ):
         
         """
         The method submits a request to the authentication system for a refreshed token, gets a response and updates the internal self._oauth2_return and self._jwt_token objects.
-
-        :param verify:       Verify ssl.
-        :type verify:        boolean
         """
         
         msg = messages.INFO_AUTHENTICATION_TOKEN_REFRESH
         logger.info(msg)
         
         response               = None
         response_oauth2_return = None
@@ -1278,15 +1273,15 @@
         :param api_key:      An api key for the authentication system.
         :type api_key:       str
         :param client_id:    A client id for the authentication system.
         :type client_id:     str
         :param endpoint:     The authentication endpoint.
         :type endpoint:      str
         :param verify:       Verify ssl.
-        :type verify:        boolean
+        :type endpoint:      boolean
         :param iam_endpoint: IBM Cloud IAM Endpoint
         :type iam_endpoint:  str
         :param org_id:       IBM EIS GA API Connect Org Id
         :type org_id:        str
         :param tenant_id:    IBM EIS GA API Connect Tenant Id
         :type tenant_id:     str
         """
@@ -1383,17 +1378,14 @@
     #
     def api_connect_refresh_auth_token(self,
                                        verify = constants.GLOBAL_SSL_VERIFY
                                       ):
         
         """
         The method performs a new api_connect_get_auth_token.
-
-        :param verify:       Verify ssl.
-        :type verify:        boolean
         """
         
         self.api_connect_get_auth_token()
         
     #
     def get_auth_token(self, 
                        api_key      = None,
```

### Comparing `ibmpairs-0.2.8/ibmpairs/catalog.py` & `ibmpairs-0.2.9/ibmpairs/catalog.py`

 * *Files identical despite different names*

### Comparing `ibmpairs-0.2.8/ibmpairs/client.py` & `ibmpairs-0.2.9/ibmpairs/client.py`

 * *Files 0% similar despite different names*

```diff
@@ -256,17 +256,17 @@
             
             if (host is not None):
                 self._host = common.ensure_protocol(host)
             elif (host is None) and (self._authentication is not None) and (self._authentication.host is not None):
                 self._host = common.ensure_protocol(self._authentication.host)
             else:
                 if self._legacy is True:
-                    self._host = common.ensure_protocol(constants.CLIENT_LEGACY_URL)
+                    self._host = common.ensure_api_path(common.ensure_protocol(constants.CLIENT_LEGACY_URL))
                 else:
-                    self._host = common.ensure_protocol(constants.CLIENT_URL)
+                    self._host = common.ensure_api_path(common.ensure_protocol(constants.CLIENT_URL))
                     
             logger.info("HOST: " + self._host)
             
             self._body = body
             
             if self._legacy is True:
                 if client_id is not None:
```

### Comparing `ibmpairs-0.2.8/ibmpairs/common.py` & `ibmpairs-0.2.9/ibmpairs/common.py`

 * *Files 4% similar despite different names*

```diff
@@ -299,14 +299,33 @@
         logger.error(msg)
         raise PAWException(msg)
     
     return string
 #}}}
 
 #
+def strip_slash(input: str):
+    
+    """
+    The method ensures a slash is not at the end of a string.
+
+    :param intput:      The input string to check.
+    :type input:        str
+    :returns:           A string without a trailing "/".
+    :rtype:             str
+    """ 
+    
+    result = str(input)
+    
+    if result.endswith("/"):
+        result = result[:-1]
+        
+    return result
+
+#
 def ensure_slash(directory: str, 
                  position: int
                 ):
     
     """
     The method ensures a slash is present.
 
@@ -463,7 +482,62 @@
             tenant_id = client_id[9:len(client_id)]
         elif client_id.startswith('geospatial-'):
             tenant_id = client_id[11:len(client_id)]
             
         return tenant_id
     else:
         return None
+
+#
+def ensure_api_path(host: str):
+    
+    """
+    Adds /core/v3 or /v2 to host
+
+    :param host:   The host string.
+    :type host:    str
+    :returns:      The host string with path added.
+    :rtype:        str
+    """ 
+    
+    result = str(strip_slash(host))
+    
+    if ("pairs.res.ibm.com" in result):
+        if ("v2" not in result):
+            result = result + "/v2"
+    elif ("api.ibm.com" in result):
+        
+        if (result.endswith("api.ibm.com")):
+            result = result + "/geospatial/run/na"
+        elif (result.endswith("api.ibm.com/geospatial")):
+            result = result + "/run/na"
+        elif (result.endswith("api.ibm.com/geospatial/run")):
+            result = result + "/na"
+            
+        if ("core/v3" not in result):
+            if (result.endswith("core")):
+                result = result + "/v3"
+            else:
+                result = result + "/core/v3"
+                
+    return result
+
+#
+def strip_api_path(host: str):
+    
+    """
+    Removes core/v3 and /v2 from a string.
+
+    :param host:   The host string.
+    :type host:    str
+    :returns:      The host string with the path.
+    :rtype:        str
+    """ 
+
+    result = str(host)
+    
+    if (result.endswith("/core/v3")):
+        result = result[:-8]
+    elif host.endswith('/v2'):
+        result = result[:-3]
+        
+    return result
```

### Comparing `ibmpairs-0.2.8/ibmpairs/config.py` & `ibmpairs-0.2.9/ibmpairs/config.py`

 * *Files identical despite different names*

### Comparing `ibmpairs-0.2.8/ibmpairs/constants.py` & `ibmpairs-0.2.9/ibmpairs/constants.py`

 * *Files 6% similar despite different names*

```diff
@@ -17,40 +17,40 @@
 
 PAW_LOG_LEVEL                 = os.environ.get('PAW_LOG_LEVEL', 'INFO')
 GLOBAL_JSON_REPR_INDENT       = int(os.environ.get('GLOBAL_JSON_REPR_INDENT', 4))
 GLOBAL_JSON_REPR_SORT_KEYS    = os.environ.get('GLOBAL_JSON_REPR_SORT_KEYS', True)
 GLOBAL_SSL_VERIFY             = True
 
 # catalog
-CATALOG_DATA_SETS_API                   = '/v2/datasets/'
-CATALOG_DATA_SETS_API_FULL              = '/v2/datasets/full'
+CATALOG_DATA_SETS_API                   = '/datasets/'
+CATALOG_DATA_SETS_API_FULL              = '/datasets/full'
 CATALOG_DATA_SETS_LAYERS_API            = '/datalayers'
 
-CATALOG_DATA_LAYERS_API                 = '/v2/datalayers/'
-CATALOG_DATA_LAYERS_API_FULL            = '/v2/datalayers/full'
+CATALOG_DATA_LAYERS_API                 = '/datalayers/'
+CATALOG_DATA_LAYERS_API_FULL            = '/datalayers/full'
 CATALOG_DATA_LAYERS_API_PROPERTIES      = '/datalayer_properties'
 CATALOG_DATA_LAYERS_API_DIMENSIONS      = '/datalayer_dimensions'
 
-CATALOG_DATA_LAYER_DIMENSIONS_API       = '/v2/datalayer_dimensions/'
-CATALOG_DATA_LAYER_DIMENSION_VALUES_API = '/v2/datalayer_dimension_values/'
+CATALOG_DATA_LAYER_DIMENSIONS_API       = '/datalayer_dimensions/'
+CATALOG_DATA_LAYER_DIMENSION_VALUES_API = '/datalayer_dimension_values/'
 
-CATALOG_DATA_LAYER_PROPERTIES_API       = '/v2/datalayer_properties/'
+CATALOG_DATA_LAYER_PROPERTIES_API       = '/datalayer_properties/'
 
 # client
-CLIENT_URL                       = os.environ.get('CLIENT_URL', 'https://api.ibm.com/geospatial/run/na/pairs-query')
-CLIENT_LEGACY_URL                = os.environ.get('CLIENT_LEGACY_URL', 'https://pairs.res.ibm.com')
+CLIENT_URL                       = os.environ.get('CLIENT_URL', 'https://api.ibm.com/geospatial/run/na/core/v3')
+CLIENT_LEGACY_URL                = os.environ.get('CLIENT_LEGACY_URL', 'https://pairs.res.ibm.com/v2')
 CLIENT_JSON_HEADER               = {"Content-Type": "application/json"}
 CLIENT_PUT_AND_POST_HEADER       = {'Content-Type': 'application/json', 'Accept': 'application/json'}
 CLIENT_PUT_AND_POST_HEADER_CSV   = {'Accept': 'text/csv'}
 CLIENT_GET_DEFAULT_RESPONSE_TYPE = 'json'
 CLIENT_TOKEN_REFRESH_MESSAGE     = 'claim expired'
 CLIENT_TIMEOUT                   = os.environ.get('CLIENT_TIMEOUT', 3600)
 
-UPLOAD_API                     = '/v2/uploader/upload'
-UPLOAD_STATUS_API              = '/v2/uploader/upload/'
+UPLOAD_API                     = '/uploader/upload'
+UPLOAD_STATUS_API              = '/uploader/upload/'
 UPLOAD_METADATA_FILE_EXTENTION = '.meta.json'
 
 UPLOAD_DEFAULT_WORKERS         = int(os.environ.get('UPLOAD_DEFAULT_WORKERS', 1))
 UPLOAD_MAX_WORKERS             = int(os.environ.get('UPLOAD_MAX_WORKERS', 8))
 UPLOAD_MIN_STATUS_INTERVAL     = int(os.environ.get('UPLOAD_MIN_STATUS_INTERVAL', 30))
 UPLOAD_STATUS_CHECK_INTERVAL   = int(os.environ.get('UPLOAD_STATUS_CHECK_INTERVAL', 60))
 UPLOAD_WORKER_DEBUG            = os.environ.get('UPLOAD_WORKER_DEBUG', "False")
@@ -61,17 +61,17 @@
 EIS_REGISTER_QUERY_URL         = EIS_V2_API_URL + '/layer/analytics/metadata'
 
 # phoenix
 PHOENIX_V1_API_URL             = os.environ.get('PHOENIX_V1_API_URL', 'https://api.auth-b2b-twc.ibm.com/api/v1')
 PHOENIX_ADD_DASHBOARD_LAYER    = PHOENIX_V1_API_URL  + '/IMAP/put-layer-config-block'
 
 #query
-QUERY_API                      = '/v2/query'
-QUERY_JOBS_API                 = '/v2/queryjobs/'
-QUERY_JOBS_DOWNLOAD_API        = '/v2/queryjobs/download/'
+QUERY_API                      = '/query'
+QUERY_JOBS_API                 = '/queryjobs/'
+QUERY_JOBS_DOWNLOAD_API        = '/queryjobs/download/'
 QUERY_JOBS_API_MERGE           = '/merge/'
 QUERY_DATE_FORMAT              = '%Y-%m-%d'
 QUERY_DEFAULT_WORKERS          = int(os.environ.get('QUERY_DEFAULT_WORKERS', 1))
 QUERY_MAX_WORKERS              = int(os.environ.get('QUERY_MAX_WORKERS', 8))
 QUERY_MIN_STATUS_INTERVAL      = int(os.environ.get('QUERY_MIN_STATUS_INTERVAL', 15))
 QUERY_STATUS_CHECK_INTERVAL    = int(os.environ.get('QUERY_STATUS_CHECK_INTERVAL', 30))
 QUERY_STATUS_RUNNING_CODES     = [0, 1, 10, 11, 12]
```

### Comparing `ibmpairs-0.2.8/ibmpairs/dashboard.py` & `ibmpairs-0.2.9/ibmpairs/dashboard.py`

 * *Files identical despite different names*

### Comparing `ibmpairs-0.2.8/ibmpairs/external/ibm.py` & `ibmpairs-0.2.9/ibmpairs/external/ibm.py`

 * *Files identical despite different names*

### Comparing `ibmpairs-0.2.8/ibmpairs/messages.py` & `ibmpairs-0.2.9/ibmpairs/messages.py`

 * *Files identical despite different names*

### Comparing `ibmpairs-0.2.8/ibmpairs/paw.py` & `ibmpairs-0.2.9/ibmpairs/paw.py`

 * *Files identical despite different names*

### Comparing `ibmpairs-0.2.8/ibmpairs/query.py` & `ibmpairs-0.2.9/ibmpairs/query.py`

 * *Files identical despite different names*

### Comparing `ibmpairs-0.2.8/ibmpairs/upload.py` & `ibmpairs-0.2.9/ibmpairs/upload.py`

 * *Files identical despite different names*

### Comparing `ibmpairs-0.2.8/ibmpairs/utils.py` & `ibmpairs-0.2.9/ibmpairs/utils.py`

 * *Files identical despite different names*

### Comparing `ibmpairs-0.2.8/ibmpairs.egg-info/PKG-INFO` & `ibmpairs-0.2.9/ibmpairs.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ibmpairs
-Version: 0.2.8
+Version: 0.2.9
 Summary: open source Python modules for the IBM PAIRS Geoscope platform
 Home-page: https://ibmpairs.mybluemix.net
 Author: Physical Analytics, IBM Research
 Author-email: pairs@us.ibm.com
 Maintainer: cmalbrec
 License: BSD-Clause-3
 Project-URL: Documentation, https://pairs.res.ibm.com/tutorial
```

### Comparing `ibmpairs-0.2.8/ibmpairs.egg-info/SOURCES.txt` & `ibmpairs-0.2.9/ibmpairs.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `ibmpairs-0.2.8/setup.py` & `ibmpairs-0.2.9/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 #!/usr/bin/env python
 from setuptools import setup
 
 # define package version
-version = '0.2.8'
+version = '0.2.9'
 # ... and record it for ibmpairs package
 with open("ibmpairs/version.py", 'w') as f:
     f.write('# generated by setup.py\nversion = "{}"\n'.format(version))
 
 def readme():
     try:
         with open('README.md') as f:
```

