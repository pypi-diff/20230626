# Comparing `tmp/oxdork-3.1.0.tar.gz` & `tmp/oxdork-3.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "oxdork-3.1.0.tar", last modified: Mon Apr 24 21:58:25 2023, max compression
+gzip compressed data, was "oxdork-3.1.1.tar", last modified: Mon Jun 26 01:23:05 2023, max compression
```

## Comparing `oxdork-3.1.0.tar` & `oxdork-3.1.1.tar`

### file list

```diff
@@ -1,26 +1,27 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 21:58:25.954233 oxdork-3.1.0/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 21:58:25.954233 oxdork-3.1.0/.github/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 21:58:25.954233 oxdork-3.1.0/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)     2949 2023-04-24 21:58:14.000000 oxdork-3.1.0/.github/workflows/codeql.yml
--rw-r--r--   0 runner    (1001) docker     (123)     1084 2023-04-24 21:58:14.000000 oxdork-3.1.0/.github/workflows/python-publish.yml
--rw-r--r--   0 runner    (1001) docker     (123)       12 2023-04-24 21:58:14.000000 oxdork-3.1.0/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)      193 2023-04-24 21:58:14.000000 oxdork-3.1.0/Dockerfile
--rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-04-24 21:58:14.000000 oxdork-3.1.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     3443 2023-04-24 21:58:25.954233 oxdork-3.1.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1407 2023-04-24 21:58:14.000000 oxdork-3.1.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 21:58:25.954233 oxdork-3.1.0/dork_queries/
--rw-r--r--   0 runner    (1001) docker     (123)   148095 2023-04-24 21:58:14.000000 oxdork-3.1.0/dork_queries/dork_queries.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 21:58:25.954233 oxdork-3.1.0/oxdork/
--rw-r--r--   0 runner    (1001) docker     (123)      574 2023-04-24 21:58:14.000000 oxdork-3.1.0/oxdork/banner.py
--rw-r--r--   0 runner    (1001) docker     (123)     1148 2023-04-24 21:58:14.000000 oxdork-3.1.0/oxdork/config.py
--rw-r--r--   0 runner    (1001) docker     (123)      551 2023-04-24 21:58:14.000000 oxdork-3.1.0/oxdork/main.py
--rw-r--r--   0 runner    (1001) docker     (123)     2243 2023-04-24 21:58:14.000000 oxdork-3.1.0/oxdork/oxdork.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 21:58:25.954233 oxdork-3.1.0/oxdork.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     3443 2023-04-24 21:58:25.000000 oxdork-3.1.0/oxdork.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      398 2023-04-24 21:58:25.000000 oxdork-3.1.0/oxdork.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-24 21:58:25.000000 oxdork-3.1.0/oxdork.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       44 2023-04-24 21:58:25.000000 oxdork-3.1.0/oxdork.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)       21 2023-04-24 21:58:25.000000 oxdork-3.1.0/oxdork.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        7 2023-04-24 21:58:25.000000 oxdork-3.1.0/oxdork.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1017 2023-04-24 21:58:14.000000 oxdork-3.1.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-24 21:58:25.954233 oxdork-3.1.0/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 01:23:05.039991 oxdork-3.1.1/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 01:23:05.035991 oxdork-3.1.1/.github/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 01:23:05.035991 oxdork-3.1.1/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)     2949 2023-06-26 01:22:50.000000 oxdork-3.1.1/.github/workflows/codeql.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1084 2023-06-26 01:22:50.000000 oxdork-3.1.1/.github/workflows/python-publish.yml
+-rw-r--r--   0 runner    (1001) docker     (123)       12 2023-06-26 01:22:50.000000 oxdork-3.1.1/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)      193 2023-06-26 01:22:50.000000 oxdork-3.1.1/Dockerfile
+-rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-06-26 01:22:50.000000 oxdork-3.1.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     3445 2023-06-26 01:23:05.039991 oxdork-3.1.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1409 2023-06-26 01:22:50.000000 oxdork-3.1.1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 01:23:05.035991 oxdork-3.1.1/dork_queries/
+-rw-r--r--   0 runner    (1001) docker     (123)   148095 2023-06-26 01:22:50.000000 oxdork-3.1.1/dork_queries/dork_queries.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 01:23:05.035991 oxdork-3.1.1/oxdork/
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-26 01:22:50.000000 oxdork-3.1.1/oxdork/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      574 2023-06-26 01:22:50.000000 oxdork-3.1.1/oxdork/banner.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1148 2023-06-26 01:22:50.000000 oxdork-3.1.1/oxdork/config.py
+-rw-r--r--   0 runner    (1001) docker     (123)      551 2023-06-26 01:22:50.000000 oxdork-3.1.1/oxdork/main.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2243 2023-06-26 01:22:50.000000 oxdork-3.1.1/oxdork/oxdork.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 01:23:05.039991 oxdork-3.1.1/oxdork.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     3445 2023-06-26 01:23:05.000000 oxdork-3.1.1/oxdork.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      417 2023-06-26 01:23:05.000000 oxdork-3.1.1/oxdork.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-26 01:23:05.000000 oxdork-3.1.1/oxdork.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       44 2023-06-26 01:23:05.000000 oxdork-3.1.1/oxdork.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       21 2023-06-26 01:23:05.000000 oxdork-3.1.1/oxdork.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        7 2023-06-26 01:23:05.000000 oxdork-3.1.1/oxdork.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1017 2023-06-26 01:22:50.000000 oxdork-3.1.1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-26 01:23:05.039991 oxdork-3.1.1/setup.cfg
```

### Comparing `oxdork-3.1.0/.github/workflows/codeql.yml` & `oxdork-3.1.1/.github/workflows/codeql.yml`

 * *Files identical despite different names*

### Comparing `oxdork-3.1.0/.github/workflows/python-publish.yml` & `oxdork-3.1.1/.github/workflows/python-publish.yml`

 * *Files identical despite different names*

### Comparing `oxdork-3.1.0/LICENSE` & `oxdork-3.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `oxdork-3.1.0/PKG-INFO` & `oxdork-3.1.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: oxdork
-Version: 3.1.0
+Version: 3.1.1
 Summary: Google dorking tool
 Author-email: Richard Mwewa <rly0nheart@duck.com>
 License: MIT License
         
         Copyright (c) 2022 Richard Mwewa
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
@@ -61,8 +61,8 @@
 
 
 # Queries
 A collection of 5,568 common dork queries [here](https://github.com/rly0nheart/oxdork/tree/master/dork_queries)
 
 
 # Support
-<a href="https://www.buymeacoffee.com/189381184" target="_blank"><img src="https://cdn.buymeacoffee.com/buttons/default-orange.png" alt="Buy Me A Coffee" height="41" width="174"></a>
+<a href="https://www.buymeacoffee.com/_rly0nheart" target="_blank"><img src="https://cdn.buymeacoffee.com/buttons/default-orange.png" alt="Buy Me A Coffee" height="41" width="174"></a>
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: oxdork Version: 3.1.0 Summary: Google dorking tool
+Metadata-Version: 2.1 Name: oxdork Version: 3.1.1 Summary: Google dorking tool
 Author-email: Richard Mwewa
 duck.com> License: MIT License Copyright (c) 2022 Richard Mwewa Permission is
 hereby granted, free of charge, to any person obtaining a copy of this software
 and associated documentation files (the "Software"), to deal in the Software
 without restriction, including without limitation the rights to use, copy,
 modify, merge, publish, distribute, sublicense, and/or sell copies of the
 Software, and to permit persons to whom the Software is furnished to do so,
```

### Comparing `oxdork-3.1.0/README.md` & `oxdork-3.1.1/README.md`

 * *Files 7% similar despite different names*

```diff
@@ -19,8 +19,8 @@
 
 
 # Queries
 A collection of 5,568 common dork queries [here](https://github.com/rly0nheart/oxdork/tree/master/dork_queries)
 
 
 # Support
-<a href="https://www.buymeacoffee.com/189381184" target="_blank"><img src="https://cdn.buymeacoffee.com/buttons/default-orange.png" alt="Buy Me A Coffee" height="41" width="174"></a>
+<a href="https://www.buymeacoffee.com/_rly0nheart" target="_blank"><img src="https://cdn.buymeacoffee.com/buttons/default-orange.png" alt="Buy Me A Coffee" height="41" width="174"></a>
```

### Comparing `oxdork-3.1.0/dork_queries/dork_queries.txt` & `oxdork-3.1.1/dork_queries/dork_queries.txt`

 * *Files identical despite different names*

### Comparing `oxdork-3.1.0/oxdork/banner.py` & `oxdork-3.1.1/oxdork/banner.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 def ascii_banner():
-    version_tag = "3.1.0"
+    version_tag = "3.1.1"
     banner = f"""[red]
       ▐▄• ▄ ·▄▄▄▄        ▄▄▄  ▄ •▄ 
  ▄█▀▄  █▌█▌▪██▪ ██  ▄█▀▄ ▀▄ █·█▌▄▌▪
 ▐█▌.▐▌ ·██· ▐█· ▐█▌▐█▌.▐▌▐▀▀▄ ▐▀▀▄·
 ▐█▌.▐▌▪▐█·█▌██. ██ ▐█▌.▐▌▐█•█▌▐█.█▌
  ▀█▄▀▪•▀▀ ▀▀▀▀▀▀▀•  ▀█▄▀▪.▀  ▀·▀  ▀
                              [/]v{version_tag}"""
```

### Comparing `oxdork-3.1.0/oxdork/config.py` & `oxdork-3.1.1/oxdork/config.py`

 * *Files identical despite different names*

### Comparing `oxdork-3.1.0/oxdork/main.py` & `oxdork-3.1.1/oxdork/main.py`

 * *Files identical despite different names*

### Comparing `oxdork-3.1.0/oxdork/oxdork.py` & `oxdork-3.1.1/oxdork/oxdork.py`

 * *Files identical despite different names*

### Comparing `oxdork-3.1.0/oxdork.egg-info/PKG-INFO` & `oxdork-3.1.1/oxdork.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: oxdork
-Version: 3.1.0
+Version: 3.1.1
 Summary: Google dorking tool
 Author-email: Richard Mwewa <rly0nheart@duck.com>
 License: MIT License
         
         Copyright (c) 2022 Richard Mwewa
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
@@ -61,8 +61,8 @@
 
 
 # Queries
 A collection of 5,568 common dork queries [here](https://github.com/rly0nheart/oxdork/tree/master/dork_queries)
 
 
 # Support
-<a href="https://www.buymeacoffee.com/189381184" target="_blank"><img src="https://cdn.buymeacoffee.com/buttons/default-orange.png" alt="Buy Me A Coffee" height="41" width="174"></a>
+<a href="https://www.buymeacoffee.com/_rly0nheart" target="_blank"><img src="https://cdn.buymeacoffee.com/buttons/default-orange.png" alt="Buy Me A Coffee" height="41" width="174"></a>
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: oxdork Version: 3.1.0 Summary: Google dorking tool
+Metadata-Version: 2.1 Name: oxdork Version: 3.1.1 Summary: Google dorking tool
 Author-email: Richard Mwewa
 duck.com> License: MIT License Copyright (c) 2022 Richard Mwewa Permission is
 hereby granted, free of charge, to any person obtaining a copy of this software
 and associated documentation files (the "Software"), to deal in the Software
 without restriction, including without limitation the rights to use, copy,
 modify, merge, publish, distribute, sublicense, and/or sell copies of the
 Software, and to permit persons to whom the Software is furnished to do so,
```

### Comparing `oxdork-3.1.0/pyproject.toml` & `oxdork-3.1.1/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 build-backend = "setuptools.build_meta"
 
 [tool.setuptools]
 packages = ["oxdork"]
 
 [project]
 name = "oxdork"
-version = "3.1.0"
+version = "3.1.1"
 description = "Google dorking tool"
 readme = "README.md"
 requires-python = ">=3.8"
 license = {file = "LICENSE"}
 keywords = ["python", "osint", "google-dorking", "osint", "inurl", "intext", "intitle"]
 authors = [{name = "Richard Mwewa", email = "rly0nheart@duck.com"}]
 classifiers = [
```

