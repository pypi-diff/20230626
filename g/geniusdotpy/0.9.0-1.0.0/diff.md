# Comparing `tmp/geniusdotpy-0.9.0.tar.gz` & `tmp/geniusdotpy-1.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "geniusdotpy-0.9.0.tar", last modified: Wed May 24 04:03:13 2023, max compression
+gzip compressed data, was "geniusdotpy-1.0.0.tar", last modified: Mon Jun 26 07:58:08 2023, max compression
```

## Comparing `geniusdotpy-0.9.0.tar` & `geniusdotpy-1.0.0.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxr-xr-x   0 joel      (1000) joel      (1000)        0 2023-05-24 04:03:13.433619 geniusdotpy-0.9.0/
--rw-r--r--   0 joel      (1000) joel      (1000)     1061 2023-05-24 03:59:34.000000 geniusdotpy-0.9.0/LICENSE
--rw-r--r--   0 joel      (1000) joel      (1000)     1957 2023-05-24 04:03:13.433619 geniusdotpy-0.9.0/PKG-INFO
--rw-r--r--   0 joel      (1000) joel      (1000)     1377 2023-05-24 03:35:41.000000 geniusdotpy-0.9.0/README.md
-drwxr-xr-x   0 joel      (1000) joel      (1000)        0 2023-05-24 04:03:13.432619 geniusdotpy-0.9.0/geniusdotpy/
--rw-r--r--   0 joel      (1000) joel      (1000)      243 2023-05-24 03:44:26.000000 geniusdotpy-0.9.0/geniusdotpy/__init__.py
--rw-r--r--   0 joel      (1000) joel      (1000)      986 2023-05-24 03:42:25.000000 geniusdotpy-0.9.0/geniusdotpy/album.py
--rw-r--r--   0 joel      (1000) joel      (1000)      652 2023-05-24 03:42:26.000000 geniusdotpy-0.9.0/geniusdotpy/artist.py
--rw-r--r--   0 joel      (1000) joel      (1000)     2991 2023-05-24 03:44:20.000000 geniusdotpy-0.9.0/geniusdotpy/genius_builder.py
--rw-r--r--   0 joel      (1000) joel      (1000)      380 2023-05-24 03:47:26.000000 geniusdotpy-0.9.0/geniusdotpy/lyrics.py
--rw-r--r--   0 joel      (1000) joel      (1000)     3360 2023-05-24 03:42:32.000000 geniusdotpy-0.9.0/geniusdotpy/track.py
--rw-r--r--   0 joel      (1000) joel      (1000)      251 2023-05-24 03:43:51.000000 geniusdotpy-0.9.0/geniusdotpy/utils.py
-drwxr-xr-x   0 joel      (1000) joel      (1000)        0 2023-05-24 04:03:13.433619 geniusdotpy-0.9.0/geniusdotpy.egg-info/
--rw-r--r--   0 joel      (1000) joel      (1000)     1957 2023-05-24 04:03:13.000000 geniusdotpy-0.9.0/geniusdotpy.egg-info/PKG-INFO
--rw-r--r--   0 joel      (1000) joel      (1000)      361 2023-05-24 04:03:13.000000 geniusdotpy-0.9.0/geniusdotpy.egg-info/SOURCES.txt
--rw-r--r--   0 joel      (1000) joel      (1000)        1 2023-05-24 04:03:13.000000 geniusdotpy-0.9.0/geniusdotpy.egg-info/dependency_links.txt
--rw-r--r--   0 joel      (1000) joel      (1000)       24 2023-05-24 04:03:13.000000 geniusdotpy-0.9.0/geniusdotpy.egg-info/requires.txt
--rw-r--r--   0 joel      (1000) joel      (1000)       12 2023-05-24 04:03:13.000000 geniusdotpy-0.9.0/geniusdotpy.egg-info/top_level.txt
--rw-r--r--   0 joel      (1000) joel      (1000)       38 2023-05-24 04:03:13.433619 geniusdotpy-0.9.0/setup.cfg
--rw-r--r--   0 joel      (1000) joel      (1000)      998 2023-05-24 04:01:26.000000 geniusdotpy-0.9.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 07:58:08.322424 geniusdotpy-1.0.0/
+-rw-r--r--   0 runner    (1001) docker     (123)     1061 2023-06-26 07:57:58.000000 geniusdotpy-1.0.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     1925 2023-06-26 07:58:08.322424 geniusdotpy-1.0.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1332 2023-06-26 07:57:58.000000 geniusdotpy-1.0.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 07:58:08.322424 geniusdotpy-1.0.0/geniusdotpy/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-26 07:57:58.000000 geniusdotpy-1.0.0/geniusdotpy/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      740 2023-06-26 07:57:58.000000 geniusdotpy-1.0.0/geniusdotpy/album.py
+-rw-r--r--   0 runner    (1001) docker     (123)      876 2023-06-26 07:57:58.000000 geniusdotpy-1.0.0/geniusdotpy/artist.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2561 2023-06-26 07:57:58.000000 geniusdotpy-1.0.0/geniusdotpy/genius_builder.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2104 2023-06-26 07:57:58.000000 geniusdotpy-1.0.0/geniusdotpy/track.py
+-rw-r--r--   0 runner    (1001) docker     (123)       61 2023-06-26 07:57:58.000000 geniusdotpy-1.0.0/geniusdotpy/typing.py
+-rw-r--r--   0 runner    (1001) docker     (123)      638 2023-06-26 07:57:58.000000 geniusdotpy-1.0.0/geniusdotpy/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 07:58:08.322424 geniusdotpy-1.0.0/geniusdotpy.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1925 2023-06-26 07:58:08.000000 geniusdotpy-1.0.0/geniusdotpy.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      361 2023-06-26 07:58:08.000000 geniusdotpy-1.0.0/geniusdotpy.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-26 07:58:08.000000 geniusdotpy-1.0.0/geniusdotpy.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       24 2023-06-26 07:58:08.000000 geniusdotpy-1.0.0/geniusdotpy.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       12 2023-06-26 07:58:08.000000 geniusdotpy-1.0.0/geniusdotpy.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-26 07:58:08.322424 geniusdotpy-1.0.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      987 2023-06-26 07:57:58.000000 geniusdotpy-1.0.0/setup.py
```

### Comparing `geniusdotpy-0.9.0/LICENSE` & `geniusdotpy-1.0.0/LICENSE`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 MIT License
 
-Copyright (c) 2022 Joel
+Copyright (c) 2023 Joel
 
 Permission is hereby granted, free of charge, to any person obtaining a copy
 of this software and associated documentation files (the "Software"), to deal
 in the Software without restriction, including without limitation the rights
 to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
 copies of the Software, and to permit persons to whom the Software is
 furnished to do so, subject to the following conditions:
```

### Comparing `geniusdotpy-0.9.0/PKG-INFO` & `geniusdotpy-1.0.0/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,37 +1,38 @@
 Metadata-Version: 2.1
 Name: geniusdotpy
-Version: 0.9.0
+Version: 1.0.0
 Summary: Python wrapper for Genius API
 Home-page: https://github.com/jjoeldaniel/genius.py
 Author: jjoeldaniel
 Author-email: <joeldanielrico@gmail.com>
 Keywords: python,genius,api-wrapper
-Classifier: Development Status :: 4 - Beta
+Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: Unix
 Classifier: Operating System :: MacOS :: MacOS X
 Classifier: Operating System :: Microsoft :: Windows
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # **genius.py**
 
 [![PyPI version](https://img.shields.io/pypi/v/geniusdotpy)](https://pypi.org/project/geniusdotpy/)
 [![Python 3.x version](https://img.shields.io/badge/python-3.x-brightgreen.svg)](https://www.python.org/downloads/)
-[![Wiki Link](https://img.shields.io/badge/wiki-documentation-forestgreen)](https://github.com/jjoeldaniel/genius.py/wiki)
+[![Documentation](https://img.shields.io/badge/documentation-8A2BE2)](https://jjoeldaniel.github.io/genius.py/)
 [![Downloads](https://static.pepy.tech/badge/geniusdotpy)](https://pepy.tech/project/geniusdotpy)
 
 > Python wrapper for Genius API
 
 With genius.py, enjoy an easy-to-use interface to interact with [Genius API](https://docs.genius.com)
 
 ## Table of Contents
 
+- [Table of Contents](#table-of-contents)
 - [Features](#features)
 - [Install](#install)
 - [Getting Started](#getting-started)
 - [References](#references)
 
 ---
 
@@ -39,15 +40,15 @@
 
 - Feature rich interface
 - Easy to use
 - Lyrics web scraper
 
 ## Install
 
-```python
+```bash
 pip install geniusdotpy
 ```
 
 ## Getting Started
 
 To get started...
 
@@ -65,12 +66,10 @@
 
 4. Profit
 
 ## References
 
 [Genius API](https://docs.genius.com)
 
-[Beautiful Soup](https://www.crummy.com/software/BeautifulSoup/bs4/doc/)
-
 ---
 
 Created with 💖 by [*jjoeldaniel*](https://github.com/jjoeldaniel)
```

### Comparing `geniusdotpy-0.9.0/README.md` & `geniusdotpy-1.0.0/README.md`

 * *Files 8% similar despite different names*

```diff
@@ -1,20 +1,21 @@
 # **genius.py**
 
 [![PyPI version](https://img.shields.io/pypi/v/geniusdotpy)](https://pypi.org/project/geniusdotpy/)
 [![Python 3.x version](https://img.shields.io/badge/python-3.x-brightgreen.svg)](https://www.python.org/downloads/)
-[![Wiki Link](https://img.shields.io/badge/wiki-documentation-forestgreen)](https://github.com/jjoeldaniel/genius.py/wiki)
+[![Documentation](https://img.shields.io/badge/documentation-8A2BE2)](https://jjoeldaniel.github.io/genius.py/)
 [![Downloads](https://static.pepy.tech/badge/geniusdotpy)](https://pepy.tech/project/geniusdotpy)
 
 > Python wrapper for Genius API
 
 With genius.py, enjoy an easy-to-use interface to interact with [Genius API](https://docs.genius.com)
 
 ## Table of Contents
 
+- [Table of Contents](#table-of-contents)
 - [Features](#features)
 - [Install](#install)
 - [Getting Started](#getting-started)
 - [References](#references)
 
 ---
 
@@ -22,15 +23,15 @@
 
 - Feature rich interface
 - Easy to use
 - Lyrics web scraper
 
 ## Install
 
-```python
+```bash
 pip install geniusdotpy
 ```
 
 ## Getting Started
 
 To get started...
 
@@ -48,12 +49,10 @@
 
 4. Profit
 
 ## References
 
 [Genius API](https://docs.genius.com)
 
-[Beautiful Soup](https://www.crummy.com/software/BeautifulSoup/bs4/doc/)
-
 ---
 
 Created with 💖 by [*jjoeldaniel*](https://github.com/jjoeldaniel)
```

### Comparing `geniusdotpy-0.9.0/geniusdotpy/album.py` & `geniusdotpy-1.0.0/geniusdotpy/album.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,37 +1,28 @@
-from geniusdotpy.utils import format_json
+from geniusdotpy.artist import Artist
 
 
 class Album:
-    def __init__(self, album_info):
+    """Album class"""
+
+    def __init__(self, album_info: dict):
         self.album_info = album_info
-        self.id = album_info["id"]
-        self.url = album_info["url"]
-        self.path = album_info["api_path"]
-
-        if "cover_art_url" in album_info:
-            self.cover_art_url = album_info["cover_art_url"]
-        else:
-            self.cover_art_url = None
-
-        # Fallback name to full_title if name is not present and vice versa
-        if "name" in album_info:
-            self.name = album_info["name"]
-        else:
-            self.name = album_info["full_title"]
+        """JSON object containing album information."""
 
-        if "full_title" in album_info:
-            self.full_title = album_info["full_title"]
-        else:
-            self.full_title = album_info["name"]
+        self.name: str = album_info["name"]
+        """Album name"""
 
-    def __str__(self):
-        return self.name
+        self.url: str = album_info["url"]
+        """Album URL"""
 
-    def to_json(self):
-        """Convert album info to JSON.
+        # Default `full_title` to name
+        self.full_title: str = album_info["name"]
+        """Album full title"""
 
-        Returns:
-            JSON object
-        """
+        # Possibly null values
+        self.artist = None
+        """Album artist"""
 
-        return format_json(self.album_info)
+        if "full_title" in album_info:
+            self.full_title = album_info["full_title"]
+        if "artist" in album_info:
+            self.artist = Artist(album_info["artist"])
```

### Comparing `geniusdotpy-0.9.0/geniusdotpy.egg-info/PKG-INFO` & `geniusdotpy-1.0.0/geniusdotpy.egg-info/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,37 +1,38 @@
 Metadata-Version: 2.1
 Name: geniusdotpy
-Version: 0.9.0
+Version: 1.0.0
 Summary: Python wrapper for Genius API
 Home-page: https://github.com/jjoeldaniel/genius.py
 Author: jjoeldaniel
 Author-email: <joeldanielrico@gmail.com>
 Keywords: python,genius,api-wrapper
-Classifier: Development Status :: 4 - Beta
+Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: Unix
 Classifier: Operating System :: MacOS :: MacOS X
 Classifier: Operating System :: Microsoft :: Windows
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # **genius.py**
 
 [![PyPI version](https://img.shields.io/pypi/v/geniusdotpy)](https://pypi.org/project/geniusdotpy/)
 [![Python 3.x version](https://img.shields.io/badge/python-3.x-brightgreen.svg)](https://www.python.org/downloads/)
-[![Wiki Link](https://img.shields.io/badge/wiki-documentation-forestgreen)](https://github.com/jjoeldaniel/genius.py/wiki)
+[![Documentation](https://img.shields.io/badge/documentation-8A2BE2)](https://jjoeldaniel.github.io/genius.py/)
 [![Downloads](https://static.pepy.tech/badge/geniusdotpy)](https://pepy.tech/project/geniusdotpy)
 
 > Python wrapper for Genius API
 
 With genius.py, enjoy an easy-to-use interface to interact with [Genius API](https://docs.genius.com)
 
 ## Table of Contents
 
+- [Table of Contents](#table-of-contents)
 - [Features](#features)
 - [Install](#install)
 - [Getting Started](#getting-started)
 - [References](#references)
 
 ---
 
@@ -39,15 +40,15 @@
 
 - Feature rich interface
 - Easy to use
 - Lyrics web scraper
 
 ## Install
 
-```python
+```bash
 pip install geniusdotpy
 ```
 
 ## Getting Started
 
 To get started...
 
@@ -65,12 +66,10 @@
 
 4. Profit
 
 ## References
 
 [Genius API](https://docs.genius.com)
 
-[Beautiful Soup](https://www.crummy.com/software/BeautifulSoup/bs4/doc/)
-
 ---
 
 Created with 💖 by [*jjoeldaniel*](https://github.com/jjoeldaniel)
```

### Comparing `geniusdotpy-0.9.0/setup.py` & `geniusdotpy-1.0.0/setup.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,15 +1,13 @@
 from setuptools import setup, find_packages
 from pathlib import Path
-import codecs
-import os
 
 this_directory = Path(__file__).parent
 
-VERSION = "0.9.0"
+VERSION = "1.0.0"
 DESCRIPTION = "Python wrapper for Genius API"
 long_description = (this_directory / "README.md").read_text()
 
 # Setting up
 setup(
     name="geniusdotpy",
     version=VERSION,
@@ -19,15 +17,15 @@
     long_description_content_type="text/markdown",
     long_description=long_description,
     url="https://github.com/jjoeldaniel/genius.py",
     packages=find_packages(),
     install_requires=["requests", "beautifulsoup4"],
     keywords=["python", "genius", "api-wrapper"],
     classifiers=[
-        "Development Status :: 4 - Beta",
+        "Development Status :: 5 - Production/Stable",
         "Intended Audience :: Developers",
         "Programming Language :: Python :: 3",
         "Operating System :: Unix",
         "Operating System :: MacOS :: MacOS X",
         "Operating System :: Microsoft :: Windows",
     ],
 )
```

