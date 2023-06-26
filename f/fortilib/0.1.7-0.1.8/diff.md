# Comparing `tmp/fortilib-0.1.7.tar.gz` & `tmp/fortilib-0.1.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "fortilib-0.1.7.tar", max compression
+gzip compressed data, was "fortilib-0.1.8.tar", max compression
```

## Comparing `fortilib-0.1.7.tar` & `fortilib-0.1.8.tar`

### file list

```diff
@@ -1,26 +1,26 @@
--rw-r--r--   0        0        0    35149 2023-06-26 06:08:41.915610 fortilib-0.1.7/LICENSE
--rw-r--r--   0        0        0     1423 2023-06-26 06:08:41.915610 fortilib-0.1.7/README.md
--rw-r--r--   0        0        0      530 2023-06-26 06:08:41.915610 fortilib-0.1.7/fortilib/__init__.py
--rw-r--r--   0        0        0     4616 2023-06-26 06:08:41.915610 fortilib-0.1.7/fortilib/address.py
--rw-r--r--   0        0        0     1456 2023-06-26 06:08:41.915610 fortilib-0.1.7/fortilib/addressgroup.py
--rw-r--r--   0        0        0     1925 2023-06-26 06:08:41.915610 fortilib-0.1.7/fortilib/base.py
--rw-r--r--   0        0        0     1403 2023-06-26 06:08:41.915610 fortilib-0.1.7/fortilib/exceptions.py
--rw-r--r--   0        0        0    30493 2023-06-26 06:08:41.915610 fortilib-0.1.7/fortilib/firewall.py
--rw-r--r--   0        0        0    35749 2023-06-26 06:08:41.919611 fortilib-0.1.7/fortilib/fortigateapi.py
--rw-r--r--   0        0        0      338 2023-06-26 06:08:41.919611 fortilib-0.1.7/fortilib/fortilib.iml
--rw-r--r--   0        0        0     1625 2023-06-26 06:08:41.919611 fortilib-0.1.7/fortilib/interface.py
--rw-r--r--   0        0        0     2186 2023-06-26 06:08:41.919611 fortilib-0.1.7/fortilib/ippool.py
--rw-r--r--   0        0        0        0 2023-06-26 06:08:41.919611 fortilib-0.1.7/fortilib/mixins/__init__.py
--rw-r--r--   0        0        0      637 2023-06-26 06:08:41.919611 fortilib-0.1.7/fortilib/mixins/group.py
--rw-r--r--   0        0        0      635 2023-06-26 06:08:41.919611 fortilib-0.1.7/fortilib/mixins/interface.py
--rw-r--r--   0        0        0    10030 2023-06-26 06:08:41.919611 fortilib-0.1.7/fortilib/policy.py
--rw-r--r--   0        0        0     1690 2023-06-26 06:08:41.919611 fortilib-0.1.7/fortilib/proxyaddress.py
--rw-r--r--   0        0        0     1760 2023-06-26 06:08:41.919611 fortilib-0.1.7/fortilib/proxyaddressgroup.py
--rw-r--r--   0        0        0    10406 2023-06-26 06:08:41.919611 fortilib-0.1.7/fortilib/proxypolicy.py
--rw-r--r--   0        0        0     2918 2023-06-26 06:08:41.919611 fortilib-0.1.7/fortilib/routes.py
--rw-r--r--   0        0        0     6579 2023-06-26 06:08:41.919611 fortilib-0.1.7/fortilib/service.py
--rw-r--r--   0        0        0     1682 2023-06-26 06:08:41.919611 fortilib-0.1.7/fortilib/servicegroup.py
--rw-r--r--   0        0        0     5249 2023-06-26 06:08:41.919611 fortilib-0.1.7/fortilib/vip.py
--rw-r--r--   0        0        0     1795 2023-06-26 06:08:41.919611 fortilib-0.1.7/fortilib/vipgroup.py
--rw-r--r--   0        0        0     1207 2023-06-26 06:08:41.919611 fortilib-0.1.7/pyproject.toml
--rw-r--r--   0        0        0     2353 1970-01-01 00:00:00.000000 fortilib-0.1.7/PKG-INFO
+-rw-r--r--   0        0        0    35149 2023-06-26 06:12:43.195049 fortilib-0.1.8/LICENSE
+-rw-r--r--   0        0        0     1423 2023-06-26 06:12:43.195049 fortilib-0.1.8/README.md
+-rw-r--r--   0        0        0      530 2023-06-26 06:12:43.195049 fortilib-0.1.8/fortilib/__init__.py
+-rw-r--r--   0        0        0     4616 2023-06-26 06:12:43.195049 fortilib-0.1.8/fortilib/address.py
+-rw-r--r--   0        0        0     1456 2023-06-26 06:12:43.195049 fortilib-0.1.8/fortilib/addressgroup.py
+-rw-r--r--   0        0        0     1925 2023-06-26 06:12:43.195049 fortilib-0.1.8/fortilib/base.py
+-rw-r--r--   0        0        0     1403 2023-06-26 06:12:43.195049 fortilib-0.1.8/fortilib/exceptions.py
+-rw-r--r--   0        0        0    30493 2023-06-26 06:12:43.195049 fortilib-0.1.8/fortilib/firewall.py
+-rw-r--r--   0        0        0    35749 2023-06-26 06:12:43.195049 fortilib-0.1.8/fortilib/fortigateapi.py
+-rw-r--r--   0        0        0      338 2023-06-26 06:12:43.195049 fortilib-0.1.8/fortilib/fortilib.iml
+-rw-r--r--   0        0        0     1625 2023-06-26 06:12:43.195049 fortilib-0.1.8/fortilib/interface.py
+-rw-r--r--   0        0        0     2186 2023-06-26 06:12:43.195049 fortilib-0.1.8/fortilib/ippool.py
+-rw-r--r--   0        0        0        0 2023-06-26 06:12:43.199049 fortilib-0.1.8/fortilib/mixins/__init__.py
+-rw-r--r--   0        0        0      637 2023-06-26 06:12:43.199049 fortilib-0.1.8/fortilib/mixins/group.py
+-rw-r--r--   0        0        0      635 2023-06-26 06:12:43.199049 fortilib-0.1.8/fortilib/mixins/interface.py
+-rw-r--r--   0        0        0    10030 2023-06-26 06:12:43.199049 fortilib-0.1.8/fortilib/policy.py
+-rw-r--r--   0        0        0     1690 2023-06-26 06:12:43.199049 fortilib-0.1.8/fortilib/proxyaddress.py
+-rw-r--r--   0        0        0     1760 2023-06-26 06:12:43.199049 fortilib-0.1.8/fortilib/proxyaddressgroup.py
+-rw-r--r--   0        0        0    10406 2023-06-26 06:12:43.199049 fortilib-0.1.8/fortilib/proxypolicy.py
+-rw-r--r--   0        0        0     2918 2023-06-26 06:12:43.199049 fortilib-0.1.8/fortilib/routes.py
+-rw-r--r--   0        0        0     6579 2023-06-26 06:12:43.199049 fortilib-0.1.8/fortilib/service.py
+-rw-r--r--   0        0        0     1682 2023-06-26 06:12:43.199049 fortilib-0.1.8/fortilib/servicegroup.py
+-rw-r--r--   0        0        0     5249 2023-06-26 06:12:43.199049 fortilib-0.1.8/fortilib/vip.py
+-rw-r--r--   0        0        0     1795 2023-06-26 06:12:43.199049 fortilib-0.1.8/fortilib/vipgroup.py
+-rw-r--r--   0        0        0     1227 2023-06-26 06:12:43.199049 fortilib-0.1.8/pyproject.toml
+-rw-r--r--   0        0        0     2373 1970-01-01 00:00:00.000000 fortilib-0.1.8/PKG-INFO
```

### Comparing `fortilib-0.1.7/LICENSE` & `fortilib-0.1.8/LICENSE`

 * *Files identical despite different names*

### Comparing `fortilib-0.1.7/README.md` & `fortilib-0.1.8/README.md`

 * *Files identical despite different names*

### Comparing `fortilib-0.1.7/fortilib/__init__.py` & `fortilib-0.1.8/fortilib/__init__.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-__version__ = "0.1.7"
+__version__ = "0.1.8"
 
 from typing import (
     Dict,
     List,
 )
```

### Comparing `fortilib-0.1.7/fortilib/address.py` & `fortilib-0.1.8/fortilib/address.py`

 * *Files identical despite different names*

### Comparing `fortilib-0.1.7/fortilib/addressgroup.py` & `fortilib-0.1.8/fortilib/addressgroup.py`

 * *Files identical despite different names*

### Comparing `fortilib-0.1.7/fortilib/base.py` & `fortilib-0.1.8/fortilib/base.py`

 * *Files identical despite different names*

### Comparing `fortilib-0.1.7/fortilib/exceptions.py` & `fortilib-0.1.8/fortilib/exceptions.py`

 * *Files identical despite different names*

### Comparing `fortilib-0.1.7/fortilib/firewall.py` & `fortilib-0.1.8/fortilib/firewall.py`

 * *Files identical despite different names*

### Comparing `fortilib-0.1.7/fortilib/fortigateapi.py` & `fortilib-0.1.8/fortilib/fortigateapi.py`

 * *Files identical despite different names*

### Comparing `fortilib-0.1.7/fortilib/interface.py` & `fortilib-0.1.8/fortilib/interface.py`

 * *Files identical despite different names*

### Comparing `fortilib-0.1.7/fortilib/ippool.py` & `fortilib-0.1.8/fortilib/ippool.py`

 * *Files identical despite different names*

### Comparing `fortilib-0.1.7/fortilib/mixins/group.py` & `fortilib-0.1.8/fortilib/mixins/group.py`

 * *Files identical despite different names*

### Comparing `fortilib-0.1.7/fortilib/mixins/interface.py` & `fortilib-0.1.8/fortilib/mixins/interface.py`

 * *Files identical despite different names*

### Comparing `fortilib-0.1.7/fortilib/policy.py` & `fortilib-0.1.8/fortilib/policy.py`

 * *Files identical despite different names*

### Comparing `fortilib-0.1.7/fortilib/proxyaddress.py` & `fortilib-0.1.8/fortilib/proxyaddress.py`

 * *Files identical despite different names*

### Comparing `fortilib-0.1.7/fortilib/proxyaddressgroup.py` & `fortilib-0.1.8/fortilib/proxyaddressgroup.py`

 * *Files identical despite different names*

### Comparing `fortilib-0.1.7/fortilib/proxypolicy.py` & `fortilib-0.1.8/fortilib/proxypolicy.py`

 * *Files identical despite different names*

### Comparing `fortilib-0.1.7/fortilib/routes.py` & `fortilib-0.1.8/fortilib/routes.py`

 * *Files identical despite different names*

### Comparing `fortilib-0.1.7/fortilib/service.py` & `fortilib-0.1.8/fortilib/service.py`

 * *Files identical despite different names*

### Comparing `fortilib-0.1.7/fortilib/servicegroup.py` & `fortilib-0.1.8/fortilib/servicegroup.py`

 * *Files identical despite different names*

### Comparing `fortilib-0.1.7/fortilib/vip.py` & `fortilib-0.1.8/fortilib/vip.py`

 * *Files identical despite different names*

### Comparing `fortilib-0.1.7/fortilib/vipgroup.py` & `fortilib-0.1.8/fortilib/vipgroup.py`

 * *Files identical despite different names*

### Comparing `fortilib-0.1.7/pyproject.toml` & `fortilib-0.1.8/pyproject.toml`

 * *Files 16% similar despite different names*

```diff
@@ -1,27 +1,27 @@
 [tool.poetry]
 name = "fortilib"
-version = "0.1.7"
+version = "0.1.8"
 description = "fortilib - a Python Library to interact with Fortigate Firewalls"
 readme = "README.md"
 authors = [
     "Daniel Zinke <Daniel.Zinke@t-systems.com>",
     "Benjamin Böhm <Benjamin.Boehm@t-systems.com>",
     "Philipp Funk <Philipp.Funk@t-systems.com>",
     "André Ellguth <Andre.Ellguth@t-systems.com>",
     "Martin Neubert <Martin.Neubert@t-systems.com>"
 ]
 license = "GPL-3.0-only"
-homepage = "https://github.com/neubi4/fortilib"
-repository = "https://github.com/neubi4/fortilib"
-documentation = "https://github.com/neubi4/fortilib"
+homepage = "https://github.com/telekom-mms/fortilib"
+repository = "https://github.com/telekom-mms/fortilib"
+documentation = "https://github.com/telekom-mms/fortilib"
 keywords = ["firewall", "fortinet", "fortigate"]
 
 [tool.poetry.urls]
-Changelog = "https://github.com/neubi4/fortilib/blob/master/CHANGELOG.md"
+Changelog = "https://github.com/telekom-mms/fortilib/blob/master/CHANGELOG.md"
 
 [tool.poetry.dependencies]
 python = ">=3.8,<4.0"
 httpx = ">=0.23.0"
 
 [tool.poetry.dev-dependencies]
 pytest = ">=7.1.2"
```

### Comparing `fortilib-0.1.7/PKG-INFO` & `fortilib-0.1.8/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,27 +1,27 @@
 Metadata-Version: 2.1
 Name: fortilib
-Version: 0.1.7
+Version: 0.1.8
 Summary: fortilib - a Python Library to interact with Fortigate Firewalls
-Home-page: https://github.com/neubi4/fortilib
+Home-page: https://github.com/telekom-mms/fortilib
 License: GPL-3.0-only
 Keywords: firewall,fortinet,fortigate
 Author: Daniel Zinke
 Author-email: Daniel.Zinke@t-systems.com
 Requires-Python: >=3.8,<4.0
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Requires-Dist: httpx (>=0.23.0)
-Project-URL: Changelog, https://github.com/neubi4/fortilib/blob/master/CHANGELOG.md
-Project-URL: Documentation, https://github.com/neubi4/fortilib
-Project-URL: Repository, https://github.com/neubi4/fortilib
+Project-URL: Changelog, https://github.com/telekom-mms/fortilib/blob/master/CHANGELOG.md
+Project-URL: Documentation, https://github.com/telekom-mms/fortilib
+Project-URL: Repository, https://github.com/telekom-mms/fortilib
 Description-Content-Type: text/markdown
 
 # fortilib - a Python Library to interact with Fortigate Firewalls
 
 This Python module contains the ability to get and configure following object on [Fortigate Firewalls](https://www.fortinet.com/products/next-generation-firewall):
 * Addresses
 * Address Groups
```

