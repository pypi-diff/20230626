# Comparing `tmp/BlitzChain-0.1.1.tar.gz` & `tmp/BlitzChain-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "BlitzChain-0.1.1.tar", last modified: Mon Jun 26 02:07:03 2023, max compression
+gzip compressed data, was "BlitzChain-0.1.2.tar", last modified: Mon Jun 26 12:15:54 2023, max compression
```

## Comparing `BlitzChain-0.1.1.tar` & `BlitzChain-0.1.2.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxr-xr-x   0 jackywong   (501) staff       (20)        0 2023-06-26 02:07:03.968326 BlitzChain-0.1.1/
-drwxr-xr-x   0 jackywong   (501) staff       (20)        0 2023-06-26 02:07:03.964886 BlitzChain-0.1.1/BlitzChain.egg-info/
--rw-r--r--   0 jackywong   (501) staff       (20)      189 2023-06-26 02:07:03.000000 BlitzChain-0.1.1/BlitzChain.egg-info/PKG-INFO
--rw-r--r--   0 jackywong   (501) staff       (20)      310 2023-06-26 02:07:03.000000 BlitzChain-0.1.1/BlitzChain.egg-info/SOURCES.txt
--rw-r--r--   0 jackywong   (501) staff       (20)        1 2023-06-26 02:07:03.000000 BlitzChain-0.1.1/BlitzChain.egg-info/dependency_links.txt
--rw-r--r--   0 jackywong   (501) staff       (20)        9 2023-06-26 02:07:03.000000 BlitzChain-0.1.1/BlitzChain.egg-info/requires.txt
--rw-r--r--   0 jackywong   (501) staff       (20)       11 2023-06-26 02:07:03.000000 BlitzChain-0.1.1/BlitzChain.egg-info/top_level.txt
--rw-r--r--   0 jackywong   (501) staff       (20)    11357 2023-06-25 04:01:50.000000 BlitzChain-0.1.1/LICENSE
--rw-r--r--   0 jackywong   (501) staff       (20)      189 2023-06-26 02:07:03.968026 BlitzChain-0.1.1/PKG-INFO
--rw-r--r--   0 jackywong   (501) staff       (20)     3488 2023-06-25 07:25:46.000000 BlitzChain-0.1.1/README.md
-drwxr-xr-x   0 jackywong   (501) staff       (20)        0 2023-06-26 02:07:03.966177 BlitzChain-0.1.1/blitzchain/
--rw-r--r--   0 jackywong   (501) staff       (20)       19 2023-06-25 04:16:58.000000 BlitzChain-0.1.1/blitzchain/__init__.py
--rw-r--r--   0 jackywong   (501) staff       (20)     2363 2023-06-25 07:10:07.000000 BlitzChain-0.1.1/blitzchain/api.py
--rw-r--r--   0 jackywong   (501) staff       (20)      177 2023-06-25 05:12:43.000000 BlitzChain-0.1.1/blitzchain/utils.py
--rw-r--r--   0 jackywong   (501) staff       (20)       38 2023-06-26 02:07:03.968419 BlitzChain-0.1.1/setup.cfg
--rw-r--r--   0 jackywong   (501) staff       (20)      555 2023-06-26 02:07:02.000000 BlitzChain-0.1.1/setup.py
-drwxr-xr-x   0 jackywong   (501) staff       (20)        0 2023-06-26 02:07:03.967469 BlitzChain-0.1.1/tests/
--rw-r--r--   0 jackywong   (501) staff       (20)      216 2023-06-25 05:27:46.000000 BlitzChain-0.1.1/tests/test_crud.py
--rw-r--r--   0 jackywong   (501) staff       (20)      715 2023-06-25 05:08:57.000000 BlitzChain-0.1.1/tests/test_pdf.py
--rw-r--r--   0 jackywong   (501) staff       (20)      621 2023-06-25 07:10:23.000000 BlitzChain-0.1.1/tests/test_qa.py
+drwxr-xr-x   0 jackywong   (501) staff       (20)        0 2023-06-26 12:15:54.684223 BlitzChain-0.1.2/
+drwxr-xr-x   0 jackywong   (501) staff       (20)        0 2023-06-26 12:15:54.680229 BlitzChain-0.1.2/BlitzChain.egg-info/
+-rw-r--r--   0 jackywong   (501) staff       (20)      189 2023-06-26 12:15:54.000000 BlitzChain-0.1.2/BlitzChain.egg-info/PKG-INFO
+-rw-r--r--   0 jackywong   (501) staff       (20)      310 2023-06-26 12:15:54.000000 BlitzChain-0.1.2/BlitzChain.egg-info/SOURCES.txt
+-rw-r--r--   0 jackywong   (501) staff       (20)        1 2023-06-26 12:15:54.000000 BlitzChain-0.1.2/BlitzChain.egg-info/dependency_links.txt
+-rw-r--r--   0 jackywong   (501) staff       (20)        9 2023-06-26 12:15:54.000000 BlitzChain-0.1.2/BlitzChain.egg-info/requires.txt
+-rw-r--r--   0 jackywong   (501) staff       (20)       11 2023-06-26 12:15:54.000000 BlitzChain-0.1.2/BlitzChain.egg-info/top_level.txt
+-rw-r--r--   0 jackywong   (501) staff       (20)    11357 2023-06-25 04:01:50.000000 BlitzChain-0.1.2/LICENSE
+-rw-r--r--   0 jackywong   (501) staff       (20)      189 2023-06-26 12:15:54.683910 BlitzChain-0.1.2/PKG-INFO
+-rw-r--r--   0 jackywong   (501) staff       (20)     3488 2023-06-25 07:25:46.000000 BlitzChain-0.1.2/README.md
+drwxr-xr-x   0 jackywong   (501) staff       (20)        0 2023-06-26 12:15:54.681494 BlitzChain-0.1.2/blitzchain/
+-rw-r--r--   0 jackywong   (501) staff       (20)       42 2023-06-26 02:24:13.000000 BlitzChain-0.1.2/blitzchain/__init__.py
+-rw-r--r--   0 jackywong   (501) staff       (20)     2783 2023-06-26 12:14:12.000000 BlitzChain-0.1.2/blitzchain/api.py
+-rw-r--r--   0 jackywong   (501) staff       (20)      177 2023-06-26 02:49:39.000000 BlitzChain-0.1.2/blitzchain/utils.py
+-rw-r--r--   0 jackywong   (501) staff       (20)       38 2023-06-26 12:15:54.684321 BlitzChain-0.1.2/setup.cfg
+-rw-r--r--   0 jackywong   (501) staff       (20)      409 2023-06-26 02:24:27.000000 BlitzChain-0.1.2/setup.py
+drwxr-xr-x   0 jackywong   (501) staff       (20)        0 2023-06-26 12:15:54.683359 BlitzChain-0.1.2/tests/
+-rw-r--r--   0 jackywong   (501) staff       (20)      216 2023-06-25 05:27:46.000000 BlitzChain-0.1.2/tests/test_crud.py
+-rw-r--r--   0 jackywong   (501) staff       (20)      715 2023-06-25 05:08:57.000000 BlitzChain-0.1.2/tests/test_pdf.py
+-rw-r--r--   0 jackywong   (501) staff       (20)      621 2023-06-25 07:10:23.000000 BlitzChain-0.1.2/tests/test_qa.py
```

### Comparing `BlitzChain-0.1.1/LICENSE` & `BlitzChain-0.1.2/LICENSE`

 * *Files identical despite different names*

### Comparing `BlitzChain-0.1.1/README.md` & `BlitzChain-0.1.2/README.md`

 * *Files identical despite different names*

### Comparing `BlitzChain-0.1.1/blitzchain/api.py` & `BlitzChain-0.1.2/blitzchain/api.py`

 * *Files 20% similar despite different names*

```diff
@@ -11,25 +11,32 @@
 
 class Collection:
     def __init__(self, api_key: str, collection_name: str):
         self.collection_name = collection_name
         self.api_key = api_key
         self.base_url = "https://app.twilix.io/api/v1/"
     
-    def insert_objects(self, objects: list):
+    def insert_objects(
+        self,
+        objects: list,
+        fields_to_vectorize: list=None,
+        field_to_split: str = None
+    ):
         url = self.base_url + "collection/bulk-insert"
         response = requests.post(
             url,
             headers={
                 "Content-Type": "application/json", 
                 "Authorization": "Bearer " + self.api_key
             },
             json={
                 "collection": self.collection_name,
-                "objects": objects
+                "objects": objects,
+                "fieldsToVectorize": fields_to_vectorize,
+                "fieldToSplit": field_to_split
             }
 
         )
         print(response.content.decode())
         return response.json()
     
     def insert_pdf(self, url: str):
@@ -47,24 +54,28 @@
             }
         )
         print(response.content.decode())
         return response.json()
 
     
     def generative_qa(self, user_input: str, answer_fields: list,
-        conversation_id: str=None, limit: int=5):
+        conversation_id: str=None, limit: int=5, fields: list=None,
+        include_rerank: bool=False, minimum_rerank_score: float=0.7):
         """Get an answer based on a question that you ask.
         """
         url =  self.base_url + "collection/generative-qa"
         print(url)
         data={
             "collection": self.collection_name,
             "userInput": user_input,
             "answerFields": answer_fields,
-            # "limit": limit,
+            "limit": limit,
+            "fields": fields,
+            "includeRerank": include_rerank,
+            "minimumRerankScore": minimum_rerank_score
         }
         if conversation_id:
             data["conversationID"] = conversation_id
         print(data)
         response = requests.post(
             url,
             headers={
```

### Comparing `BlitzChain-0.1.1/tests/test_pdf.py` & `BlitzChain-0.1.2/tests/test_pdf.py`

 * *Files identical despite different names*

### Comparing `BlitzChain-0.1.1/tests/test_qa.py` & `BlitzChain-0.1.2/tests/test_qa.py`

 * *Files identical despite different names*

