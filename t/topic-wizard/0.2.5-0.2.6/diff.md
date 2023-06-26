# Comparing `tmp/topic_wizard-0.2.5.tar.gz` & `tmp/topic_wizard-0.2.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "topic_wizard-0.2.5.tar", max compression
+gzip compressed data, was "topic_wizard-0.2.6.tar", max compression
```

## Comparing `topic_wizard-0.2.5.tar` & `topic_wizard-0.2.6.tar`

### file list

```diff
@@ -1,45 +1,46 @@
--rw-r--r--   0        0        0     1071 2022-09-18 11:34:01.304057 topic_wizard-0.2.5/LICENSE
--rw-r--r--   0        0        0     2908 2023-05-17 11:35:28.098112 topic_wizard-0.2.5/README.md
--rw-r--r--   0        0        0      640 2023-05-17 11:35:19.210098 topic_wizard-0.2.5/pyproject.toml
--rw-r--r--   0        0        0      404 2023-05-17 10:58:27.942406 topic_wizard-0.2.5/topicwizard/__init__.py
--rw-r--r--   0        0        0     7219 2023-05-17 10:58:27.942406 topic_wizard-0.2.5/topicwizard/app.py
--rw-r--r--   0        0        0   177216 2023-01-17 16:03:27.727135 topic_wizard-0.2.5/topicwizard/assets/favicon.ico
--rw-r--r--   0        0        0        0 2023-01-17 16:03:27.727135 topic_wizard-0.2.5/topicwizard/blueprints/__init__.py
--rw-r--r--   0        0        0     5602 2023-02-19 17:44:29.048902 topic_wizard-0.2.5/topicwizard/blueprints/app.py
--rw-r--r--   0        0        0     4322 2023-05-17 11:05:13.211055 topic_wizard-0.2.5/topicwizard/blueprints/documents.py
--rw-r--r--   0        0        0        0 2023-05-17 11:09:41.951533 topic_wizard-0.2.5/topicwizard/blueprints/groups.py
--rw-r--r--   0        0        0     1355 2023-01-17 16:03:27.727135 topic_wizard-0.2.5/topicwizard/blueprints/template.py
--rw-r--r--   0        0        0     5082 2023-05-17 11:05:33.415089 topic_wizard-0.2.5/topicwizard/blueprints/topics.py
--rw-r--r--   0        0        0     3015 2023-05-17 11:05:57.615132 topic_wizard-0.2.5/topicwizard/blueprints/words.py
--rw-r--r--   0        0        0     3010 2023-05-17 11:32:05.865790 topic_wizard-0.2.5/topicwizard/compatibility/bertopic.py
--rw-r--r--   0        0        0     6425 2023-05-17 11:33:07.273886 topic_wizard-0.2.5/topicwizard/compatibility/gensim.py
--rw-r--r--   0        0        0        0 2023-01-17 16:03:27.727135 topic_wizard-0.2.5/topicwizard/components/__init__.py
--rw-r--r--   0        0        0        0 2023-01-17 16:03:27.727135 topic_wizard-0.2.5/topicwizard/components/documents/__init__.py
--rw-r--r--   0        0        0     1993 2023-04-24 14:00:03.181792 topic_wizard-0.2.5/topicwizard/components/documents/document_map.py
--rw-r--r--   0        0        0     1399 2023-04-24 14:04:24.294134 topic_wizard-0.2.5/topicwizard/components/documents/document_pie.py
--rw-r--r--   0        0        0     1318 2023-02-19 17:10:14.965405 topic_wizard-0.2.5/topicwizard/components/documents/document_selector.py
--rw-r--r--   0        0        0     1468 2023-04-24 14:04:50.954173 topic_wizard-0.2.5/topicwizard/components/documents/document_timeline.py
--rw-r--r--   0        0        0     1131 2023-01-17 16:03:27.731135 topic_wizard-0.2.5/topicwizard/components/documents/document_wordcloud.py
--rw-r--r--   0        0        0     1362 2023-01-17 16:03:27.731135 topic_wizard-0.2.5/topicwizard/components/documents/window_slider.py
--rw-r--r--   0        0        0        0 2023-01-17 16:03:27.731135 topic_wizard-0.2.5/topicwizard/components/topics/__init__.py
--rw-r--r--   0        0        0     1906 2023-01-17 16:03:27.731135 topic_wizard-0.2.5/topicwizard/components/topics/intertopic_map.py
--rw-r--r--   0        0        0     1006 2023-01-17 16:03:27.731135 topic_wizard-0.2.5/topicwizard/components/topics/relevance_slider.py
--rw-r--r--   0        0        0      224 2023-01-17 16:03:27.731135 topic_wizard-0.2.5/topicwizard/components/topics/topic_barplot.py
--rw-r--r--   0        0        0     1568 2023-01-17 16:03:27.731135 topic_wizard-0.2.5/topicwizard/components/topics/topic_namer.py
--rw-r--r--   0        0        0     1447 2023-01-17 16:03:27.731135 topic_wizard-0.2.5/topicwizard/components/topics/topic_switcher.py
--rw-r--r--   0        0        0      228 2023-01-17 16:03:27.731135 topic_wizard-0.2.5/topicwizard/components/topics/wordcloud.py
--rw-r--r--   0        0        0        0 2023-01-17 16:03:27.731135 topic_wizard-0.2.5/topicwizard/components/words/__init__.py
--rw-r--r--   0        0        0     1880 2023-01-18 16:25:12.250356 topic_wizard-0.2.5/topicwizard/components/words/association_slider.py
--rw-r--r--   0        0        0     1762 2023-01-17 16:03:27.731135 topic_wizard-0.2.5/topicwizard/components/words/word_barplot.py
--rw-r--r--   0        0        0     2514 2023-04-24 14:33:48.501717 topic_wizard-0.2.5/topicwizard/components/words/word_map.py
--rw-r--r--   0        0        0     1300 2023-02-19 16:49:40.083205 topic_wizard-0.2.5/topicwizard/components/words/word_selector.py
--rw-r--r--   0        0        0        0 2022-11-04 10:16:21.833094 topic_wizard-0.2.5/topicwizard/plots/__init__.py
--rw-r--r--   0        0        0     5183 2023-05-17 10:58:27.942406 topic_wizard-0.2.5/topicwizard/plots/documents.py
--rw-r--r--   0        0        0     4257 2023-01-17 16:03:27.731135 topic_wizard-0.2.5/topicwizard/plots/topics.py
--rw-r--r--   0        0        0     3503 2023-04-24 14:33:17.069633 topic_wizard-0.2.5/topicwizard/plots/words.py
--rw-r--r--   0        0        0     2708 2023-04-24 13:29:18.682128 topic_wizard-0.2.5/topicwizard/prepare/documents.py
--rw-r--r--   0        0        0     4895 2023-05-17 10:58:27.942406 topic_wizard-0.2.5/topicwizard/prepare/topics.py
--rw-r--r--   0        0        0     1102 2023-01-17 16:03:27.735135 topic_wizard-0.2.5/topicwizard/prepare/utils.py
--rw-r--r--   0        0        0     4923 2023-04-24 14:35:51.642035 topic_wizard-0.2.5/topicwizard/prepare/words.py
--rw-r--r--   0        0        0     4204 1970-01-01 00:00:00.000000 topic_wizard-0.2.5/setup.py
--rw-r--r--   0        0        0     3931 1970-01-01 00:00:00.000000 topic_wizard-0.2.5/PKG-INFO
+-rw-r--r--   0        0        0     1071 2022-09-18 11:34:01.304057 topic_wizard-0.2.6/LICENSE
+-rw-r--r--   0        0        0     2908 2023-05-17 11:35:28.098112 topic_wizard-0.2.6/README.md
+-rw-r--r--   0        0        0      640 2023-06-26 07:38:06.759482 topic_wizard-0.2.6/pyproject.toml
+-rw-r--r--   0        0        0      404 2023-05-17 10:58:27.942406 topic_wizard-0.2.6/topicwizard/__init__.py
+-rw-r--r--   0        0        0     7219 2023-05-17 10:58:27.942406 topic_wizard-0.2.6/topicwizard/app.py
+-rw-r--r--   0        0        0   177216 2023-01-17 16:03:27.727135 topic_wizard-0.2.6/topicwizard/assets/favicon.ico
+-rw-r--r--   0        0        0        0 2023-01-17 16:03:27.727135 topic_wizard-0.2.6/topicwizard/blueprints/__init__.py
+-rw-r--r--   0        0        0     5602 2023-02-19 17:44:29.048902 topic_wizard-0.2.6/topicwizard/blueprints/app.py
+-rw-r--r--   0        0        0     4322 2023-05-17 11:05:13.211055 topic_wizard-0.2.6/topicwizard/blueprints/documents.py
+-rw-r--r--   0        0        0     1091 2023-05-17 13:10:22.409355 topic_wizard-0.2.6/topicwizard/blueprints/groups.py
+-rw-r--r--   0        0        0     1985 2023-06-26 07:34:43.425897 topic_wizard-0.2.6/topicwizard/blueprints/template.py
+-rw-r--r--   0        0        0     5082 2023-05-17 11:05:33.415089 topic_wizard-0.2.6/topicwizard/blueprints/topics.py
+-rw-r--r--   0        0        0     3015 2023-05-17 11:05:57.615132 topic_wizard-0.2.6/topicwizard/blueprints/words.py
+-rw-r--r--   0        0        0     3010 2023-05-17 11:32:05.865790 topic_wizard-0.2.6/topicwizard/compatibility/bertopic.py
+-rw-r--r--   0        0        0     6425 2023-05-17 11:33:07.273886 topic_wizard-0.2.6/topicwizard/compatibility/gensim.py
+-rw-r--r--   0        0        0        0 2023-01-17 16:03:27.727135 topic_wizard-0.2.6/topicwizard/components/__init__.py
+-rw-r--r--   0        0        0        0 2023-01-17 16:03:27.727135 topic_wizard-0.2.6/topicwizard/components/documents/__init__.py
+-rw-r--r--   0        0        0     1993 2023-04-24 14:00:03.181792 topic_wizard-0.2.6/topicwizard/components/documents/document_map.py
+-rw-r--r--   0        0        0     1399 2023-04-24 14:04:24.294134 topic_wizard-0.2.6/topicwizard/components/documents/document_pie.py
+-rw-r--r--   0        0        0     1318 2023-02-19 17:10:14.965405 topic_wizard-0.2.6/topicwizard/components/documents/document_selector.py
+-rw-r--r--   0        0        0     1468 2023-04-24 14:04:50.954173 topic_wizard-0.2.6/topicwizard/components/documents/document_timeline.py
+-rw-r--r--   0        0        0     1131 2023-01-17 16:03:27.731135 topic_wizard-0.2.6/topicwizard/components/documents/document_wordcloud.py
+-rw-r--r--   0        0        0     1362 2023-01-17 16:03:27.731135 topic_wizard-0.2.6/topicwizard/components/documents/window_slider.py
+-rw-r--r--   0        0        0        0 2023-01-17 16:03:27.731135 topic_wizard-0.2.6/topicwizard/components/topics/__init__.py
+-rw-r--r--   0        0        0     1906 2023-01-17 16:03:27.731135 topic_wizard-0.2.6/topicwizard/components/topics/intertopic_map.py
+-rw-r--r--   0        0        0     1006 2023-01-17 16:03:27.731135 topic_wizard-0.2.6/topicwizard/components/topics/relevance_slider.py
+-rw-r--r--   0        0        0      224 2023-01-17 16:03:27.731135 topic_wizard-0.2.6/topicwizard/components/topics/topic_barplot.py
+-rw-r--r--   0        0        0     1568 2023-01-17 16:03:27.731135 topic_wizard-0.2.6/topicwizard/components/topics/topic_namer.py
+-rw-r--r--   0        0        0     1447 2023-01-17 16:03:27.731135 topic_wizard-0.2.6/topicwizard/components/topics/topic_switcher.py
+-rw-r--r--   0        0        0      228 2023-01-17 16:03:27.731135 topic_wizard-0.2.6/topicwizard/components/topics/wordcloud.py
+-rw-r--r--   0        0        0        0 2023-01-17 16:03:27.731135 topic_wizard-0.2.6/topicwizard/components/words/__init__.py
+-rw-r--r--   0        0        0     1880 2023-01-18 16:25:12.250356 topic_wizard-0.2.6/topicwizard/components/words/association_slider.py
+-rw-r--r--   0        0        0     1762 2023-01-17 16:03:27.731135 topic_wizard-0.2.6/topicwizard/components/words/word_barplot.py
+-rw-r--r--   0        0        0     2514 2023-04-24 14:33:48.501717 topic_wizard-0.2.6/topicwizard/components/words/word_map.py
+-rw-r--r--   0        0        0     1300 2023-02-19 16:49:40.083205 topic_wizard-0.2.6/topicwizard/components/words/word_selector.py
+-rw-r--r--   0        0        0        0 2022-11-04 10:16:21.833094 topic_wizard-0.2.6/topicwizard/plots/__init__.py
+-rw-r--r--   0        0        0     5183 2023-05-17 10:58:27.942406 topic_wizard-0.2.6/topicwizard/plots/documents.py
+-rw-r--r--   0        0        0     4257 2023-01-17 16:03:27.731135 topic_wizard-0.2.6/topicwizard/plots/topics.py
+-rw-r--r--   0        0        0     3503 2023-04-24 14:33:17.069633 topic_wizard-0.2.6/topicwizard/plots/words.py
+-rw-r--r--   0        0        0     2708 2023-04-24 13:29:18.682128 topic_wizard-0.2.6/topicwizard/prepare/documents.py
+-rw-r--r--   0        0        0     3681 2023-05-17 13:42:09.111617 topic_wizard-0.2.6/topicwizard/prepare/groups.py
+-rw-r--r--   0        0        0     4895 2023-05-17 10:58:27.942406 topic_wizard-0.2.6/topicwizard/prepare/topics.py
+-rw-r--r--   0        0        0     1102 2023-01-17 16:03:27.735135 topic_wizard-0.2.6/topicwizard/prepare/utils.py
+-rw-r--r--   0        0        0     4923 2023-04-24 14:35:51.642035 topic_wizard-0.2.6/topicwizard/prepare/words.py
+-rw-r--r--   0        0        0     4204 1970-01-01 00:00:00.000000 topic_wizard-0.2.6/setup.py
+-rw-r--r--   0        0        0     3931 1970-01-01 00:00:00.000000 topic_wizard-0.2.6/PKG-INFO
```

### Comparing `topic_wizard-0.2.5/LICENSE` & `topic_wizard-0.2.6/LICENSE`

 * *Files identical despite different names*

### Comparing `topic_wizard-0.2.5/README.md` & `topic_wizard-0.2.6/README.md`

 * *Files identical despite different names*

### Comparing `topic_wizard-0.2.5/pyproject.toml` & `topic_wizard-0.2.6/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "topic-wizard"
-version = "0.2.5"
+version = "0.2.6"
 description = "Pretty and opinionated topic model visualization in Python."
 authors = ["Márton Kardos <power.up1163@gmail.com>"]
 license = "MIT"
 readme = "README.md"
 packages = [{include = "topicwizard"}]
 
 [tool.poetry.dependencies]
```

### Comparing `topic_wizard-0.2.5/topicwizard/app.py` & `topic_wizard-0.2.6/topicwizard/app.py`

 * *Files identical despite different names*

### Comparing `topic_wizard-0.2.5/topicwizard/assets/favicon.ico` & `topic_wizard-0.2.6/topicwizard/assets/favicon.ico`

 * *Files identical despite different names*

### Comparing `topic_wizard-0.2.5/topicwizard/blueprints/app.py` & `topic_wizard-0.2.6/topicwizard/blueprints/app.py`

 * *Files identical despite different names*

### Comparing `topic_wizard-0.2.5/topicwizard/blueprints/documents.py` & `topic_wizard-0.2.6/topicwizard/blueprints/documents.py`

 * *Files identical despite different names*

### Comparing `topic_wizard-0.2.5/topicwizard/blueprints/template.py` & `topic_wizard-0.2.6/topicwizard/blueprints/template.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,9 +1,11 @@
-from typing import Any, Iterable, Callable, List, Optional
+from typing import Any, Callable, Iterable, List, Optional
+from warnings import warn
 
+import numpy as np
 from dash_extensions.enrich import DashBlueprint
 
 from topicwizard.prepare.utils import get_vocab, prepare_transformed_data
 
 BlueprintCreator = Callable[..., DashBlueprint]
 
 
@@ -21,14 +23,25 @@
         document_names = [f"Document {i}" for i in range(n_documents)]
     vocab = get_vocab(vectorizer)
     (
         document_term_matrix,
         document_topic_matrix,
         topic_term_matrix,
     ) = prepare_transformed_data(vectorizer, topic_model, corpus)
+    nan_documents = np.isnan(document_topic_matrix).any(axis=1)
+    n_nan_docs = np.sum(nan_documents)
+    if n_nan_docs:
+        warn(
+            f"{n_nan_docs} documents had nan values in the output of the topic model,"
+            " these are removed in preprocessing and will not be visible in the app."
+        )
+        corpus = list(np.array(corpus)[~nan_documents])
+        document_topic_matrix = document_topic_matrix[~nan_documents]
+        document_term_matrix = document_term_matrix[~nan_documents]
+        document_names = list(np.array(document_names)[~nan_documents])
     n_topics = topic_term_matrix.shape[0]
     if topic_names is None:
         topic_names = [f"Topic {i}" for i in range(n_topics)]
     blueprint = create_blueprint(
         vocab=vocab,
         document_term_matrix=document_term_matrix,
         document_topic_matrix=document_topic_matrix,
```

### Comparing `topic_wizard-0.2.5/topicwizard/blueprints/topics.py` & `topic_wizard-0.2.6/topicwizard/blueprints/topics.py`

 * *Files identical despite different names*

### Comparing `topic_wizard-0.2.5/topicwizard/blueprints/words.py` & `topic_wizard-0.2.6/topicwizard/blueprints/words.py`

 * *Files identical despite different names*

### Comparing `topic_wizard-0.2.5/topicwizard/compatibility/bertopic.py` & `topic_wizard-0.2.6/topicwizard/compatibility/bertopic.py`

 * *Files identical despite different names*

### Comparing `topic_wizard-0.2.5/topicwizard/compatibility/gensim.py` & `topic_wizard-0.2.6/topicwizard/compatibility/gensim.py`

 * *Files identical despite different names*

### Comparing `topic_wizard-0.2.5/topicwizard/components/documents/document_map.py` & `topic_wizard-0.2.6/topicwizard/components/documents/document_map.py`

 * *Files identical despite different names*

### Comparing `topic_wizard-0.2.5/topicwizard/components/documents/document_pie.py` & `topic_wizard-0.2.6/topicwizard/components/documents/document_pie.py`

 * *Files identical despite different names*

### Comparing `topic_wizard-0.2.5/topicwizard/components/documents/document_selector.py` & `topic_wizard-0.2.6/topicwizard/components/documents/document_selector.py`

 * *Files identical despite different names*

### Comparing `topic_wizard-0.2.5/topicwizard/components/documents/document_timeline.py` & `topic_wizard-0.2.6/topicwizard/components/documents/document_timeline.py`

 * *Files identical despite different names*

### Comparing `topic_wizard-0.2.5/topicwizard/components/documents/document_wordcloud.py` & `topic_wizard-0.2.6/topicwizard/components/documents/document_wordcloud.py`

 * *Files identical despite different names*

### Comparing `topic_wizard-0.2.5/topicwizard/components/documents/window_slider.py` & `topic_wizard-0.2.6/topicwizard/components/documents/window_slider.py`

 * *Files identical despite different names*

### Comparing `topic_wizard-0.2.5/topicwizard/components/topics/intertopic_map.py` & `topic_wizard-0.2.6/topicwizard/components/topics/intertopic_map.py`

 * *Files identical despite different names*

### Comparing `topic_wizard-0.2.5/topicwizard/components/topics/relevance_slider.py` & `topic_wizard-0.2.6/topicwizard/components/topics/relevance_slider.py`

 * *Files identical despite different names*

### Comparing `topic_wizard-0.2.5/topicwizard/components/topics/topic_namer.py` & `topic_wizard-0.2.6/topicwizard/components/topics/topic_namer.py`

 * *Files identical despite different names*

### Comparing `topic_wizard-0.2.5/topicwizard/components/topics/topic_switcher.py` & `topic_wizard-0.2.6/topicwizard/components/topics/topic_switcher.py`

 * *Files identical despite different names*

### Comparing `topic_wizard-0.2.5/topicwizard/components/words/association_slider.py` & `topic_wizard-0.2.6/topicwizard/components/words/association_slider.py`

 * *Files identical despite different names*

### Comparing `topic_wizard-0.2.5/topicwizard/components/words/word_barplot.py` & `topic_wizard-0.2.6/topicwizard/components/words/word_barplot.py`

 * *Files identical despite different names*

### Comparing `topic_wizard-0.2.5/topicwizard/components/words/word_map.py` & `topic_wizard-0.2.6/topicwizard/components/words/word_map.py`

 * *Files identical despite different names*

### Comparing `topic_wizard-0.2.5/topicwizard/components/words/word_selector.py` & `topic_wizard-0.2.6/topicwizard/components/words/word_selector.py`

 * *Files identical despite different names*

### Comparing `topic_wizard-0.2.5/topicwizard/plots/documents.py` & `topic_wizard-0.2.6/topicwizard/plots/documents.py`

 * *Files identical despite different names*

### Comparing `topic_wizard-0.2.5/topicwizard/plots/topics.py` & `topic_wizard-0.2.6/topicwizard/plots/topics.py`

 * *Files identical despite different names*

### Comparing `topic_wizard-0.2.5/topicwizard/plots/words.py` & `topic_wizard-0.2.6/topicwizard/plots/words.py`

 * *Files identical despite different names*

### Comparing `topic_wizard-0.2.5/topicwizard/prepare/documents.py` & `topic_wizard-0.2.6/topicwizard/prepare/documents.py`

 * *Files identical despite different names*

### Comparing `topic_wizard-0.2.5/topicwizard/prepare/topics.py` & `topic_wizard-0.2.6/topicwizard/prepare/topics.py`

 * *Files identical despite different names*

### Comparing `topic_wizard-0.2.5/topicwizard/prepare/utils.py` & `topic_wizard-0.2.6/topicwizard/prepare/utils.py`

 * *Files identical despite different names*

### Comparing `topic_wizard-0.2.5/topicwizard/prepare/words.py` & `topic_wizard-0.2.6/topicwizard/prepare/words.py`

 * *Files identical despite different names*

### Comparing `topic_wizard-0.2.5/setup.py` & `topic_wizard-0.2.6/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -26,15 +26,15 @@
  'scikit-learn>=1.2.0,<1.3.0',
  'scipy>=1.8.0',
  'umap-learn>=0.5.3',
  'wordcloud>=1.8.2.2,<1.9.0.0']
 
 setup_kwargs = {
     'name': 'topic-wizard',
-    'version': '0.2.5',
+    'version': '0.2.6',
     'description': 'Pretty and opinionated topic model visualization in Python.',
     'long_description': '<img align="left" width="82" height="82" src="assets/logo.svg">\n\n# topicwizard\n\n<br>\n\nPretty and opinionated topic model visualization in Python.\n\n[![Open in Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/github/x-tabdeveloping/topic-wizard/blob/main/examples/basic_usage.ipynb)\n[![PyPI version](https://badge.fury.io/py/topic-wizard.svg)](https://pypi.org/project/topic-wizard/)\n[![pip downloads](https://img.shields.io/pypi/dm/topic-wizard.svg)](https://pypi.org/project/topic-wizard/)\n[![python version](https://img.shields.io/badge/Python-%3E=3.8-blue)](https://github.com/centre-for-humanities-computing/tweetopic)\n[![Code style: black](https://img.shields.io/badge/Code%20Style-Black-black)](https://black.readthedocs.io/en/stable/the_black_code_style/current_style.html)\n<br>\n\n\n\nhttps://user-images.githubusercontent.com/13087737/234209888-0d20ede9-2ea1-4d6e-b69b-71b863287cc9.mp4\n\n## New in version 0.2.5 🌟 🌟\n\n - [Compatiblity with Gensim topic models](https://x-tabdeveloping.github.io/topic-wizard/usage.compatibility.html) 💥\n - [Compatibility with BERTopic](https://x-tabdeveloping.github.io/topic-wizard/usage.compatibility.html)(experimental 🧪)\n - Topic name inference 🧠\n\n\n## Features\n\n-   Investigate complex relations between topics, words and documents\n-   Highly interactive\n-   Automatically infer topic names\n-   Name topics manually\n-   Pretty :art:\n-   Intuitive :cow:\n-   Clean API :candy:\n-   Sklearn, Gensim and BERTopic compatible :nut_and_bolt:\n-   Easy deployment :earth_africa:\n\n## Installation\n\nInstall from PyPI:\n\n```bash\npip install topic-wizard\n```\n\n## Usage ([documentation](https://x-tabdeveloping.github.io/topic-wizard/))\n\n### Step 1:\n\nTrain a scikit-learn compatible topic model.\n(If you want to use non-scikit-learn topic models, check [compatibility](https://x-tabdeveloping.github.io/topic-wizard/usage.compatibility.html))\n\n```python\nfrom sklearn.decomposition import NMF\nfrom sklearn.feature_extraction.text import CountVectorizer\nfrom sklearn.pipeline import make_pipeline\n\n# Create topic pipeline\ntopic_pipeline = make_pipeline(\n    CountVectorizer(),\n    NMF(n_components=10),\n)\n\n# Then fit it on the given texts\ntopic_pipeline.fit(texts)\n```\n\n### Step 2:\n\nVisualize with topicwizard.\n\n```python\nimport topicwizard\n\n# You can get automatically assigned topic labels, that you can change manually later\ntopic_names = topicwizard.infer_topic_names(pipeline=pipeline)\n\n# Then you can visualize your results\ntopicwizard.visualize(pipeline=topic_pipeline, corpus=texts, topic_names=topic_names)\n```\n\n### Step 3:\n\nInvestigate :eyes: .\n\n#### a) Topics\n\n![topics screenshot](assets/screenshot_topics.png)\n\n#### b) Words\n\n![words screenshot](assets/screenshot_words.png)\n![words screenshot](assets/screenshot_words_zoomed.png)\n\n#### c) Documents\n\n![documents screenshot](assets/screenshot_documents.png)\n',
     'author': 'Márton Kardos',
     'author_email': 'power.up1163@gmail.com',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'None',
```

### Comparing `topic_wizard-0.2.5/PKG-INFO` & `topic_wizard-0.2.6/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: topic-wizard
-Version: 0.2.5
+Version: 0.2.6
 Summary: Pretty and opinionated topic model visualization in Python.
 License: MIT
 Author: Márton Kardos
 Author-email: power.up1163@gmail.com
 Requires-Python: >=3.8.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
```

