# Comparing `tmp/st_chat_message-0.2.0.tar.gz` & `tmp/st_chat_message-0.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "st_chat_message-0.2.0.tar", max compression
+gzip compressed data, was "st_chat_message-0.3.0.tar", max compression
```

## Comparing `st_chat_message-0.2.0.tar` & `st_chat_message-0.3.0.tar`

### file list

```diff
@@ -1,5 +1,81 @@
--rw-r--r--   0        0        0      551 2023-06-26 13:38:36.661562 st_chat_message-0.2.0/README.md
--rw-r--r--   0        0        0      687 2023-06-26 13:51:22.332401 st_chat_message-0.2.0/pyproject.toml
--rw-r--r--   0        0        0     3640 2023-06-26 12:52:29.784362 st_chat_message-0.2.0/st_chat_message/__init__.py
--rw-r--r--   0        0        0     1307 1970-01-01 00:00:00.000000 st_chat_message-0.2.0/setup.py
--rw-r--r--   0        0        0     1220 1970-01-01 00:00:00.000000 st_chat_message-0.2.0/PKG-INFO
+-rw-r--r--   0        0        0      551 2023-06-26 13:38:36.661562 st_chat_message-0.3.0/README.md
+-rw-r--r--   0        0        0      680 2023-06-26 14:06:27.545642 st_chat_message-0.3.0/pyproject.toml
+-rw-r--r--   0        0        0     3640 2023-06-26 12:52:29.784362 st_chat_message-0.3.0/st_chat_message/__init__.py
+-rw-r--r--   0        0        0     2648 2023-06-26 13:09:36.988142 st_chat_message-0.3.0/st_chat_message/frontend/out/404.html
+-rw-r--r--   0        0        0      361 2023-06-26 13:09:36.865876 st_chat_message-0.3.0/st_chat_message/frontend/out/_next/static/IMEkTAcHxgV58XEAbyzrE/_buildManifest.js
+-rw-r--r--   0        0        0       77 2023-06-26 13:09:36.865873 st_chat_message-0.3.0/st_chat_message/frontend/out/_next/static/IMEkTAcHxgV58XEAbyzrE/_ssgManifest.js
+-rw-r--r--   0        0        0   266404 2023-06-26 13:09:36.865583 st_chat_message-0.3.0/st_chat_message/frontend/out/_next/static/chunks/175675d1-280cba64f0247428.js
+-rw-r--r--   0        0        0   141045 2023-06-26 13:09:36.865416 st_chat_message-0.3.0/st_chat_message/frontend/out/_next/static/chunks/framework-5e8ac8dd643904dd.js
+-rw-r--r--   0        0        0    96246 2023-06-26 13:09:36.865289 st_chat_message-0.3.0/st_chat_message/frontend/out/_next/static/chunks/main-c6459c6dbdcff8e8.js
+-rw-r--r--   0        0        0      448 2023-06-26 13:09:36.870176 st_chat_message-0.3.0/st_chat_message/frontend/out/_next/static/chunks/pages/_app-345c8177130438ac.js
+-rw-r--r--   0        0        0      250 2023-06-26 13:09:36.870210 st_chat_message-0.3.0/st_chat_message/frontend/out/_next/static/chunks/pages/_error-3f6d1c55bb8051ab.js
+-rw-r--r--   0        0        0  1407017 2023-06-26 13:09:36.871418 st_chat_message-0.3.0/st_chat_message/frontend/out/_next/static/chunks/pages/index-56e240b261b33c91.js
+-rw-r--r--   0        0        0    91381 2023-06-26 13:09:36.865988 st_chat_message-0.3.0/st_chat_message/frontend/out/_next/static/chunks/polyfills-78c92fac7aa8fdd8.js
+-rw-r--r--   0        0        0     1639 2023-06-26 13:09:36.865441 st_chat_message-0.3.0/st_chat_message/frontend/out/_next/static/chunks/webpack-9d2bee59a0ebae7b.js
+-rw-r--r--   0        0        0    26985 2023-06-26 13:09:36.865688 st_chat_message-0.3.0/st_chat_message/frontend/out/_next/static/css/1f759626be541cb1.css
+-rw-r--r--   0        0        0    20655 2023-06-26 13:09:36.865776 st_chat_message-0.3.0/st_chat_message/frontend/out/_next/static/css/2c1d693913146cab.css
+-rw-r--r--   0        0        0    33516 2023-06-26 13:09:36.866332 st_chat_message-0.3.0/st_chat_message/frontend/out/_next/static/media/KaTeX_AMS-Regular.1608a09b.woff
+-rw-r--r--   0        0        0    63632 2023-06-26 13:09:36.866593 st_chat_message-0.3.0/st_chat_message/frontend/out/_next/static/media/KaTeX_AMS-Regular.4aafdb68.ttf
+-rw-r--r--   0        0        0    28076 2023-06-26 13:09:36.866321 st_chat_message-0.3.0/st_chat_message/frontend/out/_next/static/media/KaTeX_AMS-Regular.a79f1c31.woff2
+-rw-r--r--   0        0        0     7716 2023-06-26 13:09:36.866297 st_chat_message-0.3.0/st_chat_message/frontend/out/_next/static/media/KaTeX_Caligraphic-Bold.b6770918.woff
+-rw-r--r--   0        0        0    12368 2023-06-26 13:09:36.866568 st_chat_message-0.3.0/st_chat_message/frontend/out/_next/static/media/KaTeX_Caligraphic-Bold.cce5b8ec.ttf
+-rw-r--r--   0        0        0     6912 2023-06-26 13:09:36.866543 st_chat_message-0.3.0/st_chat_message/frontend/out/_next/static/media/KaTeX_Caligraphic-Bold.ec17d132.woff2
+-rw-r--r--   0        0        0    12344 2023-06-26 13:09:36.866591 st_chat_message-0.3.0/st_chat_message/frontend/out/_next/static/media/KaTeX_Caligraphic-Regular.07ef19e7.ttf
+-rw-r--r--   0        0        0     6908 2023-06-26 13:09:36.866749 st_chat_message-0.3.0/st_chat_message/frontend/out/_next/static/media/KaTeX_Caligraphic-Regular.55fac258.woff2
+-rw-r--r--   0        0        0     7656 2023-06-26 13:09:36.866759 st_chat_message-0.3.0/st_chat_message/frontend/out/_next/static/media/KaTeX_Caligraphic-Regular.dad44a7f.woff
+-rw-r--r--   0        0        0    13296 2023-06-26 13:09:36.866851 st_chat_message-0.3.0/st_chat_message/frontend/out/_next/static/media/KaTeX_Fraktur-Bold.9f256b85.woff
+-rw-r--r--   0        0        0    19584 2023-06-26 13:09:36.866922 st_chat_message-0.3.0/st_chat_message/frontend/out/_next/static/media/KaTeX_Fraktur-Bold.b18f59e1.ttf
+-rw-r--r--   0        0        0    11348 2023-06-26 13:09:36.866958 st_chat_message-0.3.0/st_chat_message/frontend/out/_next/static/media/KaTeX_Fraktur-Bold.d42a5579.woff2
+-rw-r--r--   0        0        0    13208 2023-06-26 13:09:36.866923 st_chat_message-0.3.0/st_chat_message/frontend/out/_next/static/media/KaTeX_Fraktur-Regular.7c187121.woff
+-rw-r--r--   0        0        0    11316 2023-06-26 13:09:36.867080 st_chat_message-0.3.0/st_chat_message/frontend/out/_next/static/media/KaTeX_Fraktur-Regular.d3c882a6.woff2
+-rw-r--r--   0        0        0    19572 2023-06-26 13:09:36.867260 st_chat_message-0.3.0/st_chat_message/frontend/out/_next/static/media/KaTeX_Fraktur-Regular.ed38e79f.ttf
+-rw-r--r--   0        0        0    51336 2023-06-26 13:09:36.867423 st_chat_message-0.3.0/st_chat_message/frontend/out/_next/static/media/KaTeX_Main-Bold.b74a1a8b.ttf
+-rw-r--r--   0        0        0    25324 2023-06-26 13:09:36.867288 st_chat_message-0.3.0/st_chat_message/frontend/out/_next/static/media/KaTeX_Main-Bold.c3fb5ac2.woff2
+-rw-r--r--   0        0        0    29912 2023-06-26 13:09:36.867457 st_chat_message-0.3.0/st_chat_message/frontend/out/_next/static/media/KaTeX_Main-Bold.d181c465.woff
+-rw-r--r--   0        0        0    16780 2023-06-26 13:09:36.867578 st_chat_message-0.3.0/st_chat_message/frontend/out/_next/static/media/KaTeX_Main-BoldItalic.6f2bb1df.woff2
+-rw-r--r--   0        0        0    32968 2023-06-26 13:09:36.867727 st_chat_message-0.3.0/st_chat_message/frontend/out/_next/static/media/KaTeX_Main-BoldItalic.70d8b0a5.ttf
+-rw-r--r--   0        0        0    19412 2023-06-26 13:09:36.867704 st_chat_message-0.3.0/st_chat_message/frontend/out/_next/static/media/KaTeX_Main-BoldItalic.e3f82f9d.woff
+-rw-r--r--   0        0        0    33580 2023-06-26 13:09:36.867707 st_chat_message-0.3.0/st_chat_message/frontend/out/_next/static/media/KaTeX_Main-Italic.47373d1e.ttf
+-rw-r--r--   0        0        0    16988 2023-06-26 13:09:36.867841 st_chat_message-0.3.0/st_chat_message/frontend/out/_next/static/media/KaTeX_Main-Italic.8916142b.woff2
+-rw-r--r--   0        0        0    19676 2023-06-26 13:09:36.867919 st_chat_message-0.3.0/st_chat_message/frontend/out/_next/static/media/KaTeX_Main-Italic.9024d815.woff
+-rw-r--r--   0        0        0    26272 2023-06-26 13:09:36.867957 st_chat_message-0.3.0/st_chat_message/frontend/out/_next/static/media/KaTeX_Main-Regular.0462f03b.woff2
+-rw-r--r--   0        0        0    30772 2023-06-26 13:09:36.868092 st_chat_message-0.3.0/st_chat_message/frontend/out/_next/static/media/KaTeX_Main-Regular.7f51fe03.woff
+-rw-r--r--   0        0        0    53580 2023-06-26 13:09:36.868228 st_chat_message-0.3.0/st_chat_message/frontend/out/_next/static/media/KaTeX_Main-Regular.b7f8fe9b.ttf
+-rw-r--r--   0        0        0    16400 2023-06-26 13:09:36.868224 st_chat_message-0.3.0/st_chat_message/frontend/out/_next/static/media/KaTeX_Math-BoldItalic.572d331f.woff2
+-rw-r--r--   0        0        0    31196 2023-06-26 13:09:36.868263 st_chat_message-0.3.0/st_chat_message/frontend/out/_next/static/media/KaTeX_Math-BoldItalic.a879cf83.ttf
+-rw-r--r--   0        0        0    18668 2023-06-26 13:09:36.868330 st_chat_message-0.3.0/st_chat_message/frontend/out/_next/static/media/KaTeX_Math-BoldItalic.f1035d8d.woff
+-rw-r--r--   0        0        0    18748 2023-06-26 13:09:36.868435 st_chat_message-0.3.0/st_chat_message/frontend/out/_next/static/media/KaTeX_Math-Italic.5295ba48.woff
+-rw-r--r--   0        0        0    31308 2023-06-26 13:09:36.868531 st_chat_message-0.3.0/st_chat_message/frontend/out/_next/static/media/KaTeX_Math-Italic.939bc644.ttf
+-rw-r--r--   0        0        0    16440 2023-06-26 13:09:36.868643 st_chat_message-0.3.0/st_chat_message/frontend/out/_next/static/media/KaTeX_Math-Italic.f28c23ac.woff2
+-rw-r--r--   0        0        0    12216 2023-06-26 13:09:36.868589 st_chat_message-0.3.0/st_chat_message/frontend/out/_next/static/media/KaTeX_SansSerif-Bold.8c5b5494.woff2
+-rw-r--r--   0        0        0    24504 2023-06-26 13:09:36.868731 st_chat_message-0.3.0/st_chat_message/frontend/out/_next/static/media/KaTeX_SansSerif-Bold.94e1e8dc.ttf
+-rw-r--r--   0        0        0    14408 2023-06-26 13:09:36.868787 st_chat_message-0.3.0/st_chat_message/frontend/out/_next/static/media/KaTeX_SansSerif-Bold.bf59d231.woff
+-rw-r--r--   0        0        0    12028 2023-06-26 13:09:36.868796 st_chat_message-0.3.0/st_chat_message/frontend/out/_next/static/media/KaTeX_SansSerif-Italic.3b1e59b3.woff2
+-rw-r--r--   0        0        0    14112 2023-06-26 13:09:36.868852 st_chat_message-0.3.0/st_chat_message/frontend/out/_next/static/media/KaTeX_SansSerif-Italic.7c9bc82b.woff
+-rw-r--r--   0        0        0    22364 2023-06-26 13:09:36.869056 st_chat_message-0.3.0/st_chat_message/frontend/out/_next/static/media/KaTeX_SansSerif-Italic.b4c20c84.ttf
+-rw-r--r--   0        0        0    12316 2023-06-26 13:09:36.869067 st_chat_message-0.3.0/st_chat_message/frontend/out/_next/static/media/KaTeX_SansSerif-Regular.74048478.woff
+-rw-r--r--   0        0        0    10344 2023-06-26 13:09:36.869013 st_chat_message-0.3.0/st_chat_message/frontend/out/_next/static/media/KaTeX_SansSerif-Regular.ba21ed5f.woff2
+-rw-r--r--   0        0        0    19436 2023-06-26 13:09:36.869223 st_chat_message-0.3.0/st_chat_message/frontend/out/_next/static/media/KaTeX_SansSerif-Regular.d4d7ba48.ttf
+-rw-r--r--   0        0        0     9644 2023-06-26 13:09:36.869293 st_chat_message-0.3.0/st_chat_message/frontend/out/_next/static/media/KaTeX_Script-Regular.03e9641d.woff2
+-rw-r--r--   0        0        0    10588 2023-06-26 13:09:36.869296 st_chat_message-0.3.0/st_chat_message/frontend/out/_next/static/media/KaTeX_Script-Regular.07505710.woff
+-rw-r--r--   0        0        0    16648 2023-06-26 13:09:36.869420 st_chat_message-0.3.0/st_chat_message/frontend/out/_next/static/media/KaTeX_Script-Regular.fe9cbbe1.ttf
+-rw-r--r--   0        0        0     6496 2023-06-26 13:09:36.869470 st_chat_message-0.3.0/st_chat_message/frontend/out/_next/static/media/KaTeX_Size1-Regular.e1e279cb.woff
+-rw-r--r--   0        0        0     5468 2023-06-26 13:09:36.869566 st_chat_message-0.3.0/st_chat_message/frontend/out/_next/static/media/KaTeX_Size1-Regular.eae34984.woff2
+-rw-r--r--   0        0        0    12228 2023-06-26 13:09:36.869586 st_chat_message-0.3.0/st_chat_message/frontend/out/_next/static/media/KaTeX_Size1-Regular.fabc004a.ttf
+-rw-r--r--   0        0        0     6188 2023-06-26 13:09:36.869589 st_chat_message-0.3.0/st_chat_message/frontend/out/_next/static/media/KaTeX_Size2-Regular.57727022.woff
+-rw-r--r--   0        0        0     5208 2023-06-26 13:09:36.869635 st_chat_message-0.3.0/st_chat_message/frontend/out/_next/static/media/KaTeX_Size2-Regular.5916a24f.woff2
+-rw-r--r--   0        0        0    11508 2023-06-26 13:09:36.869791 st_chat_message-0.3.0/st_chat_message/frontend/out/_next/static/media/KaTeX_Size2-Regular.d6b476ec.ttf
+-rw-r--r--   0        0        0     4420 2023-06-26 13:09:36.869783 st_chat_message-0.3.0/st_chat_message/frontend/out/_next/static/media/KaTeX_Size3-Regular.9acaf01c.woff
+-rw-r--r--   0        0        0     7588 2023-06-26 13:09:36.869747 st_chat_message-0.3.0/st_chat_message/frontend/out/_next/static/media/KaTeX_Size3-Regular.a144ef58.ttf
+-rw-r--r--   0        0        0     3624 2023-06-26 13:09:36.869835 st_chat_message-0.3.0/st_chat_message/frontend/out/_next/static/media/KaTeX_Size3-Regular.b4230e7e.woff2
+-rw-r--r--   0        0        0     4928 2023-06-26 13:09:36.869937 st_chat_message-0.3.0/st_chat_message/frontend/out/_next/static/media/KaTeX_Size4-Regular.10d95fd3.woff2
+-rw-r--r--   0        0        0     5980 2023-06-26 13:09:36.869965 st_chat_message-0.3.0/st_chat_message/frontend/out/_next/static/media/KaTeX_Size4-Regular.7a996c9d.woff
+-rw-r--r--   0        0        0    10364 2023-06-26 13:09:36.870008 st_chat_message-0.3.0/st_chat_message/frontend/out/_next/static/media/KaTeX_Size4-Regular.fbccdabe.ttf
+-rw-r--r--   0        0        0    16028 2023-06-26 13:09:36.870005 st_chat_message-0.3.0/st_chat_message/frontend/out/_next/static/media/KaTeX_Typewriter-Regular.6258592b.woff
+-rw-r--r--   0        0        0    13568 2023-06-26 13:09:36.870097 st_chat_message-0.3.0/st_chat_message/frontend/out/_next/static/media/KaTeX_Typewriter-Regular.a8709e36.woff2
+-rw-r--r--   0        0        0    27556 2023-06-26 13:09:36.870243 st_chat_message-0.3.0/st_chat_message/frontend/out/_next/static/media/KaTeX_Typewriter-Regular.d97aaf4a.ttf
+-rw-r--r--   0        0        0    25931 2023-06-26 13:09:36.873540 st_chat_message-0.3.0/st_chat_message/frontend/out/favicon.ico
+-rw-r--r--   0        0        0     2335 2023-06-26 13:09:36.961389 st_chat_message-0.3.0/st_chat_message/frontend/out/index.html
+-rw-r--r--   0        0        0     1101 2023-06-26 13:09:36.873299 st_chat_message-0.3.0/st_chat_message/frontend/out/vercel.svg
+-rw-r--r--   0        0        0     1659 1970-01-01 00:00:00.000000 st_chat_message-0.3.0/setup.py
+-rw-r--r--   0        0        0     1220 1970-01-01 00:00:00.000000 st_chat_message-0.3.0/PKG-INFO
```

### Comparing `st_chat_message-0.2.0/README.md` & `st_chat_message-0.3.0/README.md`

 * *Files identical despite different names*

### Comparing `st_chat_message-0.2.0/pyproject.toml` & `st_chat_message-0.3.0/pyproject.toml`

 * *Files 18% similar despite different names*

```diff
@@ -1,16 +1,14 @@
 [tool.poetry]
 name = "st-chat-message"
-version = "0.2.0"
+version = "0.3.0"
 description = "A Streamlit component to display chat messages"
 authors = ["Manolo Santos <manolo.santos@gmail.com>"]
 readme = "README.md"
-packages = [
-    { include = "st_chat_message"},
-]
+packages = [{ include = "st_chat_message"}]
 
 license = "MIT"
 
 # Only include the out directory of the frontend
 # The order of the include/exclude lists is important!
 include = ["st_chat_message/frontend/out/**"]
 exclude = ["st_chat_message/frontend/*"]
```

### Comparing `st_chat_message-0.2.0/st_chat_message/__init__.py` & `st_chat_message-0.3.0/st_chat_message/__init__.py`

 * *Files identical despite different names*

### Comparing `st_chat_message-0.2.0/setup.py` & `st_chat_message-0.3.0/setup.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,22 +1,28 @@
 # -*- coding: utf-8 -*-
 from setuptools import setup
 
 packages = \
 ['st_chat_message']
 
 package_data = \
-{'': ['*']}
+{'': ['*'],
+ 'st_chat_message': ['frontend/out/*',
+                     'frontend/out/_next/static/IMEkTAcHxgV58XEAbyzrE/*',
+                     'frontend/out/_next/static/chunks/*',
+                     'frontend/out/_next/static/chunks/pages/*',
+                     'frontend/out/_next/static/css/*',
+                     'frontend/out/_next/static/media/*']}
 
 install_requires = \
 ['streamlit>=0.63']
 
 setup_kwargs = {
     'name': 'st-chat-message',
-    'version': '0.2.0',
+    'version': '0.3.0',
     'description': 'A Streamlit component to display chat messages',
     'long_description': '# ST-CHAT-MESSAGE\n\n## Description\n\nThis is a simple chat message component for streamlit. It is based on the [streamlit-chat](https://github.com/AI-Yash/st-chat) component, trying to be as compatible as possible, but it adding a few features:\n\n- Markdown support\n- LaTeX support\n- Tables\n\n## Installation\n\n```bash\npip install st-chat-message\n```\n\nor\n\n```bash\npoetry add st-chat-message\n```\n## Usage\n\n```python\nimport streamlit as st\nfrom st_chat_message import message\n\nmessage("Hello world!", is_user=True)\nmessage("Hi")\n```\n\n![img.png](docs/img.png)',
     'author': 'Manolo Santos',
     'author_email': 'manolo.santos@gmail.com',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'None',
```

### Comparing `st_chat_message-0.2.0/PKG-INFO` & `st_chat_message-0.3.0/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: st-chat-message
-Version: 0.2.0
+Version: 0.3.0
 Summary: A Streamlit component to display chat messages
 License: MIT
 Author: Manolo Santos
 Author-email: manolo.santos@gmail.com
 Requires-Python: >=3.8, !=2.7.*, !=3.0.*, !=3.1.*, !=3.2.*, !=3.3.*, !=3.4.*, !=3.5.*, !=3.6.*, !=3.7.*
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
```

