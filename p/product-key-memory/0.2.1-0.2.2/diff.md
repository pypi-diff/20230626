# Comparing `tmp/product_key_memory-0.2.1.tar.gz` & `tmp/product_key_memory-0.2.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "product_key_memory-0.2.1.tar", last modified: Mon Jun 26 18:22:01 2023, max compression
+gzip compressed data, was "product_key_memory-0.2.2.tar", last modified: Mon Jun 26 20:44:53 2023, max compression
```

## Comparing `product_key_memory-0.2.1.tar` & `product_key_memory-0.2.2.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 18:22:01.057201 product_key_memory-0.2.1/
--rw-r--r--   0 runner    (1001) docker     (123)     1066 2023-06-26 18:21:51.000000 product_key_memory-0.2.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      625 2023-06-26 18:22:01.057201 product_key_memory-0.2.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2635 2023-06-26 18:21:51.000000 product_key_memory-0.2.1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 18:22:01.057201 product_key_memory-0.2.1/product_key_memory/
--rw-r--r--   0 runner    (1001) docker     (123)      110 2023-06-26 18:21:51.000000 product_key_memory-0.2.1/product_key_memory/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4427 2023-06-26 18:21:51.000000 product_key_memory-0.2.1/product_key_memory/product_key_memory.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 18:22:01.057201 product_key_memory-0.2.1/product_key_memory.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      625 2023-06-26 18:22:01.000000 product_key_memory-0.2.1/product_key_memory.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      307 2023-06-26 18:22:01.000000 product_key_memory-0.2.1/product_key_memory.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-26 18:22:01.000000 product_key_memory-0.2.1/product_key_memory.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       18 2023-06-26 18:22:01.000000 product_key_memory-0.2.1/product_key_memory.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       19 2023-06-26 18:22:01.000000 product_key_memory-0.2.1/product_key_memory.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-26 18:22:01.057201 product_key_memory-0.2.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      834 2023-06-26 18:21:51.000000 product_key_memory-0.2.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 20:44:53.793591 product_key_memory-0.2.2/
+-rw-r--r--   0 runner    (1001) docker     (123)     1066 2023-06-26 20:44:43.000000 product_key_memory-0.2.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      625 2023-06-26 20:44:53.793591 product_key_memory-0.2.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2635 2023-06-26 20:44:43.000000 product_key_memory-0.2.2/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 20:44:53.793591 product_key_memory-0.2.2/product_key_memory/
+-rw-r--r--   0 runner    (1001) docker     (123)      110 2023-06-26 20:44:43.000000 product_key_memory-0.2.2/product_key_memory/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4547 2023-06-26 20:44:43.000000 product_key_memory-0.2.2/product_key_memory/product_key_memory.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 20:44:53.793591 product_key_memory-0.2.2/product_key_memory.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      625 2023-06-26 20:44:53.000000 product_key_memory-0.2.2/product_key_memory.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      307 2023-06-26 20:44:53.000000 product_key_memory-0.2.2/product_key_memory.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-26 20:44:53.000000 product_key_memory-0.2.2/product_key_memory.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       18 2023-06-26 20:44:53.000000 product_key_memory-0.2.2/product_key_memory.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       19 2023-06-26 20:44:53.000000 product_key_memory-0.2.2/product_key_memory.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-26 20:44:53.793591 product_key_memory-0.2.2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      834 2023-06-26 20:44:43.000000 product_key_memory-0.2.2/setup.py
```

### Comparing `product_key_memory-0.2.1/LICENSE` & `product_key_memory-0.2.2/LICENSE`

 * *Files identical despite different names*

### Comparing `product_key_memory-0.2.1/PKG-INFO` & `product_key_memory-0.2.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: product_key_memory
-Version: 0.2.1
+Version: 0.2.2
 Summary: Product Key Memory
 Home-page: https://github.com/lucidrains/product-key-memory
 Author: Aran Komatsuzaki, Phil Wang
 Author-email: aran1234321@gmail.com, lucidrains@gmail.com
 License: MIT
 Keywords: transformers,artificial intelligence
 Classifier: Development Status :: 4 - Beta
```

### Comparing `product_key_memory-0.2.1/README.md` & `product_key_memory-0.2.2/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -17,15 +17,15 @@
 ```python
 import torch
 from product_key_memory import PKM
 
 pkm = PKM(
     dim = 512,
     heads = 4,
-    dim_head = 256,       # keep at 256 for best results
+    dim_head = 128,       # keep at 128 for best results
     num_keys = 256,       # number of subkeys, # values will be num_keys ^ 2
     topk = 32             # the top number of subkeys to select
 )
 
 x = torch.randn(1, 1024, 512)
 mask = torch.ones((1, 1024)).bool()
 values = pkm(x, input_mask = mask) # (1, 1024, 512)
```

#### html2text {}

```diff
@@ -1,13 +1,13 @@
 ## Product Key Memory [![PyPI version](https://badge.fury.io/py/product-key-
 memory.svg)](https://badge.fury.io/py/product-key-memory) Standalone Product
 Key_Memory module for augmenting Transformer models ## Install ```bash $ pip
 install product-key-memory ``` ## Usage Replace the feedforwards in a
 Transformer with the following ```python import torch from product_key_memory
-import PKM pkm = PKM( dim = 512, heads = 4, dim_head = 256, # keep at 256 for
+import PKM pkm = PKM( dim = 512, heads = 4, dim_head = 128, # keep at 128 for
 best results num_keys = 256, # number of subkeys, # values will be num_keys ^ 2
 topk = 32 # the top number of subkeys to select ) x = torch.randn(1, 1024, 512)
 mask = torch.ones((1, 1024)).bool() values = pkm(x, input_mask = mask) # (1,
 1024, 512) ``` ## Learning Rates To give different learning rates to the value
 parameters of the product-key-memory network, use the following helper
 function. ```python from torch.optim import Adam from product_key_memory import
 fetch_pkm_value_parameters # this helper function, for your root model, finds
```

### Comparing `product_key_memory-0.2.1/product_key_memory/product_key_memory.py` & `product_key_memory-0.2.2/product_key_memory/product_key_memory.py`

 * *Files 5% similar despite different names*

```diff
@@ -67,16 +67,18 @@
         heads = 4,
         num_keys = 128,
         topk = 32,
         dim_head = 128,
         input_dropout = 0.,
         query_dropout = 0.,
         value_dropout = 0.,
-        use_layernorm = False,
-        pre_layernorm = False
+        attn_dropout = 0.,
+        use_layernorm = True,
+        pre_layernorm = False,
+
     ):
         super().__init__()
         self.topk = topk
         self.heads = heads
         self.num_keys = num_keys
 
         dim_query = dim_head * heads * 2
@@ -99,14 +101,15 @@
         self.values = nn.EmbeddingBag(num_keys ** 2, dim, mode = 'sum')
         init_(self.keys)
         init_(self.values.weight)
 
         self.input_dropout = nn.Dropout(input_dropout)
         self.query_dropout = nn.Dropout(query_dropout)
         self.value_dropout = nn.Dropout(value_dropout)
+        self.attn_dropout = nn.Dropout(attn_dropout)
 
     def forward(
         self,
         x,
         input_mask = None,
         **kwargs
     ):
@@ -155,14 +158,15 @@
 
         final_topk, final_indices = all_scores.topk(self.topk, dim=-1)
         value_indices = all_indices.gather(-1, final_indices)
 
         # attention
 
         attn = final_topk.softmax(dim=-1)
+        attn = self.attn_dropout(attn)
 
         value_indices, attn = map(lambda t: rearrange(t, 'b t h k -> (b t) (h k)'), (value_indices, attn))
 
         # aggregate
 
         out = self.values(value_indices, per_sample_weights=attn)
         out = self.value_dropout(out)
```

### Comparing `product_key_memory-0.2.1/product_key_memory.egg-info/PKG-INFO` & `product_key_memory-0.2.2/product_key_memory.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: product-key-memory
-Version: 0.2.1
+Version: 0.2.2
 Summary: Product Key Memory
 Home-page: https://github.com/lucidrains/product-key-memory
 Author: Aran Komatsuzaki, Phil Wang
 Author-email: aran1234321@gmail.com, lucidrains@gmail.com
 License: MIT
 Keywords: transformers,artificial intelligence
 Classifier: Development Status :: 4 - Beta
```

### Comparing `product_key_memory-0.2.1/setup.py` & `product_key_memory-0.2.2/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 from setuptools import setup, find_packages
 
 setup(
     name = 'product_key_memory',
     packages = find_packages(),
-    version = '0.2.1',
+    version = '0.2.2',
     license='MIT',
     description = 'Product Key Memory',
     long_description_content_type = 'text/markdown',
     author = 'Aran Komatsuzaki, Phil Wang',
     author_email = 'aran1234321@gmail.com, lucidrains@gmail.com',
     url = 'https://github.com/lucidrains/product-key-memory',
     keywords = ['transformers', 'artificial intelligence'],
```

