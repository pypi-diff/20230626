# Comparing `tmp/MLandPattern-0.2.5.tar.gz` & `tmp/MLandPattern-0.2.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "MLandPattern-0.2.5.tar", last modified: Sun Jun 25 21:49:14 2023, max compression
+gzip compressed data, was "MLandPattern-0.2.6.tar", last modified: Mon Jun 26 06:59:44 2023, max compression
```

## Comparing `MLandPattern-0.2.5.tar` & `MLandPattern-0.2.6.tar`

### file list

```diff
@@ -1,13 +1,13 @@
-drwxr-xr-x   0 pablomunoz   (501) staff       (20)        0 2023-06-25 21:49:14.265291 MLandPattern-0.2.5/
-drwxr-xr-x   0 pablomunoz   (501) staff       (20)        0 2023-06-25 21:49:14.255671 MLandPattern-0.2.5/MLandPattern/
--rw-r--r--   0 pablomunoz   (501) staff       (20)    26365 2023-06-25 21:47:18.000000 MLandPattern-0.2.5/MLandPattern/MLandPattern.py
--rw-r--r--   0 pablomunoz   (501) staff       (20)       27 2023-03-29 18:22:32.000000 MLandPattern-0.2.5/MLandPattern/__init__.py
-drwxr-xr-x   0 pablomunoz   (501) staff       (20)        0 2023-06-25 21:49:14.260180 MLandPattern-0.2.5/MLandPattern.egg-info/
--rw-r--r--   0 pablomunoz   (501) staff       (20)      235 2023-06-25 21:49:14.000000 MLandPattern-0.2.5/MLandPattern.egg-info/PKG-INFO
--rw-r--r--   0 pablomunoz   (501) staff       (20)      216 2023-06-25 21:49:14.000000 MLandPattern-0.2.5/MLandPattern.egg-info/SOURCES.txt
--rw-r--r--   0 pablomunoz   (501) staff       (20)        1 2023-06-25 21:49:14.000000 MLandPattern-0.2.5/MLandPattern.egg-info/dependency_links.txt
--rw-r--r--   0 pablomunoz   (501) staff       (20)       13 2023-06-25 21:49:14.000000 MLandPattern-0.2.5/MLandPattern.egg-info/top_level.txt
--rw-r--r--   0 pablomunoz   (501) staff       (20)      235 2023-06-25 21:49:14.263583 MLandPattern-0.2.5/PKG-INFO
--rw-r--r--   0 pablomunoz   (501) staff       (20)        0 2023-03-28 08:17:35.000000 MLandPattern-0.2.5/README.md
--rw-r--r--   0 pablomunoz   (501) staff       (20)       38 2023-06-25 21:49:14.266837 MLandPattern-0.2.5/setup.cfg
--rw-r--r--   0 pablomunoz   (501) staff       (20)      276 2023-06-25 21:47:09.000000 MLandPattern-0.2.5/setup.py
+drwxr-xr-x   0 pablomunoz   (501) staff       (20)        0 2023-06-26 06:59:44.164056 MLandPattern-0.2.6/
+drwxr-xr-x   0 pablomunoz   (501) staff       (20)        0 2023-06-26 06:59:44.160714 MLandPattern-0.2.6/MLandPattern/
+-rw-r--r--   0 pablomunoz   (501) staff       (20)    26627 2023-06-26 06:58:11.000000 MLandPattern-0.2.6/MLandPattern/MLandPattern.py
+-rw-r--r--   0 pablomunoz   (501) staff       (20)       27 2023-03-29 18:22:32.000000 MLandPattern-0.2.6/MLandPattern/__init__.py
+drwxr-xr-x   0 pablomunoz   (501) staff       (20)        0 2023-06-26 06:59:44.162909 MLandPattern-0.2.6/MLandPattern.egg-info/
+-rw-r--r--   0 pablomunoz   (501) staff       (20)      235 2023-06-26 06:59:44.000000 MLandPattern-0.2.6/MLandPattern.egg-info/PKG-INFO
+-rw-r--r--   0 pablomunoz   (501) staff       (20)      216 2023-06-26 06:59:44.000000 MLandPattern-0.2.6/MLandPattern.egg-info/SOURCES.txt
+-rw-r--r--   0 pablomunoz   (501) staff       (20)        1 2023-06-26 06:59:44.000000 MLandPattern-0.2.6/MLandPattern.egg-info/dependency_links.txt
+-rw-r--r--   0 pablomunoz   (501) staff       (20)       13 2023-06-26 06:59:44.000000 MLandPattern-0.2.6/MLandPattern.egg-info/top_level.txt
+-rw-r--r--   0 pablomunoz   (501) staff       (20)      235 2023-06-26 06:59:44.163746 MLandPattern-0.2.6/PKG-INFO
+-rw-r--r--   0 pablomunoz   (501) staff       (20)        0 2023-03-28 08:17:35.000000 MLandPattern-0.2.6/README.md
+-rw-r--r--   0 pablomunoz   (501) staff       (20)       38 2023-06-26 06:59:44.164181 MLandPattern-0.2.6/setup.cfg
+-rw-r--r--   0 pablomunoz   (501) staff       (20)      276 2023-06-26 06:59:41.000000 MLandPattern-0.2.6/setup.py
```

### Comparing `MLandPattern-0.2.5/MLandPattern/MLandPattern.py` & `MLandPattern-0.2.6/MLandPattern/MLandPattern.py`

 * *Files 3% similar despite different names*

```diff
@@ -3,60 +3,62 @@
 import scipy
 import math
 from matplotlib import pyplot as plt
 
 
 def loadCSV(pathname, class_label, attribute_names):
     """
-    Extracts the attributes and class labels of an input 
+    Extracts the attributes and class labels of an input
     csv file dataset
     All arguments must be of equal length.
     :param pathname: path to the data file
     :param class_label: list with class label names
     :param attribute_names: list with attribute names
     :return: two numpy arrays, one with the attributes and another
             with the class labels as numbers, ranging from [0, n]
     """
     # Read the CSV file
     df = pd.read_csv(pathname, header=None)
 
     # Extract the attributes from the dataframe
-    attribute = np.array(df.iloc[:, 0:len(attribute_names)])
+    attribute = np.array(df.iloc[:, 0 : len(attribute_names)])
     attribute = attribute.T
-    
+
     # Re-assign the values of the class names to numeric values
     label_list = []
     for lab in df.loc[:, len(attribute_names)]:
         label_list.append(class_label.index(lab))
     label = np.array(label_list)
     return attribute, label
 
+
 def split_db(D, L, ratio, seed=0):
-    '''
+    """
     Splits a dataset D into a training set and a validation set, based on the ratio
     :param D: matrix of attributes of the dataset
     :param L: vector of labels of the dataset
     :param ratio: ratio used to divide the dataset (e.g. 2 / 3)
     :param seed: seed for the random number generator of numpy (default 0)
     :return (DTR, LTR), (DTE, LTE): (DTR, LTR) attributes and labels releated to the training sub-set. (DTE, LTE) attributes and labels releated to the testing sub-set.
 
-    '''
+    """
     nTrain = int(D.shape[1] * ratio)
     np.random.seed(seed)
     idx = np.random.permutation(D.shape[1])
     idxTrain = idx[0:nTrain]
     idxTest = idx[nTrain:]
 
     DTR = D[:, idxTrain]
     DTE = D[:, idxTest]
     LTR = L[idxTrain]
     LTE = L[idxTest]
 
     return (DTR, LTR), (DTE, LTE)
 
+
 def load(pathname, vizualization=0):
     """
     Loads simple csv, assuming first n-1 columns as attributes, and n col as class labels
     :param pathname: path to the data file
     :param vizualization: flag to determine if print on console dataframe head (default false)
     :return: attributes, labels. attrributes contains a numpy matrix with the attributes of the dataset. labels contains a numpy matrix
             with the class labels as numbers, ranging from [0, n]
@@ -67,14 +69,15 @@
     attribute = np.array(df.iloc[:, 0 : len(df.columns) - 1])
     attribute = attribute.T
     # print(attribute)
     label = np.array(df.iloc[:, -1])
 
     return attribute, label
 
+
 def vcol(vector):
     """
     Reshape a vector row vector into a column vector
     :param vector: a numpy row vector
     :return: the vector reshaped as a column vector
     """
     column_vector = vector.reshape((vector.size, 1))
@@ -111,26 +114,26 @@
     each row
     """
     mean = mean_of_matrix_rows(matrix)
     centered_data = matrix - mean
     return centered_data
 
 
-def covariance(matrix, centered = 0):
+def covariance(matrix, centered=0):
     """
     Calculates the Sample Covariance Matrix of a centered-matrix
     :param matrix: Matrix of data points
     :param centered: Flag to determine if matrix data is centered (default is False)
     :return: The data covariance matrix
     """
     if not centered:
         matrix = center_data(matrix)
     n = matrix.shape[1]
     cov = np.dot(matrix, matrix.T)
-    cov = np.multiply(cov, 1/n)
+    cov = np.multiply(cov, 1 / n)
     return cov
 
 
 def eigen(matrix):
     """
     Calculates the eigen value and vectors for a matrix
     :param matrix: Matrix of data points
@@ -196,15 +199,15 @@
         norm_means = np.subtract(m_class, m_general)
         matr = np.multiply(nc, np.dot(norm_means, norm_means.T))
         between_cov = np.add(between_cov, matr)
     between_cov = np.divide(between_cov, N)
     return between_cov
 
 
-def between_within_covariance (matrix_values, label):
+def between_within_covariance(matrix_values, label):
     """
     Calculates both the average within covariance, and the between covariance of all classes on a dataset
     :param matrix_values: matrix with the values associated to the parameters of the dataset
     :param label: vector with the label values associated with the dataset
     :return:a matrix with the total average covariance within each class, and the covariance between each class
     """
     Sw = covariance_within_class(matrix_values, label)
@@ -238,52 +241,50 @@
     plt.legend()
     plt.show()
 
 
 def logpdf_GAU_ND(x, mu, C):
     """
     Calculates the Logarithmic MultiVariate Gaussian Density for a set of vector values
-    :param x: matrix of the datapoints of a dataset, with a size (n x m) 
+    :param x: matrix of the datapoints of a dataset, with a size (n x m)
     :param mu: row vector with the mean associated to each dimension
     :param C: Covariance matrix
     :return: a matrix with the Gaussian Density associated with each point of X, over each dimension
     """
     M = C.shape[1]
     inv_C = np.linalg.inv(C)
     # print(inv_C.shape)
     [_, log_C] = np.linalg.slogdet(C)
 
-    #print(log_C)
-    log_2pi = -M * math.log(2*math.pi)
-    x_norm = x-mu
+    # print(log_C)
+    log_2pi = -M * math.log(2 * math.pi)
+    x_norm = x - mu
     inter_value = np.dot(x_norm.T, inv_C)
     dot_mul = np.dot(inter_value, x_norm)
     dot_mul = np.diag(dot_mul)
 
-    y = (log_2pi - log_C - dot_mul)/2
+    y = (log_2pi - log_C - dot_mul) / 2
     return y
 
 
-def logLikelihood (X, mu, c, tot=0):
+def logLikelihood(X, mu, c, tot=0):
     """
     Calculates the Logarithmic Maximum Likelihood estimator
-    :param X: matrix of the datapoints of a dataset, with a size (n x m) 
+    :param X: matrix of the datapoints of a dataset, with a size (n x m)
     :param mu: row vector with the mean associated to each dimension
     :param c: Covariance matrix
     :param tot: flag to define if it returns value per datapoint, or total sum of logLikelihood (default is False)
     :return: the logarithm of the likelihood of the datapoints, and the associated gaussian density
     """
     M = c.shape[1]
     logN = logpdf_GAU_ND(X, mu, c)
     if tot:
         return logN.sum()
     else:
         return logN
-    
-
 
 
 def multiclass_covariance(matrix, labels):
     """
     Calculates the Covariance for each class in  dataset
     :param matrix: matrix of the datapoints of a dataset
     :param labels: row vector with the labels associated with each row of data points
@@ -329,35 +330,37 @@
     class_labels = np.unique(train_labels)
     cov = multiclass_covariance(train_data, train_labels)
     # print(cov[0])
     multi_mu = multiclass_mean(train_data, train_labels)
     # print(multi_mu[0])
     densities = []
     for i in range(class_labels.size):
-        densities.append(np.exp(logLikelihood(test_data, vcol(multi_mu[i,:]), cov[i])))
+        densities.append(np.exp(logLikelihood(test_data, vcol(multi_mu[i, :]), cov[i])))
     S = np.array(densities)
     SJoint = S * prior_probability
     SMarginal = vrow(SJoint.sum(0))
-    SPost = SJoint/SMarginal
+    SPost = SJoint / SMarginal
     predictions = np.argmax(SPost, axis=0)
 
-    if(len(test_label) != 0):
+    if len(test_label) != 0:
         acc = 0
         for i in range(len(test_label)):
             if predictions[i] == test_label[i]:
                 acc += 1
-        acc/=len(test_label)
-        acc = round(acc*100, 2)
+        acc /= len(test_label)
+        acc = round(acc * 100, 2)
         # print(f'Accuracy: {acc}%')
         # print(f'Error: {(100 - acc)}%')
 
     return S, predictions, acc
 
 
-def MVG_log_classifier(train_data, train_labels, test_data, prior_probability, test_label=[]):
+def MVG_log_classifier(
+    train_data, train_labels, test_data, prior_probability, test_label=[]
+):
     """
     Calculates the model of the MultiVariate Gaussian classifier on the logarithm dimension for a set of data, and applyes it to a test dataset
     :param train_date: matrix of the datapoints of a dataset used to train the model
     :param train_labels: row vector with the labels associated with each row of the training dataset
     :param test_data: matrix of the datapoints of a dataset used to test the model
     :param test_labels: row vector with the labels associated with each row of the test dataset
     :param prior_probability: col vector associated with the prior probability for each dimension
@@ -368,36 +371,38 @@
     class_labels = np.unique(train_labels)
     cov = multiclass_covariance(train_data, train_labels)
     # print(cov[0])
     multi_mu = multiclass_mean(train_data, train_labels)
     # print(multi_mu[0])
     densities = []
     for i in range(class_labels.size):
-        densities.append(logLikelihood(test_data, vcol(multi_mu[i,:]), cov[i]))
+        densities.append(logLikelihood(test_data, vcol(multi_mu[i, :]), cov[i]))
     S = np.array(densities)
     logSJoint = S + np.log(prior_probability)
     logSMarginal = vrow(scipy.special.logsumexp(logSJoint, axis=0))
     logSPost = logSJoint - logSMarginal
     SPost = np.exp(logSPost)
     predictions = np.argmax(SPost, axis=0)
 
-    if(len(test_label) != 0):
+    if len(test_label) != 0:
         acc = 0
         for i in range(len(test_label)):
             if predictions[i] == test_label[i]:
                 acc += 1
-        acc/=len(test_label)
-        acc = round(acc*100, 2)
+        acc /= len(test_label)
+        acc = round(acc * 100, 2)
         # print(f'Accuracy: {acc}%')
         # print(f'Error: {(100 - acc)}%')
 
     return S, predictions, acc
 
 
-def Naive_classifier(train_data, train_labels, test_data, prior_probability, test_label=[]):
+def Naive_classifier(
+    train_data, train_labels, test_data, prior_probability, test_label=[]
+):
     """
     Calculates the model of the Naive classifier for a set of data, and applyes it to a test dataset
     :param train_date: matrix of the datapoints of a dataset used to train the model
     :param train_labels: row vector with the labels associated with each row of the training dataset
     :param test_data: matrix of the datapoints of a dataset used to test the model
     :param test_labels: row vector with the labels associated with each row of the test dataset
     :param prior_probability: col vector associated with the prior probability for each dimension
@@ -405,40 +410,42 @@
     :return predictions: Vector associated with the prediction of the class for each test data point
     :return acc: Accuracy of the validation set
     """
     class_labels = np.unique(train_labels)
     cov = multiclass_covariance(train_data, train_labels)
     identity = np.eye(cov.shape[1])
     # print(identity)
-    cov = cov*identity
+    cov = cov * identity
     multi_mu = multiclass_mean(train_data, train_labels)
     # print(multi_mu[0])
     densities = []
     for i in range(class_labels.size):
-        densities.append(np.exp(logLikelihood(test_data, vcol(multi_mu[i,:]), cov[i])))
+        densities.append(np.exp(logLikelihood(test_data, vcol(multi_mu[i, :]), cov[i])))
     S = np.array(densities)
     SJoint = S * prior_probability
     SMarginal = vrow(SJoint.sum(0))
-    SPost = SJoint/SMarginal
+    SPost = SJoint / SMarginal
     predictions = np.argmax(SPost, axis=0)
 
-    if(len(test_label) != 0):
+    if len(test_label) != 0:
         acc = 0
         for i in range(len(test_label)):
             if predictions[i] == test_label[i]:
                 acc += 1
-        acc/=len(test_label)
-        acc = round(acc*100, 2)
+        acc /= len(test_label)
+        acc = round(acc * 100, 2)
         # print(f'Accuracy: {acc}%')
         # print(f'Error: {(100 - acc)}%')
 
     return S, predictions, acc
 
 
-def Naive_log_classifier(train_data, train_labels, test_data, prior_probability, test_label=[]):
+def Naive_log_classifier(
+    train_data, train_labels, test_data, prior_probability, test_label=[]
+):
     """
     Calculates the model of the Naive classifier on the logarithm realm for a set of data, and applyes it to a test dataset
     :param train_date: matrix of the datapoints of a dataset used to train the model
     :param train_labels: row vector with the labels associated with each row of the training dataset
     :param test_data: matrix of the datapoints of a dataset used to test the model
     :param test_labels: row vector with the labels associated with each row of the test dataset
     :param prior_probability: col vector associated with the prior probability for each dimension
@@ -446,52 +453,52 @@
     :return predictions: Vector associated with the prediction of the class for each test data point
     :return acc: Accuracy of the validation set
     """
     class_labels = np.unique(train_labels)
     cov = multiclass_covariance(train_data, train_labels)
     identity = np.eye(cov.shape[1])
     # print(identity)
-    cov = cov*identity
+    cov = cov * identity
     multi_mu = multiclass_mean(train_data, train_labels)
     # print(multi_mu[0])
     densities = []
     for i in range(class_labels.size):
-        densities.append(logLikelihood(test_data, vcol(multi_mu[i,:]), cov[i]))
+        densities.append(logLikelihood(test_data, vcol(multi_mu[i, :]), cov[i]))
     S = np.array(densities)
     logSJoint = S + np.log(prior_probability)
     logSMarginal = vrow(scipy.special.logsumexp(logSJoint, axis=0))
     logSPost = logSJoint - logSMarginal
     SPost = np.exp(logSPost)
     predictions = np.argmax(SPost, axis=0)
 
-    if(len(test_label) != 0):
+    if len(test_label) != 0:
         acc = 0
         for i in range(len(test_label)):
             if predictions[i] == test_label[i]:
                 acc += 1
-        acc/=len(test_label)
-        acc = round(acc*100, 2)
+        acc /= len(test_label)
+        acc = round(acc * 100, 2)
         # print(f'Accuracy: {acc}%')
         # print(f'Error: {(100 - acc)}%')
 
     return S, predictions, acc
 
 
 def TiedGaussian(train_data, train_labels, test_data, prior_probability, test_label=[]):
-    '''
+    """
     Calculates the model of the Tied Gaussian classifier for a set of data, and applyes it to a test dataset
     :param train_date: matrix of the datapoints of a dataset used to train the model
     :param train_labels: row vector with the labels associated with each row of the training dataset
     :param test_data: matrix of the datapoints of a dataset used to test the model
     :param test_labels: row vector with the labels associated with each row of the test dataset
     :param prior_probability: col vector associated with the prior probability for each dimension
     :return S: matrix associated with the probability array
     :return predictions: Vector associated with the prediction of the class for each test data point
     :return acc: Accuracy of the validation set
-    '''
+    """
     class_labels = np.unique(train_labels)
     with_cov = covariance_within_class(train_data, train_labels)
     multi_mu = multiclass_mean(train_data, train_labels)
     densities = []
     for i in range(class_labels.size):
         densities.append(
             np.exp(logLikelihood(test_data, vcol(multi_mu[i, :]), with_cov))
@@ -510,38 +517,37 @@
                 acc += 1
         acc /= len(test_label)
         # print(f"Accuracy: {acc}")
         # print(f"Error: {1 - acc}")
 
     return S, predictions, acc
 
+
 def Tied_Naive_classifier(
     train_data, train_labels, test_data, prior_probability, test_label=[]
 ):
-    '''
+    """
     Calculates the model of the Tied Naive classifier for a set of data, and applyes it to a test dataset
     :param train_date: matrix of the datapoints of a dataset used to train the model
     :param train_labels: row vector with the labels associated with each row of the training dataset
     :param test_data: matrix of the datapoints of a dataset used to test the model
     :param test_labels: row vector with the labels associated with each row of the test dataset
     :param prior_probability: col vector associated with the prior probability for each dimension
     :return S: matrix associated with the probability array
     :return predictions: Vector associated with the prediction of the class for each test data point
     :return acc: Accuracy of the validation set
-    '''
+    """
     class_labels = np.unique(train_labels)
     cov = covariance_within_class(train_data, train_labels)
     identity = np.eye(cov.shape[1])
     cov = cov * identity
     multi_mu = multiclass_mean(train_data, train_labels)
     densities = []
     for i in range(class_labels.size):
-        densities.append(
-            np.exp(logLikelihood(test_data, vcol(multi_mu[i, :]), cov))
-        )
+        densities.append(np.exp(logLikelihood(test_data, vcol(multi_mu[i, :]), cov)))
     S = np.array(densities)
     SJoint = S * prior_probability
     SMarginal = vrow(SJoint.sum(0))
     SPost = SJoint / SMarginal
     predictions = np.argmax(SPost, axis=0)
 
     if len(test_label) != 0:
@@ -551,33 +557,34 @@
                 acc += 1
         acc /= len(test_label)
         # print(f"Accuracy: {acc*100}%")
         # print(f"Error: {(1 - acc)*100}%")
 
     return S, predictions, acc
 
+
 def Generative_models(
     train_attributes, train_labels, test_attributes, prior_prob, test_labels, model
 ):
-    '''
+    """
     Calculates the desired generative model
     :param train_date: matrix of the datapoints of a dataset used to train the model
     :param train_labels: row vector with the labels associated with each row of the training dataset
     :param test_data: matrix of the datapoints of a dataset used to test the model
     :param test_labels: row vector with the labels associated with each row of the test dataset
     :param prior_probability: col vector associated with the prior probability for each dimension
     :param: `model`defines which model, based on the following criterias:
         - `mvg`: Multivariate Gaussian Model
         - `Naive`: Naive Bayes Classifier
         - `Tied Gaussian`: Tied Multivariate Gaussian Model
         - `Tied naive`: Tied Naive Bayes Classifier
     :return S: matrix associated with the probability array
     :return predictions: Vector associated with the prediction of the class for each test data point
     :return acc: Accuracy of the validation set
-    '''
+    """
     if model.lower() == "mvg":
         [Probabilities, Prediction, accuracy] = MVG_log_classifier(
             train_attributes, train_labels, test_attributes, prior_prob, test_labels
         )
     elif model.lower() == "naive":
         [Probabilities, Prediction, accuracy] = Naive_log_classifier(
             train_attributes, train_labels, test_attributes, prior_prob, test_labels
@@ -590,15 +597,16 @@
     elif model.lower() == "tied naive":
         [Probabilities, Prediction, accuracy] = Tied_Naive_classifier(
             train_attributes, train_labels, test_attributes, prior_prob, test_labels
         )
         accuracy = round(accuracy * 100, 2)
     return Probabilities, Prediction, accuracy
 
-def k_fold(k, attributes, labels, previous_prob, model="mvg"):
+
+def k_fold(k, attributes, labels, previous_prob, model="mvg", PCA_m=0):
     """
     Applies a k-fold cross validation on the dataset, applying the specified model.
     :param: `k` Number of partitions to divide the dataset
     :param: `attributes` matrix containing the whole training attributes of the dataset
     :param: `labels` the label vector related to the attribute matrix
     :param: `previous_prob` the column vector related to the prior probability of the dataset
     :param: `model` (optional). Defines the model to be applied to the model:
@@ -617,42 +625,47 @@
     model = model.lower()
     for i in range(k):
         if not i:
             validation_att = attributes[:, low:high]
             validation_labels = labels[low:high]
             train_att = attributes[:, high:]
             train_labels = labels[high:]
+            if PCA_m:
+                P, train_att = PCA(train_att, PCA_m)
+                validation_att = np.dot(P.T, validation_att)
             [S, _, acc] = Generative_models(
                 train_att,
                 train_labels,
                 validation_att,
                 previous_prob,
                 validation_labels,
-                model
+                model,
             )
             final_acc = acc
             final_S = S
             continue
         low += section_size
         high += section_size
         if high > attributes.shape[1]:
             high = attributes.shape
         validation_att = attributes[:, low:high]
         validation_labels = labels[low:high]
         train_att = attributes[:, :low]
         train_labels = labels[:low]
         train_att = np.hstack((train_att, attributes[:, high:]))
         train_labels = np.hstack((train_labels, labels[high:]))
+        if PCA_m:
+            P, train_att = PCA(train_att, PCA_m)
+            validation_att = np.dot(P.T, validation_att)
         [S, _, acc] = Generative_models(
-                train_att,
-                train_labels,
-                validation_att,
-                previous_prob,
-                validation_labels,
-                model
-            )
+            train_att,
+            train_labels,
+            validation_att,
+            previous_prob,
+            validation_labels,
+            model,
+        )
         final_acc += acc
         final_S += S
     final_acc /= k
     final_S /= k
     return final_acc, final_S
-
```

