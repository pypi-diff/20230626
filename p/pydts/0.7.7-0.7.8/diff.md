# Comparing `tmp/pydts-0.7.7.tar.gz` & `tmp/pydts-0.7.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pydts-0.7.7.tar", max compression
+gzip compressed data, was "pydts-0.7.8.tar", max compression
```

## Comparing `pydts-0.7.7.tar` & `pydts-0.7.8.tar`

### file list

```diff
@@ -1,22 +1,22 @@
--rw-r--r--   0        0        0      757 2022-06-10 18:48:04.918673 pydts-0.7.7/LICENSE
--rw-r--r--   0        0        0     2655 2023-03-03 09:40:33.185838 pydts-0.7.7/README.md
--rw-r--r--   0        0        0     1441 2023-06-24 12:15:38.501195 pydts-0.7.7/pyproject.toml
--rw-r--r--   0        0        0     6148 2022-07-28 20:14:40.680457 pydts-0.7.7/src/pydts/.DS_Store
--rw-r--r--   0        0        0       21 2022-05-31 10:30:06.735807 pydts-0.7.7/src/pydts/__init__.py
--rw-r--r--   0        0        0    12925 2023-05-02 14:58:03.593428 pydts-0.7.7/src/pydts/base_fitters.py
--rw-r--r--   0        0        0      179 2022-05-31 10:30:06.735945 pydts-0.7.7/src/pydts/config.py
--rw-r--r--   0        0        0    12393 2023-02-22 10:39:50.257509 pydts-0.7.7/src/pydts/cross_validation.py
--rw-r--r--   0        0        0    15114 2023-05-03 10:21:44.094825 pydts-0.7.7/src/pydts/data_generation.py
--rw-r--r--   0        0        0     6148 2022-07-30 20:46:05.091197 pydts-0.7.7/src/pydts/datasets/.DS_Store
--rw-r--r--   0        0        0  4942233 2022-07-30 20:42:16.583147 pydts-0.7.7/src/pydts/datasets/LOS_simulated_data.csv
--rw-r--r--   0        0        0    21459 2023-05-02 09:39:52.357498 pydts-0.7.7/src/pydts/evaluation.py
--rw-r--r--   0        0        0        0 2022-05-31 10:30:06.739086 pydts-0.7.7/src/pydts/examples_utils/__init__.py
--rw-r--r--   0        0        0      286 2022-05-31 10:30:06.739154 pydts-0.7.7/src/pydts/examples_utils/datasets.py
--rw-r--r--   0        0        0    10244 2023-05-02 16:42:26.483452 pydts-0.7.7/src/pydts/examples_utils/generate_simulations_data.py
--rw-r--r--   0        0        0    14554 2023-06-22 21:08:27.939724 pydts-0.7.7/src/pydts/examples_utils/mimic_consts.py
--rw-r--r--   0        0        0    35420 2023-06-24 12:18:25.376596 pydts-0.7.7/src/pydts/examples_utils/plots.py
--rw-r--r--   0        0        0     1708 2022-07-28 20:09:56.672834 pydts-0.7.7/src/pydts/examples_utils/simulations_data_config.py
--rw-r--r--   0        0        0    31476 2023-06-23 19:40:20.471655 pydts-0.7.7/src/pydts/fitters.py
--rw-r--r--   0        0        0     8936 2023-02-22 11:16:27.801701 pydts-0.7.7/src/pydts/model_selection.py
--rw-r--r--   0        0        0     5994 2022-12-02 13:43:44.154153 pydts-0.7.7/src/pydts/utils.py
--rw-r--r--   0        0        0     4026 1970-01-01 00:00:00.000000 pydts-0.7.7/PKG-INFO
+-rw-r--r--   0        0        0      757 2022-06-10 18:48:04.918673 pydts-0.7.8/LICENSE
+-rw-r--r--   0        0        0     2655 2023-03-03 09:40:33.185838 pydts-0.7.8/README.md
+-rw-r--r--   0        0        0     1441 2023-06-26 12:27:54.410152 pydts-0.7.8/pyproject.toml
+-rw-r--r--   0        0        0     6148 2022-07-28 20:14:40.680457 pydts-0.7.8/src/pydts/.DS_Store
+-rw-r--r--   0        0        0       21 2022-05-31 10:30:06.735807 pydts-0.7.8/src/pydts/__init__.py
+-rw-r--r--   0        0        0    12925 2023-05-02 14:58:03.593428 pydts-0.7.8/src/pydts/base_fitters.py
+-rw-r--r--   0        0        0      179 2022-05-31 10:30:06.735945 pydts-0.7.8/src/pydts/config.py
+-rw-r--r--   0        0        0    12393 2023-02-22 10:39:50.257509 pydts-0.7.8/src/pydts/cross_validation.py
+-rw-r--r--   0        0        0    15114 2023-05-03 10:21:44.094825 pydts-0.7.8/src/pydts/data_generation.py
+-rw-r--r--   0        0        0     6148 2022-07-30 20:46:05.091197 pydts-0.7.8/src/pydts/datasets/.DS_Store
+-rw-r--r--   0        0        0  4942233 2022-07-30 20:42:16.583147 pydts-0.7.8/src/pydts/datasets/LOS_simulated_data.csv
+-rw-r--r--   0        0        0    21459 2023-05-02 09:39:52.357498 pydts-0.7.8/src/pydts/evaluation.py
+-rw-r--r--   0        0        0        0 2022-05-31 10:30:06.739086 pydts-0.7.8/src/pydts/examples_utils/__init__.py
+-rw-r--r--   0        0        0      286 2022-05-31 10:30:06.739154 pydts-0.7.8/src/pydts/examples_utils/datasets.py
+-rw-r--r--   0        0        0    10244 2023-05-02 16:42:26.483452 pydts-0.7.8/src/pydts/examples_utils/generate_simulations_data.py
+-rw-r--r--   0        0        0    14554 2023-06-22 21:08:27.939724 pydts-0.7.8/src/pydts/examples_utils/mimic_consts.py
+-rw-r--r--   0        0        0    35688 2023-06-26 12:35:09.771826 pydts-0.7.8/src/pydts/examples_utils/plots.py
+-rw-r--r--   0        0        0     1708 2022-07-28 20:09:56.672834 pydts-0.7.8/src/pydts/examples_utils/simulations_data_config.py
+-rw-r--r--   0        0        0    31476 2023-06-23 19:40:20.471655 pydts-0.7.8/src/pydts/fitters.py
+-rw-r--r--   0        0        0     8936 2023-02-22 11:16:27.801701 pydts-0.7.8/src/pydts/model_selection.py
+-rw-r--r--   0        0        0     5994 2022-12-02 13:43:44.154153 pydts-0.7.8/src/pydts/utils.py
+-rw-r--r--   0        0        0     4026 1970-01-01 00:00:00.000000 pydts-0.7.8/PKG-INFO
```

### Comparing `pydts-0.7.7/LICENSE` & `pydts-0.7.8/LICENSE`

 * *Files identical despite different names*

### Comparing `pydts-0.7.7/README.md` & `pydts-0.7.8/README.md`

 * *Files identical despite different names*

### Comparing `pydts-0.7.7/pyproject.toml` & `pydts-0.7.8/pyproject.toml`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "pydts"
-version = "0.7.7"
+version = "0.7.8"
 description = "Discrete time survival analysis with competing risks"
 authors = ["Tomer Meir <tomer1812@gmail.com>", "Rom Gutman <rom.gutman1@gmail.com>", "Malka Gorfine <malkago12@gmail.com>"]
 license = "GNU GPLv3"
 readme = "README.md"
 homepage = "https://github.com/tomer1812/pydts"
 repository = "https://github.com/tomer1812/pydts"
 keywords = ["Discrete Time", "Time to Event" ,"Survival Analysis", "Competing Events"]
```

### Comparing `pydts-0.7.7/src/pydts/.DS_Store` & `pydts-0.7.8/src/pydts/.DS_Store`

 * *Files identical despite different names*

### Comparing `pydts-0.7.7/src/pydts/base_fitters.py` & `pydts-0.7.8/src/pydts/base_fitters.py`

 * *Files identical despite different names*

### Comparing `pydts-0.7.7/src/pydts/cross_validation.py` & `pydts-0.7.8/src/pydts/cross_validation.py`

 * *Files identical despite different names*

### Comparing `pydts-0.7.7/src/pydts/data_generation.py` & `pydts-0.7.8/src/pydts/data_generation.py`

 * *Files identical despite different names*

### Comparing `pydts-0.7.7/src/pydts/datasets/.DS_Store` & `pydts-0.7.8/src/pydts/datasets/.DS_Store`

 * *Files identical despite different names*

### Comparing `pydts-0.7.7/src/pydts/datasets/LOS_simulated_data.csv` & `pydts-0.7.8/src/pydts/datasets/LOS_simulated_data.csv`

 * *Files identical despite different names*

### Comparing `pydts-0.7.7/src/pydts/evaluation.py` & `pydts-0.7.8/src/pydts/evaluation.py`

 * *Files identical despite different names*

### Comparing `pydts-0.7.7/src/pydts/examples_utils/generate_simulations_data.py` & `pydts-0.7.8/src/pydts/examples_utils/generate_simulations_data.py`

 * *Files identical despite different names*

### Comparing `pydts-0.7.7/src/pydts/examples_utils/mimic_consts.py` & `pydts-0.7.8/src/pydts/examples_utils/mimic_consts.py`

 * *Files identical despite different names*

### Comparing `pydts-0.7.7/src/pydts/examples_utils/plots.py` & `pydts-0.7.8/src/pydts/examples_utils/plots.py`

 * *Files 1% similar despite different names*

```diff
@@ -114,15 +114,16 @@
 
 
 def plot_models_coefficients(alpha_dict: dict, beta_dict: dict, times: Iterable,
                              counts_df: pd.DataFrame,
                              n_cov: int = 5,
                              first_model_name: str = 'Lee et al.',
                              second_model_name: str = 'two-step',
-                             filename: str = None) -> None:
+                             filename: str = None,
+                             show: bool = True) -> None:
     """
     This method takes the repetitive runs results and plotting the comparison between the methods coefs
 
     Args:
         alpha_dict (dict): a dict that contains for each event type (key) a dataframe of all the $\alpha_t$ (value)
         beta_dict (dict): a dict that contains for each event type(key) a dataframe of all the $\beta_t$ (value)
         times (Iterable): array like that contains all the unique times that were used
@@ -189,14 +190,16 @@
     ax.set_xlabel('Covariate', fontsize=18)
     ax.set_ylabel(r'$\beta}$', fontsize=18)
     ax.legend(loc='upper center', fontsize=12)
     ax.set_ylim([-1.5, 1])
     fig.tight_layout()
     if filename is not None:
         fig.savefig(filename, dpi=300)
+    if show:
+        plt.show()
 
 
 def plot_LOS_simulation_figure1(data_df):
     text_sz = 16
 
     fig, axes = plt.subplots(2, 2, figsize=(14, 8))
 
@@ -517,15 +520,15 @@
     if filename is not None:
         fig.savefig(os.path.join(OUTPUT_DIR, filename), dpi=300)
 
     if return_summary:
         return res_dict
 
 
-def plot_jss_reps_coef_std(rep_dict: dict, return_summary: bool = True, filename: str = None, paper_plots: bool = False):
+def plot_jss_reps_coef_std(rep_dict: dict, return_summary: bool = True, filename: str = None, show: bool = True):
     alphabet_list = list(string.ascii_lowercase)
     first_key = next(iter(rep_dict))    # deal with cases where there isn't 0 in samples
     coef_types = list(rep_dict[first_key].keys())  # alpha, beta
     event_types = rep_dict[first_key][coef_types[0]].keys()
     fig, axes = plt.subplots(1, 2, figsize=(12, 5))
     res_dict = {coef: {event_type: None for event_type in event_types} for coef in coef_types}
     for idct, coef_type in enumerate(coef_types):
@@ -552,26 +555,27 @@
                     ax.set_ylim([0, 0.2])
                 elif ((idct == 0) and (idet == 1)):
                     ax.set_xlim([0, 0.25])
                     ax.set_ylim([0, 0.25])
                 latter = "\\alpha" if coef_type == "alpha" else "\\beta"
                 ax.set_title(f"${latter}{event_type}$", fontsize=18)
     fig.tight_layout()
-    fig.show()
+    if show:
+        plt.show()
     if filename is not None:
         fig.savefig(filename, dpi=300)
-
     if return_summary:
         return res_dict
 
 
 
 def plot_times(times_dict: dict,
                filename: str = None,
-               ax = None, color='tab:blue') -> None:
+               ax = None, color='tab:blue',
+               show: bool = True) -> None:
     if ax is None:
 
         ax = pd.DataFrame.from_dict(times_dict).boxplot(figsize=(8, 6), boxprops={"lw": 1.5, "color": "tab:blue"},
                                                         medianprops={"lw": 2, "color": "tab:green"},
                                                         flierprops={'markeredgecolor': "tab:blue"})
     else:
         pd.DataFrame.from_dict(times_dict).boxplot(boxprops={"lw": 1.5, "color": color},
@@ -582,15 +586,16 @@
     ax.tick_params(axis='both', which='major', labelsize=15)
     ax.tick_params(axis='both', which='minor', labelsize=15)
     ax.set_ylabel("Fitting Time [seconds]", fontdict={"size": 18}) # "weight": 'bold',
     ax.set_xlabel("Model type", fontdict={"size": 18}) # "weight": 'bold',
 
     #ax.tick_params(labelsize=14, grid_lw=0.5, grid_alpha=0.6)
     plt.tight_layout()
-    plt.show()
+    if show:
+        plt.show()
     if filename is not None:
         ax.figure.savefig(os.path.join(OUTPUT_DIR, filename), dpi=300)
     return ax
 
 
 def plot_cif_plots(pred_df: pd.DataFrame, event: str, return_ax: bool = False, ax: plt.Axes = None,
                    pad: float = 0.15, scale: int = 5) -> None:
@@ -633,15 +638,16 @@
 
     y_max = min(df[cols].max().max() + pad, 1)
     y_max = scale_perc_limits(y_max, scale=scale, up=True)
     return y_min, y_max
 
 
 def plot_events_occurrence(patients_df: pd.DataFrame, ax: plt.Axes = None, event_type_col: str = 'J',
-                           pid_col: str = 'pid', event_time_col: str = 'X', fname: str = None):
+                           pid_col: str = 'pid', event_time_col: str = 'X', fname: str = None,
+                           show: bool = True):
     if ax is None:
         tight = True
         fig, ax = plt.subplots(1, 1, figsize=(10, 4))
     else:
         tight = False
     patients_df.groupby([event_type_col, event_time_col])[pid_col].count().unstack('J').fillna(0).plot(ax=ax,
                                                                                                        kind='bar',
@@ -650,18 +656,20 @@
     ax.tick_params(axis='both', which='minor', labelsize=15)
     ax.set_xlabel(f"Time", fontdict={'size': 18})
     ax.set_ylabel(f"Number of Observations", fontdict={'size': 18})
     if tight:
         fig.tight_layout()
     if fname is not None:
         fig.savefig(fname, dpi=300)
+    if show:
+        plt.show()
     return ax
 
 
-def plot_example_pred_output(pred_df, fname: str = None):
+def plot_example_pred_output(pred_df, fname: str = None, show: bool = True):
     gs = gridspec.GridSpec(4, 4)
     ax1 = plt.subplot(gs[0, 0:2])
     ax2 = plt.subplot(gs[0, 2:])
     ax3 = plt.subplot(gs[1, 0:2])
     ax4 = plt.subplot(gs[1, 2:])
     ax5 = plt.subplot(gs[2, 0:2])
     ax6 = plt.subplot(gs[2, 2:])
@@ -703,14 +711,16 @@
             ax.tick_params(axis='both', which='major', labelsize=14)
             ax.tick_params(axis='both', which='minor', labelsize=14)
             ax.legend()
         
     fig.tight_layout()
     if fname is not None:
         fig.savefig(fname, dpi=300)
+    if show:
+        plt.show()
 
 
 def plot_example_estimated_params(fitter, fname: str = None):
     fig, axes = plt.subplots(1,2, figsize=(14,7))
     ax = axes[0]
     fitter.plot_all_events_alpha(ax=ax, show=False)
     ax.grid()
```

### Comparing `pydts-0.7.7/src/pydts/examples_utils/simulations_data_config.py` & `pydts-0.7.8/src/pydts/examples_utils/simulations_data_config.py`

 * *Files identical despite different names*

### Comparing `pydts-0.7.7/src/pydts/fitters.py` & `pydts-0.7.8/src/pydts/fitters.py`

 * *Files identical despite different names*

### Comparing `pydts-0.7.7/src/pydts/model_selection.py` & `pydts-0.7.8/src/pydts/model_selection.py`

 * *Files identical despite different names*

### Comparing `pydts-0.7.7/src/pydts/utils.py` & `pydts-0.7.8/src/pydts/utils.py`

 * *Files identical despite different names*

### Comparing `pydts-0.7.7/PKG-INFO` & `pydts-0.7.8/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pydts
-Version: 0.7.7
+Version: 0.7.8
 Summary: Discrete time survival analysis with competing risks
 Home-page: https://github.com/tomer1812/pydts
 License: GNU GPLv3
 Keywords: Discrete Time,Time to Event,Survival Analysis,Competing Events
 Author: Tomer Meir
 Author-email: tomer1812@gmail.com
 Requires-Python: >=3.8,<3.11
```

