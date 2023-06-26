# Comparing `tmp/llm-chain-0.0.1.tar.gz` & `tmp/llm-chain-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "llm-chain-0.0.1.tar", last modified: Fri Jun  9 17:18:18 2023, max compression
+gzip compressed data, was "llm-chain-0.0.2.tar", last modified: Mon Jun 26 21:19:21 2023, max compression
```

## Comparing `llm-chain-0.0.1.tar` & `llm-chain-0.0.2.tar`

### file list

```diff
@@ -1,17 +1,33 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-09 17:18:18.763452 llm-chain-0.0.1/
--rw-r--r--   0 root         (0) root         (0)     1072 2023-02-25 17:02:25.000000 llm-chain-0.0.1/LICENSE
--rw-r--r--   0 root         (0) root         (0)     2071 2023-06-09 17:18:18.763933 llm-chain-0.0.1/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     1544 2023-06-09 16:09:22.000000 llm-chain-0.0.1/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-09 17:18:18.730970 llm-chain-0.0.1/llm_chain/
--rw-r--r--   0 root         (0) root         (0)       52 2023-06-09 17:08:19.000000 llm-chain-0.0.1/llm_chain/__init__.py
--rw-r--r--   0 root         (0) root         (0)     1097 2023-06-09 17:01:12.000000 llm-chain-0.0.1/llm_chain/utilities.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-09 17:18:18.756604 llm-chain-0.0.1/llm_chain.egg-info/
--rw-r--r--   0 root         (0) root         (0)     2071 2023-06-09 17:18:18.000000 llm-chain-0.0.1/llm_chain.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      275 2023-06-09 17:18:18.000000 llm-chain-0.0.1/llm_chain.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-06-09 17:18:18.000000 llm-chain-0.0.1/llm_chain.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)        9 2023-06-09 17:18:18.000000 llm-chain-0.0.1/llm_chain.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       10 2023-06-09 17:18:18.000000 llm-chain-0.0.1/llm_chain.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)      104 2023-02-25 17:02:25.000000 llm-chain-0.0.1/pyproject.toml
--rw-r--r--   0 root         (0) root         (0)      638 2023-06-09 17:18:18.765476 llm-chain-0.0.1/setup.cfg
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-09 17:18:18.761546 llm-chain-0.0.1/tests/
--rw-r--r--   0 root         (0) root         (0)      427 2023-06-09 17:14:56.000000 llm-chain-0.0.1/tests/test_utilities.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-26 21:19:21.561850 llm-chain-0.0.2/
+-rw-r--r--   0 root         (0) root         (0)     1072 2023-02-25 17:02:25.000000 llm-chain-0.0.2/LICENSE
+-rw-r--r--   0 root         (0) root         (0)     7647 2023-06-26 21:19:21.562898 llm-chain-0.0.2/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     7119 2023-06-26 21:13:57.000000 llm-chain-0.0.2/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-26 21:19:21.504820 llm-chain-0.0.2/llm_chain/
+-rw-r--r--   0 root         (0) root         (0)       52 2023-06-09 17:08:19.000000 llm-chain-0.0.2/llm_chain/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    13569 2023-06-26 17:26:17.000000 llm-chain-0.0.2/llm_chain/base.py
+-rw-r--r--   0 root         (0) root         (0)     2577 2023-06-26 01:19:40.000000 llm-chain-0.0.2/llm_chain/indexes.py
+-rw-r--r--   0 root         (0) root         (0)     1253 2023-06-26 16:49:38.000000 llm-chain-0.0.2/llm_chain/memory.py
+-rw-r--r--   0 root         (0) root         (0)     6458 2023-06-24 02:02:59.000000 llm-chain-0.0.2/llm_chain/models.py
+-rw-r--r--   0 root         (0) root         (0)     2172 2023-06-26 01:19:59.000000 llm-chain-0.0.2/llm_chain/prompt_templates.py
+-rw-r--r--   0 root         (0) root         (0)      695 2023-06-14 02:06:25.000000 llm-chain-0.0.2/llm_chain/resources.py
+-rw-r--r--   0 root         (0) root         (0)     2714 2023-06-26 00:25:02.000000 llm-chain-0.0.2/llm_chain/tools.py
+-rw-r--r--   0 root         (0) root         (0)     4202 2023-06-23 02:34:10.000000 llm-chain-0.0.2/llm_chain/utilities.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-26 21:19:21.524264 llm-chain-0.0.2/llm_chain.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     7647 2023-06-26 21:19:21.000000 llm-chain-0.0.2/llm_chain.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      620 2023-06-26 21:19:21.000000 llm-chain-0.0.2/llm_chain.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-06-26 21:19:21.000000 llm-chain-0.0.2/llm_chain.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       33 2023-06-26 21:19:21.000000 llm-chain-0.0.2/llm_chain.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       16 2023-06-26 21:19:21.000000 llm-chain-0.0.2/llm_chain.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)      104 2023-02-25 17:02:25.000000 llm-chain-0.0.2/pyproject.toml
+-rw-r--r--   0 root         (0) root         (0)      666 2023-06-26 21:19:21.565098 llm-chain-0.0.2/setup.cfg
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-26 21:19:21.559354 llm-chain-0.0.2/tests/
+-rw-r--r--   0 root         (0) root         (0)       52 2023-06-10 00:17:26.000000 llm-chain-0.0.2/tests/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     4281 2023-06-24 02:22:45.000000 llm-chain-0.0.2/tests/conftest.py
+-rw-r--r--   0 root         (0) root         (0)    23562 2023-06-26 01:05:52.000000 llm-chain-0.0.2/tests/test_chains.py
+-rw-r--r--   0 root         (0) root         (0)    11370 2023-06-26 17:14:59.000000 llm-chain-0.0.2/tests/test_indexes.py
+-rw-r--r--   0 root         (0) root         (0)    13991 2023-06-26 16:57:51.000000 llm-chain-0.0.2/tests/test_memory.py
+-rw-r--r--   0 root         (0) root         (0)    26878 2023-06-26 17:13:47.000000 llm-chain-0.0.2/tests/test_models.py
+-rw-r--r--   0 root         (0) root         (0)     1899 2023-06-23 05:43:22.000000 llm-chain-0.0.2/tests/test_prompt_templates.py
+-rw-r--r--   0 root         (0) root         (0)     1998 2023-06-14 02:16:47.000000 llm-chain-0.0.2/tests/test_records.py
+-rw-r--r--   0 root         (0) root         (0)    13510 2023-06-26 00:34:09.000000 llm-chain-0.0.2/tests/test_tools.py
+-rw-r--r--   0 root         (0) root         (0)     3408 2023-06-26 17:18:37.000000 llm-chain-0.0.2/tests/test_utilities.py
```

### Comparing `llm-chain-0.0.1/LICENSE` & `llm-chain-0.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `llm-chain-0.0.1/setup.cfg` & `llm-chain-0.0.2/setup.cfg`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = llm-chain
-version = 0.0.1
+version = 0.0.2
 author = Shane Kercheval
 author_email = shane.kercheval@gmail.com
 description = Simple and extensible LLM Chaining
 long_description = file: README.md
 long_description_content_type = text/markdown
 url = https://github.com/shane-kercheval/llm-chain
 project_urls = 
@@ -13,15 +13,18 @@
 	Programming Language :: Python :: 3
 	License :: OSI Approved :: MIT License
 	Operating System :: OS Independent
 
 [options]
 package_dir = 
 packages = find:
-python_requires = >=3.9
+python_requires = >=3.10
 install_requires = 
+	chromadb
+	numpy
+	tenacity
 	tiktoken
 
 [egg_info]
 tag_build = 
 tag_date = 0
```

