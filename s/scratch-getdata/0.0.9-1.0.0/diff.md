# Comparing `tmp/scratch-getdata-0.0.9.tar.gz` & `tmp/scratch-getdata-1.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "scratch-getdata-0.0.9.tar", last modified: Fri Jun 23 18:38:03 2023, max compression
+gzip compressed data, was "scratch-getdata-1.0.0.tar", last modified: Mon Jun 26 02:42:03 2023, max compression
```

## Comparing `scratch-getdata-0.0.9.tar` & `scratch-getdata-1.0.0.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2023-06-23 18:38:03.379951 scratch-getdata-0.0.9/
--rw-r--r--   0 runner    (1000) runner    (1000)     2663 2023-06-23 18:38:03.379951 scratch-getdata-0.0.9/PKG-INFO
--rw-r--r--   0 runner    (1000) runner    (1000)     2100 2023-06-23 17:42:16.000000 scratch-getdata-0.0.9/README.md
--rw-r--r--   0 runner    (1000) runner    (1000)      633 2023-06-23 18:37:10.000000 scratch-getdata-0.0.9/pyproject.toml
-drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2023-06-23 18:38:03.379951 scratch-getdata-0.0.9/scratch_getdata/
--rw-r--r--   0 runner    (1000) runner    (1000)      517 2023-06-23 18:37:46.000000 scratch-getdata-0.0.9/scratch_getdata/__init__.py
--rw-r--r--   0 runner    (1000) runner    (1000)     2670 2023-06-23 18:21:14.000000 scratch-getdata-0.0.9/scratch_getdata/api_client.py
-drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2023-06-23 18:38:03.379951 scratch-getdata-0.0.9/scratch_getdata.egg-info/
--rw-r--r--   0 runner    (1000) runner    (1000)     2663 2023-06-23 18:38:03.000000 scratch-getdata-0.0.9/scratch_getdata.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1000) runner    (1000)      285 2023-06-23 18:38:03.000000 scratch-getdata-0.0.9/scratch_getdata.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1000) runner    (1000)        1 2023-06-23 18:38:03.000000 scratch-getdata-0.0.9/scratch_getdata.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1000) runner    (1000)        9 2023-06-23 18:38:03.000000 scratch-getdata-0.0.9/scratch_getdata.egg-info/requires.txt
--rw-r--r--   0 runner    (1000) runner    (1000)       16 2023-06-23 18:38:03.000000 scratch-getdata-0.0.9/scratch_getdata.egg-info/top_level.txt
--rw-r--r--   0 runner    (1000) runner    (1000)       38 2023-06-23 18:38:03.379951 scratch-getdata-0.0.9/setup.cfg
--rw-r--r--   0 runner    (1000) runner    (1000)      404 2023-06-23 17:56:58.000000 scratch-getdata-0.0.9/setup.py
+drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2023-06-26 02:42:03.609939 scratch-getdata-1.0.0/
+-rw-r--r--   0 runner    (1000) runner    (1000)     2663 2023-06-26 02:42:03.609939 scratch-getdata-1.0.0/PKG-INFO
+-rw-r--r--   0 runner    (1000) runner    (1000)     2100 2023-06-23 17:42:16.000000 scratch-getdata-1.0.0/README.md
+-rw-r--r--   0 runner    (1000) runner    (1000)      633 2023-06-26 02:38:48.000000 scratch-getdata-1.0.0/pyproject.toml
+drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2023-06-26 02:42:03.609939 scratch-getdata-1.0.0/scratch_getdata/
+-rw-r--r--   0 runner    (1000) runner    (1000)      517 2023-06-23 18:37:46.000000 scratch-getdata-1.0.0/scratch_getdata/__init__.py
+-rw-r--r--   0 runner    (1000) runner    (1000)     3370 2023-06-26 02:38:13.000000 scratch-getdata-1.0.0/scratch_getdata/api_client.py
+drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2023-06-26 02:42:03.609939 scratch-getdata-1.0.0/scratch_getdata.egg-info/
+-rw-r--r--   0 runner    (1000) runner    (1000)     2663 2023-06-26 02:42:03.000000 scratch-getdata-1.0.0/scratch_getdata.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1000) runner    (1000)      285 2023-06-26 02:42:03.000000 scratch-getdata-1.0.0/scratch_getdata.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1000) runner    (1000)        1 2023-06-26 02:42:03.000000 scratch-getdata-1.0.0/scratch_getdata.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1000) runner    (1000)        9 2023-06-26 02:42:03.000000 scratch-getdata-1.0.0/scratch_getdata.egg-info/requires.txt
+-rw-r--r--   0 runner    (1000) runner    (1000)       16 2023-06-26 02:42:03.000000 scratch-getdata-1.0.0/scratch_getdata.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1000) runner    (1000)       38 2023-06-26 02:42:03.609939 scratch-getdata-1.0.0/setup.cfg
+-rw-r--r--   0 runner    (1000) runner    (1000)      404 2023-06-23 17:56:58.000000 scratch-getdata-1.0.0/setup.py
```

### Comparing `scratch-getdata-0.0.9/PKG-INFO` & `scratch-getdata-1.0.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: scratch-getdata
-Version: 0.0.9
+Version: 1.0.0
 Summary: A Module to fetch scratch things from ScratchGetData
 Author: kokofixcomputers
 Author-email: kokofixcomputers <none@none.com>
 Project-URL: Homepage, https://github.com/kokofixcomputers/Scratch-getdata
 Project-URL: Bug Tracker, https://github.com/kokofixcomputers/Scratch-getdata/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `scratch-getdata-0.0.9/README.md` & `scratch-getdata-1.0.0/README.md`

 * *Files identical despite different names*

### Comparing `scratch-getdata-0.0.9/pyproject.toml` & `scratch-getdata-1.0.0/pyproject.toml`

 * *Files 20% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "scratch-getdata"
-version = "0.0.9"
+version = "1.0.0"
 authors = [
   { name="kokofixcomputers", email="none@none.com" },
 ]
 description = "A Module to fetch scratch things from ScratchGetData"
 readme = "README.md"
 requires-python = ">=3.7"
 classifiers = [
```

### Comparing `scratch-getdata-0.0.9/scratch_getdata/__init__.py` & `scratch-getdata-1.0.0/scratch_getdata/__init__.py`

 * *Files identical despite different names*

### Comparing `scratch-getdata-0.0.9/scratch_getdata/api_client.py` & `scratch-getdata-1.0.0/scratch_getdata/api_client.py`

 * *Files 24% similar despite different names*

```diff
@@ -4,73 +4,74 @@
     def __init__(self):
         print("If you use GetData please credit @kokofixcomputers")
         self.base_url = "https://scratch-get-data.kokoiscool.repl.co"
 
     def get_follower_count(self, username):
         url = f"{self.base_url}/get/follower-count/{username}/"
         response = requests.get(url)
-        return response.json()
+        return response.text.strip()  # Return the follower count as a string
 
     def is_scratcher(self, username):
         url = f"{self.base_url}/get/is_scratcher/{username}/"
         response = requests.get(url)
-        return response.json()
+        return response.text.strip().lower() == "true"  # Return True or False based on the response
 
     def get_following_count(self, username):
         url = f"{self.base_url}/get/following-count/{username}/"
         response = requests.get(url)
-        return response.json()
+        return response.text.strip()  # Return the following count as a string
 
     def get_wiwo(self, username):
         url = f"{self.base_url}/get/wiwo/{username}/"
         response = requests.get(url)
-        return response.json()
+        return response.text.strip()  # Return the WiWo as a string
 
     def get_about_me(self, username):
         url = f"{self.base_url}/get/aboutme/{username}/"
         response = requests.get(url)
-        return response.json()
+        return response.text.strip()  # Return the About Me text as a string
 
     def get_messages(self, username):
         url = f"{self.base_url}/get/messages/{username}/"
         response = requests.get(url)
-        return response.json()
+        return response.text.strip()  # Return the Messages as a string
 
     def get_project_creator(self, project_id):
         url = f"{self.base_url}/get/project/creator/{project_id}/"
         response = requests.get(url)
-        return response.json()
+        return response.text.strip()  # Return the project creator username as a string
 
     def get_project_name(self, project_id):
         url = f"{self.base_url}/get/project/name/{project_id}/"
         response = requests.get(url)
-        return response.json()
+        return response.text.strip()  # Return the project name as a string
 
     def get_project_description(self, project_id):
         url = f"{self.base_url}/get/project/notes_and_credits/{project_id}/"
         response = requests.get(url)
-        return response.json()
+        return response.text.strip()  # Return the project description as a string
 
     def get_project_instructions(self, project_id):
         url = f"{self.base_url}/get/project/instructions/{project_id}/"
         response = requests.get(url)
-        return response.json()
+        return response.text.strip()  # Return the project instructions as a string
 
     def get_project_blocks(self, project_id):
         url = f"{self.base_url}/get/project/blocks/{project_id}/"
         response = requests.get(url)
-        return response.json()
+        return response.text.strip()  # Return the project blocks as a string
 
     def get_forum_title(self, post_id):
         url = f"{self.base_url}/get/forum/title/{post_id}/"
         response = requests.get(url)
-        return response.json()
+        return response.text.strip()  # Return the forum post title as a string
 
     def get_forum_category(self, post_id):
         url = f"{self.base_url}/get/forum/category/{post_id}/"
         response = requests.get(url)
-        return response.json()
+        return response.text.strip()  # Return the forum post category as a string
 
     def get_scratch_user_country(self, username):
         url = f"{self.base_url}/get/user/country/{username}/"
         response = requests.get(url)
-        return response.json()
+        return response.text.strip()  # Return the Scratch user's country as a string
+
```

### Comparing `scratch-getdata-0.0.9/scratch_getdata.egg-info/PKG-INFO` & `scratch-getdata-1.0.0/scratch_getdata.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: scratch-getdata
-Version: 0.0.9
+Version: 1.0.0
 Summary: A Module to fetch scratch things from ScratchGetData
 Author: kokofixcomputers
 Author-email: kokofixcomputers <none@none.com>
 Project-URL: Homepage, https://github.com/kokofixcomputers/Scratch-getdata
 Project-URL: Bug Tracker, https://github.com/kokofixcomputers/Scratch-getdata/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

