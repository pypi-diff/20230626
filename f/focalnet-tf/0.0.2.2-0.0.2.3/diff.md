# Comparing `tmp/focalnet-tf-0.0.2.2.tar.gz` & `tmp/focalnet-tf-0.0.2.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist\focalnet-tf-0.0.2.2.tar", last modified: Sun Jun 25 19:54:31 2023, max compression
+gzip compressed data, was "dist\focalnet-tf-0.0.2.3.tar", last modified: Mon Jun 26 18:45:04 2023, max compression
```

## Comparing `focalnet-tf-0.0.2.2.tar` & `focalnet-tf-0.0.2.3.tar`

### file list

```diff
@@ -1,24 +1,24 @@
-drwxrwxrwx   0        0        0        0 2023-06-25 19:54:31.000000 focalnet-tf-0.0.2.2/
--rw-rw-rw-   0        0        0     1086 2023-06-11 19:49:16.000000 focalnet-tf-0.0.2.2/LICENSE
--rw-rw-rw-   0        0        0     4290 2023-06-25 19:54:31.000000 focalnet-tf-0.0.2.2/PKG-INFO
--rw-rw-rw-   0        0        0     3727 2023-06-11 20:34:38.000000 focalnet-tf-0.0.2.2/README.md
-drwxrwxrwx   0        0        0        0 2023-06-25 19:54:31.000000 focalnet-tf-0.0.2.2/focalnet/
--rw-rw-rw-   0        0        0      195 2023-06-11 13:35:42.000000 focalnet-tf-0.0.2.2/focalnet/__init__.py
--rw-rw-rw-   0        0        0     1667 2023-06-11 22:12:59.000000 focalnet-tf-0.0.2.2/focalnet/download_weights.py
--rw-rw-rw-   0        0        0     2173 2023-06-25 00:23:28.000000 focalnet-tf-0.0.2.2/focalnet/drop.py
--rw-rw-rw-   0        0        0    22980 2023-06-25 19:54:10.000000 focalnet-tf-0.0.2.2/focalnet/focalnet.py
--rw-rw-rw-   0        0        0     5964 2023-06-18 21:54:05.000000 focalnet-tf-0.0.2.2/focalnet/focalnet_utils.py
--rw-rw-rw-   0        0        0    35363 2023-06-09 22:50:12.000000 focalnet-tf-0.0.2.2/focalnet/imagenet-1k.json
--rw-rw-rw-   0        0        0   872487 2023-06-10 00:38:09.000000 focalnet-tf-0.0.2.2/focalnet/imagenet-21k.json
--rw-rw-rw-   0        0        0   773963 2023-06-10 00:38:09.000000 focalnet-tf-0.0.2.2/focalnet/imagenet-22k-reorder.json
-drwxrwxrwx   0        0        0        0 2023-06-25 19:54:31.000000 focalnet-tf-0.0.2.2/focalnet_tf.egg-info/
--rw-rw-rw-   0        0        0     4290 2023-06-25 19:54:30.000000 focalnet-tf-0.0.2.2/focalnet_tf.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      454 2023-06-25 19:54:30.000000 focalnet-tf-0.0.2.2/focalnet_tf.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-25 19:54:30.000000 focalnet-tf-0.0.2.2/focalnet_tf.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       38 2023-06-25 19:54:30.000000 focalnet-tf-0.0.2.2/focalnet_tf.egg-info/requires.txt
--rw-rw-rw-   0        0        0        9 2023-06-25 19:54:30.000000 focalnet-tf-0.0.2.2/focalnet_tf.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-06-25 19:54:31.000000 focalnet-tf-0.0.2.2/setup.cfg
--rw-rw-rw-   0        0        0     1105 2023-06-18 18:44:10.000000 focalnet-tf-0.0.2.2/setup.py
-drwxrwxrwx   0        0        0        0 2023-06-25 19:54:31.000000 focalnet-tf-0.0.2.2/tests/
--rw-rw-rw-   0        0        0     7608 2023-06-11 20:50:45.000000 focalnet-tf-0.0.2.2/tests/test_focalnet.py
--rw-rw-rw-   0        0        0    15552 2023-06-18 22:23:12.000000 focalnet-tf-0.0.2.2/tests/test_reproductible.py
+drwxrwxrwx   0        0        0        0 2023-06-26 18:45:04.000000 focalnet-tf-0.0.2.3/
+-rw-rw-rw-   0        0        0     1086 2023-06-11 19:49:16.000000 focalnet-tf-0.0.2.3/LICENSE
+-rw-rw-rw-   0        0        0     4390 2023-06-26 18:45:04.000000 focalnet-tf-0.0.2.3/PKG-INFO
+-rw-rw-rw-   0        0        0     3827 2023-06-25 19:57:18.000000 focalnet-tf-0.0.2.3/README.md
+drwxrwxrwx   0        0        0        0 2023-06-26 18:45:04.000000 focalnet-tf-0.0.2.3/focalnet/
+-rw-rw-rw-   0        0        0      195 2023-06-11 13:35:42.000000 focalnet-tf-0.0.2.3/focalnet/__init__.py
+-rw-rw-rw-   0        0        0     1667 2023-06-11 22:12:59.000000 focalnet-tf-0.0.2.3/focalnet/download_weights.py
+-rw-rw-rw-   0        0        0     2173 2023-06-25 00:23:28.000000 focalnet-tf-0.0.2.3/focalnet/drop.py
+-rw-rw-rw-   0        0        0    22988 2023-06-26 17:13:39.000000 focalnet-tf-0.0.2.3/focalnet/focalnet.py
+-rw-rw-rw-   0        0        0     5956 2023-06-26 16:49:30.000000 focalnet-tf-0.0.2.3/focalnet/focalnet_utils.py
+-rw-rw-rw-   0        0        0    35363 2023-06-09 22:50:12.000000 focalnet-tf-0.0.2.3/focalnet/imagenet-1k.json
+-rw-rw-rw-   0        0        0   872487 2023-06-10 00:38:09.000000 focalnet-tf-0.0.2.3/focalnet/imagenet-21k.json
+-rw-rw-rw-   0        0        0   773963 2023-06-10 00:38:09.000000 focalnet-tf-0.0.2.3/focalnet/imagenet-22k-reorder.json
+drwxrwxrwx   0        0        0        0 2023-06-26 18:45:04.000000 focalnet-tf-0.0.2.3/focalnet_tf.egg-info/
+-rw-rw-rw-   0        0        0     4390 2023-06-26 18:45:04.000000 focalnet-tf-0.0.2.3/focalnet_tf.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      454 2023-06-26 18:45:04.000000 focalnet-tf-0.0.2.3/focalnet_tf.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-26 18:45:04.000000 focalnet-tf-0.0.2.3/focalnet_tf.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       38 2023-06-26 18:45:04.000000 focalnet-tf-0.0.2.3/focalnet_tf.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        9 2023-06-26 18:45:04.000000 focalnet-tf-0.0.2.3/focalnet_tf.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-06-26 18:45:04.000000 focalnet-tf-0.0.2.3/setup.cfg
+-rw-rw-rw-   0        0        0     1105 2023-06-26 18:44:26.000000 focalnet-tf-0.0.2.3/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-26 18:45:04.000000 focalnet-tf-0.0.2.3/tests/
+-rw-rw-rw-   0        0        0     7608 2023-06-11 20:50:45.000000 focalnet-tf-0.0.2.3/tests/test_focalnet.py
+-rw-rw-rw-   0        0        0    15552 2023-06-18 22:23:12.000000 focalnet-tf-0.0.2.3/tests/test_reproductible.py
```

### Comparing `focalnet-tf-0.0.2.2/LICENSE` & `focalnet-tf-0.0.2.3/LICENSE`

 * *Files identical despite different names*

### Comparing `focalnet-tf-0.0.2.2/PKG-INFO` & `focalnet-tf-0.0.2.3/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: focalnet-tf
-Version: 0.0.2.2
+Version: 0.0.2.3
 Summary: Re-implementation of FocalNet for tensorflow 2.X
 Home-page: https://github.com/Shiro-LK/focalnet-tf
 Download-URL: https://github.com/Shiro-LK/focalnet-tf.git
 Author: Shiro-LK
 Author-email: shirosaki94@gmail.com
 License: MIT License
 Keywords: focalnet,tensorflow
@@ -23,22 +23,22 @@
 * **Translation-Invariance**: It is performed for each target token with the context centered around it.
 * **Explicit input-dependency**: The *modulator* is computed by aggregating the short- and long-rage context from the input and then applied to the target token.
 * **Spatial- and channel-specific**: It first aggregates the context spatial-wise and then channel-wise, followed by an element-wise modulation.
 * **Decoupled feature granularity**: Query token preserves the invidual information at finest level, while coarser context is extracted surrounding it. They two are decoupled but connected through the modulation operation.
 * **Easy to implement**: We can implement both context aggregation and interaction in a very simple and light-weight way. It does not need softmax, multiple attention heads, feature map rolling or unfolding, etc.
 
 <p align="center">
-<img src="figures/focalnet-model.png" width=80% height=80% 
+<img src="https://github.com/Shiro-LK/focalnet-tf/blob/main/figures/focalnet-model.png" width=80% height=80% 
 class="center">
 </p>
 
 This repository aims to reproduce the results of the paper using TensorFlow 2.4.1 and provide a modular and easy-to-use implementation of focal modulation networks. The code is based on the official PyTorch implementation of the paper, which can be found on the offical repository [here](https://github.com/microsoft/FocalNet) . Only the classification part is implemented. Pretrained checkpoints have been converted on Tensorflow.
 
 <p align="center">
-<img src="figures/modulator.JPG" width=80% height=80% 
+<img src="https://github.com/Shiro-LK/focalnet-tf/blob/main/figures/modulator.JPG" width=80% height=80% 
 class="center">
 </p>
 
 # Installation
 
 > pip install focalnet-tf
```

### Comparing `focalnet-tf-0.0.2.2/README.md` & `focalnet-tf-0.0.2.3/README.md`

 * *Files 6% similar despite different names*

```diff
@@ -7,22 +7,22 @@
 * **Translation-Invariance**: It is performed for each target token with the context centered around it.
 * **Explicit input-dependency**: The *modulator* is computed by aggregating the short- and long-rage context from the input and then applied to the target token.
 * **Spatial- and channel-specific**: It first aggregates the context spatial-wise and then channel-wise, followed by an element-wise modulation.
 * **Decoupled feature granularity**: Query token preserves the invidual information at finest level, while coarser context is extracted surrounding it. They two are decoupled but connected through the modulation operation.
 * **Easy to implement**: We can implement both context aggregation and interaction in a very simple and light-weight way. It does not need softmax, multiple attention heads, feature map rolling or unfolding, etc.
 
 <p align="center">
-<img src="figures/focalnet-model.png" width=80% height=80% 
+<img src="https://github.com/Shiro-LK/focalnet-tf/blob/main/figures/focalnet-model.png" width=80% height=80% 
 class="center">
 </p>
 
 This repository aims to reproduce the results of the paper using TensorFlow 2.4.1 and provide a modular and easy-to-use implementation of focal modulation networks. The code is based on the official PyTorch implementation of the paper, which can be found on the offical repository [here](https://github.com/microsoft/FocalNet) . Only the classification part is implemented. Pretrained checkpoints have been converted on Tensorflow.
 
 <p align="center">
-<img src="figures/modulator.JPG" width=80% height=80% 
+<img src="https://github.com/Shiro-LK/focalnet-tf/blob/main/figures/modulator.JPG" width=80% height=80% 
 class="center">
 </p>
 
 # Installation
 
 > pip install focalnet-tf
```

### Comparing `focalnet-tf-0.0.2.2/focalnet/download_weights.py` & `focalnet-tf-0.0.2.3/focalnet/download_weights.py`

 * *Files identical despite different names*

### Comparing `focalnet-tf-0.0.2.2/focalnet/drop.py` & `focalnet-tf-0.0.2.3/focalnet/drop.py`

 * *Files identical despite different names*

### Comparing `focalnet-tf-0.0.2.2/focalnet/focalnet.py` & `focalnet-tf-0.0.2.3/focalnet/focalnet.py`

 * *Files 0% similar despite different names*

```diff
@@ -328,15 +328,15 @@
                 focal_level=focal_level,
                 focal_window=focal_window, 
                 use_layerscale=use_layerscale, 
                 layerscale_value=layerscale_value,
                 use_postln=use_postln, 
                 use_postln_in_modulation=use_postln_in_modulation, 
                 normalize_modulator=normalize_modulator, 
-                name =  f"focalnet_block_{i}"
+                name =  f"{name}/focalnet_block_{i}/"
             )
             for i in range(depth)] 
 
         if downsample is not None:
             self.downsample = downsample(
                 img_size=input_resolution, 
                 patch_size=2,
```

### Comparing `focalnet-tf-0.0.2.2/focalnet/focalnet_utils.py` & `focalnet-tf-0.0.2.3/focalnet/focalnet_utils.py`

 * *Files 1% similar despite different names*

```diff
@@ -65,15 +65,15 @@
     elif model_name == "focalnet_large_fl3":
         depths = [2, 2, 18, 2]
         embed_dim = 192
         focal_levels=[3, 3, 3, 3]
         focal_windows = [5, 5, 5, 5]
         use_conv_embed = True
         use_postln = True
-        use_layerscale =  True # False #
+        use_layerscale =   True 
         default_classes = 21842
     elif model_name == "focalnet_large_fl4":
         depths = [2, 2, 18, 2]
         embed_dim = 192
         focal_levels = [4, 4, 4, 4]
         focal_windows =[3, 3, 3, 3]
         use_conv_embed = True
```

### Comparing `focalnet-tf-0.0.2.2/focalnet/imagenet-1k.json` & `focalnet-tf-0.0.2.3/focalnet/imagenet-1k.json`

 * *Files identical despite different names*

### Comparing `focalnet-tf-0.0.2.2/focalnet/imagenet-21k.json` & `focalnet-tf-0.0.2.3/focalnet/imagenet-21k.json`

 * *Files identical despite different names*

### Comparing `focalnet-tf-0.0.2.2/focalnet/imagenet-22k-reorder.json` & `focalnet-tf-0.0.2.3/focalnet/imagenet-22k-reorder.json`

 * *Files identical despite different names*

### Comparing `focalnet-tf-0.0.2.2/focalnet_tf.egg-info/PKG-INFO` & `focalnet-tf-0.0.2.3/focalnet_tf.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: focalnet-tf
-Version: 0.0.2.2
+Version: 0.0.2.3
 Summary: Re-implementation of FocalNet for tensorflow 2.X
 Home-page: https://github.com/Shiro-LK/focalnet-tf
 Download-URL: https://github.com/Shiro-LK/focalnet-tf.git
 Author: Shiro-LK
 Author-email: shirosaki94@gmail.com
 License: MIT License
 Keywords: focalnet,tensorflow
@@ -23,22 +23,22 @@
 * **Translation-Invariance**: It is performed for each target token with the context centered around it.
 * **Explicit input-dependency**: The *modulator* is computed by aggregating the short- and long-rage context from the input and then applied to the target token.
 * **Spatial- and channel-specific**: It first aggregates the context spatial-wise and then channel-wise, followed by an element-wise modulation.
 * **Decoupled feature granularity**: Query token preserves the invidual information at finest level, while coarser context is extracted surrounding it. They two are decoupled but connected through the modulation operation.
 * **Easy to implement**: We can implement both context aggregation and interaction in a very simple and light-weight way. It does not need softmax, multiple attention heads, feature map rolling or unfolding, etc.
 
 <p align="center">
-<img src="figures/focalnet-model.png" width=80% height=80% 
+<img src="https://github.com/Shiro-LK/focalnet-tf/blob/main/figures/focalnet-model.png" width=80% height=80% 
 class="center">
 </p>
 
 This repository aims to reproduce the results of the paper using TensorFlow 2.4.1 and provide a modular and easy-to-use implementation of focal modulation networks. The code is based on the official PyTorch implementation of the paper, which can be found on the offical repository [here](https://github.com/microsoft/FocalNet) . Only the classification part is implemented. Pretrained checkpoints have been converted on Tensorflow.
 
 <p align="center">
-<img src="figures/modulator.JPG" width=80% height=80% 
+<img src="https://github.com/Shiro-LK/focalnet-tf/blob/main/figures/modulator.JPG" width=80% height=80% 
 class="center">
 </p>
 
 # Installation
 
 > pip install focalnet-tf
```

### Comparing `focalnet-tf-0.0.2.2/setup.py` & `focalnet-tf-0.0.2.3/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -6,15 +6,15 @@
     with open('README.md', encoding="utf-8-sig") as f:
         README = f.read()
     return README
 
 
 setup(
     name='focalnet-tf',
-    version='0.0.2.2',    
+    version='0.0.2.3',    
     description='Re-implementation of FocalNet for tensorflow 2.X',
     author='Shiro-LK',
     author_email='shirosaki94@gmail.com',
     license='MIT License',
     packages=['focalnet'],
     package_data={'focalnet': ['imagenet-1k.json', 'imagenet-21k.json', 'imagenet-22k-reorder.json']},
     long_description=readme(),
```

### Comparing `focalnet-tf-0.0.2.2/tests/test_focalnet.py` & `focalnet-tf-0.0.2.3/tests/test_focalnet.py`

 * *Files identical despite different names*

### Comparing `focalnet-tf-0.0.2.2/tests/test_reproductible.py` & `focalnet-tf-0.0.2.3/tests/test_reproductible.py`

 * *Files identical despite different names*

