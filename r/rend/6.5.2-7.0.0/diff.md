# Comparing `tmp/rend-6.5.2.tar.gz` & `tmp/rend-7.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "rend-6.5.2.tar", last modified: Tue Feb 28 17:54:20 2023, max compression
+gzip compressed data, was "rend-7.0.0.tar", last modified: Mon Jun 26 15:32:42 2023, max compression
```

## Comparing `rend-6.5.2.tar` & `rend-7.0.0.tar`

### file list

```diff
@@ -1,36 +1,36 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-02-28 17:54:20.023905 rend-6.5.2/
--rw-r--r--   0 root         (0) root         (0)    11342 2023-02-28 17:54:06.000000 rend-6.5.2/LICENSE
--rw-r--r--   0 root         (0) root         (0)     2911 2023-02-28 17:54:20.023905 rend-6.5.2/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     1802 2023-02-28 17:54:06.000000 rend-6.5.2/README.rst
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-02-28 17:54:20.023905 rend-6.5.2/rend/
--rw-r--r--   0 root         (0) root         (0)     1071 2023-02-28 17:54:06.000000 rend-6.5.2/rend/conf.py
--rw-r--r--   0 root         (0) root         (0)      396 2023-02-28 17:54:06.000000 rend-6.5.2/rend/exc.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-02-28 17:54:20.023905 rend-6.5.2/rend/output/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-02-28 17:54:20.023905 rend-6.5.2/rend/output/contracts/
--rw-r--r--   0 root         (0) root         (0)       36 2023-02-28 17:54:06.000000 rend-6.5.2/rend/output/contracts/init.py
--rw-r--r--   0 root         (0) root         (0)      474 2023-02-28 17:54:06.000000 rend-6.5.2/rend/output/json_out.py
--rw-r--r--   0 root         (0) root         (0)     6192 2023-02-28 17:54:06.000000 rend-6.5.2/rend/output/nested.py
--rw-r--r--   0 root         (0) root         (0)      137 2023-02-28 17:54:06.000000 rend-6.5.2/rend/output/pretty.py
--rw-r--r--   0 root         (0) root         (0)       84 2023-02-28 17:54:06.000000 rend-6.5.2/rend/output/raw.py
--rw-r--r--   0 root         (0) root         (0)      621 2023-02-28 17:54:06.000000 rend-6.5.2/rend/output/yaml_out.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-02-28 17:54:20.023905 rend-6.5.2/rend/rend/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-02-28 17:54:20.023905 rend-6.5.2/rend/rend/contracts/
--rw-r--r--   0 root         (0) root         (0)       44 2023-02-28 17:54:06.000000 rend-6.5.2/rend/rend/contracts/init.py
--rw-r--r--   0 root         (0) root         (0)     4584 2023-02-28 17:54:06.000000 rend-6.5.2/rend/rend/init.py
--rw-r--r--   0 root         (0) root         (0)     2740 2023-02-28 17:54:06.000000 rend-6.5.2/rend/rend/jinja.py
--rw-r--r--   0 root         (0) root         (0)      616 2023-02-28 17:54:06.000000 rend-6.5.2/rend/rend/json_file.py
--rw-r--r--   0 root         (0) root         (0)     1597 2023-02-28 17:54:06.000000 rend-6.5.2/rend/rend/k8crd_file.py
--rw-r--r--   0 root         (0) root         (0)      704 2023-02-28 17:54:06.000000 rend-6.5.2/rend/rend/replacements.py
--rw-r--r--   0 root         (0) root         (0)      563 2023-02-28 17:54:06.000000 rend-6.5.2/rend/rend/toml_file.py
--rw-r--r--   0 root         (0) root         (0)     6599 2023-02-28 17:54:06.000000 rend-6.5.2/rend/rend/yaml_file.py
--rw-r--r--   0 root         (0) root         (0)      123 2023-02-28 17:54:06.000000 rend-6.5.2/rend/scripts.py
--rw-r--r--   0 root         (0) root         (0)       18 2023-02-28 17:54:19.000000 rend-6.5.2/rend/version.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-02-28 17:54:20.023905 rend-6.5.2/rend.egg-info/
--rw-r--r--   0 root         (0) root         (0)     2911 2023-02-28 17:54:19.000000 rend-6.5.2/rend.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      589 2023-02-28 17:54:19.000000 rend-6.5.2/rend.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-02-28 17:54:19.000000 rend-6.5.2/rend.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       45 2023-02-28 17:54:19.000000 rend-6.5.2/rend.egg-info/entry_points.txt
--rw-r--r--   0 root         (0) root         (0)       73 2023-02-28 17:54:19.000000 rend-6.5.2/rend.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)        5 2023-02-28 17:54:19.000000 rend-6.5.2/rend.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)       73 2023-02-28 17:54:20.023905 rend-6.5.2/setup.cfg
--rw-r--r--   0 root         (0) root         (0)     3668 2023-02-28 17:54:06.000000 rend-6.5.2/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-26 15:32:41.997318 rend-7.0.0/
+-rw-r--r--   0 root         (0) root         (0)    11342 2023-06-26 15:32:27.000000 rend-7.0.0/LICENSE
+-rw-r--r--   0 root         (0) root         (0)     2912 2023-06-26 15:32:41.997318 rend-7.0.0/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     1802 2023-06-26 15:32:27.000000 rend-7.0.0/README.rst
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-26 15:32:41.997318 rend-7.0.0/rend/
+-rw-r--r--   0 root         (0) root         (0)     1071 2023-06-26 15:32:27.000000 rend-7.0.0/rend/conf.py
+-rw-r--r--   0 root         (0) root         (0)      396 2023-06-26 15:32:27.000000 rend-7.0.0/rend/exc.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-26 15:32:41.997318 rend-7.0.0/rend/output/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-26 15:32:41.997318 rend-7.0.0/rend/output/contracts/
+-rw-r--r--   0 root         (0) root         (0)       36 2023-06-26 15:32:27.000000 rend-7.0.0/rend/output/contracts/init.py
+-rw-r--r--   0 root         (0) root         (0)      474 2023-06-26 15:32:27.000000 rend-7.0.0/rend/output/json_out.py
+-rw-r--r--   0 root         (0) root         (0)     6192 2023-06-26 15:32:27.000000 rend-7.0.0/rend/output/nested.py
+-rw-r--r--   0 root         (0) root         (0)      137 2023-06-26 15:32:27.000000 rend-7.0.0/rend/output/pretty.py
+-rw-r--r--   0 root         (0) root         (0)       84 2023-06-26 15:32:27.000000 rend-7.0.0/rend/output/raw.py
+-rw-r--r--   0 root         (0) root         (0)      622 2023-06-26 15:32:27.000000 rend-7.0.0/rend/output/yaml_out.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-26 15:32:41.997318 rend-7.0.0/rend/rend/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-26 15:32:41.997318 rend-7.0.0/rend/rend/contracts/
+-rw-r--r--   0 root         (0) root         (0)       44 2023-06-26 15:32:27.000000 rend-7.0.0/rend/rend/contracts/init.py
+-rw-r--r--   0 root         (0) root         (0)     4584 2023-06-26 15:32:27.000000 rend-7.0.0/rend/rend/init.py
+-rw-r--r--   0 root         (0) root         (0)     2740 2023-06-26 15:32:27.000000 rend-7.0.0/rend/rend/jinja.py
+-rw-r--r--   0 root         (0) root         (0)      616 2023-06-26 15:32:27.000000 rend-7.0.0/rend/rend/json_file.py
+-rw-r--r--   0 root         (0) root         (0)     1597 2023-06-26 15:32:27.000000 rend-7.0.0/rend/rend/k8crd_file.py
+-rw-r--r--   0 root         (0) root         (0)      704 2023-06-26 15:32:27.000000 rend-7.0.0/rend/rend/replacements.py
+-rw-r--r--   0 root         (0) root         (0)      563 2023-06-26 15:32:27.000000 rend-7.0.0/rend/rend/toml_file.py
+-rw-r--r--   0 root         (0) root         (0)     6599 2023-06-26 15:32:27.000000 rend-7.0.0/rend/rend/yaml_file.py
+-rw-r--r--   0 root         (0) root         (0)      123 2023-06-26 15:32:27.000000 rend-7.0.0/rend/scripts.py
+-rw-r--r--   0 root         (0) root         (0)       18 2023-06-26 15:32:41.000000 rend-7.0.0/rend/version.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-26 15:32:41.997318 rend-7.0.0/rend.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     2912 2023-06-26 15:32:41.000000 rend-7.0.0/rend.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      589 2023-06-26 15:32:41.000000 rend-7.0.0/rend.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-06-26 15:32:41.000000 rend-7.0.0/rend.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       45 2023-06-26 15:32:41.000000 rend-7.0.0/rend.egg-info/entry_points.txt
+-rw-r--r--   0 root         (0) root         (0)       73 2023-06-26 15:32:41.000000 rend-7.0.0/rend.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)        5 2023-06-26 15:32:41.000000 rend-7.0.0/rend.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)       73 2023-06-26 15:32:41.997318 rend-7.0.0/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)     3669 2023-06-26 15:32:27.000000 rend-7.0.0/setup.py
```

### Comparing `rend-6.5.2/LICENSE` & `rend-7.0.0/LICENSE`

 * *Files identical despite different names*

### Comparing `rend-6.5.2/PKG-INFO` & `rend-7.0.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,31 +1,31 @@
 Metadata-Version: 2.1
 Name: rend
-Version: 6.5.2
+Version: 7.0.0
 Summary: A collection of tools to render text files into data structures
 Home-page: https://vmware.gitlab.io/pop/rend/en/latest/index.html
 Author: VMware, Inc.
 Author-email: idemproject@vmware.com
 License: Apache Software License 2.0
 Project-URL: Code, https://gitlab.com/vmware/pop/rend
 Project-URL: Issue tracker, https://gitlab.com/vmware/pop/rend/issues
 Platform: UNKNOWN
 Classifier: Environment :: Console
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: Information Technology
 Classifier: Intended Audience :: System Administrators
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python
-Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: License :: OSI Approved :: Apache Software License
-Requires-Python: >=3.7
+Requires-Python: >=3.8
 Description-Content-Type: text/x-rst
 License-File: LICENSE
 
 ====
 rend
 ====
```

### Comparing `rend-6.5.2/README.rst` & `rend-7.0.0/README.rst`

 * *Files identical despite different names*

### Comparing `rend-6.5.2/rend/conf.py` & `rend-7.0.0/rend/conf.py`

 * *Files identical despite different names*

### Comparing `rend-6.5.2/rend/output/nested.py` & `rend-7.0.0/rend/output/nested.py`

 * *Files identical despite different names*

### Comparing `rend-6.5.2/rend/output/yaml_out.py` & `rend-7.0.0/rend/output/yaml_out.py`

 * *Files 19% similar despite different names*

```diff
@@ -5,14 +5,15 @@
 __virtualname__ = "yaml"
 
 
 def display(hub, data):
     """
     Print the raw data
     """
+
     # # yaml safe_dump doesn't know how to represent subclasses of dict.
     # # this registration allows arbitrary dict types to be represented
     # # without conversion to a regular dict.
     def any_dict_representer(dumper, data):
         return dumper.represent_dict(data)
 
     yaml.add_multi_representer(dict, any_dict_representer, Dumper=yaml.SafeDumper)
```

### Comparing `rend-6.5.2/rend/rend/init.py` & `rend-7.0.0/rend/rend/init.py`

 * *Files identical despite different names*

### Comparing `rend-6.5.2/rend/rend/jinja.py` & `rend-7.0.0/rend/rend/jinja.py`

 * *Files identical despite different names*

### Comparing `rend-6.5.2/rend/rend/json_file.py` & `rend-7.0.0/rend/rend/json_file.py`

 * *Files identical despite different names*

### Comparing `rend-6.5.2/rend/rend/k8crd_file.py` & `rend-7.0.0/rend/rend/k8crd_file.py`

 * *Files identical despite different names*

### Comparing `rend-6.5.2/rend/rend/replacements.py` & `rend-7.0.0/rend/rend/replacements.py`

 * *Files identical despite different names*

### Comparing `rend-6.5.2/rend/rend/toml_file.py` & `rend-7.0.0/rend/rend/toml_file.py`

 * *Files identical despite different names*

### Comparing `rend-6.5.2/rend/rend/yaml_file.py` & `rend-7.0.0/rend/rend/yaml_file.py`

 * *Files identical despite different names*

### Comparing `rend-6.5.2/rend.egg-info/PKG-INFO` & `rend-7.0.0/rend.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,31 +1,31 @@
 Metadata-Version: 2.1
 Name: rend
-Version: 6.5.2
+Version: 7.0.0
 Summary: A collection of tools to render text files into data structures
 Home-page: https://vmware.gitlab.io/pop/rend/en/latest/index.html
 Author: VMware, Inc.
 Author-email: idemproject@vmware.com
 License: Apache Software License 2.0
 Project-URL: Code, https://gitlab.com/vmware/pop/rend
 Project-URL: Issue tracker, https://gitlab.com/vmware/pop/rend/issues
 Platform: UNKNOWN
 Classifier: Environment :: Console
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: Information Technology
 Classifier: Intended Audience :: System Administrators
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python
-Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: License :: OSI Approved :: Apache Software License
-Requires-Python: >=3.7
+Requires-Python: >=3.8
 Description-Content-Type: text/x-rst
 License-File: LICENSE
 
 ====
 rend
 ====
```

### Comparing `rend-6.5.2/rend.egg-info/SOURCES.txt` & `rend-7.0.0/rend.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `rend-6.5.2/setup.py` & `rend-7.0.0/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -89,27 +89,27 @@
     },
     version=VERSION,
     install_requires=REQUIREMENTS,
     extras_require=REQUIREMENTS_EXTRA,
     description=DESC,
     long_description=LONG_DESC,
     long_description_content_type="text/x-rst",
-    python_requires=">=3.7",
+    python_requires=">=3.8",
     license="Apache Software License 2.0",
     classifiers=[
         "Environment :: Console",
         "Intended Audience :: Developers",
         "Intended Audience :: Information Technology",
         "Intended Audience :: System Administrators",
         "Operating System :: OS Independent",
         "Programming Language :: Python",
-        "Programming Language :: Python :: 3.7",
         "Programming Language :: Python :: 3.8",
         "Programming Language :: Python :: 3.9",
         "Programming Language :: Python :: 3.10",
+        "Programming Language :: Python :: 3.11",
         "Development Status :: 5 - Production/Stable",
         "License :: OSI Approved :: Apache Software License",
     ],
     entry_points={
         "console_scripts": [
             "rend = rend.scripts:start",
         ],
```

