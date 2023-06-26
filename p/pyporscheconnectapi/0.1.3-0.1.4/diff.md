# Comparing `tmp/pyporscheconnectapi-0.1.3.tar.gz` & `tmp/pyporscheconnectapi-0.1.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyporscheconnectapi-0.1.3.tar", last modified: Thu Jun 15 11:35:55 2023, max compression
+gzip compressed data, was "pyporscheconnectapi-0.1.4.tar", last modified: Mon Jun 26 13:26:54 2023, max compression
```

## Comparing `pyporscheconnectapi-0.1.3.tar` & `pyporscheconnectapi-0.1.4.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 11:35:55.986906 pyporscheconnectapi-0.1.3/
--rw-r--r--   0 runner    (1001) docker     (123)     1071 2023-06-15 11:35:39.000000 pyporscheconnectapi-0.1.3/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     4930 2023-06-15 11:35:55.986906 pyporscheconnectapi-0.1.3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     4434 2023-06-15 11:35:39.000000 pyporscheconnectapi-0.1.3/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 11:35:55.986906 pyporscheconnectapi-0.1.3/pyporscheconnectapi/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-15 11:35:39.000000 pyporscheconnectapi-0.1.3/pyporscheconnectapi/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    10930 2023-06-15 11:35:39.000000 pyporscheconnectapi-0.1.3/pyporscheconnectapi/cli.py
--rw-r--r--   0 runner    (1001) docker     (123)    19856 2023-06-15 11:35:39.000000 pyporscheconnectapi-0.1.3/pyporscheconnectapi/client.py
--rw-r--r--   0 runner    (1001) docker     (123)    11848 2023-06-15 11:35:39.000000 pyporscheconnectapi-0.1.3/pyporscheconnectapi/connection.py
--rw-r--r--   0 runner    (1001) docker     (123)     1539 2023-06-15 11:35:39.000000 pyporscheconnectapi-0.1.3/pyporscheconnectapi/exceptions.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 11:35:55.986906 pyporscheconnectapi-0.1.3/pyporscheconnectapi.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     4930 2023-06-15 11:35:55.000000 pyporscheconnectapi-0.1.3/pyporscheconnectapi.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      453 2023-06-15 11:35:55.000000 pyporscheconnectapi-0.1.3/pyporscheconnectapi.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-15 11:35:55.000000 pyporscheconnectapi-0.1.3/pyporscheconnectapi.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       59 2023-06-15 11:35:55.000000 pyporscheconnectapi-0.1.3/pyporscheconnectapi.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)       25 2023-06-15 11:35:55.000000 pyporscheconnectapi-0.1.3/pyporscheconnectapi.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       20 2023-06-15 11:35:55.000000 pyporscheconnectapi-0.1.3/pyporscheconnectapi.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      269 2023-06-15 11:35:55.986906 pyporscheconnectapi-0.1.3/setup.cfg
--rwxr-xr-x   0 runner    (1001) docker     (123)      951 2023-06-15 11:35:39.000000 pyporscheconnectapi-0.1.3/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 13:26:54.652121 pyporscheconnectapi-0.1.4/
+-rw-r--r--   0 runner    (1001) docker     (123)     1071 2023-06-26 13:26:44.000000 pyporscheconnectapi-0.1.4/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     4930 2023-06-26 13:26:54.652121 pyporscheconnectapi-0.1.4/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     4434 2023-06-26 13:26:44.000000 pyporscheconnectapi-0.1.4/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 13:26:54.652121 pyporscheconnectapi-0.1.4/pyporscheconnectapi/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-26 13:26:44.000000 pyporscheconnectapi-0.1.4/pyporscheconnectapi/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10930 2023-06-26 13:26:44.000000 pyporscheconnectapi-0.1.4/pyporscheconnectapi/cli.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19908 2023-06-26 13:26:44.000000 pyporscheconnectapi-0.1.4/pyporscheconnectapi/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11903 2023-06-26 13:26:44.000000 pyporscheconnectapi-0.1.4/pyporscheconnectapi/connection.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1539 2023-06-26 13:26:44.000000 pyporscheconnectapi-0.1.4/pyporscheconnectapi/exceptions.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 13:26:54.652121 pyporscheconnectapi-0.1.4/pyporscheconnectapi.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     4930 2023-06-26 13:26:54.000000 pyporscheconnectapi-0.1.4/pyporscheconnectapi.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      453 2023-06-26 13:26:54.000000 pyporscheconnectapi-0.1.4/pyporscheconnectapi.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-26 13:26:54.000000 pyporscheconnectapi-0.1.4/pyporscheconnectapi.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       59 2023-06-26 13:26:54.000000 pyporscheconnectapi-0.1.4/pyporscheconnectapi.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       25 2023-06-26 13:26:54.000000 pyporscheconnectapi-0.1.4/pyporscheconnectapi.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       20 2023-06-26 13:26:54.000000 pyporscheconnectapi-0.1.4/pyporscheconnectapi.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      269 2023-06-26 13:26:54.652121 pyporscheconnectapi-0.1.4/setup.cfg
+-rwxr-xr-x   0 runner    (1001) docker     (123)      951 2023-06-26 13:26:44.000000 pyporscheconnectapi-0.1.4/setup.py
```

### Comparing `pyporscheconnectapi-0.1.3/LICENSE` & `pyporscheconnectapi-0.1.4/LICENSE`

 * *Files identical despite different names*

### Comparing `pyporscheconnectapi-0.1.3/PKG-INFO` & `pyporscheconnectapi-0.1.4/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyporscheconnectapi
-Version: 0.1.3
+Version: 0.1.4
 Summary: Python library and CLI for communicating with Porsche Connect API.
 Home-page: https://github.com/cjne/pyporscheconnectapi
 Author: Johan Isaksson
 Author-email: johan@generatorhallen.se
 License: MIT
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python
```

### Comparing `pyporscheconnectapi-0.1.3/README.md` & `pyporscheconnectapi-0.1.4/README.md`

 * *Files identical despite different names*

### Comparing `pyporscheconnectapi-0.1.3/pyporscheconnectapi/cli.py` & `pyporscheconnectapi-0.1.4/pyporscheconnectapi/cli.py`

 * *Files identical despite different names*

### Comparing `pyporscheconnectapi-0.1.3/pyporscheconnectapi/client.py` & `pyporscheconnectapi-0.1.4/pyporscheconnectapi/client.py`

 * *Files 2% similar despite different names*

```diff
@@ -140,15 +140,15 @@
         progressResult = await self._connection.post(
             f"https://api.porsche.com/e-mobility/{self.locale_str}/{model}/{vin}/timer",
             json=timer,
         )
         if not waitForConfirmation:
             return progressResult
         result = await self._spinner(
-            f"https://api.porsche.com/e-mobility/{self.locale_str}/{model}/{vin}/action-status/{progressResult['actionId']}"
+            f"https://api.porsche.com/e-mobility/{self.locale_str}/{model}/{vin}/action-status/{progressResult['actionId']}?hasDX1=false"
         )
         return result
 
     async def _updateChargingProfile(
         self,
         vin,
         model=None,
@@ -162,15 +162,15 @@
         progressResult = await self._connection.put(
             f"https://api.porsche.com/e-mobility/{self.locale_str}/{model}/{vin}/profile",
             json=profile,
         )
         if not waitForConfirmation:
             return progressResult
         result = await self._spinner(
-            f"https://api.porsche.com/e-mobility/{self.locale_str}/{model}/{vin}/action-status/{progressResult['actionId']}"
+            f"https://api.porsche.com/e-mobility/{self.locale_str}/{model}/{vin}/action-status/{progressResult['actionId']}?hasDX1=false"
         )
         return result
 
     async def _updateTimer(
         self,
         vin,
         timer,
@@ -186,15 +186,15 @@
         progressResult = await self._connection.put(
             f"https://api.porsche.com/e-mobility/{self.locale_str}/{model}/{vin}/timer",
             json=timer,
         )
         if not waitForConfirmation:
             return progressResult
         result = await self._spinner(
-            f"https://api.porsche.com/e-mobility/{self.locale_str}/{model}/{vin}/action-status/{progressResult['actionId']}"
+            f"https://api.porsche.com/e-mobility/{self.locale_str}/{model}/{vin}/action-status/{progressResult['actionId']}?hasDX1=false"
         )
         return result
 
     async def _deleteTimer(
         self, vin, timerID="1", model=None, waitForConfirmation=True
     ):
         if model is None:
@@ -203,15 +203,15 @@
         """Delete existing charge & climate timer"""
         progressResult = await self._connection.delete(
             f"https://api.porsche.com/e-mobility/{self.locale_str}/{model}/{vin}/timer/{timerID}"
         )
         if not waitForConfirmation:
             return progressResult
         result = await self._spinner(
-            f"https://api.porsche.com/e-mobility/{self.locale_str}/{model}/{vin}/action-status/{progressResult['actionId']}"
+            f"https://api.porsche.com/e-mobility/{self.locale_str}/{model}/{vin}/action-status/{progressResult['actionId']}?hasDX1=false"
         )
         return result
 
     def _formatTimer(self, active, charge_settings, climate, time_date):
         """Format combined payload for charge & climate timer"""
         payload = {"active": active, "climatised": climate}
         payload.update(charge_settings)
```

### Comparing `pyporscheconnectapi-0.1.3/pyporscheconnectapi/connection.py` & `pyporscheconnectapi-0.1.4/pyporscheconnectapi/connection.py`

 * *Files 1% similar despite different names*

```diff
@@ -111,15 +111,15 @@
         start_login_url = f"https://{AUTHORIZATION_SERVER}/authorize?response_type=code&client_id={CLIENT_ID}&code_challenge_method=S256&redirect_uri={REDIRECT_URI}&ui_locales=de-DE&audience={AUDIENCE}&scope=openid"
         async with self.websession.get(start_login_url, allow_redirects=False) as resp:
             location = resp.headers["Location"]
             params = urllib.parse.parse_qs(urllib.parse.urlparse(location).query)
             _LOGGER.debug(params)
             have_code = params.get('code', None)
             if have_code is not None:
-                _LOGGER("We already have a code in session, skip login")
+                _LOGGER.debug("We already have a code in session, skip login")
                 self.auth_state['code'] = have_code
                 return
             self.auth_state["state"] = params["state"][0]
             self.auth_state["client"] = params["client"][0]
         _LOGGER.debug(self.auth_state)
 
 
@@ -142,15 +142,15 @@
         auth_url = f"https://{AUTHORIZATION_SERVER}/usernamepassword/login"
         verify_body = {} 
         async with self.websession.post(auth_url, headers={"Content-Type": "application/x-www-form-urlencoded"}, data=auth_body, max_redirects=30) as resp:
             # In case of wrong credentials there is a state param in the redirect url
 
             if resp.status == 401:
                 message = await resp.json()
-                raise WrongCredentials(message['message'])
+                raise WrongCredentials(message.get('message', message.get('description', 'Unknown error')))
 
             html_body = await resp.text()
 
             _LOGGER.debug(resp.status)
             _LOGGER.debug(html_body)
 
             soup = BeautifulSoup(html_body,features="html.parser")
```

### Comparing `pyporscheconnectapi-0.1.3/pyporscheconnectapi/exceptions.py` & `pyporscheconnectapi-0.1.4/pyporscheconnectapi/exceptions.py`

 * *Files identical despite different names*

### Comparing `pyporscheconnectapi-0.1.3/pyporscheconnectapi.egg-info/PKG-INFO` & `pyporscheconnectapi-0.1.4/pyporscheconnectapi.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyporscheconnectapi
-Version: 0.1.3
+Version: 0.1.4
 Summary: Python library and CLI for communicating with Porsche Connect API.
 Home-page: https://github.com/cjne/pyporscheconnectapi
 Author: Johan Isaksson
 Author-email: johan@generatorhallen.se
 License: MIT
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python
```

### Comparing `pyporscheconnectapi-0.1.3/setup.py` & `pyporscheconnectapi-0.1.4/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 #!/usr/bin/env python
 from setuptools import setup
 
 
 setup(
     name="pyporscheconnectapi",
-    version="0.1.3",
+    version="0.1.4",
     author="Johan Isaksson",
     author_email="johan@generatorhallen.se",
     description="Python library and CLI for communicating with Porsche Connect API.",
     long_description=open("README.md", 'r').read(),
     long_description_content_type='text/markdown',
     include_package_data=True,
     url="https://github.com/cjne/pyporscheconnectapi",
```

