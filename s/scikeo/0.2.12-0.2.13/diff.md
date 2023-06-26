# Comparing `tmp/scikeo-0.2.12.tar.gz` & `tmp/scikeo-0.2.13.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist\scikeo-0.2.12.tar", last modified: Wed Jun 14 15:31:54 2023, max compression
+gzip compressed data, was "scikeo-0.2.13.tar", last modified: Mon Jun 26 18:09:08 2023, max compression
```

## Comparing `scikeo-0.2.12.tar` & `scikeo-0.2.13.tar`

### file list

```diff
@@ -1,31 +1,31 @@
-drwxrwxrwx   0        0        0        0 2023-06-14 15:31:54.413975 scikeo-0.2.12/
--rw-rw-rw-   0        0        0      613 2023-03-17 15:59:10.000000 scikeo-0.2.12/LICENSE
--rw-rw-rw-   0        0        0      130 2023-03-17 15:59:10.000000 scikeo-0.2.12/MANIFEST.in
--rw-rw-rw-   0        0        0    10319 2023-06-14 15:31:54.413975 scikeo-0.2.12/PKG-INFO
--rw-rw-rw-   0        0        0     7948 2023-06-12 14:56:27.000000 scikeo-0.2.12/README.md
--rw-rw-rw-   0        0        0       62 2023-03-17 15:59:10.000000 scikeo-0.2.12/requirements.txt
-drwxrwxrwx   0        0        0        0 2023-06-14 15:31:54.283352 scikeo-0.2.12/scikeo/
--rw-rw-rw-   0        0        0      143 2023-03-17 15:59:10.000000 scikeo-0.2.12/scikeo/__init__.py
--rw-rw-rw-   0        0        0    10900 2023-03-17 15:59:10.000000 scikeo-0.2.12/scikeo/atmosCorr.py
--rw-rw-rw-   0        0        0     5794 2023-03-17 15:59:10.000000 scikeo-0.2.12/scikeo/calkmeans.py
--rw-rw-rw-   0        0        0    19966 2023-03-17 15:59:10.000000 scikeo-0.2.12/scikeo/calmla.py
--rw-rw-rw-   0        0        0     9681 2023-06-14 15:27:15.000000 scikeo-0.2.12/scikeo/deeplearning.py
--rw-rw-rw-   0        0        0     6113 2023-03-17 15:59:10.000000 scikeo-0.2.12/scikeo/fusionrs.py
--rw-rw-rw-   0        0        0     6668 2023-03-17 15:59:10.000000 scikeo-0.2.12/scikeo/linearTrend.py
--rw-rw-rw-   0        0        0    25713 2023-06-14 15:21:56.000000 scikeo-0.2.12/scikeo/mla.py
--rw-rw-rw-   0        0        0     5043 2023-03-17 15:59:10.000000 scikeo-0.2.12/scikeo/pca.py
--rw-rw-rw-   0        0        0     5789 2023-03-17 15:59:10.000000 scikeo-0.2.12/scikeo/plot.py
--rw-rw-rw-   0        0        0    10277 2023-04-27 16:42:51.000000 scikeo-0.2.12/scikeo/process.py
--rw-rw-rw-   0        0        0     1871 2023-03-17 15:59:10.000000 scikeo-0.2.12/scikeo/rkmeans.py
--rw-rw-rw-   0        0        0     3721 2023-06-14 15:28:55.000000 scikeo-0.2.12/scikeo/sma.py
--rw-rw-rw-   0        0        0     5235 2023-03-17 15:59:10.000000 scikeo-0.2.12/scikeo/tassCap.py
--rw-rw-rw-   0        0        0     2068 2023-03-17 15:59:10.000000 scikeo-0.2.12/scikeo/writeRaster.py
-drwxrwxrwx   0        0        0        0 2023-06-14 15:31:54.411980 scikeo-0.2.12/scikeo.egg-info/
--rw-rw-rw-   0        0        0    10319 2023-06-14 15:31:49.000000 scikeo-0.2.12/scikeo.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      516 2023-06-14 15:31:49.000000 scikeo-0.2.12/scikeo.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0       56 2023-06-14 15:31:49.000000 scikeo-0.2.12/scikeo.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        2 2023-03-20 19:51:08.000000 scikeo-0.2.12/scikeo.egg-info/not-zip-safe
--rw-rw-rw-   0        0        0       55 2023-06-14 15:31:49.000000 scikeo-0.2.12/scikeo.egg-info/requires.txt
--rw-rw-rw-   0        0        0        7 2023-06-14 15:31:49.000000 scikeo-0.2.12/scikeo.egg-info/top_level.txt
--rw-rw-rw-   0        0        0      414 2023-06-14 15:31:54.416966 scikeo-0.2.12/setup.cfg
--rw-rw-rw-   0        0        0     1756 2023-06-14 15:31:13.000000 scikeo-0.2.12/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-26 18:09:08.510575 scikeo-0.2.13/
+-rw-rw-rw-   0        0        0      613 2023-06-26 18:09:00.000000 scikeo-0.2.13/LICENSE
+-rw-rw-rw-   0        0        0      130 2023-06-26 18:09:00.000000 scikeo-0.2.13/MANIFEST.in
+-rw-rw-rw-   0        0        0     8708 2023-06-26 18:09:08.510575 scikeo-0.2.13/PKG-INFO
+-rw-rw-rw-   0        0        0     7954 2023-06-26 18:09:00.000000 scikeo-0.2.13/README.md
+-rw-rw-rw-   0        0        0       62 2023-06-26 18:09:00.000000 scikeo-0.2.13/requirements.txt
+drwxrwxrwx   0        0        0        0 2023-06-26 18:09:08.501800 scikeo-0.2.13/scikeo/
+-rw-rw-rw-   0        0        0      143 2023-06-26 18:09:00.000000 scikeo-0.2.13/scikeo/__init__.py
+-rw-rw-rw-   0        0        0    10900 2023-06-26 18:09:00.000000 scikeo-0.2.13/scikeo/atmosCorr.py
+-rw-rw-rw-   0        0        0     5794 2023-06-26 18:09:00.000000 scikeo-0.2.13/scikeo/calkmeans.py
+-rw-rw-rw-   0        0        0    19966 2023-06-26 18:09:00.000000 scikeo-0.2.13/scikeo/calmla.py
+-rw-rw-rw-   0        0        0     9941 2023-06-26 18:09:00.000000 scikeo-0.2.13/scikeo/deeplearning.py
+-rw-rw-rw-   0        0        0     6113 2023-06-26 18:09:00.000000 scikeo-0.2.13/scikeo/fusionrs.py
+-rw-rw-rw-   0        0        0     6668 2023-06-26 18:09:00.000000 scikeo-0.2.13/scikeo/linearTrend.py
+-rw-rw-rw-   0        0        0    26407 2023-06-26 18:09:00.000000 scikeo-0.2.13/scikeo/mla.py
+-rw-rw-rw-   0        0        0     5043 2023-06-26 18:09:00.000000 scikeo-0.2.13/scikeo/pca.py
+-rw-rw-rw-   0        0        0     5789 2023-06-26 18:09:00.000000 scikeo-0.2.13/scikeo/plot.py
+-rw-rw-rw-   0        0        0    10580 2023-06-26 18:09:00.000000 scikeo-0.2.13/scikeo/process.py
+-rw-rw-rw-   0        0        0     1871 2023-06-26 18:09:00.000000 scikeo-0.2.13/scikeo/rkmeans.py
+-rw-rw-rw-   0        0        0     3819 2023-06-26 18:09:00.000000 scikeo-0.2.13/scikeo/sma.py
+-rw-rw-rw-   0        0        0     5235 2023-06-26 18:09:00.000000 scikeo-0.2.13/scikeo/tassCap.py
+-rw-rw-rw-   0        0        0     2068 2023-06-26 18:09:00.000000 scikeo-0.2.13/scikeo/writeRaster.py
+drwxrwxrwx   0        0        0        0 2023-06-26 18:09:08.510575 scikeo-0.2.13/scikeo.egg-info/
+-rw-rw-rw-   0        0        0     8708 2023-06-26 18:09:08.000000 scikeo-0.2.13/scikeo.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      516 2023-06-26 18:09:08.000000 scikeo-0.2.13/scikeo.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0       56 2023-06-26 18:09:08.000000 scikeo-0.2.13/scikeo.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        2 2023-06-26 18:09:08.000000 scikeo-0.2.13/scikeo.egg-info/not-zip-safe
+-rw-rw-rw-   0        0        0       55 2023-06-26 18:09:08.000000 scikeo-0.2.13/scikeo.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        7 2023-06-26 18:09:08.000000 scikeo-0.2.13/scikeo.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0      414 2023-06-26 18:09:08.526886 scikeo-0.2.13/setup.cfg
+-rw-rw-rw-   0        0        0     1813 2023-06-26 18:09:00.000000 scikeo-0.2.13/setup.py
```

### Comparing `scikeo-0.2.12/LICENSE` & `scikeo-0.2.13/LICENSE`

 * *Files identical despite different names*

### Comparing `scikeo-0.2.12/README.md` & `scikeo-0.2.13/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -17,26 +17,26 @@
 
 Nowadays, remotely sensed data has increased dramatically. Microwaves and optical images with different spatial and temporal resolutions are available and are used to monitor a variety of environmental issues such as deforestation, land degradation, land use and land cover change, among others. Although there are efforts (i.e., Python packages, forums, communities, etc.) to make available line-of-code tools for pre-processing, processing and analysis of satellite imagery, there is still a gap that needs to be filled. In other words, too much time is still spent by many users developing Python lines of code. Algorithms for mapping land degradation through a linear trend of vegetation indices, fusion optical and radar images to classify vegetation cover, and calibration of machine learning algorithms, among others, are not available yet.
 
 Therefore, **scikit-eo** is a Python package that provides tools for remote sensing. This package was developed to fill the gaps in remotely sensed data processing tools. Most of the tools are based on scientific publications, and others are useful algorithms that will allow processing to be done in a few lines of code. With these tools, the user will be able to invest time in analyzing the results of their data and not spend time on elaborating lines of code, which can sometimes be stressful.
 
 # Tools for Remote Sensing
 
-| Name of functions  | Description|
+| Name of functions/classes  | Description|
 | -------------------| --------------------------------------------------------------------------|
 | **`mla`**          | Machine Learning (Random Forest, Support Vector Machine, Decition Tree, Naive Bayes, Neural Network, etc.)                                                          |
 | **`calmla`**       | Calibrating supervised classification in Remote Sensing (e.g., Monte Carlo Cross-Validation, Leave-One-Out Cross-Validation, etc.)                   |
 | **`confintervalML`**       | Information of confusion matrix by proportions of area, overall accuracy, user's accuracy with confidence interval and estimated area with confidence interval as well.                                    |
 | **`rkmeans`**      | K-means classification                                                    |
 | **`calkmeans`**    | This function allows to calibrate the kmeans algorithm. It is possible to obtain the best k value and the best embedded algorithm in kmeans.                               |
 | **`pca`**          | Principal Components Analysis                                             |
 | **`atmosCorr`**    | Atmospheric Correction of satellite imagery                               |
 | **`deepLearning`** | Deep Learning algorithms                                                  |
 | **`linearTrend`**  | Linear trend is useful for mapping forest degradation or land degradation |
-| **`fusionrs`**     | This algorithm allows to fusion images coming from different spectral sensors (e.g., optical-optical, optical and SAR or SAR-SAR). Among many of the qualities of this function, it is possible to obtain the contribution (%) of each variable in the fused image |
+| **`fusionrs`**     | This algorithm allows to fuse images coming from different spectral sensors (e.g., optical-optical, optical and SAR or SAR-SAR). Among many of the qualities of this function, it is possible to obtain the contribution (%) of each variable in the fused image |
 | **`sma`**          | Spectral Mixture Analysis - Classification sup-pixel                      |
 | **`tassCap`**      | The Tasseled-Cap Transformation                                           |
 
 You will find more algorithms!.
 
 
 # Installation
```

### Comparing `scikeo-0.2.12/scikeo/atmosCorr.py` & `scikeo-0.2.13/scikeo/atmosCorr.py`

 * *Files identical despite different names*

### Comparing `scikeo-0.2.12/scikeo/calkmeans.py` & `scikeo-0.2.13/scikeo/calkmeans.py`

 * *Files identical despite different names*

### Comparing `scikeo-0.2.12/scikeo/calmla.py` & `scikeo-0.2.13/scikeo/calmla.py`

 * *Files identical despite different names*

### Comparing `scikeo-0.2.12/scikeo/fusionrs.py` & `scikeo-0.2.13/scikeo/fusionrs.py`

 * *Files identical despite different names*

### Comparing `scikeo-0.2.12/scikeo/linearTrend.py` & `scikeo-0.2.13/scikeo/linearTrend.py`

 * *Files identical despite different names*

### Comparing `scikeo-0.2.12/scikeo/mla.py` & `scikeo-0.2.13/scikeo/mla.py`

 * *Ordering differences only*

 * *Files 16% similar despite different names*

```diff
@@ -1,694 +1,694 @@
-# -*- coding: utf-8 -*-
-# +
-import copy
-import rasterio
-import numpy as np
-import pandas as pd
-from dbfread import DBF
-from sklearn.svm import SVC
-from sklearn.tree import DecisionTreeClassifier as DT
-from sklearn.ensemble import RandomForestClassifier as RF
-from sklearn.naive_bayes import GaussianNB as GNB
-from sklearn.neural_network import MLPClassifier as MLP
-from sklearn.model_selection import train_test_split
-from sklearn.metrics import accuracy_score
-from sklearn.metrics import cohen_kappa_score
-from sklearn.metrics import confusion_matrix
-import warnings
-
-class MLA(object):
-    
-    'Supervised classification in Remote Sensing'
-    
-    def __init__(self, image, endmembers, nodata = -99999):
-        
-        '''
-        Parameter:
-        
-            image: Optical images. It must be rasterio.io.DatasetReader with 3d.
-            
-            endmembers: Endmembers must be a matrix (numpy.ndarray) and with more than one endmember. 
-                    Rows represent the endmembers and columns represent the spectral bands.
-                    The number of bands must be equal to the number of endmembers.
-                    E.g. an image with 6 bands, endmembers dimension should be $n*6$, where $n$ 
-                    is rows with the number of endmembers and 6 is the number of bands 
-                    (should be equal).
-                    In addition, Endmembers must have a field (type int or float) with the names 
-                    of classes to be predicted.
-            
-            nodata: The NoData value to replace with -99999.
-            
-        '''
-        
-        self.image = image
-        self.endm = endmembers
-        self.nodata = nodata
-        
-        if not isinstance(self.image, (rasterio.io.DatasetReader)):
-            raise TypeError('"image" must be raster read by rasterio.open().')
-        
-        bands = self.image.count
-        
-        rows = self.image.height
-        
-        cols = self.image.width
-        
-        st = image.read()
-        
-        # data in [rows, cols, bands]
-        st_reorder = np.moveaxis(st, 0, -1) 
-        # data in [rows*cols, bands]
-        arr = st_reorder.reshape((rows*cols, bands))
-        
-        # nodata
-        #if np.isnan(np.sum(arr)):
-            #arr[np.isnan(arr)] = self.nodata
-        
-        # dealing with nan
-        key_nan = np.isnan(np.sum(arr[:,0]))
-        
-        if key_nan:
-            # saving un array for predicted classes
-            class_final = arr[:, 0].copy()
-            # positions with nan
-            posIndx = np.argwhere(~np.isnan(class_final)).flatten()
-            # replace np.nan -> 0
-            arr[np.isnan(arr)] = 0
-        
-        # if it is read by pandas.read_csv()
-        if isinstance(self.endm, (pd.core.frame.DataFrame)):
-            
-            for i in np.arange(self.endm.shape[1]):
-                
-                if all(self.endm.iloc[:,int(i)] < 100) & all(self.endm.iloc[:,int(i)] >= 0): indx = i; break
-        
-        # if the file is .dbf    
-        elif isinstance(self.endm, (DBF)): # isinstance() function With Inheritance
-            
-            self.endm = pd.DataFrame(iter(self.endm))
-            
-            for i in np.arange(self.endm.shape[1]):
-                
-                if all(self.endm.iloc[:,int(i)] < 100) & all(self.endm.iloc[:,int(i)] >= 0): indx = i; break
-        
-        else:
-            raise TypeError('"endm" must be .csv (pandas.core.frame.DataFrame).')
-
-        if not self.endm.shape[1] == (bands + 1):
-            raise ValueError('The number of columns of signatures (included the class column) must'
-                             'be equal to the number of bands + 1.')
-        
-        self.indx = indx
-        
-        self.arr = arr
-        
-        self.rows = rows
-        
-        self.cols = cols
-        
-        if key_nan:
-            self.key_nan = key_nan
-            self.posIndx = posIndx
-            self.class_final = class_final
-        else:
-            self.key_nan = key_nan
-            
-        
-    def SVM(self, training_split = 0.8, random_state = None, kernel = 'linear', **kwargs):
-        
-        '''The Support Vector Machine (SVM) classifier is a supervised non-parametric statistical learning technique that 
-        does not assume a preliminary distribution of input data. Its discrimination criterion is a 
-        hyperplane that separates the classes in the multidimensional space in which the samples 
-        that have established the same classes are located, generally some training areas.
-        
-        SVM support raster data read by rasterio (rasterio.io.DatasetReader) as input.
-     
-        
-        Parameters:
-    
-            training_split: For splitting samples into two subsets, i.e. training data and for testing
-                            data.
-    
-            kernel : {'linear', 'poly', 'rbf', 'sigmoid', 'precomputed'}, default='rbf' Specifies 
-                     the kernel type to be used in the algorithm. It must be one of 'linear', 'poly', 
-                     'rbf', 'sigmoid', 'precomputed' or a callable. If None is given, 'rbf' will 
-                     be used. See https://scikit-learn.org/stable/modules/generated/sklearn.svm.SVC.html#sklearn.svm.SVC
-                     for more details.
-                     
-            **kwargs: These will be passed to SVM, please see full lists at:
-                  https://scikit-learn.org/stable/modules/generated/sklearn.svm.SVC.html#sklearn.svm.SVC
-    
-        Return:
-        
-            A dictionary containing labels of classification as numpy object, overall accuracy, kappa index, confusion matrix.
-        '''
-        
-        # removing the class column
-        X = self.endm.drop(self.endm.columns[[self.indx]], axis = 1)
-        
-        # only predictor variables
-        y = self.endm.iloc[:, self.indx]
-        
-        # split in training and testing
-        Xtrain, Xtest, ytrain, ytest = train_test_split(
-            X.values, 
-            y.values, 
-            train_size = training_split, 
-            test_size = 1 - training_split, 
-            random_state = random_state)
-        
-        # applying a support vector machine
-        inst_svm = SVC(kernel = kernel, **kwargs)
-        
-        # model trained
-        mt_svm = inst_svm.fit(Xtrain, ytrain)
-        
-        labels_svm = mt_svm.predict(self.arr)
-        
-        # dealing with nan
-        if self.key_nan:
-            # image border like nan
-            labels_svm = labels_svm[self.posIndx]
-            self.class_final[self.posIndx] = labels_svm
-            classSVM = self.class_final.reshape((self.rows, self.cols))
-        else:
-            classSVM = labels_svm.reshape((self.rows, self.cols))
-        
-        # Confusion matrix
-        predic_Xtest = mt_svm.predict(Xtest)
-        
-        MC = confusion_matrix(ytest, predic_Xtest)
-    
-        MC = np.transpose(MC)
-
-        # Users Accuracy and Commission
-        total_rows = np.sum(MC, axis = 1)
-        ua = np.diag(MC)/np.sum(MC, axis = 1)*100
-        co = 100 - ua
-
-        # Producer Accuracy and Comission
-        total_cols = np.sum(MC, axis = 0)
-        pa = np.diag(MC)/np.sum(MC, axis = 0)*100
-        om = 100 - pa
-
-        total_cols = np.concatenate([total_cols, np.repeat(np.nan, 3)])
-        pa = np.concatenate([pa, np.repeat(np.nan, 3)])
-        om = np.concatenate([om, np.repeat(np.nan, 3)])
-
-        n = MC.shape[0]
-        cm = np.concatenate([MC, total_rows.reshape((n,1)), ua.reshape((n,1)), 
-                             co.reshape((n,1))], axis = 1)
-        cm = np.concatenate([cm, total_cols.reshape((1,n+3)), pa.reshape((1,n+3)), 
-                             om.reshape((1,n+3))])
-
-        min_class = np.nanmin(labels_svm)
-        max_class = np.nanmax(labels_svm)
-        
-        namesCol = []
-        for i in np.arange(min_class, max_class + 1):
-            stri = str(i)
-            namesCol.append(stri)
-
-        namesCol.extend(['Total', 'Users_Accuracy', 'Commission'])
-
-        namesRow = []
-        for i in np.arange(min_class, max_class + 1):
-            stri = str(i)
-            namesRow.append(stri)
-
-        namesRow.extend(['Total', 'Producer_Accuracy', 'Omission'])
-        namesRow
-
-        confusionMatrix = pd.DataFrame(cm, 
-                                        columns = namesCol, 
-                                        index = namesRow)
-
-        oa = accuracy_score(ytest, predic_Xtest)
-        kappa = cohen_kappa_score(ytest, predic_Xtest)
-        
-        output = {'Overall_Accuracy': oa,
-                  'Kappa_Index': kappa,
-                  'Confusion_Matrix': confusionMatrix,
-                  'Classification_Map': classSVM,
-                  'Image': self.image
-                 } 
-    
-        return output
-    
-    def DT(self, training_split = 0.8, random_state = None, **kwargs):
-        
-        '''Decision Tree is also a supervised non-parametric statistical learning technique, where the input data is divided recursively 
-        into branches depending on certain decision thresholds until the data are segmented into homogeneous subgroups. 
-        This technique has substantial advantages for remote sensing classification problems due to its flexibility, intuitive simplicity, 
-        and computational efficiency.
-        
-        DT support raster data read by rasterio (rasterio.io.DatasetReader) as input.
-        
-        
-        Parameters:
-    
-            training_split: For splitting samples into two subsets, i.e. training data and for testing
-                            data.
-                     
-            **kwargs: These will be passed to DT, please see full lists at:
-                  https://scikit-learn.org/stable/modules/generated/sklearn.tree.DecisionTreeClassifier.html#sklearn.tree.DecisionTreeClassifier
-    
-        Return:
-        
-            A dictionary containing labels of classification as numpy object, overall accuracy, kappa index, confusion matrix.
-        '''
-        
-        # removing the class column
-        X = self.endm.drop(self.endm.columns[[self.indx]], axis = 1)
-            
-        # only predictor variables
-        y = self.endm.iloc[:, self.indx]
-        
-        # split in training and testing
-        Xtrain, Xtest, ytrain, ytest = train_test_split(
-            X.values, 
-            y.values, 
-            train_size = training_split, 
-            test_size = 1 - training_split, 
-            random_state = random_state)
-        
-        # applying a support vector machine
-        inst_dt = DT(**kwargs)
-        
-        # model trained
-        mt_dt = inst_dt.fit(Xtrain, ytrain)
-        
-        labels_dt = mt_dt.predict(self.arr)
-        
-        # dealing with nan
-        if self.key_nan:
-            # image border like nan
-            labels_dt = labels_dt[self.posIndx]
-            self.class_final[self.posIndx] = labels_dt
-            classDT = self.class_final.reshape((self.rows, self.cols))
-        else:
-            classDT = labels_dt.reshape((self.rows, self.cols))
-        
-        # Confusion matrix
-        predic_Xtest = mt_dt.predict(Xtest)
-        
-        MC = confusion_matrix(ytest, predic_Xtest)
-    
-        MC = np.transpose(MC)
-
-        # Users Accuracy and Commission
-        total_rows = np.sum(MC, axis = 1)
-        ua = np.diag(MC)/np.sum(MC, axis = 1)*100
-        co = 100 - ua
-
-        # Producer Accuracy and Comission
-        total_cols = np.sum(MC, axis = 0)
-        pa = np.diag(MC)/np.sum(MC, axis = 0)*100
-        om = 100 - pa
-
-        total_cols = np.concatenate([total_cols, np.repeat(np.nan, 3)])
-        pa = np.concatenate([pa, np.repeat(np.nan, 3)])
-        om = np.concatenate([om, np.repeat(np.nan, 3)])
-
-        n = MC.shape[0]
-        cm = np.concatenate([MC, total_rows.reshape((n,1)), ua.reshape((n,1)), 
-                             co.reshape((n,1))], axis = 1)
-        cm = np.concatenate([cm, total_cols.reshape((1,n+3)), pa.reshape((1,n+3)), 
-                             om.reshape((1,n+3))])
-
-        min_class = np.nanmin(labels_dt)
-        max_class = np.nanmax(labels_dt)
-        
-        namesCol = []
-        for i in np.arange(min_class, max_class + 1):
-            stri = str(i)
-            namesCol.append(stri)
-
-        namesCol.extend(['Total', 'Users_Accuracy', 'Commission'])
-
-        namesRow = []
-        for i in np.arange(min_class, max_class + 1):
-            stri = str(i)
-            namesRow.append(stri)
-
-        namesRow.extend(['Total', 'Producer_Accuracy', 'Omission'])
-        namesRow
-
-        confusionMatrix = pd.DataFrame(cm, 
-                                        columns = namesCol, 
-                                        index = namesRow)
-
-        oa = accuracy_score(ytest, predic_Xtest)
-        kappa = cohen_kappa_score(ytest, predic_Xtest)
-        
-        output = {'Overall_Accuracy': oa,
-                  'Kappa_Index': kappa,
-                  'Confusion_Matrix': confusionMatrix,
-                  'Classification_Map': classDT,
-                  'Image': self.image
-                 } 
-    
-        return output
-    
-    def RF(self, training_split = 0.8, random_state = None, **kwargs):
-        
-        '''Random Forest is a derivative of Decision Tree which provides an improvement over DT to overcome the weaknesses of a single DT. 
-        The prediction model of the RF classifier only requires two parameters to be identified: the number of classification trees desired, 
-        known as “ntree,” and the number of prediction variables, known as “mtry,” used in each node to make the tree grow.
-        
-        RF support raster data read by rasterio (rasterio.io.DatasetReader) as input.
-        
-        
-        Parameters:
-    
-            training_split: For splitting samples into two subsets, i.e. training data and for testing
-                            data.
-                     
-            **kwargs: These will be passed to RF, please see full lists at:
-                  https://scikit-learn.org/stable/modules/generated/sklearn.ensemble.RandomForestClassifier.html
-    
-        Return:
-        
-            A dictionary containing labels of classification as numpy object, overall accuracy, kappa index, confusion matrix.
-        '''
-        
-        # removing the class column
-        X = self.endm.drop(self.endm.columns[[self.indx]], axis = 1)
-            
-        # only predictor variables
-        y = self.endm.iloc[:, self.indx]
-        
-        # split in training and testing
-        Xtrain, Xtest, ytrain, ytest = train_test_split(
-            X.values, 
-            y.values, 
-            train_size = training_split, 
-            test_size = 1 - training_split, 
-            random_state = random_state)
-        
-        # applying a support vector machine
-        inst_rf = RF(**kwargs)
-        
-        # model trained
-        mt_rf = inst_rf.fit(Xtrain, ytrain)
-        
-        labels_rf = mt_rf.predict(self.arr)
-        
-        # dealing with nan
-        if self.key_nan:
-            # image border like nan
-            labels_rf = labels_rf[self.posIndx]
-            self.class_final[self.posIndx] = labels_rf
-            classRF = self.class_final.reshape((self.rows, self.cols))
-        else:
-            classRF = labels_rf.reshape((self.rows, self.cols))
-        
-        # Confusion matrix
-        predic_Xtest = mt_rf.predict(Xtest)
-        
-        MC = confusion_matrix(ytest, predic_Xtest)
-    
-        MC = np.transpose(MC)
-
-        # Users Accuracy and Commission
-        total_rows = np.sum(MC, axis = 1)
-        ua = np.diag(MC)/np.sum(MC, axis = 1)*100
-        co = 100 - ua
-
-        # Producer Accuracy and Comission
-        total_cols = np.sum(MC, axis = 0)
-        pa = np.diag(MC)/np.sum(MC, axis = 0)*100
-        om = 100 - pa
-
-        total_cols = np.concatenate([total_cols, np.repeat(np.nan, 3)])
-        pa = np.concatenate([pa, np.repeat(np.nan, 3)])
-        om = np.concatenate([om, np.repeat(np.nan, 3)])
-
-        n = MC.shape[0]
-        cm = np.concatenate([MC, total_rows.reshape((n,1)), ua.reshape((n,1)), 
-                             co.reshape((n,1))], axis = 1)
-        cm = np.concatenate([cm, total_cols.reshape((1,n+3)), pa.reshape((1,n+3)), 
-                             om.reshape((1,n+3))])
-
-        min_class = np.nanmin(labels_rf)
-        max_class = np.nanmax(labels_rf)
-        
-        namesCol = []
-        for i in np.arange(min_class, max_class + 1):
-            stri = str(i)
-            namesCol.append(stri)
-
-        namesCol.extend(['Total', 'Users_Accuracy', 'Commission'])
-
-        namesRow = []
-        for i in np.arange(min_class, max_class + 1):
-            stri = str(i)
-            namesRow.append(stri)
-
-        namesRow.extend(['Total', 'Producer_Accuracy', 'Omission'])
-        namesRow
-
-        confusionMatrix = pd.DataFrame(cm, 
-                                        columns = namesCol, 
-                                        index = namesRow)
-
-        oa = accuracy_score(ytest, predic_Xtest)
-        kappa = cohen_kappa_score(ytest, predic_Xtest)
-        
-        output = {'Overall_Accuracy': oa,
-                  'Kappa_Index': kappa,
-                  'Confusion_Matrix': confusionMatrix,
-                  'Classification_Map': classRF,
-                  'Image': self.image
-                 } 
-    
-        return output
-    
-    def NB(self, training_split = 0.8, random_state = None, **kwargs):
-        
-        '''Naive Bayes classifier is an effective and simple method for image classification based on probability theory. The NB 
-        classifier assumes an underlying probabilistic model and captures the uncertainty about the model in a principled way, 
-        that is, by calculating the occurrence probabilities of different attribute values for different classes in a training 
-        set.
-        
-        NB support raster data read by rasterio (rasterio.io.DatasetReader) as input.
-        
-        
-        Parameters:
-    
-            training_split: For splitting samples into two subsets, i.e. training data and for testing
-                            data.
-                     
-            **kwargs: These will be passed to SVM, please see full lists at:
-                  https://scikit-learn.org/stable/modules/generated/sklearn.naive_bayes.GaussianNB.html
-    
-        Return:
-        
-            A dictionary containing labels of classification as numpy object, overall accuracy, kappa index, confusion matrix.
-        '''
-        
-        # removing the class column
-        X = self.endm.drop(self.endm.columns[[self.indx]], axis = 1)
-            
-        # only predictor variables
-        y = self.endm.iloc[:, self.indx]
-        
-        # split in training and testing
-        Xtrain, Xtest, ytrain, ytest = train_test_split(
-            X.values, 
-            y.values, 
-            train_size = training_split, 
-            test_size = 1 - training_split, 
-            random_state = random_state)
-        
-        # applying a support vector machine
-        inst_nb = GNB(**kwargs)
-        
-        # model trained
-        mt_nb = inst_nb.fit(Xtrain, ytrain)
-        
-        labels_nb = mt_nb.predict(self.arr)
-        
-        # dealing with nan
-        if self.key_nan:
-            # image border like nan
-            labels_nb = labels_nb[self.posIndx]
-            self.class_final[self.posIndx] = labels_nb
-            classNB = self.class_final.reshape((self.rows, self.cols))
-        else:
-            classNB = labels_nb.reshape((self.rows, self.cols))
-        
-        # Confusion matrix
-        predic_Xtest = mt_nb.predict(Xtest)
-        
-        MC = confusion_matrix(ytest, predic_Xtest)
-    
-        MC = np.transpose(MC)
-
-        # Users Accuracy and Commission
-        total_rows = np.sum(MC, axis = 1)
-        ua = np.diag(MC)/np.sum(MC, axis = 1)*100
-        co = 100 - ua
-
-        # Producer Accuracy and Comission
-        total_cols = np.sum(MC, axis = 0)
-        pa = np.diag(MC)/np.sum(MC, axis = 0)*100
-        om = 100 - pa
-
-        total_cols = np.concatenate([total_cols, np.repeat(np.nan, 3)])
-        pa = np.concatenate([pa, np.repeat(np.nan, 3)])
-        om = np.concatenate([om, np.repeat(np.nan, 3)])
-
-        n = MC.shape[0]
-        cm = np.concatenate([MC, total_rows.reshape((n,1)), ua.reshape((n,1)), 
-                             co.reshape((n,1))], axis = 1)
-        cm = np.concatenate([cm, total_cols.reshape((1,n+3)), pa.reshape((1,n+3)), 
-                             om.reshape((1,n+3))])
-
-        min_class = np.nanmin(labels_nb)
-        max_class = np.nanmax(labels_nb)
-        
-        namesCol = []
-        for i in np.arange(min_class, max_class + 1):
-            stri = str(i)
-            namesCol.append(stri)
-
-        namesCol.extend(['Total', 'Users_Accuracy', 'Commission'])
-
-        namesRow = []
-        for i in np.arange(min_class, max_class + 1):
-            stri = str(i)
-            namesRow.append(stri)
-
-        namesRow.extend(['Total', 'Producer_Accuracy', 'Omission'])
-        namesRow
-
-        confusionMatrix = pd.DataFrame(cm, 
-                                        columns = namesCol, 
-                                        index = namesRow)
-
-        oa = accuracy_score(ytest, predic_Xtest)
-        kappa = cohen_kappa_score(ytest, predic_Xtest)
-        
-        output = {'Overall_Accuracy': oa,
-                  'Kappa_Index': kappa,
-                  'Confusion_Matrix': confusionMatrix,
-                  'Classification_Map': classNB,
-                  'Image': self.image
-                 } 
-    
-        return output
-    
-    def NN(self, training_split = 0.8, max_iter = 300, random_state = None, **kwargs):
-        
-        '''This classification consists of a neural network that is organized into several layers, that is, an input layer of predictor 
-        variables, one or more layers of hidden nodes, in which each node represents an activation function acting on a weighted input 
-        of the previous layers’ outputs, and an output layer.
-        
-        NN support raster data read by rasterio (rasterio.io.DatasetReader) as input.
-        
-        
-        Parameters:
-    
-            training_split: For splitting samples into two subsets, i.e. training data and for testing
-                            data.
-                     
-            **kwargs: These will be passed to SVM, please see full lists at:
-                  https://scikit-learn.org/stable/modules/generated/sklearn.neural_network.MLPClassifier.html
-    
-        Return:
-        
-            A dictionary containing labels of classification as numpy object, overall accuracy, kappa index, confusion matrix.
-        '''
-        
-        # removing the class column
-        X = self.endm.drop(self.endm.columns[[self.indx]], axis = 1)
-            
-        # only predictor variables
-        y = self.endm.iloc[:, self.indx]
-        
-        # split in training and testing
-        Xtrain, Xtest, ytrain, ytest = train_test_split(
-            X.values, 
-            y.values, 
-            train_size = training_split, 
-            test_size = 1 - training_split, 
-            random_state = random_state)
-        
-        # applying neural network
-        inst_nn = MLP(max_iter = max_iter, **kwargs)
-        
-        # model trained
-        mt_nn = inst_nn.fit(Xtrain, ytrain)
-        
-        labels_nn = mt_nn.predict(self.arr)
-        
-        # dealing with nan
-        if self.key_nan:
-            # image border like nan
-            labels_nn = labels_nn[self.posIndx]
-            self.class_final[self.posIndx] = labels_nn
-            classNN = self.class_final.reshape((self.rows, self.cols))
-        else:
-            classNN = labels_nn.reshape((self.rows, self.cols))
-        
-        # Confusion matrix
-        predic_Xtest = mt_nn.predict(Xtest)
-        
-        MC = confusion_matrix(ytest, predic_Xtest)
-    
-        MC = np.transpose(MC)
-
-        # Users Accuracy and Commission
-        total_rows = np.sum(MC, axis = 1)
-        ua = np.diag(MC)/np.sum(MC, axis = 1)*100
-        co = 100 - ua
-
-        # Producer Accuracy and Comission
-        total_cols = np.sum(MC, axis = 0)
-        pa = np.diag(MC)/np.sum(MC, axis = 0)*100
-        om = 100 - pa
-
-        total_cols = np.concatenate([total_cols, np.repeat(np.nan, 3)])
-        pa = np.concatenate([pa, np.repeat(np.nan, 3)])
-        om = np.concatenate([om, np.repeat(np.nan, 3)])
-
-        n = MC.shape[0]
-        cm = np.concatenate([MC, total_rows.reshape((n,1)), ua.reshape((n,1)), 
-                             co.reshape((n,1))], axis = 1)
-        cm = np.concatenate([cm, total_cols.reshape((1,n+3)), pa.reshape((1,n+3)), 
-                             om.reshape((1,n+3))])
-
-        min_class = np.nanmin(labels_nn)
-        max_class = np.nanmax(labels_nn)
-        
-        namesCol = []
-        for i in np.arange(min_class, max_class + 1):
-            stri = str(i)
-            namesCol.append(stri)
-
-        namesCol.extend(['Total', 'Users_Accuracy', 'Commission'])
-
-        namesRow = []
-        for i in np.arange(min_class, max_class + 1):
-            stri = str(i)
-            namesRow.append(stri)
-
-        namesRow.extend(['Total', 'Producer_Accuracy', 'Omission'])
-        namesRow
-
-        confusionMatrix = pd.DataFrame(cm, 
-                                        columns = namesCol, 
-                                        index = namesRow)
-
-        oa = accuracy_score(ytest, predic_Xtest)
-        kappa = cohen_kappa_score(ytest, predic_Xtest)
-        
-        output = {'Overall_Accuracy': oa,
-                  'Kappa_Index': kappa,
-                  'Confusion_Matrix': confusionMatrix,
-                  'Classification_Map': classNN,
-                  'Image': self.image
-                 } 
-    
-        return output
+# -*- coding: utf-8 -*-
+# +
+import copy
+import rasterio
+import numpy as np
+import pandas as pd
+from dbfread import DBF
+from sklearn.svm import SVC
+from sklearn.tree import DecisionTreeClassifier as DT
+from sklearn.ensemble import RandomForestClassifier as RF
+from sklearn.naive_bayes import GaussianNB as GNB
+from sklearn.neural_network import MLPClassifier as MLP
+from sklearn.model_selection import train_test_split
+from sklearn.metrics import accuracy_score
+from sklearn.metrics import cohen_kappa_score
+from sklearn.metrics import confusion_matrix
+import warnings
+
+class MLA(object):
+    
+    'Supervised classification in Remote Sensing'
+    
+    def __init__(self, image, endmembers, nodata = -99999):
+        
+        '''
+        Parameter:
+        
+            image: Optical images. It must be rasterio.io.DatasetReader with 3d.
+            
+            endmembers: Endmembers must be a matrix (numpy.ndarray) and with more than one endmember. 
+                    Rows represent the endmembers and columns represent the spectral bands.
+                    The number of bands must be equal to the number of endmembers.
+                    E.g. an image with 6 bands, endmembers dimension should be $n*6$, where $n$ 
+                    is rows with the number of endmembers and 6 is the number of bands 
+                    (should be equal).
+                    In addition, Endmembers must have a field (type int or float) with the names 
+                    of classes to be predicted.
+            
+            nodata: The NoData value to replace with -99999.
+            
+        '''
+        
+        self.image = image
+        self.endm = endmembers
+        self.nodata = nodata
+        
+        if not isinstance(self.image, (rasterio.io.DatasetReader)):
+            raise TypeError('"image" must be raster read by rasterio.open().')
+        
+        bands = self.image.count
+        
+        rows = self.image.height
+        
+        cols = self.image.width
+        
+        st = image.read()
+        
+        # data in [rows, cols, bands]
+        st_reorder = np.moveaxis(st, 0, -1) 
+        # data in [rows*cols, bands]
+        arr = st_reorder.reshape((rows*cols, bands))
+        
+        # nodata
+        #if np.isnan(np.sum(arr)):
+            #arr[np.isnan(arr)] = self.nodata
+        
+        # dealing with nan
+        key_nan = np.isnan(np.sum(arr[:,0]))
+        
+        if key_nan:
+            # saving un array for predicted classes
+            class_final = arr[:, 0].copy()
+            # positions with nan
+            posIndx = np.argwhere(~np.isnan(class_final)).flatten()
+            # replace np.nan -> 0
+            arr[np.isnan(arr)] = 0
+        
+        # if it is read by pandas.read_csv()
+        if isinstance(self.endm, (pd.core.frame.DataFrame)):
+            
+            for i in np.arange(self.endm.shape[1]):
+                
+                if all(self.endm.iloc[:,int(i)] < 100) & all(self.endm.iloc[:,int(i)] >= 0): indx = i; break
+        
+        # if the file is .dbf    
+        elif isinstance(self.endm, (DBF)): # isinstance() function With Inheritance
+            
+            self.endm = pd.DataFrame(iter(self.endm))
+            
+            for i in np.arange(self.endm.shape[1]):
+                
+                if all(self.endm.iloc[:,int(i)] < 100) & all(self.endm.iloc[:,int(i)] >= 0): indx = i; break
+        
+        else:
+            raise TypeError('"endm" must be .csv (pandas.core.frame.DataFrame).')
+
+        if not self.endm.shape[1] == (bands + 1):
+            raise ValueError('The number of columns of signatures (included the class column) must'
+                             'be equal to the number of bands + 1.')
+        
+        self.indx = indx
+        
+        self.arr = arr
+        
+        self.rows = rows
+        
+        self.cols = cols
+        
+        if key_nan:
+            self.key_nan = key_nan
+            self.posIndx = posIndx
+            self.class_final = class_final
+        else:
+            self.key_nan = key_nan
+            
+        
+    def SVM(self, training_split = 0.8, random_state = None, kernel = 'linear', **kwargs):
+        
+        '''The Support Vector Machine (SVM) classifier is a supervised non-parametric statistical learning technique that 
+        does not assume a preliminary distribution of input data. Its discrimination criterion is a 
+        hyperplane that separates the classes in the multidimensional space in which the samples 
+        that have established the same classes are located, generally some training areas.
+        
+        SVM support raster data read by rasterio (rasterio.io.DatasetReader) as input.
+     
+        
+        Parameters:
+    
+            training_split: For splitting samples into two subsets, i.e. training data and for testing
+                            data.
+    
+            kernel : {'linear', 'poly', 'rbf', 'sigmoid', 'precomputed'}, default='rbf' Specifies 
+                     the kernel type to be used in the algorithm. It must be one of 'linear', 'poly', 
+                     'rbf', 'sigmoid', 'precomputed' or a callable. If None is given, 'rbf' will 
+                     be used. See https://scikit-learn.org/stable/modules/generated/sklearn.svm.SVC.html#sklearn.svm.SVC
+                     for more details.
+                     
+            **kwargs: These will be passed to SVM, please see full lists at:
+                  https://scikit-learn.org/stable/modules/generated/sklearn.svm.SVC.html#sklearn.svm.SVC
+    
+        Return:
+        
+            A dictionary containing labels of classification as numpy object, overall accuracy, kappa index, confusion matrix.
+        '''
+        
+        # removing the class column
+        X = self.endm.drop(self.endm.columns[[self.indx]], axis = 1)
+        
+        # only predictor variables
+        y = self.endm.iloc[:, self.indx]
+        
+        # split in training and testing
+        Xtrain, Xtest, ytrain, ytest = train_test_split(
+            X.values, 
+            y.values, 
+            train_size = training_split, 
+            test_size = 1 - training_split, 
+            random_state = random_state)
+        
+        # applying a support vector machine
+        inst_svm = SVC(kernel = kernel, **kwargs)
+        
+        # model trained
+        mt_svm = inst_svm.fit(Xtrain, ytrain)
+        
+        labels_svm = mt_svm.predict(self.arr)
+        
+        # dealing with nan
+        if self.key_nan:
+            # image border like nan
+            labels_svm = labels_svm[self.posIndx]
+            self.class_final[self.posIndx] = labels_svm
+            classSVM = self.class_final.reshape((self.rows, self.cols))
+        else:
+            classSVM = labels_svm.reshape((self.rows, self.cols))
+        
+        # Confusion matrix
+        predic_Xtest = mt_svm.predict(Xtest)
+        
+        MC = confusion_matrix(ytest, predic_Xtest)
+    
+        MC = np.transpose(MC)
+
+        # Users Accuracy and Commission
+        total_rows = np.sum(MC, axis = 1)
+        ua = np.diag(MC)/np.sum(MC, axis = 1)*100
+        co = 100 - ua
+
+        # Producer Accuracy and Comission
+        total_cols = np.sum(MC, axis = 0)
+        pa = np.diag(MC)/np.sum(MC, axis = 0)*100
+        om = 100 - pa
+
+        total_cols = np.concatenate([total_cols, np.repeat(np.nan, 3)])
+        pa = np.concatenate([pa, np.repeat(np.nan, 3)])
+        om = np.concatenate([om, np.repeat(np.nan, 3)])
+
+        n = MC.shape[0]
+        cm = np.concatenate([MC, total_rows.reshape((n,1)), ua.reshape((n,1)), 
+                             co.reshape((n,1))], axis = 1)
+        cm = np.concatenate([cm, total_cols.reshape((1,n+3)), pa.reshape((1,n+3)), 
+                             om.reshape((1,n+3))])
+
+        min_class = np.nanmin(labels_svm)
+        max_class = np.nanmax(labels_svm)
+        
+        namesCol = []
+        for i in np.arange(min_class, max_class + 1):
+            stri = str(i)
+            namesCol.append(stri)
+
+        namesCol.extend(['Total', 'Users_Accuracy', 'Commission'])
+
+        namesRow = []
+        for i in np.arange(min_class, max_class + 1):
+            stri = str(i)
+            namesRow.append(stri)
+
+        namesRow.extend(['Total', 'Producer_Accuracy', 'Omission'])
+        namesRow
+
+        confusionMatrix = pd.DataFrame(cm, 
+                                        columns = namesCol, 
+                                        index = namesRow)
+
+        oa = accuracy_score(ytest, predic_Xtest)
+        kappa = cohen_kappa_score(ytest, predic_Xtest)
+        
+        output = {'Overall_Accuracy': oa,
+                  'Kappa_Index': kappa,
+                  'Confusion_Matrix': confusionMatrix,
+                  'Classification_Map': classSVM,
+                  'Image': self.image
+                 } 
+    
+        return output
+    
+    def DT(self, training_split = 0.8, random_state = None, **kwargs):
+        
+        '''Decision Tree is also a supervised non-parametric statistical learning technique, where the input data is divided recursively 
+        into branches depending on certain decision thresholds until the data are segmented into homogeneous subgroups. 
+        This technique has substantial advantages for remote sensing classification problems due to its flexibility, intuitive simplicity, 
+        and computational efficiency.
+        
+        DT support raster data read by rasterio (rasterio.io.DatasetReader) as input.
+        
+        
+        Parameters:
+    
+            training_split: For splitting samples into two subsets, i.e. training data and for testing
+                            data.
+                     
+            **kwargs: These will be passed to DT, please see full lists at:
+                  https://scikit-learn.org/stable/modules/generated/sklearn.tree.DecisionTreeClassifier.html#sklearn.tree.DecisionTreeClassifier
+    
+        Return:
+        
+            A dictionary containing labels of classification as numpy object, overall accuracy, kappa index, confusion matrix.
+        '''
+        
+        # removing the class column
+        X = self.endm.drop(self.endm.columns[[self.indx]], axis = 1)
+            
+        # only predictor variables
+        y = self.endm.iloc[:, self.indx]
+        
+        # split in training and testing
+        Xtrain, Xtest, ytrain, ytest = train_test_split(
+            X.values, 
+            y.values, 
+            train_size = training_split, 
+            test_size = 1 - training_split, 
+            random_state = random_state)
+        
+        # applying a support vector machine
+        inst_dt = DT(**kwargs)
+        
+        # model trained
+        mt_dt = inst_dt.fit(Xtrain, ytrain)
+        
+        labels_dt = mt_dt.predict(self.arr)
+        
+        # dealing with nan
+        if self.key_nan:
+            # image border like nan
+            labels_dt = labels_dt[self.posIndx]
+            self.class_final[self.posIndx] = labels_dt
+            classDT = self.class_final.reshape((self.rows, self.cols))
+        else:
+            classDT = labels_dt.reshape((self.rows, self.cols))
+        
+        # Confusion matrix
+        predic_Xtest = mt_dt.predict(Xtest)
+        
+        MC = confusion_matrix(ytest, predic_Xtest)
+    
+        MC = np.transpose(MC)
+
+        # Users Accuracy and Commission
+        total_rows = np.sum(MC, axis = 1)
+        ua = np.diag(MC)/np.sum(MC, axis = 1)*100
+        co = 100 - ua
+
+        # Producer Accuracy and Comission
+        total_cols = np.sum(MC, axis = 0)
+        pa = np.diag(MC)/np.sum(MC, axis = 0)*100
+        om = 100 - pa
+
+        total_cols = np.concatenate([total_cols, np.repeat(np.nan, 3)])
+        pa = np.concatenate([pa, np.repeat(np.nan, 3)])
+        om = np.concatenate([om, np.repeat(np.nan, 3)])
+
+        n = MC.shape[0]
+        cm = np.concatenate([MC, total_rows.reshape((n,1)), ua.reshape((n,1)), 
+                             co.reshape((n,1))], axis = 1)
+        cm = np.concatenate([cm, total_cols.reshape((1,n+3)), pa.reshape((1,n+3)), 
+                             om.reshape((1,n+3))])
+
+        min_class = np.nanmin(labels_dt)
+        max_class = np.nanmax(labels_dt)
+        
+        namesCol = []
+        for i in np.arange(min_class, max_class + 1):
+            stri = str(i)
+            namesCol.append(stri)
+
+        namesCol.extend(['Total', 'Users_Accuracy', 'Commission'])
+
+        namesRow = []
+        for i in np.arange(min_class, max_class + 1):
+            stri = str(i)
+            namesRow.append(stri)
+
+        namesRow.extend(['Total', 'Producer_Accuracy', 'Omission'])
+        namesRow
+
+        confusionMatrix = pd.DataFrame(cm, 
+                                        columns = namesCol, 
+                                        index = namesRow)
+
+        oa = accuracy_score(ytest, predic_Xtest)
+        kappa = cohen_kappa_score(ytest, predic_Xtest)
+        
+        output = {'Overall_Accuracy': oa,
+                  'Kappa_Index': kappa,
+                  'Confusion_Matrix': confusionMatrix,
+                  'Classification_Map': classDT,
+                  'Image': self.image
+                 } 
+    
+        return output
+    
+    def RF(self, training_split = 0.8, random_state = None, **kwargs):
+        
+        '''Random Forest is a derivative of Decision Tree which provides an improvement over DT to overcome the weaknesses of a single DT. 
+        The prediction model of the RF classifier only requires two parameters to be identified: the number of classification trees desired, 
+        known as “ntree,” and the number of prediction variables, known as “mtry,” used in each node to make the tree grow.
+        
+        RF support raster data read by rasterio (rasterio.io.DatasetReader) as input.
+        
+        
+        Parameters:
+    
+            training_split: For splitting samples into two subsets, i.e. training data and for testing
+                            data.
+                     
+            **kwargs: These will be passed to RF, please see full lists at:
+                  https://scikit-learn.org/stable/modules/generated/sklearn.ensemble.RandomForestClassifier.html
+    
+        Return:
+        
+            A dictionary containing labels of classification as numpy object, overall accuracy, kappa index, confusion matrix.
+        '''
+        
+        # removing the class column
+        X = self.endm.drop(self.endm.columns[[self.indx]], axis = 1)
+            
+        # only predictor variables
+        y = self.endm.iloc[:, self.indx]
+        
+        # split in training and testing
+        Xtrain, Xtest, ytrain, ytest = train_test_split(
+            X.values, 
+            y.values, 
+            train_size = training_split, 
+            test_size = 1 - training_split, 
+            random_state = random_state)
+        
+        # applying a support vector machine
+        inst_rf = RF(**kwargs)
+        
+        # model trained
+        mt_rf = inst_rf.fit(Xtrain, ytrain)
+        
+        labels_rf = mt_rf.predict(self.arr)
+        
+        # dealing with nan
+        if self.key_nan:
+            # image border like nan
+            labels_rf = labels_rf[self.posIndx]
+            self.class_final[self.posIndx] = labels_rf
+            classRF = self.class_final.reshape((self.rows, self.cols))
+        else:
+            classRF = labels_rf.reshape((self.rows, self.cols))
+        
+        # Confusion matrix
+        predic_Xtest = mt_rf.predict(Xtest)
+        
+        MC = confusion_matrix(ytest, predic_Xtest)
+    
+        MC = np.transpose(MC)
+
+        # Users Accuracy and Commission
+        total_rows = np.sum(MC, axis = 1)
+        ua = np.diag(MC)/np.sum(MC, axis = 1)*100
+        co = 100 - ua
+
+        # Producer Accuracy and Comission
+        total_cols = np.sum(MC, axis = 0)
+        pa = np.diag(MC)/np.sum(MC, axis = 0)*100
+        om = 100 - pa
+
+        total_cols = np.concatenate([total_cols, np.repeat(np.nan, 3)])
+        pa = np.concatenate([pa, np.repeat(np.nan, 3)])
+        om = np.concatenate([om, np.repeat(np.nan, 3)])
+
+        n = MC.shape[0]
+        cm = np.concatenate([MC, total_rows.reshape((n,1)), ua.reshape((n,1)), 
+                             co.reshape((n,1))], axis = 1)
+        cm = np.concatenate([cm, total_cols.reshape((1,n+3)), pa.reshape((1,n+3)), 
+                             om.reshape((1,n+3))])
+
+        min_class = np.nanmin(labels_rf)
+        max_class = np.nanmax(labels_rf)
+        
+        namesCol = []
+        for i in np.arange(min_class, max_class + 1):
+            stri = str(i)
+            namesCol.append(stri)
+
+        namesCol.extend(['Total', 'Users_Accuracy', 'Commission'])
+
+        namesRow = []
+        for i in np.arange(min_class, max_class + 1):
+            stri = str(i)
+            namesRow.append(stri)
+
+        namesRow.extend(['Total', 'Producer_Accuracy', 'Omission'])
+        namesRow
+
+        confusionMatrix = pd.DataFrame(cm, 
+                                        columns = namesCol, 
+                                        index = namesRow)
+
+        oa = accuracy_score(ytest, predic_Xtest)
+        kappa = cohen_kappa_score(ytest, predic_Xtest)
+        
+        output = {'Overall_Accuracy': oa,
+                  'Kappa_Index': kappa,
+                  'Confusion_Matrix': confusionMatrix,
+                  'Classification_Map': classRF,
+                  'Image': self.image
+                 } 
+    
+        return output
+    
+    def NB(self, training_split = 0.8, random_state = None, **kwargs):
+        
+        '''Naive Bayes classifier is an effective and simple method for image classification based on probability theory. The NB 
+        classifier assumes an underlying probabilistic model and captures the uncertainty about the model in a principled way, 
+        that is, by calculating the occurrence probabilities of different attribute values for different classes in a training 
+        set.
+        
+        NB support raster data read by rasterio (rasterio.io.DatasetReader) as input.
+        
+        
+        Parameters:
+    
+            training_split: For splitting samples into two subsets, i.e. training data and for testing
+                            data.
+                     
+            **kwargs: These will be passed to SVM, please see full lists at:
+                  https://scikit-learn.org/stable/modules/generated/sklearn.naive_bayes.GaussianNB.html
+    
+        Return:
+        
+            A dictionary containing labels of classification as numpy object, overall accuracy, kappa index, confusion matrix.
+        '''
+        
+        # removing the class column
+        X = self.endm.drop(self.endm.columns[[self.indx]], axis = 1)
+            
+        # only predictor variables
+        y = self.endm.iloc[:, self.indx]
+        
+        # split in training and testing
+        Xtrain, Xtest, ytrain, ytest = train_test_split(
+            X.values, 
+            y.values, 
+            train_size = training_split, 
+            test_size = 1 - training_split, 
+            random_state = random_state)
+        
+        # applying a support vector machine
+        inst_nb = GNB(**kwargs)
+        
+        # model trained
+        mt_nb = inst_nb.fit(Xtrain, ytrain)
+        
+        labels_nb = mt_nb.predict(self.arr)
+        
+        # dealing with nan
+        if self.key_nan:
+            # image border like nan
+            labels_nb = labels_nb[self.posIndx]
+            self.class_final[self.posIndx] = labels_nb
+            classNB = self.class_final.reshape((self.rows, self.cols))
+        else:
+            classNB = labels_nb.reshape((self.rows, self.cols))
+        
+        # Confusion matrix
+        predic_Xtest = mt_nb.predict(Xtest)
+        
+        MC = confusion_matrix(ytest, predic_Xtest)
+    
+        MC = np.transpose(MC)
+
+        # Users Accuracy and Commission
+        total_rows = np.sum(MC, axis = 1)
+        ua = np.diag(MC)/np.sum(MC, axis = 1)*100
+        co = 100 - ua
+
+        # Producer Accuracy and Comission
+        total_cols = np.sum(MC, axis = 0)
+        pa = np.diag(MC)/np.sum(MC, axis = 0)*100
+        om = 100 - pa
+
+        total_cols = np.concatenate([total_cols, np.repeat(np.nan, 3)])
+        pa = np.concatenate([pa, np.repeat(np.nan, 3)])
+        om = np.concatenate([om, np.repeat(np.nan, 3)])
+
+        n = MC.shape[0]
+        cm = np.concatenate([MC, total_rows.reshape((n,1)), ua.reshape((n,1)), 
+                             co.reshape((n,1))], axis = 1)
+        cm = np.concatenate([cm, total_cols.reshape((1,n+3)), pa.reshape((1,n+3)), 
+                             om.reshape((1,n+3))])
+
+        min_class = np.nanmin(labels_nb)
+        max_class = np.nanmax(labels_nb)
+        
+        namesCol = []
+        for i in np.arange(min_class, max_class + 1):
+            stri = str(i)
+            namesCol.append(stri)
+
+        namesCol.extend(['Total', 'Users_Accuracy', 'Commission'])
+
+        namesRow = []
+        for i in np.arange(min_class, max_class + 1):
+            stri = str(i)
+            namesRow.append(stri)
+
+        namesRow.extend(['Total', 'Producer_Accuracy', 'Omission'])
+        namesRow
+
+        confusionMatrix = pd.DataFrame(cm, 
+                                        columns = namesCol, 
+                                        index = namesRow)
+
+        oa = accuracy_score(ytest, predic_Xtest)
+        kappa = cohen_kappa_score(ytest, predic_Xtest)
+        
+        output = {'Overall_Accuracy': oa,
+                  'Kappa_Index': kappa,
+                  'Confusion_Matrix': confusionMatrix,
+                  'Classification_Map': classNB,
+                  'Image': self.image
+                 } 
+    
+        return output
+    
+    def NN(self, training_split = 0.8, max_iter = 300, random_state = None, **kwargs):
+        
+        '''This classification consists of a neural network that is organized into several layers, that is, an input layer of predictor 
+        variables, one or more layers of hidden nodes, in which each node represents an activation function acting on a weighted input 
+        of the previous layers’ outputs, and an output layer.
+        
+        NN support raster data read by rasterio (rasterio.io.DatasetReader) as input.
+        
+        
+        Parameters:
+    
+            training_split: For splitting samples into two subsets, i.e. training data and for testing
+                            data.
+                     
+            **kwargs: These will be passed to SVM, please see full lists at:
+                  https://scikit-learn.org/stable/modules/generated/sklearn.neural_network.MLPClassifier.html
+    
+        Return:
+        
+            A dictionary containing labels of classification as numpy object, overall accuracy, kappa index, confusion matrix.
+        '''
+        
+        # removing the class column
+        X = self.endm.drop(self.endm.columns[[self.indx]], axis = 1)
+            
+        # only predictor variables
+        y = self.endm.iloc[:, self.indx]
+        
+        # split in training and testing
+        Xtrain, Xtest, ytrain, ytest = train_test_split(
+            X.values, 
+            y.values, 
+            train_size = training_split, 
+            test_size = 1 - training_split, 
+            random_state = random_state)
+        
+        # applying neural network
+        inst_nn = MLP(max_iter = max_iter, **kwargs)
+        
+        # model trained
+        mt_nn = inst_nn.fit(Xtrain, ytrain)
+        
+        labels_nn = mt_nn.predict(self.arr)
+        
+        # dealing with nan
+        if self.key_nan:
+            # image border like nan
+            labels_nn = labels_nn[self.posIndx]
+            self.class_final[self.posIndx] = labels_nn
+            classNN = self.class_final.reshape((self.rows, self.cols))
+        else:
+            classNN = labels_nn.reshape((self.rows, self.cols))
+        
+        # Confusion matrix
+        predic_Xtest = mt_nn.predict(Xtest)
+        
+        MC = confusion_matrix(ytest, predic_Xtest)
+    
+        MC = np.transpose(MC)
+
+        # Users Accuracy and Commission
+        total_rows = np.sum(MC, axis = 1)
+        ua = np.diag(MC)/np.sum(MC, axis = 1)*100
+        co = 100 - ua
+
+        # Producer Accuracy and Comission
+        total_cols = np.sum(MC, axis = 0)
+        pa = np.diag(MC)/np.sum(MC, axis = 0)*100
+        om = 100 - pa
+
+        total_cols = np.concatenate([total_cols, np.repeat(np.nan, 3)])
+        pa = np.concatenate([pa, np.repeat(np.nan, 3)])
+        om = np.concatenate([om, np.repeat(np.nan, 3)])
+
+        n = MC.shape[0]
+        cm = np.concatenate([MC, total_rows.reshape((n,1)), ua.reshape((n,1)), 
+                             co.reshape((n,1))], axis = 1)
+        cm = np.concatenate([cm, total_cols.reshape((1,n+3)), pa.reshape((1,n+3)), 
+                             om.reshape((1,n+3))])
+
+        min_class = np.nanmin(labels_nn)
+        max_class = np.nanmax(labels_nn)
+        
+        namesCol = []
+        for i in np.arange(min_class, max_class + 1):
+            stri = str(i)
+            namesCol.append(stri)
+
+        namesCol.extend(['Total', 'Users_Accuracy', 'Commission'])
+
+        namesRow = []
+        for i in np.arange(min_class, max_class + 1):
+            stri = str(i)
+            namesRow.append(stri)
+
+        namesRow.extend(['Total', 'Producer_Accuracy', 'Omission'])
+        namesRow
+
+        confusionMatrix = pd.DataFrame(cm, 
+                                        columns = namesCol, 
+                                        index = namesRow)
+
+        oa = accuracy_score(ytest, predic_Xtest)
+        kappa = cohen_kappa_score(ytest, predic_Xtest)
+        
+        output = {'Overall_Accuracy': oa,
+                  'Kappa_Index': kappa,
+                  'Confusion_Matrix': confusionMatrix,
+                  'Classification_Map': classNN,
+                  'Image': self.image
+                 } 
+    
+        return output
```

### Comparing `scikeo-0.2.12/scikeo/pca.py` & `scikeo-0.2.13/scikeo/pca.py`

 * *Files identical despite different names*

### Comparing `scikeo-0.2.12/scikeo/plot.py` & `scikeo-0.2.13/scikeo/plot.py`

 * *Files identical despite different names*

### Comparing `scikeo-0.2.12/scikeo/process.py` & `scikeo-0.2.13/scikeo/process.py`

 * *Ordering differences only*

 * *Files 18% similar despite different names*

```diff
@@ -1,304 +1,304 @@
-# -*- coding: utf-8 -*-
-# +
-import os
-import copy
-import fiona
-import rasterio
-import rasterio.mask
-import numpy as np
-import pandas as pd
-import geopandas as gpd
-
-def crop(image, shp, filename = None, filepath = None):
-    
-    '''
-    This algorithm allows to clip a raster (.tif) including a satellite image using a shapefile.
-    
-    Parameters:
-        
-        image: This parameter can be a string with the raster path (e.g., r'/home/image/b3.tif') or
-        it can be a rasterio.io.DatasetReader type.
-        
-        shp: Vector file, tipically shapefile.
-        
-        filename: The image name to be saved.
-        
-        filepath: The path which the image will be stored.
-        
-    Return:
-    
-        A raster in your filepath.
-    '''
-        
-    if isinstance(image, (str)):
-        
-        image = image.replace(os.sep, '/')
-    
-        shp = shp.replace(os.sep, '/')
-        
-        if filename is None:
-        
-            filename = 'raster'
-    
-        if filepath is None:
-        
-            current_path = os.getcwd()
-        
-            path = current_path.replace(os.sep, '/') + '/' + filename + '.tif'
-        
-        else:
-            path = filepath.replace(os.sep, '/') + '/' + filename + '.tif'
-    
-        path_name = path
-    
-        # read Shapefile
-        with fiona.open(shp, "r") as shapefile:
-            shapes = [feature["geometry"] for feature in shapefile]
-
-        # read image
-        with rasterio.open(image) as src:
-            out_image, out_transform = rasterio.mask.mask(src, shapes, crop = True)
-            out_meta = src.meta
-
-        # save clipped image
-        out_meta.update({"driver": "GTiff",
-                         "height": out_image.shape[1],
-                         "width": out_image.shape[2],
-                         "transform": out_transform})
-
-        with rasterio.open(path_name, "w", **out_meta) as dest:
-            dest.write(out_image)
-    
-    elif isinstance(image, (rasterio.io.DatasetReader)):
-    
-        shp = shp.replace(os.sep, '/')
-        
-        if filename is None:
-        
-            filename = 'raster'
-    
-        if filepath is None:
-        
-            current_path = os.getcwd()
-        
-            path = current_path.replace(os.sep, '/') + '/' + filename + '.tif'
-        
-        else:
-            path = filepath.replace(os.sep, '/') + '/' + filename + '.tif'
-    
-        path_name = path
-    
-        # read Shape file
-        with fiona.open(shp, "r") as shapefile:
-            shapes = [feature["geometry"] for feature in shapefile]
-
-        # read image
-        out_image, out_transform = rasterio.mask.mask(image, shapes, crop = True)
-        out_meta = image.meta
-
-        # save clipped image
-        out_meta.update({"driver": "GTiff",
-                         "height": out_image.shape[1],
-                         "width": out_image.shape[2],
-                         "transform": out_transform})
-
-        with rasterio.open(path_name, "w", **out_meta) as dest:
-            dest.write(out_image)
-        
-    else:
-        raise TypeError(f'"image" must be a string like r"/home/image/b5.tif" or must be rasterio.io.DatasetReader. image = {type(image)}')
-
-        
-def extract(image, shp):
-    
-    '''
-    This algorithm allows to extract raster values using a shapefile.
-    
-    Parameters:
-        
-        image: Optical images. It must be rasterio.io.DatasetReader with 3d or 2d.
-        
-        shp: Vector file, tipically shapefile.
-        
-    Return:
-    
-        A dataframe with raster values obtained.
-        
-    Note:
-        This function is usually used to extract raster values to be used on machine 
-        learning algorithms.
-    '''
-    
-    if not isinstance(image, (rasterio.io.DatasetReader)):
-        raise TypeError('"image" must be raster read by rasterio.open().')
-    
-    if not isinstance(shp, (gpd.geodataframe.GeoDataFrame)):
-        raise TypeError('"shp" must be Shapefile (.shp)')
-    
-    gdf = gpd.GeoDataFrame(geometry = shp['geometry'])
-    
-    coords = [(x,y) for x, y in zip(gdf['geometry'].x, gdf['geometry'].y)]
-    
-    gdf['values'] = [x for x in image.sample(coords)]
-    
-    bands_total = gdf['values'][0].shape[0]
-    
-    col_names = [f'band{i}' for i in range(1, bands_total + 1)]
-    
-    df = pd.DataFrame(gdf["values"].to_list(), columns = col_names)
-    
-    join_df = pd.concat([shp.iloc[:,0], df], axis = 1, join = 'inner')
-
-    if join_df.isnull().values.any():
-        raise TypeError('DataFrame contains nan values. Check it out')
-        
-    return join_df
-
-
-def confintervalML(matrix, image_pred, pixel_size = 10, conf = 1.96, nodata = None):
-    
-    '''
-    The error matrix is a simple cross-tabulation of the class labels allocated by the classification of the remotely 
-    sensed data against the reference data for the sample sites. The error matrix organizes the acquired sample data 
-    in a way that summarizes key results and aids the quantification of accuracy and area. The main diagonal of the error 
-    matrix highlights correct classifications while the off-diagonal elements show omission and commission errors. 
-    The cell entries and marginal values of the error matrix are fundamental to both accuracy assessment and area 
-    estimation. The cell entries of the population error matrix and the parameters derived from it must be estimated 
-    from a sample. This function shows how to obtain a confusion matrix by estimated proportions of area with a confidence
-    interval at 95% (1.96).
-     
-    Parameters:
-    
-        matrix: confusion matrix or error matrix in numpy.ndarray.
-            
-        image_pred: Array with 2d (rows, cols). This array should be the image classified with predicted classes.
-            
-        pixel_size: Pixel size of the image classified. By default is 10m of Sentinel-2.
-            
-        conf: Confidence interval. By default is 95%.
-    
-    Return:
-        
-        Information of confusion matrix by proportions of area, overall accuracy, user's accuracy with confidence interval 
-        and estimated area with confidence interval as well.
-        
-    Note:
-        Columns and rows in a confusion matrix indicate reference and prediction respectively. 
-        
-    Reference:
-    - Olofsson, P., Foody, G.M., Herold, M., Stehman, S.V., Woodcock, C.E., and Wulder, M.A. 2014. “Good practices 
-      for estimating area and assessing accuracy of land change.” Remote Sensing of Environment, Vol. 148: 42–57. 
-      doi:https://doi.org/10.1016/j.rse.2014.02.015.
-    
-    '''
-    
-    if not isinstance(matrix, (np.ndarray)):
-        raise TypeError('"matrix" must be numpy.ndarray with rows and cols.')
-        
-    if not isinstance(image_pred, (np.ndarray)):
-        raise TypeError('"image" must be numpy.ndarray with rows and cols.')
-    
-    # xlabel
-    if nodata is None:
-        image_pred = image_pred
-    else:
-        image_pred[image_pred == nodata] = np.nan
-        
-    # classes
-    iclass = np.unique(image_pred[~np.isnan(image_pred)])
-    
-    # ni
-    ni = np.sum(matrix, axis = 1)
-    
-    # number of classes
-    n = matrix.shape[0]
-    
-    pixels = []
-    
-    for i in iclass:
-        pixels.append((image_pred == i).sum()) #((30**2)/10000) # ha    
-    
-    wi = (np.array([pixels])/np.array([pixels]).sum()).flatten()
-    
-    pixels = np.array(pixels)
-    
-    # copy of matrix
-    matConf = matrix.astype(float).copy()
-    
-    for i in range(n):
-        matConf[i,:] = (matConf[i,:]/ni[i])*wi[i]
-    
-    # user's accuracy
-    ua = np.diag(matConf)/np.sum(matConf, axis = 1)
-    
-    # total Wi
-    total_wi = np.sum(matConf, axis = 1)
-    
-    # copy the matrix of proportions
-    mat_conf = matConf.copy()
-    # building the matrix of proportion area
-    mat_conf = np.concatenate([mat_conf, total_wi.reshape(n, 1)], axis = 1)
-    mat_conf = np.concatenate([mat_conf, pixels.reshape(n, 1)], axis = 1)
-    # total Wi in rows
-    total = np.sum(mat_conf, axis = 0)
-    # final matrix
-    mat_conf = np.concatenate([mat_conf, total.reshape(1, n+2)], axis = 0)
-    
-    namesCol = []
-    for i in np.arange(1, n + 1): namesCol.append(str(i))
-    namesCol.extend(['Total[Wi]', 'Area[pixels]'])
-
-    namesRow = []
-    for i in np.arange(1, n + 1): namesRow.append(str(i))
-    namesRow.extend(['Total'])
-
-    # error matrix (DataFrame) in proportions of area
-    cm_prop_area = pd.DataFrame(np.round(mat_conf, 4), columns = namesCol, index = namesRow)
-    
-    # overall accuracy
-    oa = np.diag(matConf).sum()/np.sum(matConf)
-    
-    # confidence interval for Overall accuracy at 95% 1.96
-    conf_int_oa = list(map(lambda Wi, UA, Ni: (Wi)**2*UA*(1-UA)/(Ni-1), wi, ua, ni))
-    conf_int_oa = conf*np.sqrt(np.nansum((np.array(conf_int_oa))))
-        
-    # confidence interval for user's accuracy at 95% 1.96
-    conf_int_ua = conf*np.sqrt(np.array(list(map(lambda UA, Ni: UA*(1-UA)/(Ni-1), ua, ni))))
-    conf_int_ua[np.isnan(conf_int_ua)] = 0
-    
-    # confidence interval for the area at 95%
-    sp = []
-    for i in np.arange(n):
-        s_pi = list(map(lambda Wi, Pik, Ni: (Wi*Pik - Pik**2)/(Ni-1), wi, matConf[:,i], ni))
-        s_pi = np.sqrt(np.nansum(np.array(s_pi)))
-        sp.append(s_pi)
-    
-    # S(A)=1.96*s(p)*A(total) in ha
-    SA = conf*np.array(sp)*(np.array(pixels).sum())*(pixel_size**2/10000)
-    
-    # Area total estimated
-    A = total[0:n]*(np.array(pixels).sum())*(pixel_size**2/10000)
-    
-    # print info
-    def print_info(matrixCEA, a, b, c, d):
-        print('***** Confusion Matrix by Estimated Proportions of area an uncertainty*****')
-        print('')
-        print('Overall accuracy with 95%')
-        print(f'{oa:.4f} ± {conf_int_oa:.4f}')
-        print('')
-        print('Confusion matrix')
-        print(matrixCEA)
-        print('')
-        print('User´s accuracy with 95%')
-        for i in range(b.shape[0]):
-            print(f'{iclass[i]}: {a[i]:.4f} ± {b[i]:.4f}')
-        print('')
-        print('Estimating area (Ha) and uncertainty with 95%')
-        for i in range(b.shape[0]):
-            print(f'{iclass[i]}: {c[i]:.4f} ± {d[i]:.4f}')
-            
-    return print_info(cm_prop_area, 
-                      ua, 
-                      conf_int_ua, 
-                      A, 
+# -*- coding: utf-8 -*-
+# +
+import os
+import copy
+import fiona
+import rasterio
+import rasterio.mask
+import numpy as np
+import pandas as pd
+import geopandas as gpd
+
+def crop(image, shp, filename = None, filepath = None):
+    
+    '''
+    This algorithm allows to clip a raster (.tif) including a satellite image using a shapefile.
+    
+    Parameters:
+        
+        image: This parameter can be a string with the raster path (e.g., r'/home/image/b3.tif') or
+        it can be a rasterio.io.DatasetReader type.
+        
+        shp: Vector file, tipically shapefile.
+        
+        filename: The image name to be saved.
+        
+        filepath: The path which the image will be stored.
+        
+    Return:
+    
+        A raster in your filepath.
+    '''
+        
+    if isinstance(image, (str)):
+        
+        image = image.replace(os.sep, '/')
+    
+        shp = shp.replace(os.sep, '/')
+        
+        if filename is None:
+        
+            filename = 'raster'
+    
+        if filepath is None:
+        
+            current_path = os.getcwd()
+        
+            path = current_path.replace(os.sep, '/') + '/' + filename + '.tif'
+        
+        else:
+            path = filepath.replace(os.sep, '/') + '/' + filename + '.tif'
+    
+        path_name = path
+    
+        # read Shapefile
+        with fiona.open(shp, "r") as shapefile:
+            shapes = [feature["geometry"] for feature in shapefile]
+
+        # read image
+        with rasterio.open(image) as src:
+            out_image, out_transform = rasterio.mask.mask(src, shapes, crop = True)
+            out_meta = src.meta
+
+        # save clipped image
+        out_meta.update({"driver": "GTiff",
+                         "height": out_image.shape[1],
+                         "width": out_image.shape[2],
+                         "transform": out_transform})
+
+        with rasterio.open(path_name, "w", **out_meta) as dest:
+            dest.write(out_image)
+    
+    elif isinstance(image, (rasterio.io.DatasetReader)):
+    
+        shp = shp.replace(os.sep, '/')
+        
+        if filename is None:
+        
+            filename = 'raster'
+    
+        if filepath is None:
+        
+            current_path = os.getcwd()
+        
+            path = current_path.replace(os.sep, '/') + '/' + filename + '.tif'
+        
+        else:
+            path = filepath.replace(os.sep, '/') + '/' + filename + '.tif'
+    
+        path_name = path
+    
+        # read Shape file
+        with fiona.open(shp, "r") as shapefile:
+            shapes = [feature["geometry"] for feature in shapefile]
+
+        # read image
+        out_image, out_transform = rasterio.mask.mask(image, shapes, crop = True)
+        out_meta = image.meta
+
+        # save clipped image
+        out_meta.update({"driver": "GTiff",
+                         "height": out_image.shape[1],
+                         "width": out_image.shape[2],
+                         "transform": out_transform})
+
+        with rasterio.open(path_name, "w", **out_meta) as dest:
+            dest.write(out_image)
+        
+    else:
+        raise TypeError(f'"image" must be a string like r"/home/image/b5.tif" or must be rasterio.io.DatasetReader. image = {type(image)}')
+
+        
+def extract(image, shp):
+    
+    '''
+    This algorithm allows to extract raster values using a shapefile.
+    
+    Parameters:
+        
+        image: Optical images. It must be rasterio.io.DatasetReader with 3d or 2d.
+        
+        shp: Vector file, tipically shapefile.
+        
+    Return:
+    
+        A dataframe with raster values obtained.
+        
+    Note:
+        This function is usually used to extract raster values to be used on machine 
+        learning algorithms.
+    '''
+    
+    if not isinstance(image, (rasterio.io.DatasetReader)):
+        raise TypeError('"image" must be raster read by rasterio.open().')
+    
+    if not isinstance(shp, (gpd.geodataframe.GeoDataFrame)):
+        raise TypeError('"shp" must be Shapefile (.shp)')
+    
+    gdf = gpd.GeoDataFrame(geometry = shp['geometry'])
+    
+    coords = [(x,y) for x, y in zip(gdf['geometry'].x, gdf['geometry'].y)]
+    
+    gdf['values'] = [x for x in image.sample(coords)]
+    
+    bands_total = gdf['values'][0].shape[0]
+    
+    col_names = [f'band{i}' for i in range(1, bands_total + 1)]
+    
+    df = pd.DataFrame(gdf["values"].to_list(), columns = col_names)
+    
+    join_df = pd.concat([shp.iloc[:,0], df], axis = 1, join = 'inner')
+
+    if join_df.isnull().values.any():
+        raise TypeError('DataFrame contains nan values. Check it out')
+        
+    return join_df
+
+
+def confintervalML(matrix, image_pred, pixel_size = 10, conf = 1.96, nodata = None):
+    
+    '''
+    The error matrix is a simple cross-tabulation of the class labels allocated by the classification of the remotely 
+    sensed data against the reference data for the sample sites. The error matrix organizes the acquired sample data 
+    in a way that summarizes key results and aids the quantification of accuracy and area. The main diagonal of the error 
+    matrix highlights correct classifications while the off-diagonal elements show omission and commission errors. 
+    The cell entries and marginal values of the error matrix are fundamental to both accuracy assessment and area 
+    estimation. The cell entries of the population error matrix and the parameters derived from it must be estimated 
+    from a sample. This function shows how to obtain a confusion matrix by estimated proportions of area with a confidence
+    interval at 95% (1.96).
+     
+    Parameters:
+    
+        matrix: confusion matrix or error matrix in numpy.ndarray.
+            
+        image_pred: Array with 2d (rows, cols). This array should be the image classified with predicted classes.
+            
+        pixel_size: Pixel size of the image classified. By default is 10m of Sentinel-2.
+            
+        conf: Confidence interval. By default is 95%.
+    
+    Return:
+        
+        Information of confusion matrix by proportions of area, overall accuracy, user's accuracy with confidence interval 
+        and estimated area with confidence interval as well.
+        
+    Note:
+        Columns and rows in a confusion matrix indicate reference and prediction respectively. 
+        
+    Reference:
+    - Olofsson, P., Foody, G.M., Herold, M., Stehman, S.V., Woodcock, C.E., and Wulder, M.A. 2014. “Good practices 
+      for estimating area and assessing accuracy of land change.” Remote Sensing of Environment, Vol. 148: 42–57. 
+      doi:https://doi.org/10.1016/j.rse.2014.02.015.
+    
+    '''
+    
+    if not isinstance(matrix, (np.ndarray)):
+        raise TypeError('"matrix" must be numpy.ndarray with rows and cols.')
+        
+    if not isinstance(image_pred, (np.ndarray)):
+        raise TypeError('"image" must be numpy.ndarray with rows and cols.')
+    
+    # xlabel
+    if nodata is None:
+        image_pred = image_pred
+    else:
+        image_pred[image_pred == nodata] = np.nan
+        
+    # classes
+    iclass = np.unique(image_pred[~np.isnan(image_pred)])
+    
+    # ni
+    ni = np.sum(matrix, axis = 1)
+    
+    # number of classes
+    n = matrix.shape[0]
+    
+    pixels = []
+    
+    for i in iclass:
+        pixels.append((image_pred == i).sum()) #((30**2)/10000) # ha    
+    
+    wi = (np.array([pixels])/np.array([pixels]).sum()).flatten()
+    
+    pixels = np.array(pixels)
+    
+    # copy of matrix
+    matConf = matrix.astype(float).copy()
+    
+    for i in range(n):
+        matConf[i,:] = (matConf[i,:]/ni[i])*wi[i]
+    
+    # user's accuracy
+    ua = np.diag(matConf)/np.sum(matConf, axis = 1)
+    
+    # total Wi
+    total_wi = np.sum(matConf, axis = 1)
+    
+    # copy the matrix of proportions
+    mat_conf = matConf.copy()
+    # building the matrix of proportion area
+    mat_conf = np.concatenate([mat_conf, total_wi.reshape(n, 1)], axis = 1)
+    mat_conf = np.concatenate([mat_conf, pixels.reshape(n, 1)], axis = 1)
+    # total Wi in rows
+    total = np.sum(mat_conf, axis = 0)
+    # final matrix
+    mat_conf = np.concatenate([mat_conf, total.reshape(1, n+2)], axis = 0)
+    
+    namesCol = []
+    for i in np.arange(1, n + 1): namesCol.append(str(i))
+    namesCol.extend(['Total[Wi]', 'Area[pixels]'])
+
+    namesRow = []
+    for i in np.arange(1, n + 1): namesRow.append(str(i))
+    namesRow.extend(['Total'])
+
+    # error matrix (DataFrame) in proportions of area
+    cm_prop_area = pd.DataFrame(np.round(mat_conf, 4), columns = namesCol, index = namesRow)
+    
+    # overall accuracy
+    oa = np.diag(matConf).sum()/np.sum(matConf)
+    
+    # confidence interval for Overall accuracy at 95% 1.96
+    conf_int_oa = list(map(lambda Wi, UA, Ni: (Wi)**2*UA*(1-UA)/(Ni-1), wi, ua, ni))
+    conf_int_oa = conf*np.sqrt(np.nansum((np.array(conf_int_oa))))
+        
+    # confidence interval for user's accuracy at 95% 1.96
+    conf_int_ua = conf*np.sqrt(np.array(list(map(lambda UA, Ni: UA*(1-UA)/(Ni-1), ua, ni))))
+    conf_int_ua[np.isnan(conf_int_ua)] = 0
+    
+    # confidence interval for the area at 95%
+    sp = []
+    for i in np.arange(n):
+        s_pi = list(map(lambda Wi, Pik, Ni: (Wi*Pik - Pik**2)/(Ni-1), wi, matConf[:,i], ni))
+        s_pi = np.sqrt(np.nansum(np.array(s_pi)))
+        sp.append(s_pi)
+    
+    # S(A)=1.96*s(p)*A(total) in ha
+    SA = conf*np.array(sp)*(np.array(pixels).sum())*(pixel_size**2/10000)
+    
+    # Area total estimated
+    A = total[0:n]*(np.array(pixels).sum())*(pixel_size**2/10000)
+    
+    # print info
+    def print_info(matrixCEA, a, b, c, d):
+        print('***** Confusion Matrix by Estimated Proportions of area an uncertainty*****')
+        print('')
+        print('Overall accuracy with 95%')
+        print(f'{oa:.4f} ± {conf_int_oa:.4f}')
+        print('')
+        print('Confusion matrix')
+        print(matrixCEA)
+        print('')
+        print('User´s accuracy with 95%')
+        for i in range(b.shape[0]):
+            print(f'{iclass[i]}: {a[i]:.4f} ± {b[i]:.4f}')
+        print('')
+        print('Estimating area (Ha) and uncertainty with 95%')
+        for i in range(b.shape[0]):
+            print(f'{iclass[i]}: {c[i]:.4f} ± {d[i]:.4f}')
+            
+    return print_info(cm_prop_area, 
+                      ua, 
+                      conf_int_ua, 
+                      A, 
                       SA)
```

### Comparing `scikeo-0.2.12/scikeo/rkmeans.py` & `scikeo-0.2.13/scikeo/rkmeans.py`

 * *Files identical despite different names*

### Comparing `scikeo-0.2.12/scikeo/sma.py` & `scikeo-0.2.13/scikeo/sma.py`

 * *Ordering differences only*

 * *Files 11% similar despite different names*

```diff
@@ -1,98 +1,98 @@
-# +
-import rasterio
-import numpy as np
-
-def sma(image, endmembers, nodata = -99999):
-    
-    '''
-    The SMA assumes that the energy received within the field of vision of the remote sensor 
-    can be considered as the sum of the energies received from each dominant endmember. 
-    This function addresses a Linear Mixing Model.
-    
-    A regression analysis is used to obtain the fractions. In least squares inversion algorithms, 
-    the common objective is to estimate abundances that minimize the squared error between the 
-    actual spectrum and the estimated spectrum. The values of the fractions will be between 0 and 1.
-    
-    Parameters:
-    
-        image: Optical images. It must be rasterio.io.DatasetReader with 3d.
-        
-        endmembers: Endmembers must be a matrix (numpy.ndarray) and with more than one endmember. 
-                    Rows represent the endmembers and columns represent the spectral bands.
-                    The number of bands must be greater than the number of endmembers.
-                    E.g. an image with 6 bands, endmembers dimension should be $n*6$, where $n$ 
-                    is rows with the number of endmembers and 6 is the number of bands 
-                    (should be equal).
-                    
-        nodata: The NoData value to replace with -99999.
-    
-    Return:
-    
-        numpy.ndarray with 2d.
-        
-    References
-    Adams, J. B., Smith, M. O., & Gillespie, A. R. (1993). Imaging spectroscopy:
-    Interpretation based on spectral mixture analysis. In C. M. Pieters & P.
-    Englert (Eds.), Remote geochemical analysis: Elements and mineralogical
-    composition. NY: Cambridge Univ. Press 145-166 pp.
-    
-    Shimabukuro, Y.E. and Smith, J., (1991). The least squares mixing models to
-    generate fraction images derived from remote sensing multispectral data.
-    IEEE Transactions on Geoscience and Remote Sensing, 29, pp. 16-21.
-    
-    Note:
-    A regression analysis is used to obtain the fractions. In least squares
-    inversion algorithms, the common objective is to estimate abundances that
-    minimize the squared error between the actual spectrum and the estimated spectrum.
-    The values of the fractions will be between 0 and 1.
-    '''
-    
-    if not isinstance(image, (rasterio.io.DatasetReader)):
-        raise TypeError('"image" must be raster read by rasterio.open().')
-        
-    if not isinstance (endmembers, (np.ndarray)):
-        raise ErrorType('"endmembers" must be numpy.ndarray.')
-    
-    bands = image.count
-        
-    rows = image.height
-        
-    cols = image.width
-    
-    # number of endmembers
-    n_endm = endmembers.shape[0]
-    
-    # number of bands extracted for each endmember
-    b_endm = endmembers.shape[1]
-        
-    st = image.read()
-        
-    # data in [rows, cols, bands]
-    st_reorder = np.moveaxis(st, 0, -1) 
-    # data in [rows*cols, bands]
-    arr = st_reorder.reshape((rows*cols, bands))
-    
-    # nodata
-    if np.isnan(np.sum(arr)):
-        arr[np.isnan(arr)] = self.nodata
-    
-    if not arr.shape[1] > n_endm:
-        raise ValueError('The number of bands must be greater than the number of endmembers.')
-    
-    if not arr.shape[1] == b_endm:
-        raise ValueError('The number of values extracted in band should be equal.')
-    
-    M = np.transpose(endmembers)
-    
-    mat_oper = np.dot(np.linalg.inv(np.dot(np.transpose(M), M)), np.transpose(M)) 
-    
-    frac = np.zeros((rows*cols, n_endm))
-                
-    for i in np.arange(0, n_endm, 1):
-        for j in np.arange(0, rows*cols, 1):
-            f = np.dot(mat_oper, arr[j,:])
-            frac[j,i] = f[i,]
-    
-    sma_img = frac.reshape((rows, cols, n_endm))
-    
-    return sma_img
+# +
+import rasterio
+import numpy as np
+
+def sma(image, endmembers, nodata = -99999):
+    
+    '''
+    The SMA assumes that the energy received within the field of vision of the remote sensor 
+    can be considered as the sum of the energies received from each dominant endmember. 
+    This function addresses a Linear Mixing Model.
+    
+    A regression analysis is used to obtain the fractions. In least squares inversion algorithms, 
+    the common objective is to estimate abundances that minimize the squared error between the 
+    actual spectrum and the estimated spectrum. The values of the fractions will be between 0 and 1.
+    
+    Parameters:
+    
+        image: Optical images. It must be rasterio.io.DatasetReader with 3d.
+        
+        endmembers: Endmembers must be a matrix (numpy.ndarray) and with more than one endmember. 
+                    Rows represent the endmembers and columns represent the spectral bands.
+                    The number of bands must be greater than the number of endmembers.
+                    E.g. an image with 6 bands, endmembers dimension should be $n*6$, where $n$ 
+                    is rows with the number of endmembers and 6 is the number of bands 
+                    (should be equal).
+                    
+        nodata: The NoData value to replace with -99999.
+    
+    Return:
+    
+        numpy.ndarray with 2d.
+        
+    References
+    Adams, J. B., Smith, M. O., & Gillespie, A. R. (1993). Imaging spectroscopy:
+    Interpretation based on spectral mixture analysis. In C. M. Pieters & P.
+    Englert (Eds.), Remote geochemical analysis: Elements and mineralogical
+    composition. NY: Cambridge Univ. Press 145-166 pp.
+    
+    Shimabukuro, Y.E. and Smith, J., (1991). The least squares mixing models to
+    generate fraction images derived from remote sensing multispectral data.
+    IEEE Transactions on Geoscience and Remote Sensing, 29, pp. 16-21.
+    
+    Note:
+    A regression analysis is used to obtain the fractions. In least squares
+    inversion algorithms, the common objective is to estimate abundances that
+    minimize the squared error between the actual spectrum and the estimated spectrum.
+    The values of the fractions will be between 0 and 1.
+    '''
+    
+    if not isinstance(image, (rasterio.io.DatasetReader)):
+        raise TypeError('"image" must be raster read by rasterio.open().')
+        
+    if not isinstance (endmembers, (np.ndarray)):
+        raise ErrorType('"endmembers" must be numpy.ndarray.')
+    
+    bands = image.count
+        
+    rows = image.height
+        
+    cols = image.width
+    
+    # number of endmembers
+    n_endm = endmembers.shape[0]
+    
+    # number of bands extracted for each endmember
+    b_endm = endmembers.shape[1]
+        
+    st = image.read()
+        
+    # data in [rows, cols, bands]
+    st_reorder = np.moveaxis(st, 0, -1) 
+    # data in [rows*cols, bands]
+    arr = st_reorder.reshape((rows*cols, bands))
+    
+    # nodata
+    if np.isnan(np.sum(arr)):
+        arr[np.isnan(arr)] = self.nodata
+    
+    if not arr.shape[1] > n_endm:
+        raise ValueError('The number of bands must be greater than the number of endmembers.')
+    
+    if not arr.shape[1] == b_endm:
+        raise ValueError('The number of values extracted in band should be equal.')
+    
+    M = np.transpose(endmembers)
+    
+    mat_oper = np.dot(np.linalg.inv(np.dot(np.transpose(M), M)), np.transpose(M)) 
+    
+    frac = np.zeros((rows*cols, n_endm))
+                
+    for i in np.arange(0, n_endm, 1):
+        for j in np.arange(0, rows*cols, 1):
+            f = np.dot(mat_oper, arr[j,:])
+            frac[j,i] = f[i,]
+    
+    sma_img = frac.reshape((rows, cols, n_endm))
+    
+    return sma_img
```

### Comparing `scikeo-0.2.12/scikeo/tassCap.py` & `scikeo-0.2.13/scikeo/tassCap.py`

 * *Files identical despite different names*

### Comparing `scikeo-0.2.12/scikeo/writeRaster.py` & `scikeo-0.2.13/scikeo/writeRaster.py`

 * *Files identical despite different names*

### Comparing `scikeo-0.2.12/scikeo.egg-info/SOURCES.txt` & `scikeo-0.2.13/scikeo.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `scikeo-0.2.12/setup.py` & `scikeo-0.2.13/setup.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,57 +1,57 @@
-#!/usr/bin/env python
-"""The setup script."""
-
-import io
-from os import path as op
-from setuptools import setup, find_packages
-
-with open('README.md') as readme_file:
-    readme = readme_file.read()
-
-here = op.abspath(op.dirname(__file__))
-
-# get the dependencies and installs
-with io.open(op.join(here, "requirements.txt"), encoding="utf-8") as f:
-    all_reqs = f.read().split("\n")
-
-install_requires = [x.strip() for x in all_reqs if "git+" not in x]
-dependency_links = [x.strip().replace("git+", "") for x in all_reqs if "git+" not in x]
-
-requirements = [ ]
-
-setup_requirements = [ ]
-
-test_requirements = [ ]
-
-setup(
-    author="Yonatan Tarazona Coronel",
-    author_email='geoyons@gmail.com',
-    python_requires='>=3.5',
-    classifiers=[
-        #'Development Status ::  2 - Pre-Alpha',
-        'Intended Audience :: Developers',
-        'License :: OSI Approved :: Apache Software License',
-        'Natural Language :: English',
-        'Programming Language :: Python :: 3',
-        'Programming Language :: Python :: 3.5',
-        'Programming Language :: Python :: 3.6',
-        'Programming Language :: Python :: 3.7',
-        'Programming Language :: Python :: 3.8',
-    ],
-    description="Remote Sensing Tools",
-    install_requires=install_requires,
-    dependency_links=dependency_links,
-    license="Apache Software License 2.0",
-    long_description=readme,
-    long_description_content_type='text/markdown',
-    include_package_data=True,
-    keywords='scikeo',
-    name='scikeo',
-    packages=find_packages(include=['scikeo', 'scikeo.*']),
-    setup_requires=setup_requirements,
-    test_suite='tests',
-    tests_require=test_requirements,
-    url='https://github.com/ytarazona/scikit-eo',
-    version='0.2.12',
-    zip_safe=False,
-)
+#!/usr/bin/env python
+"""The setup script."""
+
+import io
+from os import path as op
+from setuptools import setup, find_packages
+
+with open('README.md') as readme_file:
+    readme = readme_file.read()
+
+here = op.abspath(op.dirname(__file__))
+
+# get the dependencies and installs
+with io.open(op.join(here, "requirements.txt"), encoding="utf-8") as f:
+    all_reqs = f.read().split("\n")
+
+install_requires = [x.strip() for x in all_reqs if "git+" not in x]
+dependency_links = [x.strip().replace("git+", "") for x in all_reqs if "git+" not in x]
+
+requirements = [ ]
+
+setup_requirements = [ ]
+
+test_requirements = [ ]
+
+setup(
+    author="Yonatan Tarazona Coronel",
+    author_email='geoyons@gmail.com',
+    python_requires='>=3.5',
+    classifiers=[
+        #'Development Status ::  2 - Pre-Alpha',
+        'Intended Audience :: Developers',
+        'License :: OSI Approved :: Apache Software License',
+        'Natural Language :: English',
+        'Programming Language :: Python :: 3',
+        'Programming Language :: Python :: 3.5',
+        'Programming Language :: Python :: 3.6',
+        'Programming Language :: Python :: 3.7',
+        'Programming Language :: Python :: 3.8',
+    ],
+    description="Remote Sensing Tools",
+    install_requires=install_requires,
+    dependency_links=dependency_links,
+    license="Apache Software License 2.0",
+    long_description=readme,
+    long_description_content_type='text/markdown',
+    include_package_data=True,
+    keywords='scikeo',
+    name='scikeo',
+    packages=find_packages(include=['scikeo', 'scikeo.*']),
+    setup_requires=setup_requirements,
+    test_suite='tests',
+    tests_require=test_requirements,
+    url='https://github.com/ytarazona/scikit-eo',
+    version='0.2.13',
+    zip_safe=False,
+)
```

