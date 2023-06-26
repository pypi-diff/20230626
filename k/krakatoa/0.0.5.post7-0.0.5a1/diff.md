# Comparing `tmp/krakatoa-0.0.5.post7.tar.gz` & `tmp/krakatoa-0.0.5a1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "krakatoa-0.0.5.post7.tar", last modified: Mon Jun 26 13:46:55 2023, max compression
+gzip compressed data, was "krakatoa-0.0.5a1.tar", last modified: Tue Dec 27 19:54:13 2022, max compression
```

## Comparing `krakatoa-0.0.5.post7.tar` & `krakatoa-0.0.5a1.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 13:46:55.389068 krakatoa-0.0.5.post7/
--rw-r--r--   0 runner    (1001) docker     (123)     1064 2023-06-26 13:46:43.000000 krakatoa-0.0.5.post7/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      859 2023-06-26 13:46:55.389068 krakatoa-0.0.5.post7/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      433 2023-06-26 13:46:43.000000 krakatoa-0.0.5.post7/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 13:46:55.381068 krakatoa-0.0.5.post7/krakatoa/
--rw-r--r--   0 runner    (1001) docker     (123)      349 2023-06-26 13:46:43.000000 krakatoa-0.0.5.post7/krakatoa/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 13:46:55.385068 krakatoa-0.0.5.post7/krakatoa/future/
--rw-r--r--   0 runner    (1001) docker     (123)      404 2023-06-26 13:46:43.000000 krakatoa-0.0.5.post7/krakatoa/future/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6455 2023-06-26 13:46:43.000000 krakatoa-0.0.5.post7/krakatoa/future/analysis.py
--rw-r--r--   0 runner    (1001) docker     (123)     1114 2023-06-26 13:46:43.000000 krakatoa-0.0.5.post7/krakatoa/future/evaluate.py
--rw-r--r--   0 runner    (1001) docker     (123)     1529 2023-06-26 13:46:43.000000 krakatoa-0.0.5.post7/krakatoa/future/experiment.py
--rw-r--r--   0 runner    (1001) docker     (123)     7957 2023-06-26 13:46:43.000000 krakatoa-0.0.5.post7/krakatoa/future/preprocess.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 13:46:55.389068 krakatoa-0.0.5.post7/krakatoa/models/
--rw-r--r--   0 runner    (1001) docker     (123)      346 2023-06-26 13:46:43.000000 krakatoa-0.0.5.post7/krakatoa/models/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    28354 2023-06-26 13:46:43.000000 krakatoa-0.0.5.post7/krakatoa/models/_config.py
--rw-r--r--   0 runner    (1001) docker     (123)     1165 2023-06-26 13:46:43.000000 krakatoa-0.0.5.post7/krakatoa/models/_getmodels.py
--rw-r--r--   0 runner    (1001) docker     (123)     2320 2023-06-26 13:46:43.000000 krakatoa-0.0.5.post7/krakatoa/models/_metrics.py
--rw-r--r--   0 runner    (1001) docker     (123)    21076 2023-06-26 13:46:43.000000 krakatoa-0.0.5.post7/krakatoa/models/autotune.py
--rw-r--r--   0 runner    (1001) docker     (123)     8248 2023-06-26 13:46:43.000000 krakatoa-0.0.5.post7/krakatoa/models/quick.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 13:46:55.381068 krakatoa-0.0.5.post7/krakatoa.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      859 2023-06-26 13:46:55.000000 krakatoa-0.0.5.post7/krakatoa.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      526 2023-06-26 13:46:55.000000 krakatoa-0.0.5.post7/krakatoa.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-26 13:46:55.000000 krakatoa-0.0.5.post7/krakatoa.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       34 2023-06-26 13:46:55.000000 krakatoa-0.0.5.post7/krakatoa.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       41 2023-06-26 13:46:55.000000 krakatoa-0.0.5.post7/krakatoa.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       79 2023-06-26 13:46:55.389068 krakatoa-0.0.5.post7/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1152 2023-06-26 13:46:43.000000 krakatoa-0.0.5.post7/setup.py
+drwxrwxrwx   0        0        0        0 2022-12-27 19:54:13.265231 krakatoa-0.0.5a1/
+-rw-rw-rw-   0        0        0     1084 2022-12-27 18:23:30.000000 krakatoa-0.0.5a1/LICENSE
+-rw-rw-rw-   0        0        0      728 2022-12-27 19:54:13.265231 krakatoa-0.0.5a1/PKG-INFO
+-rw-rw-rw-   0        0        0      448 2022-12-27 18:23:30.000000 krakatoa-0.0.5a1/README.md
+drwxrwxrwx   0        0        0        0 2022-12-27 19:54:13.250219 krakatoa-0.0.5a1/krakatoa/
+-rw-rw-rw-   0        0        0      363 2022-12-27 18:23:30.000000 krakatoa-0.0.5a1/krakatoa/__init__.py
+drwxrwxrwx   0        0        0        0 2022-12-27 19:54:13.257219 krakatoa-0.0.5a1/krakatoa/future/
+-rw-rw-rw-   0        0        0      420 2022-12-27 19:22:04.000000 krakatoa-0.0.5a1/krakatoa/future/__init__.py
+-rw-rw-rw-   0        0        0     4992 2022-12-27 19:21:04.000000 krakatoa-0.0.5a1/krakatoa/future/analysis.py
+-rw-rw-rw-   0        0        0      966 2022-12-27 19:21:04.000000 krakatoa-0.0.5a1/krakatoa/future/evaluate.py
+-rw-rw-rw-   0        0        0     1584 2022-12-27 19:21:04.000000 krakatoa-0.0.5a1/krakatoa/future/experiment.py
+-rw-rw-rw-   0        0        0     8192 2022-12-27 19:21:04.000000 krakatoa-0.0.5a1/krakatoa/future/preprocess.py
+drwxrwxrwx   0        0        0        0 2022-12-27 19:54:13.262219 krakatoa-0.0.5a1/krakatoa/models/
+-rw-rw-rw-   0        0        0      360 2022-12-27 18:23:30.000000 krakatoa-0.0.5a1/krakatoa/models/__init__.py
+-rw-rw-rw-   0        0        0    29218 2022-12-27 19:21:04.000000 krakatoa-0.0.5a1/krakatoa/models/_config.py
+-rw-rw-rw-   0        0        0     1208 2022-12-27 19:21:04.000000 krakatoa-0.0.5a1/krakatoa/models/_getmodels.py
+-rw-rw-rw-   0        0        0     2370 2022-12-27 19:21:04.000000 krakatoa-0.0.5a1/krakatoa/models/_metrics.py
+-rw-rw-rw-   0        0        0    21564 2022-12-27 19:21:04.000000 krakatoa-0.0.5a1/krakatoa/models/autotune.py
+-rw-rw-rw-   0        0        0     8537 2022-12-27 19:21:04.000000 krakatoa-0.0.5a1/krakatoa/models/quick.py
+drwxrwxrwx   0        0        0        0 2022-12-27 19:54:13.254219 krakatoa-0.0.5a1/krakatoa.egg-info/
+-rw-rw-rw-   0        0        0      728 2022-12-27 19:54:13.000000 krakatoa-0.0.5a1/krakatoa.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      836 2022-12-27 19:54:13.000000 krakatoa-0.0.5a1/krakatoa.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2022-12-27 19:54:13.000000 krakatoa-0.0.5a1/krakatoa.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       29 2022-12-27 19:54:13.000000 krakatoa-0.0.5a1/krakatoa.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       41 2022-12-27 19:54:13.000000 krakatoa-0.0.5a1/krakatoa.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       86 2022-12-27 19:54:13.266229 krakatoa-0.0.5a1/setup.cfg
+-rw-rw-rw-   0        0        0     1015 2022-12-27 19:53:57.000000 krakatoa-0.0.5a1/setup.py
```

### Comparing `krakatoa-0.0.5.post7/LICENSE` & `krakatoa-0.0.5a1/LICENSE`

 * *Ordering differences only*

 * *Files 11% similar despite different names*

```diff
@@ -1,21 +1,21 @@
-MIT License
-
-Copyright (c) 2022 aitec-mp
-
-Permission is hereby granted, free of charge, to any person obtaining a copy
-of this software and associated documentation files (the "Software"), to deal
-in the Software without restriction, including without limitation the rights
-to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
-copies of the Software, and to permit persons to whom the Software is
-furnished to do so, subject to the following conditions:
-
-The above copyright notice and this permission notice shall be included in all
-copies or substantial portions of the Software.
-
-THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
-IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
-FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
-AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
-LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
-OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
+MIT License
+
+Copyright (c) 2022 aitec-mp
+
+Permission is hereby granted, free of charge, to any person obtaining a copy
+of this software and associated documentation files (the "Software"), to deal
+in the Software without restriction, including without limitation the rights
+to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
+copies of the Software, and to permit persons to whom the Software is
+furnished to do so, subject to the following conditions:
+
+The above copyright notice and this permission notice shall be included in all
+copies or substantial portions of the Software.
+
+THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
+IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
+FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
+AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
+LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
+OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
 SOFTWARE.
```

### Comparing `krakatoa-0.0.5.post7/krakatoa/future/evaluate.py` & `krakatoa-0.0.5a1/krakatoa/future/evaluate.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,41 +1,34 @@
-# -*- coding: utf-8 -*-
-
-'''
-Data Evaluation (:mod:`krakatoa.future.evaluate`)
-============================================================
-'''
-
-# ============================================================
-# Imports
-# ============================================================
-
-import pandas as pd
-import numpy as np
-
-# ============================================================
-
-
-def categoryPerFeature(df, columns, sort=True):
-    n_categories_per_feature = df[columns].apply(lambda x: len(set(x)))
-
-    if sort:
-        n_categories_per_feature = n_categories_per_feature.sort_values(
-            ascending=False)
-
-    return n_categories_per_feature
-
-
-def countNull(df):
-
-    # result = ''
-
-    # if mode == 'perc':
-    #     result = (((df.isnull().sum() | df.eq('').sum())/df.shape[0])*100)
-    # elif mode == 'count':
-    #     result = (df.isnull().sum() | df.eq('').sum()).to_dict()
-
-    return pd.DataFrame({
-        'variable': list(df.columns),
-        'perc': (((df.isnull().sum() | df.eq('').sum())/df.shape[0])*100).values,
-        'count': (df.isnull().sum() | df.eq('').sum()).values
-    })
+# -*- coding: utf-8 -*-
+
+'''
+Data Evaluation (:mod:`krakatoa.future.evaluate`)
+============================================================
+'''
+
+#============================================================
+# Imports
+#============================================================
+
+import pandas as pd
+import numpy as np
+
+#============================================================
+def categoryPerFeature(df, columns, sort=True):
+    n_categories_per_feature = df[columns].apply(lambda x : len(set(x)))
+    
+    if sort:
+        n_categories_per_feature = n_categories_per_feature.sort_values(ascending=False)
+        
+    
+    return n_categories_per_feature
+    
+def countNull(df, mode='count'):
+    
+    result = ''
+    
+    if mode == 'perc':
+        result = (((df.isnull().sum() | df.eq('').sum())/df.shape[0])*100)
+    elif mode == 'count':
+        result = (df.isnull().sum() | df.eq('').sum()).to_dict()
+
+    return result
```

### Comparing `krakatoa-0.0.5.post7/krakatoa/future/preprocess.py` & `krakatoa-0.0.5a1/krakatoa/future/preprocess.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,256 +1,257 @@
-# -*- coding: utf-8 -*-
-
-'''
-Data preprocessing (:mod:`krakatoa.future.preprocess`)
-============================================================
-'''
-
-#============================================================
-# Imports
-#============================================================
-
-import pandas as pd
-from pandas.api.types import is_string_dtype, is_numeric_dtype, is_categorical_dtype
-import numpy as np
-import sys
-sys.path.append("../../")
-
-
-from sklearn.model_selection import train_test_split
-from sklearn.preprocessing import MinMaxScaler, StandardScaler, RobustScaler, MaxAbsScaler
-from sklearn.preprocessing import OrdinalEncoder
-from krakatoa.future.evaluate import countNull
-from sklearn.preprocessing import OneHotEncoder
-
-#============================================================
-def changeColType(df, columns, newType):
-    
-    for col in columns:
-        df[col] = df[col].astype(newType)
-        
-    return df
-
-def splitDataset(x, y, test_size=0.3, random_state=0):
-    x_train, x_test, y_train, y_test = train_test_split(x, 
-                                                        y, 
-                                                        test_size=test_size, 
-                                                        random_state=random_state)
-    
-    y_train, y_test = np.array(y_train).ravel(), np.array(y_test).ravel()
-    
-    return x_train, x_test, y_train, y_test
-
-def scale(dataset, columns, scaler='min_max'):
-    
-    scalers = {
-        'min_max' : MinMaxScaler(),
-        'max_abs' : MaxAbsScaler(),
-        'robust' : RobustScaler(),
-        'standard' : StandardScaler()
-        }
-    
-    cur_scaler = scalers.get(scaler)
-    dataset[columns] = cur_scaler.fit_transform(dataset[columns])
-    
-    return {
-        "scaler" : cur_scaler,
-        "dataset" : dataset
-    }
-
-
-# Class designed to dataset management   
-class DataClean():
-
-    def __init__(self, target):
-        self.dataset = pd.DataFrame()
-        self.originalDataset = pd.DataFrame()
-        self.target = target
-
-    def loadDataset(self, dataset, load_from="dataframe"):
-        if load_from == "dataframe":
-            self.dataset = dataset
-            self.originalDataset = dataset
-        elif load_from == "dict":
-            self.dataset = pd.DataFrame(dataset)
-            self.originalDataset = pd.DataFrame(dataset)
-        else:
-            print("Error! Select the right Dataset type and set it to load_from variable ('dataframe', 'dict')")
-
-        self._getUniqueFeatures()
-        self._nullPercFeatures()
-
-    def getColType(self):
-        
-        # TODO precisamos ainda identificar colunas de outros tipos , como data e quando é numerica e categorica
-        catCols = []
-        numCols = []
-        
-
-        for k, v in self.dataset.dtypes.items():
-            if v in ['object', 'category']:
-                catCols.append(k)
-            elif k != self.target:
-                numCols.append(k)
-
-        self.category_cols = catCols
-        self.numeric_cols = numCols
-        self.target_col = [self.target]
- 
-    def splitTrainTest(self):
-
-        X = self.dataset.drop(columns=[self.target])
-        y = self.dataset[self.target]
-
-        self.X = X
-        self.y = y
-
-        return X, y
-
-    def _nullPercFeatures(self):
-        result = countNull(self.dataset)
-
-        self.percNull = result
-        return result
-
-    def _getUniqueFeatures(self):
-        dataset = self.dataset.copy()
-
-        catUniqueCount = dataset[self.category_cols].nunique()
-        catUniquePerc = (dataset[self.category_cols].nunique() / dataset.shape[0])*100
-        uniqueCount = dataset.nunique()
-        uniquePerc = (dataset.nunique() / dataset.shape[0])*100
-
-        self.catUniqueCount = catUniqueCount
-        self.catUniquePerc = catUniquePerc
-        self.uniqueCount = uniqueCount
-        self.uniquePerc = uniquePerc
-
-    def dropColumns(self, columns):
-
-        self.dataset.drop(columns=columns, inplace=True)
-        return self.dataset
-    
-    def dropNaColumns(self, threshold=50):
-        
-        percNull = self._nullPercFeatures()
-
-        self.dataset.drop(columns=list(percNull[percNull > threshold].keys()), inplace=True)
-        return self.dataset
-    
-    def fillNa(self, strategy='mean'): #mean / most frequent | drop 
-        # preencher com media | mais frequente (caso categorico)
-        self.getColType()
-        dataset = self.dataset.copy()
-        if strategy == "mean":
-            for numc in self.numeric_cols:
-                mean = dataset[numc].mean()
-                dataset[numc].fillna(mean, inplace=True)
-            
-            # categoricos por mais frequentes
-            for catc in self.category_cols:
-                mode = dataset[catc].mode()[0]
-                dataset[catc].fillna(mode, inplace=True)
-        elif strategy == "drop":
-            dataset.dropna(inplace=True)
-
-        self.dataset = dataset
-        return self.dataset
-
-    def cleanUnique(self, threshold=500):
-
-        self._getUniqueFeatures()
-
-        dataset = self.dataset.copy()
-        col_drop = list(self.uniqueCount[self.uniqueCount > threshold].keys())
-
-        # Dont drop target column for any reason | Dont drop numeric columns
-        col_drop = [x for x in col_drop if x != self.target and x not in (self.numeric_cols)] 
-
-        dataset.drop(columns=col_drop, inplace=True)
-
-        self.dataset = dataset
-
-
-        # refresh column data in self
-        self.getColType()
-
-        return self.dataset
-
-    def getDummies(self):
-
-        # self.dataset = pd.get_dummies(self.dataset)
-        # return self.dataset
-        self.dataset.reset_index(inplace=True, drop=True)
-
-        cat_cols = self.category_cols
-
-        # Instancia e fit one hot encoder
-        hot = OneHotEncoder(handle_unknown='ignore', sparse=False)
-        hot.fit(self.dataset[cat_cols])
-
-        hot_ds = hot.transform(self.dataset[cat_cols])
-
-        # Cria dataframe transformada
-        hot_df = pd.DataFrame(hot_ds, columns = hot.get_feature_names_out(input_features=cat_cols))
-
-        # Concatena o dataframe do one hot com o original
-        concat_df = pd.concat([self.dataset, hot_df], axis=1).drop(columns=cat_cols, axis=1)
-        self.oneHotEncoding = hot
-        self.dataset = concat_df
-
-        return self.dataset
-
-    def dataScale(self, scaler='min_max'):
-
-        res_scale = scale(self.dataset, columns=self.numeric_cols, scaler=scaler)
-
-        self.dataset = res_scale["dataset"]
-        self.scaler = res_scale["scaler"]
-
-        return self.dataset
-
-
-    def pipeline(self, steps):
-
-        _config = {
-            'dataset' : self.loadDataset,
-            'splitColType' : self.getColType,
-            'dropNaCol' : self.dropNaColumns,
-            'fillNa' : self.fillNa,
-            'cleanUnique' : self.cleanUnique,
-            'getDummies' : self.getDummies,
-            'scale' : self.dataScale,
-            'dropCol' : self.dropColumns,
-            # 'target' : self.setTarget,
-        }
-
-        for step, args in steps:
-            fun = _config.get(step) #Else mostra error TODO
-            fun(**args)
-            
-        return self.dataset
-
-    def fit_transform(self, dataset, dropThresh=50, fillNaStrategy='mean', uniqueThresh=500, scaler='min_max'): #Metodo automatizado | pipeline
-
-        # self.loadDataset(dataset)
-        # self.getColType()
-        # self.dropNaColumns(threshold=dropThresh)
-        # self.fillNa(strategy=fillNaStrategy)
-        # self.cleanUnique(threshold=uniqueThresh)
-        # self.getDummies()
-        # self.scale(scaler=scaler)
-
-        self.pipeline(steps=[
-            ('dataset', {'dataset' : dataset}),
-            ('splitColType', {}),
-            ('dropNaCol', {'threshold' : dropThresh}),
-            ('fillNa', {'strategy' : fillNaStrategy}),
-            ('cleanUnique', {'threshold' : uniqueThresh}),
-            ('getDummies', {}),
-            ('scale', {'scaler' : scaler})
-            ])
-        
-        return self.dataset
-
-
-       
+# -*- coding: utf-8 -*-
+
+'''
+Data preprocessing (:mod:`krakatoa.future.preprocess`)
+============================================================
+'''
+
+#============================================================
+# Imports
+#============================================================
+
+import pandas as pd
+from pandas.api.types import is_string_dtype, is_numeric_dtype, is_categorical_dtype
+import numpy as np
+import sys
+sys.path.append("../../")
+
+
+from sklearn.model_selection import train_test_split
+from sklearn.preprocessing import MinMaxScaler, StandardScaler, RobustScaler, MaxAbsScaler
+from sklearn.preprocessing import OrdinalEncoder
+from krakatoa.future.evaluate import countNull
+from sklearn.preprocessing import OneHotEncoder
+
+#============================================================
+def changeColType(df, columns, newType):
+    
+    for col in columns:
+        df[col] = df[col].astype(newType)
+        
+    return df
+
+def splitDataset(x, y, test_size=0.3, random_state=0):
+    x_train, x_test, y_train, y_test = train_test_split(x, 
+                                                        y, 
+                                                        test_size=test_size, 
+                                                        random_state=random_state)
+    
+    y_train, y_test = np.array(y_train).ravel(), np.array(y_test).ravel()
+    
+    return x_train, x_test, y_train, y_test
+
+def scale(dataset, columns, scaler='min_max'):
+    
+    scalers = {
+        'min_max' : MinMaxScaler(),
+        'max_abs' : MaxAbsScaler(),
+        'robust' : RobustScaler(),
+        'standard' : StandardScaler()
+        }
+    
+    cur_scaler = scalers.get(scaler)
+    dataset[columns] = cur_scaler.fit_transform(dataset[columns])
+    
+    return {
+        "scaler" : cur_scaler,
+        "dataset" : dataset
+    }
+
+
+# Class designed to dataset management   
+class DataClean():
+
+    def __init__(self, target, mode):
+        self.dataset = pd.DataFrame()
+        self.originalDataset = pd.DataFrame()
+        self.target = target
+        self.mode = mode
+
+    def loadDataset(self, dataset, load_from="dataframe"):
+        if load_from == "dataframe":
+            self.dataset = dataset
+            self.originalDataset = dataset
+        elif load_from == "dict":
+            self.dataset = pd.DataFrame(dataset)
+            self.originalDataset = pd.DataFrame(dataset)
+        else:
+            print("Error! Select the right Dataset type and set it to load_from variable ('dataframe', 'dict')")
+
+
+
+    def getColType(self):
+        
+        # TODO precisamos ainda identificar colunas de outros tipos , como data e quando é numerica e categorica
+        catCols = []
+        numCols = []
+        
+
+        for k, v in self.dataset.dtypes.items():
+            if v in ['object', 'category']:
+                catCols.append(k)
+            elif k != self.target:
+                numCols.append(k)
+
+        self.category_cols = catCols
+        self.numeric_cols = numCols
+        self.target_col = [self.target]
+
+    
+    def splitTrainTest(self):
+
+        X = self.dataset.drop(columns=[self.target])
+        y = self.dataset[self.target]
+
+        self.X = X
+        self.y = y
+
+        return X, y
+
+    def _nullPercFeatures(self):
+        result = countNull(self.dataset, mode='perc')
+
+        self.percNull = result
+        return result
+
+    def _getUniqueFeatures(self):
+        dataset = self.dataset.copy()
+
+        catUniqueCount = dataset[self.category_cols].nunique()
+        catUniquePerc = (dataset[self.category_cols].nunique() / dataset.shape[0])*100
+        uniqueCount = dataset.nunique()
+        uniquePerc = (dataset.nunique() / dataset.shape[0])*100
+
+        self.catUniqueCount = catUniqueCount
+        self.catUniquePerc = catUniquePerc
+        self.uniqueCount = uniqueCount
+        self.uniquePerc = uniquePerc
+
+    def dropColumns(self, columns):
+
+        self.dataset.drop(columns=columns, inplace=True)
+        return self.dataset
+    
+    def dropNaColumns(self, threshold=50):
+        
+        percNull = self._nullPercFeatures()
+
+        self.dataset.drop(columns=list(percNull[percNull > threshold].keys()), inplace=True)
+        return self.dataset
+    
+    def fillNa(self, strategy='mean'): #mean / most frequent | drop 
+        # preencher com media | mais frequente (caso categorico)
+        self.getColType()
+        dataset = self.dataset.copy()
+        if strategy == "mean":
+            for numc in self.numeric_cols:
+                mean = dataset[numc].mean()
+                dataset[numc].fillna(mean, inplace=True)
+            
+            # categoricos por mais frequentes
+            for catc in self.category_cols:
+                mode = dataset[catc].mode()[0]
+                dataset[catc].fillna(mode, inplace=True)
+        elif strategy == "drop":
+            dataset.dropna(inplace=True)
+
+        self.dataset = dataset
+        return self.dataset
+
+    def cleanUnique(self, threshold=500):
+
+        self._getUniqueFeatures()
+
+        dataset = self.dataset.copy()
+        col_drop = list(self.uniqueCount[self.uniqueCount > threshold].keys())
+
+        # Dont drop target column for any reason | Dont drop numeric columns
+        col_drop = [x for x in col_drop if x != self.target and x not in (self.numeric_cols)] 
+
+        dataset.drop(columns=col_drop, inplace=True)
+
+        self.dataset = dataset
+
+
+        # refresh column data in self
+        self.getColType()
+
+        return self.dataset
+
+    def getDummies(self):
+
+        # self.dataset = pd.get_dummies(self.dataset)
+        # return self.dataset
+        self.dataset.reset_index(inplace=True, drop=True)
+
+        cat_cols = self.category_cols
+
+        # Instancia e fit one hot encoder
+        hot = OneHotEncoder(handle_unknown='ignore', sparse=False)
+        hot.fit(self.dataset[cat_cols])
+
+        hot_ds = hot.transform(self.dataset[cat_cols])
+
+        # Cria dataframe transformada
+        hot_df = pd.DataFrame(hot_ds, columns = hot.get_feature_names(input_features=cat_cols))
+
+        # Concatena o dataframe do one hot com o original
+        concat_df = pd.concat([self.dataset, hot_df], axis=1).drop(columns=cat_cols, axis=1)
+        self.oneHotEncoding = hot
+        self.dataset = concat_df
+
+        return self.dataset
+
+    def dataScale(self, scaler='min_max'):
+
+        res_scale = scale(self.dataset, columns=self.numeric_cols, scaler=scaler)
+
+        self.dataset = res_scale["dataset"]
+        self.scaler = res_scale["scaler"]
+
+        return self.dataset
+
+
+    def pipeline(self, steps):
+
+        _config = {
+            'dataset' : self.loadDataset,
+            'splitColType' : self.getColType,
+            'dropNaCol' : self.dropNaColumns,
+            'fillNa' : self.fillNa,
+            'cleanUnique' : self.cleanUnique,
+            'getDummies' : self.getDummies,
+            'scale' : self.dataScale,
+            'dropCol' : self.dropColumns,
+            # 'target' : self.setTarget,
+        }
+
+        for step, args in steps:
+            fun = _config.get(step) #Else mostra error TODO
+            fun(**args)
+            
+        return self.dataset
+
+    def fit_transform(self, dataset, dropThresh=50, fillNaStrategy='mean', uniqueThresh=500, scaler='min_max'): #Metodo automatizado | pipeline
+
+        # self.loadDataset(dataset)
+        # self.getColType()
+        # self.dropNaColumns(threshold=dropThresh)
+        # self.fillNa(strategy=fillNaStrategy)
+        # self.cleanUnique(threshold=uniqueThresh)
+        # self.getDummies()
+        # self.scale(scaler=scaler)
+
+        self.pipeline(steps=[
+            ('dataset', {'dataset' : dataset}),
+            ('splitColType', {}),
+            ('dropNaCol', {'threshold' : dropThresh}),
+            ('fillNa', {'strategy' : fillNaStrategy}),
+            ('cleanUnique', {'threshold' : uniqueThresh}),
+            ('getDummies', {}),
+            ('scale', {'scaler' : scaler})
+            ])
+        
+        return self.dataset
+
+
+
```

### Comparing `krakatoa-0.0.5.post7/krakatoa/models/_getmodels.py` & `krakatoa-0.0.5a1/krakatoa/models/_getmodels.py`

 * *Ordering differences only*

 * *Files 22% similar despite different names*

```diff
@@ -1,43 +1,43 @@
-# -*- coding: utf-8 -*-
-
-'''
-Configuration file(:mod:`krakatoa._getmodels`)
-============================================================
-'''
-
-# ============================================================
-# Imports
-# ============================================================
-
-from ._config import getConfigRegr, getConfigClass
-
-# ============================================================
-# Get models
-# ============================================================
-def getModels(mode, modelClasses, selMode = 'type', random_state=0):
-    
-
-    if mode == 'regression':
-        config = getConfigRegr()
-    elif mode == 'classification':
-        config = getConfigClass()
-    else:
-        #TODO error implementation
-        print('No configuration was selected')
-        config = None
-
-
-    if config != None:
-
-        configVals = [x for x in config.values()] 
-        result = []
-
-        if selMode in ['type', 'name']:
-            
-            for m in modelClasses:
-                res = list(filter(lambda x: x[selMode] == m, configVals))
-                
-                for r in res:
-                    result.append(r)
-        
-        return result
+# -*- coding: utf-8 -*-
+
+'''
+Configuration file(:mod:`krakatoa._getmodels`)
+============================================================
+'''
+
+# ============================================================
+# Imports
+# ============================================================
+
+from ._config import getConfigRegr, getConfigClass
+
+# ============================================================
+# Get models
+# ============================================================
+def getModels(mode, modelClasses, selMode = 'type', random_state=0):
+    
+
+    if mode == 'regression':
+        config = getConfigRegr()
+    elif mode == 'classification':
+        config = getConfigClass()
+    else:
+        #TODO error implementation
+        print('No configuration was selected')
+        config = None
+
+
+    if config != None:
+
+        configVals = [x for x in config.values()] 
+        result = []
+
+        if selMode in ['type', 'name']:
+            
+            for m in modelClasses:
+                res = list(filter(lambda x: x[selMode] == m, configVals))
+                
+                for r in res:
+                    result.append(r)
+        
+        return result
```

### Comparing `krakatoa-0.0.5.post7/krakatoa/models/_metrics.py` & `krakatoa-0.0.5a1/krakatoa/models/_metrics.py`

 * *Ordering differences only*

 * *Files 16% similar despite different names*

```diff
@@ -1,50 +1,50 @@
-# -*- coding: utf-8 -*-
-
-'''
-Metrics file(:mod:`krakatoa.models._metrics`)
-============================================================
-'''
-
-#============================================================
-# Imports
-#============================================================
-
-from sklearn import metrics
-
-#============================================================
-# Metrics
-#============================================================
-#TODO: Criar modulo para metrics
-
-def getScores(kind):
-
-    regression_scores = {
-        'explained_variance' : {'f' : metrics.explained_variance_score, 'name' : 'explained_variance'},
-        'max_error' : {'f' : metrics.max_error, 'name' : 'max_error'},
-        'mae' : {'f' : metrics.mean_absolute_error, 'name' : 'neg_mean_absolute_error'},
-        'mse' : {'f' : metrics.mean_squared_error, 'name' : 'neg_mean_squared_error'},
-        'rmse' : {'f' : metrics.mean_squared_error, 'name' : 'neg_root_mean_squared_error'}, #TODO: criar funcao RMSE,
-        'msle' : {'f' : metrics.mean_squared_log_error, 'name' : 'neg_mean_squared_log_error'},
-        'neg_median_absolute_error' : {'f' : metrics.median_absolute_error, 'name' : 'neg_median_absolute_error'},
-        'r2' : {'f' : metrics.r2_score, 'name' : 'r2'},
-        'poison' : {'f' : metrics.mean_poisson_deviance, 'name' : 'neg_mean_poisson_deviance'},
-        'gama' : {'f' : metrics.mean_gamma_deviance, 'name' : 'neg_mean_gamma_deviance'},
-        'neg_mean_absolute_percentage_error' : {'f' : metrics.mean_absolute_percentage_error, 'name' : 'neg_mean_absolute_percentage_error'},
-        'd2_absolute_error_score' : {'f' : metrics.d2_absolute_error_score, 'name' : 'd2_absolute_error_score'},
-        'd2_pinball_score' : {'f' : metrics.d2_pinball_score, 'name' : 'd2_pinball_score'},
-        'd2_tweedie_score' : {'f' : metrics.d2_tweedie_score, 'name' : 'd2_tweedie_score'}
-        }
-
-
-    classification_scores = {
-        'accuracy' : {'f' : metrics.accuracy_score, 'name' : 'accuracy'},
-        'balanced_accuracy' : {'f' : metrics.balanced_accuracy_score, 'name' : 'balanced_accuracy'},
-        'roc_auc' : {'f' : metrics.roc_auc_score, 'name' : 'roc_auc'}
-        }
-
-    if kind == "classification":
-        scores = classification_scores
-    else:
-        scores = regression_scores
-    
-    return scores
+# -*- coding: utf-8 -*-
+
+'''
+Metrics file(:mod:`krakatoa.models._metrics`)
+============================================================
+'''
+
+#============================================================
+# Imports
+#============================================================
+
+from sklearn import metrics
+
+#============================================================
+# Metrics
+#============================================================
+#TODO: Criar modulo para metrics
+
+def getScores(kind):
+
+    regression_scores = {
+        'explained_variance' : {'f' : metrics.explained_variance_score, 'name' : 'explained_variance'},
+        'max_error' : {'f' : metrics.max_error, 'name' : 'max_error'},
+        'mae' : {'f' : metrics.mean_absolute_error, 'name' : 'neg_mean_absolute_error'},
+        'mse' : {'f' : metrics.mean_squared_error, 'name' : 'neg_mean_squared_error'},
+        'rmse' : {'f' : metrics.mean_squared_error, 'name' : 'neg_root_mean_squared_error'}, #TODO: criar funcao RMSE,
+        'msle' : {'f' : metrics.mean_squared_log_error, 'name' : 'neg_mean_squared_log_error'},
+        'neg_median_absolute_error' : {'f' : metrics.median_absolute_error, 'name' : 'neg_median_absolute_error'},
+        'r2' : {'f' : metrics.r2_score, 'name' : 'r2'},
+        'poison' : {'f' : metrics.mean_poisson_deviance, 'name' : 'neg_mean_poisson_deviance'},
+        'gama' : {'f' : metrics.mean_gamma_deviance, 'name' : 'neg_mean_gamma_deviance'},
+        'neg_mean_absolute_percentage_error' : {'f' : metrics.mean_absolute_percentage_error, 'name' : 'neg_mean_absolute_percentage_error'},
+        'd2_absolute_error_score' : {'f' : metrics.d2_absolute_error_score, 'name' : 'd2_absolute_error_score'},
+        'd2_pinball_score' : {'f' : metrics.d2_pinball_score, 'name' : 'd2_pinball_score'},
+        'd2_tweedie_score' : {'f' : metrics.d2_tweedie_score, 'name' : 'd2_tweedie_score'}
+        }
+
+
+    classification_scores = {
+        'accuracy' : {'f' : metrics.accuracy_score, 'name' : 'accuracy'},
+        'balanced_accuracy' : {'f' : metrics.balanced_accuracy_score, 'name' : 'balanced_accuracy'},
+        'roc_auc' : {'f' : metrics.roc_auc_score, 'name' : 'roc_auc'}
+        }
+
+    if kind == "classification":
+        scores = classification_scores
+    else:
+        scores = regression_scores
+    
+    return scores
```

### Comparing `krakatoa-0.0.5.post7/krakatoa/models/autotune.py` & `krakatoa-0.0.5a1/krakatoa/models/autotune.py`

 * *Ordering differences only*

 * *Files 19% similar despite different names*

```diff
@@ -1,488 +1,488 @@
-# -*- coding: utf-8 -*-
-
-'''
-AutoTune models(:mod:`krakatoa.models.autotune`)
-============================================================
-'''
-
-#============================================================
-# Imports
-#============================================================
-
-from sklearn.model_selection import GridSearchCV
-from ._getmodels import getModels
-from ._metrics import getScores
-
-
-import numpy as np
-import math
-
-from sklearn.utils._testing import ignore_warnings
-from sklearn.exceptions import ConvergenceWarning
-
-#============================================================
-# Regression Functions
-#============================================================
-
-@ignore_warnings(category=ConvergenceWarning)
-class RegressorAF():
-
-    def __init__(self):
-        self._regression_scores = getScores('regression')
-
-    def fit(self, estimator, x, y, score=['r2'], cv=3, verbose=0, lr=0.001, random_state=0):
-        results = {}
-        modelConfig = getModels(mode='regression', modelClasses=[estimator], selMode='name', random_state=random_state)
-
-        #Collector variables
-        models = np.array([])
-        opt_params = dict()
-        scores = np.array([])
-        
-        if len(modelConfig) > 0:
-            #Model definition
-            # model = model[0]['estimator']
-            modelConfig = modelConfig[0]
-            model = modelConfig.get('estimator', '')
-
-            scoring = []
-            for s in score:
-                scoring.append(self._regression_scores[s]['name'])
-                            
-            #carrega parametros
-            # num_parameters = {key:attr['vals'] for key, attr in modelConfig['attr'].items() if attr['type'] == 'num' and attr['iterable'] == False}
-            # num_parameters = {key:attr for key, attr in modelConfig['attr'].items() if attr['type'] == 'num' and attr['iterable'] == False}
-            daux = {key:attr for key, attr in modelConfig['attr'].items() if attr['type'] == 'num'}
-
-            # Alterado para que seja uma lista ordenada | pois dict nao pode ser |
-            num_parameters = []
-            for k, p in daux.items():
-                p['key'] = k
-                num_parameters.append(p)
-
-
-            num_parameters = sorted(num_parameters, key= lambda item:item['iterable'])
-
-            best_score = 0
-            best_params = {}
-            # for k, p in num_parameters.items(): 
-            for item in num_parameters: 
- 
-                #Specific attr cfg
-                # paramCfg = modelConfig['attr'][k]
-                paramCfg = modelConfig['attr'][item['key']]
-
-                stop = False
-                #Process once to discover the best of initial three parameters
-                grid_params =  {**{_k:np.array([_v]) for _k, _v in opt_params.items()}, item['key']:item['vals']}
-                grid = GridSearchCV(model, param_grid=grid_params, cv=cv, n_jobs=-1, verbose=0)
-                grid.fit(x, y)
-                
-                # Verifica se aplicando o grid search melhora resultados
-                # se nao melhorar nao entra no pipeline para descobrir melhores parametros
-                if grid.best_score_ > best_score:
-                    
-                    best_score = grid.best_score_
-                    best_params = grid.best_params_
-                    
-                    last_best_model = grid.best_estimator_
-                    last_best_score = best_score
-                    last_best_param = best_params
-                    
-                else:
-                    stop = True
-                    
-                if item['iterable'] == False:
-                    param_range = item['vals']
-                    
-                    if verbose > 0:
-                        print(f'-------- {item["key"]} ----------')
-                    # TODO> Abstrair para um função             
-                    while stop == False:
-                        # if last_best_param[k] == None:
-                        if last_best_param[item['key']] == None:
-                            stop = True
-                            break
-
-                        # spec_best_param = last_best_param[k]
-                        spec_best_param = last_best_param[item['key']]
-                        
-                        #identify if the value is in the center, left or right
-                        index = np.where(param_range == spec_best_param)[0][0]
-                        #left
-                        if index == 0: 
-                            lim_r = param_range[1]
-                            lim_l = 0
-                        elif index == 1:
-                            lim_r = param_range[2]
-                            lim_l = param_range[0]
-                        else:
-                            lim_r = spec_best_param*2 #TODO: Melhorar logica 
-                            lim_l = param_range[1]
-
-                        # Calculo dos novos limites a esquerda e direita    
-                        aux_param_l = (spec_best_param - lim_l)/2
-                        aux_param_r = (lim_r - spec_best_param)/2 + spec_best_param
-
-                        param_l = aux_param_l if aux_param_l >= 0 else lim_l
-                        param_r = aux_param_r if aux_param_r >= 0 else lim_r
-
-                        # Verifica o tipo da variavel, se for INT devemos garantir que nao esteja passando como float e resolver
-
-                        # if isinstance(paramCfg['ntype'], int):
-                        if paramCfg['ntype'] == int:
-                            param_l = int(math.ceil(param_l))
-                            param_r = int(math.ceil(param_r))
-
-
-                        #re do parameter range
-                        param_range = np.array([param_l, spec_best_param , param_r])
-                        
-                        _grid_params =  {**{_k:np.array([_v]) for _k, _v in opt_params.items()}, item['key']:param_range}
-                        _grid = GridSearchCV(model, param_grid=_grid_params, cv=cv, n_jobs=-1, verbose=0)
-                        _grid.fit(x, y)
-                        
-                        _best_score = _grid.best_score_
-                        _best_params = _grid.best_params_
-                        _best_model = _grid.best_estimator_
-                        
-                        #  Show verbose if it is necessary
-                        if verbose > 0:
-                            
-                            print("-----------------")
-                            print("Range =====> ", param_range)
-                            print("opt params: ", _grid_params)
-                            print("Score: ", _best_score)
-                            print("Params: ", _best_params)
-                            print("Diff: ", (_best_score - last_best_score))
-                            print("-----------------")
-                            
-                        if _best_score > last_best_score:
-                            _diff = _best_score - last_best_score
-                            
-                            last_best_model = _best_model
-                            last_best_score = _best_score
-                            # last_best_param[k] = _best_params[k]
-                            last_best_param[item['key']] = _best_params[item['key']]
-                        
-                            if _diff <= lr:
-                                stop = True
-                                
-                        else:
-                            stop = True
-
-                # Trecho para iteraveis
-                # TODO melhorar essa parte deixando mais robusto
-                else:
-                    if verbose > 0:
-                        print(f'-------- {item["key"]} ----------')
-                    min_try = 5 # Quantidade minima de tentativas  antes de sair do loop
-                    value = item['init_val']
-                    step = item['def_step']
-                    maxVal = item['max']
-                    hist_value = [] #tuple com value e accuracy
-
-                    stop = False
-                    try_count = 1
-
-                    while stop == False:
-
-                        _grid_params =  {**{_k:np.array([_v]) for _k, _v in opt_params.items()}, item['key']:[value]}
-                        _grid = GridSearchCV(model, param_grid=_grid_params, cv=cv, n_jobs=-1, verbose=0)
-                        _grid.fit(x, y)
-                        
-                        _best_score = _grid.best_score_
-                        _best_params = _grid.best_params_
-                        _best_model = _grid.best_estimator_
-                        
-                        print("_best_score")
-                        print(_best_score)
-                        hist_value.append((value, _best_score))
-                        #  Show verbose if it is necessary
-                        if verbose > 0:
-                            
-                            print("-----------------")
-                            print("Value =====> ", value)
-                            print("opt params: ", _grid_params)
-                            print("Score: ", _best_score)
-                            print("Params: ", _best_params)
-                            print("Diff: ", (_best_score - last_best_score))
-                            print("-----------------")
-                            
-                            
-                        _diff = _best_score - last_best_score
-                        
-                        if last_best_score < _best_score:
-                            last_best_model = _best_model
-                            last_best_score = _best_score
-                            # last_best_param[k] = _best_params[k]
-                            last_best_param[item['key']] = _best_params[item['key']]
-                    
-                        if (_diff <= lr and try_count >= min_try) or (maxVal == value):
-                            stop = True
-                            print(hist_value)
-                            # maxValue = max(hist_value, key=lambda item:item[1])
-                        elif _diff >= lr and (min_try - try_count) < 2:
-                            print("reset")
-                            try_count = 0
-                            min_try = 3 #Zera o contador e deixa pelo menor 3 a mais para tentar
-
-                        try_count += 1
-                        value += step
-
-                
-                #Store best params and results
-
-                models = np.append(models, last_best_model)
-                opt_params = {**opt_params, **last_best_param}
-                scores = np.append(scores, last_best_score)
-                    
-        
-        results = {
-            'models' : models,
-            'best_params' : opt_params,
-            'scores' : scores
-            }
-
-        return results
-    
-    
-class ClassifierAF():
-
-    def __init__(self):
-        self._classification_score = getScores('classification')
-
-    def fit(self, estimator, x, y, score=['accuracy'], cv=3, verbose=0, lr=0.001, random_state=0):
-        results = {}
-        modelConfig = getModels(mode='classification', modelClasses=[estimator], selMode='name', random_state=random_state)
-
-        #Collector variables
-        models = np.array([])
-        opt_params = dict()
-        scores = np.array([])
-        
-        if len(modelConfig) > 0:
-            #Model definition
-            # model = model[0]['estimator']
-            modelConfig = modelConfig[0]
-            model = modelConfig.get('estimator', '')
-
-            scoring = []
-            for s in score:
-                scoring.append(self._classification_score[s]['name'])
-                            
-            #carrega parametros
-            # num_parameters = {key:attr['vals'] for key, attr in modelConfig['attr'].items() if attr['type'] == 'num' and attr['iterable'] == False}
-            # num_parameters = {key:attr for key, attr in modelConfig['attr'].items() if attr['type'] == 'num' and attr['iterable'] == False}
-            daux = {key:attr for key, attr in modelConfig['attr'].items() if attr['type'] == 'num'}
-
-            # Alterado para que seja uma lista ordenada | pois dict nao pode ser |
-            num_parameters = []
-            for k, p in daux.items():
-                p['key'] = k
-                num_parameters.append(p)
-
-
-            num_parameters = sorted(num_parameters, key= lambda item:item['iterable'])
-
-            best_score = 0
-            best_params = {}
-            # for k, p in num_parameters.items(): 
-            for item in num_parameters: 
- 
-                #Specific attr cfg
-                # paramCfg = modelConfig['attr'][k]
-                paramCfg = modelConfig['attr'][item['key']]
-
-                stop = False
-                #Process once to discover the best of initial three parameters
-                grid_params =  {**{_k:np.array([_v]) for _k, _v in opt_params.items()}, item['key']:item['vals']}
-                grid = GridSearchCV(model, param_grid=grid_params, cv=cv, n_jobs=-1, verbose=0)
-                grid.fit(x, y)
-                
-                # Verifica se aplicando o grid search melhora resultados
-                # se nao melhorar nao entra no pipeline para descobrir melhores parametros
-                if grid.best_score_ > best_score:
-                    
-                    best_score = grid.best_score_
-                    best_params = grid.best_params_
-                    
-                    last_best_model = grid.best_estimator_
-                    last_best_score = best_score
-                    last_best_param = best_params
-                    
-                else:
-                    stop = True
-                    
-                if item['iterable'] == False:
-                    param_range = item['vals']
-                    
-                    if verbose > 0:
-                        print(f'-------- {item["key"]} ----------')
-                        
-                    # TODO> Abstrair para um função             
-                    while stop == False:
-                        # if last_best_param[k] == None:
-                        if last_best_param[item['key']] == None:
-                            stop = True
-                            break
-
-                        # spec_best_param = last_best_param[k]
-                        spec_best_param = last_best_param[item['key']]
-                        
-                        #identify if the value is in the center, left or right
-                        index = np.where(param_range == spec_best_param)[0][0]
-                        #left
-                        if index == 0: 
-                            lim_r = param_range[1]
-                            lim_l = 0
-                        elif index == 1:
-                            lim_r = param_range[2]
-                            lim_l = param_range[0]
-                        else:
-                            lim_r = spec_best_param*2 #TODO: Melhorar logica 
-                            lim_l = param_range[1]
-
-                        # Calculo dos novos limites a esquerda e direita    
-                        aux_param_l = (spec_best_param - lim_l)/2
-                        aux_param_r = (lim_r - spec_best_param)/2 + spec_best_param
-
-                        param_l = aux_param_l if aux_param_l >= 0 else lim_l
-                        param_r = aux_param_r if aux_param_r >= 0 else lim_r
-
-                        # Verifica o tipo da variavel, se for INT devemos garantir que nao esteja passando como float e resolver
-
-                        # if isinstance(paramCfg['ntype'], int):
-                        if paramCfg['ntype'] == int:
-                            param_l = int(math.ceil(param_l))
-                            param_r = int(math.ceil(param_r))
-
-
-                        #re do parameter range
-                        param_range = np.array([param_l, spec_best_param , param_r])
-                        
-                        _grid_params =  {**{_k:np.array([_v]) for _k, _v in opt_params.items()}, item['key']:param_range}
-                        _grid = GridSearchCV(model, param_grid=_grid_params, cv=cv, n_jobs=-1, verbose=0)
-                        _grid.fit(x, y)
-                        
-                        _best_score = _grid.best_score_
-                        _best_params = _grid.best_params_
-                        _best_model = _grid.best_estimator_
-                        
-                        #  Show verbose if it is necessary
-                        if verbose > 0:
-                            
-                            print("-----------------")
-                            print("Range =====> ", param_range)
-                            print("opt params: ", _grid_params)
-                            print("Score: ", _best_score)
-                            print("Params: ", _best_params)
-                            print("Diff: ", (_best_score - last_best_score))
-                            print("-----------------")
-                            
-                        if _best_score > last_best_score:
-                            _diff = _best_score - last_best_score
-                            
-                            last_best_model = _best_model
-                            last_best_score = _best_score
-                            # last_best_param[k] = _best_params[k]
-                            last_best_param[item['key']] = _best_params[item['key']]
-                        
-                            if _diff <= lr:
-                                stop = True
-                                
-                        else:
-                            stop = True
-
-                # Trecho para iteraveis
-                # TODO melhorar essa parte deixando mais robusto
-                else:
-                    if verbose > 0:
-                        print(f'-------- {item["key"]} ----------')
-
-                    min_try = 5 # Quantidade minima de tentativas  antes de sair do loop
-                    value = item['init_val']
-                    step = item['def_step']
-                    maxVal = item['max']
-                    hist_value = [] #tuple com value e accuracy
-
-                    stop = False
-                    try_count = 1
-
-                    while stop == False:
-
-                        _grid_params =  {**{_k:np.array([_v]) for _k, _v in opt_params.items()}, item['key']:[value]}
-                        _grid = GridSearchCV(model, param_grid=_grid_params, cv=cv, n_jobs=-1, verbose=0)
-                        _grid.fit(x, y)
-                        
-                        _best_score = _grid.best_score_
-                        _best_params = _grid.best_params_
-                        _best_model = _grid.best_estimator_
-                        
-                        print("_best_score")
-                        print(_best_score)
-                        hist_value.append((value, _best_score))
-                        #  Show verbose if it is necessary
-                        if verbose > 0:
-                            
-                            print("-----------------")
-                            print("Value =====> ", value)
-                            print("opt params: ", _grid_params)
-                            print("Score: ", _best_score)
-                            print("Params: ", _best_params)
-                            print("Diff: ", (_best_score - last_best_score))
-                            print("-----------------")
-                            
-                            
-                        _diff = _best_score - last_best_score
-                        
-                        if last_best_score < _best_score:
-                            last_best_model = _best_model
-                            last_best_score = _best_score
-                            # last_best_param[k] = _best_params[k]
-                            last_best_param[item['key']] = _best_params[item['key']]
-                    
-                        if (_diff <= lr and try_count >= min_try) or (maxVal == value):
-                            stop = True
-                            print(hist_value)
-                            # maxValue = max(hist_value, key=lambda item:item[1])
-                        elif _diff >= lr and (min_try - try_count) < 2:
-                            print("reset")
-                            try_count = 0
-                            min_try = 3 #Zera o contador e deixa pelo menor 3 a mais para tentar
-
-                        try_count += 1
-                        value += step
-
-                
-                #Store best params and results
-
-                models = np.append(models, last_best_model)
-                opt_params = {**opt_params, **last_best_param}
-                scores = np.append(scores, last_best_score)
-                    
-        
-        results = {
-            'models' : models,
-            'best_params' : opt_params,
-            'scores' : scores
-            }
-
-        return results
-    
-    
-    
-    
-    
-    
-    
-    
-    
-    
-    
-    
-    
-    
-    
-    
-    
+# -*- coding: utf-8 -*-
+
+'''
+AutoTune models(:mod:`krakatoa.models.autotune`)
+============================================================
+'''
+
+#============================================================
+# Imports
+#============================================================
+
+from sklearn.model_selection import GridSearchCV
+from ._getmodels import getModels
+from ._metrics import getScores
+
+
+import numpy as np
+import math
+
+from sklearn.utils._testing import ignore_warnings
+from sklearn.exceptions import ConvergenceWarning
+
+#============================================================
+# Regression Functions
+#============================================================
+
+@ignore_warnings(category=ConvergenceWarning)
+class RegressorAF():
+
+    def __init__(self):
+        self._regression_scores = getScores('regression')
+
+    def fit(self, estimator, x, y, score=['r2'], cv=3, verbose=0, lr=0.001, random_state=0):
+        results = {}
+        modelConfig = getModels(mode='regression', modelClasses=[estimator], selMode='name', random_state=random_state)
+
+        #Collector variables
+        models = np.array([])
+        opt_params = dict()
+        scores = np.array([])
+        
+        if len(modelConfig) > 0:
+            #Model definition
+            # model = model[0]['estimator']
+            modelConfig = modelConfig[0]
+            model = modelConfig.get('estimator', '')
+
+            scoring = []
+            for s in score:
+                scoring.append(self._regression_scores[s]['name'])
+                            
+            #carrega parametros
+            # num_parameters = {key:attr['vals'] for key, attr in modelConfig['attr'].items() if attr['type'] == 'num' and attr['iterable'] == False}
+            # num_parameters = {key:attr for key, attr in modelConfig['attr'].items() if attr['type'] == 'num' and attr['iterable'] == False}
+            daux = {key:attr for key, attr in modelConfig['attr'].items() if attr['type'] == 'num'}
+
+            # Alterado para que seja uma lista ordenada | pois dict nao pode ser |
+            num_parameters = []
+            for k, p in daux.items():
+                p['key'] = k
+                num_parameters.append(p)
+
+
+            num_parameters = sorted(num_parameters, key= lambda item:item['iterable'])
+
+            best_score = 0
+            best_params = {}
+            # for k, p in num_parameters.items(): 
+            for item in num_parameters: 
+ 
+                #Specific attr cfg
+                # paramCfg = modelConfig['attr'][k]
+                paramCfg = modelConfig['attr'][item['key']]
+
+                stop = False
+                #Process once to discover the best of initial three parameters
+                grid_params =  {**{_k:np.array([_v]) for _k, _v in opt_params.items()}, item['key']:item['vals']}
+                grid = GridSearchCV(model, param_grid=grid_params, cv=cv, n_jobs=-1, verbose=0)
+                grid.fit(x, y)
+                
+                # Verifica se aplicando o grid search melhora resultados
+                # se nao melhorar nao entra no pipeline para descobrir melhores parametros
+                if grid.best_score_ > best_score:
+                    
+                    best_score = grid.best_score_
+                    best_params = grid.best_params_
+                    
+                    last_best_model = grid.best_estimator_
+                    last_best_score = best_score
+                    last_best_param = best_params
+                    
+                else:
+                    stop = True
+                    
+                if item['iterable'] == False:
+                    param_range = item['vals']
+                    
+                    if verbose > 0:
+                        print(f'-------- {item["key"]} ----------')
+                    # TODO> Abstrair para um função             
+                    while stop == False:
+                        # if last_best_param[k] == None:
+                        if last_best_param[item['key']] == None:
+                            stop = True
+                            break
+
+                        # spec_best_param = last_best_param[k]
+                        spec_best_param = last_best_param[item['key']]
+                        
+                        #identify if the value is in the center, left or right
+                        index = np.where(param_range == spec_best_param)[0][0]
+                        #left
+                        if index == 0: 
+                            lim_r = param_range[1]
+                            lim_l = 0
+                        elif index == 1:
+                            lim_r = param_range[2]
+                            lim_l = param_range[0]
+                        else:
+                            lim_r = spec_best_param*2 #TODO: Melhorar logica 
+                            lim_l = param_range[1]
+
+                        # Calculo dos novos limites a esquerda e direita    
+                        aux_param_l = (spec_best_param - lim_l)/2
+                        aux_param_r = (lim_r - spec_best_param)/2 + spec_best_param
+
+                        param_l = aux_param_l if aux_param_l >= 0 else lim_l
+                        param_r = aux_param_r if aux_param_r >= 0 else lim_r
+
+                        # Verifica o tipo da variavel, se for INT devemos garantir que nao esteja passando como float e resolver
+
+                        # if isinstance(paramCfg['ntype'], int):
+                        if paramCfg['ntype'] == int:
+                            param_l = int(math.ceil(param_l))
+                            param_r = int(math.ceil(param_r))
+
+
+                        #re do parameter range
+                        param_range = np.array([param_l, spec_best_param , param_r])
+                        
+                        _grid_params =  {**{_k:np.array([_v]) for _k, _v in opt_params.items()}, item['key']:param_range}
+                        _grid = GridSearchCV(model, param_grid=_grid_params, cv=cv, n_jobs=-1, verbose=0)
+                        _grid.fit(x, y)
+                        
+                        _best_score = _grid.best_score_
+                        _best_params = _grid.best_params_
+                        _best_model = _grid.best_estimator_
+                        
+                        #  Show verbose if it is necessary
+                        if verbose > 0:
+                            
+                            print("-----------------")
+                            print("Range =====> ", param_range)
+                            print("opt params: ", _grid_params)
+                            print("Score: ", _best_score)
+                            print("Params: ", _best_params)
+                            print("Diff: ", (_best_score - last_best_score))
+                            print("-----------------")
+                            
+                        if _best_score > last_best_score:
+                            _diff = _best_score - last_best_score
+                            
+                            last_best_model = _best_model
+                            last_best_score = _best_score
+                            # last_best_param[k] = _best_params[k]
+                            last_best_param[item['key']] = _best_params[item['key']]
+                        
+                            if _diff <= lr:
+                                stop = True
+                                
+                        else:
+                            stop = True
+
+                # Trecho para iteraveis
+                # TODO melhorar essa parte deixando mais robusto
+                else:
+                    if verbose > 0:
+                        print(f'-------- {item["key"]} ----------')
+                    min_try = 5 # Quantidade minima de tentativas  antes de sair do loop
+                    value = item['init_val']
+                    step = item['def_step']
+                    maxVal = item['max']
+                    hist_value = [] #tuple com value e accuracy
+
+                    stop = False
+                    try_count = 1
+
+                    while stop == False:
+
+                        _grid_params =  {**{_k:np.array([_v]) for _k, _v in opt_params.items()}, item['key']:[value]}
+                        _grid = GridSearchCV(model, param_grid=_grid_params, cv=cv, n_jobs=-1, verbose=0)
+                        _grid.fit(x, y)
+                        
+                        _best_score = _grid.best_score_
+                        _best_params = _grid.best_params_
+                        _best_model = _grid.best_estimator_
+                        
+                        print("_best_score")
+                        print(_best_score)
+                        hist_value.append((value, _best_score))
+                        #  Show verbose if it is necessary
+                        if verbose > 0:
+                            
+                            print("-----------------")
+                            print("Value =====> ", value)
+                            print("opt params: ", _grid_params)
+                            print("Score: ", _best_score)
+                            print("Params: ", _best_params)
+                            print("Diff: ", (_best_score - last_best_score))
+                            print("-----------------")
+                            
+                            
+                        _diff = _best_score - last_best_score
+                        
+                        if last_best_score < _best_score:
+                            last_best_model = _best_model
+                            last_best_score = _best_score
+                            # last_best_param[k] = _best_params[k]
+                            last_best_param[item['key']] = _best_params[item['key']]
+                    
+                        if (_diff <= lr and try_count >= min_try) or (maxVal == value):
+                            stop = True
+                            print(hist_value)
+                            # maxValue = max(hist_value, key=lambda item:item[1])
+                        elif _diff >= lr and (min_try - try_count) < 2:
+                            print("reset")
+                            try_count = 0
+                            min_try = 3 #Zera o contador e deixa pelo menor 3 a mais para tentar
+
+                        try_count += 1
+                        value += step
+
+                
+                #Store best params and results
+
+                models = np.append(models, last_best_model)
+                opt_params = {**opt_params, **last_best_param}
+                scores = np.append(scores, last_best_score)
+                    
+        
+        results = {
+            'models' : models,
+            'best_params' : opt_params,
+            'scores' : scores
+            }
+
+        return results
+    
+    
+class ClassifierAF():
+
+    def __init__(self):
+        self._classification_score = getScores('classification')
+
+    def fit(self, estimator, x, y, score=['accuracy'], cv=3, verbose=0, lr=0.001, random_state=0):
+        results = {}
+        modelConfig = getModels(mode='classification', modelClasses=[estimator], selMode='name', random_state=random_state)
+
+        #Collector variables
+        models = np.array([])
+        opt_params = dict()
+        scores = np.array([])
+        
+        if len(modelConfig) > 0:
+            #Model definition
+            # model = model[0]['estimator']
+            modelConfig = modelConfig[0]
+            model = modelConfig.get('estimator', '')
+
+            scoring = []
+            for s in score:
+                scoring.append(self._classification_score[s]['name'])
+                            
+            #carrega parametros
+            # num_parameters = {key:attr['vals'] for key, attr in modelConfig['attr'].items() if attr['type'] == 'num' and attr['iterable'] == False}
+            # num_parameters = {key:attr for key, attr in modelConfig['attr'].items() if attr['type'] == 'num' and attr['iterable'] == False}
+            daux = {key:attr for key, attr in modelConfig['attr'].items() if attr['type'] == 'num'}
+
+            # Alterado para que seja uma lista ordenada | pois dict nao pode ser |
+            num_parameters = []
+            for k, p in daux.items():
+                p['key'] = k
+                num_parameters.append(p)
+
+
+            num_parameters = sorted(num_parameters, key= lambda item:item['iterable'])
+
+            best_score = 0
+            best_params = {}
+            # for k, p in num_parameters.items(): 
+            for item in num_parameters: 
+ 
+                #Specific attr cfg
+                # paramCfg = modelConfig['attr'][k]
+                paramCfg = modelConfig['attr'][item['key']]
+
+                stop = False
+                #Process once to discover the best of initial three parameters
+                grid_params =  {**{_k:np.array([_v]) for _k, _v in opt_params.items()}, item['key']:item['vals']}
+                grid = GridSearchCV(model, param_grid=grid_params, cv=cv, n_jobs=-1, verbose=0)
+                grid.fit(x, y)
+                
+                # Verifica se aplicando o grid search melhora resultados
+                # se nao melhorar nao entra no pipeline para descobrir melhores parametros
+                if grid.best_score_ > best_score:
+                    
+                    best_score = grid.best_score_
+                    best_params = grid.best_params_
+                    
+                    last_best_model = grid.best_estimator_
+                    last_best_score = best_score
+                    last_best_param = best_params
+                    
+                else:
+                    stop = True
+                    
+                if item['iterable'] == False:
+                    param_range = item['vals']
+                    
+                    if verbose > 0:
+                        print(f'-------- {item["key"]} ----------')
+                        
+                    # TODO> Abstrair para um função             
+                    while stop == False:
+                        # if last_best_param[k] == None:
+                        if last_best_param[item['key']] == None:
+                            stop = True
+                            break
+
+                        # spec_best_param = last_best_param[k]
+                        spec_best_param = last_best_param[item['key']]
+                        
+                        #identify if the value is in the center, left or right
+                        index = np.where(param_range == spec_best_param)[0][0]
+                        #left
+                        if index == 0: 
+                            lim_r = param_range[1]
+                            lim_l = 0
+                        elif index == 1:
+                            lim_r = param_range[2]
+                            lim_l = param_range[0]
+                        else:
+                            lim_r = spec_best_param*2 #TODO: Melhorar logica 
+                            lim_l = param_range[1]
+
+                        # Calculo dos novos limites a esquerda e direita    
+                        aux_param_l = (spec_best_param - lim_l)/2
+                        aux_param_r = (lim_r - spec_best_param)/2 + spec_best_param
+
+                        param_l = aux_param_l if aux_param_l >= 0 else lim_l
+                        param_r = aux_param_r if aux_param_r >= 0 else lim_r
+
+                        # Verifica o tipo da variavel, se for INT devemos garantir que nao esteja passando como float e resolver
+
+                        # if isinstance(paramCfg['ntype'], int):
+                        if paramCfg['ntype'] == int:
+                            param_l = int(math.ceil(param_l))
+                            param_r = int(math.ceil(param_r))
+
+
+                        #re do parameter range
+                        param_range = np.array([param_l, spec_best_param , param_r])
+                        
+                        _grid_params =  {**{_k:np.array([_v]) for _k, _v in opt_params.items()}, item['key']:param_range}
+                        _grid = GridSearchCV(model, param_grid=_grid_params, cv=cv, n_jobs=-1, verbose=0)
+                        _grid.fit(x, y)
+                        
+                        _best_score = _grid.best_score_
+                        _best_params = _grid.best_params_
+                        _best_model = _grid.best_estimator_
+                        
+                        #  Show verbose if it is necessary
+                        if verbose > 0:
+                            
+                            print("-----------------")
+                            print("Range =====> ", param_range)
+                            print("opt params: ", _grid_params)
+                            print("Score: ", _best_score)
+                            print("Params: ", _best_params)
+                            print("Diff: ", (_best_score - last_best_score))
+                            print("-----------------")
+                            
+                        if _best_score > last_best_score:
+                            _diff = _best_score - last_best_score
+                            
+                            last_best_model = _best_model
+                            last_best_score = _best_score
+                            # last_best_param[k] = _best_params[k]
+                            last_best_param[item['key']] = _best_params[item['key']]
+                        
+                            if _diff <= lr:
+                                stop = True
+                                
+                        else:
+                            stop = True
+
+                # Trecho para iteraveis
+                # TODO melhorar essa parte deixando mais robusto
+                else:
+                    if verbose > 0:
+                        print(f'-------- {item["key"]} ----------')
+
+                    min_try = 5 # Quantidade minima de tentativas  antes de sair do loop
+                    value = item['init_val']
+                    step = item['def_step']
+                    maxVal = item['max']
+                    hist_value = [] #tuple com value e accuracy
+
+                    stop = False
+                    try_count = 1
+
+                    while stop == False:
+
+                        _grid_params =  {**{_k:np.array([_v]) for _k, _v in opt_params.items()}, item['key']:[value]}
+                        _grid = GridSearchCV(model, param_grid=_grid_params, cv=cv, n_jobs=-1, verbose=0)
+                        _grid.fit(x, y)
+                        
+                        _best_score = _grid.best_score_
+                        _best_params = _grid.best_params_
+                        _best_model = _grid.best_estimator_
+                        
+                        print("_best_score")
+                        print(_best_score)
+                        hist_value.append((value, _best_score))
+                        #  Show verbose if it is necessary
+                        if verbose > 0:
+                            
+                            print("-----------------")
+                            print("Value =====> ", value)
+                            print("opt params: ", _grid_params)
+                            print("Score: ", _best_score)
+                            print("Params: ", _best_params)
+                            print("Diff: ", (_best_score - last_best_score))
+                            print("-----------------")
+                            
+                            
+                        _diff = _best_score - last_best_score
+                        
+                        if last_best_score < _best_score:
+                            last_best_model = _best_model
+                            last_best_score = _best_score
+                            # last_best_param[k] = _best_params[k]
+                            last_best_param[item['key']] = _best_params[item['key']]
+                    
+                        if (_diff <= lr and try_count >= min_try) or (maxVal == value):
+                            stop = True
+                            print(hist_value)
+                            # maxValue = max(hist_value, key=lambda item:item[1])
+                        elif _diff >= lr and (min_try - try_count) < 2:
+                            print("reset")
+                            try_count = 0
+                            min_try = 3 #Zera o contador e deixa pelo menor 3 a mais para tentar
+
+                        try_count += 1
+                        value += step
+
+                
+                #Store best params and results
+
+                models = np.append(models, last_best_model)
+                opt_params = {**opt_params, **last_best_param}
+                scores = np.append(scores, last_best_score)
+                    
+        
+        results = {
+            'models' : models,
+            'best_params' : opt_params,
+            'scores' : scores
+            }
+
+        return results
+    
+    
+    
+    
+    
+    
+    
+    
+    
+    
+    
+    
+    
+    
+    
+    
+
```

### Comparing `krakatoa-0.0.5.post7/krakatoa/models/quick.py` & `krakatoa-0.0.5a1/krakatoa/models/quick.py`

 * *Ordering differences only*

 * *Files 23% similar despite different names*

```diff
@@ -1,290 +1,290 @@
-# -*- coding: utf-8 -*-
-
-'''
-Quick Models(:mod:`krakatoa.models.quick`)
-============================================================
-'''
-
-#============================================================
-# Imports
-#============================================================
-
-from sklearn.model_selection import cross_validate
-
-from ._getmodels import getModels
-from ._metrics import getScores
-import pandas as pd
-
-#============================================================
-# Regression Functions
-#============================================================
-
-class Regressor():
-    def __init__(self):
-
-        self._regression_scores = getScores('regression')
-
-    def _crossvalidate(self, estimator, x, y, scoring, cv=5):
-
-        result = cross_validate(estimator, x, y, scoring=scoring, cv=cv, n_jobs=-1)
-        
-        return result
-
-    def _runModels(self, models, x, y, scoring, cv):
-        results = {'estimator' : [], 'fit_time' : [], 'score_time' : []}
-        
-        for model in models:
-            res = self._crossvalidate(model['estimator'], x, y, scoring, cv)
-            
-            results['estimator'].append(model['name'])
-
-            for k, v in res.items():
-                if k not in results.keys():
-                    results[k] = []
-                    
-                results[k].append(v.mean())
-        
-        return results
-
-    def linearRegression(self, x, y, score=['r2'], cv=5, **kwargs):
-        '''
-        Quick linear regression models evaluation.
-
-        Parameters
-        ----------
-        x : DATAFRAME
-            Dataset Features.
-        y : NUMPY ARRAY
-            Target.
-        score : LIST, optional
-            Scoring metrics. The default is ['r2'].
-        cv : INT, optional
-            Number of kfolds. The default is 5.
-
-        Returns
-        -------
-        return : DATAFRAME
-            Returns dataframe with models and selected metrics score.
-
-        '''
-        
-        
-        models = getModels(mode='regression', modelClasses=['linear'])
-        
-        scoring = []
-        for s in score:
-            scoring.append(self._regression_scores[s]['name'])
-            # results['test_' + regression_scores[s]['name']]= []
-            
-        results = self._runModels(models, x, y, scoring, cv)
-        
-        return pd.DataFrame(results)
-
-    def treeRegression(self, x, y, score=['r2'], cv=5, **kwargs):
-        '''
-        Quick linear regression models evaluation.
-
-        Parameters
-        ----------
-        x : DATAFRAME
-            Dataset Features.
-        y : NUMPY ARRAY
-            Target.
-        score : LIST, optional
-            Scoring metrics. The default is ['r2'].
-        cv : INT, optional
-            Number of kfolds. The default is 5.
-
-        Returns
-        -------
-        return : DATAFRAME
-            Returns dataframe with models and selected metrics score.
-
-        '''
-        
-        models = getModels(mode='regression', modelClasses=['tree'])
-        
-        scoring = []
-        for s in score:
-            scoring.append(self._regression_scores[s]['name'])
-            # results['test_' + regression_scores[s]['name']]= []
-            
-        results = self._runModels(models, x, y, scoring, cv)
-        
-        return pd.DataFrame(results)
-
-    def boostRegression(self, x, y, score=['r2'], cv=5, **kwargs):
-        '''
-        Quick linear regression models evaluation.
-
-        Parameters
-        ----------
-        x : DATAFRAME
-            Dataset Features.
-        y : NUMPY ARRAY
-            Target.
-        score : LIST, optional
-            Scoring metrics. The default is ['r2'].
-        cv : INT, optional
-            Number of kfolds. The default is 5.
-
-        Returns
-        -------
-        return : DATAFRAME
-            Returns dataframe with models and selected metrics score.
-
-        '''
-
-        models = getModels(mode='regression', modelClasses=['boost'])
-        
-        scoring = []
-        for s in score:
-            scoring.append(self._regression_scores[s]['name'])
-            
-        results = self._runModels(models, x, y, scoring, cv)
-        
-        return pd.DataFrame(results)
-
-    def multiRegression(self, x, y, models = ['boost', 'linear', 'tree'], score=['r2'], cv=5):
-        
-        models = getModels(mode='regression', modelClasses=models)
-        
-        scoring = []
-        for s in score:
-            scoring.append(self._regression_scores[s]['name'])
-            
-        results = self._runModels(models, x, y, scoring, cv)
-        
-        return pd.DataFrame(results)
-    
-
-#============================================================
-# Classification Functions
-#============================================================
-
-
-class Classifier():
-
-    def __init__(self):
-
-        self._classification_scores = getScores('classification')
-
-    def _crossvalidate(self, estimator, x, y, scoring, cv=5):
-
-        result = cross_validate(estimator, x, y, scoring=scoring, cv=cv, n_jobs=-1)
-        
-        return result
-
-    def _runModels(self, models, x, y, scoring, cv):
-        results = {'estimator' : [], 'fit_time' : [], 'score_time' : []}
-        
-        for model in models:
-            res = self._crossvalidate(model['estimator'], x, y, scoring, cv)
-            
-            results['estimator'].append(model['name'])
-
-            for k, v in res.items():
-                if k not in results.keys():
-                    results[k] = []
-                    
-                results[k].append(v.mean())
-        
-        return results
-
-    def svmClassifier(self, x, y, score=['accuracy'], cv=5, **kwargs):
-        '''
-        Quick SVM classification models evaluation.
-
-        Parameters
-        ----------
-        x : DATAFRAME
-            Dataset Features.
-        y : NUMPY ARRAY
-            Target.
-        score : LIST, optional
-            Scoring metrics. The default is ['accuracy'].
-        cv : INT, optional
-            Number of kfolds. The default is 5.
-
-        Returns
-        -------
-        return : DATAFRAME
-            Returns dataframe with models and selected metrics score.
-
-        '''
-        
-        models = getModels(mode='classification', modelClasses=['svm'])
-        
-        scoring = []
-        for s in score:
-            scoring.append(self._classification_scores[s]['name'])
-            
-        results = self._runModels(models, x, y, scoring, cv)
-        
-        return pd.DataFrame(results)
-
-    def treeClassifier(self, x, y, score=['accuracy'], cv=5, **kwargs):
-        '''
-        Quick Tree classification models evaluation.
-
-        Parameters
-        ----------
-        x : DATAFRAME
-            Dataset Features.
-        y : NUMPY ARRAY
-            Target.
-        score : LIST, optional
-            Scoring metrics. The default is ['accuracy'].
-        cv : INT, optional
-            Number of kfolds. The default is 5.
-
-        Returns
-        -------
-        return : DATAFRAME
-            Returns dataframe with models and selected metrics score.
-
-        '''
-        
-        models = getModels(mode='classification', modelClasses=['tree'])
-        
-        scoring = []
-        for s in score:
-            scoring.append(self._classification_scores[s]['name'])
-            
-        results = self._runModels(models, x, y, scoring, cv)
-        
-        return pd.DataFrame(results)
-
-    def boostClassifier(self, x, y, score=['accuracy'], cv=5, **kwargs):
-        '''
-        Quick Boost classification models evaluation.
-
-        Parameters
-        ----------
-        x : DATAFRAME
-            Dataset Features.
-        y : NUMPY ARRAY
-            Target.
-        score : LIST, optional
-            Scoring metrics. The default is ['accuracy'].
-        cv : INT, optional
-            Number of kfolds. The default is 5.
-
-        Returns
-        -------
-        return : DATAFRAME
-            Returns dataframe with models and selected metrics score.
-
-        '''
-        
-        models = getModels(mode='classification', modelClasses=['boost'])
-        
-        scoring = []
-        for s in score:
-            scoring.append(self._classification_scores[s]['name'])
-            
-        results = self._runModels(models, x, y, scoring, cv)
-        
-        return pd.DataFrame(results)
-    
+# -*- coding: utf-8 -*-
+
+'''
+Quick Models(:mod:`krakatoa.models.quick`)
+============================================================
+'''
+
+#============================================================
+# Imports
+#============================================================
+
+from sklearn.model_selection import cross_validate
+
+from ._getmodels import getModels
+from ._metrics import getScores
+import pandas as pd
+
+#============================================================
+# Regression Functions
+#============================================================
+
+class Regressor():
+    def __init__(self):
+
+        self._regression_scores = getScores('regression')
+
+    def _crossvalidate(self, estimator, x, y, scoring, cv=5):
+
+        result = cross_validate(estimator, x, y, scoring=scoring, cv=cv, n_jobs=-1)
+        
+        return result
+
+    def _runModels(self, models, x, y, scoring, cv):
+        results = {'estimator' : [], 'fit_time' : [], 'score_time' : []}
+        
+        for model in models:
+            res = self._crossvalidate(model['estimator'], x, y, scoring, cv)
+            
+            results['estimator'].append(model['name'])
+
+            for k, v in res.items():
+                if k not in results.keys():
+                    results[k] = []
+                    
+                results[k].append(v.mean())
+        
+        return results
+
+    def linearRegression(self, x, y, score=['r2'], cv=5, **kwargs):
+        '''
+        Quick linear regression models evaluation.
+
+        Parameters
+        ----------
+        x : DATAFRAME
+            Dataset Features.
+        y : NUMPY ARRAY
+            Target.
+        score : LIST, optional
+            Scoring metrics. The default is ['r2'].
+        cv : INT, optional
+            Number of kfolds. The default is 5.
+
+        Returns
+        -------
+        return : DATAFRAME
+            Returns dataframe with models and selected metrics score.
+
+        '''
+        
+        
+        models = getModels(mode='regression', modelClasses=['linear'])
+        
+        scoring = []
+        for s in score:
+            scoring.append(self._regression_scores[s]['name'])
+            # results['test_' + regression_scores[s]['name']]= []
+            
+        results = self._runModels(models, x, y, scoring, cv)
+        
+        return pd.DataFrame(results)
+
+    def treeRegression(self, x, y, score=['r2'], cv=5, **kwargs):
+        '''
+        Quick linear regression models evaluation.
+
+        Parameters
+        ----------
+        x : DATAFRAME
+            Dataset Features.
+        y : NUMPY ARRAY
+            Target.
+        score : LIST, optional
+            Scoring metrics. The default is ['r2'].
+        cv : INT, optional
+            Number of kfolds. The default is 5.
+
+        Returns
+        -------
+        return : DATAFRAME
+            Returns dataframe with models and selected metrics score.
+
+        '''
+        
+        models = getModels(mode='regression', modelClasses=['tree'])
+        
+        scoring = []
+        for s in score:
+            scoring.append(self._regression_scores[s]['name'])
+            # results['test_' + regression_scores[s]['name']]= []
+            
+        results = self._runModels(models, x, y, scoring, cv)
+        
+        return pd.DataFrame(results)
+
+    def boostRegression(self, x, y, score=['r2'], cv=5, **kwargs):
+        '''
+        Quick linear regression models evaluation.
+
+        Parameters
+        ----------
+        x : DATAFRAME
+            Dataset Features.
+        y : NUMPY ARRAY
+            Target.
+        score : LIST, optional
+            Scoring metrics. The default is ['r2'].
+        cv : INT, optional
+            Number of kfolds. The default is 5.
+
+        Returns
+        -------
+        return : DATAFRAME
+            Returns dataframe with models and selected metrics score.
+
+        '''
+
+        models = getModels(mode='regression', modelClasses=['boost'])
+        
+        scoring = []
+        for s in score:
+            scoring.append(self._regression_scores[s]['name'])
+            
+        results = self._runModels(models, x, y, scoring, cv)
+        
+        return pd.DataFrame(results)
+
+    def multiRegression(self, x, y, models = ['boost', 'linear', 'tree'], score=['r2'], cv=5):
+        
+        models = getModels(mode='regression', modelClasses=models)
+        
+        scoring = []
+        for s in score:
+            scoring.append(self._regression_scores[s]['name'])
+            
+        results = self._runModels(models, x, y, scoring, cv)
+        
+        return pd.DataFrame(results)
+    
+
+#============================================================
+# Classification Functions
+#============================================================
+
+
+class Classifier():
+
+    def __init__(self):
+
+        self._classification_scores = getScores('classification')
+
+    def _crossvalidate(self, estimator, x, y, scoring, cv=5):
+
+        result = cross_validate(estimator, x, y, scoring=scoring, cv=cv, n_jobs=-1)
+        
+        return result
+
+    def _runModels(self, models, x, y, scoring, cv):
+        results = {'estimator' : [], 'fit_time' : [], 'score_time' : []}
+        
+        for model in models:
+            res = self._crossvalidate(model['estimator'], x, y, scoring, cv)
+            
+            results['estimator'].append(model['name'])
+
+            for k, v in res.items():
+                if k not in results.keys():
+                    results[k] = []
+                    
+                results[k].append(v.mean())
+        
+        return results
+
+    def svmClassifier(self, x, y, score=['accuracy'], cv=5, **kwargs):
+        '''
+        Quick SVM classification models evaluation.
+
+        Parameters
+        ----------
+        x : DATAFRAME
+            Dataset Features.
+        y : NUMPY ARRAY
+            Target.
+        score : LIST, optional
+            Scoring metrics. The default is ['accuracy'].
+        cv : INT, optional
+            Number of kfolds. The default is 5.
+
+        Returns
+        -------
+        return : DATAFRAME
+            Returns dataframe with models and selected metrics score.
+
+        '''
+        
+        models = getModels(mode='classification', modelClasses=['svm'])
+        
+        scoring = []
+        for s in score:
+            scoring.append(self._classification_scores[s]['name'])
+            
+        results = self._runModels(models, x, y, scoring, cv)
+        
+        return pd.DataFrame(results)
+
+    def treeClassifier(self, x, y, score=['accuracy'], cv=5, **kwargs):
+        '''
+        Quick Tree classification models evaluation.
+
+        Parameters
+        ----------
+        x : DATAFRAME
+            Dataset Features.
+        y : NUMPY ARRAY
+            Target.
+        score : LIST, optional
+            Scoring metrics. The default is ['accuracy'].
+        cv : INT, optional
+            Number of kfolds. The default is 5.
+
+        Returns
+        -------
+        return : DATAFRAME
+            Returns dataframe with models and selected metrics score.
+
+        '''
+        
+        models = getModels(mode='classification', modelClasses=['tree'])
+        
+        scoring = []
+        for s in score:
+            scoring.append(self._classification_scores[s]['name'])
+            
+        results = self._runModels(models, x, y, scoring, cv)
+        
+        return pd.DataFrame(results)
+
+    def boostClassifier(self, x, y, score=['accuracy'], cv=5, **kwargs):
+        '''
+        Quick Boost classification models evaluation.
+
+        Parameters
+        ----------
+        x : DATAFRAME
+            Dataset Features.
+        y : NUMPY ARRAY
+            Target.
+        score : LIST, optional
+            Scoring metrics. The default is ['accuracy'].
+        cv : INT, optional
+            Number of kfolds. The default is 5.
+
+        Returns
+        -------
+        return : DATAFRAME
+            Returns dataframe with models and selected metrics score.
+
+        '''
+        
+        models = getModels(mode='classification', modelClasses=['boost'])
+        
+        scoring = []
+        for s in score:
+            scoring.append(self._classification_scores[s]['name'])
+            
+        results = self._runModels(models, x, y, scoring, cv)
+        
+        return pd.DataFrame(results)
+
```

### Comparing `krakatoa-0.0.5.post7/setup.py` & `krakatoa-0.0.5a1/setup.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,32 +1,29 @@
-from setuptools import setup
-
-setup(
-  name = 'krakatoa',       
-  packages = ['krakatoa', 'krakatoa/models', 'krakatoa/future'],  
-  version = '0.0.5post7',      
-  license='MIT',        
-  description = 'Machine Learning high level package.',  
-  long_description='Machine Learning high level package.',  
-  author = 'Matheus de Prá Andrade',              
-  author_email = 'mpandrade@ucs.br',    
-  url = 'https://github.com/aitec-mp/krakatoa',  
-  download_url = 'https://github.com/aitec-mp/krakatoa/archive/refs/tags/0.0.5post7.tar.gz',    
-  keywords = ['krakatoa', 'machine learning'],  
-  install_requires=[    
-          'scikit-learn',
-          'numpy',
-          'pandas',
-          'xgboost'
-      ],
-  classifiers=[
-    'Development Status :: 3 - Alpha',     
-    'Intended Audience :: Developers',  
-    'Topic :: Software Development :: Build Tools',
-    'License :: OSI Approved :: MIT License',   
-    'Programming Language :: Python :: 3.7',
-    'Programming Language :: Python :: 3.8',
-    'Programming Language :: Python :: 3.9',
-    'Programming Language :: Python :: 3.10',
-    'Programming Language :: Python :: 3.11',
-  ],
-)
+from setuptools import setup
+
+setup(
+  name = 'krakatoa',       
+  packages = ['krakatoa', 'krakatoa/models', 'krakatoa/future'],  
+  version = '0.0.5a1',      
+  license='MIT',        
+  description = 'Machine Learning high level package.',  
+  author = 'Matheus de Prá Andrade',              
+  author_email = 'mpandrade@ucs.br',    
+  url = 'https://github.com/aitec-mp/krakatoa',  
+  download_url = 'https://github.com/aitec-mp/krakatoa/archive/refs/tags/0.0.5.tar.gz',    
+  keywords = ['krakatoa', 'machine learning'],  
+  install_requires=[    
+          'sklearn',
+          'numpy',
+          'pandas',
+          'xgboost'
+      ],
+  classifiers=[
+    'Development Status :: 3 - Alpha',     
+    'Intended Audience :: Developers',  
+    'Topic :: Software Development :: Build Tools',
+    'License :: OSI Approved :: MIT License',   
+    'Programming Language :: Python :: 3.7',
+    'Programming Language :: Python :: 3.8',
+    'Programming Language :: Python :: 3.9',
+  ],
+)
```

