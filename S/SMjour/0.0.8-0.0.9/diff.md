# Comparing `tmp/SMjour-0.0.8.tar.gz` & `tmp/SMjour-0.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "SMjour-0.0.8.tar", last modified: Mon Jun 26 15:28:55 2023, max compression
+gzip compressed data, was "SMjour-0.0.9.tar", last modified: Mon Jun 26 16:31:04 2023, max compression
```

## Comparing `SMjour-0.0.8.tar` & `SMjour-0.0.9.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxrwxrwx   0        0        0        0 2023-06-26 15:28:55.296000 SMjour-0.0.8/
--rw-rw-rw-   0        0        0     1097 2023-06-12 13:17:40.000000 SMjour-0.0.8/LICENSE
--rw-rw-rw-   0        0        0      448 2023-06-26 15:28:55.283000 SMjour-0.0.8/PKG-INFO
--rw-rw-rw-   0        0        0        0 2023-06-12 13:07:00.000000 SMjour-0.0.8/README.md
-drwxrwxrwx   0        0        0        0 2023-06-26 15:28:55.179000 SMjour-0.0.8/SMjour/
--rw-rw-rw-   0        0        0     6549 2023-06-12 19:29:11.000000 SMjour-0.0.8/SMjour/SMjour.py
--rw-rw-rw-   0        0        0       21 2023-06-26 15:28:26.000000 SMjour-0.0.8/SMjour/__init__.py
-drwxrwxrwx   0        0        0        0 2023-06-26 15:28:55.273000 SMjour-0.0.8/SMjour.egg-info/
--rw-rw-rw-   0        0        0      448 2023-06-26 15:28:55.000000 SMjour-0.0.8/SMjour.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      227 2023-06-26 15:28:55.000000 SMjour-0.0.8/SMjour.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-26 15:28:55.000000 SMjour-0.0.8/SMjour.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       88 2023-06-26 15:28:55.000000 SMjour-0.0.8/SMjour.egg-info/requires.txt
--rw-rw-rw-   0        0        0        7 2023-06-26 15:28:55.000000 SMjour-0.0.8/SMjour.egg-info/top_level.txt
--rw-rw-rw-   0        0        0      114 2023-06-12 14:12:44.000000 SMjour-0.0.8/pyproject.toml
--rw-rw-rw-   0        0        0      660 2023-06-26 15:28:55.294000 SMjour-0.0.8/setup.cfg
+drwxrwxrwx   0        0        0        0 2023-06-26 16:31:04.540000 SMjour-0.0.9/
+-rw-rw-rw-   0        0        0     1097 2023-06-12 13:17:40.000000 SMjour-0.0.9/LICENSE
+-rw-rw-rw-   0        0        0      448 2023-06-26 16:31:04.528000 SMjour-0.0.9/PKG-INFO
+-rw-rw-rw-   0        0        0        0 2023-06-12 13:07:00.000000 SMjour-0.0.9/README.md
+drwxrwxrwx   0        0        0        0 2023-06-26 16:31:04.428000 SMjour-0.0.9/SMjour/
+-rw-rw-rw-   0        0        0     8779 2023-06-26 16:26:12.000000 SMjour-0.0.9/SMjour/SMjour.py
+-rw-rw-rw-   0        0        0       21 2023-06-26 15:28:26.000000 SMjour-0.0.9/SMjour/__init__.py
+drwxrwxrwx   0        0        0        0 2023-06-26 16:31:04.514000 SMjour-0.0.9/SMjour.egg-info/
+-rw-rw-rw-   0        0        0      448 2023-06-26 16:31:04.000000 SMjour-0.0.9/SMjour.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      227 2023-06-26 16:31:04.000000 SMjour-0.0.9/SMjour.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-26 16:31:04.000000 SMjour-0.0.9/SMjour.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       88 2023-06-26 16:31:04.000000 SMjour-0.0.9/SMjour.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        7 2023-06-26 16:31:04.000000 SMjour-0.0.9/SMjour.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0      114 2023-06-12 14:12:44.000000 SMjour-0.0.9/pyproject.toml
+-rw-rw-rw-   0        0        0      660 2023-06-26 16:31:04.538000 SMjour-0.0.9/setup.cfg
```

### Comparing `SMjour-0.0.8/LICENSE` & `SMjour-0.0.9/LICENSE`

 * *Files identical despite different names*

### Comparing `SMjour-0.0.8/SMjour/SMjour.py` & `SMjour-0.0.9/SMjour/SMjour.py`

 * *Files 24% similar despite different names*

```diff
@@ -8,14 +8,16 @@
 from sklearn.linear_model import LinearRegression
 from sklearn.metrics import r2_score
 import matplotlib.pyplot as plt
 import numpy as np
 import seaborn as sns
 import plotly.express as px
 from google.colab import drive
+from tqdm import tqdm
+from IPython.display import display
 
 
 def input_path(message=""):
   raw_s=input(message)
   raw_s=raw_s.replace(r'"','')
   return "/content/drive/Shareddrives/"+'/'.join(raw_s.split("\\")[2:])
    
@@ -48,15 +50,16 @@
     #import drive
     drive.mount("/content/drive")
     newpath=input_path('Input path:')
     if (newpath.split("/")[-1].split(".")[-1] == "xlsx") or (newpath.split("/")[-1].split(".")[-1] == "xls"):
         df=pd.read_excel(newpath)
     elif (newpath.split("/")[-1].split(".")[-1] == "csv"):
         if option=='default':
-          df=pd.read_csv(newpath)
+          df=pd.read_csv(newpath).reset_index()
+          df=df.T.reset_index().T
         elif option == 1:
           with open(newpath, "r", newline="") as fp:
             # you can use verbose=True to see what CleverCSV does
             dialect = clevercsv.Sniffer().sniff(fp.read(), verbose=False)
             fp.seek(0)
             reader = clevercsv.reader(fp, dialect)
             rows = list(reader)
@@ -132,18 +135,98 @@
 
     #hago la regresion
     reg = LinearRegression().fit(pre_X, pre_y)   #############OJOTA ,weight
     #reg = LinearRegression().fit(pre_X, pre_y)
     result[i]=1/(1-r2_score(pre_y, reg.predict(pre_X)) )
     result[i]=1/(1-adjRsquare(pre_y, reg.predict(pre_X),vars) )
   return result
-def collinearity_test(df,tounderstand=None):
+
+#viffs
+def getIndexOfCol3(var,allVIFs):
+  counter=0
+  index=[]
+  for j in allVIFs: 
+    if var in j.keys():
+      index.append(counter)
+    counter+=1
+  return index
+def getFullCombination(boolArray,colls):
+  counter=0
+  final=[]
+  for j in boolArray:
+    if j==1:
+      final.append(colls[counter])
+    counter+=1
+  return final
+def vif_distance(tounderstand,stochQ=1000):
+  #'searchcont
+  X_rand=np.random.randint(2, size=[stochQ,len(tounderstand)])
+  X_rand=X_rand[np.where(X_rand.sum(axis=1)>=2)]
+  allVIFs=[]
+
+  for i in tqdm(X_rand):
+    # print(i)
+    randomX_cols=getFullCombination(i,tounderstand)
+    allVIFs.append(getVIFs(randomX_cols))
+
+  for i in allVIFs:
+    for j in i.keys():
+      if i[j]>3000:
+        i[j]=3000
+  
+  interest=tounderstand
+
+  impacten=tounderstand
+
+  fullTest=tounderstand
+  matoPato=[]
+  for k in fullTest:
+    var=k#x_cols[ind]
+    metaY=np.array([allVIFs[i][var] for i in getIndexOfCol3(var,allVIFs)])
+    metaX=X_rand[getIndexOfCol3(var,allVIFs)]
+    metaReg = LinearRegression(fit_intercept=False).fit(metaX, metaY)
+    # meta_betas
+    normed_coef=(metaReg.coef_-metaReg.coef_.mean())/metaReg.coef_.std()
+    normed_coef=metaReg.coef_
+    matoPato.append(list(normed_coef))
+  duff=pd.DataFrame(np.array(matoPato).transpose())
+  duff.columns=fullTest
+  duff.index=impacten
+
+  duff.values[[np.arange(duff.shape[0])]*2] = 0
+
+  to_test=interest
+
+  to_test_index=impacten
+
+  filtered_duff=duff.loc[to_test_index,to_test]
+  simil=np.minimum(filtered_duff.to_numpy(),filtered_duff.to_numpy().T)
+
+  simil[simil < 0] = 0
+  disimil=1/simil
+  disimil[disimil > 200] = 200
+  disimil=np.log(disimil+1)
+  n = disimil.shape[0]
+  disimil[range(n), range(n)] = 0
+  disimil=disimil/np.max(disimil)
+
+  simil=1-disimil
+  similitude=pd.DataFrame(simil)
+  similitude.columns =tounderstand
+  similitude.index=tounderstand
+  return similitude
+
+
+
+def collinearity_test(df,tounderstand=None,distance="vif"):
   tounderstand=tounderstand if tounderstand else df.columns[2:] 
   to_test=tounderstand
+  print("Coll before")
   display(getVIFs(tounderstand,df))
+  print("Coll after")
   # set figure size
   correlation=df[to_test].corr().fillna(0)
   filter=0
   corr_numpy=correlation.to_numpy()
   indices=corr_numpy.argsort()[:,-2]
   corr_numpy
   finalIndices=[]
@@ -163,19 +246,23 @@
   sns.heatmap(finalCorr, annot=True, mask=mask, vmin=-1, vmax=1,cmap="rocket_r")
   plt.title('Correlation Coefficient Of Predictors')
   plt.show()
 
 
   
   data=df[to_test]
+
+  #block distance
   #correlations
   correlations=df[to_test].corr().fillna(0)
-  similarity=abs(correlations)
-
-  similarity
+  if distance=="corr":
+    
+    similarity=abs(correlations)
+  elif distance=="vif":
+    similarity=vif_distance(tounderstand,stochQ=1000)
   
 
   plt.figure(figsize=(12,5))
   dissimilarity = 1 - similarity
   Z = linkage(squareform(dissimilarity), 'complete')
 
   dendrogram(Z, labels=to_test, orientation='top',
```

### Comparing `SMjour-0.0.8/setup.cfg` & `SMjour-0.0.9/setup.cfg`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 00000000: 5b6d 6574 6164 6174 615d 0d0a 6e61 6d65  [metadata]..name
 00000010: 203d 2053 4d6a 6f75 720d 0a76 6572 7369   = SMjour..versi
-00000020: 6f6e 203d 2030 2e30 2e38 0d0a 6175 7468  on = 0.0.8..auth
+00000020: 6f6e 203d 2030 2e30 2e39 0d0a 6175 7468  on = 0.0.9..auth
 00000030: 6f72 203d 2041 6775 7374 696e 2042 7573  or = Agustin Bus
 00000040: 746f 7320 4261 7274 6f6e 0d0a 6175 7468  tos Barton..auth
 00000050: 6f72 5f65 6d61 696c 203d 2061 6775 7374  or_email = agust
 00000060: 696e 6275 7374 6f73 6261 7274 6f6e 4067  inbustosbarton@g
 00000070: 6d61 696c 2e63 6f6d 0d0a 6465 7363 7269  mail.com..descri
 00000080: 7074 696f 6e20 3d20 696e 7665 7374 6967  ption = investig
 00000090: 6174 696f 6e20 6a6f 7572 6e61 6c0d 0a6c  ation journal..l
```

