# Comparing `tmp/aimped-0.1.52.tar.gz` & `tmp/aimped-0.1.53.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/aimped-0.1.52.tar", last modified: Sat Jun 24 17:32:53 2023, max compression
+gzip compressed data, was "aimped-0.1.53.tar", last modified: Mon Jun 26 18:51:58 2023, max compression
```

## Comparing `aimped-0.1.52.tar` & `aimped-0.1.53.tar`

### file list

```diff
@@ -1,47 +1,47 @@
-drwxr-xr-x   0 DataScience   (501) staff       (20)        0 2023-06-24 17:32:53.000000 aimped-0.1.52/
--rw-r--r--   0 DataScience   (501) staff       (20)     1751 2023-06-24 17:32:53.000000 aimped-0.1.52/PKG-INFO
-drwxr-xr-x   0 DataScience   (501) staff       (20)        0 2023-06-24 17:32:53.000000 aimped-0.1.52/aimped/
--rw-r--r--   0 DataScience   (501) staff       (20)    12438 2023-06-24 16:48:55.000000 aimped-0.1.52/aimped/io_tasks.py
--rw-r--r--   0 DataScience   (501) staff       (20)      123 2023-06-24 17:32:21.000000 aimped-0.1.52/aimped/version.py
--rw-r--r--   0 DataScience   (501) staff       (20)      502 2023-06-24 16:48:55.000000 aimped-0.1.52/aimped/models.py
-drwxr-xr-x   0 DataScience   (501) staff       (20)        0 2023-06-24 17:32:53.000000 aimped-0.1.52/aimped/test/
--rw-r--r--   0 DataScience   (501) staff       (20)     1313 2023-06-24 16:48:55.000000 aimped-0.1.52/aimped/test/test_chunk_merger.py
--rw-r--r--   0 DataScience   (501) staff       (20)     3320 2023-06-24 16:48:55.000000 aimped-0.1.52/aimped/test/test_relation_pipeline.py
--rw-r--r--   0 DataScience   (501) staff       (20)      610 2023-06-24 16:48:55.000000 aimped-0.1.52/aimped/test/test_tokenizer.py
--rw-r--r--   0 DataScience   (501) staff       (20)        0 2023-06-24 16:48:55.000000 aimped-0.1.52/aimped/test/__init__.py
--rw-r--r--   0 DataScience   (501) staff       (20)     1592 2023-06-24 16:48:55.000000 aimped-0.1.52/aimped/test/test_regex_parser.py
--rw-r--r--   0 DataScience   (501) staff       (20)     5585 2023-06-24 16:48:55.000000 aimped-0.1.52/aimped/test/test_translation_pipeline.py
--rw-r--r--   0 DataScience   (501) staff       (20)     1297 2023-06-24 16:48:55.000000 aimped-0.1.52/aimped/test/test_ner_results.py
--rw-r--r--   0 DataScience   (501) staff       (20)     2748 2023-06-24 16:48:55.000000 aimped-0.1.52/aimped/test/test_assertion.py
--rw-r--r--   0 DataScience   (501) staff       (20)     1866 2023-06-24 16:48:55.000000 aimped-0.1.52/aimped/test/test_deid_pipeline.py
--rw-r--r--   0 DataScience   (501) staff       (20)      193 2023-06-24 16:48:55.000000 aimped-0.1.52/aimped/__init__.py
--rw-r--r--   0 DataScience   (501) staff       (20)     2060 2023-06-24 16:48:55.000000 aimped-0.1.52/aimped/utils.py
-drwxr-xr-x   0 DataScience   (501) staff       (20)        0 2023-06-24 17:32:53.000000 aimped-0.1.52/aimped/model/
--rw-r--r--   0 DataScience   (501) staff       (20)        0 2023-06-24 16:48:55.000000 aimped-0.1.52/aimped/model/__init__.py
--rw-r--r--   0 DataScience   (501) staff       (20)     2338 2023-06-24 16:48:55.000000 aimped-0.1.52/aimped/model/load.py
-drwxr-xr-x   0 DataScience   (501) staff       (20)        0 2023-06-24 17:32:53.000000 aimped-0.1.52/aimped/nlp/
--rw-r--r--   0 DataScience   (501) staff       (20)    19853 2023-06-24 16:48:55.000000 aimped-0.1.52/aimped/nlp/relation_visualizer.py
--rw-r--r--   0 DataScience   (501) staff       (20)     4290 2023-06-24 17:02:00.000000 aimped-0.1.52/aimped/nlp/relation.py
--rw-r--r--   0 DataScience   (501) staff       (20)     3917 2023-06-24 16:48:55.000000 aimped-0.1.52/aimped/nlp/chunker.py
--rw-r--r--   0 DataScience   (501) staff       (20)     2251 2023-06-24 16:48:55.000000 aimped-0.1.52/aimped/nlp/tools.py
--rw-r--r--   0 DataScience   (501) staff       (20)      353 2023-06-24 16:48:55.000000 aimped-0.1.52/aimped/nlp/__init__.py
--rw-r--r--   0 DataScience   (501) staff       (20)     2228 2023-06-24 16:48:55.000000 aimped-0.1.52/aimped/nlp/assertion.py
--rw-r--r--   0 DataScience   (501) staff       (20)      803 2023-06-24 16:48:55.000000 aimped-0.1.52/aimped/nlp/tokenizer.py
--rw-r--r--   0 DataScience   (501) staff       (20)     2629 2023-06-24 16:48:55.000000 aimped-0.1.52/aimped/nlp/ner_cls_report.py
--rw-r--r--   0 DataScience   (501) staff       (20)     4521 2023-06-24 16:48:55.000000 aimped-0.1.52/aimped/nlp/ner.py
--rw-r--r--   0 DataScience   (501) staff       (20)     2825 2023-06-24 16:48:55.000000 aimped-0.1.52/aimped/nlp/deid.py
--rw-r--r--   0 DataScience   (501) staff       (20)     6873 2023-06-24 17:31:12.000000 aimped-0.1.52/aimped/nlp/pipeline.py
--rwxr-xr-x   0 DataScience   (501) staff       (20)     2524 2023-06-24 16:48:55.000000 aimped-0.1.52/aimped/nlp/translation.py
--rw-r--r--   0 DataScience   (501) staff       (20)     3899 2023-06-24 16:48:55.000000 aimped-0.1.52/aimped/nlp/regex_parser.py
-drwxr-xr-x   0 DataScience   (501) staff       (20)        0 2023-06-24 17:32:53.000000 aimped-0.1.52/aimped/nitro/
--rw-r--r--   0 DataScience   (501) staff       (20)        0 2023-06-24 16:48:55.000000 aimped-0.1.52/aimped/nitro/__init__.py
--rw-r--r--   0 DataScience   (501) staff       (20)     1063 2023-06-24 16:48:55.000000 aimped-0.1.52/LICENSE
--rw-r--r--   0 DataScience   (501) staff       (20)     1157 2023-06-24 16:48:55.000000 aimped-0.1.52/README.md
--rw-r--r--   0 DataScience   (501) staff       (20)     1163 2023-06-24 16:48:55.000000 aimped-0.1.52/setup.py
-drwxr-xr-x   0 DataScience   (501) staff       (20)        0 2023-06-24 17:32:53.000000 aimped-0.1.52/aimped.egg-info/
--rw-r--r--   0 DataScience   (501) staff       (20)     1751 2023-06-24 17:32:53.000000 aimped-0.1.52/aimped.egg-info/PKG-INFO
--rw-r--r--   0 DataScience   (501) staff       (20)      952 2023-06-24 17:32:53.000000 aimped-0.1.52/aimped.egg-info/SOURCES.txt
--rw-r--r--   0 DataScience   (501) staff       (20)       48 2023-06-24 17:32:53.000000 aimped-0.1.52/aimped.egg-info/requires.txt
--rw-r--r--   0 DataScience   (501) staff       (20)        7 2023-06-24 17:32:53.000000 aimped-0.1.52/aimped.egg-info/top_level.txt
--rw-r--r--   0 DataScience   (501) staff       (20)        1 2023-06-24 17:32:53.000000 aimped-0.1.52/aimped.egg-info/dependency_links.txt
--rw-r--r--   0 DataScience   (501) staff       (20)      103 2023-06-24 17:32:53.000000 aimped-0.1.52/setup.cfg
+drwxrwxrwx   0        0        0        0 2023-06-26 18:51:58.706464 aimped-0.1.53/
+-rw-rw-rw-   0        0        0     1063 2023-04-03 13:18:42.000000 aimped-0.1.53/LICENSE
+-rw-rw-rw-   0        0        0     1778 2023-06-26 18:51:58.707456 aimped-0.1.53/PKG-INFO
+-rw-rw-rw-   0        0        0     1205 2023-05-24 09:20:26.000000 aimped-0.1.53/README.md
+drwxrwxrwx   0        0        0        0 2023-06-26 18:51:58.657518 aimped-0.1.53/aimped/
+-rw-rw-rw-   0        0        0       39 2023-06-26 18:49:01.000000 aimped-0.1.53/aimped/__init__.py
+-rw-rw-rw-   0        0        0    13550 2023-06-26 18:40:19.000000 aimped-0.1.53/aimped/io_tasks.py
+drwxrwxrwx   0        0        0        0 2023-06-26 18:51:58.669518 aimped-0.1.53/aimped/model/
+-rw-rw-rw-   0        0        0        0 2023-04-03 13:18:42.000000 aimped-0.1.53/aimped/model/__init__.py
+-rw-rw-rw-   0        0        0     2338 2023-04-03 13:18:42.000000 aimped-0.1.53/aimped/model/load.py
+-rw-rw-rw-   0        0        0      655 2023-06-06 20:37:28.000000 aimped-0.1.53/aimped/models.py
+drwxrwxrwx   0        0        0        0 2023-06-26 18:51:58.671521 aimped-0.1.53/aimped/nitro/
+-rw-rw-rw-   0        0        0        0 2023-04-03 13:18:42.000000 aimped-0.1.53/aimped/nitro/__init__.py
+drwxrwxrwx   0        0        0        0 2023-06-26 18:51:58.692451 aimped-0.1.53/aimped/nlp/
+-rw-rw-rw-   0        0        0      353 2023-04-03 13:18:42.000000 aimped-0.1.53/aimped/nlp/__init__.py
+-rw-rw-rw-   0        0        0     2228 2023-04-03 13:18:42.000000 aimped-0.1.53/aimped/nlp/assertion.py
+-rw-rw-rw-   0        0        0     3917 2023-04-03 13:18:42.000000 aimped-0.1.53/aimped/nlp/chunker.py
+-rw-rw-rw-   0        0        0     2825 2023-04-03 13:18:42.000000 aimped-0.1.53/aimped/nlp/deid.py
+-rw-rw-rw-   0        0        0     4521 2023-04-03 13:18:42.000000 aimped-0.1.53/aimped/nlp/ner.py
+-rw-rw-rw-   0        0        0     2629 2023-04-03 13:18:42.000000 aimped-0.1.53/aimped/nlp/ner_cls_report.py
+-rw-rw-rw-   0        0        0     7055 2023-06-26 17:27:03.000000 aimped-0.1.53/aimped/nlp/pipeline.py
+-rw-rw-rw-   0        0        0     3899 2023-04-03 13:18:42.000000 aimped-0.1.53/aimped/nlp/regex_parser.py
+-rw-rw-rw-   0        0        0     4394 2023-06-26 17:27:03.000000 aimped-0.1.53/aimped/nlp/relation.py
+-rw-rw-rw-   0        0        0    19853 2023-04-03 15:23:07.000000 aimped-0.1.53/aimped/nlp/relation_visualizer.py
+-rw-rw-rw-   0        0        0      803 2023-04-03 13:18:42.000000 aimped-0.1.53/aimped/nlp/tokenizer.py
+-rw-rw-rw-   0        0        0     2251 2023-04-03 13:18:42.000000 aimped-0.1.53/aimped/nlp/tools.py
+-rw-rw-rw-   0        0        0     2587 2023-05-24 09:15:05.000000 aimped-0.1.53/aimped/nlp/translation.py
+drwxrwxrwx   0        0        0        0 2023-06-26 18:51:58.705458 aimped-0.1.53/aimped/test/
+-rw-rw-rw-   0        0        0        0 2023-04-03 13:18:42.000000 aimped-0.1.53/aimped/test/__init__.py
+-rw-rw-rw-   0        0        0     2748 2023-04-03 13:18:42.000000 aimped-0.1.53/aimped/test/test_assertion.py
+-rw-rw-rw-   0        0        0     1313 2023-04-03 13:18:42.000000 aimped-0.1.53/aimped/test/test_chunk_merger.py
+-rw-rw-rw-   0        0        0     1866 2023-04-03 13:18:42.000000 aimped-0.1.53/aimped/test/test_deid_pipeline.py
+-rw-rw-rw-   0        0        0     1297 2023-04-03 13:18:42.000000 aimped-0.1.53/aimped/test/test_ner_results.py
+-rw-rw-rw-   0        0        0     1592 2023-04-03 13:18:42.000000 aimped-0.1.53/aimped/test/test_regex_parser.py
+-rw-rw-rw-   0        0        0     3320 2023-04-03 13:18:42.000000 aimped-0.1.53/aimped/test/test_relation_pipeline.py
+-rw-rw-rw-   0        0        0      610 2023-04-03 13:18:42.000000 aimped-0.1.53/aimped/test/test_tokenizer.py
+-rw-rw-rw-   0        0        0     5585 2023-04-03 13:18:42.000000 aimped-0.1.53/aimped/test/test_translation_pipeline.py
+-rw-rw-rw-   0        0        0     2060 2023-06-05 10:53:19.000000 aimped-0.1.53/aimped/utils.py
+-rw-rw-rw-   0        0        0      130 2023-06-26 18:48:01.000000 aimped-0.1.53/aimped/version.py
+drwxrwxrwx   0        0        0        0 2023-06-26 18:51:58.667523 aimped-0.1.53/aimped.egg-info/
+-rw-rw-rw-   0        0        0     1778 2023-06-26 18:51:58.000000 aimped-0.1.53/aimped.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      952 2023-06-26 18:51:58.000000 aimped-0.1.53/aimped.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-26 18:51:58.000000 aimped-0.1.53/aimped.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       48 2023-06-26 18:51:58.000000 aimped-0.1.53/aimped.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        7 2023-06-26 18:51:58.000000 aimped-0.1.53/aimped.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0      111 2023-06-26 18:51:58.708452 aimped-0.1.53/setup.cfg
+-rw-rw-rw-   0        0        0     1176 2023-06-26 18:51:33.000000 aimped-0.1.53/setup.py
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive (GNU)
+POSIX tar archive
```

### Comparing `aimped-0.1.52/PKG-INFO` & `aimped-0.1.53/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,68 +1,64 @@
-Metadata-Version: 2.1
-Name: aimped
-Version: 0.1.52
-Summary: Aimped is a unique library that provides classes and functions for only exclusively business-tailored AI-based NLP models.
-Home-page: https://dev.aimped.ai/
-Author: Russell C.
-Author-email: russell@aimped.com
-Maintainer: aimped
-Maintainer-email: contact@aimped.com
-License: UNKNOWN
-Platform: UNKNOWN
-Classifier: Programming Language :: Python :: 3
-Classifier: License :: OSI Approved :: MIT License
-Classifier: Operating System :: OS Independent
-Requires-Python: >=3.8
-Description-Content-Type: text/markdown
-License-File: LICENSE
-
-# **aimped**
-![aimped](https://dev.aimped.ai/static/media/AimpedBirdLogo.0b3c7cc26d31afe7bd73db496acb01d1.svg)
-
-**Aimped is a unique python library that provides classes and functions for only exclusively business-tailored AI-based NLP models.**  
-
-# Installation  
-```python
-pip install aimped
-```
-
-# Usage  
-```python  
-import aimped
-print(aimped.__version__)
-```
-## Examples  
-
-### Example 1
-
-```python  
-from aimped import nlp
-
-result = nlp.sentence_tokenizer("Hi, welcome to aimped. Explore ai models.",language="english")
-print(result)
-# ['Hi, welcome to aimped.', 'Explore ai models.']
-```
-
-### Example 2
-```python  
-from aimped.nlp.tokenizer import sentence_tokenizer
-
-result = sentence_tokenizer("Hi, welcome to aimped. Explore ai models.",language="english")
-print(result)
-# ['Hi, welcome to aimped.', 'Explore ai models.']
-```
-
-### Example 3
-```python  
-from aimped.nlp.pipeline import Pipeline
-
-pipe = Pipeline(model=model, tokenizer=tokenizer, device='cpu')
-result = pipe.ner_result(
-                        text=text,
-                        sents_tokens_list=sents_tokens_list,
-                        sentences=sentences)
-print(result)
-```
-
-
-
+Metadata-Version: 2.1
+Name: aimped
+Version: 0.1.53
+Summary: Aimped is a unique library that provides classes and functions for only exclusively business-tailored AI-based NLP models.
+Home-page: https://dev.aimped.ai/
+Author: Russell C.
+Author-email: russell@aimped.com
+Maintainer: aimped
+Maintainer-email: contact@aimped.com
+Classifier: Programming Language :: Python :: 3
+Classifier: License :: OSI Approved :: MIT License
+Classifier: Operating System :: OS Independent
+Requires-Python: >=3.8
+Description-Content-Type: text/markdown
+License-File: LICENSE
+
+# **aimped**
+![aimped](https://dev.aimped.ai/static/media/AimpedBirdLogo.0b3c7cc26d31afe7bd73db496acb01d1.svg)
+
+**Aimped is a unique python library that provides classes and functions for only exclusively business-tailored AI-based NLP models.**  
+
+# Installation  
+```python
+pip install aimped
+```
+
+# Usage  
+```python  
+import aimped
+print(aimped.__version__)
+```
+## Examples  
+
+### Example 1
+
+```python  
+from aimped import nlp
+
+result = nlp.sentence_tokenizer("Hi, welcome to aimped. Explore ai models.",language="english")
+print(result)
+# ['Hi, welcome to aimped.', 'Explore ai models.']
+```
+
+### Example 2
+```python  
+from aimped.nlp.tokenizer import sentence_tokenizer
+
+result = sentence_tokenizer("Hi, welcome to aimped. Explore ai models.",language="english")
+print(result)
+# ['Hi, welcome to aimped.', 'Explore ai models.']
+```
+
+### Example 3
+```python  
+from aimped.nlp.pipeline import Pipeline
+
+pipe = Pipeline(model=model, tokenizer=tokenizer, device='cpu')
+result = pipe.ner_result(
+                        text=text,
+                        sents_tokens_list=sents_tokens_list,
+                        sentences=sentences)
+print(result)
+```
+
```

### Comparing `aimped-0.1.52/aimped/test/test_chunk_merger.py` & `aimped-0.1.53/aimped/test/test_chunk_merger.py`

 * *Files identical despite different names*

### Comparing `aimped-0.1.52/aimped/test/test_relation_pipeline.py` & `aimped-0.1.53/aimped/test/test_relation_pipeline.py`

 * *Files identical despite different names*

### Comparing `aimped-0.1.52/aimped/test/test_tokenizer.py` & `aimped-0.1.53/aimped/test/test_tokenizer.py`

 * *Files identical despite different names*

### Comparing `aimped-0.1.52/aimped/test/test_regex_parser.py` & `aimped-0.1.53/aimped/test/test_regex_parser.py`

 * *Files identical despite different names*

### Comparing `aimped-0.1.52/aimped/test/test_translation_pipeline.py` & `aimped-0.1.53/aimped/test/test_translation_pipeline.py`

 * *Files identical despite different names*

### Comparing `aimped-0.1.52/aimped/test/test_ner_results.py` & `aimped-0.1.53/aimped/test/test_ner_results.py`

 * *Files identical despite different names*

### Comparing `aimped-0.1.52/aimped/test/test_assertion.py` & `aimped-0.1.53/aimped/test/test_assertion.py`

 * *Files identical despite different names*

### Comparing `aimped-0.1.52/aimped/test/test_deid_pipeline.py` & `aimped-0.1.53/aimped/test/test_deid_pipeline.py`

 * *Files identical despite different names*

### Comparing `aimped-0.1.52/aimped/utils.py` & `aimped-0.1.53/aimped/utils.py`

 * *Files identical despite different names*

### Comparing `aimped-0.1.52/aimped/model/load.py` & `aimped-0.1.53/aimped/model/load.py`

 * *Files identical despite different names*

### Comparing `aimped-0.1.52/aimped/nlp/relation_visualizer.py` & `aimped-0.1.53/aimped/nlp/relation_visualizer.py`

 * *Files identical despite different names*

### Comparing `aimped-0.1.52/aimped/nlp/chunker.py` & `aimped-0.1.53/aimped/nlp/chunker.py`

 * *Files identical despite different names*

### Comparing `aimped-0.1.52/aimped/nlp/tools.py` & `aimped-0.1.53/aimped/nlp/tools.py`

 * *Files identical despite different names*

### Comparing `aimped-0.1.52/aimped/nlp/assertion.py` & `aimped-0.1.53/aimped/nlp/assertion.py`

 * *Files identical despite different names*

### Comparing `aimped-0.1.52/aimped/nlp/tokenizer.py` & `aimped-0.1.53/aimped/nlp/tokenizer.py`

 * *Files identical despite different names*

### Comparing `aimped-0.1.52/aimped/nlp/ner_cls_report.py` & `aimped-0.1.53/aimped/nlp/ner_cls_report.py`

 * *Files identical despite different names*

### Comparing `aimped-0.1.52/aimped/nlp/ner.py` & `aimped-0.1.53/aimped/nlp/ner.py`

 * *Files identical despite different names*

### Comparing `aimped-0.1.52/aimped/nlp/deid.py` & `aimped-0.1.53/aimped/nlp/deid.py`

 * *Files identical despite different names*

### Comparing `aimped-0.1.52/aimped/nlp/pipeline.py` & `aimped-0.1.53/aimped/nlp/pipeline.py`

 * *Ordering differences only*

 * *Files 26% similar despite different names*

```diff
@@ -1,182 +1,182 @@
-# Author AIMPED
-# Date 2023-March-11
-# Description: This file contains the pipeline wrapper for NER, Assertion and De-identification models.
-
-
-class Pipeline:
-    """
-    It returns the ner results of a text.
-    parameters:
-    ----------------
-    task: str
-    text: str
-    model: transformers.modeling_utils.PreTrainedModel
-    tokenizer: transformers.tokenization_utils_base.PreTrainedTokenizer
-    *args: arguments
-    **kwargs: keyword arguments
-    return:
-    ----------------
-    results: list of dict
-    """
-
-    def __init__(self, tokenizer, model, device='cpu'):
-        """Initialize the pipeline class."""
-        self.tokenizer = tokenizer
-        self.model = model
-        self.device = device
-
-    def ner_result(self, text, sents_tokens_list, sentences, assertion_relation=False):
-        """It returns the ner results of a text.
-        parameters:
-        ----------------
-        text: str
-        sents_tokens_list: list of list of str
-        assertion_relation: bool
-        sentences: list of str
-        return:
-        ----------------
-        ner_results: list of dict"""
-        from aimped.nlp.ner import NerModelResults
-        ner_results = NerModelResults(text=text,
-                                      tokenizer=self.tokenizer,
-                                      model=self.model,
-                                      device=self.device,
-                                      sents_tokens_list=sents_tokens_list,
-                                      sentences=sentences,
-                                      assertion_relation=assertion_relation
-                                      )
-
-        return ner_results
-
-    def deid_result(self, text, merged_results, fake_csv_path, faked=False, masked=False):
-        """It returns the deid results of a text.
-        parameters:
-        ----------------
-        text: str
-        merged_results: list of dict
-        fake_csv_path: str
-        faked: bool
-        masked: bool
-        return:
-        ----------------
-        results: list of dict
-        """
-        from aimped.nlp.deid import maskText, fakedChunk, fakedText, deidentification
-        results = deidentification(text=text,
-                                   merged_results=merged_results,
-                                   fake_csv_path=fake_csv_path,
-                                   faked=faked,
-                                   masked=masked)
-        return results
-
-    def assertion_result(self, ner_results, sentences, classifier, assertion_white_label_list):
-        """It returns the assertion results of a text.
-        parameters:
-        ----------------
-        text: str
-        ner_results: list of dict
-        sentences: list of str
-        classifier: str
-        return:
-        ----------------
-        results: list of dict
-        """
-        from aimped.nlp.assertion import AssertionAnnotateSentence, AssertionModelResults
-        results = AssertionModelResults(ner_results=ner_results,
-                                        sentences=sentences,
-                                        classifier=classifier,
-                                        assertion_white_label_list=assertion_white_label_list
-                                        )
-        return results
-
-    def chunker_result(self, text, white_label_list, tokens, preds, probs, begins, ends,
-                       assertion_relation=False, sent_begins=[], sent_ends=[], sent_idxs=[]):
-        """It returns the merged chunks of a text.
-        parameters:
-        ----------------
-        text: str
-        white_label_list: list of str
-        tokens: list of str
-        preds: list of str
-        probs: list of float
-        begins: list of int
-        ends: list of int
-        assertion_relation: bool
-        sent_begins: list of int
-        sent_ends: list of int
-        sent_idxs: list of int
-        return:
-        ----------------
-        results: list of dict
-        """
-        from aimped.nlp.chunker import ChunkMerger
-        results = ChunkMerger(text=text,
-                              white_label_list=white_label_list,
-                              tokens=tokens,
-                              preds=preds,
-                              probs=probs,
-                              begins=begins,
-                              ends=ends,
-                              assertion_relation=assertion_relation,
-                              sent_begins=sent_begins,
-                              sent_ends=sent_ends,
-                              sent_idxs=sent_idxs)
-        return results
-
-    def regex_model_output_merger(self, regex_json_files_path, model_results, text, white_label_list):
-        """It returns the regex results of a text.
-        parameters:
-        ----------------
-        regex_json_files_path: str
-        model_results: list of dict
-        text: str
-        white_label_list: list of str
-        return:
-        ----------------
-        results: list of dict
-        """
-        from aimped.nlp.regex_parser import RegexNerParser, RegexModelNerMerger, RegexModelOutputMerger
-        import glob
-        regex_json_files_path_list = glob.glob(f"{regex_json_files_path}/*.json")
-
-        merged_results = RegexModelOutputMerger(regex_json_files_path_list=regex_json_files_path_list,
-                                                model_results=model_results,
-                                                text=text,
-                                                white_label_list=white_label_list)
-        return merged_results
-
-    def relation_result(self, sentences, ner_chunk_results, relation_classifier,
-                        relation_white_label_list, relation_pairs, return_svg=False):
-        """It returns the relation results of a text.
-        parameters:
-        ----------------
-        sentences: list of str
-        ner_chunk_results: list of dict
-        relation_classifier: str
-        ner_white_label_list: list of str
-        relation_white_label_list: list of str
-        one_to_many: bool = True
-        one_label: str = None
-        return_svg: bool = False
-        return:
-        ----------------
-        results: list of dict
-        """
-        from aimped.nlp.relation import RelationResults, RelationAnnotateSentence
-        results = RelationResults(sentences=sentences,
-                                  ner_chunk_results=ner_chunk_results,
-                                  relation_classifier=relation_classifier,
-                                  relation_white_label_list=relation_white_label_list,
-                                  relation_pairs =relation_pairs,
-                                  return_svg=return_svg)
-        return results
-
- 
-   
-
-    def __str__(self) -> str:
-        """Return the string representation of the pipeline."""
-        return f"Pipeline(model={self.model}, tokenizer={self.tokenizer})"
-
-
-
+# Author AIMPED
+# Date 2023-March-11
+# Description: This file contains the pipeline wrapper for NER, Assertion and De-identification models.
+
+
+class Pipeline:
+    """
+    It returns the ner results of a text.
+    parameters:
+    ----------------
+    task: str
+    text: str
+    model: transformers.modeling_utils.PreTrainedModel
+    tokenizer: transformers.tokenization_utils_base.PreTrainedTokenizer
+    *args: arguments
+    **kwargs: keyword arguments
+    return:
+    ----------------
+    results: list of dict
+    """
+
+    def __init__(self, tokenizer, model, device='cpu'):
+        """Initialize the pipeline class."""
+        self.tokenizer = tokenizer
+        self.model = model
+        self.device = device
+
+    def ner_result(self, text, sents_tokens_list, sentences, assertion_relation=False):
+        """It returns the ner results of a text.
+        parameters:
+        ----------------
+        text: str
+        sents_tokens_list: list of list of str
+        assertion_relation: bool
+        sentences: list of str
+        return:
+        ----------------
+        ner_results: list of dict"""
+        from aimped.nlp.ner import NerModelResults
+        ner_results = NerModelResults(text=text,
+                                      tokenizer=self.tokenizer,
+                                      model=self.model,
+                                      device=self.device,
+                                      sents_tokens_list=sents_tokens_list,
+                                      sentences=sentences,
+                                      assertion_relation=assertion_relation
+                                      )
+
+        return ner_results
+
+    def deid_result(self, text, merged_results, fake_csv_path, faked=False, masked=False):
+        """It returns the deid results of a text.
+        parameters:
+        ----------------
+        text: str
+        merged_results: list of dict
+        fake_csv_path: str
+        faked: bool
+        masked: bool
+        return:
+        ----------------
+        results: list of dict
+        """
+        from aimped.nlp.deid import maskText, fakedChunk, fakedText, deidentification
+        results = deidentification(text=text,
+                                   merged_results=merged_results,
+                                   fake_csv_path=fake_csv_path,
+                                   faked=faked,
+                                   masked=masked)
+        return results
+
+    def assertion_result(self, ner_results, sentences, classifier, assertion_white_label_list):
+        """It returns the assertion results of a text.
+        parameters:
+        ----------------
+        text: str
+        ner_results: list of dict
+        sentences: list of str
+        classifier: str
+        return:
+        ----------------
+        results: list of dict
+        """
+        from aimped.nlp.assertion import AssertionAnnotateSentence, AssertionModelResults
+        results = AssertionModelResults(ner_results=ner_results,
+                                        sentences=sentences,
+                                        classifier=classifier,
+                                        assertion_white_label_list=assertion_white_label_list
+                                        )
+        return results
+
+    def chunker_result(self, text, white_label_list, tokens, preds, probs, begins, ends,
+                       assertion_relation=False, sent_begins=[], sent_ends=[], sent_idxs=[]):
+        """It returns the merged chunks of a text.
+        parameters:
+        ----------------
+        text: str
+        white_label_list: list of str
+        tokens: list of str
+        preds: list of str
+        probs: list of float
+        begins: list of int
+        ends: list of int
+        assertion_relation: bool
+        sent_begins: list of int
+        sent_ends: list of int
+        sent_idxs: list of int
+        return:
+        ----------------
+        results: list of dict
+        """
+        from aimped.nlp.chunker import ChunkMerger
+        results = ChunkMerger(text=text,
+                              white_label_list=white_label_list,
+                              tokens=tokens,
+                              preds=preds,
+                              probs=probs,
+                              begins=begins,
+                              ends=ends,
+                              assertion_relation=assertion_relation,
+                              sent_begins=sent_begins,
+                              sent_ends=sent_ends,
+                              sent_idxs=sent_idxs)
+        return results
+
+    def regex_model_output_merger(self, regex_json_files_path, model_results, text, white_label_list):
+        """It returns the regex results of a text.
+        parameters:
+        ----------------
+        regex_json_files_path: str
+        model_results: list of dict
+        text: str
+        white_label_list: list of str
+        return:
+        ----------------
+        results: list of dict
+        """
+        from aimped.nlp.regex_parser import RegexNerParser, RegexModelNerMerger, RegexModelOutputMerger
+        import glob
+        regex_json_files_path_list = glob.glob(f"{regex_json_files_path}/*.json")
+
+        merged_results = RegexModelOutputMerger(regex_json_files_path_list=regex_json_files_path_list,
+                                                model_results=model_results,
+                                                text=text,
+                                                white_label_list=white_label_list)
+        return merged_results
+
+    def relation_result(self, sentences, ner_chunk_results, relation_classifier,
+                        relation_white_label_list, relation_pairs, return_svg=False):
+        """It returns the relation results of a text.
+        parameters:
+        ----------------
+        sentences: list of str
+        ner_chunk_results: list of dict
+        relation_classifier: str
+        ner_white_label_list: list of str
+        relation_white_label_list: list of str
+        one_to_many: bool = True
+        one_label: str = None
+        return_svg: bool = False
+        return:
+        ----------------
+        results: list of dict
+        """
+        from aimped.nlp.relation import RelationResults, RelationAnnotateSentence
+        results = RelationResults(sentences=sentences,
+                                  ner_chunk_results=ner_chunk_results,
+                                  relation_classifier=relation_classifier,
+                                  relation_white_label_list=relation_white_label_list,
+                                  relation_pairs =relation_pairs,
+                                  return_svg=return_svg)
+        return results
+
+ 
+   
+
+    def __str__(self) -> str:
+        """Return the string representation of the pipeline."""
+        return f"Pipeline(model={self.model}, tokenizer={self.tokenizer})"
+
+
+
```

### Comparing `aimped-0.1.52/aimped/nlp/regex_parser.py` & `aimped-0.1.53/aimped/nlp/regex_parser.py`

 * *Files identical despite different names*

### Comparing `aimped-0.1.52/LICENSE` & `aimped-0.1.53/LICENSE`

 * *Files identical despite different names*

### Comparing `aimped-0.1.52/README.md` & `aimped-0.1.53/README.md`

 * *Ordering differences only*

 * *Files 16% similar despite different names*

```diff
@@ -1,48 +1,48 @@
-# **aimped**
-![aimped](https://dev.aimped.ai/static/media/AimpedBirdLogo.0b3c7cc26d31afe7bd73db496acb01d1.svg)
-
-**Aimped is a unique python library that provides classes and functions for only exclusively business-tailored AI-based NLP models.**  
-
-# Installation  
-```python
-pip install aimped
-```
-
-# Usage  
-```python  
-import aimped
-print(aimped.__version__)
-```
-## Examples  
-
-### Example 1
-
-```python  
-from aimped import nlp
-
-result = nlp.sentence_tokenizer("Hi, welcome to aimped. Explore ai models.",language="english")
-print(result)
-# ['Hi, welcome to aimped.', 'Explore ai models.']
-```
-
-### Example 2
-```python  
-from aimped.nlp.tokenizer import sentence_tokenizer
-
-result = sentence_tokenizer("Hi, welcome to aimped. Explore ai models.",language="english")
-print(result)
-# ['Hi, welcome to aimped.', 'Explore ai models.']
-```
-
-### Example 3
-```python  
-from aimped.nlp.pipeline import Pipeline
-
-pipe = Pipeline(model=model, tokenizer=tokenizer, device='cpu')
-result = pipe.ner_result(
-                        text=text,
-                        sents_tokens_list=sents_tokens_list,
-                        sentences=sentences)
-print(result)
-```
-
+# **aimped**
+![aimped](https://dev.aimped.ai/static/media/AimpedBirdLogo.0b3c7cc26d31afe7bd73db496acb01d1.svg)
+
+**Aimped is a unique python library that provides classes and functions for only exclusively business-tailored AI-based NLP models.**  
+
+# Installation  
+```python
+pip install aimped
+```
+
+# Usage  
+```python  
+import aimped
+print(aimped.__version__)
+```
+## Examples  
+
+### Example 1
+
+```python  
+from aimped import nlp
+
+result = nlp.sentence_tokenizer("Hi, welcome to aimped. Explore ai models.",language="english")
+print(result)
+# ['Hi, welcome to aimped.', 'Explore ai models.']
+```
+
+### Example 2
+```python  
+from aimped.nlp.tokenizer import sentence_tokenizer
+
+result = sentence_tokenizer("Hi, welcome to aimped. Explore ai models.",language="english")
+print(result)
+# ['Hi, welcome to aimped.', 'Explore ai models.']
+```
+
+### Example 3
+```python  
+from aimped.nlp.pipeline import Pipeline
+
+pipe = Pipeline(model=model, tokenizer=tokenizer, device='cpu')
+result = pipe.ner_result(
+                        text=text,
+                        sents_tokens_list=sents_tokens_list,
+                        sentences=sentences)
+print(result)
+```
+
```

### Comparing `aimped-0.1.52/setup.py` & `aimped-0.1.53/setup.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-#Author: Russell C.
+#Author: Russell, Raife, Forrest
 #Date: 2023-03-20
 #Copyright: (c) 2023 aimped
 #Description: This is the setup file for the aimped library.
 
 import setuptools
 from aimped.version import __version__
```

### Comparing `aimped-0.1.52/aimped.egg-info/PKG-INFO` & `aimped-0.1.53/aimped.egg-info/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,68 +1,64 @@
-Metadata-Version: 2.1
-Name: aimped
-Version: 0.1.52
-Summary: Aimped is a unique library that provides classes and functions for only exclusively business-tailored AI-based NLP models.
-Home-page: https://dev.aimped.ai/
-Author: Russell C.
-Author-email: russell@aimped.com
-Maintainer: aimped
-Maintainer-email: contact@aimped.com
-License: UNKNOWN
-Platform: UNKNOWN
-Classifier: Programming Language :: Python :: 3
-Classifier: License :: OSI Approved :: MIT License
-Classifier: Operating System :: OS Independent
-Requires-Python: >=3.8
-Description-Content-Type: text/markdown
-License-File: LICENSE
-
-# **aimped**
-![aimped](https://dev.aimped.ai/static/media/AimpedBirdLogo.0b3c7cc26d31afe7bd73db496acb01d1.svg)
-
-**Aimped is a unique python library that provides classes and functions for only exclusively business-tailored AI-based NLP models.**  
-
-# Installation  
-```python
-pip install aimped
-```
-
-# Usage  
-```python  
-import aimped
-print(aimped.__version__)
-```
-## Examples  
-
-### Example 1
-
-```python  
-from aimped import nlp
-
-result = nlp.sentence_tokenizer("Hi, welcome to aimped. Explore ai models.",language="english")
-print(result)
-# ['Hi, welcome to aimped.', 'Explore ai models.']
-```
-
-### Example 2
-```python  
-from aimped.nlp.tokenizer import sentence_tokenizer
-
-result = sentence_tokenizer("Hi, welcome to aimped. Explore ai models.",language="english")
-print(result)
-# ['Hi, welcome to aimped.', 'Explore ai models.']
-```
-
-### Example 3
-```python  
-from aimped.nlp.pipeline import Pipeline
-
-pipe = Pipeline(model=model, tokenizer=tokenizer, device='cpu')
-result = pipe.ner_result(
-                        text=text,
-                        sents_tokens_list=sents_tokens_list,
-                        sentences=sentences)
-print(result)
-```
-
-
-
+Metadata-Version: 2.1
+Name: aimped
+Version: 0.1.53
+Summary: Aimped is a unique library that provides classes and functions for only exclusively business-tailored AI-based NLP models.
+Home-page: https://dev.aimped.ai/
+Author: Russell C.
+Author-email: russell@aimped.com
+Maintainer: aimped
+Maintainer-email: contact@aimped.com
+Classifier: Programming Language :: Python :: 3
+Classifier: License :: OSI Approved :: MIT License
+Classifier: Operating System :: OS Independent
+Requires-Python: >=3.8
+Description-Content-Type: text/markdown
+License-File: LICENSE
+
+# **aimped**
+![aimped](https://dev.aimped.ai/static/media/AimpedBirdLogo.0b3c7cc26d31afe7bd73db496acb01d1.svg)
+
+**Aimped is a unique python library that provides classes and functions for only exclusively business-tailored AI-based NLP models.**  
+
+# Installation  
+```python
+pip install aimped
+```
+
+# Usage  
+```python  
+import aimped
+print(aimped.__version__)
+```
+## Examples  
+
+### Example 1
+
+```python  
+from aimped import nlp
+
+result = nlp.sentence_tokenizer("Hi, welcome to aimped. Explore ai models.",language="english")
+print(result)
+# ['Hi, welcome to aimped.', 'Explore ai models.']
+```
+
+### Example 2
+```python  
+from aimped.nlp.tokenizer import sentence_tokenizer
+
+result = sentence_tokenizer("Hi, welcome to aimped. Explore ai models.",language="english")
+print(result)
+# ['Hi, welcome to aimped.', 'Explore ai models.']
+```
+
+### Example 3
+```python  
+from aimped.nlp.pipeline import Pipeline
+
+pipe = Pipeline(model=model, tokenizer=tokenizer, device='cpu')
+result = pipe.ner_result(
+                        text=text,
+                        sents_tokens_list=sents_tokens_list,
+                        sentences=sentences)
+print(result)
+```
+
```

### Comparing `aimped-0.1.52/aimped.egg-info/SOURCES.txt` & `aimped-0.1.53/aimped.egg-info/SOURCES.txt`

 * *Files identical despite different names*

