# Comparing `tmp/REMLA23Team09LibProject-0.0.1.tar.gz` & `tmp/REMLA23Team09LibProject-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist\REMLA23Team09LibProject-0.0.1.tar", last modified: Sun Jun 25 22:27:37 2023, max compression
+gzip compressed data, was "REMLA23Team09LibProject-0.0.2.tar", last modified: Sun Jun 25 23:18:12 2023, max compression
```

## Comparing `REMLA23Team09LibProject-0.0.1.tar` & `REMLA23Team09LibProject-0.0.2.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxrwxrwx   0        0        0        0 2023-06-25 22:27:37.451171 REMLA23Team09LibProject-0.0.1/
--rw-rw-rw-   0        0        0      284 2023-06-25 22:27:37.435393 REMLA23Team09LibProject-0.0.1/PKG-INFO
--rw-rw-rw-   0        0        0      167 2023-05-08 20:51:51.000000 REMLA23Team09LibProject-0.0.1/README.md
-drwxrwxrwx   0        0        0        0 2023-06-25 22:27:37.435393 REMLA23Team09LibProject-0.0.1/REMLA23Team09LibProject.egg-info/
--rw-rw-rw-   0        0        0      284 2023-06-25 22:27:37.000000 REMLA23Team09LibProject-0.0.1/REMLA23Team09LibProject.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      287 2023-06-25 22:27:37.000000 REMLA23Team09LibProject-0.0.1/REMLA23Team09LibProject.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-25 22:27:37.000000 REMLA23Team09LibProject-0.0.1/REMLA23Team09LibProject.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        9 2023-06-25 22:27:37.000000 REMLA23Team09LibProject-0.0.1/REMLA23Team09LibProject.egg-info/requires.txt
--rw-rw-rw-   0        0        0        4 2023-06-25 22:27:37.000000 REMLA23Team09LibProject-0.0.1/REMLA23Team09LibProject.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-06-25 22:27:37.451171 REMLA23Team09LibProject-0.0.1/setup.cfg
--rw-rw-rw-   0        0        0      511 2023-06-25 22:27:24.000000 REMLA23Team09LibProject-0.0.1/setup.py
-drwxrwxrwx   0        0        0        0 2023-06-25 22:27:37.435393 REMLA23Team09LibProject-0.0.1/src/
--rw-rw-rw-   0        0        0      743 2023-06-25 22:26:04.000000 REMLA23Team09LibProject-0.0.1/src/VersionUtil.py
--rw-rw-rw-   0        0        0       78 2023-05-08 20:39:49.000000 REMLA23Team09LibProject-0.0.1/src/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-25 23:18:12.136727 REMLA23Team09LibProject-0.0.2/
+-rw-r--r--   0 runner    (1001) docker     (123)      244 2023-06-25 23:18:12.136727 REMLA23Team09LibProject-0.0.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      169 2023-06-25 23:18:02.000000 REMLA23Team09LibProject-0.0.2/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-25 23:18:12.136727 REMLA23Team09LibProject-0.0.2/REMLA23Team09LibProject.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      244 2023-06-25 23:18:12.000000 REMLA23Team09LibProject-0.0.2/REMLA23Team09LibProject.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      287 2023-06-25 23:18:12.000000 REMLA23Team09LibProject-0.0.2/REMLA23Team09LibProject.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-25 23:18:12.000000 REMLA23Team09LibProject-0.0.2/REMLA23Team09LibProject.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        9 2023-06-25 23:18:12.000000 REMLA23Team09LibProject-0.0.2/REMLA23Team09LibProject.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        4 2023-06-25 23:18:12.000000 REMLA23Team09LibProject-0.0.2/REMLA23Team09LibProject.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-25 23:18:12.136727 REMLA23Team09LibProject-0.0.2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      492 2023-06-25 23:18:11.000000 REMLA23Team09LibProject-0.0.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-25 23:18:12.136727 REMLA23Team09LibProject-0.0.2/src/
+-rw-r--r--   0 runner    (1001) docker     (123)      715 2023-06-25 23:18:02.000000 REMLA23Team09LibProject-0.0.2/src/VersionUtil.py
+-rw-r--r--   0 runner    (1001) docker     (123)       77 2023-06-25 23:18:02.000000 REMLA23Team09LibProject-0.0.2/src/__init__.py
```

### Comparing `REMLA23Team09LibProject-0.0.1/src/VersionUtil.py` & `REMLA23Team09LibProject-0.0.2/src/VersionUtil.py`

 * *Ordering differences only*

 * *Files 18% similar despite different names*

```diff
@@ -1,29 +1,29 @@
-import subprocess
-
-
-class VersionUtil:
-    @staticmethod
-    def get_version():
-        try:
-            version_info = subprocess.check_output(["git", "describe", "--tags"]).decode().strip()
-
-            version_parts = version_info.split('-')
-
-            if len(version_parts) > 1:
-                tag, commits, commit_hash = version_parts[:3]
-                version = tag[1:]
-            else:
-                version = version_info
-
-        except subprocess.CalledProcessError:
-            version = "Unknown"
-
-        return version
-
-
-## How to call this function to check the version:
-
-# from lib.versionutil import VersionUtil
-#
-# version = VersionUtil.get_version()
+import subprocess
+
+
+class VersionUtil:
+    @staticmethod
+    def get_version():
+        try:
+            version_info = subprocess.check_output(["git", "describe", "--tags"]).decode().strip()
+
+            version_parts = version_info.split('-')
+
+            if len(version_parts) > 1:
+                tag, commits, commit_hash = version_parts[:3]
+                version = tag[1:]
+            else:
+                version = version_info
+
+        except subprocess.CalledProcessError:
+            version = "Unknown"
+
+        return version
+
+
+## How to call this function to check the version:
+
+# from lib.versionutil import VersionUtil
+#
+# version = VersionUtil.get_version()
 # print(f"Library version: {version}")
```

