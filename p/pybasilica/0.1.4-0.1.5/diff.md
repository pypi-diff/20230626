# Comparing `tmp/pybasilica-0.1.4.tar.gz` & `tmp/pybasilica-0.1.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pybasilica-0.1.4.tar", last modified: Wed May 31 09:14:53 2023, max compression
+gzip compressed data, was "pybasilica-0.1.5.tar", last modified: Mon Jun 26 09:31:25 2023, max compression
```

## Comparing `pybasilica-0.1.4.tar` & `pybasilica-0.1.5.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 elenab     (501) staff       (20)        0 2023-05-31 09:14:53.966806 pybasilica-0.1.4/
--rw-r--r--   0 elenab     (501) staff       (20)    35149 2023-03-23 14:20:05.000000 pybasilica-0.1.4/LICENSE
--rw-r--r--   0 elenab     (501) staff       (20)      397 2023-05-31 09:14:53.966684 pybasilica-0.1.4/PKG-INFO
--rw-r--r--   0 elenab     (501) staff       (20)       90 2023-03-23 14:20:05.000000 pybasilica-0.1.4/README.md
-drwxr-xr-x   0 elenab     (501) staff       (20)        0 2023-05-31 09:14:53.965790 pybasilica-0.1.4/pybasilica/
--rw-r--r--   0 elenab     (501) staff       (20)       31 2023-03-28 16:01:28.000000 pybasilica-0.1.4/pybasilica/__init__.py
--rw-r--r--   0 elenab     (501) staff       (20)     3566 2023-03-30 17:31:10.000000 pybasilica-0.1.4/pybasilica/main.py
--rw-r--r--   0 elenab     (501) staff       (20)     9474 2023-05-30 17:34:40.000000 pybasilica-0.1.4/pybasilica/run.py
--rw-r--r--   0 elenab     (501) staff       (20)     8718 2023-03-28 16:01:28.000000 pybasilica-0.1.4/pybasilica/simulation.py
--rw-r--r--   0 elenab     (501) staff       (20)    32219 2023-05-31 09:12:36.000000 pybasilica-0.1.4/pybasilica/svi.py
--rw-r--r--   0 elenab     (501) staff       (20)     6155 2023-03-28 16:01:28.000000 pybasilica-0.1.4/pybasilica/utilities.py
-drwxr-xr-x   0 elenab     (501) staff       (20)        0 2023-05-31 09:14:53.966510 pybasilica-0.1.4/pybasilica.egg-info/
--rw-r--r--   0 elenab     (501) staff       (20)      397 2023-05-31 09:14:53.000000 pybasilica-0.1.4/pybasilica.egg-info/PKG-INFO
--rw-r--r--   0 elenab     (501) staff       (20)      322 2023-05-31 09:14:53.000000 pybasilica-0.1.4/pybasilica.egg-info/SOURCES.txt
--rw-r--r--   0 elenab     (501) staff       (20)        1 2023-05-31 09:14:53.000000 pybasilica-0.1.4/pybasilica.egg-info/dependency_links.txt
--rw-r--r--   0 elenab     (501) staff       (20)      104 2023-05-31 09:14:53.000000 pybasilica-0.1.4/pybasilica.egg-info/requires.txt
--rw-r--r--   0 elenab     (501) staff       (20)       11 2023-05-31 09:14:53.000000 pybasilica-0.1.4/pybasilica.egg-info/top_level.txt
--rw-r--r--   0 elenab     (501) staff       (20)       38 2023-05-31 09:14:53.966838 pybasilica-0.1.4/setup.cfg
--rw-r--r--   0 elenab     (501) staff       (20)      765 2023-05-31 09:13:08.000000 pybasilica-0.1.4/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 09:31:25.426395 pybasilica-0.1.5/
+-rw-r--r--   0 runner    (1001) docker     (123)    35149 2023-06-26 09:31:10.000000 pybasilica-0.1.5/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      434 2023-06-26 09:31:25.426395 pybasilica-0.1.5/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)       90 2023-06-26 09:31:10.000000 pybasilica-0.1.5/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 09:31:25.426395 pybasilica-0.1.5/pybasilica/
+-rw-r--r--   0 runner    (1001) docker     (123)       31 2023-06-26 09:31:10.000000 pybasilica-0.1.5/pybasilica/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3566 2023-06-26 09:31:10.000000 pybasilica-0.1.5/pybasilica/main.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10760 2023-06-26 09:31:10.000000 pybasilica-0.1.5/pybasilica/run.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8718 2023-06-26 09:31:10.000000 pybasilica-0.1.5/pybasilica/simulation.py
+-rw-r--r--   0 runner    (1001) docker     (123)    35268 2023-06-26 09:31:10.000000 pybasilica-0.1.5/pybasilica/svi.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6155 2023-06-26 09:31:10.000000 pybasilica-0.1.5/pybasilica/utilities.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 09:31:25.426395 pybasilica-0.1.5/pybasilica.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      434 2023-06-26 09:31:25.000000 pybasilica-0.1.5/pybasilica.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      322 2023-06-26 09:31:25.000000 pybasilica-0.1.5/pybasilica.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-26 09:31:25.000000 pybasilica-0.1.5/pybasilica.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      104 2023-06-26 09:31:25.000000 pybasilica-0.1.5/pybasilica.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       11 2023-06-26 09:31:25.000000 pybasilica-0.1.5/pybasilica.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-26 09:31:25.426395 pybasilica-0.1.5/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      765 2023-06-26 09:31:10.000000 pybasilica-0.1.5/setup.py
```

### Comparing `pybasilica-0.1.4/LICENSE` & `pybasilica-0.1.5/LICENSE`

 * *Files identical despite different names*

### Comparing `pybasilica-0.1.4/pybasilica/main.py` & `pybasilica-0.1.5/pybasilica/main.py`

 * *Files identical despite different names*

### Comparing `pybasilica-0.1.4/pybasilica/run.py` & `pybasilica-0.1.5/pybasilica/run.py`

 * *Files 16% similar despite different names*

```diff
@@ -6,24 +6,49 @@
 from rich.progress import Progress, BarColumn, TextColumn, TaskProgressColumn, TimeRemainingColumn, SpinnerColumn, RenderableColumn
 from rich.live import Live
 from rich.table import Table
 from sys import maxsize
 
 from pybasilica.svi import PyBasilica
 
-def single_run(kwargs):
-    obj = PyBasilica(**kwargs)
-    obj._fit()
+def single_run(seed_list, save_runs_seed, kwargs):
+    minBic = maxsize
+    bestRun = None
+    runs_seed = dict()
 
-    return obj
+    scores = dict()
 
+    for seed in seed_list:
+        obj = PyBasilica(seed=seed, **kwargs)
+        obj._fit()
 
-def fit(x, k_list=[0,1,2,3,4,5], lr=0.05, n_steps=500, enumer="sequential", cluster=None, groups=None, beta_fixed=None, compile_model = False, \
-        CUDA = False, enforce_sparsity = False, regularizer = "cosine", reg_weight = 1, reg_bic = False, store_parameters=False, verbose=True, 
-        stage = "random_noise", regul_compare = None, seed = 10):
+        scores["seed_"+str(seed)] = {"bic":obj.bic, "llik":obj.likelihood}
+
+        if bestRun is None or obj.bic < minBic:
+            minBic = obj.bic
+            bestRun = obj
+
+        if save_runs_seed:
+            runs_seed["seed_"+str(seed)] = obj
+
+    bestRun.runs_scores = scores
+
+    if save_runs_seed:
+        bestRun.runs_seed = runs_seed
+
+    return bestRun
+
+
+def fit(x, k_list=[0,1,2,3,4,5], lr=0.05, n_steps=500, enumer="parallel", cluster=None, groups=None, beta_fixed=None, hyperparameters=None,
+        compile_model = False, CUDA = False, enforce_sparsity = False, regularizer = "cosine", reg_weight = 1, reg_bic = False,
+        store_parameters=False, verbose=True, stage = "random_noise", regul_compare = None, seed = 10, initializ_seed = True, 
+        save_runs_seed = False, initializ_pars_fit = False):
+
+    if isinstance(seed, int):
+        seed = [seed]
 
     if isinstance(k_list, list):
         if len(k_list) > 0: pass
         else: raise Exception("k_list is an empty list!")
     elif isinstance(k_list, int):
         k_list = [k_list]
     else: raise Exception("invalid k_list datatype")
@@ -32,24 +57,26 @@
             "x":x,
             "lr":lr,
             "n_steps":n_steps,
             "enumer":enumer,
             "cluster":cluster,
             "groups":groups,
             "beta_fixed":beta_fixed,
+            "hyperparameters":hyperparameters,
             "compile_model":compile_model,
             "CUDA":CUDA,
             "enforce_sparsity":enforce_sparsity,
             "regularizer":regularizer,
             "reg_weight":reg_weight,
             "reg_bic":reg_bic,
             "store_parameters":store_parameters,
             "stage":stage,
             "regul_compare":regul_compare,
-            "seed":seed
+            "initializ_seed":initializ_seed,
+            "initializ_pars_fit":initializ_pars_fit
         }
 
     if verbose:
     # Verbose run
 
         console = Console()
         if beta_fixed is None:
@@ -72,45 +99,50 @@
         myProgress = Progress(
             TextColumn('{task.description} [bold blue] inference {task.completed}/{task.total} done'), 
             BarColumn(), 
             TaskProgressColumn(), 
             TimeRemainingColumn(), 
             SpinnerColumn(), 
             RenderableColumn())
-        
+
         with myProgress as progress:
 
             task = progress.add_task("[red]running...", total=len(k_list))
 
             minBic = maxsize
             secondMinBic = maxsize
             bestRun, secondBest = None, None
+
+            scores_k = dict()
             for k in k_list:
                 kwargs["k_denovo"] = k
 
                 try:
-                    obj = single_run(kwargs)
+                    obj = single_run(seed_list=seed, save_runs_seed=save_runs_seed, kwargs=kwargs)
 
                     if obj.bic < minBic:
                         minBic = obj.bic
                         bestRun = obj
-                    if obj.bic > minBic and obj.bic < secondMinBic:
+                    if minBic == secondMinBic or (obj.bic > minBic and obj.bic < secondMinBic):
                         secondMinBic = obj.bic
                         secondBest = obj
                 except:
                     raise Exception("Failed to run for k_denovo:{k}!")
                 
+                # scores_k["K_"+str(k)] = {"bic":obj.bic, "llik":obj.likelihood}
+                scores_k["K_"+str(k)] = obj.runs_scores
+                
                 progress.console.print(f"Running on k_denovo={k} | BIC={obj.bic}")
                 progress.update(task, advance=1)
 
             if bestRun is not None:
-                bestRun._convert_to_dataframe(x, beta_fixed)
+                bestRun.convert_to_dataframe(x, beta_fixed)
             
             if secondBest is not None:
-                secondBest._convert_to_dataframe(x, beta_fixed)
+                secondBest.convert_to_dataframe(x, beta_fixed)
             
         from uniplot import plot
         console.print('\n-------------------------------------------------------\n\n[bold red]Best Model:')
         console.print(f"k_denovo: {bestRun.k_denovo}\nBIC: {bestRun.bic}\nStopped at {len(bestRun.losses)}th step\n")
         plot(
             [bestRun.losses, bestRun.likelihoods], 
             title="Loss & Log-Likelihood vs SVI steps", 
@@ -121,38 +153,45 @@
 
     else:
     # Non-verbose run
 
         minBic = maxsize
         secondMinBic = maxsize
         bestRun, secondBest = None, None
+
+        scores_k = dict()
         for k in k_list:
             kwargs["k_denovo"] = k
 
             try:
-                obj = single_run(kwargs)
+                obj = single_run(seed_list=seed, save_runs_seed=save_runs_seed, kwargs=kwargs)
 
                 if obj.bic < minBic:
                     minBic = obj.bic
                     bestRun = obj
                     if k == k_list[0] and len(k_list)>1:
                         secondMinBic = obj.bic
                         secondBest = obj
 
                 if obj.bic > minBic and obj.bic < secondMinBic and len(k_list)>1:
                     secondMinBic = obj.bic
                     secondBest = obj
             except:
                 raise Exception("Failed to run for k_denovo:{k}!")
 
+            # scores_k["K_"+str(k)] = {"bic":obj.bic, "llik":obj.likelihood}
+            scores_k["K_"+str(k)] = obj.runs_scores
+
         if bestRun is not None:
-            bestRun._convert_to_dataframe(x, beta_fixed)
+            bestRun.convert_to_dataframe(x, beta_fixed)
         
         if secondBest is not None:
-            secondBest._convert_to_dataframe(x, beta_fixed)
+            secondBest.convert_to_dataframe(x, beta_fixed)
+
+    bestRun.scores_K = scores_k
 
     return bestRun, secondBest
 
 
 
 '''
 #import utilities
```

### Comparing `pybasilica-0.1.4/pybasilica/simulation.py` & `pybasilica-0.1.5/pybasilica/simulation.py`

 * *Files identical despite different names*

### Comparing `pybasilica-0.1.4/pybasilica/svi.py` & `pybasilica-0.1.5/pybasilica/svi.py`

 * *Files 10% similar despite different names*

```diff
@@ -4,15 +4,17 @@
 import pyro
 from pyro.infer import SVI,Trace_ELBO, JitTrace_ELBO, TraceEnum_ELBO
 from pyro.ops.indexing import Vindex
 from pyro.optim import Adam
 import pyro.distributions.constraints as constraints
 import pyro.distributions as dist
 import torch.nn.functional as F
+
 from tqdm import trange
+from logging import warning
 
 import numpy as np
 import pandas as pd
 from statsmodels.tsa.stattools import adfuller
 from statsmodels.tsa.stattools import kpss
 
 
@@ -20,72 +22,90 @@
 
     def __init__(
         self,
         x,
         k_denovo,
         lr,
         n_steps,
-        enumer=False, # if True, will enumerate the Z
-        cluster=None,
-        alpha_var=1,
-        exp_rate=3,
-        groups=None,
-        beta_fixed=None,
+        enumer = False, # if True, will enumerate the Z
+        cluster = None,
+        hyperparameters = {"alpha_var":1, "alpha_prior_var":1, "exp_rate":10, "beta_var":1, "eps_var":10},
+        groups = None,
+        beta_fixed = None,
         compile_model = True,
         CUDA = False,
         enforce_sparsity = False,
         store_parameters = False,
         regularizer = "cosine",
-        reg_weight = 1,
-        reg_bic = False, 
+        reg_weight = 1.,
+        reg_bic = True, 
         stage = "random_noise", 
         regul_compare = None,
-        seed = 10
+        seed = 10,
+        initializ_seed = True,
+        initializ_pars_fit = False
         ):
 
+        self._hyperpars_default = {"alpha_var":1, "alpha_prior_var":1, "exp_rate":10, "beta_var":1, "eps_var":10}
+
         self._set_data_catalogue(x)
+        self._set_fit_settings(enforce_sparsity, lr, n_steps, compile_model, CUDA, regularizer, reg_weight, reg_bic, \
+                               store_parameters, stage, initializ_seed, initializ_pars_fit, seed)
+
         self._set_beta_fixed(beta_fixed)
         self._set_k_denovo(k_denovo)
 
-        self._set_hyperparams(enumer, cluster, alpha_var, exp_rate, groups)
-        self._set_fit_settings(enforce_sparsity, lr, n_steps, compile_model, CUDA, regularizer, reg_weight, reg_bic, store_parameters, stage)
+        self._set_hyperparams(enumer, cluster, groups, hyperparameters)
 
         self._fix_zero_denovo_null_reference()
         self._set_external_catalogue(regul_compare)
 
-        self.seed = seed
-
 
     def _set_fit_settings(self, enforce_sparsity, lr, n_steps, compile_model, CUDA, \
-                          regularizer, reg_weight, reg_bic, store_parameters, stage):
+                          regularizer, reg_weight, reg_bic, store_parameters, stage,
+                          initializ_seed, initializ_pars_fit, seed):
         self.enforce_sparsity = enforce_sparsity
         self.lr = lr
         self.n_steps = int(n_steps)
         self.compile_model = compile_model
         self.CUDA = CUDA
         self.regularizer = regularizer
         self.reg_weight = reg_weight
         self.reg_bic = reg_bic
 
         self.store_parameters = store_parameters
         self.stage = stage
 
+        self.initializ_seed = initializ_seed
+
+        self._initializ_params_with_fit = initializ_pars_fit
+        self.seed = seed
+
+        if self.initializ_seed is True and self._initializ_params_with_fit is True:
+            warning("\n\t`initializ_seed` and `initializ_pars_fit` can't be both `True`.\n\tSetting the initialization of the seed to `False` and running with seed " +
+                    str(seed))
+            self.initializ_seed = False
+
 
-    def _set_hyperparams(self, enumer, cluster, alpha_var, exp_rate, groups):
+    def _set_hyperparams(self, enumer, cluster, groups, hyperparameters):
         self.enumer = enumer
         self.cluster = cluster
-        self.alpha_var = alpha_var
-        self.exp_rate = exp_rate
-
         self._set_groups(groups)
 
         self.init_params = None
 
+        if hyperparameters is None:
+            self.hyperparameters = self._hyperpars_default
+        else:
+            self.hyperparameters = dict()
+            for parname in self._hyperpars_default.keys():
+                self.hyperparameters[parname] = hyperparameters.get(parname, self._hyperpars_default[parname])
+
         if not enumer and cluster != None:
-            self.z_prior = torch.multinomial(torch.ones(cluster), self.n_samples, replacement=True).float()
+            self.hyperparameters["z_prior"] = torch.multinomial(torch.ones(cluster), self.n_samples, replacement=True).float()
 
 
     def _fix_zero_denovo_null_reference(self):
         if self.k_denovo == 0 and self.k_fixed == 0:
             self.stage = "random_noise"
             self.beta_fixed = torch.zeros(1, self.contexts, dtype=torch.float64)
             self.k_fixed = 1
@@ -106,78 +126,67 @@
     def _set_beta_fixed(self, beta_fixed):
         try:
             self.beta_fixed = torch.tensor(beta_fixed.values, dtype=torch.float64)
             if len(self.beta_fixed.shape)==1:
                 self.beta_fixed = self.beta_fixed.reshape(1, self.beta_fixed.shape[0])
 
             self.k_fixed = beta_fixed.shape[0]
+
         except:
             if beta_fixed is None:
                 self.beta_fixed = None
                 self.k_fixed = 0
             else:
                 raise Exception("Invalid fixed signatures catalogue, expected DataFrame!")
-        
+
         if self.k_fixed > 0:
             self._fix_zero_contexts()
 
 
     def _fix_zero_contexts(self):
         colsums = torch.sum(self.beta_fixed, axis=0)
         zero_contexts = torch.where(colsums==0)[0]
         if torch.any(colsums == 0):
-            # self.stage = "random_noise"
             random_sig = [0] if self.k_fixed == 1 else torch.randperm(self.beta_fixed.shape[0])[:torch.numel(zero_contexts)]
 
             for rr in random_sig:
                 self.beta_fixed[rr, zero_contexts] = 1e-07
 
             self.beta_fixed = self.beta_fixed / (torch.sum(self.beta_fixed, 1).unsqueeze(-1))
 
 
     def _set_external_catalogue(self, regul_compare):
         try:
             self.regul_compare = torch.tensor(regul_compare.values, dtype=torch.float64)
+            if self.CUDA and torch.cuda.is_available():
+                self.regul_compare = self.regul_compare.cuda()
         except:
             if regul_compare is None:
                 self.regul_compare = None
             else:
                 raise Exception("Invalid external signatures catalogue, expected DataFrame!")
 
 
-        if self.k_fixed > 0:
-            self._fix_zero_contexts()
-
-
-    # def _fix_zero_contexts(self):
-    #     colsums = torch.sum(self.beta_fixed, axis=0)
-    #     zero_contexts = torch.where(colsums==0)[0]
-    #     if torch.any(colsums == 0):
-    #         # self.stage = "random_noise"
-    #         random_sig = 0 if self.k_fixed == 1 else torch.randperm(self.beta_fixed.shape[0])[:torch.numel(zero_contexts)]
-
-    #         for rr in random_sig:
-    #             self.beta_fixed[rr, zero_contexts] = 1e-07
-
-    #         self.beta_fixed = self.beta_fixed / (torch.sum(self.beta_fixed, 1).unsqueeze(-1))
-
-
     def _set_k_denovo(self, k_denovo):
         if isinstance(k_denovo, int):
             self.k_denovo = k_denovo
         else:
             raise Exception("Invalid k_denovo value, expected integer!")
 
 
     def _set_groups(self, groups):
         if groups is None:
             self.groups = None
+            self.n_groups = None
         else:
             if isinstance(groups, list) and len(groups)==self.n_samples:
-                self.groups = groups
+                self.groups = torch.tensor(groups).long()
+                # n_groups = len(set(groups)) # WRONG!!!!! not working since groups is a tensor
+                self.n_groups = torch.tensor(groups).unique().numel()
+
             else:
                 raise Exception("invalid groups argument, expected 'None' or a list with {} elements!".format(self.n_samples))
 
 
     def _check_args(self):
         pass
         # if self.k_denovo==0 and self.k_fixed==0:
@@ -191,183 +200,148 @@
 
         n_samples = self.n_samples
         k_fixed = self.k_fixed
         k_denovo = self.k_denovo
         groups = self.groups
         cluster = self.cluster  # number of clusters or None
         enumer = self.enumer
+        n_groups = self.n_groups
 
-        alpha_var = self.alpha_var
-        exp_rate = self.exp_rate
+        alpha_var = self.hyperparameters["alpha_var"]
+        alpha_prior_var = self.hyperparameters["alpha_prior_var"]
+        exp_rate = self.hyperparameters["exp_rate"]
+        beta_var = self.hyperparameters["beta_var"]
+        eps_var = self.hyperparameters["eps_var"]
 
         # Alpha
-        if cluster != None:
-            pi = pyro.sample("pi", dist.Dirichlet(torch.ones(cluster) / cluster))
-            with pyro.plate("k1", k_fixed+k_denovo):
-                with pyro.plate("g", cluster):
-                    alpha_tissues = pyro.sample("alpha_t", dist.HalfNormal(alpha_var))
-
-            with pyro.plate("n",n_samples):
-                if enumer != False:
-                    z = pyro.sample("latent_class", dist.Categorical(pi), infer={"enumerate":enumer})
-                else:
-                    z = pyro.sample("latent_class", dist.Categorical(pi)).long()
-                alpha = pyro.sample("latent_exposure", dist.MultivariateNormal(alpha_tissues[z], torch.eye(k_fixed+k_denovo) * torch.tensor(alpha_var)))
-
-        elif groups != None:
-
-            n_groups = len(set(groups))
+        if groups is not None:
             if self._noise_only:
                 alpha = torch.zeros(n_samples, 1, dtype=torch.float64)
             else:
                 with pyro.plate("k1", k_fixed+k_denovo):
                     with pyro.plate("g", n_groups):
-                        alpha_tissues = pyro.sample("alpha_t", dist.HalfNormal(alpha_var))
+                        # G x K matrix
+                        alpha_prior = pyro.sample("alpha_t", dist.HalfNormal(alpha_prior_var))
 
                 # sample from the alpha prior
-                with pyro.plate("k", k_fixed + k_denovo):   # columns
-                    with pyro.plate("n", n_samples):        # rows
-                        alpha = pyro.sample("latent_exposure", dist.Normal(alpha_tissues[groups,:], alpha_var))
+                with pyro.plate("k", k_fixed + k_denovo):  # columns
+                    with pyro.plate("n", n_samples):  # rows
+                        alpha = pyro.sample("latent_exposure", dist.Normal(alpha_prior[groups,:], alpha_var))
+
+                alpha = alpha / (torch.sum(alpha, 1).unsqueeze(-1))
+                alpha = torch.clamp(alpha, 0, 1)
+
+        elif cluster is not None:
+            pi = pyro.sample("pi", dist.Dirichlet(torch.ones(cluster) / cluster))
+            with pyro.plate("k1", k_fixed + k_denovo):
+                with pyro.plate("g", cluster):
+                    # G x K matrix
+                    alpha_prior = pyro.sample("alpha_t", dist.HalfNormal(alpha_prior_var))
 
         else:
             if self._noise_only:
                 alpha = torch.zeros(n_samples, 1, dtype=torch.float64)
             else:
-                with pyro.plate("k", k_fixed + k_denovo):   # columns
-                    with pyro.plate("n", n_samples):        # rows
+                with pyro.plate("k", k_fixed + k_denovo):  # columns
+                    with pyro.plate("n", n_samples):  # rows
                         if self.enforce_sparsity:
                             alpha = pyro.sample("latent_exposure", dist.Exponential(exp_rate))
                         else:
                             alpha = pyro.sample("latent_exposure", dist.HalfNormal(alpha_var))
 
                 alpha = alpha / (torch.sum(alpha, 1).unsqueeze(-1))
                 alpha = torch.clamp(alpha, 0, 1)
 
-        '''
-        if self.stage=="two":
-            dd = torch.tensor(self.alpha0.values).float()
-            cc = torch.sum(dd, 1).unsqueeze(-1)
-            alpha = alpha * ((torch.ones(alpha.shape[0]) - self.alpha0.sum) / self.alpha0.sum)
-        '''
-
         # Epsilon
         if self.stage == "random_noise":
-            eps_var = 10
             with pyro.plate("contexts3", self.contexts):  # columns
-                    with pyro.plate("n3", n_samples):     # rows
+                    with pyro.plate("n3", n_samples):  # rows
                         epsilon = pyro.sample("latent_m", dist.HalfNormal(eps_var))
         else:
             epsilon = None
 
         # Beta
         if k_denovo == 0:
             beta_denovo = None
         else:
             with pyro.plate("contexts", self.contexts):  # columns
                 with pyro.plate("k_denovo", k_denovo):  # rows
-                    beta_denovo = pyro.sample("latent_signatures", dist.HalfNormal(1))
-            
-            beta_denovo = beta_denovo / (torch.sum(beta_denovo, 1).unsqueeze(-1))   # normalize
+                    beta_denovo = pyro.sample("latent_signatures", dist.HalfNormal(beta_var))
+
+            beta_denovo = beta_denovo / (torch.sum(beta_denovo, 1).unsqueeze(-1))  # normalize
             beta_denovo = torch.clamp(beta_denovo, 0, 1)
 
         beta = self._get_unique_beta(self.beta_fixed, beta_denovo)
         reg = self._regularizer(self.beta_fixed, beta_denovo, self.regularizer)
         self.reg = reg
 
         # Observations
-        with pyro.plate("contexts2", self.contexts):
-            with pyro.plate("n2", n_samples):
-                ## TODO might try to insert the alpha here
-
-                a = torch.matmul(torch.matmul(torch.diag(torch.sum(self.x, axis=1)), alpha), beta)
-                
-                if self.stage == "random_noise":
-                    xx = a + epsilon
-                    lk =  dist.Poisson(xx).log_prob(self.x)
-                else:
-                    lk =  dist.Poisson(a).log_prob(self.x)
-                # pyro.factor("loss", lk + self.reg_weight * (reg * self.x.shape[0] * self.x.shape[1]))
-                pyro.factor("loss", lk.sum() + self.reg_weight * (reg * self.x.shape[0] * self.x.shape[1]))
-
-
-    def _initialize_params(self):
-        if self.init_params is None:
-            params = dict()
-            
-            if self.cluster is not None:
-                params["pi_param"] = torch.ones(self.cluster)
-                params["alpha_t_param"] = dist.HalfNormal(torch.ones(self.cluster, self.k_fixed + self.k_denovo, dtype=torch.float6) * \
-                                                        torch.tensor(self.alpha_var)).sample()
-            elif self.groups is not None:
-                params["alpha_t_param"] = dist.HalfNormal(torch.ones(len(set(self.groups)), self.k_fixed + self.k_denovo, dtype=torch.float64) * \
-                                                        torch.tensor(self.alpha_var)).sample()
+        with pyro.plate("n2", n_samples):
+            if cluster is not None:
+                z = pyro.sample("latent_class", dist.Categorical(pi), infer={"enumerate":enumer})
+                alpha = pyro.sample("latent_exposure", dist.Normal(alpha_prior[z], alpha_var).expand([1, k_fixed+k_denovo]))
+
+            a = torch.matmul(torch.matmul(torch.diag(torch.sum(self.x, axis=1)), alpha), beta)
+
+            if self.stage == "random_noise":
+                xx = a + epsilon
+                lk =  dist.Poisson(xx).log_prob(self.x)
             else:
-                if self.enforce_sparsity:
-                    params["alpha_mean"] = dist.Exponential(torch.ones(self.n_samples, self.k_fixed + self.k_denovo, dtype=torch.float64) * self.exp_rate).sample()
-                else:
-                    params["alpha_mean"] = dist.HalfNormal(torch.ones(self.n_samples, self.k_fixed + self.k_denovo, dtype=torch.float64) * self.alpha_var).sample()
-
-            params["epsilon_var"] = torch.ones(self.n_samples, self.contexts, dtype=torch.float64)
-
-            if self.k_denovo > 0:
-                params["beta_dn_param"] = dist.HalfNormal(torch.ones(self.k_denovo, self.contexts, dtype=torch.float64)).sample()
-
-            self.init_params = params
-
-        return self.init_params
+                lk =  dist.Poisson(a).log_prob(self.x)
+            # pyro.factor("loss", lk + self.reg_weight * (reg * self.x.shape[0] * self.x.shape[1]))
+            pyro.factor("loss", lk.sum() + self.reg_weight * (reg * self.x.shape[0] * self.x.shape[1]))
 
 
     def guide(self):
 
         n_samples = self.n_samples
         k_fixed = self.k_fixed
         k_denovo = self.k_denovo
         groups = self.groups
         cluster = self.cluster
         enumer = self.enumer
+        n_groups = self.n_groups
 
         init_params = self._initialize_params()
 
         # Alpha
-        if cluster is not None:
-            pi_param = pyro.param("pi_param", init_params["pi_param"], constraint=constraints.simplex)
-            pi = pyro.sample("pi", dist.Delta(pi_param).to_event(1))
+        if groups is not None:
+            if not self._noise_only:
+                alpha_prior = pyro.param("alpha_t_param", init_params["alpha_t_param"], constraint=constraints.greater_than_eq(0))
 
-            alpha_tissues = pyro.param("alpha_t_param", init_params["alpha_t_param"], constraint=constraints.greater_than_eq(0))
+                with pyro.plate("k1", k_fixed+k_denovo):
+                    with pyro.plate("g", n_groups):
+                        pyro.sample("alpha_t", dist.Delta(alpha_prior))
 
-            with pyro.plate("k1", k_fixed+k_denovo):
-                with pyro.plate("g", cluster):
-                    pyro.sample("alpha_t", dist.Delta(alpha_tissues))
+                with pyro.plate("k", k_fixed + k_denovo):  # columns
+                    with pyro.plate("n", n_samples):  # rows
+                        alpha = pyro.param("alpha", alpha_prior[groups, :], constraint=constraints.greater_than_eq(0))
+                        pyro.sample("latent_exposure", dist.Delta(alpha))
 
-            if enumer == False:
-                z_par = pyro.param("latent_class_p", lambda: self.z_prior)
+        elif cluster is not None:
+            if not self._noise_only:
+                pi_param = pyro.param("pi_param", init_params["pi_param"], constraint=constraints.simplex)
+                pi = pyro.sample("pi", dist.Delta(pi_param).to_event(1))
 
-            with pyro.plate("n", n_samples):  # + (n_samples) BATCH
-                if enumer != False:
-                    z = pyro.sample("latent_class", dist.Categorical(pi), infer={"enumerate":enumer})
-                else:
-                    z = pyro.sample("latent_class", dist.Delta(z_par)).long()
-                    # Delta shape -> batch=(n_samples) + event=()
-                    # adding plate dims -> BATCH : (k_denovo+k_fixed) (n_samples)
-                alpha_p = pyro.param("alpha", lambda: alpha_tissues[z, :], constraint=constraints.greater_than_eq(0))
-                alpha = pyro.sample("latent_exposure", dist.Delta(alpha_p).to_event(1))
+                alpha_prior = pyro.param("alpha_t_param", init_params["alpha_t_param"], constraint=constraints.greater_than_eq(0))
 
-        elif groups != None:
-            if not self._noise_only:
-                n_groups = len(set(groups))
-                alpha_tissues = pyro.param("alpha_t_param", init_params["alpha_t_param"], constraint=constraints.greater_than_eq(0))
+                if enumer == False:
+                    z_par = pyro.param("latent_class_p", lambda: self.hyperparameters["z_prior"])
+                    z = pyro.sample("latent_class", dist.Delta(z_par))
 
                 with pyro.plate("k1", k_fixed+k_denovo):
-                    with pyro.plate("g", n_groups):
-                        pyro.sample("alpha_t", dist.Delta(alpha_tissues))
+                    with pyro.plate("g", cluster):
+                        pyro.sample("alpha_t", dist.Delta(alpha_prior))
 
-                with pyro.plate("k", k_fixed + k_denovo):   # columns
-                    with pyro.plate("n", n_samples):        # rows
-                        alpha = pyro.param("alpha", alpha_tissues[groups, :], constraint=constraints.greater_than_eq(0))
-                        pyro.sample("latent_exposure", dist.Delta(alpha))
+                with pyro.plate("n2", n_samples):
+                    if enumer != False:
+                        z = pyro.sample("latent_class", dist.Categorical(pi), infer={"enumerate":enumer})
+
+                    alpha = pyro.param("alpha", lambda: alpha_prior[z.long()], constraint=constraints.greater_than_eq(0))
+                    pyro.sample("latent_exposure", dist.Delta(alpha).expand([1, k_fixed+k_denovo]))
 
         # No groups
         else:
             if not self._noise_only:
                 alpha_mean = init_params["alpha_mean"]
 
                 with pyro.plate("k", k_fixed + k_denovo):
@@ -382,23 +356,101 @@
         if self.stage == "random_noise":
             eps_var = pyro.param("lambda_epsilon", init_params["epsilon_var"], constraint=constraints.positive)
 
             with pyro.plate("contexts3", self.contexts):
                 with pyro.plate("n3", n_samples):
                     pyro.sample("latent_m", dist.HalfNormal(eps_var))
 
-        # Beta 
+        # Beta
         if k_denovo > 0:
             beta_par = init_params["beta_dn_param"]
             with pyro.plate("contexts", self.contexts):
                 with pyro.plate("k_denovo", k_denovo):
                     beta = pyro.param("beta_denovo", beta_par, constraint=constraints.greater_than_eq(0.0))
                     pyro.sample("latent_signatures", dist.Delta(beta))
 
 
+    def _initialize_params_hier(self):
+        groups_true = torch.tensor(self.groups)
+        steps_true = self.n_steps
+        hyperpars_true = self.hyperparameters
+        
+        self.groups = None
+        self.n_steps = 50
+        self.initializ_seed = False
+        self.hyperparameters = self._hyperpars_default
+
+        params = dict()
+
+        print("Initializing parameters with non-hierarchical fit")
+        self._fit(set_attributes=False)
+
+        if self.cluster is not None:
+            raise NotImplementedError
+
+        alpha = self._get_param("alpha", normalize=True, to_cpu=False)
+        alpha_t_param = torch.zeros((groups_true.unique().numel(), self.k_fixed+self.k_denovo), dtype=torch.float64)
+
+        for gid in groups_true.unique().tolist(): alpha_t_param[gid] = torch.mean(alpha[groups_true == gid, :], dim=0)
+        params["alpha_t_param"] = alpha_t_param
+
+        if self.k_denovo > 0: params["beta_dn_param"] = self._get_param("beta_denovo", to_cpu=False, normalize=True)
+
+        params["epsilon_var"] = torch.ones(self.n_samples, self.contexts, dtype=torch.float64)
+
+        pyro.get_param_store().clear()
+
+        self.groups = groups_true
+        self.n_steps = steps_true
+        self.hyperparameters = hyperpars_true
+
+        return params
+
+
+    def _initialize_params_nonhier(self):
+        params = dict()
+
+        alpha_var = self.hyperparameters["alpha_var"]
+        alpha_prior_var = self.hyperparameters["alpha_prior_var"]
+        exp_rate = self.hyperparameters["exp_rate"]
+        beta_var = self.hyperparameters["beta_var"]
+        eps_var = self.hyperparameters["eps_var"]
+
+        if self.cluster is not None:
+            params["pi_param"] = torch.ones(self.cluster, dtype=torch.float64)
+            params["alpha_t_param"] = dist.HalfNormal(torch.ones(self.cluster, self.k_fixed + self.k_denovo, dtype=torch.float64) * \
+                                                      torch.tensor(alpha_prior_var)).sample()
+        elif self.groups is not None:
+            params["alpha_t_param"] = dist.HalfNormal(torch.ones(self.n_groups, self.k_fixed + self.k_denovo, dtype=torch.float64) * \
+                                                      torch.tensor(alpha_prior_var)).sample()
+        else:
+            if self.enforce_sparsity:
+                params["alpha_mean"] = dist.Exponential(torch.ones(self.n_samples, self.k_fixed + self.k_denovo, dtype=torch.float64) * exp_rate).sample()
+            else:
+                params["alpha_mean"] = dist.HalfNormal(torch.ones(self.n_samples, self.k_fixed + self.k_denovo, dtype=torch.float64) * alpha_var).sample()
+
+        params["epsilon_var"] = torch.ones(self.n_samples, self.contexts, dtype=torch.float64) * eps_var
+
+        if self.k_denovo > 0:
+            params["beta_dn_param"] = dist.HalfNormal(torch.ones(self.k_denovo, self.contexts, dtype=torch.float64) * beta_var).sample()
+
+        return params
+
+
+    def _initialize_params(self):
+        if self.init_params is None:
+
+            if self.groups is not None and self._initializ_params_with_fit:
+                self.init_params = self._initialize_params_hier()
+            else:
+                self.init_params = self._initialize_params_nonhier()
+
+        return self.init_params
+
+
     def _regularizer(self, beta_fixed, beta_denovo, reg_type = "cosine"):
         '''
         if beta_denovo == None:
             dd = 0
         else:
             dd = 0
             c1 = 0
@@ -443,15 +495,19 @@
         
         return torch.cat((beta_fixed, beta_denovo), axis=0)
 
 
     def _likelihood(self, M, alpha, beta_fixed, beta_denovo, eps_var=None):
         beta = self._get_unique_beta(beta_fixed, beta_denovo)
 
-        a = torch.matmul(torch.matmul(torch.diag(torch.sum(M, axis=1)), alpha), beta)
+        ssum = torch.sum(M, axis=1)
+        ddiag = torch.diag(ssum)
+        mmult1 = torch.matmul(ddiag, alpha)
+
+        a = torch.matmul(mmult1, beta)
 
         if eps_var == None:
             _log_like_matrix = dist.Poisson(a).log_prob(M)
         else:
             xx = a + dist.HalfNormal(eps_var).sample()
             _log_like_matrix = dist.Poisson(xx).log_prob(M)
 
@@ -471,21 +527,24 @@
         svi = SVI(self.model, self.guide, optim, elbo)
         loss = svi.step()
         self.init_params = None
 
         return np.round(loss, 3), seed
 
 
-    def _fit(self):
+    def _fit(self, set_attributes=True):
         pyro.clear_param_store()  # always clear the store before the inference
+
         if self.CUDA and torch.cuda.is_available():
             torch.set_default_tensor_type('torch.cuda.FloatTensor')
             self.x = self.x.cuda()
             if self.beta_fixed is not None:
                 self.beta_fixed = self.beta_fixed.cuda()
+            if self.regul_compare is not None:
+                self.regul_compare = self.regul_compare.cuda()
         else:
             torch.set_default_tensor_type(t=torch.FloatTensor)
 
         if self.cluster != None and self.enumer != False:
             elbo = TraceEnum_ELBO()
         elif self.compile_model and not self.CUDA:
             elbo = JitTrace_ELBO()
@@ -495,45 +554,56 @@
         min_steps = 50
 
         train_params = []
         # learning global parameters
         adam_params = {"lr": self.lr}
         optimizer = Adam(adam_params)
 
-        _, self.seed = min([self._initialize_seed(optimizer, elbo, seed) for seed in range(50)], key = lambda x: x[0])
+        if self.initializ_seed:
+            _, self.seed = min([self._initialize_seed(optimizer, elbo, seed) for seed in range(50)], key = lambda x: x[0])
+
+        print("Running with seed {}\n".format(self.seed))
         pyro.set_rng_seed(self.seed)
         pyro.get_param_store().clear()
 
+        self._initialize_params()
+
         svi = SVI(self.model, self.guide, optimizer, loss=elbo)
 
         losses = []
         regs = []
         likelihoods = []
         for _ in range(self.n_steps):   # inference - do gradient steps
+
             loss = svi.step()
             losses.append(loss)
             regs.append(self.reg)
 
             # create likelihoods 
             alpha = self._get_param("alpha", normalize=True, to_cpu=False)
             eps_var = self._get_param("eps_var", normalize=False, to_cpu=False)
             beta_denovo = self._get_param("beta_denovo", normalize=True, to_cpu=False)
             likelihoods.append(self._likelihood(self.x, alpha, self.beta_fixed, beta_denovo, eps_var))
 
+            if self.store_parameters:
+                train_params.append(self.get_param_dict())
+
             # convergence test 
             if len(losses) >= min_steps and len(losses) % min_steps == 0 and convergence(x=losses[-min_steps:], alpha=0.05):
                 break
 
-            if self.store_parameters:
-                train_params.append(self.get_param_dict())
+        if set_attributes is False:
+            return
 
         if self.CUDA and torch.cuda.is_available():
           self.x = self.x.cpu()
           if self.beta_fixed is not None:
             self.beta_fixed = self.beta_fixed.cpu()
+          if self.regul_compare is not None:
+                self.regul_compare = self.regul_compare.cpu()
 
         self.train_params = train_params
         self.losses = losses
         self.likelihoods = likelihoods
         self.regs = regs
         self._set_params()
         self._set_bic()
@@ -542,18 +612,22 @@
 
     def _set_params(self):
         self._set_alpha()
         self._set_beta_denovo()
         self._set_epsilon()
         self._set_clusters()
 
+        if isinstance(self.groups, torch.Tensor):
+            self.groups = self.groups.tolist()
+
 
     def _get_param(self, param_name, normalize=False, to_cpu=True):
         try:
-            par = pyro.param(param_name)
+            if param_name == "beta_fixed": par = self.beta_fixed
+            else: par = pyro.param(param_name)
 
             if to_cpu and self.CUDA and torch.cuda.is_available(): par = par.cpu()
 
             try:
                 par = par.clone().detach()
             finally:
                 if normalize:
@@ -620,15 +694,15 @@
 
     def get_param_dict(self):
         params = dict()
         params["alpha"] = self._get_param("alpha", normalize=True)
         params["alpha_prior"] = self._get_param("alpha_t_param", normalize=True)
 
         params["beta_d"] =  self._get_param("beta_denovo", normalize=True)
-        params["beta_f"] = self.beta_fixed
+        params["beta_f"] = self._get_param("beta_fixed")
 
         params["pi"] = self._get_param("pi", normalize=False)
 
         if self.stage=="random_noise":
             params["lambda_epsilon"] = self._get_param("lambda_epsilon", normalize=False)
         else:
             params["lambda_epsilon"] = None
@@ -670,45 +744,47 @@
             best_cl = torch.argmax(probs)
             z[n] = best_cl
 
         return z
 
 
     def _set_bic(self):
-
         M = self.x
         alpha = self.alpha
 
         _log_like = self._likelihood(M, alpha, self.beta_fixed, self.beta_denovo, self.eps_var)
 
         # adding regularizer
-        if self.reg_bic:
+        if self.reg_weight != 0 and self.reg_bic:
             reg = self._regularizer(self.beta_fixed, self.beta_denovo, reg_type = self.regularizer)
             _log_like += self.reg_weight * (reg * self.x.shape[0] * self.x.shape[1])
-        
-        k = self._number_of_params()
+
+        k = self._number_of_params() 
         n = M.shape[0] * M.shape[1]
         bic = k * torch.log(torch.tensor(n, dtype=torch.float64)) - (2 * _log_like)
 
         self.bic = bic.item()
 
-    
+
     def _number_of_params(self):
         if self.k_denovo == 0 and torch.sum(self.beta_fixed) == 0:
             k = 0
         else:
             k = (self.n_samples * (self.k_denovo + self.k_fixed)) + ((self.k_denovo) * self.contexts)
         
         if self.eps_var is not None:
             k = k + self.eps_var.shape[0] * self.eps_var.shape[1]
         
         return k
 
 
-    def _convert_to_dataframe(self, x, beta_fixed):
+    def convert_to_dataframe(self, x, beta_fixed):
+
+        if isinstance(self.beta_fixed, pd.DataFrame):
+            self.beta_fixed = torch.tensor(self.beta_fixed.values, dtype=torch.float64)
 
         # mutations catalogue
         self.x = x
         sample_names = list(x.index)
         mutation_features = list(x.columns)
 
         # fixed signatures
```

### Comparing `pybasilica-0.1.4/pybasilica/utilities.py` & `pybasilica-0.1.5/pybasilica/utilities.py`

 * *Files identical despite different names*

### Comparing `pybasilica-0.1.4/setup.py` & `pybasilica-0.1.5/setup.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from setuptools import setup
 
 with open("README.md", "r", encoding="utf-8") as fh:
     long_description = fh.read()
 
 setup(
     name = "pybasilica",
-    version = "0.1.4",
+    version = "0.1.5",
     author = "Azad Sadr",
     author_email = "azad.sadr.h@gmail.com",
     description = "A bayesian model to extract mutational signatures",
     long_description = long_description,
     long_description_content_type = "text/markdown",
     url = "https://github.com/caravagnalab/pybasilica",
     packages = ["pybasilica"],
```

