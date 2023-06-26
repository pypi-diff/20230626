# Comparing `tmp/proton-api-client-0.0.6.tar.gz` & `tmp/proton-api-client-0.0.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "proton-api-client-0.0.6.tar", last modified: Tue Jun 20 23:47:58 2023, max compression
+gzip compressed data, was "proton-api-client-0.0.7.tar", last modified: Mon Jun 26 19:17:44 2023, max compression
```

## Comparing `proton-api-client-0.0.6.tar` & `proton-api-client-0.0.7.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxr-xr-x   0 x         (1000) x         (1000)        0 2023-06-20 23:47:58.964952 proton-api-client-0.0.6/
--rw-r--r--   0 x         (1000) x         (1000)    35149 2023-06-19 17:50:26.000000 proton-api-client-0.0.6/LICENSE
--rw-r--r--   0 x         (1000) x         (1000)     1315 2023-06-20 23:47:58.964952 proton-api-client-0.0.6/PKG-INFO
--rw-r--r--   0 x         (1000) x         (1000)      922 2023-06-20 23:38:08.000000 proton-api-client-0.0.6/README.md
-drwxr-xr-x   0 x         (1000) x         (1000)        0 2023-06-20 23:47:58.964952 proton-api-client-0.0.6/proton/
--rw-r--r--   0 x         (1000) x         (1000)      156 2023-06-19 17:57:18.000000 proton-api-client-0.0.6/proton/__init__.py
--rw-r--r--   0 x         (1000) x         (1000)     9059 2023-06-19 18:23:32.000000 proton-api-client-0.0.6/proton/_ctsrp.py
--rw-r--r--   0 x         (1000) x         (1000)     3881 2023-06-20 20:05:33.000000 proton-api-client-0.0.6/proton/_pysrp.py
--rw-r--r--   0 x         (1000) x         (1000)     6009 2023-06-20 23:47:42.000000 proton-api-client-0.0.6/proton/client.py
--rw-r--r--   0 x         (1000) x         (1000)     2188 2023-06-20 19:43:36.000000 proton-api-client-0.0.6/proton/constants.py
--rw-r--r--   0 x         (1000) x         (1000)     2035 2023-06-20 23:47:42.000000 proton-api-client-0.0.6/proton/helpers.py
--rw-r--r--   0 x         (1000) x         (1000)     1541 2023-06-20 23:40:32.000000 proton-api-client-0.0.6/proton/login.py
-drwxr-xr-x   0 x         (1000) x         (1000)        0 2023-06-20 23:47:58.964952 proton-api-client-0.0.6/proton_api_client.egg-info/
--rw-r--r--   0 x         (1000) x         (1000)     1315 2023-06-20 23:47:58.000000 proton-api-client-0.0.6/proton_api_client.egg-info/PKG-INFO
--rw-r--r--   0 x         (1000) x         (1000)      354 2023-06-20 23:47:58.000000 proton-api-client-0.0.6/proton_api_client.egg-info/SOURCES.txt
--rw-r--r--   0 x         (1000) x         (1000)        1 2023-06-20 23:47:58.000000 proton-api-client-0.0.6/proton_api_client.egg-info/dependency_links.txt
--rw-r--r--   0 x         (1000) x         (1000)       79 2023-06-20 23:47:58.000000 proton-api-client-0.0.6/proton_api_client.egg-info/requires.txt
--rw-r--r--   0 x         (1000) x         (1000)        7 2023-06-20 23:47:58.000000 proton-api-client-0.0.6/proton_api_client.egg-info/top_level.txt
--rw-r--r--   0 x         (1000) x         (1000)       38 2023-06-20 23:47:58.964952 proton-api-client-0.0.6/setup.cfg
--rw-r--r--   0 x         (1000) x         (1000)     1857 2023-06-20 23:47:42.000000 proton-api-client-0.0.6/setup.py
+drwxr-xr-x   0 x         (1000) x         (1000)        0 2023-06-26 19:17:44.482118 proton-api-client-0.0.7/
+-rw-r--r--   0 x         (1000) x         (1000)    35149 2023-06-25 17:48:35.000000 proton-api-client-0.0.7/LICENSE
+-rw-r--r--   0 x         (1000) x         (1000)     1315 2023-06-26 19:17:44.482118 proton-api-client-0.0.7/PKG-INFO
+-rw-r--r--   0 x         (1000) x         (1000)      922 2023-06-25 17:48:35.000000 proton-api-client-0.0.7/README.md
+drwxr-xr-x   0 x         (1000) x         (1000)        0 2023-06-26 19:17:44.482118 proton-api-client-0.0.7/proton/
+-rw-r--r--   0 x         (1000) x         (1000)      156 2023-06-25 17:48:35.000000 proton-api-client-0.0.7/proton/__init__.py
+-rw-r--r--   0 x         (1000) x         (1000)     9059 2023-06-25 17:48:35.000000 proton-api-client-0.0.7/proton/_ctsrp.py
+-rw-r--r--   0 x         (1000) x         (1000)     3881 2023-06-25 17:48:35.000000 proton-api-client-0.0.7/proton/_pysrp.py
+-rw-r--r--   0 x         (1000) x         (1000)     6208 2023-06-26 19:12:55.000000 proton-api-client-0.0.7/proton/client.py
+-rw-r--r--   0 x         (1000) x         (1000)     2433 2023-06-26 19:15:08.000000 proton-api-client-0.0.7/proton/constants.py
+-rw-r--r--   0 x         (1000) x         (1000)     2035 2023-06-25 17:48:35.000000 proton-api-client-0.0.7/proton/helpers.py
+-rw-r--r--   0 x         (1000) x         (1000)     2320 2023-06-26 19:12:23.000000 proton-api-client-0.0.7/proton/login.py
+drwxr-xr-x   0 x         (1000) x         (1000)        0 2023-06-26 19:17:44.482118 proton-api-client-0.0.7/proton_api_client.egg-info/
+-rw-r--r--   0 x         (1000) x         (1000)     1315 2023-06-26 19:17:44.000000 proton-api-client-0.0.7/proton_api_client.egg-info/PKG-INFO
+-rw-r--r--   0 x         (1000) x         (1000)      354 2023-06-26 19:17:44.000000 proton-api-client-0.0.7/proton_api_client.egg-info/SOURCES.txt
+-rw-r--r--   0 x         (1000) x         (1000)        1 2023-06-26 19:17:44.000000 proton-api-client-0.0.7/proton_api_client.egg-info/dependency_links.txt
+-rw-r--r--   0 x         (1000) x         (1000)       79 2023-06-26 19:17:44.000000 proton-api-client-0.0.7/proton_api_client.egg-info/requires.txt
+-rw-r--r--   0 x         (1000) x         (1000)        7 2023-06-26 19:17:44.000000 proton-api-client-0.0.7/proton_api_client.egg-info/top_level.txt
+-rw-r--r--   0 x         (1000) x         (1000)       38 2023-06-26 19:17:44.482118 proton-api-client-0.0.7/setup.cfg
+-rw-r--r--   0 x         (1000) x         (1000)     1857 2023-06-26 19:15:08.000000 proton-api-client-0.0.7/setup.py
```

### Comparing `proton-api-client-0.0.6/LICENSE` & `proton-api-client-0.0.7/LICENSE`

 * *Files identical despite different names*

### Comparing `proton-api-client-0.0.6/PKG-INFO` & `proton-api-client-0.0.7/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: proton-api-client
-Version: 0.0.6
+Version: 0.0.7
 Summary: Proton Mail API
 Home-page: https://github.com/trevorhobenshield/proton-api-client
 Author: Trevor Hobenshield
 Author-email: trevorhobenshield@gmail.com
 Keywords: proton api client async search automation bot scrape mail email
 Requires-Python: >=3.10.10
 Description-Content-Type: text/markdown
```

### Comparing `proton-api-client-0.0.6/README.md` & `proton-api-client-0.0.7/README.md`

 * *Files identical despite different names*

### Comparing `proton-api-client-0.0.6/proton/_ctsrp.py` & `proton-api-client-0.0.7/proton/_ctsrp.py`

 * *Files identical despite different names*

### Comparing `proton-api-client-0.0.6/proton/_pysrp.py` & `proton-api-client-0.0.7/proton/_pysrp.py`

 * *Files identical despite different names*

### Comparing `proton-api-client-0.0.6/proton/client.py` & `proton-api-client-0.0.7/proton/client.py`

 * *Files 2% similar despite different names*

```diff
@@ -92,15 +92,15 @@
     def decrypt_conversation(self, conversation_id: dict) -> dict:
         conversation = self._get(self.api, f'mail/v4/conversations/{conversation_id}').json()
         messages = filter(None, (msg.get('Body') for msg in conversation.get('Messages', [])))
         return {'id': conversation_id, 'data': [self.gpg_decrypt(data) for data in messages]}
 
     def info(self) -> dict:
         headers = dict(self.client.headers) | {'x-pm-appversion': PM_APP_VERSION_ACCOUNT}
-        return self._get(self.account_api, 'core/v4/auth/info', headers=headers).json()
+        return self._post(self.account_api, 'core/v4/auth/info', headers=headers).json()
 
     def calendar_directory(self) -> dict:
         return self._get(self.api, 'calendar/v1/directory', params={'Type': 2}).json()
 
     def revoke_all_sessions(self) -> dict:
         return self._get(self.account_api, 'auth/v4/sessions').json()
 
@@ -137,14 +137,18 @@
     def gpg_decrypt(self, data: str, passphrase: str = None) -> str:
         return self.gpg.decrypt(data, passphrase=passphrase or self.gpg_passphrase).data.decode()
 
     def _get(self, base: str, endpoint: str, **kwargs) -> Response:
         self.client.cookies.delete('Session-Id', domain='.protonmail.ch')
         return self.client.get(f'{base}/{endpoint}', **kwargs)
 
+    def _post(self, base, endpoint, **kwargs) -> Response:
+        self.client.cookies.delete('Session-Id', domain='.protonmail.ch')
+        return self.client.post(f'{base}/{endpoint}', **kwargs)
+
     def __gpg_clear(self) -> list[dict]:
         """ Delete all GPG keys """
         fingerprints = [x['fingerprint'] for x in self.gpg.list_keys()]
         options = ['--delete-secret-keys', '--delete-keys']
         res = []
         for opt in options:
             cmd = f'gpg --yes --batch {opt} {" ".join(fingerprints)}'
```

### Comparing `proton-api-client-0.0.6/proton/constants.py` & `proton-api-client-0.0.7/proton/constants.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,24 +1,24 @@
 VERSION = "0.7.1"
-PM_APP_VERSION_MAIL = 'web-mail@5.0.23.1'
+PM_APP_VERSION_MAIL = 'web-mail@5.0.23.1'  # do not use. CAPTCHA may be triggered?
 PM_APP_VERSION_ACCOUNT = 'web-account@5.0.35.2'
 PM_API_VERSION = '4'
 SRP_LEN_BYTES = 256
 SALT_LEN_BYTES = 10
 DEFAULT_TIMEOUT = (3.05, 27)
 
 DEFAULT_HEADERS = {
     'authority': 'account.proton.me',
     'accept': 'application/vnd.protonmail.v1+json',
     'accept-language': 'en-GB,en;q=0.9',
     'content-type': 'application/json',
     'origin': 'https://account.proton.me',
     'referer': 'https://account.proton.me',
-    'user-agent': 'Mozilla/5.0 (X11; Linux x86_64; rv:109.0) Gecko/20100101 Firefox/113.0',
-    'x-pm-appversion': PM_APP_VERSION_MAIL,
+    'user-agent': 'Ubuntu_20.04',  # do not modify. CAPTCHA may be triggered?
+    'x-pm-appversion': 'Other',  # do not modify. CAPTCHA may be triggered?
     'x-pm-apiversion': PM_API_VERSION,
 }
 
 DNS_HOSTS = [
     "https://dns11.quad9.net/dns-query",
     "https://dns.google/dns-query"
 ]
@@ -59,7 +59,18 @@
 kSIgcBRE3WuXC4oj5a2/U3oASExGDW4DAQgHwmEEGBYIABMFAlwBy4MJEDUF
 hcTpUY8mAhsMAAD/XQD8DxNI6E78meodQI+wLsrKLeHn32iLvUqJbVDhfWSU
 WO4BAMcm1u02t4VKw++ttECPt+HUgPUq5pqQWe5Q2cW4TMsE
 =Y4Mw
 -----END PGP PUBLIC KEY BLOCK-----"""
 
 SRP_MOD_KEY_FINGERPRINT = "248097092b458509c508dac0350585c4e9518f26"
+
+BLACK = '\x1b[30m'
+RED = '\x1b[31m'
+GREEN = '\x1b[32m'
+YELLOW = '\x1b[33m'
+BLUE = '\x1b[34m'
+MAGENTA = '\x1b[35m'
+CYAN = '\x1b[36m'
+WHITE = '\x1b[37m'
+BOLD = '\x1b[1m'
+RESET = '\x1b[0m'
```

### Comparing `proton-api-client-0.0.6/proton/helpers.py` & `proton-api-client-0.0.7/proton/helpers.py`

 * *Files identical despite different names*

### Comparing `proton-api-client-0.0.6/proton_api_client.egg-info/PKG-INFO` & `proton-api-client-0.0.7/proton_api_client.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: proton-api-client
-Version: 0.0.6
+Version: 0.0.7
 Summary: Proton Mail API
 Home-page: https://github.com/trevorhobenshield/proton-api-client
 Author: Trevor Hobenshield
 Author-email: trevorhobenshield@gmail.com
 Keywords: proton api client async search automation bot scrape mail email
 Requires-Python: >=3.10.10
 Description-Content-Type: text/markdown
```

### Comparing `proton-api-client-0.0.6/setup.py` & `proton-api-client-0.0.7/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -12,15 +12,15 @@
     'tqdm',
     'uvloop',
     'nest_asyncio',
 ]
 
 setup(
     name='proton-api-client',
-    version='0.0.6',
+    version='0.0.7',
     python_requires='>=3.10.10',
     description='Proton Mail API',
     long_description=dedent('''
     
     ### Proton Mail API
     
     #### Examples
```

