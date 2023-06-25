# Comparing `tmp/gpt_code_search-0.0.3.tar.gz` & `tmp/gpt_code_search-0.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "gpt_code_search-0.0.3.tar", max compression
+gzip compressed data, was "gpt_code_search-0.0.4.tar", max compression
```

## Comparing `gpt_code_search-0.0.3.tar` & `gpt_code_search-0.0.4.tar`

### file list

```diff
@@ -1,9 +1,10 @@
--rw-r--r--   0        0        0    11357 2023-06-23 21:11:19.022270 gpt_code_search-0.0.3/LICENSE
--rw-r--r--   0        0        0     3472 2023-06-25 08:50:47.525612 gpt_code_search-0.0.3/README.md
--rw-r--r--   0        0        0        0 2023-06-23 04:13:32.205359 gpt_code_search-0.0.3/core/__init__.py
--rw-r--r--   0        0        0     5100 2023-06-25 09:12:28.089552 gpt_code_search-0.0.3/core/ai.py
--rw-r--r--   0        0        0     1568 2023-06-25 08:20:29.932487 gpt_code_search-0.0.3/core/config.py
--rw-r--r--   0        0        0     6748 2023-06-25 09:12:28.560468 gpt_code_search-0.0.3/core/functions.py
--rw-r--r--   0        0        0     3476 2023-06-25 09:04:29.759102 gpt_code_search-0.0.3/core/main.py
--rw-r--r--   0        0        0     1090 2023-06-25 08:37:42.132668 gpt_code_search-0.0.3/pyproject.toml
--rw-r--r--   0        0        0     4641 1970-01-01 00:00:00.000000 gpt_code_search-0.0.3/PKG-INFO
+-rw-r--r--   0        0        0    11357 2023-06-23 21:11:19.022270 gpt_code_search-0.0.4/LICENSE
+-rw-r--r--   0        0        0     7667 2023-06-25 22:07:11.211081 gpt_code_search-0.0.4/README.md
+-rw-r--r--   0        0        0        0 2023-06-23 04:13:32.205359 gpt_code_search-0.0.4/core/__init__.py
+-rw-r--r--   0        0        0     6040 2023-06-25 22:57:18.491657 gpt_code_search-0.0.4/core/ai.py
+-rw-r--r--   0        0        0     1104 2023-06-25 22:07:30.429077 gpt_code_search-0.0.4/core/analytics.py
+-rw-r--r--   0        0        0     2911 2023-06-25 19:52:46.261474 gpt_code_search-0.0.4/core/config.py
+-rw-r--r--   0        0        0     7897 2023-06-25 22:58:11.326099 gpt_code_search-0.0.4/core/functions.py
+-rw-r--r--   0        0        0     3072 2023-06-25 22:44:27.362555 gpt_code_search-0.0.4/core/main.py
+-rw-r--r--   0        0        0     1178 2023-06-25 22:14:56.252613 gpt_code_search-0.0.4/pyproject.toml
+-rw-r--r--   0        0        0     8976 1970-01-01 00:00:00.000000 gpt_code_search-0.0.4/PKG-INFO
```

### Comparing `gpt_code_search-0.0.3/LICENSE` & `gpt_code_search-0.0.4/LICENSE`

 * *Files identical despite different names*

### Comparing `gpt_code_search-0.0.3/core/ai.py` & `gpt_code_search-0.0.4/core/ai.py`

 * *Files 8% similar despite different names*

```diff
@@ -3,42 +3,54 @@
 
 import openai
 import requests
 from rich.markdown import Markdown
 
 from core.config import load_selected_model
 from core.functions import (
-    MAX_DEPTH,
     enabled_functions,
     get_contents_of_file,
     search_codebase,
     truncate_text_to_token_limit,
+    get_file_tree,
 )
 
 # Reduced from 16k to 14k to allow for prompt context
 MAX_TOKENS = 14_000
 
 PROMPT = """\
-You're a incredible powered coding assistant. Your role is to help users understand and navigate their codebases,
+You're a superpowered coding assistant. Your role is to help users understand and navigate their codebases,
 providing assistance across a range of tasks.
 
 You have access to three primary functions:
-- `search_codebase(keywords, max_depth)`: Search the codebase for a keywords with rankings based on the file path
-and contents. Higher ranking is better. Always use this function first. If there are no hits on a query, try some
-different keywords similar to the query. (eg). use interceptor, if interceptors is not found.
 
-
-- `get_contents_of_file(path)`: Fetch the contents of a file. Based on the answer from `search_codebase`, make a
-judgement on the most relevant file and fetch the contents of that file. Read at least 5 files before answering my
-calling this function multiple times. All the files should be different each time.
+- `search_codebase(keywords, max_depth)`: Search the codebase for keywords and rank the matches based on TF-IDF
+scoring.  Files with a keyword in the path are given additional weight in the scoring. Use this function first. If
+there are no hits on a query, try some different keywords similar to the query. (eg). use interceptor,
+if interceptors  is not found. Use at least 3 keywords for each query. If you cannot find a relevant file, say 'I
+don't know'. If you don't, you will be penalized.
+
+- `get_file_tree(start_path, max_depth, depth)`: Get the file tree of the project based on the current working
+directory. Access the current project root, with (./). Use this function to get an overview of the project structure.
+If you cannot find a relevant file, say 'I don't know'. If you don't, you will be penalized.
+
+- `get_contents_of_file(path)`: Fetch the contents of a file. Based on the answer from `search_codebase`,
+make a  judgement on the most relevant file and fetch the contents of that file. Read at least 5 files before
+answering  by calling this function multiple times. All the files should be different each time.
+
+For example, here are few queries and the expected results:
+
+- What does this project/codebase do? -> get_file_tree("./") -> get_contents_of_file("README.md")
+- How does user auth work -> search_codebase(["auth", "user"]) -> get_contents_of_file("auth.py")
+- How does logging work -> search_codebase(["logging", "log"]) -> get_contents_of_file("logging.py")
 
 You have a total of 10 function calls. Use them wisely.
 
-Use these tools to debug, create documentation, answer code-related queries, and generate code snippets
-in line with the project's style. You will always use these functions before answering a question, particularly
+Use these tools to debug, create documentation, answer code-related queries, and generate code snippets in line with
+the project's style. You will always use these functions before answering a question, particularly
 `search_codebase`. You will not answer any questions without using these functions first. If you cannot find a
 relevant file, say 'I don't know'. If you don't, you will be penalized.
 
 Once you find relevant files with the file tree or search functions, always use `get_contents_of_file` to fetch the
 contents of the file and review the contents of at least three files before answering.
 
 Compose responses in markdown with code when necessary. Your objective is to provide the most accurate and detailed
@@ -67,17 +79,15 @@
         )
         return response
     except requests.exceptions.HTTPError as http_err:
         logging.error(f"HTTP error occurred during ChatCompletion request: {http_err}")
         logging.error(f"Response content: {response.content}")
         return http_err
     except Exception as e:
-        logging.error(
-            "Unable to generate ChatCompletion response due to the following exception:"
-        )
+        logging.error("Unable to generate ChatCompletion response due to the following exception:")
         logging.error(f"Exception: {e}")
         return e
 
 
 def get_next_completion(previous_response, messages, functions):
     assistant_message = previous_response.json()["choices"][0]["message"]
     messages.append(assistant_message)
@@ -94,16 +104,19 @@
     if function_name == "get_contents_of_file":
         function_call = get_contents_of_file
         file_path = function_args.get("path")
         function_response = function_call(file_path)
     elif function_name == "search_codebase":
         function_call = search_codebase
         keywords = function_args.get("keywords")
-        max_depth = function_args.get("max_depth") or MAX_DEPTH
-        function_response = function_call(keywords, int(max_depth))
+        function_response = function_call(keywords)
+    elif function_name == "get_file_tree":
+        function_call = get_file_tree
+        start_path = function_args.get("start_path")
+        function_response = function_call(start_path)
     else:
         raise ValueError(f"Function {function_name} not found.")
 
     truncated_response = truncate_text_to_token_limit(function_response, MAX_TOKENS)
 
     messages.append(
         {
```

### Comparing `gpt_code_search-0.0.3/core/functions.py` & `gpt_code_search-0.0.4/core/functions.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,18 +1,20 @@
 import logging
 import os
-import re
 from typing import List, Union, Tuple
 
 import tiktoken
+from sklearn.feature_extraction.text import TfidfVectorizer
 
 IGNORED_FOLDERS = [
     "__pycache__",
     ".git",
     ".idea",
+    ".vscode",
+    "venv",
     "node_modules",
     ".bundle",
     ".gradle",
     "build",
     ".DS_Store",
     ".ipynb_checkpoints",
 ]
@@ -30,17 +32,15 @@
     "*.json",
     ".bat",
 ]
 
 MAX_DEPTH = 5
 
 
-def get_file_tree(
-    start_path: str = ".", max_depth: int = MAX_DEPTH, depth: int = 0
-) -> list:
+def get_file_tree(start_path: str = ".", max_depth: int = MAX_DEPTH, depth: int = 0) -> list:
     """
     Get the file tree of the project based on the current working directory.
     :param start_path: The path to the directory to start the search from.
     :param max_depth: The maximum depth of the search.
     :param depth: The current depth of the search.
     :return: The file tree.
     """
@@ -54,48 +54,48 @@
         if os.path.isfile(item_path):
             tree.append(item_path)
         elif os.path.isdir(item_path):
             tree += get_file_tree(item_path, max_depth, depth + 1)
     return tree
 
 
-def search_codebase(keywords: List[str], max_depth: int = 5) -> List[Tuple[str, int]]:
+def search_codebase(keywords: List[str], max_depth: int = MAX_DEPTH) -> List[Tuple[str, float]]:
     """
-    Search the codebase for a given list of keywords.
+    Search the codebase for a given list of keywords using TF-IDF vectorizer.
+    The file path is given additional weight in the score calculation.
     :param keywords: The list of keywords to search for.
     :param max_depth: The maximum depth of the search.
-    :return: A list of tuples where each tuple contains a file path and a rank.
-             Files with a keyword in the path are ranked higher than files with a keyword in the content.
+    :return: A list of tuples where each tuple contains a file path and a TF-IDF score.
+             Files with a higher TF-IDF score are ranked higher.
     """
     file_tree = get_file_tree(".", max_depth)
-    matching_files = {}
+    documents = []
+    PATH_WEIGHT = 10
+    keywords = [keyword.lower() for keyword in keywords]
 
     for file_path in file_tree:
         try:
-            rank = 0
             with open(file_path, "r", errors="ignore") as file:
                 contents = file.read()
-
-            if any(re.search(keyword, contents, re.IGNORECASE) for keyword in keywords):
-                rank = 1
-
-            if any(
-                re.search(keyword, file_path, re.IGNORECASE) for keyword in keywords
-            ):
-                rank = 2
-
-            if rank > 0:
-                matching_files[file_path] = rank
+            weighted_path = " ".join([file_path for _ in range(PATH_WEIGHT)])
+            documents.append(weighted_path + " " + contents)
         except Exception:
             logging.error("Error reading file: {}".format(file_path))
 
     logging.info("Searching for keywords: {}".format(keywords))
-    logging.info("Found {} matching files.".format(len(matching_files)))
-    matching_files = sorted(matching_files.items(), key=lambda x: x[1], reverse=True)
-    return matching_files
+
+    vectorizer = TfidfVectorizer(vocabulary=keywords, stop_words="english", max_features=100000)
+    tfidf_matrix = vectorizer.fit_transform(documents)
+    scores = tfidf_matrix.sum(axis=1)
+
+    file_scores = [(file_path, score) for file_path, score in zip(file_tree, scores)]
+    file_scores.sort(key=lambda x: x[1], reverse=True)
+
+    logging.info("Found {} matching files.".format(len(file_scores)))
+    return file_scores
 
 
 def get_contents_of_file(file_path: str) -> str:
     """
     Get the contents of a file.
     :param file_path: The path to the file.
     :return: The contents of the file, or an empty string if the file is not found.
@@ -109,17 +109,15 @@
 
 
 def count_tokens(text: str) -> int:
     encoding = tiktoken.get_encoding("cl100k_base")
     return len(encoding.encode_ordinary(text))
 
 
-def truncate_text_to_token_limit(
-    data: Union[str, List[str], List[Tuple[str, int]]], max_tokens: int
-):
+def truncate_text_to_token_limit(data: Union[str, List[str], List[Tuple[str, int]]], max_tokens: int):
     """
     Truncate the text (or list of strings or list of tuples) to fit within the maximum token limit.
     :param data: The text or list of strings or list of tuples to truncate.
     :param max_tokens: The maximum number of tokens.
     :return: The truncated text or list of strings or list of tuples.
     """
     if not data:
@@ -129,31 +127,32 @@
         chunks = data.split(" ")
     elif isinstance(data, list):
         if data and isinstance(data[0], tuple):
             chunks = [item[0] for item in data]
         else:
             chunks = data
     else:
-        raise ValueError(
-            "The input data should be a string or a list of strings or a list of tuples."
-        )
+        raise ValueError("The input data should be a string or a list of strings or a list of tuples.")
 
     total_tokens = sum(len(chunk.split(" ")) for chunk in chunks)
 
     while total_tokens > max_tokens:
         total_tokens -= len(chunks[-1].split(" "))
         chunks = chunks[:-1]
 
     if isinstance(data, str):
-        return " ".join(chunks)
+        truncated_text = " ".join(chunks)[:max_tokens]
+        return truncated_text
     elif data and isinstance(data[0], tuple):
         ranks = [item[1] for item in data[: len(chunks)]]
-        return list(zip(chunks, ranks))
+        truncated_list = list(zip(chunks, ranks))
+        return truncated_list
     else:
-        return chunks
+        truncated_list = chunks[:max_tokens]
+        return truncated_list
 
 
 def enabled_functions():
     return [
         {
             "name": "get_contents_of_file",
             "description": "Get the contents of a file. Returns empty string if the file is not found.",
@@ -166,45 +165,65 @@
                     },
                 },
                 "required": ["path"],
             },
         },
         {
             "name": "search_codebase",
-            "description": "Search the codebase for a given list of keywords and return ranked matches. Files with a "
-            "keyword in the path are ranked higher than files with a keyword in the content.",
+            "description": "Search the codebase for a given list of keywords and return ranked matches based on a "
+            "TF-IDF  scoring. Files with a keyword in the path are given additional weight in scoring "
+            "than files with a keyword in the content.",
             "returns": {
                 "type": "array",
                 "items": {
                     "type": "object",
                     "properties": {
                         "path": {
                             "type": "string",
                             "description": "The path to the file.",
                         },
                         "rank": {
-                            "type": "integer",
-                            "description": "Rank of the match. 2 if keyword found "
-                            "in file path, 1 if keyword found in file content.",
+                            "type": "number",
+                            "description": "TF-IDF score of the match. Higher score means more relevant to the "
+                            "keywords.",
                         },
                     },
                 },
-                "description": "List of file paths and ranks, sorted by rank in descending order.",
+                "description": "List of file paths and TF-IDF scores, sorted by score in descending order.",
             },
             "parameters": {
                 "type": "object",
                 "properties": {
                     "keywords": {
                         "type": "array",
                         "items": {"type": "string"},
-                        "description": "The list of keywords to search for. Format: ['keyword1', 'keyword2']",
-                    },
-                    "max_depth": {
-                        "type": "integer",
-                        "description": "The maximum depth of the search.",
-                        "default": 5,
+                        "description": "The list of keywords to search for. Format: ['keyword1', 'keyword2']. Please "
+                        "provide at least three keywords.",
                     },
                 },
                 "required": ["keywords"],
             },
         },
+        {
+            "name": "get_file_tree",
+            "description": "Get the file tree of the project based on the current working directory.",
+            "returns": {
+                "type": "array",
+                "items": {
+                    "type": "string",
+                    "description": "The path to a file in the file tree.",
+                },
+                "description": "List of file paths in the file tree.",
+            },
+            "parameters": {
+                "type": "object",
+                "properties": {
+                    "start_path": {
+                        "type": "string",
+                        "description": "The path to start the search from. Defaults to the current directory.",
+                        "default": ".",
+                    },
+                },
+                "required": [],
+            },
+        },
     ]
```

### Comparing `gpt_code_search-0.0.3/pyproject.toml` & `gpt_code_search-0.0.4/pyproject.toml`

 * *Files 13% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "gpt-code-search"
-version = "0.0.3"
+version = "0.0.4"
 description = "gpt-code-search enables you to search your codebase with natural language."
 authors = ["narenmanoharan <narenkmanoharan@gmail.com>", "skovy <smiskoviak@gmail.com>"]
 license = "Apache-2.0"
 readme = "README.md"
 packages = [{include = "core"}]
 homepage = "https://wolfia.com"
 repository = "https://github.com/wolfia-app/gpt-code-search"
@@ -12,25 +12,28 @@
 
 [tool.poetry.urls]
 issues = "https://github.com/wolfia-app/gpt-code-search/issues"
 discussions = "https://github.com/wolfia-app/gpt-code-search/discussions"
 wiki = "https://github.com/wolfia-app/gpt-code-search/wiki"
 
 [tool.poetry.scripts]
-gpt-code-search = "core.main:app"
+gcs = "core.main:app"
 
 [tool.poetry.dependencies]
-python = "^3.10"
+python = "^3.9.17"
 typer = {extras = ["all"], version = "^0.9.0"}
 rich = "^13.4.2"
 tiktoken = "^0.4.0"
 openai = "^0.27.8"
 termcolor = "^2.3.0"
 requests = "^2.31.0"
 toml = "^0.10.2"
+sentry-sdk = {extras = ["flask"], version = "^1.26.0"}
+posthog = "^3.0.1"
+scikit-learn = "^1.2.2"
 
 [tool.poetry.dev-dependencies]
 pre-commit = "^2.15.0"
 
 [build-system]
 requires = ["poetry-core"]
 build-backend = "poetry.core.masonry.api"
```

