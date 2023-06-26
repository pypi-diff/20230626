# Comparing `tmp/product_key_memory-0.2.0.tar.gz` & `tmp/product_key_memory-0.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "product_key_memory-0.2.0.tar", last modified: Mon Jun 26 15:19:23 2023, max compression
+gzip compressed data, was "product_key_memory-0.2.1.tar", last modified: Mon Jun 26 18:22:01 2023, max compression
```

## Comparing `product_key_memory-0.2.0.tar` & `product_key_memory-0.2.1.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 15:19:23.398293 product_key_memory-0.2.0/
--rw-r--r--   0 runner    (1001) docker     (123)     1066 2023-06-26 15:19:09.000000 product_key_memory-0.2.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      625 2023-06-26 15:19:23.398293 product_key_memory-0.2.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2635 2023-06-26 15:19:09.000000 product_key_memory-0.2.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 15:19:23.398293 product_key_memory-0.2.0/product_key_memory/
--rw-r--r--   0 runner    (1001) docker     (123)      110 2023-06-26 15:19:09.000000 product_key_memory-0.2.0/product_key_memory/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4244 2023-06-26 15:19:09.000000 product_key_memory-0.2.0/product_key_memory/product_key_memory.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 15:19:23.398293 product_key_memory-0.2.0/product_key_memory.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      625 2023-06-26 15:19:23.000000 product_key_memory-0.2.0/product_key_memory.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      307 2023-06-26 15:19:23.000000 product_key_memory-0.2.0/product_key_memory.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-26 15:19:23.000000 product_key_memory-0.2.0/product_key_memory.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       18 2023-06-26 15:19:23.000000 product_key_memory-0.2.0/product_key_memory.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       19 2023-06-26 15:19:23.000000 product_key_memory-0.2.0/product_key_memory.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-26 15:19:23.398293 product_key_memory-0.2.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      834 2023-06-26 15:19:09.000000 product_key_memory-0.2.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 18:22:01.057201 product_key_memory-0.2.1/
+-rw-r--r--   0 runner    (1001) docker     (123)     1066 2023-06-26 18:21:51.000000 product_key_memory-0.2.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      625 2023-06-26 18:22:01.057201 product_key_memory-0.2.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2635 2023-06-26 18:21:51.000000 product_key_memory-0.2.1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 18:22:01.057201 product_key_memory-0.2.1/product_key_memory/
+-rw-r--r--   0 runner    (1001) docker     (123)      110 2023-06-26 18:21:51.000000 product_key_memory-0.2.1/product_key_memory/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4427 2023-06-26 18:21:51.000000 product_key_memory-0.2.1/product_key_memory/product_key_memory.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 18:22:01.057201 product_key_memory-0.2.1/product_key_memory.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      625 2023-06-26 18:22:01.000000 product_key_memory-0.2.1/product_key_memory.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      307 2023-06-26 18:22:01.000000 product_key_memory-0.2.1/product_key_memory.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-26 18:22:01.000000 product_key_memory-0.2.1/product_key_memory.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       18 2023-06-26 18:22:01.000000 product_key_memory-0.2.1/product_key_memory.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       19 2023-06-26 18:22:01.000000 product_key_memory-0.2.1/product_key_memory.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-26 18:22:01.057201 product_key_memory-0.2.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      834 2023-06-26 18:21:51.000000 product_key_memory-0.2.1/setup.py
```

### Comparing `product_key_memory-0.2.0/LICENSE` & `product_key_memory-0.2.1/LICENSE`

 * *Files identical despite different names*

### Comparing `product_key_memory-0.2.0/PKG-INFO` & `product_key_memory-0.2.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: product_key_memory
-Version: 0.2.0
+Version: 0.2.1
 Summary: Product Key Memory
 Home-page: https://github.com/lucidrains/product-key-memory
 Author: Aran Komatsuzaki, Phil Wang
 Author-email: aran1234321@gmail.com, lucidrains@gmail.com
 License: MIT
 Keywords: transformers,artificial intelligence
 Classifier: Development Status :: 4 - Beta
```

### Comparing `product_key_memory-0.2.0/README.md` & `product_key_memory-0.2.1/README.md`

 * *Files identical despite different names*

### Comparing `product_key_memory-0.2.0/product_key_memory/product_key_memory.py` & `product_key_memory-0.2.1/product_key_memory/product_key_memory.py`

 * *Files 2% similar despite different names*

```diff
@@ -67,24 +67,29 @@
         heads = 4,
         num_keys = 128,
         topk = 32,
         dim_head = 128,
         input_dropout = 0.,
         query_dropout = 0.,
         value_dropout = 0.,
-        use_layernorm = False
+        use_layernorm = False,
+        pre_layernorm = False
     ):
         super().__init__()
         self.topk = topk
         self.heads = heads
         self.num_keys = num_keys
 
         dim_query = dim_head * heads * 2
         self.to_queries = nn.Linear(dim, dim_query, bias = False)
 
+        # pre-layernorm pattern
+
+        self.pre_layernorm = nn.LayerNorm(dim) if pre_layernorm else nn.Identity()
+
         # batchnorm would break causality
 
         self.use_layernorm = use_layernorm
 
         if use_layernorm:
             self.norm = nn.LayerNorm(dim_head)
         else:
@@ -102,14 +107,16 @@
     def forward(
         self,
         x,
         input_mask = None,
         **kwargs
     ):
         b, t, h = *x.shape[:2], self.heads
+
+        x = self.pre_layernorm(x)
         x = self.input_dropout(x)
 
         queries = self.to_queries(x)
 
         # split out query heads
 
         queries = rearrange(queries, 'b t (p h d) -> (b p h) t d', p = 2, h = h)
```

### Comparing `product_key_memory-0.2.0/product_key_memory.egg-info/PKG-INFO` & `product_key_memory-0.2.1/product_key_memory.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: product-key-memory
-Version: 0.2.0
+Version: 0.2.1
 Summary: Product Key Memory
 Home-page: https://github.com/lucidrains/product-key-memory
 Author: Aran Komatsuzaki, Phil Wang
 Author-email: aran1234321@gmail.com, lucidrains@gmail.com
 License: MIT
 Keywords: transformers,artificial intelligence
 Classifier: Development Status :: 4 - Beta
```

### Comparing `product_key_memory-0.2.0/setup.py` & `product_key_memory-0.2.1/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 from setuptools import setup, find_packages
 
 setup(
     name = 'product_key_memory',
     packages = find_packages(),
-    version = '0.2.0',
+    version = '0.2.1',
     license='MIT',
     description = 'Product Key Memory',
     long_description_content_type = 'text/markdown',
     author = 'Aran Komatsuzaki, Phil Wang',
     author_email = 'aran1234321@gmail.com, lucidrains@gmail.com',
     url = 'https://github.com/lucidrains/product-key-memory',
     keywords = ['transformers', 'artificial intelligence'],
```

