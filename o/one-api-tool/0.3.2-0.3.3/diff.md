# Comparing `tmp/one-api-tool-0.3.2.tar.gz` & `tmp/one-api-tool-0.3.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "one-api-tool-0.3.2.tar", last modified: Mon Jun 19 11:38:34 2023, max compression
+gzip compressed data, was "one-api-tool-0.3.3.tar", last modified: Mon Jun 26 09:13:20 2023, max compression
```

## Comparing `one-api-tool-0.3.2.tar` & `one-api-tool-0.3.3.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 zhangchong   (501) staff       (20)        0 2023-06-19 11:38:34.938673 one-api-tool-0.3.2/
--rw-r--r--   0 zhangchong   (501) staff       (20)     1055 2023-04-17 11:33:07.000000 one-api-tool-0.3.2/LICENSE
--rw-r--r--   0 zhangchong   (501) staff       (20)     4273 2023-06-19 11:38:34.938528 one-api-tool-0.3.2/PKG-INFO
--rw-r--r--   0 zhangchong   (501) staff       (20)     3717 2023-06-19 08:54:47.000000 one-api-tool-0.3.2/README.md
-drwxr-xr-x   0 zhangchong   (501) staff       (20)        0 2023-06-19 11:38:34.937759 one-api-tool-0.3.2/one_api_tool.egg-info/
--rw-r--r--   0 zhangchong   (501) staff       (20)     4273 2023-06-19 11:38:34.000000 one-api-tool-0.3.2/one_api_tool.egg-info/PKG-INFO
--rw-r--r--   0 zhangchong   (501) staff       (20)      343 2023-06-19 11:38:34.000000 one-api-tool-0.3.2/one_api_tool.egg-info/SOURCES.txt
--rw-r--r--   0 zhangchong   (501) staff       (20)        1 2023-06-19 11:38:34.000000 one-api-tool-0.3.2/one_api_tool.egg-info/dependency_links.txt
--rw-r--r--   0 zhangchong   (501) staff       (20)       64 2023-06-19 11:38:34.000000 one-api-tool-0.3.2/one_api_tool.egg-info/entry_points.txt
--rw-r--r--   0 zhangchong   (501) staff       (20)       69 2023-06-19 11:38:34.000000 one-api-tool-0.3.2/one_api_tool.egg-info/requires.txt
--rw-r--r--   0 zhangchong   (501) staff       (20)        7 2023-06-19 11:38:34.000000 one-api-tool-0.3.2/one_api_tool.egg-info/top_level.txt
-drwxr-xr-x   0 zhangchong   (501) staff       (20)        0 2023-06-19 11:38:34.938063 one-api-tool-0.3.2/oneapi/
--rw-r--r--   0 zhangchong   (501) staff       (20)       37 2023-04-28 08:45:03.000000 one-api-tool-0.3.2/oneapi/__init__.py
-drwxr-xr-x   0 zhangchong   (501) staff       (20)        0 2023-06-19 11:38:34.938317 one-api-tool-0.3.2/oneapi/commands/
--rw-r--r--   0 zhangchong   (501) staff       (20)        0 2023-04-26 09:00:27.000000 one-api-tool-0.3.2/oneapi/commands/__init__.py
--rw-r--r--   0 zhangchong   (501) staff       (20)     1923 2023-05-04 06:36:39.000000 one-api-tool-0.3.2/oneapi/commands/one_api_requst.py
--rw-r--r--   0 zhangchong   (501) staff       (20)    11137 2023-06-19 11:38:03.000000 one-api-tool-0.3.2/oneapi/one_api.py
--rw-r--r--   0 zhangchong   (501) staff       (20)       38 2023-06-19 11:38:34.938716 one-api-tool-0.3.2/setup.cfg
--rw-r--r--   0 zhangchong   (501) staff       (20)     1051 2023-06-19 11:38:25.000000 one-api-tool-0.3.2/setup.py
+drwxr-xr-x   0 zhangchong   (501) staff       (20)        0 2023-06-26 09:13:20.833313 one-api-tool-0.3.3/
+-rw-r--r--   0 zhangchong   (501) staff       (20)     1055 2023-04-17 11:33:07.000000 one-api-tool-0.3.3/LICENSE
+-rw-r--r--   0 zhangchong   (501) staff       (20)     4273 2023-06-26 09:13:20.832984 one-api-tool-0.3.3/PKG-INFO
+-rw-r--r--   0 zhangchong   (501) staff       (20)     3717 2023-06-19 08:54:47.000000 one-api-tool-0.3.3/README.md
+drwxr-xr-x   0 zhangchong   (501) staff       (20)        0 2023-06-26 09:13:20.831079 one-api-tool-0.3.3/one_api_tool.egg-info/
+-rw-r--r--   0 zhangchong   (501) staff       (20)     4273 2023-06-26 09:13:20.000000 one-api-tool-0.3.3/one_api_tool.egg-info/PKG-INFO
+-rw-r--r--   0 zhangchong   (501) staff       (20)      343 2023-06-26 09:13:20.000000 one-api-tool-0.3.3/one_api_tool.egg-info/SOURCES.txt
+-rw-r--r--   0 zhangchong   (501) staff       (20)        1 2023-06-26 09:13:20.000000 one-api-tool-0.3.3/one_api_tool.egg-info/dependency_links.txt
+-rw-r--r--   0 zhangchong   (501) staff       (20)       64 2023-06-26 09:13:20.000000 one-api-tool-0.3.3/one_api_tool.egg-info/entry_points.txt
+-rw-r--r--   0 zhangchong   (501) staff       (20)       69 2023-06-26 09:13:20.000000 one-api-tool-0.3.3/one_api_tool.egg-info/requires.txt
+-rw-r--r--   0 zhangchong   (501) staff       (20)        7 2023-06-26 09:13:20.000000 one-api-tool-0.3.3/one_api_tool.egg-info/top_level.txt
+drwxr-xr-x   0 zhangchong   (501) staff       (20)        0 2023-06-26 09:13:20.831986 one-api-tool-0.3.3/oneapi/
+-rw-r--r--   0 zhangchong   (501) staff       (20)       37 2023-04-28 08:45:03.000000 one-api-tool-0.3.3/oneapi/__init__.py
+drwxr-xr-x   0 zhangchong   (501) staff       (20)        0 2023-06-26 09:13:20.832346 one-api-tool-0.3.3/oneapi/commands/
+-rw-r--r--   0 zhangchong   (501) staff       (20)        0 2023-04-26 09:00:27.000000 one-api-tool-0.3.3/oneapi/commands/__init__.py
+-rw-r--r--   0 zhangchong   (501) staff       (20)     1923 2023-05-04 06:36:39.000000 one-api-tool-0.3.3/oneapi/commands/one_api_requst.py
+-rw-r--r--   0 zhangchong   (501) staff       (20)    11421 2023-06-26 09:09:04.000000 one-api-tool-0.3.3/oneapi/one_api.py
+-rw-r--r--   0 zhangchong   (501) staff       (20)       38 2023-06-26 09:13:20.833367 one-api-tool-0.3.3/setup.cfg
+-rw-r--r--   0 zhangchong   (501) staff       (20)     1051 2023-06-26 09:12:24.000000 one-api-tool-0.3.3/setup.py
```

### Comparing `one-api-tool-0.3.2/LICENSE` & `one-api-tool-0.3.3/LICENSE`

 * *Files identical despite different names*

### Comparing `one-api-tool-0.3.2/PKG-INFO` & `one-api-tool-0.3.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: one-api-tool
-Version: 0.3.2
+Version: 0.3.3
 Summary: Use only one line of code to call multiple model APIs similar to ChatGPT. Currently supported: Azure OpenAI Resource endpoint API, OpenAI Official API, and Anthropic Claude series model API.
 Home-page: https://github.com/muximus3/OneAPI
 Classifier: Development Status :: 3 - Alpha
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: OS Independent
 Description-Content-Type: text/markdown
```

### Comparing `one-api-tool-0.3.2/README.md` & `one-api-tool-0.3.3/README.md`

 * *Files identical despite different names*

### Comparing `one-api-tool-0.3.2/one_api_tool.egg-info/PKG-INFO` & `one-api-tool-0.3.3/one_api_tool.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: one-api-tool
-Version: 0.3.2
+Version: 0.3.3
 Summary: Use only one line of code to call multiple model APIs similar to ChatGPT. Currently supported: Azure OpenAI Resource endpoint API, OpenAI Official API, and Anthropic Claude series model API.
 Home-page: https://github.com/muximus3/OneAPI
 Classifier: Development Status :: 3 - Alpha
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: OS Independent
 Description-Content-Type: text/markdown
```

### Comparing `one-api-tool-0.3.2/oneapi/commands/one_api_requst.py` & `one-api-tool-0.3.3/oneapi/commands/one_api_requst.py`

 * *Files identical despite different names*

### Comparing `one-api-tool-0.3.2/oneapi/one_api.py` & `one-api-tool-0.3.3/oneapi/one_api.py`

 * *Files 2% similar despite different names*

```diff
@@ -236,23 +236,24 @@
 
 
     @staticmethod
     def load_json(file_path):
         with open(file_path, "r") as f:
             return json.load(f)
 
-    def simple_chat(self, prompt, model="", temperature=1, max_new_tokens=2048, stream=True, **kwargs):
+    def simple_chat(self, prompt, system_message="", model="", temperature=1, max_new_tokens=2048, stream=True, **kwargs):
         if isinstance(self.tool, OpenAITool):
-            msgs = [ChatGPTMessage(role="user", content=prompt)]
+            msgs = [] if system_message == "" else [ChatGPTMessage(role="system", content=system_message)]
+            msgs.append(ChatGPTMessage(role="user", content=prompt))
             if isinstance(self.tool.method, AzureMethod):
                 args = AzureDecodingArguments(messages=msgs, engine=model if model else "gpt-35-turbo", temperature=temperature, max_tokens=max_new_tokens, stream=stream, **kwargs)
             elif isinstance(self.tool.method, OpenAIMethod):
-                args = OpenAIDecodingArguments(messages=msgs, model=model if model else "gpt-3.5-turbo", temperature=temperature, max_tokens=max_new_tokens, stream=stream, **kwargs)
+                args = OpenAIDecodingArguments(messages=msgs, model=model if model else "gpt-3.5-turbo-0613", temperature=temperature, max_tokens=max_new_tokens, stream=stream, **kwargs)
         elif isinstance(self.tool, ClaudeAITool):
-            args = ClaudeDecodingArguments(prompt=f"\n\nHuman: {prompt}\n\nAssistant:", model=model if model else "claude-v1.3", temperature=temperature, max_tokens_to_sample=max_new_tokens, stream=stream, **kwargs)
+            args = ClaudeDecodingArguments(prompt=f"{anthropic.HUMAN_PROMPT} {prompt}{anthropic.AI_PROMPT}", model=model if model else "claude-v1.3-100k", temperature=temperature, max_tokens_to_sample=max_new_tokens, stream=stream, **kwargs)
         else:
             raise AssertionError(f"Not supported api type: {type(self.tool)}")
 
         response = self.tool.simple_chat(args)
         return response
 
     def get_embeddings(self, texts: List[str], engine="text-embedding-ada-002") -> List[List[float]]:
@@ -266,9 +267,11 @@
             return self.tool.get_embedding(text, engine)
         else:
             raise AssertionError(f"Not supported api type for embeddings: {type(self.tool)}")
     
     def count_tokens(self, texts: List[str], encoding_name: str = 'cl100k_base') -> int:
         if isinstance(self.tool, OpenAITool):
             return self.tool.count_tokens(texts, encoding_name)
+        elif isinstance(self.tool, ClaudeAITool):
+            return sum([anthropic.count_tokens(text) for text in texts])
         else:
             raise AssertionError(f"Not supported api type for token counting: {type(self.tool)}")
```

### Comparing `one-api-tool-0.3.2/setup.py` & `one-api-tool-0.3.3/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
     name="one-api-tool",
-    version="0.3.2",
+    version="0.3.3",
     packages=find_packages(),
     install_requires=[
         # Add your library's dependencies here
         "pydantic",
         "openai",
         "anthropic",
         "requests",
```

