# Comparing `tmp/sleqp-1.0.0.tar.gz` & `tmp/sleqp-1.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sleqp-1.0.0.tar", last modified: Fri Jun  9 13:41:50 2023, max compression
+gzip compressed data, was "sleqp-1.0.1.tar", last modified: Mon Jun 26 15:43:33 2023, max compression
```

## Comparing `sleqp-1.0.0.tar` & `sleqp-1.0.1.tar`

### file list

```diff
@@ -1,47 +1,47 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-09 13:41:50.553554 sleqp-1.0.0/
--rw-rw-rw-   0 root         (0) root         (0)     7652 2023-04-28 08:35:37.000000 sleqp-1.0.0/LICENSE.txt
--rw-rw-rw-   0 root         (0) root         (0)       91 2023-06-09 13:28:30.000000 sleqp-1.0.0/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)      673 2023-06-09 13:41:50.553554 sleqp-1.0.0/PKG-INFO
--rw-rw-rw-   0 root         (0) root         (0)      126 2023-06-09 13:28:30.000000 sleqp-1.0.0/pyproject.toml
--rw-rw-rw-   0 root         (0) root         (0)       12 2023-06-09 13:28:30.000000 sleqp-1.0.0/requirements.txt
--rw-r--r--   0 root         (0) root         (0)       38 2023-06-09 13:41:50.553554 sleqp-1.0.0/setup.cfg
--rw-rw-rw-   0 root         (0) root         (0)     2712 2023-06-09 13:39:40.000000 sleqp-1.0.0/setup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-09 13:41:50.545554 sleqp-1.0.0/src/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-09 13:41:50.549554 sleqp-1.0.0/src/extension/
--rw-rw-rw-   0 root         (0) root         (0)     1153 2023-06-09 13:28:30.000000 sleqp-1.0.0/src/extension/call.pxi
--rw-rw-rw-   0 root         (0) root         (0)     3827 2023-06-09 13:28:30.000000 sleqp-1.0.0/src/extension/callback.pxi
--rw-rw-rw-   0 root         (0) root         (0)       80 2023-06-09 13:28:30.000000 sleqp-1.0.0/src/extension/cmp.pxi
--rw-rw-rw-   0 root         (0) root         (0)    26164 2023-06-09 13:28:30.000000 sleqp-1.0.0/src/extension/csleqp.pxd
--rw-rw-rw-   0 root         (0) root         (0)     6111 2023-06-09 13:28:30.000000 sleqp-1.0.0/src/extension/dyn.pxi
--rw-rw-rw-   0 root         (0) root         (0)    11767 2023-06-09 13:28:30.000000 sleqp-1.0.0/src/extension/func.pxi
--rw-rw-rw-   0 root         (0) root         (0)      665 2023-06-09 13:28:30.000000 sleqp-1.0.0/src/extension/gil.pxi
--rw-rw-rw-   0 root         (0) root         (0)     1896 2023-06-09 13:28:30.000000 sleqp-1.0.0/src/extension/hess_struct.pxi
--rw-rw-rw-   0 root         (0) root         (0)     1927 2023-06-09 13:28:30.000000 sleqp-1.0.0/src/extension/iterate.pxi
--rw-rw-rw-   0 root         (0) root         (0)     1696 2023-06-09 13:28:30.000000 sleqp-1.0.0/src/extension/log.pxi
--rw-rw-rw-   0 root         (0) root         (0)     7687 2023-06-09 13:28:30.000000 sleqp-1.0.0/src/extension/lsq.pxi
--rw-rw-rw-   0 root         (0) root         (0)    12748 2023-06-09 13:28:30.000000 sleqp-1.0.0/src/extension/problem.pxi
--rw-rw-rw-   0 root         (0) root         (0)     6478 2023-06-09 13:28:30.000000 sleqp-1.0.0/src/extension/scale.pxi
--rw-rw-rw-   0 root         (0) root         (0)     7318 2023-06-09 13:28:30.000000 sleqp-1.0.0/src/extension/settings.pxi
--rw-rw-rw-   0 root         (0) root         (0)      623 2023-06-09 13:28:30.000000 sleqp-1.0.0/src/extension/sleqp.pyx
--rw-rw-rw-   0 root         (0) root         (0)    10919 2023-06-09 13:28:30.000000 sleqp-1.0.0/src/extension/solver.pxi
--rw-rw-rw-   0 root         (0) root         (0)     3643 2023-06-09 13:28:30.000000 sleqp-1.0.0/src/extension/sparse.pxi
--rw-rw-rw-   0 root         (0) root         (0)     1051 2023-06-09 13:28:30.000000 sleqp-1.0.0/src/extension/sparse_matrix.pxi
--rw-rw-rw-   0 root         (0) root         (0)     6620 2023-06-09 13:28:30.000000 sleqp-1.0.0/src/extension/types.pxi
--rw-rw-rw-   0 root         (0) root         (0)      229 2023-06-09 13:28:30.000000 sleqp-1.0.0/src/extension/version.pxi
--rw-rw-rw-   0 root         (0) root         (0)     2263 2023-06-09 13:28:30.000000 sleqp-1.0.0/src/extension/working_set.pxi
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-09 13:41:50.549554 sleqp-1.0.0/src/sleqp/
--rw-rw-rw-   0 root         (0) root         (0)      101 2023-06-09 13:28:30.000000 sleqp-1.0.0/src/sleqp/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     1323 2023-06-09 13:28:30.000000 sleqp-1.0.0/src/sleqp/_bounds.py
--rw-rw-rw-   0 root         (0) root         (0)     1696 2023-06-09 13:28:30.000000 sleqp-1.0.0/src/sleqp/_cons.py
--rw-rw-rw-   0 root         (0) root         (0)     2537 2023-06-09 13:28:30.000000 sleqp-1.0.0/src/sleqp/_cons_func.py
--rw-rw-rw-   0 root         (0) root         (0)     2139 2023-06-09 13:28:30.000000 sleqp-1.0.0/src/sleqp/_derivative.py
--rw-rw-rw-   0 root         (0) root         (0)     2113 2023-06-09 13:28:30.000000 sleqp-1.0.0/src/sleqp/_func.py
--rw-rw-rw-   0 root         (0) root         (0)     3556 2023-06-09 13:28:30.000000 sleqp-1.0.0/src/sleqp/_hessian.py
--rw-rw-rw-   0 root         (0) root         (0)      948 2023-06-09 13:28:30.000000 sleqp-1.0.0/src/sleqp/_linear.py
--rw-rw-rw-   0 root         (0) root         (0)     6465 2023-06-09 13:28:30.000000 sleqp-1.0.0/src/sleqp/minimize.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-09 13:41:50.553554 sleqp-1.0.0/src/sleqp.egg-info/
--rw-r--r--   0 root         (0) root         (0)      673 2023-06-09 13:41:50.000000 sleqp-1.0.0/src/sleqp.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      950 2023-06-09 13:41:50.000000 sleqp-1.0.0/src/sleqp.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-06-09 13:41:50.000000 sleqp-1.0.0/src/sleqp.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       12 2023-06-09 13:41:50.000000 sleqp-1.0.0/src/sleqp.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)        6 2023-06-09 13:41:50.000000 sleqp-1.0.0/src/sleqp.egg-info/top_level.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-26 15:43:33.777397 sleqp-1.0.1/
+-rw-rw-rw-   0 root         (0) root         (0)     7652 2023-04-28 08:35:37.000000 sleqp-1.0.1/LICENSE.txt
+-rw-rw-rw-   0 root         (0) root         (0)       91 2023-06-26 15:30:27.000000 sleqp-1.0.1/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)      673 2023-06-26 15:43:33.777397 sleqp-1.0.1/PKG-INFO
+-rw-rw-rw-   0 root         (0) root         (0)      126 2023-06-26 15:30:27.000000 sleqp-1.0.1/pyproject.toml
+-rw-rw-rw-   0 root         (0) root         (0)       12 2023-06-26 15:30:27.000000 sleqp-1.0.1/requirements.txt
+-rw-r--r--   0 root         (0) root         (0)       38 2023-06-26 15:43:33.777397 sleqp-1.0.1/setup.cfg
+-rw-rw-rw-   0 root         (0) root         (0)     2712 2023-06-26 15:41:31.000000 sleqp-1.0.1/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-26 15:43:33.769397 sleqp-1.0.1/src/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-26 15:43:33.773397 sleqp-1.0.1/src/extension/
+-rw-rw-rw-   0 root         (0) root         (0)     1153 2023-06-26 15:30:27.000000 sleqp-1.0.1/src/extension/call.pxi
+-rw-rw-rw-   0 root         (0) root         (0)     3827 2023-06-26 15:30:27.000000 sleqp-1.0.1/src/extension/callback.pxi
+-rw-rw-rw-   0 root         (0) root         (0)      138 2023-06-26 15:30:27.000000 sleqp-1.0.1/src/extension/cmp.pxi
+-rw-rw-rw-   0 root         (0) root         (0)    26164 2023-06-26 15:30:27.000000 sleqp-1.0.1/src/extension/csleqp.pxd
+-rw-rw-rw-   0 root         (0) root         (0)     6122 2023-06-26 15:30:27.000000 sleqp-1.0.1/src/extension/dyn.pxi
+-rw-rw-rw-   0 root         (0) root         (0)    11800 2023-06-26 15:30:27.000000 sleqp-1.0.1/src/extension/func.pxi
+-rw-rw-rw-   0 root         (0) root         (0)      665 2023-06-26 15:30:27.000000 sleqp-1.0.1/src/extension/gil.pxi
+-rw-rw-rw-   0 root         (0) root         (0)     1896 2023-06-26 15:30:27.000000 sleqp-1.0.1/src/extension/hess_struct.pxi
+-rw-rw-rw-   0 root         (0) root         (0)     1927 2023-06-26 15:30:27.000000 sleqp-1.0.1/src/extension/iterate.pxi
+-rw-rw-rw-   0 root         (0) root         (0)     1696 2023-06-26 15:30:27.000000 sleqp-1.0.1/src/extension/log.pxi
+-rw-rw-rw-   0 root         (0) root         (0)     7709 2023-06-26 15:30:27.000000 sleqp-1.0.1/src/extension/lsq.pxi
+-rw-rw-rw-   0 root         (0) root         (0)    13736 2023-06-26 15:30:27.000000 sleqp-1.0.1/src/extension/problem.pxi
+-rw-rw-rw-   0 root         (0) root         (0)     7172 2023-06-26 15:30:27.000000 sleqp-1.0.1/src/extension/scale.pxi
+-rw-rw-rw-   0 root         (0) root         (0)     7318 2023-06-26 15:30:27.000000 sleqp-1.0.1/src/extension/settings.pxi
+-rw-rw-rw-   0 root         (0) root         (0)      623 2023-06-26 15:30:27.000000 sleqp-1.0.1/src/extension/sleqp.pyx
+-rw-rw-rw-   0 root         (0) root         (0)    11347 2023-06-26 15:30:27.000000 sleqp-1.0.1/src/extension/solver.pxi
+-rw-rw-rw-   0 root         (0) root         (0)     3643 2023-06-26 15:30:27.000000 sleqp-1.0.1/src/extension/sparse.pxi
+-rw-rw-rw-   0 root         (0) root         (0)     1051 2023-06-26 15:30:27.000000 sleqp-1.0.1/src/extension/sparse_matrix.pxi
+-rw-rw-rw-   0 root         (0) root         (0)     6620 2023-06-26 15:30:27.000000 sleqp-1.0.1/src/extension/types.pxi
+-rw-rw-rw-   0 root         (0) root         (0)      229 2023-06-26 15:30:27.000000 sleqp-1.0.1/src/extension/version.pxi
+-rw-rw-rw-   0 root         (0) root         (0)     2960 2023-06-26 15:30:27.000000 sleqp-1.0.1/src/extension/working_set.pxi
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-26 15:43:33.777397 sleqp-1.0.1/src/sleqp/
+-rw-rw-rw-   0 root         (0) root         (0)      101 2023-06-26 15:30:27.000000 sleqp-1.0.1/src/sleqp/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     1323 2023-06-26 15:30:27.000000 sleqp-1.0.1/src/sleqp/_bounds.py
+-rw-rw-rw-   0 root         (0) root         (0)     1696 2023-06-26 15:30:27.000000 sleqp-1.0.1/src/sleqp/_cons.py
+-rw-rw-rw-   0 root         (0) root         (0)     2537 2023-06-26 15:30:27.000000 sleqp-1.0.1/src/sleqp/_cons_func.py
+-rw-rw-rw-   0 root         (0) root         (0)     2139 2023-06-26 15:30:27.000000 sleqp-1.0.1/src/sleqp/_derivative.py
+-rw-rw-rw-   0 root         (0) root         (0)     2113 2023-06-26 15:30:27.000000 sleqp-1.0.1/src/sleqp/_func.py
+-rw-rw-rw-   0 root         (0) root         (0)     3556 2023-06-26 15:30:27.000000 sleqp-1.0.1/src/sleqp/_hessian.py
+-rw-rw-rw-   0 root         (0) root         (0)      948 2023-06-26 15:30:27.000000 sleqp-1.0.1/src/sleqp/_linear.py
+-rw-rw-rw-   0 root         (0) root         (0)     6465 2023-06-26 15:30:27.000000 sleqp-1.0.1/src/sleqp/minimize.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-26 15:43:33.777397 sleqp-1.0.1/src/sleqp.egg-info/
+-rw-r--r--   0 root         (0) root         (0)      673 2023-06-26 15:43:33.000000 sleqp-1.0.1/src/sleqp.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      950 2023-06-26 15:43:33.000000 sleqp-1.0.1/src/sleqp.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-06-26 15:43:33.000000 sleqp-1.0.1/src/sleqp.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       12 2023-06-26 15:43:33.000000 sleqp-1.0.1/src/sleqp.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)        6 2023-06-26 15:43:33.000000 sleqp-1.0.1/src/sleqp.egg-info/top_level.txt
```

### Comparing `sleqp-1.0.0/LICENSE.txt` & `sleqp-1.0.1/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `sleqp-1.0.0/PKG-INFO` & `sleqp-1.0.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sleqp
-Version: 1.0.0
+Version: 1.0.1
 Summary: Active set-based NLP solver
 Author: Christoph Hansknecht
 Author-email: c.hansknecht@tu-braunschweig.de
 Classifier: Programming Language :: Cython
 Classifier: Intended Audience :: Science/Research
 Classifier: Topic :: Scientific/Engineering :: Mathematics
 License-File: LICENSE.txt
```

### Comparing `sleqp-1.0.0/setup.py` & `sleqp-1.0.1/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 import subprocess
 
 import numpy
 
 project_description = 'Active set-based NLP solver'
 long_description = 'This package provides SLEQP, an open-source solver for large-scale nonlinear continuous optimization. SLEQP is available as a callable library with interfaces to C, Python, AMPL, and MATLAB / Octave. It uses an active set method based on a combination of successive linear programming and equality constrained quadratic programming.'
 project_name = 'sleqp'
-project_version = '1.0.0'
+project_version = '1.0.1'
 license_file = 'LICENSE.txt'
 maintainer_name = 'Christoph Hansknecht'
 maintainer_email = 'c.hansknecht@tu-braunschweig.de'
 
 local_env = os.getenv('SLEQP_LOCAL_BUILD')
 local_build = (local_env is not None)
```

### Comparing `sleqp-1.0.0/src/extension/call.pxi` & `sleqp-1.0.1/src/extension/call.pxi`

 * *Files identical despite different names*

### Comparing `sleqp-1.0.0/src/extension/callback.pxi` & `sleqp-1.0.1/src/extension/callback.pxi`

 * *Files identical despite different names*

### Comparing `sleqp-1.0.0/src/extension/csleqp.pxd` & `sleqp-1.0.1/src/extension/csleqp.pxd`

 * *Files identical despite different names*

### Comparing `sleqp-1.0.0/src/extension/dyn.pxi` & `sleqp-1.0.1/src/extension/dyn.pxi`

 * *Files 0% similar despite different names*

```diff
@@ -82,15 +82,15 @@
                                                      const double* cons_weights,
                                                      void* func_data):
   cdef double[:] cons_view
   try:
     func_obj = (<object> func_data)
 
     num_cons = csleqp.sleqp_func_num_cons(func)
-    cons_view = <double[:num_cons]> cons_weights
+    cons_view = _readonly(<double[:num_cons]> cons_weights)
 
     func_obj.set_cons_weights(np.copy(cons_view))
 
   except BaseException as exception:
     store_func_exc(func_obj, exception)
     return csleqp.SLEQP_ERROR
```

### Comparing `sleqp-1.0.0/src/extension/func.pxi` & `sleqp-1.0.1/src/extension/func.pxi`

 * *Files 1% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 cdef csleqp.SLEQP_RETCODE sleqp_func_set(csleqp.SleqpFunc* func,
                                          csleqp.SleqpVec* x,
                                          csleqp.SLEQP_VALUE_REASON reason,
                                          csleqp.bool* reject,
                                          void* func_data):
 
   try:
-    x_array = sleqp_sparse_vec_to_array(x)
+    x_array = _readonly(sleqp_sparse_vec_to_array(x))
 
     func_obj = (<object> func_data)
 
     do_reject = func_obj.set_value(x_array, ValueReason(reason))
 
     if do_reject is True:
       reject[0] = True
@@ -233,16 +233,16 @@
     assert direction
     assert product
 
     func_obj = (<object> func_data)
 
     num_vars = csleqp.sleqp_func_num_vars(func)
 
-    direction_array = sleqp_sparse_vec_to_array(direction)
-    cons_dual_array = sleqp_sparse_vec_to_array(cons_dual)
+    direction_array = _readonly(sleqp_sparse_vec_to_array(direction))
+    cons_dual_array = _readonly(sleqp_sparse_vec_to_array(cons_dual))
 
     product_array = func_obj.hess_prod(direction_array, cons_dual_array)
 
     assert product_array is not None, "hess_prod(...) returned 'None'"
     assert product_array.ndim == 1, "Hessian product must be a vector"
     assert product_array.size == num_vars, "Hessian product has wrong size"
```

### Comparing `sleqp-1.0.0/src/extension/gil.pxi` & `sleqp-1.0.1/src/extension/gil.pxi`

 * *Files identical despite different names*

### Comparing `sleqp-1.0.0/src/extension/hess_struct.pxi` & `sleqp-1.0.1/src/extension/hess_struct.pxi`

 * *Files identical despite different names*

### Comparing `sleqp-1.0.0/src/extension/iterate.pxi` & `sleqp-1.0.1/src/extension/iterate.pxi`

 * *Files identical despite different names*

### Comparing `sleqp-1.0.0/src/extension/log.pxi` & `sleqp-1.0.1/src/extension/log.pxi`

 * *Files identical despite different names*

### Comparing `sleqp-1.0.0/src/extension/lsq.pxi` & `sleqp-1.0.1/src/extension/lsq.pxi`

 * *Files 1% similar despite different names*

```diff
@@ -76,15 +76,15 @@
 cdef csleqp.SLEQP_RETCODE sleqp_lsq_jac_forward(csleqp.SleqpFunc* func,
                                                 const csleqp.SleqpVec* forward_direction,
                                                 csleqp.SleqpVec* product,
                                                 void* func_data):
   try:
       func_obj = (<object> func_data)
 
-      forward_direction_array = sleqp_sparse_vec_to_array(forward_direction)
+      forward_direction_array = _readonly(sleqp_sparse_vec_to_array(forward_direction))
 
       product_array = func_obj.lsq_jac_forward(forward_direction_array)
 
       assert product_array is not None, "lsq_jac_forward(...) returned 'None'"
 
       csleqp_call(array_to_sleqp_sparse_vec(product_array, product))
 
@@ -109,15 +109,15 @@
 cdef csleqp.SLEQP_RETCODE sleqp_lsq_jac_adjoint(csleqp.SleqpFunc* func,
                                                 const csleqp.SleqpVec* adjoint_direction,
                                                 csleqp.SleqpVec* product,
                                                 void* func_data):
   try:
       func_obj = (<object> func_data)
 
-      adjoint_direction_array = sleqp_sparse_vec_to_array(adjoint_direction)
+      adjoint_direction_array = _readonly(sleqp_sparse_vec_to_array(adjoint_direction))
 
       product_array = func_obj.lsq_jac_adjoint(adjoint_direction_array)
 
       assert product_array is not None, "lsq_jac_adjoint(...) returned 'None'"
 
       csleqp_call(array_to_sleqp_sparse_vec(product_array, product))
   except BaseException as exception:
```

### Comparing `sleqp-1.0.0/src/extension/problem.pxi` & `sleqp-1.0.1/src/extension/problem.pxi`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,16 @@
 #cython: language_level=3
 
 
+cdef _readonly(arr):
+    result = arr.view()
+    result.flags.writeable = False
+    return result
+
+
 cdef csleqp.SLEQP_RETCODE create_problem(csleqp.SleqpProblem** problem,
                                          csleqp.SleqpFunc* cfunc,
                                          np.ndarray var_lb,
                                          np.ndarray var_ub,
                                          np.ndarray general_lb,
                                          np.ndarray general_ub,
                                          csleqp.SleqpSettings* csettings,
@@ -182,49 +188,73 @@
     return HessianStruct(self.funcref)
 
   def __dealloc__(self):
     csleqp_call(csleqp.sleqp_problem_release(&self.cproblem))
 
 
 cdef class BaseProblem:
+  """
+  Base class modeling a nonlinear optimization problem (NLP)
+  """
   cdef dict __dict__
 
   cdef object _problem
   cdef object _func
   cdef Settings _settings
 
   def __init__(self, problem):
     self._problem = problem
 
   @property
   def num_vars(self) -> int:
+    """
+    Number of variables in the problem
+    """
     return self._problem.num_vars
 
   @property
   def num_cons(self) -> int:
+    """
+    Number of constraints in the problem
+    """
     return self._problem.num_cons
 
   @property
   def var_lb(self) -> np.array:
-    return self._problem.var_lb
+    """
+    Lower bounds on variables in [-oo, oo)
+    """
+    return _readonly(self._problem.var_lb)
 
   @property
   def var_ub(self) -> np.array:
-    return self._problem.var_ub
+    """
+    Upper bounds on variables in (-oo, oo]
+    """
+    return _readonly(self._problem.var_ub)
 
   @property
   def cons_lb(self) -> np.array:
-    return self._problem.cons_lb
+    """
+    Lower bounds on constraints in [-oo, oo)
+    """
+    return _readonly(self._problem.cons_lb)
 
   @property
   def cons_ub(self) -> np.array:
-    return self._problem.cons_ub
+    """
+    Upper bounds on constraints in (-oo, oo]
+    """
+    return _readonly(self._problem.cons_ub)
 
   @property
   def func(self) -> object:
+    """
+    Underlying (user-provided) nonlinear function
+    """
     return self._func
 
   @property
   def settings(self) -> object:
     return self._settings
 
 
@@ -287,21 +317,29 @@
 
   # Actual arguments processed in __cinit__
   def __init__(self, *args, **kwds):
     super().__init__(self.problem)
 
   @property
   def hess_struct(self) -> HessianStruct:
+    """
+    Block structure of the Hessian matrix
+    """
     return self.problem.hess_struct
 
   def _get_problem(self):
     return self.problem
 
 
 cdef class LSQProblem(BaseProblem):
+  """
+  Class modeling a least-squares (LSQ) problem
+  """
+
+  cdef _Problem problem
   cdef _Func funcref
 
   def __cinit__(self,
                 object func,
                 num_residuals,
                 object var_lb=[],
                 object var_ub=[],
@@ -363,14 +401,21 @@
     super().__init__(self.problem)
 
   def _get_problem(self):
     return self.problem
 
 
 cdef class DynProblem(BaseProblem):
+  """
+  Class modeling a dynamic problem, i.e.,
+  a problem where evaluations have a limited,
+  but controllable accuracy
+  """
+
+  cdef _Problem problem
   cdef _Func funcref
 
   def __cinit__(self,
                 object func,
                 object var_lb=[],
                 object var_ub=[],
                 object cons_lb=[],
@@ -424,11 +469,14 @@
 
   # Actual arguments processed in __cinit__
   def __init__(self, *args, **kwds):
     super().__init__(self.problem)
 
   @property
   def hess_struct(self) -> HessianStruct:
+    """
+    Block structure of the Hessian matrix
+    """
     return self.problem.hess_struct
 
   def _get_problem(self):
     return self.problem
```

### Comparing `sleqp-1.0.0/src/extension/scale.pxi` & `sleqp-1.0.1/src/extension/scale.pxi`

 * *Files 16% similar despite different names*

```diff
@@ -13,14 +13,21 @@
 
   def __array_finalize__(self, obj):
     if obj is None:
       return
     self._token = getattr(obj, '_token', None)
 
 cdef class Scaling:
+  """
+  Scaling of a problem, consisting of weights (powers of 2) for
+  variables, constraints, and objective. Scaling weights can also be
+  given as nominal values, i.e., values which are transformed to ~1 by
+  the scaling.
+
+  """
   cdef dict __dict__
   cdef csleqp.SleqpScaling* scaling
   cdef csleqp.SleqpVec* gradient
   cdef csleqp.SleqpMat* cons_jac
 
   def __cinit__(self,
                 int num_vars,
@@ -38,18 +45,24 @@
     csleqp_call(csleqp.sleqp_mat_create(&self.cons_jac,
                                                   num_cons,
                                                   num_vars,
                                                   0))
 
   @property
   def num_vars(self):
+    """
+    Number of variables in the scaling
+    """
     return csleqp.sleqp_scaling_num_vars(self.scaling)
 
   @property
   def num_cons(self):
+    """
+    Number of constraints in the scaling
+    """
     return csleqp.sleqp_scaling_num_cons(self.scaling)
 
   def __dealloc__(self):
     csleqp_call(csleqp.sleqp_mat_release(&self.cons_jac))
     csleqp_call(csleqp.sleqp_vec_free(&self.gradient))
     csleqp_call(csleqp.sleqp_scaling_release(&self.scaling))
 
@@ -63,39 +76,57 @@
 
     val += "Constraint weights: {0}\n".format(self.variable_weights)
 
     return val
 
   @staticmethod
   def weights_to_nominal_values(weights):
+    """
+    Convert weights to nominal values
+    """
     return np.ldexp(np.ones(weights.shape), weights)
 
   @staticmethod
   def nominal_values_to_weights(nominal_values):
+    """
+    Convert nominal values to weights
+    """
     return np.frexp(nominal_values)[1]
 
   @staticmethod
   def nominal_value_to_weight(nominal_value):
+    """
+    Convert single nominal value to weight
+    """
     return np.frexp(np.array([nominal_value]))[1].item()
 
   @staticmethod
   def weight_to_nominal_value(weight):
+    """
+    Convert single weight to nominal value
+    """
     return np.ldexp(np.ones(1), np.array([weight])).item()
 
   @property
   def obj_weight(self):
+    """
+    Weight of objective
+    """
     return csleqp.sleqp_scaling_obj_weight(self.scaling)
 
   @obj_weight.setter
   def obj_weight(self, value):
     csleqp_call(csleqp.sleqp_scaling_set_obj_weight(self.scaling,
                                                     value))
 
   @property
   def var_weights(self):
+    """
+    Weights of variables
+    """
     length = self.num_vars
     cdef int[:] values = <int[:length]> csleqp.sleqp_scaling_var_weights(self.scaling)
 
     array = np.asarray(values)
     array.flags.writeable = False
 
     return Array(array, self)
@@ -106,14 +137,17 @@
     assert values.dtype == np.int64
 
     for i in range(self.num_vars):
       self.set_variable_weight(i, values[i])
 
   @property
   def cons_weights(self):
+    """
+    Weights of constraints
+    """
     length = self.num_cons
     cdef int[:] values = <int[:length]> csleqp.sleqp_scaling_cons_weights(self.scaling)
 
     array = np.asarray(values)
     array.flags.writeable = False
 
     return Array(array, self)
```

### Comparing `sleqp-1.0.0/src/extension/settings.pxi` & `sleqp-1.0.1/src/extension/settings.pxi`

 * *Files identical despite different names*

### Comparing `sleqp-1.0.0/src/extension/sleqp.pyx` & `sleqp-1.0.1/src/extension/sleqp.pyx`

 * *Files identical despite different names*

### Comparing `sleqp-1.0.0/src/extension/solver.pxi` & `sleqp-1.0.1/src/extension/solver.pxi`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,17 @@
 #cython: language_level=3
 
 from libc.stdlib cimport malloc, free
 
 cdef object solvers = weakref.WeakSet()
 
 cdef class Solver:
-
+  """
+  Solver class for NLP problems
+  """
   cdef dict __dict__
 
   cdef object __weakref__
 
   cdef csleqp.SleqpSolver* solver
   cdef object problem
   cdef csleqp.SleqpVec* residuals
@@ -108,28 +110,40 @@
 
   def info(self) -> str:
     return str(csleqp.sleqp_solver_info(self.solver))
 
   def solve(self,
             max_num_iterations: int = None,
             time_limit: float = None) -> None:
+    """
+    Solve the underlying NLP.
+
+    :param max_num_iterations: Iteration limit, `None` for unlimited
+    :type value: int
+
+    :param time_limit: Time limit, `None` for unlimited
+    :type value: float
+    """
 
     cdef int max_it = csleqp.SLEQP_NONE
     cdef double time = csleqp.SLEQP_NONE
 
     if max_num_iterations is not None:
       max_it = max_num_iterations
 
     if time_limit is not None:
       time = time_limit
 
     self._solve(max_it, time)
 
   @property
   def status(self) -> Status:
+    """
+    Returns status code of last solve
+    """
     return Status(csleqp.sleqp_solver_status(self.solver))
 
   def abort(self):
     """
     Aborts the solver as soon as the current iteration
     finishes.
     """
@@ -167,27 +181,30 @@
       return violated
 
     finally:
       free(violated_cons)
 
   @property
   def solution(self) -> Iterate:
+    """
+    Solution iterate of last call to solve()
+    """
     cdef csleqp.SleqpIterate* _iterate
     cdef Iterate iterate = Iterate(_create=True)
 
     csleqp_call(csleqp.sleqp_solver_solution(self.solver, &_iterate))
 
     iterate._set_iterate(_iterate)
 
     return iterate
 
 
   def add_callback(self, event, function):
     """
-    Adds a callback function to the solver.
+    Adds a callback function to the solver
     """
     cdef CallbackHandle callback_handle = CallbackHandle(self, event, function)
 
     csleqp_call(get_callback_function_pointer(event,
                                               &callback_handle.function_pointer))
 
     csleqp_call(csleqp.sleqp_solver_add_callback(self.solver,
@@ -225,15 +242,17 @@
       csleqp_call(csleqp.sleqp_solver_add_callback(self.solver,
                                                    callback_handle.event.value,
                                                    callback_handle.function_pointer,
                                                    <void*> callback_handle))
 
   @property
   def states(self):
-
+    """
+    Return state of the solver as dict
+    """
     stat_residuals = None
 
     csleqp_call(csleqp.sleqp_solver_vec_state(self.solver,
                                               csleqp.SLEQP_SOLVER_STATE_VEC_SCALED_STAT_RESIDUALS,
                                               self.residuals))
     stat_residuals = sleqp_sparse_vec_to_array(self.residuals)
```

### Comparing `sleqp-1.0.0/src/extension/sparse.pxi` & `sleqp-1.0.1/src/extension/sparse.pxi`

 * *Files identical despite different names*

### Comparing `sleqp-1.0.0/src/extension/sparse_matrix.pxi` & `sleqp-1.0.1/src/extension/sparse_matrix.pxi`

 * *Files identical despite different names*

### Comparing `sleqp-1.0.0/src/extension/types.pxi` & `sleqp-1.0.1/src/extension/types.pxi`

 * *Files identical despite different names*

### Comparing `sleqp-1.0.0/src/sleqp/_bounds.py` & `sleqp-1.0.1/src/sleqp/_bounds.py`

 * *Files identical despite different names*

### Comparing `sleqp-1.0.0/src/sleqp/_cons.py` & `sleqp-1.0.1/src/sleqp/_cons.py`

 * *Files identical despite different names*

### Comparing `sleqp-1.0.0/src/sleqp/_cons_func.py` & `sleqp-1.0.1/src/sleqp/_cons_func.py`

 * *Files identical despite different names*

### Comparing `sleqp-1.0.0/src/sleqp/_derivative.py` & `sleqp-1.0.1/src/sleqp/_derivative.py`

 * *Files identical despite different names*

### Comparing `sleqp-1.0.0/src/sleqp/_func.py` & `sleqp-1.0.1/src/sleqp/_func.py`

 * *Files identical despite different names*

### Comparing `sleqp-1.0.0/src/sleqp/_hessian.py` & `sleqp-1.0.1/src/sleqp/_hessian.py`

 * *Files identical despite different names*

### Comparing `sleqp-1.0.0/src/sleqp/_linear.py` & `sleqp-1.0.1/src/sleqp/_linear.py`

 * *Files identical despite different names*

### Comparing `sleqp-1.0.0/src/sleqp/minimize.py` & `sleqp-1.0.1/src/sleqp/minimize.py`

 * *Files identical despite different names*

### Comparing `sleqp-1.0.0/src/sleqp.egg-info/PKG-INFO` & `sleqp-1.0.1/src/sleqp.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sleqp
-Version: 1.0.0
+Version: 1.0.1
 Summary: Active set-based NLP solver
 Author: Christoph Hansknecht
 Author-email: c.hansknecht@tu-braunschweig.de
 Classifier: Programming Language :: Cython
 Classifier: Intended Audience :: Science/Research
 Classifier: Topic :: Scientific/Engineering :: Mathematics
 License-File: LICENSE.txt
```

### Comparing `sleqp-1.0.0/src/sleqp.egg-info/SOURCES.txt` & `sleqp-1.0.1/src/sleqp.egg-info/SOURCES.txt`

 * *Files identical despite different names*

