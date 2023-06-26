# Comparing `tmp/pyegt-0.0.2.tar.gz` & `tmp/pyegt-0.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyegt-0.0.2.tar", last modified: Mon Jun 26 11:54:00 2023, max compression
+gzip compressed data, was "pyegt-0.1.0.tar", last modified: Mon Jun 26 12:31:14 2023, max compression
```

## Comparing `pyegt-0.0.2.tar` & `pyegt-0.1.0.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxr-xr-x   0 iannesbitt   (501) staff       (20)        0 2023-06-26 11:54:00.283494 pyegt-0.0.2/
--rw-r--r--   0 iannesbitt   (501) staff       (20)    11357 2023-06-15 22:22:38.000000 pyegt-0.0.2/LICENSE
--rw-r--r--   0 iannesbitt   (501) staff       (20)     2737 2023-06-26 11:54:00.283334 pyegt-0.0.2/PKG-INFO
--rw-r--r--   0 iannesbitt   (501) staff       (20)     2043 2023-06-25 17:41:45.000000 pyegt-0.0.2/README.md
-drwxr-xr-x   0 iannesbitt   (501) staff       (20)        0 2023-06-26 11:54:00.282393 pyegt-0.0.2/pyegt/
--rw-r--r--   0 iannesbitt   (501) staff       (20)        0 2023-06-15 22:18:10.000000 pyegt-0.0.2/pyegt/__init__.py
--rw-r--r--   0 iannesbitt   (501) staff       (20)       21 2023-06-26 11:38:49.000000 pyegt-0.0.2/pyegt/_version.py
--rw-r--r--   0 iannesbitt   (501) staff       (20)     2853 2023-06-25 16:39:53.000000 pyegt-0.0.2/pyegt/defs.py
--rw-r--r--   0 iannesbitt   (501) staff       (20)    12502 2023-06-25 18:11:54.000000 pyegt-0.0.2/pyegt/height.py
--rw-r--r--   0 iannesbitt   (501) staff       (20)     1264 2023-06-25 18:10:51.000000 pyegt-0.0.2/pyegt/test.py
--rw-r--r--   0 iannesbitt   (501) staff       (20)     8367 2023-06-25 17:58:50.000000 pyegt-0.0.2/pyegt/utils.py
-drwxr-xr-x   0 iannesbitt   (501) staff       (20)        0 2023-06-26 11:54:00.283123 pyegt-0.0.2/pyegt.egg-info/
--rw-r--r--   0 iannesbitt   (501) staff       (20)     2737 2023-06-26 11:54:00.000000 pyegt-0.0.2/pyegt.egg-info/PKG-INFO
--rw-r--r--   0 iannesbitt   (501) staff       (20)      297 2023-06-26 11:54:00.000000 pyegt-0.0.2/pyegt.egg-info/SOURCES.txt
--rw-r--r--   0 iannesbitt   (501) staff       (20)        1 2023-06-26 11:54:00.000000 pyegt-0.0.2/pyegt.egg-info/dependency_links.txt
--rw-r--r--   0 iannesbitt   (501) staff       (20)       47 2023-06-26 11:54:00.000000 pyegt-0.0.2/pyegt.egg-info/entry_points.txt
--rw-r--r--   0 iannesbitt   (501) staff       (20)       23 2023-06-26 11:54:00.000000 pyegt-0.0.2/pyegt.egg-info/requires.txt
--rw-r--r--   0 iannesbitt   (501) staff       (20)        6 2023-06-26 11:54:00.000000 pyegt-0.0.2/pyegt.egg-info/top_level.txt
--rw-r--r--   0 iannesbitt   (501) staff       (20)       38 2023-06-26 11:54:00.283535 pyegt-0.0.2/setup.cfg
--rw-r--r--   0 iannesbitt   (501) staff       (20)     1165 2023-06-25 17:48:43.000000 pyegt-0.0.2/setup.py
+drwxr-xr-x   0 iannesbitt   (501) staff       (20)        0 2023-06-26 12:31:14.723014 pyegt-0.1.0/
+-rw-r--r--   0 iannesbitt   (501) staff       (20)    11357 2023-06-15 22:22:38.000000 pyegt-0.1.0/LICENSE
+-rw-r--r--   0 iannesbitt   (501) staff       (20)     2865 2023-06-26 12:31:14.722872 pyegt-0.1.0/PKG-INFO
+-rw-r--r--   0 iannesbitt   (501) staff       (20)     2173 2023-06-26 12:26:30.000000 pyegt-0.1.0/README.md
+drwxr-xr-x   0 iannesbitt   (501) staff       (20)        0 2023-06-26 12:31:14.721832 pyegt-0.1.0/pyegt/
+-rw-r--r--   0 iannesbitt   (501) staff       (20)        0 2023-06-15 22:18:10.000000 pyegt-0.1.0/pyegt/__init__.py
+-rw-r--r--   0 iannesbitt   (501) staff       (20)       21 2023-06-26 12:28:01.000000 pyegt-0.1.0/pyegt/_version.py
+-rw-r--r--   0 iannesbitt   (501) staff       (20)     2853 2023-06-25 16:39:53.000000 pyegt-0.1.0/pyegt/defs.py
+-rw-r--r--   0 iannesbitt   (501) staff       (20)    12502 2023-06-25 18:11:54.000000 pyegt-0.1.0/pyegt/height.py
+-rw-r--r--   0 iannesbitt   (501) staff       (20)     1264 2023-06-25 18:10:51.000000 pyegt-0.1.0/pyegt/test.py
+-rw-r--r--   0 iannesbitt   (501) staff       (20)     8367 2023-06-25 17:58:50.000000 pyegt-0.1.0/pyegt/utils.py
+drwxr-xr-x   0 iannesbitt   (501) staff       (20)        0 2023-06-26 12:31:14.722639 pyegt-0.1.0/pyegt.egg-info/
+-rw-r--r--   0 iannesbitt   (501) staff       (20)     2865 2023-06-26 12:31:14.000000 pyegt-0.1.0/pyegt.egg-info/PKG-INFO
+-rw-r--r--   0 iannesbitt   (501) staff       (20)      297 2023-06-26 12:31:14.000000 pyegt-0.1.0/pyegt.egg-info/SOURCES.txt
+-rw-r--r--   0 iannesbitt   (501) staff       (20)        1 2023-06-26 12:31:14.000000 pyegt-0.1.0/pyegt.egg-info/dependency_links.txt
+-rw-r--r--   0 iannesbitt   (501) staff       (20)       47 2023-06-26 12:31:14.000000 pyegt-0.1.0/pyegt.egg-info/entry_points.txt
+-rw-r--r--   0 iannesbitt   (501) staff       (20)       23 2023-06-26 12:31:14.000000 pyegt-0.1.0/pyegt.egg-info/requires.txt
+-rw-r--r--   0 iannesbitt   (501) staff       (20)        6 2023-06-26 12:31:14.000000 pyegt-0.1.0/pyegt.egg-info/top_level.txt
+-rw-r--r--   0 iannesbitt   (501) staff       (20)       38 2023-06-26 12:31:14.723055 pyegt-0.1.0/setup.cfg
+-rw-r--r--   0 iannesbitt   (501) staff       (20)     1163 2023-06-26 12:29:23.000000 pyegt-0.1.0/setup.py
```

### Comparing `pyegt-0.0.2/LICENSE` & `pyegt-0.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `pyegt-0.0.2/PKG-INFO` & `pyegt-0.1.0/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 Metadata-Version: 2.1
 Name: pyegt
-Version: 0.0.2
+Version: 0.1.0
 Summary: Look up geoid and tidal model heights relative to the ellipsoid
-Home-page: https://github.com/iannesbitt/pyegt
+Home-page: https://iannesbitt.github.io/pyegt
 Author: Ian Nesbitt
 Author-email: nesbitt@nceas.ucsb.edu
 License: Apache Software License 2.0
-Classifier: Development Status :: 3 - Alpha
+Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Education
 Classifier: Intended Audience :: Science/Research
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Natural Language :: English
 Classifier: Programming Language :: Python :: 3
 Classifier: Topic :: Scientific/Engineering :: GIS
 Requires-Python: >=3.9, <4.0
@@ -21,14 +21,15 @@
 
 **Ellipsoid-relative geoid and tidal model height lookup**
 
 *Ian Nesbitt, NCEAS-UCSB*
 
 [![PyPI](https://img.shields.io/pypi/v/pyegt)](https://pypi.org/project/pyegt)
 [![Conda](https://img.shields.io/conda/v/iannesbitt/pyegt)](https://anaconda.org/iannesbitt/readgssi)
+[![Docs](https://img.shields.io/github/deployments/iannesbitt/pyegt/github-pages?label=docs)](https://iannesbitt.github.io/pyegt)
 
 `pyegt` is an open source program developed by [NCEAS](https://nceas.ucsb.edu)
 to look up the geoid, tidal, or geopotential model height above the ellipsoid
 in order to convert model-referenced heights to ellipsoid height (i.e.
 compatible with [Cesium](https://cesium.com)) and vice-versa.
 
 ## About
```

### Comparing `pyegt-0.0.2/README.md` & `pyegt-0.1.0/README.md`

 * *Files 8% similar despite different names*

```diff
@@ -2,14 +2,15 @@
 
 **Ellipsoid-relative geoid and tidal model height lookup**
 
 *Ian Nesbitt, NCEAS-UCSB*
 
 [![PyPI](https://img.shields.io/pypi/v/pyegt)](https://pypi.org/project/pyegt)
 [![Conda](https://img.shields.io/conda/v/iannesbitt/pyegt)](https://anaconda.org/iannesbitt/readgssi)
+[![Docs](https://img.shields.io/github/deployments/iannesbitt/pyegt/github-pages?label=docs)](https://iannesbitt.github.io/pyegt)
 
 `pyegt` is an open source program developed by [NCEAS](https://nceas.ucsb.edu)
 to look up the geoid, tidal, or geopotential model height above the ellipsoid
 in order to convert model-referenced heights to ellipsoid height (i.e.
 compatible with [Cesium](https://cesium.com)) and vice-versa.
 
 ## About
```

### Comparing `pyegt-0.0.2/pyegt/defs.py` & `pyegt-0.1.0/pyegt/defs.py`

 * *Files identical despite different names*

### Comparing `pyegt-0.0.2/pyegt/height.py` & `pyegt-0.1.0/pyegt/height.py`

 * *Files identical despite different names*

### Comparing `pyegt-0.0.2/pyegt/test.py` & `pyegt-0.1.0/pyegt/test.py`

 * *Files identical despite different names*

### Comparing `pyegt-0.0.2/pyegt/utils.py` & `pyegt-0.1.0/pyegt/utils.py`

 * *Files identical despite different names*

### Comparing `pyegt-0.0.2/pyegt.egg-info/PKG-INFO` & `pyegt-0.1.0/pyegt.egg-info/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 Metadata-Version: 2.1
 Name: pyegt
-Version: 0.0.2
+Version: 0.1.0
 Summary: Look up geoid and tidal model heights relative to the ellipsoid
-Home-page: https://github.com/iannesbitt/pyegt
+Home-page: https://iannesbitt.github.io/pyegt
 Author: Ian Nesbitt
 Author-email: nesbitt@nceas.ucsb.edu
 License: Apache Software License 2.0
-Classifier: Development Status :: 3 - Alpha
+Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Education
 Classifier: Intended Audience :: Science/Research
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Natural Language :: English
 Classifier: Programming Language :: Python :: 3
 Classifier: Topic :: Scientific/Engineering :: GIS
 Requires-Python: >=3.9, <4.0
@@ -21,14 +21,15 @@
 
 **Ellipsoid-relative geoid and tidal model height lookup**
 
 *Ian Nesbitt, NCEAS-UCSB*
 
 [![PyPI](https://img.shields.io/pypi/v/pyegt)](https://pypi.org/project/pyegt)
 [![Conda](https://img.shields.io/conda/v/iannesbitt/pyegt)](https://anaconda.org/iannesbitt/readgssi)
+[![Docs](https://img.shields.io/github/deployments/iannesbitt/pyegt/github-pages?label=docs)](https://iannesbitt.github.io/pyegt)
 
 `pyegt` is an open source program developed by [NCEAS](https://nceas.ucsb.edu)
 to look up the geoid, tidal, or geopotential model height above the ellipsoid
 in order to convert model-referenced heights to ellipsoid height (i.e.
 compatible with [Cesium](https://cesium.com)) and vice-versa.
 
 ## About
```

### Comparing `pyegt-0.0.2/setup.py` & `pyegt-0.1.0/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -8,29 +8,29 @@
     author='Ian Nesbitt',
     author_email='nesbitt@nceas.ucsb.edu',
     name='pyegt',
     version=_version.__version__,
     description='Look up geoid and tidal model heights relative to the ellipsoid',
     long_description=long_description,
     long_description_content_type='text/markdown',
-    url='https://github.com/iannesbitt/pyegt',
+    url='https://iannesbitt.github.io/pyegt',
     packages=setuptools.find_packages(),
     include_package_data=True,
     install_requires=[
         'pyproj>=3.1.0',
         'requests'
     ],
     entry_points = {
         'console_scripts': [
             'pyegt-test=pyegt.test:test'
         ],
     },
     python_requires='>=3.9, <4.0',
     classifiers=[
-        'Development Status :: 3 - Alpha',
+        'Development Status :: 4 - Beta',
         'Intended Audience :: Education',
         'Intended Audience :: Science/Research',
         'License :: OSI Approved :: Apache Software License',
         'Natural Language :: English',
         'Programming Language :: Python :: 3',
         'Topic :: Scientific/Engineering :: GIS',
     ],
```

