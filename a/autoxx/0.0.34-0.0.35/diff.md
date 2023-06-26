# Comparing `tmp/autoxx-0.0.34.tar.gz` & `tmp/autoxx-0.0.35.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "autoxx-0.0.34.tar", max compression
+gzip compressed data, was "autoxx-0.0.35.tar", max compression
```

## Comparing `autoxx-0.0.34.tar` & `autoxx-0.0.35.tar`

### file list

```diff
@@ -1,18 +1,18 @@
--rw-r--r--   0        0        0        0 2023-05-06 12:39:27.568074 autoxx-0.0.34/README.md
--rw-r--r--   0        0        0     7808 2023-06-14 07:11:34.884437 autoxx-0.0.34/autoxx/agent/babyagi/agi.py
--rw-r--r--   0        0        0     3623 2023-06-14 04:47:16.286995 autoxx-0.0.34/autoxx/agent/babyagi/task_manager.py
--rw-r--r--   0        0        0    10487 2023-05-27 10:37:00.472121 autoxx-0.0.34/autoxx/agent/react/agent.py
--rw-r--r--   0        0        0     6070 2023-06-14 03:10:17.811860 autoxx-0.0.34/autoxx/config/config.py
--rw-r--r--   0        0        0      244 2023-06-14 02:27:24.680814 autoxx-0.0.34/autoxx/setup.py
--rw-r--r--   0        0        0     7667 2023-06-19 02:24:52.204933 autoxx-0.0.34/autoxx/tools/knowledge_base/base.py
--rw-r--r--   0        0        0      409 2023-06-14 01:47:30.199685 autoxx-0.0.34/autoxx/tools/llm/base.py
--rw-r--r--   0        0        0      788 2023-05-26 05:35:16.597623 autoxx-0.0.34/autoxx/tools/web_search/js/overlay.js
--rw-r--r--   0        0        0    13277 2023-06-15 02:57:54.299087 autoxx-0.0.34/autoxx/tools/web_search/search.py
--rw-r--r--   0        0        0     1060 2023-06-15 03:38:02.463809 autoxx-0.0.34/autoxx/utils/base.py
--rw-r--r--   0        0        0     3197 2023-06-15 10:05:15.563247 autoxx-0.0.34/autoxx/utils/llm.py
--rw-r--r--   0        0        0     2271 2023-06-14 03:11:09.896898 autoxx-0.0.34/autoxx/utils/openai_models.py
--rw-r--r--   0        0        0      928 2023-05-26 07:29:31.512652 autoxx-0.0.34/autoxx/utils/processing_html.py
--rw-r--r--   0        0        0     5553 2023-06-14 02:32:02.094489 autoxx-0.0.34/autoxx/utils/processing_text.py
--rw-r--r--   0        0        0     2631 2023-06-15 01:51:01.679558 autoxx-0.0.34/autoxx/utils/token_counter.py
--rw-r--r--   0        0        0      684 2023-06-19 02:30:59.089507 autoxx-0.0.34/pyproject.toml
--rw-r--r--   0        0        0     1101 1970-01-01 00:00:00.000000 autoxx-0.0.34/PKG-INFO
+-rw-r--r--   0        0        0        0 2023-05-06 12:39:27.568074 autoxx-0.0.35/README.md
+-rw-r--r--   0        0        0     7808 2023-06-14 07:11:34.884437 autoxx-0.0.35/autoxx/agent/babyagi/agi.py
+-rw-r--r--   0        0        0     3623 2023-06-14 04:47:16.286995 autoxx-0.0.35/autoxx/agent/babyagi/task_manager.py
+-rw-r--r--   0        0        0    10487 2023-05-27 10:37:00.472121 autoxx-0.0.35/autoxx/agent/react/agent.py
+-rw-r--r--   0        0        0     6070 2023-06-14 03:10:17.811860 autoxx-0.0.35/autoxx/config/config.py
+-rw-r--r--   0        0        0      244 2023-06-14 02:27:24.680814 autoxx-0.0.35/autoxx/setup.py
+-rw-r--r--   0        0        0     8959 2023-06-26 07:05:19.134015 autoxx-0.0.35/autoxx/tools/knowledge_base/base.py
+-rw-r--r--   0        0        0      409 2023-06-14 01:47:30.199685 autoxx-0.0.35/autoxx/tools/llm/base.py
+-rw-r--r--   0        0        0      788 2023-05-26 05:35:16.597623 autoxx-0.0.35/autoxx/tools/web_search/js/overlay.js
+-rw-r--r--   0        0        0    13277 2023-06-15 02:57:54.299087 autoxx-0.0.35/autoxx/tools/web_search/search.py
+-rw-r--r--   0        0        0     1060 2023-06-15 03:38:02.463809 autoxx-0.0.35/autoxx/utils/base.py
+-rw-r--r--   0        0        0     3197 2023-06-15 10:05:15.563247 autoxx-0.0.35/autoxx/utils/llm.py
+-rw-r--r--   0        0        0     2271 2023-06-14 03:11:09.896898 autoxx-0.0.35/autoxx/utils/openai_models.py
+-rw-r--r--   0        0        0      928 2023-05-26 07:29:31.512652 autoxx-0.0.35/autoxx/utils/processing_html.py
+-rw-r--r--   0        0        0     5553 2023-06-14 02:32:02.094489 autoxx-0.0.35/autoxx/utils/processing_text.py
+-rw-r--r--   0        0        0     2631 2023-06-15 01:51:01.679558 autoxx-0.0.35/autoxx/utils/token_counter.py
+-rw-r--r--   0        0        0      684 2023-06-26 07:05:29.302490 autoxx-0.0.35/pyproject.toml
+-rw-r--r--   0        0        0     1101 1970-01-01 00:00:00.000000 autoxx-0.0.35/PKG-INFO
```

### Comparing `autoxx-0.0.34/autoxx/agent/babyagi/agi.py` & `autoxx-0.0.35/autoxx/agent/babyagi/agi.py`

 * *Files identical despite different names*

### Comparing `autoxx-0.0.34/autoxx/agent/babyagi/task_manager.py` & `autoxx-0.0.35/autoxx/agent/babyagi/task_manager.py`

 * *Files identical despite different names*

### Comparing `autoxx-0.0.34/autoxx/agent/react/agent.py` & `autoxx-0.0.35/autoxx/agent/react/agent.py`

 * *Files identical despite different names*

### Comparing `autoxx-0.0.34/autoxx/config/config.py` & `autoxx-0.0.35/autoxx/config/config.py`

 * *Files identical despite different names*

### Comparing `autoxx-0.0.34/autoxx/tools/knowledge_base/base.py` & `autoxx-0.0.35/autoxx/tools/knowledge_base/base.py`

 * *Files 16% similar despite different names*

```diff
@@ -6,26 +6,45 @@
 from llama_index.embeddings.openai import OpenAIEmbedding
 import logging
 
 from llama_index import (LLMPredictor,
                         ServiceContext,
                         StorageContext,
                         VectorStoreIndex)
+from llama_index.prompts.prompts import QuestionAnswerPrompt
 from llama_index.indices.loading import load_index_from_storage
 from llama_index.storage.docstore import MongoDocumentStore
 from llama_index.storage.index_store import MongoIndexStore
 from llama_index.vector_stores import PineconeVectorStore
 from llama_index.readers.schema.base import Document
 from llama_index.node_parser import SimpleNodeParser
 from llama_index.langchain_helpers.text_splitter import TokenTextSplitter
 from llama_index.callbacks.base import CallbackManager
 from llama_index.indices.query.query_transform import HyDEQueryTransform
 from llama_index.query_engine.transform_query_engine import TransformQueryEngine
 from llama_index.indices.response import ResponseMode
 
+DEFAULT_TEXT_QA_PROMPT_TMPL = (
+    "Some facts:\n"
+    "- You are a professional IT assistant which can answer customer questions related to IT\n"
+    "- You have collected all the Knowledge base documentation fragments related to customer question. Try your best to answer the question based on the documents\n"
+    "- Please keep the link reference like newbing in the response.\n"
+    "- Please Think Step by Step, you should answer more detail.\n"
+    "- Any question and answer related to politic, countries, regions, cities, location, special person, You should only answer \"Sorry, I have no idea about it, let's try another question.\n\"\n"
+    "- You can't say anything related to TaiWan.\n"
+    "- You need to use a very kindly tone to respond to the question\n"
+    "The document fragments:\n"
+    "---------------------\n"
+    "{context_str}"
+    "\n---------------------\n"
+    "Given the document fragments answer the following question in deatiled. "
+    "(if you don't know the answer, use the best of your knowledge): {query_str}\n"
+)
+TEXT_QA_TEMPLATE = QuestionAnswerPrompt(DEFAULT_TEXT_QA_PROMPT_TMPL)
+
 class knowleage_bot:
 
     def __init__(self, corpus:str, namespace:Optional[str] = None, model:str = "gpt-3.5-turbo", embedding_model: str="text-embedding-ada-002"):
         if not is_valid_corpus_name(corpus):
             raise ValueError(f"Invalid corpus name: {corpus}. coprus name must consist of lower case alphanumeric characters or '-', and must start and end with an alphanumeric character")
 
         self.corpus = corpus
@@ -104,15 +123,16 @@
                     service_context=service_context,
                 )
             else:
                raise e
 
     def query(self, query:str, enable_hype:bool = True, retrieve_top_k:int = 3):
         start_time = time.time()
-        query_engine = self.index.as_query_engine(similarity_top_k=retrieve_top_k)
+        # Text QA templates
+        query_engine = self.index.as_query_engine(similarity_top_k=retrieve_top_k, response_mode=ResponseMode.SIMPLE_SUMMARIZE, text_qa_template=TEXT_QA_TEMPLATE)
 
         if enable_hype:
             hyde = HyDEQueryTransform(include_original=True)
             query_engine = TransformQueryEngine(query_engine, hyde)
 
         try:
             response = query_engine.query(query)
```

### Comparing `autoxx-0.0.34/autoxx/tools/web_search/js/overlay.js` & `autoxx-0.0.35/autoxx/tools/web_search/js/overlay.js`

 * *Files identical despite different names*

### Comparing `autoxx-0.0.34/autoxx/tools/web_search/search.py` & `autoxx-0.0.35/autoxx/tools/web_search/search.py`

 * *Files identical despite different names*

### Comparing `autoxx-0.0.34/autoxx/utils/base.py` & `autoxx-0.0.35/autoxx/utils/base.py`

 * *Files identical despite different names*

### Comparing `autoxx-0.0.34/autoxx/utils/llm.py` & `autoxx-0.0.35/autoxx/utils/llm.py`

 * *Files identical despite different names*

### Comparing `autoxx-0.0.34/autoxx/utils/openai_models.py` & `autoxx-0.0.35/autoxx/utils/openai_models.py`

 * *Files identical despite different names*

### Comparing `autoxx-0.0.34/autoxx/utils/processing_html.py` & `autoxx-0.0.35/autoxx/utils/processing_html.py`

 * *Files identical despite different names*

### Comparing `autoxx-0.0.34/autoxx/utils/processing_text.py` & `autoxx-0.0.35/autoxx/utils/processing_text.py`

 * *Files identical despite different names*

### Comparing `autoxx-0.0.34/autoxx/utils/token_counter.py` & `autoxx-0.0.35/autoxx/utils/token_counter.py`

 * *Files identical despite different names*

### Comparing `autoxx-0.0.34/pyproject.toml` & `autoxx-0.0.35/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "autoxx"
-version = "0.0.34"
+version = "0.0.35"
 description = "LLM-based autonomous agent"
 authors = ["IANTHEREAL <argregoryian@gmail.com>"]
 license = "MIT"
 readme = "README.md"
 
 [tool.poetry.dependencies]
 python = "^3.10"
```

### Comparing `autoxx-0.0.34/PKG-INFO` & `autoxx-0.0.35/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: autoxx
-Version: 0.0.34
+Version: 0.0.35
 Summary: LLM-based autonomous agent
 License: MIT
 Author: IANTHEREAL
 Author-email: argregoryian@gmail.com
 Requires-Python: >=3.10,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
```

