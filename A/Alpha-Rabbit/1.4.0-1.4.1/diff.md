# Comparing `tmp/Alpha_Rabbit-1.4.0.tar.gz` & `tmp/Alpha_Rabbit-1.4.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "Alpha_Rabbit-1.4.0.tar", last modified: Wed Jun 21 08:10:38 2023, max compression
+gzip compressed data, was "Alpha_Rabbit-1.4.1.tar", last modified: Mon Jun 26 07:41:43 2023, max compression
```

## Comparing `Alpha_Rabbit-1.4.0.tar` & `Alpha_Rabbit-1.4.1.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxrwxrwx   0        0        0        0 2023-06-21 08:10:38.773165 Alpha_Rabbit-1.4.0/
-drwxrwxrwx   0        0        0        0 2023-06-21 08:10:38.767180 Alpha_Rabbit-1.4.0/Alpha_Rabbit/
--rw-rw-rw-   0        0        0    42049 2023-06-21 05:09:58.000000 Alpha_Rabbit-1.4.0/Alpha_Rabbit/Alpha_Rabbit.py
--rw-rw-rw-   0        0        0    13938 2023-03-24 06:59:51.000000 Alpha_Rabbit-1.4.0/Alpha_Rabbit/Factor_Calculator.py
--rw-rw-rw-   0        0        0    22658 2023-06-05 07:41:31.000000 Alpha_Rabbit-1.4.0/Alpha_Rabbit/Factor_Def_and_Get_Method.py
--rw-rw-rw-   0        0        0        0 2023-02-27 02:16:19.000000 Alpha_Rabbit-1.4.0/Alpha_Rabbit/__init__.py
--rw-rw-rw-   0        0        0     1522 2023-02-27 02:16:19.000000 Alpha_Rabbit-1.4.0/Alpha_Rabbit/trade_strategy.py
-drwxrwxrwx   0        0        0        0 2023-06-21 08:10:38.772167 Alpha_Rabbit-1.4.0/Alpha_Rabbit.egg-info/
--rw-rw-rw-   0        0        0      787 2023-06-21 08:10:38.000000 Alpha_Rabbit-1.4.0/Alpha_Rabbit.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      411 2023-06-21 08:10:38.000000 Alpha_Rabbit-1.4.0/Alpha_Rabbit.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-21 08:10:38.000000 Alpha_Rabbit-1.4.0/Alpha_Rabbit.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       48 2023-06-21 08:10:38.000000 Alpha_Rabbit-1.4.0/Alpha_Rabbit.egg-info/requires.txt
--rw-rw-rw-   0        0        0       13 2023-06-21 08:10:38.000000 Alpha_Rabbit-1.4.0/Alpha_Rabbit.egg-info/top_level.txt
--rw-rw-rw-   0        0        0        2 2023-02-27 02:16:19.000000 Alpha_Rabbit-1.4.0/Alpha_Rabbit.egg-info/zip-safe
--rw-rw-rw-   0        0        0     1094 2023-02-27 02:16:19.000000 Alpha_Rabbit-1.4.0/LICENSE.txt
--rw-rw-rw-   0        0        0      787 2023-06-21 08:10:38.773165 Alpha_Rabbit-1.4.0/PKG-INFO
--rw-rw-rw-   0        0        0       69 2023-02-27 02:16:19.000000 Alpha_Rabbit-1.4.0/README.md
--rw-rw-rw-   0        0        0       85 2023-06-21 08:10:38.774162 Alpha_Rabbit-1.4.0/setup.cfg
--rw-rw-rw-   0        0        0     1229 2023-06-21 08:10:20.000000 Alpha_Rabbit-1.4.0/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-26 07:41:43.278396 Alpha_Rabbit-1.4.1/
+drwxrwxrwx   0        0        0        0 2023-06-26 07:41:43.270585 Alpha_Rabbit-1.4.1/Alpha_Rabbit/
+-rw-rw-rw-   0        0        0    42068 2023-06-26 07:40:53.000000 Alpha_Rabbit-1.4.1/Alpha_Rabbit/Alpha_Rabbit.py
+-rw-rw-rw-   0        0        0    13938 2023-03-24 06:59:51.000000 Alpha_Rabbit-1.4.1/Alpha_Rabbit/Factor_Calculator.py
+-rw-rw-rw-   0        0        0    22658 2023-06-05 07:41:31.000000 Alpha_Rabbit-1.4.1/Alpha_Rabbit/Factor_Def_and_Get_Method.py
+-rw-rw-rw-   0        0        0        0 2023-02-27 02:16:19.000000 Alpha_Rabbit-1.4.1/Alpha_Rabbit/__init__.py
+-rw-rw-rw-   0        0        0     1522 2023-02-27 02:16:19.000000 Alpha_Rabbit-1.4.1/Alpha_Rabbit/trade_strategy.py
+drwxrwxrwx   0        0        0        0 2023-06-26 07:41:43.277398 Alpha_Rabbit-1.4.1/Alpha_Rabbit.egg-info/
+-rw-rw-rw-   0        0        0      787 2023-06-26 07:41:43.000000 Alpha_Rabbit-1.4.1/Alpha_Rabbit.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      411 2023-06-26 07:41:43.000000 Alpha_Rabbit-1.4.1/Alpha_Rabbit.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-26 07:41:43.000000 Alpha_Rabbit-1.4.1/Alpha_Rabbit.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       48 2023-06-26 07:41:43.000000 Alpha_Rabbit-1.4.1/Alpha_Rabbit.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       13 2023-06-26 07:41:43.000000 Alpha_Rabbit-1.4.1/Alpha_Rabbit.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0        2 2023-02-27 02:16:19.000000 Alpha_Rabbit-1.4.1/Alpha_Rabbit.egg-info/zip-safe
+-rw-rw-rw-   0        0        0     1094 2023-02-27 02:16:19.000000 Alpha_Rabbit-1.4.1/LICENSE.txt
+-rw-rw-rw-   0        0        0      787 2023-06-26 07:41:43.278396 Alpha_Rabbit-1.4.1/PKG-INFO
+-rw-rw-rw-   0        0        0       69 2023-02-27 02:16:19.000000 Alpha_Rabbit-1.4.1/README.md
+-rw-rw-rw-   0        0        0       85 2023-06-26 07:41:43.279388 Alpha_Rabbit-1.4.1/setup.cfg
+-rw-rw-rw-   0        0        0     1229 2023-06-26 07:41:17.000000 Alpha_Rabbit-1.4.1/setup.py
```

### Comparing `Alpha_Rabbit-1.4.0/Alpha_Rabbit/Alpha_Rabbit.py` & `Alpha_Rabbit-1.4.1/Alpha_Rabbit/Alpha_Rabbit.py`

 * *Files 1% similar despite different names*

```diff
@@ -406,15 +406,15 @@
                 temp1[i] = self.mat_ranknormlize(temp1[i])
                 continue
             fclist = list(filter(lambda x: x!=i,list(temp1)[:no]))
             temp1[i] = self.orthog(temp1,i,fclist)[0]
         return temp1
     
     def ts_mat_orthog(self,factor_mat):
-        return factor_mat.groupby(level = 'date').apply(self.mat_orthog)
+        return factor_mat.groupby(level = 'date',group_keys = False).apply(self.mat_orthog)
     
     def mat_normlize(self,factor_mat):
         df = factor_mat.rename_axis(['date','symbol'])
         def norm(x):
             return (x - x.min())/(x.max()-x.min())
         return df.groupby(level = 'date',group_keys = False).apply(norm)
```

### Comparing `Alpha_Rabbit-1.4.0/Alpha_Rabbit/Factor_Calculator.py` & `Alpha_Rabbit-1.4.1/Alpha_Rabbit/Factor_Calculator.py`

 * *Files identical despite different names*

### Comparing `Alpha_Rabbit-1.4.0/Alpha_Rabbit/Factor_Def_and_Get_Method.py` & `Alpha_Rabbit-1.4.1/Alpha_Rabbit/Factor_Def_and_Get_Method.py`

 * *Files identical despite different names*

### Comparing `Alpha_Rabbit-1.4.0/Alpha_Rabbit/trade_strategy.py` & `Alpha_Rabbit-1.4.1/Alpha_Rabbit/trade_strategy.py`

 * *Files identical despite different names*

### Comparing `Alpha_Rabbit-1.4.0/Alpha_Rabbit.egg-info/PKG-INFO` & `Alpha_Rabbit-1.4.1/Alpha_Rabbit.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: Alpha-Rabbit
-Version: 1.4.0
+Version: 1.4.1
 Summary: Alpha_Rabbit
 Home-page: UNKNOWN
 Author: lijiongting
 Author-email: 448986334@qq.com
 License: MIT
 Platform: UNKNOWN
 Classifier: Intended Audience :: Developers
```

### Comparing `Alpha_Rabbit-1.4.0/LICENSE.txt` & `Alpha_Rabbit-1.4.1/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `Alpha_Rabbit-1.4.0/PKG-INFO` & `Alpha_Rabbit-1.4.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: Alpha_Rabbit
-Version: 1.4.0
+Version: 1.4.1
 Summary: Alpha_Rabbit
 Home-page: UNKNOWN
 Author: lijiongting
 Author-email: 448986334@qq.com
 License: MIT
 Platform: UNKNOWN
 Classifier: Intended Audience :: Developers
```

### Comparing `Alpha_Rabbit-1.4.0/setup.py` & `Alpha_Rabbit-1.4.1/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -9,15 +9,15 @@
 from setuptools import setup, find_packages
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 setup(
     name="Alpha_Rabbit",
-    version="1.4.0",
+    version="1.4.1",
     author="lijiongting",
     author_email="448986334@qq.com",
     description="Alpha_Rabbit",
     long_description=long_description,
     long_description_content_type="text/markdown",
     license="MIT",
     url="",
```

