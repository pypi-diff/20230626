# Comparing `tmp/cyanure-1.0.0.tar.gz` & `tmp/cyanure-1.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cyanure-1.0.0.tar", last modified: Thu Apr 21 09:28:32 2022, max compression
+gzip compressed data, was "cyanure-1.1.0.tar", last modified: Mon Jun 26 14:50:12 2023, max compression
```

## Comparing `cyanure-1.0.0.tar` & `cyanure-1.1.0.tar`

### file list

```diff
@@ -1,75 +1,77 @@
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-04-21 09:28:32.464495 cyanure-1.0.0/
--rw-r--r--   0 runner    (1001) docker     (121)      267 2022-04-21 09:28:32.464495 cyanure-1.0.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)        5 2022-04-21 09:28:24.080382 cyanure-1.0.0/VERSION
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-04-21 09:28:32.464495 cyanure-1.0.0/cyanure/
--rw-r--r--   0 runner    (1001) docker     (121)       61 2022-04-21 09:28:24.080382 cyanure-1.0.0/cyanure/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)    11389 2022-04-21 09:28:24.080382 cyanure-1.0.0/cyanure/data_processing.py
--rw-r--r--   0 runner    (1001) docker     (121)    48636 2022-04-21 09:28:24.080382 cyanure-1.0.0/cyanure/estimators.py
--rw-r--r--   0 runner    (1001) docker     (121)      728 2022-04-21 09:28:24.080382 cyanure-1.0.0/cyanure/logger.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-04-21 09:28:32.464495 cyanure-1.0.0/cyanure_lib/
--rw-r--r--   0 runner    (1001) docker     (121)       77 2022-04-21 09:28:24.080382 cyanure-1.0.0/cyanure_lib/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)    13152 2022-04-21 09:28:24.080382 cyanure-1.0.0/cyanure_lib/cyanure_wrap_module.cpp
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-04-21 09:28:32.464495 cyanure-1.0.0/cyanure_lib/lib/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-04-21 09:28:32.464495 cyanure-1.0.0/cyanure_lib/lib/BLAS/
--rw-r--r--   0 runner    (1001) docker     (121)    49988 2022-04-21 09:28:24.080382 cyanure-1.0.0/cyanure_lib/lib/BLAS/cblas_alt_template.h
--rw-r--r--   0 runner    (1001) docker     (121)     1291 2022-04-21 09:28:24.080382 cyanure-1.0.0/cyanure_lib/lib/BLAS/cblas_defvar.h
--rw-r--r--   0 runner    (1001) docker     (121)      778 2022-04-21 09:28:24.080382 cyanure-1.0.0/cyanure_lib/lib/BLAS/configure_blas.h
--rw-r--r--   0 runner    (1001) docker     (121)     3340 2022-04-21 09:28:24.080382 cyanure-1.0.0/cyanure_lib/lib/basic_math_template.h
--rw-r--r--   0 runner    (1001) docker     (121)     7707 2022-04-21 09:28:24.080382 cyanure-1.0.0/cyanure_lib/lib/convert_cxx_to_python.h
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-04-21 09:28:32.464495 cyanure-1.0.0/cyanure_lib/lib/data_structure/
--rw-r--r--   0 runner    (1001) docker     (121)     7860 2022-04-21 09:28:24.080382 cyanure-1.0.0/cyanure_lib/lib/data_structure/data.h
--rw-r--r--   0 runner    (1001) docker     (121)      582 2022-04-21 09:28:24.080382 cyanure-1.0.0/cyanure_lib/lib/data_structure/declare_structures.h
--rw-r--r--   0 runner    (1001) docker     (121)     3474 2022-04-21 09:28:24.080382 cyanure-1.0.0/cyanure_lib/lib/data_structure/linalg.h
--rw-r--r--   0 runner    (1001) docker     (121)     4662 2022-04-21 09:28:24.080382 cyanure-1.0.0/cyanure_lib/lib/data_structure/list.h
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-04-21 09:28:32.464495 cyanure-1.0.0/cyanure_lib/lib/data_structure/structures/
--rw-r--r--   0 runner    (1001) docker     (121)    77159 2022-04-21 09:28:24.080382 cyanure-1.0.0/cyanure_lib/lib/data_structure/structures/matrix.h
--rw-r--r--   0 runner    (1001) docker     (121)     7181 2022-04-21 09:28:24.080382 cyanure-1.0.0/cyanure_lib/lib/data_structure/structures/optim_info.h
--rw-r--r--   0 runner    (1001) docker     (121)    31550 2022-04-21 09:28:24.080382 cyanure-1.0.0/cyanure_lib/lib/data_structure/structures/sp_matrix.h
--rw-r--r--   0 runner    (1001) docker     (121)     8274 2022-04-21 09:28:24.080382 cyanure-1.0.0/cyanure_lib/lib/data_structure/structures/sp_vector.h
--rw-r--r--   0 runner    (1001) docker     (121)    60918 2022-04-21 09:28:24.080382 cyanure-1.0.0/cyanure_lib/lib/data_structure/structures/vector.h
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-04-21 09:28:32.464495 cyanure-1.0.0/cyanure_lib/lib/erm/
--rw-r--r--   0 runner    (1001) docker     (121)     1599 2022-04-21 09:28:24.080382 cyanure-1.0.0/cyanure_lib/lib/erm/erm.h
--rw-r--r--   0 runner    (1001) docker     (121)    15181 2022-04-21 09:28:24.080382 cyanure-1.0.0/cyanure_lib/lib/erm/multi_erm.h
--rw-r--r--   0 runner    (1001) docker     (121)     9980 2022-04-21 09:28:24.080382 cyanure-1.0.0/cyanure_lib/lib/erm/simple_erm.h
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-04-21 09:28:32.464495 cyanure-1.0.0/cyanure_lib/lib/error_management/
--rw-r--r--   0 runner    (1001) docker     (121)     1347 2022-04-21 09:28:24.080382 cyanure-1.0.0/cyanure_lib/lib/error_management/exception.h
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-04-21 09:28:32.464495 cyanure-1.0.0/cyanure_lib/lib/logging/
--rw-r--r--   0 runner    (1001) docker     (121)     1954 2022-04-21 09:28:24.080382 cyanure-1.0.0/cyanure_lib/lib/logging/logger.h
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-04-21 09:28:32.464495 cyanure-1.0.0/cyanure_lib/lib/losses/
--rw-r--r--   0 runner    (1001) docker     (121)     8950 2022-04-21 09:28:24.080382 cyanure-1.0.0/cyanure_lib/lib/losses/loss.h
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-04-21 09:28:32.464495 cyanure-1.0.0/cyanure_lib/lib/losses/loss_mat/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-04-21 09:28:32.464495 cyanure-1.0.0/cyanure_lib/lib/losses/loss_mat/loss/
--rw-r--r--   0 runner    (1001) docker     (121)     3054 2022-04-21 09:28:24.080382 cyanure-1.0.0/cyanure_lib/lib/losses/loss_mat/loss/multi_logistic_loss.h
--rw-r--r--   0 runner    (1001) docker     (121)     1724 2022-04-21 09:28:24.080382 cyanure-1.0.0/cyanure_lib/lib/losses/loss_mat/loss/square_loss.h
--rw-r--r--   0 runner    (1001) docker     (121)     7606 2022-04-21 09:28:24.080382 cyanure-1.0.0/cyanure_lib/lib/losses/loss_mat/loss_mat.h
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-04-21 09:28:32.464495 cyanure-1.0.0/cyanure_lib/lib/losses/loss_vec/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-04-21 09:28:32.464495 cyanure-1.0.0/cyanure_lib/lib/losses/loss_vec/loss/
--rw-r--r--   0 runner    (1001) docker     (121)     1785 2022-04-21 09:28:24.080382 cyanure-1.0.0/cyanure_lib/lib/losses/loss_vec/loss/hinge_loss.h
--rw-r--r--   0 runner    (1001) docker     (121)     1876 2022-04-21 09:28:24.080382 cyanure-1.0.0/cyanure_lib/lib/losses/loss_vec/loss/logistic_loss.h
--rw-r--r--   0 runner    (1001) docker     (121)     2112 2022-04-21 09:28:24.080382 cyanure-1.0.0/cyanure_lib/lib/losses/loss_vec/loss/safe_logistic_loss.h
--rw-r--r--   0 runner    (1001) docker     (121)     2479 2022-04-21 09:28:24.080382 cyanure-1.0.0/cyanure_lib/lib/losses/loss_vec/loss/square_hinge_loss.h
--rw-r--r--   0 runner    (1001) docker     (121)     1475 2022-04-21 09:28:24.080382 cyanure-1.0.0/cyanure_lib/lib/losses/loss_vec/loss/square_loss.h
--rw-r--r--   0 runner    (1001) docker     (121)     1564 2022-04-21 09:28:24.080382 cyanure-1.0.0/cyanure_lib/lib/losses/loss_vec/loss_vec.h
--rw-r--r--   0 runner    (1001) docker     (121)     1091 2022-04-21 09:28:24.080382 cyanure-1.0.0/cyanure_lib/lib/macro.h
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-04-21 09:28:32.464495 cyanure-1.0.0/cyanure_lib/lib/regul/
--rw-r--r--   0 runner    (1001) docker     (121)     5851 2022-04-21 09:28:24.080382 cyanure-1.0.0/cyanure_lib/lib/regul/compute_regularization.h
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-04-21 09:28:32.464495 cyanure-1.0.0/cyanure_lib/lib/regul/mixed_l1_norm/
--rw-r--r--   0 runner    (1001) docker     (121)     5205 2022-04-21 09:28:24.080382 cyanure-1.0.0/cyanure_lib/lib/regul/mixed_l1_norm/mixed_l1_norm.h
--rw-r--r--   0 runner    (1001) docker     (121)     3256 2022-04-21 09:28:24.080382 cyanure-1.0.0/cyanure_lib/lib/regul/mixed_l1_norm/norms.h
--rw-r--r--   0 runner    (1001) docker     (121)     3118 2022-04-21 09:28:24.080382 cyanure-1.0.0/cyanure_lib/lib/regul/regularizer.h
--rw-r--r--   0 runner    (1001) docker     (121)    10952 2022-04-21 09:28:24.080382 cyanure-1.0.0/cyanure_lib/lib/regul/regularizers.h
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-04-21 09:28:32.464495 cyanure-1.0.0/cyanure_lib/lib/solvers/
--rw-r--r--   0 runner    (1001) docker     (121)     9337 2022-04-21 09:28:24.080382 cyanure-1.0.0/cyanure_lib/lib/solvers/accelerator.h
--rw-r--r--   0 runner    (1001) docker     (121)     5282 2022-04-21 09:28:24.080382 cyanure-1.0.0/cyanure_lib/lib/solvers/incremental_solver.h
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-04-21 09:28:32.464495 cyanure-1.0.0/cyanure_lib/lib/solvers/incremental_solvers/
--rw-r--r--   0 runner    (1001) docker     (121)     6550 2022-04-21 09:28:24.080382 cyanure-1.0.0/cyanure_lib/lib/solvers/incremental_solvers/miso.h
--rw-r--r--   0 runner    (1001) docker     (121)    14696 2022-04-21 09:28:24.080382 cyanure-1.0.0/cyanure_lib/lib/solvers/incremental_solvers/svrg.h
--rw-r--r--   0 runner    (1001) docker     (121)     2792 2022-04-21 09:28:24.080382 cyanure-1.0.0/cyanure_lib/lib/solvers/ista.h
--rw-r--r--   0 runner    (1001) docker     (121)     8199 2022-04-21 09:28:24.080382 cyanure-1.0.0/cyanure_lib/lib/solvers/solver.h
--rw-r--r--   0 runner    (1001) docker     (121)     3127 2022-04-21 09:28:24.080382 cyanure-1.0.0/cyanure_lib/lib/sorting_algorithms.h
--rw-r--r--   0 runner    (1001) docker     (121)     3523 2022-04-21 09:28:24.080382 cyanure-1.0.0/cyanure_lib/lib/timer.h
--rw-r--r--   0 runner    (1001) docker     (121)     4436 2022-04-21 09:28:24.136383 cyanure-1.0.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-04-21 09:28:32.464495 cyanure-1.0.0/test/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-04-21 09:28:24.136383 cyanure-1.0.0/test/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)      391 2022-04-21 09:28:24.136383 cyanure-1.0.0/test/test_estimator.py
--rw-r--r--   0 runner    (1001) docker     (121)    36420 2022-04-21 09:28:24.136383 cyanure-1.0.0/test/test_logistic_regression.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 14:50:12.243794 cyanure-1.1.0/
+-rw-r--r--   0 runner    (1001) docker     (123)     1511 2023-06-26 14:50:05.787707 cyanure-1.1.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      839 2023-06-26 14:50:12.243794 cyanure-1.1.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)        5 2023-06-26 14:50:05.787707 cyanure-1.1.0/VERSION
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 14:50:12.243794 cyanure-1.1.0/cyanure/
+-rw-r--r--   0 runner    (1001) docker     (123)       61 2023-06-26 14:50:05.787707 cyanure-1.1.0/cyanure/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19789 2023-06-26 14:50:05.787707 cyanure-1.1.0/cyanure/data_processing.py
+-rw-r--r--   0 runner    (1001) docker     (123)    50655 2023-06-26 14:50:05.787707 cyanure-1.1.0/cyanure/estimators.py
+-rw-r--r--   0 runner    (1001) docker     (123)      728 2023-06-26 14:50:05.787707 cyanure-1.1.0/cyanure/logger.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 14:50:12.243794 cyanure-1.1.0/cyanure_lib/
+-rw-r--r--   0 runner    (1001) docker     (123)       77 2023-06-26 14:50:05.787707 cyanure-1.1.0/cyanure_lib/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13379 2023-06-26 14:50:05.787707 cyanure-1.1.0/cyanure_lib/cyanure_wrap_module.cpp
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 14:50:12.243794 cyanure-1.1.0/cyanure_lib/lib/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 14:50:12.243794 cyanure-1.1.0/cyanure_lib/lib/BLAS/
+-rw-r--r--   0 runner    (1001) docker     (123)    50010 2023-06-26 14:50:05.787707 cyanure-1.1.0/cyanure_lib/lib/BLAS/cblas_alt_template.h
+-rw-r--r--   0 runner    (1001) docker     (123)     1291 2023-06-26 14:50:05.787707 cyanure-1.1.0/cyanure_lib/lib/BLAS/cblas_defvar.h
+-rw-r--r--   0 runner    (1001) docker     (123)      976 2023-06-26 14:50:05.787707 cyanure-1.1.0/cyanure_lib/lib/BLAS/configure_blas.h
+-rw-r--r--   0 runner    (1001) docker     (123)     3340 2023-06-26 14:50:05.787707 cyanure-1.1.0/cyanure_lib/lib/basic_math_template.h
+-rw-r--r--   0 runner    (1001) docker     (123)     7707 2023-06-26 14:50:05.787707 cyanure-1.1.0/cyanure_lib/lib/convert_cxx_to_python.h
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 14:50:12.243794 cyanure-1.1.0/cyanure_lib/lib/data_structure/
+-rw-r--r--   0 runner    (1001) docker     (123)     7860 2023-06-26 14:50:05.787707 cyanure-1.1.0/cyanure_lib/lib/data_structure/data.h
+-rw-r--r--   0 runner    (1001) docker     (123)      582 2023-06-26 14:50:05.787707 cyanure-1.1.0/cyanure_lib/lib/data_structure/declare_structures.h
+-rw-r--r--   0 runner    (1001) docker     (123)     3474 2023-06-26 14:50:05.787707 cyanure-1.1.0/cyanure_lib/lib/data_structure/linalg.h
+-rw-r--r--   0 runner    (1001) docker     (123)     4662 2023-06-26 14:50:05.787707 cyanure-1.1.0/cyanure_lib/lib/data_structure/list.h
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 14:50:12.243794 cyanure-1.1.0/cyanure_lib/lib/data_structure/structures/
+-rw-r--r--   0 runner    (1001) docker     (123)    77159 2023-06-26 14:50:05.787707 cyanure-1.1.0/cyanure_lib/lib/data_structure/structures/matrix.h
+-rw-r--r--   0 runner    (1001) docker     (123)     7181 2023-06-26 14:50:05.787707 cyanure-1.1.0/cyanure_lib/lib/data_structure/structures/optim_info.h
+-rw-r--r--   0 runner    (1001) docker     (123)    30955 2023-06-26 14:50:05.787707 cyanure-1.1.0/cyanure_lib/lib/data_structure/structures/sp_matrix.h
+-rw-r--r--   0 runner    (1001) docker     (123)     8274 2023-06-26 14:50:05.791707 cyanure-1.1.0/cyanure_lib/lib/data_structure/structures/sp_vector.h
+-rw-r--r--   0 runner    (1001) docker     (123)    60844 2023-06-26 14:50:05.791707 cyanure-1.1.0/cyanure_lib/lib/data_structure/structures/vector.h
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 14:50:12.243794 cyanure-1.1.0/cyanure_lib/lib/erm/
+-rw-r--r--   0 runner    (1001) docker     (123)     1599 2023-06-26 14:50:05.791707 cyanure-1.1.0/cyanure_lib/lib/erm/erm.h
+-rw-r--r--   0 runner    (1001) docker     (123)    15179 2023-06-26 14:50:05.791707 cyanure-1.1.0/cyanure_lib/lib/erm/multi_erm.h
+-rw-r--r--   0 runner    (1001) docker     (123)     9980 2023-06-26 14:50:05.791707 cyanure-1.1.0/cyanure_lib/lib/erm/simple_erm.h
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 14:50:12.243794 cyanure-1.1.0/cyanure_lib/lib/error_management/
+-rw-r--r--   0 runner    (1001) docker     (123)     1347 2023-06-26 14:50:05.791707 cyanure-1.1.0/cyanure_lib/lib/error_management/exception.h
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 14:50:12.243794 cyanure-1.1.0/cyanure_lib/lib/logging/
+-rw-r--r--   0 runner    (1001) docker     (123)     1954 2023-06-26 14:50:05.791707 cyanure-1.1.0/cyanure_lib/lib/logging/logger.h
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 14:50:12.243794 cyanure-1.1.0/cyanure_lib/lib/losses/
+-rw-r--r--   0 runner    (1001) docker     (123)     8950 2023-06-26 14:50:05.791707 cyanure-1.1.0/cyanure_lib/lib/losses/loss.h
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 14:50:12.243794 cyanure-1.1.0/cyanure_lib/lib/losses/loss_mat/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 14:50:12.243794 cyanure-1.1.0/cyanure_lib/lib/losses/loss_mat/loss/
+-rw-r--r--   0 runner    (1001) docker     (123)     3093 2023-06-26 14:50:05.791707 cyanure-1.1.0/cyanure_lib/lib/losses/loss_mat/loss/multi_logistic_loss.h
+-rw-r--r--   0 runner    (1001) docker     (123)     1724 2023-06-26 14:50:05.791707 cyanure-1.1.0/cyanure_lib/lib/losses/loss_mat/loss/square_loss.h
+-rw-r--r--   0 runner    (1001) docker     (123)     7626 2023-06-26 14:50:05.791707 cyanure-1.1.0/cyanure_lib/lib/losses/loss_mat/loss_mat.h
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 14:50:12.243794 cyanure-1.1.0/cyanure_lib/lib/losses/loss_vec/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 14:50:12.243794 cyanure-1.1.0/cyanure_lib/lib/losses/loss_vec/loss/
+-rw-r--r--   0 runner    (1001) docker     (123)     1785 2023-06-26 14:50:05.791707 cyanure-1.1.0/cyanure_lib/lib/losses/loss_vec/loss/hinge_loss.h
+-rw-r--r--   0 runner    (1001) docker     (123)     1876 2023-06-26 14:50:05.791707 cyanure-1.1.0/cyanure_lib/lib/losses/loss_vec/loss/logistic_loss.h
+-rw-r--r--   0 runner    (1001) docker     (123)     2112 2023-06-26 14:50:05.791707 cyanure-1.1.0/cyanure_lib/lib/losses/loss_vec/loss/safe_logistic_loss.h
+-rw-r--r--   0 runner    (1001) docker     (123)     2479 2023-06-26 14:50:05.791707 cyanure-1.1.0/cyanure_lib/lib/losses/loss_vec/loss/square_hinge_loss.h
+-rw-r--r--   0 runner    (1001) docker     (123)     1475 2023-06-26 14:50:05.791707 cyanure-1.1.0/cyanure_lib/lib/losses/loss_vec/loss/square_loss.h
+-rw-r--r--   0 runner    (1001) docker     (123)     1564 2023-06-26 14:50:05.791707 cyanure-1.1.0/cyanure_lib/lib/losses/loss_vec/loss_vec.h
+-rw-r--r--   0 runner    (1001) docker     (123)     1091 2023-06-26 14:50:05.791707 cyanure-1.1.0/cyanure_lib/lib/macro.h
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 14:50:12.243794 cyanure-1.1.0/cyanure_lib/lib/regul/
+-rw-r--r--   0 runner    (1001) docker     (123)     5851 2023-06-26 14:50:05.791707 cyanure-1.1.0/cyanure_lib/lib/regul/compute_regularization.h
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 14:50:12.243794 cyanure-1.1.0/cyanure_lib/lib/regul/mixed_l1_norm/
+-rw-r--r--   0 runner    (1001) docker     (123)     5205 2023-06-26 14:50:05.791707 cyanure-1.1.0/cyanure_lib/lib/regul/mixed_l1_norm/mixed_l1_norm.h
+-rw-r--r--   0 runner    (1001) docker     (123)     3256 2023-06-26 14:50:05.791707 cyanure-1.1.0/cyanure_lib/lib/regul/mixed_l1_norm/norms.h
+-rw-r--r--   0 runner    (1001) docker     (123)     3118 2023-06-26 14:50:05.791707 cyanure-1.1.0/cyanure_lib/lib/regul/regularizer.h
+-rw-r--r--   0 runner    (1001) docker     (123)    10892 2023-06-26 14:50:05.791707 cyanure-1.1.0/cyanure_lib/lib/regul/regularizers.h
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 14:50:12.243794 cyanure-1.1.0/cyanure_lib/lib/solvers/
+-rw-r--r--   0 runner    (1001) docker     (123)     9337 2023-06-26 14:50:05.791707 cyanure-1.1.0/cyanure_lib/lib/solvers/accelerator.h
+-rw-r--r--   0 runner    (1001) docker     (123)     5311 2023-06-26 14:50:05.791707 cyanure-1.1.0/cyanure_lib/lib/solvers/incremental_solver.h
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 14:50:12.243794 cyanure-1.1.0/cyanure_lib/lib/solvers/incremental_solvers/
+-rw-r--r--   0 runner    (1001) docker     (123)     6578 2023-06-26 14:50:05.791707 cyanure-1.1.0/cyanure_lib/lib/solvers/incremental_solvers/miso.h
+-rw-r--r--   0 runner    (1001) docker     (123)    14753 2023-06-26 14:50:05.791707 cyanure-1.1.0/cyanure_lib/lib/solvers/incremental_solvers/svrg.h
+-rw-r--r--   0 runner    (1001) docker     (123)     2792 2023-06-26 14:50:05.791707 cyanure-1.1.0/cyanure_lib/lib/solvers/ista.h
+-rw-r--r--   0 runner    (1001) docker     (123)     8316 2023-06-26 14:50:05.791707 cyanure-1.1.0/cyanure_lib/lib/solvers/solver.h
+-rw-r--r--   0 runner    (1001) docker     (123)     3127 2023-06-26 14:50:05.791707 cyanure-1.1.0/cyanure_lib/lib/sorting_algorithms.h
+-rw-r--r--   0 runner    (1001) docker     (123)     3523 2023-06-26 14:50:05.791707 cyanure-1.1.0/cyanure_lib/lib/timer.h
+-rw-r--r--   0 runner    (1001) docker     (123)     6345 2023-06-26 14:50:06.475716 cyanure-1.1.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 14:50:12.243794 cyanure-1.1.0/test/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-26 14:50:06.475716 cyanure-1.1.0/test/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4815 2023-06-26 14:50:06.475716 cyanure-1.1.0/test/test_active_set.py
+-rw-r--r--   0 runner    (1001) docker     (123)      469 2023-06-26 14:50:06.475716 cyanure-1.1.0/test/test_estimator.py
+-rw-r--r--   0 runner    (1001) docker     (123)    36545 2023-06-26 14:50:06.475716 cyanure-1.1.0/test/test_logistic_regression.py
```

### Comparing `cyanure-1.0.0/cyanure/estimators.py` & `cyanure-1.1.0/cyanure/estimators.py`

 * *Files 4% similar despite different names*

```diff
@@ -4,25 +4,27 @@
 
 import math
 import inspect
 import warnings
 import platform
 from collections import defaultdict
 
+import concurrent.futures
+
 import numpy as np
 import scipy.sparse
 
 from sklearn.base import BaseEstimator
 from sklearn.utils.validation import check_is_fitted
 from sklearn.utils.extmath import safe_sparse_dot, softmax
 from sklearn.exceptions import ConvergenceWarning
 
 import cyanure_lib
 
-from cyanure.data_processing import check_input_fit, check_input_inference
+from cyanure.data_processing import check_input_fit, check_input_inference, windows_conversion
 
 from cyanure.logger import setup_custom_logger
 
 logger = setup_custom_logger("INFO")
 
 
 class ERM(BaseEstimator, ABC):
@@ -72,30 +74,30 @@
             initial_weight = np.zeros((p), dtype=X.dtype)
             yf = np.squeeze(labels.astype(X.dtype))
         else:
             if labels.squeeze().ndim > 1:
                 nclasses = labels.squeeze().shape[1]
                 yf = np.asfortranarray(labels.T)
             else:
-                nclasses = int(np.max(labels) + 1)
+                nclasses = len(np.unique(labels))
                 if platform.system() == "Windows":
                     yf = np.squeeze(np.intc(np.float64(labels)))
                 else:
                     yf = np.squeeze(np.int32(labels))
             initial_weight = np.zeros(
                 [p, nclasses], dtype=X.dtype, order='F')
 
         initial_weight = self._warm_start(X, initial_weight, nclasses)
 
         return initial_weight, yf, nclasses
 
     def __init__(self, loss='square', penalty='l2', fit_intercept=False, dual=None, tol=1e-3,
                  solver="auto", random_state=0, max_iter=2000, fista_restart=60,
                  verbose=True, warm_start=False, limited_memory_qning=50, multi_class="auto",
-                 lambda_1=0, lambda_2=0, lambda_3=0, duality_gap_interval=5, n_threads=-1):
+                 lambda_1=0, lambda_2=0, lambda_3=0, duality_gap_interval=5, n_threads=-1, safe=True):
         r"""
         Instantiate the ERM class.
 
         Parameters
         ----------
         loss: string, default='square'
             Loss function to be used. Possible choices are
@@ -245,16 +247,17 @@
         self.limited_memory_qning = limited_memory_qning
         self.fista_restart = fista_restart
         self.verbose = verbose
         self.warm_start = warm_start
         self.multi_class = multi_class
         self.duality_gap_interval = duality_gap_interval
         self.n_threads = n_threads
+        self.safe = safe
 
-    def fit(self, X, y, le_parameter=None):
+    def fit(self, X, labels, le_parameter=None):
         """
         Fit the parameters.
 
         Parameters
         ----------
             X (numpy array or scipy sparse CSR matrix):
                 input n X p numpy matrix; the samples are on the rows
@@ -270,20 +273,15 @@
 
         Returns
         -------
             self (ERM):
                 Returns the instance
         """
         loss = None
-
-        X, labels, le = check_input_fit(X, y, self)
-        if le_parameter is not None:
-            self.le_ = le_parameter
-        else:
-            self.le_ = le
+        self.le_ = le_parameter
 
         if (self.multi_class == "multinomial" or
            (self.multi_class == "auto" and not self._binary_problem)) and self.loss == "logistic":
             if self.multi_class == "multinomial":
                 if len(np.unique(labels)) != 2:
                     self._binary_problem = False
 
@@ -292,20 +290,22 @@
                 "Loss has been set to multiclass-logistic because "
                 "the multiclass parameter is set to multinomial!")
 
         if loss is None:
             loss = self.loss
 
         labels = np.squeeze(labels)
-
         initial_weight, yf, nclasses = self._initialize_weight(X, labels)
 
         training_data_fortran = X.T if scipy.sparse.issparse(
             X) else np.asfortranarray(X.T)
         w = np.copy(initial_weight)
+
+        training_data_fortran, yf = windows_conversion(training_data_fortran, yf)
+
         self.optimization_info_ = cyanure_lib.erm_(
             training_data_fortran, yf, initial_weight, w, dual_variable=self.dual, loss=loss,
             penalty=self.penalty, solver=self.solver, lambda_1=float(self.lambda_1),
             lambda_2=float(self.lambda_2), lambda_3=float(self.lambda_3),
             intercept=bool(self.fit_intercept),
             tol=float(self.tol), duality_gap_interval=int(self.duality_gap_interval),
             max_iter=int(self.max_iter), limited_memory_qning=int(self.limited_memory_qning),
@@ -661,24 +661,24 @@
     def _more_tags(self):
         return {"multioutput": True, "requires_y": True}
 
     def __init__(self, loss='square', penalty='l2', fit_intercept=True, random_state=0,
                  lambda_1=0, lambda_2=0, lambda_3=0, solver='auto', tol=1e-3,
                  duality_gap_interval=10, max_iter=500,
                  limited_memory_qning=20, fista_restart=50, verbose=True,
-                 warm_start=False, n_threads=-1, dual=None):
+                 warm_start=False, n_threads=-1, dual=None, safe=True):
         if loss != 'square':
             raise ValueError("square loss should be used")
         super().__init__(loss=loss, penalty=penalty,
                          fit_intercept=fit_intercept, random_state=random_state, lambda_1=lambda_1,
                          lambda_2=lambda_2, lambda_3=lambda_3, solver=solver, tol=tol,
                          duality_gap_interval=duality_gap_interval, max_iter=max_iter,
                          limited_memory_qning=limited_memory_qning,
                          fista_restart=fista_restart, verbose=verbose,
-                         warm_start=warm_start, n_threads=n_threads, dual=dual)
+                         warm_start=warm_start, n_threads=n_threads, dual=dual, safe=safe)
 
     def fit(self, X, y, le_parameter=None):
         """
         Fit the parameters.
 
         Parameters
         ----------
@@ -690,15 +690,18 @@
                 - matrix of size n X k for multivariate regression
 
         Returns
         -------
             self (ERM):
                 Returns the instance of the class
         """
-        X, labels, _ = check_input_fit(X, y, self)
+        if self.safe:
+            X, labels, _ = check_input_fit(X, y, self)
+        else:
+            labels = y
 
         if labels.squeeze().ndim <= 1:
             self._binary_problem = True
         else:
             self._binary_problem = False
 
         return super().fit(X, labels, le_parameter)
@@ -715,19 +718,23 @@
         Returns
         -------
             pred (numpy.array):
                 Prediction for the X matrix
         """
         check_is_fitted(self)
 
-        X = check_input_inference(X, self)
+        if self.safe:
+            X = check_input_inference(X, self)
 
         X = self._validate_data(X, accept_sparse="csr", reset=False)
-        pred = safe_sparse_dot(
-            X, self.coef_, dense_output=False) + self.intercept_
+        if self.fit_intercept:
+            pred = safe_sparse_dot(
+                X, self.coef_, dense_output=False) + self.intercept_
+        else:
+            pred = safe_sparse_dot(X, self.coef_, dense_output=False)
 
         return pred.squeeze()
 
     def score(self, X, y, sample_weight=None):
         r"""
         Return the coefficient of determination of the prediction.
 
@@ -914,23 +921,23 @@
 
     _estimator_type = "classifier"
 
     def __init__(self, loss='square', penalty='l2', fit_intercept=True, tol=1e-3, solver="auto",
                  random_state=0, max_iter=500, fista_restart=50, verbose=True,
                  warm_start=False, multi_class="auto",
                  limited_memory_qning=20, lambda_1=0, lambda_2=0, lambda_3=0,
-                 duality_gap_interval=5, n_threads=-1, dual=None):
+                 duality_gap_interval=5, n_threads=-1, dual=None, safe=True):
         super().__init__(loss=loss, penalty=penalty, fit_intercept=fit_intercept,
                          tol=tol, solver=solver,
                          random_state=random_state, max_iter=max_iter, fista_restart=fista_restart,
                          verbose=verbose, warm_start=warm_start,
                          limited_memory_qning=limited_memory_qning,
                          lambda_1=lambda_1, lambda_2=lambda_2, lambda_3=lambda_3,
                          duality_gap_interval=duality_gap_interval,
-                         n_threads=n_threads, multi_class=multi_class, dual=dual)
+                         n_threads=n_threads, multi_class=multi_class, dual=dual, safe=safe)
 
     def fit(self, X, y, le_parameter=None):
         """
         Fit the parameters.
 
         Parameters
         ----------
@@ -940,15 +947,20 @@
         y (numpy.array):
             Input labels.
 
             - vector of size n with {-1, +1} labels for binary classification,
               which will be automatically converted if labels in {0,1} are
               provided and {0,1,..., n} for multiclass classification.
         """
-        X, labels, le = check_input_fit(X, y, self)
+        if self.safe:
+            X, labels, le = check_input_fit(X, y, self)
+        else:
+            labels = y
+            le = None
+
         if le_parameter is not None:
             self.le_ = le_parameter
         else:
             self.le_ = le
 
         labels = np.squeeze(labels)
         unique = np.unique(labels)
@@ -983,14 +995,15 @@
                 labels = labels - min_value
             self._binary_problem = False
 
         super().fit(
             X, labels, le_parameter=self.le_)
 
         self.coef_ = self.coef_.reshape(self.coef_.shape[0], -1)
+        self.coef_ = np.squeeze(self.coef_)
         if self.fit_intercept:
             self.intercept_ = self.intercept_.reshape(1, -1)
 
         return self
 
     def predict(self, X):
         """
@@ -1004,16 +1017,14 @@
         Returns
         -------
             pred (numpy.array):
                 Prediction for the X matrix
         """
         check_is_fitted(self)
 
-        X = check_input_inference(X, self)
-
         pred = self.decision_function(X)
 
         output = None
         if len(self.classes_) == 2:
             if self.le_ is None:
                 output = np.sign(pred)
                 output[output == -1.0] = self.classes_[0]
@@ -1047,15 +1058,16 @@
         Returns
         -------
             score : float
                 Mean accuracy of ``self.predict(X)`` wrt. `y`.
         """
         check_is_fitted(self)
 
-        X = check_input_inference(X, self)
+        if self.safe:
+            X = check_input_inference(X, self)
 
         pred = np.squeeze(self.predict(X))
         return np.sum(np.squeeze(y) == pred) / pred.shape[0]
 
     def decision_function(self, X):
         """
         Predict confidence scores for samples.
@@ -1070,15 +1082,16 @@
             scores (numpy.array):
                 Confidence scores per (n_samples, n_classes) combination.
                 In the binary case, confidence score for self.classes_[1] where >0 means t
                 his class would be predicted.
         """
         check_is_fitted(self)
 
-        X = check_input_inference(X, self)
+        if self.safe:
+            X = check_input_inference(X, self)
 
         if self.fit_intercept:
             scores = safe_sparse_dot(
                 X, self.coef_, dense_output=False) + self.intercept_
         else:
             scores = safe_sparse_dot(X, self.coef_, dense_output=False)
 
@@ -1102,15 +1115,16 @@
         Returns
         -------
             proba (numpy.array):
                 Return the probability of the samples for each class.
         """
         check_is_fitted(self)
 
-        X = check_input_inference(X, self)
+        if self.safe:
+            X = check_input_inference(X, self)
 
         decision = self.decision_function(X)
         if decision.ndim == 1:
             # Workaround for binary outcomes
             # which requires softmax prediction with only a 1D decision.
             decision = np.c_[-decision, decision]
         return softmax(decision, copy=False)
@@ -1119,48 +1133,48 @@
 class LinearSVC(Classifier):
     """A pre-configured class for square hinge loss."""
 
     def __init__(self, loss='sqhinge', penalty='l2', fit_intercept=True,
                  verbose=False, lambda_1=0.1, lambda_2=0, lambda_3=0,
                  solver='auto', tol=1e-3, duality_gap_interval=10,
                  max_iter=500, limited_memory_qning=20,
-                 fista_restart=50, warm_start=False, n_threads=-1, random_state=0, dual=None):
+                 fista_restart=50, warm_start=False, n_threads=-1, random_state=0, dual=None, safe=True):
         if loss not in ['squared_hinge', 'sqhinge']:
             logger.error("LinearSVC is only compatible with squared hinge loss at "
                          "the moment")
         super().__init__(
             loss=loss, penalty=penalty, fit_intercept=fit_intercept,
             solver=solver, tol=tol, random_state=random_state, verbose=verbose,
             lambda_1=lambda_1, lambda_2=lambda_2, lambda_3=lambda_3,
             duality_gap_interval=duality_gap_interval, max_iter=max_iter,
             limited_memory_qning=limited_memory_qning,
-            fista_restart=fista_restart, warm_start=warm_start, n_threads=n_threads, dual=dual)
+            fista_restart=fista_restart, warm_start=warm_start, n_threads=n_threads, dual=dual, safe=safe)
 
 
 class LogisticRegression(Classifier):
     """A pre-configured class for logistic regression loss."""
 
     _estimator_type = "classifier"
 
     def __init__(self, penalty='l2', loss='logistic', fit_intercept=True,
                  verbose=False, lambda_1=0, lambda_2=0, lambda_3=0,
                  solver='auto', tol=1e-3, duality_gap_interval=10,
                  max_iter=500, limited_memory_qning=20,
                  fista_restart=50, warm_start=False, n_threads=-1,
-                 random_state=0, multi_class="auto", dual=None):
+                 random_state=0, multi_class="auto", dual=None, safe=True):
         super().__init__(loss=loss, penalty=penalty, fit_intercept=fit_intercept,
                          solver=solver, tol=tol, random_state=random_state, verbose=verbose,
                          lambda_1=lambda_1, lambda_2=lambda_2, lambda_3=lambda_3,
                          duality_gap_interval=duality_gap_interval, max_iter=max_iter,
                          limited_memory_qning=limited_memory_qning, multi_class=multi_class,
                          fista_restart=fista_restart, warm_start=warm_start,
-                         n_threads=n_threads, dual=dual)
+                         n_threads=n_threads, dual=dual, safe=safe)
 
 
-def compute_r(estimator_name, aux, X, labels, active_set):
+def compute_r(estimator_name, aux, X, labels, active_set, fit_intercept):
     """
     Compute R coefficient corresponding to the estimator.
 
     Parameters
     ----------
         estimator_name (string):
             Name of the estimator class
@@ -1180,25 +1194,28 @@
     Returns
     -------
         R (float):
             _description_
     """
     R = None
 
-    pred = aux.predict(X[:, active_set])
+    if len(active_set) != 0:
+        pred = aux.predict(X[:, active_set])
     if estimator_name == "Lasso":
         if len(active_set) == 0:
             R = labels
         else:
             R = labels.ravel() - pred.ravel()
     elif estimator_name == "L1Logistic":
         if len(active_set) == 0:
             R = -0.5 * labels.ravel()
         else:
             R = -labels.ravel() / (1.0 + np.exp(labels.ravel() * pred.ravel()))
+        if fit_intercept:
+            pred += aux.intercept_
 
     return R
 
 
 def fit_large_feature_number(estimator, aux, X, labels):
     """
     Fitting function when the number of feature is superior to 1000.
@@ -1217,68 +1234,90 @@
         labels (numpy.array):
             Labels matrix
     """
     n, p = X.shape
 
     scaling = 4.0
     init = min(100, p)
-    estimator.restart = True
+
     num_as = math.ceil(math.log10(p / init) / math.log10(scaling))
     active_set = []
     n_active = 0
+
     estimator.coef_ = np.zeros(p, dtype=X.dtype)
+    estimator.restart = True
+
     if estimator.fit_intercept:
         estimator.intercept_ = 0
 
+    estimator_name = type(estimator).__name__
+
     for ii in range(num_as):
-        R = compute_r(estimator.__name__, aux, X, labels, active_set)
+        R = compute_r(estimator_name, aux, X, labels, active_set, estimator.fit_intercept)
 
         corr = np.abs(X.transpose().dot(R).ravel()) / n
+
         if n_active > 0:
             corr[active_set] = -10e10
+
         n_new_as = max(
             min(init * math.ceil(scaling ** ii), p) - n_active, 0)
         new_as = corr.argsort()[-n_new_as:]
+
         if len(new_as) == 0 or max(corr[new_as]) <= estimator.lambda_1 * (1 + estimator.tol):
             break
+
         if len(active_set) > 0:
             neww = np.zeros(n_active + n_new_as,
                             dtype=X.dtype)
             neww[0:n_active] = aux.coef_
             aux.coef_ = neww
             active_set = np.concatenate((active_set, new_as))
         else:
             active_set = new_as
             aux.coef_ = np.zeros(
                 len(active_set), dtype=X.dtype)
+
         n_active = len(active_set)
+
         if estimator.verbose:
             logger.info("Size of the active set: {%d}", n_active)
+
         aux.fit(X[:, active_set], labels)
+
         estimator.coef_[active_set] = aux.coef_
         if estimator.fit_intercept:
             estimator.intercept_ = aux.intercept_
 
+    return estimator
+
+
+def execute_fit_large_feature_number(instance, auxiliary_solver, X, labels):
+
+    with concurrent.futures.ProcessPoolExecutor() as executor:
+        f = executor.submit(fit_large_feature_number, instance, auxiliary_solver, X, labels)
+        return f.result()  # will rethrow any exceptions
+
 
 class Lasso(Regression):
     """
     A pre-configured class for Lasso regression.
 
     Using active set when the number of features is superior to 1000.
     """
 
     def __init__(self, lambda_1=0, solver='auto', tol=1e-3,
                  duality_gap_interval=10, max_iter=500, limited_memory_qning=20,
                  fista_restart=50, verbose=True,
-                 warm_start=False, n_threads=-1, random_state=0, fit_intercept=True, dual=None):
+                 warm_start=False, n_threads=-1, random_state=0, fit_intercept=True, dual=None, safe=True):
         super().__init__(loss='square', penalty='l1', lambda_1=lambda_1, solver=solver, tol=tol,
                          duality_gap_interval=duality_gap_interval, max_iter=max_iter,
                          limited_memory_qning=limited_memory_qning, fista_restart=fista_restart,
                          verbose=verbose, warm_start=warm_start, n_threads=n_threads,
-                         random_state=random_state, fit_intercept=fit_intercept, dual=dual)
+                         random_state=random_state, fit_intercept=fit_intercept, dual=dual, safe=safe)
 
     def fit(self, X, y):
         """
         Fit the parameters.
 
         Parameters
         ----------
@@ -1290,25 +1329,35 @@
                 - matrix of size n X k for multivariate regression
 
         Returns
         -------
             self (ERM):
                 Returns the instance of the class
         """
-        X, labels, _ = check_input_fit(X, y, self)
+        if self.safe:
+            X, labels, _ = check_input_fit(X, y, self)
+        else:
+            labels = y
 
         _, p = X.shape
         if p <= 1000:
             # no active set
             super().fit(X, labels)
         else:
             aux = Regression(loss='square', penalty='l1',
-                             fit_intercept=self.fit_intercept, random_state=self.random_state)
+                             fit_intercept=self.fit_intercept, random_state=self.random_state,
+                             lambda_1=self.lambda_1, safe=self.safe,
+                             tol=self.tol, duality_gap_interval=self.duality_gap_interval,
+                             max_iter=self.max_iter, solver=self.solver, verbose=self.verbose)
+
+            estimator = execute_fit_large_feature_number(self, aux, X, labels)
 
-            fit_large_feature_number(self, aux, X, labels)
+            self.coef_ = estimator.coef_
+            if self.fit_intercept:
+                self.intercept_ = estimator.intercept_
 
         return self
 
 
 class L1Logistic(Classifier):
     """
     A pre-configured class for L1 logistic classification.
@@ -1324,21 +1373,21 @@
                     "We have a different implementation of _n_iter in the multinomial case."
                 ),
                 }}
 
     def __init__(self, lambda_1=0, solver='auto', tol=1e-3,
                  duality_gap_interval=10, max_iter=500, limited_memory_qning=20,
                  fista_restart=50, verbose=True, warm_start=False, n_threads=-1,
-                 random_state=0, fit_intercept=True, multi_class="auto", dual=None):
+                 random_state=0, fit_intercept=True, multi_class="auto", dual=None, safe=True):
         super().__init__(loss='logistic', penalty='l1', lambda_1=lambda_1, solver=solver, tol=tol,
                          duality_gap_interval=duality_gap_interval, max_iter=max_iter,
                          limited_memory_qning=limited_memory_qning,
                          fista_restart=fista_restart, verbose=verbose,
                          warm_start=warm_start, n_threads=n_threads, random_state=random_state,
-                         fit_intercept=fit_intercept, multi_class=multi_class, dual=dual)
+                         fit_intercept=fit_intercept, multi_class=multi_class, dual=dual, safe=safe)
 
         if multi_class == "multinomial":
             self.loss = "multiclass-logistic"
 
     def fit(self, X, y):
         """
         Fit the parameters.
@@ -1351,21 +1400,34 @@
         y (numpy.array):
             Input labels.
 
             - vector of size n with {-1, +1} labels for binary classification,
               which will be automatically converted if labels in {0,1} are
               provided and {0,1,..., n} for multiclass classification.
         """
-        X, labels, le = check_input_fit(X, y, self)
+
+        if self.safe:
+            X, labels, le = check_input_fit(X, y, self)
+        else:
+            le = None
+            labels = y
         self.le_ = le
 
         _, p = X.shape
         if p <= 1000:
             # no active set
             super().fit(X, labels, le_parameter=self.le_)
         else:
             aux = Classifier(
-                loss='logistic', penalty='l1', fit_intercept=self.fit_intercept)
+                loss='logistic', penalty='l1', fit_intercept=self.fit_intercept,
+                random_state=self.random_state,
+                lambda_1=self.lambda_1, safe=self.safe, tol=self.tol,
+                duality_gap_interval=self.duality_gap_interval, max_iter=self.max_iter,
+                solver=self.solver, verbose=self.verbose)
 
-            fit_large_feature_number(self, aux, X, labels)
+            estimator = execute_fit_large_feature_number(self, aux, X, labels)
+
+            self.coef_ = estimator.coef_
+            if self.fit_intercept:
+                self.intercept_ = estimator.intercept_
 
         return self
```

### Comparing `cyanure-1.0.0/cyanure/logger.py` & `cyanure-1.1.0/cyanure/logger.py`

 * *Files identical despite different names*

### Comparing `cyanure-1.0.0/cyanure_lib/cyanure_wrap_module.cpp` & `cyanure-1.1.0/cyanure_lib/cyanure_wrap_module.cpp`

 * *Files 3% similar despite different names*

```diff
@@ -49,15 +49,15 @@
                 PyErr_SetString(PyExc_TypeError, "Got wrong input size");
                 return NULL;
             }
             if (isSparseMatrix(inX))
             {
                 SpMatrix<M, sparse_type> X;
                 npyToSpMatrix<M, sparse_type>(inX, X, "Data");
-                param.minibatch = MIN((int)floor((M(X.n()) * M(X.m())) / M(X.nzmax())), X.n() / 100); // aggressive strategy, but only uses minibatch if required
+                param.minibatch = MAX(MIN((int)floor((M(X.n()) * M(X.m())) / M(X.nzmax())), X.n() / 100), 1); // aggressive strategy, but only uses minibatch if required
                 SIMPLE_ERM<SpMatrix<M, sparse_type>, LinearLossVec<SpMatrix<M, sparse_type>>> problem_configuration(w0, w, dual_variable, optim_info, param, model);
                 problem_configuration.solve_problem(X, y);
             }
             else
             {
                 Matrix<M> X;
                 param.minibatch = 1;
@@ -194,14 +194,15 @@
     }
     else if (M == getTypeNumber<double>() && sparse_type == getTypeNumber<long long int>())
     {
         optim_info = erm<double, long long int>(X, y, w0, w, dual, max_iter, limited_memory_qning, fista_restart, tol, duality_gap_interval, verbose, solver, loss, regul, lambda_1, lambda_2, lambda_3, intercept, univariate, n_threads);
     }
     else
     {
+        //PyErr_SetString(PyExc_TypeError, ("Wrong data type combinaison: data type is: " + std::to_string(getTypeNumber<double>()) + " and pointer type is: " + std::to_string(getTypeNumber<long long int>())).c_str());
         PyErr_SetString(PyExc_TypeError, ("Wrong data type combinaison: data type is: " + std::to_string(M) + " and pointer type is: " + std::to_string(sparse_type)).c_str());
         return NULL;
     }
     return PyArray_Return(optim_info);
 };
 
 template <typename M, typename sparse_type>
```

### Comparing `cyanure-1.0.0/cyanure_lib/lib/BLAS/cblas_alt_template.h` & `cyanure-1.1.0/cyanure_lib/lib/BLAS/cblas_alt_template.h`

 * *Files 0% similar despite different names*

```diff
@@ -140,14 +140,15 @@
 #endif
 
 /// external functions
 INTT cblas_idamin( INTT n,  double* X,  INTT incX);
 INTT cblas_isamin( INTT n,  float* X,  INTT incX);
 
 //#define HAVE_MKL
+#define HAVE_OPENBLAS
 
 template <typename T>
 static inline T alt_log(const T x);
 template <> inline double alt_log<double>(const double x) { return log(x); };
 template <> inline float alt_log<float>(const float x) { return logf(x); };
 
 template <typename T>
```

### Comparing `cyanure-1.0.0/cyanure_lib/lib/BLAS/cblas_defvar.h` & `cyanure-1.1.0/cyanure_lib/lib/BLAS/cblas_defvar.h`

 * *Files identical despite different names*

### Comparing `cyanure-1.0.0/cyanure_lib/lib/BLAS/configure_blas.h` & `cyanure-1.1.0/cyanure_lib/lib/BLAS/configure_blas.h`

 * *Files 23% similar despite different names*

```diff
@@ -1,42 +1,53 @@
 #ifndef CONFIGURE_BLAS_H
 #define CONFIGURE_BLAS_H
 
+#include <cblas.h>
+
 #ifdef HAVE_MKL
 extern "C" {
-   void MKL_Set_Num_Threads(int n_threads);
-   int MKL_Get_Max_Threads();
+    void MKL_Set_Num_Threads(int n_threads);
+    int MKL_Get_Max_Threads();
+}
+#endif
+
+#ifdef HAVE_OPENBLAS
+extern "C" {
+    void openblas_set_num_threads(int n_threads);
 }
 #endif
 
 static inline void set_mkl_sequential() {
 #ifdef HAVE_MKL
-   MKL_Set_Num_Threads(1);
+    MKL_Set_Num_Threads(1);
 #endif
 };
 
 static inline void set_mkl_parallel() {
 #ifdef HAVE_MKL
 #ifdef _OPENMP
-   MKL_Set_Num_Threads(omp_get_max_threads());
+    MKL_Set_Num_Threads(omp_get_max_threads());
 #endif
 #endif
 };
 
 
 static inline int init_omp(const int numThreads) {
-   int NUM_THREADS;
+    int NUM_THREADS;
 #ifdef _OPENMP
-   NUM_THREADS = (numThreads == -1) ? MIN(MAX_THREADS,omp_get_num_procs()) : numThreads;
-   //omp_set_nested(0);
-   omp_set_dynamic(1);
-   omp_set_num_threads(NUM_THREADS);
-   omp_set_max_active_levels(1);
-   set_mkl_parallel();
+    NUM_THREADS = (numThreads == -1) ? MIN(MAX_THREADS, omp_get_num_procs()) : numThreads;
+    omp_set_dynamic(1);
+    omp_set_num_threads(NUM_THREADS);
+    omp_set_max_active_levels(1);
+#ifdef HAVE_MKL
+    set_mkl_parallel();
+#elif defined(HAVE_OPENBLAS)
+    openblas_set_num_threads(NUM_THREADS);
+#endif
 #else
-   NUM_THREADS = 1;
+    NUM_THREADS = 1;
 #endif
-   return NUM_THREADS;
+    return NUM_THREADS;
 }
 
 
 #endif
```

### Comparing `cyanure-1.0.0/cyanure_lib/lib/basic_math_template.h` & `cyanure-1.1.0/cyanure_lib/lib/basic_math_template.h`

 * *Files identical despite different names*

### Comparing `cyanure-1.0.0/cyanure_lib/lib/convert_cxx_to_python.h` & `cyanure-1.1.0/cyanure_lib/lib/convert_cxx_to_python.h`

 * *Files identical despite different names*

### Comparing `cyanure-1.0.0/cyanure_lib/lib/data_structure/data.h` & `cyanure-1.1.0/cyanure_lib/lib/data_structure/data.h`

 * *Files identical despite different names*

### Comparing `cyanure-1.0.0/cyanure_lib/lib/data_structure/declare_structures.h` & `cyanure-1.1.0/cyanure_lib/lib/data_structure/declare_structures.h`

 * *Files identical despite different names*

### Comparing `cyanure-1.0.0/cyanure_lib/lib/data_structure/linalg.h` & `cyanure-1.1.0/cyanure_lib/lib/data_structure/linalg.h`

 * *Files identical despite different names*

### Comparing `cyanure-1.0.0/cyanure_lib/lib/data_structure/list.h` & `cyanure-1.1.0/cyanure_lib/lib/data_structure/list.h`

 * *Files identical despite different names*

### Comparing `cyanure-1.0.0/cyanure_lib/lib/data_structure/structures/matrix.h` & `cyanure-1.1.0/cyanure_lib/lib/data_structure/structures/matrix.h`

 * *Files identical despite different names*

### Comparing `cyanure-1.0.0/cyanure_lib/lib/data_structure/structures/optim_info.h` & `cyanure-1.1.0/cyanure_lib/lib/data_structure/structures/optim_info.h`

 * *Files identical despite different names*

### Comparing `cyanure-1.0.0/cyanure_lib/lib/data_structure/structures/sp_matrix.h` & `cyanure-1.1.0/cyanure_lib/lib/data_structure/structures/sp_matrix.h`

 * *Files 1% similar despite different names*

```diff
@@ -362,15 +362,15 @@
     if (beta) {
         y.scal(beta);
     }
     else {
         y.setZeros();
     }
     const floating_type* prX = x.rawX();
-#pragma omp parallel for
+ #pragma omp parallel for
     for (I i = 0; i < _n; ++i) {
         floating_type sum = floating_type();
         for (I j = _pB[i]; j < _pE[i]; ++j) {
             sum += _v[j] * prX[_r[j]];
         }
         y[i] += alpha * sum;
     }
@@ -723,35 +723,21 @@
     Matrix<floating_type>& XAt) const {
     I j, i;
     I n = X._m;
     I K = _m;
     I M = _n;
 
     XAt.resize(n, K);
-    /* compute X alpha^floating_type */
- //   int NUM_THREADS=init_omp(MAX_THREADS);
-    //floating_type* XatT=new floating_type[NUM_THREADS*n*K];
-    //for (j = 0; j<NUM_THREADS*n*K; ++j) XatT[j]=floating_type();
 
- //#pragma omp parallel for private(i,j)
+ #pragma omp parallel for private(i,j)
     for (i = 0; i < M; ++i) {
-        //#ifdef _OPENMP
-        //      int numT=omp_get_thread_num();
-        //#else
-        //      int numT=0;
-        //#endif
-        //      floating_type* write_area=XatT+numT*n*K;
         for (j = _pB[i]; j < _pE[i]; ++j) {
             cblas_axpy<floating_type>(n, _v[j], X._X + i * n, 1, XAt._X + _r[j] * n, 1);
         }
     }
-    //  cblas_copy<floating_type>(n*K,XatT,1,XAt._X,1);
-   //   for (i = 1; i<NUM_THREADS; ++i) 
-   //      cblas_axpy<floating_type>(n*K,1.0,XatT+n*K*i,1,XAt._X,1);
-   //   delete[](XatT);
 };
 
 /// XAt <- X(:,indices)*A(:,indices)'
 template <typename floating_type, typename I> inline void SpMatrix<floating_type, I>::XAt(const Matrix<floating_type>& X,
     Matrix<floating_type>& XAt, const Vector<I>& indices) const {
     I j, i;
     I n = X._m;
```

### Comparing `cyanure-1.0.0/cyanure_lib/lib/data_structure/structures/sp_vector.h` & `cyanure-1.1.0/cyanure_lib/lib/data_structure/structures/sp_vector.h`

 * *Files identical despite different names*

### Comparing `cyanure-1.0.0/cyanure_lib/lib/data_structure/structures/vector.h` & `cyanure-1.1.0/cyanure_lib/lib/data_structure/structures/vector.h`

 * *Files 0% similar despite different names*

```diff
@@ -557,25 +557,23 @@
             _X[i] = 0;
         }
     }
 };
 
 /// performs soft-thresholding of the vector
 template <typename floating_type> inline void Vector<floating_type>::fastSoftThrshold(const floating_type nu) {
-    //#pragma omp parallel for
     for (INTM i = 0; i < _n; ++i)
     {
         _X[i] = fastSoftThrs(_X[i], nu);
     }
 };
 
 /// performs soft-thresholding of the vector
 template <typename floating_type> inline void Vector<floating_type>::fastSoftThrshold(Vector<floating_type>& output, const floating_type nu) const {
     output.resize(_n, false);
-    //#pragma omp parallel for
     for (INTM i = 0; i < _n; ++i)
         output[i] = fastSoftThrs(_X[i], nu);
 };
 
 /// performs soft-thresholding of the vector
 template <typename floating_type> inline void Vector<floating_type>::softThrsholdScal(Vector<floating_type>& out, const floating_type nu, const floating_type s) {
     floating_type* Y = out.rawX();
@@ -600,15 +598,16 @@
         }
     }
 };
 
 
 /// performs thresholding of the vector
 template <typename floating_type> inline void Vector<floating_type>::thrsmax(const floating_type nu) {
-    //#pragma omp parallel for private(i)
+
+    #pragma omp parallel for
     for (INTM i = 0; i < _n; ++i)
         if (_X[i] < nu) _X[i] = nu;
 }
 
 /// performs thresholding of the vector
 template <typename floating_type> inline void Vector<floating_type>::thrsmin(const floating_type nu) {
     for (INTM i = 0; i < _n; ++i)
```

### Comparing `cyanure-1.0.0/cyanure_lib/lib/erm/erm.h` & `cyanure-1.1.0/cyanure_lib/lib/erm/erm.h`

 * *Files identical despite different names*

### Comparing `cyanure-1.0.0/cyanure_lib/lib/erm/multi_erm.h` & `cyanure-1.1.0/cyanure_lib/lib/erm/multi_erm.h`

 * *Files 0% similar despite different names*

```diff
@@ -17,29 +17,29 @@
     // X is p x n
    // y is nclasses x n
    // W0 is p x nclasses if no intercept (or p+1 x nclasses with intercept)
    // prediction model is   W0^FeatureType X  gives  nclasses x n
     void solve_problem_vector(const InputMatrixType& X, const Vector<int>& y) {
         verify_input(X);
 
+        init_omp(super::param.threads);
+
         const int nclass = y.maxval() + 1;
         if ((super::is_regression_loss(super::model.loss) || !super::is_loss_for_matrices(super::model.loss)))
         {
             const int n = y.n();
             Matrix<typename InputMatrixType::value_type> labels(nclass, n);
 
             labels.set(-(1.0));
             for (int ii = 0; ii < n; ++ii)
                 labels(y[ii], ii) = (1.0);
             MULTI_ERM<InputMatrixType, LinearLossMat<InputMatrixType, Matrix<typename InputMatrixType::value_type>>> problem_configuration(W0, W, dual_variable, super::optim_info, super::param, super::model);
             return problem_configuration.solve_problem_matrix(X, labels);
         }
 
-        init_omp(super::param.threads);
-
         typedef Matrix<FeatureType> D;
         DataMatrixLinear<InputMatrixType> data(X, super::model.intercept);
 
         if (super::param.verbose)
             data.print();
 
         LinearLossMat<InputMatrixType, Vector<int>>* loss = new MultiClassLogisticLoss<InputMatrixType>(data, y);
@@ -112,16 +112,16 @@
                 {
                     dual_variable.copyRow(ii, dualcol);
                 }
                 SIMPLE_ERM<InputMatrixType, LinearLossVec<InputMatrixType>> problem_configuration = SIMPLE_ERM<InputMatrixType, LinearLossVec<InputMatrixType>>(w0col, wcol, dualcol, optim_info_col, param2, super::model);
                 problem_configuration.solve_problem(X, ycol);
                 if (dual_variable.m() == nclass)
                     dual_variable.copyToRow(ii, dualcol);
-#pragma omp critical
                 {
+#pragma omp critical
                     super::optim_info.add(optim_info_col, ii);
                     if (super::param.verbose)
                     {
                         const int noptim = optim_info_col.n() - 1;
                         logging(logINFO) << "Solver " << ii << " has terminated after " << optim_info_col(0, 0, noptim) << " epochs in " << optim_info_col(0, 5, noptim) << " seconds";
                         if (optim_info_col(0, 4, noptim) == 0)
                         {
@@ -149,15 +149,15 @@
     typedef typename InputMatrixType::value_type FeatureType;
     typedef typename InputMatrixType::index_type PointerType;
     const Matrix<FeatureType>& W0;
     Matrix<FeatureType>& W;
     Matrix<FeatureType>& dual_variable;
 
     inline void verify_input(const InputMatrixType& X) {
-        if ((super::model.intercept && X.m() + 1 != W0.m()) || (!super::model.intercept && X.m() != W0.m())){
+        if ((super::model.intercept && X.m() + 1 != W0.m()) || (!super::model.intercept && X.m() != W0.m())) {
             logging(logERROR) << "Dimension of initial point is not consistent.";
             return;
         }
         if (super::param.max_iter < 0)
         {
             throw ValueError("Maximum number of iteration must be positive");
         }
@@ -339,23 +339,23 @@
     {
         typedef Matrix<FeatureType> D;
         typedef Vector<FeatureType> V;
         Regularizer<D, PointerType>* regul;
         switch (super::model.regul)
         {
         case L2:
-            regul = transpose ? static_cast<Regularizer<D, PointerType> *>(new RegVecToMat<Ridge<V, PointerType>>(super::model))
+            regul = transpose ? static_cast<Regularizer<D, PointerType>*>(new RegVecToMat<Ridge<V, PointerType>>(super::model))
                 : new RegMat<Ridge<V, PointerType>>(super::model, nclass, transpose);
             break;
         case L1:
-            regul = transpose ? static_cast<Regularizer<D, PointerType> *>(new RegVecToMat<Lasso<V, PointerType>>(super::model))
+            regul = transpose ? static_cast<Regularizer<D, PointerType>*>(new RegVecToMat<Lasso<V, PointerType>>(super::model))
                 : new RegMat<Lasso<V, PointerType>>(super::model, nclass, transpose);
             break;
         case ELASTICNET:
-            regul = transpose ? static_cast<Regularizer<D, PointerType> *>(new RegVecToMat<ElasticNet<V, PointerType>>(super::model))
+            regul = transpose ? static_cast<Regularizer<D, PointerType>*>(new RegVecToMat<ElasticNet<V, PointerType>>(super::model))
                 : new RegMat<ElasticNet<V, PointerType>>(super::model, nclass, transpose);
             break;
         case L1BALL:
             regul = new RegMat<L1Ball<V, PointerType>>(super::model, nclass, transpose);
             break;
         case L2BALL:
             regul = new RegMat<L2Ball<V, PointerType>>(super::model, nclass, transpose);
```

### Comparing `cyanure-1.0.0/cyanure_lib/lib/erm/simple_erm.h` & `cyanure-1.1.0/cyanure_lib/lib/erm/simple_erm.h`

 * *Files identical despite different names*

### Comparing `cyanure-1.0.0/cyanure_lib/lib/error_management/exception.h` & `cyanure-1.1.0/cyanure_lib/lib/error_management/exception.h`

 * *Files identical despite different names*

### Comparing `cyanure-1.0.0/cyanure_lib/lib/logging/logger.h` & `cyanure-1.1.0/cyanure_lib/lib/logging/logger.h`

 * *Files identical despite different names*

### Comparing `cyanure-1.0.0/cyanure_lib/lib/losses/loss.h` & `cyanure-1.1.0/cyanure_lib/lib/losses/loss.h`

 * *Files identical despite different names*

### Comparing `cyanure-1.0.0/cyanure_lib/lib/losses/loss_mat/loss/multi_logistic_loss.h` & `cyanure-1.1.0/cyanure_lib/lib/losses/loss_mat/loss/multi_logistic_loss.h`

 * *Files 8% similar despite different names*

```diff
@@ -1,96 +1,97 @@
 #ifndef MULTI_LOGISTIC_LOSS_H
 #define MULTI_LOGISTIC_LOSS_H
 
 #include "../loss_mat.h"
 
 template <typename M>
-class MultiClassLogisticLoss final : public LinearLossMat<M, Vector<int> > {
-   typedef typename M::value_type T;
-   using LinearLossMat<M, Vector<int> >::_data;
-   using LinearLossMat<M, Vector<int> >::_y;
-   public:
-      MultiClassLogisticLoss(DataMatrixLinear<M>& data, const Vector<int>& y) : LinearLossMat<M, Vector<int> >(data,y) { 
-         _nclasses=y.maxval()+1;
-         this->_id=MULTI_LOGISTIC;
-      };
+class MultiClassLogisticLoss final: public LinearLossMat<M, Vector<int> > {
+    typedef typename M::value_type T;
+    using LinearLossMat<M, Vector<int> >::_data;
+    using LinearLossMat<M, Vector<int> >::_y;
+public:
+    MultiClassLogisticLoss(DataMatrixLinear<M>& data, const Vector<int>& y): LinearLossMat<M, Vector<int> >(data, y) {
+        _nclasses = y.maxval() + 1;
+        this->_id = MULTI_LOGISTIC;
+    };
 
-      inline T eval(const Matrix<T>& input) const {
+    inline T eval(const Matrix<T>& input) const {
          Matrix<T> tmp;
          _data.pred(input,tmp); 
          const int n = tmp.n();
          T sum=0;
 #pragma omp parallel for reduction(+:sum) schedule(static)
          for (int ii = 0; ii<n; ++ii) {
             Vector<T> col;
             tmp.refCol(ii,col);
             col.add(-col[_y[ii]]);
             sum+=col.logsumexp();
          }
          return sum / n;
       };
-      inline T eval(const Matrix<T>& input, const INTM i) const {
-         Vector<T> tmp;
-         _data.pred(i,input,tmp); 
-         tmp.add(-tmp[_y[i]]);
-         return tmp.logsumexp();
-      }
-      inline void print() const {
-         logging(logINFO) << "Multiclass logistic Loss is used";
-      };
-     inline T fenchel(const Matrix<T>& input) const {
+    inline T eval(const Matrix<T>& input, const INTM i) const {
+        Vector<T> tmp;
+        _data.pred(i, input, tmp);
+        tmp.add(-tmp[_y[i]]);
+        return tmp.logsumexp();
+    }
+    inline void print() const {
+        logging(logINFO) << "Multiclass logistic Loss is used";
+    };
+    inline T fenchel(const Matrix<T>& input) const {
         T sum = 0;
         const int n = input.n();
-#pragma omp parallel for reduction(+:sum) schedule(static) 
-        for (long long i = 0; i<n; ++i) {
-           const long long clas = _y[i];
-           for (long long j = 0; j<_nclasses; ++j) {
-              if (j == clas) {
-                 sum += xlogx(input[i*_nclasses+j]+1.0);
-              } else {
-                 sum += xlogx(input[i*_nclasses+j]);
-              }
-           }
+        //pragma omp parallel for reduction(+:sum) schedule(static) 
+        for (long long i = 0; i < n; ++i) {
+            const long long clas = _y[i];
+            for (long long j = 0; j < _nclasses; ++j) {
+                if (j == clas) {
+                    sum += xlogx(input[i * _nclasses + j] + 1.0);
+                }
+                else {
+                    sum += xlogx(input[i * _nclasses + j]);
+                }
+            }
         }
-        return sum/n;
-     };
+        return sum / n;
+    };
 
-   private:
-     int _nclasses; 
-     inline void get_grad_aux2(Vector<T>& col, const int ind) const {
+private:
+    int _nclasses;
+    inline void get_grad_aux2(Vector<T>& col, const int ind) const {
         col.add(-col[ind]);
         const T mm = col.maxval();
         col.add(-mm);
         col.exp();
-        col.scal(T(1.0)/col.asum());
-        col[ind]=0;
-        col[ind]=-col.asum();
-     }
-     inline void get_grad_aux(const Matrix<T>& input, Matrix<T>& grad1) const {
-         _data.pred(input,grad1);
-         const int n = grad1.n();
-#pragma omp parallel for schedule(static,16)
-         for (int ii = 0; ii<n; ++ii) {
+        col.scal(T(1.0) / col.asum());
+        col[ind] = 0;
+        col[ind] = -col.asum();
+    }
+    inline void get_grad_aux(const Matrix<T>& input, Matrix<T>& grad1) const {
+        _data.pred(input, grad1);
+        const int n = grad1.n();
+        //pragma omp parallel for schedule(static,16)
+        for (int ii = 0; ii < n; ++ii) {
             Vector<T> col;
-            grad1.refCol(ii,col);
-            get_grad_aux2(col,_y[ii]);
-         }
-      };
-      inline void scal_grad(const Matrix<T>& input, const INTM i, Vector<T>& col) const {
-          _data.pred(i,input,col);
-          get_grad_aux2(col,_y[i]);
-      };
-      inline T lipschitz_constant() const { return T(0.25);};
-      inline void get_dual_constraints(Matrix<T>& grad1) const {
-         // scale grad1 by 1/Nclasses
-         if (_data.intercept()) {
+            grad1.refCol(ii, col);
+            get_grad_aux2(col, _y[ii]);
+        }
+    };
+    inline void scal_grad(const Matrix<T>& input, const INTM i, Vector<T>& col) const {
+        _data.pred(i, input, col);
+        get_grad_aux2(col, _y[i]);
+    };
+    inline T lipschitz_constant() const { return T(0.25); };
+    inline void get_dual_constraints(Matrix<T>& grad1) const {
+        // scale grad1 by 1/Nclasses
+        if (_data.intercept()) {
             Vector<T> row;
-            for (int i = 0; i<grad1.m(); ++i) {
-               grad1.extractRow(i,row);
-               row.project_sft(_y,i);
-               grad1.setRow(i,row);
+            for (int i = 0; i < grad1.m(); ++i) {
+                grad1.extractRow(i, row);
+                row.project_sft(_y, i);
+                grad1.setRow(i, row);
             }
-         }
-      }
+        }
+    }
 };
 
 #endif
```

### Comparing `cyanure-1.0.0/cyanure_lib/lib/losses/loss_mat/loss/square_loss.h` & `cyanure-1.1.0/cyanure_lib/lib/losses/loss_mat/loss/square_loss.h`

 * *Files identical despite different names*

### Comparing `cyanure-1.0.0/cyanure_lib/lib/losses/loss_mat/loss_mat.h` & `cyanure-1.1.0/cyanure_lib/lib/losses/loss_mat/loss_mat.h`

 * *Files 2% similar despite different names*

```diff
@@ -82,46 +82,46 @@
             input.refCol(ii,col);
             sum += _losses[ii]->eval(col);
          }
          return sum;
       };
       inline T eval(const Matrix<T>& input, const INTM i) const {
          T sum=0;
-//#pragma omp parallel for reduction(+ : sum) num_threads(2)
+#pragma omp parallel for reduction(+ : sum) num_threads(2)
          for (int ii=0; ii<_N; ++ii) {
             Vector<T> col;
             input.refCol(ii,col);
             sum += _losses[ii]->eval(col,i);
          }
          return sum;
       };
       inline void add_grad(const Matrix<T>& input, const INTM i, Matrix<T>& output, const T eta = T(1.0)) const {
          output.resize(input.m(),input.n());
-//#pragma omp parallel for num_threads(2)
+#pragma omp parallel for num_threads(2)
          for (int ii=0; ii<_N; ++ii) {
             Vector<T> col_input, col_output;
             input.refCol(ii,col_input);
             output.refCol(ii,col_output);
             _losses[ii]->add_grad(col_input,i,col_output,eta);
          }
       };
       inline void double_add_grad(const Matrix<T>& input1, const Matrix<T>& input2, const INTM i, Matrix<T>& output, const T eta1 = T(1.0), const T eta2 = -T(1.0), const T dummy =T(1.0)) const {
          output.resize(input1.m(),input1.n());
-//#pragma omp parallel for num_threads(2)
+#pragma omp parallel for num_threads(2)
          for (int ii=0; ii<_N; ++ii) {
             Vector<T> col_input1, col_input2, col_output;
             input1.refCol(ii,col_input1);
             input2.refCol(ii,col_input2);
             output.refCol(ii,col_output);
             _losses[ii]->double_add_grad(col_input1,col_input2,i,col_output,eta1,eta2,dummy);
          }
       };
       inline void grad(const Matrix<T>& input, Matrix<T>& output) const {
          output.resize(input.m(),input.n());
-#pragma omp parallel for 
+#pragma omp parallel for ordered
          for (int ii=0; ii<_N; ++ii) {
             Vector<T> col_input, col_output;
             input.refCol(ii,col_input);
             output.refCol(ii,col_output);
             _losses[ii]->grad(col_input,col_output);
          }
       }
@@ -131,15 +131,15 @@
       };
       inline bool provides_fenchel() const {
          return _losses[0]->provides_fenchel();
       };
       inline void get_dual_variable(const Matrix<T>& input, Matrix<T>& grad1, Matrix<T>& grad2) const {
          grad1.resize(_n,input.n());
          grad2.resize(input.m(),input.n());
-#pragma omp parallel for 
+#pragma omp parallel for ordered         
          for (int ii=0; ii<_N; ++ii) {
             Vector<T> col1, col2, col3;
             input.refCol(ii,col1);
             grad1.refCol(ii,col2);
             grad2.refCol(ii,col3);
             _losses[ii]->get_dual_variable(col1,col2,col3);
          }
@@ -159,33 +159,33 @@
       }
       inline void lipschitz(Vector<T>& Li) const {
          _losses[0]->lipschitz(Li);
       };
       // input; nclass x n
       // output: p x nclass
       virtual void  add_feature(const Matrix<T>& input, Matrix<T>& output, const T s) const { 
-#pragma omp parallel for 
+#pragma omp parallel for ordered
          for (int ii=0; ii<_N; ++ii) {
             Vector<T> col1, col2;
             input.copyRow(ii,col1);
             output.refCol(ii,col2);
             _losses[ii]->add_feature(col1,col2,s);
          }
       }
       virtual void  add_feature(Matrix<T>& output, const INTM i, const Vector<T>& s) const { 
-//#pragma omp parallel for num_threads(2)
+#pragma omp parallel for num_threads(2)
          for (int ii=0; ii<_N; ++ii) {
             Vector<T> col;
             output.refCol(ii,col);
             _losses[ii]->add_feature(col,i,s[ii]);
          } 
       };
       virtual void scal_grad(const Matrix<T>& input, const INTM i, Vector<T>& output) const {
          output.resize(_N);
-//#pragma omp parallel for num_threads(2)
+#pragma omp parallel for num_threads(2)
          for (int ii=0; ii<_N; ++ii) {
             Vector<T> col;
             input.refCol(ii,col);
             _losses[ii]->scal_grad(col,i,output[ii]);
          }
       };
       virtual bool transpose() const {
```

### Comparing `cyanure-1.0.0/cyanure_lib/lib/losses/loss_vec/loss/hinge_loss.h` & `cyanure-1.1.0/cyanure_lib/lib/losses/loss_vec/loss/hinge_loss.h`

 * *Files identical despite different names*

### Comparing `cyanure-1.0.0/cyanure_lib/lib/losses/loss_vec/loss/logistic_loss.h` & `cyanure-1.1.0/cyanure_lib/lib/losses/loss_vec/loss/logistic_loss.h`

 * *Files identical despite different names*

### Comparing `cyanure-1.0.0/cyanure_lib/lib/losses/loss_vec/loss/safe_logistic_loss.h` & `cyanure-1.1.0/cyanure_lib/lib/losses/loss_vec/loss/safe_logistic_loss.h`

 * *Files identical despite different names*

### Comparing `cyanure-1.0.0/cyanure_lib/lib/losses/loss_vec/loss/square_hinge_loss.h` & `cyanure-1.1.0/cyanure_lib/lib/losses/loss_vec/loss/square_hinge_loss.h`

 * *Files identical despite different names*

### Comparing `cyanure-1.0.0/cyanure_lib/lib/losses/loss_vec/loss/square_loss.h` & `cyanure-1.1.0/cyanure_lib/lib/losses/loss_vec/loss/square_loss.h`

 * *Files identical despite different names*

### Comparing `cyanure-1.0.0/cyanure_lib/lib/losses/loss_vec/loss_vec.h` & `cyanure-1.1.0/cyanure_lib/lib/losses/loss_vec/loss_vec.h`

 * *Files identical despite different names*

### Comparing `cyanure-1.0.0/cyanure_lib/lib/macro.h` & `cyanure-1.1.0/cyanure_lib/lib/macro.h`

 * *Files identical despite different names*

### Comparing `cyanure-1.0.0/cyanure_lib/lib/regul/compute_regularization.h` & `cyanure-1.1.0/cyanure_lib/lib/regul/compute_regularization.h`

 * *Files identical despite different names*

### Comparing `cyanure-1.0.0/cyanure_lib/lib/regul/mixed_l1_norm/mixed_l1_norm.h` & `cyanure-1.1.0/cyanure_lib/lib/regul/mixed_l1_norm/mixed_l1_norm.h`

 * *Files identical despite different names*

### Comparing `cyanure-1.0.0/cyanure_lib/lib/regul/mixed_l1_norm/norms.h` & `cyanure-1.1.0/cyanure_lib/lib/regul/mixed_l1_norm/norms.h`

 * *Files identical despite different names*

### Comparing `cyanure-1.0.0/cyanure_lib/lib/regul/regularizer.h` & `cyanure-1.1.0/cyanure_lib/lib/regul/regularizer.h`

 * *Files identical despite different names*

### Comparing `cyanure-1.0.0/cyanure_lib/lib/regul/regularizers.h` & `cyanure-1.1.0/cyanure_lib/lib/regul/regularizers.h`

 * *Files 2% similar despite different names*

```diff
@@ -113,15 +113,14 @@
     }
     virtual T lambda_1() const { return _lambda; };
     inline void lazy_prox(const D &input, D &output, const Vector<I> &indices, const T eta) const
     {
         const int p = input.n();
         const int r = indices.n();
         const T thrs = _lambda * eta;
-        //#pragma omp parallel for
         for (int jj = 0; jj < r; ++jj)
             output[indices[jj]] = fastSoftThrs(input[indices[jj]], thrs);
         ;
         if (this->_intercept)
             output[p - 1] = input[p - 1];
     };
     virtual bool is_lazy() const { return true; };
@@ -187,15 +186,14 @@
     virtual T lambda_1() const { return _lambda; };
     inline void lazy_prox(const D &input, D &output, const Vector<I> &indices, const T eta) const
     {
         const int p = input.n();
         const int r = indices.n();
         const T thrs = _lambda * eta;
         const T scal = T(1.0) / (T(1.0) + _lambda2 * eta);
-#pragma omp parallel for
         for (int jj = 0; jj < r; ++jj)
             output[indices[jj]] = scal * fastSoftThrs(input[indices[jj]], thrs);
         ;
         if (this->_intercept)
             output[p - 1] = input[p - 1];
     };
     virtual bool is_lazy() const { return true; };
```

### Comparing `cyanure-1.0.0/cyanure_lib/lib/solvers/accelerator.h` & `cyanure-1.1.0/cyanure_lib/lib/solvers/accelerator.h`

 * *Files identical despite different names*

### Comparing `cyanure-1.0.0/cyanure_lib/lib/solvers/incremental_solver.h` & `cyanure-1.1.0/cyanure_lib/lib/solvers/incremental_solver.h`

 * *Files 7% similar despite different names*

```diff
@@ -2,27 +2,25 @@
 #define INCREMENTAL_SOLVER_H
 
 #include "solver.h"
 
 
 #define USING_INCREMENTAL_SOLVER                               \
     USING_SOLVER;                                              \
-    using IncrementalSolver<loss_type>::_minibatch;            \
     using IncrementalSolver<loss_type>::_non_uniform_sampling; \
     using IncrementalSolver<loss_type>::_n;                    \
     using IncrementalSolver<loss_type>::_qi;
 
 template <typename loss_type>
 class IncrementalSolver : public Solver<loss_type>
 {
 public:
     USING_SOLVER;
     IncrementalSolver(const loss_type& loss, const Regularizer<D, PointerType>& regul, const ParamSolver<FeatureType>& param, const Vector<FeatureType>* Li = NULL) : Solver<loss_type>(loss, regul, param)
     {
-        _minibatch = 1;
         _non_uniform_sampling = param.non_uniform_sampling;
         if (Li)
             _Li.copy(*Li);
     };
 
 protected:
     virtual void solver_init(const D& x0)
@@ -34,15 +32,15 @@
         {
             _qi.copy(_Li);
             _qi.scal(FeatureType(1.0) / _qi.sum());
             const FeatureType Lmean = _Li.mean();
             const FeatureType Lmax = _Li.maxval();
             _non_uniform_sampling = (_non_uniform_sampling && Lmean <= FeatureType(0.9) * Lmax);
             _L = _non_uniform_sampling ? Lmean : Lmax;
-            if (_minibatch > 1)
+            if (Solver<loss_type>::_minibatch > 1)
                 heuristic_L(x0);
             _oldL = _L;
             if (_non_uniform_sampling)
                 init_nonu_sampling();
         }
         this->check_mkl(x0);
     };
@@ -58,15 +56,15 @@
         {
             logging(logINFO) << "with uniform sampling";
         }
         logging(logINFO) << "Lipschitz constant: " << _L;
     };
 
     bool _non_uniform_sampling;
-    int _minibatch;
+    
     int _n;
     Vector<FeatureType> _qi;
     Vector<double> _Ui;
     Vector<int> _Ki;
     FeatureType _oldL;
 
     void init_nonu_sampling()
@@ -116,15 +114,15 @@
         const double y = _n * x + 1 - ind;
         if (y < _Ui[ind - 1])
             return ind - 1;
         return _Ki[ind - 1];
     };
     
     virtual int minibatch() const { 
-        return _minibatch; 
+        return Solver<loss_type>::_minibatch; 
     };
     
     FeatureType init_kappa_acceleration(const D& x0)
     {
         IncrementalSolver<loss_type>::solver_init(x0);
         const FeatureType mu = _regul.strong_convexity();
         return ((this->_oldL / (_n)-mu));
@@ -142,25 +140,25 @@
 private:
     void heuristic_L(const D& x)
     {
         if (_verbose) {
             logging(logINFO) << "Heuristic: Initial L=" << _L;
         }
         const FeatureType Lmax = _L;
-        _L /= _minibatch;
+        _L /= Solver<loss_type>::_minibatch;
         int iter = 0;
         D tmp, tmp2, grad;
-        while (iter <= log(_minibatch) / log(2.0) && _L < Lmax)
+        while (iter <= log(Solver<loss_type>::_minibatch) / log(2.0) && _L < Lmax)
         {
             tmp.copy(x);
-            const FeatureType fx = _loss.eval_random_minibatch(tmp, _minibatch);
-            _loss.grad_random_minibatch(tmp, grad, _minibatch); // should do non uniform
+            const FeatureType fx = _loss.eval_random_minibatch(tmp, Solver<loss_type>::_minibatch);
+            _loss.grad_random_minibatch(tmp, grad, Solver<loss_type>::_minibatch); // should do non uniform
             // compute grad and fx
             tmp.add(grad, -FeatureType(1.0) / _L);
-            const FeatureType ftmp = _loss.eval_random_minibatch(tmp, _minibatch);
+            const FeatureType ftmp = _loss.eval_random_minibatch(tmp, Solver<loss_type>::_minibatch);
             tmp2.copy(tmp);
             tmp2.sub(x);
             const FeatureType s1 = fx + grad.dot(tmp2);
             const FeatureType s2 = FeatureType(0.5) * tmp2.nrm2sq();
             if (ftmp > s1 + _L * s2)
                 _L = MIN(MAX(2.0 * _L, (ftmp - s1) / s2), Lmax);
             ++iter;
```

### Comparing `cyanure-1.0.0/cyanure_lib/lib/solvers/incremental_solvers/miso.h` & `cyanure-1.1.0/cyanure_lib/lib/solvers/incremental_solvers/miso.h`

 * *Files 1% similar despite different names*

```diff
@@ -12,14 +12,15 @@
     {
         _minibatch = 1;
         _mu = _regul.id() == L2 || _regul.id() == ELASTICNET ? _regul.strong_convexity() : 0;
         _kappa = _loss.kappa();
         if (_loss.id() == PPA){
             _mu += _kappa;
         }
+        
         _isprox = (_regul.id() != L2 || _regul.intercept()) && _regul.id() != NONE;
         _is_lazy = _isprox && _regul.is_lazy() && _loss.is_sparse();
         _extern_zis = false;
         _count = 0;
     };
 
     virtual void set_dual_variable(const D& dual0)
@@ -134,16 +135,17 @@
             if (_is_lazy)
             {
                 _loss.get_coordinates(ind, indices);
                 _regul.lazy_prox(ref_barz, x, indices, FeatureType(1.0) / _mu);
             }
             solver_aux_aux(x, ref_barz, ind, deltas);
 
-            if (_isprox && (!_is_lazy || ii == _n - 1))
+            if (_isprox && (!_is_lazy || ii == _n - 1)){
                 _regul.prox(ref_barz, x, FeatureType(1.0) / _mu);
+                }
         }
     };
     
     void print() const
     {
         logging(logINFO) << "MISO Solver";
         IncrementalSolver<loss_type>::print();
```

### Comparing `cyanure-1.0.0/cyanure_lib/lib/solvers/incremental_solvers/svrg.h` & `cyanure-1.1.0/cyanure_lib/lib/solvers/incremental_solvers/svrg.h`

 * *Files 2% similar despite different names*

```diff
@@ -20,16 +20,14 @@
 
 template <typename loss_type>
 class SVRG_Solver : public IncrementalSolver<loss_type>
 {
 public:
     USING_INCREMENTAL_SOLVER;
     SVRG_Solver(const loss_type& loss, const Regularizer<D, PointerType>& regul, const ParamSolver<FeatureType>& param, const Vector<FeatureType>* Li = NULL) : IncrementalSolver<loss_type>(loss, regul, param, Li) {
-        //TODO Vérifier avec Julien
-        _minibatch = 1;
     };
 
 protected:
     virtual void solver_init(const D& x0)
     {
         // Rename x0 and x with w0 and w
         IncrementalSolver<loss_type>::solver_init(x0);
@@ -74,21 +72,22 @@
 class Acc_SVRG_Solver : public SVRG_Solver<loss_type>
 {
 public:
     USING_SVRG_SOLVER;
     Acc_SVRG_Solver(const loss_type& loss, const Regularizer<D, PointerType>& regul, const ParamSolver<FeatureType>& param, const Vector<FeatureType>* Li = NULL) : SVRG_Solver<loss_type>(loss, regul, param, Li)
     {
         _accelerated_solver = allow_acc;
-        _minibatch = 1;
+        printf("%d \n", param.minibatch);
     };
 
     virtual void solver_init(const D& x0)
     {
         IncrementalSolver<loss_type>::solver_init(x0);
         _mu = _regul.strong_convexity();
+        printf("%d \n", _minibatch);
         _nn = _n / _minibatch;
         _accelerated_solver = allow_acc && (FeatureType(20) * this->_oldL / _nn > _mu);
         if (_accelerated_solver)
         {
             _gammak = MAX(_L / (_nn), _mu);
             update_acceleration_parameters();
             _xtilde.copy(x0);
@@ -106,14 +105,15 @@
 
     virtual void solver_aux(D& x)
     {
         if (_accelerated_solver)
         {
             for (int ii = 0; ii < _nn; ++ii)
             {
+                
                 x.copy(_y);
                 x.add(_gtilde, -_etak);
                 for (int jj = 0; jj < _minibatch; ++jj)
                 {
                     const int ind = _non_uniform_sampling ? this->nonu_sampling() : random() % _n;
                     const FeatureType scal = _non_uniform_sampling ? FeatureType(1.0) / (_qi[ind] * _n * _minibatch) : FeatureType(1.0) / _minibatch;
                     _loss.double_add_grad(_y, _xtilde, ind, x, -scal * _etak, scal * _etak);
@@ -175,15 +175,15 @@
     USING_ACC_SVRG_SOLVER;
 
     SVRG_Solver_FastRidge(const loss_type& loss, const Regularizer<D, PointerType>& regul, const ParamSolver<FeatureType>& param, const Vector<FeatureType>* Li = NULL) : Acc_SVRG_Solver<loss_type, allow_acc>(loss, regul, param, Li),
         _is_lazy(loss_type::is_sparse())
     {
         if (param.minibatch > 1)
         {
-            logging(logERROR) << "Minibatch is not compatible with lazy updates";
+            logging(logWARNING) << "Minibatch is not compatible with lazy updates. The minibatch parameter has been set to 1.";
         }
         _minibatch = 1;
     };
     virtual void solver_init(const D& x0)
     {
         Acc_SVRG_Solver<loss_type, allow_acc>::solver_init(x0);
         if (_loss.id() == PPA)
```

#### encoding

```diff
@@ -1 +1 @@
-utf-8
+us-ascii
```

### Comparing `cyanure-1.0.0/cyanure_lib/lib/solvers/ista.h` & `cyanure-1.1.0/cyanure_lib/lib/solvers/ista.h`

 * *Files identical despite different names*

### Comparing `cyanure-1.0.0/cyanure_lib/lib/solvers/solver.h` & `cyanure-1.1.0/cyanure_lib/lib/solvers/solver.h`

 * *Files 4% similar despite different names*

```diff
@@ -15,15 +15,17 @@
     typedef typename loss_type::index_type PointerType;    \
     typedef loss_type LT;                        \
     using Solver<loss_type>::_L;                 \
     using Solver<loss_type>::_loss;              \
     using Solver<loss_type>::_regul;             \
     using Solver<loss_type>::_Li;                \
     using Solver<loss_type>::_verbose;           \
+    using Solver<loss_type>::_minibatch;            \
     using Solver<loss_type>::_max_iter_backtracking;
+    
 
 static const int NUMBER_OPTIM_PROCESS_INFO = 6;
 
 loglevel_e loglevel = logDEBUG4;
 
 enum solver_t
 {
@@ -123,14 +125,15 @@
         _nepochs = param.max_iter;
         _max_iter_backtracking = param.max_iter_backtracking;
         _best_dual = -INFINITY;
         _best_primal = INFINITY;
         _duality = _loss.provides_fenchel() && regul.provides_fenchel();
         _optim_info.resize(NUMBER_OPTIM_PROCESS_INFO, MAX(param.max_iter / _it0, 1));
         _L = 0;
+        _minibatch = param.minibatch;
     };
     virtual ~Solver() {};
 
     virtual void solve(const D& x0, D& x)
     {
         _time.start();
         x.copy(x0);
@@ -262,14 +265,15 @@
     }
 
 protected:
     virtual void solver_init(const D& x0) = 0;
     virtual void solver_aux(D& x) = 0;
     virtual void print() const = 0;
     virtual int minibatch() const { return 1; };
+    int _minibatch;
     bool _verbose;
     int _it0;
     int _nepochs;
     int _max_iter_backtracking;
     int _restart_frequency;
     T _tol;
     const loss_type& _loss;
```

### Comparing `cyanure-1.0.0/cyanure_lib/lib/sorting_algorithms.h` & `cyanure-1.1.0/cyanure_lib/lib/sorting_algorithms.h`

 * *Files identical despite different names*

### Comparing `cyanure-1.0.0/cyanure_lib/lib/timer.h` & `cyanure-1.1.0/cyanure_lib/lib/timer.h`

 * *Files identical despite different names*

### Comparing `cyanure-1.0.0/test/test_logistic_regression.py` & `cyanure-1.1.0/test/test_logistic_regression.py`

 * *Files 2% similar despite different names*

```diff
@@ -335,16 +335,16 @@
         tol=1e-10,
     )
     lr_saga.fit(X, y)
     assert_array_almost_equal(lr_saga.coef_, lr_liblinear.coef_)
 
     # Noise and constant features should be regularized to zero by the l1
     # penalty
-    assert_array_almost_equal(lr_liblinear.coef_[-5:, 0], np.zeros(5))
-    assert_array_almost_equal(lr_saga.coef_[-5:, 0], np.zeros(5))
+    assert_array_almost_equal(lr_liblinear.coef_[-5:], np.zeros(5))
+    assert_array_almost_equal(lr_saga.coef_[-5:], np.zeros(5))
 
 
 def test_logreg_l1_sparse_data():
     # Because liblinear penalizes the intercept and saga does not, we do not
     # fit the intercept to make it possible to compare the coefficients of
     # the two models at convergence.
     rng = np.random.RandomState(42)
@@ -375,16 +375,16 @@
         max_iter=1000,
         tol=1e-10,
     )
     lr_saga.fit(X, y)
     assert_array_almost_equal(lr_saga.coef_, lr_miso.coef_)
     # Noise and constant features should be regularized to zero by the l1
     # penalty
-    assert_array_almost_equal(lr_miso.coef_[-5:, 0], np.zeros(5))
-    assert_array_almost_equal(lr_saga.coef_[-5:, 0], np.zeros(5))
+    assert_array_almost_equal(lr_miso.coef_[-5:], np.zeros(5))
+    assert_array_almost_equal(lr_saga.coef_[-5:], np.zeros(5))
 
     # Check that solving on the sparse and dense data yield the same results
     lr_saga_dense = LogisticRegression(
         penalty="l1",
         lambda_1=1.0,
         solver="ista",
         fit_intercept=False,
@@ -947,15 +947,15 @@
     X = scale(X)
     lambda_1 = 1.0 / C / n_samples
 
     sgd = SGDClassifier(
         penalty="elasticnet",
         random_state=1,
         fit_intercept=False,
-        tol=-np.inf,
+        tol=None,
         max_iter=2000,
         l1_ratio=multiplier,
         alpha=lambda_1,
         loss="log",
     )
     log = LogisticRegression(
         penalty="elasticnet",
@@ -966,15 +966,19 @@
         lambda_1=lambda_1 * multiplier,
         lambda_2=lambda_1 * (1 - multiplier),
         solver="qning-svrg",
     )
 
     sgd.fit(X, y)
     log.fit(X, y)
-    assert_array_almost_equal(sgd.coef_, np.transpose(log.coef_), decimal=1)
+    print(sgd.coef_.shape)
+    print(np.squeeze(sgd.coef_).shape)
+    print(log.coef_.shape)
+    print(np.transpose(log.coef_).shape)
+    assert_array_almost_equal(np.squeeze(sgd.coef_), np.transpose(log.coef_), decimal=1)
 
 @pytest.mark.parametrize(
     "est",
     [
         LogisticRegression(random_state=0, max_iter=500),
     ],
     ids=lambda x: x.__class__.__name__,
@@ -1005,16 +1009,16 @@
 
     # Make sure multi_class='ovr' is distinct from ='multinomial'
     assert not np.allclose(
         est_auto_bin.coef_,
         fit(X, y_bin, multi_class="multinomial", solver=solver).coef_,
     )
     assert not np.allclose(
-        est_auto_bin.coef_,
-        fit(X, y_multi, multi_class="multinomial", solver=solver).coef_,
+        est_auto_multi.coef_,
+        fit(X, y_multi, multi_class="ovr", solver=solver).coef_,
     )
 
 
 
 @pytest.mark.parametrize("solver", solvers)
 def test_penalty_none(solver):
     # - Make sure warning is raised if penalty='none' and lambda_1 is set to a
```

