# Comparing `tmp/judini-0.0.2.tar.gz` & `tmp/judini-0.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "judini-0.0.2.tar", last modified: Mon Jun 26 04:25:04 2023, max compression
+gzip compressed data, was "judini-0.0.3.tar", last modified: Mon Jun 26 04:43:21 2023, max compression
```

## Comparing `judini-0.0.2.tar` & `judini-0.0.3.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxr-xr-x   0 danipower   (501) staff       (20)        0 2023-06-26 04:25:04.756277 judini-0.0.2/
--rw-r--r--   0 danipower   (501) staff       (20)     1073 2023-06-25 22:23:04.000000 judini-0.0.2/LICENSE
--rw-r--r--   0 danipower   (501) staff       (20)     1177 2023-06-26 04:25:04.756410 judini-0.0.2/PKG-INFO
--rw-r--r--   0 danipower   (501) staff       (20)      752 2023-06-26 04:14:29.000000 judini-0.0.2/README.md
--rw-r--r--   0 danipower   (501) staff       (20)      119 2023-06-26 04:06:55.000000 judini-0.0.2/pyproject.toml
--rw-r--r--   0 danipower   (501) staff       (20)      662 2023-06-26 04:25:04.756916 judini-0.0.2/setup.cfg
-drwxr-xr-x   0 danipower   (501) staff       (20)        0 2023-06-26 04:25:04.752291 judini-0.0.2/src/
-drwxr-xr-x   0 danipower   (501) staff       (20)        0 2023-06-26 04:25:04.754130 judini-0.0.2/src/judini/
--rw-r--r--   0 danipower   (501) staff       (20)        0 2023-06-25 22:06:54.000000 judini-0.0.2/src/judini/__init__.py
--rw-r--r--   0 danipower   (501) staff       (20)      836 2023-06-26 04:24:20.000000 judini-0.0.2/src/judini/agent.py
-drwxr-xr-x   0 danipower   (501) staff       (20)        0 2023-06-26 04:25:04.755980 judini-0.0.2/src/judini.egg-info/
--rw-r--r--   0 danipower   (501) staff       (20)     1177 2023-06-26 04:25:04.000000 judini-0.0.2/src/judini.egg-info/PKG-INFO
--rw-r--r--   0 danipower   (501) staff       (20)      221 2023-06-26 04:25:04.000000 judini-0.0.2/src/judini.egg-info/SOURCES.txt
--rw-r--r--   0 danipower   (501) staff       (20)        1 2023-06-26 04:25:04.000000 judini-0.0.2/src/judini.egg-info/dependency_links.txt
--rw-r--r--   0 danipower   (501) staff       (20)        7 2023-06-26 04:25:04.000000 judini-0.0.2/src/judini.egg-info/top_level.txt
+drwxr-xr-x   0 danipower   (501) staff       (20)        0 2023-06-26 04:43:21.270466 judini-0.0.3/
+-rw-r--r--   0 danipower   (501) staff       (20)     1073 2023-06-25 22:23:04.000000 judini-0.0.3/LICENSE
+-rw-r--r--   0 danipower   (501) staff       (20)     1438 2023-06-26 04:43:21.270605 judini-0.0.3/PKG-INFO
+-rw-r--r--   0 danipower   (501) staff       (20)     1013 2023-06-26 04:42:21.000000 judini-0.0.3/README.md
+-rw-r--r--   0 danipower   (501) staff       (20)      119 2023-06-26 04:06:55.000000 judini-0.0.3/pyproject.toml
+-rw-r--r--   0 danipower   (501) staff       (20)      662 2023-06-26 04:43:21.271118 judini-0.0.3/setup.cfg
+drwxr-xr-x   0 danipower   (501) staff       (20)        0 2023-06-26 04:43:21.266950 judini-0.0.3/src/
+drwxr-xr-x   0 danipower   (501) staff       (20)        0 2023-06-26 04:43:21.269004 judini-0.0.3/src/judini/
+-rw-r--r--   0 danipower   (501) staff       (20)        0 2023-06-25 22:06:54.000000 judini-0.0.3/src/judini/__init__.py
+-rw-r--r--   0 danipower   (501) staff       (20)     1109 2023-06-26 04:38:50.000000 judini-0.0.3/src/judini/agent.py
+drwxr-xr-x   0 danipower   (501) staff       (20)        0 2023-06-26 04:43:21.270212 judini-0.0.3/src/judini.egg-info/
+-rw-r--r--   0 danipower   (501) staff       (20)     1438 2023-06-26 04:43:21.000000 judini-0.0.3/src/judini.egg-info/PKG-INFO
+-rw-r--r--   0 danipower   (501) staff       (20)      221 2023-06-26 04:43:21.000000 judini-0.0.3/src/judini.egg-info/SOURCES.txt
+-rw-r--r--   0 danipower   (501) staff       (20)        1 2023-06-26 04:43:21.000000 judini-0.0.3/src/judini.egg-info/dependency_links.txt
+-rw-r--r--   0 danipower   (501) staff       (20)        7 2023-06-26 04:43:21.000000 judini-0.0.3/src/judini.egg-info/top_level.txt
```

### Comparing `judini-0.0.2/LICENSE` & `judini-0.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `judini-0.0.2/PKG-INFO` & `judini-0.0.3/PKG-INFO`

 * *Files 17% similar despite different names*

```diff
@@ -1,51 +1,55 @@
 Metadata-Version: 2.1
 Name: judini
-Version: 0.0.2
+Version: 0.0.3
 Summary: Judini python package
 Home-page: https://github.com/JudiniLabs/judini-python.git
 Author: Daniel Avila
 Author-email: daniel@judini.ai
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
-# Judini python package
+# Judini Python Package
+This package provides you with an easy way to interact with the Judini API in your Python applications.
 
 ## Install
+To install the package, simply run the following command:
 
-``` pip install judini ```
-
-## Use
+```bash 
+pip install judini 
+```
 
+## Usege
+Below is a sample code demonstrating how to use the Judini package in your Python application:
 ``` python
 
-# import
-from judini import Judini
+# Import the package
+from judini import Agent
 
 def main():
     # Replace with your actual API key and URL ID
     api_key = "your_api_key_here"
     agent_id = "your_agent_id_here"
 
     # Initialize the Judini class
-    judini_instance = Judini(api_key, agent_id)
+    agent_instance = Agent(api_key, agent_id)
 
     # Optional: update API key or URL ID if needed
-    judini_instance.set_api_key("new_api_key")
-    judini_instance.set_agent_id("new_agent_id")
+    agent_instance.set_api_key("new_api_key")
+    agent_instance.set_agent_id("new_agent_id")
 
-    # create the user prompt
-    question = "Who is the President of the United States?"
+    # Create the prompt
+    prompt = "Who is the President of the United States?"
 
     # Make a POST request
-    response = judini_instance.completion(question)
+    response = agent_instance.completion(prompt)
 
     # Handle the response as needed
     print(response)
 
 if __name__ == "__main__":
     main()
 ```
```

### Comparing `judini-0.0.2/setup.cfg` & `judini-0.0.3/setup.cfg`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = judini
-version = 0.0.2
+version = 0.0.3
 author = Daniel Avila
 author_email = daniel@judini.ai
 description = Judini python package
 long_description = file: README.md
 long_description_content_type = text/markdown
 url = https://github.com/JudiniLabs/judini-python.git
 classifiers =
```

### Comparing `judini-0.0.2/src/judini.egg-info/PKG-INFO` & `judini-0.0.3/src/judini.egg-info/PKG-INFO`

 * *Files 17% similar despite different names*

```diff
@@ -1,51 +1,55 @@
 Metadata-Version: 2.1
 Name: judini
-Version: 0.0.2
+Version: 0.0.3
 Summary: Judini python package
 Home-page: https://github.com/JudiniLabs/judini-python.git
 Author: Daniel Avila
 Author-email: daniel@judini.ai
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
-# Judini python package
+# Judini Python Package
+This package provides you with an easy way to interact with the Judini API in your Python applications.
 
 ## Install
+To install the package, simply run the following command:
 
-``` pip install judini ```
-
-## Use
+```bash 
+pip install judini 
+```
 
+## Usege
+Below is a sample code demonstrating how to use the Judini package in your Python application:
 ``` python
 
-# import
-from judini import Judini
+# Import the package
+from judini import Agent
 
 def main():
     # Replace with your actual API key and URL ID
     api_key = "your_api_key_here"
     agent_id = "your_agent_id_here"
 
     # Initialize the Judini class
-    judini_instance = Judini(api_key, agent_id)
+    agent_instance = Agent(api_key, agent_id)
 
     # Optional: update API key or URL ID if needed
-    judini_instance.set_api_key("new_api_key")
-    judini_instance.set_agent_id("new_agent_id")
+    agent_instance.set_api_key("new_api_key")
+    agent_instance.set_agent_id("new_agent_id")
 
-    # create the user prompt
-    question = "Who is the President of the United States?"
+    # Create the prompt
+    prompt = "Who is the President of the United States?"
 
     # Make a POST request
-    response = judini_instance.completion(question)
+    response = agent_instance.completion(prompt)
 
     # Handle the response as needed
     print(response)
 
 if __name__ == "__main__":
     main()
 ```
```

