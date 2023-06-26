# Comparing `tmp/docker_shaper-0.1.2.tar.gz` & `tmp/docker_shaper-0.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "docker_shaper-0.1.2.tar", max compression
+gzip compressed data, was "docker_shaper-0.1.3.tar", max compression
```

## Comparing `docker_shaper-0.1.2.tar` & `docker_shaper-0.1.3.tar`

### file list

```diff
@@ -1,11 +1,18 @@
--rw-r--r--   0        0        0     2140 2023-06-22 11:46:34.742492 docker_shaper-0.1.2/Readme.md
--rw-r--r--   0        0        0        0 2023-06-22 08:21:29.063512 docker_shaper-0.1.2/docker_shaper/__init__.py
--rwxr-xr-x   0        0        0     1459 2023-06-22 14:10:38.638778 docker_shaper-0.1.2/docker_shaper/cli.py
--rw-r--r--   0        0        0        0 2023-06-22 08:30:25.674562 docker_shaper-0.1.2/docker_shaper/common.py
--rw-r--r--   0        0        0     2502 2023-06-22 15:03:04.151806 docker_shaper-0.1.2/docker_shaper/docker_stuff.py
--rw-r--r--   0        0        0     3977 2023-06-22 13:56:29.288322 docker_shaper-0.1.2/docker_shaper/dynamic.py
--rw-r--r--   0        0        0     8379 2023-06-22 15:03:04.195806 docker_shaper-0.1.2/docker_shaper/server.py
--rw-r--r--   0        0        0      149 2023-06-22 09:02:28.913379 docker_shaper-0.1.2/docker_shaper/templates/result.html
--rw-r--r--   0        0        0     4907 2023-06-22 15:03:03.603804 docker_shaper-0.1.2/docker_shaper/utils.py
--rw-r--r--   0        0        0     2171 2023-06-22 15:05:30.024252 docker_shaper-0.1.2/pyproject.toml
--rw-r--r--   0        0        0     2852 1970-01-01 00:00:00.000000 docker_shaper-0.1.2/PKG-INFO
+-rw-r--r--   0        0        0     2299 2023-06-23 11:06:28.356138 docker_shaper-0.1.3/Readme.md
+-rw-r--r--   0        0        0        0 2023-06-23 11:06:28.356138 docker_shaper-0.1.3/docker_shaper/__init__.py
+-rwxr-xr-x   0        0        0     1459 2023-06-23 11:06:28.356138 docker_shaper-0.1.3/docker_shaper/cli.py
+-rw-r--r--   0        0        0        0 2023-06-23 11:06:28.356138 docker_shaper-0.1.3/docker_shaper/common.py
+-rw-r--r--   0        0        0        1 2023-06-26 12:05:10.251336 docker_shaper-0.1.3/docker_shaper/docker_stuff.py
+-rw-r--r--   0        0        0    13194 2023-06-26 15:22:16.795198 docker_shaper-0.1.3/docker_shaper/dynamic.py
+-rw-r--r--   0        0        0     6488 2023-06-26 14:51:02.321955 docker_shaper-0.1.3/docker_shaper/server.py
+-rw-r--r--   0        0        0        0 2023-06-26 15:27:42.516049 docker_shaper-0.1.3/docker_shaper/static/__init__.py
+-rw-r--r--   0        0        0   155631 2023-06-23 06:50:12.242199 docker_shaper-0.1.3/docker_shaper/static/base.css
+-rw-r--r--   0        0        0     9017 2023-06-26 07:29:52.330340 docker_shaper-0.1.3/docker_shaper/static/normalize.css
+-rw-r--r--   0        0        0     6108 2023-06-26 07:36:31.223451 docker_shaper-0.1.3/docker_shaper/static/pills.css
+-rw-r--r--   0        0        0     2474 2023-06-26 07:30:04.714374 docker_shaper-0.1.3/docker_shaper/static/style.css
+-rw-r--r--   0        0        0        0 2023-06-26 15:27:53.160076 docker_shaper-0.1.3/docker_shaper/templates/__init__.py
+-rw-r--r--   0        0        0      528 2023-06-26 15:29:05.292266 docker_shaper-0.1.3/docker_shaper/templates/base.html
+-rw-r--r--   0        0        0     1749 2023-06-26 15:18:56.202659 docker_shaper-0.1.3/docker_shaper/templates/dashboard.html
+-rw-r--r--   0        0        0     4641 2023-06-26 14:51:01.673953 docker_shaper-0.1.3/docker_shaper/utils.py
+-rw-r--r--   0        0        0     2209 2023-06-26 15:29:39.828358 docker_shaper-0.1.3/pyproject.toml
+-rw-r--r--   0        0        0     3011 1970-01-01 00:00:00.000000 docker_shaper-0.1.3/PKG-INFO
```

### Comparing `docker_shaper-0.1.2/Readme.md` & `docker_shaper-0.1.3/Readme.md`

 * *Files 8% similar despite different names*

```diff
@@ -17,23 +17,23 @@
 
 
 ## Development & Contribution
 
 ### Todo
 
 - [x] pip package
-- [x] quart interface
-- [ ] increase/decrease logging
+- [x] Quart interface
+- [ ] bring in dockermon
+- [ ] auto update
 - [ ] bring in dgcd
-- [ ] untag certain tags
-- [ ] outsource config
 - [ ] bring in list_volumes
-- [ ] dockermon
-- [ ] container cleanup
-- [ ] Quart interface
+- [ ] outsource config
+- [ ] 	increase/decrease logging
+- [ ] new: untag certain tags
+- [ ] new: container cleanup
 
 
 ### Setup
 
 ### Prerequisites
 
 * Python 3.8.10
@@ -76,12 +76,13 @@
   - check installed package
   - go through review process
   - publish the new package `poetry publish --build --repository checkmk`
   - commit new version && push
 
 
 ## Knowledge
-
+https://github.com/torfsen/python-systemd-tutorial
+https://www.digitalocean.com/community/tutorials/how-to-use-templates-in-a-flask-application
 * https://blog.miguelgrinberg.com/post/beautiful-interactive-tables-for-your-flask-templates
 * https://stackoverflow.com/questions/49957034/live-updating-dynamic-variable-on-html-with-flask
 * https://pgjones.gitlab.io/quart/how_to_guides/templating.html
```

### Comparing `docker_shaper-0.1.2/docker_shaper/cli.py` & `docker_shaper-0.1.3/docker_shaper/cli.py`

 * *Files identical despite different names*

### Comparing `docker_shaper-0.1.2/docker_shaper/utils.py` & `docker_shaper-0.1.3/docker_shaper/utils.py`

 * *Files 6% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 import os
 import shlex
 from functools import wraps
 from pathlib import Path
 from subprocess import DEVNULL, CalledProcessError, check_output, run
 
 # we need 3.8 compatible typing (python on build nodes)
-from typing import Callable, Coroutine, Set, cast
+from typing import Callable, Coroutine, Iterator, Union, cast
 
 from asyncinotify import Event, Inotify, Mask
 
 LOG_LEVELS = ("DEBUG", "INFO", "WARNING", "ERROR", "CRITICAL")
 
 
 def log() -> logging.Logger:
@@ -59,41 +59,39 @@
             log().exception("Exception in `%s`:", afunc.__name__)
             asyncio.get_event_loop().stop()
         return None
 
     return run
 
 
-@watchdog
-async def watch_changes(
-    path: Path,
-    callback: Callable[[Set[Path]], None],
-    *,
+async def fs_changes(
+    *paths: Path,
     queue: asyncio.Queue = asyncio.Queue(),
     mask: Mask = Mask.CLOSE_WRITE | Mask.MOVED_TO | Mask.CREATE,
     postpone: bool = False,
     timeout: float = 2,
-) -> None:
+) -> Iterator[Path]:
     """Controllable, timed filesystem watcher"""
 
     # pylint: disable=too-many-locals
 
-    async def fuse_fn(queue: asyncio.Queue[str], timeout: float) -> None:
+    async def fuse_fn(queue: asyncio.Queue, timeout: float) -> None:
         await asyncio.sleep(timeout)
         await queue.put("timeout")
 
-    def task(name: str) -> asyncio.Task[str | Event]:
+    def task(name: str) -> asyncio.Task:
         """Creates a task from a name identifying a data source to read from"""
         return asyncio.create_task(
-            cast(asyncio.Queue[str] | Inotify, {"inotify": inotify, "mqueue": queue}[name]).get(),
+            cast(Union[asyncio.Queue, Inotify], {"inotify": inotify, "mqueue": queue}[name]).get(),
             name=name,
         )
 
     with Inotify() as inotify:
-        inotify.add_watch(path, mask)
+        for path in paths:
+            inotify.add_watch(path, mask)
         fuse = None
         changed_files = set()
         tasks = set(map(task, ("inotify", "mqueue")))
 
         while True:
             done, tasks = await asyncio.wait(
                 fs=tasks,
@@ -112,36 +110,28 @@
                         fuse = None
                     if not fuse:
                         fuse = asyncio.create_task(fuse_fn(queue, timeout))
                 elif event_type == "mqueue":
                     if event_value == "timeout":
                         del fuse
                         fuse = None
-                        callback(changed_files)
+                        for file in changed_files:
+                            yield file
                         changed_files.clear()
 
 
-@watchdog
-async def read_process_output(cmd: str, callback) -> None:
+async def read_process_output(cmd: str) -> None:
     """Run a process asynchronously and handle each line on stdout using provided callback"""
     process = await asyncio.create_subprocess_exec(
         *shlex.split(cmd),
         stdout=asyncio.subprocess.PIPE,
     )
     assert process.stdout
     while True:
         if not (line := (await process.stdout.readline()).decode().strip("\n")):
             break
-        log_exceptions(callback, line)
+        yield line
 
 
 def process_output(cmd: str) -> str:
     """Return command output as one blob"""
     return check_output(shlex.split(cmd), stderr=DEVNULL, text=True)
-
-
-def log_exceptions(callback, *args, **kwargs):
-    """Convenience function, for removing try/except noise"""
-    try:
-        callback(*args, **kwargs)
-    except Exception as exc:  # pylint:disable=broad-except
-        log().exception(exc)
```

### Comparing `docker_shaper-0.1.2/pyproject.toml` & `docker_shaper-0.1.3/pyproject.toml`

 * *Files 16% similar despite different names*

```diff
@@ -1,17 +1,18 @@
 [tool.poetry]
 name = "docker-shaper"
-version = "0.1.2"
+version = "0.1.3"
 description = "Keeps Docker resources in shape based on rules and usage"
 authors = ["Frans Fürst <frans.fuerst@checkmk.com>"]
 repository = "https://github.com/Checkmk/checkmk-dev-tools"
 readme = "Readme.md"
 packages = [
   {include = "docker_shaper/**/*.py"},
-  {include = "docker_shaper/**/*.html"},
+  {include = "docker_shaper/static"},
+  {include = "docker_shaper/templates"},
 ]
 
 [tool.poetry.scripts]
 docker-shaper = 'docker_shaper.cli:main'
 
 [tool.poetry.dependencies]
 python = ">=3.8.1,<4.0.0"
```

### Comparing `docker_shaper-0.1.2/PKG-INFO` & `docker_shaper-0.1.3/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: docker-shaper
-Version: 0.1.2
+Version: 0.1.3
 Summary: Keeps Docker resources in shape based on rules and usage
 Home-page: https://github.com/Checkmk/checkmk-dev-tools
 Author: Frans Fürst
 Author-email: frans.fuerst@checkmk.com
 Requires-Python: >=3.8.1,<4.0.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
@@ -35,23 +35,23 @@
 
 
 ## Development & Contribution
 
 ### Todo
 
 - [x] pip package
-- [x] quart interface
-- [ ] increase/decrease logging
+- [x] Quart interface
+- [ ] bring in dockermon
+- [ ] auto update
 - [ ] bring in dgcd
-- [ ] untag certain tags
-- [ ] outsource config
 - [ ] bring in list_volumes
-- [ ] dockermon
-- [ ] container cleanup
-- [ ] Quart interface
+- [ ] outsource config
+- [ ] 	increase/decrease logging
+- [ ] new: untag certain tags
+- [ ] new: container cleanup
 
 
 ### Setup
 
 ### Prerequisites
 
 * Python 3.8.10
@@ -94,13 +94,14 @@
   - check installed package
   - go through review process
   - publish the new package `poetry publish --build --repository checkmk`
   - commit new version && push
 
 
 ## Knowledge
-
+https://github.com/torfsen/python-systemd-tutorial
+https://www.digitalocean.com/community/tutorials/how-to-use-templates-in-a-flask-application
 * https://blog.miguelgrinberg.com/post/beautiful-interactive-tables-for-your-flask-templates
 * https://stackoverflow.com/questions/49957034/live-updating-dynamic-variable-on-html-with-flask
 * https://pgjones.gitlab.io/quart/how_to_guides/templating.html
```

