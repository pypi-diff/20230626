# Comparing `tmp/DoubleML-0.6.2.tar.gz` & `tmp/DoubleML-0.6.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "DoubleML-0.6.2.tar", last modified: Wed Jun 21 14:29:30 2023, max compression
+gzip compressed data, was "DoubleML-0.6.3.tar", last modified: Mon Jun 26 12:41:17 2023, max compression
```

## Comparing `DoubleML-0.6.2.tar` & `DoubleML-0.6.3.tar`

### file list

```diff
@@ -1,113 +1,113 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 14:29:30.087888 DoubleML-0.6.2/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 14:29:30.075888 DoubleML-0.6.2/DoubleML.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     8771 2023-06-21 14:29:29.000000 DoubleML-0.6.2/DoubleML.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     3603 2023-06-21 14:29:30.000000 DoubleML-0.6.2/DoubleML.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-21 14:29:29.000000 DoubleML-0.6.2/DoubleML.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       51 2023-06-21 14:29:29.000000 DoubleML-0.6.2/DoubleML.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        9 2023-06-21 14:29:29.000000 DoubleML-0.6.2/DoubleML.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1583 2023-06-21 14:28:54.000000 DoubleML-0.6.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)       34 2023-06-21 14:28:54.000000 DoubleML-0.6.2/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     8771 2023-06-21 14:29:30.087888 DoubleML-0.6.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     6648 2023-06-21 14:28:54.000000 DoubleML-0.6.2/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 14:29:30.079888 DoubleML-0.6.2/doubleml/
--rw-r--r--   0 runner    (1001) docker     (123)      948 2023-06-21 14:28:54.000000 DoubleML-0.6.2/doubleml/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    13825 2023-06-21 14:28:54.000000 DoubleML-0.6.2/doubleml/_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     8740 2023-06-21 14:28:54.000000 DoubleML-0.6.2/doubleml/_utils_checks.py
--rw-r--r--   0 runner    (1001) docker     (123)     2810 2023-06-21 14:28:54.000000 DoubleML-0.6.2/doubleml/_utils_plots.py
--rw-r--r--   0 runner    (1001) docker     (123)     4818 2023-06-21 14:28:54.000000 DoubleML-0.6.2/doubleml/_utils_resampling.py
--rw-r--r--   0 runner    (1001) docker     (123)    47326 2023-06-21 14:28:54.000000 DoubleML-0.6.2/doubleml/datasets.py
--rw-r--r--   0 runner    (1001) docker     (123)    83209 2023-06-21 14:28:54.000000 DoubleML-0.6.2/doubleml/double_ml.py
--rw-r--r--   0 runner    (1001) docker     (123)     8137 2023-06-21 14:28:54.000000 DoubleML-0.6.2/doubleml/double_ml_blp.py
--rw-r--r--   0 runner    (1001) docker     (123)    16340 2023-06-21 14:28:54.000000 DoubleML-0.6.2/doubleml/double_ml_cvar.py
--rw-r--r--   0 runner    (1001) docker     (123)    37992 2023-06-21 14:28:54.000000 DoubleML-0.6.2/doubleml/double_ml_data.py
--rw-r--r--   0 runner    (1001) docker     (123)    17385 2023-06-21 14:28:54.000000 DoubleML-0.6.2/doubleml/double_ml_did.py
--rw-r--r--   0 runner    (1001) docker     (123)    26082 2023-06-21 14:28:54.000000 DoubleML-0.6.2/doubleml/double_ml_did_cs.py
--rw-r--r--   0 runner    (1001) docker     (123)    22294 2023-06-21 14:28:54.000000 DoubleML-0.6.2/doubleml/double_ml_iivm.py
--rw-r--r--   0 runner    (1001) docker     (123)    20984 2023-06-21 14:28:54.000000 DoubleML-0.6.2/doubleml/double_ml_irm.py
--rw-r--r--   0 runner    (1001) docker     (123)    25935 2023-06-21 14:28:54.000000 DoubleML-0.6.2/doubleml/double_ml_lpq.py
--rw-r--r--   0 runner    (1001) docker     (123)    32893 2023-06-21 14:28:54.000000 DoubleML-0.6.2/doubleml/double_ml_pliv.py
--rw-r--r--   0 runner    (1001) docker     (123)    15561 2023-06-21 14:28:54.000000 DoubleML-0.6.2/doubleml/double_ml_plr.py
--rw-r--r--   0 runner    (1001) docker     (123)    17066 2023-06-21 14:28:54.000000 DoubleML-0.6.2/doubleml/double_ml_pq.py
--rw-r--r--   0 runner    (1001) docker     (123)    30882 2023-06-21 14:28:54.000000 DoubleML-0.6.2/doubleml/double_ml_qte.py
--rw-r--r--   0 runner    (1001) docker     (123)    10102 2023-06-21 14:28:54.000000 DoubleML-0.6.2/doubleml/double_ml_score_mixins.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 14:29:30.087888 DoubleML-0.6.2/doubleml/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-21 14:28:54.000000 DoubleML-0.6.2/doubleml/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2768 2023-06-21 14:28:54.000000 DoubleML-0.6.2/doubleml/tests/_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     1486 2023-06-21 14:28:54.000000 DoubleML-0.6.2/doubleml/tests/_utils_blp_manual.py
--rw-r--r--   0 runner    (1001) docker     (123)     1468 2023-06-21 14:28:54.000000 DoubleML-0.6.2/doubleml/tests/_utils_boot.py
--rw-r--r--   0 runner    (1001) docker     (123)     4421 2023-06-21 14:28:54.000000 DoubleML-0.6.2/doubleml/tests/_utils_cluster.py
--rw-r--r--   0 runner    (1001) docker     (123)     8278 2023-06-21 14:28:54.000000 DoubleML-0.6.2/doubleml/tests/_utils_cvar_manual.py
--rw-r--r--   0 runner    (1001) docker     (123)    17870 2023-06-21 14:28:54.000000 DoubleML-0.6.2/doubleml/tests/_utils_did_cs_manual.py
--rw-r--r--   0 runner    (1001) docker     (123)    10877 2023-06-21 14:28:54.000000 DoubleML-0.6.2/doubleml/tests/_utils_did_manual.py
--rw-r--r--   0 runner    (1001) docker     (123)     4839 2023-06-21 14:28:54.000000 DoubleML-0.6.2/doubleml/tests/_utils_dml_cv_predict.py
--rw-r--r--   0 runner    (1001) docker     (123)     2143 2023-06-21 14:28:54.000000 DoubleML-0.6.2/doubleml/tests/_utils_doubleml_sensitivtiy_manual.py
--rw-r--r--   0 runner    (1001) docker     (123)    13278 2023-06-21 14:28:54.000000 DoubleML-0.6.2/doubleml/tests/_utils_iivm_manual.py
--rw-r--r--   0 runner    (1001) docker     (123)    12850 2023-06-21 14:28:54.000000 DoubleML-0.6.2/doubleml/tests/_utils_irm_manual.py
--rw-r--r--   0 runner    (1001) docker     (123)    14377 2023-06-21 14:28:54.000000 DoubleML-0.6.2/doubleml/tests/_utils_lpq_manual.py
--rw-r--r--   0 runner    (1001) docker     (123)     9759 2023-06-21 14:28:54.000000 DoubleML-0.6.2/doubleml/tests/_utils_pliv_manual.py
--rw-r--r--   0 runner    (1001) docker     (123)     6815 2023-06-21 14:28:54.000000 DoubleML-0.6.2/doubleml/tests/_utils_pliv_partial_x_manual.py
--rw-r--r--   0 runner    (1001) docker     (123)     7049 2023-06-21 14:28:54.000000 DoubleML-0.6.2/doubleml/tests/_utils_pliv_partial_xz_manual.py
--rw-r--r--   0 runner    (1001) docker     (123)     4674 2023-06-21 14:28:54.000000 DoubleML-0.6.2/doubleml/tests/_utils_pliv_partial_z_manual.py
--rw-r--r--   0 runner    (1001) docker     (123)    14846 2023-06-21 14:28:54.000000 DoubleML-0.6.2/doubleml/tests/_utils_plr_manual.py
--rw-r--r--   0 runner    (1001) docker     (123)     8097 2023-06-21 14:28:54.000000 DoubleML-0.6.2/doubleml/tests/_utils_pq_manual.py
--rw-r--r--   0 runner    (1001) docker     (123)     4986 2023-06-21 14:28:54.000000 DoubleML-0.6.2/doubleml/tests/_utils_qte_manual.py
--rw-r--r--   0 runner    (1001) docker     (123)    11826 2023-06-21 14:28:54.000000 DoubleML-0.6.2/doubleml/tests/conftest.py
--rw-r--r--   0 runner    (1001) docker     (123)     5708 2023-06-21 14:28:54.000000 DoubleML-0.6.2/doubleml/tests/test_blp.py
--rw-r--r--   0 runner    (1001) docker     (123)     2868 2023-06-21 14:28:54.000000 DoubleML-0.6.2/doubleml/tests/test_cv_predict.py
--rw-r--r--   0 runner    (1001) docker     (123)     3540 2023-06-21 14:28:54.000000 DoubleML-0.6.2/doubleml/tests/test_cvar.py
--rw-r--r--   0 runner    (1001) docker     (123)     4917 2023-06-21 14:28:54.000000 DoubleML-0.6.2/doubleml/tests/test_cvar_tune.py
--rw-r--r--   0 runner    (1001) docker     (123)     9458 2023-06-21 14:28:54.000000 DoubleML-0.6.2/doubleml/tests/test_datasets.py
--rw-r--r--   0 runner    (1001) docker     (123)     7858 2023-06-21 14:28:54.000000 DoubleML-0.6.2/doubleml/tests/test_did.py
--rw-r--r--   0 runner    (1001) docker     (123)     8142 2023-06-21 14:28:54.000000 DoubleML-0.6.2/doubleml/tests/test_did_cs.py
--rw-r--r--   0 runner    (1001) docker     (123)     6300 2023-06-21 14:28:54.000000 DoubleML-0.6.2/doubleml/tests/test_did_cs_tune.py
--rw-r--r--   0 runner    (1001) docker     (123)     5834 2023-06-21 14:28:54.000000 DoubleML-0.6.2/doubleml/tests/test_did_tune.py
--rw-r--r--   0 runner    (1001) docker     (123)    29385 2023-06-21 14:28:54.000000 DoubleML-0.6.2/doubleml/tests/test_dml_data.py
--rw-r--r--   0 runner    (1001) docker     (123)     2841 2023-06-21 14:28:54.000000 DoubleML-0.6.2/doubleml/tests/test_doubleml_evaluate_learner.py
--rw-r--r--   0 runner    (1001) docker     (123)    65581 2023-06-21 14:28:54.000000 DoubleML-0.6.2/doubleml/tests/test_doubleml_exceptions.py
--rw-r--r--   0 runner    (1001) docker     (123)     6054 2023-06-21 14:28:54.000000 DoubleML-0.6.2/doubleml/tests/test_doubleml_model_defaults.py
--rw-r--r--   0 runner    (1001) docker     (123)    18257 2023-06-21 14:28:54.000000 DoubleML-0.6.2/doubleml/tests/test_doubleml_return_types.py
--rw-r--r--   0 runner    (1001) docker     (123)    11176 2023-06-21 14:28:54.000000 DoubleML-0.6.2/doubleml/tests/test_doubleml_scores.py
--rw-r--r--   0 runner    (1001) docker     (123)     3048 2023-06-21 14:28:54.000000 DoubleML-0.6.2/doubleml/tests/test_doubleml_sensitivity.py
--rw-r--r--   0 runner    (1001) docker     (123)     5076 2023-06-21 14:28:54.000000 DoubleML-0.6.2/doubleml/tests/test_doubleml_sensitivity_cluster.py
--rw-r--r--   0 runner    (1001) docker     (123)     3915 2023-06-21 14:28:54.000000 DoubleML-0.6.2/doubleml/tests/test_doubleml_set_ml_nuisance_params.py
--rw-r--r--   0 runner    (1001) docker     (123)    12535 2023-06-21 14:28:54.000000 DoubleML-0.6.2/doubleml/tests/test_doubleml_set_sample_splitting.py
--rw-r--r--   0 runner    (1001) docker     (123)     4980 2023-06-21 14:28:54.000000 DoubleML-0.6.2/doubleml/tests/test_iivm.py
--rw-r--r--   0 runner    (1001) docker     (123)     4714 2023-06-21 14:28:54.000000 DoubleML-0.6.2/doubleml/tests/test_iivm_classifier.py
--rw-r--r--   0 runner    (1001) docker     (123)     4744 2023-06-21 14:28:54.000000 DoubleML-0.6.2/doubleml/tests/test_iivm_no_cross_fit.py
--rw-r--r--   0 runner    (1001) docker     (123)     5805 2023-06-21 14:28:54.000000 DoubleML-0.6.2/doubleml/tests/test_iivm_subgroups.py
--rw-r--r--   0 runner    (1001) docker     (123)     7284 2023-06-21 14:28:54.000000 DoubleML-0.6.2/doubleml/tests/test_iivm_tune.py
--rw-r--r--   0 runner    (1001) docker     (123)     8259 2023-06-21 14:28:54.000000 DoubleML-0.6.2/doubleml/tests/test_irm.py
--rw-r--r--   0 runner    (1001) docker     (123)     4693 2023-06-21 14:28:54.000000 DoubleML-0.6.2/doubleml/tests/test_irm_classifier.py
--rw-r--r--   0 runner    (1001) docker     (123)     4569 2023-06-21 14:28:54.000000 DoubleML-0.6.2/doubleml/tests/test_irm_no_cross_fit.py
--rw-r--r--   0 runner    (1001) docker     (123)     5984 2023-06-21 14:28:54.000000 DoubleML-0.6.2/doubleml/tests/test_irm_tune.py
--rw-r--r--   0 runner    (1001) docker     (123)     5955 2023-06-21 14:28:54.000000 DoubleML-0.6.2/doubleml/tests/test_irm_with_missings.py
--rw-r--r--   0 runner    (1001) docker     (123)     4663 2023-06-21 14:28:54.000000 DoubleML-0.6.2/doubleml/tests/test_lpq.py
--rw-r--r--   0 runner    (1001) docker     (123)     6136 2023-06-21 14:28:54.000000 DoubleML-0.6.2/doubleml/tests/test_lpq_tune.py
--rw-r--r--   0 runner    (1001) docker     (123)    13954 2023-06-21 14:28:54.000000 DoubleML-0.6.2/doubleml/tests/test_multiway_cluster.py
--rw-r--r--   0 runner    (1001) docker     (123)    10468 2023-06-21 14:28:54.000000 DoubleML-0.6.2/doubleml/tests/test_nonlinear_cluster.py
--rw-r--r--   0 runner    (1001) docker     (123)    11256 2023-06-21 14:28:54.000000 DoubleML-0.6.2/doubleml/tests/test_nonlinear_score_mixin.py
--rw-r--r--   0 runner    (1001) docker     (123)      131 2023-06-21 14:28:54.000000 DoubleML-0.6.2/doubleml/tests/test_package.py
--rw-r--r--   0 runner    (1001) docker     (123)     4446 2023-06-21 14:28:54.000000 DoubleML-0.6.2/doubleml/tests/test_pliv.py
--rw-r--r--   0 runner    (1001) docker     (123)     4420 2023-06-21 14:28:54.000000 DoubleML-0.6.2/doubleml/tests/test_pliv_no_cross_fit.py
--rw-r--r--   0 runner    (1001) docker     (123)     3848 2023-06-21 14:28:54.000000 DoubleML-0.6.2/doubleml/tests/test_pliv_partial_x.py
--rw-r--r--   0 runner    (1001) docker     (123)     6642 2023-06-21 14:28:54.000000 DoubleML-0.6.2/doubleml/tests/test_pliv_partial_x_tune.py
--rw-r--r--   0 runner    (1001) docker     (123)     3855 2023-06-21 14:28:54.000000 DoubleML-0.6.2/doubleml/tests/test_pliv_partial_xz.py
--rw-r--r--   0 runner    (1001) docker     (123)     6702 2023-06-21 14:28:54.000000 DoubleML-0.6.2/doubleml/tests/test_pliv_partial_xz_tune.py
--rw-r--r--   0 runner    (1001) docker     (123)     3847 2023-06-21 14:28:54.000000 DoubleML-0.6.2/doubleml/tests/test_pliv_partial_z.py
--rw-r--r--   0 runner    (1001) docker     (123)     5114 2023-06-21 14:28:54.000000 DoubleML-0.6.2/doubleml/tests/test_pliv_partial_z_tune.py
--rw-r--r--   0 runner    (1001) docker     (123)     6290 2023-06-21 14:28:54.000000 DoubleML-0.6.2/doubleml/tests/test_pliv_tune.py
--rw-r--r--   0 runner    (1001) docker     (123)    10810 2023-06-21 14:28:54.000000 DoubleML-0.6.2/doubleml/tests/test_plr.py
--rw-r--r--   0 runner    (1001) docker     (123)     3968 2023-06-21 14:28:54.000000 DoubleML-0.6.2/doubleml/tests/test_plr_classifier.py
--rw-r--r--   0 runner    (1001) docker     (123)     6229 2023-06-21 14:28:54.000000 DoubleML-0.6.2/doubleml/tests/test_plr_multi_treat.py
--rw-r--r--   0 runner    (1001) docker     (123)    13395 2023-06-21 14:28:54.000000 DoubleML-0.6.2/doubleml/tests/test_plr_no_cross_fit.py
--rw-r--r--   0 runner    (1001) docker     (123)     2576 2023-06-21 14:28:54.000000 DoubleML-0.6.2/doubleml/tests/test_plr_reestimate_from_scores.py
--rw-r--r--   0 runner    (1001) docker     (123)     3970 2023-06-21 14:28:54.000000 DoubleML-0.6.2/doubleml/tests/test_plr_rep_cross.py
--rw-r--r--   0 runner    (1001) docker     (123)     4002 2023-06-21 14:28:54.000000 DoubleML-0.6.2/doubleml/tests/test_plr_set_ml_nuisance_pars.py
--rw-r--r--   0 runner    (1001) docker     (123)     2480 2023-06-21 14:28:54.000000 DoubleML-0.6.2/doubleml/tests/test_plr_set_smpls_externally.py
--rw-r--r--   0 runner    (1001) docker     (123)     5856 2023-06-21 14:28:54.000000 DoubleML-0.6.2/doubleml/tests/test_plr_tune.py
--rw-r--r--   0 runner    (1001) docker     (123)     3152 2023-06-21 14:28:54.000000 DoubleML-0.6.2/doubleml/tests/test_pq.py
--rw-r--r--   0 runner    (1001) docker     (123)     4727 2023-06-21 14:28:54.000000 DoubleML-0.6.2/doubleml/tests/test_pq_tune.py
--rw-r--r--   0 runner    (1001) docker     (123)     6453 2023-06-21 14:28:54.000000 DoubleML-0.6.2/doubleml/tests/test_qte.py
--rw-r--r--   0 runner    (1001) docker     (123)      138 2023-06-21 14:28:54.000000 DoubleML-0.6.2/pytest.ini
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-21 14:29:30.087888 DoubleML-0.6.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1415 2023-06-21 14:28:54.000000 DoubleML-0.6.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 12:41:17.604149 DoubleML-0.6.3/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 12:41:17.580147 DoubleML-0.6.3/DoubleML.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     8771 2023-06-26 12:41:17.000000 DoubleML-0.6.3/DoubleML.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3603 2023-06-26 12:41:17.000000 DoubleML-0.6.3/DoubleML.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-26 12:41:17.000000 DoubleML-0.6.3/DoubleML.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       58 2023-06-26 12:41:17.000000 DoubleML-0.6.3/DoubleML.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        9 2023-06-26 12:41:17.000000 DoubleML-0.6.3/DoubleML.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1583 2023-06-26 12:40:34.000000 DoubleML-0.6.3/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       34 2023-06-26 12:40:34.000000 DoubleML-0.6.3/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     8771 2023-06-26 12:41:17.604149 DoubleML-0.6.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     6648 2023-06-26 12:40:34.000000 DoubleML-0.6.3/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 12:41:17.588148 DoubleML-0.6.3/doubleml/
+-rw-r--r--   0 runner    (1001) docker     (123)      948 2023-06-26 12:40:34.000000 DoubleML-0.6.3/doubleml/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13825 2023-06-26 12:40:34.000000 DoubleML-0.6.3/doubleml/_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8740 2023-06-26 12:40:34.000000 DoubleML-0.6.3/doubleml/_utils_checks.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2810 2023-06-26 12:40:34.000000 DoubleML-0.6.3/doubleml/_utils_plots.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4818 2023-06-26 12:40:34.000000 DoubleML-0.6.3/doubleml/_utils_resampling.py
+-rw-r--r--   0 runner    (1001) docker     (123)    47328 2023-06-26 12:40:34.000000 DoubleML-0.6.3/doubleml/datasets.py
+-rw-r--r--   0 runner    (1001) docker     (123)    83209 2023-06-26 12:40:34.000000 DoubleML-0.6.3/doubleml/double_ml.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8137 2023-06-26 12:40:34.000000 DoubleML-0.6.3/doubleml/double_ml_blp.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16340 2023-06-26 12:40:34.000000 DoubleML-0.6.3/doubleml/double_ml_cvar.py
+-rw-r--r--   0 runner    (1001) docker     (123)    37992 2023-06-26 12:40:34.000000 DoubleML-0.6.3/doubleml/double_ml_data.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17385 2023-06-26 12:40:34.000000 DoubleML-0.6.3/doubleml/double_ml_did.py
+-rw-r--r--   0 runner    (1001) docker     (123)    26082 2023-06-26 12:40:34.000000 DoubleML-0.6.3/doubleml/double_ml_did_cs.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22294 2023-06-26 12:40:34.000000 DoubleML-0.6.3/doubleml/double_ml_iivm.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20984 2023-06-26 12:40:34.000000 DoubleML-0.6.3/doubleml/double_ml_irm.py
+-rw-r--r--   0 runner    (1001) docker     (123)    25935 2023-06-26 12:40:34.000000 DoubleML-0.6.3/doubleml/double_ml_lpq.py
+-rw-r--r--   0 runner    (1001) docker     (123)    32893 2023-06-26 12:40:34.000000 DoubleML-0.6.3/doubleml/double_ml_pliv.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15561 2023-06-26 12:40:34.000000 DoubleML-0.6.3/doubleml/double_ml_plr.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17066 2023-06-26 12:40:34.000000 DoubleML-0.6.3/doubleml/double_ml_pq.py
+-rw-r--r--   0 runner    (1001) docker     (123)    30882 2023-06-26 12:40:34.000000 DoubleML-0.6.3/doubleml/double_ml_qte.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10102 2023-06-26 12:40:34.000000 DoubleML-0.6.3/doubleml/double_ml_score_mixins.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 12:41:17.604149 DoubleML-0.6.3/doubleml/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-26 12:40:34.000000 DoubleML-0.6.3/doubleml/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2768 2023-06-26 12:40:34.000000 DoubleML-0.6.3/doubleml/tests/_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1486 2023-06-26 12:40:34.000000 DoubleML-0.6.3/doubleml/tests/_utils_blp_manual.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1468 2023-06-26 12:40:34.000000 DoubleML-0.6.3/doubleml/tests/_utils_boot.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4421 2023-06-26 12:40:34.000000 DoubleML-0.6.3/doubleml/tests/_utils_cluster.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8278 2023-06-26 12:40:34.000000 DoubleML-0.6.3/doubleml/tests/_utils_cvar_manual.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17870 2023-06-26 12:40:34.000000 DoubleML-0.6.3/doubleml/tests/_utils_did_cs_manual.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10877 2023-06-26 12:40:34.000000 DoubleML-0.6.3/doubleml/tests/_utils_did_manual.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4839 2023-06-26 12:40:34.000000 DoubleML-0.6.3/doubleml/tests/_utils_dml_cv_predict.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2143 2023-06-26 12:40:34.000000 DoubleML-0.6.3/doubleml/tests/_utils_doubleml_sensitivtiy_manual.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13278 2023-06-26 12:40:34.000000 DoubleML-0.6.3/doubleml/tests/_utils_iivm_manual.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12850 2023-06-26 12:40:34.000000 DoubleML-0.6.3/doubleml/tests/_utils_irm_manual.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14377 2023-06-26 12:40:34.000000 DoubleML-0.6.3/doubleml/tests/_utils_lpq_manual.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9759 2023-06-26 12:40:34.000000 DoubleML-0.6.3/doubleml/tests/_utils_pliv_manual.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6815 2023-06-26 12:40:34.000000 DoubleML-0.6.3/doubleml/tests/_utils_pliv_partial_x_manual.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7049 2023-06-26 12:40:34.000000 DoubleML-0.6.3/doubleml/tests/_utils_pliv_partial_xz_manual.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4674 2023-06-26 12:40:34.000000 DoubleML-0.6.3/doubleml/tests/_utils_pliv_partial_z_manual.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14846 2023-06-26 12:40:34.000000 DoubleML-0.6.3/doubleml/tests/_utils_plr_manual.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8097 2023-06-26 12:40:34.000000 DoubleML-0.6.3/doubleml/tests/_utils_pq_manual.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4986 2023-06-26 12:40:34.000000 DoubleML-0.6.3/doubleml/tests/_utils_qte_manual.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11826 2023-06-26 12:40:34.000000 DoubleML-0.6.3/doubleml/tests/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5708 2023-06-26 12:40:34.000000 DoubleML-0.6.3/doubleml/tests/test_blp.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2868 2023-06-26 12:40:34.000000 DoubleML-0.6.3/doubleml/tests/test_cv_predict.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3540 2023-06-26 12:40:34.000000 DoubleML-0.6.3/doubleml/tests/test_cvar.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4917 2023-06-26 12:40:34.000000 DoubleML-0.6.3/doubleml/tests/test_cvar_tune.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9458 2023-06-26 12:40:34.000000 DoubleML-0.6.3/doubleml/tests/test_datasets.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7858 2023-06-26 12:40:34.000000 DoubleML-0.6.3/doubleml/tests/test_did.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8142 2023-06-26 12:40:34.000000 DoubleML-0.6.3/doubleml/tests/test_did_cs.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6300 2023-06-26 12:40:34.000000 DoubleML-0.6.3/doubleml/tests/test_did_cs_tune.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5834 2023-06-26 12:40:34.000000 DoubleML-0.6.3/doubleml/tests/test_did_tune.py
+-rw-r--r--   0 runner    (1001) docker     (123)    29385 2023-06-26 12:40:34.000000 DoubleML-0.6.3/doubleml/tests/test_dml_data.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2841 2023-06-26 12:40:34.000000 DoubleML-0.6.3/doubleml/tests/test_doubleml_evaluate_learner.py
+-rw-r--r--   0 runner    (1001) docker     (123)    65581 2023-06-26 12:40:34.000000 DoubleML-0.6.3/doubleml/tests/test_doubleml_exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6054 2023-06-26 12:40:34.000000 DoubleML-0.6.3/doubleml/tests/test_doubleml_model_defaults.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18257 2023-06-26 12:40:34.000000 DoubleML-0.6.3/doubleml/tests/test_doubleml_return_types.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11176 2023-06-26 12:40:34.000000 DoubleML-0.6.3/doubleml/tests/test_doubleml_scores.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3048 2023-06-26 12:40:34.000000 DoubleML-0.6.3/doubleml/tests/test_doubleml_sensitivity.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5076 2023-06-26 12:40:34.000000 DoubleML-0.6.3/doubleml/tests/test_doubleml_sensitivity_cluster.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3915 2023-06-26 12:40:34.000000 DoubleML-0.6.3/doubleml/tests/test_doubleml_set_ml_nuisance_params.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12535 2023-06-26 12:40:34.000000 DoubleML-0.6.3/doubleml/tests/test_doubleml_set_sample_splitting.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4980 2023-06-26 12:40:34.000000 DoubleML-0.6.3/doubleml/tests/test_iivm.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4714 2023-06-26 12:40:34.000000 DoubleML-0.6.3/doubleml/tests/test_iivm_classifier.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4744 2023-06-26 12:40:34.000000 DoubleML-0.6.3/doubleml/tests/test_iivm_no_cross_fit.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5805 2023-06-26 12:40:34.000000 DoubleML-0.6.3/doubleml/tests/test_iivm_subgroups.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7284 2023-06-26 12:40:34.000000 DoubleML-0.6.3/doubleml/tests/test_iivm_tune.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8259 2023-06-26 12:40:34.000000 DoubleML-0.6.3/doubleml/tests/test_irm.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4693 2023-06-26 12:40:34.000000 DoubleML-0.6.3/doubleml/tests/test_irm_classifier.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4569 2023-06-26 12:40:34.000000 DoubleML-0.6.3/doubleml/tests/test_irm_no_cross_fit.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5984 2023-06-26 12:40:34.000000 DoubleML-0.6.3/doubleml/tests/test_irm_tune.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5955 2023-06-26 12:40:34.000000 DoubleML-0.6.3/doubleml/tests/test_irm_with_missings.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4663 2023-06-26 12:40:34.000000 DoubleML-0.6.3/doubleml/tests/test_lpq.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6136 2023-06-26 12:40:34.000000 DoubleML-0.6.3/doubleml/tests/test_lpq_tune.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13954 2023-06-26 12:40:34.000000 DoubleML-0.6.3/doubleml/tests/test_multiway_cluster.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10468 2023-06-26 12:40:34.000000 DoubleML-0.6.3/doubleml/tests/test_nonlinear_cluster.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11256 2023-06-26 12:40:34.000000 DoubleML-0.6.3/doubleml/tests/test_nonlinear_score_mixin.py
+-rw-r--r--   0 runner    (1001) docker     (123)      131 2023-06-26 12:40:34.000000 DoubleML-0.6.3/doubleml/tests/test_package.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4446 2023-06-26 12:40:34.000000 DoubleML-0.6.3/doubleml/tests/test_pliv.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4420 2023-06-26 12:40:34.000000 DoubleML-0.6.3/doubleml/tests/test_pliv_no_cross_fit.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3848 2023-06-26 12:40:34.000000 DoubleML-0.6.3/doubleml/tests/test_pliv_partial_x.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6642 2023-06-26 12:40:34.000000 DoubleML-0.6.3/doubleml/tests/test_pliv_partial_x_tune.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3855 2023-06-26 12:40:34.000000 DoubleML-0.6.3/doubleml/tests/test_pliv_partial_xz.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6702 2023-06-26 12:40:34.000000 DoubleML-0.6.3/doubleml/tests/test_pliv_partial_xz_tune.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3847 2023-06-26 12:40:34.000000 DoubleML-0.6.3/doubleml/tests/test_pliv_partial_z.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5114 2023-06-26 12:40:34.000000 DoubleML-0.6.3/doubleml/tests/test_pliv_partial_z_tune.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6290 2023-06-26 12:40:34.000000 DoubleML-0.6.3/doubleml/tests/test_pliv_tune.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10810 2023-06-26 12:40:34.000000 DoubleML-0.6.3/doubleml/tests/test_plr.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3968 2023-06-26 12:40:34.000000 DoubleML-0.6.3/doubleml/tests/test_plr_classifier.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6229 2023-06-26 12:40:34.000000 DoubleML-0.6.3/doubleml/tests/test_plr_multi_treat.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13395 2023-06-26 12:40:34.000000 DoubleML-0.6.3/doubleml/tests/test_plr_no_cross_fit.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2576 2023-06-26 12:40:34.000000 DoubleML-0.6.3/doubleml/tests/test_plr_reestimate_from_scores.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3970 2023-06-26 12:40:34.000000 DoubleML-0.6.3/doubleml/tests/test_plr_rep_cross.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4002 2023-06-26 12:40:34.000000 DoubleML-0.6.3/doubleml/tests/test_plr_set_ml_nuisance_pars.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2480 2023-06-26 12:40:34.000000 DoubleML-0.6.3/doubleml/tests/test_plr_set_smpls_externally.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5856 2023-06-26 12:40:34.000000 DoubleML-0.6.3/doubleml/tests/test_plr_tune.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3152 2023-06-26 12:40:34.000000 DoubleML-0.6.3/doubleml/tests/test_pq.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4727 2023-06-26 12:40:34.000000 DoubleML-0.6.3/doubleml/tests/test_pq_tune.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6453 2023-06-26 12:40:34.000000 DoubleML-0.6.3/doubleml/tests/test_qte.py
+-rw-r--r--   0 runner    (1001) docker     (123)      138 2023-06-26 12:40:34.000000 DoubleML-0.6.3/pytest.ini
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-26 12:41:17.604149 DoubleML-0.6.3/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1433 2023-06-26 12:40:34.000000 DoubleML-0.6.3/setup.py
```

### Comparing `DoubleML-0.6.2/DoubleML.egg-info/PKG-INFO` & `DoubleML-0.6.3/DoubleML.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: DoubleML
-Version: 0.6.2
+Version: 0.6.3
 Summary: Double Machine Learning in Python
 Home-page: https://docs.doubleml.org
 Author: Bach, P., Chernozhukov, V., Kurz, M. S., and Spindler, M.
 Maintainer: Malte S. Kurz
 Maintainer-email: malte.simon.kurz@uni-hamburg.de
 License: UNKNOWN
 Project-URL: Documentation, https://docs.doubleml.org
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: DoubleML Version: 0.6.2 Summary: Double Machine
+Metadata-Version: 2.1 Name: DoubleML Version: 0.6.3 Summary: Double Machine
 Learning in Python Home-page: https://docs.doubleml.org Author: Bach, P.,
 Chernozhukov, V., Kurz, M. S., and Spindler, M. Maintainer: Malte S. Kurz
 Maintainer-email: malte.simon.kurz@uni-hamburg.de License: UNKNOWN Project-URL:
 Documentation, https://docs.doubleml.org Project-URL: Source Code, https://
 github.com/DoubleML/doubleml-for-py Project-URL: Bug Tracker, https://
 github.com/DoubleML/doubleml-for-py/issues Description: # DoubleML - Double
 Machine Learning in Python [https://raw.githubusercontent.com/DoubleML/
```

### Comparing `DoubleML-0.6.2/DoubleML.egg-info/SOURCES.txt` & `DoubleML-0.6.3/DoubleML.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `DoubleML-0.6.2/LICENSE` & `DoubleML-0.6.3/LICENSE`

 * *Files identical despite different names*

### Comparing `DoubleML-0.6.2/PKG-INFO` & `DoubleML-0.6.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: DoubleML
-Version: 0.6.2
+Version: 0.6.3
 Summary: Double Machine Learning in Python
 Home-page: https://docs.doubleml.org
 Author: Bach, P., Chernozhukov, V., Kurz, M. S., and Spindler, M.
 Maintainer: Malte S. Kurz
 Maintainer-email: malte.simon.kurz@uni-hamburg.de
 License: UNKNOWN
 Project-URL: Documentation, https://docs.doubleml.org
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: DoubleML Version: 0.6.2 Summary: Double Machine
+Metadata-Version: 2.1 Name: DoubleML Version: 0.6.3 Summary: Double Machine
 Learning in Python Home-page: https://docs.doubleml.org Author: Bach, P.,
 Chernozhukov, V., Kurz, M. S., and Spindler, M. Maintainer: Malte S. Kurz
 Maintainer-email: malte.simon.kurz@uni-hamburg.de License: UNKNOWN Project-URL:
 Documentation, https://docs.doubleml.org Project-URL: Source Code, https://
 github.com/DoubleML/doubleml-for-py Project-URL: Bug Tracker, https://
 github.com/DoubleML/doubleml-for-py/issues Description: # DoubleML - Double
 Machine Learning in Python [https://raw.githubusercontent.com/DoubleML/
```

### Comparing `DoubleML-0.6.2/README.md` & `DoubleML-0.6.3/README.md`

 * *Files identical despite different names*

### Comparing `DoubleML-0.6.2/doubleml/__init__.py` & `DoubleML-0.6.3/doubleml/__init__.py`

 * *Files identical despite different names*

### Comparing `DoubleML-0.6.2/doubleml/_utils.py` & `DoubleML-0.6.3/doubleml/_utils.py`

 * *Files identical despite different names*

### Comparing `DoubleML-0.6.2/doubleml/_utils_checks.py` & `DoubleML-0.6.3/doubleml/_utils_checks.py`

 * *Files identical despite different names*

### Comparing `DoubleML-0.6.2/doubleml/_utils_plots.py` & `DoubleML-0.6.3/doubleml/_utils_plots.py`

 * *Files identical despite different names*

### Comparing `DoubleML-0.6.2/doubleml/_utils_resampling.py` & `DoubleML-0.6.3/doubleml/_utils_resampling.py`

 * *Files identical despite different names*

### Comparing `DoubleML-0.6.2/doubleml/datasets.py` & `DoubleML-0.6.3/doubleml/datasets.py`

 * *Files 0% similar despite different names*

```diff
@@ -243,16 +243,16 @@
     **kwargs
         Additional keyword arguments to set non-default values for the parameters
         :math:`\\nu=0`, or :math:`\\gamma=1`.
 
     References
     ----------
     Turrell, A. (2018), Econometrics in Python part I - Double machine learning, Markov Wanderer: A blog on economics,
-    science, coding and data. `http://aeturrell.com/2018/02/10/econometrics-in-python-partI-ML/
-    <http://aeturrell.com/2018/02/10/econometrics-in-python-partI-ML/>`_.
+    science, coding and data. `https://aeturrell.com/blog/posts/econometrics-in-python-parti-ml/
+    <https://aeturrell.com/blog/posts/econometrics-in-python-parti-ml/>`_.
     """
     nu = kwargs.get('nu', 0.)
     gamma = kwargs.get('gamma', 1.)
 
     b = [1 / k for k in range(1, dim_x + 1)]
     sigma = make_spd_matrix(dim_x)
```

### Comparing `DoubleML-0.6.2/doubleml/double_ml.py` & `DoubleML-0.6.3/doubleml/double_ml.py`

 * *Files identical despite different names*

### Comparing `DoubleML-0.6.2/doubleml/double_ml_blp.py` & `DoubleML-0.6.3/doubleml/double_ml_blp.py`

 * *Files identical despite different names*

### Comparing `DoubleML-0.6.2/doubleml/double_ml_cvar.py` & `DoubleML-0.6.3/doubleml/double_ml_cvar.py`

 * *Files identical despite different names*

### Comparing `DoubleML-0.6.2/doubleml/double_ml_data.py` & `DoubleML-0.6.3/doubleml/double_ml_data.py`

 * *Files identical despite different names*

### Comparing `DoubleML-0.6.2/doubleml/double_ml_did.py` & `DoubleML-0.6.3/doubleml/double_ml_did.py`

 * *Files identical despite different names*

### Comparing `DoubleML-0.6.2/doubleml/double_ml_did_cs.py` & `DoubleML-0.6.3/doubleml/double_ml_did_cs.py`

 * *Files identical despite different names*

### Comparing `DoubleML-0.6.2/doubleml/double_ml_iivm.py` & `DoubleML-0.6.3/doubleml/double_ml_iivm.py`

 * *Files identical despite different names*

### Comparing `DoubleML-0.6.2/doubleml/double_ml_irm.py` & `DoubleML-0.6.3/doubleml/double_ml_irm.py`

 * *Files identical despite different names*

### Comparing `DoubleML-0.6.2/doubleml/double_ml_lpq.py` & `DoubleML-0.6.3/doubleml/double_ml_lpq.py`

 * *Files identical despite different names*

### Comparing `DoubleML-0.6.2/doubleml/double_ml_pliv.py` & `DoubleML-0.6.3/doubleml/double_ml_pliv.py`

 * *Files identical despite different names*

### Comparing `DoubleML-0.6.2/doubleml/double_ml_plr.py` & `DoubleML-0.6.3/doubleml/double_ml_plr.py`

 * *Files identical despite different names*

### Comparing `DoubleML-0.6.2/doubleml/double_ml_pq.py` & `DoubleML-0.6.3/doubleml/double_ml_pq.py`

 * *Files identical despite different names*

### Comparing `DoubleML-0.6.2/doubleml/double_ml_qte.py` & `DoubleML-0.6.3/doubleml/double_ml_qte.py`

 * *Files identical despite different names*

### Comparing `DoubleML-0.6.2/doubleml/double_ml_score_mixins.py` & `DoubleML-0.6.3/doubleml/double_ml_score_mixins.py`

 * *Files identical despite different names*

### Comparing `DoubleML-0.6.2/doubleml/tests/_utils.py` & `DoubleML-0.6.3/doubleml/tests/_utils.py`

 * *Files identical despite different names*

### Comparing `DoubleML-0.6.2/doubleml/tests/_utils_blp_manual.py` & `DoubleML-0.6.3/doubleml/tests/_utils_blp_manual.py`

 * *Files identical despite different names*

### Comparing `DoubleML-0.6.2/doubleml/tests/_utils_boot.py` & `DoubleML-0.6.3/doubleml/tests/_utils_boot.py`

 * *Files identical despite different names*

### Comparing `DoubleML-0.6.2/doubleml/tests/_utils_cluster.py` & `DoubleML-0.6.3/doubleml/tests/_utils_cluster.py`

 * *Files identical despite different names*

### Comparing `DoubleML-0.6.2/doubleml/tests/_utils_cvar_manual.py` & `DoubleML-0.6.3/doubleml/tests/_utils_cvar_manual.py`

 * *Files identical despite different names*

### Comparing `DoubleML-0.6.2/doubleml/tests/_utils_did_cs_manual.py` & `DoubleML-0.6.3/doubleml/tests/_utils_did_cs_manual.py`

 * *Files identical despite different names*

### Comparing `DoubleML-0.6.2/doubleml/tests/_utils_did_manual.py` & `DoubleML-0.6.3/doubleml/tests/_utils_did_manual.py`

 * *Files identical despite different names*

### Comparing `DoubleML-0.6.2/doubleml/tests/_utils_dml_cv_predict.py` & `DoubleML-0.6.3/doubleml/tests/_utils_dml_cv_predict.py`

 * *Files identical despite different names*

### Comparing `DoubleML-0.6.2/doubleml/tests/_utils_doubleml_sensitivtiy_manual.py` & `DoubleML-0.6.3/doubleml/tests/_utils_doubleml_sensitivtiy_manual.py`

 * *Files identical despite different names*

### Comparing `DoubleML-0.6.2/doubleml/tests/_utils_iivm_manual.py` & `DoubleML-0.6.3/doubleml/tests/_utils_iivm_manual.py`

 * *Files identical despite different names*

### Comparing `DoubleML-0.6.2/doubleml/tests/_utils_irm_manual.py` & `DoubleML-0.6.3/doubleml/tests/_utils_irm_manual.py`

 * *Files identical despite different names*

### Comparing `DoubleML-0.6.2/doubleml/tests/_utils_lpq_manual.py` & `DoubleML-0.6.3/doubleml/tests/_utils_lpq_manual.py`

 * *Files identical despite different names*

### Comparing `DoubleML-0.6.2/doubleml/tests/_utils_pliv_manual.py` & `DoubleML-0.6.3/doubleml/tests/_utils_pliv_manual.py`

 * *Files identical despite different names*

### Comparing `DoubleML-0.6.2/doubleml/tests/_utils_pliv_partial_x_manual.py` & `DoubleML-0.6.3/doubleml/tests/_utils_pliv_partial_x_manual.py`

 * *Files identical despite different names*

### Comparing `DoubleML-0.6.2/doubleml/tests/_utils_pliv_partial_xz_manual.py` & `DoubleML-0.6.3/doubleml/tests/_utils_pliv_partial_xz_manual.py`

 * *Files identical despite different names*

### Comparing `DoubleML-0.6.2/doubleml/tests/_utils_pliv_partial_z_manual.py` & `DoubleML-0.6.3/doubleml/tests/_utils_pliv_partial_z_manual.py`

 * *Files identical despite different names*

### Comparing `DoubleML-0.6.2/doubleml/tests/_utils_plr_manual.py` & `DoubleML-0.6.3/doubleml/tests/_utils_plr_manual.py`

 * *Files identical despite different names*

### Comparing `DoubleML-0.6.2/doubleml/tests/_utils_pq_manual.py` & `DoubleML-0.6.3/doubleml/tests/_utils_pq_manual.py`

 * *Files identical despite different names*

### Comparing `DoubleML-0.6.2/doubleml/tests/_utils_qte_manual.py` & `DoubleML-0.6.3/doubleml/tests/_utils_qte_manual.py`

 * *Files identical despite different names*

### Comparing `DoubleML-0.6.2/doubleml/tests/conftest.py` & `DoubleML-0.6.3/doubleml/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `DoubleML-0.6.2/doubleml/tests/test_blp.py` & `DoubleML-0.6.3/doubleml/tests/test_blp.py`

 * *Files identical despite different names*

### Comparing `DoubleML-0.6.2/doubleml/tests/test_cv_predict.py` & `DoubleML-0.6.3/doubleml/tests/test_cv_predict.py`

 * *Files identical despite different names*

### Comparing `DoubleML-0.6.2/doubleml/tests/test_cvar.py` & `DoubleML-0.6.3/doubleml/tests/test_cvar.py`

 * *Files identical despite different names*

### Comparing `DoubleML-0.6.2/doubleml/tests/test_cvar_tune.py` & `DoubleML-0.6.3/doubleml/tests/test_cvar_tune.py`

 * *Files identical despite different names*

### Comparing `DoubleML-0.6.2/doubleml/tests/test_datasets.py` & `DoubleML-0.6.3/doubleml/tests/test_datasets.py`

 * *Files identical despite different names*

### Comparing `DoubleML-0.6.2/doubleml/tests/test_did.py` & `DoubleML-0.6.3/doubleml/tests/test_did.py`

 * *Files identical despite different names*

### Comparing `DoubleML-0.6.2/doubleml/tests/test_did_cs.py` & `DoubleML-0.6.3/doubleml/tests/test_did_cs.py`

 * *Files identical despite different names*

### Comparing `DoubleML-0.6.2/doubleml/tests/test_did_cs_tune.py` & `DoubleML-0.6.3/doubleml/tests/test_did_cs_tune.py`

 * *Files identical despite different names*

### Comparing `DoubleML-0.6.2/doubleml/tests/test_did_tune.py` & `DoubleML-0.6.3/doubleml/tests/test_did_tune.py`

 * *Files identical despite different names*

### Comparing `DoubleML-0.6.2/doubleml/tests/test_dml_data.py` & `DoubleML-0.6.3/doubleml/tests/test_dml_data.py`

 * *Files identical despite different names*

### Comparing `DoubleML-0.6.2/doubleml/tests/test_doubleml_evaluate_learner.py` & `DoubleML-0.6.3/doubleml/tests/test_doubleml_evaluate_learner.py`

 * *Files identical despite different names*

### Comparing `DoubleML-0.6.2/doubleml/tests/test_doubleml_exceptions.py` & `DoubleML-0.6.3/doubleml/tests/test_doubleml_exceptions.py`

 * *Files identical despite different names*

### Comparing `DoubleML-0.6.2/doubleml/tests/test_doubleml_model_defaults.py` & `DoubleML-0.6.3/doubleml/tests/test_doubleml_model_defaults.py`

 * *Files identical despite different names*

### Comparing `DoubleML-0.6.2/doubleml/tests/test_doubleml_return_types.py` & `DoubleML-0.6.3/doubleml/tests/test_doubleml_return_types.py`

 * *Files identical despite different names*

### Comparing `DoubleML-0.6.2/doubleml/tests/test_doubleml_scores.py` & `DoubleML-0.6.3/doubleml/tests/test_doubleml_scores.py`

 * *Files identical despite different names*

### Comparing `DoubleML-0.6.2/doubleml/tests/test_doubleml_sensitivity.py` & `DoubleML-0.6.3/doubleml/tests/test_doubleml_sensitivity.py`

 * *Files identical despite different names*

### Comparing `DoubleML-0.6.2/doubleml/tests/test_doubleml_sensitivity_cluster.py` & `DoubleML-0.6.3/doubleml/tests/test_doubleml_sensitivity_cluster.py`

 * *Files identical despite different names*

### Comparing `DoubleML-0.6.2/doubleml/tests/test_doubleml_set_ml_nuisance_params.py` & `DoubleML-0.6.3/doubleml/tests/test_doubleml_set_ml_nuisance_params.py`

 * *Files identical despite different names*

### Comparing `DoubleML-0.6.2/doubleml/tests/test_doubleml_set_sample_splitting.py` & `DoubleML-0.6.3/doubleml/tests/test_doubleml_set_sample_splitting.py`

 * *Files identical despite different names*

### Comparing `DoubleML-0.6.2/doubleml/tests/test_iivm.py` & `DoubleML-0.6.3/doubleml/tests/test_iivm.py`

 * *Files identical despite different names*

### Comparing `DoubleML-0.6.2/doubleml/tests/test_iivm_classifier.py` & `DoubleML-0.6.3/doubleml/tests/test_iivm_classifier.py`

 * *Files identical despite different names*

### Comparing `DoubleML-0.6.2/doubleml/tests/test_iivm_no_cross_fit.py` & `DoubleML-0.6.3/doubleml/tests/test_iivm_no_cross_fit.py`

 * *Files identical despite different names*

### Comparing `DoubleML-0.6.2/doubleml/tests/test_iivm_subgroups.py` & `DoubleML-0.6.3/doubleml/tests/test_iivm_subgroups.py`

 * *Files identical despite different names*

### Comparing `DoubleML-0.6.2/doubleml/tests/test_iivm_tune.py` & `DoubleML-0.6.3/doubleml/tests/test_iivm_tune.py`

 * *Files identical despite different names*

### Comparing `DoubleML-0.6.2/doubleml/tests/test_irm.py` & `DoubleML-0.6.3/doubleml/tests/test_irm.py`

 * *Files identical despite different names*

### Comparing `DoubleML-0.6.2/doubleml/tests/test_irm_classifier.py` & `DoubleML-0.6.3/doubleml/tests/test_irm_classifier.py`

 * *Files identical despite different names*

### Comparing `DoubleML-0.6.2/doubleml/tests/test_irm_no_cross_fit.py` & `DoubleML-0.6.3/doubleml/tests/test_irm_no_cross_fit.py`

 * *Files identical despite different names*

### Comparing `DoubleML-0.6.2/doubleml/tests/test_irm_tune.py` & `DoubleML-0.6.3/doubleml/tests/test_irm_tune.py`

 * *Files identical despite different names*

### Comparing `DoubleML-0.6.2/doubleml/tests/test_irm_with_missings.py` & `DoubleML-0.6.3/doubleml/tests/test_irm_with_missings.py`

 * *Files identical despite different names*

### Comparing `DoubleML-0.6.2/doubleml/tests/test_lpq.py` & `DoubleML-0.6.3/doubleml/tests/test_lpq.py`

 * *Files identical despite different names*

### Comparing `DoubleML-0.6.2/doubleml/tests/test_lpq_tune.py` & `DoubleML-0.6.3/doubleml/tests/test_lpq_tune.py`

 * *Files identical despite different names*

### Comparing `DoubleML-0.6.2/doubleml/tests/test_multiway_cluster.py` & `DoubleML-0.6.3/doubleml/tests/test_multiway_cluster.py`

 * *Files identical despite different names*

### Comparing `DoubleML-0.6.2/doubleml/tests/test_nonlinear_cluster.py` & `DoubleML-0.6.3/doubleml/tests/test_nonlinear_cluster.py`

 * *Files identical despite different names*

### Comparing `DoubleML-0.6.2/doubleml/tests/test_nonlinear_score_mixin.py` & `DoubleML-0.6.3/doubleml/tests/test_nonlinear_score_mixin.py`

 * *Files identical despite different names*

### Comparing `DoubleML-0.6.2/doubleml/tests/test_pliv.py` & `DoubleML-0.6.3/doubleml/tests/test_pliv.py`

 * *Files identical despite different names*

### Comparing `DoubleML-0.6.2/doubleml/tests/test_pliv_no_cross_fit.py` & `DoubleML-0.6.3/doubleml/tests/test_pliv_no_cross_fit.py`

 * *Files identical despite different names*

### Comparing `DoubleML-0.6.2/doubleml/tests/test_pliv_partial_x.py` & `DoubleML-0.6.3/doubleml/tests/test_pliv_partial_x.py`

 * *Files identical despite different names*

### Comparing `DoubleML-0.6.2/doubleml/tests/test_pliv_partial_x_tune.py` & `DoubleML-0.6.3/doubleml/tests/test_pliv_partial_x_tune.py`

 * *Files identical despite different names*

### Comparing `DoubleML-0.6.2/doubleml/tests/test_pliv_partial_xz.py` & `DoubleML-0.6.3/doubleml/tests/test_pliv_partial_xz.py`

 * *Files identical despite different names*

### Comparing `DoubleML-0.6.2/doubleml/tests/test_pliv_partial_xz_tune.py` & `DoubleML-0.6.3/doubleml/tests/test_pliv_partial_xz_tune.py`

 * *Files identical despite different names*

### Comparing `DoubleML-0.6.2/doubleml/tests/test_pliv_partial_z.py` & `DoubleML-0.6.3/doubleml/tests/test_pliv_partial_z.py`

 * *Files identical despite different names*

### Comparing `DoubleML-0.6.2/doubleml/tests/test_pliv_partial_z_tune.py` & `DoubleML-0.6.3/doubleml/tests/test_pliv_partial_z_tune.py`

 * *Files identical despite different names*

### Comparing `DoubleML-0.6.2/doubleml/tests/test_pliv_tune.py` & `DoubleML-0.6.3/doubleml/tests/test_pliv_tune.py`

 * *Files identical despite different names*

### Comparing `DoubleML-0.6.2/doubleml/tests/test_plr.py` & `DoubleML-0.6.3/doubleml/tests/test_plr.py`

 * *Files identical despite different names*

### Comparing `DoubleML-0.6.2/doubleml/tests/test_plr_classifier.py` & `DoubleML-0.6.3/doubleml/tests/test_plr_classifier.py`

 * *Files identical despite different names*

### Comparing `DoubleML-0.6.2/doubleml/tests/test_plr_multi_treat.py` & `DoubleML-0.6.3/doubleml/tests/test_plr_multi_treat.py`

 * *Files identical despite different names*

### Comparing `DoubleML-0.6.2/doubleml/tests/test_plr_no_cross_fit.py` & `DoubleML-0.6.3/doubleml/tests/test_plr_no_cross_fit.py`

 * *Files identical despite different names*

### Comparing `DoubleML-0.6.2/doubleml/tests/test_plr_reestimate_from_scores.py` & `DoubleML-0.6.3/doubleml/tests/test_plr_reestimate_from_scores.py`

 * *Files identical despite different names*

### Comparing `DoubleML-0.6.2/doubleml/tests/test_plr_rep_cross.py` & `DoubleML-0.6.3/doubleml/tests/test_plr_rep_cross.py`

 * *Files identical despite different names*

### Comparing `DoubleML-0.6.2/doubleml/tests/test_plr_set_ml_nuisance_pars.py` & `DoubleML-0.6.3/doubleml/tests/test_plr_set_ml_nuisance_pars.py`

 * *Files identical despite different names*

### Comparing `DoubleML-0.6.2/doubleml/tests/test_plr_set_smpls_externally.py` & `DoubleML-0.6.3/doubleml/tests/test_plr_set_smpls_externally.py`

 * *Files identical despite different names*

### Comparing `DoubleML-0.6.2/doubleml/tests/test_plr_tune.py` & `DoubleML-0.6.3/doubleml/tests/test_plr_tune.py`

 * *Files identical despite different names*

### Comparing `DoubleML-0.6.2/doubleml/tests/test_pq.py` & `DoubleML-0.6.3/doubleml/tests/test_pq.py`

 * *Files identical despite different names*

### Comparing `DoubleML-0.6.2/doubleml/tests/test_pq_tune.py` & `DoubleML-0.6.3/doubleml/tests/test_pq_tune.py`

 * *Files identical despite different names*

### Comparing `DoubleML-0.6.2/doubleml/tests/test_qte.py` & `DoubleML-0.6.3/doubleml/tests/test_qte.py`

 * *Files identical despite different names*

### Comparing `DoubleML-0.6.2/setup.py` & `DoubleML-0.6.3/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -7,15 +7,15 @@
     'Documentation': 'https://docs.doubleml.org',
     'Source Code': 'https://github.com/DoubleML/doubleml-for-py',
     'Bug Tracker': 'https://github.com/DoubleML/doubleml-for-py/issues',
 }
 
 setup(
     name='DoubleML',
-    version='0.6.2',
+    version='0.6.3',
     author='Bach, P., Chernozhukov, V., Kurz, M. S., and Spindler, M.',
     maintainer='Malte S. Kurz',
     maintainer_email='malte.simon.kurz@uni-hamburg.de',
     description='Double Machine Learning in Python',
     long_description=long_description,
     long_description_content_type='text/markdown',
     url='https://docs.doubleml.org',
@@ -24,14 +24,15 @@
     install_requires=[
         'joblib',
         'numpy',
         'pandas',
         'scipy',
         'scikit-learn',
         'statsmodels',
+        'plotly',
     ],
     python_requires=">=3.6",
     classifiers=[
         'Programming Language :: Python :: 3',
         'Programming Language :: Python :: 3.6',
         'Programming Language :: Python :: 3.7',
         'Programming Language :: Python :: 3.8',
```

