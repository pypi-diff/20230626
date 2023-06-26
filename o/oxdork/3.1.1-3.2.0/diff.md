# Comparing `tmp/oxdork-3.1.1.tar.gz` & `tmp/oxdork-3.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "oxdork-3.1.1.tar", last modified: Mon Jun 26 01:23:05 2023, max compression
+gzip compressed data, was "oxdork-3.2.0.tar", max compression
```

## Comparing `oxdork-3.1.1.tar` & `oxdork-3.2.0.tar`

### file list

```diff
@@ -1,27 +1,9 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 01:23:05.039991 oxdork-3.1.1/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 01:23:05.035991 oxdork-3.1.1/.github/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 01:23:05.035991 oxdork-3.1.1/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)     2949 2023-06-26 01:22:50.000000 oxdork-3.1.1/.github/workflows/codeql.yml
--rw-r--r--   0 runner    (1001) docker     (123)     1084 2023-06-26 01:22:50.000000 oxdork-3.1.1/.github/workflows/python-publish.yml
--rw-r--r--   0 runner    (1001) docker     (123)       12 2023-06-26 01:22:50.000000 oxdork-3.1.1/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)      193 2023-06-26 01:22:50.000000 oxdork-3.1.1/Dockerfile
--rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-06-26 01:22:50.000000 oxdork-3.1.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     3445 2023-06-26 01:23:05.039991 oxdork-3.1.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1409 2023-06-26 01:22:50.000000 oxdork-3.1.1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 01:23:05.035991 oxdork-3.1.1/dork_queries/
--rw-r--r--   0 runner    (1001) docker     (123)   148095 2023-06-26 01:22:50.000000 oxdork-3.1.1/dork_queries/dork_queries.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 01:23:05.035991 oxdork-3.1.1/oxdork/
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-26 01:22:50.000000 oxdork-3.1.1/oxdork/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      574 2023-06-26 01:22:50.000000 oxdork-3.1.1/oxdork/banner.py
--rw-r--r--   0 runner    (1001) docker     (123)     1148 2023-06-26 01:22:50.000000 oxdork-3.1.1/oxdork/config.py
--rw-r--r--   0 runner    (1001) docker     (123)      551 2023-06-26 01:22:50.000000 oxdork-3.1.1/oxdork/main.py
--rw-r--r--   0 runner    (1001) docker     (123)     2243 2023-06-26 01:22:50.000000 oxdork-3.1.1/oxdork/oxdork.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 01:23:05.039991 oxdork-3.1.1/oxdork.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     3445 2023-06-26 01:23:05.000000 oxdork-3.1.1/oxdork.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      417 2023-06-26 01:23:05.000000 oxdork-3.1.1/oxdork.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-26 01:23:05.000000 oxdork-3.1.1/oxdork.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       44 2023-06-26 01:23:05.000000 oxdork-3.1.1/oxdork.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)       21 2023-06-26 01:23:05.000000 oxdork-3.1.1/oxdork.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        7 2023-06-26 01:23:05.000000 oxdork-3.1.1/oxdork.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1017 2023-06-26 01:22:50.000000 oxdork-3.1.1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-26 01:23:05.039991 oxdork-3.1.1/setup.cfg
+-rw-r--r--   0        0        0     1070 2023-06-26 04:37:34.806616 oxdork-3.2.0/LICENSE
+-rw-r--r--   0        0        0     1364 2023-06-26 04:37:34.806616 oxdork-3.2.0/README.md
+-rw-r--r--   0        0        0        1 2023-06-26 04:37:34.806616 oxdork-3.2.0/oxdork/__init__.py
+-rw-r--r--   0        0        0     2366 2023-06-26 04:37:34.806616 oxdork-3.2.0/oxdork/config.py
+-rw-r--r--   0        0        0      454 2023-06-26 04:37:34.806616 oxdork-3.2.0/oxdork/data/data.json
+-rw-r--r--   0        0        0      763 2023-06-26 04:37:34.806616 oxdork-3.2.0/oxdork/main.py
+-rw-r--r--   0        0        0     3000 2023-06-26 04:37:34.806616 oxdork-3.2.0/oxdork/oxdork.py
+-rw-r--r--   0        0        0      980 2023-06-26 04:37:34.806616 oxdork-3.2.0/pyproject.toml
+-rw-r--r--   0        0        0     2658 1970-01-01 00:00:00.000000 oxdork-3.2.0/PKG-INFO
```

### Comparing `oxdork-3.1.1/LICENSE` & `oxdork-3.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `oxdork-3.1.1/README.md` & `oxdork-3.2.0/README.md`

 * *Files 12% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 ![Screenshot_20210827-111909-removebg-preview](https://user-images.githubusercontent.com/74001397/131107876-db415339-0c1d-4876-8665-fe9b76c4518c.png)
 
-![OS](https://img.shields.io/badge/OS-GNU%2FLinux-red?style=for-the-badge&logo=linux)
-![OS](https://img.shields.io/badge/OS-Windows-blue?style=for-the-badge&logo=Windows)
-![GitHub](https://img.shields.io/github/license/rly0nheart/oxdork?style=for-the-badge&logo=github)
-![GitHub release (latest by date including pre-releases)](https://img.shields.io/github/v/release/rly0nheart/oxdork?include_prereleases&style=for-the-badge&logo=github)
-![GitHub repo size](https://img.shields.io/github/repo-size/rly0nheart/oxdork?style=for-the-badge&logo=github)
+![OS](https://img.shields.io/badge/OS-GNU%2FLinux-red?style=flat&logo=linux)
+![OS](https://img.shields.io/badge/OS-Windows-blue?style=flat&logo=Windows)
+![GitHub](https://img.shields.io/github/license/rly0nheart/oxdork?style=flat&logo=github)
+![GitHub release (latest by date including pre-releases)](https://img.shields.io/github/v/release/rly0nheart/oxdork?include_prereleases&style=flat&logo=github)
+![GitHub repo size](https://img.shields.io/github/repo-size/rly0nheart/oxdork?style=flat&logo=github)
 
 
 
 ![Screenshot_20230207_124512](https://user-images.githubusercontent.com/74001397/217223738-9a432f18-a30e-4121-87ca-09c7dad081e3.png)
 
 oxDork uses Google dorking techniques and Google dorks to find security holes and misconfigurations in web servers.
```

#### html2text {}

```diff
@@ -1,18 +1,17 @@
 ![Screenshot_20210827-111909-removebg-preview](https://user-
 images.githubusercontent.com/74001397/131107876-db415339-0c1d-4876-8665-
 fe9b76c4518c.png) ![OS](https://img.shields.io/badge/OS-GNU%2FLinux-
-red?style=for-the-badge&logo=linux) ![OS](https://img.shields.io/badge/OS-
-Windows-blue?style=for-the-badge&logo=Windows) ![GitHub](https://
-img.shields.io/github/license/rly0nheart/oxdork?style=for-the-
-badge&logo=github) ![GitHub release (latest by date including pre-releases)]
-(https://img.shields.io/github/v/release/rly0nheart/
-oxdork?include_prereleases&style=for-the-badge&logo=github) ![GitHub repo size]
-(https://img.shields.io/github/repo-size/rly0nheart/oxdork?style=for-the-
-badge&logo=github) ![Screenshot_20230207_124512](https://user-
-images.githubusercontent.com/74001397/217223738-9a432f18-a30e-4121-87ca-
-09c7dad081e3.png) oxDork uses Google dorking techniques and Google dorks to
-find security holes and misconfigurations in web servers. # Wiki Check the
-*Installation guide*, *Usage*, and *a Available options* on the [wiki](https://
-github.com/rly0nheart/oxdork/wiki/) # Queries A collection of 5,568 common dork
-queries [here](https://github.com/rly0nheart/oxdork/tree/master/dork_queries) #
-Support [Buy_Me_A_Coffee]
+red?style=flat&logo=linux) ![OS](https://img.shields.io/badge/OS-Windows-
+blue?style=flat&logo=Windows) ![GitHub](https://img.shields.io/github/license/
+rly0nheart/oxdork?style=flat&logo=github) ![GitHub release (latest by date
+including pre-releases)](https://img.shields.io/github/v/release/rly0nheart/
+oxdork?include_prereleases&style=flat&logo=github) ![GitHub repo size](https://
+img.shields.io/github/repo-size/rly0nheart/oxdork?style=flat&logo=github) !
+[Screenshot_20230207_124512](https://user-images.githubusercontent.com/
+74001397/217223738-9a432f18-a30e-4121-87ca-09c7dad081e3.png) oxDork uses Google
+dorking techniques and Google dorks to find security holes and
+misconfigurations in web servers. # Wiki Check the *Installation guide*,
+*Usage*, and *a Available options* on the [wiki](https://github.com/rly0nheart/
+oxdork/wiki/) # Queries A collection of 5,568 common dork queries [here](https:
+//github.com/rly0nheart/oxdork/tree/master/dork_queries) # Support [Buy_Me_A
+Coffee]
```

### Comparing `oxdork-3.1.1/pyproject.toml` & `oxdork-3.2.0/pyproject.toml`

 * *Files 21% similar despite different names*

```diff
@@ -1,39 +1,37 @@
 [build-system]
-requires = ["setuptools", "setuptools-scm"]
-build-backend = "setuptools.build_meta"
+requires = ["poetry-core"]
+build-backend = "poetry.core.masonry.api"
 
-[tool.setuptools]
-packages = ["oxdork"]
+[tool.poetry]
+include = [
+    {path = "oxdork/data/data.json"}
+]
 
-[project]
 name = "oxdork"
-version = "3.1.1"
-description = "Google dorking tool"
+version = "3.2.0"
+description = "Google dorking tool."
 readme = "README.md"
 requires-python = ">=3.8"
-license = {file = "LICENSE"}
+license = "MIT License"
+homepage = "https://github.com/rly0nheart/oxdork"
+documentation = "https://github.com/rly0nheart/oxdork/wiki/"
+repository = "https://github.com/rly0nheart/oxdork.git"
 keywords = ["python", "osint", "google-dorking", "osint", "inurl", "intext", "intitle"]
-authors = [{name = "Richard Mwewa", email = "rly0nheart@duck.com"}]
+authors = ["Richard Mwewa <rly0nheart@duck.com>"]
 classifiers = [
   "Development Status :: 5 - Production/Stable",
   "Programming Language :: Python :: 3",
   "Intended Audience :: Information Technology",
   "License :: OSI Approved :: MIT License",
   "Operating System :: OS Independent",
   "Natural Language :: English",
   ""
 ]
 
-dependencies = [
-  "rich",
-  "google",
-  "requests"
-]
+[tool.poetry.dependencies]
+rich = "*"
+google = "*"
 
-[project.urls]
-homepage = "https://github.com/rly0nheart/oxdork"
-documentation = "https://github.com/rly0nheart/oxdork/wiki/"
-repository = "https://github.com/rly0nheart/oxdork.git"
 
-[project.scripts]
-oxdork = "oxdork.main:main"
+[tool.poetry.scripts]
+oxdork = "oxdork.main:run"
```

