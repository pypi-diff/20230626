# Comparing `tmp/sqlite-web-0.4.1.tar.gz` & `tmp/sqlite-web-0.5.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/sqlite-web-0.4.1.tar", last modified: Fri Dec  9 13:29:02 2022, max compression
+gzip compressed data, was "dist/sqlite-web-0.5.0.tar", last modified: Mon Jun 26 01:40:16 2023, max compression
```

## Comparing `sqlite-web-0.4.1.tar` & `sqlite-web-0.5.0.tar`

### file list

```diff
@@ -1,71 +1,75 @@
-drwxr-xr-x   0 charles   (1000) charles   (1000)        0 2022-12-09 13:29:02.000000 sqlite-web-0.4.1/
--rw-r--r--   0 charles   (1000) charles   (1000)       94 2018-08-16 18:40:47.000000 sqlite-web-0.4.1/MANIFEST.in
--rw-r--r--   0 charles   (1000) charles   (1000)      511 2022-12-09 13:29:02.000000 sqlite-web-0.4.1/PKG-INFO
--rw-r--r--   0 charles   (1000) charles   (1000)     3230 2021-10-13 13:24:19.000000 sqlite-web-0.4.1/README.md
-drwxr-xr-x   0 charles   (1000) charles   (1000)        0 2022-12-09 13:29:02.000000 sqlite-web-0.4.1/docker/
--rw-r--r--   0 charles   (1000) charles   (1000)      309 2018-08-16 18:40:47.000000 sqlite-web-0.4.1/docker/Dockerfile
--rwxr-xr-x   0 charles   (1000) charles   (1000)      334 2018-08-16 18:40:47.000000 sqlite-web-0.4.1/run-docker
--rw-r--r--   0 charles   (1000) charles   (1000)       38 2022-12-09 13:29:02.000000 sqlite-web-0.4.1/setup.cfg
--rw-r--r--   0 charles   (1000) charles   (1000)     1219 2022-12-09 13:28:51.000000 sqlite-web-0.4.1/setup.py
-drwxr-xr-x   0 charles   (1000) charles   (1000)        0 2022-12-09 13:29:02.000000 sqlite-web-0.4.1/sqlite_web/
--rw-r--r--   0 charles   (1000) charles   (1000)        0 2018-08-16 18:40:47.000000 sqlite-web-0.4.1/sqlite_web/__init__.py
--rw-r--r--   0 charles   (1000) charles   (1000)      153 2022-03-11 19:44:53.000000 sqlite-web-0.4.1/sqlite_web/__main__.py
-drwxr-xr-x   0 charles   (1000) charles   (1000)        0 2022-12-09 13:29:02.000000 sqlite-web-0.4.1/sqlite_web/__pycache__/
--rw-r--r--   0 charles   (1000) charles   (1000)      139 2022-06-13 19:07:21.000000 sqlite-web-0.4.1/sqlite_web/__pycache__/__init__.cpython-37.pyc
--rw-r--r--   0 charles   (1000) charles   (1000)      287 2022-06-13 19:07:21.000000 sqlite-web-0.4.1/sqlite_web/__pycache__/__main__.cpython-37.pyc
--rw-r--r--   0 charles   (1000) charles   (1000)    25756 2022-06-13 19:07:21.000000 sqlite-web-0.4.1/sqlite_web/__pycache__/sqlite_web.cpython-37.pyc
--rwxr-xr-x   0 charles   (1000) charles   (1000)    28750 2022-03-29 14:33:41.000000 sqlite-web-0.4.1/sqlite_web/sqlite_web.py
-drwxr-xr-x   0 charles   (1000) charles   (1000)        0 2022-12-09 13:29:02.000000 sqlite-web-0.4.1/sqlite_web/static/
-drwxr-xr-x   0 charles   (1000) charles   (1000)        0 2022-12-09 13:29:02.000000 sqlite-web-0.4.1/sqlite_web/static/css/
--rw-r--r--   0 charles   (1000) charles   (1000)   153641 2018-08-16 18:40:47.000000 sqlite-web-0.4.1/sqlite_web/static/css/bootstrap.min.css
--rw-r--r--   0 charles   (1000) charles   (1000)      169 2018-08-16 18:40:47.000000 sqlite-web-0.4.1/sqlite_web/static/css/sqlbrowse.css
--rw-r--r--   0 charles   (1000) charles   (1000)     3489 2018-08-16 18:40:47.000000 sqlite-web-0.4.1/sqlite_web/static/css/syntax-highlight.css
-drwxr-xr-x   0 charles   (1000) charles   (1000)        0 2022-12-09 13:29:02.000000 sqlite-web-0.4.1/sqlite_web/static/fonts/
--rw-r--r--   0 charles   (1000) charles   (1000)    20335 2018-08-16 18:40:47.000000 sqlite-web-0.4.1/sqlite_web/static/fonts/glyphicons-halflings-regular.eot
--rw-r--r--   0 charles   (1000) charles   (1000)    62927 2018-08-16 18:40:47.000000 sqlite-web-0.4.1/sqlite_web/static/fonts/glyphicons-halflings-regular.svg
--rw-r--r--   0 charles   (1000) charles   (1000)    41280 2018-08-16 18:40:47.000000 sqlite-web-0.4.1/sqlite_web/static/fonts/glyphicons-halflings-regular.ttf
--rw-r--r--   0 charles   (1000) charles   (1000)    23320 2018-08-16 18:40:47.000000 sqlite-web-0.4.1/sqlite_web/static/fonts/glyphicons-halflings-regular.woff
-drwxr-xr-x   0 charles   (1000) charles   (1000)        0 2022-12-09 13:29:02.000000 sqlite-web-0.4.1/sqlite_web/static/img/
--rw-r--r--   0 charles   (1000) charles   (1000)     8076 2018-08-16 18:40:47.000000 sqlite-web-0.4.1/sqlite_web/static/img/delete.png
--rw-r--r--   0 charles   (1000) charles   (1000)    42695 2018-08-16 18:40:47.000000 sqlite-web-0.4.1/sqlite_web/static/img/expression.png
--rw-r--r--   0 charles   (1000) charles   (1000)     7681 2018-08-16 18:40:47.000000 sqlite-web-0.4.1/sqlite_web/static/img/index-create.png
--rw-r--r--   0 charles   (1000) charles   (1000)     2982 2018-08-16 18:40:47.000000 sqlite-web-0.4.1/sqlite_web/static/img/index-drop.png
--rw-r--r--   0 charles   (1000) charles   (1000)    20342 2018-08-16 18:40:47.000000 sqlite-web-0.4.1/sqlite_web/static/img/insert.png
--rw-r--r--   0 charles   (1000) charles   (1000)    25300 2018-08-16 18:40:47.000000 sqlite-web-0.4.1/sqlite_web/static/img/select-advanced.png
--rw-r--r--   0 charles   (1000) charles   (1000)    14405 2018-08-16 18:40:47.000000 sqlite-web-0.4.1/sqlite_web/static/img/select.png
--rw-r--r--   0 charles   (1000) charles   (1000)     5221 2018-08-16 18:40:47.000000 sqlite-web-0.4.1/sqlite_web/static/img/table-alter.png
--rw-r--r--   0 charles   (1000) charles   (1000)    12190 2018-08-16 18:40:47.000000 sqlite-web-0.4.1/sqlite_web/static/img/table-create.png
--rw-r--r--   0 charles   (1000) charles   (1000)     3039 2018-08-16 18:40:47.000000 sqlite-web-0.4.1/sqlite_web/static/img/table-drop.png
--rw-r--r--   0 charles   (1000) charles   (1000)    23018 2018-08-16 18:40:47.000000 sqlite-web-0.4.1/sqlite_web/static/img/trigger-create.png
--rw-r--r--   0 charles   (1000) charles   (1000)     3669 2018-08-16 18:40:47.000000 sqlite-web-0.4.1/sqlite_web/static/img/trigger-drop.png
--rw-r--r--   0 charles   (1000) charles   (1000)    17914 2018-08-16 18:40:47.000000 sqlite-web-0.4.1/sqlite_web/static/img/update.png
--rw-r--r--   0 charles   (1000) charles   (1000)     7284 2018-08-16 18:40:47.000000 sqlite-web-0.4.1/sqlite_web/static/img/view-create.png
--rw-r--r--   0 charles   (1000) charles   (1000)     3040 2018-08-16 18:40:47.000000 sqlite-web-0.4.1/sqlite_web/static/img/view-drop.png
-drwxr-xr-x   0 charles   (1000) charles   (1000)        0 2022-12-09 13:29:02.000000 sqlite-web-0.4.1/sqlite_web/static/js/
--rw-r--r--   0 charles   (1000) charles   (1000)    67742 2018-08-16 18:40:47.000000 sqlite-web-0.4.1/sqlite_web/static/js/bootstrap.bundle.min.js
--rw-r--r--   0 charles   (1000) charles   (1000)    96381 2018-08-16 18:40:47.000000 sqlite-web-0.4.1/sqlite_web/static/js/jquery-1.11.0.min.js
-drwxr-xr-x   0 charles   (1000) charles   (1000)        0 2022-12-09 13:29:02.000000 sqlite-web-0.4.1/sqlite_web/templates/
--rw-r--r--   0 charles   (1000) charles   (1000)     1090 2022-03-29 14:33:41.000000 sqlite-web-0.4.1/sqlite_web/templates/add_column.html
--rw-r--r--   0 charles   (1000) charles   (1000)     1086 2018-08-16 18:40:47.000000 sqlite-web-0.4.1/sqlite_web/templates/add_index.html
--rw-r--r--   0 charles   (1000) charles   (1000)     3517 2022-03-29 14:33:41.000000 sqlite-web-0.4.1/sqlite_web/templates/base.html
--rw-r--r--   0 charles   (1000) charles   (1000)     1251 2018-08-16 18:40:47.000000 sqlite-web-0.4.1/sqlite_web/templates/base_table.html
--rw-r--r--   0 charles   (1000) charles   (1000)     1375 2021-05-26 21:50:16.000000 sqlite-web-0.4.1/sqlite_web/templates/base_tables.html
--rw-r--r--   0 charles   (1000) charles   (1000)      811 2018-08-16 18:40:47.000000 sqlite-web-0.4.1/sqlite_web/templates/drop_column.html
--rw-r--r--   0 charles   (1000) charles   (1000)      777 2018-08-16 18:40:47.000000 sqlite-web-0.4.1/sqlite_web/templates/drop_index.html
--rw-r--r--   0 charles   (1000) charles   (1000)      558 2018-08-16 18:40:47.000000 sqlite-web-0.4.1/sqlite_web/templates/drop_table.html
--rw-r--r--   0 charles   (1000) charles   (1000)      796 2018-08-16 18:40:47.000000 sqlite-web-0.4.1/sqlite_web/templates/drop_trigger.html
--rw-r--r--   0 charles   (1000) charles   (1000)     1229 2018-08-16 18:40:47.000000 sqlite-web-0.4.1/sqlite_web/templates/index.html
--rw-r--r--   0 charles   (1000) charles   (1000)      465 2018-08-16 18:40:47.000000 sqlite-web-0.4.1/sqlite_web/templates/login.html
--rw-r--r--   0 charles   (1000) charles   (1000)     1139 2018-08-16 18:40:47.000000 sqlite-web-0.4.1/sqlite_web/templates/rename_column.html
--rw-r--r--   0 charles   (1000) charles   (1000)     2418 2018-08-16 18:40:47.000000 sqlite-web-0.4.1/sqlite_web/templates/table_content.html
--rw-r--r--   0 charles   (1000) charles   (1000)     1345 2018-08-16 18:40:47.000000 sqlite-web-0.4.1/sqlite_web/templates/table_import.html
--rw-r--r--   0 charles   (1000) charles   (1000)     5462 2022-12-09 03:15:35.000000 sqlite-web-0.4.1/sqlite_web/templates/table_query.html
--rw-r--r--   0 charles   (1000) charles   (1000)     5629 2018-08-16 18:40:47.000000 sqlite-web-0.4.1/sqlite_web/templates/table_structure.html
-drwxr-xr-x   0 charles   (1000) charles   (1000)        0 2022-12-09 13:29:02.000000 sqlite-web-0.4.1/sqlite_web.egg-info/
--rw-r--r--   0 charles   (1000) charles   (1000)      511 2022-12-09 13:29:02.000000 sqlite-web-0.4.1/sqlite_web.egg-info/PKG-INFO
--rw-r--r--   0 charles   (1000) charles   (1000)     2095 2022-12-09 13:29:02.000000 sqlite-web-0.4.1/sqlite_web.egg-info/SOURCES.txt
--rw-r--r--   0 charles   (1000) charles   (1000)        1 2022-12-09 13:29:02.000000 sqlite-web-0.4.1/sqlite_web.egg-info/dependency_links.txt
--rw-r--r--   0 charles   (1000) charles   (1000)       59 2022-12-09 13:29:02.000000 sqlite-web-0.4.1/sqlite_web.egg-info/entry_points.txt
--rw-r--r--   0 charles   (1000) charles   (1000)        1 2022-12-09 13:29:02.000000 sqlite-web-0.4.1/sqlite_web.egg-info/not-zip-safe
--rw-r--r--   0 charles   (1000) charles   (1000)       29 2022-12-09 13:29:02.000000 sqlite-web-0.4.1/sqlite_web.egg-info/requires.txt
--rw-r--r--   0 charles   (1000) charles   (1000)       11 2022-12-09 13:29:02.000000 sqlite-web-0.4.1/sqlite_web.egg-info/top_level.txt
+drwxr-xr-x   0 charles   (1000) charles   (1000)        0 2023-06-26 01:40:16.000000 sqlite-web-0.5.0/
+-rw-r--r--   0 charles   (1000) charles   (1000)       94 2018-08-16 18:40:47.000000 sqlite-web-0.5.0/MANIFEST.in
+-rw-r--r--   0 charles   (1000) charles   (1000)      511 2023-06-26 01:40:16.000000 sqlite-web-0.5.0/PKG-INFO
+-rw-r--r--   0 charles   (1000) charles   (1000)     3835 2023-04-18 18:28:09.000000 sqlite-web-0.5.0/README.md
+drwxr-xr-x   0 charles   (1000) charles   (1000)        0 2023-06-26 01:40:16.000000 sqlite-web-0.5.0/docker/
+-rw-r--r--   0 charles   (1000) charles   (1000)     2105 2023-04-19 14:27:45.000000 sqlite-web-0.5.0/docker/Dockerfile
+-rwxr-xr-x   0 charles   (1000) charles   (1000)      334 2018-08-16 18:40:47.000000 sqlite-web-0.5.0/run-docker
+-rw-r--r--   0 charles   (1000) charles   (1000)       38 2023-06-26 01:40:16.000000 sqlite-web-0.5.0/setup.cfg
+-rw-r--r--   0 charles   (1000) charles   (1000)     1219 2023-06-26 01:38:48.000000 sqlite-web-0.5.0/setup.py
+drwxr-xr-x   0 charles   (1000) charles   (1000)        0 2023-06-26 01:40:16.000000 sqlite-web-0.5.0/sqlite_web/
+-rw-r--r--   0 charles   (1000) charles   (1000)        0 2018-08-16 18:40:47.000000 sqlite-web-0.5.0/sqlite_web/__init__.py
+-rw-r--r--   0 charles   (1000) charles   (1000)      153 2022-03-11 19:44:53.000000 sqlite-web-0.5.0/sqlite_web/__main__.py
+drwxr-xr-x   0 charles   (1000) charles   (1000)        0 2023-06-26 01:40:16.000000 sqlite-web-0.5.0/sqlite_web/__pycache__/
+-rw-r--r--   0 charles   (1000) charles   (1000)      139 2022-06-13 19:07:21.000000 sqlite-web-0.5.0/sqlite_web/__pycache__/__init__.cpython-37.pyc
+-rw-r--r--   0 charles   (1000) charles   (1000)      287 2022-06-13 19:07:21.000000 sqlite-web-0.5.0/sqlite_web/__pycache__/__main__.cpython-37.pyc
+-rw-r--r--   0 charles   (1000) charles   (1000)    25756 2022-06-13 19:07:21.000000 sqlite-web-0.5.0/sqlite_web/__pycache__/sqlite_web.cpython-37.pyc
+-rwxr-xr-x   0 charles   (1000) charles   (1000)    38799 2023-04-18 18:28:09.000000 sqlite-web-0.5.0/sqlite_web/sqlite_web.py
+drwxr-xr-x   0 charles   (1000) charles   (1000)        0 2023-06-26 01:40:16.000000 sqlite-web-0.5.0/sqlite_web/static/
+drwxr-xr-x   0 charles   (1000) charles   (1000)        0 2023-06-26 01:40:16.000000 sqlite-web-0.5.0/sqlite_web/static/css/
+-rw-r--r--   0 charles   (1000) charles   (1000)   153641 2018-08-16 18:40:47.000000 sqlite-web-0.5.0/sqlite_web/static/css/bootstrap.min.css
+-rw-r--r--   0 charles   (1000) charles   (1000)      169 2018-08-16 18:40:47.000000 sqlite-web-0.5.0/sqlite_web/static/css/sqlbrowse.css
+-rw-r--r--   0 charles   (1000) charles   (1000)     3489 2018-08-16 18:40:47.000000 sqlite-web-0.5.0/sqlite_web/static/css/syntax-highlight.css
+drwxr-xr-x   0 charles   (1000) charles   (1000)        0 2023-06-26 01:40:16.000000 sqlite-web-0.5.0/sqlite_web/static/fonts/
+-rw-r--r--   0 charles   (1000) charles   (1000)    20335 2018-08-16 18:40:47.000000 sqlite-web-0.5.0/sqlite_web/static/fonts/glyphicons-halflings-regular.eot
+-rw-r--r--   0 charles   (1000) charles   (1000)    62927 2018-08-16 18:40:47.000000 sqlite-web-0.5.0/sqlite_web/static/fonts/glyphicons-halflings-regular.svg
+-rw-r--r--   0 charles   (1000) charles   (1000)    41280 2018-08-16 18:40:47.000000 sqlite-web-0.5.0/sqlite_web/static/fonts/glyphicons-halflings-regular.ttf
+-rw-r--r--   0 charles   (1000) charles   (1000)    23320 2018-08-16 18:40:47.000000 sqlite-web-0.5.0/sqlite_web/static/fonts/glyphicons-halflings-regular.woff
+drwxr-xr-x   0 charles   (1000) charles   (1000)        0 2023-06-26 01:40:16.000000 sqlite-web-0.5.0/sqlite_web/static/img/
+-rw-r--r--   0 charles   (1000) charles   (1000)     8076 2018-08-16 18:40:47.000000 sqlite-web-0.5.0/sqlite_web/static/img/delete.png
+-rw-r--r--   0 charles   (1000) charles   (1000)    42695 2018-08-16 18:40:47.000000 sqlite-web-0.5.0/sqlite_web/static/img/expression.png
+-rw-r--r--   0 charles   (1000) charles   (1000)     7681 2018-08-16 18:40:47.000000 sqlite-web-0.5.0/sqlite_web/static/img/index-create.png
+-rw-r--r--   0 charles   (1000) charles   (1000)     2982 2018-08-16 18:40:47.000000 sqlite-web-0.5.0/sqlite_web/static/img/index-drop.png
+-rw-r--r--   0 charles   (1000) charles   (1000)    20342 2018-08-16 18:40:47.000000 sqlite-web-0.5.0/sqlite_web/static/img/insert.png
+-rw-r--r--   0 charles   (1000) charles   (1000)    25300 2018-08-16 18:40:47.000000 sqlite-web-0.5.0/sqlite_web/static/img/select-advanced.png
+-rw-r--r--   0 charles   (1000) charles   (1000)    14405 2018-08-16 18:40:47.000000 sqlite-web-0.5.0/sqlite_web/static/img/select.png
+-rw-r--r--   0 charles   (1000) charles   (1000)     5221 2018-08-16 18:40:47.000000 sqlite-web-0.5.0/sqlite_web/static/img/table-alter.png
+-rw-r--r--   0 charles   (1000) charles   (1000)    12190 2018-08-16 18:40:47.000000 sqlite-web-0.5.0/sqlite_web/static/img/table-create.png
+-rw-r--r--   0 charles   (1000) charles   (1000)     3039 2018-08-16 18:40:47.000000 sqlite-web-0.5.0/sqlite_web/static/img/table-drop.png
+-rw-r--r--   0 charles   (1000) charles   (1000)    23018 2018-08-16 18:40:47.000000 sqlite-web-0.5.0/sqlite_web/static/img/trigger-create.png
+-rw-r--r--   0 charles   (1000) charles   (1000)     3669 2018-08-16 18:40:47.000000 sqlite-web-0.5.0/sqlite_web/static/img/trigger-drop.png
+-rw-r--r--   0 charles   (1000) charles   (1000)    17914 2018-08-16 18:40:47.000000 sqlite-web-0.5.0/sqlite_web/static/img/update.png
+-rw-r--r--   0 charles   (1000) charles   (1000)     7284 2018-08-16 18:40:47.000000 sqlite-web-0.5.0/sqlite_web/static/img/view-create.png
+-rw-r--r--   0 charles   (1000) charles   (1000)     3040 2018-08-16 18:40:47.000000 sqlite-web-0.5.0/sqlite_web/static/img/view-drop.png
+drwxr-xr-x   0 charles   (1000) charles   (1000)        0 2023-06-26 01:40:16.000000 sqlite-web-0.5.0/sqlite_web/static/js/
+-rw-r--r--   0 charles   (1000) charles   (1000)    67742 2018-08-16 18:40:47.000000 sqlite-web-0.5.0/sqlite_web/static/js/bootstrap.bundle.min.js
+-rw-r--r--   0 charles   (1000) charles   (1000)    96381 2018-08-16 18:40:47.000000 sqlite-web-0.5.0/sqlite_web/static/js/jquery-1.11.0.min.js
+drwxr-xr-x   0 charles   (1000) charles   (1000)        0 2023-06-26 01:40:16.000000 sqlite-web-0.5.0/sqlite_web/templates/
+-rw-r--r--   0 charles   (1000) charles   (1000)     1090 2022-03-29 14:33:41.000000 sqlite-web-0.5.0/sqlite_web/templates/add_column.html
+-rw-r--r--   0 charles   (1000) charles   (1000)     1086 2018-08-16 18:40:47.000000 sqlite-web-0.5.0/sqlite_web/templates/add_index.html
+-rw-r--r--   0 charles   (1000) charles   (1000)     3517 2022-03-29 14:33:41.000000 sqlite-web-0.5.0/sqlite_web/templates/base.html
+-rw-r--r--   0 charles   (1000) charles   (1000)     1634 2023-04-18 18:28:09.000000 sqlite-web-0.5.0/sqlite_web/templates/base_table.html
+-rw-r--r--   0 charles   (1000) charles   (1000)     1375 2021-05-26 21:50:16.000000 sqlite-web-0.5.0/sqlite_web/templates/base_tables.html
+-rw-r--r--   0 charles   (1000) charles   (1000)      811 2018-08-16 18:40:47.000000 sqlite-web-0.5.0/sqlite_web/templates/drop_column.html
+-rw-r--r--   0 charles   (1000) charles   (1000)      777 2018-08-16 18:40:47.000000 sqlite-web-0.5.0/sqlite_web/templates/drop_index.html
+-rw-r--r--   0 charles   (1000) charles   (1000)      558 2023-04-17 10:00:39.000000 sqlite-web-0.5.0/sqlite_web/templates/drop_table.html
+-rw-r--r--   0 charles   (1000) charles   (1000)      796 2018-08-16 18:40:47.000000 sqlite-web-0.5.0/sqlite_web/templates/drop_trigger.html
+-rw-r--r--   0 charles   (1000) charles   (1000)     1229 2018-08-16 18:40:47.000000 sqlite-web-0.5.0/sqlite_web/templates/index.html
+-rw-r--r--   0 charles   (1000) charles   (1000)      465 2018-08-16 18:40:47.000000 sqlite-web-0.5.0/sqlite_web/templates/login.html
+-rw-r--r--   0 charles   (1000) charles   (1000)     1139 2018-08-16 18:40:47.000000 sqlite-web-0.5.0/sqlite_web/templates/rename_column.html
+-rw-r--r--   0 charles   (1000) charles   (1000)     2873 2023-04-18 18:28:09.000000 sqlite-web-0.5.0/sqlite_web/templates/table_content.html
+-rw-r--r--   0 charles   (1000) charles   (1000)      721 2023-04-18 18:28:09.000000 sqlite-web-0.5.0/sqlite_web/templates/table_delete.html
+-rw-r--r--   0 charles   (1000) charles   (1000)     1060 2023-04-18 18:28:09.000000 sqlite-web-0.5.0/sqlite_web/templates/table_export.html
+-rw-r--r--   0 charles   (1000) charles   (1000)     1345 2018-08-16 18:40:47.000000 sqlite-web-0.5.0/sqlite_web/templates/table_import.html
+-rw-r--r--   0 charles   (1000) charles   (1000)     2690 2023-04-18 18:28:09.000000 sqlite-web-0.5.0/sqlite_web/templates/table_insert.html
+-rw-r--r--   0 charles   (1000) charles   (1000)     5499 2023-04-11 19:10:55.000000 sqlite-web-0.5.0/sqlite_web/templates/table_query.html
+-rw-r--r--   0 charles   (1000) charles   (1000)     5362 2023-04-11 19:10:55.000000 sqlite-web-0.5.0/sqlite_web/templates/table_structure.html
+-rw-r--r--   0 charles   (1000) charles   (1000)     3175 2023-04-18 18:28:09.000000 sqlite-web-0.5.0/sqlite_web/templates/table_update.html
+drwxr-xr-x   0 charles   (1000) charles   (1000)        0 2023-06-26 01:40:16.000000 sqlite-web-0.5.0/sqlite_web.egg-info/
+-rw-r--r--   0 charles   (1000) charles   (1000)      511 2023-06-26 01:40:16.000000 sqlite-web-0.5.0/sqlite_web.egg-info/PKG-INFO
+-rw-r--r--   0 charles   (1000) charles   (1000)     2251 2023-06-26 01:40:16.000000 sqlite-web-0.5.0/sqlite_web.egg-info/SOURCES.txt
+-rw-r--r--   0 charles   (1000) charles   (1000)        1 2023-06-26 01:40:16.000000 sqlite-web-0.5.0/sqlite_web.egg-info/dependency_links.txt
+-rw-r--r--   0 charles   (1000) charles   (1000)       59 2023-06-26 01:40:16.000000 sqlite-web-0.5.0/sqlite_web.egg-info/entry_points.txt
+-rw-r--r--   0 charles   (1000) charles   (1000)        1 2022-12-09 13:29:02.000000 sqlite-web-0.5.0/sqlite_web.egg-info/not-zip-safe
+-rw-r--r--   0 charles   (1000) charles   (1000)       29 2023-06-26 01:40:16.000000 sqlite-web-0.5.0/sqlite_web.egg-info/requires.txt
+-rw-r--r--   0 charles   (1000) charles   (1000)       11 2023-06-26 01:40:16.000000 sqlite-web-0.5.0/sqlite_web.egg-info/top_level.txt
```

### Comparing `sqlite-web-0.4.1/README.md` & `sqlite-web-0.5.0/README.md`

 * *Files 21% similar despite different names*

```diff
@@ -28,36 +28,53 @@
 * Add or drop:
   * Tables
   * Columns (yes, you can drop and rename columns!)
   * Indexes
 * Export data as JSON or CSV.
 * Import JSON or CSV files.
 * Browse table data.
+* Insert, Update or Delete rows.
 
 ### Screenshots
 
 The index page shows some basic information about the database, including the number of tables and indexes, as well as its size on disk:
 
-![](http://media.charlesleifer.com/blog/photos/s1415479324.32.png)
+![](https://media.charlesleifer.com/blog/photos/sqw-index.png)
 
-The `structure` tab displays information about the structure of the table, including columns, indexes, and foreign keys (if any exist). From this page you can also create, rename or drop columns and indexes.
+The `structure` tab displays information about the structure of the table, including columns, indexes, triggers, and foreign keys (if any exist). From this page you can also create, rename or drop columns and indexes.
 
-![](http://media.charlesleifer.com/blog/photos/s1415479418.23.png)
+![](https://media.charlesleifer.com/blog/photos/sqw-structure.png)
+
+Columns are easy to add, drop or rename:
+
+![](https://media.charlesleifer.com/blog/photos/sqw-add-column.png)
 
 The `content` tab displays all the table data. Links in the table header can be used to sort the data:
 
-![](http://media.charlesleifer.com/blog/photos/s1415479502.61.png)
+![](https://media.charlesleifer.com/blog/photos/sqw-content.png)
 
 The `query` tab allows you to execute arbitrary SQL queries on a table. The query results are displayed in a table and can be exported to either JSON or CSV:
 
-![](http://media.charlesleifer.com/blog/photos/s1415487149.3.png)
+![](https://media.charlesleifer.com/blog/photos/sqw-query.png)
 
 The `import` tab supports importing CSV and JSON files into a table. There is an option to automatically create columns for any unrecognized keys in the import file:
 
-![](http://media.charlesleifer.com/blog/photos/s1415479625.44.png)
+![](https://media.charlesleifer.com/blog/photos/sqw-import.png)
+
+The `export` tab supports exporting all, or a subset, of columns:
+
+![](https://media.charlesleifer.com/blog/photos/sqw-export.png)
+
+Basic INSERT, UPDATE and DELETE queries are supported:
+
+![](https://media.charlesleifer.com/blog/photos/sqw-insert.png)
+
+![](https://media.charlesleifer.com/blog/photos/sqw-update.png)
+
+![](https://media.charlesleifer.com/blog/photos/sqw-delete.png)
 
 ### Command-line options
 
 The syntax for invoking sqlite-web is:
 
 ```console
 
@@ -71,14 +88,15 @@
 * ``-d``, ``--debug``: default is false
 * ``-x``, ``--no-browser``: do not open a web-browser when sqlite-web starts.
 * ``-P``, ``--password``: prompt for password to access sqlite-web.
   Alternatively, the password can be stored in the "SQLITE_WEB_PASSWORD"
   environment variable, in which case the application will not prompt for a
   password, but will use the value from the environment.
 * ``-r``, ``--read-only``: open database in read-only mode.
+* ``-R``, ``--rows-per-page``: set pagination on content page, default 50 rows.
 * ``-e``, ``--extension``: path or name of loadable extension(s). To load
   multiple extensions, specify ``-e [path]`` for each extension.
 * ``-u``, ``--url-prefix``: URL prefix for application, e.g. "/sqlite-web".
 * ``-c``, ``--cert`` and ``-k``, ``--key`` - specify SSL cert and private key.
 * ``-a``, ``--ad-hoc`` - run using an ad-hoc SSL context.
 
 ### Using docker
```

### Comparing `sqlite-web-0.4.1/setup.py` & `sqlite-web-0.5.0/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -8,15 +8,15 @@
     with open(readme) as fh:
         long_description = fh.read()
 else:
     long_description = ''
 
 setup(
     name='sqlite-web',
-    version='0.4.1',
+    version='0.5.0',
     description='Web-based SQLite database browser.',
     long_description='Web-based SQLite database browser.',
     author='Charles Leifer',
     author_email='coleifer@gmail.com',
     url='https://github.com/coleifer/sqlite-web',
     license='MIT',
     install_requires=[
```

### Comparing `sqlite-web-0.4.1/sqlite_web/__pycache__/sqlite_web.cpython-37.pyc` & `sqlite-web-0.5.0/sqlite_web/__pycache__/sqlite_web.cpython-37.pyc`

 * *Files identical despite different names*

### Comparing `sqlite-web-0.4.1/sqlite_web/sqlite_web.py` & `sqlite-web-0.5.0/sqlite_web/sqlite_web.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,9 +1,10 @@
 #!/usr/bin/env python
 
+import base64
 import datetime
 import hashlib
 import math
 import operator
 import optparse
 import os
 import re
@@ -26,23 +27,29 @@
     from StringIO import StringIO
 else:
     PY2 = False
     binary_types = (bytes, bytearray)
     decode_handler = 'backslashreplace'
     numeric = (int, float)
     unicode_type = str
+    from functools import reduce
     from io import StringIO
 
 try:
     from flask import (
-        Flask, abort, escape, flash, jsonify, make_response, Markup, redirect,
+        Flask, abort, flash, jsonify, make_response, redirect,
         render_template, request, session, url_for)
 except ImportError:
     raise RuntimeError('Unable to import flask module. Install by running '
                        'pip install flask')
+try:
+    from markupsafe import Markup, escape
+except ImportError:
+    raise RuntimeError('Unable to import markupsafe module. Install by running'
+                       ' pip install markupsafe')
 
 try:
     from pygments import formatters, highlight, lexers
 except ImportError:
     import warnings
     warnings.warn('pygments library not found.', ImportWarning)
     syntax_highlight = lambda data: '<pre>%s</pre>' % data
@@ -252,25 +259,28 @@
     if request.method == 'POST':
         return request.form
     return request.args
 
 @app.route('/<table>/add-column/', methods=['GET', 'POST'])
 @require_table
 def add_column(table):
+    class JsonField(TextField):
+        field_type = 'JSON'
     column_mapping = OrderedDict((
-        ('VARCHAR', CharField),
         ('TEXT', TextField),
         ('INTEGER', IntegerField),
         ('REAL', FloatField),
-        ('BOOL', BooleanField),
         ('BLOB', BlobField),
+        ('JSON', JsonField),
+        ('BOOL', BooleanField),
         ('DATETIME', DateTimeField),
         ('DATE', DateField),
+        ('DECIMAL', DecimalField),
         ('TIME', TimeField),
-        ('DECIMAL', DecimalField)))
+        ('VARCHAR', CharField)))
 
     request_data = get_request_data()
     col_type = request_data.get('type')
     name = request_data.get('name', '')
 
     if request.method == 'POST':
         if name and col_type in column_mapping:
@@ -419,41 +429,47 @@
     return render_template(
         'drop_trigger.html',
         triggers=triggers,
         trigger_names=trigger_names,
         name=name,
         table=table)
 
+
 @app.route('/<table>/content/')
 @require_table
 def table_content(table):
     page_number = request.args.get('page') or ''
+    if page_number == 'last': page_number = '1000000'
     page_number = int(page_number) if page_number.isdigit() else 1
 
     dataset.update_cache(table)
     ds_table = dataset[table]
+    model = ds_table.model_class
+
     total_rows = ds_table.all().count()
     rows_per_page = app.config['ROWS_PER_PAGE']
-    total_pages = int(math.ceil(total_rows / float(rows_per_page)))
+    total_pages = max(1, int(math.ceil(total_rows / float(rows_per_page))))
     # Restrict bounds.
     page_number = min(page_number, total_pages)
     page_number = max(page_number, 1)
 
     previous_page = page_number - 1 if page_number > 1 else None
     next_page = page_number + 1 if page_number < total_pages else None
 
     query = ds_table.all().paginate(page_number, rows_per_page)
 
     ordering = request.args.get('ordering')
     if ordering:
-        field = ds_table.model_class._meta.columns[ordering.lstrip('-')]
+        field = model._meta.columns[ordering.lstrip('-')]
         if ordering.startswith('-'):
             field = field.desc()
         query = query.order_by(field)
 
+    session['%s.last_viewed' % table] = (page_number, ordering)
+
     field_names = ds_table.columns
     columns = [f.column_name for f in ds_table.model_class._meta.sorted_fields]
 
     table_sql = dataset.query(
         'SELECT sql FROM sqlite_master WHERE tbl_name = ? AND type = ?',
         [table, 'table']).fetchone()[0]
 
@@ -464,29 +480,254 @@
         field_names=field_names,
         next_page=next_page,
         ordering=ordering,
         page=page_number,
         previous_page=previous_page,
         query=query,
         table=table,
+        table_pk=model._meta.primary_key,
         total_pages=total_pages,
         total_rows=total_rows)
 
+def minimal_validate_field(field, value):
+    if value.lower().strip() == 'null':
+        value = None
+    if value is None and not field.null:
+        return 'NULL', 'Column does not allow NULL values.'
+    if isinstance(field, IntegerField) and not value.isdigit():
+        return value, 'Value is not a number.'
+    elif isinstance(field, FloatField):
+        try:
+            _ = float(value)
+        except Exception:
+            return value, 'Value is not a numeric/real.'
+    elif isinstance(field, BooleanField):
+        if value.lower() not in ('1', '0', 'true', 'false', 't', 'f'):
+            return value, 'Value must be 1, 0, true, false, t or f.'
+        value = True if value.lower() in ('1', 't', 'true') else False
+    elif isinstance(field, BlobField):
+        try:
+            value = base64.b64decode(value)
+        except Exception as exc:
+            return value, 'Value must be base64-encoded binary data.'
+    try:
+        field.db_value(value)
+    except Exception as exc:
+        return value, str(exc)
+
+    return value, None
+
+@app.route('/<table>/insert/', methods=['GET', 'POST'])
+@require_table
+def table_insert(table):
+    dataset.update_cache(table)
+    model = dataset[table].model_class
+
+    columns = []
+    col_dict = {}
+    row = {}
+    for column in dataset.get_columns(table):
+        field = model._meta.columns[column.name]
+        if isinstance(field, AutoField):
+            continue
+        columns.append(column)
+        col_dict[column.name] = column
+        row[column.name] = ''
+
+    edited = set()
+    errors = {}
+    if request.method == 'POST':
+        insert = {}
+        for key, value in request.form.items():
+            if key not in col_dict: continue
+            column = col_dict[key]
+            edited.add(column.name)
+            row[column.name] = value
+
+            field = model._meta.columns[column.name]
+            value, err = minimal_validate_field(field, value)
+            if err:
+                errors[key] = err
+            else:
+                insert[field] = value
+
+        if errors:
+            flash('One or more errors prevented the row being inserted.',
+                  'danger')
+        elif insert:
+            try:
+                with dataset.transaction() as txn:
+                    n = model.insert(insert).execute()
+            except Exception as exc:
+                flash('Insert failed: %s' % exc, 'danger')
+            else:
+                flash('Successfully inserted record (%s).' % n, 'success')
+                return redirect(url_for(
+                    'table_content',
+                    table=table,
+                    page='last'))
+        else:
+            flash('No data was specified to be inserted.', 'warning')
+    else:
+        edited = set(col_dict)  # Make all fields editable on load.
+
+    return render_template(
+        'table_insert.html',
+        columns=columns,
+        edited=edited,
+        errors=errors,
+        model=model,
+        row=row,
+        table=table)
+
+def redirect_to_previous(table):
+    page_ordering = session.get('%s.last_viewed' % table)
+    if not page_ordering:
+        return redirect(url_for('table_content', table=table))
+    page, ordering = page_ordering
+    kw = {}
+    if page and page != 1:
+        kw['page'] = page
+    if ordering:
+        kw['ordering'] = ordering
+    return redirect(url_for('table_content', table=table, **kw))
+
+@app.route('/<table>/update/<pk>/', methods=['GET', 'POST'])
+@require_table
+def table_update(table, pk):
+    dataset.update_cache(table)
+    model = dataset[table].model_class
+    table_pk = model._meta.primary_key
+    if not table_pk:
+        flash('Table must have a primary key to perform update.', 'danger')
+        return redirect(url_for('table_content', table=table))
+    elif pk == '__uneditable__':
+        flash('Could not encode primary key to perform update.', 'danger')
+        return redirect(url_for('table_content', table=table))
+
+    expr = decode_pk(model, pk)
+    try:
+        obj = model.get(expr)
+    except model.DoesNotExist:
+        pk_repr = pk_display(table_pk, pk)
+        flash('Could not fetch row with primary-key %s.' % pk_repr, 'danger')
+        return redirect(url_for('table_content', table=table))
+
+    columns = dataset.get_columns(table)
+    col_dict = {}
+    row = {}
+    for column in columns:
+        value = getattr(obj, column.name)
+        if value is None:
+            row[column.name] = None
+        elif column.data_type.lower() == 'blob':
+            row[column.name] = base64.b64encode(value).decode('utf8')
+        else:
+            row[column.name] = value
+
+        col_dict[column.name] = column
+
+    edited = set()
+    errors = {}
+    if request.method == 'POST':
+        update = {}
+        for key, value in request.form.items():
+            if key not in col_dict: continue
+            column = col_dict[key]
+            edited.add(column.name)
+            row[column.name] = value
+
+            field = model._meta.columns[column.name]
+            value, err = minimal_validate_field(field, value)
+            if err:
+                errors[key] = err
+            else:
+                update[field] = value
+
+        if errors:
+            flash('One or more errors prevented the row being updated.',
+                  'danger')
+        elif update:
+            try:
+                with dataset.transaction() as txn:
+                    n = model.update(update).where(expr).execute()
+            except Exception as exc:
+                flash('Update failed: %s' % exc, 'danger')
+            else:
+                flash('Successfully updated %s record.' % n, 'success')
+                return redirect_to_previous(table)
+        else:
+            flash('No data was specified to be updated.', 'warning')
+
+    return render_template(
+        'table_update.html',
+        columns=columns,
+        edited=edited,
+        errors=errors,
+        model=model,
+        pk=pk,
+        row=row,
+        table=table,
+        table_pk=model._meta.primary_key)
+
+@app.route('/<table>/delete/<pk>/', methods=['GET', 'POST'])
+@require_table
+def table_delete(table, pk):
+    dataset.update_cache(table)
+    model = dataset[table].model_class
+    table_pk = model._meta.primary_key
+    if not table_pk:
+        flash('Table must have a primary key to perform delete.', 'danger')
+        return redirect(url_for('table_content', table=table))
+    elif pk == '__uneditable__':
+        flash('Could not encode primary key to perform delete.', 'danger')
+        return redirect(url_for('table_content', table=table))
+
+    expr = decode_pk(model, pk)
+    try:
+        row = model.select().where(expr).dicts().get()
+    except model.DoesNotExist:
+        pk_repr = pk_display(table_pk, pk)
+        flash('Could not fetch row with primary-key %s.' % pk_repr, 'danger')
+        return redirect(url_for('table_content', table=table))
+
+    if request.method == 'POST':
+        try:
+            with dataset.transaction() as txn:
+                n = model.delete().where(expr).execute()
+        except Exception as exc:
+            flash('Delete failed: %s' % exc, 'danger')
+        else:
+            flash('Successfully deleted %s record.' % n, 'success')
+            return redirect_to_previous(table)
+
+    return render_template(
+        'table_delete.html',
+        column_names=[c.name for c in dataset.get_columns(table)],
+        model=model,
+        pk=pk,
+        row=row,
+        table=table,
+        table_pk=table_pk)
+
 @app.route('/<table>/query/', methods=['GET', 'POST'])
 @require_table
 def table_query(table):
     data = []
     data_description = error = row_count = sql = None
 
     if request.method == 'POST':
         sql = request.form['sql']
+        model_class = dataset[table].model_class
         if 'export_json' in request.form:
-            return export(table, sql, 'json')
+            query = model_class.raw(sql).dicts()
+            return export(table, query, 'json')
         elif 'export_csv' in request.form:
-            return export(table, sql, 'csv')
+            query = model_class.raw(sql).dicts()
+            return export(table, query, 'csv')
 
         try:
             cursor = dataset.query(sql)
         except Exception as exc:
             error = str(exc)
         else:
             data = cursor.fetchall()[:app.config['MAX_RESULT_SIZE']]
@@ -519,39 +760,62 @@
     show = False
     if request.form.get(key) and request.form.get(key) != 'false':
         session[key] = show = True
     elif key in session:
         del session[key]
     return jsonify({key: show})
 
-def export(table, sql, export_format):
-    model_class = dataset[table].model_class
-    query = model_class.raw(sql).dicts()
+def export(table, query, export_format):
     buf = StringIO()
     if export_format == 'json':
         kwargs = {'indent': 2}
         filename = '%s-export.json' % table
         mimetype = 'text/javascript'
     else:
         kwargs = {}
         filename = '%s-export.csv' % table
         mimetype = 'text/csv'
 
+    # Avoid any special chars in export filename.
+    filename = re.sub(r'[^\w\d\-\.]+', '', filename)
+
     dataset.freeze(query, export_format, file_obj=buf, **kwargs)
 
     response_data = buf.getvalue()
     response = make_response(response_data)
     response.headers['Content-Length'] = len(response_data)
     response.headers['Content-Type'] = mimetype
-    response.headers['Content-Disposition'] = 'attachment; filename=%s' % (
+    response.headers['Content-Disposition'] = 'attachment; filename="%s"' % (
         filename)
     response.headers['Expires'] = 0
     response.headers['Pragma'] = 'public'
     return response
 
+@app.route('/<table>/export/', methods=['GET', 'POST'])
+@require_table
+def table_export(table):
+    columns = dataset.get_columns(table)
+    if request.method == 'POST':
+        export_format = request.form.get('export_format') or 'json'
+        col_dict = {c.name: c for c in columns}
+        selected = [c for c in (request.form.getlist('columns') or [])
+                    if c in col_dict]
+        if not selected:
+            flash('Please select one or more columns to export.', 'danger')
+        else:
+            model = dataset[table].model_class
+            fields = [model._meta.columns[c] for c in selected]
+            query = model.select(*fields).dicts()
+            return export(table, query, export_format)
+
+    return render_template(
+        'table_export.html',
+        columns=columns,
+        table=table)
+
 @app.route('/<table>/import/', methods=['GET', 'POST'])
 @require_table
 def table_import(table):
     count = None
     request_data = get_request_data()
     strict = bool(request_data.get('strict'))
 
@@ -624,23 +888,47 @@
     split_regex = re.compile(r'\bon\b', re.I)
     if not split_regex.search(index_sql):
         return index_sql
 
     create, definition = split_regex.split(index_sql)
     return '\nON '.join((create.strip(), definition.strip()))
 
+@app.template_filter('encode_pk')
+def encode_pk(row, pk):
+    if isinstance(pk, CompositeKey):
+        try:
+            return ':::'.join([str(row[k]) for k in pk.field_names])
+        except Exception as exc:
+            return '__uneditable__'
+    return row[pk.column_name]
+
+def decode_pk(model, pk_data):
+    pk = model._meta.primary_key
+    if isinstance(pk, CompositeKey):
+        fields = [pk.model._meta.columns[f] for f in pk.field_names]
+        values = pk_data.split(':::')
+        expressions = [(f == v) for f, v in zip(fields, values)]
+        return reduce(operator.and_, expressions)
+    return (pk == pk_data)
+
+@app.template_filter('pk_display')
+def pk_display(table_pk, pk):
+    if isinstance(table_pk, CompositeKey):
+        return tuple(pk.split(':::'))
+    return pk
+
 @app.template_filter('value_filter')
 def value_filter(value, max_length=50):
     if isinstance(value, numeric):
         return value
 
     if isinstance(value, binary_types):
         if not isinstance(value, (bytes, bytearray)):
             value = bytes(value)  # Handle `buffer` type.
-        value = value.decode('utf-8', decode_handler)
+        value = base64.b64encode(value)[:1024].decode('utf8')
     if isinstance(value, unicode_type):
         value = escape(value)
         if len(value) > max_length:
             return ('<span class="truncated">%s</span> '
                     '<span class="full" style="display:none;">%s</span>'
                     '<a class="toggle-value" href="#">...</a>') % (
                         value[:max_length],
@@ -759,14 +1047,21 @@
     parser.add_option(
         '-r',
         '--read-only',
         action='store_true',
         dest='read_only',
         help='Open database in read-only mode.')
     parser.add_option(
+        '-R',
+        '--rows-per-page',
+        default=50,
+        dest='rows_per_page',
+        help='Number of rows to display per page (default=50)',
+        type='int')
+    parser.add_option(
         '-u',
         '--url-prefix',
         dest='url_prefix',
         help='URL prefix for application.')
     parser.add_option(
         '-e',
         '--extension',
@@ -870,14 +1165,17 @@
                 password = getpass('Enter password: ')
                 password_confirm = getpass('Confirm password: ')
                 if password != password_confirm:
                     print('Passwords did not match!')
                 else:
                     break
 
+    if options.rows_per_page:
+        app.config['ROWS_PER_PAGE'] = options.rows_per_page
+
     # Initialize the dataset instance and (optionally) authentication handler.
     initialize_app(args[0], options.read_only, password, options.url_prefix,
                    options.extensions)
 
     if options.browser:
         open_browser_tab(options.host, options.port)
```

### Comparing `sqlite-web-0.4.1/sqlite_web/static/css/bootstrap.min.css` & `sqlite-web-0.5.0/sqlite_web/static/css/bootstrap.min.css`

 * *Files identical despite different names*

### Comparing `sqlite-web-0.4.1/sqlite_web/static/css/syntax-highlight.css` & `sqlite-web-0.5.0/sqlite_web/static/css/syntax-highlight.css`

 * *Files identical despite different names*

### Comparing `sqlite-web-0.4.1/sqlite_web/static/fonts/glyphicons-halflings-regular.eot` & `sqlite-web-0.5.0/sqlite_web/static/fonts/glyphicons-halflings-regular.eot`

 * *Files identical despite different names*

### Comparing `sqlite-web-0.4.1/sqlite_web/static/fonts/glyphicons-halflings-regular.svg` & `sqlite-web-0.5.0/sqlite_web/static/fonts/glyphicons-halflings-regular.svg`

 * *Files identical despite different names*

### Comparing `sqlite-web-0.4.1/sqlite_web/static/fonts/glyphicons-halflings-regular.ttf` & `sqlite-web-0.5.0/sqlite_web/static/fonts/glyphicons-halflings-regular.ttf`

 * *Files identical despite different names*

### Comparing `sqlite-web-0.4.1/sqlite_web/static/fonts/glyphicons-halflings-regular.woff` & `sqlite-web-0.5.0/sqlite_web/static/fonts/glyphicons-halflings-regular.woff`

 * *Files identical despite different names*

### Comparing `sqlite-web-0.4.1/sqlite_web/static/img/delete.png` & `sqlite-web-0.5.0/sqlite_web/static/img/delete.png`

 * *Files identical despite different names*

### Comparing `sqlite-web-0.4.1/sqlite_web/static/img/expression.png` & `sqlite-web-0.5.0/sqlite_web/static/img/expression.png`

 * *Files identical despite different names*

### Comparing `sqlite-web-0.4.1/sqlite_web/static/img/index-create.png` & `sqlite-web-0.5.0/sqlite_web/static/img/index-create.png`

 * *Files identical despite different names*

### Comparing `sqlite-web-0.4.1/sqlite_web/static/img/index-drop.png` & `sqlite-web-0.5.0/sqlite_web/static/img/index-drop.png`

 * *Files identical despite different names*

### Comparing `sqlite-web-0.4.1/sqlite_web/static/img/insert.png` & `sqlite-web-0.5.0/sqlite_web/static/img/insert.png`

 * *Files identical despite different names*

### Comparing `sqlite-web-0.4.1/sqlite_web/static/img/select-advanced.png` & `sqlite-web-0.5.0/sqlite_web/static/img/select-advanced.png`

 * *Files identical despite different names*

### Comparing `sqlite-web-0.4.1/sqlite_web/static/img/select.png` & `sqlite-web-0.5.0/sqlite_web/static/img/select.png`

 * *Files identical despite different names*

### Comparing `sqlite-web-0.4.1/sqlite_web/static/img/table-alter.png` & `sqlite-web-0.5.0/sqlite_web/static/img/table-alter.png`

 * *Files identical despite different names*

### Comparing `sqlite-web-0.4.1/sqlite_web/static/img/table-create.png` & `sqlite-web-0.5.0/sqlite_web/static/img/table-create.png`

 * *Files identical despite different names*

### Comparing `sqlite-web-0.4.1/sqlite_web/static/img/table-drop.png` & `sqlite-web-0.5.0/sqlite_web/static/img/table-drop.png`

 * *Files identical despite different names*

### Comparing `sqlite-web-0.4.1/sqlite_web/static/img/trigger-create.png` & `sqlite-web-0.5.0/sqlite_web/static/img/trigger-create.png`

 * *Files identical despite different names*

### Comparing `sqlite-web-0.4.1/sqlite_web/static/img/trigger-drop.png` & `sqlite-web-0.5.0/sqlite_web/static/img/trigger-drop.png`

 * *Files identical despite different names*

### Comparing `sqlite-web-0.4.1/sqlite_web/static/img/update.png` & `sqlite-web-0.5.0/sqlite_web/static/img/update.png`

 * *Files identical despite different names*

### Comparing `sqlite-web-0.4.1/sqlite_web/static/img/view-create.png` & `sqlite-web-0.5.0/sqlite_web/static/img/view-create.png`

 * *Files identical despite different names*

### Comparing `sqlite-web-0.4.1/sqlite_web/static/img/view-drop.png` & `sqlite-web-0.5.0/sqlite_web/static/img/view-drop.png`

 * *Files identical despite different names*

### Comparing `sqlite-web-0.4.1/sqlite_web/static/js/bootstrap.bundle.min.js` & `sqlite-web-0.5.0/sqlite_web/static/js/bootstrap.bundle.min.js`

 * *Files identical despite different names*

### Comparing `sqlite-web-0.4.1/sqlite_web/static/js/jquery-1.11.0.min.js` & `sqlite-web-0.5.0/sqlite_web/static/js/jquery-1.11.0.min.js`

 * *Files identical despite different names*

### Comparing `sqlite-web-0.4.1/sqlite_web/templates/add_column.html` & `sqlite-web-0.5.0/sqlite_web/templates/add_column.html`

 * *Files identical despite different names*

### Comparing `sqlite-web-0.4.1/sqlite_web/templates/add_index.html` & `sqlite-web-0.5.0/sqlite_web/templates/add_index.html`

 * *Files identical despite different names*

### Comparing `sqlite-web-0.4.1/sqlite_web/templates/base.html` & `sqlite-web-0.5.0/sqlite_web/templates/base.html`

 * *Files identical despite different names*

### Comparing `sqlite-web-0.4.1/sqlite_web/templates/base_table.html` & `sqlite-web-0.5.0/sqlite_web/templates/base_table.html`

 * *Files 13% similar despite different names*

```diff
@@ -12,21 +12,29 @@
     <li class="nav-item">
       <a class="nav-link{% block content_tab_class %}{% endblock %}" href="{{ url_for('table_content', table=table) }}">Content</a>
     </li>
     <li class="nav-item">
       <a class="nav-link{% block query_tab_class %}{% endblock %}" href="{{ url_for('table_query', table=table) }}">Query</a>
     </li>
     {% if not dataset.is_readonly %}
+    <li class="nav-item">
+      <a class="nav-link{% block insert_tab_class %}{% endblock %}" href="{{ url_for('table_insert', table=table) }}">Insert</a>
+    </li>
+    {% endif %}
+    {% if not dataset.is_readonly %}
     <li class="nav-item ml-auto">
       <a class="nav-link{% block drop_tab_class %}{% endblock %}" href="{{ url_for('drop_table', table=table) }}">Drop</a>
     </li>
     <li class="nav-item">
       <a class="nav-link{% block import_tab_class %}{% endblock %}" href="{{ url_for('table_import', table=table) }}">Import</a>
     </li>
     {% endif %}
+    <li class="nav-item">
+      <a class="nav-link{% block export_tab_class %}{% endblock %}" href="{{ url_for('table_export', table=table) }}">Export</a>
+    </li>
     {% block inner_nav %}{% endblock %}
   </ul>
   <div style="margin-top: 20px;">
     {% block inner_content %}
     {% endblock %}
   </div>
 {% endblock %}
```

#### html2text {}

```diff
@@ -1,11 +1,15 @@
 {% extends "base_tables.html" %} {% block content_title %} {{_dataset.base_name
 }} — {{ table }} {% endblock %} {% block content %}
     * Structure
     * Content
     * Query
     * {% if not dataset.is_readonly %}
+    * Insert
+    * {% endif %} {% if not dataset.is_readonly %}
     * Drop
     * Import
-    * {% endif %} {% block inner_nav %}{% endblock %}
+    * {% endif %}
+    * Export
+    * {% block inner_nav %}{% endblock %}
 {% block inner_content %} {% endblock %}
 {% endblock %}
```

### Comparing `sqlite-web-0.4.1/sqlite_web/templates/base_tables.html` & `sqlite-web-0.5.0/sqlite_web/templates/base_tables.html`

 * *Files identical despite different names*

### Comparing `sqlite-web-0.4.1/sqlite_web/templates/drop_column.html` & `sqlite-web-0.5.0/sqlite_web/templates/drop_column.html`

 * *Files identical despite different names*

### Comparing `sqlite-web-0.4.1/sqlite_web/templates/drop_index.html` & `sqlite-web-0.5.0/sqlite_web/templates/drop_index.html`

 * *Files identical despite different names*

### Comparing `sqlite-web-0.4.1/sqlite_web/templates/drop_table.html` & `sqlite-web-0.5.0/sqlite_web/templates/drop_table.html`

 * *Files identical despite different names*

### Comparing `sqlite-web-0.4.1/sqlite_web/templates/drop_trigger.html` & `sqlite-web-0.5.0/sqlite_web/templates/drop_trigger.html`

 * *Files identical despite different names*

### Comparing `sqlite-web-0.4.1/sqlite_web/templates/index.html` & `sqlite-web-0.5.0/sqlite_web/templates/index.html`

 * *Files identical despite different names*

### Comparing `sqlite-web-0.4.1/sqlite_web/templates/rename_column.html` & `sqlite-web-0.5.0/sqlite_web/templates/rename_column.html`

 * *Files identical despite different names*

### Comparing `sqlite-web-0.4.1/sqlite_web/templates/table_content.html` & `sqlite-web-0.5.0/sqlite_web/templates/table_content.html`

 * *Files 14% similar despite different names*

```diff
@@ -21,37 +21,45 @@
   <small>{{ ds_table.all().count() }} rows, showing page {{ page }}</small>
 {% endblock %}
 
 {% block content_tab_class %} active{% endblock %}
 
 {% block inner_content %}
   {# add filters #}
-  <table class="table table-striped">
+  <table class="table table-striped small">
     <thead>
       <tr>
         {% for column in columns %}
           <th>
             <a href="./?ordering={% if ordering == column %}-{% endif %}{{ column }}">{{ column }}</a>
           </th>
         {% endfor %}
+        {% if not dataset.is_readonly and table_pk %}<th></th>{% endif %}
       </tr>
     </thead>
     <tbody>
       {% for row in query %}
         <tr>
           {% for field in field_names %}
             {% set value = row[field] %}
             <td>
               {% if value is none %}
-                NULL
+                <code>NULL</code>
               {% else %}
                 {{ value|value_filter|safe }}
               {% endif %}
             </td>
           {% endfor %}
+          {% if not dataset.is_readonly and table_pk %}
+            <td>
+              {% set pk = row|encode_pk(table_pk) %}
+              <a class="small" href="{{ url_for('table_update', table=table, pk=pk) }}">Edit</a>
+              <a class="small" href="{{ url_for('table_delete', table=table, pk=pk) }}">Delete</a>
+            </td>
+          {% endif %}
         </tr>
       {% endfor %}
     </tbody>
   </table>
   <nav>
     <ul class="pagination">
       <li class="{% if not previous_page %}disabled {% endif %}page-item">
```

### Comparing `sqlite-web-0.4.1/sqlite_web/templates/table_import.html` & `sqlite-web-0.5.0/sqlite_web/templates/table_import.html`

 * *Files identical despite different names*

### Comparing `sqlite-web-0.4.1/sqlite_web/templates/table_query.html` & `sqlite-web-0.5.0/sqlite_web/templates/table_query.html`

 * *Files 4% similar despite different names*

```diff
@@ -109,28 +109,28 @@
     {% if not data %}
       <p>Empty result set.</p>
     {% else %}
       <a class="float-right" href="{{ url_for('table_query', table=table, sql=sql) }}">Permalink</a>
       <h3>
         Results ({{ data|length }})
       </h3>
-      <table class="table table-striped">
+      <table class="table table-striped small">
         <thead>
           <tr>
             {% for col_desc in data_description %}
               <th>{{ col_desc[0] }}</th>
             {% endfor %}
           </tr>
         </thead>
         <tbody>
           {% for row in data %}
             <tr>
               {% for value in row %}
                 <td>
-                  {% if value is none %}NULL{% else %}{{ value }}{% endif %}
+                  {% if value is none %}<code>NULL</code>{% else %}{{ value|value_filter|safe }}{% endif %}
                 </td>
               {% endfor %}
             </tr>
           {% endfor %}
         </tbody>
       </table>
     {% endif %}
```

### Comparing `sqlite-web-0.4.1/sqlite_web/templates/table_structure.html` & `sqlite-web-0.5.0/sqlite_web/templates/table_structure.html`

 * *Files 13% similar despite different names*

```diff
@@ -39,24 +39,16 @@
       </tr>
     </thead>
     <tbody>
       {% for column in columns %}
         <tr>
           <td><code>{{ column.name }}</code></td>
           <td><code>{{ column.data_type }}</code></td>
-          <td>
-            {% if column.null %}
-              <span class="glyphicon glyphicon-ok"></span>
-            {% endif %}
-          </td>
-          <td>
-            {% if column.primary_key %}
-              <span class="glyphicon glyphicon-ok"></span>
-            {% endif %}
-          </td>
+          <td>{% if column.null %}&check;{% endif %}</td>
+          <td>{% if column.primary_key %}&check;{% endif %}</td>
           <td>
             {% if dataset.is_readonly %}
               <strong>read-only</strong>
             {% else %}
               <a href="{{ url_for('rename_column', table=table, rename=column.name) }}">Rename</a>
               <span class="separator">|</span>
               <a href="{{ url_for('drop_column', table=table, name=column.name) }}">Drop</a>
@@ -116,19 +108,15 @@
               <ul>
                 {% for column in index.columns %}
                   <li><code>{{ column }}</code></li>
                 {% endfor %}
               </ul>
             {% endif %}
           </td>
-          <td>
-            {% if index.unique %}
-              <span class="glyphicon glyphicon-ok"></span>
-            {% endif %}
-          </td>
+          <td>{% if index.unique %}&check;{% endif %}</td>
           <td>
             <a class="view-sql" data-name="{{ index.name }}" href="#">SQL</a>
             <div style="display:none;">{% if index.sql %}{{ index.sql|format_index|highlight }}{% else %}-- no sql found --{% endif %}</div>
           </td>
           <td>
             {% if dataset.is_readonly %}
               <strong>read-only</strong>
```

### Comparing `sqlite-web-0.4.1/sqlite_web.egg-info/SOURCES.txt` & `sqlite-web-0.5.0/sqlite_web.egg-info/SOURCES.txt`

 * *Files 3% similar despite different names*

```diff
@@ -49,10 +49,14 @@
 sqlite_web/templates/drop_index.html
 sqlite_web/templates/drop_table.html
 sqlite_web/templates/drop_trigger.html
 sqlite_web/templates/index.html
 sqlite_web/templates/login.html
 sqlite_web/templates/rename_column.html
 sqlite_web/templates/table_content.html
+sqlite_web/templates/table_delete.html
+sqlite_web/templates/table_export.html
 sqlite_web/templates/table_import.html
+sqlite_web/templates/table_insert.html
 sqlite_web/templates/table_query.html
-sqlite_web/templates/table_structure.html
+sqlite_web/templates/table_structure.html
+sqlite_web/templates/table_update.html
```

