# Comparing `tmp/MLandPattern-0.2.6.tar.gz` & `tmp/MLandPattern-0.2.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "MLandPattern-0.2.6.tar", last modified: Mon Jun 26 06:59:44 2023, max compression
+gzip compressed data, was "MLandPattern-0.2.7.tar", last modified: Mon Jun 26 14:07:59 2023, max compression
```

## Comparing `MLandPattern-0.2.6.tar` & `MLandPattern-0.2.7.tar`

### file list

```diff
@@ -1,13 +1,13 @@
-drwxr-xr-x   0 pablomunoz   (501) staff       (20)        0 2023-06-26 06:59:44.164056 MLandPattern-0.2.6/
-drwxr-xr-x   0 pablomunoz   (501) staff       (20)        0 2023-06-26 06:59:44.160714 MLandPattern-0.2.6/MLandPattern/
--rw-r--r--   0 pablomunoz   (501) staff       (20)    26627 2023-06-26 06:58:11.000000 MLandPattern-0.2.6/MLandPattern/MLandPattern.py
--rw-r--r--   0 pablomunoz   (501) staff       (20)       27 2023-03-29 18:22:32.000000 MLandPattern-0.2.6/MLandPattern/__init__.py
-drwxr-xr-x   0 pablomunoz   (501) staff       (20)        0 2023-06-26 06:59:44.162909 MLandPattern-0.2.6/MLandPattern.egg-info/
--rw-r--r--   0 pablomunoz   (501) staff       (20)      235 2023-06-26 06:59:44.000000 MLandPattern-0.2.6/MLandPattern.egg-info/PKG-INFO
--rw-r--r--   0 pablomunoz   (501) staff       (20)      216 2023-06-26 06:59:44.000000 MLandPattern-0.2.6/MLandPattern.egg-info/SOURCES.txt
--rw-r--r--   0 pablomunoz   (501) staff       (20)        1 2023-06-26 06:59:44.000000 MLandPattern-0.2.6/MLandPattern.egg-info/dependency_links.txt
--rw-r--r--   0 pablomunoz   (501) staff       (20)       13 2023-06-26 06:59:44.000000 MLandPattern-0.2.6/MLandPattern.egg-info/top_level.txt
--rw-r--r--   0 pablomunoz   (501) staff       (20)      235 2023-06-26 06:59:44.163746 MLandPattern-0.2.6/PKG-INFO
--rw-r--r--   0 pablomunoz   (501) staff       (20)        0 2023-03-28 08:17:35.000000 MLandPattern-0.2.6/README.md
--rw-r--r--   0 pablomunoz   (501) staff       (20)       38 2023-06-26 06:59:44.164181 MLandPattern-0.2.6/setup.cfg
--rw-r--r--   0 pablomunoz   (501) staff       (20)      276 2023-06-26 06:59:41.000000 MLandPattern-0.2.6/setup.py
+drwxr-xr-x   0 pablomunoz   (501) staff       (20)        0 2023-06-26 14:07:59.204138 MLandPattern-0.2.7/
+drwxr-xr-x   0 pablomunoz   (501) staff       (20)        0 2023-06-26 14:07:59.198421 MLandPattern-0.2.7/MLandPattern/
+-rw-r--r--   0 pablomunoz   (501) staff       (20)    27039 2023-06-26 14:07:44.000000 MLandPattern-0.2.7/MLandPattern/MLandPattern.py
+-rw-r--r--   0 pablomunoz   (501) staff       (20)       27 2023-03-29 18:22:32.000000 MLandPattern-0.2.7/MLandPattern/__init__.py
+drwxr-xr-x   0 pablomunoz   (501) staff       (20)        0 2023-06-26 14:07:59.200748 MLandPattern-0.2.7/MLandPattern.egg-info/
+-rw-r--r--   0 pablomunoz   (501) staff       (20)      235 2023-06-26 14:07:59.000000 MLandPattern-0.2.7/MLandPattern.egg-info/PKG-INFO
+-rw-r--r--   0 pablomunoz   (501) staff       (20)      216 2023-06-26 14:07:59.000000 MLandPattern-0.2.7/MLandPattern.egg-info/SOURCES.txt
+-rw-r--r--   0 pablomunoz   (501) staff       (20)        1 2023-06-26 14:07:59.000000 MLandPattern-0.2.7/MLandPattern.egg-info/dependency_links.txt
+-rw-r--r--   0 pablomunoz   (501) staff       (20)       13 2023-06-26 14:07:59.000000 MLandPattern-0.2.7/MLandPattern.egg-info/top_level.txt
+-rw-r--r--   0 pablomunoz   (501) staff       (20)      235 2023-06-26 14:07:59.201553 MLandPattern-0.2.7/PKG-INFO
+-rw-r--r--   0 pablomunoz   (501) staff       (20)        0 2023-03-28 08:17:35.000000 MLandPattern-0.2.7/README.md
+-rw-r--r--   0 pablomunoz   (501) staff       (20)       38 2023-06-26 14:07:59.204371 MLandPattern-0.2.7/setup.cfg
+-rw-r--r--   0 pablomunoz   (501) staff       (20)      276 2023-06-26 14:07:49.000000 MLandPattern-0.2.7/setup.py
```

### Comparing `MLandPattern-0.2.6/MLandPattern/MLandPattern.py` & `MLandPattern-0.2.7/MLandPattern/MLandPattern.py`

 * *Files 2% similar despite different names*

```diff
@@ -598,15 +598,15 @@
         [Probabilities, Prediction, accuracy] = Tied_Naive_classifier(
             train_attributes, train_labels, test_attributes, prior_prob, test_labels
         )
         accuracy = round(accuracy * 100, 2)
     return Probabilities, Prediction, accuracy
 
 
-def k_fold(k, attributes, labels, previous_prob, model="mvg", PCA_m=0):
+def k_fold(k, attributes, labels, previous_prob, model="mvg", PCA_m=0, LDA_m=0):
     """
     Applies a k-fold cross validation on the dataset, applying the specified model.
     :param: `k` Number of partitions to divide the dataset
     :param: `attributes` matrix containing the whole training attributes of the dataset
     :param: `labels` the label vector related to the attribute matrix
     :param: `previous_prob` the column vector related to the prior probability of the dataset
     :param: `model` (optional). Defines the model to be applied to the model:
@@ -628,14 +628,18 @@
             validation_att = attributes[:, low:high]
             validation_labels = labels[low:high]
             train_att = attributes[:, high:]
             train_labels = labels[high:]
             if PCA_m:
                 P, train_att = PCA(train_att, PCA_m)
                 validation_att = np.dot(P.T, validation_att)
+                if LDA_m:
+                    W, _ = LDA1(train_att, train_labels, LDA_m)
+                    train_att = np.dot(W.T, train_att)
+                    validation_att = np.dot(W.T, validation_att)
             [S, _, acc] = Generative_models(
                 train_att,
                 train_labels,
                 validation_att,
                 previous_prob,
                 validation_labels,
                 model,
@@ -652,20 +656,24 @@
         train_att = attributes[:, :low]
         train_labels = labels[:low]
         train_att = np.hstack((train_att, attributes[:, high:]))
         train_labels = np.hstack((train_labels, labels[high:]))
         if PCA_m:
             P, train_att = PCA(train_att, PCA_m)
             validation_att = np.dot(P.T, validation_att)
+            if LDA_m:
+                W, _ = LDA1(train_att, train_labels, LDA_m)
+                train_att = np.dot(W.T, train_att)
+                validation_att = np.dot(W.T, validation_att)
         [S, _, acc] = Generative_models(
             train_att,
             train_labels,
             validation_att,
             previous_prob,
             validation_labels,
             model,
         )
         final_acc += acc
         final_S += S
     final_acc /= k
     final_S /= k
-    return final_acc, final_S
+    return final_acc, final_S
```

