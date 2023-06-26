# Comparing `tmp/product_key_memory-0.1.9.tar.gz` & `tmp/product_key_memory-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/product_key_memory-0.1.9.tar", last modified: Tue Jun  9 15:06:37 2020, max compression
+gzip compressed data, was "product_key_memory-0.2.0.tar", last modified: Mon Jun 26 15:19:23 2023, max compression
```

## Comparing `product_key_memory-0.1.9.tar` & `product_key_memory-0.2.0.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxrwxr-x   0 phil      (1000) phil      (1000)        0 2020-06-09 15:06:37.000000 product_key_memory-0.1.9/
-drwxrwxr-x   0 phil      (1000) phil      (1000)        0 2020-06-09 15:06:37.000000 product_key_memory-0.1.9/product_key_memory/
--rw-rw-r--   0 phil      (1000) phil      (1000)      159 2020-06-09 15:05:58.000000 product_key_memory-0.1.9/product_key_memory/__init__.py
--rw-rw-r--   0 phil      (1000) phil      (1000)     3843 2020-06-09 06:19:03.000000 product_key_memory-0.1.9/product_key_memory/product_key_memory.py
--rw-rw-r--   0 phil      (1000) phil      (1000)     2423 2020-06-09 06:45:38.000000 product_key_memory-0.1.9/product_key_memory/evonorm.py
--rw-rw-r--   0 phil      (1000) phil      (1000)      602 2020-06-09 15:06:37.000000 product_key_memory-0.1.9/PKG-INFO
-drwxrwxr-x   0 phil      (1000) phil      (1000)        0 2020-06-09 15:06:37.000000 product_key_memory-0.1.9/product_key_memory.egg-info/
--rw-rw-r--   0 phil      (1000) phil      (1000)      329 2020-06-09 15:06:37.000000 product_key_memory-0.1.9/product_key_memory.egg-info/SOURCES.txt
--rw-rw-r--   0 phil      (1000) phil      (1000)       19 2020-06-09 15:06:37.000000 product_key_memory-0.1.9/product_key_memory.egg-info/top_level.txt
--rw-rw-r--   0 phil      (1000) phil      (1000)        1 2020-06-09 15:06:37.000000 product_key_memory-0.1.9/product_key_memory.egg-info/dependency_links.txt
--rw-rw-r--   0 phil      (1000) phil      (1000)      602 2020-06-09 15:06:37.000000 product_key_memory-0.1.9/product_key_memory.egg-info/PKG-INFO
--rw-rw-r--   0 phil      (1000) phil      (1000)        6 2020-06-09 15:06:37.000000 product_key_memory-0.1.9/product_key_memory.egg-info/requires.txt
--rw-rw-r--   0 phil      (1000) phil      (1000)       38 2020-06-09 15:06:37.000000 product_key_memory-0.1.9/setup.cfg
--rw-rw-r--   0 phil      (1000) phil      (1000)      719 2020-06-09 15:05:38.000000 product_key_memory-0.1.9/setup.py
--rw-rw-r--   0 phil      (1000) phil      (1000)     2777 2020-06-09 06:19:03.000000 product_key_memory-0.1.9/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 15:19:23.398293 product_key_memory-0.2.0/
+-rw-r--r--   0 runner    (1001) docker     (123)     1066 2023-06-26 15:19:09.000000 product_key_memory-0.2.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      625 2023-06-26 15:19:23.398293 product_key_memory-0.2.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2635 2023-06-26 15:19:09.000000 product_key_memory-0.2.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 15:19:23.398293 product_key_memory-0.2.0/product_key_memory/
+-rw-r--r--   0 runner    (1001) docker     (123)      110 2023-06-26 15:19:09.000000 product_key_memory-0.2.0/product_key_memory/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4244 2023-06-26 15:19:09.000000 product_key_memory-0.2.0/product_key_memory/product_key_memory.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 15:19:23.398293 product_key_memory-0.2.0/product_key_memory.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      625 2023-06-26 15:19:23.000000 product_key_memory-0.2.0/product_key_memory.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      307 2023-06-26 15:19:23.000000 product_key_memory-0.2.0/product_key_memory.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-26 15:19:23.000000 product_key_memory-0.2.0/product_key_memory.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       18 2023-06-26 15:19:23.000000 product_key_memory-0.2.0/product_key_memory.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       19 2023-06-26 15:19:23.000000 product_key_memory-0.2.0/product_key_memory.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-26 15:19:23.398293 product_key_memory-0.2.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      834 2023-06-26 15:19:09.000000 product_key_memory-0.2.0/setup.py
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive (GNU)
+POSIX tar archive
```

### Comparing `product_key_memory-0.1.9/product_key_memory/product_key_memory.py` & `product_key_memory-0.2.0/product_key_memory/product_key_memory.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,23 +1,29 @@
-import torch
 import math
-from torch import nn
-from product_key_memory.evonorm import EvoNorm1D
+import torch
+from torch import nn, einsum
+
+from einops import rearrange
+
+# helper functions
+
+def exists(val):
+    return val is not None
+
+def default(val, d):
+    return val if exists(val) else d
+
+# init
 
 def init_(t, dim = None):
-    dim = dim if dim is not None else t.shape[-1]
+    dim = default(dim, t.shape[-1])
     std = 1. / math.sqrt(dim)
     return nn.init.normal_(t, mean=0, std=std)
 
-def expand_dim(t, dim, k, unsqueeze = False):
-    if unsqueeze:
-        t = t.unsqueeze(dim)
-    expand_shape = [-1] * len(t.shape)
-    expand_shape[dim] = k
-    return t.expand(*expand_shape)
+# optimizer
 
 def list_subtract(l, r):
     return [el for el in l if el not in set(r)]
 
 def fetch_pkm_value_parameters(module):
     params = []
     for m in module.modules():
@@ -26,91 +32,132 @@
     rest = list_subtract(module.parameters(), params)
     return params, rest
 
 def fetch_optimizer_parameters(module, pkm_learning_rate = 1e-2):
     pkm_params, rest = fetch_pkm_value_parameters(module)
     return [{'params': rest}, {'params': pkm_params, 'lr': pkm_learning_rate}]
 
+# norm
+
 class MaskedBatchNorm1D(nn.Module):
     def __init__(self, fn):
         super().__init__()
         self.fn = fn
 
-    def forward(self, x, mask = None):
-        b, t, d = x.shape
-        has_mask = mask is not None
-
-        if has_mask:
+    def forward(
+        self,
+        x,
+        mask = None
+    ):
+        if exists(mask):
             initial_x = x
-            mask = mask.unsqueeze(-1)
-            x = x.masked_select(mask)
+            x = x[mask]
 
-        shape = x.shape
-        x = x.reshape(-1, d)
         x = self.fn(x)
-        x = x.reshape(*shape)
 
-        if has_mask:
-            x = initial_x.masked_scatter(mask, x)
+        if exists(mask):
+            initial_x[mask] = x
+            x = initial_x
 
         return x
 
 class PKM(nn.Module):
-    def __init__(self, dim, heads = 4, num_keys = 128, topk = 32, dim_head = 256, input_dropout = 0., query_dropout = 0., value_dropout = 0., use_evonorm = False, causal = False):
+    def __init__(
+        self,
+        dim,
+        heads = 4,
+        num_keys = 128,
+        topk = 32,
+        dim_head = 128,
+        input_dropout = 0.,
+        query_dropout = 0.,
+        value_dropout = 0.,
+        use_layernorm = False
+    ):
         super().__init__()
-        assert (dim % heads == 0), 'dimension must be divisible by number of heads'
         self.topk = topk
         self.heads = heads
         self.num_keys = num_keys
 
-        dim_query = dim_head * heads
+        dim_query = dim_head * heads * 2
         self.to_queries = nn.Linear(dim, dim_query, bias = False)
-        self.norm = MaskedBatchNorm1D(nn.BatchNorm1d(dim_query)) if not use_evonorm else EvoNorm1D(dim_query, causal = causal)
 
-        self.keys = nn.Parameter(torch.zeros(heads, num_keys, 2, dim_head // 2))
-        self.values = nn.EmbeddingBag(num_keys ** 2, dim, mode='sum')
+        # batchnorm would break causality
+
+        self.use_layernorm = use_layernorm
+
+        if use_layernorm:
+            self.norm = nn.LayerNorm(dim_head)
+        else:
+            self.norm = MaskedBatchNorm1D(nn.BatchNorm1d(dim_head))
+
+        self.keys = nn.Parameter(torch.zeros(heads, num_keys, 2, dim_head))
+        self.values = nn.EmbeddingBag(num_keys ** 2, dim, mode = 'sum')
         init_(self.keys)
         init_(self.values.weight)
 
         self.input_dropout = nn.Dropout(input_dropout)
         self.query_dropout = nn.Dropout(query_dropout)
         self.value_dropout = nn.Dropout(value_dropout)
 
-    def forward(self, x, input_mask = None, **kwargs):
-        b, t, e, h = *x.shape, self.heads
+    def forward(
+        self,
+        x,
+        input_mask = None,
+        **kwargs
+    ):
+        b, t, h = *x.shape[:2], self.heads
         x = self.input_dropout(x)
 
         queries = self.to_queries(x)
-        queries = self.norm(queries, mask = input_mask)
+
+        # split out query heads
+
+        queries = rearrange(queries, 'b t (p h d) -> (b p h) t d', p = 2, h = h)
+
+        # norm and dropout queries
+
+        norm_kwargs = dict(mask = input_mask) if not self.use_layernorm else dict()
+        queries = self.norm(queries, **norm_kwargs)
         queries = self.query_dropout(queries)
 
-        queries = queries.chunk(2, dim=-1)
-        queries = torch.stack(queries).reshape(2, b, t, h, -1)
+        # ready queries
+
+        queries = rearrange(queries, '(b p h) t d -> p b t h d', p = 2, h = h)
+
+        # similarity to keys
 
-        dots = torch.einsum('pbthd,hnpd->bthpn', queries, self.keys)
-        scores, indices = dots.topk(k=self.topk, dim=-1)
-        scores, indices = map(lambda x: x.chunk(2, dim=3), (scores, indices))
+        dots = einsum('p b t h d, h n p d -> b t h p n', queries, self.keys)
+
+        # topk scores
+
+        scores, indices = dots.topk(k = self.topk, dim = -1)
+
+        (scores_x, scores_y), (indices_x, indices_y) = map(lambda t: t.chunk(2, dim = 3), (scores, indices))
 
         all_topk = self.topk ** 2
-        shape = (b, t, h, all_topk)
 
-        all_scores = (
-            scores[0][..., :, None] +
-            scores[1][..., None, :]
-        ).reshape(*shape)
-
-        all_indices = (
-            indices[0][..., :, None] * self.num_keys +
-            indices[1][..., None, :]
-        ).reshape(*shape)
+        all_scores = rearrange((
+            rearrange(scores_x, '... k -> ... k 1') +
+            rearrange(scores_y, '... k -> ... 1 k')
+        ), 'b t h ... -> b t h (...)')
+
+        all_indices = rearrange((
+            rearrange(indices_x, '... k -> ... k 1') * self.num_keys +
+            rearrange(indices_y, '... k -> ... 1 k')
+        ), 'b t h ... -> b t h (...)')
 
         final_topk, final_indices = all_scores.topk(self.topk, dim=-1)
         value_indices = all_indices.gather(-1, final_indices)
 
+        # attention
+
         attn = final_topk.softmax(dim=-1)
 
-        value_indices, attn = map(lambda x: x.reshape(-1, self.topk * h), (value_indices, attn))
+        value_indices, attn = map(lambda t: rearrange(t, 'b t h k -> (b t) (h k)'), (value_indices, attn))
+
+        # aggregate
 
         out = self.values(value_indices, per_sample_weights=attn)
         out = self.value_dropout(out)
-        return out.reshape(b, t, e)
 
+        return rearrange(out, '(b t) d -> b t d', b = b)
```

### Comparing `product_key_memory-0.1.9/PKG-INFO` & `product_key_memory-0.2.0/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,16 +1,16 @@
-Metadata-Version: 1.1
+Metadata-Version: 2.1
 Name: product_key_memory
-Version: 0.1.9
+Version: 0.2.0
 Summary: Product Key Memory
 Home-page: https://github.com/lucidrains/product-key-memory
 Author: Aran Komatsuzaki, Phil Wang
 Author-email: aran1234321@gmail.com, lucidrains@gmail.com
 License: MIT
-Description: UNKNOWN
 Keywords: transformers,artificial intelligence
-Platform: UNKNOWN
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Scientific/Engineering :: Artificial Intelligence
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3.6
+Description-Content-Type: text/markdown
+License-File: LICENSE
```

### Comparing `product_key_memory-0.1.9/product_key_memory.egg-info/PKG-INFO` & `product_key_memory-0.2.0/product_key_memory.egg-info/PKG-INFO`

 * *Files 24% similar despite different names*

```diff
@@ -1,16 +1,16 @@
-Metadata-Version: 1.1
+Metadata-Version: 2.1
 Name: product-key-memory
-Version: 0.1.9
+Version: 0.2.0
 Summary: Product Key Memory
 Home-page: https://github.com/lucidrains/product-key-memory
 Author: Aran Komatsuzaki, Phil Wang
 Author-email: aran1234321@gmail.com, lucidrains@gmail.com
 License: MIT
-Description: UNKNOWN
 Keywords: transformers,artificial intelligence
-Platform: UNKNOWN
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Scientific/Engineering :: Artificial Intelligence
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3.6
+Description-Content-Type: text/markdown
+License-File: LICENSE
```

### Comparing `product_key_memory-0.1.9/setup.py` & `product_key_memory-0.2.0/setup.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,23 +1,25 @@
 from setuptools import setup, find_packages
 
 setup(
-  name = 'product_key_memory',
-  packages = find_packages(),
-  version = '0.1.9',
-  license='MIT',
-  description = 'Product Key Memory',
-  author = 'Aran Komatsuzaki, Phil Wang',
-  author_email = 'aran1234321@gmail.com, lucidrains@gmail.com',
-  url = 'https://github.com/lucidrains/product-key-memory',
-  keywords = ['transformers', 'artificial intelligence'],
-  install_requires=[
-      'torch'
-  ],
-  classifiers=[
-      'Development Status :: 4 - Beta',
-      'Intended Audience :: Developers',
-      'Topic :: Scientific/Engineering :: Artificial Intelligence',
-      'License :: OSI Approved :: MIT License',
-      'Programming Language :: Python :: 3.6',
-  ],
-)
+    name = 'product_key_memory',
+    packages = find_packages(),
+    version = '0.2.0',
+    license='MIT',
+    description = 'Product Key Memory',
+    long_description_content_type = 'text/markdown',
+    author = 'Aran Komatsuzaki, Phil Wang',
+    author_email = 'aran1234321@gmail.com, lucidrains@gmail.com',
+    url = 'https://github.com/lucidrains/product-key-memory',
+    keywords = ['transformers', 'artificial intelligence'],
+    install_requires=[
+        'einops>=0.6',
+        'torch'
+    ],
+    classifiers=[
+        'Development Status :: 4 - Beta',
+        'Intended Audience :: Developers',
+        'Topic :: Scientific/Engineering :: Artificial Intelligence',
+        'License :: OSI Approved :: MIT License',
+        'Programming Language :: Python :: 3.6',
+    ],
+)
```

### Comparing `product_key_memory-0.1.9/README.md` & `product_key_memory-0.2.0/README.md`

 * *Files 5% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 ## Product Key Memory
 
 [![PyPI version](https://badge.fury.io/py/product-key-memory.svg)](https://badge.fury.io/py/product-key-memory)
 
-Standalone Product Key Memory module for augmenting Transformer models
+Standalone <a href="https://arxiv.org/abs/1907.05242">Product Key Memory</a> module for augmenting Transformer models
 
 ## Install
 
 ```bash
 $ pip install product-key-memory
 ```
 
@@ -19,16 +19,15 @@
 from product_key_memory import PKM
 
 pkm = PKM(
     dim = 512,
     heads = 4,
     dim_head = 256,       # keep at 256 for best results
     num_keys = 256,       # number of subkeys, # values will be num_keys ^ 2
-    topk = 32,            # the top number of subkeys to select
-    use_evonorm = True    # usually PKM requires decent batch sizes with batchnorm to work well. this is an experimental feature using the new evonorm-s0 for batch-independent normalization
+    topk = 32             # the top number of subkeys to select
 )
 
 x = torch.randn(1, 1024, 512)
 mask = torch.ones((1, 1024)).bool()
 values = pkm(x, input_mask = mask) # (1, 1024, 512)
 ```
 
@@ -79,8 +78,8 @@
 @misc{liu2020evolving,
     title   = {Evolving Normalization-Activation Layers},
     author  = {Hanxiao Liu and Andrew Brock and Karen Simonyan and Quoc V. Le},
     year    = {2020},
     eprint  = {2004.02967},
     archivePrefix = {arXiv}
 }
-```
+```
```

#### html2text {}

```diff
@@ -1,33 +1,30 @@
 ## Product Key Memory [![PyPI version](https://badge.fury.io/py/product-key-
 memory.svg)](https://badge.fury.io/py/product-key-memory) Standalone Product
-Key Memory module for augmenting Transformer models ## Install ```bash $ pip
+Key_Memory module for augmenting Transformer models ## Install ```bash $ pip
 install product-key-memory ``` ## Usage Replace the feedforwards in a
 Transformer with the following ```python import torch from product_key_memory
 import PKM pkm = PKM( dim = 512, heads = 4, dim_head = 256, # keep at 256 for
 best results num_keys = 256, # number of subkeys, # values will be num_keys ^ 2
-topk = 32, # the top number of subkeys to select use_evonorm = True # usually
-PKM requires decent batch sizes with batchnorm to work well. this is an
-experimental feature using the new evonorm-s0 for batch-independent
-normalization ) x = torch.randn(1, 1024, 512) mask = torch.ones((1, 1024)).bool
-() values = pkm(x, input_mask = mask) # (1, 1024, 512) ``` ## Learning Rates To
-give different learning rates to the value parameters of the product-key-memory
-network, use the following helper function. ```python from torch.optim import
-Adam from product_key_memory import fetch_pkm_value_parameters # this helper
-function, for your root model, finds all the PKM models and the embedding bag
-weight parameters pkm_parameters, other_parameters = fetch_pkm_value_parameters
-(model) optim = Adam([ {'params': other_parameters}, {'params': pkm_parameters,
-'lr': 1e-2} ], lr=1e-3) ``` Or, if product-key-memory parameters are the only
-other parameters you have a different learning rate for ```python from
-torch.optim import Adam from product_key_memory import
-fetch_optimizer_parameters parameters = fetch_optimizer_parameters(model) #
-automatically creates array of parameter settings with learning rate set at 1e-
-2 for pkm values optim = Adam(parameters, lr=1e-3) ``` ## Appreciation Special
-thanks go to Aran for encouraging me to look into this, and to Madison_May for
-his educational_blog_post, which helped me understand this better. ## Citations
-```bibtex @misc{lample2019large, title = {Large Memory Layers with Product
-Keys}, author = {Guillaume Lample and Alexandre Sablayrolles and Marc'Aurelio
-Ranzato and Ludovic Denoyer and HervÃ© JÃ©gou}, year = {2019}, eprint =
-{1907.05242}, archivePrefix = {arXiv} } ``` ```bibtex @misc{liu2020evolving,
-title = {Evolving Normalization-Activation Layers}, author = {Hanxiao Liu and
-Andrew Brock and Karen Simonyan and Quoc V. Le}, year = {2020}, eprint =
-{2004.02967}, archivePrefix = {arXiv} } ```
+topk = 32 # the top number of subkeys to select ) x = torch.randn(1, 1024, 512)
+mask = torch.ones((1, 1024)).bool() values = pkm(x, input_mask = mask) # (1,
+1024, 512) ``` ## Learning Rates To give different learning rates to the value
+parameters of the product-key-memory network, use the following helper
+function. ```python from torch.optim import Adam from product_key_memory import
+fetch_pkm_value_parameters # this helper function, for your root model, finds
+all the PKM models and the embedding bag weight parameters pkm_parameters,
+other_parameters = fetch_pkm_value_parameters(model) optim = Adam([ {'params':
+other_parameters}, {'params': pkm_parameters, 'lr': 1e-2} ], lr=1e-3) ``` Or,
+if product-key-memory parameters are the only other parameters you have a
+different learning rate for ```python from torch.optim import Adam from
+product_key_memory import fetch_optimizer_parameters parameters =
+fetch_optimizer_parameters(model) # automatically creates array of parameter
+settings with learning rate set at 1e-2 for pkm values optim = Adam(parameters,
+lr=1e-3) ``` ## Appreciation Special thanks go to Aran for encouraging me to
+look into this, and to Madison_May for his educational_blog_post, which helped
+me understand this better. ## Citations ```bibtex @misc{lample2019large, title
+= {Large Memory Layers with Product Keys}, author = {Guillaume Lample and
+Alexandre Sablayrolles and Marc'Aurelio Ranzato and Ludovic Denoyer and HervÃ©
+JÃ©gou}, year = {2019}, eprint = {1907.05242}, archivePrefix = {arXiv} } ```
+```bibtex @misc{liu2020evolving, title = {Evolving Normalization-Activation
+Layers}, author = {Hanxiao Liu and Andrew Brock and Karen Simonyan and Quoc V.
+Le}, year = {2020}, eprint = {2004.02967}, archivePrefix = {arXiv} } ```
```

