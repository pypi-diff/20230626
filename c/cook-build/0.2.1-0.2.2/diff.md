# Comparing `tmp/cook-build-0.2.1.tar.gz` & `tmp/cook-build-0.2.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cook-build-0.2.1.tar", last modified: Sat Apr 29 00:26:26 2023, max compression
+gzip compressed data, was "cook-build-0.2.2.tar", last modified: Mon Jun 26 21:14:30 2023, max compression
```

## Comparing `cook-build-0.2.1.tar` & `cook-build-0.2.2.tar`

### file list

```diff
@@ -1,30 +1,30 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-29 00:26:26.662414 cook-build-0.2.1/
--rw-r--r--   0 runner    (1001) docker     (123)     1500 2023-04-29 00:26:04.000000 cook-build-0.2.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     3676 2023-04-29 00:26:26.662414 cook-build-0.2.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     3539 2023-04-29 00:26:04.000000 cook-build-0.2.1/README.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-29 00:26:26.662414 cook-build-0.2.1/cook/
--rw-r--r--   0 runner    (1001) docker     (123)      180 2023-04-29 00:26:04.000000 cook-build-0.2.1/cook/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7765 2023-04-29 00:26:04.000000 cook-build-0.2.1/cook/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4753 2023-04-29 00:26:04.000000 cook-build-0.2.1/cook/actions.py
--rw-r--r--   0 runner    (1001) docker     (123)     8735 2023-04-29 00:26:04.000000 cook-build-0.2.1/cook/contexts.py
--rw-r--r--   0 runner    (1001) docker     (123)     7885 2023-04-29 00:26:04.000000 cook-build-0.2.1/cook/controller.py
--rw-r--r--   0 runner    (1001) docker     (123)     4604 2023-04-29 00:26:04.000000 cook-build-0.2.1/cook/manager.py
--rw-r--r--   0 runner    (1001) docker     (123)     1232 2023-04-29 00:26:04.000000 cook-build-0.2.1/cook/task.py
--rw-r--r--   0 runner    (1001) docker     (123)     2055 2023-04-29 00:26:04.000000 cook-build-0.2.1/cook/util.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-29 00:26:26.662414 cook-build-0.2.1/cook_build.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     3676 2023-04-29 00:26:26.000000 cook-build-0.2.1/cook_build.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      524 2023-04-29 00:26:26.000000 cook-build-0.2.1/cook_build.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-29 00:26:26.000000 cook-build-0.2.1/cook_build.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       48 2023-04-29 00:26:26.000000 cook-build-0.2.1/cook_build.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)        9 2023-04-29 00:26:26.000000 cook-build-0.2.1/cook_build.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        5 2023-04-29 00:26:26.000000 cook-build-0.2.1/cook_build.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      274 2023-04-29 00:26:26.662414 cook-build-0.2.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      751 2023-04-29 00:26:04.000000 cook-build-0.2.1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-29 00:26:26.662414 cook-build-0.2.1/tests/
--rw-r--r--   0 runner    (1001) docker     (123)     1245 2023-04-29 00:26:04.000000 cook-build-0.2.1/tests/test_actions.py
--rw-r--r--   0 runner    (1001) docker     (123)     3071 2023-04-29 00:26:04.000000 cook-build-0.2.1/tests/test_contexts.py
--rw-r--r--   0 runner    (1001) docker     (123)     5684 2023-04-29 00:26:04.000000 cook-build-0.2.1/tests/test_controller.py
--rw-r--r--   0 runner    (1001) docker     (123)      296 2023-04-29 00:26:04.000000 cook-build-0.2.1/tests/test_examples.py
--rw-r--r--   0 runner    (1001) docker     (123)     2172 2023-04-29 00:26:04.000000 cook-build-0.2.1/tests/test_main.py
--rw-r--r--   0 runner    (1001) docker     (123)     2339 2023-04-29 00:26:04.000000 cook-build-0.2.1/tests/test_manager.py
--rw-r--r--   0 runner    (1001) docker     (123)      240 2023-04-29 00:26:04.000000 cook-build-0.2.1/tests/test_util.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 21:14:30.070451 cook-build-0.2.2/
+-rw-r--r--   0 runner    (1001) docker     (123)     1500 2023-06-26 21:14:00.000000 cook-build-0.2.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     3676 2023-06-26 21:14:30.070451 cook-build-0.2.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3539 2023-06-26 21:14:00.000000 cook-build-0.2.2/README.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 21:14:30.066450 cook-build-0.2.2/cook/
+-rw-r--r--   0 runner    (1001) docker     (123)      180 2023-06-26 21:14:00.000000 cook-build-0.2.2/cook/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7765 2023-06-26 21:14:00.000000 cook-build-0.2.2/cook/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4753 2023-06-26 21:14:00.000000 cook-build-0.2.2/cook/actions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8893 2023-06-26 21:14:00.000000 cook-build-0.2.2/cook/contexts.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7885 2023-06-26 21:14:00.000000 cook-build-0.2.2/cook/controller.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4604 2023-06-26 21:14:00.000000 cook-build-0.2.2/cook/manager.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1232 2023-06-26 21:14:00.000000 cook-build-0.2.2/cook/task.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2055 2023-06-26 21:14:00.000000 cook-build-0.2.2/cook/util.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 21:14:30.070451 cook-build-0.2.2/cook_build.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     3676 2023-06-26 21:14:29.000000 cook-build-0.2.2/cook_build.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      524 2023-06-26 21:14:30.000000 cook-build-0.2.2/cook_build.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-26 21:14:29.000000 cook-build-0.2.2/cook_build.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       48 2023-06-26 21:14:29.000000 cook-build-0.2.2/cook_build.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        9 2023-06-26 21:14:29.000000 cook-build-0.2.2/cook_build.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        5 2023-06-26 21:14:29.000000 cook-build-0.2.2/cook_build.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      274 2023-06-26 21:14:30.070451 cook-build-0.2.2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      751 2023-06-26 21:14:00.000000 cook-build-0.2.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 21:14:30.070451 cook-build-0.2.2/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     1245 2023-06-26 21:14:00.000000 cook-build-0.2.2/tests/test_actions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3617 2023-06-26 21:14:00.000000 cook-build-0.2.2/tests/test_contexts.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5684 2023-06-26 21:14:00.000000 cook-build-0.2.2/tests/test_controller.py
+-rw-r--r--   0 runner    (1001) docker     (123)      296 2023-06-26 21:14:00.000000 cook-build-0.2.2/tests/test_examples.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2172 2023-06-26 21:14:00.000000 cook-build-0.2.2/tests/test_main.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2339 2023-06-26 21:14:00.000000 cook-build-0.2.2/tests/test_manager.py
+-rw-r--r--   0 runner    (1001) docker     (123)      240 2023-06-26 21:14:00.000000 cook-build-0.2.2/tests/test_util.py
```

### Comparing `cook-build-0.2.1/LICENSE` & `cook-build-0.2.2/LICENSE`

 * *Files identical despite different names*

### Comparing `cook-build-0.2.1/PKG-INFO` & `cook-build-0.2.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cook-build
-Version: 0.2.1
+Version: 0.2.2
 Requires-Python: >=3.8
 Description-Content-Type: text/x-rst
 License-File: LICENSE
 
 🧑‍🍳 Cook
 ==========
```

### Comparing `cook-build-0.2.1/README.rst` & `cook-build-0.2.2/README.rst`

 * *Files identical despite different names*

### Comparing `cook-build-0.2.1/cook/__main__.py` & `cook-build-0.2.2/cook/__main__.py`

 * *Files identical despite different names*

### Comparing `cook-build-0.2.1/cook/actions.py` & `cook-build-0.2.2/cook/actions.py`

 * *Files identical despite different names*

### Comparing `cook-build-0.2.1/cook/contexts.py` & `cook-build-0.2.2/cook/contexts.py`

 * *Files 2% similar despite different names*

```diff
@@ -126,19 +126,22 @@
     .. note::
 
         This context is active by default.
     """
     def apply(self, task: "Task") -> Task:
         for target in task.targets:
             name = f"_create_target_directories:{target.parent}"
-            if name in self.manager.tasks or target.parent.is_dir():
+            # No need to create a task if the parent already exists.
+            if target.parent.is_dir():
                 continue
-            create = self.manager.create_task(name, action=actions.FunctionAction(
-                lambda _: target.parent.mkdir(parents=True, exist_ok=True)
-            ))
+            # Create a task if necessary.
+            if (create := self.manager.tasks.get(name)) is None:
+                create = self.manager.create_task(name, action=actions.FunctionAction(
+                    lambda _: target.parent.mkdir(parents=True, exist_ok=True)
+                ))
             task.task_dependencies.append(create)
         return task
 
 
 class normalize_action(Context):
     """
     Normalize actions of tasks.
```

### Comparing `cook-build-0.2.1/cook/controller.py` & `cook-build-0.2.2/cook/controller.py`

 * *Files identical despite different names*

### Comparing `cook-build-0.2.1/cook/manager.py` & `cook-build-0.2.2/cook/manager.py`

 * *Files identical despite different names*

### Comparing `cook-build-0.2.1/cook/task.py` & `cook-build-0.2.2/cook/task.py`

 * *Files identical despite different names*

### Comparing `cook-build-0.2.1/cook/util.py` & `cook-build-0.2.2/cook/util.py`

 * *Files identical despite different names*

### Comparing `cook-build-0.2.1/cook_build.egg-info/PKG-INFO` & `cook-build-0.2.2/cook_build.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cook-build
-Version: 0.2.1
+Version: 0.2.2
 Requires-Python: >=3.8
 Description-Content-Type: text/x-rst
 License-File: LICENSE
 
 🧑‍🍳 Cook
 ==========
```

### Comparing `cook-build-0.2.1/cook_build.egg-info/SOURCES.txt` & `cook-build-0.2.2/cook_build.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `cook-build-0.2.1/setup.py` & `cook-build-0.2.2/setup.py`

 * *Files 14% similar despite different names*

```diff
@@ -10,15 +10,15 @@
     .replace(":class:", ":code:") \
     .replace(".. toctree::", "..") \
     .replace(".. sh::", "..")
 
 
 setup(
     name="cook-build",
-    version="0.2.1",
+    version="0.2.2",
     long_description=long_description,
     long_description_content_type="text/x-rst",
     python_requires=">=3.8",
     install_requires=[
         "colorama",
     ],
     packages=find_packages(),
```

### Comparing `cook-build-0.2.1/tests/test_actions.py` & `cook-build-0.2.2/tests/test_actions.py`

 * *Files identical despite different names*

### Comparing `cook-build-0.2.1/tests/test_contexts.py` & `cook-build-0.2.2/tests/test_contexts.py`

 * *Files 13% similar despite different names*

```diff
@@ -43,14 +43,27 @@
     assert not filename.parent.is_dir()
 
     controller = Controller(m, conn)
     controller.execute_sync(task)
     assert filename.parent.is_dir()
 
 
+def test_create_target_directories_with_multiple_targets(m: Manager, tmp_wd: Path, conn: sqlite3) \
+        -> None:
+    filenames = [tmp_wd / "this/is/a/hierarchy.txt", tmp_wd / "this/is/a/hierarchy2.txt"]
+    with normalize_action(), create_target_directories():
+        for filename in filenames:
+            task = m.create_task(filename.name, targets=[filename], action=["touch", filename])
+    assert not filename.parent.is_dir()
+
+    controller = Controller(m, conn)
+    controller.execute_sync(task)
+    assert filename.parent.is_dir()
+
+
 def test_normalize_action(m: Manager) -> None:
     with normalize_action():
         task = m.create_task("foo", action="bar")
         assert isinstance(task.action, ShellAction) and task.action.cmd == "bar"
 
         task = m.create_task("bar", action=["baz"])
         assert isinstance(task.action, SubprocessAction) and task.action.program == "baz"
```

### Comparing `cook-build-0.2.1/tests/test_controller.py` & `cook-build-0.2.2/tests/test_controller.py`

 * *Files identical despite different names*

### Comparing `cook-build-0.2.1/tests/test_main.py` & `cook-build-0.2.2/tests/test_main.py`

 * *Files identical despite different names*

### Comparing `cook-build-0.2.1/tests/test_manager.py` & `cook-build-0.2.2/tests/test_manager.py`

 * *Files identical despite different names*

