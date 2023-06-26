# Comparing `tmp/judini-0.0.7.tar.gz` & `tmp/judini-0.0.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "judini-0.0.7.tar", last modified: Mon Jun 26 21:16:55 2023, max compression
+gzip compressed data, was "judini-0.0.8.tar", last modified: Mon Jun 26 21:48:36 2023, max compression
```

## Comparing `judini-0.0.7.tar` & `judini-0.0.8.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxr-xr-x   0 danipower   (501) staff       (20)        0 2023-06-26 21:16:55.657210 judini-0.0.7/
--rw-r--r--   0 danipower   (501) staff       (20)     1073 2023-06-25 22:23:04.000000 judini-0.0.7/LICENSE
--rw-r--r--   0 danipower   (501) staff       (20)     1458 2023-06-26 21:16:55.657337 judini-0.0.7/PKG-INFO
--rw-r--r--   0 danipower   (501) staff       (20)     1033 2023-06-26 19:49:33.000000 judini-0.0.7/README.md
--rw-r--r--   0 danipower   (501) staff       (20)      119 2023-06-26 05:00:34.000000 judini-0.0.7/pyproject.toml
--rw-r--r--   0 danipower   (501) staff       (20)      662 2023-06-26 21:16:55.657857 judini-0.0.7/setup.cfg
-drwxr-xr-x   0 danipower   (501) staff       (20)        0 2023-06-26 21:16:55.652856 judini-0.0.7/src/
-drwxr-xr-x   0 danipower   (501) staff       (20)        0 2023-06-26 21:16:55.654887 judini-0.0.7/src/judini/
--rw-r--r--   0 danipower   (501) staff       (20)        0 2023-06-25 22:06:54.000000 judini-0.0.7/src/judini/__init__.py
--rw-r--r--   0 danipower   (501) staff       (20)     1839 2023-06-26 21:16:31.000000 judini-0.0.7/src/judini/agent.py
-drwxr-xr-x   0 danipower   (501) staff       (20)        0 2023-06-26 21:16:55.656353 judini-0.0.7/src/judini.egg-info/
--rw-r--r--   0 danipower   (501) staff       (20)     1458 2023-06-26 21:16:55.000000 judini-0.0.7/src/judini.egg-info/PKG-INFO
--rw-r--r--   0 danipower   (501) staff       (20)      241 2023-06-26 21:16:55.000000 judini-0.0.7/src/judini.egg-info/SOURCES.txt
--rw-r--r--   0 danipower   (501) staff       (20)        1 2023-06-26 21:16:55.000000 judini-0.0.7/src/judini.egg-info/dependency_links.txt
--rw-r--r--   0 danipower   (501) staff       (20)        7 2023-06-26 21:16:55.000000 judini-0.0.7/src/judini.egg-info/top_level.txt
-drwxr-xr-x   0 danipower   (501) staff       (20)        0 2023-06-26 21:16:55.656650 judini-0.0.7/tests/
--rw-r--r--   0 danipower   (501) staff       (20)      520 2023-06-26 19:24:22.000000 judini-0.0.7/tests/test_agent.py
+drwxr-xr-x   0 danipower   (501) staff       (20)        0 2023-06-26 21:48:36.733667 judini-0.0.8/
+-rw-r--r--   0 danipower   (501) staff       (20)     1073 2023-06-25 22:23:04.000000 judini-0.0.8/LICENSE
+-rw-r--r--   0 danipower   (501) staff       (20)     1458 2023-06-26 21:48:36.733809 judini-0.0.8/PKG-INFO
+-rw-r--r--   0 danipower   (501) staff       (20)     1033 2023-06-26 19:49:33.000000 judini-0.0.8/README.md
+-rw-r--r--   0 danipower   (501) staff       (20)      119 2023-06-26 05:00:34.000000 judini-0.0.8/pyproject.toml
+-rw-r--r--   0 danipower   (501) staff       (20)      662 2023-06-26 21:48:36.734372 judini-0.0.8/setup.cfg
+drwxr-xr-x   0 danipower   (501) staff       (20)        0 2023-06-26 21:48:36.729024 judini-0.0.8/src/
+drwxr-xr-x   0 danipower   (501) staff       (20)        0 2023-06-26 21:48:36.731007 judini-0.0.8/src/judini/
+-rw-r--r--   0 danipower   (501) staff       (20)        0 2023-06-25 22:06:54.000000 judini-0.0.8/src/judini/__init__.py
+-rw-r--r--   0 danipower   (501) staff       (20)     1898 2023-06-26 21:43:33.000000 judini-0.0.8/src/judini/agent.py
+drwxr-xr-x   0 danipower   (501) staff       (20)        0 2023-06-26 21:48:36.732859 judini-0.0.8/src/judini.egg-info/
+-rw-r--r--   0 danipower   (501) staff       (20)     1458 2023-06-26 21:48:36.000000 judini-0.0.8/src/judini.egg-info/PKG-INFO
+-rw-r--r--   0 danipower   (501) staff       (20)      241 2023-06-26 21:48:36.000000 judini-0.0.8/src/judini.egg-info/SOURCES.txt
+-rw-r--r--   0 danipower   (501) staff       (20)        1 2023-06-26 21:48:36.000000 judini-0.0.8/src/judini.egg-info/dependency_links.txt
+-rw-r--r--   0 danipower   (501) staff       (20)        7 2023-06-26 21:48:36.000000 judini-0.0.8/src/judini.egg-info/top_level.txt
+drwxr-xr-x   0 danipower   (501) staff       (20)        0 2023-06-26 21:48:36.733182 judini-0.0.8/tests/
+-rw-r--r--   0 danipower   (501) staff       (20)      520 2023-06-26 19:24:22.000000 judini-0.0.8/tests/test_agent.py
```

### Comparing `judini-0.0.7/LICENSE` & `judini-0.0.8/LICENSE`

 * *Files identical despite different names*

### Comparing `judini-0.0.7/PKG-INFO` & `judini-0.0.8/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: judini
-Version: 0.0.7
+Version: 0.0.8
 Summary: Judini python package
 Home-page: https://github.com/JudiniLabs/judini-python.git
 Author: Daniel Avila
 Author-email: daniel@judini.ai
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `judini-0.0.7/README.md` & `judini-0.0.8/README.md`

 * *Files identical despite different names*

### Comparing `judini-0.0.7/setup.cfg` & `judini-0.0.8/setup.cfg`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = judini
-version = 0.0.7
+version = 0.0.8
 author = Daniel Avila
 author_email = daniel@judini.ai
 description = Judini python package
 long_description = file: README.md
 long_description_content_type = text/markdown
 url = https://github.com/JudiniLabs/judini-python.git
 classifiers =
```

### Comparing `judini-0.0.7/src/judini/agent.py` & `judini-0.0.8/src/judini/agent.py`

 * *Files 10% similar despite different names*

```diff
@@ -26,15 +26,16 @@
                 {
                     "role": "user",
                     "content": prompt
                 }
             ]
         }
         response = requests.post(url, json=data, headers=headers)
-        tokens = 'Response: '
+        tokens = ''
+        error = ''
         if(stream == False):
             for chunk in response.iter_content(chunk_size=1024):
                 if chunk:
                     raw_data = chunk.decode('utf-8').replace("data: ", '')
                     if raw_data != "":
                         lines = raw_data.strip().splitlines()
                         for line in lines:
@@ -42,12 +43,13 @@
                             if line and line != "[DONE]":
                                 try:
                                     json_object = json.loads(line)
                                     result = json_object['data']
                                     result = result.replace("\n", "")
                                     tokens += result
                                 except json.JSONDecodeError:
-                                    print(f'Error al decodificar el objeto JSON en la línea: {line}')    
+                                    error = line
+                                    #print(f'Error al decodificar el objeto JSON en la línea: {line}')    
         else:
             return response
         
         return tokens
```

### Comparing `judini-0.0.7/src/judini.egg-info/PKG-INFO` & `judini-0.0.8/src/judini.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: judini
-Version: 0.0.7
+Version: 0.0.8
 Summary: Judini python package
 Home-page: https://github.com/JudiniLabs/judini-python.git
 Author: Daniel Avila
 Author-email: daniel@judini.ai
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `judini-0.0.7/tests/test_agent.py` & `judini-0.0.8/tests/test_agent.py`

 * *Files identical despite different names*

