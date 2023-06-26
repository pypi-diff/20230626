# Comparing `tmp/chatgpt_functions-0.0.3.tar.gz` & `tmp/chatgpt_functions-0.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "chatgpt_functions-0.0.3.tar", last modified: Mon Jun 26 14:38:11 2023, max compression
+gzip compressed data, was "chatgpt_functions-0.0.4.tar", last modified: Mon Jun 26 15:01:36 2023, max compression
```

## Comparing `chatgpt_functions-0.0.3.tar` & `chatgpt_functions-0.0.4.tar`

### file list

```diff
@@ -1,14 +1,13 @@
-drwxrwxrwx   0        0        0        0 2023-06-26 14:38:11.228014 chatgpt_functions-0.0.3/
--rw-rw-rw-   0        0        0     1091 2023-06-26 13:13:15.000000 chatgpt_functions-0.0.3/LICENSE
--rw-rw-rw-   0        0        0     1865 2023-06-26 14:38:11.228014 chatgpt_functions-0.0.3/PKG-INFO
--rw-rw-rw-   0        0        0     1374 2023-06-26 12:54:41.000000 chatgpt_functions-0.0.3/README.md
-drwxrwxrwx   0        0        0        0 2023-06-26 14:38:11.226008 chatgpt_functions-0.0.3/chatgpt_functions.egg-info/
--rw-rw-rw-   0        0        0     1865 2023-06-26 14:38:11.000000 chatgpt_functions-0.0.3/chatgpt_functions.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      291 2023-06-26 14:38:11.000000 chatgpt_functions-0.0.3/chatgpt_functions.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-26 14:38:11.000000 chatgpt_functions-0.0.3/chatgpt_functions.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       36 2023-06-26 14:38:11.000000 chatgpt_functions-0.0.3/chatgpt_functions.egg-info/requires.txt
--rw-rw-rw-   0        0        0        1 2023-06-26 14:38:11.000000 chatgpt_functions-0.0.3/chatgpt_functions.egg-info/top_level.txt
--rw-rw-rw-   0        0        0        2 2023-06-26 14:38:11.000000 chatgpt_functions-0.0.3/chatgpt_functions.egg-info/zip-safe
--rw-rw-rw-   0        0        0      682 2023-06-26 14:36:57.000000 chatgpt_functions-0.0.3/pyproject.toml
--rw-rw-rw-   0        0        0      690 2023-06-26 14:38:11.230015 chatgpt_functions-0.0.3/setup.cfg
--rw-rw-rw-   0        0        0       39 2023-06-26 14:27:24.000000 chatgpt_functions-0.0.3/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-26 15:01:36.481387 chatgpt_functions-0.0.4/
+-rw-rw-rw-   0        0        0     1091 2023-06-26 13:13:15.000000 chatgpt_functions-0.0.4/LICENSE
+-rw-rw-rw-   0        0        0     1935 2023-06-26 15:01:36.481387 chatgpt_functions-0.0.4/PKG-INFO
+-rw-rw-rw-   0        0        0     1374 2023-06-26 12:54:41.000000 chatgpt_functions-0.0.4/README.md
+drwxrwxrwx   0        0        0        0 2023-06-26 15:01:36.479388 chatgpt_functions-0.0.4/chatgpt_functions.egg-info/
+-rw-rw-rw-   0        0        0     1935 2023-06-26 15:01:36.000000 chatgpt_functions-0.0.4/chatgpt_functions.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      255 2023-06-26 15:01:36.000000 chatgpt_functions-0.0.4/chatgpt_functions.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-26 15:01:36.000000 chatgpt_functions-0.0.4/chatgpt_functions.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       36 2023-06-26 15:01:36.000000 chatgpt_functions-0.0.4/chatgpt_functions.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        1 2023-06-26 15:01:36.000000 chatgpt_functions-0.0.4/chatgpt_functions.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0      682 2023-06-26 14:36:57.000000 chatgpt_functions-0.0.4/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2023-06-26 15:01:36.484906 chatgpt_functions-0.0.4/setup.cfg
+-rw-rw-rw-   0        0        0      875 2023-06-26 14:59:48.000000 chatgpt_functions-0.0.4/setup.py
```

### Comparing `chatgpt_functions-0.0.3/LICENSE` & `chatgpt_functions-0.0.4/LICENSE`

 * *Files identical despite different names*

### Comparing `chatgpt_functions-0.0.3/PKG-INFO` & `chatgpt_functions-0.0.4/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,18 +1,19 @@
 Metadata-Version: 2.1
 Name: chatgpt_functions
-Version: 0.0.3
+Version: 0.0.4
 Summary: Wrapper over the gpt3.5 model, capable of calling functions
 Home-page: https://github.com/Wellmare/chatgpt-functions
 Author: Wellmare
 Author-email: ivan.kolipov@gmail.com
-Classifier: Programming Language :: Python :: 3
+Keywords: chatgpt functions gpt
+Classifier: Programming Language :: Python :: 3.10
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
-Requires-Python: >=3.7.1
+Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # Example of usage:
 ```python
 import asyncio
 from chatgpt_functions import (
@@ -50,15 +51,15 @@
                             description="Greeting",
                         ),
                     ]
                 ),
                 function_description="Say hello to user",
             )
         ],
-        messages=[Message(role=Roles.USER, content='Скажи приветик миче')]
+        messages=[Message(role=Roles.USER, content='РЎРєР°Р¶Рё РїСЂРёРІРµС‚РёРє РјРёС‡Рµ')]
     )
 
 
 loop = asyncio.new_event_loop()
 asyncio.set_event_loop(loop)
 loop.run_until_complete(main())
 ```
```

### Comparing `chatgpt_functions-0.0.3/README.md` & `chatgpt_functions-0.0.4/README.md`

 * *Files identical despite different names*

### Comparing `chatgpt_functions-0.0.3/chatgpt_functions.egg-info/PKG-INFO` & `chatgpt_functions-0.0.4/chatgpt_functions.egg-info/PKG-INFO`

 * *Files 19% similar despite different names*

```diff
@@ -1,18 +1,19 @@
 Metadata-Version: 2.1
 Name: chatgpt-functions
-Version: 0.0.3
+Version: 0.0.4
 Summary: Wrapper over the gpt3.5 model, capable of calling functions
 Home-page: https://github.com/Wellmare/chatgpt-functions
 Author: Wellmare
 Author-email: ivan.kolipov@gmail.com
-Classifier: Programming Language :: Python :: 3
+Keywords: chatgpt functions gpt
+Classifier: Programming Language :: Python :: 3.10
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
-Requires-Python: >=3.7.1
+Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # Example of usage:
 ```python
 import asyncio
 from chatgpt_functions import (
@@ -50,15 +51,15 @@
                             description="Greeting",
                         ),
                     ]
                 ),
                 function_description="Say hello to user",
             )
         ],
-        messages=[Message(role=Roles.USER, content='Скажи приветик миче')]
+        messages=[Message(role=Roles.USER, content='РЎРєР°Р¶Рё РїСЂРёРІРµС‚РёРє РјРёС‡Рµ')]
     )
 
 
 loop = asyncio.new_event_loop()
 asyncio.set_event_loop(loop)
 loop.run_until_complete(main())
 ```
```

### Comparing `chatgpt_functions-0.0.3/pyproject.toml` & `chatgpt_functions-0.0.4/pyproject.toml`

 * *Files identical despite different names*

