# Comparing `tmp/text2text-1.1.7.tar.gz` & `tmp/text2text-1.1.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "text2text-1.1.7.tar", last modified: Sun Jun 25 19:58:32 2023, max compression
+gzip compressed data, was "text2text-1.1.8.tar", last modified: Mon Jun 26 01:58:32 2023, max compression
```

## Comparing `text2text-1.1.7.tar` & `text2text-1.1.8.tar`

### file list

```diff
@@ -1,44 +1,44 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-25 19:58:32.671464 text2text-1.1.7/
--rwxr-xr-x   0 root         (0) root         (0)     1418 2023-06-25 19:54:29.000000 text2text-1.1.7/LICENSE.txt
--rw-r--r--   0 root         (0) root         (0)    56220 2023-06-25 19:58:32.670464 text2text-1.1.7/PKG-INFO
--rwxr-xr-x   0 root         (0) root         (0)    55406 2023-06-25 19:55:57.000000 text2text-1.1.7/README.md
--rw-r--r--   0 root         (0) root         (0)       38 2023-06-25 19:58:32.671464 text2text-1.1.7/setup.cfg
--rwxr-xr-x   0 root         (0) root         (0)     1246 2023-06-25 19:58:15.000000 text2text-1.1.7/setup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-25 19:58:32.667463 text2text-1.1.7/text2text/
--rwxr-xr-x   0 root         (0) root         (0)      573 2023-06-25 19:55:06.000000 text2text-1.1.7/text2text/__init__.py
--rw-r--r--   0 root         (0) root         (0)     7162 2023-06-25 19:54:29.000000 text2text-1.1.7/text2text/abstractor.py
--rw-r--r--   0 root         (0) root         (0)     2157 2023-06-25 19:54:29.000000 text2text-1.1.7/text2text/answerer.py
--rw-r--r--   0 root         (0) root         (0)     2308 2023-06-25 19:54:29.000000 text2text-1.1.7/text2text/assistant.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-25 19:58:32.669463 text2text-1.1.7/text2text/biunilm/
--rwxr-xr-x   0 root         (0) root         (0)      110 2023-06-25 19:54:29.000000 text2text-1.1.7/text2text/biunilm/__init__.py
--rwxr-xr-x   0 root         (0) root         (0)    10937 2023-06-25 19:54:29.000000 text2text-1.1.7/text2text/biunilm/loader_utils.py
--rwxr-xr-x   0 root         (0) root         (0)    17726 2023-06-25 19:54:29.000000 text2text-1.1.7/text2text/biunilm/seq2seq_loader.py
--rw-r--r--   0 root         (0) root         (0)     1533 2023-06-25 19:54:29.000000 text2text-1.1.7/text2text/bm25er.py
--rw-r--r--   0 root         (0) root         (0)      519 2023-06-25 19:54:29.000000 text2text-1.1.7/text2text/counter.py
--rw-r--r--   0 root         (0) root         (0)     1177 2023-06-25 19:54:29.000000 text2text-1.1.7/text2text/fitter.py
--rw-r--r--   0 root         (0) root         (0)     1393 2023-06-25 19:55:00.000000 text2text-1.1.7/text2text/handler.py
--rw-r--r--   0 root         (0) root         (0)     2106 2023-06-25 19:54:29.000000 text2text-1.1.7/text2text/identifier.py
--rw-r--r--   0 root         (0) root         (0)     2237 2023-06-25 19:54:29.000000 text2text-1.1.7/text2text/indexer.py
--rw-r--r--   0 root         (0) root         (0)     1165 2023-06-25 19:54:29.000000 text2text-1.1.7/text2text/measurer.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-25 19:58:32.670464 text2text-1.1.7/text2text/pytorch_pretrained_bert/
--rwxr-xr-x   0 root         (0) root         (0)      120 2023-06-25 19:54:29.000000 text2text-1.1.7/text2text/pytorch_pretrained_bert/__init__.py
--rwxr-xr-x   0 root         (0) root         (0)      932 2023-06-25 19:54:29.000000 text2text-1.1.7/text2text/pytorch_pretrained_bert/__main__.py
--rwxr-xr-x   0 root         (0) root         (0)     7964 2023-06-25 19:54:29.000000 text2text-1.1.7/text2text/pytorch_pretrained_bert/file_utils.py
--rwxr-xr-x   0 root         (0) root         (0)     1821 2023-06-25 19:54:29.000000 text2text-1.1.7/text2text/pytorch_pretrained_bert/loss.py
--rwxr-xr-x   0 root         (0) root         (0)   108506 2023-06-25 19:54:29.000000 text2text-1.1.7/text2text/pytorch_pretrained_bert/modeling.py
--rwxr-xr-x   0 root         (0) root         (0)    15035 2023-06-25 19:54:29.000000 text2text-1.1.7/text2text/pytorch_pretrained_bert/tokenization.py
--rw-r--r--   0 root         (0) root         (0)     1782 2023-06-25 19:54:29.000000 text2text-1.1.7/text2text/questioner.py
--rw-r--r--   0 root         (0) root         (0)     1519 2023-06-25 19:54:29.000000 text2text-1.1.7/text2text/server.py
--rw-r--r--   0 root         (0) root         (0)     1103 2023-06-25 19:54:29.000000 text2text-1.1.7/text2text/summarizer.py
--rw-r--r--   0 root         (0) root         (0)     1766 2023-06-25 19:54:29.000000 text2text-1.1.7/text2text/tfidfer.py
--rw-r--r--   0 root         (0) root         (0)      797 2023-06-25 19:54:29.000000 text2text-1.1.7/text2text/tokenizer.py
--rw-r--r--   0 root         (0) root         (0)    12577 2023-06-25 19:54:29.000000 text2text-1.1.7/text2text/transformer.py
--rw-r--r--   0 root         (0) root         (0)     1489 2023-06-25 19:54:29.000000 text2text-1.1.7/text2text/translator.py
--rw-r--r--   0 root         (0) root         (0)      500 2023-06-25 19:54:29.000000 text2text-1.1.7/text2text/variator.py
--rw-r--r--   0 root         (0) root         (0)      816 2023-06-25 19:54:29.000000 text2text-1.1.7/text2text/vectorizer.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-25 19:58:32.668463 text2text-1.1.7/text2text.egg-info/
--rw-r--r--   0 root         (0) root         (0)    56220 2023-06-25 19:58:32.000000 text2text-1.1.7/text2text.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     1019 2023-06-25 19:58:32.000000 text2text-1.1.7/text2text.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-06-25 19:58:32.000000 text2text-1.1.7/text2text.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      134 2023-06-25 19:58:32.000000 text2text-1.1.7/text2text.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       10 2023-06-25 19:58:32.000000 text2text-1.1.7/text2text.egg-info/top_level.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-26 01:58:32.264148 text2text-1.1.8/
+-rwxr-xr-x   0 root         (0) root         (0)     1418 2023-06-25 23:15:10.000000 text2text-1.1.8/LICENSE.txt
+-rw-r--r--   0 root         (0) root         (0)    56262 2023-06-26 01:58:32.264148 text2text-1.1.8/PKG-INFO
+-rwxr-xr-x   0 root         (0) root         (0)    55448 2023-06-26 01:57:47.000000 text2text-1.1.8/README.md
+-rw-r--r--   0 root         (0) root         (0)       38 2023-06-26 01:58:32.264148 text2text-1.1.8/setup.cfg
+-rwxr-xr-x   0 root         (0) root         (0)     1246 2023-06-26 01:08:21.000000 text2text-1.1.8/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-26 01:58:32.260147 text2text-1.1.8/text2text/
+-rwxr-xr-x   0 root         (0) root         (0)      603 2023-06-26 00:47:46.000000 text2text-1.1.8/text2text/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     7162 2023-06-25 23:15:10.000000 text2text-1.1.8/text2text/abstractor.py
+-rw-r--r--   0 root         (0) root         (0)     2246 2023-06-26 01:05:37.000000 text2text-1.1.8/text2text/answerer.py
+-rw-r--r--   0 root         (0) root         (0)     2308 2023-06-25 23:15:10.000000 text2text-1.1.8/text2text/assistant.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-26 01:58:32.262148 text2text-1.1.8/text2text/biunilm/
+-rwxr-xr-x   0 root         (0) root         (0)      110 2023-06-25 23:15:10.000000 text2text-1.1.8/text2text/biunilm/__init__.py
+-rwxr-xr-x   0 root         (0) root         (0)    10937 2023-06-25 23:15:10.000000 text2text-1.1.8/text2text/biunilm/loader_utils.py
+-rwxr-xr-x   0 root         (0) root         (0)    17726 2023-06-25 23:15:10.000000 text2text-1.1.8/text2text/biunilm/seq2seq_loader.py
+-rw-r--r--   0 root         (0) root         (0)     1533 2023-06-25 23:15:10.000000 text2text-1.1.8/text2text/bm25er.py
+-rw-r--r--   0 root         (0) root         (0)      519 2023-06-25 23:15:10.000000 text2text-1.1.8/text2text/counter.py
+-rw-r--r--   0 root         (0) root         (0)     1177 2023-06-25 23:15:10.000000 text2text-1.1.8/text2text/fitter.py
+-rw-r--r--   0 root         (0) root         (0)     1393 2023-06-25 23:15:10.000000 text2text-1.1.8/text2text/handler.py
+-rw-r--r--   0 root         (0) root         (0)     2106 2023-06-25 23:15:10.000000 text2text-1.1.8/text2text/identifier.py
+-rw-r--r--   0 root         (0) root         (0)     2534 2023-06-26 01:51:41.000000 text2text-1.1.8/text2text/indexer.py
+-rw-r--r--   0 root         (0) root         (0)     1165 2023-06-25 23:15:10.000000 text2text-1.1.8/text2text/measurer.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-26 01:58:32.263148 text2text-1.1.8/text2text/pytorch_pretrained_bert/
+-rwxr-xr-x   0 root         (0) root         (0)      120 2023-06-25 23:15:10.000000 text2text-1.1.8/text2text/pytorch_pretrained_bert/__init__.py
+-rwxr-xr-x   0 root         (0) root         (0)      932 2023-06-25 23:15:10.000000 text2text-1.1.8/text2text/pytorch_pretrained_bert/__main__.py
+-rwxr-xr-x   0 root         (0) root         (0)     7964 2023-06-25 23:15:10.000000 text2text-1.1.8/text2text/pytorch_pretrained_bert/file_utils.py
+-rwxr-xr-x   0 root         (0) root         (0)     1821 2023-06-25 23:15:10.000000 text2text-1.1.8/text2text/pytorch_pretrained_bert/loss.py
+-rwxr-xr-x   0 root         (0) root         (0)   108506 2023-06-25 23:15:10.000000 text2text-1.1.8/text2text/pytorch_pretrained_bert/modeling.py
+-rwxr-xr-x   0 root         (0) root         (0)    15035 2023-06-25 23:15:10.000000 text2text-1.1.8/text2text/pytorch_pretrained_bert/tokenization.py
+-rw-r--r--   0 root         (0) root         (0)     1782 2023-06-25 23:15:10.000000 text2text-1.1.8/text2text/questioner.py
+-rw-r--r--   0 root         (0) root         (0)     1530 2023-06-26 01:55:49.000000 text2text-1.1.8/text2text/server.py
+-rw-r--r--   0 root         (0) root         (0)     1103 2023-06-25 23:15:10.000000 text2text-1.1.8/text2text/summarizer.py
+-rw-r--r--   0 root         (0) root         (0)     1766 2023-06-25 23:15:10.000000 text2text-1.1.8/text2text/tfidfer.py
+-rw-r--r--   0 root         (0) root         (0)      797 2023-06-25 23:23:25.000000 text2text-1.1.8/text2text/tokenizer.py
+-rw-r--r--   0 root         (0) root         (0)    12577 2023-06-25 23:15:10.000000 text2text-1.1.8/text2text/transformer.py
+-rw-r--r--   0 root         (0) root         (0)     1506 2023-06-26 01:41:07.000000 text2text-1.1.8/text2text/translator.py
+-rw-r--r--   0 root         (0) root         (0)      500 2023-06-25 23:15:10.000000 text2text-1.1.8/text2text/variator.py
+-rw-r--r--   0 root         (0) root         (0)      833 2023-06-25 23:23:55.000000 text2text-1.1.8/text2text/vectorizer.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-26 01:58:32.261148 text2text-1.1.8/text2text.egg-info/
+-rw-r--r--   0 root         (0) root         (0)    56262 2023-06-26 01:58:32.000000 text2text-1.1.8/text2text.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     1019 2023-06-26 01:58:32.000000 text2text-1.1.8/text2text.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-06-26 01:58:32.000000 text2text-1.1.8/text2text.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      134 2023-06-26 01:58:32.000000 text2text-1.1.8/text2text.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       10 2023-06-26 01:58:32.000000 text2text-1.1.8/text2text.egg-info/top_level.txt
```

### Comparing `text2text-1.1.7/LICENSE.txt` & `text2text-1.1.8/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `text2text-1.1.7/PKG-INFO` & `text2text-1.1.8/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: text2text
-Version: 1.1.7
+Version: 1.1.8
 Summary: Text2Text: Crosslingual NLP/G toolkit
 Home-page: https://github.com/artitw/text2text
 Author: Artit Wangperawong
 Author-email: artitw@gmail.com
 Keywords: multilingual crosslingual gpt chatgpt bert natural language processing nlp nlg text generation gpt question answer answering information retrieval tfidf tf-idf bm25 search index summary summarizer summarization tokenizer tokenization translation backtranslation data augmentation science machine learning colab embedding levenshtein sub-word edit distance conversational dialog chatbot
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
@@ -309,19 +309,19 @@
   "Let's go hiking tomorrow, let's go!",
   "안녕하세요.",
   "돼지꿈을 꾸세요~~",
 ])
 
 index.retrieve(["돼지"], k=1) #[['"돼지꿈을 꾸세요~~"']]
 
-# Add documents incrementing on ids if none specified
+# Add documents
 index.add(["Hello, World! 你好,世界!"])
 
 # Remove by ids
-index.remove([2]) #Removes "안녕하세요."
+index.remove([2]) #Removes "돼지꿈을 꾸세요~~"
 
 # Retrieve k results per query sorted by distance
 index.retrieve(["你好, World"], k=3)
 ```
 To learn more, see [STF-IDF](https://arxiv.org/abs/2209.14281).
 
 ### Levenshtein Sub-word Edit Distance
@@ -651,29 +651,30 @@
 
 # Make POST requests
 import socket
 import requests
 
 address = socket.gethostbyname(socket.getfqdn(socket.gethostname()))
 url = f"http://{address}"
-transform = "translate"
+transformer = "Translator"
 payload = {
   "input_lines": ["hello", "world"],
   "src_lang": "en",
   "tgt_lang": "ko",
 }
-r = requests.post(f"{url}/{transform}", json=payload)
+r = requests.post(f"{url}/{transformer}", json=payload)
 print(r.json()) #{'result': ['안녕하세요', '세계']}
 
 # Indexer actions
-r = requests.post(f"{url}/index/add", json=payload)
-r = requests.post(f"{url}/index/size")
-r = requests.post(f"{url}/index/search", json=payload)
+r = requests.post(f"{url}/Indexer/add", json=payload)
+r = requests.post(f"{url}/Indexer/size")
+r = requests.post(f"{url}/Indexer/search", json=payload)
+r = requests.post(f"{url}/Indexer/retrieve", json=payload)
 payload["ids"] = [0,1]
-r = requests.post(f"{url}/index/remove", json=payload)
+r = requests.post(f"{url}/Indexer/remove", json=payload)
 ```
 
 ## Questions?
 For questions or help using Text2Text, please submit a [GitHub issue](https://github.com/artitw/text2text/issues).
 
 ## Citation
 To cite this work, use the following BibTeX citations.
```

### Comparing `text2text-1.1.7/README.md` & `text2text-1.1.8/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -295,19 +295,19 @@
   "Let's go hiking tomorrow, let's go!",
   "안녕하세요.",
   "돼지꿈을 꾸세요~~",
 ])
 
 index.retrieve(["돼지"], k=1) #[['"돼지꿈을 꾸세요~~"']]
 
-# Add documents incrementing on ids if none specified
+# Add documents
 index.add(["Hello, World! 你好,世界!"])
 
 # Remove by ids
-index.remove([2]) #Removes "안녕하세요."
+index.remove([2]) #Removes "돼지꿈을 꾸세요~~"
 
 # Retrieve k results per query sorted by distance
 index.retrieve(["你好, World"], k=3)
 ```
 To learn more, see [STF-IDF](https://arxiv.org/abs/2209.14281).
 
 ### Levenshtein Sub-word Edit Distance
@@ -637,29 +637,30 @@
 
 # Make POST requests
 import socket
 import requests
 
 address = socket.gethostbyname(socket.getfqdn(socket.gethostname()))
 url = f"http://{address}"
-transform = "translate"
+transformer = "Translator"
 payload = {
   "input_lines": ["hello", "world"],
   "src_lang": "en",
   "tgt_lang": "ko",
 }
-r = requests.post(f"{url}/{transform}", json=payload)
+r = requests.post(f"{url}/{transformer}", json=payload)
 print(r.json()) #{'result': ['안녕하세요', '세계']}
 
 # Indexer actions
-r = requests.post(f"{url}/index/add", json=payload)
-r = requests.post(f"{url}/index/size")
-r = requests.post(f"{url}/index/search", json=payload)
+r = requests.post(f"{url}/Indexer/add", json=payload)
+r = requests.post(f"{url}/Indexer/size")
+r = requests.post(f"{url}/Indexer/search", json=payload)
+r = requests.post(f"{url}/Indexer/retrieve", json=payload)
 payload["ids"] = [0,1]
-r = requests.post(f"{url}/index/remove", json=payload)
+r = requests.post(f"{url}/Indexer/remove", json=payload)
 ```
 
 ## Questions?
 For questions or help using Text2Text, please submit a [GitHub issue](https://github.com/artitw/text2text/issues).
 
 ## Citation
 To cite this work, use the following BibTeX citations.
```

### Comparing `text2text-1.1.7/setup.py` & `text2text-1.1.8/setup.py`

 * *Files identical despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 with open("README.md", "r") as fh:
   long_description = fh.read()
 
 setuptools.setup(
   name="text2text",
-  version="1.1.7",
+  version="1.1.8",
   author="Artit Wangperawong",
   author_email="artitw@gmail.com",
   description="Text2Text: Crosslingual NLP/G toolkit",
   long_description=long_description,
   long_description_content_type="text/markdown",
   url="https://github.com/artitw/text2text",
   packages=setuptools.find_packages(),
```

### Comparing `text2text-1.1.7/text2text/__init__.py` & `text2text-1.1.8/text2text/__init__.py`

 * *Files 15% similar despite different names*

```diff
@@ -11,8 +11,9 @@
 from .indexer import Indexer
 from .variator import Variator
 from .abstractor import Abstractor
 from .questioner import Questioner
 from .summarizer import Summarizer
 from .answerer import Answerer
 from .identifier import Identifier
-from .server import Server
+from .server import Server
+from .handler import Handler
```

### Comparing `text2text-1.1.7/text2text/abstractor.py` & `text2text-1.1.8/text2text/abstractor.py`

 * *Files identical despite different names*

### Comparing `text2text-1.1.7/text2text/answerer.py` & `text2text-1.1.8/text2text/answerer.py`

 * *Files 3% similar despite different names*

```diff
@@ -7,26 +7,26 @@
   pretrained_answerer = "valhalla/longformer-base-4096-finetuned-squadv1"
 
   def __init__(self, **kwargs):
     pretrained_answerer = kwargs.get('pretrained_answerer')
     if not pretrained_answerer:
       pretrained_answerer = self.__class__.pretrained_answerer
     self.__class__.tokenizer = AutoTokenizer.from_pretrained(pretrained_answerer)
-    self.__class__.model = AutoModelForQuestionAnswering.from_pretrained(pretrained_answerer)
+    self.__class__.model = AutoModelForQuestionAnswering.from_pretrained(pretrained_answerer, device_map="auto", load_in_8bit=True)
 
   def _translate_lines(self, input_lines, src_lang, tgt_lang):
     translator = getattr(self.__class__, "translator", t2t.Translator())
     self.__class__.translator = translator
     return translator.transform(input_lines, src_lang=src_lang, tgt_lang=tgt_lang)
 
   def _get_answers(self, input_lines):
     tokenizer = self.__class__.tokenizer
     model = self.__class__.model
     num_examples = len(input_lines)
-    encoded_inputs = tokenizer.batch_encode_plus(input_lines, padding=True, return_tensors="pt")
+    encoded_inputs = tokenizer.batch_encode_plus(input_lines, padding=True, return_tensors="pt").to("cuda" if torch.cuda.is_available() else "cpu")
     input_ids = encoded_inputs["input_ids"]
     attention_mask = encoded_inputs["attention_mask"]
     results = model(input_ids, attention_mask=attention_mask)
     ans_ids = [None] * num_examples
     for i in range(num_examples):
       max_startscore = torch.argmax(results["start_logits"][i])
       max_endscore = torch.argmax(results["end_logits"][i])
```

### Comparing `text2text-1.1.7/text2text/assistant.py` & `text2text-1.1.8/text2text/assistant.py`

 * *Files identical despite different names*

### Comparing `text2text-1.1.7/text2text/biunilm/loader_utils.py` & `text2text-1.1.8/text2text/biunilm/loader_utils.py`

 * *Files identical despite different names*

### Comparing `text2text-1.1.7/text2text/biunilm/seq2seq_loader.py` & `text2text-1.1.8/text2text/biunilm/seq2seq_loader.py`

 * *Files identical despite different names*

### Comparing `text2text-1.1.7/text2text/bm25er.py` & `text2text-1.1.8/text2text/bm25er.py`

 * *Files identical despite different names*

### Comparing `text2text-1.1.7/text2text/counter.py` & `text2text-1.1.8/text2text/counter.py`

 * *Files identical despite different names*

### Comparing `text2text-1.1.7/text2text/fitter.py` & `text2text-1.1.8/text2text/fitter.py`

 * *Files identical despite different names*

### Comparing `text2text-1.1.7/text2text/handler.py` & `text2text-1.1.8/text2text/handler.py`

 * *Files identical despite different names*

### Comparing `text2text-1.1.7/text2text/identifier.py` & `text2text-1.1.8/text2text/identifier.py`

 * *Files identical despite different names*

### Comparing `text2text-1.1.7/text2text/indexer.py` & `text2text-1.1.8/text2text/indexer.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 import text2text as t2t
 import faiss
 import numpy as np
+import pandas as pd
 import scipy.sparse as sp
 import warnings
 
 class Indexer(t2t.Transformer):
 
   def get_formatted_matrix(self, input_lines, src_lang='en', **kwargs):
     res = np.array([[]]*len(input_lines))
@@ -17,42 +18,46 @@
 
   def size(self, **kwargs):
     return self.index.ntotal
 
   def add(self, input_lines, src_lang='en', faiss_index=None, **kwargs):
     if faiss_index is not None:
       self.index = faiss_index
-    starting_id = np.amax(faiss.vector_to_array(self.index.id_map), initial=0)
+    starting_id = 0
+    if self.index.ntotal:
+      starting_id = 1+np.amax(faiss.vector_to_array(self.index.id_map), initial=0)
     ids = list(range(starting_id, starting_id+len(input_lines)))
-    v = self.get_formatted_matrix(input_lines, src_lang=src_lang, **kwargs)
-    self.index.add_with_ids(v, np.array(ids))
-    self.corpus += list(input_lines)
+    vectors = self.get_formatted_matrix(input_lines, src_lang=src_lang, **kwargs)
+    self.index.add_with_ids(vectors, np.array(ids))
+    new_docs = pd.DataFrame({'document': input_lines})
+    new_docs.index = ids
+    self.corpus = pd.concat([self.corpus, new_docs])
     return self
 
   def remove(self, ids, faiss_index=None, **kwargs):
     if faiss_index is not None:
       self.index = faiss_index
     self.index.remove_ids(np.array(ids))
-    for i in ids:
-      del self.corpus[i]
+    self.corpus = self.corpus[~self.corpus.index.isin(ids)]
 
   def search(self, input_lines, src_lang='en', k=3, faiss_index=None, **kwargs):
     if faiss_index is not None:
       self.index = faiss_index
     if not self.index or not self.index.ntotal:
       warnings.warn('Empty results because no index found. Make sure to build your index before searching.')
       return []
     xq = self.get_formatted_matrix(input_lines, src_lang=src_lang, **kwargs)
     return self.index.search(xq, k)
 
-  def retrieve(self, input_lines, k=3):
+  def retrieve(self, input_lines, k=3, **kwargs):
     distances, pred_ids = self.search(input_lines, k=k)
-    return [[self.corpus[i] for i in line_ids] for line_ids in pred_ids]
+    return [self.corpus["document"].loc[[i for i in line_ids if i >= 0]].tolist() for line_ids in pred_ids]
 
   def transform(self, input_lines, src_lang='en', encoders=[t2t.Tfidfer], **kwargs):
     self.encoders = encoders
+    self.src_lang = src_lang
     d = self.get_formatted_matrix(["DUMMY"], src_lang=src_lang, **kwargs).shape[-1]
     self.index = faiss.IndexIDMap2(faiss.IndexFlatL2(d))
-    self.corpus = []
+    self.corpus = pd.DataFrame({"document": []})
     if not input_lines:
       return self
     return self.add(input_lines, src_lang=src_lang, **kwargs)
```

### Comparing `text2text-1.1.7/text2text/measurer.py` & `text2text-1.1.8/text2text/measurer.py`

 * *Files identical despite different names*

### Comparing `text2text-1.1.7/text2text/pytorch_pretrained_bert/__main__.py` & `text2text-1.1.8/text2text/pytorch_pretrained_bert/__main__.py`

 * *Files identical despite different names*

### Comparing `text2text-1.1.7/text2text/pytorch_pretrained_bert/file_utils.py` & `text2text-1.1.8/text2text/pytorch_pretrained_bert/file_utils.py`

 * *Files identical despite different names*

### Comparing `text2text-1.1.7/text2text/pytorch_pretrained_bert/loss.py` & `text2text-1.1.8/text2text/pytorch_pretrained_bert/loss.py`

 * *Files identical despite different names*

### Comparing `text2text-1.1.7/text2text/pytorch_pretrained_bert/modeling.py` & `text2text-1.1.8/text2text/pytorch_pretrained_bert/modeling.py`

 * *Files identical despite different names*

### Comparing `text2text-1.1.7/text2text/pytorch_pretrained_bert/tokenization.py` & `text2text-1.1.8/text2text/pytorch_pretrained_bert/tokenization.py`

 * *Files identical despite different names*

### Comparing `text2text-1.1.7/text2text/questioner.py` & `text2text-1.1.8/text2text/questioner.py`

 * *Files identical despite different names*

### Comparing `text2text-1.1.7/text2text/server.py` & `text2text-1.1.8/text2text/server.py`

 * *Files 23% similar despite different names*

```diff
@@ -6,42 +6,40 @@
 
 app = Flask(__name__)
 
 @app.route("/", methods=['GET', 'POST'])
 def hello():
   return {"result": "Hello, this Text2Text at your service."}
 
-@app.route('/indexer/<action>', methods=['POST'])
+@app.route('/Indexer/<action>', methods=['POST'])
 def indexer(action):
   try:
-    data = request.get_json() or {}
-    input_lines = data.get("input_lines", [])
-    src_lang = data.get("src_lang", "en")
-    if hasattr(t2t.Server, "index"):
-      index = t2t.Server.index
-    else:
-      t2t.Server.index = t2t.Indexer().add(input_lines)
+    if not hasattr(t2t.Server, "index"):
+      t2t.Server.index = t2t.Indexer().transform([])
+    index = t2t.Server.index
     assert hasattr(index, action)
+    data = request.get_json() or {}
     res = getattr(index, action)(**data)
     if action in ["search", "size"]:
       return {"result": np.array(res).tolist()}
+    elif action in ["retrieve"]:
+      return {"result": res}
   except Exception as e:
     return {"result": str(e)}
-  return {"result": f"indexer/{action} performed"}
+  return {"result": f"Indexer/{action} performed"}
 
 @app.route('/<transformer>', methods=['POST'])
 def transform(transformer):
   try:
     assert hasattr(t2t, transformer)
+    transformer_instance = transformer.lower()
+    if not hasattr(t2t.Server, transformer_instance):
+      setattr(t2t.Server, transformer_instance, getattr(t2t, transformer)())
     data = request.get_json() or {}
-    input_lines = data.get("input_lines", [])
-    src_lang = data.get("src_lang", "en")
-    res = getattr(t2t, transformer)(input_lines, src_lang)
-    del data["input_lines"]
-    del data["src_lang"]
+    res = getattr(t2t.Server, transformer_instance).transform(**data)
     return {"result": res}
   except Exception as e:
     return {"result": str(e)}
 
 class Server(object):
   def __init__(self, **kwargs):
     address = socket.gethostbyname(socket.getfqdn(socket.gethostname()))
```

### Comparing `text2text-1.1.7/text2text/summarizer.py` & `text2text-1.1.8/text2text/summarizer.py`

 * *Files identical despite different names*

### Comparing `text2text-1.1.7/text2text/tfidfer.py` & `text2text-1.1.8/text2text/tfidfer.py`

 * *Files identical despite different names*

### Comparing `text2text-1.1.7/text2text/tokenizer.py` & `text2text-1.1.8/text2text/tokenizer.py`

 * *Files identical despite different names*

### Comparing `text2text-1.1.7/text2text/transformer.py` & `text2text-1.1.8/text2text/transformer.py`

 * *Files identical despite different names*

### Comparing `text2text-1.1.7/text2text/translator.py` & `text2text-1.1.8/text2text/translator.py`

 * *Files 8% similar despite different names*

```diff
@@ -16,15 +16,15 @@
     if 'tgt_lang' not in kwargs:
       raise ValueError('tgt_lang not specified')
     tgt_lang = kwargs.get('tgt_lang')
     if src_lang==tgt_lang:
       return input_lines
     if tgt_lang not in self.__class__.LANGUAGES:
       raise ValueError(f'{tgt_lang} not found in {self.__class__.LANGUAGES}')
-    encoded_inputs = tokenizer(input_lines, padding=True, return_tensors="pt").to("cuda" if torch.cuda.is_available() else "cpu")
+    encoded_inputs = tokenizer(input_lines, padding=True, truncation=True, return_tensors="pt").to("cuda" if torch.cuda.is_available() else "cpu")
     tgt_token_id = tokenizer.lang_code_to_id[tgt_lang]
     generated_tokens = model.generate(**encoded_inputs, forced_bos_token_id=tgt_token_id)
     return tokenizer.batch_decode(generated_tokens, skip_special_tokens=True) 
 
   def transform(self, input_lines, src_lang='en', **kwargs):
     input_lines = t2t.Transformer.transform(self, input_lines, src_lang=src_lang, **kwargs)
     return self._translate(input_lines, src_lang=src_lang, **kwargs)
```

### Comparing `text2text-1.1.7/text2text/vectorizer.py` & `text2text-1.1.8/text2text/vectorizer.py`

 * *Files 2% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 class Vectorizer(t2t.Translator):
 
   def transform(self, input_lines, src_lang='en', output_dimension=1, **kwargs):
     input_lines = t2t.Transformer.transform(self, input_lines, src_lang=src_lang, **kwargs)
     tokenizer = self.__class__.tokenizer
     model = self.__class__.model
     tokenizer.src_lang = src_lang
-    encoder_inputs = tokenizer(input_lines, padding=True, return_tensors="pt")
+    encoder_inputs = tokenizer(input_lines, padding=True, truncation=True, return_tensors="pt")
     outputs = model.forward(**encoder_inputs, decoder_input_ids=torch.zeros(len(input_lines),1,dtype=int))
     last_layer_states = outputs.encoder_last_hidden_state.cpu().detach().numpy()
     if output_dimension==1:
       x = np.mean(last_layer_states, axis=1)
       x /= np.linalg.norm(x, axis=1).reshape(x.shape[0],-1)
       return x
     return last_layer_states
```

### Comparing `text2text-1.1.7/text2text.egg-info/PKG-INFO` & `text2text-1.1.8/text2text.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: text2text
-Version: 1.1.7
+Version: 1.1.8
 Summary: Text2Text: Crosslingual NLP/G toolkit
 Home-page: https://github.com/artitw/text2text
 Author: Artit Wangperawong
 Author-email: artitw@gmail.com
 Keywords: multilingual crosslingual gpt chatgpt bert natural language processing nlp nlg text generation gpt question answer answering information retrieval tfidf tf-idf bm25 search index summary summarizer summarization tokenizer tokenization translation backtranslation data augmentation science machine learning colab embedding levenshtein sub-word edit distance conversational dialog chatbot
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
@@ -309,19 +309,19 @@
   "Let's go hiking tomorrow, let's go!",
   "안녕하세요.",
   "돼지꿈을 꾸세요~~",
 ])
 
 index.retrieve(["돼지"], k=1) #[['"돼지꿈을 꾸세요~~"']]
 
-# Add documents incrementing on ids if none specified
+# Add documents
 index.add(["Hello, World! 你好,世界!"])
 
 # Remove by ids
-index.remove([2]) #Removes "안녕하세요."
+index.remove([2]) #Removes "돼지꿈을 꾸세요~~"
 
 # Retrieve k results per query sorted by distance
 index.retrieve(["你好, World"], k=3)
 ```
 To learn more, see [STF-IDF](https://arxiv.org/abs/2209.14281).
 
 ### Levenshtein Sub-word Edit Distance
@@ -651,29 +651,30 @@
 
 # Make POST requests
 import socket
 import requests
 
 address = socket.gethostbyname(socket.getfqdn(socket.gethostname()))
 url = f"http://{address}"
-transform = "translate"
+transformer = "Translator"
 payload = {
   "input_lines": ["hello", "world"],
   "src_lang": "en",
   "tgt_lang": "ko",
 }
-r = requests.post(f"{url}/{transform}", json=payload)
+r = requests.post(f"{url}/{transformer}", json=payload)
 print(r.json()) #{'result': ['안녕하세요', '세계']}
 
 # Indexer actions
-r = requests.post(f"{url}/index/add", json=payload)
-r = requests.post(f"{url}/index/size")
-r = requests.post(f"{url}/index/search", json=payload)
+r = requests.post(f"{url}/Indexer/add", json=payload)
+r = requests.post(f"{url}/Indexer/size")
+r = requests.post(f"{url}/Indexer/search", json=payload)
+r = requests.post(f"{url}/Indexer/retrieve", json=payload)
 payload["ids"] = [0,1]
-r = requests.post(f"{url}/index/remove", json=payload)
+r = requests.post(f"{url}/Indexer/remove", json=payload)
 ```
 
 ## Questions?
 For questions or help using Text2Text, please submit a [GitHub issue](https://github.com/artitw/text2text/issues).
 
 ## Citation
 To cite this work, use the following BibTeX citations.
```

### Comparing `text2text-1.1.7/text2text.egg-info/SOURCES.txt` & `text2text-1.1.8/text2text.egg-info/SOURCES.txt`

 * *Files identical despite different names*

