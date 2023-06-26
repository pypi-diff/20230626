# Comparing `tmp/Kanon4txt-0.0.3.tar.gz` & `tmp/Kanon4txt-0.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "Kanon4txt-0.0.3.tar", last modified: Mon Jun 26 09:55:03 2023, max compression
+gzip compressed data, was "Kanon4txt-0.0.4.tar", last modified: Mon Jun 26 10:14:01 2023, max compression
```

## Comparing `Kanon4txt-0.0.3.tar` & `Kanon4txt-0.0.4.tar`

### file list

```diff
@@ -1,23 +1,23 @@
-drwxrwxrwx   0        0        0        0 2023-06-26 09:55:03.290106 Kanon4txt-0.0.3/
-drwxrwxrwx   0        0        0        0 2023-06-26 09:55:03.238110 Kanon4txt-0.0.3/Kanon4txt/
--rw-rw-rw-   0        0        0        0 2023-06-06 19:44:31.000000 Kanon4txt-0.0.3/Kanon4txt/__init__.py
--rw-rw-rw-   0        0        0     8955 2023-06-26 09:51:20.000000 Kanon4txt-0.0.3/Kanon4txt/k_anonym_text.py
-drwxrwxrwx   0        0        0        0 2023-06-26 09:55:03.288134 Kanon4txt-0.0.3/Kanon4txt/utils/
--rw-rw-rw-   0        0        0        0 2023-04-27 08:18:12.000000 Kanon4txt-0.0.3/Kanon4txt/utils/__init__.py
--rw-rw-rw-   0        0        0    19915 2023-06-19 08:12:01.000000 Kanon4txt-0.0.3/Kanon4txt/utils/anonym_utils.py
--rw-rw-rw-   0        0        0    13766 2023-06-19 08:12:01.000000 Kanon4txt-0.0.3/Kanon4txt/utils/cluster_utils.py
--rw-rw-rw-   0        0        0     7107 2023-06-19 08:12:01.000000 Kanon4txt-0.0.3/Kanon4txt/utils/llm_utils.py
--rw-rw-rw-   0        0        0      485 2023-06-19 08:12:01.000000 Kanon4txt-0.0.3/Kanon4txt/utils/models.py
--rw-rw-rw-   0        0        0    13040 2023-06-19 08:12:01.000000 Kanon4txt-0.0.3/Kanon4txt/utils/nlp_utils.py
--rw-rw-rw-   0        0        0     6458 2023-06-19 08:12:01.000000 Kanon4txt-0.0.3/Kanon4txt/utils/utilization_utils.py
-drwxrwxrwx   0        0        0        0 2023-06-26 09:55:03.272107 Kanon4txt-0.0.3/Kanon4txt.egg-info/
--rw-rw-rw-   0        0        0      724 2023-06-26 09:55:03.000000 Kanon4txt-0.0.3/Kanon4txt.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      463 2023-06-26 09:55:03.000000 Kanon4txt-0.0.3/Kanon4txt.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-26 09:55:03.000000 Kanon4txt-0.0.3/Kanon4txt.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      142 2023-06-26 09:55:03.000000 Kanon4txt-0.0.3/Kanon4txt.egg-info/requires.txt
--rw-rw-rw-   0        0        0       10 2023-06-26 09:55:03.000000 Kanon4txt-0.0.3/Kanon4txt.egg-info/top_level.txt
--rw-rw-rw-   0        0        0     1091 2023-06-06 20:01:19.000000 Kanon4txt-0.0.3/LICENSE
--rw-rw-rw-   0        0        0      724 2023-06-26 09:55:03.291108 Kanon4txt-0.0.3/PKG-INFO
--rw-rw-rw-   0        0        0     4499 2023-06-21 09:41:31.000000 Kanon4txt-0.0.3/README.md
--rw-rw-rw-   0        0        0       86 2023-06-26 09:55:03.299105 Kanon4txt-0.0.3/setup.cfg
--rw-rw-rw-   0        0        0     1407 2023-06-26 09:54:03.000000 Kanon4txt-0.0.3/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-26 10:14:01.706119 Kanon4txt-0.0.4/
+drwxrwxrwx   0        0        0        0 2023-06-26 10:14:01.658518 Kanon4txt-0.0.4/Kanon4txt/
+-rw-rw-rw-   0        0        0        0 2023-06-06 19:44:31.000000 Kanon4txt-0.0.4/Kanon4txt/__init__.py
+-rw-rw-rw-   0        0        0     8955 2023-06-26 09:51:20.000000 Kanon4txt-0.0.4/Kanon4txt/k_anonym_text.py
+drwxrwxrwx   0        0        0        0 2023-06-26 10:14:01.703960 Kanon4txt-0.0.4/Kanon4txt/utils/
+-rw-rw-rw-   0        0        0       73 2023-06-26 10:11:38.000000 Kanon4txt-0.0.4/Kanon4txt/utils/__init__.py
+-rw-rw-rw-   0        0        0    19915 2023-06-19 08:12:01.000000 Kanon4txt-0.0.4/Kanon4txt/utils/anonym_utils.py
+-rw-rw-rw-   0        0        0    13766 2023-06-19 08:12:01.000000 Kanon4txt-0.0.4/Kanon4txt/utils/cluster_utils.py
+-rw-rw-rw-   0        0        0     7107 2023-06-19 08:12:01.000000 Kanon4txt-0.0.4/Kanon4txt/utils/llm_utils.py
+-rw-rw-rw-   0        0        0      485 2023-06-19 08:12:01.000000 Kanon4txt-0.0.4/Kanon4txt/utils/models.py
+-rw-rw-rw-   0        0        0    13040 2023-06-19 08:12:01.000000 Kanon4txt-0.0.4/Kanon4txt/utils/nlp_utils.py
+-rw-rw-rw-   0        0        0     6458 2023-06-19 08:12:01.000000 Kanon4txt-0.0.4/Kanon4txt/utils/utilization_utils.py
+drwxrwxrwx   0        0        0        0 2023-06-26 10:14:01.683235 Kanon4txt-0.0.4/Kanon4txt.egg-info/
+-rw-rw-rw-   0        0        0      724 2023-06-26 10:14:01.000000 Kanon4txt-0.0.4/Kanon4txt.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      463 2023-06-26 10:14:01.000000 Kanon4txt-0.0.4/Kanon4txt.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-26 10:14:01.000000 Kanon4txt-0.0.4/Kanon4txt.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      142 2023-06-26 10:14:01.000000 Kanon4txt-0.0.4/Kanon4txt.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       10 2023-06-26 10:14:01.000000 Kanon4txt-0.0.4/Kanon4txt.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0     1091 2023-06-06 20:01:19.000000 Kanon4txt-0.0.4/LICENSE
+-rw-rw-rw-   0        0        0      724 2023-06-26 10:14:01.706119 Kanon4txt-0.0.4/PKG-INFO
+-rw-rw-rw-   0        0        0     4499 2023-06-21 09:41:31.000000 Kanon4txt-0.0.4/README.md
+-rw-rw-rw-   0        0        0       86 2023-06-26 10:14:01.708120 Kanon4txt-0.0.4/setup.cfg
+-rw-rw-rw-   0        0        0     1407 2023-06-26 10:13:45.000000 Kanon4txt-0.0.4/setup.py
```

### Comparing `Kanon4txt-0.0.3/Kanon4txt/k_anonym_text.py` & `Kanon4txt-0.0.4/Kanon4txt/k_anonym_text.py`

 * *Files identical despite different names*

### Comparing `Kanon4txt-0.0.3/Kanon4txt/utils/anonym_utils.py` & `Kanon4txt-0.0.4/Kanon4txt/utils/anonym_utils.py`

 * *Files identical despite different names*

### Comparing `Kanon4txt-0.0.3/Kanon4txt/utils/cluster_utils.py` & `Kanon4txt-0.0.4/Kanon4txt/utils/cluster_utils.py`

 * *Files identical despite different names*

### Comparing `Kanon4txt-0.0.3/Kanon4txt/utils/llm_utils.py` & `Kanon4txt-0.0.4/Kanon4txt/utils/llm_utils.py`

 * *Files identical despite different names*

### Comparing `Kanon4txt-0.0.3/Kanon4txt/utils/nlp_utils.py` & `Kanon4txt-0.0.4/Kanon4txt/utils/nlp_utils.py`

 * *Files identical despite different names*

### Comparing `Kanon4txt-0.0.3/Kanon4txt/utils/utilization_utils.py` & `Kanon4txt-0.0.4/Kanon4txt/utils/utilization_utils.py`

 * *Files identical despite different names*

### Comparing `Kanon4txt-0.0.3/Kanon4txt.egg-info/PKG-INFO` & `Kanon4txt-0.0.4/Kanon4txt.egg-info/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 Metadata-Version: 2.1
 Name: Kanon4txt
-Version: 0.0.3
+Version: 0.0.4
 Summary: K Anonymity for Text first Try
 Home-page: https://github.com/LiorTrieman/Kanon4txt/tree/maine
-Download-URL: https://github.com/LiorTrieman/Kanon4txt/archive/refs/tags/0.0.3.tar.gz
+Download-URL: https://github.com/LiorTrieman/Kanon4txt/archive/refs/tags/0.0.4.tar.gz
 Author: Lior Trieman
 Author-email: <liortr30@gmail.com>
 License: MIT
 Keywords: python,corpus,stopwords,DBSCAN,generalization,reduction
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `Kanon4txt-0.0.3/LICENSE` & `Kanon4txt-0.0.4/LICENSE`

 * *Files identical despite different names*

### Comparing `Kanon4txt-0.0.3/PKG-INFO` & `Kanon4txt-0.0.4/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 Metadata-Version: 2.1
 Name: Kanon4txt
-Version: 0.0.3
+Version: 0.0.4
 Summary: K Anonymity for Text first Try
 Home-page: https://github.com/LiorTrieman/Kanon4txt/tree/maine
-Download-URL: https://github.com/LiorTrieman/Kanon4txt/archive/refs/tags/0.0.3.tar.gz
+Download-URL: https://github.com/LiorTrieman/Kanon4txt/archive/refs/tags/0.0.4.tar.gz
 Author: Lior Trieman
 Author-email: <liortr30@gmail.com>
 License: MIT
 Keywords: python,corpus,stopwords,DBSCAN,generalization,reduction
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `Kanon4txt-0.0.3/README.md` & `Kanon4txt-0.0.4/README.md`

 * *Files identical despite different names*

### Comparing `Kanon4txt-0.0.3/setup.py` & `Kanon4txt-0.0.4/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,22 +1,22 @@
 
 from setuptools import setup, find_packages
 
-VERSION = '0.0.3'
+VERSION = '0.0.4'
 DESCRIPTION = 'K Anonymity for Text first Try'
 LONG_DESCRIPTION = 'A package that takes a dataframe with a corpus and return an anonymized corpus'
 
 # Setting up
 setup(
     name="Kanon4txt",
     version=VERSION,
     author="Lior Trieman",
     author_email="<liortr30@gmail.com>",
     url='https://github.com/LiorTrieman/Kanon4txt/tree/maine',
-    download_url='https://github.com/LiorTrieman/Kanon4txt/archive/refs/tags/0.0.3.tar.gz',  # I explain this later on
+    download_url='https://github.com/LiorTrieman/Kanon4txt/archive/refs/tags/0.0.4.tar.gz',  # I explain this later on
 
     license='MIT',
     description=DESCRIPTION,
     long_description_content_type="text/markdown",
     long_description=LONG_DESCRIPTION,
     packages=find_packages(),
     # NEED TO ADD HERE ALL REQUIREMENTS!!!!!
```

