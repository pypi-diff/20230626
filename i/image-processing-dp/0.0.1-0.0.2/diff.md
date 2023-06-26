# Comparing `tmp/image_processing_dp-0.0.1.tar.gz` & `tmp/image_processing_dp-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "image_processing_dp-0.0.1.tar", last modified: Mon Jun 26 02:56:34 2023, max compression
+gzip compressed data, was "image_processing_dp-0.0.2.tar", last modified: Mon Jun 26 03:05:07 2023, max compression
```

## Comparing `image_processing_dp-0.0.1.tar` & `image_processing_dp-0.0.2.tar`

### file list

```diff
@@ -1,22 +1,22 @@
-drwxrwxrwx   0        0        0        0 2023-06-26 02:56:34.816192 image_processing_dp-0.0.1/
--rw-rw-rw-   0        0        0     1084 2023-06-26 02:38:55.000000 image_processing_dp-0.0.1/LICENSE
--rw-rw-rw-   0        0        0      847 2023-06-26 02:56:34.815192 image_processing_dp-0.0.1/PKG-INFO
--rw-rw-rw-   0        0        0      502 2023-06-26 02:55:00.000000 image_processing_dp-0.0.1/README.md
-drwxrwxrwx   0        0        0        0 2023-06-26 02:56:34.765189 image_processing_dp-0.0.1/image_processing_dp/
--rw-rw-rw-   0        0        0        0 2022-02-28 21:38:11.000000 image_processing_dp-0.0.1/image_processing_dp/__init__.py
-drwxrwxrwx   0        0        0        0 2023-06-26 02:56:34.796191 image_processing_dp-0.0.1/image_processing_dp/turn/
--rw-rw-rw-   0        0        0        0 2022-02-28 21:38:11.000000 image_processing_dp-0.0.1/image_processing_dp/turn/__init__.py
--rw-rw-rw-   0        0        0      797 2023-06-26 01:39:23.000000 image_processing_dp-0.0.1/image_processing_dp/turn/combination.py
--rw-rw-rw-   0        0        0      351 2023-06-26 01:40:04.000000 image_processing_dp-0.0.1/image_processing_dp/turn/transformation.py
-drwxrwxrwx   0        0        0        0 2023-06-26 02:56:34.809191 image_processing_dp-0.0.1/image_processing_dp/utility/
--rw-rw-rw-   0        0        0        0 2022-02-28 21:38:11.000000 image_processing_dp-0.0.1/image_processing_dp/utility/__init__.py
--rw-rw-rw-   0        0        0      200 2023-06-26 01:37:52.000000 image_processing_dp-0.0.1/image_processing_dp/utility/io.py
--rw-rw-rw-   0        0        0     1006 2023-06-26 01:38:24.000000 image_processing_dp-0.0.1/image_processing_dp/utility/plot.py
-drwxrwxrwx   0        0        0        0 2023-06-26 02:56:34.784190 image_processing_dp-0.0.1/image_processing_dp.egg-info/
--rw-rw-rw-   0        0        0      847 2023-06-26 02:56:34.000000 image_processing_dp-0.0.1/image_processing_dp.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      502 2023-06-26 02:56:34.000000 image_processing_dp-0.0.1/image_processing_dp.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-26 02:56:34.000000 image_processing_dp-0.0.1/image_processing_dp.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       39 2023-06-26 02:56:34.000000 image_processing_dp-0.0.1/image_processing_dp.egg-info/requires.txt
--rw-rw-rw-   0        0        0       20 2023-06-26 02:56:34.000000 image_processing_dp-0.0.1/image_processing_dp.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-06-26 02:56:34.818192 image_processing_dp-0.0.1/setup.cfg
--rw-rw-rw-   0        0        0      627 2023-06-26 02:51:19.000000 image_processing_dp-0.0.1/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-26 03:05:07.525517 image_processing_dp-0.0.2/
+-rw-rw-rw-   0        0        0     1084 2023-06-26 02:38:55.000000 image_processing_dp-0.0.2/LICENSE
+-rw-rw-rw-   0        0        0      847 2023-06-26 03:05:07.523517 image_processing_dp-0.0.2/PKG-INFO
+-rw-rw-rw-   0        0        0      502 2023-06-26 02:55:00.000000 image_processing_dp-0.0.2/README.md
+drwxrwxrwx   0        0        0        0 2023-06-26 03:05:07.488515 image_processing_dp-0.0.2/image_processing_dp/
+-rw-rw-rw-   0        0        0        0 2022-02-28 21:38:11.000000 image_processing_dp-0.0.2/image_processing_dp/__init__.py
+drwxrwxrwx   0        0        0        0 2023-06-26 03:05:07.511516 image_processing_dp-0.0.2/image_processing_dp/turn/
+-rw-rw-rw-   0        0        0        0 2022-02-28 21:38:11.000000 image_processing_dp-0.0.2/image_processing_dp/turn/__init__.py
+-rw-rw-rw-   0        0        0      797 2023-06-26 01:39:23.000000 image_processing_dp-0.0.2/image_processing_dp/turn/combination.py
+-rw-rw-rw-   0        0        0      351 2023-06-26 01:40:04.000000 image_processing_dp-0.0.2/image_processing_dp/turn/transformation.py
+drwxrwxrwx   0        0        0        0 2023-06-26 03:05:07.519517 image_processing_dp-0.0.2/image_processing_dp/utility/
+-rw-rw-rw-   0        0        0        0 2022-02-28 21:38:11.000000 image_processing_dp-0.0.2/image_processing_dp/utility/__init__.py
+-rw-rw-rw-   0        0        0      200 2023-06-26 01:37:52.000000 image_processing_dp-0.0.2/image_processing_dp/utility/io.py
+-rw-rw-rw-   0        0        0     1006 2023-06-26 01:38:24.000000 image_processing_dp-0.0.2/image_processing_dp/utility/plot.py
+drwxrwxrwx   0        0        0        0 2023-06-26 03:05:07.503516 image_processing_dp-0.0.2/image_processing_dp.egg-info/
+-rw-rw-rw-   0        0        0      847 2023-06-26 03:05:07.000000 image_processing_dp-0.0.2/image_processing_dp.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      502 2023-06-26 03:05:07.000000 image_processing_dp-0.0.2/image_processing_dp.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-26 03:05:07.000000 image_processing_dp-0.0.2/image_processing_dp.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       38 2023-06-26 03:05:07.000000 image_processing_dp-0.0.2/image_processing_dp.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       20 2023-06-26 03:05:07.000000 image_processing_dp-0.0.2/image_processing_dp.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-06-26 03:05:07.527517 image_processing_dp-0.0.2/setup.cfg
+-rw-rw-rw-   0        0        0      627 2023-06-26 03:04:17.000000 image_processing_dp-0.0.2/setup.py
```

### Comparing `image_processing_dp-0.0.1/LICENSE` & `image_processing_dp-0.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `image_processing_dp-0.0.1/PKG-INFO` & `image_processing_dp-0.0.2/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: image_processing_dp
-Version: 0.0.1
+Version: 0.0.2
 Summary: Pacote para processar imagens usando Skimage
 Home-page: https://github.com/DanilloSouza03/Pacote-de-processar-imagens
 Author: Danillo Souza Pereira
 Requires-Python: >=3.5
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

### Comparing `image_processing_dp-0.0.1/image_processing_dp/turn/combination.py` & `image_processing_dp-0.0.2/image_processing_dp/turn/combination.py`

 * *Files identical despite different names*

### Comparing `image_processing_dp-0.0.1/image_processing_dp/utility/plot.py` & `image_processing_dp-0.0.2/image_processing_dp/utility/plot.py`

 * *Files identical despite different names*

### Comparing `image_processing_dp-0.0.1/image_processing_dp.egg-info/PKG-INFO` & `image_processing_dp-0.0.2/image_processing_dp.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: image-processing-dp
-Version: 0.0.1
+Version: 0.0.2
 Summary: Pacote para processar imagens usando Skimage
 Home-page: https://github.com/DanilloSouza03/Pacote-de-processar-imagens
 Author: Danillo Souza Pereira
 Requires-Python: >=3.5
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

### Comparing `image_processing_dp-0.0.1/setup.py` & `image_processing_dp-0.0.2/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -4,15 +4,15 @@
     page_description = f.read()
 
 with open("requirements.txt") as f:
     requirements = f.read().splitlines()
 
 setup(
     name="image_processing_dp",
-    version="0.0.1",
+    version="0.0.2",
     author="Danillo Souza Pereira",
     description="Pacote para processar imagens usando Skimage",
     long_description=page_description,
     long_description_content_type="text/markdown",
     url="https://github.com/DanilloSouza03/Pacote-de-processar-imagens",
     packages=find_packages(),
     install_requires=requirements,
```

