# Comparing `tmp/petkitaio-0.1.4.tar.gz` & `tmp/petkitaio-0.1.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "petkitaio-0.1.4.tar", last modified: Wed Jun 21 21:30:05 2023, max compression
+gzip compressed data, was "petkitaio-0.1.5.tar", last modified: Mon Jun 26 20:30:38 2023, max compression
```

## Comparing `petkitaio-0.1.4.tar` & `petkitaio-0.1.5.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 robertdrinovac   (501) staff       (20)        0 2023-06-21 21:30:05.510163 petkitaio-0.1.4/
--rw-rw-r--   0 robertdrinovac   (501) staff       (20)     1067 2023-06-21 21:26:42.000000 petkitaio-0.1.4/LICENSE
--rw-r--r--   0 robertdrinovac   (501) staff       (20)     5891 2023-06-21 21:30:05.510517 petkitaio-0.1.4/PKG-INFO
--rw-rw-r--   0 robertdrinovac   (501) staff       (20)     4300 2023-06-21 21:26:42.000000 petkitaio-0.1.4/README.md
-drwxr-xr-x   0 robertdrinovac   (501) staff       (20)        0 2023-06-21 21:30:05.507165 petkitaio-0.1.4/petkitaio/
--rw-rw-r--   0 robertdrinovac   (501) staff       (20)     1902 2023-06-21 21:26:42.000000 petkitaio-0.1.4/petkitaio/__init__.py
--rw-rw-r--   0 robertdrinovac   (501) staff       (20)    10226 2023-06-21 21:26:42.000000 petkitaio-0.1.4/petkitaio/constants.py
--rw-rw-r--   0 robertdrinovac   (501) staff       (20)      835 2023-06-21 21:26:42.000000 petkitaio-0.1.4/petkitaio/exceptions.py
--rw-rw-r--   0 robertdrinovac   (501) staff       (20)     1392 2023-06-21 21:26:42.000000 petkitaio-0.1.4/petkitaio/model.py
--rw-rw-r--   0 robertdrinovac   (501) staff       (20)    42583 2023-06-21 21:26:42.000000 petkitaio-0.1.4/petkitaio/petkit_client.py
--rw-rw-r--   0 robertdrinovac   (501) staff       (20)      680 2023-06-21 21:26:42.000000 petkitaio-0.1.4/petkitaio/str_enum.py
-drwxr-xr-x   0 robertdrinovac   (501) staff       (20)        0 2023-06-21 21:30:05.509665 petkitaio-0.1.4/petkitaio.egg-info/
--rw-r--r--   0 robertdrinovac   (501) staff       (20)     5891 2023-06-21 21:30:05.000000 petkitaio-0.1.4/petkitaio.egg-info/PKG-INFO
--rw-r--r--   0 robertdrinovac   (501) staff       (20)      337 2023-06-21 21:30:05.000000 petkitaio-0.1.4/petkitaio.egg-info/SOURCES.txt
--rw-r--r--   0 robertdrinovac   (501) staff       (20)        1 2023-06-21 21:30:05.000000 petkitaio-0.1.4/petkitaio.egg-info/dependency_links.txt
--rw-r--r--   0 robertdrinovac   (501) staff       (20)       28 2023-06-21 21:30:05.000000 petkitaio-0.1.4/petkitaio.egg-info/requires.txt
--rw-r--r--   0 robertdrinovac   (501) staff       (20)       10 2023-06-21 21:30:05.000000 petkitaio-0.1.4/petkitaio.egg-info/top_level.txt
--rw-rw-r--   0 robertdrinovac   (501) staff       (20)       38 2023-06-21 21:30:05.511210 petkitaio-0.1.4/setup.cfg
--rw-rw-r--   0 robertdrinovac   (501) staff       (20)     1050 2023-06-21 21:26:42.000000 petkitaio-0.1.4/setup.py
+drwxr-xr-x   0 robertdrinovac   (501) staff       (20)        0 2023-06-26 20:30:38.385862 petkitaio-0.1.5/
+-rw-rw-r--   0 robertdrinovac   (501) staff       (20)     1067 2023-06-26 20:28:52.000000 petkitaio-0.1.5/LICENSE
+-rw-r--r--   0 robertdrinovac   (501) staff       (20)     5891 2023-06-26 20:30:38.386092 petkitaio-0.1.5/PKG-INFO
+-rw-rw-r--   0 robertdrinovac   (501) staff       (20)     4300 2023-06-26 20:28:52.000000 petkitaio-0.1.5/README.md
+drwxr-xr-x   0 robertdrinovac   (501) staff       (20)        0 2023-06-26 20:30:38.383650 petkitaio-0.1.5/petkitaio/
+-rw-rw-r--   0 robertdrinovac   (501) staff       (20)     1868 2023-06-26 20:28:52.000000 petkitaio-0.1.5/petkitaio/__init__.py
+-rw-rw-r--   0 robertdrinovac   (501) staff       (20)    10226 2023-06-26 20:28:52.000000 petkitaio-0.1.5/petkitaio/constants.py
+-rw-rw-r--   0 robertdrinovac   (501) staff       (20)      835 2023-06-26 20:28:52.000000 petkitaio-0.1.5/petkitaio/exceptions.py
+-rw-rw-r--   0 robertdrinovac   (501) staff       (20)     1392 2023-06-26 20:28:52.000000 petkitaio-0.1.5/petkitaio/model.py
+-rw-rw-r--   0 robertdrinovac   (501) staff       (20)    41909 2023-06-26 20:28:52.000000 petkitaio-0.1.5/petkitaio/petkit_client.py
+-rw-rw-r--   0 robertdrinovac   (501) staff       (20)      680 2023-06-26 20:28:52.000000 petkitaio-0.1.5/petkitaio/str_enum.py
+drwxr-xr-x   0 robertdrinovac   (501) staff       (20)        0 2023-06-26 20:30:38.385582 petkitaio-0.1.5/petkitaio.egg-info/
+-rw-r--r--   0 robertdrinovac   (501) staff       (20)     5891 2023-06-26 20:30:38.000000 petkitaio-0.1.5/petkitaio.egg-info/PKG-INFO
+-rw-r--r--   0 robertdrinovac   (501) staff       (20)      337 2023-06-26 20:30:38.000000 petkitaio-0.1.5/petkitaio.egg-info/SOURCES.txt
+-rw-r--r--   0 robertdrinovac   (501) staff       (20)        1 2023-06-26 20:30:38.000000 petkitaio-0.1.5/petkitaio.egg-info/dependency_links.txt
+-rw-r--r--   0 robertdrinovac   (501) staff       (20)       28 2023-06-26 20:30:38.000000 petkitaio-0.1.5/petkitaio.egg-info/requires.txt
+-rw-r--r--   0 robertdrinovac   (501) staff       (20)       10 2023-06-26 20:30:38.000000 petkitaio-0.1.5/petkitaio.egg-info/top_level.txt
+-rw-rw-r--   0 robertdrinovac   (501) staff       (20)       38 2023-06-26 20:30:38.386663 petkitaio-0.1.5/setup.cfg
+-rw-rw-r--   0 robertdrinovac   (501) staff       (20)     1050 2023-06-26 20:28:52.000000 petkitaio-0.1.5/setup.py
```

### Comparing `petkitaio-0.1.4/LICENSE` & `petkitaio-0.1.5/LICENSE`

 * *Files identical despite different names*

### Comparing `petkitaio-0.1.4/PKG-INFO` & `petkitaio-0.1.5/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: petkitaio
-Version: 0.1.4
+Version: 0.1.5
 Summary: Asynchronous Python library for PetKit's API
 Home-page: https://github.com/RobertD502/petkitaio
 Author: Robert Drinovac
 Author-email: unlisted@gmail.com
 License: UNKNOWN
 Project-URL: Bug Reports, https://github.com/RobertD502/petkitaio/issues
 Project-URL: Source, https://github.com/RobertD502/petkitaio/
```

### Comparing `petkitaio-0.1.4/README.md` & `petkitaio-0.1.5/README.md`

 * *Files identical despite different names*

### Comparing `petkitaio-0.1.4/petkitaio/__init__.py` & `petkitaio-0.1.5/petkitaio/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,9 +1,8 @@
 from .constants import (
-    ASIA_REGIONS,
     AUTH_ERROR_CODES,
     BLE_HEADER,
     BLUETOOTH_ERRORS,
     CLIENT_DICT,
     FEEDER_LIST,
     FeederSetting,
     LB_CMD_TO_KEY,
@@ -38,13 +37,13 @@
     W5_SETTINGS_COMMANDS,
 )
 from .petkit_client import (PetKitClient, LOGGER,)
 from .exceptions import (AuthError, BluetoothError, PetKitError, ServerError)
 from .model import (Feeder, LitterBox, Pet, PetKitData, Purifier, W5Fountain, )
 from .str_enum import StrEnum
 
-__all__ = ['ASIA_REGIONS', 'AuthError', 'AUTH_ERROR_CODES', 'BLE_HEADER', 'BluetoothError', 'BLUETOOTH_ERRORS', 'CLIENT_DICT', 'Feeder', 'Endpoint',
+__all__ = ['AuthError', 'AUTH_ERROR_CODES', 'BLE_HEADER', 'BluetoothError', 'BLUETOOTH_ERRORS', 'CLIENT_DICT', 'Feeder', 'Endpoint',
            'FEEDER_LIST', 'FeederSetting', 'Header', 'LB_CMD_TO_KEY', 'LB_CMD_TO_TYPE', 'LB_CMD_TO_VALUE', 'LitterBox', 'LitterBoxCommand', 'LitterBoxCommandKey',
            'LitterBoxCommandType', 'LitterBoxSetting', 'LITTER_LIST', 'LOGGER', 'Pet', 'PetKitClient', 'PetKitData', 'PetKitError', 'PetSetting', 'Purifier',
            'PurifierCommand', 'PurifierCommandKey', 'PurifierCommandType', 'PUR_CMD_TO_KEY', 'PUR_CMD_TO_TYPE', 'PUR_CMD_TO_VALUE', 'PURIFIER_LIST', 'PurifierSetting', 'Region',
            'ServerError', 'SERVER_ERROR_CODES', 'StrEnum', 'TIMEOUT', 'WATER_FOUNTAIN_LIST', 'W5Command', 'W5_COMMAND_TO_CODE', 'W5_DND_COMMANDS', 'W5Fountain', 'W5_LIGHT_BRIGHTNESS',
            'W5_LIGHT_POWER', 'W5_MODE', 'W5_SETTINGS_COMMANDS',  ]
```

### Comparing `petkitaio-0.1.4/petkitaio/constants.py` & `petkitaio-0.1.5/petkitaio/constants.py`

 * *Files identical despite different names*

### Comparing `petkitaio-0.1.4/petkitaio/exceptions.py` & `petkitaio-0.1.5/petkitaio/exceptions.py`

 * *Files identical despite different names*

### Comparing `petkitaio-0.1.4/petkitaio/model.py` & `petkitaio-0.1.5/petkitaio/model.py`

 * *Files identical despite different names*

### Comparing `petkitaio-0.1.4/petkitaio/petkit_client.py` & `petkitaio-0.1.5/petkitaio/petkit_client.py`

 * *Files 2% similar despite different names*

```diff
@@ -11,15 +11,14 @@
 import urllib.parse as urlencode
 
 from aiohttp import ClientResponse, ClientSession
 import hashlib
 from tzlocal import get_localzone_name
 
 from petkitaio.constants import (
-    ASIA_REGIONS,
     AUTH_ERROR_CODES,
     BLE_HEADER,
     BLUETOOTH_ERRORS,
     CLIENT_DICT,
     Endpoint,
     FEEDER_LIST,
     FeederSetting,
@@ -54,27 +53,26 @@
 LOGGER = logging.getLogger(__name__)
 
 
 class PetKitClient:
     """PetKit client."""
 
     def __init__(
-        self, username: str, password: str, session: ClientSession | None = None, timeout: int = TIMEOUT
+        self, username: str, password: str, session: ClientSession | None = None, asia_account: bool = False, timeout: int = TIMEOUT
     ) -> None:
         """Initialize PetKit Client.
 
         username: PetKit username/email
         password: PetKit account password
         session: aiohttp.ClientSession or None to create a new session
         """
 
         self.username: str = username
         self.password: str = password
-        self.base_login: Region = Region.US
-        self.base_url: str | None = None
+        self.base_url: Region = Region.ASIA if asia_account else Region.US
         self.server_list: list | None = None
         self._session: ClientSession = session if session else ClientSession()
         self.tz: str = get_localzone_name()
         self.timeout: int = timeout
         self.token: str | None = None
         self.token_expiration: datetime | None = None
         self.user_id: str | None = None
@@ -100,16 +98,15 @@
         }
         data = {}
         response = await self._post(url, headers, data)
         self.server_list = response['result']['list']
 
     async def login(self) -> None:
 
-        await self.get_api_server_list()
-        login_url = f'{self.base_login}{Endpoint.LOGIN}'
+        login_url = f'{self.base_url}{Endpoint.LOGIN}'
 
         headers = {
             'Accept': Header.ACCEPT,
             'Accept-Language': Header.ACCEPT_LANG,
             'Accept-Encoding': Header.ENCODING,
             'X-Api-Version': Header.API_VERSION,
             'Content-Type': Header.CONTENT_TYPE,
@@ -125,27 +122,14 @@
             'username': self.username
         }
 
         response = await self._post(login_url, headers, data)
         self.user_id = response['result']['session']['userId']
         self.token = response['result']['session']['id']
         self.token_expiration = datetime.now() + timedelta(seconds=response['result']['session']['expiresIn'])
-        account_region = response['result']['user']['account']['region']
-        # Determine base URL based on region account is from
-        for region in self.server_list:
-            if region['id'] == account_region:
-                # Need to remove trailing forward slash
-                self.base_url = region['gateway'][:-1]
-                break
-            else:
-                # Fallback base url if region server can't be found based on account region
-                if account_region in ASIA_REGIONS:
-                    self.base_url = Region.ASIA
-                else:
-                    self.base_url = Region.US
 
     async def check_token(self) -> None:
         """Check to see if there is a valid token or if token is about to expire.
         If there is no token, a new token is obtained. In addition,
         if the current token is about to expire within 60 minutes
         or has already expired, a new token is obtained.
         """
```

### Comparing `petkitaio-0.1.4/petkitaio/str_enum.py` & `petkitaio-0.1.5/petkitaio/str_enum.py`

 * *Files identical despite different names*

### Comparing `petkitaio-0.1.4/petkitaio.egg-info/PKG-INFO` & `petkitaio-0.1.5/petkitaio.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: petkitaio
-Version: 0.1.4
+Version: 0.1.5
 Summary: Asynchronous Python library for PetKit's API
 Home-page: https://github.com/RobertD502/petkitaio
 Author: Robert Drinovac
 Author-email: unlisted@gmail.com
 License: UNKNOWN
 Project-URL: Bug Reports, https://github.com/RobertD502/petkitaio/issues
 Project-URL: Source, https://github.com/RobertD502/petkitaio/
```

### Comparing `petkitaio-0.1.4/setup.py` & `petkitaio-0.1.5/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="petkitaio",
-    version="0.1.4",
+    version="0.1.5",
     author="Robert Drinovac",
     author_email="unlisted@gmail.com",
     description="Asynchronous Python library for PetKit's API",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url='https://github.com/RobertD502/petkitaio',
     keywords='petkit, eversweet 3 pro, feeder mini, d4, petkit feeder, petkit water fountain, freshelement solo, pura x, pura max, pura air',
```

