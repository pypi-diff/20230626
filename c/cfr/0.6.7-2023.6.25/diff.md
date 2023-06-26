# Comparing `tmp/cfr-0.6.7.tar.gz` & `tmp/cfr-2023.6.25.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cfr-0.6.7.tar", last modified: Thu Jun 22 18:58:17 2023, max compression
+gzip compressed data, was "cfr-2023.6.25.tar", last modified: Mon Jun 26 05:07:57 2023, max compression
```

## Comparing `cfr-0.6.7.tar` & `cfr-2023.6.25.tar`

### file list

```diff
@@ -1,30 +1,30 @@
-drwxr-xr-x   0 fengzhu    (502) staff       (20)        0 2023-06-22 18:58:17.140037 cfr-0.6.7/
--rw-r--r--   0 fengzhu    (502) staff       (20)     1516 2022-04-27 05:34:15.000000 cfr-0.6.7/LICENSE
--rw-r--r--   0 fengzhu    (502) staff       (20)     1770 2023-06-22 18:58:17.139842 cfr-0.6.7/PKG-INFO
--rw-r--r--   0 fengzhu    (502) staff       (20)     1207 2023-05-29 21:16:00.000000 cfr-0.6.7/README.md
-drwxr-xr-x   0 fengzhu    (502) staff       (20)        0 2023-06-22 18:58:17.132615 cfr-0.6.7/bin/
--rw-r--r--   0 fengzhu    (502) staff       (20)     5163 2023-06-19 02:34:42.000000 cfr-0.6.7/bin/cfr
-drwxr-xr-x   0 fengzhu    (502) staff       (20)        0 2023-06-22 18:58:17.136906 cfr-0.6.7/cfr/
--rw-r--r--   0 fengzhu    (502) staff       (20)      732 2023-06-21 18:25:21.000000 cfr-0.6.7/cfr/__init__.py
--rw-r--r--   0 fengzhu    (502) staff       (20)    22467 2023-05-29 23:34:35.000000 cfr-0.6.7/cfr/climate.py
-drwxr-xr-x   0 fengzhu    (502) staff       (20)        0 2023-06-22 18:58:17.139499 cfr-0.6.7/cfr/da/
--rw-r--r--   0 fengzhu    (502) staff       (20)       22 2022-07-02 05:30:36.000000 cfr-0.6.7/cfr/da/__init__.py
--rw-r--r--   0 fengzhu    (502) staff       (20)    16319 2023-03-27 02:39:30.000000 cfr-0.6.7/cfr/da/enkf.py
--rw-r--r--   0 fengzhu    (502) staff       (20)    22484 2023-04-17 19:25:37.000000 cfr-0.6.7/cfr/gcm.py
--rw-r--r--   0 fengzhu    (502) staff       (20)     7623 2022-05-05 04:13:16.000000 cfr-0.6.7/cfr/ml.py
--rw-r--r--   0 fengzhu    (502) staff       (20)    67033 2023-06-22 17:29:40.000000 cfr-0.6.7/cfr/proxy.py
--rw-r--r--   0 fengzhu    (502) staff       (20)    45058 2023-06-20 03:51:38.000000 cfr-0.6.7/cfr/psm.py
--rw-r--r--   0 fengzhu    (502) staff       (20)    54926 2023-06-21 23:52:13.000000 cfr-0.6.7/cfr/reconjob.py
--rw-r--r--   0 fengzhu    (502) staff       (20)     2311 2023-03-27 02:39:30.000000 cfr-0.6.7/cfr/reconres.py
--rw-r--r--   0 fengzhu    (502) staff       (20)    19837 2023-05-29 21:16:00.000000 cfr-0.6.7/cfr/ts.py
--rw-r--r--   0 fengzhu    (502) staff       (20)    26722 2023-06-20 23:08:04.000000 cfr-0.6.7/cfr/utils.py
--rw-r--r--   0 fengzhu    (502) staff       (20)    54810 2023-04-17 19:25:37.000000 cfr-0.6.7/cfr/visual.py
-drwxr-xr-x   0 fengzhu    (502) staff       (20)        0 2023-06-22 18:58:17.138842 cfr-0.6.7/cfr.egg-info/
--rw-r--r--   0 fengzhu    (502) staff       (20)     1770 2023-06-22 18:58:17.000000 cfr-0.6.7/cfr.egg-info/PKG-INFO
--rw-r--r--   0 fengzhu    (502) staff       (20)      373 2023-06-22 18:58:17.000000 cfr-0.6.7/cfr.egg-info/SOURCES.txt
--rw-r--r--   0 fengzhu    (502) staff       (20)        1 2023-06-22 18:58:17.000000 cfr-0.6.7/cfr.egg-info/dependency_links.txt
--rw-r--r--   0 fengzhu    (502) staff       (20)        1 2022-04-28 04:59:29.000000 cfr-0.6.7/cfr.egg-info/not-zip-safe
--rw-r--r--   0 fengzhu    (502) staff       (20)      201 2023-06-22 18:58:17.000000 cfr-0.6.7/cfr.egg-info/requires.txt
--rw-r--r--   0 fengzhu    (502) staff       (20)        4 2023-06-22 18:58:17.000000 cfr-0.6.7/cfr.egg-info/top_level.txt
--rw-r--r--   0 fengzhu    (502) staff       (20)       38 2023-06-22 18:58:17.140095 cfr-0.6.7/setup.cfg
--rw-r--r--   0 fengzhu    (502) staff       (20)     1400 2023-06-22 18:58:04.000000 cfr-0.6.7/setup.py
+drwxr-xr-x   0 fengzhu    (502) staff       (20)        0 2023-06-26 05:07:57.484315 cfr-2023.6.25/
+-rw-r--r--   0 fengzhu    (502) staff       (20)     1516 2022-04-27 05:34:15.000000 cfr-2023.6.25/LICENSE
+-rw-r--r--   0 fengzhu    (502) staff       (20)     1774 2023-06-26 05:07:57.484111 cfr-2023.6.25/PKG-INFO
+-rw-r--r--   0 fengzhu    (502) staff       (20)     1207 2023-05-29 21:16:00.000000 cfr-2023.6.25/README.md
+drwxr-xr-x   0 fengzhu    (502) staff       (20)        0 2023-06-26 05:07:57.475570 cfr-2023.6.25/bin/
+-rw-r--r--   0 fengzhu    (502) staff       (20)     5134 2023-06-22 22:28:33.000000 cfr-2023.6.25/bin/cfr
+drwxr-xr-x   0 fengzhu    (502) staff       (20)        0 2023-06-26 05:07:57.480863 cfr-2023.6.25/cfr/
+-rw-r--r--   0 fengzhu    (502) staff       (20)      732 2023-06-21 18:25:21.000000 cfr-2023.6.25/cfr/__init__.py
+-rw-r--r--   0 fengzhu    (502) staff       (20)    22467 2023-05-29 23:34:35.000000 cfr-2023.6.25/cfr/climate.py
+drwxr-xr-x   0 fengzhu    (502) staff       (20)        0 2023-06-26 05:07:57.483768 cfr-2023.6.25/cfr/da/
+-rw-r--r--   0 fengzhu    (502) staff       (20)       22 2022-07-02 05:30:36.000000 cfr-2023.6.25/cfr/da/__init__.py
+-rw-r--r--   0 fengzhu    (502) staff       (20)    16319 2023-03-27 02:39:30.000000 cfr-2023.6.25/cfr/da/enkf.py
+-rw-r--r--   0 fengzhu    (502) staff       (20)    22484 2023-04-17 19:25:37.000000 cfr-2023.6.25/cfr/gcm.py
+-rw-r--r--   0 fengzhu    (502) staff       (20)     7623 2022-05-05 04:13:16.000000 cfr-2023.6.25/cfr/ml.py
+-rw-r--r--   0 fengzhu    (502) staff       (20)    67033 2023-06-22 17:29:40.000000 cfr-2023.6.25/cfr/proxy.py
+-rw-r--r--   0 fengzhu    (502) staff       (20)    45058 2023-06-20 03:51:38.000000 cfr-2023.6.25/cfr/psm.py
+-rw-r--r--   0 fengzhu    (502) staff       (20)    57502 2023-06-25 20:44:57.000000 cfr-2023.6.25/cfr/reconjob.py
+-rw-r--r--   0 fengzhu    (502) staff       (20)     4551 2023-06-26 04:44:01.000000 cfr-2023.6.25/cfr/reconres.py
+-rw-r--r--   0 fengzhu    (502) staff       (20)    19837 2023-06-26 04:41:16.000000 cfr-2023.6.25/cfr/ts.py
+-rw-r--r--   0 fengzhu    (502) staff       (20)    26716 2023-06-26 04:30:02.000000 cfr-2023.6.25/cfr/utils.py
+-rw-r--r--   0 fengzhu    (502) staff       (20)    55370 2023-06-26 05:04:39.000000 cfr-2023.6.25/cfr/visual.py
+drwxr-xr-x   0 fengzhu    (502) staff       (20)        0 2023-06-26 05:07:57.483043 cfr-2023.6.25/cfr.egg-info/
+-rw-r--r--   0 fengzhu    (502) staff       (20)     1774 2023-06-26 05:07:57.000000 cfr-2023.6.25/cfr.egg-info/PKG-INFO
+-rw-r--r--   0 fengzhu    (502) staff       (20)      373 2023-06-26 05:07:57.000000 cfr-2023.6.25/cfr.egg-info/SOURCES.txt
+-rw-r--r--   0 fengzhu    (502) staff       (20)        1 2023-06-26 05:07:57.000000 cfr-2023.6.25/cfr.egg-info/dependency_links.txt
+-rw-r--r--   0 fengzhu    (502) staff       (20)        1 2022-04-28 04:59:29.000000 cfr-2023.6.25/cfr.egg-info/not-zip-safe
+-rw-r--r--   0 fengzhu    (502) staff       (20)      201 2023-06-26 05:07:57.000000 cfr-2023.6.25/cfr.egg-info/requires.txt
+-rw-r--r--   0 fengzhu    (502) staff       (20)        4 2023-06-26 05:07:57.000000 cfr-2023.6.25/cfr.egg-info/top_level.txt
+-rw-r--r--   0 fengzhu    (502) staff       (20)       38 2023-06-26 05:07:57.484367 cfr-2023.6.25/setup.cfg
+-rw-r--r--   0 fengzhu    (502) staff       (20)     1404 2023-06-25 19:28:42.000000 cfr-2023.6.25/setup.py
```

### Comparing `cfr-0.6.7/LICENSE` & `cfr-2023.6.25/LICENSE`

 * *Files identical despite different names*

### Comparing `cfr-0.6.7/PKG-INFO` & `cfr-2023.6.25/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cfr
-Version: 0.6.7
+Version: 2023.6.25
 Summary: cfr: a Python package for Climate Field Reconstruction
 Home-page: https://github.com/fzhu2e/cfr
 Author: Feng Zhu, Julien Emile-Geay
 Author-email: fengzhu@ucar.edu, julieneg@usc.edu
 License: BSD 3-Clause
 Keywords: climate field reconstruction
 Classifier: Natural Language :: English
```

### Comparing `cfr-0.6.7/README.md` & `cfr-2023.6.25/README.md`

 * *Files identical despite different names*

### Comparing `cfr-0.6.7/bin/cfr` & `cfr-2023.6.25/bin/cfr`

 * *Files 2% similar despite different names*

```diff
@@ -10,15 +10,15 @@
 import os
 import cfr
 
 def main():
     parser = argparse.ArgumentParser(
             description='''
 ========================================================================================
- cfr: a scripting system for CFR (Feng Zhu, fengzhu@ucar.edu)
+ cfr: a scripting system for CFR
 ----------------------------------------------------------------------------------------
  Usage example for DA:
     cfr da -c config.yml -vb -s 1 2 -r
     # -c config.yml: run the reconstruction job according to config.yml
     # -vb: output the verbose runtime information
     # -s 1 2: set seeds as integers from 1 to 2
     # -r: run the Monte-Carlo iterations for PDA
```

### Comparing `cfr-0.6.7/cfr/__init__.py` & `cfr-2023.6.25/cfr/__init__.py`

 * *Files identical despite different names*

### Comparing `cfr-0.6.7/cfr/climate.py` & `cfr-2023.6.25/cfr/climate.py`

 * *Files identical despite different names*

### Comparing `cfr-0.6.7/cfr/da/enkf.py` & `cfr-2023.6.25/cfr/da/enkf.py`

 * *Files identical despite different names*

### Comparing `cfr-0.6.7/cfr/gcm.py` & `cfr-2023.6.25/cfr/gcm.py`

 * *Files identical despite different names*

### Comparing `cfr-0.6.7/cfr/ml.py` & `cfr-2023.6.25/cfr/ml.py`

 * *Files identical despite different names*

### Comparing `cfr-0.6.7/cfr/proxy.py` & `cfr-2023.6.25/cfr/proxy.py`

 * *Files identical despite different names*

### Comparing `cfr-0.6.7/cfr/psm.py` & `cfr-2023.6.25/cfr/psm.py`

 * *Files identical despite different names*

### Comparing `cfr-0.6.7/cfr/reconjob.py` & `cfr-2023.6.25/cfr/reconjob.py`

 * *Files 3% similar despite different names*

```diff
@@ -819,15 +819,15 @@
         self.save_cfg(save_dirpath=self.configs['save_dirpath'], verbose=verbose)
         if save_job: self.save(save_dirpath=self.configs['save_dirpath'], verbose=verbose)
 
         t_e = time.time()
         t_used = t_e - t_s
         p_success(f'>>> DONE! Total time used: {t_used/60:.2f} mins.')
 
-    def prep_graphem(self, recon_time=None, calib_time=None,  recon_period=None, recon_timescale=None, calib_period=None, verbose=False):
+    def prep_graphem(self, recon_time=None, calib_time=None,  recon_period=None, recon_timescale=None, calib_period=None, uniform_pdb=None, verbose=False):
         ''' A shortcut of the steps for GraphEM data preparation
 
         Args:
             recon_time (array list, optional): the time points to reconstruct
             calib_time (array list, optional): the time points for calibration
             recon_period (tuple, optional): the reconstruction timespan.
                 Effective when `recon_time` or `calib_time` is None. Defaults to None.
@@ -842,21 +842,38 @@
             calib_period = self.io_cfg('calib_period', list(calib_period), default=[1850, 2000], verbose=verbose)
 
             recon_time = np.arange(recon_period[0], recon_period[1]+1, recon_timescale)
             calib_time = np.arange(calib_period[0], calib_period[1]+1, recon_timescale)
         else:
             recon_time = self.io_cfg('recon_time', recon_time, verbose=verbose)
             calib_time = self.io_cfg('calib_time', calib_time, verbose=verbose)
+            recon_period = self.io_cfg('recon_period', [np.min(recon_time), np.max(recon_time)], verbose=verbose)
+            calib_period = self.io_cfg('calib_period', [np.min(calib_time), np.max(calib_time)], verbose=verbose)
+            recon_timescale = self.io_cfg('recon_timescale', np.median(np.diff(recon_time)), verbose=verbose)  # unit: yr
+
+        uniform_pdb = self.io_cfg('uniform_pdb', uniform_pdb, default=True, verbose=verbose)
+        if uniform_pdb:
+            pobj_list = []
+            for pobj in self.proxydb:
+                if np.min(pobj.time) <= recon_period[0]:
+                    pobj_list.append(pobj)
+            new_pdb = ProxyDatabase()
+            new_pdb += pobj_list
+            self.proxydb = new_pdb
+            if verbose: p_success(f'>>> ProxyDatabase filtered to be more uniform. {self.proxydb.nrec} records remaining.')
 
+        self.center_proxydb(ref_period=calib_period, verbose=verbose)
+    
         self.graphem_params = {}
         self.graphem_params['recon_time'] = recon_time
         self.graphem_params['calib_time'] = calib_time
         if verbose: p_success(f'>>> job.graphem_params["recon_time"] created')
         if verbose: p_success(f'>>> job.graphem_params["calib_time"] created')
 
+
         vn = list(self.obs.keys())[0]
         obs = self.obs[vn]  
         obs_nt = obs.da.shape[0]
         obs_2d = obs.da.values.reshape(obs_nt, -1)
         obs_npos = np.shape(obs_2d)[-1]
 
         recon_idx = [list(obs.da.time).index(t) for t in recon_time if t in obs.da.time]
@@ -906,15 +923,15 @@
     def graphem_kcv(self, cv_time, ctrl_params, graph_type='neighborhood', stat='MSE', n_splits=5):
         ''' k-fold cross-validation
         
         Arguments
         ---------
         
         cv_time : array-like, 1d
-            explain how it differs from recon_time or calib_time
+            cross validation time points
             
         ctrl_params : array-like, 1d
             array of control parameters to try
             
         graph_type : str
             type of graph. Either "neighborhood" or "glasso"
             
@@ -987,14 +1004,17 @@
         `estimate_graph=False` and `graph=g.adj`, where `g` is the :py:`Graph` object.
 
         Args:
             save_dirpath (str): the path to save the related results
             load_precalculated (bool, optional): load the precalculated `Graph` object. Defaults to False.
             verbose (bool, optional): print verbose information. Defaults to False.
             fit_kws (dict): the arguments for :py:meth: `GraphEM.solver.GraphEM.fit`
+                The most important one is "graph_method"; availabel options include "neighborhood", "glasso", and "hybrid", where
+                "hybrid" means run "neighborhood" first with default `cutoff_radius=1500` to infill the data matrix and then
+                ran "glasso" with default `sp_FF=3, sp_FP=3` to improve the result further.
 
         See also:
             cfr.graphem.solver.GraphEM.fit : fitting the GraphEM method
 
         '''
         compress_params = self.io_cfg('compress_params', compress_params, default={'zlib': True}, verbose=verbose)
 
@@ -1012,22 +1032,49 @@
             self.graphem_solver = pd.read_pickle(solver_save_path)
             if verbose: p_success(f'job.graphem_solver created with the existing result at: {solver_save_path}')
         else:
             self.graphem_solver = GraphEM()
             fit_kwargs = {
                 'lonlat': self.graphem_params['lonlat'],
                 'graph_method': 'neighborhood',
+                'cutoff_radius': 1500,
+                'sp_FF': 3,
+                'sp_FP': 3,
             }
             fit_kwargs.update(fit_kws)
-            self.graphem_solver.fit(
-                self.graphem_params['field'],
-                self.graphem_params['proxy'],
-                self.graphem_params['calib_idx'],
-                verbose=verbose,
-                **fit_kwargs)
+            if fit_kwargs['graph_method'] in ['neighborhood', 'glasso']:
+                self.graphem_solver.fit(
+                    self.graphem_params['field'],
+                    self.graphem_params['proxy'],
+                    self.graphem_params['calib_idx'],
+                    verbose=verbose,
+                    **fit_kwargs)
+            elif fit_kwargs['graph_method'] == 'hybrid':
+                fit_kwargs.update({'graph_method': 'neighborhood'})
+                self.graphem_solver.fit(
+                    self.graphem_params['field'],
+                    self.graphem_params['proxy'],
+                    self.graphem_params['calib_idx'],
+                    verbose=verbose,
+                    **fit_kwargs)
+
+                inst = self.graphem_params['calib_idx']
+                G_L = Graph(
+                    lonlat = self.graphem_params['lonlat'],
+                    field = self.graphem_solver.field_r[inst],
+                    proxy = self.graphem_solver.proxy_r[inst,:])
+
+                G_L.glasso_adj(target_FF=fit_kwargs['sp_FF'], target_FP=fit_kwargs['sp_FP'])
+                fit_kwargs.update({'estimate_graph': False, 'graph': G_L.adj})
+                self.graphem_solver.fit(
+                    self.graphem_params['field'],
+                    self.graphem_params['proxy'],
+                    self.graphem_params['calib_idx'],
+                    verbose=verbose,
+                    **fit_kwargs)
 
             if verbose: p_success(f'job.graphem_solver created and saved to: {solver_save_path}')
 
             if solver_save_path is not None:
                 pd.to_pickle(self.graphem_solver, solver_save_path)
                 if verbose: p_success(f'job.graphem_solver saved to: {solver_save_path}')
```

### Comparing `cfr-0.6.7/cfr/ts.py` & `cfr-2023.6.25/cfr/ts.py`

 * *Files 0% similar despite different names*

```diff
@@ -500,15 +500,15 @@
         if ylabel is None: ylabel = self.value_name
         ax.set_ylabel(ylabel)
 
         if xlim is not None:
             ax.set_xlim(xlim)
 
         if ylim is not None:
-            ax.set_xlim(ylim)
+            ax.set_ylim(ylim)
 
 
         _legend_kwargs = {'ncol': len(qs)//2+1+n_ref, 'loc': 'upper left'}
         _legend_kwargs.update(lgd_kws)
         ax.legend(**_legend_kwargs)
 
         if title is not None:
```

### Comparing `cfr-0.6.7/cfr/utils.py` & `cfr-2023.6.25/cfr/utils.py`

 * *Files 1% similar despite different names*

```diff
@@ -511,16 +511,16 @@
 
     CE = np.zeros(dims)
 
     # error
     error = test - ref
 
     # CE
-    numer = np.nansum(np.power(error,2),axis=0)
-    denom = np.nansum(np.power(ref-np.nanmean(ref,axis=0),2),axis=0)
+    numer = np.sum(np.power(error,2),axis=0)
+    denom = np.sum(np.power(ref-np.nanmean(ref,axis=0),2),axis=0)
     CE    = 1. - np.divide(numer,denom)
 
     if valid:
         nbok  = np.sum(np.isfinite(ref),axis=0)
         nball = float(dims_ref[0])
         ratio = np.divide(nbok,nball)
         indok  = np.where(ratio >= valid)
```

### Comparing `cfr-0.6.7/cfr/visual.py` & `cfr-2023.6.25/cfr/visual.py`

 * *Files 2% similar despite different names*

```diff
@@ -19,14 +19,15 @@
 from scipy.stats import cumfreq, gaussian_kde
 from scipy.integrate import cumtrapz
 from matplotlib.lines import Line2D
 from matplotlib.patches import Patch
 from matplotlib.legend_handler import HandlerLine2D
 import pathlib
 import pandas as pd
+import string
 
 from cartopy import util as cutil
 from . import utils
 
 class PAGES2k:
     ''' A bunch of PAGES2k style settings
     '''
@@ -1392,8 +1393,29 @@
     ax['pc'].set_title(pc_title)
     ax['pc'].set_xlabel('Year')
     ax['pc'].set_ylabel(pc_title)
     ax['pc'].grid(ls='--')
     ax['pc'].spines.top.set_visible(False)
     ax['pc'].spines.right.set_visible(False)
 
-    return fig, ax
+    return fig, ax
+
+def add_annotation(ax, fs=20, loc_x=0, loc_y=1.03, start=0, style=None):
+    if type(ax) is dict:
+        ax = ax.values()
+
+    if type(fs) is not list:
+        fs = [fs] * len(ax)
+
+    for i, v in enumerate(ax):
+        letter_str = string.ascii_lowercase[i+start]
+
+        if style == ')':
+            letter_str = f'{letter_str})'
+        elif style == '()':
+            letter_str = f'({letter_str})'
+
+        v.text(
+            loc_x, loc_y, letter_str,
+            transform=v.transAxes, 
+            size=fs[i], weight='bold',
+        )
```

### Comparing `cfr-0.6.7/cfr.egg-info/PKG-INFO` & `cfr-2023.6.25/cfr.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cfr
-Version: 0.6.7
+Version: 2023.6.25
 Summary: cfr: a Python package for Climate Field Reconstruction
 Home-page: https://github.com/fzhu2e/cfr
 Author: Feng Zhu, Julien Emile-Geay
 Author-email: fengzhu@ucar.edu, julieneg@usc.edu
 License: BSD 3-Clause
 Keywords: climate field reconstruction
 Classifier: Natural Language :: English
```

### Comparing `cfr-0.6.7/setup.py` & `cfr-2023.6.25/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from setuptools import setup, find_packages
 
 with open('README.md', 'r') as fh:
     long_description = fh.read()
 
 setup(
     name='cfr',  # required
-    version='0.6.7',
+    version='2023.6.25',
     description='cfr: a Python package for Climate Field Reconstruction',
     long_description=long_description,
     long_description_content_type='text/x-rst',
     author='Feng Zhu, Julien Emile-Geay',
     author_email='fengzhu@ucar.edu, julieneg@usc.edu',
     url='https://github.com/fzhu2e/cfr',
     packages=find_packages(),
```

