# Comparing `tmp/wagtail_sb_imageserializer-0.3.0.tar.gz` & `tmp/wagtail_sb_imageserializer-0.4.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "wagtail_sb_imageserializer-0.3.0.tar", max compression
+gzip compressed data, was "wagtail_sb_imageserializer-0.4.0.tar", max compression
```

## Comparing `wagtail_sb_imageserializer-0.3.0.tar` & `wagtail_sb_imageserializer-0.4.0.tar`

### file list

```diff
@@ -1,15 +1,15 @@
--rw-r--r--   0        0        0      272 2023-06-22 16:35:22.192421 wagtail_sb_imageserializer-0.3.0/CHANGELOG.md
--rw-r--r--   0        0        0     1070 2023-06-22 12:48:47.544906 wagtail_sb_imageserializer-0.3.0/LICENSE.txt
--rw-r--r--   0        0        0     3707 2023-06-22 12:48:47.544906 wagtail_sb_imageserializer-0.3.0/README.md
--rw-r--r--   0        0        0     2499 2023-06-22 16:35:22.192421 wagtail_sb_imageserializer-0.3.0/pyproject.toml
--rw-r--r--   0        0        0       88 2023-06-22 12:48:47.548906 wagtail_sb_imageserializer-0.3.0/src/wagtail_sb_imageserializer/__init__.py
--rw-r--r--   0        0        0        0 2023-06-22 12:48:47.548906 wagtail_sb_imageserializer-0.3.0/src/wagtail_sb_imageserializer/admin.py
--rw-r--r--   0        0        0        0 2023-06-22 12:48:47.548906 wagtail_sb_imageserializer-0.3.0/src/wagtail_sb_imageserializer/api/__init__.py
--rw-r--r--   0        0        0     1211 2023-06-22 12:48:47.548906 wagtail_sb_imageserializer-0.3.0/src/wagtail_sb_imageserializer/api/fields.py
--rw-r--r--   0        0        0      182 2023-06-22 12:48:47.548906 wagtail_sb_imageserializer-0.3.0/src/wagtail_sb_imageserializer/apps.py
--rw-r--r--   0        0        0        0 2023-06-22 12:48:47.548906 wagtail_sb_imageserializer-0.3.0/src/wagtail_sb_imageserializer/migrations/__init__.py
--rw-r--r--   0        0        0        0 2023-06-22 12:48:47.548906 wagtail_sb_imageserializer-0.3.0/src/wagtail_sb_imageserializer/models.py
--rw-r--r--   0        0        0        0 2023-06-22 12:48:47.548906 wagtail_sb_imageserializer-0.3.0/src/wagtail_sb_imageserializer/tests.py
--rw-r--r--   0        0        0       20 2023-06-22 16:35:22.192421 wagtail_sb_imageserializer-0.3.0/src/wagtail_sb_imageserializer/version.py
--rw-r--r--   0        0        0        0 2023-06-22 12:48:47.548906 wagtail_sb_imageserializer-0.3.0/src/wagtail_sb_imageserializer/views.py
--rw-r--r--   0        0        0     5497 1970-01-01 00:00:00.000000 wagtail_sb_imageserializer-0.3.0/PKG-INFO
+-rw-r--r--   0        0        0      357 2023-06-26 02:18:28.486886 wagtail_sb_imageserializer-0.4.0/CHANGELOG.md
+-rw-r--r--   0        0        0     1070 2023-06-26 01:08:37.414092 wagtail_sb_imageserializer-0.4.0/LICENSE.txt
+-rw-r--r--   0        0        0     3965 2023-06-26 01:08:37.414092 wagtail_sb_imageserializer-0.4.0/README.md
+-rw-r--r--   0        0        0     2499 2023-06-26 02:18:28.486886 wagtail_sb_imageserializer-0.4.0/pyproject.toml
+-rw-r--r--   0        0        0       88 2023-06-26 01:08:37.418092 wagtail_sb_imageserializer-0.4.0/src/wagtail_sb_imageserializer/__init__.py
+-rw-r--r--   0        0        0        0 2023-06-26 01:08:37.418092 wagtail_sb_imageserializer-0.4.0/src/wagtail_sb_imageserializer/admin.py
+-rw-r--r--   0        0        0        0 2023-06-26 01:08:37.418092 wagtail_sb_imageserializer-0.4.0/src/wagtail_sb_imageserializer/api/__init__.py
+-rw-r--r--   0        0        0     1211 2023-06-26 01:08:37.418092 wagtail_sb_imageserializer-0.4.0/src/wagtail_sb_imageserializer/api/fields.py
+-rw-r--r--   0        0        0      182 2023-06-26 01:08:37.418092 wagtail_sb_imageserializer-0.4.0/src/wagtail_sb_imageserializer/apps.py
+-rw-r--r--   0        0        0        0 2023-06-26 01:08:37.418092 wagtail_sb_imageserializer-0.4.0/src/wagtail_sb_imageserializer/migrations/__init__.py
+-rw-r--r--   0        0        0        0 2023-06-26 01:08:37.418092 wagtail_sb_imageserializer-0.4.0/src/wagtail_sb_imageserializer/models.py
+-rw-r--r--   0        0        0        0 2023-06-26 01:08:37.418092 wagtail_sb_imageserializer-0.4.0/src/wagtail_sb_imageserializer/tests.py
+-rw-r--r--   0        0        0       20 2023-06-26 02:18:28.486886 wagtail_sb_imageserializer-0.4.0/src/wagtail_sb_imageserializer/version.py
+-rw-r--r--   0        0        0        0 2023-06-26 01:08:37.418092 wagtail_sb_imageserializer-0.4.0/src/wagtail_sb_imageserializer/views.py
+-rw-r--r--   0        0        0     5709 1970-01-01 00:00:00.000000 wagtail_sb_imageserializer-0.4.0/PKG-INFO
```

### Comparing `wagtail_sb_imageserializer-0.3.0/LICENSE.txt` & `wagtail_sb_imageserializer-0.4.0/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `wagtail_sb_imageserializer-0.3.0/README.md` & `wagtail_sb_imageserializer-0.4.0/README.md`

 * *Files 7% similar despite different names*

```diff
@@ -2,25 +2,26 @@
 
 ![PyPI - Supported versions](https://img.shields.io/pypi/pyversions/wagtail-sb-imageserializer)
 ![PyPI - Package version](https://img.shields.io/pypi/v/wagtail-sb-imageserializer)
 ![PyPI - Downloads](https://img.shields.io/pypi/dm/wagtail-sb-imageserializer)
 ![PyPI - MIT License](https://img.shields.io/pypi/l/wagtail-sb-imageserializer)
 
 [![Codacy Badge](https://app.codacy.com/project/badge/Grade/329484ea99434c708f5c8dbd611f3d35)](https://app.codacy.com/gl/softbutterfly/wagtail-sb-imageserializer/dashboard?utm_source=gl&utm_medium=referral&utm_content=&utm_campaign=Badge_grade)
+[![Codacy Coverage Badge](https://app.codacy.com/project/badge/Coverage/900411c7b5e443f89f85c7978f7504e5)](https://app.codacy.com/gl/softbutterfly/wagtail-sb-imageserializer/dashboard?utm_source=gl&utm_medium=referral&utm_content=&utm_campaign=Badge_coverage)
 
 # Wagtail Image Serializer
 
 Wagtail package to render images with rendition in a single API Field.
 
 ## Requirements
 
 - Python 3.8.1 or higher
-- Django lower than 4.0
-- Wagtail lower than 6.0
-- Django Rest Framework lower than 4.0
+- Wagtail 3.0 or higher
+- Django 3.2 or higher
+- Django Rest Framework 3.13 or higher
 
 ## Install
 
 ```bash
 pip install wagtail-sb-imageserializer
 ```
```

### Comparing `wagtail_sb_imageserializer-0.3.0/pyproject.toml` & `wagtail_sb_imageserializer-0.4.0/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "wagtail-sb-imageserializer"
-version = "0.3.0"
+version = "0.4.0"
 description = "Social Networks settings for wagtail sites."
 authors = [
   "SoftButterfly Development Team <dev@softbutterfly.io>",
   "zodiacfireworks <martin.vuelta@gmail.com>"
 ]
 license = "MIT License"
 readme = "README.md"
@@ -34,24 +34,23 @@
 ]
 include = [
   "LICENSE.txt",
   "CHANGELOG.md",
 ]
 
 [tool.poetry.urls]
-"Download" = "https://gitlab.com/softbutterfly/open-source/wagtail-sb-imageserializer/-/archive/v0.3.0/wagtail-sb-imageserializer-v0.3.0.tar.gz"
+"Download" = "https://gitlab.com/softbutterfly/open-source/wagtail-sb-imageserializer/-/archive/v0.4.0/wagtail-sb-imageserializer-v0.4.0.tar.gz"
 "Bug Tracker" = "https://gitlab.com/softbutterfly/open-source/wagtail-sb-imageserializer/-/issues"
 
 
 [tool.poetry.dependencies]
 python = ">= 3.8.1, < 4.0.0"
 Django = "< 5.0"
 wagtail = "< 6.0"
 djangorestframework = "< 4.0"
-pytest-django = "^4.5.2"
 
 [tool.poetry.group.dev.dependencies]
 autopep8 = "^2.0.2"
 bandit = "^1.7.5"
 black = "^23.3.0"
 coverage = "^7.2.7"
 flake8 = "^6.0.0"
@@ -60,14 +59,15 @@
 mypy = "^1.3.0"
 pre-commit = "^3.3.3"
 pydocstyle = "^6.3.0"
 pylint = "^2.17.4"
 pylint-django = "^2.5.3"
 pytest = "^7.3.2"
 pytest-cov = "^4.1.0"
+pytest-django = "^4.5.2"
 python-dotenv = "^1.0.0"
 tbump = "^6.10.0"
 tox = "^4.6.2"
 
 [tool.pytest.ini_options]
 DJANGO_SETTINGS_MODULE = "demoproject.settings.dev"
 pythonpath = "demoproject"
```

### Comparing `wagtail_sb_imageserializer-0.3.0/src/wagtail_sb_imageserializer/api/fields.py` & `wagtail_sb_imageserializer-0.4.0/src/wagtail_sb_imageserializer/api/fields.py`

 * *Files identical despite different names*

### Comparing `wagtail_sb_imageserializer-0.3.0/PKG-INFO` & `wagtail_sb_imageserializer-0.4.0/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: wagtail-sb-imageserializer
-Version: 0.3.0
+Version: 0.4.0
 Summary: Social Networks settings for wagtail sites.
 Home-page: https://gitlab.com/softbutterfly/open-source/wagtail-sb-imageserializer
 License: MIT
 Keywords: Softbutterfly,Django,Migrations
 Author: SoftButterfly Development Team
 Author-email: dev@softbutterfly.io
 Requires-Python: >=3.8.1,<4.0.0
@@ -23,41 +23,41 @@
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Requires-Dist: Django (<5.0)
 Requires-Dist: djangorestframework (<4.0)
-Requires-Dist: pytest-django (>=4.5.2,<5.0.0)
 Requires-Dist: wagtail (<6.0)
 Project-URL: Bug Tracker, https://gitlab.com/softbutterfly/open-source/wagtail-sb-imageserializer/-/issues
 Project-URL: Documentation, https://gitlab.com/softbutterfly/open-source/wagtail-sb-imageserializer/-/wikis
-Project-URL: Download, https://gitlab.com/softbutterfly/open-source/wagtail-sb-imageserializer/-/archive/v0.3.0/wagtail-sb-imageserializer-v0.3.0.tar.gz
+Project-URL: Download, https://gitlab.com/softbutterfly/open-source/wagtail-sb-imageserializer/-/archive/v0.4.0/wagtail-sb-imageserializer-v0.4.0.tar.gz
 Project-URL: Repository, https://gitlab.com/softbutterfly/open-source/wagtail-sb-imageserializer
 Description-Content-Type: text/markdown
 
 ![Community-Project](https://gitlab.com/softbutterfly/open-source/open-source-office/-/raw/master/banners/softbutterfly-open-source--banner--community-project.png)
 
 ![PyPI - Supported versions](https://img.shields.io/pypi/pyversions/wagtail-sb-imageserializer)
 ![PyPI - Package version](https://img.shields.io/pypi/v/wagtail-sb-imageserializer)
 ![PyPI - Downloads](https://img.shields.io/pypi/dm/wagtail-sb-imageserializer)
 ![PyPI - MIT License](https://img.shields.io/pypi/l/wagtail-sb-imageserializer)
 
 [![Codacy Badge](https://app.codacy.com/project/badge/Grade/329484ea99434c708f5c8dbd611f3d35)](https://app.codacy.com/gl/softbutterfly/wagtail-sb-imageserializer/dashboard?utm_source=gl&utm_medium=referral&utm_content=&utm_campaign=Badge_grade)
+[![Codacy Coverage Badge](https://app.codacy.com/project/badge/Coverage/900411c7b5e443f89f85c7978f7504e5)](https://app.codacy.com/gl/softbutterfly/wagtail-sb-imageserializer/dashboard?utm_source=gl&utm_medium=referral&utm_content=&utm_campaign=Badge_coverage)
 
 # Wagtail Image Serializer
 
 Wagtail package to render images with rendition in a single API Field.
 
 ## Requirements
 
 - Python 3.8.1 or higher
-- Django lower than 4.0
-- Wagtail lower than 6.0
-- Django Rest Framework lower than 4.0
+- Wagtail 3.0 or higher
+- Django 3.2 or higher
+- Django Rest Framework 3.13 or higher
 
 ## Install
 
 ```bash
 pip install wagtail-sb-imageserializer
 ```
```

