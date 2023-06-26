# Comparing `tmp/pillar1-0.1.9.6.tar.gz` & `tmp/pillar1-0.1.9.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pillar1-0.1.9.6.tar", last modified: Mon Jun 26 13:11:27 2023, max compression
+gzip compressed data, was "pillar1-0.1.9.7.tar", last modified: Mon Jun 26 13:13:00 2023, max compression
```

## Comparing `pillar1-0.1.9.6.tar` & `pillar1-0.1.9.7.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxr-xr-x   0 aymanhajja   (501) staff       (20)        0 2023-06-26 13:11:27.412727 pillar1-0.1.9.6/
--rw-r--r--   0 aymanhajja   (501) staff       (20)     3202 2023-06-26 13:11:27.412562 pillar1-0.1.9.6/PKG-INFO
--rw-r--r--   0 aymanhajja   (501) staff       (20)     2842 2023-06-19 22:34:12.000000 pillar1-0.1.9.6/README.md
-drwxr-xr-x   0 aymanhajja   (501) staff       (20)        0 2023-06-26 13:11:27.406745 pillar1-0.1.9.6/pillar1/
--rw-r--r--   0 aymanhajja   (501) staff       (20)       55 2023-06-24 20:02:24.000000 pillar1-0.1.9.6/pillar1/__init__.py
--rw-r--r--   0 aymanhajja   (501) staff       (20)     6792 2023-06-26 13:11:05.000000 pillar1-0.1.9.6/pillar1/constants.py
--rw-r--r--   0 aymanhajja   (501) staff       (20)     9993 2023-06-23 13:24:20.000000 pillar1-0.1.9.6/pillar1/constants_original.py
--rw-r--r--   0 aymanhajja   (501) staff       (20)     8938 2023-06-26 13:11:23.000000 pillar1-0.1.9.6/pillar1/pillar1.py
-drwxr-xr-x   0 aymanhajja   (501) staff       (20)        0 2023-06-26 13:11:27.408399 pillar1-0.1.9.6/pillar1.egg-info/
--rw-r--r--   0 aymanhajja   (501) staff       (20)     3202 2023-06-26 13:11:27.000000 pillar1-0.1.9.6/pillar1.egg-info/PKG-INFO
--rw-r--r--   0 aymanhajja   (501) staff       (20)      232 2023-06-26 13:11:27.000000 pillar1-0.1.9.6/pillar1.egg-info/SOURCES.txt
--rw-r--r--   0 aymanhajja   (501) staff       (20)        1 2023-06-26 13:11:27.000000 pillar1-0.1.9.6/pillar1.egg-info/dependency_links.txt
--rw-r--r--   0 aymanhajja   (501) staff       (20)        8 2023-06-26 13:11:27.000000 pillar1-0.1.9.6/pillar1.egg-info/top_level.txt
--rw-r--r--   0 aymanhajja   (501) staff       (20)       38 2023-06-26 13:11:27.412823 pillar1-0.1.9.6/setup.cfg
--rw-r--r--   0 aymanhajja   (501) staff       (20)      621 2023-06-26 13:11:27.000000 pillar1-0.1.9.6/setup.py
+drwxr-xr-x   0 aymanhajja   (501) staff       (20)        0 2023-06-26 13:13:00.953005 pillar1-0.1.9.7/
+-rw-r--r--   0 aymanhajja   (501) staff       (20)     3202 2023-06-26 13:13:00.952888 pillar1-0.1.9.7/PKG-INFO
+-rw-r--r--   0 aymanhajja   (501) staff       (20)     2842 2023-06-19 22:34:12.000000 pillar1-0.1.9.7/README.md
+drwxr-xr-x   0 aymanhajja   (501) staff       (20)        0 2023-06-26 13:13:00.952234 pillar1-0.1.9.7/pillar1/
+-rw-r--r--   0 aymanhajja   (501) staff       (20)       55 2023-06-24 20:02:24.000000 pillar1-0.1.9.7/pillar1/__init__.py
+-rw-r--r--   0 aymanhajja   (501) staff       (20)     6792 2023-06-26 13:11:05.000000 pillar1-0.1.9.7/pillar1/constants.py
+-rw-r--r--   0 aymanhajja   (501) staff       (20)     9993 2023-06-23 13:24:20.000000 pillar1-0.1.9.7/pillar1/constants_original.py
+-rw-r--r--   0 aymanhajja   (501) staff       (20)     9031 2023-06-26 13:12:59.000000 pillar1-0.1.9.7/pillar1/pillar1.py
+drwxr-xr-x   0 aymanhajja   (501) staff       (20)        0 2023-06-26 13:13:00.952707 pillar1-0.1.9.7/pillar1.egg-info/
+-rw-r--r--   0 aymanhajja   (501) staff       (20)     3202 2023-06-26 13:13:00.000000 pillar1-0.1.9.7/pillar1.egg-info/PKG-INFO
+-rw-r--r--   0 aymanhajja   (501) staff       (20)      232 2023-06-26 13:13:00.000000 pillar1-0.1.9.7/pillar1.egg-info/SOURCES.txt
+-rw-r--r--   0 aymanhajja   (501) staff       (20)        1 2023-06-26 13:13:00.000000 pillar1-0.1.9.7/pillar1.egg-info/dependency_links.txt
+-rw-r--r--   0 aymanhajja   (501) staff       (20)        8 2023-06-26 13:13:00.000000 pillar1-0.1.9.7/pillar1.egg-info/top_level.txt
+-rw-r--r--   0 aymanhajja   (501) staff       (20)       38 2023-06-26 13:13:00.953044 pillar1-0.1.9.7/setup.cfg
+-rw-r--r--   0 aymanhajja   (501) staff       (20)      621 2023-06-26 13:13:00.000000 pillar1-0.1.9.7/setup.py
```

### Comparing `pillar1-0.1.9.6/PKG-INFO` & `pillar1-0.1.9.7/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pillar1
-Version: 0.1.9.6
+Version: 0.1.9.7
 Summary: Official package for Pillar1 company
 Home-page: https://github.com/amhajja/pillar1
 Author: Ayman Hajja
 Author-email: amhajja@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Requires-Python: >=3.9
```

### Comparing `pillar1-0.1.9.6/README.md` & `pillar1-0.1.9.7/README.md`

 * *Files identical despite different names*

### Comparing `pillar1-0.1.9.6/pillar1/constants.py` & `pillar1-0.1.9.7/pillar1/constants.py`

 * *Files identical despite different names*

### Comparing `pillar1-0.1.9.6/pillar1/constants_original.py` & `pillar1-0.1.9.7/pillar1/constants_original.py`

 * *Files identical despite different names*

### Comparing `pillar1-0.1.9.6/pillar1/pillar1.py` & `pillar1-0.1.9.7/pillar1/pillar1.py`

 * *Files 2% similar despite different names*

```diff
@@ -215,14 +215,17 @@
                 print(self.cleaned_code)
 
             # Executing code
             result = self.execute()
             return result
 
         else:
+            print("Please provide a value in the textbox at the top...")
+            return
+
             question = input('What SQL are you looking for: ')
             prompt = f"{self.curr_model['prepend']}:\n\"{self.background}\"\n\nAnswer this question: {question}\" {self.curr_model.get('append', '')}"
             self.prompt = prompt
             submit_request(self.prompt)
 
             # input_text = widgets.Text(description='What SQL are you looking for:', layout=widgets.Layout(width='80%'), style={'description_width': 'initial'})
             # button = widgets.Button(description='Submit')
```

### Comparing `pillar1-0.1.9.6/pillar1.egg-info/PKG-INFO` & `pillar1-0.1.9.7/pillar1.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pillar1
-Version: 0.1.9.6
+Version: 0.1.9.7
 Summary: Official package for Pillar1 company
 Home-page: https://github.com/amhajja/pillar1
 Author: Ayman Hajja
 Author-email: amhajja@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Requires-Python: >=3.9
```

### Comparing `pillar1-0.1.9.6/setup.py` & `pillar1-0.1.9.7/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from setuptools import setup, find_packages
 
 with open("README.md", "r", encoding="utf-8") as fh:
     long_description = fh.read()
 
 setup(
     name='pillar1',
-    version='0.1.9.6',
+    version='0.1.9.7',
     packages=find_packages(),
     description='Official package for Pillar1 company',
     long_description=long_description,
     long_description_content_type='text/markdown',
     author='Ayman Hajja',
     author_email='amhajja@gmail.com',
     url='https://github.com/amhajja/pillar1',
```

