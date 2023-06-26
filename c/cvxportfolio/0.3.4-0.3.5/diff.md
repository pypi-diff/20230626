# Comparing `tmp/cvxportfolio-0.3.4.tar.gz` & `tmp/cvxportfolio-0.3.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cvxportfolio-0.3.4.tar", last modified: Wed Jun 21 02:55:07 2023, max compression
+gzip compressed data, was "cvxportfolio-0.3.5.tar", last modified: Mon Jun 26 17:12:20 2023, max compression
```

## Comparing `cvxportfolio-0.3.4.tar` & `cvxportfolio-0.3.5.tar`

### file list

```diff
@@ -1,43 +1,43 @@
-drwxr-xr-x   0 enzo       (501) staff       (20)        0 2023-06-21 02:55:07.841200 cvxportfolio-0.3.4/
--rw-r--r--   0 enzo       (501) staff       (20)      199 2023-04-08 05:48:25.000000 cvxportfolio-0.3.4/AUTHORS
--rw-r--r--   0 enzo       (501) staff       (20)      599 2023-04-08 05:48:25.000000 cvxportfolio-0.3.4/LICENSE
--rw-r--r--   0 enzo       (501) staff       (20)     6080 2023-06-21 02:55:07.840826 cvxportfolio-0.3.4/PKG-INFO
--rw-r--r--   0 enzo       (501) staff       (20)     5710 2023-06-18 05:48:46.000000 cvxportfolio-0.3.4/README.md
-drwxr-xr-x   0 enzo       (501) staff       (20)        0 2023-06-21 02:55:07.821729 cvxportfolio-0.3.4/cvxportfolio/
--rw-r--r--   0 enzo       (501) staff       (20)      912 2023-06-21 02:54:26.000000 cvxportfolio-0.3.4/cvxportfolio/__init__.py
--rw-r--r--   0 enzo       (501) staff       (20)     2053 2023-06-14 04:09:34.000000 cvxportfolio-0.3.4/cvxportfolio/benchmark.py
--rw-r--r--   0 enzo       (501) staff       (20)    11940 2023-06-18 05:48:46.000000 cvxportfolio-0.3.4/cvxportfolio/constraints.py
--rw-r--r--   0 enzo       (501) staff       (20)    14023 2023-06-18 05:48:46.000000 cvxportfolio-0.3.4/cvxportfolio/costs.py
--rw-r--r--   0 enzo       (501) staff       (20)    20123 2023-06-10 04:38:54.000000 cvxportfolio-0.3.4/cvxportfolio/data.py
--rw-r--r--   0 enzo       (501) staff       (20)     1004 2023-05-11 16:35:10.000000 cvxportfolio-0.3.4/cvxportfolio/errors.py
--rw-r--r--   0 enzo       (501) staff       (20)    14756 2023-06-18 05:48:46.000000 cvxportfolio-0.3.4/cvxportfolio/estimator.py
--rw-r--r--   0 enzo       (501) staff       (20)     9724 2023-06-18 05:48:46.000000 cvxportfolio-0.3.4/cvxportfolio/forecast.py
--rw-r--r--   0 enzo       (501) staff       (20)    21189 2023-06-18 05:48:46.000000 cvxportfolio-0.3.4/cvxportfolio/policies.py
--rw-r--r--   0 enzo       (501) staff       (20)     6483 2023-06-14 04:09:34.000000 cvxportfolio-0.3.4/cvxportfolio/result.py
--rw-r--r--   0 enzo       (501) staff       (20)     9003 2023-06-18 05:48:46.000000 cvxportfolio-0.3.4/cvxportfolio/returns.py
--rw-r--r--   0 enzo       (501) staff       (20)    17823 2023-06-18 05:48:46.000000 cvxportfolio-0.3.4/cvxportfolio/risks.py
--rw-r--r--   0 enzo       (501) staff       (20)    39887 2023-06-21 02:54:26.000000 cvxportfolio-0.3.4/cvxportfolio/simulator.py
-drwxr-xr-x   0 enzo       (501) staff       (20)        0 2023-06-21 02:55:07.838670 cvxportfolio-0.3.4/cvxportfolio/tests/
--rw-r--r--   0 enzo       (501) staff       (20)        0 2023-06-19 17:48:06.000000 cvxportfolio-0.3.4/cvxportfolio/tests/__init__.py
--rw-r--r--   0 enzo       (501) staff       (20)     1623 2023-05-27 05:39:35.000000 cvxportfolio-0.3.4/cvxportfolio/tests/base.py
--rw-r--r--   0 enzo       (501) staff       (20)   156730 2023-05-11 16:35:10.000000 cvxportfolio-0.3.4/cvxportfolio/tests/returns.csv
--rw-r--r--   0 enzo       (501) staff       (20)   149356 2023-05-11 16:35:10.000000 cvxportfolio-0.3.4/cvxportfolio/tests/sigmas.csv
--rw-r--r--   0 enzo       (501) staff       (20)     9929 2023-05-27 05:39:35.000000 cvxportfolio-0.3.4/cvxportfolio/tests/test_constraints.py
--rw-r--r--   0 enzo       (501) staff       (20)     8359 2023-06-14 04:09:34.000000 cvxportfolio-0.3.4/cvxportfolio/tests/test_costs.py
--rw-r--r--   0 enzo       (501) staff       (20)    10308 2023-05-27 05:39:35.000000 cvxportfolio-0.3.4/cvxportfolio/tests/test_data.py
--rw-r--r--   0 enzo       (501) staff       (20)     6737 2023-06-18 05:48:46.000000 cvxportfolio-0.3.4/cvxportfolio/tests/test_estimator.py
--rw-r--r--   0 enzo       (501) staff       (20)     8877 2023-06-10 04:38:54.000000 cvxportfolio-0.3.4/cvxportfolio/tests/test_forecast.py
--rw-r--r--   0 enzo       (501) staff       (20)    21842 2023-06-14 04:09:34.000000 cvxportfolio-0.3.4/cvxportfolio/tests/test_policies.py
--rw-r--r--   0 enzo       (501) staff       (20)     5754 2023-06-10 04:38:54.000000 cvxportfolio-0.3.4/cvxportfolio/tests/test_returns.py
--rw-r--r--   0 enzo       (501) staff       (20)     9065 2023-05-27 05:39:35.000000 cvxportfolio-0.3.4/cvxportfolio/tests/test_risks.py
--rw-r--r--   0 enzo       (501) staff       (20)    26143 2023-06-18 05:48:46.000000 cvxportfolio-0.3.4/cvxportfolio/tests/test_simulator.py
--rw-r--r--   0 enzo       (501) staff       (20)   116620 2023-05-11 16:35:10.000000 cvxportfolio-0.3.4/cvxportfolio/tests/volumes.csv
--rw-r--r--   0 enzo       (501) staff       (20)     1269 2023-06-18 05:48:46.000000 cvxportfolio-0.3.4/cvxportfolio/utils.py
-drwxr-xr-x   0 enzo       (501) staff       (20)        0 2023-06-21 02:55:07.824043 cvxportfolio-0.3.4/cvxportfolio.egg-info/
--rw-r--r--   0 enzo       (501) staff       (20)     6080 2023-06-21 02:55:07.000000 cvxportfolio-0.3.4/cvxportfolio.egg-info/PKG-INFO
--rw-r--r--   0 enzo       (501) staff       (20)     1019 2023-06-21 02:55:07.000000 cvxportfolio-0.3.4/cvxportfolio.egg-info/SOURCES.txt
--rw-r--r--   0 enzo       (501) staff       (20)        1 2023-06-21 02:55:07.000000 cvxportfolio-0.3.4/cvxportfolio.egg-info/dependency_links.txt
--rw-r--r--   0 enzo       (501) staff       (20)       59 2023-06-21 02:55:07.000000 cvxportfolio-0.3.4/cvxportfolio.egg-info/requires.txt
--rw-r--r--   0 enzo       (501) staff       (20)       13 2023-06-21 02:55:07.000000 cvxportfolio-0.3.4/cvxportfolio.egg-info/top_level.txt
--rw-r--r--   0 enzo       (501) staff       (20)       38 2023-06-21 02:55:07.841290 cvxportfolio-0.3.4/setup.cfg
--rw-r--r--   0 enzo       (501) staff       (20)      937 2023-06-21 02:54:26.000000 cvxportfolio-0.3.4/setup.py
+drwxr-xr-x   0 enzo       (501) staff       (20)        0 2023-06-26 17:12:20.527514 cvxportfolio-0.3.5/
+-rw-r--r--   0 enzo       (501) staff       (20)      199 2023-04-08 05:48:25.000000 cvxportfolio-0.3.5/AUTHORS
+-rw-r--r--   0 enzo       (501) staff       (20)      599 2023-04-08 05:48:25.000000 cvxportfolio-0.3.5/LICENSE
+-rw-r--r--   0 enzo       (501) staff       (20)     6235 2023-06-26 17:12:20.527187 cvxportfolio-0.3.5/PKG-INFO
+-rw-r--r--   0 enzo       (501) staff       (20)     5865 2023-06-26 16:58:22.000000 cvxportfolio-0.3.5/README.md
+drwxr-xr-x   0 enzo       (501) staff       (20)        0 2023-06-26 17:12:20.506578 cvxportfolio-0.3.5/cvxportfolio/
+-rw-r--r--   0 enzo       (501) staff       (20)     1010 2023-06-26 17:12:06.000000 cvxportfolio-0.3.5/cvxportfolio/__init__.py
+-rw-r--r--   0 enzo       (501) staff       (20)     2155 2023-06-26 16:58:07.000000 cvxportfolio-0.3.5/cvxportfolio/benchmark.py
+-rw-r--r--   0 enzo       (501) staff       (20)    11454 2023-06-26 16:58:07.000000 cvxportfolio-0.3.5/cvxportfolio/constraints.py
+-rw-r--r--   0 enzo       (501) staff       (20)    13746 2023-06-26 16:58:07.000000 cvxportfolio-0.3.5/cvxportfolio/costs.py
+-rw-r--r--   0 enzo       (501) staff       (20)    20391 2023-06-26 16:58:07.000000 cvxportfolio-0.3.5/cvxportfolio/data.py
+-rw-r--r--   0 enzo       (501) staff       (20)     1004 2023-05-11 16:35:10.000000 cvxportfolio-0.3.5/cvxportfolio/errors.py
+-rw-r--r--   0 enzo       (501) staff       (20)    15400 2023-06-26 16:58:07.000000 cvxportfolio-0.3.5/cvxportfolio/estimator.py
+-rw-r--r--   0 enzo       (501) staff       (20)     9287 2023-06-26 16:58:07.000000 cvxportfolio-0.3.5/cvxportfolio/forecast.py
+-rw-r--r--   0 enzo       (501) staff       (20)    22146 2023-06-26 16:58:07.000000 cvxportfolio-0.3.5/cvxportfolio/policies.py
+-rw-r--r--   0 enzo       (501) staff       (20)     6483 2023-06-14 04:09:34.000000 cvxportfolio-0.3.5/cvxportfolio/result.py
+-rw-r--r--   0 enzo       (501) staff       (20)     8554 2023-06-26 16:58:07.000000 cvxportfolio-0.3.5/cvxportfolio/returns.py
+-rw-r--r--   0 enzo       (501) staff       (20)    17384 2023-06-26 16:58:07.000000 cvxportfolio-0.3.5/cvxportfolio/risks.py
+-rw-r--r--   0 enzo       (501) staff       (20)    34392 2023-06-26 16:58:07.000000 cvxportfolio-0.3.5/cvxportfolio/simulator.py
+drwxr-xr-x   0 enzo       (501) staff       (20)        0 2023-06-26 17:12:20.526106 cvxportfolio-0.3.5/cvxportfolio/tests/
+-rw-r--r--   0 enzo       (501) staff       (20)        0 2023-06-26 17:12:06.000000 cvxportfolio-0.3.5/cvxportfolio/tests/__init__.py
+-rw-r--r--   0 enzo       (501) staff       (20)     1635 2023-06-26 16:58:07.000000 cvxportfolio-0.3.5/cvxportfolio/tests/base.py
+-rw-r--r--   0 enzo       (501) staff       (20)   156730 2023-05-11 16:35:10.000000 cvxportfolio-0.3.5/cvxportfolio/tests/returns.csv
+-rw-r--r--   0 enzo       (501) staff       (20)   149356 2023-05-11 16:35:10.000000 cvxportfolio-0.3.5/cvxportfolio/tests/sigmas.csv
+-rw-r--r--   0 enzo       (501) staff       (20)    10030 2023-06-26 16:58:07.000000 cvxportfolio-0.3.5/cvxportfolio/tests/test_constraints.py
+-rw-r--r--   0 enzo       (501) staff       (20)     8457 2023-06-26 16:58:07.000000 cvxportfolio-0.3.5/cvxportfolio/tests/test_costs.py
+-rw-r--r--   0 enzo       (501) staff       (20)    10330 2023-06-26 16:58:07.000000 cvxportfolio-0.3.5/cvxportfolio/tests/test_data.py
+-rw-r--r--   0 enzo       (501) staff       (20)     7078 2023-06-26 16:58:07.000000 cvxportfolio-0.3.5/cvxportfolio/tests/test_estimator.py
+-rw-r--r--   0 enzo       (501) staff       (20)     8956 2023-06-26 16:58:07.000000 cvxportfolio-0.3.5/cvxportfolio/tests/test_forecast.py
+-rw-r--r--   0 enzo       (501) staff       (20)    22256 2023-06-26 16:58:07.000000 cvxportfolio-0.3.5/cvxportfolio/tests/test_policies.py
+-rw-r--r--   0 enzo       (501) staff       (20)     5832 2023-06-26 16:58:07.000000 cvxportfolio-0.3.5/cvxportfolio/tests/test_returns.py
+-rw-r--r--   0 enzo       (501) staff       (20)     9194 2023-06-26 16:58:07.000000 cvxportfolio-0.3.5/cvxportfolio/tests/test_risks.py
+-rw-r--r--   0 enzo       (501) staff       (20)    26221 2023-06-26 16:58:07.000000 cvxportfolio-0.3.5/cvxportfolio/tests/test_simulator.py
+-rw-r--r--   0 enzo       (501) staff       (20)   116620 2023-05-11 16:35:10.000000 cvxportfolio-0.3.5/cvxportfolio/tests/volumes.csv
+-rw-r--r--   0 enzo       (501) staff       (20)     1269 2023-06-18 05:48:46.000000 cvxportfolio-0.3.5/cvxportfolio/utils.py
+drwxr-xr-x   0 enzo       (501) staff       (20)        0 2023-06-26 17:12:20.509184 cvxportfolio-0.3.5/cvxportfolio.egg-info/
+-rw-r--r--   0 enzo       (501) staff       (20)     6235 2023-06-26 17:12:20.000000 cvxportfolio-0.3.5/cvxportfolio.egg-info/PKG-INFO
+-rw-r--r--   0 enzo       (501) staff       (20)     1019 2023-06-26 17:12:20.000000 cvxportfolio-0.3.5/cvxportfolio.egg-info/SOURCES.txt
+-rw-r--r--   0 enzo       (501) staff       (20)        1 2023-06-26 17:12:20.000000 cvxportfolio-0.3.5/cvxportfolio.egg-info/dependency_links.txt
+-rw-r--r--   0 enzo       (501) staff       (20)       65 2023-06-26 17:12:20.000000 cvxportfolio-0.3.5/cvxportfolio.egg-info/requires.txt
+-rw-r--r--   0 enzo       (501) staff       (20)       13 2023-06-26 17:12:20.000000 cvxportfolio-0.3.5/cvxportfolio.egg-info/top_level.txt
+-rw-r--r--   0 enzo       (501) staff       (20)       38 2023-06-26 17:12:20.527604 cvxportfolio-0.3.5/setup.cfg
+-rw-r--r--   0 enzo       (501) staff       (20)     1032 2023-06-26 17:12:06.000000 cvxportfolio-0.3.5/setup.py
```

### Comparing `cvxportfolio-0.3.4/LICENSE` & `cvxportfolio-0.3.5/LICENSE`

 * *Files identical despite different names*

### Comparing `cvxportfolio-0.3.4/PKG-INFO` & `cvxportfolio-0.3.5/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cvxportfolio
-Version: 0.3.4
+Version: 0.3.5
 Summary: Portfolio optimization.
 Home-page: https://cvxportfolio.readthedocs.io
 Author: Enzo Busseti, Stephen Boyd, Steven Diamond, BlackRock Inc.
 Author-email: enzo.busseti@gmail.com
 Maintainer: Enzo Busseti
 License: Apache 2.0
 Description-Content-Type: text/markdown
@@ -12,15 +12,15 @@
 License-File: AUTHORS
 
 # Cvxportfolio
 
 [![CVXportfolio on PyPI](https://img.shields.io/pypi/v/cvxportfolio.svg)](https://pypi.org/project/cvxportfolio/)
 [![Downloads](https://static.pepy.tech/personalized-badge/cvxportfolio?period=month&units=international_system&left_color=black&right_color=orange&left_text=PyPI%20downloads%20per%20month)](https://pepy.tech/project/cvxportfolio)
 [![Coverage Status](https://coveralls.io/repos/github/cvxgrp/cvxportfolio/badge.svg?branch=master)](https://coveralls.io/github/cvxgrp/cvxportfolio?branch=master)
-
+[![Documentation Status](https://readthedocs.org/projects/cvxportfolio/badge/?version=latest)](https://cvxportfolio.readthedocs.io/en/latest/?badge=latest)
 
 **WORK IN PROGRESS. Cvxportfolio is currently under development. We will freeze the user interface by end of 2023Q2 and release the first stable version by end of 2023Q3.**
 
 
 `cvxportfolio` is a python library for portfolio optimization and simulation
 based on the book [Multi-Period Trading via Convex Optimization](https://web.stanford.edu/~boyd/papers/pdf/cvx_portfolio.pdf)
 (also [available in print](https://www.amazon.com/Multi-Period-Trading-Convex-Optimization-Foundations/dp/1680833286/)).
```

### Comparing `cvxportfolio-0.3.4/README.md` & `cvxportfolio-0.3.5/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 # Cvxportfolio
 
 [![CVXportfolio on PyPI](https://img.shields.io/pypi/v/cvxportfolio.svg)](https://pypi.org/project/cvxportfolio/)
 [![Downloads](https://static.pepy.tech/personalized-badge/cvxportfolio?period=month&units=international_system&left_color=black&right_color=orange&left_text=PyPI%20downloads%20per%20month)](https://pepy.tech/project/cvxportfolio)
 [![Coverage Status](https://coveralls.io/repos/github/cvxgrp/cvxportfolio/badge.svg?branch=master)](https://coveralls.io/github/cvxgrp/cvxportfolio?branch=master)
-
+[![Documentation Status](https://readthedocs.org/projects/cvxportfolio/badge/?version=latest)](https://cvxportfolio.readthedocs.io/en/latest/?badge=latest)
 
 **WORK IN PROGRESS. Cvxportfolio is currently under development. We will freeze the user interface by end of 2023Q2 and release the first stable version by end of 2023Q3.**
 
 
 `cvxportfolio` is a python library for portfolio optimization and simulation
 based on the book [Multi-Period Trading via Convex Optimization](https://web.stanford.edu/~boyd/papers/pdf/cvx_portfolio.pdf)
 (also [available in print](https://www.amazon.com/Multi-Period-Trading-Convex-Optimization-Foundations/dp/1680833286/)).
```

### Comparing `cvxportfolio-0.3.4/cvxportfolio/__init__.py` & `cvxportfolio-0.3.5/cvxportfolio/__init__.py`

 * *Files 15% similar despite different names*

```diff
@@ -7,20 +7,24 @@
 #    http://www.apache.org/licenses/LICENSE-2.0
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
+"""Cvxportfolio __init__ module.
+
+This module only republishes the api of a selection of cvxportfolio modules.
+The __all__ attribute of each is used.
+"""
+
+__version__ = "0.3.5"
 
-__version__ = "0.3.4"
-from .data import *
 from .simulator import *
-from .result import *
 from .policies import *
 from .constraints import *
 from .costs import *
 from .returns import *
-from .estimator import DataEstimator
 from .risks import *
 from .returns import *
 from .benchmark import *
+from .result import *
```

### Comparing `cvxportfolio-0.3.4/cvxportfolio/benchmark.py` & `cvxportfolio-0.3.5/cvxportfolio/benchmark.py`

 * *Files 14% similar despite different names*

```diff
@@ -18,38 +18,44 @@
 import numpy as np
 import pandas as pd
 
 from .estimator import PolicyEstimator
 
 __all__ = ['CashBenchmark', 'UniformBenchmark', 'MarketBenchmark']
 
-class CashBenchmark(PolicyEstimator):
+
+class BaseBenchmark(PolicyEstimator):
+    """Base class for cvxportfolio benchmark weights."""
+    pass
+
+class CashBenchmark(BaseBenchmark):
     """Default benchmark weights for cvxportfolio risk models.
     """
 
-    def pre_evaluation(self, universe, backtest_times):
+    def _pre_evaluation(self, universe, backtest_times):
         """Define current_value as a constant."""
         self.current_value = np.zeros(len(universe))
         self.current_value[-1] = 1.
 
 
-class UniformBenchmark(PolicyEstimator):
+class UniformBenchmark(BaseBenchmark):
     """Benchmark weights uniform on non-cash assets.
     """
 
-    def pre_evaluation(self, universe, backtest_times):
+    def _pre_evaluation(self, universe, backtest_times):
         """Define current_value as a constant."""
         self.current_value = np.ones(len(universe))
         self.current_value[-1] = 0.
         self.current_value /= np.sum(self.current_value[:-1])
    
      
-class MarketBenchmark(PolicyEstimator):
+class MarketBenchmark(BaseBenchmark):
     """Portfolio weighted by last year's total volumes.
     """
     
-    def values_in_time(self, past_volumes, **kwargs):
+    def _values_in_time(self, past_volumes, **kwargs):
         """Update current_value using past year's volumes."""
-        sumvolumes = past_volumes.loc[past_volumes.index >= (past_volumes.index[-1] - pd.Timedelta('365d'))].sum()
-        self.current_value = np.zeros(len(sumvolumes) + 1)
-        self.current_value[:-1] = sumvolumes / sum(sumvolumes)
+        sumvolumes = past_volumes.loc[past_volumes.index >= (past_volumes.index[-1] - pd.Timedelta('365d'))].mean()
+        result = np.zeros(len(sumvolumes) + 1)
+        result[:-1] = sumvolumes / sum(sumvolumes)
+        return result
```

### Comparing `cvxportfolio-0.3.4/cvxportfolio/constraints.py` & `cvxportfolio-0.3.5/cvxportfolio/constraints.py`

 * *Files 5% similar despite different names*

```diff
@@ -69,28 +69,26 @@
     but instead should be their own class (used as well
     by risk models, ...).
     """
     
     def __init__(self):
         self.covarianceforecaster = HistoricalFactorizedCovariance()
     
-    def pre_evaluation(self, universe, backtest_times):
-        super().pre_evaluation(universe=universe, backtest_times=backtest_times)
+    def _pre_evaluation(self, universe, backtest_times):
         self.market_vector = cp.Parameter(len(universe)-1)
     
-    def values_in_time(self, t, past_volumes, past_returns, **kwargs):
-        super().values_in_time(past_volumes=past_volumes, past_returns=past_returns, t=t, **kwargs)
+    def _values_in_time(self, t, past_volumes, past_returns, **kwargs):
         tmp = past_volumes.iloc[-250:].mean()
         tmp /= sum(tmp)
         
         tmp2 = self.covarianceforecaster.current_value @ (self.covarianceforecaster.current_value.T @ tmp)
         # print(tmp2)
         self.market_vector.value = np.array(tmp2)
         
-    def compile_to_cvxpy(self, w_plus, z, w_plus_minus_w_bm):
+    def _compile_to_cvxpy(self, w_plus, z, w_plus_minus_w_bm):
         return w_plus[:-1].T @ self.market_vector == 0
         
         
 class TurnoverLimit(BaseTradeConstraint):
     """Turnover limit as a fraction of the portfolio value.
     
     See page 37 of the book.
@@ -98,15 +96,15 @@
     :param delta: constant or changing in time turnover limit 
     :type delta: float or pd.Series 
     """
     
     def __init__(self, delta):
         self.delta = DataEstimator(delta, compile_parameter=True)
         
-    def compile_to_cvxpy(self, w_plus, z, w_plus_minus_w_bm):
+    def _compile_to_cvxpy(self, w_plus, z, w_plus_minus_w_bm):
         return .5 * cp.norm1(z[:-1]) <= self.delta.parameter
         
 
 class ParticipationRateLimit(BaseTradeConstraint):
     """A limit on maximum trades size as a fraction of market volumes.
     
 
@@ -118,58 +116,57 @@
 
     def __init__(self, volumes, max_fraction_of_volumes=0.05):
         self.volumes = DataEstimator(volumes, compile_parameter=True)
         self.max_participation_rate = DataEstimator(
             max_fraction_of_volumes, compile_parameter=True)
         self.portfolio_value = cp.Parameter(nonneg=True)
 
-    def values_in_time(self, current_portfolio_value, **kwargs):
+    def _values_in_time(self, current_portfolio_value, **kwargs):
         self.portfolio_value.value = current_portfolio_value
-        super().values_in_time(current_portfolio_value=current_portfolio_value, **kwargs)
         
-    def compile_to_cvxpy(self, w_plus, z, w_plus_minus_w_bm):
+    def _compile_to_cvxpy(self, w_plus, z, w_plus_minus_w_bm):
         """Return a Cvxpy constraint."""
         return cp.multiply(cp.abs(z[:-1]), self.portfolio_value) <= cp.multiply(
             self.volumes.parameter, self.max_participation_rate.parameter
         )
 
 
 class LongOnly(BaseWeightConstraint):
     """A long only constraint.
     
     Imposes that at each point in time the post-trade
     weights are non-negative.
     """
 
-    def compile_to_cvxpy(self, w_plus, z, w_plus_minus_w_bm):
+    def _compile_to_cvxpy(self, w_plus, z, w_plus_minus_w_bm):
         """Return a Cvxpy constraint."""
         return w_plus[:-1] >= 0
 
 
 class NoTrade(BaseTradeConstraint):
     """No-trade condition on name on periods(s)."""
     
     def __init__(self, asset, periods):
         self.asset = asset
         self.periods = periods
     
-    def pre_evaluation(self, universe, backtest_times):
+    def _pre_evaluation(self, universe, backtest_times):
         self.index = universe.get_loc(self.asset)
         self.low = cp.Parameter()
         self.high = cp.Parameter()
     
-    def values_in_time(self, t, **kwargs):
+    def _values_in_time(self, t, **kwargs):
         if t in self.periods:
             self.low.value = 0.
             self.high.value = 0.
         else:
             self.low.value = -100.
             self.high.value = +100.
     
-    def compile_to_cvxpy(self, w_plus, z, w_plus_minus_w_bm):
+    def _compile_to_cvxpy(self, w_plus, z, w_plus_minus_w_bm):
         return [z[self.index] >= self.low, 
             z[self.index] <= self.high] 
         
 
 
 class LeverageLimit(BaseWeightConstraint):
     """A limit on leverage.
@@ -181,15 +178,15 @@
     :param limit: constant or varying in time leverage limit
     :type limit: float or pd.Series
     """
 
     def __init__(self, limit):
         self.limit = DataEstimator(limit, compile_parameter=True)
 
-    def compile_to_cvxpy(self, w_plus, z, w_plus_minus_w_bm):
+    def _compile_to_cvxpy(self, w_plus, z, w_plus_minus_w_bm):
         """Return a Cvxpy constraint."""
         return cp.norm(w_plus[:-1], 1) <= self.limit.parameter
 
 
 class MinCashBalance(BaseWeightConstraint):
     """Requires that the cash account is larger than c_min dollars.
     
@@ -198,19 +195,18 @@
     equivalent to the book definition's for long-only stock positions.
     """
     
     def __init__(self, c_min):
         self.c_min = DataEstimator(c_min)
         self.rhs = cp.Parameter()
     
-    def values_in_time(self, current_portfolio_value, **kwargs):
-        super().values_in_time(current_portfolio_value=current_portfolio_value, **kwargs)
+    def _values_in_time(self, current_portfolio_value, **kwargs):
         self.rhs.value = self.c_min.current_value/current_portfolio_value
     
-    def compile_to_cvxpy(self, w_plus, z, w_plus_minus_w_bm):
+    def _compile_to_cvxpy(self, w_plus, z, w_plus_minus_w_bm):
         """Return a Cvxpy constraint."""
         # TODO clarify this
         realcash = (w_plus[-1] - 2 * cp.sum(cp.neg(w_plus[:-1])))
         return realcash >= self.rhs
         
     
 class LongCash(MinCashBalance):
@@ -219,82 +215,80 @@
     def __init__(self):
         super().__init__(0.)
 
 
 class DollarNeutral(BaseWeightConstraint):
     """Long-short dollar neutral strategy."""
 
-    def compile_to_cvxpy(self, w_plus, z, w_plus_minus_w_bm):
+    def _compile_to_cvxpy(self, w_plus, z, w_plus_minus_w_bm):
         """Return a Cvxpy constraint."""
         return w_plus[-1] == 1
 
 
 class MaxWeights(BaseWeightConstraint):
     """A max limit on weights.
 
     Attributes:
       limit: A series or number giving the weights limit.
     """
 
     def __init__(self, limit):
         self.limit = DataEstimator(limit, compile_parameter=True)
 
-    def compile_to_cvxpy(self, w_plus, z, w_plus_minus_w_bm):
+    def _compile_to_cvxpy(self, w_plus, z, w_plus_minus_w_bm):
         """Return a Cvxpy constraint."""
         return w_plus[:-1] <= self.limit.parameter
 
 
 class MinWeights(BaseWeightConstraint):
     """A min limit on weights.
 
     Attributes:
       limit: A series or number giving the weights limit.
     """
 
     def __init__(self, limit):
         self.limit = DataEstimator(limit, compile_parameter=True)
 
-    def compile_to_cvxpy(self, w_plus, z, w_plus_minus_w_bm):
+    def _compile_to_cvxpy(self, w_plus, z, w_plus_minus_w_bm):
         """Return a Cvxpy constraint."""
         return w_plus[:-1] >= self.limit.parameter
 
 class MinMaxWeightsAtTimes(BaseWeightConstraint):
 
     def __init__(self, limit, times):
         self.base_limit = limit
         self.times = times
     
-    def pre_evaluation(self, universe, backtest_times):
-        super().pre_evaluation(universe=universe, backtest_times = backtest_times)
+    def _pre_evaluation(self, universe, backtest_times):
         self.backtest_times = backtest_times
         self.limit = cp.Parameter()
         
-    def values_in_time(self, t, mpo_step, **kwargs):
-        super().values_in_time(t=t, mpo_step=mpo_step, **kwargs)
+    def _values_in_time(self, t, mpo_step, **kwargs):
         tidx = self.backtest_times.get_loc(t)
         nowtidx = tidx + mpo_step
         if (nowtidx < len(self.backtest_times)) and self.backtest_times[nowtidx] in self.times:
             self.limit.value = self.base_limit
         else:
             self.limit.value = 100 * self.sign
 
 
 class MinWeightsAtTimes(MinMaxWeightsAtTimes):
     
     sign = -1.
 
-    def compile_to_cvxpy(self, w_plus, z, w_plus_minus_w_bm):
+    def _compile_to_cvxpy(self, w_plus, z, w_plus_minus_w_bm):
         """Return a Cvxpy constraint."""
         return w_plus[:-1] >= self.limit
         
 class MaxWeightsAtTimes(MinMaxWeightsAtTimes):
 
     sign = 1.
     
-    def compile_to_cvxpy(self, w_plus, z, w_plus_minus_w_bm):
+    def _compile_to_cvxpy(self, w_plus, z, w_plus_minus_w_bm):
         """Return a Cvxpy constraint."""
         return w_plus[:-1] <= self.limit
         
 
 class FactorMaxLimit(BaseWeightConstraint):
     """A max limit on portfolio-wide factor (e.g. beta) exposure.
 
@@ -304,15 +298,15 @@
         limit: A series of list or a single list giving the factor limits
     """
 
     def __init__(self, factor_exposure, limit):
         self.factor_exposure = DataEstimator(factor_exposure, compile_parameter=True)
         self.limit = DataEstimator(limit, compile_parameter=True)
 
-    def compile_to_cvxpy(self, w_plus, z, w_plus_minus_w_bm):
+    def _compile_to_cvxpy(self, w_plus, z, w_plus_minus_w_bm):
         """Return a Cvxpy constraint."""
         return self.factor_exposure.parameter.T @ w_plus[:-1] <= self.limit.parameter
 
 
 class FactorMinLimit(BaseWeightConstraint):
     """A min limit on portfolio-wide factor (e.g. beta) exposure.
 
@@ -322,15 +316,15 @@
         limit: A series of list or a single list giving the factor limits
     """
 
     def __init__(self, factor_exposure, limit):
         self.factor_exposure = DataEstimator(factor_exposure, compile_parameter=True)
         self.limit = DataEstimator(limit, compile_parameter=True)
 
-    def compile_to_cvxpy(self, w_plus, z, w_plus_minus_w_bm):
+    def _compile_to_cvxpy(self, w_plus, z, w_plus_minus_w_bm):
         """Return a Cvxpy constraint."""
         return self.factor_exposure.parameter.T @ w_plus[:-1] >= self.limit.parameter
 
 
 class FixedFactorLoading(BaseWeightConstraint):
     """A constraint to fix portfolio loadings to a set of factors.
 
@@ -342,10 +336,10 @@
         target: A series or number giving the targeted factor loading
     """
 
     def __init__(self, factor_exposure, target):
         self.factor_exposure = DataEstimator(factor_exposure, compile_parameter=True)
         self.target = DataEstimator(target, compile_parameter=True)
 
-    def compile_to_cvxpy(self, w_plus, z, w_plus_minus_w_bm):
+    def _compile_to_cvxpy(self, w_plus, z, w_plus_minus_w_bm):
         """Return a Cvxpy constraint."""
         return self.factor_exposure.parameter.T @ w_plus[:-1] == self.target.parameter
```

### Comparing `cvxportfolio-0.3.4/cvxportfolio/costs.py` & `cvxportfolio-0.3.5/cvxportfolio/costs.py`

 * *Files 4% similar despite different names*

```diff
@@ -44,15 +44,15 @@
             raise SyntaxError("You can only multiply cost by a scalar.")
         return CombinedCosts([self], [other])
 
     def __add__(self, other):
         """Add cost expression to another cost expression.
 
         Idea is to create a new CombinedCost class that
-        implements `compile_to_cvxpy` and values_in_time
+        implements `_compile_to_cvxpy` and _recursive_values_in_time
         by summing over costs.
 
         """
         if isinstance(other, CombinedCosts):
             return other + self
         return CombinedCosts([self, other], [1.0, 1.0])
 
@@ -100,27 +100,27 @@
         else:
             return CombinedCosts(self.costs + [other], self.multipliers + [1.0])
 
     def __mul__(self, other):
         """Multiply by constant."""
         return CombinedCosts(self.costs, [el * other for el in self.multipliers])
 
-    def pre_evaluation(self, *args, **kwargs):
+    def _recursive_pre_evaluation(self, *args, **kwargs):
         """Iterate over constituent costs."""
-        [el.pre_evaluation(*args, **kwargs) for el in self.costs]
+        [el._recursive_pre_evaluation(*args, **kwargs) for el in self.costs]
 
-    def values_in_time(self, **kwargs):
+    def _recursive_values_in_time(self, **kwargs):
         """Iterate over constituent costs."""
-        [el.values_in_time(**kwargs) for el in self.costs ]
+        [el._recursive_values_in_time(**kwargs) for el in self.costs ]
 
-    def compile_to_cvxpy(self, w_plus, z, portfolio_value):
+    def _compile_to_cvxpy(self, w_plus, z, portfolio_value):
         """Iterate over constituent costs."""
         self.expression = 0
         for multiplier, cost in zip(self.multipliers, self.costs):
-            self.expression += multiplier * cost.compile_to_cvxpy(w_plus, z, portfolio_value) 
+            self.expression += multiplier * cost._compile_to_cvxpy(w_plus, z, portfolio_value) 
         return self.expression
 
 
 class HoldingCost(BaseCost):
     """A model for holding costs.
 
     :param spread_on_borrowing_stocks_percent: spread on top of cash return payed for borrowing assets,
@@ -164,66 +164,64 @@
             DataEstimator(spread_on_lending_cash_percent)        
         self.spread_on_borrowing_cash_percent = None if spread_on_borrowing_cash_percent is None else \
             DataEstimator(spread_on_borrowing_cash_percent)
             
         self.periods_per_year = periods_per_year
         self.cash_return_on_borrow = cash_return_on_borrow
         
-    def pre_evaluation(self, universe, backtest_times):
-        super().pre_evaluation(universe=universe, backtest_times=backtest_times)
+    def _pre_evaluation(self, universe, backtest_times):
         
         if not (self.spread_on_borrowing_stocks_percent is None):
             self.borrow_cost_stocks = cp.Parameter(len(universe) - 1, nonneg=True)
         
         
-    def values_in_time(self, t, past_returns, **kwargs):
+    def _values_in_time(self, t, past_returns, **kwargs):
         """We use yesterday's value of the cash return here while in the simulator
         we use today's. In the US, updates to the FED rate are published outside
         of trading hours so we might as well use the actual value for today's. The difference
         is very small so for now we do this. 
         """
-        super().values_in_time(t=t, past_returns=past_returns, **kwargs)
         ppy = periods_per_year(past_returns.index) if self.periods_per_year is None else \
             self.periods_per_year
                                
         cash_return = past_returns.iloc[-1,-1]
 
         if not (self.spread_on_borrowing_stocks_percent is None):
             self.borrow_cost_stocks.value = np.ones(past_returns.shape[1] - 1) * (
                     cash_return if self.cash_return_on_borrow else 0.) + \
                 self.spread_on_borrowing_stocks_percent.current_value / (100 * ppy)
                 
-    def simulate(self, t, h_plus, current_and_past_returns, **kwargs):
+    def _simulate(self, t, h_plus, current_and_past_returns, **kwargs):
         
         ppy = periods_per_year(current_and_past_returns.index) if self.periods_per_year is None else \
             self.periods_per_year
         
         cash_return = current_and_past_returns.iloc[-1,-1]        
         multiplier = 1 / (100 * ppy)
         result = 0.
         borrowed_stock_positions = np.minimum(h_plus.iloc[:-1], 0.)
         result += np.sum(((cash_return if self.cash_return_on_borrow else 0.) + 
-            self.spread_on_borrowing_stocks_percent.values_in_time(t) * multiplier) * borrowed_stock_positions)
-        result += np.sum(h_plus[:-1] * self.dividends.values_in_time(t))
+            self.spread_on_borrowing_stocks_percent._recursive_values_in_time(t) * multiplier) * borrowed_stock_positions)
+        result += np.sum(h_plus[:-1] * self.dividends._recursive_values_in_time(t))
           
-        # lending_spread = DataEstimator(spread_on_lending_cash_percent).values_in_time(t) * multiplier
-        # borrowing_spread = DataEstimator(spread_on_borrowing_cash_percent).values_in_time(t) * multiplier
+        # lending_spread = DataEstimator(spread_on_lending_cash_percent)._recursive_values_in_time(t) * multiplier
+        # borrowing_spread = DataEstimator(spread_on_borrowing_cash_percent)._recursive_values_in_time(t) * multiplier
 
         # cash_return = current_and_past_returns.iloc[-1,-1]
         real_cash = h_plus.iloc[-1] + sum(np.minimum(h_plus.iloc[:-1], 0.))
 
         if real_cash > 0:
-            result += real_cash * (max(cash_return - self.spread_on_lending_cash_percent.values_in_time(t) * multiplier, 0.) - cash_return)
+            result += real_cash * (max(cash_return - self.spread_on_lending_cash_percent._recursive_values_in_time(t) * multiplier, 0.) - cash_return)
         else:
-            result += real_cash * self.spread_on_borrowing_cash_percent.values_in_time(t) * multiplier
+            result += real_cash * self.spread_on_borrowing_cash_percent._recursive_values_in_time(t) * multiplier
             
         return result
             
             
-    def compile_to_cvxpy(self, w_plus, z, w_plus_minus_w_bm):
+    def _compile_to_cvxpy(self, w_plus, z, w_plus_minus_w_bm):
         """Compile cost to cvxpy expression."""
         
         expression = 0. 
         
         if not (self.spread_on_borrowing_stocks_percent is None):
            expression += cp.multiply(self.borrow_cost_stocks, cp.neg(w_plus)[:-1])
         
@@ -259,60 +257,55 @@
         self.a = None if a is None else DataEstimator(a)
         self.pershare_cost = None if pershare_cost is None else DataEstimator(pershare_cost)
         self.b = None if b is None else DataEstimator(b)
         self.window_sigma_est = window_sigma_est
         self.window_volume_est = window_volume_est
         self.exponent = exponent
             
-    def pre_evaluation(self, universe, backtest_times):
-        super().pre_evaluation(universe=universe, backtest_times=backtest_times)
+    def _pre_evaluation(self, universe, backtest_times):
         self.first_term_multiplier = cp.Parameter(len(universe)-1, nonneg=True)
         if not (self.b is None):
             self.second_term_multiplier = cp.Parameter(len(universe)-1, nonneg=True)
 
-    def values_in_time(self, t,  current_portfolio_value, past_returns, past_volumes, current_prices, **kwargs):
-        
-        super().values_in_time(t=t, current_portfolio_value=current_portfolio_value, 
-            past_returns=past_returns, past_volumes=past_volumes, 
-            current_prices=current_prices, **kwargs)
-            
+    def _values_in_time(self, t,  current_portfolio_value, past_returns, past_volumes, current_prices, **kwargs):
+                    
         self.first_term_multiplier.value = self.a.current_value + self.pershare_cost.current_value / current_prices.values
         if not (self.b is None):
             sigma_est = np.sqrt((past_returns.iloc[-self.window_sigma_est:, :-1]**2).mean()).values
             volume_est = past_volumes.iloc[-self.window_volume_est:].mean().values
 
             self.second_term_multiplier.value = self.b.current_value * sigma_est * \
                 (current_portfolio_value / volume_est) ** (self.exponent - 1)
                 
-    def simulate(self, t, u, current_and_past_returns, current_and_past_volumes, current_prices, **kwargs):
+    def _simulate(self, t, u, current_and_past_returns, current_and_past_volumes, current_prices, **kwargs):
         
         sigma = np.std(current_and_past_returns.iloc[-self.window_sigma_est:, :-1], axis=0)
 
         result = 0.
         if not (self.pershare_cost is None):
             if current_prices is None:
                 raise SyntaxError("If you don't provide prices you should set persharecost to None")
-            result += self.pershare_cost.values_in_time(t) * int(sum(np.abs(u.iloc[:-1] + 1E-6) / current_prices.values))
+            result += self.pershare_cost._recursive_values_in_time(t) * int(sum(np.abs(u.iloc[:-1] + 1E-6) / current_prices.values))
 
-        result += sum(self.a.values_in_time(t) * np.abs(u.iloc[:-1]))
+        result += sum(self.a._recursive_values_in_time(t) * np.abs(u.iloc[:-1]))
 
         if not (self.b is None):
             if current_and_past_volumes is None:
                 raise SyntaxError("If you don't provide volumes you should set b to None")
             # we add 1 to the volumes to prevent 0 volumes error (trades are cancelled on 0 volumes)
-            result += (np.abs(u.iloc[:-1])**self.exponent) @ (self.b.values_in_time(t)  *
+            result += (np.abs(u.iloc[:-1])**self.exponent) @ (self.b._recursive_values_in_time(t)  *
                 sigma / ((current_and_past_volumes.iloc[-1] + 1) ** (self.exponent - 1)))
 
         assert not np.isnan(result)
         assert not np.isinf(result)
 
         return -result
         
         
-    def compile_to_cvxpy(self, w_plus, z, w_plus_minus_w_bm):
+    def _compile_to_cvxpy(self, w_plus, z, w_plus_minus_w_bm):
 
         expression = cp.abs(z[:-1]).T @ self.first_term_multiplier
         assert expression.is_convex()
         if not (self.b is None):
             expression += (cp.abs(z[:-1]) ** self.exponent).T @ self.second_term_multiplier
             assert expression.is_convex()
         return expression
```

### Comparing `cvxportfolio-0.3.4/cvxportfolio/data.py` & `cvxportfolio-0.3.5/cvxportfolio/data.py`

 * *Files 2% similar despite different names*

```diff
@@ -7,14 +7,20 @@
 #    http://www.apache.org/licenses/LICENSE-2.0
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
+"""DEPRECATED.
+
+This module will be removed or heavily reformatted, most of it is unused.
+The only parts that will remain are the FRED and YFinance interfaces, simplified,
+and not meant to be accessed directly by users.
+"""
 
 from pathlib import Path
 import yfinance as yf
 import pandas as pd
 import numpy as np
 import sqlite3
 
@@ -461,36 +467,36 @@
 class YfinanceTimeSeries(DataEstimator, YfinanceBase, PickleStore):
     
     def __init__(self, symbol, use_last_available_time=False, base_location=BASE_LOCATION):
         self.symbol = symbol
         self.base_location = base_location
         self.use_last_available_time = use_last_available_time
 
-    def pre_evaluation(self, *args, **kwargs):
+    def _recursive_pre_evaluation(self, *args, **kwargs):
         self.data = self.update_and_load(self.symbol)
         
         
 class FredTimeSeries(DataEstimator, FredBase, PickleStore):
     
     def __init__(self, symbol, use_last_available_time=False, base_location=BASE_LOCATION):
         self.symbol = symbol
         self.base_location = base_location
         self.use_last_available_time = use_last_available_time
 
-    def pre_evaluation(self, *args, **kwargs):
+    def _recursive_pre_evaluation(self, *args, **kwargs):
         self.data = self.update_and_load(self.symbol)
     
 class FredRateTimeSeries(DataEstimator, FredBase, RateBase, PickleStore):
     
     def __init__(self, symbol, use_last_available_time=False, base_location=BASE_LOCATION):
         self.symbol = symbol
         self.base_location = base_location
         self.use_last_available_time = use_last_available_time
 
-    def pre_evaluation(self, *args, **kwargs):
+    def _recursive_pre_evaluation(self, *args, **kwargs):
         self.data = self.update_and_load(self.symbol)    
         
 
 class TimeSeries(DataEstimator):
     """Class for time series data managed by Cvxportfolio.
 
     Args:
@@ -544,9 +550,9 @@
         self.__class__ = cls.__class__(
             cls.__name__ + "With" + storage.__name__, (cls, storage), {}
         )
 
         self.base_location = base_location
         self.use_last_available_time = use_last_available_time
 
-    def pre_evaluation(self, *args, **kwargs):
+    def _recursive_pre_evaluation(self, *args, **kwargs):
         self.data = self.update_and_load(self.symbol)
```

### Comparing `cvxportfolio-0.3.4/cvxportfolio/errors.py` & `cvxportfolio-0.3.5/cvxportfolio/errors.py`

 * *Files identical despite different names*

### Comparing `cvxportfolio-0.3.4/cvxportfolio/estimator.py` & `cvxportfolio-0.3.5/cvxportfolio/estimator.py`

 * *Files 9% similar despite different names*

```diff
@@ -31,52 +31,57 @@
     the `super()` corresponding method. It can make sense to call it before
     some logic, after, or not calling it at all. Also, any subclass of this that uses
     logic defined here should be careful to put estimator subclasses at the class
     attribute level, so that the two methods defined here get called recursively
     on them.
     """
 
-    def values_in_time(self, **kwargs):
+    def _recursive_values_in_time(self, **kwargs):
         """Evaluates estimator at a point in time recursively on its sub-estimators.
 
         This function is called by Simulator classes on Policy classes
         returning the current trades list. Policy classes, if
         they contain internal estimators, should declare them as attributes
         and call this base function (via `super()`) before
         they do their internal computation. CvxpyExpression estimators
         should instead define this method to update their Cvxpy parameters.
         
         Once we finalize the interface all parameters will be listed here.
         """
         for _, subestimator in self.__dict__.items():
-            if hasattr(subestimator, "values_in_time"):
-                subestimator.values_in_time(**kwargs)
+            if hasattr(subestimator, "_recursive_values_in_time"):
+                subestimator._recursive_values_in_time(**kwargs)
+        if hasattr(self, "_values_in_time"):
+            self.current_value = self._values_in_time(**kwargs)
+            return self.current_value
 
 
 class PolicyEstimator(Estimator):
     """Base class for (most) estimators that are part of policy objects."""
     
 
-    def pre_evaluation(self, universe, backtest_times):
-        """Initialize estimator and its sub-estimators.
+    def _recursive_pre_evaluation(self, universe, backtest_times):
+        """Recursively initialize estimator tree for backtest.
 
         :param universe: names of assets to be traded 
         :type universe: pandas.Index
         :param backtest_times: times at which the estimator will be evaluated
         :type backtest_time: pandas.DatetimeIndex
         """
         for _, subestimator in self.__dict__.items():
-            if hasattr(subestimator, "pre_evaluation"):
-                subestimator.pre_evaluation(universe, backtest_times)
+            if hasattr(subestimator, "_recursive_pre_evaluation"):
+                subestimator._recursive_pre_evaluation(universe, backtest_times)
+        if hasattr(self, "_pre_evaluation"):
+            self._pre_evaluation(universe, backtest_times)
     
 
 class CvxpyExpressionEstimator(PolicyEstimator):
     """Base class for estimators that are Cvxpy expressions."""
 
-    def compile_to_cvxpy(self, w_plus, z, w_plus_minus_w_bm):
+    def _compile_to_cvxpy(self, w_plus, z, w_plus_minus_w_bm):
         """Compile term to cvxpy expression.
 
         This is called by a Policy class on its terms before the start of the backtest
         to compile its Cvxpy problem. If the Policy changes in time
         this is called at every time step.
 
         It can either return a scalar expression, in the case of objective terms,
@@ -97,91 +102,91 @@
         raise NotImplementedError
 
 
 class DataEstimator(PolicyEstimator):
     """Estimator of point-in-time values from internal `self.data`.
 
     It also implements logic to check that no `np.nan` are returned
-    by its `values_in_time` method, which is the way `cvxportfolio`
+    by its `_recursive_values_in_time` method, which is the way `cvxportfolio`
     objects use this class to get data.
 
     Args:
         data (object, pandas.Series, pandas.DataFrame): Data expressed
             preferably as pandas Series or DataFrame where the first
             index is a pandas.DateTimeIndex. Otherwise you can
-            pass a callable object which implements the values_in_time method
+            pass a callable object which implements the _recursive_values_in_time method
             (with the standard signature) and returns the corresponding value in time,
              or a constant float, numpy.array, or even pandas Series or DataFrame not
             indexed by time (e.g., a covariance matrix where both index and columns
             are the stock symbols).
         use_last_available_time (bool): if the pandas index exists
-            and is a pandas.DateTimeIndex you can instruct self.values_in_time
+            and is a pandas.DateTimeIndex you can instruct self._recursive_values_in_time
             to retrieve the last available value at time t by setting
             this to True. Default is False.
 
     """
 
     def __init__(self, data, use_last_available_time=False, allow_nans=False, 
         compile_parameter=False, non_negative=False, positive_semi_definite=False):
         self.data = data
         self.use_last_available_time = use_last_available_time
         self.allow_nans = allow_nans
         self.compile_parameter = compile_parameter
         self.non_negative = non_negative
         self.positive_semi_definite =positive_semi_definite
     
-    def pre_evaluation(self, universe, backtest_times):
-        # super().pre_evaluation(universe, backtest_times)
+    def _recursive_pre_evaluation(self, universe, backtest_times):
+        # super()._recursive_pre_evaluation(universe, backtest_times)
         if self.compile_parameter:
-            value = self.internal_values_in_time(t=backtest_times[0])
+            value = self.internal__recursive_values_in_time(t=backtest_times[0])
             self.parameter = cp.Parameter(value.shape if hasattr(value, "shape") else (), 
                 PSD=self.positive_semi_definite, nonneg=self.non_negative)
             
 
     def value_checker(self, result):
         """Ensure that only scalars or arrays without np.nan are returned.
 
         Args:
-            result (int, float, or np.array): data produced by self.values_in_time
+            result (int, float, or np.array): data produced by self._recursive_values_in_time
 
         Returns:
             result (int, float, or np.array): same data if no np.nan are present and type is correct
 
         Raises:
             cvxportfolio.MissingValuesError: if np.nan's are present in result
             cvxportfolio.DataError: if data is not in the right form
         """
 
         if np.isscalar(result):
             if np.isnan(result) and not self.allow_nans:
                 raise MissingValuesError(
-                    f"{self.__class__.__name__}.values_in_time result is a np.nan scalar."
+                    f"{self.__class__.__name__}._recursive_values_in_time result is a np.nan scalar."
                 )
             else:
                 return result
 
         if isinstance(result, np.ndarray):
             if np.any(np.isnan(result)) and not self.allow_nans:
-                message = f"{self.__class__.__name__}.values_in_time result is an array with np.nan's."
+                message = f"{self.__class__.__name__}._recursive_values_in_time result is an array with np.nan's."
                 if hasattr(self.data, 'columns') and len(self.data.columns) == len(result):
                     message += "Specifically, the problem is with symbol(s): " + str(self.data.columns[np.isnan(result)])
                 raise MissingValuesError(message)
             else:
                 return result
 
         raise DataError(
-            f"{self.__class__.__name__}.values_in_time result is not a scalar or array."
+            f"{self.__class__.__name__}._recursive_values_in_time result is not a scalar or array."
         )
 
-    def internal_values_in_time(self, t, *args, **kwargs):
-        """Internal method called by `self.values_in_time`."""
+    def internal__recursive_values_in_time(self, t, *args, **kwargs):
+        """Internal method called by `self._recursive_values_in_time`."""
 
-        if hasattr(self.data, "values_in_time"):
+        if hasattr(self.data, "_recursive_values_in_time"):
             return self.value_checker(
-                self.data.values_in_time(
+                self.data._recursive_values_in_time(
                     t, *args, **kwargs))
 
         if (
             hasattr(self.data, "loc")
             and hasattr(self.data, "index")
             and (
                 isinstance(self.data.index, pd.DatetimeIndex)
@@ -205,45 +210,45 @@
                 if hasattr(tmp, "values"):
                     return self.value_checker(tmp.values)
                 else:
                     return self.value_checker(tmp)
 
             except (KeyError, IndexError):
                 raise MissingValuesError(
-                    f"{self.__class__.__name__}.values_in_time could not find data for requested time."
+                    f"{self.__class__.__name__}._recursive_values_in_time could not find data for requested time."
                 )
 
         if hasattr(self.data, "values"):
             return self.value_checker(self.data.values)
 
         return self.value_checker(self.data)
 
-    def values_in_time(self, t, *args, **kwargs):
+    def _recursive_values_in_time(self, t, *args, **kwargs):
         """Obtain value of `self.data` at time t or right before.
 
         Args:
             t (pandas.TimeStamp): time at which we evaluate the estimator
 
         Returns:
             result (float, numpy.array): if you use a callable object make
                 sure that it returns a float or numpy array (and not,
                 for example, a pandas object)
 
         """
-        self.current_value = self.internal_values_in_time(t, *args, **kwargs)
+        self.current_value = self.internal__recursive_values_in_time(t, *args, **kwargs)
         # we do this because in some cases they never get compiled
         if hasattr(self, 'parameter'): 
             self.parameter.value = self.current_value
         return self.current_value
 
 
 # class ConstantEstimator(cvxpy.Constant, DataEstimator):
 #     """Cvxpy constant that uses the pre_evalution method to be initialized."""
 #
-#     def pre_evaluation(self, returns, volumes, start_time, end_time, **kwargs):
+#     def _recursive_pre_evaluation(self, returns, volumes, start_time, end_time, **kwargs):
 #         """You should call super().__init__ it here."""
 #         raise NotImplementedError
 
 
 # class KnownData(DataEstimator):
 #     """Data known beforehand to use in backtest.
 #
@@ -262,16 +267,16 @@
 #     :raises MissingValueError: if data retrieved at a point in time contains nan's
 #     """
 #
 #     def __init__(self, data, use_last_available_time=False):
 #         self.data = data
 #         self.use_last_available_time = use_last_available_time
 #
-#     def values_in_time(self, t, **kwargs):
-#         self.value = self.internal_values_in_time(t, *args, **kwargs)
+#     def _recursive_values_in_time(self, t, **kwargs):
+#         self.value = self.internal__recursive_values_in_time(t, *args, **kwargs)
 #
 #
 # class KnownDataParameter(KnownData):
 #     """Data known beforehand to use in backtest as Cvxpy parameter.
 #
 #     :param data: user-provided data (known beforehand) in the form of time-indexed
 #         Series or DataFrame (points-in-time are used in the backtest),
@@ -298,22 +303,22 @@
 #     """
 #
 #     def __init__(self, data, positive_semi_definite=False, non_negative=False, **kwargs):
 #         super().__init__(data, **kwargs)
 #         self.positive_semi_definite = positive_semi_definite
 #         self.non_negative = non_negative
 #
-#     def pre_evaluation(self, universe, backtest_times):
-#         value = super().internal_values_in_time(t=backtest_times[0])
+#     def _recursive_pre_evaluation(self, universe, backtest_times):
+#         value = super().internal__recursive_values_in_time(t=backtest_times[0])
 #         self.parameter = cp.Parameter(
 #             value if hasattr(value, "shape") else (),
 #             PSD=self.positive_semi_definite, nonneg=self.non_negative)
 #
-#     def values_in_time(self, t, **kwargs):
-#         self.parameter.value = self.internal_values_in_time(t, **kwargs)
+#     def _recursive_values_in_time(self, t, **kwargs):
+#         self.parameter.value = self.internal__recursive_values_in_time(t, **kwargs)
         
         
 #
 # class ParameterEstimator(DataEstimator):
 #     def __init__(self, *args, **kwargs):
 #         super().__init__(self, *args, compile_parameter=True, **kwargs)
         
@@ -332,17 +337,17 @@
 #         self.positive_semi_definite = positive_semi_definite
 #         self.non_negative = non_negative
 #         self.use_last_available_time = use_last_available_time
 #         self.data = data
 #         self.allow_nans = allow_nans
 #         # super(DataEstimator).__init__(data, use_last_available_time)
 #
-#     def pre_evaluation(self, universe, backtest_times):
+#     def _recursive_pre_evaluation(self, universe, backtest_times):
 #         """Use the start time of the simulation to initialize the Parameter."""
-#         super().pre_evaluation(universe, backtest_times)
-#         value = super().values_in_time(t=backtest_times[0])
+#         super()._recursive_pre_evaluation(universe, backtest_times)
+#         value = super()._recursive_values_in_time(t=backtest_times[0])
 #         super().__init__(value.shape if hasattr(value, "shape") else (),
 #             PSD=self.positive_semi_definite, nonneg=self.non_negative)
 #
-#     def values_in_time(self, t, **kwargs):
+#     def _recursive_values_in_time(self, t, **kwargs):
 #         """Update Cvxpy Parameter value."""
-#         self.value = super().values_in_time(t=t, **kwargs)
+#         self.value = super()._recursive_values_in_time(t=t, **kwargs)
```

### Comparing `cvxportfolio-0.3.4/cvxportfolio/forecast.py` & `cvxportfolio-0.3.5/cvxportfolio/forecast.py`

 * *Files 14% similar despite different names*

```diff
@@ -22,63 +22,63 @@
 from dataclasses import dataclass
 
 import numpy as np
 
 from .estimator import PolicyEstimator
 
 
-def online_cache(values_in_time):
-    """A simple online cache that decorates values_in_time.
+def online_cache(_values_in_time):
+    """A simple online cache that decorates _values_in_time.
     
     The instance it is used on needs to be hashable (we currently
     use the hash of its __repr__ via dataclass).
     """
     
     def wrapped(self, t, cache=None, **kwargs):
         
         if cache is None: # temporary to not change tests
             cache = {}
             
         if not (self in cache):
             cache[self] = {}
         
         if t in cache[self]:
-            logging.debug(f'{self}.values_in_time at time {t} is retrieved from cache.')
-            self.current_value = cache[self][t]
+            logging.debug(f'{self}._values_in_time at time {t} is retrieved from cache.')
+            result = cache[self][t]
         else:
-            logging.debug(f'{self}.values_in_time at time {t} is stored in cache.')
-            values_in_time(self, t=t, cache=cache, **kwargs)  
-            cache[self][t] = self.current_value
-        return self.current_value
+            logging.debug(f'{self}._values_in_time at time {t} is stored in cache.')
+            result = _values_in_time(self, t=t, cache=cache, **kwargs)  
+            cache[self][t] = result
+        return result
         
     return wrapped
 
 class BaseForecast(PolicyEstimator):
     """Base class for forecasters."""
     
-    # def pre_evaluation(self, universe, backtest_times):
+    # def _recursive_pre_evaluation(self, universe, backtest_times):
     #     self.universe = universe
     #     self.backtest_times = backtest_times
     #
     
     
-    def update_chooser(self, t, past_returns):
+    def _agnostic_update(self, t, past_returns):
         """Choose whether to make forecast from scratch or update last one."""
         if (self.last_time is None) or (self.last_time != past_returns.index[-1]):
-            logging.debug(f'{self}.values_in_time at time {t} is computed from scratch.')
-            self.compute_from_scratch(t=t, past_returns=past_returns)
+            logging.debug(f'{self}._recursive_values_in_time at time {t} is computed from scratch.')
+            self._initial_compute(t=t, past_returns=past_returns)
         else:
-            logging.debug(f'{self}.values_in_time at time {t} is updated from previous value.')
-            self.update(t=t, past_returns=past_returns)
+            logging.debug(f'{self}._recursive_values_in_time at time {t} is updated from previous value.')
+            self._online_update(t=t, past_returns=past_returns)
             
-    def compute_from_scratch(self, t, past_returns):
+    def _initial_compute(self, t, past_returns):
         """Make forecast from scratch."""
         raise NotImplementedError
 
-    def update(self, t, past_returns):
+    def _online_update(self, t, past_returns):
         """Update forecast from period before."""
         raise NotImplementedError
 
 @dataclass(unsafe_hash=True)
 class HistoricalMeanReturn(BaseForecast):
     r"""Historical mean returns.
     
@@ -86,30 +86,28 @@
     """
          
     def __post_init__(self):
         self.last_time = None
         self.last_counts = None
         self.last_sum = None
         
-    def pre_evaluation(self, universe, backtest_times):
+    def _pre_evaluation(self, universe, backtest_times):
         self.__post_init__()
     
-    def values_in_time(self, t, past_returns, cache=None, **kwargs):
-        super().values_in_time(t=t, past_returns=past_returns, cache=cache, **kwargs)
-        self.update_chooser(t=t, past_returns=past_returns)
-        self.current_value = (self.last_sum / self.last_counts).values        
-        return self.current_value
+    def _values_in_time(self, t, past_returns, cache=None, **kwargs):
+        self._agnostic_update(t=t, past_returns=past_returns)
+        return (self.last_sum / self.last_counts).values        
         
-    def compute_from_scratch(self, t, past_returns):
+    def _initial_compute(self, t, past_returns):
         """Make forecast from scratch."""
         self.last_counts = past_returns.iloc[:, :-1].count()
         self.last_sum = past_returns.iloc[:, :-1].sum()
         self.last_time = t
         
-    def update(self, t, past_returns):
+    def _online_update(self, t, past_returns):
         """Update forecast from period before."""
         self.last_counts += ~(past_returns.iloc[-1, :-1].isnull())
         self.last_sum += past_returns.iloc[-1, :-1].fillna(0.)
         self.last_time = t
 
         
 class HistoricalMeanError(BaseForecast):
@@ -119,18 +117,16 @@
     :math:`\sqrt{\text{Var}[r]/t}`. When there are missing values we ignore them,
     both to compute the variance and the count.
     """
 
     def __init__(self):
         self.varianceforecaster = HistoricalVariance(kelly=False)
     
-    def values_in_time(self, t, past_returns, **kwargs):
-        super().values_in_time(t=t, past_returns=past_returns, **kwargs)
-        self.current_value  = np.sqrt(self.varianceforecaster.current_value / self.varianceforecaster.last_counts.values)
-        return self.current_value  
+    def _values_in_time(self, t, past_returns, **kwargs):
+        return np.sqrt(self.varianceforecaster.current_value / self.varianceforecaster.last_counts.values)
         
         
 @dataclass(unsafe_hash=True)
 class HistoricalVariance(BaseForecast):
     r"""Historical variances of non-cash returns.
     
     :param kelly: if ``True`` compute :math:`\mathbf{E}[r^2]`, else
@@ -145,31 +141,30 @@
     def __post_init__(self):
         if not self.kelly:
             self.meanforecaster = HistoricalMeanReturn()
         self.last_time = None
         self.last_counts = None
         self.last_sum = None
         
-    def pre_evaluation(self, universe, backtest_times):
+    def _pre_evaluation(self, universe, backtest_times):
         self.__post_init__()
     
-    def values_in_time(self, t, past_returns, **kwargs):
-        super().values_in_time(t=t, past_returns=past_returns, **kwargs)
-        self.update_chooser(t=t, past_returns=past_returns)
-        self.current_value = (self.last_sum / self.last_counts).values
+    def _values_in_time(self, t, past_returns, **kwargs):
+        self._agnostic_update(t=t, past_returns=past_returns)
+        result = (self.last_sum / self.last_counts).values
         if not self.kelly:
-            self.current_value -= self.meanforecaster.current_value**2
-        return self.current_value  
+            result -= self.meanforecaster.current_value**2
+        return result
         
-    def compute_from_scratch(self, t, past_returns):
+    def _initial_compute(self, t, past_returns):
         self.last_counts = past_returns.iloc[:, :-1].count()
         self.last_sum = (past_returns.iloc[:, :-1]**2).sum()
         self.last_time = t
         
-    def update(self, t, past_returns): #, last_estimation, last_counts, last_time):
+    def _online_update(self, t, past_returns): #, last_estimation, last_counts, last_time):
         self.last_counts += ~(past_returns.iloc[-1, :-1].isnull())
         self.last_sum += past_returns.iloc[-1, :-1].fillna(0.)**2
         self.last_time = t
 
 
 @dataclass(unsafe_hash=True)
 class HistoricalFactorizedCovariance(BaseForecast):
@@ -184,67 +179,65 @@
     """
     
     kelly: bool = True
     
     def __post_init__(self):
         self.last_time = None
     
-    def pre_evaluation(self, universe, backtest_times):
+    def _pre_evaluation(self, universe, backtest_times):
         self.__post_init__()
     
     @staticmethod
-    def get_count_matrix(past_returns):
+    def _get_count_matrix(past_returns):
         r"""We obtain the matrix of non-null joint counts:
         
         .. math::
         
             \text{Count}\left(r^{i}r^{j} \neq \texttt{nan}\right).
         """
         tmp = (~past_returns.iloc[:,:-1].isnull()) * 1.
         return tmp.T @ tmp
     
     @staticmethod
-    def get_initial_joint_mean(past_returns):
+    def _get_initial_joint_mean(past_returns):
         r"""Compute precursor of :math:`\Sigma_{i,j} = \mathbf{E}[r^{i}]\mathbf{E}[r^{j}]`.
         """
         nonnull = (~past_returns.iloc[:,:-1].isnull()) * 1.
         tmp = nonnull.T @ past_returns.iloc[:,:-1].fillna(0.)
         return tmp # * tmp.T
 
     @staticmethod
-    def factorize(Sigma):
+    def _factorize(Sigma):
         """Factorize matrix and remove negative eigenvalues."""
         eigval, eigvec = np.linalg.eigh(Sigma)
         eigval = np.maximum(eigval, 0.)
         return eigvec @ np.diag(np.sqrt(eigval))
         
-    def compute_from_scratch(self, t, past_returns):
-        self.last_counts_matrix = self.get_count_matrix(past_returns).values
+    def _initial_compute(self, t, past_returns):
+        self.last_counts_matrix = self._get_count_matrix(past_returns).values
         filled = past_returns.iloc[:,:-1].fillna(0.).values
         self.last_sum_matrix = filled.T @ filled
         if not self.kelly:
-            self.joint_mean = self.get_initial_joint_mean(past_returns)
+            self.joint_mean = self._get_initial_joint_mean(past_returns)
 
         self.last_time = t
         
-    def update(self, t, past_returns):
+    def _online_update(self, t, past_returns):
         nonnull = ~(past_returns.iloc[-1, :-1].isnull())
         self.last_counts_matrix += np.outer(nonnull, nonnull)
         last_ret = past_returns.iloc[-1, :-1].fillna(0.)
         self.last_sum_matrix += np.outer(last_ret, last_ret)
         self.last_time = t
         if not self.kelly:
             self.joint_mean += last_ret
 
     @online_cache
-    def values_in_time(self, t, past_returns, **kwargs):
-        super().values_in_time(t=t, past_returns=past_returns, **kwargs)
+    def _values_in_time(self, t, past_returns, **kwargs):
   
-        self.update_chooser(t=t, past_returns=past_returns)
+        self._agnostic_update(t=t, past_returns=past_returns)
         Sigma = self.last_sum_matrix / self.last_counts_matrix
         
         if not self.kelly:
             tmp = self.joint_mean / self.last_counts_matrix
             Sigma -= tmp.T * tmp
                
-        self.current_value = self.factorize(Sigma) 
-        return self.current_value
+        return self._factorize(Sigma)
```

### Comparing `cvxportfolio-0.3.4/cvxportfolio/policies.py` & `cvxportfolio-0.3.5/cvxportfolio/policies.py`

 * *Files 5% similar despite different names*

```diff
@@ -49,15 +49,15 @@
 class BaseTradingPolicy(PolicyEstimator):
     """Base class for a trading policy."""
 
 
 class Hold(BaseTradingPolicy):
     """Hold initial portfolio, don't trade."""
 
-    def values_in_time(self, current_weights, **kwargs):
+    def _values_in_time(self, current_weights, **kwargs):
         """Update sub-estimators and produce current estimate."""
         return pd.Series(0., index=current_weights.index)
 
 
 class RankAndLongShort(BaseTradingPolicy):
     """Rank assets by signal; long highest and short lowest.
 
@@ -79,17 +79,16 @@
     def __init__(self, signal, num_long=1, num_short=1, target_leverage=1.):
         """Define sub-estimators at class attribute level."""
         self.num_long = DataEstimator(num_long)
         self.num_short = DataEstimator(num_short)
         self.signal = DataEstimator(signal)
         self.target_leverage = DataEstimator(target_leverage)
 
-    def values_in_time(self, t, current_weights, **kwargs):
+    def _values_in_time(self, t, current_weights, **kwargs):
         """Update sub-estimators and produce current estimate."""
-        super().values_in_time(t=t, current_weights=current_weights, **kwargs)
 
         sorted_ret = pd.Series(
             self.signal.current_value, current_weights.index[:-1]
         ).sort_values()
         short_positions = sorted_ret.index[: self.num_short.current_value]
         long_positions = sorted_ret.index[-self.num_long.current_value:]
 
@@ -119,43 +118,39 @@
             given points in time (e.g., start of each month).
 
     """
 
     def __init__(self, targets):
         self.targets = targets
 
-    def pre_evaluation(self, universe, backtest_times):
+    def _pre_evaluation(self, universe, backtest_times):
         """Get list of trading days."""
         self.trading_days = backtest_times
-        super().pre_evaluation(universe, backtest_times)
 
-    def values_in_time(self, t, current_weights, **kwargs):
+    def _values_in_time(self, t, current_weights, **kwargs):
         """Get current trade weights."""
-        super().values_in_time(t=t, current_weights=current_weights, **kwargs)
         next_targets = self.targets.loc[self.targets.index >= t]
         assert np.allclose(next_targets.sum(1), 1.)
         if not len(next_targets):
             return pd.Series(0., index=current_weights.index)
         next_target = next_targets.iloc[0]
         next_target_day = next_targets.index[0]
         trading_days_to_target = len(self.trading_days[(
             self.trading_days >= t) & (self.trading_days < next_target_day)])
         return (next_target - current_weights) / (trading_days_to_target + 1)
 
 
 class SellAll(BaseTradingPolicy):
     """Sell all assets to cash.
 
-    This is useful to check the tcost model in the simulator,
-    or as an element in a (currently not implemented) composite policy.
+    This is useful to check the tcost model in the simulator.
     """
 
-    def values_in_time(self, t, current_weights, **kwargs):
+    def _values_in_time(self, t, current_weights, **kwargs):
         """Get current trade weights."""
-        super().values_in_time(t=t, current_weights=current_weights, **kwargs)
         target = np.zeros(len(current_weights))
         target[-1] = 1.
         return target - current_weights
 
 
 class FixedTrades(BaseTradingPolicy):
     """Each day trade the provided trade weights vector.
@@ -169,17 +164,18 @@
             indexed by time. It trades each day the corresponding vector.
     """
 
     def __init__(self, trades_weights):
         """Trade the tradevec vector (dollars) or tradeweight weights."""
         self.trades_weights = DataEstimator(trades_weights)
 
-    def values_in_time(self, t, current_weights, **kwargs):
+    def _recursive_values_in_time(self, t, current_weights, **kwargs):
+        """We need to override recursion b/c we catch exception."""
         try:
-            super().values_in_time(t=t, current_weights=current_weights, **kwargs)
+            super()._recursive_values_in_time(t=t, current_weights=current_weights, **kwargs)
             return pd.Series(
                 self.trades_weights.current_value,
                 current_weights.index)
         except MissingValuesError:
             return pd.Series(0., current_weights.index)
 
 
@@ -195,30 +191,31 @@
             indexed by time. It trades each day to the corresponding vector.
     """
 
     def __init__(self, target_weights):
         """Trade the tradevec vector (dollars) or tradeweight weights."""
         self.target_weights = DataEstimator(target_weights)
 
-    def values_in_time(self, t, current_weights, **kwargs):
+    def _recursive_values_in_time(self, t, current_weights, **kwargs):
+        """We need to override recursion b/c we catch exception."""
         try:
-            super().values_in_time(t=t, current_weights=current_weights, **kwargs)
+            super()._recursive_values_in_time(t=t, current_weights=current_weights, **kwargs)
             return pd.Series(self.target_weights.current_value,
                     current_weights.index) - current_weights
         except MissingValuesError:
             return pd.Series(0., current_weights.index)
             
             
 class Uniform(FixedWeights):
     """Uniform allocation on non-cash assets."""
     
     def __init__(self):
         pass
     
-    def pre_evaluation(self, universe, backtest_times):
+    def _pre_evaluation(self, universe, backtest_times):
         target_weights = pd.Series(1., universe)
         target_weights.iloc[-1] = 0
         target_weights /= sum(target_weights)
         self.target_weights = DataEstimator(target_weights)
 
 
 class PeriodicRebalance(FixedWeights):
@@ -277,27 +274,26 @@
     
     """
 
     def __init__(self, target, tracking_error):
         self.target = DataEstimator(target)
         self.tracking_error = DataEstimator(tracking_error)
 
-    def values_in_time(self, t, current_weights, **kwargs):
-        super().values_in_time(t=t, current_weights=current_weights, **kwargs)
+    def _values_in_time(self, t, current_weights, **kwargs):
         if np.linalg.norm(current_weights - self.target.current_value) > \
           self.tracking_error.current_value:
             return self.target.current_value - current_weights
         else:
             return pd.Series(0., current_weights.index)
 
 
 
 
 class MultiPeriodOptimization(BaseTradingPolicy):
-    """Multi Period Optimization policy.
+    r"""Multi Period Optimization policy.
 
     Implements the model developed in Chapter 5, in particular
     at page 49, of the book. You specify the objective terms
     using classes such as ReturnsForecast and TcostModel, each
     multiplied by its multiplier. You also specify lists
     of constraints. There are two ways to do it. You either
     define the same objective terms and costraints for each 
@@ -307,34 +303,44 @@
     simply impose that at the last step in the optimization the
     post-trade weights match the given weights (see page 51).
     
     When it computes the trajectory of weights for the future
     it only returns the first step (to the Simulator, typically).
     The future steps (planning horizon) are by default not returned.
 
-    Args:
-        objective (algebra of BaseCost or list of those): these will be maximized;
-            if you pass a single expression of BaseCost it is understood as the 
-            same for all steps; if it's a list you must also pass a list of lists
-            for `constraints`, each term represents the cost for each step of the optimization
-            (starting from the first, i.e., today) and the length of the list is 
-            used as planning_horizon (the value you pass there will be ignored) 
-        constraints (list of BaseConstraints or list of those): these will be
-            imposed on the optimization. Default []. Pass this as a list of
-            lists of the same length as `objective` to specify different 
-            constraints at different time steps.
-        planning_horizon (int or None): how many steps in the future we 
-            plan for. Ignored if passing `objective` and `constraints` as lists.
-            Default is None.
-        terminal_constraint (pd.Series or None): if you pass a Series to this
-            (default is None) it will impose that at the last step of the multi
-            period optimization the post-trade weights are equal to this.
-        **kwargs: these will be passed to cvxpy.Problem.solve,
-            so you can choose your own solver and pass
-            parameters to it.
+    :param objective: these will be maximized;
+        if you pass a single expression of BaseCost it is understood as the 
+        same for all steps; if it's a list you must also pass a list of lists
+        for `constraints`, each term represents the cost for each step of the optimization
+        (starting from the first, i.e., today) and the length of the list is 
+        used as planning_horizon (the value you pass there will be ignored) 
+    :type objective: algebra of BaseCost or list of
+    :param constraints: these will be
+        imposed on the optimization. Default []. Pass this as a list of
+        lists of the same length as `objective` to specify different 
+        constraints at different time steps.
+    :type constraints: list of BaseConstraints or list of those
+    :param planning_horizon:  how many steps in the future we 
+        plan for. Ignored if passing `objective` and `constraints` as lists.
+        Default is None.
+    :type planning_horizon: int or None
+    :param terminal_constraint: if you pass a Series to this
+        (default is None) it will impose that at the last step of the multi
+        period optimization the post-trade weights are equal to this.
+    :type terminal_constraint: pd.Series or None
+    :param include_cash_return: whether to automatically include the ``CashReturn`` term in the objective,
+        with default parameters. Default is ``True``.
+    :type include_cash_return: bool
+    :param benchmark: benchmark weights to use in the risk model and other terms that need it. Implemented
+        ones are ``CashBenchmark``, the default, ``UniformBenchmark`` (uniform allocation on non-cash assets),
+        and ``MarketBenchmark``, which approximates the market-weighted portfolio.
+    :type benchmark: BaseBenchmark class or instance
+    :param \**kwargs: these will be passed to cvxpy.Problem.solve,
+        so you can choose your own solver and pass
+        parameters to it.
     """
 
     def __init__(self, objective, constraints=[], include_cash_return=True, planning_horizon=None, terminal_constraint=None, benchmark=CashBenchmark, **kwargs):
         if hasattr(objective, '__iter__'):
             if not (hasattr(constraints, '__iter__') and len(constraints) and (hasattr(constraints[0], '__iter__') and len(objective) == len(constraints))):
                 raise SyntaxError('If you pass objective as a list, constraints should be a list of lists of the same length.')
             self.planning_horizon = len(objective)
@@ -350,48 +356,48 @@
         self.include_cash_return = include_cash_return
         if self.include_cash_return:
             self.objective = [el + CashReturn() for el in self.objective]
         self.terminal_constraint = terminal_constraint
         self.benchmark = benchmark() if isinstance(benchmark, type) else benchmark
         self.cvxpy_kwargs = kwargs
 
-    def compile_to_cvxpy(self):#, w_plus, z, value):
+    def _compile_to_cvxpy(self):#, w_plus, z, value):
         """Compile all cvxpy expressions and the problem."""
         self.cvxpy_objective = [
-            el.compile_to_cvxpy(self.w_plus_at_lags[i], self.z_at_lags[i], self.w_plus_minus_w_bm_at_lags[i]) 
+            el._compile_to_cvxpy(self.w_plus_at_lags[i], self.z_at_lags[i], self.w_plus_minus_w_bm_at_lags[i]) 
             for i, el in enumerate(self.objective)]
         self.cvxpy_objective = sum(self.cvxpy_objective)
         assert self.cvxpy_objective.is_dcp()  # dpp=True)
         assert self.cvxpy_objective.is_concave()
         self.cvxpy_constraints = [
-            flatten_heterogeneous_list([constr.compile_to_cvxpy(self.w_plus_at_lags[i], self.z_at_lags[i], self.w_plus_minus_w_bm_at_lags[i]) 
+            flatten_heterogeneous_list([constr._compile_to_cvxpy(self.w_plus_at_lags[i], self.z_at_lags[i], self.w_plus_minus_w_bm_at_lags[i]) 
                 for constr in el])
             for i, el in enumerate(self.constraints)]
         self.cvxpy_constraints = sum(self.cvxpy_constraints, [])
         self.cvxpy_constraints += [cp.sum(z) == 0 for z in self.z_at_lags]
         w = self.w_current
         for i in range(self.planning_horizon):
             self.cvxpy_constraints.append(self.w_plus_at_lags[i] == self.z_at_lags[i] + w)
             self.cvxpy_constraints.append(self.w_plus_at_lags[i] - self.w_bm == self.w_plus_minus_w_bm_at_lags[i])
             w = self.w_plus_at_lags[i]
         if not self.terminal_constraint is None:
             self.cvxpy_constraints.append(w == self.terminal_constraint)
         self.problem = cp.Problem(cp.Maximize(self.cvxpy_objective), self.cvxpy_constraints)
         assert self.problem.is_dcp()  # dpp=True)
 
-    def pre_evaluation(self, universe, backtest_times):
-        """Pass a full view of the data to initialize objects that need it."""
+    def _recursive_pre_evaluation(self, universe, backtest_times):
+        """No point in using recursive super() method."""
         
         for obj in self.objective:
-            obj.pre_evaluation(universe=universe, backtest_times=backtest_times)
+            obj._recursive_pre_evaluation(universe=universe, backtest_times=backtest_times)
         for constr_at_lag in self.constraints:
             for constr in constr_at_lag:
-                constr.pre_evaluation(universe=universe, backtest_times=backtest_times)
+                constr._recursive_pre_evaluation(universe=universe, backtest_times=backtest_times)
         
-        self.benchmark.pre_evaluation(universe=universe, backtest_times=backtest_times)
+        self.benchmark._recursive_pre_evaluation(universe=universe, backtest_times=backtest_times)
         self.w_bm = cp.Parameter(len(universe))
 
         # temporary
         # self.w_bm = np.zeros(len(universe))
         # self.w_bm[-1] = 1.
         
         # initialize the problem
@@ -400,38 +406,37 @@
         self.z_at_lags = [cp.Variable(len(universe)) for i in range(self.planning_horizon)] 
         self.w_plus_at_lags = [cp.Variable(len(universe)) for i in range(self.planning_horizon)]
         self.w_plus_minus_w_bm_at_lags = [cp.Variable(len(universe)) for i in range(self.planning_horizon)]
 
         # simulator will overwrite this with cached loaded from disk
         self.cache = {}
 
-        # self.compile_to_cvxpy()#self.w_plus, self.z, self.portfolio_value)
+        # self._compile_to_cvxpy()#self.w_plus, self.z, self.portfolio_value)
         
 
-
-    def values_in_time(self, t, current_weights, current_portfolio_value, past_returns, past_volumes, current_prices, **kwargs):
+    def _recursive_values_in_time(self, t, current_weights, current_portfolio_value, past_returns, past_volumes, current_prices, **kwargs):
         """Update all cvxpy parameters and solve."""
         
         assert current_portfolio_value > 0
         assert np.isclose(sum(current_weights), 1)
                 
         for i, obj in enumerate(self.objective):
-            obj.values_in_time(t=t, current_weights=current_weights, 
+            obj._recursive_values_in_time(t=t, current_weights=current_weights, 
                     current_portfolio_value=current_portfolio_value, 
                     past_returns=past_returns, past_volumes=past_volumes, 
                     current_prices=current_prices, mpo_step=i, cache=self.cache, **kwargs)     
                      
         for i, constr_at_lag in enumerate(self.constraints):
             for constr in constr_at_lag:
-                constr.values_in_time(t=t, current_weights=current_weights, 
+                constr._recursive_values_in_time(t=t, current_weights=current_weights, 
                     current_portfolio_value=current_portfolio_value, 
                     past_returns=past_returns, past_volumes=past_volumes, 
                     current_prices=current_prices, mpo_step=i, cache=self.cache, **kwargs)   
                     
-        self.benchmark.values_in_time(t=t, current_weights=current_weights, 
+        self.benchmark._recursive_values_in_time(t=t, current_weights=current_weights, 
                     current_portfolio_value=current_portfolio_value, 
                     past_returns=past_returns, past_volumes=past_volumes, 
                     current_prices=current_prices, mpo_step=i, cache=self.cache, **kwargs) 
                     
         self.w_bm.value = self.benchmark.current_value
 
         # self.portfolio_value.value = 1. # not used current_portfolio_value
@@ -453,27 +458,34 @@
             )
 
         return pd.Series(self.z_at_lags[0].value, current_weights.index)
 
 
     
 class SinglePeriodOptimization(MultiPeriodOptimization):
-    """Single Period Optimization policy.
+    r"""Single Period Optimization policy.
 
     Implements the model developed in Chapter 4, in particular
     at page 43, of the book. You specify the objective term
     using classes such as ReturnsForecast and TcostModel, each
     multiplied by its multiplier. You also specify a list
     of constraints.
 
     :param objective: this algebraic combination of cvxportfolio cost objects will be maximized
     :type objective: CombinedCost
     :param constraints: these will be imposed on the optimization. Default [].
     :type constraints: list of BaseConstraints
-    :param **kwargs: these will be passed to cvxpy.Problem.solve, so you can choose your own solver and pass
+    :param include_cash_return: whether to automatically include the ``CashReturn`` term in the objective,
+        with default parameters. Default is ``True``.
+    :type include_cash_return: bool
+    :param benchmark: benchmark weights to use in the risk model and other terms that need it. Implemented
+        ones are ``CashBenchmark``, the default, ``UniformBenchmark`` (uniform allocation on non-cash assets),
+        and ``MarketBenchmark``, which approximates the market-weighted portfolio.
+    :type benchmark: BaseBenchmark class or instance
+    :param \**kwargs: these will be passed to cvxpy.Problem.solve, so you can choose your own solver and pass
         parameters to it.
     """
 
     def __init__(self, objective, constraints=[], include_cash_return=True, benchmark=CashBenchmark, **kwargs):
         super().__init__([objective], [constraints], include_cash_return=include_cash_return, 
             benchmark=benchmark, **kwargs)
```

### Comparing `cvxportfolio-0.3.4/cvxportfolio/result.py` & `cvxportfolio-0.3.5/cvxportfolio/result.py`

 * *Files identical despite different names*

### Comparing `cvxportfolio-0.3.4/cvxportfolio/returns.py` & `cvxportfolio-0.3.5/cvxportfolio/returns.py`

 * *Files 6% similar despite different names*

```diff
@@ -55,29 +55,27 @@
     """
     
     def __init__(self, cash_returns=None, short_margin_requirement=1.):
         self.cash_returns = None if cash_returns is None else DataEstimator(cash_returns, 
             compile_parameter=True, non_negative=True)
         self.short_margin_requirement = short_margin_requirement
         
-    def pre_evaluation(self, universe, backtest_times):
-        super().pre_evaluation(universe, backtest_times)
+    def _pre_evaluation(self, universe, backtest_times):
         self.cash_return_parameter = cp.Parameter(nonneg=True) if self.cash_returns is None \
             else self.cash_returns.parameter
             
         # else DataEstimator(self.cash_returns, non_negative=True, compile_parameter=True)
         
         
-    def values_in_time(self, t, past_returns, **kwargs):
+    def _values_in_time(self, t, past_returns, **kwargs):
         """Update cash return parameter as last cash return."""
-        super().values_in_time(t=t, past_returns=past_returns, **kwargs)
         if self.cash_returns is None:
             self.cash_return_parameter.value = past_returns.iloc[-1,-1]
         
-    def compile_to_cvxpy(self, w_plus, z, w_plus_minus_w_bm):
+    def _compile_to_cvxpy(self, w_plus, z, w_plus_minus_w_bm):
         """Apply cash return to "real" cash position (without shorts and margins)."""
         realcash = (w_plus[-1] - (1 + self.short_margin_requirement) * cp.sum(cp.neg(w_plus[:-1])))
         result = realcash * self.cash_return_parameter
         assert result.is_concave()
         return result
         
     
@@ -145,23 +143,21 @@
         
         if not r_hat is None:
             self.r_hat = DataEstimator(r_hat)
         else:
             self.r_hat = HistoricalMeanReturn()
         self.decay = decay
         
-    def pre_evaluation(self, universe, backtest_times):
-        super().pre_evaluation(universe=universe, backtest_times=backtest_times)
+    def _pre_evaluation(self, universe, backtest_times):
         self.r_hat_parameter = cp.Parameter(len(universe)-1)
         
-    def values_in_time(self, t, past_returns, mpo_step=0, **kwargs):
-        super().values_in_time(t=t, past_returns=past_returns, mpo_step=mpo_step, **kwargs)
+    def _values_in_time(self, t, past_returns, mpo_step=0, **kwargs):
         self.r_hat_parameter.value = self.r_hat.current_value * self.decay**(mpo_step)
 
-    def compile_to_cvxpy(self, w_plus, z, w_plus_minus_w_bm):
+    def _compile_to_cvxpy(self, w_plus, z, w_plus_minus_w_bm):
         """Cvxpy expression acts on non-cash assets."""
         return w_plus[:-1].T @ self.r_hat_parameter 
         
 
 
 class ReturnsForecastError(BaseRiskModel):
     """Simple return forecast error risk with values provided by the user.
@@ -184,24 +180,21 @@
     def __init__(self, deltas=None):
         
         if not deltas is None:
             self.deltas = DataEstimator(deltas)
         else:
             self.deltas = HistoricalMeanError()
             
-    def pre_evaluation(self, universe, backtest_times):
-        super().pre_evaluation(universe=universe, backtest_times=backtest_times)
+    def _pre_evaluation(self, universe, backtest_times):
         self.deltas_parameter = cp.Parameter(len(universe)-1, nonneg=True)
 
 
-    def values_in_time(self, t, past_returns, **kwargs):
-        super().values_in_time(t=t, past_returns=past_returns, **kwargs)
+    def _values_in_time(self, t, past_returns, **kwargs):
         self.deltas_parameter.value = self.deltas.current_value
 
-
-    def compile_to_cvxpy(self, w_plus, z, w_plus_minus_w_bm):
+    def _compile_to_cvxpy(self, w_plus, z, w_plus_minus_w_bm):
         """Compile to cvxpy expression."""
         return cp.abs(w_plus_minus_w_bm[:-1]).T @ self.deltas_parameter
```

### Comparing `cvxportfolio-0.3.4/cvxportfolio/risks.py` & `cvxportfolio-0.3.5/cvxportfolio/risks.py`

 * *Files 3% similar despite different names*

```diff
@@ -117,32 +117,29 @@
         if not Sigma is None:
             self.Sigma = DataEstimator(Sigma)
             self.alreadyfactorized = False
         else:
             self.Sigma = HistoricalFactorizedCovariance(kelly=kelly) 
             self.alreadyfactorized = True
             
-    def pre_evaluation(self, universe, backtest_times):
-        super().pre_evaluation(universe, backtest_times)
-        
+    def _pre_evaluation(self, universe, backtest_times):
         self.Sigma_sqrt = cp.Parameter((len(universe)-1, len(universe)-1))
 
-    def values_in_time(self, t, past_returns, **kwargs):
+    def _values_in_time(self, t, past_returns, **kwargs):
         """Update forecast error risk here, and take square root of Sigma."""
-        super().values_in_time(t=t, past_returns=past_returns, **kwargs)
         
         if self.alreadyfactorized:
             self.Sigma_sqrt.value = self.Sigma.current_value
         else:
             Sigma = self.Sigma.current_value
             eigval, eigvec = np.linalg.eigh(Sigma)
             eigval = np.maximum(eigval, 0.)
             self.Sigma_sqrt.value = eigvec @ np.diag(np.sqrt(eigval))
 
-    def compile_to_cvxpy(self, w_plus, z, w_plus_minus_w_bm):
+    def _compile_to_cvxpy(self, w_plus, z, w_plus_minus_w_bm):
         self.cvxpy_expression = cp.sum_squares(self.Sigma_sqrt.T @ w_plus_minus_w_bm[:-1])
         return self.cvxpy_expression
 
 class RiskForecastError(BaseRiskModel):
     """Risk forecast error. 
     
     Implements the model defined in page 31 of the book. Takes same arguments
@@ -158,21 +155,19 @@
             self.sigma_squares = HistoricalVariance(kelly=True) #None None
         else:
             self.sigma_squares = DataEstimator(sigma_squares)
         # self.standard_deviations = ParameterEstimator(standard_deviations)
         # self.zeroforcash=True
         # self.kelly=True
         
-    def pre_evaluation(self, universe, backtest_times):
-        super().pre_evaluation(universe, backtest_times)
+    def _pre_evaluation(self, universe, backtest_times):
         self.sigmas_parameter = cp.Parameter(len(universe)-1, nonneg=True)#+self.kelly))
 
-    def values_in_time(self, t, past_returns, **kwargs):
+    def _values_in_time(self, t, past_returns, **kwargs):
         """Update forecast error risk here, and take square root of Sigma."""
-        super().values_in_time(t=t, past_returns=past_returns)
         
         # if self.sigma_squares is None:
         #     sigma_squares = past_returns.var(ddof=0)
         #     if self.kelly:
         #         mean = past_returns.mean()
         #         sigma_squares += mean**2
         #     if self.zeroforcash:
@@ -181,15 +176,15 @@
         # else:
         #     sigma_squares = self.sigma_squares.current_value
             
         sigma_squares = self.sigma_squares.current_value
         
         self.sigmas_parameter.value = np.sqrt(sigma_squares)
 
-    def compile_to_cvxpy(self, w_plus, z, w_plus_minus_w_bm):
+    def _compile_to_cvxpy(self, w_plus, z, w_plus_minus_w_bm):
 
         return cp.square(cp.abs(w_plus_minus_w_bm[:-1]).T @ self.sigmas_parameter)
                 
 
 class DiagonalCovariance(BaseRiskModel):
     """Diagonal covariance matrix, user-provided or fit from data.
 
@@ -203,22 +198,20 @@
             self.sigma_squares = DataEstimator(sigma_squares)
         else:
             self.sigma_squares = HistoricalVariance(kelly=True) #None
         #self.zeroforcash = True
         #self.kelly = True
         # self.standard_deviations = ParameterEstimator(standard_deviations)
         
-    def pre_evaluation(self, universe, backtest_times):
-        super().pre_evaluation(universe, backtest_times)
+    def _pre_evaluation(self, universe, backtest_times):
         self.sigmas_parameter = cp.Parameter(len(universe)-1) #+self.kelly))
 
-    def values_in_time(self, t, past_returns, **kwargs):
+    def _values_in_time(self, t, past_returns, **kwargs):
         """Update forecast error risk here, and take square root of Sigma."""
-        #super().values_in_time(t, current_weights, current_portfolio_value, past_returns, past_volumes, **kwargs)
-        super().values_in_time(t=t, past_returns=past_returns, **kwargs)
+        #super()._recursive_values_in_time(t, current_weights, current_portfolio_value, past_returns, past_volumes, **kwargs)
         
         # if self.sigma_squares is None:
         #     sigma_squares = past_returns.var(ddof=0)
         #     if self.kelly:
         #         mean = past_returns.mean()
         #         sigma_squares += mean**2
         #     if self.zeroforcash:
@@ -227,15 +220,15 @@
         # else:
         #     sigma_squares = self.sigma_squares.current_value
         
         sigma_squares = self.sigma_squares.current_value
 
         self.sigmas_parameter.value = np.sqrt(sigma_squares)
 
-    def compile_to_cvxpy(self, w_plus, z, w_plus_minus_w_bm):
+    def _compile_to_cvxpy(self, w_plus, z, w_plus_minus_w_bm):
 
         return cp.sum_squares(cp.multiply(w_plus_minus_w_bm[:-1], self.sigmas_parameter))
 
 
 class FactorModelCovariance(BaseRiskModel):
     """Factor model covariance, either user-provided or fitted from the data.
     
@@ -318,25 +311,23 @@
     #     else:
     #         F = pd.DataFrame(F.T, columns=normalizer.index)
     #     idyosyncratic = normalizer**2 - (F**2).sum(0)
     #     if not np.all(idyosyncratic >= 0.):
     #         raise ForeCastError("Low rank risk estimation with iterative SVD did not work.")
     #     return F, idyosyncratic
 
-    def pre_evaluation(self, universe, backtest_times):
-        super().pre_evaluation(universe, backtest_times)
-        # super().pre_evaluation(returns, volumes, start_time, end_time, **kwargs)
+    def _pre_evaluation(self, universe, backtest_times):
+        # super()._recursive_pre_evaluation(returns, volumes, start_time, end_time, **kwargs)
         self.idyosync_sqrt_parameter = cp.Parameter(len(universe)-1)
         self.F_parameter = cp.Parameter((self.num_factors, len(universe)-1)) if self.F is None else self.F.parameter
         # if not (self.factor_Sigma is None):
         #     self.factor_Sigma_sqrt = cp.Parameter(self.factor_Sigma.shape, PSD=True)
         # self.forecast_error_penalizer = cp.Parameter(returns.shape[1], nonneg=True)
 
-    def values_in_time(self, t, past_returns, **kwargs):
-        super().values_in_time(t=t, past_returns=past_returns, **kwargs)
+    def _values_in_time(self, t, past_returns, **kwargs):
         
         # if self.F is None:
         #     if not self.kelly:
         #         past_returns = past_returns - past_returns.mean()
         #     if self.zeroforcash:
         #         past_returns = pd.DataFrame(past_returns, copy=True)
         #         past_returns.iloc[:, -1] = 0.
@@ -351,15 +342,15 @@
             self.F_parameter.value = Sigmasqrt[:, -self.num_factors:].T
             d = (Sigmasqrt[:, :-self.num_factors]**2).sum(1)
         else:
             d = self.d.current_value
         self.idyosync_sqrt_parameter.value = np.sqrt(d)
 
 
-    def compile_to_cvxpy(self, w_plus, z, w_plus_minus_w_bm):
+    def _compile_to_cvxpy(self, w_plus, z, w_plus_minus_w_bm):
         self.expression = cp.sum_squares(cp.multiply(self.idyosync_sqrt_parameter, w_plus_minus_w_bm[:-1]))
         assert self.expression.is_dcp(dpp=True)
 
         self.expression += cp.sum_squares(self.F_parameter @ w_plus_minus_w_bm[:-1])
         assert self.expression.is_dcp(dpp=True)
 
         return self.expression
@@ -376,21 +367,21 @@
         risk.
     :type riskmodels: list 
     """
 
     def __init__(self, riskmodels):
         self.riskmodels = riskmodels
 
-    def pre_evaluation(self, universe, backtest_times):
+    def _recursive_pre_evaluation(self, universe, backtest_times):
         """Initialize objects."""
         for risk in self.riskmodels:
-            risk.pre_evaluation(universe, backtest_times)
+            risk._recursive_pre_evaluation(universe, backtest_times)
 
-    def values_in_time(self, **kwargs):
+    def _recursive_values_in_time(self, **kwargs):
         """Update parameters."""
         for risk in self.riskmodels:
-            risk.values_in_time(**kwargs)
+            risk._recursive_values_in_time(**kwargs)
 
-    def compile_to_cvxpy(self, w_plus, z, w_plus_minus_w_bm):
-        risks = [risk.compile_to_cvxpy(w_plus, z, w_plus_minus_w_bm)
+    def _compile_to_cvxpy(self, w_plus, z, w_plus_minus_w_bm):
+        risks = [risk._compile_to_cvxpy(w_plus, z, w_plus_minus_w_bm)
                  for risk in self.riskmodels]
         return cp.max(cp.hstack(risks))
```

### Comparing `cvxportfolio-0.3.4/cvxportfolio/simulator.py` & `cvxportfolio-0.3.5/cvxportfolio/simulator.py`

 * *Files 23% similar despite different names*

```diff
@@ -35,214 +35,86 @@
 from .data import FredTimeSeries, YfinanceTimeSeries, BASE_LOCATION
 from .estimator import Estimator, DataEstimator
 from .result import BacktestResult
 from .utils import *
 from .errors import DataError
 
 PPY = 252
-__all__ = ['MarketSimulator', #'simulate_cash_holding_cost', 'simulate_stocks_holding_cost', 'simulate_transaction_cost', 
-    'MarketData']
+__all__ = ['MarketSimulator']
 
     
-def hash_universe(universe):
+def _hash_universe(universe):
     return hashlib.sha256(bytes(str(tuple(universe)), 'utf-8')).hexdigest()
         
-def load_cache(universe, trading_interval, base_location):
-    folder = base_location/f'hash(universe)={hash_universe(universe)},trading_interval={trading_interval}'
+def _load_cache(universe, trading_frequency, base_location):
+    folder = base_location/f'hash(universe)={_hash_universe(universe)},trading_frequency={trading_frequency}'
     try:
         with open(folder/'cache.pkl', 'rb') as f:
             return pickle.load(f)
     except FileNotFoundError:
         return {}
     
-def store_cache(cache, universe, trading_interval, base_location):
-    folder = base_location/f'hash(universe)={hash_universe(universe)},trading_interval={trading_interval}'
+def _store_cache(cache, universe, trading_frequency, base_location):
+    folder = base_location/f'hash(universe)={_hash_universe(universe)},trading_frequency={trading_frequency}'
     folder.mkdir(exist_ok=True)
     with open(folder/'cache.pkl', 'wb') as f:
         pickle.dump(cache, f)
     
-    
-# def simulate_cash_holding_cost(t, h_plus, current_and_past_returns,
-#                                 spread_on_lending_cash_percent=0.5,
-#                                 spread_on_borrowing_cash_percent=0.5,
-#                                 periods_per_year=PPY, **kwargs):
-#     """Simulate holding cost for the cash account.
-#
-#     :param spread_on_lending_cash_percent: the cash account will generate annualized
-#         return equal to the cash return minus this number, expressed in percent annualized, or zero if
-#         the spread is larger than the cash return. For example with USDOLLAR cash,
-#         if the FRED-DFF annualized rate is 4.8% and spread_on_lending_cash_percent is 0.5
-#         (the default value), then the uninvested cash in the portfolio generates annualized
-#         return of 4.3%. See `this page <https://www.interactivebrokers.com/en/accounts/fees/pricing-interest-rates.php>_`.
-#     :type spread_on_lending_cash_percent: float, pd.Series
-#     :param spread_on_borrowing_cash_percent: if one instead borrows cash he pays the
-#         cash rate plus this spread, expressed in percent annualized. Default value is 0.5.
-#         See `this page <https://www.interactivebrokers.com/en/trading/margin-rates.php>_`.
-#     :type spread_on_borrowing_cash_percent: float, pd.Series
-#     """
-#
-#     multiplier = 1 / (100 * periods_per_year)
-#     lending_spread = DataEstimator(spread_on_lending_cash_percent).values_in_time(t) * multiplier
-#     borrowing_spread = DataEstimator(spread_on_borrowing_cash_percent).values_in_time(t) * multiplier
-#
-#     cash_return = current_and_past_returns.iloc[-1,-1]
-#     real_cash = h_plus.iloc[-1] + sum(np.minimum(h_plus.iloc[:-1], 0.))
-#
-#     if real_cash > 0:
-#         return real_cash * (max(cash_return - lending_spread, 0.) - cash_return)
-#     else:
-#         return real_cash * borrowing_spread
-#
-#
-# def simulate_stocks_holding_cost(t, h_plus, current_and_past_returns,
-#                                 spread_on_borrowing_stocks_percent=0.5,
-#                                 dividends=0., periods_per_year=PPY, **kwargs):
-#     """Holding cost for stocks used by MarketSimulator.
-#
-#     :param spread_on_borrowing_stocks_percent: when shorting a stock,
-#         one pays a rate on the value of the position equal to the cash return plus this spread,
-#         expressed in percent annualized. These values are hard to find historically, if you are unsure consider
-#         long-only portfolios or look at CFDs/futures instead. We set the default value to 0.5 (percent annualized)
-#         which is probably OK for US large cap stocks. See `this page <https://www.interactivebrokers.com/en/pricing/short-sale-cost.php>`_.
-#     :type spread_on_borrowing_stocks_percent: float, pd.Series, pd.DataFrame
-#     :param dividends: if not included in the returns (as they are by the default data interface,
-#         based on `yfinance`), you can pass a DataFrame of dividend payments which will be credited to the cash
-#         account (or debited, if short) at each round. Default is 0., corresponding to no dividends.
-#     :type dividends: float, pd.DataFrame
-#     """
-#
-#     multiplier = 1 / (100 * periods_per_year)
-#     borrowing_spread = DataEstimator(spread_on_borrowing_stocks_percent).values_in_time(t) * multiplier
-#     dividends = DataEstimator(dividends).values_in_time(t)
-#     result = 0.
-#     cash_return = current_and_past_returns.iloc[-1,-1]
-#     borrowed_stock_positions = np.minimum(h_plus.iloc[:-1], 0.)
-#     result += np.sum((cash_return + borrowing_spread) * borrowed_stock_positions)
-#     result += np.sum(h_plus[:-1] * DataEstimator(dividends).values_in_time(t))
-#     return result
-#
-#
-# def simulate_transaction_cost(t, u, current_prices, current_and_past_volumes,
-#                             current_and_past_returns, persharecost=0.005,
-#                             linearcost=0., nonlinearcoefficient=1.,
-#                             windowsigma=PPY, exponent=1.5, **kwargs):
-#     """Transaction cost model for the MarketSimulator.
-#
-#     :param per_share_fixed_cost: transaction cost per share traded. Default value is 0.005 (USD), uses
-#         Yahoo Finance open prices to simulate the number of stocks traded. See
-#         `this page <https://www.interactivebrokers.com/en/pricing/commissions-home.php>`_.
-#     :type per_share_fixed_cost: float
-#     :param transaction_cost_coefficient_b: coefficient that multiplies the non-linear
-#         term of the transaction cost. Default value is 1, you can pass any other constant value, a per-stock Series,
-#         or a per-day and per-stock DataFrame
-#     :type transaction_cost_coefficient_b: float, pd.Series, or pd.DataFrame
-#     :param transaction_cost_exponent: exponent of the non-linear term of the transaction cost model. Default value 1.5,
-#         this is applied to the trade volume (in US dollars) over the total market volume (in US dollars). See the
-#         paper for more details; this model is supported by a long tradition of research in market microstructure.
-#     :type transaction_cost_exponent: float
-#     """
-#
-#     persharecost = DataEstimator(persharecost).values_in_time(t) if not \
-#         (persharecost is None) else None
-#     nonlinearcoefficient = DataEstimator(nonlinearcoefficient).values_in_time(t) if not \
-#         (nonlinearcoefficient is None) else None
-#
-#     sigma = np.std(current_and_past_returns.iloc[-windowsigma:, :-1], axis=0)
-#
-#     result = 0.
-#     if not (persharecost is None):
-#         if current_prices is None:
-#             raise SyntaxError("If you don't provide prices you should set persharecost to None")
-#         result += persharecost * int(sum(np.abs(u.iloc[:-1] + 1E-6) / current_prices.values))
-#
-#     result += sum(DataEstimator(linearcost).values_in_time(t) * np.abs(u.iloc[:-1]))
-#
-#     if not (nonlinearcoefficient is None):
-#         if current_and_past_volumes is None:
-#             raise SyntaxError("If you don't provide volumes you should set nonlinearcoefficient to None")
-#         # we add 1 to the volumes to prevent 0 volumes error (trades are cancelled on 0 volumes)
-#         result += (np.abs(u.iloc[:-1])**exponent) @ (nonlinearcoefficient  *
-#             sigma / ((current_and_past_volumes.iloc[-1] + 1) ** (exponent - 1)))
-#
-#     assert not np.isnan(result)
-#     assert not np.isinf(result)
-#
-#     return -result
-        
-
-
         
 class MarketData:
-    """Prepare, hold, and serve market data.
-    
-    :param universe: list of `Yahoo Finance <https://finance.yahoo.com/>`_ tickers on which to
-        simulate performance of the trading strategy. If left unspecified you should at least
-        pass `returns` and `volumes`. If you define a different market data access interface
-        (look in `cvxportfolio.data` for how to do it) you should pass instead
-        the symbol names for that data provider. Default is empty list.
-    :type universe: list or None
-    :param returns: historical open-to-open returns. Default is None, it is ignored
-        if universe is specified.
-    :type returns: pandas.DataFrame 
-    :param volumes: historical market volumes expressed in value (e.g., US dollars).
-            Default is None, it is ignored if universe is specified.
-    :type volumes: pandas.DataFrame
-    :param prices: historical open prices. Default is None, it is ignored
-        if universe is specified. These are used to round the trades to integer number of stocks
-        if round_trades is True, and compute per-share transaction costs (if `per_share_fixed_cost`
-        is greater than zero).
-    :type prices: pandas.DataFrame
-    
+    """Prepare, hold, and serve market data. 
     
+    Not meant to be accessed by user. Most of its initialization
+    is documented in MarketSimulator.    
     """
     
     def __init__(self, 
         universe = [], 
         returns=None,
         volumes=None,
         prices=None, 
         cash_key='USDOLLAR',
         base_location=BASE_LOCATION, 
         min_history=pd.Timedelta('365.24d'),
         max_contiguous_missing='10d',
-        trading_interval=None,  # disabled for now because cache is not robust against this
+        trading_frequency=None,  # disabled for now because cache is not robust against this
         **kwargs,
     ):
         
         # TODO unblock once cache fixed
-        # trading_interval = None
+        # trading_frequency = None
         
         # drop duplicates and ensure ordering
         universe = sorted(set(universe))
         
         self.base_location = Path(base_location)
         self.min_history_timedelta = min_history
         self.max_contiguous_missing = max_contiguous_missing
         self.cash_key = cash_key
         
         if len(universe):
-            self.get_market_data(universe)
-            self.add_cash_column(self.cash_key)
+            self._get_market_data(universe)
+            self._add_cash_column(self.cash_key)
         else:
             if returns is None:
                 raise SyntaxError("If you don't specify a universe you should pass `returns`.")
             # if not returns.shape[1] == volumes.shape[1] + 1:
             #     raise SyntaxError(
             #         "In `returns` you must include the cash returns as the last column (and not in `volumes`).")
             self.returns = returns
             self.volumes = volumes
             self.prices = prices
             if cash_key != returns.columns[-1]:
-                self.add_cash_column(cash_key)
+                self._add_cash_column(cash_key)
                             
-        if trading_interval:
-            self.downsample(trading_interval)
+        if trading_frequency:
+            self._downsample(trading_frequency)
         
-        self.set_read_only()
-        self.check_sizes()
+        self._set_read_only()
+        self._check_sizes()
     
     
     def _reduce_universe(self, reduced_universe):
         assert reduced_universe[-1] == self.cash_key
         return MarketData(
             returns=self.returns[reduced_universe],
             volumes=self.volumes[reduced_universe[:-1]] if not (self.volumes is None) else None,
@@ -256,78 +128,78 @@
         
     @property
     def universe(self):
         return self.returns.columns
         
     sampling_intervals = {'weekly': 'W-MON', 'monthly':'MS', 'quarterly':'QS', 'annual':'AS'}
         
-    def downsample(self, interval):
-        """Downsample market data."""
+    def _downsample(self, interval):
+        """_downsample market data."""
         if not interval in self.sampling_intervals:
             raise SyntaxError('Unsopported trading interval for down-sampling.')
         interval = self.sampling_intervals[interval]
         self.returns = np.exp(np.log(1+self.returns).resample(interval, closed='left', label='left').sum(False, 1))-1
         self.volumes = self.volumes.resample(interval, closed='left', label='left').sum(False, 1)
         self.prices = self.prices.resample(interval, closed='left', label='left').first()
         
     @property
     def PPY(self):
         "Periods per year, assumes returns are about equally spaced."
         return periods_per_year(self.returns.index)
         
     
-    def check_sizes(self):
+    def _check_sizes(self):
         
         if (not self.volumes is None) and (not (self.volumes.shape[1] == self.returns.shape[1] - 1) \
             or not all(self.volumes.columns == self.returns.columns[:-1])):
             raise SyntaxError('Volumes should have same columns as returns, minus cash_key.')
         
         if (not self.prices is None) and (not (self.prices.shape[1] == self.returns.shape[1] - 1) \
             or not all(self.prices.columns == self.returns.columns[:-1])):
             raise SyntaxError('Prices should have same columns as returns, minus cash_key.')            
         
         
-    def serve_data_policy(self, t):
+    def _serve_data_policy(self, t):
         """Give data to policy at time t."""
         
         tidx = self.returns.index.get_loc(t)
         past_returns = pd.DataFrame(self.returns.iloc[:tidx])
         if not self.volumes is None:
             tidx = self.volumes.index.get_loc(t)
             past_volumes = pd.DataFrame(self.volumes.iloc[:tidx]) 
         else:
             past_volumes = None
         current_prices = pd.Series(self.prices.loc[t]) if not self.prices is None else None
         
         return past_returns, past_volumes, current_prices
         
     
-    def serve_data_simulator(self, t):
+    def _serve_data_simulator(self, t):
         """Give data to simulator at time t."""
         
         tidx = self.returns.index.get_loc(t)
         current_and_past_returns = pd.DataFrame(self.returns.iloc[:tidx+1])
         if not self.volumes is None:
             tidx = self.volumes.index.get_loc(t)
             current_and_past_volumes = pd.DataFrame(self.volumes.iloc[:tidx+1])
         else:
             current_and_past_volumes = None
         current_prices = pd.Series(self.prices.loc[t]) if not self.prices is None else None
         
         return current_and_past_returns, current_and_past_volumes, current_prices
         
         
-    def set_read_only(self):
+    def _set_read_only(self):
         """Set numpy array contained in dataframe to read only.
         
         This is enough to prevent direct assignement to the resulting 
         dataframe. However it could still be accidentally corrupted by assigning
         to columns or indices that are not present in the original.
         We avoid that case as well by returning a wrapped dataframe (which doesn't
-        copy data on creation) in serve_data_policy and serve_data_simulator.
+        copy data on creation) in _serve_data_policy and _serve_data_simulator.
         """
         
         def ro(df):
             data = df.values
             data.flags.writeable = False
             return pd.DataFrame(data, index=df.index, columns=df.columns)
             
@@ -335,41 +207,41 @@
         
         if not self.prices is None:
             self.prices = ro(self.prices)
             
         if not self.volumes is None:
             self.volumes = ro(self.volumes)
             
-    def add_cash_column(self, cash_key):
+    def _add_cash_column(self, cash_key):
         
         if not cash_key == 'USDOLLAR':
             raise NotImplementedError('Currently the only data pipeline built is for USDOLLAR cash')
             
         data = FredTimeSeries('DFF', base_location=self.base_location)
-        data.pre_evaluation()
+        data._recursive_pre_evaluation()
         self.returns[cash_key] = resample_returns(data.data / 100, periods=self.PPY)
         self.returns[cash_key] = self.returns[cash_key].fillna(method='ffill')
         
     
-    def get_market_data(self, universe):
+    def _get_market_data(self, universe):
         database_accesses = {}
         print('Updating data')
         for stock in universe:
             print('.')
             database_accesses[stock] = YfinanceTimeSeries(stock, base_location=self.base_location)
-            database_accesses[stock].pre_evaluation()
+            database_accesses[stock]._recursive_pre_evaluation()
 
         self.returns = pd.DataFrame({stock: database_accesses[stock].data['Return'] for stock in universe})
         self.volumes = pd.DataFrame({stock: database_accesses[stock].data['ValueVolume'] for stock in universe})
         self.prices = pd.DataFrame({stock: database_accesses[stock].data['Open'] for stock in universe})
         
-        self.remove_missing_recent()
+        self._remove_missing_recent()
                 
         
-    def remove_missing_recent(self):
+    def _remove_missing_recent(self):
         """Clean recent data.
         
         Yfinance has some issues with most recent data; 
         we remove recent days if there are NaNs.
         """
         
         if self.prices.iloc[-5:].isnull().any().any():
@@ -379,28 +251,28 @@
             self.volumes = self.volumes.loc[self.volumes.index<drop_at]
         
         # for consistency we must also nan-out the last row of returns and volumes
         self.returns.iloc[-1] = np.nan
         self.volumes.iloc[-1] = np.nan
         
         
-    def backtest_times(self, start_time=None, end_time=None, include_end=True):
+    def _get_backtest_times(self, start_time=None, end_time=None, include_end=True):
         """Get trading calendar from market data."""
         result = self.returns.index
-        result = result[result >= self.earliest_backtest_start]
+        result = result[result >= self._earliest_backtest_start]
         if start_time:
             result = result[result >= start_time]
         if end_time:
             result = result[(result <= end_time)]
         if not include_end:
             result = result[:-1]
         return result
 
-    @cached_property
-    def break_timestamps(self):
+    @property
+    def _break_timestamps(self):
         """List of timestamps at which a backtest should be broken.
         
         An asset enters into a backtest after having non-NaN returns
         for self.min_history periods and exits after having NaN returns
         for self.max_contiguous_missing. Defaults values are 252 and 10 
         respectively.
         """
@@ -412,50 +284,50 @@
                 self.entry_dates[single_asset_returns.index[self.min_history]].append(asset)
                 exit_date = single_asset_returns.index[-1]
                 if (self.returns.index[-1] - exit_date) >= pd.Timedelta(self.max_contiguous_missing):
                     self.exit_dates[exit_date].append(asset) 
 
         return sorted(set(self.exit_dates) | set(self.entry_dates))
         
-    @cached_property    
-    def limited_universes(self):
+    @property    
+    def _limited_universes(self):
         """Valid universes for each section, minus cash.
         
         A backtest is broken into multiple ones that start at each key
         of this, have the universe specified by this, and end
         at the next startpoint.  
         """
         result = OrderedDict()
         uni = []
-        for ts in self.break_timestamps:
+        for ts in self._break_timestamps:
             uni += self.entry_dates[ts]
             uni = [el for el in uni if not el in self.exit_dates[ts]]
             result[ts] = tuple(sorted(uni))
         return result
     
     @property
-    def earliest_backtest_start(self):
+    def _earliest_backtest_start(self):
         """Earliest date at which we can start a backtest."""
         return self.returns.iloc[:,:-1].dropna(how='all').index[self.min_history]
         
         
-    def get_limited_backtests(self, start_time, end_time):
+    def _get_limited_backtests(self, start_time, end_time):
         """Get start/end times and universes of constituent backtests.
         
         Each one has constant universe with assets' that meet the
         ``min_history`` requirement and has not disappeared from the
         dataset.
         """
                 
-        full_backtest_times = self.backtest_times(start_time, end_time)
-        brkt = np.array(self.break_timestamps)
+        full_backtest_times = self._get_backtest_times(start_time, end_time)
+        brkt = np.array(self._break_timestamps)
 
         def get_valid_universe_and_its_expiration_for(time):    
             try:
-                return self.limited_universes[brkt[brkt<=time][-1]], \
+                return self._limited_universes[brkt[brkt<=time][-1]], \
                     brkt[brkt>time][0] if len(brkt[brkt>time]) else full_backtest_times[-1]
             except IndexError:
                 raise DataError('There are no assets that meet the required min_history.')
         
         result = []
         start = full_backtest_times[0]
         while True:
@@ -483,138 +355,156 @@
     #     See the paper for an explanation of the model. Here you specify the length of the rolling window to use,
     #     default is 252 (typical number of trading days in a year).
     # :type window_sigma_estimate: int
 
 class MarketSimulator:
     """This class implements a simulator of market performance for trading strategies.
     
-    
-
     We strive to make the parameters here as accurate as possible. The following is
     accurate as of 2023 using numbers obtained on the public website of a
     `large US-based broker <https://www.interactivebrokers.com/>`_.
 
+    :param universe: list of `Yahoo Finance <https://finance.yahoo.com/>`_ tickers on which to
+        simulate performance of the trading strategy. If left unspecified you should at least
+        pass `returns` and `volumes`. If you define a different market data access interface
+        (look in `cvxportfolio.data` for how to do it) you should pass instead
+        the symbol names for that data provider. Default is empty list.
+    :type universe: list or None
+    :param returns: historical open-to-open returns. Default is None, it is ignored
+        if universe is specified.
+    :type returns: pandas.DataFrame 
+    :param volumes: historical market volumes expressed in value (e.g., US dollars).
+            Default is None, it is ignored if universe is specified.
+    :type volumes: pandas.DataFrame
+    :param prices: historical open prices. Default is None, it is ignored
+        if universe is specified. These are used to round the trades to integer number of stocks
+        if round_trades is True, and compute per-share transaction costs (if `per_share_fixed_cost`
+        is greater than zero).
+    :type prices: pandas.DataFrame
     :param round_trades: round the trade weights provided by a policy so they correspond to an integer
         number of stocks traded. Default is True using Yahoo Finance open prices.
     :type round_trades: bool
-    
     :param costs: list of BaseCost instances or class objects. If class objects (the default) they will
         be instantiated internally with their default arguments.
     :type costs: list
     :param cash_key: name of the cash account. Default is 'USDOLLAR', which gets downloaded by `cvxportfolio.data`
         as the Federal Funds effective rate from FRED. If None, you must pass the cash returns
         along with the stock returns as its last column.
     :type cash_key: str or None
     :param base_location: base location for storage of data.
         Default is `Path.home() / "cvxportfolio_data"`. Unused if passing `returns` and `volumes`.
     :type base_location: pathlib.Path or str: 
-    
-    
+    :param trading_frequency: optionally choose a different frequency for 
+        trades than the one of the data used.
+        The default interface (Yahoo finance) provides daily trading data, 
+        and so that is the default frequency for trades. With this argument you can set instead 
+        the trading frequency to ``"weekly"``, which trades every Monday (or the first
+        non-holiday trading day of each week), ``"monthly"``, which trades every first of the month (ditto), 
+        ``"quarterly"``, and ``"annual"``. 
+    :type trading_frequency: str or None
     """
 
     def __init__(
         self,
         universe=[],
         returns=None,
         volumes=None,
         prices=None,
-        costs=[TransactionCost, HoldingCost,
-            #simulate_transaction_cost, simulate_stocks_holding_cost, simulate_cash_holding_cost
-        ],
+        costs=[TransactionCost, HoldingCost],
         round_trades=True,
         min_history_for_inclusion=pd.Timedelta('365d'), # TODO temporary, will use MarketData infrastructure
         cash_key="USDOLLAR",
         base_location=BASE_LOCATION,
-        trading_interval=None,
+        trading_frequency=None,
         **kwargs,
     ):
         """Initialize the Simulator and download data if necessary."""
         self.base_location = Path(base_location)
         
         self.market_data = MarketData(
             universe=universe, returns=returns,
             volumes=volumes, prices=prices,
             cash_key=cash_key, base_location=base_location,
-            trading_interval=trading_interval,
+            trading_frequency=trading_frequency,
             min_history=min_history_for_inclusion,
             **kwargs)
             
-        self.trading_interval = trading_interval
+        self.trading_frequency = trading_frequency
                 
         if not len(universe) and prices is None:
             if round_trades:
                 raise SyntaxError(
                     "If you don't specify prices you can't request `round_trades`.")
 
         self.round_trades = round_trades
         self.min_history_for_inclusion = min_history_for_inclusion
         
         self.costs = [el() if isinstance(el, type) else el for el in costs]
        # self.kwargs = kwargs
 
         
     @staticmethod
-    def round_trade_vector(u, current_prices):
+    def _round_trade_vector(u, current_prices):
         """Round dollar trade vector u.
         """
         result = pd.Series(u, copy=True)
         result[:-1] = np.round(u[:-1] / current_prices) * current_prices
         result[-1] = -sum(result[:-1])
         return result
 
 
-    def simulate(self, t, h, policy, **kwargs):
+    def _simulate(self, t, h, policy, **kwargs):
         """Get next portfolio and statistics used by Backtest for reporting.
 
         The signature of this method differs from other estimators
         because we pass the policy directly to it, and the past returns and past volumes
         are computed by it.
         """
         
         # translate to weights
         current_portfolio_value = sum(h)
         current_weights = h / current_portfolio_value
 
-        past_returns, past_volumes, current_prices = self.market_data.serve_data_policy(t)
+        past_returns, past_volumes, current_prices = self.market_data._serve_data_policy(t)
 
         # evaluate the policy
         s = time.time()
-        z = policy.values_in_time(t=t, current_weights=current_weights, current_portfolio_value=current_portfolio_value, 
+        z = policy._recursive_values_in_time(t=t, current_weights=current_weights, current_portfolio_value=current_portfolio_value, 
             past_returns=past_returns, past_volumes=past_volumes, current_prices=current_prices, **kwargs)
         policy_time = time.time() - s
         
         # for safety recompute cash
         z[-1] = -sum(z[:-1])
         assert sum(z) == 0.
         
         # trades in dollars
         u = z * current_portfolio_value
         
         # get data for simulator
-        current_and_past_returns, current_and_past_volumes, current_prices = self.market_data.serve_data_simulator(t)
+        current_and_past_returns, current_and_past_volumes, current_prices = self.market_data._serve_data_simulator(t)
 
         # zero out trades on stock that weren't trading on that day 
         if not (current_and_past_volumes is None):
             current_volumes = current_and_past_volumes.iloc[-1]
             non_tradable_stocks = current_volumes[current_volumes <= 0].index
             u[non_tradable_stocks] = 0.
 
         # round trades
         if self.round_trades:
-            u = self.round_trade_vector(u, current_prices)
+            u = self._round_trade_vector(u, current_prices)
             
         # for safety recompute cash
         u[-1] = -sum(u[:-1])
         assert sum(u) == 0.
 
         # compute post-trade holdings (including cash balance)
         h_plus = h + u
 
         # evaluate cost functions
-        realized_costs = {cost.__class__.__name__: cost.simulate(t=t, u=u,  h_plus=h_plus, 
+        realized_costs = {cost.__class__.__name__: cost._simulate(t=t, u=u,  h_plus=h_plus, 
             current_and_past_volumes=current_and_past_volumes, 
             current_and_past_returns=current_and_past_returns,
             current_prices=current_prices,
             periods_per_year=self.market_data.PPY,
             windowsigma=self.market_data.PPY, #**self.kwargs
             ) for cost in self.costs}
         
@@ -626,64 +516,64 @@
 
         # multiply positions by market returns
         current_returns = current_and_past_returns.iloc[-1]
         h_next *= (1 + current_returns)
             
         return h_next, z, u, realized_costs, policy_time
         
-    def initialize_policy(self, policy, start_time, end_time):
+    def _initialize_policy(self, policy, start_time, end_time):
         """Initialize the policy object.
         """
-        policy.pre_evaluation(universe = self.market_data.universe,
-                             backtest_times = self.market_data.backtest_times(start_time, end_time, include_end=False))
+        policy._recursive_pre_evaluation(universe = self.market_data.universe,
+                             backtest_times = self.market_data._get_backtest_times(start_time, end_time, include_end=False))
 
         # if policy initialized a cache, rewrite it with loaded one
         #if hasattr(policy, 'cache'):
-        #    policy.cache = load_cache(universe=self.market_data.universe, trading_interval = self.trading_interval,
+        #    policy.cache = _load_cache(universe=self.market_data.universe, trading_frequency = self.trading_frequency,
         #        base_location=self.base_location)
 
 
     def _single_backtest(self, policy, start_time, end_time, h, universe=None#, backtest_times=None
     ):
         if universe is None:
             universe = self.market_data.universe
         #if backtest_times is None:
-        backtest_times = self.market_data.backtest_times(start_time, end_time, include_end=False)
+        backtest_times = self.market_data._get_backtest_times(start_time, end_time, include_end=False)
 
-        # self.initialize_policy(policy, start_time, end_time)
+        # self._initialize_policy(policy, start_time, end_time)
 
-        if hasattr(policy, 'compile_to_cvxpy'):
-            policy.compile_to_cvxpy()
+        if hasattr(policy, '_compile_to_cvxpy'):
+            policy._compile_to_cvxpy()
 
         result = BacktestResult(universe, backtest_times, self.costs)
 
         # this is the main loop of a backtest
         for t in backtest_times:
             result.h.loc[t] = h
             # print(t, h)
             s = time.time()
             h, result.z.loc[t], result.u.loc[t], realized_costs, \
-                    result.policy_times.loc[t] = self.simulate(t=t, h=h, policy=policy)
+                    result.policy_times.loc[t] = self._simulate(t=t, h=h, policy=policy)
             for cost in realized_costs:
                 result.costs[cost].loc[t] = realized_costs[cost]
             result.simulator_times.loc[t] = time.time() - s - result.policy_times.loc[t]
 
         result.h.loc[pd.Timestamp(end_time)] = h
 
         # TODO fix this
         result.cash_returns = self.market_data.returns.iloc[:,-1].loc[result.u.index]
 
         #if hasattr(policy, 'cache'):
-        #    store_cache(cache=policy.cache, universe=universe,
-        #    trading_interval = self.trading_interval, base_location=self.base_location)
+        #    _store_cache(cache=policy.cache, universe=universe,
+        #    trading_frequency = self.trading_frequency, base_location=self.base_location)
 
         return result
 
     def _concatenated_backtests(self, policy, start_time, end_time, h):
-        constituent_backtests_params = self.market_data.get_limited_backtests(start_time, end_time)
+        constituent_backtests_params = self.market_data._get_limited_backtests(start_time, end_time)
         # print(constituent_backtests_params)
         results = []
         orig_md = self.market_data
         orig_policy = policy
         for el in constituent_backtests_params:
             logging.info(f"current universe: {el['universe']}")
             logging.info(f"interval: {el['start_time']}, {el['end_time']}")
@@ -696,31 +586,31 @@
             else:
                 h = h[el['universe']]
            #  # print('h')
             # print(h)
             
             policy = copy.deepcopy(orig_policy)
             # print(el['start_time'], el['end_time'])
-            policy.pre_evaluation(universe = el['universe'],
-                backtest_times = self.market_data.backtest_times(el['start_time'], el['end_time'], include_end=True))
+            policy._recursive_pre_evaluation(universe = el['universe'],
+                backtest_times = self.market_data._get_backtest_times(el['start_time'], el['end_time'], include_end=True))
             if not (hasattr(self, 'PARALLEL') and self.PARALLEL):
                 if hasattr(policy, 'cache'):
-                    policy.cache = load_cache(universe=el['universe'], trading_interval = self.trading_interval, 
+                    policy.cache = _load_cache(universe=el['universe'], trading_frequency = self.trading_frequency, 
                         base_location=self.base_location)
                     
             results.append(self._single_backtest(policy, el['start_time'], el['end_time'], h, el['universe']))
             # print(results[0].w)
             #print(results[0].h)
             # print(results[0].returns)
             # print(dir(results[0]))
             h = results[-1].h.iloc[-1]
             if not (hasattr(self, 'PARALLEL') and self.PARALLEL):
                 if hasattr(policy, 'cache'):
-                    store_cache(cache=policy.cache, universe=el['universe'], 
-                    trading_interval = self.trading_interval, base_location=self.base_location)
+                    _store_cache(cache=policy.cache, universe=el['universe'], 
+                    trading_frequency = self.trading_frequency, base_location=self.base_location)
         # print(results)
         
         res = BacktestResult.__new__(BacktestResult)
         res.costs = {}
         
         res.h = pd.concat([el.h.iloc[:-1] if i < len(results) -1 else el.h for i, el in enumerate(results)])
         for attr in ['cash_returns', 'u', 'z', 'simulator_times', 'policy_times']:
@@ -742,128 +632,134 @@
                 
         self.market_data = orig_md
         # raise Exception
         return res
         
             
     @staticmethod
-    def worker(policy, simulator, start_time, end_time, h):
+    def _worker(policy, simulator, start_time, end_time, h):
         #return simulator._single_backtest(policy, start_time, end_time, h)
         return simulator._concatenated_backtests(policy, start_time, end_time, h)
-                                    
-    def backtest(self, policy, start_time=None, end_time=None, initial_value = 1E6, h=None, parallel=True):
-        """Backtest one or more trading policy.
         
-        If runnning in parallel you must be careful at how you use this method. If 
-        you use this in a script, you should define the MarketSimulator
-        *in* the `if __name__ == '__main__:'` clause, and call this method there as well.
+    def backtest(self, policy, start_time=None, end_time=None, initial_value = 1E6, h=None):
+        """Backtest trading policy.
         
         The default initial portfolio is all cash, or you can pass any portfolio with
-        the `h` argument, or a list of those if running multiple backtests.
+        the `h` argument.
         
-        :param policy: if passing a single trading policy it performs a single backtest 
-            in the main process. If passing a list, it uses Python multiprocessing to
-            create multiple processes and run many policies in parallel.
-        :type policy: cvx.BaseTradingPolicy or list
-        :param start_time: start time of the backtest(s), if holiday, the first trading day
+        :param policy: trading policy
+        :type policy: cvx.BaseTradingPolicy
+        :param start_time: start time of the backtest; if market it close, the first trading day
              after it is selected
         :type start_time: str or datetime 
-        :param end_time: end time of the backtest(s), if holiday, the last trading day
+        :param end_time: end time of the backtest; if market it close, the last trading day
              before it is selected
         :type end_time: str or datetime or None
         :param initial_value: initial value in dollar of the portfolio, if not specifying
-            `h` it is assumed the initial portfolio is all cash
+            ``h`` it is assumed the initial portfolio is all cash; if ``h`` is specified 
+            this is ignored
         :type initial_value: float
-        :param h: initial portfolio `h` expressed in dollar positions, or list of those 
-            for multiple backtests
+        :param h: initial portfolio ``h`` expressed in dollar positions. If ``None`` 
+            an initial portfolio of ``initial_value`` in cash is used.
+        :type h: pd.Series or None
+        
+        :returns result: instance of :class:`BacktestResult` which has all relevant backtest
+            data and logic to compute metrics, generate plots, ...
+        :rtype result: cvx.BacktestResult
+        """
+        return self.backtest_many([policy], start_time = start_time, end_time = end_time, 
+                             initial_value = initial_value, h=h, parallel=False)[0]
+                                    
+    def backtest_many(self, policies, start_time=None, end_time=None, initial_value = 1E6, h=None, parallel=True):
+        """Backtest many trading policies.
+        
+        The default initial portfolio is all cash, or you can pass any portfolio with
+        the `h` argument, or a list of those.
+        
+        :param policies: trading policies
+        :type policy: list of cvx.BaseTradingPolicy:
+        :param start_time: start time of the backtests; if market it close, the first trading day
+             after it is selected. Currently it is not possible to specify different start times
+            for different policies, so the same is used for all.
+        :type start_time: str or datetime 
+        :param end_time: end time of the backtests; if market it close, the last trading day
+             before it is selected. Currently it is not possible to specify different end times
+            for different policies, so the same is used for all.
+        :type end_time: str or datetime or None
+        :param initial_value: initial value in dollar of the portfolio, if not specifying
+            ``h`` it is assumed the initial portfolio is all cash; if ``h`` is specified 
+            this is ignored
+        :param h: initial portfolio `h` expressed in dollar positions, or list of those. If 
+            passing a list it must have the same lenght as the policies. If this argument
+            is specified, ``initial_value`` is ignored, otherwise the same portfolio of 
+            ``initial_value`` all in cash is used as starting point for all backtests.
         :type h: list or pd.Series or None
-        :param parallel: whether to run in parallel if there are multiple policies or not.
-            If not, it just iterates through the policies in the main process.
+        :param parallel: whether to run in parallel. If runnning in parallel you **must be careful 
+            at how you use this method**. If you use this in a script, you *should* define the MarketSimulator
+            *in* the `if __name__ == '__main__:'` clause, and call this method there as well.
         :type parallel: bool
         
-        :returns result: instance of :class:`BacktestResult` which has all relevant backtest
+        :returns result: list of instances of :class:`BacktestResult` which have all relevant backtest
             data and logic to compute metrics, generate plots, ...
-        :rtype result: cvx.BacktestResult or list
+        :rtype result: list of cvx.BacktestResult
         """
         
         # turn policy and h into lists
-        if not hasattr(policy, '__len__'):
-            policy = [policy]
+        assert hasattr(policies, '__len__')
+        # if not hasattr(policies, '__len__'):
+        #     policies = [policies]
         
         if not hasattr(h, '__len__'):
-            h = [h] * len(policy)
+            h = [h] * len(policies)
             
-        if not (len(policy) == len(h)):
+        if not (len(policies) == len(h)):
             raise SyntaxError("If passing lists of policies and initial portfolios they must have the same length.")
         
-        # discover start and end times
-        # start_time = pd.Series(self.returns.data.index >= start_time, self.returns.data.index).idxmax()
-        # if end_time is None:
-        #     end_time  = self.returns.data.index[-1]
-        # else:
-        #    end_time = self.returns.data.index[self.returns.data.index <= end_time][-1]
             
-        backtest_times_inclusive = self.market_data.backtest_times(start_time, end_time, include_end=True)
+        backtest_times_inclusive = self.market_data._get_backtest_times(start_time, end_time, include_end=True)
         start_time = backtest_times_inclusive[0]
         end_time = backtest_times_inclusive[-1]
         
-        #constituent_backtests = self.market_data.get_limited_backtests(start_time, end_time)
-        #raise Exception
-            
-        if False:
-            # TODO fix this - discard names that don't meet the min_history_for_inclusion
-            min_history = self.market_data.PPY * int(round(self.min_history_for_inclusion.days/365))
-            # print('min_history', min_history)
-            history = (~self.market_data.returns.loc[self.market_data.returns.index < start_time].isnull()).sum()
-            reduced_universe = self.market_data.returns.columns[history >= min_history]
-            # print('reduced_universe', reduced_universe)
-            self.market_data.returns = self.market_data.returns[reduced_universe]
-            if not (self.market_data.volumes is None):
-                self.market_data.volumes = self.market_data.volumes[reduced_universe[:-1]]
-            if not (self.market_data.prices is None):
-                self.market_data.prices = self.market_data.prices[reduced_universe[:-1]]
-            # self.sigma_estimate.data = self.sigma_estimate.data[reduced_universe[:-1]]
-        
         # initialize policies and get initial portfolios
-        for i in range(len(policy)):
-            # self.initialize_policy(policy[i], start_time, end_time)
+        for i in range(len(policies)):
+            # self._initialize_policy(policy[i], start_time, end_time)
         
             if h[i] is None:
                 h[i] = pd.Series(0., self.market_data.universe)
                 h[i][-1] = initial_value
                 
         # def nonparallel_runner(zipped):
         #     return self._single_backtest(zipped[0], start_time, end_time, zipped[1])
         
-        zip_args = zip(policy, [self] * len(policy), [start_time] * len(policy), [end_time] * len(policy), h)
+        zip_args = zip(policies, [self] * len(policies), [start_time] * len(policies), [end_time] * len(policies), h)
         
         # decide if run in parallel or not
-        if (not parallel) or len(policy)==1: 
+        if (not parallel) or len(policies)==1: 
             #result = list(map(nonparallel_runner, zip(policy, h)))
-            result = list(starmap(self.worker, zip_args))
+            result = list(starmap(self._worker, zip_args))
         else:
             self.PARALLEL = True # TODO temporary, to disable some features when running in parallel
             with Pool() as p:
-                result = p.starmap(self.worker, zip_args)   
+                result = p.starmap(self._worker, zip_args)   
             del self.PARALLEL
-        if len(result) == 1:
-            return result[0]
+        # if len(result) == 1:
+        #     return result[0]
         return result
 
 # def _do_single_backtest(policy, start_time, end_time, simulator, cache):
 #     """This function can run on remote process/machine."""
 #
 #     universe = simulator.market_data.universe
-#     backtest_times = simulator.market_data.backtest_times(start_time, end_time)
+#     backtest_times = simulator.market_data._get_backtest_times(start_time, end_time)
 #
-#     policy.pre_evaluation(universe=universe, backtest_times=backtest_times)
+#     policy._recursive_pre_evaluation(universe=universe, backtest_times=backtest_times)
 #     if hasattr(policy, 'cache'):
 #         policy.cache = cache
-#     if hasattr(policy, 'compile_to_cvxpy'):
-#         policy.compile_to_cvxpy()
+#     if hasattr(policy, '_compile_to_cvxpy'):
+#         policy._compile_to_cvxpy()
 #
 #     result = BacktestResult(universe, backtest_times, simulator.costs)
 #
 #     # this is the main loop of a backtest
 #     for t in backtest_times:
 #         result.h.loc[t] = h
 #         s = time.time()
```

### Comparing `cvxportfolio-0.3.4/cvxportfolio/tests/base.py` & `cvxportfolio-0.3.5/cvxportfolio/tests/base.py`

 * *Files 2% similar despite different names*

```diff
@@ -31,9 +31,9 @@
         cls.volumes = pd.read_csv(Path(__file__).parent / "volumes.csv", index_col=0, parse_dates=[0])
         cls.w_plus = cp.Variable(cls.returns.shape[1])
         cls.w_plus_minus_w_bm = cp.Variable(cls.returns.shape[1])
         cls.z = cp.Variable(cls.returns.shape[1])
         cls.N = cls.returns.shape[1]
     
     def boilerplate(self, model):
-        model.pre_evaluation(universe=self.returns.columns, backtest_times=self.returns.index)
-        return model.compile_to_cvxpy(self.w_plus, self.z, self.w_plus_minus_w_bm)
+        model._recursive_pre_evaluation(universe=self.returns.columns, backtest_times=self.returns.index)
+        return model._compile_to_cvxpy(self.w_plus, self.z, self.w_plus_minus_w_bm)
```

### Comparing `cvxportfolio-0.3.4/cvxportfolio/tests/returns.csv` & `cvxportfolio-0.3.5/cvxportfolio/tests/returns.csv`

 * *Files identical despite different names*

### Comparing `cvxportfolio-0.3.4/cvxportfolio/tests/sigmas.csv` & `cvxportfolio-0.3.5/cvxportfolio/tests/sigmas.csv`

 * *Files identical despite different names*

### Comparing `cvxportfolio-0.3.4/cvxportfolio/tests/test_constraints.py` & `cvxportfolio-0.3.5/cvxportfolio/tests/test_constraints.py`

 * *Files 2% similar despite different names*

```diff
@@ -34,17 +34,17 @@
         cls.w_plus = cp.Variable(cls.returns.shape[1])
         cls.w_plus_minus_w_bm = cp.Variable(cls.returns.shape[1])
         cls.z = cp.Variable(cls.returns.shape[1])
         cls.N = cls.returns.shape[1]
         
     def build_constraint(self, constraint, t=None):
         """Initialize constraint, build expression, and point it to given time."""
-        constraint.pre_evaluation(self.returns.columns, self.returns.index)
-        cvxpy_expression = constraint.compile_to_cvxpy(self.w_plus, self.z, self.w_plus_minus_w_bm)
-        constraint.values_in_time(t=pd.Timestamp("2020-01-01") if t is None else t, current_portfolio_value=1000)
+        constraint._recursive_pre_evaluation(self.returns.columns, self.returns.index)
+        cvxpy_expression = constraint._compile_to_cvxpy(self.w_plus, self.z, self.w_plus_minus_w_bm)
+        constraint._recursive_values_in_time(t=pd.Timestamp("2020-01-01") if t is None else t, current_portfolio_value=1000)
         return cvxpy_expression
         
     def test_long_only(self):
         model = cvx.LongOnly()
         cons = self.build_constraint(model)
         self.w_plus.value = np.ones(self.N)
         self.assertTrue(cons.value())
@@ -64,17 +64,17 @@
         self.assertFalse(cons.value())
         
     def test_min_cash(self):
         model = cvx.MinCashBalance(10000) # USD
         cons = self.build_constraint(model)
         self.w_plus.value = np.zeros( self.N)
         self.w_plus.value[-1] = 1
-        model.values_in_time(t=pd.Timestamp("2020-01-01"), current_portfolio_value=10001)
+        model._recursive_values_in_time(t=pd.Timestamp("2020-01-01"), current_portfolio_value=10001)
         self.assertTrue(cons.value())
-        model.values_in_time(t=pd.Timestamp("2020-01-01"), current_portfolio_value=9999)
+        model._recursive_values_in_time(t=pd.Timestamp("2020-01-01"), current_portfolio_value=9999)
         self.assertFalse(cons.value())        
         
 
     def test_dollar_neutral(self):
         model = cvx.DollarNeutral()
         cons = self.build_constraint(model)
         tmpvalue = np.zeros( self.N)
@@ -110,15 +110,15 @@
         model = cvx.LeverageLimit(limits)
         cons = self.build_constraint(model, t=self.returns.index[1])
         tmp = np.zeros(self.N)
         tmp[0] = 4
         tmp[-1] = -3
         self.w_plus.value = tmp
         self.assertTrue(cons.value())
-        model.values_in_time(t=self.returns.index[2])
+        model._recursive_values_in_time(t=self.returns.index[2])
         self.assertFalse(cons.value())
         
     def test_max_weights(self):
         model = cvx.MaxWeights(2)
         cons = self.build_constraint(model)
         self.w_plus.value = np.ones(self.N) / self.N
         self.assertTrue(cons.value())
@@ -144,15 +144,15 @@
         cons = self.build_constraint(model, t=self.returns.index[1])
 
         tmp = np.zeros(self.N)
         tmp[0] = 4
         tmp[-1] = -3
         self.w_plus.value = tmp
         self.assertTrue(cons.value())
-        model.values_in_time(t=self.returns.index[2])
+        model._recursive_values_in_time(t=self.returns.index[2])
         self.assertFalse(cons.value())
         
     def test_min_weights(self):
         model = cvx.MinWeights(2)
         cons = self.build_constraint(model, self.returns.index[1])
 
         self.w_plus.value = np.ones(self.N) / self.N
@@ -175,15 +175,15 @@
         model = cvx.MinWeights(limits)
         cons = self.build_constraint(model, t=self.returns.index[1])
         tmp = np.zeros(self.N)
         tmp[0] = 4
         tmp[-1] = -3
         self.w_plus.value = tmp
         self.assertTrue(cons.value())
-        model.values_in_time(t=self.returns.index[2])
+        model._recursive_values_in_time(t=self.returns.index[2])
         self.assertFalse(cons.value())
 
     def test_factor_max_limit(self):
         
         model = cvx.FactorMaxLimit(np.ones((self.N - 1, 2)), np.array([0.5, 1]))
         cons = self.build_constraint(model, self.returns.index[1])
 
@@ -260,17 +260,17 @@
         """Test trading constraints."""
 
         t = self.returns.index[1]
 
         # avg daily value limits.
         value = 1e6
         model = cvx.ParticipationRateLimit(self.volumes, max_fraction_of_volumes=0.1)
-        model.pre_evaluation(self.returns.columns, self.returns.index)
-        cons = model.compile_to_cvxpy(self.w_plus, self.z, self.w_plus_minus_w_bm)
-        model.values_in_time(t=t, current_portfolio_value=value)
+        model._recursive_pre_evaluation(self.returns.columns, self.returns.index)
+        cons = model._compile_to_cvxpy(self.w_plus, self.z, self.w_plus_minus_w_bm)
+        model._recursive_values_in_time(t=t, current_portfolio_value=value)
         print(model.portfolio_value.value)
         # cons = model.weight_expr(t, None, z, value)[0]
         tmp = np.zeros(self.N)
         tmp[:-1] = self.volumes.loc[t].values / value * 0.05
         self.z.value = tmp
         self.assertTrue(cons.value())
         self.z.value = -100 * self.z.value  # -100*np.ones(n)
```

### Comparing `cvxportfolio-0.3.4/cvxportfolio/tests/test_costs.py` & `cvxportfolio-0.3.5/cvxportfolio/tests/test_costs.py`

 * *Files 4% similar despite different names*

```diff
@@ -49,52 +49,52 @@
         self.w_plus_minus_w_bm.value /= sum(self.w_plus_minus_w_bm.value)
         t = self.returns.index[1]
 
         cost1 = DiagonalCovariance()
         cost2 = FullCovariance(self.returns.iloc[:, :-1].T @ self.returns.iloc[:, :-1] / len(self.returns))
         cost3 = cost1 + cost2
 
-        cost3.pre_evaluation(universe=self.returns.columns, backtest_times=self.returns.index)
-        expr3 = cost3.compile_to_cvxpy(self.w_plus, self.z, self.w_plus_minus_w_bm)
-        expr1 = cost1.compile_to_cvxpy(self.w_plus, self.z, self.w_plus_minus_w_bm)
-        expr2 = cost2.compile_to_cvxpy(self.w_plus, self.z, self.w_plus_minus_w_bm)
-        cost3.values_in_time(t=t, past_returns=self.returns.loc[self.returns.index < t])
+        cost3._recursive_pre_evaluation(universe=self.returns.columns, backtest_times=self.returns.index)
+        expr3 = cost3._compile_to_cvxpy(self.w_plus, self.z, self.w_plus_minus_w_bm)
+        expr1 = cost1._compile_to_cvxpy(self.w_plus, self.z, self.w_plus_minus_w_bm)
+        expr2 = cost2._compile_to_cvxpy(self.w_plus, self.z, self.w_plus_minus_w_bm)
+        cost3._recursive_values_in_time(t=t, past_returns=self.returns.loc[self.returns.index < t])
         self.assertTrue(expr3.value == expr1.value + expr2.value)
 
         cost4 = cost1 * 2
-        expr4 = cost4.compile_to_cvxpy(self.w_plus, self.z, self.w_plus_minus_w_bm)
+        expr4 = cost4._compile_to_cvxpy(self.w_plus, self.z, self.w_plus_minus_w_bm)
         self.assertTrue(expr4.value == expr1.value * 2)
 
         cost3 = cost1 - cost2
-        expr3 = cost3.compile_to_cvxpy(self.w_plus, self.z, self.w_plus_minus_w_bm)
+        expr3 = cost3._compile_to_cvxpy(self.w_plus, self.z, self.w_plus_minus_w_bm)
         self.assertTrue(expr3.value == expr1.value - expr2.value)
 
         cost3 = -cost1 + 2 * cost2
-        expr3 = cost3.compile_to_cvxpy(self.w_plus, self.z, self.w_plus_minus_w_bm)
+        expr3 = cost3._compile_to_cvxpy(self.w_plus, self.z, self.w_plus_minus_w_bm)
         self.assertTrue( expr3.value == -expr1.value + 2 * expr2.value)
 
         cost3 = -cost1 + 2 * (cost2 + cost1)
-        expr3 = cost3.compile_to_cvxpy(self.w_plus, self.z, self.w_plus_minus_w_bm)
+        expr3 = cost3._compile_to_cvxpy(self.w_plus, self.z, self.w_plus_minus_w_bm)
         self.assertTrue( np.isclose(expr3.value, -expr1.value + 2 * (expr2.value + expr1.value)))
 
         cost3 = cost1 - 2 * (cost2 + cost1)
-        expr3 = cost3.compile_to_cvxpy(self.w_plus, self.z, self.w_plus_minus_w_bm)
+        expr3 = cost3._compile_to_cvxpy(self.w_plus, self.z, self.w_plus_minus_w_bm)
         self.assertTrue( expr3.value == expr1.value - 2 * (expr2.value + expr1.value))
         
     def test_hcost(self):
         """Test holding cost model."""
         dividends = pd.Series(np.random.randn(self.N-1), self.returns.columns[:-1])
         dividends *= 0.
         hcost = HoldingCost(spread_on_borrowing_stocks_percent=.5,
                             dividends=dividends)
         
         t = 100 # this is picked so that periods_per_year evaluates to 252
-        hcost.pre_evaluation(universe=self.returns.columns, backtest_times=self.returns.index)
-        expression = hcost.compile_to_cvxpy(self.w_plus, self.z, self.w_plus_minus_w_bm)
-        hcost.values_in_time(t=self.returns.index[t], past_returns=self.returns.iloc[:t])
+        hcost._recursive_pre_evaluation(universe=self.returns.columns, backtest_times=self.returns.index)
+        expression = hcost._compile_to_cvxpy(self.w_plus, self.z, self.w_plus_minus_w_bm)
+        hcost._recursive_values_in_time(t=self.returns.index[t], past_returns=self.returns.iloc[:t])
         cash_ret = self.returns.iloc[t-1][-1]
         
         for i in range(10):
             self.w_plus.value = np.random.randn(self.N)
             self.w_plus.value[-1] = 1 - np.sum(self.w_plus.value[:-1])
         
             print(expression.value)
@@ -119,20 +119,20 @@
         b = pd.Series([0., 0., 1.], [self.returns.index[12], self.returns.index[23], self.returns.index[34]])
         
         tcost = TransactionCost(
             a=0.001/2, pershare_cost=pershare_cost, b=b, window_sigma_est=250, window_volume_est=250, exponent=1.5)
         
         t = self.returns.index[12]
         
-        tcost.pre_evaluation(universe=self.returns.columns, backtest_times=self.returns.index)
-        expression = tcost.compile_to_cvxpy(self.w_plus, self.z, self.w_plus_minus_w_bm)
+        tcost._recursive_pre_evaluation(universe=self.returns.columns, backtest_times=self.returns.index)
+        expression = tcost._compile_to_cvxpy(self.w_plus, self.z, self.w_plus_minus_w_bm)
         
         # only spread
         
-        tcost.values_in_time(t=self.returns.index[12], 
+        tcost._recursive_values_in_time(t=self.returns.index[12], 
             current_portfolio_value = value,
             past_returns=self.returns.iloc[:12], 
             past_volumes=self.volumes.iloc[:12],
             current_prices=pd.Series(np.ones(self.returns.shape[1]-1), self.returns.columns[:-1]))
         
         
         self.z.value = np.random.randn(self.returns.shape[1])
@@ -144,15 +144,15 @@
         self.assertTrue(np.isclose(expression.value, est_tcost_lin))
         
         
         # spread and fixed cost
         
         prices = pd.Series(np.random.uniform(1, 100, size=self.returns.shape[1]-1), self.returns.columns[:-1])
         
-        tcost.values_in_time(t=self.returns.index[23], 
+        tcost._recursive_values_in_time(t=self.returns.index[23], 
             current_portfolio_value = value,
             past_returns=self.returns.iloc[:23], 
             past_volumes=self.volumes.iloc[:23],
             current_prices=prices)
         
         
         self.z.value = np.random.randn(self.returns.shape[1])
@@ -162,15 +162,15 @@
         est_tcost_lin += np.abs(self.z.value[:-1]) @ (0.005 / prices)
         print(est_tcost_lin)
         print(expression.value)
         self.assertTrue(np.isclose(expression.value, est_tcost_lin))
         
         # spread and nonlin cost
         
-        tcost.values_in_time(t=self.returns.index[34], 
+        tcost._recursive_values_in_time(t=self.returns.index[34], 
             current_portfolio_value = value,
             past_returns=self.returns.iloc[:34], 
             past_volumes=self.volumes.iloc[:34],
             current_prices=pd.Series(np.ones(self.returns.shape[1]-1), self.returns.columns[:-1]))
         
         
         self.z.value = np.random.randn(self.returns.shape[1])
```

### Comparing `cvxportfolio-0.3.4/cvxportfolio/tests/test_data.py` & `cvxportfolio-0.3.5/cvxportfolio/tests/test_data.py`

 * *Files 0% similar despite different names*

```diff
@@ -47,17 +47,17 @@
         print('removing', cls.datadir)
         shutil.rmtree(cls.datadir)
         
         
     def test_time_series(self):
         ts = TimeSeries("ZM", base_location=self.datadir)
         assert not hasattr(ts, "data")
-        ts.pre_evaluation()
+        ts._recursive_pre_evaluation()
         assert np.all(
-            ts.values_in_time(pd.Timestamp("2023-04-11"), "foo", bar=None)
+            ts._recursive_values_in_time(pd.Timestamp("2023-04-11"), "foo", bar=None)
             == ts.data.loc["2023-04-11"]
         )
         
     def test_yfinance_download(self):
         """Test YfinanceBase."""
 
         data = YfinanceBase().download("AAPL", start="2023-04-01", end="2023-04-15")
```

### Comparing `cvxportfolio-0.3.4/cvxportfolio/tests/test_forecast.py` & `cvxportfolio-0.3.5/cvxportfolio/tests/test_forecast.py`

 * *Files 4% similar despite different names*

```diff
@@ -35,82 +35,82 @@
         # cls.volumes = pd.read_csv(Path(__file__).parent / "volumes.csv", index_col=0, parse_dates=[0])
         cls.w_plus = cp.Variable(cls.returns.shape[1])
         cls.w_plus_minus_w_bm = cp.Variable(cls.returns.shape[1])
         cls.z = cp.Variable(cls.returns.shape[1])
         cls.N = cls.returns.shape[1]
     
     # def boilerplate(self, model):
-    #     model.pre_evaluation(universe=self.returns.columns, backtest_times=self.returns.index)
-    #     return model.compile_to_cvxpy(self.w_plus, self.z, self.w_plus_minus_w_bm)
+    #     model._recursive_pre_evaluation(universe=self.returns.columns, backtest_times=self.returns.index)
+    #     return model._compile_to_cvxpy(self.w_plus, self.z, self.w_plus_minus_w_bm)
          
     
     def test_mean_update(self):
         forecaster = HistoricalMeanReturn()#lastforcash=True)
         
         returns = pd.DataFrame(self.returns, copy=True)
         returns.iloc[:20, 3:10] = np.nan
         
         for tidx in [50,51,52,55,56,57]:
             t = returns.index[tidx]
             past_returns = returns.loc[returns.index<t]
-            mean = forecaster.values_in_time(t=t, past_returns=past_returns)
+            mean = forecaster._recursive_values_in_time(t=t, past_returns=past_returns)
             # print(mean)
             # self.assertTrue(mean[-1] == past_returns.iloc[-1,-1])
             self.assertTrue(np.allclose(mean, past_returns.iloc[:,:-1].mean()))
         
     
     def test_variance_update(self):
         forecaster = HistoricalVariance(kelly=False)
         
         returns = pd.DataFrame(self.returns, copy=True)
         returns.iloc[:20, 3:10] = np.nan
         
         for tidx in [50,51,52,55,56,57]:
             t = returns.index[tidx]
             past_returns = returns.loc[returns.index<t]
-            var = forecaster.values_in_time(t=t, past_returns=past_returns)
+            var = forecaster._recursive_values_in_time(t=t, past_returns=past_returns)
             print(var)
             #self.assertTrue(mean[-1] == past_returns.iloc[-1,-1])
             self.assertTrue(np.allclose(var, past_returns.var(ddof=0)[:-1]))    
             
     def test_meanerror_update(self):
         forecaster = HistoricalMeanError()
         
         returns = pd.DataFrame(self.returns, copy=True)
         returns.iloc[:20, 3:10] = np.nan
         
         for tidx in [50,51,52,55,56,57]:
             t = returns.index[tidx]
             past_returns = returns.loc[returns.index<t]
-            val = forecaster.values_in_time(t=t, past_returns=past_returns)
+            val = forecaster._recursive_values_in_time(t=t, past_returns=past_returns)
             print(val)
             #self.assertTrue(mean[-1] == past_returns.iloc[-1,-1])
             self.assertTrue(np.allclose(val, past_returns.std(ddof=0)[:-1] / np.sqrt(past_returns.count()[:-1]) ))  
             
     def test_counts_matrix(self):
         forecaster = HistoricalFactorizedCovariance()#kelly=True)
         returns = pd.DataFrame(self.returns, copy=True)
         returns.iloc[:20, 3:10] = np.nan
         returns.iloc[10:15, 10:20] = np.nan
         
-        count_matrix = forecaster.get_count_matrix(returns)
+        count_matrix = forecaster._get_count_matrix(returns)
         
         for indexes in [(1,2), (4,5), (1,5), (7, 18), (7,24), (1,15), (13,22)]:
             print(count_matrix.iloc[indexes[0], indexes[1]])
             print(len((returns.iloc[:,indexes[0]] * returns.iloc[:,indexes[1]]).dropna()))
             self.assertTrue(np.isclose(count_matrix.iloc[indexes[0], indexes[1]],
                 len((returns.iloc[:,indexes[0]] * returns.iloc[:,indexes[1]]).dropna())))
                 
     def test_sum_matrix(self):
         forecaster = HistoricalFactorizedCovariance()#kelly=True)
         returns = pd.DataFrame(self.returns, copy=True)
         returns.iloc[:20, 3:10] = np.nan
         returns.iloc[10:15, 10:20] = np.nan
         
-        forecaster.values_in_time(t=pd.Timestamp('2022-01-01'), past_returns=returns)
+        forecaster._recursive_values_in_time(t=pd.Timestamp('2022-01-01'), past_returns=returns)
          
         sum_matrix = forecaster.last_sum_matrix
         
         for indexes in [(1,2), (4,5), (1,5), (7, 18), (7,24), (1,15), (13,22)]:
             print()
             print(sum_matrix[indexes[0], indexes[1]])
             print( (returns.iloc[:,indexes[0]] * returns.iloc[:,indexes[1]]).sum())
@@ -141,15 +141,15 @@
             res[2,0] = res[0,2]
             res[2,1] = res[1,2]
             return res
         
         for tidx in [50,51,52,55,56,57]:
             t = returns.index[tidx]
             past_returns = returns.loc[returns.index<t]
-            val = forecaster.values_in_time(t=t, past_returns=past_returns)
+            val = forecaster._recursive_values_in_time(t=t, past_returns=past_returns)
             Sigma = val @ val.T
             self.assertTrue(np.allclose(Sigma, compute_Sigma(past_returns)))
 
     def test_covariance_update_nokelly(self):
         """Test covariance forecast estimator.
         
         NOTE: due to a bug in pandas we can't test against pandas.DataFrame.cov, 
@@ -189,15 +189,15 @@
             res[2,1] = res[1,2]
             return res
         
         
         for tidx in [50,51,52,55,56,57]:
             t = returns.index[tidx]
             past_returns = returns.loc[returns.index<t]
-            val = forecaster.values_in_time(t=t, past_returns=past_returns)
+            val = forecaster._recursive_values_in_time(t=t, past_returns=past_returns)
             Sigma = val @ val.T
 
             self.assertTrue(np.allclose(Sigma, compute_Sigma(past_returns)))
             # pandasSigma = past_returns.iloc[:,:-1].cov(ddof=0)
             # self.assertTrue(np.allclose(Sigma, pandasSigma))
             self.assertTrue(np.allclose(np.diag(Sigma), past_returns.iloc[:,:-1].var(ddof=0)))
```

### Comparing `cvxportfolio-0.3.4/cvxportfolio/tests/test_policies.py` & `cvxportfolio-0.3.5/cvxportfolio/tests/test_policies.py`

 * *Files 8% similar despite different names*

```diff
@@ -44,15 +44,15 @@
         cls.z = cp.Variable(cls.returns.shape[1])
         cls.N = cls.returns.shape[1]
 
     def test_hold(self):
         hold = Hold()
         w = pd.Series(0.5, ["AAPL", "CASH"])
         self.assertTrue(np.all(
-            hold.values_in_time(current_weights=w).values == np.zeros(2)))
+            hold._recursive_values_in_time(current_weights=w).values == np.zeros(2)))
             
             
     def test_rank_and_long_short(self):
         hold = Hold()
         w = pd.Series(0.25, ["AAPL", "TSLA", "GOOGL", "CASH"])
         signal = pd.Series([1, 2, 3], ["AAPL", "TSLA", "GOOGL"])
         num_long = 1
@@ -60,15 +60,15 @@
         target_leverage = 3.0
         rls = RankAndLongShort(
             signal=signal,
             num_long=num_long,
             num_short=num_short,
             target_leverage=target_leverage,
         )
-        z = rls.values_in_time(t=None, current_weights=w)
+        z = rls._recursive_values_in_time(t=None, current_weights=w)
         print(z)
         wplus = w + z
         self.assertTrue(wplus["CASH"] == 1)
         self.assertTrue( wplus["TSLA"] == 0)
         self.assertTrue( wplus["AAPL"] == -wplus["GOOGL"])
         self.assertTrue( np.abs(wplus[:-1]).sum() == 3)
 
@@ -82,29 +82,29 @@
         )
         rls = RankAndLongShort(
             signal=signal,
             num_long=num_long,
             num_short=num_short,
             target_leverage=target_leverage,
         )
-        z1 = rls.values_in_time(t=index[0], current_weights=w)
+        z1 = rls._recursive_values_in_time(t=index[0], current_weights=w)
         print(z1)
         wplus = w + z1
         self.assertTrue( wplus["CASH"] == 1)
         self.assertTrue( wplus["TSLA"] == 0)
         self.assertTrue( wplus["AAPL"] == -wplus["GOOGL"])
         self.assertTrue( np.abs(wplus[:-1]).sum() == 3)
-        z2 = rls.values_in_time(t=index[1], current_weights=w)
+        z2 = rls._recursive_values_in_time(t=index[1], current_weights=w)
         print(z2)
         wplus = w + z2
         self.assertTrue( wplus["CASH"] == 1)
         self.assertTrue( wplus["TSLA"] == 0)
         self.assertTrue( wplus["AAPL"] == -wplus["GOOGL"])
         self.assertTrue( np.abs(wplus[:-1]).sum() == 3)
-        z3 = rls.values_in_time(t=index[2], current_weights=w)
+        z3 = rls._recursive_values_in_time(t=index[2], current_weights=w)
         wplus = w + z3
         self.assertTrue( wplus["CASH"] == 1)
         self.assertTrue( wplus["AAPL"] == 0)
         self.assertTrue( wplus["TSLA"] == -wplus["GOOGL"])
         self.assertTrue( np.abs(wplus[:-1]).sum() == 3)
         print(z3)
 
@@ -117,40 +117,40 @@
         b[-1] = 1 - sum(b[:-1])
 
         targets = pd.DataFrame({self.returns.index[3]: a,
                                 self.returns.index[15]: b
                                 }).T
         policy = ProportionalTradeToTargets(targets)
 
-        policy.pre_evaluation(universe=self.returns.columns, backtest_times=self.returns.index)
+        policy._recursive_pre_evaluation(universe=self.returns.columns, backtest_times=self.returns.index)
         start_portfolio = pd.Series(
             np.random.randn(
                 self.returns.shape[1]),
             self.returns.columns)
         start_portfolio[-1] = 1 - sum(start_portfolio[:-1])
         for t in self.returns.index[:17]:
             print(t)
             print(start_portfolio)
         
-            trade = policy.values_in_time(t=t, current_weights=start_portfolio)
+            trade = policy._recursive_values_in_time(t=t, current_weights=start_portfolio)
             start_portfolio += trade
         
             if t in targets.index:
                 self.assertTrue(np.all(start_portfolio == targets.loc[t]))
 
         self.assertTrue( np.all(trade == 0.))
         
     def test_sell_all(self):
         start_portfolio = pd.Series(
             np.random.randn(
                 self.returns.shape[1]),
             self.returns.columns)
         policy = SellAll()
         t = pd.Timestamp('2022-01-01')
-        trade = policy.values_in_time(t=t, current_weights=start_portfolio)
+        trade = policy._recursive_values_in_time(t=t, current_weights=start_portfolio)
         allcash = np.zeros(len(start_portfolio))
         allcash[-1] = 1
         assert isinstance(trade, pd.Series)
         assert np.allclose(allcash, start_portfolio + trade)
 
 
     def test_fixed_trade(self):
@@ -159,87 +159,87 @@
                 len(self.returns),
                 self.returns.shape[1]),
             index=self.returns.index,
             columns=self.returns.columns)
 
         policy = FixedTrades(fixed_trades)
         t = self.returns.index[123]
-        trade = policy.values_in_time(t=t, current_weights=pd.Series(
+        trade = policy._recursive_values_in_time(t=t, current_weights=pd.Series(
             0., self.returns.columns))
         self.assertTrue(np.all(trade == fixed_trades.loc[t]))
 
         t = pd.Timestamp('1900-01-01')
-        trade = policy.values_in_time(t=t, current_weights=trade)
+        trade = policy._recursive_values_in_time(t=t, current_weights=trade)
         self.assertTrue(np.all(trade == 0.))
 
 
     def test_fixed_weights(self):
         fixed_weights = pd.DataFrame(
             np.random.randn(
                 len(self.returns),
                 self.returns.shape[1]),
             index=self.returns.index,
             columns=self.returns.columns)
 
         policy = FixedWeights(fixed_weights)
         t = self.returns.index[123]
-        trade = policy.values_in_time(t=t, current_weights=pd.Series(
+        trade = policy._recursive_values_in_time(t=t, current_weights=pd.Series(
             0., self.returns.columns))
         self.assertTrue(np.all(trade == fixed_weights.loc[t]))
 
         t = self.returns.index[111]
-        trade = policy.values_in_time(t=t, current_weights=fixed_weights.iloc[110])
+        trade = policy._recursive_values_in_time(t=t, current_weights=fixed_weights.iloc[110])
         self.assertTrue( np.allclose(trade + fixed_weights.iloc[110], fixed_weights.loc[t]))
 
         t = pd.Timestamp('1900-01-01')
-        trade = policy.values_in_time(t=t, current_weights=trade)
+        trade = policy._recursive_values_in_time(t=t, current_weights=trade)
         self.assertTrue( np.all(trade == 0.))
 
 
     def test_periodic_rebalance(self):
 
         target = pd.Series(np.random.uniform(size=self.returns.shape[1]), self.returns.columns)
         target /= sum(target)
         rebalancing_times = pd.date_range(start=self.returns.index[0], end=self.returns.index[-1], 
             freq='7d')
 
         policy = PeriodicRebalance(target, rebalancing_times=rebalancing_times)
         init = pd.Series(np.random.randn(self.returns.shape[1]), self.returns.columns)
 
-        trade = policy.values_in_time(t=rebalancing_times[0], current_weights=init)
+        trade = policy._recursive_values_in_time(t=rebalancing_times[0], current_weights=init)
         self.assertTrue(np.allclose(trade + init, target))
 
-        trade = policy.values_in_time(t=rebalancing_times[0] + pd.Timedelta('1d'),
+        trade = policy._recursive_values_in_time(t=rebalancing_times[0] + pd.Timedelta('1d'),
             current_weights=init)
         self.assertTrue(np.allclose(trade, 0))
 
     def test_uniform(self):
         pol = Uniform()
-        pol.pre_evaluation(self.returns.columns, self.returns.index)
+        pol._recursive_pre_evaluation(self.returns.columns, self.returns.index)
         
         init = pd.Series(np.random.randn(self.returns.shape[1]), self.returns.columns)
-        trade = pol.values_in_time(t=self.returns.index[123], current_weights=init)
+        trade = pol._recursive_values_in_time(t=self.returns.index[123], current_weights=init)
         self.assertTrue(np.allclose((trade + init)[:-1], 
             np.ones(self.returns.shape[1]-1)/(self.returns.shape[1]-1)))
         
 
     def test_proportional_rebalance(self):
 
         target = pd.Series(np.random.uniform(size=self.returns.shape[1]), self.returns.columns)
         target /= sum(target)
         target_matching_times = self.returns.index[::3]
 
         policy = ProportionalRebalance(target, target_matching_times=target_matching_times)
-        policy.pre_evaluation(universe=self.returns.columns, backtest_times=self.returns.index)
+        policy._recursive_pre_evaluation(universe=self.returns.columns, backtest_times=self.returns.index)
 
         init = pd.Series(np.random.randn(self.returns.shape[1]), self.returns.columns)
 
-        trade = policy.values_in_time(t=self.returns.index[1], current_weights=init)
+        trade = policy._recursive_values_in_time(t=self.returns.index[1], current_weights=init)
         init += trade
-        trade2 = policy.values_in_time(t=self.returns.index[2], current_weights=init)
+        trade2 = policy._recursive_values_in_time(t=self.returns.index[2], current_weights=init)
         self.assertTrue(np.allclose(trade, trade2))
         self.assertTrue(np.allclose(trade + trade2 + init, target))
     
     def test_adaptive_rebalance(self):
         np.random.seed(0)
         target = pd.Series(
             np.random.uniform(
@@ -249,20 +249,20 @@
         target = pd.DataFrame({ind: target for ind in self.returns.index}).T
 
         init = pd.Series(np.random.uniform(size=self.returns.shape[1]), self.returns.columns)
         init /= sum(init)
 
         for tracking_error in [0.01, .02, .05, .1]:
             policy = AdaptiveRebalance(target, tracking_error=tracking_error)
-            trade = policy.values_in_time(t=self.returns.index[1], current_weights=init)
+            trade = policy._recursive_values_in_time(t=self.returns.index[1], current_weights=init)
             self.assertTrue(np.allclose(init + trade, target.iloc[0]))
 
         for tracking_error in [.2, .5]:
             policy = AdaptiveRebalance(target, tracking_error=tracking_error)
-            trade = policy.values_in_time(t=self.returns.index[1], current_weights=init)
+            trade = policy._recursive_values_in_time(t=self.returns.index[1], current_weights=init)
             self.assertTrue(np.allclose(trade, 0.))
 
 
     def test_single_period_optimization(self):
 
         return_forecast = ReturnsForecast()
         risk_forecast = FullCovariance(kelly=False)
@@ -276,21 +276,21 @@
             ,
             constraints=[LongOnly(), LeverageLimit(1)],
             include_cash_return=False,
             # verbose=True,
             solver='ECOS')
             
 
-        policy.pre_evaluation(universe=self.returns.columns, backtest_times=self.returns.index)
-        policy.compile_to_cvxpy()
+        policy._recursive_pre_evaluation(universe=self.returns.columns, backtest_times=self.returns.index)
+        policy._compile_to_cvxpy()
         
         curw = np.zeros(self.N)
         curw[-1] = 1.
 
-        result = policy.values_in_time(
+        result = policy._recursive_values_in_time(
             t=self.returns.index[121],
             current_weights=pd.Series(
                 curw,
                 self.returns.columns),
             current_portfolio_value=1000,
             past_returns=self.returns.iloc[:121],
             past_volumes=self.volumes.iloc[:121],
@@ -334,21 +334,21 @@
             - 2 * risk_forecast
             - TransactionCost(a=5 * 1E-4, pershare_cost=0., b=0.)  # , power=2)
             ,
             constraints=[LongOnly(), LeverageLimit(1)],
             # verbose=True,
             solver='ECOS')
 
-        policy.pre_evaluation(universe=self.returns.columns, backtest_times=self.returns.index)
-        policy.compile_to_cvxpy()
+        policy._recursive_pre_evaluation(universe=self.returns.columns, backtest_times=self.returns.index)
+        policy._compile_to_cvxpy()
 
         curw = np.zeros(self.N)
         curw[-1] = 1.
 
-        result = policy.values_in_time(
+        result = policy._recursive_values_in_time(
             t=self.returns.index[134],
             current_weights=pd.Series(
                 curw,
                 self.returns.columns),
             current_portfolio_value=1000,
             past_returns=self.returns.iloc[:134],
             past_volumes=self.volumes.iloc[:134],
@@ -356,15 +356,15 @@
 
         self.assertFalse(np.allclose(result, 0.))
 
         cvxportfolio_result = pd.Series(result, self.returns.columns)
 
         curw += result
 
-        result2 = policy.values_in_time(
+        result2 = policy._recursive_values_in_time(
             t=self.returns.index[134],
             current_weights=pd.Series(
                 curw,
                 self.returns.columns),
             current_portfolio_value=1000,
             past_returns=self.returns.iloc[:134],
             past_volumes=self.volumes.iloc[:134],
@@ -382,23 +382,23 @@
             - 2 * risk_forecast
             - TransactionCost(a=5 * 1E-4, pershare_cost=0., b=0.)  # , power=2)
             ,
             constraints=[LongOnly(), LeverageLimit(1), MaxWeights(-1)],
             # verbose=True,
             solver='ECOS')
 
-        policy.pre_evaluation(universe=self.returns.columns, backtest_times=self.returns.index)
-        policy.compile_to_cvxpy()
+        policy._recursive_pre_evaluation(universe=self.returns.columns, backtest_times=self.returns.index)
+        policy._compile_to_cvxpy()
 
 
         curw = np.zeros(self.N)
         curw[-1] = 1.
 
         with self.assertRaises(PortfolioOptimizationError):
-            result = policy.values_in_time(
+            result = policy._recursive_values_in_time(
                 t=self.returns.index[134],
                 current_weights=pd.Series(
                     curw,
                     self.returns.columns),
                 current_portfolio_value=1000,
                 past_returns=self.returns.iloc[:134],
                 past_volumes=self.volumes.iloc[:134],
@@ -414,23 +414,23 @@
             #- TransactionCost(spreads=10 * 1E-4, pershare_cost=0., b=0.)  # , power=2)
             ,
             constraints=[LongOnly(), #LeverageLimit(1), MaxWeights(-1)
         ],
             # verbose=True,
             solver='ECOS')
 
-        policy.pre_evaluation(universe=self.returns.columns, backtest_times=self.returns.index)
-        policy.compile_to_cvxpy()
+        policy._recursive_pre_evaluation(universe=self.returns.columns, backtest_times=self.returns.index)
+        policy._compile_to_cvxpy()
 
 
         curw = np.zeros(self.N)
         curw[-1] = 1.
 
         with self.assertRaises(PortfolioOptimizationError):
-            result = policy.values_in_time(
+            result = policy._recursive_values_in_time(
                 t=self.returns.index[134],
                 current_weights=pd.Series(
                     curw,
                     self.returns.columns),
                 current_portfolio_value=1000,
                 past_returns=self.returns.iloc[:134],
                 past_volumes=self.volumes.iloc[:134],
@@ -449,22 +449,22 @@
                 #- TcostModel(half_spread=5 * 1E-4)  # , power=2)
                 ,
                 constraints=[LongOnly(), LeverageLimit(1)],
                 # verbose=True,
                 planning_horizon=planning_horizon,
                 solver='ECOS')
 
-            policy.pre_evaluation(universe=self.returns.columns, backtest_times=self.returns.index)
-            policy.compile_to_cvxpy()
+            policy._recursive_pre_evaluation(universe=self.returns.columns, backtest_times=self.returns.index)
+            policy._compile_to_cvxpy()
 
 
             curw = np.zeros(self.N)
             curw[-1] = 1.
 
-            results.append(policy.values_in_time(
+            results.append(policy._recursive_values_in_time(
                 t=self.returns.index[67],
                 current_weights=pd.Series(
                     curw,
                     self.returns.columns),
                 current_portfolio_value=1000,
                 past_returns=self.returns.iloc[:67],
                 past_volumes=self.volumes.iloc[:67],
@@ -486,21 +486,21 @@
                 #- TcostModel(half_spread=5 * 1E-4)  # , power=2)
                 ,
                 constraints=[LongOnly(), LeverageLimit(1)],
                 # verbose=True,
                 planning_horizon=planning_horizon,
                 solver='ECOS')
 
-            policy.pre_evaluation(universe=self.returns.columns, backtest_times=self.returns.index)
-            policy.compile_to_cvxpy()
+            policy._recursive_pre_evaluation(universe=self.returns.columns, backtest_times=self.returns.index)
+            policy._compile_to_cvxpy()
             
             curw = np.zeros(self.N)
             curw[-1] = 1.
 
-            results.append(policy.values_in_time(
+            results.append(policy._recursive_values_in_time(
                 t=self.returns.index[67],
                 current_weights=pd.Series(
                     curw,
                     self.returns.columns),
                 current_portfolio_value=1000,
                 past_returns=self.returns.iloc[:67],
                 past_volumes=self.volumes.iloc[:67],
@@ -540,21 +540,21 @@
                 ,
                 constraints=[LongOnly(), LeverageLimit(1)],
                 #verbose=True,
                 terminal_constraint=benchmark,
                 planning_horizon=planning_horizon,
                 solver='ECOS')
 
-            policy.pre_evaluation(universe=self.returns.columns, backtest_times=self.returns.index)
-            policy.compile_to_cvxpy()
+            policy._recursive_pre_evaluation(universe=self.returns.columns, backtest_times=self.returns.index)
+            policy._compile_to_cvxpy()
             
             curw = np.zeros(self.N)
             curw[-1] = 1.
 
-            diff_to_benchmarks.append(policy.values_in_time(
+            diff_to_benchmarks.append(policy._recursive_values_in_time(
                 t=self.returns.index[67],
                 current_weights=pd.Series(
                     curw,
                     self.returns.columns),
                 current_portfolio_value=1000,
                 past_returns=self.returns.iloc[:67],
                 past_volumes=self.volumes.iloc[:67],
```

### Comparing `cvxportfolio-0.3.4/cvxportfolio/tests/test_returns.py` & `cvxportfolio-0.3.5/cvxportfolio/tests/test_returns.py`

 * *Files 2% similar despite different names*

```diff
@@ -37,79 +37,79 @@
         cls.w_plus = cp.Variable(cls.returns.shape[1])
         cls.w_plus_minus_w_bm = cp.Variable(cls.returns.shape[1])
         cls.z = cp.Variable(cls.returns.shape[1])
         cls.N = cls.returns.shape[1]
         
     def boilerplate(self, model):
         """Initialize objects, compile cvxpy expression."""
-        model.pre_evaluation(universe=self.returns.columns, backtest_times=self.returns.index)
-        return model.compile_to_cvxpy(self.w_plus, self.z, self.w_plus_minus_w_bm)
+        model._recursive_pre_evaluation(universe=self.returns.columns, backtest_times=self.returns.index)
+        return model._compile_to_cvxpy(self.w_plus, self.z, self.w_plus_minus_w_bm)
         
         
     def test_cash_returns(self):
         "Test CashReturn object with last return as forecast."
         cash_model = CashReturn()
         cvxpy_expression = self.boilerplate(cash_model)
         self.w_plus.value = np.random.randn(self.N)
-        cash_model.values_in_time(t=None, past_returns=self.returns.iloc[:123])
+        cash_model._recursive_values_in_time(t=None, past_returns=self.returns.iloc[:123])
         cr = self.returns.iloc[122, -1]
         self.assertTrue(cvxpy_expression.value == cr * (self.w_plus[-1].value + 2 * np.sum(np.minimum(self.w_plus[:-1].value, 0.))))
         
     def test_cash_returns_provided(self):
         "Test CashReturn object with provided cash returns."
         cash_model = CashReturn(self.returns.iloc[:,-1])
         cvxpy_expression = self.boilerplate(cash_model)
         self.w_plus.value = np.random.randn(self.N)
-        cash_model.values_in_time(t=self.returns.index[123], past_returns=None)
+        cash_model._recursive_values_in_time(t=self.returns.index[123], past_returns=None)
         cr = self.returns.iloc[123, -1]
         self.assertTrue(cvxpy_expression.value == cr * (self.w_plus[-1].value + 2 * np.sum(np.minimum(self.w_plus[:-1].value, 0.))))
         
     def test_returns_forecast(self):
         "Test ReturnsForecast object with provided assets' returns."
         alpha_model = ReturnsForecast(self.returns.iloc[:,:-1])
         cvxpy_expression = self.boilerplate(alpha_model)
-        alpha_model.values_in_time(t=self.returns.index[123], past_returns=None)
+        alpha_model._recursive_values_in_time(t=self.returns.index[123], past_returns=None)
         self.w_plus.value = np.random.randn(self.N)
         print(cvxpy_expression.value)
         print(self.w_plus[:-1].value @ self.returns.iloc[123][:-1]) 
         #+ ((self.w_plus[-1].value + np.sum(np.minimum(self.w_plus[:-1].value, 0.))) * self.returns.iloc[123][-1]))
         self.assertTrue(np.isclose(cvxpy_expression.value, self.w_plus[:-1].value @ self.returns.iloc[123][:-1]))
                 #+ ((self.w_plus[-1].value + 2 * np.sum(np.minimum(self.w_plus[:-1].value, 0.))) * self.returns.iloc[123][-1])))
         
         
     def test_full_returns_forecast(self):
         "Test ReturnsForecast object with historical mean forecasts."
         alpha_model = ReturnsForecast()
         cvxpy_expression = self.boilerplate(alpha_model)
         t = self.returns.index[123]
-        alpha_model.values_in_time(t=t, past_returns = self.returns.loc[self.returns.index<t])
+        alpha_model._recursive_values_in_time(t=t, past_returns = self.returns.loc[self.returns.index<t])
         self.w_plus.value = np.random.uniform(size=self.N)
         self.w_plus.value /= sum(self.w_plus.value)
         myforecast = self.returns.iloc[:, :-1].loc[self.returns.index < t].mean()
         # myforecast.iloc[-1] = self.returns.iloc[122, -1]
         self.assertTrue(np.isclose(cvxpy_expression.value, self.w_plus.value[:-1] @ myforecast))
         
     def test_returns_forecast_error(self):
         "Test ReturnsForecastError object with provided values."
         delta = self.returns.iloc[:, :-1].std(ddof=0) / np.sqrt(len(self.returns))
         # delta.iloc[-1] = 0
         error_risk = ReturnsForecastError(delta)
         cvxpy_expression = self.boilerplate(error_risk)
-        error_risk.values_in_time(t='ciao', past_returns='hello')
+        error_risk._recursive_values_in_time(t='ciao', past_returns='hello')
         self.w_plus_minus_w_bm.value = np.random.randn(self.N)
         self.assertTrue(np.isclose(cvxpy_expression.value, np.abs(self.w_plus_minus_w_bm.value[:-1]) @ delta))
 
 
     def test_full_returns_forecast_error(self):
         "Test ReturnsForecastError object with as forecast the std of the mean estimator."
         error_risk = ReturnsForecastError()
         cvxpy_expression = self.boilerplate(error_risk)
         t = self.returns.index[123]
         past_returns = self.returns.loc[self.returns.index < t]
-        error_risk.values_in_time(t=t, past_returns = past_returns)
+        error_risk._recursive_values_in_time(t=t, past_returns = past_returns)
         self.w_plus_minus_w_bm.value = np.random.randn(self.N)
         delta = past_returns.std(ddof=0) / np.sqrt(past_returns.count())
         print(cvxpy_expression.value)
         print(np.abs(self.w_plus_minus_w_bm.value[:-1]) @ delta[:-1])
         self.assertTrue(np.isclose(cvxpy_expression.value, np.abs(self.w_plus_minus_w_bm.value[:-1]) @ delta[:-1]))
```

### Comparing `cvxportfolio-0.3.4/cvxportfolio/tests/test_risks.py` & `cvxportfolio-0.3.5/cvxportfolio/tests/test_risks.py`

 * *Files 2% similar despite different names*

```diff
@@ -33,30 +33,30 @@
         cls.returns = pd.read_csv(Path(__file__).parent / "returns.csv", index_col=0, parse_dates=[0]).iloc[:, :USED_RETURNS]
         cls.w_plus = cp.Variable(cls.returns.shape[1])
         cls.w_plus_minus_w_bm = cp.Variable(cls.returns.shape[1])
         cls.z = cp.Variable(cls.returns.shape[1])
         cls.N = cls.returns.shape[1]
         
     def boilerplate(self, model):
-        model.pre_evaluation(universe=self.returns.columns, backtest_times=self.returns.index)
-        return model.compile_to_cvxpy(self.w_plus, self.z, self.w_plus_minus_w_bm)
+        model._recursive_pre_evaluation(universe=self.returns.columns, backtest_times=self.returns.index)
+        return model._compile_to_cvxpy(self.w_plus, self.z, self.w_plus_minus_w_bm)
 
 
     def test_full_sigma(self):
         historical_covariances = self.returns.iloc[:, :-1].rolling(50).cov(ddof=0).dropna()
         risk_model = FullCovariance(historical_covariances)
         
         cvxpy_expression = self.boilerplate(risk_model)
 
         self.assertTrue(cvxpy_expression.is_convex())
 
         t = historical_covariances.index[123][0]
         self.w_plus_minus_w_bm.value = np.random.randn(self.N)
 
-        risk_model.values_in_time(t=t, past_returns='Hello!')
+        risk_model._recursive_values_in_time(t=t, past_returns='Hello!')
 
         self.assertTrue(np.isclose(cvxpy_expression.value, self.w_plus_minus_w_bm.value[:-1] @
                           historical_covariances.loc[t] @ self.w_plus_minus_w_bm.value[:-1]))
                                
     def test_full_estimated_sigma(self):
 
         risk_model = FullCovariance()
@@ -64,25 +64,25 @@
         cvxpy_expression = self.boilerplate(risk_model)
         self.assertTrue(cvxpy_expression.is_convex())
 
         # N = returns.shape[1]
         # returns.iloc[:, -1] = 0.
 
         # w_plus = cp.Variable(N)
-        # risk_model.pre_evaluation(
+        # risk_model._recursive_pre_evaluation(
         #     returns.iloc[:, :], None, start_time=returns.index[50], end_time=None)
-        # cvxpy_expression = risk_model.compile_to_cvxpy(w_plus, None, None)
+        # cvxpy_expression = risk_model._compile_to_cvxpy(w_plus, None, None)
         
         t = pd.Timestamp('2014-06-02')
         past = self.returns.loc[self.returns.index < t]
         should_be = past.iloc[:,:-1].T @ past.iloc[:,:-1] / len(past)
         
         self.w_plus_minus_w_bm.value = np.random.randn(self.N) 
         
-        risk_model.values_in_time(t=t, past_returns=past)
+        risk_model._recursive_values_in_time(t=t, past_returns=past)
         print(cvxpy_expression.value)
         
         print(self.w_plus_minus_w_bm.value[:-1] @ should_be @ self.w_plus_minus_w_bm.value[:-1])
         
         self.assertTrue(np.isclose(cvxpy_expression.value,
                           self.w_plus_minus_w_bm.value[:-1] @ should_be @ self.w_plus_minus_w_bm.value[:-1]))
                           
@@ -95,15 +95,15 @@
         risk_model = DiagonalCovariance(historical_variances)
         cvxpy_expression = self.boilerplate(risk_model)
         self.assertTrue(cvxpy_expression.is_convex())
 
         t = historical_variances.index[123]
         self.w_plus_minus_w_bm.value = np.random.randn(self.N) 
 
-        risk_model.values_in_time(t, past_returns='hello')
+        risk_model._recursive_values_in_time(t=t, past_returns='hello')
 
         self.assertTrue(np.isclose(cvxpy_expression.value, self.w_plus_minus_w_bm.value[:-1] @
                           np.diag(historical_variances.loc[t]) @ self.w_plus_minus_w_bm.value[:-1]))
 
     def test_full_diagonal_covariance(self):
 
         risk_model = DiagonalCovariance()
@@ -111,15 +111,15 @@
         self.assertTrue(cvxpy_expression.is_convex())
 
         t = pd.Timestamp('2014-06-02')
         past = self.returns.loc[self.returns.index < t]
         should_be = (past**2).mean()
         should_be.iloc[-1] = 0.
         
-        risk_model.values_in_time(t=t, past_returns=past)
+        risk_model._recursive_values_in_time(t=t, past_returns=past)
         self.w_plus_minus_w_bm.value = np.random.randn(self.N) 
         
         self.assertTrue(np.isclose(cvxpy_expression.value, self.w_plus_minus_w_bm.value @
                           np.diag(should_be) @ self.w_plus_minus_w_bm.value))
 
 
     def test_forecast_error(self):
@@ -131,15 +131,15 @@
         
         self.assertTrue(cvxpy_expression.is_convex())
 
         t = historical_variances.index[123]
         
         self.w_plus_minus_w_bm.value = np.random.randn(self.N) 
 
-        risk_model.values_in_time(t, past_returns='hello')
+        risk_model._recursive_values_in_time(t=t, past_returns='hello')
 
         print(cvxpy_expression.value)
         print((np.abs(self.w_plus_minus_w_bm.value[:-1]) @ np.sqrt(historical_variances.loc[t]))**2)
         self.assertTrue(np.isclose(cvxpy_expression.value, 
         
         (np.abs(self.w_plus_minus_w_bm.value[:-1]) @ np.sqrt(historical_variances.loc[t]))**2
         
@@ -153,15 +153,15 @@
 
         t = pd.Timestamp('2014-06-02')
         
         past = self.returns.loc[self.returns.index < t]
         should_be = (past**2).mean()
         should_be.iloc[-1] = 0.
 
-        risk_model.values_in_time(t=t, past_returns=past)
+        risk_model._recursive_values_in_time(t=t, past_returns=past)
         self.w_plus_minus_w_bm.value = np.random.randn(self.N)
 
         self.assertTrue(np.isclose(cvxpy_expression.value, 
         
         (np.abs(self.w_plus_minus_w_bm.value) @ np.sqrt(should_be))**2
         
         ))
@@ -171,15 +171,15 @@
         F = pd.DataFrame(np.random.randn(2, self.N-1), columns=self.returns.columns[:-1])
         d = pd.Series(np.random.uniform(size=(self.N-1)), self.returns.columns[:-1])
         risk_model = FactorModelCovariance(F=F, d=d)
         
         cvxpy_expression = self.boilerplate(risk_model)
         self.assertTrue(cvxpy_expression.is_convex())
         
-        risk_model.values_in_time(t=self.returns.index[12], past_returns='hello')
+        risk_model._recursive_values_in_time(t=self.returns.index[12], past_returns='hello')
         self.w_plus_minus_w_bm.value = np.random.randn(self.N)
         
         self.assertTrue(np.isclose(cvxpy_expression.value, 
             self.w_plus_minus_w_bm.value[:-1] @ np.diag(d) @ self.w_plus_minus_w_bm.value[:-1] + \
                 ((F @ self.w_plus_minus_w_bm.value[:-1])**2).sum()))
                 
     def test_estimated_low_rank_covariance(self):
@@ -196,15 +196,15 @@
         FS = past.T @ past / len(past)
         FS.iloc[:, -1] = 0.
         FS.iloc[-1, :] = 0.
         eigval, eigvec = np.linalg.eigh(FS)
         F = np.sqrt(eigval[-1]) * eigvec[:, -1]
         d = np.diag(FS) - F**2
         
-        risk_model.values_in_time(t=t, past_returns=past)
+        risk_model._recursive_values_in_time(t=t, past_returns=past)
         self.w_plus_minus_w_bm.value = np.random.randn(self.N)
         
         self.assertTrue(np.isclose(cvxpy_expression.value,
             self.w_plus_minus_w_bm.value @ np.diag(d) @ self.w_plus_minus_w_bm.value + \
                 ((F @ self.w_plus_minus_w_bm.value)**2).sum()))
                 
                 
@@ -215,22 +215,22 @@
         risk_model1 = DiagonalCovariance()
         worst_case = WorstCaseRisk([risk_model0, risk_model1])
         
         cvxpy_expression = self.boilerplate(worst_case)
 
         assert cvxpy_expression.is_convex()
 
-        cvxpy_expression0 = risk_model0.compile_to_cvxpy(self.w_plus, self.z, self.w_plus_minus_w_bm)
-        cvxpy_expression1 = risk_model1.compile_to_cvxpy(self.w_plus, self.z, self.w_plus_minus_w_bm)
+        cvxpy_expression0 = risk_model0._compile_to_cvxpy(self.w_plus, self.z, self.w_plus_minus_w_bm)
+        cvxpy_expression1 = risk_model1._compile_to_cvxpy(self.w_plus, self.z, self.w_plus_minus_w_bm)
 
         self.w_plus_minus_w_bm.value = np.ones(self.N)
 
         t = pd.Timestamp('2014-06-02')
         
-        worst_case.values_in_time(t=t, past_returns=self.returns.loc[self.returns.index < t])
+        worst_case._recursive_values_in_time(t=t, past_returns=self.returns.loc[self.returns.index < t])
 
         print(cvxpy_expression.value)
         print(cvxpy_expression0.value)
         print(cvxpy_expression1.value)
         assert (cvxpy_expression.value == cvxpy_expression0.value)
         assert (cvxpy_expression.value > cvxpy_expression1.value)
```

### Comparing `cvxportfolio-0.3.4/cvxportfolio/tests/test_simulator.py` & `cvxportfolio-0.3.5/cvxportfolio/tests/test_simulator.py`

 * *Files 3% similar despite different names*

```diff
@@ -21,15 +21,15 @@
 import multiprocessing
 import time
 
 import numpy as np
 import pandas as pd
 
 from cvxportfolio.simulator import MarketSimulator, MarketData #, \
-    #simulate_stocks_holding_cost, simulate_transaction_cost, simulate_cash_holding_cost
+    #_simulate_stocks_holding_cost, _simulate_transaction_cost, _simulate_cash_holding_cost
 from cvxportfolio.estimator import DataEstimator
 
 from copy import deepcopy
 import cvxportfolio as cvx
 
 class TestSimulator(unittest.TestCase):
     
@@ -49,15 +49,15 @@
         
     @classmethod
     def tearDownClass(cls):
         """Remove data directory."""
         print('removing', cls.datadir)
         shutil.rmtree(cls.datadir)
         
-    def test_market_data_downsample(self):
+    def test_market_data__downsample(self):
         "Test downsampling of market data."
         md = MarketData(['AAPL', 'GOOG'])
         
         
         idx = md.returns.index
     
         freqs = ['weekly', 'monthly', 'quarterly'] # not doing annual because XXXX-01-01 is holiday
@@ -66,15 +66,15 @@
                     idx[(idx >= '2023-05-01') & (idx < '2023-06-01')],
                 idx[(idx >= '2022-04-01') & (idx < '2022-07-01')]  ]
         
         for i in range(len(freqs)):
             
             new_md = deepcopy(md)
         
-            new_md.downsample(freqs[i])
+            new_md._downsample(freqs[i])
             print(new_md.returns)
             self.assertTrue(np.isnan(new_md.returns.GOOG.iloc[0]))
             self.assertTrue(np.isnan(new_md.volumes.GOOG.iloc[0]))
             self.assertTrue(np.isnan(new_md.prices.GOOG.iloc[0]))
             
             if freqs[i] == 'weekly':
                 self.assertTrue(all(new_md.returns.index.weekday==0))
@@ -85,78 +85,78 @@
             self.assertTrue(all(md.prices.loc[testdays[i]] == new_md.prices.loc[testdays[i]]))
             self.assertTrue(np.allclose(md.volumes.loc[periods[i]].sum(), new_md.volumes.loc[testdays[i]]))
             self.assertTrue(np.allclose((1 + md.returns.loc[periods[i]]).prod(), 1 + new_md.returns.loc[testdays[i]]))
 
     
     def test_market_data_methods1(self):
         t = self.returns.index[10]
-        past_returns, past_volumes, current_prices = self.market_data.serve_data_policy(t)
+        past_returns, past_volumes, current_prices = self.market_data._serve_data_policy(t)
         self.assertTrue(past_returns.index[-1] < t)
         self.assertTrue(past_volumes.index[-1] < t)
         self.assertTrue(past_volumes.index[-1] == past_returns.index[-1])
         print(current_prices.name)
         print(t)
         self.assertTrue(current_prices.name == t)
         
     def test_market_data_methods2(self):
         t = self.returns.index[10]
-        current_and_past_returns, current_and_past_volumes, current_prices = self.market_data.serve_data_simulator(t)
+        current_and_past_returns, current_and_past_volumes, current_prices = self.market_data._serve_data_simulator(t)
         self.assertTrue(current_and_past_returns.index[-1] == t)
         self.assertTrue(current_and_past_volumes.index[-1] == t)
         print(current_prices.name)
         print(t)
         self.assertTrue(current_prices.name == t)
         
     def test_break_timestamp(self):
         md = MarketData(['AAPL', 'ZM', 'TSLA'], min_history=pd.Timedelta('365d'), base_location=self.datadir)
-        self.assertTrue(pd.Timestamp('2020-04-20') in md.break_timestamps)
+        self.assertTrue(pd.Timestamp('2020-04-20') in md._break_timestamps)
         # self.assertTrue(len(md.break_up_backtest('2000-01-01')) == 3)
-        self.assertTrue(md.limited_universes[pd.Timestamp('2011-06-28')] == ('AAPL', 'TSLA'))
+        self.assertTrue(md._limited_universes[pd.Timestamp('2011-06-28')] == ('AAPL', 'TSLA'))
         
         
     def test_market_data_object_safety(self):
         t = self.returns.index[10]
         
-        past_returns, past_volumes, current_prices = self.market_data.serve_data_policy(t)
+        past_returns, past_volumes, current_prices = self.market_data._serve_data_policy(t)
         
         with self.assertRaises(ValueError):
             past_returns.iloc[-2,-2] = 2.
             
         with self.assertRaises(ValueError):
             past_volumes.iloc[-1,-1] = 2.
             
         obj2 = deepcopy(self.market_data)
-        obj2.set_read_only()
+        obj2._set_read_only()
         
-        past_returns, past_volumes, current_prices = obj2.serve_data_policy(t)
+        past_returns, past_volumes, current_prices = obj2._serve_data_policy(t)
         
         with self.assertRaises(ValueError):
             current_prices.iloc[-1] = 2.
             
         current_prices.loc['BABA'] = 3.
         
-        past_returns, past_volumes, current_prices = obj2.serve_data_policy(t)
+        past_returns, past_volumes, current_prices = obj2._serve_data_policy(t)
         
         self.assertFalse( 'BABA' in current_prices.index)
         
     def test_market_data_initializations(self):
         
         used_returns = self.returns.iloc[:, :-1]
         t = self.returns.index[20]
         
         with_download_fred = MarketData(returns=used_returns, volumes=self.volumes, prices=self.prices, 
             cash_key='USDOLLAR', base_location=self.datadir)
         
         without_prices = MarketData(returns=used_returns, volumes=self.volumes, cash_key='USDOLLAR',
              base_location=self.datadir)
-        past_returns, past_volumes, current_prices = without_prices.serve_data_policy(t)
+        past_returns, past_volumes, current_prices = without_prices._serve_data_policy(t)
         self.assertTrue(current_prices is None)
         
         without_volumes = MarketData(returns=used_returns, cash_key='USDOLLAR', base_location=self.datadir)
-        current_and_past_returns, current_and_past_volumes, current_prices = without_volumes.serve_data_simulator(t)
+        current_and_past_returns, current_and_past_volumes, current_prices = without_volumes._serve_data_simulator(t)
         self.assertTrue(current_and_past_volumes is None)
         
         with self.assertRaises(SyntaxError):
             MarketData(returns=self.returns, volumes=self.volumes, prices=self.prices.iloc[:, :-1], cash_key='cash', 
                 base_location=self.datadir)
              
         with self.assertRaises(SyntaxError):
@@ -176,15 +176,15 @@
     def test_market_data_full(self):
         
         md = MarketData(['AAPL', 'ZM'], base_location=self.datadir)
         assert np.all(md.universe == ['AAPL', 'ZM', 'USDOLLAR'])
         
         t = md.returns.index[-40]
         
-        past_returns, past_volumes, current_prices = md.serve_data_policy(t)
+        past_returns, past_volumes, current_prices = md._serve_data_policy(t)
         self.assertFalse(past_volumes is None)
         self.assertFalse(current_prices is None)
         
     
     def test_simulator_raises(self):
 
         with self.assertRaises(SyntaxError):
@@ -230,18 +230,18 @@
     #
     # def test_new_tcost(self):
     #
     #     for i in range(10):
     #         np.random.seed(i)
     #         tmp = np.random.uniform(size=4)*1000
     #         tmp[3] = -sum(tmp[:3])
-    #         u = simulator.round_trade_vector(u)
+    #         u = simulator._round_trade_vector(u)
     #
     #         simulator.spreads = DataEstimator(np.random.uniform(size=3) * 1E-3)
-    #         simulator.spreads.values_in_time(t=t)
+    #         simulator.spreads._recursive_values_in_time(t=t)
     #
     #         shares = sum(np.abs(u[:-1] / simulator.prices.data.loc[t]))
     #         tcost = - simulator.per_share_fixed_cost * shares
     #         tcost -= np.abs(u[:-1]) @ simulator.spreads.data / 2
     #         tcost -= sum((np.abs(u[:-1])**1.5) * simulator.sigma_estimate.data.loc[t] / np.sqrt(simulator.volumes.data.loc[t]))
     #         sim_tcost = simulator.transaction_costs(u)
     #
@@ -249,15 +249,15 @@
     #
             
         
     def test_cash_holding_cost(self):
         
         t = self.returns.index[-40]
         
-        current_and_past_returns, current_and_past_volumes, current_prices = self.market_data.serve_data_simulator(t)
+        current_and_past_returns, current_and_past_volumes, current_prices = self.market_data._serve_data_simulator(t)
         
         cash_return = self.returns.loc[t, 'cash']
         
         hcost = cvx.HoldingCost(
             #spread_on_lending_cash_percent=0.,
             #spread_on_borrowing_cash_percent=0.,
             dividends=0.,
@@ -267,30 +267,30 @@
         
         for i in range(10):
             np.random.seed(i)
             h_plus = np.random.randn(self.returns.shape[1])*1000
             h_plus = pd.Series(h_plus, self.returns.columns)
             h_plus[-1] = 1000 - sum(h_plus[:-1])
             
-            sim_cash_hcost = hcost.simulate(t, h_plus=h_plus, current_and_past_returns=current_and_past_returns)
+            sim_cash_hcost = hcost._simulate(t, h_plus=h_plus, current_and_past_returns=current_and_past_returns)
 
             real_cash_position = h_plus[-1] + sum(np.minimum(h_plus[:-1],0.))
             if real_cash_position > 0:
                 cash_hcost = real_cash_position * (np.maximum(cash_return - 0.005/252, 0.) - cash_return)
             if real_cash_position < 0:
                 cash_hcost = real_cash_position * (0.005/252)
 
             self.assertTrue(np.isclose(cash_hcost, sim_cash_hcost))
 
 
     def test_stocks_holding_cost(self):
                 
         t = self.returns.index[-20]
         
-        current_and_past_returns, current_and_past_volumes, current_prices = self.market_data.serve_data_simulator(t)
+        current_and_past_returns, current_and_past_volumes, current_prices = self.market_data._serve_data_simulator(t)
         
         cash_return = self.returns.loc[t, 'cash']
         
         ## stock holding cost
         for i in range(10):
             np.random.seed(i)
             h_plus = np.random.randn(4)*10000
@@ -301,75 +301,75 @@
             
             hcost = cvx.HoldingCost(
                 spread_on_lending_cash_percent=0.,
                 spread_on_borrowing_cash_percent=0.,
                 dividends=dividends, periods_per_year=252)
             
             
-            sim_hcost = hcost.simulate(t=t, h_plus = h_plus, current_and_past_returns=current_and_past_returns)
+            sim_hcost = hcost._simulate(t=t, h_plus = h_plus, current_and_past_returns=current_and_past_returns)
             
             total_borrow_cost = cash_return + (0.005)/252
             hcost = -total_borrow_cost * sum(-np.minimum(h_plus,0.)[:-1])
             hcost += dividends @ h_plus[:-1]
             
             self.assertTrue(np.isclose(hcost, sim_hcost))
     
     
     def test_transaction_cost_syntax(self):
                 
         t = self.returns.index[-20]
         
-        current_and_past_returns, current_and_past_volumes, current_prices = self.market_data.serve_data_simulator(t)
+        current_and_past_returns, current_and_past_volumes, current_prices = self.market_data._serve_data_simulator(t)
         
         u = pd.Series(np.ones(len(current_prices)+1), self.universe)
         
         tcost = cvx.TransactionCost()
         # syntax checks
         with self.assertRaises(SyntaxError):
-            tcost.simulate(t, u=u, current_prices=None, 
+            tcost._simulate(t, u=u, current_prices=None, 
                             current_and_past_volumes=current_and_past_volumes, 
                             current_and_past_returns=current_and_past_returns)
         
         tcost = cvx.TransactionCost(pershare_cost=None,)
-        tcost.simulate(t, u=u, current_prices=None, 
+        tcost._simulate(t, u=u, current_prices=None, 
                         current_and_past_volumes=current_and_past_volumes, 
                         current_and_past_returns=current_and_past_returns)
         
         tcost = cvx.TransactionCost()           
         with self.assertRaises(SyntaxError):
-            tcost.simulate(t, u=u, current_prices=current_prices, 
+            tcost._simulate(t, u=u, current_prices=current_prices, 
                             current_and_past_volumes=None, 
                             current_and_past_returns=current_and_past_returns)
         
         tcost = cvx.TransactionCost(b=None)
-        tcost.simulate(t, u=u, current_prices=current_prices, 
+        tcost._simulate(t, u=u, current_prices=current_prices, 
                         current_and_past_volumes=None, 
                         current_and_past_returns=current_and_past_returns)
         
         
     def test_transaction_cost(self):
         
         t = self.returns.index[-5]
         
-        current_and_past_returns, current_and_past_volumes, current_prices = self.market_data.serve_data_simulator(t)
+        current_and_past_returns, current_and_past_volumes, current_prices = self.market_data._serve_data_simulator(t)
         print(current_prices)
                 
         n = len(current_prices)
         
         for i in range(10):
             np.random.seed(i)
             spreads = np.random.uniform(size=n)*1E-3
             u = np.random.uniform(size=n+1)*1E4
             u[-1] = -sum(u[:-1])
             u = pd.Series(u, self.universe)
-            u = MarketSimulator.round_trade_vector(u, current_prices)
+            u = MarketSimulator._round_trade_vector(u, current_prices)
             
             tcost = cvx.TransactionCost(a = spreads/2)
                         
-            sim_cost = tcost.simulate(t, u=u, current_prices=current_prices, 
+            sim_cost = tcost._simulate(t, u=u, current_prices=current_prices, 
                             current_and_past_volumes=current_and_past_volumes, 
                             current_and_past_returns=current_and_past_returns)
 
             shares = sum(np.abs(u[:-1] / current_prices))
             tcost = -0.005 * shares
             # print(tcost, sim_cost)
             tcost -= np.abs(u.iloc[:-1]) @ spreads / 2
@@ -382,50 +382,50 @@
         
 
              
     def test_methods(self):
         simulator = MarketSimulator(['ZM', 'META', 'AAPL'], base_location=self.datadir)
     
         for t in [pd.Timestamp('2023-04-13')]:#, pd.Timestamp('2022-04-11')]: # can't because sigma requires 1000 days
-            #super(simulator.__class__, simulator).values_in_time(t=t)
+            #super(simulator.__class__, simulator)._recursive_values_in_time(t=t)
             
             ## round trade
     
             for i in range(10):
                 np.random.seed(i)
                 tmp = np.random.uniform(size=4)*1000
                 tmp[3] = -sum(tmp[:3])
                 u = pd.Series(tmp, simulator.market_data.universe)
-                rounded = simulator.round_trade_vector(u, simulator.market_data.prices.loc[t])
+                rounded = simulator._round_trade_vector(u, simulator.market_data.prices.loc[t])
                 self.assertTrue(sum(rounded) == 0)
                 self.assertTrue(np.linalg.norm(rounded[:-1] - u[:-1]) < \
                     np.linalg.norm(simulator.market_data.prices.loc[t]/2))
         
                 print(u)
         
                 
-    def test_simulate_policy(self):
+    def test__simulate_policy(self):
         simulator = MarketSimulator(['META', 'AAPL'], base_location=self.datadir)
     
 
         start_time = '2023-03-10'
         end_time = '2023-04-20'
     
         ## hold
         policy = cvx.Hold()
         for i in range(10):
             np.random.seed(i)
             h = np.random.randn(3)*10000
             h[-1] = 10000 - sum(h[:-1])
             h0 = pd.Series(h, simulator.market_data.universe)
             h = pd.Series(h0, copy=True)
-            simulator.initialize_policy(policy, start_time, end_time)
+            simulator._initialize_policy(policy, start_time, end_time)
             for t in simulator.market_data.returns.index[(simulator.market_data.returns.index >= start_time) & (simulator.market_data.returns.index <= end_time)]:
                 oldcash = h[-1]
-                h, z, u, costs, timer = simulator.simulate(t=t, h=h, policy=policy)
+                h, z, u, costs, timer = simulator._simulate(t=t, h=h, policy=policy)
                 tcost, hcost = costs['TransactionCost'], costs['HoldingCost']
                 assert tcost == 0.
                 #if np.all(h0[:2] > 0):
                 #    assert hcost == 0.
                 assert np.isclose((oldcash + hcost) * (1+simulator.market_data.returns.loc[t, 'USDOLLAR']), h[-1])
             
             simh = h0[:-1] * simulator.market_data.prices.loc[pd.Timestamp(end_time) + pd.Timedelta('1d')] / simulator.market_data.prices.loc[start_time]
@@ -437,18 +437,18 @@
         
         for i in range(10):
             np.random.seed(i)
             h = np.random.randn(3)*10000
             h[-1] = 10000 - sum(h[:-1])
             h0 = pd.Series(h, simulator.market_data.returns.columns)
             h = pd.Series(h0, copy=True)
-            simulator.initialize_policy(policy, start_time, end_time)
+            simulator._initialize_policy(policy, start_time, end_time)
             for t in simulator.market_data.returns.index[(simulator.market_data.returns.index >= start_time) & (simulator.market_data.returns.index <= end_time)]:
                 oldcash = h[-1]
-                h, z, u, costs, timer = simulator.simulate(t=t, h=h, policy=policy)
+                h, z, u, costs, timer = simulator._simulate(t=t, h=h, policy=policy)
                 tcost, hcost = costs['TransactionCost'], costs['HoldingCost']
                 print(h)
                 # print(tcost, stock_hcost, cash_hcost)
             
             self.assertTrue(np.all(np.abs(h[:-1]) < simulator.market_data.prices.loc[end_time]))
             
     def test_backtest(self):
@@ -490,68 +490,68 @@
             
         pol1 = cvx.Uniform()
         
         sim = cvx.MarketSimulator(['AAPL', 'MSFT'],#', 'GE', 'CVX', 'XOM', 'AMZN', 'ORCL', 'WMT', 'HD', 'DIS', 'MCD', 'NKE']
          base_location=self.datadir)
          
         with self.assertRaises(SyntaxError):
-            result = sim.backtest([pol, pol1], pd.Timestamp('2023-01-01'), pd.Timestamp('2023-04-20'), h=['hello'])
+            result = sim.backtest_many([pol, pol1], pd.Timestamp('2023-01-01'), pd.Timestamp('2023-04-20'), h=['hello'])
             
-        result =  sim.backtest([pol1], pd.Timestamp('2023-01-01'), pd.Timestamp('2023-04-20'))
+        result =  sim.backtest(pol1, pd.Timestamp('2023-01-01'), pd.Timestamp('2023-04-20'))
         
-        result2, result3 =  sim.backtest([pol, pol1], pd.Timestamp('2023-01-01'), pd.Timestamp('2023-04-20'))
+        result2, result3 =  sim.backtest_many([pol, pol1], pd.Timestamp('2023-01-01'), pd.Timestamp('2023-04-20'))
         
         self.assertTrue(np.all(result.h == result3.h))
         
     
     def test_multiple_backtest2(self):
         """Test re-use of a worker process"""
         cpus = multiprocessing.cpu_count()
         
         sim = cvx.MarketSimulator(['AAPL', 'MSFT'], base_location=self.datadir)
         pols = [cvx.SinglePeriodOptimization(cvx.ReturnsForecast() - 1 * cvx.FullCovariance(), [cvx.LeverageLimit(1)])
             for i in range(cpus*2)]
-        results = sim.backtest(pols, pd.Timestamp('2023-01-01'), pd.Timestamp('2023-01-15'), parallel=True)
+        results = sim.backtest_many(pols, pd.Timestamp('2023-01-01'), pd.Timestamp('2023-01-15'), parallel=True)
         sharpes = [result.sharpe_ratio for result in results]
         self.assertTrue(len(set(sharpes)) == 1)
         
         
     def test_multiple_backtest3(self):
         """Test benchmarks."""
         
         
         sim = cvx.MarketSimulator(['AAPL', 'MSFT'], base_location=self.datadir)
         pols = [
             cvx.SinglePeriodOptimization(cvx.ReturnsForecast() - 1 * cvx.FullCovariance(), [cvx.LeverageLimit(1)]),
             cvx.SinglePeriodOptimization(cvx.ReturnsForecast() - 1 * cvx.FullCovariance(), [cvx.LeverageLimit(1)], benchmark=cvx.UniformBenchmark),
             cvx.SinglePeriodOptimization(cvx.ReturnsForecast() - 1 * cvx.FullCovariance(), [cvx.LeverageLimit(1)], benchmark=cvx.MarketBenchmark),
                 ]
-        results = sim.backtest(pols, pd.Timestamp('2023-01-01'), pd.Timestamp('2023-01-15'), parallel=True)
+        results = sim.backtest_many(pols, pd.Timestamp('2023-01-01'), pd.Timestamp('2023-01-15'), parallel=True)
         print(np.linalg.norm(results[0].w.sum()[:2] - .5))
         print(np.linalg.norm(results[1].w.sum()[:2] - .5))
         print(np.linalg.norm(results[2].w.sum()[:2] - .5))
         self.assertTrue( np.linalg.norm(results[1].w.sum()[:2] - .5) < np.linalg.norm(results[0].w.sum()[:2] - .5) )
         self.assertTrue( np.linalg.norm(results[1].w.sum()[:2] - .5) < np.linalg.norm(results[2].w.sum()[:2] - .5) )
         
     def test_multiple_backtest4(self):
-        """Test downsample and offline cache."""
+        """Test _downsample and offline cache."""
         
         time_first = 0.
         results_first = []
         for downsampling in ['weekly', 'monthly', 'quarterly', 'annual']:
-            sim = cvx.MarketSimulator(['AAPL', 'MSFT', 'GE'], base_location=self.datadir, trading_interval=downsampling)
+            sim = cvx.MarketSimulator(['AAPL', 'MSFT', 'GE'], base_location=self.datadir, trading_frequency=downsampling)
             pol = cvx.SinglePeriodOptimization(cvx.ReturnsForecast() - 1 * cvx.FullCovariance() - cvx.TransactionCost(exponent=1.5), [cvx.LeverageLimit(1)])
             s = time.time()
             results_first.append(sim.backtest(pol, pd.Timestamp('2021-12-01')))
             time_first += time.time() - s 
             
         time_second = 0.
         results_second = []
         for downsampling in ['weekly', 'monthly', 'quarterly', 'annual']:
-            sim = cvx.MarketSimulator(['AAPL', 'MSFT', 'GE'], base_location=self.datadir, trading_interval=downsampling)
+            sim = cvx.MarketSimulator(['AAPL', 'MSFT', 'GE'], base_location=self.datadir, trading_frequency=downsampling)
             pol = cvx.SinglePeriodOptimization(cvx.ReturnsForecast() - 1 * cvx.FullCovariance() - cvx.TransactionCost(exponent=1.5), [cvx.LeverageLimit(1)])
             s = time.time()
             results_second.append(sim.backtest(pol, pd.Timestamp('2021-12-01')))
             time_second += time.time() - s
         
         self.assertTrue(time_second < time_first)
         [self.assertTrue(np.isclose(results_first[i].sharpe_ratio, results_second[i].sharpe_ratio)) for i in range(len(results_first))]
```

### Comparing `cvxportfolio-0.3.4/cvxportfolio/tests/volumes.csv` & `cvxportfolio-0.3.5/cvxportfolio/tests/volumes.csv`

 * *Files identical despite different names*

### Comparing `cvxportfolio-0.3.4/cvxportfolio/utils.py` & `cvxportfolio-0.3.5/cvxportfolio/utils.py`

 * *Files identical despite different names*

### Comparing `cvxportfolio-0.3.4/cvxportfolio.egg-info/PKG-INFO` & `cvxportfolio-0.3.5/cvxportfolio.egg-info/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cvxportfolio
-Version: 0.3.4
+Version: 0.3.5
 Summary: Portfolio optimization.
 Home-page: https://cvxportfolio.readthedocs.io
 Author: Enzo Busseti, Stephen Boyd, Steven Diamond, BlackRock Inc.
 Author-email: enzo.busseti@gmail.com
 Maintainer: Enzo Busseti
 License: Apache 2.0
 Description-Content-Type: text/markdown
@@ -12,15 +12,15 @@
 License-File: AUTHORS
 
 # Cvxportfolio
 
 [![CVXportfolio on PyPI](https://img.shields.io/pypi/v/cvxportfolio.svg)](https://pypi.org/project/cvxportfolio/)
 [![Downloads](https://static.pepy.tech/personalized-badge/cvxportfolio?period=month&units=international_system&left_color=black&right_color=orange&left_text=PyPI%20downloads%20per%20month)](https://pepy.tech/project/cvxportfolio)
 [![Coverage Status](https://coveralls.io/repos/github/cvxgrp/cvxportfolio/badge.svg?branch=master)](https://coveralls.io/github/cvxgrp/cvxportfolio?branch=master)
-
+[![Documentation Status](https://readthedocs.org/projects/cvxportfolio/badge/?version=latest)](https://cvxportfolio.readthedocs.io/en/latest/?badge=latest)
 
 **WORK IN PROGRESS. Cvxportfolio is currently under development. We will freeze the user interface by end of 2023Q2 and release the first stable version by end of 2023Q3.**
 
 
 `cvxportfolio` is a python library for portfolio optimization and simulation
 based on the book [Multi-Period Trading via Convex Optimization](https://web.stanford.edu/~boyd/papers/pdf/cvx_portfolio.pdf)
 (also [available in print](https://www.amazon.com/Multi-Period-Trading-Convex-Optimization-Foundations/dp/1680833286/)).
```

### Comparing `cvxportfolio-0.3.4/cvxportfolio.egg-info/SOURCES.txt` & `cvxportfolio-0.3.5/cvxportfolio.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `cvxportfolio-0.3.4/setup.py` & `cvxportfolio-0.3.5/setup.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,28 +1,30 @@
 from setuptools import setup
 
 with open('README.md') as f:
     long_descr = ''.join(f.readlines())
 
 setup(
     name='cvxportfolio',
-    version='0.3.4',
+    version='0.3.5',
     author='Enzo Busseti, Stephen Boyd, Steven Diamond, BlackRock Inc.',
     maintainer='Enzo Busseti',
     author_email='enzo.busseti@gmail.com',
     packages=['cvxportfolio',
               'cvxportfolio.tests'],
     package_dir={'cvxportfolio': 'cvxportfolio'},
     package_data={'cvxportfolio': [
         'tests/returns.csv', 'tests/sigmas.csv', 'tests/volumes.csv']},
     url='https://cvxportfolio.readthedocs.io',
     license='Apache 2.0',
     description='Portfolio optimization.',
     install_requires=["pandas",
                       "numpy",
+                      "scipy<1.11.0",  # on 2023-06-26 introduced bug in cvxpy
                       "matplotlib",
                       "yfinance",
-                      "cvxpy>=1.0.6",
-                      "multiprocess"],
+                      "cvxpy",
+                      "multiprocess"
+                      ],
     long_description=long_descr,
     long_description_content_type='text/markdown',
 )
```

