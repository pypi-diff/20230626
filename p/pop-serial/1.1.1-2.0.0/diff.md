# Comparing `tmp/pop-serial-1.1.1.tar.gz` & `tmp/pop-serial-2.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pop-serial-1.1.1.tar", last modified: Thu Nov  3 22:00:01 2022, max compression
+gzip compressed data, was "pop-serial-2.0.0.tar", last modified: Mon Jun 26 15:23:19 2023, max compression
```

## Comparing `pop-serial-1.1.1.tar` & `pop-serial-2.0.0.tar`

### file list

```diff
@@ -1,22 +1,22 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-11-03 22:00:01.893625 pop-serial-1.1.1/
--rw-r--r--   0 root         (0) root         (0)    11342 2022-11-03 21:59:39.000000 pop-serial-1.1.1/LICENSE
--rw-r--r--   0 root         (0) root         (0)     3273 2022-11-03 22:00:01.893625 pop-serial-1.1.1/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     2098 2022-11-03 21:59:39.000000 pop-serial-1.1.1/README.rst
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-11-03 22:00:01.891625 pop-serial-1.1.1/pop_serial/
--rw-r--r--   0 root         (0) root         (0)       30 2022-11-03 21:59:39.000000 pop-serial-1.1.1/pop_serial/conf.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-11-03 22:00:01.892625 pop-serial-1.1.1/pop_serial/serial/
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-11-03 22:00:01.892625 pop-serial-1.1.1/pop_serial/serial/contracts/
--rw-r--r--   0 root         (0) root         (0)       84 2022-11-03 21:59:39.000000 pop-serial-1.1.1/pop_serial/serial/contracts/init.py
--rw-r--r--   0 root         (0) root         (0)      396 2022-11-03 21:59:39.000000 pop-serial-1.1.1/pop_serial/serial/json_serial.py
--rw-r--r--   0 root         (0) root         (0)      403 2022-11-03 21:59:39.000000 pop-serial-1.1.1/pop_serial/serial/msgpack_serial.py
--rw-r--r--   0 root         (0) root         (0)      287 2022-11-03 21:59:39.000000 pop-serial-1.1.1/pop_serial/serial/str_serial.py
--rw-r--r--   0 root         (0) root         (0)       18 2022-11-03 22:00:01.000000 pop-serial-1.1.1/pop_serial/version.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-11-03 22:00:01.892625 pop-serial-1.1.1/pop_serial.egg-info/
--rw-r--r--   0 root         (0) root         (0)     3273 2022-11-03 22:00:01.000000 pop-serial-1.1.1/pop_serial.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      421 2022-11-03 22:00:01.000000 pop-serial-1.1.1/pop_serial.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2022-11-03 22:00:01.000000 pop-serial-1.1.1/pop_serial.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       20 2022-11-03 22:00:01.000000 pop-serial-1.1.1/pop_serial.egg-info/entry_points.txt
--rw-r--r--   0 root         (0) root         (0)       12 2022-11-03 22:00:01.000000 pop-serial-1.1.1/pop_serial.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       11 2022-11-03 22:00:01.000000 pop-serial-1.1.1/pop_serial.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)       73 2022-11-03 22:00:01.893625 pop-serial-1.1.1/setup.cfg
--rw-r--r--   0 root         (0) root         (0)     3154 2022-11-03 21:59:39.000000 pop-serial-1.1.1/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-26 15:23:19.879111 pop-serial-2.0.0/
+-rw-r--r--   0 root         (0) root         (0)    11342 2023-06-26 15:23:06.000000 pop-serial-2.0.0/LICENSE
+-rw-r--r--   0 root         (0) root         (0)     3274 2023-06-26 15:23:19.879111 pop-serial-2.0.0/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     2098 2023-06-26 15:23:06.000000 pop-serial-2.0.0/README.rst
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-26 15:23:19.879111 pop-serial-2.0.0/pop_serial/
+-rw-r--r--   0 root         (0) root         (0)       30 2023-06-26 15:23:06.000000 pop-serial-2.0.0/pop_serial/conf.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-26 15:23:19.879111 pop-serial-2.0.0/pop_serial/serial/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-26 15:23:19.879111 pop-serial-2.0.0/pop_serial/serial/contracts/
+-rw-r--r--   0 root         (0) root         (0)       84 2023-06-26 15:23:06.000000 pop-serial-2.0.0/pop_serial/serial/contracts/init.py
+-rw-r--r--   0 root         (0) root         (0)      396 2023-06-26 15:23:06.000000 pop-serial-2.0.0/pop_serial/serial/json_serial.py
+-rw-r--r--   0 root         (0) root         (0)      403 2023-06-26 15:23:06.000000 pop-serial-2.0.0/pop_serial/serial/msgpack_serial.py
+-rw-r--r--   0 root         (0) root         (0)      287 2023-06-26 15:23:06.000000 pop-serial-2.0.0/pop_serial/serial/str_serial.py
+-rw-r--r--   0 root         (0) root         (0)       18 2023-06-26 15:23:19.000000 pop-serial-2.0.0/pop_serial/version.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-26 15:23:19.879111 pop-serial-2.0.0/pop_serial.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     3274 2023-06-26 15:23:19.000000 pop-serial-2.0.0/pop_serial.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      421 2023-06-26 15:23:19.000000 pop-serial-2.0.0/pop_serial.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-06-26 15:23:19.000000 pop-serial-2.0.0/pop_serial.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       20 2023-06-26 15:23:19.000000 pop-serial-2.0.0/pop_serial.egg-info/entry_points.txt
+-rw-r--r--   0 root         (0) root         (0)       12 2023-06-26 15:23:19.000000 pop-serial-2.0.0/pop_serial.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       11 2023-06-26 15:23:19.000000 pop-serial-2.0.0/pop_serial.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)       73 2023-06-26 15:23:19.879111 pop-serial-2.0.0/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)     3155 2023-06-26 15:23:06.000000 pop-serial-2.0.0/setup.py
```

### Comparing `pop-serial-1.1.1/LICENSE` & `pop-serial-2.0.0/LICENSE`

 * *Files identical despite different names*

### Comparing `pop-serial-1.1.1/PKG-INFO` & `pop-serial-2.0.0/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,31 +1,31 @@
 Metadata-Version: 2.1
 Name: pop-serial
-Version: 1.1.1
+Version: 2.0.0
 Summary: An app-merge component for larger projects that provides a standardized interface for serializing and de-serializing data.
 Home-page: https://gitlab.com/vmware/idem/pop-serial
 Author: VMware, Inc.
 Author-email: idemproject@vmware.com
 License: Apache Software License 2.0
 Project-URL: Code, https://gitlab.com/vmware/idem/pop-serial
 Project-URL: Issue tracker, https://gitlab.com/vmware/idem/pop-serial/issues
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
 
 ==========
 pop-serial
 ==========
 
@@ -56,15 +56,15 @@
 
 Getting Started
 ===============
 
 Prerequisites
 -------------
 
-* Python 3.7+
+* Python 3.8+
 * git *(if installing from source, or contributing to the project)*
 
 Installation
 ------------
 
 .. note::
```

### Comparing `pop-serial-1.1.1/README.rst` & `pop-serial-2.0.0/README.rst`

 * *Files 1% similar despite different names*

```diff
@@ -29,15 +29,15 @@
 
 Getting Started
 ===============
 
 Prerequisites
 -------------
 
-* Python 3.7+
+* Python 3.8+
 * git *(if installing from source, or contributing to the project)*
 
 Installation
 ------------
 
 .. note::
```

### Comparing `pop-serial-1.1.1/pop_serial.egg-info/PKG-INFO` & `pop-serial-2.0.0/pop_serial.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,31 +1,31 @@
 Metadata-Version: 2.1
 Name: pop-serial
-Version: 1.1.1
+Version: 2.0.0
 Summary: An app-merge component for larger projects that provides a standardized interface for serializing and de-serializing data.
 Home-page: https://gitlab.com/vmware/idem/pop-serial
 Author: VMware, Inc.
 Author-email: idemproject@vmware.com
 License: Apache Software License 2.0
 Project-URL: Code, https://gitlab.com/vmware/idem/pop-serial
 Project-URL: Issue tracker, https://gitlab.com/vmware/idem/pop-serial/issues
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
 
 ==========
 pop-serial
 ==========
 
@@ -56,15 +56,15 @@
 
 Getting Started
 ===============
 
 Prerequisites
 -------------
 
-* Python 3.7+
+* Python 3.8+
 * git *(if installing from source, or contributing to the project)*
 
 Installation
 ------------
 
 .. note::
```

### Comparing `pop-serial-1.1.1/setup.py` & `pop-serial-2.0.0/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -74,27 +74,27 @@
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
     packages=discover_packages(),
     entry_points={"console_scripts": [""]},
     cmdclass={"clean": Clean},
 )
```

