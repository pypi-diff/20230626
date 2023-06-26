# Comparing `tmp/jinaai-0.1.2.tar.gz` & `tmp/jinaai-0.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "jinaai-0.1.2.tar", last modified: Wed Jun 21 05:46:03 2023, max compression
+gzip compressed data, was "jinaai-0.1.3.tar", last modified: Mon Jun 26 06:15:55 2023, max compression
```

## Comparing `jinaai-0.1.2.tar` & `jinaai-0.1.3.tar`

### file list

```diff
@@ -1,21 +1,21 @@
-drwxr-xr-x   0 guillaumeroncari   (501) staff       (20)        0 2023-06-21 05:46:03.427412 jinaai-0.1.2/
--rw-r--r--   0 guillaumeroncari   (501) staff       (20)    11358 2023-06-12 03:23:49.000000 jinaai-0.1.2/LICENSE
--rw-r--r--   0 guillaumeroncari   (501) staff       (20)    12903 2023-06-21 05:46:03.427099 jinaai-0.1.2/PKG-INFO
--rw-r--r--   0 guillaumeroncari   (501) staff       (20)    12653 2023-06-21 05:42:42.000000 jinaai-0.1.2/README.md
-drwxr-xr-x   0 guillaumeroncari   (501) staff       (20)        0 2023-06-21 05:46:03.424633 jinaai-0.1.2/jinaai/
--rw-r--r--   0 guillaumeroncari   (501) staff       (20)     2617 2023-06-20 03:59:26.000000 jinaai-0.1.2/jinaai/__init__.py
-drwxr-xr-x   0 guillaumeroncari   (501) staff       (20)        0 2023-06-21 05:46:03.426862 jinaai-0.1.2/jinaai/clients/
--rw-r--r--   0 guillaumeroncari   (501) staff       (20)     1809 2023-06-20 05:46:39.000000 jinaai-0.1.2/jinaai/clients/ChatCatClient.py
--rw-r--r--   0 guillaumeroncari   (501) staff       (20)     1082 2023-06-19 03:53:55.000000 jinaai-0.1.2/jinaai/clients/HTTPClient.py
--rw-r--r--   0 guillaumeroncari   (501) staff       (20)     2110 2023-06-19 04:25:56.000000 jinaai-0.1.2/jinaai/clients/PromptPerfectClient.py
--rw-r--r--   0 guillaumeroncari   (501) staff       (20)     1934 2023-06-19 08:21:16.000000 jinaai-0.1.2/jinaai/clients/RationaleClient.py
--rw-r--r--   0 guillaumeroncari   (501) staff       (20)     1686 2023-06-19 03:26:43.000000 jinaai-0.1.2/jinaai/clients/SceneXClient.py
--rw-r--r--   0 guillaumeroncari   (501) staff       (20)        0 2023-06-12 04:44:46.000000 jinaai-0.1.2/jinaai/clients/__init__.py
--rw-r--r--   0 guillaumeroncari   (501) staff       (20)      891 2023-06-16 08:41:29.000000 jinaai-0.1.2/jinaai/utils.py
-drwxr-xr-x   0 guillaumeroncari   (501) staff       (20)        0 2023-06-21 05:46:03.425289 jinaai-0.1.2/jinaai.egg-info/
--rw-r--r--   0 guillaumeroncari   (501) staff       (20)    12903 2023-06-21 05:46:03.000000 jinaai-0.1.2/jinaai.egg-info/PKG-INFO
--rw-r--r--   0 guillaumeroncari   (501) staff       (20)      372 2023-06-21 05:46:03.000000 jinaai-0.1.2/jinaai.egg-info/SOURCES.txt
--rw-r--r--   0 guillaumeroncari   (501) staff       (20)        1 2023-06-21 05:46:03.000000 jinaai-0.1.2/jinaai.egg-info/dependency_links.txt
--rw-r--r--   0 guillaumeroncari   (501) staff       (20)        7 2023-06-21 05:46:03.000000 jinaai-0.1.2/jinaai.egg-info/top_level.txt
--rw-r--r--   0 guillaumeroncari   (501) staff       (20)       38 2023-06-21 05:46:03.427460 jinaai-0.1.2/setup.cfg
--rw-r--r--   0 guillaumeroncari   (501) staff       (20)      483 2023-06-21 05:45:46.000000 jinaai-0.1.2/setup.py
+drwxr-xr-x   0 guillaumeroncari   (501) staff       (20)        0 2023-06-26 06:15:55.262952 jinaai-0.1.3/
+-rw-r--r--   0 guillaumeroncari   (501) staff       (20)    11358 2023-06-12 03:23:49.000000 jinaai-0.1.3/LICENSE
+-rw-r--r--   0 guillaumeroncari   (501) staff       (20)    12903 2023-06-26 06:15:55.262670 jinaai-0.1.3/PKG-INFO
+-rw-r--r--   0 guillaumeroncari   (501) staff       (20)    12653 2023-06-21 05:42:42.000000 jinaai-0.1.3/README.md
+drwxr-xr-x   0 guillaumeroncari   (501) staff       (20)        0 2023-06-26 06:15:55.260595 jinaai-0.1.3/jinaai/
+-rw-r--r--   0 guillaumeroncari   (501) staff       (20)     2617 2023-06-26 05:41:46.000000 jinaai-0.1.3/jinaai/__init__.py
+drwxr-xr-x   0 guillaumeroncari   (501) staff       (20)        0 2023-06-26 06:15:55.262505 jinaai-0.1.3/jinaai/clients/
+-rw-r--r--   0 guillaumeroncari   (501) staff       (20)     1866 2023-06-26 05:41:25.000000 jinaai-0.1.3/jinaai/clients/ChatCatClient.py
+-rw-r--r--   0 guillaumeroncari   (501) staff       (20)     1082 2023-06-19 03:53:55.000000 jinaai-0.1.3/jinaai/clients/HTTPClient.py
+-rw-r--r--   0 guillaumeroncari   (501) staff       (20)     2110 2023-06-19 04:25:56.000000 jinaai-0.1.3/jinaai/clients/PromptPerfectClient.py
+-rw-r--r--   0 guillaumeroncari   (501) staff       (20)     1934 2023-06-19 08:21:16.000000 jinaai-0.1.3/jinaai/clients/RationaleClient.py
+-rw-r--r--   0 guillaumeroncari   (501) staff       (20)     1686 2023-06-19 03:26:43.000000 jinaai-0.1.3/jinaai/clients/SceneXClient.py
+-rw-r--r--   0 guillaumeroncari   (501) staff       (20)        0 2023-06-12 04:44:46.000000 jinaai-0.1.3/jinaai/clients/__init__.py
+-rw-r--r--   0 guillaumeroncari   (501) staff       (20)      891 2023-06-16 08:41:29.000000 jinaai-0.1.3/jinaai/utils.py
+drwxr-xr-x   0 guillaumeroncari   (501) staff       (20)        0 2023-06-26 06:15:55.261208 jinaai-0.1.3/jinaai.egg-info/
+-rw-r--r--   0 guillaumeroncari   (501) staff       (20)    12903 2023-06-26 06:15:55.000000 jinaai-0.1.3/jinaai.egg-info/PKG-INFO
+-rw-r--r--   0 guillaumeroncari   (501) staff       (20)      372 2023-06-26 06:15:55.000000 jinaai-0.1.3/jinaai.egg-info/SOURCES.txt
+-rw-r--r--   0 guillaumeroncari   (501) staff       (20)        1 2023-06-26 06:15:55.000000 jinaai-0.1.3/jinaai.egg-info/dependency_links.txt
+-rw-r--r--   0 guillaumeroncari   (501) staff       (20)        7 2023-06-26 06:15:55.000000 jinaai-0.1.3/jinaai.egg-info/top_level.txt
+-rw-r--r--   0 guillaumeroncari   (501) staff       (20)       38 2023-06-26 06:15:55.262997 jinaai-0.1.3/setup.cfg
+-rw-r--r--   0 guillaumeroncari   (501) staff       (20)      483 2023-06-26 06:14:56.000000 jinaai-0.1.3/setup.py
```

### Comparing `jinaai-0.1.2/LICENSE` & `jinaai-0.1.3/LICENSE`

 * *Files identical despite different names*

### Comparing `jinaai-0.1.2/PKG-INFO` & `jinaai-0.1.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: jinaai
-Version: 0.1.2
+Version: 0.1.3
 Summary: Jina AI Python SDK
 Home-page: https://github.com/jina-ai/jinaai-py.git
 Author: Jina AI
 Author-email: guillaume.roncari@jina.ai
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

### Comparing `jinaai-0.1.2/README.md` & `jinaai-0.1.3/README.md`

 * *Files identical despite different names*

### Comparing `jinaai-0.1.2/jinaai/__init__.py` & `jinaai-0.1.3/jinaai/__init__.py`

 * *Files identical despite different names*

### Comparing `jinaai-0.1.2/jinaai/clients/ChatCatClient.py` & `jinaai-0.1.3/jinaai/clients/ChatCatClient.py`

 * *Files 15% similar despite different names*

```diff
@@ -35,20 +35,20 @@
                     **(options or {})
                 }
             ],
             **(options or {})
         }
 
     def to_simplified_output(self, output):
-        if 'responseContent' not in output or output['responseContent'] == '':
+        if 'choices' not in output or len(output['choices']) < 1 or output['choices'][0]['message']['content'] == '':
             raise Exception('Remote API Error, bad output: ' + str(output))
         return {
-            'output': output['responseContent'],
+            'output': output['choices'][0]['message']['content'],
             'chatId': output['chatId']
         }
 
     def generate(self, data, options = None):
-        raw_output = self.post('/completion', data)
+        raw_output = self.post('/completions', data)
         simplified_output = self.to_simplified_output(raw_output)
         if options and 'raw' in options:
             simplified_output['raw'] = raw_output
         return simplified_output
```

### Comparing `jinaai-0.1.2/jinaai/clients/HTTPClient.py` & `jinaai-0.1.3/jinaai/clients/HTTPClient.py`

 * *Files identical despite different names*

### Comparing `jinaai-0.1.2/jinaai/clients/PromptPerfectClient.py` & `jinaai-0.1.3/jinaai/clients/PromptPerfectClient.py`

 * *Files identical despite different names*

### Comparing `jinaai-0.1.2/jinaai/clients/RationaleClient.py` & `jinaai-0.1.3/jinaai/clients/RationaleClient.py`

 * *Files identical despite different names*

### Comparing `jinaai-0.1.2/jinaai/clients/SceneXClient.py` & `jinaai-0.1.3/jinaai/clients/SceneXClient.py`

 * *Files identical despite different names*

### Comparing `jinaai-0.1.2/jinaai/utils.py` & `jinaai-0.1.3/jinaai/utils.py`

 * *Files identical despite different names*

### Comparing `jinaai-0.1.2/jinaai.egg-info/PKG-INFO` & `jinaai-0.1.3/jinaai.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: jinaai
-Version: 0.1.2
+Version: 0.1.3
 Summary: Jina AI Python SDK
 Home-page: https://github.com/jina-ai/jinaai-py.git
 Author: Jina AI
 Author-email: guillaume.roncari@jina.ai
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

