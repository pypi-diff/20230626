# Comparing `tmp/agent_summarizer-0.1.1.tar.gz` & `tmp/agent_summarizer-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "agent_summarizer-0.1.1.tar", max compression
+gzip compressed data, was "agent_summarizer-0.1.2.tar", max compression
```

## Comparing `agent_summarizer-0.1.1.tar` & `agent_summarizer-0.1.2.tar`

### file list

```diff
@@ -1,7 +1,7 @@
--rw-r--r--   0        0        0    11357 2023-06-19 09:36:08.930199 agent_summarizer-0.1.1/LICENSE
--rw-r--r--   0        0        0      462 2023-06-23 12:47:40.304840 agent_summarizer-0.1.1/README.md
--rw-r--r--   0        0        0      108 2023-06-19 13:40:24.114440 agent_summarizer-0.1.1/agent_summarizer/__init__.py
--rw-r--r--   0        0        0      642 2023-06-23 12:29:06.788197 agent_summarizer-0.1.1/agent_summarizer/link_type.py
--rw-r--r--   0        0        0     4202 2023-06-23 14:41:58.103765 agent_summarizer-0.1.1/agent_summarizer/summarizer.py
--rw-r--r--   0        0        0      543 2023-06-23 14:42:14.969918 agent_summarizer-0.1.1/pyproject.toml
--rw-r--r--   0        0        0     1194 1970-01-01 00:00:00.000000 agent_summarizer-0.1.1/PKG-INFO
+-rw-r--r--   0        0        0    11357 2023-06-19 09:36:08.930199 agent_summarizer-0.1.2/LICENSE
+-rw-r--r--   0        0        0      462 2023-06-23 12:47:40.304840 agent_summarizer-0.1.2/README.md
+-rw-r--r--   0        0        0      118 2023-06-26 09:26:01.484033 agent_summarizer-0.1.2/agent_summarizer/__init__.py
+-rw-r--r--   0        0        0      642 2023-06-23 12:29:06.788197 agent_summarizer-0.1.2/agent_summarizer/link_type.py
+-rw-r--r--   0        0        0     4326 2023-06-26 09:25:40.513538 agent_summarizer-0.1.2/agent_summarizer/summarizer.py
+-rw-r--r--   0        0        0      543 2023-06-26 09:31:34.631782 agent_summarizer-0.1.2/pyproject.toml
+-rw-r--r--   0        0        0     1194 1970-01-01 00:00:00.000000 agent_summarizer-0.1.2/PKG-INFO
```

### Comparing `agent_summarizer-0.1.1/LICENSE` & `agent_summarizer-0.1.2/LICENSE`

 * *Files identical despite different names*

### Comparing `agent_summarizer-0.1.1/agent_summarizer/link_type.py` & `agent_summarizer-0.1.2/agent_summarizer/link_type.py`

 * *Files identical despite different names*

### Comparing `agent_summarizer-0.1.1/agent_summarizer/summarizer.py` & `agent_summarizer-0.1.2/agent_summarizer/summarizer.py`

 * *Files 2% similar despite different names*

```diff
@@ -88,26 +88,15 @@
   soup = get_the_page_content(url)
   element = soup.find('div', attrs={'id': 'abstract'})
   text = None
   if element is not None:
     text = element.get_text()
   return text
 
-def summarize(url, llm):
-  text_splitter = RecursiveCharacterTextSplitter()
-  prompt_template = """Write a concise summary of the following text. 
-  I want you to provide me with bullet points highlighting the core ideas
-  of this piece. Keep each bullet point under one or two sentences.
-
-    {text}
-
-  Bullet points:"""
-  summarizer_prompt = PromptTemplate(template=prompt_template,
-                                      input_variables=["text"])
-  
+def retrieve(url):
   type = LinkType.get_type_from_link(url)
 
   if type == LinkType.PROJECT:
     text = read_github_content(url)
     title = read_github_title(url)
   elif type == LinkType.PAPER:
     text = read_arxiv_content(url)
@@ -115,16 +104,35 @@
   elif type == LinkType.OA_PAPER:
     text = read_openaccess_content(url)
     title = read_openaccess_title(url)
   else:
     text = read_webpage_content(url)
     title = read_webpage_title(url)
 
-  text = text.strip()
-  title = title.strip()
+  return {
+    "title": title.strip(),
+    "content": text.strip()
+  }
+
+
+def summarize(url, llm):
+  text_splitter = RecursiveCharacterTextSplitter()
+  prompt_template = """Write a concise summary of the following text. 
+  I want you to provide me with bullet points highlighting the core ideas
+  of this piece. Keep each bullet point under one or two sentences.
+
+    {text}
+
+  Bullet points:"""
+  summarizer_prompt = PromptTemplate(template=prompt_template,
+                                      input_variables=["text"])
+  
+  result = retrieve(url)
+  text = result["content"]
+  title = result["title"]
 
   try:
     texts = text_splitter.split_text(text)
     docs = [Document(page_content=t) for t in texts]
     chain = load_summarize_chain(llm,
                                 chain_type="map_reduce",
                                 map_prompt=summarizer_prompt,
```

### Comparing `agent_summarizer-0.1.1/pyproject.toml` & `agent_summarizer-0.1.2/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "agent_summarizer"
-version = "0.1.1"
+version = "0.1.2"
 description = "Intelligent Summarizer of various types of media"
 authors = ["Mariya Davydova <mrs.mariya.davydova@gmail.com>"]
 license = "Apache 2.0"
 readme = "README.md"
 
 [tool.poetry.dependencies]
 python = "^3.10"
```

### Comparing `agent_summarizer-0.1.1/PKG-INFO` & `agent_summarizer-0.1.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: agent-summarizer
-Version: 0.1.1
+Version: 0.1.2
 Summary: Intelligent Summarizer of various types of media
 License: Apache 2.0
 Author: Mariya Davydova
 Author-email: mrs.mariya.davydova@gmail.com
 Requires-Python: >=3.10,<4.0
 Classifier: License :: Other/Proprietary License
 Classifier: Programming Language :: Python :: 3
```

