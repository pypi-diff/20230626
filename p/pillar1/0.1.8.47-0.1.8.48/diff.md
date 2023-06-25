# Comparing `tmp/pillar1-0.1.8.47.tar.gz` & `tmp/pillar1-0.1.8.48.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pillar1-0.1.8.47.tar", last modified: Sun Jun 25 23:37:27 2023, max compression
+gzip compressed data, was "pillar1-0.1.8.48.tar", last modified: Sun Jun 25 23:44:13 2023, max compression
```

## Comparing `pillar1-0.1.8.47.tar` & `pillar1-0.1.8.48.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxr-xr-x   0 aymanhajja   (501) staff       (20)        0 2023-06-25 23:37:27.139898 pillar1-0.1.8.47/
--rw-r--r--   0 aymanhajja   (501) staff       (20)     3203 2023-06-25 23:37:27.139773 pillar1-0.1.8.47/PKG-INFO
--rw-r--r--   0 aymanhajja   (501) staff       (20)     2842 2023-06-19 22:34:12.000000 pillar1-0.1.8.47/README.md
-drwxr-xr-x   0 aymanhajja   (501) staff       (20)        0 2023-06-25 23:37:27.139049 pillar1-0.1.8.47/pillar1/
--rw-r--r--   0 aymanhajja   (501) staff       (20)       55 2023-06-24 20:02:24.000000 pillar1-0.1.8.47/pillar1/__init__.py
--rw-r--r--   0 aymanhajja   (501) staff       (20)     1372 2023-06-25 23:21:21.000000 pillar1-0.1.8.47/pillar1/constants.py
--rw-r--r--   0 aymanhajja   (501) staff       (20)     9993 2023-06-23 13:24:20.000000 pillar1-0.1.8.47/pillar1/constants_original.py
--rw-r--r--   0 aymanhajja   (501) staff       (20)     8549 2023-06-25 23:37:24.000000 pillar1-0.1.8.47/pillar1/pillar1.py
-drwxr-xr-x   0 aymanhajja   (501) staff       (20)        0 2023-06-25 23:37:27.139582 pillar1-0.1.8.47/pillar1.egg-info/
--rw-r--r--   0 aymanhajja   (501) staff       (20)     3203 2023-06-25 23:37:27.000000 pillar1-0.1.8.47/pillar1.egg-info/PKG-INFO
--rw-r--r--   0 aymanhajja   (501) staff       (20)      232 2023-06-25 23:37:27.000000 pillar1-0.1.8.47/pillar1.egg-info/SOURCES.txt
--rw-r--r--   0 aymanhajja   (501) staff       (20)        1 2023-06-25 23:37:27.000000 pillar1-0.1.8.47/pillar1.egg-info/dependency_links.txt
--rw-r--r--   0 aymanhajja   (501) staff       (20)        8 2023-06-25 23:37:27.000000 pillar1-0.1.8.47/pillar1.egg-info/top_level.txt
--rw-r--r--   0 aymanhajja   (501) staff       (20)       38 2023-06-25 23:37:27.139943 pillar1-0.1.8.47/setup.cfg
--rw-r--r--   0 aymanhajja   (501) staff       (20)      622 2023-06-25 23:37:26.000000 pillar1-0.1.8.47/setup.py
+drwxr-xr-x   0 aymanhajja   (501) staff       (20)        0 2023-06-25 23:44:13.456098 pillar1-0.1.8.48/
+-rw-r--r--   0 aymanhajja   (501) staff       (20)     3203 2023-06-25 23:44:13.455972 pillar1-0.1.8.48/PKG-INFO
+-rw-r--r--   0 aymanhajja   (501) staff       (20)     2842 2023-06-19 22:34:12.000000 pillar1-0.1.8.48/README.md
+drwxr-xr-x   0 aymanhajja   (501) staff       (20)        0 2023-06-25 23:44:13.455280 pillar1-0.1.8.48/pillar1/
+-rw-r--r--   0 aymanhajja   (501) staff       (20)       55 2023-06-24 20:02:24.000000 pillar1-0.1.8.48/pillar1/__init__.py
+-rw-r--r--   0 aymanhajja   (501) staff       (20)     1372 2023-06-25 23:21:21.000000 pillar1-0.1.8.48/pillar1/constants.py
+-rw-r--r--   0 aymanhajja   (501) staff       (20)     9993 2023-06-23 13:24:20.000000 pillar1-0.1.8.48/pillar1/constants_original.py
+-rw-r--r--   0 aymanhajja   (501) staff       (20)     8614 2023-06-25 23:44:10.000000 pillar1-0.1.8.48/pillar1/pillar1.py
+drwxr-xr-x   0 aymanhajja   (501) staff       (20)        0 2023-06-25 23:44:13.455791 pillar1-0.1.8.48/pillar1.egg-info/
+-rw-r--r--   0 aymanhajja   (501) staff       (20)     3203 2023-06-25 23:44:13.000000 pillar1-0.1.8.48/pillar1.egg-info/PKG-INFO
+-rw-r--r--   0 aymanhajja   (501) staff       (20)      232 2023-06-25 23:44:13.000000 pillar1-0.1.8.48/pillar1.egg-info/SOURCES.txt
+-rw-r--r--   0 aymanhajja   (501) staff       (20)        1 2023-06-25 23:44:13.000000 pillar1-0.1.8.48/pillar1.egg-info/dependency_links.txt
+-rw-r--r--   0 aymanhajja   (501) staff       (20)        8 2023-06-25 23:44:13.000000 pillar1-0.1.8.48/pillar1.egg-info/top_level.txt
+-rw-r--r--   0 aymanhajja   (501) staff       (20)       38 2023-06-25 23:44:13.456146 pillar1-0.1.8.48/setup.cfg
+-rw-r--r--   0 aymanhajja   (501) staff       (20)      622 2023-06-25 23:44:13.000000 pillar1-0.1.8.48/setup.py
```

### Comparing `pillar1-0.1.8.47/PKG-INFO` & `pillar1-0.1.8.48/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pillar1
-Version: 0.1.8.47
+Version: 0.1.8.48
 Summary: Official package for Pillar1 company
 Home-page: https://github.com/amhajja/pillar1
 Author: Ayman Hajja
 Author-email: amhajja@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Requires-Python: >=3.9
```

### Comparing `pillar1-0.1.8.47/README.md` & `pillar1-0.1.8.48/README.md`

 * *Files identical despite different names*

### Comparing `pillar1-0.1.8.47/pillar1/constants.py` & `pillar1-0.1.8.48/pillar1/constants.py`

 * *Files identical despite different names*

### Comparing `pillar1-0.1.8.47/pillar1/constants_original.py` & `pillar1-0.1.8.48/pillar1/constants_original.py`

 * *Files identical despite different names*

### Comparing `pillar1-0.1.8.47/pillar1/pillar1.py` & `pillar1-0.1.8.48/pillar1/pillar1.py`

 * *Files 2% similar despite different names*

```diff
@@ -139,14 +139,15 @@
             layout=widgets.Layout(width='80%'),
         )
 
         html_widget = widgets.HTML(value='')
 
         # Function to handle button click event
         def on_button_clicked(b):
+            textarea.value = 'Request submitted, please wait...'
             self.query(f'For the question: {dropdown.value.lower()}, here is the SQL, ```sql')
             self.code()
             textarea.value = self.cleaned_code
             display(widgets.HBox([textarea, button_execute]))
 
         def show_html_res(b):
             html_widget.value = ''
```

### Comparing `pillar1-0.1.8.47/pillar1.egg-info/PKG-INFO` & `pillar1-0.1.8.48/pillar1.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pillar1
-Version: 0.1.8.47
+Version: 0.1.8.48
 Summary: Official package for Pillar1 company
 Home-page: https://github.com/amhajja/pillar1
 Author: Ayman Hajja
 Author-email: amhajja@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Requires-Python: >=3.9
```

### Comparing `pillar1-0.1.8.47/setup.py` & `pillar1-0.1.8.48/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from setuptools import setup, find_packages
 
 with open("README.md", "r", encoding="utf-8") as fh:
     long_description = fh.read()
 
 setup(
     name='pillar1',
-    version='0.1.8.47',
+    version='0.1.8.48',
     packages=find_packages(),
     description='Official package for Pillar1 company',
     long_description=long_description,
     long_description_content_type='text/markdown',
     author='Ayman Hajja',
     author_email='amhajja@gmail.com',
     url='https://github.com/amhajja/pillar1',
```

