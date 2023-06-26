# Comparing `tmp/chatgpt_functions-0.0.4.tar.gz` & `tmp/chatgpt_functions-0.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "chatgpt_functions-0.0.4.tar", last modified: Mon Jun 26 15:01:36 2023, max compression
+gzip compressed data, was "chatgpt_functions-0.0.5.tar", last modified: Mon Jun 26 15:07:50 2023, max compression
```

## Comparing `chatgpt_functions-0.0.4.tar` & `chatgpt_functions-0.0.5.tar`

### file list

```diff
@@ -1,13 +1,19 @@
-drwxrwxrwx   0        0        0        0 2023-06-26 15:01:36.481387 chatgpt_functions-0.0.4/
--rw-rw-rw-   0        0        0     1091 2023-06-26 13:13:15.000000 chatgpt_functions-0.0.4/LICENSE
--rw-rw-rw-   0        0        0     1935 2023-06-26 15:01:36.481387 chatgpt_functions-0.0.4/PKG-INFO
--rw-rw-rw-   0        0        0     1374 2023-06-26 12:54:41.000000 chatgpt_functions-0.0.4/README.md
-drwxrwxrwx   0        0        0        0 2023-06-26 15:01:36.479388 chatgpt_functions-0.0.4/chatgpt_functions.egg-info/
--rw-rw-rw-   0        0        0     1935 2023-06-26 15:01:36.000000 chatgpt_functions-0.0.4/chatgpt_functions.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      255 2023-06-26 15:01:36.000000 chatgpt_functions-0.0.4/chatgpt_functions.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-26 15:01:36.000000 chatgpt_functions-0.0.4/chatgpt_functions.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       36 2023-06-26 15:01:36.000000 chatgpt_functions-0.0.4/chatgpt_functions.egg-info/requires.txt
--rw-rw-rw-   0        0        0        1 2023-06-26 15:01:36.000000 chatgpt_functions-0.0.4/chatgpt_functions.egg-info/top_level.txt
--rw-rw-rw-   0        0        0      682 2023-06-26 14:36:57.000000 chatgpt_functions-0.0.4/pyproject.toml
--rw-rw-rw-   0        0        0       42 2023-06-26 15:01:36.484906 chatgpt_functions-0.0.4/setup.cfg
--rw-rw-rw-   0        0        0      875 2023-06-26 14:59:48.000000 chatgpt_functions-0.0.4/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-26 15:07:50.534144 chatgpt_functions-0.0.5/
+-rw-rw-rw-   0        0        0     1091 2023-06-26 13:13:15.000000 chatgpt_functions-0.0.5/LICENSE
+-rw-rw-rw-   0        0        0     1935 2023-06-26 15:07:50.534144 chatgpt_functions-0.0.5/PKG-INFO
+-rw-rw-rw-   0        0        0     1374 2023-06-26 12:54:41.000000 chatgpt_functions-0.0.5/README.md
+drwxrwxrwx   0        0        0        0 2023-06-26 15:07:50.516627 chatgpt_functions-0.0.5/chatgpt_functions/
+-rw-rw-rw-   0        0        0       83 2023-06-26 13:35:12.000000 chatgpt_functions-0.0.5/chatgpt_functions/__init__.py
+-rw-rw-rw-   0        0        0     2060 2023-06-26 12:52:30.000000 chatgpt_functions-0.0.5/chatgpt_functions/chatgpt.py
+-rw-rw-rw-   0        0        0      722 2023-06-26 11:01:56.000000 chatgpt_functions-0.0.5/chatgpt_functions/chatgpt_function.py
+-rw-rw-rw-   0        0        0      448 2023-06-26 09:48:36.000000 chatgpt_functions-0.0.5/chatgpt_functions/chatgpt_types.py
+-rw-rw-rw-   0        0        0     1319 2023-06-26 12:53:31.000000 chatgpt_functions-0.0.5/chatgpt_functions/function_parameters.py
+drwxrwxrwx   0        0        0        0 2023-06-26 15:07:50.532145 chatgpt_functions-0.0.5/chatgpt_functions.egg-info/
+-rw-rw-rw-   0        0        0     1935 2023-06-26 15:07:50.000000 chatgpt_functions-0.0.5/chatgpt_functions.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      428 2023-06-26 15:07:50.000000 chatgpt_functions-0.0.5/chatgpt_functions.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-26 15:07:50.000000 chatgpt_functions-0.0.5/chatgpt_functions.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       36 2023-06-26 15:07:50.000000 chatgpt_functions-0.0.5/chatgpt_functions.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       18 2023-06-26 15:07:50.000000 chatgpt_functions-0.0.5/chatgpt_functions.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0      682 2023-06-26 14:36:57.000000 chatgpt_functions-0.0.5/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2023-06-26 15:07:50.536662 chatgpt_functions-0.0.5/setup.cfg
+-rw-rw-rw-   0        0        0      875 2023-06-26 15:06:32.000000 chatgpt_functions-0.0.5/setup.py
```

### Comparing `chatgpt_functions-0.0.4/LICENSE` & `chatgpt_functions-0.0.5/LICENSE`

 * *Files identical despite different names*

### Comparing `chatgpt_functions-0.0.4/PKG-INFO` & `chatgpt_functions-0.0.5/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: chatgpt_functions
-Version: 0.0.4
+Version: 0.0.5
 Summary: Wrapper over the gpt3.5 model, capable of calling functions
 Home-page: https://github.com/Wellmare/chatgpt-functions
 Author: Wellmare
 Author-email: ivan.kolipov@gmail.com
 Keywords: chatgpt functions gpt
 Classifier: Programming Language :: Python :: 3.10
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `chatgpt_functions-0.0.4/README.md` & `chatgpt_functions-0.0.5/README.md`

 * *Files identical despite different names*

### Comparing `chatgpt_functions-0.0.4/chatgpt_functions.egg-info/PKG-INFO` & `chatgpt_functions-0.0.5/chatgpt_functions.egg-info/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: chatgpt-functions
-Version: 0.0.4
+Version: 0.0.5
 Summary: Wrapper over the gpt3.5 model, capable of calling functions
 Home-page: https://github.com/Wellmare/chatgpt-functions
 Author: Wellmare
 Author-email: ivan.kolipov@gmail.com
 Keywords: chatgpt functions gpt
 Classifier: Programming Language :: Python :: 3.10
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `chatgpt_functions-0.0.4/pyproject.toml` & `chatgpt_functions-0.0.5/pyproject.toml`

 * *Files identical despite different names*

### Comparing `chatgpt_functions-0.0.4/setup.py` & `chatgpt_functions-0.0.5/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 def readme():
     with open("README.md", "r") as f:
         return f.read()
 
 
 setup(
     name="chatgpt_functions",
-    version="0.0.4",
+    version="0.0.5",
     author="Wellmare",
     author_email="ivan.kolipov@gmail.com",
     description="Wrapper over the gpt3.5 model, capable of calling functions",
     long_description=readme(),
     long_description_content_type="text/markdown",
     url="https://github.com/Wellmare/chatgpt-functions",
     packages=find_packages(),
```

