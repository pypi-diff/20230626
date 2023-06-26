# Comparing `tmp/bpy_addon_build-0.1.7.tar.gz` & `tmp/bpy_addon_build-0.1.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "bpy_addon_build-0.1.7.tar", max compression
+gzip compressed data, was "bpy_addon_build-0.1.8.tar", max compression
```

## Comparing `bpy_addon_build-0.1.7.tar` & `bpy_addon_build-0.1.8.tar`

### file list

```diff
@@ -1,5 +1,5 @@
--rw-r--r--   0        0        0     4770 2023-05-15 23:17:22.409369 bpy_addon_build-0.1.7/bpy_addon_build/__init__.py
--rw-r--r--   0        0        0     1141 2023-05-15 23:40:10.223641 bpy_addon_build-0.1.7/bpy_addon_build/actions.py
--rw-r--r--   0        0        0     1021 2023-05-15 23:16:32.883680 bpy_addon_build-0.1.7/bpy_addon_build/yaml_conf.py
--rw-r--r--   0        0        0      548 2023-05-15 23:40:30.227513 bpy_addon_build-0.1.7/pyproject.toml
--rw-r--r--   0        0        0      730 1970-01-01 00:00:00.000000 bpy_addon_build-0.1.7/PKG-INFO
+-rw-r--r--   0        0        0     4770 2023-06-26 06:31:43.813373 bpy_addon_build-0.1.8/bpy_addon_build/__init__.py
+-rw-r--r--   0        0        0     1642 2023-06-26 06:57:34.395633 bpy_addon_build-0.1.8/bpy_addon_build/actions.py
+-rw-r--r--   0        0        0     1021 2023-06-26 06:24:00.511775 bpy_addon_build-0.1.8/bpy_addon_build/yaml_conf.py
+-rw-r--r--   0        0        0      548 2023-06-26 06:26:02.362017 bpy_addon_build-0.1.8/pyproject.toml
+-rw-r--r--   0        0        0      730 1970-01-01 00:00:00.000000 bpy_addon_build-0.1.8/PKG-INFO
```

### Comparing `bpy_addon_build-0.1.7/bpy_addon_build/__init__.py` & `bpy_addon_build-0.1.8/bpy_addon_build/__init__.py`

 * *Files identical despite different names*

### Comparing `bpy_addon_build-0.1.7/bpy_addon_build/actions.py` & `bpy_addon_build-0.1.8/bpy_addon_build/actions.py`

 * *Files 24% similar despite different names*

```diff
@@ -2,32 +2,52 @@
 import shlex
 from typing import List
 from pathlib import Path
 import shutil
 import re
 from rich.console import Console
 
+
 # Execute an action
 def execute_action(action: str, inter_dir: Path, console: Console):
-    extracted_str = re.search("\((.+?)\)", action)
-    if not extracted_str:
-        console.print(
-            f"Invalid action: {action}, perhaps you forgot parenthesis?",
-            style="[bold red]"
-        )
-        quit()
+    print(action)
+    if isinstance(action, list):
+        for cmd in action:
+            command = shlex.split(cmd)
+            output = subprocess.run(
+                command,
+                shell=True,
+                cwd=inter_dir,
+                stdout=subprocess.PIPE,
+                stderr=subprocess.STDOUT,
+            )
+            console.print(output.stdout.decode("UTF-8"))
+
+    elif "create_file" in action:
+        extracted_str = re.search("\((.+?)\)", action)
+        if not extracted_str:
+            console.print(
+                f"Invalid action: {action}, perhaps you forgot parenthesis?",
+                style="bold red",
+            )
+            quit()
 
-    if "create_file" in action:
         file_path = inter_dir / Path(extracted_str.group(1).replace('"', ""))
         with open(file_path, "w") as f:
             f.write("")
 
-    if "copy_file" in action:
+    elif "copy_file" in action:
+        extracted_str = re.search("\((.+?)\)", action)
+        if not extracted_str:
+            console.print(
+                f"Invalid action: {action}, perhaps you forgot parenthesis?",
+                style="bold red",
+            )
+
         files: List[str] = extracted_str.group(1).split("->")
         src: Path = Path(files[0].replace('"', "")).expanduser()
         dst: Path = inter_dir / Path(files[1].replace('"', ""))
         shutil.copy2(src, dst)
 
-    if "execute_sh" in action:
-        command = shlex.split(extracted_str.group(1))
-        output = subprocess.run(command, shell=True, cwd=inter_dir, stdout=subprocess.PIPE, stderr=subprocess.STDOUT)
-        console.print(output.stdout.decode("UTF-8"))
+    else:
+        console.print(f"Unknown action {action}!", style="bold red")
+        quit()
```

### Comparing `bpy_addon_build-0.1.7/bpy_addon_build/yaml_conf.py` & `bpy_addon_build-0.1.8/bpy_addon_build/yaml_conf.py`

 * *Files identical despite different names*

### Comparing `bpy_addon_build-0.1.7/pyproject.toml` & `bpy_addon_build-0.1.8/pyproject.toml`

 * *Files 23% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "bpy-addon-build"
-version = "0.1.7"
+version = "0.1.8"
 description = "A build system to make building and testing Blender addons 10 times easier"
 authors = ["StandingPad"]
 license = "MIT"
 homepage = "https://github.com/StandingPadAnimations/bpy-build"
 
 [tool.poetry.dependencies]
 python = "^3.7"
```

### Comparing `bpy_addon_build-0.1.7/PKG-INFO` & `bpy_addon_build-0.1.8/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: bpy-addon-build
-Version: 0.1.7
+Version: 0.1.8
 Summary: A build system to make building and testing Blender addons 10 times easier
 Home-page: https://github.com/StandingPadAnimations/bpy-build
 License: MIT
 Author: StandingPad
 Requires-Python: >=3.7,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
```

