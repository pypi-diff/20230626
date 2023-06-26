# Comparing `tmp/geovisio_cli-0.2.1.tar.gz` & `tmp/geovisio_cli-0.2.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "geovisio_cli-0.2.1.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
+gzip compressed data, was "geovisio_cli-0.2.2.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
```

## Comparing `geovisio_cli-0.2.1.tar` & `geovisio_cli-0.2.2.tar`

### file list

```diff
@@ -1,35 +1,35 @@
--rw-r--r--   0        0        0       47 2023-03-24 13:15:13.689899 geovisio_cli-0.2.1/.gitignore
--rw-r--r--   0        0        0     1413 2023-06-22 09:18:10.500879 geovisio_cli-0.2.1/.gitlab-ci.yml
--rw-r--r--   0        0        0     3716 2023-06-22 10:32:13.532461 geovisio_cli-0.2.1/CHANGELOG.md
--rw-r--r--   0        0        0     5468 2023-03-24 13:15:13.689899 geovisio_cli-0.2.1/CODE_OF_CONDUCT.md
--rw-r--r--   0        0        0     1070 2023-03-14 15:26:20.137987 geovisio_cli-0.2.1/LICENSE
--rw-r--r--   0        0        0      590 2023-05-24 13:17:27.558420 geovisio_cli-0.2.1/Makefile
--rw-r--r--   0        0        0     7516 2023-05-24 13:17:27.558420 geovisio_cli-0.2.1/README.md
--rw-r--r--   0        0        0     3250 2023-06-22 09:18:10.500879 geovisio_cli-0.2.1/USAGE.md
--rw-r--r--   0        0        0       53 2023-06-22 10:32:13.532461 geovisio_cli-0.2.1/geovisio_cli/__init__.py
--rw-r--r--   0        0        0     6173 2023-05-24 13:17:27.558420 geovisio_cli-0.2.1/geovisio_cli/auth.py
--rw-r--r--   0        0        0      284 2023-04-14 11:12:54.559203 geovisio_cli-0.2.1/geovisio_cli/exception.py
--rw-r--r--   0        0        0     6180 2023-06-22 09:18:10.500879 geovisio_cli-0.2.1/geovisio_cli/main.py
--rw-r--r--   0        0        0      136 2023-05-24 13:17:27.558420 geovisio_cli-0.2.1/geovisio_cli/model.py
--rw-r--r--   0        0        0    21407 2023-06-20 08:50:48.042695 geovisio_cli-0.2.1/geovisio_cli/sequence.py
--rw-r--r--   0        0        0     2107 2023-06-22 09:18:10.500879 geovisio_cli-0.2.1/geovisio_cli/utils.py
--rw-r--r--   0        0        0     1196 2023-06-22 09:18:10.500879 geovisio_cli-0.2.1/pyproject.toml
--rw-r--r--   0        0        0        0 2023-03-14 15:26:20.137987 geovisio_cli-0.2.1/tests/__init__.py
--rw-r--r--   0        0        0      234 2023-06-19 17:19:08.702865 geovisio_cli-0.2.1/tests/conftest.py
--rw-r--r--   0        0        0   523332 2023-03-14 15:26:20.137987 geovisio_cli-0.2.1/tests/fixtures/e1.jpg
--rw-r--r--   0        0        0   483454 2023-03-14 15:26:20.141986 geovisio_cli-0.2.1/tests/fixtures/e2.jpg
--rw-r--r--   0        0        0   529344 2023-03-14 15:26:20.141986 geovisio_cli-0.2.1/tests/fixtures/e3.jpg
--rw-r--r--   0        0        0       16 2023-03-14 15:26:20.141986 geovisio_cli-0.2.1/tests/fixtures/invalid_pic.jpg
--rw-r--r--   0        0        0       27 2023-03-14 15:26:20.141986 geovisio_cli-0.2.1/tests/fixtures/not_a_pic.md
--rw-r--r--   0        0        0        0 2023-03-14 15:26:20.141986 geovisio_cli-0.2.1/tests/integration/__init__.py
--rw-r--r--   0        0        0     3327 2023-05-24 13:17:27.558420 geovisio_cli-0.2.1/tests/integration/conftest.py
--rw-r--r--   0        0        0     2189 2023-05-22 08:59:23.607560 geovisio_cli-0.2.1/tests/integration/docker-compose-geovisio.yml
--rw-r--r--   0        0        0      584 2023-05-22 08:59:23.607560 geovisio_cli-0.2.1/tests/integration/docker-compose-gitlab-override.yml
--rw-r--r--   0        0        0    76457 2023-05-22 08:59:23.611560 geovisio_cli-0.2.1/tests/integration/keycloak-realm.json
--rw-r--r--   0        0        0     3210 2023-06-22 08:20:49.394297 geovisio_cli-0.2.1/tests/integration/test_auth.py
--rw-r--r--   0        0        0      369 2023-05-24 13:17:27.558420 geovisio_cli-0.2.1/tests/integration/test_status.py
--rw-r--r--   0        0        0     7087 2023-06-22 08:20:49.394297 geovisio_cli-0.2.1/tests/integration/test_upload.py
--rw-r--r--   0        0        0      583 2023-05-10 11:47:16.328656 geovisio_cli-0.2.1/tests/test_process.py
--rw-r--r--   0        0        0    10801 2023-06-22 08:20:49.394297 geovisio_cli-0.2.1/tests/test_sequence.py
--rw-r--r--   0        0        0      682 2023-06-22 09:18:10.500879 geovisio_cli-0.2.1/tests/test_utils.py
--rw-r--r--   0        0        0     8652 1970-01-01 00:00:00.000000 geovisio_cli-0.2.1/PKG-INFO
+-rw-r--r--   0        0        0       47 2023-03-24 13:15:13.689899 geovisio_cli-0.2.2/.gitignore
+-rw-r--r--   0        0        0     1413 2023-06-22 09:18:10.500879 geovisio_cli-0.2.2/.gitlab-ci.yml
+-rw-r--r--   0        0        0     3789 2023-06-26 07:08:10.068178 geovisio_cli-0.2.2/CHANGELOG.md
+-rw-r--r--   0        0        0     5468 2023-03-24 13:15:13.689899 geovisio_cli-0.2.2/CODE_OF_CONDUCT.md
+-rw-r--r--   0        0        0     1070 2023-03-14 15:26:20.137987 geovisio_cli-0.2.2/LICENSE
+-rw-r--r--   0        0        0      590 2023-05-24 13:17:27.558420 geovisio_cli-0.2.2/Makefile
+-rw-r--r--   0        0        0     7516 2023-05-24 13:17:27.558420 geovisio_cli-0.2.2/README.md
+-rw-r--r--   0        0        0     3250 2023-06-22 09:18:10.500879 geovisio_cli-0.2.2/USAGE.md
+-rw-r--r--   0        0        0       53 2023-06-26 07:08:10.068178 geovisio_cli-0.2.2/geovisio_cli/__init__.py
+-rw-r--r--   0        0        0     6173 2023-05-24 13:17:27.558420 geovisio_cli-0.2.2/geovisio_cli/auth.py
+-rw-r--r--   0        0        0      284 2023-04-14 11:12:54.559203 geovisio_cli-0.2.2/geovisio_cli/exception.py
+-rw-r--r--   0        0        0     6180 2023-06-22 09:18:10.500879 geovisio_cli-0.2.2/geovisio_cli/main.py
+-rw-r--r--   0        0        0      136 2023-05-24 13:17:27.558420 geovisio_cli-0.2.2/geovisio_cli/model.py
+-rw-r--r--   0        0        0    21407 2023-06-20 08:50:48.042695 geovisio_cli-0.2.2/geovisio_cli/sequence.py
+-rw-r--r--   0        0        0     2107 2023-06-22 09:18:10.500879 geovisio_cli-0.2.2/geovisio_cli/utils.py
+-rw-r--r--   0        0        0     1221 2023-06-26 07:08:10.068178 geovisio_cli-0.2.2/pyproject.toml
+-rw-r--r--   0        0        0        0 2023-03-14 15:26:20.137987 geovisio_cli-0.2.2/tests/__init__.py
+-rw-r--r--   0        0        0      234 2023-06-19 17:19:08.702865 geovisio_cli-0.2.2/tests/conftest.py
+-rw-r--r--   0        0        0   523332 2023-03-14 15:26:20.137987 geovisio_cli-0.2.2/tests/fixtures/e1.jpg
+-rw-r--r--   0        0        0   483454 2023-03-14 15:26:20.141986 geovisio_cli-0.2.2/tests/fixtures/e2.jpg
+-rw-r--r--   0        0        0   529344 2023-03-14 15:26:20.141986 geovisio_cli-0.2.2/tests/fixtures/e3.jpg
+-rw-r--r--   0        0        0       16 2023-03-14 15:26:20.141986 geovisio_cli-0.2.2/tests/fixtures/invalid_pic.jpg
+-rw-r--r--   0        0        0       27 2023-03-14 15:26:20.141986 geovisio_cli-0.2.2/tests/fixtures/not_a_pic.md
+-rw-r--r--   0        0        0        0 2023-03-14 15:26:20.141986 geovisio_cli-0.2.2/tests/integration/__init__.py
+-rw-r--r--   0        0        0     3327 2023-05-24 13:17:27.558420 geovisio_cli-0.2.2/tests/integration/conftest.py
+-rw-r--r--   0        0        0     2189 2023-05-22 08:59:23.607560 geovisio_cli-0.2.2/tests/integration/docker-compose-geovisio.yml
+-rw-r--r--   0        0        0      584 2023-05-22 08:59:23.607560 geovisio_cli-0.2.2/tests/integration/docker-compose-gitlab-override.yml
+-rw-r--r--   0        0        0    76457 2023-05-22 08:59:23.611560 geovisio_cli-0.2.2/tests/integration/keycloak-realm.json
+-rw-r--r--   0        0        0     3210 2023-06-22 08:20:49.394297 geovisio_cli-0.2.2/tests/integration/test_auth.py
+-rw-r--r--   0        0        0      369 2023-05-24 13:17:27.558420 geovisio_cli-0.2.2/tests/integration/test_status.py
+-rw-r--r--   0        0        0     7087 2023-06-22 08:20:49.394297 geovisio_cli-0.2.2/tests/integration/test_upload.py
+-rw-r--r--   0        0        0      583 2023-05-10 11:47:16.328656 geovisio_cli-0.2.2/tests/test_process.py
+-rw-r--r--   0        0        0    10801 2023-06-22 08:20:49.394297 geovisio_cli-0.2.2/tests/test_sequence.py
+-rw-r--r--   0        0        0      682 2023-06-22 09:18:10.500879 geovisio_cli-0.2.2/tests/test_utils.py
+-rw-r--r--   0        0        0     8685 1970-01-01 00:00:00.000000 geovisio_cli-0.2.2/PKG-INFO
```

### Comparing `geovisio_cli-0.2.1/.gitlab-ci.yml` & `geovisio_cli-0.2.2/.gitlab-ci.yml`

 * *Files identical despite different names*

### Comparing `geovisio_cli-0.2.1/CHANGELOG.md` & `geovisio_cli-0.2.2/CHANGELOG.md`

 * *Files 5% similar despite different names*

```diff
@@ -2,14 +2,19 @@
 All notable changes to this project will be documented in this file.
 
 The format is based on [Keep a Changelog](https://keepachangelog.com/en/1.0.0/),
 and this project adheres to [Semantic Versioning](https://semver.org/spec/v2.0.0.html).
 
 ## [Unreleased]
 
+## [0.2.2] - 2023-06-26
+
+### Fixes
+- Add missing `packaging` dependency
+
 ## [0.2.1] - 2023-06-22
 
 ### Added
 - A new parameter `--sort-method` allows user to choose how pictures should be sorted, either by their date/time or file name, in ascending or descending order. Default is now by date/time ascending (was previously by filename ascending).
 - A new `--version` parameter to get the geovisio_cli version
 
 ### Changed
```

### Comparing `geovisio_cli-0.2.1/CODE_OF_CONDUCT.md` & `geovisio_cli-0.2.2/CODE_OF_CONDUCT.md`

 * *Files identical despite different names*

### Comparing `geovisio_cli-0.2.1/LICENSE` & `geovisio_cli-0.2.2/LICENSE`

 * *Files identical despite different names*

### Comparing `geovisio_cli-0.2.1/Makefile` & `geovisio_cli-0.2.2/Makefile`

 * *Files identical despite different names*

### Comparing `geovisio_cli-0.2.1/README.md` & `geovisio_cli-0.2.2/README.md`

 * *Files identical despite different names*

### Comparing `geovisio_cli-0.2.1/USAGE.md` & `geovisio_cli-0.2.2/USAGE.md`

 * *Files identical despite different names*

### Comparing `geovisio_cli-0.2.1/geovisio_cli/auth.py` & `geovisio_cli-0.2.2/geovisio_cli/auth.py`

 * *Files identical despite different names*

### Comparing `geovisio_cli-0.2.1/geovisio_cli/main.py` & `geovisio_cli-0.2.2/geovisio_cli/main.py`

 * *Files identical despite different names*

### Comparing `geovisio_cli-0.2.1/geovisio_cli/sequence.py` & `geovisio_cli-0.2.2/geovisio_cli/sequence.py`

 * *Files identical despite different names*

### Comparing `geovisio_cli-0.2.1/geovisio_cli/utils.py` & `geovisio_cli-0.2.2/geovisio_cli/utils.py`

 * *Files identical despite different names*

### Comparing `geovisio_cli-0.2.1/pyproject.toml` & `geovisio_cli-0.2.2/pyproject.toml`

 * *Files 4% similar despite different names*

```diff
@@ -14,14 +14,15 @@
 dependencies = [
     "requests ~= 2.28.0",
     "typer ~= 0.9.0",
     "rich[all] ~= 13.3.0",
     "toml ~= 0.10.2",
     "qrcode ~= 7.4.2",
     "geopic-tag-reader ~= 0.1.3",
+    "packaging ~= 23.1",
 ]
 
 [project.urls]
 Home = "https://gitlab.com/geovisio/cli"
 
 [project.scripts]
 geovisio="geovisio_cli.main:app"
```

### Comparing `geovisio_cli-0.2.1/tests/fixtures/e1.jpg` & `geovisio_cli-0.2.2/tests/fixtures/e1.jpg`

 * *Files identical despite different names*

### Comparing `geovisio_cli-0.2.1/tests/fixtures/e2.jpg` & `geovisio_cli-0.2.2/tests/fixtures/e2.jpg`

 * *Files identical despite different names*

### Comparing `geovisio_cli-0.2.1/tests/fixtures/e3.jpg` & `geovisio_cli-0.2.2/tests/fixtures/e3.jpg`

 * *Files identical despite different names*

### Comparing `geovisio_cli-0.2.1/tests/integration/conftest.py` & `geovisio_cli-0.2.2/tests/integration/conftest.py`

 * *Files identical despite different names*

### Comparing `geovisio_cli-0.2.1/tests/integration/docker-compose-geovisio.yml` & `geovisio_cli-0.2.2/tests/integration/docker-compose-geovisio.yml`

 * *Files identical despite different names*

### Comparing `geovisio_cli-0.2.1/tests/integration/docker-compose-gitlab-override.yml` & `geovisio_cli-0.2.2/tests/integration/docker-compose-gitlab-override.yml`

 * *Files identical despite different names*

### Comparing `geovisio_cli-0.2.1/tests/integration/keycloak-realm.json` & `geovisio_cli-0.2.2/tests/integration/keycloak-realm.json`

 * *Files identical despite different names*

### Comparing `geovisio_cli-0.2.1/tests/integration/test_auth.py` & `geovisio_cli-0.2.2/tests/integration/test_auth.py`

 * *Files identical despite different names*

### Comparing `geovisio_cli-0.2.1/tests/integration/test_upload.py` & `geovisio_cli-0.2.2/tests/integration/test_upload.py`

 * *Files identical despite different names*

### Comparing `geovisio_cli-0.2.1/tests/test_process.py` & `geovisio_cli-0.2.2/tests/test_process.py`

 * *Files identical despite different names*

### Comparing `geovisio_cli-0.2.1/tests/test_sequence.py` & `geovisio_cli-0.2.2/tests/test_sequence.py`

 * *Files identical despite different names*

### Comparing `geovisio_cli-0.2.1/tests/test_utils.py` & `geovisio_cli-0.2.2/tests/test_utils.py`

 * *Files identical despite different names*

### Comparing `geovisio_cli-0.2.1/PKG-INFO` & `geovisio_cli-0.2.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,20 +1,21 @@
 Metadata-Version: 2.1
 Name: geovisio_cli
-Version: 0.2.1
+Version: 0.2.2
 Summary: Geovio client cli tool
 Author-email: Antoine Desbordes <antoine.desbordes@gmail.com>
 Description-Content-Type: text/markdown
 Classifier: License :: OSI Approved :: MIT License
 Requires-Dist: requests ~= 2.28.0
 Requires-Dist: typer ~= 0.9.0
 Requires-Dist: rich[all] ~= 13.3.0
 Requires-Dist: toml ~= 0.10.2
 Requires-Dist: qrcode ~= 7.4.2
 Requires-Dist: geopic-tag-reader ~= 0.1.3
+Requires-Dist: packaging ~= 23.1
 Requires-Dist: flit ~= 3.8.0 ; extra == "build"
 Requires-Dist: black ~= 22.8.0 ; extra == "dev"
 Requires-Dist: mypy ~= 1.0.0 ; extra == "dev"
 Requires-Dist: types-requests ~= 2.28.0 ; extra == "dev"
 Requires-Dist: pytest ~= 7.2.0 ; extra == "dev"
 Requires-Dist: testcontainers-compose ~= 0.0.1rc1 ; extra == "dev"
 Requires-Dist: pytest-datafiles ~= 2.0.1 ; extra == "dev"
```

