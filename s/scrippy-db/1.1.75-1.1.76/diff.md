# Comparing `tmp/scrippy-db-1.1.75.tar.gz` & `tmp/scrippy-db-1.1.76.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "scrippy-db-1.1.75.tar", last modified: Sun Apr  2 01:41:36 2023, max compression
+gzip compressed data, was "scrippy-db-1.1.76.tar", last modified: Mon Jun 26 04:14:01 2023, max compression
```

## Comparing `scrippy-db-1.1.75.tar` & `scrippy-db-1.1.76.tar`

### file list

```diff
@@ -1,19 +1,20 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-02 01:41:36.704648 scrippy-db-1.1.75/
--rwxr-xr-x   0 root         (0) root         (0)     1179 2023-04-02 01:40:48.000000 scrippy-db-1.1.75/LICENSE
--rw-r--r--   0 root         (0) root         (0)     4669 2023-04-02 01:41:36.704648 scrippy-db-1.1.75/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     3865 2023-04-02 01:40:48.000000 scrippy-db-1.1.75/README.md
--rw-r--r--   0 root         (0) root         (0)     1349 2023-04-02 01:41:36.705648 scrippy-db-1.1.75/setup.cfg
--rwxr-xr-x   0 root         (0) root         (0)       38 2023-04-02 01:40:48.000000 scrippy-db-1.1.75/setup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-02 01:41:36.699648 scrippy-db-1.1.75/src/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-02 01:41:36.701648 scrippy-db-1.1.75/src/scrippy_db/
--rw-r--r--   0 root         (0) root         (0)      241 2023-04-02 01:40:48.000000 scrippy-db-1.1.75/src/scrippy_db/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-02 01:41:36.703648 scrippy-db-1.1.75/src/scrippy_db/db/
--rwxr-xr-x   0 root         (0) root         (0)     7143 2023-04-02 01:40:48.000000 scrippy-db-1.1.75/src/scrippy_db/db/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-02 01:41:36.703648 scrippy-db-1.1.75/src/scrippy_db.egg-info/
--rw-r--r--   0 root         (0) root         (0)     4669 2023-04-02 01:41:36.000000 scrippy-db-1.1.75/src/scrippy_db.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      299 2023-04-02 01:41:36.000000 scrippy-db-1.1.75/src/scrippy_db.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-04-02 01:41:36.000000 scrippy-db-1.1.75/src/scrippy_db.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      317 2023-04-02 01:41:36.000000 scrippy-db-1.1.75/src/scrippy_db.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       11 2023-04-02 01:41:36.000000 scrippy-db-1.1.75/src/scrippy_db.egg-info/top_level.txt
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-02 01:41:36.704648 scrippy-db-1.1.75/tests/
--rw-r--r--   0 root         (0) root         (0)      731 2023-04-02 01:40:48.000000 scrippy-db-1.1.75/tests/test_db.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-26 04:14:01.520036 scrippy-db-1.1.76/
+-rwxr-xr-x   0 root         (0) root         (0)     1179 2023-06-26 04:12:58.000000 scrippy-db-1.1.76/LICENSE
+-rw-r--r--   0 root         (0) root         (0)     4669 2023-06-26 04:14:01.520036 scrippy-db-1.1.76/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     3866 2023-06-26 04:12:58.000000 scrippy-db-1.1.76/README.md
+-rw-r--r--   0 root         (0) root         (0)      210 2023-06-26 04:12:58.000000 scrippy-db-1.1.76/pyproject.toml
+-rw-r--r--   0 root         (0) root         (0)     1356 2023-06-26 04:14:01.522036 scrippy-db-1.1.76/setup.cfg
+-rwxr-xr-x   0 root         (0) root         (0)       38 2023-06-26 04:12:58.000000 scrippy-db-1.1.76/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-26 04:14:01.514036 scrippy-db-1.1.76/src/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-26 04:14:01.517036 scrippy-db-1.1.76/src/scrippy_db/
+-rw-r--r--   0 root         (0) root         (0)      241 2023-06-26 04:12:58.000000 scrippy-db-1.1.76/src/scrippy_db/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-26 04:14:01.520036 scrippy-db-1.1.76/src/scrippy_db/db/
+-rwxr-xr-x   0 root         (0) root         (0)     7143 2023-06-26 04:12:58.000000 scrippy-db-1.1.76/src/scrippy_db/db/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-26 04:14:01.519036 scrippy-db-1.1.76/src/scrippy_db.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     4669 2023-06-26 04:14:01.000000 scrippy-db-1.1.76/src/scrippy_db.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      314 2023-06-26 04:14:01.000000 scrippy-db-1.1.76/src/scrippy_db.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-06-26 04:14:01.000000 scrippy-db-1.1.76/src/scrippy_db.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      323 2023-06-26 04:14:01.000000 scrippy-db-1.1.76/src/scrippy_db.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       11 2023-06-26 04:14:01.000000 scrippy-db-1.1.76/src/scrippy_db.egg-info/top_level.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-26 04:14:01.520036 scrippy-db-1.1.76/tests/
+-rw-r--r--   0 root         (0) root         (0)      731 2023-06-26 04:12:58.000000 scrippy-db-1.1.76/tests/test_db.py
```

### Comparing `scrippy-db-1.1.75/LICENSE` & `scrippy-db-1.1.76/LICENSE`

 * *Files identical despite different names*

### Comparing `scrippy-db-1.1.75/PKG-INFO` & `scrippy-db-1.1.76/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: scrippy-db
-Version: 1.1.75
+Version: 1.1.76
 Summary: "Client de bases de données pour le cadriciel Scrippy"
 Home-page: https://codeberg.org/scrippy/scrippy-db
 Author: Michael Costa, Florent Chevalier
 Author-email: michael.costa@mcos.nc, florent.chevalier.nc@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
@@ -15,15 +15,15 @@
 Classifier: Development Status :: 5 - Production/Stable
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 Provides-Extra: dev
 License-File: LICENSE
 
 
-![Build Status](https://drone.mcos.nc/api/badges/scrippy/scrippy-db/status.svg) ![License](https://img.shields.io/static/v1?label=license&color=orange&message=MIT) ![Language](https://img.shields.io/static/v1?label=language&color=informational&message=Python)
+![Build Status](https://drone-ext.mcos.nc/api/badges/scrippy/scrippy-db/status.svg) ![License](https://img.shields.io/static/v1?label=license&color=orange&message=MIT) ![Language](https://img.shields.io/static/v1?label=language&color=informational&message=Python)
 
 ![Scrippy, my scrangourou friend](./scrippy-db.png "Scrippy, my scrangourou friend")
 
 # `scrippy_db`
 
 Generic database client for the [`Scrippy`](https://codeberg.org/scrippy) framework.
 
@@ -41,15 +41,15 @@
 
 ## Installation
 
 ### Manual
 
 ```bash
 git clone https://codeberg.org/scrippy/scrippy-db.git
-cd scrippy-db.git
+cd scrippy-db
 python -m pip install -r requirements.txt
 make install
 ```
 
 ### With `pip`
 
 ```bash
```

### Comparing `scrippy-db-1.1.75/README.md` & `scrippy-db-1.1.76/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 
-![Build Status](https://drone.mcos.nc/api/badges/scrippy/scrippy-db/status.svg) ![License](https://img.shields.io/static/v1?label=license&color=orange&message=MIT) ![Language](https://img.shields.io/static/v1?label=language&color=informational&message=Python)
+![Build Status](https://drone-ext.mcos.nc/api/badges/scrippy/scrippy-db/status.svg) ![License](https://img.shields.io/static/v1?label=license&color=orange&message=MIT) ![Language](https://img.shields.io/static/v1?label=language&color=informational&message=Python)
 
 ![Scrippy, my scrangourou friend](./scrippy-db.png "Scrippy, my scrangourou friend")
 
 # `scrippy_db`
 
 Generic database client for the [`Scrippy`](https://codeberg.org/scrippy) framework.
 
@@ -21,15 +21,15 @@
 
 ## Installation
 
 ### Manual
 
 ```bash
 git clone https://codeberg.org/scrippy/scrippy-db.git
-cd scrippy-db.git
+cd scrippy-db
 python -m pip install -r requirements.txt
 make install
 ```
 
 ### With `pip`
 
 ```bash
@@ -102,8 +102,8 @@
   else:
     # The application has never been registered, we register the application and its status.
     req = """insert into apps
             (app_name, app_version, app_status, date)
             values (%(app_name)s, %(app_version)s, %(app_status)s, %(date)s);"""
     params = (app_name, app_version, app_status, date)
     result = database.execute(req, params)
-```
+```
```

### Comparing `scrippy-db-1.1.75/setup.cfg` & `scrippy-db-1.1.76/setup.cfg`

 * *Files 2% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 [metadata]
-version = 1.1.75
+version = 1.1.76
 classifiers = 
 	Programming Language :: Python :: 3
 	License :: OSI Approved :: MIT License
 	Operating System :: OS Independent
 	Topic :: Software Development :: Libraries :: Application Frameworks
 	Intended Audience :: Developers
 	Intended Audience :: System Administrators
@@ -21,22 +21,23 @@
 package_dir = 
 	= src
 packages = find:
 python_requires = >=3.8
 install_requires = 
 	psycopg2-binary>=2.8.3
 	cx-Oracle>=7.2.2
-	mysqlclient>=2.1.1
+	mysqlclient==2.1.1
 
 [options.packages.find]
 where = src
 
 [options.extras_require]
 dev = 
 	twine
+	build
 	wheel>=0.37.0
 	flake8>=4.0.1
 	flake8-breakpoint>=1.1.0
 	flake8-builtins>=1.5.3
 	flake8-print>=4.0.0
 	flake8-return>=1.1.3
 	pep8-naming>=0.8.2
```

### Comparing `scrippy-db-1.1.75/src/scrippy_db/db/__init__.py` & `scrippy-db-1.1.76/src/scrippy_db/db/__init__.py`

 * *Files identical despite different names*

### Comparing `scrippy-db-1.1.75/src/scrippy_db.egg-info/PKG-INFO` & `scrippy-db-1.1.76/src/scrippy_db.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: scrippy-db
-Version: 1.1.75
+Version: 1.1.76
 Summary: "Client de bases de données pour le cadriciel Scrippy"
 Home-page: https://codeberg.org/scrippy/scrippy-db
 Author: Michael Costa, Florent Chevalier
 Author-email: michael.costa@mcos.nc, florent.chevalier.nc@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
@@ -15,15 +15,15 @@
 Classifier: Development Status :: 5 - Production/Stable
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 Provides-Extra: dev
 License-File: LICENSE
 
 
-![Build Status](https://drone.mcos.nc/api/badges/scrippy/scrippy-db/status.svg) ![License](https://img.shields.io/static/v1?label=license&color=orange&message=MIT) ![Language](https://img.shields.io/static/v1?label=language&color=informational&message=Python)
+![Build Status](https://drone-ext.mcos.nc/api/badges/scrippy/scrippy-db/status.svg) ![License](https://img.shields.io/static/v1?label=license&color=orange&message=MIT) ![Language](https://img.shields.io/static/v1?label=language&color=informational&message=Python)
 
 ![Scrippy, my scrangourou friend](./scrippy-db.png "Scrippy, my scrangourou friend")
 
 # `scrippy_db`
 
 Generic database client for the [`Scrippy`](https://codeberg.org/scrippy) framework.
 
@@ -41,15 +41,15 @@
 
 ## Installation
 
 ### Manual
 
 ```bash
 git clone https://codeberg.org/scrippy/scrippy-db.git
-cd scrippy-db.git
+cd scrippy-db
 python -m pip install -r requirements.txt
 make install
 ```
 
 ### With `pip`
 
 ```bash
```

### Comparing `scrippy-db-1.1.75/tests/test_db.py` & `scrippy-db-1.1.76/tests/test_db.py`

 * *Files identical despite different names*

