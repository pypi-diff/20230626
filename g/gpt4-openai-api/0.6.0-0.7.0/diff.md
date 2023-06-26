# Comparing `tmp/gpt4-openai-api-0.6.0.tar.gz` & `tmp/gpt4-openai-api-0.7.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist\gpt4-openai-api-0.6.0.tar", last modified: Wed Jun 14 11:18:49 2023, max compression
+gzip compressed data, was "dist\gpt4-openai-api-0.7.0.tar", last modified: Mon Jun 26 12:31:09 2023, max compression
```

## Comparing `gpt4-openai-api-0.6.0.tar` & `gpt4-openai-api-0.7.0.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxrwxrwx   0        0        0        0 2023-06-14 11:18:49.976379 gpt4-openai-api-0.6.0/
--rw-rw-rw-   0        0        0     6253 2023-06-14 11:18:49.975382 gpt4-openai-api-0.6.0/PKG-INFO
-drwxrwxrwx   0        0        0        0 2023-06-14 11:18:49.862381 gpt4-openai-api-0.6.0/gpt4_openai/
--rw-rw-rw-   0        0        0     1580 2023-06-14 11:17:48.000000 gpt4-openai-api-0.6.0/gpt4_openai/__init__.py
-drwxrwxrwx   0        0        0        0 2023-06-14 11:18:49.929380 gpt4-openai-api-0.6.0/gpt4_openai_api.egg-info/
--rw-rw-rw-   0        0        0     6253 2023-06-14 11:18:49.000000 gpt4-openai-api-0.6.0/gpt4_openai_api.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      358 2023-06-14 11:18:49.000000 gpt4-openai-api-0.6.0/gpt4_openai_api.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-14 11:18:49.000000 gpt4-openai-api-0.6.0/gpt4_openai_api.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       28 2023-06-14 11:18:49.000000 gpt4-openai-api-0.6.0/gpt4_openai_api.egg-info/requires.txt
--rw-rw-rw-   0        0        0       12 2023-06-14 11:18:49.000000 gpt4-openai-api-0.6.0/gpt4_openai_api.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-06-14 11:18:49.977381 gpt4-openai-api-0.6.0/setup.cfg
--rw-rw-rw-   0        0        0     1164 2023-06-14 11:17:48.000000 gpt4-openai-api-0.6.0/setup.py
-drwxrwxrwx   0        0        0        0 2023-06-14 11:18:49.973382 gpt4-openai-api-0.6.0/test/
--rw-rw-rw-   0        0        0      449 2023-05-20 10:56:45.000000 gpt4-openai-api-0.6.0/test/test.py
--rw-rw-rw-   0        0        0      637 2023-06-14 11:16:05.000000 gpt4-openai-api-0.6.0/test/test_browsing.py
--rw-rw-rw-   0        0        0      985 2023-06-14 11:13:17.000000 gpt4-openai-api-0.6.0/test/test_continue_generating.py
--rw-rw-rw-   0        0        0      987 2023-06-02 17:56:38.000000 gpt4-openai-api-0.6.0/test/test_langchain.py
--rw-rw-rw-   0        0        0     1737 2023-06-14 11:13:29.000000 gpt4-openai-api-0.6.0/test/test_phones.py
--rw-rw-rw-   0        0        0      931 2023-06-02 17:56:38.000000 gpt4-openai-api-0.6.0/test/test_plugins.py
+drwxrwxrwx   0        0        0        0 2023-06-26 12:31:09.730800 gpt4-openai-api-0.7.0/
+-rw-rw-rw-   0        0        0     6253 2023-06-26 12:31:09.728801 gpt4-openai-api-0.7.0/PKG-INFO
+drwxrwxrwx   0        0        0        0 2023-06-26 12:31:09.595815 gpt4-openai-api-0.7.0/gpt4_openai/
+-rw-rw-rw-   0        0        0     1580 2023-06-14 11:17:48.000000 gpt4-openai-api-0.7.0/gpt4_openai/__init__.py
+drwxrwxrwx   0        0        0        0 2023-06-26 12:31:09.695797 gpt4-openai-api-0.7.0/gpt4_openai_api.egg-info/
+-rw-rw-rw-   0        0        0     6253 2023-06-26 12:31:09.000000 gpt4-openai-api-0.7.0/gpt4_openai_api.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      358 2023-06-26 12:31:09.000000 gpt4-openai-api-0.7.0/gpt4_openai_api.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-26 12:31:09.000000 gpt4-openai-api-0.7.0/gpt4_openai_api.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       28 2023-06-26 12:31:09.000000 gpt4-openai-api-0.7.0/gpt4_openai_api.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       12 2023-06-26 12:31:09.000000 gpt4-openai-api-0.7.0/gpt4_openai_api.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-06-26 12:31:09.731799 gpt4-openai-api-0.7.0/setup.cfg
+-rw-rw-rw-   0        0        0     1164 2023-06-26 12:30:34.000000 gpt4-openai-api-0.7.0/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-26 12:31:09.725801 gpt4-openai-api-0.7.0/test/
+-rw-rw-rw-   0        0        0      449 2023-05-20 10:56:45.000000 gpt4-openai-api-0.7.0/test/test.py
+-rw-rw-rw-   0        0        0      637 2023-06-14 11:16:05.000000 gpt4-openai-api-0.7.0/test/test_browsing.py
+-rw-rw-rw-   0        0        0     2045 2023-06-26 12:23:30.000000 gpt4-openai-api-0.7.0/test/test_continue_generating.py
+-rw-rw-rw-   0        0        0      987 2023-06-02 17:56:38.000000 gpt4-openai-api-0.7.0/test/test_langchain.py
+-rw-rw-rw-   0        0        0     1737 2023-06-14 11:13:29.000000 gpt4-openai-api-0.7.0/test/test_phones.py
+-rw-rw-rw-   0        0        0      931 2023-06-02 17:56:38.000000 gpt4-openai-api-0.7.0/test/test_plugins.py
```

### Comparing `gpt4-openai-api-0.6.0/PKG-INFO` & `gpt4-openai-api-0.7.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: gpt4-openai-api
-Version: 0.6.0
+Version: 0.7.0
 Summary: Python package for unofficial GPT-4 API access via chat.openai.com
 Home-page: https://github.com/Erol444/gpt4-openai-api
 Author: Erol444
 Author-email: erol123444@gmail.com
 License: UNKNOWN
 Description: # GPT4 OpenAI unofficial API
```

### Comparing `gpt4-openai-api-0.6.0/gpt4_openai/__init__.py` & `gpt4-openai-api-0.7.0/gpt4_openai/__init__.py`

 * *Files identical despite different names*

### Comparing `gpt4-openai-api-0.6.0/gpt4_openai_api.egg-info/PKG-INFO` & `gpt4-openai-api-0.7.0/gpt4_openai_api.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: gpt4-openai-api
-Version: 0.6.0
+Version: 0.7.0
 Summary: Python package for unofficial GPT-4 API access via chat.openai.com
 Home-page: https://github.com/Erol444/gpt4-openai-api
 Author: Erol444
 Author-email: erol123444@gmail.com
 License: UNKNOWN
 Description: # GPT4 OpenAI unofficial API
```

### Comparing `gpt4-openai-api-0.6.0/setup.py` & `gpt4-openai-api-0.7.0/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -3,24 +3,24 @@
 
 root = Path(__file__).parent.resolve()
 readme_file = root / 'readme.md'
 long_description = readme_file.read_text(encoding='utf-8')
 
 setup(
     name="gpt4-openai-api",
-    version="0.6.0",
+    version="0.7.0",
     description="Python package for unofficial GPT-4 API access via chat.openai.com",
     long_description=long_description,
     long_description_content_type='text/markdown',
     author="Erol444",
     author_email="erol123444@gmail.com",
     url="https://github.com/Erol444/gpt4-openai-api",
     packages=["gpt4_openai"],
     install_requires=[
-        "revChatGPT==6.2.2",
+        "revChatGPT==6.4.4",
         "langchain",
     ],
     classifiers=[
         "Development Status :: 3 - Alpha",
         "Intended Audience :: Developers",
         "License :: OSI Approved :: MIT License",
         "Programming Language :: Python :: 3",
```

### Comparing `gpt4-openai-api-0.6.0/test/test_browsing.py` & `gpt4-openai-api-0.7.0/test/test_browsing.py`

 * *Files identical despite different names*

### Comparing `gpt4-openai-api-0.6.0/test/test_langchain.py` & `gpt4-openai-api-0.7.0/test/test_langchain.py`

 * *Files identical despite different names*

### Comparing `gpt4-openai-api-0.6.0/test/test_phones.py` & `gpt4-openai-api-0.7.0/test/test_phones.py`

 * *Files identical despite different names*

### Comparing `gpt4-openai-api-0.6.0/test/test_plugins.py` & `gpt4-openai-api-0.7.0/test/test_plugins.py`

 * *Files identical despite different names*

