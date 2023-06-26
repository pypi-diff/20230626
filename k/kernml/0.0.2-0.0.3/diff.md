# Comparing `tmp/kernml-0.0.2.tar.gz` & `tmp/kernml-0.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "kernml-0.0.2.tar", last modified: Fri Jun 23 05:17:04 2023, max compression
+gzip compressed data, was "kernml-0.0.3.tar", last modified: Mon Jun 26 07:51:35 2023, max compression
```

## Comparing `kernml-0.0.2.tar` & `kernml-0.0.3.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxrwxrwx   0        0        0        0 2023-06-23 05:17:04.996840 kernml-0.0.2/
--rw-rw-rw-   0        0        0     1091 2023-06-23 01:54:01.000000 kernml-0.0.2/LICENSE
--rw-rw-rw-   0        0        0      417 2023-06-23 05:17:04.992850 kernml-0.0.2/PKG-INFO
--rw-rw-rw-   0        0        0       48 2023-06-23 01:52:37.000000 kernml-0.0.2/README.md
--rw-rw-rw-   0        0        0      447 2023-06-23 05:16:46.000000 kernml-0.0.2/pyproject.toml
--rw-rw-rw-   0        0        0       42 2023-06-23 05:17:04.996840 kernml-0.0.2/setup.cfg
-drwxrwxrwx   0        0        0        0 2023-06-23 05:17:04.960886 kernml-0.0.2/src/
-drwxrwxrwx   0        0        0        0 2023-06-23 05:17:04.976880 kernml-0.0.2/src/kernml/
--rw-rw-rw-   0        0        0        0 2023-06-23 05:13:51.000000 kernml-0.0.2/src/kernml/__init__.py
--rw-rw-rw-   0        0        0    23898 2023-06-23 04:35:07.000000 kernml-0.0.2/src/kernml/prg.py
-drwxrwxrwx   0        0        0        0 2023-06-23 05:17:04.988868 kernml-0.0.2/src/kernml.egg-info/
--rw-rw-rw-   0        0        0      417 2023-06-23 05:17:04.000000 kernml-0.0.2/src/kernml.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      209 2023-06-23 05:17:04.000000 kernml-0.0.2/src/kernml.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-23 05:17:04.000000 kernml-0.0.2/src/kernml.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        7 2023-06-23 05:17:04.000000 kernml-0.0.2/src/kernml.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-06-26 07:51:35.826195 kernml-0.0.3/
+-rw-rw-rw-   0        0        0     1091 2023-06-23 01:54:01.000000 kernml-0.0.3/LICENSE
+-rw-rw-rw-   0        0        0      417 2023-06-26 07:51:35.825238 kernml-0.0.3/PKG-INFO
+-rw-rw-rw-   0        0        0       48 2023-06-23 01:52:37.000000 kernml-0.0.3/README.md
+-rw-rw-rw-   0        0        0      447 2023-06-26 07:38:49.000000 kernml-0.0.3/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2023-06-26 07:51:35.826195 kernml-0.0.3/setup.cfg
+drwxrwxrwx   0        0        0        0 2023-06-26 07:51:35.803256 kernml-0.0.3/src/
+drwxrwxrwx   0        0        0        0 2023-06-26 07:51:35.815225 kernml-0.0.3/src/kernml/
+-rw-rw-rw-   0        0        0        0 2023-06-23 05:13:51.000000 kernml-0.0.3/src/kernml/__init__.py
+-rw-rw-rw-   0        0        0    26033 2023-06-26 07:51:11.000000 kernml-0.0.3/src/kernml/prg.py
+drwxrwxrwx   0        0        0        0 2023-06-26 07:51:35.823202 kernml-0.0.3/src/kernml.egg-info/
+-rw-rw-rw-   0        0        0      417 2023-06-26 07:51:35.000000 kernml-0.0.3/src/kernml.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      209 2023-06-26 07:51:35.000000 kernml-0.0.3/src/kernml.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-26 07:51:35.000000 kernml-0.0.3/src/kernml.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        7 2023-06-26 07:51:35.000000 kernml-0.0.3/src/kernml.egg-info/top_level.txt
```

### Comparing `kernml-0.0.2/LICENSE` & `kernml-0.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `kernml-0.0.2/src/kernml/prg.py` & `kernml-0.0.3/src/kernml/prg.py`

 * *Files 4% similar despite different names*

```diff
@@ -834,15 +834,99 @@
 plt.ylabel("Predicted Category")
 plt.show() 
 '''
     p7 = print(p7)
     return p7
 
 def pr_8():
-    p8 = ''''''
+    p8 = '''
+import pandas as pd
+from pgmpy.models import BayesianNetwork
+from pgmpy.estimators import MaximumLikelihoodEstimator
+from pgmpy.inference import VariableElimination
+
+with open("./../Data/heart_disease/processed.cleveland.attributes", "r", newline=None) as f:
+    attributes = f.readline().replace('\n', '').split(',')
+print(attributes)
+
+data = pd.read_csv("./../Data/heart_disease/processed.cleveland.data", header=None, names=attributes)
+display(data)
+
+display(data.info())
+
+print(data.ca.value_counts())
+print(data.thal.value_counts())
+
+data = data[data.ca != '?']
+data = data[data.thal != '?']
+
+data = data.convert_dtypes()
+print(data.dtypes)
+
+data.ca = pd.to_numeric(data['ca']).astype(int)
+data.thal = pd.to_numeric(data['thal']).astype(int)
+
+print(data.dtypes)
+
+display(data)
+
+model = BayesianNetwork([
+    ('age', 'heartdisease'), 
+    ('sex', 'heartdisease'),
+    ('cp','heartdisease'), 
+    ('exang','heartdisease'),
+    ('heartdisease','restecg'),
+    ('heartdisease','chol')
+])
+
+model.fit(data, estimator=MaximumLikelihoodEstimator)
+
+inference = VariableElimination(model)
+
+print(inference.query(variables=['heartdisease'], evidence={'restecg': 1}))
+
+print(inference.query(variables=['heartdisease'],evidence={'cp':2}))
+    '''
     p8 = print(p8)
     return p8
 
 def pr_9():
-    p9 = ''''''
+    p9 = '''
+import numpy as np
+from sklearn.datasets import load_iris
+from sklearn.mixture import GaussianMixture
+import matplotlib.pyplot as plt
+
+iris = load_iris()
+
+print(iris.keys())
+
+print(iris.data.shape)
+
+print(iris.feature_names)
+
+print(iris.target_names)
+
+X = iris.data[:, 2:]
+
+colormap = np.array(['blue', 'orange', 'green'])
+
+plt.scatter(X[:,0], X[:,1], c=colormap[iris.target])
+plt.xlabel("Petal length (cm)")
+plt.ylabel("Petal width (cm)")
+plt.title("Actual Clusters")
+plt.show()
+
+model = GaussianMixture(n_components = 3, random_state=42)
+
+model.fit(X)
+
+predicted_labels = model.predict(X)
+
+colormap_prediction = np.array(['purple', 'cyan', 'red'])
+markers = ['o', 'v', 's']
+for i, l in enumerate(predicted_labels):
+    plt.plot(X[i,0], X[i,1], color=colormap_prediction[l], marker=markers[l])    
+plt.show()
+    '''
     p9 = print(p9)
     return p9
```

