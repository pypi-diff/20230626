# Comparing `tmp/cyberwatch_api-0.2.0.tar.gz` & `tmp/cyberwatch_api-0.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/cyberwatch_api-0.2.0.tar", last modified: Fri Jun  9 14:11:12 2023, max compression
+gzip compressed data, was "dist/cyberwatch_api-0.3.0.tar", last modified: Mon Jun 26 08:01:07 2023, max compression
```

## Comparing `cyberwatch_api-0.2.0.tar` & `cyberwatch_api-0.3.0.tar`

### file list

```diff
@@ -1,13 +1,13 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 14:11:12.000000 cyberwatch_api-0.2.0/
--rw-r--r--   0 runner    (1001) docker     (123)     1067 2023-06-09 14:11:00.000000 cyberwatch_api-0.2.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     3960 2023-06-09 14:11:12.000000 cyberwatch_api-0.2.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     3748 2023-06-09 14:11:00.000000 cyberwatch_api-0.2.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 14:11:12.000000 cyberwatch_api-0.2.0/cyberwatch_api.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     3960 2023-06-09 14:11:12.000000 cyberwatch_api-0.2.0/cyberwatch_api.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      233 2023-06-09 14:11:12.000000 cyberwatch_api-0.2.0/cyberwatch_api.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-09 14:11:12.000000 cyberwatch_api-0.2.0/cyberwatch_api.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       17 2023-06-09 14:11:12.000000 cyberwatch_api-0.2.0/cyberwatch_api.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       15 2023-06-09 14:11:12.000000 cyberwatch_api-0.2.0/cyberwatch_api.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)     6587 2023-06-09 14:11:00.000000 cyberwatch_api-0.2.0/cyberwatch_api.py
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-09 14:11:12.000000 cyberwatch_api-0.2.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      447 2023-06-09 14:11:00.000000 cyberwatch_api-0.2.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 08:01:07.000000 cyberwatch_api-0.3.0/
+-rw-r--r--   0 runner    (1001) docker     (123)     1067 2023-06-26 08:00:58.000000 cyberwatch_api-0.3.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     4554 2023-06-26 08:01:07.000000 cyberwatch_api-0.3.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     4342 2023-06-26 08:00:58.000000 cyberwatch_api-0.3.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 08:01:07.000000 cyberwatch_api-0.3.0/cyberwatch_api.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     4554 2023-06-26 08:01:07.000000 cyberwatch_api-0.3.0/cyberwatch_api.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      233 2023-06-26 08:01:07.000000 cyberwatch_api-0.3.0/cyberwatch_api.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-26 08:01:07.000000 cyberwatch_api-0.3.0/cyberwatch_api.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       17 2023-06-26 08:01:07.000000 cyberwatch_api-0.3.0/cyberwatch_api.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       15 2023-06-26 08:01:07.000000 cyberwatch_api-0.3.0/cyberwatch_api.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     5887 2023-06-26 08:00:58.000000 cyberwatch_api-0.3.0/cyberwatch_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-26 08:01:07.000000 cyberwatch_api-0.3.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      447 2023-06-26 08:00:58.000000 cyberwatch_api-0.3.0/setup.py
```

### Comparing `cyberwatch_api-0.2.0/LICENSE` & `cyberwatch_api-0.3.0/LICENSE`

 * *Files identical despite different names*

### Comparing `cyberwatch_api-0.2.0/PKG-INFO` & `cyberwatch_api-0.3.0/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cyberwatch_api
-Version: 0.2.0
+Version: 0.3.0
 Summary: Python Api client for the Cyberwatch software
 Author: CyberWatch SAS
 License: MIT
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # Cyberwatch API
@@ -18,14 +18,15 @@
   - [Prerequisites](#prerequisites)
   - [Module installation](#module-installation)
   - [Configuration](#configuration)
   - [api.conf file location](#apiconf-file-location)
 - [Ping](#ping)
 - [Examples](#examples)
 - [Usage](#usage)
+- [FAQs](#faqs)
 
 <!-- END doctoc generated TOC please keep comment here to allow auto update -->
 ## Installation
 
 ### Prerequisites
 - [ ] [Python 3](https://www.python.org/)
 - [ ] Python [PIP](https://pypi.org/project/pip/)
@@ -125,10 +126,37 @@
     params={'id' : 7}
 )
 ```
 ```python
 output = Cyberwatch_Pyhelper().request(
     method="put",
     endpoint="/api/v3/vulnerabilities/servers/{id}",
-    body_params={'id' : 7, 'description' : "this is a description", "groups":[3,4]}
+    body_params={'id' : 7,'description' : "this is a description", "groups":[3,4]}
 )
 ```
+
+## FAQs
+
+**What if I don't want to verify the SSL certificate?**
+
+Error example:
+
+
+```bash
+ssl.SSLCertVerificationError: [SSL: CERTIFICATE_VERIFY_FAILED] certificate verify failed: self-signed certificate (_ssl.c:997)
+```
+
+Certificate verification can be bypassed with the `verify_ssl` option.
+
+For example, this option was added to the previous ping.py script as follows:
+
+```python
+from cyberwatch_api import Cyberwatch_Pyhelper
+
+output = Cyberwatch_Pyhelper().request(
+    method="get",
+    endpoint="/api/v3/ping",
+    verify_ssl=False
+    )
+
+print(next(output).json())
+```
```

### Comparing `cyberwatch_api-0.2.0/README.md` & `cyberwatch_api-0.3.0/README.md`

 * *Files 18% similar despite different names*

```diff
@@ -9,14 +9,15 @@
   - [Prerequisites](#prerequisites)
   - [Module installation](#module-installation)
   - [Configuration](#configuration)
   - [api.conf file location](#apiconf-file-location)
 - [Ping](#ping)
 - [Examples](#examples)
 - [Usage](#usage)
+- [FAQs](#faqs)
 
 <!-- END doctoc generated TOC please keep comment here to allow auto update -->
 ## Installation
 
 ### Prerequisites
 - [ ] [Python 3](https://www.python.org/)
 - [ ] Python [PIP](https://pypi.org/project/pip/)
@@ -116,10 +117,37 @@
     params={'id' : 7}
 )
 ```
 ```python
 output = Cyberwatch_Pyhelper().request(
     method="put",
     endpoint="/api/v3/vulnerabilities/servers/{id}",
-    body_params={'id' : 7, 'description' : "this is a description", "groups":[3,4]}
+    body_params={'id' : 7,'description' : "this is a description", "groups":[3,4]}
 )
 ```
+
+## FAQs
+
+**What if I don't want to verify the SSL certificate?**
+
+Error example:
+
+
+```bash
+ssl.SSLCertVerificationError: [SSL: CERTIFICATE_VERIFY_FAILED] certificate verify failed: self-signed certificate (_ssl.c:997)
+```
+
+Certificate verification can be bypassed with the `verify_ssl` option.
+
+For example, this option was added to the previous ping.py script as follows:
+
+```python
+from cyberwatch_api import Cyberwatch_Pyhelper
+
+output = Cyberwatch_Pyhelper().request(
+    method="get",
+    endpoint="/api/v3/ping",
+    verify_ssl=False
+    )
+
+print(next(output).json())
+```
```

### Comparing `cyberwatch_api-0.2.0/cyberwatch_api.egg-info/PKG-INFO` & `cyberwatch_api-0.3.0/cyberwatch_api.egg-info/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cyberwatch-api
-Version: 0.2.0
+Version: 0.3.0
 Summary: Python Api client for the Cyberwatch software
 Author: CyberWatch SAS
 License: MIT
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # Cyberwatch API
@@ -18,14 +18,15 @@
   - [Prerequisites](#prerequisites)
   - [Module installation](#module-installation)
   - [Configuration](#configuration)
   - [api.conf file location](#apiconf-file-location)
 - [Ping](#ping)
 - [Examples](#examples)
 - [Usage](#usage)
+- [FAQs](#faqs)
 
 <!-- END doctoc generated TOC please keep comment here to allow auto update -->
 ## Installation
 
 ### Prerequisites
 - [ ] [Python 3](https://www.python.org/)
 - [ ] Python [PIP](https://pypi.org/project/pip/)
@@ -125,10 +126,37 @@
     params={'id' : 7}
 )
 ```
 ```python
 output = Cyberwatch_Pyhelper().request(
     method="put",
     endpoint="/api/v3/vulnerabilities/servers/{id}",
-    body_params={'id' : 7, 'description' : "this is a description", "groups":[3,4]}
+    body_params={'id' : 7,'description' : "this is a description", "groups":[3,4]}
 )
 ```
+
+## FAQs
+
+**What if I don't want to verify the SSL certificate?**
+
+Error example:
+
+
+```bash
+ssl.SSLCertVerificationError: [SSL: CERTIFICATE_VERIFY_FAILED] certificate verify failed: self-signed certificate (_ssl.c:997)
+```
+
+Certificate verification can be bypassed with the `verify_ssl` option.
+
+For example, this option was added to the previous ping.py script as follows:
+
+```python
+from cyberwatch_api import Cyberwatch_Pyhelper
+
+output = Cyberwatch_Pyhelper().request(
+    method="get",
+    endpoint="/api/v3/ping",
+    verify_ssl=False
+    )
+
+print(next(output).json())
+```
```

### Comparing `cyberwatch_api-0.2.0/cyberwatch_api.py` & `cyberwatch_api-0.3.0/cyberwatch_api.py`

 * *Files 14% similar despite different names*

```diff
@@ -38,25 +38,27 @@
     @property
     def api_url(self) -> str:
         return self.__api_url
 
     def clear_endpoint(f):
         """
         Decorator that takes the endpoint that was given by the API user,
-        and replaces the {id} by the id parameter that was given inside the params or body params dict
+        and replaces the {parameter} by the one that was given inside the params or body params dict
         """
         def wrapper(*args, **kwargs):
             endpoint = kwargs.get("endpoint")
-            if "{id}" in endpoint:
-                params_id = (kwargs.get("params",{}).get("id") or kwargs.get("body_params",{}).get("id"))
-                for key in kwargs:
-                    if type(kwargs[key]) == dict :
-                        del(kwargs[key]["id"])
-                endpoint = endpoint.replace("{id}", str(params_id))
-                kwargs.update({"endpoint": endpoint})
+            parameters = [parameter.split("}")[0] for parameter in endpoint.split("{")[1:]]
+
+            for parameter in parameters:
+                parameter_value = (kwargs.get("params",{}).get(parameter) or kwargs.get("body_params",{}).get(parameter))
+                endpoint = endpoint.replace("{" + parameter + "}", str(parameter_value))
+                # Deleting the 'parameter' from the kwargs arguments if it exists
+                [kwargs[key].pop(parameter, "") for key in kwargs if type(kwargs[key]) == dict]
+
+            kwargs.update({"endpoint": endpoint})
             return f(*args, **kwargs)
         return wrapper
 
     @api_url.setter
     def api_url(self, value: str):
         """
         This setter will search for a parameter given during the initialization of the class.
@@ -108,89 +110,46 @@
         elif self.path_to_conf is not None:
             self.__api_secret = self.CONF.get("cyberwatch", "secret_key")
         else:
             self.__api_secret = os.getenv("api_secret")
         if self.__api_secret is None:
             raise Exception("api_secret not found")
 
-    @property
-    def method(self) -> str:
-        return self.__method
-
-    @method.setter
-    def method(self, value: str):
-        if isinstance(value, str):
-            self.__method = str(value).upper()
-        else:
-            raise Exception("The type of method parameter should be a str")
-
-    @property
-    def url(self) -> str:
-        return self.__url
-
-    @url.setter
-    def url(self, value: str):
-        if isinstance(value, str):
-            self.__url = self.api_url + value
-        else:
-            raise Exception("The type of endpoint parameter should be str")
-
-    @property
-    def timeout(self) -> int:
-        return self.__timeout
-
-    @timeout.setter
-    def timeout(self, value: int):
-        if isinstance(value, int):
-            self.__timeout = value
-        else:
-            raise Exception("The type of timeout parameter should be int")
-
     def __basic_auth(self) -> requests.auth.HTTPBasicAuth:
         """
         Private method returning a BasicAuth
         """
         return requests.auth.HTTPBasicAuth(self.api_key, self.api_secret)
-
+    
     @clear_endpoint
     def request(self, **kwargs) -> Generator[requests.models.Response, None, None]:
         """
         Only accessible method, handles every step of the API call
         """
-        self.method = kwargs.get("method")
-        self.url = kwargs.get("endpoint")
-        self.timeout = kwargs.get("timeout") or 10
-        params = kwargs.get("params") or {}
-        body_params = kwargs.get("body_params") or {}
+        if not isinstance(kwargs.get("method"), str): raise Exception("The type of endpoint parameter should be str")
+        if kwargs.get("timeout") and not isinstance(kwargs.get("timeout"), int): raise Exception("The type of timeout parameter should be int")
 
+        method = str(kwargs.get("method")).upper()
+        timeout = kwargs.get("timeout") or 10
+        params = kwargs.get("params") or {}
+        body_params = json.dumps(kwargs.get("body_params")) if kwargs.get("body_params") else {}
         headers = {'Content-type': 'application/json'}
+        verify_ssl = kwargs.get("verify_ssl")
+        url = self.api_url + kwargs.get("endpoint")
 
-        if body_params is not None:
-            body_params = json.dumps(body_params)
-
-        self.verify_ssl = kwargs.get("verify_ssl")
-
-        response = requests.request(
-            method=self.method,
-            url=self.url,
-            headers=headers,
-            auth=self.__basic_auth(),
-            params=params,
-            data=body_params,
-            timeout=self.timeout,
-            verify=self.verify_ssl
-        )
-        yield response
-        while "next" in response.links:
+        while url:
             response = requests.request(
-                method=self.method,
-                url=response.links["next"]["url"],
+                method=method,
+                url=url,
+                headers=headers,
                 auth=self.__basic_auth(),
                 params=params,
-                timeout=self.timeout,
-                verify=self.verify_ssl
+                data=body_params,
+                timeout=timeout,
+                verify=verify_ssl
             )
+            url = response.links["next"]["url"] if "next" in response.links else None
             yield response
 
 
 if __name__ == "__main__":
     Cyberwatch_Pyhelper()
```

