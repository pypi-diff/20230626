# Comparing `tmp/BlitzChain-0.1.3.tar.gz` & `tmp/BlitzChain-0.1.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "BlitzChain-0.1.3.tar", last modified: Mon Jun 26 13:28:16 2023, max compression
+gzip compressed data, was "BlitzChain-0.1.4.tar", last modified: Mon Jun 26 15:31:54 2023, max compression
```

## Comparing `BlitzChain-0.1.3.tar` & `BlitzChain-0.1.4.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxr-xr-x   0 jackywong   (501) staff       (20)        0 2023-06-26 13:28:16.905695 BlitzChain-0.1.3/
-drwxr-xr-x   0 jackywong   (501) staff       (20)        0 2023-06-26 13:28:16.902107 BlitzChain-0.1.3/BlitzChain.egg-info/
--rw-r--r--   0 jackywong   (501) staff       (20)      189 2023-06-26 13:28:16.000000 BlitzChain-0.1.3/BlitzChain.egg-info/PKG-INFO
--rw-r--r--   0 jackywong   (501) staff       (20)      310 2023-06-26 13:28:16.000000 BlitzChain-0.1.3/BlitzChain.egg-info/SOURCES.txt
--rw-r--r--   0 jackywong   (501) staff       (20)        1 2023-06-26 13:28:16.000000 BlitzChain-0.1.3/BlitzChain.egg-info/dependency_links.txt
--rw-r--r--   0 jackywong   (501) staff       (20)        9 2023-06-26 13:28:16.000000 BlitzChain-0.1.3/BlitzChain.egg-info/requires.txt
--rw-r--r--   0 jackywong   (501) staff       (20)       11 2023-06-26 13:28:16.000000 BlitzChain-0.1.3/BlitzChain.egg-info/top_level.txt
--rw-r--r--   0 jackywong   (501) staff       (20)    11357 2023-06-25 04:01:50.000000 BlitzChain-0.1.3/LICENSE
--rw-r--r--   0 jackywong   (501) staff       (20)      189 2023-06-26 13:28:16.905374 BlitzChain-0.1.3/PKG-INFO
--rw-r--r--   0 jackywong   (501) staff       (20)     3488 2023-06-25 07:25:46.000000 BlitzChain-0.1.3/README.md
-drwxr-xr-x   0 jackywong   (501) staff       (20)        0 2023-06-26 13:28:16.903189 BlitzChain-0.1.3/blitzchain/
--rw-r--r--   0 jackywong   (501) staff       (20)       42 2023-06-26 13:28:03.000000 BlitzChain-0.1.3/blitzchain/__init__.py
--rw-r--r--   0 jackywong   (501) staff       (20)     2924 2023-06-26 13:24:55.000000 BlitzChain-0.1.3/blitzchain/api.py
--rw-r--r--   0 jackywong   (501) staff       (20)      177 2023-06-26 02:49:39.000000 BlitzChain-0.1.3/blitzchain/utils.py
--rw-r--r--   0 jackywong   (501) staff       (20)       38 2023-06-26 13:28:16.905785 BlitzChain-0.1.3/setup.cfg
--rw-r--r--   0 jackywong   (501) staff       (20)      409 2023-06-26 02:24:27.000000 BlitzChain-0.1.3/setup.py
-drwxr-xr-x   0 jackywong   (501) staff       (20)        0 2023-06-26 13:28:16.904800 BlitzChain-0.1.3/tests/
--rw-r--r--   0 jackywong   (501) staff       (20)      216 2023-06-25 05:27:46.000000 BlitzChain-0.1.3/tests/test_crud.py
--rw-r--r--   0 jackywong   (501) staff       (20)      715 2023-06-25 05:08:57.000000 BlitzChain-0.1.3/tests/test_pdf.py
--rw-r--r--   0 jackywong   (501) staff       (20)      621 2023-06-25 07:10:23.000000 BlitzChain-0.1.3/tests/test_qa.py
+drwxr-xr-x   0 jackywong   (501) staff       (20)        0 2023-06-26 15:31:54.934707 BlitzChain-0.1.4/
+drwxr-xr-x   0 jackywong   (501) staff       (20)        0 2023-06-26 15:31:54.930494 BlitzChain-0.1.4/BlitzChain.egg-info/
+-rw-r--r--   0 jackywong   (501) staff       (20)      189 2023-06-26 15:31:54.000000 BlitzChain-0.1.4/BlitzChain.egg-info/PKG-INFO
+-rw-r--r--   0 jackywong   (501) staff       (20)      310 2023-06-26 15:31:54.000000 BlitzChain-0.1.4/BlitzChain.egg-info/SOURCES.txt
+-rw-r--r--   0 jackywong   (501) staff       (20)        1 2023-06-26 15:31:54.000000 BlitzChain-0.1.4/BlitzChain.egg-info/dependency_links.txt
+-rw-r--r--   0 jackywong   (501) staff       (20)        9 2023-06-26 15:31:54.000000 BlitzChain-0.1.4/BlitzChain.egg-info/requires.txt
+-rw-r--r--   0 jackywong   (501) staff       (20)       11 2023-06-26 15:31:54.000000 BlitzChain-0.1.4/BlitzChain.egg-info/top_level.txt
+-rw-r--r--   0 jackywong   (501) staff       (20)    11357 2023-06-25 04:01:50.000000 BlitzChain-0.1.4/LICENSE
+-rw-r--r--   0 jackywong   (501) staff       (20)      189 2023-06-26 15:31:54.934041 BlitzChain-0.1.4/PKG-INFO
+-rw-r--r--   0 jackywong   (501) staff       (20)     3488 2023-06-25 07:25:46.000000 BlitzChain-0.1.4/README.md
+drwxr-xr-x   0 jackywong   (501) staff       (20)        0 2023-06-26 15:31:54.931559 BlitzChain-0.1.4/blitzchain/
+-rw-r--r--   0 jackywong   (501) staff       (20)       42 2023-06-26 15:30:19.000000 BlitzChain-0.1.4/blitzchain/__init__.py
+-rw-r--r--   0 jackywong   (501) staff       (20)     3063 2023-06-26 15:31:41.000000 BlitzChain-0.1.4/blitzchain/api.py
+-rw-r--r--   0 jackywong   (501) staff       (20)      177 2023-06-26 02:49:39.000000 BlitzChain-0.1.4/blitzchain/utils.py
+-rw-r--r--   0 jackywong   (501) staff       (20)       38 2023-06-26 15:31:54.934875 BlitzChain-0.1.4/setup.cfg
+-rw-r--r--   0 jackywong   (501) staff       (20)      409 2023-06-26 02:24:27.000000 BlitzChain-0.1.4/setup.py
+drwxr-xr-x   0 jackywong   (501) staff       (20)        0 2023-06-26 15:31:54.932977 BlitzChain-0.1.4/tests/
+-rw-r--r--   0 jackywong   (501) staff       (20)      216 2023-06-25 05:27:46.000000 BlitzChain-0.1.4/tests/test_crud.py
+-rw-r--r--   0 jackywong   (501) staff       (20)      715 2023-06-25 05:08:57.000000 BlitzChain-0.1.4/tests/test_pdf.py
+-rw-r--r--   0 jackywong   (501) staff       (20)      621 2023-06-25 07:10:23.000000 BlitzChain-0.1.4/tests/test_qa.py
```

### Comparing `BlitzChain-0.1.3/LICENSE` & `BlitzChain-0.1.4/LICENSE`

 * *Files identical despite different names*

### Comparing `BlitzChain-0.1.3/README.md` & `BlitzChain-0.1.4/README.md`

 * *Files identical despite different names*

### Comparing `BlitzChain-0.1.3/blitzchain/api.py` & `BlitzChain-0.1.4/blitzchain/api.py`

 * *Files 14% similar despite different names*

```diff
@@ -38,14 +38,16 @@
                 "objects": objects,
                 "fieldsToVectorize": fields_to_vectorize,
                 "fieldToSplit": field_to_split
             }
 
         )
         print(response.content.decode())
+        if not wait_to_finish:
+            return response.status_code == 200, "Request failed - please make sure parameters are correct."
         return response.json()
     
     def insert_pdf(self, url: str):
         api_url = self.base_url + "collection/insert-pdf"
         print(api_url)
         response = requests.post(
             api_url,
```

### Comparing `BlitzChain-0.1.3/tests/test_pdf.py` & `BlitzChain-0.1.4/tests/test_pdf.py`

 * *Files identical despite different names*

### Comparing `BlitzChain-0.1.3/tests/test_qa.py` & `BlitzChain-0.1.4/tests/test_qa.py`

 * *Files identical despite different names*

