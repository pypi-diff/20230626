# Comparing `tmp/one-api-tool-0.3.3.tar.gz` & `tmp/one-api-tool-0.3.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "one-api-tool-0.3.3.tar", last modified: Mon Jun 26 09:13:20 2023, max compression
+gzip compressed data, was "one-api-tool-0.3.4.tar", last modified: Mon Jun 26 09:23:36 2023, max compression
```

## Comparing `one-api-tool-0.3.3.tar` & `one-api-tool-0.3.4.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 zhangchong   (501) staff       (20)        0 2023-06-26 09:13:20.833313 one-api-tool-0.3.3/
--rw-r--r--   0 zhangchong   (501) staff       (20)     1055 2023-04-17 11:33:07.000000 one-api-tool-0.3.3/LICENSE
--rw-r--r--   0 zhangchong   (501) staff       (20)     4273 2023-06-26 09:13:20.832984 one-api-tool-0.3.3/PKG-INFO
--rw-r--r--   0 zhangchong   (501) staff       (20)     3717 2023-06-19 08:54:47.000000 one-api-tool-0.3.3/README.md
-drwxr-xr-x   0 zhangchong   (501) staff       (20)        0 2023-06-26 09:13:20.831079 one-api-tool-0.3.3/one_api_tool.egg-info/
--rw-r--r--   0 zhangchong   (501) staff       (20)     4273 2023-06-26 09:13:20.000000 one-api-tool-0.3.3/one_api_tool.egg-info/PKG-INFO
--rw-r--r--   0 zhangchong   (501) staff       (20)      343 2023-06-26 09:13:20.000000 one-api-tool-0.3.3/one_api_tool.egg-info/SOURCES.txt
--rw-r--r--   0 zhangchong   (501) staff       (20)        1 2023-06-26 09:13:20.000000 one-api-tool-0.3.3/one_api_tool.egg-info/dependency_links.txt
--rw-r--r--   0 zhangchong   (501) staff       (20)       64 2023-06-26 09:13:20.000000 one-api-tool-0.3.3/one_api_tool.egg-info/entry_points.txt
--rw-r--r--   0 zhangchong   (501) staff       (20)       69 2023-06-26 09:13:20.000000 one-api-tool-0.3.3/one_api_tool.egg-info/requires.txt
--rw-r--r--   0 zhangchong   (501) staff       (20)        7 2023-06-26 09:13:20.000000 one-api-tool-0.3.3/one_api_tool.egg-info/top_level.txt
-drwxr-xr-x   0 zhangchong   (501) staff       (20)        0 2023-06-26 09:13:20.831986 one-api-tool-0.3.3/oneapi/
--rw-r--r--   0 zhangchong   (501) staff       (20)       37 2023-04-28 08:45:03.000000 one-api-tool-0.3.3/oneapi/__init__.py
-drwxr-xr-x   0 zhangchong   (501) staff       (20)        0 2023-06-26 09:13:20.832346 one-api-tool-0.3.3/oneapi/commands/
--rw-r--r--   0 zhangchong   (501) staff       (20)        0 2023-04-26 09:00:27.000000 one-api-tool-0.3.3/oneapi/commands/__init__.py
--rw-r--r--   0 zhangchong   (501) staff       (20)     1923 2023-05-04 06:36:39.000000 one-api-tool-0.3.3/oneapi/commands/one_api_requst.py
--rw-r--r--   0 zhangchong   (501) staff       (20)    11421 2023-06-26 09:09:04.000000 one-api-tool-0.3.3/oneapi/one_api.py
--rw-r--r--   0 zhangchong   (501) staff       (20)       38 2023-06-26 09:13:20.833367 one-api-tool-0.3.3/setup.cfg
--rw-r--r--   0 zhangchong   (501) staff       (20)     1051 2023-06-26 09:12:24.000000 one-api-tool-0.3.3/setup.py
+drwxr-xr-x   0 zhangchong   (501) staff       (20)        0 2023-06-26 09:23:36.394638 one-api-tool-0.3.4/
+-rw-r--r--   0 zhangchong   (501) staff       (20)     1055 2023-04-17 11:33:07.000000 one-api-tool-0.3.4/LICENSE
+-rw-r--r--   0 zhangchong   (501) staff       (20)     4427 2023-06-26 09:23:36.394394 one-api-tool-0.3.4/PKG-INFO
+-rw-r--r--   0 zhangchong   (501) staff       (20)     3871 2023-06-26 09:23:01.000000 one-api-tool-0.3.4/README.md
+drwxr-xr-x   0 zhangchong   (501) staff       (20)        0 2023-06-26 09:23:36.393107 one-api-tool-0.3.4/one_api_tool.egg-info/
+-rw-r--r--   0 zhangchong   (501) staff       (20)     4427 2023-06-26 09:23:36.000000 one-api-tool-0.3.4/one_api_tool.egg-info/PKG-INFO
+-rw-r--r--   0 zhangchong   (501) staff       (20)      343 2023-06-26 09:23:36.000000 one-api-tool-0.3.4/one_api_tool.egg-info/SOURCES.txt
+-rw-r--r--   0 zhangchong   (501) staff       (20)        1 2023-06-26 09:23:36.000000 one-api-tool-0.3.4/one_api_tool.egg-info/dependency_links.txt
+-rw-r--r--   0 zhangchong   (501) staff       (20)       64 2023-06-26 09:23:36.000000 one-api-tool-0.3.4/one_api_tool.egg-info/entry_points.txt
+-rw-r--r--   0 zhangchong   (501) staff       (20)       69 2023-06-26 09:23:36.000000 one-api-tool-0.3.4/one_api_tool.egg-info/requires.txt
+-rw-r--r--   0 zhangchong   (501) staff       (20)        7 2023-06-26 09:23:36.000000 one-api-tool-0.3.4/one_api_tool.egg-info/top_level.txt
+drwxr-xr-x   0 zhangchong   (501) staff       (20)        0 2023-06-26 09:23:36.393607 one-api-tool-0.3.4/oneapi/
+-rw-r--r--   0 zhangchong   (501) staff       (20)       37 2023-04-28 08:45:03.000000 one-api-tool-0.3.4/oneapi/__init__.py
+drwxr-xr-x   0 zhangchong   (501) staff       (20)        0 2023-06-26 09:23:36.394029 one-api-tool-0.3.4/oneapi/commands/
+-rw-r--r--   0 zhangchong   (501) staff       (20)        0 2023-04-26 09:00:27.000000 one-api-tool-0.3.4/oneapi/commands/__init__.py
+-rw-r--r--   0 zhangchong   (501) staff       (20)     2131 2023-06-26 09:16:41.000000 one-api-tool-0.3.4/oneapi/commands/one_api_requst.py
+-rw-r--r--   0 zhangchong   (501) staff       (20)    11397 2023-06-26 09:16:49.000000 one-api-tool-0.3.4/oneapi/one_api.py
+-rw-r--r--   0 zhangchong   (501) staff       (20)       38 2023-06-26 09:23:36.394694 one-api-tool-0.3.4/setup.cfg
+-rw-r--r--   0 zhangchong   (501) staff       (20)     1051 2023-06-26 09:23:32.000000 one-api-tool-0.3.4/setup.py
```

### Comparing `one-api-tool-0.3.3/LICENSE` & `one-api-tool-0.3.4/LICENSE`

 * *Files identical despite different names*

### Comparing `one-api-tool-0.3.3/PKG-INFO` & `one-api-tool-0.3.4/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: one-api-tool
-Version: 0.3.3
+Version: 0.3.4
 Summary: Use only one line of code to call multiple model APIs similar to ChatGPT. Currently supported: Azure OpenAI Resource endpoint API, OpenAI Official API, and Anthropic Claude series model API.
 Home-page: https://github.com/muximus3/OneAPI
 Classifier: Development Status :: 3 - Alpha
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: OS Independent
 Description-Content-Type: text/markdown
@@ -71,15 +71,15 @@
 print(res)
 # Get embeddings of some sentences for further usage, e.g., clustering
 embeddings = tool.get_embeddings(["Hello AI!", "Hello world!"])
 print(len(embeddings)))
 # Count the number of tokens
 print(tool.count_tokens(["Hello AI!", "Hello world!"]))
 ```
-**Note: Currently, `count_tokens` and `get_embeddings` only support OpenAI or Microsoft Azure API.**
+**Note: Currently, `get_embeddings` only support OpenAI or Microsoft Azure API.**
 ### 2. Using command line
 ```sh
 open-api --config_file CHANGE_TO_YOUR_CONFIG_PATH \
 --model gpt-3.5-turbo \
 --prompt "1+1=?" 
 ```
 <details open><summary>Output detail</summary>
@@ -103,19 +103,22 @@
 #### Arguments detail:
 
 `--config_file` string ${\color{orange}\text{Required}}$ <br>A local configuration file containing API key information.
 
 `--prompt` string ${\color{orange}\text{Required}}$ <br>
 The question that would be predicted by LLMs, e.g., A math question would be like: "1+1=?".
 
+`--system` string ${\color{grey}\text{Optional}}$  Defaults to null <br> System message to instruct chatGPT, e.g., You are a helpful assistant.
+
 `--model` string ${\color{grey}\text{Optional}}$  Defaults to GPT-3.5-turbo or Claude-v1.3 depends on `api_type`<br> Which model to use, e.g., gpt-4.
 
 `--temperature` number ${\color{grey}\text{Optional}}$ Defaults to 1 <br>What sampling temperature to use.  Higher values like 0.9 will make the output more random, while lower values like 0.1 will make it more focused and deterministic. 
 
 `--max_new_tokens` integer ${\color{grey}\text{Optional}}$ Defaults to 2048 <br>
 The maximum number of tokens to generate in the chat completion.
 The total length of input tokens and generated tokens is limited by the model's context length.
 
 ## ToDo
 - [ ] Batch requests.
-- [ ] Token number counting.
+- [ ] OpenAI function_call.
+- [x] Token number counting.
 - [ ] Custom token budget.
```

### Comparing `one-api-tool-0.3.3/README.md` & `one-api-tool-0.3.4/README.md`

 * *Files 3% similar despite different names*

```diff
@@ -59,15 +59,15 @@
 print(res)
 # Get embeddings of some sentences for further usage, e.g., clustering
 embeddings = tool.get_embeddings(["Hello AI!", "Hello world!"])
 print(len(embeddings)))
 # Count the number of tokens
 print(tool.count_tokens(["Hello AI!", "Hello world!"]))
 ```
-**Note: Currently, `count_tokens` and `get_embeddings` only support OpenAI or Microsoft Azure API.**
+**Note: Currently, `get_embeddings` only support OpenAI or Microsoft Azure API.**
 ### 2. Using command line
 ```sh
 open-api --config_file CHANGE_TO_YOUR_CONFIG_PATH \
 --model gpt-3.5-turbo \
 --prompt "1+1=?" 
 ```
 <details open><summary>Output detail</summary>
@@ -91,19 +91,22 @@
 #### Arguments detail:
 
 `--config_file` string ${\color{orange}\text{Required}}$ <br>A local configuration file containing API key information.
 
 `--prompt` string ${\color{orange}\text{Required}}$ <br>
 The question that would be predicted by LLMs, e.g., A math question would be like: "1+1=?".
 
+`--system` string ${\color{grey}\text{Optional}}$  Defaults to null <br> System message to instruct chatGPT, e.g., You are a helpful assistant.
+
 `--model` string ${\color{grey}\text{Optional}}$  Defaults to GPT-3.5-turbo or Claude-v1.3 depends on `api_type`<br> Which model to use, e.g., gpt-4.
 
 `--temperature` number ${\color{grey}\text{Optional}}$ Defaults to 1 <br>What sampling temperature to use.  Higher values like 0.9 will make the output more random, while lower values like 0.1 will make it more focused and deterministic. 
 
 `--max_new_tokens` integer ${\color{grey}\text{Optional}}$ Defaults to 2048 <br>
 The maximum number of tokens to generate in the chat completion.
 The total length of input tokens and generated tokens is limited by the model's context length.
 
 ## ToDo
 - [ ] Batch requests.
-- [ ] Token number counting.
+- [ ] OpenAI function_call.
+- [x] Token number counting.
 - [ ] Custom token budget.
```

### Comparing `one-api-tool-0.3.3/one_api_tool.egg-info/PKG-INFO` & `one-api-tool-0.3.4/one_api_tool.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: one-api-tool
-Version: 0.3.3
+Version: 0.3.4
 Summary: Use only one line of code to call multiple model APIs similar to ChatGPT. Currently supported: Azure OpenAI Resource endpoint API, OpenAI Official API, and Anthropic Claude series model API.
 Home-page: https://github.com/muximus3/OneAPI
 Classifier: Development Status :: 3 - Alpha
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: OS Independent
 Description-Content-Type: text/markdown
@@ -71,15 +71,15 @@
 print(res)
 # Get embeddings of some sentences for further usage, e.g., clustering
 embeddings = tool.get_embeddings(["Hello AI!", "Hello world!"])
 print(len(embeddings)))
 # Count the number of tokens
 print(tool.count_tokens(["Hello AI!", "Hello world!"]))
 ```
-**Note: Currently, `count_tokens` and `get_embeddings` only support OpenAI or Microsoft Azure API.**
+**Note: Currently, `get_embeddings` only support OpenAI or Microsoft Azure API.**
 ### 2. Using command line
 ```sh
 open-api --config_file CHANGE_TO_YOUR_CONFIG_PATH \
 --model gpt-3.5-turbo \
 --prompt "1+1=?" 
 ```
 <details open><summary>Output detail</summary>
@@ -103,19 +103,22 @@
 #### Arguments detail:
 
 `--config_file` string ${\color{orange}\text{Required}}$ <br>A local configuration file containing API key information.
 
 `--prompt` string ${\color{orange}\text{Required}}$ <br>
 The question that would be predicted by LLMs, e.g., A math question would be like: "1+1=?".
 
+`--system` string ${\color{grey}\text{Optional}}$  Defaults to null <br> System message to instruct chatGPT, e.g., You are a helpful assistant.
+
 `--model` string ${\color{grey}\text{Optional}}$  Defaults to GPT-3.5-turbo or Claude-v1.3 depends on `api_type`<br> Which model to use, e.g., gpt-4.
 
 `--temperature` number ${\color{grey}\text{Optional}}$ Defaults to 1 <br>What sampling temperature to use.  Higher values like 0.9 will make the output more random, while lower values like 0.1 will make it more focused and deterministic. 
 
 `--max_new_tokens` integer ${\color{grey}\text{Optional}}$ Defaults to 2048 <br>
 The maximum number of tokens to generate in the chat completion.
 The total length of input tokens and generated tokens is limited by the model's context length.
 
 ## ToDo
 - [ ] Batch requests.
-- [ ] Token number counting.
+- [ ] OpenAI function_call.
+- [x] Token number counting.
 - [ ] Custom token budget.
```

### Comparing `one-api-tool-0.3.3/oneapi/commands/one_api_requst.py` & `one-api-tool-0.3.4/oneapi/commands/one_api_requst.py`

 * *Files 4% similar despite different names*

```diff
@@ -15,14 +15,19 @@
                         help="config file path",
                         required=True)
     parser.add_argument("-p",
                         "--prompt",
                         type=str,
                         help="question",
                         required=True)
+    parser.add_argument("-s",
+                        "--system",
+                        type=str,
+                        help="question",
+                        required=True)
     parser.add_argument("-m",
                         "--model",
                         type=str,
                         default="",
                         help="evaluate model name, e.g., gpt-35-turbo, gpt-4",
                         required=False)
     parser.add_argument("-te",
@@ -40,14 +45,15 @@
     args = parser.parse_args()
     tool = OneAPITool.from_config_file(args.config_file)
     print(
         f"\n{'-'*20} prompt detail 🚀  {'-'*20}\n\n{args.prompt}\n\n{'-'*20} prompt end {'-'*20}"
     )
     response = tool.simple_chat(
         prompt=args.prompt,
+        system=args.system,
         model=args.model,
         temperature=args.temperature,
         max_new_tokens=args.max_new_tokens,
     )
     print(
         f"{'-'*20} {args.model} response ⭐️ {'-'*20}\n\n{response}\n\n{'-'*20} response end {'-'*20}\n\n"
     )
```

### Comparing `one-api-tool-0.3.3/oneapi/one_api.py` & `one-api-tool-0.3.4/oneapi/one_api.py`

 * *Files 1% similar despite different names*

```diff
@@ -236,17 +236,17 @@
 
 
     @staticmethod
     def load_json(file_path):
         with open(file_path, "r") as f:
             return json.load(f)
 
-    def simple_chat(self, prompt, system_message="", model="", temperature=1, max_new_tokens=2048, stream=True, **kwargs):
+    def simple_chat(self, prompt, system="", model="", temperature=1, max_new_tokens=2048, stream=True, **kwargs):
         if isinstance(self.tool, OpenAITool):
-            msgs = [] if system_message == "" else [ChatGPTMessage(role="system", content=system_message)]
+            msgs = [] if system == "" else [ChatGPTMessage(role="system", content=system)]
             msgs.append(ChatGPTMessage(role="user", content=prompt))
             if isinstance(self.tool.method, AzureMethod):
                 args = AzureDecodingArguments(messages=msgs, engine=model if model else "gpt-35-turbo", temperature=temperature, max_tokens=max_new_tokens, stream=stream, **kwargs)
             elif isinstance(self.tool.method, OpenAIMethod):
                 args = OpenAIDecodingArguments(messages=msgs, model=model if model else "gpt-3.5-turbo-0613", temperature=temperature, max_tokens=max_new_tokens, stream=stream, **kwargs)
         elif isinstance(self.tool, ClaudeAITool):
             args = ClaudeDecodingArguments(prompt=f"{anthropic.HUMAN_PROMPT} {prompt}{anthropic.AI_PROMPT}", model=model if model else "claude-v1.3-100k", temperature=temperature, max_tokens_to_sample=max_new_tokens, stream=stream, **kwargs)
```

### Comparing `one-api-tool-0.3.3/setup.py` & `one-api-tool-0.3.4/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
     name="one-api-tool",
-    version="0.3.3",
+    version="0.3.4",
     packages=find_packages(),
     install_requires=[
         # Add your library's dependencies here
         "pydantic",
         "openai",
         "anthropic",
         "requests",
```

