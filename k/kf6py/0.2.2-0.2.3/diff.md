# Comparing `tmp/kf6py-0.2.2.tar.gz` & `tmp/kf6py-0.2.3.tar.gz`

## Comparing `kf6py-0.2.2.tar` & `kf6py-0.2.3.tar`

### file list

```diff
@@ -1,8 +1,8 @@
--rw-r--r--   0        0        0       23 2020-02-02 00:00:00.000000 kf6py-0.2.2/src/kf6py/__init__.py
--rw-r--r--   0        0        0     6222 2020-02-02 00:00:00.000000 kf6py-0.2.2/src/kf6py/api.py
--rw-r--r--   0        0        0      687 2020-02-02 00:00:00.000000 kf6py-0.2.2/tests/testing.py
--rw-r--r--   0        0        0       13 2020-02-02 00:00:00.000000 kf6py-0.2.2/.gitignore
--rw-r--r--   0        0        0     1091 2020-02-02 00:00:00.000000 kf6py-0.2.2/LICENSE
--rw-r--r--   0        0        0      719 2020-02-02 00:00:00.000000 kf6py-0.2.2/README.md
--rw-r--r--   0        0        0      709 2020-02-02 00:00:00.000000 kf6py-0.2.2/pyproject.toml
--rw-r--r--   0        0        0     1306 2020-02-02 00:00:00.000000 kf6py-0.2.2/PKG-INFO
+-rw-r--r--   0        0        0       23 2020-02-02 00:00:00.000000 kf6py-0.2.3/src/kf6py/__init__.py
+-rw-r--r--   0        0        0     7527 2020-02-02 00:00:00.000000 kf6py-0.2.3/src/kf6py/api.py
+-rw-r--r--   0        0        0      788 2020-02-02 00:00:00.000000 kf6py-0.2.3/tests/testing.py
+-rw-r--r--   0        0        0       16 2020-02-02 00:00:00.000000 kf6py-0.2.3/.gitignore
+-rw-r--r--   0        0        0     1091 2020-02-02 00:00:00.000000 kf6py-0.2.3/LICENSE
+-rw-r--r--   0        0        0      762 2020-02-02 00:00:00.000000 kf6py-0.2.3/README.md
+-rw-r--r--   0        0        0      709 2020-02-02 00:00:00.000000 kf6py-0.2.3/pyproject.toml
+-rw-r--r--   0        0        0     1344 2020-02-02 00:00:00.000000 kf6py-0.2.3/PKG-INFO
```

### Comparing `kf6py-0.2.2/src/kf6py/api.py` & `kf6py-0.2.3/src/kf6py/api.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,22 +1,22 @@
 import requests
 from typing import List, Dict, Any
 from bs4 import BeautifulSoup
 
 class KF6API:
-    def __init__(self, url, username, password):
+    def __init__(self, url: str, username: str, password: str):
         self.login_credential = {
             'userName': username,
             'password': password
         }
-        self.KF_URL = url
+        self.KF_URL = url.strip('/ ')
         self.token = self._login()
         self.author_id = None
         self.current_community = None
-        self.temp_data = []
+        self.temp_data = {} # holds contributions map in current community
 
     def _login(self) -> str:
         res = requests.post(f"{self.KF_URL}/auth/local", json = self.login_credential)
         if res.status_code != 200:
             raise Exception("Something is not right", res)
 
         return res.json()['token']
@@ -110,27 +110,57 @@
         if res.json(): 
             print("VIEW TITLE:", res.json()[0]["_from"]["title"])
 
         riseaboves = []
         target_ids = [i['to'] for i in res.json()]
         result = []
         for i in target_ids:
-            data = self.temp_data[i]
+            data = self.temp_data.setdefault(i, self.get_single_object(i))
             result.append(data)
             
-            riseabove_view = data['riseabove_view']
+            riseabove_view = data.get('riseabove_view', None) # this helps for some scheme where this doesn't exist
             if riseabove_view:
                 riseaboves.append(riseabove_view)
         
         while riseaboves:
             ra_view_id = riseaboves.pop(0)
             result += self.get_notes_from_view(community_id, ra_view_id)
 
         return result
     
+    def get_single_object(self, object_id: str):
+        response = requests.get(f"{self.KF_URL}/api/objects/{object_id}", headers=self._craft_header() ).json()
+        return response
+
+    def get_links(self, community_id: str, type: str = None, succinct: bool = True):
+        body = {
+            'query': {
+                "_from.status": "active"
+            }
+        }
+        if type:
+            assert type in ['buildson', 'contains'] # support these for now...
+            body['query']['type'] = type
+
+        res_links = requests.post(f"{self.KF_URL}/api/links/{community_id}/search", headers=self._craft_header(), json=body)
+        if succinct:
+            return [{
+                "from": i["from"],
+                "to": i["to"]
+            } for i in res_links.json()]
+        else:
+            return res_links.json()
+
+    def get_notes_from_author(self, author_id: str) -> List:
+        """get notes from a given author"""
+        assert self.current_community is not None
+        
+        return {i: j for i, j in self.temp_data.items() if author_id in j["authors"]}
+        
+
     def create_contribution(self, community_id: str, view_id: str, title: str, content: str):
     
         res_authors = requests.get(f"{self.KF_URL}/api/authors/{community_id}/me", headers= self._craft_header())
         self.author_id = res_authors.json()["_id"]
         contribution = {
             'communityId': community_id,
             'type': "Note",
```

### Comparing `kf6py-0.2.2/LICENSE` & `kf6py-0.2.3/LICENSE`

 * *Files identical despite different names*

### Comparing `kf6py-0.2.2/README.md` & `kf6py-0.2.3/README.md`

 * *Files 7% similar despite different names*

```diff
@@ -1,11 +1,16 @@
 # KF6 API for Python
 
 This is python package for calling KF6's API's, in hope to make it more friendly for learning analytic researchers.
 
+## install
+```
+pip install kf6py
+```
+
 ## usage
 ``` python
 from kf6py import KF6API
 
 # we recommend using environment variables to store sensitive information
 kf6api = KF6API(kfurl, username, password)
```

### Comparing `kf6py-0.2.2/pyproject.toml` & `kf6py-0.2.3/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 
 [project]
 name = "kf6py"
 dependencies = [
     'requests >=2.28, <3',
     'beautifulsoup4 >=4, <5',
 ]
-version = "0.2.2"
+version = "0.2.3"
 
 authors = [
     { name="Jerrison Chang-Sundin", email="chunyen.cs@gmail.com"}
 ]
 
 description = "A small tool for calling APIs in Knowledge Forum"
```

### Comparing `kf6py-0.2.2/PKG-INFO` & `kf6py-0.2.3/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: kf6py
-Version: 0.2.2
+Version: 0.2.3
 Summary: A small tool for calling APIs in Knowledge Forum
 Project-URL: Homepage, https://github.com/JerrisonChang/kf6api-py
 Project-URL: Bug Tracker, https://github.com/JerrisonChang/kf6api-py/issues
 Author-email: Jerrison Chang-Sundin <chunyen.cs@gmail.com>
 License-File: LICENSE
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
@@ -14,14 +14,19 @@
 Requires-Dist: requests<3,>=2.28
 Description-Content-Type: text/markdown
 
 # KF6 API for Python
 
 This is python package for calling KF6's API's, in hope to make it more friendly for learning analytic researchers.
 
+## install
+```
+pip install kf6py
+```
+
 ## usage
 ``` python
 from kf6py import KF6API
 
 # we recommend using environment variables to store sensitive information
 kf6api = KF6API(kfurl, username, password)
```

