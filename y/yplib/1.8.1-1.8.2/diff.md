# Comparing `tmp/yplib-1.8.1.tar.gz` & `tmp/yplib-1.8.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist\yplib-1.8.1.tar", last modified: Mon Jun 26 01:19:49 2023, max compression
+gzip compressed data, was "dist\yplib-1.8.2.tar", last modified: Mon Jun 26 01:33:37 2023, max compression
```

## Comparing `yplib-1.8.1.tar` & `yplib-1.8.2.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxrwxrwx   0        0        0        0 2023-06-26 01:19:49.812380 yplib-1.8.1/
--rw-rw-rw-   0        0        0     1091 2023-06-08 01:05:18.000000 yplib-1.8.1/LICENSE
--rw-rw-rw-   0        0        0      352 2023-06-26 01:19:49.811880 yplib-1.8.1/PKG-INFO
--rw-rw-rw-   0        0        0       13 2023-06-14 02:50:41.000000 yplib-1.8.1/README.md
--rw-rw-rw-   0        0        0       42 2023-06-26 01:19:49.812380 yplib-1.8.1/setup.cfg
--rw-rw-rw-   0        0        0      513 2023-06-26 01:19:38.000000 yplib-1.8.1/setup.py
-drwxrwxrwx   0        0        0        0 2023-06-26 01:19:49.808881 yplib-1.8.1/yplib/
--rw-rw-rw-   0        0        0      469 2023-06-25 08:09:01.000000 yplib-1.8.1/yplib/__init__.py
--rw-rw-rw-   0        0        0    11744 2023-06-26 01:19:30.000000 yplib-1.8.1/yplib/chart.py
--rw-rw-rw-   0        0        0     8553 2023-06-26 00:52:29.000000 yplib-1.8.1/yplib/chart_html.py
--rw-rw-rw-   0        0        0      531 2023-06-25 08:07:04.000000 yplib-1.8.1/yplib/db.py
--rw-rw-rw-   0        0        0     6984 2023-06-16 00:59:15.000000 yplib-1.8.1/yplib/file.py
--rw-rw-rw-   0        0        0     3471 2023-06-19 01:33:36.000000 yplib-1.8.1/yplib/http_util.py
--rw-rw-rw-   0        0        0    26687 2023-06-25 07:43:37.000000 yplib-1.8.1/yplib/index.py
--rw-rw-rw-   0        0        0      124 2023-06-25 07:57:19.000000 yplib-1.8.1/yplib/temp.py
-drwxrwxrwx   0        0        0        0 2023-06-26 01:19:49.811381 yplib-1.8.1/yplib.egg-info/
--rw-rw-rw-   0        0        0      352 2023-06-26 01:19:49.000000 yplib-1.8.1/yplib.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      269 2023-06-26 01:19:49.000000 yplib-1.8.1/yplib.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-26 01:19:49.000000 yplib-1.8.1/yplib.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        6 2023-06-26 01:19:49.000000 yplib-1.8.1/yplib.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-06-26 01:33:37.337210 yplib-1.8.2/
+-rw-rw-rw-   0        0        0     1091 2023-06-08 01:05:18.000000 yplib-1.8.2/LICENSE
+-rw-rw-rw-   0        0        0      352 2023-06-26 01:33:37.336762 yplib-1.8.2/PKG-INFO
+-rw-rw-rw-   0        0        0       13 2023-06-14 02:50:41.000000 yplib-1.8.2/README.md
+-rw-rw-rw-   0        0        0       42 2023-06-26 01:33:37.337546 yplib-1.8.2/setup.cfg
+-rw-rw-rw-   0        0        0      513 2023-06-26 01:33:20.000000 yplib-1.8.2/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-26 01:33:37.333373 yplib-1.8.2/yplib/
+-rw-rw-rw-   0        0        0      469 2023-06-25 08:09:01.000000 yplib-1.8.2/yplib/__init__.py
+-rw-rw-rw-   0        0        0    11744 2023-06-26 01:25:08.000000 yplib-1.8.2/yplib/chart.py
+-rw-rw-rw-   0        0        0     8553 2023-06-26 00:52:29.000000 yplib-1.8.2/yplib/chart_html.py
+-rw-rw-rw-   0        0        0      838 2023-06-26 01:33:00.000000 yplib-1.8.2/yplib/db.py
+-rw-rw-rw-   0        0        0     6984 2023-06-16 00:59:15.000000 yplib-1.8.2/yplib/file.py
+-rw-rw-rw-   0        0        0     3471 2023-06-19 01:33:36.000000 yplib-1.8.2/yplib/http_util.py
+-rw-rw-rw-   0        0        0    26687 2023-06-25 07:43:37.000000 yplib-1.8.2/yplib/index.py
+-rw-rw-rw-   0        0        0      124 2023-06-25 07:57:19.000000 yplib-1.8.2/yplib/temp.py
+drwxrwxrwx   0        0        0        0 2023-06-26 01:33:37.336283 yplib-1.8.2/yplib.egg-info/
+-rw-rw-rw-   0        0        0      352 2023-06-26 01:33:37.000000 yplib-1.8.2/yplib.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      269 2023-06-26 01:33:37.000000 yplib-1.8.2/yplib.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-26 01:33:37.000000 yplib-1.8.2/yplib.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        6 2023-06-26 01:33:37.000000 yplib-1.8.2/yplib.egg-info/top_level.txt
```

### Comparing `yplib-1.8.1/LICENSE` & `yplib-1.8.2/LICENSE`

 * *Files identical despite different names*

### Comparing `yplib-1.8.1/setup.py` & `yplib-1.8.2/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 with open("README.md", "r") as fh:
   long_description = fh.read()
 
 setuptools.setup(
   name="yplib",
-  version="1.8.1",
+  version="1.8.2",
   author="yangpu",
   author_email="wantwaterfish@gmail.com",
   description="util",
   long_description=long_description,
   long_description_content_type="text/markdown",
   packages=setuptools.find_packages(),
   classifiers=[
```

### Comparing `yplib-1.8.1/yplib/chart.py` & `yplib-1.8.2/yplib/chart.py`

 * *Files identical despite different names*

### Comparing `yplib-1.8.1/yplib/chart_html.py` & `yplib-1.8.2/yplib/chart_html.py`

 * *Files identical despite different names*

### Comparing `yplib-1.8.1/yplib/db.py` & `yplib-1.8.2/yplib/db.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,19 +1,24 @@
 from yplib.index import *
 import pymysql
 
 
 # 有关数据库操作的类
-def get_connect(db, user, passwd, charset, port, host):
-    return pymysql.connect(db='MoneyKing', user='moneyking_uer', passwd='3^qp3Xqt4bG7', charset="utf8mb4",
-                           port=3307,
-                           host='192.168.40.230')
+def get_connect(db='MoneyKing', user='moneyking_uer', passwd='3^qp3Xqt4bG7', charset='utf8mb4', port=3306, host='192.168.40.230'):
+    # return pymysql.connect(db='MoneyKing', user='moneyking_uer', passwd='3^qp3Xqt4bG7', charset="utf8mb4",
+    #                        port=3307,
+    #                        host='192.168.40.230')
+    return pymysql.connect(db=db, user=user, passwd=passwd, charset=charset, port=port, host=host)
 
 
 # 执行 sql 语句
 def exec_sql(db_conn, sql='', commit=True):
-    local_cursor = db_conn.cursor()
-    local_cursor.execute(sql)
+    db_cursor = db_conn.cursor()
+    if isinstance(sql, list) or isinstance(sql, set):
+        for s in sql:
+            db_cursor.execute(s)
+    else:
+        db_cursor.execute(str(sql))
     if commit:
         db_conn.commit()
 
 # print('end')
```

### Comparing `yplib-1.8.1/yplib/file.py` & `yplib-1.8.2/yplib/file.py`

 * *Files identical despite different names*

### Comparing `yplib-1.8.1/yplib/http_util.py` & `yplib-1.8.2/yplib/http_util.py`

 * *Files identical despite different names*

### Comparing `yplib-1.8.1/yplib/index.py` & `yplib-1.8.2/yplib/index.py`

 * *Files identical despite different names*

