# Comparing `tmp/iterative_stats-0.0.6.tar.gz` & `tmp/iterative_stats-0.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "iterative_stats-0.0.6.tar", max compression
+gzip compressed data, was "iterative_stats-0.1.0.tar", max compression
```

## Comparing `iterative_stats-0.0.6.tar` & `iterative_stats-0.1.0.tar`

### file list

```diff
@@ -1,20 +1,21 @@
--rw-r--r--   0        0        0     1549 2023-06-26 12:42:26.773409 iterative_stats-0.0.6/LICENSE
--rw-r--r--   0        0        0     7818 2023-06-26 12:42:26.773409 iterative_stats-0.0.6/README.md
--rw-r--r--   0        0        0     1357 2023-06-26 12:42:26.773409 iterative_stats-0.0.6/iterative_stats/abstract_iterative_statistics.py
--rw-r--r--   0        0        0     2038 2023-06-26 12:42:26.773409 iterative_stats-0.0.6/iterative_stats/iterative_covariance.py
--rw-r--r--   0        0        0     4374 2023-06-26 12:42:26.773409 iterative_stats-0.0.6/iterative_stats/iterative_dotproduct.py
--rw-r--r--   0        0        0     1055 2023-06-26 12:42:26.773409 iterative_stats-0.0.6/iterative_stats/iterative_extrema.py
--rw-r--r--   0        0        0     1661 2023-06-26 12:42:26.773409 iterative_stats-0.0.6/iterative_stats/iterative_mean.py
--rw-r--r--   0        0        0     2803 2023-06-26 12:42:26.773409 iterative_stats-0.0.6/iterative_stats/iterative_moments.py
--rw-r--r--   0        0        0     2205 2023-06-26 12:42:26.773409 iterative_stats-0.0.6/iterative_stats/iterative_quantile.py
--rw-r--r--   0        0        0      920 2023-06-26 12:42:26.773409 iterative_stats-0.0.6/iterative_stats/iterative_threshold.py
--rw-r--r--   0        0        0     1751 2023-06-26 12:42:26.773409 iterative_stats-0.0.6/iterative_stats/iterative_variance.py
--rw-r--r--   0        0        0       63 2023-06-26 12:42:26.773409 iterative_stats-0.0.6/iterative_stats/sensitivity/__init__.py
--rw-r--r--   0        0        0     9146 2023-06-26 12:42:26.773409 iterative_stats-0.0.6/iterative_stats/sensitivity/abstract_sensitivity.py
--rw-r--r--   0        0        0     1864 2023-06-26 12:42:26.773409 iterative_stats-0.0.6/iterative_stats/sensitivity/sensitivity_jansen.py
--rw-r--r--   0        0        0     3740 2023-06-26 12:42:26.773409 iterative_stats-0.0.6/iterative_stats/sensitivity/sensitivity_martinez.py
--rw-r--r--   0        0        0     3401 2023-06-26 12:42:26.773409 iterative_stats-0.0.6/iterative_stats/sensitivity/sensitivity_saltelli.py
--rw-r--r--   0        0        0      277 2023-06-26 12:42:26.773409 iterative_stats-0.0.6/iterative_stats/utils/dot_prod.py
--rw-r--r--   0        0        0       84 2023-06-26 12:42:26.773409 iterative_stats-0.0.6/iterative_stats/utils/logger.py
--rw-r--r--   0        0        0     1309 2023-06-26 12:42:26.773409 iterative_stats-0.0.6/pyproject.toml
--rw-r--r--   0        0        0     8493 1970-01-01 00:00:00.000000 iterative_stats-0.0.6/PKG-INFO
+-rw-r--r--   0        0        0     1549 2023-06-26 13:21:55.215218 iterative_stats-0.1.0/LICENSE
+-rw-r--r--   0        0        0     7834 2023-06-26 13:21:55.215218 iterative_stats-0.1.0/README.md
+-rw-r--r--   0        0        0     1357 2023-06-26 13:21:55.215218 iterative_stats-0.1.0/iterative_stats/abstract_iterative_statistics.py
+-rw-r--r--   0        0        0     1711 2023-06-26 13:21:55.215218 iterative_stats-0.1.0/iterative_stats/experimental_design/experiment.py
+-rw-r--r--   0        0        0     2038 2023-06-26 13:21:55.215218 iterative_stats-0.1.0/iterative_stats/iterative_covariance.py
+-rw-r--r--   0        0        0     4374 2023-06-26 13:21:55.215218 iterative_stats-0.1.0/iterative_stats/iterative_dotproduct.py
+-rw-r--r--   0        0        0     1055 2023-06-26 13:21:55.215218 iterative_stats-0.1.0/iterative_stats/iterative_extrema.py
+-rw-r--r--   0        0        0     1661 2023-06-26 13:21:55.215218 iterative_stats-0.1.0/iterative_stats/iterative_mean.py
+-rw-r--r--   0        0        0     2803 2023-06-26 13:21:55.215218 iterative_stats-0.1.0/iterative_stats/iterative_moments.py
+-rw-r--r--   0        0        0     2205 2023-06-26 13:21:55.215218 iterative_stats-0.1.0/iterative_stats/iterative_quantile.py
+-rw-r--r--   0        0        0      920 2023-06-26 13:21:55.215218 iterative_stats-0.1.0/iterative_stats/iterative_threshold.py
+-rw-r--r--   0        0        0     1751 2023-06-26 13:21:55.215218 iterative_stats-0.1.0/iterative_stats/iterative_variance.py
+-rw-r--r--   0        0        0       63 2023-06-26 13:21:55.215218 iterative_stats-0.1.0/iterative_stats/sensitivity/__init__.py
+-rw-r--r--   0        0        0     9146 2023-06-26 13:21:55.215218 iterative_stats-0.1.0/iterative_stats/sensitivity/abstract_sensitivity.py
+-rw-r--r--   0        0        0     1864 2023-06-26 13:21:55.215218 iterative_stats-0.1.0/iterative_stats/sensitivity/sensitivity_jansen.py
+-rw-r--r--   0        0        0     3740 2023-06-26 13:21:55.219218 iterative_stats-0.1.0/iterative_stats/sensitivity/sensitivity_martinez.py
+-rw-r--r--   0        0        0     3401 2023-06-26 13:21:55.219218 iterative_stats-0.1.0/iterative_stats/sensitivity/sensitivity_saltelli.py
+-rw-r--r--   0        0        0      277 2023-06-26 13:21:55.219218 iterative_stats-0.1.0/iterative_stats/utils/dot_prod.py
+-rw-r--r--   0        0        0       84 2023-06-26 13:21:55.219218 iterative_stats-0.1.0/iterative_stats/utils/logger.py
+-rw-r--r--   0        0        0     1309 2023-06-26 13:21:55.219218 iterative_stats-0.1.0/pyproject.toml
+-rw-r--r--   0        0        0     8509 1970-01-01 00:00:00.000000 iterative_stats-0.1.0/PKG-INFO
```

### Comparing `iterative_stats-0.0.6/LICENSE` & `iterative_stats-0.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `iterative_stats-0.0.6/README.md` & `iterative_stats-0.1.0/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -120,15 +120,15 @@
 total_order = sensitivity_instance.getFirstOrderIndices()
 print(f" Total Order Sobol indices (Martinez method): {first_order}")
 
 second_order = sensitivity_instance.getFirstOrderIndices()
 print(f" Second Order Sobol indices (Martinez method): {first_order}")
 ```
 
-NB: The computation of Sobol Indices requires the preparation of a specific experimental design based on the pick-freeze method (see [[1]](#1) for details). This method has been implemented into the class [**AbstractExperiment**](experimental_design/experiment.py) and some examples can be found [here](tests/unit/experimental_design/test_experiments.py).
+NB: The computation of Sobol Indices requires the preparation of a specific experimental design based on the pick-freeze method (see [[1]](#1) for details). This method has been implemented into the class [**AbstractExperiment**](iterative_stats/experimental_design/experiment.py) and some examples can be found [here](tests/unit/experimental_design/test_experiments.py).
 
 
 ## References 
 The implementation of the iterative formulas is based on the following papers:
 
 <a id="1">[1]</a>  Théophile Terraz, Alejandro Ribes, Yvan Fournier, Bertrand Iooss, and Bruno Raffin. 2017. Melissa: large scale in transit sensitivity analysis avoiding intermediate files. In Proceedings of the International Conference for High Performance Computing, Networking, Storage and Analysis (SC '17). Association for Computing Machinery, New York, NY, USA, Article 61, 1–14. https://doi.org/10.1145/3126908.3126922
```

### Comparing `iterative_stats-0.0.6/iterative_stats/abstract_iterative_statistics.py` & `iterative_stats-0.1.0/iterative_stats/abstract_iterative_statistics.py`

 * *Files identical despite different names*

### Comparing `iterative_stats-0.0.6/iterative_stats/iterative_covariance.py` & `iterative_stats-0.1.0/iterative_stats/iterative_covariance.py`

 * *Files identical despite different names*

### Comparing `iterative_stats-0.0.6/iterative_stats/iterative_dotproduct.py` & `iterative_stats-0.1.0/iterative_stats/iterative_dotproduct.py`

 * *Files identical despite different names*

### Comparing `iterative_stats-0.0.6/iterative_stats/iterative_extrema.py` & `iterative_stats-0.1.0/iterative_stats/iterative_extrema.py`

 * *Files identical despite different names*

### Comparing `iterative_stats-0.0.6/iterative_stats/iterative_mean.py` & `iterative_stats-0.1.0/iterative_stats/iterative_mean.py`

 * *Files identical despite different names*

### Comparing `iterative_stats-0.0.6/iterative_stats/iterative_moments.py` & `iterative_stats-0.1.0/iterative_stats/iterative_moments.py`

 * *Files identical despite different names*

### Comparing `iterative_stats-0.0.6/iterative_stats/iterative_quantile.py` & `iterative_stats-0.1.0/iterative_stats/iterative_quantile.py`

 * *Files identical despite different names*

### Comparing `iterative_stats-0.0.6/iterative_stats/iterative_threshold.py` & `iterative_stats-0.1.0/iterative_stats/iterative_threshold.py`

 * *Files identical despite different names*

### Comparing `iterative_stats-0.0.6/iterative_stats/iterative_variance.py` & `iterative_stats-0.1.0/iterative_stats/iterative_variance.py`

 * *Files identical despite different names*

### Comparing `iterative_stats-0.0.6/iterative_stats/sensitivity/abstract_sensitivity.py` & `iterative_stats-0.1.0/iterative_stats/sensitivity/abstract_sensitivity.py`

 * *Files identical despite different names*

### Comparing `iterative_stats-0.0.6/iterative_stats/sensitivity/sensitivity_jansen.py` & `iterative_stats-0.1.0/iterative_stats/sensitivity/sensitivity_jansen.py`

 * *Files identical despite different names*

### Comparing `iterative_stats-0.0.6/iterative_stats/sensitivity/sensitivity_martinez.py` & `iterative_stats-0.1.0/iterative_stats/sensitivity/sensitivity_martinez.py`

 * *Files identical despite different names*

### Comparing `iterative_stats-0.0.6/iterative_stats/sensitivity/sensitivity_saltelli.py` & `iterative_stats-0.1.0/iterative_stats/sensitivity/sensitivity_saltelli.py`

 * *Files identical despite different names*

### Comparing `iterative_stats-0.0.6/pyproject.toml` & `iterative_stats-0.1.0/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "iterative_stats"
-version = "0.0.6"
+version = "0.1.0"
 description = "This package implements iterative algorithms to compute some basics statistics"
 authors = ['Frederique Robin']
 readme = "README.md"
 license = "LICENSE" 
 classifiers = [
     "Programming Language :: Python :: 3",
     "License :: OSI Approved :: BSD License",
```

### Comparing `iterative_stats-0.0.6/PKG-INFO` & `iterative_stats-0.1.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: iterative-stats
-Version: 0.0.6
+Version: 0.1.0
 Summary: This package implements iterative algorithms to compute some basics statistics
 License: LICENSE
 Author: Frederique Robin
 Requires-Python: >=3.8,<3.11
 Classifier: License :: OSI Approved :: BSD License
 Classifier: License :: Other/Proprietary License
 Classifier: Operating System :: OS Independent
@@ -138,15 +138,15 @@
 total_order = sensitivity_instance.getFirstOrderIndices()
 print(f" Total Order Sobol indices (Martinez method): {first_order}")
 
 second_order = sensitivity_instance.getFirstOrderIndices()
 print(f" Second Order Sobol indices (Martinez method): {first_order}")
 ```
 
-NB: The computation of Sobol Indices requires the preparation of a specific experimental design based on the pick-freeze method (see [[1]](#1) for details). This method has been implemented into the class [**AbstractExperiment**](experimental_design/experiment.py) and some examples can be found [here](tests/unit/experimental_design/test_experiments.py).
+NB: The computation of Sobol Indices requires the preparation of a specific experimental design based on the pick-freeze method (see [[1]](#1) for details). This method has been implemented into the class [**AbstractExperiment**](iterative_stats/experimental_design/experiment.py) and some examples can be found [here](tests/unit/experimental_design/test_experiments.py).
 
 
 ## References 
 The implementation of the iterative formulas is based on the following papers:
 
 <a id="1">[1]</a>  Théophile Terraz, Alejandro Ribes, Yvan Fournier, Bertrand Iooss, and Bruno Raffin. 2017. Melissa: large scale in transit sensitivity analysis avoiding intermediate files. In Proceedings of the International Conference for High Performance Computing, Networking, Storage and Analysis (SC '17). Association for Computing Machinery, New York, NY, USA, Article 61, 1–14. https://doi.org/10.1145/3126908.3126922
```

