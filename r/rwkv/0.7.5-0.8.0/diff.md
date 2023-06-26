# Comparing `tmp/rwkv-0.7.5.tar.gz` & `tmp/rwkv-0.8.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "rwkv-0.7.5.tar", last modified: Sat Jun 10 18:52:42 2023, max compression
+gzip compressed data, was "rwkv-0.8.0.tar", last modified: Mon Jun 26 03:15:20 2023, max compression
```

## Comparing `rwkv-0.7.5.tar` & `rwkv-0.8.0.tar`

### file list

```diff
@@ -1,23 +1,23 @@
-drwxr-xr-x   0 blinkdl  (424401630) Domain Users (424400513)        0 2023-06-10 18:52:42.000000 rwkv-0.7.5/
--rw-r--r--   0 blinkdl  (424401630) Domain Users (424400513)    11357 2023-03-01 07:25:16.000000 rwkv-0.7.5/LICENSE
--rw-r--r--   0 blinkdl  (424401630) Domain Users (424400513)       47 2023-05-19 16:15:03.000000 rwkv-0.7.5/MANIFEST.in
--rw-r--r--   0 blinkdl  (424401630) Domain Users (424400513)     4770 2023-06-10 18:52:42.000000 rwkv-0.7.5/PKG-INFO
--rw-r--r--   0 blinkdl  (424401630) Domain Users (424400513)     4300 2023-03-18 18:39:01.000000 rwkv-0.7.5/README.md
--rw-r--r--   0 blinkdl  (424401630) Domain Users (424400513)      499 2023-06-10 18:51:50.000000 rwkv-0.7.5/pyproject.toml
--rw-r--r--   0 blinkdl  (424401630) Domain Users (424400513)       38 2023-06-10 18:52:42.000000 rwkv-0.7.5/setup.cfg
-drwxr-xr-x   0 blinkdl  (424401630) Domain Users (424400513)        0 2023-06-10 18:52:42.000000 rwkv-0.7.5/src/
-drwxr-xr-x   0 blinkdl  (424401630) Domain Users (424400513)        0 2023-06-10 18:52:42.000000 rwkv-0.7.5/src/rwkv/
--rw-r--r--   0 blinkdl  (424401630) Domain Users (424400513)        0 2023-02-28 12:56:58.000000 rwkv-0.7.5/src/rwkv/__init__.py
-drwxr-xr-x   0 blinkdl  (424401630) Domain Users (424400513)        0 2023-06-10 18:52:42.000000 rwkv-0.7.5/src/rwkv/cuda/
--rw-r--r--   0 blinkdl  (424401630) Domain Users (424400513)     8677 2023-04-27 19:18:02.000000 rwkv-0.7.5/src/rwkv/cuda/operators.cu
--rw-r--r--   0 blinkdl  (424401630) Domain Users (424400513)     4702 2023-04-27 19:18:02.000000 rwkv-0.7.5/src/rwkv/cuda/wrapper.cpp
--rw-r--r--   0 blinkdl  (424401630) Domain Users (424400513)    33248 2023-05-20 13:47:14.000000 rwkv-0.7.5/src/rwkv/model.py
--rw-r--r--   0 blinkdl  (424401630) Domain Users (424400513)     3201 2023-06-10 18:48:52.000000 rwkv-0.7.5/src/rwkv/rwkv_tokenizer.py
--rw-r--r--   0 blinkdl  (424401630) Domain Users (424400513)  1093733 2023-05-18 04:00:58.000000 rwkv-0.7.5/src/rwkv/rwkv_vocab_v20230424.txt
--rw-r--r--   0 blinkdl  (424401630) Domain Users (424400513)     5141 2023-05-20 13:47:38.000000 rwkv-0.7.5/src/rwkv/utils.py
-drwxr-xr-x   0 blinkdl  (424401630) Domain Users (424400513)        0 2023-06-10 18:52:42.000000 rwkv-0.7.5/src/rwkv.egg-info/
--rw-r--r--   0 blinkdl  (424401630) Domain Users (424400513)     4770 2023-06-10 18:52:42.000000 rwkv-0.7.5/src/rwkv.egg-info/PKG-INFO
--rw-r--r--   0 blinkdl  (424401630) Domain Users (424400513)      374 2023-06-10 18:52:42.000000 rwkv-0.7.5/src/rwkv.egg-info/SOURCES.txt
--rw-r--r--   0 blinkdl  (424401630) Domain Users (424400513)        1 2023-06-10 18:52:42.000000 rwkv-0.7.5/src/rwkv.egg-info/dependency_links.txt
--rw-r--r--   0 blinkdl  (424401630) Domain Users (424400513)       19 2023-06-10 18:52:42.000000 rwkv-0.7.5/src/rwkv.egg-info/requires.txt
--rw-r--r--   0 blinkdl  (424401630) Domain Users (424400513)        5 2023-06-10 18:52:42.000000 rwkv-0.7.5/src/rwkv.egg-info/top_level.txt
+drwxr-xr-x   0 blinkdl  (424401630) Domain Users (424400513)        0 2023-06-26 03:15:20.000000 rwkv-0.8.0/
+-rw-r--r--   0 blinkdl  (424401630) Domain Users (424400513)    11357 2023-03-01 07:25:16.000000 rwkv-0.8.0/LICENSE
+-rw-r--r--   0 blinkdl  (424401630) Domain Users (424400513)       47 2023-05-19 16:15:03.000000 rwkv-0.8.0/MANIFEST.in
+-rw-r--r--   0 blinkdl  (424401630) Domain Users (424400513)     4840 2023-06-26 03:15:20.000000 rwkv-0.8.0/PKG-INFO
+-rw-r--r--   0 blinkdl  (424401630) Domain Users (424400513)     4370 2023-06-26 03:06:27.000000 rwkv-0.8.0/README.md
+-rw-r--r--   0 blinkdl  (424401630) Domain Users (424400513)      499 2023-06-26 02:50:44.000000 rwkv-0.8.0/pyproject.toml
+-rw-r--r--   0 blinkdl  (424401630) Domain Users (424400513)       38 2023-06-26 03:15:20.000000 rwkv-0.8.0/setup.cfg
+drwxr-xr-x   0 blinkdl  (424401630) Domain Users (424400513)        0 2023-06-26 03:15:20.000000 rwkv-0.8.0/src/
+drwxr-xr-x   0 blinkdl  (424401630) Domain Users (424400513)        0 2023-06-26 03:15:20.000000 rwkv-0.8.0/src/rwkv/
+-rw-r--r--   0 blinkdl  (424401630) Domain Users (424400513)        0 2023-02-28 12:56:58.000000 rwkv-0.8.0/src/rwkv/__init__.py
+drwxr-xr-x   0 blinkdl  (424401630) Domain Users (424400513)        0 2023-06-26 03:15:20.000000 rwkv-0.8.0/src/rwkv/cuda/
+-rw-r--r--   0 blinkdl  (424401630) Domain Users (424400513)     8677 2023-04-27 19:18:02.000000 rwkv-0.8.0/src/rwkv/cuda/operators.cu
+-rw-r--r--   0 blinkdl  (424401630) Domain Users (424400513)     4702 2023-04-27 19:18:02.000000 rwkv-0.8.0/src/rwkv/cuda/wrapper.cpp
+-rw-r--r--   0 blinkdl  (424401630) Domain Users (424400513)    33248 2023-05-20 13:47:14.000000 rwkv-0.8.0/src/rwkv/model.py
+-rw-r--r--   0 blinkdl  (424401630) Domain Users (424400513)     3201 2023-06-10 18:48:52.000000 rwkv-0.8.0/src/rwkv/rwkv_tokenizer.py
+-rw-r--r--   0 blinkdl  (424401630) Domain Users (424400513)  1093733 2023-05-18 04:00:58.000000 rwkv-0.8.0/src/rwkv/rwkv_vocab_v20230424.txt
+-rw-r--r--   0 blinkdl  (424401630) Domain Users (424400513)     5356 2023-06-26 03:07:02.000000 rwkv-0.8.0/src/rwkv/utils.py
+drwxr-xr-x   0 blinkdl  (424401630) Domain Users (424400513)        0 2023-06-26 03:15:20.000000 rwkv-0.8.0/src/rwkv.egg-info/
+-rw-r--r--   0 blinkdl  (424401630) Domain Users (424400513)     4840 2023-06-26 03:15:20.000000 rwkv-0.8.0/src/rwkv.egg-info/PKG-INFO
+-rw-r--r--   0 blinkdl  (424401630) Domain Users (424400513)      374 2023-06-26 03:15:20.000000 rwkv-0.8.0/src/rwkv.egg-info/SOURCES.txt
+-rw-r--r--   0 blinkdl  (424401630) Domain Users (424400513)        1 2023-06-26 03:15:20.000000 rwkv-0.8.0/src/rwkv.egg-info/dependency_links.txt
+-rw-r--r--   0 blinkdl  (424401630) Domain Users (424400513)       19 2023-06-26 03:15:20.000000 rwkv-0.8.0/src/rwkv.egg-info/requires.txt
+-rw-r--r--   0 blinkdl  (424401630) Domain Users (424400513)        5 2023-06-26 03:15:20.000000 rwkv-0.8.0/src/rwkv.egg-info/top_level.txt
```

### Comparing `rwkv-0.7.5/LICENSE` & `rwkv-0.8.0/LICENSE`

 * *Files identical despite different names*

### Comparing `rwkv-0.7.5/PKG-INFO` & `rwkv-0.8.0/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -1,21 +1,7 @@
-Metadata-Version: 2.1
-Name: rwkv
-Version: 0.7.5
-Summary: The RWKV Language Model
-Author: Bo PENG
-Project-URL: Homepage, https://github.com/BlinkDL/ChatRWKV
-Project-URL: Bug Tracker, https://github.com/BlinkDL/ChatRWKV/issues
-Classifier: Programming Language :: Python :: 3
-Classifier: License :: OSI Approved :: Apache Software License
-Classifier: Operating System :: OS Independent
-Requires-Python: >=3.7
-Description-Content-Type: text/markdown
-License-File: LICENSE
-
 The RWKV Language Model
 
 https://github.com/BlinkDL/ChatRWKV
 
 https://github.com/BlinkDL/RWKV-LM
 
 ```python
@@ -76,22 +62,23 @@
 
 # For alpha_frequency and alpha_presence, see "Frequency and presence penalties":
 # https://platform.openai.com/docs/api-reference/parameter-details
 
 args = PIPELINE_ARGS(temperature = 1.0, top_p = 0.7, top_k = 100, # top_k = 0 then ignore
                      alpha_frequency = 0.25,
                      alpha_presence = 0.25,
+                     alpha_decay=0.996, # gradually decay the penalty
                      token_ban = [0], # ban the generation of some tokens
                      token_stop = [], # stop generation whenever you see any token here
                      chunk_len = 256) # split input into chunks to save VRAM (shorter -> slower)
 
 pipeline.generate(ctx, token_count=200, args=args, callback=my_print)
 print('\n')
 
 out, state = model.forward([187, 510, 1563, 310, 247], None)
 print(out.detach().cpu().numpy())                   # get logits
 out, state = model.forward([187, 510], None)
 out, state = model.forward([1563], state)           # RNN has state (use deepcopy to clone states)
 out, state = model.forward([310, 247], state)
 print(out.detach().cpu().numpy())                   # same result as above
 print('\n')
-```
+```
```

### Comparing `rwkv-0.7.5/README.md` & `rwkv-0.8.0/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,7 +1,21 @@
+Metadata-Version: 2.1
+Name: rwkv
+Version: 0.8.0
+Summary: The RWKV Language Model
+Author: Bo PENG
+Project-URL: Homepage, https://github.com/BlinkDL/ChatRWKV
+Project-URL: Bug Tracker, https://github.com/BlinkDL/ChatRWKV/issues
+Classifier: Programming Language :: Python :: 3
+Classifier: License :: OSI Approved :: Apache Software License
+Classifier: Operating System :: OS Independent
+Requires-Python: >=3.7
+Description-Content-Type: text/markdown
+License-File: LICENSE
+
 The RWKV Language Model
 
 https://github.com/BlinkDL/ChatRWKV
 
 https://github.com/BlinkDL/RWKV-LM
 
 ```python
@@ -62,22 +76,23 @@
 
 # For alpha_frequency and alpha_presence, see "Frequency and presence penalties":
 # https://platform.openai.com/docs/api-reference/parameter-details
 
 args = PIPELINE_ARGS(temperature = 1.0, top_p = 0.7, top_k = 100, # top_k = 0 then ignore
                      alpha_frequency = 0.25,
                      alpha_presence = 0.25,
+                     alpha_decay=0.996, # gradually decay the penalty
                      token_ban = [0], # ban the generation of some tokens
                      token_stop = [], # stop generation whenever you see any token here
                      chunk_len = 256) # split input into chunks to save VRAM (shorter -> slower)
 
 pipeline.generate(ctx, token_count=200, args=args, callback=my_print)
 print('\n')
 
 out, state = model.forward([187, 510, 1563, 310, 247], None)
 print(out.detach().cpu().numpy())                   # get logits
 out, state = model.forward([187, 510], None)
 out, state = model.forward([1563], state)           # RNN has state (use deepcopy to clone states)
 out, state = model.forward([310, 247], state)
 print(out.detach().cpu().numpy())                   # same result as above
 print('\n')
-```
+```
```

### Comparing `rwkv-0.7.5/src/rwkv/cuda/operators.cu` & `rwkv-0.8.0/src/rwkv/cuda/operators.cu`

 * *Files identical despite different names*

### Comparing `rwkv-0.7.5/src/rwkv/cuda/wrapper.cpp` & `rwkv-0.8.0/src/rwkv/cuda/wrapper.cpp`

 * *Files identical despite different names*

### Comparing `rwkv-0.7.5/src/rwkv/model.py` & `rwkv-0.8.0/src/rwkv/model.py`

 * *Files identical despite different names*

### Comparing `rwkv-0.7.5/src/rwkv/rwkv_tokenizer.py` & `rwkv-0.8.0/src/rwkv/rwkv_tokenizer.py`

 * *Files identical despite different names*

### Comparing `rwkv-0.7.5/src/rwkv/rwkv_vocab_v20230424.txt` & `rwkv-0.8.0/src/rwkv/rwkv_vocab_v20230424.txt`

 * *Files identical despite different names*

### Comparing `rwkv-0.7.5/src/rwkv/utils.py` & `rwkv-0.8.0/src/rwkv/utils.py`

 * *Files 8% similar despite different names*

```diff
@@ -4,20 +4,21 @@
 
 import os, sys
 import numpy as np
 import torch
 from torch.nn import functional as F
 
 class PIPELINE_ARGS():
-    def __init__(self, temperature=1.0, top_p=0.85, top_k=0, alpha_frequency=0.2, alpha_presence=0.2, token_ban=[], token_stop=[], chunk_len=256):
+    def __init__(self, temperature=1.0, top_p=0.85, top_k=0, alpha_frequency=0.2, alpha_presence=0.2, alpha_decay=0.996, token_ban=[], token_stop=[], chunk_len=256):
         self.temperature = temperature
         self.top_p = top_p
         self.top_k = top_k
         self.alpha_frequency = alpha_frequency # Frequency Penalty (as in GPT-3)
         self.alpha_presence = alpha_presence # Presence Penalty (as in GPT-3)
+        self.alpha_decay = alpha_decay # gradually decay the penalty
         self.token_ban = token_ban # ban the generation of some tokens
         self.token_stop = token_stop # stop generation whenever you see any token here
         self.chunk_len = chunk_len # split input into chunks to save VRAM (shorter -> slower)
 
 class PIPELINE():
     def __init__(self, model, WORD_NAME):
         self.model = model
@@ -101,18 +102,21 @@
                 out[n] -= (args.alpha_presence + occurrence[n] * args.alpha_frequency)
             
             # sampler
             token = self.sample_logits(out, temperature=args.temperature, top_p=args.top_p, top_k=args.top_k)
             if token in args.token_stop:
                 break
             all_tokens += [token]
+            for xxx in occurrence:
+                occurrence[xxx] *= args.alpha_decay
             if token not in occurrence:
                 occurrence[token] = 1
             else:
                 occurrence[token] += 1
+            # print(occurrence) # debug
             
             # output
             tmp = self.decode(all_tokens[out_last:])
             if '\ufffd' not in tmp: # is valid utf-8 string?
                 if callback:
                     callback(tmp)
                 out_str += tmp
```

### Comparing `rwkv-0.7.5/src/rwkv.egg-info/PKG-INFO` & `rwkv-0.8.0/src/rwkv.egg-info/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: rwkv
-Version: 0.7.5
+Version: 0.8.0
 Summary: The RWKV Language Model
 Author: Bo PENG
 Project-URL: Homepage, https://github.com/BlinkDL/ChatRWKV
 Project-URL: Bug Tracker, https://github.com/BlinkDL/ChatRWKV/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: OS Independent
@@ -76,14 +76,15 @@
 
 # For alpha_frequency and alpha_presence, see "Frequency and presence penalties":
 # https://platform.openai.com/docs/api-reference/parameter-details
 
 args = PIPELINE_ARGS(temperature = 1.0, top_p = 0.7, top_k = 100, # top_k = 0 then ignore
                      alpha_frequency = 0.25,
                      alpha_presence = 0.25,
+                     alpha_decay=0.996, # gradually decay the penalty
                      token_ban = [0], # ban the generation of some tokens
                      token_stop = [], # stop generation whenever you see any token here
                      chunk_len = 256) # split input into chunks to save VRAM (shorter -> slower)
 
 pipeline.generate(ctx, token_count=200, args=args, callback=my_print)
 print('\n')
```

