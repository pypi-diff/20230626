# Comparing `tmp/smawe_tools-0.3.0.tar.gz` & `tmp/smawe_tools-0.3.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "smawe_tools-0.3.0.tar", last modified: Thu Jun  8 12:46:32 2023, max compression
+gzip compressed data, was "smawe_tools-0.3.1.tar", last modified: Mon Jun 26 07:42:09 2023, max compression
```

## Comparing `smawe_tools-0.3.0.tar` & `smawe_tools-0.3.1.tar`

### file list

```diff
@@ -1,32 +1,33 @@
-drwxrwxrwx   0        0        0        0 2023-06-08 12:46:32.798761 smawe_tools-0.3.0/
--rw-rw-rw-   0        0        0     1091 2023-01-15 03:19:33.000000 smawe_tools-0.3.0/LICENSE
--rw-rw-rw-   0        0        0     6568 2023-06-08 12:46:32.797758 smawe_tools-0.3.0/PKG-INFO
--rw-rw-rw-   0        0        0     6091 2023-06-08 12:45:40.000000 smawe_tools-0.3.0/README.md
--rw-rw-rw-   0        0        0       42 2023-06-08 12:46:32.798761 smawe_tools-0.3.0/setup.cfg
--rw-rw-rw-   0        0        0     1019 2023-04-04 10:22:33.000000 smawe_tools-0.3.0/setup.py
-drwxrwxrwx   0        0        0        0 2023-06-08 12:46:32.778761 smawe_tools-0.3.0/smawe_tools/
--rw-rw-rw-   0        0        0      194 2023-06-03 07:46:52.000000 smawe_tools-0.3.0/smawe_tools/__init__.py
--rw-rw-rw-   0        0        0       76 2023-06-08 12:45:40.000000 smawe_tools-0.3.0/smawe_tools/__version__.py
--rw-rw-rw-   0        0        0      394 2023-06-08 12:35:51.000000 smawe_tools-0.3.0/smawe_tools/algorithm.py
--rw-rw-rw-   0        0        0     6799 2023-05-28 10:27:58.000000 smawe_tools-0.3.0/smawe_tools/config.py
-drwxrwxrwx   0        0        0        0 2023-06-08 12:46:32.788757 smawe_tools-0.3.0/smawe_tools/exception/
--rw-rw-rw-   0        0        0       98 2023-04-02 12:50:55.000000 smawe_tools-0.3.0/smawe_tools/exception/__init__.py
-drwxrwxrwx   0        0        0        0 2023-06-08 12:46:32.791757 smawe_tools-0.3.0/smawe_tools/net/
--rw-rw-rw-   0        0        0       29 2023-03-29 05:15:59.000000 smawe_tools-0.3.0/smawe_tools/net/__init__.py
--rw-rw-rw-   0        0        0     2905 2023-04-04 10:22:33.000000 smawe_tools-0.3.0/smawe_tools/net/network_tool.py
-drwxrwxrwx   0        0        0        0 2023-06-08 12:46:32.793758 smawe_tools-0.3.0/smawe_tools/retrying/
--rw-rw-rw-   0        0        0       26 2023-04-04 07:07:45.000000 smawe_tools-0.3.0/smawe_tools/retrying/__init__.py
--rw-rw-rw-   0        0        0     2889 2023-06-03 07:46:52.000000 smawe_tools-0.3.0/smawe_tools/retrying/retry.py
--rw-rw-rw-   0        0        0      670 2023-04-18 02:48:31.000000 smawe_tools-0.3.0/smawe_tools/settings.py
-drwxrwxrwx   0        0        0        0 2023-06-08 12:46:32.795758 smawe_tools-0.3.0/smawe_tools/struct/
--rw-rw-rw-   0        0        0      946 2023-04-06 10:03:49.000000 smawe_tools-0.3.0/smawe_tools/struct/__init__.py
--rw-rw-rw-   0        0        0     2842 2023-04-19 07:48:57.000000 smawe_tools-0.3.0/smawe_tools/tool.py
--rw-rw-rw-   0        0        0     1627 2023-06-08 12:35:51.000000 smawe_tools-0.3.0/smawe_tools/utils.py
-drwxrwxrwx   0        0        0        0 2023-06-08 12:46:32.784758 smawe_tools-0.3.0/smawe_tools.egg-info/
--rw-rw-rw-   0        0        0     6568 2023-06-08 12:46:32.000000 smawe_tools-0.3.0/smawe_tools.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      565 2023-06-08 12:46:32.000000 smawe_tools-0.3.0/smawe_tools.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-08 12:46:32.000000 smawe_tools-0.3.0/smawe_tools.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        9 2023-06-08 12:46:32.000000 smawe_tools-0.3.0/smawe_tools.egg-info/requires.txt
--rw-rw-rw-   0        0        0       12 2023-06-08 12:46:32.000000 smawe_tools-0.3.0/smawe_tools.egg-info/top_level.txt
-drwxrwxrwx   0        0        0        0 2023-06-08 12:46:32.796762 smawe_tools-0.3.0/tests/
--rw-rw-rw-   0        0        0       79 2023-06-08 12:39:15.000000 smawe_tools-0.3.0/tests/test.py
+drwxrwxrwx   0        0        0        0 2023-06-26 07:42:09.953637 smawe_tools-0.3.1/
+-rw-rw-rw-   0        0        0     1091 2023-01-15 03:19:33.000000 smawe_tools-0.3.1/LICENSE
+-rw-rw-rw-   0        0        0     6568 2023-06-26 07:42:09.952641 smawe_tools-0.3.1/PKG-INFO
+-rw-rw-rw-   0        0        0     6091 2023-06-08 12:45:40.000000 smawe_tools-0.3.1/README.md
+-rw-rw-rw-   0        0        0       42 2023-06-26 07:42:09.953637 smawe_tools-0.3.1/setup.cfg
+-rw-rw-rw-   0        0        0     1019 2023-04-04 10:22:33.000000 smawe_tools-0.3.1/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-26 07:42:09.933642 smawe_tools-0.3.1/smawe_tools/
+-rw-rw-rw-   0        0        0      194 2023-06-03 07:46:52.000000 smawe_tools-0.3.1/smawe_tools/__init__.py
+-rw-rw-rw-   0        0        0       76 2023-06-26 07:38:46.000000 smawe_tools-0.3.1/smawe_tools/__version__.py
+-rw-rw-rw-   0        0        0      394 2023-06-18 06:13:54.000000 smawe_tools-0.3.1/smawe_tools/algorithm.py
+-rw-rw-rw-   0        0        0     6799 2023-05-28 10:27:58.000000 smawe_tools-0.3.1/smawe_tools/config.py
+drwxrwxrwx   0        0        0        0 2023-06-26 07:42:09.941638 smawe_tools-0.3.1/smawe_tools/exception/
+-rw-rw-rw-   0        0        0       98 2023-04-02 12:50:55.000000 smawe_tools-0.3.1/smawe_tools/exception/__init__.py
+-rw-rw-rw-   0        0        0     7105 2023-06-26 07:41:08.000000 smawe_tools-0.3.1/smawe_tools/mail_gui.py
+drwxrwxrwx   0        0        0        0 2023-06-26 07:42:09.945637 smawe_tools-0.3.1/smawe_tools/net/
+-rw-rw-rw-   0        0        0       29 2023-03-29 05:15:59.000000 smawe_tools-0.3.1/smawe_tools/net/__init__.py
+-rw-rw-rw-   0        0        0     2905 2023-04-04 10:22:33.000000 smawe_tools-0.3.1/smawe_tools/net/network_tool.py
+drwxrwxrwx   0        0        0        0 2023-06-26 07:42:09.948637 smawe_tools-0.3.1/smawe_tools/retrying/
+-rw-rw-rw-   0        0        0       26 2023-04-04 07:07:45.000000 smawe_tools-0.3.1/smawe_tools/retrying/__init__.py
+-rw-rw-rw-   0        0        0     2889 2023-06-03 07:46:52.000000 smawe_tools-0.3.1/smawe_tools/retrying/retry.py
+-rw-rw-rw-   0        0        0      670 2023-04-18 02:48:31.000000 smawe_tools-0.3.1/smawe_tools/settings.py
+drwxrwxrwx   0        0        0        0 2023-06-26 07:42:09.949642 smawe_tools-0.3.1/smawe_tools/struct/
+-rw-rw-rw-   0        0        0      946 2023-04-06 10:03:49.000000 smawe_tools-0.3.1/smawe_tools/struct/__init__.py
+-rw-rw-rw-   0        0        0     2842 2023-04-19 07:48:57.000000 smawe_tools-0.3.1/smawe_tools/tool.py
+-rw-rw-rw-   0        0        0     1750 2023-06-12 11:20:42.000000 smawe_tools-0.3.1/smawe_tools/utils.py
+drwxrwxrwx   0        0        0        0 2023-06-26 07:42:09.939637 smawe_tools-0.3.1/smawe_tools.egg-info/
+-rw-rw-rw-   0        0        0     6568 2023-06-26 07:42:09.000000 smawe_tools-0.3.1/smawe_tools.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      589 2023-06-26 07:42:09.000000 smawe_tools-0.3.1/smawe_tools.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-26 07:42:09.000000 smawe_tools-0.3.1/smawe_tools.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        9 2023-06-26 07:42:09.000000 smawe_tools-0.3.1/smawe_tools.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       12 2023-06-26 07:42:09.000000 smawe_tools-0.3.1/smawe_tools.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-06-26 07:42:09.950641 smawe_tools-0.3.1/tests/
+-rw-rw-rw-   0        0        0      725 2023-06-25 09:21:46.000000 smawe_tools-0.3.1/tests/test.py
```

### Comparing `smawe_tools-0.3.0/LICENSE` & `smawe_tools-0.3.1/LICENSE`

 * *Files identical despite different names*

### Comparing `smawe_tools-0.3.0/PKG-INFO` & `smawe_tools-0.3.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: smawe_tools
-Version: 0.3.0
+Version: 0.3.1
 Summary: small tool
 Author: Samwe
 Author-email: 1281722462@qq.com
 License: MIT
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: Implementation :: CPython
```

### Comparing `smawe_tools-0.3.0/README.md` & `smawe_tools-0.3.1/README.md`

 * *Files identical despite different names*

### Comparing `smawe_tools-0.3.0/setup.py` & `smawe_tools-0.3.1/setup.py`

 * *Files identical despite different names*

### Comparing `smawe_tools-0.3.0/smawe_tools/config.py` & `smawe_tools-0.3.1/smawe_tools/config.py`

 * *Files identical despite different names*

### Comparing `smawe_tools-0.3.0/smawe_tools/net/network_tool.py` & `smawe_tools-0.3.1/smawe_tools/net/network_tool.py`

 * *Files identical despite different names*

### Comparing `smawe_tools-0.3.0/smawe_tools/retrying/retry.py` & `smawe_tools-0.3.1/smawe_tools/retrying/retry.py`

 * *Files identical despite different names*

### Comparing `smawe_tools-0.3.0/smawe_tools/settings.py` & `smawe_tools-0.3.1/smawe_tools/settings.py`

 * *Files identical despite different names*

### Comparing `smawe_tools-0.3.0/smawe_tools/struct/__init__.py` & `smawe_tools-0.3.1/smawe_tools/struct/__init__.py`

 * *Files identical despite different names*

### Comparing `smawe_tools-0.3.0/smawe_tools/tool.py` & `smawe_tools-0.3.1/smawe_tools/tool.py`

 * *Files identical despite different names*

### Comparing `smawe_tools-0.3.0/smawe_tools/utils.py` & `smawe_tools-0.3.1/smawe_tools/utils.py`

 * *Files 4% similar despite different names*

```diff
@@ -35,7 +35,17 @@
         smtp_handler.setLevel(kwargs.pop("handler_level", logging.INFO))
         fmt = logging.Formatter("%(filename)s %(funcName)s %(levelname)s: (%(lineno)d)%(message)s")
         smtp_handler.setFormatter(fmt)
         error_logger = logging.getLogger("error_logger")
         error_logger.setLevel(kwargs.pop("logger_level", logging.INFO))
         error_logger.addHandler(smtp_handler)
         return error_logger
+
+
+class Email:
+
+    def __init__(self, **kwargs):
+        pass
+
+    def send_mail(self, **kwargs):
+        pass
+
```

### Comparing `smawe_tools-0.3.0/smawe_tools.egg-info/PKG-INFO` & `smawe_tools-0.3.1/smawe_tools.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: smawe-tools
-Version: 0.3.0
+Version: 0.3.1
 Summary: small tool
 Author: Samwe
 Author-email: 1281722462@qq.com
 License: MIT
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: Implementation :: CPython
```

### Comparing `smawe_tools-0.3.0/smawe_tools.egg-info/SOURCES.txt` & `smawe_tools-0.3.1/smawe_tools.egg-info/SOURCES.txt`

 * *Files 12% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 LICENSE
 README.md
 setup.py
 smawe_tools/__init__.py
 smawe_tools/__version__.py
 smawe_tools/algorithm.py
 smawe_tools/config.py
+smawe_tools/mail_gui.py
 smawe_tools/settings.py
 smawe_tools/tool.py
 smawe_tools/utils.py
 smawe_tools.egg-info/PKG-INFO
 smawe_tools.egg-info/SOURCES.txt
 smawe_tools.egg-info/dependency_links.txt
 smawe_tools.egg-info/requires.txt
```

