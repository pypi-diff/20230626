# Comparing `tmp/devCellPy-1.2.0.tar.gz` & `tmp/devCellPy-1.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "devCellPy-1.2.0.tar", last modified: Sat May 20 19:46:28 2023, max compression
+gzip compressed data, was "devCellPy-1.3.0.tar", last modified: Mon Jun 26 07:15:34 2023, max compression
```

## Comparing `devCellPy-1.2.0.tar` & `devCellPy-1.3.0.tar`

### file list

```diff
@@ -1,22 +1,22 @@
-drwxr-xr-x   0 vivian     (501) staff       (20)        0 2023-05-20 19:46:28.502220 devCellPy-1.2.0/
--rw-r--r--   0 vivian     (501) staff       (20)     1063 2022-08-21 02:13:40.000000 devCellPy-1.2.0/LICENSE.txt
--rw-r--r--   0 vivian     (501) staff       (20)      756 2023-05-20 19:46:28.501551 devCellPy-1.2.0/PKG-INFO
--rw-r--r--   0 vivian     (501) staff       (20)     1665 2022-08-21 02:13:49.000000 devCellPy-1.2.0/README.md
-drwxr-xr-x   0 vivian     (501) staff       (20)        0 2023-05-20 19:46:28.498659 devCellPy-1.2.0/devCellPy/
--rw-r--r--   0 vivian     (501) staff       (20)        0 2023-05-20 18:58:00.000000 devCellPy-1.2.0/devCellPy/__init__.py
--rw-r--r--   0 vivian     (501) staff       (20)    10275 2023-05-20 18:58:25.000000 devCellPy-1.2.0/devCellPy/__main__.py
--rw-r--r--   0 vivian     (501) staff       (20)      380 2023-05-20 18:58:49.000000 devCellPy-1.2.0/devCellPy/config.py
--rw-r--r--   0 vivian     (501) staff       (20)     2471 2023-05-20 18:59:06.000000 devCellPy-1.2.0/devCellPy/featurerank.py
--rw-r--r--   0 vivian     (501) staff       (20)     1201 2023-05-20 18:59:27.000000 devCellPy-1.2.0/devCellPy/helpers.py
--rw-r--r--   0 vivian     (501) staff       (20)      529 2023-05-20 18:59:47.000000 devCellPy-1.2.0/devCellPy/importing_modules.py
--rw-r--r--   0 vivian     (501) staff       (20)    30567 2023-05-20 19:00:09.000000 devCellPy-1.2.0/devCellPy/layer.py
--rw-r--r--   0 vivian     (501) staff       (20)     7808 2023-05-20 19:00:30.000000 devCellPy-1.2.0/devCellPy/predict.py
--rw-r--r--   0 vivian     (501) staff       (20)     6347 2023-05-20 19:00:48.000000 devCellPy-1.2.0/devCellPy/train.py
-drwxr-xr-x   0 vivian     (501) staff       (20)        0 2023-05-20 19:46:28.500901 devCellPy-1.2.0/devCellPy.egg-info/
--rw-r--r--   0 vivian     (501) staff       (20)      756 2023-05-20 19:46:28.000000 devCellPy-1.2.0/devCellPy.egg-info/PKG-INFO
--rw-r--r--   0 vivian     (501) staff       (20)      398 2023-05-20 19:46:28.000000 devCellPy-1.2.0/devCellPy.egg-info/SOURCES.txt
--rw-r--r--   0 vivian     (501) staff       (20)        1 2023-05-20 19:46:28.000000 devCellPy-1.2.0/devCellPy.egg-info/dependency_links.txt
--rw-r--r--   0 vivian     (501) staff       (20)       54 2023-05-20 19:46:28.000000 devCellPy-1.2.0/devCellPy.egg-info/entry_points.txt
--rw-r--r--   0 vivian     (501) staff       (20)       10 2023-05-20 19:46:28.000000 devCellPy-1.2.0/devCellPy.egg-info/top_level.txt
--rw-r--r--   0 vivian     (501) staff       (20)       38 2023-05-20 19:46:28.502431 devCellPy-1.2.0/setup.cfg
--rw-r--r--   0 vivian     (501) staff       (20)     1095 2023-05-20 19:46:08.000000 devCellPy-1.2.0/setup.py
+drwxr-xr-x   0 vivian     (501) staff       (20)        0 2023-06-26 07:15:34.517479 devCellPy-1.3.0/
+-rw-r--r--   0 vivian     (501) staff       (20)     1063 2022-08-21 02:13:40.000000 devCellPy-1.3.0/LICENSE.txt
+-rw-r--r--   0 vivian     (501) staff       (20)      756 2023-06-26 07:15:34.517162 devCellPy-1.3.0/PKG-INFO
+-rw-r--r--   0 vivian     (501) staff       (20)     1665 2022-08-21 02:13:49.000000 devCellPy-1.3.0/README.md
+drwxr-xr-x   0 vivian     (501) staff       (20)        0 2023-06-26 07:15:34.515044 devCellPy-1.3.0/devCellPy/
+-rw-r--r--   0 vivian     (501) staff       (20)        0 2023-06-26 07:10:41.000000 devCellPy-1.3.0/devCellPy/__init__.py
+-rw-r--r--   0 vivian     (501) staff       (20)    10300 2023-06-26 07:10:41.000000 devCellPy-1.3.0/devCellPy/__main__.py
+-rw-r--r--   0 vivian     (501) staff       (20)      400 2023-06-26 07:10:41.000000 devCellPy-1.3.0/devCellPy/config.py
+-rw-r--r--   0 vivian     (501) staff       (20)     2495 2023-06-26 07:10:41.000000 devCellPy-1.3.0/devCellPy/featurerank.py
+-rw-r--r--   0 vivian     (501) staff       (20)     1200 2023-06-26 07:10:41.000000 devCellPy-1.3.0/devCellPy/helpers.py
+-rw-r--r--   0 vivian     (501) staff       (20)      579 2023-06-26 07:10:41.000000 devCellPy-1.3.0/devCellPy/importing_modules.py
+-rw-r--r--   0 vivian     (501) staff       (20)    30610 2023-06-26 07:10:41.000000 devCellPy-1.3.0/devCellPy/layer.py
+-rw-r--r--   0 vivian     (501) staff       (20)     7118 2023-06-26 07:10:41.000000 devCellPy-1.3.0/devCellPy/predict.py
+-rw-r--r--   0 vivian     (501) staff       (20)     6346 2023-06-26 07:10:41.000000 devCellPy-1.3.0/devCellPy/train.py
+drwxr-xr-x   0 vivian     (501) staff       (20)        0 2023-06-26 07:15:34.516668 devCellPy-1.3.0/devCellPy.egg-info/
+-rw-r--r--   0 vivian     (501) staff       (20)      756 2023-06-26 07:15:34.000000 devCellPy-1.3.0/devCellPy.egg-info/PKG-INFO
+-rw-r--r--   0 vivian     (501) staff       (20)      398 2023-06-26 07:15:34.000000 devCellPy-1.3.0/devCellPy.egg-info/SOURCES.txt
+-rw-r--r--   0 vivian     (501) staff       (20)        1 2023-06-26 07:15:34.000000 devCellPy-1.3.0/devCellPy.egg-info/dependency_links.txt
+-rw-r--r--   0 vivian     (501) staff       (20)       54 2023-06-26 07:15:34.000000 devCellPy-1.3.0/devCellPy.egg-info/entry_points.txt
+-rw-r--r--   0 vivian     (501) staff       (20)       10 2023-06-26 07:15:34.000000 devCellPy-1.3.0/devCellPy.egg-info/top_level.txt
+-rw-r--r--   0 vivian     (501) staff       (20)       38 2023-06-26 07:15:34.517573 devCellPy-1.3.0/setup.cfg
+-rw-r--r--   0 vivian     (501) staff       (20)     1095 2023-06-26 07:15:13.000000 devCellPy-1.3.0/setup.py
```

### Comparing `devCellPy-1.2.0/LICENSE.txt` & `devCellPy-1.3.0/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `devCellPy-1.2.0/PKG-INFO` & `devCellPy-1.3.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: devCellPy
-Version: 1.2.0
+Version: 1.3.0
 Summary: devCellPy -- hierarchical multilayered classification of cells based on scRNA-seq
 Home-page: https://github.com/devCellPy-Team/devCellPy
 Author: Sidra Xu
 Author-email: sidraxu@stanford.edu
 Maintainer: Sean Wu Lab
 Maintainer-email: smwu@stanford.edu
 License: MIT
```

### Comparing `devCellPy-1.2.0/README.md` & `devCellPy-1.3.0/README.md`

 * *Files identical despite different names*

### Comparing `devCellPy-1.2.0/devCellPy/__main__.py` & `devCellPy-1.3.0/devCellPy/__main__.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 #!/usr/bin/env python3
 # -*- coding: utf-8 -*-
 
 from .importing_modules import *
 from . import config, train, predict, featurerank
+from .layer import Layer
 
 # Ensures given files satisfy one of the possible pathways provided by devcellpy
 # Ensures user input for train or predict matches file inputs
 # Certain files must appear together for training and/or validation to proceed
 def check_combinations(user_train, user_predictOne, user_predictAll, user_fr, train_normexpr, labelinfo, train_metadata, testsplit,
                        rejection_cutoff, val_normexpr, val_metadata, layer_paths, frsplit):
     passed = True
```

### Comparing `devCellPy-1.2.0/devCellPy/featurerank.py` & `devCellPy-1.3.0/devCellPy/featurerank.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,9 +1,10 @@
 from .importing_modules import *
 from . import config, helpers
+from .layer import Layer
 
 def check_featurerankingfiles(train_normexpr, train_metadata, layer_paths, frsplit):
     passed = True
     if not os.path.exists(train_normexpr):
         print('ERROR: Given normalized expression data file for training does not exist')
         passed = False
     if not os.path.exists(train_metadata):
@@ -47,8 +48,8 @@
         path = os.path.join(config.path, layer.path)
         os.makedirs(path)
         os.chdir(path)
         path = path + '/'
         layer.featurerank_layer(train_normexpr, train_metadata, frsplit)
         os.chdir(config.path) # return to prediction directory
         path = os.getcwd()
-    print('Feature Ranking Complete')
+    print('Feature Ranking Complete')
```

### Comparing `devCellPy-1.2.0/devCellPy/helpers.py` & `devCellPy-1.3.0/devCellPy/helpers.py`

 * *Ordering differences only*

 * *Files 0% similar despite different names*

```diff
@@ -29,8 +29,8 @@
 
 # Imports Layer objects from a list of given paths
 def import_layers(layer_paths):
     layers = []
     for layer_path in layer_paths:
          layer = pd.read_pickle(layer_path)
          layers.append(layer)
-    return layers
+    return layers
```

### Comparing `devCellPy-1.2.0/devCellPy/importing_modules.py` & `devCellPy-1.3.0/devCellPy/importing_modules.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,7 +1,10 @@
+import warnings
+warnings.filterwarnings('ignore')
+
 import time
 import resource
 import sys
 import getopt
 import os
 import datetime
 import csv
@@ -13,8 +16,8 @@
 import matplotlib.pyplot as plt
 import itertools
 from numpy import interp
 from sklearn.utils import shuffle
 from sklearn.model_selection import train_test_split, StratifiedShuffleSplit
 from sklearn.metrics import classification_report, confusion_matrix, roc_curve, auc, precision_recall_curve, average_precision_score
 import shap
-import scanpy as sc
+import scanpy as sc
```

### Comparing `devCellPy-1.2.0/devCellPy/layer.py` & `devCellPy-1.3.0/devCellPy/layer.py`

 * *Files 2% similar despite different names*

```diff
@@ -121,17 +121,17 @@
     # XGBoost w/o cross validation, no output files, just accuracy score on user-provided testsplit value
     # Returns mean absolute error (mae) as float and csv output string
     #       Accuracy for each class and mae in a comma-separated string for classification
     # Only for finetuning!
     def xgboost_model_shortver(self, X_tr, X_test, Y_tr, Y_test, params):
         params['num_class'] = len(self.labeldict)
 
-        d_tr = xgb.DMatrix(X_tr, Y_tr, feature_names=feature_names)
+        d_tr = xgb.DMatrix(X_tr, Y_tr, feature_names=config.feature_names)
         model = xgb.train(params, d_tr, 20, verbose_eval=10)
-        d_test = xgb.DMatrix(X_test, Y_test, feature_names=feature_names)
+        d_test = xgb.DMatrix(X_test, Y_test, feature_names=config.feature_names)
         probabilities_xgb = model.predict(d_test)
 
         returned_str = ''
         predictions_xgb = probabilities_xgb.argmax(axis=1)
         cm = confusion_matrix(Y_test, predictions_xgb)
         cm = cm.astype('float') / cm.sum(axis=1)[:, np.newaxis]
         mae = 1-sum(cm.diagonal())/len(cm.diagonal())
@@ -154,22 +154,22 @@
             X, Y, X_tr, X_test, Y_tr, Y_test, test_cellnames = self.read_data(normexprpkl, metadatacsv, testsplit)
             kfold = 10
             sss = StratifiedShuffleSplit(n_splits=kfold, test_size=0.1, random_state=720)
             for i, (train_index, test_index) in enumerate(sss.split(X_tr, Y_tr)):
                 print('[Fold %d/%d]' % (i + 1, kfold))
                 X_train, X_valid = X_tr[train_index], X_tr[test_index]
                 Y_train, Y_valid = Y_tr[train_index], Y_tr[test_index]
-                d_train = xgb.DMatrix(X_train, Y_train, feature_names=feature_names)
+                d_train = xgb.DMatrix(X_train, Y_train, feature_names=config.feature_names)
                 cv_model = xgb.train(params, d_train, 20, verbose_eval=500)
                 self.xgbmodel = cv_model # temporarily set xgbmodel to cv 0.9*(1-testsplit)% model
                 self.model_metrics('cv', rejectcutoffs[1], X_valid, Y_valid)
                 self.cvmetrics = self.name + '_cvmetrics.txt'
 
             # 90% model, 10% testing
-            d_tr = xgb.DMatrix(X_tr, Y_tr, feature_names=feature_names)
+            d_tr = xgb.DMatrix(X_tr, Y_tr, feature_names=config.feature_names)
             temp_model = xgb.train(params, d_tr, 20, verbose_eval=500)
             self.xgbmodel = temp_model # temporarily set xgbmodel to (1-testsplit)% model
             self.model_metrics('final', rejectcutoffs[1], X_test, Y_test)
             self.finalmetrics = self.name + '_finalmetrics.txt'
             self.cell_predictions('training', rejectcutoffs, test_cellnames, X_test, Y_test)
             for cutoff in rejectcutoffs:
                 self.predictions.append(self.name + '_trainingpredictions_reject' + str(cutoff) + '.csv')
@@ -183,15 +183,15 @@
             self.pr = self.name + '_allpr.svg'
 
         # skip cross validation and metric calculations
         if testsplit is None:
             X, Y, all_cellnames = self.read_data(normexprpkl, metadatacsv)
 
         # final 100% model
-        d_all = xgb.DMatrix(X, Y, feature_names=feature_names)
+        d_all = xgb.DMatrix(X, Y, feature_names=config.feature_names)
         final_model = xgb.train(params, d_all, 20, verbose_eval=500)
         pickle.dump(final_model, open(config.path + self.path + '/' + self.name + '_xgbmodel.sav', 'wb'))
         self.xgbmodel = final_model
 
 
     # Outputs predictions of the 90% model on the 10% test set in a given dataset
     # 1 csv file outputted for each rejection cutoff in the list rejectioncutoffs
@@ -268,19 +268,18 @@
     # Reads the specified column in the metadata csv into a label dataframe
     # Metadata CSV file must contain samples as row names, first column name (cell A1) is empty
     # subsetcolumn and subsetcriterium are strings for extracting rows with the specified label in the specified column
     #                                 eg. for per timepoint classification
     #                                 can both be set to None if all samples are to be included
     # Converts norm_expr and label dataframes into numpy arrays X and Y, splits them into 90/10
     # Retrieves cell names of samples in 10% testing data
-    # global feature_names defined here, list of all gene names -> should be equivalent for all csvs (except subsetted versions)
+    # global feature_names set here, list of all gene names -> should be equivalent for all csvs (except subsetted versions)
     def read_data(self, normexprpkl, metadatacsv=None, testsplit=None):
         norm_express = pd.read_pickle(normexprpkl)
-        global feature_names
-        feature_names = list(norm_express)
+        config.feature_names = list(norm_express)
         print(norm_express.shape)
 
         # If validation w/o metadata, metadata not provided, return all data w/o subsetting
         if metadatacsv is None:
             X = norm_express.values
             norm_express.index.name = 'cells'
             norm_express.reset_index(inplace=True)
@@ -350,15 +349,15 @@
         return X, Y, X_tr, X_test, Y_tr, Y_test, test_cellnames
 
 
     # Calculates metrics of the Layer model on a provided test set and outputs it in a file
     # cv_final_val is a naming string to differentiate between cv, final, and validation metrics
     def model_metrics(self, cv_final_val, rejectcutoff, X_test, Y_test):
         self.add_dictentry('Unclassified')
-        d_test = xgb.DMatrix(X_test, Y_test, feature_names=feature_names)
+        d_test = xgb.DMatrix(X_test, Y_test, feature_names=config.feature_names)
         probabilities_xgb = self.xgbmodel.predict(d_test)
         predictions_xgb = probabilities_xgb.argmax(axis=1)
         for i in range(len(probabilities_xgb)):
             if probabilities_xgb[i,probabilities_xgb.argmax(axis=1)[i]] < rejectcutoff:
                 predictions_xgb[i] = len(self.labeldict)-1
         target_names = [str(x) for x in sorted(list(set(Y_test).union(predictions_xgb)))]
         metrics = classification_report(Y_test, predictions_xgb, target_names=target_names)
@@ -370,15 +369,15 @@
     # Outputs predictions of the Layer model on a provided test set
     # Adds a key value pair in the labeldict for an unclassified class, removes it when completed
     # 1 csv file outputted for each rejection cutoff in the list rejectioncutoffs
     # A cutoff of 0.5 means the probability of the label must be >=0.5 for a prediction to be called
     # A cutoff of 0 is equivalent to no rejection option
     # train_val is a naming string to differentiate between train/test predictions and validation predictions
     def cell_predictions(self, train_val, rejectcutoffs, test_cellnames, X_test, Y_test=None):
-        d_test = xgb.DMatrix(X_test, feature_names=feature_names)
+        d_test = xgb.DMatrix(X_test, feature_names=config.feature_names)
         probabilities_xgb = self.xgbmodel.predict(d_test)
         predictions_xgb = probabilities_xgb.argmax(axis=1)
         self.add_dictentry('Unclassified')
         for cutoff in rejectcutoffs:
             counter = 0
             for i in range(len(probabilities_xgb)):
                 if probabilities_xgb[i,probabilities_xgb.argmax(axis=1)[i]] < cutoff:
@@ -408,15 +407,15 @@
             f.close()
         del self.labeldict[len(self.labeldict)-1]
 
 
     # Outputs a confusion matrix of the Layer model's results on a provided test set
     # train_val is a naming string to differentiate between train/test predictions and validation predictions
     def cfsn_mtx(self, train_val, rejectcutoff, X_test, Y_test):
-        d_test = xgb.DMatrix(X_test, feature_names=feature_names)
+        d_test = xgb.DMatrix(X_test, feature_names=config.feature_names)
         probabilities_xgb = self.xgbmodel.predict(d_test)
         predictions_xgb = probabilities_xgb.argmax(axis=1)
         self.add_dictentry('Unclassified')
         for i in range(len(probabilities_xgb)):
             if probabilities_xgb[i,probabilities_xgb.argmax(axis=1)[i]] < rejectcutoff:
                 predictions_xgb[i] = len(self.labeldict)-1
         cm = confusion_matrix(Y_test, predictions_xgb)
@@ -453,15 +452,15 @@
         plt.clf()
 
 
     # Creates ROC curves for the Layer model on a provided test set
     # Calculates curves using probability values and thresholds
     # Outputs 3 figures: micro and macro ROC curves, per class ROC curves, and all combined
     def roc_curves(self, X_test, Y_test):
-        d_test = xgb.DMatrix(X_test, feature_names=feature_names)
+        d_test = xgb.DMatrix(X_test, feature_names=config.feature_names)
         probabilities_xgb = self.xgbmodel.predict(d_test)
         n_classes = len(self.labeldict)
         lw = 2
         y_test = np.zeros((Y_test.size, Y_test.max()+1))
         y_test[np.arange(Y_test.size),Y_test] = 1
         y_score = probabilities_xgb
         fpr = dict()
@@ -541,15 +540,15 @@
         plt.clf()
 
 
     # Creates precision-recall curves for the Layer model on a provided test set
     # Calculates curves using probability values and thresholds
     # Outputs 1 figure: per class PR curvs and a micro PR curve
     def pr_curves(self, X_test, Y_test):
-        d_test = xgb.DMatrix(X_test, feature_names=feature_names)
+        d_test = xgb.DMatrix(X_test, feature_names=config.feature_names)
         probabilities_xgb = self.xgbmodel.predict(d_test)
         n_classes = len(self.labeldict)
         lw = 2
         y_test = np.zeros((Y_test.size, Y_test.max()+1))
         y_test[np.arange(Y_test.size),Y_test] = 1
         y_score = probabilities_xgb
         precision = dict()
@@ -577,8 +576,8 @@
         plt.xlim([0.0, 1.0])
         plt.ylim([0.0, 1.05])
         plt.xlabel('Recall')
         plt.ylabel('Precision')
         plt.title('PR Curves')
         plt.legend(loc="lower left")
         plt.savefig(config.path + self.path + '/' + self.name + '_allpr.svg')
-        plt.clf()
+        plt.clf()
```

### Comparing `devCellPy-1.2.0/devCellPy/predict.py` & `devCellPy-1.3.0/devCellPy/predict.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,9 +1,10 @@
 from .importing_modules import *
 from . import config, helpers
+from .layer import Layer
 
 # Ensures all the user given variables for predictOne or predictAll exist and are in the correct format
 def check_predictionfiles(val_normexpr, val_metadata, layer_paths):
     passed = True
     if not os.path.exists(val_normexpr):
         print('ERROR: Given validation normalized expression data file for prediction does not exist')
         passed = False
@@ -30,18 +31,15 @@
     config.path = os.path.join(config.path, 'devcellpy_predictOne_' + datetime.datetime.now().strftime('%Y%m%d%H%M%S'))
     config.path += '/'
     os.makedirs(config.path)
     os.chdir(config.path)
     all_layers = helpers.import_layers(object_paths)
     featurenames = all_layers[0].xgbmodel.feature_names
     reorder_pickle(val_normexpr, featurenames)
-    if val_normexpr[-3:] == 'csv':
-        val_normexpr = val_normexpr[:-3] + 'pkl'
-    elif val_normexpr[-4:] == 'h5ad':
-        val_normexpr = val_normexpr[:-4] + 'pkl'
+    val_normexpr = val_normexpr[:val_normexpr.index('.')] + '_reordered.pkl'
     for layer in all_layers:
         path = os.path.join(config.path, layer.path)
         os.makedirs(path)
         os.chdir(path)
         path = path + '/'
         layer.predict_layer([0, config.rejection_cutoff], val_normexpr, val_metadata)
         os.chdir(config.path) # return to prediction directory
@@ -140,41 +138,23 @@
         norm_express = pd.DataFrame(adata.X.toarray(), columns = adata.var.index, index = adata.obs.index)
         norm_express.to_pickle(h5adpath[:-4] + 'pkl')
     elif path[-3:] == 'pkl':
         norm_express = pd.read_pickle(path)
     else:
         raise ValueError('Format of normalized expression data file not recognized')
     print ('Training Data # of  genes: ' + str(len(featurenames)))
+    origfeat = list(norm_express)
+    print ('Validation Data # of genes: ' + str(len(origfeat)))
+    print ('Overlapping # of genes: ' + str(len(set(featurenames).intersection(origfeat))))
 
     ## Manually reorder columns according to training data index
     # Reorder overlapping genes, remove genes not in training data
-    origfeat = list(norm_express)
-    print ('Validation Data # of genes: ' + str(len(origfeat)))
-    newindex = []
-    for i in range(len(featurenames)):
-        if featurenames[i] in origfeat:
-            newindex.append(featurenames[i])
-    print ('Overlapping # of genes: ' + str(len(newindex)))
-    norm_express = norm_express.reindex(columns=newindex)
-    # Add missing features, remove extra features to match atlas
-    i = 0
-    missing_counter = 0
-    while i < len(list(norm_express)):
-        if list(norm_express)[i] != featurenames[i]:
-            norm_express.insert(i, featurenames[i], None)
-            missing_counter += 1
-        i += 1
-    while i < len(featurenames):
-        norm_express.insert(i, featurenames[i], None)
-        i += 1
-        missing_counter += 1
-    # Overlapping + missing = training total
-    print ('Missing # of genes: ' + str(missing_counter))
+    norm_express = norm_express.reindex(columns=featurenames, fill_value=None)
     norm_express.to_pickle(path[:-4] + '_reordered.pkl')
 
 
 # Utility function, searches a list of all_layers for a layer with the given name
 def find_predictlayer(all_layers, name):
     for layer in all_layers:
         if layer.predictname == name:
             return layer
-    return None
+    return None
```

### Comparing `devCellPy-1.2.0/devCellPy/train.py` & `devCellPy-1.3.0/devCellPy/train.py`

 * *Ordering differences only*

 * *Files 0% similar despite different names*

```diff
@@ -129,8 +129,8 @@
 
 # Summarizes and lists the path names of all the files created during training
 # Prints the summary of each Layer object
 def training_summary(all_layers):
     f = open(config.path + 'training_summaryfile.txt', 'w')
     for layer in all_layers:
         f.write(str(layer))
-        f.write('\n')
+        f.write('\n')
```

### Comparing `devCellPy-1.2.0/devCellPy.egg-info/PKG-INFO` & `devCellPy-1.3.0/devCellPy.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: devCellPy
-Version: 1.2.0
+Version: 1.3.0
 Summary: devCellPy -- hierarchical multilayered classification of cells based on scRNA-seq
 Home-page: https://github.com/devCellPy-Team/devCellPy
 Author: Sidra Xu
 Author-email: sidraxu@stanford.edu
 Maintainer: Sean Wu Lab
 Maintainer-email: smwu@stanford.edu
 License: MIT
```

### Comparing `devCellPy-1.2.0/setup.py` & `devCellPy-1.3.0/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -10,15 +10,15 @@
     multilayered classification of cells based on single-cell
     RNA-sequencing (scRNA-seq). It implements the machine
     learning algorithm Extreme Gradient Boost (XGBoost)
     (Chen and Guestrin, 2016) to automatically predict cell
     identities across complex permutations of layers and
     sublayers of annotation.""",  # wrap at col 60
     url = 'https://github.com/devCellPy-Team/devCellPy',
-    version = '1.2.0',
+    version = '1.3.0',
     author = 'Sidra Xu',
     author_email = 'sidraxu@stanford.edu',
     maintainer = 'Sean Wu Lab',
     maintainer_email = 'smwu@stanford.edu',
     license = 'MIT',
     python_requires = '>=3.7',
     include_package_data = True,
```

