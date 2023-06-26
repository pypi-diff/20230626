# Comparing `tmp/openmdao-3.9.1.tar.gz` & `tmp/openmdao-3.9.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "openmdao-3.9.1.tar", last modified: Tue May  4 15:48:01 2021, max compression
+gzip compressed data, was "dist/openmdao-3.9.2.tar", last modified: Fri May 14 19:15:33 2021, max compression
```

## Comparing `openmdao-3.9.1.tar` & `openmdao-3.9.2.tar`

### file list

```diff
@@ -1,640 +1,640 @@
-drwxr-xr-x   0 swryan    (1000) swryan    (1000)        0 2021-05-04 15:48:01.068785 openmdao-3.9.1/
--rw-r--r--   0 swryan    (1000) swryan    (1000)      558 2021-03-09 15:34:37.000000 openmdao-3.9.1/LICENSE.txt
--rw-r--r--   0 swryan    (1000) swryan    (1000)       95 2021-03-09 15:34:37.000000 openmdao-3.9.1/MANIFEST.in
--rw-r--r--   0 swryan    (1000) swryan    (1000)     1496 2021-05-04 15:48:01.068785 openmdao-3.9.1/PKG-INFO
--rw-r--r--   0 swryan    (1000) swryan    (1000)     6252 2021-04-26 14:01:50.000000 openmdao-3.9.1/README.md
-drwxr-xr-x   0 swryan    (1000) swryan    (1000)        0 2021-05-04 15:47:58.632794 openmdao-3.9.1/openmdao/
--rw-r--r--   0 swryan    (1000) swryan    (1000)       42 2021-05-04 14:59:31.000000 openmdao-3.9.1/openmdao/__init__.py
--rw-r--r--   0 swryan    (1000) swryan    (1000)     5348 2021-04-29 15:52:07.000000 openmdao-3.9.1/openmdao/api.py
-drwxr-xr-x   0 swryan    (1000) swryan    (1000)        0 2021-05-04 15:47:58.668793 openmdao-3.9.1/openmdao/approximation_schemes/
--rw-r--r--   0 swryan    (1000) swryan    (1000)        0 2021-03-09 15:34:37.000000 openmdao-3.9.1/openmdao/approximation_schemes/__init__.py
--rw-r--r--   0 swryan    (1000) swryan    (1000)    23805 2021-05-04 13:01:55.000000 openmdao-3.9.1/openmdao/approximation_schemes/approximation_scheme.py
--rw-r--r--   0 swryan    (1000) swryan    (1000)     6836 2021-04-29 15:52:07.000000 openmdao-3.9.1/openmdao/approximation_schemes/complex_step.py
--rw-r--r--   0 swryan    (1000) swryan    (1000)    11165 2021-04-29 15:52:07.000000 openmdao-3.9.1/openmdao/approximation_schemes/finite_difference.py
-drwxr-xr-x   0 swryan    (1000) swryan    (1000)        0 2021-05-04 15:47:58.712793 openmdao-3.9.1/openmdao/code_review/
--rw-r--r--   0 swryan    (1000) swryan    (1000)        0 2021-03-09 15:34:37.000000 openmdao-3.9.1/openmdao/code_review/__init__.py
--rw-r--r--   0 swryan    (1000) swryan    (1000)     9286 2021-04-29 15:52:07.000000 openmdao-3.9.1/openmdao/code_review/test_lint_attributes.py
--rw-r--r--   0 swryan    (1000) swryan    (1000)    21036 2021-04-29 15:52:07.000000 openmdao-3.9.1/openmdao/code_review/test_lint_docstrings.py
--rw-r--r--   0 swryan    (1000) swryan    (1000)     4084 2021-03-15 19:14:32.000000 openmdao-3.9.1/openmdao/code_review/test_lint_peps.py
-drwxr-xr-x   0 swryan    (1000) swryan    (1000)        0 2021-05-04 15:47:58.792793 openmdao-3.9.1/openmdao/components/
--rw-r--r--   0 swryan    (1000) swryan    (1000)        0 2021-03-09 15:34:37.000000 openmdao-3.9.1/openmdao/components/__init__.py
--rw-r--r--   0 swryan    (1000) swryan    (1000)    12200 2021-04-29 15:52:07.000000 openmdao-3.9.1/openmdao/components/add_subtract_comp.py
--rw-r--r--   0 swryan    (1000) swryan    (1000)    15205 2021-04-29 15:52:07.000000 openmdao-3.9.1/openmdao/components/balance_comp.py
--rw-r--r--   0 swryan    (1000) swryan    (1000)     8384 2021-04-29 15:52:07.000000 openmdao-3.9.1/openmdao/components/cross_product_comp.py
--rw-r--r--   0 swryan    (1000) swryan    (1000)     4606 2021-04-29 15:52:07.000000 openmdao-3.9.1/openmdao/components/demux_comp.py
--rw-r--r--   0 swryan    (1000) swryan    (1000)     8552 2021-04-29 15:52:07.000000 openmdao-3.9.1/openmdao/components/dot_product_comp.py
--rw-r--r--   0 swryan    (1000) swryan    (1000)    14605 2021-04-29 15:52:07.000000 openmdao-3.9.1/openmdao/components/eq_constraint_comp.py
--rw-r--r--   0 swryan    (1000) swryan    (1000)    37428 2021-04-29 15:52:07.000000 openmdao-3.9.1/openmdao/components/exec_comp.py
--rw-r--r--   0 swryan    (1000) swryan    (1000)    14528 2021-04-29 15:52:07.000000 openmdao-3.9.1/openmdao/components/external_code_comp.py
-drwxr-xr-x   0 swryan    (1000) swryan    (1000)        0 2021-05-04 15:47:58.884793 openmdao-3.9.1/openmdao/components/interp_util/
--rw-r--r--   0 swryan    (1000) swryan    (1000)        0 2021-03-09 15:34:37.000000 openmdao-3.9.1/openmdao/components/interp_util/__init__.py
--rw-r--r--   0 swryan    (1000) swryan    (1000)    20900 2021-04-29 15:52:07.000000 openmdao-3.9.1/openmdao/components/interp_util/interp.py
--rw-r--r--   0 swryan    (1000) swryan    (1000)    26162 2021-04-29 15:52:07.000000 openmdao-3.9.1/openmdao/components/interp_util/interp_akima.py
--rw-r--r--   0 swryan    (1000) swryan    (1000)     7622 2021-04-29 15:52:07.000000 openmdao-3.9.1/openmdao/components/interp_util/interp_algorithm.py
--rw-r--r--   0 swryan    (1000) swryan    (1000)     6142 2021-04-29 15:52:07.000000 openmdao-3.9.1/openmdao/components/interp_util/interp_bsplines.py
--rw-r--r--   0 swryan    (1000) swryan    (1000)     7049 2021-04-29 15:52:07.000000 openmdao-3.9.1/openmdao/components/interp_util/interp_cubic.py
--rw-r--r--   0 swryan    (1000) swryan    (1000)     4306 2021-04-29 15:52:07.000000 openmdao-3.9.1/openmdao/components/interp_util/interp_lagrange2.py
--rw-r--r--   0 swryan    (1000) swryan    (1000)     5105 2021-04-29 15:52:07.000000 openmdao-3.9.1/openmdao/components/interp_util/interp_lagrange3.py
--rw-r--r--   0 swryan    (1000) swryan    (1000)    11768 2021-04-29 15:52:07.000000 openmdao-3.9.1/openmdao/components/interp_util/interp_scipy.py
--rw-r--r--   0 swryan    (1000) swryan    (1000)     3282 2021-04-29 15:52:07.000000 openmdao-3.9.1/openmdao/components/interp_util/interp_slinear.py
--rw-r--r--   0 swryan    (1000) swryan    (1000)     1253 2021-04-29 15:52:07.000000 openmdao-3.9.1/openmdao/components/interp_util/outofbounds_error.py
-drwxr-xr-x   0 swryan    (1000) swryan    (1000)        0 2021-05-04 15:47:58.884793 openmdao-3.9.1/openmdao/components/interp_util/tests/
--rw-r--r--   0 swryan    (1000) swryan    (1000)        0 2021-03-09 15:34:37.000000 openmdao-3.9.1/openmdao/components/interp_util/tests/__init__.py
--rw-r--r--   0 swryan    (1000) swryan    (1000)    27721 2021-03-15 19:14:32.000000 openmdao-3.9.1/openmdao/components/interp_util/tests/test_interp_nd.py
--rw-r--r--   0 swryan    (1000) swryan    (1000)     8898 2021-04-29 15:52:07.000000 openmdao-3.9.1/openmdao/components/ks_comp.py
--rw-r--r--   0 swryan    (1000) swryan    (1000)     7161 2021-04-29 15:52:07.000000 openmdao-3.9.1/openmdao/components/linear_system_comp.py
--rw-r--r--   0 swryan    (1000) swryan    (1000)     9955 2021-04-29 15:52:07.000000 openmdao-3.9.1/openmdao/components/matrix_vector_product_comp.py
--rw-r--r--   0 swryan    (1000) swryan    (1000)     9638 2021-04-29 15:52:07.000000 openmdao-3.9.1/openmdao/components/meta_model_structured_comp.py
--rw-r--r--   0 swryan    (1000) swryan    (1000)    24465 2021-04-29 15:52:07.000000 openmdao-3.9.1/openmdao/components/meta_model_unstructured_comp.py
--rw-r--r--   0 swryan    (1000) swryan    (1000)    13855 2021-04-29 15:52:07.000000 openmdao-3.9.1/openmdao/components/multifi_meta_model_unstructured_comp.py
--rw-r--r--   0 swryan    (1000) swryan    (1000)     4493 2021-04-29 15:52:07.000000 openmdao-3.9.1/openmdao/components/mux_comp.py
--rw-r--r--   0 swryan    (1000) swryan    (1000)     7569 2021-04-29 15:52:07.000000 openmdao-3.9.1/openmdao/components/spline_comp.py
-drwxr-xr-x   0 swryan    (1000) swryan    (1000)        0 2021-05-04 15:47:58.984792 openmdao-3.9.1/openmdao/components/tests/
--rw-r--r--   0 swryan    (1000) swryan    (1000)        0 2021-03-09 15:34:37.000000 openmdao-3.9.1/openmdao/components/tests/__init__.py
--rw-r--r--   0 swryan    (1000) swryan    (1000)     1240 2021-03-09 15:34:37.000000 openmdao-3.9.1/openmdao/components/tests/extcode_example.py
--rw-r--r--   0 swryan    (1000) swryan    (1000)     2148 2021-03-09 15:34:37.000000 openmdao-3.9.1/openmdao/components/tests/extcode_mach.py
--rw-r--r--   0 swryan    (1000) swryan    (1000)      976 2021-03-09 15:34:37.000000 openmdao-3.9.1/openmdao/components/tests/extcode_node.py
--rw-r--r--   0 swryan    (1000) swryan    (1000)      649 2021-03-09 15:34:37.000000 openmdao-3.9.1/openmdao/components/tests/extcode_paraboloid.py
--rw-r--r--   0 swryan    (1000) swryan    (1000)      988 2021-03-09 15:34:37.000000 openmdao-3.9.1/openmdao/components/tests/extcode_paraboloid_derivs.py
--rw-r--r--   0 swryan    (1000) swryan    (1000)      637 2021-03-09 15:34:37.000000 openmdao-3.9.1/openmdao/components/tests/extcode_resistor.py
--rw-r--r--   0 swryan    (1000) swryan    (1000)    15629 2021-03-09 15:34:37.000000 openmdao-3.9.1/openmdao/components/tests/test_add_subtract_comp.py
--rw-r--r--   0 swryan    (1000) swryan    (1000)    28803 2021-03-09 15:34:37.000000 openmdao-3.9.1/openmdao/components/tests/test_balance_comp.py
--rw-r--r--   0 swryan    (1000) swryan    (1000)    21721 2021-03-09 15:34:37.000000 openmdao-3.9.1/openmdao/components/tests/test_cross_product_comp.py
--rw-r--r--   0 swryan    (1000) swryan    (1000)     6242 2021-03-09 15:34:37.000000 openmdao-3.9.1/openmdao/components/tests/test_demux_comp.py
--rw-r--r--   0 swryan    (1000) swryan    (1000)    21010 2021-03-09 15:34:37.000000 openmdao-3.9.1/openmdao/components/tests/test_dot_product_comp.py
--rw-r--r--   0 swryan    (1000) swryan    (1000)    19831 2021-03-09 15:34:37.000000 openmdao-3.9.1/openmdao/components/tests/test_eq_constraint_comp.py
--rw-r--r--   0 swryan    (1000) swryan    (1000)    70612 2021-04-15 15:43:36.000000 openmdao-3.9.1/openmdao/components/tests/test_exec_comp.py
--rw-r--r--   0 swryan    (1000) swryan    (1000)    22588 2021-03-09 15:34:37.000000 openmdao-3.9.1/openmdao/components/tests/test_external_code_comp.py
--rw-r--r--   0 swryan    (1000) swryan    (1000)    11252 2021-04-15 15:43:36.000000 openmdao-3.9.1/openmdao/components/tests/test_ks_comp.py
--rw-r--r--   0 swryan    (1000) swryan    (1000)    12997 2021-03-09 15:34:37.000000 openmdao-3.9.1/openmdao/components/tests/test_linear_system_comp.py
--rw-r--r--   0 swryan    (1000) swryan    (1000)    23366 2021-03-09 15:34:37.000000 openmdao-3.9.1/openmdao/components/tests/test_matrix_vector_product_comp.py
--rw-r--r--   0 swryan    (1000) swryan    (1000)    54326 2021-03-09 15:34:37.000000 openmdao-3.9.1/openmdao/components/tests/test_meta_model_structured_comp.py
--rw-r--r--   0 swryan    (1000) swryan    (1000)    42560 2021-04-15 15:43:36.000000 openmdao-3.9.1/openmdao/components/tests/test_meta_model_unstructured_comp.py
--rw-r--r--   0 swryan    (1000) swryan    (1000)    19161 2021-03-09 15:34:37.000000 openmdao-3.9.1/openmdao/components/tests/test_multifi_meta_model_unstructured_comp.py
--rw-r--r--   0 swryan    (1000) swryan    (1000)     8581 2021-03-09 15:34:37.000000 openmdao-3.9.1/openmdao/components/tests/test_mux_comp.py
--rw-r--r--   0 swryan    (1000) swryan    (1000)    21876 2021-03-09 15:34:37.000000 openmdao-3.9.1/openmdao/components/tests/test_spline_comp.py
--rw-r--r--   0 swryan    (1000) swryan    (1000)    13083 2021-03-09 15:34:37.000000 openmdao-3.9.1/openmdao/components/tests/test_vector_magnitude_comp.py
--rw-r--r--   0 swryan    (1000) swryan    (1000)     6347 2021-04-29 15:52:07.000000 openmdao-3.9.1/openmdao/components/vector_magnitude_comp.py
-drwxr-xr-x   0 swryan    (1000) swryan    (1000)        0 2021-05-04 15:47:59.008792 openmdao-3.9.1/openmdao/core/
--rw-r--r--   0 swryan    (1000) swryan    (1000)        0 2021-03-09 15:34:37.000000 openmdao-3.9.1/openmdao/core/__init__.py
--rw-r--r--   0 swryan    (1000) swryan    (1000)     1073 2021-04-29 15:52:07.000000 openmdao-3.9.1/openmdao/core/analysis_error.py
--rw-r--r--   0 swryan    (1000) swryan    (1000)    74220 2021-04-29 15:52:07.000000 openmdao-3.9.1/openmdao/core/component.py
--rw-r--r--   0 swryan    (1000) swryan    (1000)     3366 2021-04-29 15:52:07.000000 openmdao-3.9.1/openmdao/core/configinfo.py
--rw-r--r--   0 swryan    (1000) swryan    (1000)     2002 2021-04-29 15:52:07.000000 openmdao-3.9.1/openmdao/core/constants.py
--rw-r--r--   0 swryan    (1000) swryan    (1000)    50500 2021-04-29 15:52:07.000000 openmdao-3.9.1/openmdao/core/driver.py
--rw-r--r--   0 swryan    (1000) swryan    (1000)    22657 2021-04-29 15:52:07.000000 openmdao-3.9.1/openmdao/core/explicitcomponent.py
--rw-r--r--   0 swryan    (1000) swryan    (1000)   162316 2021-04-29 15:52:07.000000 openmdao-3.9.1/openmdao/core/group.py
--rw-r--r--   0 swryan    (1000) swryan    (1000)    22064 2021-04-29 15:52:07.000000 openmdao-3.9.1/openmdao/core/implicitcomponent.py
--rw-r--r--   0 swryan    (1000) swryan    (1000)    13779 2021-04-29 15:52:07.000000 openmdao-3.9.1/openmdao/core/indepvarcomp.py
--rw-r--r--   0 swryan    (1000) swryan    (1000)      550 2021-04-29 15:52:07.000000 openmdao-3.9.1/openmdao/core/parallel_group.py
--rw-r--r--   0 swryan    (1000) swryan    (1000)   108281 2021-04-29 15:52:07.000000 openmdao-3.9.1/openmdao/core/problem.py
--rw-r--r--   0 swryan    (1000) swryan    (1000)   213965 2021-04-29 15:52:07.000000 openmdao-3.9.1/openmdao/core/system.py
-drwxr-xr-x   0 swryan    (1000) swryan    (1000)        0 2021-05-04 15:47:59.400791 openmdao-3.9.1/openmdao/core/tests/
--rw-r--r--   0 swryan    (1000) swryan    (1000)        0 2021-03-09 15:34:37.000000 openmdao-3.9.1/openmdao/core/tests/__init__.py
--rw-r--r--   0 swryan    (1000) swryan    (1000)     7470 2021-03-09 15:34:37.000000 openmdao-3.9.1/openmdao/core/tests/test_add_var.py
--rw-r--r--   0 swryan    (1000) swryan    (1000)    94225 2021-05-04 13:01:55.000000 openmdao-3.9.1/openmdao/core/tests/test_approx_derivs.py
--rw-r--r--   0 swryan    (1000) swryan    (1000)     9367 2021-03-09 15:34:37.000000 openmdao-3.9.1/openmdao/core/tests/test_auto_ivc.py
--rw-r--r--   0 swryan    (1000) swryan    (1000)     1958 2021-03-09 15:34:37.000000 openmdao-3.9.1/openmdao/core/tests/test_aviary_mpi_bug.py
--rw-r--r--   0 swryan    (1000) swryan    (1000)   119893 2021-04-14 16:44:17.000000 openmdao-3.9.1/openmdao/core/tests/test_check_derivs.py
--rw-r--r--   0 swryan    (1000) swryan    (1000)    60518 2021-04-14 16:44:17.000000 openmdao-3.9.1/openmdao/core/tests/test_coloring.py
--rw-r--r--   0 swryan    (1000) swryan    (1000)    13691 2021-04-15 15:43:36.000000 openmdao-3.9.1/openmdao/core/tests/test_component.py
--rw-r--r--   0 swryan    (1000) swryan    (1000)     3535 2021-04-21 12:26:58.000000 openmdao-3.9.1/openmdao/core/tests/test_component_io_independence_from_prob.py
--rw-r--r--   0 swryan    (1000) swryan    (1000)     7689 2021-03-09 15:34:37.000000 openmdao-3.9.1/openmdao/core/tests/test_compute_jacvec_prod.py
--rw-r--r--   0 swryan    (1000) swryan    (1000)    27444 2021-04-15 15:43:36.000000 openmdao-3.9.1/openmdao/core/tests/test_connections.py
--rw-r--r--   0 swryan    (1000) swryan    (1000)     8042 2021-03-09 15:34:37.000000 openmdao-3.9.1/openmdao/core/tests/test_connections_in_configure.py
--rw-r--r--   0 swryan    (1000) swryan    (1000)     3172 2021-03-09 15:34:37.000000 openmdao-3.9.1/openmdao/core/tests/test_core_simple.py
--rw-r--r--   0 swryan    (1000) swryan    (1000)    13666 2021-04-29 15:52:07.000000 openmdao-3.9.1/openmdao/core/tests/test_deriv_transfers.py
--rw-r--r--   0 swryan    (1000) swryan    (1000)    31378 2021-03-09 15:34:37.000000 openmdao-3.9.1/openmdao/core/tests/test_des_vars_responses.py
--rw-r--r--   0 swryan    (1000) swryan    (1000)     2326 2021-03-09 15:34:37.000000 openmdao-3.9.1/openmdao/core/tests/test_direct_nondistrib_comp.py
--rw-r--r--   0 swryan    (1000) swryan    (1000)    31640 2021-04-15 15:43:36.000000 openmdao-3.9.1/openmdao/core/tests/test_discrete.py
--rw-r--r--   0 swryan    (1000) swryan    (1000)     2758 2021-03-09 15:34:37.000000 openmdao-3.9.1/openmdao/core/tests/test_discrete_mpi.py
--rw-r--r--   0 swryan    (1000) swryan    (1000)     3646 2021-04-29 15:52:07.000000 openmdao-3.9.1/openmdao/core/tests/test_distrib_adder.py
--rw-r--r--   0 swryan    (1000) swryan    (1000)    54876 2021-04-29 15:52:07.000000 openmdao-3.9.1/openmdao/core/tests/test_distrib_derivs.py
--rw-r--r--   0 swryan    (1000) swryan    (1000)     4138 2021-03-09 15:34:37.000000 openmdao-3.9.1/openmdao/core/tests/test_distrib_driver_debug_print_options.py
--rw-r--r--   0 swryan    (1000) swryan    (1000)    24450 2021-04-29 15:52:07.000000 openmdao-3.9.1/openmdao/core/tests/test_distrib_list_vars.py
--rw-r--r--   0 swryan    (1000) swryan    (1000)    42588 2021-04-29 15:52:07.000000 openmdao-3.9.1/openmdao/core/tests/test_distribcomp.py
--rw-r--r--   0 swryan    (1000) swryan    (1000)    38606 2021-04-15 15:43:36.000000 openmdao-3.9.1/openmdao/core/tests/test_driver.py
--rw-r--r--   0 swryan    (1000) swryan    (1000)    37491 2021-04-29 15:52:07.000000 openmdao-3.9.1/openmdao/core/tests/test_dyn_sizing.py
--rw-r--r--   0 swryan    (1000) swryan    (1000)    47707 2021-03-15 19:14:32.000000 openmdao-3.9.1/openmdao/core/tests/test_expl_comp.py
--rw-r--r--   0 swryan    (1000) swryan    (1000)    57945 2021-04-29 15:52:08.000000 openmdao-3.9.1/openmdao/core/tests/test_fd_color.py
--rw-r--r--   0 swryan    (1000) swryan    (1000)     3996 2021-03-09 15:34:37.000000 openmdao-3.9.1/openmdao/core/tests/test_fd_color_chk_partials.py
--rw-r--r--   0 swryan    (1000) swryan    (1000)     3630 2021-03-09 15:34:37.000000 openmdao-3.9.1/openmdao/core/tests/test_feature_cache_linear_solution.py
--rw-r--r--   0 swryan    (1000) swryan    (1000)    18289 2021-03-09 15:34:37.000000 openmdao-3.9.1/openmdao/core/tests/test_getset_vars.py
--rw-r--r--   0 swryan    (1000) swryan    (1000)   156775 2021-04-29 15:52:08.000000 openmdao-3.9.1/openmdao/core/tests/test_group.py
--rw-r--r--   0 swryan    (1000) swryan    (1000)    56346 2021-03-15 19:14:32.000000 openmdao-3.9.1/openmdao/core/tests/test_impl_comp.py
--rw-r--r--   0 swryan    (1000) swryan    (1000)     8900 2021-04-15 15:43:36.000000 openmdao-3.9.1/openmdao/core/tests/test_indep_var_comp.py
--rw-r--r--   0 swryan    (1000) swryan    (1000)     2425 2021-03-09 15:34:37.000000 openmdao-3.9.1/openmdao/core/tests/test_leaks.py
--rw-r--r--   0 swryan    (1000) swryan    (1000)     9456 2021-03-09 15:34:37.000000 openmdao-3.9.1/openmdao/core/tests/test_masking.py
--rw-r--r--   0 swryan    (1000) swryan    (1000)    36903 2021-04-22 20:40:02.000000 openmdao-3.9.1/openmdao/core/tests/test_matmat.py
--rw-r--r--   0 swryan    (1000) swryan    (1000)    17354 2021-03-09 15:34:37.000000 openmdao-3.9.1/openmdao/core/tests/test_mpi_coloring_bug.py
--rw-r--r--   0 swryan    (1000) swryan    (1000)     2013 2021-03-09 15:34:37.000000 openmdao-3.9.1/openmdao/core/tests/test_mwe_matmat.py
--rw-r--r--   0 swryan    (1000) swryan    (1000)    36714 2021-03-15 19:14:32.000000 openmdao-3.9.1/openmdao/core/tests/test_parallel_derivatives.py
--rw-r--r--   0 swryan    (1000) swryan    (1000)    18264 2021-03-09 15:34:37.000000 openmdao-3.9.1/openmdao/core/tests/test_parallel_fd.py
--rw-r--r--   0 swryan    (1000) swryan    (1000)    16261 2021-03-09 15:34:37.000000 openmdao-3.9.1/openmdao/core/tests/test_parallel_groups.py
--rw-r--r--   0 swryan    (1000) swryan    (1000)     2790 2021-03-09 15:34:37.000000 openmdao-3.9.1/openmdao/core/tests/test_parallel_src_indices.py
--rw-r--r--   0 swryan    (1000) swryan    (1000)    14694 2021-04-29 15:52:08.000000 openmdao-3.9.1/openmdao/core/tests/test_prob_remote.py
--rw-r--r--   0 swryan    (1000) swryan    (1000)    83460 2021-04-15 15:43:36.000000 openmdao-3.9.1/openmdao/core/tests/test_problem.py
--rw-r--r--   0 swryan    (1000) swryan    (1000)     7293 2021-03-09 15:34:37.000000 openmdao-3.9.1/openmdao/core/tests/test_proc_alloc.py
--rw-r--r--   0 swryan    (1000) swryan    (1000)     2386 2021-03-09 15:34:37.000000 openmdao-3.9.1/openmdao/core/tests/test_remote_vois.py
--rw-r--r--   0 swryan    (1000) swryan    (1000)      951 2021-03-09 15:34:37.000000 openmdao-3.9.1/openmdao/core/tests/test_root_comp_list_outputs.py
--rw-r--r--   0 swryan    (1000) swryan    (1000)    13290 2021-04-29 15:52:08.000000 openmdao-3.9.1/openmdao/core/tests/test_run_root_only.py
--rw-r--r--   0 swryan    (1000) swryan    (1000)    53772 2021-03-15 19:14:32.000000 openmdao-3.9.1/openmdao/core/tests/test_scaling.py
--rw-r--r--   0 swryan    (1000) swryan    (1000)      618 2021-03-15 19:14:32.000000 openmdao-3.9.1/openmdao/core/tests/test_serialize.py
--rw-r--r--   0 swryan    (1000) swryan    (1000)     2049 2021-03-09 15:34:37.000000 openmdao-3.9.1/openmdao/core/tests/test_setup_memleak.py
--rw-r--r--   0 swryan    (1000) swryan    (1000)     3967 2021-03-09 15:34:37.000000 openmdao-3.9.1/openmdao/core/tests/test_simple_impl_comp.py
--rw-r--r--   0 swryan    (1000) swryan    (1000)    15717 2021-03-09 15:34:37.000000 openmdao-3.9.1/openmdao/core/tests/test_src_indices.py
--rw-r--r--   0 swryan    (1000) swryan    (1000)    11342 2021-04-15 15:43:36.000000 openmdao-3.9.1/openmdao/core/tests/test_system.py
--rw-r--r--   0 swryan    (1000) swryan    (1000)    38772 2021-03-25 15:33:56.000000 openmdao-3.9.1/openmdao/core/tests/test_units.py
--rw-r--r--   0 swryan    (1000) swryan    (1000)    78891 2021-04-29 15:52:08.000000 openmdao-3.9.1/openmdao/core/total_jac.py
-drwxr-xr-x   0 swryan    (1000) swryan    (1000)        0 2021-05-04 15:47:59.436791 openmdao-3.9.1/openmdao/devtools/
--rw-r--r--   0 swryan    (1000) swryan    (1000)        0 2021-03-09 15:34:37.000000 openmdao-3.9.1/openmdao/devtools/__init__.py
--rw-r--r--   0 swryan    (1000) swryan    (1000)    18068 2021-04-29 15:52:08.000000 openmdao-3.9.1/openmdao/devtools/debug.py
--rw-r--r--   0 swryan    (1000) swryan    (1000)     4458 2021-03-09 15:34:37.000000 openmdao-3.9.1/openmdao/devtools/dump_sqlite_recorder_file.py
--rw-r--r--   0 swryan    (1000) swryan    (1000)    16162 2021-04-29 15:52:08.000000 openmdao-3.9.1/openmdao/devtools/iprof_mem.py
--rw-r--r--   0 swryan    (1000) swryan    (1000)    11680 2021-04-29 15:52:08.000000 openmdao-3.9.1/openmdao/devtools/iprof_utils.py
--rw-r--r--   0 swryan    (1000) swryan    (1000)    12382 2021-04-29 15:52:08.000000 openmdao-3.9.1/openmdao/devtools/iprofile.py
-drwxr-xr-x   0 swryan    (1000) swryan    (1000)        0 2021-05-04 15:47:59.464791 openmdao-3.9.1/openmdao/devtools/iprofile_app/
--rw-r--r--   0 swryan    (1000) swryan    (1000)        0 2021-03-09 15:34:37.000000 openmdao-3.9.1/openmdao/devtools/iprofile_app/__init__.py
--rw-r--r--   0 swryan    (1000) swryan    (1000)     7990 2021-04-22 20:40:02.000000 openmdao-3.9.1/openmdao/devtools/iprofile_app/iprofile_app.py
-drwxr-xr-x   0 swryan    (1000) swryan    (1000)        0 2021-05-04 15:47:59.464791 openmdao-3.9.1/openmdao/devtools/iprofile_app/templates/
--rw-r--r--   0 swryan    (1000) swryan    (1000)     6206 2021-03-09 15:34:37.000000 openmdao-3.9.1/openmdao/devtools/iprofile_app/templates/iprofview.html
--rw-r--r--   0 swryan    (1000) swryan    (1000)    14101 2021-04-29 15:52:08.000000 openmdao-3.9.1/openmdao/devtools/itrace.py
--rw-r--r--   0 swryan    (1000) swryan    (1000)     9090 2021-04-29 15:52:08.000000 openmdao-3.9.1/openmdao/devtools/memory.py
--rw-r--r--   0 swryan    (1000) swryan    (1000)     1875 2021-03-09 15:34:37.000000 openmdao-3.9.1/openmdao/devtools/run_test.py
-drwxr-xr-x   0 swryan    (1000) swryan    (1000)        0 2021-05-04 15:47:59.484790 openmdao-3.9.1/openmdao/devtools/tests/
--rw-r--r--   0 swryan    (1000) swryan    (1000)        0 2021-03-09 15:34:37.000000 openmdao-3.9.1/openmdao/devtools/tests/__init__.py
--rw-r--r--   0 swryan    (1000) swryan    (1000)      559 2021-03-09 15:34:37.000000 openmdao-3.9.1/openmdao/devtools/tests/mem_model.py
--rw-r--r--   0 swryan    (1000) swryan    (1000)     1901 2021-03-09 15:34:37.000000 openmdao-3.9.1/openmdao/devtools/tests/test_debug.py
--rw-r--r--   0 swryan    (1000) swryan    (1000)     3454 2021-03-09 15:34:37.000000 openmdao-3.9.1/openmdao/devtools/tests/test_iprof_mem.py
--rw-r--r--   0 swryan    (1000) swryan    (1000)     4711 2021-03-09 15:34:37.000000 openmdao-3.9.1/openmdao/devtools/wing_proj_template.wpr
--rw-r--r--   0 swryan    (1000) swryan    (1000)     5361 2021-04-29 15:52:08.000000 openmdao-3.9.1/openmdao/devtools/wingproj.py
-drwxr-xr-x   0 swryan    (1000) swryan    (1000)        0 2021-05-04 15:47:59.528790 openmdao-3.9.1/openmdao/docs/
--rw-r--r--   0 swryan    (1000) swryan    (1000)      324 2021-03-09 15:34:37.000000 openmdao-3.9.1/openmdao/docs/README.md
--rw-r--r--   0 swryan    (1000) swryan    (1000)        0 2021-03-09 15:34:37.000000 openmdao-3.9.1/openmdao/docs/__init__.py
-drwxr-xr-x   0 swryan    (1000) swryan    (1000)        0 2021-05-04 15:47:59.540790 openmdao-3.9.1/openmdao/docs/_exts/
--rw-r--r--   0 swryan    (1000) swryan    (1000)        0 2021-03-09 15:34:37.000000 openmdao-3.9.1/openmdao/docs/_exts/__init__.py
--rw-r--r--   0 swryan    (1000) swryan    (1000)     2021 2021-03-09 15:34:37.000000 openmdao-3.9.1/openmdao/docs/_exts/embed_bibtex.py
--rw-r--r--   0 swryan    (1000) swryan    (1000)    11478 2021-03-25 15:33:56.000000 openmdao-3.9.1/openmdao/docs/_exts/embed_code.py
--rw-r--r--   0 swryan    (1000) swryan    (1000)     4452 2021-03-09 15:34:37.000000 openmdao-3.9.1/openmdao/docs/_exts/embed_compare.py
--rw-r--r--   0 swryan    (1000) swryan    (1000)     3662 2021-03-09 15:34:37.000000 openmdao-3.9.1/openmdao/docs/_exts/embed_n2.py
--rw-r--r--   0 swryan    (1000) swryan    (1000)     2127 2021-03-09 15:34:37.000000 openmdao-3.9.1/openmdao/docs/_exts/embed_options.py
--rw-r--r--   0 swryan    (1000) swryan    (1000)     4891 2021-03-09 15:34:37.000000 openmdao-3.9.1/openmdao/docs/_exts/embed_shell_cmd.py
--rw-r--r--   0 swryan    (1000) swryan    (1000)     3941 2021-03-09 15:34:37.000000 openmdao-3.9.1/openmdao/docs/_exts/link_class_from_docstring.py
--rw-r--r--   0 swryan    (1000) swryan    (1000)     2323 2021-03-09 15:34:37.000000 openmdao-3.9.1/openmdao/docs/_exts/tags.py
-drwxr-xr-x   0 swryan    (1000) swryan    (1000)        0 2021-05-04 15:47:59.556790 openmdao-3.9.1/openmdao/docs/_utils/
--rw-r--r--   0 swryan    (1000) swryan    (1000)        0 2021-03-09 15:34:37.000000 openmdao-3.9.1/openmdao/docs/_utils/__init__.py
--rw-r--r--   0 swryan    (1000) swryan    (1000)    28663 2021-04-29 15:52:08.000000 openmdao-3.9.1/openmdao/docs/_utils/docutil.py
--rw-r--r--   0 swryan    (1000) swryan    (1000)     6222 2021-03-09 15:34:37.000000 openmdao-3.9.1/openmdao/docs/_utils/generate_sourcedocs.py
--rw-r--r--   0 swryan    (1000) swryan    (1000)     4283 2021-03-09 15:34:37.000000 openmdao-3.9.1/openmdao/docs/_utils/patch.py
--rw-r--r--   0 swryan    (1000) swryan    (1000)     3058 2021-03-09 15:34:37.000000 openmdao-3.9.1/openmdao/docs/_utils/preprocess_tags.py
--rw-r--r--   0 swryan    (1000) swryan    (1000)     1251 2021-03-09 15:34:37.000000 openmdao-3.9.1/openmdao/docs/_utils/run_sub.py
--rw-r--r--   0 swryan    (1000) swryan    (1000)     2912 2021-04-22 20:39:54.000000 openmdao-3.9.1/openmdao/docs/_utils/upload_doc_version.py
--rw-r--r--   0 swryan    (1000) swryan    (1000)     5308 2021-03-09 15:34:37.000000 openmdao-3.9.1/openmdao/docs/conf.py
--rw-r--r--   0 swryan    (1000) swryan    (1000)      183 2021-03-09 15:34:37.000000 openmdao-3.9.1/openmdao/docs/config_params.py
--rw-r--r--   0 swryan    (1000) swryan    (1000)      313 2021-03-09 15:34:37.000000 openmdao-3.9.1/openmdao/docs/debug_build_docs.py
--rw-r--r--   0 swryan    (1000) swryan    (1000)      469 2021-03-09 15:34:37.000000 openmdao-3.9.1/openmdao/docutils.py
-drwxr-xr-x   0 swryan    (1000) swryan    (1000)        0 2021-05-04 15:47:59.564790 openmdao-3.9.1/openmdao/drivers/
--rw-r--r--   0 swryan    (1000) swryan    (1000)        0 2021-03-09 15:34:37.000000 openmdao-3.9.1/openmdao/drivers/__init__.py
--rw-r--r--   0 swryan    (1000) swryan    (1000)    22343 2021-04-29 15:52:08.000000 openmdao-3.9.1/openmdao/drivers/differential_evolution_driver.py
--rw-r--r--   0 swryan    (1000) swryan    (1000)     9579 2021-04-29 15:52:08.000000 openmdao-3.9.1/openmdao/drivers/doe_driver.py
--rw-r--r--   0 swryan    (1000) swryan    (1000)    21019 2021-04-29 15:52:08.000000 openmdao-3.9.1/openmdao/drivers/doe_generators.py
--rw-r--r--   0 swryan    (1000) swryan    (1000)    36701 2021-04-29 15:52:08.000000 openmdao-3.9.1/openmdao/drivers/genetic_algorithm_driver.py
--rw-r--r--   0 swryan    (1000) swryan    (1000)    30012 2021-04-29 15:52:08.000000 openmdao-3.9.1/openmdao/drivers/pyoptsparse_driver.py
--rw-r--r--   0 swryan    (1000) swryan    (1000)    32029 2021-04-29 15:52:08.000000 openmdao-3.9.1/openmdao/drivers/scipy_optimizer.py
-drwxr-xr-x   0 swryan    (1000) swryan    (1000)        0 2021-05-04 15:47:59.616790 openmdao-3.9.1/openmdao/drivers/tests/
--rw-r--r--   0 swryan    (1000) swryan    (1000)        0 2021-03-09 15:34:37.000000 openmdao-3.9.1/openmdao/drivers/tests/__init__.py
--rw-r--r--   0 swryan    (1000) swryan    (1000)    36801 2021-04-29 15:52:08.000000 openmdao-3.9.1/openmdao/drivers/tests/test_differential_evolution_driver.py
--rw-r--r--   0 swryan    (1000) swryan    (1000)    82397 2021-04-29 15:52:08.000000 openmdao-3.9.1/openmdao/drivers/tests/test_doe_driver.py
--rw-r--r--   0 swryan    (1000) swryan    (1000)    59486 2021-04-29 15:52:08.000000 openmdao-3.9.1/openmdao/drivers/tests/test_genetic_algorithm_driver.py
--rw-r--r--   0 swryan    (1000) swryan    (1000)    99325 2021-04-29 15:52:08.000000 openmdao-3.9.1/openmdao/drivers/tests/test_pyoptsparse_driver.py
--rw-r--r--   0 swryan    (1000) swryan    (1000)    77763 2021-04-29 15:52:08.000000 openmdao-3.9.1/openmdao/drivers/tests/test_scipy_optimizer.py
-drwxr-xr-x   0 swryan    (1000) swryan    (1000)        0 2021-05-04 15:47:59.624790 openmdao-3.9.1/openmdao/error_checking/
--rw-r--r--   0 swryan    (1000) swryan    (1000)        0 2021-03-09 15:34:37.000000 openmdao-3.9.1/openmdao/error_checking/__init__.py
--rw-r--r--   0 swryan    (1000) swryan    (1000)    22408 2021-04-29 15:52:08.000000 openmdao-3.9.1/openmdao/error_checking/check_config.py
-drwxr-xr-x   0 swryan    (1000) swryan    (1000)        0 2021-05-04 15:47:59.636790 openmdao-3.9.1/openmdao/error_checking/tests/
--rw-r--r--   0 swryan    (1000) swryan    (1000)        0 2021-03-09 15:34:37.000000 openmdao-3.9.1/openmdao/error_checking/tests/__init__.py
--rw-r--r--   0 swryan    (1000) swryan    (1000)    19085 2021-03-09 15:34:37.000000 openmdao-3.9.1/openmdao/error_checking/tests/test_check_config.py
--rw-r--r--   0 swryan    (1000) swryan    (1000)    10886 2021-03-09 15:34:37.000000 openmdao-3.9.1/openmdao/error_checking/tests/test_check_solvers.py
-drwxr-xr-x   0 swryan    (1000) swryan    (1000)        0 2021-05-04 15:47:59.636790 openmdao-3.9.1/openmdao/jacobians/
--rw-r--r--   0 swryan    (1000) swryan    (1000)        0 2021-03-09 15:34:37.000000 openmdao-3.9.1/openmdao/jacobians/__init__.py
--rw-r--r--   0 swryan    (1000) swryan    (1000)    17502 2021-04-29 15:52:08.000000 openmdao-3.9.1/openmdao/jacobians/assembled_jacobian.py
--rw-r--r--   0 swryan    (1000) swryan    (1000)    11249 2021-04-29 15:52:08.000000 openmdao-3.9.1/openmdao/jacobians/dictionary_jacobian.py
--rw-r--r--   0 swryan    (1000) swryan    (1000)    14467 2021-04-29 15:52:08.000000 openmdao-3.9.1/openmdao/jacobians/jacobian.py
-drwxr-xr-x   0 swryan    (1000) swryan    (1000)        0 2021-05-04 15:47:59.640790 openmdao-3.9.1/openmdao/jacobians/tests/
--rw-r--r--   0 swryan    (1000) swryan    (1000)        0 2021-03-09 15:34:37.000000 openmdao-3.9.1/openmdao/jacobians/tests/__init__.py
--rw-r--r--   0 swryan    (1000) swryan    (1000)    43820 2021-04-14 16:44:17.000000 openmdao-3.9.1/openmdao/jacobians/tests/test_jacobian.py
--rw-r--r--   0 swryan    (1000) swryan    (1000)    23098 2021-03-09 15:34:37.000000 openmdao-3.9.1/openmdao/jacobians/tests/test_jacobian_features.py
-drwxr-xr-x   0 swryan    (1000) swryan    (1000)        0 2021-05-04 15:47:59.648790 openmdao-3.9.1/openmdao/matrices/
--rw-r--r--   0 swryan    (1000) swryan    (1000)        0 2021-03-09 15:34:37.000000 openmdao-3.9.1/openmdao/matrices/__init__.py
--rw-r--r--   0 swryan    (1000) swryan    (1000)     9494 2021-04-29 15:52:08.000000 openmdao-3.9.1/openmdao/matrices/coo_matrix.py
--rw-r--r--   0 swryan    (1000) swryan    (1000)     2767 2021-04-29 15:52:08.000000 openmdao-3.9.1/openmdao/matrices/csc_matrix.py
--rw-r--r--   0 swryan    (1000) swryan    (1000)     1154 2021-04-29 15:52:08.000000 openmdao-3.9.1/openmdao/matrices/csr_matrix.py
--rw-r--r--   0 swryan    (1000) swryan    (1000)     3656 2021-04-29 15:52:08.000000 openmdao-3.9.1/openmdao/matrices/dense_matrix.py
--rw-r--r--   0 swryan    (1000) swryan    (1000)     5076 2021-04-29 15:52:08.000000 openmdao-3.9.1/openmdao/matrices/matrix.py
--rw-r--r--   0 swryan    (1000) swryan    (1000)      132 2021-03-09 15:34:37.000000 openmdao-3.9.1/openmdao/parallel_api.py
-drwxr-xr-x   0 swryan    (1000) swryan    (1000)        0 2021-05-04 15:47:59.648790 openmdao-3.9.1/openmdao/proc_allocators/
--rw-r--r--   0 swryan    (1000) swryan    (1000)        0 2021-03-09 15:34:37.000000 openmdao-3.9.1/openmdao/proc_allocators/__init__.py
--rw-r--r--   0 swryan    (1000) swryan    (1000)     5025 2021-04-29 15:52:08.000000 openmdao-3.9.1/openmdao/proc_allocators/default_allocator.py
--rw-r--r--   0 swryan    (1000) swryan    (1000)     4574 2021-04-29 15:52:08.000000 openmdao-3.9.1/openmdao/proc_allocators/proc_allocator.py
-drwxr-xr-x   0 swryan    (1000) swryan    (1000)        0 2021-05-04 15:47:59.656790 openmdao-3.9.1/openmdao/recorders/
--rw-r--r--   0 swryan    (1000) swryan    (1000)        0 2021-03-09 15:34:37.000000 openmdao-3.9.1/openmdao/recorders/__init__.py
--rw-r--r--   0 swryan    (1000) swryan    (1000)     7052 2021-04-29 15:52:08.000000 openmdao-3.9.1/openmdao/recorders/base_case_reader.py
--rw-r--r--   0 swryan    (1000) swryan    (1000)    39848 2021-04-29 15:52:08.000000 openmdao-3.9.1/openmdao/recorders/case.py
--rw-r--r--   0 swryan    (1000) swryan    (1000)      758 2021-04-29 15:52:08.000000 openmdao-3.9.1/openmdao/recorders/case_reader.py
--rw-r--r--   0 swryan    (1000) swryan    (1000)    10625 2021-04-29 15:52:08.000000 openmdao-3.9.1/openmdao/recorders/case_recorder.py
--rw-r--r--   0 swryan    (1000) swryan    (1000)     4837 2021-04-29 15:52:08.000000 openmdao-3.9.1/openmdao/recorders/recording_iteration_stack.py
--rw-r--r--   0 swryan    (1000) swryan    (1000)     9407 2021-04-29 15:52:08.000000 openmdao-3.9.1/openmdao/recorders/recording_manager.py
--rw-r--r--   0 swryan    (1000) swryan    (1000)    63232 2021-04-29 15:52:08.000000 openmdao-3.9.1/openmdao/recorders/sqlite_reader.py
--rw-r--r--   0 swryan    (1000) swryan    (1000)    32982 2021-04-29 15:52:08.000000 openmdao-3.9.1/openmdao/recorders/sqlite_recorder.py
-drwxr-xr-x   0 swryan    (1000) swryan    (1000)        0 2021-05-04 15:47:59.712790 openmdao-3.9.1/openmdao/recorders/tests/
--rw-r--r--   0 swryan    (1000) swryan    (1000)        0 2021-03-09 15:34:37.000000 openmdao-3.9.1/openmdao/recorders/tests/__init__.py
-drwxr-xr-x   0 swryan    (1000) swryan    (1000)        0 2021-05-04 15:47:59.836789 openmdao-3.9.1/openmdao/recorders/tests/legacy_sql/
--rw-r--r--   0 swryan    (1000) swryan    (1000)   122880 2021-03-09 15:34:37.000000 openmdao-3.9.1/openmdao/recorders/tests/legacy_sql/case_database_v4.sql
--rw-r--r--   0 swryan    (1000) swryan    (1000)    33792 2021-03-09 15:34:37.000000 openmdao-3.9.1/openmdao/recorders/tests/legacy_sql/case_driver_01.sql
--rw-r--r--   0 swryan    (1000) swryan    (1000)    61440 2021-03-09 15:34:37.000000 openmdao-3.9.1/openmdao/recorders/tests/legacy_sql/case_driver_pre01.sql
--rw-r--r--   0 swryan    (1000) swryan    (1000)   114688 2021-03-09 15:34:37.000000 openmdao-3.9.1/openmdao/recorders/tests/legacy_sql/case_driver_solver_system_02.sql
--rw-r--r--   0 swryan    (1000) swryan    (1000)   122880 2021-03-09 15:34:37.000000 openmdao-3.9.1/openmdao/recorders/tests/legacy_sql/case_driver_solver_system_03.sql
--rw-r--r--   0 swryan    (1000) swryan    (1000)    73728 2021-03-09 15:34:37.000000 openmdao-3.9.1/openmdao/recorders/tests/legacy_sql/case_driver_v5.sql
--rw-r--r--   0 swryan    (1000) swryan    (1000)    94208 2021-03-09 15:34:37.000000 openmdao-3.9.1/openmdao/recorders/tests/legacy_sql/case_problem_driver_v7.sql
--rw-r--r--   0 swryan    (1000) swryan    (1000)    73728 2021-03-09 15:34:37.000000 openmdao-3.9.1/openmdao/recorders/tests/legacy_sql/case_problem_driver_v8.sql
--rw-r--r--   0 swryan    (1000) swryan    (1000)   102400 2021-03-09 15:34:37.000000 openmdao-3.9.1/openmdao/recorders/tests/legacy_sql/case_problem_v11.sql
--rw-r--r--   0 swryan    (1000) swryan    (1000)    81920 2021-03-09 15:34:37.000000 openmdao-3.9.1/openmdao/recorders/tests/legacy_sql/case_problem_v6.sql
--rw-r--r--   0 swryan    (1000) swryan    (1000)      142 2021-03-09 15:34:37.000000 openmdao-3.9.1/openmdao/recorders/tests/recorder_test_utils.py
--rw-r--r--   0 swryan    (1000) swryan    (1000)    23618 2021-04-14 16:44:17.000000 openmdao-3.9.1/openmdao/recorders/tests/sqlite_recorder_test_utils.py
--rw-r--r--   0 swryan    (1000) swryan    (1000)     9160 2021-04-29 15:52:08.000000 openmdao-3.9.1/openmdao/recorders/tests/test_distrib_sqlite_recorder.py
--rw-r--r--   0 swryan    (1000) swryan    (1000)   185372 2021-04-29 15:52:08.000000 openmdao-3.9.1/openmdao/recorders/tests/test_sqlite_reader.py
--rw-r--r--   0 swryan    (1000) swryan    (1000)   128831 2021-04-29 15:52:08.000000 openmdao-3.9.1/openmdao/recorders/tests/test_sqlite_recorder.py
-drwxr-xr-x   0 swryan    (1000) swryan    (1000)        0 2021-05-04 15:47:59.856789 openmdao-3.9.1/openmdao/solvers/
--rw-r--r--   0 swryan    (1000) swryan    (1000)        0 2021-03-09 15:34:37.000000 openmdao-3.9.1/openmdao/solvers/__init__.py
-drwxr-xr-x   0 swryan    (1000) swryan    (1000)        0 2021-05-04 15:47:59.884789 openmdao-3.9.1/openmdao/solvers/linear/
--rw-r--r--   0 swryan    (1000) swryan    (1000)        0 2021-03-09 15:34:37.000000 openmdao-3.9.1/openmdao/solvers/linear/__init__.py
--rw-r--r--   0 swryan    (1000) swryan    (1000)    15278 2021-04-29 15:52:08.000000 openmdao-3.9.1/openmdao/solvers/linear/direct.py
--rw-r--r--   0 swryan    (1000) swryan    (1000)     8567 2021-04-29 15:52:08.000000 openmdao-3.9.1/openmdao/solvers/linear/linear_block_gs.py
--rw-r--r--   0 swryan    (1000) swryan    (1000)     1778 2021-03-09 15:34:37.000000 openmdao-3.9.1/openmdao/solvers/linear/linear_block_jac.py
--rw-r--r--   0 swryan    (1000) swryan    (1000)     1396 2021-04-29 15:52:08.000000 openmdao-3.9.1/openmdao/solvers/linear/linear_runonce.py
--rw-r--r--   0 swryan    (1000) swryan    (1000)    13874 2021-04-29 15:52:08.000000 openmdao-3.9.1/openmdao/solvers/linear/petsc_ksp.py
--rw-r--r--   0 swryan    (1000) swryan    (1000)     9036 2021-04-29 15:52:08.000000 openmdao-3.9.1/openmdao/solvers/linear/scipy_iter_solver.py
-drwxr-xr-x   0 swryan    (1000) swryan    (1000)        0 2021-05-04 15:47:59.916789 openmdao-3.9.1/openmdao/solvers/linear/tests/
--rw-r--r--   0 swryan    (1000) swryan    (1000)        0 2021-03-09 15:34:37.000000 openmdao-3.9.1/openmdao/solvers/linear/tests/__init__.py
--rw-r--r--   0 swryan    (1000) swryan    (1000)    18631 2021-03-09 15:34:37.000000 openmdao-3.9.1/openmdao/solvers/linear/tests/linear_test_base.py
--rw-r--r--   0 swryan    (1000) swryan    (1000)    38408 2021-04-29 15:52:08.000000 openmdao-3.9.1/openmdao/solvers/linear/tests/test_direct_solver.py
--rw-r--r--   0 swryan    (1000) swryan    (1000)    14387 2021-03-09 15:34:37.000000 openmdao-3.9.1/openmdao/solvers/linear/tests/test_linear_block_gs.py
--rw-r--r--   0 swryan    (1000) swryan    (1000)     7038 2021-03-09 15:34:37.000000 openmdao-3.9.1/openmdao/solvers/linear/tests/test_linear_block_jac.py
--rw-r--r--   0 swryan    (1000) swryan    (1000)     2603 2021-03-09 15:34:37.000000 openmdao-3.9.1/openmdao/solvers/linear/tests/test_linear_runonce.py
--rw-r--r--   0 swryan    (1000) swryan    (1000)    22938 2021-04-29 15:52:08.000000 openmdao-3.9.1/openmdao/solvers/linear/tests/test_petsc_ksp.py
--rw-r--r--   0 swryan    (1000) swryan    (1000)    13076 2021-03-09 15:34:37.000000 openmdao-3.9.1/openmdao/solvers/linear/tests/test_scipy_iter_solver.py
--rw-r--r--   0 swryan    (1000) swryan    (1000)     9846 2021-04-22 20:40:02.000000 openmdao-3.9.1/openmdao/solvers/linear/tests/test_user_defined.py
--rw-r--r--   0 swryan    (1000) swryan    (1000)     2071 2021-04-29 15:52:08.000000 openmdao-3.9.1/openmdao/solvers/linear/user_defined.py
-drwxr-xr-x   0 swryan    (1000) swryan    (1000)        0 2021-05-04 15:47:59.928789 openmdao-3.9.1/openmdao/solvers/linesearch/
--rw-r--r--   0 swryan    (1000) swryan    (1000)        0 2021-03-09 15:34:37.000000 openmdao-3.9.1/openmdao/solvers/linesearch/__init__.py
--rw-r--r--   0 swryan    (1000) swryan    (1000)    20612 2021-04-29 15:52:08.000000 openmdao-3.9.1/openmdao/solvers/linesearch/backtracking.py
-drwxr-xr-x   0 swryan    (1000) swryan    (1000)        0 2021-05-04 15:47:59.936789 openmdao-3.9.1/openmdao/solvers/linesearch/tests/
--rw-r--r--   0 swryan    (1000) swryan    (1000)        0 2021-03-09 15:34:37.000000 openmdao-3.9.1/openmdao/solvers/linesearch/tests/__init__.py
--rw-r--r--   0 swryan    (1000) swryan    (1000)    39454 2021-04-15 15:43:36.000000 openmdao-3.9.1/openmdao/solvers/linesearch/tests/test_backtracking.py
-drwxr-xr-x   0 swryan    (1000) swryan    (1000)        0 2021-05-04 15:47:59.968789 openmdao-3.9.1/openmdao/solvers/nonlinear/
--rw-r--r--   0 swryan    (1000) swryan    (1000)        0 2021-03-09 15:34:37.000000 openmdao-3.9.1/openmdao/solvers/nonlinear/__init__.py
--rw-r--r--   0 swryan    (1000) swryan    (1000)    22501 2021-04-29 15:52:08.000000 openmdao-3.9.1/openmdao/solvers/nonlinear/broyden.py
--rw-r--r--   0 swryan    (1000) swryan    (1000)     9342 2021-04-29 15:52:08.000000 openmdao-3.9.1/openmdao/solvers/nonlinear/newton.py
--rw-r--r--   0 swryan    (1000) swryan    (1000)     9455 2021-04-29 15:52:08.000000 openmdao-3.9.1/openmdao/solvers/nonlinear/nonlinear_block_gs.py
--rw-r--r--   0 swryan    (1000) swryan    (1000)     1603 2021-03-09 15:34:37.000000 openmdao-3.9.1/openmdao/solvers/nonlinear/nonlinear_block_jac.py
--rw-r--r--   0 swryan    (1000) swryan    (1000)     1704 2021-03-09 15:34:37.000000 openmdao-3.9.1/openmdao/solvers/nonlinear/nonlinear_runonce.py
-drwxr-xr-x   0 swryan    (1000) swryan    (1000)        0 2021-05-04 15:47:59.980789 openmdao-3.9.1/openmdao/solvers/nonlinear/tests/
--rw-r--r--   0 swryan    (1000) swryan    (1000)        0 2021-03-09 15:34:37.000000 openmdao-3.9.1/openmdao/solvers/nonlinear/tests/__init__.py
--rw-r--r--   0 swryan    (1000) swryan    (1000)    33153 2021-03-09 15:34:37.000000 openmdao-3.9.1/openmdao/solvers/nonlinear/tests/test_broyden.py
--rw-r--r--   0 swryan    (1000) swryan    (1000)    42253 2021-03-09 15:34:37.000000 openmdao-3.9.1/openmdao/solvers/nonlinear/tests/test_newton.py
--rw-r--r--   0 swryan    (1000) swryan    (1000)    23974 2021-03-09 15:34:37.000000 openmdao-3.9.1/openmdao/solvers/nonlinear/tests/test_nonlinear_block_gs.py
--rw-r--r--   0 swryan    (1000) swryan    (1000)     6642 2021-03-09 15:34:37.000000 openmdao-3.9.1/openmdao/solvers/nonlinear/tests/test_nonlinear_block_jac.py
--rw-r--r--   0 swryan    (1000) swryan    (1000)     3194 2021-03-09 15:34:37.000000 openmdao-3.9.1/openmdao/solvers/nonlinear/tests/test_nonlinear_runonce.py
--rw-r--r--   0 swryan    (1000) swryan    (1000)    36622 2021-04-29 15:52:08.000000 openmdao-3.9.1/openmdao/solvers/solver.py
-drwxr-xr-x   0 swryan    (1000) swryan    (1000)        0 2021-05-04 15:47:59.984789 openmdao-3.9.1/openmdao/solvers/tests/
--rw-r--r--   0 swryan    (1000) swryan    (1000)        0 2021-03-09 15:34:37.000000 openmdao-3.9.1/openmdao/solvers/tests/__init__.py
--rw-r--r--   0 swryan    (1000) swryan    (1000)     8578 2021-03-09 15:34:37.000000 openmdao-3.9.1/openmdao/solvers/tests/test_solver_debug_print.py
--rw-r--r--   0 swryan    (1000) swryan    (1000)     7284 2021-03-09 15:34:37.000000 openmdao-3.9.1/openmdao/solvers/tests/test_solver_features.py
--rw-r--r--   0 swryan    (1000) swryan    (1000)    18116 2021-03-09 15:34:37.000000 openmdao-3.9.1/openmdao/solvers/tests/test_solver_iprint.py
--rw-r--r--   0 swryan    (1000) swryan    (1000)     4686 2021-03-09 15:34:37.000000 openmdao-3.9.1/openmdao/solvers/tests/test_solver_parametric_suite.py
-drwxr-xr-x   0 swryan    (1000) swryan    (1000)        0 2021-05-04 15:48:00.024789 openmdao-3.9.1/openmdao/surrogate_models/
--rw-r--r--   0 swryan    (1000) swryan    (1000)        0 2021-03-09 15:34:37.000000 openmdao-3.9.1/openmdao/surrogate_models/__init__.py
--rw-r--r--   0 swryan    (1000) swryan    (1000)    12532 2021-04-29 15:52:08.000000 openmdao-3.9.1/openmdao/surrogate_models/kriging.py
--rw-r--r--   0 swryan    (1000) swryan    (1000)    40845 2021-04-29 15:52:08.000000 openmdao-3.9.1/openmdao/surrogate_models/multifi_cokriging.py
--rw-r--r--   0 swryan    (1000) swryan    (1000)     3485 2021-04-29 15:52:08.000000 openmdao-3.9.1/openmdao/surrogate_models/nearest_neighbor.py
-drwxr-xr-x   0 swryan    (1000) swryan    (1000)        0 2021-05-04 15:48:00.044789 openmdao-3.9.1/openmdao/surrogate_models/nn_interpolators/
--rw-r--r--   0 swryan    (1000) swryan    (1000)        0 2021-03-09 15:34:37.000000 openmdao-3.9.1/openmdao/surrogate_models/nn_interpolators/__init__.py
--rw-r--r--   0 swryan    (1000) swryan    (1000)     5319 2021-04-29 15:52:08.000000 openmdao-3.9.1/openmdao/surrogate_models/nn_interpolators/linear_interpolator.py
--rw-r--r--   0 swryan    (1000) swryan    (1000)     3156 2021-04-29 15:52:08.000000 openmdao-3.9.1/openmdao/surrogate_models/nn_interpolators/nn_base.py
--rw-r--r--   0 swryan    (1000) swryan    (1000)    18609 2021-04-29 15:52:08.000000 openmdao-3.9.1/openmdao/surrogate_models/nn_interpolators/rbf_interpolator.py
--rw-r--r--   0 swryan    (1000) swryan    (1000)     5305 2021-04-29 15:52:08.000000 openmdao-3.9.1/openmdao/surrogate_models/nn_interpolators/weighted_interpolator.py
--rw-r--r--   0 swryan    (1000) swryan    (1000)     3563 2021-04-29 15:52:08.000000 openmdao-3.9.1/openmdao/surrogate_models/response_surface.py
--rw-r--r--   0 swryan    (1000) swryan    (1000)     3244 2021-04-29 15:52:08.000000 openmdao-3.9.1/openmdao/surrogate_models/surrogate_model.py
-drwxr-xr-x   0 swryan    (1000) swryan    (1000)        0 2021-05-04 15:48:00.064788 openmdao-3.9.1/openmdao/surrogate_models/tests/
--rw-r--r--   0 swryan    (1000) swryan    (1000)        0 2021-03-09 15:34:37.000000 openmdao-3.9.1/openmdao/surrogate_models/tests/__init__.py
--rw-r--r--   0 swryan    (1000) swryan    (1000)     5683 2021-04-22 20:40:02.000000 openmdao-3.9.1/openmdao/surrogate_models/tests/test_kriging.py
--rw-r--r--   0 swryan    (1000) swryan    (1000)     2641 2021-03-09 15:34:37.000000 openmdao-3.9.1/openmdao/surrogate_models/tests/test_map.py
--rw-r--r--   0 swryan    (1000) swryan    (1000)    11356 2021-03-09 15:34:37.000000 openmdao-3.9.1/openmdao/surrogate_models/tests/test_multifi_cokriging.py
--rw-r--r--   0 swryan    (1000) swryan    (1000)    15590 2021-03-09 15:34:37.000000 openmdao-3.9.1/openmdao/surrogate_models/tests/test_nearest_neighbor.py
--rw-r--r--   0 swryan    (1000) swryan    (1000)     3861 2021-03-09 15:34:37.000000 openmdao-3.9.1/openmdao/surrogate_models/tests/test_response_surface.py
-drwxr-xr-x   0 swryan    (1000) swryan    (1000)        0 2021-05-04 15:48:00.084788 openmdao-3.9.1/openmdao/test_suite/
--rw-r--r--   0 swryan    (1000) swryan    (1000)        0 2021-03-09 15:34:37.000000 openmdao-3.9.1/openmdao/test_suite/__init__.py
--rw-r--r--   0 swryan    (1000) swryan    (1000)     4033 2021-03-09 15:34:37.000000 openmdao-3.9.1/openmdao/test_suite/build4test.py
-drwxr-xr-x   0 swryan    (1000) swryan    (1000)        0 2021-05-04 15:48:00.184788 openmdao-3.9.1/openmdao/test_suite/components/
--rw-r--r--   0 swryan    (1000) swryan    (1000)        0 2021-03-09 15:34:37.000000 openmdao-3.9.1/openmdao/test_suite/components/__init__.py
--rw-r--r--   0 swryan    (1000) swryan    (1000)      846 2021-03-09 15:34:37.000000 openmdao-3.9.1/openmdao/test_suite/components/ae_tests.py
--rw-r--r--   0 swryan    (1000) swryan    (1000)     1203 2021-03-09 15:34:37.000000 openmdao-3.9.1/openmdao/test_suite/components/array_comp.py
--rw-r--r--   0 swryan    (1000) swryan    (1000)     3309 2021-03-09 15:34:37.000000 openmdao-3.9.1/openmdao/test_suite/components/branin.py
--rw-r--r--   0 swryan    (1000) swryan    (1000)    17441 2021-03-09 15:34:37.000000 openmdao-3.9.1/openmdao/test_suite/components/cycle_comps.py
--rw-r--r--   0 swryan    (1000) swryan    (1000)     3918 2021-03-09 15:34:37.000000 openmdao-3.9.1/openmdao/test_suite/components/distributed_components.py
--rw-r--r--   0 swryan    (1000) swryan    (1000)     2446 2021-03-09 15:34:37.000000 openmdao-3.9.1/openmdao/test_suite/components/double_sellar.py
--rw-r--r--   0 swryan    (1000) swryan    (1000)     1879 2021-03-09 15:34:37.000000 openmdao-3.9.1/openmdao/test_suite/components/eggcrate.py
--rw-r--r--   0 swryan    (1000) swryan    (1000)     3000 2021-04-29 15:52:08.000000 openmdao-3.9.1/openmdao/test_suite/components/exec_comp_for_test.py
--rw-r--r--   0 swryan    (1000) swryan    (1000)     3084 2021-04-29 15:52:08.000000 openmdao-3.9.1/openmdao/test_suite/components/expl_comp_array.py
--rw-r--r--   0 swryan    (1000) swryan    (1000)     1767 2021-04-29 15:52:08.000000 openmdao-3.9.1/openmdao/test_suite/components/expl_comp_simple.py
--rw-r--r--   0 swryan    (1000) swryan    (1000)     2036 2021-04-29 15:52:08.000000 openmdao-3.9.1/openmdao/test_suite/components/impl_comp_array.py
--rw-r--r--   0 swryan    (1000) swryan    (1000)     1831 2021-03-09 15:34:37.000000 openmdao-3.9.1/openmdao/test_suite/components/impl_comp_simple.py
--rw-r--r--   0 swryan    (1000) swryan    (1000)     3869 2021-04-29 15:52:08.000000 openmdao-3.9.1/openmdao/test_suite/components/implicit_newton_linesearch.py
--rw-r--r--   0 swryan    (1000) swryan    (1000)     1974 2021-03-09 15:34:37.000000 openmdao-3.9.1/openmdao/test_suite/components/matmultcomp.py
--rw-r--r--   0 swryan    (1000) swryan    (1000)     2130 2021-03-09 15:34:37.000000 openmdao-3.9.1/openmdao/test_suite/components/misc_components.py
--rw-r--r--   0 swryan    (1000) swryan    (1000)      624 2021-03-09 15:34:37.000000 openmdao-3.9.1/openmdao/test_suite/components/options_feature_array.py
--rw-r--r--   0 swryan    (1000) swryan    (1000)      585 2021-03-09 15:34:37.000000 openmdao-3.9.1/openmdao/test_suite/components/options_feature_function.py
--rw-r--r--   0 swryan    (1000) swryan    (1000)      661 2021-03-09 15:34:37.000000 openmdao-3.9.1/openmdao/test_suite/components/options_feature_lincomb.py
--rw-r--r--   0 swryan    (1000) swryan    (1000)      727 2021-03-09 15:34:37.000000 openmdao-3.9.1/openmdao/test_suite/components/options_feature_vector.py
--rw-r--r--   0 swryan    (1000) swryan    (1000)     1642 2021-03-09 15:34:37.000000 openmdao-3.9.1/openmdao/test_suite/components/paraboloid.py
--rw-r--r--   0 swryan    (1000) swryan    (1000)     4305 2021-03-09 15:34:37.000000 openmdao-3.9.1/openmdao/test_suite/components/paraboloid_distributed.py
--rw-r--r--   0 swryan    (1000) swryan    (1000)     1178 2021-03-09 15:34:37.000000 openmdao-3.9.1/openmdao/test_suite/components/paraboloid_feature.py
--rw-r--r--   0 swryan    (1000) swryan    (1000)      938 2021-03-09 15:34:37.000000 openmdao-3.9.1/openmdao/test_suite/components/paraboloid_mat_vec.py
--rw-r--r--   0 swryan    (1000) swryan    (1000)      787 2021-03-09 15:34:37.000000 openmdao-3.9.1/openmdao/test_suite/components/paraboloid_problem.py
--rw-r--r--   0 swryan    (1000) swryan    (1000)     1029 2021-03-09 15:34:37.000000 openmdao-3.9.1/openmdao/test_suite/components/partial_check_feature.py
--rw-r--r--   0 swryan    (1000) swryan    (1000)     1242 2021-03-09 15:34:37.000000 openmdao-3.9.1/openmdao/test_suite/components/quad_implicit.py
--rw-r--r--   0 swryan    (1000) swryan    (1000)    25297 2021-03-09 15:34:37.000000 openmdao-3.9.1/openmdao/test_suite/components/sellar.py
--rw-r--r--   0 swryan    (1000) swryan    (1000)    13262 2021-03-09 15:34:37.000000 openmdao-3.9.1/openmdao/test_suite/components/sellar_feature.py
--rw-r--r--   0 swryan    (1000) swryan    (1000)     2774 2021-03-09 15:34:37.000000 openmdao-3.9.1/openmdao/test_suite/components/simple_comps.py
--rw-r--r--   0 swryan    (1000) swryan    (1000)     7196 2021-03-09 15:34:37.000000 openmdao-3.9.1/openmdao/test_suite/components/three_bar_truss.py
--rw-r--r--   0 swryan    (1000) swryan    (1000)     5815 2021-03-09 15:34:37.000000 openmdao-3.9.1/openmdao/test_suite/components/unit_conv.py
-drwxr-xr-x   0 swryan    (1000) swryan    (1000)        0 2021-05-04 15:48:00.216788 openmdao-3.9.1/openmdao/test_suite/groups/
--rw-r--r--   0 swryan    (1000) swryan    (1000)        0 2021-03-09 15:34:37.000000 openmdao-3.9.1/openmdao/test_suite/groups/__init__.py
--rw-r--r--   0 swryan    (1000) swryan    (1000)     7879 2021-04-29 15:52:08.000000 openmdao-3.9.1/openmdao/test_suite/groups/cycle_group.py
--rw-r--r--   0 swryan    (1000) swryan    (1000)     3395 2021-03-09 15:34:37.000000 openmdao-3.9.1/openmdao/test_suite/groups/implicit_group.py
--rw-r--r--   0 swryan    (1000) swryan    (1000)    11058 2021-03-09 15:34:37.000000 openmdao-3.9.1/openmdao/test_suite/groups/parallel_groups.py
--rw-r--r--   0 swryan    (1000) swryan    (1000)     1925 2021-03-09 15:34:37.000000 openmdao-3.9.1/openmdao/test_suite/groups/parametric_group.py
--rw-r--r--   0 swryan    (1000) swryan    (1000)    10603 2021-04-29 15:52:08.000000 openmdao-3.9.1/openmdao/test_suite/groups/sin_fitter.py
-drwxr-xr-x   0 swryan    (1000) swryan    (1000)        0 2021-05-04 15:48:00.376788 openmdao-3.9.1/openmdao/test_suite/matrices/
--rw-r--r--   0 swryan    (1000) swryan    (1000)    13814 2021-03-09 15:34:37.000000 openmdao-3.9.1/openmdao/test_suite/matrices/D_6.npz
--rw-r--r--   0 swryan    (1000) swryan    (1000)     3697 2021-03-09 15:34:37.000000 openmdao-3.9.1/openmdao/test_suite/matrices/Harvard500.npz
--rw-r--r--   0 swryan    (1000) swryan    (1000)    39084 2021-03-09 15:34:37.000000 openmdao-3.9.1/openmdao/test_suite/matrices/af23560.npz
--rw-r--r--   0 swryan    (1000) swryan    (1000)     2136 2021-03-09 15:34:37.000000 openmdao-3.9.1/openmdao/test_suite/matrices/ash331.npz
--rw-r--r--   0 swryan    (1000) swryan    (1000)     3156 2021-03-09 15:34:37.000000 openmdao-3.9.1/openmdao/test_suite/matrices/ash608.npz
--rw-r--r--   0 swryan    (1000) swryan    (1000)     7459 2021-03-09 15:34:37.000000 openmdao-3.9.1/openmdao/test_suite/matrices/bibd_12_5.npz
--rw-r--r--   0 swryan    (1000) swryan    (1000)     7073 2021-03-09 15:34:37.000000 openmdao-3.9.1/openmdao/test_suite/matrices/can_715.npz
--rw-r--r--   0 swryan    (1000) swryan    (1000)     1660 2021-03-09 15:34:37.000000 openmdao-3.9.1/openmdao/test_suite/matrices/color_mats.py
--rw-r--r--   0 swryan    (1000) swryan    (1000)      653 2021-03-09 15:34:37.000000 openmdao-3.9.1/openmdao/test_suite/matrices/dl_matrix.py
--rw-r--r--   0 swryan    (1000) swryan    (1000)  2765232 2021-03-09 15:34:37.000000 openmdao-3.9.1/openmdao/test_suite/matrices/e40r0100.npz
--rw-r--r--   0 swryan    (1000) swryan    (1000)    21447 2021-03-09 15:34:37.000000 openmdao-3.9.1/openmdao/test_suite/matrices/illc1033.npz
--rw-r--r--   0 swryan    (1000) swryan    (1000)    40384 2021-03-09 15:34:37.000000 openmdao-3.9.1/openmdao/test_suite/matrices/lp_cre_a.npz
--rw-r--r--   0 swryan    (1000) swryan    (1000)    93861 2021-03-09 15:34:37.000000 openmdao-3.9.1/openmdao/test_suite/matrices/lp_dfl001.npz
--rw-r--r--   0 swryan    (1000) swryan    (1000)     9350 2021-03-09 15:34:37.000000 openmdao-3.9.1/openmdao/test_suite/matrices/lp_finnis.npz
--rw-r--r--   0 swryan    (1000) swryan    (1000)    81939 2021-03-09 15:34:37.000000 openmdao-3.9.1/openmdao/test_suite/matrices/lp_maros_r7.npz
--rw-r--r--   0 swryan    (1000) swryan    (1000)    37978 2021-03-09 15:34:37.000000 openmdao-3.9.1/openmdao/test_suite/matrices/m3plates.npz
--rw-r--r--   0 swryan    (1000) swryan    (1000)      878 2021-03-09 15:34:37.000000 openmdao-3.9.1/openmdao/test_suite/matrices/ml2np.py
--rw-r--r--   0 swryan    (1000) swryan    (1000)     3048 2021-03-09 15:34:37.000000 openmdao-3.9.1/openmdao/test_suite/matrices/n4c6-b15.npz
--rw-r--r--   0 swryan    (1000) swryan    (1000)     8236 2021-03-09 15:34:37.000000 openmdao-3.9.1/openmdao/test_suite/parametric_suite.py
-drwxr-xr-x   0 swryan    (1000) swryan    (1000)        0 2021-05-04 15:48:00.396788 openmdao-3.9.1/openmdao/test_suite/scripts/
--rw-r--r--   0 swryan    (1000) swryan    (1000)        0 2021-03-09 15:34:37.000000 openmdao-3.9.1/openmdao/test_suite/scripts/__init__.py
--rw-r--r--   0 swryan    (1000) swryan    (1000)      685 2021-03-09 15:34:37.000000 openmdao-3.9.1/openmdao/test_suite/scripts/bad_connection.py
--rw-r--r--   0 swryan    (1000) swryan    (1000)     1231 2021-03-09 15:34:37.000000 openmdao-3.9.1/openmdao/test_suite/scripts/beam_opt.py
--rw-r--r--   0 swryan    (1000) swryan    (1000)      351 2021-03-09 15:34:37.000000 openmdao-3.9.1/openmdao/test_suite/scripts/circle_coloring_dynpartials.py
--rw-r--r--   0 swryan    (1000) swryan    (1000)      503 2021-03-09 15:34:37.000000 openmdao-3.9.1/openmdao/test_suite/scripts/circle_coloring_needs_args.py
--rw-r--r--   0 swryan    (1000) swryan    (1000)     3407 2021-03-09 15:34:37.000000 openmdao-3.9.1/openmdao/test_suite/scripts/circle_opt.py
--rw-r--r--   0 swryan    (1000) swryan    (1000)     1530 2021-03-09 15:34:37.000000 openmdao-3.9.1/openmdao/test_suite/scripts/circuit.py
--rw-r--r--   0 swryan    (1000) swryan    (1000)     5818 2021-03-09 15:34:37.000000 openmdao-3.9.1/openmdao/test_suite/scripts/circuit_analysis.py
--rw-r--r--   0 swryan    (1000) swryan    (1000)     1692 2021-03-09 15:34:37.000000 openmdao-3.9.1/openmdao/test_suite/scripts/circuit_with_unconnected_input.py
--rw-r--r--   0 swryan    (1000) swryan    (1000)     1412 2021-03-09 15:34:37.000000 openmdao-3.9.1/openmdao/test_suite/scripts/dyn_system.py
--rw-r--r--   0 swryan    (1000) swryan    (1000)     1988 2021-03-09 15:34:37.000000 openmdao-3.9.1/openmdao/test_suite/scripts/multipoint_beam_opt.py
--rw-r--r--   0 swryan    (1000) swryan    (1000)     2078 2021-03-09 15:34:37.000000 openmdao-3.9.1/openmdao/test_suite/scripts/sellar.py
-drwxr-xr-x   0 swryan    (1000) swryan    (1000)        0 2021-05-04 15:48:00.416787 openmdao-3.9.1/openmdao/test_suite/test_examples/
--rw-r--r--   0 swryan    (1000) swryan    (1000)        0 2021-03-09 15:34:37.000000 openmdao-3.9.1/openmdao/test_suite/test_examples/__init__.py
--rw-r--r--   0 swryan    (1000) swryan    (1000)     2866 2021-03-09 15:34:37.000000 openmdao-3.9.1/openmdao/test_suite/test_examples/basic_opt_paraboloid.py
-drwxr-xr-x   0 swryan    (1000) swryan    (1000)        0 2021-05-04 15:48:00.436787 openmdao-3.9.1/openmdao/test_suite/test_examples/beam_optimization/
--rw-r--r--   0 swryan    (1000) swryan    (1000)        0 2021-03-09 15:34:37.000000 openmdao-3.9.1/openmdao/test_suite/test_examples/beam_optimization/__init__.py
--rw-r--r--   0 swryan    (1000) swryan    (1000)     2290 2021-03-09 15:34:37.000000 openmdao-3.9.1/openmdao/test_suite/test_examples/beam_optimization/beam_group.py
-drwxr-xr-x   0 swryan    (1000) swryan    (1000)        0 2021-05-04 15:48:00.460787 openmdao-3.9.1/openmdao/test_suite/test_examples/beam_optimization/components/
--rw-r--r--   0 swryan    (1000) swryan    (1000)        0 2021-03-09 15:34:37.000000 openmdao-3.9.1/openmdao/test_suite/test_examples/beam_optimization/components/__init__.py
--rw-r--r--   0 swryan    (1000) swryan    (1000)      821 2021-03-09 15:34:37.000000 openmdao-3.9.1/openmdao/test_suite/test_examples/beam_optimization/components/compliance_comp.py
--rw-r--r--   0 swryan    (1000) swryan    (1000)     1315 2021-03-09 15:34:37.000000 openmdao-3.9.1/openmdao/test_suite/test_examples/beam_optimization/components/local_stiffness_matrix_comp.py
--rw-r--r--   0 swryan    (1000) swryan    (1000)      776 2021-03-09 15:34:37.000000 openmdao-3.9.1/openmdao/test_suite/test_examples/beam_optimization/components/moment_comp.py
--rw-r--r--   0 swryan    (1000) swryan    (1000)     1099 2021-03-09 15:34:37.000000 openmdao-3.9.1/openmdao/test_suite/test_examples/beam_optimization/components/multi_compliance_comp.py
--rw-r--r--   0 swryan    (1000) swryan    (1000)     4462 2021-03-09 15:34:37.000000 openmdao-3.9.1/openmdao/test_suite/test_examples/beam_optimization/components/multi_states_comp.py
--rw-r--r--   0 swryan    (1000) swryan    (1000)     1946 2021-03-09 15:34:37.000000 openmdao-3.9.1/openmdao/test_suite/test_examples/beam_optimization/components/multi_stress_comp.py
--rw-r--r--   0 swryan    (1000) swryan    (1000)     3776 2021-03-09 15:34:37.000000 openmdao-3.9.1/openmdao/test_suite/test_examples/beam_optimization/components/states_comp.py
--rw-r--r--   0 swryan    (1000) swryan    (1000)      733 2021-03-09 15:34:37.000000 openmdao-3.9.1/openmdao/test_suite/test_examples/beam_optimization/components/volume_comp.py
--rw-r--r--   0 swryan    (1000) swryan    (1000)     4936 2021-04-29 15:52:08.000000 openmdao-3.9.1/openmdao/test_suite/test_examples/beam_optimization/multipoint_beam_group.py
--rw-r--r--   0 swryan    (1000) swryan    (1000)     5707 2021-04-29 15:52:08.000000 openmdao-3.9.1/openmdao/test_suite/test_examples/beam_optimization/multipoint_beam_stress.py
--rw-r--r--   0 swryan    (1000) swryan    (1000)     9208 2021-03-09 15:34:37.000000 openmdao-3.9.1/openmdao/test_suite/test_examples/beam_optimization/test_beam_optimization.py
-drwxr-xr-x   0 swryan    (1000) swryan    (1000)        0 2021-05-04 15:48:00.476787 openmdao-3.9.1/openmdao/test_suite/test_examples/cannonball/
--rw-r--r--   0 swryan    (1000) swryan    (1000)        0 2021-03-09 15:34:37.000000 openmdao-3.9.1/openmdao/test_suite/test_examples/cannonball/__init__.py
--rw-r--r--   0 swryan    (1000) swryan    (1000)     4958 2021-03-09 15:34:37.000000 openmdao-3.9.1/openmdao/test_suite/test_examples/cannonball/cannonball_ode.py
--rw-r--r--   0 swryan    (1000) swryan    (1000)     4107 2021-04-29 15:52:08.000000 openmdao-3.9.1/openmdao/test_suite/test_examples/cannonball/test_euler_integration.py
-drwxr-xr-x   0 swryan    (1000) swryan    (1000)        0 2021-05-04 15:48:00.476787 openmdao-3.9.1/openmdao/test_suite/test_examples/meta_model_examples/
--rw-r--r--   0 swryan    (1000) swryan    (1000)        0 2021-03-09 15:34:37.000000 openmdao-3.9.1/openmdao/test_suite/test_examples/meta_model_examples/__init__.py
--rw-r--r--   0 swryan    (1000) swryan    (1000)     2076 2021-03-09 15:34:37.000000 openmdao-3.9.1/openmdao/test_suite/test_examples/meta_model_examples/structured_meta_model_example.py
--rw-r--r--   0 swryan    (1000) swryan    (1000)      711 2021-03-09 15:34:37.000000 openmdao-3.9.1/openmdao/test_suite/test_examples/meta_model_examples/unstructured_meta_model_example.py
--rw-r--r--   0 swryan    (1000) swryan    (1000)    13847 2021-03-09 15:34:37.000000 openmdao-3.9.1/openmdao/test_suite/test_examples/test_betz_limit.py
--rw-r--r--   0 swryan    (1000) swryan    (1000)     9895 2021-03-09 15:34:37.000000 openmdao-3.9.1/openmdao/test_suite/test_examples/test_circuit_analysis.py
--rw-r--r--   0 swryan    (1000) swryan    (1000)     6027 2021-03-09 15:34:37.000000 openmdao-3.9.1/openmdao/test_suite/test_examples/test_circuit_analysis_derivs.py
--rw-r--r--   0 swryan    (1000) swryan    (1000)     7020 2021-03-09 15:34:37.000000 openmdao-3.9.1/openmdao/test_suite/test_examples/test_hohmann_transfer.py
--rw-r--r--   0 swryan    (1000) swryan    (1000)     1882 2021-03-09 15:34:37.000000 openmdao-3.9.1/openmdao/test_suite/test_examples/test_keplers_equation.py
--rw-r--r--   0 swryan    (1000) swryan    (1000)     8345 2021-03-09 15:34:37.000000 openmdao-3.9.1/openmdao/test_suite/test_examples/test_sellar_mda_promote_connect.py
--rw-r--r--   0 swryan    (1000) swryan    (1000)     1338 2021-03-09 15:34:37.000000 openmdao-3.9.1/openmdao/test_suite/test_examples/test_sellar_opt.py
--rw-r--r--   0 swryan    (1000) swryan    (1000)     1304 2021-03-09 15:34:37.000000 openmdao-3.9.1/openmdao/test_suite/test_examples/test_tldr_paraboloid.py
-drwxr-xr-x   0 swryan    (1000) swryan    (1000)        0 2021-05-04 15:48:00.480787 openmdao-3.9.1/openmdao/test_suite/tests/
--rw-r--r--   0 swryan    (1000) swryan    (1000)        0 2021-03-09 15:34:37.000000 openmdao-3.9.1/openmdao/test_suite/tests/__init__.py
--rw-r--r--   0 swryan    (1000) swryan    (1000)     7063 2021-03-09 15:34:37.000000 openmdao-3.9.1/openmdao/test_suite/tests/test_auto_ivc_api_conversion.py
--rw-r--r--   0 swryan    (1000) swryan    (1000)     1721 2021-03-09 15:34:37.000000 openmdao-3.9.1/openmdao/test_suite/tests/test_feature_sellar.py
--rw-r--r--   0 swryan    (1000) swryan    (1000)     4106 2021-03-09 15:34:37.000000 openmdao-3.9.1/openmdao/test_suite/tests/test_general.py
--rw-r--r--   0 swryan    (1000) swryan    (1000)      785 2021-03-09 15:34:37.000000 openmdao-3.9.1/openmdao/test_suite/tests/test_paraboloid_feature.py
--rw-r--r--   0 swryan    (1000) swryan    (1000)     1074 2021-03-09 15:34:37.000000 openmdao-3.9.1/openmdao/test_suite/tests/test_quad_implicit.py
--rw-r--r--   0 swryan    (1000) swryan    (1000)     5169 2021-04-15 15:43:36.000000 openmdao-3.9.1/openmdao/test_suite/tests/test_warnings.py
--rw-r--r--   0 swryan    (1000) swryan    (1000)     7545 2021-03-09 15:34:37.000000 openmdao-3.9.1/openmdao/test_suite/tot_jac_builder.py
-drwxr-xr-x   0 swryan    (1000) swryan    (1000)        0 2021-05-04 15:48:00.520787 openmdao-3.9.1/openmdao/utils/
--rw-r--r--   0 swryan    (1000) swryan    (1000)        0 2021-03-09 15:34:37.000000 openmdao-3.9.1/openmdao/utils/__init__.py
--rw-r--r--   0 swryan    (1000) swryan    (1000)    14141 2021-04-29 15:52:08.000000 openmdao-3.9.1/openmdao/utils/array_utils.py
--rw-r--r--   0 swryan    (1000) swryan    (1000)    19537 2021-04-29 15:52:08.000000 openmdao-3.9.1/openmdao/utils/assert_utils.py
--rw-r--r--   0 swryan    (1000) swryan    (1000)     1908 2021-04-29 15:52:08.000000 openmdao-3.9.1/openmdao/utils/class_util.py
--rw-r--r--   0 swryan    (1000) swryan    (1000)     8895 2021-04-29 15:52:08.000000 openmdao-3.9.1/openmdao/utils/code_utils.py
--rw-r--r--   0 swryan    (1000) swryan    (1000)    85853 2021-04-29 15:52:08.000000 openmdao-3.9.1/openmdao/utils/coloring.py
--rw-r--r--   0 swryan    (1000) swryan    (1000)     7329 2021-04-29 15:52:08.000000 openmdao-3.9.1/openmdao/utils/concurrent.py
--rw-r--r--   0 swryan    (1000) swryan    (1000)     1484 2021-04-29 15:52:08.000000 openmdao-3.9.1/openmdao/utils/cs_safe.py
--rw-r--r--   0 swryan    (1000) swryan    (1000)    14605 2021-04-29 15:52:08.000000 openmdao-3.9.1/openmdao/utils/entry_points.py
--rw-r--r--   0 swryan    (1000) swryan    (1000)     7490 2021-04-29 15:52:08.000000 openmdao-3.9.1/openmdao/utils/file_utils.py
--rw-r--r--   0 swryan    (1000) swryan    (1000)    33963 2021-04-29 15:52:08.000000 openmdao-3.9.1/openmdao/utils/file_wrap.py
--rw-r--r--   0 swryan    (1000) swryan    (1000)     3182 2021-04-29 15:52:08.000000 openmdao-3.9.1/openmdao/utils/find_cite.py
--rw-r--r--   0 swryan    (1000) swryan    (1000)    33705 2021-04-29 15:52:08.000000 openmdao-3.9.1/openmdao/utils/general_utils.py
--rw-r--r--   0 swryan    (1000) swryan    (1000)     1240 2021-04-29 15:52:08.000000 openmdao-3.9.1/openmdao/utils/graph_utils.py
--rw-r--r--   0 swryan    (1000) swryan    (1000)     5872 2021-04-29 15:52:08.000000 openmdao-3.9.1/openmdao/utils/hooks.py
--rw-r--r--   0 swryan    (1000) swryan    (1000)     6426 2021-04-29 15:52:08.000000 openmdao-3.9.1/openmdao/utils/logger_utils.py
--rw-r--r--   0 swryan    (1000) swryan    (1000)     8783 2021-04-29 15:52:08.000000 openmdao-3.9.1/openmdao/utils/mpi.py
--rw-r--r--   0 swryan    (1000) swryan    (1000)     8628 2021-04-29 15:52:08.000000 openmdao-3.9.1/openmdao/utils/name_maps.py
--rw-r--r--   0 swryan    (1000) swryan    (1000)     3451 2021-04-29 15:52:08.000000 openmdao-3.9.1/openmdao/utils/notebook_utils.py
--rw-r--r--   0 swryan    (1000) swryan    (1000)    23346 2021-04-29 15:52:08.000000 openmdao-3.9.1/openmdao/utils/om.py
--rw-r--r--   0 swryan    (1000) swryan    (1000)    16517 2021-04-29 15:52:08.000000 openmdao-3.9.1/openmdao/utils/options_dictionary.py
--rw-r--r--   0 swryan    (1000) swryan    (1000)     6572 2021-04-29 15:52:08.000000 openmdao-3.9.1/openmdao/utils/record_util.py
--rw-r--r--   0 swryan    (1000) swryan    (1000)     6355 2021-04-29 15:52:08.000000 openmdao-3.9.1/openmdao/utils/scaffold.py
-drwxr-xr-x   0 swryan    (1000) swryan    (1000)        0 2021-05-04 15:48:00.556787 openmdao-3.9.1/openmdao/utils/scaffolding_templates/
--rw-r--r--   0 swryan    (1000) swryan    (1000)     3600 2021-03-09 15:34:37.000000 openmdao-3.9.1/openmdao/utils/scaffolding_templates/BaseCaseReader_template
--rw-r--r--   0 swryan    (1000) swryan    (1000)     4303 2021-03-09 15:34:37.000000 openmdao-3.9.1/openmdao/utils/scaffolding_templates/CaseRecorder_template
--rw-r--r--   0 swryan    (1000) swryan    (1000)     2635 2021-03-09 15:34:37.000000 openmdao-3.9.1/openmdao/utils/scaffolding_templates/Driver_template
--rw-r--r--   0 swryan    (1000) swryan    (1000)     1814 2021-03-09 15:34:37.000000 openmdao-3.9.1/openmdao/utils/scaffolding_templates/ExplicitComponent_template
--rw-r--r--   0 swryan    (1000) swryan    (1000)     1031 2021-03-09 15:34:37.000000 openmdao-3.9.1/openmdao/utils/scaffolding_templates/Group_template
--rw-r--r--   0 swryan    (1000) swryan    (1000)     3888 2021-03-09 15:34:37.000000 openmdao-3.9.1/openmdao/utils/scaffolding_templates/ImplicitComponent_template
--rw-r--r--   0 swryan    (1000) swryan    (1000)     1928 2021-03-09 15:34:37.000000 openmdao-3.9.1/openmdao/utils/scaffolding_templates/LinearSolver_template
--rw-r--r--   0 swryan    (1000) swryan    (1000)     1836 2021-03-09 15:34:37.000000 openmdao-3.9.1/openmdao/utils/scaffolding_templates/NonlinearSolver_template
--rw-r--r--   0 swryan    (1000) swryan    (1000)       31 2021-03-09 15:34:37.000000 openmdao-3.9.1/openmdao/utils/scaffolding_templates/README_template
--rw-r--r--   0 swryan    (1000) swryan    (1000)     2122 2021-03-09 15:34:37.000000 openmdao-3.9.1/openmdao/utils/scaffolding_templates/SurrogateModel_template
--rw-r--r--   0 swryan    (1000) swryan    (1000)     2265 2021-03-09 15:34:37.000000 openmdao-3.9.1/openmdao/utils/scaffolding_templates/command_template
--rw-r--r--   0 swryan    (1000) swryan    (1000)       78 2021-03-09 15:34:37.000000 openmdao-3.9.1/openmdao/utils/scaffolding_templates/setup_template
--rw-r--r--   0 swryan    (1000) swryan    (1000)      569 2021-03-09 15:34:37.000000 openmdao-3.9.1/openmdao/utils/scaffolding_templates/test_template
--rw-r--r--   0 swryan    (1000) swryan    (1000)    11980 2021-04-29 15:52:08.000000 openmdao-3.9.1/openmdao/utils/shell_proc.py
--rw-r--r--   0 swryan    (1000) swryan    (1000)     1646 2021-04-29 15:52:08.000000 openmdao-3.9.1/openmdao/utils/spline_distributions.py
--rw-r--r--   0 swryan    (1000) swryan    (1000)     2541 2021-04-29 15:52:08.000000 openmdao-3.9.1/openmdao/utils/testing_utils.py
-drwxr-xr-x   0 swryan    (1000) swryan    (1000)        0 2021-05-04 15:48:00.684786 openmdao-3.9.1/openmdao/utils/tests/
--rw-r--r--   0 swryan    (1000) swryan    (1000)        0 2021-03-09 15:34:37.000000 openmdao-3.9.1/openmdao/utils/tests/__init__.py
--rw-r--r--   0 swryan    (1000) swryan    (1000)     2198 2021-03-09 15:34:37.000000 openmdao-3.9.1/openmdao/utils/tests/test_array_utils.py
--rw-r--r--   0 swryan    (1000) swryan    (1000)     6027 2021-03-09 15:34:37.000000 openmdao-3.9.1/openmdao/utils/tests/test_assert_utils.py
--rw-r--r--   0 swryan    (1000) swryan    (1000)     6058 2021-04-15 15:43:36.000000 openmdao-3.9.1/openmdao/utils/tests/test_cmdline.py
--rw-r--r--   0 swryan    (1000) swryan    (1000)      586 2021-03-09 15:34:37.000000 openmdao-3.9.1/openmdao/utils/tests/test_code_utils.py
--rw-r--r--   0 swryan    (1000) swryan    (1000)     1739 2021-03-09 15:34:37.000000 openmdao-3.9.1/openmdao/utils/tests/test_cs_safe.py
--rw-r--r--   0 swryan    (1000) swryan    (1000)     2738 2021-03-09 15:34:37.000000 openmdao-3.9.1/openmdao/utils/tests/test_entry_points.py
--rw-r--r--   0 swryan    (1000) swryan    (1000)    29602 2021-03-09 15:34:37.000000 openmdao-3.9.1/openmdao/utils/tests/test_file_wrap.py
--rw-r--r--   0 swryan    (1000) swryan    (1000)     6922 2021-03-09 15:34:37.000000 openmdao-3.9.1/openmdao/utils/tests/test_find_citations.py
--rw-r--r--   0 swryan    (1000) swryan    (1000)     1213 2021-03-09 15:34:37.000000 openmdao-3.9.1/openmdao/utils/tests/test_general_utils.py
--rw-r--r--   0 swryan    (1000) swryan    (1000)     3087 2021-03-09 15:34:37.000000 openmdao-3.9.1/openmdao/utils/tests/test_hooks.py
--rw-r--r--   0 swryan    (1000) swryan    (1000)    13748 2021-04-15 15:43:36.000000 openmdao-3.9.1/openmdao/utils/tests/test_options_dictionary.py
--rw-r--r--   0 swryan    (1000) swryan    (1000)     4553 2021-03-09 15:34:37.000000 openmdao-3.9.1/openmdao/utils/tests/test_options_dictionary_feature.py
--rw-r--r--   0 swryan    (1000) swryan    (1000)     3425 2021-03-09 15:34:37.000000 openmdao-3.9.1/openmdao/utils/tests/test_scaffold.py
--rw-r--r--   0 swryan    (1000) swryan    (1000)     2946 2021-03-09 15:34:37.000000 openmdao-3.9.1/openmdao/utils/tests/test_shell_proc.py
--rw-r--r--   0 swryan    (1000) swryan    (1000)     2695 2021-03-09 15:34:37.000000 openmdao-3.9.1/openmdao/utils/tests/test_spline_distributions.py
--rw-r--r--   0 swryan    (1000) swryan    (1000)    13877 2021-04-15 15:43:36.000000 openmdao-3.9.1/openmdao/utils/tests/test_units.py
--rw-r--r--   0 swryan    (1000) swryan    (1000)    23342 2021-04-29 15:52:08.000000 openmdao-3.9.1/openmdao/utils/tests/test_vartable.py
--rw-r--r--   0 swryan    (1000) swryan    (1000)    10063 2021-03-09 15:34:37.000000 openmdao-3.9.1/openmdao/utils/tests/test_visualization.py
--rw-r--r--   0 swryan    (1000) swryan    (1000)     6031 2021-03-09 15:34:37.000000 openmdao-3.9.1/openmdao/utils/unit_library.ini
--rw-r--r--   0 swryan    (1000) swryan    (1000)    32876 2021-04-29 15:52:08.000000 openmdao-3.9.1/openmdao/utils/units.py
--rw-r--r--   0 swryan    (1000) swryan    (1000)    11179 2021-04-29 15:52:08.000000 openmdao-3.9.1/openmdao/utils/variable_table.py
--rw-r--r--   0 swryan    (1000) swryan    (1000)      645 2021-04-29 15:52:08.000000 openmdao-3.9.1/openmdao/utils/webview.py
-drwxr-xr-x   0 swryan    (1000) swryan    (1000)        0 2021-05-04 15:48:00.692786 openmdao-3.9.1/openmdao/vectors/
--rw-r--r--   0 swryan    (1000) swryan    (1000)        0 2021-03-09 15:34:37.000000 openmdao-3.9.1/openmdao/vectors/__init__.py
--rw-r--r--   0 swryan    (1000) swryan    (1000)    11203 2021-04-29 15:52:08.000000 openmdao-3.9.1/openmdao/vectors/default_transfer.py
--rw-r--r--   0 swryan    (1000) swryan    (1000)    12476 2021-05-04 13:01:55.000000 openmdao-3.9.1/openmdao/vectors/default_vector.py
--rw-r--r--   0 swryan    (1000) swryan    (1000)    14420 2021-04-29 15:52:08.000000 openmdao-3.9.1/openmdao/vectors/petsc_transfer.py
--rw-r--r--   0 swryan    (1000) swryan    (1000)     7753 2021-04-29 15:52:08.000000 openmdao-3.9.1/openmdao/vectors/petsc_vector.py
-drwxr-xr-x   0 swryan    (1000) swryan    (1000)        0 2021-05-04 15:48:00.696786 openmdao-3.9.1/openmdao/vectors/tests/
--rw-r--r--   0 swryan    (1000) swryan    (1000)        0 2021-03-09 15:34:37.000000 openmdao-3.9.1/openmdao/vectors/tests/__init__.py
--rw-r--r--   0 swryan    (1000) swryan    (1000)     7768 2021-04-29 15:52:08.000000 openmdao-3.9.1/openmdao/vectors/tests/test_vector.py
--rw-r--r--   0 swryan    (1000) swryan    (1000)     1803 2021-04-29 15:52:08.000000 openmdao-3.9.1/openmdao/vectors/transfer.py
--rw-r--r--   0 swryan    (1000) swryan    (1000)    17850 2021-04-29 15:52:08.000000 openmdao-3.9.1/openmdao/vectors/vector.py
-drwxr-xr-x   0 swryan    (1000) swryan    (1000)        0 2021-05-04 15:48:00.724786 openmdao-3.9.1/openmdao/visualization/
--rw-r--r--   0 swryan    (1000) swryan    (1000)        0 2021-03-09 15:34:37.000000 openmdao-3.9.1/openmdao/visualization/__init__.py
-drwxr-xr-x   0 swryan    (1000) swryan    (1000)        0 2021-05-04 15:47:58.564794 openmdao-3.9.1/openmdao/visualization/common/
-drwxr-xr-x   0 swryan    (1000) swryan    (1000)        0 2021-05-04 15:48:00.768786 openmdao-3.9.1/openmdao/visualization/common/libs/
--rw-r--r--   0 swryan    (1000) swryan    (1000)   267993 2021-03-09 15:34:37.000000 openmdao-3.9.1/openmdao/visualization/common/libs/d3.v6.min.js
--rw-r--r--   0 swryan    (1000) swryan    (1000)   106266 2021-03-09 15:34:37.000000 openmdao-3.9.1/openmdao/visualization/common/libs/jquery-3.4.1.min.js
--rw-r--r--   0 swryan    (1000) swryan    (1000)   359216 2021-03-09 15:34:37.000000 openmdao-3.9.1/openmdao/visualization/common/libs/tabulator.min.js
-drwxr-xr-x   0 swryan    (1000) swryan    (1000)        0 2021-05-04 15:48:00.784786 openmdao-3.9.1/openmdao/visualization/common/style/
--rwxr-xr-x   0 swryan    (1000) swryan    (1000)    22678 2021-03-09 15:34:37.000000 openmdao-3.9.1/openmdao/visualization/common/style/tabulator.min.css
-drwxr-xr-x   0 swryan    (1000) swryan    (1000)        0 2021-05-04 15:48:00.820786 openmdao-3.9.1/openmdao/visualization/connection_viewer/
--rw-r--r--   0 swryan    (1000) swryan    (1000)        0 2021-03-09 15:34:37.000000 openmdao-3.9.1/openmdao/visualization/connection_viewer/__init__.py
--rw-r--r--   0 swryan    (1000) swryan    (1000)     5952 2021-03-09 15:34:37.000000 openmdao-3.9.1/openmdao/visualization/connection_viewer/connect_table.html
-drwxr-xr-x   0 swryan    (1000) swryan    (1000)        0 2021-05-04 15:48:00.824786 openmdao-3.9.1/openmdao/visualization/connection_viewer/tests/
--rw-r--r--   0 swryan    (1000) swryan    (1000)        0 2021-03-09 15:34:37.000000 openmdao-3.9.1/openmdao/visualization/connection_viewer/tests/__init__.py
--rw-r--r--   0 swryan    (1000) swryan    (1000)     1933 2021-04-30 12:56:59.000000 openmdao-3.9.1/openmdao/visualization/connection_viewer/tests/test_viewconns.py
--rw-r--r--   0 swryan    (1000) swryan    (1000)     6789 2021-04-30 12:56:59.000000 openmdao-3.9.1/openmdao/visualization/connection_viewer/viewconns.py
--rw-r--r--   0 swryan    (1000) swryan    (1000)     5225 2021-04-29 15:52:08.000000 openmdao-3.9.1/openmdao/visualization/dyn_shape_plot.py
--rw-r--r--   0 swryan    (1000) swryan    (1000)    18850 2021-04-29 15:52:08.000000 openmdao-3.9.1/openmdao/visualization/html_utils.py
-drwxr-xr-x   0 swryan    (1000) swryan    (1000)        0 2021-05-04 15:48:00.824786 openmdao-3.9.1/openmdao/visualization/meta_model_viewer/
--rw-r--r--   0 swryan    (1000) swryan    (1000)        0 2021-03-09 15:34:37.000000 openmdao-3.9.1/openmdao/visualization/meta_model_viewer/__init__.py
--rw-r--r--   0 swryan    (1000) swryan    (1000)    38980 2021-04-29 15:52:08.000000 openmdao-3.9.1/openmdao/visualization/meta_model_viewer/meta_model_visualization.py
-drwxr-xr-x   0 swryan    (1000) swryan    (1000)        0 2021-05-04 15:48:00.868786 openmdao-3.9.1/openmdao/visualization/meta_model_viewer/tests/
--rw-r--r--   0 swryan    (1000) swryan    (1000)        0 2021-03-09 15:34:37.000000 openmdao-3.9.1/openmdao/visualization/meta_model_viewer/tests/__init__.py
--rw-r--r--   0 swryan    (1000) swryan    (1000)      800 2021-03-09 15:34:37.000000 openmdao-3.9.1/openmdao/visualization/meta_model_viewer/tests/example.py
-drwxr-xr-x   0 swryan    (1000) swryan    (1000)        0 2021-05-04 15:48:00.880786 openmdao-3.9.1/openmdao/visualization/meta_model_viewer/tests/known_data_point_files/
--rw-r--r--   0 swryan    (1000) swryan    (1000)      968 2021-03-09 15:34:37.000000 openmdao-3.9.1/openmdao/visualization/meta_model_viewer/tests/known_data_point_files/test_five_alpha_points.csv
--rw-r--r--   0 swryan    (1000) swryan    (1000)     2763 2021-03-09 15:34:37.000000 openmdao-3.9.1/openmdao/visualization/meta_model_viewer/tests/known_data_point_files/unstructured_data_points.csv
--rw-r--r--   0 swryan    (1000) swryan    (1000)     2524 2021-03-09 15:34:37.000000 openmdao-3.9.1/openmdao/visualization/meta_model_viewer/tests/known_data_point_files/unstructured_test_points_bottom.csv
--rw-r--r--   0 swryan    (1000) swryan    (1000)     2481 2021-03-09 15:34:37.000000 openmdao-3.9.1/openmdao/visualization/meta_model_viewer/tests/known_data_point_files/unstructured_test_points_right.csv
--rw-r--r--   0 swryan    (1000) swryan    (1000)     5430 2021-03-09 15:34:37.000000 openmdao-3.9.1/openmdao/visualization/meta_model_viewer/tests/known_data_point_files/updated_scatter_distance.csv
--rw-r--r--   0 swryan    (1000) swryan    (1000)     1321 2021-03-09 15:34:37.000000 openmdao-3.9.1/openmdao/visualization/meta_model_viewer/tests/multiple_metamodels.py
--rw-r--r--   0 swryan    (1000) swryan    (1000)    20179 2021-03-09 15:34:37.000000 openmdao-3.9.1/openmdao/visualization/meta_model_viewer/tests/test_structured.py
--rw-r--r--   0 swryan    (1000) swryan    (1000)    12216 2021-03-09 15:34:37.000000 openmdao-3.9.1/openmdao/visualization/meta_model_viewer/tests/test_unstruct.py
--rw-r--r--   0 swryan    (1000) swryan    (1000)     1463 2021-03-09 15:34:37.000000 openmdao-3.9.1/openmdao/visualization/meta_model_viewer/tests/test_view_mm_cmd_line.py
-drwxr-xr-x   0 swryan    (1000) swryan    (1000)        0 2021-05-04 15:48:00.884786 openmdao-3.9.1/openmdao/visualization/n2_viewer/
--rw-r--r--   0 swryan    (1000) swryan    (1000)        0 2021-03-09 15:34:37.000000 openmdao-3.9.1/openmdao/visualization/n2_viewer/__init__.py
-drwxr-xr-x   0 swryan    (1000) swryan    (1000)        0 2021-05-04 15:48:00.888786 openmdao-3.9.1/openmdao/visualization/n2_viewer/assets/
--rw-r--r--   0 swryan    (1000) swryan    (1000)    13359 2021-03-09 15:34:37.000000 openmdao-3.9.1/openmdao/visualization/n2_viewer/assets/logo.png
--rw-r--r--   0 swryan    (1000) swryan    (1000)    15592 2021-03-15 19:14:32.000000 openmdao-3.9.1/openmdao/visualization/n2_viewer/assets/n2toolbar_screenshot_png.b64
--rw-r--r--   0 swryan    (1000) swryan    (1000)    91128 2021-03-09 15:34:37.000000 openmdao-3.9.1/openmdao/visualization/n2_viewer/assets/spinner.png
--rw-r--r--   0 swryan    (1000) swryan    (1000)    14095 2021-04-14 16:44:17.000000 openmdao-3.9.1/openmdao/visualization/n2_viewer/index.html
-drwxr-xr-x   0 swryan    (1000) swryan    (1000)        0 2021-05-04 15:48:00.908786 openmdao-3.9.1/openmdao/visualization/n2_viewer/libs/
--rw-r--r--   0 swryan    (1000) swryan    (1000)     9483 2021-03-09 15:34:37.000000 openmdao-3.9.1/openmdao/visualization/n2_viewer/libs/awesomplete.js
--rw-r--r--   0 swryan    (1000) swryan    (1000)   511371 2021-03-09 15:34:37.000000 openmdao-3.9.1/openmdao/visualization/n2_viewer/libs/d3.js
--rw-r--r--   0 swryan    (1000) swryan    (1000)   246120 2021-03-09 15:34:37.000000 openmdao-3.9.1/openmdao/visualization/n2_viewer/libs/d3.v5.min.js
--rw-r--r--   0 swryan    (1000) swryan    (1000)    31305 2021-04-14 16:44:17.000000 openmdao-3.9.1/openmdao/visualization/n2_viewer/libs/json5_2.2.0.min.js
--rw-r--r--   0 swryan    (1000) swryan    (1000)    24324 2021-03-09 15:34:37.000000 openmdao-3.9.1/openmdao/visualization/n2_viewer/libs/pako_inflate.min.js
--rw-r--r--   0 swryan    (1000) swryan    (1000)     4679 2021-03-09 15:34:37.000000 openmdao-3.9.1/openmdao/visualization/n2_viewer/libs/vkBeautify.js
--rw-r--r--   0 swryan    (1000) swryan    (1000)    24133 2021-04-29 15:52:08.000000 openmdao-3.9.1/openmdao/visualization/n2_viewer/n2_viewer.py
-drwxr-xr-x   0 swryan    (1000) swryan    (1000)        0 2021-05-04 15:48:00.964785 openmdao-3.9.1/openmdao/visualization/n2_viewer/src/
--rw-r--r--   0 swryan    (1000) swryan    (1000)    16299 2021-04-14 16:44:17.000000 openmdao-3.9.1/openmdao/visualization/n2_viewer/src/ModelData.js
--rw-r--r--   0 swryan    (1000) swryan    (1000)    39388 2021-03-09 15:34:37.000000 openmdao-3.9.1/openmdao/visualization/n2_viewer/src/N2Arrow.js
--rw-r--r--   0 swryan    (1000) swryan    (1000)    38862 2021-03-15 19:14:32.000000 openmdao-3.9.1/openmdao/visualization/n2_viewer/src/N2Diagram.js
--rw-r--r--   0 swryan    (1000) swryan    (1000)     1167 2021-03-09 15:34:37.000000 openmdao-3.9.1/openmdao/visualization/n2_viewer/src/N2ErrorHandling.js
--rw-r--r--   0 swryan    (1000) swryan    (1000)    24044 2021-03-09 15:34:37.000000 openmdao-3.9.1/openmdao/visualization/n2_viewer/src/N2Layout.js
--rw-r--r--   0 swryan    (1000) swryan    (1000)    13448 2021-03-22 16:37:55.000000 openmdao-3.9.1/openmdao/visualization/n2_viewer/src/N2Legend.js
--rw-r--r--   0 swryan    (1000) swryan    (1000)    35360 2021-03-09 15:34:37.000000 openmdao-3.9.1/openmdao/visualization/n2_viewer/src/N2Matrix.js
--rw-r--r--   0 swryan    (1000) swryan    (1000)    22419 2021-03-15 19:14:32.000000 openmdao-3.9.1/openmdao/visualization/n2_viewer/src/N2MatrixCell.js
--rw-r--r--   0 swryan    (1000) swryan    (1000)    11228 2021-03-15 19:14:32.000000 openmdao-3.9.1/openmdao/visualization/n2_viewer/src/N2Search.js
--rw-r--r--   0 swryan    (1000) swryan    (1000)    10678 2021-03-09 15:34:37.000000 openmdao-3.9.1/openmdao/visualization/n2_viewer/src/N2Style.js
--rw-r--r--   0 swryan    (1000) swryan    (1000)    19011 2021-03-15 19:14:32.000000 openmdao-3.9.1/openmdao/visualization/n2_viewer/src/N2Toolbar.js
--rw-r--r--   0 swryan    (1000) swryan    (1000)     9871 2021-03-15 19:14:32.000000 openmdao-3.9.1/openmdao/visualization/n2_viewer/src/N2TreeNode.js
--rw-r--r--   0 swryan    (1000) swryan    (1000)    30934 2021-03-22 16:37:55.000000 openmdao-3.9.1/openmdao/visualization/n2_viewer/src/N2UserInterface.js
--rw-r--r--   0 swryan    (1000) swryan    (1000)    23433 2021-03-15 19:14:32.000000 openmdao-3.9.1/openmdao/visualization/n2_viewer/src/N2Window.js
--rw-r--r--   0 swryan    (1000) swryan    (1000)    21076 2021-03-09 15:34:37.000000 openmdao-3.9.1/openmdao/visualization/n2_viewer/src/NodeInfo.js
--rw-r--r--   0 swryan    (1000) swryan    (1000)     3877 2021-03-09 15:34:37.000000 openmdao-3.9.1/openmdao/visualization/n2_viewer/src/SymbolType.js
--rw-r--r--   0 swryan    (1000) swryan    (1000)     2055 2021-03-23 16:05:26.000000 openmdao-3.9.1/openmdao/visualization/n2_viewer/src/defaults.js
--rw-r--r--   0 swryan    (1000) swryan    (1000)      423 2021-03-09 15:34:37.000000 openmdao-3.9.1/openmdao/visualization/n2_viewer/src/ptN2.js
--rw-r--r--   0 swryan    (1000) swryan    (1000)     4132 2021-03-09 15:34:37.000000 openmdao-3.9.1/openmdao/visualization/n2_viewer/src/utils.js
-drwxr-xr-x   0 swryan    (1000) swryan    (1000)        0 2021-05-04 15:48:00.984785 openmdao-3.9.1/openmdao/visualization/n2_viewer/style/
--rw-r--r--   0 swryan    (1000) swryan    (1000)     1938 2021-03-09 15:34:37.000000 openmdao-3.9.1/openmdao/visualization/n2_viewer/style/awesomplete.css
--rw-r--r--   0 swryan    (1000) swryan    (1000)     3749 2021-03-15 19:14:32.000000 openmdao-3.9.1/openmdao/visualization/n2_viewer/style/legend.css
--rw-r--r--   0 swryan    (1000) swryan    (1000)    17812 2021-03-09 15:34:37.000000 openmdao-3.9.1/openmdao/visualization/n2_viewer/style/logo_png.b64
--rw-r--r--   0 swryan    (1000) swryan    (1000)     4588 2021-03-15 19:14:32.000000 openmdao-3.9.1/openmdao/visualization/n2_viewer/style/n2toolbar-icons-font.woff
--rw-r--r--   0 swryan    (1000) swryan    (1000)     2673 2021-03-15 19:14:32.000000 openmdao-3.9.1/openmdao/visualization/n2_viewer/style/n2toolbar-icons.css
--rw-r--r--   0 swryan    (1000) swryan    (1000)     5415 2021-03-15 19:14:32.000000 openmdao-3.9.1/openmdao/visualization/n2_viewer/style/partition_tree.css
--rw-r--r--   0 swryan    (1000) swryan    (1000)     8433 2021-03-22 16:37:55.000000 openmdao-3.9.1/openmdao/visualization/n2_viewer/style/toolbar.css
--rw-r--r--   0 swryan    (1000) swryan    (1000)    16643 2021-03-15 19:14:32.000000 openmdao-3.9.1/openmdao/visualization/n2_viewer/style/window.css
-drwxr-xr-x   0 swryan    (1000) swryan    (1000)        0 2021-05-04 15:48:01.020785 openmdao-3.9.1/openmdao/visualization/n2_viewer/tests/
--rw-r--r--   0 swryan    (1000) swryan    (1000)        0 2021-03-09 15:34:37.000000 openmdao-3.9.1/openmdao/visualization/n2_viewer/tests/__init__.py
--rw-r--r--   0 swryan    (1000) swryan    (1000)     7997 2021-04-29 15:52:08.000000 openmdao-3.9.1/openmdao/visualization/n2_viewer/tests/betz_tree.json
-drwxr-xr-x   0 swryan    (1000) swryan    (1000)        0 2021-05-04 15:48:01.044785 openmdao-3.9.1/openmdao/visualization/n2_viewer/tests/gui_test_models/
--rw-r--r--   0 swryan    (1000) swryan    (1000)     1491 2021-03-09 15:34:37.000000 openmdao-3.9.1/openmdao/visualization/n2_viewer/tests/gui_test_models/bug_arrow.py
--rw-r--r--   0 swryan    (1000) swryan    (1000)     4766 2021-03-09 15:34:37.000000 openmdao-3.9.1/openmdao/visualization/n2_viewer/tests/gui_test_models/circuit.py
--rw-r--r--   0 swryan    (1000) swryan    (1000)      690 2021-03-09 15:34:37.000000 openmdao-3.9.1/openmdao/visualization/n2_viewer/tests/gui_test_models/double_sellar.py
--rw-r--r--   0 swryan    (1000) swryan    (1000)      544 2021-03-09 15:34:37.000000 openmdao-3.9.1/openmdao/visualization/n2_viewer/tests/gui_test_models/nan_value.py
--rw-r--r--   0 swryan    (1000) swryan    (1000)      790 2021-03-09 15:34:37.000000 openmdao-3.9.1/openmdao/visualization/n2_viewer/tests/gui_test_models/parabaloid.py
--rw-r--r--   0 swryan    (1000) swryan    (1000)      955 2021-03-09 15:34:37.000000 openmdao-3.9.1/openmdao/visualization/n2_viewer/tests/gui_test_models/valuewin2.py
--rw-r--r--   0 swryan    (1000) swryan    (1000)    30212 2021-03-25 15:33:56.000000 openmdao-3.9.1/openmdao/visualization/n2_viewer/tests/n2_gui_test.py
--rw-r--r--   0 swryan    (1000) swryan    (1000)    18229 2021-04-29 15:52:08.000000 openmdao-3.9.1/openmdao/visualization/n2_viewer/tests/sellar_tree.json
--rw-r--r--   0 swryan    (1000) swryan    (1000)     2315 2021-03-09 15:34:37.000000 openmdao-3.9.1/openmdao/visualization/n2_viewer/tests/test_gui.py
--rw-r--r--   0 swryan    (1000) swryan    (1000)     9002 2021-03-09 15:34:37.000000 openmdao-3.9.1/openmdao/visualization/n2_viewer/tests/test_n2_viewer.py
--rw-r--r--   0 swryan    (1000) swryan    (1000)     1763 2021-03-09 15:34:37.000000 openmdao-3.9.1/openmdao/visualization/n2_viewer/tests/test_parallel_n2.py
--rw-r--r--   0 swryan    (1000) swryan    (1000)     5247 2021-03-09 15:34:37.000000 openmdao-3.9.1/openmdao/visualization/n2_viewer/tests/test_serialization.py
--rw-r--r--   0 swryan    (1000) swryan    (1000)    23728 2021-04-29 15:52:08.000000 openmdao-3.9.1/openmdao/visualization/n2_viewer/tests/test_viewmodeldata.py
--rw-r--r--   0 swryan    (1000) swryan    (1000)     4802 2021-04-29 15:52:08.000000 openmdao-3.9.1/openmdao/visualization/partial_deriv_plot.py
-drwxr-xr-x   0 swryan    (1000) swryan    (1000)        0 2021-05-04 15:48:01.064785 openmdao-3.9.1/openmdao/visualization/scaling_viewer/
--rw-r--r--   0 swryan    (1000) swryan    (1000)        0 2021-03-09 15:34:37.000000 openmdao-3.9.1/openmdao/visualization/scaling_viewer/__init__.py
--rw-r--r--   0 swryan    (1000) swryan    (1000)    18945 2021-04-29 15:52:08.000000 openmdao-3.9.1/openmdao/visualization/scaling_viewer/scaling_report.py
--rw-r--r--   0 swryan    (1000) swryan    (1000)    22001 2021-03-09 15:34:37.000000 openmdao-3.9.1/openmdao/visualization/scaling_viewer/scaling_table.html
--rw-r--r--   0 swryan    (1000) swryan    (1000)     8957 2021-04-29 15:52:08.000000 openmdao-3.9.1/openmdao/warnings.py
-drwxr-xr-x   0 swryan    (1000) swryan    (1000)        0 2021-05-04 15:47:58.652793 openmdao-3.9.1/openmdao.egg-info/
--rw-r--r--   0 swryan    (1000) swryan    (1000)     1496 2021-05-04 15:47:58.000000 openmdao-3.9.1/openmdao.egg-info/PKG-INFO
--rw-r--r--   0 swryan    (1000) swryan    (1000)    25895 2021-05-04 15:47:58.000000 openmdao-3.9.1/openmdao.egg-info/SOURCES.txt
--rw-r--r--   0 swryan    (1000) swryan    (1000)        1 2021-05-04 15:47:58.000000 openmdao-3.9.1/openmdao.egg-info/dependency_links.txt
--rw-r--r--   0 swryan    (1000) swryan    (1000)     3740 2021-05-04 15:47:58.000000 openmdao-3.9.1/openmdao.egg-info/entry_points.txt
--rw-r--r--   0 swryan    (1000) swryan    (1000)      567 2021-05-04 15:47:58.000000 openmdao-3.9.1/openmdao.egg-info/requires.txt
--rw-r--r--   0 swryan    (1000) swryan    (1000)        9 2021-05-04 15:47:58.000000 openmdao-3.9.1/openmdao.egg-info/top_level.txt
--rw-r--r--   0 swryan    (1000) swryan    (1000)       38 2021-05-04 15:48:01.068785 openmdao-3.9.1/setup.cfg
--rw-r--r--   0 swryan    (1000) swryan    (1000)     9859 2021-04-22 20:40:02.000000 openmdao-3.9.1/setup.py
+drwxr-xr-x   0 swryan    (1000) swryan    (1000)        0 2021-05-14 19:15:32.000000 openmdao-3.9.2/
+-rw-r--r--   0 swryan    (1000) swryan    (1000)      558 2021-03-09 15:34:37.000000 openmdao-3.9.2/LICENSE.txt
+-rw-r--r--   0 swryan    (1000) swryan    (1000)       95 2021-03-09 15:34:37.000000 openmdao-3.9.2/MANIFEST.in
+-rw-r--r--   0 swryan    (1000) swryan    (1000)     1496 2021-05-14 19:15:32.000000 openmdao-3.9.2/PKG-INFO
+-rw-r--r--   0 swryan    (1000) swryan    (1000)     6252 2021-05-12 14:15:10.000000 openmdao-3.9.2/README.md
+drwxr-xr-x   0 swryan    (1000) swryan    (1000)        0 2021-05-14 19:15:30.000000 openmdao-3.9.2/openmdao/
+-rw-r--r--   0 swryan    (1000) swryan    (1000)       42 2021-05-14 19:11:54.000000 openmdao-3.9.2/openmdao/__init__.py
+-rw-r--r--   0 swryan    (1000) swryan    (1000)     5348 2021-05-12 14:15:10.000000 openmdao-3.9.2/openmdao/api.py
+drwxr-xr-x   0 swryan    (1000) swryan    (1000)        0 2021-05-14 19:15:30.000000 openmdao-3.9.2/openmdao/approximation_schemes/
+-rw-r--r--   0 swryan    (1000) swryan    (1000)        0 2021-03-09 15:34:37.000000 openmdao-3.9.2/openmdao/approximation_schemes/__init__.py
+-rw-r--r--   0 swryan    (1000) swryan    (1000)    23805 2021-05-12 14:15:10.000000 openmdao-3.9.2/openmdao/approximation_schemes/approximation_scheme.py
+-rw-r--r--   0 swryan    (1000) swryan    (1000)     6836 2021-05-12 14:15:10.000000 openmdao-3.9.2/openmdao/approximation_schemes/complex_step.py
+-rw-r--r--   0 swryan    (1000) swryan    (1000)    11165 2021-05-12 14:15:10.000000 openmdao-3.9.2/openmdao/approximation_schemes/finite_difference.py
+drwxr-xr-x   0 swryan    (1000) swryan    (1000)        0 2021-05-14 19:15:30.000000 openmdao-3.9.2/openmdao/code_review/
+-rw-r--r--   0 swryan    (1000) swryan    (1000)        0 2021-03-09 15:34:37.000000 openmdao-3.9.2/openmdao/code_review/__init__.py
+-rw-r--r--   0 swryan    (1000) swryan    (1000)     9286 2021-04-29 15:52:07.000000 openmdao-3.9.2/openmdao/code_review/test_lint_attributes.py
+-rw-r--r--   0 swryan    (1000) swryan    (1000)    21036 2021-04-29 15:52:07.000000 openmdao-3.9.2/openmdao/code_review/test_lint_docstrings.py
+-rw-r--r--   0 swryan    (1000) swryan    (1000)     4084 2021-03-15 19:14:32.000000 openmdao-3.9.2/openmdao/code_review/test_lint_peps.py
+drwxr-xr-x   0 swryan    (1000) swryan    (1000)        0 2021-05-14 19:15:30.000000 openmdao-3.9.2/openmdao/components/
+-rw-r--r--   0 swryan    (1000) swryan    (1000)        0 2021-03-09 15:34:37.000000 openmdao-3.9.2/openmdao/components/__init__.py
+-rw-r--r--   0 swryan    (1000) swryan    (1000)    12200 2021-05-12 14:15:10.000000 openmdao-3.9.2/openmdao/components/add_subtract_comp.py
+-rw-r--r--   0 swryan    (1000) swryan    (1000)    15205 2021-04-29 15:52:07.000000 openmdao-3.9.2/openmdao/components/balance_comp.py
+-rw-r--r--   0 swryan    (1000) swryan    (1000)     8384 2021-04-29 15:52:07.000000 openmdao-3.9.2/openmdao/components/cross_product_comp.py
+-rw-r--r--   0 swryan    (1000) swryan    (1000)     4616 2021-05-12 14:15:10.000000 openmdao-3.9.2/openmdao/components/demux_comp.py
+-rw-r--r--   0 swryan    (1000) swryan    (1000)     8552 2021-04-29 15:52:07.000000 openmdao-3.9.2/openmdao/components/dot_product_comp.py
+-rw-r--r--   0 swryan    (1000) swryan    (1000)    14605 2021-04-29 15:52:07.000000 openmdao-3.9.2/openmdao/components/eq_constraint_comp.py
+-rw-r--r--   0 swryan    (1000) swryan    (1000)    37428 2021-05-12 14:15:10.000000 openmdao-3.9.2/openmdao/components/exec_comp.py
+-rw-r--r--   0 swryan    (1000) swryan    (1000)    14528 2021-05-12 14:15:10.000000 openmdao-3.9.2/openmdao/components/external_code_comp.py
+drwxr-xr-x   0 swryan    (1000) swryan    (1000)        0 2021-05-14 19:15:30.000000 openmdao-3.9.2/openmdao/components/interp_util/
+-rw-r--r--   0 swryan    (1000) swryan    (1000)        0 2021-03-09 15:34:37.000000 openmdao-3.9.2/openmdao/components/interp_util/__init__.py
+-rw-r--r--   0 swryan    (1000) swryan    (1000)    20900 2021-04-29 15:52:07.000000 openmdao-3.9.2/openmdao/components/interp_util/interp.py
+-rw-r--r--   0 swryan    (1000) swryan    (1000)    26162 2021-05-12 14:15:10.000000 openmdao-3.9.2/openmdao/components/interp_util/interp_akima.py
+-rw-r--r--   0 swryan    (1000) swryan    (1000)     7622 2021-05-12 14:15:10.000000 openmdao-3.9.2/openmdao/components/interp_util/interp_algorithm.py
+-rw-r--r--   0 swryan    (1000) swryan    (1000)     6142 2021-04-29 15:52:07.000000 openmdao-3.9.2/openmdao/components/interp_util/interp_bsplines.py
+-rw-r--r--   0 swryan    (1000) swryan    (1000)     7049 2021-05-12 14:15:10.000000 openmdao-3.9.2/openmdao/components/interp_util/interp_cubic.py
+-rw-r--r--   0 swryan    (1000) swryan    (1000)     4306 2021-05-12 14:15:10.000000 openmdao-3.9.2/openmdao/components/interp_util/interp_lagrange2.py
+-rw-r--r--   0 swryan    (1000) swryan    (1000)     5105 2021-05-12 14:15:10.000000 openmdao-3.9.2/openmdao/components/interp_util/interp_lagrange3.py
+-rw-r--r--   0 swryan    (1000) swryan    (1000)    11768 2021-05-12 14:15:10.000000 openmdao-3.9.2/openmdao/components/interp_util/interp_scipy.py
+-rw-r--r--   0 swryan    (1000) swryan    (1000)     3282 2021-05-12 14:15:10.000000 openmdao-3.9.2/openmdao/components/interp_util/interp_slinear.py
+-rw-r--r--   0 swryan    (1000) swryan    (1000)     1253 2021-04-29 15:52:07.000000 openmdao-3.9.2/openmdao/components/interp_util/outofbounds_error.py
+drwxr-xr-x   0 swryan    (1000) swryan    (1000)        0 2021-05-14 19:15:30.000000 openmdao-3.9.2/openmdao/components/interp_util/tests/
+-rw-r--r--   0 swryan    (1000) swryan    (1000)        0 2021-03-09 15:34:37.000000 openmdao-3.9.2/openmdao/components/interp_util/tests/__init__.py
+-rw-r--r--   0 swryan    (1000) swryan    (1000)    27721 2021-03-15 19:14:32.000000 openmdao-3.9.2/openmdao/components/interp_util/tests/test_interp_nd.py
+-rw-r--r--   0 swryan    (1000) swryan    (1000)     8898 2021-04-29 15:52:07.000000 openmdao-3.9.2/openmdao/components/ks_comp.py
+-rw-r--r--   0 swryan    (1000) swryan    (1000)     7161 2021-04-29 15:52:07.000000 openmdao-3.9.2/openmdao/components/linear_system_comp.py
+-rw-r--r--   0 swryan    (1000) swryan    (1000)     9955 2021-04-29 15:52:07.000000 openmdao-3.9.2/openmdao/components/matrix_vector_product_comp.py
+-rw-r--r--   0 swryan    (1000) swryan    (1000)     9638 2021-04-29 15:52:07.000000 openmdao-3.9.2/openmdao/components/meta_model_structured_comp.py
+-rw-r--r--   0 swryan    (1000) swryan    (1000)    24491 2021-05-12 14:15:10.000000 openmdao-3.9.2/openmdao/components/meta_model_unstructured_comp.py
+-rw-r--r--   0 swryan    (1000) swryan    (1000)    13855 2021-05-12 14:15:10.000000 openmdao-3.9.2/openmdao/components/multifi_meta_model_unstructured_comp.py
+-rw-r--r--   0 swryan    (1000) swryan    (1000)     4493 2021-04-29 15:52:07.000000 openmdao-3.9.2/openmdao/components/mux_comp.py
+-rw-r--r--   0 swryan    (1000) swryan    (1000)     7569 2021-04-29 15:52:07.000000 openmdao-3.9.2/openmdao/components/spline_comp.py
+drwxr-xr-x   0 swryan    (1000) swryan    (1000)        0 2021-05-14 19:15:31.000000 openmdao-3.9.2/openmdao/components/tests/
+-rw-r--r--   0 swryan    (1000) swryan    (1000)        0 2021-03-09 15:34:37.000000 openmdao-3.9.2/openmdao/components/tests/__init__.py
+-rw-r--r--   0 swryan    (1000) swryan    (1000)     1240 2021-03-09 15:34:37.000000 openmdao-3.9.2/openmdao/components/tests/extcode_example.py
+-rw-r--r--   0 swryan    (1000) swryan    (1000)     2148 2021-03-09 15:34:37.000000 openmdao-3.9.2/openmdao/components/tests/extcode_mach.py
+-rw-r--r--   0 swryan    (1000) swryan    (1000)      976 2021-03-09 15:34:37.000000 openmdao-3.9.2/openmdao/components/tests/extcode_node.py
+-rw-r--r--   0 swryan    (1000) swryan    (1000)      649 2021-03-09 15:34:37.000000 openmdao-3.9.2/openmdao/components/tests/extcode_paraboloid.py
+-rw-r--r--   0 swryan    (1000) swryan    (1000)      988 2021-03-09 15:34:37.000000 openmdao-3.9.2/openmdao/components/tests/extcode_paraboloid_derivs.py
+-rw-r--r--   0 swryan    (1000) swryan    (1000)      637 2021-03-09 15:34:37.000000 openmdao-3.9.2/openmdao/components/tests/extcode_resistor.py
+-rw-r--r--   0 swryan    (1000) swryan    (1000)    15629 2021-03-09 15:34:37.000000 openmdao-3.9.2/openmdao/components/tests/test_add_subtract_comp.py
+-rw-r--r--   0 swryan    (1000) swryan    (1000)    28803 2021-03-09 15:34:37.000000 openmdao-3.9.2/openmdao/components/tests/test_balance_comp.py
+-rw-r--r--   0 swryan    (1000) swryan    (1000)    21721 2021-03-09 15:34:37.000000 openmdao-3.9.2/openmdao/components/tests/test_cross_product_comp.py
+-rw-r--r--   0 swryan    (1000) swryan    (1000)     9411 2021-05-12 14:15:10.000000 openmdao-3.9.2/openmdao/components/tests/test_demux_comp.py
+-rw-r--r--   0 swryan    (1000) swryan    (1000)    21010 2021-03-09 15:34:37.000000 openmdao-3.9.2/openmdao/components/tests/test_dot_product_comp.py
+-rw-r--r--   0 swryan    (1000) swryan    (1000)    19831 2021-03-09 15:34:37.000000 openmdao-3.9.2/openmdao/components/tests/test_eq_constraint_comp.py
+-rw-r--r--   0 swryan    (1000) swryan    (1000)    70612 2021-05-12 14:15:10.000000 openmdao-3.9.2/openmdao/components/tests/test_exec_comp.py
+-rw-r--r--   0 swryan    (1000) swryan    (1000)    22588 2021-03-09 15:34:37.000000 openmdao-3.9.2/openmdao/components/tests/test_external_code_comp.py
+-rw-r--r--   0 swryan    (1000) swryan    (1000)    11252 2021-05-12 14:15:10.000000 openmdao-3.9.2/openmdao/components/tests/test_ks_comp.py
+-rw-r--r--   0 swryan    (1000) swryan    (1000)    12997 2021-03-09 15:34:37.000000 openmdao-3.9.2/openmdao/components/tests/test_linear_system_comp.py
+-rw-r--r--   0 swryan    (1000) swryan    (1000)    23366 2021-03-09 15:34:37.000000 openmdao-3.9.2/openmdao/components/tests/test_matrix_vector_product_comp.py
+-rw-r--r--   0 swryan    (1000) swryan    (1000)    54326 2021-03-09 15:34:37.000000 openmdao-3.9.2/openmdao/components/tests/test_meta_model_structured_comp.py
+-rw-r--r--   0 swryan    (1000) swryan    (1000)    43719 2021-05-12 14:15:10.000000 openmdao-3.9.2/openmdao/components/tests/test_meta_model_unstructured_comp.py
+-rw-r--r--   0 swryan    (1000) swryan    (1000)    19161 2021-03-09 15:34:37.000000 openmdao-3.9.2/openmdao/components/tests/test_multifi_meta_model_unstructured_comp.py
+-rw-r--r--   0 swryan    (1000) swryan    (1000)     8581 2021-03-09 15:34:37.000000 openmdao-3.9.2/openmdao/components/tests/test_mux_comp.py
+-rw-r--r--   0 swryan    (1000) swryan    (1000)    21876 2021-03-09 15:34:37.000000 openmdao-3.9.2/openmdao/components/tests/test_spline_comp.py
+-rw-r--r--   0 swryan    (1000) swryan    (1000)    13083 2021-03-09 15:34:37.000000 openmdao-3.9.2/openmdao/components/tests/test_vector_magnitude_comp.py
+-rw-r--r--   0 swryan    (1000) swryan    (1000)     6347 2021-04-29 15:52:07.000000 openmdao-3.9.2/openmdao/components/vector_magnitude_comp.py
+drwxr-xr-x   0 swryan    (1000) swryan    (1000)        0 2021-05-14 19:15:31.000000 openmdao-3.9.2/openmdao/core/
+-rw-r--r--   0 swryan    (1000) swryan    (1000)        0 2021-03-09 15:34:37.000000 openmdao-3.9.2/openmdao/core/__init__.py
+-rw-r--r--   0 swryan    (1000) swryan    (1000)     1073 2021-05-12 14:15:10.000000 openmdao-3.9.2/openmdao/core/analysis_error.py
+-rw-r--r--   0 swryan    (1000) swryan    (1000)    74220 2021-05-12 14:15:10.000000 openmdao-3.9.2/openmdao/core/component.py
+-rw-r--r--   0 swryan    (1000) swryan    (1000)     3366 2021-04-29 15:52:07.000000 openmdao-3.9.2/openmdao/core/configinfo.py
+-rw-r--r--   0 swryan    (1000) swryan    (1000)     2002 2021-04-29 15:52:07.000000 openmdao-3.9.2/openmdao/core/constants.py
+-rw-r--r--   0 swryan    (1000) swryan    (1000)    50537 2021-05-14 13:26:18.000000 openmdao-3.9.2/openmdao/core/driver.py
+-rw-r--r--   0 swryan    (1000) swryan    (1000)    22657 2021-05-12 14:15:10.000000 openmdao-3.9.2/openmdao/core/explicitcomponent.py
+-rw-r--r--   0 swryan    (1000) swryan    (1000)   162316 2021-05-12 14:15:10.000000 openmdao-3.9.2/openmdao/core/group.py
+-rw-r--r--   0 swryan    (1000) swryan    (1000)    22064 2021-05-12 14:15:10.000000 openmdao-3.9.2/openmdao/core/implicitcomponent.py
+-rw-r--r--   0 swryan    (1000) swryan    (1000)    13779 2021-05-12 14:15:10.000000 openmdao-3.9.2/openmdao/core/indepvarcomp.py
+-rw-r--r--   0 swryan    (1000) swryan    (1000)      550 2021-04-29 15:52:07.000000 openmdao-3.9.2/openmdao/core/parallel_group.py
+-rw-r--r--   0 swryan    (1000) swryan    (1000)   108337 2021-05-14 13:26:18.000000 openmdao-3.9.2/openmdao/core/problem.py
+-rw-r--r--   0 swryan    (1000) swryan    (1000)   213964 2021-05-12 14:15:10.000000 openmdao-3.9.2/openmdao/core/system.py
+drwxr-xr-x   0 swryan    (1000) swryan    (1000)        0 2021-05-14 19:15:31.000000 openmdao-3.9.2/openmdao/core/tests/
+-rw-r--r--   0 swryan    (1000) swryan    (1000)        0 2021-03-09 15:34:37.000000 openmdao-3.9.2/openmdao/core/tests/__init__.py
+-rw-r--r--   0 swryan    (1000) swryan    (1000)     7470 2021-03-09 15:34:37.000000 openmdao-3.9.2/openmdao/core/tests/test_add_var.py
+-rw-r--r--   0 swryan    (1000) swryan    (1000)    94225 2021-05-12 14:15:10.000000 openmdao-3.9.2/openmdao/core/tests/test_approx_derivs.py
+-rw-r--r--   0 swryan    (1000) swryan    (1000)     9367 2021-03-09 15:34:37.000000 openmdao-3.9.2/openmdao/core/tests/test_auto_ivc.py
+-rw-r--r--   0 swryan    (1000) swryan    (1000)     1958 2021-03-09 15:34:37.000000 openmdao-3.9.2/openmdao/core/tests/test_aviary_mpi_bug.py
+-rw-r--r--   0 swryan    (1000) swryan    (1000)   121074 2021-05-12 14:15:10.000000 openmdao-3.9.2/openmdao/core/tests/test_check_derivs.py
+-rw-r--r--   0 swryan    (1000) swryan    (1000)    60518 2021-05-12 14:15:10.000000 openmdao-3.9.2/openmdao/core/tests/test_coloring.py
+-rw-r--r--   0 swryan    (1000) swryan    (1000)    13691 2021-05-12 14:15:10.000000 openmdao-3.9.2/openmdao/core/tests/test_component.py
+-rw-r--r--   0 swryan    (1000) swryan    (1000)     3535 2021-05-12 14:15:10.000000 openmdao-3.9.2/openmdao/core/tests/test_component_io_independence_from_prob.py
+-rw-r--r--   0 swryan    (1000) swryan    (1000)     7689 2021-03-09 15:34:37.000000 openmdao-3.9.2/openmdao/core/tests/test_compute_jacvec_prod.py
+-rw-r--r--   0 swryan    (1000) swryan    (1000)    27444 2021-05-12 14:15:10.000000 openmdao-3.9.2/openmdao/core/tests/test_connections.py
+-rw-r--r--   0 swryan    (1000) swryan    (1000)     8042 2021-03-09 15:34:37.000000 openmdao-3.9.2/openmdao/core/tests/test_connections_in_configure.py
+-rw-r--r--   0 swryan    (1000) swryan    (1000)     3172 2021-03-09 15:34:37.000000 openmdao-3.9.2/openmdao/core/tests/test_core_simple.py
+-rw-r--r--   0 swryan    (1000) swryan    (1000)    13666 2021-05-12 14:15:10.000000 openmdao-3.9.2/openmdao/core/tests/test_deriv_transfers.py
+-rw-r--r--   0 swryan    (1000) swryan    (1000)    31378 2021-03-09 15:34:37.000000 openmdao-3.9.2/openmdao/core/tests/test_des_vars_responses.py
+-rw-r--r--   0 swryan    (1000) swryan    (1000)     2326 2021-03-09 15:34:37.000000 openmdao-3.9.2/openmdao/core/tests/test_direct_nondistrib_comp.py
+-rw-r--r--   0 swryan    (1000) swryan    (1000)    31640 2021-05-12 14:15:10.000000 openmdao-3.9.2/openmdao/core/tests/test_discrete.py
+-rw-r--r--   0 swryan    (1000) swryan    (1000)     2758 2021-03-09 15:34:37.000000 openmdao-3.9.2/openmdao/core/tests/test_discrete_mpi.py
+-rw-r--r--   0 swryan    (1000) swryan    (1000)     3646 2021-05-12 14:15:10.000000 openmdao-3.9.2/openmdao/core/tests/test_distrib_adder.py
+-rw-r--r--   0 swryan    (1000) swryan    (1000)    54876 2021-05-12 14:15:10.000000 openmdao-3.9.2/openmdao/core/tests/test_distrib_derivs.py
+-rw-r--r--   0 swryan    (1000) swryan    (1000)     4138 2021-03-09 15:34:37.000000 openmdao-3.9.2/openmdao/core/tests/test_distrib_driver_debug_print_options.py
+-rw-r--r--   0 swryan    (1000) swryan    (1000)    24450 2021-05-12 14:15:10.000000 openmdao-3.9.2/openmdao/core/tests/test_distrib_list_vars.py
+-rw-r--r--   0 swryan    (1000) swryan    (1000)    42588 2021-05-12 14:15:10.000000 openmdao-3.9.2/openmdao/core/tests/test_distribcomp.py
+-rw-r--r--   0 swryan    (1000) swryan    (1000)    38606 2021-05-12 14:15:10.000000 openmdao-3.9.2/openmdao/core/tests/test_driver.py
+-rw-r--r--   0 swryan    (1000) swryan    (1000)    37491 2021-05-12 14:15:10.000000 openmdao-3.9.2/openmdao/core/tests/test_dyn_sizing.py
+-rw-r--r--   0 swryan    (1000) swryan    (1000)    47707 2021-03-15 19:14:32.000000 openmdao-3.9.2/openmdao/core/tests/test_expl_comp.py
+-rw-r--r--   0 swryan    (1000) swryan    (1000)    59532 2021-05-12 14:15:10.000000 openmdao-3.9.2/openmdao/core/tests/test_fd_color.py
+-rw-r--r--   0 swryan    (1000) swryan    (1000)     3996 2021-03-09 15:34:37.000000 openmdao-3.9.2/openmdao/core/tests/test_fd_color_chk_partials.py
+-rw-r--r--   0 swryan    (1000) swryan    (1000)     3630 2021-03-09 15:34:37.000000 openmdao-3.9.2/openmdao/core/tests/test_feature_cache_linear_solution.py
+-rw-r--r--   0 swryan    (1000) swryan    (1000)    18289 2021-03-09 15:34:37.000000 openmdao-3.9.2/openmdao/core/tests/test_getset_vars.py
+-rw-r--r--   0 swryan    (1000) swryan    (1000)   156775 2021-05-12 14:15:10.000000 openmdao-3.9.2/openmdao/core/tests/test_group.py
+-rw-r--r--   0 swryan    (1000) swryan    (1000)    56346 2021-03-15 19:14:32.000000 openmdao-3.9.2/openmdao/core/tests/test_impl_comp.py
+-rw-r--r--   0 swryan    (1000) swryan    (1000)     8900 2021-05-12 14:15:10.000000 openmdao-3.9.2/openmdao/core/tests/test_indep_var_comp.py
+-rw-r--r--   0 swryan    (1000) swryan    (1000)     2425 2021-03-09 15:34:37.000000 openmdao-3.9.2/openmdao/core/tests/test_leaks.py
+-rw-r--r--   0 swryan    (1000) swryan    (1000)     9456 2021-03-09 15:34:37.000000 openmdao-3.9.2/openmdao/core/tests/test_masking.py
+-rw-r--r--   0 swryan    (1000) swryan    (1000)    36903 2021-05-12 14:15:10.000000 openmdao-3.9.2/openmdao/core/tests/test_matmat.py
+-rw-r--r--   0 swryan    (1000) swryan    (1000)    17354 2021-03-09 15:34:37.000000 openmdao-3.9.2/openmdao/core/tests/test_mpi_coloring_bug.py
+-rw-r--r--   0 swryan    (1000) swryan    (1000)     2013 2021-03-09 15:34:37.000000 openmdao-3.9.2/openmdao/core/tests/test_mwe_matmat.py
+-rw-r--r--   0 swryan    (1000) swryan    (1000)    36714 2021-03-15 19:14:32.000000 openmdao-3.9.2/openmdao/core/tests/test_parallel_derivatives.py
+-rw-r--r--   0 swryan    (1000) swryan    (1000)    18264 2021-03-09 15:34:37.000000 openmdao-3.9.2/openmdao/core/tests/test_parallel_fd.py
+-rw-r--r--   0 swryan    (1000) swryan    (1000)    16261 2021-03-09 15:34:37.000000 openmdao-3.9.2/openmdao/core/tests/test_parallel_groups.py
+-rw-r--r--   0 swryan    (1000) swryan    (1000)     2790 2021-03-09 15:34:37.000000 openmdao-3.9.2/openmdao/core/tests/test_parallel_src_indices.py
+-rw-r--r--   0 swryan    (1000) swryan    (1000)    14694 2021-05-12 14:15:10.000000 openmdao-3.9.2/openmdao/core/tests/test_prob_remote.py
+-rw-r--r--   0 swryan    (1000) swryan    (1000)    84181 2021-05-14 13:26:18.000000 openmdao-3.9.2/openmdao/core/tests/test_problem.py
+-rw-r--r--   0 swryan    (1000) swryan    (1000)     7293 2021-03-09 15:34:37.000000 openmdao-3.9.2/openmdao/core/tests/test_proc_alloc.py
+-rw-r--r--   0 swryan    (1000) swryan    (1000)     2386 2021-03-09 15:34:37.000000 openmdao-3.9.2/openmdao/core/tests/test_remote_vois.py
+-rw-r--r--   0 swryan    (1000) swryan    (1000)      951 2021-03-09 15:34:37.000000 openmdao-3.9.2/openmdao/core/tests/test_root_comp_list_outputs.py
+-rw-r--r--   0 swryan    (1000) swryan    (1000)    13290 2021-05-12 14:15:10.000000 openmdao-3.9.2/openmdao/core/tests/test_run_root_only.py
+-rw-r--r--   0 swryan    (1000) swryan    (1000)    53772 2021-03-15 19:14:32.000000 openmdao-3.9.2/openmdao/core/tests/test_scaling.py
+-rw-r--r--   0 swryan    (1000) swryan    (1000)      618 2021-03-15 19:14:32.000000 openmdao-3.9.2/openmdao/core/tests/test_serialize.py
+-rw-r--r--   0 swryan    (1000) swryan    (1000)     2049 2021-03-09 15:34:37.000000 openmdao-3.9.2/openmdao/core/tests/test_setup_memleak.py
+-rw-r--r--   0 swryan    (1000) swryan    (1000)     3967 2021-03-09 15:34:37.000000 openmdao-3.9.2/openmdao/core/tests/test_simple_impl_comp.py
+-rw-r--r--   0 swryan    (1000) swryan    (1000)    15717 2021-03-09 15:34:37.000000 openmdao-3.9.2/openmdao/core/tests/test_src_indices.py
+-rw-r--r--   0 swryan    (1000) swryan    (1000)    11342 2021-05-12 14:15:10.000000 openmdao-3.9.2/openmdao/core/tests/test_system.py
+-rw-r--r--   0 swryan    (1000) swryan    (1000)    38772 2021-05-12 14:15:10.000000 openmdao-3.9.2/openmdao/core/tests/test_units.py
+-rw-r--r--   0 swryan    (1000) swryan    (1000)    80902 2021-05-14 13:26:18.000000 openmdao-3.9.2/openmdao/core/total_jac.py
+drwxr-xr-x   0 swryan    (1000) swryan    (1000)        0 2021-05-14 19:15:31.000000 openmdao-3.9.2/openmdao/devtools/
+-rw-r--r--   0 swryan    (1000) swryan    (1000)        0 2021-03-09 15:34:37.000000 openmdao-3.9.2/openmdao/devtools/__init__.py
+-rw-r--r--   0 swryan    (1000) swryan    (1000)    18068 2021-05-12 14:15:10.000000 openmdao-3.9.2/openmdao/devtools/debug.py
+-rw-r--r--   0 swryan    (1000) swryan    (1000)     4458 2021-03-09 15:34:37.000000 openmdao-3.9.2/openmdao/devtools/dump_sqlite_recorder_file.py
+-rw-r--r--   0 swryan    (1000) swryan    (1000)    16162 2021-04-29 15:52:08.000000 openmdao-3.9.2/openmdao/devtools/iprof_mem.py
+-rw-r--r--   0 swryan    (1000) swryan    (1000)    11680 2021-04-29 15:52:08.000000 openmdao-3.9.2/openmdao/devtools/iprof_utils.py
+-rw-r--r--   0 swryan    (1000) swryan    (1000)    12382 2021-04-29 15:52:08.000000 openmdao-3.9.2/openmdao/devtools/iprofile.py
+drwxr-xr-x   0 swryan    (1000) swryan    (1000)        0 2021-05-14 19:15:31.000000 openmdao-3.9.2/openmdao/devtools/iprofile_app/
+-rw-r--r--   0 swryan    (1000) swryan    (1000)        0 2021-03-09 15:34:37.000000 openmdao-3.9.2/openmdao/devtools/iprofile_app/__init__.py
+-rw-r--r--   0 swryan    (1000) swryan    (1000)     7991 2021-05-12 14:15:10.000000 openmdao-3.9.2/openmdao/devtools/iprofile_app/iprofile_app.py
+drwxr-xr-x   0 swryan    (1000) swryan    (1000)        0 2021-05-14 19:15:31.000000 openmdao-3.9.2/openmdao/devtools/iprofile_app/templates/
+-rw-r--r--   0 swryan    (1000) swryan    (1000)     6206 2021-03-09 15:34:37.000000 openmdao-3.9.2/openmdao/devtools/iprofile_app/templates/iprofview.html
+-rw-r--r--   0 swryan    (1000) swryan    (1000)    14101 2021-04-29 15:52:08.000000 openmdao-3.9.2/openmdao/devtools/itrace.py
+-rw-r--r--   0 swryan    (1000) swryan    (1000)     9090 2021-05-12 14:15:10.000000 openmdao-3.9.2/openmdao/devtools/memory.py
+-rw-r--r--   0 swryan    (1000) swryan    (1000)     1875 2021-03-09 15:34:37.000000 openmdao-3.9.2/openmdao/devtools/run_test.py
+drwxr-xr-x   0 swryan    (1000) swryan    (1000)        0 2021-05-14 19:15:31.000000 openmdao-3.9.2/openmdao/devtools/tests/
+-rw-r--r--   0 swryan    (1000) swryan    (1000)        0 2021-03-09 15:34:37.000000 openmdao-3.9.2/openmdao/devtools/tests/__init__.py
+-rw-r--r--   0 swryan    (1000) swryan    (1000)      559 2021-03-09 15:34:37.000000 openmdao-3.9.2/openmdao/devtools/tests/mem_model.py
+-rw-r--r--   0 swryan    (1000) swryan    (1000)     1901 2021-03-09 15:34:37.000000 openmdao-3.9.2/openmdao/devtools/tests/test_debug.py
+-rw-r--r--   0 swryan    (1000) swryan    (1000)     3454 2021-03-09 15:34:37.000000 openmdao-3.9.2/openmdao/devtools/tests/test_iprof_mem.py
+-rw-r--r--   0 swryan    (1000) swryan    (1000)     4711 2021-03-09 15:34:37.000000 openmdao-3.9.2/openmdao/devtools/wing_proj_template.wpr
+-rw-r--r--   0 swryan    (1000) swryan    (1000)     5361 2021-04-29 15:52:08.000000 openmdao-3.9.2/openmdao/devtools/wingproj.py
+drwxr-xr-x   0 swryan    (1000) swryan    (1000)        0 2021-05-14 19:15:31.000000 openmdao-3.9.2/openmdao/docs/
+-rw-r--r--   0 swryan    (1000) swryan    (1000)      324 2021-03-09 15:34:37.000000 openmdao-3.9.2/openmdao/docs/README.md
+-rw-r--r--   0 swryan    (1000) swryan    (1000)        0 2021-03-09 15:34:37.000000 openmdao-3.9.2/openmdao/docs/__init__.py
+drwxr-xr-x   0 swryan    (1000) swryan    (1000)        0 2021-05-14 19:15:31.000000 openmdao-3.9.2/openmdao/docs/_exts/
+-rw-r--r--   0 swryan    (1000) swryan    (1000)        0 2021-03-09 15:34:37.000000 openmdao-3.9.2/openmdao/docs/_exts/__init__.py
+-rw-r--r--   0 swryan    (1000) swryan    (1000)     2021 2021-03-09 15:34:37.000000 openmdao-3.9.2/openmdao/docs/_exts/embed_bibtex.py
+-rw-r--r--   0 swryan    (1000) swryan    (1000)    11478 2021-05-12 14:15:10.000000 openmdao-3.9.2/openmdao/docs/_exts/embed_code.py
+-rw-r--r--   0 swryan    (1000) swryan    (1000)     4452 2021-03-09 15:34:37.000000 openmdao-3.9.2/openmdao/docs/_exts/embed_compare.py
+-rw-r--r--   0 swryan    (1000) swryan    (1000)     3662 2021-03-09 15:34:37.000000 openmdao-3.9.2/openmdao/docs/_exts/embed_n2.py
+-rw-r--r--   0 swryan    (1000) swryan    (1000)     2127 2021-03-09 15:34:37.000000 openmdao-3.9.2/openmdao/docs/_exts/embed_options.py
+-rw-r--r--   0 swryan    (1000) swryan    (1000)     4891 2021-03-09 15:34:37.000000 openmdao-3.9.2/openmdao/docs/_exts/embed_shell_cmd.py
+-rw-r--r--   0 swryan    (1000) swryan    (1000)     3941 2021-03-09 15:34:37.000000 openmdao-3.9.2/openmdao/docs/_exts/link_class_from_docstring.py
+-rw-r--r--   0 swryan    (1000) swryan    (1000)     2323 2021-03-09 15:34:37.000000 openmdao-3.9.2/openmdao/docs/_exts/tags.py
+drwxr-xr-x   0 swryan    (1000) swryan    (1000)        0 2021-05-14 19:15:31.000000 openmdao-3.9.2/openmdao/docs/_utils/
+-rw-r--r--   0 swryan    (1000) swryan    (1000)        0 2021-03-09 15:34:37.000000 openmdao-3.9.2/openmdao/docs/_utils/__init__.py
+-rw-r--r--   0 swryan    (1000) swryan    (1000)    28663 2021-04-29 15:52:08.000000 openmdao-3.9.2/openmdao/docs/_utils/docutil.py
+-rw-r--r--   0 swryan    (1000) swryan    (1000)     6222 2021-03-09 15:34:37.000000 openmdao-3.9.2/openmdao/docs/_utils/generate_sourcedocs.py
+-rw-r--r--   0 swryan    (1000) swryan    (1000)     4283 2021-03-09 15:34:37.000000 openmdao-3.9.2/openmdao/docs/_utils/patch.py
+-rw-r--r--   0 swryan    (1000) swryan    (1000)     3058 2021-03-09 15:34:37.000000 openmdao-3.9.2/openmdao/docs/_utils/preprocess_tags.py
+-rw-r--r--   0 swryan    (1000) swryan    (1000)     1251 2021-03-09 15:34:37.000000 openmdao-3.9.2/openmdao/docs/_utils/run_sub.py
+-rw-r--r--   0 swryan    (1000) swryan    (1000)     2912 2021-05-12 14:15:10.000000 openmdao-3.9.2/openmdao/docs/_utils/upload_doc_version.py
+-rw-r--r--   0 swryan    (1000) swryan    (1000)     5308 2021-03-09 15:34:37.000000 openmdao-3.9.2/openmdao/docs/conf.py
+-rw-r--r--   0 swryan    (1000) swryan    (1000)      183 2021-03-09 15:34:37.000000 openmdao-3.9.2/openmdao/docs/config_params.py
+-rw-r--r--   0 swryan    (1000) swryan    (1000)      313 2021-03-09 15:34:37.000000 openmdao-3.9.2/openmdao/docs/debug_build_docs.py
+-rw-r--r--   0 swryan    (1000) swryan    (1000)      469 2021-03-09 15:34:37.000000 openmdao-3.9.2/openmdao/docutils.py
+drwxr-xr-x   0 swryan    (1000) swryan    (1000)        0 2021-05-14 19:15:31.000000 openmdao-3.9.2/openmdao/drivers/
+-rw-r--r--   0 swryan    (1000) swryan    (1000)        0 2021-03-09 15:34:37.000000 openmdao-3.9.2/openmdao/drivers/__init__.py
+-rw-r--r--   0 swryan    (1000) swryan    (1000)    22343 2021-05-12 14:15:10.000000 openmdao-3.9.2/openmdao/drivers/differential_evolution_driver.py
+-rw-r--r--   0 swryan    (1000) swryan    (1000)     9579 2021-05-12 14:15:10.000000 openmdao-3.9.2/openmdao/drivers/doe_driver.py
+-rw-r--r--   0 swryan    (1000) swryan    (1000)    21019 2021-05-12 14:15:10.000000 openmdao-3.9.2/openmdao/drivers/doe_generators.py
+-rw-r--r--   0 swryan    (1000) swryan    (1000)    36701 2021-04-29 15:52:08.000000 openmdao-3.9.2/openmdao/drivers/genetic_algorithm_driver.py
+-rw-r--r--   0 swryan    (1000) swryan    (1000)    30284 2021-05-12 14:15:10.000000 openmdao-3.9.2/openmdao/drivers/pyoptsparse_driver.py
+-rw-r--r--   0 swryan    (1000) swryan    (1000)    32029 2021-05-12 14:15:10.000000 openmdao-3.9.2/openmdao/drivers/scipy_optimizer.py
+drwxr-xr-x   0 swryan    (1000) swryan    (1000)        0 2021-05-14 19:15:31.000000 openmdao-3.9.2/openmdao/drivers/tests/
+-rw-r--r--   0 swryan    (1000) swryan    (1000)        0 2021-03-09 15:34:37.000000 openmdao-3.9.2/openmdao/drivers/tests/__init__.py
+-rw-r--r--   0 swryan    (1000) swryan    (1000)    36801 2021-05-12 14:15:10.000000 openmdao-3.9.2/openmdao/drivers/tests/test_differential_evolution_driver.py
+-rw-r--r--   0 swryan    (1000) swryan    (1000)    82397 2021-05-12 14:15:10.000000 openmdao-3.9.2/openmdao/drivers/tests/test_doe_driver.py
+-rw-r--r--   0 swryan    (1000) swryan    (1000)    59486 2021-05-12 14:15:10.000000 openmdao-3.9.2/openmdao/drivers/tests/test_genetic_algorithm_driver.py
+-rw-r--r--   0 swryan    (1000) swryan    (1000)    99048 2021-05-14 13:26:18.000000 openmdao-3.9.2/openmdao/drivers/tests/test_pyoptsparse_driver.py
+-rw-r--r--   0 swryan    (1000) swryan    (1000)    80761 2021-05-14 13:26:18.000000 openmdao-3.9.2/openmdao/drivers/tests/test_scipy_optimizer.py
+drwxr-xr-x   0 swryan    (1000) swryan    (1000)        0 2021-05-14 19:15:31.000000 openmdao-3.9.2/openmdao/error_checking/
+-rw-r--r--   0 swryan    (1000) swryan    (1000)        0 2021-03-09 15:34:37.000000 openmdao-3.9.2/openmdao/error_checking/__init__.py
+-rw-r--r--   0 swryan    (1000) swryan    (1000)    22408 2021-05-12 14:15:10.000000 openmdao-3.9.2/openmdao/error_checking/check_config.py
+drwxr-xr-x   0 swryan    (1000) swryan    (1000)        0 2021-05-14 19:15:31.000000 openmdao-3.9.2/openmdao/error_checking/tests/
+-rw-r--r--   0 swryan    (1000) swryan    (1000)        0 2021-03-09 15:34:37.000000 openmdao-3.9.2/openmdao/error_checking/tests/__init__.py
+-rw-r--r--   0 swryan    (1000) swryan    (1000)    19085 2021-03-09 15:34:37.000000 openmdao-3.9.2/openmdao/error_checking/tests/test_check_config.py
+-rw-r--r--   0 swryan    (1000) swryan    (1000)    10886 2021-03-09 15:34:37.000000 openmdao-3.9.2/openmdao/error_checking/tests/test_check_solvers.py
+drwxr-xr-x   0 swryan    (1000) swryan    (1000)        0 2021-05-14 19:15:31.000000 openmdao-3.9.2/openmdao/jacobians/
+-rw-r--r--   0 swryan    (1000) swryan    (1000)        0 2021-03-09 15:34:37.000000 openmdao-3.9.2/openmdao/jacobians/__init__.py
+-rw-r--r--   0 swryan    (1000) swryan    (1000)    17502 2021-04-29 15:52:08.000000 openmdao-3.9.2/openmdao/jacobians/assembled_jacobian.py
+-rw-r--r--   0 swryan    (1000) swryan    (1000)    11249 2021-05-12 14:15:10.000000 openmdao-3.9.2/openmdao/jacobians/dictionary_jacobian.py
+-rw-r--r--   0 swryan    (1000) swryan    (1000)    14467 2021-05-12 14:15:10.000000 openmdao-3.9.2/openmdao/jacobians/jacobian.py
+drwxr-xr-x   0 swryan    (1000) swryan    (1000)        0 2021-05-14 19:15:31.000000 openmdao-3.9.2/openmdao/jacobians/tests/
+-rw-r--r--   0 swryan    (1000) swryan    (1000)        0 2021-03-09 15:34:37.000000 openmdao-3.9.2/openmdao/jacobians/tests/__init__.py
+-rw-r--r--   0 swryan    (1000) swryan    (1000)    43820 2021-05-12 14:15:10.000000 openmdao-3.9.2/openmdao/jacobians/tests/test_jacobian.py
+-rw-r--r--   0 swryan    (1000) swryan    (1000)    23098 2021-03-09 15:34:37.000000 openmdao-3.9.2/openmdao/jacobians/tests/test_jacobian_features.py
+drwxr-xr-x   0 swryan    (1000) swryan    (1000)        0 2021-05-14 19:15:31.000000 openmdao-3.9.2/openmdao/matrices/
+-rw-r--r--   0 swryan    (1000) swryan    (1000)        0 2021-03-09 15:34:37.000000 openmdao-3.9.2/openmdao/matrices/__init__.py
+-rw-r--r--   0 swryan    (1000) swryan    (1000)     9494 2021-05-12 14:15:10.000000 openmdao-3.9.2/openmdao/matrices/coo_matrix.py
+-rw-r--r--   0 swryan    (1000) swryan    (1000)     2767 2021-04-29 15:52:08.000000 openmdao-3.9.2/openmdao/matrices/csc_matrix.py
+-rw-r--r--   0 swryan    (1000) swryan    (1000)     1154 2021-04-29 15:52:08.000000 openmdao-3.9.2/openmdao/matrices/csr_matrix.py
+-rw-r--r--   0 swryan    (1000) swryan    (1000)     3656 2021-05-12 14:15:10.000000 openmdao-3.9.2/openmdao/matrices/dense_matrix.py
+-rw-r--r--   0 swryan    (1000) swryan    (1000)     5076 2021-05-12 14:15:10.000000 openmdao-3.9.2/openmdao/matrices/matrix.py
+-rw-r--r--   0 swryan    (1000) swryan    (1000)      132 2021-03-09 15:34:37.000000 openmdao-3.9.2/openmdao/parallel_api.py
+drwxr-xr-x   0 swryan    (1000) swryan    (1000)        0 2021-05-14 19:15:31.000000 openmdao-3.9.2/openmdao/proc_allocators/
+-rw-r--r--   0 swryan    (1000) swryan    (1000)        0 2021-03-09 15:34:37.000000 openmdao-3.9.2/openmdao/proc_allocators/__init__.py
+-rw-r--r--   0 swryan    (1000) swryan    (1000)     5025 2021-04-29 15:52:08.000000 openmdao-3.9.2/openmdao/proc_allocators/default_allocator.py
+-rw-r--r--   0 swryan    (1000) swryan    (1000)     4574 2021-05-12 14:15:10.000000 openmdao-3.9.2/openmdao/proc_allocators/proc_allocator.py
+drwxr-xr-x   0 swryan    (1000) swryan    (1000)        0 2021-05-14 19:15:31.000000 openmdao-3.9.2/openmdao/recorders/
+-rw-r--r--   0 swryan    (1000) swryan    (1000)        0 2021-03-09 15:34:37.000000 openmdao-3.9.2/openmdao/recorders/__init__.py
+-rw-r--r--   0 swryan    (1000) swryan    (1000)     7052 2021-05-12 14:15:10.000000 openmdao-3.9.2/openmdao/recorders/base_case_reader.py
+-rw-r--r--   0 swryan    (1000) swryan    (1000)    39848 2021-05-12 14:15:10.000000 openmdao-3.9.2/openmdao/recorders/case.py
+-rw-r--r--   0 swryan    (1000) swryan    (1000)      758 2021-05-12 14:15:10.000000 openmdao-3.9.2/openmdao/recorders/case_reader.py
+-rw-r--r--   0 swryan    (1000) swryan    (1000)    10625 2021-04-29 15:52:08.000000 openmdao-3.9.2/openmdao/recorders/case_recorder.py
+-rw-r--r--   0 swryan    (1000) swryan    (1000)     4837 2021-04-29 15:52:08.000000 openmdao-3.9.2/openmdao/recorders/recording_iteration_stack.py
+-rw-r--r--   0 swryan    (1000) swryan    (1000)     9407 2021-05-12 14:15:10.000000 openmdao-3.9.2/openmdao/recorders/recording_manager.py
+-rw-r--r--   0 swryan    (1000) swryan    (1000)    63232 2021-05-12 14:15:10.000000 openmdao-3.9.2/openmdao/recorders/sqlite_reader.py
+-rw-r--r--   0 swryan    (1000) swryan    (1000)    32982 2021-05-12 14:15:10.000000 openmdao-3.9.2/openmdao/recorders/sqlite_recorder.py
+drwxr-xr-x   0 swryan    (1000) swryan    (1000)        0 2021-05-14 19:15:31.000000 openmdao-3.9.2/openmdao/recorders/tests/
+-rw-r--r--   0 swryan    (1000) swryan    (1000)        0 2021-03-09 15:34:37.000000 openmdao-3.9.2/openmdao/recorders/tests/__init__.py
+drwxr-xr-x   0 swryan    (1000) swryan    (1000)        0 2021-05-14 19:15:31.000000 openmdao-3.9.2/openmdao/recorders/tests/legacy_sql/
+-rw-r--r--   0 swryan    (1000) swryan    (1000)   122880 2021-03-09 15:34:37.000000 openmdao-3.9.2/openmdao/recorders/tests/legacy_sql/case_database_v4.sql
+-rw-r--r--   0 swryan    (1000) swryan    (1000)    33792 2021-03-09 15:34:37.000000 openmdao-3.9.2/openmdao/recorders/tests/legacy_sql/case_driver_01.sql
+-rw-r--r--   0 swryan    (1000) swryan    (1000)    61440 2021-03-09 15:34:37.000000 openmdao-3.9.2/openmdao/recorders/tests/legacy_sql/case_driver_pre01.sql
+-rw-r--r--   0 swryan    (1000) swryan    (1000)   114688 2021-03-09 15:34:37.000000 openmdao-3.9.2/openmdao/recorders/tests/legacy_sql/case_driver_solver_system_02.sql
+-rw-r--r--   0 swryan    (1000) swryan    (1000)   122880 2021-03-09 15:34:37.000000 openmdao-3.9.2/openmdao/recorders/tests/legacy_sql/case_driver_solver_system_03.sql
+-rw-r--r--   0 swryan    (1000) swryan    (1000)    73728 2021-03-09 15:34:37.000000 openmdao-3.9.2/openmdao/recorders/tests/legacy_sql/case_driver_v5.sql
+-rw-r--r--   0 swryan    (1000) swryan    (1000)    94208 2021-03-09 15:34:37.000000 openmdao-3.9.2/openmdao/recorders/tests/legacy_sql/case_problem_driver_v7.sql
+-rw-r--r--   0 swryan    (1000) swryan    (1000)    73728 2021-03-09 15:34:37.000000 openmdao-3.9.2/openmdao/recorders/tests/legacy_sql/case_problem_driver_v8.sql
+-rw-r--r--   0 swryan    (1000) swryan    (1000)   102400 2021-03-09 15:34:37.000000 openmdao-3.9.2/openmdao/recorders/tests/legacy_sql/case_problem_v11.sql
+-rw-r--r--   0 swryan    (1000) swryan    (1000)    81920 2021-03-09 15:34:37.000000 openmdao-3.9.2/openmdao/recorders/tests/legacy_sql/case_problem_v6.sql
+-rw-r--r--   0 swryan    (1000) swryan    (1000)      142 2021-03-09 15:34:37.000000 openmdao-3.9.2/openmdao/recorders/tests/recorder_test_utils.py
+-rw-r--r--   0 swryan    (1000) swryan    (1000)    23618 2021-05-12 14:15:10.000000 openmdao-3.9.2/openmdao/recorders/tests/sqlite_recorder_test_utils.py
+-rw-r--r--   0 swryan    (1000) swryan    (1000)    10375 2021-05-14 13:26:18.000000 openmdao-3.9.2/openmdao/recorders/tests/test_distrib_sqlite_recorder.py
+-rw-r--r--   0 swryan    (1000) swryan    (1000)   185372 2021-05-12 14:15:10.000000 openmdao-3.9.2/openmdao/recorders/tests/test_sqlite_reader.py
+-rw-r--r--   0 swryan    (1000) swryan    (1000)   128831 2021-05-12 14:15:10.000000 openmdao-3.9.2/openmdao/recorders/tests/test_sqlite_recorder.py
+drwxr-xr-x   0 swryan    (1000) swryan    (1000)        0 2021-05-14 19:15:31.000000 openmdao-3.9.2/openmdao/solvers/
+-rw-r--r--   0 swryan    (1000) swryan    (1000)        0 2021-03-09 15:34:37.000000 openmdao-3.9.2/openmdao/solvers/__init__.py
+drwxr-xr-x   0 swryan    (1000) swryan    (1000)        0 2021-05-14 19:15:31.000000 openmdao-3.9.2/openmdao/solvers/linear/
+-rw-r--r--   0 swryan    (1000) swryan    (1000)        0 2021-03-09 15:34:37.000000 openmdao-3.9.2/openmdao/solvers/linear/__init__.py
+-rw-r--r--   0 swryan    (1000) swryan    (1000)    15278 2021-04-29 15:52:08.000000 openmdao-3.9.2/openmdao/solvers/linear/direct.py
+-rw-r--r--   0 swryan    (1000) swryan    (1000)     8567 2021-04-29 15:52:08.000000 openmdao-3.9.2/openmdao/solvers/linear/linear_block_gs.py
+-rw-r--r--   0 swryan    (1000) swryan    (1000)     1778 2021-03-09 15:34:37.000000 openmdao-3.9.2/openmdao/solvers/linear/linear_block_jac.py
+-rw-r--r--   0 swryan    (1000) swryan    (1000)     1396 2021-04-29 15:52:08.000000 openmdao-3.9.2/openmdao/solvers/linear/linear_runonce.py
+-rw-r--r--   0 swryan    (1000) swryan    (1000)    13874 2021-05-12 14:15:10.000000 openmdao-3.9.2/openmdao/solvers/linear/petsc_ksp.py
+-rw-r--r--   0 swryan    (1000) swryan    (1000)     9036 2021-04-29 15:52:08.000000 openmdao-3.9.2/openmdao/solvers/linear/scipy_iter_solver.py
+drwxr-xr-x   0 swryan    (1000) swryan    (1000)        0 2021-05-14 19:15:31.000000 openmdao-3.9.2/openmdao/solvers/linear/tests/
+-rw-r--r--   0 swryan    (1000) swryan    (1000)        0 2021-03-09 15:34:37.000000 openmdao-3.9.2/openmdao/solvers/linear/tests/__init__.py
+-rw-r--r--   0 swryan    (1000) swryan    (1000)    18631 2021-03-09 15:34:37.000000 openmdao-3.9.2/openmdao/solvers/linear/tests/linear_test_base.py
+-rw-r--r--   0 swryan    (1000) swryan    (1000)    38408 2021-05-12 14:15:10.000000 openmdao-3.9.2/openmdao/solvers/linear/tests/test_direct_solver.py
+-rw-r--r--   0 swryan    (1000) swryan    (1000)    14387 2021-03-09 15:34:37.000000 openmdao-3.9.2/openmdao/solvers/linear/tests/test_linear_block_gs.py
+-rw-r--r--   0 swryan    (1000) swryan    (1000)     7038 2021-03-09 15:34:37.000000 openmdao-3.9.2/openmdao/solvers/linear/tests/test_linear_block_jac.py
+-rw-r--r--   0 swryan    (1000) swryan    (1000)     2603 2021-03-09 15:34:37.000000 openmdao-3.9.2/openmdao/solvers/linear/tests/test_linear_runonce.py
+-rw-r--r--   0 swryan    (1000) swryan    (1000)    22938 2021-05-12 14:15:10.000000 openmdao-3.9.2/openmdao/solvers/linear/tests/test_petsc_ksp.py
+-rw-r--r--   0 swryan    (1000) swryan    (1000)    13076 2021-03-09 15:34:37.000000 openmdao-3.9.2/openmdao/solvers/linear/tests/test_scipy_iter_solver.py
+-rw-r--r--   0 swryan    (1000) swryan    (1000)     9846 2021-05-12 14:15:10.000000 openmdao-3.9.2/openmdao/solvers/linear/tests/test_user_defined.py
+-rw-r--r--   0 swryan    (1000) swryan    (1000)     2071 2021-04-29 15:52:08.000000 openmdao-3.9.2/openmdao/solvers/linear/user_defined.py
+drwxr-xr-x   0 swryan    (1000) swryan    (1000)        0 2021-05-14 19:15:31.000000 openmdao-3.9.2/openmdao/solvers/linesearch/
+-rw-r--r--   0 swryan    (1000) swryan    (1000)        0 2021-03-09 15:34:37.000000 openmdao-3.9.2/openmdao/solvers/linesearch/__init__.py
+-rw-r--r--   0 swryan    (1000) swryan    (1000)    20612 2021-05-12 14:15:10.000000 openmdao-3.9.2/openmdao/solvers/linesearch/backtracking.py
+drwxr-xr-x   0 swryan    (1000) swryan    (1000)        0 2021-05-14 19:15:31.000000 openmdao-3.9.2/openmdao/solvers/linesearch/tests/
+-rw-r--r--   0 swryan    (1000) swryan    (1000)        0 2021-03-09 15:34:37.000000 openmdao-3.9.2/openmdao/solvers/linesearch/tests/__init__.py
+-rw-r--r--   0 swryan    (1000) swryan    (1000)    39454 2021-05-12 14:15:10.000000 openmdao-3.9.2/openmdao/solvers/linesearch/tests/test_backtracking.py
+drwxr-xr-x   0 swryan    (1000) swryan    (1000)        0 2021-05-14 19:15:31.000000 openmdao-3.9.2/openmdao/solvers/nonlinear/
+-rw-r--r--   0 swryan    (1000) swryan    (1000)        0 2021-03-09 15:34:37.000000 openmdao-3.9.2/openmdao/solvers/nonlinear/__init__.py
+-rw-r--r--   0 swryan    (1000) swryan    (1000)    22501 2021-05-12 14:15:10.000000 openmdao-3.9.2/openmdao/solvers/nonlinear/broyden.py
+-rw-r--r--   0 swryan    (1000) swryan    (1000)     9342 2021-04-29 15:52:08.000000 openmdao-3.9.2/openmdao/solvers/nonlinear/newton.py
+-rw-r--r--   0 swryan    (1000) swryan    (1000)     9455 2021-04-29 15:52:08.000000 openmdao-3.9.2/openmdao/solvers/nonlinear/nonlinear_block_gs.py
+-rw-r--r--   0 swryan    (1000) swryan    (1000)     1603 2021-03-09 15:34:37.000000 openmdao-3.9.2/openmdao/solvers/nonlinear/nonlinear_block_jac.py
+-rw-r--r--   0 swryan    (1000) swryan    (1000)     1704 2021-03-09 15:34:37.000000 openmdao-3.9.2/openmdao/solvers/nonlinear/nonlinear_runonce.py
+drwxr-xr-x   0 swryan    (1000) swryan    (1000)        0 2021-05-14 19:15:31.000000 openmdao-3.9.2/openmdao/solvers/nonlinear/tests/
+-rw-r--r--   0 swryan    (1000) swryan    (1000)        0 2021-03-09 15:34:37.000000 openmdao-3.9.2/openmdao/solvers/nonlinear/tests/__init__.py
+-rw-r--r--   0 swryan    (1000) swryan    (1000)    33153 2021-03-09 15:34:37.000000 openmdao-3.9.2/openmdao/solvers/nonlinear/tests/test_broyden.py
+-rw-r--r--   0 swryan    (1000) swryan    (1000)    42253 2021-03-09 15:34:37.000000 openmdao-3.9.2/openmdao/solvers/nonlinear/tests/test_newton.py
+-rw-r--r--   0 swryan    (1000) swryan    (1000)    23974 2021-03-09 15:34:37.000000 openmdao-3.9.2/openmdao/solvers/nonlinear/tests/test_nonlinear_block_gs.py
+-rw-r--r--   0 swryan    (1000) swryan    (1000)     6642 2021-03-09 15:34:37.000000 openmdao-3.9.2/openmdao/solvers/nonlinear/tests/test_nonlinear_block_jac.py
+-rw-r--r--   0 swryan    (1000) swryan    (1000)     3194 2021-03-09 15:34:37.000000 openmdao-3.9.2/openmdao/solvers/nonlinear/tests/test_nonlinear_runonce.py
+-rw-r--r--   0 swryan    (1000) swryan    (1000)    36622 2021-05-12 14:15:10.000000 openmdao-3.9.2/openmdao/solvers/solver.py
+drwxr-xr-x   0 swryan    (1000) swryan    (1000)        0 2021-05-14 19:15:31.000000 openmdao-3.9.2/openmdao/solvers/tests/
+-rw-r--r--   0 swryan    (1000) swryan    (1000)        0 2021-03-09 15:34:37.000000 openmdao-3.9.2/openmdao/solvers/tests/__init__.py
+-rw-r--r--   0 swryan    (1000) swryan    (1000)     8578 2021-03-09 15:34:37.000000 openmdao-3.9.2/openmdao/solvers/tests/test_solver_debug_print.py
+-rw-r--r--   0 swryan    (1000) swryan    (1000)     7284 2021-03-09 15:34:37.000000 openmdao-3.9.2/openmdao/solvers/tests/test_solver_features.py
+-rw-r--r--   0 swryan    (1000) swryan    (1000)    18116 2021-03-09 15:34:37.000000 openmdao-3.9.2/openmdao/solvers/tests/test_solver_iprint.py
+-rw-r--r--   0 swryan    (1000) swryan    (1000)     4686 2021-03-09 15:34:37.000000 openmdao-3.9.2/openmdao/solvers/tests/test_solver_parametric_suite.py
+drwxr-xr-x   0 swryan    (1000) swryan    (1000)        0 2021-05-14 19:15:31.000000 openmdao-3.9.2/openmdao/surrogate_models/
+-rw-r--r--   0 swryan    (1000) swryan    (1000)        0 2021-03-09 15:34:37.000000 openmdao-3.9.2/openmdao/surrogate_models/__init__.py
+-rw-r--r--   0 swryan    (1000) swryan    (1000)    12532 2021-05-12 14:15:10.000000 openmdao-3.9.2/openmdao/surrogate_models/kriging.py
+-rw-r--r--   0 swryan    (1000) swryan    (1000)    40845 2021-05-12 14:15:10.000000 openmdao-3.9.2/openmdao/surrogate_models/multifi_cokriging.py
+-rw-r--r--   0 swryan    (1000) swryan    (1000)     3485 2021-04-29 15:52:08.000000 openmdao-3.9.2/openmdao/surrogate_models/nearest_neighbor.py
+drwxr-xr-x   0 swryan    (1000) swryan    (1000)        0 2021-05-14 19:15:31.000000 openmdao-3.9.2/openmdao/surrogate_models/nn_interpolators/
+-rw-r--r--   0 swryan    (1000) swryan    (1000)        0 2021-03-09 15:34:37.000000 openmdao-3.9.2/openmdao/surrogate_models/nn_interpolators/__init__.py
+-rw-r--r--   0 swryan    (1000) swryan    (1000)     5319 2021-04-29 15:52:08.000000 openmdao-3.9.2/openmdao/surrogate_models/nn_interpolators/linear_interpolator.py
+-rw-r--r--   0 swryan    (1000) swryan    (1000)     3156 2021-04-29 15:52:08.000000 openmdao-3.9.2/openmdao/surrogate_models/nn_interpolators/nn_base.py
+-rw-r--r--   0 swryan    (1000) swryan    (1000)    18609 2021-04-29 15:52:08.000000 openmdao-3.9.2/openmdao/surrogate_models/nn_interpolators/rbf_interpolator.py
+-rw-r--r--   0 swryan    (1000) swryan    (1000)     5305 2021-05-12 14:15:10.000000 openmdao-3.9.2/openmdao/surrogate_models/nn_interpolators/weighted_interpolator.py
+-rw-r--r--   0 swryan    (1000) swryan    (1000)     3563 2021-04-29 15:52:08.000000 openmdao-3.9.2/openmdao/surrogate_models/response_surface.py
+-rw-r--r--   0 swryan    (1000) swryan    (1000)     3244 2021-04-29 15:52:08.000000 openmdao-3.9.2/openmdao/surrogate_models/surrogate_model.py
+drwxr-xr-x   0 swryan    (1000) swryan    (1000)        0 2021-05-14 19:15:31.000000 openmdao-3.9.2/openmdao/surrogate_models/tests/
+-rw-r--r--   0 swryan    (1000) swryan    (1000)        0 2021-03-09 15:34:37.000000 openmdao-3.9.2/openmdao/surrogate_models/tests/__init__.py
+-rw-r--r--   0 swryan    (1000) swryan    (1000)     5683 2021-05-12 14:15:10.000000 openmdao-3.9.2/openmdao/surrogate_models/tests/test_kriging.py
+-rw-r--r--   0 swryan    (1000) swryan    (1000)     2641 2021-03-09 15:34:37.000000 openmdao-3.9.2/openmdao/surrogate_models/tests/test_map.py
+-rw-r--r--   0 swryan    (1000) swryan    (1000)    11356 2021-03-09 15:34:37.000000 openmdao-3.9.2/openmdao/surrogate_models/tests/test_multifi_cokriging.py
+-rw-r--r--   0 swryan    (1000) swryan    (1000)    15590 2021-03-09 15:34:37.000000 openmdao-3.9.2/openmdao/surrogate_models/tests/test_nearest_neighbor.py
+-rw-r--r--   0 swryan    (1000) swryan    (1000)     3861 2021-03-09 15:34:37.000000 openmdao-3.9.2/openmdao/surrogate_models/tests/test_response_surface.py
+drwxr-xr-x   0 swryan    (1000) swryan    (1000)        0 2021-05-14 19:15:31.000000 openmdao-3.9.2/openmdao/test_suite/
+-rw-r--r--   0 swryan    (1000) swryan    (1000)        0 2021-03-09 15:34:37.000000 openmdao-3.9.2/openmdao/test_suite/__init__.py
+-rw-r--r--   0 swryan    (1000) swryan    (1000)     4033 2021-03-09 15:34:37.000000 openmdao-3.9.2/openmdao/test_suite/build4test.py
+drwxr-xr-x   0 swryan    (1000) swryan    (1000)        0 2021-05-14 19:15:32.000000 openmdao-3.9.2/openmdao/test_suite/components/
+-rw-r--r--   0 swryan    (1000) swryan    (1000)        0 2021-03-09 15:34:37.000000 openmdao-3.9.2/openmdao/test_suite/components/__init__.py
+-rw-r--r--   0 swryan    (1000) swryan    (1000)      846 2021-03-09 15:34:37.000000 openmdao-3.9.2/openmdao/test_suite/components/ae_tests.py
+-rw-r--r--   0 swryan    (1000) swryan    (1000)     1203 2021-03-09 15:34:37.000000 openmdao-3.9.2/openmdao/test_suite/components/array_comp.py
+-rw-r--r--   0 swryan    (1000) swryan    (1000)     3309 2021-03-09 15:34:37.000000 openmdao-3.9.2/openmdao/test_suite/components/branin.py
+-rw-r--r--   0 swryan    (1000) swryan    (1000)    17441 2021-03-09 15:34:37.000000 openmdao-3.9.2/openmdao/test_suite/components/cycle_comps.py
+-rw-r--r--   0 swryan    (1000) swryan    (1000)     3918 2021-03-09 15:34:37.000000 openmdao-3.9.2/openmdao/test_suite/components/distributed_components.py
+-rw-r--r--   0 swryan    (1000) swryan    (1000)     2446 2021-03-09 15:34:37.000000 openmdao-3.9.2/openmdao/test_suite/components/double_sellar.py
+-rw-r--r--   0 swryan    (1000) swryan    (1000)     1879 2021-03-09 15:34:37.000000 openmdao-3.9.2/openmdao/test_suite/components/eggcrate.py
+-rw-r--r--   0 swryan    (1000) swryan    (1000)     3000 2021-04-29 15:52:08.000000 openmdao-3.9.2/openmdao/test_suite/components/exec_comp_for_test.py
+-rw-r--r--   0 swryan    (1000) swryan    (1000)     3084 2021-05-12 14:15:10.000000 openmdao-3.9.2/openmdao/test_suite/components/expl_comp_array.py
+-rw-r--r--   0 swryan    (1000) swryan    (1000)     1767 2021-05-12 14:15:10.000000 openmdao-3.9.2/openmdao/test_suite/components/expl_comp_simple.py
+-rw-r--r--   0 swryan    (1000) swryan    (1000)     2036 2021-05-12 14:15:10.000000 openmdao-3.9.2/openmdao/test_suite/components/impl_comp_array.py
+-rw-r--r--   0 swryan    (1000) swryan    (1000)     1831 2021-03-09 15:34:37.000000 openmdao-3.9.2/openmdao/test_suite/components/impl_comp_simple.py
+-rw-r--r--   0 swryan    (1000) swryan    (1000)     3869 2021-05-12 14:15:10.000000 openmdao-3.9.2/openmdao/test_suite/components/implicit_newton_linesearch.py
+-rw-r--r--   0 swryan    (1000) swryan    (1000)     1974 2021-03-09 15:34:37.000000 openmdao-3.9.2/openmdao/test_suite/components/matmultcomp.py
+-rw-r--r--   0 swryan    (1000) swryan    (1000)     2130 2021-03-09 15:34:37.000000 openmdao-3.9.2/openmdao/test_suite/components/misc_components.py
+-rw-r--r--   0 swryan    (1000) swryan    (1000)      624 2021-03-09 15:34:37.000000 openmdao-3.9.2/openmdao/test_suite/components/options_feature_array.py
+-rw-r--r--   0 swryan    (1000) swryan    (1000)      585 2021-03-09 15:34:37.000000 openmdao-3.9.2/openmdao/test_suite/components/options_feature_function.py
+-rw-r--r--   0 swryan    (1000) swryan    (1000)      661 2021-03-09 15:34:37.000000 openmdao-3.9.2/openmdao/test_suite/components/options_feature_lincomb.py
+-rw-r--r--   0 swryan    (1000) swryan    (1000)      727 2021-03-09 15:34:37.000000 openmdao-3.9.2/openmdao/test_suite/components/options_feature_vector.py
+-rw-r--r--   0 swryan    (1000) swryan    (1000)     1642 2021-03-09 15:34:37.000000 openmdao-3.9.2/openmdao/test_suite/components/paraboloid.py
+-rw-r--r--   0 swryan    (1000) swryan    (1000)     4305 2021-03-09 15:34:37.000000 openmdao-3.9.2/openmdao/test_suite/components/paraboloid_distributed.py
+-rw-r--r--   0 swryan    (1000) swryan    (1000)     1178 2021-03-09 15:34:37.000000 openmdao-3.9.2/openmdao/test_suite/components/paraboloid_feature.py
+-rw-r--r--   0 swryan    (1000) swryan    (1000)      938 2021-03-09 15:34:37.000000 openmdao-3.9.2/openmdao/test_suite/components/paraboloid_mat_vec.py
+-rw-r--r--   0 swryan    (1000) swryan    (1000)      787 2021-03-09 15:34:37.000000 openmdao-3.9.2/openmdao/test_suite/components/paraboloid_problem.py
+-rw-r--r--   0 swryan    (1000) swryan    (1000)     1029 2021-03-09 15:34:37.000000 openmdao-3.9.2/openmdao/test_suite/components/partial_check_feature.py
+-rw-r--r--   0 swryan    (1000) swryan    (1000)     1242 2021-03-09 15:34:37.000000 openmdao-3.9.2/openmdao/test_suite/components/quad_implicit.py
+-rw-r--r--   0 swryan    (1000) swryan    (1000)    25297 2021-03-09 15:34:37.000000 openmdao-3.9.2/openmdao/test_suite/components/sellar.py
+-rw-r--r--   0 swryan    (1000) swryan    (1000)    13262 2021-03-09 15:34:37.000000 openmdao-3.9.2/openmdao/test_suite/components/sellar_feature.py
+-rw-r--r--   0 swryan    (1000) swryan    (1000)     2774 2021-03-09 15:34:37.000000 openmdao-3.9.2/openmdao/test_suite/components/simple_comps.py
+-rw-r--r--   0 swryan    (1000) swryan    (1000)     7196 2021-03-09 15:34:37.000000 openmdao-3.9.2/openmdao/test_suite/components/three_bar_truss.py
+-rw-r--r--   0 swryan    (1000) swryan    (1000)     5815 2021-03-09 15:34:37.000000 openmdao-3.9.2/openmdao/test_suite/components/unit_conv.py
+drwxr-xr-x   0 swryan    (1000) swryan    (1000)        0 2021-05-14 19:15:32.000000 openmdao-3.9.2/openmdao/test_suite/groups/
+-rw-r--r--   0 swryan    (1000) swryan    (1000)        0 2021-03-09 15:34:37.000000 openmdao-3.9.2/openmdao/test_suite/groups/__init__.py
+-rw-r--r--   0 swryan    (1000) swryan    (1000)     7879 2021-05-12 14:15:10.000000 openmdao-3.9.2/openmdao/test_suite/groups/cycle_group.py
+-rw-r--r--   0 swryan    (1000) swryan    (1000)     3395 2021-03-09 15:34:37.000000 openmdao-3.9.2/openmdao/test_suite/groups/implicit_group.py
+-rw-r--r--   0 swryan    (1000) swryan    (1000)    11058 2021-03-09 15:34:37.000000 openmdao-3.9.2/openmdao/test_suite/groups/parallel_groups.py
+-rw-r--r--   0 swryan    (1000) swryan    (1000)     1925 2021-03-09 15:34:37.000000 openmdao-3.9.2/openmdao/test_suite/groups/parametric_group.py
+-rw-r--r--   0 swryan    (1000) swryan    (1000)    10603 2021-04-29 15:52:08.000000 openmdao-3.9.2/openmdao/test_suite/groups/sin_fitter.py
+drwxr-xr-x   0 swryan    (1000) swryan    (1000)        0 2021-05-14 19:15:32.000000 openmdao-3.9.2/openmdao/test_suite/matrices/
+-rw-r--r--   0 swryan    (1000) swryan    (1000)    13814 2021-03-09 15:34:37.000000 openmdao-3.9.2/openmdao/test_suite/matrices/D_6.npz
+-rw-r--r--   0 swryan    (1000) swryan    (1000)     3697 2021-03-09 15:34:37.000000 openmdao-3.9.2/openmdao/test_suite/matrices/Harvard500.npz
+-rw-r--r--   0 swryan    (1000) swryan    (1000)    39084 2021-03-09 15:34:37.000000 openmdao-3.9.2/openmdao/test_suite/matrices/af23560.npz
+-rw-r--r--   0 swryan    (1000) swryan    (1000)     2136 2021-03-09 15:34:37.000000 openmdao-3.9.2/openmdao/test_suite/matrices/ash331.npz
+-rw-r--r--   0 swryan    (1000) swryan    (1000)     3156 2021-03-09 15:34:37.000000 openmdao-3.9.2/openmdao/test_suite/matrices/ash608.npz
+-rw-r--r--   0 swryan    (1000) swryan    (1000)     7459 2021-03-09 15:34:37.000000 openmdao-3.9.2/openmdao/test_suite/matrices/bibd_12_5.npz
+-rw-r--r--   0 swryan    (1000) swryan    (1000)     7073 2021-03-09 15:34:37.000000 openmdao-3.9.2/openmdao/test_suite/matrices/can_715.npz
+-rw-r--r--   0 swryan    (1000) swryan    (1000)     1660 2021-03-09 15:34:37.000000 openmdao-3.9.2/openmdao/test_suite/matrices/color_mats.py
+-rw-r--r--   0 swryan    (1000) swryan    (1000)      653 2021-03-09 15:34:37.000000 openmdao-3.9.2/openmdao/test_suite/matrices/dl_matrix.py
+-rw-r--r--   0 swryan    (1000) swryan    (1000)  2765232 2021-03-09 15:34:37.000000 openmdao-3.9.2/openmdao/test_suite/matrices/e40r0100.npz
+-rw-r--r--   0 swryan    (1000) swryan    (1000)    21447 2021-03-09 15:34:37.000000 openmdao-3.9.2/openmdao/test_suite/matrices/illc1033.npz
+-rw-r--r--   0 swryan    (1000) swryan    (1000)    40384 2021-03-09 15:34:37.000000 openmdao-3.9.2/openmdao/test_suite/matrices/lp_cre_a.npz
+-rw-r--r--   0 swryan    (1000) swryan    (1000)    93861 2021-03-09 15:34:37.000000 openmdao-3.9.2/openmdao/test_suite/matrices/lp_dfl001.npz
+-rw-r--r--   0 swryan    (1000) swryan    (1000)     9350 2021-03-09 15:34:37.000000 openmdao-3.9.2/openmdao/test_suite/matrices/lp_finnis.npz
+-rw-r--r--   0 swryan    (1000) swryan    (1000)    81939 2021-03-09 15:34:37.000000 openmdao-3.9.2/openmdao/test_suite/matrices/lp_maros_r7.npz
+-rw-r--r--   0 swryan    (1000) swryan    (1000)    37978 2021-03-09 15:34:37.000000 openmdao-3.9.2/openmdao/test_suite/matrices/m3plates.npz
+-rw-r--r--   0 swryan    (1000) swryan    (1000)      878 2021-03-09 15:34:37.000000 openmdao-3.9.2/openmdao/test_suite/matrices/ml2np.py
+-rw-r--r--   0 swryan    (1000) swryan    (1000)     3048 2021-03-09 15:34:37.000000 openmdao-3.9.2/openmdao/test_suite/matrices/n4c6-b15.npz
+-rw-r--r--   0 swryan    (1000) swryan    (1000)     8236 2021-03-09 15:34:37.000000 openmdao-3.9.2/openmdao/test_suite/parametric_suite.py
+drwxr-xr-x   0 swryan    (1000) swryan    (1000)        0 2021-05-14 19:15:32.000000 openmdao-3.9.2/openmdao/test_suite/scripts/
+-rw-r--r--   0 swryan    (1000) swryan    (1000)        0 2021-03-09 15:34:37.000000 openmdao-3.9.2/openmdao/test_suite/scripts/__init__.py
+-rw-r--r--   0 swryan    (1000) swryan    (1000)      685 2021-03-09 15:34:37.000000 openmdao-3.9.2/openmdao/test_suite/scripts/bad_connection.py
+-rw-r--r--   0 swryan    (1000) swryan    (1000)     1231 2021-03-09 15:34:37.000000 openmdao-3.9.2/openmdao/test_suite/scripts/beam_opt.py
+-rw-r--r--   0 swryan    (1000) swryan    (1000)      351 2021-03-09 15:34:37.000000 openmdao-3.9.2/openmdao/test_suite/scripts/circle_coloring_dynpartials.py
+-rw-r--r--   0 swryan    (1000) swryan    (1000)      503 2021-03-09 15:34:37.000000 openmdao-3.9.2/openmdao/test_suite/scripts/circle_coloring_needs_args.py
+-rw-r--r--   0 swryan    (1000) swryan    (1000)     3407 2021-03-09 15:34:37.000000 openmdao-3.9.2/openmdao/test_suite/scripts/circle_opt.py
+-rw-r--r--   0 swryan    (1000) swryan    (1000)     1530 2021-03-09 15:34:37.000000 openmdao-3.9.2/openmdao/test_suite/scripts/circuit.py
+-rw-r--r--   0 swryan    (1000) swryan    (1000)     5818 2021-03-09 15:34:37.000000 openmdao-3.9.2/openmdao/test_suite/scripts/circuit_analysis.py
+-rw-r--r--   0 swryan    (1000) swryan    (1000)     1692 2021-03-09 15:34:37.000000 openmdao-3.9.2/openmdao/test_suite/scripts/circuit_with_unconnected_input.py
+-rw-r--r--   0 swryan    (1000) swryan    (1000)     1412 2021-03-09 15:34:37.000000 openmdao-3.9.2/openmdao/test_suite/scripts/dyn_system.py
+-rw-r--r--   0 swryan    (1000) swryan    (1000)     1988 2021-03-09 15:34:37.000000 openmdao-3.9.2/openmdao/test_suite/scripts/multipoint_beam_opt.py
+-rw-r--r--   0 swryan    (1000) swryan    (1000)     2078 2021-03-09 15:34:37.000000 openmdao-3.9.2/openmdao/test_suite/scripts/sellar.py
+drwxr-xr-x   0 swryan    (1000) swryan    (1000)        0 2021-05-14 19:15:32.000000 openmdao-3.9.2/openmdao/test_suite/test_examples/
+-rw-r--r--   0 swryan    (1000) swryan    (1000)        0 2021-03-09 15:34:37.000000 openmdao-3.9.2/openmdao/test_suite/test_examples/__init__.py
+-rw-r--r--   0 swryan    (1000) swryan    (1000)     2866 2021-03-09 15:34:37.000000 openmdao-3.9.2/openmdao/test_suite/test_examples/basic_opt_paraboloid.py
+drwxr-xr-x   0 swryan    (1000) swryan    (1000)        0 2021-05-14 19:15:32.000000 openmdao-3.9.2/openmdao/test_suite/test_examples/beam_optimization/
+-rw-r--r--   0 swryan    (1000) swryan    (1000)        0 2021-03-09 15:34:37.000000 openmdao-3.9.2/openmdao/test_suite/test_examples/beam_optimization/__init__.py
+-rw-r--r--   0 swryan    (1000) swryan    (1000)     2290 2021-03-09 15:34:37.000000 openmdao-3.9.2/openmdao/test_suite/test_examples/beam_optimization/beam_group.py
+drwxr-xr-x   0 swryan    (1000) swryan    (1000)        0 2021-05-14 19:15:32.000000 openmdao-3.9.2/openmdao/test_suite/test_examples/beam_optimization/components/
+-rw-r--r--   0 swryan    (1000) swryan    (1000)        0 2021-03-09 15:34:37.000000 openmdao-3.9.2/openmdao/test_suite/test_examples/beam_optimization/components/__init__.py
+-rw-r--r--   0 swryan    (1000) swryan    (1000)      821 2021-03-09 15:34:37.000000 openmdao-3.9.2/openmdao/test_suite/test_examples/beam_optimization/components/compliance_comp.py
+-rw-r--r--   0 swryan    (1000) swryan    (1000)     1315 2021-03-09 15:34:37.000000 openmdao-3.9.2/openmdao/test_suite/test_examples/beam_optimization/components/local_stiffness_matrix_comp.py
+-rw-r--r--   0 swryan    (1000) swryan    (1000)      776 2021-03-09 15:34:37.000000 openmdao-3.9.2/openmdao/test_suite/test_examples/beam_optimization/components/moment_comp.py
+-rw-r--r--   0 swryan    (1000) swryan    (1000)     1099 2021-03-09 15:34:37.000000 openmdao-3.9.2/openmdao/test_suite/test_examples/beam_optimization/components/multi_compliance_comp.py
+-rw-r--r--   0 swryan    (1000) swryan    (1000)     4462 2021-03-09 15:34:37.000000 openmdao-3.9.2/openmdao/test_suite/test_examples/beam_optimization/components/multi_states_comp.py
+-rw-r--r--   0 swryan    (1000) swryan    (1000)     1946 2021-03-09 15:34:37.000000 openmdao-3.9.2/openmdao/test_suite/test_examples/beam_optimization/components/multi_stress_comp.py
+-rw-r--r--   0 swryan    (1000) swryan    (1000)     3776 2021-03-09 15:34:37.000000 openmdao-3.9.2/openmdao/test_suite/test_examples/beam_optimization/components/states_comp.py
+-rw-r--r--   0 swryan    (1000) swryan    (1000)      733 2021-03-09 15:34:37.000000 openmdao-3.9.2/openmdao/test_suite/test_examples/beam_optimization/components/volume_comp.py
+-rw-r--r--   0 swryan    (1000) swryan    (1000)     4936 2021-04-29 15:52:08.000000 openmdao-3.9.2/openmdao/test_suite/test_examples/beam_optimization/multipoint_beam_group.py
+-rw-r--r--   0 swryan    (1000) swryan    (1000)     5707 2021-04-29 15:52:08.000000 openmdao-3.9.2/openmdao/test_suite/test_examples/beam_optimization/multipoint_beam_stress.py
+-rw-r--r--   0 swryan    (1000) swryan    (1000)     9208 2021-03-09 15:34:37.000000 openmdao-3.9.2/openmdao/test_suite/test_examples/beam_optimization/test_beam_optimization.py
+drwxr-xr-x   0 swryan    (1000) swryan    (1000)        0 2021-05-14 19:15:32.000000 openmdao-3.9.2/openmdao/test_suite/test_examples/cannonball/
+-rw-r--r--   0 swryan    (1000) swryan    (1000)        0 2021-03-09 15:34:37.000000 openmdao-3.9.2/openmdao/test_suite/test_examples/cannonball/__init__.py
+-rw-r--r--   0 swryan    (1000) swryan    (1000)     4958 2021-03-09 15:34:37.000000 openmdao-3.9.2/openmdao/test_suite/test_examples/cannonball/cannonball_ode.py
+-rw-r--r--   0 swryan    (1000) swryan    (1000)     4107 2021-04-29 15:52:08.000000 openmdao-3.9.2/openmdao/test_suite/test_examples/cannonball/test_euler_integration.py
+drwxr-xr-x   0 swryan    (1000) swryan    (1000)        0 2021-05-14 19:15:32.000000 openmdao-3.9.2/openmdao/test_suite/test_examples/meta_model_examples/
+-rw-r--r--   0 swryan    (1000) swryan    (1000)        0 2021-03-09 15:34:37.000000 openmdao-3.9.2/openmdao/test_suite/test_examples/meta_model_examples/__init__.py
+-rw-r--r--   0 swryan    (1000) swryan    (1000)     2076 2021-03-09 15:34:37.000000 openmdao-3.9.2/openmdao/test_suite/test_examples/meta_model_examples/structured_meta_model_example.py
+-rw-r--r--   0 swryan    (1000) swryan    (1000)      711 2021-03-09 15:34:37.000000 openmdao-3.9.2/openmdao/test_suite/test_examples/meta_model_examples/unstructured_meta_model_example.py
+-rw-r--r--   0 swryan    (1000) swryan    (1000)    13847 2021-03-09 15:34:37.000000 openmdao-3.9.2/openmdao/test_suite/test_examples/test_betz_limit.py
+-rw-r--r--   0 swryan    (1000) swryan    (1000)     9895 2021-03-09 15:34:37.000000 openmdao-3.9.2/openmdao/test_suite/test_examples/test_circuit_analysis.py
+-rw-r--r--   0 swryan    (1000) swryan    (1000)     6027 2021-03-09 15:34:37.000000 openmdao-3.9.2/openmdao/test_suite/test_examples/test_circuit_analysis_derivs.py
+-rw-r--r--   0 swryan    (1000) swryan    (1000)     7020 2021-03-09 15:34:37.000000 openmdao-3.9.2/openmdao/test_suite/test_examples/test_hohmann_transfer.py
+-rw-r--r--   0 swryan    (1000) swryan    (1000)     1882 2021-03-09 15:34:37.000000 openmdao-3.9.2/openmdao/test_suite/test_examples/test_keplers_equation.py
+-rw-r--r--   0 swryan    (1000) swryan    (1000)     8345 2021-03-09 15:34:37.000000 openmdao-3.9.2/openmdao/test_suite/test_examples/test_sellar_mda_promote_connect.py
+-rw-r--r--   0 swryan    (1000) swryan    (1000)     1338 2021-03-09 15:34:37.000000 openmdao-3.9.2/openmdao/test_suite/test_examples/test_sellar_opt.py
+-rw-r--r--   0 swryan    (1000) swryan    (1000)     1304 2021-03-09 15:34:37.000000 openmdao-3.9.2/openmdao/test_suite/test_examples/test_tldr_paraboloid.py
+drwxr-xr-x   0 swryan    (1000) swryan    (1000)        0 2021-05-14 19:15:32.000000 openmdao-3.9.2/openmdao/test_suite/tests/
+-rw-r--r--   0 swryan    (1000) swryan    (1000)        0 2021-03-09 15:34:37.000000 openmdao-3.9.2/openmdao/test_suite/tests/__init__.py
+-rw-r--r--   0 swryan    (1000) swryan    (1000)     7063 2021-03-09 15:34:37.000000 openmdao-3.9.2/openmdao/test_suite/tests/test_auto_ivc_api_conversion.py
+-rw-r--r--   0 swryan    (1000) swryan    (1000)     1721 2021-03-09 15:34:37.000000 openmdao-3.9.2/openmdao/test_suite/tests/test_feature_sellar.py
+-rw-r--r--   0 swryan    (1000) swryan    (1000)     4106 2021-03-09 15:34:37.000000 openmdao-3.9.2/openmdao/test_suite/tests/test_general.py
+-rw-r--r--   0 swryan    (1000) swryan    (1000)      785 2021-03-09 15:34:37.000000 openmdao-3.9.2/openmdao/test_suite/tests/test_paraboloid_feature.py
+-rw-r--r--   0 swryan    (1000) swryan    (1000)     1074 2021-03-09 15:34:37.000000 openmdao-3.9.2/openmdao/test_suite/tests/test_quad_implicit.py
+-rw-r--r--   0 swryan    (1000) swryan    (1000)     5169 2021-05-12 14:15:10.000000 openmdao-3.9.2/openmdao/test_suite/tests/test_warnings.py
+-rw-r--r--   0 swryan    (1000) swryan    (1000)     7545 2021-03-09 15:34:37.000000 openmdao-3.9.2/openmdao/test_suite/tot_jac_builder.py
+drwxr-xr-x   0 swryan    (1000) swryan    (1000)        0 2021-05-14 19:15:32.000000 openmdao-3.9.2/openmdao/utils/
+-rw-r--r--   0 swryan    (1000) swryan    (1000)        0 2021-03-09 15:34:37.000000 openmdao-3.9.2/openmdao/utils/__init__.py
+-rw-r--r--   0 swryan    (1000) swryan    (1000)    14141 2021-05-12 14:15:10.000000 openmdao-3.9.2/openmdao/utils/array_utils.py
+-rw-r--r--   0 swryan    (1000) swryan    (1000)    19537 2021-05-12 14:15:10.000000 openmdao-3.9.2/openmdao/utils/assert_utils.py
+-rw-r--r--   0 swryan    (1000) swryan    (1000)     1908 2021-04-29 15:52:08.000000 openmdao-3.9.2/openmdao/utils/class_util.py
+-rw-r--r--   0 swryan    (1000) swryan    (1000)     8895 2021-04-29 15:52:08.000000 openmdao-3.9.2/openmdao/utils/code_utils.py
+-rw-r--r--   0 swryan    (1000) swryan    (1000)    85853 2021-05-12 14:15:10.000000 openmdao-3.9.2/openmdao/utils/coloring.py
+-rw-r--r--   0 swryan    (1000) swryan    (1000)     7329 2021-05-12 14:15:10.000000 openmdao-3.9.2/openmdao/utils/concurrent.py
+-rw-r--r--   0 swryan    (1000) swryan    (1000)     1484 2021-04-29 15:52:08.000000 openmdao-3.9.2/openmdao/utils/cs_safe.py
+-rw-r--r--   0 swryan    (1000) swryan    (1000)    14605 2021-05-12 14:15:10.000000 openmdao-3.9.2/openmdao/utils/entry_points.py
+-rw-r--r--   0 swryan    (1000) swryan    (1000)     7490 2021-05-12 14:15:10.000000 openmdao-3.9.2/openmdao/utils/file_utils.py
+-rw-r--r--   0 swryan    (1000) swryan    (1000)    33972 2021-05-14 13:26:18.000000 openmdao-3.9.2/openmdao/utils/file_wrap.py
+-rw-r--r--   0 swryan    (1000) swryan    (1000)     3182 2021-04-29 15:52:08.000000 openmdao-3.9.2/openmdao/utils/find_cite.py
+-rw-r--r--   0 swryan    (1000) swryan    (1000)    33705 2021-05-12 14:15:10.000000 openmdao-3.9.2/openmdao/utils/general_utils.py
+-rw-r--r--   0 swryan    (1000) swryan    (1000)     1240 2021-04-29 15:52:08.000000 openmdao-3.9.2/openmdao/utils/graph_utils.py
+-rw-r--r--   0 swryan    (1000) swryan    (1000)     5872 2021-04-29 15:52:08.000000 openmdao-3.9.2/openmdao/utils/hooks.py
+-rw-r--r--   0 swryan    (1000) swryan    (1000)     6426 2021-04-29 15:52:08.000000 openmdao-3.9.2/openmdao/utils/logger_utils.py
+-rw-r--r--   0 swryan    (1000) swryan    (1000)     8783 2021-05-12 14:15:10.000000 openmdao-3.9.2/openmdao/utils/mpi.py
+-rw-r--r--   0 swryan    (1000) swryan    (1000)     8628 2021-04-29 15:52:08.000000 openmdao-3.9.2/openmdao/utils/name_maps.py
+-rw-r--r--   0 swryan    (1000) swryan    (1000)     3451 2021-05-12 14:15:10.000000 openmdao-3.9.2/openmdao/utils/notebook_utils.py
+-rw-r--r--   0 swryan    (1000) swryan    (1000)    23346 2021-05-12 14:15:10.000000 openmdao-3.9.2/openmdao/utils/om.py
+-rw-r--r--   0 swryan    (1000) swryan    (1000)    16517 2021-05-12 14:15:10.000000 openmdao-3.9.2/openmdao/utils/options_dictionary.py
+-rw-r--r--   0 swryan    (1000) swryan    (1000)     6572 2021-04-29 15:52:08.000000 openmdao-3.9.2/openmdao/utils/record_util.py
+-rw-r--r--   0 swryan    (1000) swryan    (1000)     6355 2021-05-12 14:15:10.000000 openmdao-3.9.2/openmdao/utils/scaffold.py
+drwxr-xr-x   0 swryan    (1000) swryan    (1000)        0 2021-05-14 19:15:32.000000 openmdao-3.9.2/openmdao/utils/scaffolding_templates/
+-rw-r--r--   0 swryan    (1000) swryan    (1000)     3600 2021-03-09 15:34:37.000000 openmdao-3.9.2/openmdao/utils/scaffolding_templates/BaseCaseReader_template
+-rw-r--r--   0 swryan    (1000) swryan    (1000)     4303 2021-03-09 15:34:37.000000 openmdao-3.9.2/openmdao/utils/scaffolding_templates/CaseRecorder_template
+-rw-r--r--   0 swryan    (1000) swryan    (1000)     2635 2021-03-09 15:34:37.000000 openmdao-3.9.2/openmdao/utils/scaffolding_templates/Driver_template
+-rw-r--r--   0 swryan    (1000) swryan    (1000)     1814 2021-03-09 15:34:37.000000 openmdao-3.9.2/openmdao/utils/scaffolding_templates/ExplicitComponent_template
+-rw-r--r--   0 swryan    (1000) swryan    (1000)     1031 2021-03-09 15:34:37.000000 openmdao-3.9.2/openmdao/utils/scaffolding_templates/Group_template
+-rw-r--r--   0 swryan    (1000) swryan    (1000)     3888 2021-03-09 15:34:37.000000 openmdao-3.9.2/openmdao/utils/scaffolding_templates/ImplicitComponent_template
+-rw-r--r--   0 swryan    (1000) swryan    (1000)     1928 2021-03-09 15:34:37.000000 openmdao-3.9.2/openmdao/utils/scaffolding_templates/LinearSolver_template
+-rw-r--r--   0 swryan    (1000) swryan    (1000)     1836 2021-03-09 15:34:37.000000 openmdao-3.9.2/openmdao/utils/scaffolding_templates/NonlinearSolver_template
+-rw-r--r--   0 swryan    (1000) swryan    (1000)       31 2021-03-09 15:34:37.000000 openmdao-3.9.2/openmdao/utils/scaffolding_templates/README_template
+-rw-r--r--   0 swryan    (1000) swryan    (1000)     2122 2021-03-09 15:34:37.000000 openmdao-3.9.2/openmdao/utils/scaffolding_templates/SurrogateModel_template
+-rw-r--r--   0 swryan    (1000) swryan    (1000)     2265 2021-03-09 15:34:37.000000 openmdao-3.9.2/openmdao/utils/scaffolding_templates/command_template
+-rw-r--r--   0 swryan    (1000) swryan    (1000)       78 2021-03-09 15:34:37.000000 openmdao-3.9.2/openmdao/utils/scaffolding_templates/setup_template
+-rw-r--r--   0 swryan    (1000) swryan    (1000)      569 2021-03-09 15:34:37.000000 openmdao-3.9.2/openmdao/utils/scaffolding_templates/test_template
+-rw-r--r--   0 swryan    (1000) swryan    (1000)    11980 2021-04-29 15:52:08.000000 openmdao-3.9.2/openmdao/utils/shell_proc.py
+-rw-r--r--   0 swryan    (1000) swryan    (1000)     1646 2021-04-29 15:52:08.000000 openmdao-3.9.2/openmdao/utils/spline_distributions.py
+-rw-r--r--   0 swryan    (1000) swryan    (1000)     3936 2021-05-14 13:26:18.000000 openmdao-3.9.2/openmdao/utils/testing_utils.py
+drwxr-xr-x   0 swryan    (1000) swryan    (1000)        0 2021-05-14 19:15:32.000000 openmdao-3.9.2/openmdao/utils/tests/
+-rw-r--r--   0 swryan    (1000) swryan    (1000)        0 2021-03-09 15:34:37.000000 openmdao-3.9.2/openmdao/utils/tests/__init__.py
+-rw-r--r--   0 swryan    (1000) swryan    (1000)     2198 2021-03-09 15:34:37.000000 openmdao-3.9.2/openmdao/utils/tests/test_array_utils.py
+-rw-r--r--   0 swryan    (1000) swryan    (1000)     6027 2021-03-09 15:34:37.000000 openmdao-3.9.2/openmdao/utils/tests/test_assert_utils.py
+-rw-r--r--   0 swryan    (1000) swryan    (1000)     6058 2021-05-12 14:15:10.000000 openmdao-3.9.2/openmdao/utils/tests/test_cmdline.py
+-rw-r--r--   0 swryan    (1000) swryan    (1000)      586 2021-03-09 15:34:37.000000 openmdao-3.9.2/openmdao/utils/tests/test_code_utils.py
+-rw-r--r--   0 swryan    (1000) swryan    (1000)     1739 2021-03-09 15:34:37.000000 openmdao-3.9.2/openmdao/utils/tests/test_cs_safe.py
+-rw-r--r--   0 swryan    (1000) swryan    (1000)     2738 2021-03-09 15:34:37.000000 openmdao-3.9.2/openmdao/utils/tests/test_entry_points.py
+-rw-r--r--   0 swryan    (1000) swryan    (1000)    29602 2021-03-09 15:34:37.000000 openmdao-3.9.2/openmdao/utils/tests/test_file_wrap.py
+-rw-r--r--   0 swryan    (1000) swryan    (1000)     6922 2021-03-09 15:34:37.000000 openmdao-3.9.2/openmdao/utils/tests/test_find_citations.py
+-rw-r--r--   0 swryan    (1000) swryan    (1000)     1213 2021-03-09 15:34:37.000000 openmdao-3.9.2/openmdao/utils/tests/test_general_utils.py
+-rw-r--r--   0 swryan    (1000) swryan    (1000)     3087 2021-03-09 15:34:37.000000 openmdao-3.9.2/openmdao/utils/tests/test_hooks.py
+-rw-r--r--   0 swryan    (1000) swryan    (1000)    13748 2021-05-12 14:15:10.000000 openmdao-3.9.2/openmdao/utils/tests/test_options_dictionary.py
+-rw-r--r--   0 swryan    (1000) swryan    (1000)     4553 2021-03-09 15:34:37.000000 openmdao-3.9.2/openmdao/utils/tests/test_options_dictionary_feature.py
+-rw-r--r--   0 swryan    (1000) swryan    (1000)     3425 2021-03-09 15:34:37.000000 openmdao-3.9.2/openmdao/utils/tests/test_scaffold.py
+-rw-r--r--   0 swryan    (1000) swryan    (1000)     2946 2021-03-09 15:34:37.000000 openmdao-3.9.2/openmdao/utils/tests/test_shell_proc.py
+-rw-r--r--   0 swryan    (1000) swryan    (1000)     2695 2021-03-09 15:34:37.000000 openmdao-3.9.2/openmdao/utils/tests/test_spline_distributions.py
+-rw-r--r--   0 swryan    (1000) swryan    (1000)    13877 2021-05-12 14:15:10.000000 openmdao-3.9.2/openmdao/utils/tests/test_units.py
+-rw-r--r--   0 swryan    (1000) swryan    (1000)    23342 2021-05-12 14:15:10.000000 openmdao-3.9.2/openmdao/utils/tests/test_vartable.py
+-rw-r--r--   0 swryan    (1000) swryan    (1000)    10063 2021-03-09 15:34:37.000000 openmdao-3.9.2/openmdao/utils/tests/test_visualization.py
+-rw-r--r--   0 swryan    (1000) swryan    (1000)     6031 2021-03-09 15:34:37.000000 openmdao-3.9.2/openmdao/utils/unit_library.ini
+-rw-r--r--   0 swryan    (1000) swryan    (1000)    32876 2021-05-12 14:15:10.000000 openmdao-3.9.2/openmdao/utils/units.py
+-rw-r--r--   0 swryan    (1000) swryan    (1000)    11179 2021-05-12 14:15:10.000000 openmdao-3.9.2/openmdao/utils/variable_table.py
+-rw-r--r--   0 swryan    (1000) swryan    (1000)      645 2021-04-29 15:52:08.000000 openmdao-3.9.2/openmdao/utils/webview.py
+drwxr-xr-x   0 swryan    (1000) swryan    (1000)        0 2021-05-14 19:15:32.000000 openmdao-3.9.2/openmdao/vectors/
+-rw-r--r--   0 swryan    (1000) swryan    (1000)        0 2021-03-09 15:34:37.000000 openmdao-3.9.2/openmdao/vectors/__init__.py
+-rw-r--r--   0 swryan    (1000) swryan    (1000)    11203 2021-05-12 14:15:10.000000 openmdao-3.9.2/openmdao/vectors/default_transfer.py
+-rw-r--r--   0 swryan    (1000) swryan    (1000)    12476 2021-05-12 14:15:10.000000 openmdao-3.9.2/openmdao/vectors/default_vector.py
+-rw-r--r--   0 swryan    (1000) swryan    (1000)    14420 2021-05-12 14:15:10.000000 openmdao-3.9.2/openmdao/vectors/petsc_transfer.py
+-rw-r--r--   0 swryan    (1000) swryan    (1000)     7753 2021-05-12 14:15:10.000000 openmdao-3.9.2/openmdao/vectors/petsc_vector.py
+drwxr-xr-x   0 swryan    (1000) swryan    (1000)        0 2021-05-14 19:15:32.000000 openmdao-3.9.2/openmdao/vectors/tests/
+-rw-r--r--   0 swryan    (1000) swryan    (1000)        0 2021-03-09 15:34:37.000000 openmdao-3.9.2/openmdao/vectors/tests/__init__.py
+-rw-r--r--   0 swryan    (1000) swryan    (1000)     7768 2021-05-12 14:15:10.000000 openmdao-3.9.2/openmdao/vectors/tests/test_vector.py
+-rw-r--r--   0 swryan    (1000) swryan    (1000)     1803 2021-04-29 15:52:08.000000 openmdao-3.9.2/openmdao/vectors/transfer.py
+-rw-r--r--   0 swryan    (1000) swryan    (1000)    17850 2021-05-12 14:15:10.000000 openmdao-3.9.2/openmdao/vectors/vector.py
+drwxr-xr-x   0 swryan    (1000) swryan    (1000)        0 2021-05-14 19:15:32.000000 openmdao-3.9.2/openmdao/visualization/
+-rw-r--r--   0 swryan    (1000) swryan    (1000)        0 2021-03-09 15:34:37.000000 openmdao-3.9.2/openmdao/visualization/__init__.py
+drwxr-xr-x   0 swryan    (1000) swryan    (1000)        0 2021-05-14 19:15:30.000000 openmdao-3.9.2/openmdao/visualization/common/
+drwxr-xr-x   0 swryan    (1000) swryan    (1000)        0 2021-05-14 19:15:32.000000 openmdao-3.9.2/openmdao/visualization/common/libs/
+-rw-r--r--   0 swryan    (1000) swryan    (1000)   267993 2021-03-09 15:34:37.000000 openmdao-3.9.2/openmdao/visualization/common/libs/d3.v6.min.js
+-rw-r--r--   0 swryan    (1000) swryan    (1000)   106266 2021-03-09 15:34:37.000000 openmdao-3.9.2/openmdao/visualization/common/libs/jquery-3.4.1.min.js
+-rw-r--r--   0 swryan    (1000) swryan    (1000)   359216 2021-03-09 15:34:37.000000 openmdao-3.9.2/openmdao/visualization/common/libs/tabulator.min.js
+drwxr-xr-x   0 swryan    (1000) swryan    (1000)        0 2021-05-14 19:15:32.000000 openmdao-3.9.2/openmdao/visualization/common/style/
+-rwxr-xr-x   0 swryan    (1000) swryan    (1000)    22678 2021-03-09 15:34:37.000000 openmdao-3.9.2/openmdao/visualization/common/style/tabulator.min.css
+drwxr-xr-x   0 swryan    (1000) swryan    (1000)        0 2021-05-14 19:15:32.000000 openmdao-3.9.2/openmdao/visualization/connection_viewer/
+-rw-r--r--   0 swryan    (1000) swryan    (1000)        0 2021-03-09 15:34:37.000000 openmdao-3.9.2/openmdao/visualization/connection_viewer/__init__.py
+-rw-r--r--   0 swryan    (1000) swryan    (1000)     5952 2021-03-09 15:34:37.000000 openmdao-3.9.2/openmdao/visualization/connection_viewer/connect_table.html
+drwxr-xr-x   0 swryan    (1000) swryan    (1000)        0 2021-05-14 19:15:32.000000 openmdao-3.9.2/openmdao/visualization/connection_viewer/tests/
+-rw-r--r--   0 swryan    (1000) swryan    (1000)        0 2021-03-09 15:34:37.000000 openmdao-3.9.2/openmdao/visualization/connection_viewer/tests/__init__.py
+-rw-r--r--   0 swryan    (1000) swryan    (1000)     1933 2021-05-12 14:15:10.000000 openmdao-3.9.2/openmdao/visualization/connection_viewer/tests/test_viewconns.py
+-rw-r--r--   0 swryan    (1000) swryan    (1000)     6789 2021-05-12 14:15:10.000000 openmdao-3.9.2/openmdao/visualization/connection_viewer/viewconns.py
+-rw-r--r--   0 swryan    (1000) swryan    (1000)     5225 2021-05-12 14:15:10.000000 openmdao-3.9.2/openmdao/visualization/dyn_shape_plot.py
+-rw-r--r--   0 swryan    (1000) swryan    (1000)    18850 2021-05-12 14:15:10.000000 openmdao-3.9.2/openmdao/visualization/html_utils.py
+drwxr-xr-x   0 swryan    (1000) swryan    (1000)        0 2021-05-14 19:15:32.000000 openmdao-3.9.2/openmdao/visualization/meta_model_viewer/
+-rw-r--r--   0 swryan    (1000) swryan    (1000)        0 2021-03-09 15:34:37.000000 openmdao-3.9.2/openmdao/visualization/meta_model_viewer/__init__.py
+-rw-r--r--   0 swryan    (1000) swryan    (1000)    38980 2021-05-12 14:15:10.000000 openmdao-3.9.2/openmdao/visualization/meta_model_viewer/meta_model_visualization.py
+drwxr-xr-x   0 swryan    (1000) swryan    (1000)        0 2021-05-14 19:15:32.000000 openmdao-3.9.2/openmdao/visualization/meta_model_viewer/tests/
+-rw-r--r--   0 swryan    (1000) swryan    (1000)        0 2021-03-09 15:34:37.000000 openmdao-3.9.2/openmdao/visualization/meta_model_viewer/tests/__init__.py
+-rw-r--r--   0 swryan    (1000) swryan    (1000)      800 2021-03-09 15:34:37.000000 openmdao-3.9.2/openmdao/visualization/meta_model_viewer/tests/example.py
+drwxr-xr-x   0 swryan    (1000) swryan    (1000)        0 2021-05-14 19:15:32.000000 openmdao-3.9.2/openmdao/visualization/meta_model_viewer/tests/known_data_point_files/
+-rw-r--r--   0 swryan    (1000) swryan    (1000)      968 2021-03-09 15:34:37.000000 openmdao-3.9.2/openmdao/visualization/meta_model_viewer/tests/known_data_point_files/test_five_alpha_points.csv
+-rw-r--r--   0 swryan    (1000) swryan    (1000)     2763 2021-03-09 15:34:37.000000 openmdao-3.9.2/openmdao/visualization/meta_model_viewer/tests/known_data_point_files/unstructured_data_points.csv
+-rw-r--r--   0 swryan    (1000) swryan    (1000)     2524 2021-03-09 15:34:37.000000 openmdao-3.9.2/openmdao/visualization/meta_model_viewer/tests/known_data_point_files/unstructured_test_points_bottom.csv
+-rw-r--r--   0 swryan    (1000) swryan    (1000)     2481 2021-03-09 15:34:37.000000 openmdao-3.9.2/openmdao/visualization/meta_model_viewer/tests/known_data_point_files/unstructured_test_points_right.csv
+-rw-r--r--   0 swryan    (1000) swryan    (1000)     5430 2021-03-09 15:34:37.000000 openmdao-3.9.2/openmdao/visualization/meta_model_viewer/tests/known_data_point_files/updated_scatter_distance.csv
+-rw-r--r--   0 swryan    (1000) swryan    (1000)     1321 2021-03-09 15:34:37.000000 openmdao-3.9.2/openmdao/visualization/meta_model_viewer/tests/multiple_metamodels.py
+-rw-r--r--   0 swryan    (1000) swryan    (1000)    20179 2021-03-09 15:34:37.000000 openmdao-3.9.2/openmdao/visualization/meta_model_viewer/tests/test_structured.py
+-rw-r--r--   0 swryan    (1000) swryan    (1000)    12216 2021-03-09 15:34:37.000000 openmdao-3.9.2/openmdao/visualization/meta_model_viewer/tests/test_unstruct.py
+-rw-r--r--   0 swryan    (1000) swryan    (1000)     1463 2021-03-09 15:34:37.000000 openmdao-3.9.2/openmdao/visualization/meta_model_viewer/tests/test_view_mm_cmd_line.py
+drwxr-xr-x   0 swryan    (1000) swryan    (1000)        0 2021-05-14 19:15:32.000000 openmdao-3.9.2/openmdao/visualization/n2_viewer/
+-rw-r--r--   0 swryan    (1000) swryan    (1000)        0 2021-03-09 15:34:37.000000 openmdao-3.9.2/openmdao/visualization/n2_viewer/__init__.py
+drwxr-xr-x   0 swryan    (1000) swryan    (1000)        0 2021-05-14 19:15:32.000000 openmdao-3.9.2/openmdao/visualization/n2_viewer/assets/
+-rw-r--r--   0 swryan    (1000) swryan    (1000)    13359 2021-03-09 15:34:37.000000 openmdao-3.9.2/openmdao/visualization/n2_viewer/assets/logo.png
+-rw-r--r--   0 swryan    (1000) swryan    (1000)    15592 2021-03-15 19:14:32.000000 openmdao-3.9.2/openmdao/visualization/n2_viewer/assets/n2toolbar_screenshot_png.b64
+-rw-r--r--   0 swryan    (1000) swryan    (1000)    91128 2021-03-09 15:34:37.000000 openmdao-3.9.2/openmdao/visualization/n2_viewer/assets/spinner.png
+-rw-r--r--   0 swryan    (1000) swryan    (1000)    14095 2021-05-12 14:15:10.000000 openmdao-3.9.2/openmdao/visualization/n2_viewer/index.html
+drwxr-xr-x   0 swryan    (1000) swryan    (1000)        0 2021-05-14 19:15:32.000000 openmdao-3.9.2/openmdao/visualization/n2_viewer/libs/
+-rw-r--r--   0 swryan    (1000) swryan    (1000)     9483 2021-03-09 15:34:37.000000 openmdao-3.9.2/openmdao/visualization/n2_viewer/libs/awesomplete.js
+-rw-r--r--   0 swryan    (1000) swryan    (1000)   511371 2021-03-09 15:34:37.000000 openmdao-3.9.2/openmdao/visualization/n2_viewer/libs/d3.js
+-rw-r--r--   0 swryan    (1000) swryan    (1000)   246120 2021-03-09 15:34:37.000000 openmdao-3.9.2/openmdao/visualization/n2_viewer/libs/d3.v5.min.js
+-rw-r--r--   0 swryan    (1000) swryan    (1000)    31305 2021-05-12 14:15:10.000000 openmdao-3.9.2/openmdao/visualization/n2_viewer/libs/json5_2.2.0.min.js
+-rw-r--r--   0 swryan    (1000) swryan    (1000)    24324 2021-03-09 15:34:37.000000 openmdao-3.9.2/openmdao/visualization/n2_viewer/libs/pako_inflate.min.js
+-rw-r--r--   0 swryan    (1000) swryan    (1000)     4679 2021-03-09 15:34:37.000000 openmdao-3.9.2/openmdao/visualization/n2_viewer/libs/vkBeautify.js
+-rw-r--r--   0 swryan    (1000) swryan    (1000)    24133 2021-05-12 14:15:10.000000 openmdao-3.9.2/openmdao/visualization/n2_viewer/n2_viewer.py
+drwxr-xr-x   0 swryan    (1000) swryan    (1000)        0 2021-05-14 19:15:32.000000 openmdao-3.9.2/openmdao/visualization/n2_viewer/src/
+-rw-r--r--   0 swryan    (1000) swryan    (1000)    16299 2021-05-12 14:15:10.000000 openmdao-3.9.2/openmdao/visualization/n2_viewer/src/ModelData.js
+-rw-r--r--   0 swryan    (1000) swryan    (1000)    39388 2021-03-09 15:34:37.000000 openmdao-3.9.2/openmdao/visualization/n2_viewer/src/N2Arrow.js
+-rw-r--r--   0 swryan    (1000) swryan    (1000)    38862 2021-03-15 19:14:32.000000 openmdao-3.9.2/openmdao/visualization/n2_viewer/src/N2Diagram.js
+-rw-r--r--   0 swryan    (1000) swryan    (1000)     1167 2021-03-09 15:34:37.000000 openmdao-3.9.2/openmdao/visualization/n2_viewer/src/N2ErrorHandling.js
+-rw-r--r--   0 swryan    (1000) swryan    (1000)    24044 2021-03-09 15:34:37.000000 openmdao-3.9.2/openmdao/visualization/n2_viewer/src/N2Layout.js
+-rw-r--r--   0 swryan    (1000) swryan    (1000)    13448 2021-05-12 14:15:10.000000 openmdao-3.9.2/openmdao/visualization/n2_viewer/src/N2Legend.js
+-rw-r--r--   0 swryan    (1000) swryan    (1000)    35360 2021-03-09 15:34:37.000000 openmdao-3.9.2/openmdao/visualization/n2_viewer/src/N2Matrix.js
+-rw-r--r--   0 swryan    (1000) swryan    (1000)    22419 2021-03-15 19:14:32.000000 openmdao-3.9.2/openmdao/visualization/n2_viewer/src/N2MatrixCell.js
+-rw-r--r--   0 swryan    (1000) swryan    (1000)    11228 2021-03-15 19:14:32.000000 openmdao-3.9.2/openmdao/visualization/n2_viewer/src/N2Search.js
+-rw-r--r--   0 swryan    (1000) swryan    (1000)    10678 2021-03-09 15:34:37.000000 openmdao-3.9.2/openmdao/visualization/n2_viewer/src/N2Style.js
+-rw-r--r--   0 swryan    (1000) swryan    (1000)    19011 2021-03-15 19:14:32.000000 openmdao-3.9.2/openmdao/visualization/n2_viewer/src/N2Toolbar.js
+-rw-r--r--   0 swryan    (1000) swryan    (1000)     9871 2021-03-15 19:14:32.000000 openmdao-3.9.2/openmdao/visualization/n2_viewer/src/N2TreeNode.js
+-rw-r--r--   0 swryan    (1000) swryan    (1000)    30934 2021-05-12 14:15:10.000000 openmdao-3.9.2/openmdao/visualization/n2_viewer/src/N2UserInterface.js
+-rw-r--r--   0 swryan    (1000) swryan    (1000)    23433 2021-03-15 19:14:32.000000 openmdao-3.9.2/openmdao/visualization/n2_viewer/src/N2Window.js
+-rw-r--r--   0 swryan    (1000) swryan    (1000)    21076 2021-03-09 15:34:37.000000 openmdao-3.9.2/openmdao/visualization/n2_viewer/src/NodeInfo.js
+-rw-r--r--   0 swryan    (1000) swryan    (1000)     3877 2021-03-09 15:34:37.000000 openmdao-3.9.2/openmdao/visualization/n2_viewer/src/SymbolType.js
+-rw-r--r--   0 swryan    (1000) swryan    (1000)     2055 2021-05-12 14:15:10.000000 openmdao-3.9.2/openmdao/visualization/n2_viewer/src/defaults.js
+-rw-r--r--   0 swryan    (1000) swryan    (1000)      423 2021-03-09 15:34:37.000000 openmdao-3.9.2/openmdao/visualization/n2_viewer/src/ptN2.js
+-rw-r--r--   0 swryan    (1000) swryan    (1000)     4132 2021-03-09 15:34:37.000000 openmdao-3.9.2/openmdao/visualization/n2_viewer/src/utils.js
+drwxr-xr-x   0 swryan    (1000) swryan    (1000)        0 2021-05-14 19:15:32.000000 openmdao-3.9.2/openmdao/visualization/n2_viewer/style/
+-rw-r--r--   0 swryan    (1000) swryan    (1000)     1938 2021-03-09 15:34:37.000000 openmdao-3.9.2/openmdao/visualization/n2_viewer/style/awesomplete.css
+-rw-r--r--   0 swryan    (1000) swryan    (1000)     3749 2021-03-15 19:14:32.000000 openmdao-3.9.2/openmdao/visualization/n2_viewer/style/legend.css
+-rw-r--r--   0 swryan    (1000) swryan    (1000)    17812 2021-03-09 15:34:37.000000 openmdao-3.9.2/openmdao/visualization/n2_viewer/style/logo_png.b64
+-rw-r--r--   0 swryan    (1000) swryan    (1000)     4588 2021-03-15 19:14:32.000000 openmdao-3.9.2/openmdao/visualization/n2_viewer/style/n2toolbar-icons-font.woff
+-rw-r--r--   0 swryan    (1000) swryan    (1000)     2673 2021-03-15 19:14:32.000000 openmdao-3.9.2/openmdao/visualization/n2_viewer/style/n2toolbar-icons.css
+-rw-r--r--   0 swryan    (1000) swryan    (1000)     5415 2021-03-15 19:14:32.000000 openmdao-3.9.2/openmdao/visualization/n2_viewer/style/partition_tree.css
+-rw-r--r--   0 swryan    (1000) swryan    (1000)     8433 2021-05-12 14:15:10.000000 openmdao-3.9.2/openmdao/visualization/n2_viewer/style/toolbar.css
+-rw-r--r--   0 swryan    (1000) swryan    (1000)    16643 2021-03-15 19:14:32.000000 openmdao-3.9.2/openmdao/visualization/n2_viewer/style/window.css
+drwxr-xr-x   0 swryan    (1000) swryan    (1000)        0 2021-05-14 19:15:32.000000 openmdao-3.9.2/openmdao/visualization/n2_viewer/tests/
+-rw-r--r--   0 swryan    (1000) swryan    (1000)        0 2021-03-09 15:34:37.000000 openmdao-3.9.2/openmdao/visualization/n2_viewer/tests/__init__.py
+-rw-r--r--   0 swryan    (1000) swryan    (1000)     7997 2021-05-12 14:15:10.000000 openmdao-3.9.2/openmdao/visualization/n2_viewer/tests/betz_tree.json
+drwxr-xr-x   0 swryan    (1000) swryan    (1000)        0 2021-05-14 19:15:32.000000 openmdao-3.9.2/openmdao/visualization/n2_viewer/tests/gui_test_models/
+-rw-r--r--   0 swryan    (1000) swryan    (1000)     1491 2021-03-09 15:34:37.000000 openmdao-3.9.2/openmdao/visualization/n2_viewer/tests/gui_test_models/bug_arrow.py
+-rw-r--r--   0 swryan    (1000) swryan    (1000)     4766 2021-03-09 15:34:37.000000 openmdao-3.9.2/openmdao/visualization/n2_viewer/tests/gui_test_models/circuit.py
+-rw-r--r--   0 swryan    (1000) swryan    (1000)      690 2021-03-09 15:34:37.000000 openmdao-3.9.2/openmdao/visualization/n2_viewer/tests/gui_test_models/double_sellar.py
+-rw-r--r--   0 swryan    (1000) swryan    (1000)      544 2021-03-09 15:34:37.000000 openmdao-3.9.2/openmdao/visualization/n2_viewer/tests/gui_test_models/nan_value.py
+-rw-r--r--   0 swryan    (1000) swryan    (1000)      790 2021-03-09 15:34:37.000000 openmdao-3.9.2/openmdao/visualization/n2_viewer/tests/gui_test_models/parabaloid.py
+-rw-r--r--   0 swryan    (1000) swryan    (1000)      955 2021-03-09 15:34:37.000000 openmdao-3.9.2/openmdao/visualization/n2_viewer/tests/gui_test_models/valuewin2.py
+-rw-r--r--   0 swryan    (1000) swryan    (1000)    30212 2021-05-12 14:15:10.000000 openmdao-3.9.2/openmdao/visualization/n2_viewer/tests/n2_gui_test.py
+-rw-r--r--   0 swryan    (1000) swryan    (1000)    18229 2021-05-12 14:15:10.000000 openmdao-3.9.2/openmdao/visualization/n2_viewer/tests/sellar_tree.json
+-rw-r--r--   0 swryan    (1000) swryan    (1000)     2315 2021-03-09 15:34:37.000000 openmdao-3.9.2/openmdao/visualization/n2_viewer/tests/test_gui.py
+-rw-r--r--   0 swryan    (1000) swryan    (1000)     9002 2021-03-09 15:34:37.000000 openmdao-3.9.2/openmdao/visualization/n2_viewer/tests/test_n2_viewer.py
+-rw-r--r--   0 swryan    (1000) swryan    (1000)     1763 2021-03-09 15:34:37.000000 openmdao-3.9.2/openmdao/visualization/n2_viewer/tests/test_parallel_n2.py
+-rw-r--r--   0 swryan    (1000) swryan    (1000)     5247 2021-03-09 15:34:37.000000 openmdao-3.9.2/openmdao/visualization/n2_viewer/tests/test_serialization.py
+-rw-r--r--   0 swryan    (1000) swryan    (1000)    23728 2021-05-12 14:15:10.000000 openmdao-3.9.2/openmdao/visualization/n2_viewer/tests/test_viewmodeldata.py
+-rw-r--r--   0 swryan    (1000) swryan    (1000)     4802 2021-04-29 15:52:08.000000 openmdao-3.9.2/openmdao/visualization/partial_deriv_plot.py
+drwxr-xr-x   0 swryan    (1000) swryan    (1000)        0 2021-05-14 19:15:32.000000 openmdao-3.9.2/openmdao/visualization/scaling_viewer/
+-rw-r--r--   0 swryan    (1000) swryan    (1000)        0 2021-03-09 15:34:37.000000 openmdao-3.9.2/openmdao/visualization/scaling_viewer/__init__.py
+-rw-r--r--   0 swryan    (1000) swryan    (1000)    18945 2021-04-29 15:52:08.000000 openmdao-3.9.2/openmdao/visualization/scaling_viewer/scaling_report.py
+-rw-r--r--   0 swryan    (1000) swryan    (1000)    22001 2021-03-09 15:34:37.000000 openmdao-3.9.2/openmdao/visualization/scaling_viewer/scaling_table.html
+-rw-r--r--   0 swryan    (1000) swryan    (1000)     8957 2021-05-12 14:15:10.000000 openmdao-3.9.2/openmdao/warnings.py
+drwxr-xr-x   0 swryan    (1000) swryan    (1000)        0 2021-05-14 19:15:30.000000 openmdao-3.9.2/openmdao.egg-info/
+-rw-r--r--   0 swryan    (1000) swryan    (1000)     1496 2021-05-14 19:15:29.000000 openmdao-3.9.2/openmdao.egg-info/PKG-INFO
+-rw-r--r--   0 swryan    (1000) swryan    (1000)    25895 2021-05-14 19:15:30.000000 openmdao-3.9.2/openmdao.egg-info/SOURCES.txt
+-rw-r--r--   0 swryan    (1000) swryan    (1000)        1 2021-05-14 19:15:29.000000 openmdao-3.9.2/openmdao.egg-info/dependency_links.txt
+-rw-r--r--   0 swryan    (1000) swryan    (1000)     3740 2021-05-14 19:15:29.000000 openmdao-3.9.2/openmdao.egg-info/entry_points.txt
+-rw-r--r--   0 swryan    (1000) swryan    (1000)      577 2021-05-14 19:15:29.000000 openmdao-3.9.2/openmdao.egg-info/requires.txt
+-rw-r--r--   0 swryan    (1000) swryan    (1000)        9 2021-05-14 19:15:29.000000 openmdao-3.9.2/openmdao.egg-info/top_level.txt
+-rw-r--r--   0 swryan    (1000) swryan    (1000)       38 2021-05-14 19:15:32.000000 openmdao-3.9.2/setup.cfg
+-rw-r--r--   0 swryan    (1000) swryan    (1000)     9864 2021-05-12 14:15:10.000000 openmdao-3.9.2/setup.py
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive
+POSIX tar archive (GNU)
```

### Comparing `openmdao-3.9.1/LICENSE.txt` & `openmdao-3.9.2/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `openmdao-3.9.1/PKG-INFO` & `openmdao-3.9.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: openmdao
-Version: 3.9.1
+Version: 3.9.2
 Summary: OpenMDAO framework infrastructure
 Home-page: http://openmdao.org
 Author: OpenMDAO Team
 Author-email: openmdao@openmdao.org
 License: Apache License, Version 2.0
 Description: OpenMDAO is an open-source high-performance computing platform
             for systems analysis and multidisciplinary optimization, written in Python. It
```

### Comparing `openmdao-3.9.1/README.md` & `openmdao-3.9.2/README.md`

 * *Files identical despite different names*

### Comparing `openmdao-3.9.1/openmdao/api.py` & `openmdao-3.9.2/openmdao/api.py`

 * *Files identical despite different names*

### Comparing `openmdao-3.9.1/openmdao/approximation_schemes/approximation_scheme.py` & `openmdao-3.9.2/openmdao/approximation_schemes/approximation_scheme.py`

 * *Files identical despite different names*

### Comparing `openmdao-3.9.1/openmdao/approximation_schemes/complex_step.py` & `openmdao-3.9.2/openmdao/approximation_schemes/complex_step.py`

 * *Files identical despite different names*

### Comparing `openmdao-3.9.1/openmdao/approximation_schemes/finite_difference.py` & `openmdao-3.9.2/openmdao/approximation_schemes/finite_difference.py`

 * *Files identical despite different names*

### Comparing `openmdao-3.9.1/openmdao/code_review/test_lint_attributes.py` & `openmdao-3.9.2/openmdao/code_review/test_lint_attributes.py`

 * *Files identical despite different names*

### Comparing `openmdao-3.9.1/openmdao/code_review/test_lint_docstrings.py` & `openmdao-3.9.2/openmdao/code_review/test_lint_docstrings.py`

 * *Files identical despite different names*

### Comparing `openmdao-3.9.1/openmdao/code_review/test_lint_peps.py` & `openmdao-3.9.2/openmdao/code_review/test_lint_peps.py`

 * *Files identical despite different names*

### Comparing `openmdao-3.9.1/openmdao/components/add_subtract_comp.py` & `openmdao-3.9.2/openmdao/components/add_subtract_comp.py`

 * *Files identical despite different names*

### Comparing `openmdao-3.9.1/openmdao/components/balance_comp.py` & `openmdao-3.9.2/openmdao/components/balance_comp.py`

 * *Files identical despite different names*

### Comparing `openmdao-3.9.1/openmdao/components/cross_product_comp.py` & `openmdao-3.9.2/openmdao/components/cross_product_comp.py`

 * *Files identical despite different names*

### Comparing `openmdao-3.9.1/openmdao/components/demux_comp.py` & `openmdao-3.9.2/openmdao/components/demux_comp.py`

 * *Files 1% similar despite different names*

```diff
@@ -101,15 +101,15 @@
             self.add_output(name=out_name,
                             val=options['val'],
                             shape=out_shape,
                             units=options['units'],
                             desc=options['desc'])
 
             rs = np.arange(np.prod(out_shape))
-            cs = np.atleast_1d(np.take(template, indices=i, axis=axis))
+            cs = np.atleast_1d(np.take(template, indices=i, axis=axis)).flatten()
 
             self.declare_partials(of=out_name, wrt=name, rows=rs, cols=cs, val=1.0)
 
     def compute(self, inputs, outputs):
         """
         Demux the inputs into the appropriate outputs using numpy.take.
```

### Comparing `openmdao-3.9.1/openmdao/components/dot_product_comp.py` & `openmdao-3.9.2/openmdao/components/dot_product_comp.py`

 * *Files identical despite different names*

### Comparing `openmdao-3.9.1/openmdao/components/eq_constraint_comp.py` & `openmdao-3.9.2/openmdao/components/eq_constraint_comp.py`

 * *Files identical despite different names*

### Comparing `openmdao-3.9.1/openmdao/components/exec_comp.py` & `openmdao-3.9.2/openmdao/components/exec_comp.py`

 * *Files identical despite different names*

### Comparing `openmdao-3.9.1/openmdao/components/external_code_comp.py` & `openmdao-3.9.2/openmdao/components/external_code_comp.py`

 * *Files identical despite different names*

### Comparing `openmdao-3.9.1/openmdao/components/interp_util/interp.py` & `openmdao-3.9.2/openmdao/components/interp_util/interp.py`

 * *Files identical despite different names*

### Comparing `openmdao-3.9.1/openmdao/components/interp_util/interp_akima.py` & `openmdao-3.9.2/openmdao/components/interp_util/interp_akima.py`

 * *Files identical despite different names*

### Comparing `openmdao-3.9.1/openmdao/components/interp_util/interp_algorithm.py` & `openmdao-3.9.2/openmdao/components/interp_util/interp_algorithm.py`

 * *Files identical despite different names*

### Comparing `openmdao-3.9.1/openmdao/components/interp_util/interp_bsplines.py` & `openmdao-3.9.2/openmdao/components/interp_util/interp_bsplines.py`

 * *Files identical despite different names*

### Comparing `openmdao-3.9.1/openmdao/components/interp_util/interp_cubic.py` & `openmdao-3.9.2/openmdao/components/interp_util/interp_cubic.py`

 * *Files identical despite different names*

### Comparing `openmdao-3.9.1/openmdao/components/interp_util/interp_lagrange2.py` & `openmdao-3.9.2/openmdao/components/interp_util/interp_lagrange2.py`

 * *Files identical despite different names*

### Comparing `openmdao-3.9.1/openmdao/components/interp_util/interp_lagrange3.py` & `openmdao-3.9.2/openmdao/components/interp_util/interp_lagrange3.py`

 * *Files identical despite different names*

### Comparing `openmdao-3.9.1/openmdao/components/interp_util/interp_scipy.py` & `openmdao-3.9.2/openmdao/components/interp_util/interp_scipy.py`

 * *Files identical despite different names*

### Comparing `openmdao-3.9.1/openmdao/components/interp_util/interp_slinear.py` & `openmdao-3.9.2/openmdao/components/interp_util/interp_slinear.py`

 * *Files identical despite different names*

### Comparing `openmdao-3.9.1/openmdao/components/interp_util/outofbounds_error.py` & `openmdao-3.9.2/openmdao/components/interp_util/outofbounds_error.py`

 * *Files identical despite different names*

### Comparing `openmdao-3.9.1/openmdao/components/interp_util/tests/test_interp_nd.py` & `openmdao-3.9.2/openmdao/components/interp_util/tests/test_interp_nd.py`

 * *Files identical despite different names*

### Comparing `openmdao-3.9.1/openmdao/components/ks_comp.py` & `openmdao-3.9.2/openmdao/components/ks_comp.py`

 * *Files identical despite different names*

### Comparing `openmdao-3.9.1/openmdao/components/linear_system_comp.py` & `openmdao-3.9.2/openmdao/components/linear_system_comp.py`

 * *Files identical despite different names*

### Comparing `openmdao-3.9.1/openmdao/components/matrix_vector_product_comp.py` & `openmdao-3.9.2/openmdao/components/matrix_vector_product_comp.py`

 * *Files identical despite different names*

### Comparing `openmdao-3.9.1/openmdao/components/meta_model_structured_comp.py` & `openmdao-3.9.2/openmdao/components/meta_model_structured_comp.py`

 * *Files identical despite different names*

### Comparing `openmdao-3.9.1/openmdao/components/meta_model_unstructured_comp.py` & `openmdao-3.9.2/openmdao/components/meta_model_unstructured_comp.py`

 * *Files 0% similar despite different names*

```diff
@@ -581,14 +581,15 @@
             if isinstance(val[0], float):
                 inputs[:, idx] = val
                 idx += 1
             else:
                 for row_idx, v in enumerate(val):
                     v = np.asarray(v)
                     inputs[row_idx, idx:idx + sz] = v.flat
+                idx += sz
 
         # Assemble output data and train each output.
         for name, shape in self._surrogate_output_names:
             output_size = np.prod(shape)
 
             outputs = np.zeros((num_sample, output_size))
             self._training_output[name] = outputs
```

### Comparing `openmdao-3.9.1/openmdao/components/multifi_meta_model_unstructured_comp.py` & `openmdao-3.9.2/openmdao/components/multifi_meta_model_unstructured_comp.py`

 * *Files identical despite different names*

### Comparing `openmdao-3.9.1/openmdao/components/mux_comp.py` & `openmdao-3.9.2/openmdao/components/mux_comp.py`

 * *Files identical despite different names*

### Comparing `openmdao-3.9.1/openmdao/components/spline_comp.py` & `openmdao-3.9.2/openmdao/components/spline_comp.py`

 * *Files identical despite different names*

### Comparing `openmdao-3.9.1/openmdao/components/tests/extcode_example.py` & `openmdao-3.9.2/openmdao/components/tests/extcode_example.py`

 * *Files identical despite different names*

### Comparing `openmdao-3.9.1/openmdao/components/tests/extcode_mach.py` & `openmdao-3.9.2/openmdao/components/tests/extcode_mach.py`

 * *Files identical despite different names*

### Comparing `openmdao-3.9.1/openmdao/components/tests/extcode_node.py` & `openmdao-3.9.2/openmdao/components/tests/extcode_node.py`

 * *Files identical despite different names*

### Comparing `openmdao-3.9.1/openmdao/components/tests/extcode_paraboloid.py` & `openmdao-3.9.2/openmdao/components/tests/extcode_paraboloid.py`

 * *Files identical despite different names*

### Comparing `openmdao-3.9.1/openmdao/components/tests/extcode_paraboloid_derivs.py` & `openmdao-3.9.2/openmdao/components/tests/extcode_paraboloid_derivs.py`

 * *Files identical despite different names*

### Comparing `openmdao-3.9.1/openmdao/components/tests/extcode_resistor.py` & `openmdao-3.9.2/openmdao/components/tests/extcode_resistor.py`

 * *Files identical despite different names*

### Comparing `openmdao-3.9.1/openmdao/components/tests/test_add_subtract_comp.py` & `openmdao-3.9.2/openmdao/components/tests/test_add_subtract_comp.py`

 * *Files identical despite different names*

### Comparing `openmdao-3.9.1/openmdao/components/tests/test_balance_comp.py` & `openmdao-3.9.2/openmdao/components/tests/test_balance_comp.py`

 * *Files identical despite different names*

### Comparing `openmdao-3.9.1/openmdao/components/tests/test_cross_product_comp.py` & `openmdao-3.9.2/openmdao/components/tests/test_cross_product_comp.py`

 * *Files identical despite different names*

### Comparing `openmdao-3.9.1/openmdao/components/tests/test_demux_comp.py` & `openmdao-3.9.2/openmdao/components/tests/test_demux_comp.py`

 * *Files 20% similar despite different names*

```diff
@@ -135,14 +135,108 @@
             assert_near_equal(in_i, out_i)
 
     def test_partials(self):
         np.set_printoptions(linewidth=1024)
         cpd = self.p.check_partials(compact_print=False, method='cs', out_stream=None)
         assert_check_partials(cpd, atol=1.0E-8, rtol=1.0E-8)
 
+class TestDemuxComp3D(unittest.TestCase):
+
+    def setUp(self):
+        self.nn = 10
+
+        self.p = om.Problem()
+
+        ivc = om.IndepVarComp()
+        ivc.add_output(name='a', shape=(self.nn, 7, 3))
+        ivc.add_output(name='b', shape=(3, self.nn))
+
+        self.p.model.add_subsystem(name='ivc',
+                                   subsys=ivc,
+                                   promotes_outputs=['a', 'b'])
+
+        demux_comp = self.p.model.add_subsystem(name='demux_comp',
+                                                subsys=om.DemuxComp(vec_size=self.nn))
+
+        demux_comp.add_var('a', shape=(self.nn, 7, 3), axis=0)
+        demux_comp.add_var('b', shape=(3, self.nn), axis=1)
+
+        self.p.model.connect('a', 'demux_comp.a')
+        self.p.model.connect('b', 'demux_comp.b')
+
+        self.p.setup(force_alloc_complex=True)
+
+        self.p['a'] = np.random.rand(self.nn, 7, 3)
+        self.p['b'] = np.random.rand(3, self.nn)
+
+        self.p.run_model()
+
+    def test_results(self):
+
+        for i in range(self.nn):
+            in_i = np.take(self.p['a'], indices=i, axis=0)
+            out_i = self.p['demux_comp.a_{0}'.format(i)]
+            assert_near_equal(in_i, out_i)
+
+            in_i = np.take(self.p['b'], indices=i, axis=1)
+            out_i = self.p['demux_comp.b_{0}'.format(i)]
+            assert_near_equal(in_i, out_i)
+
+    def test_partials(self):
+        np.set_printoptions(linewidth=1024)
+        cpd = self.p.check_partials(compact_print=False, method='cs', out_stream=None)
+        assert_check_partials(cpd, atol=1.0E-8, rtol=1.0E-8)
+
+class TestDemuxComp4D(unittest.TestCase):
+
+    def setUp(self):
+        self.nn = 10
+
+        self.p = om.Problem()
+
+        ivc = om.IndepVarComp()
+        ivc.add_output(name='a', shape=(self.nn, 7, 3, 4))
+        ivc.add_output(name='b', shape=(3, self.nn))
+
+        self.p.model.add_subsystem(name='ivc',
+                                   subsys=ivc,
+                                   promotes_outputs=['a', 'b'])
+
+        demux_comp = self.p.model.add_subsystem(name='demux_comp',
+                                                subsys=om.DemuxComp(vec_size=self.nn))
+
+        demux_comp.add_var('a', shape=(self.nn, 7, 3, 4), axis=0)
+        demux_comp.add_var('b', shape=(3, self.nn), axis=1)
+
+        self.p.model.connect('a', 'demux_comp.a')
+        self.p.model.connect('b', 'demux_comp.b')
+
+        self.p.setup(force_alloc_complex=True)
+
+        self.p['a'] = np.random.rand(self.nn, 7, 3, 4)
+        self.p['b'] = np.random.rand(3, self.nn)
+
+        self.p.run_model()
+
+    def test_results(self):
+
+        for i in range(self.nn):
+            in_i = np.take(self.p['a'], indices=i, axis=0)
+            out_i = self.p['demux_comp.a_{0}'.format(i)]
+            assert_near_equal(in_i, out_i)
+
+            in_i = np.take(self.p['b'], indices=i, axis=1)
+            out_i = self.p['demux_comp.b_{0}'.format(i)]
+            assert_near_equal(in_i, out_i)
+
+    def test_partials(self):
+        np.set_printoptions(linewidth=1024)
+        cpd = self.p.check_partials(compact_print=False, method='cs', out_stream=None)
+        assert_check_partials(cpd, atol=1.0E-8, rtol=1.0E-8)
+
 
 class TestFeature(unittest.TestCase):
 
     def test(self):
         """
         An example demonstrating a trivial use case of DemuxComp
         """
```

### Comparing `openmdao-3.9.1/openmdao/components/tests/test_dot_product_comp.py` & `openmdao-3.9.2/openmdao/components/tests/test_dot_product_comp.py`

 * *Files identical despite different names*

### Comparing `openmdao-3.9.1/openmdao/components/tests/test_eq_constraint_comp.py` & `openmdao-3.9.2/openmdao/components/tests/test_eq_constraint_comp.py`

 * *Files identical despite different names*

### Comparing `openmdao-3.9.1/openmdao/components/tests/test_exec_comp.py` & `openmdao-3.9.2/openmdao/components/tests/test_exec_comp.py`

 * *Files identical despite different names*

### Comparing `openmdao-3.9.1/openmdao/components/tests/test_external_code_comp.py` & `openmdao-3.9.2/openmdao/components/tests/test_external_code_comp.py`

 * *Files identical despite different names*

### Comparing `openmdao-3.9.1/openmdao/components/tests/test_ks_comp.py` & `openmdao-3.9.2/openmdao/components/tests/test_ks_comp.py`

 * *Files identical despite different names*

### Comparing `openmdao-3.9.1/openmdao/components/tests/test_linear_system_comp.py` & `openmdao-3.9.2/openmdao/components/tests/test_linear_system_comp.py`

 * *Files identical despite different names*

### Comparing `openmdao-3.9.1/openmdao/components/tests/test_matrix_vector_product_comp.py` & `openmdao-3.9.2/openmdao/components/tests/test_matrix_vector_product_comp.py`

 * *Files identical despite different names*

### Comparing `openmdao-3.9.1/openmdao/components/tests/test_meta_model_structured_comp.py` & `openmdao-3.9.2/openmdao/components/tests/test_meta_model_structured_comp.py`

 * *Files identical despite different names*

### Comparing `openmdao-3.9.1/openmdao/components/tests/test_meta_model_unstructured_comp.py` & `openmdao-3.9.2/openmdao/components/tests/test_meta_model_unstructured_comp.py`

 * *Files 6% similar despite different names*

```diff
@@ -233,14 +233,51 @@
 
         prob['mm.x'] = [1.0, 2.0, 1.0, 1.0]
         prob.run_model()
 
         assert_near_equal(prob['mm.y1'], 1.0, .00001)
         assert_near_equal(prob['mm.y2'], 7.0, .00001)
 
+    def test_two_vector_inputs(self):
+        mm = om.MetaModelUnStructuredComp()
+        mm.add_input('x1', np.zeros(4))
+        mm.add_input('x2', np.zeros(4))
+        mm.add_output('y1', 0.)
+        mm.add_output('y2', 0.)
+
+        mm.options['default_surrogate'] = om.KrigingSurrogate()
+
+        prob = om.Problem()
+        prob.model.add_subsystem('mm', mm)
+        prob.setup()
+
+        mm.options['train:x1'] = [
+            [1.0, 1.0, 1.0, 1.0],
+            [2.0, 1.0, 1.0, 1.0],
+            [1.0, 2.0, 1.0, 1.0],
+            [1.0, 1.0, 2.0, 1.0],
+            [1.0, 1.0, 1.0, 2.0]
+        ]
+        mm.options['train:x2'] = [
+            [1.0, 1.0, 1.0, 1.0],
+            [2.0, 1.0, 1.0, 1.0],
+            [1.0, 2.0, 1.0, 1.0],
+            [1.0, 1.0, 2.0, 1.0],
+            [1.0, 1.0, 1.0, 2.0]
+        ]
+        mm.options['train:y1'] = [3.0, 2.0, 1.0, 6.0, -2.0]
+        mm.options['train:y2'] = [1.0, 4.0, 7.0, -3.0, 3.0]
+
+        prob['mm.x1'] = [1.0, 2.0, 1.0, 1.0]
+        prob['mm.x2'] = [1.0, 2.0, 1.0, 1.0]
+        prob.run_model()
+
+        assert_near_equal(prob['mm.y1'], 1.0, .00001)
+        assert_near_equal(prob['mm.y2'], 7.0, .00001)
+
     def test_array_inputs(self):
         mm = om.MetaModelUnStructuredComp()
         mm.add_input('x', np.zeros((2,2)))
         mm.add_output('y1', 0.)
         mm.add_output('y2', 0.)
 
         mm.options['default_surrogate'] = om.KrigingSurrogate()
```

### Comparing `openmdao-3.9.1/openmdao/components/tests/test_multifi_meta_model_unstructured_comp.py` & `openmdao-3.9.2/openmdao/components/tests/test_multifi_meta_model_unstructured_comp.py`

 * *Files identical despite different names*

### Comparing `openmdao-3.9.1/openmdao/components/tests/test_mux_comp.py` & `openmdao-3.9.2/openmdao/components/tests/test_mux_comp.py`

 * *Files identical despite different names*

### Comparing `openmdao-3.9.1/openmdao/components/tests/test_spline_comp.py` & `openmdao-3.9.2/openmdao/components/tests/test_spline_comp.py`

 * *Files identical despite different names*

### Comparing `openmdao-3.9.1/openmdao/components/tests/test_vector_magnitude_comp.py` & `openmdao-3.9.2/openmdao/components/tests/test_vector_magnitude_comp.py`

 * *Files identical despite different names*

### Comparing `openmdao-3.9.1/openmdao/components/vector_magnitude_comp.py` & `openmdao-3.9.2/openmdao/components/vector_magnitude_comp.py`

 * *Files identical despite different names*

### Comparing `openmdao-3.9.1/openmdao/core/analysis_error.py` & `openmdao-3.9.2/openmdao/core/analysis_error.py`

 * *Files identical despite different names*

### Comparing `openmdao-3.9.1/openmdao/core/component.py` & `openmdao-3.9.2/openmdao/core/component.py`

 * *Files identical despite different names*

### Comparing `openmdao-3.9.1/openmdao/core/configinfo.py` & `openmdao-3.9.2/openmdao/core/configinfo.py`

 * *Files identical despite different names*

### Comparing `openmdao-3.9.1/openmdao/core/constants.py` & `openmdao-3.9.2/openmdao/core/constants.py`

 * *Files identical despite different names*

### Comparing `openmdao-3.9.1/openmdao/core/driver.py` & `openmdao-3.9.2/openmdao/core/driver.py`

 * *Files 1% similar despite different names*

```diff
@@ -442,15 +442,15 @@
         #    options of those
 
         # includes and excludes for outputs are specified using _promoted_ names
         # vectors are keyed on absolute name, discretes on relative/promoted name
         myinputs = myoutputs = myresiduals = []
 
         if recording_options['record_outputs']:
-            myoutputs = sorted([n for n, prom in abs2prom.items() if check_path(prom, incl, excl)])
+            myoutputs = [n for n, prom in abs2prom.items() if check_path(prom, incl, excl)]
 
             model_outs = model._outputs
 
             if model._var_discrete['output']:
                 # if we have discrete outputs then residual name set doesn't match output one
                 if recording_options['record_residuals']:
                     myresiduals = [n for n in myoutputs if model_outs._contains_abs(n)]
@@ -459,31 +459,31 @@
 
         elif recording_options['record_residuals']:
             myresiduals = [n for n in model._residuals._abs_iter()
                            if check_path(abs2prom[n], incl, excl)]
 
         myoutputs = set(myoutputs)
         if recording_options['record_desvars']:
-            myoutputs.update(self._designvars)
+            myoutputs.update(model.get_source(n) for n in self._designvars)
         if recording_options['record_objectives'] or recording_options['record_responses']:
             myoutputs.update(self._objs)
         if recording_options['record_constraints'] or recording_options['record_responses']:
             myoutputs.update(self._cons)
 
         # inputs (if in options). inputs use _absolute_ names for includes/excludes
         if 'record_inputs' in recording_options:
             if recording_options['record_inputs']:
-                # sort the results since _var_allprocs_abs2prom isn't ordered
-                myinputs = sorted([n for n in model._var_allprocs_abs2prom['input']
-                                  if check_path(n, incl, excl)])
+                myinputs = [n for n in model._var_allprocs_abs2prom['input']
+                            if check_path(n, incl, excl)]
 
+        # sort lists to ensure that vars are iterated over in the same order on all procs
         vars2record = {
-            'input': myinputs,
-            'output': list(myoutputs),
-            'residual': myresiduals
+            'input': sorted(myinputs),
+            'output': sorted(myoutputs),
+            'residual': sorted(myresiduals)
         }
 
         return vars2record
 
     def _setup_recording(self):
         """
         Set up case recording.
```

### Comparing `openmdao-3.9.1/openmdao/core/explicitcomponent.py` & `openmdao-3.9.2/openmdao/core/explicitcomponent.py`

 * *Files identical despite different names*

### Comparing `openmdao-3.9.1/openmdao/core/group.py` & `openmdao-3.9.2/openmdao/core/group.py`

 * *Files identical despite different names*

### Comparing `openmdao-3.9.1/openmdao/core/implicitcomponent.py` & `openmdao-3.9.2/openmdao/core/implicitcomponent.py`

 * *Files identical despite different names*

### Comparing `openmdao-3.9.1/openmdao/core/indepvarcomp.py` & `openmdao-3.9.2/openmdao/core/indepvarcomp.py`

 * *Files identical despite different names*

### Comparing `openmdao-3.9.1/openmdao/core/parallel_group.py` & `openmdao-3.9.2/openmdao/core/parallel_group.py`

 * *Files identical despite different names*

### Comparing `openmdao-3.9.1/openmdao/core/problem.py` & `openmdao-3.9.2/openmdao/core/problem.py`

 * *Files identical despite different names*

```diff
@@ -527,21 +527,22 @@
                         if tlocmeta:  # target is local
                             src_indices = tlocmeta['src_indices']
                             flat = False
                             if name in model._var_prom2inds:
                                 sshape, inds, flat = model._var_prom2inds[name]
                                 if inds is not None:
                                     if _is_slicer_op(inds):
-                                        inds = _slice_indices(inds, np.prod(sshape), sshape).ravel()
-                                        value = value.ravel()
+                                        inds = _slice_indices(inds, np.prod(sshape), sshape)
                                         flat = True
                                 src_indices = inds
                             if src_indices is None:
                                 model._outputs.set_var(src, value, None, flat)
                             else:
+                                if flat:
+                                    src_indices = src_indices.ravel()
                                 if tmeta['distributed']:
                                     ssizes = model._var_sizes['nonlinear']['output']
                                     sidx = model._var_allprocs_abs2idx['nonlinear'][src]
                                     ssize = ssizes[myrank, sidx]
                                     start = np.sum(ssizes[:myrank, sidx])
                                     end = start + ssize
                                     if np.any(src_indices < start) or np.any(src_indices >= end):
@@ -1123,15 +1124,15 @@
 
             jac_key = 'J_' + mode
 
             for comp in comps:
 
                 # Only really need to linearize once.
                 if mode == 'fwd':
-                    comp.run_linearize()
+                    comp.run_linearize(sub_do_ln=False)
 
                 explicit = isinstance(comp, ExplicitComponent)
                 matrix_free = comp.matrix_free
                 c_name = comp.pathname
                 if mode == 'fwd':
                     indep_key[c_name] = set()
```

### Comparing `openmdao-3.9.1/openmdao/core/system.py` & `openmdao-3.9.2/openmdao/core/system.py`

 * *Files 0% similar despite different names*

```diff
@@ -718,25 +718,26 @@
             Absolute or promoted name of the variable.
 
         Returns
         -------
         str
             The absolute name of the source variable.
         """
-        if self._problem_meta is None or 'prom2abs' not in self._problem_meta:
+        try:
+            prom2abs = self._problem_meta['prom2abs']
+        except StandardError:
             raise RuntimeError(f"{self.msginfo}: get_source cannot be called for variable {name} "
-                               "before Problem.setup is complete.")
+                               "before Problem.setup has been called.")
 
-        model = self._problem_meta['model_ref']()
-        prom2abs = self._problem_meta['prom2abs']
-        if name in prom2abs['input']:
-            name = prom2abs['input'][name][0]
-        elif name in prom2abs['output']:
+        if name in prom2abs['output']:
             return prom2abs['output'][name][0]
 
+        if name in prom2abs['input']:
+            name = prom2abs['input'][name][0]
+        model = self._problem_meta['model_ref']()
         if name in model._conn_global_abs_in2out:
             return model._conn_global_abs_in2out[name]
 
         return name
 
     def _setup(self, comm, mode, prob_meta):
         """
@@ -1129,15 +1130,15 @@
                 else:
                     self._apply_nonlinear()
 
                 for scheme in self._approx_schemes.values():
                     scheme._reset()  # force a re-initialization of approx
                     approx_scheme._during_sparsity_comp = True
 
-            self.run_linearize()
+            self.run_linearize(sub_do_ln=False)
 
         sparsity, sp_info = self._jacobian.get_sparsity()
 
         self._jacobian = save_jac
 
         # revert uncolored approx back to normal
         approx_scheme._reset()
@@ -3873,15 +3874,15 @@
         ----------
         sub_do_ln : boolean
             Flag indicating if the children should call linearize on their linear solvers.
         """
         with self._scaled_context_all():
             do_ln = self._linear_solver is not None and self._linear_solver._linearize_children()
             self._linearize(self._assembled_jac, sub_do_ln=do_ln)
-            if self._linear_solver is not None:
+            if self._linear_solver is not None and sub_do_ln:
                 self._linear_solver._linearize()
 
     def _apply_nonlinear(self):
         """
         Compute residuals. The model is assumed to be in a scaled state.
         """
         pass
```

### Comparing `openmdao-3.9.1/openmdao/core/tests/test_add_var.py` & `openmdao-3.9.2/openmdao/core/tests/test_add_var.py`

 * *Files identical despite different names*

### Comparing `openmdao-3.9.1/openmdao/core/tests/test_approx_derivs.py` & `openmdao-3.9.2/openmdao/core/tests/test_approx_derivs.py`

 * *Files identical despite different names*

### Comparing `openmdao-3.9.1/openmdao/core/tests/test_auto_ivc.py` & `openmdao-3.9.2/openmdao/core/tests/test_auto_ivc.py`

 * *Files identical despite different names*

### Comparing `openmdao-3.9.1/openmdao/core/tests/test_aviary_mpi_bug.py` & `openmdao-3.9.2/openmdao/core/tests/test_aviary_mpi_bug.py`

 * *Files identical despite different names*

### Comparing `openmdao-3.9.1/openmdao/core/tests/test_check_derivs.py` & `openmdao-3.9.2/openmdao/core/tests/test_check_derivs.py`

 * *Files 0% similar despite different names*

```diff
@@ -1908,14 +1908,53 @@
 
         prob.setup(force_alloc_complex=True)
         prob.run_model()
         partials = prob.check_partials(method='cs', out_stream=None)
 
         assert_check_partials(partials)
 
+    def test_no_linsolve_during_check(self):
+        # ensure that solve_linear is not called during check partials
+        from openmdao.solvers.solver import LinearSolver
+
+        class ErrSolver(LinearSolver):
+            def _linearize(self):
+                raise RuntimeError("_linearize called")
+
+            def solve(self, vec_names, mode, rel_systems=None):
+                raise RuntimeError("solve called")
+
+            def _run_apply(self):
+                raise RuntimeError("_run_apply called")
+
+        class SingularImplicitComp(om.ImplicitComponent):
+
+            def setup(self):
+                self.add_input('lhs', shape=10)
+                self.add_input('rhs', shape=10)
+
+                self.add_output('resid', shape=10)
+
+                self.declare_partials('*', '*', method='cs')
+
+            def apply_nonlinear(self, inputs, outputs, residuals):
+
+                residuals['resid'] = inputs['lhs'] - inputs['rhs']
+
+
+        p = om.Problem()
+
+        p.model.add_subsystem('sing_check', SingularImplicitComp())
+        p.model.sing_check.linear_solver = ErrSolver()
+        p.setup()
+
+        p.run_model()
+
+        p.check_partials(out_stream=None)
+
 
 class TestCheckPartialsFeature(unittest.TestCase):
 
     def test_feature_incorrect_jacobian(self):
         import numpy as np
 
         import openmdao.api as om
```

### Comparing `openmdao-3.9.1/openmdao/core/tests/test_coloring.py` & `openmdao-3.9.2/openmdao/core/tests/test_coloring.py`

 * *Files identical despite different names*

### Comparing `openmdao-3.9.1/openmdao/core/tests/test_component.py` & `openmdao-3.9.2/openmdao/core/tests/test_component.py`

 * *Files identical despite different names*

### Comparing `openmdao-3.9.1/openmdao/core/tests/test_component_io_independence_from_prob.py` & `openmdao-3.9.2/openmdao/core/tests/test_component_io_independence_from_prob.py`

 * *Files identical despite different names*

### Comparing `openmdao-3.9.1/openmdao/core/tests/test_compute_jacvec_prod.py` & `openmdao-3.9.2/openmdao/core/tests/test_compute_jacvec_prod.py`

 * *Files identical despite different names*

### Comparing `openmdao-3.9.1/openmdao/core/tests/test_connections.py` & `openmdao-3.9.2/openmdao/core/tests/test_connections.py`

 * *Files identical despite different names*

### Comparing `openmdao-3.9.1/openmdao/core/tests/test_connections_in_configure.py` & `openmdao-3.9.2/openmdao/core/tests/test_connections_in_configure.py`

 * *Files identical despite different names*

### Comparing `openmdao-3.9.1/openmdao/core/tests/test_core_simple.py` & `openmdao-3.9.2/openmdao/core/tests/test_core_simple.py`

 * *Files identical despite different names*

### Comparing `openmdao-3.9.1/openmdao/core/tests/test_deriv_transfers.py` & `openmdao-3.9.2/openmdao/core/tests/test_deriv_transfers.py`

 * *Files identical despite different names*

### Comparing `openmdao-3.9.1/openmdao/core/tests/test_des_vars_responses.py` & `openmdao-3.9.2/openmdao/core/tests/test_des_vars_responses.py`

 * *Files identical despite different names*

### Comparing `openmdao-3.9.1/openmdao/core/tests/test_direct_nondistrib_comp.py` & `openmdao-3.9.2/openmdao/core/tests/test_direct_nondistrib_comp.py`

 * *Files identical despite different names*

### Comparing `openmdao-3.9.1/openmdao/core/tests/test_discrete.py` & `openmdao-3.9.2/openmdao/core/tests/test_discrete.py`

 * *Files identical despite different names*

### Comparing `openmdao-3.9.1/openmdao/core/tests/test_discrete_mpi.py` & `openmdao-3.9.2/openmdao/core/tests/test_discrete_mpi.py`

 * *Files identical despite different names*

### Comparing `openmdao-3.9.1/openmdao/core/tests/test_distrib_adder.py` & `openmdao-3.9.2/openmdao/core/tests/test_distrib_adder.py`

 * *Files identical despite different names*

### Comparing `openmdao-3.9.1/openmdao/core/tests/test_distrib_derivs.py` & `openmdao-3.9.2/openmdao/core/tests/test_distrib_derivs.py`

 * *Files identical despite different names*

### Comparing `openmdao-3.9.1/openmdao/core/tests/test_distrib_driver_debug_print_options.py` & `openmdao-3.9.2/openmdao/core/tests/test_distrib_driver_debug_print_options.py`

 * *Files identical despite different names*

### Comparing `openmdao-3.9.1/openmdao/core/tests/test_distrib_list_vars.py` & `openmdao-3.9.2/openmdao/core/tests/test_distrib_list_vars.py`

 * *Files identical despite different names*

### Comparing `openmdao-3.9.1/openmdao/core/tests/test_distribcomp.py` & `openmdao-3.9.2/openmdao/core/tests/test_distribcomp.py`

 * *Files identical despite different names*

### Comparing `openmdao-3.9.1/openmdao/core/tests/test_driver.py` & `openmdao-3.9.2/openmdao/core/tests/test_driver.py`

 * *Files identical despite different names*

### Comparing `openmdao-3.9.1/openmdao/core/tests/test_dyn_sizing.py` & `openmdao-3.9.2/openmdao/core/tests/test_dyn_sizing.py`

 * *Files identical despite different names*

### Comparing `openmdao-3.9.1/openmdao/core/tests/test_expl_comp.py` & `openmdao-3.9.2/openmdao/core/tests/test_expl_comp.py`

 * *Files identical despite different names*

### Comparing `openmdao-3.9.1/openmdao/core/tests/test_fd_color.py` & `openmdao-3.9.2/openmdao/core/tests/test_fd_color.py`

 * *Files 1% similar despite different names*

```diff
@@ -9,15 +9,15 @@
 except ImportError:
     from openmdao.utils.assert_utils import SkipParameterized as parameterized
 
 import numpy as np
 from scipy.sparse import coo_matrix
 
 from openmdao.api import Problem, Group, IndepVarComp, ImplicitComponent, ExecComp, \
-    ExplicitComponent, NonlinearBlockGS, ScipyOptimizeDriver
+    ExplicitComponent, NonlinearBlockGS, ScipyOptimizeDriver, NewtonSolver, DirectSolver
 from openmdao.utils.assert_utils import assert_near_equal, assert_warning
 from openmdao.utils.array_utils import evenly_distrib_idxs, rand_sparsity
 from openmdao.utils.mpi import MPI
 from openmdao.utils.coloring import compute_total_coloring, Coloring
 
 from openmdao.test_suite.components.simple_comps import DoubleArrayComp, NonSquareArrayComp
 
@@ -951,14 +951,58 @@
         derivs = prob.driver._compute_totals()  # colored
 
         self.assertEqual(model._nruns - start_nruns, 2)
         cols = [0,2,3,4]
         rows = [1,3,4]
         _check_total_matrix(model, derivs, sparsity[rows, :][:, cols], method)
 
+    def test_no_solver_linearize(self):
+        # this raised a singularity error before the fix
+        class Get_val_imp(ImplicitComponent):
+            def initialize(self):
+                self.options.declare('size',default=1)
+            def setup(self):
+                size = self.options['size']
+                self.add_output('state',val=5.0*np.ones(size))
+                self.add_input('bar',val=1.4*np.ones(size))
+                self.add_input('foobar')
+
+                self.nonlinear_solver = NewtonSolver()
+                self.linear_solver = DirectSolver()
+
+                self.nonlinear_solver.options['iprint'] = 2
+                self.nonlinear_solver.options['maxiter']=1
+                self.nonlinear_solver.options['solve_subsystems']=False
+
+                self.declare_partials(of="*", wrt="*", method="fd")
+
+                self.declare_coloring(method="fd", num_full_jacs=2)
+
+            def apply_nonlinear(self,inputs,outputs,residuals):
+                foo = outputs['state']
+                bar = inputs['bar']
+
+                area_ratio = 1 / foo * np.sqrt(1/(bar+1)* (1/foo**2))
+
+                residuals['state']=inputs['foobar']-area_ratio
+
+        size = 3
+
+        ivc = IndepVarComp()
+        ivc.add_output('bar',val=1.4*np.ones(size))
+        ivc.add_output('foobar',val=40)
+
+
+        p = Problem()
+        p.model.add_subsystem('ivc',ivc,promotes=['*'])
+        p.model.add_subsystem('comp_check', Get_val_imp(size=size))
+        p.model.connect('bar','comp_check.bar')
+        p.setup()
+        p.run_model()
+
 
 class TestStaticColoring(unittest.TestCase):
 
     def setUp(self):
         np.random.seed(11)
         self.startdir = os.getcwd()
         self.tempdir = tempfile.mkdtemp(prefix=self.__class__.__name__ + '_')
```

### Comparing `openmdao-3.9.1/openmdao/core/tests/test_fd_color_chk_partials.py` & `openmdao-3.9.2/openmdao/core/tests/test_fd_color_chk_partials.py`

 * *Files identical despite different names*

### Comparing `openmdao-3.9.1/openmdao/core/tests/test_feature_cache_linear_solution.py` & `openmdao-3.9.2/openmdao/core/tests/test_feature_cache_linear_solution.py`

 * *Files identical despite different names*

### Comparing `openmdao-3.9.1/openmdao/core/tests/test_getset_vars.py` & `openmdao-3.9.2/openmdao/core/tests/test_getset_vars.py`

 * *Files identical despite different names*

### Comparing `openmdao-3.9.1/openmdao/core/tests/test_group.py` & `openmdao-3.9.2/openmdao/core/tests/test_group.py`

 * *Files identical despite different names*

### Comparing `openmdao-3.9.1/openmdao/core/tests/test_impl_comp.py` & `openmdao-3.9.2/openmdao/core/tests/test_impl_comp.py`

 * *Files identical despite different names*

### Comparing `openmdao-3.9.1/openmdao/core/tests/test_indep_var_comp.py` & `openmdao-3.9.2/openmdao/core/tests/test_indep_var_comp.py`

 * *Files identical despite different names*

### Comparing `openmdao-3.9.1/openmdao/core/tests/test_leaks.py` & `openmdao-3.9.2/openmdao/core/tests/test_leaks.py`

 * *Files identical despite different names*

### Comparing `openmdao-3.9.1/openmdao/core/tests/test_masking.py` & `openmdao-3.9.2/openmdao/core/tests/test_masking.py`

 * *Files identical despite different names*

### Comparing `openmdao-3.9.1/openmdao/core/tests/test_matmat.py` & `openmdao-3.9.2/openmdao/core/tests/test_matmat.py`

 * *Files identical despite different names*

### Comparing `openmdao-3.9.1/openmdao/core/tests/test_mpi_coloring_bug.py` & `openmdao-3.9.2/openmdao/core/tests/test_mpi_coloring_bug.py`

 * *Files identical despite different names*

### Comparing `openmdao-3.9.1/openmdao/core/tests/test_mwe_matmat.py` & `openmdao-3.9.2/openmdao/core/tests/test_mwe_matmat.py`

 * *Files identical despite different names*

### Comparing `openmdao-3.9.1/openmdao/core/tests/test_parallel_derivatives.py` & `openmdao-3.9.2/openmdao/core/tests/test_parallel_derivatives.py`

 * *Files identical despite different names*

### Comparing `openmdao-3.9.1/openmdao/core/tests/test_parallel_fd.py` & `openmdao-3.9.2/openmdao/core/tests/test_parallel_fd.py`

 * *Files identical despite different names*

### Comparing `openmdao-3.9.1/openmdao/core/tests/test_parallel_groups.py` & `openmdao-3.9.2/openmdao/core/tests/test_parallel_groups.py`

 * *Files identical despite different names*

### Comparing `openmdao-3.9.1/openmdao/core/tests/test_parallel_src_indices.py` & `openmdao-3.9.2/openmdao/core/tests/test_parallel_src_indices.py`

 * *Files identical despite different names*

### Comparing `openmdao-3.9.1/openmdao/core/tests/test_prob_remote.py` & `openmdao-3.9.2/openmdao/core/tests/test_prob_remote.py`

 * *Files identical despite different names*

### Comparing `openmdao-3.9.1/openmdao/core/tests/test_problem.py` & `openmdao-3.9.2/openmdao/core/tests/test_problem.py`

 * *Files 1% similar despite different names*

```diff
@@ -2141,14 +2141,29 @@
         model = prob.model
         model.add_subsystem('comp', Paraboloid(), promotes=['x', 'y', 'f_xy'])
 
         with self.assertRaises(RuntimeError) as cm:
             prob.set_val('x', 0.)
         self.assertEqual(str(cm.exception), "Problem: 'x' Cannot call set_val before setup.")
 
+    def test_nonflat_flat_inds(self):
+        # this tests when we have src_indices that refer to a flat source and are defined
+        # as 'flat_src_indices' but are not themselves in a flat array (in this case they're
+        # in a column array).
+        p = om.Problem()
+        p.model.add_subsystem('ivc', om.IndepVarComp('x', val=np.ones((3,3))))
+        p.model.add_subsystem('comp', om.ExecComp('y=x*2', shape=(3, 1)))
+        p.model.connect('ivc.x', 'comp.x', src_indices=np.arange(3, dtype=int).reshape((3,1)),
+                        flat_src_indices=True)
+        p.setup()
+        p.run_model()
+
+        # this test passes if it doesn't raise an exception here...
+        p['comp.x'] = np.arange(3) + 1.
+
 
 class NestedProblemTestCase(unittest.TestCase):
 
     def test_nested_prob(self):
 
         class _ProblemSolver(om.NonlinearRunOnce):
             def solve(self):
```

### Comparing `openmdao-3.9.1/openmdao/core/tests/test_proc_alloc.py` & `openmdao-3.9.2/openmdao/core/tests/test_proc_alloc.py`

 * *Files identical despite different names*

### Comparing `openmdao-3.9.1/openmdao/core/tests/test_remote_vois.py` & `openmdao-3.9.2/openmdao/core/tests/test_remote_vois.py`

 * *Files identical despite different names*

### Comparing `openmdao-3.9.1/openmdao/core/tests/test_root_comp_list_outputs.py` & `openmdao-3.9.2/openmdao/core/tests/test_root_comp_list_outputs.py`

 * *Files identical despite different names*

### Comparing `openmdao-3.9.1/openmdao/core/tests/test_run_root_only.py` & `openmdao-3.9.2/openmdao/core/tests/test_run_root_only.py`

 * *Files identical despite different names*

### Comparing `openmdao-3.9.1/openmdao/core/tests/test_scaling.py` & `openmdao-3.9.2/openmdao/core/tests/test_scaling.py`

 * *Files identical despite different names*

### Comparing `openmdao-3.9.1/openmdao/core/tests/test_serialize.py` & `openmdao-3.9.2/openmdao/core/tests/test_serialize.py`

 * *Files identical despite different names*

### Comparing `openmdao-3.9.1/openmdao/core/tests/test_setup_memleak.py` & `openmdao-3.9.2/openmdao/core/tests/test_setup_memleak.py`

 * *Files identical despite different names*

### Comparing `openmdao-3.9.1/openmdao/core/tests/test_simple_impl_comp.py` & `openmdao-3.9.2/openmdao/core/tests/test_simple_impl_comp.py`

 * *Files identical despite different names*

### Comparing `openmdao-3.9.1/openmdao/core/tests/test_src_indices.py` & `openmdao-3.9.2/openmdao/core/tests/test_src_indices.py`

 * *Files identical despite different names*

### Comparing `openmdao-3.9.1/openmdao/core/tests/test_system.py` & `openmdao-3.9.2/openmdao/core/tests/test_system.py`

 * *Files identical despite different names*

### Comparing `openmdao-3.9.1/openmdao/core/tests/test_units.py` & `openmdao-3.9.2/openmdao/core/tests/test_units.py`

 * *Files identical despite different names*

### Comparing `openmdao-3.9.1/openmdao/core/total_jac.py` & `openmdao-3.9.2/openmdao/core/total_jac.py`

 * *Files 2% similar despite different names*

```diff
@@ -1674,14 +1674,49 @@
 
         if debug_print:
             # Debug outputs scaled derivatives.
             self._print_derivatives()
 
         return totals
 
+    def _get_zero_inds(self, name, tup, jac_arr):
+        """
+        Get zero indices relative to the named variable for jac row/col 'jac_arr'.
+
+        Parameters
+        ----------
+        name : str
+            Name of the design var or response.
+        tup : tuple
+            Contains jacobian slice and dv/response indices, if any.
+        jac_arr : ndarray
+            Row or column of jacobian being checked for zero entries.
+
+        Returns
+        -------
+        ndarray
+            Index array of zero entries.
+        """
+        inds = tup[1]  # these must be indices into the flattened var
+        shname = 'shape' if self.get_remote else 'global_shape'
+        shape = self.model._var_allprocs_abs2meta['output'][name][shname]
+        vslice = jac_arr[tup[0]]
+
+        if inds is None:
+            zero_idxs = np.nonzero(vslice.reshape(shape))
+        else:
+            zero_idxs = np.nonzero(vslice)
+            if zero_idxs[0].size == 0:
+                return zero_idxs
+            varr = np.zeros(shape, dtype=bool)
+            varr.flat[inds[zero_idxs]] = True
+            zero_idxs = np.nonzero(varr)
+
+        return zero_idxs
+
     def check_total_jac(self, raise_error=True, tol=1e-16):
         """
         Check recently computed totals derivative jacobian for problems.
 
         Some optimizers can't handle a jacobian when a design variable has no effect on the
         constraints, or a constraint is unaffected by a design variable. This method
         checks for these cases.
@@ -1689,57 +1724,65 @@
         Parameters
         ----------
         tol : double
             Tolerance for the check.
         raise_error : bool
             If True, raise an exception if a zero row or column is found.
         """
-        J = np.abs(self.J)
-        nrows, ncols = J.shape
-        zero_rows = []
-        zero_cols = []
+        nzrows, nzcols = np.nonzero(np.abs(self.J) > tol)
 
         # Check for zero rows, which correspond to constraints unaffected by any design vars.
-        for j in np.arange(nrows):
-            if np.all(J[j, :] < tol):
-                for name, val in self.of_meta.items():
-                    if j > val[0].stop - 1:
-                        continue
-                    break
-                if name in self.ivc_print_names:
-                    name = self.ivc_print_names[name]
-                if name not in zero_rows:
-                    zero_rows.append(name)
-
-        if zero_rows:
-            msg = f"Constraints or objectives {zero_rows} cannot be impacted by the design " + \
-                "variables of the problem."
-            if raise_error:
-                raise RuntimeError(msg)
-            else:
-                issue_warning(msg, category=DerivativesWarning)
+        col = np.ones(self.J.shape[0], dtype=bool)
+        col[nzrows] = False  # False in this case means nonzero
+        if np.any(col):  # there's at least 1 row that's zero across all columns
+            zero_rows = []
+            for name, tup in self.of_meta.items():
+                zero_idxs = self._get_zero_inds(name, tup, col)
+
+                if zero_idxs[0].size > 0:
+                    if len(zero_idxs) == 1:
+                        zero_rows.append((self.ivc_print_names.get(name, name),
+                                          list(zero_idxs[0])))
+                    else:
+                        zero_rows.append((self.ivc_print_names.get(name, name),
+                                          list(zip(*zero_idxs))))
+
+            if zero_rows:
+                zero_rows = [f"('{n}', inds={idxs})" for n, idxs in zero_rows]
+                msg = (f"Constraints or objectives [{', '.join(zero_rows)}] cannot be impacted by "
+                       "the design variables of the problem.")
+                if raise_error:
+                    raise RuntimeError(msg)
+                else:
+                    issue_warning(msg, category=DerivativesWarning)
 
         # Check for zero cols, which correspond to design vars that don't affect anything.
-        for j in np.arange(ncols):
-            if np.all(J[:, j] < tol):
-                for name, val in self.wrt_meta.items():
-                    if j > val[0].stop - 1:
-                        continue
-                    break
-                if name in self.ivc_print_names:
-                    name = self.ivc_print_names[name]
-                if name not in zero_cols:
-                    zero_cols.append(name)
-
-        if zero_cols:
-            msg = f"Design variables {zero_cols} have no impact on the constraints or objective."
-            if raise_error:
-                raise RuntimeError(msg)
-            else:
-                issue_warning(msg, category=DerivativesWarning)
+        row = np.ones(self.J.shape[1], dtype=bool)
+        row[nzcols] = False  # False in this case means nonzero
+        if np.any(row):  # there's at least 1 col that's zero across all rows
+            zero_cols = []
+            for name, tup in self.wrt_meta.items():
+                zero_idxs = self._get_zero_inds(name, tup, row)
+
+                if zero_idxs[0].size > 0:
+                    if len(zero_idxs) == 1:
+                        zero_cols.append((self.ivc_print_names.get(name, name),
+                                          list(zero_idxs[0])))
+                    else:
+                        zero_cols.append((self.ivc_print_names.get(name, name),
+                                          list(zip(*zero_idxs))))
+
+            if zero_cols:
+                zero_cols = [f"('{n}', inds={idxs})" for n, idxs in zero_cols]
+                msg = (f"Design variables [{', '.join(zero_cols)}] have no impact on the "
+                       "constraints or objective.")
+                if raise_error:
+                    raise RuntimeError(msg)
+                else:
+                    issue_warning(msg, category=DerivativesWarning)
 
     def _restore_linear_solution(self, vec_names, key, mode):
         """
         Restore the previous linear solution.
 
         Parameters
         ----------
```

### Comparing `openmdao-3.9.1/openmdao/devtools/debug.py` & `openmdao-3.9.2/openmdao/devtools/debug.py`

 * *Files identical despite different names*

### Comparing `openmdao-3.9.1/openmdao/devtools/dump_sqlite_recorder_file.py` & `openmdao-3.9.2/openmdao/devtools/dump_sqlite_recorder_file.py`

 * *Files identical despite different names*

### Comparing `openmdao-3.9.1/openmdao/devtools/iprof_mem.py` & `openmdao-3.9.2/openmdao/devtools/iprof_mem.py`

 * *Files identical despite different names*

### Comparing `openmdao-3.9.1/openmdao/devtools/iprof_utils.py` & `openmdao-3.9.2/openmdao/devtools/iprof_utils.py`

 * *Files identical despite different names*

### Comparing `openmdao-3.9.1/openmdao/devtools/iprofile.py` & `openmdao-3.9.2/openmdao/devtools/iprofile.py`

 * *Files identical despite different names*

### Comparing `openmdao-3.9.1/openmdao/devtools/iprofile_app/iprofile_app.py` & `openmdao-3.9.2/openmdao/devtools/iprofile_app/iprofile_app.py`

 * *Files 1% similar despite different names*

```diff
@@ -221,9 +221,9 @@
             app.listen(options.port)
 
             print("starting server on port %d" % options.port)
 
             serve_thread = _startThread(tornado.ioloop.IOLoop.current().start)
             launch_thread = _startThread(lambda: _launch_browser(options.port))
 
-            while serve_thread.isAlive():
+            while serve_thread.is_alive():
                 serve_thread.join(timeout=1)
```

### Comparing `openmdao-3.9.1/openmdao/devtools/iprofile_app/templates/iprofview.html` & `openmdao-3.9.2/openmdao/devtools/iprofile_app/templates/iprofview.html`

 * *Files identical despite different names*

### Comparing `openmdao-3.9.1/openmdao/devtools/itrace.py` & `openmdao-3.9.2/openmdao/devtools/itrace.py`

 * *Files identical despite different names*

### Comparing `openmdao-3.9.1/openmdao/devtools/memory.py` & `openmdao-3.9.2/openmdao/devtools/memory.py`

 * *Files identical despite different names*

### Comparing `openmdao-3.9.1/openmdao/devtools/run_test.py` & `openmdao-3.9.2/openmdao/devtools/run_test.py`

 * *Files identical despite different names*

### Comparing `openmdao-3.9.1/openmdao/devtools/tests/mem_model.py` & `openmdao-3.9.2/openmdao/devtools/tests/mem_model.py`

 * *Files identical despite different names*

### Comparing `openmdao-3.9.1/openmdao/devtools/tests/test_debug.py` & `openmdao-3.9.2/openmdao/devtools/tests/test_debug.py`

 * *Files identical despite different names*

### Comparing `openmdao-3.9.1/openmdao/devtools/tests/test_iprof_mem.py` & `openmdao-3.9.2/openmdao/devtools/tests/test_iprof_mem.py`

 * *Files identical despite different names*

### Comparing `openmdao-3.9.1/openmdao/devtools/wing_proj_template.wpr` & `openmdao-3.9.2/openmdao/devtools/wing_proj_template.wpr`

 * *Files identical despite different names*

### Comparing `openmdao-3.9.1/openmdao/devtools/wingproj.py` & `openmdao-3.9.2/openmdao/devtools/wingproj.py`

 * *Files identical despite different names*

### Comparing `openmdao-3.9.1/openmdao/docs/_exts/embed_bibtex.py` & `openmdao-3.9.2/openmdao/docs/_exts/embed_bibtex.py`

 * *Files identical despite different names*

### Comparing `openmdao-3.9.1/openmdao/docs/_exts/embed_code.py` & `openmdao-3.9.2/openmdao/docs/_exts/embed_code.py`

 * *Files identical despite different names*

### Comparing `openmdao-3.9.1/openmdao/docs/_exts/embed_compare.py` & `openmdao-3.9.2/openmdao/docs/_exts/embed_compare.py`

 * *Files identical despite different names*

### Comparing `openmdao-3.9.1/openmdao/docs/_exts/embed_n2.py` & `openmdao-3.9.2/openmdao/docs/_exts/embed_n2.py`

 * *Files identical despite different names*

### Comparing `openmdao-3.9.1/openmdao/docs/_exts/embed_options.py` & `openmdao-3.9.2/openmdao/docs/_exts/embed_options.py`

 * *Files identical despite different names*

### Comparing `openmdao-3.9.1/openmdao/docs/_exts/embed_shell_cmd.py` & `openmdao-3.9.2/openmdao/docs/_exts/embed_shell_cmd.py`

 * *Files identical despite different names*

### Comparing `openmdao-3.9.1/openmdao/docs/_exts/link_class_from_docstring.py` & `openmdao-3.9.2/openmdao/docs/_exts/link_class_from_docstring.py`

 * *Files identical despite different names*

### Comparing `openmdao-3.9.1/openmdao/docs/_exts/tags.py` & `openmdao-3.9.2/openmdao/docs/_exts/tags.py`

 * *Files identical despite different names*

### Comparing `openmdao-3.9.1/openmdao/docs/_utils/docutil.py` & `openmdao-3.9.2/openmdao/docs/_utils/docutil.py`

 * *Files identical despite different names*

### Comparing `openmdao-3.9.1/openmdao/docs/_utils/generate_sourcedocs.py` & `openmdao-3.9.2/openmdao/docs/_utils/generate_sourcedocs.py`

 * *Files identical despite different names*

### Comparing `openmdao-3.9.1/openmdao/docs/_utils/patch.py` & `openmdao-3.9.2/openmdao/docs/_utils/patch.py`

 * *Files identical despite different names*

### Comparing `openmdao-3.9.1/openmdao/docs/_utils/preprocess_tags.py` & `openmdao-3.9.2/openmdao/docs/_utils/preprocess_tags.py`

 * *Files identical despite different names*

### Comparing `openmdao-3.9.1/openmdao/docs/_utils/run_sub.py` & `openmdao-3.9.2/openmdao/docs/_utils/run_sub.py`

 * *Files identical despite different names*

### Comparing `openmdao-3.9.1/openmdao/docs/_utils/upload_doc_version.py` & `openmdao-3.9.2/openmdao/docs/_utils/upload_doc_version.py`

 * *Files identical despite different names*

### Comparing `openmdao-3.9.1/openmdao/docs/conf.py` & `openmdao-3.9.2/openmdao/docs/conf.py`

 * *Files identical despite different names*

### Comparing `openmdao-3.9.1/openmdao/drivers/differential_evolution_driver.py` & `openmdao-3.9.2/openmdao/drivers/differential_evolution_driver.py`

 * *Files identical despite different names*

### Comparing `openmdao-3.9.1/openmdao/drivers/doe_driver.py` & `openmdao-3.9.2/openmdao/drivers/doe_driver.py`

 * *Files identical despite different names*

### Comparing `openmdao-3.9.1/openmdao/drivers/doe_generators.py` & `openmdao-3.9.2/openmdao/drivers/doe_generators.py`

 * *Files identical despite different names*

### Comparing `openmdao-3.9.1/openmdao/drivers/genetic_algorithm_driver.py` & `openmdao-3.9.2/openmdao/drivers/genetic_algorithm_driver.py`

 * *Files identical despite different names*

### Comparing `openmdao-3.9.1/openmdao/drivers/pyoptsparse_driver.py` & `openmdao-3.9.2/openmdao/drivers/pyoptsparse_driver.py`

 * *Files 2% similar despite different names*

```diff
@@ -5,22 +5,25 @@
 formulating and solving nonlinear constrained optimization problems, with
 additional MPI capability.
 """
 
 from collections import OrderedDict
 import json
 import signal
+from distutils.version import LooseVersion
 
 import numpy as np
 from scipy.sparse import coo_matrix
 
 try:
-    from pyoptsparse import Optimization
+    import pyoptsparse
+    Optimization = pyoptsparse.Optimization
 except ImportError:
     Optimization = None
+    pyoptsparse = None
 
 from openmdao.core.constants import INT_DTYPE
 from openmdao.core.analysis_error import AnalysisError
 from openmdao.core.driver import Driver, RecordingDebugging
 import openmdao.utils.coloring as c_mod
 from openmdao.utils.class_util import weak_method_wrapper
 from openmdao.utils.mpi import FakeComm
@@ -326,15 +329,19 @@
 
         for name, meta in input_meta.items():
             size = meta['global_size'] if meta['distributed'] else meta['size']
             opt_prob.addVarGroup(name, size, type='c',
                                  value=input_vals[name],
                                  lower=meta['lower'], upper=meta['upper'])
 
-        opt_prob.finalizeDesignVariables()
+        if not hasattr(pyoptsparse, '__version__') or \
+           LooseVersion(pyoptsparse.__version__) < LooseVersion('2.5.1'):
+            opt_prob.finalizeDesignVariables()
+        else:
+            opt_prob.finalize()
 
         # Add all objectives
         objs = self.get_objective_values()
         for name in objs:
             opt_prob.addObj(name)
             self._quantities.append(name)
```

### Comparing `openmdao-3.9.1/openmdao/drivers/scipy_optimizer.py` & `openmdao-3.9.2/openmdao/drivers/scipy_optimizer.py`

 * *Files identical despite different names*

### Comparing `openmdao-3.9.1/openmdao/drivers/tests/test_differential_evolution_driver.py` & `openmdao-3.9.2/openmdao/drivers/tests/test_differential_evolution_driver.py`

 * *Files identical despite different names*

### Comparing `openmdao-3.9.1/openmdao/drivers/tests/test_doe_driver.py` & `openmdao-3.9.2/openmdao/drivers/tests/test_doe_driver.py`

 * *Files identical despite different names*

### Comparing `openmdao-3.9.1/openmdao/drivers/tests/test_genetic_algorithm_driver.py` & `openmdao-3.9.2/openmdao/drivers/tests/test_genetic_algorithm_driver.py`

 * *Files identical despite different names*

### Comparing `openmdao-3.9.1/openmdao/drivers/tests/test_pyoptsparse_driver.py` & `openmdao-3.9.2/openmdao/drivers/tests/test_pyoptsparse_driver.py`

 * *Files 0% similar despite different names*

```diff
@@ -11,15 +11,15 @@
 import openmdao.api as om
 from openmdao.test_suite.components.expl_comp_array import TestExplCompArrayDense
 from openmdao.test_suite.components.paraboloid import Paraboloid
 from openmdao.test_suite.components.paraboloid_distributed import DistParab
 from openmdao.test_suite.components.sellar import SellarDerivativesGrouped
 from openmdao.utils.assert_utils import assert_near_equal, assert_warning
 from openmdao.utils.general_utils import set_pyoptsparse_opt, run_driver
-from openmdao.utils.testing_utils import use_tempdirs
+from openmdao.utils.testing_utils import use_tempdirs, require_pyoptsparse
 from openmdao.utils.mpi import MPI
 from openmdao.warnings import OMDeprecationWarning
 
 # check that pyoptsparse is installed
 # if it is, try to use SNOPT but fall back to SLSQP
 OPT, OPTIMIZER = set_pyoptsparse_opt('SNOPT')
 
@@ -157,19 +157,19 @@
         with self.assertRaises(RuntimeError) as ctx:
             pyOptSparseDriver()
 
         self.assertEqual(str(ctx.exception),
                          'pyOptSparseDriver is not available, pyOptsparse is not installed.')
 
 
-@unittest.skipIf(OPT is None or OPTIMIZER is None, "only run if pyoptsparse is installed.")
 @unittest.skipUnless(MPI, "MPI is required.")
 class TestMPIScatter(unittest.TestCase):
     N_PROCS = 2
 
+    @require_pyoptsparse(OPTIMIZER)
     def test_design_vars_on_all_procs_pyopt(self):
 
         prob = om.Problem()
         model = prob.model
 
         model.add_subsystem('comp', Paraboloid(), promotes=['*'])
         model.add_subsystem('con', DummyComp(), promotes=['*'])
@@ -187,14 +187,15 @@
 
         prob.setup()
         prob.run_driver()
 
         proc_vals = MPI.COMM_WORLD.allgather([prob['x'], prob['y'], prob['c'], prob['f_xy']])
         np.testing.assert_array_almost_equal(proc_vals[0], proc_vals[1])
 
+    @require_pyoptsparse(OPTIMIZER)
     def test_opt_distcomp(self):
         size = 7
 
         prob = om.Problem()
         model = prob.model
 
         ivc = om.IndepVarComp()
@@ -226,18 +227,16 @@
         obj = prob.driver.get_objective_values()
 
         assert_near_equal(obj['sum.f_sum'], 0.0, 2e-6)
         assert_near_equal(con['parab.f_xy'],
                           np.zeros(7),
                           1e-5)
 
+    @require_pyoptsparse('ParOpt')
     def test_paropt_distcomp(self):
-        _, local_opt = set_pyoptsparse_opt('ParOpt')
-        if local_opt != 'ParOpt':
-            raise unittest.SkipTest("pyoptsparse is not providing ParOpt")
         size = 7
 
         prob = om.Problem()
         model = prob.model
 
         ivc = om.IndepVarComp()
         ivc.add_output('x', np.ones((size, )))
@@ -268,15 +267,15 @@
 
         assert_near_equal(obj['sum.f_sum'], 0.0, 4e-6)
         assert_near_equal(con['parab.f_xy'],
                           np.zeros(7),
                           1e-5)
 
 
-@unittest.skipIf(OPT is None or OPTIMIZER is None, "only run if pyoptsparse is installed.")
+@require_pyoptsparse(OPTIMIZER)
 @use_tempdirs
 class TestPyoptSparse(unittest.TestCase):
 
     def test_simple_paraboloid_upper(self):
 
         prob = om.Problem()
         model = prob.model
@@ -2022,18 +2021,16 @@
         prob.set_solver_print(level=0)
 
         prob.setup(check=False, mode='rev')
         prob.run_driver()
 
         assert_near_equal(prob['z'][0], 1.9776, 1e-3)
 
+    @require_pyoptsparse('ParOpt')
     def test_ParOpt_basic(self):
-        _, local_opt = set_pyoptsparse_opt('ParOpt')
-        if local_opt != 'ParOpt':
-            raise unittest.SkipTest("pyoptsparse is not providing ParOpt")
 
         prob = om.Problem()
         model = prob.model = SellarDerivativesGrouped()
 
         prob.driver = om.pyOptSparseDriver()
         prob.driver.options['optimizer'] = "ParOpt"
 
@@ -2139,15 +2136,15 @@
 
         prob.setup()
 
         with self.assertRaises(RuntimeError) as msg:
             prob.run_driver()
 
         self.assertEqual(str(msg.exception),
-                         "Constraints or objectives ['parab.z'] cannot be impacted by the design " + \
+                         "Constraints or objectives [('parab.z', inds=[0])] cannot be impacted by the design " + \
                          "variables of the problem.")
 
     def test_singular_jac_error_desvars(self):
         prob = om.Problem()
         prob.model.add_subsystem('parab',
                                      om.ExecComp(['f_xy = (x-3.0)**2 + x*y + (y+4.0)**2 - 3.0 - 0*z',
                                                   ]), #'foo = 0.0 * z'],),
@@ -2174,15 +2171,15 @@
 
         prob.setup()
 
         with self.assertRaises(RuntimeError) as msg:
             prob.run_driver()
 
         self.assertEqual(str(msg.exception),
-                         "Design variables ['z'] have no impact on the constraints or objective.")
+                         "Design variables [('z', inds=[0])] have no impact on the constraints or objective.")
 
     def test_singular_jac_ignore(self):
         prob = om.Problem()
         prob.model.add_subsystem('parab',
                                  om.ExecComp(['f_xy = (x-3.0)**2 + x*y + (y+4.0)**2 - 3.0',
                                               'z = 12.0'],),
                                  promotes_inputs=['x', 'y'])
@@ -2233,15 +2230,15 @@
         prob.model.add_constraint('const.g', lower=0, upper=10.)
 
         # This constraint produces a zero row.
         prob.model.add_constraint('parab.z', equals=12.)
 
         prob.setup()
 
-        msg = "Constraints or objectives ['parab.z'] cannot be impacted by the design variables of the problem."
+        msg = "Constraints or objectives [('parab.z', inds=[0])] cannot be impacted by the design variables of the problem."
 
         with assert_warning(UserWarning, msg):
             prob.run_driver()
 
     def test_singular_jac_tol(self):
         prob = om.Problem()
         prob.model.add_subsystem('parab',
```

### Comparing `openmdao-3.9.1/openmdao/drivers/tests/test_scipy_optimizer.py` & `openmdao-3.9.2/openmdao/drivers/tests/test_scipy_optimizer.py`

 * *Files 1% similar despite different names*

```diff
@@ -1833,51 +1833,53 @@
         prob.setup()
         prob.run_driver()
         assert_near_equal(prob['x'], np.ones(rosenbrock_size), 1e-2)
         assert_near_equal(prob['f'], 0.0, 1e-2)
 
     def test_singular_jac_error_responses(self):
         prob = om.Problem()
+        size = 3
         prob.model.add_subsystem('parab',
                                  om.ExecComp(['f_xy = (x-3.0)**2 + x*y + (y+4.0)**2 - 3.0',
-                                              'z = 12.0'],),
+                                              'z = 12.0'], shape=(size,)),
                                  promotes_inputs=['x', 'y'])
 
-        prob.model.add_subsystem('const', om.ExecComp('g = x + y'), promotes_inputs=['x', 'y'])
+        prob.model.add_subsystem('const', om.ExecComp('g = x + y', shape=(size,)),
+                                 promotes_inputs=['x', 'y'])
 
-        prob.model.set_input_defaults('x', 3.0)
-        prob.model.set_input_defaults('y', -4.0)
+        prob.model.set_input_defaults('x', 3.0 * np.ones(size))
+        prob.model.set_input_defaults('y', -4.0 * np.ones(size))
 
         prob.driver = om.ScipyOptimizeDriver()
         prob.driver.options['optimizer'] = 'SLSQP'
         prob.driver.options['singular_jac_behavior'] = 'error'
 
         prob.model.add_design_var('x', lower=-50, upper=50)
         prob.model.add_design_var('y', lower=-50, upper=50)
-        prob.model.add_objective('parab.f_xy')
+        prob.model.add_objective('parab.f_xy', index=1)
 
         prob.model.add_constraint('const.g', lower=0, upper=10.)
 
         # This constraint produces a zero row.
         prob.model.add_constraint('parab.z', equals=12.)
 
         prob.setup()
 
         with self.assertRaises(RuntimeError) as msg:
             prob.run_driver()
 
         self.assertEqual(str(msg.exception),
-                         "Constraints or objectives ['parab.z'] cannot be impacted by the design " + \
+                         "Constraints or objectives [('parab.z', inds=[0, 1, 2])] cannot be impacted by the design " + \
                          "variables of the problem.")
 
     def test_singular_jac_error_desvars(self):
         prob = om.Problem()
         prob.model.add_subsystem('parab',
                                      om.ExecComp(['f_xy = (x-3.0)**2 + x*y + (y+4.0)**2 - 3.0 - 0*z',
-                                                  ]), #'foo = 0.0 * z'],),
+                                                  ]),
                                      promotes_inputs=['x', 'y', 'z'])
 
         prob.model.add_subsystem('const', om.ExecComp('g = x + y'), promotes_inputs=['x', 'y'])
 
         prob.model.set_input_defaults('x', 3.0)
         prob.model.set_input_defaults('y', -4.0)
 
@@ -1897,15 +1899,15 @@
 
         prob.setup()
 
         with self.assertRaises(RuntimeError) as msg:
             prob.run_driver()
 
         self.assertEqual(str(msg.exception),
-                         "Design variables ['z'] have no impact on the constraints or objective.")
+                         "Design variables [('z', inds=[0])] have no impact on the constraints or objective.")
 
     def test_singular_jac_ignore(self):
         prob = om.Problem()
         prob.model.add_subsystem('parab',
                                  om.ExecComp(['f_xy = (x-3.0)**2 + x*y + (y+4.0)**2 - 3.0',
                                               'z = 12.0'],),
                                  promotes_inputs=['x', 'y'])
@@ -1956,19 +1958,85 @@
         prob.model.add_constraint('const.g', lower=0, upper=10.)
 
         # This constraint produces a zero row.
         prob.model.add_constraint('parab.z', equals=12.)
 
         prob.setup()
 
-        msg = "Constraints or objectives ['parab.z'] cannot be impacted by the design variables of the problem."
+        msg = "Constraints or objectives [('parab.z', inds=[0])] cannot be impacted by the design variables of the problem."
 
         with assert_warning(UserWarning, msg):
             prob.run_driver()
 
+    def test_singular_jac_error_desvars_multidim_indices_dv(self):
+        prob = om.Problem()
+        prob.model.add_subsystem('parab',
+                                 om.ExecComp(['f_xy = (x-3.0)**2 + x*y + (y+4.0)**2 - 3.0 - 0*z'], shape=(3,2,2)),
+                                 promotes_inputs=['x', 'y', 'z'])
+
+        prob.model.add_subsystem('const', om.ExecComp('g = x + y', shape=(3,2,2)), promotes_inputs=['x', 'y'])
+
+        prob.model.set_input_defaults('x', np.ones((3,2,2)) * 3.0)
+        prob.model.set_input_defaults('y', np.ones((3,2,2)) * -4.0)
+
+        prob.driver = om.ScipyOptimizeDriver()
+        prob.driver.options['optimizer'] = 'SLSQP'
+        prob.driver.options['singular_jac_behavior'] = 'error'
+
+        prob.model.add_design_var('x', lower=-50, upper=50)
+        prob.model.add_design_var('y', lower=-50, upper=50)
+
+        # Design var z does not affect any quantities.
+        prob.model.add_design_var('z', lower=-50, upper=50, indices=[2,5,6])
+
+        prob.model.add_objective('parab.f_xy', index=6)
+
+        prob.model.add_constraint('const.g', lower=0, upper=10.)
+
+        prob.setup()
+
+        with self.assertRaises(RuntimeError) as msg:
+            prob.run_driver()
+
+        self.assertEqual(str(msg.exception),
+                         "Design variables [('z', inds=[(0, 1, 0), (1, 0, 1), (1, 1, 0)])] have no impact on the constraints or objective.")
+
+    def test_singular_jac_error_desvars_multidim_indices_con(self):
+        prob = om.Problem()
+        prob.model.add_subsystem('parab',
+                                 om.ExecComp(['f_xy = (x-3.0)**2 + x*y + (y+4.0)**2 - 3.0 - z',
+                                              'f_z = z * 0.0'], shape=(3,2,2)),
+                                 promotes_inputs=['x', 'y', 'z'])
+
+        prob.model.add_subsystem('const', om.ExecComp('g = x + y', shape=(3,2,2)), promotes_inputs=['x', 'y'])
+
+        prob.model.set_input_defaults('x', np.ones((3,2,2)) * 3.0)
+        prob.model.set_input_defaults('y', np.ones((3,2,2)) * -4.0)
+
+        prob.driver = om.ScipyOptimizeDriver()
+        prob.driver.options['optimizer'] = 'SLSQP'
+        prob.driver.options['singular_jac_behavior'] = 'error'
+
+        prob.model.add_design_var('x', lower=-50, upper=50)
+        prob.model.add_design_var('y', lower=-50, upper=50)
+        prob.model.add_design_var('z', lower=-50, upper=50)
+
+        # objective parab.f_z is not impacted by any quantities.
+        prob.model.add_objective('parab.f_z', index=6)
+
+        prob.model.add_constraint('const.g', lower=0, upper=10.)
+
+        prob.setup()
+
+        with self.assertRaises(RuntimeError) as msg:
+            prob.run_driver()
+
+        self.assertEqual(str(msg.exception),
+                         "Constraints or objectives [('parab.f_z', inds=[(1, 1, 0)])] cannot be impacted by the design variables of the problem.")
+
 
 class TestScipyOptimizeDriverFeatures(unittest.TestCase):
 
     def test_feature_basic(self):
         import openmdao.api as om
         from openmdao.test_suite.components.paraboloid import Paraboloid
```

### Comparing `openmdao-3.9.1/openmdao/error_checking/check_config.py` & `openmdao-3.9.2/openmdao/error_checking/check_config.py`

 * *Files identical despite different names*

### Comparing `openmdao-3.9.1/openmdao/error_checking/tests/test_check_config.py` & `openmdao-3.9.2/openmdao/error_checking/tests/test_check_config.py`

 * *Files identical despite different names*

### Comparing `openmdao-3.9.1/openmdao/error_checking/tests/test_check_solvers.py` & `openmdao-3.9.2/openmdao/error_checking/tests/test_check_solvers.py`

 * *Files identical despite different names*

### Comparing `openmdao-3.9.1/openmdao/jacobians/assembled_jacobian.py` & `openmdao-3.9.2/openmdao/jacobians/assembled_jacobian.py`

 * *Files identical despite different names*

### Comparing `openmdao-3.9.1/openmdao/jacobians/dictionary_jacobian.py` & `openmdao-3.9.2/openmdao/jacobians/dictionary_jacobian.py`

 * *Files identical despite different names*

### Comparing `openmdao-3.9.1/openmdao/jacobians/jacobian.py` & `openmdao-3.9.2/openmdao/jacobians/jacobian.py`

 * *Files identical despite different names*

### Comparing `openmdao-3.9.1/openmdao/jacobians/tests/test_jacobian.py` & `openmdao-3.9.2/openmdao/jacobians/tests/test_jacobian.py`

 * *Files identical despite different names*

### Comparing `openmdao-3.9.1/openmdao/jacobians/tests/test_jacobian_features.py` & `openmdao-3.9.2/openmdao/jacobians/tests/test_jacobian_features.py`

 * *Files identical despite different names*

### Comparing `openmdao-3.9.1/openmdao/matrices/coo_matrix.py` & `openmdao-3.9.2/openmdao/matrices/coo_matrix.py`

 * *Files identical despite different names*

### Comparing `openmdao-3.9.1/openmdao/matrices/csc_matrix.py` & `openmdao-3.9.2/openmdao/matrices/csc_matrix.py`

 * *Files identical despite different names*

### Comparing `openmdao-3.9.1/openmdao/matrices/csr_matrix.py` & `openmdao-3.9.2/openmdao/matrices/csr_matrix.py`

 * *Files identical despite different names*

### Comparing `openmdao-3.9.1/openmdao/matrices/dense_matrix.py` & `openmdao-3.9.2/openmdao/matrices/dense_matrix.py`

 * *Files identical despite different names*

### Comparing `openmdao-3.9.1/openmdao/matrices/matrix.py` & `openmdao-3.9.2/openmdao/matrices/matrix.py`

 * *Files identical despite different names*

### Comparing `openmdao-3.9.1/openmdao/proc_allocators/default_allocator.py` & `openmdao-3.9.2/openmdao/proc_allocators/default_allocator.py`

 * *Files identical despite different names*

### Comparing `openmdao-3.9.1/openmdao/proc_allocators/proc_allocator.py` & `openmdao-3.9.2/openmdao/proc_allocators/proc_allocator.py`

 * *Files identical despite different names*

### Comparing `openmdao-3.9.1/openmdao/recorders/base_case_reader.py` & `openmdao-3.9.2/openmdao/recorders/base_case_reader.py`

 * *Files identical despite different names*

### Comparing `openmdao-3.9.1/openmdao/recorders/case.py` & `openmdao-3.9.2/openmdao/recorders/case.py`

 * *Files identical despite different names*

### Comparing `openmdao-3.9.1/openmdao/recorders/case_reader.py` & `openmdao-3.9.2/openmdao/recorders/case_reader.py`

 * *Files identical despite different names*

### Comparing `openmdao-3.9.1/openmdao/recorders/case_recorder.py` & `openmdao-3.9.2/openmdao/recorders/case_recorder.py`

 * *Files identical despite different names*

### Comparing `openmdao-3.9.1/openmdao/recorders/recording_iteration_stack.py` & `openmdao-3.9.2/openmdao/recorders/recording_iteration_stack.py`

 * *Files identical despite different names*

### Comparing `openmdao-3.9.1/openmdao/recorders/recording_manager.py` & `openmdao-3.9.2/openmdao/recorders/recording_manager.py`

 * *Files identical despite different names*

### Comparing `openmdao-3.9.1/openmdao/recorders/sqlite_reader.py` & `openmdao-3.9.2/openmdao/recorders/sqlite_reader.py`

 * *Files identical despite different names*

### Comparing `openmdao-3.9.1/openmdao/recorders/sqlite_recorder.py` & `openmdao-3.9.2/openmdao/recorders/sqlite_recorder.py`

 * *Files identical despite different names*

### Comparing `openmdao-3.9.1/openmdao/recorders/tests/legacy_sql/case_database_v4.sql` & `openmdao-3.9.2/openmdao/recorders/tests/legacy_sql/case_database_v4.sql`

 * *Files identical despite different names*

### Comparing `openmdao-3.9.1/openmdao/recorders/tests/legacy_sql/case_driver_01.sql` & `openmdao-3.9.2/openmdao/recorders/tests/legacy_sql/case_driver_01.sql`

 * *Files identical despite different names*

### Comparing `openmdao-3.9.1/openmdao/recorders/tests/legacy_sql/case_driver_pre01.sql` & `openmdao-3.9.2/openmdao/recorders/tests/legacy_sql/case_driver_pre01.sql`

 * *Files identical despite different names*

### Comparing `openmdao-3.9.1/openmdao/recorders/tests/legacy_sql/case_driver_solver_system_02.sql` & `openmdao-3.9.2/openmdao/recorders/tests/legacy_sql/case_driver_solver_system_02.sql`

 * *Files identical despite different names*

### Comparing `openmdao-3.9.1/openmdao/recorders/tests/legacy_sql/case_driver_solver_system_03.sql` & `openmdao-3.9.2/openmdao/recorders/tests/legacy_sql/case_driver_solver_system_03.sql`

 * *Files identical despite different names*

### Comparing `openmdao-3.9.1/openmdao/recorders/tests/legacy_sql/case_driver_v5.sql` & `openmdao-3.9.2/openmdao/recorders/tests/legacy_sql/case_driver_v5.sql`

 * *Files identical despite different names*

### Comparing `openmdao-3.9.1/openmdao/recorders/tests/legacy_sql/case_problem_driver_v7.sql` & `openmdao-3.9.2/openmdao/recorders/tests/legacy_sql/case_problem_driver_v7.sql`

 * *Files identical despite different names*

### Comparing `openmdao-3.9.1/openmdao/recorders/tests/legacy_sql/case_problem_driver_v8.sql` & `openmdao-3.9.2/openmdao/recorders/tests/legacy_sql/case_problem_driver_v8.sql`

 * *Files identical despite different names*

### Comparing `openmdao-3.9.1/openmdao/recorders/tests/legacy_sql/case_problem_v11.sql` & `openmdao-3.9.2/openmdao/recorders/tests/legacy_sql/case_problem_v11.sql`

 * *Files identical despite different names*

### Comparing `openmdao-3.9.1/openmdao/recorders/tests/legacy_sql/case_problem_v6.sql` & `openmdao-3.9.2/openmdao/recorders/tests/legacy_sql/case_problem_v6.sql`

 * *Files identical despite different names*

### Comparing `openmdao-3.9.1/openmdao/recorders/tests/sqlite_recorder_test_utils.py` & `openmdao-3.9.2/openmdao/recorders/tests/sqlite_recorder_test_utils.py`

 * *Files identical despite different names*

### Comparing `openmdao-3.9.1/openmdao/recorders/tests/test_distrib_sqlite_recorder.py` & `openmdao-3.9.2/openmdao/recorders/tests/test_distrib_sqlite_recorder.py`

 * *Files 12% similar despite different names*

```diff
@@ -6,208 +6,207 @@
 from tempfile import mkdtemp
 
 import numpy as np
 
 from openmdao.utils.general_utils import set_pyoptsparse_opt
 from openmdao.utils.mpi import MPI
 
-from openmdao.api import ExecComp, ExplicitComponent, Problem, \
-    Group, ParallelGroup, IndepVarComp, SqliteRecorder, ScipyOptimizeDriver, slicer
+import openmdao.api as om
 from openmdao.utils.array_utils import evenly_distrib_idxs
 from openmdao.recorders.tests.sqlite_recorder_test_utils import \
     assertDriverIterDataRecorded, assertProblemDataRecorded
 from openmdao.recorders.tests.recorder_test_utils import run_driver
 
 if MPI:
     from openmdao.api import PETScVector
 else:
     PETScVector = None
 
 
-class DistributedAdder(ExplicitComponent):
+class DistributedAdder(om.ExplicitComponent):
     """
-    Distributes the work of adding 10 to every item in the param vector
+    Distributes the work of adding 10 to every item in the input vectors
     """
 
-    def __init__(self, size):
+    def __init__(self, sizes):
         super().__init__()
-
-        self.options['distributed'] = True
-
-        self.local_size = self.size = size
+        self.sizes = sizes
 
     def setup(self):
         """
         specify the local sizes of the variables and which specific indices this specific
         distributed component will handle. Indices do NOT need to be sequential or
         contiguous!
         """
         comm = self.comm
         rank = comm.rank
 
-        # NOTE: evenly_distrib_idxs is a helper function to split the array
-        #       up as evenly as possible
-        sizes, offsets = evenly_distrib_idxs(comm.size, self.size)
-        local_size, local_offset = sizes[rank], offsets[rank]
-        self.local_size = local_size
-
-        start = local_offset
-        end = local_offset + local_size
-
-        self.add_input('x', val=np.zeros(local_size, float),
-                       src_indices=np.arange(start, end, dtype=int))
-        self.add_output('y', val=np.zeros(local_size, float))
+        for n, size in enumerate(self.sizes):
+            # NOTE: evenly_distrib_idxs is a helper function to split the array
+            #       up as evenly as possible
+            local_sizes, _ = evenly_distrib_idxs(comm.size, size)
+            local_size = local_sizes[rank]
+
+            self.add_input(f'in{n}', val=np.zeros(local_size, float), distributed=True)
+            self.add_output(f'out{n}', val=np.zeros(local_size, float), distributed=True)
 
     def compute(self, inputs, outputs):
 
         # NOTE: Each process will get just its local part of the vector
-        # print('process {0:d}: {1}'.format(self.comm.rank, params['x'].shape))
-
-        outputs['y'] = inputs['x'] + 10.
+        for n, size in enumerate(self.sizes):
+            outputs[f'out{n}'] = inputs[f'in{n}'] + 10.
 
 
-class Summer(ExplicitComponent):
+class Summer(om.ExplicitComponent):
     """
     Aggregation component that collects all the values from the distributed
-    vector addition and computes a total
+    vectors and computes a total
     """
 
-    def __init__(self, size):
+    def __init__(self, sizes):
         super().__init__()
-        self.size = size
+        self.sizes = sizes
 
     def setup(self):
-        # NOTE: this component depends on the full y array, so OpenMDAO
-        #       will automatically gather all the values for it
-        self.add_input('y', val=np.zeros(self.size))
+        for n, size in enumerate(self.sizes):
+            self.add_input(f'summand{n}', val=np.zeros(size))
+
         self.add_output('sum', 0.0, shape=1)
 
     def compute(self, inputs, outputs):
-        outputs['sum'] = np.sum(inputs['y'])
+        val = 0.
+
+        for name in inputs:
+             val += np.sum(inputs[name])
 
+        outputs['sum'] = val
 
-class Mygroup(Group):
+
+class Mygroup(om.Group):
 
     def setup(self):
-        self.add_subsystem('indep_var_comp', IndepVarComp('x'), promotes=['*'])
-        self.add_subsystem('Cy', ExecComp('y=2*x'), promotes=['*'])
-        self.add_subsystem('Cc', ExecComp('c=x+2'), promotes=['*'])
+        self.add_subsystem('indep_var_comp', om.IndepVarComp('x'), promotes=['*'])
+        self.add_subsystem('Cy', om.ExecComp('y=2*x'), promotes=['*'])
+        self.add_subsystem('Cc', om.ExecComp('c=x+2'), promotes=['*'])
 
         self.add_design_var('x')
         self.add_constraint('c', lower=-3.)
 
 
 @unittest.skipUnless(MPI and PETScVector, "MPI and PETSc are required.")
 class DistributedRecorderTest(unittest.TestCase):
 
     N_PROCS = 2
 
     def setUp(self):
         self.dir = mkdtemp()
         self.filename = os.path.join(self.dir, "sqlite_test")
-        self.recorder = SqliteRecorder(self.filename)
+        self.recorder = om.SqliteRecorder(self.filename)
         self.eps = 1e-5
 
     def tearDown(self):
         try:
             rmtree(self.dir)
         except OSError as e:
             # If directory already deleted, keep going
             if e.errno not in (errno.ENOENT, errno.EACCES, errno.EPERM):
                 raise e
 
     def test_distrib_record_system(self):
-        prob = Problem()
+        prob = om.Problem()
 
         try:
             prob.model.add_recorder(self.recorder)
         except RuntimeError as err:
             msg = "<class Group>: Recording of Systems when running parallel code is not supported yet"
             self.assertEqual(str(err), msg)
         else:
             self.fail('RuntimeError expected.')
 
     def test_distrib_record_solver(self):
-        prob = Problem()
+        prob = om.Problem()
         try:
             prob.model.nonlinear_solver.add_recorder(self.recorder)
         except RuntimeError as err:
             msg = "Recording of Solvers when running parallel code is not supported yet"
             self.assertEqual(str(err), msg)
         else:
             self.fail('RuntimeError expected.')
 
     def test_distrib_record_driver(self):
-        size = 100  # how many items in the array
-        prob = Problem()
+        # create distributed variables of different sizes to catch mismatched collective calls
+        sizes = [7, 10, 12, 25, 33, 42]
+
+        prob = om.Problem()
+
+        ivc = prob.model.add_subsystem('ivc', om.IndepVarComp(), promotes_outputs=['*'])
+        for n, size in enumerate(sizes):
+            ivc.add_output(f'in{n}', np.ones(size), distributed=True)
+            prob.model.add_design_var(f'in{n}')
+
+        prob.model.add_subsystem('adder', DistributedAdder(sizes), promotes=['*'])
+
+        prob.model.add_subsystem('summer', Summer(sizes), promotes_outputs=['sum'])
+        for n, size in enumerate(sizes):
+            prob.model.promotes('summer', inputs=[f'summand{n}'], src_indices=om.slicer[:], src_shape=size)
+        prob.model.add_objective('sum')
 
-        prob.model.add_subsystem('des_vars', IndepVarComp('x', np.ones(size)), promotes=['x'])
-        prob.model.add_subsystem('plus', DistributedAdder(size), promotes=['x', 'y'])
-        prob.model.add_subsystem('summer', Summer(size), promotes_outputs=['sum'])
-        prob.model.promotes('summer', inputs=['y'], src_indices=slicer[:])
         prob.driver.recording_options['record_desvars'] = True
         prob.driver.recording_options['record_objectives'] = True
         prob.driver.recording_options['record_constraints'] = True
-        prob.driver.recording_options['includes'] = ['y']
+        prob.driver.recording_options['includes'] = [f'out{n}' for n in range(len(sizes))]
         prob.driver.add_recorder(self.recorder)
 
-        prob.model.add_design_var('x')
-        prob.model.add_objective('sum')
-
         prob.setup()
-
-        prob['x'] = np.ones(size)
-
         t0, t1 = run_driver(prob)
         prob.cleanup()
 
         coordinate = [0, 'Driver', (0,)]
 
-        expected_desvars = {
-            "des_vars.x": prob['des_vars.x'],
-        }
-
-        expected_objectives = {
-            "summer.sum": prob['summer.sum'],
-        }
+        expected_desvars = {}
+        for n in range(len(sizes)):
+            expected_desvars[f'ivc.in{n}'] = prob.get_val(f'ivc.in{n}', get_remote=True)
+
+        expected_objectives = { "summer.sum": prob['summer.sum'] }
 
         expected_outputs = expected_desvars.copy()
-        expected_outputs['plus.y'] = prob.get_val('plus.y', get_remote=True)
+        for n in range(len(sizes)):
+            expected_outputs[f'adder.out{n}'] = prob.get_val(f'adder.out{n}', get_remote=True)
 
         if prob.comm.rank == 0:
             expected_outputs.update(expected_objectives)
 
             expected_data = ((coordinate, (t0, t1), expected_outputs, None, None),)
             assertDriverIterDataRecorded(self, expected_data, self.eps)
 
     def test_recording_remote_voi(self):
         # Create a parallel model
-        model = Group()
+        model = om.Group()
 
-        model.add_subsystem('par', ParallelGroup())
+        model.add_subsystem('par', om.ParallelGroup())
         model.par.add_subsystem('G1', Mygroup())
         model.par.add_subsystem('G2', Mygroup())
         model.connect('par.G1.y', 'Obj.y1')
         model.connect('par.G2.y', 'Obj.y2')
 
-        model.add_subsystem('Obj', ExecComp('obj=y1+y2'))
+        model.add_subsystem('Obj', om.ExecComp('obj=y1+y2'))
         model.add_objective('Obj.obj')
 
         # Configure driver to record VOIs on both procs
-        driver = ScipyOptimizeDriver(disp=False)
+        driver = om.ScipyOptimizeDriver(disp=False)
 
         driver.recording_options['record_desvars'] = True
         driver.recording_options['record_objectives'] = True
         driver.recording_options['record_constraints'] = True
         driver.recording_options['includes'] = ['par.G1.y', 'par.G2.y']
 
         driver.add_recorder(self.recorder)
 
         # Create problem and run driver
-        prob = Problem(model, driver)
+        prob = om.Problem(model, driver)
         prob.add_recorder(self.recorder)
         prob.setup(mode='fwd')
 
         t0, t1 = run_driver(prob)
         prob.record('final')
         t2 = time()
 
@@ -257,11 +256,48 @@
 
             expected_data = ((coordinate, (t0, t1), expected_outputs, None, None),)
             assertDriverIterDataRecorded(self, expected_data, self.eps)
 
             expected_data = (('final', (t1, t2), expected_outputs),)
             assertProblemDataRecorded(self, expected_data, self.eps)
 
+    def test_input_desvar(self):
+        # this failed with a KeyError before the fix
+        class TopComp(om.ExplicitComponent):
+
+            def setup(self):
+
+                size = 10
+
+                self.add_input('c_ae_C', np.zeros(size))
+                self.add_input('theta_c2_C', np.zeros(size))
+                self.add_output('c_ae', np.zeros(size))
+
+            def compute(self, inputs, outputs):
+                pass
+
+            def compute_partials(self, inputs, partials):
+                pass
+
+        prob = om.Problem()
+        model = prob.model
+
+        geom = model.add_subsystem('tcomp', TopComp())
+
+        model.add_design_var('tcomp.theta_c2_C', lower=-20., upper=20., indices=range(2, 9))
+        model.add_constraint('tcomp.c_ae', lower=0.e0,)
+
+        # Attach recorder to the problem
+        prob.add_recorder(self.recorder)
+        prob.recording_options['record_inputs'] = True
+        prob.recording_options['record_outputs'] = True
+        prob.recording_options['includes'] = ['*']
+
+        prob.setup()
+
+        prob.run_model()
+        prob.record('final')
+
 
 if __name__ == "__main__":
     from openmdao.utils.mpi import mpirun_tests
     mpirun_tests()
```

### Comparing `openmdao-3.9.1/openmdao/recorders/tests/test_sqlite_reader.py` & `openmdao-3.9.2/openmdao/recorders/tests/test_sqlite_reader.py`

 * *Files identical despite different names*

### Comparing `openmdao-3.9.1/openmdao/recorders/tests/test_sqlite_recorder.py` & `openmdao-3.9.2/openmdao/recorders/tests/test_sqlite_recorder.py`

 * *Files identical despite different names*

### Comparing `openmdao-3.9.1/openmdao/solvers/linear/direct.py` & `openmdao-3.9.2/openmdao/solvers/linear/direct.py`

 * *Files identical despite different names*

### Comparing `openmdao-3.9.1/openmdao/solvers/linear/linear_block_gs.py` & `openmdao-3.9.2/openmdao/solvers/linear/linear_block_gs.py`

 * *Files identical despite different names*

### Comparing `openmdao-3.9.1/openmdao/solvers/linear/linear_block_jac.py` & `openmdao-3.9.2/openmdao/solvers/linear/linear_block_jac.py`

 * *Files identical despite different names*

### Comparing `openmdao-3.9.1/openmdao/solvers/linear/linear_runonce.py` & `openmdao-3.9.2/openmdao/solvers/linear/linear_runonce.py`

 * *Files identical despite different names*

### Comparing `openmdao-3.9.1/openmdao/solvers/linear/petsc_ksp.py` & `openmdao-3.9.2/openmdao/solvers/linear/petsc_ksp.py`

 * *Files identical despite different names*

### Comparing `openmdao-3.9.1/openmdao/solvers/linear/scipy_iter_solver.py` & `openmdao-3.9.2/openmdao/solvers/linear/scipy_iter_solver.py`

 * *Files identical despite different names*

### Comparing `openmdao-3.9.1/openmdao/solvers/linear/tests/linear_test_base.py` & `openmdao-3.9.2/openmdao/solvers/linear/tests/linear_test_base.py`

 * *Files identical despite different names*

### Comparing `openmdao-3.9.1/openmdao/solvers/linear/tests/test_direct_solver.py` & `openmdao-3.9.2/openmdao/solvers/linear/tests/test_direct_solver.py`

 * *Files identical despite different names*

### Comparing `openmdao-3.9.1/openmdao/solvers/linear/tests/test_linear_block_gs.py` & `openmdao-3.9.2/openmdao/solvers/linear/tests/test_linear_block_gs.py`

 * *Files identical despite different names*

### Comparing `openmdao-3.9.1/openmdao/solvers/linear/tests/test_linear_block_jac.py` & `openmdao-3.9.2/openmdao/solvers/linear/tests/test_linear_block_jac.py`

 * *Files identical despite different names*

### Comparing `openmdao-3.9.1/openmdao/solvers/linear/tests/test_linear_runonce.py` & `openmdao-3.9.2/openmdao/solvers/linear/tests/test_linear_runonce.py`

 * *Files identical despite different names*

### Comparing `openmdao-3.9.1/openmdao/solvers/linear/tests/test_petsc_ksp.py` & `openmdao-3.9.2/openmdao/solvers/linear/tests/test_petsc_ksp.py`

 * *Files identical despite different names*

### Comparing `openmdao-3.9.1/openmdao/solvers/linear/tests/test_scipy_iter_solver.py` & `openmdao-3.9.2/openmdao/solvers/linear/tests/test_scipy_iter_solver.py`

 * *Files identical despite different names*

### Comparing `openmdao-3.9.1/openmdao/solvers/linear/tests/test_user_defined.py` & `openmdao-3.9.2/openmdao/solvers/linear/tests/test_user_defined.py`

 * *Files identical despite different names*

### Comparing `openmdao-3.9.1/openmdao/solvers/linear/user_defined.py` & `openmdao-3.9.2/openmdao/solvers/linear/user_defined.py`

 * *Files identical despite different names*

### Comparing `openmdao-3.9.1/openmdao/solvers/linesearch/backtracking.py` & `openmdao-3.9.2/openmdao/solvers/linesearch/backtracking.py`

 * *Files identical despite different names*

### Comparing `openmdao-3.9.1/openmdao/solvers/linesearch/tests/test_backtracking.py` & `openmdao-3.9.2/openmdao/solvers/linesearch/tests/test_backtracking.py`

 * *Files identical despite different names*

### Comparing `openmdao-3.9.1/openmdao/solvers/nonlinear/broyden.py` & `openmdao-3.9.2/openmdao/solvers/nonlinear/broyden.py`

 * *Files identical despite different names*

### Comparing `openmdao-3.9.1/openmdao/solvers/nonlinear/newton.py` & `openmdao-3.9.2/openmdao/solvers/nonlinear/newton.py`

 * *Files identical despite different names*

### Comparing `openmdao-3.9.1/openmdao/solvers/nonlinear/nonlinear_block_gs.py` & `openmdao-3.9.2/openmdao/solvers/nonlinear/nonlinear_block_gs.py`

 * *Files identical despite different names*

### Comparing `openmdao-3.9.1/openmdao/solvers/nonlinear/nonlinear_block_jac.py` & `openmdao-3.9.2/openmdao/solvers/nonlinear/nonlinear_block_jac.py`

 * *Files identical despite different names*

### Comparing `openmdao-3.9.1/openmdao/solvers/nonlinear/nonlinear_runonce.py` & `openmdao-3.9.2/openmdao/solvers/nonlinear/nonlinear_runonce.py`

 * *Files identical despite different names*

### Comparing `openmdao-3.9.1/openmdao/solvers/nonlinear/tests/test_broyden.py` & `openmdao-3.9.2/openmdao/solvers/nonlinear/tests/test_broyden.py`

 * *Files identical despite different names*

### Comparing `openmdao-3.9.1/openmdao/solvers/nonlinear/tests/test_newton.py` & `openmdao-3.9.2/openmdao/solvers/nonlinear/tests/test_newton.py`

 * *Files identical despite different names*

### Comparing `openmdao-3.9.1/openmdao/solvers/nonlinear/tests/test_nonlinear_block_gs.py` & `openmdao-3.9.2/openmdao/solvers/nonlinear/tests/test_nonlinear_block_gs.py`

 * *Files identical despite different names*

### Comparing `openmdao-3.9.1/openmdao/solvers/nonlinear/tests/test_nonlinear_block_jac.py` & `openmdao-3.9.2/openmdao/solvers/nonlinear/tests/test_nonlinear_block_jac.py`

 * *Files identical despite different names*

### Comparing `openmdao-3.9.1/openmdao/solvers/nonlinear/tests/test_nonlinear_runonce.py` & `openmdao-3.9.2/openmdao/solvers/nonlinear/tests/test_nonlinear_runonce.py`

 * *Files identical despite different names*

### Comparing `openmdao-3.9.1/openmdao/solvers/solver.py` & `openmdao-3.9.2/openmdao/solvers/solver.py`

 * *Files identical despite different names*

### Comparing `openmdao-3.9.1/openmdao/solvers/tests/test_solver_debug_print.py` & `openmdao-3.9.2/openmdao/solvers/tests/test_solver_debug_print.py`

 * *Files identical despite different names*

### Comparing `openmdao-3.9.1/openmdao/solvers/tests/test_solver_features.py` & `openmdao-3.9.2/openmdao/solvers/tests/test_solver_features.py`

 * *Files identical despite different names*

### Comparing `openmdao-3.9.1/openmdao/solvers/tests/test_solver_iprint.py` & `openmdao-3.9.2/openmdao/solvers/tests/test_solver_iprint.py`

 * *Files identical despite different names*

### Comparing `openmdao-3.9.1/openmdao/solvers/tests/test_solver_parametric_suite.py` & `openmdao-3.9.2/openmdao/solvers/tests/test_solver_parametric_suite.py`

 * *Files identical despite different names*

### Comparing `openmdao-3.9.1/openmdao/surrogate_models/kriging.py` & `openmdao-3.9.2/openmdao/surrogate_models/kriging.py`

 * *Files identical despite different names*

### Comparing `openmdao-3.9.1/openmdao/surrogate_models/multifi_cokriging.py` & `openmdao-3.9.2/openmdao/surrogate_models/multifi_cokriging.py`

 * *Files identical despite different names*

### Comparing `openmdao-3.9.1/openmdao/surrogate_models/nearest_neighbor.py` & `openmdao-3.9.2/openmdao/surrogate_models/nearest_neighbor.py`

 * *Files identical despite different names*

### Comparing `openmdao-3.9.1/openmdao/surrogate_models/nn_interpolators/linear_interpolator.py` & `openmdao-3.9.2/openmdao/surrogate_models/nn_interpolators/linear_interpolator.py`

 * *Files identical despite different names*

### Comparing `openmdao-3.9.1/openmdao/surrogate_models/nn_interpolators/nn_base.py` & `openmdao-3.9.2/openmdao/surrogate_models/nn_interpolators/nn_base.py`

 * *Files identical despite different names*

### Comparing `openmdao-3.9.1/openmdao/surrogate_models/nn_interpolators/rbf_interpolator.py` & `openmdao-3.9.2/openmdao/surrogate_models/nn_interpolators/rbf_interpolator.py`

 * *Files identical despite different names*

### Comparing `openmdao-3.9.1/openmdao/surrogate_models/nn_interpolators/weighted_interpolator.py` & `openmdao-3.9.2/openmdao/surrogate_models/nn_interpolators/weighted_interpolator.py`

 * *Files identical despite different names*

### Comparing `openmdao-3.9.1/openmdao/surrogate_models/response_surface.py` & `openmdao-3.9.2/openmdao/surrogate_models/response_surface.py`

 * *Files identical despite different names*

### Comparing `openmdao-3.9.1/openmdao/surrogate_models/surrogate_model.py` & `openmdao-3.9.2/openmdao/surrogate_models/surrogate_model.py`

 * *Files identical despite different names*

### Comparing `openmdao-3.9.1/openmdao/surrogate_models/tests/test_kriging.py` & `openmdao-3.9.2/openmdao/surrogate_models/tests/test_kriging.py`

 * *Files identical despite different names*

### Comparing `openmdao-3.9.1/openmdao/surrogate_models/tests/test_map.py` & `openmdao-3.9.2/openmdao/surrogate_models/tests/test_map.py`

 * *Files identical despite different names*

### Comparing `openmdao-3.9.1/openmdao/surrogate_models/tests/test_multifi_cokriging.py` & `openmdao-3.9.2/openmdao/surrogate_models/tests/test_multifi_cokriging.py`

 * *Files identical despite different names*

### Comparing `openmdao-3.9.1/openmdao/surrogate_models/tests/test_nearest_neighbor.py` & `openmdao-3.9.2/openmdao/surrogate_models/tests/test_nearest_neighbor.py`

 * *Files identical despite different names*

### Comparing `openmdao-3.9.1/openmdao/surrogate_models/tests/test_response_surface.py` & `openmdao-3.9.2/openmdao/surrogate_models/tests/test_response_surface.py`

 * *Files identical despite different names*

### Comparing `openmdao-3.9.1/openmdao/test_suite/build4test.py` & `openmdao-3.9.2/openmdao/test_suite/build4test.py`

 * *Files identical despite different names*

### Comparing `openmdao-3.9.1/openmdao/test_suite/components/ae_tests.py` & `openmdao-3.9.2/openmdao/test_suite/components/ae_tests.py`

 * *Files identical despite different names*

### Comparing `openmdao-3.9.1/openmdao/test_suite/components/array_comp.py` & `openmdao-3.9.2/openmdao/test_suite/components/array_comp.py`

 * *Files identical despite different names*

### Comparing `openmdao-3.9.1/openmdao/test_suite/components/branin.py` & `openmdao-3.9.2/openmdao/test_suite/components/branin.py`

 * *Files identical despite different names*

### Comparing `openmdao-3.9.1/openmdao/test_suite/components/cycle_comps.py` & `openmdao-3.9.2/openmdao/test_suite/components/cycle_comps.py`

 * *Files identical despite different names*

### Comparing `openmdao-3.9.1/openmdao/test_suite/components/distributed_components.py` & `openmdao-3.9.2/openmdao/test_suite/components/distributed_components.py`

 * *Files identical despite different names*

### Comparing `openmdao-3.9.1/openmdao/test_suite/components/double_sellar.py` & `openmdao-3.9.2/openmdao/test_suite/components/double_sellar.py`

 * *Files identical despite different names*

### Comparing `openmdao-3.9.1/openmdao/test_suite/components/eggcrate.py` & `openmdao-3.9.2/openmdao/test_suite/components/eggcrate.py`

 * *Files identical despite different names*

### Comparing `openmdao-3.9.1/openmdao/test_suite/components/exec_comp_for_test.py` & `openmdao-3.9.2/openmdao/test_suite/components/exec_comp_for_test.py`

 * *Files identical despite different names*

### Comparing `openmdao-3.9.1/openmdao/test_suite/components/expl_comp_array.py` & `openmdao-3.9.2/openmdao/test_suite/components/expl_comp_array.py`

 * *Files identical despite different names*

### Comparing `openmdao-3.9.1/openmdao/test_suite/components/expl_comp_simple.py` & `openmdao-3.9.2/openmdao/test_suite/components/expl_comp_simple.py`

 * *Files identical despite different names*

### Comparing `openmdao-3.9.1/openmdao/test_suite/components/impl_comp_array.py` & `openmdao-3.9.2/openmdao/test_suite/components/impl_comp_array.py`

 * *Files identical despite different names*

### Comparing `openmdao-3.9.1/openmdao/test_suite/components/impl_comp_simple.py` & `openmdao-3.9.2/openmdao/test_suite/components/impl_comp_simple.py`

 * *Files identical despite different names*

### Comparing `openmdao-3.9.1/openmdao/test_suite/components/implicit_newton_linesearch.py` & `openmdao-3.9.2/openmdao/test_suite/components/implicit_newton_linesearch.py`

 * *Files identical despite different names*

### Comparing `openmdao-3.9.1/openmdao/test_suite/components/matmultcomp.py` & `openmdao-3.9.2/openmdao/test_suite/components/matmultcomp.py`

 * *Files identical despite different names*

### Comparing `openmdao-3.9.1/openmdao/test_suite/components/misc_components.py` & `openmdao-3.9.2/openmdao/test_suite/components/misc_components.py`

 * *Files identical despite different names*

### Comparing `openmdao-3.9.1/openmdao/test_suite/components/options_feature_array.py` & `openmdao-3.9.2/openmdao/test_suite/components/options_feature_array.py`

 * *Files identical despite different names*

### Comparing `openmdao-3.9.1/openmdao/test_suite/components/options_feature_function.py` & `openmdao-3.9.2/openmdao/test_suite/components/options_feature_function.py`

 * *Files identical despite different names*

### Comparing `openmdao-3.9.1/openmdao/test_suite/components/options_feature_lincomb.py` & `openmdao-3.9.2/openmdao/test_suite/components/options_feature_lincomb.py`

 * *Files identical despite different names*

### Comparing `openmdao-3.9.1/openmdao/test_suite/components/options_feature_vector.py` & `openmdao-3.9.2/openmdao/test_suite/components/options_feature_vector.py`

 * *Files identical despite different names*

### Comparing `openmdao-3.9.1/openmdao/test_suite/components/paraboloid.py` & `openmdao-3.9.2/openmdao/test_suite/components/paraboloid.py`

 * *Files identical despite different names*

### Comparing `openmdao-3.9.1/openmdao/test_suite/components/paraboloid_distributed.py` & `openmdao-3.9.2/openmdao/test_suite/components/paraboloid_distributed.py`

 * *Files identical despite different names*

### Comparing `openmdao-3.9.1/openmdao/test_suite/components/paraboloid_feature.py` & `openmdao-3.9.2/openmdao/test_suite/components/paraboloid_feature.py`

 * *Files identical despite different names*

### Comparing `openmdao-3.9.1/openmdao/test_suite/components/paraboloid_mat_vec.py` & `openmdao-3.9.2/openmdao/test_suite/components/paraboloid_mat_vec.py`

 * *Files identical despite different names*

### Comparing `openmdao-3.9.1/openmdao/test_suite/components/paraboloid_problem.py` & `openmdao-3.9.2/openmdao/test_suite/components/paraboloid_problem.py`

 * *Files identical despite different names*

### Comparing `openmdao-3.9.1/openmdao/test_suite/components/partial_check_feature.py` & `openmdao-3.9.2/openmdao/test_suite/components/partial_check_feature.py`

 * *Files identical despite different names*

### Comparing `openmdao-3.9.1/openmdao/test_suite/components/quad_implicit.py` & `openmdao-3.9.2/openmdao/test_suite/components/quad_implicit.py`

 * *Files identical despite different names*

### Comparing `openmdao-3.9.1/openmdao/test_suite/components/sellar.py` & `openmdao-3.9.2/openmdao/test_suite/components/sellar.py`

 * *Files identical despite different names*

### Comparing `openmdao-3.9.1/openmdao/test_suite/components/sellar_feature.py` & `openmdao-3.9.2/openmdao/test_suite/components/sellar_feature.py`

 * *Files identical despite different names*

### Comparing `openmdao-3.9.1/openmdao/test_suite/components/simple_comps.py` & `openmdao-3.9.2/openmdao/test_suite/components/simple_comps.py`

 * *Files identical despite different names*

### Comparing `openmdao-3.9.1/openmdao/test_suite/components/three_bar_truss.py` & `openmdao-3.9.2/openmdao/test_suite/components/three_bar_truss.py`

 * *Files identical despite different names*

### Comparing `openmdao-3.9.1/openmdao/test_suite/components/unit_conv.py` & `openmdao-3.9.2/openmdao/test_suite/components/unit_conv.py`

 * *Files identical despite different names*

### Comparing `openmdao-3.9.1/openmdao/test_suite/groups/cycle_group.py` & `openmdao-3.9.2/openmdao/test_suite/groups/cycle_group.py`

 * *Files identical despite different names*

### Comparing `openmdao-3.9.1/openmdao/test_suite/groups/implicit_group.py` & `openmdao-3.9.2/openmdao/test_suite/groups/implicit_group.py`

 * *Files identical despite different names*

### Comparing `openmdao-3.9.1/openmdao/test_suite/groups/parallel_groups.py` & `openmdao-3.9.2/openmdao/test_suite/groups/parallel_groups.py`

 * *Files identical despite different names*

### Comparing `openmdao-3.9.1/openmdao/test_suite/groups/parametric_group.py` & `openmdao-3.9.2/openmdao/test_suite/groups/parametric_group.py`

 * *Files identical despite different names*

### Comparing `openmdao-3.9.1/openmdao/test_suite/groups/sin_fitter.py` & `openmdao-3.9.2/openmdao/test_suite/groups/sin_fitter.py`

 * *Files identical despite different names*

### Comparing `openmdao-3.9.1/openmdao/test_suite/matrices/D_6.npz` & `openmdao-3.9.2/openmdao/test_suite/matrices/D_6.npz`

 * *Files identical despite different names*

### Comparing `openmdao-3.9.1/openmdao/test_suite/matrices/Harvard500.npz` & `openmdao-3.9.2/openmdao/test_suite/matrices/Harvard500.npz`

 * *Files identical despite different names*

### Comparing `openmdao-3.9.1/openmdao/test_suite/matrices/af23560.npz` & `openmdao-3.9.2/openmdao/test_suite/matrices/af23560.npz`

 * *Files identical despite different names*

### Comparing `openmdao-3.9.1/openmdao/test_suite/matrices/ash331.npz` & `openmdao-3.9.2/openmdao/test_suite/matrices/ash331.npz`

 * *Files identical despite different names*

### Comparing `openmdao-3.9.1/openmdao/test_suite/matrices/ash608.npz` & `openmdao-3.9.2/openmdao/test_suite/matrices/ash608.npz`

 * *Files identical despite different names*

### Comparing `openmdao-3.9.1/openmdao/test_suite/matrices/bibd_12_5.npz` & `openmdao-3.9.2/openmdao/test_suite/matrices/bibd_12_5.npz`

 * *Files identical despite different names*

### Comparing `openmdao-3.9.1/openmdao/test_suite/matrices/can_715.npz` & `openmdao-3.9.2/openmdao/test_suite/matrices/can_715.npz`

 * *Files identical despite different names*

### Comparing `openmdao-3.9.1/openmdao/test_suite/matrices/color_mats.py` & `openmdao-3.9.2/openmdao/test_suite/matrices/color_mats.py`

 * *Files identical despite different names*

### Comparing `openmdao-3.9.1/openmdao/test_suite/matrices/dl_matrix.py` & `openmdao-3.9.2/openmdao/test_suite/matrices/dl_matrix.py`

 * *Files identical despite different names*

### Comparing `openmdao-3.9.1/openmdao/test_suite/matrices/e40r0100.npz` & `openmdao-3.9.2/openmdao/test_suite/matrices/e40r0100.npz`

 * *Files identical despite different names*

### Comparing `openmdao-3.9.1/openmdao/test_suite/matrices/illc1033.npz` & `openmdao-3.9.2/openmdao/test_suite/matrices/illc1033.npz`

 * *Files identical despite different names*

### Comparing `openmdao-3.9.1/openmdao/test_suite/matrices/lp_cre_a.npz` & `openmdao-3.9.2/openmdao/test_suite/matrices/lp_cre_a.npz`

 * *Files identical despite different names*

### Comparing `openmdao-3.9.1/openmdao/test_suite/matrices/lp_dfl001.npz` & `openmdao-3.9.2/openmdao/test_suite/matrices/lp_dfl001.npz`

 * *Files identical despite different names*

### Comparing `openmdao-3.9.1/openmdao/test_suite/matrices/lp_finnis.npz` & `openmdao-3.9.2/openmdao/test_suite/matrices/lp_finnis.npz`

 * *Files identical despite different names*

### Comparing `openmdao-3.9.1/openmdao/test_suite/matrices/lp_maros_r7.npz` & `openmdao-3.9.2/openmdao/test_suite/matrices/lp_maros_r7.npz`

 * *Files identical despite different names*

### Comparing `openmdao-3.9.1/openmdao/test_suite/matrices/m3plates.npz` & `openmdao-3.9.2/openmdao/test_suite/matrices/m3plates.npz`

 * *Files identical despite different names*

### Comparing `openmdao-3.9.1/openmdao/test_suite/matrices/ml2np.py` & `openmdao-3.9.2/openmdao/test_suite/matrices/ml2np.py`

 * *Files identical despite different names*

### Comparing `openmdao-3.9.1/openmdao/test_suite/matrices/n4c6-b15.npz` & `openmdao-3.9.2/openmdao/test_suite/matrices/n4c6-b15.npz`

 * *Files identical despite different names*

### Comparing `openmdao-3.9.1/openmdao/test_suite/parametric_suite.py` & `openmdao-3.9.2/openmdao/test_suite/parametric_suite.py`

 * *Files identical despite different names*

### Comparing `openmdao-3.9.1/openmdao/test_suite/scripts/bad_connection.py` & `openmdao-3.9.2/openmdao/test_suite/scripts/bad_connection.py`

 * *Files identical despite different names*

### Comparing `openmdao-3.9.1/openmdao/test_suite/scripts/beam_opt.py` & `openmdao-3.9.2/openmdao/test_suite/scripts/beam_opt.py`

 * *Files identical despite different names*

### Comparing `openmdao-3.9.1/openmdao/test_suite/scripts/circle_opt.py` & `openmdao-3.9.2/openmdao/test_suite/scripts/circle_opt.py`

 * *Files identical despite different names*

### Comparing `openmdao-3.9.1/openmdao/test_suite/scripts/circuit.py` & `openmdao-3.9.2/openmdao/test_suite/scripts/circuit.py`

 * *Files identical despite different names*

### Comparing `openmdao-3.9.1/openmdao/test_suite/scripts/circuit_analysis.py` & `openmdao-3.9.2/openmdao/test_suite/scripts/circuit_analysis.py`

 * *Files identical despite different names*

### Comparing `openmdao-3.9.1/openmdao/test_suite/scripts/circuit_with_unconnected_input.py` & `openmdao-3.9.2/openmdao/test_suite/scripts/circuit_with_unconnected_input.py`

 * *Files identical despite different names*

### Comparing `openmdao-3.9.1/openmdao/test_suite/scripts/dyn_system.py` & `openmdao-3.9.2/openmdao/test_suite/scripts/dyn_system.py`

 * *Files identical despite different names*

### Comparing `openmdao-3.9.1/openmdao/test_suite/scripts/multipoint_beam_opt.py` & `openmdao-3.9.2/openmdao/test_suite/scripts/multipoint_beam_opt.py`

 * *Files identical despite different names*

### Comparing `openmdao-3.9.1/openmdao/test_suite/scripts/sellar.py` & `openmdao-3.9.2/openmdao/test_suite/scripts/sellar.py`

 * *Files identical despite different names*

### Comparing `openmdao-3.9.1/openmdao/test_suite/test_examples/basic_opt_paraboloid.py` & `openmdao-3.9.2/openmdao/test_suite/test_examples/basic_opt_paraboloid.py`

 * *Files identical despite different names*

### Comparing `openmdao-3.9.1/openmdao/test_suite/test_examples/beam_optimization/beam_group.py` & `openmdao-3.9.2/openmdao/test_suite/test_examples/beam_optimization/beam_group.py`

 * *Files identical despite different names*

### Comparing `openmdao-3.9.1/openmdao/test_suite/test_examples/beam_optimization/components/compliance_comp.py` & `openmdao-3.9.2/openmdao/test_suite/test_examples/beam_optimization/components/compliance_comp.py`

 * *Files identical despite different names*

### Comparing `openmdao-3.9.1/openmdao/test_suite/test_examples/beam_optimization/components/local_stiffness_matrix_comp.py` & `openmdao-3.9.2/openmdao/test_suite/test_examples/beam_optimization/components/local_stiffness_matrix_comp.py`

 * *Files identical despite different names*

### Comparing `openmdao-3.9.1/openmdao/test_suite/test_examples/beam_optimization/components/moment_comp.py` & `openmdao-3.9.2/openmdao/test_suite/test_examples/beam_optimization/components/moment_comp.py`

 * *Files identical despite different names*

### Comparing `openmdao-3.9.1/openmdao/test_suite/test_examples/beam_optimization/components/multi_compliance_comp.py` & `openmdao-3.9.2/openmdao/test_suite/test_examples/beam_optimization/components/multi_compliance_comp.py`

 * *Files identical despite different names*

### Comparing `openmdao-3.9.1/openmdao/test_suite/test_examples/beam_optimization/components/multi_states_comp.py` & `openmdao-3.9.2/openmdao/test_suite/test_examples/beam_optimization/components/multi_states_comp.py`

 * *Files identical despite different names*

### Comparing `openmdao-3.9.1/openmdao/test_suite/test_examples/beam_optimization/components/multi_stress_comp.py` & `openmdao-3.9.2/openmdao/test_suite/test_examples/beam_optimization/components/multi_stress_comp.py`

 * *Files identical despite different names*

### Comparing `openmdao-3.9.1/openmdao/test_suite/test_examples/beam_optimization/components/states_comp.py` & `openmdao-3.9.2/openmdao/test_suite/test_examples/beam_optimization/components/states_comp.py`

 * *Files identical despite different names*

### Comparing `openmdao-3.9.1/openmdao/test_suite/test_examples/beam_optimization/components/volume_comp.py` & `openmdao-3.9.2/openmdao/test_suite/test_examples/beam_optimization/components/volume_comp.py`

 * *Files identical despite different names*

### Comparing `openmdao-3.9.1/openmdao/test_suite/test_examples/beam_optimization/multipoint_beam_group.py` & `openmdao-3.9.2/openmdao/test_suite/test_examples/beam_optimization/multipoint_beam_group.py`

 * *Files identical despite different names*

### Comparing `openmdao-3.9.1/openmdao/test_suite/test_examples/beam_optimization/multipoint_beam_stress.py` & `openmdao-3.9.2/openmdao/test_suite/test_examples/beam_optimization/multipoint_beam_stress.py`

 * *Files identical despite different names*

### Comparing `openmdao-3.9.1/openmdao/test_suite/test_examples/beam_optimization/test_beam_optimization.py` & `openmdao-3.9.2/openmdao/test_suite/test_examples/beam_optimization/test_beam_optimization.py`

 * *Files identical despite different names*

### Comparing `openmdao-3.9.1/openmdao/test_suite/test_examples/cannonball/cannonball_ode.py` & `openmdao-3.9.2/openmdao/test_suite/test_examples/cannonball/cannonball_ode.py`

 * *Files identical despite different names*

### Comparing `openmdao-3.9.1/openmdao/test_suite/test_examples/cannonball/test_euler_integration.py` & `openmdao-3.9.2/openmdao/test_suite/test_examples/cannonball/test_euler_integration.py`

 * *Files identical despite different names*

### Comparing `openmdao-3.9.1/openmdao/test_suite/test_examples/meta_model_examples/structured_meta_model_example.py` & `openmdao-3.9.2/openmdao/test_suite/test_examples/meta_model_examples/structured_meta_model_example.py`

 * *Files identical despite different names*

### Comparing `openmdao-3.9.1/openmdao/test_suite/test_examples/meta_model_examples/unstructured_meta_model_example.py` & `openmdao-3.9.2/openmdao/test_suite/test_examples/meta_model_examples/unstructured_meta_model_example.py`

 * *Files identical despite different names*

### Comparing `openmdao-3.9.1/openmdao/test_suite/test_examples/test_betz_limit.py` & `openmdao-3.9.2/openmdao/test_suite/test_examples/test_betz_limit.py`

 * *Files identical despite different names*

### Comparing `openmdao-3.9.1/openmdao/test_suite/test_examples/test_circuit_analysis.py` & `openmdao-3.9.2/openmdao/test_suite/test_examples/test_circuit_analysis.py`

 * *Files identical despite different names*

### Comparing `openmdao-3.9.1/openmdao/test_suite/test_examples/test_circuit_analysis_derivs.py` & `openmdao-3.9.2/openmdao/test_suite/test_examples/test_circuit_analysis_derivs.py`

 * *Files identical despite different names*

### Comparing `openmdao-3.9.1/openmdao/test_suite/test_examples/test_hohmann_transfer.py` & `openmdao-3.9.2/openmdao/test_suite/test_examples/test_hohmann_transfer.py`

 * *Files identical despite different names*

### Comparing `openmdao-3.9.1/openmdao/test_suite/test_examples/test_keplers_equation.py` & `openmdao-3.9.2/openmdao/test_suite/test_examples/test_keplers_equation.py`

 * *Files identical despite different names*

### Comparing `openmdao-3.9.1/openmdao/test_suite/test_examples/test_sellar_mda_promote_connect.py` & `openmdao-3.9.2/openmdao/test_suite/test_examples/test_sellar_mda_promote_connect.py`

 * *Files identical despite different names*

### Comparing `openmdao-3.9.1/openmdao/test_suite/test_examples/test_sellar_opt.py` & `openmdao-3.9.2/openmdao/test_suite/test_examples/test_sellar_opt.py`

 * *Files identical despite different names*

### Comparing `openmdao-3.9.1/openmdao/test_suite/test_examples/test_tldr_paraboloid.py` & `openmdao-3.9.2/openmdao/test_suite/test_examples/test_tldr_paraboloid.py`

 * *Files identical despite different names*

### Comparing `openmdao-3.9.1/openmdao/test_suite/tests/test_auto_ivc_api_conversion.py` & `openmdao-3.9.2/openmdao/test_suite/tests/test_auto_ivc_api_conversion.py`

 * *Files identical despite different names*

### Comparing `openmdao-3.9.1/openmdao/test_suite/tests/test_feature_sellar.py` & `openmdao-3.9.2/openmdao/test_suite/tests/test_feature_sellar.py`

 * *Files identical despite different names*

### Comparing `openmdao-3.9.1/openmdao/test_suite/tests/test_general.py` & `openmdao-3.9.2/openmdao/test_suite/tests/test_general.py`

 * *Files identical despite different names*

### Comparing `openmdao-3.9.1/openmdao/test_suite/tests/test_paraboloid_feature.py` & `openmdao-3.9.2/openmdao/test_suite/tests/test_paraboloid_feature.py`

 * *Files identical despite different names*

### Comparing `openmdao-3.9.1/openmdao/test_suite/tests/test_quad_implicit.py` & `openmdao-3.9.2/openmdao/test_suite/tests/test_quad_implicit.py`

 * *Files identical despite different names*

### Comparing `openmdao-3.9.1/openmdao/test_suite/tests/test_warnings.py` & `openmdao-3.9.2/openmdao/test_suite/tests/test_warnings.py`

 * *Files identical despite different names*

### Comparing `openmdao-3.9.1/openmdao/test_suite/tot_jac_builder.py` & `openmdao-3.9.2/openmdao/test_suite/tot_jac_builder.py`

 * *Files identical despite different names*

### Comparing `openmdao-3.9.1/openmdao/utils/array_utils.py` & `openmdao-3.9.2/openmdao/utils/array_utils.py`

 * *Files identical despite different names*

### Comparing `openmdao-3.9.1/openmdao/utils/assert_utils.py` & `openmdao-3.9.2/openmdao/utils/assert_utils.py`

 * *Files identical despite different names*

### Comparing `openmdao-3.9.1/openmdao/utils/class_util.py` & `openmdao-3.9.2/openmdao/utils/class_util.py`

 * *Files identical despite different names*

### Comparing `openmdao-3.9.1/openmdao/utils/code_utils.py` & `openmdao-3.9.2/openmdao/utils/code_utils.py`

 * *Files identical despite different names*

### Comparing `openmdao-3.9.1/openmdao/utils/coloring.py` & `openmdao-3.9.2/openmdao/utils/coloring.py`

 * *Files identical despite different names*

### Comparing `openmdao-3.9.1/openmdao/utils/concurrent.py` & `openmdao-3.9.2/openmdao/utils/concurrent.py`

 * *Files identical despite different names*

### Comparing `openmdao-3.9.1/openmdao/utils/cs_safe.py` & `openmdao-3.9.2/openmdao/utils/cs_safe.py`

 * *Files identical despite different names*

### Comparing `openmdao-3.9.1/openmdao/utils/entry_points.py` & `openmdao-3.9.2/openmdao/utils/entry_points.py`

 * *Files identical despite different names*

### Comparing `openmdao-3.9.1/openmdao/utils/file_utils.py` & `openmdao-3.9.2/openmdao/utils/file_utils.py`

 * *Files identical despite different names*

### Comparing `openmdao-3.9.1/openmdao/utils/file_wrap.py` & `openmdao-3.9.2/openmdao/utils/file_wrap.py`

 * *Files 1% similar despite different names*

```diff
@@ -158,15 +158,15 @@
                 newval = str(self._newtext[self._counter])
             self._counter += 1
             return newval
         else:
             return text.group()
 
 
-class ToInteger(TokenConverter):
+class _ToInteger(TokenConverter):
     """
     Converter for PyParsing that is used to turn a token into an int.
     """
 
     def postParse(self, instring, loc, tokenlist):
         """
         Convert token into an integer.
@@ -184,15 +184,15 @@
         -------
         int
             integer value for token.
         """
         return int(tokenlist[0])
 
 
-class ToFloat(TokenConverter):
+class _ToFloat(TokenConverter):
     """
     Converter for PyParsing that is used to turn a token into a float.
     """
 
     def postParse(self, instring, loc, tokenlist):
         """
         Convert token into a float.
@@ -210,15 +210,15 @@
         -------
         float
             float value for token.
         """
         return float(tokenlist[0].replace('D', 'E'))
 
 
-class ToNan(TokenConverter):
+class _ToNan(TokenConverter):
     """
     Converter for PyParsing that is used to turn a token into Python nan.
     """
 
     def postParse(self, instring, loc, tokenlist):
         """
         Convert token into Python nan.
@@ -236,15 +236,15 @@
         -------
         float
             the float value for NaN.
         """
         return float('nan')
 
 
-class ToInf(TokenConverter):
+class _ToInf(TokenConverter):
     """
     Converter for PyParsing that is used to turn a token into Python inf.
     """
 
     def postParse(self, instring, loc, tokenlist):
         """
         Convert token into Python inf.
@@ -1065,24 +1065,24 @@
                     textchars = textchars + symbol
 
         digits = Word(nums)
         dot = "."
         sign = oneOf("+ -")
         ee = CaselessLiteral('E') | CaselessLiteral('D')
 
-        num_int = ToInteger(Combine(Optional(sign) + digits))
+        num_int = _ToInteger(Combine(Optional(sign) + digits))
 
-        num_float = ToFloat(Combine(
+        num_float = _ToFloat(Combine(
             Optional(sign) +
             ((digits + dot + Optional(digits)) | (dot + digits)) +
             Optional(ee + Optional(sign) + digits)
         ))
 
         # special case for a float written like "3e5"
-        mixed_exp = ToFloat(Combine(digits + ee + Optional(sign) + digits))
+        mixed_exp = _ToFloat(Combine(digits + ee + Optional(sign) + digits))
 
-        nan = (ToInf(oneOf("Inf -Inf")) |
-               ToNan(oneOf("NaN nan NaN%  NaNQ NaNS qNaN sNaN 1.#SNAN 1.#QNAN -1.#IND")))
+        nan = (_ToInf(oneOf("Inf -Inf")) |
+               _ToNan(oneOf("NaN nan NaN%  NaNQ NaNS qNaN sNaN 1.#SNAN 1.#QNAN -1.#IND")))
 
         string_text = Word(textchars)
 
         self.line_parse_token = (OneOrMore((nan | num_float | mixed_exp | num_int | string_text)))
```

### Comparing `openmdao-3.9.1/openmdao/utils/find_cite.py` & `openmdao-3.9.2/openmdao/utils/find_cite.py`

 * *Files identical despite different names*

### Comparing `openmdao-3.9.1/openmdao/utils/general_utils.py` & `openmdao-3.9.2/openmdao/utils/general_utils.py`

 * *Files identical despite different names*

### Comparing `openmdao-3.9.1/openmdao/utils/graph_utils.py` & `openmdao-3.9.2/openmdao/utils/graph_utils.py`

 * *Files identical despite different names*

### Comparing `openmdao-3.9.1/openmdao/utils/hooks.py` & `openmdao-3.9.2/openmdao/utils/hooks.py`

 * *Files identical despite different names*

### Comparing `openmdao-3.9.1/openmdao/utils/logger_utils.py` & `openmdao-3.9.2/openmdao/utils/logger_utils.py`

 * *Files identical despite different names*

### Comparing `openmdao-3.9.1/openmdao/utils/mpi.py` & `openmdao-3.9.2/openmdao/utils/mpi.py`

 * *Files identical despite different names*

### Comparing `openmdao-3.9.1/openmdao/utils/name_maps.py` & `openmdao-3.9.2/openmdao/utils/name_maps.py`

 * *Files identical despite different names*

### Comparing `openmdao-3.9.1/openmdao/utils/notebook_utils.py` & `openmdao-3.9.2/openmdao/utils/notebook_utils.py`

 * *Files identical despite different names*

### Comparing `openmdao-3.9.1/openmdao/utils/om.py` & `openmdao-3.9.2/openmdao/utils/om.py`

 * *Files identical despite different names*

### Comparing `openmdao-3.9.1/openmdao/utils/options_dictionary.py` & `openmdao-3.9.2/openmdao/utils/options_dictionary.py`

 * *Files identical despite different names*

### Comparing `openmdao-3.9.1/openmdao/utils/record_util.py` & `openmdao-3.9.2/openmdao/utils/record_util.py`

 * *Files identical despite different names*

### Comparing `openmdao-3.9.1/openmdao/utils/scaffold.py` & `openmdao-3.9.2/openmdao/utils/scaffold.py`

 * *Files identical despite different names*

### Comparing `openmdao-3.9.1/openmdao/utils/scaffolding_templates/BaseCaseReader_template` & `openmdao-3.9.2/openmdao/utils/scaffolding_templates/BaseCaseReader_template`

 * *Files identical despite different names*

### Comparing `openmdao-3.9.1/openmdao/utils/scaffolding_templates/CaseRecorder_template` & `openmdao-3.9.2/openmdao/utils/scaffolding_templates/CaseRecorder_template`

 * *Files identical despite different names*

### Comparing `openmdao-3.9.1/openmdao/utils/scaffolding_templates/Driver_template` & `openmdao-3.9.2/openmdao/utils/scaffolding_templates/Driver_template`

 * *Files identical despite different names*

### Comparing `openmdao-3.9.1/openmdao/utils/scaffolding_templates/ExplicitComponent_template` & `openmdao-3.9.2/openmdao/utils/scaffolding_templates/ExplicitComponent_template`

 * *Files identical despite different names*

### Comparing `openmdao-3.9.1/openmdao/utils/scaffolding_templates/Group_template` & `openmdao-3.9.2/openmdao/utils/scaffolding_templates/Group_template`

 * *Files identical despite different names*

### Comparing `openmdao-3.9.1/openmdao/utils/scaffolding_templates/ImplicitComponent_template` & `openmdao-3.9.2/openmdao/utils/scaffolding_templates/ImplicitComponent_template`

 * *Files identical despite different names*

### Comparing `openmdao-3.9.1/openmdao/utils/scaffolding_templates/LinearSolver_template` & `openmdao-3.9.2/openmdao/utils/scaffolding_templates/LinearSolver_template`

 * *Files identical despite different names*

### Comparing `openmdao-3.9.1/openmdao/utils/scaffolding_templates/NonlinearSolver_template` & `openmdao-3.9.2/openmdao/utils/scaffolding_templates/NonlinearSolver_template`

 * *Files identical despite different names*

### Comparing `openmdao-3.9.1/openmdao/utils/scaffolding_templates/SurrogateModel_template` & `openmdao-3.9.2/openmdao/utils/scaffolding_templates/SurrogateModel_template`

 * *Files identical despite different names*

### Comparing `openmdao-3.9.1/openmdao/utils/scaffolding_templates/command_template` & `openmdao-3.9.2/openmdao/utils/scaffolding_templates/command_template`

 * *Files identical despite different names*

### Comparing `openmdao-3.9.1/openmdao/utils/scaffolding_templates/test_template` & `openmdao-3.9.2/openmdao/utils/scaffolding_templates/test_template`

 * *Files identical despite different names*

### Comparing `openmdao-3.9.1/openmdao/utils/shell_proc.py` & `openmdao-3.9.2/openmdao/utils/shell_proc.py`

 * *Files identical despite different names*

### Comparing `openmdao-3.9.1/openmdao/utils/spline_distributions.py` & `openmdao-3.9.2/openmdao/utils/spline_distributions.py`

 * *Files identical despite different names*

### Comparing `openmdao-3.9.1/openmdao/utils/tests/test_array_utils.py` & `openmdao-3.9.2/openmdao/utils/tests/test_array_utils.py`

 * *Files identical despite different names*

### Comparing `openmdao-3.9.1/openmdao/utils/tests/test_assert_utils.py` & `openmdao-3.9.2/openmdao/utils/tests/test_assert_utils.py`

 * *Files identical despite different names*

### Comparing `openmdao-3.9.1/openmdao/utils/tests/test_cmdline.py` & `openmdao-3.9.2/openmdao/utils/tests/test_cmdline.py`

 * *Files identical despite different names*

### Comparing `openmdao-3.9.1/openmdao/utils/tests/test_code_utils.py` & `openmdao-3.9.2/openmdao/utils/tests/test_code_utils.py`

 * *Files identical despite different names*

### Comparing `openmdao-3.9.1/openmdao/utils/tests/test_cs_safe.py` & `openmdao-3.9.2/openmdao/utils/tests/test_cs_safe.py`

 * *Files identical despite different names*

### Comparing `openmdao-3.9.1/openmdao/utils/tests/test_entry_points.py` & `openmdao-3.9.2/openmdao/utils/tests/test_entry_points.py`

 * *Files identical despite different names*

### Comparing `openmdao-3.9.1/openmdao/utils/tests/test_file_wrap.py` & `openmdao-3.9.2/openmdao/utils/tests/test_file_wrap.py`

 * *Files identical despite different names*

### Comparing `openmdao-3.9.1/openmdao/utils/tests/test_find_citations.py` & `openmdao-3.9.2/openmdao/utils/tests/test_find_citations.py`

 * *Files identical despite different names*

### Comparing `openmdao-3.9.1/openmdao/utils/tests/test_general_utils.py` & `openmdao-3.9.2/openmdao/utils/tests/test_general_utils.py`

 * *Files identical despite different names*

### Comparing `openmdao-3.9.1/openmdao/utils/tests/test_hooks.py` & `openmdao-3.9.2/openmdao/utils/tests/test_hooks.py`

 * *Files identical despite different names*

### Comparing `openmdao-3.9.1/openmdao/utils/tests/test_options_dictionary.py` & `openmdao-3.9.2/openmdao/utils/tests/test_options_dictionary.py`

 * *Files identical despite different names*

### Comparing `openmdao-3.9.1/openmdao/utils/tests/test_options_dictionary_feature.py` & `openmdao-3.9.2/openmdao/utils/tests/test_options_dictionary_feature.py`

 * *Files identical despite different names*

### Comparing `openmdao-3.9.1/openmdao/utils/tests/test_scaffold.py` & `openmdao-3.9.2/openmdao/utils/tests/test_scaffold.py`

 * *Files identical despite different names*

### Comparing `openmdao-3.9.1/openmdao/utils/tests/test_shell_proc.py` & `openmdao-3.9.2/openmdao/utils/tests/test_shell_proc.py`

 * *Files identical despite different names*

### Comparing `openmdao-3.9.1/openmdao/utils/tests/test_spline_distributions.py` & `openmdao-3.9.2/openmdao/utils/tests/test_spline_distributions.py`

 * *Files identical despite different names*

### Comparing `openmdao-3.9.1/openmdao/utils/tests/test_units.py` & `openmdao-3.9.2/openmdao/utils/tests/test_units.py`

 * *Files identical despite different names*

### Comparing `openmdao-3.9.1/openmdao/utils/tests/test_vartable.py` & `openmdao-3.9.2/openmdao/utils/tests/test_vartable.py`

 * *Files identical despite different names*

### Comparing `openmdao-3.9.1/openmdao/utils/tests/test_visualization.py` & `openmdao-3.9.2/openmdao/utils/tests/test_visualization.py`

 * *Files identical despite different names*

### Comparing `openmdao-3.9.1/openmdao/utils/unit_library.ini` & `openmdao-3.9.2/openmdao/utils/unit_library.ini`

 * *Files identical despite different names*

### Comparing `openmdao-3.9.1/openmdao/utils/units.py` & `openmdao-3.9.2/openmdao/utils/units.py`

 * *Files identical despite different names*

### Comparing `openmdao-3.9.1/openmdao/utils/variable_table.py` & `openmdao-3.9.2/openmdao/utils/variable_table.py`

 * *Files identical despite different names*

### Comparing `openmdao-3.9.1/openmdao/utils/webview.py` & `openmdao-3.9.2/openmdao/utils/webview.py`

 * *Files identical despite different names*

### Comparing `openmdao-3.9.1/openmdao/vectors/default_transfer.py` & `openmdao-3.9.2/openmdao/vectors/default_transfer.py`

 * *Files identical despite different names*

### Comparing `openmdao-3.9.1/openmdao/vectors/default_vector.py` & `openmdao-3.9.2/openmdao/vectors/default_vector.py`

 * *Files identical despite different names*

### Comparing `openmdao-3.9.1/openmdao/vectors/petsc_transfer.py` & `openmdao-3.9.2/openmdao/vectors/petsc_transfer.py`

 * *Files identical despite different names*

### Comparing `openmdao-3.9.1/openmdao/vectors/petsc_vector.py` & `openmdao-3.9.2/openmdao/vectors/petsc_vector.py`

 * *Files identical despite different names*

### Comparing `openmdao-3.9.1/openmdao/vectors/tests/test_vector.py` & `openmdao-3.9.2/openmdao/vectors/tests/test_vector.py`

 * *Files identical despite different names*

### Comparing `openmdao-3.9.1/openmdao/vectors/transfer.py` & `openmdao-3.9.2/openmdao/vectors/transfer.py`

 * *Files identical despite different names*

### Comparing `openmdao-3.9.1/openmdao/vectors/vector.py` & `openmdao-3.9.2/openmdao/vectors/vector.py`

 * *Files identical despite different names*

### Comparing `openmdao-3.9.1/openmdao/visualization/common/libs/d3.v6.min.js` & `openmdao-3.9.2/openmdao/visualization/common/libs/d3.v6.min.js`

 * *Files identical despite different names*

### Comparing `openmdao-3.9.1/openmdao/visualization/common/libs/jquery-3.4.1.min.js` & `openmdao-3.9.2/openmdao/visualization/common/libs/jquery-3.4.1.min.js`

 * *Files identical despite different names*

### Comparing `openmdao-3.9.1/openmdao/visualization/common/libs/tabulator.min.js` & `openmdao-3.9.2/openmdao/visualization/common/libs/tabulator.min.js`

 * *Files identical despite different names*

### Comparing `openmdao-3.9.1/openmdao/visualization/common/style/tabulator.min.css` & `openmdao-3.9.2/openmdao/visualization/common/style/tabulator.min.css`

 * *Files identical despite different names*

### Comparing `openmdao-3.9.1/openmdao/visualization/connection_viewer/connect_table.html` & `openmdao-3.9.2/openmdao/visualization/connection_viewer/connect_table.html`

 * *Files identical despite different names*

### Comparing `openmdao-3.9.1/openmdao/visualization/connection_viewer/tests/test_viewconns.py` & `openmdao-3.9.2/openmdao/visualization/connection_viewer/tests/test_viewconns.py`

 * *Files identical despite different names*

### Comparing `openmdao-3.9.1/openmdao/visualization/connection_viewer/viewconns.py` & `openmdao-3.9.2/openmdao/visualization/connection_viewer/viewconns.py`

 * *Files identical despite different names*

### Comparing `openmdao-3.9.1/openmdao/visualization/dyn_shape_plot.py` & `openmdao-3.9.2/openmdao/visualization/dyn_shape_plot.py`

 * *Files identical despite different names*

### Comparing `openmdao-3.9.1/openmdao/visualization/html_utils.py` & `openmdao-3.9.2/openmdao/visualization/html_utils.py`

 * *Files identical despite different names*

### Comparing `openmdao-3.9.1/openmdao/visualization/meta_model_viewer/meta_model_visualization.py` & `openmdao-3.9.2/openmdao/visualization/meta_model_viewer/meta_model_visualization.py`

 * *Files identical despite different names*

### Comparing `openmdao-3.9.1/openmdao/visualization/meta_model_viewer/tests/example.py` & `openmdao-3.9.2/openmdao/visualization/meta_model_viewer/tests/example.py`

 * *Files identical despite different names*

### Comparing `openmdao-3.9.1/openmdao/visualization/meta_model_viewer/tests/known_data_point_files/test_five_alpha_points.csv` & `openmdao-3.9.2/openmdao/visualization/meta_model_viewer/tests/known_data_point_files/test_five_alpha_points.csv`

 * *Files identical despite different names*

### Comparing `openmdao-3.9.1/openmdao/visualization/meta_model_viewer/tests/known_data_point_files/unstructured_data_points.csv` & `openmdao-3.9.2/openmdao/visualization/meta_model_viewer/tests/known_data_point_files/unstructured_data_points.csv`

 * *Files identical despite different names*

### Comparing `openmdao-3.9.1/openmdao/visualization/meta_model_viewer/tests/known_data_point_files/unstructured_test_points_bottom.csv` & `openmdao-3.9.2/openmdao/visualization/meta_model_viewer/tests/known_data_point_files/unstructured_test_points_bottom.csv`

 * *Files identical despite different names*

### Comparing `openmdao-3.9.1/openmdao/visualization/meta_model_viewer/tests/known_data_point_files/unstructured_test_points_right.csv` & `openmdao-3.9.2/openmdao/visualization/meta_model_viewer/tests/known_data_point_files/unstructured_test_points_right.csv`

 * *Files identical despite different names*

### Comparing `openmdao-3.9.1/openmdao/visualization/meta_model_viewer/tests/known_data_point_files/updated_scatter_distance.csv` & `openmdao-3.9.2/openmdao/visualization/meta_model_viewer/tests/known_data_point_files/updated_scatter_distance.csv`

 * *Files identical despite different names*

### Comparing `openmdao-3.9.1/openmdao/visualization/meta_model_viewer/tests/multiple_metamodels.py` & `openmdao-3.9.2/openmdao/visualization/meta_model_viewer/tests/multiple_metamodels.py`

 * *Files identical despite different names*

### Comparing `openmdao-3.9.1/openmdao/visualization/meta_model_viewer/tests/test_structured.py` & `openmdao-3.9.2/openmdao/visualization/meta_model_viewer/tests/test_structured.py`

 * *Files identical despite different names*

### Comparing `openmdao-3.9.1/openmdao/visualization/meta_model_viewer/tests/test_unstruct.py` & `openmdao-3.9.2/openmdao/visualization/meta_model_viewer/tests/test_unstruct.py`

 * *Files identical despite different names*

### Comparing `openmdao-3.9.1/openmdao/visualization/meta_model_viewer/tests/test_view_mm_cmd_line.py` & `openmdao-3.9.2/openmdao/visualization/meta_model_viewer/tests/test_view_mm_cmd_line.py`

 * *Files identical despite different names*

### Comparing `openmdao-3.9.1/openmdao/visualization/n2_viewer/assets/logo.png` & `openmdao-3.9.2/openmdao/visualization/n2_viewer/assets/logo.png`

 * *Files identical despite different names*

### Comparing `openmdao-3.9.1/openmdao/visualization/n2_viewer/assets/n2toolbar_screenshot_png.b64` & `openmdao-3.9.2/openmdao/visualization/n2_viewer/assets/n2toolbar_screenshot_png.b64`

 * *Files identical despite different names*

### Comparing `openmdao-3.9.1/openmdao/visualization/n2_viewer/assets/spinner.png` & `openmdao-3.9.2/openmdao/visualization/n2_viewer/assets/spinner.png`

 * *Files identical despite different names*

### Comparing `openmdao-3.9.1/openmdao/visualization/n2_viewer/index.html` & `openmdao-3.9.2/openmdao/visualization/n2_viewer/index.html`

 * *Files identical despite different names*

### Comparing `openmdao-3.9.1/openmdao/visualization/n2_viewer/libs/awesomplete.js` & `openmdao-3.9.2/openmdao/visualization/n2_viewer/libs/awesomplete.js`

 * *Files identical despite different names*

### Comparing `openmdao-3.9.1/openmdao/visualization/n2_viewer/libs/d3.js` & `openmdao-3.9.2/openmdao/visualization/n2_viewer/libs/d3.js`

 * *Files identical despite different names*

### Comparing `openmdao-3.9.1/openmdao/visualization/n2_viewer/libs/d3.v5.min.js` & `openmdao-3.9.2/openmdao/visualization/n2_viewer/libs/d3.v5.min.js`

 * *Files identical despite different names*

### Comparing `openmdao-3.9.1/openmdao/visualization/n2_viewer/libs/json5_2.2.0.min.js` & `openmdao-3.9.2/openmdao/visualization/n2_viewer/libs/json5_2.2.0.min.js`

 * *Files identical despite different names*

### Comparing `openmdao-3.9.1/openmdao/visualization/n2_viewer/libs/pako_inflate.min.js` & `openmdao-3.9.2/openmdao/visualization/n2_viewer/libs/pako_inflate.min.js`

 * *Files identical despite different names*

### Comparing `openmdao-3.9.1/openmdao/visualization/n2_viewer/libs/vkBeautify.js` & `openmdao-3.9.2/openmdao/visualization/n2_viewer/libs/vkBeautify.js`

 * *Files identical despite different names*

### Comparing `openmdao-3.9.1/openmdao/visualization/n2_viewer/n2_viewer.py` & `openmdao-3.9.2/openmdao/visualization/n2_viewer/n2_viewer.py`

 * *Files identical despite different names*

### Comparing `openmdao-3.9.1/openmdao/visualization/n2_viewer/src/ModelData.js` & `openmdao-3.9.2/openmdao/visualization/n2_viewer/src/ModelData.js`

 * *Files identical despite different names*

### Comparing `openmdao-3.9.1/openmdao/visualization/n2_viewer/src/N2Arrow.js` & `openmdao-3.9.2/openmdao/visualization/n2_viewer/src/N2Arrow.js`

 * *Files identical despite different names*

### Comparing `openmdao-3.9.1/openmdao/visualization/n2_viewer/src/N2Diagram.js` & `openmdao-3.9.2/openmdao/visualization/n2_viewer/src/N2Diagram.js`

 * *Files identical despite different names*

### Comparing `openmdao-3.9.1/openmdao/visualization/n2_viewer/src/N2ErrorHandling.js` & `openmdao-3.9.2/openmdao/visualization/n2_viewer/src/N2ErrorHandling.js`

 * *Files identical despite different names*

### Comparing `openmdao-3.9.1/openmdao/visualization/n2_viewer/src/N2Layout.js` & `openmdao-3.9.2/openmdao/visualization/n2_viewer/src/N2Layout.js`

 * *Files identical despite different names*

### Comparing `openmdao-3.9.1/openmdao/visualization/n2_viewer/src/N2Legend.js` & `openmdao-3.9.2/openmdao/visualization/n2_viewer/src/N2Legend.js`

 * *Files identical despite different names*

### Comparing `openmdao-3.9.1/openmdao/visualization/n2_viewer/src/N2Matrix.js` & `openmdao-3.9.2/openmdao/visualization/n2_viewer/src/N2Matrix.js`

 * *Files identical despite different names*

### Comparing `openmdao-3.9.1/openmdao/visualization/n2_viewer/src/N2MatrixCell.js` & `openmdao-3.9.2/openmdao/visualization/n2_viewer/src/N2MatrixCell.js`

 * *Files identical despite different names*

### Comparing `openmdao-3.9.1/openmdao/visualization/n2_viewer/src/N2Search.js` & `openmdao-3.9.2/openmdao/visualization/n2_viewer/src/N2Search.js`

 * *Files identical despite different names*

### Comparing `openmdao-3.9.1/openmdao/visualization/n2_viewer/src/N2Style.js` & `openmdao-3.9.2/openmdao/visualization/n2_viewer/src/N2Style.js`

 * *Files identical despite different names*

### Comparing `openmdao-3.9.1/openmdao/visualization/n2_viewer/src/N2Toolbar.js` & `openmdao-3.9.2/openmdao/visualization/n2_viewer/src/N2Toolbar.js`

 * *Files identical despite different names*

### Comparing `openmdao-3.9.1/openmdao/visualization/n2_viewer/src/N2TreeNode.js` & `openmdao-3.9.2/openmdao/visualization/n2_viewer/src/N2TreeNode.js`

 * *Files identical despite different names*

### Comparing `openmdao-3.9.1/openmdao/visualization/n2_viewer/src/N2UserInterface.js` & `openmdao-3.9.2/openmdao/visualization/n2_viewer/src/N2UserInterface.js`

 * *Files identical despite different names*

### Comparing `openmdao-3.9.1/openmdao/visualization/n2_viewer/src/N2Window.js` & `openmdao-3.9.2/openmdao/visualization/n2_viewer/src/N2Window.js`

 * *Files identical despite different names*

### Comparing `openmdao-3.9.1/openmdao/visualization/n2_viewer/src/NodeInfo.js` & `openmdao-3.9.2/openmdao/visualization/n2_viewer/src/NodeInfo.js`

 * *Files identical despite different names*

### Comparing `openmdao-3.9.1/openmdao/visualization/n2_viewer/src/SymbolType.js` & `openmdao-3.9.2/openmdao/visualization/n2_viewer/src/SymbolType.js`

 * *Files identical despite different names*

### Comparing `openmdao-3.9.1/openmdao/visualization/n2_viewer/src/defaults.js` & `openmdao-3.9.2/openmdao/visualization/n2_viewer/src/defaults.js`

 * *Files identical despite different names*

### Comparing `openmdao-3.9.1/openmdao/visualization/n2_viewer/src/utils.js` & `openmdao-3.9.2/openmdao/visualization/n2_viewer/src/utils.js`

 * *Files identical despite different names*

### Comparing `openmdao-3.9.1/openmdao/visualization/n2_viewer/style/awesomplete.css` & `openmdao-3.9.2/openmdao/visualization/n2_viewer/style/awesomplete.css`

 * *Files identical despite different names*

### Comparing `openmdao-3.9.1/openmdao/visualization/n2_viewer/style/legend.css` & `openmdao-3.9.2/openmdao/visualization/n2_viewer/style/legend.css`

 * *Files identical despite different names*

### Comparing `openmdao-3.9.1/openmdao/visualization/n2_viewer/style/logo_png.b64` & `openmdao-3.9.2/openmdao/visualization/n2_viewer/style/logo_png.b64`

 * *Files identical despite different names*

### Comparing `openmdao-3.9.1/openmdao/visualization/n2_viewer/style/n2toolbar-icons-font.woff` & `openmdao-3.9.2/openmdao/visualization/n2_viewer/style/n2toolbar-icons-font.woff`

 * *Files identical despite different names*

### Comparing `openmdao-3.9.1/openmdao/visualization/n2_viewer/style/n2toolbar-icons.css` & `openmdao-3.9.2/openmdao/visualization/n2_viewer/style/n2toolbar-icons.css`

 * *Files identical despite different names*

### Comparing `openmdao-3.9.1/openmdao/visualization/n2_viewer/style/partition_tree.css` & `openmdao-3.9.2/openmdao/visualization/n2_viewer/style/partition_tree.css`

 * *Files identical despite different names*

### Comparing `openmdao-3.9.1/openmdao/visualization/n2_viewer/style/toolbar.css` & `openmdao-3.9.2/openmdao/visualization/n2_viewer/style/toolbar.css`

 * *Files identical despite different names*

### Comparing `openmdao-3.9.1/openmdao/visualization/n2_viewer/style/window.css` & `openmdao-3.9.2/openmdao/visualization/n2_viewer/style/window.css`

 * *Files identical despite different names*

### Comparing `openmdao-3.9.1/openmdao/visualization/n2_viewer/tests/betz_tree.json` & `openmdao-3.9.2/openmdao/visualization/n2_viewer/tests/betz_tree.json`

 * *Files identical despite different names*

### Comparing `openmdao-3.9.1/openmdao/visualization/n2_viewer/tests/gui_test_models/bug_arrow.py` & `openmdao-3.9.2/openmdao/visualization/n2_viewer/tests/gui_test_models/bug_arrow.py`

 * *Files identical despite different names*

### Comparing `openmdao-3.9.1/openmdao/visualization/n2_viewer/tests/gui_test_models/circuit.py` & `openmdao-3.9.2/openmdao/visualization/n2_viewer/tests/gui_test_models/circuit.py`

 * *Files identical despite different names*

### Comparing `openmdao-3.9.1/openmdao/visualization/n2_viewer/tests/gui_test_models/double_sellar.py` & `openmdao-3.9.2/openmdao/visualization/n2_viewer/tests/gui_test_models/double_sellar.py`

 * *Files identical despite different names*

### Comparing `openmdao-3.9.1/openmdao/visualization/n2_viewer/tests/gui_test_models/nan_value.py` & `openmdao-3.9.2/openmdao/visualization/n2_viewer/tests/gui_test_models/nan_value.py`

 * *Files identical despite different names*

### Comparing `openmdao-3.9.1/openmdao/visualization/n2_viewer/tests/gui_test_models/parabaloid.py` & `openmdao-3.9.2/openmdao/visualization/n2_viewer/tests/gui_test_models/parabaloid.py`

 * *Files identical despite different names*

### Comparing `openmdao-3.9.1/openmdao/visualization/n2_viewer/tests/gui_test_models/valuewin2.py` & `openmdao-3.9.2/openmdao/visualization/n2_viewer/tests/gui_test_models/valuewin2.py`

 * *Files identical despite different names*

### Comparing `openmdao-3.9.1/openmdao/visualization/n2_viewer/tests/n2_gui_test.py` & `openmdao-3.9.2/openmdao/visualization/n2_viewer/tests/n2_gui_test.py`

 * *Files identical despite different names*

### Comparing `openmdao-3.9.1/openmdao/visualization/n2_viewer/tests/sellar_tree.json` & `openmdao-3.9.2/openmdao/visualization/n2_viewer/tests/sellar_tree.json`

 * *Files identical despite different names*

### Comparing `openmdao-3.9.1/openmdao/visualization/n2_viewer/tests/test_gui.py` & `openmdao-3.9.2/openmdao/visualization/n2_viewer/tests/test_gui.py`

 * *Files identical despite different names*

### Comparing `openmdao-3.9.1/openmdao/visualization/n2_viewer/tests/test_n2_viewer.py` & `openmdao-3.9.2/openmdao/visualization/n2_viewer/tests/test_n2_viewer.py`

 * *Files identical despite different names*

### Comparing `openmdao-3.9.1/openmdao/visualization/n2_viewer/tests/test_parallel_n2.py` & `openmdao-3.9.2/openmdao/visualization/n2_viewer/tests/test_parallel_n2.py`

 * *Files identical despite different names*

### Comparing `openmdao-3.9.1/openmdao/visualization/n2_viewer/tests/test_serialization.py` & `openmdao-3.9.2/openmdao/visualization/n2_viewer/tests/test_serialization.py`

 * *Files identical despite different names*

### Comparing `openmdao-3.9.1/openmdao/visualization/n2_viewer/tests/test_viewmodeldata.py` & `openmdao-3.9.2/openmdao/visualization/n2_viewer/tests/test_viewmodeldata.py`

 * *Files identical despite different names*

### Comparing `openmdao-3.9.1/openmdao/visualization/partial_deriv_plot.py` & `openmdao-3.9.2/openmdao/visualization/partial_deriv_plot.py`

 * *Files identical despite different names*

### Comparing `openmdao-3.9.1/openmdao/visualization/scaling_viewer/scaling_report.py` & `openmdao-3.9.2/openmdao/visualization/scaling_viewer/scaling_report.py`

 * *Files identical despite different names*

### Comparing `openmdao-3.9.1/openmdao/visualization/scaling_viewer/scaling_table.html` & `openmdao-3.9.2/openmdao/visualization/scaling_viewer/scaling_table.html`

 * *Files identical despite different names*

### Comparing `openmdao-3.9.1/openmdao/warnings.py` & `openmdao-3.9.2/openmdao/warnings.py`

 * *Files identical despite different names*

### Comparing `openmdao-3.9.1/openmdao.egg-info/PKG-INFO` & `openmdao-3.9.2/openmdao.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: openmdao
-Version: 3.9.1
+Version: 3.9.2
 Summary: OpenMDAO framework infrastructure
 Home-page: http://openmdao.org
 Author: OpenMDAO Team
 Author-email: openmdao@openmdao.org
 License: Apache License, Version 2.0
 Description: OpenMDAO is an open-source high-performance computing platform
             for systems analysis and multidisciplinary optimization, written in Python. It
```

### Comparing `openmdao-3.9.1/openmdao.egg-info/SOURCES.txt` & `openmdao-3.9.2/openmdao.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `openmdao-3.9.1/openmdao.egg-info/entry_points.txt` & `openmdao-3.9.2/openmdao.egg-info/entry_points.txt`

 * *Files identical despite different names*

### Comparing `openmdao-3.9.1/openmdao.egg-info/requires.txt` & `openmdao-3.9.2/openmdao.egg-info/requires.txt`

 * *Files 3% similar despite different names*

```diff
@@ -16,24 +16,24 @@
 numpydoc>=0.9.1
 numpydoc>=0.9.1
 parameterized
 pycodestyle>=2.4.0
 pydocstyle==2.0.0
 pyppeteer
 redbaron
-sphinx>=1.8.5
+sphinx<4.0,>=1.8.5
 tabulate
 tabulate
 testflo>=1.3.6websockets>8
 
 [docs]
 matplotlib
 numpydoc>=0.9.1
 redbaron
-sphinx>=1.8.5
+sphinx<4.0,>=1.8.5
 tabulate
 ipython
 
 [notebooks]
 notebook
 tabulate
 ipython
```

### Comparing `openmdao-3.9.1/setup.py` & `openmdao-3.9.2/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 )[0]
 
 optional_dependencies = {
     'docs': [
         'matplotlib',
         'numpydoc>=0.9.1',
         'redbaron',
-        'sphinx>=1.8.5',
+        'sphinx>=1.8.5,<4.0',
         'tabulate',
         'ipython'
     ],
     'notebooks': [
         'notebook',
         'tabulate',
         'ipython'
```

