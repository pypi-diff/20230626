# Comparing `tmp/uqtestfuns-0.1.1.tar.gz` & `tmp/uqtestfuns-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "uqtestfuns-0.1.1.tar", last modified: Tue Mar  7 08:25:57 2023, max compression
+gzip compressed data, was "uqtestfuns-0.2.0.tar", last modified: Mon Jun 26 17:18:56 2023, max compression
```

## Comparing `uqtestfuns-0.1.1.tar` & `uqtestfuns-0.2.0.tar`

### file list

```diff
@@ -1,64 +1,70 @@
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-03-07 08:25:57.180280 uqtestfuns-0.1.1/
--rw-r--r--   0 runner    (1001) docker     (122)     1072 2023-03-07 08:25:48.000000 uqtestfuns-0.1.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (122)       50 2023-03-07 08:25:48.000000 uqtestfuns-0.1.1/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (122)    10086 2023-03-07 08:25:57.180280 uqtestfuns-0.1.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (122)     9012 2023-03-07 08:25:48.000000 uqtestfuns-0.1.1/README.md
--rw-r--r--   0 runner    (1001) docker     (122)      172 2023-03-07 08:25:48.000000 uqtestfuns-0.1.1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (122)     2561 2023-03-07 08:25:57.180280 uqtestfuns-0.1.1/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-03-07 08:25:57.168280 uqtestfuns-0.1.1/src/
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-03-07 08:25:57.172280 uqtestfuns-0.1.1/src/uqtestfuns/
--rw-r--r--   0 runner    (1001) docker     (122)      588 2023-03-07 08:25:48.000000 uqtestfuns-0.1.1/src/uqtestfuns/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-03-07 08:25:57.176280 uqtestfuns-0.1.1/src/uqtestfuns/core/
--rw-r--r--   0 runner    (1001) docker     (122)      293 2023-03-07 08:25:48.000000 uqtestfuns-0.1.1/src/uqtestfuns/core/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-03-07 08:25:57.176280 uqtestfuns-0.1.1/src/uqtestfuns/core/prob_input/
--rw-r--r--   0 runner    (1001) docker     (122)       61 2023-03-07 08:25:48.000000 uqtestfuns-0.1.1/src/uqtestfuns/core/prob_input/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     6496 2023-03-07 08:25:48.000000 uqtestfuns-0.1.1/src/uqtestfuns/core/prob_input/probabilistic_input.py
--rw-r--r--   0 runner    (1001) docker     (122)     4463 2023-03-07 08:25:48.000000 uqtestfuns-0.1.1/src/uqtestfuns/core/prob_input/univariate_distribution.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-03-07 08:25:57.176280 uqtestfuns-0.1.1/src/uqtestfuns/core/prob_input/univariate_distributions/
--rw-r--r--   0 runner    (1001) docker     (122)      173 2023-03-07 08:25:48.000000 uqtestfuns-0.1.1/src/uqtestfuns/core/prob_input/univariate_distributions/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     5984 2023-03-07 08:25:48.000000 uqtestfuns-0.1.1/src/uqtestfuns/core/prob_input/univariate_distributions/beta.py
--rw-r--r--   0 runner    (1001) docker     (122)     6845 2023-03-07 08:25:48.000000 uqtestfuns-0.1.1/src/uqtestfuns/core/prob_input/univariate_distributions/gumbel.py
--rw-r--r--   0 runner    (1001) docker     (122)     6096 2023-03-07 08:25:48.000000 uqtestfuns-0.1.1/src/uqtestfuns/core/prob_input/univariate_distributions/logitnormal.py
--rw-r--r--   0 runner    (1001) docker     (122)     6394 2023-03-07 08:25:48.000000 uqtestfuns-0.1.1/src/uqtestfuns/core/prob_input/univariate_distributions/lognormal.py
--rw-r--r--   0 runner    (1001) docker     (122)     6169 2023-03-07 08:25:48.000000 uqtestfuns-0.1.1/src/uqtestfuns/core/prob_input/univariate_distributions/normal.py
--rw-r--r--   0 runner    (1001) docker     (122)     6425 2023-03-07 08:25:48.000000 uqtestfuns-0.1.1/src/uqtestfuns/core/prob_input/univariate_distributions/triangular.py
--rw-r--r--   0 runner    (1001) docker     (122)     9632 2023-03-07 08:25:48.000000 uqtestfuns-0.1.1/src/uqtestfuns/core/prob_input/univariate_distributions/trunc_gumbel.py
--rw-r--r--   0 runner    (1001) docker     (122)     9350 2023-03-07 08:25:48.000000 uqtestfuns-0.1.1/src/uqtestfuns/core/prob_input/univariate_distributions/trunc_normal.py
--rw-r--r--   0 runner    (1001) docker     (122)     5254 2023-03-07 08:25:48.000000 uqtestfuns-0.1.1/src/uqtestfuns/core/prob_input/univariate_distributions/uniform.py
--rw-r--r--   0 runner    (1001) docker     (122)     2098 2023-03-07 08:25:48.000000 uqtestfuns-0.1.1/src/uqtestfuns/core/prob_input/univariate_distributions/utils.py
--rw-r--r--   0 runner    (1001) docker     (122)     3875 2023-03-07 08:25:48.000000 uqtestfuns-0.1.1/src/uqtestfuns/core/prob_input/utils.py
--rw-r--r--   0 runner    (1001) docker     (122)     1004 2023-03-07 08:25:48.000000 uqtestfuns-0.1.1/src/uqtestfuns/core/uqtestfun.py
--rw-r--r--   0 runner    (1001) docker     (122)    10025 2023-03-07 08:25:48.000000 uqtestfuns-0.1.1/src/uqtestfuns/core/uqtestfun_abc.py
--rw-r--r--   0 runner    (1001) docker     (122)     1046 2023-03-07 08:25:48.000000 uqtestfuns-0.1.1/src/uqtestfuns/core/utils.py
--rw-r--r--   0 runner    (1001) docker     (122)       85 2023-03-07 08:25:48.000000 uqtestfuns-0.1.1/src/uqtestfuns/global_settings.py
--rw-r--r--   0 runner    (1001) docker     (122)     8182 2023-03-07 08:25:48.000000 uqtestfuns-0.1.1/src/uqtestfuns/helpers.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-03-07 08:25:57.176280 uqtestfuns-0.1.1/src/uqtestfuns/meta/
--rw-r--r--   0 runner    (1001) docker     (122)      183 2023-03-07 08:25:48.000000 uqtestfuns-0.1.1/src/uqtestfuns/meta/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     1967 2023-03-07 08:25:48.000000 uqtestfuns-0.1.1/src/uqtestfuns/meta/basis_functions.py
--rw-r--r--   0 runner    (1001) docker     (122)    12619 2023-03-07 08:25:48.000000 uqtestfuns-0.1.1/src/uqtestfuns/meta/metaspec.py
--rw-r--r--   0 runner    (1001) docker     (122)     7364 2023-03-07 08:25:48.000000 uqtestfuns-0.1.1/src/uqtestfuns/meta/uqmetatestfun.py
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-03-07 08:25:48.000000 uqtestfuns-0.1.1/src/uqtestfuns/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-03-07 08:25:57.180280 uqtestfuns-0.1.1/src/uqtestfuns/test_functions/
--rw-r--r--   0 runner    (1001) docker     (122)      756 2023-03-07 08:25:48.000000 uqtestfuns-0.1.1/src/uqtestfuns/test_functions/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     5290 2023-03-07 08:25:48.000000 uqtestfuns-0.1.1/src/uqtestfuns/test_functions/ackley.py
--rw-r--r--   0 runner    (1001) docker     (122)     2579 2023-03-07 08:25:48.000000 uqtestfuns-0.1.1/src/uqtestfuns/test_functions/available.py
--rw-r--r--   0 runner    (1001) docker     (122)     5298 2023-03-07 08:25:48.000000 uqtestfuns-0.1.1/src/uqtestfuns/test_functions/borehole.py
--rw-r--r--   0 runner    (1001) docker     (122)     7240 2023-03-07 08:25:48.000000 uqtestfuns-0.1.1/src/uqtestfuns/test_functions/damped_oscillator.py
--rw-r--r--   0 runner    (1001) docker     (122)     5499 2023-03-07 08:25:48.000000 uqtestfuns-0.1.1/src/uqtestfuns/test_functions/flood.py
--rw-r--r--   0 runner    (1001) docker     (122)     4568 2023-03-07 08:25:48.000000 uqtestfuns-0.1.1/src/uqtestfuns/test_functions/ishigami.py
--rw-r--r--   0 runner    (1001) docker     (122)     2648 2023-03-07 08:25:48.000000 uqtestfuns-0.1.1/src/uqtestfuns/test_functions/oakley_ohagan_1d.py
--rw-r--r--   0 runner    (1001) docker     (122)     5340 2023-03-07 08:25:48.000000 uqtestfuns-0.1.1/src/uqtestfuns/test_functions/otl_circuit.py
--rw-r--r--   0 runner    (1001) docker     (122)     5699 2023-03-07 08:25:48.000000 uqtestfuns-0.1.1/src/uqtestfuns/test_functions/piston.py
--rw-r--r--   0 runner    (1001) docker     (122)     8713 2023-03-07 08:25:48.000000 uqtestfuns-0.1.1/src/uqtestfuns/test_functions/sobol_g.py
--rw-r--r--   0 runner    (1001) docker     (122)     8178 2023-03-07 08:25:48.000000 uqtestfuns-0.1.1/src/uqtestfuns/test_functions/sulfur.py
--rw-r--r--   0 runner    (1001) docker     (122)     1791 2023-03-07 08:25:48.000000 uqtestfuns-0.1.1/src/uqtestfuns/test_functions/utils.py
--rw-r--r--   0 runner    (1001) docker     (122)     4861 2023-03-07 08:25:48.000000 uqtestfuns-0.1.1/src/uqtestfuns/test_functions/wing_weight.py
--rw-r--r--   0 runner    (1001) docker     (122)     2007 2023-03-07 08:25:48.000000 uqtestfuns-0.1.1/src/uqtestfuns/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-03-07 08:25:57.172280 uqtestfuns-0.1.1/src/uqtestfuns.egg-info/
--rw-r--r--   0 runner    (1001) docker     (122)    10086 2023-03-07 08:25:57.000000 uqtestfuns-0.1.1/src/uqtestfuns.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (122)     2222 2023-03-07 08:25:57.000000 uqtestfuns-0.1.1/src/uqtestfuns.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (122)        1 2023-03-07 08:25:57.000000 uqtestfuns-0.1.1/src/uqtestfuns.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (122)      264 2023-03-07 08:25:57.000000 uqtestfuns-0.1.1/src/uqtestfuns.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (122)       11 2023-03-07 08:25:57.000000 uqtestfuns-0.1.1/src/uqtestfuns.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-03-07 08:25:57.180280 uqtestfuns-0.1.1/tests/
--rw-r--r--   0 runner    (1001) docker     (122)     1953 2023-03-07 08:25:48.000000 uqtestfuns-0.1.1/tests/test_list_functions.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-26 17:18:56.922831 uqtestfuns-0.2.0/
+-rw-r--r--   0 runner    (1001) docker     (122)     1072 2023-06-26 17:18:44.000000 uqtestfuns-0.2.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (122)       50 2023-06-26 17:18:44.000000 uqtestfuns-0.2.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (122)    10086 2023-06-26 17:18:56.922831 uqtestfuns-0.2.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (122)     9012 2023-06-26 17:18:44.000000 uqtestfuns-0.2.0/README.md
+-rw-r--r--   0 runner    (1001) docker     (122)      172 2023-06-26 17:18:44.000000 uqtestfuns-0.2.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (122)     2610 2023-06-26 17:18:56.922831 uqtestfuns-0.2.0/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-26 17:18:56.910832 uqtestfuns-0.2.0/src/
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-26 17:18:56.910832 uqtestfuns-0.2.0/src/uqtestfuns/
+-rw-r--r--   0 runner    (1001) docker     (122)      740 2023-06-26 17:18:44.000000 uqtestfuns-0.2.0/src/uqtestfuns/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-26 17:18:56.914831 uqtestfuns-0.2.0/src/uqtestfuns/core/
+-rw-r--r--   0 runner    (1001) docker     (122)      354 2023-06-26 17:18:44.000000 uqtestfuns-0.2.0/src/uqtestfuns/core/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-26 17:18:56.914831 uqtestfuns-0.2.0/src/uqtestfuns/core/prob_input/
+-rw-r--r--   0 runner    (1001) docker     (122)       61 2023-06-26 17:18:44.000000 uqtestfuns-0.2.0/src/uqtestfuns/core/prob_input/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2195 2023-06-26 17:18:44.000000 uqtestfuns-0.2.0/src/uqtestfuns/core/prob_input/input_spec.py
+-rw-r--r--   0 runner    (1001) docker     (122)     8331 2023-06-26 17:18:44.000000 uqtestfuns-0.2.0/src/uqtestfuns/core/prob_input/probabilistic_input.py
+-rw-r--r--   0 runner    (1001) docker     (122)     6077 2023-06-26 17:18:44.000000 uqtestfuns-0.2.0/src/uqtestfuns/core/prob_input/univariate_distribution.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-26 17:18:56.918831 uqtestfuns-0.2.0/src/uqtestfuns/core/prob_input/univariate_distributions/
+-rw-r--r--   0 runner    (1001) docker     (122)      173 2023-06-26 17:18:44.000000 uqtestfuns-0.2.0/src/uqtestfuns/core/prob_input/univariate_distributions/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     5984 2023-06-26 17:18:44.000000 uqtestfuns-0.2.0/src/uqtestfuns/core/prob_input/univariate_distributions/beta.py
+-rw-r--r--   0 runner    (1001) docker     (122)     6845 2023-06-26 17:18:44.000000 uqtestfuns-0.2.0/src/uqtestfuns/core/prob_input/univariate_distributions/gumbel.py
+-rw-r--r--   0 runner    (1001) docker     (122)     6096 2023-06-26 17:18:44.000000 uqtestfuns-0.2.0/src/uqtestfuns/core/prob_input/univariate_distributions/logitnormal.py
+-rw-r--r--   0 runner    (1001) docker     (122)     6394 2023-06-26 17:18:44.000000 uqtestfuns-0.2.0/src/uqtestfuns/core/prob_input/univariate_distributions/lognormal.py
+-rw-r--r--   0 runner    (1001) docker     (122)     6169 2023-06-26 17:18:44.000000 uqtestfuns-0.2.0/src/uqtestfuns/core/prob_input/univariate_distributions/normal.py
+-rw-r--r--   0 runner    (1001) docker     (122)     6425 2023-06-26 17:18:44.000000 uqtestfuns-0.2.0/src/uqtestfuns/core/prob_input/univariate_distributions/triangular.py
+-rw-r--r--   0 runner    (1001) docker     (122)     9632 2023-06-26 17:18:44.000000 uqtestfuns-0.2.0/src/uqtestfuns/core/prob_input/univariate_distributions/trunc_gumbel.py
+-rw-r--r--   0 runner    (1001) docker     (122)     9350 2023-06-26 17:18:44.000000 uqtestfuns-0.2.0/src/uqtestfuns/core/prob_input/univariate_distributions/trunc_normal.py
+-rw-r--r--   0 runner    (1001) docker     (122)     5254 2023-06-26 17:18:44.000000 uqtestfuns-0.2.0/src/uqtestfuns/core/prob_input/univariate_distributions/uniform.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2098 2023-06-26 17:18:44.000000 uqtestfuns-0.2.0/src/uqtestfuns/core/prob_input/univariate_distributions/utils.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3875 2023-06-26 17:18:44.000000 uqtestfuns-0.2.0/src/uqtestfuns/core/prob_input/utils.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1275 2023-06-26 17:18:44.000000 uqtestfuns-0.2.0/src/uqtestfuns/core/uqtestfun.py
+-rw-r--r--   0 runner    (1001) docker     (122)    15916 2023-06-26 17:18:44.000000 uqtestfuns-0.2.0/src/uqtestfuns/core/uqtestfun_abc.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1046 2023-06-26 17:18:44.000000 uqtestfuns-0.2.0/src/uqtestfuns/core/utils.py
+-rw-r--r--   0 runner    (1001) docker     (122)       85 2023-06-26 17:18:44.000000 uqtestfuns-0.2.0/src/uqtestfuns/global_settings.py
+-rw-r--r--   0 runner    (1001) docker     (122)     8816 2023-06-26 17:18:44.000000 uqtestfuns-0.2.0/src/uqtestfuns/helpers.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-26 17:18:56.918831 uqtestfuns-0.2.0/src/uqtestfuns/meta/
+-rw-r--r--   0 runner    (1001) docker     (122)      183 2023-06-26 17:18:44.000000 uqtestfuns-0.2.0/src/uqtestfuns/meta/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1967 2023-06-26 17:18:44.000000 uqtestfuns-0.2.0/src/uqtestfuns/meta/basis_functions.py
+-rw-r--r--   0 runner    (1001) docker     (122)    12619 2023-06-26 17:18:44.000000 uqtestfuns-0.2.0/src/uqtestfuns/meta/metaspec.py
+-rw-r--r--   0 runner    (1001) docker     (122)     7364 2023-06-26 17:18:44.000000 uqtestfuns-0.2.0/src/uqtestfuns/meta/uqmetatestfun.py
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-06-26 17:18:44.000000 uqtestfuns-0.2.0/src/uqtestfuns/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-26 17:18:56.922831 uqtestfuns-0.2.0/src/uqtestfuns/test_functions/
+-rw-r--r--   0 runner    (1001) docker     (122)     1378 2023-06-26 17:18:44.000000 uqtestfuns-0.2.0/src/uqtestfuns/test_functions/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3321 2023-06-26 17:18:44.000000 uqtestfuns-0.2.0/src/uqtestfuns/test_functions/ackley.py
+-rw-r--r--   0 runner    (1001) docker     (122)     4792 2023-06-26 17:18:44.000000 uqtestfuns-0.2.0/src/uqtestfuns/test_functions/borehole.py
+-rw-r--r--   0 runner    (1001) docker     (122)     7945 2023-06-26 17:18:44.000000 uqtestfuns-0.2.0/src/uqtestfuns/test_functions/bratley1992.py
+-rw-r--r--   0 runner    (1001) docker     (122)     6105 2023-06-26 17:18:44.000000 uqtestfuns-0.2.0/src/uqtestfuns/test_functions/damped_oscillator.py
+-rw-r--r--   0 runner    (1001) docker     (122)     4881 2023-06-26 17:18:44.000000 uqtestfuns-0.2.0/src/uqtestfuns/test_functions/flood.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1807 2023-06-26 17:18:44.000000 uqtestfuns-0.2.0/src/uqtestfuns/test_functions/forrester.py
+-rw-r--r--   0 runner    (1001) docker     (122)     9717 2023-06-26 17:18:44.000000 uqtestfuns-0.2.0/src/uqtestfuns/test_functions/franke.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3017 2023-06-26 17:18:44.000000 uqtestfuns-0.2.0/src/uqtestfuns/test_functions/gramacy2007.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3668 2023-06-26 17:18:44.000000 uqtestfuns-0.2.0/src/uqtestfuns/test_functions/ishigami.py
+-rw-r--r--   0 runner    (1001) docker     (122)     7421 2023-06-26 17:18:44.000000 uqtestfuns-0.2.0/src/uqtestfuns/test_functions/mclain.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2103 2023-06-26 17:18:44.000000 uqtestfuns-0.2.0/src/uqtestfuns/test_functions/oakley2002.py
+-rw-r--r--   0 runner    (1001) docker     (122)     4754 2023-06-26 17:18:44.000000 uqtestfuns-0.2.0/src/uqtestfuns/test_functions/otl_circuit.py
+-rw-r--r--   0 runner    (1001) docker     (122)     5040 2023-06-26 17:18:44.000000 uqtestfuns-0.2.0/src/uqtestfuns/test_functions/piston.py
+-rw-r--r--   0 runner    (1001) docker     (122)     9614 2023-06-26 17:18:44.000000 uqtestfuns-0.2.0/src/uqtestfuns/test_functions/sobol_g.py
+-rw-r--r--   0 runner    (1001) docker     (122)     7550 2023-06-26 17:18:44.000000 uqtestfuns-0.2.0/src/uqtestfuns/test_functions/sulfur.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1791 2023-06-26 17:18:44.000000 uqtestfuns-0.2.0/src/uqtestfuns/test_functions/utils.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2974 2023-06-26 17:18:44.000000 uqtestfuns-0.2.0/src/uqtestfuns/test_functions/welch1992.py
+-rw-r--r--   0 runner    (1001) docker     (122)     4263 2023-06-26 17:18:44.000000 uqtestfuns-0.2.0/src/uqtestfuns/test_functions/wing_weight.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2045 2023-06-26 17:18:44.000000 uqtestfuns-0.2.0/src/uqtestfuns/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-26 17:18:56.914831 uqtestfuns-0.2.0/src/uqtestfuns.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (122)    10086 2023-06-26 17:18:56.000000 uqtestfuns-0.2.0/src/uqtestfuns.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (122)     2474 2023-06-26 17:18:56.000000 uqtestfuns-0.2.0/src/uqtestfuns.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (122)        1 2023-06-26 17:18:56.000000 uqtestfuns-0.2.0/src/uqtestfuns.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (122)      315 2023-06-26 17:18:56.000000 uqtestfuns-0.2.0/src/uqtestfuns.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (122)       11 2023-06-26 17:18:56.000000 uqtestfuns-0.2.0/src/uqtestfuns.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-26 17:18:56.922831 uqtestfuns-0.2.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (122)     1953 2023-06-26 17:18:44.000000 uqtestfuns-0.2.0/tests/test_list_functions.py
```

### Comparing `uqtestfuns-0.1.1/LICENSE` & `uqtestfuns-0.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `uqtestfuns-0.1.1/PKG-INFO` & `uqtestfuns-0.2.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: uqtestfuns
-Version: 0.1.1
+Version: 0.2.0
 Summary: A Python3 library of test functions from the uncertainty quantification community with a common interface for benchmarking purpose.
 Home-page: https://github.com/damar-wicaksono/uqtestfuns
 Author: Damar Wicaksono
 Author-email: damar.wicaksono@outlook.com
 License: MIT
 Platform: ANY
 Classifier: License :: OSI Approved :: MIT License
@@ -22,15 +22,15 @@
 Description-Content-Type: text/markdown
 Provides-Extra: dev
 Provides-Extra: docs
 Provides-Extra: all
 License-File: LICENSE
 
 # UQTestFuns
-[![DOI](http://img.shields.io/badge/DOI-10.5281/zenodo.7701904-blue.svg?style=flat-square)](https://doi.org/10.5281/zenodo.7701904)
+[![DOI](http://img.shields.io/badge/DOI-10.5281/zenodo.7703922-blue.svg?style=flat-square)](https://doi.org/10.5281/zenodo.7703922)
 [![Code style: black](https://img.shields.io/badge/code%20style-black-000000.svg?style=flat-square)](https://github.com/psf/black)
 [![Python 3.8](https://img.shields.io/badge/python-3.7-blue.svg?style=flat-square)](https://www.python.org/downloads/release/python-370/)
 [![License](https://img.shields.io/github/license/damar-wicaksono/uqtestfuns?style=flat-square)](https://choosealicense.com/licenses/mit/)
 
 |                                  Branches                                  | Status                                                                                                                                                                                                                                                                                                                                                                                                                                                                                            |
 |:--------------------------------------------------------------------------:|---------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
 | [`main`](https://github.com/damar-wicaksono/uqtestfuns/tree/main) (stable) | ![build](https://img.shields.io/github/actions/workflow/status/damar-wicaksono/uqtestfuns/main.yml?branch=main&style=flat-square) [![codecov](https://img.shields.io/codecov/c/github/damar-wicaksono/uqtestfuns/main?logo=CodeCov&style=flat-square&token=Y6YQEPJ1TT)](https://app.codecov.io/gh/damar-wicaksono/uqtestfuns/tree/main) [![Docs](https://readthedocs.org/projects/uqtestfuns/badge/?version=stable&style=flat-square)](https://uqtestfuns.readthedocs.io/en/latest/?badge=stable) |
```

### Comparing `uqtestfuns-0.1.1/README.md` & `uqtestfuns-0.2.0/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 # UQTestFuns
-[![DOI](http://img.shields.io/badge/DOI-10.5281/zenodo.7701904-blue.svg?style=flat-square)](https://doi.org/10.5281/zenodo.7701904)
+[![DOI](http://img.shields.io/badge/DOI-10.5281/zenodo.7703922-blue.svg?style=flat-square)](https://doi.org/10.5281/zenodo.7703922)
 [![Code style: black](https://img.shields.io/badge/code%20style-black-000000.svg?style=flat-square)](https://github.com/psf/black)
 [![Python 3.8](https://img.shields.io/badge/python-3.7-blue.svg?style=flat-square)](https://www.python.org/downloads/release/python-370/)
 [![License](https://img.shields.io/github/license/damar-wicaksono/uqtestfuns?style=flat-square)](https://choosealicense.com/licenses/mit/)
 
 |                                  Branches                                  | Status                                                                                                                                                                                                                                                                                                                                                                                                                                                                                            |
 |:--------------------------------------------------------------------------:|---------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
 | [`main`](https://github.com/damar-wicaksono/uqtestfuns/tree/main) (stable) | ![build](https://img.shields.io/github/actions/workflow/status/damar-wicaksono/uqtestfuns/main.yml?branch=main&style=flat-square) [![codecov](https://img.shields.io/codecov/c/github/damar-wicaksono/uqtestfuns/main?logo=CodeCov&style=flat-square&token=Y6YQEPJ1TT)](https://app.codecov.io/gh/damar-wicaksono/uqtestfuns/tree/main) [![Docs](https://readthedocs.org/projects/uqtestfuns/badge/?version=stable&style=flat-square)](https://uqtestfuns.readthedocs.io/en/latest/?badge=stable) |
```

### Comparing `uqtestfuns-0.1.1/setup.cfg` & `uqtestfuns-0.2.0/setup.cfg`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = uqtestfuns
-version = 0.1.1
+version = 0.2.0
 url = https://github.com/damar-wicaksono/uqtestfuns
 author = Damar Wicaksono
 author_email = damar.wicaksono@outlook.com
 description = A Python3 library of test functions from the uncertainty quantification community with a common interface for benchmarking purpose.
 long_description = file: README.md
 long_description_content_type = text/markdown
 platform = ANY
@@ -29,14 +29,15 @@
 packages = find:
 include_package_data = True
 python_requires = >=3.7
 install_requires = 
 	numpy>=1.13.3
 	scipy>=1.7.3
 	tabulate>=0.8.10
+	importlib-metadata>=1.0; python_version < "3.8"
 
 [options.packages.find]
 where = src
 
 [options.extras_require]
 dev = 
 	pytest>=4.6
```

### Comparing `uqtestfuns-0.1.1/src/uqtestfuns/__init__.py` & `uqtestfuns-0.2.0/src/uqtestfuns/__init__.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,30 +1,38 @@
 """
 This is the package init for UQTestFuns.
 """
-import pkg_resources
+import sys
 
 from .core import UnivDist
 from .core import ProbInput
-from .core import UQTestFunABC
+from .core import UQTestFunBareABC, UQTestFunABC
 from .core import UQTestFun
 
+
 from . import test_functions
 from .test_functions import *  # noqa
 
 from .meta import UQMetaFunSpec
 from .meta import UQMetaTestFun
 
 from .helpers import list_functions
 
-__version__ = pkg_resources.require("uqtestfuns")[0].version
+if sys.version_info >= (3, 8):
+    from importlib import metadata
+else:
+    import importlib_metadata as metadata
+
+__version__ = metadata.version("uqtestfuns")
 
 __all__ = [
     "UnivDist",
     "ProbInput",
     "UQTestFunABC",
+    "UQTestFunBareABC",
+    "UQTestFunABC",
     "UQTestFun",
     "test_functions",
     "UQMetaFunSpec",
     "UQMetaTestFun",
     "list_functions",
 ]
```

### Comparing `uqtestfuns-0.1.1/src/uqtestfuns/core/prob_input/probabilistic_input.py` & `uqtestfuns-0.2.0/src/uqtestfuns/core/prob_input/probabilistic_input.py`

 * *Files 22% similar despite different names*

```diff
@@ -4,51 +4,62 @@
 The ``ProbInput`` class represents a probabilistic input model.
 Each probabilistic input has a set of one-dimensional marginals each of which
 is defined by an instance of the ``UnivDist`` class.
 """
 from __future__ import annotations
 
 import numpy as np
+
+from dataclasses import dataclass, field
+from numpy.random._generator import Generator
 from tabulate import tabulate
 from typing import Any, List, Optional, Union, Tuple
-from dataclasses import dataclass, field
 
 from .univariate_distribution import UnivDist, FIELD_NAMES
-
+from .input_spec import ProbInputSpecFixDim, ProbInputSpecVarDim
 
 __all__ = ["ProbInput"]
 
 
 @dataclass
 class ProbInput:
     """A class for multivariate input variables.
 
     Parameters
     ----------
     marginals : Union[List[UnivDist], Tuple[UnivDist, ...]]
-        A list of one-dimensional marginals (univariate random variables)
+        A list of one-dimensional marginals (univariate random variables).
     copulas : Any
         Copulas between univariate inputs that define dependence structure
-        (currently not used)
+        (currently not used).
     name : str, optional
-        The name of the probabilistic input model
+        The name of the probabilistic input model.
     description : str, optional
-        The short description regarding the input model
+        The short description regarding the input model.
+    rng_seed : int, optional.
+        The seed used to initialize the pseudo-random number generator.
+        If not specified, the value is taken from the system entropy.
 
     Attributes
     ----------
     spatial_dimension : int
         Number of constituents (random) input variables.
+    _rng : Generator
+        The default pseudo-random number generator of NumPy.
+        The generator is only created if or when needed (e.g., generating
+        a random sample from the distribution).
     """
 
     spatial_dimension: int = field(init=False)
     marginals: Union[List[UnivDist], Tuple[UnivDist, ...]]
     copulas: Any = None
     name: Optional[str] = None
     description: Optional[str] = None
+    rng_seed: Optional[int] = field(default=None, repr=False)
+    _rng: Optional[Generator] = field(init=False, default=None, repr=False)
 
     def __post_init__(self):
         self.spatial_dimension = len(self.marginals)
         # Protect marginals by making it immutable
         self.marginals = tuple(self.marginals)
 
     def transform_sample(self, xx: np.ndarray, other: ProbInput):
@@ -84,21 +95,23 @@
         Returns
         -------
         np.ndarray
             The generated sample in an :math:`N`-by-:math:`M` array
             where :math:`N` and :math:`M` are the sample size
             and the number of spatial dimensions, respectively.
         """
+        if self._rng is None:  # pragma: no cover
+            # Create a pseudo-random number generator (lazy evaluation)
+            self._rng = np.random.default_rng(self.rng_seed)
 
-        xx = np.empty((sample_size, self.spatial_dimension))
-        # Transform the sample in [0, 1] to the domain of the distribution
+        xx = self._rng.random((sample_size, self.spatial_dimension))
         if not self.copulas:
-            # Independent inputs generate sample marginal by marginal
+            # Transform the sample in [0, 1] to the domain of the distribution
             for idx_dim, marginal in enumerate(self.marginals):
-                xx[:, idx_dim] = marginal.get_sample(sample_size)
+                xx[:, idx_dim] = marginal.icdf(xx[:, idx_dim])
         else:
             raise ValueError("Copulas are not currently supported!")
 
         return xx
 
     def pdf(self, xx: np.ndarray) -> np.ndarray:
         """Get the PDF value of the distribution on a set of values.
@@ -166,14 +179,45 @@
         )
 
         table += "\n"
         table += f"<p><b>Copulas</b>:&nbsp;{self.copulas}</p>"
 
         return table
 
+    @classmethod
+    def from_spec(
+        cls,
+        prob_input_spec: Union[ProbInputSpecFixDim, ProbInputSpecVarDim],
+        *,
+        spatial_dimension: Optional[int] = None,
+        rng_seed: Optional[int] = None,
+    ):
+        """Create an instance from a ProbInputSpec instance."""
+
+        if isinstance(prob_input_spec, ProbInputSpecVarDim):
+            if spatial_dimension is None:
+                raise ValueError("Spatial dimension must be specified!")
+            marginals_gen = prob_input_spec.marginals_generator
+            marginals_spec = marginals_gen(spatial_dimension)
+        else:
+            marginals_spec = prob_input_spec.marginals
+
+        # Create a list of UnivDist instances representing univariate marginals
+        marginals = [
+            UnivDist.from_spec(marginal) for marginal in marginals_spec
+        ]
+
+        return cls(
+            marginals=marginals,
+            copulas=prob_input_spec.copulas,
+            name=prob_input_spec.name,
+            description=prob_input_spec.description,
+            rng_seed=rng_seed,
+        )
+
 
 def _get_values_as_list(
     univ_inputs: Union[List[UnivDist], Tuple[UnivDist, ...]],
     field_names: List[str],
 ) -> list:
     """Get the values from each field from a list of UnivariateInput
```

### Comparing `uqtestfuns-0.1.1/src/uqtestfuns/core/prob_input/univariate_distribution.py` & `uqtestfuns-0.2.0/src/uqtestfuns/core/prob_input/univariate_distribution.py`

 * *Files 22% similar despite different names*

```diff
@@ -4,26 +4,28 @@
 The ``UnivDist`` class represents a univariate random variable.
 Each random variable has a (parametric) probability distribution.
 """
 from __future__ import annotations
 
 import numpy as np
 
+from numpy.random._generator import Generator
 from numpy.typing import ArrayLike
 from dataclasses import dataclass, field
 from typing import Optional, Union
 
 from .utils import (
     verify_distribution,
     get_distribution_bounds,
     verify_parameters,
     get_pdf_values,
     get_cdf_values,
     get_icdf_values,
 )
+from .input_spec import UnivDistSpec
 from ...global_settings import ARRAY_FLOAT
 
 __all__ = ["UnivDist"]
 
 # Ordered field names for printing purpose
 FIELD_NAMES = ["name", "distribution", "parameters", "description"]
 
@@ -38,29 +40,38 @@
         The type of the probability distribution
     parameters : ArrayLike
         The parameters of the chosen probability distribution
     name : str, optional
         The name of the random variable
     description : str, optional
         The short text description of the random variable
+    rng_seed : int, optional.
+        The seed used to initialize the pseudo-random number generator.
+        If not specified, the value is taken from the system entropy.
 
     Attributes
     ----------
     lower : float
         The lower bound of the distribution
     upper : float
         The upper bound of the distribution
+    _rng : Generator
+        The default pseudo-random number generator of NumPy.
+        The generator is only created if or when needed (e.g., generating
+        a random sample from the distribution).
     """
 
     distribution: str
     parameters: ArrayLike
     name: Optional[str] = None
     description: Optional[str] = None
     lower: float = field(init=False, repr=False)
     upper: float = field(init=False, repr=False)
+    rng_seed: Optional[int] = field(default=None, repr=False)
+    _rng: Optional[Generator] = field(init=False, default=None, repr=False)
 
     def __post_init__(self) -> None:
         # Because frozen=True, post init must access self via setattr
         # Make sure the distribution is lower-case
         object.__setattr__(self, "distribution", self.distribution.lower())
 
         # Convert parameters to a numpy array
@@ -96,15 +107,20 @@
             other.parameters,
             other.lower,
             other.upper,
         )
 
     def get_sample(self, sample_size: int = 1) -> np.ndarray:
         """Get a random sample from the distribution."""
-        xx = np.random.rand(sample_size)
+        if self._rng is None:  # pragma: no cover
+            # Create a pseudo-random number generator (lazy evaluation)
+            rng = np.random.default_rng(self.rng_seed)
+            object.__setattr__(self, "_rng", rng)
+
+        xx = self._rng.random(sample_size)  # type: ignore
 
         return get_icdf_values(
             xx, self.distribution, self.parameters, self.lower, self.upper
         )
 
     def pdf(self, xx: Union[float, np.ndarray]) -> ARRAY_FLOAT:
         """Compute the PDF of the distribution on a set of values."""
@@ -138,7 +154,29 @@
         """
         # TODO: verify that the input is in [0, 1]
         xx = np.asarray(xx)
 
         return get_icdf_values(
             xx, self.distribution, self.parameters, self.lower, self.upper
         )
+
+    @classmethod
+    def from_spec(
+        cls, marginal_spec: UnivDistSpec, rng_seed: Optional[int] = None
+    ):
+        """Create an instance of UnivDist from a marginal specification.
+
+        Parameters
+        ----------
+        marginal_spec : UnivDistSpec
+            The specification for the univariate marginal.
+        rng_seed : int, optional
+            The seed used to initialize the pseudo-random number generator.
+            If not specified, the value is taken from the system entropy.
+        """
+        return cls(
+            distribution=marginal_spec.distribution,
+            parameters=marginal_spec.parameters,
+            name=marginal_spec.name,
+            description=marginal_spec.description,
+            rng_seed=rng_seed,
+        )
```

### Comparing `uqtestfuns-0.1.1/src/uqtestfuns/core/prob_input/univariate_distributions/beta.py` & `uqtestfuns-0.2.0/src/uqtestfuns/core/prob_input/univariate_distributions/beta.py`

 * *Files identical despite different names*

### Comparing `uqtestfuns-0.1.1/src/uqtestfuns/core/prob_input/univariate_distributions/gumbel.py` & `uqtestfuns-0.2.0/src/uqtestfuns/core/prob_input/univariate_distributions/gumbel.py`

 * *Files identical despite different names*

### Comparing `uqtestfuns-0.1.1/src/uqtestfuns/core/prob_input/univariate_distributions/logitnormal.py` & `uqtestfuns-0.2.0/src/uqtestfuns/core/prob_input/univariate_distributions/logitnormal.py`

 * *Files identical despite different names*

### Comparing `uqtestfuns-0.1.1/src/uqtestfuns/core/prob_input/univariate_distributions/lognormal.py` & `uqtestfuns-0.2.0/src/uqtestfuns/core/prob_input/univariate_distributions/lognormal.py`

 * *Files identical despite different names*

### Comparing `uqtestfuns-0.1.1/src/uqtestfuns/core/prob_input/univariate_distributions/normal.py` & `uqtestfuns-0.2.0/src/uqtestfuns/core/prob_input/univariate_distributions/normal.py`

 * *Files identical despite different names*

### Comparing `uqtestfuns-0.1.1/src/uqtestfuns/core/prob_input/univariate_distributions/triangular.py` & `uqtestfuns-0.2.0/src/uqtestfuns/core/prob_input/univariate_distributions/triangular.py`

 * *Files identical despite different names*

### Comparing `uqtestfuns-0.1.1/src/uqtestfuns/core/prob_input/univariate_distributions/trunc_gumbel.py` & `uqtestfuns-0.2.0/src/uqtestfuns/core/prob_input/univariate_distributions/trunc_gumbel.py`

 * *Files identical despite different names*

### Comparing `uqtestfuns-0.1.1/src/uqtestfuns/core/prob_input/univariate_distributions/trunc_normal.py` & `uqtestfuns-0.2.0/src/uqtestfuns/core/prob_input/univariate_distributions/trunc_normal.py`

 * *Files identical despite different names*

### Comparing `uqtestfuns-0.1.1/src/uqtestfuns/core/prob_input/univariate_distributions/uniform.py` & `uqtestfuns-0.2.0/src/uqtestfuns/core/prob_input/univariate_distributions/uniform.py`

 * *Files identical despite different names*

### Comparing `uqtestfuns-0.1.1/src/uqtestfuns/core/prob_input/univariate_distributions/utils.py` & `uqtestfuns-0.2.0/src/uqtestfuns/core/prob_input/univariate_distributions/utils.py`

 * *Files identical despite different names*

### Comparing `uqtestfuns-0.1.1/src/uqtestfuns/core/prob_input/utils.py` & `uqtestfuns-0.2.0/src/uqtestfuns/core/prob_input/utils.py`

 * *Files identical despite different names*

### Comparing `uqtestfuns-0.1.1/src/uqtestfuns/core/uqtestfun.py` & `uqtestfuns-0.2.0/src/uqtestfuns/core/uqtestfun.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,41 +1,44 @@
 """
 This module contains the concrete implementation of a generic class to
 create a UQ test function in runtime or within a running Python session.
 """
 from typing import Any, Callable, Optional
 
-from .uqtestfun_abc import UQTestFunABC
+from .uqtestfun_abc import UQTestFunBareABC
 from .prob_input.probabilistic_input import ProbInput
 
 __all__ = ["UQTestFun"]
 
 
-class UQTestFun(UQTestFunABC):
-    """Generic concrete class of UQ test function."""
+class UQTestFun(UQTestFunBareABC):
+    """Generic concrete class of UQ test function.
 
-    _TAGS = None
-
-    _AVAILABLE_INPUTS = None
-
-    _AVAILABLE_PARAMETERS = None
-
-    _DEFAULT_SPATIAL_DIMENSION = None
-
-    _DESCRIPTION = None
+    Parameters
+    ----------
+    evaluate : Callable
+        The evaluation function of the UQ test function implemented as a
+        Python callable.
+    prob_input : ProbInput
+        The probabilistic input model of the UQ test function.
+    parameters : Any, optional
+        The parameters set of the UQ test function.
+        If not specified, `None` is used.
+    name : str, optional
+        The name of the UQ test function.
+    """
 
     def __init__(
         self,
         evaluate: Callable,
-        prob_input: Optional[ProbInput] = None,
+        prob_input: ProbInput,
         parameters: Optional[Any] = None,
         name: Optional[str] = None,
     ):
         self._evaluate = evaluate
-
         super().__init__(prob_input, parameters, name)
 
     def evaluate(self, xx):
-        if self.parameters is None:
-            return self._evaluate(xx)
-        else:
+        if self.parameters is not None:
             return self._evaluate(xx, self.parameters)
+
+        return self._evaluate(xx)
```

### Comparing `uqtestfuns-0.1.1/src/uqtestfuns/core/utils.py` & `uqtestfuns-0.2.0/src/uqtestfuns/core/utils.py`

 * *Files identical despite different names*

### Comparing `uqtestfuns-0.1.1/src/uqtestfuns/helpers.py` & `uqtestfuns-0.2.0/src/uqtestfuns/helpers.py`

 * *Files 11% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 -----
 - High-level functions typically contain many guardrails against invalidity
   of the input arguments.
 """
 from tabulate import tabulate as tbl  # 'tabulate' is used as a parameter name
 from .utils import get_available_classes, SUPPORTED_TAGS
 from . import test_functions
-from typing import List, Optional, Tuple, Union, Dict
+from typing import List, Optional, Union
 
 from .core import UQTestFunABC
 
 __all__ = ["list_functions"]
 
 
 def list_functions(
@@ -50,17 +50,15 @@
       intersected. Entries that satisfy both are returned.
     """
 
     # --- Parse input arguments
     _verify_input_args(spatial_dimension, tag, tabulate)
 
     # --- Get all the available classes that implement the test functions
-    available_classes: List[Tuple[str, UQTestFunABC]] = get_available_classes(
-        test_functions
-    )
+    available_classes = get_available_classes(test_functions)
     available_classes_dict = dict(available_classes)
 
     # --- Filter according to the requested spatial dimension
     if spatial_dimension:
         available_classes_from_dimension = _get_functions_from_dimension(
             available_classes_dict, spatial_dimension
         )
@@ -90,52 +88,78 @@
         for available_class_name in available_class_names:
             constructor = available_classes_dict[available_class_name]
             constructors.append(constructor)
 
         return constructors
 
     # --- Create a tabulated view of the list
-    header_names = [
-        "No.",
-        "Constructor",
-        "Spatial Dimension",
-        "Application",
-        "Description",
-    ]
+    if tag is None:
+        header_names = [
+            "No.",
+            "Constructor",
+            "Dimension",
+            "Application",
+            "Description",
+        ]
+    else:
+        header_names = [
+            "No.",
+            "Constructor",
+            "Dimension",
+            "Description",
+        ]
 
     values = []
     for idx, available_class_name in enumerate(
         sorted(list(available_class_names))
     ):
         available_class = available_classes_dict[available_class_name]
 
-        default_spatial_dimension = available_class.DEFAULT_SPATIAL_DIMENSION
-        if not default_spatial_dimension:
+        if not available_class.default_spatial_dimension:
             default_spatial_dimension = "M"
+        else:
+            default_spatial_dimension = (
+                available_class.default_spatial_dimension
+            )
 
-        tags = ", ".join(available_class.TAGS)
+        description = available_class.description
 
-        description = available_class.DESCRIPTION
-
-        value = [
-            idx + 1,
-            f"{available_class_name}()",
-            f"{default_spatial_dimension}",
-            tags,
-            f"{description}",
-        ]
+        if tag is None:
+            tags = ", ".join(available_class.tags)
+            value = [
+                idx + 1,
+                f"{available_class_name}()",
+                f"{default_spatial_dimension}",
+                tags,
+                f"{description}",
+            ]
+        else:
+            value = [
+                idx + 1,
+                f"{available_class_name}()",
+                f"{default_spatial_dimension}",
+                f"{description}",
+            ]
 
         values.append(value)
 
-    table = tbl(
-        values,
-        headers=header_names,
-        stralign="center",
-        colalign=("center", "center", "center", "center", "left"),
-    )
+    if tag is None:
+        table = tbl(
+            values,
+            headers=header_names,
+            stralign="center",
+            colalign=("center", "center", "center", "center", "left"),
+        )
+    else:
+        table = tbl(
+            values,
+            headers=header_names,
+            stralign="center",
+            colalign=("center", "center", "center", "left"),
+        )
 
     print(table)
 
     return None
 
 
 def _verify_input_args(
@@ -208,49 +232,47 @@
     if not isinstance(tabulate, (bool, type(None))):
         raise TypeError(
             f"'tabulate' argument must be of bool type! Got {type(tabulate)}."
         )
 
 
 def _get_functions_from_dimension(
-    available_classes: Dict[str, UQTestFunABC],
+    available_classes: dict,
     spatial_dimension: Union[int, str],
 ) -> List[str]:
     """Get the function keys that satisfy the spatial dimension filter."""
     values = []
 
     # --- Make sure to check against a lower-case string
     if isinstance(spatial_dimension, str):
         spatial_dimension = spatial_dimension.lower()
 
     for (
         available_class_name,
         available_class_path,
     ) in available_classes.items():
         default_spatial_dimension = (
-            available_class_path.DEFAULT_SPATIAL_DIMENSION
+            available_class_path.default_spatial_dimension
         )
         if not default_spatial_dimension:
             default_spatial_dimension = "m"
 
         if default_spatial_dimension == spatial_dimension:
             values.append(available_class_name)
 
     return values
 
 
-def _get_functions_from_tag(
-    available_classes: Dict[str, UQTestFunABC], tag: str
-) -> List[str]:
+def _get_functions_from_tag(available_classes: dict, tag: str) -> List[str]:
     """Get the function keys that satisfy the tag filter."""
     values = []
 
     for (
         available_class_name,
         available_class_path,
     ) in available_classes.items():
-        tags = available_class_path.TAGS
+        tags = available_class_path.tags
 
         if tag in tags:
             values.append(available_class_name)
 
     return values
```

### Comparing `uqtestfuns-0.1.1/src/uqtestfuns/meta/basis_functions.py` & `uqtestfuns-0.2.0/src/uqtestfuns/meta/basis_functions.py`

 * *Files identical despite different names*

### Comparing `uqtestfuns-0.1.1/src/uqtestfuns/meta/metaspec.py` & `uqtestfuns-0.2.0/src/uqtestfuns/meta/metaspec.py`

 * *Files identical despite different names*

### Comparing `uqtestfuns-0.1.1/src/uqtestfuns/meta/uqmetatestfun.py` & `uqtestfuns-0.2.0/src/uqtestfuns/meta/uqmetatestfun.py`

 * *Files identical despite different names*

### Comparing `uqtestfuns-0.1.1/src/uqtestfuns/test_functions/__init__.py` & `uqtestfuns-0.2.0/src/uqtestfuns/test_functions/__init__.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,31 +1,55 @@
 """
 The init for the 'test_functions' subpackage of UQTestFuns.
 """
 from .ackley import Ackley
 from .borehole import Borehole
+from .bratley1992 import Bratley1992a, Bratley1992b, Bratley1992c, Bratley1992d
 from .damped_oscillator import DampedOscillator
 from .flood import Flood
+from .forrester import Forrester2008
+from .franke import Franke1, Franke2, Franke3, Franke4, Franke5, Franke6
+from .gramacy2007 import Gramacy1DSine
 from .ishigami import Ishigami
-from .oakley_ohagan_1d import OakleyOHagan1D
+from .oakley2002 import Oakley1D
 from .otl_circuit import OTLCircuit
+from .mclain import McLainS1, McLainS2, McLainS3, McLainS4, McLainS5
 from .piston import Piston
 from .sobol_g import SobolG
 from .sulfur import Sulfur
+from .welch1992 import Welch1992
 from .wing_weight import WingWeight
 
 # NOTE: Import the new test function implementation class from its respective
 # module manually here and update the list below.
 
 __all__ = [
     "Ackley",
     "Borehole",
+    "Bratley1992a",
+    "Bratley1992b",
+    "Bratley1992c",
+    "Bratley1992d",
     "DampedOscillator",
     "Flood",
+    "Forrester2008",
+    "Franke1",
+    "Franke2",
+    "Franke3",
+    "Franke4",
+    "Franke5",
+    "Franke6",
+    "Gramacy1DSine",
     "Ishigami",
-    "OakleyOHagan1D",
+    "Oakley1D",
     "OTLCircuit",
+    "McLainS1",
+    "McLainS2",
+    "McLainS3",
+    "McLainS4",
+    "McLainS5",
     "Piston",
     "SobolG",
     "Sulfur",
+    "Welch1992",
     "WingWeight",
 ]
```

### Comparing `uqtestfuns-0.1.1/src/uqtestfuns/test_functions/borehole.py` & `uqtestfuns-0.2.0/src/uqtestfuns/test_functions/borehole.py`

 * *Files 8% similar despite different names*

```diff
@@ -19,166 +19,147 @@
 2. Max D. Morris, T. J. Mitchell, and D. Ylvisaker, “Bayesian design and
    analysis of computer experiments: Use of derivatives in surface
    prediction,” Technometrics, vol. 35, no. 3, pp. 243–255, 1993.
    DOI: 10.1080/00401706.1993.10485320
 """
 import numpy as np
 
-from typing import Optional
-
-from ..core.prob_input.univariate_distribution import UnivDist
 from ..core.uqtestfun_abc import UQTestFunABC
-from .available import create_prob_input_from_available
+from ..core.prob_input.input_spec import UnivDistSpec, ProbInputSpecFixDim
 
 __all__ = ["Borehole"]
 
 # From Ref. [1]
 INPUT_MARGINALS_HARPER1983 = [
-    UnivDist(
+    UnivDistSpec(
         name="rw",
         distribution="normal",
         parameters=[0.10, 0.0161812],
         description="radius of the borehole [m]",
     ),
-    UnivDist(
+    UnivDistSpec(
         name="r",
         distribution="lognormal",
         parameters=[7.71, 1.0056],
         description="radius of influence [m]",
     ),
-    UnivDist(
+    UnivDistSpec(
         name="Tu",
         distribution="uniform",
         parameters=[63070.0, 115600.0],
         description="transmissivity of upper aquifer [m^2/year]",
     ),
-    UnivDist(
+    UnivDistSpec(
         name="Hu",
         distribution="uniform",
         parameters=[990.0, 1100.0],
         description="potentiometric head of upper aquifer [m]",
     ),
-    UnivDist(
+    UnivDistSpec(
         name="Tl",
         distribution="uniform",
         parameters=[63.1, 116.0],
         description="transmissivity of lower aquifer [m^2/year]",
     ),
-    UnivDist(
+    UnivDistSpec(
         name="Hl",
         distribution="uniform",
         parameters=[700.0, 820.0],
         description="potentiometric head of lower aquifer [m]",
     ),
-    UnivDist(
+    UnivDistSpec(
         name="L",
         distribution="uniform",
         parameters=[1120.0, 1680.0],
         description="length of the borehole [m]",
     ),
-    UnivDist(
+    UnivDistSpec(
         name="Kw",
         distribution="uniform",
         parameters=[9985.0, 12045.0],
         description="hydraulic conductivity of the borehole [m/year]",
     ),
 ]
 
 # From Ref. [2]
 INPUT_MARGINALS_MORRIS1993 = list(INPUT_MARGINALS_HARPER1983)
 INPUT_MARGINALS_MORRIS1993[0:2] = [
-    UnivDist(
+    UnivDistSpec(
         name="rw",
         distribution="uniform",
         parameters=[0.05, 0.15],
         description="radius of the borehole [m]",
     ),
-    UnivDist(
+    UnivDistSpec(
         name="r",
         distribution="uniform",
         parameters=[100, 50000],
         description="radius of influence [m]",
     ),
 ]
 
 AVAILABLE_INPUT_SPECS = {
-    "Harper1983": {
-        "name": "Borehole-Harper-1983",
-        "description": (
+    "Harper1983": ProbInputSpecFixDim(
+        name="Borehole-Harper-1983",
+        description=(
             "Probabilistic input model of the Borehole model "
             "from Harper and Gupta (1983)."
         ),
-        "marginals": INPUT_MARGINALS_HARPER1983,
-        "copulas": None,
-    },
-    "Morris1993": {
-        "name": "Borehole-Morris-1993",
-        "description": (
+        marginals=INPUT_MARGINALS_HARPER1983,
+        copulas=None,
+    ),
+    "Morris1993": ProbInputSpecFixDim(
+        name="Borehole-Morris-1993",
+        description=(
             "Probabilistic input model of the Borehole model "
             "from Morris et al. (1993)."
         ),
-        "marginals": INPUT_MARGINALS_MORRIS1993,
-        "copulas": None,
-    },
+        marginals=INPUT_MARGINALS_MORRIS1993,
+        copulas=None,
+    ),
 }
 
 DEFAULT_INPUT_SELECTION = "Harper1983"
 
 
-class Borehole(UQTestFunABC):
-    """A concrete implementation of the Borehole function."""
+def evaluate(xx: np.ndarray) -> np.ndarray:
+    """Evaluate the Borehole function on a set of input values.
 
-    _TAGS = ["metamodeling", "sensitivity"]
+    Parameters
+    ----------
+    xx : np.ndarray
+        8-Dimensional input values given by N-by-8 arrays where
+        N is the number of input values.
+
+    Returns
+    -------
+    np.ndarray
+        The output of the Borehole function evaluated on the input values.
+        The output is a 1-dimensional array of length N.
+    """
+    # Compute the Borehole function
+    nom = 2 * np.pi * xx[:, 2] * (xx[:, 3] - xx[:, 5])
+    denom_1 = np.log(xx[:, 1] / xx[:, 0])
+    denom_2 = (
+        2
+        * xx[:, 6]
+        * xx[:, 2]
+        / (np.log(xx[:, 1] / xx[:, 0]) * xx[:, 0] ** 2 * xx[:, 7])
+    )
+    denom_3 = xx[:, 2] / xx[:, 4]
 
-    _AVAILABLE_INPUTS = tuple(AVAILABLE_INPUT_SPECS.keys())
+    yy = nom / (denom_1 * (1 + denom_2 + denom_3))
 
-    _AVAILABLE_PARAMETERS = None
+    return yy
 
-    _DEFAULT_SPATIAL_DIMENSION = 8
 
-    _DESCRIPTION = "Borehole function from Harper and Gupta (1983)"
-
-    def __init__(
-        self,
-        *,
-        prob_input_selection: Optional[str] = DEFAULT_INPUT_SELECTION,
-        name: Optional[str] = None,
-    ):
-        # --- Arguments processing
-        prob_input = create_prob_input_from_available(
-            prob_input_selection, AVAILABLE_INPUT_SPECS
-        )
-        # Process the default name
-        if name is None:
-            name = Borehole.__name__
-
-        super().__init__(prob_input=prob_input, name=name)
-
-    def evaluate(self, xx):
-        """Evaluate the Borehole function on a set of input values.
-
-        Parameters
-        ----------
-        xx : np.ndarray
-            8-Dimensional input values given by N-by-8 arrays where
-            N is the number of input values.
-
-        Returns
-        -------
-        np.ndarray
-            The output of the Borehole function evaluated on the input values.
-            The output is a 1-dimensional array of length N.
-        """
-        # Compute the Borehole function
-        nom = 2 * np.pi * xx[:, 2] * (xx[:, 3] - xx[:, 5])
-        denom_1 = np.log(xx[:, 1] / xx[:, 0])
-        denom_2 = (
-            2
-            * xx[:, 6]
-            * xx[:, 2]
-            / (np.log(xx[:, 1] / xx[:, 0]) * xx[:, 0] ** 2 * xx[:, 7])
-        )
-        denom_3 = xx[:, 2] / xx[:, 4]
+class Borehole(UQTestFunABC):
+    """A concrete implementation of the Borehole function."""
 
-        yy = nom / (denom_1 * (1 + denom_2 + denom_3))
+    _tags = ["metamodeling", "sensitivity"]
+    _description = "Borehole function from Harper and Gupta (1983)"
+    _available_inputs = AVAILABLE_INPUT_SPECS
+    _available_parameters = None
+    _default_input = DEFAULT_INPUT_SELECTION
+    _default_spatial_dimension = 8
 
-        return yy
+    eval_ = staticmethod(evaluate)
```

### Comparing `uqtestfuns-0.1.1/src/uqtestfuns/test_functions/damped_oscillator.py` & `uqtestfuns-0.2.0/src/uqtestfuns/test_functions/sulfur.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,228 +1,205 @@
 """
-Module with an implementation of the damped oscillator model.
+Module with an implementation of the Sulfur model test function.
 
-The damped oscillator model is a seven-dimensional scalar-valued function
-that computes the relative displacement of a secondary spring
-under a white noise base acceleration.
-The model was first proposed in [1] and used in the context of reliability
-analysis in [2] and [3]. Note, however, that the reliability analysis
-variant differs from this base model.
-Used in the context of reliability analysis,
-the model also includes additional parameters related to a capacity factor and
-load such that the performance function can be computed.
-
-The damped oscillator model is based on a two-degree-of-freedom
-primary-secondary mechanical system characterized by two masses, two springs,
-and the corresponding damping ratios.
+The Sulfur model from [1] is a nine-dimensional scalar-valued function
+that analytically computes the direct radiative forcing by sulfate aerosols.
+The test function was used in [2] for metamodeling and uncertainty propagation
+purposes.
+The probabilistic input specification used in [2] was originally based
+from [3].
+
+Due to the construction of the test function, the geometric mean and geometric
+standard deviation of the response are analytically available given the input
+specification (from [2], all are lognormals). Note that the geometric mean
+and the geometric standard deviation of a lognormal distribution are
+the exponentiated mu and sigma parameters (i.e., the mean and
+standard deviation of the underlying normal distribution).
+
+To complete the test function specification, two additional parameters are
+taken from the literature: the solar constant [4] and the surface area
+of the earth [5].
+
+Notes
+-----
+
+- The equation of the Sulfur model in [2] (Eq. (12)) is erroneous.
+  The solar constant term S0 should not be squared otherwise the dimension
+  will not agree. Moreover, the equation is missing factors of 365 in the
+  denominator and 10^12 in the numerator because the parameter L
+  (Sulfate lifetime in the atmosphere) is given in [days]
+  while the parameter Q (Global input flux of anthropogenic sulfur is
+  given in [TgS/year].
+- The input specification of the model here is taken from [3] (Table 2).
+  While they are similar, the parameters T and (1-Rs) in [3] are in the
+  squared form (i.e., T^2 and (1-Rs)^2).
 
 References
 ----------
-1. Takeru Igusa and Armen Der Kiureghian, “Dynamic characterization of
-   two‐degree‐of‐freedom equipment‐structure systems,”
-   Journal of Engineering Mechanics, vol. 111, no. 1, pp. 1–19, 1985.
-   DOI: 10.1061/(ASCE)0733-9399(1985)111:1(1)
-2. Armen Der Kiureghian and Mario De Stefano, “Efficient algorithm for
-   second‐order reliability analysis,” Journal of Engineering Mechanics,
-   vol. 117, no. 12, pp. 2904–2923, 1991.
-   DOI: 10.1061/(ASCE)0733-9399(1991)117:12(2904)
-3. Vincent Dubourg, “Adaptive surrogate models for reliability analysis
-   and reliability-based design optimization,”
-   Université Blaise Pascal - Clermont II, Clermont-Ferrand, France, 2011.
-   URL: https://sites.google.com/site/vincentdubourg/phd-thesis
+1. R. J. Charlson, S. E. Schwartz, J. M. Hales, R. D. Cess, J. A. Coakley,
+   J. E. Hansen, and D. J. Hofmann, “Climate forcing by anthropogenic
+   aerosols,” Science, vol. 255, no. 5043, pp. 423–430, 1992.
+   DOI: 10.1126/science.255.5043.423.
+2. M. A. Tatang, W. Pan, R. G. Prinn, and G. J. McRae, “An efficient method
+   for parametric uncertainty analysis of numerical geophysical models,”
+   Journal of Geophysical Research, vol. 102, no. D18, pp. 21925–21932, 1997.
+   DOI: 10.1029/97JD01654.
+3. J. E. Penner, R. J. Charlson, S.E. Schwartz, J. M. Hales, N. S. Laulainen,
+   L. Travis, R. Leifer, T. Novakov, J. Ogren, L. F. Radke, “Quantifying and
+   Minimizing Uncertainty of Climate Forcing by Anthropogenic Aerosols,”
+   Bulletin of the American Meteorological Society, vol. 75, no. 3,
+   pp. 375–400, 1994.
+   DOI: 10.1175/1520-0477(1994)075<0375:QAMUOC>2.0.CO;2.
+4. G. Kopp and J. L. Lean, “A new, lower value of total solar irradiance:
+   Evidence and climate significance,” Geophysical Research Letter, vol. 38,
+   no. 1, 2011.
+   DOI: 10.1029/2010GL045777.
+5. M. Pidwirny, “Introduction to the Oceans,”
+   Fundamentals of Physical Geography, 2nd Edition, 2006.
+   Accessed: Jan. 25, 2023
+   URL: http://www.physicalgeography.net/fundamentals/8o.html.
 """
 import numpy as np
 
-from typing import Optional
-
-from ..core.prob_input.univariate_distribution import UnivDist
+from ..core.prob_input.input_spec import UnivDistSpec, ProbInputSpecFixDim
 from ..core.uqtestfun_abc import UQTestFunABC
-from .utils import lognorm2norm_mean, lognorm2norm_std
-from .available import create_prob_input_from_available
 
-__all__ = ["DampedOscillator"]
+__all__ = ["Sulfur"]
 
-INPUT_MARGINALS_DERKIUREGHIAN1991 = [  # From [2]
-    UnivDist(
-        name="Mp",
-        distribution="lognormal",
-        parameters=[
-            lognorm2norm_mean(1.5, 0.1 * 1.5),
-            lognorm2norm_std(1.5, 0.1 * 1.5),
-        ],
-        description="Primary mass",
-    ),
-    UnivDist(
-        name="Ms",
-        distribution="lognormal",
-        parameters=[
-            lognorm2norm_mean(0.01, 0.1 * 0.01),
-            lognorm2norm_std(0.01, 0.1 * 0.01),
-        ],
-        description="Secondary mass",
-    ),
-    UnivDist(
-        name="Kp",
-        distribution="lognormal",
-        parameters=[
-            lognorm2norm_mean(1.0, 0.2 * 1.0),
-            lognorm2norm_std(1.0, 0.2 * 1.0),
-        ],
-        description="Primary spring stiffness",
-    ),
-    UnivDist(
-        name="Ks",
-        distribution="lognormal",
-        parameters=[
-            lognorm2norm_mean(0.01, 0.2 * 0.01),
-            lognorm2norm_std(0.01, 0.2 * 0.01),
-        ],
-        description="Secondary spring stiffness",
-    ),
-    UnivDist(
-        name="Zeta_p",
-        distribution="lognormal",
-        parameters=[
-            lognorm2norm_mean(0.05, 0.4 * 0.05),
-            lognorm2norm_std(0.05, 0.4 * 0.05),
-        ],
-        description="Primary damping ratio",
-    ),
-    UnivDist(
-        name="Zeta_s",
-        distribution="lognormal",
-        parameters=[
-            lognorm2norm_mean(0.02, 0.5 * 0.02),
-            lognorm2norm_std(0.02, 0.5 * 0.02),
-        ],
-        description="Secondary damping ratio",
-    ),
-    UnivDist(
-        name="S0",
-        distribution="lognormal",
-        parameters=[
-            lognorm2norm_mean(100.0, 0.1 * 100.0),
-            lognorm2norm_std(100.0, 0.1 * 100.0),
-        ],
-        description="White noise base acceleration",
+INPUT_MARGINALS_PENNER1994 = [  # From [3] (Table 2)
+    UnivDistSpec(
+        name="Q",
+        distribution="lognormal",
+        parameters=[np.log(71.0), np.log(1.15)],
+        description="Source strength of anthropogenic Sulfur [10^12 g/year]",
+    ),
+    UnivDistSpec(
+        name="Y",
+        distribution="lognormal",
+        parameters=[np.log(0.5), np.log(1.5)],
+        description="Fraction of SO2 oxidized to SO4(2-) aerosol [-]",
+    ),
+    UnivDistSpec(
+        name="L",
+        distribution="lognormal",
+        parameters=[np.log(5.5), np.log(1.5)],
+        description="Average lifetime of atmospheric SO4(2-) [days]",
+    ),
+    UnivDistSpec(
+        name="Psi_e",
+        distribution="lognormal",
+        parameters=[np.log(5.0), np.log(1.4)],
+        description="Aerosol mass scattering efficiency [m^2/g]",
+    ),
+    UnivDistSpec(
+        name="beta",
+        distribution="lognormal",
+        parameters=[np.log(0.3), np.log(1.3)],
+        description="Fraction of light scattered upward hemisphere [-]",
+    ),
+    UnivDistSpec(
+        name="f_Psi_e",
+        distribution="lognormal",
+        parameters=[np.log(1.7), np.log(1.2)],
+        description="Fractional increase in aerosol scattering efficiency "
+        "due to hygroscopic growth [-]",
+    ),
+    UnivDistSpec(
+        name="T^2",
+        distribution="lognormal",
+        parameters=[np.log(0.58), np.log(1.4)],
+        description="Square of atmospheric "
+        "transmittance above aerosol layer [-]",
+    ),
+    UnivDistSpec(
+        name="(1-Ac)",
+        distribution="lognormal",
+        parameters=[np.log(0.39), np.log(1.1)],
+        description="Fraction of earth not covered by cloud [-]",
+    ),
+    UnivDistSpec(
+        name="(1-Rs)^2",
+        distribution="lognormal",
+        parameters=[np.log(0.72), np.log(1.2)],
+        description="Square of surface coalbedo [-]",
     ),
 ]
 
 AVAILABLE_INPUT_SPECS = {
-    "DerKiureghian1991": {
-        "name": "Damped-Oscillator-Der-Kiureghian-1991",
-        "description": (
-            "Probabilistic input model for the Damped Oscillator model "
-            "from Der Kiureghian and De Stefano (1991)."
+    "Penner1994": ProbInputSpecFixDim(
+        name="Sulfur-Penner1994",
+        description=(
+            "Probabilistic input model for the Sulfur model "
+            "from Penner et al. (1994)."
         ),
-        "marginals": INPUT_MARGINALS_DERKIUREGHIAN1991,
-        "copulas": None,
-    },
+        marginals=INPUT_MARGINALS_PENNER1994,
+        copulas=None,
+    ),
 }
 
-DEFAULT_INPUT_SELECTION = "DerKiureghian1991"
-
-
-class DampedOscillator(UQTestFunABC):
-    """A concrete implementation of the Damped oscillator test function."""
-
-    _TAGS = ["metamodeling", "sensitivity"]
-
-    _AVAILABLE_INPUTS = tuple(AVAILABLE_INPUT_SPECS.keys())
-
-    _AVAILABLE_PARAMETERS = None
-
-    _DEFAULT_SPATIAL_DIMENSION = 8
+DEFAULT_INPUT_SELECTION = "Penner1994"
 
-    _DESCRIPTION = (
-        "Damped oscillator model from Igusa and Der Kiureghian (1985)"
-    )
+SOLAR_CONSTANT = 1361  # [W/m^2] from [4]
+EARTH_AREA = 5.1e14  # [m^2] from [5]
+DAYS_IN_YEAR = 365  # [days]
 
-    def __init__(
-        self,
-        *,
-        prob_input_selection: Optional[str] = DEFAULT_INPUT_SELECTION,
-        name: Optional[str] = None,
-    ):
-        # --- Arguments processing
-        prob_input = create_prob_input_from_available(
-            prob_input_selection, AVAILABLE_INPUT_SPECS
-        )
-        # Process the default name
-        if name is None:
-            name = DampedOscillator.__name__
 
-        super().__init__(prob_input=prob_input, name=name)
+def evaluate(xx: np.ndarray) -> np.ndarray:
+    """Evaluate the Sulfur model test function on a set of input values.
 
-    def evaluate(self, xx: np.ndarray):
-        """Evaluate the damped oscillator model on a set of input values.
-
-        Parameters
-        ----------
-        xx : np.ndarray
-            A 7-dimensional input values given by an N-by-7 array
-            where N is the number of input values.
-
-        Returns
-        -------
-        np.ndarray
-            The output of the damped oscillator model test function, i.e.,
-            the relative displacement of the secondary spring.
-        """
-        yy = evaluate_mean_square_displacement(xx)
-
-        return np.sqrt(yy)
-
-
-def evaluate_mean_square_displacement(xx: np.ndarray):
-    """Evaluate the mean-square displacement of the damped oscillator model.
-
-    Parameters
+    References
     ----------
     xx : np.ndarray
-        A 7-dimensional input values given by an N-by-7 array
+        A nine-dimensional input values given by an N-by-9 array
         where N is the number of input values.
 
     Returns
     -------
     np.ndarray
-        The mean-square relative displacement of the secondary spring.
+        The output of the Sulfur model test function, i.e.,
+        the direct radiative forcing by sulfate aerosols.
     """
+    # Source strength of anthropogenic Sulfur (initially given in Teragram)
+    qq = xx[:, 0] * 1e12
+    # Fraction of SO2 oxidized to SO4(2-) aerosol
+    yy = xx[:, 1]
+    # Average lifetime of atmospheric SO4(2-)
+    ll = xx[:, 2]
+    # Aerosol mass scattering efficiency
+    psi_e = xx[:, 3]
+    # Fraction of light scattered upward hemisphere
+    beta = xx[:, 4]
+    # Fractional increase in aerosol scattering eff. due hygroscopic growth
+    ff_psi = xx[:, 5]
+    # Square of atmospheric transmittance above aerosol layer
+    tt_sq = xx[:, 6]
+    # Fraction of earth not covered by cloud
+    aa_c_complement = xx[:, 7]
+    # Square of surface coalbedo
+    co_rr_s_sq = xx[:, 8]
+
+    # Sulfate burden (Eq. (5) in [1], notation from [2])
+    # NOTE: Factor 3.0 due to conversion of mass from S to SO4(2-)
+    # NOTE: Factor 1/365.0 due to average lifetime is given in [days]
+    #       while qq is in [gS / year]
+    sulfate_burden = 3.0 * qq * yy * ll / EARTH_AREA / DAYS_IN_YEAR
+
+    # Loading of sulfate aerosol (Eq. (4) in [1], notation from [2])
+    sulfate_loading = psi_e * ff_psi * sulfate_burden
+
+    # Direct radiative forcing by sulfate aerosols
+    factor_1 = SOLAR_CONSTANT * aa_c_complement * tt_sq * co_rr_s_sq * beta
+    dd_f = -0.5 * factor_1 * sulfate_loading
+
+    return dd_f
+
+
+class Sulfur(UQTestFunABC):
+    """A concrete implementation of the Sulfur model test function."""
+
+    _tags = ["metamodeling", "sensitivity"]
+    _description = "Sulfur model from Charlson et al. (1992)"
+    _available_inputs = AVAILABLE_INPUT_SPECS
+    _available_parameters = None
+    _default_spatial_dimension = 9
 
-    # Get the parameters
-    mm_p = xx[:, 0]  # Primary mass
-    mm_s = xx[:, 1]  # Secondary mass
-    kk_p = xx[:, 2]  # Primary spring stiffness
-    kk_s = xx[:, 3]  # Secondary spring stiffness
-    zt_p = xx[:, 4]  # Damping ratio of the primary damper
-    zt_s = xx[:, 5]  # Damping ratio of the secondary damper
-    ss_0 = xx[:, 6]  # White noise base acceleration intensity
-
-    # Compute natural frequencies
-    omega_p = np.sqrt(kk_p / mm_p)  # Primary system
-    omega_s = np.sqrt(kk_s / mm_s)  # Secondary system
-
-    # Compute additional parameters
-    gamma = mm_s / mm_p  # relative mass
-    omega_a = (omega_p + omega_s) / 2.0  # average natural frequency
-    zt_a = (zt_p + zt_s) / 2.0  # average damping ratio
-    theta = (omega_p - omega_s) / omega_a  # tuning parameter
-
-    # Compute the mean-square relative displacement of the secondary spring
-    first_term = np.pi * ss_0 / 4 / zt_s / (omega_s**3)
-    second_term = (
-        zt_a
-        * zt_s
-        / (zt_p * zt_s * (4 * zt_a**2 + theta**2) + gamma * zt_a**2)
-    )
-    third_term = (
-        (zt_p * omega_p**3 + zt_s * omega_s**3)
-        * omega_p
-        / 4
-        / zt_a
-        / (omega_a**4)
-    )
-
-    # NOTE: This is squared displacement
-    xx_s = first_term * second_term * third_term
-
-    return xx_s
+    eval_ = staticmethod(evaluate)
```

### Comparing `uqtestfuns-0.1.1/src/uqtestfuns/test_functions/flood.py` & `uqtestfuns-0.2.0/src/uqtestfuns/test_functions/flood.py`

 * *Files 22% similar despite different names*

```diff
@@ -28,144 +28,122 @@
    in Handbook of Uncertainty Quantification, R. Ghanem, D. Higdon,
    and H. Owhadi, Eds. Cham: Springer International Publishing, 2017,
    pp. 2001–2038.
    DOI: 10.1007/978-3-319-12385-1_64
 """
 import numpy as np
 
-from typing import Optional
-
-from ..core.prob_input.univariate_distribution import UnivDist
+from ..core.prob_input.input_spec import UnivDistSpec, ProbInputSpecFixDim
 from ..core.uqtestfun_abc import UQTestFunABC
-from .available import create_prob_input_from_available
 
 __all__ = ["Flood"]
 
 INPUT_MARGINALS_IOOSS2015 = [  # From Ref. [1]
-    UnivDist(
+    UnivDistSpec(
         name="Q",
         distribution="trunc-gumbel",
         parameters=[1013.0, 558.0, 500.0, 3000.0],
         description="Maximum annual flow rate [m^3/s]",
     ),
-    UnivDist(
+    UnivDistSpec(
         name="Ks",
         distribution="trunc-normal",
         parameters=[30.0, 8.0, 15.0, np.inf],
         description="Strickler coefficient [m^(1/3)/s]",
     ),
-    UnivDist(
+    UnivDistSpec(
         name="Zv",
         distribution="triangular",
         parameters=[49.0, 51.0, 50.0],
         description="River downstream level [m]",
     ),
-    UnivDist(
+    UnivDistSpec(
         name="Zm",
         distribution="triangular",
         parameters=[54.0, 56.0, 55.0],
         description="River upstream level [m]",
     ),
-    UnivDist(
+    UnivDistSpec(
         name="Hd",
         distribution="uniform",
         parameters=[7.0, 9.0],
         description="Dyke height [m]",
     ),
-    UnivDist(
+    UnivDistSpec(
         name="Cb",
         distribution="triangular",
         parameters=[55.0, 56.0, 55.5],
         description="Bank level [m]",
     ),
-    UnivDist(
+    UnivDistSpec(
         name="L",
         distribution="triangular",
         parameters=[4990.0, 5010.0, 5000.0],
         description="Length of the river stretch [m]",
     ),
-    UnivDist(
+    UnivDistSpec(
         name="B",
         distribution="triangular",
         parameters=[295.0, 305.0, 300.0],
         description="River width [m]",
     ),
 ]
 
 AVAILABLE_INPUT_SPECS = {
-    "Iooss2015": {
-        "name": "Flood-Iooss-2015",
-        "description": (
+    "Iooss2015": ProbInputSpecFixDim(
+        name="Flood-Iooss2015",
+        description=(
             "Probabilistic input model for the Flood model "
             "from Iooss and Lemaître (2015)."
         ),
-        "marginals": INPUT_MARGINALS_IOOSS2015,
-        "copulas": None,
-    }
+        marginals=INPUT_MARGINALS_IOOSS2015,
+        copulas=None,
+    ),
 }
 
-DEFAULT_INPUT_SELECTION = "Iooss2015"
 
+def evaluate(xx: np.ndarray) -> np.ndarray:
+    """Evaluate the flood model test function on a set of input values.
 
-class Flood(UQTestFunABC):
-    """Concrete implementation of the Flood model test function."""
+    Parameters
+    ----------
+    xx : np.ndarray
+        A six-dimensional input values given by an N-by-8 array
+        where N is the number of input values.
+
+    Returns
+    -------
+    np.ndarray
+        The output of the flood model test function, i.e.,
+        the height of a river.
+        The output is a one-dimensional array of length N.
+    """
+    qq = xx[:, 0]  # Maximum annual flow rate
+    kk_s = xx[:, 1]  # Strickler coefficient
+    zz_v = xx[:, 2]  # River downstream level
+    zz_m = xx[:, 3]  # River upstream level
+    hh_d = xx[:, 4]  # Dyke height
+    cc_b = xx[:, 5]  # Bank level
+    ll = xx[:, 6]  # Length of the river stretch
+    bb = xx[:, 7]  # River width
+
+    # Compute the maximum annual height of the river [m]
+    hh_w = (qq / (bb * kk_s * np.sqrt((zz_m - zz_v) / ll))) ** 0.6
+
+    # Compute the maximum annual underflow [m]
+    # NOTE: The sign compared to [1] has been inverted below, a negative
+    # value indicates an overflow
+    ss = cc_b + hh_d - zz_v - hh_w
 
-    _TAGS = ["metamodeling", "sensitivity"]
+    return ss
 
-    _AVAILABLE_INPUTS = tuple(AVAILABLE_INPUT_SPECS.keys())
 
-    _AVAILABLE_PARAMETERS = None
-
-    _DEFAULT_SPATIAL_DIMENSION = 8
+class Flood(UQTestFunABC):
+    """Concrete implementation of the Flood model test function."""
 
-    _DESCRIPTION = "Flood model from Iooss and Lemaître (2015)"
-
-    def __init__(
-        self,
-        *,
-        prob_input_selection: Optional[str] = DEFAULT_INPUT_SELECTION,
-        name: Optional[str] = None,
-    ):
-        # --- Arguments processing
-        prob_input = create_prob_input_from_available(
-            prob_input_selection, AVAILABLE_INPUT_SPECS
-        )
-        # Process the default name
-        if name is None:
-            name = Flood.__name__
-
-        super().__init__(prob_input=prob_input, name=name)
-
-    def evaluate(self, xx):
-        """Evaluate the flood model test function on a set of input values.
-
-        Parameters
-        ----------
-        xx : np.ndarray
-            A six-dimensional input values given by an N-by-8 array
-            where N is the number of input values.
-
-        Returns
-        -------
-        np.ndarray
-            The output of the flood model test function, i.e.,
-            the height of a river.
-            The output is a one-dimensional array of length N.
-        """
-        qq = xx[:, 0]  # Maximum annual flow rate
-        kk_s = xx[:, 1]  # Strickler coefficient
-        zz_v = xx[:, 2]  # River downstream level
-        zz_m = xx[:, 3]  # River upstream level
-        hh_d = xx[:, 4]  # Dyke height
-        cc_b = xx[:, 5]  # Bank level
-        ll = xx[:, 6]  # Length of the river stretch
-        bb = xx[:, 7]  # River width
-
-        # Compute the maximum annual height of the river [m]
-        hh_w = (qq / (bb * kk_s * np.sqrt((zz_m - zz_v) / ll))) ** 0.6
-
-        # Compute the maximum annual underflow [m]
-        # NOTE: The sign compared to [1] has been inverted below, a negative
-        # value indicates an overflow
-        ss = cc_b + hh_d - zz_v - hh_w
+    _tags = ["metamodeling", "sensitivity"]
+    _description = "Flood model from Iooss and Lemaître (2015)"
+    _available_inputs = AVAILABLE_INPUT_SPECS
+    _available_parameters = None
+    _default_spatial_dimension = 8
 
-        return ss
+    eval_ = staticmethod(evaluate)
```

### Comparing `uqtestfuns-0.1.1/src/uqtestfuns/test_functions/ishigami.py` & `uqtestfuns-0.2.0/src/uqtestfuns/test_functions/ishigami.py`

 * *Files 25% similar despite different names*

```diff
@@ -25,124 +25,94 @@
    Sobol indices for the Gaussian process metamodel,”
    Reliability Engineering & System Safety,
    vol. 94, no. 3, pp. 742–751, 2009.
    DOI:10.1016/j.ress.2008.07.008
 """
 import numpy as np
 
-from typing import Optional
+from typing import Tuple
 
-from ..core.prob_input.univariate_distribution import UnivDist
+from ..core.prob_input.input_spec import UnivDistSpec, ProbInputSpecFixDim
 from ..core.uqtestfun_abc import UQTestFunABC
-from .available import (
-    create_prob_input_from_available,
-    create_parameters_from_available,
-)
 
 __all__ = ["Ishigami"]
 
 
 INPUT_MARGINALS_ISHIGAMI1991 = [
-    UnivDist(
+    UnivDistSpec(
         name="X1",
         distribution="uniform",
         parameters=[-np.pi, np.pi],
         description="None",
     ),
-    UnivDist(
+    UnivDistSpec(
         name="X2",
         distribution="uniform",
         parameters=[-np.pi, np.pi],
         description="None",
     ),
-    UnivDist(
+    UnivDistSpec(
         name="X3",
         distribution="uniform",
         parameters=[-np.pi, np.pi],
         description="None",
     ),
 ]
 
 AVAILABLE_INPUT_SPECS = {
-    "Ishigami1991": {
-        "name": "Ishigami-1991",
-        "description": (
+    "Ishigami1991": ProbInputSpecFixDim(
+        name="Ishigami1991",
+        description=(
             "Probabilistic input model for the Ishigami function "
             "from Ishigami and Homma (1991)."
         ),
-        "marginals": INPUT_MARGINALS_ISHIGAMI1991,
-        "copulas": None,
-    }
+        marginals=INPUT_MARGINALS_ISHIGAMI1991,
+        copulas=None,
+    ),
 }
 
-DEFAULT_INPUT_SELECTION = "Ishigami1991"
-
 AVAILABLE_PARAMETERS = {
     "Ishigami1991": (7, 0.05),  # from [1]
     "Sobol1999": (7, 0.1),  # from [2]
 }
 
 DEFAULT_PARAMETERS_SELECTION = "Ishigami1991"
 
 
-class Ishigami(UQTestFunABC):
-    """A concrete implementation of the Ishigami function."""
+def evaluate(xx: np.ndarray, parameters: Tuple[float, float]):
+    """Evaluate the Ishigami function on a set of input values.
 
-    _TAGS = ["sensitivity"]
+    Parameters
+    ----------
+    xx : np.ndarray
+        3-Dimensional input values given by N-by-3 arrays where
+        N is the number of input values.
+    parameters : Tuple[float, float]
+        Tuple of two values as the parameters of the function.
+
+    Returns
+    -------
+    np.ndarray
+        The output of the Ishigami function evaluated on the input values.
+        The output is a 1-dimensional array of length N.
+    """
+    # Compute the Ishigami function
+    term_1 = np.sin(xx[:, 0])
+    term_2 = parameters[0] * np.sin(xx[:, 1]) ** 2
+    term_3 = parameters[1] * xx[:, 2] ** 4 * np.sin(xx[:, 0])
 
-    _AVAILABLE_INPUTS = tuple(AVAILABLE_INPUT_SPECS.keys())
+    yy = term_1 + term_2 + term_3
 
-    _AVAILABLE_PARAMETERS = tuple(AVAILABLE_PARAMETERS.keys())
+    return yy
 
-    _DEFAULT_SPATIAL_DIMENSION = 3
-
-    _DESCRIPTION = "Ishigami function from Ishigami and Homma (1991)"
-
-    def __init__(
-        self,
-        *,
-        prob_input_selection: Optional[str] = DEFAULT_INPUT_SELECTION,
-        parameters_selection: Optional[str] = DEFAULT_PARAMETERS_SELECTION,
-        name: Optional[str] = None,
-    ):
-        # --- Arguments processing
-        prob_input = create_prob_input_from_available(
-            prob_input_selection, AVAILABLE_INPUT_SPECS
-        )
-        # Ishigami supports several different parameterizations
-        parameters = create_parameters_from_available(
-            parameters_selection, AVAILABLE_PARAMETERS
-        )
-        # Process the default name
-        if name is None:
-            name = Ishigami.__name__
-
-        super().__init__(
-            prob_input=prob_input, parameters=parameters, name=name
-        )
-
-    def evaluate(self, xx):
-        """Evaluate the Ishigami function on a set of input values.
-
-        Parameters
-        ----------
-        xx : np.ndarray
-            3-Dimensional input values given by N-by-3 arrays where
-            N is the number of input values.
-        params : tuple
-            Tuple of two values as the parameters of the function.
-
-        Returns
-        -------
-        np.ndarray
-            The output of the Ishigami function evaluated on the input values.
-            The output is a 1-dimensional array of length N.
-        """
-        # Compute the Ishigami function
-        parameters = self.parameters
-        term_1 = np.sin(xx[:, 0])
-        term_2 = parameters[0] * np.sin(xx[:, 1]) ** 2
-        term_3 = parameters[1] * xx[:, 2] ** 4 * np.sin(xx[:, 0])
 
-        yy = term_1 + term_2 + term_3
+class Ishigami(UQTestFunABC):
+    """An implementation of the Ishigami test function."""
+
+    _tags = ["sensitivity"]
+    _description = "Ishigami function from Ishigami and Homma (1991)"
+    _available_inputs = AVAILABLE_INPUT_SPECS
+    _available_parameters = AVAILABLE_PARAMETERS
+    _default_parameters = DEFAULT_PARAMETERS_SELECTION
+    _default_spatial_dimension = 3
 
-        return yy
+    eval_ = staticmethod(evaluate)
```

### Comparing `uqtestfuns-0.1.1/src/uqtestfuns/test_functions/oakley_ohagan_1d.py` & `uqtestfuns-0.2.0/src/uqtestfuns/test_functions/gramacy2007.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,96 +1,104 @@
 """
-Module with an implementation of the 1D Oakley-O'Hagan test function.
+Module with an implementation of the 1D Gramacy (2007) test function.
 
-The 1D Oakley-O'Hagan test function is a one-dimensional scalar-valued
-function. It was used in [1] as a test function for illustrating metamodeling
-and uncertainty propagation approaches.
+The Gramacy (2007) one-dimensional sine function is a scalar-valued function
+that features two regimes: one part is a mixture of sines and cosines and
+another part is a linear function. The function was introduced in [1]
+as a test function for non-stationary Gaussian process metamodeling
+by partitioning the input parameter space.
+
+In its original usage, the response is disturbed by an i.i.d Gaussian noise.
 
 References
 ----------
 
-1. Jeremy Oakley and Anthony O'Hagan, "Bayesian inference for the uncertainty
-   distribution of computer model outputs," Biometrika , Vol. 89, No. 4,
-   p. 769-784, 2002.
-   DOI: 10.1093/biomet/89.4.769
+1. Robert B. Gramacy, “tgp: An R Package for Bayesian nonstationary,
+   semiparametric nonlinear regression and design by Treed Gaussian Process
+   models,” Journal of Statistical Software, vol. 19, no. 9, 2007.
+   DOI: 10.18637/jss.v019.i09.
 """
 import numpy as np
 
+from numpy.random._generator import Generator
 from typing import Optional
 
-from ..core.prob_input.univariate_distribution import UnivDist
+from ..core.prob_input.input_spec import UnivDistSpec, ProbInputSpecFixDim
 from ..core.uqtestfun_abc import UQTestFunABC
-from .available import create_prob_input_from_available
-
-__all__ = ["OakleyOHagan1D"]
 
-INPUT_MARGINALS_OAKLEY2002 = [
-    UnivDist(
-        name="x",
-        distribution="normal",
-        parameters=[0.0, 4.0],
-        description="None",
-    ),
-]
+__all__ = ["Gramacy1DSine"]
 
 AVAILABLE_INPUT_SPECS = {
-    "Oakley2002": {
-        "name": "Oakley-OHagan-2002",
-        "description": (
-            "Probabilistic input model for the one-dimensional function "
-            "from Oakley-O'Hagan function (2002)"
+    "Gramacy2007": ProbInputSpecFixDim(
+        name="Gramacy2007",
+        description=(
+            "Input model for the one-dimensional function "
+            "from Gramacy (2007)"
         ),
-        "marginals": INPUT_MARGINALS_OAKLEY2002,
-    }
+        marginals=[
+            UnivDistSpec(
+                name="x",
+                distribution="uniform",
+                parameters=[0.0, 20.0],
+                description="None",
+            )
+        ],
+        copulas=None,
+    ),
 }
 
-DEFAULT_INPUT_SELECTION = "Oakley2002"
-
-
-class OakleyOHagan1D(UQTestFunABC):
-    """A concrete implementation of the 1D Oakley-O'Hagan test function."""
-
-    _TAGS = ["metamodeling"]
-
-    _AVAILABLE_INPUTS = tuple(AVAILABLE_INPUT_SPECS.keys())
-
-    _AVAILABLE_PARAMETERS = None
-
-    _DEFAULT_SPATIAL_DIMENSION = 1
-
-    _DESCRIPTION = "One-dimensional function from Oakley and O'Hagan (2002)"
-
-    def __init__(
-        self,
-        *,
-        prob_input_selection: Optional[str] = DEFAULT_INPUT_SELECTION,
-        name: Optional[str] = None,
-    ):
-        # --- Arguments processing
-        prob_input = create_prob_input_from_available(
-            prob_input_selection, AVAILABLE_INPUT_SPECS
-        )
-        # Process the default name
-        if name is None:
-            name = OakleyOHagan1D.__name__
-
-        super().__init__(prob_input=prob_input, name=name)
+AVAILABLE_PARAMETERS = {
+    "noisy": np.random.default_rng(),
+    "noiseless": None,
+}
 
-    def evaluate(self, xx: np.ndarray):
-        """Evaluate the 1D Oakley-O'Hagan function on a set of input values.
+DEFAULT_PARAMETERS_SELECTION = "noisy"
 
-        Parameters
-        ----------
-        xx : np.ndarray
-            1-Dimensional input values given by an N-by-1 array
-            where N is the number of input values.
 
-        Returns
-        -------
-        np.ndarray
-            The output of the 1D Oakley-O'Hagan function evaluated
-            on the input values.
-            The output is a 1-dimensional array of length N.
-        """
-        yy = 5 + xx + np.cos(xx)
+def evaluate_1dsine(
+    xx: np.ndarray, parameters: Optional[Generator] = None
+) -> np.ndarray:
+    """Evaluate the 1D Gramacy (2007) Sine function on a set of input values.
+
+    Parameters
+    ----------
+    xx : np.ndarray
+        1-Dimensional input values given by an N-by-1 array
+        where N is the number of input values.
+
+    parameters : Generator, optional
+        A random number generator to generate the noise.
+
+    Returns
+    -------
+    np.ndarray
+        The output of the 1D Gramacy (2007) function evaluated
+        on the input values.
+        The output is a 1-dimensional array of length N.
+    """
+    yy = np.zeros(len(xx))
+    idx_1 = xx[:, 0] <= 9.6
+    idx_2 = xx[:, 0] > 9.6
+    yy[idx_1] = np.sin(0.2 * np.pi * xx[idx_1, 0]) + 0.2 * np.cos(
+        0.8 * np.pi * xx[idx_1, 0]
+    )
+    yy[idx_2] = -1 + 0.1 * xx[idx_2, 0]
+
+    if parameters is not None:
+        yy_noise = parameters.normal(size=len(xx), scale=0.1)
+
+        return yy + yy_noise
+
+    return yy
+
+
+class Gramacy1DSine(UQTestFunABC):
+    """A concrete implementation of the 1D Gramacy (2007) Sine function."""
+
+    _tags = ["metamodeling"]
+    _description = "One-dimensional sine function from Gramacy (2007)"
+    _available_inputs = AVAILABLE_INPUT_SPECS
+    _available_parameters = AVAILABLE_PARAMETERS
+    _default_spatial_dimension = 1
+    _default_parameters = "noisy"
 
-        return yy
+    eval_ = staticmethod(evaluate_1dsine)
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `uqtestfuns-0.1.1/src/uqtestfuns/test_functions/otl_circuit.py` & `uqtestfuns-0.2.0/src/uqtestfuns/test_functions/otl_circuit.py`

 * *Files 8% similar despite different names*

```diff
@@ -19,162 +19,144 @@
 2. H. Moon, "Design and Analysis of Computer Experiments for Screening Input
    Variables," Ph. D. dissertation, Ohio State University, Ohio, 2010.
    URL: http://rave.ohiolink.edu/etdc/view?acc_num=osu1275422248
 """
 import numpy as np
 
 from copy import copy
-from typing import Optional
 
-from ..core.prob_input.univariate_distribution import UnivDist
+from ..core.prob_input.input_spec import UnivDistSpec, ProbInputSpecFixDim
 from ..core.uqtestfun_abc import UQTestFunABC
-from .available import create_prob_input_from_available
 
 __all__ = ["OTLCircuit"]
 
 INPUT_MARGINALS_BENARI2007 = [
-    UnivDist(
+    UnivDistSpec(
         name="Rb1",
         distribution="uniform",
         parameters=[50.0, 150.0],
         description="Resistance b1 [kOhm]",
     ),
-    UnivDist(
+    UnivDistSpec(
         name="Rb2",
         distribution="uniform",
         parameters=[25.0, 70.0],
         description="Resistance b2 [kOhm]",
     ),
-    UnivDist(
+    UnivDistSpec(
         name="Rf",
         distribution="uniform",
         parameters=[0.5, 3.0],
         description="Resistance f [kOhm]",
     ),
-    UnivDist(
+    UnivDistSpec(
         name="Rc1",
         distribution="uniform",
         parameters=[1.2, 2.5],
         description="Resistance c1 [kOhm]",
     ),
-    UnivDist(
+    UnivDistSpec(
         name="Rc2",
         distribution="uniform",
         parameters=[0.25, 1.20],
         description="Resistance c2 [kOhm]",
     ),
-    UnivDist(
+    UnivDistSpec(
         name="beta",
         distribution="uniform",
         parameters=[50.0, 300.0],
         description="Current gain [A]",
     ),
 ]
 
 INPUT_MARGINALS_MOON2010 = [copy(_) for _ in INPUT_MARGINALS_BENARI2007]
 for i in range(14):
     INPUT_MARGINALS_MOON2010.append(
-        UnivDist(
+        UnivDistSpec(
             name=f"Inert {i+1}",
             distribution="uniform",
             parameters=[100.0, 200.0],
             description="Inert input [-]",
         )
     )
 
 AVAILABLE_INPUT_SPECS = {
-    "BenAri2007": {
-        "name": "OTL-Circuit-Ben-Ari-2007",
-        "description": (
+    "BenAri2007": ProbInputSpecFixDim(
+        name="OTLCircuit-BenAri2007",
+        description=(
             "Probabilistic input model for the OTL Circuit function "
             "from Ben-Ari and Steinberg (2007)."
         ),
-        "marginals": INPUT_MARGINALS_BENARI2007,
-        "copulas": None,
-    },
-    "Moon2010": {
-        "name": "OTL-Circuit-Moon-2010",
-        "description": (
+        marginals=INPUT_MARGINALS_BENARI2007,
+        copulas=None,
+    ),
+    "Moon2010": ProbInputSpecFixDim(
+        name="OTLCircuit-Moon2010",
+        description=(
             "Probabilistic input model for the OTL Circuit function "
             "from Moon (2010)."
         ),
-        "marginals": INPUT_MARGINALS_MOON2010,
-        "copulas": None,
-    },
+        marginals=INPUT_MARGINALS_MOON2010,
+        copulas=None,
+    ),
 }
 
 DEFAULT_INPUT_SELECTION = "BenAri2007"
 
 
-class OTLCircuit(UQTestFunABC):
-    """A concrete implementation of the OTL circuit test function."""
+def evaluate(xx: np.ndarray) -> np.ndarray:
+    """Evaluate the OTL circuit test function on a set of input values.
+
+    Parameters
+    ----------
+    xx : np.ndarray
+        (At least) 6-dimensional input values given by N-by-6 arrays
+        where N is the number of input values.
+
+    Returns
+    -------
+    np.ndarray
+        The output of the OTL circuit test function,
+        i.e., the mid-point voltage in Volt.
+        The output is a one-dimensional array of length N.
+
+    Notes
+    -----
+    - The variant of this test function has 14 additional inputs,
+      but they are all taken to be inert and therefore should not affect
+      the output.
+    """
+    rr_b1 = xx[:, 0]  # Resistance b1
+    rr_b2 = xx[:, 1]  # Resistance b2
+    rr_f = xx[:, 2]  # Resistance f
+    rr_c1 = xx[:, 3]  # Resistance c1
+    rr_c2 = xx[:, 4]  # Resistance c2
+    beta = xx[:, 5]  # Current gain
+
+    # Compute the voltage across b1
+    vb1 = 12 * rr_b2 / (rr_b1 + rr_b2)
+
+    # Compute the mid-point voltage
+    denom = beta * (rr_c2 + 9) + rr_f
+    term_1 = ((vb1 + 0.74) * beta * (rr_c2 + 9)) / denom
+    term_2 = 11.35 * rr_f / denom
+    term_3 = 0.74 * rr_f * beta * (rr_c2 + 9) / (rr_c1 * denom)
 
-    _TAGS = ["metamodeling", "sensitivity"]
+    vm = term_1 + term_2 + term_3
 
-    _AVAILABLE_INPUTS = tuple(AVAILABLE_INPUT_SPECS.keys())
+    return vm
 
-    _AVAILABLE_PARAMETERS = None
 
-    _DEFAULT_SPATIAL_DIMENSION = 6
+class OTLCircuit(UQTestFunABC):
+    """A concrete implementation of the OTL circuit test function."""
 
-    _DESCRIPTION = (
+    _tags = ["metamodeling", "sensitivity"]
+    _default_spatial_dimension = 6
+    _description = (
         "Output transformerless (OTL) circuit model "
         "from Ben-Ari and Steinberg (2007)"
     )
+    _available_inputs = AVAILABLE_INPUT_SPECS
+    _available_parameters = None
+    _default_input = DEFAULT_INPUT_SELECTION
 
-    def __init__(
-        self,
-        *,
-        prob_input_selection: Optional[str] = DEFAULT_INPUT_SELECTION,
-        name: Optional[str] = None,
-    ):
-        # --- Arguments processing
-        prob_input = create_prob_input_from_available(
-            prob_input_selection, AVAILABLE_INPUT_SPECS
-        )
-        # Process the default name
-        if name is None:
-            name = OTLCircuit.__name__
-
-        super().__init__(prob_input=prob_input, name=name)
-
-    def evaluate(self, xx: np.ndarray) -> np.ndarray:
-        """Evaluate the OTL circuit test function on a set of input values.
-
-        Parameters
-        ----------
-        xx : np.ndarray
-            (At least) 6-dimensional input values given by N-by-6 arrays
-            where N is the number of input values.
-
-        Returns
-        -------
-        np.ndarray
-            The output of the OTL circuit test function,
-            i.e., the mid-point voltage in Volt.
-            The output is a one-dimensional array of length N.
-
-        Notes
-        -----
-        - The variant of this test function has 14 additional inputs,
-          but they are all taken to be inert and therefore should not affect
-          the output.
-        """
-        rr_b1 = xx[:, 0]  # Resistance b1
-        rr_b2 = xx[:, 1]  # Resistance b2
-        rr_f = xx[:, 2]  # Resistance f
-        rr_c1 = xx[:, 3]  # Resistance c1
-        rr_c2 = xx[:, 4]  # Resistance c2
-        beta = xx[:, 5]  # Current gain
-
-        # Compute the voltage across b1
-        vb1 = 12 * rr_b2 / (rr_b1 + rr_b2)
-
-        # Compute the mid-point voltage
-        denom = beta * (rr_c2 + 9) + rr_f
-        term_1 = ((vb1 + 0.74) * beta * (rr_c2 + 9)) / denom
-        term_2 = 11.35 * rr_f / denom
-        term_3 = 0.74 * rr_f * beta * (rr_c2 + 9) / (rr_c1 * denom)
-
-        vm = term_1 + term_2 + term_3
-
-        return vm
+    eval_ = staticmethod(evaluate)
```

### Comparing `uqtestfuns-0.1.1/src/uqtestfuns/test_functions/piston.py` & `uqtestfuns-0.2.0/src/uqtestfuns/test_functions/piston.py`

 * *Files 19% similar despite different names*

```diff
@@ -19,175 +19,154 @@
 2. H. Moon, "Design and Analysis of Computer Experiments for Screening Input
    Variables," Ph. D. dissertation, Ohio State University, Ohio, 2010.
    URL: http://rave.ohiolink.edu/etdc/view?acc_num=osu1275422248
 """
 import numpy as np
 
 from copy import copy
-from typing import Optional
 
-from ..core.prob_input.univariate_distribution import UnivDist
+from ..core.prob_input.input_spec import UnivDistSpec, ProbInputSpecFixDim
 from ..core.uqtestfun_abc import UQTestFunABC
-from .available import create_prob_input_from_available
 
 __all__ = ["Piston"]
 
 # Marginals specification from [1]
 INPUT_MARGINALS_BENARI2007 = [
-    UnivDist(
+    UnivDistSpec(
         name="M",
         distribution="uniform",
         parameters=[30.0, 60.0],
         description="Piston weight [kg]",
     ),
-    UnivDist(
+    UnivDistSpec(
         name="S",
         distribution="uniform",
         parameters=[0.005, 0.020],
         description="Piston surface area [m^2]",
     ),
-    UnivDist(
+    UnivDistSpec(
         name="V0",
         distribution="uniform",
         parameters=[0.002, 0.010],
         description="Initial gas volume [m^3]",
     ),
-    UnivDist(
+    UnivDistSpec(
         name="k",
         distribution="uniform",
         parameters=[1000.0, 5000.0],
         description="Spring coefficient [N/m]",
     ),
-    UnivDist(
+    UnivDistSpec(
         name="P0",
         distribution="uniform",
         parameters=[90000.0, 110000.0],
         description="Atmospheric pressure [N/m^2]",
     ),
-    UnivDist(
+    UnivDistSpec(
         name="Ta",
         distribution="uniform",
         parameters=[290.0, 296.0],
         description="Ambient temperature [K]",
     ),
-    UnivDist(
+    UnivDistSpec(
         name="T0",
         distribution="uniform",
         parameters=[340.0, 360.0],
         description="Filling gas temperature [K]",
     ),
 ]
 
 # Marginals specification from [2]
 INPUT_MARGINALS_MOON2010 = [copy(_) for _ in INPUT_MARGINALS_BENARI2007]
 for i in range(13):
     INPUT_MARGINALS_MOON2010.append(
-        UnivDist(
+        UnivDistSpec(
             name=f"Inert {i+1}",
             distribution="uniform",
             parameters=[100.0, 200.0],
             description="Inert input [-]",
         )
     )
 
 AVAILABLE_INPUT_SPECS = {
-    "BenAri2007": {
-        "name": "Piston-Ben-Ari-2007",
-        "description": (
+    "BenAri2007": ProbInputSpecFixDim(
+        name="Piston-BenAri2007",
+        description=(
             "Probabilistic input model for the Piston simulation model "
             "from Ben-Ari and Steinberg (2007)."
         ),
-        "marginals": INPUT_MARGINALS_BENARI2007,
-        "copulas": None,
-    },
-    "Moon2010": {
-        "name": "Piston-Moon-2010",
-        "description": (
+        marginals=INPUT_MARGINALS_BENARI2007,
+        copulas=None,
+    ),
+    "Moon2010": ProbInputSpecFixDim(
+        name="Piston-Moon2010",
+        description=(
             "Probabilistic input model for the Piston simulation model "
             "from Moon (2010)."
         ),
-        "marginals": INPUT_MARGINALS_MOON2010,
-        "copulas": None,
-    },
+        marginals=INPUT_MARGINALS_MOON2010,
+        copulas=None,
+    ),
 }
 
 DEFAULT_INPUT_SELECTION = "BenAri2007"
 
 
-class Piston(UQTestFunABC):
-    """A concrete implementation of the Piston simulation test function."""
-
-    _TAGS = ["metamodeling", "sensitivity"]
+def evaluate(xx: np.ndarray) -> np.ndarray:
+    """Evaluate the Piston simulation test function on a set of input values.
 
-    _AVAILABLE_INPUTS = tuple(AVAILABLE_INPUT_SPECS.keys())
+    Parameters
+    ----------
+    xx : np.ndarray
+        (At least) 6-dimensional input values given by N-by-6 arrays
+        where N is the number of input values.
+
+    Returns
+    -------
+    np.ndarray
+        The output of the Piston simulation test function,
+        The output is a one-dimensional array of length N.
+
+    Notes
+    -----
+    - The variant of this test function has 13 additional inputs,
+      but they are all taken to be inert and therefore should not affect
+      the output.
+    """
+    mm = xx[:, 0]  # piston weight
+    ss = xx[:, 1]  # piston surface area
+    vv_0 = xx[:, 2]  # initial gas volume
+    kk = xx[:, 3]  # spring coefficient
+    pp_0 = xx[:, 4]  # atmospheric pressure
+    tt_a = xx[:, 5]  # ambient temperature
+    tt_0 = xx[:, 6]  # filling gas temperature
+
+    # Compute the force
+    aa = pp_0 * ss + 19.62 * mm - kk * vv_0 / ss
+
+    # Compute the force difference
+    daa = np.sqrt(aa**2 + 4.0 * kk * pp_0 * vv_0 * tt_a / tt_0) - aa
+
+    # Compute the volume difference
+    vv = ss / 2.0 / kk * daa
+
+    # Compute the cycle time
+    cc = (
+        2.0
+        * np.pi
+        * np.sqrt(mm / (kk + ss**2 * pp_0 * vv_0 * tt_a / tt_0 / vv**2))
+    )
 
-    _AVAILABLE_PARAMETERS = None
+    return cc
 
-    _DEFAULT_SPATIAL_DIMENSION = 7
 
-    _DESCRIPTION = "Piston simulation model from Ben-Ari and Steinberg (2007)"
+class Piston(UQTestFunABC):
+    """A concrete implementation of the Piston simulation test function."""
 
-    def __init__(
-        self,
-        *,
-        prob_input_selection: Optional[str] = DEFAULT_INPUT_SELECTION,
-        name: Optional[str] = None,
-    ):
-        # --- Arguments processing
-        prob_input = create_prob_input_from_available(
-            prob_input_selection, AVAILABLE_INPUT_SPECS
-        )
-        # Process the default name
-        if name is None:
-            name = Piston.__name__
-
-        super().__init__(prob_input=prob_input, name=name)
-
-    def evaluate(self, xx: np.ndarray) -> np.ndarray:
-        """Evaluate the OTL circuit test function on a set of input values.
-
-        Parameters
-        ----------
-        xx : np.ndarray
-            (At least) 6-dimensional input values given by N-by-6 arrays
-            where N is the number of input values.
-
-        Returns
-        -------
-        np.ndarray
-            The output of the OTL circuit test function,
-            i.e., the mid-point voltage in Volt.
-            The output is a one-dimensional array of length N.
-
-        Notes
-        -----
-        - The variant of this test function has 14 additional inputs,
-          but they are all taken to be inert and therefore should not affect
-          the output.
-        """
-        mm = xx[:, 0]  # piston weight
-        ss = xx[:, 1]  # piston surface area
-        vv_0 = xx[:, 2]  # initial gas volume
-        kk = xx[:, 3]  # spring coefficient
-        pp_0 = xx[:, 4]  # atmospheric pressure
-        tt_a = xx[:, 5]  # ambient temperature
-        tt_0 = xx[:, 6]  # filling gas temperature
-
-        # Compute the force
-        aa = pp_0 * ss + 19.62 * mm - kk * vv_0 / ss
-
-        # Compute the force difference
-        daa = np.sqrt(aa**2 + 4.0 * kk * pp_0 * vv_0 * tt_a / tt_0) - aa
-
-        # Compute the volume difference
-        vv = ss / 2.0 / kk * daa
-
-        # Compute the cycle time
-        cc = (
-            2.0
-            * np.pi
-            * np.sqrt(
-                mm / (kk + ss**2 * pp_0 * vv_0 * tt_a / tt_0 / vv**2)
-            )
-        )
+    _tags = ["metamodeling", "sensitivity"]
+    _description = "Piston simulation model from Ben-Ari and Steinberg (2007)"
+    _available_inputs = AVAILABLE_INPUT_SPECS
+    _available_parameters = None
+    _default_spatial_dimension = 7
+    _default_input = DEFAULT_INPUT_SELECTION
 
-        return cc
+    eval_ = staticmethod(evaluate)
```

### Comparing `uqtestfuns-0.1.1/src/uqtestfuns/test_functions/sobol_g.py` & `uqtestfuns-0.2.0/src/uqtestfuns/test_functions/sobol_g.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,111 +1,171 @@
 """
 Module with an implementation of the Sobol-G test function.
 
 The Sobol'-G function is an M-dimensional scalar-valued function.
 It was introduced in [1] for testing numerical integration algorithms
-(e.g., quasi-Monte-Carlo; see for instance [2].
+(e.g., quasi-Monte-Carlo; see also for instance [2] and [3]).
+The current form (and name) was from [4] and used in the context of global
+sensitivity analysis. There, the function was generalized by introducing
+a set of parameters that determines the importance of each input variable.
 Later on, it becomes a popular testing function for global sensitivity analysis
-methods; see, for instances, [3], [4], and [5].
+methods; see, for instances, [5], [6], and [7].
 
-The parameters of the Sobol'-G function (i.e., the coefficients) determine
-the importance of each input variable.
 There are several sets of parameters used in the literature.
 
 Notes
 -----
-- The parameters used in [3] and [4] correspond to
-  the parameter choice 3 in [1].
+- The parameters used in [5] and [6] correspond to
+  the parameter choice 3 in [3].
 
 References
 ----------
-1. I. Radović, I. M. Sobol’, and R. F. Tichy, “Quasi-Monte Carlo Methods for
+
+1. Paul Bratley, Bennet L. Fox, and Harald Niederreiter, "Implementation and
+   tests of low-discrepancy sequences," ACM Transactions on Modeling and
+   Computer Simulation, vol. 2, no. 3, pp. 195-213, 1992.
+   DOI:10.1145/146382.146385
+2. I. Radović, I. M. Sobol’, and R. F. Tichy, “Quasi-Monte Carlo Methods for
    Numerical Integration: Comparison of Different Low Discrepancy Sequences,”
    Monte Carlo Methods and Applications, vol. 2, no. 1, pp. 1–14, 1996.
    DOI: 10.1515/mcma.1996.2.1.1.
-2. I. M. Sobol’, “On quasi-Monte Carlo integrations,” Mathematics and Computers
+3. I. M. Sobol’, “On quasi-Monte Carlo integrations,” Mathematics and Computers
    in Simulation, vol. 47, no. 2–5, pp. 103–112, 1998.
    DOI: 10.1016/S0378-4754(98)00096-2
-3. A. Marrel, B. Iooss, F. Van Dorpe, and E. Volkova, “An efficient
+4. A. Saltelli and I. M. Sobol’, “About the use of rank transformation in
+   sensitivity analysis of model output,” Reliability Engineering
+   & System Safety, vol. 50, no. 3, pp. 225–239, 1995.
+   DOI: 10.1016/0951-8320(95)00099-2.
+5. A. Marrel, B. Iooss, F. Van Dorpe, and E. Volkova, “An efficient
    methodology for modeling complex computer codes with Gaussian processes,”
    Computational Statistics & Data Analysis, vol. 52, no. 10,
    pp. 4731–4744, 2008.
    DOI: 10.1016/j.csda.2008.03.026
-4. A. Marrel, B. Iooss, B. Laurent, and O. Roustant, “Calculations of Sobol
+6. A. Marrel, B. Iooss, B. Laurent, and O. Roustant, “Calculations of Sobol
    indices for the Gaussian process metamodel,” Reliability Engineering &
    System Safety, vol. 94, no. 3, pp. 742–751, 2009.
     DOI: 10.1016/j.ress.2008.07.008
-5. S. Kucherenko, B. Feil, N. Shah, and W. Mauntz, “The identification of
+7. S. Kucherenko, B. Feil, N. Shah, and W. Mauntz, “The identification of
    model effective dimensions using global sensitivity analysis,”
    Reliability Engineering & System Safety, vol. 96, no. 4, pp. 440–449, 2011.
    DOI: 10.1016/j.ress.2010.11.003
-6. T. Crestaux, J.-M. Martinez, O. Le Maître, and O. Lafitte, “Polynomial
+8. T. Crestaux, J.-M. Martinez, O. Le Maître, and O. Lafitte, “Polynomial
    chaos expansion for uncertainties quantification and sensitivity analysis,”
    presented at the Fifth International Conference on Sensitivity Analysis
    of Model Output, 2007.
    Accessed: Jan. 25, 2023
    URL: http://samo2007.chem.elte.hu/lectures/Crestaux.pdf
 """
 import numpy as np
 
-from typing import List, Optional
+from typing import List
 
-from ..core.prob_input.univariate_distribution import UnivDist
+from ..core.prob_input.input_spec import UnivDistSpec, ProbInputSpecVarDim
 from ..core.uqtestfun_abc import UQTestFunABC
-from .available import (
-    create_prob_input_from_available,
-    create_parameters_from_available,
-)
 
 __all__ = ["SobolG"]
 
 
-def _create_sobol_input(spatial_dimension: int) -> List[UnivDist]:
+def _create_sobol_input(spatial_dimension: int) -> List[UnivDistSpec]:
     """Construct an input instance for a given dimension according to [1].
 
     Parameters
     ----------
     spatial_dimension : int
         The number of marginals to be created.
 
     Returns
     -------
-    List[UnivDist]
+    List[UnivDistSpec]
         A list of M marginals as UnivariateInput instances to construct
         the MultivariateInput.
     """
     marginals = []
     for i in range(spatial_dimension):
         marginals.append(
-            UnivDist(
+            UnivDistSpec(
                 name=f"X{i + 1}",
                 distribution="uniform",
                 parameters=[0.0, 1.0],
                 description="None",
             )
         )
 
     return marginals
 
 
 AVAILABLE_INPUT_SPECS = {
-    "Radovic1996": {
-        "name": "Sobol-G-Radovic-1996",
-        "description": (
+    "Radovic1996": ProbInputSpecVarDim(
+        name="Sobol-G-Radovic-1996",
+        description=(
             "Probabilistic input model for the Sobol'-G function "
             "from Radović et al. (1996)."
         ),
-        "marginals": _create_sobol_input,
-        "copulas": None,
-    },
+        marginals_generator=_create_sobol_input,
+        copulas=None,
+    ),
 }
 
 DEFAULT_INPUT_SELECTION = "Radovic1996"
 
 
+def _get_params_saltelli_1995_1(spatial_dimension: int) -> np.ndarray:
+    """Construct a parameter array for Sobol'-G according to example 1 in [4].
+
+    Notes
+    -----
+    - The function was most probably first appear in its original form
+      in [1] (without parameters).
+    - With the selected parameters, all input variables are equally important.
+    """
+    yy = np.zeros(spatial_dimension)
+
+    return yy
+
+
+def _get_params_saltelli_1995_2(spatial_dimension: int) -> np.ndarray:
+    """Construct a parameter array for Sobol'-G according to example 2 in [4].
+
+    Notes
+    -----
+    - With the selected parameters, the first two input variables are
+      important, one is moderately important, and the rest is non-influential.
+    - Originally, the dimension is limited to 8-dimensions; if more dimensions
+      are used then the remaining dimension is also non-influential.
+    """
+    yy = np.zeros(spatial_dimension)
+
+    if spatial_dimension > 1:
+        yy[1] = 0
+
+    if spatial_dimension > 2:
+        yy[2] = 3
+
+    if spatial_dimension > 3:
+        yy[3:] = 9
+
+    return yy
+
+
+def _get_params_saltelli_1995_3(spatial_dimension: int) -> np.ndarray:
+    """Construct a parameter array for Sobol'-G according to example 3 in [4].
+
+    Notes
+    -----
+    - With the selected parameters, the first input variable is the most
+      important and the importance of the remaining variables is decreasing.
+    - Originally, the dimension is limited to 20-dimensions; if more dimensions
+      are used then the remaining dimension is also non-influential.
+    - The parameter set is also used in [8].
+    """
+    yy = (np.arange(1, spatial_dimension + 1) - 1) / 2.0
+
+    return yy
+
+
 def _get_params_sobol_1998_1(spatial_dimension: int) -> np.ndarray:
     """Construct a parameter array for Sobol'-G according to choice 1 in [2].
 
     Notes
     -----
     - Using this choice of parameters, the supremum of the Sobol-G function
       grows exponentially as a function of dimension about 2^M [1].
@@ -173,93 +233,56 @@
       grows exponentially as a function of dimension about (1.13)^M.
     """
     yy = 6.52 * np.ones(spatial_dimension)
 
     return yy
 
 
-def _get_params_crestaux_2007(spatial_dimension: int) -> np.ndarray:
-    """Construct a parameter array for Sobol'-G according to [6]."""
-    yy = (np.arange(1, spatial_dimension + 1) - 1) / 2.0
-
-    return yy
-
-
 AVAILABLE_PARAMETERS = {
+    "Saltelli1995-1": _get_params_saltelli_1995_1,
+    "Saltelli1995-2": _get_params_saltelli_1995_2,
+    "Saltelli1995-3": _get_params_saltelli_1995_3,
     "Sobol1998-1": _get_params_sobol_1998_1,
     "Sobol1998-2": _get_params_sobol_1998_2,
     "Sobol1998-3": _get_params_sobol_1998_3,
     "Sobol1998-4": _get_params_sobol_1998_4,
     "Kucherenko2011-2a": _get_params_kucherenko_2011_2a,
     "Kucherenko2011-3b": _get_params_kucherenko_2011_3b,
-    "Crestaux2007": _get_params_crestaux_2007,
 }
 
-DEFAULT_PARAMETERS_SELECTION = "Crestaux2007"
-
-# The dimension is variable, it requires a default for fallback
-DEFAULT_DIMENSION_SELECTION = 2
+DEFAULT_PARAMETERS_SELECTION = "Saltelli1995-3"
 
 
-class SobolG(UQTestFunABC):
-    """A concrete implementation of the M-dimensional Sobol'-G function."""
+def evaluate(xx: np.ndarray, parameters: np.ndarray):
+    """Evaluate the Sobol-G function on a set of input values.
 
-    _TAGS = ["sensitivity"]
-
-    _AVAILABLE_INPUTS = tuple(AVAILABLE_INPUT_SPECS.keys())
+    Parameters
+    ----------
+    xx : np.ndarray
+        M-Dimensional input values given by an N-by-M array where
+        N is the number of input values.
+    parameters : np.ndarray
+        The parameters (i.e., coefficients) of the Sobol'-G function.
 
-    _AVAILABLE_PARAMETERS = tuple(AVAILABLE_PARAMETERS.keys())
+    Returns
+    -------
+    np.ndarray
+        The output of the Sobol-G function evaluated on the input values.
+        The output is a 1-dimensional array of length N.
+    """
+    aa = parameters
+    yy = np.prod(((np.abs(4 * xx - 2) + aa) / (1 + aa)), axis=1)
 
-    _DEFAULT_SPATIAL_DIMENSION = None
-
-    _DESCRIPTION = "Sobol'-G function from Radović et al. (1996)"
-
-    def __init__(
-        self,
-        spatial_dimension: int = DEFAULT_DIMENSION_SELECTION,
-        *,
-        prob_input_selection: Optional[str] = DEFAULT_INPUT_SELECTION,
-        parameters_selection: Optional[str] = DEFAULT_PARAMETERS_SELECTION,
-        name: Optional[str] = None,
-    ):
-        # --- Arguments processing
-        if not isinstance(spatial_dimension, int):
-            raise TypeError(
-                f"Spatial dimension is expected to be of 'int'. "
-                f"Got {type(spatial_dimension):!r} instead."
-            )
-        # Sobol-G is an M-dimensional test function, either given / use default
-        # Create the input according to spatial dimension
-        prob_input = create_prob_input_from_available(
-            prob_input_selection, AVAILABLE_INPUT_SPECS, spatial_dimension
-        )
-        # Create the parameters according to spatial dimension
-        parameters = create_parameters_from_available(
-            parameters_selection, AVAILABLE_PARAMETERS, spatial_dimension
-        )
-        # Process the default name
-        if name is None:
-            name = SobolG.__name__
+    return yy
 
-        super().__init__(
-            prob_input=prob_input, parameters=parameters, name=name
-        )
 
-    def evaluate(self, xx: np.ndarray):
-        """Evaluate the Sobol-G function on a set of input values.
+class SobolG(UQTestFunABC):
+    """An implementation of the M-dimensional Sobol'-G test function."""
 
-        Parameters
-        ----------
-        xx : np.ndarray
-            M-Dimensional input values given by an N-by-M array where
-            N is the number of input values.
-
-        Returns
-        -------
-        np.ndarray
-            The output of the Sobol-G function evaluated on the input values.
-            The output is a 1-dimensional array of length N.
-        """
-        params = self.parameters
-        yy = np.prod(((np.abs(4 * xx - 2) + params) / (1 + params)), axis=1)
+    _tags = ["sensitivity", "integration"]
+    _description = "Sobol'-G function from Saltelli and Sobol' (1995)"
+    _available_inputs = AVAILABLE_INPUT_SPECS
+    _available_parameters = AVAILABLE_PARAMETERS
+    _default_parameters = DEFAULT_PARAMETERS_SELECTION
+    _default_spatial_dimension = None
 
-        return yy
+    eval_ = staticmethod(evaluate)
```

### Comparing `uqtestfuns-0.1.1/src/uqtestfuns/test_functions/utils.py` & `uqtestfuns-0.2.0/src/uqtestfuns/test_functions/utils.py`

 * *Files identical despite different names*

### Comparing `uqtestfuns-0.1.1/src/uqtestfuns/test_functions/wing_weight.py` & `uqtestfuns-0.2.0/src/uqtestfuns/test_functions/wing_weight.py`

 * *Files 11% similar despite different names*

```diff
@@ -17,151 +17,129 @@
    and Rhea P. Liem, "Gradient-enhanced universal Kriging with polynomial
    chaos as trend function," In AIAA Scitech 2020 Forum,
    Orlando, Florida, 2020. American Institute of Aeronautics and Astronautics.
    DOI: 10.2514/6.2020-1865.
 """
 import numpy as np
 
-from typing import Optional
-
-from ..core.prob_input.univariate_distribution import UnivDist
+from ..core.prob_input.input_spec import UnivDistSpec, ProbInputSpecFixDim
 from ..core.uqtestfun_abc import UQTestFunABC
-from .available import create_prob_input_from_available
 from .utils import deg2rad
 
 __all__ = ["WingWeight"]
 
 INPUT_MARGINALS_FORRESTER2008 = [
-    UnivDist(
+    UnivDistSpec(
         name="Sw",
         distribution="uniform",
         parameters=[150.0, 200.0],
         description="wing area [ft^2]",
     ),
-    UnivDist(
+    UnivDistSpec(
         name="Wfw",
         distribution="uniform",
         parameters=[220.0, 300.0],
         description="weight of fuel in the wing [lb]",
     ),
-    UnivDist(
+    UnivDistSpec(
         name="A",
         distribution="uniform",
         parameters=[6.0, 10.0],
         description="aspect ratio [-]",
     ),
-    UnivDist(
+    UnivDistSpec(
         name="Lambda",
         distribution="uniform",
         parameters=[-10.0, 10.0],
         description="quarter-chord sweep [degrees]",
     ),
-    UnivDist(
+    UnivDistSpec(
         name="q",
         distribution="uniform",
         parameters=[16.0, 45.0],
         description="dynamic pressure at cruise [lb/ft^2]",
     ),
-    UnivDist(
+    UnivDistSpec(
         name="lambda",
         distribution="uniform",
         parameters=[0.5, 1.0],
         description="taper ratio [-]",
     ),
-    UnivDist(
+    UnivDistSpec(
         name="tc",
         distribution="uniform",
         parameters=[0.08, 0.18],
         description="aerofoil thickness to chord ratio [-]",
     ),
-    UnivDist(
+    UnivDistSpec(
         name="Nz",
         distribution="uniform",
         parameters=[2.5, 6.0],
         description="ultimate load factor [-]",
     ),
-    UnivDist(
+    UnivDistSpec(
         name="Wdg",
         distribution="uniform",
         parameters=[1700, 2500],
         description="flight design gross weight [lb]",
     ),
-    UnivDist(
+    UnivDistSpec(
         name="Wp",
         distribution="uniform",
         parameters=[0.025, 0.08],
         description="paint weight [lb/ft^2]",
     ),
 ]
 
 AVAILABLE_INPUT_SPECS = {
-    "Forrester2008": {
-        "name": "Wing-Weight-Forrester-2008",
-        "description": (
+    "Forrester2008": ProbInputSpecFixDim(
+        name="Wing-Weight-Forrester-2008",
+        description=(
             "Probabilistic input model for the Wing Weight model "
             "from Forrester et al. (2008)."
         ),
-        "marginals": INPUT_MARGINALS_FORRESTER2008,
-        "copulas": None,
-    }
+        marginals=INPUT_MARGINALS_FORRESTER2008,
+        copulas=None,
+    ),
 }
 
-DEFAULT_INPUT_SELECTION = "Forrester2008"
 
+def evaluate(xx: np.ndarray) -> np.ndarray:
+    """Evaluate the Wing Weight function on a set of input values.
 
-class WingWeight(UQTestFunABC):
-    """A concrete implementation of the wing weight test function."""
+    Parameters
+    ----------
+    xx : np.ndarray
+        10-Dimensional input values given by N-by-10 arrays where
+        N is the number of input values.
+
+    Returns
+    -------
+    np.ndarray
+        The output of the Wing Weight function evaluated
+        on the input values.
+        The output is a 1-dimensional array of length N.
+    """
+    # Compute the Wing Weight function
+    term_1 = 0.036 * xx[:, 0] ** 0.758 * xx[:, 1] ** 0.0035
+    term_2 = (xx[:, 2] / np.cos(deg2rad(xx[:, 3])) ** 2) ** 0.6
+    term_3 = xx[:, 4] ** 0.006
+    term_4 = xx[:, 5] ** 0.04
+    term_5 = (100 * xx[:, 6] / np.cos(np.pi / 180.0 * xx[:, 3])) ** (-0.3)
+    term_6 = (xx[:, 7] * xx[:, 8]) ** 0.49
+    term_7 = xx[:, 0] * xx[:, 9]
 
-    _TAGS = ["metamodeling", "sensitivity"]
+    yy = term_1 * term_2 * term_3 * term_4 * term_5 * term_6 + term_7
 
-    _AVAILABLE_INPUTS = tuple(AVAILABLE_INPUT_SPECS.keys())
+    return yy
 
-    _AVAILABLE_PARAMETERS = None
 
-    _DEFAULT_SPATIAL_DIMENSION = 10
-
-    _DESCRIPTION = "Wing weight model from Forrester et al. (2008)"
-
-    def __init__(
-        self,
-        *,
-        prob_input_selection: Optional[str] = DEFAULT_INPUT_SELECTION,
-        name: Optional[str] = None,
-    ):
-        # --- Arguments processing
-        prob_input = create_prob_input_from_available(
-            prob_input_selection, AVAILABLE_INPUT_SPECS
-        )
-        # Process the default name
-        if name is None:
-            name = WingWeight.__name__
-
-        super().__init__(prob_input=prob_input, name=name)
-
-    def evaluate(self, xx):
-        """Evaluate the Wing Weight function on a set of input values.
-
-        Parameters
-        ----------
-        xx : np.ndarray
-            10-Dimensional input values given by N-by-10 arrays where
-            N is the number of input values.
-
-        Returns
-        -------
-        np.ndarray
-            The output of the Wing Weight function evaluated
-            on the input values.
-            The output is a 1-dimensional array of length N.
-        """
-        # Compute the Wing Weight function
-        term_1 = 0.036 * xx[:, 0] ** 0.758 * xx[:, 1] ** 0.0035
-        term_2 = (xx[:, 2] / np.cos(deg2rad(xx[:, 3])) ** 2) ** 0.6
-        term_3 = xx[:, 4] ** 0.006
-        term_4 = xx[:, 5] ** 0.04
-        term_5 = (100 * xx[:, 6] / np.cos(np.pi / 180.0 * xx[:, 3])) ** (-0.3)
-        term_6 = (xx[:, 7] * xx[:, 8]) ** 0.49
-        term_7 = xx[:, 0] * xx[:, 9]
+class WingWeight(UQTestFunABC):
+    """A concrete implementation of the wing weight test function."""
 
-        yy = term_1 * term_2 * term_3 * term_4 * term_5 * term_6 + term_7
+    _tags = ["metamodeling", "sensitivity"]
+    _description = "Wing weight model from Forrester et al. (2008)"
+    _available_inputs = AVAILABLE_INPUT_SPECS
+    _available_parameters = None
+    _default_spatial_dimension = 10
 
-        return yy
+    eval_ = staticmethod(evaluate)
```

### Comparing `uqtestfuns-0.1.1/src/uqtestfuns/utils.py` & `uqtestfuns-0.2.0/src/uqtestfuns/utils.py`

 * *Files 5% similar despite different names*

```diff
@@ -4,15 +4,21 @@
 import os
 import inspect
 
 from importlib import import_module
 from typing import List, Optional, Tuple, Any
 from types import ModuleType
 
-SUPPORTED_TAGS = ["sensitivity", "optimization", "metamodeling", "reliability"]
+SUPPORTED_TAGS = [
+    "sensitivity",
+    "optimization",
+    "metamodeling",
+    "reliability",
+    "integration",
+]
 
 
 def get_available_classes(
     package: ModuleType, exclude: Optional[List[str]] = None
 ) -> List[Tuple[str, Any]]:
     """Get the available classes within a given package.
```

### Comparing `uqtestfuns-0.1.1/src/uqtestfuns.egg-info/PKG-INFO` & `uqtestfuns-0.2.0/src/uqtestfuns.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: uqtestfuns
-Version: 0.1.1
+Version: 0.2.0
 Summary: A Python3 library of test functions from the uncertainty quantification community with a common interface for benchmarking purpose.
 Home-page: https://github.com/damar-wicaksono/uqtestfuns
 Author: Damar Wicaksono
 Author-email: damar.wicaksono@outlook.com
 License: MIT
 Platform: ANY
 Classifier: License :: OSI Approved :: MIT License
@@ -22,15 +22,15 @@
 Description-Content-Type: text/markdown
 Provides-Extra: dev
 Provides-Extra: docs
 Provides-Extra: all
 License-File: LICENSE
 
 # UQTestFuns
-[![DOI](http://img.shields.io/badge/DOI-10.5281/zenodo.7701904-blue.svg?style=flat-square)](https://doi.org/10.5281/zenodo.7701904)
+[![DOI](http://img.shields.io/badge/DOI-10.5281/zenodo.7703922-blue.svg?style=flat-square)](https://doi.org/10.5281/zenodo.7703922)
 [![Code style: black](https://img.shields.io/badge/code%20style-black-000000.svg?style=flat-square)](https://github.com/psf/black)
 [![Python 3.8](https://img.shields.io/badge/python-3.7-blue.svg?style=flat-square)](https://www.python.org/downloads/release/python-370/)
 [![License](https://img.shields.io/github/license/damar-wicaksono/uqtestfuns?style=flat-square)](https://choosealicense.com/licenses/mit/)
 
 |                                  Branches                                  | Status                                                                                                                                                                                                                                                                                                                                                                                                                                                                                            |
 |:--------------------------------------------------------------------------:|---------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
 | [`main`](https://github.com/damar-wicaksono/uqtestfuns/tree/main) (stable) | ![build](https://img.shields.io/github/actions/workflow/status/damar-wicaksono/uqtestfuns/main.yml?branch=main&style=flat-square) [![codecov](https://img.shields.io/codecov/c/github/damar-wicaksono/uqtestfuns/main?logo=CodeCov&style=flat-square&token=Y6YQEPJ1TT)](https://app.codecov.io/gh/damar-wicaksono/uqtestfuns/tree/main) [![Docs](https://readthedocs.org/projects/uqtestfuns/badge/?version=stable&style=flat-square)](https://uqtestfuns.readthedocs.io/en/latest/?badge=stable) |
```

### Comparing `uqtestfuns-0.1.1/src/uqtestfuns.egg-info/SOURCES.txt` & `uqtestfuns-0.2.0/src/uqtestfuns.egg-info/SOURCES.txt`

 * *Files 15% similar despite different names*

```diff
@@ -14,14 +14,15 @@
 src/uqtestfuns.egg-info/requires.txt
 src/uqtestfuns.egg-info/top_level.txt
 src/uqtestfuns/core/__init__.py
 src/uqtestfuns/core/uqtestfun.py
 src/uqtestfuns/core/uqtestfun_abc.py
 src/uqtestfuns/core/utils.py
 src/uqtestfuns/core/prob_input/__init__.py
+src/uqtestfuns/core/prob_input/input_spec.py
 src/uqtestfuns/core/prob_input/probabilistic_input.py
 src/uqtestfuns/core/prob_input/univariate_distribution.py
 src/uqtestfuns/core/prob_input/utils.py
 src/uqtestfuns/core/prob_input/univariate_distributions/__init__.py
 src/uqtestfuns/core/prob_input/univariate_distributions/beta.py
 src/uqtestfuns/core/prob_input/univariate_distributions/gumbel.py
 src/uqtestfuns/core/prob_input/univariate_distributions/logitnormal.py
@@ -34,20 +35,25 @@
 src/uqtestfuns/core/prob_input/univariate_distributions/utils.py
 src/uqtestfuns/meta/__init__.py
 src/uqtestfuns/meta/basis_functions.py
 src/uqtestfuns/meta/metaspec.py
 src/uqtestfuns/meta/uqmetatestfun.py
 src/uqtestfuns/test_functions/__init__.py
 src/uqtestfuns/test_functions/ackley.py
-src/uqtestfuns/test_functions/available.py
 src/uqtestfuns/test_functions/borehole.py
+src/uqtestfuns/test_functions/bratley1992.py
 src/uqtestfuns/test_functions/damped_oscillator.py
 src/uqtestfuns/test_functions/flood.py
+src/uqtestfuns/test_functions/forrester.py
+src/uqtestfuns/test_functions/franke.py
+src/uqtestfuns/test_functions/gramacy2007.py
 src/uqtestfuns/test_functions/ishigami.py
-src/uqtestfuns/test_functions/oakley_ohagan_1d.py
+src/uqtestfuns/test_functions/mclain.py
+src/uqtestfuns/test_functions/oakley2002.py
 src/uqtestfuns/test_functions/otl_circuit.py
 src/uqtestfuns/test_functions/piston.py
 src/uqtestfuns/test_functions/sobol_g.py
 src/uqtestfuns/test_functions/sulfur.py
 src/uqtestfuns/test_functions/utils.py
+src/uqtestfuns/test_functions/welch1992.py
 src/uqtestfuns/test_functions/wing_weight.py
 tests/test_list_functions.py
```

### Comparing `uqtestfuns-0.1.1/tests/test_list_functions.py` & `uqtestfuns-0.2.0/tests/test_list_functions.py`

 * *Files identical despite different names*

