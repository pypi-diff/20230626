# Comparing `tmp/Mensajes-brandoncap-5.0.tar.gz` & `tmp/Mensajes-brandoncap-6.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "Mensajes-brandoncap-5.0.tar", last modified: Mon Jun 26 03:56:31 2023, max compression
+gzip compressed data, was "Mensajes-brandoncap-6.0.tar", last modified: Mon Jun 26 04:40:50 2023, max compression
```

## Comparing `Mensajes-brandoncap-5.0.tar` & `Mensajes-brandoncap-6.0.tar`

### file list

```diff
@@ -1,25 +1,25 @@
-drwxrwxrwx   0        0        0        0 2023-06-26 03:56:31.991104 Mensajes-brandoncap-5.0/
--rw-rw-rw-   0        0        0     1096 2023-06-26 02:53:12.000000 Mensajes-brandoncap-5.0/LICENSE
--rw-rw-rw-   0        0        0       60 2023-06-26 02:53:29.000000 Mensajes-brandoncap-5.0/MANIFEST.in
-drwxrwxrwx   0        0        0        0 2023-06-26 03:56:31.975518 Mensajes-brandoncap-5.0/Mensajes_brandoncap.egg-info/
--rw-rw-rw-   0        0        0      705 2023-06-26 03:56:31.000000 Mensajes-brandoncap-5.0/Mensajes_brandoncap.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      434 2023-06-26 03:56:31.000000 Mensajes-brandoncap-5.0/Mensajes_brandoncap.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-26 03:56:31.000000 Mensajes-brandoncap-5.0/Mensajes_brandoncap.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       14 2023-06-26 03:56:31.000000 Mensajes-brandoncap-5.0/Mensajes_brandoncap.egg-info/requires.txt
--rw-rw-rw-   0        0        0       15 2023-06-26 03:56:31.000000 Mensajes-brandoncap-5.0/Mensajes_brandoncap.egg-info/top_level.txt
--rw-rw-rw-   0        0        0      705 2023-06-26 03:56:31.991104 Mensajes-brandoncap-5.0/PKG-INFO
--rw-rw-rw-   0        0        0       63 2023-06-26 02:44:18.000000 Mensajes-brandoncap-5.0/README.md
-drwxrwxrwx   0        0        0        0 2023-06-26 03:56:31.977050 Mensajes-brandoncap-5.0/mensajes/
--rw-rw-rw-   0        0        0       37 2023-06-22 20:49:29.000000 Mensajes-brandoncap-5.0/mensajes/__init__.py
-drwxrwxrwx   0        0        0        0 2023-06-26 03:56:31.980050 Mensajes-brandoncap-5.0/mensajes/adios/
--rw-rw-rw-   0        0        0       46 2023-06-22 20:59:04.000000 Mensajes-brandoncap-5.0/mensajes/adios/__init__.py
--rw-rw-rw-   0        0        0      266 2023-06-23 19:21:18.000000 Mensajes-brandoncap-5.0/mensajes/adios/despedidas.py
-drwxrwxrwx   0        0        0        0 2023-06-26 03:56:31.984053 Mensajes-brandoncap-5.0/mensajes/hola/
--rw-rw-rw-   0        0        0       45 2023-06-22 20:59:16.000000 Mensajes-brandoncap-5.0/mensajes/hola/__init__.py
--rw-rw-rw-   0        0        0      316 2023-06-25 22:38:35.000000 Mensajes-brandoncap-5.0/mensajes/hola/saludos.py
--rw-rw-rw-   0        0        0       13 2023-06-25 23:17:40.000000 Mensajes-brandoncap-5.0/requirements.txt
--rw-rw-rw-   0        0        0       42 2023-06-26 03:56:31.992104 Mensajes-brandoncap-5.0/setup.cfg
--rw-rw-rw-   0        0        0      964 2023-06-26 03:55:59.000000 Mensajes-brandoncap-5.0/setup.py
-drwxrwxrwx   0        0        0        0 2023-06-26 03:56:31.990105 Mensajes-brandoncap-5.0/tests/
--rw-rw-rw-   0        0        0       25 2023-06-26 00:09:08.000000 Mensajes-brandoncap-5.0/tests/__init__.py
--rw-rw-rw-   0        0        0      408 2023-06-26 00:08:36.000000 Mensajes-brandoncap-5.0/tests/test_hola.py
+drwxrwxrwx   0        0        0        0 2023-06-26 04:40:50.046330 Mensajes-brandoncap-6.0/
+-rw-rw-rw-   0        0        0     1096 2023-06-26 02:53:12.000000 Mensajes-brandoncap-6.0/LICENSE
+-rw-rw-rw-   0        0        0       60 2023-06-26 02:53:29.000000 Mensajes-brandoncap-6.0/MANIFEST.in
+drwxrwxrwx   0        0        0        0 2023-06-26 04:40:50.029124 Mensajes-brandoncap-6.0/Mensajes_brandoncap.egg-info/
+-rw-rw-rw-   0        0        0      705 2023-06-26 04:40:49.000000 Mensajes-brandoncap-6.0/Mensajes_brandoncap.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      434 2023-06-26 04:40:49.000000 Mensajes-brandoncap-6.0/Mensajes_brandoncap.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-26 04:40:49.000000 Mensajes-brandoncap-6.0/Mensajes_brandoncap.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       14 2023-06-26 04:40:49.000000 Mensajes-brandoncap-6.0/Mensajes_brandoncap.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       15 2023-06-26 04:40:49.000000 Mensajes-brandoncap-6.0/Mensajes_brandoncap.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0      705 2023-06-26 04:40:50.045231 Mensajes-brandoncap-6.0/PKG-INFO
+-rw-rw-rw-   0        0        0       63 2023-06-26 02:44:18.000000 Mensajes-brandoncap-6.0/README.md
+drwxrwxrwx   0        0        0        0 2023-06-26 04:40:50.030560 Mensajes-brandoncap-6.0/mensajes/
+-rw-rw-rw-   0        0        0       37 2023-06-22 20:49:29.000000 Mensajes-brandoncap-6.0/mensajes/__init__.py
+drwxrwxrwx   0        0        0        0 2023-06-26 04:40:50.035583 Mensajes-brandoncap-6.0/mensajes/adios/
+-rw-rw-rw-   0        0        0       46 2023-06-22 20:59:04.000000 Mensajes-brandoncap-6.0/mensajes/adios/__init__.py
+-rw-rw-rw-   0        0        0      272 2023-06-26 04:39:48.000000 Mensajes-brandoncap-6.0/mensajes/adios/despedidas.py
+drwxrwxrwx   0        0        0        0 2023-06-26 04:40:50.039158 Mensajes-brandoncap-6.0/mensajes/hola/
+-rw-rw-rw-   0        0        0       45 2023-06-22 20:59:16.000000 Mensajes-brandoncap-6.0/mensajes/hola/__init__.py
+-rw-rw-rw-   0        0        0      316 2023-06-25 22:38:35.000000 Mensajes-brandoncap-6.0/mensajes/hola/saludos.py
+-rw-rw-rw-   0        0        0       13 2023-06-25 23:17:40.000000 Mensajes-brandoncap-6.0/requirements.txt
+-rw-rw-rw-   0        0        0       42 2023-06-26 04:40:50.046330 Mensajes-brandoncap-6.0/setup.cfg
+-rw-rw-rw-   0        0        0      964 2023-06-26 04:39:58.000000 Mensajes-brandoncap-6.0/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-26 04:40:50.043219 Mensajes-brandoncap-6.0/tests/
+-rw-rw-rw-   0        0        0       25 2023-06-26 00:09:08.000000 Mensajes-brandoncap-6.0/tests/__init__.py
+-rw-rw-rw-   0        0        0      408 2023-06-26 00:08:36.000000 Mensajes-brandoncap-6.0/tests/test_hola.py
```

### Comparing `Mensajes-brandoncap-5.0/LICENSE` & `Mensajes-brandoncap-6.0/LICENSE`

 * *Files identical despite different names*

### Comparing `Mensajes-brandoncap-5.0/Mensajes_brandoncap.egg-info/PKG-INFO` & `Mensajes-brandoncap-6.0/Mensajes_brandoncap.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: Mensajes-brandoncap
-Version: 5.0
+Version: 6.0
 Summary: un paquete para saludar y despedir
 Home-page: https://www.brandon.dev
 Author: Brandon Fornes
 Author-email: Brandon@gmail.com
 Classifier: Environment :: Console
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: Academic Free License (AFL)
```

### Comparing `Mensajes-brandoncap-5.0/PKG-INFO` & `Mensajes-brandoncap-6.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: Mensajes-brandoncap
-Version: 5.0
+Version: 6.0
 Summary: un paquete para saludar y despedir
 Home-page: https://www.brandon.dev
 Author: Brandon Fornes
 Author-email: Brandon@gmail.com
 Classifier: Environment :: Console
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: Academic Free License (AFL)
```

### Comparing `Mensajes-brandoncap-5.0/setup.py` & `Mensajes-brandoncap-6.0/setup.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
     name='Mensajes-brandoncap',
-    version='5.0',
+    version='6.0',
     description='un paquete para saludar y despedir',
     long_description=open('README.md').read(),
     long_description_content_type='text/markdown',
     author='Brandon Fornes',
     author_email='Brandon@gmail.com',
     url='https://www.brandon.dev',
     license_files=['LICENSE'],
```

