# Comparing `tmp/autooc-0.0.8.tar.gz` & `tmp/autooc-0.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "autooc-0.0.8.tar", last modified: Sat Jun 24 15:15:01 2023, max compression
+gzip compressed data, was "autooc-0.0.9.tar", last modified: Sat Jun 24 15:25:55 2023, max compression
```

## Comparing `autooc-0.0.8.tar` & `autooc-0.0.9.tar`

### file list

```diff
@@ -1,111 +1,121 @@
-drwxr-xr-x   0 luis      (1000) luis      (1000)        0 2023-06-24 15:15:01.158877 autooc-0.0.8/
--rw-r--r--   0 luis      (1000) luis      (1000)     1071 2023-06-24 14:17:33.000000 autooc-0.0.8/LICENSE
--rw-r--r--   0 luis      (1000) luis      (1000)       42 2023-06-24 14:17:33.000000 autooc-0.0.8/MANIFEST.in
--rw-r--r--   0 luis      (1000) luis      (1000)    12349 2023-06-24 15:15:01.158877 autooc-0.0.8/PKG-INFO
--rw-r--r--   0 luis      (1000) luis      (1000)    11738 2023-06-24 14:29:17.000000 autooc-0.0.8/README.md
-drwxr-xr-x   0 luis      (1000) luis      (1000)        0 2023-06-24 15:15:01.138877 autooc-0.0.8/autooc/
--rw-r--r--   0 luis      (1000) luis      (1000)        0 2023-06-24 14:17:34.000000 autooc-0.0.8/autooc/__init__.py
-drwxr-xr-x   0 luis      (1000) luis      (1000)        0 2023-06-24 15:15:01.138877 autooc-0.0.8/autooc/algorithm/
--rw-r--r--   0 luis      (1000) luis      (1000)        0 2023-06-24 14:17:34.000000 autooc-0.0.8/autooc/algorithm/__init__.py
-drwxr-xr-x   0 luis      (1000) luis      (1000)        0 2023-06-24 15:15:01.138877 autooc-0.0.8/autooc/algorithm/distributed_algorithm/
--rw-r--r--   0 luis      (1000) luis      (1000)        0 2023-06-24 14:17:34.000000 autooc-0.0.8/autooc/algorithm/distributed_algorithm/__init__.py
--rw-r--r--   0 luis      (1000) luis      (1000)      994 2023-06-24 14:17:34.000000 autooc-0.0.8/autooc/algorithm/distributed_algorithm/search_loop.py
--rw-r--r--   0 luis      (1000) luis      (1000)      426 2023-06-24 14:17:34.000000 autooc-0.0.8/autooc/algorithm/distributed_algorithm/step.py
--rw-r--r--   0 luis      (1000) luis      (1000)     9888 2023-06-24 14:17:34.000000 autooc-0.0.8/autooc/algorithm/hill_climbing.py
--rw-r--r--   0 luis      (1000) luis      (1000)    11897 2023-06-24 14:17:34.000000 autooc-0.0.8/autooc/algorithm/mapper.py
--rw-r--r--   0 luis      (1000) luis      (1000)    13826 2023-06-24 14:17:34.000000 autooc-0.0.8/autooc/algorithm/parameters.py
--rw-r--r--   0 luis      (1000) luis      (1000)     2460 2023-06-24 14:17:34.000000 autooc-0.0.8/autooc/algorithm/search_loop.py
--rw-r--r--   0 luis      (1000) luis      (1000)     1643 2023-06-24 14:17:34.000000 autooc-0.0.8/autooc/algorithm/step.py
--rw-r--r--   0 luis      (1000) luis      (1000)    25075 2023-06-24 15:14:49.000000 autooc-0.0.8/autooc/autooc.py
-drwxr-xr-x   0 luis      (1000) luis      (1000)        0 2023-06-24 15:15:01.138877 autooc-0.0.8/autooc/fitness/
--rw-r--r--   0 luis      (1000) luis      (1000)        0 2023-06-24 14:17:34.000000 autooc-0.0.8/autooc/fitness/__init__.py
-drwxr-xr-x   0 luis      (1000) luis      (1000)        0 2023-06-24 15:15:01.138877 autooc-0.0.8/autooc/fitness/base_ff_classes/
--rw-r--r--   0 luis      (1000) luis      (1000)        0 2023-06-24 14:17:34.000000 autooc-0.0.8/autooc/fitness/base_ff_classes/__init__.py
--rw-r--r--   0 luis      (1000) luis      (1000)     2130 2023-06-24 14:17:34.000000 autooc-0.0.8/autooc/fitness/base_ff_classes/base_ff.py
--rw-r--r--   0 luis      (1000) luis      (1000)     2587 2023-06-24 14:17:34.000000 autooc-0.0.8/autooc/fitness/base_ff_classes/ff_template.py
--rw-r--r--   0 luis      (1000) luis      (1000)     2662 2023-06-24 14:17:34.000000 autooc-0.0.8/autooc/fitness/base_ff_classes/moo_ff.py
--rw-r--r--   0 luis      (1000) luis      (1000)      484 2023-06-24 14:17:34.000000 autooc-0.0.8/autooc/fitness/bic.py
--rw-r--r--   0 luis      (1000) luis      (1000)     5108 2023-06-24 14:17:34.000000 autooc-0.0.8/autooc/fitness/evaluation.py
--rw-r--r--   0 luis      (1000) luis      (1000)      362 2023-06-24 14:17:34.000000 autooc-0.0.8/autooc/fitness/minimise_nodes.py
-drwxr-xr-x   0 luis      (1000) luis      (1000)        0 2023-06-24 15:15:01.138877 autooc-0.0.8/autooc/fitness/multi_objective/
--rw-r--r--   0 luis      (1000) luis      (1000)        0 2023-06-24 14:17:34.000000 autooc-0.0.8/autooc/fitness/multi_objective/__init__.py
--rw-r--r--   0 luis      (1000) luis      (1000)      796 2023-06-24 14:17:34.000000 autooc-0.0.8/autooc/fitness/multi_objective/binary_phenotype_to_float.py
--rw-r--r--   0 luis      (1000) luis      (1000)     3944 2023-06-24 14:17:34.000000 autooc-0.0.8/autooc/fitness/multi_objective/singlefit_autoencoders.py
--rw-r--r--   0 luis      (1000) luis      (1000)     1845 2023-06-24 14:17:34.000000 autooc-0.0.8/autooc/fitness/multi_objective/singlefit_multiobj.py
--rw-r--r--   0 luis      (1000) luis      (1000)     1007 2023-06-24 14:17:34.000000 autooc-0.0.8/autooc/fitness/multi_objective/zdt1.py
--rw-r--r--   0 luis      (1000) luis      (1000)      407 2023-06-24 14:17:34.000000 autooc-0.0.8/autooc/fitness/num_params.py
--rw-r--r--   0 luis      (1000) luis      (1000)      403 2023-06-24 14:17:34.000000 autooc-0.0.8/autooc/fitness/predict_time.py
--rw-r--r--   0 luis      (1000) luis      (1000)     6022 2023-06-24 14:17:34.000000 autooc-0.0.8/autooc/fitness/progsys.py
--rw-r--r--   0 luis      (1000) luis      (1000)     1337 2023-06-24 14:17:34.000000 autooc-0.0.8/autooc/fitness/pymax.py
--rw-r--r--   0 luis      (1000) luis      (1000)     5886 2023-06-24 14:17:34.000000 autooc-0.0.8/autooc/fitness/sequence_match.py
--rw-r--r--   0 luis      (1000) luis      (1000)     1038 2023-06-24 14:17:34.000000 autooc-0.0.8/autooc/fitness/string_match.py
-drwxr-xr-x   0 luis      (1000) luis      (1000)        0 2023-06-24 15:15:01.148877 autooc-0.0.8/autooc/fitness/supervised_learning/
--rw-r--r--   0 luis      (1000) luis      (1000)        0 2023-06-24 14:17:34.000000 autooc-0.0.8/autooc/fitness/supervised_learning/__init__.py
--rw-r--r--   0 luis      (1000) luis      (1000)     3731 2023-06-24 14:17:34.000000 autooc-0.0.8/autooc/fitness/supervised_learning/boolean_problem.py
--rw-r--r--   0 luis      (1000) luis      (1000)      659 2023-06-24 14:17:34.000000 autooc-0.0.8/autooc/fitness/supervised_learning/classification.py
--rw-r--r--   0 luis      (1000) luis      (1000)     2912 2023-06-24 14:17:34.000000 autooc-0.0.8/autooc/fitness/supervised_learning/if_else_classifier.py
--rw-r--r--   0 luis      (1000) luis      (1000)      643 2023-06-24 14:17:34.000000 autooc-0.0.8/autooc/fitness/supervised_learning/regression.py
--rw-r--r--   0 luis      (1000) luis      (1000)     4478 2023-06-24 14:17:34.000000 autooc-0.0.8/autooc/fitness/supervised_learning/regression_random_polynomial.py
--rw-r--r--   0 luis      (1000) luis      (1000)    10335 2023-06-24 14:17:34.000000 autooc-0.0.8/autooc/fitness/supervised_learning/supervised_learning.py
--rw-r--r--   0 luis      (1000) luis      (1000)     3627 2023-06-24 14:17:34.000000 autooc-0.0.8/autooc/fitness/supervised_learning/supervised_learning_backup.py
--rw-r--r--   0 luis      (1000) luis      (1000)      406 2023-06-24 14:17:34.000000 autooc-0.0.8/autooc/fitness/training_time.py
-drwxr-xr-x   0 luis      (1000) luis      (1000)        0 2023-06-24 15:15:01.148877 autooc-0.0.8/autooc/operators/
--rw-r--r--   0 luis      (1000) luis      (1000)        0 2023-06-24 14:17:34.000000 autooc-0.0.8/autooc/operators/__init__.py
--rw-r--r--   0 luis      (1000) luis      (1000)    16352 2023-06-24 14:17:34.000000 autooc-0.0.8/autooc/operators/crossover.py
--rw-r--r--   0 luis      (1000) luis      (1000)    16207 2023-06-24 14:17:34.000000 autooc-0.0.8/autooc/operators/initialisation.py
--rw-r--r--   0 luis      (1000) luis      (1000)     8189 2023-06-24 14:17:34.000000 autooc-0.0.8/autooc/operators/mutation.py
--rw-r--r--   0 luis      (1000) luis      (1000)     5351 2023-06-24 14:17:34.000000 autooc-0.0.8/autooc/operators/replacement.py
--rw-r--r--   0 luis      (1000) luis      (1000)     4486 2023-06-24 14:17:34.000000 autooc-0.0.8/autooc/operators/selection.py
--rw-r--r--   0 luis      (1000) luis      (1000)    28915 2023-06-24 14:17:34.000000 autooc-0.0.8/autooc/operators/subtree_parse.py
-drwxr-xr-x   0 luis      (1000) luis      (1000)        0 2023-06-24 15:15:01.148877 autooc-0.0.8/autooc/representation/
--rw-r--r--   0 luis      (1000) luis      (1000)        0 2023-06-24 14:17:35.000000 autooc-0.0.8/autooc/representation/__init__.py
--rw-r--r--   0 luis      (1000) luis      (1000)    14379 2023-06-24 14:17:35.000000 autooc-0.0.8/autooc/representation/derivation.py
--rw-r--r--   0 luis      (1000) luis      (1000)    28989 2023-06-24 14:17:35.000000 autooc-0.0.8/autooc/representation/grammar.py
--rw-r--r--   0 luis      (1000) luis      (1000)     6994 2023-06-24 14:17:35.000000 autooc-0.0.8/autooc/representation/individual.py
--rw-r--r--   0 luis      (1000) luis      (1000)     6384 2023-06-24 14:17:35.000000 autooc-0.0.8/autooc/representation/latent_tree.py
--rw-r--r--   0 luis      (1000) luis      (1000)     8567 2023-06-24 14:17:35.000000 autooc-0.0.8/autooc/representation/tree.py
-drwxr-xr-x   0 luis      (1000) luis      (1000)        0 2023-06-24 15:15:01.148877 autooc-0.0.8/autooc/scripts/
--rw-r--r--   0 luis      (1000) luis      (1000)    13836 2023-06-24 14:17:35.000000 autooc-0.0.8/autooc/scripts/GE_LR_parser.py
--rw-r--r--   0 luis      (1000) luis      (1000)        0 2023-06-24 14:17:35.000000 autooc-0.0.8/autooc/scripts/__init__.py
--rw-r--r--   0 luis      (1000) luis      (1000)     3387 2023-06-24 14:17:35.000000 autooc-0.0.8/autooc/scripts/baselines.py
--rw-r--r--   0 luis      (1000) luis      (1000)     2532 2023-06-24 14:17:35.000000 autooc-0.0.8/autooc/scripts/experiment_manager.py
--rw-r--r--   0 luis      (1000) luis      (1000)     2642 2023-06-24 14:17:35.000000 autooc-0.0.8/autooc/scripts/grammar_analyser.py
--rw-r--r--   0 luis      (1000) luis      (1000)     4583 2023-06-24 14:17:35.000000 autooc-0.0.8/autooc/scripts/python_script_evaluation.py
--rw-r--r--   0 luis      (1000) luis      (1000)    10267 2023-06-24 14:17:35.000000 autooc-0.0.8/autooc/scripts/stats_parser.py
-drwxr-xr-x   0 luis      (1000) luis      (1000)        0 2023-06-24 15:15:01.148877 autooc-0.0.8/autooc/stats/
--rw-r--r--   0 luis      (1000) luis      (1000)        0 2023-06-24 14:17:35.000000 autooc-0.0.8/autooc/stats/__init__.py
--rw-r--r--   0 luis      (1000) luis      (1000)    13101 2023-06-24 14:17:35.000000 autooc-0.0.8/autooc/stats/stats.py
-drwxr-xr-x   0 luis      (1000) luis      (1000)        0 2023-06-24 15:15:01.148877 autooc-0.0.8/autooc/utilities/
--rw-r--r--   0 luis      (1000) luis      (1000)        0 2023-06-24 14:17:35.000000 autooc-0.0.8/autooc/utilities/__init__.py
-drwxr-xr-x   0 luis      (1000) luis      (1000)        0 2023-06-24 15:15:01.148877 autooc-0.0.8/autooc/utilities/algorithm/
--rw-r--r--   0 luis      (1000) luis      (1000)    12775 2023-06-24 14:17:35.000000 autooc-0.0.8/autooc/utilities/algorithm/NSGA2.py
--rw-r--r--   0 luis      (1000) luis      (1000)        0 2023-06-24 14:17:35.000000 autooc-0.0.8/autooc/utilities/algorithm/__init__.py
--rw-r--r--   0 luis      (1000) luis      (1000)    23627 2023-06-24 14:17:35.000000 autooc-0.0.8/autooc/utilities/algorithm/command_line_parser.py
--rw-r--r--   0 luis      (1000) luis      (1000)      418 2023-06-24 14:17:35.000000 autooc-0.0.8/autooc/utilities/algorithm/general.py
--rw-r--r--   0 luis      (1000) luis      (1000)    11564 2023-06-24 14:17:35.000000 autooc-0.0.8/autooc/utilities/algorithm/initialise_run.py
--rw-r--r--   0 luis      (1000) luis      (1000)     4433 2023-06-24 14:17:35.000000 autooc-0.0.8/autooc/utilities/algorithm/state.py
-drwxr-xr-x   0 luis      (1000) luis      (1000)        0 2023-06-24 15:15:01.158877 autooc-0.0.8/autooc/utilities/fitness/
--rw-r--r--   0 luis      (1000) luis      (1000)        0 2023-06-24 14:17:35.000000 autooc-0.0.8/autooc/utilities/fitness/__init__.py
--rw-r--r--   0 luis      (1000) luis      (1000)     8348 2023-06-24 14:17:35.000000 autooc-0.0.8/autooc/utilities/fitness/error_metric.py
--rw-r--r--   0 luis      (1000) luis      (1000)     3663 2023-06-24 14:17:35.000000 autooc-0.0.8/autooc/utilities/fitness/get_data.py
--rw-r--r--   0 luis      (1000) luis      (1000)     6753 2023-06-24 14:17:35.000000 autooc-0.0.8/autooc/utilities/fitness/math_functions.py
--rw-r--r--   0 luis      (1000) luis      (1000)     2993 2023-06-24 14:17:35.000000 autooc-0.0.8/autooc/utilities/fitness/optimize_constants.py
-drwxr-xr-x   0 luis      (1000) luis      (1000)        0 2023-06-24 15:15:01.158877 autooc-0.0.8/autooc/utilities/representation/
--rw-r--r--   0 luis      (1000) luis      (1000)        0 2023-06-24 14:17:35.000000 autooc-0.0.8/autooc/utilities/representation/__init__.py
--rw-r--r--   0 luis      (1000) luis      (1000)    13533 2023-06-24 14:17:35.000000 autooc-0.0.8/autooc/utilities/representation/check_methods.py
--rw-r--r--   0 luis      (1000) luis      (1000)      720 2023-06-24 14:17:35.000000 autooc-0.0.8/autooc/utilities/representation/python_filter.py
-drwxr-xr-x   0 luis      (1000) luis      (1000)        0 2023-06-24 15:15:01.158877 autooc-0.0.8/autooc/utilities/stats/
--rw-r--r--   0 luis      (1000) luis      (1000)        0 2023-06-24 14:17:35.000000 autooc-0.0.8/autooc/utilities/stats/__init__.py
--rw-r--r--   0 luis      (1000) luis      (1000)      498 2023-06-24 14:17:35.000000 autooc-0.0.8/autooc/utilities/stats/clean_stats.py
--rw-r--r--   0 luis      (1000) luis      (1000)     6086 2023-06-24 14:17:35.000000 autooc-0.0.8/autooc/utilities/stats/file_io.py
--rw-r--r--   0 luis      (1000) luis      (1000)     4512 2023-06-24 14:17:35.000000 autooc-0.0.8/autooc/utilities/stats/save_plots.py
--rw-r--r--   0 luis      (1000) luis      (1000)     1015 2023-06-24 14:17:35.000000 autooc-0.0.8/autooc/utilities/stats/trackers.py
--rw-r--r--   0 luis      (1000) luis      (1000)     1966 2023-06-24 14:17:35.000000 autooc-0.0.8/autooc/utilities/utils.py
-drwxr-xr-x   0 luis      (1000) luis      (1000)        0 2023-06-24 15:15:01.138877 autooc-0.0.8/autooc.egg-info/
--rw-r--r--   0 luis      (1000) luis      (1000)    12349 2023-06-24 15:15:01.000000 autooc-0.0.8/autooc.egg-info/PKG-INFO
--rw-r--r--   0 luis      (1000) luis      (1000)     3283 2023-06-24 15:15:01.000000 autooc-0.0.8/autooc.egg-info/SOURCES.txt
--rw-r--r--   0 luis      (1000) luis      (1000)        1 2023-06-24 15:15:01.000000 autooc-0.0.8/autooc.egg-info/dependency_links.txt
--rw-r--r--   0 luis      (1000) luis      (1000)      150 2023-06-24 15:15:01.000000 autooc-0.0.8/autooc.egg-info/requires.txt
--rw-r--r--   0 luis      (1000) luis      (1000)        7 2023-06-24 15:15:01.000000 autooc-0.0.8/autooc.egg-info/top_level.txt
--rw-r--r--   0 luis      (1000) luis      (1000)      103 2023-06-24 15:15:01.158877 autooc-0.0.8/setup.cfg
--rw-r--r--   0 luis      (1000) luis      (1000)     1356 2023-06-24 15:14:57.000000 autooc-0.0.8/setup.py
+drwxr-xr-x   0 luis      (1000) luis      (1000)        0 2023-06-24 15:25:55.698882 autooc-0.0.9/
+-rw-r--r--   0 luis      (1000) luis      (1000)     1071 2023-06-24 14:17:33.000000 autooc-0.0.9/LICENSE
+-rw-r--r--   0 luis      (1000) luis      (1000)       43 2023-06-24 15:24:06.000000 autooc-0.0.9/MANIFEST.in
+-rw-r--r--   0 luis      (1000) luis      (1000)    12349 2023-06-24 15:25:55.698882 autooc-0.0.9/PKG-INFO
+-rw-r--r--   0 luis      (1000) luis      (1000)    11738 2023-06-24 14:29:17.000000 autooc-0.0.9/README.md
+drwxr-xr-x   0 luis      (1000) luis      (1000)        0 2023-06-24 15:25:55.678882 autooc-0.0.9/autooc/
+-rw-r--r--   0 luis      (1000) luis      (1000)        0 2023-06-24 14:17:34.000000 autooc-0.0.9/autooc/__init__.py
+drwxr-xr-x   0 luis      (1000) luis      (1000)        0 2023-06-24 15:25:55.678882 autooc-0.0.9/autooc/algorithm/
+-rw-r--r--   0 luis      (1000) luis      (1000)        0 2023-06-24 14:17:34.000000 autooc-0.0.9/autooc/algorithm/__init__.py
+drwxr-xr-x   0 luis      (1000) luis      (1000)        0 2023-06-24 15:25:55.678882 autooc-0.0.9/autooc/algorithm/distributed_algorithm/
+-rw-r--r--   0 luis      (1000) luis      (1000)        0 2023-06-24 14:17:34.000000 autooc-0.0.9/autooc/algorithm/distributed_algorithm/__init__.py
+-rw-r--r--   0 luis      (1000) luis      (1000)     1001 2023-06-24 15:21:52.000000 autooc-0.0.9/autooc/algorithm/distributed_algorithm/search_loop.py
+-rw-r--r--   0 luis      (1000) luis      (1000)      426 2023-06-24 14:17:34.000000 autooc-0.0.9/autooc/algorithm/distributed_algorithm/step.py
+-rw-r--r--   0 luis      (1000) luis      (1000)     9892 2023-06-24 15:21:16.000000 autooc-0.0.9/autooc/algorithm/hill_climbing.py
+-rw-r--r--   0 luis      (1000) luis      (1000)    11900 2023-06-24 15:21:19.000000 autooc-0.0.9/autooc/algorithm/mapper.py
+-rw-r--r--   0 luis      (1000) luis      (1000)    13842 2023-06-24 15:24:37.000000 autooc-0.0.9/autooc/algorithm/parameters.py
+-rw-r--r--   0 luis      (1000) luis      (1000)     2466 2023-06-24 15:21:25.000000 autooc-0.0.9/autooc/algorithm/search_loop.py
+-rw-r--r--   0 luis      (1000) luis      (1000)     1649 2023-06-24 15:21:31.000000 autooc-0.0.9/autooc/algorithm/step.py
+-rw-r--r--   0 luis      (1000) luis      (1000)    25082 2023-06-24 15:18:20.000000 autooc-0.0.9/autooc/autooc.py
+drwxr-xr-x   0 luis      (1000) luis      (1000)        0 2023-06-24 15:25:55.678882 autooc-0.0.9/autooc/fitness/
+-rw-r--r--   0 luis      (1000) luis      (1000)        0 2023-06-24 14:17:34.000000 autooc-0.0.9/autooc/fitness/__init__.py
+drwxr-xr-x   0 luis      (1000) luis      (1000)        0 2023-06-24 15:25:55.678882 autooc-0.0.9/autooc/fitness/base_ff_classes/
+-rw-r--r--   0 luis      (1000) luis      (1000)        0 2023-06-24 14:17:34.000000 autooc-0.0.9/autooc/fitness/base_ff_classes/__init__.py
+-rw-r--r--   0 luis      (1000) luis      (1000)     2130 2023-06-24 14:17:34.000000 autooc-0.0.9/autooc/fitness/base_ff_classes/base_ff.py
+-rw-r--r--   0 luis      (1000) luis      (1000)     2588 2023-06-24 15:21:52.000000 autooc-0.0.9/autooc/fitness/base_ff_classes/ff_template.py
+-rw-r--r--   0 luis      (1000) luis      (1000)     2662 2023-06-24 14:17:34.000000 autooc-0.0.9/autooc/fitness/base_ff_classes/moo_ff.py
+-rw-r--r--   0 luis      (1000) luis      (1000)      487 2023-06-24 15:21:52.000000 autooc-0.0.9/autooc/fitness/bic.py
+-rw-r--r--   0 luis      (1000) luis      (1000)     5111 2023-06-24 15:18:57.000000 autooc-0.0.9/autooc/fitness/evaluation.py
+-rw-r--r--   0 luis      (1000) luis      (1000)      363 2023-06-24 15:21:52.000000 autooc-0.0.9/autooc/fitness/minimise_nodes.py
+drwxr-xr-x   0 luis      (1000) luis      (1000)        0 2023-06-24 15:25:55.678882 autooc-0.0.9/autooc/fitness/multi_objective/
+-rw-r--r--   0 luis      (1000) luis      (1000)        0 2023-06-24 14:17:34.000000 autooc-0.0.9/autooc/fitness/multi_objective/__init__.py
+-rw-r--r--   0 luis      (1000) luis      (1000)      798 2023-06-24 15:21:52.000000 autooc-0.0.9/autooc/fitness/multi_objective/binary_phenotype_to_float.py
+-rw-r--r--   0 luis      (1000) luis      (1000)     3948 2023-06-24 15:21:52.000000 autooc-0.0.9/autooc/fitness/multi_objective/singlefit_autoencoders.py
+-rw-r--r--   0 luis      (1000) luis      (1000)     1846 2023-06-24 15:21:52.000000 autooc-0.0.9/autooc/fitness/multi_objective/singlefit_multiobj.py
+-rw-r--r--   0 luis      (1000) luis      (1000)     1009 2023-06-24 15:21:52.000000 autooc-0.0.9/autooc/fitness/multi_objective/zdt1.py
+-rw-r--r--   0 luis      (1000) luis      (1000)      409 2023-06-24 15:21:52.000000 autooc-0.0.9/autooc/fitness/num_params.py
+-rw-r--r--   0 luis      (1000) luis      (1000)      405 2023-06-24 15:21:52.000000 autooc-0.0.9/autooc/fitness/predict_time.py
+-rw-r--r--   0 luis      (1000) luis      (1000)     6024 2023-06-24 15:21:52.000000 autooc-0.0.9/autooc/fitness/progsys.py
+-rw-r--r--   0 luis      (1000) luis      (1000)     1338 2023-06-24 15:21:52.000000 autooc-0.0.9/autooc/fitness/pymax.py
+-rw-r--r--   0 luis      (1000) luis      (1000)     5888 2023-06-24 15:21:52.000000 autooc-0.0.9/autooc/fitness/sequence_match.py
+-rw-r--r--   0 luis      (1000) luis      (1000)     1040 2023-06-24 15:21:52.000000 autooc-0.0.9/autooc/fitness/string_match.py
+drwxr-xr-x   0 luis      (1000) luis      (1000)        0 2023-06-24 15:25:55.688882 autooc-0.0.9/autooc/fitness/supervised_learning/
+-rw-r--r--   0 luis      (1000) luis      (1000)        0 2023-06-24 14:17:34.000000 autooc-0.0.9/autooc/fitness/supervised_learning/__init__.py
+-rw-r--r--   0 luis      (1000) luis      (1000)     3734 2023-06-24 15:21:52.000000 autooc-0.0.9/autooc/fitness/supervised_learning/boolean_problem.py
+-rw-r--r--   0 luis      (1000) luis      (1000)      662 2023-06-24 15:21:52.000000 autooc-0.0.9/autooc/fitness/supervised_learning/classification.py
+-rw-r--r--   0 luis      (1000) luis      (1000)     2915 2023-06-24 15:21:52.000000 autooc-0.0.9/autooc/fitness/supervised_learning/if_else_classifier.py
+-rw-r--r--   0 luis      (1000) luis      (1000)      646 2023-06-24 15:21:52.000000 autooc-0.0.9/autooc/fitness/supervised_learning/regression.py
+-rw-r--r--   0 luis      (1000) luis      (1000)     4481 2023-06-24 15:21:52.000000 autooc-0.0.9/autooc/fitness/supervised_learning/regression_random_polynomial.py
+-rw-r--r--   0 luis      (1000) luis      (1000)    10342 2023-06-24 15:21:52.000000 autooc-0.0.9/autooc/fitness/supervised_learning/supervised_learning.py
+-rw-r--r--   0 luis      (1000) luis      (1000)     3632 2023-06-24 15:21:52.000000 autooc-0.0.9/autooc/fitness/supervised_learning/supervised_learning_backup.py
+-rw-r--r--   0 luis      (1000) luis      (1000)      408 2023-06-24 15:21:52.000000 autooc-0.0.9/autooc/fitness/training_time.py
+drwxr-xr-x   0 luis      (1000) luis      (1000)        0 2023-06-24 15:25:55.688882 autooc-0.0.9/autooc/grammars/
+-rw-r--r--   0 luis      (1000) luis      (1000)      538 2023-06-24 14:17:34.000000 autooc-0.0.9/autooc/grammars/autoencoders.bnf
+-rw-r--r--   0 luis      (1000) luis      (1000)      823 2023-06-24 14:17:34.000000 autooc-0.0.9/autooc/grammars/autoencoders.pybnf
+-rw-r--r--   0 luis      (1000) luis      (1000)     1159 2023-06-24 14:17:34.000000 autooc-0.0.9/autooc/grammars/autoencoders_v2.pybnf
+-rw-r--r--   0 luis      (1000) luis      (1000)     1148 2023-06-24 14:17:34.000000 autooc-0.0.9/autooc/grammars/autoencoders_v3.pybnf
+-rw-r--r--   0 luis      (1000) luis      (1000)      962 2023-06-24 14:17:34.000000 autooc-0.0.9/autooc/grammars/autoencoders_v4.pybnf
+-rw-r--r--   0 luis      (1000) luis      (1000)      465 2023-06-24 14:17:34.000000 autooc-0.0.9/autooc/grammars/iforest.pybnf
+-rw-r--r--   0 luis      (1000) luis      (1000)      720 2023-06-24 14:17:34.000000 autooc-0.0.9/autooc/grammars/lof.pybnf
+-rw-r--r--   0 luis      (1000) luis      (1000)     2088 2023-06-24 14:17:34.000000 autooc-0.0.9/autooc/grammars/multi_algo.pybnf
+-rw-r--r--   0 luis      (1000) luis      (1000)      303 2023-06-24 14:17:34.000000 autooc-0.0.9/autooc/grammars/svm.pybnf
+drwxr-xr-x   0 luis      (1000) luis      (1000)        0 2023-06-24 15:25:55.688882 autooc-0.0.9/autooc/operators/
+-rw-r--r--   0 luis      (1000) luis      (1000)        0 2023-06-24 14:17:34.000000 autooc-0.0.9/autooc/operators/__init__.py
+-rw-r--r--   0 luis      (1000) luis      (1000)    16356 2023-06-24 15:21:52.000000 autooc-0.0.9/autooc/operators/crossover.py
+-rw-r--r--   0 luis      (1000) luis      (1000)    16215 2023-06-24 15:20:57.000000 autooc-0.0.9/autooc/operators/initialisation.py
+-rw-r--r--   0 luis      (1000) luis      (1000)     8194 2023-06-24 15:21:52.000000 autooc-0.0.9/autooc/operators/mutation.py
+-rw-r--r--   0 luis      (1000) luis      (1000)     5357 2023-06-24 15:21:52.000000 autooc-0.0.9/autooc/operators/replacement.py
+-rw-r--r--   0 luis      (1000) luis      (1000)     4488 2023-06-24 15:21:52.000000 autooc-0.0.9/autooc/operators/selection.py
+-rw-r--r--   0 luis      (1000) luis      (1000)    28919 2023-06-24 15:21:52.000000 autooc-0.0.9/autooc/operators/subtree_parse.py
+drwxr-xr-x   0 luis      (1000) luis      (1000)        0 2023-06-24 15:25:55.688882 autooc-0.0.9/autooc/representation/
+-rw-r--r--   0 luis      (1000) luis      (1000)        0 2023-06-24 14:17:35.000000 autooc-0.0.9/autooc/representation/__init__.py
+-rw-r--r--   0 luis      (1000) luis      (1000)    14382 2023-06-24 15:21:52.000000 autooc-0.0.9/autooc/representation/derivation.py
+-rw-r--r--   0 luis      (1000) luis      (1000)    28990 2023-06-24 15:21:52.000000 autooc-0.0.9/autooc/representation/grammar.py
+-rw-r--r--   0 luis      (1000) luis      (1000)     6996 2023-06-24 15:21:52.000000 autooc-0.0.9/autooc/representation/individual.py
+-rw-r--r--   0 luis      (1000) luis      (1000)     6386 2023-06-24 15:21:52.000000 autooc-0.0.9/autooc/representation/latent_tree.py
+-rw-r--r--   0 luis      (1000) luis      (1000)     8568 2023-06-24 15:21:52.000000 autooc-0.0.9/autooc/representation/tree.py
+drwxr-xr-x   0 luis      (1000) luis      (1000)        0 2023-06-24 15:25:55.688882 autooc-0.0.9/autooc/scripts/
+-rw-r--r--   0 luis      (1000) luis      (1000)    13842 2023-06-24 15:21:52.000000 autooc-0.0.9/autooc/scripts/GE_LR_parser.py
+-rw-r--r--   0 luis      (1000) luis      (1000)        0 2023-06-24 14:17:35.000000 autooc-0.0.9/autooc/scripts/__init__.py
+-rw-r--r--   0 luis      (1000) luis      (1000)     3388 2023-06-24 15:21:52.000000 autooc-0.0.9/autooc/scripts/baselines.py
+-rw-r--r--   0 luis      (1000) luis      (1000)     2535 2023-06-24 15:21:52.000000 autooc-0.0.9/autooc/scripts/experiment_manager.py
+-rw-r--r--   0 luis      (1000) luis      (1000)     2646 2023-06-24 15:21:52.000000 autooc-0.0.9/autooc/scripts/grammar_analyser.py
+-rw-r--r--   0 luis      (1000) luis      (1000)     4583 2023-06-24 14:17:35.000000 autooc-0.0.9/autooc/scripts/python_script_evaluation.py
+-rw-r--r--   0 luis      (1000) luis      (1000)    10269 2023-06-24 15:25:09.000000 autooc-0.0.9/autooc/scripts/stats_parser.py
+drwxr-xr-x   0 luis      (1000) luis      (1000)        0 2023-06-24 15:25:55.688882 autooc-0.0.9/autooc/stats/
+-rw-r--r--   0 luis      (1000) luis      (1000)        0 2023-06-24 14:17:35.000000 autooc-0.0.9/autooc/stats/__init__.py
+-rw-r--r--   0 luis      (1000) luis      (1000)    13107 2023-06-24 15:19:42.000000 autooc-0.0.9/autooc/stats/stats.py
+drwxr-xr-x   0 luis      (1000) luis      (1000)        0 2023-06-24 15:25:55.688882 autooc-0.0.9/autooc/utilities/
+-rw-r--r--   0 luis      (1000) luis      (1000)        0 2023-06-24 14:17:35.000000 autooc-0.0.9/autooc/utilities/__init__.py
+drwxr-xr-x   0 luis      (1000) luis      (1000)        0 2023-06-24 15:25:55.688882 autooc-0.0.9/autooc/utilities/algorithm/
+-rw-r--r--   0 luis      (1000) luis      (1000)    12777 2023-06-24 15:19:56.000000 autooc-0.0.9/autooc/utilities/algorithm/NSGA2.py
+-rw-r--r--   0 luis      (1000) luis      (1000)        0 2023-06-24 14:17:35.000000 autooc-0.0.9/autooc/utilities/algorithm/__init__.py
+-rw-r--r--   0 luis      (1000) luis      (1000)    23627 2023-06-24 14:17:35.000000 autooc-0.0.9/autooc/utilities/algorithm/command_line_parser.py
+-rw-r--r--   0 luis      (1000) luis      (1000)      418 2023-06-24 14:17:35.000000 autooc-0.0.9/autooc/utilities/algorithm/general.py
+-rw-r--r--   0 luis      (1000) luis      (1000)    11579 2023-06-24 15:24:58.000000 autooc-0.0.9/autooc/utilities/algorithm/initialise_run.py
+-rw-r--r--   0 luis      (1000) luis      (1000)     4440 2023-06-24 15:21:52.000000 autooc-0.0.9/autooc/utilities/algorithm/state.py
+drwxr-xr-x   0 luis      (1000) luis      (1000)        0 2023-06-24 15:25:55.688882 autooc-0.0.9/autooc/utilities/fitness/
+-rw-r--r--   0 luis      (1000) luis      (1000)        0 2023-06-24 14:17:35.000000 autooc-0.0.9/autooc/utilities/fitness/__init__.py
+-rw-r--r--   0 luis      (1000) luis      (1000)     8349 2023-06-24 15:21:52.000000 autooc-0.0.9/autooc/utilities/fitness/error_metric.py
+-rw-r--r--   0 luis      (1000) luis      (1000)     3664 2023-06-24 15:21:52.000000 autooc-0.0.9/autooc/utilities/fitness/get_data.py
+-rw-r--r--   0 luis      (1000) luis      (1000)     6753 2023-06-24 14:17:35.000000 autooc-0.0.9/autooc/utilities/fitness/math_functions.py
+-rw-r--r--   0 luis      (1000) luis      (1000)     2995 2023-06-24 15:21:52.000000 autooc-0.0.9/autooc/utilities/fitness/optimize_constants.py
+drwxr-xr-x   0 luis      (1000) luis      (1000)        0 2023-06-24 15:25:55.688882 autooc-0.0.9/autooc/utilities/representation/
+-rw-r--r--   0 luis      (1000) luis      (1000)        0 2023-06-24 14:17:35.000000 autooc-0.0.9/autooc/utilities/representation/__init__.py
+-rw-r--r--   0 luis      (1000) luis      (1000)    13535 2023-06-24 15:21:52.000000 autooc-0.0.9/autooc/utilities/representation/check_methods.py
+-rw-r--r--   0 luis      (1000) luis      (1000)      720 2023-06-24 14:17:35.000000 autooc-0.0.9/autooc/utilities/representation/python_filter.py
+drwxr-xr-x   0 luis      (1000) luis      (1000)        0 2023-06-24 15:25:55.698882 autooc-0.0.9/autooc/utilities/stats/
+-rw-r--r--   0 luis      (1000) luis      (1000)        0 2023-06-24 14:17:35.000000 autooc-0.0.9/autooc/utilities/stats/__init__.py
+-rw-r--r--   0 luis      (1000) luis      (1000)      500 2023-06-24 15:21:52.000000 autooc-0.0.9/autooc/utilities/stats/clean_stats.py
+-rw-r--r--   0 luis      (1000) luis      (1000)     6088 2023-06-24 15:20:09.000000 autooc-0.0.9/autooc/utilities/stats/file_io.py
+-rw-r--r--   0 luis      (1000) luis      (1000)     4516 2023-06-24 15:21:52.000000 autooc-0.0.9/autooc/utilities/stats/save_plots.py
+-rw-r--r--   0 luis      (1000) luis      (1000)     1015 2023-06-24 14:17:35.000000 autooc-0.0.9/autooc/utilities/stats/trackers.py
+-rw-r--r--   0 luis      (1000) luis      (1000)     1966 2023-06-24 14:17:35.000000 autooc-0.0.9/autooc/utilities/utils.py
+drwxr-xr-x   0 luis      (1000) luis      (1000)        0 2023-06-24 15:25:55.678882 autooc-0.0.9/autooc.egg-info/
+-rw-r--r--   0 luis      (1000) luis      (1000)    12349 2023-06-24 15:25:55.000000 autooc-0.0.9/autooc.egg-info/PKG-INFO
+-rw-r--r--   0 luis      (1000) luis      (1000)     3580 2023-06-24 15:25:55.000000 autooc-0.0.9/autooc.egg-info/SOURCES.txt
+-rw-r--r--   0 luis      (1000) luis      (1000)        1 2023-06-24 15:25:55.000000 autooc-0.0.9/autooc.egg-info/dependency_links.txt
+-rw-r--r--   0 luis      (1000) luis      (1000)      150 2023-06-24 15:25:55.000000 autooc-0.0.9/autooc.egg-info/requires.txt
+-rw-r--r--   0 luis      (1000) luis      (1000)        7 2023-06-24 15:25:55.000000 autooc-0.0.9/autooc.egg-info/top_level.txt
+-rw-r--r--   0 luis      (1000) luis      (1000)      103 2023-06-24 15:25:55.698882 autooc-0.0.9/setup.cfg
+-rw-r--r--   0 luis      (1000) luis      (1000)     1357 2023-06-24 15:25:38.000000 autooc-0.0.9/setup.py
```

### Comparing `autooc-0.0.8/LICENSE` & `autooc-0.0.9/LICENSE`

 * *Files identical despite different names*

### Comparing `autooc-0.0.8/PKG-INFO` & `autooc-0.0.9/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: autooc
-Version: 0.0.8
+Version: 0.0.9
 Summary: AutoOC: Automated Machine Learning (AutoML) library for One-Class Learning
 Home-page: https://github.com/luisferreira97/AutoOC
 Author: Luís Ferreira
 Author-email: luis_ferreira223@hotmail.com
 Keywords: automl,machine learning,one-class learning,one-class classification,autoencoder,isolation forest,one-class svm
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: autooc Version: 0.0.8 Summary: AutoOC: Automated
+Metadata-Version: 2.1 Name: autooc Version: 0.0.9 Summary: AutoOC: Automated
 Machine Learning (AutoML) library for One-Class Learning Home-page: https://
 github.com/luisferreira97/AutoOC Author: LuÃ­s Ferreira Author-email:
 luis_ferreira223@hotmail.com Keywords: automl,machine learning,one-class
 learning,one-class classification,autoencoder,isolation forest,one-class svm
 Classifier: Programming Language :: Python :: 3 Classifier: License :: OSI
 Approved :: MIT License Classifier: Operating System :: OS Independent
 Requires-Python: >=3.6, <3.9 Description-Content-Type: text/markdown License-
```

### Comparing `autooc-0.0.8/README.md` & `autooc-0.0.9/README.md`

 * *Files identical despite different names*

### Comparing `autooc-0.0.8/autooc/algorithm/distributed_algorithm/search_loop.py` & `autooc-0.0.9/autooc/algorithm/distributed_algorithm/search_loop.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,15 +1,15 @@
-from talos.agent.agent import Agent
-from talos.algorithm.parameters import params
-# from talos.fitness.evaluation import evaluate_fitness
-from talos.stats.stats import stats
+from autooc.agent.agent import Agent
+from autooc.algorithm.parameters import params
+# from autooc.fitness.evaluation import evaluate_fitness
+from autooc.stats.stats import stats
 
-# from talos.utilities.stats import trackers
-# from talos.operators.initialisation import initialisation
-# from talos.utilities.algorithm.initialise_run import pool_init
+# from autooc.utilities.stats import trackers
+# from autooc.operators.initialisation import initialisation
+# from autooc.utilities.algorithm.initialise_run import pool_init
 
 
 def create_agents(n, p):
     """
     Create a list of agent specified by n parameter
     """
     return [Agent(p) for a in range(n)]
```

### Comparing `autooc-0.0.8/autooc/algorithm/hill_climbing.py` & `autooc-0.0.9/autooc/algorithm/hill_climbing.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
-from talos.algorithm.parameters import params
-from talos.fitness.evaluation import evaluate_fitness
-from talos.stats.stats import get_stats, stats
-from talos.utilities.stats import trackers
+from autooc.algorithm.parameters import params
+from autooc.fitness.evaluation import evaluate_fitness
+from autooc.stats.stats import get_stats, stats
+from autooc.utilities.stats import trackers
 
 """Hill-climbing is just about the simplest meta-heuristic there
 is. It's of interest in GP/GE because of the lingering suspicion among
 many researchers that crossover just doesn't work. This goes back to
 90s work by Chellapilla and by O'Reilly. Today, many papers are
 published which use mutation only.
```

### Comparing `autooc-0.0.8/autooc/algorithm/mapper.py` & `autooc-0.0.9/autooc/algorithm/mapper.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 from collections import deque
 
 import numpy as np
 
-from talos.algorithm.parameters import params
-from talos.representation.tree import Tree
-from talos.utilities.representation.python_filter import python_filter
+from autooc.algorithm.parameters import params
+from autooc.representation.tree import Tree
+from autooc.utilities.representation.python_filter import python_filter
 
 
 def mapper(genome, tree):
     """
     Wheel for mapping. Calls the correct mapper for a given _input. Checks
     the params dict to ensure the correct type of individual is being created.
```

### Comparing `autooc-0.0.8/autooc/algorithm/parameters.py` & `autooc-0.0.9/autooc/algorithm/parameters.py`

 * *Files 6% similar despite different names*

```diff
@@ -13,15 +13,15 @@
     "STEP": "step",
     # Evolutionary Parameters
     "POPULATION_SIZE": 500,
     "GENERATIONS": 50,
     "HILL_CLIMBING_HISTORY": 1000,
     "SCHC_COUNT_METHOD": "count_all",
     # Set optional experiment name
-    "EXPERIMENT_NAME": "Talos",
+    "EXPERIMENT_NAME": "AutoOC",
     # Set default number of runs to be done.
     # ONLY USED WITH EXPERIMENT MANAGER.
     "RUNS": 1,
     # Class of problem
     "FITNESS_FUNCTION": "supervised_learning.regression",
     # Select problem dataset
     "DATASET_TRAIN": None,
@@ -53,45 +53,45 @@
     "INIT_GENOME_LENGTH": 200,
     # Set the maximum tree depth for initialisation.
     "MAX_INIT_TREE_DEPTH": 10,
     # Set the minimum tree depth for initialisation.
     "MIN_INIT_TREE_DEPTH": None,
     # SELECTION
     # Set selection operator.
-    "SELECTION": "talos.operators.selection.tournament",
+    "SELECTION": "autooc.operators.selection.tournament",
     # For tournament selection
     "TOURNAMENT_SIZE": 2,
     # For truncation selection
     "SELECTION_PROPORTION": 0.5,
     # Allow for selection of invalid individuals during selection process.
     "INVALID_SELECTION": False,
     # OPERATOR OPTIONS
     # Boolean flag for selecting whether or not mutation is confined to
     # within the used portion of the genome. Default set to True.
     "WITHIN_USED": True,
     # CROSSOVER
     # Set crossover operator.
-    "CROSSOVER": "talos.operators.crossover.variable_onepoint",
+    "CROSSOVER": "autooc.operators.crossover.variable_onepoint",
     # Set crossover probability.
     "CROSSOVER_PROBABILITY": 0.75,
     # Prevents crossover from generating invalids.
     "NO_CROSSOVER_INVALIDS": False,
     # MUTATION
     # Set mutation operator.
-    "MUTATION": "talos.operators.mutation.int_flip_per_codon",
+    "MUTATION": "autooc.operators.mutation.int_flip_per_codon",
     # Set mutation probability (None defaults to 1 over the length of
     # the genome for each codon)
     "MUTATION_PROBABILITY": None,
     # Set number of mutation events
     "MUTATION_EVENTS": 1,
     # Prevents mutation from generating invalids.
     "NO_MUTATION_INVALIDS": False,
     # REPLACEMENT
     # Set replacement operator.
-    "REPLACEMENT": "talos.operators.replacement.generational",
+    "REPLACEMENT": "autooc.operators.replacement.generational",
     # Set elite size.
     "ELITE_SIZE": None,
     # DEBUGGING
     # Use this to turn on debugging mode. This mode doesn't write any files
     # and should be used when you want to test new methods.
     "DEBUG": False,
     # PRINTING
@@ -223,20 +223,20 @@
     seeds, elite size). Sets the correct imports given command line
     arguments. Sets correct grammar file and fitness function. Also
     initialises save folders and tracker lists in utilities.trackers.
 
     :param command_line_args: Command line arguments specified by the user.
     :return: Nothing.
     """
-    from talos.representation import grammar
-    from talos.utilities.algorithm.command_line_parser import parse_cmd_args
-    from talos.utilities.algorithm.initialise_run import (
+    from autooc.representation import grammar
+    from autooc.utilities.algorithm.command_line_parser import parse_cmd_args
+    from autooc.utilities.algorithm.initialise_run import (
         initialise_run_params, set_param_imports)
-    from talos.utilities.fitness.math_functions import return_one_percent
-    from talos.utilities.stats import clean_stats, trackers
+    from autooc.utilities.fitness.math_functions import return_one_percent
+    from autooc.utilities.stats import clean_stats, trackers
 
     cmd_args, unknown = parse_cmd_args(command_line_args)
 
     if unknown:
         # We currently do not parse unknown parameters. Raise error.
         s = (
             "algorithm.parameters.set_params\nError: "
@@ -245,30 +245,30 @@
             "--extra_parameters" % str(unknown)
         )
         raise Exception(s)
 
     # LOAD PARAMETERS FILE
     # NOTE that the parameters file overwrites all previously set parameters.
     if "PARAMETERS" in cmd_args:
-        load_params(path.join(getcwd(), "talos",
+        load_params(path.join(getcwd(), "autooc",
                     "parameters", cmd_args["PARAMETERS"]))
 
     # Join original params dictionary with command line specified arguments.
     # NOTE that command line arguments overwrite all previously set parameters.
     params.update(cmd_args)
 
     if params["LOAD_STATE"]:
         # Load run from state.
-        from talos.utilities.algorithm.state import load_state
+        from autooc.utilities.algorithm.state import load_state
 
         # Load in state information.
         individuals = load_state(params["LOAD_STATE"])
 
         # Set correct search loop.
-        from talos.algorithm.search_loop import search_loop_from_state
+        from autooc.algorithm.search_loop import search_loop_from_state
 
         params["SEARCH_LOOP"] = search_loop_from_state
 
         # Set population.
         setattr(trackers, "state_individuals", individuals)
 
     else:
@@ -332,29 +332,29 @@
                         "fitness functions."
                     )
                     raise Exception(s)
 
         # Parse grammar file and set grammar class.
         params["BNF_GRAMMAR"] = grammar.Grammar(
             params["GRAMMAR_FILE"]
-            #path.join("talos", "grammars", params["GRAMMAR_FILE"])
+            #path.join("autooc", "grammars", params["GRAMMAR_FILE"])
             #path.join(path.dirname(path.abspath(__file__)), "..", "grammars", params["GRAMMAR_FILE"])
         )
 
         # Population loading for seeding runs (if specified)
         if params["TARGET_SEED_FOLDER"]:
 
             # Import population loading function.
-            from talos.operators.initialisation import load_population
+            from autooc.operators.initialisation import load_population
 
             # A target folder containing seed individuals has been given.
             params["SEED_INDIVIDUALS"] = load_population(
                 params["TARGET_SEED_FOLDER"])
 
         elif params["REVERSE_MAPPING_TARGET"]:
             # A single seed phenotype has been given. Parse and run.
 
             # Import GE LR Parser.
-            from talos.scripts import GE_LR_parser
+            from autooc.scripts import GE_LR_parser
 
             # Parse seed individual and store in params.
             params["SEED_INDIVIDUALS"] = [GE_LR_parser.main()]
```

### Comparing `autooc-0.0.8/autooc/algorithm/search_loop.py` & `autooc-0.0.9/autooc/algorithm/search_loop.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from multiprocessing import Pool
 
-from talos.algorithm.parameters import params
-from talos.fitness.evaluation import evaluate_fitness
-from talos.operators.initialisation import initialisation
-from talos.stats.stats import get_stats, stats
-from talos.utilities.algorithm.initialise_run import pool_init
-from talos.utilities.stats import trackers
+from autooc.algorithm.parameters import params
+from autooc.fitness.evaluation import evaluate_fitness
+from autooc.operators.initialisation import initialisation
+from autooc.stats.stats import get_stats, stats
+from autooc.utilities.algorithm.initialise_run import pool_init
+from autooc.utilities.stats import trackers
 
 
 def search_loop():
     """
     This is a standard search process for an evolutionary algorithm. Loop over
     a given number of generations.
```

### Comparing `autooc-0.0.8/autooc/algorithm/step.py` & `autooc-0.0.9/autooc/algorithm/step.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,13 +1,13 @@
-from talos.fitness.evaluation import evaluate_fitness
-from talos.operators.crossover import crossover
-from talos.operators.mutation import mutation
-from talos.operators.replacement import replacement, steady_state
-from talos.operators.selection import selection
-from talos.stats.stats import get_stats
+from autooc.fitness.evaluation import evaluate_fitness
+from autooc.operators.crossover import crossover
+from autooc.operators.mutation import mutation
+from autooc.operators.replacement import replacement, steady_state
+from autooc.operators.selection import selection
+from autooc.stats.stats import get_stats
 
 
 def step(individuals):
     """
     Runs a single generation of the evolutionary algorithm process:
         Selection
         Variation
```

### Comparing `autooc-0.0.8/autooc/autooc.py` & `autooc-0.0.9/autooc/autooc.py`

 * *Files 1% similar despite different names*

```diff
@@ -11,21 +11,21 @@
 #import pygmo as pg
 from mlflow.tracking import MlflowClient
 from sklearn.metrics import *
 from sklearn.model_selection import train_test_split
 from sklearn.preprocessing import MinMaxScaler
 from tqdm import tqdm
 
-from talos.algorithm.parameters import params, set_params
-from talos.fitness.evaluation import evaluate_fitness
-from talos.operators.initialisation import initialisation
-from talos.stats.stats import get_stats, stats
-from talos.utilities.algorithm.general import check_python_version
-from talos.utilities.algorithm.initialise_run import initialise_run_params
-from talos.utilities.algorithm.NSGA2 import compute_pareto_metrics
+from autooc.algorithm.parameters import params, set_params
+from autooc.fitness.evaluation import evaluate_fitness
+from autooc.operators.initialisation import initialisation
+from autooc.stats.stats import get_stats, stats
+from autooc.utilities.algorithm.general import check_python_version
+from autooc.utilities.algorithm.initialise_run import initialise_run_params
+from autooc.utilities.algorithm.NSGA2 import compute_pareto_metrics
 
 check_python_version()
 
 
 class AutoOC(object):
     def __init__(self, anomaly_class: str, normal_class: str, multiobjective: bool = False, algorithm: str = "all", performance_metric: str = "num_params", multicore: bool = False):
         #self.params = params.copy()
```

### Comparing `autooc-0.0.8/autooc/fitness/base_ff_classes/base_ff.py` & `autooc-0.0.9/autooc/fitness/base_ff_classes/base_ff.py`

 * *Files identical despite different names*

### Comparing `autooc-0.0.8/autooc/fitness/base_ff_classes/ff_template.py` & `autooc-0.0.9/autooc/fitness/base_ff_classes/ff_template.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-from talos.fitness.base_ff_classes.base_ff import base_ff
+from autooc.fitness.base_ff_classes.base_ff import base_ff
 
 
 class ff_template(base_ff):
     """
     Basic fitness function template for writing new fitness functions. This
     basic template inherits from the base fitness function class, which
     contains various checks and balances.
```

### Comparing `autooc-0.0.8/autooc/fitness/base_ff_classes/moo_ff.py` & `autooc-0.0.9/autooc/fitness/base_ff_classes/moo_ff.py`

 * *Files identical despite different names*

### Comparing `autooc-0.0.8/autooc/fitness/evaluation.py` & `autooc-0.0.9/autooc/fitness/evaluation.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 import numpy as np
 
-from talos.algorithm.parameters import params
-from talos.stats.stats import stats
-from talos.utilities.stats.trackers import cache, runtime_error_cache
+from autooc.algorithm.parameters import params
+from autooc.stats.stats import stats
+from autooc.utilities.stats.trackers import cache, runtime_error_cache
 
 
 def evaluate_fitness(individuals):
     """
     Evaluate an entire population of individuals. Invalid individuals are given
     a default bad fitness. If params['CACHE'] is specified then individuals
     have their fitness stored in a dictionary called utilities.trackers.cache.
```

### Comparing `autooc-0.0.8/autooc/fitness/multi_objective/binary_phenotype_to_float.py` & `autooc-0.0.9/autooc/fitness/multi_objective/binary_phenotype_to_float.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,9 +1,9 @@
-from talos.fitness.base_ff_classes.base_ff import base_ff
-from talos.utilities.fitness.math_functions import binary_phen_to_float
+from autooc.fitness.base_ff_classes.base_ff import base_ff
+from autooc.utilities.fitness.math_functions import binary_phen_to_float
 
 
 class binary_phenotype_to_float(base_ff):
 
     """
     Fitness function for the first problem (T_1) presented in
     [Zitzler2000].
```

### Comparing `autooc-0.0.8/autooc/fitness/multi_objective/singlefit_autoencoders.py` & `autooc-0.0.9/autooc/fitness/multi_objective/singlefit_autoencoders.py`

 * *Files 9% similar despite different names*

```diff
@@ -11,18 +11,18 @@
 import numpy as np
 # imports relative to keras model (ind.phenotype)
 from tensorflow.keras import Input, Sequential
 from tensorflow.keras.callbacks import EarlyStopping
 from tensorflow.keras.layers import BatchNormalization, Dense, Dropout
 from tensorflow.keras.utils import plot_model
 
-from talos.algorithm.parameters import params
-from talos.fitness.base_ff_classes.base_ff import base_ff
-from talos.stats.stats import stats
-from talos.utilities.utils import get_model_from_encoder
+from autooc.algorithm.parameters import params
+from autooc.fitness.base_ff_classes.base_ff import base_ff
+from autooc.stats.stats import stats
+from autooc.utilities.utils import get_model_from_encoder
 
 
 class singlefit_autoencoders(base_ff):
     """
     An example of a single fitness class that generates
     two fitness values for multi-objective optimisation
     """
```

### Comparing `autooc-0.0.8/autooc/fitness/multi_objective/singlefit_multiobj.py` & `autooc-0.0.9/autooc/fitness/multi_objective/singlefit_multiobj.py`

 * *Files 5% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 """
 @author: Jonathan Byrne
 @17/01/18 11:09
 """
 
 import numpy as np
 
-from talos.fitness.base_ff_classes.base_ff import base_ff
+from autooc.fitness.base_ff_classes.base_ff import base_ff
 
 
 class singlefit_multiobj(base_ff):
     """
     An example of a single fitness class that generates
     two fitness values for multi-objective optimisation
     """
```

### Comparing `autooc-0.0.8/autooc/fitness/multi_objective/zdt1.py` & `autooc-0.0.9/autooc/fitness/multi_objective/zdt1.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 from math import sqrt
 
-from talos.algorithm.fitness.math_functions import binary_phen_to_float
-from talos.fitness.base_ff_classes.base_ff import base_ff
+from autooc.algorithm.fitness.math_functions import binary_phen_to_float
+from autooc.fitness.base_ff_classes.base_ff import base_ff
 
 
 class zdt1(base_ff):
     """
     Fitness function for the first problem (T_1) presented in
     [Zitzler2000].
```

### Comparing `autooc-0.0.8/autooc/fitness/progsys.py` & `autooc-0.0.9/autooc/fitness/progsys.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 import json
 import subprocess
 import sys
 from os import path
 
-from talos.algorithm.parameters import params
-from talos.fitness.base_ff_classes.base_ff import base_ff
+from autooc.algorithm.parameters import params
+from autooc.fitness.base_ff_classes.base_ff import base_ff
 
 
 class progsys(base_ff):
     """Fitness function for program synthesis problems. Grammars and datasets
     for 29 benchmark problems from doi.org/10.1145/2739480.2754769 are
     provided. Evaluation is done in a separate python process."""
```

### Comparing `autooc-0.0.8/autooc/fitness/pymax.py` & `autooc-0.0.9/autooc/fitness/pymax.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-from talos.fitness.base_ff_classes.base_ff import base_ff
+from autooc.fitness.base_ff_classes.base_ff import base_ff
 
 
 class pymax(base_ff):
     """
     Py-max is a max-style problem where the goal is to generate a function
     which outputs a large number. In the standard GP Max [Gathercole and
     Ross] problem this function can only use the constant (0.5) and functions
```

### Comparing `autooc-0.0.8/autooc/fitness/sequence_match.py` & `autooc-0.0.9/autooc/fitness/sequence_match.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 import dtw  # https://pypi.python.org/pypi/dtw
 import editdistance  # https://pypi.python.org/pypi/editdistance
 import lzstring  # https://pypi.python.org/pypi/lzstring/
 
-from talos.algorithm.parameters import params
-from talos.fitness.base_ff_classes.base_ff import base_ff
+from autooc.algorithm.parameters import params
+from autooc.fitness.base_ff_classes.base_ff import base_ff
 
 """
 
 This fitness function is for a sequence-match problem: we're given
 an integer sequence target, say [0, 5, 0, 5, 0, 5], and we try to synthesize a
 program (loops, if-statements, etc) which will *yield* that sequence,
 one item at a time.
```

### Comparing `autooc-0.0.8/autooc/fitness/string_match.py` & `autooc-0.0.9/autooc/fitness/string_match.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,9 +1,9 @@
-from talos.algorithm.parameters import params
-from talos.fitness.base_ff_classes.base_ff import base_ff
+from autooc.algorithm.parameters import params
+from autooc.fitness.base_ff_classes.base_ff import base_ff
 
 
 class string_match(base_ff):
     """Fitness function for matching a string. Takes a string and returns
     fitness. Penalises output that is not the same length as the target.
     Penalty given to individual string components which do not match ASCII
     value of target."""
```

### Comparing `autooc-0.0.8/autooc/fitness/supervised_learning/boolean_problem.py` & `autooc-0.0.9/autooc/fitness/supervised_learning/boolean_problem.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 import itertools
 import random
 
 import numpy as np
 
-from talos.algorithm.parameters import params
-from talos.fitness.supervised_learning.supervised_learning import \
+from autooc.algorithm.parameters import params
+from autooc.fitness.supervised_learning.supervised_learning import \
     supervised_learning
-from talos.utilities.fitness.error_metric import Hamming_error
+from autooc.utilities.fitness.error_metric import Hamming_error
 
 
 class boolean_problem(supervised_learning):
     """Fitness function for Boolean problems. We specialise the
     supervised learning fitness function.
 
     The user must pass in the name of the target function, and n_vars.
```

### Comparing `autooc-0.0.8/autooc/fitness/supervised_learning/classification.py` & `autooc-0.0.9/autooc/fitness/supervised_learning/classification.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,11 +1,11 @@
-from talos.algorithm.parameters import params
-from talos.fitness.supervised_learning.supervised_learning import \
+from autooc.algorithm.parameters import params
+from autooc.fitness.supervised_learning.supervised_learning import \
     supervised_learning
-from talos.utilities.fitness.error_metric import f1_score
+from autooc.utilities.fitness.error_metric import f1_score
 
 
 class classification(supervised_learning):
     """Fitness function for classification. We just slightly specialise the
     function for supervised_learning."""
 
     def __init__(self):
```

### Comparing `autooc-0.0.8/autooc/fitness/supervised_learning/if_else_classifier.py` & `autooc-0.0.9/autooc/fitness/supervised_learning/if_else_classifier.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 import itertools
 import random
 
 import numpy as np
 
-from talos.algorithm.parameters import params
-from talos.fitness.supervised_learning.supervised_learning import \
+from autooc.algorithm.parameters import params
+from autooc.fitness.supervised_learning.supervised_learning import \
     supervised_learning
-from talos.utilities.fitness.error_metric import Hamming_error
+from autooc.utilities.fitness.error_metric import Hamming_error
 
 
 class if_else_classifier(supervised_learning):
     """Fitness function for if-else classifier problems. We
     specialise the supervised learning fitness function.
 
     The user must pass in n_vars, n_is, n_os (number of variables,
```

### Comparing `autooc-0.0.8/autooc/fitness/supervised_learning/regression.py` & `autooc-0.0.9/autooc/fitness/supervised_learning/regression.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,11 +1,11 @@
-from talos.algorithm.parameters import params
-from talos.fitness.supervised_learning.supervised_learning import \
+from autooc.algorithm.parameters import params
+from autooc.fitness.supervised_learning.supervised_learning import \
     supervised_learning
-from talos.utilities.fitness.error_metric import rmse
+from autooc.utilities.fitness.error_metric import rmse
 
 
 class regression(supervised_learning):
     """Fitness function for regression. We just slightly specialise the
     function for supervised_learning."""
 
     def __init__(self):
```

### Comparing `autooc-0.0.8/autooc/fitness/supervised_learning/regression_random_polynomial.py` & `autooc-0.0.9/autooc/fitness/supervised_learning/regression_random_polynomial.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import itertools
 import random
 
 import numpy as np
 
-from talos.algorithm.parameters import params
-from talos.fitness.supervised_learning.regression import regression
-from talos.utilities.fitness.error_metric import rmse
+from autooc.algorithm.parameters import params
+from autooc.fitness.supervised_learning.regression import regression
+from autooc.utilities.fitness.error_metric import rmse
 
 
 class regression_random_polynomial(regression):
     """Fitness function for regression of random polynomials. We
     specialise the regression fitness function.
 
     The user must pass in the degree, n_vars, and n_samples. A random
```

### Comparing `autooc-0.0.8/autooc/fitness/supervised_learning/supervised_learning.py` & `autooc-0.0.9/autooc/fitness/supervised_learning/supervised_learning.py`

 * *Files 3% similar despite different names*

```diff
@@ -8,22 +8,22 @@
 from sklearn.neighbors import LocalOutlierFactor
 from sklearn.svm import OneClassSVM
 from tensorflow.keras import Input, Sequential
 from tensorflow.keras.callbacks import EarlyStopping
 from tensorflow.keras.layers import BatchNormalization, Dense, Dropout, Input
 from tensorflow.keras.utils import plot_model
 
-from talos.algorithm.parameters import params
-from talos.fitness.base_ff_classes.base_ff import base_ff
-from talos.stats.stats import stats
-from talos.utilities.fitness.error_metric import (auc_autoencoder, auc_sklearn,
+from autooc.algorithm.parameters import params
+from autooc.fitness.base_ff_classes.base_ff import base_ff
+from autooc.stats.stats import stats
+from autooc.utilities.fitness.error_metric import (auc_autoencoder, auc_sklearn,
                                                   reconstruction_error)
-from talos.utilities.fitness.get_data import get_data
-from talos.utilities.fitness.optimize_constants import optimize_constants
-from talos.utilities.utils import (get_model_from_encoder,
+from autooc.utilities.fitness.get_data import get_data
+from autooc.utilities.fitness.optimize_constants import optimize_constants
+from autooc.utilities.utils import (get_model_from_encoder,
                                    get_model_from_encoder2)
 
 np.seterr(all="raise")
 
 
 class supervised_learning(base_ff):
     """
```

### Comparing `autooc-0.0.8/autooc/fitness/supervised_learning/supervised_learning_backup.py` & `autooc-0.0.9/autooc/fitness/supervised_learning/supervised_learning_backup.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 import numpy as np
 
-from talos.algorithm.parameters import params
-from talos.fitness.base_ff_classes.base_ff import base_ff
-from talos.utilities.fitness.get_data import get_data
-from talos.utilities.fitness.math_functions import *
-from talos.utilities.fitness.optimize_constants import optimize_constants
+from autooc.algorithm.parameters import params
+from autooc.fitness.base_ff_classes.base_ff import base_ff
+from autooc.utilities.fitness.get_data import get_data
+from autooc.utilities.fitness.math_functions import *
+from autooc.utilities.fitness.optimize_constants import optimize_constants
 
 np.seterr(all="raise")
 
 
 class supervised_learning(base_ff):
     """
     Fitness function for supervised learning, ie regression and
```

### Comparing `autooc-0.0.8/autooc/operators/crossover.py` & `autooc-0.0.9/autooc/operators/crossover.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 from random import choice, randint, random, sample
 
-from talos.algorithm.parameters import params
-from talos.representation import individual
-from talos.representation.latent_tree import (latent_tree_crossover,
+from autooc.algorithm.parameters import params
+from autooc.representation import individual
+from autooc.representation.latent_tree import (latent_tree_crossover,
                                               latent_tree_repair)
-from talos.utilities.representation.check_methods import check_ind
+from autooc.utilities.representation.check_methods import check_ind
 
 
 def crossover(parents):
     """
     Perform crossover on a population of individuals. The size of the crossover
     population is defined as params['GENERATION_SIZE'] rather than params[
     'POPULATION_SIZE']. This saves on wasted evaluations and prevents search
```

### Comparing `autooc-0.0.8/autooc/operators/initialisation.py` & `autooc-0.0.9/autooc/operators/initialisation.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,19 +1,19 @@
 from math import floor
 from os import getcwd, listdir, path
 from random import randint, shuffle
 
-from talos.algorithm.parameters import params
-from talos.representation import individual
-from talos.representation.derivation import generate_tree, pi_grow
-from talos.representation.individual import Individual
-from talos.representation.latent_tree import latent_tree_random_ind
-from talos.representation.tree import Tree
-from talos.scripts import GE_LR_parser
-from talos.utilities.representation.python_filter import python_filter
+from autooc.algorithm.parameters import params
+from autooc.representation import individual
+from autooc.representation.derivation import generate_tree, pi_grow
+from autooc.representation.individual import Individual
+from autooc.representation.latent_tree import latent_tree_random_ind
+from autooc.representation.tree import Tree
+from autooc.scripts import GE_LR_parser
+from autooc.utilities.representation.python_filter import python_filter
 
 
 def initialisation(size):
     """
     Perform selection on a population in order to select a population of
     individuals for variation.
```

### Comparing `autooc-0.0.8/autooc/operators/mutation.py` & `autooc-0.0.9/autooc/operators/mutation.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from random import choice, randint, random
 
-from talos.algorithm.parameters import params
-from talos.representation import individual
-from talos.representation.derivation import generate_tree
-from talos.representation.latent_tree import (latent_tree_mutate,
+from autooc.algorithm.parameters import params
+from autooc.representation import individual
+from autooc.representation.derivation import generate_tree
+from autooc.representation.latent_tree import (latent_tree_mutate,
                                               latent_tree_repair)
-from talos.utilities.representation.check_methods import check_ind
+from autooc.utilities.representation.check_methods import check_ind
 
 
 def mutation(pop):
     """
     Perform mutation on a population of individuals. Calls mutation operator as
     specified in params dictionary.
```

### Comparing `autooc-0.0.8/autooc/operators/replacement.py` & `autooc-0.0.9/autooc/operators/replacement.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,13 @@
-from talos.algorithm.parameters import params
-from talos.fitness.evaluation import evaluate_fitness
-from talos.operators.crossover import crossover_inds
-from talos.operators.mutation import mutation
-from talos.operators.selection import selection
-from talos.utilities.algorithm.NSGA2 import compute_pareto_metrics
+from autooc.algorithm.parameters import params
+from autooc.fitness.evaluation import evaluate_fitness
+from autooc.operators.crossover import crossover_inds
+from autooc.operators.mutation import mutation
+from autooc.operators.selection import selection
+from autooc.utilities.algorithm.NSGA2 import compute_pareto_metrics
 
 
 def replacement(new_pop, old_pop):
     """
     Given a new population and an old population, performs replacement using
     specified replacement operator.
```

### Comparing `autooc-0.0.8/autooc/operators/selection.py` & `autooc-0.0.9/autooc/operators/selection.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 from random import sample
 
-from talos.algorithm.parameters import params
-from talos.utilities.algorithm.NSGA2 import (compute_pareto_metrics,
+from autooc.algorithm.parameters import params
+from autooc.utilities.algorithm.NSGA2 import (compute_pareto_metrics,
                                              crowded_comparison_operator)
 
 
 def selection(population):
     """
     Perform selection on a population in order to select a population of
     individuals for variation.
```

### Comparing `autooc-0.0.8/autooc/operators/subtree_parse.py` & `autooc-0.0.9/autooc/operators/subtree_parse.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 import re
 from copy import copy
 from itertools import zip_longest
 
-from talos.algorithm.parameters import params
-from talos.representation import individual, tree
-from talos.utilities.representation.check_methods import (generate_codon,
+from autooc.algorithm.parameters import params
+from autooc.representation import individual, tree
+from autooc.utilities.representation.check_methods import (generate_codon,
                                                           get_output)
-from talos.utilities.stats import trackers
+from autooc.utilities.stats import trackers
 
 
 def combine_snippets():
     """
     As the snippets repository grows, we can start to combine
     neighboring snippets to build bigger snippets. Eventually we hope this
     can just build the perfect solution. Iteratively builds snippets until
```

### Comparing `autooc-0.0.8/autooc/representation/derivation.py` & `autooc-0.0.9/autooc/representation/derivation.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from random import choice, randint, randrange
 
-from talos.algorithm.parameters import params
-from talos.representation.tree import Tree
-from talos.utilities.representation.check_methods import (get_nodes_and_depth,
+from autooc.algorithm.parameters import params
+from autooc.representation.tree import Tree
+from autooc.utilities.representation.check_methods import (get_nodes_and_depth,
                                                           ret_true)
 
 
 def generate_tree(tree, genome, output, method, nodes, depth, max_depth, depth_limit):
     """
     Recursive function to derive a tree using a given method.
```

### Comparing `autooc-0.0.8/autooc/representation/grammar.py` & `autooc-0.0.9/autooc/representation/grammar.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from math import floor
 from re import DOTALL, MULTILINE, finditer, match
 from sys import maxsize
 
-from talos.algorithm.parameters import params
+from autooc.algorithm.parameters import params
 
 
 class Grammar(object):
     """
     Parser for Backus-Naur Form (BNF) Context-Free Grammars.
     """
```

### Comparing `autooc-0.0.8/autooc/representation/individual.py` & `autooc-0.0.9/autooc/representation/individual.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import time
 
 import numpy as np
 import pandas as pd
 import tensorflow as tf
 
-from talos.algorithm.mapper import mapper
-from talos.algorithm.parameters import params
+from autooc.algorithm.mapper import mapper
+from autooc.algorithm.parameters import params
 
 
 class Individual(object):
     """
     A GE individual.
     """
```

### Comparing `autooc-0.0.8/autooc/representation/latent_tree.py` & `autooc-0.0.9/autooc/representation/latent_tree.py`

 * *Files 1% similar despite different names*

```diff
@@ -26,16 +26,16 @@
 derivation trees.
 
 """
 
 
 import random
 
-from talos.algorithm.parameters import params
-from talos.representation.derivation import legal_productions
+from autooc.algorithm.parameters import params
+from autooc.representation.derivation import legal_productions
 
 
 def latent_tree_random_ind(grammar, maxdepth, old_genome=None):
     """Generate a random individual (genome and string), OR repair a
     genome and generate its string. These two things are conceptually
     distinct, but they share almost all code. The idea is that
     repairing a genome consists of traversing it and using its choices
```

### Comparing `autooc-0.0.8/autooc/representation/tree.py` & `autooc-0.0.9/autooc/representation/tree.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-from talos.algorithm.parameters import params
+from autooc.algorithm.parameters import params
 
 
 class Tree:
     def __init__(self, expr, parent):
         """
         Initialise an instance of the tree class.
```

### Comparing `autooc-0.0.8/autooc/scripts/GE_LR_parser.py` & `autooc-0.0.9/autooc/scripts/GE_LR_parser.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,19 +1,19 @@
 import sys
 from sys import path
 
-from talos.algorithm.parameters import params, set_params
-from talos.operators.subtree_parse import (check_snippets_for_solution,
+from autooc.algorithm.parameters import params, set_params
+from autooc.operators.subtree_parse import (check_snippets_for_solution,
                                            generate_key_and_check,
                                            get_NT_from_str, get_num_from_str)
-from talos.representation.tree import Tree
-from talos.utilities.algorithm.general import check_python_version
-from talos.utilities.representation.check_methods import (
+from autooc.representation.tree import Tree
+from autooc.utilities.algorithm.general import check_python_version
+from autooc.utilities.representation.check_methods import (
     check_ind_from_parser, generate_codon)
-from talos.utilities.stats import trackers
+from autooc.utilities.stats import trackers
 
 path.append("../src")
 
 
 check_python_version()
```

### Comparing `autooc-0.0.8/autooc/scripts/baselines.py` & `autooc-0.0.9/autooc/scripts/baselines.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 #!/usr/bin/env python
 import sys
 from collections import Counter
 
 import numpy as np
 from sklearn.linear_model import ElasticNet, LinearRegression
 
-from talos.algorithm.fitness.get_data import get_data
+from autooc.algorithm.fitness.get_data import get_data
 
 
 def pprint(a, format_string="{0:.2f}"):
     """
     Function to pretty print a array without scientific notation and with given
     precision.
```

### Comparing `autooc-0.0.8/autooc/scripts/experiment_manager.py` & `autooc-0.0.9/autooc/scripts/experiment_manager.py`

 * *Files 2% similar despite different names*

```diff
@@ -4,17 +4,17 @@
     Copyright (c) 2014 Michael Fenton
     Hereby licensed under the GNU GPL v3."""
 import sys
 from multiprocessing import Pool
 from subprocess import call
 from sys import path
 
-from talos.algorithm.algorithm.general import check_python_version
-from talos.algorithm.parameters import params, set_params
-from talos.scripts.stats_parser import parse_stats_from_runs
+from autooc.algorithm.algorithm.general import check_python_version
+from autooc.algorithm.parameters import params, set_params
+from autooc.scripts.stats_parser import parse_stats_from_runs
 
 path.append("../src")
 
 
 check_python_version()
```

### Comparing `autooc-0.0.8/autooc/scripts/grammar_analyser.py` & `autooc-0.0.9/autooc/scripts/grammar_analyser.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,17 +1,17 @@
 import os
 import sys
 from sys import path
 
 import utilities.algorithm.command_line_parser as parser
 
-from talos.algorithm.algorithm.general import check_python_version
-from talos.algorithm.fitness.math_functions import sci_notation
-from talos.algorithm.parameters import params
-from talos.representation.grammar import Grammar
+from autooc.algorithm.algorithm.general import check_python_version
+from autooc.algorithm.fitness.math_functions import sci_notation
+from autooc.algorithm.parameters import params
+from autooc.representation.grammar import Grammar
 
 path.append("../src")
 
 
 check_python_version()
```

### Comparing `autooc-0.0.8/autooc/scripts/python_script_evaluation.py` & `autooc-0.0.9/autooc/scripts/python_script_evaluation.py`

 * *Files identical despite different names*

### Comparing `autooc-0.0.8/autooc/scripts/stats_parser.py` & `autooc-0.0.9/autooc/scripts/stats_parser.py`

 * *Files 2% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 from sys import path
 
 import matplotlib
 import matplotlib.pyplot as plt
 import numpy as np
 import pandas as pd
 
-from talos.algorithm.algorithm.general import check_python_version
+from autooc.algorithm.algorithm.general import check_python_version
 
 path.append("../src")
 
 
 check_python_version()
 
 
@@ -131,15 +131,15 @@
     ./results folder which holds multiple runs.
     :param graph: A boolean flag for whether or not to save figure.
     :return: Nothing.
     """
 
     # Since results files are not kept in source directory, need to escape
     # one folder.
-    file_path = path.join(getcwd(), "talos", "results")
+    file_path = path.join(getcwd(), "autooc", "results")
 
     # Check for use of experiment manager.
     if experiment_name:
         file_path = path.join(file_path, experiment_name)
 
     else:
         s = (
```

### Comparing `autooc-0.0.8/autooc/stats/stats.py` & `autooc-0.0.9/autooc/stats/stats.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,22 +1,22 @@
 from copy import copy
 from sys import stdout
 from time import time
 
 import numpy as np
 
-from talos.algorithm.parameters import params
-from talos.utilities.algorithm.NSGA2 import compute_pareto_metrics
-from talos.utilities.algorithm.state import create_state
-from talos.utilities.stats import trackers
-from talos.utilities.stats.file_io import (save_best_ind_to_file,
+from autooc.algorithm.parameters import params
+from autooc.utilities.algorithm.NSGA2 import compute_pareto_metrics
+from autooc.utilities.algorithm.state import create_state
+from autooc.utilities.stats import trackers
+from autooc.utilities.stats.file_io import (save_best_ind_to_file,
                                            save_first_front_to_file,
                                            save_stats_headers,
                                            save_stats_to_file)
-from talos.utilities.stats.save_plots import (save_pareto_fitness_plot,
+from autooc.utilities.stats.save_plots import (save_pareto_fitness_plot,
                                               save_plot_from_data)
 
 """Algorithm statistics"""
 stats = {
     "gen": 0,
     "total_inds": 0,
     "regens": 0,
```

### Comparing `autooc-0.0.8/autooc/utilities/algorithm/NSGA2.py` & `autooc-0.0.9/autooc/utilities/algorithm/NSGA2.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 from collections import defaultdict
 
 from numpy import isnan
 
-from talos.algorithm.parameters import params
-from talos.utilities.fitness.math_functions import percentile
+from autooc.algorithm.parameters import params
+from autooc.utilities.fitness.math_functions import percentile
 
 
 def compute_pareto_metrics(population):
     """
     Compute the pareto fronts using NSGA-II.
 
     :param population: A population to be sorted into fronts using NSGA-II.
```

### Comparing `autooc-0.0.8/autooc/utilities/algorithm/command_line_parser.py` & `autooc-0.0.9/autooc/utilities/algorithm/command_line_parser.py`

 * *Files identical despite different names*

### Comparing `autooc-0.0.8/autooc/utilities/algorithm/initialise_run.py` & `autooc-0.0.9/autooc/utilities/algorithm/initialise_run.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,17 +1,17 @@
 import importlib
 from datetime import datetime
 from os import getpid
 from random import seed
 from socket import gethostname
 from time import time
 
-from talos.algorithm.parameters import params
-from talos.utilities.stats import trackers
-from talos.utilities.stats.file_io import generate_folders_and_files
+from autooc.algorithm.parameters import params
+from autooc.utilities.stats import trackers
+from autooc.utilities.stats.file_io import generate_folders_and_files
 
 
 def initialise_run_params(create_files):
     """
     Initialises all lists and trackers. Generates save folders and initial
     parameter files if debugging is not active.
 
@@ -71,43 +71,43 @@
     class name matches the file name.
 
     :return: Nothing.
     """
 
     # For these ops we let the param equal the function itself.
     ops = {
-        "talos.operators": [
+        "autooc.operators": [
             "INITIALISATION",
             "SELECTION",
             "CROSSOVER",
             "MUTATION",
             "REPLACEMENT",
         ],
-        "talos.utilities.fitness": ["ERROR_METRIC"],
-        "talos.fitness": ["FITNESS_FUNCTION"],
-        "talos.algorithm": ["SEARCH_LOOP", "STEP"],
+        "autooc.utilities.fitness": ["ERROR_METRIC"],
+        "autooc.fitness": ["FITNESS_FUNCTION"],
+        "autooc.algorithm": ["SEARCH_LOOP", "STEP"],
     }
 
     # We have to take 'algorithm' first as the functions from
     # algorithm need to be imported before any others to prevent
     # circular imports. We have to take 'utilities.fitness' before
     # 'fitness' because ERROR_METRIC has to be set in order to call
     # the fitness function constructor.
 
-    for special_ops in ["talos.algorithm", "talos.utilities.fitness", "talos.operators", "talos.fitness"]:
+    for special_ops in ["autooc.algorithm", "autooc.utilities.fitness", "autooc.operators", "autooc.fitness"]:
 
         if all([callable(params[op]) for op in ops[special_ops]]):
             # params are already functions
             pass
 
         else:
 
             for op in ops[special_ops]:
 
-                if special_ops == "talos.fitness":
+                if special_ops == "autooc.fitness":
                     # Fitness functions represent a special case.
 
                     get_fit_func_imports()
 
                 elif params[op] is not None:
                     # Split import name based on "." to find nested modules.
                     split_name = params[op].split(".")
@@ -233,22 +233,22 @@
 
         for i, name in enumerate(params[op]):
 
             # Split import name based on "." to find nested modules.
             split_name = name.strip().split(".")
 
             # Get module and attribute names.
-            module_path = ".".join(["talos.fitness", name.strip()])
+            module_path = ".".join(["autooc.fitness", name.strip()])
             attr = split_name[-1]
 
             # Import this fitness function.
             params[op][i] = return_attr_from_module(module_path, attr)
 
         # Import base multi-objective fitness function class.
-        from talos.fitness.base_ff_classes.moo_ff import moo_ff
+        from autooc.fitness.base_ff_classes.moo_ff import moo_ff
 
         # Set main fitness function as base multi-objective fitness
         # function class.
         params[op] = moo_ff(params[op])
 
     else:
         # A single fitness function has been specified.
@@ -256,15 +256,15 @@
         # Split import name based on "." to find nested modules.
         split_name = params[op].strip().split(".")
 
         # Get attribute name.
         attr_name = split_name[-1]
 
         # Get module name.
-        module_name = ".".join(["talos.fitness", params[op]])
+        module_name = ".".join(["autooc.fitness", params[op]])
 
         # Import module and attribute and save.
         params[op] = return_attr_from_module(module_name, attr_name)
 
         # Initialise fitness function.
         params[op] = params[op]()
```

### Comparing `autooc-0.0.8/autooc/utilities/algorithm/state.py` & `autooc-0.0.9/autooc/utilities/algorithm/state.py`

 * *Files 2% similar despite different names*

```diff
@@ -12,17 +12,17 @@
 
     :param individuals: A population of individuals to be saved.
     :return: The complete state of a run.
     """
 
     from time import time
 
-    from talos.algorithm.parameters import params
-    from talos.stats.stats import stats
-    from talos.utilities.stats import trackers
+    from autooc.algorithm.parameters import params
+    from autooc.stats.stats import stats
+    from autooc.utilities.stats import trackers
 
     # Get time.
     state_time = time()
 
     # Get random state.
     random_state = random.getstate()
 
@@ -110,18 +110,18 @@
 
     :param state: The complete state of a run.
     :return: A population of individuals.
     """
 
     from time import time
 
-    from talos.algorithm.parameters import params
-    from talos.stats.stats import stats
-    from talos.utilities.algorithm.initialise_run import set_param_imports
-    from talos.utilities.stats import trackers
+    from autooc.algorithm.parameters import params
+    from autooc.stats.stats import stats
+    from autooc.utilities.algorithm.initialise_run import set_param_imports
+    from autooc.utilities.stats import trackers
 
     # Set random state.
     random.setstate(state["random_state"])
 
     # Set stats.
     for stat in state["stats"]:
         stats[stat] = state["stats"][stat]
```

### Comparing `autooc-0.0.8/autooc/utilities/fitness/error_metric.py` & `autooc-0.0.9/autooc/utilities/fitness/error_metric.py`

 * *Files 0% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 import numpy as np
 import tensorflow as tf
 from sklearn.metrics import auc
 from sklearn.metrics import f1_score as sklearn_f1_score
 from sklearn.metrics import log_loss, roc_auc_score
 from tqdm import tqdm
 
-from talos.algorithm.parameters import params
+from autooc.algorithm.parameters import params
 
 
 def mae(y, yhat):
     """
     Calculate mean absolute error between inputs.
 
     :param y: The expected input (i.e. from dataset).
```

### Comparing `autooc-0.0.8/autooc/utilities/fitness/get_data.py` & `autooc-0.0.9/autooc/utilities/fitness/get_data.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from os import path
 
 import numpy as np
 
-from talos.algorithm.parameters import params
+from autooc.algorithm.parameters import params
 
 
 def get_Xy_train_test_separate(train_filename, test_filename, skip_header=0):
     """
     Read in training and testing data files, and split each into X
     (all columns up to last) and y (last column).
```

### Comparing `autooc-0.0.8/autooc/utilities/fitness/math_functions.py` & `autooc-0.0.9/autooc/utilities/fitness/math_functions.py`

 * *Files identical despite different names*

### Comparing `autooc-0.0.8/autooc/utilities/fitness/optimize_constants.py` & `autooc-0.0.9/autooc/utilities/fitness/optimize_constants.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 import re
 
 import scipy
 
-from talos.algorithm.parameters import params
-from talos.utilities.fitness.math_functions import *
+from autooc.algorithm.parameters import params
+from autooc.utilities.fitness.math_functions import *
 
 
 def optimize_constants(x, y, ind):
     """
     Use gradient descent to search for values for the constants in
     ind.phenotype which minimise loss.
```

### Comparing `autooc-0.0.8/autooc/utilities/representation/check_methods.py` & `autooc-0.0.9/autooc/utilities/representation/check_methods.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 import numpy as np
 
-from talos.algorithm.parameters import params
-from talos.representation import individual
+from autooc.algorithm.parameters import params
+from autooc.representation import individual
 
 
 def check_ind(ind, check):
     """
     Check all shallow aspects of an individual to ensure everything is correct.
 
     :param ind: An individual to be checked.
```

### Comparing `autooc-0.0.8/autooc/utilities/representation/python_filter.py` & `autooc-0.0.9/autooc/utilities/representation/python_filter.py`

 * *Files identical despite different names*

### Comparing `autooc-0.0.8/autooc/utilities/stats/file_io.py` & `autooc-0.0.9/autooc/utilities/stats/file_io.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 import pickle
 from copy import copy
 from os import getcwd, makedirs, path
 from shutil import rmtree
 
-from talos.algorithm.parameters import params
-from talos.utilities.stats import trackers
+from autooc.algorithm.parameters import params
+from autooc.utilities.stats import trackers
 
 
 def save_stats_to_file(stats, end=False):
     """
     Write the results to a results file for later analysis
 
     :param stats: The stats.stats.stats dictionary.
```

### Comparing `autooc-0.0.8/autooc/utilities/stats/save_plots.py` & `autooc-0.0.9/autooc/utilities/stats/save_plots.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,29 +1,29 @@
 from os import path, pathsep
 
 import matplotlib
 import matplotlib.pyplot as plt
 import numpy as np
 import pandas as pd
 
-from talos.utilities.stats.trackers import first_pareto_list
+from autooc.utilities.stats.trackers import first_pareto_list
 
 matplotlib.use("Agg")
 
 plt.rc("font", family="Times New Roman")
 
 
 def save_pareto_fitness_plot():
     """
     Saves a plot of the current fitness for a pareto front.
 
     :return: Nothing
     """
 
-    from talos.algorithm.parameters import params
+    from autooc.algorithm.parameters import params
 
     # Initialise up figure instance.
     fig = plt.figure()
     ax1 = fig.add_subplot(1, 1, 1)
 
     # Set up iterator for color plotting.
     color = iter(plt.cm.jet(np.linspace(0, 1, len(first_pareto_list))))
@@ -74,15 +74,15 @@
     Saves a plot of a given set of data.
 
     :param data: the data to be plotted
     :param name: the name of the data to be plotted.
     :return: Nothing.
     """
 
-    from talos.algorithm.parameters import params
+    from autooc.algorithm.parameters import params
 
     # Initialise up figure instance.
     fig = plt.figure()
     ax1 = fig.add_subplot(1, 1, 1)
 
     # Plot data.
     ax1.plot(data)
@@ -146,15 +146,15 @@
     :param names: A list of names of that data.
     :param title: The title of the plot.
     :return: Nothing
     """
 
     import matplotlib.pyplot as plt
 
-    from talos.algorithm.parameters import params
+    from autooc.algorithm.parameters import params
 
     plt.rc("font", family="Times New Roman")
 
     # Set up the figure.
     fig = plt.figure()
     ax1 = fig.add_subplot(1, 1, 1)
```

### Comparing `autooc-0.0.8/autooc/utilities/stats/trackers.py` & `autooc-0.0.9/autooc/utilities/stats/trackers.py`

 * *Files identical despite different names*

### Comparing `autooc-0.0.8/autooc/utilities/utils.py` & `autooc-0.0.9/autooc/utilities/utils.py`

 * *Files identical despite different names*

### Comparing `autooc-0.0.8/autooc.egg-info/PKG-INFO` & `autooc-0.0.9/autooc.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: autooc
-Version: 0.0.8
+Version: 0.0.9
 Summary: AutoOC: Automated Machine Learning (AutoML) library for One-Class Learning
 Home-page: https://github.com/luisferreira97/AutoOC
 Author: Luís Ferreira
 Author-email: luis_ferreira223@hotmail.com
 Keywords: automl,machine learning,one-class learning,one-class classification,autoencoder,isolation forest,one-class svm
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: autooc Version: 0.0.8 Summary: AutoOC: Automated
+Metadata-Version: 2.1 Name: autooc Version: 0.0.9 Summary: AutoOC: Automated
 Machine Learning (AutoML) library for One-Class Learning Home-page: https://
 github.com/luisferreira97/AutoOC Author: LuÃ­s Ferreira Author-email:
 luis_ferreira223@hotmail.com Keywords: automl,machine learning,one-class
 learning,one-class classification,autoencoder,isolation forest,one-class svm
 Classifier: Programming Language :: Python :: 3 Classifier: License :: OSI
 Approved :: MIT License Classifier: Operating System :: OS Independent
 Requires-Python: >=3.6, <3.9 Description-Content-Type: text/markdown License-
```

### Comparing `autooc-0.0.8/autooc.egg-info/SOURCES.txt` & `autooc-0.0.9/autooc.egg-info/SOURCES.txt`

 * *Files 18% similar despite different names*

```diff
@@ -43,14 +43,23 @@
 autooc/fitness/supervised_learning/boolean_problem.py
 autooc/fitness/supervised_learning/classification.py
 autooc/fitness/supervised_learning/if_else_classifier.py
 autooc/fitness/supervised_learning/regression.py
 autooc/fitness/supervised_learning/regression_random_polynomial.py
 autooc/fitness/supervised_learning/supervised_learning.py
 autooc/fitness/supervised_learning/supervised_learning_backup.py
+autooc/grammars/autoencoders.bnf
+autooc/grammars/autoencoders.pybnf
+autooc/grammars/autoencoders_v2.pybnf
+autooc/grammars/autoencoders_v3.pybnf
+autooc/grammars/autoencoders_v4.pybnf
+autooc/grammars/iforest.pybnf
+autooc/grammars/lof.pybnf
+autooc/grammars/multi_algo.pybnf
+autooc/grammars/svm.pybnf
 autooc/operators/__init__.py
 autooc/operators/crossover.py
 autooc/operators/initialisation.py
 autooc/operators/mutation.py
 autooc/operators/replacement.py
 autooc/operators/selection.py
 autooc/operators/subtree_parse.py
```

### Comparing `autooc-0.0.8/setup.py` & `autooc-0.0.9/setup.py`

 * *Files 12% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 import setuptools
 
 this_directory = Path(__file__).parent
 long_description = (this_directory / "README.md").read_text()
 
 setuptools.setup(
     name="autooc",
-    version="0.0.8",
+    version="0.0.9",
     author_email="luis_ferreira223@hotmail.com",
     author="Luís Ferreira",
     description="AutoOC: Automated Machine Learning (AutoML) library for One-Class Learning",
     long_description=long_description,
     long_description_content_type="text/markdown",
     packages=setuptools.find_packages(),
     url="https://github.com/luisferreira97/AutoOC",
@@ -24,15 +24,15 @@
         "Operating System :: OS Independent",
     ],
     py_modules=["autooc"],
     python_requires='>=3.6, <3.9',
     keywords=['automl', 'machine learning', 'one-class learning',
               'one-class classification', 'autoencoder', 'isolation forest', 'one-class svm'],
     include_package_data=True,
-    #package_dir={"": "src/talos"},
+    #package_dir={"": "src/autooc"},
     install_requires=[
         'keras==2.6.0',
         'matplotlib==3.4.1',
         'mlflow==1.15.0',
         'pandas==1.2.4',
         'pydot==1.4.2',
         'scikit-learn==1.0',
```

