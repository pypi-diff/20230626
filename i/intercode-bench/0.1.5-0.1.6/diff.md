# Comparing `tmp/intercode-bench-0.1.5.tar.gz` & `tmp/intercode-bench-0.1.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "intercode-bench-0.1.5.tar", last modified: Sun Jun 25 03:45:13 2023, max compression
+gzip compressed data, was "intercode-bench-0.1.6.tar", last modified: Mon Jun 26 14:46:45 2023, max compression
```

## Comparing `intercode-bench-0.1.5.tar` & `intercode-bench-0.1.6.tar`

### file list

```diff
@@ -1,37 +1,37 @@
-drwxr-xr-x   0 johnbyang   (502) staff       (20)        0 2023-06-25 03:45:13.204807 intercode-bench-0.1.5/
--rw-r--r--   0 johnbyang   (502) staff       (20)     1093 2023-06-23 00:41:05.000000 intercode-bench-0.1.5/LICENSE
--rw-r--r--   0 johnbyang   (502) staff       (20)     3057 2023-06-25 03:45:13.205498 intercode-bench-0.1.5/PKG-INFO
--rw-r--r--   0 johnbyang   (502) staff       (20)     2059 2023-06-25 03:44:01.000000 intercode-bench-0.1.5/README.md
--rw-r--r--   0 johnbyang   (502) staff       (20)       84 2023-06-23 00:11:41.000000 intercode-bench-0.1.5/pyproject.toml
--rw-r--r--   0 johnbyang   (502) staff       (20)      112 2023-06-25 03:45:13.206958 intercode-bench-0.1.5/setup.cfg
--rw-r--r--   0 johnbyang   (502) staff       (20)     1451 2023-06-23 21:38:26.000000 intercode-bench-0.1.5/setup.py
-drwxr-xr-x   0 johnbyang   (502) staff       (20)        0 2023-06-25 03:45:13.173379 intercode-bench-0.1.5/src/
-drwxr-xr-x   0 johnbyang   (502) staff       (20)        0 2023-06-25 03:45:13.178092 intercode-bench-0.1.5/src/intercode/
--rw-r--r--   0 johnbyang   (502) staff       (20)      137 2023-06-25 03:44:58.000000 intercode-bench-0.1.5/src/intercode/__init__.py
-drwxr-xr-x   0 johnbyang   (502) staff       (20)        0 2023-06-25 03:45:13.180093 intercode-bench-0.1.5/src/intercode/envs/
--rw-r--r--   0 johnbyang   (502) staff       (20)      141 2023-06-23 21:20:36.000000 intercode-bench-0.1.5/src/intercode/envs/__init__.py
-drwxr-xr-x   0 johnbyang   (502) staff       (20)        0 2023-06-25 03:45:13.181725 intercode-bench-0.1.5/src/intercode/envs/bash/
--rw-r--r--   0 johnbyang   (502) staff       (20)        0 2023-06-23 02:52:42.000000 intercode-bench-0.1.5/src/intercode/envs/bash/__init__.py
--rw-r--r--   0 johnbyang   (502) staff       (20)     7682 2023-06-23 02:47:20.000000 intercode-bench-0.1.5/src/intercode/envs/bash/bash_env.py
-drwxr-xr-x   0 johnbyang   (502) staff       (20)        0 2023-06-25 03:45:13.183559 intercode-bench-0.1.5/src/intercode/envs/game/
--rw-r--r--   0 johnbyang   (502) staff       (20)        0 2023-06-23 02:52:55.000000 intercode-bench-0.1.5/src/intercode/envs/game/__init__.py
--rw-r--r--   0 johnbyang   (502) staff       (20)     4552 2023-06-23 02:47:20.000000 intercode-bench-0.1.5/src/intercode/envs/game/ctf_env.py
--rw-r--r--   0 johnbyang   (502) staff       (20)     8569 2023-06-23 02:47:20.000000 intercode-bench-0.1.5/src/intercode/envs/ic_env.py
-drwxr-xr-x   0 johnbyang   (502) staff       (20)        0 2023-06-25 03:45:13.185282 intercode-bench-0.1.5/src/intercode/envs/sql/
--rw-r--r--   0 johnbyang   (502) staff       (20)        0 2023-06-23 02:52:45.000000 intercode-bench-0.1.5/src/intercode/envs/sql/__init__.py
--rw-r--r--   0 johnbyang   (502) staff       (20)     5045 2023-06-23 04:27:43.000000 intercode-bench-0.1.5/src/intercode/envs/sql/sql_env.py
-drwxr-xr-x   0 johnbyang   (502) staff       (20)        0 2023-06-25 03:45:13.189279 intercode-bench-0.1.5/src/intercode/utils/
--rw-r--r--   0 johnbyang   (502) staff       (20)      148 2023-06-23 00:31:02.000000 intercode-bench-0.1.5/src/intercode/utils/__init__.py
--rw-r--r--   0 johnbyang   (502) staff       (20)     2428 2023-06-23 00:31:02.000000 intercode-bench-0.1.5/src/intercode/utils/data_loader.py
--rw-r--r--   0 johnbyang   (502) staff       (20)     1718 2023-06-23 00:31:02.000000 intercode-bench-0.1.5/src/intercode/utils/utils.py
-drwxr-xr-x   0 johnbyang   (502) staff       (20)        0 2023-06-25 03:45:13.194956 intercode-bench-0.1.5/src/intercode_bench.egg-info/
--rw-r--r--   0 johnbyang   (502) staff       (20)     3057 2023-06-25 03:45:13.000000 intercode-bench-0.1.5/src/intercode_bench.egg-info/PKG-INFO
--rw-r--r--   0 johnbyang   (502) staff       (20)      751 2023-06-25 03:45:13.000000 intercode-bench-0.1.5/src/intercode_bench.egg-info/SOURCES.txt
--rw-r--r--   0 johnbyang   (502) staff       (20)        1 2023-06-25 03:45:13.000000 intercode-bench-0.1.5/src/intercode_bench.egg-info/dependency_links.txt
--rw-r--r--   0 johnbyang   (502) staff       (20)       72 2023-06-25 03:45:13.000000 intercode-bench-0.1.5/src/intercode_bench.egg-info/requires.txt
--rw-r--r--   0 johnbyang   (502) staff       (20)       10 2023-06-25 03:45:13.000000 intercode-bench-0.1.5/src/intercode_bench.egg-info/top_level.txt
-drwxr-xr-x   0 johnbyang   (502) staff       (20)        0 2023-06-25 03:45:13.203723 intercode-bench-0.1.5/tests/
--rw-r--r--   0 johnbyang   (502) staff       (20)     1757 2023-06-23 02:47:20.000000 intercode-bench-0.1.5/tests/test_data_loader.py
--rw-r--r--   0 johnbyang   (502) staff       (20)     2498 2023-06-23 02:47:20.000000 intercode-bench-0.1.5/tests/test_env_bash.py
--rw-r--r--   0 johnbyang   (502) staff       (20)     1334 2023-06-23 02:47:20.000000 intercode-bench-0.1.5/tests/test_env_ic.py
--rw-r--r--   0 johnbyang   (502) staff       (20)     1683 2023-06-23 02:47:20.000000 intercode-bench-0.1.5/tests/test_env_sql.py
+drwxr-xr-x   0 johnbyang   (502) staff       (20)        0 2023-06-26 14:46:45.592644 intercode-bench-0.1.6/
+-rw-r--r--   0 johnbyang   (502) staff       (20)     1093 2023-06-23 00:41:05.000000 intercode-bench-0.1.6/LICENSE
+-rw-r--r--   0 johnbyang   (502) staff       (20)     3071 2023-06-26 14:46:45.592834 intercode-bench-0.1.6/PKG-INFO
+-rw-r--r--   0 johnbyang   (502) staff       (20)     2073 2023-06-26 14:45:26.000000 intercode-bench-0.1.6/README.md
+-rw-r--r--   0 johnbyang   (502) staff       (20)       84 2023-06-23 00:11:41.000000 intercode-bench-0.1.6/pyproject.toml
+-rw-r--r--   0 johnbyang   (502) staff       (20)      112 2023-06-26 14:46:45.593695 intercode-bench-0.1.6/setup.cfg
+-rw-r--r--   0 johnbyang   (502) staff       (20)     1451 2023-06-23 21:38:26.000000 intercode-bench-0.1.6/setup.py
+drwxr-xr-x   0 johnbyang   (502) staff       (20)        0 2023-06-26 14:46:45.573613 intercode-bench-0.1.6/src/
+drwxr-xr-x   0 johnbyang   (502) staff       (20)        0 2023-06-26 14:46:45.577816 intercode-bench-0.1.6/src/intercode/
+-rw-r--r--   0 johnbyang   (502) staff       (20)      137 2023-06-26 14:44:17.000000 intercode-bench-0.1.6/src/intercode/__init__.py
+drwxr-xr-x   0 johnbyang   (502) staff       (20)        0 2023-06-26 14:46:45.579116 intercode-bench-0.1.6/src/intercode/envs/
+-rw-r--r--   0 johnbyang   (502) staff       (20)      141 2023-06-23 21:20:36.000000 intercode-bench-0.1.6/src/intercode/envs/__init__.py
+drwxr-xr-x   0 johnbyang   (502) staff       (20)        0 2023-06-26 14:46:45.580330 intercode-bench-0.1.6/src/intercode/envs/bash/
+-rw-r--r--   0 johnbyang   (502) staff       (20)        0 2023-06-23 02:52:42.000000 intercode-bench-0.1.6/src/intercode/envs/bash/__init__.py
+-rw-r--r--   0 johnbyang   (502) staff       (20)     7682 2023-06-23 02:47:20.000000 intercode-bench-0.1.6/src/intercode/envs/bash/bash_env.py
+drwxr-xr-x   0 johnbyang   (502) staff       (20)        0 2023-06-26 14:46:45.581606 intercode-bench-0.1.6/src/intercode/envs/game/
+-rw-r--r--   0 johnbyang   (502) staff       (20)        0 2023-06-23 02:52:55.000000 intercode-bench-0.1.6/src/intercode/envs/game/__init__.py
+-rw-r--r--   0 johnbyang   (502) staff       (20)     4552 2023-06-23 02:47:20.000000 intercode-bench-0.1.6/src/intercode/envs/game/ctf_env.py
+-rw-r--r--   0 johnbyang   (502) staff       (20)     8569 2023-06-23 02:47:20.000000 intercode-bench-0.1.6/src/intercode/envs/ic_env.py
+drwxr-xr-x   0 johnbyang   (502) staff       (20)        0 2023-06-26 14:46:45.582961 intercode-bench-0.1.6/src/intercode/envs/sql/
+-rw-r--r--   0 johnbyang   (502) staff       (20)        0 2023-06-23 02:52:45.000000 intercode-bench-0.1.6/src/intercode/envs/sql/__init__.py
+-rw-r--r--   0 johnbyang   (502) staff       (20)     5045 2023-06-23 04:27:43.000000 intercode-bench-0.1.6/src/intercode/envs/sql/sql_env.py
+drwxr-xr-x   0 johnbyang   (502) staff       (20)        0 2023-06-26 14:46:45.585237 intercode-bench-0.1.6/src/intercode/utils/
+-rw-r--r--   0 johnbyang   (502) staff       (20)      148 2023-06-23 00:31:02.000000 intercode-bench-0.1.6/src/intercode/utils/__init__.py
+-rw-r--r--   0 johnbyang   (502) staff       (20)     2428 2023-06-23 00:31:02.000000 intercode-bench-0.1.6/src/intercode/utils/data_loader.py
+-rw-r--r--   0 johnbyang   (502) staff       (20)     1718 2023-06-23 00:31:02.000000 intercode-bench-0.1.6/src/intercode/utils/utils.py
+drwxr-xr-x   0 johnbyang   (502) staff       (20)        0 2023-06-26 14:46:45.588972 intercode-bench-0.1.6/src/intercode_bench.egg-info/
+-rw-r--r--   0 johnbyang   (502) staff       (20)     3071 2023-06-26 14:46:45.000000 intercode-bench-0.1.6/src/intercode_bench.egg-info/PKG-INFO
+-rw-r--r--   0 johnbyang   (502) staff       (20)      751 2023-06-26 14:46:45.000000 intercode-bench-0.1.6/src/intercode_bench.egg-info/SOURCES.txt
+-rw-r--r--   0 johnbyang   (502) staff       (20)        1 2023-06-26 14:46:45.000000 intercode-bench-0.1.6/src/intercode_bench.egg-info/dependency_links.txt
+-rw-r--r--   0 johnbyang   (502) staff       (20)       72 2023-06-26 14:46:45.000000 intercode-bench-0.1.6/src/intercode_bench.egg-info/requires.txt
+-rw-r--r--   0 johnbyang   (502) staff       (20)       10 2023-06-26 14:46:45.000000 intercode-bench-0.1.6/src/intercode_bench.egg-info/top_level.txt
+drwxr-xr-x   0 johnbyang   (502) staff       (20)        0 2023-06-26 14:46:45.592106 intercode-bench-0.1.6/tests/
+-rw-r--r--   0 johnbyang   (502) staff       (20)     1757 2023-06-23 02:47:20.000000 intercode-bench-0.1.6/tests/test_data_loader.py
+-rw-r--r--   0 johnbyang   (502) staff       (20)     2498 2023-06-23 02:47:20.000000 intercode-bench-0.1.6/tests/test_env_bash.py
+-rw-r--r--   0 johnbyang   (502) staff       (20)     1334 2023-06-23 02:47:20.000000 intercode-bench-0.1.6/tests/test_env_ic.py
+-rw-r--r--   0 johnbyang   (502) staff       (20)     1683 2023-06-23 02:47:20.000000 intercode-bench-0.1.6/tests/test_env_sql.py
```

### Comparing `intercode-bench-0.1.5/LICENSE` & `intercode-bench-0.1.6/LICENSE`

 * *Files identical despite different names*

### Comparing `intercode-bench-0.1.5/PKG-INFO` & `intercode-bench-0.1.6/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: intercode-bench
-Version: 0.1.5
+Version: 0.1.6
 Summary: The official InterCode benchmark package - a framework for interactive code tasks
 Home-page: http://github.com/intercode-benchmark/intercode-benchmark
 Author: John Yang
 Author-email: byjohnyang@gmail.com
 Project-URL: Documentation, https://github.com/intercode-benchmark/intercode-benchmark
 Project-URL: Bug Reports, https://github.com/intercode-benchmark/intercode-benchmark/issues
 Project-URL: Source Code, https://github.com/intercode-benchmark/intercode-benchmark
@@ -39,22 +39,22 @@
 
 For an overview of InterCode, building interactive code tasks with InterCode, and evaluating agents on InterCode environments, please check out our [wiki](TO DO) and the original paper:
 
 **[InterCode: Standardizing and Benchmarking Interactive Coding with Execution Feedback](https://intercode-benchmark.github.io/)**  
 
 ## 🛠️ Installation
 > **Note**
-> InterCode requires a local `docker` installation to run. Learn more [here](https://docs.docker.com/get-docker/) to install.
+> InterCode requires `python` >= 3.8 a local `docker` installation to run. Learn more [here](https://docs.docker.com/get-docker/) to install.
 
 ```
 pip install intercode-bench
 ```
 
 ## 🚀 Quick Start
-* Clone the [InterCode starter repository](https://github.com/intercode-benchmark/starter-files)
+* Clone the [InterCode repository](https://github.com/intercode-benchmark/intercode-benchmark)
 * Run `./setup.sh`
 * Run `python run_sql.py` 
 
 If InterCode was installed successfully, the InterCode SQL environment should be started successfully and a CLI interpreter should appear, allowing you to enter `SQL` commands
 to interact with the task setting.
 
 ## 🔎 Learn More
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: intercode-bench Version: 0.1.5 Summary: The
+Metadata-Version: 2.1 Name: intercode-bench Version: 0.1.6 Summary: The
 official InterCode benchmark package - a framework for interactive code tasks
 Home-page: http://github.com/intercode-benchmark/intercode-benchmark Author:
 John Yang Author-email: byjohnyang@gmail.com Project-URL: Documentation, https:
 //github.com/intercode-benchmark/intercode-benchmark Project-URL: Bug Reports,
 https://github.com/intercode-benchmark/intercode-benchmark/issues Project-URL:
 Source Code, https://github.com/intercode-benchmark/intercode-benchmark
 Project-URL: Website, https://intercode-benchmark.github.io/ Keywords:
@@ -19,18 +19,18 @@
 [`gym`](https://gymnasium.farama.org/) interface definition, InterCode makes it
 easy to quickly define a code environment and deploy an agent to operate in
 code within the context of the environment. For an overview of InterCode,
 building interactive code tasks with InterCode, and evaluating agents on
 InterCode environments, please check out our [wiki](TO DO) and the original
 paper: **[InterCode: Standardizing and Benchmarking Interactive Coding with
 Execution Feedback](https://intercode-benchmark.github.io/)** ## ð ï¸
-Installation > **Note** > InterCode requires a local `docker` installation to
-run. Learn more [here](https://docs.docker.com/get-docker/) to install. ``` pip
-install intercode-bench ``` ## ð Quick Start * Clone the [InterCode starter
-repository](https://github.com/intercode-benchmark/starter-files) * Run `./
-setup.sh` * Run `python run_sql.py` If InterCode was installed successfully,
-the InterCode SQL environment should be started successfully and a CLI
-interpreter should appear, allowing you to enter `SQL` commands to interact
-with the task setting. ## ð Learn More To learn more about the InterCode
-framework, please check out the [website](https://intercode-
-benchmark.github.io/) and GitHub [repository](https://github.com/intercode-
-benchmark/intercode-benchmark) ## ðªª License Check `LICENSE.md`
+Installation > **Note** > InterCode requires `python` >= 3.8 a local `docker`
+installation to run. Learn more [here](https://docs.docker.com/get-docker/) to
+install. ``` pip install intercode-bench ``` ## ð Quick Start * Clone the
+[InterCode repository](https://github.com/intercode-benchmark/intercode-
+benchmark) * Run `./setup.sh` * Run `python run_sql.py` If InterCode was
+installed successfully, the InterCode SQL environment should be started
+successfully and a CLI interpreter should appear, allowing you to enter `SQL`
+commands to interact with the task setting. ## ð Learn More To learn more
+about the InterCode framework, please check out the [website](https://
+intercode-benchmark.github.io/) and GitHub [repository](https://github.com/
+intercode-benchmark/intercode-benchmark) ## ðªª License Check `LICENSE.md`
```

### Comparing `intercode-bench-0.1.5/README.md` & `intercode-bench-0.1.6/README.md`

 * *Files 9% similar despite different names*

```diff
@@ -18,22 +18,22 @@
 
 For an overview of InterCode, building interactive code tasks with InterCode, and evaluating agents on InterCode environments, please check out our [wiki](TO DO) and the original paper:
 
 **[InterCode: Standardizing and Benchmarking Interactive Coding with Execution Feedback](https://intercode-benchmark.github.io/)**  
 
 ## 🛠️ Installation
 > **Note**
-> InterCode requires a local `docker` installation to run. Learn more [here](https://docs.docker.com/get-docker/) to install.
+> InterCode requires `python` >= 3.8 a local `docker` installation to run. Learn more [here](https://docs.docker.com/get-docker/) to install.
 
 ```
 pip install intercode-bench
 ```
 
 ## 🚀 Quick Start
-* Clone the [InterCode starter repository](https://github.com/intercode-benchmark/starter-files)
+* Clone the [InterCode repository](https://github.com/intercode-benchmark/intercode-benchmark)
 * Run `./setup.sh`
 * Run `python run_sql.py` 
 
 If InterCode was installed successfully, the InterCode SQL environment should be started successfully and a CLI interpreter should appear, allowing you to enter `SQL` commands
 to interact with the task setting.
 
 ## 🔎 Learn More
```

#### html2text {}

```diff
@@ -6,18 +6,18 @@
 [`gym`](https://gymnasium.farama.org/) interface definition, InterCode makes it
 easy to quickly define a code environment and deploy an agent to operate in
 code within the context of the environment. For an overview of InterCode,
 building interactive code tasks with InterCode, and evaluating agents on
 InterCode environments, please check out our [wiki](TO DO) and the original
 paper: **[InterCode: Standardizing and Benchmarking Interactive Coding with
 Execution Feedback](https://intercode-benchmark.github.io/)** ## ð ï¸
-Installation > **Note** > InterCode requires a local `docker` installation to
-run. Learn more [here](https://docs.docker.com/get-docker/) to install. ``` pip
-install intercode-bench ``` ## ð Quick Start * Clone the [InterCode starter
-repository](https://github.com/intercode-benchmark/starter-files) * Run `./
-setup.sh` * Run `python run_sql.py` If InterCode was installed successfully,
-the InterCode SQL environment should be started successfully and a CLI
-interpreter should appear, allowing you to enter `SQL` commands to interact
-with the task setting. ## ð Learn More To learn more about the InterCode
-framework, please check out the [website](https://intercode-
-benchmark.github.io/) and GitHub [repository](https://github.com/intercode-
-benchmark/intercode-benchmark) ## ðªª License Check `LICENSE.md`
+Installation > **Note** > InterCode requires `python` >= 3.8 a local `docker`
+installation to run. Learn more [here](https://docs.docker.com/get-docker/) to
+install. ``` pip install intercode-bench ``` ## ð Quick Start * Clone the
+[InterCode repository](https://github.com/intercode-benchmark/intercode-
+benchmark) * Run `./setup.sh` * Run `python run_sql.py` If InterCode was
+installed successfully, the InterCode SQL environment should be started
+successfully and a CLI interpreter should appear, allowing you to enter `SQL`
+commands to interact with the task setting. ## ð Learn More To learn more
+about the InterCode framework, please check out the [website](https://
+intercode-benchmark.github.io/) and GitHub [repository](https://github.com/
+intercode-benchmark/intercode-benchmark) ## ðªª License Check `LICENSE.md`
```

### Comparing `intercode-bench-0.1.5/setup.py` & `intercode-bench-0.1.6/setup.py`

 * *Files identical despite different names*

### Comparing `intercode-bench-0.1.5/src/intercode/envs/bash/bash_env.py` & `intercode-bench-0.1.6/src/intercode/envs/bash/bash_env.py`

 * *Files identical despite different names*

### Comparing `intercode-bench-0.1.5/src/intercode/envs/game/ctf_env.py` & `intercode-bench-0.1.6/src/intercode/envs/game/ctf_env.py`

 * *Files identical despite different names*

### Comparing `intercode-bench-0.1.5/src/intercode/envs/ic_env.py` & `intercode-bench-0.1.6/src/intercode/envs/ic_env.py`

 * *Files identical despite different names*

### Comparing `intercode-bench-0.1.5/src/intercode/envs/sql/sql_env.py` & `intercode-bench-0.1.6/src/intercode/envs/sql/sql_env.py`

 * *Files identical despite different names*

### Comparing `intercode-bench-0.1.5/src/intercode/utils/data_loader.py` & `intercode-bench-0.1.6/src/intercode/utils/data_loader.py`

 * *Files identical despite different names*

### Comparing `intercode-bench-0.1.5/src/intercode/utils/utils.py` & `intercode-bench-0.1.6/src/intercode/utils/utils.py`

 * *Files identical despite different names*

### Comparing `intercode-bench-0.1.5/src/intercode_bench.egg-info/PKG-INFO` & `intercode-bench-0.1.6/src/intercode_bench.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: intercode-bench
-Version: 0.1.5
+Version: 0.1.6
 Summary: The official InterCode benchmark package - a framework for interactive code tasks
 Home-page: http://github.com/intercode-benchmark/intercode-benchmark
 Author: John Yang
 Author-email: byjohnyang@gmail.com
 Project-URL: Documentation, https://github.com/intercode-benchmark/intercode-benchmark
 Project-URL: Bug Reports, https://github.com/intercode-benchmark/intercode-benchmark/issues
 Project-URL: Source Code, https://github.com/intercode-benchmark/intercode-benchmark
@@ -39,22 +39,22 @@
 
 For an overview of InterCode, building interactive code tasks with InterCode, and evaluating agents on InterCode environments, please check out our [wiki](TO DO) and the original paper:
 
 **[InterCode: Standardizing and Benchmarking Interactive Coding with Execution Feedback](https://intercode-benchmark.github.io/)**  
 
 ## 🛠️ Installation
 > **Note**
-> InterCode requires a local `docker` installation to run. Learn more [here](https://docs.docker.com/get-docker/) to install.
+> InterCode requires `python` >= 3.8 a local `docker` installation to run. Learn more [here](https://docs.docker.com/get-docker/) to install.
 
 ```
 pip install intercode-bench
 ```
 
 ## 🚀 Quick Start
-* Clone the [InterCode starter repository](https://github.com/intercode-benchmark/starter-files)
+* Clone the [InterCode repository](https://github.com/intercode-benchmark/intercode-benchmark)
 * Run `./setup.sh`
 * Run `python run_sql.py` 
 
 If InterCode was installed successfully, the InterCode SQL environment should be started successfully and a CLI interpreter should appear, allowing you to enter `SQL` commands
 to interact with the task setting.
 
 ## 🔎 Learn More
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: intercode-bench Version: 0.1.5 Summary: The
+Metadata-Version: 2.1 Name: intercode-bench Version: 0.1.6 Summary: The
 official InterCode benchmark package - a framework for interactive code tasks
 Home-page: http://github.com/intercode-benchmark/intercode-benchmark Author:
 John Yang Author-email: byjohnyang@gmail.com Project-URL: Documentation, https:
 //github.com/intercode-benchmark/intercode-benchmark Project-URL: Bug Reports,
 https://github.com/intercode-benchmark/intercode-benchmark/issues Project-URL:
 Source Code, https://github.com/intercode-benchmark/intercode-benchmark
 Project-URL: Website, https://intercode-benchmark.github.io/ Keywords:
@@ -19,18 +19,18 @@
 [`gym`](https://gymnasium.farama.org/) interface definition, InterCode makes it
 easy to quickly define a code environment and deploy an agent to operate in
 code within the context of the environment. For an overview of InterCode,
 building interactive code tasks with InterCode, and evaluating agents on
 InterCode environments, please check out our [wiki](TO DO) and the original
 paper: **[InterCode: Standardizing and Benchmarking Interactive Coding with
 Execution Feedback](https://intercode-benchmark.github.io/)** ## ð ï¸
-Installation > **Note** > InterCode requires a local `docker` installation to
-run. Learn more [here](https://docs.docker.com/get-docker/) to install. ``` pip
-install intercode-bench ``` ## ð Quick Start * Clone the [InterCode starter
-repository](https://github.com/intercode-benchmark/starter-files) * Run `./
-setup.sh` * Run `python run_sql.py` If InterCode was installed successfully,
-the InterCode SQL environment should be started successfully and a CLI
-interpreter should appear, allowing you to enter `SQL` commands to interact
-with the task setting. ## ð Learn More To learn more about the InterCode
-framework, please check out the [website](https://intercode-
-benchmark.github.io/) and GitHub [repository](https://github.com/intercode-
-benchmark/intercode-benchmark) ## ðªª License Check `LICENSE.md`
+Installation > **Note** > InterCode requires `python` >= 3.8 a local `docker`
+installation to run. Learn more [here](https://docs.docker.com/get-docker/) to
+install. ``` pip install intercode-bench ``` ## ð Quick Start * Clone the
+[InterCode repository](https://github.com/intercode-benchmark/intercode-
+benchmark) * Run `./setup.sh` * Run `python run_sql.py` If InterCode was
+installed successfully, the InterCode SQL environment should be started
+successfully and a CLI interpreter should appear, allowing you to enter `SQL`
+commands to interact with the task setting. ## ð Learn More To learn more
+about the InterCode framework, please check out the [website](https://
+intercode-benchmark.github.io/) and GitHub [repository](https://github.com/
+intercode-benchmark/intercode-benchmark) ## ðªª License Check `LICENSE.md`
```

### Comparing `intercode-bench-0.1.5/src/intercode_bench.egg-info/SOURCES.txt` & `intercode-bench-0.1.6/src/intercode_bench.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `intercode-bench-0.1.5/tests/test_data_loader.py` & `intercode-bench-0.1.6/tests/test_data_loader.py`

 * *Files identical despite different names*

### Comparing `intercode-bench-0.1.5/tests/test_env_bash.py` & `intercode-bench-0.1.6/tests/test_env_bash.py`

 * *Files identical despite different names*

### Comparing `intercode-bench-0.1.5/tests/test_env_ic.py` & `intercode-bench-0.1.6/tests/test_env_ic.py`

 * *Files identical despite different names*

### Comparing `intercode-bench-0.1.5/tests/test_env_sql.py` & `intercode-bench-0.1.6/tests/test_env_sql.py`

 * *Files identical despite different names*

