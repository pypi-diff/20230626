# Comparing `tmp/farm_ng_package-0.1.1.tar.gz` & `tmp/farm_ng_package-0.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/farm_ng_package-0.1.1.tar", last modified: Tue Nov  8 10:50:48 2022, max compression
+gzip compressed data, was "farm_ng_package-0.1.3.tar", last modified: Mon Jun 26 09:37:12 2023, max compression
```

## Comparing `farm_ng_package-0.1.1.tar` & `farm_ng_package-0.1.3.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-08 10:50:48.000000 farm_ng_package-0.1.1/
--rw-r--r--   0 runner    (1001) docker     (121)    11357 2022-11-08 10:50:46.000000 farm_ng_package-0.1.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (121)      688 2022-11-08 10:50:48.000000 farm_ng_package-0.1.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)       61 2022-11-08 10:50:46.000000 farm_ng_package-0.1.1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-08 10:50:48.000000 farm_ng_package-0.1.1/farm_ng/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-08 10:50:48.000000 farm_ng_package-0.1.1/farm_ng/package/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-11-08 10:50:46.000000 farm_ng_package-0.1.1/farm_ng/package/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     2101 2022-11-08 10:50:46.000000 farm_ng_package-0.1.1/farm_ng/package/commands.py
--rw-r--r--   0 runner    (1001) docker     (121)     2342 2022-11-08 10:50:46.000000 farm_ng_package-0.1.1/farm_ng/package/package.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-08 10:50:48.000000 farm_ng_package-0.1.1/farm_ng_package.egg-info/
--rw-r--r--   0 runner    (1001) docker     (121)      688 2022-11-08 10:50:48.000000 farm_ng_package-0.1.1/farm_ng_package.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)      313 2022-11-08 10:50:48.000000 farm_ng_package-0.1.1/farm_ng_package.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2022-11-08 10:50:48.000000 farm_ng_package-0.1.1/farm_ng_package.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (121)       13 2022-11-08 10:50:48.000000 farm_ng_package-0.1.1/farm_ng_package.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (121)        8 2022-11-08 10:50:48.000000 farm_ng_package-0.1.1/farm_ng_package.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (121)      800 2022-11-08 10:50:48.000000 farm_ng_package-0.1.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (121)       69 2022-11-08 10:50:46.000000 farm_ng_package-0.1.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 09:37:12.611762 farm_ng_package-0.1.3/
+-rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-06-26 09:37:09.000000 farm_ng_package-0.1.3/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      835 2023-06-26 09:37:12.611762 farm_ng_package-0.1.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      168 2023-06-26 09:37:09.000000 farm_ng_package-0.1.3/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 09:37:12.611762 farm_ng_package-0.1.3/farm_ng/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 09:37:12.611762 farm_ng_package-0.1.3/farm_ng/package/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-26 09:37:09.000000 farm_ng_package-0.1.3/farm_ng/package/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2101 2023-06-26 09:37:09.000000 farm_ng_package-0.1.3/farm_ng/package/commands.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2395 2023-06-26 09:37:09.000000 farm_ng_package-0.1.3/farm_ng/package/package.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 09:37:12.611762 farm_ng_package-0.1.3/farm_ng_package.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      835 2023-06-26 09:37:12.000000 farm_ng_package-0.1.3/farm_ng_package.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      313 2023-06-26 09:37:12.000000 farm_ng_package-0.1.3/farm_ng_package.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-26 09:37:12.000000 farm_ng_package-0.1.3/farm_ng_package.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       13 2023-06-26 09:37:12.000000 farm_ng_package-0.1.3/farm_ng_package.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        8 2023-06-26 09:37:12.000000 farm_ng_package-0.1.3/farm_ng_package.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      846 2023-06-26 09:37:12.611762 farm_ng_package-0.1.3/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)       69 2023-06-26 09:37:09.000000 farm_ng_package-0.1.3/setup.py
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive (GNU)
+POSIX tar archive
```

### Comparing `farm_ng_package-0.1.1/LICENSE` & `farm_ng_package-0.1.3/LICENSE`

 * *Files identical despite different names*

### Comparing `farm_ng_package-0.1.1/PKG-INFO` & `farm_ng_package-0.1.3/PKG-INFO`

 * *Files 15% similar despite different names*

```diff
@@ -1,21 +1,24 @@
 Metadata-Version: 2.1
 Name: farm_ng_package
-Version: 0.1.1
+Version: 0.1.3
 Home-page: https://github.com/farm-ng/farm-ng-pysetup
 Download-URL: https://github.com/farm-ng/farm-ng-pysetup
 Author: Farm-ng Inc.
 Author-email: info@farm-ng.com
 Keywords: robotics,open-source
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
 Classifier: Topic :: Software Development
 Classifier: Framework :: Robot Framework
 Requires-Python: >=3.6
+Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # farm-ng-package
 
+[![PyPI version](https://badge.fury.io/py/farm-ng-package.svg)](https://pypi.org/project/farm-ng-package)
+
 Farm-ng setup scripts for python projects
```

### Comparing `farm_ng_package-0.1.1/farm_ng/package/commands.py` & `farm_ng_package-0.1.3/farm_ng/package/commands.py`

 * *Files identical despite different names*

### Comparing `farm_ng_package-0.1.1/farm_ng/package/package.py` & `farm_ng_package-0.1.3/farm_ng/package/package.py`

 * *Files 4% similar despite different names*

```diff
@@ -37,14 +37,15 @@
                 "grpc_tools.protoc",
                 "--proto_path={}".format(inclusion_root),
                 "--proto_path={}".format(well_known_protos_include),
             ]
             + includes
             + [
                 "--python_out={}".format(package_root),
+                "--pyi_out={}".format(package_root),
                 "--grpc_python_out={}".format(package_root),
             ]
             + [proto_file]
         )
         if protoc.main(command) != 0:
             raise Exception("error: {} failed".format(command))
```

### Comparing `farm_ng_package-0.1.1/farm_ng_package.egg-info/PKG-INFO` & `farm_ng_package-0.1.3/farm_ng_package.egg-info/PKG-INFO`

 * *Files 16% similar despite different names*

```diff
@@ -1,21 +1,24 @@
 Metadata-Version: 2.1
 Name: farm-ng-package
-Version: 0.1.1
+Version: 0.1.3
 Home-page: https://github.com/farm-ng/farm-ng-pysetup
 Download-URL: https://github.com/farm-ng/farm-ng-pysetup
 Author: Farm-ng Inc.
 Author-email: info@farm-ng.com
 Keywords: robotics,open-source
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
 Classifier: Topic :: Software Development
 Classifier: Framework :: Robot Framework
 Requires-Python: >=3.6
+Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # farm-ng-package
 
+[![PyPI version](https://badge.fury.io/py/farm-ng-package.svg)](https://pypi.org/project/farm-ng-package)
+
 Farm-ng setup scripts for python projects
```

