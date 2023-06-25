# Comparing `tmp/bare_estate-0.3.tar.gz` & `tmp/bare_estate-0.4.tar.gz`

## Comparing `bare_estate-0.3.tar` & `bare_estate-0.4.tar`

### file list

```diff
@@ -1,11 +1,11 @@
--rw-r--r--   0        0        0      569 2020-02-02 00:00:00.000000 bare_estate-0.3/CHANGELOG.md
--rw-r--r--   0        0        0      619 2020-02-02 00:00:00.000000 bare_estate-0.3/actions.mk
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 bare_estate-0.3/bare_estate/__init__.py
--rw-r--r--   0        0        0     1044 2020-02-02 00:00:00.000000 bare_estate-0.3/bare_estate/cli.py
--rw-r--r--   0        0        0     2831 2020-02-02 00:00:00.000000 bare_estate-0.3/bare_estate/commands.py
--rw-r--r--   0        0        0      801 2020-02-02 00:00:00.000000 bare_estate-0.3/bare_estate/config.py
--rw-r--r--   0        0        0       57 2020-02-02 00:00:00.000000 bare_estate-0.3/.gitignore
--rw-r--r--   0        0        0     1074 2020-02-02 00:00:00.000000 bare_estate-0.3/LICENSE
--rw-r--r--   0        0        0     2624 2020-02-02 00:00:00.000000 bare_estate-0.3/README.md
--rw-r--r--   0        0        0      693 2020-02-02 00:00:00.000000 bare_estate-0.3/pyproject.toml
--rw-r--r--   0        0        0     3080 2020-02-02 00:00:00.000000 bare_estate-0.3/PKG-INFO
+-rw-r--r--   0        0        0      722 2020-02-02 00:00:00.000000 bare_estate-0.4/CHANGELOG.md
+-rw-r--r--   0        0        0      619 2020-02-02 00:00:00.000000 bare_estate-0.4/actions.mk
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 bare_estate-0.4/bare_estate/__init__.py
+-rw-r--r--   0        0        0     1044 2020-02-02 00:00:00.000000 bare_estate-0.4/bare_estate/cli.py
+-rw-r--r--   0        0        0     2831 2020-02-02 00:00:00.000000 bare_estate-0.4/bare_estate/commands.py
+-rw-r--r--   0        0        0      748 2020-02-02 00:00:00.000000 bare_estate-0.4/bare_estate/config.py
+-rw-r--r--   0        0        0       57 2020-02-02 00:00:00.000000 bare_estate-0.4/.gitignore
+-rw-r--r--   0        0        0     1074 2020-02-02 00:00:00.000000 bare_estate-0.4/LICENSE
+-rw-r--r--   0        0        0     2848 2020-02-02 00:00:00.000000 bare_estate-0.4/README.md
+-rw-r--r--   0        0        0      693 2020-02-02 00:00:00.000000 bare_estate-0.4/pyproject.toml
+-rw-r--r--   0        0        0     3304 2020-02-02 00:00:00.000000 bare_estate-0.4/PKG-INFO
```

### Comparing `bare_estate-0.3/CHANGELOG.md` & `bare_estate-0.4/CHANGELOG.md`

 * *Files 23% similar despite different names*

```diff
@@ -1,7 +1,17 @@
+## 0.4.0 - 2023-06-25
+
+### Added
+
+- Add support for the XDG_DATA_HOME environment variable.
+
+### Fixed
+
+- Fix application when no config file is found.
+
 ## 0.3.0 - 2023-06-03
 
 ### Added
 
 - Add base directory to config options. Now you can create repositories using
 other directories as base, instead of just HOME.
 - Add support for default configs. Now the program works even without a
```

### Comparing `bare_estate-0.3/actions.mk` & `bare_estate-0.4/actions.mk`

 * *Files identical despite different names*

### Comparing `bare_estate-0.3/bare_estate/cli.py` & `bare_estate-0.4/bare_estate/cli.py`

 * *Files identical despite different names*

### Comparing `bare_estate-0.3/bare_estate/commands.py` & `bare_estate-0.4/bare_estate/commands.py`

 * *Files identical despite different names*

### Comparing `bare_estate-0.3/LICENSE` & `bare_estate-0.4/LICENSE`

 * *Files identical despite different names*

### Comparing `bare_estate-0.3/README.md` & `bare_estate-0.4/README.md`

 * *Files 8% similar despite different names*

```diff
@@ -33,21 +33,25 @@
 `${HOME}/.config/bare_estate.json`.
 
 ### Config Options:
 
 - history_location: it says where your bare repository directory will be
 located. Environment variables don't expand. So you will have to write the
 complete path of the file.
+- base_directory: the directory from where you will manage all your dotfiles.
+You can either put them directly in the base directory, or in subdirectories
+within it.
 
 ### Examples:
 
 bare_estate.json:
-```
+```json
 {
-  "history_location": "/home/lucas/.dotfiles"
+    "history_location": "/home/lucas/.local/share/bare_estate",
+    "base_directory": "/home/lucas"
 }
 ```
 
 ## Usage
 
 The package introduces an executable script called `estate` as the main
 entrypoint for the application. It is used just like you would use git.
```

### Comparing `bare_estate-0.3/pyproject.toml` & `bare_estate-0.4/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -9,15 +9,15 @@
     "dev_requirements.txt",
     ".?*",
     "estate",
 ]
 
 [project]
 name = "bare_estate"
-version = "0.3"
+version = "0.4"
 authors = [
     { name="Lucas L. S. Haine", email="lucaslshaine@gmail.com" },
 ]
 description = "Manage your dotfiles seamlessly with a bare repo"
 readme = "README.md"
 requires-python = ">=3.7"
 classifiers = [
```

### Comparing `bare_estate-0.3/PKG-INFO` & `bare_estate-0.4/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: bare_estate
-Version: 0.3
+Version: 0.4
 Summary: Manage your dotfiles seamlessly with a bare repo
 Project-URL: Homepage, https://github.com/llucasls/bare-estate
 Author-email: "Lucas L. S. Haine" <lucaslshaine@gmail.com>
 License-File: LICENSE
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: POSIX
 Classifier: Programming Language :: Python :: 3
@@ -46,21 +46,25 @@
 `${HOME}/.config/bare_estate.json`.
 
 ### Config Options:
 
 - history_location: it says where your bare repository directory will be
 located. Environment variables don't expand. So you will have to write the
 complete path of the file.
+- base_directory: the directory from where you will manage all your dotfiles.
+You can either put them directly in the base directory, or in subdirectories
+within it.
 
 ### Examples:
 
 bare_estate.json:
-```
+```json
 {
-  "history_location": "/home/lucas/.dotfiles"
+    "history_location": "/home/lucas/.local/share/bare_estate",
+    "base_directory": "/home/lucas"
 }
 ```
 
 ## Usage
 
 The package introduces an executable script called `estate` as the main
 entrypoint for the application. It is used just like you would use git.
```

