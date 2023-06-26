# Comparing `tmp/gpt_code_search-0.0.5.tar.gz` & `tmp/gpt_code_search-0.0.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "gpt_code_search-0.0.5.tar", max compression
+gzip compressed data, was "gpt_code_search-0.0.6.tar", max compression
```

## Comparing `gpt_code_search-0.0.5.tar` & `gpt_code_search-0.0.6.tar`

### file list

```diff
@@ -1,12 +1,12 @@
--rw-r--r--   0        0        0    11357 2023-06-23 21:11:19.022270 gpt_code_search-0.0.5/LICENSE
--rw-r--r--   0        0        0     7667 2023-06-25 22:07:11.211081 gpt_code_search-0.0.5/README.md
--rw-r--r--   0        0        0        0 2023-06-23 04:13:32.205359 gpt_code_search-0.0.5/core/__init__.py
--rw-r--r--   0        0        0     6035 2023-06-26 02:41:46.649895 gpt_code_search-0.0.5/core/ai.py
--rw-r--r--   0        0        0     1104 2023-06-25 22:07:30.429077 gpt_code_search-0.0.5/core/analytics.py
--rw-r--r--   0        0        0     2911 2023-06-25 19:52:46.261474 gpt_code_search-0.0.5/core/config.py
--rw-r--r--   0        0        0     7637 2023-06-26 02:43:17.380254 gpt_code_search-0.0.5/core/functions.py
--rw-r--r--   0        0        0     3072 2023-06-25 22:44:27.362555 gpt_code_search-0.0.5/core/main.py
--rw-r--r--   0        0        0        0 2023-06-26 01:55:02.493714 gpt_code_search-0.0.5/core/tests/__init__.py
--rw-r--r--   0        0        0     1057 2023-06-26 03:07:33.872866 gpt_code_search-0.0.5/core/tests/test_truncate_text.py
--rw-r--r--   0        0        0     1258 2023-06-26 02:50:42.325898 gpt_code_search-0.0.5/pyproject.toml
--rw-r--r--   0        0        0     8976 1970-01-01 00:00:00.000000 gpt_code_search-0.0.5/PKG-INFO
+-rw-r--r--   0        0        0    11357 2023-06-23 21:11:19.022270 gpt_code_search-0.0.6/LICENSE
+-rw-r--r--   0        0        0     7511 2023-06-26 14:56:05.849955 gpt_code_search-0.0.6/README.md
+-rw-r--r--   0        0        0        0 2023-06-23 04:13:32.205359 gpt_code_search-0.0.6/core/__init__.py
+-rw-r--r--   0        0        0     6035 2023-06-26 02:41:46.649895 gpt_code_search-0.0.6/core/ai.py
+-rw-r--r--   0        0        0     1104 2023-06-25 22:07:30.429077 gpt_code_search-0.0.6/core/analytics.py
+-rw-r--r--   0        0        0     2911 2023-06-25 19:52:46.261474 gpt_code_search-0.0.6/core/config.py
+-rw-r--r--   0        0        0     7637 2023-06-26 02:43:17.380254 gpt_code_search-0.0.6/core/functions.py
+-rw-r--r--   0        0        0     3072 2023-06-25 22:44:27.362555 gpt_code_search-0.0.6/core/main.py
+-rw-r--r--   0        0        0        0 2023-06-26 01:55:02.493714 gpt_code_search-0.0.6/core/tests/__init__.py
+-rw-r--r--   0        0        0      968 2023-06-26 14:44:25.615029 gpt_code_search-0.0.6/core/tests/test_truncate_text.py
+-rw-r--r--   0        0        0     1258 2023-06-26 15:49:06.690608 gpt_code_search-0.0.6/pyproject.toml
+-rw-r--r--   0        0        0     8870 1970-01-01 00:00:00.000000 gpt_code_search-0.0.6/PKG-INFO
```

### Comparing `gpt_code_search-0.0.5/LICENSE` & `gpt_code_search-0.0.6/LICENSE`

 * *Files identical despite different names*

### Comparing `gpt_code_search-0.0.5/README.md` & `gpt_code_search-0.0.6/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,7 +1,38 @@
+Metadata-Version: 2.1
+Name: gpt-code-search
+Version: 0.0.6
+Summary: gpt-code-search enables you to search your codebase with natural language.
+Home-page: https://wolfia.com
+License: Apache-2.0
+Keywords: gpt,code,search,wolfia,gpt4,llm
+Author: narenmanoharan
+Author-email: narenkmanoharan@gmail.com
+Requires-Python: >=3.8.17,<4.0.0
+Classifier: License :: OSI Approved :: Apache Software License
+Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
+Requires-Dist: openai (>=0.27.8,<0.28.0)
+Requires-Dist: posthog (>=3.0.1,<4.0.0)
+Requires-Dist: requests (>=2.31.0,<3.0.0)
+Requires-Dist: rich (>=13.4.2,<14.0.0)
+Requires-Dist: scikit-learn (>=1.2.2,<2.0.0)
+Requires-Dist: sentry-sdk[flask] (>=1.26.0,<2.0.0)
+Requires-Dist: termcolor (>=2.3.0,<3.0.0)
+Requires-Dist: tiktoken (>=0.4.0,<0.5.0)
+Requires-Dist: toml (>=0.10.2,<0.11.0)
+Requires-Dist: typer[all] (>=0.9.0,<0.10.0)
+Project-URL: Repository, https://github.com/wolfia-app/gpt-code-search
+Project-URL: discussions, https://github.com/wolfia-app/gpt-code-search/discussions
+Project-URL: issues, https://github.com/wolfia-app/gpt-code-search/issues
+Project-URL: wiki, https://github.com/wolfia-app/gpt-code-search/wiki
+Description-Content-Type: text/markdown
+
 <div align="center">
   <h1>gpt-code-search</h1>
   <img
     height="240"
     width="240"
     alt="logo"
     src="https://raw.githubusercontent.com/wolfia-app/gpt-code-search/main/public/logo.png"
@@ -82,20 +113,29 @@
 
 The only data sent to LLM is the question you ask and the code snippets that it requests related to your question. All code snippets are retrieved from your local machine.
 
 ## Limitations
 
 This does have some limitations, namely:
 
-- The LLM is unable to search and load context across mutliple files at once. This means that if you ask a question that requires context from multiple files, you will need to ask multiple questions.
+- The LLM is unable to load context across multiple files at once. This means that if you ask a question that requires context from multiple files, you will need to ask multiple questions.
 - Specify the file name and keywords in your question to improve accuracy. For example, if you want to ask a question about `analytics.py`, mention the file name in your question.
 - The level of search and retrieval is limited by the context window, which refers to the scope of the search conducted by the tool, meaning that we can only search 5 levels deep in the file system. So you need to run the tool from the folder/package closest to the code you want to search.
 
 These limitations lead to suboptimal results in a few cases, but we're working on improving this. **We wanted to get this tool out there as soon as possible to get feedback and iterate on it!**
 
+## Roadmap
+
+- [ ] Use vector embeddings to improve search and retrieval
+- [ ] Add support for generating code and saving it to a file
+- [ ] Support for searching across multiple codebases
+- [ ] Allow the model to create new functions that it can then execute
+- [ ] Use [guidance](https://github.com/microsoft/guidance) to improve prompts
+- [ ] Add support for additional models (Claude, Bedrock, etc)
+
 ## Wolfia Codex
 
 `gpt-code-search` is a simplified version of [Wolfia Codex](https://wolfia.com), a cloud tool that enables you to ask any question about open source and private code bases like [`Langchain`](https://wolfia.com/?projectId=2b964031-0ce8-472a-abb7-27079a7b84f3), [`Vercel ai`](https://wolfia.com/?projectId=4710df1f-43f8-4d30-863b-d67876ae0f06), or [`gpt-engineer`](https://wolfia.com/?projectId=8d9dd449-da2d-410e-a4fc-f2ff75a30f73).
 
 If you're looking for a more powerful tool which solves the above limitations by using vector embeddings and a more powerful search and retrieval system, or avoiding the setup, check out [Wolfia Codex](https://wolfia.com), search codebases, share your questions and answers, and more!
 
 ## Analytics
@@ -115,42 +155,14 @@
 - uuid - a unique identifier for the user
 - model - the model used for the query
 - usage - the type of usage (query_count, query_at, query_execution_time)
 ```
 
 **Note: We do not collect any PII (ip-address), queries or code snippets.**
 
-## Development
-
-The project uses [poetry](https://python-poetry.org/) for dependency management and packaging. The codebase is structured in a modular fashion, making it easier for contributions. To get started, install poetry and run the following commands:
-
-```bash
-# Install dependencies
-poetry install
-```
-
-Run the project
-
-```bash
-# Run the project
-poetry run python core/main.py
-```
-
-Install pre-commit hooks
-
-```bash
-# Install pre-commit hooks
-poetry run pre-commit install
-```
-
-```bash
-# Setup local development
-export LOCAL_DEV=true
-```
-
 ## Contributing
 
 We love contributions from the community! ❤️ If you'd like to contribute, feel free to fork the repository and submit a pull request.
 
 Please read our [Code of Conduct](CODE_OF_CONDUCT.md) and [Contributing Guide](CONTRIBUTING.md) for more detailed steps and information.
 
 ## Code of Conduct
@@ -164,7 +176,8 @@
 ## Feedback
 
 Your feedback is very important to us! If you have ideas for how we can improve `gpt-code-search`, we'd love to hear from you. Please [open an issue](https://github.com/wolfia-app/gpt-code-search/issues) with your suggestions, or you can email [support@wolfia.com](mailto:support@wolfia.com).
 
 ## License
 
 Apache 2.0 © [Wolfia](https://wolfia.com)
+
```

### Comparing `gpt_code_search-0.0.5/core/ai.py` & `gpt_code_search-0.0.6/core/ai.py`

 * *Files identical despite different names*

### Comparing `gpt_code_search-0.0.5/core/analytics.py` & `gpt_code_search-0.0.6/core/analytics.py`

 * *Files identical despite different names*

### Comparing `gpt_code_search-0.0.5/core/config.py` & `gpt_code_search-0.0.6/core/config.py`

 * *Files identical despite different names*

### Comparing `gpt_code_search-0.0.5/core/functions.py` & `gpt_code_search-0.0.6/core/functions.py`

 * *Files identical despite different names*

### Comparing `gpt_code_search-0.0.5/core/main.py` & `gpt_code_search-0.0.6/core/main.py`

 * *Files identical despite different names*

### Comparing `gpt_code_search-0.0.5/core/tests/test_truncate_text.py` & `gpt_code_search-0.0.6/core/tests/test_truncate_text.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,31 +1,32 @@
 import pytest
+
 from core.functions import truncate_text_to_token_limit, count_tokens
 
 
 @pytest.fixture(scope="module")
 def max_tokens():
     return 5
 
 
 @pytest.mark.parametrize(
-    "data, expected",
+    "data",
     [
-        ("", True),
-        ("This is a long string with many tokens", True),
-        (["This", "is", "a", "sample", "sentence", "and", "this", "is", "another"], True),
-        ([("This", 1), ("is", 2), ("a", 3), ("sample", 4), ("sentence", 5), ("and", 6), ("this", 7), ("is", 8)], True),
-        ("This", True),
-        (["T", "h", "i", "s"], True),
-        ([("T", 1), ("h", 2), ("i", 3), ("s", 4)], True),
-        ("This is a string with special chars!@#", True),
+        "",
+        "This is a long string with many tokens",
+        (["This", "is", "a", "sample", "sentence", "and", "this", "is", "another"]),
+        ([("This", 1), ("is", 2), ("a", 3), ("sample", 4), ("sentence", 5), ("and", 6), ("this", 7), ("is", 8)]),
+        "This",
+        (["T", "h", "i", "s"]),
+        ([("T", 1), ("h", 2), ("i", 3), ("s", 4)]),
+        "This is a string with special chars!@#",
     ],
 )
-def test_truncate_text_to_token_limit(data, expected, max_tokens):
+def test_truncate_text_to_token_limit(data, max_tokens):
     result = truncate_text_to_token_limit(data, max_tokens)
-    assert (count_tokens(result) <= max_tokens) == expected
+    assert count_tokens(result) <= max_tokens
 
 
 def test_truncate_text_invalid_data_type_in_list(max_tokens):
     data = ["This", 1, ("is", 2)]
     with pytest.raises(ValueError):
         truncate_text_to_token_limit(data, max_tokens)
```

### Comparing `gpt_code_search-0.0.5/pyproject.toml` & `gpt_code_search-0.0.6/pyproject.toml`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "gpt-code-search"
-version = "0.0.5"
+version = "0.0.6"
 description = "gpt-code-search enables you to search your codebase with natural language."
 authors = ["narenmanoharan <narenkmanoharan@gmail.com>", "skovy <smiskoviak@gmail.com>"]
 license = "Apache-2.0"
 readme = "README.md"
 packages = [{include = "core"}]
 homepage = "https://wolfia.com"
 repository = "https://github.com/wolfia-app/gpt-code-search"
@@ -15,15 +15,15 @@
 discussions = "https://github.com/wolfia-app/gpt-code-search/discussions"
 wiki = "https://github.com/wolfia-app/gpt-code-search/wiki"
 
 [tool.poetry.scripts]
 gcs = "core.main:app"
 
 [tool.poetry.dependencies]
-python = "^3.9.17"
+python = "^3.8.17"
 typer = {extras = ["all"], version = "^0.9.0"}
 rich = "^13.4.2"
 tiktoken = "^0.4.0"
 openai = "^0.27.8"
 termcolor = "^2.3.0"
 requests = "^2.31.0"
 toml = "^0.10.2"
```

### Comparing `gpt_code_search-0.0.5/PKG-INFO` & `gpt_code_search-0.0.6/README.md`

 * *Files 18% similar despite different names*

```diff
@@ -1,37 +1,7 @@
-Metadata-Version: 2.1
-Name: gpt-code-search
-Version: 0.0.5
-Summary: gpt-code-search enables you to search your codebase with natural language.
-Home-page: https://wolfia.com
-License: Apache-2.0
-Keywords: gpt,code,search,wolfia,gpt4,llm
-Author: narenmanoharan
-Author-email: narenkmanoharan@gmail.com
-Requires-Python: >=3.9.17,<4.0.0
-Classifier: License :: OSI Approved :: Apache Software License
-Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.10
-Classifier: Programming Language :: Python :: 3.11
-Requires-Dist: openai (>=0.27.8,<0.28.0)
-Requires-Dist: posthog (>=3.0.1,<4.0.0)
-Requires-Dist: requests (>=2.31.0,<3.0.0)
-Requires-Dist: rich (>=13.4.2,<14.0.0)
-Requires-Dist: scikit-learn (>=1.2.2,<2.0.0)
-Requires-Dist: sentry-sdk[flask] (>=1.26.0,<2.0.0)
-Requires-Dist: termcolor (>=2.3.0,<3.0.0)
-Requires-Dist: tiktoken (>=0.4.0,<0.5.0)
-Requires-Dist: toml (>=0.10.2,<0.11.0)
-Requires-Dist: typer[all] (>=0.9.0,<0.10.0)
-Project-URL: Repository, https://github.com/wolfia-app/gpt-code-search
-Project-URL: discussions, https://github.com/wolfia-app/gpt-code-search/discussions
-Project-URL: issues, https://github.com/wolfia-app/gpt-code-search/issues
-Project-URL: wiki, https://github.com/wolfia-app/gpt-code-search/wiki
-Description-Content-Type: text/markdown
-
 <div align="center">
   <h1>gpt-code-search</h1>
   <img
     height="240"
     width="240"
     alt="logo"
     src="https://raw.githubusercontent.com/wolfia-app/gpt-code-search/main/public/logo.png"
@@ -112,20 +82,29 @@
 
 The only data sent to LLM is the question you ask and the code snippets that it requests related to your question. All code snippets are retrieved from your local machine.
 
 ## Limitations
 
 This does have some limitations, namely:
 
-- The LLM is unable to search and load context across mutliple files at once. This means that if you ask a question that requires context from multiple files, you will need to ask multiple questions.
+- The LLM is unable to load context across multiple files at once. This means that if you ask a question that requires context from multiple files, you will need to ask multiple questions.
 - Specify the file name and keywords in your question to improve accuracy. For example, if you want to ask a question about `analytics.py`, mention the file name in your question.
 - The level of search and retrieval is limited by the context window, which refers to the scope of the search conducted by the tool, meaning that we can only search 5 levels deep in the file system. So you need to run the tool from the folder/package closest to the code you want to search.
 
 These limitations lead to suboptimal results in a few cases, but we're working on improving this. **We wanted to get this tool out there as soon as possible to get feedback and iterate on it!**
 
+## Roadmap
+
+- [ ] Use vector embeddings to improve search and retrieval
+- [ ] Add support for generating code and saving it to a file
+- [ ] Support for searching across multiple codebases
+- [ ] Allow the model to create new functions that it can then execute
+- [ ] Use [guidance](https://github.com/microsoft/guidance) to improve prompts
+- [ ] Add support for additional models (Claude, Bedrock, etc)
+
 ## Wolfia Codex
 
 `gpt-code-search` is a simplified version of [Wolfia Codex](https://wolfia.com), a cloud tool that enables you to ask any question about open source and private code bases like [`Langchain`](https://wolfia.com/?projectId=2b964031-0ce8-472a-abb7-27079a7b84f3), [`Vercel ai`](https://wolfia.com/?projectId=4710df1f-43f8-4d30-863b-d67876ae0f06), or [`gpt-engineer`](https://wolfia.com/?projectId=8d9dd449-da2d-410e-a4fc-f2ff75a30f73).
 
 If you're looking for a more powerful tool which solves the above limitations by using vector embeddings and a more powerful search and retrieval system, or avoiding the setup, check out [Wolfia Codex](https://wolfia.com), search codebases, share your questions and answers, and more!
 
 ## Analytics
@@ -145,42 +124,14 @@
 - uuid - a unique identifier for the user
 - model - the model used for the query
 - usage - the type of usage (query_count, query_at, query_execution_time)
 ```
 
 **Note: We do not collect any PII (ip-address), queries or code snippets.**
 
-## Development
-
-The project uses [poetry](https://python-poetry.org/) for dependency management and packaging. The codebase is structured in a modular fashion, making it easier for contributions. To get started, install poetry and run the following commands:
-
-```bash
-# Install dependencies
-poetry install
-```
-
-Run the project
-
-```bash
-# Run the project
-poetry run python core/main.py
-```
-
-Install pre-commit hooks
-
-```bash
-# Install pre-commit hooks
-poetry run pre-commit install
-```
-
-```bash
-# Setup local development
-export LOCAL_DEV=true
-```
-
 ## Contributing
 
 We love contributions from the community! ❤️ If you'd like to contribute, feel free to fork the repository and submit a pull request.
 
 Please read our [Code of Conduct](CODE_OF_CONDUCT.md) and [Contributing Guide](CONTRIBUTING.md) for more detailed steps and information.
 
 ## Code of Conduct
@@ -194,8 +145,7 @@
 ## Feedback
 
 Your feedback is very important to us! If you have ideas for how we can improve `gpt-code-search`, we'd love to hear from you. Please [open an issue](https://github.com/wolfia-app/gpt-code-search/issues) with your suggestions, or you can email [support@wolfia.com](mailto:support@wolfia.com).
 
 ## License
 
 Apache 2.0 © [Wolfia](https://wolfia.com)
-
```

