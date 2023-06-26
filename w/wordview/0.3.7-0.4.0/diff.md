# Comparing `tmp/wordview-0.3.7.tar.gz` & `tmp/wordview-0.4.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "wordview-0.3.7.tar", max compression
+gzip compressed data, was "wordview-0.4.0.tar", max compression
```

## Comparing `wordview-0.3.7.tar` & `wordview-0.4.0.tar`

### file list

```diff
@@ -1,20 +1,20 @@
--rw-r--r--   0        0        0     1662 2023-06-23 09:52:21.149500 wordview-0.3.7/CHANGES.rst
--rw-r--r--   0        0        0     1074 2023-06-23 09:52:21.149500 wordview-0.3.7/LICENSE
--rw-r--r--   0        0        0     4638 2023-06-23 09:52:21.149500 wordview-0.3.7/README.rst
--rw-r--r--   0        0        0      873 2023-06-23 09:52:21.249501 wordview-0.3.7/pyproject.toml
--rw-r--r--   0        0        0      163 2023-06-23 09:52:21.249501 wordview-0.3.7/wordview/__init__.py
--rw-r--r--   0        0        0       60 2023-06-23 09:52:21.249501 wordview-0.3.7/wordview/anomaly/__init__.py
--rw-r--r--   0        0        0     7343 2023-06-23 09:52:21.249501 wordview-0.3.7/wordview/anomaly/gaussianize.py
--rw-r--r--   0        0        0     4788 2023-06-23 09:52:21.249501 wordview-0.3.7/wordview/anomaly/normaldist.py
--rw-r--r--   0        0        0       48 2023-06-23 09:52:21.249501 wordview-0.3.7/wordview/clustering/__init__.py
--rw-r--r--   0        0        0     3027 2023-06-23 09:52:21.249501 wordview-0.3.7/wordview/clustering/cluster.py
--rw-r--r--   0        0        0       85 2023-06-23 09:52:21.249501 wordview-0.3.7/wordview/mwes/__init__.py
--rw-r--r--   0        0        0     2900 2023-06-23 09:52:21.249501 wordview-0.3.7/wordview/mwes/am.py
--rw-r--r--   0        0        0     8698 2023-06-23 09:52:21.249501 wordview-0.3.7/wordview/mwes/mwe.py
--rw-r--r--   0        0        0     3962 2023-06-23 09:52:21.249501 wordview-0.3.7/wordview/mwes/mwe_utils.py
--rw-r--r--   0        0        0       55 2023-06-23 09:52:21.249501 wordview-0.3.7/wordview/preprocessing/__init__.py
--rw-r--r--   0        0        0     3078 2023-06-23 09:52:21.249501 wordview-0.3.7/wordview/preprocessing/cleaning.py
--rw-r--r--   0        0        0       75 2023-06-23 09:52:21.253501 wordview-0.3.7/wordview/text_analysis/__init__.py
--rw-r--r--   0        0        0    11805 2023-06-23 09:52:21.253501 wordview-0.3.7/wordview/text_analysis/core.py
--rw-r--r--   0        0        0     8399 2023-06-23 09:52:21.253501 wordview-0.3.7/wordview/text_analysis/wrapper.py
--rw-r--r--   0        0        0     5477 1970-01-01 00:00:00.000000 wordview-0.3.7/PKG-INFO
+-rw-r--r--   0        0        0     1771 2023-06-26 11:05:22.732620 wordview-0.4.0/CHANGES.rst
+-rw-r--r--   0        0        0     1074 2023-06-26 11:05:22.732620 wordview-0.4.0/LICENSE
+-rw-r--r--   0        0        0     4342 2023-06-26 11:05:22.732620 wordview-0.4.0/README.rst
+-rw-r--r--   0        0        0      873 2023-06-26 11:05:22.812623 wordview-0.4.0/pyproject.toml
+-rw-r--r--   0        0        0      163 2023-06-26 11:05:22.812623 wordview-0.4.0/wordview/__init__.py
+-rw-r--r--   0        0        0       60 2023-06-26 11:05:22.812623 wordview-0.4.0/wordview/anomaly/__init__.py
+-rw-r--r--   0        0        0     7343 2023-06-26 11:05:22.812623 wordview-0.4.0/wordview/anomaly/gaussianize.py
+-rw-r--r--   0        0        0     4788 2023-06-26 11:05:22.812623 wordview-0.4.0/wordview/anomaly/normaldist.py
+-rw-r--r--   0        0        0       48 2023-06-26 11:05:22.812623 wordview-0.4.0/wordview/clustering/__init__.py
+-rw-r--r--   0        0        0     3027 2023-06-26 11:05:22.812623 wordview-0.4.0/wordview/clustering/cluster.py
+-rw-r--r--   0        0        0       85 2023-06-26 11:05:22.812623 wordview-0.4.0/wordview/mwes/__init__.py
+-rw-r--r--   0        0        0     2900 2023-06-26 11:05:22.812623 wordview-0.4.0/wordview/mwes/am.py
+-rw-r--r--   0        0        0    11822 2023-06-26 11:05:22.812623 wordview-0.4.0/wordview/mwes/mwe.py
+-rw-r--r--   0        0        0     3962 2023-06-26 11:05:22.812623 wordview-0.4.0/wordview/mwes/mwe_utils.py
+-rw-r--r--   0        0        0       55 2023-06-26 11:05:22.812623 wordview-0.4.0/wordview/preprocessing/__init__.py
+-rw-r--r--   0        0        0     3078 2023-06-26 11:05:22.812623 wordview-0.4.0/wordview/preprocessing/cleaning.py
+-rw-r--r--   0        0        0       75 2023-06-26 11:05:22.812623 wordview-0.4.0/wordview/text_analysis/__init__.py
+-rw-r--r--   0        0        0    11805 2023-06-26 11:05:22.812623 wordview-0.4.0/wordview/text_analysis/core.py
+-rw-r--r--   0        0        0     8399 2023-06-26 11:05:22.812623 wordview-0.4.0/wordview/text_analysis/wrapper.py
+-rw-r--r--   0        0        0     5181 1970-01-01 00:00:00.000000 wordview-0.4.0/PKG-INFO
```

### Comparing `wordview-0.3.7/CHANGES.rst` & `wordview-0.4.0/CHANGES.rst`

 * *Files 3% similar despite different names*

```diff
@@ -1,7 +1,12 @@
+Version 0.4.0
+-------------
+- Support for extracting variable length MWE given a user pattern of POS tags.
+
+
 Version 0.3.7
 -------------
 - Change newline encoding.
 - To support multiline in GitHub release body.
 
 
 Version 0.3.6
```

### Comparing `wordview-0.3.7/LICENSE` & `wordview-0.4.0/LICENSE`

 * *Files identical despite different names*

### Comparing `wordview-0.3.7/README.rst` & `wordview-0.4.0/README.rst`

 * *Files 7% similar despite different names*

```diff
@@ -1,13 +1,19 @@
 Wordview (Work In Progress)
 ###########################
 
-|PyPI version|
 
-|Python 3.9|
+.. image:: https://img.shields.io/pypi/v/wordview
+   :alt: PyPI
+
+.. image:: https://img.shields.io/pypi/pyversions/wordview
+   :alt: PyPI - Python Version
+
+.. image:: https://img.shields.io/pypi/dm/wordview
+   :alt: PyPI - Downloads
 
 Wordview is a Python package for Exploratory Data Analysis (EDA) and Feature Extraction for text.
 Wordview's Python API is open-source and available under the `MIT
 license <https://en.wikipedia.org/wiki/MIT_License>`__. We, however,
 offer a framework on top of Wordview for enterprise use under a commercial license. See this page for
 more information about this framework.
 
@@ -89,24 +95,12 @@
 
 Contributing
 ############
 
 Thank you for contributing to wordview! We and the users of this repo
 appreciate your efforts! You can visit the `contributing page <CONTRIBUTING.rst>`__ for detailed instructions about how you can contribute to Wordview.
 
-
-.. |PyPI version| image:: https://badge.fury.io/py/wordview.svg
-    :target: https://badge.fury.io/py/wordview
-
-.. |Python 3.9| image:: https://img.shields.io/badge/python-3.9-blue.svg
-   :target: https://www.python.org/downloads/release/python-390/
-.. |verbs| image:: docs/figs/verbs.png
-.. |nouns| image:: docs/figs/nouns.png
-.. |adjs| image:: docs/figs/adjectives.png
-.. |doclen| image:: docs/figs/doclen.png
-.. |wordszipf| image:: docs/figs/wordszipf.png
-.. |labels| image:: docs/figs/labels.png
 .. |cover| image:: docs/figs/abstract_cover_2.png
 .. |clustering_cover| image:: docs/figs/clustering_cover.png
 .. |text_analysis_cover| image:: docs/figs/text_analysis.png
```

### Comparing `wordview-0.3.7/pyproject.toml` & `wordview-0.4.0/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "wordview"
-version = "0.3.7"
+version = "0.4.0"
 description = "Wordview is a Python package for text analysis."
 authors = ["meghdadFar <meghdad.farahmand@gmail.com>"]
 readme = "README.rst"
 include = ["CHANGES.rst"]
 license = "MIT"
 keywords = ["nlp", "text analysis", "statistics"]
```

### Comparing `wordview-0.3.7/wordview/anomaly/gaussianize.py` & `wordview-0.4.0/wordview/anomaly/gaussianize.py`

 * *Files identical despite different names*

### Comparing `wordview-0.3.7/wordview/anomaly/normaldist.py` & `wordview-0.4.0/wordview/anomaly/normaldist.py`

 * *Files identical despite different names*

### Comparing `wordview-0.3.7/wordview/clustering/cluster.py` & `wordview-0.4.0/wordview/clustering/cluster.py`

 * *Files identical despite different names*

### Comparing `wordview-0.3.7/wordview/mwes/am.py` & `wordview-0.4.0/wordview/mwes/am.py`

 * *Files identical despite different names*

### Comparing `wordview-0.3.7/wordview/mwes/mwe.py` & `wordview-0.4.0/wordview/mwes/mwe.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,16 +1,14 @@
 import json
-import re
 from collections import Counter
-from pathlib import Path
-from typing import Dict, List, Optional, Union
+from typing import Dict, Optional
 
 import pandas
 import tqdm
-from nltk import word_tokenize
+from nltk import RegexpParser, word_tokenize
 
 from wordview import logger
 from wordview.mwes.am import calculate_am
 from wordview.mwes.mwe_utils import get_pos_tags, is_alphanumeric_latinscript_multigram
 
 
 class MWE(object):
@@ -236,7 +234,85 @@
                         w3 = postag_tokens[i + 2]
                         if w3 not in ["NN", "NNS"]:
                             mwes.append(w1[0] + " " + w2[0])
                     else:
                         mwes.append(w1[0] + " " + w2[0])
         mwes_count_dic = Counter(mwes)
         return mwes_count_dic
+
+
+class HigherOrderMWEExtractor:
+    def __init__(self, tokens: list[str], pattern: str) -> None:
+        self.tokens = tokens
+        self.pattern = pattern
+        self._validate_input()
+
+    def _validate_input(self) -> None:
+        if not isinstance(self.tokens, list):
+            raise TypeError(
+                f'Input argument "tokens" must be a list of string. Currently it is of type {type(self.tokens)} \
+                with a value of: {self.tokens}.'
+            )
+        if len(self.tokens) == 0:
+            raise ValueError(
+                'Input argument "tokens" must be a non-empty list of string.'
+            )
+        if not isinstance(self.pattern, str):
+            raise TypeError(
+                f'Input argument "pattern" must be a string. Currently it is of type {type(self.pattern)} \
+                with a value of: {self.pattern}.'
+            )
+        if len(self.pattern) == 0:
+            raise ValueError(
+                'Input argument "pattern" must be a non-zero length string.'
+            )
+
+    def extract_higher_order_mwe_candidates(self) -> dict:
+        """
+        Extract variable-length MWE from tokenized input, using a user-defined POS regex pattern.
+
+        Parameters:
+            tokens (list[str]): A list of tuples containing the word and its corresponding part-of-speech tag.
+            pattern (str): A string containing a user-defined pattern for nltk.RegexpParser.
+
+        Returns:
+            match_counter (dict[str, dict[str, int]]): A counter dictionary with count of matched strings, grouped by pattern label.
+                                                    An empty list if none were found.
+
+        Examples of user-defined patterns:
+        - NP: {<DT>?<JJ>*<NN>} # Noun phrase
+        - VP: {<MD>?<VB.*><NP|PP|CLAUSE>+$} # Verb phrase
+        - PP: {<IN><NP>} # Prepositional phrase
+
+        You can use multiple and/or nested patterns, separated by a newline character:
+        pattern = '''
+        NP: {<DT>?<JJ>*<NN>} # Noun phrase
+        PROPN: {<NNP>+} # Proper noun
+        ADJP: {<RB|RBR|RBS>*<JJ>} # Adjective phrase
+        ADVP: {<RB.*>+<VB.*><RB.*>*} # Adverb phrase
+        '''
+
+        In this case, patterns of a clause are executed in order.  An earlier
+        pattern may introduce a chunk boundary that prevents a later pattern from executing.
+        """
+
+        tagged_tokens: list[tuple[str, str]] = get_pos_tags(self.tokens)
+        parser = RegexpParser(self.pattern)
+        parsed_tokens = parser.parse(tagged_tokens)
+
+        labels: list[str] = [
+            rule.split(":")[0].strip() for rule in self.pattern.split("\n") if rule
+        ]
+
+        matches: dict[str, list[str]] = {label: [] for label in labels}
+
+        for subtree in parsed_tokens.subtrees():
+            label = subtree.label()
+            if label in matches:
+                matches[label].append(
+                    " ".join(word for (word, tag) in subtree.leaves())
+                )
+
+        matches_counter: dict[str, dict[str, int]] = {
+            label: dict(Counter(match_list)) for label, match_list in matches.items()
+        }
+        return matches_counter
```

### Comparing `wordview-0.3.7/wordview/mwes/mwe_utils.py` & `wordview-0.4.0/wordview/mwes/mwe_utils.py`

 * *Files identical despite different names*

### Comparing `wordview-0.3.7/wordview/preprocessing/cleaning.py` & `wordview-0.4.0/wordview/preprocessing/cleaning.py`

 * *Files identical despite different names*

### Comparing `wordview-0.3.7/wordview/text_analysis/core.py` & `wordview-0.4.0/wordview/text_analysis/core.py`

 * *Files identical despite different names*

### Comparing `wordview-0.3.7/wordview/text_analysis/wrapper.py` & `wordview-0.4.0/wordview/text_analysis/wrapper.py`

 * *Files identical despite different names*

### Comparing `wordview-0.3.7/PKG-INFO` & `wordview-0.4.0/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: wordview
-Version: 0.3.7
+Version: 0.4.0
 Summary: Wordview is a Python package for text analysis.
 License: MIT
 Keywords: nlp,text analysis,statistics
 Author: meghdadFar
 Author-email: meghdad.farahmand@gmail.com
 Requires-Python: >=3.9,<3.11
 Classifier: License :: OSI Approved :: MIT License
@@ -22,17 +22,23 @@
 Requires-Dist: tqdm (==4.62.3)
 Requires-Dist: wordcloud (==1.9.1.1)
 Description-Content-Type: text/x-rst
 
 Wordview (Work In Progress)
 ###########################
 
-|PyPI version|
 
-|Python 3.9|
+.. image:: https://img.shields.io/pypi/v/wordview
+   :alt: PyPI
+
+.. image:: https://img.shields.io/pypi/pyversions/wordview
+   :alt: PyPI - Python Version
+
+.. image:: https://img.shields.io/pypi/dm/wordview
+   :alt: PyPI - Downloads
 
 Wordview is a Python package for Exploratory Data Analysis (EDA) and Feature Extraction for text.
 Wordview's Python API is open-source and available under the `MIT
 license <https://en.wikipedia.org/wiki/MIT_License>`__. We, however,
 offer a framework on top of Wordview for enterprise use under a commercial license. See this page for
 more information about this framework.
 
@@ -114,25 +120,13 @@
 
 Contributing
 ############
 
 Thank you for contributing to wordview! We and the users of this repo
 appreciate your efforts! You can visit the `contributing page <CONTRIBUTING.rst>`__ for detailed instructions about how you can contribute to Wordview.
 
-
-.. |PyPI version| image:: https://badge.fury.io/py/wordview.svg
-    :target: https://badge.fury.io/py/wordview
-
-.. |Python 3.9| image:: https://img.shields.io/badge/python-3.9-blue.svg
-   :target: https://www.python.org/downloads/release/python-390/
-.. |verbs| image:: docs/figs/verbs.png
-.. |nouns| image:: docs/figs/nouns.png
-.. |adjs| image:: docs/figs/adjectives.png
-.. |doclen| image:: docs/figs/doclen.png
-.. |wordszipf| image:: docs/figs/wordszipf.png
-.. |labels| image:: docs/figs/labels.png
 .. |cover| image:: docs/figs/abstract_cover_2.png
 .. |clustering_cover| image:: docs/figs/clustering_cover.png
 .. |text_analysis_cover| image:: docs/figs/text_analysis.png
```

