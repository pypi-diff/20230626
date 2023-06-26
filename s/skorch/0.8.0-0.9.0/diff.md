# Comparing `tmp/skorch-0.8.0.tar.gz` & `tmp/skorch-0.9.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/skorch-0.8.0.tar", last modified: Sun Apr 12 16:28:14 2020, max compression
+gzip compressed data, was "dist/skorch-0.9.0.tar", last modified: Sun Aug 30 10:43:14 2020, max compression
```

## Comparing `skorch-0.8.0.tar` & `skorch-0.9.0.tar`

### file list

```diff
@@ -1,51 +1,53 @@
-drwxr-xr-x   0 vinh      (1000) vinh      (1000)        0 2020-04-12 16:28:14.000000 skorch-0.8.0/
--rw-r--r--   0 vinh      (1000) vinh      (1000)     1543 2020-02-08 20:37:16.000000 skorch-0.8.0/LICENSE
--rw-r--r--   0 vinh      (1000) vinh      (1000)       68 2020-02-08 20:37:16.000000 skorch-0.8.0/MANIFEST.in
--rw-r--r--   0 vinh      (1000) vinh      (1000)     9438 2020-04-12 16:28:14.000000 skorch-0.8.0/PKG-INFO
--rw-r--r--   0 vinh      (1000) vinh      (1000)     7113 2020-04-12 16:19:26.000000 skorch-0.8.0/README.rst
--rw-r--r--   0 vinh      (1000) vinh      (1000)        6 2020-04-10 15:29:08.000000 skorch-0.8.0/VERSION
--rw-r--r--   0 vinh      (1000) vinh      (1000)      196 2020-04-10 08:42:33.000000 skorch-0.8.0/requirements-dev.txt
--rw-r--r--   0 vinh      (1000) vinh      (1000)       77 2020-02-08 20:37:16.000000 skorch-0.8.0/requirements.txt
--rw-r--r--   0 vinh      (1000) vinh      (1000)      211 2020-04-12 16:28:14.000000 skorch-0.8.0/setup.cfg
--rw-r--r--   0 vinh      (1000) vinh      (1000)     1027 2020-02-08 20:37:16.000000 skorch-0.8.0/setup.py
-drwxr-xr-x   0 vinh      (1000) vinh      (1000)        0 2020-04-12 16:28:14.000000 skorch-0.8.0/skorch/
--rw-r--r--   0 vinh      (1000) vinh      (1000)     1286 2020-02-08 20:37:16.000000 skorch-0.8.0/skorch/__init__.py
-drwxr-xr-x   0 vinh      (1000) vinh      (1000)        0 2020-04-12 16:28:14.000000 skorch-0.8.0/skorch/callbacks/
--rw-r--r--   0 vinh      (1000) vinh      (1000)      762 2020-04-10 08:42:33.000000 skorch-0.8.0/skorch/callbacks/__init__.py
--rw-r--r--   0 vinh      (1000) vinh      (1000)     2167 2020-02-08 20:37:16.000000 skorch-0.8.0/skorch/callbacks/base.py
--rw-r--r--   0 vinh      (1000) vinh      (1000)    25027 2020-04-10 08:42:33.000000 skorch-0.8.0/skorch/callbacks/logging.py
--rw-r--r--   0 vinh      (1000) vinh      (1000)     7886 2020-02-08 20:37:16.000000 skorch-0.8.0/skorch/callbacks/lr_scheduler.py
--rw-r--r--   0 vinh      (1000) vinh      (1000)     1499 2020-02-21 23:19:51.000000 skorch-0.8.0/skorch/callbacks/regularization.py
--rw-r--r--   0 vinh      (1000) vinh      (1000)    19719 2020-04-11 08:51:06.000000 skorch-0.8.0/skorch/callbacks/scoring.py
--rw-r--r--   0 vinh      (1000) vinh      (1000)    24830 2020-03-17 21:16:50.000000 skorch-0.8.0/skorch/callbacks/training.py
--rw-r--r--   0 vinh      (1000) vinh      (1000)    13557 2020-04-10 08:42:33.000000 skorch-0.8.0/skorch/classifier.py
--rw-r--r--   0 vinh      (1000) vinh      (1000)     9522 2020-02-08 20:37:16.000000 skorch-0.8.0/skorch/cli.py
--rw-r--r--   0 vinh      (1000) vinh      (1000)    11164 2020-04-11 08:58:07.000000 skorch-0.8.0/skorch/dataset.py
--rw-r--r--   0 vinh      (1000) vinh      (1000)      471 2020-02-08 20:37:16.000000 skorch-0.8.0/skorch/exceptions.py
--rw-r--r--   0 vinh      (1000) vinh      (1000)    16923 2020-03-11 21:34:25.000000 skorch-0.8.0/skorch/helper.py
--rw-r--r--   0 vinh      (1000) vinh      (1000)     7606 2020-02-08 20:37:16.000000 skorch-0.8.0/skorch/history.py
--rw-r--r--   0 vinh      (1000) vinh      (1000)    60104 2020-04-10 08:42:33.000000 skorch-0.8.0/skorch/net.py
--rw-r--r--   0 vinh      (1000) vinh      (1000)     2990 2020-02-08 20:37:16.000000 skorch-0.8.0/skorch/regressor.py
--rw-r--r--   0 vinh      (1000) vinh      (1000)     2355 2020-02-08 20:37:16.000000 skorch-0.8.0/skorch/setter.py
-drwxr-xr-x   0 vinh      (1000) vinh      (1000)        0 2020-04-12 16:28:14.000000 skorch-0.8.0/skorch/tests/
--rw-r--r--   0 vinh      (1000) vinh      (1000)        0 2020-02-08 20:37:16.000000 skorch-0.8.0/skorch/tests/__init__.py
--rw-r--r--   0 vinh      (1000) vinh      (1000)     3918 2020-04-10 08:42:33.000000 skorch-0.8.0/skorch/tests/conftest.py
--rw-r--r--   0 vinh      (1000) vinh      (1000)    11278 2020-02-29 11:56:39.000000 skorch-0.8.0/skorch/tests/test_classifier.py
--rw-r--r--   0 vinh      (1000) vinh      (1000)    11084 2020-02-08 20:37:16.000000 skorch-0.8.0/skorch/tests/test_cli.py
--rw-r--r--   0 vinh      (1000) vinh      (1000)    30702 2020-02-29 11:56:39.000000 skorch-0.8.0/skorch/tests/test_dataset.py
--rw-r--r--   0 vinh      (1000) vinh      (1000)    24150 2020-03-11 21:34:25.000000 skorch-0.8.0/skorch/tests/test_helper.py
--rw-r--r--   0 vinh      (1000) vinh      (1000)     8506 2020-02-08 20:37:16.000000 skorch-0.8.0/skorch/tests/test_history.py
--rw-r--r--   0 vinh      (1000) vinh      (1000)    88304 2020-04-10 08:42:33.000000 skorch-0.8.0/skorch/tests/test_net.py
--rw-r--r--   0 vinh      (1000) vinh      (1000)     4102 2020-02-29 11:56:39.000000 skorch-0.8.0/skorch/tests/test_regressor.py
--rw-r--r--   0 vinh      (1000) vinh      (1000)     2493 2020-02-08 20:37:16.000000 skorch-0.8.0/skorch/tests/test_setter.py
--rw-r--r--   0 vinh      (1000) vinh      (1000)     3326 2020-02-08 20:37:16.000000 skorch-0.8.0/skorch/tests/test_toy.py
--rw-r--r--   0 vinh      (1000) vinh      (1000)    22158 2020-04-10 08:42:33.000000 skorch-0.8.0/skorch/tests/test_utils.py
--rw-r--r--   0 vinh      (1000) vinh      (1000)     4715 2020-02-08 20:37:16.000000 skorch-0.8.0/skorch/toy.py
--rw-r--r--   0 vinh      (1000) vinh      (1000)    15371 2020-04-10 08:42:33.000000 skorch-0.8.0/skorch/utils.py
-drwxr-xr-x   0 vinh      (1000) vinh      (1000)        0 2020-04-12 16:28:14.000000 skorch-0.8.0/skorch.egg-info/
--rw-r--r--   0 vinh      (1000) vinh      (1000)     9438 2020-04-12 16:28:14.000000 skorch-0.8.0/skorch.egg-info/PKG-INFO
--rw-r--r--   0 vinh      (1000) vinh      (1000)     1018 2020-04-12 16:28:14.000000 skorch-0.8.0/skorch.egg-info/SOURCES.txt
--rw-r--r--   0 vinh      (1000) vinh      (1000)        1 2020-04-12 16:28:14.000000 skorch-0.8.0/skorch.egg-info/dependency_links.txt
--rw-r--r--   0 vinh      (1000) vinh      (1000)        1 2020-04-12 16:28:14.000000 skorch-0.8.0/skorch.egg-info/not-zip-safe
--rw-r--r--   0 vinh      (1000) vinh      (1000)      147 2020-04-12 16:28:14.000000 skorch-0.8.0/skorch.egg-info/requires.txt
--rw-r--r--   0 vinh      (1000) vinh      (1000)        7 2020-04-12 16:28:14.000000 skorch-0.8.0/skorch.egg-info/top_level.txt
+drwxr-xr-x   0 vinh      (1000) vinh      (1000)        0 2020-08-30 10:43:14.000000 skorch-0.9.0/
+-rw-r--r--   0 vinh      (1000) vinh      (1000)     1543 2020-02-08 20:37:16.000000 skorch-0.9.0/LICENSE
+-rw-r--r--   0 vinh      (1000) vinh      (1000)       68 2020-02-08 20:37:16.000000 skorch-0.9.0/MANIFEST.in
+-rw-r--r--   0 vinh      (1000) vinh      (1000)    10061 2020-08-30 10:43:14.000000 skorch-0.9.0/PKG-INFO
+-rw-r--r--   0 vinh      (1000) vinh      (1000)     7664 2020-08-16 10:14:28.000000 skorch-0.9.0/README.rst
+-rw-r--r--   0 vinh      (1000) vinh      (1000)        6 2020-08-16 10:15:22.000000 skorch-0.9.0/VERSION
+-rw-r--r--   0 vinh      (1000) vinh      (1000)      196 2020-05-12 19:58:32.000000 skorch-0.9.0/requirements-dev.txt
+-rw-r--r--   0 vinh      (1000) vinh      (1000)       77 2020-02-08 20:37:16.000000 skorch-0.9.0/requirements.txt
+-rw-r--r--   0 vinh      (1000) vinh      (1000)      211 2020-08-30 10:43:14.000000 skorch-0.9.0/setup.cfg
+-rw-r--r--   0 vinh      (1000) vinh      (1000)     1027 2020-02-08 20:37:16.000000 skorch-0.9.0/setup.py
+drwxr-xr-x   0 vinh      (1000) vinh      (1000)        0 2020-08-30 10:43:14.000000 skorch-0.9.0/skorch/
+-rw-r--r--   0 vinh      (1000) vinh      (1000)     1532 2020-07-30 21:48:45.000000 skorch-0.9.0/skorch/__init__.py
+drwxr-xr-x   0 vinh      (1000) vinh      (1000)        0 2020-08-30 10:43:14.000000 skorch-0.9.0/skorch/callbacks/
+-rw-r--r--   0 vinh      (1000) vinh      (1000)      762 2020-05-12 19:58:32.000000 skorch-0.9.0/skorch/callbacks/__init__.py
+-rw-r--r--   0 vinh      (1000) vinh      (1000)     2167 2020-05-11 20:35:47.000000 skorch-0.9.0/skorch/callbacks/base.py
+-rw-rw-r--   0 vinh      (1000) vinh      (1000)    25295 2020-07-05 18:18:28.000000 skorch-0.9.0/skorch/callbacks/logging.py
+-rw-r--r--   0 vinh      (1000) vinh      (1000)     9173 2020-06-06 18:35:12.000000 skorch-0.9.0/skorch/callbacks/lr_scheduler.py
+-rw-r--r--   0 vinh      (1000) vinh      (1000)     1499 2020-05-11 20:35:47.000000 skorch-0.9.0/skorch/callbacks/regularization.py
+-rw-r--r--   0 vinh      (1000) vinh      (1000)    19719 2020-05-12 19:58:32.000000 skorch-0.9.0/skorch/callbacks/scoring.py
+-rw-r--r--   0 vinh      (1000) vinh      (1000)    26370 2020-07-30 21:50:11.000000 skorch-0.9.0/skorch/callbacks/training.py
+-rw-r--r--   0 vinh      (1000) vinh      (1000)    11805 2020-07-30 21:50:11.000000 skorch-0.9.0/skorch/classifier.py
+-rw-r--r--   0 vinh      (1000) vinh      (1000)     9522 2020-02-08 20:37:16.000000 skorch-0.9.0/skorch/cli.py
+-rw-r--r--   0 vinh      (1000) vinh      (1000)    11613 2020-06-06 18:35:12.000000 skorch-0.9.0/skorch/dataset.py
+-rw-r--r--   0 vinh      (1000) vinh      (1000)      471 2020-02-08 20:37:16.000000 skorch-0.9.0/skorch/exceptions.py
+-rw-r--r--   0 vinh      (1000) vinh      (1000)    16927 2020-06-06 20:15:12.000000 skorch-0.9.0/skorch/helper.py
+-rw-r--r--   0 vinh      (1000) vinh      (1000)     7606 2020-02-08 20:37:16.000000 skorch-0.9.0/skorch/history.py
+-rw-r--r--   0 vinh      (1000) vinh      (1000)    72668 2020-08-13 20:17:04.000000 skorch-0.9.0/skorch/net.py
+-rw-r--r--   0 vinh      (1000) vinh      (1000)     2990 2020-02-08 20:37:16.000000 skorch-0.9.0/skorch/regressor.py
+-rw-r--r--   0 vinh      (1000) vinh      (1000)     3000 2020-07-30 21:50:11.000000 skorch-0.9.0/skorch/scoring.py
+-rw-r--r--   0 vinh      (1000) vinh      (1000)     2355 2020-02-08 20:37:16.000000 skorch-0.9.0/skorch/setter.py
+drwxr-xr-x   0 vinh      (1000) vinh      (1000)        0 2020-08-30 10:43:14.000000 skorch-0.9.0/skorch/tests/
+-rw-r--r--   0 vinh      (1000) vinh      (1000)        0 2020-02-08 20:37:16.000000 skorch-0.9.0/skorch/tests/__init__.py
+-rw-r--r--   0 vinh      (1000) vinh      (1000)     3993 2020-06-06 18:35:12.000000 skorch-0.9.0/skorch/tests/conftest.py
+-rw-r--r--   0 vinh      (1000) vinh      (1000)    11831 2020-08-16 10:14:28.000000 skorch-0.9.0/skorch/tests/test_classifier.py
+-rw-r--r--   0 vinh      (1000) vinh      (1000)    11084 2020-02-08 20:37:16.000000 skorch-0.9.0/skorch/tests/test_cli.py
+-rw-r--r--   0 vinh      (1000) vinh      (1000)    31725 2020-06-06 18:35:12.000000 skorch-0.9.0/skorch/tests/test_dataset.py
+-rw-r--r--   0 vinh      (1000) vinh      (1000)    24150 2020-03-11 21:34:25.000000 skorch-0.9.0/skorch/tests/test_helper.py
+-rw-r--r--   0 vinh      (1000) vinh      (1000)     8506 2020-02-08 20:37:16.000000 skorch-0.9.0/skorch/tests/test_history.py
+-rw-r--r--   0 vinh      (1000) vinh      (1000)   104875 2020-08-16 10:14:28.000000 skorch-0.9.0/skorch/tests/test_net.py
+-rw-r--r--   0 vinh      (1000) vinh      (1000)     4027 2020-08-16 10:14:28.000000 skorch-0.9.0/skorch/tests/test_regressor.py
+-rw-r--r--   0 vinh      (1000) vinh      (1000)     3813 2020-07-30 21:50:11.000000 skorch-0.9.0/skorch/tests/test_scoring.py
+-rw-r--r--   0 vinh      (1000) vinh      (1000)     2493 2020-02-08 20:37:16.000000 skorch-0.9.0/skorch/tests/test_setter.py
+-rw-r--r--   0 vinh      (1000) vinh      (1000)     3326 2020-02-08 20:37:16.000000 skorch-0.9.0/skorch/tests/test_toy.py
+-rw-r--r--   0 vinh      (1000) vinh      (1000)    29230 2020-07-30 21:50:11.000000 skorch-0.9.0/skorch/tests/test_utils.py
+-rw-r--r--   0 vinh      (1000) vinh      (1000)     4715 2020-02-08 20:37:16.000000 skorch-0.9.0/skorch/toy.py
+-rw-r--r--   0 vinh      (1000) vinh      (1000)    19241 2020-08-16 10:14:26.000000 skorch-0.9.0/skorch/utils.py
+drwxr-xr-x   0 vinh      (1000) vinh      (1000)        0 2020-08-30 10:43:14.000000 skorch-0.9.0/skorch.egg-info/
+-rw-r--r--   0 vinh      (1000) vinh      (1000)    10061 2020-08-30 10:43:14.000000 skorch-0.9.0/skorch.egg-info/PKG-INFO
+-rw-r--r--   0 vinh      (1000) vinh      (1000)     1065 2020-08-30 10:43:14.000000 skorch-0.9.0/skorch.egg-info/SOURCES.txt
+-rw-r--r--   0 vinh      (1000) vinh      (1000)        1 2020-08-30 10:43:14.000000 skorch-0.9.0/skorch.egg-info/dependency_links.txt
+-rw-r--r--   0 vinh      (1000) vinh      (1000)        1 2020-04-12 16:28:14.000000 skorch-0.9.0/skorch.egg-info/not-zip-safe
+-rw-r--r--   0 vinh      (1000) vinh      (1000)      147 2020-08-30 10:43:14.000000 skorch-0.9.0/skorch.egg-info/requires.txt
+-rw-r--r--   0 vinh      (1000) vinh      (1000)        7 2020-08-30 10:43:14.000000 skorch-0.9.0/skorch.egg-info/top_level.txt
```

### Comparing `skorch-0.8.0/LICENSE` & `skorch-0.9.0/LICENSE`

 * *Files identical despite different names*

### Comparing `skorch-0.8.0/PKG-INFO` & `skorch-0.9.0/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: skorch
-Version: 0.8.0
+Version: 0.9.0
 Summary: scikit-learn compatible neural network library for pytorch
 Home-page: https://github.com/skorch-dev/skorch
 License: new BSD 3-Clause
 Description: .. image:: https://github.com/skorch-dev/skorch/blob/master/assets/skorch.svg
            :width: 30%
         
         ------------
@@ -47,53 +47,53 @@
         <https://github.com/skorch-dev/skorch/tree/master/notebooks/README.md>`__.
         
         .. code:: python
         
             import numpy as np
             from sklearn.datasets import make_classification
             from torch import nn
-            import torch.nn.functional as F
         
             from skorch import NeuralNetClassifier
         
         
             X, y = make_classification(1000, 20, n_informative=10, random_state=0)
             X = X.astype(np.float32)
             y = y.astype(np.int64)
         
             class MyModule(nn.Module):
-                def __init__(self, num_units=10, nonlin=F.relu):
+                def __init__(self, num_units=10, nonlin=nn.ReLU()):
                     super(MyModule, self).__init__()
         
                     self.dense0 = nn.Linear(20, num_units)
                     self.nonlin = nonlin
                     self.dropout = nn.Dropout(0.5)
-                    self.dense1 = nn.Linear(num_units, 10)
-                    self.output = nn.Linear(10, 2)
+                    self.dense1 = nn.Linear(num_units, num_units)
+                    self.output = nn.Linear(num_units, 2)
+                    self.softmax = nn.Softmax(dim=-1)
         
                 def forward(self, X, **kwargs):
                     X = self.nonlin(self.dense0(X))
                     X = self.dropout(X)
-                    X = F.relu(self.dense1(X))
-                    X = F.softmax(self.output(X), dim=-1)
+                    X = self.nonlin(self.dense1(X))
+                    X = self.softmax(self.output(X))
                     return X
         
         
             net = NeuralNetClassifier(
                 MyModule,
                 max_epochs=10,
                 lr=0.1,
                 # Shuffle training data on each epoch
                 iterator_train__shuffle=True,
             )
         
             net.fit(X, y)
             y_proba = net.predict_proba(X)
         
-        In an sklearn Pipeline:
+        In an `sklearn Pipeline <https://scikit-learn.org/stable/modules/generated/sklearn.pipeline.Pipeline.html>`_:
         
         .. code:: python
         
             from sklearn.pipeline import Pipeline
             from sklearn.preprocessing import StandardScaler
         
         
@@ -101,30 +101,33 @@
                 ('scale', StandardScaler()),
                 ('net', net),
             ])
         
             pipe.fit(X, y)
             y_proba = pipe.predict_proba(X)
         
-        With grid search
+        With `grid search <https://scikit-learn.org/stable/modules/generated/sklearn.model_selection.GridSearchCV.html>`_:
         
         .. code:: python
         
             from sklearn.model_selection import GridSearchCV
         
         
+            # deactivate skorch-internal train-valid split and verbose logging
+            net.set_params(train_split=False, verbose=0)
             params = {
                 'lr': [0.01, 0.02],
                 'max_epochs': [10, 20],
                 'module__num_units': [10, 20],
             }
-            gs = GridSearchCV(net, params, refit=False, cv=3, scoring='accuracy')
+            gs = GridSearchCV(net, params, refit=False, cv=3, scoring='accuracy', verbose=2)
         
             gs.fit(X, y)
-            print(gs.best_score_, gs.best_params_)
+            print("best score: {:.3f}, best params: {}".format(gs.best_score_, gs.best_params_))
+        
         
         skorch also provides many convenient features, among others:
         
         - `Learning rate schedulers <https://skorch.readthedocs.io/en/stable/callbacks.html#skorch.callbacks.LRScheduler>`_ (Warm restarts, cyclic LR and many more)
         - `Scoring using sklearn (and custom) scoring functions <https://skorch.readthedocs.io/en/stable/callbacks.html#skorch.callbacks.EpochScoring>`_
         - `Early stopping <https://skorch.readthedocs.io/en/stable/callbacks.html#skorch.callbacks.EarlyStopping>`_
         - `Checkpointing <https://skorch.readthedocs.io/en/stable/callbacks.html#skorch.callbacks.Checkpoint>`_
@@ -134,124 +137,130 @@
         
         ============
         Installation
         ============
         
         skorch requires Python 3.5 or higher.
         
+        conda installation
+        ==================
+        
+        You need a working conda installation. Get the correct miniconda for
+        your system from `here <https://conda.io/miniconda.html>`__.
+        
+        To install skorch, you need to use the conda-forge channel:
+        
+        .. code:: bash
+        
+            conda install -c conda-forge skorch
+        
+        We recommend to use a `conda virtual environment <https://docs.conda.io/projects/conda/en/latest/user-guide/tasks/manage-environments.html>`_.
+        
+        **Note**: The conda channel is *not* managed by the skorch
+        maintainers. More information is available `here
+        <https://github.com/conda-forge/skorch-feedstock>`__.
+        
         pip installation
         ================
         
         To install with pip, run:
         
         .. code:: bash
         
             pip install -U skorch
         
-        We recommend to use a virtual environment for this.
+        Again, we recommend to use a `virtual environment
+        <https://docs.python.org/3/tutorial/venv.html>`_ for this.
         
         From source
         ===========
         
-        If you would like to use the must recent additions to skorch or
-        help development, you should install skorch from source:
-        
-        .. code:: bash
-        
-            git clone https://github.com/skorch-dev/skorch.git
-            cd skorch
-            # install pytorch version for your system (see below)
-            python setup.py install
+        If you would like to use the most recent additions to skorch or
+        help development, you should install skorch from source.
         
         Using conda
-        ===========
+        -----------
         
-        You need a working conda installation. Get the correct miniconda for
-        your system from `here <https://conda.io/miniconda.html>`__.
-        
-        You can also install skorch through the conda-forge channel. 
-        The instructions for doing so are 
-        available `here <https://github.com/conda-forge/skorch-feedstock>`__.
-        **Note**: The conda channel is _not_ managed by the skorch maintainers.
-        
-        If you do not want to use conda-forge, you may install skorch using:
+        To install skorch from source using conda, proceed as follows:
         
         .. code:: bash
         
             git clone https://github.com/skorch-dev/skorch.git
             cd skorch
             conda env create
             source activate skorch
-            # install pytorch version for your system (see below)
-            python setup.py install
+            pip install .
         
         If you want to help developing, run:
         
         .. code:: bash
         
             git clone https://github.com/skorch-dev/skorch.git
             cd skorch
             conda env create
             source activate skorch
-            # install pytorch version for your system (see below)
-            conda install -c conda-forge --file requirements-dev.txt
-            python setup.py develop
+            pip install -e .
         
             py.test  # unit tests
             pylint skorch  # static code checks
         
         Using pip
-        =========
+        ---------
         
-        If you just want to use skorch, use:
+        For pip, follow these instructions instead:
         
         .. code:: bash
         
             git clone https://github.com/skorch-dev/skorch.git
             cd skorch
             # create and activate a virtual environment
             pip install -r requirements.txt
             # install pytorch version for your system (see below)
-            python setup.py install
+            pip install .
         
         If you want to help developing, run:
         
         .. code:: bash
         
             git clone https://github.com/skorch-dev/skorch.git
             cd skorch
             # create and activate a virtual environment
             pip install -r requirements.txt
             # install pytorch version for your system (see below)
             pip install -r requirements-dev.txt
-            python setup.py develop
+            pip install -e .
         
             py.test  # unit tests
             pylint skorch  # static code checks
         
         PyTorch
         =======
         
         PyTorch is not covered by the dependencies, since the PyTorch version
-        you need is dependent on your system. For installation instructions
-        for PyTorch, visit the `PyTorch website
-        <http://pytorch.org/>`__. skorch officially supports the following
-        PyTorch versions:
+        you need is dependent on your OS and device. For installation
+        instructions for PyTorch, visit the `PyTorch website
+        <http://pytorch.org/>`__. skorch officially supports the last four
+        minor PyTorch versions, which currently are:
         
-        - 1.1.0
-        - 1.2.0
         - 1.3.1
         - 1.4.0
+        - 1.5.1
+        - 1.6.0
+        
+        However, that doesn't mean that older versions don't work, just that
+        they aren't tested. Since skorch mostly relies on the stable part of
+        the PyTorch API, older PyTorch versions should work fine.
         
-        In general, this should work (assuming CUDA 9):
+        In general, running this to install PyTorch should work (assuming CUDA
+        10.2):
         
         .. code:: bash
         
             # using conda:
-            conda install pytorch cudatoolkit=9.0 -c pytorch
+            conda install pytorch cudatoolkit==10.2 -c pytorch
             # using pip
             pip install torch
         
         =============
         Communication
         =============
```

### Comparing `skorch-0.8.0/README.rst` & `skorch-0.9.0/README.rst`

 * *Files 7% similar despite different names*

```diff
@@ -41,53 +41,53 @@
 <https://github.com/skorch-dev/skorch/tree/master/notebooks/README.md>`__.
 
 .. code:: python
 
     import numpy as np
     from sklearn.datasets import make_classification
     from torch import nn
-    import torch.nn.functional as F
 
     from skorch import NeuralNetClassifier
 
 
     X, y = make_classification(1000, 20, n_informative=10, random_state=0)
     X = X.astype(np.float32)
     y = y.astype(np.int64)
 
     class MyModule(nn.Module):
-        def __init__(self, num_units=10, nonlin=F.relu):
+        def __init__(self, num_units=10, nonlin=nn.ReLU()):
             super(MyModule, self).__init__()
 
             self.dense0 = nn.Linear(20, num_units)
             self.nonlin = nonlin
             self.dropout = nn.Dropout(0.5)
-            self.dense1 = nn.Linear(num_units, 10)
-            self.output = nn.Linear(10, 2)
+            self.dense1 = nn.Linear(num_units, num_units)
+            self.output = nn.Linear(num_units, 2)
+            self.softmax = nn.Softmax(dim=-1)
 
         def forward(self, X, **kwargs):
             X = self.nonlin(self.dense0(X))
             X = self.dropout(X)
-            X = F.relu(self.dense1(X))
-            X = F.softmax(self.output(X), dim=-1)
+            X = self.nonlin(self.dense1(X))
+            X = self.softmax(self.output(X))
             return X
 
 
     net = NeuralNetClassifier(
         MyModule,
         max_epochs=10,
         lr=0.1,
         # Shuffle training data on each epoch
         iterator_train__shuffle=True,
     )
 
     net.fit(X, y)
     y_proba = net.predict_proba(X)
 
-In an sklearn Pipeline:
+In an `sklearn Pipeline <https://scikit-learn.org/stable/modules/generated/sklearn.pipeline.Pipeline.html>`_:
 
 .. code:: python
 
     from sklearn.pipeline import Pipeline
     from sklearn.preprocessing import StandardScaler
 
 
@@ -95,30 +95,33 @@
         ('scale', StandardScaler()),
         ('net', net),
     ])
 
     pipe.fit(X, y)
     y_proba = pipe.predict_proba(X)
 
-With grid search
+With `grid search <https://scikit-learn.org/stable/modules/generated/sklearn.model_selection.GridSearchCV.html>`_:
 
 .. code:: python
 
     from sklearn.model_selection import GridSearchCV
 
 
+    # deactivate skorch-internal train-valid split and verbose logging
+    net.set_params(train_split=False, verbose=0)
     params = {
         'lr': [0.01, 0.02],
         'max_epochs': [10, 20],
         'module__num_units': [10, 20],
     }
-    gs = GridSearchCV(net, params, refit=False, cv=3, scoring='accuracy')
+    gs = GridSearchCV(net, params, refit=False, cv=3, scoring='accuracy', verbose=2)
 
     gs.fit(X, y)
-    print(gs.best_score_, gs.best_params_)
+    print("best score: {:.3f}, best params: {}".format(gs.best_score_, gs.best_params_))
+
 
 skorch also provides many convenient features, among others:
 
 - `Learning rate schedulers <https://skorch.readthedocs.io/en/stable/callbacks.html#skorch.callbacks.LRScheduler>`_ (Warm restarts, cyclic LR and many more)
 - `Scoring using sklearn (and custom) scoring functions <https://skorch.readthedocs.io/en/stable/callbacks.html#skorch.callbacks.EpochScoring>`_
 - `Early stopping <https://skorch.readthedocs.io/en/stable/callbacks.html#skorch.callbacks.EarlyStopping>`_
 - `Checkpointing <https://skorch.readthedocs.io/en/stable/callbacks.html#skorch.callbacks.Checkpoint>`_
@@ -128,124 +131,130 @@
 
 ============
 Installation
 ============
 
 skorch requires Python 3.5 or higher.
 
+conda installation
+==================
+
+You need a working conda installation. Get the correct miniconda for
+your system from `here <https://conda.io/miniconda.html>`__.
+
+To install skorch, you need to use the conda-forge channel:
+
+.. code:: bash
+
+    conda install -c conda-forge skorch
+
+We recommend to use a `conda virtual environment <https://docs.conda.io/projects/conda/en/latest/user-guide/tasks/manage-environments.html>`_.
+
+**Note**: The conda channel is *not* managed by the skorch
+maintainers. More information is available `here
+<https://github.com/conda-forge/skorch-feedstock>`__.
+
 pip installation
 ================
 
 To install with pip, run:
 
 .. code:: bash
 
     pip install -U skorch
 
-We recommend to use a virtual environment for this.
+Again, we recommend to use a `virtual environment
+<https://docs.python.org/3/tutorial/venv.html>`_ for this.
 
 From source
 ===========
 
-If you would like to use the must recent additions to skorch or
-help development, you should install skorch from source:
-
-.. code:: bash
-
-    git clone https://github.com/skorch-dev/skorch.git
-    cd skorch
-    # install pytorch version for your system (see below)
-    python setup.py install
+If you would like to use the most recent additions to skorch or
+help development, you should install skorch from source.
 
 Using conda
-===========
-
-You need a working conda installation. Get the correct miniconda for
-your system from `here <https://conda.io/miniconda.html>`__.
-
-You can also install skorch through the conda-forge channel. 
-The instructions for doing so are 
-available `here <https://github.com/conda-forge/skorch-feedstock>`__.
-**Note**: The conda channel is _not_ managed by the skorch maintainers.
+-----------
 
-If you do not want to use conda-forge, you may install skorch using:
+To install skorch from source using conda, proceed as follows:
 
 .. code:: bash
 
     git clone https://github.com/skorch-dev/skorch.git
     cd skorch
     conda env create
     source activate skorch
-    # install pytorch version for your system (see below)
-    python setup.py install
+    pip install .
 
 If you want to help developing, run:
 
 .. code:: bash
 
     git clone https://github.com/skorch-dev/skorch.git
     cd skorch
     conda env create
     source activate skorch
-    # install pytorch version for your system (see below)
-    conda install -c conda-forge --file requirements-dev.txt
-    python setup.py develop
+    pip install -e .
 
     py.test  # unit tests
     pylint skorch  # static code checks
 
 Using pip
-=========
+---------
 
-If you just want to use skorch, use:
+For pip, follow these instructions instead:
 
 .. code:: bash
 
     git clone https://github.com/skorch-dev/skorch.git
     cd skorch
     # create and activate a virtual environment
     pip install -r requirements.txt
     # install pytorch version for your system (see below)
-    python setup.py install
+    pip install .
 
 If you want to help developing, run:
 
 .. code:: bash
 
     git clone https://github.com/skorch-dev/skorch.git
     cd skorch
     # create and activate a virtual environment
     pip install -r requirements.txt
     # install pytorch version for your system (see below)
     pip install -r requirements-dev.txt
-    python setup.py develop
+    pip install -e .
 
     py.test  # unit tests
     pylint skorch  # static code checks
 
 PyTorch
 =======
 
 PyTorch is not covered by the dependencies, since the PyTorch version
-you need is dependent on your system. For installation instructions
-for PyTorch, visit the `PyTorch website
-<http://pytorch.org/>`__. skorch officially supports the following
-PyTorch versions:
+you need is dependent on your OS and device. For installation
+instructions for PyTorch, visit the `PyTorch website
+<http://pytorch.org/>`__. skorch officially supports the last four
+minor PyTorch versions, which currently are:
 
-- 1.1.0
-- 1.2.0
 - 1.3.1
 - 1.4.0
+- 1.5.1
+- 1.6.0
+
+However, that doesn't mean that older versions don't work, just that
+they aren't tested. Since skorch mostly relies on the stable part of
+the PyTorch API, older PyTorch versions should work fine.
 
-In general, this should work (assuming CUDA 9):
+In general, running this to install PyTorch should work (assuming CUDA
+10.2):
 
 .. code:: bash
 
     # using conda:
-    conda install pytorch cudatoolkit=9.0 -c pytorch
+    conda install pytorch cudatoolkit==10.2 -c pytorch
     # using pip
     pip install torch
 
 =============
 Communication
 =============
```

### Comparing `skorch-0.8.0/setup.py` & `skorch-0.9.0/setup.py`

 * *Files identical despite different names*

### Comparing `skorch-0.8.0/skorch/__init__.py` & `skorch-0.9.0/skorch/__init__.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,22 +1,34 @@
 """skorch base imports"""
 
+import sys
+import warnings
+
 import pkg_resources
 from pkg_resources import parse_version
 
 from .history import History
 from .net import NeuralNet
 from .classifier import NeuralNetClassifier
 from .classifier import NeuralNetBinaryClassifier
 from .regressor import NeuralNetRegressor
 from . import callbacks
 
 
 MIN_TORCH_VERSION = '1.1.0'
 
+
+# TODO: remove in skorch 0.10.0
+if sys.version_info < (3, 6):
+    warnings.warn(
+        "Official support for Python 3.5 will be dropped starting from "
+        "skorch version 0.10.0",
+        FutureWarning,
+    )
+
 try:
     # pylint: disable=wrong-import-position
     import torch
 except ModuleNotFoundError:
     raise ModuleNotFoundError(
         "No module named 'torch', and skorch depends on PyTorch "
         "(aka 'torch'). "
```

### Comparing `skorch-0.8.0/skorch/callbacks/__init__.py` & `skorch-0.9.0/skorch/callbacks/__init__.py`

 * *Files identical despite different names*

### Comparing `skorch-0.8.0/skorch/callbacks/base.py` & `skorch-0.9.0/skorch/callbacks/base.py`

 * *Files identical despite different names*

### Comparing `skorch-0.8.0/skorch/callbacks/logging.py` & `skorch-0.9.0/skorch/callbacks/logging.py`

 * *Files 2% similar despite different names*

```diff
@@ -552,16 +552,16 @@
                 postfix[key] = net.history[-1, 'batches', -1, key]
             except KeyError:
                 pass
         return postfix
 
     # pylint: disable=attribute-defined-outside-init
     def on_batch_end(self, net, **kwargs):
-        self.pbar.set_postfix(self._get_postfix_dict(net), refresh=False)
-        self.pbar.update()
+        self.pbar_.set_postfix(self._get_postfix_dict(net), refresh=False)
+        self.pbar_.update()
 
     # pylint: disable=attribute-defined-outside-init, arguments-differ
     def on_epoch_begin(self, net, dataset_train=None, dataset_valid=None, **kwargs):
         # Assume it is a number until proven otherwise.
         batches_per_epoch = self.batches_per_epoch
 
         if self.batches_per_epoch == 'auto':
@@ -572,20 +572,27 @@
             if len(net.history) <= 1:
                 # No limit is known until the end of the first epoch.
                 batches_per_epoch = None
             else:
                 batches_per_epoch = len(net.history[-2, 'batches'])
 
         if self._use_notebook():
-            self.pbar = tqdm.tqdm_notebook(total=batches_per_epoch, leave=False)
+            self.pbar_ = tqdm.tqdm_notebook(total=batches_per_epoch, leave=False)
         else:
-            self.pbar = tqdm.tqdm(total=batches_per_epoch, leave=False)
+            self.pbar_ = tqdm.tqdm(total=batches_per_epoch, leave=False)
 
     def on_epoch_end(self, net, **kwargs):
-        self.pbar.close()
+        self.pbar_.close()
+
+    def __getstate__(self):
+        # don't save away the temporary pbar_ object which gets created on
+        # epoch begin anew anyway. This avoids pickling errors with tqdm.
+        state = self.__dict__.copy()
+        del state['pbar_']
+        return state
 
 
 def rename_tensorboard_key(key):
     """Rename keys from history to keys in TensorBoard
 
     Specifically, prefixes all names with "Loss/" if they seem to be
     losses.
```

### Comparing `skorch-0.8.0/skorch/callbacks/lr_scheduler.py` & `skorch-0.9.0/skorch/callbacks/lr_scheduler.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,34 +1,35 @@
 """Contains learning rate scheduler callbacks"""
 
 import sys
 
 # pylint: disable=unused-import
+import warnings
+
 import numpy as np
 import torch
 from torch.optim.lr_scheduler import _LRScheduler
 from torch.optim.lr_scheduler import CosineAnnealingLR
 from torch.optim.lr_scheduler import ExponentialLR
 from torch.optim.lr_scheduler import LambdaLR
 from torch.optim.lr_scheduler import MultiStepLR
 from torch.optim.lr_scheduler import ReduceLROnPlateau
 from torch.optim.lr_scheduler import StepLR
+
 try:
     from torch.optim.lr_scheduler import CyclicLR as TorchCyclicLR
 except ImportError:
     # Backward compatibility with torch >= 1.0 && < 1.1
     TorchCyclicLR = None
 from torch.optim.optimizer import Optimizer
 from skorch.callbacks import Callback
 
-
 __all__ = ['LRScheduler', 'WarmRestartLR']
 
 
-
 def _check_lr(name, optimizer, lr):
     """Return one learning rate for each param group."""
     n = len(optimizer.param_groups)
     if not isinstance(lr, (list, tuple)):
         return lr * np.ones(n)
 
     if len(lr) != n:
@@ -49,22 +50,38 @@
 
     monitor : str or callable (default=None)
       Value of the history to monitor or function/callable. In
       the latter case, the callable receives the net instance as
       argument and is expected to return the score (float) used to
       determine the learning rate adjustment.
 
+    event_name: str, (default='event_lr')
+      Name of event to be placed in history when the scheduler takes a step.
+      Pass ``None`` to disable placing events in history.
+      **Note:** This feature works only for pytorch version >=1.4
+
+    step_every: str, (default='epoch')
+      Value for when to apply the learning scheduler step. Can be either 'batch'
+       or 'epoch'.
+
     kwargs
       Additional arguments passed to the lr scheduler.
 
     """
 
-    def __init__(self, policy='WarmRestartLR', monitor='train_loss', **kwargs):
+    def __init__(self,
+                 policy='WarmRestartLR',
+                 monitor='train_loss',
+                 event_name="event_lr",
+                 step_every='epoch',
+                 **kwargs):
         self.policy = policy
         self.monitor = monitor
+        self.event_name = event_name
+        self.step_every = step_every
         vars(self).update(kwargs)
 
     def simulate(self, steps, initial_lr):
         """
         Simulates the learning rate scheduler.
 
         Parameters
@@ -82,43 +99,49 @@
 
         """
         test = torch.ones(1, requires_grad=True)
         opt = torch.optim.SGD([{'params': test, 'lr': initial_lr}])
         policy_cls = self._get_policy_cls()
         sch = policy_cls(opt, **self.kwargs)
 
-        if hasattr(sch, 'batch_step') and callable(sch.batch_step):
-            step = sch.batch_step
-        else:
-            step = sch.step
         lrs = []
         for _ in range(steps):
-            opt.step() # suppress warning about .step call order
+            opt.step()  # suppress warning about .step call order
             lrs.append(opt.param_groups[0]['lr'])
-            step()
+            sch.step()
 
         return np.array(lrs)
 
     def initialize(self):
         self.policy_ = self._get_policy_cls()
         self.lr_scheduler_ = None
         self.batch_idx_ = 0
+        # TODO: Remove this warning on 0.10 release
+        if (self.policy_ == TorchCyclicLR or self.policy_ == "TorchCyclicLR"
+                and self.step_every == 'epoch'):
+            warnings.warn(
+                "The LRScheduler now makes a step every epoch by default. "
+                "To have the cyclic lr scheduler update "
+                "every batch set step_every='batch'",
+                FutureWarning
+            )
+
         return self
 
     def _get_policy_cls(self):
         if isinstance(self.policy, str):
             return getattr(sys.modules[__name__], self.policy)
         return self.policy
 
     @property
     def kwargs(self):
         # These are the parameters that are passed to the
         # scheduler. Parameters that don't belong there must be
         # excluded.
-        excluded = ('policy', 'monitor')
+        excluded = ('policy', 'monitor', 'event_name', 'step_every')
         kwargs = {key: val for key, val in vars(self).items()
                   if not (key in excluded or key.endswith('_'))}
         return kwargs
 
     def on_train_begin(self, net, **kwargs):
         if net.history:
             try:
@@ -126,50 +149,53 @@
             except KeyError:
                 self.batch_idx_ = sum(len(b) for b in net.history[:, 'batches'])
         self.lr_scheduler_ = self._get_scheduler(
             net, self.policy_, **self.kwargs
         )
 
     def on_epoch_end(self, net, **kwargs):
-        epoch = len(net.history) - 1
+        if not self.step_every == 'epoch':
+            return
+        epoch = len(net.history)
         if isinstance(self.lr_scheduler_, ReduceLROnPlateau):
             if callable(self.monitor):
                 score = self.monitor(net)
             else:
-                if epoch:
-                    score = net.history[-2, self.monitor]
+                if self.lr_scheduler_.mode == 'max':
+                    score = -np.inf
+                elif self.lr_scheduler_.mode == 'min':
+                    score = np.inf
                 else:
-                    if self.lr_scheduler_.mode == 'max':
-                        score = -np.inf
-                    else:
-                        score = np.inf
+                    score = net.history[-1, self.monitor]
+
             self.lr_scheduler_.step(score, epoch)
+            # ReduceLROnPlateau does not expose the current lr so it can't be recorded
         else:
+            if self.event_name is not None and hasattr(
+                    self.lr_scheduler_, "get_last_lr"):
+                net.history.record(self.event_name,
+                                   self.lr_scheduler_.get_last_lr()[0])
             self.lr_scheduler_.step(epoch)
 
     def on_batch_end(self, net, training, **kwargs):
-        if (
-                training and
-                hasattr(self.lr_scheduler_, 'batch_step') and
-                callable(self.lr_scheduler_.batch_step)
-        ):
-            self.lr_scheduler_.batch_step(self.batch_idx_)
-
-        if TorchCyclicLR and isinstance(self.lr_scheduler_, TorchCyclicLR):
-            self.lr_scheduler_.step(self.batch_idx_)
-
-        if training:
-            self.batch_idx_ += 1
+        if not training or not self.step_every == 'batch':
+            return
+        if self.event_name is not None and hasattr(
+                self.lr_scheduler_, "get_last_lr"):
+            net.history.record_batch(self.event_name,
+                                     self.lr_scheduler_.get_last_lr()[0])
+        self.lr_scheduler_.step()
+        self.batch_idx_ += 1
 
     def _get_scheduler(self, net, policy, **scheduler_kwargs):
         """Return scheduler, based on indicated policy, with appropriate
         parameters.
         """
         if policy not in [ReduceLROnPlateau] and \
-           'last_epoch' not in scheduler_kwargs:
+                'last_epoch' not in scheduler_kwargs:
             last_epoch = len(net.history) - 1
             scheduler_kwargs['last_epoch'] = last_epoch
 
         return policy(net.optimizer_, **scheduler_kwargs)
 
 
 class WarmRestartLR(_LRScheduler):
@@ -214,23 +240,24 @@
     def __init__(
             self, optimizer,
             min_lr=1e-6,
             max_lr=0.05,
             base_period=10,
             period_mult=2,
             last_epoch=-1
-        ):
+    ):
         self.min_lr = _check_lr('min_lr', optimizer, min_lr)
         self.max_lr = _check_lr('max_lr', optimizer, max_lr)
         self.base_period = base_period
         self.period_mult = period_mult
         super(WarmRestartLR, self).__init__(optimizer, last_epoch)
 
     def _get_current_lr(self, min_lr, max_lr, period, epoch):
-        return min_lr + 0.5*(max_lr-min_lr)*(1+ np.cos(epoch * np.pi/period))
+        return min_lr + 0.5 * (max_lr - min_lr) * (
+                1 + np.cos(epoch * np.pi / period))
 
     def get_lr(self):
         epoch_idx = float(self.last_epoch)
         current_period = float(self.base_period)
         while epoch_idx / current_period > 1.0:
             epoch_idx -= current_period + 1
             current_period *= self.period_mult
```

### Comparing `skorch-0.8.0/skorch/callbacks/regularization.py` & `skorch-0.9.0/skorch/callbacks/regularization.py`

 * *Files identical despite different names*

### Comparing `skorch-0.8.0/skorch/callbacks/scoring.py` & `skorch-0.9.0/skorch/callbacks/scoring.py`

 * *Files identical despite different names*

### Comparing `skorch-0.8.0/skorch/callbacks/training.py` & `skorch-0.9.0/skorch/callbacks/training.py`

 * *Files 7% similar despite different names*

```diff
@@ -7,14 +7,15 @@
 from fnmatch import fnmatch
 from functools import partial
 from itertools import product
 
 import numpy as np
 from skorch.callbacks import Callback
 from skorch.exceptions import SkorchException
+from skorch.utils import _check_f_arguments
 from skorch.utils import noop
 from skorch.utils import open_file_like
 from skorch.utils import freeze_parameter
 from skorch.utils import unfreeze_parameter
 
 
 __all__ = ['Checkpoint', 'EarlyStopping', 'ParamMapper', 'Freezer',
@@ -33,17 +34,21 @@
     callback that dynamically evaluates whether the model should
     be saved in this epoch.
 
     Some or all of the following can be saved:
 
       - model parameters (see ``f_params`` parameter);
       - optimizer state (see ``f_optimizer`` parameter);
+      - criterion state (see ``f_criterion`` parameter);
       - training history (see ``f_history`` parameter);
       - entire model object (see ``f_pickle`` parameter).
 
+    If you've created a custom module, e.g. ``net.mymodule_``, you
+    can save that as well by passing ``f_mymodule``.
+
     You can implement your own save protocol by subclassing
     ``Checkpoint`` and overriding :func:`~Checkpoint.save_model`.
 
     This callback writes a bool flag to the history column
     ``event_cp`` indicating whether a checkpoint was created or not.
 
     Example:
@@ -88,14 +93,21 @@
     f_optimizer : file-like object, str, None (default='optimizer.pt')
       File path to the file or file-like object where the optimizer
       state should be saved. Pass ``None`` to disable saving
       model parameters.
 
       Supports the same format specifiers as ``f_params``.
 
+    f_criterion : file-like object, str, None (default='criterion.pt')
+      File path to the file or file-like object where the criterion
+      state should be saved. Pass ``None`` to disable saving
+      model parameters.
+
+      Supports the same format specifiers as ``f_params``.
+
     f_history : file-like object, str, None (default='history.json')
       File path to the file or file-like object where the model
       training history should be saved. Pass ``None`` to disable
       saving history.
 
     f_pickle : file-like object, str, None (default=None)
       File path to the file or file-like object where the entire
@@ -122,32 +134,44 @@
 
     """
     def __init__(
             self,
             monitor='valid_loss_best',
             f_params='params.pt',
             f_optimizer='optimizer.pt',
+            f_criterion='criterion.pt',
             f_history='history.json',
             f_pickle=None,
             fn_prefix='',
             dirname='',
             event_name='event_cp',
             sink=noop,
+            **kwargs
     ):
         self.monitor = monitor
         self.f_params = f_params
         self.f_optimizer = f_optimizer
+        self.f_criterion = f_criterion
         self.f_history = f_history
         self.f_pickle = f_pickle
         self.fn_prefix = fn_prefix
         self.dirname = dirname
         self.event_name = event_name
         self.sink = sink
+        self._check_kwargs(kwargs)
+        vars(self).update(**kwargs)
         self._validate_filenames()
 
+    def _check_kwargs(self, kwargs):
+        for key in kwargs:
+            if not key.startswith('f_'):
+                raise TypeError(
+                    "{cls_name} got an unexpected argument '{key}', did you mean "
+                    "'f_{key}'?".format(cls_name=self.__class__.__name__, key=key))
+
     def initialize(self):
         self._validate_filenames()
         if self.dirname and not os.path.exists(self.dirname):
             os.makedirs(self.dirname, exist_ok=True)
         return self
 
     def on_epoch_end(self, net, **kwargs):
@@ -175,38 +199,50 @@
 
         if do_checkpoint:
             self.save_model(net)
             self._sink("A checkpoint was triggered in epoch {}.".format(
                 len(net.history) + 1
             ), net.verbose)
 
+    def _f_kwargs(self):
+        return {key: getattr(self, key) for key in dir(self)
+                if key.startswith('f_') and (key != 'f_history_')}
+
     def save_model(self, net):
         """Save the model.
 
         This function saves some or all of the following:
 
           - model parameters;
           - optimizer state;
+          - criterion state;
           - training history;
+          - custom modules;
           - entire model object.
+
         """
-        if self.f_params is not None:
-            f = self._format_target(net, self.f_params, -1)
-            self._save_params(f, net, "f_params", "model parameters")
-
-        if self.f_optimizer is not None:
-            f = self._format_target(net, self.f_optimizer, -1)
-            self._save_params(f, net, "f_optimizer", "optimizer state")
+        kwargs_module, kwargs_other = _check_f_arguments(
+            self.__class__.__name__, **self._f_kwargs())
 
-        if self.f_history is not None:
+        for key, val in kwargs_module.items():
+            if val is None:
+                continue
+
+            f = self._format_target(net, val, -1)
+            key = key[:-1]  # remove trailing '_'
+            self._save_params(f, net, 'f_' + key, key + " state")
+
+        f_history = kwargs_other.get('f_history')
+        if f_history is not None:
             f = self.f_history_
             self._save_params(f, net, "f_history", "history")
 
-        if self.f_pickle:
-            f_pickle = self._format_target(net, self.f_pickle, -1)
+        f_pickle = kwargs_other.get('f_pickle')
+        if f_pickle:
+            f_pickle = self._format_target(net, f_pickle, -1)
             with open_file_like(f_pickle, 'wb') as f:
                 pickle.dump(net, f)
 
     @property
     def f_history_(self):
         # This is a property and not in initialize to allow ``NeuralNet``
         # to call ``load_params`` without needing the checkpoint to
@@ -222,20 +258,17 @@
         if (
                 self.event_name is not None and
                 net.history
         ):
             for i, v in enumerate(net.history[:, self.event_name]):
                 if v:
                     idx = i
-        return {
-            "f_params": self._format_target(net, self.f_params, idx),
-            "f_optimizer": self._format_target(net, self.f_optimizer, idx),
-            "f_history": self.f_history_,
-            "f_pickle": self._format_target(net, self.f_pickle, idx)
-        }
+
+        return {key: self._format_target(net, val, idx) for key, val
+                in self._f_kwargs().items()}
 
     def _save_params(self, f, net, f_name, log_name):
         try:
             net.save_params(**{f_name: f})
         except Exception as e:  # pylint: disable=broad-except
             self._sink(
                 "Unable to save {} to {}, {}: {}".format(
@@ -257,26 +290,23 @@
     def _validate_filenames(self):
         """Checks if passed filenames are valid.
 
         Specifically, f_* parameter should not be passed in
         conjunction with dirname.
 
         """
+        _check_f_arguments(self.__class__.__name__, **self._f_kwargs())
+
         if not self.dirname:
             return
 
         def _is_truthy_and_not_str(f):
             return f and not isinstance(f, str)
 
-        if (
-                _is_truthy_and_not_str(self.f_optimizer) or
-                _is_truthy_and_not_str(self.f_params) or
-                _is_truthy_and_not_str(self.f_history) or
-                _is_truthy_and_not_str(self.f_pickle)
-        ):
+        if any(_is_truthy_and_not_str(val) for val in self._f_kwargs().values()):
             raise SkorchException(
                 'dirname can only be used when f_* are strings')
 
     def _sink(self, text, verbose):
         #  We do not want to be affected by verbosity if sink is not print
         if (self.sink is not print) or verbose:
             self.sink(text)
@@ -629,14 +659,21 @@
     f_optimizer : file-like object, str, None (default='optimizer.pt')
       File path to the file or file-like object where the optimizer
       state should be saved. Pass ``None`` to disable saving
       model parameters.
 
       Supports the same format specifiers as ``f_params``.
 
+    f_criterion : file-like object, str, None (default='criterion.pt')
+      File path to the file or file-like object where the criterion
+      state should be saved. Pass ``None`` to disable saving
+      model parameters.
+
+      Supports the same format specifiers as ``f_params``.
+
     f_history : file-like object, str, None (default='history.json')
       File path to the file or file-like object where the model
       training history should be saved. Pass ``None`` to disable
       saving history.
 
     f_pickle : file-like object, str, None (default=None)
       File path to the file or file-like object where the entire
@@ -652,44 +689,52 @@
     dirname: str (default='')
       Directory where files are stored.
 
     sink : callable (default=noop)
       The target that the information about created checkpoints is
       sent to. This can be a logger or ``print`` function (to send to
       stdout). By default the output is discarded.
+
     """
     def __init__(
             self,
             f_params='params.pt',
             f_optimizer='optimizer.pt',
+            f_criterion='criterion.pt',
             f_history='history.json',
             f_pickle=None,
             fn_prefix='train_end_',
             dirname='',
             sink=noop,
+            **kwargs
     ):
         self.f_params = f_params
         self.f_optimizer = f_optimizer
+        self.f_criterion = f_criterion
         self.f_history = f_history
         self.f_pickle = f_pickle
         self.fn_prefix = fn_prefix
         self.dirname = dirname
         self.sink = sink
+        Checkpoint._check_kwargs(self, kwargs)
+        vars(self).update(**kwargs)
+
+    def _f_kwargs(self):
+        return {name: getattr(self, name) for name in dir(self)
+                if name.startswith('f_')}
 
     def initialize(self):
         self.checkpoint_ = Checkpoint(
             monitor=None,
-            f_params=self.f_params,
-            f_optimizer=self.f_optimizer,
-            f_history=self.f_history,
-            f_pickle=self.f_pickle,
             fn_prefix=self.fn_prefix,
             dirname=self.dirname,
             event_name=None,
-            sink=self.sink)
+            sink=self.sink,
+            **self._f_kwargs()
+        )
         self.checkpoint_.initialize()
 
     def on_train_end(self, net, **kwargs):
         self.checkpoint_.save_model(net)
         self.checkpoint_._sink("Final checkpoint triggered", net.verbose)
 
     def __getattr__(self, attr):
```

### Comparing `skorch-0.8.0/skorch/classifier.py` & `skorch-0.9.0/skorch/classifier.py`

 * *Files 14% similar despite different names*

```diff
@@ -202,20 +202,15 @@
           ``Dataset`` that can deal with the data.
 
         Returns
         -------
         y_pred : numpy ndarray
 
         """
-        y_preds = []
-        for yp in self.forward_iter(X, training=False):
-            yp = yp[0] if isinstance(yp, tuple) else yp
-            y_preds.append(to_numpy(yp.max(-1)[-1]))
-        y_pred = np.concatenate(y_preds, 0)
-        return y_pred
+        return super().predict_proba(X).argmax(axis=1)
 
 
 neural_net_binary_clf_doc_start = """NeuralNet for binary classification tasks
 
     Use this specifically if you have a binary classification task,
     with input data X and target y. y must be 1d.
 
@@ -284,15 +279,15 @@
     @property
     def classes_(self):
         return [0, 1]
 
     # pylint: disable=signature-differs
     def check_data(self, X, y):
         super().check_data(X, y)
-        if get_dim(y) != 1:
+        if (not is_dataset(X)) and (get_dim(y) != 1):
             raise ValueError("The target data should be 1-dimensional.")
 
     def infer(self, x, **fit_params):
         """Perform an inference step
 
         The first output of the ``module`` must be a single array that
         has either shape (n,) or shape (n, 1). In the latter case, the
@@ -357,53 +352,7 @@
         Returns
         -------
         y_pred : numpy ndarray
 
         """
         y_proba = self.predict_proba(X)
         return (y_proba[:, 1] > self.threshold).astype('uint8')
-
-    # pylint: disable=missing-docstring
-    def predict_proba(self, X):
-        """Where applicable, return probability estimates for
-        samples.
-
-        If the module's forward method returns multiple outputs as a
-        tuple, it is assumed that the first output contains the
-        relevant information and the other values are ignored. If all
-        values are relevant, consider using
-        :func:`~skorch.NeuralNet.forward` instead.
-
-        Parameters
-        ----------
-        X : input data, compatible with skorch.dataset.Dataset
-          By default, you should be able to pass:
-
-            * numpy arrays
-            * torch tensors
-            * pandas DataFrame or Series
-            * scipy sparse CSR matrices
-            * a dictionary of the former three
-            * a list/tuple of the former three
-            * a Dataset
-
-          If this doesn't work with your data, you have to pass a
-          ``Dataset`` that can deal with the data.
-
-        Returns
-        -------
-        y_proba : numpy ndarray
-
-        """
-        y_probas = []
-        self.check_is_fitted(attributes=['criterion_'])
-        bce_logits_loss = isinstance(
-            self.criterion_, torch.nn.BCEWithLogitsLoss)
-
-        for yp in self.forward_iter(X, training=False):
-            yp = yp[0] if isinstance(yp, tuple) else yp
-            if bce_logits_loss:
-                yp = torch.sigmoid(yp)
-            y_probas.append(to_numpy(yp))
-        y_proba = np.concatenate(y_probas, 0)
-        y_proba = np.stack((1 - y_proba, y_proba), axis=1)
-        return y_proba
```

### Comparing `skorch-0.8.0/skorch/cli.py` & `skorch-0.9.0/skorch/cli.py`

 * *Files identical despite different names*

### Comparing `skorch-0.8.0/skorch/dataset.py` & `skorch-0.9.0/skorch/dataset.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 """Contains custom skorch Dataset and CVSplit."""
-
+import warnings
 from functools import partial
 from numbers import Number
 
 import numpy as np
 from scipy import sparse
 from sklearn.model_selection import ShuffleSplit
 from sklearn.model_selection import StratifiedKFold
@@ -257,14 +257,24 @@
     ):
         self.stratified = stratified
         self.random_state = random_state
 
         if isinstance(cv, Number) and (cv <= 0):
             raise ValueError("Numbers less than 0 are not allowed for cv "
                              "but CVSplit got {}".format(cv))
+
+        if not self._is_float(cv) and random_state is not None:
+            # TODO: raise a ValueError instead of a warning
+            warnings.warn(
+                "Setting a random_state has no effect since cv is not a float. "
+                "This will raise an error in a future. You should leave "
+                "random_state to its default (None), or set cv to a float value.",
+                FutureWarning
+            )
+
         self.cv = cv
 
     def _is_stratified(self, cv):
         return isinstance(cv, (StratifiedKFold, StratifiedShuffleSplit))
 
     def _is_float(self, x):
         if not isinstance(x, Number):
@@ -298,15 +308,15 @@
         return self._check_cv_non_float(y_arr)
 
     def _is_regular(self, x):
         return (x is None) or isinstance(x, np.ndarray) or is_pandas_ndframe(x)
 
     def __call__(self, dataset, y=None, groups=None):
         bad_y_error = ValueError(
-            "Stratified CV requires explicitely passing a suitable y.")
+            "Stratified CV requires explicitly passing a suitable y.")
         if (y is None) and self.stratified:
             raise bad_y_error
 
         cv = self.check_cv(y)
         if self.stratified and not self._is_stratified(cv):
             raise bad_y_error
```

### Comparing `skorch-0.8.0/skorch/helper.py` & `skorch-0.9.0/skorch/helper.py`

 * *Files 1% similar despite different names*

```diff
@@ -244,20 +244,20 @@
             if i.dtype == np.bool:
                 i = np.flatnonzero(i)
 
         return SliceDataset(self.dataset, idx=self.idx, indices=self.indices_[i])
 
 
 def predefined_split(dataset):
-    """Uses ``dataset`` for validiation in ``NeutralNet``.
+    """Uses ``dataset`` for validiation in :class:`.NeuralNet`.
 
     Examples
     --------
     >>> valid_ds = skorch.Dataset(X, y)
-    >>> net = NeutralNet(..., train_split=predefined_split(valid_ds))
+    >>> net = NeuralNet(..., train_split=predefined_split(valid_ds))
 
     Parameters
     ----------
     dataset: torch Dataset
        Validiation dataset
 
     """
```

### Comparing `skorch-0.8.0/skorch/history.py` & `skorch-0.9.0/skorch/history.py`

 * *Files identical despite different names*

### Comparing `skorch-0.8.0/skorch/net.py` & `skorch-0.9.0/skorch/net.py`

 * *Files 11% similar despite different names*

```diff
@@ -18,26 +18,39 @@
 from skorch.dataset import CVSplit
 from skorch.dataset import get_len
 from skorch.dataset import unpack_data
 from skorch.dataset import uses_placeholder_y
 from skorch.exceptions import DeviceWarning
 from skorch.history import History
 from skorch.setter import optimizer_setter
+from skorch.utils import _identity
+from skorch.utils import _infer_predict_nonlinearty
 from skorch.utils import FirstStepAccumulator
 from skorch.utils import TeeGenerator
+from skorch.utils import _check_f_arguments
 from skorch.utils import check_is_fitted
 from skorch.utils import duplicate_items
 from skorch.utils import get_map_location
 from skorch.utils import is_dataset
 from skorch.utils import params_for
 from skorch.utils import to_device
 from skorch.utils import to_numpy
 from skorch.utils import to_tensor
 
 
+_PYTORCH_COMPONENTS = {'criterion', 'module', 'optimizer'}
+"""Special names that mark pytorch components.
+
+These special names are used to recognize whether an attribute that is
+being set in the net should be added to prefixes_ and
+cuda_dependent_attributes_
+
+"""
+
+
 # pylint: disable=too-many-instance-attributes
 class NeuralNet:
     # pylint: disable=anomalous-backslash-in-string
     """NeuralNet base class.
 
     The base class covers more generic cases. Depending on your use
     case, you might want to use :class:`.NeuralNetClassifier` or
@@ -138,21 +151,53 @@
       a tuple ``(name, callback)`` can be passed, where ``name``
       should be unique. Callbacks may or may not be instantiated.
       The callback name can be used to set parameters on specific
       callbacks (e.g., for the callback with name ``'print_log'``, use
       ``net.set_params(callbacks__print_log__keys_ignored=['epoch',
       'train_loss'])``).
 
+    predict_nonlinearity : callable, None, or 'auto' (default='auto')
+      The nonlinearity to be applied to the prediction. When set to
+      'auto', infers the correct nonlinearity based on the criterion
+      (softmax for :class:`~torch.nn.CrossEntropyLoss` and sigmoid for
+      :class:`~torch.nn.BCEWithLogitsLoss`). If it cannot be inferred
+      or if the parameter is None, just use the identity
+      function. Don't pass a lambda function if you want the net to be
+      pickleable.
+
+      In case a callable is passed, it should accept the output of the
+      module (the first output if there is more than one), which is a
+      PyTorch tensor, and return the transformed PyTorch tensor.
+
+      This can be useful, e.g., when
+      :func:`~skorch.NeuralNetClassifier.predict_proba`
+      should return probabilities but a criterion is used that does
+      not expect probabilities. In that case, the module can return
+      whatever is required by the criterion and the
+      ``predict_nonlinearity`` transforms this output into
+      probabilities.
+
+      The nonlinearity is applied only when calling
+      :func:`~skorch.classifier.NeuralNetClassifier.predict` or
+      :func:`~skorch.classifier.NeuralNetClassifier.predict_proba` but
+      not anywhere else -- notably, the loss is unaffected by this
+      nonlinearity.
+
     warm_start : bool (default=False)
       Whether each fit call should lead to a re-initialization of the
       module (cold start) or whether the module should be trained
       further (warm start).
 
     verbose : int (default=1)
-      Control the verbosity level.
+      This parameter controls how much print output is generated by
+      the net and its callbacks. By setting this value to 0, e.g. the
+      summary scores at the end of each epoch are no longer printed.
+      This can be useful when running a hyperparameter search. The
+      summary scores are always logged in the history attribute,
+      regardless of the verbose setting.
 
     device : str, torch.device (default='cpu')
       The compute device to be used. If set to 'cuda', data in torch
       tensors will be pushed to cuda tensors before being sent to the
       module. If set to None, then all compute devices will be left
       unmodified.
 
@@ -199,14 +244,15 @@
             max_epochs=10,
             batch_size=128,
             iterator_train=DataLoader,
             iterator_valid=DataLoader,
             dataset=Dataset,
             train_split=CVSplit(5),
             callbacks=None,
+            predict_nonlinearity='auto',
             warm_start=False,
             verbose=1,
             device='cpu',
             **kwargs
     ):
         self.module = module
         self.criterion = criterion
@@ -215,14 +261,15 @@
         self.max_epochs = max_epochs
         self.batch_size = batch_size
         self.iterator_train = iterator_train
         self.iterator_valid = iterator_valid
         self.dataset = dataset
         self.train_split = train_split
         self.callbacks = callbacks
+        self.predict_nonlinearity = predict_nonlinearity
         self.warm_start = warm_start
         self.verbose = verbose
         self.device = device
 
         self._check_deprecated_params(**kwargs)
         history = kwargs.pop('history', None)
         initialized = kwargs.pop('initialized_', False)
@@ -399,15 +446,15 @@
             # check if callback itself is changed
             param_callback = getattr(self, 'callbacks__' + name, Dummy)
             if param_callback is not Dummy:  # callback itself was set
                 cb = param_callback
 
             # below: check for callback params
             # don't set a parameter for non-existing callback
-            params = self._get_params_for('callbacks__{}'.format(name))
+            params = self.get_params_for('callbacks__{}'.format(name))
             if (cb is None) and params:
                 raise ValueError("Trying to set a parameter for callback {} "
                                  "which does not exist.".format(name))
             if cb is None:
                 continue
 
             if isinstance(cb, type):  # uninitialized:
@@ -418,15 +465,15 @@
             callbacks_.append((name, cb))
 
         self.callbacks_ = callbacks_
         return self
 
     def initialize_criterion(self):
         """Initializes the criterion."""
-        criterion_params = self._get_params_for('criterion')
+        criterion_params = self.get_params_for('criterion')
         self.criterion_ = self.criterion(**criterion_params)
         if isinstance(self.criterion_, torch.nn.Module):
             self.criterion_ = to_device(self.criterion_, self.device)
         return self
 
     def _format_reinit_msg(self, name, kwargs=None, triggered_directly=True):
         """Returns a message that informs about re-initializing a compoment.
@@ -448,15 +495,15 @@
     def initialize_module(self):
         """Initializes the module.
 
         Note that if the module has learned parameters, those will be
         reset.
 
         """
-        kwargs = self._get_params_for('module')
+        kwargs = self.get_params_for('module')
         module = self.module
         is_initialized = isinstance(module, torch.nn.Module)
 
         if kwargs or not is_initialized:
             if is_initialized:
                 module = type(module)
 
@@ -502,15 +549,15 @@
           Initialization of the optimizer can be triggered directly
           (e.g. when lr was changed) or indirectly (e.g. when the
           module was re-initialized). If and only if the former
           happens, the user should receive a message informing them
           about the parameters that caused the re-initialization.
 
         """
-        args, kwargs = self._get_params_for_optimizer(
+        args, kwargs = self.get_params_for_optimizer(
             'optimizer', self.module_.named_parameters())
 
         if self.initialized_ and self.verbose:
             msg = self._format_reinit_msg(
                 "optimizer", kwargs, triggered_directly=triggered_directly)
             print(msg)
 
@@ -648,20 +695,22 @@
 
         **fit_params : dict
           Additional parameters passed to the ``forward`` method of
           the module and to the train_split call.
 
         """
         step_accumulator = self.get_train_step_accumulator()
+
         def step_fn():
+            self.optimizer_.zero_grad()
             step = self.train_step_single(Xi, yi, **fit_params)
             step_accumulator.store_step(step)
             return step['loss']
+
         self.optimizer_.step(step_fn)
-        self.optimizer_.zero_grad()
         return step_accumulator.get_step()
 
     def evaluation_step(self, Xi, training=False):
         """Perform a forward step to produce the output used for
         prediction and scoring.
 
         Therefore the module is set to evaluation mode by default
@@ -994,14 +1043,53 @@
         """
         x = to_tensor(x, device=self.device)
         if isinstance(x, dict):
             x_dict = self._merge_x_and_fit_params(x, fit_params)
             return self.module_(**x_dict)
         return self.module_(x, **fit_params)
 
+    def _get_predict_nonlinearity(self):
+        """Return the nonlinearity to be applied to the prediction
+
+        This can be useful, e.g., when
+        :func:`~skorch.classifier.NeuralNetClassifier.predict_proba`
+        should return probabilities but a criterion is used that does
+        not expect probabilities. In that case, the module can return
+        whatever is required by the criterion and the
+        ``predict_nonlinearity`` transforms this output into
+        probabilities.
+
+        The nonlinearity is applied only when calling
+        :func:`~skorch.classifier.NeuralNetClassifier.predict` or
+        :func:`~skorch.classifier.NeuralNetClassifier.predict_proba`
+        but not anywhere else -- notably, the loss is unaffected by
+        this nonlinearity.
+
+        Raises
+        ------
+        TypeError
+          Raise a TypeError if the return value is not callable.
+
+        Returns
+        -------
+        nonlin : callable
+          A callable that takes a single argument, which is a PyTorch
+          tensor, and returns a PyTorch tensor.
+
+        """
+        self.check_is_fitted()
+        nonlin = self.predict_nonlinearity
+        if nonlin is None:
+            nonlin = _identity
+        elif nonlin == 'auto':
+            nonlin = _infer_predict_nonlinearty(self)
+        if not callable(nonlin):
+            raise TypeError("predict_nonlinearity has to be a callable, 'auto' or None")
+        return nonlin
+
     def predict_proba(self, X):
         """Return the output of the module's forward method as a numpy
         array.
 
         If the module's forward method returns multiple outputs as a
         tuple, it is assumed that the first output contains the
         relevant information and the other values are ignored. If all
@@ -1025,17 +1113,19 @@
           ``Dataset`` that can deal with the data.
 
         Returns
         -------
         y_proba : numpy ndarray
 
         """
+        nonlin = self._get_predict_nonlinearity()
         y_probas = []
         for yp in self.forward_iter(X, training=False):
             yp = yp[0] if isinstance(yp, tuple) else yp
+            yp = nonlin(yp)
             y_probas.append(to_numpy(yp))
         y_proba = np.concatenate(y_probas, 0)
         return y_proba
 
     def predict(self, X):
         """Where applicable, return class labels for samples in X.
 
@@ -1095,14 +1185,18 @@
           ``Dataset`` that can deal with the data.
 
         training : bool (default=False)
           Whether train mode should be used or not.
 
         """
         y_true = to_tensor(y_true, device=self.device)
+
+        if isinstance(self.criterion_, torch.nn.Module):
+            self.criterion_.train(training)
+
         return self.criterion_(y_pred, y_true)
 
     def get_dataset(self, X, y=None):
         """Get a dataset that contains the input data and is passed to
         the iterator.
 
         Override this if you want to initialize your dataset
@@ -1137,15 +1231,15 @@
         """
         if is_dataset(X):
             return X
 
         dataset = self.dataset
         is_initialized = not callable(dataset)
 
-        kwargs = self._get_params_for('dataset')
+        kwargs = self.get_params_for('dataset')
         if kwargs and is_initialized:
             raise TypeError("Trying to pass an initialized Dataset while "
                             "passing Dataset arguments ({}) is not "
                             "allowed.".format(kwargs))
 
         if is_initialized:
             return dataset
@@ -1192,20 +1286,24 @@
           The initialized training dataset.
 
         dataset_valid
           The initialized validation dataset or None
 
         """
         dataset = self.get_dataset(X, y)
-        if self.train_split:
-            dataset_train, dataset_valid = self.train_split(
-                dataset, y, **fit_params)
-        else:
-            dataset_train, dataset_valid = dataset, None
-        return dataset_train, dataset_valid
+        if not self.train_split:
+            return dataset, None
+
+        # After a change in (#646),
+        # `y` is no longer passed to `self.train_split` if it is `None`.
+        # To revert to the previous behavior, remove the following two lines:
+        if y is None:
+            return self.train_split(dataset, **fit_params)
+
+        return self.train_split(dataset, y, **fit_params)
 
     def get_iterator(self, dataset, training=False):
         """Get an iterator that allows to loop over the batches of the
         given data.
 
         If ``self.iterator_train__batch_size`` and/or
         ``self.iterator_test__batch_size`` are not set, use
@@ -1224,68 +1322,152 @@
         -------
         iterator
           An instantiated iterator that allows to loop over the
           mini-batches.
 
         """
         if training:
-            kwargs = self._get_params_for('iterator_train')
+            kwargs = self.get_params_for('iterator_train')
             iterator = self.iterator_train
         else:
-            kwargs = self._get_params_for('iterator_valid')
+            kwargs = self.get_params_for('iterator_valid')
             iterator = self.iterator_valid
 
         if 'batch_size' not in kwargs:
             kwargs['batch_size'] = self.batch_size
 
         if kwargs['batch_size'] == -1:
             kwargs['batch_size'] = len(dataset)
 
         return iterator(dataset, **kwargs)
 
     def _get_params_for(self, prefix):
         return params_for(prefix, self.__dict__)
 
-    def _get_params_for_optimizer(self, prefix, named_parameters):
-        """Parse kwargs configuration for the optimizer identified by
-        the given prefix. Supports param group assignment using wildcards:
+    def get_params_for(self, prefix):
+        """Collect and return init parameters for an attribute.
 
-            optimizer__lr=0.05,
-            optimizer__param_groups=[
-                ('rnn*.period', {'lr': 0.3, 'momentum': 0}),
-                ('rnn0', {'lr': 0.1}),
-            ]
+        Attributes could be, for instance, pytorch modules, criteria,
+        or data loaders (for optimizers, use
+        :meth:`.get_params_for_optimizer` instead). Use the returned
+        arguments to initialize the given attribute like this:
+
+        .. code:: python
+
+            # inside initialize_module method
+            kwargs = self.get_params_for('module')
+            self.module_ = self.module(**kwargs)
+
+        Proceed analogously for the criterion etc.
+
+        The reason to use this method is so that it's possible to
+        change the init parameters with :meth:`.set_params`, which
+        in turn makes grid search and other similar things work.
+
+        Note that in general, as a user, you never have to deal with
+        this method because :meth:`.initialize_module` etc. are
+        already taking care of this. You only need to deal with this
+        if you override :meth:`.initialize_module` (or similar
+        methods) because you have some custom code that requires it.
+
+        Parameters
+        ----------
+        prefix : str
+          The name of the attribute whose arguments should be
+          returned. E.g. for the module, it should be ``'module'``.
+
+        Returns
+        -------
+        kwargs : dict
+          Keyword arguments to be used as init parameters.
 
-        The first positional argument are the param groups.
         """
-        kwargs = self._get_params_for(prefix)
+        return self._get_params_for(prefix)
+
+    def _get_params_for_optimizer(self, prefix, named_parameters):
+        kwargs = self.get_params_for(prefix)
         params = list(named_parameters)
         pgroups = []
 
         for pattern, group in kwargs.pop('param_groups', []):
             matches = [i for i, (name, _) in enumerate(params) if
                        fnmatch.fnmatch(name, pattern)]
             if matches:
                 p = [params.pop(i)[1] for i in reversed(matches)]
                 pgroups.append({'params': p, **group})
 
         if params:
             pgroups.append({'params': [p for _, p in params]})
 
-        return [pgroups], kwargs
+        args = (pgroups,)
+        return args, kwargs
 
-    def _get_param_names(self):
-        return (k for k in self.__dict__.keys() if k != 'history_')
+    def get_params_for_optimizer(self, prefix, named_parameters):
+        """Collect and return init parameters for an optimizer.
+
+        Parse kwargs configuration for the optimizer identified by
+        the given prefix. Supports param group assignment using wildcards:
+
+        .. code:: python
+
+            optimizer__lr=0.05,
+            optimizer__param_groups=[
+                ('rnn*.period', {'lr': 0.3, 'momentum': 0}),
+                ('rnn0', {'lr': 0.1}),
+            ]
+
+        Generally, use this method like this:
+
+        .. code:: python
+
+            # inside initialize_optimizer method
+            named_params = self.module_.named_parameters()
+            pgroups, kwargs = self.get_params_for_optimizer('optimizer', named_params)
+            if 'lr' not in kwargs:
+                kwargs['lr'] = self.lr
+            self.optimizer_ = self.optimizer(*pgroups, **kwargs)
+
+        The reason to use this method is so that it's possible to
+        change the init parameters with :meth:`.set_params`, which
+        in turn makes grid search and other similar things work.
+
+        Note that in general, as a user, you never have to deal with
+        this method because :meth:`.initialize_optimizer` is already
+        taking care of this. You only need to deal with this if you
+        override :meth:`.initialize_optimizer` because you have some
+        custom code that requires it.
+
+        Parameters
+        ----------
+        prefix : str
+          The name of the optimizer whose arguments should be
+          returned. Typically, this should just be
+          ``'optimizer'``. There can be exceptions, however, e.g. if
+          you want to use more than one optimizer.
+
+        named_parameters : iterator
+          Iterator over the parameters of the module that is intended
+          to be optimized. It's the return value of
+          ``my_module.named_parameters()``.
 
-    def _get_param_names_new(self):
-        # TODO: This will be the new behavior for _get_param_names in
-        # a future release. This is to make get_params work as in
-        # sklearn, i.e. not returning "learned" attributes (ending on
-        # '_'). Once the transition period has passed, remove the old
-        # code and use the new one instead.
+        Returns
+        -------
+        args : tuple
+          All positional arguments for this optimizer (right now only
+          one, the parameter groups).
+
+        kwargs : dict
+          All other parameters for this optimizer, e.g. the learning
+          rate.
+
+        """
+        args, kwargs = self._get_params_for_optimizer(prefix, named_parameters)
+        return args, kwargs
+
+    def _get_param_names(self):
         return (k for k in self.__dict__ if not k.endswith('_'))
 
     def _get_params_callbacks(self, deep=True):
         """sklearn's .get_params checks for `hasattr(value,
         'get_params')`. This returns False for a list. But our
         callbacks reside within a list. Hence their parameters have to
         be retrieved separately.
@@ -1351,15 +1533,15 @@
                 unexpected_kwargs.append(key)
 
         msgs = []
         if unexpected_kwargs:
             tmpl = ("__init__() got unexpected argument(s) {}. "
                     "Either you made a typo, or you added new arguments "
                     "in a subclass; if that is the case, the subclass "
-                    "should deal with the new arguments explicitely.")
+                    "should deal with the new arguments explicitly.")
             msg = tmpl.format(', '.join(sorted(unexpected_kwargs)))
             msgs.append(msg)
 
         for prefix, key in sorted(missing_dunder_kwargs, key=lambda tup: tup[1]):
             tmpl = "Got an unexpected argument {}, did you mean {}?"
             suffix = key[len(prefix):].lstrip('_')
             suggestion = prefix + '__' + suffix
@@ -1412,25 +1594,25 @@
         # Below: Re-initialize parts of the net if necessary.
 
         if cb_params:
             # callbacks need special treatmeant since they are list of tuples
             self.initialize_callbacks()
             self._set_params_callback(**cb_params)
 
-        if any(key.startswith('criterion') for key in special_params):
+        if any('criterion' in key.split('__', 1)[0] for key in special_params):
             self.initialize_criterion()
 
         module_triggers_optimizer_reinit = False
-        if any(key.startswith('module') for key in special_params):
+        if any('module' in key.split('__', 1)[0] for key in special_params):
             self.initialize_module()
             module_triggers_optimizer_reinit = True
 
         optimizer_changed = (
-            any(key.startswith('optimizer') for key in special_params) or
-            'lr' in normal_params
+            any('optimizer' in key.split('__', 1)[0] for key in special_params)
+            or 'lr' in normal_params
         )
         if module_triggers_optimizer_reinit or optimizer_changed:
             # Model selectors such as GridSearchCV will set the
             # parameters before .initialize() is called, therefore we
             # need to make sure that we have an initialized model here
             # as the optimizer depends on it.
             if not hasattr(self, 'module_'):
@@ -1514,66 +1696,208 @@
             cuda_attrs = torch.load(f, **load_kwargs)
 
         state.update(cuda_attrs)
         state.pop('__cuda_dependent_attributes__')
 
         self.__dict__.update(state)
 
+    def _register_attribute(
+            self,
+            name,
+            prefixes=True,
+            cuda_dependent_attributes=True,
+    ):
+        """Add attribute name to prefixes_ and
+        cuda_dependent_attributes_.
+
+        The first is to take care that the attribute works correctly
+        with set_params, e.g. when it comes to re-initialization.
+
+        The second is to make sure that nets trained with CUDA can be
+        loaded without CUDA.
+
+        This method takes care of not mutating the lists.
+
+        Parameters
+        ----------
+        prefixes : bool (default=True)
+          Whether to add to prefixes_.
+
+        cuda_dependent_attributes : bool (default=True)
+          Whether to add to cuda_dependent_attributes_.
+
+        """
+        # copy the lists to avoid mutation
+        if prefixes:
+            self.prefixes_ = self.prefixes_[:] + [name]
+
+        if cuda_dependent_attributes:
+            self.cuda_dependent_attributes_ = (
+                self.cuda_dependent_attributes_[:] + [name + '_'])
+
+    def _unregister_attribute(
+            self,
+            name,
+            prefixes=True,
+            cuda_dependent_attributes=True,
+    ):
+        """Remove attribute name from prefixes_ and
+        cuda_dependent_attributes_.
+
+        Use this to remove PyTorch components that are not needed
+        anymore. This is mostly a clean up job, so as to not leave
+        unnecessary prefixes or cuda-dependent attributes.
+
+        This method takes care of not mutating the lists.
+
+        Parameters
+        ----------
+        prefixes : bool (default=True)
+          Whether to remove from prefixes_.
+
+        cuda_dependent_attributes : bool (default=True)
+          Whether to remove from cuda_dependent_attributes_.
+
+        """
+        # copy the lists to avoid mutation
+        if prefixes:
+            self.prefixes_ = [p for p in self.prefixes_ if p != name]
+
+        if cuda_dependent_attributes:
+            self.cuda_dependent_attributes_ = [
+                a for a in self.cuda_dependent_attributes_ if a != name + '_']
+
+    def __setattr__(self, name, attr):
+        """Set an attribute on the net
+
+        When a custom net with additional torch modules or optimizers
+        is created, those attributes are added to ``prefixes_`` and
+        ``cuda_dependent_attributes_`` automatically.
+
+        """
+        # If it's a
+        # 1. known attribute or
+        # 2. special param like module__num_units or
+        # 3. not a torch module/optimizer instance or class
+        # just setattr as usual.
+        # For a discussion why we chose this implementation, see here:
+        # https://github.com/skorch-dev/skorch/pull/597
+        is_known = name.endswith('_') or (name in self.prefixes_)
+        is_special_param = '__' in name
+        is_torch_component = any(c in name for c in _PYTORCH_COMPONENTS)
+
+        if not (is_known or is_special_param) and is_torch_component:
+            self._register_attribute(name)
+        super().__setattr__(name, attr)
+
+    def __delattr__(self, name):
+        # take extra precautions to undo the changes made in __setattr__
+        self._unregister_attribute(name)
+        super().__delattr__(name)
+
+    def _get_module(self, name, msg):
+        """Return the PyTorch module with the given name
+
+        If a module with such a name doesn't exist, also check the
+        name without trailing underscore.
+
+        Raises
+        ------
+        AttributeError
+          If no module with the given name could be found, with a
+          message formatted according to the passed ``msg`` argument.
+
+        """
+        try:
+            module = getattr(self, name)
+            if not hasattr(module, 'state_dict'):
+                raise AttributeError
+            return module
+        except AttributeError:
+            if name.endswith('_'):
+                name = name[:-1]
+            raise AttributeError(msg.format(name=name))
+
     def save_params(
-            self, f_params=None, f_optimizer=None, f_history=None):
+            self,
+            f_params=None,
+            f_optimizer=None,
+            f_criterion=None,
+            f_history=None,
+            **kwargs):
         """Saves the module's parameters, history, and optimizer,
         not the whole object.
 
         To save the whole object, use pickle. This is necessary when
         you need additional learned attributes on the net, e.g. the
         ``classes_`` attribute on
         :class:`skorch.classifier.NeuralNetClassifier`.
 
-        ``f_params`` and ``f_optimizer`` uses PyTorchs'
+        ``f_params``, ``f_optimizer``, etc. use PyTorch's
         :func:`~torch.save`.
 
+        If you've created a custom module, e.g. ``net.mymodule_``, you
+        can save that as well by passing ``f_mymodule``.
+
         Parameters
         ----------
         f_params : file-like object, str, None (default=None)
           Path of module parameters. Pass ``None`` to not save
 
         f_optimizer : file-like object, str, None (default=None)
           Path of optimizer. Pass ``None`` to not save
 
+        f_criterion : file-like object, str, None (default=None)
+          Path of criterion. Pass ``None`` to not save
+
         f_history : file-like object, str, None (default=None)
           Path to history. Pass ``None`` to not save
 
         Examples
         --------
         >>> before = NeuralNetClassifier(mymodule)
         >>> before.save_params(f_params='model.pkl',
-        >>>                    f_optimizer='optimizer.pkl',
-        >>>                    f_history='history.json')
+        ...                    f_optimizer='optimizer.pkl',
+        ...                    f_history='history.json')
         >>> after = NeuralNetClassifier(mymodule).initialize()
         >>> after.load_params(f_params='model.pkl',
-        >>>                   f_optimizer='optimizer.pkl',
-        >>>                   f_history='history.json')
+        ...                   f_optimizer='optimizer.pkl',
+        ...                   f_history='history.json')
 
         """
-        if f_params is not None:
-            msg = (
-                "Cannot save parameters of an un-initialized model. "
-                "Please initialize first by calling .initialize() "
-                "or by fitting the model with .fit(...).")
-            self.check_is_fitted(msg=msg)
-            torch.save(self.module_.state_dict(), f_params)
-
-        if f_optimizer is not None:
-            msg = (
-                "Cannot save state of an un-initialized optimizer. "
-                "Please initialize first by calling .initialize() "
-                "or by fitting the model with .fit(...).")
-            self.check_is_fitted(attributes=['optimizer_'], msg=msg)
-            torch.save(self.optimizer_.state_dict(), f_optimizer)
+        kwargs_module, kwargs_other = _check_f_arguments(
+            'save_params',
+            f_params=f_params,
+            f_optimizer=f_optimizer,
+            f_criterion=f_criterion,
+            f_history=f_history,
+            **kwargs)
+
+        if not kwargs_module and not kwargs_other:
+            print("Nothing to save")
+            return
+
+        msg_init = (
+            "Cannot save state of an un-initialized model. "
+            "Please initialize first by calling .initialize() "
+            "or by fitting the model with .fit(...).")
+        msg_module = (
+            "You are trying to save 'f_{name}' but for that to work, the net "
+            "needs to have an attribute called 'net.{name}_' that is a PyTorch "
+            "Module; make sure that it exists and check for typos.")
+
+        for attr, f_name in kwargs_module.items():
+            # valid attrs can be 'module_', 'optimizer_', etc.
+            if attr[:-1] in self.prefixes_:
+                self.check_is_fitted([attr], msg=msg_init)
+            module = self._get_module(attr, msg=msg_module)
+            torch.save(module.state_dict(), f_name)
 
+        # only valid key in kwargs_other is f_history
+        f_history = kwargs_other.get('f_history')
         if f_history is not None:
             self.history.to_file(f_history)
 
     def _check_device(self, requested_device, map_device):
         """Compare the requested device with the map device and
         return the map device if it differs from the requested device
         along with a warning.
@@ -1587,32 +1911,43 @@
                 DeviceWarning)
             return map_device
         # return requested_device instead of map_device even though we
         # checked for *type* equality as we might have 'cuda:0' vs. 'cuda:1'.
         return requested_device
 
     def load_params(
-            self, f_params=None, f_optimizer=None, f_history=None,
-            checkpoint=None):
+            self,
+            f_params=None,
+            f_optimizer=None,
+            f_criterion=None,
+            f_history=None,
+            checkpoint=None,
+            **kwargs):
         """Loads the the module's parameters, history, and optimizer,
         not the whole object.
 
         To save and load the whole object, use pickle.
 
-        ``f_params`` and ``f_optimizer`` uses PyTorchs'
-        :func:`~torch.save`.
+        ``f_params``, ``f_optimizer``, etc. uses PyTorch's
+        :func:`~torch.load`.
+
+        If you've created a custom module, e.g. ``net.mymodule_``, you
+        can save that as well by passing ``f_mymodule``.
 
         Parameters
         ----------
         f_params : file-like object, str, None (default=None)
           Path of module parameters. Pass ``None`` to not load.
 
         f_optimizer : file-like object, str, None (default=None)
           Path of optimizer. Pass ``None`` to not load.
 
+        f_criterion : file-like object, str, None (default=None)
+          Path of criterion. Pass ``None`` to not save
+
         f_history : file-like object, str, None (default=None)
           Path to history. Pass ``None`` to not load.
 
         checkpoint : :class:`.Checkpoint`, None (default=None)
           Checkpoint to load params from. If a checkpoint and a ``f_*``
           path is passed in, the ``f_*`` will be loaded. Pass
           ``None`` to not load.
@@ -1630,43 +1965,56 @@
 
         """
         def _get_state_dict(f):
             map_location = get_map_location(self.device)
             self.device = self._check_device(self.device, map_location)
             return torch.load(f, map_location=map_location)
 
-        if f_history is not None:
-            self.history = History.from_file(f_history)
-
+        kwargs_full = {}
         if checkpoint is not None:
             if not self.initialized_:
                 self.initialize()
             if f_history is None and checkpoint.f_history is not None:
                 self.history = History.from_file(checkpoint.f_history_)
-            formatted_files = checkpoint.get_formatted_files(self)
-            f_params = f_params or formatted_files['f_params']
-            f_optimizer = f_optimizer or formatted_files['f_optimizer']
-
-        if f_params is not None:
-            msg = (
-                "Cannot load parameters of an un-initialized model. "
-                "Please initialize first by calling .initialize() "
-                "or by fitting the model with .fit(...).")
-            self.check_is_fitted(msg=msg)
-            state_dict = _get_state_dict(f_params)
-            self.module_.load_state_dict(state_dict)
-
-        if f_optimizer is not None:
-            msg = (
-                "Cannot load state of an un-initialized optimizer. "
-                "Please initialize first by calling .initialize() "
-                "or by fitting the model with .fit(...).")
-            self.check_is_fitted(attributes=['optimizer_'], msg=msg)
-            state_dict = _get_state_dict(f_optimizer)
-            self.optimizer_.load_state_dict(state_dict)
+            kwargs_full.update(**checkpoint.get_formatted_files(self))
+
+        # explicit arguments may override checkpoint arguments
+        kwargs_full.update(**kwargs)
+        for key, val in [('f_params', f_params), ('f_optimizer', f_optimizer),
+                         ('f_criterion', f_criterion), ('f_history', f_history)]:
+            if val:
+                kwargs_full[key] = val
+
+        kwargs_module, kwargs_other = _check_f_arguments('load_params', **kwargs_full)
+
+        if not kwargs_module and not kwargs_other:
+            print("Nothing to load")
+            return
+
+        # only valid key in kwargs_other is f_history
+        f_history = kwargs_other.get('f_history')
+        if f_history is not None:
+            self.history = History.from_file(f_history)
+
+        msg_init = (
+            "Cannot load state of an un-initialized model. "
+            "Please initialize first by calling .initialize() "
+            "or by fitting the model with .fit(...).")
+        msg_module = (
+            "You are trying to load 'f_{name}' but for that to work, the net "
+            "needs to have an attribute called 'net.{name}_' that is a PyTorch "
+            "Module; make sure that it exists and check for typos.")
+
+        for attr, f_name in kwargs_module.items():
+            # valid attrs can be 'module_', 'optimizer_', etc.
+            if attr[:-1] in self.prefixes_:
+                self.check_is_fitted([attr], msg=msg_init)
+            module = self._get_module(attr, msg=msg_module)
+            state_dict = _get_state_dict(f_name)
+            module.load_state_dict(state_dict)
 
     def __repr__(self):
         to_include = ['module']
         to_exclude = []
         parts = [str(self.__class__) + '[uninitialized](']
         if self.initialized_:
             parts = [str(self.__class__) + '[initialized](']
```

### Comparing `skorch-0.8.0/skorch/regressor.py` & `skorch-0.9.0/skorch/regressor.py`

 * *Files identical despite different names*

### Comparing `skorch-0.8.0/skorch/setter.py` & `skorch-0.9.0/skorch/setter.py`

 * *Files identical despite different names*

### Comparing `skorch-0.8.0/skorch/tests/conftest.py` & `skorch-0.9.0/skorch/tests/conftest.py`

 * *Files 10% similar despite different names*

```diff
@@ -3,25 +3,34 @@
 from unittest.mock import Mock
 
 import numpy as np
 import pytest
 from sklearn.datasets import make_classification
 from sklearn.datasets import make_regression
 from sklearn.preprocessing import StandardScaler
+import torch
 from torch import nn
 
 F = nn.functional
 
 INFERENCE_METHODS = ['predict', 'predict_proba', 'forward', 'forward_iter']
 
 
 ###################
 # shared fixtures #
 ###################
 
+
+@pytest.fixture(autouse=True)
+def seeds_fixed():
+    torch.manual_seed(0)
+    torch.cuda.manual_seed(0)
+    np.random.seed(0)
+
+
 @pytest.fixture
 def module_cls():
     """Simple mock module for triggering scoring.
 
     This module returns the input without modifying it.
 
     """
@@ -118,15 +127,14 @@
 
     return func
 
 
 @pytest.fixture
 def net_cls():
     from skorch import NeuralNetRegressor
-    NeuralNetRegressor.score = Mock(side_effect=[10, 8, 6, 11, 7])
     return NeuralNetRegressor
 
 
 @pytest.fixture
 def data():
     X = np.array([0, 2, 3, 0]).astype(np.float32).reshape(-1, 1)
     y = np.array([-1, 0, 5, 4]).astype(np.float32).reshape(-1, 1)
```

### Comparing `skorch-0.8.0/skorch/tests/test_classifier.py` & `skorch-0.9.0/skorch/tests/test_classifier.py`

 * *Files 2% similar despite different names*

```diff
@@ -2,27 +2,23 @@
 
 Only contains tests that are specific for classifier subclasses.
 
 """
 
 from unittest.mock import Mock
 
-from flaky import flaky
 import numpy as np
 import pytest
 import torch
 from sklearn.base import clone
 from torch import nn
 
 from skorch.tests.conftest import INFERENCE_METHODS
 
 
-torch.manual_seed(0)
-
-
 class TestNeuralNet:
     @pytest.fixture(scope='module')
     def data(self, classifier_data):
         return classifier_data
 
     @pytest.fixture(scope='module')
     def dummy_callback(self):
@@ -66,17 +62,17 @@
 
         y_proba = net_fit.predict_proba(X)
         assert np.allclose(y_proba.sum(1), 1, rtol=1e-5)
 
         y_pred = net_fit.predict(X)
         assert np.allclose(np.argmax(y_proba, 1), y_pred, rtol=1e-5)
 
-    def test_score(self, net, data):
+    def test_score(self, net_fit, data):
         X, y = data
-        accuracy = net.score(X, y)
+        accuracy = net_fit.score(X, y)
         assert 0. <= accuracy <= 1.
 
     # classifier-specific test
     def test_takes_log_with_nllloss(self, net_cls, module_cls, data):
         net = net_cls(module_cls, criterion=nn.NLLLoss, max_epochs=1)
         net.initialize()
 
@@ -214,15 +210,14 @@
             list(getattr(net, method)(X))
 
         msg = ("This NeuralNetBinaryClassifier instance is not initialized "
                "yet. Call 'initialize' or 'fit' with appropriate arguments "
                "before using this method.")
         assert exc.value.args[0] == msg
 
-    @flaky(max_runs=3)
     def test_net_learns(self, net_cls, module_cls, data):
         X, y = data
         net = net_cls(
             module_cls,
             max_epochs=10,
             lr=1,
             batch_size=64,
@@ -261,33 +256,49 @@
         assert y_pred_proba.shape == (X.shape[0], 2)
 
         y_pred_exp = (y_pred_proba[:, 1] > threshold).astype('uint8')
 
         y_pred_actual = net.predict(X)
         assert np.allclose(y_pred_exp, y_pred_actual)
 
-    def test_score(self, net, data):
+    def test_score(self, net_fit, data):
         X, y = data
-        accuracy = net.score(X, y)
+        accuracy = net_fit.score(X, y)
         assert 0. <= accuracy <= 1.
 
+    def test_fit_with_dataset_and_y_none(self, net_cls, module_cls, data):
+        from skorch.dataset import Dataset
+
+        # deactivate train split since it requires y
+        net = net_cls(module_cls, train_split=False, max_epochs=1)
+        X, y = data
+        dataset = Dataset(X, y)
+        assert net.fit(dataset, y=None)
+
     def test_target_2d_raises(self, net, data):
         X, y = data
         with pytest.raises(ValueError) as exc:
             net.fit(X, y[:, None])
 
         assert exc.value.args[0] == (
             "The target data should be 1-dimensional.")
 
     def test_custom_loss_does_not_call_sigmoid(
             self, net_cls, data, module_cls, monkeypatch):
         mock = Mock(side_effect=lambda x: x)
         monkeypatch.setattr(torch, "sigmoid", mock)
 
-        net = net_cls(module_cls, max_epochs=1, lr=0.1, criterion=nn.MSELoss)
+        # add a custom nonlinearity - note that the output must return
+        # a 2d array from a 1d vector to conform to the required
+        # y_proba
+        def nonlin(x):
+            return torch.stack((1 - x, x), 1)
+
+        net = net_cls(module_cls, max_epochs=1, lr=0.1, criterion=nn.MSELoss,
+                      predict_nonlinearity=nonlin)
         X, y = data
         net.fit(X, y)
 
         net.predict_proba(X)
         assert mock.call_count == 0
 
     def test_default_loss_does_call_sigmoid(
```

### Comparing `skorch-0.8.0/skorch/tests/test_cli.py` & `skorch-0.9.0/skorch/tests/test_cli.py`

 * *Files identical despite different names*

### Comparing `skorch-0.8.0/skorch/tests/test_dataset.py` & `skorch-0.9.0/skorch/tests/test_dataset.py`

 * *Files 2% similar despite different names*

```diff
@@ -838,15 +838,15 @@
 
     def test_y_list_of_arr_stratified(self, cv_split_cls, data):
         y = [np.zeros(self.num_samples), np.ones(self.num_samples)]
         data.y = y
         with pytest.raises(ValueError) as exc:
             cv_split_cls(5, stratified=True)(data, y)
 
-        expected = "Stratified CV requires explicitely passing a suitable y."
+        expected = "Stratified CV requires explicitly passing a suitable y."
         assert exc.value.args[0] == expected
 
     def test_y_dict_does_not_raise(self, cv_split_cls, data):
         y = {'a': np.zeros(self.num_samples), 'b': np.ones(self.num_samples)}
         data.y = y
 
         cv_split_cls(5, stratified=False)(data)
@@ -862,15 +862,15 @@
     @pytest.mark.parametrize('cv', [5, 0.2])
     @pytest.mark.parametrize('X', [np.zeros((100, 10)), torch.zeros((100, 10))])
     def test_y_none_stratified(self, cv_split_cls, data, cv, X):
         data.X = X
         with pytest.raises(ValueError) as exc:
             cv_split_cls(cv, stratified=True)(data, None)
 
-        expected = "Stratified CV requires explicitely passing a suitable y."
+        expected = "Stratified CV requires explicitly passing a suitable y."
         assert exc.value.args[0] == expected
 
     def test_shuffle_split_reproducible_with_random_state(
             self, cv_split_cls, dataset_cls):
         n = self.num_samples
         X, y = np.random.random((n, 10)), np.random.randint(0, 10, size=n)
         cv = cv_split_cls(0.2, stratified=False)
@@ -901,7 +901,34 @@
         X_train, y_train = data_from_dataset(dataset_train)
         X_valid, y_valid = data_from_dataset(dataset_valid)
 
         assert np.allclose(X[:n], X_train)
         assert np.allclose(y[:n], y_train)
         assert np.allclose(X[n:], X_valid)
         assert np.allclose(y[n:], y_valid)
+
+    @pytest.mark.parametrize(
+        'args, kwargs, expect_warning',
+        [
+            ([], {}, False),
+            ([], {"random_state": 0}, True),
+            ([10], {"random_state": 0}, True),
+            ([0.7], {"random_state": 0}, False),
+            ([[]], {}, False),
+            ([[]], {"random_state": 0}, True),
+        ])
+    def test_random_state_not_used_warning(
+            self, cv_split_cls, args, kwargs, expect_warning):
+        with pytest.warns(None) as record:
+            cv_split_cls(*args, **kwargs)
+
+        if expect_warning:
+            assert len(record) == 1
+            warning = record[0].message
+            assert isinstance(warning, FutureWarning)
+            assert warning.args[0] == (
+                "Setting a random_state has no effect since cv is not a float. "
+                "This will raise an error in a future. You should leave "
+                "random_state to its default (None), or set cv to a float value."
+            )
+        else:
+            assert not record
```

### Comparing `skorch-0.8.0/skorch/tests/test_helper.py` & `skorch-0.9.0/skorch/tests/test_helper.py`

 * *Files identical despite different names*

### Comparing `skorch-0.8.0/skorch/tests/test_history.py` & `skorch-0.9.0/skorch/tests/test_history.py`

 * *Files identical despite different names*

### Comparing `skorch-0.8.0/skorch/tests/test_net.py` & `skorch-0.9.0/skorch/tests/test_net.py`

 * *Files 8% similar despite different names*

```diff
@@ -2,43 +2,43 @@
 
 Although NeuralNetClassifier is used in tests, test only functionality
 that is general to NeuralNet class.
 
 """
 
 import copy
+from distutils.version import LooseVersion
 from functools import partial
 import os
 from pathlib import Path
 import pickle
 from unittest.mock import Mock
 from unittest.mock import patch
 import sys
+import time
 from contextlib import ExitStack
 
+from flaky import flaky
 import numpy as np
-from distutils.version import LooseVersion
 import pytest
 from sklearn.base import clone
 from sklearn.feature_extraction.text import TfidfVectorizer
 from sklearn.metrics import accuracy_score
 from sklearn.model_selection import GridSearchCV
 from sklearn.pipeline import Pipeline
 from sklearn.preprocessing import StandardScaler
 import torch
 from torch import nn
-from flaky import flaky
 
 from skorch.tests.conftest import INFERENCE_METHODS
 from skorch.utils import flatten
 from skorch.utils import to_numpy
 from skorch.utils import is_torch_data_type
 
 
-torch.manual_seed(0)
 ACCURACY_EXPECTED = 0.65
 
 
 # pylint: disable=too-many-public-methods
 class TestNeuralNet:
     @pytest.fixture(scope='module')
     def data(self, classifier_data):
@@ -85,18 +85,29 @@
     def pipe(self, net):
         return Pipeline([
             ('scale', StandardScaler()),
             ('net', net),
         ])
 
     @pytest.fixture(scope='module')
-    def net_fit(self, net, data):
-        # Careful, don't call additional fits on this, since that would have
-        # side effects on other tests.
+    def net_fit(self, net_cls, module_cls, dummy_callback, data):
+        # Careful, don't call additional fits or set_params on this,
+        # since that would have side effects on other tests.
         X, y = data
+
+        # We need a new instance of the net and cannot reuse the net
+        # fixture, because otherwise fixture net and net_fit refer to
+        # the same object; also, we cannot clone(net) because this
+        # will result in the dummy_callback not being the mock anymore
+        net = net_cls(
+            module_cls,
+            callbacks=[('dummy', dummy_callback)],
+            max_epochs=10,
+            lr=0.1,
+        )
         return net.fit(X, y)
 
     @pytest.fixture
     def net_pickleable(self, net_fit):
         """NeuralNet instance that removes callbacks that are not
         pickleable.
 
@@ -162,27 +173,27 @@
     def test_net_init_one_unknown_argument(self, net_cls, module_cls):
         with pytest.raises(TypeError) as e:
             net_cls(module_cls, unknown_arg=123)
 
         expected = ("__init__() got unexpected argument(s) unknown_arg. "
                     "Either you made a typo, or you added new arguments "
                     "in a subclass; if that is the case, the subclass "
-                    "should deal with the new arguments explicitely.")
+                    "should deal with the new arguments explicitly.")
         assert e.value.args[0] == expected
 
     def test_net_init_two_unknown_arguments(self, net_cls, module_cls):
         with pytest.raises(TypeError) as e:
             net_cls(module_cls, lr=0.1, mxa_epochs=5,
                     warm_start=False, bathc_size=20)
 
         expected = ("__init__() got unexpected argument(s) "
                     "bathc_size, mxa_epochs. "
                     "Either you made a typo, or you added new arguments "
                     "in a subclass; if that is the case, the subclass "
-                    "should deal with the new arguments explicitely.")
+                    "should deal with the new arguments explicitly.")
         assert e.value.args[0] == expected
 
     @pytest.mark.parametrize('name, suggestion', [
         ('iterator_train_shuffle', 'iterator_train__shuffle'),
         ('optimizer_momentum', 'optimizer__momentum'),
         ('modulenum_units', 'module__num_units'),
         ('criterionreduce', 'criterion__reduce'),
@@ -222,15 +233,15 @@
                 module_cls,
                 foobar=123,
                 iterator_train_shuffle=True,
             )
         expected = ("__init__() got unexpected argument(s) foobar. "
                     "Either you made a typo, or you added new arguments "
                     "in a subclass; if that is the case, the subclass "
-                    "should deal with the new arguments explicitely.\n"
+                    "should deal with the new arguments explicitly.\n"
                     "Got an unexpected argument iterator_train_shuffle, "
                     "did you mean iterator_train__shuffle?")
         assert e.value.args[0] == expected
 
     def test_net_with_new_attribute_with_name_clash(
             self, net_cls, module_cls):
         # This covers a bug that existed when a new "settable"
@@ -278,15 +289,14 @@
             net = NeuralNetClassifier(module_cls)
             attributes = ['foo', 'bar_']
 
             net.check_is_fitted(attributes=attributes)
             args = check.call_args_list[0][0][1]
             assert args == attributes
 
-    @flaky(max_runs=3)
     def test_net_learns(self, net_cls, module_cls, data):
         X, y = data
         net = net_cls(
             module_cls,
             max_epochs=10,
             lr=0.1,
         )
@@ -453,14 +463,62 @@
         p = tmpdir.mkdir('skorch').join('testmodel.pkl')
         with open(str(p), 'wb') as f:
             # does not raise
             pickle.dump(net, f)
         with open(str(p), 'rb') as f:
             pickle.load(f)
 
+    def test_save_params_invalid_argument_name_raises(self, net_fit):
+        msg = "save_params got an unexpected argument 'foobar', did you mean 'f_foobar'?"
+        with pytest.raises(TypeError, match=msg):
+            net_fit.save_params(foobar='some-file.pt')
+
+    def test_load_params_invalid_argument_name_raises(self, net_fit):
+        msg = "load_params got an unexpected argument 'foobar', did you mean 'f_foobar'?"
+        with pytest.raises(TypeError, match=msg):
+            net_fit.load_params(foobar='some-file.pt')
+
+    def test_save_params_with_f_params_and_f_module_raises(self, net_fit):
+        msg = "save_params called with both f_params and f_module, please choose one"
+        with pytest.raises(TypeError, match=msg):
+            net_fit.save_params(f_module='weights.pt', f_params='params.pt')
+
+    def test_load_params_with_f_params_and_f_module_raises(self, net_fit):
+        msg = "load_params called with both f_params and f_module, please choose one"
+        with pytest.raises(TypeError, match=msg):
+            net_fit.load_params(f_module='weights.pt', f_params='params.pt')
+
+    def test_save_params_no_state_dict_raises(self, net_fit):
+        msg = ("You are trying to save 'f_max_epochs' but for that to work, the net "
+               "needs to have an attribute called 'net.max_epochs_' that is a PyTorch "
+               "Module; make sure that it exists and check for typos.")
+        with pytest.raises(AttributeError, match=msg):
+            net_fit.save_params(f_max_epochs='some-file.pt')
+
+    def test_load_params_no_state_dict_raises(self, net_fit):
+        msg = ("You are trying to load 'f_max_epochs' but for that to work, the net "
+               "needs to have an attribute called 'net.max_epochs_' that is a PyTorch "
+               "Module; make sure that it exists and check for typos.")
+        with pytest.raises(AttributeError, match=msg):
+            net_fit.load_params(f_max_epochs='some-file.pt')
+
+    def test_save_params_unknown_attribute_raises(self, net_fit):
+        msg = ("You are trying to save 'f_unknown' but for that to work, the net "
+               "needs to have an attribute called 'net.unknown_' that is a PyTorch "
+               "Module; make sure that it exists and check for typos.")
+        with pytest.raises(AttributeError, match=msg):
+            net_fit.save_params(f_unknown='some-file.pt')
+
+    def test_load_params_unknown_attribute_raises(self, net_fit):
+        msg = ("You are trying to load 'f_unknown' but for that to work, the net "
+               "needs to have an attribute called 'net.unknown_' that is a PyTorch "
+               "Module; make sure that it exists and check for typos.")
+        with pytest.raises(AttributeError, match=msg):
+            net_fit.load_params(f_unknown='some-file.pt')
+
     def test_save_load_state_dict_file(
             self, net_cls, module_cls, net_fit, data, tmpdir):
         net = net_cls(module_cls).initialize()
         X, y = data
 
         score_before = accuracy_score(y, net_fit.predict(X))
         score_untrained = accuracy_score(y, net.predict(X))
@@ -497,50 +555,66 @@
     def net_fit_adam(self, net_cls, module_cls, data):
         net = net_cls(
             module_cls, max_epochs=2, lr=0.1,
             optimizer=torch.optim.Adam)
         net.fit(*data)
         return net
 
-    def test_save_load_state_dict_file_with_history_optimizer(
-            self, net_cls, module_cls, net_fit_adam, tmpdir):
+    @pytest.fixture
+    def net_fit_criterion(self, net_fit_adam, module_cls):
+        """Replace criterion by a module so that it has learnt parameters"""
+        criterion = net_fit_adam.criterion_
+        net_fit_adam.criterion_ = module_cls()
+        yield net_fit_adam
+        net_fit_adam.criterion_ = criterion
+
+    def test_save_load_state_dict_file_with_history_optimizer_criterion(
+            self, net_cls, module_cls, net_fit_criterion, tmpdir):
 
         skorch_tmpdir = tmpdir.mkdir('skorch')
         p = skorch_tmpdir.join('testmodel.pkl')
         o = skorch_tmpdir.join('optimizer.pkl')
+        c = skorch_tmpdir.join('criterion.pkl')
         h = skorch_tmpdir.join('history.json')
 
         with ExitStack() as stack:
             p_fp = stack.enter_context(open(str(p), 'wb'))
             o_fp = stack.enter_context(open(str(o), 'wb'))
+            c_fp = stack.enter_context(open(str(c), 'wb'))
             h_fp = stack.enter_context(open(str(h), 'w'))
-            net_fit_adam.save_params(
-                f_params=p_fp, f_optimizer=o_fp, f_history=h_fp)
+            net_fit_criterion.save_params(
+                f_params=p_fp, f_optimizer=o_fp, f_criterion=c_fp, f_history=h_fp)
 
             # 'step' is state from the Adam optimizer
             orig_steps = [v['step'] for v in
-                          net_fit_adam.optimizer_.state_dict()['state'].values()]
-            orig_loss = np.array(net_fit_adam.history[:, 'train_loss'])
-            del net_fit_adam
+                          net_fit_criterion.optimizer_.state_dict()['state'].values()]
+            orig_loss = np.array(net_fit_criterion.history[:, 'train_loss'])
+            orig_criterion_weight = dict(net_fit_criterion.criterion_.named_parameters())[
+                'sequential.0.weight']
+            del net_fit_criterion
 
         with ExitStack() as stack:
             p_fp = stack.enter_context(open(str(p), 'rb'))
             o_fp = stack.enter_context(open(str(o), 'rb'))
+            c_fp = stack.enter_context(open(str(c), 'rb'))
             h_fp = stack.enter_context(open(str(h), 'r'))
             new_net = net_cls(
-                module_cls, optimizer=torch.optim.Adam).initialize()
+                module_cls, criterion=module_cls, optimizer=torch.optim.Adam).initialize()
             new_net.load_params(
-                f_params=p_fp, f_optimizer=o_fp, f_history=h_fp)
+                f_params=p_fp, f_optimizer=o_fp, f_criterion=c_fp, f_history=h_fp)
 
             new_steps = [v['step'] for v in
                          new_net.optimizer_.state_dict()['state'].values()]
             new_loss = np.array(new_net.history[:, 'train_loss'])
 
             assert np.allclose(orig_loss, new_loss)
             assert orig_steps == new_steps
+            new_criterion_weight = dict(new_net.criterion_.named_parameters())[
+                'sequential.0.weight']
+            assert (orig_criterion_weight == new_criterion_weight).all()
 
     def test_save_load_state_dict_str_with_history_optimizer(
             self, net_cls, module_cls, net_fit_adam, tmpdir):
 
         skorch_tmpdir = tmpdir.mkdir('skorch')
         p = str(skorch_tmpdir.join('testmodel.pkl'))
         o = str(skorch_tmpdir.join('optimizer.pkl'))
@@ -569,29 +643,32 @@
     def test_save_and_load_from_checkpoint(
             self, net_cls, module_cls, data, checkpoint_cls, tmpdir,
             explicit_init):
 
         skorch_dir = tmpdir.mkdir('skorch')
         f_params = skorch_dir.join('params.pt')
         f_optimizer = skorch_dir.join('optimizer.pt')
+        f_criterion = skorch_dir.join('criterion.pt')
         f_history = skorch_dir.join('history.json')
 
         cp = checkpoint_cls(
             monitor=None,
             f_params=str(f_params),
             f_optimizer=str(f_optimizer),
+            f_criterion=str(f_criterion),
             f_history=str(f_history))
         net = net_cls(
             module_cls, max_epochs=4, lr=0.1,
             optimizer=torch.optim.Adam, callbacks=[cp])
         net.fit(*data)
         del net
 
         assert f_params.exists()
         assert f_optimizer.exists()
+        assert f_criterion.exists()
         assert f_history.exists()
 
         new_net = net_cls(
             module_cls, max_epochs=4, lr=0.1,
             optimizer=torch.optim.Adam, callbacks=[cp])
         if explicit_init:
             new_net.initialize()
@@ -631,33 +708,37 @@
             scoring=epoch_3_scorer, on_train=True)
 
         skorch_dir = tmpdir.mkdir('skorch')
         f_params = skorch_dir.join(
             'model_epoch_{last_epoch[epoch]}.pt')
         f_optimizer = skorch_dir.join(
             'optimizer_epoch_{last_epoch[epoch]}.pt')
+        f_criterion = skorch_dir.join(
+            'criterion_epoch_{last_epoch[epoch]}.pt')
         f_history = skorch_dir.join(
             'history.json')
 
         cp = checkpoint_cls(
             monitor='epoch_3_scorer',
             f_params=str(f_params),
             f_optimizer=str(f_optimizer),
+            f_criterion=str(f_criterion),
             f_history=str(f_history))
 
         net = net_cls(
             module_cls, max_epochs=5, lr=0.1,
             optimizer=torch.optim.Adam, callbacks=[
                 ('my_score', scoring), cp
             ])
         net.fit(*data)
         del net
 
         assert skorch_dir.join('model_epoch_3.pt').exists()
         assert skorch_dir.join('optimizer_epoch_3.pt').exists()
+        assert skorch_dir.join('criterion_epoch_3.pt').exists()
         assert skorch_dir.join('history.json').exists()
 
         new_net = net_cls(
             module_cls, max_epochs=5, lr=0.1,
             optimizer=torch.optim.Adam, callbacks=[
                 ('my_score', scoring), cp
             ])
@@ -683,15 +764,15 @@
         net = net_cls(module_cls).initialize_module()
         skorch_tmpdir = tmpdir.mkdir('skorch')
         p = skorch_tmpdir.join('testmodel.pkl')
         o = skorch_tmpdir.join('optimizer.pkl')
 
         with pytest.raises(NotInitializedError) as exc:
             net.save_params(f_params=str(p), f_optimizer=o)
-        expected = ("Cannot save state of an un-initialized optimizer. "
+        expected = ("Cannot save state of an un-initialized model. "
                     "Please initialize first by calling .initialize() "
                     "or by fitting the model with .fit(...).")
         assert exc.value.args[0] == expected
 
     def test_load_params_not_init_optimizer(
             self, net_cls, module_cls, tmpdir):
         from skorch.exceptions import NotInitializedError
@@ -701,43 +782,43 @@
         p = skorch_tmpdir.join('testmodel.pkl')
         o = skorch_tmpdir.join('optimizer.pkl')
 
         net.save_params(f_params=str(p))
 
         with pytest.raises(NotInitializedError) as exc:
             net.load_params(f_params=str(p), f_optimizer=o)
-        expected = ("Cannot load state of an un-initialized optimizer. "
+        expected = ("Cannot load state of an un-initialized model. "
                     "Please initialize first by calling .initialize() "
                     "or by fitting the model with .fit(...).")
         assert exc.value.args[0] == expected
 
     def test_save_state_dict_not_init(
             self, net_cls, module_cls, tmpdir):
         from skorch.exceptions import NotInitializedError
 
         net = net_cls(module_cls)
         p = tmpdir.mkdir('skorch').join('testmodel.pkl')
 
         with pytest.raises(NotInitializedError) as exc:
             net.save_params(f_params=str(p))
-        expected = ("Cannot save parameters of an un-initialized model. "
+        expected = ("Cannot save state of an un-initialized model. "
                     "Please initialize first by calling .initialize() "
                     "or by fitting the model with .fit(...).")
         assert exc.value.args[0] == expected
 
     def test_load_state_dict_not_init(
             self, net_cls, module_cls, tmpdir):
         from skorch.exceptions import NotInitializedError
 
         net = net_cls(module_cls)
         p = tmpdir.mkdir('skorch').join('testmodel.pkl')
 
         with pytest.raises(NotInitializedError) as exc:
             net.load_params(f_params=str(p))
-        expected = ("Cannot load parameters of an un-initialized model. "
+        expected = ("Cannot load state of an un-initialized model. "
                     "Please initialize first by calling .initialize() "
                     "or by fitting the model with .fit(...).")
         assert exc.value.args[0] == expected
 
     @pytest.mark.skipif(not torch.cuda.is_available(), reason="no cuda device")
     def test_save_load_state_cuda_intercompatibility(
             self, net_cls, module_cls, tmpdir):
@@ -1265,44 +1346,33 @@
         )
         # none of this raises an exception
         net = clone(net)
         net.get_params()
         net.initialize()
         net.get_params()
 
-    @pytest.mark.new_get_params_behavior
-    @pytest.mark.xfail(strict=True)
     def test_get_params_no_learned_params(self, net_fit):
-        # TODO: This test should fail for now but should succeed once
-        # we change the behavior of get_params to be more in line with
-        # sklearn. At that point, remove the decorators.
         params = net_fit.get_params()
         params_learned = set(filter(lambda x: x.endswith('_'), params))
         assert not params_learned
 
-    @pytest.mark.new_get_params_behavior
-    @pytest.mark.xfail(strict=True)
     def test_clone_results_in_uninitialized_net(
             self, net_fit, data):
-        # TODO: This test should fail for now but should succeed once
-        # we change the behavior of get_params to be more in line with
-        # sklearn. At that point, remove the decorators.
         X, y = data
         accuracy = accuracy_score(net_fit.predict(X), y)
         assert accuracy > ACCURACY_EXPECTED  # make sure net has learned
 
         net_cloned = clone(net_fit).set_params(max_epochs=0)
         net_cloned.callbacks_ = []
         net_cloned.partial_fit(X, y)
         accuracy_cloned = accuracy_score(net_cloned.predict(X), y)
         assert accuracy_cloned < ACCURACY_EXPECTED
 
         assert not net_cloned.history
 
-    @pytest.mark.new_get_params_behavior
     def test_clone_copies_parameters(self, net_cls, module_cls):
         kwargs = dict(
             module__hidden_units=20,
             lr=0.2,
             iterator_train__batch_size=123,
         )
         net = net_cls(module_cls, **kwargs)
@@ -1755,15 +1825,15 @@
             module_cls,
             train_split=CVSplit(stratified=True),
         )
         ds = dataset_cls(*data)
         with pytest.raises(ValueError) as exc:
             net.fit(ds, None)
 
-        msg = "Stratified CV requires explicitely passing a suitable y."
+        msg = "Stratified CV requires explicitly passing a suitable y."
         assert exc.value.args[0] == msg
 
     @pytest.fixture
     def dataset_1_item(self):
         class Dataset(torch.utils.data.Dataset):
             def __len__(self):
                 return 100
@@ -2135,22 +2205,33 @@
 
         train_batch_count = int(0.8 * len(X)) / batch_size
         valid_batch_count = int(0.2 * len(X)) / batch_size
 
         assert net.history[:, "train_batch_count"] == [train_batch_count]
         assert net.history[:, "valid_batch_count"] == [valid_batch_count]
 
+    @flaky(max_runs=5)
     def test_fit_lbfgs_optimizer(self, net_cls, module_cls, data):
+        # need to randomize the seed, otherwise flaky always runs with
+        # the exact same seed
+        torch.manual_seed(int(time.time()))
         X, y = data
         net = net_cls(
             module_cls,
             optimizer=torch.optim.LBFGS,
-            batch_size=len(X))
+            lr=1.0,
+            batch_size=-1,
+        )
         net.fit(X, y)
 
+        last_epoch = net.history[-1]
+        assert last_epoch['train_loss'] < 1.0
+        assert last_epoch['valid_loss'] < 1.0
+        assert last_epoch['valid_acc'] > 0.75
+
     def test_accumulator_that_returns_last_value(
             self, net_cls, module_cls, data):
         # We define an optimizer that calls the step function 3 times
         # and an accumulator that returns the last of those calls. We
         # then test that the correct values were stored.
         from skorch.utils import FirstStepAccumulator
 
@@ -2268,14 +2349,46 @@
 
         net.set_params(optimizer__param_groups__0__lr=lr_pgroup_0_new)
         net.set_params(optimizer__param_groups__1__lr=lr_pgroup_1_new)
 
         assert net.optimizer_.param_groups[0]['lr'] == lr_pgroup_0_new
         assert net.optimizer_.param_groups[1]['lr'] == lr_pgroup_1_new
 
+    def test_criterion_training_set_correctly(self, net_cls, module_cls, data):
+        # check that criterion's training attribute is set correctly
+
+        X, y = data[0][:50], data[1][:50]  # don't need all the data
+        side_effect = []
+
+        class MyCriterion(nn.NLLLoss):
+            """Criterion that records its training attribute"""
+            def forward(self, *args, **kwargs):
+                side_effect.append(self.training)
+                return super().forward(*args, **kwargs)
+
+        net = net_cls(module_cls, criterion=MyCriterion, max_epochs=1)
+        net.fit(X, y)
+
+        # called once with training=True for train step, once with
+        # training=False for validation step
+        assert side_effect == [True, False]
+
+        net.partial_fit(X, y)
+        # same logic as before
+        assert side_effect == [True, False, True, False]
+
+    def test_criterion_is_not_a_torch_module(self, net_cls, module_cls, data):
+        X, y = data[0][:50], data[1][:50]  # don't need all the data
+
+        def my_criterion():
+            return torch.nn.functional.nll_loss
+
+        net = net_cls(module_cls, criterion=my_criterion, max_epochs=1)
+        net.fit(X, y)  # does not raise
+
     @pytest.mark.parametrize('acc_steps', [1, 2, 3, 5, 10])
     def test_gradient_accumulation(self, net_cls, module_cls, data, acc_steps):
         # Test if gradient accumulation technique is possible,
         # i.e. performing a weight update only every couple of
         # batches.
         mock_optimizer = Mock()
 
@@ -2323,14 +2436,298 @@
         b = np.ceil(n / net.batch_size)  # batches per epoch
         s = b // acc_steps  # number of acc steps per epoch
         calls_total = s * max_epochs
         calls_step = mock_optimizer.step.call_count
         calls_zero_grad = mock_optimizer.zero_grad.call_count
         assert calls_total == calls_step == calls_zero_grad
 
+    def test_setattr_module(self, net_cls, module_cls):
+        net = net_cls(module_cls)
+        assert 'mymodule' not in net.prefixes_
+        assert 'mymodule' not in net.cuda_dependent_attributes_
+
+        class MyNet(net_cls):
+            def __init__(self, *args, **kwargs):
+                super().__init__(*args, **kwargs)
+                self.mymodule = module_cls
+
+        net = MyNet(module_cls)
+        assert 'mymodule' in net.prefixes_
+        assert 'mymodule_' in net.cuda_dependent_attributes_
+
+        del net.mymodule
+        assert 'mymodule' not in net.prefixes_
+        assert 'mymodule_' not in net.cuda_dependent_attributes_
+
+    def test_setattr_module_instance(self, net_cls, module_cls):
+        net = net_cls(module_cls)
+        assert 'mymodule' not in net.prefixes_
+        assert 'mymodule' not in net.cuda_dependent_attributes_
+
+        class MyNet(net_cls):
+            def __init__(self, *args, **kwargs):
+                super().__init__(*args, **kwargs)
+                self.mymodule = module_cls()
+
+        net = MyNet(module_cls)
+        assert 'mymodule' in net.prefixes_
+        assert 'mymodule_' in net.cuda_dependent_attributes_
+
+        del net.mymodule
+        assert 'mymodule' not in net.prefixes_
+        assert 'mymodule_' not in net.cuda_dependent_attributes_
+
+    def test_setattr_optimizer(self, net_cls, module_cls):
+        net = net_cls(module_cls)
+        assert 'myoptimizer' not in net.prefixes_
+        assert 'myoptimizer' not in net.cuda_dependent_attributes_
+
+        class MyNet(net_cls):
+            def __init__(self, *args, **kwargs):
+                super().__init__(*args, **kwargs)
+                self.myoptimizer = torch.optim.SGD
+
+        net = MyNet(module_cls)
+        assert 'myoptimizer' in net.prefixes_
+        assert 'myoptimizer_' in net.cuda_dependent_attributes_
+
+        del net.myoptimizer
+        assert 'myoptimizer' not in net.prefixes_
+        assert 'myoptimizer_' not in net.cuda_dependent_attributes_
+
+    def test_setattr_ending_in_underscore(self, net_cls, module_cls):
+        # attributes whose name ends in underscore should not be
+        # registered
+        class MyNet(net_cls):
+            def __init__(self, *args, **kwargs):
+                super().__init__(*args, **kwargs)
+                self.mymodule_ = module_cls
+
+        net = MyNet(module_cls)
+        assert 'mymodule' not in net.prefixes_
+        assert 'mymodule_' not in net.prefixes_
+        assert 'mymodule_' not in net.cuda_dependent_attributes_
+
+    def test_setattr_no_duplicates(self, net_cls, module_cls):
+        # the 'module' attribute is set twice but that shouldn't lead
+        # to duplicates in prefixes_ or cuda_dependent_attributes_
+        class MyNet(net_cls):
+            def __init__(self, *args, **kwargs):
+                super().__init__(*args, **kwargs)
+                self.module = module_cls
+
+        net = MyNet(module_cls)
+        assert net.prefixes_.count('module') == 1
+        assert net.cuda_dependent_attributes_.count('module_') == 1
+
+    def test_setattr_non_torch_attribute(self, net_cls, module_cls):
+        # attributes that are not torch modules or optimizers should
+        # not be registered
+        class MyNet(net_cls):
+            def __init__(self, *args, **kwargs):
+                super().__init__(*args, **kwargs)
+                self.num = 123
+
+        net = MyNet(module_cls)
+        assert 'num' not in net.prefixes_
+        assert 'num_' not in net.cuda_dependent_attributes_
+
+    def test_setattr_does_not_modify_class_attribute(self, net_cls, module_cls):
+        net = net_cls(module_cls)
+        assert 'mymodule' not in net.prefixes_
+        assert 'mymodule' not in net.cuda_dependent_attributes_
+
+        class MyNet(net_cls):
+            def __init__(self, *args, **kwargs):
+                super().__init__(*args, **kwargs)
+                self.mymodule = module_cls
+
+        net = MyNet(module_cls)
+        assert 'mymodule' in net.prefixes_
+        assert 'mymodule_' in net.cuda_dependent_attributes_
+
+        assert 'mymodule' not in net_cls.prefixes_
+        assert 'mymodule_' not in net_cls.cuda_dependent_attributes_
+
+    @pytest.fixture
+    def net_custom_module_cls(self, net_cls, module_cls):
+        class MyNet(net_cls):
+            """Net with custom attribute mymodule"""
+            def __init__(self, *args, mymodule=module_cls, **kwargs):
+                self.mymodule = mymodule
+                super().__init__(*args, **kwargs)
+
+            def initialize_module(self, *args, **kwargs):
+                super().initialize_module(*args, **kwargs)
+
+                params = self.get_params_for('mymodule')
+                self.mymodule_ = self.mymodule(**params)
+
+                return self
+
+        return MyNet
+
+    def test_set_params_on_custom_module(self, net_custom_module_cls, module_cls):
+        # set_params requires the prefixes_ attribute to be correctly
+        # set, which is what is tested here
+        net = net_custom_module_cls(module_cls, mymodule__hidden_units=77).initialize()
+        hidden_units = net.mymodule_.state_dict()['sequential.3.weight'].shape[1]
+        assert hidden_units == 77
+
+        net.set_params(mymodule__hidden_units=99)
+        hidden_units = net.mymodule_.state_dict()['sequential.3.weight'].shape[1]
+        assert hidden_units == 99
+
+    def test_save_load_state_dict_custom_module(
+            self, net_custom_module_cls, module_cls, tmpdir):
+        # test that we can store and load an arbitrary attribute like 'mymodule'
+        net = net_custom_module_cls(module_cls).initialize()
+        weights_before = net.mymodule_.state_dict()['sequential.3.weight']
+        tmpdir_mymodule = str(tmpdir.mkdir('skorch').join('mymodule.pkl'))
+        net.save_params(f_mymodule=tmpdir_mymodule)
+        del net
+
+        # initialize a new net, weights should differ
+        net_new = net_custom_module_cls(module_cls).initialize()
+        weights_new = net_new.mymodule_.state_dict()['sequential.3.weight']
+        assert not (weights_before == weights_new).all()
+
+        # after loading, weights should be the same again
+        net_new.load_params(f_mymodule=tmpdir_mymodule)
+        weights_loaded = net_new.mymodule_.state_dict()['sequential.3.weight']
+        assert (weights_before == weights_loaded).all()
+
+    @pytest.mark.parametrize("needs_y, train_split, raises", [
+        (False, None, ExitStack()),  # ExitStack = does not raise
+        (True, None, ExitStack()),
+        (False, "default", ExitStack()),  # Default parameters for NeuralNet
+        (True, "default", ExitStack()),  # Default parameters for NeuralNet
+        (False, lambda x: (x, x), ExitStack()),  # Earlier this was not allowed
+        (True, lambda x, y: (x, x), ExitStack()),  # Works for custom split
+        (True, lambda x: (x, x), pytest.raises(TypeError)),  # Raises an error
+    ])
+    def test_passes_y_to_train_split_when_not_none(
+            self, needs_y, train_split, raises):
+        from skorch.net import NeuralNet
+        from skorch.toy import MLPModule
+
+        # By default, `train_split=CVSplit(5)` in the `NeuralNet` definition
+        kwargs = {} if train_split == 'default' else {
+            'train_split': train_split}
+
+        # Dummy loss that ignores y_true
+        class UnsupervisedLoss(torch.nn.NLLLoss):
+            def forward(self, y_pred, _):
+                return y_pred.mean()
+
+        # Generate the dummy dataset
+        n_samples, n_features = 128, 10
+        X = np.random.rand(n_samples, n_features).astype(np.float32)
+        y = np.random.binomial(n=1, p=0.5, size=n_samples) if needs_y else None
+
+        # The `NeuralNetClassifier` or `NeuralNetRegressor` always require `y`
+        # Only `NeuralNet` can transfer `y=None` to `train_split` method.
+        net = NeuralNet(
+            MLPModule,  # Any model, it's not important here
+            module__input_units=n_features,
+            max_epochs=2,  # Run train loop twice to detect possible errors
+            criterion=UnsupervisedLoss,
+            **kwargs,
+        )
+
+        # Check if the code should fail or not
+        with raises:
+            net.fit(X, y)
+
+    def test_predict_nonlinearity_called_with_predict(
+            self, net_cls, module_cls, data):
+        side_effect = []
+        def nonlin(X):
+            side_effect.append(X)
+            return np.zeros_like(X)
+
+        X, y = data[0][:200], data[1][:200]
+        net = net_cls(
+            module_cls, max_epochs=1, predict_nonlinearity=nonlin).initialize()
+
+        # don't want callbacks to trigger side effects
+        net.callbacks_ = []
+        net.partial_fit(X, y)
+        assert not side_effect
+
+        # 2 calls, since batch size == 128 and n == 200
+        y_proba = net.predict(X)
+        assert len(side_effect) == 2
+        assert side_effect[0].shape == (128, 2)
+        assert side_effect[1].shape == (72, 2)
+        assert (y_proba == 0).all()
+
+        net.predict(X)
+        assert len(side_effect) == 4
+
+    def test_predict_nonlinearity_called_with_predict_proba(
+            self, net_cls, module_cls, data):
+        side_effect = []
+        def nonlin(X):
+            side_effect.append(X)
+            return np.zeros_like(X)
+
+        X, y = data[0][:200], data[1][:200]
+        net = net_cls(
+            module_cls, max_epochs=1, predict_nonlinearity=nonlin).initialize()
+
+        net.callbacks_ = []
+        # don't want callbacks to trigger side effects
+        net.partial_fit(X, y)
+        assert not side_effect
+
+        # 2 calls, since batch size == 128 and n == 200
+        y_proba = net.predict_proba(X)
+        assert len(side_effect) == 2
+        assert side_effect[0].shape == (128, 2)
+        assert side_effect[1].shape == (72, 2)
+        assert np.allclose(y_proba, 0)
+
+        net.predict_proba(X)
+        assert len(side_effect) == 4
+
+    def test_predict_nonlinearity_none(
+            self, net_cls, module_cls, data):
+        # even though we have CrossEntropyLoss, we don't want the
+        # output from predict_proba to be modified, thus we set
+        # predict_nonlinearity to None
+        X = data[0][:200]
+        net = net_cls(
+            module_cls,
+            max_epochs=1,
+            criterion=nn.CrossEntropyLoss,
+            predict_nonlinearity=None,
+        ).initialize()
+
+        rv = np.random.random((20, 5))
+        net.forward_iter = lambda *args, **kwargs: (torch.as_tensor(rv) for _ in range(2))
+
+        # 2 batches, mock return value has shape 20,5 thus y_proba has
+        # shape 40,5
+        y_proba = net.predict_proba(X)
+        assert y_proba.shape == (40, 5)
+        assert np.allclose(y_proba[:20], rv)
+        assert np.allclose(y_proba[20:], rv)
+
+    def test_predict_nonlinearity_type_error(self, net_cls, module_cls):
+        # if predict_nonlinearity is not callable, raise a TypeError
+        net = net_cls(module_cls, predict_nonlinearity=123).initialize()
+
+        msg = "predict_nonlinearity has to be a callable, 'auto' or None"
+        with pytest.raises(TypeError, match=msg):
+            net.predict(np.zeros((3, 3)))
+
+        with pytest.raises(TypeError, match=msg):
+            net.predict_proba(np.zeros((3, 3)))
+
 
 class TestNetSparseInput:
     @pytest.fixture(scope='module')
     def net_cls(self):
         from skorch import NeuralNetClassifier
         return NeuralNetClassifier
 
@@ -2357,25 +2754,23 @@
         return np.asarray(lines)
 
     @pytest.fixture(scope='module')
     def y(self, X):
         return np.array(
             [1 if (' def ' in x) or (' assert ' in x) else 0 for x in X])
 
-    @flaky(max_runs=3)
     def test_fit_sparse_csr_learns(self, model, X, y):
         model.fit(X, y)
         net = model.steps[-1][1]
         score_start = net.history[0]['train_loss']
         score_end = net.history[-1]['train_loss']
 
         assert score_start > 1.25 * score_end
 
     @pytest.mark.skipif(not torch.cuda.is_available(), reason="no cuda device")
-    @flaky(max_runs=3)
     def test_fit_sparse_csr_learns_cuda(self, model, X, y):
         model.set_params(net__device='cuda')
         model.fit(X, y)
         net = model.steps[-1][1]
         score_start = net.history[0]['train_loss']
         score_end = net.history[-1]['train_loss']
```

### Comparing `skorch-0.8.0/skorch/tests/test_regressor.py` & `skorch-0.9.0/skorch/tests/test_regressor.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,25 +1,20 @@
 """Tests for regressor.py
 
 Only contains tests that are specific for regressor subclasses.
 
 """
 
-from flaky import flaky
 import numpy as np
 import pytest
 from sklearn.base import clone
-import torch
 
 from skorch.tests.conftest import INFERENCE_METHODS
 
 
-torch.manual_seed(0)
-
-
 class TestNeuralNetRegressor:
     @pytest.fixture(scope='module')
     def data(self, regression_data):
         return regression_data
 
     @pytest.fixture(scope='module')
     def module_cls(self):
@@ -76,15 +71,14 @@
             list(getattr(net, method)(X))
 
         msg = ("This NeuralNetRegressor instance is not initialized "
                "yet. Call 'initialize' or 'fit' with appropriate arguments "
                "before using this method.")
         assert exc.value.args[0] == msg
 
-    @flaky(max_runs=3)
     def test_net_learns(self, net, net_cls, data, module_cls):
         X, y = data
         net = net_cls(
             module_cls,
             max_epochs=10,
             lr=0.1,
         )
@@ -115,17 +109,17 @@
         # predictions should not be all zeros
         assert not np.allclose(y_pred, 0)
 
         y_proba = net_fit.predict_proba(X)
         # predict and predict_proba should be identical for regression
         assert np.allclose(y_pred, y_proba, atol=1e-6)
 
-    def test_score(self, net, data):
+    def test_score(self, net_fit, data):
         X, y = data
-        r2_score = net.score(X, y)
+        r2_score = net_fit.score(X, y)
         assert r2_score <= 1.
 
     def test_multioutput_score(self, multioutput_net, multioutput_regression_data):
         X, y = multioutput_regression_data
         multioutput_net.fit(X, y)
         r2_score = multioutput_net.score(X, y)
         assert r2_score <= 1.
```

### Comparing `skorch-0.8.0/skorch/tests/test_setter.py` & `skorch-0.9.0/skorch/tests/test_setter.py`

 * *Files identical despite different names*

### Comparing `skorch-0.8.0/skorch/tests/test_toy.py` & `skorch-0.9.0/skorch/tests/test_toy.py`

 * *Files identical despite different names*

### Comparing `skorch-0.8.0/skorch/tests/test_utils.py` & `skorch-0.9.0/skorch/tests/test_utils.py`

 * *Files 24% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 import pytest
 from scipy import sparse
 import torch
 from torch.nn.utils.rnn import PackedSequence
 from torch.nn.utils.rnn import pack_padded_sequence
 
 from skorch.tests.conftest import pandas_installed
-
+from copy import deepcopy
 
 class TestToTensor:
     @pytest.fixture
     def to_tensor(self):
         from skorch.utils import to_tensor
         return to_tensor
 
@@ -131,14 +131,77 @@
             to_tensor(inp, device=device)
 
         msg = ("Sparse matrices are not supported. Set "
                "accept_sparse=True to allow sparse matrices.")
         assert exc.value.args[0] == msg
 
 
+class TestToNumpy:
+    @pytest.fixture
+    def to_numpy(self):
+        from skorch.utils import to_numpy
+        return to_numpy
+
+    @pytest.fixture
+    def x_tensor(self):
+        return torch.zeros(3, 4)
+
+    @pytest.fixture
+    def x_tuple(self):
+        return torch.ones(3), torch.zeros(3, 4)
+
+    @pytest.fixture
+    def x_list(self):
+        return [torch.ones(3), torch.zeros(3, 4)]
+
+    @pytest.fixture
+    def x_dict(self):
+        return {'a': torch.ones(3), 'b': (torch.zeros(2), torch.zeros(3))}
+
+    def compare_array_to_tensor(self, x_numpy, x_tensor):
+        assert isinstance(x_tensor, torch.Tensor)
+        assert isinstance(x_numpy, np.ndarray)
+        assert x_numpy.shape == x_tensor.shape
+        for a, b in zip(x_numpy.flatten(), x_tensor.flatten()):
+            assert np.isclose(a, b.item())
+
+    def test_tensor(self, to_numpy, x_tensor):
+        x_numpy = to_numpy(x_tensor)
+        self.compare_array_to_tensor(x_numpy, x_tensor)
+
+    def test_list(self, to_numpy, x_list):
+        x_numpy = to_numpy(x_list)
+        for entry_numpy, entry_torch in zip(x_numpy, x_list):
+            self.compare_array_to_tensor(entry_numpy, entry_torch)
+
+    def test_tuple(self, to_numpy, x_tuple):
+        x_numpy = to_numpy(x_tuple)
+        for entry_numpy, entry_torch in zip(x_numpy, x_tuple):
+            self.compare_array_to_tensor(entry_numpy, entry_torch)
+
+    def test_dict(self, to_numpy, x_dict):
+        x_numpy = to_numpy(x_dict)
+        self.compare_array_to_tensor(x_numpy['a'], x_dict['a'])
+        self.compare_array_to_tensor(x_numpy['b'][0], x_dict['b'][0])
+        self.compare_array_to_tensor(x_numpy['b'][1], x_dict['b'][1])
+
+    @pytest.mark.parametrize('x_invalid', [
+        1,
+        [1,2,3],
+        (1,2,3),
+        {'a': 1},
+    ])
+    def test_invalid_inputs(self, to_numpy, x_invalid):
+        # Inputs that are invalid for the scope of to_numpy.
+        with pytest.raises(TypeError) as e:
+            to_numpy(x_invalid)
+        expected = "Cannot convert this data type to a numpy array."
+        assert e.value.args[0] == expected
+
+
 class TestToDevice:
     @pytest.fixture
     def to_device(self):
         from skorch.utils import to_device
         return to_device
 
     @pytest.fixture
@@ -146,19 +209,30 @@
         return torch.zeros(3)
 
     @pytest.fixture
     def x_tup(self):
         return torch.zeros(3), torch.ones((4, 5))
 
     @pytest.fixture
+    def x_dict(self):
+        return {
+            'x': torch.zeros(3),
+            'y': torch.ones((4, 5))
+        }
+
+    @pytest.fixture
     def x_pad_seq(self):
         value = torch.zeros((5, 3)).float()
         length = torch.as_tensor([2, 2, 1])
         return pack_padded_sequence(value, length)
 
+    @pytest.fixture
+    def x_list(self):
+        return [torch.zeros(3), torch.ones(2, 4)]
+
     def check_device_type(self, tensor, device_input, prev_device):
         """assert expected device type conditioned on the input argument for `to_device`"""
         if None is device_input:
             assert tensor.device.type == prev_device
 
         else:
             assert tensor.device.type == device_input
@@ -211,14 +285,44 @@
     @pytest.mark.parametrize('device_from, device_to', [
         ('cpu', 'cpu'),
         ('cpu', 'cuda'),
         ('cuda', 'cpu'),
         ('cuda', 'cuda'),
         (None, None),
     ])
+    def test_check_device_dict_torch_tensor(
+            self, to_device, x_dict, device_from, device_to):
+        if 'cuda' in (device_from, device_to) and not torch.cuda.is_available():
+            pytest.skip()
+
+        original_x_dict = deepcopy(x_dict)
+
+        prev_devices=[None for _ in range(len(list(x_dict.keys())))]
+        if None in (device_from, device_to):
+            prev_devices = [x.device.type for x in x_dict.values()]
+
+        new_x_dict = to_device(x_dict, device=device_from)
+        for xi, prev_d in zip(new_x_dict.values(), prev_devices):
+            self.check_device_type(xi, device_from, prev_d)
+
+        new_x_dict = to_device(new_x_dict, device=device_to)
+        for xi, prev_d in zip(new_x_dict.values(), prev_devices):
+            self.check_device_type(xi, device_to, prev_d)
+
+        assert x_dict.keys() == original_x_dict.keys()
+        for k in x_dict:
+            assert np.allclose(x_dict[k], original_x_dict[k])
+
+    @pytest.mark.parametrize('device_from, device_to', [
+        ('cpu', 'cpu'),
+        ('cpu', 'cuda'),
+        ('cuda', 'cpu'),
+        ('cuda', 'cuda'),
+        (None, None),
+    ])
     def test_check_device_packed_padded_sequence(
             self, to_device, x_pad_seq, device_from, device_to):
         if 'cuda' in (device_from, device_to) and not torch.cuda.is_available():
             pytest.skip()
 
         prev_device = None
         if None in (device_from, device_to):
@@ -226,14 +330,44 @@
 
         x_pad_seq = to_device(x_pad_seq, device=device_from)
         self.check_device_type(x_pad_seq.data, device_from, prev_device)
 
         x_pad_seq = to_device(x_pad_seq, device=device_to)
         self.check_device_type(x_pad_seq.data, device_to, prev_device)
 
+    @pytest.mark.parametrize('device_from, device_to', [
+        ('cpu', 'cpu'),
+        ('cpu', 'cuda'),
+        ('cuda', 'cpu'),
+        ('cuda', 'cuda'),
+        (None, None),
+    ])
+    def test_nested_data(self, to_device, x_list, device_from, device_to):
+        # Sometimes data is nested because it would need to be padded so it's
+        # easier to return a list of tensors with different shapes.
+        # to_device should honor this.
+        if 'cuda' in (device_from, device_to) and not torch.cuda.is_available():
+            pytest.skip()
+
+        prev_devices = [None for _ in range(len(x_list))]
+        if None in (device_from, device_to):
+            prev_devices = [x.device.type for x in x_list]
+
+        x_list = to_device(x_list, device=device_from)
+        assert isinstance(x_list, list)
+
+        for xi, prev_d in zip(x_list, prev_devices):
+            self.check_device_type(xi, device_from, prev_d)
+
+        x_list = to_device(x_list, device=device_to)
+        assert isinstance(x_list, list)
+
+        for xi, prev_d in zip(x_list, prev_devices):
+            self.check_device_type(xi, device_to, prev_d)
+
 
 class TestDuplicateItems:
     @pytest.fixture
     def duplicate_items(self):
         from skorch.utils import duplicate_items
         return duplicate_items
 
@@ -665,7 +799,73 @@
         lazy_gen = lazy_generator_cls(list_gen())
 
         first_return = list(lazy_gen)
         second_return = [item for item in lazy_gen]
 
         assert first_return == expected_list
         assert second_return == expected_list
+
+
+class TestInferPredictNonlinearity:
+    @pytest.fixture
+    def infer_predict_nonlinearity(self):
+        from skorch.utils import _infer_predict_nonlinearty
+        return _infer_predict_nonlinearty
+
+    @pytest.fixture
+    def net_clf_cls(self):
+        from skorch import NeuralNetClassifier
+        return NeuralNetClassifier
+
+    @pytest.fixture
+    def net_bin_clf_cls(self):
+        from skorch import NeuralNetBinaryClassifier
+        return NeuralNetBinaryClassifier
+
+    @pytest.fixture
+    def net_regr_cls(self):
+        from skorch import NeuralNetRegressor
+        return NeuralNetRegressor
+
+    def test_infer_neural_net_classifier_default(
+            self, infer_predict_nonlinearity, net_clf_cls, module_cls):
+        # default NeuralNetClassifier: no output nonlinearity
+        net = net_clf_cls(module_cls).initialize()
+        fn = infer_predict_nonlinearity(net)
+
+        X = np.random.random((20, 5))
+        out = fn(X)
+        assert out is X
+
+    def test_infer_neural_net_classifier_crossentropy_loss(
+            self, infer_predict_nonlinearity, net_clf_cls, module_cls):
+        # CrossEntropyLoss criteron: nonlinearity should return valid probabilities
+        net = net_clf_cls(module_cls, criterion=torch.nn.CrossEntropyLoss).initialize()
+        fn = infer_predict_nonlinearity(net)
+
+        X = torch.rand((20, 5))
+        out = fn(X).numpy()
+        assert np.allclose(out.sum(axis=1), 1.0)
+        assert ((0 <= out) & (out <= 1.0)).all()
+
+    def test_infer_neural_binary_net_classifier_default(
+            self, infer_predict_nonlinearity, net_bin_clf_cls, module_cls):
+        # BCEWithLogitsLoss should return valid probabilities
+        net = net_bin_clf_cls(module_cls).initialize()
+        fn = infer_predict_nonlinearity(net)
+
+        X = torch.rand(20)  # binary classifier returns 1-dim output
+        X = 10 * X - 5.0  # random values from -5 to 5
+        out = fn(X).numpy()
+        assert out.shape == (20, 2)  # output should be 2-dim
+        assert np.allclose(out.sum(axis=1), 1.0)
+        assert ((0 <= out) & (out <= 1.0)).all()
+
+    def test_infer_neural_net_regressor_default(
+            self, infer_predict_nonlinearity, net_regr_cls, module_cls):
+        # default NeuralNetRegressor: no output nonlinearity
+        net = net_regr_cls(module_cls).initialize()
+        fn = infer_predict_nonlinearity(net)
+
+        X = np.random.random((20, 5))
+        out = fn(X)
+        assert out is X
```

### Comparing `skorch-0.8.0/skorch/toy.py` & `skorch-0.9.0/skorch/toy.py`

 * *Files identical despite different names*

### Comparing `skorch-0.8.0/skorch/utils.py` & `skorch-0.9.0/skorch/utils.py`

 * *Files 14% similar despite different names*

```diff
@@ -2,25 +2,27 @@
 
 Should not have any dependency on other skorch packages.
 
 """
 
 from collections.abc import Sequence
 from contextlib import contextmanager
+from distutils.version import LooseVersion
 from enum import Enum
 from functools import partial
 from itertools import tee
-from distutils.version import LooseVersion
 import pathlib
 import warnings
 
 import numpy as np
 from scipy import sparse
 import sklearn
 import torch
+from torch.nn import BCEWithLogitsLoss
+from torch.nn import CrossEntropyLoss
 from torch.nn.utils.rnn import PackedSequence
 from torch.utils.data.dataset import Subset
 
 from skorch.exceptions import DeviceWarning
 from skorch.exceptions import NotInitializedError
 
 if LooseVersion(sklearn.__version__) >= '0.22.0':
@@ -100,23 +102,33 @@
 
     raise TypeError("Cannot convert this data type to a torch tensor.")
 
 
 def to_numpy(X):
     """Generic function to convert a pytorch tensor to numpy.
 
+    This function tries to unpack the tensor(s) from supported
+    data structures (e.g., dicts, lists, etc.) but doesn't go
+    beyond.
+
     Returns X when it already is a numpy array.
 
     """
     if isinstance(X, np.ndarray):
         return X
 
+    if isinstance(X, dict):
+        return {key: to_numpy(val) for key, val in X.items()}
+
     if is_pandas_ndframe(X):
         return X.values
 
+    if isinstance(X, (tuple, list)):
+        return type(X)(to_numpy(x) for x in X)
+
     if not is_torch_data_type(X):
         raise TypeError("Cannot convert this data type to a numpy array.")
 
     if X.is_cuda:
         X = X.cpu()
 
     if X.requires_grad:
@@ -131,28 +143,32 @@
     Parameters
     ----------
     X : input data
         Deals with X being a:
 
          * torch tensor
          * tuple of torch tensors
+         * dict of torch tensors
          * PackSequence instance
          * torch.nn.Module
 
     device : str, torch.device
         The compute device to be used. If device=None, return the input
         unmodified
 
     """
     if device is None:
         return X
 
+    if isinstance(X, dict):
+        return {key: to_device(val,device) for key, val in X.items()}
+
     # PackedSequence class inherits from a namedtuple
-    if isinstance(X, tuple) and (type(X) != PackedSequence):
-        return tuple(x.to(device) for x in X)
+    if isinstance(X, (tuple, list)) and (type(X) != PackedSequence):
+        return type(X)(to_device(x, device) for x in X)
     return X.to(device)
 
 
 def get_dim(y):
     """Return the number of dimensions of a torch tensor or numpy
     array-like object.
 
@@ -471,15 +487,15 @@
             self.step = step
 
     def get_step(self):
         """Return the stored step."""
         return self.step
 
 
-def _make_split(X, y, valid_ds, **kwargs):
+def _make_split(X, valid_ds, **kwargs):
     """Used by ``predefined_split`` to allow for pickling"""
     return X, valid_ds
 
 
 def freeze_parameter(param):
     """Convenience function to freeze a passed torch parameter.
     Used by ``skorch.callbacks.Freezer``
@@ -526,27 +542,136 @@
 
     """
     if msg is None:
         msg = ("This %(name)s instance is not initialized yet. Call "
                "'initialize' or 'fit' with appropriate arguments "
                "before using this method.")
 
-
     if not isinstance(attributes, (list, tuple)):
         attributes = [attributes]
 
     if not all_or_any([hasattr(estimator, attr) for attr in attributes]):
         raise NotInitializedError(msg % {'name': type(estimator).__name__})
 
 
+def _identity(x):
+    """Return input as is, the identity operation"""
+    return x
+
+
+def _sigmoid_then_2d(x):
+    """Transform 1-dim logits to valid y_proba
+
+    Sigmoid is applied to x to transform it to probabilities. Then
+    concatenate the probabilities with 1 - these probabilities to
+    return a correctly formed ``y_proba``. This is required for
+    sklearn, which expects probabilities to be 2d arrays whose sum
+    along axis 1 is 1.0.
+
+    Parameters
+    ----------
+    x : torch.tensor
+      A 1 dimensional float torch tensor containing raw logits.
+
+    Returns
+    -------
+    y_proba : torch.tensor
+      A 2 dimensional float tensor of probabilities that sum up to 1
+      on axis 1.
+
+    """
+    prob = torch.sigmoid(x)
+    y_proba = torch.stack((1 - prob, prob), 1)
+    return y_proba
+
+
+def _infer_predict_nonlinearty(net):
+    """Infers the correct nonlinearity to apply for this net
+
+    The nonlinearity is applied only when calling
+    :func:`~skorch.classifier.NeuralNetClassifier.predict` or
+    :func:`~skorch.classifier.NeuralNetClassifier.predict_proba`.
+
+    """
+    # Implementation: At the moment, this function "dispatches" only
+    # based on the criterion, not the class of the net. We still pass
+    # the whole net as input in case we want to modify this at a
+    # future point in time.
+    criterion = net.criterion_
+
+    if isinstance(criterion, CrossEntropyLoss):
+        return partial(torch.softmax, dim=-1)
+
+    if isinstance(criterion, BCEWithLogitsLoss):
+        return _sigmoid_then_2d
+
+    return _identity
+
+
 class TeeGenerator:
     """Stores a generator and calls ``tee`` on it to create new generators
     when ``TeeGenerator`` is iterated over to let you iterate over the given
     generator more than once.
 
     """
     def __init__(self, gen):
         self.gen = gen
 
     def __iter__(self):
         self.gen, it = tee(self.gen)
         yield from it
+
+
+def _check_f_arguments(caller_name, **kwargs):
+    """Check file name arguments and return them
+
+    This is used for checking if arguments to, e.g., ``save_params``
+    are correct.
+
+    Parameters
+    ----------
+    caller_name : str
+      Name of caller, is only required for the error message.
+
+    kwargs : dict
+      Keyword arguments that are intended to be checked.
+
+    Returns
+    -------
+    kwargs_module : dict
+      Keyword arguments for saving/loading modules.
+
+    kwargs_other : dict
+      Keyword arguments for saving/loading everything else.
+
+    Raises
+    ------
+    TypeError
+      There are two possibilities for arguments to be
+      incorrect. First, if they're not called 'f_*'. Second, if both
+      'f_params' and 'f_module' are passed, since those designate the
+      same thing.
+
+    """
+    if kwargs.get('f_params') and kwargs.get('f_module'):
+        raise TypeError("{} called with both f_params and f_module, please choose one"
+                        .format(caller_name))
+
+    kwargs_module = {}
+    kwargs_other = {}
+    keys_other = {'f_history', 'f_pickle'}
+    for key, val in kwargs.items():
+        if not key.startswith('f_'):
+            raise TypeError(
+                "{name} got an unexpected argument '{key}', did you mean 'f_{key}'?"
+                .format(name=caller_name, key=key))
+
+        if val is None:
+            continue
+        if key in keys_other:
+            kwargs_other[key] = val
+        else:
+            # strip 'f_' prefix and attach '_', and normalize 'params' to 'module'
+            # e.g. 'f_optimizer' becomes 'optimizer_', 'f_params' becomes 'module_'
+            key = 'module_' if key == 'f_params' else key[2:] + '_'
+            kwargs_module[key] = val
+    return kwargs_module, kwargs_other
```

### Comparing `skorch-0.8.0/skorch.egg-info/PKG-INFO` & `skorch-0.9.0/skorch.egg-info/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: skorch
-Version: 0.8.0
+Version: 0.9.0
 Summary: scikit-learn compatible neural network library for pytorch
 Home-page: https://github.com/skorch-dev/skorch
 License: new BSD 3-Clause
 Description: .. image:: https://github.com/skorch-dev/skorch/blob/master/assets/skorch.svg
            :width: 30%
         
         ------------
@@ -47,53 +47,53 @@
         <https://github.com/skorch-dev/skorch/tree/master/notebooks/README.md>`__.
         
         .. code:: python
         
             import numpy as np
             from sklearn.datasets import make_classification
             from torch import nn
-            import torch.nn.functional as F
         
             from skorch import NeuralNetClassifier
         
         
             X, y = make_classification(1000, 20, n_informative=10, random_state=0)
             X = X.astype(np.float32)
             y = y.astype(np.int64)
         
             class MyModule(nn.Module):
-                def __init__(self, num_units=10, nonlin=F.relu):
+                def __init__(self, num_units=10, nonlin=nn.ReLU()):
                     super(MyModule, self).__init__()
         
                     self.dense0 = nn.Linear(20, num_units)
                     self.nonlin = nonlin
                     self.dropout = nn.Dropout(0.5)
-                    self.dense1 = nn.Linear(num_units, 10)
-                    self.output = nn.Linear(10, 2)
+                    self.dense1 = nn.Linear(num_units, num_units)
+                    self.output = nn.Linear(num_units, 2)
+                    self.softmax = nn.Softmax(dim=-1)
         
                 def forward(self, X, **kwargs):
                     X = self.nonlin(self.dense0(X))
                     X = self.dropout(X)
-                    X = F.relu(self.dense1(X))
-                    X = F.softmax(self.output(X), dim=-1)
+                    X = self.nonlin(self.dense1(X))
+                    X = self.softmax(self.output(X))
                     return X
         
         
             net = NeuralNetClassifier(
                 MyModule,
                 max_epochs=10,
                 lr=0.1,
                 # Shuffle training data on each epoch
                 iterator_train__shuffle=True,
             )
         
             net.fit(X, y)
             y_proba = net.predict_proba(X)
         
-        In an sklearn Pipeline:
+        In an `sklearn Pipeline <https://scikit-learn.org/stable/modules/generated/sklearn.pipeline.Pipeline.html>`_:
         
         .. code:: python
         
             from sklearn.pipeline import Pipeline
             from sklearn.preprocessing import StandardScaler
         
         
@@ -101,30 +101,33 @@
                 ('scale', StandardScaler()),
                 ('net', net),
             ])
         
             pipe.fit(X, y)
             y_proba = pipe.predict_proba(X)
         
-        With grid search
+        With `grid search <https://scikit-learn.org/stable/modules/generated/sklearn.model_selection.GridSearchCV.html>`_:
         
         .. code:: python
         
             from sklearn.model_selection import GridSearchCV
         
         
+            # deactivate skorch-internal train-valid split and verbose logging
+            net.set_params(train_split=False, verbose=0)
             params = {
                 'lr': [0.01, 0.02],
                 'max_epochs': [10, 20],
                 'module__num_units': [10, 20],
             }
-            gs = GridSearchCV(net, params, refit=False, cv=3, scoring='accuracy')
+            gs = GridSearchCV(net, params, refit=False, cv=3, scoring='accuracy', verbose=2)
         
             gs.fit(X, y)
-            print(gs.best_score_, gs.best_params_)
+            print("best score: {:.3f}, best params: {}".format(gs.best_score_, gs.best_params_))
+        
         
         skorch also provides many convenient features, among others:
         
         - `Learning rate schedulers <https://skorch.readthedocs.io/en/stable/callbacks.html#skorch.callbacks.LRScheduler>`_ (Warm restarts, cyclic LR and many more)
         - `Scoring using sklearn (and custom) scoring functions <https://skorch.readthedocs.io/en/stable/callbacks.html#skorch.callbacks.EpochScoring>`_
         - `Early stopping <https://skorch.readthedocs.io/en/stable/callbacks.html#skorch.callbacks.EarlyStopping>`_
         - `Checkpointing <https://skorch.readthedocs.io/en/stable/callbacks.html#skorch.callbacks.Checkpoint>`_
@@ -134,124 +137,130 @@
         
         ============
         Installation
         ============
         
         skorch requires Python 3.5 or higher.
         
+        conda installation
+        ==================
+        
+        You need a working conda installation. Get the correct miniconda for
+        your system from `here <https://conda.io/miniconda.html>`__.
+        
+        To install skorch, you need to use the conda-forge channel:
+        
+        .. code:: bash
+        
+            conda install -c conda-forge skorch
+        
+        We recommend to use a `conda virtual environment <https://docs.conda.io/projects/conda/en/latest/user-guide/tasks/manage-environments.html>`_.
+        
+        **Note**: The conda channel is *not* managed by the skorch
+        maintainers. More information is available `here
+        <https://github.com/conda-forge/skorch-feedstock>`__.
+        
         pip installation
         ================
         
         To install with pip, run:
         
         .. code:: bash
         
             pip install -U skorch
         
-        We recommend to use a virtual environment for this.
+        Again, we recommend to use a `virtual environment
+        <https://docs.python.org/3/tutorial/venv.html>`_ for this.
         
         From source
         ===========
         
-        If you would like to use the must recent additions to skorch or
-        help development, you should install skorch from source:
-        
-        .. code:: bash
-        
-            git clone https://github.com/skorch-dev/skorch.git
-            cd skorch
-            # install pytorch version for your system (see below)
-            python setup.py install
+        If you would like to use the most recent additions to skorch or
+        help development, you should install skorch from source.
         
         Using conda
-        ===========
+        -----------
         
-        You need a working conda installation. Get the correct miniconda for
-        your system from `here <https://conda.io/miniconda.html>`__.
-        
-        You can also install skorch through the conda-forge channel. 
-        The instructions for doing so are 
-        available `here <https://github.com/conda-forge/skorch-feedstock>`__.
-        **Note**: The conda channel is _not_ managed by the skorch maintainers.
-        
-        If you do not want to use conda-forge, you may install skorch using:
+        To install skorch from source using conda, proceed as follows:
         
         .. code:: bash
         
             git clone https://github.com/skorch-dev/skorch.git
             cd skorch
             conda env create
             source activate skorch
-            # install pytorch version for your system (see below)
-            python setup.py install
+            pip install .
         
         If you want to help developing, run:
         
         .. code:: bash
         
             git clone https://github.com/skorch-dev/skorch.git
             cd skorch
             conda env create
             source activate skorch
-            # install pytorch version for your system (see below)
-            conda install -c conda-forge --file requirements-dev.txt
-            python setup.py develop
+            pip install -e .
         
             py.test  # unit tests
             pylint skorch  # static code checks
         
         Using pip
-        =========
+        ---------
         
-        If you just want to use skorch, use:
+        For pip, follow these instructions instead:
         
         .. code:: bash
         
             git clone https://github.com/skorch-dev/skorch.git
             cd skorch
             # create and activate a virtual environment
             pip install -r requirements.txt
             # install pytorch version for your system (see below)
-            python setup.py install
+            pip install .
         
         If you want to help developing, run:
         
         .. code:: bash
         
             git clone https://github.com/skorch-dev/skorch.git
             cd skorch
             # create and activate a virtual environment
             pip install -r requirements.txt
             # install pytorch version for your system (see below)
             pip install -r requirements-dev.txt
-            python setup.py develop
+            pip install -e .
         
             py.test  # unit tests
             pylint skorch  # static code checks
         
         PyTorch
         =======
         
         PyTorch is not covered by the dependencies, since the PyTorch version
-        you need is dependent on your system. For installation instructions
-        for PyTorch, visit the `PyTorch website
-        <http://pytorch.org/>`__. skorch officially supports the following
-        PyTorch versions:
+        you need is dependent on your OS and device. For installation
+        instructions for PyTorch, visit the `PyTorch website
+        <http://pytorch.org/>`__. skorch officially supports the last four
+        minor PyTorch versions, which currently are:
         
-        - 1.1.0
-        - 1.2.0
         - 1.3.1
         - 1.4.0
+        - 1.5.1
+        - 1.6.0
+        
+        However, that doesn't mean that older versions don't work, just that
+        they aren't tested. Since skorch mostly relies on the stable part of
+        the PyTorch API, older PyTorch versions should work fine.
         
-        In general, this should work (assuming CUDA 9):
+        In general, running this to install PyTorch should work (assuming CUDA
+        10.2):
         
         .. code:: bash
         
             # using conda:
-            conda install pytorch cudatoolkit=9.0 -c pytorch
+            conda install pytorch cudatoolkit==10.2 -c pytorch
             # using pip
             pip install torch
         
         =============
         Communication
         =============
```

### Comparing `skorch-0.8.0/skorch.egg-info/SOURCES.txt` & `skorch-0.9.0/skorch.egg-info/SOURCES.txt`

 * *Files 5% similar despite different names*

```diff
@@ -11,14 +11,15 @@
 skorch/cli.py
 skorch/dataset.py
 skorch/exceptions.py
 skorch/helper.py
 skorch/history.py
 skorch/net.py
 skorch/regressor.py
+skorch/scoring.py
 skorch/setter.py
 skorch/toy.py
 skorch/utils.py
 skorch.egg-info/PKG-INFO
 skorch.egg-info/SOURCES.txt
 skorch.egg-info/dependency_links.txt
 skorch.egg-info/not-zip-safe
@@ -36,10 +37,11 @@
 skorch/tests/test_classifier.py
 skorch/tests/test_cli.py
 skorch/tests/test_dataset.py
 skorch/tests/test_helper.py
 skorch/tests/test_history.py
 skorch/tests/test_net.py
 skorch/tests/test_regressor.py
+skorch/tests/test_scoring.py
 skorch/tests/test_setter.py
 skorch/tests/test_toy.py
 skorch/tests/test_utils.py
```

