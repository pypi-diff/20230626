# Comparing `tmp/wisedata-1.0.0.tar.gz` & `tmp/wisedata-1.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "wisedata-1.0.0.tar", max compression
+gzip compressed data, was "wisedata-1.0.1.tar", max compression
```

## Comparing `wisedata-1.0.0.tar` & `wisedata-1.0.1.tar`

### file list

```diff
@@ -1,6 +1,6 @@
--rw-r--r--   0        0        0    11357 2023-06-16 12:22:48.812559 wisedata-1.0.0/LICENSE
--rw-r--r--   0        0        0     6743 2023-06-26 12:19:58.647123 wisedata-1.0.0/README.md
--rw-r--r--   0        0        0      588 2023-06-26 12:13:54.231183 wisedata-1.0.0/pyproject.toml
--rw-r--r--   0        0        0     8384 2023-06-26 12:19:30.469356 wisedata-1.0.0/wisedata/__init__.py
--rw-r--r--   0        0        0      704 2023-06-26 12:18:32.144558 wisedata-1.0.0/wisedata/exceptions.py
--rw-r--r--   0        0        0     7300 1970-01-01 00:00:00.000000 wisedata-1.0.0/PKG-INFO
+-rw-r--r--   0        0        0    11357 2023-06-16 12:22:48.812559 wisedata-1.0.1/LICENSE
+-rw-r--r--   0        0        0     6743 2023-06-26 13:59:59.003655 wisedata-1.0.1/README.md
+-rw-r--r--   0        0        0      588 2023-06-26 14:00:27.109458 wisedata-1.0.1/pyproject.toml
+-rw-r--r--   0        0        0     8384 2023-06-26 12:19:30.469356 wisedata-1.0.1/wisedata/__init__.py
+-rw-r--r--   0        0        0      704 2023-06-26 12:18:32.144558 wisedata-1.0.1/wisedata/exceptions.py
+-rw-r--r--   0        0        0     7300 1970-01-01 00:00:00.000000 wisedata-1.0.1/PKG-INFO
```

### Comparing `wisedata-1.0.0/LICENSE` & `wisedata-1.0.1/LICENSE`

 * *Files identical despite different names*

### Comparing `wisedata-1.0.0/README.md` & `wisedata-1.0.1/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -12,15 +12,15 @@
 Try out WiseData in your browser:
 
 [![Open in Colab](https://camo.githubusercontent.com/84f0493939e0c4de4e6dbe113251b4bfb5353e57134ffd9fcab6b8714514d4d1/68747470733a2f2f636f6c61622e72657365617263682e676f6f676c652e636f6d2f6173736574732f636f6c61622d62616467652e737667)](https://colab.research.google.com/drive/1onQI_V6NrAnEDY-o6N068xLyvsFojynf?usp=sharing)
 
 ## 🔧 Quick install
 Install WiseData client first:
 ```bash
-pip install WiseData
+pip install wisedata
 ```
 
 Configure with your account's API key.
 Either set it as `WISEDATA_API_KEY` environment variable before using the library:
 ```bash
 export WISEDATA_API_KEY=sk-...
 ```
```

### Comparing `wisedata-1.0.0/pyproject.toml` & `wisedata-1.0.1/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "wisedata"
-version = "1.0.0"
+version = "1.0.1"
 description = "AI Assistant for Python Data Analytics"
 authors = ["WiseData Team"]
 readme = "README.md"
 
 [tool.poetry.dependencies]
 python = "^3.9.0"
 python-dotenv = "^1.0.0"
```

### Comparing `wisedata-1.0.0/wisedata/__init__.py` & `wisedata-1.0.1/wisedata/__init__.py`

 * *Files identical despite different names*

### Comparing `wisedata-1.0.0/wisedata/exceptions.py` & `wisedata-1.0.1/wisedata/exceptions.py`

 * *Files identical despite different names*

### Comparing `wisedata-1.0.0/PKG-INFO` & `wisedata-1.0.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: wisedata
-Version: 1.0.0
+Version: 1.0.1
 Summary: AI Assistant for Python Data Analytics
 Author: WiseData Team
 Requires-Python: >=3.9.0,<4.0.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
@@ -28,15 +28,15 @@
 Try out WiseData in your browser:
 
 [![Open in Colab](https://camo.githubusercontent.com/84f0493939e0c4de4e6dbe113251b4bfb5353e57134ffd9fcab6b8714514d4d1/68747470733a2f2f636f6c61622e72657365617263682e676f6f676c652e636f6d2f6173736574732f636f6c61622d62616467652e737667)](https://colab.research.google.com/drive/1onQI_V6NrAnEDY-o6N068xLyvsFojynf?usp=sharing)
 
 ## 🔧 Quick install
 Install WiseData client first:
 ```bash
-pip install WiseData
+pip install wisedata
 ```
 
 Configure with your account's API key.
 Either set it as `WISEDATA_API_KEY` environment variable before using the library:
 ```bash
 export WISEDATA_API_KEY=sk-...
 ```
```

