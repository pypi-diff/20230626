# Comparing `tmp/autosbatch-0.2.2.tar.gz` & `tmp/autosbatch-0.2.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "autosbatch-0.2.2.tar", max compression
+gzip compressed data, was "autosbatch-0.2.3.tar", max compression
```

## Comparing `autosbatch-0.2.2.tar` & `autosbatch-0.2.3.tar`

### file list

```diff
@@ -1,13 +1,13 @@
--rw-r--r--   0        0        0     1070 2023-03-01 08:51:40.713825 autosbatch-0.2.2/LICENSE
--rw-r--r--   0        0        0     2030 2023-03-01 08:51:40.713825 autosbatch-0.2.2/README.md
--rw-r--r--   0        0        0      393 2023-03-01 08:51:40.713825 autosbatch-0.2.2/autosbatch/__init__.py
--rw-r--r--   0        0        0    14609 2023-03-01 08:51:40.713825 autosbatch-0.2.2/autosbatch/autosbatch.py
--rw-r--r--   0        0        0     3535 2023-03-01 08:51:40.713825 autosbatch-0.2.2/autosbatch/cli.py
--rw-r--r--   0        0        0     1745 2023-03-01 08:51:40.713825 autosbatch-0.2.2/autosbatch/template/CPU_MPI.j2
--rw-r--r--   0        0        0      516 2023-03-01 08:51:40.713825 autosbatch-0.2.2/autosbatch/template/CPU_OpenMP.j2
--rw-r--r--   0        0        0     2995 2023-03-01 08:51:40.717826 autosbatch-0.2.2/pyproject.toml
--rw-r--r--   0        0        0       40 2023-03-01 08:51:40.717826 autosbatch-0.2.2/tests/__init__.py
--rw-r--r--   0        0        0     1675 2023-03-01 08:51:40.717826 autosbatch-0.2.2/tests/test_autosbatch.py
--rw-r--r--   0        0        0     1079 2023-03-01 08:51:40.717826 autosbatch-0.2.2/tests/test_cli.py
--rw-r--r--   0        0        0      188 2023-03-01 08:51:40.717826 autosbatch-0.2.2/tests/test_logger.py
--rw-r--r--   0        0        0     4396 1970-01-01 00:00:00.000000 autosbatch-0.2.2/PKG-INFO
+-rw-r--r--   0        0        0     1070 2023-06-26 12:24:58.195585 autosbatch-0.2.3/LICENSE
+-rw-r--r--   0        0        0     2030 2023-06-26 12:24:58.195585 autosbatch-0.2.3/README.md
+-rw-r--r--   0        0        0      393 2023-06-26 12:24:58.195585 autosbatch-0.2.3/autosbatch/__init__.py
+-rw-r--r--   0        0        0    14761 2023-06-26 12:24:58.195585 autosbatch-0.2.3/autosbatch/autosbatch.py
+-rw-r--r--   0        0        0     3535 2023-06-26 12:24:58.195585 autosbatch-0.2.3/autosbatch/cli.py
+-rw-r--r--   0        0        0     1745 2023-06-26 12:24:58.195585 autosbatch-0.2.3/autosbatch/template/CPU_MPI.j2
+-rw-r--r--   0        0        0      516 2023-06-26 12:24:58.195585 autosbatch-0.2.3/autosbatch/template/CPU_OpenMP.j2
+-rw-r--r--   0        0        0     2995 2023-06-26 12:24:58.199585 autosbatch-0.2.3/pyproject.toml
+-rw-r--r--   0        0        0       40 2023-06-26 12:24:58.199585 autosbatch-0.2.3/tests/__init__.py
+-rw-r--r--   0        0        0     1675 2023-06-26 12:24:58.199585 autosbatch-0.2.3/tests/test_autosbatch.py
+-rw-r--r--   0        0        0     1079 2023-06-26 12:24:58.199585 autosbatch-0.2.3/tests/test_cli.py
+-rw-r--r--   0        0        0      188 2023-06-26 12:24:58.199585 autosbatch-0.2.3/tests/test_logger.py
+-rw-r--r--   0        0        0     4248 1970-01-01 00:00:00.000000 autosbatch-0.2.3/PKG-INFO
```

### Comparing `autosbatch-0.2.2/LICENSE` & `autosbatch-0.2.3/LICENSE`

 * *Files identical despite different names*

### Comparing `autosbatch-0.2.2/README.md` & `autosbatch-0.2.3/README.md`

 * *Files identical despite different names*

### Comparing `autosbatch-0.2.2/autosbatch/autosbatch.py` & `autosbatch-0.2.3/autosbatch/autosbatch.py`

 * *Files 2% similar despite different names*

```diff
@@ -89,23 +89,26 @@
         result = run(command, stdout=PIPE, stderr=PIPE, universal_newlines=True)
         nodes = {}
         for line in result.stdout.splitlines():
             line = line.strip('\"')
             if line.startswith('HOSTNAMES'):
                 continue
             node, free_mem, memory, avail, cpus, free_cpus, load, partition, state = line.split()
+            free_mem = int(free_mem) if free_mem != 'N/A' else 0
+            memory = int(memory) if memory != 'N/A' else 0
+            load = float(load) if load != 'N/A' else 0
             nodes[node] = {
-                'free_mem': int(free_mem),
-                'used_mem': int(memory) - int(free_mem),
-                'memory': int(memory),
+                'free_mem': free_mem,
+                'used_mem': memory - free_mem,
+                'memory': memory,
                 'AVAIL': avail,
                 'cpus': int(cpus),
                 'used_cpus': int(free_cpus.split('/')[0]),
                 'free_cpus': int(free_cpus.split('/')[1]),
-                'load': float(load),
+                'load': load,
                 'partition': partition,
                 'state': state,
             }
         if sortByload:
             nodes = dict(
                 OrderedDict(sorted(nodes.items(), key=lambda x: (x[1]['load'], x[1]['used_mem'], x[1]['used_cpus'])))
             )
```

### Comparing `autosbatch-0.2.2/autosbatch/cli.py` & `autosbatch-0.2.3/autosbatch/cli.py`

 * *Files identical despite different names*

### Comparing `autosbatch-0.2.2/autosbatch/template/CPU_MPI.j2` & `autosbatch-0.2.3/autosbatch/template/CPU_MPI.j2`

 * *Files identical despite different names*

### Comparing `autosbatch-0.2.2/autosbatch/template/CPU_OpenMP.j2` & `autosbatch-0.2.3/autosbatch/template/CPU_OpenMP.j2`

 * *Files identical despite different names*

### Comparing `autosbatch-0.2.2/pyproject.toml` & `autosbatch-0.2.3/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 [tool]
 [tool.poetry]
 name = "autosbatch"
-version = "0.2.2"
+version = "0.2.3"
 homepage = "https://github.com/Jianhua-Wang/autosbatch"
 description = "submit hundreds of jobs to slurm automatically."
 authors = ["Jianhua Wang <jianhua.mert@gmail.com>"]
 readme = "README.md"
 license = "MIT"
 classifiers = [
     'Development Status :: 2 - Pre-Alpha',
```

### Comparing `autosbatch-0.2.2/tests/test_autosbatch.py` & `autosbatch-0.2.3/tests/test_autosbatch.py`

 * *Files identical despite different names*

### Comparing `autosbatch-0.2.2/tests/test_cli.py` & `autosbatch-0.2.3/tests/test_cli.py`

 * *Files identical despite different names*

### Comparing `autosbatch-0.2.2/PKG-INFO` & `autosbatch-0.2.3/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: autosbatch
-Version: 0.2.2
+Version: 0.2.3
 Summary: submit hundreds of jobs to slurm automatically.
 Home-page: https://github.com/Jianhua-Wang/autosbatch
 License: MIT
 Author: Jianhua Wang
 Author-email: jianhua.mert@gmail.com
 Requires-Python: >=3.8,<3.12
 Classifier: Development Status :: 2 - Pre-Alpha
@@ -12,18 +12,15 @@
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Natural Language :: English
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
-Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.7
-Classifier: Programming Language :: Python :: 3.8
-Classifier: Programming Language :: Python :: 3.9
 Provides-Extra: dev
 Provides-Extra: doc
 Provides-Extra: test
 Requires-Dist: black (>=22.3.0) ; extra == "test"
 Requires-Dist: bump2version (>=1.0.1,<2.0.0) ; extra == "dev"
 Requires-Dist: flake8 (>=3.9.2,<4.0.0) ; extra == "test"
 Requires-Dist: flake8-docstrings (>=1.6.0,<2.0.0) ; extra == "test"
```

