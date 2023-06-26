# Comparing `tmp/pillar1-0.1.9.4.tar.gz` & `tmp/pillar1-0.1.9.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pillar1-0.1.9.4.tar", last modified: Mon Jun 26 12:52:32 2023, max compression
+gzip compressed data, was "pillar1-0.1.9.5.tar", last modified: Mon Jun 26 13:06:28 2023, max compression
```

## Comparing `pillar1-0.1.9.4.tar` & `pillar1-0.1.9.5.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxr-xr-x   0 aymanhajja   (501) staff       (20)        0 2023-06-26 12:52:32.435707 pillar1-0.1.9.4/
--rw-r--r--   0 aymanhajja   (501) staff       (20)     3202 2023-06-26 12:52:32.433309 pillar1-0.1.9.4/PKG-INFO
--rw-r--r--   0 aymanhajja   (501) staff       (20)     2842 2023-06-19 22:34:12.000000 pillar1-0.1.9.4/README.md
-drwxr-xr-x   0 aymanhajja   (501) staff       (20)        0 2023-06-26 12:52:32.429090 pillar1-0.1.9.4/pillar1/
--rw-r--r--   0 aymanhajja   (501) staff       (20)       55 2023-06-24 20:02:24.000000 pillar1-0.1.9.4/pillar1/__init__.py
--rw-r--r--   0 aymanhajja   (501) staff       (20)     6825 2023-06-26 12:31:09.000000 pillar1-0.1.9.4/pillar1/constants.py
--rw-r--r--   0 aymanhajja   (501) staff       (20)     9993 2023-06-23 13:24:20.000000 pillar1-0.1.9.4/pillar1/constants_original.py
--rw-r--r--   0 aymanhajja   (501) staff       (20)     8810 2023-06-26 12:52:10.000000 pillar1-0.1.9.4/pillar1/pillar1.py
-drwxr-xr-x   0 aymanhajja   (501) staff       (20)        0 2023-06-26 12:52:32.432077 pillar1-0.1.9.4/pillar1.egg-info/
--rw-r--r--   0 aymanhajja   (501) staff       (20)     3202 2023-06-26 12:52:32.000000 pillar1-0.1.9.4/pillar1.egg-info/PKG-INFO
--rw-r--r--   0 aymanhajja   (501) staff       (20)      232 2023-06-26 12:52:32.000000 pillar1-0.1.9.4/pillar1.egg-info/SOURCES.txt
--rw-r--r--   0 aymanhajja   (501) staff       (20)        1 2023-06-26 12:52:32.000000 pillar1-0.1.9.4/pillar1.egg-info/dependency_links.txt
--rw-r--r--   0 aymanhajja   (501) staff       (20)        8 2023-06-26 12:52:32.000000 pillar1-0.1.9.4/pillar1.egg-info/top_level.txt
--rw-r--r--   0 aymanhajja   (501) staff       (20)       38 2023-06-26 12:52:32.436605 pillar1-0.1.9.4/setup.cfg
--rw-r--r--   0 aymanhajja   (501) staff       (20)      621 2023-06-26 12:52:32.000000 pillar1-0.1.9.4/setup.py
+drwxr-xr-x   0 aymanhajja   (501) staff       (20)        0 2023-06-26 13:06:28.628237 pillar1-0.1.9.5/
+-rw-r--r--   0 aymanhajja   (501) staff       (20)     3202 2023-06-26 13:06:28.628117 pillar1-0.1.9.5/PKG-INFO
+-rw-r--r--   0 aymanhajja   (501) staff       (20)     2842 2023-06-19 22:34:12.000000 pillar1-0.1.9.5/README.md
+drwxr-xr-x   0 aymanhajja   (501) staff       (20)        0 2023-06-26 13:06:28.627182 pillar1-0.1.9.5/pillar1/
+-rw-r--r--   0 aymanhajja   (501) staff       (20)       55 2023-06-24 20:02:24.000000 pillar1-0.1.9.5/pillar1/__init__.py
+-rw-r--r--   0 aymanhajja   (501) staff       (20)     6825 2023-06-26 12:31:09.000000 pillar1-0.1.9.5/pillar1/constants.py
+-rw-r--r--   0 aymanhajja   (501) staff       (20)     9993 2023-06-23 13:24:20.000000 pillar1-0.1.9.5/pillar1/constants_original.py
+-rw-r--r--   0 aymanhajja   (501) staff       (20)     8902 2023-06-26 12:58:09.000000 pillar1-0.1.9.5/pillar1/pillar1.py
+drwxr-xr-x   0 aymanhajja   (501) staff       (20)        0 2023-06-26 13:06:28.627935 pillar1-0.1.9.5/pillar1.egg-info/
+-rw-r--r--   0 aymanhajja   (501) staff       (20)     3202 2023-06-26 13:06:28.000000 pillar1-0.1.9.5/pillar1.egg-info/PKG-INFO
+-rw-r--r--   0 aymanhajja   (501) staff       (20)      232 2023-06-26 13:06:28.000000 pillar1-0.1.9.5/pillar1.egg-info/SOURCES.txt
+-rw-r--r--   0 aymanhajja   (501) staff       (20)        1 2023-06-26 13:06:28.000000 pillar1-0.1.9.5/pillar1.egg-info/dependency_links.txt
+-rw-r--r--   0 aymanhajja   (501) staff       (20)        8 2023-06-26 13:06:28.000000 pillar1-0.1.9.5/pillar1.egg-info/top_level.txt
+-rw-r--r--   0 aymanhajja   (501) staff       (20)       38 2023-06-26 13:06:28.628275 pillar1-0.1.9.5/setup.cfg
+-rw-r--r--   0 aymanhajja   (501) staff       (20)      621 2023-06-26 13:06:28.000000 pillar1-0.1.9.5/setup.py
```

### Comparing `pillar1-0.1.9.4/PKG-INFO` & `pillar1-0.1.9.5/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pillar1
-Version: 0.1.9.4
+Version: 0.1.9.5
 Summary: Official package for Pillar1 company
 Home-page: https://github.com/amhajja/pillar1
 Author: Ayman Hajja
 Author-email: amhajja@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Requires-Python: >=3.9
```

### Comparing `pillar1-0.1.9.4/README.md` & `pillar1-0.1.9.5/README.md`

 * *Files identical despite different names*

### Comparing `pillar1-0.1.9.4/pillar1/constants.py` & `pillar1-0.1.9.5/pillar1/constants.py`

 * *Files identical despite different names*

### Comparing `pillar1-0.1.9.4/pillar1/constants_original.py` & `pillar1-0.1.9.5/pillar1/constants_original.py`

 * *Files identical despite different names*

### Comparing `pillar1-0.1.9.4/pillar1/pillar1.py` & `pillar1-0.1.9.5/pillar1/pillar1.py`

 * *Files 1% similar despite different names*

```diff
@@ -166,15 +166,15 @@
         display(widgets.HBox([html_widget]))
 
     def execute(self):
         spark = SparkSession.builder.getOrCreate()
         self.result = spark.sql(self.cleaned_code)
         return self.result
 
-    def query(self, prompt: str = ''):
+    def query(self, prompt: str = '', print_sql: bool = False):
         def submit_request(prompt):
             payload = {
                 'inputs': prompt,
                 "parameters": {
                     "do_sample": self.do_sample,
                     "top_p": 0.7,
                     "temperature": self.temperature,
@@ -207,14 +207,16 @@
             self.prompt = prompt
             # prompt = f"{self.curr_model['prepend']}{self.background}{prompt}{self.curr_model.get('append')}"
             # self.prompt = prompt
             submit_request(self.prompt)
 
             # Getting code
             self.code()
+            if print_sql:
+                print(self.cleaned_code)
 
             # Executing code
             result = self.execute()
             return result
 
         else:
             question = input('What SQL are you looking for: ')
```

### Comparing `pillar1-0.1.9.4/pillar1.egg-info/PKG-INFO` & `pillar1-0.1.9.5/pillar1.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pillar1
-Version: 0.1.9.4
+Version: 0.1.9.5
 Summary: Official package for Pillar1 company
 Home-page: https://github.com/amhajja/pillar1
 Author: Ayman Hajja
 Author-email: amhajja@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Requires-Python: >=3.9
```

### Comparing `pillar1-0.1.9.4/setup.py` & `pillar1-0.1.9.5/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from setuptools import setup, find_packages
 
 with open("README.md", "r", encoding="utf-8") as fh:
     long_description = fh.read()
 
 setup(
     name='pillar1',
-    version='0.1.9.4',
+    version='0.1.9.5',
     packages=find_packages(),
     description='Official package for Pillar1 company',
     long_description=long_description,
     long_description_content_type='text/markdown',
     author='Ayman Hajja',
     author_email='amhajja@gmail.com',
     url='https://github.com/amhajja/pillar1',
```

