# Comparing `tmp/spyx-0.0.8.tar.gz` & `tmp/spyx-0.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "spyx-0.0.8.tar", last modified: Sat Jun 24 16:27:19 2023, max compression
+gzip compressed data, was "spyx-0.0.9.tar", last modified: Sun Jun 25 09:02:32 2023, max compression
```

## Comparing `spyx-0.0.8.tar` & `spyx-0.0.9.tar`

### file list

```diff
@@ -1,21 +1,21 @@
-drwxrwxr-x   0 legion    (1000) legion    (1000)        0 2023-06-24 16:27:19.542202 spyx-0.0.8/
--rw-rw-r--   0 legion    (1000) legion    (1000)     1064 2023-06-21 21:10:32.000000 spyx-0.0.8/LICENSE
--rw-rw-r--   0 legion    (1000) legion    (1000)      760 2023-06-24 16:27:19.542202 spyx-0.0.8/PKG-INFO
--rw-rw-r--   0 legion    (1000) legion    (1000)     1374 2023-06-22 22:36:29.000000 spyx-0.0.8/README.md
--rw-rw-r--   0 legion    (1000) legion    (1000)       38 2023-06-24 16:27:19.542202 spyx-0.0.8/setup.cfg
--rw-rw-r--   0 legion    (1000) legion    (1000)     1384 2023-06-24 16:26:55.000000 spyx-0.0.8/setup.py
-drwxrwxr-x   0 legion    (1000) legion    (1000)        0 2023-06-24 16:27:19.542202 spyx-0.0.8/spyx/
--rw-rw-r--   0 legion    (1000) legion    (1000)      188 2023-06-22 10:53:53.000000 spyx-0.0.8/spyx/__init__.py
--rw-rw-r--   0 legion    (1000) legion    (1000)       21 2023-06-23 17:32:35.000000 spyx-0.0.8/spyx/_version.py
--rw-rw-r--   0 legion    (1000) legion    (1000)     8952 2023-06-23 07:55:56.000000 spyx-0.0.8/spyx/activation.py
--rw-rw-r--   0 legion    (1000) legion    (1000)    12388 2023-06-24 10:16:27.000000 spyx-0.0.8/spyx/data.py
--rw-rw-r--   0 legion    (1000) legion    (1000)     2707 2023-06-24 16:23:53.000000 spyx-0.0.8/spyx/loss.py
--rw-rw-r--   0 legion    (1000) legion    (1000)     8325 2023-06-24 16:22:34.000000 spyx-0.0.8/spyx/nn.py
-drwxrwxr-x   0 legion    (1000) legion    (1000)        0 2023-06-24 16:27:19.542202 spyx-0.0.8/spyx.egg-info/
--rw-rw-r--   0 legion    (1000) legion    (1000)      760 2023-06-24 16:27:19.000000 spyx-0.0.8/spyx.egg-info/PKG-INFO
--rw-rw-r--   0 legion    (1000) legion    (1000)      278 2023-06-24 16:27:19.000000 spyx-0.0.8/spyx.egg-info/SOURCES.txt
--rw-rw-r--   0 legion    (1000) legion    (1000)        1 2023-06-24 16:27:19.000000 spyx-0.0.8/spyx.egg-info/dependency_links.txt
--rw-rw-r--   0 legion    (1000) legion    (1000)       40 2023-06-24 16:27:19.000000 spyx-0.0.8/spyx.egg-info/requires.txt
--rw-rw-r--   0 legion    (1000) legion    (1000)        5 2023-06-24 16:27:19.000000 spyx-0.0.8/spyx.egg-info/top_level.txt
-drwxrwxr-x   0 legion    (1000) legion    (1000)        0 2023-06-24 16:27:19.542202 spyx-0.0.8/tests/
--rw-rw-r--   0 legion    (1000) legion    (1000)       85 2023-06-22 08:36:33.000000 spyx-0.0.8/tests/test_networks.py
+drwxrwxr-x   0 legion    (1000) legion    (1000)        0 2023-06-25 09:02:32.762703 spyx-0.0.9/
+-rw-rw-r--   0 legion    (1000) legion    (1000)     1064 2023-06-21 21:10:32.000000 spyx-0.0.9/LICENSE
+-rw-rw-r--   0 legion    (1000) legion    (1000)      760 2023-06-25 09:02:32.762703 spyx-0.0.9/PKG-INFO
+-rw-rw-r--   0 legion    (1000) legion    (1000)     1374 2023-06-22 22:36:29.000000 spyx-0.0.9/README.md
+-rw-rw-r--   0 legion    (1000) legion    (1000)       38 2023-06-25 09:02:32.762703 spyx-0.0.9/setup.cfg
+-rw-rw-r--   0 legion    (1000) legion    (1000)     1384 2023-06-25 09:00:27.000000 spyx-0.0.9/setup.py
+drwxrwxr-x   0 legion    (1000) legion    (1000)        0 2023-06-25 09:02:32.762703 spyx-0.0.9/spyx/
+-rw-rw-r--   0 legion    (1000) legion    (1000)      188 2023-06-22 10:53:53.000000 spyx-0.0.9/spyx/__init__.py
+-rw-rw-r--   0 legion    (1000) legion    (1000)       21 2023-06-23 17:32:35.000000 spyx-0.0.9/spyx/_version.py
+-rw-rw-r--   0 legion    (1000) legion    (1000)     8952 2023-06-23 07:55:56.000000 spyx-0.0.9/spyx/activation.py
+-rw-rw-r--   0 legion    (1000) legion    (1000)    12630 2023-06-25 08:47:58.000000 spyx-0.0.9/spyx/data.py
+-rw-rw-r--   0 legion    (1000) legion    (1000)     3349 2023-06-24 16:56:38.000000 spyx-0.0.9/spyx/loss.py
+-rw-rw-r--   0 legion    (1000) legion    (1000)     8298 2023-06-24 21:02:33.000000 spyx-0.0.9/spyx/nn.py
+drwxrwxr-x   0 legion    (1000) legion    (1000)        0 2023-06-25 09:02:32.762703 spyx-0.0.9/spyx.egg-info/
+-rw-rw-r--   0 legion    (1000) legion    (1000)      760 2023-06-25 09:02:32.000000 spyx-0.0.9/spyx.egg-info/PKG-INFO
+-rw-rw-r--   0 legion    (1000) legion    (1000)      278 2023-06-25 09:02:32.000000 spyx-0.0.9/spyx.egg-info/SOURCES.txt
+-rw-rw-r--   0 legion    (1000) legion    (1000)        1 2023-06-25 09:02:32.000000 spyx-0.0.9/spyx.egg-info/dependency_links.txt
+-rw-rw-r--   0 legion    (1000) legion    (1000)       40 2023-06-25 09:02:32.000000 spyx-0.0.9/spyx.egg-info/requires.txt
+-rw-rw-r--   0 legion    (1000) legion    (1000)        5 2023-06-25 09:02:32.000000 spyx-0.0.9/spyx.egg-info/top_level.txt
+drwxrwxr-x   0 legion    (1000) legion    (1000)        0 2023-06-25 09:02:32.762703 spyx-0.0.9/tests/
+-rw-rw-r--   0 legion    (1000) legion    (1000)       85 2023-06-22 08:36:33.000000 spyx-0.0.9/tests/test_networks.py
```

### Comparing `spyx-0.0.8/LICENSE` & `spyx-0.0.9/LICENSE`

 * *Files identical despite different names*

### Comparing `spyx-0.0.8/PKG-INFO` & `spyx-0.0.9/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: spyx
-Version: 0.0.8
+Version: 0.0.9
 Summary: Spyx: SNNs in JAX
 Home-page: https://github.com/kmheckel/spyx
 Author: Kade Heckel
 Author-email: example@email.com
 License: MIT
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `spyx-0.0.8/README.md` & `spyx-0.0.9/README.md`

 * *Files identical despite different names*

### Comparing `spyx-0.0.8/setup.py` & `spyx-0.0.9/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -20,15 +20,15 @@
         "numpy",
     ],
 )
 
 # This call to setup() does all the work
 setup(
     name="spyx",
-    version="0.0.8",
+    version="0.0.9",
     description="Spyx: SNNs in JAX",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/kmheckel/spyx",
     author="Kade Heckel",
     author_email="example@email.com",
     license="MIT",
```

### Comparing `spyx-0.0.8/spyx/activation.py` & `spyx-0.0.9/spyx/activation.py`

 * *Files identical despite different names*

### Comparing `spyx-0.0.8/spyx/data.py` & `spyx-0.0.9/spyx/data.py`

 * *Files 5% similar despite different names*

```diff
@@ -27,19 +27,19 @@
 class MNIST_loader():
     """
     Dataloader for the MNIST dataset, right now it is rate encoded.
     
     """
 
     # Change this to allow a config dictionary of 
-    def __init__(self, batch_size=32, val_size=0.3, key=0, download_dir='./MNIST'):
+    def __init__(self, time_steps=64, max_rate = 0.5, batch_size=32, val_size=0.3, key=0, download_dir='./MNIST'):
            
         self.key = jax.random.PRNGKey(key)
-        self.sample_T = 64
-        self.spike_rate = 0.7
+        self.sample_T = time_steps
+        self.max_rate = max_rate
         self.val_size = val_size
         self.batch_size = batch_size
         self.obs_shape = (28,28)
         self.act_shape = tuple([10,])
         
         transform = tv.transforms.Compose([
             tv.transforms.Resize(self.obs_shape),
@@ -83,35 +83,35 @@
         
     def train_reset(self):
         self.train_dl = iter(self._train_dl)
         
     def train_step(self):
         batch_data, batch_labels = next(self.train_dl)
         key, self.key = jax.random.split(self.key)
-        spike_data = jnp.expand_dims(rate_code(batch_data, self.sample_T, key), -1)
+        spike_data = jnp.expand_dims(rate_code(batch_data, self.sample_T, key, self.max_rate), -1)
         return State(obs=jnp.array(spike_data, dtype=jnp.int8), # perform cast to jnp.int8 here
                      labels=jnp.array(batch_labels))
     
     def val_reset(self):
         self.val_dl = iter(self._val_dl)
         
     def val_step(self):
         batch_data, batch_labels = next(self.val_dl)
         key, self.key = jax.random.split(self.key)
-        spike_data = jnp.expand_dims(rate_code(batch_data, self.sample_T, key), -1)
+        spike_data = jnp.expand_dims(rate_code(batch_data, self.sample_T, key, self.max_rate), -1)
         return State(obs=jnp.array(spike_data, dtype=jnp.int8), # perform cast to jnp.int8 here
                      labels=jnp.array(batch_labels))
         
     def test_reset(self):
         self.test_dl = iter(self._test_dl)
         
     def test_step(self):
         batch_data, batch_labels = next(self.test_dl)
         key, self.key = jax.random.split(self.key)
-        spike_data = jnp.expand_dims(rate_code(batch_data, self.sample_T, key), -1)
+        spike_data = jnp.expand_dims(rate_code(batch_data, self.sample_T, key, self.max_rate), -1)
         return State(obs=jnp.array(spike_data, dtype=jnp.int8), # perform cast to jnp.int8 here
                      labels=jnp.array(batch_labels))
 
 
 ###############################################
 
 class NMNIST_loader():
@@ -189,52 +189,55 @@
 
 ###########################################################
 
 # should push all of the transforms into here and make a single bin/frame func
 class SHD2Raster():
     """ Tool for rastering SHD samples into frames."""
 
-    def __init__(self, encoding_dim, sample_T = 100):
+    def __init__(self, encoding_dim, sample_T = 100, binarize=True):
         self.encoding_dim = encoding_dim
         self.sample_T = sample_T
+        self.binarize = binarize
         
     def __call__(self, events):
         # tensor has dimensions (time_steps, encoding_dim)
         tensor = np.zeros((events["t"].max()+1, self.encoding_dim), dtype=int)
         np.add.at(tensor, (events["t"], events["x"]), 1)
         #return tensor[:self.sample_T,:]
         tensor = tensor[:self.sample_T,:]
-        return np.minimum(tensor, 1)
+        if self.binarize:
+            tensor = np.minimum(tensor, 1)
+        return tensor
     
 
 class SHD_loader():
     """
     Dataloading wrapper for the Spiking Heidelberg Dataset.
 
     https://zenkelab.org/resources/spiking-heidelberg-datasets-shd/
     """
 
 
     # Change this to allow a config dictionary of 
-    def __init__(self, batch_size=128, sample_T = 100):        
+    def __init__(self, batch_size=128, sample_T = 100, channels=128, binarize=True):        
         shd_timestep = 1e-6
         shd_channels = 700
-        net_channels = 128
+        net_channels = channels
         net_dt = 10e-3
            
         self.batch_size = batch_size
         self.obs_shape = tuple([net_channels,])
         self.act_shape = tuple([20,])
         
         transform = transforms.Compose([
         transforms.Downsample(
             time_factor=shd_timestep / net_dt,
             spatial_factor=net_channels / shd_channels
             ),
-            SHD2Raster(net_channels, sample_T = sample_T)
+            SHD2Raster(net_channels, sample_T = sample_T, binarize=binarize)
         ])
         
         self.train_val_dataset = datasets.SHD("./data", train=True, transform=transform)
         test_dataset = datasets.SHD("./data", train=False, transform=transform)
         
         logo = LeaveOneGroupOut()
         self.logo = cycle(logo.split([*range(len(self.train_val_dataset))], groups=self.train_val_dataset.speaker))
```

### Comparing `spyx-0.0.8/spyx/loss.py` & `spyx-0.0.9/spyx/loss.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,21 +1,36 @@
 import jax
 import jax.numpy as jnp
 import optax
 
 # need to make these consistent...
 
 @jax.jit
-def mse_spike_count_reg(avg_spike_counts, target_count):
+def l2_spike_count_reg(avg_spike_counts, target_count):
     """Spike rate regularization based on mean squared error from target rate."""
 
     flat = jnp.concatenate(jax.tree_util.tree_flatten(avg_spike_counts)[0])
     return jnp.sum(optax.l2_loss(flat, jnp.array([target_count]*flat.shape[0])))
 
 @jax.jit
+def clipped_l2_spike_count_reg(avg_spike_counts, target_count, radius):
+    """
+    Spike rate regularization based on clipped mean squared error from target spike count.
+    
+    Attributes:
+        avg_spike_counts: array of average spikes per neuron over a batch.
+        target_count: the target number of spikes to be emitted by a neuron
+        radius: the tolerance +/- r from the target count where loss is clipped to zero
+    
+    """
+
+    flat = jnp.concatenate(jax.tree_util.tree_flatten(avg_spike_counts)[0])
+    return jnp.sum(jnp.maximum(0,optax.l2_loss(flat, jnp.array([target_count]*flat.shape[0]))/radius - radius))
+
+@jax.jit
 def inverse_spike_count_reg(avg_spike_counts, time_len):
     """
     Spike rate regularization based on an inverse function that strongly
     discourages neurons from silencing and gradually penalizes higher spike rates.
     
     """
```

### Comparing `spyx-0.0.8/spyx/nn.py` & `spyx-0.0.9/spyx/nn.py`

 * *Files 2% similar despite different names*

```diff
@@ -47,18 +47,15 @@
         T = gamma*T + (1-gamma)*spikes
         
         VT = jnp.concatenate([V,T], axis=-1, dtype=jnp.float16)
         return spikes, VT
     
     def initial_state(self, batch_size):
         return jnp.zeros([batch_size, self.hidden_size*2], dtype=jnp.float16)
-    
-
-        
-# allow for population encoding???
+         
 class LI(hk.RNNCore):
     """
     Leaky-Integrate (Non-spiking) neuron model.
 
     Attributes:
         layer_size: Number of output neurons from the previous linear layer.
 
@@ -137,14 +134,15 @@
         
         # numerical stability gremlin...
         beta = self.beta
         if not beta:
             beta = hk.get_parameter("b", [self.hidden_size], dtype=jnp.float16,
                                 init=hk.initializers.TruncatedNormal(0.25, 0.5))
             beta = jax.nn.hard_sigmoid(beta)
+            
         # calculate whether spike is generated, and update membrane potential
         spikes = self.act(V - self.threshold)
         V = (beta*V + x - spikes*self.threshold).astype(jnp.float16)
         
         return spikes, V
 
     def initial_state(self, batch_size): # figure out how to make dynamic...
```

### Comparing `spyx-0.0.8/spyx.egg-info/PKG-INFO` & `spyx-0.0.9/spyx.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: spyx
-Version: 0.0.8
+Version: 0.0.9
 Summary: Spyx: SNNs in JAX
 Home-page: https://github.com/kmheckel/spyx
 Author: Kade Heckel
 Author-email: example@email.com
 License: MIT
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
```

