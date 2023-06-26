# Comparing `tmp/judini-0.0.5.tar.gz` & `tmp/judini-0.0.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "judini-0.0.5.tar", last modified: Mon Jun 26 05:01:20 2023, max compression
+gzip compressed data, was "judini-0.0.6.tar", last modified: Mon Jun 26 19:50:00 2023, max compression
```

## Comparing `judini-0.0.5.tar` & `judini-0.0.6.tar`

### file list

```diff
@@ -1,15 +1,17 @@
-drwxr-xr-x   0 danipower   (501) staff       (20)        0 2023-06-26 05:01:20.091215 judini-0.0.5/
--rw-r--r--   0 danipower   (501) staff       (20)     1073 2023-06-25 22:23:04.000000 judini-0.0.5/LICENSE
--rw-r--r--   0 danipower   (501) staff       (20)     1444 2023-06-26 05:01:20.091335 judini-0.0.5/PKG-INFO
--rw-r--r--   0 danipower   (501) staff       (20)     1019 2023-06-26 04:48:43.000000 judini-0.0.5/README.md
--rw-r--r--   0 danipower   (501) staff       (20)      119 2023-06-26 05:00:34.000000 judini-0.0.5/pyproject.toml
--rw-r--r--   0 danipower   (501) staff       (20)      662 2023-06-26 05:01:20.091892 judini-0.0.5/setup.cfg
-drwxr-xr-x   0 danipower   (501) staff       (20)        0 2023-06-26 05:01:20.087888 judini-0.0.5/src/
-drwxr-xr-x   0 danipower   (501) staff       (20)        0 2023-06-26 05:01:20.089483 judini-0.0.5/src/judini/
--rw-r--r--   0 danipower   (501) staff       (20)        0 2023-06-25 22:06:54.000000 judini-0.0.5/src/judini/__init__.py
--rw-r--r--   0 danipower   (501) staff       (20)     1331 2023-06-26 04:59:30.000000 judini-0.0.5/src/judini/agent.py
-drwxr-xr-x   0 danipower   (501) staff       (20)        0 2023-06-26 05:01:20.090905 judini-0.0.5/src/judini.egg-info/
--rw-r--r--   0 danipower   (501) staff       (20)     1444 2023-06-26 05:01:20.000000 judini-0.0.5/src/judini.egg-info/PKG-INFO
--rw-r--r--   0 danipower   (501) staff       (20)      221 2023-06-26 05:01:20.000000 judini-0.0.5/src/judini.egg-info/SOURCES.txt
--rw-r--r--   0 danipower   (501) staff       (20)        1 2023-06-26 05:01:20.000000 judini-0.0.5/src/judini.egg-info/dependency_links.txt
--rw-r--r--   0 danipower   (501) staff       (20)        7 2023-06-26 05:01:20.000000 judini-0.0.5/src/judini.egg-info/top_level.txt
+drwxr-xr-x   0 danipower   (501) staff       (20)        0 2023-06-26 19:50:00.149537 judini-0.0.6/
+-rw-r--r--   0 danipower   (501) staff       (20)     1073 2023-06-25 22:23:04.000000 judini-0.0.6/LICENSE
+-rw-r--r--   0 danipower   (501) staff       (20)     1458 2023-06-26 19:50:00.149664 judini-0.0.6/PKG-INFO
+-rw-r--r--   0 danipower   (501) staff       (20)     1033 2023-06-26 19:49:33.000000 judini-0.0.6/README.md
+-rw-r--r--   0 danipower   (501) staff       (20)      119 2023-06-26 05:00:34.000000 judini-0.0.6/pyproject.toml
+-rw-r--r--   0 danipower   (501) staff       (20)      662 2023-06-26 19:50:00.150181 judini-0.0.6/setup.cfg
+drwxr-xr-x   0 danipower   (501) staff       (20)        0 2023-06-26 19:50:00.144799 judini-0.0.6/src/
+drwxr-xr-x   0 danipower   (501) staff       (20)        0 2023-06-26 19:50:00.147057 judini-0.0.6/src/judini/
+-rw-r--r--   0 danipower   (501) staff       (20)        0 2023-06-25 22:06:54.000000 judini-0.0.6/src/judini/__init__.py
+-rw-r--r--   0 danipower   (501) staff       (20)     1573 2023-06-26 19:48:26.000000 judini-0.0.6/src/judini/agent.py
+drwxr-xr-x   0 danipower   (501) staff       (20)        0 2023-06-26 19:50:00.148538 judini-0.0.6/src/judini.egg-info/
+-rw-r--r--   0 danipower   (501) staff       (20)     1458 2023-06-26 19:50:00.000000 judini-0.0.6/src/judini.egg-info/PKG-INFO
+-rw-r--r--   0 danipower   (501) staff       (20)      241 2023-06-26 19:50:00.000000 judini-0.0.6/src/judini.egg-info/SOURCES.txt
+-rw-r--r--   0 danipower   (501) staff       (20)        1 2023-06-26 19:50:00.000000 judini-0.0.6/src/judini.egg-info/dependency_links.txt
+-rw-r--r--   0 danipower   (501) staff       (20)        7 2023-06-26 19:50:00.000000 judini-0.0.6/src/judini.egg-info/top_level.txt
+drwxr-xr-x   0 danipower   (501) staff       (20)        0 2023-06-26 19:50:00.148820 judini-0.0.6/tests/
+-rw-r--r--   0 danipower   (501) staff       (20)      520 2023-06-26 19:24:22.000000 judini-0.0.6/tests/test_agent.py
```

### Comparing `judini-0.0.5/LICENSE` & `judini-0.0.6/LICENSE`

 * *Files identical despite different names*

### Comparing `judini-0.0.5/PKG-INFO` & `judini-0.0.6/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: judini
-Version: 0.0.5
+Version: 0.0.6
 Summary: Judini python package
 Home-page: https://github.com/JudiniLabs/judini-python.git
 Author: Daniel Avila
 Author-email: daniel@judini.ai
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
@@ -41,15 +41,15 @@
     agent_instance.set_api_key("new_api_key")
     agent_instance.set_agent_id("new_agent_id")
 
     # Create the prompt
     prompt = "Who is the President of the United States?"
 
     # Make a completion request
-    response = agent_instance.completion(prompt)
+    response = agent_instance.completion(prompt, stream=False)
 
     # Handle the response as needed
     print(response)
 
 if __name__ == "__main__":
     main()
 ```
```

### Comparing `judini-0.0.5/README.md` & `judini-0.0.6/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -27,15 +27,15 @@
     agent_instance.set_api_key("new_api_key")
     agent_instance.set_agent_id("new_agent_id")
 
     # Create the prompt
     prompt = "Who is the President of the United States?"
 
     # Make a completion request
-    response = agent_instance.completion(prompt)
+    response = agent_instance.completion(prompt, stream=False)
 
     # Handle the response as needed
     print(response)
 
 if __name__ == "__main__":
     main()
 ```
```

### Comparing `judini-0.0.5/setup.cfg` & `judini-0.0.6/setup.cfg`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = judini
-version = 0.0.5
+version = 0.0.6
 author = Daniel Avila
 author_email = daniel@judini.ai
 description = Judini python package
 long_description = file: README.md
 long_description_content_type = text/markdown
 url = https://github.com/JudiniLabs/judini-python.git
 classifiers =
```

### Comparing `judini-0.0.5/src/judini/agent.py` & `judini-0.0.6/src/judini/agent.py`

 * *Files 10% similar despite different names*

```diff
@@ -9,15 +9,15 @@
 
     def set_api_key(self, api_key):
         self.api_key = api_key
 
     def set_agent_id(self, agent_id):
         self.agent_id = agent_id
 
-    def completion(self, prompt):
+    def completion(self, prompt, stream=False):
         # Headers
         headers = {
             "Content-Type": "application/json",
             "Authorization": f"Bearer {self.api_key}"
         }
         # Endpoint
         url = 'https://playground.judini.ai/api/v1/agent/'+ self.agent_id
@@ -26,19 +26,24 @@
                 {
                     "role": "user",
                     "content": prompt
                 }
             ]
         }
         response = requests.post(url, json=data, headers=headers)
-        token = ''
-        for chunk in response.iter_content(chunk_size=1024):
-            if chunk:
-                raw_data = chunk.decode('utf-8').replace("data: ", '')
-                if raw_data != "[DONE]":
-                    try:
-                        json_object = json.loads(raw_data.strip())
-                        token += json_object['data']
-                    except json.JSONDecodeError as e:
-                        # TODO: fix this error
-                        error= e
-        return token
+        tokens = ''
+        report = []
+        if(stream == False):
+            for chunk in response.iter_content(chunk_size=1024):
+                if chunk:
+                    raw_data = chunk.decode('utf-8').replace("data: ", '')
+                    if "[DONE]" in raw_data or raw_data != "":
+                        try:
+                            json_object = json.loads(raw_data.strip())
+                            result = json_object['data']
+                            result = result.replace("\n", "")        
+                            tokens += result
+                        except json.JSONDecodeError as e:
+                            print('error', e)
+            return tokens
+        else:
+            return response
```

### Comparing `judini-0.0.5/src/judini.egg-info/PKG-INFO` & `judini-0.0.6/src/judini.egg-info/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: judini
-Version: 0.0.5
+Version: 0.0.6
 Summary: Judini python package
 Home-page: https://github.com/JudiniLabs/judini-python.git
 Author: Daniel Avila
 Author-email: daniel@judini.ai
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
@@ -41,15 +41,15 @@
     agent_instance.set_api_key("new_api_key")
     agent_instance.set_agent_id("new_agent_id")
 
     # Create the prompt
     prompt = "Who is the President of the United States?"
 
     # Make a completion request
-    response = agent_instance.completion(prompt)
+    response = agent_instance.completion(prompt, stream=False)
 
     # Handle the response as needed
     print(response)
 
 if __name__ == "__main__":
     main()
 ```
```

