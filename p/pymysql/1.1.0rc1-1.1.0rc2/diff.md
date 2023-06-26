# Comparing `tmp/PyMySQL-1.1.0rc1.tar.gz` & `tmp/PyMySQL-1.1.0rc2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "PyMySQL-1.1.0rc1.tar", last modified: Thu May 25 06:27:52 2023, max compression
+gzip compressed data, was "PyMySQL-1.1.0rc2.tar", last modified: Thu Jun 15 07:59:10 2023, max compression
```

## Comparing `PyMySQL-1.1.0rc1.tar` & `PyMySQL-1.1.0rc2.tar`

### file list

```diff
@@ -1,36 +1,36 @@
-drwxr-xr-x   0 inada-n    (502) staff       (20)        0 2023-05-25 06:27:52.993198 PyMySQL-1.1.0rc1/
--rw-r--r--   0 inada-n    (502) staff       (20)    12745 2023-05-25 06:27:10.000000 PyMySQL-1.1.0rc1/CHANGELOG.md
--rw-r--r--   0 inada-n    (502) staff       (20)     1070 2013-11-27 14:43:24.000000 PyMySQL-1.1.0rc1/LICENSE
--rw-r--r--   0 inada-n    (502) staff       (20)       39 2023-05-23 15:12:24.000000 PyMySQL-1.1.0rc1/MANIFEST.in
--rw-r--r--   0 inada-n    (502) staff       (20)     4260 2023-05-25 06:27:52.993087 PyMySQL-1.1.0rc1/PKG-INFO
-drwxr-xr-x   0 inada-n    (502) staff       (20)        0 2023-05-25 06:27:52.990740 PyMySQL-1.1.0rc1/PyMySQL.egg-info/
--rw-r--r--   0 inada-n    (502) staff       (20)     4260 2023-05-25 06:27:52.000000 PyMySQL-1.1.0rc1/PyMySQL.egg-info/PKG-INFO
--rw-r--r--   0 inada-n    (502) staff       (20)      652 2023-05-25 06:27:52.000000 PyMySQL-1.1.0rc1/PyMySQL.egg-info/SOURCES.txt
--rw-r--r--   0 inada-n    (502) staff       (20)        1 2023-05-25 06:27:52.000000 PyMySQL-1.1.0rc1/PyMySQL.egg-info/dependency_links.txt
--rw-r--r--   0 inada-n    (502) staff       (20)       45 2023-05-25 06:27:52.000000 PyMySQL-1.1.0rc1/PyMySQL.egg-info/requires.txt
--rw-r--r--   0 inada-n    (502) staff       (20)        8 2023-05-25 06:27:52.000000 PyMySQL-1.1.0rc1/PyMySQL.egg-info/top_level.txt
--rw-r--r--   0 inada-n    (502) staff       (20)     3168 2023-05-24 05:52:56.000000 PyMySQL-1.1.0rc1/README.md
-drwxr-xr-x   0 inada-n    (502) staff       (20)        0 2023-05-25 06:27:52.991877 PyMySQL-1.1.0rc1/pymysql/
--rw-r--r--   0 inada-n    (502) staff       (20)     4264 2023-05-25 06:27:10.000000 PyMySQL-1.1.0rc1/pymysql/__init__.py
--rw-r--r--   0 inada-n    (502) staff       (20)     7416 2023-05-24 05:21:28.000000 PyMySQL-1.1.0rc1/pymysql/_auth.py
--rw-r--r--   0 inada-n    (502) staff       (20)    10301 2023-05-24 16:54:14.000000 PyMySQL-1.1.0rc1/pymysql/charset.py
--rw-r--r--   0 inada-n    (502) staff       (20)    53589 2023-05-25 06:27:10.000000 PyMySQL-1.1.0rc1/pymysql/connections.py
-drwxr-xr-x   0 inada-n    (502) staff       (20)        0 2023-05-25 06:27:52.992849 PyMySQL-1.1.0rc1/pymysql/constants/
--rw-r--r--   0 inada-n    (502) staff       (20)      878 2021-01-03 03:07:14.000000 PyMySQL-1.1.0rc1/pymysql/constants/CLIENT.py
--rw-r--r--   0 inada-n    (502) staff       (20)      679 2021-01-03 03:07:14.000000 PyMySQL-1.1.0rc1/pymysql/constants/COMMAND.py
--rw-r--r--   0 inada-n    (502) staff       (20)     2320 2023-05-23 15:12:24.000000 PyMySQL-1.1.0rc1/pymysql/constants/CR.py
--rw-r--r--   0 inada-n    (502) staff       (20)    12357 2023-05-23 15:12:24.000000 PyMySQL-1.1.0rc1/pymysql/constants/ER.py
--rw-r--r--   0 inada-n    (502) staff       (20)      370 2021-01-03 03:07:14.000000 PyMySQL-1.1.0rc1/pymysql/constants/FIELD_TYPE.py
--rw-r--r--   0 inada-n    (502) staff       (20)      214 2018-12-18 12:04:22.000000 PyMySQL-1.1.0rc1/pymysql/constants/FLAG.py
--rw-r--r--   0 inada-n    (502) staff       (20)      333 2021-01-03 03:07:14.000000 PyMySQL-1.1.0rc1/pymysql/constants/SERVER_STATUS.py
--rw-r--r--   0 inada-n    (502) staff       (20)        0 2014-08-29 11:32:54.000000 PyMySQL-1.1.0rc1/pymysql/constants/__init__.py
--rw-r--r--   0 inada-n    (502) staff       (20)     9591 2023-05-24 07:46:55.000000 PyMySQL-1.1.0rc1/pymysql/converters.py
--rw-r--r--   0 inada-n    (502) staff       (20)    16535 2023-05-24 16:03:44.000000 PyMySQL-1.1.0rc1/pymysql/cursors.py
--rw-r--r--   0 inada-n    (502) staff       (20)     3773 2021-01-03 03:07:14.000000 PyMySQL-1.1.0rc1/pymysql/err.py
--rw-r--r--   0 inada-n    (502) staff       (20)      651 2023-05-24 13:30:02.000000 PyMySQL-1.1.0rc1/pymysql/optionfile.py
--rw-r--r--   0 inada-n    (502) staff       (20)    11863 2023-05-24 16:03:44.000000 PyMySQL-1.1.0rc1/pymysql/protocol.py
--rw-r--r--   0 inada-n    (502) staff       (20)      360 2021-01-02 07:55:27.000000 PyMySQL-1.1.0rc1/pymysql/times.py
--rw-r--r--   0 inada-n    (502) staff       (20)     1557 2023-05-25 02:33:20.000000 PyMySQL-1.1.0rc1/pyproject.toml
--rw-r--r--   0 inada-n    (502) staff       (20)       38 2023-05-25 06:27:52.993228 PyMySQL-1.1.0rc1/setup.cfg
-drwxr-xr-x   0 inada-n    (502) staff       (20)        0 2023-05-25 06:27:52.992940 PyMySQL-1.1.0rc1/tests/
--rw-r--r--   0 inada-n    (502) staff       (20)     2140 2021-01-03 03:07:14.000000 PyMySQL-1.1.0rc1/tests/test_auth.py
+drwxr-xr-x   0 inada-n    (502) staff       (20)        0 2023-06-15 07:59:10.718175 PyMySQL-1.1.0rc2/
+-rw-r--r--   0 inada-n    (502) staff       (20)    12790 2023-06-15 07:58:34.000000 PyMySQL-1.1.0rc2/CHANGELOG.md
+-rw-r--r--   0 inada-n    (502) staff       (20)     1070 2013-11-27 14:43:24.000000 PyMySQL-1.1.0rc2/LICENSE
+-rw-r--r--   0 inada-n    (502) staff       (20)       39 2023-05-23 15:12:24.000000 PyMySQL-1.1.0rc2/MANIFEST.in
+-rw-r--r--   0 inada-n    (502) staff       (20)     4260 2023-06-15 07:59:10.718065 PyMySQL-1.1.0rc2/PKG-INFO
+drwxr-xr-x   0 inada-n    (502) staff       (20)        0 2023-06-15 07:59:10.713454 PyMySQL-1.1.0rc2/PyMySQL.egg-info/
+-rw-r--r--   0 inada-n    (502) staff       (20)     4260 2023-06-15 07:59:10.000000 PyMySQL-1.1.0rc2/PyMySQL.egg-info/PKG-INFO
+-rw-r--r--   0 inada-n    (502) staff       (20)      652 2023-06-15 07:59:10.000000 PyMySQL-1.1.0rc2/PyMySQL.egg-info/SOURCES.txt
+-rw-r--r--   0 inada-n    (502) staff       (20)        1 2023-06-15 07:59:10.000000 PyMySQL-1.1.0rc2/PyMySQL.egg-info/dependency_links.txt
+-rw-r--r--   0 inada-n    (502) staff       (20)       45 2023-06-15 07:59:10.000000 PyMySQL-1.1.0rc2/PyMySQL.egg-info/requires.txt
+-rw-r--r--   0 inada-n    (502) staff       (20)        8 2023-06-15 07:59:10.000000 PyMySQL-1.1.0rc2/PyMySQL.egg-info/top_level.txt
+-rw-r--r--   0 inada-n    (502) staff       (20)     3168 2023-06-14 18:03:30.000000 PyMySQL-1.1.0rc2/README.md
+drwxr-xr-x   0 inada-n    (502) staff       (20)        0 2023-06-15 07:59:10.715919 PyMySQL-1.1.0rc2/pymysql/
+-rw-r--r--   0 inada-n    (502) staff       (20)     4264 2023-06-15 07:58:34.000000 PyMySQL-1.1.0rc2/pymysql/__init__.py
+-rw-r--r--   0 inada-n    (502) staff       (20)     7416 2023-05-24 05:21:28.000000 PyMySQL-1.1.0rc2/pymysql/_auth.py
+-rw-r--r--   0 inada-n    (502) staff       (20)    10238 2023-06-15 04:22:40.000000 PyMySQL-1.1.0rc2/pymysql/charset.py
+-rw-r--r--   0 inada-n    (502) staff       (20)    53589 2023-05-25 06:27:10.000000 PyMySQL-1.1.0rc2/pymysql/connections.py
+drwxr-xr-x   0 inada-n    (502) staff       (20)        0 2023-06-15 07:59:10.717796 PyMySQL-1.1.0rc2/pymysql/constants/
+-rw-r--r--   0 inada-n    (502) staff       (20)      878 2021-01-03 03:07:14.000000 PyMySQL-1.1.0rc2/pymysql/constants/CLIENT.py
+-rw-r--r--   0 inada-n    (502) staff       (20)      679 2021-01-03 03:07:14.000000 PyMySQL-1.1.0rc2/pymysql/constants/COMMAND.py
+-rw-r--r--   0 inada-n    (502) staff       (20)     2320 2023-05-23 15:12:24.000000 PyMySQL-1.1.0rc2/pymysql/constants/CR.py
+-rw-r--r--   0 inada-n    (502) staff       (20)    12357 2023-05-23 15:12:24.000000 PyMySQL-1.1.0rc2/pymysql/constants/ER.py
+-rw-r--r--   0 inada-n    (502) staff       (20)      370 2021-01-03 03:07:14.000000 PyMySQL-1.1.0rc2/pymysql/constants/FIELD_TYPE.py
+-rw-r--r--   0 inada-n    (502) staff       (20)      214 2018-12-18 12:04:22.000000 PyMySQL-1.1.0rc2/pymysql/constants/FLAG.py
+-rw-r--r--   0 inada-n    (502) staff       (20)      333 2021-01-03 03:07:14.000000 PyMySQL-1.1.0rc2/pymysql/constants/SERVER_STATUS.py
+-rw-r--r--   0 inada-n    (502) staff       (20)        0 2014-08-29 11:32:54.000000 PyMySQL-1.1.0rc2/pymysql/constants/__init__.py
+-rw-r--r--   0 inada-n    (502) staff       (20)     9591 2023-05-24 07:46:55.000000 PyMySQL-1.1.0rc2/pymysql/converters.py
+-rw-r--r--   0 inada-n    (502) staff       (20)    16535 2023-05-24 16:03:44.000000 PyMySQL-1.1.0rc2/pymysql/cursors.py
+-rw-r--r--   0 inada-n    (502) staff       (20)     3773 2021-01-03 03:07:14.000000 PyMySQL-1.1.0rc2/pymysql/err.py
+-rw-r--r--   0 inada-n    (502) staff       (20)      651 2023-05-24 13:30:02.000000 PyMySQL-1.1.0rc2/pymysql/optionfile.py
+-rw-r--r--   0 inada-n    (502) staff       (20)    11863 2023-05-24 16:03:44.000000 PyMySQL-1.1.0rc2/pymysql/protocol.py
+-rw-r--r--   0 inada-n    (502) staff       (20)      360 2021-01-02 07:55:27.000000 PyMySQL-1.1.0rc2/pymysql/times.py
+-rw-r--r--   0 inada-n    (502) staff       (20)     1557 2023-06-14 18:37:22.000000 PyMySQL-1.1.0rc2/pyproject.toml
+-rw-r--r--   0 inada-n    (502) staff       (20)       38 2023-06-15 07:59:10.718204 PyMySQL-1.1.0rc2/setup.cfg
+drwxr-xr-x   0 inada-n    (502) staff       (20)        0 2023-06-15 07:59:10.717889 PyMySQL-1.1.0rc2/tests/
+-rw-r--r--   0 inada-n    (502) staff       (20)     2140 2021-01-03 03:07:14.000000 PyMySQL-1.1.0rc2/tests/test_auth.py
```

### Comparing `PyMySQL-1.1.0rc1/CHANGELOG.md` & `PyMySQL-1.1.0rc2/CHANGELOG.md`

 * *Files 0% similar despite different names*

```diff
@@ -10,14 +10,15 @@
 * Support '_' in key name in my.cnf (#1114)
 * `Cursor.fetchall()` returns empty list instead of tuple (#1115). Note that `Cursor.fetchmany()` still return empty tuple after reading all rows for compatibility with Django.
 * Deprecate Error classes in Cursor class (#1117)
 * Add `Connection.set_character_set(charset, collation=None)` (#1119)
 * Deprecate `Connection.set_charset(charset)` (#1119)
 * New connection always send "SET NAMES charset [COLLATE collation]" query. (#1119)
   Since collation table is vary on MySQL server versions, collation in handshake is fragile.
+* Support `charset="utf8mb3"` option (#1127)
 
 
 ## v1.0.3
 
 Release date: 2023-03-28
 
 * Dropped support of end of life MySQL version 5.6
```

### Comparing `PyMySQL-1.1.0rc1/LICENSE` & `PyMySQL-1.1.0rc2/LICENSE`

 * *Files identical despite different names*

### Comparing `PyMySQL-1.1.0rc1/PKG-INFO` & `PyMySQL-1.1.0rc2/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: PyMySQL
-Version: 1.1.0rc1
+Version: 1.1.0rc2
 Summary: Pure Python MySQL Driver
 Author-email: Inada Naoki <songofacandy@gmail.com>, Yutaka Matsubara <yutaka.matsubara@gmail.com>
 License: MIT License
 Project-URL: Project, https://github.com/PyMySQL/PyMySQL
 Project-URL: Documentation, https://pymysql.readthedocs.io/
 Keywords: MySQL
 Classifier: Development Status :: 5 - Production/Stable
@@ -36,15 +36,15 @@
 ## Requirements
 
 - Python -- one of the following:
   - [CPython](https://www.python.org/) : 3.7 and newer
   - [PyPy](https://pypy.org/) : Latest 3.x version
 - MySQL Server -- one of the following:
   - [MySQL](https://www.mysql.com/) \>= 5.7
-  - [MariaDB](https://mariadb.org/) \>= 10.3
+  - [MariaDB](https://mariadb.org/) \>= 10.4
 
 ## Installation
 
 Package is uploaded on [PyPI](https://pypi.org/project/PyMySQL).
 
 You can install it with pip:
```

### Comparing `PyMySQL-1.1.0rc1/PyMySQL.egg-info/PKG-INFO` & `PyMySQL-1.1.0rc2/PyMySQL.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: PyMySQL
-Version: 1.1.0rc1
+Version: 1.1.0rc2
 Summary: Pure Python MySQL Driver
 Author-email: Inada Naoki <songofacandy@gmail.com>, Yutaka Matsubara <yutaka.matsubara@gmail.com>
 License: MIT License
 Project-URL: Project, https://github.com/PyMySQL/PyMySQL
 Project-URL: Documentation, https://pymysql.readthedocs.io/
 Keywords: MySQL
 Classifier: Development Status :: 5 - Production/Stable
@@ -36,15 +36,15 @@
 ## Requirements
 
 - Python -- one of the following:
   - [CPython](https://www.python.org/) : 3.7 and newer
   - [PyPy](https://pypy.org/) : Latest 3.x version
 - MySQL Server -- one of the following:
   - [MySQL](https://www.mysql.com/) \>= 5.7
-  - [MariaDB](https://mariadb.org/) \>= 10.3
+  - [MariaDB](https://mariadb.org/) \>= 10.4
 
 ## Installation
 
 Package is uploaded on [PyPI](https://pypi.org/project/PyMySQL).
 
 You can install it with pip:
```

### Comparing `PyMySQL-1.1.0rc1/PyMySQL.egg-info/SOURCES.txt` & `PyMySQL-1.1.0rc2/PyMySQL.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `PyMySQL-1.1.0rc1/README.md` & `PyMySQL-1.1.0rc2/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -9,15 +9,15 @@
 ## Requirements
 
 - Python -- one of the following:
   - [CPython](https://www.python.org/) : 3.7 and newer
   - [PyPy](https://pypy.org/) : Latest 3.x version
 - MySQL Server -- one of the following:
   - [MySQL](https://www.mysql.com/) \>= 5.7
-  - [MariaDB](https://mariadb.org/) \>= 10.3
+  - [MariaDB](https://mariadb.org/) \>= 10.4
 
 ## Installation
 
 Package is uploaded on [PyPI](https://pypi.org/project/PyMySQL).
 
 You can install it with pip:
```

### Comparing `PyMySQL-1.1.0rc1/pymysql/__init__.py` & `PyMySQL-1.1.0rc2/pymysql/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -44,16 +44,16 @@
     DateFromTicks,
     TimeFromTicks,
     TimestampFromTicks,
 )
 
 # PyMySQL version.
 # Used by setuptools and connection_attrs
-VERSION = (1, 1, 0, "rc", 1)
-VERSION_STRING = "1.1.0rc1"
+VERSION = (1, 1, 0, "rc", 2)
+VERSION_STRING = "1.1.0rc2"
 
 ### for mysqlclient compatibility
 ### Django checks mysqlclient version.
 version_info = (1, 4, 3, "final", 0)
 __version__ = "1.4.3"
```

### Comparing `PyMySQL-1.1.0rc1/pymysql/_auth.py` & `PyMySQL-1.1.0rc2/pymysql/_auth.py`

 * *Files identical despite different names*

### Comparing `PyMySQL-1.1.0rc1/pymysql/connections.py` & `PyMySQL-1.1.0rc2/pymysql/connections.py`

 * *Files identical despite different names*

### Comparing `PyMySQL-1.1.0rc1/pymysql/constants/CLIENT.py` & `PyMySQL-1.1.0rc2/pymysql/constants/CLIENT.py`

 * *Files identical despite different names*

### Comparing `PyMySQL-1.1.0rc1/pymysql/constants/COMMAND.py` & `PyMySQL-1.1.0rc2/pymysql/constants/COMMAND.py`

 * *Files identical despite different names*

### Comparing `PyMySQL-1.1.0rc1/pymysql/constants/CR.py` & `PyMySQL-1.1.0rc2/pymysql/constants/CR.py`

 * *Files identical despite different names*

### Comparing `PyMySQL-1.1.0rc1/pymysql/constants/ER.py` & `PyMySQL-1.1.0rc2/pymysql/constants/ER.py`

 * *Files identical despite different names*

### Comparing `PyMySQL-1.1.0rc1/pymysql/converters.py` & `PyMySQL-1.1.0rc2/pymysql/converters.py`

 * *Files identical despite different names*

### Comparing `PyMySQL-1.1.0rc1/pymysql/cursors.py` & `PyMySQL-1.1.0rc2/pymysql/cursors.py`

 * *Files identical despite different names*

### Comparing `PyMySQL-1.1.0rc1/pymysql/err.py` & `PyMySQL-1.1.0rc2/pymysql/err.py`

 * *Files identical despite different names*

### Comparing `PyMySQL-1.1.0rc1/pymysql/optionfile.py` & `PyMySQL-1.1.0rc2/pymysql/optionfile.py`

 * *Files identical despite different names*

### Comparing `PyMySQL-1.1.0rc1/pymysql/protocol.py` & `PyMySQL-1.1.0rc2/pymysql/protocol.py`

 * *Files identical despite different names*

### Comparing `PyMySQL-1.1.0rc1/pyproject.toml` & `PyMySQL-1.1.0rc2/pyproject.toml`

 * *Files identical despite different names*

### Comparing `PyMySQL-1.1.0rc1/tests/test_auth.py` & `PyMySQL-1.1.0rc2/tests/test_auth.py`

 * *Files identical despite different names*

