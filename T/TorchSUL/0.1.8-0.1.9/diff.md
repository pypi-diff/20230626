# Comparing `tmp/TorchSUL-0.1.8.tar.gz` & `tmp/TorchSUL-0.1.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist\TorchSUL-0.1.8.tar", last modified: Thu Feb 20 12:29:07 2020, max compression
+gzip compressed data, was "dist\TorchSUL-0.1.9.tar", last modified: Fri Feb 21 17:40:17 2020, max compression
```

## Comparing `TorchSUL-0.1.8.tar` & `TorchSUL-0.1.9.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxrwxrwx   0        0        0        0 2020-02-20 12:29:07.000000 TorchSUL-0.1.8/
--rw-rw-rw-   0        0        0      405 2020-02-20 12:29:07.000000 TorchSUL-0.1.8/PKG-INFO
--rw-rw-rw-   0        0        0       83 2020-01-31 08:23:29.000000 TorchSUL-0.1.8/README.md
--rw-rw-rw-   0        0        0       42 2020-02-20 12:29:07.000000 TorchSUL-0.1.8/setup.cfg
--rw-rw-rw-   0        0        0      559 2020-02-20 12:28:01.000000 TorchSUL-0.1.8/setup.py
-drwxrwxrwx   0        0        0        0 2020-02-20 12:29:07.000000 TorchSUL-0.1.8/TorchSUL/
--rw-rw-rw-   0        0        0     3031 2020-02-08 16:14:36.000000 TorchSUL-0.1.8/TorchSUL/DataReader.py
--rw-rw-rw-   0        0        0    16131 2020-02-20 12:04:14.000000 TorchSUL-0.1.8/TorchSUL/Layers.py
--rw-rw-rw-   0        0        0     8933 2020-02-20 12:03:44.000000 TorchSUL-0.1.8/TorchSUL/Model.py
--rw-rw-rw-   0        0        0     1552 2020-02-08 16:14:36.000000 TorchSUL-0.1.8/TorchSUL/sul_tool.py
--rw-rw-rw-   0        0        0      162 2020-02-08 14:57:10.000000 TorchSUL-0.1.8/TorchSUL/__init__.py
-drwxrwxrwx   0        0        0        0 2020-02-20 12:29:07.000000 TorchSUL-0.1.8/TorchSUL.egg-info/
--rw-rw-rw-   0        0        0        1 2020-02-20 12:29:07.000000 TorchSUL-0.1.8/TorchSUL.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      405 2020-02-20 12:29:07.000000 TorchSUL-0.1.8/TorchSUL.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      248 2020-02-20 12:29:07.000000 TorchSUL-0.1.8/TorchSUL.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        9 2020-02-20 12:29:07.000000 TorchSUL-0.1.8/TorchSUL.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2020-02-21 17:40:17.000000 TorchSUL-0.1.9/
+-rw-rw-rw-   0        0        0      405 2020-02-21 17:40:17.000000 TorchSUL-0.1.9/PKG-INFO
+-rw-rw-rw-   0        0        0       83 2020-02-03 04:58:11.000000 TorchSUL-0.1.9/README.md
+-rw-rw-rw-   0        0        0       42 2020-02-21 17:40:17.000000 TorchSUL-0.1.9/setup.cfg
+-rw-rw-rw-   0        0        0      559 2020-02-21 17:39:51.000000 TorchSUL-0.1.9/setup.py
+drwxrwxrwx   0        0        0        0 2020-02-21 17:40:17.000000 TorchSUL-0.1.9/TorchSUL/
+-rw-rw-rw-   0        0        0     3031 2020-02-06 08:20:11.000000 TorchSUL-0.1.9/TorchSUL/DataReader.py
+-rw-rw-rw-   0        0        0    16629 2020-02-20 17:33:41.000000 TorchSUL-0.1.9/TorchSUL/Layers.py
+-rw-rw-rw-   0        0        0     9515 2020-02-20 17:33:57.000000 TorchSUL-0.1.9/TorchSUL/Model.py
+-rw-rw-rw-   0        0        0     1552 2020-02-03 04:58:11.000000 TorchSUL-0.1.9/TorchSUL/sul_tool.py
+-rw-rw-rw-   0        0        0      162 2020-02-03 04:58:11.000000 TorchSUL-0.1.9/TorchSUL/__init__.py
+drwxrwxrwx   0        0        0        0 2020-02-21 17:40:17.000000 TorchSUL-0.1.9/TorchSUL.egg-info/
+-rw-rw-rw-   0        0        0        1 2020-02-21 17:40:16.000000 TorchSUL-0.1.9/TorchSUL.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      405 2020-02-21 17:40:16.000000 TorchSUL-0.1.9/TorchSUL.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      248 2020-02-21 17:40:16.000000 TorchSUL-0.1.9/TorchSUL.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        9 2020-02-21 17:40:16.000000 TorchSUL-0.1.9/TorchSUL.egg-info/top_level.txt
```

### Comparing `TorchSUL-0.1.8/setup.py` & `TorchSUL-0.1.9/setup.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from setuptools import setup, find_packages 
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 setup_args = dict(
     name='TorchSUL',
-    version='0.1.8',
+    version='0.1.9',
     description='Simple but useful layers for Pytorch',
     packages=find_packages(),
     long_description=long_description,
     long_description_content_type="text/markdown",
     author='Cheng Yu',
     author_email='chengyu996@gmail.com',
     url='https://github.com/ddddwee1/TorchSUL',
```

### Comparing `TorchSUL-0.1.8/TorchSUL/DataReader.py` & `TorchSUL-0.1.9/TorchSUL/DataReader.py`

 * *Files identical despite different names*

### Comparing `TorchSUL-0.1.8/TorchSUL/Layers.py` & `TorchSUL-0.1.9/TorchSUL/Layers.py`

 * *Files 2% similar despite different names*

```diff
@@ -3,14 +3,15 @@
 import torch.nn.functional as F 
 import torch.nn.init as init 
 from torch.nn.parameter import Parameter
 import math 
 
 record_params = []
 
+
 def _resnet_normal(tensor):
 	fan_in, fan_out = init._calculate_fan_in_and_fan_out(tensor)
 	std = math.sqrt(2.0 / float(fan_out))
 	return init._no_grad_normal_(tensor, 0., std)
 
 class Model(nn.Module):
 	def __init__(self, *args, **kwargs):
@@ -288,14 +289,18 @@
 			weight = self.weight
 		return F.linear(x, weight, self.bias)
 
 def flatten(x):
 	x = x.view(x.size(0), -1)
 	return x 
 
+class Flatten(Model):
+	def forward(self, x):
+		return flatten(x)
+
 class MaxPool2d(Model):
 	def initialize(self, size, stride=1, pad='SAME_LEFT', dilation_rate=1):
 		self.size = size
 		self.stride = stride
 		self.pad = pad
 		self.dilation_rate = dilation_rate
 
@@ -431,28 +436,45 @@
 	# 		state_dict, prefix, local_metadata, strict,
 	# 		missing_keys, unexpected_keys, error_msgs)
 
 def GlobalAvgPool2D(x):
 	x = x.mean(dim=(2,3), keepdim=True)
 	return x 
 
+class GlobalAvgPool2DLayer(Model):
+	def forward(self, x):
+		return GlobalAvgPool2D(x)
+
 def activation(x, act, **kwargs):
 	if act==-1:
 		return x
 	elif act==0:
 		return F.relu(x)
 	elif act==1:
 		return F.leaky_relu(x, negative_slope=0.2)
 	elif act==2:
 		return F.elu(x)
 	elif act==3:
 		return F.tanh(x)
 	elif act==6:
 		return torch.sigmoid(x)
 
+class Activation(Model):
+	def initialize(self, act):
+		self.act = act 
+		if act==8:
+			self.act = torch.nn.PReLU(num_parameters=outchn)
+		elif act==9:
+			self.act = torch.nn.PReLU(num_parameters=1)
+	def forward(self, x):
+		if self.act==8 or self.act==9:
+			return self.act(x)
+		else:
+			return activation(x, self.act)
+
 class graphConvLayer(Model):
 	def __init__(self, outsize, adj_mtx=None, adj_fn=None, values=None, usebias=True):
 		assert (adj_mtx is None) ^ (adj_fn is None), 'Assign either adj_mtx or adj_fn' 
 		self.outsize = outsize
 		self.adj_mtx = adj_mtx
 		self.adj_fn = adj_fn
 		self.values = values
@@ -499,8 +521,9 @@
 				self.adj_mtx = self._normalize_adj_mtx(self.adj_mtx)
 				self.normalized = True
 		else:
 			A = self.adj_fn(x)
 		res = torch.mm(A, x)
 		res = F.linear(res, self.weight, self.bias)
 		return res 
-		
+	
+
```

### Comparing `TorchSUL-0.1.8/TorchSUL/Model.py` & `TorchSUL-0.1.9/TorchSUL/Model.py`

 * *Files 6% similar despite different names*

```diff
@@ -4,15 +4,17 @@
 import torch.nn as nn 
 import torch.nn.functional as F 
 import os 
 
 Model = L.Model
 activation = L.activation
 flatten = L.flatten
+Flatten = L.Flatten
 GlobalAvgPool = L.GlobalAvgPool2D
+GlobalAvgPoolLayer = L.GlobalAvgPool2DLayer
 BatchNorm = L.BatchNorm
 MaxPool2D = L.MaxPool2d
 AvgPool2D = L.AvgPool2d
 
 # activation const
 PARAM_RELU = 0
 PARAM_LRELU = 1
@@ -21,14 +23,27 @@
 PARAM_MFM = 4
 PARAM_MFM_FC = 5
 PARAM_SIGMOID = 6
 PARAM_SWISH = 7
 PARAM_PRELU = 8
 PARAM_PRELU1 = 9
 
+def init_caffe_input(x):
+	global caffe_string, layer_counter
+	if not 'caffe_string' in globals():
+		caffe_string = ''
+	if not 'layer_counter' in globals():
+		layer_counter = 0
+	caffe_string += 'layer{\n'
+	caffe_string += ' name: "%s"\n'%x[1]()
+	caffe_string += ' type: "Input"\n'
+	caffe_string += ' top: "%s"\n'%x[1]()
+	caffe_string += ' input_param{\n  shape{\n   dim:%d\n   dim:%d\n   dim:%d\n   dim:%d\n  }\n }\n}\n'%(x[0].shape[0], x[0].shape[3], x[0].shape[1], x[0].shape[2])
+	layer_counter += 1 
+
 class Saver():
 	def __init__(self, module):
 		self.model = module
 
 	def _get_checkpoint(self, path):
 		path = path.replace('\\','/')
 		ckpt = path + 'checkpoint'
```

### Comparing `TorchSUL-0.1.8/TorchSUL/sul_tool.py` & `TorchSUL-0.1.9/TorchSUL/sul_tool.py`

 * *Files identical despite different names*

