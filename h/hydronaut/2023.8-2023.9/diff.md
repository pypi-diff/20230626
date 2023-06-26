# Comparing `tmp/hydronaut-2023.8.tar.gz` & `tmp/hydronaut-2023.9.tar.gz`

## Comparing `hydronaut-2023.8.tar` & `hydronaut-2023.9.tar`

### file list

```diff
@@ -1,50 +1,50 @@
--rw-r--r--   0        0        0      238 2020-02-02 00:00:00.000000 hydronaut-2023.8/.gitlab-ci.yml
--rw-r--r--   0        0        0      110 2020-02-02 00:00:00.000000 hydronaut-2023.8/.gitmodules
--rw-r--r--   0        0        0     1374 2020-02-02 00:00:00.000000 hydronaut-2023.8/TODO.md
--rw-r--r--   0        0        0      345 2020-02-02 00:00:00.000000 hydronaut-2023.8/env.sh
--rw-r--r--   0        0        0      638 2020-02-02 00:00:00.000000 hydronaut-2023.8/doc/Makefile
--rw-r--r--   0        0        0      804 2020-02-02 00:00:00.000000 hydronaut-2023.8/doc/make.bat
--rw-r--r--   0        0        0       36 2020-02-02 00:00:00.000000 hydronaut-2023.8/doc/requirements.txt
--rw-r--r--   0        0        0     1179 2020-02-02 00:00:00.000000 hydronaut-2023.8/doc/source/conf.py
--rw-r--r--   0        0        0      823 2020-02-02 00:00:00.000000 hydronaut-2023.8/doc/source/hydronaut.hydra.rst
--rw-r--r--   0        0        0     1460 2020-02-02 00:00:00.000000 hydronaut-2023.8/doc/source/hydronaut.rst
--rw-r--r--   0        0        0      307 2020-02-02 00:00:00.000000 hydronaut-2023.8/doc/source/index.rst
--rw-r--r--   0        0        0       80 2020-02-02 00:00:00.000000 hydronaut-2023.8/doc/source/modules.rst
--rw-r--r--   0        0        0       33 2020-02-02 00:00:00.000000 hydronaut-2023.8/doc/source/readme.md
--rw-r--r--   0        0        0      413 2020-02-02 00:00:00.000000 hydronaut-2023.8/examples/dummy/README.md
--rw-r--r--   0        0        0     1125 2020-02-02 00:00:00.000000 hydronaut-2023.8/examples/dummy/conf/config.yaml
--rw-r--r--   0        0        0      693 2020-02-02 00:00:00.000000 hydronaut-2023.8/examples/dummy/src/experiment.py
--rw-r--r--   0        0        0     2606 2020-02-02 00:00:00.000000 hydronaut-2023.8/examples/pytorch_lightning-mnist/README.md
--rw-r--r--   0        0        0       36 2020-02-02 00:00:00.000000 hydronaut-2023.8/examples/pytorch_lightning-mnist/requirements.txt
--rw-r--r--   0        0        0     3344 2020-02-02 00:00:00.000000 hydronaut-2023.8/examples/pytorch_lightning-mnist/conf/config.yaml
--rw-r--r--   0        0        0     2208 2020-02-02 00:00:00.000000 hydronaut-2023.8/examples/pytorch_lightning-mnist/src/data.py
--rw-r--r--   0        0        0      904 2020-02-02 00:00:00.000000 hydronaut-2023.8/examples/pytorch_lightning-mnist/src/experiment.py
--rw-r--r--   0        0        0     5190 2020-02-02 00:00:00.000000 hydronaut-2023.8/examples/pytorch_lightning-mnist/src/model.py
--rw-r--r--   0        0        0     2344 2020-02-02 00:00:00.000000 hydronaut-2023.8/img/hydronaut_icon.svg
--rw-r--r--   0        0        0     6881 2020-02-02 00:00:00.000000 hydronaut-2023.8/img/hydronaut_logo.svg
--rwxr-xr-x   0        0        0      135 2020-02-02 00:00:00.000000 hydronaut-2023.8/scripts/hydronaut-initialize.sh
--rwxr-xr-x   0        0        0      256 2020-02-02 00:00:00.000000 hydronaut-2023.8/scripts/hydronaut-install_in_venv.sh
--rwxr-xr-x   0        0        0      232 2020-02-02 00:00:00.000000 hydronaut-2023.8/scripts/hydronaut-lint.sh
--rwxr-xr-x   0        0        0     1416 2020-02-02 00:00:00.000000 hydronaut-2023.8/scripts/hydronaut-rsync-results.sh
--rwxr-xr-x   0        0        0     2544 2020-02-02 00:00:00.000000 hydronaut-2023.8/scripts/hydronaut-run_in_venv.sh
--rw-r--r--   0        0        0       42 2020-02-02 00:00:00.000000 hydronaut-2023.8/src/hydronaut/__init__.py
--rw-r--r--   0        0        0     7994 2020-02-02 00:00:00.000000 hydronaut-2023.8/src/hydronaut/experiment.py
--rw-r--r--   0        0        0     2626 2020-02-02 00:00:00.000000 hydronaut-2023.8/src/hydronaut/file.py
--rw-r--r--   0        0        0     9661 2020-02-02 00:00:00.000000 hydronaut-2023.8/src/hydronaut/init.py
--rw-r--r--   0        0        0      389 2020-02-02 00:00:00.000000 hydronaut-2023.8/src/hydronaut/log.py
--rw-r--r--   0        0        0     4059 2020-02-02 00:00:00.000000 hydronaut-2023.8/src/hydronaut/mlflow.py
--rw-r--r--   0        0        0     2574 2020-02-02 00:00:00.000000 hydronaut-2023.8/src/hydronaut/paths.py
--rw-r--r--   0        0        0     6191 2020-02-02 00:00:00.000000 hydronaut-2023.8/src/hydronaut/run.py
--rw-r--r--   0        0        0      418 2020-02-02 00:00:00.000000 hydronaut-2023.8/src/hydronaut/types.py
--rw-r--r--   0        0        0      273 2020-02-02 00:00:00.000000 hydronaut-2023.8/src/hydronaut/version.py
--rw-r--r--   0        0        0       42 2020-02-02 00:00:00.000000 hydronaut-2023.8/src/hydronaut/hydra/__init__.py
--rw-r--r--   0        0        0     7894 2020-02-02 00:00:00.000000 hydronaut-2023.8/src/hydronaut/hydra/config.py
--rw-r--r--   0        0        0      343 2020-02-02 00:00:00.000000 hydronaut-2023.8/src/hydronaut/hydra/info.py
--rw-r--r--   0        0        0     1670 2020-02-02 00:00:00.000000 hydronaut-2023.8/src/hydronaut/hydra/omegaconf.py
--rw-r--r--   0        0        0     2961 2020-02-02 00:00:00.000000 hydronaut-2023.8/src/hydronaut/hydra/resolvers.py
--rw-r--r--   0        0        0     3188 2020-02-02 00:00:00.000000 hydronaut-2023.8/src/hydronaut/torch/lightning/experiment.py
--rw-r--r--   0        0        0      120 2020-02-02 00:00:00.000000 hydronaut-2023.8/.gitignore
--rw-r--r--   0        0        0     1063 2020-02-02 00:00:00.000000 hydronaut-2023.8/LICENSE.txt
--rw-r--r--   0        0        0    21613 2020-02-02 00:00:00.000000 hydronaut-2023.8/README.md
--rw-r--r--   0        0        0     1714 2020-02-02 00:00:00.000000 hydronaut-2023.8/pyproject.toml
--rw-r--r--   0        0        0    22441 2020-02-02 00:00:00.000000 hydronaut-2023.8/PKG-INFO
+-rw-r--r--   0        0        0      238 2020-02-02 00:00:00.000000 hydronaut-2023.9/.gitlab-ci.yml
+-rw-r--r--   0        0        0      110 2020-02-02 00:00:00.000000 hydronaut-2023.9/.gitmodules
+-rw-r--r--   0        0        0     1374 2020-02-02 00:00:00.000000 hydronaut-2023.9/TODO.md
+-rw-r--r--   0        0        0      345 2020-02-02 00:00:00.000000 hydronaut-2023.9/env.sh
+-rw-r--r--   0        0        0      638 2020-02-02 00:00:00.000000 hydronaut-2023.9/doc/Makefile
+-rw-r--r--   0        0        0      804 2020-02-02 00:00:00.000000 hydronaut-2023.9/doc/make.bat
+-rw-r--r--   0        0        0       36 2020-02-02 00:00:00.000000 hydronaut-2023.9/doc/requirements.txt
+-rw-r--r--   0        0        0     1179 2020-02-02 00:00:00.000000 hydronaut-2023.9/doc/source/conf.py
+-rw-r--r--   0        0        0      823 2020-02-02 00:00:00.000000 hydronaut-2023.9/doc/source/hydronaut.hydra.rst
+-rw-r--r--   0        0        0     1460 2020-02-02 00:00:00.000000 hydronaut-2023.9/doc/source/hydronaut.rst
+-rw-r--r--   0        0        0      307 2020-02-02 00:00:00.000000 hydronaut-2023.9/doc/source/index.rst
+-rw-r--r--   0        0        0       80 2020-02-02 00:00:00.000000 hydronaut-2023.9/doc/source/modules.rst
+-rw-r--r--   0        0        0       33 2020-02-02 00:00:00.000000 hydronaut-2023.9/doc/source/readme.md
+-rw-r--r--   0        0        0      413 2020-02-02 00:00:00.000000 hydronaut-2023.9/examples/dummy/README.md
+-rw-r--r--   0        0        0     1132 2020-02-02 00:00:00.000000 hydronaut-2023.9/examples/dummy/conf/config.yaml
+-rw-r--r--   0        0        0      693 2020-02-02 00:00:00.000000 hydronaut-2023.9/examples/dummy/src/experiment.py
+-rw-r--r--   0        0        0     2606 2020-02-02 00:00:00.000000 hydronaut-2023.9/examples/pytorch_lightning-mnist/README.md
+-rw-r--r--   0        0        0       36 2020-02-02 00:00:00.000000 hydronaut-2023.9/examples/pytorch_lightning-mnist/requirements.txt
+-rw-r--r--   0        0        0     3351 2020-02-02 00:00:00.000000 hydronaut-2023.9/examples/pytorch_lightning-mnist/conf/config.yaml
+-rw-r--r--   0        0        0     2208 2020-02-02 00:00:00.000000 hydronaut-2023.9/examples/pytorch_lightning-mnist/src/data.py
+-rw-r--r--   0        0        0      904 2020-02-02 00:00:00.000000 hydronaut-2023.9/examples/pytorch_lightning-mnist/src/experiment.py
+-rw-r--r--   0        0        0     5190 2020-02-02 00:00:00.000000 hydronaut-2023.9/examples/pytorch_lightning-mnist/src/model.py
+-rw-r--r--   0        0        0     2344 2020-02-02 00:00:00.000000 hydronaut-2023.9/img/hydronaut_icon.svg
+-rw-r--r--   0        0        0     6881 2020-02-02 00:00:00.000000 hydronaut-2023.9/img/hydronaut_logo.svg
+-rwxr-xr-x   0        0        0      135 2020-02-02 00:00:00.000000 hydronaut-2023.9/scripts/hydronaut-initialize.sh
+-rwxr-xr-x   0        0        0      256 2020-02-02 00:00:00.000000 hydronaut-2023.9/scripts/hydronaut-install_in_venv.sh
+-rwxr-xr-x   0        0        0      232 2020-02-02 00:00:00.000000 hydronaut-2023.9/scripts/hydronaut-lint.sh
+-rwxr-xr-x   0        0        0     1416 2020-02-02 00:00:00.000000 hydronaut-2023.9/scripts/hydronaut-rsync-results.sh
+-rwxr-xr-x   0        0        0     2544 2020-02-02 00:00:00.000000 hydronaut-2023.9/scripts/hydronaut-run_in_venv.sh
+-rw-r--r--   0        0        0       42 2020-02-02 00:00:00.000000 hydronaut-2023.9/src/hydronaut/__init__.py
+-rw-r--r--   0        0        0     7994 2020-02-02 00:00:00.000000 hydronaut-2023.9/src/hydronaut/experiment.py
+-rw-r--r--   0        0        0     2626 2020-02-02 00:00:00.000000 hydronaut-2023.9/src/hydronaut/file.py
+-rw-r--r--   0        0        0     9668 2020-02-02 00:00:00.000000 hydronaut-2023.9/src/hydronaut/init.py
+-rw-r--r--   0        0        0      389 2020-02-02 00:00:00.000000 hydronaut-2023.9/src/hydronaut/log.py
+-rw-r--r--   0        0        0     4059 2020-02-02 00:00:00.000000 hydronaut-2023.9/src/hydronaut/mlflow.py
+-rw-r--r--   0        0        0     2574 2020-02-02 00:00:00.000000 hydronaut-2023.9/src/hydronaut/paths.py
+-rw-r--r--   0        0        0     6191 2020-02-02 00:00:00.000000 hydronaut-2023.9/src/hydronaut/run.py
+-rw-r--r--   0        0        0      418 2020-02-02 00:00:00.000000 hydronaut-2023.9/src/hydronaut/types.py
+-rw-r--r--   0        0        0      273 2020-02-02 00:00:00.000000 hydronaut-2023.9/src/hydronaut/version.py
+-rw-r--r--   0        0        0       42 2020-02-02 00:00:00.000000 hydronaut-2023.9/src/hydronaut/hydra/__init__.py
+-rw-r--r--   0        0        0     7915 2020-02-02 00:00:00.000000 hydronaut-2023.9/src/hydronaut/hydra/config.py
+-rw-r--r--   0        0        0      343 2020-02-02 00:00:00.000000 hydronaut-2023.9/src/hydronaut/hydra/info.py
+-rw-r--r--   0        0        0     1670 2020-02-02 00:00:00.000000 hydronaut-2023.9/src/hydronaut/hydra/omegaconf.py
+-rw-r--r--   0        0        0     2961 2020-02-02 00:00:00.000000 hydronaut-2023.9/src/hydronaut/hydra/resolvers.py
+-rw-r--r--   0        0        0     3188 2020-02-02 00:00:00.000000 hydronaut-2023.9/src/hydronaut/torch/lightning/experiment.py
+-rw-r--r--   0        0        0      120 2020-02-02 00:00:00.000000 hydronaut-2023.9/.gitignore
+-rw-r--r--   0        0        0     1063 2020-02-02 00:00:00.000000 hydronaut-2023.9/LICENSE.txt
+-rw-r--r--   0        0        0    21613 2020-02-02 00:00:00.000000 hydronaut-2023.9/README.md
+-rw-r--r--   0        0        0     1714 2020-02-02 00:00:00.000000 hydronaut-2023.9/pyproject.toml
+-rw-r--r--   0        0        0    22441 2020-02-02 00:00:00.000000 hydronaut-2023.9/PKG-INFO
```

### Comparing `hydronaut-2023.8/TODO.md` & `hydronaut-2023.9/TODO.md`

 * *Files identical despite different names*

### Comparing `hydronaut-2023.8/doc/Makefile` & `hydronaut-2023.9/doc/Makefile`

 * *Files identical despite different names*

### Comparing `hydronaut-2023.8/doc/make.bat` & `hydronaut-2023.9/doc/make.bat`

 * *Files identical despite different names*

### Comparing `hydronaut-2023.8/doc/source/conf.py` & `hydronaut-2023.9/doc/source/conf.py`

 * *Files identical despite different names*

### Comparing `hydronaut-2023.8/doc/source/hydronaut.hydra.rst` & `hydronaut-2023.9/doc/source/hydronaut.hydra.rst`

 * *Files identical despite different names*

### Comparing `hydronaut-2023.8/doc/source/hydronaut.rst` & `hydronaut-2023.9/doc/source/hydronaut.rst`

 * *Files identical despite different names*

### Comparing `hydronaut-2023.8/examples/dummy/conf/config.yaml` & `hydronaut-2023.9/examples/dummy/conf/config.yaml`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 # Common defaults to provide a validating schema and default logging
 # configuration.
 defaults:
-  - hf_config
+  - hydronaut_config
   - _self_
 
 # When invoked with --multirun, run the experiment for each combination of these
 # parameters (Cartesian product).
 hydra:
   sweeper:
     params:
```

### Comparing `hydronaut-2023.8/examples/dummy/src/experiment.py` & `hydronaut-2023.9/examples/dummy/src/experiment.py`

 * *Files identical despite different names*

### Comparing `hydronaut-2023.8/examples/pytorch_lightning-mnist/README.md` & `hydronaut-2023.9/examples/pytorch_lightning-mnist/README.md`

 * *Files identical despite different names*

### Comparing `hydronaut-2023.8/examples/pytorch_lightning-mnist/conf/config.yaml` & `hydronaut-2023.9/examples/pytorch_lightning-mnist/conf/config.yaml`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 # PyTorch lightning handles all parallelization so there is no need to use a
 # parallelized job launcher such as joblib here.
 defaults:
-  - hf_config
+  - hydronaut_config
   # Use the Optuna optimizer with the TPE sampler.
   - override hydra/sweeper: optuna
   - override hydra/sweeper/sampler: tpe
   - _self_
 
 hydra:
   # Set the default mode to MULTIRUN to obviate passing --multirun on each
```

### Comparing `hydronaut-2023.8/examples/pytorch_lightning-mnist/src/data.py` & `hydronaut-2023.9/examples/pytorch_lightning-mnist/src/data.py`

 * *Files identical despite different names*

### Comparing `hydronaut-2023.8/examples/pytorch_lightning-mnist/src/experiment.py` & `hydronaut-2023.9/examples/pytorch_lightning-mnist/src/experiment.py`

 * *Files identical despite different names*

### Comparing `hydronaut-2023.8/examples/pytorch_lightning-mnist/src/model.py` & `hydronaut-2023.9/examples/pytorch_lightning-mnist/src/model.py`

 * *Files identical despite different names*

### Comparing `hydronaut-2023.8/img/hydronaut_icon.svg` & `hydronaut-2023.9/img/hydronaut_icon.svg`

 * *Files identical despite different names*

### Comparing `hydronaut-2023.8/img/hydronaut_logo.svg` & `hydronaut-2023.9/img/hydronaut_logo.svg`

 * *Files identical despite different names*

### Comparing `hydronaut-2023.8/scripts/hydronaut-rsync-results.sh` & `hydronaut-2023.9/scripts/hydronaut-rsync-results.sh`

 * *Files identical despite different names*

### Comparing `hydronaut-2023.8/scripts/hydronaut-run_in_venv.sh` & `hydronaut-2023.9/scripts/hydronaut-run_in_venv.sh`

 * *Files identical despite different names*

### Comparing `hydronaut-2023.8/src/hydronaut/experiment.py` & `hydronaut-2023.9/src/hydronaut/experiment.py`

 * *Files identical despite different names*

### Comparing `hydronaut-2023.8/src/hydronaut/file.py` & `hydronaut-2023.9/src/hydronaut/file.py`

 * *Files identical despite different names*

### Comparing `hydronaut-2023.8/src/hydronaut/init.py` & `hydronaut-2023.9/src/hydronaut/init.py`

 * *Files 1% similar despite different names*

```diff
@@ -83,15 +83,15 @@
 # https://pypi.org/project/omegaconf/
 
 # Default values are used to override sections of the configuration file with
 # values from other files.
 defaults:
   # Ensure type-checking for the experiment section. This is specific to
   # Hydronaut. This will also set some defaults for logging configuration.
-  - hf_config'''.strip())
+  - hydronaut_config'''.strip())
 
             if pargs.sweeper == 'optuna':
                 handle.write('''
 
   # Use the Optuna sweeper. This is configured in the hydra.sweeper section
   # below.
   - override hydra/sweeper: optuna
```

### Comparing `hydronaut-2023.8/src/hydronaut/mlflow.py` & `hydronaut-2023.9/src/hydronaut/mlflow.py`

 * *Files identical despite different names*

### Comparing `hydronaut-2023.8/src/hydronaut/paths.py` & `hydronaut-2023.9/src/hydronaut/paths.py`

 * *Files identical despite different names*

### Comparing `hydronaut-2023.8/src/hydronaut/run.py` & `hydronaut-2023.9/src/hydronaut/run.py`

 * *Files identical despite different names*

### Comparing `hydronaut-2023.8/src/hydronaut/hydra/config.py` & `hydronaut-2023.9/src/hydronaut/hydra/config.py`

 * *Files 1% similar despite different names*

```diff
@@ -92,15 +92,15 @@
     defaults: Optional[DefaultsType] = field(default_factory=_get_hydronaut_defaults)
 
 
 def _get_hydronaut_defaults():
     '''
     Factory for defaults list.
     '''
-    return ['experiment/hf_experiment']
+    return ['experiment/hydronaut_experiment']
 
 
 @dataclass
 class HydronautConfig:
     '''
     Common Hydronaut configuration.
     '''
@@ -157,16 +157,16 @@
 
     Args:
         from_env:
             If True, re-initialize the Hydra configuration object from
             environment variables set configure_environment().
     '''
     store = ConfigStore.instance()
-    store.store(name='hf_experiment', group='experiment', node=ExperimentConfig)
-    store.store(name='hf_config', node=HydronautConfig)
+    store.store(name='hydronaut_experiment', group='experiment', node=ExperimentConfig)
+    store.store(name='hydronaut_config', node=HydronautConfig)
     reregister()
     if from_env:
         _reinitialize_from_environment()
 
 
 def _safe_resolve_hydra_conf(hydra_conf: DictConfig, conf: DictConfig) -> DictConfig:
     '''
```

### Comparing `hydronaut-2023.8/src/hydronaut/hydra/omegaconf.py` & `hydronaut-2023.9/src/hydronaut/hydra/omegaconf.py`

 * *Files identical despite different names*

### Comparing `hydronaut-2023.8/src/hydronaut/hydra/resolvers.py` & `hydronaut-2023.9/src/hydronaut/hydra/resolvers.py`

 * *Files identical despite different names*

### Comparing `hydronaut-2023.8/src/hydronaut/torch/lightning/experiment.py` & `hydronaut-2023.9/src/hydronaut/torch/lightning/experiment.py`

 * *Files identical despite different names*

### Comparing `hydronaut-2023.8/LICENSE.txt` & `hydronaut-2023.9/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `hydronaut-2023.8/README.md` & `hydronaut-2023.9/README.md`

 * *Files identical despite different names*

### Comparing `hydronaut-2023.8/pyproject.toml` & `hydronaut-2023.9/pyproject.toml`

 * *Files identical despite different names*

### Comparing `hydronaut-2023.8/PKG-INFO` & `hydronaut-2023.9/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: hydronaut
-Version: 2023.8
+Version: 2023.9
 Summary: A framework for exploring the depths of hyperparameter space with Hydra and MLflow.
 Project-URL: Source, https://gitlab.inria.fr/jrye/hydronaut
 Project-URL: Documentation, https://jrye.gitlabpages.inria.fr/hydronaut/
 Author-email: Jan-Michael Rye <jan-michael.rye@inria.fr>
 License-Expression: MIT
 License-File: LICENSE.txt
 Classifier: Operating System :: OS Independent
```

