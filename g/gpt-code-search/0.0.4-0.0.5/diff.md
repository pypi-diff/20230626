# Comparing `tmp/gpt_code_search-0.0.4.tar.gz` & `tmp/gpt_code_search-0.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "gpt_code_search-0.0.4.tar", max compression
+gzip compressed data, was "gpt_code_search-0.0.5.tar", max compression
```

## Comparing `gpt_code_search-0.0.4.tar` & `gpt_code_search-0.0.5.tar`

### file list

```diff
@@ -1,10 +1,12 @@
--rw-r--r--   0        0        0    11357 2023-06-23 21:11:19.022270 gpt_code_search-0.0.4/LICENSE
--rw-r--r--   0        0        0     7667 2023-06-25 22:07:11.211081 gpt_code_search-0.0.4/README.md
--rw-r--r--   0        0        0        0 2023-06-23 04:13:32.205359 gpt_code_search-0.0.4/core/__init__.py
--rw-r--r--   0        0        0     6040 2023-06-25 22:57:18.491657 gpt_code_search-0.0.4/core/ai.py
--rw-r--r--   0        0        0     1104 2023-06-25 22:07:30.429077 gpt_code_search-0.0.4/core/analytics.py
--rw-r--r--   0        0        0     2911 2023-06-25 19:52:46.261474 gpt_code_search-0.0.4/core/config.py
--rw-r--r--   0        0        0     7897 2023-06-25 22:58:11.326099 gpt_code_search-0.0.4/core/functions.py
--rw-r--r--   0        0        0     3072 2023-06-25 22:44:27.362555 gpt_code_search-0.0.4/core/main.py
--rw-r--r--   0        0        0     1178 2023-06-25 22:14:56.252613 gpt_code_search-0.0.4/pyproject.toml
--rw-r--r--   0        0        0     8976 1970-01-01 00:00:00.000000 gpt_code_search-0.0.4/PKG-INFO
+-rw-r--r--   0        0        0    11357 2023-06-23 21:11:19.022270 gpt_code_search-0.0.5/LICENSE
+-rw-r--r--   0        0        0     7667 2023-06-25 22:07:11.211081 gpt_code_search-0.0.5/README.md
+-rw-r--r--   0        0        0        0 2023-06-23 04:13:32.205359 gpt_code_search-0.0.5/core/__init__.py
+-rw-r--r--   0        0        0     6035 2023-06-26 02:41:46.649895 gpt_code_search-0.0.5/core/ai.py
+-rw-r--r--   0        0        0     1104 2023-06-25 22:07:30.429077 gpt_code_search-0.0.5/core/analytics.py
+-rw-r--r--   0        0        0     2911 2023-06-25 19:52:46.261474 gpt_code_search-0.0.5/core/config.py
+-rw-r--r--   0        0        0     7637 2023-06-26 02:43:17.380254 gpt_code_search-0.0.5/core/functions.py
+-rw-r--r--   0        0        0     3072 2023-06-25 22:44:27.362555 gpt_code_search-0.0.5/core/main.py
+-rw-r--r--   0        0        0        0 2023-06-26 01:55:02.493714 gpt_code_search-0.0.5/core/tests/__init__.py
+-rw-r--r--   0        0        0     1057 2023-06-26 03:07:33.872866 gpt_code_search-0.0.5/core/tests/test_truncate_text.py
+-rw-r--r--   0        0        0     1258 2023-06-26 02:50:42.325898 gpt_code_search-0.0.5/pyproject.toml
+-rw-r--r--   0        0        0     8976 1970-01-01 00:00:00.000000 gpt_code_search-0.0.5/PKG-INFO
```

### Comparing `gpt_code_search-0.0.4/LICENSE` & `gpt_code_search-0.0.5/LICENSE`

 * *Files identical despite different names*

### Comparing `gpt_code_search-0.0.4/README.md` & `gpt_code_search-0.0.5/README.md`

 * *Files identical despite different names*

### Comparing `gpt_code_search-0.0.4/core/ai.py` & `gpt_code_search-0.0.5/core/ai.py`

 * *Files 1% similar despite different names*

```diff
@@ -118,15 +118,15 @@
 
     truncated_response = truncate_text_to_token_limit(function_response, MAX_TOKENS)
 
     messages.append(
         {
             "role": "function",
             "name": function_name,
-            "content": str(truncated_response),
+            "content": truncated_response,
         }
     )
     next_response = chat_completion_request(
         messages=messages,
         functions=functions,
     )
     return next_response
```

### Comparing `gpt_code_search-0.0.4/core/analytics.py` & `gpt_code_search-0.0.5/core/analytics.py`

 * *Files identical despite different names*

### Comparing `gpt_code_search-0.0.4/core/config.py` & `gpt_code_search-0.0.5/core/config.py`

 * *Files identical despite different names*

### Comparing `gpt_code_search-0.0.4/core/functions.py` & `gpt_code_search-0.0.5/core/functions.py`

 * *Files 11% similar despite different names*

```diff
@@ -104,55 +104,42 @@
         with open(file_path, "r") as file:
             logging.info("Reading file: {}".format(file_path))
             return file.read()
     except FileNotFoundError:
         return ""
 
 
-def count_tokens(text: str) -> int:
+def count_tokens(text) -> int:
     encoding = tiktoken.get_encoding("cl100k_base")
-    return len(encoding.encode_ordinary(text))
+    return len(encoding.encode_ordinary(str(text)))
 
 
-def truncate_text_to_token_limit(data: Union[str, List[str], List[Tuple[str, int]]], max_tokens: int):
+def truncate_text_to_token_limit(data: Union[str, List[str], List[Tuple[str, float]]], max_tokens: int) -> str:
     """
     Truncate the text (or list of strings or list of tuples) to fit within the maximum token limit.
     :param data: The text or list of strings or list of tuples to truncate.
     :param max_tokens: The maximum number of tokens.
-    :return: The truncated text or list of strings or list of tuples.
+    :return: The truncated data.
     """
-    if not data:
-        return []
-
     if isinstance(data, str):
-        chunks = data.split(" ")
+        truncated_data = data
     elif isinstance(data, list):
-        if data and isinstance(data[0], tuple):
-            chunks = [item[0] for item in data]
+        if all(isinstance(i, tuple) and len(i) == 2 for i in data):
+            truncated_data = ", ".join(f"({text}, {value})" for text, value in data)
+        elif all(isinstance(i, str) for i in data):
+            truncated_data = " ".join(data)
         else:
-            chunks = data
+            raise ValueError("Invalid data type. Expected str, list of str, or list of tuples (str, float).")
     else:
-        raise ValueError("The input data should be a string or a list of strings or a list of tuples.")
-
-    total_tokens = sum(len(chunk.split(" ")) for chunk in chunks)
+        raise ValueError("Invalid data type. Expected str, list of str, or list of tuples (str, float).")
 
-    while total_tokens > max_tokens:
-        total_tokens -= len(chunks[-1].split(" "))
-        chunks = chunks[:-1]
+    while count_tokens(truncated_data) > max_tokens:
+        truncated_data = truncated_data[:-1]
 
-    if isinstance(data, str):
-        truncated_text = " ".join(chunks)[:max_tokens]
-        return truncated_text
-    elif data and isinstance(data[0], tuple):
-        ranks = [item[1] for item in data[: len(chunks)]]
-        truncated_list = list(zip(chunks, ranks))
-        return truncated_list
-    else:
-        truncated_list = chunks[:max_tokens]
-        return truncated_list
+    return truncated_data
 
 
 def enabled_functions():
     return [
         {
             "name": "get_contents_of_file",
             "description": "Get the contents of a file. Returns empty string if the file is not found.",
@@ -219,11 +206,11 @@
                 "properties": {
                     "start_path": {
                         "type": "string",
                         "description": "The path to start the search from. Defaults to the current directory.",
                         "default": ".",
                     },
                 },
-                "required": [],
+                "required": ["start_path"],
             },
         },
     ]
```

### Comparing `gpt_code_search-0.0.4/core/main.py` & `gpt_code_search-0.0.5/core/main.py`

 * *Files identical despite different names*

### Comparing `gpt_code_search-0.0.4/pyproject.toml` & `gpt_code_search-0.0.5/pyproject.toml`

 * *Files 9% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "gpt-code-search"
-version = "0.0.4"
+version = "0.0.5"
 description = "gpt-code-search enables you to search your codebase with natural language."
 authors = ["narenmanoharan <narenkmanoharan@gmail.com>", "skovy <smiskoviak@gmail.com>"]
 license = "Apache-2.0"
 readme = "README.md"
 packages = [{include = "core"}]
 homepage = "https://wolfia.com"
 repository = "https://github.com/wolfia-app/gpt-code-search"
@@ -30,10 +30,14 @@
 sentry-sdk = {extras = ["flask"], version = "^1.26.0"}
 posthog = "^3.0.1"
 scikit-learn = "^1.2.2"
 
 [tool.poetry.dev-dependencies]
 pre-commit = "^2.15.0"
 
+[tool.poetry.group.dev.dependencies]
+pytest = "^7.4.0"
+pytest-mock = "^3.11.1"
+
 [build-system]
 requires = ["poetry-core"]
 build-backend = "poetry.core.masonry.api"
```

### Comparing `gpt_code_search-0.0.4/PKG-INFO` & `gpt_code_search-0.0.5/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: gpt-code-search
-Version: 0.0.4
+Version: 0.0.5
 Summary: gpt-code-search enables you to search your codebase with natural language.
 Home-page: https://wolfia.com
 License: Apache-2.0
 Keywords: gpt,code,search,wolfia,gpt4,llm
 Author: narenmanoharan
 Author-email: narenkmanoharan@gmail.com
 Requires-Python: >=3.9.17,<4.0.0
```

