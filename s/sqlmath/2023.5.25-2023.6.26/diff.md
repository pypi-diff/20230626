# Comparing `tmp/sqlmath-2023.5.25.tar.gz` & `tmp/sqlmath-2023.6.26.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sqlmath-2023.5.25.tar", last modified: Thu May 25 20:53:24 2023, max compression
+gzip compressed data, was "sqlmath-2023.6.26.tar", last modified: Mon Jun 26 18:19:42 2023, max compression
```

## Comparing `sqlmath-2023.5.25.tar` & `sqlmath-2023.6.26.tar`

### file list

```diff
@@ -1,49 +1,49 @@
-drwxrwxrwx   0        0        0        0 2023-05-25 20:53:24.706018 sqlmath-2023.5.25/
--rw-rw-rw-   0        0        0    14419 2023-05-19 17:59:37.000000 sqlmath-2023.5.25/.ci.sh
--rw-rw-rw-   0        0        0      649 2023-05-25 18:35:33.000000 sqlmath-2023.5.25/.gitconfig
-drwxrwxrwx   0        0        0        0 2023-05-25 20:53:24.647016 sqlmath-2023.5.25/.github/
-drwxrwxrwx   0        0        0        0 2023-05-25 20:53:24.698018 sqlmath-2023.5.25/.github/workflows/
--rw-rw-rw-   0        0        0     2678 2023-05-25 18:35:33.000000 sqlmath-2023.5.25/.github/workflows/ci.yml
--rw-rw-rw-   0        0        0     1979 2023-05-25 18:35:34.000000 sqlmath-2023.5.25/.github/workflows/publish.yml
--rw-rw-rw-   0        0        0      350 2023-05-25 18:35:34.000000 sqlmath-2023.5.25/.gitignore
--rw-rw-rw-   0        0        0      121 2023-05-16 16:00:43.000000 sqlmath-2023.5.25/.npmignore
--rw-rw-rw-   0        0        0    22045 2023-05-25 18:58:37.000000 sqlmath-2023.5.25/CHANGELOG.md
--rw-rw-rw-   0        0        0     1051 2023-04-27 14:22:07.000000 sqlmath-2023.5.25/LICENSE
--rw-rw-rw-   0        0        0      941 2023-05-25 20:10:06.000000 sqlmath-2023.5.25/MANIFEST.in
--rw-rw-rw-   0        0        0     7332 2023-05-25 20:53:24.705018 sqlmath-2023.5.25/PKG-INFO
--rw-rw-rw-   0        0        0     4920 2023-05-25 20:53:13.000000 sqlmath-2023.5.25/README.md
--rw-rw-rw-   0        0        0      564 2023-05-16 16:00:43.000000 sqlmath-2023.5.25/asset_image_folder_open_solid.svg
--rw-rw-rw-   0        0        0     1536 2023-05-16 16:00:43.000000 sqlmath-2023.5.25/asset_image_github_brands.svg
--rw-rw-rw-   0        0        0     1060 2023-05-16 16:00:43.000000 sqlmath-2023.5.25/asset_image_logo_512.html
--rw-rw-rw-   0        0        0     7087 2023-05-16 16:00:43.000000 sqlmath-2023.5.25/asset_image_logo_512.png
--rw-rw-rw-   0        0        0     2823 2023-05-16 16:00:43.000000 sqlmath-2023.5.25/asset_image_logo_512.svg
--rw-rw-rw-   0        0        0   472927 2023-05-25 17:09:49.000000 sqlmath-2023.5.25/asset_sqlmath_external_rollup.js
--rw-rw-rw-   0        0        0   262193 2023-05-16 16:00:43.000000 sqlmath-2023.5.25/cpplint.py
--rw-rw-rw-   0        0        0   385557 2023-05-16 16:00:43.000000 sqlmath-2023.5.25/csslint.js
--rwxrwxrwx   0        0        0    72704 2023-05-16 16:00:43.000000 sqlmath-2023.5.25/indent.exe
--rw-rw-rw-   0        0        0    23525 2023-05-25 17:09:50.000000 sqlmath-2023.5.25/index.html
--rw-rw-rw-   0        0        0   337350 2023-05-24 18:34:34.000000 sqlmath-2023.5.25/jslint.mjs
--rw-rw-rw-   0        0        0   100564 2023-05-25 18:03:44.000000 sqlmath-2023.5.25/jslint_ci.sh
--rw-rw-rw-   0        0        0  1008128 2023-05-16 16:00:43.000000 sqlmath-2023.5.25/libiconv2.dll
--rw-rw-rw-   0        0        0   103424 2023-05-16 16:00:43.000000 sqlmath-2023.5.25/libintl3.dll
--rw-rw-rw-   0        0        0      920 2023-05-25 17:01:15.000000 sqlmath-2023.5.25/package.json
--rw-rw-rw-   0        0        0     1497 2023-05-25 19:02:01.000000 sqlmath-2023.5.25/pyproject.toml
--rw-rw-rw-   0        0        0       42 2023-05-25 20:53:24.706018 sqlmath-2023.5.25/setup.cfg
--rw-rw-rw-   0        0        0    12581 2023-05-25 20:09:52.000000 sqlmath-2023.5.25/setup.py
--rw-rw-rw-   0        0        0 11372418 2023-05-25 17:09:57.000000 sqlmath-2023.5.25/sqlite_rollup.c
-drwxrwxrwx   0        0        0        0 2023-05-25 20:53:24.700018 sqlmath-2023.5.25/sqlmath/
--rw-rw-rw-   0        0        0      855 2023-05-25 20:41:18.000000 sqlmath-2023.5.25/sqlmath/__init__.py
--rw-rw-rw-   0        0        0   148110 2023-05-25 17:09:58.000000 sqlmath-2023.5.25/sqlmath/sqlmath_dbapi2.py
-drwxrwxrwx   0        0        0        0 2023-05-25 20:53:24.704019 sqlmath-2023.5.25/sqlmath.egg-info/
--rw-rw-rw-   0        0        0     7332 2023-05-25 20:53:24.000000 sqlmath-2023.5.25/sqlmath.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      760 2023-05-25 20:53:24.000000 sqlmath-2023.5.25/sqlmath.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-25 20:53:24.000000 sqlmath-2023.5.25/sqlmath.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        8 2023-05-25 20:53:24.000000 sqlmath-2023.5.25/sqlmath.egg-info/top_level.txt
--rw-rw-rw-   0        0        0    37595 2023-05-25 17:01:15.000000 sqlmath-2023.5.25/sqlmath.mjs
--rw-rw-rw-   0        0        0    75038 2023-05-25 16:56:48.000000 sqlmath-2023.5.25/sqlmath_base.c
--rw-rw-rw-   0        0        0   142223 2023-05-16 16:00:43.000000 sqlmath-2023.5.25/sqlmath_browser.mjs
--rw-rw-rw-   0        0        0     1522 2023-05-16 16:00:43.000000 sqlmath-2023.5.25/sqlmath_custom.c
--rw-rw-rw-   0        0        0      150 2023-05-16 16:00:43.000000 sqlmath-2023.5.25/sqlmath_custom.mjs
--rw-rw-rw-   0        0        0    32647 2023-05-16 16:00:43.000000 sqlmath-2023.5.25/sqlmath_jenks.c
--rw-rw-rw-   0        0        0     7931 2023-05-16 16:00:43.000000 sqlmath-2023.5.25/sqlmath_wrapper_wasm.js
--rw-rw-rw-   0        0        0    50059 2023-05-18 18:57:46.000000 sqlmath-2023.5.25/test.mjs
+drwxrwxrwx   0        0        0        0 2023-06-26 18:19:42.369035 sqlmath-2023.6.26/
+-rw-rw-rw-   0        0        0    14419 2023-05-19 17:59:37.000000 sqlmath-2023.6.26/.ci.sh
+-rw-rw-rw-   0        0        0      649 2023-06-26 18:06:40.000000 sqlmath-2023.6.26/.gitconfig
+drwxrwxrwx   0        0        0        0 2023-06-26 18:19:42.320034 sqlmath-2023.6.26/.github/
+drwxrwxrwx   0        0        0        0 2023-06-26 18:19:42.363037 sqlmath-2023.6.26/.github/workflows/
+-rw-rw-rw-   0        0        0     2678 2023-06-26 18:06:40.000000 sqlmath-2023.6.26/.github/workflows/ci.yml
+-rw-rw-rw-   0        0        0     1979 2023-06-26 18:06:41.000000 sqlmath-2023.6.26/.github/workflows/publish.yml
+-rw-rw-rw-   0        0        0      350 2023-06-26 18:06:41.000000 sqlmath-2023.6.26/.gitignore
+-rw-rw-rw-   0        0        0      121 2023-05-16 16:00:43.000000 sqlmath-2023.6.26/.npmignore
+-rw-rw-rw-   0        0        0    22602 2023-06-26 17:28:16.000000 sqlmath-2023.6.26/CHANGELOG.md
+-rw-rw-rw-   0        0        0     1051 2023-04-27 14:22:07.000000 sqlmath-2023.6.26/LICENSE
+-rw-rw-rw-   0        0        0      941 2023-06-26 17:31:00.000000 sqlmath-2023.6.26/MANIFEST.in
+-rw-rw-rw-   0        0        0     7336 2023-06-26 18:19:42.369035 sqlmath-2023.6.26/PKG-INFO
+-rw-rw-rw-   0        0        0     4924 2023-06-26 17:31:03.000000 sqlmath-2023.6.26/README.md
+-rw-rw-rw-   0        0        0      564 2023-05-16 16:00:43.000000 sqlmath-2023.6.26/asset_image_folder_open_solid.svg
+-rw-rw-rw-   0        0        0     1536 2023-05-16 16:00:43.000000 sqlmath-2023.6.26/asset_image_github_brands.svg
+-rw-rw-rw-   0        0        0     1060 2023-05-16 16:00:43.000000 sqlmath-2023.6.26/asset_image_logo_512.html
+-rw-rw-rw-   0        0        0     7087 2023-05-16 16:00:43.000000 sqlmath-2023.6.26/asset_image_logo_512.png
+-rw-rw-rw-   0        0        0     2823 2023-05-16 16:00:43.000000 sqlmath-2023.6.26/asset_image_logo_512.svg
+-rw-rw-rw-   0        0        0   472927 2023-06-26 17:31:58.000000 sqlmath-2023.6.26/asset_sqlmath_external_rollup.js
+-rw-rw-rw-   0        0        0   262193 2023-05-16 16:00:43.000000 sqlmath-2023.6.26/cpplint.py
+-rw-rw-rw-   0        0        0   385557 2023-05-16 16:00:43.000000 sqlmath-2023.6.26/csslint.js
+-rwxrwxrwx   0        0        0    72704 2023-05-16 16:00:43.000000 sqlmath-2023.6.26/indent.exe
+-rw-rw-rw-   0        0        0    23525 2023-06-26 17:31:59.000000 sqlmath-2023.6.26/index.html
+-rw-rw-rw-   0        0        0   337350 2023-05-24 18:34:34.000000 sqlmath-2023.6.26/jslint.mjs
+-rw-rw-rw-   0        0        0   100564 2023-05-25 18:03:44.000000 sqlmath-2023.6.26/jslint_ci.sh
+-rw-rw-rw-   0        0        0  1008128 2023-05-16 16:00:43.000000 sqlmath-2023.6.26/libiconv2.dll
+-rw-rw-rw-   0        0        0   103424 2023-05-16 16:00:43.000000 sqlmath-2023.6.26/libintl3.dll
+-rw-rw-rw-   0        0        0      920 2023-06-26 17:30:54.000000 sqlmath-2023.6.26/package.json
+-rw-rw-rw-   0        0        0     1497 2023-05-25 19:02:01.000000 sqlmath-2023.6.26/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2023-06-26 18:19:42.369035 sqlmath-2023.6.26/setup.cfg
+-rw-rw-rw-   0        0        0    12790 2023-05-26 16:26:03.000000 sqlmath-2023.6.26/setup.py
+-rw-rw-rw-   0        0        0 11372418 2023-06-26 17:32:05.000000 sqlmath-2023.6.26/sqlite_rollup.c
+drwxrwxrwx   0        0        0        0 2023-06-26 18:19:42.365039 sqlmath-2023.6.26/sqlmath/
+-rw-rw-rw-   0        0        0      855 2023-06-26 17:31:03.000000 sqlmath-2023.6.26/sqlmath/__init__.py
+-rw-rw-rw-   0        0        0   148110 2023-06-26 17:32:07.000000 sqlmath-2023.6.26/sqlmath/sqlmath_dbapi2.py
+drwxrwxrwx   0        0        0        0 2023-06-26 18:19:42.368035 sqlmath-2023.6.26/sqlmath.egg-info/
+-rw-rw-rw-   0        0        0     7336 2023-06-26 18:19:42.000000 sqlmath-2023.6.26/sqlmath.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      760 2023-06-26 18:19:42.000000 sqlmath-2023.6.26/sqlmath.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-26 18:19:42.000000 sqlmath-2023.6.26/sqlmath.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        8 2023-06-26 18:19:42.000000 sqlmath-2023.6.26/sqlmath.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0    37595 2023-06-26 17:30:54.000000 sqlmath-2023.6.26/sqlmath.mjs
+-rw-rw-rw-   0        0        0    92524 2023-06-20 14:29:28.000000 sqlmath-2023.6.26/sqlmath_base.c
+-rw-rw-rw-   0        0        0   142223 2023-05-16 16:00:43.000000 sqlmath-2023.6.26/sqlmath_browser.mjs
+-rw-rw-rw-   0        0        0     1522 2023-05-16 16:00:43.000000 sqlmath-2023.6.26/sqlmath_custom.c
+-rw-rw-rw-   0        0        0      150 2023-05-16 16:00:43.000000 sqlmath-2023.6.26/sqlmath_custom.mjs
+-rw-rw-rw-   0        0        0    32647 2023-05-16 16:00:43.000000 sqlmath-2023.6.26/sqlmath_jenks.c
+-rw-rw-rw-   0        0        0     7931 2023-05-16 16:00:43.000000 sqlmath-2023.6.26/sqlmath_wrapper_wasm.js
+-rw-rw-rw-   0        0        0    73312 2023-06-20 14:29:28.000000 sqlmath-2023.6.26/test.mjs
```

### Comparing `sqlmath-2023.5.25/.ci.sh` & `sqlmath-2023.6.26/.ci.sh`

 * *Files identical despite different names*

### Comparing `sqlmath-2023.5.25/.gitconfig` & `sqlmath-2023.6.26/.gitconfig`

 * *Files identical despite different names*

### Comparing `sqlmath-2023.5.25/.github/workflows/ci.yml` & `sqlmath-2023.6.26/.github/workflows/ci.yml`

 * *Files identical despite different names*

### Comparing `sqlmath-2023.5.25/.github/workflows/publish.yml` & `sqlmath-2023.6.26/.github/workflows/publish.yml`

 * *Files identical despite different names*

### Comparing `sqlmath-2023.5.25/CHANGELOG.md` & `sqlmath-2023.6.26/CHANGELOG.md`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,25 @@
 # Changelog
 
 # Todo
 - none
 
+# v2023.6.26
+- sqlmath - fix broken interpolation in sql-function quantile().
+- sqlmath - Add sql-function win_quantile1(), win_quantile2().
+- sqlmath - Update sql-function win_slr2() to be vectorized.
+- sqlmath - Add sql-function win_ema2().
+- betadog - Add feature xema_xxx into ml model.
+- sqlmath - Add sql-function win_slr().
+- sqlmath - Add sql-function vec_win_slr_updatelast().
+- sqlmath - Add sql-function vec_win_slr().
+- sqlmath - Revamp struct Vector99.
+- sqlmath - Add sql-function vec_concat().
+- sqlmath - Add sql-function castrealornull().
+
 # v2023.5.25
 - ci - auto-update python version
 - jslint - Add grammar for "export async function ...".
 - sqlite - Remove hacky sqlite-extension-function.
 - python - Migrate python-driver from pysqlite3 to cpython.
 - jslint - Add grammar for regexp-named-capture-group and regexp-named-backreference.
 - betadog - Reconcile differences with betadog.
```

### Comparing `sqlmath-2023.5.25/LICENSE` & `sqlmath-2023.6.26/LICENSE`

 * *Files identical despite different names*

### Comparing `sqlmath-2023.5.25/MANIFEST.in` & `sqlmath-2023.6.26/MANIFEST.in`

 * *Files identical despite different names*

### Comparing `sqlmath-2023.5.25/PKG-INFO` & `sqlmath-2023.6.26/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sqlmath
-Version: 2023.5.25
+Version: 2023.6.26
 Summary: sqlite for datascience
 Author: Kai Zhu
 License: Copyright (c) 2021 Kai Zhu
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
         of this software and associated documentation files (the "Software"), to deal
         in the Software without restriction, including without limitation the rights
@@ -44,15 +44,15 @@
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # sqlmath - sqlite for data-science
 
 
 # Status
-| Branch | [master<br>(v2023.5.25)](https://github.com/sqlmath/sqlmath/tree/master) | [beta<br>(Web Demo)](https://github.com/sqlmath/sqlmath/tree/beta) | [alpha<br>(Development)](https://github.com/sqlmath/sqlmath/tree/alpha) |
+| Branch | [master<br>(v2023.6.26)](https://github.com/sqlmath/sqlmath/tree/master) | [beta<br>(Web Demo)](https://github.com/sqlmath/sqlmath/tree/beta) | [alpha<br>(Development)](https://github.com/sqlmath/sqlmath/tree/alpha) |
 |--:|:--:|:--:|:--:|
 | CI | [![ci](https://github.com/sqlmath/sqlmath/actions/workflows/ci.yml/badge.svg?branch=master)](https://github.com/sqlmath/sqlmath/actions?query=branch%3Amaster) | [![ci](https://github.com/sqlmath/sqlmath/actions/workflows/ci.yml/badge.svg?branch=beta)](https://github.com/sqlmath/sqlmath/actions?query=branch%3Abeta) | [![ci](https://github.com/sqlmath/sqlmath/actions/workflows/ci.yml/badge.svg?branch=alpha)](https://github.com/sqlmath/sqlmath/actions?query=branch%3Aalpha) |
 | Coverage | [![coverage](https://sqlmath.github.io/sqlmath/branch-master/.artifact/coverage/coverage_badge.svg)](https://sqlmath.github.io/sqlmath/branch-master/.artifact/coverage/index.html) | [![coverage](https://sqlmath.github.io/sqlmath/branch-beta/.artifact/coverage/coverage_badge.svg)](https://sqlmath.github.io/sqlmath/branch-beta/.artifact/coverage/index.html) | [![coverage](https://sqlmath.github.io/sqlmath/branch-alpha/.artifact/coverage/coverage_badge.svg)](https://sqlmath.github.io/sqlmath/branch-alpha/.artifact/coverage/index.html) |
 | Demo | [<img src="asset_image_github_brands.svg" height="32">](https://sqlmath.github.io/sqlmath/branch-master/index.html) | [<img src="asset_image_github_brands.svg" height="32">](https://sqlmath.github.io/sqlmath/branch-beta/index.html) | [<img src="asset_image_github_brands.svg" height="32">](https://sqlmath.github.io/sqlmath/branch-alpha/index.html) |
 | Artifacts | [<img src="asset_image_folder_open_solid.svg" height="30">](https://github.com/sqlmath/sqlmath/tree/gh-pages/branch-master/.artifact) | [<img src="asset_image_folder_open_solid.svg" height="30">](https://github.com/sqlmath/sqlmath/tree/gh-pages/branch-beta/.artifact) | [<img src="asset_image_folder_open_solid.svg" height="30">](https://github.com/sqlmath/sqlmath/tree/gh-pages/branch-alpha/.artifact) |
 
 
@@ -162,13 +162,13 @@
 
 
 <br><br>
 ### python pypi publish
 ```shell
 python -m build
 #
-twine upload --repository testpypi dist/sqlmath-2023.5.25*
-py -m pip install --index-url https://test.pypi.org/simple/ sqlmath==0.0.5
+twine upload --repository testpypi dist/sqlmath-2023.6.26*
+py -m pip install --index-url https://test.pypi.org/simple/ sqlmath==2023.6.26
 #
-twine upload dist/sqlmath-2023.5.25*
-pip install sqlmath==2023.5.25
+twine upload dist/sqlmath-2023.6.26*
+pip install sqlmath==2023.6.26
 ```
```

### Comparing `sqlmath-2023.5.25/README.md` & `sqlmath-2023.6.26/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 # sqlmath - sqlite for data-science
 
 
 # Status
-| Branch | [master<br>(v2023.5.25)](https://github.com/sqlmath/sqlmath/tree/master) | [beta<br>(Web Demo)](https://github.com/sqlmath/sqlmath/tree/beta) | [alpha<br>(Development)](https://github.com/sqlmath/sqlmath/tree/alpha) |
+| Branch | [master<br>(v2023.6.26)](https://github.com/sqlmath/sqlmath/tree/master) | [beta<br>(Web Demo)](https://github.com/sqlmath/sqlmath/tree/beta) | [alpha<br>(Development)](https://github.com/sqlmath/sqlmath/tree/alpha) |
 |--:|:--:|:--:|:--:|
 | CI | [![ci](https://github.com/sqlmath/sqlmath/actions/workflows/ci.yml/badge.svg?branch=master)](https://github.com/sqlmath/sqlmath/actions?query=branch%3Amaster) | [![ci](https://github.com/sqlmath/sqlmath/actions/workflows/ci.yml/badge.svg?branch=beta)](https://github.com/sqlmath/sqlmath/actions?query=branch%3Abeta) | [![ci](https://github.com/sqlmath/sqlmath/actions/workflows/ci.yml/badge.svg?branch=alpha)](https://github.com/sqlmath/sqlmath/actions?query=branch%3Aalpha) |
 | Coverage | [![coverage](https://sqlmath.github.io/sqlmath/branch-master/.artifact/coverage/coverage_badge.svg)](https://sqlmath.github.io/sqlmath/branch-master/.artifact/coverage/index.html) | [![coverage](https://sqlmath.github.io/sqlmath/branch-beta/.artifact/coverage/coverage_badge.svg)](https://sqlmath.github.io/sqlmath/branch-beta/.artifact/coverage/index.html) | [![coverage](https://sqlmath.github.io/sqlmath/branch-alpha/.artifact/coverage/coverage_badge.svg)](https://sqlmath.github.io/sqlmath/branch-alpha/.artifact/coverage/index.html) |
 | Demo | [<img src="asset_image_github_brands.svg" height="32">](https://sqlmath.github.io/sqlmath/branch-master/index.html) | [<img src="asset_image_github_brands.svg" height="32">](https://sqlmath.github.io/sqlmath/branch-beta/index.html) | [<img src="asset_image_github_brands.svg" height="32">](https://sqlmath.github.io/sqlmath/branch-alpha/index.html) |
 | Artifacts | [<img src="asset_image_folder_open_solid.svg" height="30">](https://github.com/sqlmath/sqlmath/tree/gh-pages/branch-master/.artifact) | [<img src="asset_image_folder_open_solid.svg" height="30">](https://github.com/sqlmath/sqlmath/tree/gh-pages/branch-beta/.artifact) | [<img src="asset_image_folder_open_solid.svg" height="30">](https://github.com/sqlmath/sqlmath/tree/gh-pages/branch-alpha/.artifact) |
 
 
@@ -116,13 +116,13 @@
 
 
 <br><br>
 ### python pypi publish
 ```shell
 python -m build
 #
-twine upload --repository testpypi dist/sqlmath-2023.5.25*
-py -m pip install --index-url https://test.pypi.org/simple/ sqlmath==0.0.5
+twine upload --repository testpypi dist/sqlmath-2023.6.26*
+py -m pip install --index-url https://test.pypi.org/simple/ sqlmath==2023.6.26
 #
-twine upload dist/sqlmath-2023.5.25*
-pip install sqlmath==2023.5.25
+twine upload dist/sqlmath-2023.6.26*
+pip install sqlmath==2023.6.26
 ```
```

### Comparing `sqlmath-2023.5.25/asset_image_folder_open_solid.svg` & `sqlmath-2023.6.26/asset_image_folder_open_solid.svg`

 * *Files identical despite different names*

### Comparing `sqlmath-2023.5.25/asset_image_github_brands.svg` & `sqlmath-2023.6.26/asset_image_github_brands.svg`

 * *Files identical despite different names*

### Comparing `sqlmath-2023.5.25/asset_image_logo_512.html` & `sqlmath-2023.6.26/asset_image_logo_512.html`

 * *Files identical despite different names*

### Comparing `sqlmath-2023.5.25/asset_image_logo_512.png` & `sqlmath-2023.6.26/asset_image_logo_512.png`

 * *Files identical despite different names*

### Comparing `sqlmath-2023.5.25/asset_image_logo_512.svg` & `sqlmath-2023.6.26/asset_image_logo_512.svg`

 * *Files identical despite different names*

### Comparing `sqlmath-2023.5.25/asset_sqlmath_external_rollup.js` & `sqlmath-2023.6.26/asset_sqlmath_external_rollup.js`

 * *Files identical despite different names*

### Comparing `sqlmath-2023.5.25/cpplint.py` & `sqlmath-2023.6.26/cpplint.py`

 * *Files identical despite different names*

### Comparing `sqlmath-2023.5.25/csslint.js` & `sqlmath-2023.6.26/csslint.js`

 * *Files identical despite different names*

### Comparing `sqlmath-2023.5.25/indent.exe` & `sqlmath-2023.6.26/indent.exe`

 * *Files identical despite different names*

### Comparing `sqlmath-2023.5.25/index.html` & `sqlmath-2023.6.26/index.html`

 * *Files identical despite different names*

### Comparing `sqlmath-2023.5.25/jslint.mjs` & `sqlmath-2023.6.26/jslint.mjs`

 * *Files identical despite different names*

### Comparing `sqlmath-2023.5.25/jslint_ci.sh` & `sqlmath-2023.6.26/jslint_ci.sh`

 * *Files identical despite different names*

### Comparing `sqlmath-2023.5.25/libiconv2.dll` & `sqlmath-2023.6.26/libiconv2.dll`

 * *Files identical despite different names*

### Comparing `sqlmath-2023.5.25/libintl3.dll` & `sqlmath-2023.6.26/libintl3.dll`

 * *Files identical despite different names*

### Comparing `sqlmath-2023.5.25/package.json` & `sqlmath-2023.6.26/package.json`

 * *Files 1% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9705882352941176%*

 * *Differences: {"'version'": "'2023.6.26'"}*

```diff
@@ -34,9 +34,9 @@
     "scripts": {
         "build": "sh jslint_ci.sh shCiBuildNodejs",
         "test": "sh jslint_ci.sh shCiTestNodejs",
         "test2": "sh jslint_ci.sh shCiBase"
     },
     "shCiArtifactUpload": 1,
     "shCiNpmPublish": 1,
-    "version": "2023.5.25"
+    "version": "2023.6.26"
 }
```

### Comparing `sqlmath-2023.5.25/pyproject.toml` & `sqlmath-2023.6.26/pyproject.toml`

 * *Files identical despite different names*

### Comparing `sqlmath-2023.5.25/setup.py` & `sqlmath-2023.6.26/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -82,16 +82,22 @@
             *arg_list,
             env=env,
             stdout=subprocess.DEVNULL if npm_config_mode_debug else None,
         )
 
     async def build_ext_obj(cdefine):
         file_obj = f"build/{cdefine}.obj"
-        if cdefine != "SRC_SQLITE_PYTHON" and pathlib.Path(file_obj).exists():
-            return
+        match cdefine:
+            case "SQLMATH_BASE":
+                pass
+            case "SRC_SQLITE_PYTHON":
+                pass
+            case _:
+                if pathlib.Path(file_obj).exists():
+                    return
         file_src = f"build/{cdefine}.c"
         arg_list = [
             *[f"-I{path}" for path in path_include],
             #
             f"-D{cdefine}_C2=",
             "-DSRC_SQLITE_BASE_C2=",
             "-D_REENTRANT=1",
@@ -145,15 +151,16 @@
         child = await asyncio.create_subprocess_exec(*args, **kwds)
         await child.communicate()
         if child.returncode != 0:
             raise subprocess.SubprocessError("returncode=" + child.returncode)
     #
     # build_ext - update version
     with pathlib.Path("package.json").open() as file1:
-        version = json.load(file1)["version"].split("-")[0]
+        package_json = json.load(file1)
+        version = package_json["version"].split("-")[0]
     for filename in [
         "README.md",
         "sqlmath/__init__.py",
     ]:
         with pathlib.Path(filename).open("r+", newline="\n") as file1:
             data0 = file1.read()
             data1 = data0
@@ -174,15 +181,15 @@
                 (
                     '__version_info__ = ("'
                     + '", "'.join(version.split("."))
                     + '")'
                 ),
                 data1,
             )
-            if (data1 != data0):
+            if package_json["name"] == "sqlmath" and data1 != data0:
                 print(f"build_ext - update file {file1.name}")
                 file1.seek(0)
                 file1.write(data1)
                 file1.truncate()
     #
     # build_ext - init sysconfig
     cc_ccshared = sysconfig.get_config_var("CCSHARED") or ""
```

### Comparing `sqlmath-2023.5.25/sqlite_rollup.c` & `sqlmath-2023.6.26/sqlite_rollup.c`

 * *Files 0% similar despite different names*

```diff
@@ -916,17 +916,17 @@
 00003930: 2020 207b 0a20 2020 2020 2020 2020 2020     {.           
 00003940: 2022 636f 6d6d 656e 7422 3a20 7472 7565   "comment": true
 00003950: 2c0a 2020 2020 2020 2020 2020 2020 2268  ,.            "h
 00003960: 6561 6465 7222 3a20 225c 6e23 6966 2064  eader": "\n#if d
 00003970: 6566 696e 6564 2853 514c 4d41 5448 5f4e  efined(SQLMATH_N
 00003980: 4f44 454a 535f 4332 2920 2626 2021 6465  ODEJS_C2) && !de
 00003990: 6669 6e65 6428 5351 4c4d 4154 485f 4e4f  fined(SQLMATH_NO
-000039a0: 4445 4a53 5f43 3329 5c6e 2364 6566 696e  DEJS_C3)\n#defin
+000039a0: 4445 4a53 5f48 3329 5c6e 2364 6566 696e  DEJS_H3)\n#defin
 000039b0: 6520 5351 4c4d 4154 485f 4e4f 4445 4a53  e SQLMATH_NODEJS
-000039c0: 5f43 335c 6e22 2c0a 2020 2020 2020 2020  _C3\n",.        
+000039c0: 5f48 335c 6e22 2c0a 2020 2020 2020 2020  _H3\n",.        
 000039d0: 2020 2020 2275 726c 223a 2022 6874 7470      "url": "http
 000039e0: 733a 2f2f 6769 7468 7562 2e63 6f6d 2f6e  s://github.com/n
 000039f0: 6f64 656a 732f 6e6f 6465 2f62 6c6f 622f  odejs/node/blob/
 00003a00: 7631 302e 3232 2e31 2f4c 4943 454e 5345  v10.22.1/LICENSE
 00003a10: 220a 2020 2020 2020 2020 7d2c 0a20 2020  ".        },.   
 00003a20: 2020 2020 207b 0a20 2020 2020 2020 2020       {.         
 00003a30: 2020 2022 7572 6c22 3a20 2268 7474 7073     "url": "https
@@ -934,15 +934,15 @@
 00003a50: 6465 6a73 2f6e 6f64 652f 626c 6f62 2f76  dejs/node/blob/v
 00003a60: 3130 2e32 322e 312f 7372 632f 6e6f 6465  10.22.1/src/node
 00003a70: 5f61 7069 5f74 7970 6573 2e68 220a 2020  _api_types.h".  
 00003a80: 2020 2020 2020 7d2c 0a20 2020 2020 2020        },.       
 00003a90: 207b 0a20 2020 2020 2020 2020 2020 2022   {.            "
 00003aa0: 666f 6f74 6572 223a 2022 5c6e 2365 6e64  footer": "\n#end
 00003ab0: 6966 202f 2f20 5351 4c4d 4154 485f 4e4f  if // SQLMATH_NO
-00003ac0: 4445 4a53 5f43 335c 6e22 2c0a 2020 2020  DEJS_C3\n",.    
+00003ac0: 4445 4a53 5f48 335c 6e22 2c0a 2020 2020  DEJS_H3\n",.    
 00003ad0: 2020 2020 2020 2020 2272 6570 6c61 6365          "replace
 00003ae0: 4c69 7374 223a 205b 0a20 2020 2020 2020  List": [.       
 00003af0: 2020 2020 2020 2020 207b 0a20 2020 2020           {.     
 00003b00: 2020 2020 2020 2020 2020 2020 2020 2022                 "
 00003b10: 6161 223a 2022 5e23 696e 636c 7564 6520  aa": "^#include 
 00003b20: 5c22 6e6f 6465 5f61 7069 5f74 7970 6573  \"node_api_types
 00003b30: 2e68 5c22 222c 0a20 2020 2020 2020 2020  .h\"",.         
@@ -703651,16 +703651,16 @@
 00abca20: 6874 7470 733a 2f2f 6769 7468 7562 2e63  https://github.c
 00abca30: 6f6d 2f6e 6f64 656a 732f 6e6f 6465 2f62  om/nodejs/node/b
 00abca40: 6c6f 622f 7631 302e 3232 2e31 2f4c 4943  lob/v10.22.1/LIC
 00abca50: 454e 5345 0a2a 2f0a 0a23 6966 2064 6566  ENSE.*/..#if def
 00abca60: 696e 6564 2853 514c 4d41 5448 5f4e 4f44  ined(SQLMATH_NOD
 00abca70: 454a 535f 4332 2920 2626 2021 6465 6669  EJS_C2) && !defi
 00abca80: 6e65 6428 5351 4c4d 4154 485f 4e4f 4445  ned(SQLMATH_NODE
-00abca90: 4a53 5f43 3329 0a23 6465 6669 6e65 2053  JS_C3).#define S
-00abcaa0: 514c 4d41 5448 5f4e 4f44 454a 535f 4333  QLMATH_NODEJS_C3
+00abca90: 4a53 5f48 3329 0a23 6465 6669 6e65 2053  JS_H3).#define S
+00abcaa0: 514c 4d41 5448 5f4e 4f44 454a 535f 4833  QLMATH_NODEJS_H3
 00abcab0: 0a2f 2a0a 4e6f 6465 2e6a 7320 6973 206c  ./*.Node.js is l
 00abcac0: 6963 656e 7365 6420 666f 7220 7573 6520  icensed for use 
 00abcad0: 6173 2066 6f6c 6c6f 7773 3a0a 0a22 2222  as follows:.."""
 00abcae0: 0a43 6f70 7972 6967 6874 204e 6f64 652e  .Copyright Node.
 00abcaf0: 6a73 2063 6f6e 7472 6962 7574 6f72 732e  js contributors.
 00abcb00: 2041 6c6c 2072 6967 6874 7320 7265 7365   All rights rese
 00abcb10: 7276 6564 2e0a 0a50 6572 6d69 7373 696f  rved...Permissio
@@ -710601,15 +710601,15 @@
 00ad7c80: 2020 2020 2020 2020 626f 6f6c 2a20 7265          bool* re
 00ad7c90: 7375 6c74 293b 0a23 656e 6469 6620 202f  sult);.#endif  /
 00ad7ca0: 2f20 4e41 5049 5f45 5850 4552 494d 454e  / NAPI_EXPERIMEN
 00ad7cb0: 5441 4c0a 0a45 5854 4552 4e5f 435f 454e  TAL..EXTERN_C_EN
 00ad7cc0: 440a 0a23 656e 6469 6620 202f 2f20 5352  D..#endif  // SR
 00ad7cd0: 435f 4e4f 4445 5f41 5049 5f48 5f0a 2365  C_NODE_API_H_.#e
 00ad7ce0: 6e64 6966 202f 2f20 5351 4c4d 4154 485f  ndif // SQLMATH_
-00ad7cf0: 4e4f 4445 4a53 5f43 330a 0a0a 2f2a 0a66  NODEJS_C3.../*.f
+00ad7cf0: 4e4f 4445 4a53 5f48 330a 0a0a 2f2a 0a66  NODEJS_H3.../*.f
 00ad7d00: 696c 6520 6e6f 6e65 0a2a 2f0a 2f2a 6a73  ile none.*/./*js
 00ad7d10: 6c69 6e74 2d65 6e61 626c 652a 2f0a 0a0a  lint-enable*/...
 00ad7d20: 2f2f 202a 494e 4445 4e54 2d4f 4e2a 0a0a  // *INDENT-ON*..
 00ad7d30: 0a23 6966 2064 6566 696e 6564 2853 5243  .#if defined(SRC
 00ad7d40: 5f53 514c 4954 455f 4241 5345 5f43 3229  _SQLITE_BASE_C2)
 00ad7d50: 2026 2620 2164 6566 696e 6564 2853 5243   && !defined(SRC
 00ad7d60: 5f53 514c 4954 455f 4241 5345 5f43 3429  _SQLITE_BASE_C4)
```

### Comparing `sqlmath-2023.5.25/sqlmath/__init__.py` & `sqlmath-2023.6.26/sqlmath/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 """sqlmath.py."""
 
-__version__ = "2023.5.25"
-__version_info__ = ("2023", "5", "25")
+__version__ = "2023.6.26"
+__version_info__ = ("2023", "6", "26")
 
 import sys
 
 from .sqlmath_dbapi2 import *  # noqa=F403
 
 
 def debugInline(*argv): # noqa=N802
```

### Comparing `sqlmath-2023.5.25/sqlmath/sqlmath_dbapi2.py` & `sqlmath-2023.6.26/sqlmath/sqlmath_dbapi2.py`

 * *Files identical despite different names*

### Comparing `sqlmath-2023.5.25/sqlmath.egg-info/PKG-INFO` & `sqlmath-2023.6.26/sqlmath.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sqlmath
-Version: 2023.5.25
+Version: 2023.6.26
 Summary: sqlite for datascience
 Author: Kai Zhu
 License: Copyright (c) 2021 Kai Zhu
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
         of this software and associated documentation files (the "Software"), to deal
         in the Software without restriction, including without limitation the rights
@@ -44,15 +44,15 @@
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # sqlmath - sqlite for data-science
 
 
 # Status
-| Branch | [master<br>(v2023.5.25)](https://github.com/sqlmath/sqlmath/tree/master) | [beta<br>(Web Demo)](https://github.com/sqlmath/sqlmath/tree/beta) | [alpha<br>(Development)](https://github.com/sqlmath/sqlmath/tree/alpha) |
+| Branch | [master<br>(v2023.6.26)](https://github.com/sqlmath/sqlmath/tree/master) | [beta<br>(Web Demo)](https://github.com/sqlmath/sqlmath/tree/beta) | [alpha<br>(Development)](https://github.com/sqlmath/sqlmath/tree/alpha) |
 |--:|:--:|:--:|:--:|
 | CI | [![ci](https://github.com/sqlmath/sqlmath/actions/workflows/ci.yml/badge.svg?branch=master)](https://github.com/sqlmath/sqlmath/actions?query=branch%3Amaster) | [![ci](https://github.com/sqlmath/sqlmath/actions/workflows/ci.yml/badge.svg?branch=beta)](https://github.com/sqlmath/sqlmath/actions?query=branch%3Abeta) | [![ci](https://github.com/sqlmath/sqlmath/actions/workflows/ci.yml/badge.svg?branch=alpha)](https://github.com/sqlmath/sqlmath/actions?query=branch%3Aalpha) |
 | Coverage | [![coverage](https://sqlmath.github.io/sqlmath/branch-master/.artifact/coverage/coverage_badge.svg)](https://sqlmath.github.io/sqlmath/branch-master/.artifact/coverage/index.html) | [![coverage](https://sqlmath.github.io/sqlmath/branch-beta/.artifact/coverage/coverage_badge.svg)](https://sqlmath.github.io/sqlmath/branch-beta/.artifact/coverage/index.html) | [![coverage](https://sqlmath.github.io/sqlmath/branch-alpha/.artifact/coverage/coverage_badge.svg)](https://sqlmath.github.io/sqlmath/branch-alpha/.artifact/coverage/index.html) |
 | Demo | [<img src="asset_image_github_brands.svg" height="32">](https://sqlmath.github.io/sqlmath/branch-master/index.html) | [<img src="asset_image_github_brands.svg" height="32">](https://sqlmath.github.io/sqlmath/branch-beta/index.html) | [<img src="asset_image_github_brands.svg" height="32">](https://sqlmath.github.io/sqlmath/branch-alpha/index.html) |
 | Artifacts | [<img src="asset_image_folder_open_solid.svg" height="30">](https://github.com/sqlmath/sqlmath/tree/gh-pages/branch-master/.artifact) | [<img src="asset_image_folder_open_solid.svg" height="30">](https://github.com/sqlmath/sqlmath/tree/gh-pages/branch-beta/.artifact) | [<img src="asset_image_folder_open_solid.svg" height="30">](https://github.com/sqlmath/sqlmath/tree/gh-pages/branch-alpha/.artifact) |
 
 
@@ -162,13 +162,13 @@
 
 
 <br><br>
 ### python pypi publish
 ```shell
 python -m build
 #
-twine upload --repository testpypi dist/sqlmath-2023.5.25*
-py -m pip install --index-url https://test.pypi.org/simple/ sqlmath==0.0.5
+twine upload --repository testpypi dist/sqlmath-2023.6.26*
+py -m pip install --index-url https://test.pypi.org/simple/ sqlmath==2023.6.26
 #
-twine upload dist/sqlmath-2023.5.25*
-pip install sqlmath==2023.5.25
+twine upload dist/sqlmath-2023.6.26*
+pip install sqlmath==2023.6.26
 ```
```

### Comparing `sqlmath-2023.5.25/sqlmath.egg-info/SOURCES.txt` & `sqlmath-2023.6.26/sqlmath.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `sqlmath-2023.5.25/sqlmath.mjs` & `sqlmath-2023.6.26/sqlmath.mjs`

 * *Files 0% similar despite different names*

```diff
@@ -93,15 +93,15 @@
     npm_config_mode_debug,
     npm_config_mode_setup,
     npm_config_mode_test
 } = typeof process === "object" && process?.env;
 let sqlMessageDict = {}; // dict of web-worker-callbacks
 let sqlMessageId = 0;
 let sqlWorker;
-let version = "v2023.5.25";
+let version = "v2023.6.26";
 
 function assertJsonEqual(aa, bb, message) {
 
 // This function will assert JSON.stringify(<aa>) === JSON.stringify(<bb>).
 
     aa = JSON.stringify(objectDeepCopyWithKeysSorted(aa), undefined, 1);
     bb = JSON.stringify(objectDeepCopyWithKeysSorted(bb), undefined, 1);
```

### Comparing `sqlmath-2023.5.25/sqlmath_base.c` & `sqlmath-2023.6.26/sqlmath_base.c`

 * *Files 18% similar despite different names*

```diff
@@ -84,15 +84,15 @@
 #define SQLITE_ERROR_DATATYPE_INVALID   0x10003
 #define SQLITE_ERROR_JSON_ARRAY_INVALID         0x71
 #define SQLITE_ERROR_ZSQL_NULL          0x10004
 #define SQLITE_MAX_LENGTH2 1000000000
 #define SQLITE_RESPONSETYPE_LASTBLOB 1
 #define SQLMATH_API
 #define SQLMATH_FUNC
-#define SWAP(aa, bb) tmp = (aa); (aa) = (bb); (bb) = tmp
+#define SWAP(aa, bb, tmp) tmp = (aa); (aa) = (bb); (bb) = tmp
 #define UNUSED_PARAMETER(x) ((void)(x))
 
 
 // This function will exec <sql> and if <errcode> is not ok,
 // throw <baton>->errmsg with given sqlite-<errcode>.
 #define JSBATON_ASSERT_OK() \
     if (errcode != SQLITE_OK) { \
@@ -128,90 +128,147 @@
         UNUSED_PARAMETER(env); \
         func((Jsbaton *) data); \
     } \
     static napi_value _##func(napi_env env, napi_callback_info info) { \
         return jspromiseCreate(env, info, __##napi##_##func); \
     } \
 
+#define SQLITE3_AGGREGATE_CONTEXT(type) \
+    type *agg = (type *) sqlite3_aggregate_context(context, sizeof(*agg)); \
+    if (agg == NULL) { \
+        sqlite3_result_error_nomem(context); \
+        goto catch_error; \
+    }
+
 #define SQLITE3_CREATE_FUNCTION1(func, argc) \
     errcode = sqlite3_create_function(db, #func, argc, \
         SQLITE_DETERMINISTIC | SQLITE_DIRECTONLY | SQLITE_UTF8, NULL, \
-        sql_##func##_func, NULL, NULL); \
+        sql1_##func##_func, NULL, NULL); \
     if (errcode != SQLITE_OK) { return errcode; }
 
 #define SQLITE3_CREATE_FUNCTION2(func, argc) \
     errcode = sqlite3_create_function(db, #func, argc, \
         SQLITE_DETERMINISTIC | SQLITE_DIRECTONLY | SQLITE_UTF8, NULL, \
-        NULL, sql_##func##_step, sql_##func##_final); \
+        NULL, sql2_##func##_step, sql2_##func##_final); \
     if (errcode != SQLITE_OK) { return errcode; }
 
 #define SQLITE3_CREATE_FUNCTION3(func, argc) \
     errcode = sqlite3_create_window_function(db, #func, argc, \
         SQLITE_DETERMINISTIC | SQLITE_DIRECTONLY | SQLITE_UTF8, NULL, \
-        sql_##func##_step, sql_##func##_final, \
-        sql_##func##_value, sql_##func##_inverse, NULL); \
+        sql3_##func##_step, sql3_##func##_final, \
+        sql3_##func##_value, sql3_##func##_inverse, NULL); \
     if (errcode != SQLITE_OK) { return errcode; }
 
 #define SQLITE3_RESULT_ERROR_CODE(errcode) \
     if (errcode) { \
         sqlite3_result_error_code(context, errcode); \
         goto catch_error; \
     }
 
-#define SQLITE3_RESULT_ERROR_MALLOC(pp) \
-    if (pp == NULL) { \
-        sqlite3_result_error_nomem(context); \
-        goto catch_error; \
-    }
+#define SQLITE3_RESULT_JSONFLOAT64ARRAY(str99, arr, nn) \
+    STR99_ALLOCA(str99); \
+    str99JsonAppendFloat64array(str99, arr, nn); \
+    STR99_RESULT_ERROR(str99); \
+    str99ResultText(str99, context);
 
 #define STR99_ALLOCA(str99) \
     sqlite3_str __##str99 = { 0 }; \
     sqlite3_str *str99 = &__##str99; \
     str99->mxAlloc = SQLITE_MAX_LENGTH2; \
 
 #define STR99_RESULT_ERROR(str99) \
     errcode = sqlite3_str_errcode(str99); \
     if (errcode == SQLITE_ERROR_JSON_ARRAY_INVALID) { \
         sqlite3_str_reset(str99); \
         sqlite3_result_error(context, \
-            "str99ArrayAppendJsonarray() - invalid JSON array", \
-            SQLITE_ERROR_JSON_ARRAY_INVALID); \
+            "str99ArrayAppendJsonarray() - invalid JSON array", -1); \
         goto catch_error; \
     } \
     if (errcode) { \
         sqlite3_str_reset(str99); \
         sqlite3_result_error_code(context, errcode); \
         goto catch_error; \
     } \
     if (sqlite3_str_length(str99) <= 0) { \
         sqlite3_str_reset(str99); \
         sqlite3_result_null(context); \
         goto catch_error; \
     }
 
-#define VECTOR99_AGGREGATE_CONTEXT() \
-    Vector99 *vec99 = \
-        (Vector99 *) sqlite3_aggregate_context(context, sizeof(*vec99)); \
-    if (vec99 == NULL) { \
+#define VECTOR99_AGGREGATE_CONTEXT(nhead) \
+    Vector99 **vec99_agg = \
+        (Vector99 **) sqlite3_aggregate_context(context, sizeof(*vec99_agg)); \
+    if (vec99_agg == NULL) { \
         sqlite3_result_error_nomem(context); \
         return; \
     } \
-    if (vec99->buf == NULL && vector99_buf_malloc(vec99)) { \
-        sqlite3_result_error_nomem(context); \
-        return; \
-    }
+    Vector99 *vec99 = *vec99_agg; \
+    if (vec99 == NULL) { \
+        vec99 = vector99_malloc(nhead); \
+        if (vec99 == NULL) { \
+            sqlite3_result_error_nomem(context); \
+            return; \
+        } \
+        *vec99_agg = vec99; \
+    } \
+    double *vec99_body = vector99_body(vec99); \
+    double *vec99_head = vector99_head(vec99); \
+    UNUSED_PARAMETER(vec99_body); \
+    UNUSED_PARAMETER(vec99_head);
+
+#define VECTOR99_AGGREGATE_PUSH(xx) \
+    errcode = vector99_push(vec99_agg, xx); \
+    SQLITE3_RESULT_ERROR_CODE(errcode); \
+    vec99 = *vec99_agg; \
+    vec99_body = vector99_body(vec99); \
+    vec99_head = vector99_head(vec99);
 
 // file sqlmath_h - sqlite3
 // *INDENT-OFF*
 SQLITE_API const sqlite3_api_routines *sqlite3ApiGet();
 typedef uint32_t u32;
 typedef uint64_t u64;
 typedef uint8_t u8;
 
 
+// file sqlmath_h - db
+typedef struct Jsbaton {
+    int32_t nallc;              // offset - 0-4
+    int32_t nused;              // offset - 4-8
+    int64_t argv[JSBATON_ARGC]; // offset - 8-136
+    int64_t bufv[JSBATON_ARGC]; // offset - 136-264
+    int64_t cfuncname;          // offset - 264-272
+    char errmsg[SIZEOF_MESSAGE_DEFAULT];        // offset 272-528
+    void *napi_argv;
+    void *napi_work;
+    void *napi_deferred;
+} Jsbaton;
+SQLMATH_API int __dbFileImportOrExport(
+    sqlite3 * pInMemory,
+    char *zFilename,
+    const int isSave
+);
+SQLMATH_API void dbClose(
+    Jsbaton * baton
+);
+SQLMATH_API void dbExec(
+    Jsbaton * baton
+);
+SQLMATH_API void dbFileImportOrExport(
+    Jsbaton * baton
+);
+SQLMATH_API void dbNoop(
+    Jsbaton * baton
+);
+SQLMATH_API void dbOpen(
+    Jsbaton * baton
+);
+
+
+
 // file sqlmath_h - str99
 /*
 ** An objected used to accumulate the text of a string where we
 ** do not necessarily know how big the string will be in the end.
 */
 struct sqlite3_str {
   sqlite3 *db;         /* Optional database for lookaside.  Can be NULL */
@@ -226,15 +283,15 @@
 SQLITE_API void str99JsonAppendText(
     sqlite3_str * str99,
     const char *zIn,
     u32 nn
 );
 SQLMATH_API void str99ArrayAppendDouble(
     sqlite3_str * str99,
-    const double val
+    const double xx
 );
 SQLMATH_API void str99ArrayAppendJsonarray(
     sqlite3_str * str99,
     const char *json,
     int nn
 );
 SQLMATH_API void str99JsonAppendFloat64array(
@@ -244,115 +301,75 @@
 );
 SQLMATH_API void str99JsonAppendJenks(
     sqlite3_str * str99,
     int kk,
     const double *arr,
     int nn
 );
-SQLMATH_API void str99JsonAppendText(
-    sqlite3_str * str99,
-    const char *zIn,
-    u32 nn
-);
 SQLMATH_API void str99ResultBlob(
     sqlite3_str * str99,
     sqlite3_context * context
 );
 SQLMATH_API void str99ResultText(
     sqlite3_str * str99,
     sqlite3_context * context
 );
 
 
-// file sqlmath_h - Vector99
+// file sqlmath_h - vector99
 typedef struct Vector99 {
-    double *buf;
-    int alloc;
-    int size;
-    double arg0;
-    double arg1;
+    double alloc;               // allocated size in bytes
+    double nbody;               // number of body elements
+    double nhead;               // number of head elements
+    //
+    double ncol;                // number of columns
+    double wii;                 // counter of window elements
+    double wnn;                 // number of window elements
 } Vector99;
-SQLMATH_API void vector99_buf_free(
-    Vector99 * vec99
+SQLMATH_API void vector99_agg_free(
+    Vector99 ** vec99_agg
 );
-SQLMATH_API int vector99_buf_malloc(
-    Vector99 * vec99
+SQLMATH_API double *vector99_body(
+    const Vector99 * vec99
 );
-SQLMATH_API int vector99_nomem(
+SQLMATH_API double *vector99_head(
     const Vector99 * vec99
 );
-SQLMATH_API double vector99_pop_front(
-    Vector99 * vec99
+SQLMATH_API Vector99 *vector99_malloc(
+    const int nhead
 );
-SQLMATH_API int vector99_push_back(
-    Vector99 * vec99,
-    double val
+SQLMATH_API int vector99_push(
+    Vector99 ** vec99_agg,
+    double xx
 );
 SQLMATH_API void vector99_result_blob(
     Vector99 * vec99,
     sqlite3_context * context
 );
-
-
-// file sqlmath_h - Jsbaton
-typedef struct Jsbaton {
-    int32_t nallc;              // offset - 0-4
-    int32_t nused;              // offset - 4-8
-    int64_t argv[JSBATON_ARGC]; // offset - 8-136
-    int64_t bufv[JSBATON_ARGC]; // offset - 136-264
-    int64_t cfuncname;          // offset - 264-272
-    char errmsg[SIZEOF_MESSAGE_DEFAULT];        // offset 272-528
-    void *napi_argv;
-    void *napi_work;
-    void *napi_deferred;
-} Jsbaton;
-
-
-// file sqlmath_h - SQLMATH_API
-SQLMATH_API int __dbFileImportOrExport(
-    sqlite3 * pInMemory,
-    char *zFilename,
-    const int isSave
-);
-
-SQLMATH_API void dbClose(
-    Jsbaton * baton
-);
-
-SQLMATH_API void dbExec(
-    Jsbaton * baton
-);
-
-SQLMATH_API void dbFileImportOrExport(
-    Jsbaton * baton
+SQLMATH_API int vector99_valid(
+    const Vector99 * vec99
 );
 
-SQLMATH_API void dbNoop(
-    Jsbaton * baton
-);
 
-SQLMATH_API void dbOpen(
-    Jsbaton * baton
+// file sqlmath_h - SQLMATH_API
+SQLMATH_API double *jenksCreate(
+    int kk,
+    const double *values,
+    int nn
 );
 
 SQLMATH_API int doubleSign(
     const double aa
 );
 
 SQLMATH_API int doubleSortCompare(
     const void *aa,
     const void *bb
 );
 
-SQLMATH_API double *jenksCreate(
-    int kk,
-    const double *values,
-    int nn
-);
-
 SQLMATH_API const char *jsbatonValueErrmsg(
     Jsbaton * baton
 );
 
 SQLMATH_API const char *jsbatonValueStringArgi(
     Jsbaton * baton,
     int argi
@@ -369,15 +386,20 @@
 SQLMATH_API double quantile(
     double *arr,
     const int nn,
     const double pp
 );
 
 SQLMATH_API double sqlite3_value_double_or_nan(
-    sqlite3_value * argv
+    sqlite3_value * arg
+);
+
+SQLMATH_API double sqlite3_value_double_or_prev(
+    sqlite3_value * arg,
+    double *previous
 );
 
 SQLMATH_API const char *sqlmathSnprintfTrace(
     char *buf,
     const char *prefix,
     const char *errmsg,
     const char *func,
@@ -396,25 +418,21 @@
 file sqlmath_base - start
 */
 #if defined(SQLMATH_BASE_C2) && !defined(SQLMATH_BASE_C3)
 #define SQLMATH_BASE_C3
 
 
 #include "sqlmath_jenks.c"
-typedef struct DbExecBindElem {
-    const char *buf;
-    char *key;
-    int buflen;
-    char datatype;
-} DbExecBindElem;
 // track how many sqlite-db open
 static int dbCount = 0;
 
 
 // file sqlmath_base - SQLMATH_API
+
+// SQLMATH_API db - start
 SQLMATH_API int __dbFileImportOrExport(
     sqlite3 * pInMemory,
     char *zFilename,
     const int isSave
 ) {
     // fprintf(stderr, "\nsqlmath.dbFileImportOrExport(pp=%p ff=%s ss=%d)\n",
     //     pInMemory, zFilename, isSave);
@@ -492,15 +510,22 @@
         // fprintf(stderr, "\nsqlmath.dbClose(argv0=%lld db=%lld dbCount=%d)\n",
         //     baton->argv[0], (int64_t) db, dbCount);
     }
   catch_error:
     (void) 0;
 }
 
-// SQLMATH_API dbexec - start
+// SQLMATH_API dbExec - start
+typedef struct DbExecBindElem {
+    const char *buf;
+    char *key;
+    int buflen;
+    char datatype;
+} DbExecBindElem;
+
 SQLMATH_API void dbExec(
     Jsbaton * baton
 ) {
 // This function will run <zSql> in <db> and save any result (list of tables
 // containing rows from SELECT/pragma/etc) as serialized json-string in <str99>.
     // declare var
     DbExecBindElem *bindElem = NULL;
@@ -822,15 +847,15 @@
     }
 #ifndef EMSCRIPTEN
     // mutex leave
     sqlite3_mutex_leave(sqlite3_db_mutex(db));
 #endif                          // EMSCRIPTEN
 }
 
-// SQLMATH_API dbexec - end
+// SQLMATH_API dbExec - end
 
 SQLMATH_API void dbFileImportOrExport(
     Jsbaton * baton
 ) {
 // This function will load/save <zFilename> to/from <db>.
     // declare var
     int errcode = 0;
@@ -878,190 +903,23 @@
     //     filename);
     // save db
     baton->argv[0] = (int64_t) db;
   catch_error:
     (void) 0;
 }
 
-SQLMATH_API void vector99_buf_free(
-    Vector99 * vec99
-) {
-// This function will free <vec99>->buf and reset everything to zero.
-    if (vec99 == NULL) {
-        return;
-    }
-    sqlite3_free(vec99->buf);
-    memset(vec99, 0, sizeof(*vec99));
-}
-
-SQLMATH_API int vector99_buf_malloc(
-    Vector99 * vec99
-) {
-// This function will malloc <vec99>->buf, or return SQLITE_NOMEM.
-    static const int alloc0 = 256;
-    if (vec99 == NULL) {
-        return SQLITE_NOMEM;
-    }
-    vec99->buf = sqlite3_malloc(alloc0 * sizeof(double));
-    if (vec99->buf == NULL) {
-        return SQLITE_NOMEM;
-    }
-    vec99->alloc = alloc0;
-    vec99->size = 0;
-    vec99->arg0 = NAN;
-    vec99->arg1 = NAN;
-    return SQLITE_OK;
-}
-
-SQLMATH_API int vector99_nomem(
-    const Vector99 * vec99
-) {
-// This function will check if <vec99>->buf is null.
-    return vec99 == NULL || vec99->buf == NULL;
-}
-
-SQLMATH_API double vector99_pop_front(
-    Vector99 * vec99
-) {
-// This function will pop_front <vec99>, or return NAN if empty.
-    if (vector99_nomem(vec99) || vec99->size <= 0) {
-        return NAN;
-    }
-    double val = vec99->buf[0];
-    vec99->size -= 1;
-    memmove(vec99->buf, vec99->buf + 1, vec99->size * sizeof(double));
-    return val;
-}
-
-SQLMATH_API int vector99_push_back(
-    Vector99 * vec99,
-    double val
-) {
-// This function will push_back <val> to <vec99>,
-// and dynamically grow <vec99> if necessary.
-    // error - nomem
-    if (vector99_nomem(vec99)) {
-        return SQLITE_NOMEM;
-    }
-    if (vec99->size >= vec99->alloc) {
-        vec99->alloc *= 2;
-        // error - toobig
-        if (vec99->alloc > SQLITE_MAX_LENGTH2) {
-            vector99_buf_free(vec99);
-            return SQLITE_TOOBIG;
-        }
-        double *buf_old = vec99->buf;
-        vec99->buf =
-            sqlite3_realloc(vec99->buf, vec99->alloc * sizeof(double));
-        // error - nomem
-        if (vector99_nomem(vec99)) {
-            // dont forget to free buf_old
-            vec99->buf = buf_old;
-            vector99_buf_free(vec99);
-            return SQLITE_NOMEM;
-        }
-    }
-    vec99->buf[vec99->size] = val;
-    vec99->size += 1;
-    return SQLITE_OK;
-}
-
-SQLMATH_API void vector99_result_blob(
-    Vector99 * vec99,
-    sqlite3_context * context
-) {
-// This function will return <vec99> as result-blob in given <context>.
-    sqlite3_result_blob(context, (const char *) vec99->buf,
-        vec99->size * sizeof(double),
-        // destructor
-        sqlite3_free);
-}
-
-// SQLMATH_API Vector99 - end
-
-SQLMATH_API int doubleSign(
-    const double aa
-) {
-// This function will return sign of <aa>.
-    return aa < 0 ? -1 : aa > 0 ? 1 : 0;
-}
-
-SQLMATH_API int doubleSortCompare(
-    const void *aa,
-    const void *bb
-) {
-// This function will compare <aa> with <bb>.
-    const double cc = *(double *) aa - *(double *) bb;
-    return cc < 0 ? -1 : cc > 0 ? 1 : 0;
-}
-
-SQLMATH_API const char *jsbatonValueErrmsg(
-    Jsbaton * baton
-) {
-// This function will return <baton>->errmsg.
-    return (const char *) baton->errmsg;
-}
-
-SQLMATH_API const char *jsbatonValueStringArgi(
-    Jsbaton * baton,
-    int argi
-) {
-// This function will return string-value from <baton> at given <argi>.
-    if (baton->argv[argi] == 0) {
-        return NULL;
-    }
-    return ((const char *) baton) + ((size_t) baton->argv[argi] + 1 + 4);
-}
-
-SQLMATH_API int noop(
-) {
-// This function will do nothing except return 0.
-    return 0;
-}
-
-SQLMATH_API double sqlite3_value_double_or_nan(
-    sqlite3_value * arg
-) {
-// This function will return double if finite else nan.
-    switch (sqlite3_value_numeric_type(arg)) {
-    case SQLITE_INTEGER:
-    case SQLITE_FLOAT:
-        {
-            const double xx = sqlite3_value_double(arg);
-            if (isfinite(xx)) {
-                return xx;
-            }
-        }
-        break;
-    }
-    return NAN;
-}
-
-SQLMATH_API const char *sqlmathSnprintfTrace(
-    char *buf,
-    const char *prefix,
-    const char *errmsg,
-    const char *func,
-    const char *file,
-    int line
-) {
-// This function will write <errmsg> to <buf> with additional trace-info.
-    if (snprintf(buf, SIZEOF_MESSAGE_DEFAULT, "%s%s\n    at %s (%s:%d)",
-            prefix, errmsg, func, file, line) < 0) {
-        abort();
-    }
-    return (const char *) buf;
-}
+// SQLMATH_API db - end
 
+// SQLMATH_API str99 - start
 SQLMATH_API void str99ArrayAppendDouble(
     sqlite3_str * str99,
-    const double val
+    const double xx
 ) {
-// This function will append double <val> to <str99>.
-    sqlite3_str_append(str99, (const char *) &val, 8);
+// This function will append double <xx> to <str99>.
+    sqlite3_str_append(str99, (const char *) &xx, 8);
 }
 
 SQLMATH_API void str99ArrayAppendJsonarray(
     sqlite3_str * str99,
     const char *json,
     int nn
 ) {
@@ -1187,80 +1045,206 @@
 // This function will return <str99> as result-text in given <context>.
     sqlite3_result_text(context, (const char *) sqlite3_str_value(str99),
         sqlite3_str_length(str99),
         // destructor
         sqlite3_free);
 }
 
+// SQLMATH_API str99 - end
 
-// file sqlmath_base - SQLMATH_FUNC
-// SQLMATH_FUNC sql_avg_ema_func - start
-SQLMATH_FUNC static void sql_avg_ema_value(
-    sqlite3_context * context
+// SQLMATH_API vector99 - start
+SQLMATH_API void vector99_agg_free(
+    Vector99 ** vec99_agg
 ) {
-// This function will aggregate exponential-moving-average.
-    // vec99 - init
-    VECTOR99_AGGREGATE_CONTEXT();
-    sqlite3_result_double(context, vec99->buf[0]);
+    if (vec99_agg != NULL) {
+        sqlite3_free(*vec99_agg);
+        *vec99_agg = NULL;
+    }
 }
 
-SQLMATH_FUNC static void sql_avg_ema_final(
-    sqlite3_context * context
+SQLMATH_API double *vector99_body(
+    const Vector99 * vec99
 ) {
-// This function will aggregate exponential-moving-average.
-    // vec99 - value
-    sql_avg_ema_value(context);
-    // vec99 - init
-    VECTOR99_AGGREGATE_CONTEXT();
-    // vec99 - cleanup
-    vector99_buf_free(vec99);
+    return (double *) ((char *) vec99 + sizeof(Vector99)) +
+        (int) vec99->nhead;
 }
 
-SQLMATH_FUNC static void sql_avg_ema_inverse(
-    sqlite3_context * context,
-    int argc,
-    sqlite3_value ** argv
+SQLMATH_API double *vector99_head(
+    const Vector99 * vec99
 ) {
-// This function will aggregate exponential-moving-average.
-    UNUSED_PARAMETER(argc);
-    UNUSED_PARAMETER(argv);
-    // vec99 - init
-    VECTOR99_AGGREGATE_CONTEXT();
-    vector99_pop_front(vec99);
+    return (double *) ((char *) vec99 + sizeof(Vector99));
 }
 
-SQLMATH_FUNC static void sql_avg_ema_step(
-    sqlite3_context * context,
-    int argc,
-    sqlite3_value ** argv
+SQLMATH_API Vector99 *vector99_malloc(
+    const int nhead
 ) {
-// This function will aggregate exponential-moving-average.
-    UNUSED_PARAMETER(argc);
-    // vec99 - init
-    VECTOR99_AGGREGATE_CONTEXT();
-    if (isnan(vec99->arg0)) {
-        vec99->arg0 = sqlite3_value_double(argv[1]);    // alpha
+    // const int alloc = sizeof(Vector99) + nhead * sizeof(double) + 0;
+    const int alloc = sizeof(Vector99) + nhead * sizeof(double) + 256;
+    if (alloc > SQLITE_MAX_LENGTH2) {
+        return NULL;
     }
-    // vec99 - calculate ema
-    const double alpha = vec99->arg0;
-    const double elem = sqlite3_value_double(argv[0]);
-    for (int ii = 0; ii < vec99->size; ii += 1) {
-        vec99->buf[ii] = alpha * elem + (1 - alpha) * vec99->buf[ii];
+    Vector99 *vec99 = sqlite3_malloc(alloc);
+    if (vec99 == NULL) {
+        return NULL;
     }
-    // vec99 - push_back elem
-    const int errcode = vector99_push_back(vec99, elem);
-    SQLITE3_RESULT_ERROR_CODE(errcode);
-    return;
+    // zero vec99
+    memset(vec99, 0, alloc);
+    vec99->alloc = alloc;
+    vec99->nhead = MAX(0, nhead);
+    return vec99;
+}
+
+SQLMATH_API int vector99_push(
+    Vector99 ** vec99_agg,
+    double xx
+) {
+    if (vec99_agg == NULL || *vec99_agg == NULL) {
+        return SQLITE_NOMEM;
+    }
+    Vector99 *vec99 = *vec99_agg;
+    // rotate wnn
+    if (vec99->wnn) {
+        vector99_body(vec99)[(int) vec99->wii] = xx;
+        vec99->wii += 1;
+        if (vec99->wii >= vec99->wnn) {
+            vec99->wii -= vec99->wnn;
+        }
+        return SQLITE_OK;
+    }
+    const int nn =
+        (sizeof(Vector99) / sizeof(double) + vec99->nbody + vec99->nhead);
+    uint32_t alloc = vec99->alloc;
+    if (nn * sizeof(double) >= alloc) {
+        // error - toobig
+        if (alloc >= SQLITE_MAX_LENGTH2) {
+            goto catch_error;
+        }
+        alloc = MIN(SQLITE_MAX_LENGTH2, alloc * 2);
+        vec99 = sqlite3_realloc(vec99, alloc);
+        // error - nomem
+        if (vec99 == NULL) {
+            goto catch_error;
+        }
+        vec99->alloc = alloc;
+        *vec99_agg = vec99;
+    }
+    ((double *) vec99)[nn] = xx;
+    vec99->nbody += 1;
+    return SQLITE_OK;
   catch_error:
-    vector99_buf_free(vec99);
+    vector99_agg_free(vec99_agg);
+    return SQLITE_NOMEM;
+}
+
+SQLMATH_API void vector99_result_blob(
+    Vector99 * vec99,
+    sqlite3_context * context
+) {
+// This function will return <vec99> as result-blob in given <context>.
+    vec99->alloc =
+        sizeof(Vector99) + (vec99->nhead + vec99->nbody) * sizeof(double);
+    sqlite3_result_blob(context, (const char *) vec99, vec99->alloc,
+        // destructor
+        sqlite3_free);
+}
+
+SQLMATH_API int vector99_valid(
+    const Vector99 * vec99
+) {
+// This function will validate <vec99>.
+    if (vec99 == NULL) {
+        return 0;
+    }
+    const double alloc = vec99->alloc;
+    const double nbody = vec99->nbody;
+    return (alloc >= sizeof(*vec99) + nbody * sizeof(double)
+        && alloc <= SQLITE_MAX_LENGTH2 && nbody >= 0
+        && nbody <= SQLITE_MAX_LENGTH2);
+}
+
+// SQLMATH_API vector99 - end
+
+SQLMATH_API int doubleSign(
+    const double aa
+) {
+// This function will return sign of <aa>.
+    return aa < 0 ? -1 : aa > 0 ? 1 : 0;
+}
+
+SQLMATH_API int doubleSortCompare(
+    const void *aa,
+    const void *bb
+) {
+// This function will compare <aa> with <bb>.
+    const double cc = *(double *) aa - *(double *) bb;
+    return cc < 0 ? -1 : cc > 0 ? 1 : 0;
+}
+
+SQLMATH_API const char *jsbatonValueErrmsg(
+    Jsbaton * baton
+) {
+// This function will return <baton>->errmsg.
+    return (const char *) baton->errmsg;
+}
+
+SQLMATH_API const char *jsbatonValueStringArgi(
+    Jsbaton * baton,
+    int argi
+) {
+// This function will return string-value from <baton> at given <argi>.
+    if (baton->argv[argi] == 0) {
+        return NULL;
+    }
+    return ((const char *) baton) + ((size_t) baton->argv[argi] + 1 + 4);
+}
+
+SQLMATH_API int noop(
+) {
+// This function will do nothing except return 0.
+    return 0;
+}
+
+SQLMATH_API double sqlite3_value_double_or_nan(
+    sqlite3_value * arg
+) {
+// This function will return NAN if NULL else double.
+    return sqlite3_value_type(arg) ==
+        SQLITE_NULL ? NAN : sqlite3_value_double(arg);
+}
+
+SQLMATH_API double sqlite3_value_double_or_prev(
+    sqlite3_value * arg,
+    double *previous
+) {
+// This function will save <arg> as <previous> if not NULL.
+    if (sqlite3_value_type(arg) != SQLITE_NULL) {
+        *previous = sqlite3_value_double(arg);
+    }
+    return *previous;
+}
+
+SQLMATH_API const char *sqlmathSnprintfTrace(
+    char *buf,
+    const char *prefix,
+    const char *errmsg,
+    const char *func,
+    const char *file,
+    int line
+) {
+// This function will write <errmsg> to <buf> with additional trace-info.
+    if (snprintf(buf, SIZEOF_MESSAGE_DEFAULT, "%s%s\n    at %s (%s:%d)",
+            prefix, errmsg, func, file, line) < 0) {
+        abort();
+    }
+    return (const char *) buf;
 }
 
-// SQLMATH_FUNC sql_avg_ema_func - end
 
-// SQLMATH_FUNC sql_btobase64_func - start
+// file sqlmath_base - SQLMATH_FUNC
+// SQLMATH_FUNC sql1_btobase64_func - start
 static char *base64Encode(
     const unsigned char *blob,
     int *nn
 ) {
 // This function will base64-encode <blob> to <text>.
     if (blob == NULL || *nn < 0) {
         *nn = 0;
@@ -1315,15 +1299,15 @@
     }
     // save bb
     *nn = bb;
     // return text
     return text - bb;
 }
 
-SQLMATH_FUNC static void sql_btobase64_func(
+SQLMATH_FUNC static void sql1_btobase64_func(
     sqlite3_context * context,
     int argc,
     sqlite3_value ** argv
 ) {
 // This function will convert blob to base64-encoded-text.
     UNUSED_PARAMETER(argc);
     // declare var
@@ -1339,40 +1323,49 @@
         return;
     }
     sqlite3_result_text(context, (const char *) text, nn,
         // cleanup base64Encode()
         sqlite3_free);
 }
 
-// SQLMATH_FUNC sql_btobase64_func - end
+// SQLMATH_FUNC sql1_btobase64_func - end
 
-SQLMATH_FUNC static void sql_btotext_func(
+SQLMATH_FUNC static void sql1_btotext_func(
     sqlite3_context * context,
     int argc,
     sqlite3_value ** argv
 ) {
 // This function will convert blob to text.
     UNUSED_PARAMETER(argc);
     sqlite3_result_text(context, (const char *) sqlite3_value_text(argv[0]),
         -1, SQLITE_TRANSIENT);
 }
 
+SQLMATH_FUNC static void sql1_castrealornull_func(
+    sqlite3_context * context,
+    int argc,
+    sqlite3_value ** argv
+) {
+// This function will cast <argv>[0] to double or zero.
+    UNUSED_PARAMETER(argc);
+    sqlite3_result_double(context, sqlite3_value_double_or_nan(argv[0]));
+}
 
-SQLMATH_FUNC static void sql_castrealorzero_func(
+SQLMATH_FUNC static void sql1_castrealorzero_func(
     sqlite3_context * context,
     int argc,
     sqlite3_value ** argv
 ) {
 // This function will cast <argv>[0] to double or zero.
     UNUSED_PARAMETER(argc);
-    const double num = sqlite3_value_double(argv[0]);
-    sqlite3_result_double(context, isfinite(num) ? num : 0);
+    const double xx = sqlite3_value_double(argv[0]);
+    sqlite3_result_double(context, isfinite(xx) ? xx : 0);
 }
 
-SQLMATH_FUNC static void sql_casttextorempty_func(
+SQLMATH_FUNC static void sql1_casttextorempty_func(
     sqlite3_context * context,
     int argc,
     sqlite3_value ** argv
 ) {
 // This function will cast <argv>[0] to text or empty-string.
     UNUSED_PARAMETER(argc);
     switch (sqlite3_value_type(argv[0])) {
@@ -1406,47 +1399,47 @@
 // If you insist on round-tripping through sqlite3_value_text,
 // then you must pass SQLITE_TRANSIENT for the last parameter
 // - the pointer returned by sqlite3_value_text is only guaranteed
 // to be valid until the custom function returns.
         SQLITE_TRANSIENT);
 }
 
-SQLMATH_FUNC static void sql_copyblob_func(
+SQLMATH_FUNC static void sql1_copyblob_func(
     sqlite3_context * context,
     int argc,
     sqlite3_value ** argv
 ) {
 // This function will copy blob/text/value <argv>[0].
     UNUSED_PARAMETER(argc);
     sqlite3_result_value(context, argv[0]);
 }
 
-SQLMATH_FUNC static void sql_cot_func(
+SQLMATH_FUNC static void sql1_cot_func(
     sqlite3_context * context,
     int argc,
     sqlite3_value ** argv
 ) {
 // This function will return cot(argv[0]).
     UNUSED_PARAMETER(argc);
     sqlite3_result_double(context,
         1.0 / tan(sqlite3_value_double_or_nan(argv[0])));
 }
 
-SQLMATH_FUNC static void sql_coth_func(
+SQLMATH_FUNC static void sql1_coth_func(
     sqlite3_context * context,
     int argc,
     sqlite3_value ** argv
 ) {
 // This function will return coth(argv[0]).
     UNUSED_PARAMETER(argc);
     sqlite3_result_double(context,
         1.0 / tanh(sqlite3_value_double_or_nan(argv[0])));
 }
 
-SQLMATH_FUNC static void sql_jenks_blob_func(
+SQLMATH_FUNC static void sql1_jenks_blob_func(
     sqlite3_context * context,
     int argc,
     sqlite3_value ** argv
 ) {
 // This function will calculate <kk> jenks-natrual-breaks in given <values>,
 // and return a mallocd (double *) array with length (1 + kk * 2) of form:
 // [
@@ -1473,15 +1466,228 @@
         return;
     }
     // jenks - result
     sqlite3_result_blob(context, (void *) result,
         (1 + ((int) result[0]) * 2) * 8, sqlite3_free);
 }
 
-// SQLMATH_FUNC sql_jenks_concat_func - start
+SQLMATH_FUNC static void sql1_jenks_json_func(
+    sqlite3_context * context,
+    int argc,
+    sqlite3_value ** argv
+) {
+// This function will calculate <kk> jenks-natrual-breaks in given <values>,
+// and return a json array with length (1 + kk * 2) of form:
+// [
+// (double) kk,
+// (double) break_1, (double) count_1,
+// (double) break_2, (double) count_2,
+// ...,
+// (double) break_k, (double) count_k
+// ]
+    UNUSED_PARAMETER(argc);
+    // declare var
+    int errcode = 0;
+    // str99 - to-array
+    STR99_ALLOCA(arr);
+    str99ArrayAppendJsonarray(  //
+        arr,                    // array
+        (char *) sqlite3_value_blob(argv[1]),   // json
+        sqlite3_value_bytes(argv[1]));  // nn
+    STR99_RESULT_ERROR(arr);
+    // jenks - classify
+    STR99_ALLOCA(str99);
+    str99JsonAppendJenks(       //
+        str99,                  // json
+        sqlite3_value_int(argv[0]),     // kk
+        (double *) arr->zText,  // array
+        sqlite3_str_length(arr) / 8);   // nn
+    sqlite3_str_reset(arr);
+    STR99_RESULT_ERROR(str99);
+    // str99 - result
+    str99ResultText(str99, context);
+  catch_error:
+    (void) 0;
+}
+
+SQLMATH_FUNC static void sql1_jsonfromfloat64array_func(
+    sqlite3_context * context,
+    int argc,
+    sqlite3_value ** argv
+) {
+// This function will create json-encoded-flat-array from binary-Float64Array.
+    UNUSED_PARAMETER(argc);
+    // declare var
+    int errcode = 0;
+    SQLITE3_RESULT_JSONFLOAT64ARRAY(str99,
+        (double *) sqlite3_value_blob(argv[0]),
+        sqlite3_value_bytes(argv[0]) / 8);
+  catch_error:
+    (void) 0;
+}
+
+SQLMATH_FUNC static void sql1_jsontofloat64array_func(
+    sqlite3_context * context,
+    int argc,
+    sqlite3_value ** argv
+) {
+// This function will create binary-Float64Array from json-encoded-flat-array.
+    UNUSED_PARAMETER(argc);
+    // declare var
+    int errcode = 0;
+    // str99 - to-array
+    STR99_ALLOCA(str99);
+    str99ArrayAppendJsonarray(  //
+        str99,                  // array
+        (char *) sqlite3_value_blob(argv[0]),   // json
+        sqlite3_value_bytes(argv[0]));  // nn
+    STR99_RESULT_ERROR(str99);
+    // str99 - result
+    str99ResultBlob(str99, context);
+  catch_error:
+    (void) 0;
+}
+
+// SQLMATH_FUNC sql1_marginoferror95_func - start
+SQLMATH_API double marginoferror95(
+    double nn,
+    double pp
+) {
+// This function will calculate margin-of-error sqrt(pp*(1-pp)/nn).
+    return 1.9599639845400542 * sqrt(pp * (1 - pp) / nn);
+}
+
+SQLMATH_FUNC static void sql1_marginoferror95_func(
+    sqlite3_context * context,
+    int argc,
+    sqlite3_value ** argv
+) {
+// This function will calculate margin-of-error sqrt(pp*(1-pp)/nn).
+    UNUSED_PARAMETER(argc);
+    sqlite3_result_double(context,
+        marginoferror95(sqlite3_value_double_or_nan(argv[0]),
+            sqlite3_value_double_or_nan(argv[1])));
+}
+
+// SQLMATH_FUNC sql1_marginoferror95_func - end
+
+SQLMATH_FUNC static void sql1_random1_func(
+    sqlite3_context * context,
+    int argc,
+    sqlite3_value ** argv
+) {
+// This function will generate high-quality random-float between 0 <= xx < 1.
+    UNUSED_PARAMETER(argc);
+    UNUSED_PARAMETER(argv);
+    static const double inv = 1.0 / 0x100000000;
+    uint32_t xx[1];
+    sqlite3_randomness(4, (void *) xx);
+    sqlite3_result_double(context, ((double) *xx) * inv);
+}
+
+SQLMATH_FUNC static void sql1_roundorzero_func(
+    sqlite3_context * context,
+    int argc,
+    sqlite3_value ** argv
+) {
+// This function will round <argv>[0] to decimal <argv>[1].
+    UNUSED_PARAMETER(argc);
+    if (sqlite3_value_numeric_type(argv[0]) == SQLITE_NULL) {
+        sqlite3_result_double(context, 0);
+        return;
+    }
+    // declare var
+    char *zBuf = NULL;
+    double rr = sqlite3_value_double(argv[0]);
+    int nn = sqlite3_value_int(argv[1]);
+    nn = MIN(nn, 30);
+    nn = MAX(nn, 0);
+    // If YY==0 and XX will fit in a 64-bit int,
+    // handle the rounding directly,
+    // otherwise use printf.
+    if (rr < -4503599627370496.0 || rr > +4503599627370496.0) {
+    } else if (nn == 0) {
+        // The value has no fractional part so there is nothing to round
+        rr = (double) ((sqlite_int64) (rr + (rr < 0 ? -0.5 : +0.5)));
+    } else {
+        zBuf = sqlite3_mprintf("%.*f", nn, rr);
+        if (zBuf == NULL) {
+            sqlite3_result_error_nomem(context);
+            return;
+        }
+        rr = strtod(zBuf, NULL);
+        // cleanup sqlite3_mprintf()
+        sqlite3_free(zBuf);
+    }
+    sqlite3_result_double(context, rr);
+}
+
+SQLMATH_FUNC static void sql1_sign_func(
+    sqlite3_context * context,
+    int argc,
+    sqlite3_value ** argv
+) {
+/*
+** Implementation of the sign() function
+** return one of 3 possibilities +1,0 or -1 when the argument is respectively
+** positive, 0 or negative.
+** When the argument is NULL the result is also NULL (completly conventional)
+*/
+    UNUSED_PARAMETER(argc);
+    switch (sqlite3_value_numeric_type(argv[0])) {
+    case SQLITE_INTEGER:
+    case SQLITE_FLOAT:
+        {
+            double rVal = sqlite3_value_double(argv[0]);
+            sqlite3_result_double(context,
+                (rVal > 0) ? 1 : (rVal < 0) ? -1 : 0);
+        }
+        return;
+    }
+}
+
+SQLMATH_FUNC static void sql1_squared_func(
+    sqlite3_context * context,
+    int argc,
+    sqlite3_value ** argv
+) {
+/*
+** Implementation of the squared() function
+** the argument is an integer.
+** Since SQLite isn't strongly typed (almost untyped actually) this is a bit pedantic
+*/
+    UNUSED_PARAMETER(argc);
+    switch (sqlite3_value_numeric_type(argv[0])) {
+    case SQLITE_INTEGER:
+    case SQLITE_FLOAT:
+        {
+            double rVal = sqlite3_value_double(argv[0]);
+            sqlite3_result_double(context, rVal * rVal);
+        }
+        return;
+    }
+}
+
+SQLMATH_FUNC static void sql1_throwerror_func(
+    sqlite3_context * context,
+    int argc,
+    sqlite3_value ** argv
+) {
+// This function will return sqlite3_result_error_code(argv[0]).
+    UNUSED_PARAMETER(argc);
+    // declare var
+    int errcode = sqlite3_value_int(argv[0]);
+    if (0 <= errcode && errcode <= 28) {
+        sqlite3_result_error_code(context, errcode);
+        return;
+    }
+    sqlite3_result_error_code(context, SQLITE_INTERNAL);
+}
+
+// SQLMATH_FUNC sql2_jenks_concat_func - start
 static void str99arrCleanup(
     const int argc,
     sqlite3_str ** str99arr
 ) {
     for (int ii = 0; ii < argc; ii += 1) {
         sqlite3_str *str99 = str99arr[ii];
         if (str99 != NULL) {
@@ -1490,15 +1696,15 @@
             }
             sqlite3_free(str99);
             str99arr[ii] = NULL;
         }
     }
 }
 
-SQLMATH_FUNC static void sql_jenks_concat_final(
+SQLMATH_FUNC static void sql2_jenks_concat_final(
     sqlite3_context * context
 ) {
 // This function will calculate <kk> jenks-natrual-breaks in each column <ii>,
 // and return a json array.
     // str99arr - init
     sqlite3_str **str99arr =
         (sqlite3_str **) sqlite3_aggregate_context(context, 0);
@@ -1534,15 +1740,15 @@
     // str99json - result
     str99ResultText(str99json, context);
   catch_error:
     // str99arr - cleanup
     str99arrCleanup(argc, str99arr);
 }
 
-SQLMATH_FUNC static void sql_jenks_concat_step(
+SQLMATH_FUNC static void sql2_jenks_concat_step(
     sqlite3_context * context,
     int argc,
     sqlite3_value ** argv
 ) {
 // This function will calculate <kk> jenks-natrual-breaks in each column <ii>,
 // and return a json array.
     // init kk
@@ -1581,204 +1787,100 @@
         sqlite3_str *str99 = str99arr[ii];
         if (sqlite3_value_numeric_type(argv[ii]) != SQLITE_NULL) {
             str99ArrayAppendDouble(str99, sqlite3_value_double(argv[ii]));
         }
     }
 }
 
-// SQLMATH_FUNC sql_jenks_concat_func - end
+// SQLMATH_FUNC sql2_jenks_concat_func - end
 
-SQLMATH_FUNC static void sql_jenks_json_func(
-    sqlite3_context * context,
-    int argc,
-    sqlite3_value ** argv
-) {
-// This function will calculate <kk> jenks-natrual-breaks in given <values>,
-// and return a json array with length (1 + kk * 2) of form:
-// [
-// (double) kk,
-// (double) break_1, (double) count_1,
-// (double) break_2, (double) count_2,
-// ...,
-// (double) break_k, (double) count_k
-// ]
-    UNUSED_PARAMETER(argc);
-    // declare var
-    int errcode = 0;
-    // str99 - to-array
-    STR99_ALLOCA(arr);
-    str99ArrayAppendJsonarray(  //
-        arr,                    // array
-        (char *) sqlite3_value_blob(argv[1]),   // json
-        sqlite3_value_bytes(argv[1]));  // nn
-    STR99_RESULT_ERROR(arr);
-    // jenks - classify
-    STR99_ALLOCA(str99);
-    str99JsonAppendJenks(       //
-        str99,                  // json
-        sqlite3_value_int(argv[0]),     // kk
-        (double *) arr->zText,  // array
-        sqlite3_str_length(arr) / 8);   // nn
-    sqlite3_str_reset(arr);
-    STR99_RESULT_ERROR(str99);
-    // str99 - result
-    str99ResultText(str99, context);
-  catch_error:
-    (void) 0;
-}
-
-SQLMATH_FUNC static void sql_jsonfromfloat64array_func(
-    sqlite3_context * context,
-    int argc,
-    sqlite3_value ** argv
-) {
-// This function will create json-encoded-flat-array from binary-Float64Array.
-    UNUSED_PARAMETER(argc);
-    // declare var
-    int errcode = 0;
-    // str99 - init
-    STR99_ALLOCA(str99);
-    // str99 - jsonfrom
-    str99JsonAppendFloat64array(        //
-        str99,                  //
-        (double *) sqlite3_value_blob(argv[0]), //
-        sqlite3_value_bytes(argv[0]) / 8);
-    STR99_RESULT_ERROR(str99);
-    // str99 - result
-    str99ResultText(str99, context);
-  catch_error:
-    (void) 0;
-}
-
-SQLMATH_FUNC static void sql_jsontofloat64array_func(
-    sqlite3_context * context,
-    int argc,
-    sqlite3_value ** argv
-) {
-// This function will create binary-Float64Array from json-encoded-flat-array.
-    UNUSED_PARAMETER(argc);
-    // declare var
-    int errcode = 0;
-    // str99 - to-array
-    STR99_ALLOCA(str99);
-    str99ArrayAppendJsonarray(  //
-        str99,                  // array
-        (char *) sqlite3_value_blob(argv[0]),   // json
-        sqlite3_value_bytes(argv[0]));  // nn
-    STR99_RESULT_ERROR(str99);
-    // str99 - result
-    str99ResultBlob(str99, context);
-  catch_error:
-    (void) 0;
-}
-
-// SQLMATH_FUNC sql_marginoferror95_func - start
-SQLMATH_API double marginoferror95(
-    double nn,
-    double pp
-) {
-// This function will calculate margin-of-error sqrt(pp*(1-pp)/nn).
-    return 1.9599639845400542 * sqrt(pp * (1 - pp) / nn);
-}
-
-SQLMATH_FUNC static void sql_marginoferror95_func(
-    sqlite3_context * context,
-    int argc,
-    sqlite3_value ** argv
-) {
-// This function will calculate margin-of-error sqrt(pp*(1-pp)/nn).
-    UNUSED_PARAMETER(argc);
-    sqlite3_result_double(context,
-        marginoferror95(sqlite3_value_double_or_nan(argv[0]),
-            sqlite3_value_double_or_nan(argv[1])));
-}
-
-// SQLMATH_FUNC sql_marginoferror95_func - end
-
-// SQLMATH_FUNC sql_matrix2d_concat_func - start
-SQLMATH_FUNC static void sql_matrix2d_concat_final(
+// SQLMATH_FUNC sql2_matrix2d_concat_func - start
+SQLMATH_FUNC static void sql2_matrix2d_concat_final(
     sqlite3_context * context
 ) {
 // This function will concat rows of nCol doubles to a 2d-matrix.
     // vec99 - init
-    VECTOR99_AGGREGATE_CONTEXT();
+    VECTOR99_AGGREGATE_CONTEXT(0);
     // vec99 - null-case
-    if (vec99->size <= 2) {
+    if (vec99->nbody <= 2) {
         sqlite3_result_null(context);
         return;
     }
     // vec99 - result
-    vector99_result_blob(vec99, context);
+    int alloc = vec99->nbody * sizeof(double);
+    memmove(vec99, vec99_body, alloc);
+    sqlite3_result_blob(context, (const char *) vec99, alloc,
+        // destructor
+        sqlite3_free);
 }
 
-SQLMATH_FUNC static void sql_matrix2d_concat_step(
+SQLMATH_FUNC static void sql2_matrix2d_concat_step(
     sqlite3_context * context,
     int argc,
     sqlite3_value ** argv
 ) {
 // This function will concat rows of nCol doubles to a 2d-matrix.
     // declare var
     int errcode = 0;
     // vec99 - init
-    VECTOR99_AGGREGATE_CONTEXT();
-    if (vec99->size <= 0) {
-        errcode = vector99_push_back(vec99, 0);
-        errcode = vector99_push_back(vec99, (double) argc);
-        SQLITE3_RESULT_ERROR_CODE(errcode);
+    VECTOR99_AGGREGATE_CONTEXT(0);
+    if ((*vec99_agg)->nbody <= 0) {
+        errcode = vector99_push(vec99_agg, 0);
+        errcode = vector99_push(vec99_agg, (double) argc);
     }
     // vec99 - append double
     for (int ii = 0; ii < argc; ii += 1) {
-        errcode = vector99_push_back(vec99, sqlite3_value_double(argv[ii]));
+        errcode = vector99_push(vec99_agg, sqlite3_value_double(argv[ii]));
     }
     SQLITE3_RESULT_ERROR_CODE(errcode);
-    vec99->buf[0] += 1;
+    vector99_body(*vec99_agg)[0] += 1;
     return;
   catch_error:
-    vector99_buf_free(vec99);
+    vector99_agg_free(vec99_agg);
 }
 
-// SQLMATH_FUNC sql_matrix2d_concat_func - end
+// SQLMATH_FUNC sql2_matrix2d_concat_func - end
 
-// SQLMATH_FUNC sql_quantile_func - start
+// SQLMATH_FUNC sql2_quantile_func - start
 static double quickselect(
     double *arr,
     const int nn,
     const int kk
 ) {
 // This function will find <kk>-th element in <arr> using quickselect-algorithm.
 // https://www.stat.cmu.edu/~ryantibs/median/quickselect.c
     if (nn <= 0) {
-        return 0;
+        return NAN;
     }
     double aa = *arr;
     double tmp = 0;
     int ii;
     int ir;
     int jj;
     int ll;
     int mid;
     ll = 0;
     ir = nn - 1;
     while (1) {
         if (ir <= ll + 1) {
             if (ir == ll + 1 && arr[ir] < arr[ll]) {
-                SWAP(arr[ll], arr[ir]);
+                SWAP(arr[ll], arr[ir], tmp);
             }
             return arr[kk];
         } else {
             mid = (ll + ir) >> 1;
-            SWAP(arr[mid], arr[ll + 1]);
+            SWAP(arr[mid], arr[ll + 1], tmp);
             if (arr[ll] > arr[ir]) {
-                SWAP(arr[ll], arr[ir]);
+                SWAP(arr[ll], arr[ir], tmp);
             }
             if (arr[ll + 1] > arr[ir]) {
-                SWAP(arr[ll + 1], arr[ir]);
+                SWAP(arr[ll + 1], arr[ir], tmp);
             }
             if (arr[ll] > arr[ll + 1]) {
-                SWAP(arr[ll], arr[ll + 1]);
+                SWAP(arr[ll], arr[ll + 1], tmp);
             }
             ii = ll + 1;
             jj = ir;
             aa = arr[ll + 1];
             while (1) {
                 while (1) {
                     ii += 1;
@@ -1791,15 +1893,15 @@
                     if (arr[jj] <= aa) {
                         break;
                     }
                 }
                 if (jj < ii) {
                     break;
                 }
-                SWAP(arr[ii], arr[jj]);
+                SWAP(arr[ii], arr[jj], tmp);
             }
             arr[ll + 1] = arr[jj];
             arr[jj] = aa;
             if (jj >= kk) {
                 ir = jj - 1;
             }
             if (jj <= kk) {
@@ -1808,297 +1910,732 @@
         }
     }
 }
 
 SQLMATH_API double quantile(
     double *arr,
     const int nn,
-    const double pp
+    const double qq
 ) {
-// This function will find <pp>-th-quantile element in <arr>
+// This function will find <qq>-th-quantile element in <arr>
 // using quickselect-algorithm.
 // https://www.stat.cmu.edu/~ryantibs/median/quickselect.c
     if (!(nn >= 1)) {
         return NAN;
     }
-    const int kk = MAX(0, MIN(nn - 1, (const int) (pp * nn)));
-    // handle even-case
-    if ((0 < kk && kk + 1 <= nn) && (double) kk == (pp * nn)) {
-        return 0.5 * (quickselect(arr, nn, kk) + quickselect(arr, nn,
-                kk - 1));
-    }
-    // handle odd-case
-    return quickselect(arr, nn, kk);
+    double kmod = MAX(0, MIN(1, qq)) * (nn - 1);
+    const int kk = kmod;
+    kmod = fmod(kmod, 1);
+    return kmod == 0            //
+        ? quickselect(arr, nn, kk)      //
+        : (1 - kmod) * quickselect(arr, nn, kk) + kmod * quickselect(arr, nn,
+        kk + 1);
 }
 
-SQLMATH_FUNC static void sql_quantile_final(
+SQLMATH_FUNC static void sql2_quantile_final(
     sqlite3_context * context
 ) {
 // This function will aggregate kth-quantile element.
     // vec99 - init
-    VECTOR99_AGGREGATE_CONTEXT();
+    VECTOR99_AGGREGATE_CONTEXT(0);
     // vec99 - null-case
-    if (vec99->size <= 0) {
+    if (vec99->nbody == 0) {
         sqlite3_result_null(context);
         goto catch_error;
     }
-    sqlite3_result_double(context, quantile(vec99->buf, vec99->size,
-            vec99->arg0));
+    sqlite3_result_double(context, quantile(vec99_body, vec99->nbody,
+            vec99_head[0]));
   catch_error:
-    vector99_buf_free(vec99);
+    vector99_agg_free(vec99_agg);
 }
 
-static void sql_quantile_step0(
+static void sql2_quantile_step0(
     sqlite3_context * context,
     int argc,
     sqlite3_value ** argv,
-    const double pp
+    const double qq
 ) {
 // This function will aggregate kth-quantile element.
     UNUSED_PARAMETER(argc);
     // vec99 - init
-    VECTOR99_AGGREGATE_CONTEXT();
-    if (isnan(vec99->arg0)) {
-        vec99->arg0 = pp;       // kth-quantile
+    VECTOR99_AGGREGATE_CONTEXT(1);
+    if (vec99->nbody == 0) {
+        vec99_head[0] = qq;     // kth-quantile
     }
     // vec99 - append isfinite
     const double xx = sqlite3_value_double_or_nan(argv[0]);
     if (!isnan(xx)) {
-        const int errcode = vector99_push_back(vec99, xx);
+        const int errcode = vector99_push(vec99_agg, xx);
         SQLITE3_RESULT_ERROR_CODE(errcode);
     }
     return;
   catch_error:
-    vector99_buf_free(vec99);
+    vector99_agg_free(vec99_agg);
 }
 
-SQLMATH_FUNC static void sql_quantile_step(
+SQLMATH_FUNC static void sql2_quantile_step(
     sqlite3_context * context,
     int argc,
     sqlite3_value ** argv
 ) {
 // This function will aggregate kth-quantile element.
-    sql_quantile_step0(context, argc, argv, sqlite3_value_double(argv[1]));
+    sql2_quantile_step0(context, argc, argv, sqlite3_value_double(argv[1]));
 }
 
-SQLMATH_FUNC static void sql_median_final(
+SQLMATH_FUNC static void sql2_median_final(
     sqlite3_context * context
 ) {
-    sql_quantile_final(context);
+    sql2_quantile_final(context);
 }
 
-SQLMATH_FUNC static void sql_median_step(
+SQLMATH_FUNC static void sql2_median_step(
     sqlite3_context * context,
     int argc,
     sqlite3_value ** argv
 ) {
 // This function will aggregate kth-quantile element.
-    sql_quantile_step0(context, argc, argv, 0.5);
+    sql2_quantile_step0(context, argc, argv, 0.5);
 }
 
-// SQLMATH_FUNC sql_quantile_func - end
+// SQLMATH_FUNC sql2_quantile_func - end
+
+// SQLMATH_FUNC sql2_stdev_func - start
+typedef struct AggStdev {
+    double mxx;                 // average xx
+    double nnn;                 // number of elements
+    double sxx;                 // variance.p xx
+} AggStdev;
 
+SQLMATH_FUNC static void sql2_stdev_final(
+    sqlite3_context * context
+) {
+// This function will aggregate elements and calculate sample stdev.
+    // agg - init
+    SQLITE3_AGGREGATE_CONTEXT(AggStdev);
+    // agg - null-case
+    if (agg->nnn <= 0) {
+        sqlite3_result_null(context);
+        goto catch_error;
+    }
+    sqlite3_result_double(context,
+        agg->nnn == 1 ? 0 : sqrt(agg->sxx / (agg->nnn - 1)));
+  catch_error:
+    (void) 0;
+}
 
-SQLMATH_FUNC static void sql_roundorzero_func(
+static void sql2_stdev_step(
     sqlite3_context * context,
     int argc,
     sqlite3_value ** argv
 ) {
-// This function will round <argv>[0] to decimal <argv>[1].
+// This function will aggregate elements and calculate stdev.
     UNUSED_PARAMETER(argc);
-    if (sqlite3_value_numeric_type(argv[0]) == SQLITE_NULL) {
-        sqlite3_result_double(context, 0);
-        return;
+    // agg - init
+    SQLITE3_AGGREGATE_CONTEXT(AggStdev);
+    // agg - welford - increment agg->sxx
+    if (sqlite3_value_numeric_type(argv[0]) != SQLITE_NULL) {
+        const double xx = sqlite3_value_double(argv[0]);
+        const double dxx0 = xx - agg->mxx;
+        agg->nnn += 1;
+        agg->mxx += dxx0 / agg->nnn;
+        agg->sxx += dxx0 * (xx - agg->mxx);
     }
-    // declare var
-    char *zBuf = NULL;
-    double rr = sqlite3_value_double(argv[0]);
-    int nn = sqlite3_value_int(argv[1]);
-    nn = MIN(nn, 30);
-    nn = MAX(nn, 0);
-    // If YY==0 and XX will fit in a 64-bit int,
-    // handle the rounding directly,
-    // otherwise use printf.
-    if (rr < -4503599627370496.0 || rr > +4503599627370496.0) {
-    } else if (nn == 0) {
-        // The value has no fractional part so there is nothing to round
-        rr = (double) ((sqlite_int64) (rr + (rr < 0 ? -0.5 : +0.5)));
-    } else {
-        zBuf = sqlite3_mprintf("%.*f", nn, rr);
-        if (zBuf == NULL) {
-            sqlite3_result_error_nomem(context);
-            return;
+  catch_error:
+    (void) 0;
+}
+
+// SQLMATH_FUNC sql2_stdev_func - end
+
+// SQLMATH_FUNC sql2_vec_concat_func - start
+SQLMATH_FUNC static void sql2_vec_concat_final(
+    sqlite3_context * context
+) {
+// This function will concat rows of nCol doubles to a 2d-matrix.
+    // vec99 - init
+    VECTOR99_AGGREGATE_CONTEXT(0);
+    // vec99 - null-case
+    if (vec99->nbody == 0) {
+        sqlite3_result_null(context);
+        goto catch_error;
+    }
+    // debug
+    // fprintf(stderr, "\n");
+    // for (int ii = 0; ii < (int) vec99->nbody; ii += 1) {
+    //     fprintf(stderr, "vec_concat ii=%d xx=%f\n", ii, vec99_body[ii]);
+    // }
+    // vec99 - fill-forward
+    const int nn = (int) vec99->nbody;
+    for (int ii = 1; ii < nn; ii += 1) {
+        if (isnan(vec99_body[ii])) {
+            vec99_body[ii] = vec99_body[ii - 1];
+        }
+    }
+    // vec99 - fill-backward
+    for (int ii = nn - 2; ii >= 0; ii -= 1) {
+        if (isnan(vec99_body[ii])) {
+            vec99_body[ii] = vec99_body[ii + 1];
         }
-        rr = strtod(zBuf, NULL);
-        // cleanup sqlite3_mprintf()
-        sqlite3_free(zBuf);
     }
-    sqlite3_result_double(context, rr);
+    // vec99 - result
+    vector99_result_blob(vec99, context);
+    return;
+  catch_error:
+    vector99_agg_free(vec99_agg);
 }
 
-SQLMATH_FUNC static void sql_random1_func(
+SQLMATH_FUNC static void sql2_vec_concat_step(
     sqlite3_context * context,
     int argc,
     sqlite3_value ** argv
 ) {
-// This function will generate high-quality random-float between 0 <= xx < 1.
+// This function will concat argv[0] to carray of double
+    UNUSED_PARAMETER(argc);
+    // vec99 - init
+    VECTOR99_AGGREGATE_CONTEXT(0);
+    // vec99 - append double
+    const int errcode =
+        vector99_push(vec99_agg, sqlite3_value_double_or_nan(argv[0]));
+    SQLITE3_RESULT_ERROR_CODE(errcode);
+    return;
+  catch_error:
+    vector99_agg_free(vec99_agg);
+}
+
+// SQLMATH_FUNC sql2_vec_concat_func - end
+
+// SQLMATH_FUNC sql3_win_ema1_func - start
+SQLMATH_FUNC static void sql3_win_ema1_value(
+    sqlite3_context * context
+) {
+// This function will calculate running exponential-moving-average.
+    // vec99 - init
+    VECTOR99_AGGREGATE_CONTEXT(0);
+    sqlite3_result_double(context, vec99_body[(int) vec99->wii]);
+}
+
+SQLMATH_FUNC static void sql3_win_ema1_final(
+    sqlite3_context * context
+) {
+// This function will calculate running exponential-moving-average.
+    // vec99 - value
+    sql3_win_ema1_value(context);
+    // vec99 - init
+    VECTOR99_AGGREGATE_CONTEXT(0);
+    // vec99 - cleanup
+    vector99_agg_free(vec99_agg);
+}
+
+SQLMATH_FUNC static void sql3_win_ema1_inverse(
+    sqlite3_context * context,
+    int argc,
+    sqlite3_value ** argv
+) {
+// This function will calculate running exponential-moving-average.
     UNUSED_PARAMETER(argc);
     UNUSED_PARAMETER(argv);
-    static const double inv = 1.0 / 0x100000000;
-    uint32_t xx[1];
-    sqlite3_randomness(4, (void *) xx);
-    sqlite3_result_double(context, ((double) *xx) * inv);
+    // vec99 - init
+    VECTOR99_AGGREGATE_CONTEXT(0);
+    if (!vec99->wnn) {
+        vec99->wnn = vec99->nbody;
+    }
 }
 
-SQLMATH_FUNC static void sql_sign_func(
+SQLMATH_FUNC static void sql3_win_ema1_step(
     sqlite3_context * context,
     int argc,
     sqlite3_value ** argv
 ) {
-/*
-** Implementation of the sign() function
-** return one of 3 possibilities +1,0 or -1 when the argument is respectively
-** positive, 0 or negative.
-** When the argument is NULL the result is also NULL (completly conventional)
-*/
+// This function will calculate running exponential-moving-average.
+    if (argc < 2) {
+        sqlite3_result_error(context,
+            "wrong number of arguments to function win_ema2()", -1);
+        return;
+    }
+    // vec99 - init
+    const int ncol = argc - 1;
+    double arg_alpha = NAN;
+    VECTOR99_AGGREGATE_CONTEXT(argc);
+    if (vec99->nbody == 0) {
+        // ncol
+        vec99->ncol = ncol;
+        // arg_alpha
+        arg_alpha = sqlite3_value_double_or_nan(argv[argc - 1]);
+        if (isnan(arg_alpha)) {
+            sqlite3_result_error(context,
+                "invalid argument 'alpha' to function win_emax()", -1);
+            return;
+        }
+        vec99_head[ncol + 0] = arg_alpha;
+    }
+    // declare var
+    arg_alpha = vec99_head[ncol + 0];
+    const int nrow = vec99->nbody / ncol;
+    int errcode = 0;
+    // vec99 - calculate ema
+    for (int ii = 0; ii < ncol; ii += 1) {
+        sqlite3_value_double_or_prev(argv[ii], &vec99_head[ii]);
+        double *row = vec99_body + ii;
+        // debug
+        // fprintf(stderr,         //
+        //     "win_ema2 - nbody=%.0f xx0=%f xx=%f arg_alpha=%f\n",        //
+        //     vec99->nbody, *row, vec99_head[0], arg_alpha);
+        for (int jj = 0; jj < nrow; jj += 1) {
+            *row = arg_alpha * vec99_head[ii] + (1 - arg_alpha) * *row;
+            row += ncol;
+        }
+    }
+    // vec99 - push xx
+    for (int ii = 0; ii < ncol; ii += 1) {
+        errcode = vector99_push(vec99_agg, vec99_head[ii]);
+    }
+    SQLITE3_RESULT_ERROR_CODE(errcode);
+    return;
+  catch_error:
+    vector99_agg_free(vec99_agg);
+}
+
+// SQLMATH_FUNC sql3_win_ema1_func - end
+
+// SQLMATH_FUNC sql3_win_ema2_func - start
+SQLMATH_FUNC static void sql3_win_ema2_value(
+    sqlite3_context * context
+) {
+// This function will calculate running exponential-moving-average.
+    // vec99 - init
+    VECTOR99_AGGREGATE_CONTEXT(0);
+    if (!vec99->ncol) {
+        sqlite3_result_null(context);
+    }
+    int errcode = 0;
+    SQLITE3_RESULT_JSONFLOAT64ARRAY(str99, vec99_body + (int) vec99->wii,
+        (int) vec99->ncol);
+  catch_error:
+    (void) 0;
+}
+
+SQLMATH_FUNC static void sql3_win_ema2_final(
+    sqlite3_context * context
+) {
+// This function will calculate running exponential-moving-average.
+    // vec99 - value
+    sql3_win_ema2_value(context);
+    // vec99 - init
+    VECTOR99_AGGREGATE_CONTEXT(0);
+    // vec99 - cleanup
+    vector99_agg_free(vec99_agg);
+}
+
+SQLMATH_FUNC static void sql3_win_ema2_inverse(
+    sqlite3_context * context,
+    int argc,
+    sqlite3_value ** argv
+) {
+// This function will calculate running exponential-moving-average.
+    sql3_win_ema1_inverse(context, argc, argv);
+}
+
+SQLMATH_FUNC static void sql3_win_ema2_step(
+    sqlite3_context * context,
+    int argc,
+    sqlite3_value ** argv
+) {
+// This function will calculate running exponential-moving-average.
+    sql3_win_ema1_step(context, argc, argv);
+}
+
+// SQLMATH_FUNC sql3_win_ema2_func - end
+
+// SQLMATH_FUNC sql3_win_quantile1_func - start
+SQLMATH_FUNC static void sql3_win_quantile1_value(
+    sqlite3_context * context
+) {
+// This function will calculate running quantile.
+    // vec99 - init
+    VECTOR99_AGGREGATE_CONTEXT(0);
+    sqlite3_result_double(context, vec99_head[(int) vec99->ncol + 1]);
+}
+
+SQLMATH_FUNC static void sql3_win_quantile1_final(
+    sqlite3_context * context
+) {
+// This function will calculate running quantile.
+    // vec99 - value
+    sql3_win_quantile1_value(context);
+    // vec99 - init
+    VECTOR99_AGGREGATE_CONTEXT(0);
+    // vec99 - cleanup
+    vector99_agg_free(vec99_agg);
+}
+
+SQLMATH_FUNC static void sql3_win_quantile1_inverse(
+    sqlite3_context * context,
+    int argc,
+    sqlite3_value ** argv
+) {
+// This function will calculate running quantile.
     UNUSED_PARAMETER(argc);
-    switch (sqlite3_value_numeric_type(argv[0])) {
-    case SQLITE_INTEGER:
-    case SQLITE_FLOAT:
-        {
-            double rVal = sqlite3_value_double(argv[0]);
-            sqlite3_result_double(context,
-                (rVal > 0) ? 1 : (rVal < 0) ? -1 : 0);
+    UNUSED_PARAMETER(argv);
+    // vec99 - init
+    VECTOR99_AGGREGATE_CONTEXT(0);
+    if (!vec99->wnn) {
+        vec99->wnn = vec99->nbody;
+    }
+    // vec99 - invert
+    const int ncol = argc - 1;
+    const int nstep = ncol * 2;
+    const int nn = vec99->nbody - nstep;
+    double *arr = vec99_body + 1;
+    double *xx0 = vec99_body + 0 + (int) vec99->wii;
+    for (int ii = 0; ii < ncol; ii += 1) {
+        const double xx = *xx0;
+        int jj = 0;
+        for (; jj < nn && arr[jj] < xx; jj += nstep) {
+        }
+        for (; jj < nn; jj += nstep) {
+            arr[jj] = arr[jj + nstep];
         }
+        arr[jj] = INFINITY;
+        arr += 2;
+        xx0 += 2;
+    }
+}
+
+SQLMATH_FUNC static void sql3_win_quantile1_step(
+    sqlite3_context * context,
+    int argc,
+    sqlite3_value ** argv
+) {
+// This function will calculate running quantile.
+    if (argc < 2) {
+        sqlite3_result_error(context,
+            "wrong number of arguments to function win_quantile2()", -1);
         return;
     }
+    // vec99 - init
+    const int ncol = argc - 1;
+    double arg_quantile = NAN;
+    VECTOR99_AGGREGATE_CONTEXT(argc + ncol);
+    if (vec99->nbody == 0) {
+        // ncol
+        vec99->ncol = ncol;
+        // arg_quantile
+        arg_quantile = sqlite3_value_double_or_nan(argv[ncol + 0]);
+        if (!(0 <= arg_quantile && arg_quantile <= 1)) {
+            sqlite3_result_error(context,
+                "invalid argument 'quantile' to function win_quantilex()",
+                -1);
+            return;
+        }
+        vec99_head[ncol + 0] = arg_quantile;
+    }
+    // declare var
+    int errcode = 0;
+    // debug
+    // fprintf(stderr, "\n");
+    // vec99 - push xx
+    for (int ii = 0; ii < ncol; ii += 1) {
+        sqlite3_value_double_or_prev(argv[ii], &vec99_head[ii]);
+        VECTOR99_AGGREGATE_PUSH(vec99_head[ii]);
+        VECTOR99_AGGREGATE_PUSH(        //
+            vec99->wnn ? vec99_body[(int) vec99->wii] : INFINITY);
+    }
+    // vec99 - calculate quantile
+    const int nstep = ncol * 2;
+    const int nn = vec99->nbody / nstep;
+    double *arr = vec99_body + 1;
+    //
+    arg_quantile = vec99_head[ncol + 0] * (nn - 1);
+    const int kk1 = floor(arg_quantile) * nstep;
+    const int kk2 = kk1 + nstep;
+    arg_quantile = fmod(arg_quantile, 1);
+    for (int ii = 0; ii < ncol; ii += 1) {
+        const double xx = vec99_head[ii];
+        int jj = (nn - 2) * nstep;
+        for (; jj >= 0 && arr[jj] > xx; jj -= nstep) {
+            arr[jj + nstep] = arr[jj];
+        }
+        arr[jj + nstep] = xx;
+        vec99_head[ncol + 1 + ii] = arg_quantile == 0   //
+            ? arr[kk1]          //
+            : (1 - arg_quantile) * arr[kk1] + arg_quantile * arr[kk2];
+        // debug
+        // fprintf(stderr, "ii=%d arg=%f, xx0=%f\n",       //
+        //     ii, sqlite3_value_double_or_nan(argv[ii]), vec99_head[ii]);
+        // fprintf(stderr,         //
+        //     "win_quantile1 - nn=%d wii=%.0f kk1=%d kk2=%d"      //
+        //     " xx=%f qq=%f xx1=%f xx2=%f\n",     //
+        //     nn, vec99->wii, kk1, kk2,   //
+        //     xx, arg_quantile, arr[kk1], arr[kk2]);
+        arr += 2;
+    }
+    return;
+  catch_error:
+    vector99_agg_free(vec99_agg);
 }
 
-// SQLMATH_FUNC sql_stdev_func - start
-typedef struct StdevElem {
-    double exx;                 // stdev of xx
-    double mxx;                 // avg xx
-    double nnn;                 // number-of-samples
-} StdevElem;
+// SQLMATH_FUNC sql3_win_quantile1_func - end
 
-SQLMATH_API double stdev(
-    double *arr,
-    const int nn,
-    const double pp
+// SQLMATH_FUNC sql3_win_quantile2_func - start
+SQLMATH_FUNC static void sql3_win_quantile2_value(
+    sqlite3_context * context
 ) {
-// This function will find <pp>-th-stdev element in <arr>
-// using quickselect-algorithm.
-// https://www.stat.cmu.edu/~ryantibs/median/quickselect.c
-    if (nn <= 0) {
-        return 0;
-    }
-    const int kk = MAX(0, MIN(nn - 1, (const int) (pp * nn)));
-    // handle even-case
-    if ((0 < kk && kk + 1 <= nn) && (double) kk == (pp * nn)) {
-        return 0.5 * (quickselect(arr, nn, kk) + quickselect(arr, nn,
-                kk - 1));
-    }
-    // handle odd-case
-    return quickselect(arr, nn, kk);
-}
-
-SQLMATH_FUNC static void sql_stdev_final(
-    sqlite3_context * context
-) {
-// This function will aggregate kth-stdev element.
-    // pp - init
-    StdevElem *pp =
-        (StdevElem *) sqlite3_aggregate_context(context, sizeof(*pp));
-    SQLITE3_RESULT_ERROR_MALLOC(pp);
-    // pp - null-case
-    if (pp->nnn <= 0) {
+// This function will calculate running quantile.
+    // vec99 - init
+    VECTOR99_AGGREGATE_CONTEXT(0);
+    if (!vec99->ncol) {
         sqlite3_result_null(context);
-        goto catch_error;
     }
-    sqlite3_result_double(context,
-        pp->nnn == 1 ? 0 : sqrt(pp->exx / (pp->nnn - 1)));
+    int errcode = 0;
+    SQLITE3_RESULT_JSONFLOAT64ARRAY(str99, vec99_head + (int) vec99->ncol + 1,
+        (int) vec99->ncol);
   catch_error:
     (void) 0;
 }
 
-static void sql_stdev_step(
+SQLMATH_FUNC static void sql3_win_quantile2_final(
+    sqlite3_context * context
+) {
+// This function will calculate running quantile.
+    // vec99 - value
+    sql3_win_quantile2_value(context);
+    // vec99 - init
+    VECTOR99_AGGREGATE_CONTEXT(0);
+    // vec99 - cleanup
+    vector99_agg_free(vec99_agg);
+}
+
+SQLMATH_FUNC static void sql3_win_quantile2_inverse(
     sqlite3_context * context,
     int argc,
     sqlite3_value ** argv
 ) {
-// This function will aggregate kth-stdev element.
-    UNUSED_PARAMETER(argc);
-    // pp - init
-    StdevElem *pp =
-        (StdevElem *) sqlite3_aggregate_context(context, sizeof(*pp));
-    SQLITE3_RESULT_ERROR_MALLOC(pp);
-    // pp - welford - increment pp->exx
-    if (sqlite3_value_numeric_type(argv[0]) != SQLITE_NULL) {
-        const double xx = sqlite3_value_double(argv[0]);
-        const double dxx0 = xx - pp->mxx;
-        pp->nnn += 1;
-        pp->mxx += dxx0 / pp->nnn;
-        pp->exx += dxx0 * (xx - pp->mxx);
+// This function will calculate running quantile.
+    sql3_win_quantile1_inverse(context, argc, argv);
+}
+
+SQLMATH_FUNC static void sql3_win_quantile2_step(
+    sqlite3_context * context,
+    int argc,
+    sqlite3_value ** argv
+) {
+// This function will calculate running quantile.
+    sql3_win_quantile1_step(context, argc, argv);
+}
+
+// SQLMATH_FUNC sql3_win_quantile2_func - end
+
+// SQLMATH_FUNC sql3_win_slr2_func - start
+typedef struct WinSlrResult {
+    double nnn;                 // number of elements
+    double mxx;                 // average xx
+    double myy;                 // average yy
+    double exx;                 // stdev.s xx
+    double eyy;                 // stdev.s yy
+    double crr;                 // pearson xy
+    double cbb;                 // linest slope
+    double caa;                 // linest intercept
+} WinSlrResult;
+static const int WinSlrResultN = sizeof(WinSlrResult) / sizeof(double);
+
+typedef struct WinSlrStep {
+    double invp;                // 1.0 / nnn
+    double invs;                // 1.0 / (nnn - 1)
+    double mxx;                 // average xx
+    double myy;                 // average yy
+    double nnn;                 // number of elements
+    double sxx;                 // variance.p xx
+    double sxy;                 // covariance.p xy
+    double syy;                 // variance.p yy
+    double xx0;                 // previous xx
+    double yy0;                 // previous yy
+} WinSlrStep;
+static const int WinSlrStepN = sizeof(WinSlrStep) / sizeof(double);
+
+SQLMATH_FUNC static void sql3_win_slr2_value(
+    sqlite3_context * context
+) {
+// This function will calculate running simple-linear-regression.
+    // vec99 - init
+    VECTOR99_AGGREGATE_CONTEXT(0);
+    // declare var
+    const WinSlrStep *slr = (WinSlrStep *) vec99_head;
+    const int ncol = vec99->ncol;
+    double *result = vec99_head + ncol * WinSlrStepN;
+    int errcode = 0;
+    // calculate slr
+    for (int ii = 0; ii < ncol; ii += 1) {
+        const double mxx = slr->mxx;
+        const double myy = slr->myy;
+        const double exx = sqrt(slr->sxx * slr->invs);
+        const double eyy = sqrt(slr->syy * slr->invs);
+        const double crr = slr->sxy / sqrt(slr->sxx * slr->syy);
+        const double cbb = slr->sxy / slr->sxx;
+        const double caa = myy - cbb * mxx;
+        result[0] = slr->nnn;
+        result[1] = mxx;
+        result[2] = myy;
+        result[3] = exx;
+        result[4] = eyy;
+        result[5] = crr;
+        result[6] = cbb;
+        result[7] = caa;
+        result += WinSlrResultN;
+        slr += 1;
     }
+    // str99 - result
+    SQLITE3_RESULT_JSONFLOAT64ARRAY(str99, result - ncol * WinSlrResultN,
+        ncol * WinSlrResultN);
   catch_error:
     (void) 0;
 }
 
-// SQLMATH_FUNC sql_stdev_func - end
+SQLMATH_FUNC static void sql3_win_slr2_final(
+    sqlite3_context * context
+) {
+// This function will calculate running simple-linear-regression.
+    // vec99 - value
+    sql3_win_slr2_value(context);
+    // vec99 - init
+    VECTOR99_AGGREGATE_CONTEXT(0);
+    // vec99 - cleanup
+    vector99_agg_free(vec99_agg);
+}
 
-SQLMATH_FUNC static void sql_squared_func(
+SQLMATH_FUNC static void sql3_win_slr2_inverse(
     sqlite3_context * context,
     int argc,
     sqlite3_value ** argv
 ) {
-/*
-** Implementation of the squared() function
-** the argument is an integer.
-** Since SQLite isn't strongly typed (almost untyped actually) this is a bit pedantic
-*/
+// This function will calculate running simple-linear-regression.
     UNUSED_PARAMETER(argc);
-    switch (sqlite3_value_numeric_type(argv[0])) {
-    case SQLITE_INTEGER:
-    case SQLITE_FLOAT:
-        {
-            double rVal = sqlite3_value_double(argv[0]);
-            sqlite3_result_double(context, rVal * rVal);
-        }
-        return;
+    UNUSED_PARAMETER(argv);
+    // vec99 - init
+    VECTOR99_AGGREGATE_CONTEXT(0);
+    if (!vec99->wnn) {
+        vec99->wnn = vec99->nbody;
     }
 }
 
-SQLMATH_FUNC static void sql_throwerror_func(
+SQLMATH_FUNC static void sql3_win_slr2_step(
     sqlite3_context * context,
     int argc,
     sqlite3_value ** argv
 ) {
-// This function will return sqlite3_result_error_code(argv[0]).
-    UNUSED_PARAMETER(argc);
-    // declare var
-    int errcode = sqlite3_value_int(argv[0]);
-    if (0 <= errcode && errcode <= 28) {
-        sqlite3_result_error_code(context, errcode);
+// This function will calculate running simple-linear-regression.
+    if (argc < 2 || argc % 2) {
+        sqlite3_result_error(context,
+            "wrong number of arguments to function win_slr2()", -1);
         return;
     }
-    sqlite3_result_error_code(context, SQLITE_INTERNAL);
+    // vec99 - init
+    const int ncol = argc / 2;
+    VECTOR99_AGGREGATE_CONTEXT(ncol * (WinSlrStepN + WinSlrResultN));
+    if (vec99->nbody == 0) {
+        // ncol
+        vec99->ncol = ncol;
+    }
+    // declare var
+    WinSlrStep *slr = (WinSlrStep *) vec99_head;
+    const double *xxyy0 = vec99_body + (int) vec99->wii;
+    int errcode = 0;
+    // debug
+    // fprintf(stderr, "\n");
+    // vec99 - calculate slr
+    for (int ii = 0; ii < ncol; ii += 1) {
+        // debug
+        // fprintf(stderr, "ii=%d argv0=%f, xx0=%f mxx=%f pp=%p\n",        //
+        //     ii, sqlite3_value_double_or_nan(argv[0]), slr->xx0, slr->mxx,
+        //     slr);
+        const double xx = sqlite3_value_double_or_prev(argv[0], &slr->xx0);
+        const double yy = sqlite3_value_double_or_prev(argv[1], &slr->yy0);
+        double mxx = slr->mxx;
+        double myy = slr->myy;
+        double sxx = slr->sxx;
+        double sxy = slr->sxy;
+        double syy = slr->syy;
+        // vec99 - calculate slr
+        if (vec99->wnn) {
+            // calculate running slr - window
+            const double invp = slr->invp;
+            const double xx0 = xxyy0[0];
+            const double yy0 = xxyy0[1];
+            const double dx = xx - xx0;
+            const double dy = yy - yy0;
+            sxx += (xx * xx - xx0 * xx0) - invp * dx * dx - 2 * dx * mxx;
+            sxy +=
+                (xx * yy - xx0 * yy0) - invp * dx * dy - mxx * dy - dx * myy;
+            syy += (yy * yy - yy0 * yy0) - invp * dy * dy - 2 * dy * myy;
+            mxx += dx * invp;
+            myy += dy * invp;
+            // debug
+            // fprintf(stderr,     //
+            //     "win_slr2 - wnn=%.0f wii=%.0f xx,yy=%f,%f xx0,yy0=%f,%f\n",
+            //     vec99->wnn, vec99->wii, xx, yy, xx0, yy0);
+        } else {
+            // calculate running slr - welford
+            double dd;
+            slr->invp = 1.0 / (slr->nnn + 1);
+            slr->invs = 1.0 / (slr->nnn + 0);
+            slr->nnn += 1;
+            // welford - increment syy
+            dd = yy - myy;
+            myy += dd * slr->invp;
+            syy += dd * (yy - myy);
+            // welford - increment sxx
+            dd = xx - mxx;
+            mxx += dd * slr->invp;
+            sxx += dd * (xx - mxx);
+            // welford - increment sxy
+            sxy += dd * (yy - myy);
+            // debug
+            // fprintf(stderr,     //
+            //     "win_slr2 - nbody=%.0f xx,yy=%f,%f\n",  //
+            //     vec99->nbody, xx, yy);
+        }
+        slr->mxx = mxx;
+        slr->myy = myy;
+        slr->sxx = sxx;
+        slr->sxy = sxy;
+        slr->syy = syy;
+        // debug
+        // fprintf(stderr, "ii=%d argv0=%f, xx0=%f mxx=%f pp=%p\n",        //
+        //     ii, sqlite3_value_double_or_nan(argv[0]), slr->xx0, slr->mxx,
+        //     slr);
+        // increment counter
+        argv += 2;
+        slr += 1;
+        xxyy0 += 2;
+    }
+    slr -= ncol;
+    // vec99 - push xx
+    for (int ii = 0; ii < ncol; ii += 1) {
+        errcode = vector99_push(vec99_agg, slr->xx0);
+        errcode = vector99_push(vec99_agg, slr->yy0);
+        slr += 1;
+    }
+    SQLITE3_RESULT_ERROR_CODE(errcode);
+    return;
+  catch_error:
+    vector99_agg_free(vec99_agg);
 }
 
+// SQLMATH_FUNC sql3_win_slr2_func - end
 
 // file sqlmath_base - init
 int sqlite3_sqlmath_base_init(
     sqlite3 * db,
     char **pzErrMsg,
     const sqlite3_api_routines * pApi
 ) {
     UNUSED_PARAMETER(pApi);
     UNUSED_PARAMETER(pzErrMsg);
     int errcode = 0;
     SQLITE3_CREATE_FUNCTION1(btobase64, 1);
     SQLITE3_CREATE_FUNCTION1(btotext, 1);
+    SQLITE3_CREATE_FUNCTION1(castrealornull, 1);
     SQLITE3_CREATE_FUNCTION1(castrealorzero, 1);
     SQLITE3_CREATE_FUNCTION1(casttextorempty, 1);
     SQLITE3_CREATE_FUNCTION1(copyblob, 1);
     SQLITE3_CREATE_FUNCTION1(cot, 1);
     SQLITE3_CREATE_FUNCTION1(coth, 1);
     SQLITE3_CREATE_FUNCTION1(jenks_blob, 2);
     SQLITE3_CREATE_FUNCTION1(jenks_json, 2);
@@ -2110,35 +2647,39 @@
     SQLITE3_CREATE_FUNCTION1(squared, 1);
     SQLITE3_CREATE_FUNCTION1(throwerror, 1);
     SQLITE3_CREATE_FUNCTION2(jenks_concat, -1);
     SQLITE3_CREATE_FUNCTION2(matrix2d_concat, -1);
     SQLITE3_CREATE_FUNCTION2(median, 1);
     SQLITE3_CREATE_FUNCTION2(quantile, 2);
     SQLITE3_CREATE_FUNCTION2(stdev, 1);
-    SQLITE3_CREATE_FUNCTION3(avg_ema, 2);
+    SQLITE3_CREATE_FUNCTION2(vec_concat, 1);
+    SQLITE3_CREATE_FUNCTION3(win_ema1, 2);
+    SQLITE3_CREATE_FUNCTION3(win_ema2, -1);
+    SQLITE3_CREATE_FUNCTION3(win_quantile1, 2);
+    SQLITE3_CREATE_FUNCTION3(win_quantile2, -1);
+    SQLITE3_CREATE_FUNCTION3(win_slr2, -1);
     errcode =
         sqlite3_create_function(db, "random1", 0,
-        SQLITE_DIRECTONLY | SQLITE_UTF8, NULL, sql_random1_func, NULL, NULL);
+        SQLITE_DIRECTONLY | SQLITE_UTF8, NULL, sql1_random1_func, NULL, NULL);
     if (errcode != SQLITE_OK) {
         return errcode;
     }
     return 0;
 }
 #endif                          // SQLMATH_BASE_C3
 /*
 file sqlmath_base - end
 */
 
 
 /*
 file sqlmath_nodejs - start
 */
-#ifdef SQLMATH_NODEJS_C2
-//!! #if defined(SQLMATH_NODEJS_C2) && !defined(SQLMATH_NODEJS_C3)
-//!! #define SQLMATH_NODEJS_C3
+#if defined(SQLMATH_NODEJS_C2) && !defined(SQLMATH_NODEJS_C3)
+#define SQLMATH_NODEJS_C3
 
 
 #ifdef WIN32
 #include <windows.h>
 #endif
```

### Comparing `sqlmath-2023.5.25/sqlmath_browser.mjs` & `sqlmath-2023.6.26/sqlmath_browser.mjs`

 * *Files identical despite different names*

### Comparing `sqlmath-2023.5.25/sqlmath_custom.c` & `sqlmath-2023.6.26/sqlmath_custom.c`

 * *Files identical despite different names*

### Comparing `sqlmath-2023.5.25/sqlmath_jenks.c` & `sqlmath-2023.6.26/sqlmath_jenks.c`

 * *Files identical despite different names*

### Comparing `sqlmath-2023.5.25/sqlmath_wrapper_wasm.js` & `sqlmath-2023.6.26/sqlmath_wrapper_wasm.js`

 * *Files identical despite different names*

### Comparing `sqlmath-2023.5.25/test.mjs` & `sqlmath-2023.6.26/test.mjs`

 * *Files 22% similar despite different names*

```diff
@@ -43,14 +43,15 @@
     fsReadFileUnlessTest,
     fsWriteFileUnlessTest,
     jsbatonValueString,
     noop,
     sqlmathWebworkerInit,
     version
 } from "./sqlmath.mjs";
+let VECTOR99_NOFFSET = 6;
 let {
     assertErrorThrownAsync,
     jstestDescribe,
     jstestIt
 } = jslint;
 noop(debugInline);
 
@@ -731,134 +732,23 @@
             [27, "notification message"],
             [28, "warning message"],
             [100, "unknown error"],
             [101, "unknown error"]
         ].map(async function ([
             errno, errmsg
         ]) {
-            await assertErrorThrownAsync(async function () {
-                return await dbExecAsync({
+            await assertErrorThrownAsync(function () {
+                return dbExecAsync({
                     db,
                     sql: `SELECT throwerror(${errno})`
                 });
             }, errmsg);
         }));
     });
     jstestIt((
-        "test sqlite-extension-avg_ema handling-behavior"
-    ), async function test_sqlite_extension_avg_ema() {
-        let db = await dbOpenAsync({filename: ":memory:"});
-        let result;
-        result = await dbExecAsync({
-            db,
-            sql: (`
-SELECT
-    ROUND(
-        avg_ema(val, 2 * 1.0 / (4 + 1)) OVER ( -- alpha=0.4000
-            ORDER BY id ASC
-            ROWS BETWEEN 0 PRECEDING AND 4-1 FOLLOWING
-        ),
-        4
-    ) AS val
-    FROM (
-        SELECT 11 AS id, NULL AS val
-        UNION ALL SELECT 10,   10
-        UNION ALL SELECT  9,    9
-        UNION ALL SELECT  8,    8
-        UNION ALL SELECT  7,    7
-        UNION ALL SELECT  6,    6
-        UNION ALL SELECT  5,    5
-        UNION ALL SELECT  4,    4
-        UNION ALL SELECT  3,    3
-        UNION ALL SELECT  2,    2
-        UNION ALL SELECT  1,    1
-        UNION ALL SELECT  0, NULL
-    );
-            `)
-        });
-        result = result[0].map(function ({val}) {
-            return val;
-        });
-        assertJsonEqual(result, [
-            1.824, 2.824, 3.824, 4.824,
-            5.824, 6.824, 7.824, 8.824,
-            5.424, 5.640, 6.000, 0.000
-        ]);
-        result = await dbExecAsync({
-            db,
-            sql: (`
-SELECT
-    ROUND(
-        avg_ema(val, 2 * 1.0 / (4 + 1)) OVER ( -- alpha=0.4000
-            ORDER BY id ASC
-            ROWS BETWEEN 3 - 1 PRECEDING AND 2 - 1 FOLLOWING
-        ),
-        4
-    ) AS val
-    FROM (
-        SELECT 11 AS id, NULL AS val
-        UNION ALL SELECT 10,   10
-        UNION ALL SELECT  9,    9
-        UNION ALL SELECT  8,    8
-        UNION ALL SELECT  7,    7
-        UNION ALL SELECT  6,    6
-        UNION ALL SELECT  5,    5
-        UNION ALL SELECT  4,    4
-        UNION ALL SELECT  3,    3
-        UNION ALL SELECT  2,    2
-        UNION ALL SELECT  1,    1
-        UNION ALL SELECT  0, NULL
-    );
-            `)
-        });
-        result = result[0].map(function ({val}) {
-            return val;
-        });
-        assertJsonEqual(result, [
-            0.400, 1.040, 1.824, 2.824,
-            3.824, 4.824, 5.824, 6.824,
-            7.824, 8.824, 5.424, 5.640
-        ]);
-        result = await dbExecAsync({
-            db,
-            sql: (`
-SELECT
-    ROUND(
-        avg_ema(val, 2 * 1.0 / (4 + 1)) OVER ( -- alpha=0.4000
-            ORDER BY id ASC
-            ROWS BETWEEN 4 - 1 PRECEDING AND 0 FOLLOWING
-        ),
-        4
-    ) AS val
-    FROM (
-        SELECT 11 AS id, NULL AS val
-        UNION ALL SELECT 10,   10
-        UNION ALL SELECT  9,    9
-        UNION ALL SELECT  8,    8
-        UNION ALL SELECT  7,    7
-        UNION ALL SELECT  6,    6
-        UNION ALL SELECT  5,    5
-        UNION ALL SELECT  4,    4
-        UNION ALL SELECT  3,    3
-        UNION ALL SELECT  2,    2
-        UNION ALL SELECT  1,    1
-        UNION ALL SELECT  0, NULL
-    );
-            `)
-        });
-        result = result[0].map(function ({val}) {
-            return val;
-        });
-        assertJsonEqual(result, [
-            0.000, 0.400, 1.040, 1.824,
-            2.824, 3.824, 4.824, 5.824,
-            6.824, 7.824, 8.824, 5.424
-        ]);
-    });
-    jstestIt((
         "test sqlite-extension-base64 handling-behavior"
     ), async function test_sqlite_extension_base64() {
         let db = await dbOpenAsync({
             filename: ":memory:"
         });
         await Promise.all([
             {
@@ -1238,90 +1128,102 @@
     ), async function test_sqlite_extension_math() {
         let db = await dbOpenAsync({
             filename: ":memory:"
         });
         // test sqlmath-defined-func handling-behavior
         Object.entries({
             "''": {
+                "castrealornull": 0,
                 "castrealorzero": 0,
                 "casttextorempty": "",
                 "copyblob": ""
             },
             "'-0.5'": {
+                "castrealornull": -0.5,
                 "castrealorzero": -0.5,
                 "casttextorempty": "-0.5",
                 "copyblob": "-0.5"
             },
             "'-1'": {
+                "castrealornull": -1,
                 "castrealorzero": -1,
                 "casttextorempty": "-1",
                 "copyblob": "-1",
                 "cot": -0.642092615934331,
                 "coth": -1.31303528549933,
                 "sign": -1
             },
             "'0'": {
+                "castrealornull": 0,
                 "castrealorzero": 0,
                 "casttextorempty": "0",
                 "copyblob": "0",
                 "cot": null,
                 "coth": null,
                 "sign": 0
             },
             "'0.5'": {
+                "castrealornull": 0.5,
                 "castrealorzero": 0.5,
                 "casttextorempty": "0.5",
                 "copyblob": "0.5"
             },
             "'1'": {
+                "castrealornull": 1,
                 "castrealorzero": 1,
                 "casttextorempty": "1",
                 "copyblob": "1",
                 "cot": 0.642092615934331,
                 "coth": 1.31303528549933,
                 "sign": 1
             },
             "'aa'": {
+                "castrealornull": 0,
                 "castrealorzero": 0,
                 "casttextorempty": "aa",
                 "copyblob": "aa"
             },
             "'hello'": {
+                "castrealornull": 0,
                 "castrealorzero": 0,
                 "casttextorempty": "hello",
                 "copyblob": "hello"
             },
             "-0.5": {
+                "castrealornull": -0.5,
                 "castrealorzero": -0.5,
                 "casttextorempty": "-0.5",
                 "copyblob": -0.5
             },
             "-0x7fffffffffffffff": {
                 "sign": -1
             },
             "-1": {
+                "castrealornull": -1,
                 "castrealorzero": -1,
                 "casttextorempty": "-1",
                 "copyblob": -1,
                 "cot": -0.642092615934331,
                 "coth": -1.31303528549933,
                 "sign": -1
             },
             "-1e999": {
                 "sign": -1
             },
             "0": {
+                "castrealornull": 0,
                 "castrealorzero": 0,
                 "casttextorempty": "0",
                 "copyblob": 0,
                 "cot": null,
                 "coth": null,
                 "sign": 0
             },
             "0.5": {
+                "castrealornull": 0.5,
                 "castrealorzero": 0.5,
                 "casttextorempty": "0.5",
                 "copyblob": 0.5
             },
             "0.5, 0.5": {
                 "roundorzero": 1
             },
@@ -1337,25 +1239,29 @@
             "0x8000000000000000": {
                 "sign": -1
             },
             "0xffffffffffffffff": {
                 "sign": -1
             },
             "1": {
+                "castrealornull": 1,
                 "castrealorzero": 1,
                 "casttextorempty": "1",
                 "copyblob": 1,
                 "cot": 0.642092615934331,
                 "coth": 1.31303528549933,
                 "sign": 1
             },
             "1e999": {
+                "castrealornull": null,
+                "castrealorzero": 0,
                 "sign": 1
             },
             "null": {
+                "castrealornull": null,
                 "castrealorzero": 0,
                 "casttextorempty": "",
                 "copyblob": null,
                 "cot": null,
                 "coth": null,
                 "sign": null
             },
@@ -1365,19 +1271,21 @@
             "null, 0.5": {
                 "roundorzero": 0
             },
             "null, null": {
                 "roundorzero": 0
             },
             "zeroblob(0)": {
+                "castrealornull": 0,
                 "castrealorzero": 0,
                 "casttextorempty": "",
                 "copyblob": null
             },
             "zeroblob(1)": {
+                "castrealornull": 0,
                 "castrealorzero": 0,
                 "casttextorempty": "",
                 "copyblob": null
             }
         }).forEach(function ([
             arg, funcDict
         ]) {
@@ -1427,15 +1335,14 @@
         UNION ALL SELECT '12.34'
         UNION ALL SELECT 'abcd'
         UNION ALL SELECT 12.34
         UNION ALL SELECT zeroblob(0)
         UNION ALL SELECT zeroblob(1)
         UNION ALL SELECT NULL
     );
-
                 `),
                 [
                     7, 2,
                     0, 0,
                     12.34, 12.34,
                     0, 0,
                     12.34, 12.34,
@@ -1499,21 +1406,21 @@
                 [[undefined, undefined, 1, 1, 2, 3, 4], 0.5, 2],
                 [[undefined, undefined, 1, 2, 3, 4], 0.5, 2.5],
                 [[undefined], 0.5, undefined]
             ],
             [
                 [[], -99, 1],
                 [[], 0, 1],
-                [[], 0.125, 1.5],
-                [[], 0.250, 2.5],
-                [[], 0.375, 3.5],
+                [[], 0.125, 1.875],
+                [[], 0.250, 2.75],
+                [[], 0.375, 3.625],
                 [[], 0.500, 4.5],
-                [[], 0.625, 5.5],
-                [[], 0.750, 6.5],
-                [[], 0.875, 7.5],
+                [[], 0.625, 5.375],
+                [[], 0.750, 6.25],
+                [[], 0.875, 7.125],
                 [[], 1, 8],
                 [[], 99, 8],
                 [[0.1], 0, 0.1],
                 [[1.1], 0.125, 1.1],
                 [[2.1], 0.250, 2.1],
                 [[3.1], 0.375, 3.1],
                 [[4.1], 0.500, 4.1],
@@ -1566,21 +1473,23 @@
             data2.forEach(function (elem) {
                 avg += elem;
             });
             avg *= 1 / data2.length;
             data2.forEach(function (elem) {
                 valExpectedStd += (elem - avg) ** 2;
             });
-            valExpectedStd = Math.round(1_000_000 * (
+            valExpectedStd = (
                 data2.length <= 0
-                ? undefined
+                ? null
                 // : data2.length === 1
                 // ? 0
-                : Math.sqrt(valExpectedStd / (data2.length - 1))
-            ));
+                : Number(Math.sqrt(
+                    valExpectedStd / (data2.length - 1)
+                ).toFixed(8))
+            );
             await Promise.all([
                 data,
                 Array.from(data).reverse()
             ].map(async function (data) {
                 let valActual;
                 valActual = noop(
                     await dbExecAsync({
@@ -1588,15 +1497,15 @@
                             tmp1: JSON.stringify(data)
                         },
                         db,
                         sql: (`
 SELECT
         median(value) AS mdn,
         quantile(value, ${kk}) AS qnt,
-        ROUND(1000000 * stdev(value)) AS std
+        ROUND(stdev(value), 8) AS std
     FROM JSON_EACH($tmp1);
 -- test null-case handling-behavior
 SELECT quantile(value, ${kk}) AS qnt FROM JSON_EACH($tmp1) WHERE 0;
                         `)
                     })
                 )[0][0];
                 assertJsonEqual(
@@ -1614,14 +1523,823 @@
                         valExpectedMdn,
                         valExpectedStd
                     }
                 );
             }));
         }));
     });
+    jstestIt((
+        "test sqlite-extension-vec_concat handling-behavior"
+    ), async function test_sqlite_extension_vec_concat() {
+        let db = await dbOpenAsync({
+            filename: ":memory:"
+        });
+        await Promise.all([
+            [
+                (`
+SELECT vec_concat(NULL);
+                `),
+                [null]
+            ],
+            [
+                (`
+SELECT vec_concat(NULL) FROM (SELECT 1 UNION ALL SELECT 2);
+                `),
+                [null, null]
+            ],
+            [
+                (`
+SELECT
+        vec_concat(aa)
+    FROM (
+        SELECT NULL AS aa
+        UNION ALL SELECT '12.34'
+        UNION ALL SELECT NULL
+        UNION ALL SELECT 43.21
+        UNION ALL SELECT NULL
+        UNION ALL SELECT NULL
+        UNION ALL SELECT NULL
+    );
+                `),
+                [
+                    12.34,
+                    12.34,
+                    12.34,
+                    43.21,
+                    43.21,
+                    43.21,
+                    43.21
+                ]
+            ]
+        ].map(async function ([
+            sql, valExpected
+        ], ii) {
+            let valActual = Array.from(new Float64Array(
+                await dbExecAndReturnLastBlobAsync({
+                    db,
+                    sql
+                })
+            )).slice(VECTOR99_NOFFSET);
+            assertJsonEqual(valActual, valExpected, {
+                ii,
+                sql,
+                valActual,
+                valExpected
+            });
+        }));
+    });
+    jstestIt((
+        "test sqlite-extension-win_emax handling-behavior"
+    ), async function test_sqlite_extension_win_emax() {
+        let db = await dbOpenAsync({filename: ":memory:"});
+        let valIn;
+        async function test_win_emax_aggregate({
+            aa,
+            bb,
+            valExpected,
+            valExpected2
+        }) {
+            let alpha = 2 * 1.0 / (4 + 1);
+            let sqlBetween = "";
+            let valActual;
+            if (aa !== undefined) {
+                sqlBetween = (
+                    `ROWS BETWEEN ${aa - 1} PRECEDING AND ${bb} FOLLOWING`
+                );
+            }
+            // test win_ema1-aggregate handling-behavior
+            valActual = await dbExecAsync({
+                bindList: {
+                    valIn: JSON.stringify(valIn)
+                },
+                db,
+                sql: (`
+SELECT
+        win_ema1(value->>1, ${alpha}) OVER (
+            ORDER BY value->>0 ASC
+            ${sqlBetween}
+        ) AS val
+    FROM JSON_EAcH($valIn);
+                `)
+            });
+            valActual = valActual[0].map(function ({val}) {
+                return Number(val.toFixed(4));
+            });
+            assertJsonEqual(valActual, valExpected);
+            // test win_ema2-aggregate handling-behavior
+            valActual = await dbExecAsync({
+                bindList: {
+                    valIn: JSON.stringify(valIn)
+                },
+                db,
+                sql: (`
+SELECT
+        id,
+        win_ema2(
+            value->>1,
+            IIF(id = 1, -1, value->>1),
+            ${alpha}
+        ) OVER (
+            ORDER BY value->>0 ASC
+            ${sqlBetween}
+        ) AS val
+    FROM JSON_EAcH($valIn);
+                `)
+            });
+            valActual = valActual[0].map(function ({val}, ii, list) {
+                val = JSON.parse(val).map(function (elem) {
+                    return Number(elem.toFixed(4));
+                });
+                if (ii + (bb || 0) + 1 >= list.length) {
+                    assertJsonEqual(val[1], valExpected2, valActual);
+                } else {
+                    assertJsonEqual(val[1], val[0], valActual);
+                }
+                return val[0];
+            });
+            assertJsonEqual(valActual, valExpected);
+        }
+        valIn = [
+            [11, NaN],
+            [10, "10"],
+            [9, 9],
+            [8, "8"],
+            [7, 7],
+            [6, 6],
+            [5, Infinity],
+            [4, "4"],
+            [3, 3],
+            [2, 2],
+            [1, "1"],
+            [0, undefined]
+        ];
+        await Promise.all([
+            (async function () {
+                let valActual;
+                // test win_ema2-error handling-behavior
+                await assertErrorThrownAsync(function () {
+                    return dbExecAsync({
+                        db,
+                        sql: (`
+SELECT win_ema2(1) FROM (SELECT 1);
+                        `)
+                    });
+                }, "wrong number of arguments");
+                await assertErrorThrownAsync(function () {
+                    return dbExecAsync({
+                        db,
+                        sql: (`
+SELECT win_ema2(1, NULL) FROM (SELECT 1);
+                        `)
+                    });
+                }, "invalid argument 'alpha'");
+                // test win_ema1-null-case handling-behavior
+                valActual = await dbExecAsync({
+                    db,
+                    sql: (`
+DROP TABLE IF EXISTS __tmp1;
+CREATE TEMP TABLE __tmp1 (val REAL);
+SELECT win_ema1(1, 1) FROM __tmp1;
+                    `)
+                });
+                valActual = valActual[0].map(function ({val}) {
+                    return val;
+                });
+                assertJsonEqual(valActual, [null]);
+                // test win_ema2-null-case handling-behavior
+                valActual = await dbExecAsync({
+                    db,
+                    sql: (`
+DROP TABLE IF EXISTS __tmp1;
+CREATE TEMP TABLE __tmp1 (val REAL);
+SELECT win_ema2(1, 2, 3) FROM __tmp1;
+                    `)
+                });
+                valActual = valActual[0].map(function ({val}) {
+                    return val;
+                });
+                assertJsonEqual(valActual, [null]);
+            }()),
+            // test win_emax-aggregate-normal handling-behavior
+            test_win_emax_aggregate({
+                valExpected: [
+                    0.0000, 0.4000, 1.0400, 1.8240,
+                    2.6944, 3.2166, 4.3300, 5.3980,
+                    6.4388, 7.4633, 8.4780, 9.0868
+                ],
+                valExpected2: 4.6868
+            }),
+            // test win_emax-aggregate-window handling-behavior
+            test_win_emax_aggregate({
+                aa: 1,
+                bb: 3,
+                valExpected: [
+                    1.824, 2.824, 3.424, 4.584,
+                    5.680, 6.608, 7.824, 8.824,
+                    9.424, 9.424, 9.424, 9.424
+                ],
+                valExpected2: 5.024
+            }),
+            test_win_emax_aggregate({
+                aa: 3,
+                bb: 1,
+                valExpected: [
+                    0.400, 1.040, 1.824, 2.824,
+                    3.424, 4.584, 5.680, 6.608,
+                    7.824, 8.824, 9.424, 9.424
+                ],
+                valExpected2: 5.024
+            }),
+            test_win_emax_aggregate({
+                aa: 4,
+                bb: 0,
+                valExpected: [
+                    0.000, 0.400, 1.040, 1.824,
+                    2.824, 3.424, 4.584, 5.680,
+                    6.608, 7.824, 8.824, 9.424
+                ],
+                valExpected2: 5.024
+            })
+        ]);
+    });
+    jstestIt((
+        "test sqlite-extension-win_quantilex handling-behavior"
+    ), async function test_sqlite_extension_win_quantilex() {
+        let db = await dbOpenAsync({filename: ":memory:"});
+        let valIn;
+        async function test_win_quantilex_aggregate({
+            aa,
+            bb,
+            quantile,
+            valExpected,
+            valExpected2
+        }) {
+            let sqlBetween = "";
+            let valActual;
+            if (aa !== undefined) {
+                sqlBetween = (
+                    `ROWS BETWEEN ${aa - 1} PRECEDING AND ${bb} FOLLOWING`
+                );
+            }
+            // test win_quantile1-aggregate handling-behavior
+            valActual = await dbExecAsync({
+                bindList: {
+                    valIn: JSON.stringify(valIn)
+                },
+                db,
+                sql: (`
+SELECT
+        win_quantile1(value->>1, ${quantile}) OVER (
+            ORDER BY value->>0 ASC
+            ${sqlBetween}
+        ) AS val
+    FROM JSON_EAcH($valIn);
+                `)
+            });
+            valActual = valActual[0].map(function ({val}) {
+                return Number(val.toFixed(4));
+            });
+            assertJsonEqual(valActual, valExpected);
+            // test win_quantile2-aggregate handling-behavior
+            valActual = await dbExecAsync({
+                bindList: {
+                    valIn: JSON.stringify(valIn)
+                },
+                db,
+                sql: (`
+SELECT
+        id,
+        win_quantile2(
+            value->>1,
+            IIF(id = 34, -1, value->>1),
+            ${quantile}
+        ) OVER (
+            ORDER BY value->>0 ASC
+            ${sqlBetween}
+        ) AS val
+    FROM JSON_EAcH($valIn);
+                `)
+            });
+            valActual = valActual[0].map(function ({val}, ii) {
+                val = JSON.parse(val).map(function (elem) {
+                    return Number(elem.toFixed(4));
+                });
+                if (ii === 11) {
+                    assertJsonEqual(val[1], valExpected2, valActual);
+                } else {
+                    assertJsonEqual(val[1], val[0], valActual);
+                }
+                return val[0];
+            });
+            assertJsonEqual(valActual, valExpected);
+        }
+        valIn = [
+            [1, undefined],
+            [2, "1"],
+            [3, "2"],
+            [4, 3],
+            [5, 4],
+            [6, "abcd"],
+            [7, 6],
+            [8, NaN],
+            [9, 8],
+            [10, 9],
+            [11, 10],
+            [12, 11]
+        ];
+        await Promise.all([
+            (async function () {
+                let valActual;
+                // test win_quantile2-error handling-behavior
+                await assertErrorThrownAsync(function () {
+                    return dbExecAsync({
+                        db,
+                        sql: (`
+SELECT win_quantile2(1) FROM (SELECT 1);
+                        `)
+                    });
+                }, "wrong number of arguments");
+                await assertErrorThrownAsync(function () {
+                    return dbExecAsync({
+                        db,
+                        sql: (`
+SELECT win_quantile2(1, NULL) FROM (SELECT 1);
+                        `)
+                    });
+                }, "invalid argument 'quantile'");
+                // test win_quantile1-null-case handling-behavior
+                valActual = await dbExecAsync({
+                    db,
+                    sql: (`
+DROP TABLE IF EXISTS __tmp1;
+CREATE TEMP TABLE __tmp1 (val REAL);
+SELECT win_quantile1(1, 1) FROM __tmp1;
+                    `)
+                });
+                valActual = valActual[0].map(function ({val}) {
+                    return val;
+                });
+                assertJsonEqual(valActual, [null]);
+                // test win_quantile2-null-case handling-behavior
+                valActual = await dbExecAsync({
+                    db,
+                    sql: (`
+DROP TABLE IF EXISTS __tmp1;
+CREATE TEMP TABLE __tmp1 (val REAL);
+SELECT win_quantile2(1, 2, 3) FROM __tmp1;
+                    `)
+                });
+                valActual = valActual[0].map(function ({val}) {
+                    return val;
+                });
+                assertJsonEqual(valActual, [null]);
+            }()),
+            // test win_quantilex-aggregate-normal handling-behavior
+            test_win_quantilex_aggregate({
+                quantile: 0,
+                valExpected: [
+                    0.0000, 0.0000, 0.0000, 0.0000,
+                    0.0000, 0.0000, 0.0000, 0.0000,
+                    0.0000, 0.0000, 0.0000, 0.0000
+                ],
+                valExpected2: -1
+            }),
+            test_win_quantilex_aggregate({
+                quantile: 0.25,
+                valExpected: [
+                    0.0000, 0.2500, 0.5000, 0.7500,
+                    1.0000, 0.2500, 0.5000, 0.7500,
+                    1.0000, 1.2500, 1.5000, 1.7500
+                ],
+                valExpected2: 0.7500
+            }),
+            test_win_quantilex_aggregate({
+                quantile: 0.33333333,
+                valExpected: [
+                    0.0000, 0.3333, 0.6667, 1.0000,
+                    1.3333, 0.6667, 1.0000, 1.3333,
+                    1.6667, 2.0000, 2.3333, 2.6667
+                ],
+                valExpected2: 1.6667
+            }),
+            test_win_quantilex_aggregate({
+                quantile: 0.5,
+                valExpected: [
+                    0.0000, 0.5000, 1.0000, 1.5000,
+                    2.0000, 1.5000, 2.0000, 2.5000,
+                    3.0000, 3.5000, 4.0000, 5.0000
+                ],
+                valExpected2: 3.5000
+            }),
+            test_win_quantilex_aggregate({
+                quantile: 0.66666667,
+                valExpected: [
+                    0.0000, 0.6667, 1.3333, 2.0000,
+                    2.6667, 2.3333, 3.0000, 3.6667,
+                    4.6667, 6.0000, 6.0000, 6.6667
+                ],
+                valExpected2: 6.0000
+            }),
+            test_win_quantilex_aggregate({
+                quantile: 0.75,
+                valExpected: [
+                    0.0000, 0.7500, 1.5000, 2.2500,
+                    3.0000, 2.7500, 3.5000, 4.5000,
+                    6.0000, 6.0000, 7.0000, 8.2500
+                ],
+                valExpected2: 6.5000
+            }),
+            test_win_quantilex_aggregate({
+                quantile: 1,
+                valExpected: [
+                    0.0000, 1.0000, 2.0000, 3.0000,
+                    4.0000, 4.0000, 6.0000, 6.0000,
+                    8.0000, 9.0000, 10.0000, 11.0000
+                ],
+                valExpected2: 10.0000
+            }),
+            // test win_quantilex-aggregate-window handling-behavior
+            test_win_quantilex_aggregate({
+                aa: 8,
+                bb: 0,
+                quantile: 0,
+                valExpected: [
+                    0.0000, 0.0000, 0.0000, 0.0000,
+                    0.0000, 0.0000, 0.0000, 0.0000,
+                    0.0000, 0.0000, 0.0000, 0.0000
+                ],
+                valExpected2: -1
+            }),
+            test_win_quantilex_aggregate({
+                aa: 8,
+                bb: 0,
+                quantile: 0.25,
+                valExpected: [
+                    0.0000, 0.2500, 0.5000, 0.7500,
+                    1.0000, 0.2500, 0.5000, 0.7500,
+                    1.7500, 2.7500, 3.7500, 5.5000
+                ],
+                valExpected2: 3
+            }),
+            test_win_quantilex_aggregate({
+                aa: 8,
+                bb: 0,
+                quantile: 0.33333333,
+                valExpected: [
+                    0.0000, 0.3333, 0.6667, 1.0000,
+                    1.3333, 0.6667, 1.0000, 1.3333,
+                    2.3333, 3.3333, 4.6667, 6.0000
+                ],
+                valExpected2: 4.6667
+            }),
+            test_win_quantilex_aggregate({
+                aa: 8,
+                bb: 0,
+                quantile: 0.5000,
+                valExpected: [
+                    0.0000, 0.5000, 1.0000, 1.5000,
+                    2.0000, 1.5000, 2.0000, 2.5000,
+                    3.5000, 5.0000, 6.0000, 7.0000
+                ],
+                valExpected2: 6.0000
+            }),
+            test_win_quantilex_aggregate({
+                aa: 8,
+                bb: 0,
+                quantile: 0.66666667,
+                valExpected: [
+                    0.0000, 0.6667, 1.3333, 2.0000,
+                    2.6667, 2.3333, 3.0000, 3.6667,
+                    5.3333, 6.0000, 7.3333, 8.6667
+                ],
+                valExpected2: 7.3333
+            }),
+            test_win_quantilex_aggregate({
+                aa: 8,
+                bb: 0,
+                quantile: 0.75,
+                valExpected: [
+                    0.0000, 0.7500, 1.5000, 2.2500,
+                    3.0000, 2.7500, 3.5000, 4.5000,
+                    6.0000, 6.5000, 8.2500, 9.2500
+                ],
+                valExpected2: 8.2500
+            }),
+            test_win_quantilex_aggregate({
+                aa: 8,
+                bb: 0,
+                quantile: 1.0000,
+                valExpected: [
+                    0.0000, 1.0000, 2.0000, 3.0000,
+                    4.0000, 4.0000, 6.0000, 6.0000,
+                    8.0000, 9.0000, 10.0000, 11.0000
+                ],
+                valExpected2: 10.0000
+            })
+        ]);
+    });
+    jstestIt((
+        "test sqlite-extension-win_slr2 handling-behavior"
+    ), async function test_sqlite_extension_win_slr2() {
+        let db = await dbOpenAsync({filename: ":memory:"});
+        let valActual;
+        let valExpected;
+        let valIn;
+        async function test_win_slr2_aggregate({
+            aa,
+            bb,
+            valExpected,
+            valExpected2
+        }) {
+            let sqlBetween = "";
+            let valActual; //jslint-ignore-line
+            if (aa !== undefined) {
+                sqlBetween = (
+                    `ROWS BETWEEN ${aa - 1} PRECEDING AND ${bb} FOLLOWING`
+                );
+            }
+            // test win_slr2-aggregate handling-behavior
+            valActual = await dbExecAsync({
+                bindList: {
+                    valIn: JSON.stringify(valIn)
+                },
+                db,
+                sql: (`
+SELECT
+        id,
+        --
+        ROUND(slr->>(0 + 0), 8) AS nnn1,
+        ROUND(slr->>(0 + 1), 8) AS mxx1,
+        ROUND(slr->>(0 + 2), 8) AS myy1,
+        ROUND(slr->>(0 + 3), 8) AS exx1,
+        ROUND(slr->>(0 + 4), 8) AS eyy1,
+        ROUND(slr->>(0 + 5), 8) AS crr1,
+        ROUND(slr->>(0 + 6), 8) AS cbb1,
+        ROUND(slr->>(0 + 7), 8) AS caa1,
+        --
+        ROUND(slr->>(8 + 0), 8) AS nnn2,
+        ROUND(slr->>(8 + 1), 8) AS mxx2,
+        ROUND(slr->>(8 + 2), 8) AS myy2,
+        ROUND(slr->>(8 + 3), 8) AS exx2,
+        ROUND(slr->>(8 + 4), 8) AS eyy2,
+        ROUND(slr->>(8 + 5), 8) AS crr2,
+        ROUND(slr->>(8 + 6), 8) AS cbb2,
+        ROUND(slr->>(8 + 7), 8) AS caa2
+    FROM (
+        SELECT
+            id,
+            win_slr2(
+                value->>0,
+                value->>1,
+                value->>0,
+                IIF(id = 28, -1, value->>1)
+            ) OVER (
+                ORDER BY NULL ASC
+                ${sqlBetween}
+            ) AS slr
+        FROM JSON_EAcH($valIn)
+    );
+                `)
+            });
+            valActual = valActual[0].map(function ({
+                caa1,
+                caa2,
+                cbb1,
+                cbb2,
+                crr1,
+                crr2,
+                exx1,
+                exx2,
+                eyy1,
+                eyy2,
+                mxx1,
+                mxx2,
+                myy1,
+                myy2,
+                nnn1,
+                nnn2
+            }, ii, list) {
+                let obj1;
+                let obj2;
+                obj1 = {
+                    caa: caa1,
+                    cbb: cbb1,
+                    crr: crr1,
+                    exx: exx1,
+                    eyy: eyy1,
+                    mxx: mxx1,
+                    myy: myy1,
+                    nnn: nnn1
+                };
+                obj2 = {
+                    caa: caa2,
+                    cbb: cbb2,
+                    crr: crr2,
+                    exx: exx2,
+                    eyy: eyy2,
+                    mxx: mxx2,
+                    myy: myy2,
+                    nnn: nnn2
+                };
+                if (ii + (bb || 0) + 1 >= list.length) {
+                    assertJsonEqual(obj2, valExpected2, valActual);
+                } else {
+                    assertJsonEqual(obj2, obj1, valActual);
+                }
+                return obj1;
+            });
+            assertJsonEqual(valActual, valExpected);
+        }
+        noop(test_win_slr2_aggregate);
+        valExpected = [
+            {
+                "caa": null,
+                "cbb": null,
+                "crr": null,
+                "exx": null,
+                "eyy": null,
+                "mxx": 2,
+                "myy": 0,
+                "nnn": 1
+            },
+            {
+                "caa": null,
+                "cbb": null,
+                "crr": null,
+                "exx": 0,
+                "eyy": 0.70710678,
+                "mxx": 2,
+                "myy": 0.5,
+                "nnn": 2
+            },
+            {
+                "caa": -4.5,
+                "cbb": 2.5,
+                "crr": 0.94491118,
+                "exx": 0.57735027,
+                "eyy": 1.52752523,
+                "mxx": 2.33333333,
+                "myy": 1.33333333,
+                "nnn": 3
+            },
+            {
+                "caa": -3,
+                "cbb": 1.81818182,
+                "crr": 0.95346259,
+                "exx": 0.95742711,
+                "eyy": 1.82574186,
+                "mxx": 2.75,
+                "myy": 2,
+                "nnn": 4
+            },
+            {
+                "caa": -2.29411765,
+                "cbb": 1.52941176,
+                "crr": 0.96164474,
+                "exx": 1.30384048,
+                "eyy": 2.07364414,
+                "mxx": 3.2,
+                "myy": 2.6,
+                "nnn": 5
+            },
+            {
+                "caa": -2.54385965,
+                "cbb": 1.63157895,
+                "crr": 0.97080629,
+                "exx": 1.37840488,
+                "eyy": 2.31660671,
+                "mxx": 3.5,
+                "myy": 3.16666667,
+                "nnn": 6
+            },
+            {
+                "caa": -2.65,
+                "cbb": 1.675,
+                "crr": 0.9752227,
+                "exx": 1.38013112,
+                "eyy": 2.37045304,
+                "mxx": 3.71428571,
+                "myy": 3.57142857,
+                "nnn": 7
+            },
+            {
+                "caa": -2.5,
+                "cbb": 1.625,
+                "crr": 0.97991187,
+                "exx": 1.51185789,
+                "eyy": 2.50713268,
+                "mxx": 4,
+                "myy": 4,
+                "nnn": 8
+            },
+            {
+                "caa": 0.75,
+                "cbb": 0.85,
+                "crr": 0.89597867,
+                "exx": 2.39045722,
+                "eyy": 2.26778684,
+                "mxx": 5,
+                "myy": 5,
+                "nnn": 8
+            },
+            {
+                "caa": 2.75,
+                "cbb": 0.55,
+                "crr": 0.81989159,
+                "exx": 2.39045722,
+                "eyy": 1.60356745,
+                "mxx": 5,
+                "myy": 5.5,
+                "nnn": 8
+            }
+        ];
+        valIn = [
+            [2, "abcd"],
+            [NaN, 1],
+            [3, 3],
+            [4, 4],
+            [5, 5],
+            [5, 6],
+            [5, undefined],
+            [6, 7],
+            //
+            [10, 8],
+            [2, 5]
+        ];
+        await Promise.all([
+            (async function () {
+                // test win_slr2-error handling-behavior
+                await assertErrorThrownAsync(function () {
+                    return dbExecAsync({
+                        db,
+                        sql: (`
+SELECT win_slr2(1) FROM (SELECT 1);
+                        `)
+                    });
+                }, "wrong number of arguments");
+                // test win_slr2-null-case handling-behavior
+                valActual = await dbExecAsync({
+                    db,
+                    sql: (`
+DROP TABLE IF EXISTS __tmp1;
+CREATE TEMP TABLE __tmp1 (val REAL);
+SELECT win_slr2(1, 1) FROM __tmp1;
+                    `)
+                });
+                valActual = valActual[0].map(function ({val}) {
+                    return val;
+                });
+                assertJsonEqual(valActual, [null]);
+            }()),
+            // test win_slr2-aggregate-normal handling-behavior
+            (async function () {
+                valActual = await dbExecAndReturnLastJsonAsync({
+                    bindList: {
+                        valIn: JSON.stringify(valIn)
+                    },
+                    db,
+                    sql: (`
+SELECT win_slr2(value->>0, value->>1) AS slr FROM JSON_EACH($valIn);
+                    `)
+                });
+                valActual = valActual.map(function (xx) {
+                    return Number(xx.toFixed(8));
+                });
+                assertJsonEqual(
+                    valActual,
+                    [
+                        10, // nnn
+                        4.4, // mxx
+                        4.5, // myy
+                        2.45854519, // exx
+                        2.54950976, // eyy
+                        0.81541829, // crr
+                        0.84558824, // cbb
+                        0.77941176 // caa
+                    ]
+                );
+            }()),
+            // test win_slr2-aggregate-window handling-behavior
+            test_win_slr2_aggregate({
+                aa: 8,
+                bb: 0,
+                valExpected,
+                valExpected2: {
+                    caa: -0.25,
+                    cbb: 1,
+                    crr: 0.84895272,
+                    exx: 2.39045722,
+                    eyy: 2.81577191,
+                    mxx: 5,
+                    myy: 4.75,
+                    nnn: 8
+                }
+            })
+        ]);
+    });
 });
 
 jstestDescribe((
     "test_sqlmathWebworkerInit"
 ), function test_sqlmathWebworkerInit() {
     jstestIt((
         "test sqlmathWebworkerInit handling-behavior"
```

