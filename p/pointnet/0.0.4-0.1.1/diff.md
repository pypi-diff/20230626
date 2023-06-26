# Comparing `tmp/pointnet-0.0.4.tar.gz` & `tmp/pointnet-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pointnet-0.0.4.tar", last modified: Sun Jun 25 18:08:51 2023, max compression
+gzip compressed data, was "pointnet-0.1.1.tar", last modified: Mon Jun 26 19:36:36 2023, max compression
```

## Comparing `pointnet-0.0.4.tar` & `pointnet-0.1.1.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-25 18:08:51.720523 pointnet-0.0.4/
--rw-r--r--   0 runner    (1001) docker     (123)     1065 2023-06-25 18:08:42.000000 pointnet-0.0.4/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      551 2023-06-25 18:08:51.720523 pointnet-0.0.4/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     3468 2023-06-25 18:08:42.000000 pointnet-0.0.4/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-25 18:08:51.720523 pointnet-0.0.4/pointnet/
--rw-r--r--   0 runner    (1001) docker     (123)      212 2023-06-25 18:08:42.000000 pointnet-0.0.4/pointnet/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5841 2023-06-25 18:08:42.000000 pointnet-0.0.4/pointnet/pointnet.py
--rw-r--r--   0 runner    (1001) docker     (123)    17431 2023-06-25 18:08:42.000000 pointnet-0.0.4/pointnet/pointnet2.py
--rw-r--r--   0 runner    (1001) docker     (123)     1401 2023-06-25 18:08:42.000000 pointnet-0.0.4/pointnet/taichi.py
--rw-r--r--   0 runner    (1001) docker     (123)     1746 2023-06-25 18:08:42.000000 pointnet-0.0.4/pointnet/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-25 18:08:51.720523 pointnet-0.0.4/pointnet.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      551 2023-06-25 18:08:51.000000 pointnet-0.0.4/pointnet.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      299 2023-06-25 18:08:51.000000 pointnet-0.0.4/pointnet.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-25 18:08:51.000000 pointnet-0.0.4/pointnet.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       40 2023-06-25 18:08:51.000000 pointnet-0.0.4/pointnet.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        9 2023-06-25 18:08:51.000000 pointnet-0.0.4/pointnet.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-25 18:08:51.720523 pointnet-0.0.4/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      803 2023-06-25 18:08:42.000000 pointnet-0.0.4/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-25 18:08:51.720523 pointnet-0.0.4/test/
--rw-r--r--   0 runner    (1001) docker     (123)     1748 2023-06-25 18:08:42.000000 pointnet-0.0.4/test/test.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 19:36:36.859671 pointnet-0.1.1/
+-rw-r--r--   0 runner    (1001) docker     (123)     1065 2023-06-26 19:36:25.000000 pointnet-0.1.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      551 2023-06-26 19:36:36.859671 pointnet-0.1.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3617 2023-06-26 19:36:25.000000 pointnet-0.1.1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 19:36:36.859671 pointnet-0.1.1/pointnet/
+-rw-r--r--   0 runner    (1001) docker     (123)      231 2023-06-26 19:36:25.000000 pointnet-0.1.1/pointnet/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5841 2023-06-26 19:36:25.000000 pointnet-0.1.1/pointnet/pointnet.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17704 2023-06-26 19:36:25.000000 pointnet-0.1.1/pointnet/pointnet2.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1401 2023-06-26 19:36:25.000000 pointnet-0.1.1/pointnet/taichi.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1746 2023-06-26 19:36:25.000000 pointnet-0.1.1/pointnet/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 19:36:36.859671 pointnet-0.1.1/pointnet.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      551 2023-06-26 19:36:36.000000 pointnet-0.1.1/pointnet.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      299 2023-06-26 19:36:36.000000 pointnet-0.1.1/pointnet.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-26 19:36:36.000000 pointnet-0.1.1/pointnet.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       40 2023-06-26 19:36:36.000000 pointnet-0.1.1/pointnet.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        9 2023-06-26 19:36:36.000000 pointnet-0.1.1/pointnet.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-26 19:36:36.859671 pointnet-0.1.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      803 2023-06-26 19:36:25.000000 pointnet-0.1.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 19:36:36.859671 pointnet-0.1.1/test/
+-rw-r--r--   0 runner    (1001) docker     (123)     1748 2023-06-26 19:36:25.000000 pointnet-0.1.1/test/test.py
```

### Comparing `pointnet-0.0.4/LICENSE` & `pointnet-0.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `pointnet-0.0.4/PKG-INFO` & `pointnet-0.1.1/PKG-INFO`

 * *Files 25% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pointnet
-Version: 0.0.4
+Version: 0.1.1
 Summary: PointNet - Pytorch
 Home-page: https://github.com/kentechx/pointnet
 Author: Kaidi Shen
 License: MIT
 Keywords: 3D segmentation,3D classification,point cloud understanding
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
```

### Comparing `pointnet-0.0.4/README.md` & `pointnet-0.1.1/README.md`

 * *Files 8% similar despite different names*

```diff
@@ -58,44 +58,48 @@
 model = PointNetSeg(3, 40)
 x = torch.randn(16, 3, 1024)
 logits = model(x)
 ```
 
 ### PointNet2
 
-PointNet2 uses [taichi](https://github.com/taichi-dev/taichi) to accelerate the computation of ball query. You need to
-initialize taichi before using PointNet2.
-
-Perform classification with inputs xyz coordinates:
+Classification:
 
 ```python
 import torch
 from pointnet import PointNet2ClsSSG
 
-import taichi as ti
-
-ti.init(arch=ti.cuda)
-
-model = PointNet2ClsSSG(in_dim=3, out_dim=40).cuda()
-x = torch.randn(16, 3, 1024).cuda()
-xyz = x.clone()
-logits = model(x, xyz)
+model = PointNet2ClsSSG(in_dim=3, out_dim=40)
+x = torch.randn(16, 3, 1024)
+logits = model(x)
 ```
 
 Semantic segmentation:
 
 ```python
 import torch
 from pointnet import PointNet2SegSSG
 
-import taichi as ti
+model = PointNet2SegSSG(in_dim=3, out_dim=10)
+x = torch.randn(16, 3, 1024)
+xyz = x.clone()
+logits = model(x, xyz)
+```
+
+PointNet2 can use [taichi](https://github.com/taichi-dev/taichi) to accelerate the computation of ball query.
+If you are about to train on a single GPU, you can enable taichi by calling `enable_taichi()`.
 
-ti.init(arch=ti.cuda)
+Perform classification with inputs xyz coordinates:
 
-model = PointNet2SegSSG(in_dim=3, out_dim=40).cuda()
+```python
+import torch
+from pointnet import PointNet2ClsSSG, enable_taichi
+
+enable_taichi()
+model = PointNet2ClsSSG(in_dim=3, out_dim=40).cuda()
 x = torch.randn(16, 3, 1024).cuda()
 xyz = x.clone()
 logits = model(x, xyz)
 ```
 
 ## Performance
```

### Comparing `pointnet-0.0.4/pointnet/pointnet.py` & `pointnet-0.1.1/pointnet/pointnet.py`

 * *Files identical despite different names*

### Comparing `pointnet-0.0.4/pointnet/pointnet2.py` & `pointnet-0.1.1/pointnet/pointnet2.py`

 * *Files 0% similar despite different names*

```diff
@@ -2,18 +2,27 @@
 from typing import Union, Iterable
 
 import torch
 import torch.nn as nn
 import torch.nn.functional as F
 from einops import repeat, rearrange
 
-from .taichi import ball_query
-from .utils import farthest_point_sampling
+from .utils import farthest_point_sampling, ball_query_pytorch
 from .pointnet import STN
 
+# whether to use taichi for ball query
+TAICHI = False
+
+
+def enable_taichi():
+    import taichi as ti
+    global TAICHI
+    TAICHI = True
+    ti.init(ti.cuda)
+
 
 def exists(val):
     return val is not None
 
 
 def default(*vals):
     for val in vals:
@@ -21,15 +30,19 @@
             return val
 
 
 def _ball_query(src, query, radius, k):
     # conduct ball query on dim 1
     src = rearrange(src, 'b d n -> b n d')
     query = rearrange(query, 'b d m -> b m d')
-    return ball_query(src, query, radius, k)
+    if TAICHI:
+        from .taichi import ball_query
+        return ball_query(src, query, radius, k)
+    else:
+        return ball_query_pytorch(src, query, radius, k)
 
 
 def cdist(x, y=None):
     # perform cdist in dimension 1
     # x: (b, d, n)
     # y: (b, d, m)
     if exists(y):
```

### Comparing `pointnet-0.0.4/pointnet/taichi.py` & `pointnet-0.1.1/pointnet/taichi.py`

 * *Files identical despite different names*

### Comparing `pointnet-0.0.4/pointnet/utils.py` & `pointnet-0.1.1/pointnet/utils.py`

 * *Files identical despite different names*

### Comparing `pointnet-0.0.4/pointnet.egg-info/PKG-INFO` & `pointnet-0.1.1/pointnet.egg-info/PKG-INFO`

 * *Files 25% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pointnet
-Version: 0.0.4
+Version: 0.1.1
 Summary: PointNet - Pytorch
 Home-page: https://github.com/kentechx/pointnet
 Author: Kaidi Shen
 License: MIT
 Keywords: 3D segmentation,3D classification,point cloud understanding
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
```

### Comparing `pointnet-0.0.4/setup.py` & `pointnet-0.1.1/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 from setuptools import setup, find_packages
 
 setup(
     name='pointnet',
     packages=find_packages(),
-    version='0.0.4',
+    version='0.1.1',
     license='MIT',
     description='PointNet - Pytorch',
     author='Kaidi Shen',
     url='https://github.com/kentechx/pointnet',
     long_description_content_type='text/markdown',
     keywords=[
         '3D segmentation',
```

### Comparing `pointnet-0.0.4/test/test.py` & `pointnet-0.1.1/test/test.py`

 * *Files identical despite different names*

