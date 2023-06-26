# Comparing `tmp/twitter-api-client-0.9.8.tar.gz` & `tmp/twitter-api-client-0.9.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "twitter-api-client-0.9.8.tar", last modified: Mon Jun 19 16:50:21 2023, max compression
+gzip compressed data, was "twitter-api-client-0.9.9.tar", last modified: Sat Jun 24 21:37:45 2023, max compression
```

## Comparing `twitter-api-client-0.9.8.tar` & `twitter-api-client-0.9.9.tar`

### file list

```diff
@@ -1,19 +1,20 @@
-drwxr-xr-x   0 x         (1000) x         (1000)        0 2023-06-19 16:50:21.741431 twitter-api-client-0.9.8/
--rw-r--r--   0 x         (1000) x         (1000)     1075 2023-06-16 21:34:23.000000 twitter-api-client-0.9.8/LICENSE
--rw-r--r--   0 x         (1000) x         (1000)    12136 2023-06-19 16:50:21.741431 twitter-api-client-0.9.8/PKG-INFO
--rw-r--r--   0 x         (1000) x         (1000)       38 2023-06-19 16:50:21.741431 twitter-api-client-0.9.8/setup.cfg
--rw-r--r--   0 x         (1000) x         (1000)    14177 2023-06-19 16:48:37.000000 twitter-api-client-0.9.8/setup.py
-drwxr-xr-x   0 x         (1000) x         (1000)        0 2023-06-19 16:50:21.741431 twitter-api-client-0.9.8/twitter/
--rw-r--r--   0 x         (1000) x         (1000)        0 2023-06-16 21:34:23.000000 twitter-api-client-0.9.8/twitter/__init__.py
--rw-r--r--   0 x         (1000) x         (1000)    31300 2023-06-19 16:46:01.000000 twitter-api-client-0.9.8/twitter/account.py
--rw-r--r--   0 x         (1000) x         (1000)    30178 2023-06-18 18:29:35.000000 twitter-api-client-0.9.8/twitter/constants.py
--rw-r--r--   0 x         (1000) x         (1000)     7418 2023-06-16 21:34:23.000000 twitter-api-client-0.9.8/twitter/login.py
--rw-r--r--   0 x         (1000) x         (1000)    34250 2023-06-16 21:34:23.000000 twitter-api-client-0.9.8/twitter/scraper.py
--rw-r--r--   0 x         (1000) x         (1000)     6874 2023-06-16 21:34:23.000000 twitter-api-client-0.9.8/twitter/search.py
--rw-r--r--   0 x         (1000) x         (1000)    10178 2023-06-19 15:54:08.000000 twitter-api-client-0.9.8/twitter/util.py
-drwxr-xr-x   0 x         (1000) x         (1000)        0 2023-06-19 16:50:21.741431 twitter-api-client-0.9.8/twitter_api_client.egg-info/
--rw-r--r--   0 x         (1000) x         (1000)    12136 2023-06-19 16:50:21.000000 twitter-api-client-0.9.8/twitter_api_client.egg-info/PKG-INFO
--rw-r--r--   0 x         (1000) x         (1000)      355 2023-06-19 16:50:21.000000 twitter-api-client-0.9.8/twitter_api_client.egg-info/SOURCES.txt
--rw-r--r--   0 x         (1000) x         (1000)        1 2023-06-19 16:50:21.000000 twitter-api-client-0.9.8/twitter_api_client.egg-info/dependency_links.txt
--rw-r--r--   0 x         (1000) x         (1000)       91 2023-06-19 16:50:21.000000 twitter-api-client-0.9.8/twitter_api_client.egg-info/requires.txt
--rw-r--r--   0 x         (1000) x         (1000)        8 2023-06-19 16:50:21.000000 twitter-api-client-0.9.8/twitter_api_client.egg-info/top_level.txt
+drwxr-xr-x   0 x         (1000) x         (1000)        0 2023-06-24 21:37:45.170894 twitter-api-client-0.9.9/
+-rw-r--r--   0 x         (1000) x         (1000)     1075 2023-06-16 21:34:23.000000 twitter-api-client-0.9.9/LICENSE
+-rw-r--r--   0 x         (1000) x         (1000)    12136 2023-06-24 21:37:45.170894 twitter-api-client-0.9.9/PKG-INFO
+-rw-r--r--   0 x         (1000) x         (1000)       38 2023-06-24 21:37:45.170894 twitter-api-client-0.9.9/setup.cfg
+-rw-r--r--   0 x         (1000) x         (1000)    14177 2023-06-24 21:36:42.000000 twitter-api-client-0.9.9/setup.py
+drwxr-xr-x   0 x         (1000) x         (1000)        0 2023-06-24 21:37:45.170894 twitter-api-client-0.9.9/twitter/
+-rw-r--r--   0 x         (1000) x         (1000)        0 2023-06-16 21:34:23.000000 twitter-api-client-0.9.9/twitter/__init__.py
+-rw-r--r--   0 x         (1000) x         (1000)    31517 2023-06-24 21:27:21.000000 twitter-api-client-0.9.9/twitter/account.py
+-rw-r--r--   0 x         (1000) x         (1000)    30178 2023-06-18 18:29:35.000000 twitter-api-client-0.9.9/twitter/constants.py
+-rw-r--r--   0 x         (1000) x         (1000)     7418 2023-06-16 21:34:23.000000 twitter-api-client-0.9.9/twitter/login.py
+-rw-r--r--   0 x         (1000) x         (1000)    34250 2023-06-16 21:34:23.000000 twitter-api-client-0.9.9/twitter/scraper.py
+-rw-r--r--   0 x         (1000) x         (1000)     6874 2023-06-21 19:21:59.000000 twitter-api-client-0.9.9/twitter/search.py
+-rw-r--r--   0 x         (1000) x         (1000)     6651 2023-06-21 18:57:18.000000 twitter-api-client-0.9.9/twitter/search2.py
+-rw-r--r--   0 x         (1000) x         (1000)    11797 2023-06-24 21:36:24.000000 twitter-api-client-0.9.9/twitter/util.py
+drwxr-xr-x   0 x         (1000) x         (1000)        0 2023-06-24 21:37:45.170894 twitter-api-client-0.9.9/twitter_api_client.egg-info/
+-rw-r--r--   0 x         (1000) x         (1000)    12136 2023-06-24 21:37:45.000000 twitter-api-client-0.9.9/twitter_api_client.egg-info/PKG-INFO
+-rw-r--r--   0 x         (1000) x         (1000)      374 2023-06-24 21:37:45.000000 twitter-api-client-0.9.9/twitter_api_client.egg-info/SOURCES.txt
+-rw-r--r--   0 x         (1000) x         (1000)        1 2023-06-24 21:37:45.000000 twitter-api-client-0.9.9/twitter_api_client.egg-info/dependency_links.txt
+-rw-r--r--   0 x         (1000) x         (1000)       91 2023-06-24 21:37:45.000000 twitter-api-client-0.9.9/twitter_api_client.egg-info/requires.txt
+-rw-r--r--   0 x         (1000) x         (1000)        8 2023-06-24 21:37:45.000000 twitter-api-client-0.9.9/twitter_api_client.egg-info/top_level.txt
```

### Comparing `twitter-api-client-0.9.8/LICENSE` & `twitter-api-client-0.9.9/LICENSE`

 * *Files identical despite different names*

### Comparing `twitter-api-client-0.9.8/PKG-INFO` & `twitter-api-client-0.9.9/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: twitter-api-client
-Version: 0.9.8
+Version: 0.9.9
 Summary: Twitter API
 Home-page: https://github.com/trevorhobenshield/twitter-api-client
 Author: Trevor Hobenshield
 Author-email: trevorhobenshield@gmail.com
 Keywords: twitter api client async search automation bot scrape
 Requires-Python: >=3.10.10
 Description-Content-Type: text/markdown
```

### Comparing `twitter-api-client-0.9.8/setup.py` & `twitter-api-client-0.9.9/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -10,15 +10,15 @@
     "tqdm",
     "orjson",
     'uvloop; platform_system != "Windows"',
 ]
 
 setup(
     name="twitter-api-client",
-    version="0.9.8",
+    version="0.9.9",
     python_requires=">=3.10.10",
     description="Twitter API",
     long_description=dedent('''
     
     ## Implementation of Twitter's v1, v2, and GraphQL APIs
```

### Comparing `twitter-api-client-0.9.8/twitter/account.py` & `twitter-api-client-0.9.9/twitter/account.py`

 * *Files 2% similar despite different names*

```diff
@@ -611,32 +611,37 @@
 
     @staticmethod
     def _validate_session(*args, **kwargs):
         email, username, password, session = args
 
         # validate credentials
         if all((email, username, password)):
-            return login(email, username, password, **kwargs)
+            session = login(email, username, password, **kwargs)
+            session._init_with_cookies = False
+            return session
 
         # invalid credentials, try validating session
         if session and all(session.cookies.get(c) for c in {'ct0', 'auth_token'}):
+            session._init_with_cookies = True
             return session
 
         # invalid credentials and session
         cookies = kwargs.get('cookies')
 
         # try validating cookies dict
         if isinstance(cookies, dict) and all(cookies.get(c) for c in {'ct0', 'auth_token'}):
             _session = Client(cookies=cookies, follow_redirects=True)
+            _session._init_with_cookies = True
             _session.headers.update(get_headers(_session))
             return _session
 
         # try validating cookies from file
         if isinstance(cookies, str):
             _session = Client(cookies=orjson.loads(Path(cookies).read_bytes()), follow_redirects=True)
+            _session._init_with_cookies = True
             _session.headers.update(get_headers(_session))
             return _session
 
         raise Exception('Session not authenticated. '
                         'Please use an authenticated session or remove the `session` argument and try again.')
 
     def dm_inbox(self) -> dict:
```

### Comparing `twitter-api-client-0.9.8/twitter/constants.py` & `twitter-api-client-0.9.9/twitter/constants.py`

 * *Files identical despite different names*

### Comparing `twitter-api-client-0.9.8/twitter/login.py` & `twitter-api-client-0.9.9/twitter/login.py`

 * *Files identical despite different names*

### Comparing `twitter-api-client-0.9.8/twitter/scraper.py` & `twitter-api-client-0.9.9/twitter/scraper.py`

 * *Files identical despite different names*

### Comparing `twitter-api-client-0.9.8/twitter/search.py` & `twitter-api-client-0.9.9/twitter/search.py`

 * *Files identical despite different names*

### Comparing `twitter-api-client-0.9.8/twitter/util.py` & `twitter-api-client-0.9.9/twitter/util.py`

 * *Files 6% similar despite different names*

```diff
@@ -105,29 +105,66 @@
 
 
 def get_headers(session, **kwargs) -> dict:
     """
     Get the headers required for authenticated requests
     """
     cookies = session.cookies
-    cookies.delete('ct0', domain='.twitter.com')
+    # todo httpx cookie issues
+    try:
+        if session._init_with_cookies:
+            cookies.delete('ct0', domain='.twitter.com')
+    except:
+        ...
     headers = kwargs | {
         'authorization': 'Bearer AAAAAAAAAAAAAAAAAAAAANRILgAAAAAAnNwIzUejRCOuH5E6I8xnZz4puTs=1Zv7ttfk8LF81IUq16cHjhLTvJu4FA33AGWWjCpTnA',
         'cookie': '; '.join(f'{k}={v}' for k, v in cookies.items()),
         'referer': 'https://twitter.com/',
         'user-agent': 'Mozilla/5.0 (Windows NT 10.0; Win64; x64) AppleWebKit/537.36 (KHTML, like Gecko) Chrome/113.0.0.0 Safari/537.36',
         'x-csrf-token': cookies.get('ct0', ''),
         'x-guest-token': cookies.get('guest_token', ''),
         'x-twitter-auth-type': 'OAuth2Session' if cookies.get('auth_token') else '',
         'x-twitter-active-user': 'yes',
         'x-twitter-client-language': 'en',
     }
     return dict(sorted({k.lower(): v for k, v in headers.items()}.items()))
 
 
+# def get_headers(session, **kwargs) -> dict:
+#     """
+#     Get the headers required for authenticated requests
+#     """
+#     cookies = {}
+#     for k in {'auth_token', 'ct0', 'flow_token', 'guest_id', 'guest_id_ads', 'guest_id_marketing', 'guest_token', 'kdt',
+#               'personalization_id', 'twid'}:
+#         cookies[k] = session.cookies.get(k, domain=None) or session.cookies.get(k, domain='.twitter.com')
+#     #
+#     # if cookies.get('ct0', domain=None):
+#     #     cookies.delete('ct0', domain='.twitter.com')
+#     # elif cookies.get('ct0', domain='.twitter.com'):
+#     #     cookies.delete('ct0', domain=None)
+#
+#     session.cookies.clear_session_cookies()
+#
+#     session.cookies.update(cookies)
+#
+#     headers = kwargs | {
+#         'authorization': 'Bearer AAAAAAAAAAAAAAAAAAAAANRILgAAAAAAnNwIzUejRCOuH5E6I8xnZz4puTs=1Zv7ttfk8LF81IUq16cHjhLTvJu4FA33AGWWjCpTnA',
+#         'cookie': '; '.join(f'{k}={v}' for k, v in cookies.items()),
+#         'referer': 'https://twitter.com/',
+#         'user-agent': 'Mozilla/5.0 (Windows NT 10.0; Win64; x64) AppleWebKit/537.36 (KHTML, like Gecko) Chrome/113.0.0.0 Safari/537.36',
+#         'x-csrf-token': cookies['ct0'] or '',
+#         'x-guest-token': cookies['guest_token'] or '',
+#         'x-twitter-auth-type': 'OAuth2Session' if cookies['auth_token'] else '',
+#         'x-twitter-active-user': 'yes',
+#         'x-twitter-client-language': 'en',
+#     }
+#     return dict(sorted({k.lower(): v for k, v in headers.items()}.items()))
+
+
 def find_key(obj: any, key: str) -> list:
     """
     Find all values of a given key within a nested dict or list of dicts
 
     Most data of interest is nested, and sometimes defined by different schemas.
     It is not worth our time to enumerate all absolute paths to a given key, then update
     the paths in our parsing functions every time Twitter changes their API.
```

### Comparing `twitter-api-client-0.9.8/twitter_api_client.egg-info/PKG-INFO` & `twitter-api-client-0.9.9/twitter_api_client.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: twitter-api-client
-Version: 0.9.8
+Version: 0.9.9
 Summary: Twitter API
 Home-page: https://github.com/trevorhobenshield/twitter-api-client
 Author: Trevor Hobenshield
 Author-email: trevorhobenshield@gmail.com
 Keywords: twitter api client async search automation bot scrape
 Requires-Python: >=3.10.10
 Description-Content-Type: text/markdown
```

