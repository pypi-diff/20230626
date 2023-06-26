# Comparing `tmp/stepmix-1.2.0.tar.gz` & `tmp/stepmix-1.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "stepmix-1.2.0.tar", last modified: Mon Jun 19 18:18:43 2023, max compression
+gzip compressed data, was "stepmix-1.2.1.tar", last modified: Mon Jun 26 18:13:50 2023, max compression
```

## Comparing `stepmix-1.2.0.tar` & `stepmix-1.2.1.tar`

### file list

```diff
@@ -1,43 +1,43 @@
--rw-r--r--   0        0        0      954 2023-01-11 22:01:14.079040 stepmix-1.2.0/.github/workflows/pytest.yaml
--rw-r--r--   0        0        0       54 2023-01-11 22:01:14.079040 stepmix-1.2.0/.gitignore
--rw-r--r--   0        0        0      309 2023-01-11 22:01:14.079040 stepmix-1.2.0/.readthedocs.yaml
--rw-r--r--   0        0        0     1068 2023-01-11 22:01:14.079040 stepmix-1.2.0/LICENSE
--rw-r--r--   0        0        0     2428 2023-04-25 21:29:34.007800 stepmix-1.2.0/README-dev.md
--rw-r--r--   0        0        0     5261 2023-04-30 21:21:22.007846 stepmix-1.2.0/README.md
--rw-r--r--   0        0        0      638 2023-01-11 22:01:14.079040 stepmix-1.2.0/docs/Makefile
--rw-r--r--   0        0        0      764 2023-01-11 22:01:14.079040 stepmix-1.2.0/docs/make.bat
--rw-r--r--   0        0        0     1051 2023-05-16 17:54:29.612732 stepmix-1.2.0/docs/source/api.rst
--rw-r--r--   0        0        0     1016 2023-06-19 18:10:41.385049 stepmix-1.2.0/docs/source/conf.py
--rw-r--r--   0        0        0      955 2023-01-11 22:01:14.083040 stepmix-1.2.0/docs/source/index.rst
--rw-r--r--   0        0        0      283 2023-04-25 21:29:34.007800 stepmix-1.2.0/docs/source/installation.rst
--rw-r--r--   0        0        0     3426 2023-05-16 17:54:29.612732 stepmix-1.2.0/docs/source/tutorials.rst
--rw-r--r--   0        0        0     1884 2023-06-19 18:10:41.381049 stepmix-1.2.0/pyproject.toml
--rw-r--r--   0        0        0      557 2023-05-16 17:54:29.612732 stepmix-1.2.0/scripts/README.md
--rwxr-xr-x   0        0        0     5644 2023-05-16 17:54:29.612732 stepmix-1.2.0/scripts/run_bakk_simulation.py
--rwxr-xr-x   0        0        0     5038 2023-05-16 17:54:29.612732 stepmix-1.2.0/scripts/run_bakk_simulation_complete.py
--rw-r--r--   0        0        0      174 2023-06-19 18:10:41.381049 stepmix-1.2.0/stepmix/__init__.py
--rw-r--r--   0        0        0    10523 2023-06-19 18:10:28.893235 stepmix-1.2.0/stepmix/bootstrap.py
--rw-r--r--   0        0        0     2033 2023-01-11 22:01:14.083040 stepmix-1.2.0/stepmix/corrections.py
--rw-r--r--   0        0        0    11630 2023-03-09 22:19:26.676204 stepmix-1.2.0/stepmix/datasets.py
--rw-r--r--   0        0        0        0 2023-01-11 22:01:14.083040 stepmix-1.2.0/stepmix/emission/__init__.py
--rw-r--r--   0        0        0     1660 2023-01-11 22:01:14.083040 stepmix-1.2.0/stepmix/emission/build_emission.py
--rw-r--r--   0        0        0     8129 2023-06-19 18:10:28.893235 stepmix-1.2.0/stepmix/emission/categorical.py
--rw-r--r--   0        0        0     4831 2023-03-09 21:04:30.147441 stepmix-1.2.0/stepmix/emission/covariate.py
--rw-r--r--   0        0        0     6162 2023-06-19 18:10:28.893235 stepmix-1.2.0/stepmix/emission/emission.py
--rw-r--r--   0        0        0    15489 2023-01-12 20:57:50.331048 stepmix-1.2.0/stepmix/emission/gaussian.py
--rw-r--r--   0        0        0     4681 2023-03-09 22:19:26.676204 stepmix-1.2.0/stepmix/emission/nested.py
--rw-r--r--   0        0        0    57865 2023-06-19 18:10:28.893235 stepmix-1.2.0/stepmix/stepmix.py
--rw-r--r--   0        0        0    19721 2023-06-19 18:10:28.893235 stepmix-1.2.0/stepmix/utils.py
--rw-r--r--   0        0        0     4074 2023-05-11 17:57:51.569120 stepmix-1.2.0/test/conftest.py
--rw-r--r--   0        0        0     3608 2023-03-09 22:19:26.676204 stepmix-1.2.0/test/test_benchmarks.py
--rw-r--r--   0        0        0     5571 2023-05-11 21:02:57.820805 stepmix-1.2.0/test/test_bootstrap.py
--rw-r--r--   0        0        0      735 2023-06-19 18:10:28.893235 stepmix-1.2.0/test/test_buffers.py
--rw-r--r--   0        0        0    10743 2023-06-19 18:10:28.893235 stepmix-1.2.0/test/test_emission.py
--rw-r--r--   0        0        0     1479 2023-01-11 22:01:14.083040 stepmix-1.2.0/test/test_fiml.py
--rw-r--r--   0        0        0     1781 2023-04-30 21:21:22.007846 stepmix-1.2.0/test/test_inputs.py
--rw-r--r--   0        0        0      337 2023-05-16 17:54:29.616732 stepmix-1.2.0/test/test_progress_bar.py
--rw-r--r--   0        0        0     4284 2023-03-09 18:24:49.769774 stepmix-1.2.0/test/test_random_state.py
--rw-r--r--   0        0        0     2101 2023-05-16 17:54:29.616732 stepmix-1.2.0/test/test_sample_weight.py
--rw-r--r--   0        0        0      792 2023-06-19 18:10:28.893235 stepmix-1.2.0/test/test_sklearn.py
--rw-r--r--   0        0        0     4570 2023-01-11 22:01:14.083040 stepmix-1.2.0/test/test_steps.py
--rw-r--r--   0        0        0     6545 1970-01-01 00:00:00.000000 stepmix-1.2.0/PKG-INFO
+-rw-r--r--   0        0        0      954 2023-01-11 22:01:14.079040 stepmix-1.2.1/.github/workflows/pytest.yaml
+-rw-r--r--   0        0        0       54 2023-01-11 22:01:14.079040 stepmix-1.2.1/.gitignore
+-rw-r--r--   0        0        0      309 2023-01-11 22:01:14.079040 stepmix-1.2.1/.readthedocs.yaml
+-rw-r--r--   0        0        0     1068 2023-01-11 22:01:14.079040 stepmix-1.2.1/LICENSE
+-rw-r--r--   0        0        0     2428 2023-04-25 21:29:34.007800 stepmix-1.2.1/README-dev.md
+-rw-r--r--   0        0        0     5261 2023-04-30 21:21:22.007846 stepmix-1.2.1/README.md
+-rw-r--r--   0        0        0      638 2023-01-11 22:01:14.079040 stepmix-1.2.1/docs/Makefile
+-rw-r--r--   0        0        0      764 2023-01-11 22:01:14.079040 stepmix-1.2.1/docs/make.bat
+-rw-r--r--   0        0        0     1051 2023-05-16 17:54:29.612732 stepmix-1.2.1/docs/source/api.rst
+-rw-r--r--   0        0        0     1016 2023-06-26 18:09:07.154854 stepmix-1.2.1/docs/source/conf.py
+-rw-r--r--   0        0        0      955 2023-01-11 22:01:14.083040 stepmix-1.2.1/docs/source/index.rst
+-rw-r--r--   0        0        0      283 2023-04-25 21:29:34.007800 stepmix-1.2.1/docs/source/installation.rst
+-rw-r--r--   0        0        0     3426 2023-05-16 17:54:29.612732 stepmix-1.2.1/docs/source/tutorials.rst
+-rw-r--r--   0        0        0     1884 2023-06-26 18:09:07.154854 stepmix-1.2.1/pyproject.toml
+-rw-r--r--   0        0        0      557 2023-05-16 17:54:29.612732 stepmix-1.2.1/scripts/README.md
+-rwxr-xr-x   0        0        0     5644 2023-05-16 17:54:29.612732 stepmix-1.2.1/scripts/run_bakk_simulation.py
+-rwxr-xr-x   0        0        0     5038 2023-05-16 17:54:29.612732 stepmix-1.2.1/scripts/run_bakk_simulation_complete.py
+-rw-r--r--   0        0        0      174 2023-06-26 18:09:07.154854 stepmix-1.2.1/stepmix/__init__.py
+-rw-r--r--   0        0        0    10523 2023-06-19 18:10:28.893235 stepmix-1.2.1/stepmix/bootstrap.py
+-rw-r--r--   0        0        0     2033 2023-01-11 22:01:14.083040 stepmix-1.2.1/stepmix/corrections.py
+-rw-r--r--   0        0        0    11630 2023-03-09 22:19:26.676204 stepmix-1.2.1/stepmix/datasets.py
+-rw-r--r--   0        0        0        0 2023-01-11 22:01:14.083040 stepmix-1.2.1/stepmix/emission/__init__.py
+-rw-r--r--   0        0        0     1660 2023-01-11 22:01:14.083040 stepmix-1.2.1/stepmix/emission/build_emission.py
+-rw-r--r--   0        0        0     8129 2023-06-19 18:10:28.893235 stepmix-1.2.1/stepmix/emission/categorical.py
+-rw-r--r--   0        0        0     4831 2023-03-09 21:04:30.147441 stepmix-1.2.1/stepmix/emission/covariate.py
+-rw-r--r--   0        0        0     6162 2023-06-19 18:10:28.893235 stepmix-1.2.1/stepmix/emission/emission.py
+-rw-r--r--   0        0        0    15489 2023-01-12 20:57:50.331048 stepmix-1.2.1/stepmix/emission/gaussian.py
+-rw-r--r--   0        0        0     4681 2023-03-09 22:19:26.676204 stepmix-1.2.1/stepmix/emission/nested.py
+-rw-r--r--   0        0        0    57922 2023-06-26 18:00:08.954995 stepmix-1.2.1/stepmix/stepmix.py
+-rw-r--r--   0        0        0    19721 2023-06-19 18:10:28.893235 stepmix-1.2.1/stepmix/utils.py
+-rw-r--r--   0        0        0     4074 2023-05-11 17:57:51.569120 stepmix-1.2.1/test/conftest.py
+-rw-r--r--   0        0        0     3608 2023-03-09 22:19:26.676204 stepmix-1.2.1/test/test_benchmarks.py
+-rw-r--r--   0        0        0     5571 2023-05-11 21:02:57.820805 stepmix-1.2.1/test/test_bootstrap.py
+-rw-r--r--   0        0        0      735 2023-06-19 18:10:28.893235 stepmix-1.2.1/test/test_buffers.py
+-rw-r--r--   0        0        0    10743 2023-06-19 18:10:28.893235 stepmix-1.2.1/test/test_emission.py
+-rw-r--r--   0        0        0     1479 2023-01-11 22:01:14.083040 stepmix-1.2.1/test/test_fiml.py
+-rw-r--r--   0        0        0     1944 2023-06-26 18:00:08.954995 stepmix-1.2.1/test/test_inputs.py
+-rw-r--r--   0        0        0      337 2023-05-16 17:54:29.616732 stepmix-1.2.1/test/test_progress_bar.py
+-rw-r--r--   0        0        0     4284 2023-03-09 18:24:49.769774 stepmix-1.2.1/test/test_random_state.py
+-rw-r--r--   0        0        0     2101 2023-05-16 17:54:29.616732 stepmix-1.2.1/test/test_sample_weight.py
+-rw-r--r--   0        0        0      792 2023-06-19 18:10:28.893235 stepmix-1.2.1/test/test_sklearn.py
+-rw-r--r--   0        0        0     4570 2023-01-11 22:01:14.083040 stepmix-1.2.1/test/test_steps.py
+-rw-r--r--   0        0        0     6545 1970-01-01 00:00:00.000000 stepmix-1.2.1/PKG-INFO
```

### Comparing `stepmix-1.2.0/.github/workflows/pytest.yaml` & `stepmix-1.2.1/.github/workflows/pytest.yaml`

 * *Files identical despite different names*

### Comparing `stepmix-1.2.0/LICENSE` & `stepmix-1.2.1/LICENSE`

 * *Files identical despite different names*

### Comparing `stepmix-1.2.0/README-dev.md` & `stepmix-1.2.1/README-dev.md`

 * *Files identical despite different names*

### Comparing `stepmix-1.2.0/README.md` & `stepmix-1.2.1/README.md`

 * *Files identical despite different names*

### Comparing `stepmix-1.2.0/docs/Makefile` & `stepmix-1.2.1/docs/Makefile`

 * *Files identical despite different names*

### Comparing `stepmix-1.2.0/docs/make.bat` & `stepmix-1.2.1/docs/make.bat`

 * *Files identical despite different names*

### Comparing `stepmix-1.2.0/docs/source/api.rst` & `stepmix-1.2.1/docs/source/api.rst`

 * *Files identical despite different names*

### Comparing `stepmix-1.2.0/docs/source/conf.py` & `stepmix-1.2.1/docs/source/conf.py`

 * *Files 1% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 sys.path.insert(0, os.path.abspath("../.."))
 
 project = "StepMix"
 copyright = "2022, Labo-Lacourse"
 author = "Sacha Morin, Robin Legault"
 
 release = "0.0"
-version = "1.2.0"
+version = "1.2.1"
 
 
 # -- General configuration
 
 extensions = [
     "sphinx.ext.napoleon",
     # 'numpydoc',
```

### Comparing `stepmix-1.2.0/docs/source/index.rst` & `stepmix-1.2.1/docs/source/index.rst`

 * *Files identical despite different names*

### Comparing `stepmix-1.2.0/docs/source/tutorials.rst` & `stepmix-1.2.1/docs/source/tutorials.rst`

 * *Files identical despite different names*

### Comparing `stepmix-1.2.0/pyproject.toml` & `stepmix-1.2.1/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -38,15 +38,15 @@
 [project.optional-dependencies]
 dev = ["black", "bumpver", "flit", "pytest", "sphinx", "sphinx-rtd-theme"]
 
 [project.urls]
 Homepage = "https://stepmix.readthedocs.io/en/latest/"
 
 [tool.bumpver]
-current_version = "1.2.0"
+current_version = "1.2.1"
 version_pattern = "MAJOR.MINOR.PATCH"
 commit_message = "bump version {old_version} -> {new_version}"
 commit = true
 tag = true
 push = true
 
 [tool.bumpver.file_patterns]
```

### Comparing `stepmix-1.2.0/scripts/README.md` & `stepmix-1.2.1/scripts/README.md`

 * *Files identical despite different names*

### Comparing `stepmix-1.2.0/scripts/run_bakk_simulation.py` & `stepmix-1.2.1/scripts/run_bakk_simulation.py`

 * *Files identical despite different names*

### Comparing `stepmix-1.2.0/scripts/run_bakk_simulation_complete.py` & `stepmix-1.2.1/scripts/run_bakk_simulation_complete.py`

 * *Files identical despite different names*

### Comparing `stepmix-1.2.0/stepmix/bootstrap.py` & `stepmix-1.2.1/stepmix/bootstrap.py`

 * *Files identical despite different names*

### Comparing `stepmix-1.2.0/stepmix/corrections.py` & `stepmix-1.2.1/stepmix/corrections.py`

 * *Files identical despite different names*

### Comparing `stepmix-1.2.0/stepmix/datasets.py` & `stepmix-1.2.1/stepmix/datasets.py`

 * *Files identical despite different names*

### Comparing `stepmix-1.2.0/stepmix/emission/build_emission.py` & `stepmix-1.2.1/stepmix/emission/build_emission.py`

 * *Files identical despite different names*

### Comparing `stepmix-1.2.0/stepmix/emission/categorical.py` & `stepmix-1.2.1/stepmix/emission/categorical.py`

 * *Files identical despite different names*

### Comparing `stepmix-1.2.0/stepmix/emission/covariate.py` & `stepmix-1.2.1/stepmix/emission/covariate.py`

 * *Files identical despite different names*

### Comparing `stepmix-1.2.0/stepmix/emission/emission.py` & `stepmix-1.2.1/stepmix/emission/emission.py`

 * *Files identical despite different names*

### Comparing `stepmix-1.2.0/stepmix/emission/gaussian.py` & `stepmix-1.2.1/stepmix/emission/gaussian.py`

 * *Files identical despite different names*

### Comparing `stepmix-1.2.0/stepmix/emission/nested.py` & `stepmix-1.2.1/stepmix/emission/nested.py`

 * *Files identical despite different names*

### Comparing `stepmix-1.2.0/stepmix/stepmix.py` & `stepmix-1.2.1/stepmix/stepmix.py`

 * *Files 0% similar despite different names*

```diff
@@ -119,15 +119,15 @@
         The convergence threshold. EM iterations will stop when the
         relative lower bound average gain is below this threshold.
     max_iter : int, default=1000
         The number of EM iterations to perform.
     n_init : int, default=1
         The number of initializations to perform. The best results are kept.
     save_param_init : bool, default=False
-        Save the estimated parameters of all initializations to self.param_buffer_.
+        Save the estimated parameters of all initializations to self.param_buffer\_.
     init_params : {'kmeans', 'random'}, default='random'
         The method used to initialize the weights, the means and the
         precisions.
         Must be one of:
 
             - 'kmeans' : responsibilities are initialized using kmeans.
             - 'random' : responsibilities are initialized randomly.
@@ -1001,19 +1001,19 @@
             variables with L possible outcomes (n_features=n_columns_structural/L).
             Each row corresponds to a  single data point of the structural model.
         sample_weight : array-like of shape(n_samples,), default=None
             Array of weights that are assigned to individual samples.
             If not provided, then each sample is given unit weight.
 
         """
-        sample_weight = _check_sample_weight(sample_weight, Y, dtype=Y.dtype, copy=True)
-
         check_is_fitted(self)
         _, Y = self._check_x_y(None, Y, reset=True)
 
+        sample_weight = _check_sample_weight(sample_weight, Y, dtype=Y.dtype, copy=True)
+
         # For the third step of the 3-step approach
         random_state = check_random_state(self.random_state)
         self._initialize_parameters_structural(Y, random_state=random_state)
         self._sm.m_step(Y, resp * sample_weight[:, np.newaxis])
 
     ########################################################################################################################
     # INFERENCE
@@ -1127,14 +1127,15 @@
             Each row corresponds to a  single data point of the structural model.
         Returns
         -------
         entropy : float
         """
         check_is_fitted(self)
         resp = self.predict_proba(X, Y)
+        resp = np.clip(resp, 1e-15, 1 - 1e-15)
 
         return -1 * np.sum(resp * np.log(resp))
 
     def relative_entropy(self, X, Y=None):
         """Scaled Relative Entropy of the posterior over latent classes.
 
         Ramaswamy et al., 1993.
@@ -1153,15 +1154,15 @@
             List of n_features-dimensional data points, where each column corresponds
             to a feature for univariate variables (n_features=n_columns_structural)
             and each group of L columns corresponds to a feature for one-hot encoded
             variables with L possible outcomes (n_features=n_columns_structural/L).
             Each row corresponds to a  single data point of the structural model.
         Returns
         -------
-        entropy : float
+        relative_entropy : float
         """
         entropy = self.entropy(X, Y)
         n_samples = X.shape[0]
 
         return 1 - entropy / (n_samples * np.log(self.n_components))
 
     def predict(self, X, Y=None):
```

### Comparing `stepmix-1.2.0/stepmix/utils.py` & `stepmix-1.2.1/stepmix/utils.py`

 * *Files identical despite different names*

### Comparing `stepmix-1.2.0/test/conftest.py` & `stepmix-1.2.1/test/conftest.py`

 * *Files identical despite different names*

### Comparing `stepmix-1.2.0/test/test_benchmarks.py` & `stepmix-1.2.1/test/test_benchmarks.py`

 * *Files identical despite different names*

### Comparing `stepmix-1.2.0/test/test_bootstrap.py` & `stepmix-1.2.1/test/test_bootstrap.py`

 * *Files identical despite different names*

### Comparing `stepmix-1.2.0/test/test_buffers.py` & `stepmix-1.2.1/test/test_buffers.py`

 * *Files identical despite different names*

### Comparing `stepmix-1.2.0/test/test_emission.py` & `stepmix-1.2.1/test/test_emission.py`

 * *Files identical despite different names*

### Comparing `stepmix-1.2.0/test/test_fiml.py` & `stepmix-1.2.1/test/test_fiml.py`

 * *Files identical despite different names*

### Comparing `stepmix-1.2.0/test/test_inputs.py` & `stepmix-1.2.1/test/test_inputs.py`

 * *Files 21% similar despite different names*

```diff
@@ -2,25 +2,31 @@
 import pandas as pd
 import numpy as np
 
 from stepmix.stepmix import StepMix
 from stepmix.emission.build_emission import EMISSION_DICT
 
 
-def test_dataframe(data, kwargs):
+@pytest.mark.parametrize(
+    "n_steps,corr", [(1, None), (2, None), (3, None), (3, "BCH"), (3, "ML")]
+)
+def test_dataframe(data, kwargs, n_steps, corr):
     X, Y = data
     X_df, Y_df = pd.DataFrame(X), pd.DataFrame(Y)
 
+    kwargs["n_steps"] = n_steps
+    kwargs["correction"] = corr
+
     # Test on numpy arrays
-    model_1 = StepMix(n_steps=1, **kwargs)
+    model_1 = StepMix(**kwargs)
     model_1.fit(X, Y)
     ll_1 = model_1.score(X, Y)  # Average log-likelihood
 
     # Test on dataframes
-    model_2 = StepMix(n_steps=1, **kwargs)
+    model_2 = StepMix(**kwargs)
     model_2.fit(X_df, Y_df)
     ll_2 = model_1.score(X_df, Y_df)  # Average log-likelihood
 
     assert ll_1 == ll_2
 
 
 @pytest.mark.filterwarnings(
```

### Comparing `stepmix-1.2.0/test/test_random_state.py` & `stepmix-1.2.1/test/test_random_state.py`

 * *Files identical despite different names*

### Comparing `stepmix-1.2.0/test/test_sample_weight.py` & `stepmix-1.2.1/test/test_sample_weight.py`

 * *Files identical despite different names*

### Comparing `stepmix-1.2.0/test/test_sklearn.py` & `stepmix-1.2.1/test/test_sklearn.py`

 * *Files identical despite different names*

### Comparing `stepmix-1.2.0/test/test_steps.py` & `stepmix-1.2.1/test/test_steps.py`

 * *Files identical despite different names*

### Comparing `stepmix-1.2.0/PKG-INFO` & `stepmix-1.2.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: stepmix
-Version: 1.2.0
+Version: 1.2.1
 Summary: A Python package for stepwise estimation of latent class models with measurement and structural components. The package can also be used to fit mixture models with various observed random variables.
 Keywords: clustering,mixtures,lca,em,latent-class-analysis,expectation–maximization
 Author-email: Sacha Morin <sacha.morin@mila.quebec>, Robin Legault <robin.legault@umontreal.ca>, Charles-Édouard Giguère <ce.giguere@gmail.com>, Éric Lacourse <eric.lacourse@umontreal.ca>, Roxane de la Sablonnière <roxane.de.la.sablonniere@umontreal.ca>
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: stepmix Version: 1.2.0 Summary: A Python package
+Metadata-Version: 2.1 Name: stepmix Version: 1.2.1 Summary: A Python package
 for stepwise estimation of latent class models with measurement and structural
 components. The package can also be used to fit mixture models with various
 observed random variables. Keywords: clustering,mixtures,lca,em,latent-class-
 analysis,expectationâmaximization Author-email: Sacha Morin
 morin@mila.quebec>, Robin Legault
 legault@umontreal.ca>, Charles-Ãdouard GiguÃ¨re
 giguere@gmail.com>, Ãric Lacourse
```

