# Comparing `tmp/docusign-monitor-1.1.0.tar.gz` & `tmp/docusign-monitor-1.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/docusign-monitor-1.1.0.tar", last modified: Tue Apr 12 00:01:53 2022, max compression
+gzip compressed data, was "dist/docusign-monitor-1.2.0.tar", last modified: Mon Jun 26 16:38:20 2023, max compression
```

## Comparing `docusign-monitor-1.1.0.tar` & `docusign-monitor-1.2.0.tar`

### file list

```diff
@@ -1,39 +1,40 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-04-12 00:01:53.000000 docusign-monitor-1.1.0/
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-04-12 00:01:53.000000 docusign-monitor-1.1.0/docusign_monitor.egg-info/
--rw-r--r--   0 root         (0) root         (0)       22 2022-04-12 00:01:53.000000 docusign-monitor-1.1.0/docusign_monitor.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)     3765 2022-04-12 00:01:53.000000 docusign-monitor-1.1.0/docusign_monitor.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      131 2022-04-12 00:01:53.000000 docusign-monitor-1.1.0/docusign_monitor.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)        1 2022-04-12 00:01:53.000000 docusign-monitor-1.1.0/docusign_monitor.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      989 2022-04-12 00:01:53.000000 docusign-monitor-1.1.0/docusign_monitor.egg-info/SOURCES.txt
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-04-12 00:01:53.000000 docusign-monitor-1.1.0/test/
--rwxr-xr-x   0 root         (0) root         (0)     4770 2022-04-12 00:01:51.000000 docusign-monitor-1.1.0/test/test_oauth.py
--rwxr-xr-x   0 root         (0) root         (0)     2990 2022-04-12 00:01:51.000000 docusign-monitor-1.1.0/test/unit_tests.py
--rwxr-xr-x   0 root         (0) root         (0)        0 2022-04-12 00:01:51.000000 docusign-monitor-1.1.0/test/__init__.py
--rw-r--r--   0 root         (0) root         (0)     3765 2022-04-12 00:01:53.000000 docusign-monitor-1.1.0/PKG-INFO
--rwxr-xr-x   0 root         (0) root         (0)       79 2022-04-12 00:01:53.000000 docusign-monitor-1.1.0/setup.cfg
--rwxr-xr-x   0 root         (0) root         (0)     3498 2022-04-12 00:01:51.000000 docusign-monitor-1.1.0/README.md
--rwxr-xr-x   0 root         (0) root         (0)     1102 2022-04-12 00:01:51.000000 docusign-monitor-1.1.0/LICENSE
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-04-12 00:01:53.000000 docusign-monitor-1.1.0/docusign_monitor/
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-04-12 00:01:53.000000 docusign-monitor-1.1.0/docusign_monitor/client/
--rwxr-xr-x   0 root         (0) root         (0)    11315 2022-04-12 00:01:51.000000 docusign-monitor-1.1.0/docusign_monitor/client/api_response.py
--rwxr-xr-x   0 root         (0) root         (0)     1503 2022-04-12 00:01:51.000000 docusign-monitor-1.1.0/docusign_monitor/client/api_exception.py
--rwxr-xr-x   0 root         (0) root         (0)     7245 2022-04-12 00:01:51.000000 docusign-monitor-1.1.0/docusign_monitor/client/configuration.py
--rwxr-xr-x   0 root         (0) root         (0)    35255 2022-04-12 00:01:51.000000 docusign-monitor-1.1.0/docusign_monitor/client/api_client.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-04-12 00:01:53.000000 docusign-monitor-1.1.0/docusign_monitor/client/auth/
--rwxr-xr-x   0 root         (0) root         (0)    14756 2022-04-12 00:01:51.000000 docusign-monitor-1.1.0/docusign_monitor/client/auth/oauth.py
--rwxr-xr-x   0 root         (0) root         (0)      219 2022-04-12 00:01:51.000000 docusign-monitor-1.1.0/docusign_monitor/client/auth/__init__.py
--rwxr-xr-x   0 root         (0) root         (0)      283 2022-04-12 00:01:51.000000 docusign-monitor-1.1.0/docusign_monitor/client/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-04-12 00:01:53.000000 docusign-monitor-1.1.0/docusign_monitor/apis/
--rw-r--r--   0 root         (0) root         (0)    12829 2022-04-12 00:01:51.000000 docusign-monitor-1.1.0/docusign_monitor/apis/data_set_api.py
--rw-r--r--   0 root         (0) root         (0)      124 2022-04-12 00:01:51.000000 docusign-monitor-1.1.0/docusign_monitor/apis/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-04-12 00:01:53.000000 docusign-monitor-1.1.0/docusign_monitor/models/
--rw-r--r--   0 root         (0) root         (0)     3262 2022-04-12 00:01:51.000000 docusign-monitor-1.1.0/docusign_monitor/models/aggregation.py
--rw-r--r--   0 root         (0) root         (0)     4822 2022-04-12 00:01:51.000000 docusign-monitor-1.1.0/docusign_monitor/models/raw_request.py
--rw-r--r--   0 root         (0) root         (0)     5891 2022-04-12 00:01:51.000000 docusign-monitor-1.1.0/docusign_monitor/models/web_query.py
--rw-r--r--   0 root         (0) root         (0)     4052 2022-04-12 00:01:51.000000 docusign-monitor-1.1.0/docusign_monitor/models/aggregate_result_result.py
--rw-r--r--   0 root         (0) root         (0)     4068 2022-04-12 00:01:51.000000 docusign-monitor-1.1.0/docusign_monitor/models/cursored_result.py
--rw-r--r--   0 root         (0) root         (0)     3122 2022-04-12 00:01:51.000000 docusign-monitor-1.1.0/docusign_monitor/models/filter.py
--rw-r--r--   0 root         (0) root         (0)     3465 2022-04-12 00:01:51.000000 docusign-monitor-1.1.0/docusign_monitor/models/aggregate_result.py
--rw-r--r--   0 root         (0) root         (0)      630 2022-04-12 00:01:51.000000 docusign-monitor-1.1.0/docusign_monitor/models/__init__.py
--rw-r--r--   0 root         (0) root         (0)     1095 2022-04-12 00:01:51.000000 docusign-monitor-1.1.0/docusign_monitor/__init__.py
--rwxr-xr-x   0 root         (0) root         (0)     1582 2022-04-12 00:01:51.000000 docusign-monitor-1.1.0/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-26 16:38:20.000000 docusign-monitor-1.2.0/
+-rwxr-xr-x   0 root         (0) root         (0)     1102 2023-06-26 16:38:17.000000 docusign-monitor-1.2.0/LICENSE
+-rw-r--r--   0 root         (0) root         (0)     3721 2023-06-26 16:38:20.000000 docusign-monitor-1.2.0/PKG-INFO
+-rwxr-xr-x   0 root         (0) root         (0)     3498 2023-06-26 16:38:17.000000 docusign-monitor-1.2.0/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-26 16:38:20.000000 docusign-monitor-1.2.0/docusign_monitor/
+-rw-r--r--   0 root         (0) root         (0)      942 2023-06-26 16:38:17.000000 docusign-monitor-1.2.0/docusign_monitor/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-26 16:38:20.000000 docusign-monitor-1.2.0/docusign_monitor/apis/
+-rw-r--r--   0 root         (0) root         (0)      124 2023-06-26 16:38:17.000000 docusign-monitor-1.2.0/docusign_monitor/apis/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     8167 2023-06-26 16:38:17.000000 docusign-monitor-1.2.0/docusign_monitor/apis/data_set_api.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-26 16:38:20.000000 docusign-monitor-1.2.0/docusign_monitor/client/
+-rwxr-xr-x   0 root         (0) root         (0)      283 2023-06-26 16:38:17.000000 docusign-monitor-1.2.0/docusign_monitor/client/__init__.py
+-rwxr-xr-x   0 root         (0) root         (0)    35255 2023-06-26 16:38:17.000000 docusign-monitor-1.2.0/docusign_monitor/client/api_client.py
+-rwxr-xr-x   0 root         (0) root         (0)     1503 2023-06-26 16:38:17.000000 docusign-monitor-1.2.0/docusign_monitor/client/api_exception.py
+-rwxr-xr-x   0 root         (0) root         (0)    11315 2023-06-26 16:38:17.000000 docusign-monitor-1.2.0/docusign_monitor/client/api_response.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-26 16:38:20.000000 docusign-monitor-1.2.0/docusign_monitor/client/auth/
+-rwxr-xr-x   0 root         (0) root         (0)      219 2023-06-26 16:38:17.000000 docusign-monitor-1.2.0/docusign_monitor/client/auth/__init__.py
+-rwxr-xr-x   0 root         (0) root         (0)    14756 2023-06-26 16:38:17.000000 docusign-monitor-1.2.0/docusign_monitor/client/auth/oauth.py
+-rwxr-xr-x   0 root         (0) root         (0)     7245 2023-06-26 16:38:17.000000 docusign-monitor-1.2.0/docusign_monitor/client/configuration.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-26 16:38:20.000000 docusign-monitor-1.2.0/docusign_monitor/models/
+-rw-r--r--   0 root         (0) root         (0)      477 2023-06-26 16:38:17.000000 docusign-monitor-1.2.0/docusign_monitor/models/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     3465 2023-06-26 16:38:17.000000 docusign-monitor-1.2.0/docusign_monitor/models/aggregate_result.py
+-rw-r--r--   0 root         (0) root         (0)     4052 2023-06-26 16:38:17.000000 docusign-monitor-1.2.0/docusign_monitor/models/aggregate_result_result.py
+-rw-r--r--   0 root         (0) root         (0)     3262 2023-06-26 16:38:17.000000 docusign-monitor-1.2.0/docusign_monitor/models/aggregation.py
+-rw-r--r--   0 root         (0) root         (0)     4160 2023-06-26 16:38:17.000000 docusign-monitor-1.2.0/docusign_monitor/models/cursored_result.py
+-rw-r--r--   0 root         (0) root         (0)     4069 2023-06-26 16:38:17.000000 docusign-monitor-1.2.0/docusign_monitor/models/data_set.py
+-rw-r--r--   0 root         (0) root         (0)     3122 2023-06-26 16:38:17.000000 docusign-monitor-1.2.0/docusign_monitor/models/filter.py
+-rw-r--r--   0 root         (0) root         (0)     4822 2023-06-26 16:38:17.000000 docusign-monitor-1.2.0/docusign_monitor/models/raw_request.py
+-rw-r--r--   0 root         (0) root         (0)     5891 2023-06-26 16:38:17.000000 docusign-monitor-1.2.0/docusign_monitor/models/web_query.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-26 16:38:20.000000 docusign-monitor-1.2.0/docusign_monitor.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     3721 2023-06-26 16:38:20.000000 docusign-monitor-1.2.0/docusign_monitor.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     1025 2023-06-26 16:38:20.000000 docusign-monitor-1.2.0/docusign_monitor.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-06-26 16:38:20.000000 docusign-monitor-1.2.0/docusign_monitor.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      128 2023-06-26 16:38:20.000000 docusign-monitor-1.2.0/docusign_monitor.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       22 2023-06-26 16:38:20.000000 docusign-monitor-1.2.0/docusign_monitor.egg-info/top_level.txt
+-rwxr-xr-x   0 root         (0) root         (0)       79 2023-06-26 16:38:20.000000 docusign-monitor-1.2.0/setup.cfg
+-rwxr-xr-x   0 root         (0) root         (0)     1579 2023-06-26 16:38:17.000000 docusign-monitor-1.2.0/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-26 16:38:20.000000 docusign-monitor-1.2.0/test/
+-rwxr-xr-x   0 root         (0) root         (0)        0 2023-06-26 16:38:17.000000 docusign-monitor-1.2.0/test/__init__.py
+-rwxr-xr-x   0 root         (0) root         (0)     4770 2023-06-26 16:38:17.000000 docusign-monitor-1.2.0/test/test_oauth.py
+-rwxr-xr-x   0 root         (0) root         (0)     2990 2023-06-26 16:38:17.000000 docusign-monitor-1.2.0/test/unit_tests.py
```

### Comparing `docusign-monitor-1.1.0/docusign_monitor.egg-info/PKG-INFO` & `docusign-monitor-1.2.0/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,16 +1,14 @@
 Metadata-Version: 2.1
 Name: docusign-monitor
-Version: 1.1.0
+Version: 1.2.0
 Summary: Monitor API
-Home-page: UNKNOWN
+Home-page: 
 Author-email: devcenter@docusign.com
-License: UNKNOWN
 Keywords: Swagger,Monitor API
-Platform: UNKNOWN
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # The Official DocuSign Monitor Python Client
 
 [![PyPI version][pypi-image]][pypi-url]
 <!--[![PyPI downloads][downloads-image]][downloads-url]-->
@@ -96,9 +94,7 @@
 
 [pypi-image]: https://img.shields.io/pypi/v/docusign_monitor.svg?style=flat
 [pypi-url]: https://pypi.python.org/pypi/docusign_monitor
 [downloads-image]: https://img.shields.io/pypi/dm/docusign_monitor.svg?style=flat
 [downloads-url]: https://pypi.python.org/pypi/docusign_monitor
 [travis-image]: https://img.shields.io/travis/docusign/docusign-monitor-python-client.svg?style=flat
 [travis-url]: https://travis-ci.org/docusign/docusign-monitor-python-client
-
-
```

#### html2text {}

```diff
@@ -1,26 +1,26 @@
-Metadata-Version: 2.1 Name: docusign-monitor Version: 1.1.0 Summary: Monitor
-API Home-page: UNKNOWN Author-email: devcenter@docusign.com License: UNKNOWN
-Keywords: Swagger,Monitor API Platform: UNKNOWN Description-Content-Type: text/
-markdown License-File: LICENSE # The Official DocuSign Monitor Python Client [!
-[PyPI version][pypi-image]][pypi-url]  [![Build status][travis-image]][travis-
-url] [PyPI module](https://pypi.python.org/pypi/docusign_monitor) that wraps
-the DocuSign_Monitor API [Documentation about the DocuSign Monitor API](https:/
-/developers.docusign.com/) ## Requirements - Python 2.7 (3.7+ recommended) -
-Free [Developer Sandbox](https://go.docusign.com/sandbox/productshot/
-?elqCampaignId=16531) ## Compatibility - Python 2.7+ ## Installation ### Path
-Setup: 1. Locate your Python installation, also referred to as a **site-
-packages** folder. This folder is usually labeled in a format of Python
-{VersionNumber}. **Examples:** - **Unix/Linux:** /usr/lib/python2.7 - **Mac:**
-/Library/Frameworks/Python.framework/Versions/2.7/lib/python2.7 - **Windows:**
-C:\Users\{username}\AppData\Local\Programs\Python\Python37 1. Add the path to
-your Python folder as an environment variable. **Unix/Linux:** - Type the
-following command into your console: **export PYTHONPATH = "${PYTHONPATH}:.:/
-path/to/site-packages"** - Optionally, you can add this command to your system
-profile, which will run the command each time Python is launched. **Windows:**
+Metadata-Version: 2.1 Name: docusign-monitor Version: 1.2.0 Summary: Monitor
+API Home-page: Author-email: devcenter@docusign.com Keywords: Swagger,Monitor
+API Description-Content-Type: text/markdown License-File: LICENSE # The
+Official DocuSign Monitor Python Client [![PyPI version][pypi-image]][pypi-url]
+[![Build status][travis-image]][travis-url] [PyPI module](https://
+pypi.python.org/pypi/docusign_monitor) that wraps the DocuSign_Monitor API
+[Documentation about the DocuSign Monitor API](https://developers.docusign.com/
+) ## Requirements - Python 2.7 (3.7+ recommended) - Free [Developer Sandbox]
+(https://go.docusign.com/sandbox/productshot/?elqCampaignId=16531) ##
+Compatibility - Python 2.7+ ## Installation ### Path Setup: 1. Locate your
+Python installation, also referred to as a **site-packages** folder. This
+folder is usually labeled in a format of Python{VersionNumber}. **Examples:** -
+**Unix/Linux:** /usr/lib/python2.7 - **Mac:** /Library/Frameworks/
+Python.framework/Versions/2.7/lib/python2.7 - **Windows:** C:\Users\
+{username}\AppData\Local\Programs\Python\Python37 1. Add the path to your
+Python folder as an environment variable. **Unix/Linux:** - Type the following
+command into your console: **export PYTHONPATH = "${PYTHONPATH}:.:/path/to/
+site-packages"** - Optionally, you can add this command to your system profile,
+which will run the command each time Python is launched. **Windows:**
    1. Open the Windows Control Panel.
    2. Under the System and Security category, open the System
    3. Select Advanced System Settings to open the System Properties dialog box.
    4. On the Advanced tab, select the Environmental Variables button at the
       lower-right corner.
          1. Check if PYTHONPATH has been added as a system variable.
          2. If it has not, select New to add it. The variable you add is the
```

### Comparing `docusign-monitor-1.1.0/docusign_monitor.egg-info/SOURCES.txt` & `docusign-monitor-1.2.0/docusign_monitor.egg-info/SOURCES.txt`

 * *Files 5% similar despite different names*

```diff
@@ -18,13 +18,14 @@
 docusign_monitor/client/auth/__init__.py
 docusign_monitor/client/auth/oauth.py
 docusign_monitor/models/__init__.py
 docusign_monitor/models/aggregate_result.py
 docusign_monitor/models/aggregate_result_result.py
 docusign_monitor/models/aggregation.py
 docusign_monitor/models/cursored_result.py
+docusign_monitor/models/data_set.py
 docusign_monitor/models/filter.py
 docusign_monitor/models/raw_request.py
 docusign_monitor/models/web_query.py
 test/__init__.py
 test/test_oauth.py
 test/unit_tests.py
```

### Comparing `docusign-monitor-1.1.0/test/test_oauth.py` & `docusign-monitor-1.2.0/test/test_oauth.py`

 * *Files identical despite different names*

### Comparing `docusign-monitor-1.1.0/test/unit_tests.py` & `docusign-monitor-1.2.0/test/unit_tests.py`

 * *Files identical despite different names*

### Comparing `docusign-monitor-1.1.0/PKG-INFO` & `docusign-monitor-1.2.0/docusign_monitor.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,16 +1,14 @@
 Metadata-Version: 2.1
 Name: docusign-monitor
-Version: 1.1.0
+Version: 1.2.0
 Summary: Monitor API
-Home-page: UNKNOWN
+Home-page: 
 Author-email: devcenter@docusign.com
-License: UNKNOWN
 Keywords: Swagger,Monitor API
-Platform: UNKNOWN
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # The Official DocuSign Monitor Python Client
 
 [![PyPI version][pypi-image]][pypi-url]
 <!--[![PyPI downloads][downloads-image]][downloads-url]-->
@@ -96,9 +94,7 @@
 
 [pypi-image]: https://img.shields.io/pypi/v/docusign_monitor.svg?style=flat
 [pypi-url]: https://pypi.python.org/pypi/docusign_monitor
 [downloads-image]: https://img.shields.io/pypi/dm/docusign_monitor.svg?style=flat
 [downloads-url]: https://pypi.python.org/pypi/docusign_monitor
 [travis-image]: https://img.shields.io/travis/docusign/docusign-monitor-python-client.svg?style=flat
 [travis-url]: https://travis-ci.org/docusign/docusign-monitor-python-client
-
-
```

#### html2text {}

```diff
@@ -1,26 +1,26 @@
-Metadata-Version: 2.1 Name: docusign-monitor Version: 1.1.0 Summary: Monitor
-API Home-page: UNKNOWN Author-email: devcenter@docusign.com License: UNKNOWN
-Keywords: Swagger,Monitor API Platform: UNKNOWN Description-Content-Type: text/
-markdown License-File: LICENSE # The Official DocuSign Monitor Python Client [!
-[PyPI version][pypi-image]][pypi-url]  [![Build status][travis-image]][travis-
-url] [PyPI module](https://pypi.python.org/pypi/docusign_monitor) that wraps
-the DocuSign_Monitor API [Documentation about the DocuSign Monitor API](https:/
-/developers.docusign.com/) ## Requirements - Python 2.7 (3.7+ recommended) -
-Free [Developer Sandbox](https://go.docusign.com/sandbox/productshot/
-?elqCampaignId=16531) ## Compatibility - Python 2.7+ ## Installation ### Path
-Setup: 1. Locate your Python installation, also referred to as a **site-
-packages** folder. This folder is usually labeled in a format of Python
-{VersionNumber}. **Examples:** - **Unix/Linux:** /usr/lib/python2.7 - **Mac:**
-/Library/Frameworks/Python.framework/Versions/2.7/lib/python2.7 - **Windows:**
-C:\Users\{username}\AppData\Local\Programs\Python\Python37 1. Add the path to
-your Python folder as an environment variable. **Unix/Linux:** - Type the
-following command into your console: **export PYTHONPATH = "${PYTHONPATH}:.:/
-path/to/site-packages"** - Optionally, you can add this command to your system
-profile, which will run the command each time Python is launched. **Windows:**
+Metadata-Version: 2.1 Name: docusign-monitor Version: 1.2.0 Summary: Monitor
+API Home-page: Author-email: devcenter@docusign.com Keywords: Swagger,Monitor
+API Description-Content-Type: text/markdown License-File: LICENSE # The
+Official DocuSign Monitor Python Client [![PyPI version][pypi-image]][pypi-url]
+[![Build status][travis-image]][travis-url] [PyPI module](https://
+pypi.python.org/pypi/docusign_monitor) that wraps the DocuSign_Monitor API
+[Documentation about the DocuSign Monitor API](https://developers.docusign.com/
+) ## Requirements - Python 2.7 (3.7+ recommended) - Free [Developer Sandbox]
+(https://go.docusign.com/sandbox/productshot/?elqCampaignId=16531) ##
+Compatibility - Python 2.7+ ## Installation ### Path Setup: 1. Locate your
+Python installation, also referred to as a **site-packages** folder. This
+folder is usually labeled in a format of Python{VersionNumber}. **Examples:** -
+**Unix/Linux:** /usr/lib/python2.7 - **Mac:** /Library/Frameworks/
+Python.framework/Versions/2.7/lib/python2.7 - **Windows:** C:\Users\
+{username}\AppData\Local\Programs\Python\Python37 1. Add the path to your
+Python folder as an environment variable. **Unix/Linux:** - Type the following
+command into your console: **export PYTHONPATH = "${PYTHONPATH}:.:/path/to/
+site-packages"** - Optionally, you can add this command to your system profile,
+which will run the command each time Python is launched. **Windows:**
    1. Open the Windows Control Panel.
    2. Under the System and Security category, open the System
    3. Select Advanced System Settings to open the System Properties dialog box.
    4. On the Advanced tab, select the Environmental Variables button at the
       lower-right corner.
          1. Check if PYTHONPATH has been added as a system variable.
          2. If it has not, select New to add it. The variable you add is the
```

### Comparing `docusign-monitor-1.1.0/README.md` & `docusign-monitor-1.2.0/README.md`

 * *Files identical despite different names*

### Comparing `docusign-monitor-1.1.0/LICENSE` & `docusign-monitor-1.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `docusign-monitor-1.1.0/docusign_monitor/client/api_response.py` & `docusign-monitor-1.2.0/docusign_monitor/client/api_response.py`

 * *Files identical despite different names*

### Comparing `docusign-monitor-1.1.0/docusign_monitor/client/api_exception.py` & `docusign-monitor-1.2.0/docusign_monitor/client/api_exception.py`

 * *Files identical despite different names*

### Comparing `docusign-monitor-1.1.0/docusign_monitor/client/configuration.py` & `docusign-monitor-1.2.0/docusign_monitor/client/configuration.py`

 * *Files identical despite different names*

### Comparing `docusign-monitor-1.1.0/docusign_monitor/client/api_client.py` & `docusign-monitor-1.2.0/docusign_monitor/client/api_client.py`

 * *Files identical despite different names*

### Comparing `docusign-monitor-1.1.0/docusign_monitor/client/auth/oauth.py` & `docusign-monitor-1.2.0/docusign_monitor/client/auth/oauth.py`

 * *Files identical despite different names*

### Comparing `docusign-monitor-1.1.0/docusign_monitor/models/aggregation.py` & `docusign-monitor-1.2.0/docusign_monitor/models/aggregation.py`

 * *Files identical despite different names*

### Comparing `docusign-monitor-1.1.0/docusign_monitor/models/raw_request.py` & `docusign-monitor-1.2.0/docusign_monitor/models/raw_request.py`

 * *Files identical despite different names*

### Comparing `docusign-monitor-1.1.0/docusign_monitor/models/web_query.py` & `docusign-monitor-1.2.0/docusign_monitor/models/web_query.py`

 * *Files identical despite different names*

### Comparing `docusign-monitor-1.1.0/docusign_monitor/models/aggregate_result_result.py` & `docusign-monitor-1.2.0/docusign_monitor/models/aggregate_result_result.py`

 * *Files identical despite different names*

### Comparing `docusign-monitor-1.1.0/docusign_monitor/models/cursored_result.py` & `docusign-monitor-1.2.0/docusign_monitor/models/cursored_result.py`

 * *Files 8% similar despite different names*

```diff
@@ -55,45 +55,49 @@
         setattr(self, "_{}".format('end_cursor'), kwargs.get('end_cursor', None))
         setattr(self, "_{}".format('data'), kwargs.get('data', None))
 
     @property
     def end_cursor(self):
         """Gets the end_cursor of this CursoredResult.  # noqa: E501
 
+          # noqa: E501
 
         :return: The end_cursor of this CursoredResult.  # noqa: E501
         :rtype: str
         """
         return self._end_cursor
 
     @end_cursor.setter
     def end_cursor(self, end_cursor):
         """Sets the end_cursor of this CursoredResult.
 
+          # noqa: E501
 
         :param end_cursor: The end_cursor of this CursoredResult.  # noqa: E501
         :type: str
         """
 
         self._end_cursor = end_cursor
 
     @property
     def data(self):
         """Gets the data of this CursoredResult.  # noqa: E501
 
+          # noqa: E501
 
         :return: The data of this CursoredResult.  # noqa: E501
         :rtype: list[object]
         """
         return self._data
 
     @data.setter
     def data(self, data):
         """Sets the data of this CursoredResult.
 
+          # noqa: E501
 
         :param data: The data of this CursoredResult.  # noqa: E501
         :type: list[object]
         """
 
         self._data = data
```

### Comparing `docusign-monitor-1.1.0/docusign_monitor/models/filter.py` & `docusign-monitor-1.2.0/docusign_monitor/models/filter.py`

 * *Files identical despite different names*

### Comparing `docusign-monitor-1.1.0/docusign_monitor/models/aggregate_result.py` & `docusign-monitor-1.2.0/docusign_monitor/models/aggregate_result.py`

 * *Files identical despite different names*

### Comparing `docusign-monitor-1.1.0/docusign_monitor/__init__.py` & `docusign-monitor-1.2.0/docusign_monitor/__init__.py`

 * *Files 26% similar despite different names*

```diff
@@ -26,14 +26,12 @@
 from .client.auth.oauth import OAuth	
 from .client.auth.oauth import OAuthToken	
 from .client.auth.oauth import Account	
 from .client.auth.oauth import Organization	
 from .client.auth.oauth import Link
 
 # import models into sdk package
-from docusign_monitor.models.aggregate_result import AggregateResult
-from docusign_monitor.models.aggregate_result_result import AggregateResultResult
 from docusign_monitor.models.cursored_result import CursoredResult
-from docusign_monitor.models.web_query import WebQuery
+from docusign_monitor.models.data_set import DataSet
 
 
 configuration = Configuration()
```

### Comparing `docusign-monitor-1.1.0/setup.py` & `docusign-monitor-1.2.0/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -10,23 +10,23 @@
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 
 from setuptools import setup, find_packages, Command, os  # noqa: H301	
 
 NAME = "docusign-monitor"
-VERSION = "1.1.0"
+VERSION = "1.2.0"
 # To install the library, run the following
 #
 # python setup.py install
 #
 # prerequisite: setuptools
 # http://pypi.python.org/pypi/setuptools
 
-REQUIRES = ["urllib3 >= 1.15", "six >= 1.8.0", "certifi >= 14.05.14", "python-dateutil >= 2.5.3", "setuptools >= 21.0.0", "PyJWT>=1.7.1,<2", "cryptography>=2.5", "nose>=1.3.7"]
+REQUIRES = ["urllib3 >= 1.15", "six >= 1.8.0", "certifi >= 14.05.14", "python-dateutil >= 2.5.3", "setuptools >= 21.0.0", "PyJWT>=1.7.1", "cryptography>=2.5", "nose>=1.3.7"]
 
 class CleanCommand(Command):
     """Custom clean command to tidy up the project root."""
     user_options = []
     def initialize_options(self):
         pass
     def finalize_options(self):
```

