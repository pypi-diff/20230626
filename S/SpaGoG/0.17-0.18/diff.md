# Comparing `tmp/SpaGoG-0.17.tar.gz` & `tmp/SpaGoG-0.18.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/SpaGoG-0.17.tar", last modified: Sat Jun 24 21:47:12 2023, max compression
+gzip compressed data, was "dist/SpaGoG-0.18.tar", last modified: Mon Jun 26 07:07:41 2023, max compression
```

## Comparing `SpaGoG-0.17.tar` & `SpaGoG-0.18.tar`

### file list

```diff
@@ -1,9 +1,9 @@
-drwxrwxr-x   0 shachar   (1000) shachar   (1000)        0 2023-06-24 21:47:12.000000 SpaGoG-0.17/
--rw-rw-r--   0 shachar   (1000) shachar   (1000)     1344 2023-06-24 21:46:57.000000 SpaGoG-0.17/setup.py
--rw-rw-r--   0 shachar   (1000) shachar   (1000)       39 2023-05-12 23:49:44.000000 SpaGoG-0.17/setup.cfg
--rw-rw-r--   0 shachar   (1000) shachar   (1000)        0 2023-06-22 20:43:34.000000 SpaGoG-0.17/README
--rw-rw-r--   0 shachar   (1000) shachar   (1000)      486 2023-06-24 21:47:12.000000 SpaGoG-0.17/PKG-INFO
-drwxrwxr-x   0 shachar   (1000) shachar   (1000)        0 2023-06-24 21:47:12.000000 SpaGoG-0.17/spagog/
--rw-rw-r--   0 shachar   (1000) shachar   (1000)     5201 2023-06-23 22:45:43.000000 SpaGoG-0.17/spagog/main.py
--rw-rw-r--   0 shachar   (1000) shachar   (1000)        0 2023-06-23 22:45:43.000000 SpaGoG-0.17/spagog/__init__.py
--rw-rw-r--   0 shachar   (1000) shachar   (1000)    11778 2023-06-23 22:45:43.000000 SpaGoG-0.17/spagog/experiments.py
+drwxrwxr-x   0 shachar   (1000) shachar   (1000)        0 2023-06-26 07:07:41.000000 SpaGoG-0.18/
+-rw-rw-r--   0 shachar   (1000) shachar   (1000)     1353 2023-06-26 07:07:08.000000 SpaGoG-0.18/setup.py
+-rw-rw-r--   0 shachar   (1000) shachar   (1000)       39 2023-05-12 23:49:44.000000 SpaGoG-0.18/setup.cfg
+-rw-rw-r--   0 shachar   (1000) shachar   (1000)        0 2023-06-22 20:43:34.000000 SpaGoG-0.18/README
+-rw-rw-r--   0 shachar   (1000) shachar   (1000)      386 2023-06-26 07:07:41.000000 SpaGoG-0.18/PKG-INFO
+drwxrwxr-x   0 shachar   (1000) shachar   (1000)        0 2023-06-26 07:07:41.000000 SpaGoG-0.18/spagog/
+-rw-rw-r--   0 shachar   (1000) shachar   (1000)     5201 2023-06-23 22:45:43.000000 SpaGoG-0.18/spagog/main.py
+-rw-rw-r--   0 shachar   (1000) shachar   (1000)        0 2023-06-23 22:45:43.000000 SpaGoG-0.18/spagog/__init__.py
+-rw-rw-r--   0 shachar   (1000) shachar   (1000)    11778 2023-06-23 22:45:43.000000 SpaGoG-0.18/spagog/experiments.py
```

### Comparing `SpaGoG-0.17/setup.py` & `SpaGoG-0.18/setup.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,26 +1,26 @@
 from distutils.core import setup
 
 setup(
     name='SpaGoG',  # How you named your package folder (MyLib)
     packages=['spagog'],  # Chose the same as "name"
-    version='0.17',  # Start with a small number and increase it with every change you make
+    version='0.18',  # Start with a small number and increase it with every change you make
     license='MIT',  # Chose a license from here: https://help.github.com/articles/licensing-a-repository
     description='Sparse data classification using Graph of Graphs',  # Give a short description about your library
     author='Shachar Hananya',  # Type in your name
     author_email='shacharhananya@gmail.com',  # Type in your E-Mail
     url='https://github.com/HananyaS/SpaGoG',  # Provide either the link to your github or to your website
-    download_url='https://github.com/HananyaS/SpaGoG/archive/refs/tags/v_0.17.tar.gz',  # I explain this later on
+    download_url='https://github.com/HananyaS/SpaGoG/archive/refs/tags/v_0.1.8.tar.gz',  # I explain this later on
     keywords=['GoG', 'Missing values', 'Graphs'],  # Keywords that define your package best
     install_requires=[  # I get to this in a second
         'pandas==1.0.5',
         'torch==2.0.1',
         'torch-geometric==2.3.1',
         'matplotlib==3.7.1',
     ],
-    classifiers=[
-        'License :: OSI Approved :: MIT License',  # Again, pick a license
-        'Programming Language :: Python :: 3.8',
-    ],
+    # classifiers=[
+    #     'License :: OSI Approved :: MIT License',  # Again, pick a license
+    #     'Programming Language :: Python :: 3.8',
+    # ],
     # add the json files that appear in default_params folder
     # package_data={'spagog': ['default_params/*.json']},
 )
```

### Comparing `SpaGoG-0.17/spagog/main.py` & `SpaGoG-0.18/spagog/main.py`

 * *Files identical despite different names*

### Comparing `SpaGoG-0.17/spagog/experiments.py` & `SpaGoG-0.18/spagog/experiments.py`

 * *Files identical despite different names*

