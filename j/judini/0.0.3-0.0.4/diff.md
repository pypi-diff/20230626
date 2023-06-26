# Comparing `tmp/judini-0.0.3.tar.gz` & `tmp/judini-0.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "judini-0.0.3.tar", last modified: Mon Jun 26 04:43:21 2023, max compression
+gzip compressed data, was "judini-0.0.4.tar", last modified: Mon Jun 26 04:48:55 2023, max compression
```

## Comparing `judini-0.0.3.tar` & `judini-0.0.4.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxr-xr-x   0 danipower   (501) staff       (20)        0 2023-06-26 04:43:21.270466 judini-0.0.3/
--rw-r--r--   0 danipower   (501) staff       (20)     1073 2023-06-25 22:23:04.000000 judini-0.0.3/LICENSE
--rw-r--r--   0 danipower   (501) staff       (20)     1438 2023-06-26 04:43:21.270605 judini-0.0.3/PKG-INFO
--rw-r--r--   0 danipower   (501) staff       (20)     1013 2023-06-26 04:42:21.000000 judini-0.0.3/README.md
--rw-r--r--   0 danipower   (501) staff       (20)      119 2023-06-26 04:06:55.000000 judini-0.0.3/pyproject.toml
--rw-r--r--   0 danipower   (501) staff       (20)      662 2023-06-26 04:43:21.271118 judini-0.0.3/setup.cfg
-drwxr-xr-x   0 danipower   (501) staff       (20)        0 2023-06-26 04:43:21.266950 judini-0.0.3/src/
-drwxr-xr-x   0 danipower   (501) staff       (20)        0 2023-06-26 04:43:21.269004 judini-0.0.3/src/judini/
--rw-r--r--   0 danipower   (501) staff       (20)        0 2023-06-25 22:06:54.000000 judini-0.0.3/src/judini/__init__.py
--rw-r--r--   0 danipower   (501) staff       (20)     1109 2023-06-26 04:38:50.000000 judini-0.0.3/src/judini/agent.py
-drwxr-xr-x   0 danipower   (501) staff       (20)        0 2023-06-26 04:43:21.270212 judini-0.0.3/src/judini.egg-info/
--rw-r--r--   0 danipower   (501) staff       (20)     1438 2023-06-26 04:43:21.000000 judini-0.0.3/src/judini.egg-info/PKG-INFO
--rw-r--r--   0 danipower   (501) staff       (20)      221 2023-06-26 04:43:21.000000 judini-0.0.3/src/judini.egg-info/SOURCES.txt
--rw-r--r--   0 danipower   (501) staff       (20)        1 2023-06-26 04:43:21.000000 judini-0.0.3/src/judini.egg-info/dependency_links.txt
--rw-r--r--   0 danipower   (501) staff       (20)        7 2023-06-26 04:43:21.000000 judini-0.0.3/src/judini.egg-info/top_level.txt
+drwxr-xr-x   0 danipower   (501) staff       (20)        0 2023-06-26 04:48:55.091369 judini-0.0.4/
+-rw-r--r--   0 danipower   (501) staff       (20)     1073 2023-06-25 22:23:04.000000 judini-0.0.4/LICENSE
+-rw-r--r--   0 danipower   (501) staff       (20)     1444 2023-06-26 04:48:55.091489 judini-0.0.4/PKG-INFO
+-rw-r--r--   0 danipower   (501) staff       (20)     1019 2023-06-26 04:48:43.000000 judini-0.0.4/README.md
+-rw-r--r--   0 danipower   (501) staff       (20)      119 2023-06-26 04:06:55.000000 judini-0.0.4/pyproject.toml
+-rw-r--r--   0 danipower   (501) staff       (20)      662 2023-06-26 04:48:55.092002 judini-0.0.4/setup.cfg
+drwxr-xr-x   0 danipower   (501) staff       (20)        0 2023-06-26 04:48:55.087473 judini-0.0.4/src/
+drwxr-xr-x   0 danipower   (501) staff       (20)        0 2023-06-26 04:48:55.089578 judini-0.0.4/src/judini/
+-rw-r--r--   0 danipower   (501) staff       (20)        0 2023-06-25 22:06:54.000000 judini-0.0.4/src/judini/__init__.py
+-rw-r--r--   0 danipower   (501) staff       (20)     1131 2023-06-26 04:48:06.000000 judini-0.0.4/src/judini/agent.py
+drwxr-xr-x   0 danipower   (501) staff       (20)        0 2023-06-26 04:48:55.091131 judini-0.0.4/src/judini.egg-info/
+-rw-r--r--   0 danipower   (501) staff       (20)     1444 2023-06-26 04:48:55.000000 judini-0.0.4/src/judini.egg-info/PKG-INFO
+-rw-r--r--   0 danipower   (501) staff       (20)      221 2023-06-26 04:48:55.000000 judini-0.0.4/src/judini.egg-info/SOURCES.txt
+-rw-r--r--   0 danipower   (501) staff       (20)        1 2023-06-26 04:48:55.000000 judini-0.0.4/src/judini.egg-info/dependency_links.txt
+-rw-r--r--   0 danipower   (501) staff       (20)        7 2023-06-26 04:48:55.000000 judini-0.0.4/src/judini.egg-info/top_level.txt
```

### Comparing `judini-0.0.3/LICENSE` & `judini-0.0.4/LICENSE`

 * *Files identical despite different names*

### Comparing `judini-0.0.3/PKG-INFO` & `judini-0.0.4/README.md`

 * *Files 16% similar despite different names*

```diff
@@ -1,21 +1,7 @@
-Metadata-Version: 2.1
-Name: judini
-Version: 0.0.3
-Summary: Judini python package
-Home-page: https://github.com/JudiniLabs/judini-python.git
-Author: Daniel Avila
-Author-email: daniel@judini.ai
-Classifier: Programming Language :: Python :: 3
-Classifier: License :: OSI Approved :: MIT License
-Classifier: Operating System :: OS Independent
-Requires-Python: >=3.6
-Description-Content-Type: text/markdown
-License-File: LICENSE
-
 # Judini Python Package
 This package provides you with an easy way to interact with the Judini API in your Python applications.
 
 ## Install
 To install the package, simply run the following command:
 
 ```bash 
@@ -40,16 +26,16 @@
     # Optional: update API key or URL ID if needed
     agent_instance.set_api_key("new_api_key")
     agent_instance.set_agent_id("new_agent_id")
 
     # Create the prompt
     prompt = "Who is the President of the United States?"
 
-    # Make a POST request
+    # Make a completion request
     response = agent_instance.completion(prompt)
 
     # Handle the response as needed
     print(response)
 
 if __name__ == "__main__":
     main()
-```
+```
```

### Comparing `judini-0.0.3/setup.cfg` & `judini-0.0.4/setup.cfg`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = judini
-version = 0.0.3
+version = 0.0.4
 author = Daniel Avila
 author_email = daniel@judini.ai
 description = Judini python package
 long_description = file: README.md
 long_description_content_type = text/markdown
 url = https://github.com/JudiniLabs/judini-python.git
 classifiers =
```

### Comparing `judini-0.0.3/src/judini/agent.py` & `judini-0.0.4/src/judini/agent.py`

 * *Files 17% similar despite different names*

```diff
@@ -25,14 +25,15 @@
                 {
                     "role": "user",
                     "content": prompt
                 }
             ]
         }
         response = requests.post(url, json=data, headers=headers)
+        raw_data = ''
         for chunk in response.iter_content(chunk_size=1024):
             if chunk:
                 raw_data += chunk.decode('utf-8')
 
         raw_data = raw_data.replace("data: ", '')
         raw_data = raw_data.replace("\n", '')
         raw_data = raw_data.replace("[DONE]", '')
```

### Comparing `judini-0.0.3/src/judini.egg-info/PKG-INFO` & `judini-0.0.4/PKG-INFO`

 * *Files 17% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: judini
-Version: 0.0.3
+Version: 0.0.4
 Summary: Judini python package
 Home-page: https://github.com/JudiniLabs/judini-python.git
 Author: Daniel Avila
 Author-email: daniel@judini.ai
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
@@ -40,15 +40,15 @@
     # Optional: update API key or URL ID if needed
     agent_instance.set_api_key("new_api_key")
     agent_instance.set_agent_id("new_agent_id")
 
     # Create the prompt
     prompt = "Who is the President of the United States?"
 
-    # Make a POST request
+    # Make a completion request
     response = agent_instance.completion(prompt)
 
     # Handle the response as needed
     print(response)
 
 if __name__ == "__main__":
     main()
```

