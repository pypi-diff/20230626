# Comparing `tmp/GPTConnect-0.2.4.tar.gz` & `tmp/GPTConnect-0.2.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "GPTConnect-0.2.4.tar", last modified: Mon Jun 26 05:16:54 2023, max compression
+gzip compressed data, was "GPTConnect-0.2.5.tar", last modified: Mon Jun 26 05:24:51 2023, max compression
```

## Comparing `GPTConnect-0.2.4.tar` & `GPTConnect-0.2.5.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxrwxrwx   0        0        0        0 2023-06-26 05:16:54.134539 GPTConnect-0.2.4/
-drwxrwxrwx   0        0        0        0 2023-06-26 05:16:54.121516 GPTConnect-0.2.4/GPTConnect.egg-info/
--rw-rw-rw-   0        0        0     1380 2023-06-26 05:16:53.000000 GPTConnect-0.2.4/GPTConnect.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      328 2023-06-26 05:16:54.000000 GPTConnect-0.2.4/GPTConnect.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-26 05:16:53.000000 GPTConnect-0.2.4/GPTConnect.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        7 2023-06-26 05:16:53.000000 GPTConnect-0.2.4/GPTConnect.egg-info/requires.txt
--rw-rw-rw-   0        0        0       11 2023-06-26 05:16:53.000000 GPTConnect-0.2.4/GPTConnect.egg-info/top_level.txt
--rw-rw-rw-   0        0        0    11558 2023-06-25 05:39:53.000000 GPTConnect-0.2.4/LICENSE
--rw-rw-rw-   0        0        0     1380 2023-06-26 05:16:54.134539 GPTConnect-0.2.4/PKG-INFO
--rw-rw-rw-   0        0        0     1150 2023-06-26 05:06:39.000000 GPTConnect-0.2.4/README.md
-drwxrwxrwx   0        0        0        0 2023-06-26 05:16:54.131541 GPTConnect-0.2.4/gptconnect/
--rw-rw-rw-   0        0        0      118 2023-06-26 04:19:52.000000 GPTConnect-0.2.4/gptconnect/__init__.py
--rw-rw-rw-   0        0        0      728 2023-06-26 05:05:04.000000 GPTConnect-0.2.4/gptconnect/dataclasses.py
--rw-rw-rw-   0        0        0     2830 2023-06-26 04:57:37.000000 GPTConnect-0.2.4/gptconnect/gptconnect.py
--rw-rw-rw-   0        0        0      994 2023-06-26 05:12:47.000000 GPTConnect-0.2.4/gptconnect/gptfunction.py
--rw-rw-rw-   0        0        0      382 2023-06-25 06:33:58.000000 GPTConnect-0.2.4/gptconnect/gptfunctionhandler.py
--rw-rw-rw-   0        0        0       42 2023-06-26 05:16:54.135533 GPTConnect-0.2.4/setup.cfg
--rw-rw-rw-   0        0        0      391 2023-06-26 05:16:42.000000 GPTConnect-0.2.4/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-26 05:24:51.215359 GPTConnect-0.2.5/
+drwxrwxrwx   0        0        0        0 2023-06-26 05:24:51.202464 GPTConnect-0.2.5/GPTConnect.egg-info/
+-rw-rw-rw-   0        0        0     1380 2023-06-26 05:24:51.000000 GPTConnect-0.2.5/GPTConnect.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      328 2023-06-26 05:24:51.000000 GPTConnect-0.2.5/GPTConnect.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-26 05:24:51.000000 GPTConnect-0.2.5/GPTConnect.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        7 2023-06-26 05:24:51.000000 GPTConnect-0.2.5/GPTConnect.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       11 2023-06-26 05:24:51.000000 GPTConnect-0.2.5/GPTConnect.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0    11558 2023-06-25 05:39:53.000000 GPTConnect-0.2.5/LICENSE
+-rw-rw-rw-   0        0        0     1380 2023-06-26 05:24:51.214358 GPTConnect-0.2.5/PKG-INFO
+-rw-rw-rw-   0        0        0     1150 2023-06-26 05:06:39.000000 GPTConnect-0.2.5/README.md
+drwxrwxrwx   0        0        0        0 2023-06-26 05:24:51.212359 GPTConnect-0.2.5/gptconnect/
+-rw-rw-rw-   0        0        0      118 2023-06-26 04:19:52.000000 GPTConnect-0.2.5/gptconnect/__init__.py
+-rw-rw-rw-   0        0        0      739 2023-06-26 05:23:53.000000 GPTConnect-0.2.5/gptconnect/dataclasses.py
+-rw-rw-rw-   0        0        0     2830 2023-06-26 05:21:03.000000 GPTConnect-0.2.5/gptconnect/gptconnect.py
+-rw-rw-rw-   0        0        0      994 2023-06-26 05:12:47.000000 GPTConnect-0.2.5/gptconnect/gptfunction.py
+-rw-rw-rw-   0        0        0      382 2023-06-25 06:33:58.000000 GPTConnect-0.2.5/gptconnect/gptfunctionhandler.py
+-rw-rw-rw-   0        0        0       42 2023-06-26 05:24:51.215359 GPTConnect-0.2.5/setup.cfg
+-rw-rw-rw-   0        0        0      391 2023-06-26 05:24:39.000000 GPTConnect-0.2.5/setup.py
```

### Comparing `GPTConnect-0.2.4/GPTConnect.egg-info/PKG-INFO` & `GPTConnect-0.2.5/GPTConnect.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: GPTConnect
-Version: 0.2.4
+Version: 0.2.5
 Summary: A python package to make GPT functions easy
 Home-page: https://github.com/SleepyStew/gptconnect
 Author: SleepyStew
 License: Apache 2.0
 License-File: LICENSE
 
 # GPTConnect
```

### Comparing `GPTConnect-0.2.4/LICENSE` & `GPTConnect-0.2.5/LICENSE`

 * *Files identical despite different names*

### Comparing `GPTConnect-0.2.4/PKG-INFO` & `GPTConnect-0.2.5/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: GPTConnect
-Version: 0.2.4
+Version: 0.2.5
 Summary: A python package to make GPT functions easy
 Home-page: https://github.com/SleepyStew/gptconnect
 Author: SleepyStew
 License: Apache 2.0
 License-File: LICENSE
 
 # GPTConnect
```

### Comparing `GPTConnect-0.2.4/README.md` & `GPTConnect-0.2.5/README.md`

 * *Files identical despite different names*

### Comparing `GPTConnect-0.2.4/gptconnect/dataclasses.py` & `GPTConnect-0.2.5/gptconnect/dataclasses.py`

 * *Files 7% similar despite different names*

```diff
@@ -14,24 +14,23 @@
 
 @dataclass
 class Property:
     type: type
     description: str
     enum: list = None
 
-    def __post_init__(self):
-        if not self.enum:
-            self.enum = []
-
 
 @dataclass
 class Params:
     properties: dict
     required: list
 
     def properties_dict(self):
         _properties = {}
         for key, value in self.properties.items():
             _properties[key] = value.__dict__
             _properties[key]["type"] = types_lookup[_properties[key]["type"]]
+            if not _properties[key].get("enum"):
+                del _properties[key]["enum"]
+
         return _properties
```

### Comparing `GPTConnect-0.2.4/gptconnect/gptconnect.py` & `GPTConnect-0.2.5/gptconnect/gptconnect.py`

 * *Files identical despite different names*

### Comparing `GPTConnect-0.2.4/gptconnect/gptfunction.py` & `GPTConnect-0.2.5/gptconnect/gptfunction.py`

 * *Files identical despite different names*

