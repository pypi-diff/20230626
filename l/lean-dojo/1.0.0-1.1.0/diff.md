# Comparing `tmp/lean_dojo-1.0.0.tar.gz` & `tmp/lean_dojo-1.1.0.tar.gz`

## Comparing `lean_dojo-1.0.0.tar` & `lean_dojo-1.1.0.tar`

### file list

```diff
@@ -1,36 +1,35 @@
--rw-r--r--   0        0        0      874 2020-02-02 00:00:00.000000 lean_dojo-1.0.0/.readthedocs.yaml
--rw-r--r--   0        0        0      125 2020-02-02 00:00:00.000000 lean_dojo-1.0.0/mypy.ini
--rw-r--r--   0        0        0   665100 2020-02-02 00:00:00.000000 lean_dojo-1.0.0/nohup.out
--rw-r--r--   0        0        0      711 2020-02-02 00:00:00.000000 lean_dojo-1.0.0/src/lean_dojo/__init__.py
--rw-r--r--   0        0        0     2178 2020-02-02 00:00:00.000000 lean_dojo-1.0.0/src/lean_dojo/constants.py
--rw-r--r--   0        0        0    11641 2020-02-02 00:00:00.000000 lean_dojo-1.0.0/src/lean_dojo/container.py
--rw-r--r--   0        0        0    11619 2020-02-02 00:00:00.000000 lean_dojo-1.0.0/src/lean_dojo/utils.py
--rw-r--r--   0        0        0    17589 2020-02-02 00:00:00.000000 lean_dojo-1.0.0/src/lean_dojo/data_extraction/0001-Modify-Lean-for-proof-recording.patch
--rw-r--r--   0        0        0    12056 2020-02-02 00:00:00.000000 lean_dojo-1.0.0/src/lean_dojo/data_extraction/ExtractData.lean
--rw-r--r--   0        0        0     5376 2020-02-02 00:00:00.000000 lean_dojo-1.0.0/src/lean_dojo/data_extraction/build_lean3_repo.py
--rw-r--r--   0        0        0     4307 2020-02-02 00:00:00.000000 lean_dojo-1.0.0/src/lean_dojo/data_extraction/build_lean4_repo.py
--rw-r--r--   0        0        0     2663 2020-02-02 00:00:00.000000 lean_dojo-1.0.0/src/lean_dojo/data_extraction/cache.py
--rw-r--r--   0        0        0    17787 2020-02-02 00:00:00.000000 lean_dojo-1.0.0/src/lean_dojo/data_extraction/lean.py
--rw-r--r--   0        0        0     6097 2020-02-02 00:00:00.000000 lean_dojo-1.0.0/src/lean_dojo/data_extraction/trace.py
--rw-r--r--   0        0        0    47696 2020-02-02 00:00:00.000000 lean_dojo-1.0.0/src/lean_dojo/data_extraction/traced_data.py
--rw-r--r--   0        0        0      390 2020-02-02 00:00:00.000000 lean_dojo-1.0.0/src/lean_dojo/data_extraction/ast/lean3/ast_utils.py
--rw-r--r--   0        0        0    12503 2020-02-02 00:00:00.000000 lean_dojo-1.0.0/src/lean_dojo/data_extraction/ast/lean3/expr.py
--rw-r--r--   0        0        0    74077 2020-02-02 00:00:00.000000 lean_dojo-1.0.0/src/lean_dojo/data_extraction/ast/lean3/node.py
--rw-r--r--   0        0        0    26808 2020-02-02 00:00:00.000000 lean_dojo-1.0.0/src/lean_dojo/data_extraction/ast/lean4/node.py
--rw-r--r--   0        0        0     8056 2020-02-02 00:00:00.000000 lean_dojo-1.0.0/src/lean_dojo/interaction/Lean4Repl.lean
--rw-r--r--   0        0        0    17589 2020-02-02 00:00:00.000000 lean_dojo-1.0.0/src/lean_dojo/interaction/dojo.py
--rw-r--r--   0        0        0    20967 2020-02-02 00:00:00.000000 lean_dojo-1.0.0/src/lean_dojo/interaction/lean3_repl.lean
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 lean_dojo-1.0.0/tests/__init__.py
--rw-r--r--   0        0        0     2406 2020-02-02 00:00:00.000000 lean_dojo-1.0.0/tests/conftest.py
--rw-r--r--   0        0        0      390 2020-02-02 00:00:00.000000 lean_dojo-1.0.0/tests/data_extraction/test_trace.py
--rw-r--r--   0        0        0      634 2020-02-02 00:00:00.000000 lean_dojo-1.0.0/tests/interaction/test_env.py
--rw-r--r--   0        0        0    11411 2020-02-02 00:00:00.000000 lean_dojo-1.0.0/tests/interaction/test_examples.py
--rw-r--r--   0        0        0     1632 2020-02-02 00:00:00.000000 lean_dojo-1.0.0/tests/interaction/test_init_errors.py
--rw-r--r--   0        0        0      739 2020-02-02 00:00:00.000000 lean_dojo-1.0.0/tests/interaction/test_sorry.py
--rw-r--r--   0        0        0     1134 2020-02-02 00:00:00.000000 lean_dojo-1.0.0/tests/interaction/test_timeout.py
--rw-r--r--   0        0        0     4457 2020-02-02 00:00:00.000000 lean_dojo-1.0.0/tests/interaction/test_unexpected_errors.py
--rw-r--r--   0        0        0     1821 2020-02-02 00:00:00.000000 lean_dojo-1.0.0/.gitignore
--rw-r--r--   0        0        0     1079 2020-02-02 00:00:00.000000 lean_dojo-1.0.0/LICENSE
--rw-r--r--   0        0        0     3123 2020-02-02 00:00:00.000000 lean_dojo-1.0.0/README.md
--rw-r--r--   0        0        0     1396 2020-02-02 00:00:00.000000 lean_dojo-1.0.0/pyproject.toml
--rw-r--r--   0        0        0     5841 2020-02-02 00:00:00.000000 lean_dojo-1.0.0/PKG-INFO
+-rw-r--r--   0        0        0      874 2020-02-02 00:00:00.000000 lean_dojo-1.1.0/.readthedocs.yaml
+-rw-r--r--   0        0        0      125 2020-02-02 00:00:00.000000 lean_dojo-1.1.0/mypy.ini
+-rw-r--r--   0        0        0      711 2020-02-02 00:00:00.000000 lean_dojo-1.1.0/src/lean_dojo/__init__.py
+-rw-r--r--   0        0        0     2549 2020-02-02 00:00:00.000000 lean_dojo-1.1.0/src/lean_dojo/constants.py
+-rw-r--r--   0        0        0    11641 2020-02-02 00:00:00.000000 lean_dojo-1.1.0/src/lean_dojo/container.py
+-rw-r--r--   0        0        0    11619 2020-02-02 00:00:00.000000 lean_dojo-1.1.0/src/lean_dojo/utils.py
+-rw-r--r--   0        0        0    17589 2020-02-02 00:00:00.000000 lean_dojo-1.1.0/src/lean_dojo/data_extraction/0001-Modify-Lean-for-proof-recording.patch
+-rw-r--r--   0        0        0    12065 2020-02-02 00:00:00.000000 lean_dojo-1.1.0/src/lean_dojo/data_extraction/ExtractData.lean
+-rw-r--r--   0        0        0     5376 2020-02-02 00:00:00.000000 lean_dojo-1.1.0/src/lean_dojo/data_extraction/build_lean3_repo.py
+-rw-r--r--   0        0        0     4699 2020-02-02 00:00:00.000000 lean_dojo-1.1.0/src/lean_dojo/data_extraction/build_lean4_repo.py
+-rw-r--r--   0        0        0     3746 2020-02-02 00:00:00.000000 lean_dojo-1.1.0/src/lean_dojo/data_extraction/cache.py
+-rw-r--r--   0        0        0    17785 2020-02-02 00:00:00.000000 lean_dojo-1.1.0/src/lean_dojo/data_extraction/lean.py
+-rw-r--r--   0        0        0     6185 2020-02-02 00:00:00.000000 lean_dojo-1.1.0/src/lean_dojo/data_extraction/trace.py
+-rw-r--r--   0        0        0    47904 2020-02-02 00:00:00.000000 lean_dojo-1.1.0/src/lean_dojo/data_extraction/traced_data.py
+-rw-r--r--   0        0        0      390 2020-02-02 00:00:00.000000 lean_dojo-1.1.0/src/lean_dojo/data_extraction/ast/lean3/ast_utils.py
+-rw-r--r--   0        0        0    12503 2020-02-02 00:00:00.000000 lean_dojo-1.1.0/src/lean_dojo/data_extraction/ast/lean3/expr.py
+-rw-r--r--   0        0        0    74077 2020-02-02 00:00:00.000000 lean_dojo-1.1.0/src/lean_dojo/data_extraction/ast/lean3/node.py
+-rw-r--r--   0        0        0    26808 2020-02-02 00:00:00.000000 lean_dojo-1.1.0/src/lean_dojo/data_extraction/ast/lean4/node.py
+-rw-r--r--   0        0        0     8056 2020-02-02 00:00:00.000000 lean_dojo-1.1.0/src/lean_dojo/interaction/Lean4Repl.lean
+-rw-r--r--   0        0        0    17727 2020-02-02 00:00:00.000000 lean_dojo-1.1.0/src/lean_dojo/interaction/dojo.py
+-rw-r--r--   0        0        0    20967 2020-02-02 00:00:00.000000 lean_dojo-1.1.0/src/lean_dojo/interaction/lean3_repl.lean
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 lean_dojo-1.1.0/tests/__init__.py
+-rw-r--r--   0        0        0     2490 2020-02-02 00:00:00.000000 lean_dojo-1.1.0/tests/conftest.py
+-rw-r--r--   0        0        0      390 2020-02-02 00:00:00.000000 lean_dojo-1.1.0/tests/data_extraction/test_trace.py
+-rw-r--r--   0        0        0      634 2020-02-02 00:00:00.000000 lean_dojo-1.1.0/tests/interaction/test_env.py
+-rw-r--r--   0        0        0    11463 2020-02-02 00:00:00.000000 lean_dojo-1.1.0/tests/interaction/test_examples.py
+-rw-r--r--   0        0        0     1632 2020-02-02 00:00:00.000000 lean_dojo-1.1.0/tests/interaction/test_init_errors.py
+-rw-r--r--   0        0        0      739 2020-02-02 00:00:00.000000 lean_dojo-1.1.0/tests/interaction/test_sorry.py
+-rw-r--r--   0        0        0      978 2020-02-02 00:00:00.000000 lean_dojo-1.1.0/tests/interaction/test_timeout.py
+-rw-r--r--   0        0        0     4364 2020-02-02 00:00:00.000000 lean_dojo-1.1.0/tests/interaction/test_unexpected_errors.py
+-rw-r--r--   0        0        0     1821 2020-02-02 00:00:00.000000 lean_dojo-1.1.0/.gitignore
+-rw-r--r--   0        0        0     1070 2020-02-02 00:00:00.000000 lean_dojo-1.1.0/LICENSE
+-rw-r--r--   0        0        0     4107 2020-02-02 00:00:00.000000 lean_dojo-1.1.0/README.md
+-rw-r--r--   0        0        0     1418 2020-02-02 00:00:00.000000 lean_dojo-1.1.0/pyproject.toml
+-rw-r--r--   0        0        0     6890 2020-02-02 00:00:00.000000 lean_dojo-1.1.0/PKG-INFO
```

### Comparing `lean_dojo-1.0.0/.readthedocs.yaml` & `lean_dojo-1.1.0/.readthedocs.yaml`

 * *Files identical despite different names*

### Comparing `lean_dojo-1.0.0/src/lean_dojo/__init__.py` & `lean_dojo-1.1.0/src/lean_dojo/__init__.py`

 * *Files identical despite different names*

### Comparing `lean_dojo-1.0.0/src/lean_dojo/constants.py` & `lean_dojo-1.1.0/src/lean_dojo/constants.py`

 * *Files 12% similar despite different names*

```diff
@@ -2,24 +2,31 @@
 Many of them are configurable via :ref:`environment-variables`.
 """
 import os
 import multiprocessing
 from pathlib import Path
 
 
-__version__ = "1.0.0"
+__version__ = "1.1.0"
 
 CACHE_DIR = (
     Path(os.environ["CACHE_DIR"])
     if "CACHE_DIR" in os.environ
     else Path.home() / ".cache/lean_dojo"
 )
 """Cache directory for storing traced repos (see :ref:`caching`).
 """
 
+REMOTE_CACHE_URL = "https://lean-dojo.s3.amazonaws.com"
+"""URL of the remote cache (see :ref:`caching`)."""
+
+DISABLE_REMOTE_CACHE = "DISABLE_REMOTE_CACHE" in os.environ
+"""Whether to disable remote caching (see :ref:`caching`) and build all repos locally.
+"""
+
 TMP_DIR = Path(os.environ["TMP_DIR"]) if "TMP_DIR" in os.environ else None
 """Temporary directory used by LeanDo for storing intermediate files
 """
 
 MAX_NUM_PROCS = 32
 
 NUM_PROCS = int(os.getenv("NUM_PROCS", min(multiprocessing.cpu_count(), MAX_NUM_PROCS)))
@@ -62,13 +69,13 @@
 DOCKER_AVAILABLE = os.system("docker version 1>/dev/null 2>/dev/null") == 0
 
 DOCKER_TAG = "yangky11/lean-dojo"
 
 if CONTAINER == "docker":
     assert (
         DOCKER_AVAILABLE
-    ), "Failed to access Docker. Please make sure Docker is running and you have access."
+    ), "Failed to access Docker. Please make sure Docker is running and you have access. Alternatively, you can try to run without Docker by setting the `CONTAINER` environment variable to `native`."
     os.system(f"docker pull {DOCKER_TAG} 1>/dev/null 2>/dev/null")
 
 MIN_LEAN3_VERSION = "v3.42.1"
 """The minimum version of Lean 3 that LeanDojo supports.
 """
```

### Comparing `lean_dojo-1.0.0/src/lean_dojo/container.py` & `lean_dojo-1.1.0/src/lean_dojo/container.py`

 * *Files identical despite different names*

### Comparing `lean_dojo-1.0.0/src/lean_dojo/utils.py` & `lean_dojo-1.1.0/src/lean_dojo/utils.py`

 * *Files identical despite different names*

### Comparing `lean_dojo-1.0.0/src/lean_dojo/data_extraction/0001-Modify-Lean-for-proof-recording.patch` & `lean_dojo-1.1.0/src/lean_dojo/data_extraction/0001-Modify-Lean-for-proof-recording.patch`

 * *Files identical despite different names*

### Comparing `lean_dojo-1.0.0/src/lean_dojo/data_extraction/ExtractData.lean` & `lean_dojo-1.1.0/src/lean_dojo/data_extraction/ExtractData.lean`

 * *Files 1% similar despite different names*

```diff
@@ -338,15 +338,15 @@
   | [] =>
     let cwd ← IO.currentDir
     println! "Extracting data at {cwd}"
     let _ ← System.FilePath.walkDir cwd fun dir => do
       for p in ← System.FilePath.readDir dir do
         if ← shouldProcess p.path then
           let _ ← IO.asTask $ IO.Process.run
-            (if cwd != "lean4" then
+            (if cwd.fileName != "lean4" then
               {cmd := "lake", args := #["env", "lean", "--run", "ExtractData.lean", p.path.toString]}
             else
               {cmd := "./build/release/stage1/bin/lean", args := #["--run", "ExtractData.lean", p.path.toString]})
           println! p.path
       pure true
   | path :: _ =>
     processFile (← Path.toAbsolute ⟨path⟩)
```

### Comparing `lean_dojo-1.0.0/src/lean_dojo/data_extraction/build_lean3_repo.py` & `lean_dojo-1.1.0/src/lean_dojo/data_extraction/build_lean3_repo.py`

 * *Files 10% similar despite different names*

```diff
@@ -26,26 +26,26 @@
     res = subprocess.run(cmd, shell=True, capture_output=capture_output, check=True)
     if capture_output:
         return res.stdout.decode()
     else:
         return None
 
 
-def record_paths(dir: Path, root: Path, lean_exe: Path) -> None:
+def record_paths(dir: Path, root: Path, lean_bin: Path) -> None:
     """Run ``lean --deps`` for all Lean files in ``dir`` to record its dependencies.
 
     Args:
         dir (Path): The directory containing Lean files.
     """
     dir = Path(dir)
 
     for p in dir.glob("**/*.lean"):
         with p.with_suffix(".dep_paths").open("wt") as oup:
             for line in run_cmd(
-                f"{lean_exe} --deps {p}", capture_output=True
+                f"{lean_bin} --deps {p}", capture_output=True
             ).splitlines():
                 olean_path = PurePath(line.strip())
                 assert olean_path.suffix == ".olean"
                 lean_path = olean_path.relative_to(root).with_suffix(".lean")
                 oup.write(str(lean_path) + "\n")
 
 
@@ -92,16 +92,16 @@
     repo_name = sys.argv[1]
     traced_repo_root = Path.cwd() / repo_name
     if repo_name == "lean":
         modified_lean_root = traced_repo_root
     else:
         modified_lean_root = traced_repo_root / "_target/deps/lean"
     modifed_lean_lib = modified_lean_root / "library"
-    modifed_lean_exe = modified_lean_root / "bin/lean"
-    modified_leanpkg_exe = modified_lean_root / "bin/leanpkg"
+    modifed_lean_bin = modified_lean_root / "bin/lean"
+    modified_leanpkg_bin = modified_lean_root / "bin/leanpkg"
 
     # Build modified Lean without installing it.
     logger.info("Building modifed Lean")
     run_cmd(
         [
             f"mkdir -p {modified_lean_root}/build/release",
             f"cd {modified_lean_root}/build/release",
@@ -115,45 +115,45 @@
     os.chdir(repo_name)
 
     if repo_name == "lean":
         # Use modified Lean to trace it self.
         src_dir = "library"
     else:
         # Build the repo and all its dependencies.
-        modifed_lean_exe = modified_lean_root / "bin/lean"
-        record_paths(modifed_lean_lib, traced_repo_root, modifed_lean_exe)
+        modifed_lean_bin = modified_lean_root / "bin/lean"
+        record_paths(modifed_lean_lib, traced_repo_root, modifed_lean_bin)
         config = toml.load(open("leanpkg.toml"))
         src_dir = config["package"]["path"]
-        run_cmd(f"{modified_leanpkg_exe} configure")
+        run_cmd(f"{modified_leanpkg_bin} configure")
 
         path_file = Path("leanpkg.path")
         lines = [
             line.replace("builtin_path", "path _target/deps/lean/library")
             for line in path_file.open()
         ]
         with open(path_file, "w") as f:
             f.writelines(lines)
 
         for dep in Path("_target/deps").glob("*"):
             if dep.name == "lean":
                 continue
             dep_config = toml.load((dep / "leanpkg.toml").open())
             dep_src_dir = dep / dep_config["package"]["path"]
-            record_paths(dep_src_dir, traced_repo_root, modifed_lean_exe)
+            record_paths(dep_src_dir, traced_repo_root, modifed_lean_bin)
 
     logger.info(f"Tracing {repo_name}")
     remove_files(modifed_lean_lib, ".olean")
-    modified_lean = f"{modifed_lean_exe} --ast --tsast --tspp --recursive --make --threads={num_procs}"
+    modified_lean = f"{modifed_lean_bin} --ast --tsast --tspp --recursive --make --threads={num_procs}"
     io_path = modifed_lean_lib / "system/io.lean"
     run_cmd(f"{modified_lean} {io_path}", capture_output=True)
     launch_progressbar(["_target/deps", src_dir])
     try:
         run_cmd(f"{modified_lean} {src_dir}", capture_output=True)
     except subprocess.CalledProcessError as ex:
         logger.error(ex)
         logger.error("Please check if the repo can be built with `leanpkg build`.")
-    record_paths(src_dir, traced_repo_root, modifed_lean_exe)
+    record_paths(src_dir, traced_repo_root, modifed_lean_bin)
     os.chdir("..")
 
 
 if __name__ == "__main__":
     main()
```

### Comparing `lean_dojo-1.0.0/src/lean_dojo/data_extraction/build_lean4_repo.py` & `lean_dojo-1.1.0/src/lean_dojo/data_extraction/build_lean4_repo.py`

 * *Files 9% similar despite different names*

```diff
@@ -3,14 +3,15 @@
 Only this file runs in Docker. So it must be self-contained.
 """
 import os
 import sys
 import shutil
 import itertools
 import subprocess
+from glob import glob
 from tqdm import tqdm
 from loguru import logger
 from time import sleep, monotonic
 from pathlib import Path, PurePath
 from multiprocessing import Process
 from typing import Union, List, Optional
 
@@ -26,26 +27,26 @@
     res = subprocess.run(cmd, shell=True, capture_output=capture_output, check=True)
     if capture_output:
         return res.stdout.decode()
     else:
         return None
 
 
-def record_paths(dir: Path, root: Path, lean_exe: Path) -> None:
+def record_paths(dir: Path, root: Path, lean_bin: Path) -> None:
     """Run ``lean --deps`` for all Lean files in ``dir`` to record its dependencies.
 
     Args:
         dir (Path): The directory containing Lean files.
     """
     dir = Path(dir)
 
     for p in dir.glob("**/*.lean"):
         with p.with_suffix(".dep_paths").open("wt") as oup:
             for line in run_cmd(
-                f"{lean_exe} --deps {p}", capture_output=True
+                f"{lean_bin} --deps {p}", capture_output=True
             ).splitlines():
                 olean_path = PurePath(line.strip())
                 assert olean_path.suffix == ".olean"
                 lean_path = olean_path.relative_to(root).with_suffix(".lean")
                 oup.write(str(lean_path) + "\n")
 
 
@@ -100,16 +101,17 @@
         run_cmd(
             [
                 f"mkdir -p build/release",
                 f"cd build/release",
                 "cmake ../..",
                 f"make -j{num_procs}",
                 "cd ../..",
-                "rm build/release/stage1/src/lean && rm build/release/stage0/src/lean",
-                "cp -r build/release/stage1/lib lib",
+                "rm build/release/stage1/src/lean",  # Remove symbolic link.
+                "rm build/release/stage0/src/lean",  # Remove symbolic link.
+                "mkdir lib && cp -r build/release/stage1/lib/lean lib/lean",
                 "mv src src_tmp && mkdir src && mv src_tmp src/lean",
             ]
         )
 
         logger.info(f"Tracing {repo_name}")
         launch_progressbar(["lib"])
         run_cmd(
@@ -129,10 +131,15 @@
         logger.info(f"Tracing {repo_name}")
         launch_progressbar(["build"])
         run_cmd(
             f"lake env lean --threads {num_procs} --run ExtractData.lean",
             capture_output=True,
         )
 
+        num_json = len(glob("build/ir/**/*.ast.json", recursive=True))
+        num_dep = len(glob("build/ir/**/*.dep_paths", recursive=True))
+        num_c = len(glob("build/ir/**/*.c", recursive=True))
+        assert num_json == num_dep == num_c, f"{num_json} {num_dep} {num_c}"
+
 
 if __name__ == "__main__":
     main()
```

### Comparing `lean_dojo-1.0.0/src/lean_dojo/data_extraction/cache.py` & `lean_dojo-1.1.0/src/lean_dojo/data_extraction/cache.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,22 +1,25 @@
 """Cache manager of traced repos.
 """
 import os
 import shutil
+import tarfile
 from pathlib import Path
+from loguru import logger
 from filelock import FileLock
-from typing import Optional, Tuple
 from dataclasses import dataclass, field
+from typing import Optional, Tuple, Generator
 
 from ..utils import (
     execute,
+    url_exists,
     get_repo_info,
     report_critical_failure,
 )
-from ..constants import CACHE_DIR
+from ..constants import CACHE_DIR, DISABLE_REMOTE_CACHE, REMOTE_CACHE_URL
 
 
 def _split_git_url(url: str) -> Tuple[str, str]:
     """Split a Git URL into user name and repo name."""
     if url.endswith("/"):
         url = url[:-1]
         assert not url.endswith("/"), f"Unexpected URL: {url}"
@@ -37,46 +40,68 @@
 @dataclass(frozen=True, eq=False)
 class Cache:
     """Cache manager."""
 
     cache_dir: Path
     lock: FileLock = field(init=False, repr=False)
 
+    def __iter__(self) -> Generator[Path, None, None]:
+        """Iterate over all traced repos in the cache."""
+        yield from self.cache_dir.glob("*")
+
     def __post_init__(self):
         if not os.path.exists(self.cache_dir):
             self.cache_dir.mkdir()
         lock_path = self.cache_dir.with_suffix(".lock")
         object.__setattr__(self, "lock", FileLock(lock_path))
 
     def get(self, url: str, commit: str) -> Optional[Path]:
         """Get the path of a traced repo with URL ``url`` and commit hash ``commit``. Return None if no such repo can be found."""
         _, repo_name = _split_git_url(url)
-        dirpath = self._format_dirpath(url, commit) / repo_name
+        dirname = _format_dirname(url, commit)
+        dirpath = self.cache_dir / dirname
+
         with self.lock:
             if dirpath.exists():
-                return dirpath
+                assert (dirpath / repo_name).exists()
+                return dirpath / repo_name
+
+            elif not DISABLE_REMOTE_CACHE:
+                url = os.path.join(REMOTE_CACHE_URL, f"{dirname}.tar.gz")
+                if not url_exists(url):
+                    return None
+                logger.info(
+                    f"Downloading the traced repo from the remote cache. Set the environment variable `DISABLE_REMOTE_CACHE` if you want to trace the repo locally."
+                )
+                execute(f"wget {url} -O {dirpath}.tar.gz")
+
+                with report_critical_failure(_CACHE_CORRPUTION_MSG):
+                    with tarfile.open(f"{dirpath}.tar.gz") as tar:
+                        tar.extractall(self.cache_dir)
+                    os.remove(f"{dirpath}.tar.gz")
+                    execute(f"chmod -R a-w {dirpath}")
+                    assert (dirpath / repo_name).exists()
+
+                return dirpath / repo_name
+
             else:
                 return None
 
     def store(self, src: Path) -> Path:
         """Store a traced repo at path ``src``. Return its path in the cache."""
         dirs = list(src.glob("*"))
         assert len(dirs) == 1, f"Unexpected number of directories in {src}"
         url, commit = get_repo_info(dirs[0])
-        dirpath = self._format_dirpath(url, commit)
+        dirpath = self.cache_dir / _format_dirname(url, commit)
         if not dirpath.exists():
             with self.lock:
                 with report_critical_failure(_CACHE_CORRPUTION_MSG):
                     shutil.copytree(src, dirpath)
                     # Prevent the cache from being modified accidentally.
                     execute(f"chmod -R a-w {dirpath}")
         _, repo_name = _split_git_url(url)
         return dirpath / repo_name
 
-    def _format_dirpath(self, url: str, commit: str) -> Path:
-        dirname = _format_dirname(url, commit)
-        return self.cache_dir / dirname
-
 
 cache = Cache(CACHE_DIR)
 """A global :class:`Cache` object managing LeanDojo's caching of traced repos (see :ref:`caching`).
 """
```

### Comparing `lean_dojo-1.0.0/src/lean_dojo/data_extraction/lean.py` & `lean_dojo-1.1.0/src/lean_dojo/data_extraction/lean.py`

 * *Files 0% similar despite different names*

```diff
@@ -352,15 +352,15 @@
         if self.is_lean4:
             return True
         config_url = self._get_config_url("lean-toolchain")
         return url_exists(config_url)
 
     @property
     def commit_url(self) -> str:
-        return os.path.join(self.url, f"commit/{self.commit}")
+        return os.path.join(self.url, f"tree/{self.commit}")
 
     def show(self) -> None:
         """Show the repo in the default browser."""
         webbrowser.open(self.commit_url)
 
     def exists(self) -> bool:
         return url_exists(self.commit_url)
```

### Comparing `lean_dojo-1.0.0/src/lean_dojo/data_extraction/trace.py` & `lean_dojo-1.1.0/src/lean_dojo/data_extraction/trace.py`

 * *Files 2% similar despite different names*

```diff
@@ -108,15 +108,15 @@
         {"NUM_PROCS": NUM_PROCS},
         as_current_user=True,
         work_dir="/workspace",
     )
 
 
 def is_available_in_cache(repo: LeanGitRepo) -> bool:
-    """Check if ``repo`` has a traced repo available in the cache."""
+    """Check if ``repo`` has a traced repo available in the cache (including the remote cache)."""
     return cache.get(repo.url, repo.commit) is not None
 
 
 def get_traced_repo_path(repo: LeanGitRepo) -> Path:
     """Return the path of a traced repo in the cache.
 
     The function will trace a repo if it is not available in the cache. See :ref:`caching` for details.
@@ -125,14 +125,15 @@
         repo (LeanGitRepo): The Lean repo to trace.
 
     Returns:
         Path: The path of the traced repo in the cache, e.g. :file:`/home/kaiyu/.cache/lean_dojo/leanprover-community-mathlib-2196ab363eb097c008d4497125e0dde23fb36db2`
     """
     path = cache.get(repo.url, repo.commit)
     if path is None:
+        logger.info(f"Tracing {repo}")
         with working_directory() as tmp_dir:
             logger.debug(f"Working in the temporary directory {tmp_dir}")
             _trace(repo)
             traced_repo = TracedRepo.from_traced_files(tmp_dir / repo.name)
             traced_repo.save_to_disk()
             path = cache.store(tmp_dir)
     else:
@@ -156,15 +157,15 @@
     if dst_dir is not None:
         dst_dir = Path(dst_dir)
         assert (
             not dst_dir.exists()
         ), f"The destination directory {dst_dir} already exists."
 
     cached_path = get_traced_repo_path(repo)
-    logger.info("Loading the traced repo")
+    logger.info(f"Loading the traced repo from {cached_path}")
     traced_repo = TracedRepo.load_from_disk(cached_path)
     traced_repo.check_sanity()
 
     if dst_dir is not None:
         dst_dir.mkdir(parents=True)
         shutil.copytree(cached_path, dst_dir / cached_path.name)
         execute(f"chmod -R a+w {dst_dir}")
```

### Comparing `lean_dojo-1.0.0/src/lean_dojo/data_extraction/traced_data.py` & `lean_dojo-1.1.0/src/lean_dojo/data_extraction/traced_data.py`

 * *Files 1% similar despite different names*

```diff
@@ -587,14 +587,16 @@
             root_dir (Union[str, Path]): Root directory of the traced repo.
             json_path (Path): Path of the :file:`*.ast.json` file relative to ``root_dir``.
         """
         root_dir = Path(root_dir)
         root_dir = root_dir.resolve()
         if not json_path.is_absolute():
             json_path = root_dir / json_path
+        if not json_path.exists():
+            raise FileNotFoundError(f"{json_path} does not exist")
         assert json_path.suffixes == [
             ".ast",
             ".json",
         ], f"{json_path} is not a *.ast.json file"
 
         if repo.uses_lean3:
             return cls._from_lean3_traced_file(root_dir, json_path)
@@ -1121,14 +1123,18 @@
         return self.repo.uses_lean3
 
     @property
     def uses_lean4(self) -> bool:
         """Whether the repo uses Lean 4."""
         return self.repo.uses_lean4
 
+    def show(self) -> None:
+        """Show the repo in the default browser."""
+        self.repo.show()
+
     def check_sanity(self) -> None:
         """Perform some basic sanity checks.
 
         The function raises exceptions in case of unsuccessful checks.
         """
         assert isinstance(self.repo, LeanGitRepo)
         assert isinstance(self.dependencies, dict)
```

### Comparing `lean_dojo-1.0.0/src/lean_dojo/data_extraction/ast/lean3/expr.py` & `lean_dojo-1.1.0/src/lean_dojo/data_extraction/ast/lean3/expr.py`

 * *Files identical despite different names*

### Comparing `lean_dojo-1.0.0/src/lean_dojo/data_extraction/ast/lean3/node.py` & `lean_dojo-1.1.0/src/lean_dojo/data_extraction/ast/lean3/node.py`

 * *Files identical despite different names*

### Comparing `lean_dojo-1.0.0/src/lean_dojo/data_extraction/ast/lean4/node.py` & `lean_dojo-1.1.0/src/lean_dojo/data_extraction/ast/lean4/node.py`

 * *Files identical despite different names*

### Comparing `lean_dojo-1.0.0/src/lean_dojo/interaction/Lean4Repl.lean` & `lean_dojo-1.1.0/src/lean_dojo/interaction/Lean4Repl.lean`

 * *Files identical despite different names*

### Comparing `lean_dojo-1.0.0/src/lean_dojo/interaction/dojo.py` & `lean_dojo-1.1.0/src/lean_dojo/interaction/dojo.py`

 * *Files 2% similar despite different names*

```diff
@@ -198,17 +198,16 @@
 
         try:
             self.old_sigint = signal.signal(signal.SIGINT, self._exit_gracefully)
             self.old_sigterm = signal.signal(signal.SIGTERM, self._exit_gracefully)
             os.chdir(self.tmp_dir)
 
             repo = self.theorem.repo
-
-            if repo.name == "lean4":
-                raise DojoInitError("The Lean 4 repo itself is not supported yet.")
+            if repo.is_lean4:
+                raise NotImplementedError("InteractingLean 4 is not supported yet.")
             traced_repo_path = get_traced_repo_path(repo)
 
             # Copy and `cd` into the repo.
             shutil.copytree(
                 traced_repo_path,
                 repo.name,
                 ignore=ignore_patterns("*.dep_paths", "*.ast.json", "*.trace.xml"),
@@ -233,25 +232,27 @@
             if repo.uses_lean3:
                 if repo.is_lean:
                     path = Path("library/system/io.lean")
                 else:
                     path = LEAN3_DEPS_DIR / "lean/library/system/io.lean"
             else:
                 if repo.is_lean:
-                    path = Path("src/Lean/Elab/Tactic.lean")
+                    path = Path("src/lean/Lean/Elab/Tactic.lean")
                 else:
                     path = LEAN4_DEPS_DIR / "lean4/src/lean/Lean/Elab/Tactic.lean"
             deps = [path] + _get_all_dependencies(traced_repo_path, path, repo)
 
             # Run the modified proof in a container.
             self.container = get_container()
             logger.debug(f"Launching the proof using {type(self.container)}")
             mts = [Mount(Path.cwd(), f"/workspace/{repo.name}")]
             if repo.uses_lean3:
                 cmd = f"lean {self.theorem.file_path}"
+            elif repo.is_lean4:
+                cmd = f"./build/release/stage1/bin/lean {self.theorem.file_path}"
             else:
                 self.container.run(
                     f"lake build Lean4Repl",
                     mts,
                     as_current_user=True,
                     capture_output=True,
                     work_dir=f"/workspace/{repo.name}",
@@ -312,15 +313,15 @@
         if self.hard_timeout is not None:
             signal.alarm(0)
             signal.signal(signal.SIGALRM, signal.SIG_DFL)
 
         if not self.is_proved:
             logger.debug(f"Failed to prove {self.theorem}")
 
-        if not self.is_crashed:
+        if not self.is_crashed and not self.has_timedout:
             if self.uses_lean4:
                 req = "exit"
             else:
                 req = json.dumps(["exit_repl", []])
             try:
                 self._submit_request(req)
             except Exception:
```

### Comparing `lean_dojo-1.0.0/src/lean_dojo/interaction/lean3_repl.lean` & `lean_dojo-1.1.0/src/lean_dojo/interaction/lean3_repl.lean`

 * *Files identical despite different names*

### Comparing `lean_dojo-1.0.0/tests/conftest.py` & `lean_dojo-1.1.0/tests/conftest.py`

 * *Files 8% similar despite different names*

```diff
@@ -6,25 +6,27 @@
 
 
 LEAN3_URL = "https://github.com/leanprover-community/lean"
 MATHLIB_URL = "https://github.com/leanprover-community/mathlib"
 MINIF2F_URL = "https://github.com/facebookresearch/miniF2F"
 LEAN_LIQUID_URL = "https://github.com/leanprover-community/lean-liquid"
 PROOFNET_URL = "https://github.com/zhangir-azerbayev/ProofNet"
+LEAN_EXAMPLE_URL = "https://github.com/yangky11/lean-example"
 LEAN4_URL = "https://github.com/leanprover/lean4"
 STD4_URL = "https://github.com/leanprover/std4"
 AESOP_URL = "https://github.com/JLimperg/aesop"
 MATHLIB4_URL = "https://github.com/leanprover-community/mathlib4"
 LEAN4_EXAMPLE_URL = "https://github.com/yangky11/lean4-example"
 URLS = [
     LEAN3_URL,
     MINIF2F_URL,
     MATHLIB_URL,
     LEAN_LIQUID_URL,
     PROOFNET_URL,
+    LEAN_EXAMPLE_URL,
     LEAN4_URL,
     STD4_URL,
     AESOP_URL,
     MATHLIB4_URL,
     LEAN4_EXAMPLE_URL,
 ]
 
@@ -57,15 +59,15 @@
 def std4_repo():
     commit = "ccbe74d4406be21b91c04d62b4c93dec9adfc546"
     return LeanGitRepo(STD4_URL, commit)
 
 
 @pytest.fixture(scope="session")
 def mathlib_repo():
-    commit = "bd9851ca476957ea4549eb19b40e7b5ade9428cc"
+    commit = "8c1b484d6a214e059531e22f1be9898ed6c1fd47"
     return LeanGitRepo(MATHLIB_URL, commit)
 
 
 @pytest.fixture(scope="session")
 def mathlib4_repo():
     commit = "5a919533f110b7d76410134a237ee374f24eaaad"
     return LeanGitRepo(MATHLIB4_URL, commit)
```

### Comparing `lean_dojo-1.0.0/tests/interaction/test_env.py` & `lean_dojo-1.1.0/tests/interaction/test_env.py`

 * *Files identical despite different names*

### Comparing `lean_dojo-1.0.0/tests/interaction/test_examples.py` & `lean_dojo-1.1.0/tests/interaction/test_examples.py`

 * *Files 1% similar despite different names*

```diff
@@ -45,15 +45,15 @@
             s2,
             "· suffices x ^ 2 ^ d.succ - y ^ 2 ^ d.succ = (x ^ 2 ^ d + y ^ 2 ^ d) * (x ^ 2 ^ d - y ^ 2 ^ d) by rw [this, hd, Finset.prod_range_succ, ← mul_assoc, mul_comm (x ^ 2 ^ d + y ^ 2 ^ d)]",
         )
         assert not isinstance(s3, ProofFinished)
         assert not dojo.is_proved
 
 
-@pytest.mark.skip()
+@pytest.mark.skip(reason="The lean4 repo itself is not supported yet.")
 def test_example_4(lean4_repo: LeanGitRepo) -> None:
     thm = Theorem(
         lean4_repo,
         "src/Init/Data/Nat/Gcd.lean",
         "Nat.gcd_self",
     )
     with Dojo(thm) as (dojo, s0):
```

### Comparing `lean_dojo-1.0.0/tests/interaction/test_init_errors.py` & `lean_dojo-1.1.0/tests/interaction/test_init_errors.py`

 * *Files identical despite different names*

### Comparing `lean_dojo-1.0.0/tests/interaction/test_sorry.py` & `lean_dojo-1.1.0/tests/interaction/test_sorry.py`

 * *Files identical despite different names*

### Comparing `lean_dojo-1.0.0/tests/interaction/test_unexpected_errors.py` & `lean_dojo-1.1.0/tests/interaction/test_unexpected_errors.py`

 * *Files 2% similar despite different names*

```diff
@@ -30,21 +30,21 @@
         assert isinstance(res, TacticError)
         assert not dojo.is_proved
 
 
 def test_parse_tactic_failure_1(mathlib_repo: LeanGitRepo) -> None:
     thm = Theorem(
         mathlib_repo,
-        "src/linear_algebra/dimension.lean",
-        "basis.nonempty_fintype_index_of_dim_lt_aleph_0",
+        "src/set_theory/ordinal/arithmetic.lean",
+        "ordinal.le_sup_shrink_equiv",
     )
     with Dojo(thm) as (dojo, init_state):
         res = dojo.run_tac(
             init_state,
-            "{ rwa [← cardinal.lift_lt, ← b.mk_eq_dim, cardinal.lift_aleph_0, ← cardinal.lift_aleph_0.{u_1 v}, cardinal.lift_lt, cardinal.lt_aleph_0_iff_fintype] at h }",
+            "{ convert le_sup.{u u} _ ((@equiv_shrink s hs) ⟨a, ha⟩), rw symm_apply_apply }",
         )
         assert isinstance(res, TacticError)
         assert not dojo.is_proved
 
 
 def test_proof_check_failure_1(mathlib_repo: LeanGitRepo) -> None:
     thm = Theorem(
```

### Comparing `lean_dojo-1.0.0/.gitignore` & `lean_dojo-1.1.0/.gitignore`

 * *Files identical despite different names*

### Comparing `lean_dojo-1.0.0/LICENSE` & `lean_dojo-1.1.0/LICENSE`

 * *Files 23% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 MIT License
 
-Copyright (c) 2023 Anima AI + Science Lab
+Copyright (c) 2023 LeanDojo Team
 
 Permission is hereby granted, free of charge, to any person obtaining a copy
 of this software and associated documentation files (the "Software"), to deal
 in the Software without restriction, including without limitation the rights
 to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
 copies of the Software, and to permit persons to whom the Software is
 furnished to do so, subject to the following conditions:
```

### Comparing `lean_dojo-1.0.0/pyproject.toml` & `lean_dojo-1.1.0/pyproject.toml`

 * *Files 8% similar despite different names*

```diff
@@ -9,15 +9,15 @@
   "/docs",
   "/images",
   "/scripts",
 ]
 
 [project]
 name = "lean-dojo"
-version = "1.0.0"
+version = "1.1.0"
 authors = [
   { name="Kaiyu Yang", email="kaiyuy@caltech.edu" },
 ]
 description = "LeanDojo: Machine Learning for Theorem Proving in Lean"
 keywords = ["theorem proving", "machine learning", "Lean"]
 readme = "README.md"
 license = { file = "LICENSE" }
@@ -38,15 +38,16 @@
   "lxml",
   "ray[default] >= 1.5",
 ]
 
 [project.optional-dependencies]
 dev = [
   "ipython",
-  "notebook"
+  "notebook",
+  "hatch"
 ]
 test = [
   "pytest",
 ]
 docs = [
   "sphinx",
   "sphinx-rtd-theme",
@@ -54,14 +55,15 @@
 lint = [
   "mypy",
   "black[jupyter]",
 ]
 all = [
   "ipython",
   "notebook",
+  "hatch",
   "pytest",
   "sphinx",
   "sphinx-rtd-theme",
   "mypy",
   "black[jupyter]",
 ]
```

### Comparing `lean_dojo-1.0.0/PKG-INFO` & `lean_dojo-1.1.0/PKG-INFO`

 * *Files 24% similar despite different names*

```diff
@@ -1,17 +1,17 @@
 Metadata-Version: 2.1
 Name: lean-dojo
-Version: 1.0.0
+Version: 1.1.0
 Summary: LeanDojo: Machine Learning for Theorem Proving in Lean
 Project-URL: Homepage, https://leandojo.org/
 Project-URL: Bug Tracker, https://github.com/lean-dojo/LeanDojo/issues
 Author-email: Kaiyu Yang <kaiyuy@caltech.edu>
 License: MIT License
         
-        Copyright (c) 2023 Anima AI + Science Lab
+        Copyright (c) 2023 LeanDojo Team
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
         of this software and associated documentation files (the "Software"), to deal
         in the Software without restriction, including without limitation the rights
         to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
         copies of the Software, and to permit persons to whom the Software is
         furnished to do so, subject to the following conditions:
@@ -39,21 +39,23 @@
 Requires-Dist: networkx
 Requires-Dist: ray[default]>=1.5
 Requires-Dist: toml
 Requires-Dist: tqdm
 Requires-Dist: types-toml
 Provides-Extra: all
 Requires-Dist: black[jupyter]; extra == 'all'
+Requires-Dist: hatch; extra == 'all'
 Requires-Dist: ipython; extra == 'all'
 Requires-Dist: mypy; extra == 'all'
 Requires-Dist: notebook; extra == 'all'
 Requires-Dist: pytest; extra == 'all'
 Requires-Dist: sphinx; extra == 'all'
 Requires-Dist: sphinx-rtd-theme; extra == 'all'
 Provides-Extra: dev
+Requires-Dist: hatch; extra == 'dev'
 Requires-Dist: ipython; extra == 'dev'
 Requires-Dist: notebook; extra == 'dev'
 Provides-Extra: docs
 Requires-Dist: sphinx; extra == 'docs'
 Requires-Dist: sphinx-rtd-theme; extra == 'docs'
 Provides-Extra: lint
 Requires-Dist: black[jupyter]; extra == 'lint'
@@ -61,65 +63,75 @@
 Provides-Extra: test
 Requires-Dist: pytest; extra == 'test'
 Description-Content-Type: text/markdown
 
 LeanDojo: Machine Learning for Theorem Proving in Lean
 ======================================================
 
-![Model](images/LeanDojo.jpg)
+![LeanDojo](https://github.com/lean-dojo/LeanDojo/blob/main/images/LeanDojo.jpg)
 
 [LeanDojo](https://leandojo.org/) is a Python library for learning–based theorem provers in Lean, supporting both [Lean 3](https://github.com/leanprover-community/lean) and [Lean 4](https://leanprover.github.io/). It provides two main features:
 
 * Extracting data (proof states, tactics, premises, etc.) from Lean repos.
 * Interacting with Lean programmatically.
 
 
-[![Documentation Status](https://readthedocs.org/projects/leandojo/badge/?version=latest)](https://leandojo.readthedocs.io/en/latest/?badge=latest) [![Code style: black](https://img.shields.io/badge/code%20style-black-000000.svg)](https://github.com/psf/black)
+[![Documentation Status](https://readthedocs.org/projects/leandojo/badge/?version=latest)](https://leandojo.readthedocs.io/en/latest/?badge=latest) [![PyPI](https://img.shields.io/pypi/v/lean-dojo)](https://pypi.org/project/lean-dojo/) [![GitHub license](https://img.shields.io/github/license/MineDojo/MineDojo)](https://github.com/MineDojo/MineDojo/blob/main/LICENSE) [![Code style: black](https://img.shields.io/badge/code%20style-black-000000.svg)](https://github.com/psf/black) 
 
+______________________________________________________________________
 
 ## Requirements
 
 * Linux or macOS
 * Git >= 2.25
 * Python >= 3.9
 * Docker strongly recommended
 
 
 ## Installation
 
-LeanDojo is available on [PyPI]() and can be installed via pip:
+LeanDojo is available on [PyPI](https://pypi.org/project/lean-dojo/) and can be installed via pip:
 ```bash
 pip install lean-dojo
 ```
 
-It can also be installed locally from this Git repo:
+It can also be installed locally from the Git repo:
 ```bash
 pip install .
 ```
 
 
 ## Documentation
 
-[LeanDojo's documentation]((https://leandojo.readthedocs.io/en/latest/index.html)) is available on Read the Docs.
+* [Getting Started](https://leandojo.readthedocs.io/en/latest/getting-started.html)
+* [Demo](https://github.com/lean-dojo/LeanDojo/blob/main/scripts/demo.ipynb)
+* [Full documentation](https://leandojo.readthedocs.io/en/latest/index.html)
 
 
+## Questions and Bugs
+
+* For general questions and discussions, please use [GitHub Discussions](https://github.com/lean-dojo/LeanDojo/discussions).  
+* To report a potential bug, please open an issue.
+
 
 ## Related Links
 
 * [LeanDojo Website](https://leandojo.org/): The official website of LeanDojo.
-* [LeanDojo Benchmark](https://zenodo.org/record/8016386): The dataset used in our paper, consisting of 96,962 theorems and proofs extracted from [mathlib](https://github.com/leanprover-community/mathlib/commits/8c1b484d6a214e059531e22f1be9898ed6c1fd47) by [generate-benchmark-lean3.ipynb](./scripts/generate-benchmark-lean3.ipynb).
-* [LeanDojo Benchmark 4](https://zenodo.org/record/8040110): The Lean 4 version of LeanDojo Benchmark, consisting of 91,766 theorems and proofs extracted from [mathlib4](https://github.com/leanprover-community/mathlib4/commit/5a919533f110b7d76410134a237ee374f24eaaad) by [generate-benchmark-lean4.ipynb](./scripts/generate-benchmark-lean4.ipynb).
+* [LeanDojo Benchmark](https://zenodo.org/record/8016386) [![DOI](https://zenodo.org/badge/DOI/10.5281/zenodo.8016386.svg)](https://doi.org/10.5281/zenodo.8016386): The dataset used in our paper, consisting of 96,962 theorems and proofs extracted from [mathlib](https://github.com/leanprover-community/mathlib/commits/8c1b484d6a214e059531e22f1be9898ed6c1fd47) by [generate-benchmark-lean3.ipynb](./scripts/generate-benchmark-lean3.ipynb). 
+* [LeanDojo Benchmark 4](https://zenodo.org/record/8040110) [![DOI](https://zenodo.org/badge/DOI/10.5281/zenodo.8040110.svg)](https://doi.org/10.5281/zenodo.8040110)
+: The Lean 4 version of LeanDojo Benchmark, consisting of 91,766 theorems and proofs extracted from [mathlib4](https://github.com/leanprover-community/mathlib4/commit/5a919533f110b7d76410134a237ee374f24eaaad) by [generate-benchmark-lean4.ipynb](./scripts/generate-benchmark-lean4.ipynb).
 * [ReProver](https://github.com/lean-dojo/ReProver): The ReProver (Retrieval-Augmented Prover) model in our paper.
+* [LeanDojo ChatGPT Plugin](https://github.com/lean-dojo/LeanDojoChatGPT)
 
 
 ## Citation
 
 [LeanDojo: Theorem Proving with Retrieval-Augmented Language Models](https://arxiv.org/abs/xxxx.xxxxx)      
-Under review, NeuIPS (Datasets and Benchmarks Track), 2023  
-[Kaiyu Yang](https://yangky11.github.io/), [Aidan Swope](https://aidanswope.com/about), [Alex Gu](https://minimario.github.io/), [Rahul Chalamala](https://www.linkedin.com/in/rchalamala),  
+Under review, NeurIPS (Datasets and Benchmarks Track), 2023  
+[Kaiyu Yang](https://yangky11.github.io/), [Aidan Swope](https://aidanswope.com/about), [Alex Gu](https://minimario.github.io/), [Rahul Chalamala](https://rchalamala.github.io/),  
 [Peiyang Song](https://www.linkedin.com/in/peiyang-song-3279b3251/), [Shixing Yu](https://billysx.github.io/), [Saad Godil](https://www.linkedin.com/in/saad-godil-9728353/), [Ryan Prenger](https://www.linkedin.com/in/ryan-prenger-18797ba1/), [Anima Anandkumar](http://tensorlab.cms.caltech.edu/users/anima/)
 
 ```bibtex
 @article{yang2023leandojo,
   title={{LeanDojo}: Theorem Proving with Retrieval-Augmented Language Models},
   author={Yang, Kaiyu and Swope, Aidan and Gu, Alex and Chalamala, Rahul and Song, Peiyang and Yu, Shixing and Godil, Saad and Prenger, Ryan and Anandkumar, Anima},
   journal={arXiv preprint arXiv:xxxx.xxxxx},
```

