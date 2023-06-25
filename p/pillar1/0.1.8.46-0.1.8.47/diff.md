# Comparing `tmp/pillar1-0.1.8.46.tar.gz` & `tmp/pillar1-0.1.8.47.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pillar1-0.1.8.46.tar", last modified: Sun Jun 25 23:26:44 2023, max compression
+gzip compressed data, was "pillar1-0.1.8.47.tar", last modified: Sun Jun 25 23:37:27 2023, max compression
```

## Comparing `pillar1-0.1.8.46.tar` & `pillar1-0.1.8.47.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxr-xr-x   0 aymanhajja   (501) staff       (20)        0 2023-06-25 23:26:44.801812 pillar1-0.1.8.46/
--rw-r--r--   0 aymanhajja   (501) staff       (20)     3203 2023-06-25 23:26:44.801050 pillar1-0.1.8.46/PKG-INFO
--rw-r--r--   0 aymanhajja   (501) staff       (20)     2842 2023-06-19 22:34:12.000000 pillar1-0.1.8.46/README.md
-drwxr-xr-x   0 aymanhajja   (501) staff       (20)        0 2023-06-25 23:26:44.796596 pillar1-0.1.8.46/pillar1/
--rw-r--r--   0 aymanhajja   (501) staff       (20)       55 2023-06-24 20:02:24.000000 pillar1-0.1.8.46/pillar1/__init__.py
--rw-r--r--   0 aymanhajja   (501) staff       (20)     1372 2023-06-25 23:21:21.000000 pillar1-0.1.8.46/pillar1/constants.py
--rw-r--r--   0 aymanhajja   (501) staff       (20)     9993 2023-06-23 13:24:20.000000 pillar1-0.1.8.46/pillar1/constants_original.py
--rw-r--r--   0 aymanhajja   (501) staff       (20)     8391 2023-06-25 23:26:07.000000 pillar1-0.1.8.46/pillar1/pillar1.py
-drwxr-xr-x   0 aymanhajja   (501) staff       (20)        0 2023-06-25 23:26:44.797480 pillar1-0.1.8.46/pillar1.egg-info/
--rw-r--r--   0 aymanhajja   (501) staff       (20)     3203 2023-06-25 23:26:44.000000 pillar1-0.1.8.46/pillar1.egg-info/PKG-INFO
--rw-r--r--   0 aymanhajja   (501) staff       (20)      232 2023-06-25 23:26:44.000000 pillar1-0.1.8.46/pillar1.egg-info/SOURCES.txt
--rw-r--r--   0 aymanhajja   (501) staff       (20)        1 2023-06-25 23:26:44.000000 pillar1-0.1.8.46/pillar1.egg-info/dependency_links.txt
--rw-r--r--   0 aymanhajja   (501) staff       (20)        8 2023-06-25 23:26:44.000000 pillar1-0.1.8.46/pillar1.egg-info/top_level.txt
--rw-r--r--   0 aymanhajja   (501) staff       (20)       38 2023-06-25 23:26:44.801864 pillar1-0.1.8.46/setup.cfg
--rw-r--r--   0 aymanhajja   (501) staff       (20)      622 2023-06-25 23:26:44.000000 pillar1-0.1.8.46/setup.py
+drwxr-xr-x   0 aymanhajja   (501) staff       (20)        0 2023-06-25 23:37:27.139898 pillar1-0.1.8.47/
+-rw-r--r--   0 aymanhajja   (501) staff       (20)     3203 2023-06-25 23:37:27.139773 pillar1-0.1.8.47/PKG-INFO
+-rw-r--r--   0 aymanhajja   (501) staff       (20)     2842 2023-06-19 22:34:12.000000 pillar1-0.1.8.47/README.md
+drwxr-xr-x   0 aymanhajja   (501) staff       (20)        0 2023-06-25 23:37:27.139049 pillar1-0.1.8.47/pillar1/
+-rw-r--r--   0 aymanhajja   (501) staff       (20)       55 2023-06-24 20:02:24.000000 pillar1-0.1.8.47/pillar1/__init__.py
+-rw-r--r--   0 aymanhajja   (501) staff       (20)     1372 2023-06-25 23:21:21.000000 pillar1-0.1.8.47/pillar1/constants.py
+-rw-r--r--   0 aymanhajja   (501) staff       (20)     9993 2023-06-23 13:24:20.000000 pillar1-0.1.8.47/pillar1/constants_original.py
+-rw-r--r--   0 aymanhajja   (501) staff       (20)     8549 2023-06-25 23:37:24.000000 pillar1-0.1.8.47/pillar1/pillar1.py
+drwxr-xr-x   0 aymanhajja   (501) staff       (20)        0 2023-06-25 23:37:27.139582 pillar1-0.1.8.47/pillar1.egg-info/
+-rw-r--r--   0 aymanhajja   (501) staff       (20)     3203 2023-06-25 23:37:27.000000 pillar1-0.1.8.47/pillar1.egg-info/PKG-INFO
+-rw-r--r--   0 aymanhajja   (501) staff       (20)      232 2023-06-25 23:37:27.000000 pillar1-0.1.8.47/pillar1.egg-info/SOURCES.txt
+-rw-r--r--   0 aymanhajja   (501) staff       (20)        1 2023-06-25 23:37:27.000000 pillar1-0.1.8.47/pillar1.egg-info/dependency_links.txt
+-rw-r--r--   0 aymanhajja   (501) staff       (20)        8 2023-06-25 23:37:27.000000 pillar1-0.1.8.47/pillar1.egg-info/top_level.txt
+-rw-r--r--   0 aymanhajja   (501) staff       (20)       38 2023-06-25 23:37:27.139943 pillar1-0.1.8.47/setup.cfg
+-rw-r--r--   0 aymanhajja   (501) staff       (20)      622 2023-06-25 23:37:26.000000 pillar1-0.1.8.47/setup.py
```

### Comparing `pillar1-0.1.8.46/PKG-INFO` & `pillar1-0.1.8.47/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pillar1
-Version: 0.1.8.46
+Version: 0.1.8.47
 Summary: Official package for Pillar1 company
 Home-page: https://github.com/amhajja/pillar1
 Author: Ayman Hajja
 Author-email: amhajja@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Requires-Python: >=3.9
```

### Comparing `pillar1-0.1.8.46/README.md` & `pillar1-0.1.8.47/README.md`

 * *Files identical despite different names*

### Comparing `pillar1-0.1.8.46/pillar1/constants.py` & `pillar1-0.1.8.47/pillar1/constants.py`

 * *Files identical despite different names*

### Comparing `pillar1-0.1.8.46/pillar1/constants_original.py` & `pillar1-0.1.8.47/pillar1/constants_original.py`

 * *Files identical despite different names*

### Comparing `pillar1-0.1.8.46/pillar1/pillar1.py` & `pillar1-0.1.8.47/pillar1/pillar1.py`

 * *Files 2% similar despite different names*

```diff
@@ -145,17 +145,21 @@
         def on_button_clicked(b):
             self.query(f'For the question: {dropdown.value.lower()}, here is the SQL, ```sql')
             self.code()
             textarea.value = self.cleaned_code
             display(widgets.HBox([textarea, button_execute]))
 
         def show_html_res(b):
-            self.cleaned_code = textarea.value
-            res = self.execute().toPandas().to_html()
-            html_widget.value = res
+            html_widget.value = ''
+            try:
+                self.cleaned_code = textarea.value
+                res = self.execute().toPandas().to_html()
+                html_widget.value = res
+            except Exception as e:
+                html_widget.value = f"<h3>Error: {e}</h3>"
 
         button.on_click(on_button_clicked)
         button_execute.on_click(show_html_res)
 
         # Display the widgets
         display(widgets.HBox([dropdown, button]))
         display(widgets.HBox([textarea, button_execute]))
```

### Comparing `pillar1-0.1.8.46/pillar1.egg-info/PKG-INFO` & `pillar1-0.1.8.47/pillar1.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pillar1
-Version: 0.1.8.46
+Version: 0.1.8.47
 Summary: Official package for Pillar1 company
 Home-page: https://github.com/amhajja/pillar1
 Author: Ayman Hajja
 Author-email: amhajja@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Requires-Python: >=3.9
```

### Comparing `pillar1-0.1.8.46/setup.py` & `pillar1-0.1.8.47/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from setuptools import setup, find_packages
 
 with open("README.md", "r", encoding="utf-8") as fh:
     long_description = fh.read()
 
 setup(
     name='pillar1',
-    version='0.1.8.46',
+    version='0.1.8.47',
     packages=find_packages(),
     description='Official package for Pillar1 company',
     long_description=long_description,
     long_description_content_type='text/markdown',
     author='Ayman Hajja',
     author_email='amhajja@gmail.com',
     url='https://github.com/amhajja/pillar1',
```

