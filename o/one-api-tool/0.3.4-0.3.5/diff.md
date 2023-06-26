# Comparing `tmp/one-api-tool-0.3.4.tar.gz` & `tmp/one-api-tool-0.3.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "one-api-tool-0.3.4.tar", last modified: Mon Jun 26 09:23:36 2023, max compression
+gzip compressed data, was "one-api-tool-0.3.5.tar", last modified: Mon Jun 26 09:40:52 2023, max compression
```

## Comparing `one-api-tool-0.3.4.tar` & `one-api-tool-0.3.5.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 zhangchong   (501) staff       (20)        0 2023-06-26 09:23:36.394638 one-api-tool-0.3.4/
--rw-r--r--   0 zhangchong   (501) staff       (20)     1055 2023-04-17 11:33:07.000000 one-api-tool-0.3.4/LICENSE
--rw-r--r--   0 zhangchong   (501) staff       (20)     4427 2023-06-26 09:23:36.394394 one-api-tool-0.3.4/PKG-INFO
--rw-r--r--   0 zhangchong   (501) staff       (20)     3871 2023-06-26 09:23:01.000000 one-api-tool-0.3.4/README.md
-drwxr-xr-x   0 zhangchong   (501) staff       (20)        0 2023-06-26 09:23:36.393107 one-api-tool-0.3.4/one_api_tool.egg-info/
--rw-r--r--   0 zhangchong   (501) staff       (20)     4427 2023-06-26 09:23:36.000000 one-api-tool-0.3.4/one_api_tool.egg-info/PKG-INFO
--rw-r--r--   0 zhangchong   (501) staff       (20)      343 2023-06-26 09:23:36.000000 one-api-tool-0.3.4/one_api_tool.egg-info/SOURCES.txt
--rw-r--r--   0 zhangchong   (501) staff       (20)        1 2023-06-26 09:23:36.000000 one-api-tool-0.3.4/one_api_tool.egg-info/dependency_links.txt
--rw-r--r--   0 zhangchong   (501) staff       (20)       64 2023-06-26 09:23:36.000000 one-api-tool-0.3.4/one_api_tool.egg-info/entry_points.txt
--rw-r--r--   0 zhangchong   (501) staff       (20)       69 2023-06-26 09:23:36.000000 one-api-tool-0.3.4/one_api_tool.egg-info/requires.txt
--rw-r--r--   0 zhangchong   (501) staff       (20)        7 2023-06-26 09:23:36.000000 one-api-tool-0.3.4/one_api_tool.egg-info/top_level.txt
-drwxr-xr-x   0 zhangchong   (501) staff       (20)        0 2023-06-26 09:23:36.393607 one-api-tool-0.3.4/oneapi/
--rw-r--r--   0 zhangchong   (501) staff       (20)       37 2023-04-28 08:45:03.000000 one-api-tool-0.3.4/oneapi/__init__.py
-drwxr-xr-x   0 zhangchong   (501) staff       (20)        0 2023-06-26 09:23:36.394029 one-api-tool-0.3.4/oneapi/commands/
--rw-r--r--   0 zhangchong   (501) staff       (20)        0 2023-04-26 09:00:27.000000 one-api-tool-0.3.4/oneapi/commands/__init__.py
--rw-r--r--   0 zhangchong   (501) staff       (20)     2131 2023-06-26 09:16:41.000000 one-api-tool-0.3.4/oneapi/commands/one_api_requst.py
--rw-r--r--   0 zhangchong   (501) staff       (20)    11397 2023-06-26 09:16:49.000000 one-api-tool-0.3.4/oneapi/one_api.py
--rw-r--r--   0 zhangchong   (501) staff       (20)       38 2023-06-26 09:23:36.394694 one-api-tool-0.3.4/setup.cfg
--rw-r--r--   0 zhangchong   (501) staff       (20)     1051 2023-06-26 09:23:32.000000 one-api-tool-0.3.4/setup.py
+drwxr-xr-x   0 zhangchong   (501) staff       (20)        0 2023-06-26 09:40:52.990080 one-api-tool-0.3.5/
+-rw-r--r--   0 zhangchong   (501) staff       (20)     1055 2023-04-17 11:33:07.000000 one-api-tool-0.3.5/LICENSE
+-rw-r--r--   0 zhangchong   (501) staff       (20)     4427 2023-06-26 09:40:52.989856 one-api-tool-0.3.5/PKG-INFO
+-rw-r--r--   0 zhangchong   (501) staff       (20)     3871 2023-06-26 09:23:01.000000 one-api-tool-0.3.5/README.md
+drwxr-xr-x   0 zhangchong   (501) staff       (20)        0 2023-06-26 09:40:52.988751 one-api-tool-0.3.5/one_api_tool.egg-info/
+-rw-r--r--   0 zhangchong   (501) staff       (20)     4427 2023-06-26 09:40:52.000000 one-api-tool-0.3.5/one_api_tool.egg-info/PKG-INFO
+-rw-r--r--   0 zhangchong   (501) staff       (20)      343 2023-06-26 09:40:52.000000 one-api-tool-0.3.5/one_api_tool.egg-info/SOURCES.txt
+-rw-r--r--   0 zhangchong   (501) staff       (20)        1 2023-06-26 09:40:52.000000 one-api-tool-0.3.5/one_api_tool.egg-info/dependency_links.txt
+-rw-r--r--   0 zhangchong   (501) staff       (20)       64 2023-06-26 09:40:52.000000 one-api-tool-0.3.5/one_api_tool.egg-info/entry_points.txt
+-rw-r--r--   0 zhangchong   (501) staff       (20)       69 2023-06-26 09:40:52.000000 one-api-tool-0.3.5/one_api_tool.egg-info/requires.txt
+-rw-r--r--   0 zhangchong   (501) staff       (20)        7 2023-06-26 09:40:52.000000 one-api-tool-0.3.5/one_api_tool.egg-info/top_level.txt
+drwxr-xr-x   0 zhangchong   (501) staff       (20)        0 2023-06-26 09:40:52.989168 one-api-tool-0.3.5/oneapi/
+-rw-r--r--   0 zhangchong   (501) staff       (20)       37 2023-04-28 08:45:03.000000 one-api-tool-0.3.5/oneapi/__init__.py
+drwxr-xr-x   0 zhangchong   (501) staff       (20)        0 2023-06-26 09:40:52.989524 one-api-tool-0.3.5/oneapi/commands/
+-rw-r--r--   0 zhangchong   (501) staff       (20)        0 2023-04-26 09:00:27.000000 one-api-tool-0.3.5/oneapi/commands/__init__.py
+-rw-r--r--   0 zhangchong   (501) staff       (20)     2168 2023-06-26 09:39:20.000000 one-api-tool-0.3.5/oneapi/commands/one_api_requst.py
+-rw-r--r--   0 zhangchong   (501) staff       (20)    11395 2023-06-26 09:40:17.000000 one-api-tool-0.3.5/oneapi/one_api.py
+-rw-r--r--   0 zhangchong   (501) staff       (20)       38 2023-06-26 09:40:52.990131 one-api-tool-0.3.5/setup.cfg
+-rw-r--r--   0 zhangchong   (501) staff       (20)     1051 2023-06-26 09:40:46.000000 one-api-tool-0.3.5/setup.py
```

### Comparing `one-api-tool-0.3.4/LICENSE` & `one-api-tool-0.3.5/LICENSE`

 * *Files identical despite different names*

### Comparing `one-api-tool-0.3.4/PKG-INFO` & `one-api-tool-0.3.5/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: one-api-tool
-Version: 0.3.4
+Version: 0.3.5
 Summary: Use only one line of code to call multiple model APIs similar to ChatGPT. Currently supported: Azure OpenAI Resource endpoint API, OpenAI Official API, and Anthropic Claude series model API.
 Home-page: https://github.com/muximus3/OneAPI
 Classifier: Development Status :: 3 - Alpha
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: OS Independent
 Description-Content-Type: text/markdown
```

### Comparing `one-api-tool-0.3.4/README.md` & `one-api-tool-0.3.5/README.md`

 * *Files identical despite different names*

### Comparing `one-api-tool-0.3.4/one_api_tool.egg-info/PKG-INFO` & `one-api-tool-0.3.5/one_api_tool.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: one-api-tool
-Version: 0.3.4
+Version: 0.3.5
 Summary: Use only one line of code to call multiple model APIs similar to ChatGPT. Currently supported: Azure OpenAI Resource endpoint API, OpenAI Official API, and Anthropic Claude series model API.
 Home-page: https://github.com/muximus3/OneAPI
 Classifier: Development Status :: 3 - Alpha
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: OS Independent
 Description-Content-Type: text/markdown
```

### Comparing `one-api-tool-0.3.4/oneapi/commands/one_api_requst.py` & `one-api-tool-0.3.5/oneapi/commands/one_api_requst.py`

 * *Files 2% similar despite different names*

```diff
@@ -18,16 +18,17 @@
                         "--prompt",
                         type=str,
                         help="question",
                         required=True)
     parser.add_argument("-s",
                         "--system",
                         type=str,
+                        default="",
                         help="question",
-                        required=True)
+                        required=False)
     parser.add_argument("-m",
                         "--model",
                         type=str,
                         default="",
                         help="evaluate model name, e.g., gpt-35-turbo, gpt-4",
                         required=False)
     parser.add_argument("-te",
```

### Comparing `one-api-tool-0.3.4/oneapi/one_api.py` & `one-api-tool-0.3.5/oneapi/one_api.py`

 * *Files 0% similar despite different names*

```diff
@@ -238,15 +238,15 @@
     @staticmethod
     def load_json(file_path):
         with open(file_path, "r") as f:
             return json.load(f)
 
     def simple_chat(self, prompt, system="", model="", temperature=1, max_new_tokens=2048, stream=True, **kwargs):
         if isinstance(self.tool, OpenAITool):
-            msgs = [] if system == "" else [ChatGPTMessage(role="system", content=system)]
+            msgs = [] if not system else [ChatGPTMessage(role="system", content=system)]
             msgs.append(ChatGPTMessage(role="user", content=prompt))
             if isinstance(self.tool.method, AzureMethod):
                 args = AzureDecodingArguments(messages=msgs, engine=model if model else "gpt-35-turbo", temperature=temperature, max_tokens=max_new_tokens, stream=stream, **kwargs)
             elif isinstance(self.tool.method, OpenAIMethod):
                 args = OpenAIDecodingArguments(messages=msgs, model=model if model else "gpt-3.5-turbo-0613", temperature=temperature, max_tokens=max_new_tokens, stream=stream, **kwargs)
         elif isinstance(self.tool, ClaudeAITool):
             args = ClaudeDecodingArguments(prompt=f"{anthropic.HUMAN_PROMPT} {prompt}{anthropic.AI_PROMPT}", model=model if model else "claude-v1.3-100k", temperature=temperature, max_tokens_to_sample=max_new_tokens, stream=stream, **kwargs)
```

### Comparing `one-api-tool-0.3.4/setup.py` & `one-api-tool-0.3.5/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
     name="one-api-tool",
-    version="0.3.4",
+    version="0.3.5",
     packages=find_packages(),
     install_requires=[
         # Add your library's dependencies here
         "pydantic",
         "openai",
         "anthropic",
         "requests",
```

