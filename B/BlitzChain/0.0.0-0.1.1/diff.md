# Comparing `tmp/BlitzChain-0.0.0.tar.gz` & `tmp/BlitzChain-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "BlitzChain-0.0.0.tar", last modified: Sun Jun 25 04:18:27 2023, max compression
+gzip compressed data, was "BlitzChain-0.1.1.tar", last modified: Mon Jun 26 02:07:03 2023, max compression
```

## Comparing `BlitzChain-0.0.0.tar` & `BlitzChain-0.1.1.tar`

### file list

```diff
@@ -1,15 +1,20 @@
-drwxr-xr-x   0 jackywong   (501) staff       (20)        0 2023-06-25 04:18:27.377664 BlitzChain-0.0.0/
-drwxr-xr-x   0 jackywong   (501) staff       (20)        0 2023-06-25 04:18:27.376068 BlitzChain-0.0.0/BlitzChain.egg-info/
--rw-r--r--   0 jackywong   (501) staff       (20)      189 2023-06-25 04:18:27.000000 BlitzChain-0.0.0/BlitzChain.egg-info/PKG-INFO
--rw-r--r--   0 jackywong   (501) staff       (20)      236 2023-06-25 04:18:27.000000 BlitzChain-0.0.0/BlitzChain.egg-info/SOURCES.txt
--rw-r--r--   0 jackywong   (501) staff       (20)        1 2023-06-25 04:18:27.000000 BlitzChain-0.0.0/BlitzChain.egg-info/dependency_links.txt
--rw-r--r--   0 jackywong   (501) staff       (20)        9 2023-06-25 04:18:27.000000 BlitzChain-0.0.0/BlitzChain.egg-info/requires.txt
--rw-r--r--   0 jackywong   (501) staff       (20)       11 2023-06-25 04:18:27.000000 BlitzChain-0.0.0/BlitzChain.egg-info/top_level.txt
--rw-r--r--   0 jackywong   (501) staff       (20)    11357 2023-06-25 04:01:50.000000 BlitzChain-0.0.0/LICENSE
--rw-r--r--   0 jackywong   (501) staff       (20)      189 2023-06-25 04:18:27.377375 BlitzChain-0.0.0/PKG-INFO
--rw-r--r--   0 jackywong   (501) staff       (20)     3240 2023-06-25 04:11:24.000000 BlitzChain-0.0.0/README.md
-drwxr-xr-x   0 jackywong   (501) staff       (20)        0 2023-06-25 04:18:27.376928 BlitzChain-0.0.0/blitzchain/
--rw-r--r--   0 jackywong   (501) staff       (20)       19 2023-06-25 04:16:58.000000 BlitzChain-0.0.0/blitzchain/__init__.py
--rw-r--r--   0 jackywong   (501) staff       (20)     1645 2023-06-25 04:17:58.000000 BlitzChain-0.0.0/blitzchain/api.py
--rw-r--r--   0 jackywong   (501) staff       (20)       38 2023-06-25 04:18:27.377771 BlitzChain-0.0.0/setup.cfg
--rw-r--r--   0 jackywong   (501) staff       (20)      302 2023-06-25 04:02:37.000000 BlitzChain-0.0.0/setup.py
+drwxr-xr-x   0 jackywong   (501) staff       (20)        0 2023-06-26 02:07:03.968326 BlitzChain-0.1.1/
+drwxr-xr-x   0 jackywong   (501) staff       (20)        0 2023-06-26 02:07:03.964886 BlitzChain-0.1.1/BlitzChain.egg-info/
+-rw-r--r--   0 jackywong   (501) staff       (20)      189 2023-06-26 02:07:03.000000 BlitzChain-0.1.1/BlitzChain.egg-info/PKG-INFO
+-rw-r--r--   0 jackywong   (501) staff       (20)      310 2023-06-26 02:07:03.000000 BlitzChain-0.1.1/BlitzChain.egg-info/SOURCES.txt
+-rw-r--r--   0 jackywong   (501) staff       (20)        1 2023-06-26 02:07:03.000000 BlitzChain-0.1.1/BlitzChain.egg-info/dependency_links.txt
+-rw-r--r--   0 jackywong   (501) staff       (20)        9 2023-06-26 02:07:03.000000 BlitzChain-0.1.1/BlitzChain.egg-info/requires.txt
+-rw-r--r--   0 jackywong   (501) staff       (20)       11 2023-06-26 02:07:03.000000 BlitzChain-0.1.1/BlitzChain.egg-info/top_level.txt
+-rw-r--r--   0 jackywong   (501) staff       (20)    11357 2023-06-25 04:01:50.000000 BlitzChain-0.1.1/LICENSE
+-rw-r--r--   0 jackywong   (501) staff       (20)      189 2023-06-26 02:07:03.968026 BlitzChain-0.1.1/PKG-INFO
+-rw-r--r--   0 jackywong   (501) staff       (20)     3488 2023-06-25 07:25:46.000000 BlitzChain-0.1.1/README.md
+drwxr-xr-x   0 jackywong   (501) staff       (20)        0 2023-06-26 02:07:03.966177 BlitzChain-0.1.1/blitzchain/
+-rw-r--r--   0 jackywong   (501) staff       (20)       19 2023-06-25 04:16:58.000000 BlitzChain-0.1.1/blitzchain/__init__.py
+-rw-r--r--   0 jackywong   (501) staff       (20)     2363 2023-06-25 07:10:07.000000 BlitzChain-0.1.1/blitzchain/api.py
+-rw-r--r--   0 jackywong   (501) staff       (20)      177 2023-06-25 05:12:43.000000 BlitzChain-0.1.1/blitzchain/utils.py
+-rw-r--r--   0 jackywong   (501) staff       (20)       38 2023-06-26 02:07:03.968419 BlitzChain-0.1.1/setup.cfg
+-rw-r--r--   0 jackywong   (501) staff       (20)      555 2023-06-26 02:07:02.000000 BlitzChain-0.1.1/setup.py
+drwxr-xr-x   0 jackywong   (501) staff       (20)        0 2023-06-26 02:07:03.967469 BlitzChain-0.1.1/tests/
+-rw-r--r--   0 jackywong   (501) staff       (20)      216 2023-06-25 05:27:46.000000 BlitzChain-0.1.1/tests/test_crud.py
+-rw-r--r--   0 jackywong   (501) staff       (20)      715 2023-06-25 05:08:57.000000 BlitzChain-0.1.1/tests/test_pdf.py
+-rw-r--r--   0 jackywong   (501) staff       (20)      621 2023-06-25 07:10:23.000000 BlitzChain-0.1.1/tests/test_qa.py
```

### Comparing `BlitzChain-0.0.0/LICENSE` & `BlitzChain-0.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `BlitzChain-0.0.0/README.md` & `BlitzChain-0.1.1/README.md`

 * *Files 22% similar despite different names*

```diff
@@ -2,22 +2,22 @@
 
 
 Retrieval-Augmented Generation For Powerful Results
 
 ## Installation
 
 ```
-pip install blitzchain
+pip install -e git+https://github.com/mr-gpt/blitzchain.git#egg=blitzchain
 ```
 
 Once you install, you can get your API key from https://app.twilix.io/
 
 If you would like to then use this for your solutions, we recommend the following: 
 
-## Inserting Data
+## QuickStart
 
 ```python
 import blitzchain
 
 # Get API key from https://app.twilix.io
 client = blitzchain.Client(api_key="XYZ")
 collection = client.Collection()
@@ -81,16 +81,24 @@
     handbook_example_5,
     handbook_example_6,
     handbook_example_7,
     handbook_example_8,
     handbook_example_9
 ]
 
-collection.insert_obejcts(docs)
+collection.insert_objects(docs)
 
 ```
 
 ## Retrieving RAG Results
 
 ```python
-collection.generative_qa()
+collection.generative_qa(
+    user_input="Why?",
+    answer_fields=["content"],
+)
 ```
+
+# Documentation
+
+If you would like to read more about how to use this - 
+we recommend visiting [https://docs.twilix.io](https://docs.twilix.io)
```

### Comparing `BlitzChain-0.0.0/blitzchain/api.py` & `BlitzChain-0.1.1/blitzchain/api.py`

 * *Files 16% similar despite different names*

```diff
@@ -9,43 +9,69 @@
     def Collection(self, collection_name: str):
         return Collection(api_key=self.api_key, collection_name=collection_name)
 
 class Collection:
     def __init__(self, api_key: str, collection_name: str):
         self.collection_name = collection_name
         self.api_key = api_key
-        self.base_url = "https://app.twilix.io/"
-
+        self.base_url = "https://app.twilix.io/api/v1/"
+    
     def insert_objects(self, objects: list):
+        url = self.base_url + "collection/bulk-insert"
         response = requests.post(
-            self.base_url + "api/v1/collection/insert_objects",
+            url,
             headers={
                 "Content-Type": "application/json", 
                 "Authorization": "Bearer " + self.api_key
             },
             json={
-                "collection_name": self.collection_name,
+                "collection": self.collection_name,
                 "objects": objects
             }
 
         )
+        print(response.content.decode())
+        return response.json()
+    
+    def insert_pdf(self, url: str):
+        api_url = self.base_url + "collection/insert-pdf"
+        print(api_url)
+        response = requests.post(
+            api_url,
+            headers={
+                # "Content-Type": "application/json",
+                "Authorization": "Bearer " + self.api_key
+            },
+            json={
+                "collection": self.collection_name,
+                "url": url
+            }
+        )
+        print(response.content.decode())
         return response.json()
+
     
-    def generative_qa(self, user_input: str, fields: list,
-        conversation_id: str, limit: int=5):
+    def generative_qa(self, user_input: str, answer_fields: list,
+        conversation_id: str=None, limit: int=5):
         """Get an answer based on a question that you ask.
         """
+        url =  self.base_url + "collection/generative-qa"
+        print(url)
+        data={
+            "collection": self.collection_name,
+            "userInput": user_input,
+            "answerFields": answer_fields,
+            # "limit": limit,
+        }
+        if conversation_id:
+            data["conversationID"] = conversation_id
+        print(data)
         response = requests.post(
-            self.base_url + "api/v1/collection/generative_qa",
+            url,
             headers={
                 "Content-Type": "application/json",
                 "Authorization": "Bearer " + self.api_key
             },
-            json={
-                "collection_name": self.collection_name,
-                "userInput": user_input,
-                "fields": fields,
-                "conversationID": conversation_id,
-                "limit": limit,
-            }
+            json=data
         )
+        print(response.content.decode())
         return response.json()
```

