# Comparing `tmp/pillar1-0.1.9.2.tar.gz` & `tmp/pillar1-0.1.9.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pillar1-0.1.9.2.tar", last modified: Mon Jun 26 12:31:36 2023, max compression
+gzip compressed data, was "pillar1-0.1.9.4.tar", last modified: Mon Jun 26 12:52:32 2023, max compression
```

## Comparing `pillar1-0.1.9.2.tar` & `pillar1-0.1.9.4.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxr-xr-x   0 aymanhajja   (501) staff       (20)        0 2023-06-26 12:31:36.845296 pillar1-0.1.9.2/
--rw-r--r--   0 aymanhajja   (501) staff       (20)     3202 2023-06-26 12:31:36.845157 pillar1-0.1.9.2/PKG-INFO
--rw-r--r--   0 aymanhajja   (501) staff       (20)     2842 2023-06-19 22:34:12.000000 pillar1-0.1.9.2/README.md
-drwxr-xr-x   0 aymanhajja   (501) staff       (20)        0 2023-06-26 12:31:36.844471 pillar1-0.1.9.2/pillar1/
--rw-r--r--   0 aymanhajja   (501) staff       (20)       55 2023-06-24 20:02:24.000000 pillar1-0.1.9.2/pillar1/__init__.py
--rw-r--r--   0 aymanhajja   (501) staff       (20)     6825 2023-06-26 12:31:09.000000 pillar1-0.1.9.2/pillar1/constants.py
--rw-r--r--   0 aymanhajja   (501) staff       (20)     9993 2023-06-23 13:24:20.000000 pillar1-0.1.9.2/pillar1/constants_original.py
--rw-r--r--   0 aymanhajja   (501) staff       (20)     8567 2023-06-26 12:31:26.000000 pillar1-0.1.9.2/pillar1/pillar1.py
-drwxr-xr-x   0 aymanhajja   (501) staff       (20)        0 2023-06-26 12:31:36.844964 pillar1-0.1.9.2/pillar1.egg-info/
--rw-r--r--   0 aymanhajja   (501) staff       (20)     3202 2023-06-26 12:31:36.000000 pillar1-0.1.9.2/pillar1.egg-info/PKG-INFO
--rw-r--r--   0 aymanhajja   (501) staff       (20)      232 2023-06-26 12:31:36.000000 pillar1-0.1.9.2/pillar1.egg-info/SOURCES.txt
--rw-r--r--   0 aymanhajja   (501) staff       (20)        1 2023-06-26 12:31:36.000000 pillar1-0.1.9.2/pillar1.egg-info/dependency_links.txt
--rw-r--r--   0 aymanhajja   (501) staff       (20)        8 2023-06-26 12:31:36.000000 pillar1-0.1.9.2/pillar1.egg-info/top_level.txt
--rw-r--r--   0 aymanhajja   (501) staff       (20)       38 2023-06-26 12:31:36.845340 pillar1-0.1.9.2/setup.cfg
--rw-r--r--   0 aymanhajja   (501) staff       (20)      621 2023-06-26 12:31:36.000000 pillar1-0.1.9.2/setup.py
+drwxr-xr-x   0 aymanhajja   (501) staff       (20)        0 2023-06-26 12:52:32.435707 pillar1-0.1.9.4/
+-rw-r--r--   0 aymanhajja   (501) staff       (20)     3202 2023-06-26 12:52:32.433309 pillar1-0.1.9.4/PKG-INFO
+-rw-r--r--   0 aymanhajja   (501) staff       (20)     2842 2023-06-19 22:34:12.000000 pillar1-0.1.9.4/README.md
+drwxr-xr-x   0 aymanhajja   (501) staff       (20)        0 2023-06-26 12:52:32.429090 pillar1-0.1.9.4/pillar1/
+-rw-r--r--   0 aymanhajja   (501) staff       (20)       55 2023-06-24 20:02:24.000000 pillar1-0.1.9.4/pillar1/__init__.py
+-rw-r--r--   0 aymanhajja   (501) staff       (20)     6825 2023-06-26 12:31:09.000000 pillar1-0.1.9.4/pillar1/constants.py
+-rw-r--r--   0 aymanhajja   (501) staff       (20)     9993 2023-06-23 13:24:20.000000 pillar1-0.1.9.4/pillar1/constants_original.py
+-rw-r--r--   0 aymanhajja   (501) staff       (20)     8810 2023-06-26 12:52:10.000000 pillar1-0.1.9.4/pillar1/pillar1.py
+drwxr-xr-x   0 aymanhajja   (501) staff       (20)        0 2023-06-26 12:52:32.432077 pillar1-0.1.9.4/pillar1.egg-info/
+-rw-r--r--   0 aymanhajja   (501) staff       (20)     3202 2023-06-26 12:52:32.000000 pillar1-0.1.9.4/pillar1.egg-info/PKG-INFO
+-rw-r--r--   0 aymanhajja   (501) staff       (20)      232 2023-06-26 12:52:32.000000 pillar1-0.1.9.4/pillar1.egg-info/SOURCES.txt
+-rw-r--r--   0 aymanhajja   (501) staff       (20)        1 2023-06-26 12:52:32.000000 pillar1-0.1.9.4/pillar1.egg-info/dependency_links.txt
+-rw-r--r--   0 aymanhajja   (501) staff       (20)        8 2023-06-26 12:52:32.000000 pillar1-0.1.9.4/pillar1.egg-info/top_level.txt
+-rw-r--r--   0 aymanhajja   (501) staff       (20)       38 2023-06-26 12:52:32.436605 pillar1-0.1.9.4/setup.cfg
+-rw-r--r--   0 aymanhajja   (501) staff       (20)      621 2023-06-26 12:52:32.000000 pillar1-0.1.9.4/setup.py
```

### Comparing `pillar1-0.1.9.2/PKG-INFO` & `pillar1-0.1.9.4/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pillar1
-Version: 0.1.9.2
+Version: 0.1.9.4
 Summary: Official package for Pillar1 company
 Home-page: https://github.com/amhajja/pillar1
 Author: Ayman Hajja
 Author-email: amhajja@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Requires-Python: >=3.9
```

### Comparing `pillar1-0.1.9.2/README.md` & `pillar1-0.1.9.4/README.md`

 * *Files identical despite different names*

### Comparing `pillar1-0.1.9.2/pillar1/constants.py` & `pillar1-0.1.9.4/pillar1/constants.py`

 * *Files identical despite different names*

### Comparing `pillar1-0.1.9.2/pillar1/constants_original.py` & `pillar1-0.1.9.4/pillar1/constants_original.py`

 * *Files identical despite different names*

### Comparing `pillar1-0.1.9.2/pillar1/pillar1.py` & `pillar1-0.1.9.4/pillar1/pillar1.py`

 * *Files 3% similar despite different names*

```diff
@@ -199,18 +199,27 @@
 
             if self.api_type == 'free':
                 response = requests.post(self.curr_model['API_URL'], headers={"Authorization": f"Bearer {self.huggingface_token}"}, json=payload)
                 self.response = response.json()[0]['generated_text']
                 return self.response
 
         if prompt:
-            prompt = f"{self.curr_model['prepend']}{self.background}{prompt}{self.curr_model.get('append')}"
+            prompt = f'For the question: {prompt}{cn.APPEND}'
             self.prompt = prompt
+            # prompt = f"{self.curr_model['prepend']}{self.background}{prompt}{self.curr_model.get('append')}"
+            # self.prompt = prompt
             submit_request(self.prompt)
 
+            # Getting code
+            self.code()
+
+            # Executing code
+            result = self.execute()
+            return result
+
         else:
             question = input('What SQL are you looking for: ')
             prompt = f"{self.curr_model['prepend']}:\n\"{self.background}\"\n\nAnswer this question: {question}\" {self.curr_model.get('append', '')}"
             self.prompt = prompt
             submit_request(self.prompt)
 
             # input_text = widgets.Text(description='What SQL are you looking for:', layout=widgets.Layout(width='80%'), style={'description_width': 'initial'})
```

### Comparing `pillar1-0.1.9.2/pillar1.egg-info/PKG-INFO` & `pillar1-0.1.9.4/pillar1.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pillar1
-Version: 0.1.9.2
+Version: 0.1.9.4
 Summary: Official package for Pillar1 company
 Home-page: https://github.com/amhajja/pillar1
 Author: Ayman Hajja
 Author-email: amhajja@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Requires-Python: >=3.9
```

### Comparing `pillar1-0.1.9.2/setup.py` & `pillar1-0.1.9.4/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from setuptools import setup, find_packages
 
 with open("README.md", "r", encoding="utf-8") as fh:
     long_description = fh.read()
 
 setup(
     name='pillar1',
-    version='0.1.9.2',
+    version='0.1.9.4',
     packages=find_packages(),
     description='Official package for Pillar1 company',
     long_description=long_description,
     long_description_content_type='text/markdown',
     author='Ayman Hajja',
     author_email='amhajja@gmail.com',
     url='https://github.com/amhajja/pillar1',
```

