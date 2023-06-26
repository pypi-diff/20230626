# Comparing `tmp/audiolm-pytorch-1.2.8.tar.gz` & `tmp/audiolm-pytorch-1.2.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "audiolm-pytorch-1.2.8.tar", last modified: Sun Jun 25 16:41:44 2023, max compression
+gzip compressed data, was "audiolm-pytorch-1.2.9.tar", last modified: Mon Jun 26 17:56:44 2023, max compression
```

## Comparing `audiolm-pytorch-1.2.8.tar` & `audiolm-pytorch-1.2.9.tar`

### file list

```diff
@@ -1,26 +1,26 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-25 16:41:44.662612 audiolm-pytorch-1.2.8/
--rw-r--r--   0 runner    (1001) docker     (123)     1066 2023-06-25 16:41:34.000000 audiolm-pytorch-1.2.8/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      698 2023-06-25 16:41:44.662612 audiolm-pytorch-1.2.8/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    18642 2023-06-25 16:41:34.000000 audiolm-pytorch-1.2.8/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-25 16:41:44.658612 audiolm-pytorch-1.2.8/audiolm_pytorch/
--rw-r--r--   0 runner    (1001) docker     (123)      932 2023-06-25 16:41:34.000000 audiolm-pytorch-1.2.8/audiolm_pytorch/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4172 2023-06-25 16:41:34.000000 audiolm-pytorch-1.2.8/audiolm_pytorch/attend.py
--rw-r--r--   0 runner    (1001) docker     (123)    68033 2023-06-25 16:41:34.000000 audiolm-pytorch-1.2.8/audiolm_pytorch/audiolm_pytorch.py
--rw-r--r--   0 runner    (1001) docker     (123)     4573 2023-06-25 16:41:34.000000 audiolm-pytorch-1.2.8/audiolm_pytorch/data.py
--rw-r--r--   0 runner    (1001) docker     (123)     7161 2023-06-25 16:41:34.000000 audiolm-pytorch-1.2.8/audiolm_pytorch/encodec.py
--rw-r--r--   0 runner    (1001) docker     (123)     2788 2023-06-25 16:41:34.000000 audiolm-pytorch-1.2.8/audiolm_pytorch/hubert_kmeans.py
--rw-r--r--   0 runner    (1001) docker     (123)     1119 2023-06-25 16:41:34.000000 audiolm-pytorch-1.2.8/audiolm_pytorch/optimizer.py
--rw-r--r--   0 runner    (1001) docker     (123)    30358 2023-06-25 16:41:34.000000 audiolm-pytorch-1.2.8/audiolm_pytorch/soundstream.py
--rw-r--r--   0 runner    (1001) docker     (123)     2548 2023-06-25 16:41:34.000000 audiolm-pytorch-1.2.8/audiolm_pytorch/t5.py
--rw-r--r--   0 runner    (1001) docker     (123)    42491 2023-06-25 16:41:34.000000 audiolm-pytorch-1.2.8/audiolm_pytorch/trainer.py
--rw-r--r--   0 runner    (1001) docker     (123)      454 2023-06-25 16:41:34.000000 audiolm-pytorch-1.2.8/audiolm_pytorch/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)       22 2023-06-25 16:41:34.000000 audiolm-pytorch-1.2.8/audiolm_pytorch/version.py
--rw-r--r--   0 runner    (1001) docker     (123)     2344 2023-06-25 16:41:34.000000 audiolm-pytorch-1.2.8/audiolm_pytorch/vq_wav2vec.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-25 16:41:44.658612 audiolm-pytorch-1.2.8/audiolm_pytorch.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      698 2023-06-25 16:41:44.000000 audiolm-pytorch-1.2.8/audiolm_pytorch.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      584 2023-06-25 16:41:44.000000 audiolm-pytorch-1.2.8/audiolm_pytorch.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-25 16:41:44.000000 audiolm-pytorch-1.2.8/audiolm_pytorch.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      220 2023-06-25 16:41:44.000000 audiolm-pytorch-1.2.8/audiolm_pytorch.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       16 2023-06-25 16:41:44.000000 audiolm-pytorch-1.2.8/audiolm_pytorch.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-25 16:41:44.662612 audiolm-pytorch-1.2.8/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1246 2023-06-25 16:41:34.000000 audiolm-pytorch-1.2.8/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 17:56:44.816538 audiolm-pytorch-1.2.9/
+-rw-r--r--   0 runner    (1001) docker     (123)     1066 2023-06-26 17:56:33.000000 audiolm-pytorch-1.2.9/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      698 2023-06-26 17:56:44.816538 audiolm-pytorch-1.2.9/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    18642 2023-06-26 17:56:33.000000 audiolm-pytorch-1.2.9/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 17:56:44.812538 audiolm-pytorch-1.2.9/audiolm_pytorch/
+-rw-r--r--   0 runner    (1001) docker     (123)      932 2023-06-26 17:56:33.000000 audiolm-pytorch-1.2.9/audiolm_pytorch/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4172 2023-06-26 17:56:33.000000 audiolm-pytorch-1.2.9/audiolm_pytorch/attend.py
+-rw-r--r--   0 runner    (1001) docker     (123)    68033 2023-06-26 17:56:33.000000 audiolm-pytorch-1.2.9/audiolm_pytorch/audiolm_pytorch.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4573 2023-06-26 17:56:33.000000 audiolm-pytorch-1.2.9/audiolm_pytorch/data.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7161 2023-06-26 17:56:33.000000 audiolm-pytorch-1.2.9/audiolm_pytorch/encodec.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2820 2023-06-26 17:56:33.000000 audiolm-pytorch-1.2.9/audiolm_pytorch/hubert_kmeans.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1119 2023-06-26 17:56:33.000000 audiolm-pytorch-1.2.9/audiolm_pytorch/optimizer.py
+-rw-r--r--   0 runner    (1001) docker     (123)    30358 2023-06-26 17:56:33.000000 audiolm-pytorch-1.2.9/audiolm_pytorch/soundstream.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2548 2023-06-26 17:56:33.000000 audiolm-pytorch-1.2.9/audiolm_pytorch/t5.py
+-rw-r--r--   0 runner    (1001) docker     (123)    42491 2023-06-26 17:56:33.000000 audiolm-pytorch-1.2.9/audiolm_pytorch/trainer.py
+-rw-r--r--   0 runner    (1001) docker     (123)      454 2023-06-26 17:56:33.000000 audiolm-pytorch-1.2.9/audiolm_pytorch/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)       22 2023-06-26 17:56:33.000000 audiolm-pytorch-1.2.9/audiolm_pytorch/version.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2344 2023-06-26 17:56:33.000000 audiolm-pytorch-1.2.9/audiolm_pytorch/vq_wav2vec.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 17:56:44.816538 audiolm-pytorch-1.2.9/audiolm_pytorch.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      698 2023-06-26 17:56:44.000000 audiolm-pytorch-1.2.9/audiolm_pytorch.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      584 2023-06-26 17:56:44.000000 audiolm-pytorch-1.2.9/audiolm_pytorch.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-26 17:56:44.000000 audiolm-pytorch-1.2.9/audiolm_pytorch.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      220 2023-06-26 17:56:44.000000 audiolm-pytorch-1.2.9/audiolm_pytorch.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       16 2023-06-26 17:56:44.000000 audiolm-pytorch-1.2.9/audiolm_pytorch.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-26 17:56:44.816538 audiolm-pytorch-1.2.9/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1246 2023-06-26 17:56:33.000000 audiolm-pytorch-1.2.9/setup.py
```

### Comparing `audiolm-pytorch-1.2.8/LICENSE` & `audiolm-pytorch-1.2.9/LICENSE`

 * *Files identical despite different names*

### Comparing `audiolm-pytorch-1.2.8/PKG-INFO` & `audiolm-pytorch-1.2.9/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: audiolm-pytorch
-Version: 1.2.8
+Version: 1.2.9
 Summary: AudioLM - Language Modeling Approach to Audio Generation from Google Research - Pytorch
 Home-page: https://github.com/lucidrains/audiolm-pytorch
 Author: Phil Wang
 Author-email: lucidrains@gmail.com
 License: MIT
 Keywords: artificial intelligence,deep learning,transformers,attention mechanism,audio generation
 Classifier: Development Status :: 4 - Beta
```

### Comparing `audiolm-pytorch-1.2.8/README.md` & `audiolm-pytorch-1.2.9/README.md`

 * *Files identical despite different names*

### Comparing `audiolm-pytorch-1.2.8/audiolm_pytorch/__init__.py` & `audiolm-pytorch-1.2.9/audiolm_pytorch/__init__.py`

 * *Files identical despite different names*

### Comparing `audiolm-pytorch-1.2.8/audiolm_pytorch/attend.py` & `audiolm-pytorch-1.2.9/audiolm_pytorch/attend.py`

 * *Files identical despite different names*

### Comparing `audiolm-pytorch-1.2.8/audiolm_pytorch/audiolm_pytorch.py` & `audiolm-pytorch-1.2.9/audiolm_pytorch/audiolm_pytorch.py`

 * *Files identical despite different names*

### Comparing `audiolm-pytorch-1.2.8/audiolm_pytorch/data.py` & `audiolm-pytorch-1.2.9/audiolm_pytorch/data.py`

 * *Files identical despite different names*

### Comparing `audiolm-pytorch-1.2.8/audiolm_pytorch/encodec.py` & `audiolm-pytorch-1.2.9/audiolm_pytorch/encodec.py`

 * *Files identical despite different names*

### Comparing `audiolm-pytorch-1.2.8/audiolm_pytorch/hubert_kmeans.py` & `audiolm-pytorch-1.2.9/audiolm_pytorch/hubert_kmeans.py`

 * *Files 2% similar despite different names*

```diff
@@ -93,12 +93,13 @@
 
         embed, packed_shape = pack([embed['x']], '* d')
 
         codebook_indices = self.kmeans.predict(embed.cpu().detach().numpy())
 
         codebook_indices = torch.from_numpy(codebook_indices).to(device).long()
 
+        codebook_indices, = unpack(codebook_indices, packed_shape, '*')
+
         if flatten:
             return codebook_indices
 
-        codebook_indices, = unpack(codebook_indices, packed_shape, '*')
-        return codebook_indices
+        return rearrange(codebook_indices, 'b ... -> b (...)')
```

### Comparing `audiolm-pytorch-1.2.8/audiolm_pytorch/optimizer.py` & `audiolm-pytorch-1.2.9/audiolm_pytorch/optimizer.py`

 * *Files identical despite different names*

### Comparing `audiolm-pytorch-1.2.8/audiolm_pytorch/soundstream.py` & `audiolm-pytorch-1.2.9/audiolm_pytorch/soundstream.py`

 * *Files identical despite different names*

### Comparing `audiolm-pytorch-1.2.8/audiolm_pytorch/t5.py` & `audiolm-pytorch-1.2.9/audiolm_pytorch/t5.py`

 * *Files identical despite different names*

### Comparing `audiolm-pytorch-1.2.8/audiolm_pytorch/trainer.py` & `audiolm-pytorch-1.2.9/audiolm_pytorch/trainer.py`

 * *Files identical despite different names*

### Comparing `audiolm-pytorch-1.2.8/audiolm_pytorch/vq_wav2vec.py` & `audiolm-pytorch-1.2.9/audiolm_pytorch/vq_wav2vec.py`

 * *Files identical despite different names*

### Comparing `audiolm-pytorch-1.2.8/audiolm_pytorch.egg-info/PKG-INFO` & `audiolm-pytorch-1.2.9/audiolm_pytorch.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: audiolm-pytorch
-Version: 1.2.8
+Version: 1.2.9
 Summary: AudioLM - Language Modeling Approach to Audio Generation from Google Research - Pytorch
 Home-page: https://github.com/lucidrains/audiolm-pytorch
 Author: Phil Wang
 Author-email: lucidrains@gmail.com
 License: MIT
 Keywords: artificial intelligence,deep learning,transformers,attention mechanism,audio generation
 Classifier: Development Status :: 4 - Beta
```

### Comparing `audiolm-pytorch-1.2.8/audiolm_pytorch.egg-info/SOURCES.txt` & `audiolm-pytorch-1.2.9/audiolm_pytorch.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `audiolm-pytorch-1.2.8/setup.py` & `audiolm-pytorch-1.2.9/setup.py`

 * *Files identical despite different names*

