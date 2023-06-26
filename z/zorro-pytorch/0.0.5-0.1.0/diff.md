# Comparing `tmp/zorro-pytorch-0.0.5.tar.gz` & `tmp/zorro-pytorch-0.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "zorro-pytorch-0.0.5.tar", last modified: Thu Feb 23 23:41:03 2023, max compression
+gzip compressed data, was "zorro-pytorch-0.1.0.tar", last modified: Mon Jun 26 21:34:53 2023, max compression
```

## Comparing `zorro-pytorch-0.0.5.tar` & `zorro-pytorch-0.1.0.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-23 23:41:03.059837 zorro-pytorch-0.0.5/
--rw-r--r--   0 runner    (1001) docker     (123)     1066 2023-02-23 23:40:51.000000 zorro-pytorch-0.0.5/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      623 2023-02-23 23:41:03.059837 zorro-pytorch-0.0.5/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2376 2023-02-23 23:40:51.000000 zorro-pytorch-0.0.5/README.md
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-02-23 23:41:03.059837 zorro-pytorch-0.0.5/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      858 2023-02-23 23:40:51.000000 zorro-pytorch-0.0.5/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-23 23:41:03.059837 zorro-pytorch-0.0.5/zorro_pytorch/
--rw-r--r--   0 runner    (1001) docker     (123)       58 2023-02-23 23:40:51.000000 zorro-pytorch-0.0.5/zorro_pytorch/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     9995 2023-02-23 23:40:51.000000 zorro-pytorch-0.0.5/zorro_pytorch/zorro_pytorch.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-23 23:41:03.059837 zorro-pytorch-0.0.5/zorro_pytorch.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      623 2023-02-23 23:41:03.000000 zorro-pytorch-0.0.5/zorro_pytorch.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      267 2023-02-23 23:41:03.000000 zorro-pytorch-0.0.5/zorro_pytorch.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-02-23 23:41:03.000000 zorro-pytorch-0.0.5/zorro_pytorch.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       43 2023-02-23 23:41:03.000000 zorro-pytorch-0.0.5/zorro_pytorch.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       14 2023-02-23 23:41:03.000000 zorro-pytorch-0.0.5/zorro_pytorch.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 21:34:53.702134 zorro-pytorch-0.1.0/
+-rw-r--r--   0 runner    (1001) docker     (123)     1066 2023-06-26 21:34:43.000000 zorro-pytorch-0.1.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      623 2023-06-26 21:34:53.702134 zorro-pytorch-0.1.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2394 2023-06-26 21:34:43.000000 zorro-pytorch-0.1.0/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-26 21:34:53.702134 zorro-pytorch-0.1.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      858 2023-06-26 21:34:43.000000 zorro-pytorch-0.1.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 21:34:53.698134 zorro-pytorch-0.1.0/zorro_pytorch/
+-rw-r--r--   0 runner    (1001) docker     (123)       58 2023-06-26 21:34:43.000000 zorro-pytorch-0.1.0/zorro_pytorch/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10061 2023-06-26 21:34:43.000000 zorro-pytorch-0.1.0/zorro_pytorch/zorro_pytorch.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 21:34:53.702134 zorro-pytorch-0.1.0/zorro_pytorch.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      623 2023-06-26 21:34:53.000000 zorro-pytorch-0.1.0/zorro_pytorch.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      267 2023-06-26 21:34:53.000000 zorro-pytorch-0.1.0/zorro_pytorch.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-26 21:34:53.000000 zorro-pytorch-0.1.0/zorro_pytorch.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       43 2023-06-26 21:34:53.000000 zorro-pytorch-0.1.0/zorro_pytorch.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       14 2023-06-26 21:34:53.000000 zorro-pytorch-0.1.0/zorro_pytorch.egg-info/top_level.txt
```

### Comparing `zorro-pytorch-0.0.5/LICENSE` & `zorro-pytorch-0.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `zorro-pytorch-0.0.5/PKG-INFO` & `zorro-pytorch-0.1.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: zorro-pytorch
-Version: 0.0.5
+Version: 0.1.0
 Summary: Zorro - Pytorch
 Home-page: https://github.com/lucidrains/zorro-pytorch
 Author: Phil Wang
 Author-email: lucidrains@gmail.com
 License: MIT
 Keywords: artificial intelligence,deep learning,transformers,attention mechanism,multimodal fusion
 Classifier: Development Status :: 4 - Beta
```

### Comparing `zorro-pytorch-0.0.5/README.md` & `zorro-pytorch-0.1.0/README.md`

 * *Files 5% similar despite different names*

```diff
@@ -31,14 +31,15 @@
     video_patch_size = 16,            # video patch size, can also be Tuple[int, int]
     video_temporal_patch_size = 2,    # video temporal patch size
     video_channels = 3,               # video channels
     return_token_types = (
         T.AUDIO,
         T.AUDIO,
         T.FUSION,
+        T.GLOBAL,
         T.VIDEO,
         T.VIDEO,
         T.VIDEO,
     ) # say you want to return 2 tokens for audio, 1 token for fusion, 3 for video - for whatever self-supervised learning, supervised learning, etc etc
 )
 
 video = torch.randn(2, 3, 8, 32, 32) # (batch, channels, time, height, width)
```

#### html2text {}

```diff
@@ -7,20 +7,21 @@
 zorro_pytorch import Zorro, TokenTypes as T model = Zorro( dim = 512, # model
 dimensions depth = 6, # depth dim_head = 64, # attention dimension heads heads
 = 8, # attention heads ff_mult = 4, # feedforward multiple num_fusion_tokens =
 16, # number of fusion tokens audio_patch_size = 16, # audio patch size, can
 also be Tuple[int, int] video_patch_size = 16, # video patch size, can also be
 Tuple[int, int] video_temporal_patch_size = 2, # video temporal patch size
 video_channels = 3, # video channels return_token_types = ( T.AUDIO, T.AUDIO,
-T.FUSION, T.VIDEO, T.VIDEO, T.VIDEO, ) # say you want to return 2 tokens for
-audio, 1 token for fusion, 3 for video - for whatever self-supervised learning,
-supervised learning, etc etc ) video = torch.randn(2, 3, 8, 32, 32) # (batch,
-channels, time, height, width) audio = torch.randn(2, 1024 * 10) # (batch,
-time) return_tokens = model(audio = audio, video = video) # (2, 6, 512) - all 6
-tokes as indicated above is returned # say you only want 1 audio and 1 video
-token, for contrastive learning audio_token, video_token = model(audio = audio,
-video = video, return_token_indices = (0, 3)).unbind(dim = -2) # (2, 512), (2,
-512) ``` ## Citations ```bibtex @inproceedings{Recasens2023ZorroTM, title =
-{Zorro: the masked multimodal transformer}, author = {Adri{\`a} Recasens and
-Jason Lin and Jo{\~a}o Carreira and Drew Jaegle and Luyu Wang and Jean-Baptiste
-Alayrac and Pauline Luc and Antoine Miech and Lucas Smaira and Ross Hemsley and
-Andrew Zisserman}, year = {2023} } ```
+T.FUSION, T.GLOBAL, T.VIDEO, T.VIDEO, T.VIDEO, ) # say you want to return 2
+tokens for audio, 1 token for fusion, 3 for video - for whatever self-
+supervised learning, supervised learning, etc etc ) video = torch.randn(2, 3,
+8, 32, 32) # (batch, channels, time, height, width) audio = torch.randn(2, 1024
+* 10) # (batch, time) return_tokens = model(audio = audio, video = video) # (2,
+6, 512) - all 6 tokes as indicated above is returned # say you only want 1
+audio and 1 video token, for contrastive learning audio_token, video_token =
+model(audio = audio, video = video, return_token_indices = (0, 3)).unbind(dim =
+-2) # (2, 512), (2, 512) ``` ## Citations ```bibtex @inproceedings
+{Recasens2023ZorroTM, title = {Zorro: the masked multimodal transformer},
+author = {Adri{\`a} Recasens and Jason Lin and Jo{\~a}o Carreira and Drew
+Jaegle and Luyu Wang and Jean-Baptiste Alayrac and Pauline Luc and Antoine
+Miech and Lucas Smaira and Ross Hemsley and Andrew Zisserman}, year = {2023} }
+```
```

### Comparing `zorro-pytorch-0.0.5/setup.py` & `zorro-pytorch-0.1.0/setup.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 from setuptools import setup, find_packages
 
 setup(
   name = 'zorro-pytorch',
   packages = find_packages(exclude=[]),
-  version = '0.0.5',
+  version = '0.1.0',
   license='MIT',
   description = 'Zorro - Pytorch',
   author = 'Phil Wang',
   author_email = 'lucidrains@gmail.com',
   long_description_content_type = 'text/markdown',
   url = 'https://github.com/lucidrains/zorro-pytorch',
   keywords = [
```

### Comparing `zorro-pytorch-0.0.5/zorro_pytorch/zorro_pytorch.py` & `zorro-pytorch-0.1.0/zorro_pytorch/zorro_pytorch.py`

 * *Files 2% similar despite different names*

```diff
@@ -16,14 +16,15 @@
 
 # constants
 
 class TokenTypes(Enum):
     AUDIO = 0
     VIDEO = 1
     FUSION = 2
+    GLOBAL = 3
 
 # functions
 
 def exists(val):
     return val is not None
 
 def default(*args):
@@ -282,18 +283,14 @@
 
         zorro_mask = token_types_attend_from == token_types_attend_to
 
         # fusion can attend to everything
 
         zorro_mask = zorro_mask | token_types_attend_from == TokenTypes.FUSION.value
 
-        # and both specific modalities like audio and video can attend to fusion
-
-        zorro_mask = zorro_mask | token_types_attend_to == TokenTypes.FUSION.value
-
         # attend and feedforward
 
         for attn, ff in self.layers:
             tokens = attn(tokens, attn_mask = zorro_mask) + tokens
             tokens = ff(tokens) + tokens
 
         tokens = self.norm(tokens)
@@ -310,11 +307,13 @@
             return_token_indices = torch.tensor(return_token_indices, dtype = torch.long, device = device)
 
             return_token_types_tensor = return_token_types_tensor[return_token_indices]
             return_tokens = return_tokens[return_token_indices]
 
         return_tokens = repeat(return_tokens, 'n d -> b n d', b = batch)
         pool_mask = rearrange(return_token_types_tensor, 'i -> i 1') == token_types_attend_to
+        # global queries can attend to all tokens
+        pool_mask = pool_mask | rearrange(return_token_types_tensor, 'i -> i 1') == torch.ones_like(token_types_attend_to, dtype=torch.long) * TokenTypes.GLOBAL.value
 
         pooled_tokens = self.attn_pool(return_tokens, context = tokens, attn_mask = pool_mask) + return_tokens
 
         return pooled_tokens
```

### Comparing `zorro-pytorch-0.0.5/zorro_pytorch.egg-info/PKG-INFO` & `zorro-pytorch-0.1.0/zorro_pytorch.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: zorro-pytorch
-Version: 0.0.5
+Version: 0.1.0
 Summary: Zorro - Pytorch
 Home-page: https://github.com/lucidrains/zorro-pytorch
 Author: Phil Wang
 Author-email: lucidrains@gmail.com
 License: MIT
 Keywords: artificial intelligence,deep learning,transformers,attention mechanism,multimodal fusion
 Classifier: Development Status :: 4 - Beta
```

