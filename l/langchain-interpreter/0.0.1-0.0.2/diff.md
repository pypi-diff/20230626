# Comparing `tmp/langchain_interpreter-0.0.1.tar.gz` & `tmp/langchain_interpreter-0.0.2.tar.gz`

## Comparing `langchain_interpreter-0.0.1.tar` & `langchain_interpreter-0.0.2.tar`

### file list

```diff
@@ -1,13 +1,13 @@
--rw-r--r--   0        0        0     9921 2020-02-02 00:00:00.000000 langchain_interpreter-0.0.1/src/examples/chains_from_json.ipynb
--rw-r--r--   0        0        0     2255 2020-02-02 00:00:00.000000 langchain_interpreter-0.0.1/src/examples/json_from_chains.ipynb
--rwxr-xr-x   0        0        0      262 2020-02-02 00:00:00.000000 langchain_interpreter-0.0.1/src/json/llmchain.json
--rw-r--r--   0        0        0     1146 2020-02-02 00:00:00.000000 langchain_interpreter-0.0.1/src/json/seq_chain.json
--rw-r--r--   0        0        0     2096 2020-02-02 00:00:00.000000 langchain_interpreter-0.0.1/src/json/seq_chain_memory.json
--rw-r--r--   0        0        0      942 2020-02-02 00:00:00.000000 langchain_interpreter-0.0.1/src/json/simple_seq_chain.json
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 langchain_interpreter-0.0.1/src/langchain_interpreter/__init__.py
--rwxr-xr-x   0        0        0     2222 2020-02-02 00:00:00.000000 langchain_interpreter-0.0.1/src/langchain_interpreter/main.py
--rw-r--r--   0        0        0     3087 2020-02-02 00:00:00.000000 langchain_interpreter-0.0.1/.gitignore
--rw-r--r--   0        0        0     1068 2020-02-02 00:00:00.000000 langchain_interpreter-0.0.1/LICENSE
--rw-r--r--   0        0        0      110 2020-02-02 00:00:00.000000 langchain_interpreter-0.0.1/README.md
--rw-r--r--   0        0        0      616 2020-02-02 00:00:00.000000 langchain_interpreter-0.0.1/pyproject.toml
--rw-r--r--   0        0        0      665 2020-02-02 00:00:00.000000 langchain_interpreter-0.0.1/PKG-INFO
+-rw-r--r--   0        0        0     9921 2020-02-02 00:00:00.000000 langchain_interpreter-0.0.2/src/examples/chains_from_json.ipynb
+-rw-r--r--   0        0        0     2255 2020-02-02 00:00:00.000000 langchain_interpreter-0.0.2/src/examples/json_from_chains.ipynb
+-rwxr-xr-x   0        0        0      262 2020-02-02 00:00:00.000000 langchain_interpreter-0.0.2/src/json/llmchain.json
+-rw-r--r--   0        0        0     1146 2020-02-02 00:00:00.000000 langchain_interpreter-0.0.2/src/json/seq_chain.json
+-rw-r--r--   0        0        0     2096 2020-02-02 00:00:00.000000 langchain_interpreter-0.0.2/src/json/seq_chain_memory.json
+-rw-r--r--   0        0        0      942 2020-02-02 00:00:00.000000 langchain_interpreter-0.0.2/src/json/simple_seq_chain.json
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 langchain_interpreter-0.0.2/src/langchain_interpreter/__init__.py
+-rwxr-xr-x   0        0        0     2393 2020-02-02 00:00:00.000000 langchain_interpreter-0.0.2/src/langchain_interpreter/main.py
+-rw-r--r--   0        0        0     3087 2020-02-02 00:00:00.000000 langchain_interpreter-0.0.2/.gitignore
+-rw-r--r--   0        0        0     1068 2020-02-02 00:00:00.000000 langchain_interpreter-0.0.2/LICENSE
+-rw-r--r--   0        0        0      110 2020-02-02 00:00:00.000000 langchain_interpreter-0.0.2/README.md
+-rw-r--r--   0        0        0      616 2020-02-02 00:00:00.000000 langchain_interpreter-0.0.2/pyproject.toml
+-rw-r--r--   0        0        0      665 2020-02-02 00:00:00.000000 langchain_interpreter-0.0.2/PKG-INFO
```

### Comparing `langchain_interpreter-0.0.1/src/examples/chains_from_json.ipynb` & `langchain_interpreter-0.0.2/src/examples/chains_from_json.ipynb`

 * *Files identical despite different names*

### Comparing `langchain_interpreter-0.0.1/src/examples/json_from_chains.ipynb` & `langchain_interpreter-0.0.2/src/examples/json_from_chains.ipynb`

 * *Files identical despite different names*

### Comparing `langchain_interpreter-0.0.1/src/json/seq_chain.json` & `langchain_interpreter-0.0.2/src/json/seq_chain.json`

 * *Files identical despite different names*

### Comparing `langchain_interpreter-0.0.1/src/json/seq_chain_memory.json` & `langchain_interpreter-0.0.2/src/json/seq_chain_memory.json`

 * *Files identical despite different names*

### Comparing `langchain_interpreter-0.0.1/src/json/simple_seq_chain.json` & `langchain_interpreter-0.0.2/src/json/simple_seq_chain.json`

 * *Files identical despite different names*

### Comparing `langchain_interpreter-0.0.1/src/langchain_interpreter/main.py` & `langchain_interpreter-0.0.2/src/langchain_interpreter/main.py`

 * *Files 20% similar despite different names*

```diff
@@ -7,56 +7,56 @@
 
 def chain_from_file(filename):
     with open(filename) as f:
         cfg = json.load(f)
     return get_chain(cfg)
 
 
-def chain_from_str(s):
-    return get_chain(json.loads(s))
+def chain_from_str(s, **kwargs):
+    return get_chain(json.loads(s), **kwargs)
 
 
-def get_chain(cfg):
+def get_chain(cfg, **kwargs):
     if cfg["type"] == "LLMChain":
-        return get_llm_chain(cfg)
+        return get_llm_chain(cfg, **kwargs)
     if cfg["type"] == "SimpleSequentialChain":
-        return get_simple_sequential_chain(cfg)
+        return get_simple_sequential_chain(cfg, **kwargs)
     if cfg["type"] == "SequentialChain":
-        return get_sequential_chain(cfg)
+        return get_sequential_chain(cfg, **kwargs)
 
 
-def get_llm(cfg):
+def get_llm(cfg, **kwargs):
     llm_type = type_to_cls_dict[cfg["name"]]
-    llm = llm_type(**cfg["args"])
+    llm = llm_type(**cfg["args"], openai_api_key=kwargs["openai_api_key"])
     return llm
 
 
-def get_llm_chain(cfg):
-    llm = get_llm(cfg["llm"])
+def get_llm_chain(cfg, **kwargs):
+    llm = get_llm(cfg["llm"], **kwargs)
     prompt = get_prompt(cfg["prompt"])
     output_key = cfg.get("output_key", "text")
     memory = try_memory(cfg)
     llm_chain = LLMChain(llm=llm, prompt=prompt, output_key=output_key, memory=memory)
     return llm_chain
 
 
-def get_simple_sequential_chain(cfg):
-    chains = [get_chain(chain) for chain in cfg["chains"]]
+def get_simple_sequential_chain(cfg, **kwargs):
+    chains = [get_chain(chain, **kwargs) for chain in cfg["chains"]]
     memory = try_memory(cfg)
     ss_chain = SimpleSequentialChain(chains=chains, verbose=True, memory=memory)
     return ss_chain
 
 
 def get_prompt(cfg):
     prompt = PromptTemplate(**cfg)
     return prompt
 
 
-def get_sequential_chain(cfg):
-    chains = [get_chain(chain) for chain in cfg["chains"]]
+def get_sequential_chain(cfg, **kwargs):
+    chains = [get_chain(chain, **kwargs) for chain in cfg["chains"]]
     input_variables = cfg["input_variables"]
     output_variables = cfg["output_variables"]
     memory = try_memory(cfg)
     seq_chain = SequentialChain(
         chains=chains,
         input_variables=input_variables,
         output_variables=output_variables,
```

### Comparing `langchain_interpreter-0.0.1/.gitignore` & `langchain_interpreter-0.0.2/.gitignore`

 * *Files identical despite different names*

### Comparing `langchain_interpreter-0.0.1/LICENSE` & `langchain_interpreter-0.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `langchain_interpreter-0.0.1/pyproject.toml` & `langchain_interpreter-0.0.2/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["hatchling"]
 build-backend = "hatchling.build"
 
 [project]
 name = "langchain_interpreter"
-version = "0.0.1"
+version = "0.0.2"
 authors = [
   { name="Elijah Tarr", email="elijahotarr@gmail.com" },
 ]
 description = "A way to turn json into langchain pipelines."
 readme = "README.md"
 requires-python = ">=3.7"
 classifiers = [
```

### Comparing `langchain_interpreter-0.0.1/PKG-INFO` & `langchain_interpreter-0.0.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: langchain_interpreter
-Version: 0.0.1
+Version: 0.0.2
 Summary: A way to turn json into langchain pipelines.
 Project-URL: Homepage, https://github.com/eoriont/langchain_interpreter
 Project-URL: Bug Tracker, https://github.com/eoriont/langchain_interpreter/issues
 Author-email: Elijah Tarr <elijahotarr@gmail.com>
 License-File: LICENSE
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

