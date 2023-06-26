# Comparing `tmp/kedro_fast_api-0.6.0.tar.gz` & `tmp/kedro_fast_api-0.6.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "kedro_fast_api-0.6.0.tar", last modified: Fri Aug 26 17:46:37 2022, max compression
+gzip compressed data, was "kedro_fast_api-0.6.1.tar", last modified: Mon Jun 26 18:12:33 2023, max compression
```

## Comparing `kedro_fast_api-0.6.0.tar` & `kedro_fast_api-0.6.1.tar`

### file list

```diff
@@ -1,39 +1,39 @@
-drwxrwxrwx   0 root         (0) root         (0)        0 2022-08-26 17:46:37.173240 kedro_fast_api-0.6.0/
--rw-rw-rw-   0 root         (0) root         (0)     1056 2022-08-26 17:46:27.000000 kedro_fast_api-0.6.0/LICENSE.txt
--rw-rw-rw-   0 root         (0) root         (0)      474 2022-08-26 17:46:27.000000 kedro_fast_api-0.6.0/MANIFEST.in
--rw-rw-rw-   0 root         (0) root         (0)     1031 2022-08-26 17:46:37.173240 kedro_fast_api-0.6.0/PKG-INFO
--rw-rw-rw-   0 root         (0) root         (0)     5572 2022-08-26 17:46:27.000000 kedro_fast_api-0.6.0/README.md
-drwxrwxrwx   0 root         (0) root         (0)        0 2022-08-26 17:46:37.169240 kedro_fast_api-0.6.0/kedro_fast_api/
--rw-rw-rw-   0 root         (0) root         (0)        0 2022-08-26 17:46:27.000000 kedro_fast_api-0.6.0/kedro_fast_api/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)      722 2022-08-26 17:46:27.000000 kedro_fast_api-0.6.0/kedro_fast_api/api_factory.py
-drwxrwxrwx   0 root         (0) root         (0)        0 2022-08-26 17:46:37.173240 kedro_fast_api-0.6.0/kedro_fast_api/docker_files/
--rw-rw-rw-   0 root         (0) root         (0)      428 2022-08-26 17:46:27.000000 kedro_fast_api-0.6.0/kedro_fast_api/docker_files/.dockerignore
--rw-rw-rw-   0 root         (0) root         (0)      770 2022-08-26 17:46:27.000000 kedro_fast_api-0.6.0/kedro_fast_api/docker_files/Dockerfile
--rw-rw-rw-   0 root         (0) root         (0)      742 2022-08-26 17:46:27.000000 kedro_fast_api-0.6.0/kedro_fast_api/docker_files/create_credentials_in_kedro.py
--rw-rw-rw-   0 root         (0) root         (0)      404 2022-08-26 17:46:27.000000 kedro_fast_api-0.6.0/kedro_fast_api/dockerfile_generator.py
-drwxrwxrwx   0 root         (0) root         (0)        0 2022-08-26 17:46:37.173240 kedro_fast_api-0.6.0/kedro_fast_api/init_files/
--rw-rw-rw-   0 root         (0) root         (0)     1186 2022-08-26 17:46:27.000000 kedro_fast_api-0.6.0/kedro_fast_api/init_files/api.yml
-drwxrwxrwx   0 root         (0) root         (0)        0 2022-08-26 17:46:37.173240 kedro_fast_api-0.6.0/kedro_fast_api/init_files/api_pipeline/
--rw-rw-rw-   0 root         (0) root         (0)       46 2022-08-26 17:46:27.000000 kedro_fast_api-0.6.0/kedro_fast_api/init_files/api_pipeline/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)      359 2022-08-26 17:46:27.000000 kedro_fast_api-0.6.0/kedro_fast_api/init_files/api_pipeline/nodes.py
--rw-rw-rw-   0 root         (0) root         (0)      365 2022-08-26 17:46:27.000000 kedro_fast_api-0.6.0/kedro_fast_api/init_files/api_pipeline/pipeline.py
--rw-rw-rw-   0 root         (0) root         (0)      108 2022-08-26 17:46:27.000000 kedro_fast_api-0.6.0/kedro_fast_api/init_files/catalog.yml
--rw-rw-rw-   0 root         (0) root         (0)      820 2022-08-26 17:46:27.000000 kedro_fast_api-0.6.0/kedro_fast_api/init_files.py
-drwxrwxrwx   0 root         (0) root         (0)        0 2022-08-26 17:46:37.173240 kedro_fast_api-0.6.0/kedro_fast_api/models/
--rw-rw-rw-   0 root         (0) root         (0)        0 2022-08-26 17:46:27.000000 kedro_fast_api-0.6.0/kedro_fast_api/models/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)      165 2022-08-26 17:46:27.000000 kedro_fast_api-0.6.0/kedro_fast_api/models/config.py
--rw-rw-rw-   0 root         (0) root         (0)      958 2022-08-26 17:46:27.000000 kedro_fast_api-0.6.0/kedro_fast_api/models/config_parser.py
--rw-rw-rw-   0 root         (0) root         (0)     1966 2022-08-26 17:46:27.000000 kedro_fast_api-0.6.0/kedro_fast_api/plugin.py
-drwxrwxrwx   0 root         (0) root         (0)        0 2022-08-26 17:46:37.173240 kedro_fast_api-0.6.0/kedro_fast_api/templates/
--rw-rw-rw-   0 root         (0) root         (0)     4102 2022-08-26 17:46:27.000000 kedro_fast_api-0.6.0/kedro_fast_api/templates/api_template.j2
--rw-rw-rw-   0 root         (0) root         (0)      111 2022-08-26 17:46:27.000000 kedro_fast_api-0.6.0/kedro_fast_api/utils.py
-drwxrwxrwx   0 root         (0) root         (0)        0 2022-08-26 17:46:37.169240 kedro_fast_api-0.6.0/kedro_fast_api.egg-info/
--rw-rw-rw-   0 root         (0) root         (0)     1031 2022-08-26 17:46:37.000000 kedro_fast_api-0.6.0/kedro_fast_api.egg-info/PKG-INFO
--rw-rw-rw-   0 root         (0) root         (0)     1001 2022-08-26 17:46:37.000000 kedro_fast_api-0.6.0/kedro_fast_api.egg-info/SOURCES.txt
--rw-rw-rw-   0 root         (0) root         (0)        1 2022-08-26 17:46:37.000000 kedro_fast_api-0.6.0/kedro_fast_api.egg-info/dependency_links.txt
--rw-rw-rw-   0 root         (0) root         (0)      124 2022-08-26 17:46:37.000000 kedro_fast_api-0.6.0/kedro_fast_api.egg-info/entry_points.txt
--rw-rw-rw-   0 root         (0) root         (0)        1 2022-08-26 17:46:37.000000 kedro_fast_api-0.6.0/kedro_fast_api.egg-info/not-zip-safe
--rw-rw-rw-   0 root         (0) root         (0)       42 2022-08-26 17:46:37.000000 kedro_fast_api-0.6.0/kedro_fast_api.egg-info/requires.txt
--rw-rw-rw-   0 root         (0) root         (0)       15 2022-08-26 17:46:37.000000 kedro_fast_api-0.6.0/kedro_fast_api.egg-info/top_level.txt
--rw-rw-rw-   0 root         (0) root         (0)      507 2022-08-26 17:46:37.173240 kedro_fast_api-0.6.0/setup.cfg
--rw-rw-rw-   0 root         (0) root         (0)     1759 2022-08-26 17:46:27.000000 kedro_fast_api-0.6.0/setup.py
+drwxrwxrwx   0 root         (0) root         (0)        0 2023-06-26 18:12:33.532401 kedro_fast_api-0.6.1/
+-rw-rw-rw-   0 root         (0) root         (0)     1056 2023-06-26 18:12:22.000000 kedro_fast_api-0.6.1/LICENSE.txt
+-rw-rw-rw-   0 root         (0) root         (0)      474 2023-06-26 18:12:22.000000 kedro_fast_api-0.6.1/MANIFEST.in
+-rw-rw-rw-   0 root         (0) root         (0)     1031 2023-06-26 18:12:33.532401 kedro_fast_api-0.6.1/PKG-INFO
+-rw-rw-rw-   0 root         (0) root         (0)     5572 2023-06-26 18:12:22.000000 kedro_fast_api-0.6.1/README.md
+drwxrwxrwx   0 root         (0) root         (0)        0 2023-06-26 18:12:33.528401 kedro_fast_api-0.6.1/kedro_fast_api/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-06-26 18:12:22.000000 kedro_fast_api-0.6.1/kedro_fast_api/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)      722 2023-06-26 18:12:22.000000 kedro_fast_api-0.6.1/kedro_fast_api/api_factory.py
+drwxrwxrwx   0 root         (0) root         (0)        0 2023-06-26 18:12:33.532401 kedro_fast_api-0.6.1/kedro_fast_api/docker_files/
+-rw-rw-rw-   0 root         (0) root         (0)      428 2023-06-26 18:12:22.000000 kedro_fast_api-0.6.1/kedro_fast_api/docker_files/.dockerignore
+-rw-rw-rw-   0 root         (0) root         (0)      770 2023-06-26 18:12:22.000000 kedro_fast_api-0.6.1/kedro_fast_api/docker_files/Dockerfile
+-rw-rw-rw-   0 root         (0) root         (0)      742 2023-06-26 18:12:22.000000 kedro_fast_api-0.6.1/kedro_fast_api/docker_files/create_credentials_in_kedro.py
+-rw-rw-rw-   0 root         (0) root         (0)      404 2023-06-26 18:12:22.000000 kedro_fast_api-0.6.1/kedro_fast_api/dockerfile_generator.py
+drwxrwxrwx   0 root         (0) root         (0)        0 2023-06-26 18:12:33.532401 kedro_fast_api-0.6.1/kedro_fast_api/init_files/
+-rw-rw-rw-   0 root         (0) root         (0)     1186 2023-06-26 18:12:22.000000 kedro_fast_api-0.6.1/kedro_fast_api/init_files/api.yml
+drwxrwxrwx   0 root         (0) root         (0)        0 2023-06-26 18:12:33.532401 kedro_fast_api-0.6.1/kedro_fast_api/init_files/api_pipeline/
+-rw-rw-rw-   0 root         (0) root         (0)       46 2023-06-26 18:12:22.000000 kedro_fast_api-0.6.1/kedro_fast_api/init_files/api_pipeline/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)      359 2023-06-26 18:12:22.000000 kedro_fast_api-0.6.1/kedro_fast_api/init_files/api_pipeline/nodes.py
+-rw-rw-rw-   0 root         (0) root         (0)      365 2023-06-26 18:12:22.000000 kedro_fast_api-0.6.1/kedro_fast_api/init_files/api_pipeline/pipeline.py
+-rw-rw-rw-   0 root         (0) root         (0)      108 2023-06-26 18:12:22.000000 kedro_fast_api-0.6.1/kedro_fast_api/init_files/catalog.yml
+-rw-rw-rw-   0 root         (0) root         (0)      820 2023-06-26 18:12:22.000000 kedro_fast_api-0.6.1/kedro_fast_api/init_files.py
+drwxrwxrwx   0 root         (0) root         (0)        0 2023-06-26 18:12:33.532401 kedro_fast_api-0.6.1/kedro_fast_api/models/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-06-26 18:12:22.000000 kedro_fast_api-0.6.1/kedro_fast_api/models/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)      165 2023-06-26 18:12:22.000000 kedro_fast_api-0.6.1/kedro_fast_api/models/config.py
+-rw-rw-rw-   0 root         (0) root         (0)      958 2023-06-26 18:12:22.000000 kedro_fast_api-0.6.1/kedro_fast_api/models/config_parser.py
+-rw-rw-rw-   0 root         (0) root         (0)     1966 2023-06-26 18:12:22.000000 kedro_fast_api-0.6.1/kedro_fast_api/plugin.py
+drwxrwxrwx   0 root         (0) root         (0)        0 2023-06-26 18:12:33.532401 kedro_fast_api-0.6.1/kedro_fast_api/templates/
+-rw-rw-rw-   0 root         (0) root         (0)     4102 2023-06-26 18:12:22.000000 kedro_fast_api-0.6.1/kedro_fast_api/templates/api_template.j2
+-rw-rw-rw-   0 root         (0) root         (0)      111 2023-06-26 18:12:22.000000 kedro_fast_api-0.6.1/kedro_fast_api/utils.py
+drwxrwxrwx   0 root         (0) root         (0)        0 2023-06-26 18:12:33.532401 kedro_fast_api-0.6.1/kedro_fast_api.egg-info/
+-rw-rw-rw-   0 root         (0) root         (0)     1031 2023-06-26 18:12:33.000000 kedro_fast_api-0.6.1/kedro_fast_api.egg-info/PKG-INFO
+-rw-rw-rw-   0 root         (0) root         (0)     1001 2023-06-26 18:12:33.000000 kedro_fast_api-0.6.1/kedro_fast_api.egg-info/SOURCES.txt
+-rw-rw-rw-   0 root         (0) root         (0)        1 2023-06-26 18:12:33.000000 kedro_fast_api-0.6.1/kedro_fast_api.egg-info/dependency_links.txt
+-rw-rw-rw-   0 root         (0) root         (0)      124 2023-06-26 18:12:33.000000 kedro_fast_api-0.6.1/kedro_fast_api.egg-info/entry_points.txt
+-rw-rw-rw-   0 root         (0) root         (0)        1 2023-06-26 18:12:33.000000 kedro_fast_api-0.6.1/kedro_fast_api.egg-info/not-zip-safe
+-rw-rw-rw-   0 root         (0) root         (0)       41 2023-06-26 18:12:33.000000 kedro_fast_api-0.6.1/kedro_fast_api.egg-info/requires.txt
+-rw-rw-rw-   0 root         (0) root         (0)       15 2023-06-26 18:12:33.000000 kedro_fast_api-0.6.1/kedro_fast_api.egg-info/top_level.txt
+-rw-rw-rw-   0 root         (0) root         (0)      507 2023-06-26 18:12:33.532401 kedro_fast_api-0.6.1/setup.cfg
+-rw-rw-rw-   0 root         (0) root         (0)     1758 2023-06-26 18:12:22.000000 kedro_fast_api-0.6.1/setup.py
```

### Comparing `kedro_fast_api-0.6.0/LICENSE.txt` & `kedro_fast_api-0.6.1/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `kedro_fast_api-0.6.0/PKG-INFO` & `kedro_fast_api-0.6.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: kedro_fast_api
-Version: 0.6.0
+Version: 0.6.1
 Summary: API to run pickle models with kedro.
 Home-page: https://bitbucket.org/indiciumtech/kedro_fast_api
 Author: Artur Wagner
 Author-email: artur.wagner@indicium.tech
 License: Apache Software License 2.0
 Download-URL: https://bitbucket.org/indiciumtech/kedro_fast_api/get/master.zip
 Keywords: kedro_fast_api
```

### Comparing `kedro_fast_api-0.6.0/README.md` & `kedro_fast_api-0.6.1/README.md`

 * *Files identical despite different names*

### Comparing `kedro_fast_api-0.6.0/kedro_fast_api/api_factory.py` & `kedro_fast_api-0.6.1/kedro_fast_api/api_factory.py`

 * *Files identical despite different names*

### Comparing `kedro_fast_api-0.6.0/kedro_fast_api/docker_files/Dockerfile` & `kedro_fast_api-0.6.1/kedro_fast_api/docker_files/Dockerfile`

 * *Files identical despite different names*

### Comparing `kedro_fast_api-0.6.0/kedro_fast_api/docker_files/create_credentials_in_kedro.py` & `kedro_fast_api-0.6.1/kedro_fast_api/docker_files/create_credentials_in_kedro.py`

 * *Files identical despite different names*

### Comparing `kedro_fast_api-0.6.0/kedro_fast_api/init_files/api.yml` & `kedro_fast_api-0.6.1/kedro_fast_api/init_files/api.yml`

 * *Files identical despite different names*

### Comparing `kedro_fast_api-0.6.0/kedro_fast_api/init_files.py` & `kedro_fast_api-0.6.1/kedro_fast_api/init_files.py`

 * *Files identical despite different names*

### Comparing `kedro_fast_api-0.6.0/kedro_fast_api/models/config_parser.py` & `kedro_fast_api-0.6.1/kedro_fast_api/models/config_parser.py`

 * *Files identical despite different names*

### Comparing `kedro_fast_api-0.6.0/kedro_fast_api/plugin.py` & `kedro_fast_api-0.6.1/kedro_fast_api/plugin.py`

 * *Files identical despite different names*

### Comparing `kedro_fast_api-0.6.0/kedro_fast_api/templates/api_template.j2` & `kedro_fast_api-0.6.1/kedro_fast_api/templates/api_template.j2`

 * *Files identical despite different names*

### Comparing `kedro_fast_api-0.6.0/kedro_fast_api.egg-info/PKG-INFO` & `kedro_fast_api-0.6.1/kedro_fast_api.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: kedro-fast-api
-Version: 0.6.0
+Version: 0.6.1
 Summary: API to run pickle models with kedro.
 Home-page: https://bitbucket.org/indiciumtech/kedro_fast_api
 Author: Artur Wagner
 Author-email: artur.wagner@indicium.tech
 License: Apache Software License 2.0
 Download-URL: https://bitbucket.org/indiciumtech/kedro_fast_api/get/master.zip
 Keywords: kedro_fast_api
```

### Comparing `kedro_fast_api-0.6.0/kedro_fast_api.egg-info/SOURCES.txt` & `kedro_fast_api-0.6.1/kedro_fast_api.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `kedro_fast_api-0.6.0/setup.py` & `kedro_fast_api-0.6.1/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 from setuptools import setup, find_packages
 
 requirements = [
     'fastapi',
     'click',
     'uvicorn',
     'pyyaml',
-    'kedro>=-0.16'
+    'kedro>=0.16'
 ]
 
 setup_requirements = [ ]
 
 test_requirements = [ ]
 
 setup(
@@ -48,10 +48,10 @@
     keywords='kedro_fast_api',
     name='kedro_fast_api',
     packages=find_packages(include=['kedro_fast_api', 'kedro_fast_api.*']),
     setup_requires=setup_requirements,
     test_suite='tests',
     tests_require=test_requirements,
     url='https://bitbucket.org/indiciumtech/kedro_fast_api',
-    version='0.6.0',
+    version='0.6.1',
     zip_safe=False,
 )
```

