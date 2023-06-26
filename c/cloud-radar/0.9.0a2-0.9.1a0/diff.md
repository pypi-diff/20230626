# Comparing `tmp/cloud_radar-0.9.0a2.tar.gz` & `tmp/cloud_radar-0.9.1a0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cloud_radar-0.9.0a2.tar", max compression
+gzip compressed data, was "cloud_radar-0.9.1a0.tar", max compression
```

## Comparing `cloud_radar-0.9.0a2.tar` & `cloud_radar-0.9.1a0.tar`

### file list

```diff
@@ -1,16 +1,16 @@
--rw-r--r--   0        0        0    11357 2023-06-23 19:30:23.828901 cloud_radar-0.9.0a2/LICENSE.txt
--rw-r--r--   0        0        0    14071 2023-06-23 19:30:23.828901 cloud_radar-0.9.0a2/README.md
--rw-r--r--   0        0        0     1435 2023-06-23 19:30:34.765111 cloud_radar-0.9.0a2/pyproject.toml
--rw-r--r--   0        0        0        0 2023-06-23 19:30:23.828901 cloud_radar-0.9.0a2/src/cloud_radar/__init__.py
--rw-r--r--   0        0        0        0 2023-06-23 19:30:23.828901 cloud_radar-0.9.0a2/src/cloud_radar/cf/__init__.py
--rw-r--r--   0        0        0       48 2023-06-23 19:30:23.828901 cloud_radar-0.9.0a2/src/cloud_radar/cf/e2e/__init__.py
--rw-r--r--   0        0        0     1677 2023-06-23 19:30:23.828901 cloud_radar-0.9.0a2/src/cloud_radar/cf/e2e/_stack.py
--rw-r--r--   0        0        0       57 2023-06-23 19:30:23.828901 cloud_radar-0.9.0a2/src/cloud_radar/cf/unit/__init__.py
--rw-r--r--   0        0        0      711 2023-06-23 19:30:23.828901 cloud_radar-0.9.0a2/src/cloud_radar/cf/unit/_condition.py
--rw-r--r--   0        0        0     1822 2023-06-23 19:30:23.828901 cloud_radar-0.9.0a2/src/cloud_radar/cf/unit/_output.py
--rw-r--r--   0        0        0     3199 2023-06-23 19:30:23.828901 cloud_radar-0.9.0a2/src/cloud_radar/cf/unit/_parameter.py
--rw-r--r--   0        0        0     3872 2023-06-23 19:30:23.828901 cloud_radar-0.9.0a2/src/cloud_radar/cf/unit/_resource.py
--rw-r--r--   0        0        0     5230 2023-06-23 19:30:23.832901 cloud_radar-0.9.0a2/src/cloud_radar/cf/unit/_stack.py
--rw-r--r--   0        0        0    23707 2023-06-23 19:30:23.832901 cloud_radar-0.9.0a2/src/cloud_radar/cf/unit/_template.py
--rw-r--r--   0        0        0    24791 2023-06-23 19:30:23.832901 cloud_radar-0.9.0a2/src/cloud_radar/cf/unit/functions.py
--rw-r--r--   0        0        0    15227 1970-01-01 00:00:00.000000 cloud_radar-0.9.0a2/PKG-INFO
+-rw-r--r--   0        0        0    11357 2023-06-26 05:24:10.268731 cloud_radar-0.9.1a0/LICENSE.txt
+-rw-r--r--   0        0        0    14071 2023-06-26 05:24:10.268731 cloud_radar-0.9.1a0/README.md
+-rw-r--r--   0        0        0     1435 2023-06-26 05:24:22.433448 cloud_radar-0.9.1a0/pyproject.toml
+-rw-r--r--   0        0        0        0 2023-06-26 05:24:10.268731 cloud_radar-0.9.1a0/src/cloud_radar/__init__.py
+-rw-r--r--   0        0        0        0 2023-06-26 05:24:10.268731 cloud_radar-0.9.1a0/src/cloud_radar/cf/__init__.py
+-rw-r--r--   0        0        0       48 2023-06-26 05:24:10.268731 cloud_radar-0.9.1a0/src/cloud_radar/cf/e2e/__init__.py
+-rw-r--r--   0        0        0     1677 2023-06-26 05:24:10.268731 cloud_radar-0.9.1a0/src/cloud_radar/cf/e2e/_stack.py
+-rw-r--r--   0        0        0       57 2023-06-26 05:24:10.268731 cloud_radar-0.9.1a0/src/cloud_radar/cf/unit/__init__.py
+-rw-r--r--   0        0        0      711 2023-06-26 05:24:10.268731 cloud_radar-0.9.1a0/src/cloud_radar/cf/unit/_condition.py
+-rw-r--r--   0        0        0     1822 2023-06-26 05:24:10.268731 cloud_radar-0.9.1a0/src/cloud_radar/cf/unit/_output.py
+-rw-r--r--   0        0        0     3199 2023-06-26 05:24:10.268731 cloud_radar-0.9.1a0/src/cloud_radar/cf/unit/_parameter.py
+-rw-r--r--   0        0        0     3872 2023-06-26 05:24:10.268731 cloud_radar-0.9.1a0/src/cloud_radar/cf/unit/_resource.py
+-rw-r--r--   0        0        0     5230 2023-06-26 05:24:10.268731 cloud_radar-0.9.1a0/src/cloud_radar/cf/unit/_stack.py
+-rw-r--r--   0        0        0    23707 2023-06-26 05:24:10.268731 cloud_radar-0.9.1a0/src/cloud_radar/cf/unit/_template.py
+-rw-r--r--   0        0        0    24791 2023-06-26 05:24:10.268731 cloud_radar-0.9.1a0/src/cloud_radar/cf/unit/functions.py
+-rw-r--r--   0        0        0    15227 1970-01-01 00:00:00.000000 cloud_radar-0.9.1a0/PKG-INFO
```

### Comparing `cloud_radar-0.9.0a2/LICENSE.txt` & `cloud_radar-0.9.1a0/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `cloud_radar-0.9.0a2/README.md` & `cloud_radar-0.9.1a0/README.md`

 * *Files identical despite different names*

### Comparing `cloud_radar-0.9.0a2/pyproject.toml` & `cloud_radar-0.9.1a0/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "cloud-radar"
-version = "0.9.0a2"
+version = "0.9.1a0"
 description = "Run functional tests on cloudformation stacks."
 readme = "README.md"
 authors = ["Levi Blaney <shadycuz@gmail.com>"]
 license = "Apache-2.0"
 repository = "https://github.com/DontShaveTheYak/cloud-radar"
 keywords = ["aws", "cloudformation", "cloud-radar", "testing", "taskcat", "cloud", "radar"]
 classifiers = [
```

### Comparing `cloud_radar-0.9.0a2/src/cloud_radar/cf/e2e/_stack.py` & `cloud_radar-0.9.1a0/src/cloud_radar/cf/e2e/_stack.py`

 * *Files identical despite different names*

### Comparing `cloud_radar-0.9.0a2/src/cloud_radar/cf/unit/_condition.py` & `cloud_radar-0.9.1a0/src/cloud_radar/cf/unit/_condition.py`

 * *Files identical despite different names*

### Comparing `cloud_radar-0.9.0a2/src/cloud_radar/cf/unit/_output.py` & `cloud_radar-0.9.1a0/src/cloud_radar/cf/unit/_output.py`

 * *Files identical despite different names*

### Comparing `cloud_radar-0.9.0a2/src/cloud_radar/cf/unit/_parameter.py` & `cloud_radar-0.9.1a0/src/cloud_radar/cf/unit/_parameter.py`

 * *Files identical despite different names*

### Comparing `cloud_radar-0.9.0a2/src/cloud_radar/cf/unit/_resource.py` & `cloud_radar-0.9.1a0/src/cloud_radar/cf/unit/_resource.py`

 * *Files identical despite different names*

### Comparing `cloud_radar-0.9.0a2/src/cloud_radar/cf/unit/_stack.py` & `cloud_radar-0.9.1a0/src/cloud_radar/cf/unit/_stack.py`

 * *Files identical despite different names*

### Comparing `cloud_radar-0.9.0a2/src/cloud_radar/cf/unit/_template.py` & `cloud_radar-0.9.1a0/src/cloud_radar/cf/unit/_template.py`

 * *Files identical despite different names*

### Comparing `cloud_radar-0.9.0a2/src/cloud_radar/cf/unit/functions.py` & `cloud_radar-0.9.1a0/src/cloud_radar/cf/unit/functions.py`

 * *Files identical despite different names*

### Comparing `cloud_radar-0.9.0a2/PKG-INFO` & `cloud_radar-0.9.1a0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cloud-radar
-Version: 0.9.0a2
+Version: 0.9.1a0
 Summary: Run functional tests on cloudformation stacks.
 Home-page: https://github.com/DontShaveTheYak/cloud-radar
 License: Apache-2.0
 Keywords: aws,cloudformation,cloud-radar,testing,taskcat,cloud,radar
 Author: Levi Blaney
 Author-email: shadycuz@gmail.com
 Requires-Python: >=3.8.1,<4.0.0
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: cloud-radar Version: 0.9.0a2 Summary: Run
+Metadata-Version: 2.1 Name: cloud-radar Version: 0.9.1a0 Summary: Run
 functional tests on cloudformation stacks. Home-page: https://github.com/
 DontShaveTheYak/cloud-radar License: Apache-2.0 Keywords:
 aws,cloudformation,cloud-radar,testing,taskcat,cloud,radar Author: Levi Blaney
 Author-email: shadycuz@gmail.com Requires-Python: >=3.8.1,<4.0.0 Classifier:
 Development Status :: 2 - Pre-Alpha Classifier: License :: OSI Approved ::
 Apache Software License Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3 Classifier: Programming
```

