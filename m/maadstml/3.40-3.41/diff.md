# Comparing `tmp/maadstml-3.40.tar.gz` & `tmp/maadstml-3.41.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "maadstml-3.40.tar", last modified: Sat Jun 24 19:41:00 2023, max compression
+gzip compressed data, was "maadstml-3.41.tar", last modified: Mon Jun 26 14:44:40 2023, max compression
```

## Comparing `maadstml-3.40.tar` & `maadstml-3.41.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxrwxrwx   0        0        0        0 2023-06-24 19:41:00.530276 maadstml-3.40/
--rw-rw-rw-   0        0        0      852 2020-02-09 18:05:54.000000 maadstml-3.40/LICENSE.txt
--rw-rw-rw-   0        0        0       65 2021-01-25 23:03:44.000000 maadstml-3.40/MANIFEST.in
--rw-rw-rw-   0        0        0   173475 2023-06-24 19:41:00.530276 maadstml-3.40/PKG-INFO
--rw-rw-rw-   0        0        0   172878 2023-06-24 19:39:52.000000 maadstml-3.40/README.md
-drwxrwxrwx   0        0        0        0 2023-06-24 19:41:00.502869 maadstml-3.40/maadstml/
--rw-rw-rw-   0        0        0     2260 2023-06-24 18:40:37.000000 maadstml-3.40/maadstml/__init__.py
--rw-rw-rw-   0        0        0     4871 2023-06-10 19:44:05.000000 maadstml-3.40/maadstml/readpdf.py
--rw-rw-rw-   0        0        0    81197 2023-06-24 18:12:26.000000 maadstml-3.40/maadstml/sendfiles.py
--rw-rw-rw-   0        0        0    10850 2023-06-10 19:08:28.000000 maadstml-3.40/maadstml/tmltextsummary.py
-drwxrwxrwx   0        0        0        0 2023-06-24 19:41:00.522427 maadstml-3.40/maadstml.egg-info/
--rw-rw-rw-   0        0        0   173475 2023-06-24 19:41:00.000000 maadstml-3.40/maadstml.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      320 2023-06-24 19:41:00.000000 maadstml-3.40/maadstml.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-24 19:41:00.000000 maadstml-3.40/maadstml.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      189 2023-06-24 19:41:00.000000 maadstml-3.40/maadstml.egg-info/requires.txt
--rw-rw-rw-   0        0        0        9 2023-06-24 19:41:00.000000 maadstml-3.40/maadstml.egg-info/top_level.txt
--rw-rw-rw-   0        0        0      204 2023-06-24 18:15:22.000000 maadstml-3.40/requirements.txt
--rw-rw-rw-   0        0        0       42 2023-06-24 19:41:00.530276 maadstml-3.40/setup.cfg
--rw-rw-rw-   0        0        0     1088 2023-06-24 19:40:15.000000 maadstml-3.40/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-26 14:44:40.690343 maadstml-3.41/
+-rw-rw-rw-   0        0        0      852 2020-02-09 18:05:54.000000 maadstml-3.41/LICENSE.txt
+-rw-rw-rw-   0        0        0       65 2021-01-25 23:03:44.000000 maadstml-3.41/MANIFEST.in
+-rw-rw-rw-   0        0        0   173465 2023-06-26 14:44:40.690343 maadstml-3.41/PKG-INFO
+-rw-rw-rw-   0        0        0   172868 2023-06-26 14:42:26.000000 maadstml-3.41/README.md
+drwxrwxrwx   0        0        0        0 2023-06-26 14:44:40.659860 maadstml-3.41/maadstml/
+-rw-rw-rw-   0        0        0     2260 2023-06-24 18:40:37.000000 maadstml-3.41/maadstml/__init__.py
+-rw-rw-rw-   0        0        0     4871 2023-06-10 19:44:05.000000 maadstml-3.41/maadstml/readpdf.py
+-rw-rw-rw-   0        0        0    81197 2023-06-24 18:12:26.000000 maadstml-3.41/maadstml/sendfiles.py
+-rw-rw-rw-   0        0        0    10850 2023-06-10 19:08:28.000000 maadstml-3.41/maadstml/tmltextsummary.py
+drwxrwxrwx   0        0        0        0 2023-06-26 14:44:40.688118 maadstml-3.41/maadstml.egg-info/
+-rw-rw-rw-   0        0        0   173465 2023-06-26 14:44:40.000000 maadstml-3.41/maadstml.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      320 2023-06-26 14:44:40.000000 maadstml-3.41/maadstml.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-26 14:44:40.000000 maadstml-3.41/maadstml.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      189 2023-06-26 14:44:40.000000 maadstml-3.41/maadstml.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        9 2023-06-26 14:44:40.000000 maadstml-3.41/maadstml.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0      204 2023-06-24 18:15:22.000000 maadstml-3.41/requirements.txt
+-rw-rw-rw-   0        0        0       42 2023-06-26 14:44:40.690343 maadstml-3.41/setup.cfg
+-rw-rw-rw-   0        0        0     1088 2023-06-26 14:43:30.000000 maadstml-3.41/setup.py
```

### Comparing `maadstml-3.40/LICENSE.txt` & `maadstml-3.41/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `maadstml-3.40/PKG-INFO` & `maadstml-3.41/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: maadstml
-Version: 3.40
+Version: 3.41
 Summary: Multi-Agent Accelerator for Data Science (MAADS): Transactional Machine Learning
 Home-page: https://github.com/smaurice101/transactionalmachinelearning
 Author: Sebastian Maurice
 Author-email: sebastian.maurice@otics.ca
 License: MIT License
 Keywords: multi-agent, transactional machine learning, data streams, data science, optimization, prescriptive analytics, machine learning, automl,auto-ml,artificial intelligence,predictive analytics,advanced analytics
 Description-Content-Type: text/markdown
@@ -4560,25 +4560,25 @@
 
 - ChatGPT model to use.  For example, text-davinci-002, text-curie-001, text-babbage-001.
 
 RETURNS: ChatGPT response.
 
 **38. maadstml.viperexractpdffields(pdffilename)**
 
-**Parameters:**	Start a conversation with ChatGPT
+**Parameters:**	Extract data from PDF
 
 *pdffilename* : string, required
 
 - PDF filename
 
 RETURNS: JSON of PDF and writes JSON and XML files of PDF to disk.
 
 **39. maadstml.viperexractpdffieldbylabel(pdffilename,labelname,arcotype)**
 
-**Parameters:**	Start a conversation with ChatGPT
+**Parameters:**	Extract data from PDF by PDF labels
 
 *pdffilename* : string, required
 
 - PDF filename
 
 *labelname* : string, required
```

### Comparing `maadstml-3.40/README.md` & `maadstml-3.41/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -4548,25 +4548,25 @@
 
 - ChatGPT model to use.  For example, text-davinci-002, text-curie-001, text-babbage-001.
 
 RETURNS: ChatGPT response.
 
 **38. maadstml.viperexractpdffields(pdffilename)**
 
-**Parameters:**	Start a conversation with ChatGPT
+**Parameters:**	Extract data from PDF
 
 *pdffilename* : string, required
 
 - PDF filename
 
 RETURNS: JSON of PDF and writes JSON and XML files of PDF to disk.
 
 **39. maadstml.viperexractpdffieldbylabel(pdffilename,labelname,arcotype)**
 
-**Parameters:**	Start a conversation with ChatGPT
+**Parameters:**	Extract data from PDF by PDF labels
 
 *pdffilename* : string, required
 
 - PDF filename
 
 *labelname* : string, required
```

### Comparing `maadstml-3.40/maadstml/__init__.py` & `maadstml-3.41/maadstml/__init__.py`

 * *Files identical despite different names*

### Comparing `maadstml-3.40/maadstml/readpdf.py` & `maadstml-3.41/maadstml/readpdf.py`

 * *Files identical despite different names*

### Comparing `maadstml-3.40/maadstml/sendfiles.py` & `maadstml-3.41/maadstml/sendfiles.py`

 * *Files identical despite different names*

### Comparing `maadstml-3.40/maadstml/tmltextsummary.py` & `maadstml-3.41/maadstml/tmltextsummary.py`

 * *Files identical despite different names*

### Comparing `maadstml-3.40/maadstml.egg-info/PKG-INFO` & `maadstml-3.41/maadstml.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: maadstml
-Version: 3.40
+Version: 3.41
 Summary: Multi-Agent Accelerator for Data Science (MAADS): Transactional Machine Learning
 Home-page: https://github.com/smaurice101/transactionalmachinelearning
 Author: Sebastian Maurice
 Author-email: sebastian.maurice@otics.ca
 License: MIT License
 Keywords: multi-agent, transactional machine learning, data streams, data science, optimization, prescriptive analytics, machine learning, automl,auto-ml,artificial intelligence,predictive analytics,advanced analytics
 Description-Content-Type: text/markdown
@@ -4560,25 +4560,25 @@
 
 - ChatGPT model to use.  For example, text-davinci-002, text-curie-001, text-babbage-001.
 
 RETURNS: ChatGPT response.
 
 **38. maadstml.viperexractpdffields(pdffilename)**
 
-**Parameters:**	Start a conversation with ChatGPT
+**Parameters:**	Extract data from PDF
 
 *pdffilename* : string, required
 
 - PDF filename
 
 RETURNS: JSON of PDF and writes JSON and XML files of PDF to disk.
 
 **39. maadstml.viperexractpdffieldbylabel(pdffilename,labelname,arcotype)**
 
-**Parameters:**	Start a conversation with ChatGPT
+**Parameters:**	Extract data from PDF by PDF labels
 
 *pdffilename* : string, required
 
 - PDF filename
 
 *labelname* : string, required
```

### Comparing `maadstml-3.40/setup.py` & `maadstml-3.41/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -10,15 +10,15 @@
 	
 
 with open("requirements.txt","r") as f:
     required = f.read().splitlines()
     
 setuptools.setup(
     name='maadstml',
-    version='3.40',
+    version='3.41',
     description='Multi-Agent Accelerator for Data Science (MAADS): Transactional Machine Learning',
     license='MIT License',
     packages=['maadstml'],
     author='Sebastian Maurice',
     author_email='sebastian.maurice@otics.ca',
     keywords=['multi-agent, transactional machine learning, data streams, data science, optimization, prescriptive analytics, machine learning, automl,auto-ml,artificial intelligence', 'predictive analytics', 'advanced analytics'],
     long_description=long_description,
```

