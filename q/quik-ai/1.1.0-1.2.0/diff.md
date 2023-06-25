# Comparing `tmp/quik-ai-1.1.0.tar.gz` & `tmp/quik-ai-1.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "quik-ai-1.1.0.tar", last modified: Mon Jun 12 22:25:55 2023, max compression
+gzip compressed data, was "quik-ai-1.2.0.tar", last modified: Sat Jun 24 20:57:06 2023, max compression
```

## Comparing `quik-ai-1.1.0.tar` & `quik-ai-1.2.0.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxrwxrwx   0        0        0        0 2023-06-12 22:25:55.003455 quik-ai-1.1.0/
--rw-rw-rw-   0        0        0    11554 2023-06-07 20:40:55.000000 quik-ai-1.1.0/LICENSE
--rw-rw-rw-   0        0        0     2235 2023-06-12 22:25:55.004459 quik-ai-1.1.0/PKG-INFO
--rw-rw-rw-   0        0        0     1697 2023-06-11 13:33:07.000000 quik-ai-1.1.0/README.md
--rw-rw-rw-   0        0        0       97 2023-05-29 14:14:26.000000 quik-ai-1.1.0/pyproject.toml
--rw-rw-rw-   0        0        0      768 2023-06-12 22:25:55.007446 quik-ai-1.1.0/setup.cfg
--rw-rw-rw-   0        0        0      289 2023-06-09 23:06:08.000000 quik-ai-1.1.0/setup.py
-drwxrwxrwx   0        0        0        0 2023-06-12 22:25:54.856707 quik-ai-1.1.0/src/
-drwxrwxrwx   0        0        0        0 2023-06-12 22:25:54.972538 quik-ai-1.1.0/src/quik_ai/
--rw-rw-rw-   0        0        0      429 2023-06-09 00:21:28.000000 quik-ai-1.1.0/src/quik_ai/__init__.py
--rw-rw-rw-   0        0        0     2440 2023-06-11 23:04:01.000000 quik-ai-1.1.0/src/quik_ai/backend.py
--rw-rw-rw-   0        0        0    11500 2023-06-12 22:23:55.000000 quik-ai-1.1.0/src/quik_ai/engine.py
--rw-rw-rw-   0        0        0     4917 2023-06-07 22:39:50.000000 quik-ai-1.1.0/src/quik_ai/heads.py
--rw-rw-rw-   0        0        0    18541 2023-06-08 20:45:11.000000 quik-ai-1.1.0/src/quik_ai/layers.py
--rw-rw-rw-   0        0        0      940 2023-06-07 22:39:39.000000 quik-ai-1.1.0/src/quik_ai/losses.py
--rw-rw-rw-   0        0        0     1291 2023-06-10 01:46:43.000000 quik-ai-1.1.0/src/quik_ai/metrics.py
--rw-rw-rw-   0        0        0    29800 2023-06-12 22:25:24.000000 quik-ai-1.1.0/src/quik_ai/models.py
--rw-rw-rw-   0        0        0     1633 2023-06-06 23:57:01.000000 quik-ai-1.1.0/src/quik_ai/optimizers.py
--rw-rw-rw-   0        0        0     8255 2023-06-12 21:22:26.000000 quik-ai-1.1.0/src/quik_ai/predictors.py
--rw-rw-rw-   0        0        0     9621 2023-06-08 21:13:03.000000 quik-ai-1.1.0/src/quik_ai/tuners.py
--rw-rw-rw-   0        0        0     3344 2023-06-10 16:18:42.000000 quik-ai-1.1.0/src/quik_ai/tuning.py
-drwxrwxrwx   0        0        0        0 2023-06-12 22:25:55.001459 quik-ai-1.1.0/src/quik_ai.egg-info/
--rw-rw-rw-   0        0        0     2235 2023-06-12 22:25:54.000000 quik-ai-1.1.0/src/quik_ai.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      500 2023-06-12 22:25:54.000000 quik-ai-1.1.0/src/quik_ai.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-12 22:25:54.000000 quik-ai-1.1.0/src/quik_ai.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      109 2023-06-12 22:25:54.000000 quik-ai-1.1.0/src/quik_ai.egg-info/requires.txt
--rw-rw-rw-   0        0        0        8 2023-06-12 22:25:54.000000 quik-ai-1.1.0/src/quik_ai.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-06-24 20:57:06.144433 quik-ai-1.2.0/
+-rw-rw-rw-   0        0        0    11554 2023-06-07 20:40:55.000000 quik-ai-1.2.0/LICENSE
+-rw-rw-rw-   0        0        0     2235 2023-06-24 20:57:06.144433 quik-ai-1.2.0/PKG-INFO
+-rw-rw-rw-   0        0        0     1697 2023-06-11 13:33:07.000000 quik-ai-1.2.0/README.md
+-rw-rw-rw-   0        0        0       97 2023-05-29 14:14:26.000000 quik-ai-1.2.0/pyproject.toml
+-rw-rw-rw-   0        0        0      768 2023-06-24 20:57:06.147425 quik-ai-1.2.0/setup.cfg
+-rw-rw-rw-   0        0        0      289 2023-06-09 23:06:08.000000 quik-ai-1.2.0/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-24 20:57:06.028822 quik-ai-1.2.0/src/
+drwxrwxrwx   0        0        0        0 2023-06-24 20:57:06.114509 quik-ai-1.2.0/src/quik_ai/
+-rw-rw-rw-   0        0        0      429 2023-06-09 00:21:28.000000 quik-ai-1.2.0/src/quik_ai/__init__.py
+-rw-rw-rw-   0        0        0     2440 2023-06-11 23:04:01.000000 quik-ai-1.2.0/src/quik_ai/backend.py
+-rw-rw-rw-   0        0        0    13147 2023-06-24 13:52:15.000000 quik-ai-1.2.0/src/quik_ai/engine.py
+-rw-rw-rw-   0        0        0     5288 2023-06-24 20:39:53.000000 quik-ai-1.2.0/src/quik_ai/heads.py
+-rw-rw-rw-   0        0        0    18541 2023-06-08 20:45:11.000000 quik-ai-1.2.0/src/quik_ai/layers.py
+-rw-rw-rw-   0        0        0      941 2023-06-24 18:02:43.000000 quik-ai-1.2.0/src/quik_ai/losses.py
+-rw-rw-rw-   0        0        0     2750 2023-06-24 19:15:10.000000 quik-ai-1.2.0/src/quik_ai/metrics.py
+-rw-rw-rw-   0        0        0    29563 2023-06-24 13:10:54.000000 quik-ai-1.2.0/src/quik_ai/models.py
+-rw-rw-rw-   0        0        0     1633 2023-06-06 23:57:01.000000 quik-ai-1.2.0/src/quik_ai/optimizers.py
+-rw-rw-rw-   0        0        0     8255 2023-06-12 21:22:26.000000 quik-ai-1.2.0/src/quik_ai/predictors.py
+-rw-rw-rw-   0        0        0     9426 2023-06-24 00:56:24.000000 quik-ai-1.2.0/src/quik_ai/tuners.py
+-rw-rw-rw-   0        0        0     3344 2023-06-10 16:18:42.000000 quik-ai-1.2.0/src/quik_ai/tuning.py
+drwxrwxrwx   0        0        0        0 2023-06-24 20:57:06.143436 quik-ai-1.2.0/src/quik_ai.egg-info/
+-rw-rw-rw-   0        0        0     2235 2023-06-24 20:57:05.000000 quik-ai-1.2.0/src/quik_ai.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      500 2023-06-24 20:57:06.000000 quik-ai-1.2.0/src/quik_ai.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-24 20:57:05.000000 quik-ai-1.2.0/src/quik_ai.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      109 2023-06-24 20:57:05.000000 quik-ai-1.2.0/src/quik_ai.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        8 2023-06-24 20:57:05.000000 quik-ai-1.2.0/src/quik_ai.egg-info/top_level.txt
```

### Comparing `quik-ai-1.1.0/LICENSE` & `quik-ai-1.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `quik-ai-1.1.0/PKG-INFO` & `quik-ai-1.2.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 Metadata-Version: 2.1
 Name: quik-ai
-Version: 1.1.0
+Version: 1.2.0
 Summary: Quick Unifying Infrastructure Kit for Machine Learning and AI
 Home-page: https://github.com/touzov1012/quik-ai
-Download-URL: https://github.com/touzov1012/quik-ai/archive/refs/tags/v1.1.0.tar.gz
+Download-URL: https://github.com/touzov1012/quik-ai/archive/refs/tags/v1.2.0.tar.gz
 Author: Aleksandr Touzov
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

### Comparing `quik-ai-1.1.0/README.md` & `quik-ai-1.2.0/README.md`

 * *Files identical despite different names*

### Comparing `quik-ai-1.1.0/setup.cfg` & `quik-ai-1.2.0/setup.cfg`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 00000000: 5b6d 6574 6164 6174 615d 0d0a 6e61 6d65  [metadata]..name
 00000010: 203d 2071 7569 6b2d 6169 0d0a 7665 7273   = quik-ai..vers
-00000020: 696f 6e20 3d20 312e 312e 300d 0a61 7574  ion = 1.1.0..aut
+00000020: 696f 6e20 3d20 312e 322e 300d 0a61 7574  ion = 1.2.0..aut
 00000030: 686f 7220 3d20 416c 656b 7361 6e64 7220  hor = Aleksandr 
 00000040: 546f 757a 6f76 0d0a 6465 7363 7269 7074  Touzov..descript
 00000050: 696f 6e20 3d20 5175 6963 6b20 556e 6966  ion = Quick Unif
 00000060: 7969 6e67 2049 6e66 7261 7374 7275 6374  ying Infrastruct
 00000070: 7572 6520 4b69 7420 666f 7220 4d61 6368  ure Kit for Mach
 00000080: 696e 6520 4c65 6172 6e69 6e67 2061 6e64  ine Learning and
 00000090: 2041 490d 0a6c 6f6e 675f 6465 7363 7269   AI..long_descri
@@ -15,15 +15,15 @@
 000000e0: 726b 646f 776e 0d0a 7572 6c20 3d20 6874  rkdown..url = ht
 000000f0: 7470 733a 2f2f 6769 7468 7562 2e63 6f6d  tps://github.com
 00000100: 2f74 6f75 7a6f 7631 3031 322f 7175 696b  /touzov1012/quik
 00000110: 2d61 690d 0a64 6f77 6e6c 6f61 645f 7572  -ai..download_ur
 00000120: 6c20 3d20 6874 7470 733a 2f2f 6769 7468  l = https://gith
 00000130: 7562 2e63 6f6d 2f74 6f75 7a6f 7631 3031  ub.com/touzov101
 00000140: 322f 7175 696b 2d61 692f 6172 6368 6976  2/quik-ai/archiv
-00000150: 652f 7265 6673 2f74 6167 732f 7631 2e31  e/refs/tags/v1.1
+00000150: 652f 7265 6673 2f74 6167 732f 7631 2e32  e/refs/tags/v1.2
 00000160: 2e30 2e74 6172 2e67 7a0d 0a63 6c61 7373  .0.tar.gz..class
 00000170: 6966 6965 7273 203d 200d 0a09 5072 6f67  ifiers = ...Prog
 00000180: 7261 6d6d 696e 6720 4c61 6e67 7561 6765  ramming Language
 00000190: 203a 3a20 5079 7468 6f6e 203a 3a20 330d   :: Python :: 3.
 000001a0: 0a09 4c69 6365 6e73 6520 3a3a 204f 5349  ..License :: OSI
 000001b0: 2041 7070 726f 7665 6420 3a3a 2041 7061   Approved :: Apa
 000001c0: 6368 6520 536f 6674 7761 7265 204c 6963  che Software Lic
```

### Comparing `quik-ai-1.1.0/src/quik_ai/backend.py` & `quik-ai-1.2.0/src/quik_ai/backend.py`

 * *Files identical despite different names*

### Comparing `quik-ai-1.1.0/src/quik_ai/engine.py` & `quik-ai-1.2.0/src/quik_ai/engine.py`

 * *Files 10% similar despite different names*

```diff
@@ -2,42 +2,46 @@
 from quik_ai import optimizers
 from quik_ai import backend
 
 import tensorflow as tf
 import keras_tuner as kt
 import numpy as np
 import pandas as pd
+import os
 
 class Driver(tuning.Tunable):
     
     def __init__(
         self, 
         training_data, 
         validation_data, 
         testing_data, 
         optimizer='adam',
         max_steps_per_epoch=None,
         weights_column=None,
         time_group_column=None,
         shuffle=True,
         batch_size=tuning.HyperChoice([64, 128, 256, 512, 1024, 2048, 4096]),
+        working_dir='./tmp', 
         **kwargs
     ):
         super().__init__('Driver', **kwargs)
         
         self.training_data = training_data
         self.validation_data = validation_data 
         self.testing_data = testing_data
         self.optimizer = optimizer
         self.max_steps_per_epoch = max_steps_per_epoch
         self.weights_column = weights_column
         self.time_group_column = time_group_column
         
         self.shuffle = shuffle
         self.batch_size = batch_size
+        self.working_dir = working_dir
+        self.file_dir = backend.create_unique_dir(working_dir=self.working_dir)
     
     def get_parameters(self, hp):
         config = super().get_parameters(hp)
         config.update({
             'shuffle' : self._get_hp(None, 'shuffle', hp),
             'batch_size' : self._get_hp(None, 'batch_size', hp),
         })
@@ -93,20 +97,17 @@
         if isinstance(self.optimizer, optimizers.Optimizer):
             return self.optimizer.build(hp)
         
         return self.optimizer
     
     def get_training_steps_per_epoch(self, hp):
         steps_per_epoch = max(self.training_data.shape[0] // self.get_parameters(hp)['batch_size'], 1)
-        if self.max_steps_per_epoch is not None:
-            return min(self.max_steps_per_epoch, steps_per_epoch)
-        return steps_per_epoch
-    
-    def get_validation_steps_per_epoch(self, hp):
-        return max(self.validation_data.shape[0] // self.get_parameters(hp)['batch_size'], 1)
+        if self.max_steps_per_epoch is not None and self.max_steps_per_epoch < steps_per_epoch:
+            return self.max_steps_per_epoch
+        return None
     
     def __get_partitioned_data(self, data, input_names, response, time_window):
         
         # cache the names of the columns corresponding to each tensor type
         names_map = {}
         for name in input_names:
             key = (self.get_input_dtype(name), self.get_input_shape(name, time_window))
@@ -129,161 +130,208 @@
         
         # get the str and float parts of the new_data
         tensor_map = {}
         for key, value in names_map.items():
             tensor_map[key] = self.get_data_tensor(data, value)
         
         # generate y and w if we have them
-        y = np.squeeze(self.get_data_tensor(data, response), axis=1) if response is not None else None
-        w = data[self.weights_column].to_numpy() if self.weights_column is not None else None
+        y = np.float32(np.squeeze(self.get_data_tensor(data, response), axis=1)) if response is not None else None
+        w = data[self.weights_column].to_numpy(dtype=np.float32) if self.weights_column is not None else None
         
         # remove w if no response
         w = None if y is None else w
         
         return {
             'row_order' : row_order,
             'group_order' : group_order,
             'names_map' : names_map,
             'tensor_map' : tensor_map,
             'y' : y,
             'w' : w,
         }
     
+    def __bytes_feature(self, value):
+        if isinstance(value, type(tf.constant(0))):
+            value = value.numpy()
+        return tf.train.Feature(bytes_list=tf.train.BytesList(value=[tf.io.serialize_tensor(value).numpy()]))
+    
+    def __float_feature(self, value):
+        return tf.train.Feature(float_list=tf.train.FloatList(value=[value]))
+    
+    def __serialize_example(self, x, y=None, w=None):
+        input_features = {name: self.__bytes_feature(tensor) for name, tensor in x.items()}
+        if y is not None:
+            input_features['__response__'] = self.__bytes_feature(y)
+        if w is not None:
+            input_features['__weights__'] = self.__float_feature(w)
+        example_proto = tf.train.Example(features=tf.train.Features(feature=input_features))
+        return example_proto.SerializeToString()
+    
     def __get_tensorflow_generator(
         self, 
         data, 
         input_names, 
         response, 
-        run_forever,
         time_window, 
-        batch_size, 
+        batch_size,
         shuffle, 
+        name,
+        reinit=True,
         **kwargs
     ):  
-        # presort by index
-        data = data.sort_index()
+        # file name
+        filepath = backend.join_path(self.file_dir, '%s.tfrecords' % name)
         
-        # if we have a time group, first sort by group
-        if self.time_group_column is not None:
-            data = data.reset_index().rename(columns={'index': '__group_id__'})
-            data = data.sort_values(by=[self.time_group_column, '__group_id__'])
-            data['__group_id__'] = data.groupby(self.time_group_column).cumcount()
-        
-        # split the data into different type tensors and get the
-        # order of the rows as well as the element of the row in
-        # each group if we have a time group
-        cache = self.__get_partitioned_data(data, input_names, response, time_window)
-        
-        # get the order of our results
-        row_order = cache['row_order']
-        
-        # sliced tensor input
-        sliced_tensors = {}
-        
-        # build the generator
-        def generator():
-            while True:
-                # shuffle if we need to
-                if shuffle:
-                    np.random.shuffle(row_order)
+        # check if we already have this record dataset
+        # if we do, and we want to reinit, then delete it
+        if not os.path.exists(filepath) or reinit:
+            
+            # presort by index
+            data = data.sort_index()
 
-                # yield loop to iterate over the data
+            # if we have a time group, first sort by group
+            if self.time_group_column is not None:
+                data = data.reset_index().rename(columns={'index': '__group_id__'})
+                data = data.sort_values(by=[self.time_group_column, '__group_id__'])
+                data['__group_id__'] = data.groupby(self.time_group_column).cumcount()
+
+            # split the data into different type tensors and get the
+            # order of the rows as well as the element of the row in
+            # each group if we have a time group
+            cache = self.__get_partitioned_data(data, input_names, response, time_window)
+
+            # get the order of our results
+            row_order = cache['row_order']
+
+            # sliced tensor input
+            sliced_tensors = {}
+
+            # shuffle if we need to
+            if shuffle:
+                np.random.shuffle(row_order)
+
+            # combine the predictor names
+            x_keys = []
+            for value in cache['names_map'].values():
+                x_keys += value
+                
+            # yield loop to iterate over the data
+            with tf.io.TFRecordWriter(filepath) as writer:
                 for end in row_order:
-                    
+
                     # clear the previous slices
                     sliced_tensors.clear()
-                    
+
                     # filter to sub-array depending on if we have a time group
                     if self.time_group_column is None:
                         for key, value in cache['tensor_map'].items():
                             sliced_tensors[key] = value[:end+1]
                     else:
                         group_id = cache['group_order'][end]
                         for key, value in cache['tensor_map'].items():
                             sliced_tensors[key] = value[end-group_id:end+1]
 
                     # different fetch for time series and flat array, we may need to pad
                     # the time series if it there is not enough history
                     for key in sliced_tensors.keys():
                         fill_type = '[UNK]' if key[0] == tf.string else 0
                         sliced_tensors[key] = backend.get_k_from_end(sliced_tensors[key], time_window, fill=fill_type)
-                        
-                    # combine the predictor names
-                    x_keys = []
-                    for value in cache['names_map'].values():
-                        x_keys += value
-                    
+
                     # combine the predictor vectors
                     x_values = []
                     for key, value in sliced_tensors.items():
                         splits = np.split(value, value.shape[1], axis=1)
                         for split in splits:
                             squeezed = np.squeeze(split, axis=(0,1)) if time_window <= 1 else np.squeeze(split, axis=1)
-                            x_values.append(np.reshape(squeezed, key[1]))
-                    
+                            squeezed = np.reshape(squeezed, key[1])
+                            x_values.append(tf.convert_to_tensor(squeezed, dtype=key[0]))
+
                     if cache['y'] is None:
-                        yield dict(zip(x_keys, x_values))
+                        example = self.__serialize_example(dict(zip(x_keys, x_values)))
+                    elif cache['w'] is None:
+                        example = self.__serialize_example(dict(zip(x_keys, x_values)), cache['y'][end])
                     else:
-                        if cache['w'] is None:
-                            yield (dict(zip(x_keys, x_values)), cache['y'][end])
-                        else:
-                            yield (dict(zip(x_keys, x_values)), cache['y'][end], cache['w'][end])
-                
-                # should we terminate the forever loop for a single data pass?
-                if not run_forever:
-                    break
-        
-        # we either have a time series or not, if we have a time series
-        # we will use the generator to get data to avoid memory overflow
-        # otherwise we can use the full data without processing
-        input_tensor_specs = []
-        for name in input_names:
-            dtype = self.get_input_dtype(name)
-            shape = self.get_input_shape(name, time_window)
+                        example = self.__serialize_example(dict(zip(x_keys, x_values)), cache['y'][end], cache['w'][end])
+                    
+                    # write the observation
+                    writer.write(example)
             
-            input_tensor_specs.append(tf.TensorSpec(shape=shape, dtype=dtype))
+        # create the raw data
+        raw_dataset = tf.data.TFRecordDataset(filepath)
         
-        # build the signature
-        output_signature = dict(zip(input_names, input_tensor_specs))
-
-        # append the response and weights
-        if cache['y'] is not None:
-            # get the response shape
-            response_shape = self.get_input_shape(response, 1)
-            response_shape = () if response_shape == (1,) else response_shape
-            
-            # append to the signature
-            output_signature = (output_signature, tf.TensorSpec(shape=response_shape, dtype=self.get_input_dtype(response)))
+        # create the description of each feature
+        feature_description = {key: tf.io.FixedLenFeature([], tf.string) for key in input_names}
+        if response is not None:
+            feature_description['__response__'] = tf.io.FixedLenFeature([], tf.string)
+        if self.weights_column is not None and response is not None:
+            feature_description['__weights__'] = tf.io.FixedLenFeature([], tf.float32)
+        
+        # create a mapping to parse our serialized data
+        def _parse_function(example_proto):
+            features = tf.io.parse_single_example(example_proto, feature_description)
+            inputs = {name: tf.io.parse_tensor(features[name], out_type=self.get_input_dtype(name)) 
+                      for name in features if name != '__response__' and name != '__weights__'}
+            if response is None:
+                return inputs
+            elif self.weights_column is None:
+                return inputs, tf.io.parse_tensor(features['__response__'], out_type=tf.float32)
+            else:
+                return inputs, tf.io.parse_tensor(features['__response__'], out_type=tf.float32), features['__weights__']
+        
+        # return the deserialized dataset of observations
+        tdf = raw_dataset.map(_parse_function)
+        
+        # if we shuffle
+        if shuffle:
+            tdf = tdf.shuffle(2048, seed=1337)
         
-        # append the weights to the signature
-        if cache['w'] is not None:
-            output_signature += (tf.TensorSpec(shape=(), dtype=tf.float32),)
-        
-        # return the built generator
-        return tf.data.Dataset.from_generator(
-            generator,
-            output_signature=output_signature
-        )
+        return tdf.batch(batch_size).prefetch(tf.data.AUTOTUNE)
     
-    def get_tensorflow_dataset(self, data, input_names, response, run_forever, time_window, hp, shuffle=None):
+    def get_tensorflow_dataset(
+        self, 
+        data, 
+        input_names, 
+        response,
+        time_window, 
+        hp, 
+        shuffle=None, 
+        name='testing',
+        reinit=True
+    ):
+        # we may have tuning parameters
         config = self.get_parameters(hp)
         
         # option added to not shuffle if we want to do inference
         if shuffle is not None:
             config['shuffle'] = shuffle
         
-        tdf = self.__get_tensorflow_generator(
+        return self.__get_tensorflow_generator(
             data, 
             input_names, 
             response, 
-            run_forever=run_forever,
             time_window=time_window,
+            name=name,
+            reinit=reinit,
             **config
         )
-        
-        return tdf.batch(config['batch_size']).prefetch(tf.data.AUTOTUNE)
     
     def get_training_tensorflow_dataset(self, input_names, response, time_window, hp):
-        return self.get_tensorflow_dataset(self.training_data, input_names, response, True, time_window, hp)
+        return self.get_tensorflow_dataset(
+            self.training_data, 
+            input_names, 
+            response, 
+            time_window, 
+            hp, 
+            name='training', 
+            reinit=False
+        )
     
     def get_validation_tensorflow_dataset(self, input_names, response, time_window, hp):
-        return self.get_tensorflow_dataset(self.validation_data, input_names, response, True, time_window, hp)
+        return self.get_tensorflow_dataset(
+            self.validation_data, 
+            input_names, 
+            response, 
+            time_window, 
+            hp, 
+            name='validation', 
+            reinit=False
+        )
```

### Comparing `quik-ai-1.1.0/src/quik_ai/heads.py` & `quik-ai-1.2.0/src/quik_ai/heads.py`

 * *Files 4% similar despite different names*

```diff
@@ -2,14 +2,24 @@
 from quik_ai import layers
 from quik_ai import losses
 from quik_ai import metrics
 
 import tensorflow as tf
 import tensorflow_probability as tfp
 
+losses_dictionary = {
+    'mean_squared_error' : tf.keras.losses.MeanSquaredError,
+    'log_prob' : losses.LogProbLoss,
+}
+
+metrics_dictionary = {
+    'mean_squared_error' : metrics.MeanSquaredErrorMetric,
+    'log_prob' : metrics.LogProbMetric,
+}
+
 class Head(tuning.Tunable):
     def __init__(
         self, 
         name, 
         non_linear_projection=tuning.HyperBoolean(),
         projection_scale=tuning.HyperInt(min_value=1, max_value=4),
         activation=tuning.HyperChoice(['relu','gelu']),
@@ -51,18 +61,18 @@
     def body(self, inputs, **kwargs):
         return tf.keras.layers.Dense(self.event_size)(inputs)
     
     def monitor(self):
         return self.loss_name
     
     def loss(self):
-        return self.loss_name
+        return losses_dictionary[self.loss_name]()
     
     def metrics(self):
-        return self.loss_name
+        return metrics_dictionary[self.loss_name]()
 
 class Logistic(Head):
     def __init__(self, event_size, sparse_response=True, multi_label=False, name='Logistic', **kwargs):
         super().__init__(name, **kwargs)
         
         self.event_size = event_size
         self.sparse_response = sparse_response
@@ -85,19 +95,19 @@
         elif self.multi_label:
             return tf.keras.losses.BinaryCrossentropy(from_logits=True)
         else:
             return tf.keras.losses.CategoricalCrossentropy(from_logits=True)
     
     def metrics(self):
         if self.sparse_response:
-            return tf.keras.metrics.SparseCategoricalCrossentropy(from_logits=True)
+            return [tf.keras.metrics.SparseCategoricalCrossentropy(from_logits=True), 'sparse_categorical_accuracy']
         elif self.multi_label:
-            return tf.keras.metrics.BinaryCrossentropy(from_logits=True)
+            return [tf.keras.metrics.BinaryCrossentropy(from_logits=True), 'binary_accuracy']
         else:
-            return tf.keras.metrics.CategoricalCrossentropy(from_logits=True)
+            return [tf.keras.metrics.CategoricalCrossentropy(from_logits=True), 'categorical_accuracy']
         
 class GaussianMixture(Head):
     def __init__(
         self,  
         event_shape=[1], 
         mix_components=tuning.HyperChoice([8, 16, 32, 64, 128]), 
         positive_only=False,
```

### Comparing `quik-ai-1.1.0/src/quik_ai/layers.py` & `quik-ai-1.2.0/src/quik_ai/layers.py`

 * *Files identical despite different names*

### Comparing `quik-ai-1.1.0/src/quik_ai/losses.py` & `quik-ai-1.2.0/src/quik_ai/losses.py`

 * *Files 13% similar despite different names*

```diff
@@ -4,18 +4,19 @@
 class LogProbLoss(tf.keras.losses.Loss):
     def __init__(self, response_noise, log_response, name='log_prob', **kwargs):
         super().__init__(name=name, **kwargs)
         
         self.response_noise = response_noise
         self.log_response = log_response
 
-    def call(self, response, model, w=None):
-        response = tf.cast(response, tf.float32) + tf.random.uniform(tf.shape(response), -self.response_noise, self.response_noise)
+    def call(self, response, model):
+        response = tf.cast(tf.reshape(response, tf.shape(model)), tf.float32)
+        response = response + tf.random.uniform(tf.shape(response), -self.response_noise, self.response_noise)
         response = tf.math.log(tf.math.maximum(response,1.0)) if self.log_response else response
-        return -model.log_prob(response) if w is None else -model.log_prob(response) * w
+        return -model.log_prob(response)
     
     def get_config(self):
         config = super().get_config()
         config.update({
             'response_noise' : self.response_noise,
             'log_response' : self.log_response,
         })
```

### Comparing `quik-ai-1.1.0/src/quik_ai/models.py` & `quik-ai-1.2.0/src/quik_ai/models.py`

 * *Files 2% similar despite different names*

```diff
@@ -26,14 +26,15 @@
         predictors,
         driver,
         instance=None,
         time_window=1,
         time_dropout=0.05,
         seed=None,
         run_eagerly=None,
+        working_dir='./tmp', 
         **kwargs
     ):
         kt.HyperModel.__init__(self, name, **kwargs)
         tuning.Tunable.__init__(self, name, **kwargs)
         
         self.response = response
         self.head = head
@@ -41,14 +42,15 @@
         self.driver = driver
         self.instance = instance
         
         self.time_window = time_window
         self.time_dropout = time_dropout
         self.seed = seed
         self.run_eagerly = run_eagerly
+        self.working_dir = working_dir
     
     @classmethod
     def load(cls, filepath='./model'):
         # load tensorflow model, if it was saved
         model = None
         tf_model_path = backend.join_path(filepath, 'tf_model')
         if os.path.exists(tf_model_path):
@@ -189,14 +191,17 @@
     def build(self, hp):
         
         # if we want to build without tuning fill out a
         # dummy instance of hp so we can sample some params
         if hp is None:
             hp = kt.HyperParameters()
         
+        # cache parameters of driver
+        self.driver.get_parameters(hp)
+        
         # get parameters
         config = self.get_parameters(hp)
         
         # get input layers as a dict
         inputs = self.__build_input_layers(**config)
         
         # build the input tensor from all input layers
@@ -239,15 +244,14 @@
             *args, 
         ]
         
         # cache the kwargs to the fit function
         fit_kwargs = dict(
             steps_per_epoch=self.driver.get_training_steps_per_epoch(hp), 
             validation_data=self.driver.get_validation_tensorflow_dataset(input_names, self.response, config['time_window'], hp), 
-            validation_steps=self.driver.get_validation_steps_per_epoch(hp), 
         )
         
         # check if we have mlflow active
         active_run = mlflow.active_run() if mlflow is not None else None
         
         # if we have an active mlflow run
         if active_run is not None:
@@ -257,37 +261,33 @@
                 return model.fit(*fit_args, **fit_kwargs, **kwargs)
         
         # no mlflow run, return as normal
         return model.fit(*fit_args, **fit_kwargs, **kwargs)
     
     def train(
         self,
-        tuner_container=None,
+        tuner=tuners.BOHB,
         early_stopping_tune=10, 
         early_stopping_full=10,
         full_rounds=1,
-        working_dir='.', 
+        tuner_params={},
         verbose=1
     ):
-        # if no tuner, set the default option
-        if tuner_container is None:
-            tuner_container = tuners.TunerContainer(tuners.BOHB)
         
         # create working directory for the build
-        build_dir = backend.create_unique_dir(working_dir=working_dir)
+        build_dir = backend.create_unique_dir(working_dir=self.working_dir)
 
         backend.info('Checking for hyper-parameters to tune ...', verbose)
 
         # set up the keras tuner parameters
         checkpoint_monitor = 'val_' + self.head.monitor()
 
         # create the tuner
-        tuner_params = tuner_container.get_tuner_params()
         tuner_epochs = tuner_params.pop('epochs', 1)
-        tuner = tuner_container.tuner(
+        tuner = tuner(
             self, 
             objective=kt.Objective(checkpoint_monitor, direction=self.head.objective_direction),
             directory=backend.join_path(build_dir, 'tuner'),
             project_name='kt_tuner', 
             **tuner_params
         )
 
@@ -411,18 +411,17 @@
             return None
         
         # build the input dataset from the numpy array
         tdf = self.driver.get_tensorflow_dataset(
             data, 
             input_names=self.get_input_names(), 
             response=None, 
-            run_forever=False, 
             time_window=self.time_window, 
             hp=None, 
-            shuffle=False
+            shuffle=False,
         )
         
         return self.instance.predict(tdf, verbose=verbose)
     
     def predict_distribution(self, data, samples):
         
         if self.instance is None:
@@ -430,18 +429,17 @@
             return None
         
         # build the input dataset from the numpy array
         tdf = self.driver.get_tensorflow_dataset(
             data, 
             input_names=self.get_input_names(), 
             response=None, 
-            run_forever=False, 
             time_window=self.time_window, 
             hp=None, 
-            shuffle=False
+            shuffle=False,
         )
         
         # get outputs for each data point
         outputs = []
         for x in tdf:
             outputs.append(self.instance(x))
         
@@ -474,18 +472,17 @@
             data = self.driver.testing_data
         
         # build the input dataset from the numpy array
         tdf = self.driver.get_tensorflow_dataset(
             data, 
             input_names=self.get_input_names(), 
             response=self.response, 
-            run_forever=False, 
             time_window=self.time_window, 
             hp=None, 
-            shuffle=False
+            shuffle=False,
         )
         
         # evalute the results
         evals = self.instance.evaluate(tdf, verbose=verbose)
         
         # pair each result with the metric name
         res = {}
```

### Comparing `quik-ai-1.1.0/src/quik_ai/optimizers.py` & `quik-ai-1.2.0/src/quik_ai/optimizers.py`

 * *Files identical despite different names*

### Comparing `quik-ai-1.1.0/src/quik_ai/predictors.py` & `quik-ai-1.2.0/src/quik_ai/predictors.py`

 * *Files identical despite different names*

### Comparing `quik-ai-1.1.0/src/quik_ai/tuners.py` & `quik-ai-1.2.0/src/quik_ai/tuners.py`

 * *Files 2% similar despite different names*

```diff
@@ -14,22 +14,14 @@
 
 from keras_tuner.engine import hyperparameters as hp_module
 from keras_tuner.engine import tuner as tuner_module
 
 from keras_tuner.tuners import hyperband as hyperband_module
 from keras_tuner.tuners import bayesian as bayesian_module
 
-class TunerContainer:
-    def __init__(self, tuner, **kwargs):
-        self.tuner = tuner
-        self.kwargs = kwargs
-        
-    def get_tuner_params(self):
-        return self.kwargs.copy()
-
 class BOHBOracle(hyperband_module.HyperbandOracle):
 
     def __init__(
         self,
         objective=None,
         max_epochs=100,
         factor=3,
```

### Comparing `quik-ai-1.1.0/src/quik_ai/tuning.py` & `quik-ai-1.2.0/src/quik_ai/tuning.py`

 * *Files identical despite different names*

### Comparing `quik-ai-1.1.0/src/quik_ai.egg-info/PKG-INFO` & `quik-ai-1.2.0/src/quik_ai.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 Metadata-Version: 2.1
 Name: quik-ai
-Version: 1.1.0
+Version: 1.2.0
 Summary: Quick Unifying Infrastructure Kit for Machine Learning and AI
 Home-page: https://github.com/touzov1012/quik-ai
-Download-URL: https://github.com/touzov1012/quik-ai/archive/refs/tags/v1.1.0.tar.gz
+Download-URL: https://github.com/touzov1012/quik-ai/archive/refs/tags/v1.2.0.tar.gz
 Author: Aleksandr Touzov
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

