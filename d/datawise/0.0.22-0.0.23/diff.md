# Comparing `tmp/datawise-0.0.22.tar.gz` & `tmp/datawise-0.0.23.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "datawise-0.0.22.tar", max compression
+gzip compressed data, was "datawise-0.0.23.tar", max compression
```

## Comparing `datawise-0.0.22.tar` & `datawise-0.0.23.tar`

### file list

```diff
@@ -1,6 +1,6 @@
--rw-r--r--   0        0        0    11357 2023-06-16 12:22:48.812559 datawise-0.0.22/LICENSE
--rw-r--r--   0        0        0     6750 2023-06-24 02:47:18.454410 datawise-0.0.22/README.md
--rw-r--r--   0        0        0     8384 2023-06-25 19:37:03.295583 datawise-0.0.22/datawise/__init__.py
--rw-r--r--   0        0        0      704 2023-06-25 18:46:09.256341 datawise-0.0.22/datawise/exceptions.py
--rw-r--r--   0        0        0      589 2023-06-25 19:40:35.826780 datawise-0.0.22/pyproject.toml
--rw-r--r--   0        0        0     7308 1970-01-01 00:00:00.000000 datawise-0.0.22/PKG-INFO
+-rw-r--r--   0        0        0    11357 2023-06-16 12:22:48.812559 datawise-0.0.23/LICENSE
+-rw-r--r--   0        0        0     6743 2023-06-26 11:47:04.978091 datawise-0.0.23/README.md
+-rw-r--r--   0        0        0     8384 2023-06-26 11:46:11.563716 datawise-0.0.23/datawise/__init__.py
+-rw-r--r--   0        0        0      704 2023-06-25 18:46:09.256341 datawise-0.0.23/datawise/exceptions.py
+-rw-r--r--   0        0        0      589 2023-06-26 11:43:04.654914 datawise-0.0.23/pyproject.toml
+-rw-r--r--   0        0        0     7301 1970-01-01 00:00:00.000000 datawise-0.0.23/PKG-INFO
```

### Comparing `datawise-0.0.22/LICENSE` & `datawise-0.0.23/LICENSE`

 * *Files identical despite different names*

### Comparing `datawise-0.0.22/README.md` & `datawise-0.0.23/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 
 ### AI Assistant for Python Data Analytics
 | Capabilities                                      | Limitations                                 |
 |---------------------------------------------------|---------------------------------------------|
 | Use SQL to transform Pandas dataframes            | May occasionally generate incorrect results |
 | Use English to visualize Pandas dataframes (beta) |                                             |
 
-[Get your API Key](https://datawise.vercel.app/)
+[Get your API Key](https://wisedata.app/)
 
 ## 🔍 Demo
 Try out DataWise in your browser:
 
 [![Open in Colab](https://camo.githubusercontent.com/84f0493939e0c4de4e6dbe113251b4bfb5353e57134ffd9fcab6b8714514d4d1/68747470733a2f2f636f6c61622e72657365617263682e676f6f676c652e636f6d2f6173736574732f636f6c61622d62616467652e737667)](https://colab.research.google.com/drive/1onQI_V6NrAnEDY-o6N068xLyvsFojynf?usp=sharing)
 
 ## 🔧 Quick install
```

### Comparing `datawise-0.0.22/datawise/__init__.py` & `datawise-0.0.23/datawise/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -9,15 +9,15 @@
 from retry import retry
 
 
 class DataWise:
   """Creates a new DataWise API client."""
   def __init__(
     self, 
-    api_base="https://datawise.vercel.app/api",
+    api_base="https://wisedata.vercel.app/api",
     api_key=None
   ):
     load_dotenv()
     self.api_base = api_base if api_base else os.getenv("DATAWISE_API_BASE")
     self.api_key = api_key if api_key else os.getenv("DATAWISE_API_KEY")
   
   def sql(self, query, dataframes, code=False):
```

### Comparing `datawise-0.0.22/datawise/exceptions.py` & `datawise-0.0.23/datawise/exceptions.py`

 * *Files identical despite different names*

### Comparing `datawise-0.0.22/pyproject.toml` & `datawise-0.0.23/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "datawise"
-version = "0.0.22"
+version = "0.0.23"
 description = "AI Assistant for Python Data Analytics"
 authors = ["DataWise Team"]
 readme = "README.md"
 
 [tool.poetry.dependencies]
 python = "^3.9.0"
 python-dotenv = "^1.0.0"
```

### Comparing `datawise-0.0.22/PKG-INFO` & `datawise-0.0.23/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: datawise
-Version: 0.0.22
+Version: 0.0.23
 Summary: AI Assistant for Python Data Analytics
 Author: DataWise Team
 Requires-Python: >=3.9.0,<4.0.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
@@ -18,15 +18,15 @@
 
 ### AI Assistant for Python Data Analytics
 | Capabilities                                      | Limitations                                 |
 |---------------------------------------------------|---------------------------------------------|
 | Use SQL to transform Pandas dataframes            | May occasionally generate incorrect results |
 | Use English to visualize Pandas dataframes (beta) |                                             |
 
-[Get your API Key](https://datawise.vercel.app/)
+[Get your API Key](https://wisedata.app/)
 
 ## 🔍 Demo
 Try out DataWise in your browser:
 
 [![Open in Colab](https://camo.githubusercontent.com/84f0493939e0c4de4e6dbe113251b4bfb5353e57134ffd9fcab6b8714514d4d1/68747470733a2f2f636f6c61622e72657365617263682e676f6f676c652e636f6d2f6173736574732f636f6c61622d62616467652e737667)](https://colab.research.google.com/drive/1onQI_V6NrAnEDY-o6N068xLyvsFojynf?usp=sharing)
 
 ## 🔧 Quick install
```

