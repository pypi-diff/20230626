# Comparing `tmp/ax-platform-0.3.2.tar.gz` & `tmp/ax-platform-0.3.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ax-platform-0.3.2.tar", last modified: Mon May  8 20:45:14 2023, max compression
+gzip compressed data, was "ax-platform-0.3.3.tar", last modified: Mon Jun 26 21:06:04 2023, max compression
```

## Comparing `ax-platform-0.3.2.tar` & `ax-platform-0.3.3.tar`

### file list

```diff
@@ -1,727 +1,738 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 20:45:14.172678 ax-platform-0.3.2/
--rw-r--r--   0 runner    (1001) docker     (123)      407 2023-05-08 20:41:24.000000 ax-platform-0.3.2/.flake8
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 20:45:13.856656 ax-platform-0.3.2/.github/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 20:45:13.864657 ax-platform-0.3.2/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)     2401 2023-05-08 20:41:24.000000 ax-platform-0.3.2/.github/workflows/build-and-test.yml
--rw-r--r--   0 runner    (1001) docker     (123)     3934 2023-05-08 20:41:24.000000 ax-platform-0.3.2/.github/workflows/cron.yml
--rw-r--r--   0 runner    (1001) docker     (123)     2639 2023-05-08 20:41:24.000000 ax-platform-0.3.2/.github/workflows/deploy.yml
--rw-r--r--   0 runner    (1001) docker     (123)      568 2023-05-08 20:41:24.000000 ax-platform-0.3.2/.github/workflows/reusable_tutorials.yml
--rw-r--r--   0 runner    (1001) docker     (123)      321 2023-05-08 20:41:24.000000 ax-platform-0.3.2/.github/workflows/tutorials.yml
--rw-r--r--   0 runner    (1001) docker     (123)     2058 2023-05-08 20:41:24.000000 ax-platform-0.3.2/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)      106 2023-05-08 20:41:24.000000 ax-platform-0.3.2/CHANGELOG.md
--rw-r--r--   0 runner    (1001) docker     (123)     3355 2023-05-08 20:41:24.000000 ax-platform-0.3.2/CODE_OF_CONDUCT.md
--rw-r--r--   0 runner    (1001) docker     (123)     5500 2023-05-08 20:41:24.000000 ax-platform-0.3.2/CONTRIBUTING.md
--rw-r--r--   0 runner    (1001) docker     (123)     1088 2023-05-08 20:41:24.000000 ax-platform-0.3.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     9979 2023-05-08 20:45:14.172678 ax-platform-0.3.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     7877 2023-05-08 20:41:24.000000 ax-platform-0.3.2/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 20:45:13.868657 ax-platform-0.3.2/ax/
--rw-r--r--   0 runner    (1001) docker     (123)     1393 2023-05-08 20:41:24.000000 ax-platform-0.3.2/ax/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      207 2023-05-08 20:41:24.000000 ax-platform-0.3.2/ax/__version__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 20:45:13.868657 ax-platform-0.3.2/ax/benchmark/
--rw-r--r--   0 runner    (1001) docker     (123)      202 2023-05-08 20:41:24.000000 ax-platform-0.3.2/ax/benchmark/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4391 2023-05-08 20:41:24.000000 ax-platform-0.3.2/ax/benchmark/benchmark.py
--rw-r--r--   0 runner    (1001) docker     (123)     1440 2023-05-08 20:41:24.000000 ax-platform-0.3.2/ax/benchmark/benchmark_method.py
--rw-r--r--   0 runner    (1001) docker     (123)     8098 2023-05-08 20:41:24.000000 ax-platform-0.3.2/ax/benchmark/benchmark_problem.py
--rw-r--r--   0 runner    (1001) docker     (123)     7714 2023-05-08 20:41:24.000000 ax-platform-0.3.2/ax/benchmark/benchmark_result.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 20:45:13.872657 ax-platform-0.3.2/ax/benchmark/methods/
--rw-r--r--   0 runner    (1001) docker     (123)      179 2023-05-08 20:41:24.000000 ax-platform-0.3.2/ax/benchmark/methods/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      934 2023-05-08 20:41:24.000000 ax-platform-0.3.2/ax/benchmark/methods/choose_generation_strategy.py
--rw-r--r--   0 runner    (1001) docker     (123)     1594 2023-05-08 20:41:24.000000 ax-platform-0.3.2/ax/benchmark/methods/gpei_and_moo.py
--rw-r--r--   0 runner    (1001) docker     (123)     7190 2023-05-08 20:41:24.000000 ax-platform-0.3.2/ax/benchmark/methods/modular_botorch.py
--rw-r--r--   0 runner    (1001) docker     (123)     1647 2023-05-08 20:41:24.000000 ax-platform-0.3.2/ax/benchmark/methods/saasbo.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 20:45:13.872657 ax-platform-0.3.2/ax/benchmark/problems/
--rw-r--r--   0 runner    (1001) docker     (123)      179 2023-05-08 20:41:24.000000 ax-platform-0.3.2/ax/benchmark/problems/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1287 2023-05-08 20:41:24.000000 ax-platform-0.3.2/ax/benchmark/problems/hd_embedding.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 20:45:13.872657 ax-platform-0.3.2/ax/benchmark/problems/hpo/
--rw-r--r--   0 runner    (1001) docker     (123)      179 2023-05-08 20:41:24.000000 ax-platform-0.3.2/ax/benchmark/problems/hpo/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7815 2023-05-08 20:41:24.000000 ax-platform-0.3.2/ax/benchmark/problems/hpo/pytorch_cnn.py
--rw-r--r--   0 runner    (1001) docker     (123)     3762 2023-05-08 20:41:24.000000 ax-platform-0.3.2/ax/benchmark/problems/hpo/torchvision.py
--rw-r--r--   0 runner    (1001) docker     (123)     8375 2023-05-08 20:41:24.000000 ax-platform-0.3.2/ax/benchmark/problems/registry.py
--rw-r--r--   0 runner    (1001) docker     (123)     7036 2023-05-08 20:41:24.000000 ax-platform-0.3.2/ax/benchmark/problems/surrogate.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 20:45:13.876658 ax-platform-0.3.2/ax/benchmark/problems/synthetic/
--rw-r--r--   0 runner    (1001) docker     (123)      179 2023-05-08 20:41:24.000000 ax-platform-0.3.2/ax/benchmark/problems/synthetic/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 20:45:13.876658 ax-platform-0.3.2/ax/benchmark/problems/synthetic/discretized/
--rw-r--r--   0 runner    (1001) docker     (123)      179 2023-05-08 20:41:24.000000 ax-platform-0.3.2/ax/benchmark/problems/synthetic/discretized/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5634 2023-05-08 20:41:24.000000 ax-platform-0.3.2/ax/benchmark/problems/synthetic/discretized/mixed_integer.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 20:45:13.876658 ax-platform-0.3.2/ax/benchmark/problems/synthetic/hss/
--rw-r--r--   0 runner    (1001) docker     (123)      179 2023-05-08 20:41:24.000000 ax-platform-0.3.2/ax/benchmark/problems/synthetic/hss/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2392 2023-05-08 20:41:24.000000 ax-platform-0.3.2/ax/benchmark/problems/synthetic/hss/jenatton.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 20:45:13.880658 ax-platform-0.3.2/ax/benchmark/tests/
--rw-r--r--   0 runner    (1001) docker     (123)      202 2023-05-08 20:41:24.000000 ax-platform-0.3.2/ax/benchmark/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4639 2023-05-08 20:41:24.000000 ax-platform-0.3.2/ax/benchmark/tests/test_benchmark.py
--rw-r--r--   0 runner    (1001) docker     (123)     1065 2023-05-08 20:41:24.000000 ax-platform-0.3.2/ax/benchmark/tests/test_benchmark_method.py
--rw-r--r--   0 runner    (1001) docker     (123)     3649 2023-05-08 20:41:24.000000 ax-platform-0.3.2/ax/benchmark/tests/test_benchmark_problem.py
--rw-r--r--   0 runner    (1001) docker     (123)     1951 2023-05-08 20:41:24.000000 ax-platform-0.3.2/ax/benchmark/tests/test_methods.py
--rw-r--r--   0 runner    (1001) docker     (123)     4493 2023-05-08 20:41:24.000000 ax-platform-0.3.2/ax/benchmark/tests/test_mixed_integer_problems.py
--rw-r--r--   0 runner    (1001) docker     (123)      869 2023-05-08 20:41:24.000000 ax-platform-0.3.2/ax/benchmark/tests/test_problem_storage.py
--rw-r--r--   0 runner    (1001) docker     (123)      648 2023-05-08 20:41:24.000000 ax-platform-0.3.2/ax/benchmark/tests/test_problems.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 20:45:13.892659 ax-platform-0.3.2/ax/core/
--rw-r--r--   0 runner    (1001) docker     (123)     1883 2023-05-08 20:41:24.000000 ax-platform-0.3.2/ax/core/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4629 2023-05-08 20:41:24.000000 ax-platform-0.3.2/ax/core/arm.py
--rw-r--r--   0 runner    (1001) docker     (123)    32190 2023-05-08 20:41:24.000000 ax-platform-0.3.2/ax/core/base_trial.py
--rw-r--r--   0 runner    (1001) docker     (123)    27143 2023-05-08 20:41:24.000000 ax-platform-0.3.2/ax/core/batch_trial.py
--rw-r--r--   0 runner    (1001) docker     (123)    18301 2023-05-08 20:41:24.000000 ax-platform-0.3.2/ax/core/data.py
--rw-r--r--   0 runner    (1001) docker     (123)    60990 2023-05-08 20:41:24.000000 ax-platform-0.3.2/ax/core/experiment.py
--rw-r--r--   0 runner    (1001) docker     (123)     5088 2023-05-08 20:41:24.000000 ax-platform-0.3.2/ax/core/formatting_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)    15255 2023-05-08 20:41:24.000000 ax-platform-0.3.2/ax/core/generator_run.py
--rw-r--r--   0 runner    (1001) docker     (123)    16558 2023-05-08 20:41:24.000000 ax-platform-0.3.2/ax/core/map_data.py
--rw-r--r--   0 runner    (1001) docker     (123)     1156 2023-05-08 20:41:24.000000 ax-platform-0.3.2/ax/core/map_metric.py
--rw-r--r--   0 runner    (1001) docker     (123)    17067 2023-05-08 20:41:24.000000 ax-platform-0.3.2/ax/core/metric.py
--rw-r--r--   0 runner    (1001) docker     (123)    10616 2023-05-08 20:41:24.000000 ax-platform-0.3.2/ax/core/multi_type_experiment.py
--rw-r--r--   0 runner    (1001) docker     (123)     8264 2023-05-08 20:41:24.000000 ax-platform-0.3.2/ax/core/objective.py
--rw-r--r--   0 runner    (1001) docker     (123)    20542 2023-05-08 20:41:24.000000 ax-platform-0.3.2/ax/core/observation.py
--rw-r--r--   0 runner    (1001) docker     (123)    19264 2023-05-08 20:41:24.000000 ax-platform-0.3.2/ax/core/optimization_config.py
--rw-r--r--   0 runner    (1001) docker     (123)    10024 2023-05-08 20:41:24.000000 ax-platform-0.3.2/ax/core/outcome_constraint.py
--rw-r--r--   0 runner    (1001) docker     (123)    25465 2023-05-08 20:41:24.000000 ax-platform-0.3.2/ax/core/parameter.py
--rw-r--r--   0 runner    (1001) docker     (123)    10253 2023-05-08 20:41:24.000000 ax-platform-0.3.2/ax/core/parameter_constraint.py
--rw-r--r--   0 runner    (1001) docker     (123)     5723 2023-05-08 20:41:24.000000 ax-platform-0.3.2/ax/core/parameter_distribution.py
--rw-r--r--   0 runner    (1001) docker     (123)     2270 2023-05-08 20:41:24.000000 ax-platform-0.3.2/ax/core/risk_measures.py
--rw-r--r--   0 runner    (1001) docker     (123)     5363 2023-05-08 20:41:24.000000 ax-platform-0.3.2/ax/core/runner.py
--rw-r--r--   0 runner    (1001) docker     (123)    45577 2023-05-08 20:41:24.000000 ax-platform-0.3.2/ax/core/search_space.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 20:45:13.900659 ax-platform-0.3.2/ax/core/tests/
--rw-r--r--   0 runner    (1001) docker     (123)      202 2023-05-08 20:41:24.000000 ax-platform-0.3.2/ax/core/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2434 2023-05-08 20:41:24.000000 ax-platform-0.3.2/ax/core/tests/test_arm.py
--rw-r--r--   0 runner    (1001) docker     (123)    30540 2023-05-08 20:41:24.000000 ax-platform-0.3.2/ax/core/tests/test_batch_trial.py
--rw-r--r--   0 runner    (1001) docker     (123)    12917 2023-05-08 20:41:24.000000 ax-platform-0.3.2/ax/core/tests/test_data.py
--rw-r--r--   0 runner    (1001) docker     (123)    48974 2023-05-08 20:41:24.000000 ax-platform-0.3.2/ax/core/tests/test_experiment.py
--rw-r--r--   0 runner    (1001) docker     (123)     3942 2023-05-08 20:41:24.000000 ax-platform-0.3.2/ax/core/tests/test_formatting_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     7352 2023-05-08 20:41:24.000000 ax-platform-0.3.2/ax/core/tests/test_generator_run.py
--rw-r--r--   0 runner    (1001) docker     (123)    12229 2023-05-08 20:41:24.000000 ax-platform-0.3.2/ax/core/tests/test_map_data.py
--rw-r--r--   0 runner    (1001) docker     (123)     1875 2023-05-08 20:41:24.000000 ax-platform-0.3.2/ax/core/tests/test_map_metric.py
--rw-r--r--   0 runner    (1001) docker     (123)     3256 2023-05-08 20:41:24.000000 ax-platform-0.3.2/ax/core/tests/test_metric.py
--rw-r--r--   0 runner    (1001) docker     (123)     5328 2023-05-08 20:41:24.000000 ax-platform-0.3.2/ax/core/tests/test_multi_type_experiment.py
--rw-r--r--   0 runner    (1001) docker     (123)     5451 2023-05-08 20:41:24.000000 ax-platform-0.3.2/ax/core/tests/test_objective.py
--rw-r--r--   0 runner    (1001) docker     (123)    31569 2023-05-08 20:41:24.000000 ax-platform-0.3.2/ax/core/tests/test_observation.py
--rw-r--r--   0 runner    (1001) docker     (123)    22183 2023-05-08 20:41:24.000000 ax-platform-0.3.2/ax/core/tests/test_optimization_config.py
--rw-r--r--   0 runner    (1001) docker     (123)     8604 2023-05-08 20:41:24.000000 ax-platform-0.3.2/ax/core/tests/test_outcome_constraint.py
--rw-r--r--   0 runner    (1001) docker     (123)    17549 2023-05-08 20:41:24.000000 ax-platform-0.3.2/ax/core/tests/test_parameter.py
--rw-r--r--   0 runner    (1001) docker     (123)     8345 2023-05-08 20:41:24.000000 ax-platform-0.3.2/ax/core/tests/test_parameter_constraint.py
--rw-r--r--   0 runner    (1001) docker     (123)     2888 2023-05-08 20:41:24.000000 ax-platform-0.3.2/ax/core/tests/test_parameter_distribution.py
--rw-r--r--   0 runner    (1001) docker     (123)      885 2023-05-08 20:41:24.000000 ax-platform-0.3.2/ax/core/tests/test_risk_measures.py
--rw-r--r--   0 runner    (1001) docker     (123)     1900 2023-05-08 20:41:24.000000 ax-platform-0.3.2/ax/core/tests/test_runner.py
--rw-r--r--   0 runner    (1001) docker     (123)    44614 2023-05-08 20:41:24.000000 ax-platform-0.3.2/ax/core/tests/test_search_space.py
--rw-r--r--   0 runner    (1001) docker     (123)    10538 2023-05-08 20:41:24.000000 ax-platform-0.3.2/ax/core/tests/test_trial.py
--rw-r--r--   0 runner    (1001) docker     (123)     1506 2023-05-08 20:41:24.000000 ax-platform-0.3.2/ax/core/tests/test_types.py
--rw-r--r--   0 runner    (1001) docker     (123)     6914 2023-05-08 20:41:24.000000 ax-platform-0.3.2/ax/core/tests/test_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)    12059 2023-05-08 20:41:24.000000 ax-platform-0.3.2/ax/core/trial.py
--rw-r--r--   0 runner    (1001) docker     (123)     3666 2023-05-08 20:41:24.000000 ax-platform-0.3.2/ax/core/types.py
--rw-r--r--   0 runner    (1001) docker     (123)     6975 2023-05-08 20:41:24.000000 ax-platform-0.3.2/ax/core/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 20:45:13.904660 ax-platform-0.3.2/ax/early_stopping/
--rw-r--r--   0 runner    (1001) docker     (123)      271 2023-05-08 20:41:24.000000 ax-platform-0.3.2/ax/early_stopping/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 20:45:13.904660 ax-platform-0.3.2/ax/early_stopping/strategies/
--rw-r--r--   0 runner    (1001) docker     (123)      961 2023-05-08 20:41:24.000000 ax-platform-0.3.2/ax/early_stopping/strategies/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    24312 2023-05-08 20:41:24.000000 ax-platform-0.3.2/ax/early_stopping/strategies/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     2552 2023-05-08 20:41:24.000000 ax-platform-0.3.2/ax/early_stopping/strategies/logical.py
--rw-r--r--   0 runner    (1001) docker     (123)    10738 2023-05-08 20:41:24.000000 ax-platform-0.3.2/ax/early_stopping/strategies/percentile.py
--rw-r--r--   0 runner    (1001) docker     (123)     8594 2023-05-08 20:41:24.000000 ax-platform-0.3.2/ax/early_stopping/strategies/threshold.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 20:45:13.904660 ax-platform-0.3.2/ax/early_stopping/tests/
--rw-r--r--   0 runner    (1001) docker     (123)      202 2023-05-08 20:41:24.000000 ax-platform-0.3.2/ax/early_stopping/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    31888 2023-05-08 20:41:24.000000 ax-platform-0.3.2/ax/early_stopping/tests/test_strategies.py
--rw-r--r--   0 runner    (1001) docker     (123)     4977 2023-05-08 20:41:24.000000 ax-platform-0.3.2/ax/early_stopping/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 20:45:13.908660 ax-platform-0.3.2/ax/exceptions/
--rw-r--r--   0 runner    (1001) docker     (123)      202 2023-05-08 20:41:24.000000 ax-platform-0.3.2/ax/exceptions/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      891 2023-05-08 20:41:24.000000 ax-platform-0.3.2/ax/exceptions/constants.py
--rw-r--r--   0 runner    (1001) docker     (123)     4940 2023-05-08 20:41:24.000000 ax-platform-0.3.2/ax/exceptions/core.py
--rw-r--r--   0 runner    (1001) docker     (123)     1650 2023-05-08 20:41:24.000000 ax-platform-0.3.2/ax/exceptions/data_provider.py
--rw-r--r--   0 runner    (1001) docker     (123)     1569 2023-05-08 20:41:24.000000 ax-platform-0.3.2/ax/exceptions/generation_strategy.py
--rw-r--r--   0 runner    (1001) docker     (123)      480 2023-05-08 20:41:24.000000 ax-platform-0.3.2/ax/exceptions/model.py
--rw-r--r--   0 runner    (1001) docker     (123)     1082 2023-05-08 20:41:24.000000 ax-platform-0.3.2/ax/exceptions/storage.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 20:45:13.908660 ax-platform-0.3.2/ax/global_stopping/
--rw-r--r--   0 runner    (1001) docker     (123)      272 2023-05-08 20:41:24.000000 ax-platform-0.3.2/ax/global_stopping/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 20:45:13.908660 ax-platform-0.3.2/ax/global_stopping/strategies/
--rw-r--r--   0 runner    (1001) docker     (123)      456 2023-05-08 20:41:24.000000 ax-platform-0.3.2/ax/global_stopping/strategies/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2091 2023-05-08 20:41:24.000000 ax-platform-0.3.2/ax/global_stopping/strategies/base.py
--rw-r--r--   0 runner    (1001) docker     (123)    12870 2023-05-08 20:41:24.000000 ax-platform-0.3.2/ax/global_stopping/strategies/improvement.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 20:45:13.912660 ax-platform-0.3.2/ax/global_stopping/tests/
--rw-r--r--   0 runner    (1001) docker     (123)      202 2023-05-08 20:41:24.000000 ax-platform-0.3.2/ax/global_stopping/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    13571 2023-05-08 20:41:24.000000 ax-platform-0.3.2/ax/global_stopping/tests/tests_strategies.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 20:45:13.916660 ax-platform-0.3.2/ax/metrics/
--rw-r--r--   0 runner    (1001) docker     (123)      511 2023-05-08 20:41:24.000000 ax-platform-0.3.2/ax/metrics/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2190 2023-05-08 20:41:24.000000 ax-platform-0.3.2/ax/metrics/botorch_test_problem.py
--rw-r--r--   0 runner    (1001) docker     (123)      840 2023-05-08 20:41:24.000000 ax-platform-0.3.2/ax/metrics/branin.py
--rw-r--r--   0 runner    (1001) docker     (123)     5649 2023-05-08 20:41:24.000000 ax-platform-0.3.2/ax/metrics/branin_map.py
--rw-r--r--   0 runner    (1001) docker     (123)     4692 2023-05-08 20:41:24.000000 ax-platform-0.3.2/ax/metrics/chemistry.py
--rw-r--r--   0 runner    (1001) docker     (123)    31150 2023-05-08 20:41:24.000000 ax-platform-0.3.2/ax/metrics/chemistry_data.zip
--rw-r--r--   0 runner    (1001) docker     (123)    20145 2023-05-08 20:41:24.000000 ax-platform-0.3.2/ax/metrics/curve.py
--rw-r--r--   0 runner    (1001) docker     (123)     3897 2023-05-08 20:41:24.000000 ax-platform-0.3.2/ax/metrics/dict_lookup.py
--rw-r--r--   0 runner    (1001) docker     (123)     4602 2023-05-08 20:41:24.000000 ax-platform-0.3.2/ax/metrics/factorial.py
--rw-r--r--   0 runner    (1001) docker     (123)      694 2023-05-08 20:41:24.000000 ax-platform-0.3.2/ax/metrics/hartmann6.py
--rw-r--r--   0 runner    (1001) docker     (123)     2176 2023-05-08 20:41:24.000000 ax-platform-0.3.2/ax/metrics/jenatton.py
--rw-r--r--   0 runner    (1001) docker     (123)      401 2023-05-08 20:41:24.000000 ax-platform-0.3.2/ax/metrics/l2norm.py
--rw-r--r--   0 runner    (1001) docker     (123)     5196 2023-05-08 20:41:24.000000 ax-platform-0.3.2/ax/metrics/noisy_function.py
--rw-r--r--   0 runner    (1001) docker     (123)     3968 2023-05-08 20:41:24.000000 ax-platform-0.3.2/ax/metrics/noisy_function_map.py
--rw-r--r--   0 runner    (1001) docker     (123)     6708 2023-05-08 20:41:24.000000 ax-platform-0.3.2/ax/metrics/sklearn.py
--rw-r--r--   0 runner    (1001) docker     (123)     4835 2023-05-08 20:41:24.000000 ax-platform-0.3.2/ax/metrics/tensorboard.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 20:45:13.920661 ax-platform-0.3.2/ax/metrics/tests/
--rw-r--r--   0 runner    (1001) docker     (123)      202 2023-05-08 20:41:24.000000 ax-platform-0.3.2/ax/metrics/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3652 2023-05-08 20:41:24.000000 ax-platform-0.3.2/ax/metrics/tests/test_chemistry.py
--rw-r--r--   0 runner    (1001) docker     (123)      640 2023-05-08 20:41:24.000000 ax-platform-0.3.2/ax/metrics/tests/test_curve.py
--rw-r--r--   0 runner    (1001) docker     (123)     2620 2023-05-08 20:41:24.000000 ax-platform-0.3.2/ax/metrics/tests/test_dict_lookup.py
--rw-r--r--   0 runner    (1001) docker     (123)     2617 2023-05-08 20:41:24.000000 ax-platform-0.3.2/ax/metrics/tests/test_noisy_function.py
--rw-r--r--   0 runner    (1001) docker     (123)     4367 2023-05-08 20:41:24.000000 ax-platform-0.3.2/ax/metrics/tests/test_sklearn.py
--rw-r--r--   0 runner    (1001) docker     (123)     7279 2023-05-08 20:41:24.000000 ax-platform-0.3.2/ax/metrics/tests/test_tensorboard.py
--rw-r--r--   0 runner    (1001) docker     (123)     2679 2023-05-08 20:41:24.000000 ax-platform-0.3.2/ax/metrics/torchx.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 20:45:13.932662 ax-platform-0.3.2/ax/modelbridge/
--rw-r--r--   0 runner    (1001) docker     (123)      772 2023-05-08 20:41:24.000000 ax-platform-0.3.2/ax/modelbridge/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    44868 2023-05-08 20:41:24.000000 ax-platform-0.3.2/ax/modelbridge/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     1603 2023-05-08 20:41:24.000000 ax-platform-0.3.2/ax/modelbridge/completion_criterion.py
--rw-r--r--   0 runner    (1001) docker     (123)    16680 2023-05-08 20:41:24.000000 ax-platform-0.3.2/ax/modelbridge/cross_validation.py
--rw-r--r--   0 runner    (1001) docker     (123)     9872 2023-05-08 20:41:24.000000 ax-platform-0.3.2/ax/modelbridge/discrete.py
--rw-r--r--   0 runner    (1001) docker     (123)    28288 2023-05-08 20:41:24.000000 ax-platform-0.3.2/ax/modelbridge/dispatch_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)    24504 2023-05-08 20:41:24.000000 ax-platform-0.3.2/ax/modelbridge/factory.py
--rw-r--r--   0 runner    (1001) docker     (123)    19309 2023-05-08 20:41:24.000000 ax-platform-0.3.2/ax/modelbridge/generation_node.py
--rw-r--r--   0 runner    (1001) docker     (123)    40066 2023-05-08 20:41:24.000000 ax-platform-0.3.2/ax/modelbridge/generation_strategy.py
--rw-r--r--   0 runner    (1001) docker     (123)    17579 2023-05-08 20:41:24.000000 ax-platform-0.3.2/ax/modelbridge/map_torch.py
--rw-r--r--   0 runner    (1001) docker     (123)    13878 2023-05-08 20:41:24.000000 ax-platform-0.3.2/ax/modelbridge/model_spec.py
--rw-r--r--   0 runner    (1001) docker     (123)    58315 2023-05-08 20:41:24.000000 ax-platform-0.3.2/ax/modelbridge/modelbridge_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     4409 2023-05-08 20:41:24.000000 ax-platform-0.3.2/ax/modelbridge/pairwise.py
--rw-r--r--   0 runner    (1001) docker     (123)     3421 2023-05-08 20:41:24.000000 ax-platform-0.3.2/ax/modelbridge/prediction_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     4103 2023-05-08 20:41:24.000000 ax-platform-0.3.2/ax/modelbridge/random.py
--rw-r--r--   0 runner    (1001) docker     (123)    21913 2023-05-08 20:41:24.000000 ax-platform-0.3.2/ax/modelbridge/registry.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 20:45:13.932662 ax-platform-0.3.2/ax/modelbridge/strategies/
--rw-r--r--   0 runner    (1001) docker     (123)      202 2023-05-08 20:41:24.000000 ax-platform-0.3.2/ax/modelbridge/strategies/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4582 2023-05-08 20:41:24.000000 ax-platform-0.3.2/ax/modelbridge/strategies/alebo.py
--rw-r--r--   0 runner    (1001) docker     (123)    10030 2023-05-08 20:41:24.000000 ax-platform-0.3.2/ax/modelbridge/strategies/rembo.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 20:45:13.960663 ax-platform-0.3.2/ax/modelbridge/tests/
--rw-r--r--   0 runner    (1001) docker     (123)      202 2023-05-08 20:41:24.000000 ax-platform-0.3.2/ax/modelbridge/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2807 2023-05-08 20:41:24.000000 ax-platform-0.3.2/ax/modelbridge/tests/test_alebo_strategy.py
--rw-r--r--   0 runner    (1001) docker     (123)    32245 2023-05-08 20:41:24.000000 ax-platform-0.3.2/ax/modelbridge/tests/test_base_modelbridge.py
--rw-r--r--   0 runner    (1001) docker     (123)     2236 2023-05-08 20:41:24.000000 ax-platform-0.3.2/ax/modelbridge/tests/test_base_transform.py
--rw-r--r--   0 runner    (1001) docker     (123)     2340 2023-05-08 20:41:24.000000 ax-platform-0.3.2/ax/modelbridge/tests/test_cap_parameter_transform.py
--rw-r--r--   0 runner    (1001) docker     (123)     8209 2023-05-08 20:41:24.000000 ax-platform-0.3.2/ax/modelbridge/tests/test_cast_transform.py
--rw-r--r--   0 runner    (1001) docker     (123)      593 2023-05-08 20:41:24.000000 ax-platform-0.3.2/ax/modelbridge/tests/test_centered_unit_x_transform.py
--rw-r--r--   0 runner    (1001) docker     (123)    10982 2023-05-08 20:41:24.000000 ax-platform-0.3.2/ax/modelbridge/tests/test_choice_encode_transform.py
--rw-r--r--   0 runner    (1001) docker     (123)     4751 2023-05-08 20:41:24.000000 ax-platform-0.3.2/ax/modelbridge/tests/test_completion_criterion.py
--rw-r--r--   0 runner    (1001) docker     (123)     4059 2023-05-08 20:41:24.000000 ax-platform-0.3.2/ax/modelbridge/tests/test_convert_metric_names.py
--rw-r--r--   0 runner    (1001) docker     (123)    14248 2023-05-08 20:41:24.000000 ax-platform-0.3.2/ax/modelbridge/tests/test_cross_validation.py
--rw-r--r--   0 runner    (1001) docker     (123)    11305 2023-05-08 20:41:24.000000 ax-platform-0.3.2/ax/modelbridge/tests/test_derelativize_transform.py
--rw-r--r--   0 runner    (1001) docker     (123)    11824 2023-05-08 20:41:24.000000 ax-platform-0.3.2/ax/modelbridge/tests/test_discrete_modelbridge.py
--rw-r--r--   0 runner    (1001) docker     (123)    33932 2023-05-08 20:41:24.000000 ax-platform-0.3.2/ax/modelbridge/tests/test_dispatch_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)    22595 2023-05-08 20:41:24.000000 ax-platform-0.3.2/ax/modelbridge/tests/test_factory.py
--rw-r--r--   0 runner    (1001) docker     (123)    10464 2023-05-08 20:41:24.000000 ax-platform-0.3.2/ax/modelbridge/tests/test_generation_node.py
--rw-r--r--   0 runner    (1001) docker     (123)    36153 2023-05-08 20:41:24.000000 ax-platform-0.3.2/ax/modelbridge/tests/test_generation_strategy.py
--rw-r--r--   0 runner    (1001) docker     (123)     7123 2023-05-08 20:41:24.000000 ax-platform-0.3.2/ax/modelbridge/tests/test_int_range_to_choice_transform.py
--rw-r--r--   0 runner    (1001) docker     (123)    13466 2023-05-08 20:41:24.000000 ax-platform-0.3.2/ax/modelbridge/tests/test_int_to_float_transform.py
--rw-r--r--   0 runner    (1001) docker     (123)     2600 2023-05-08 20:41:24.000000 ax-platform-0.3.2/ax/modelbridge/tests/test_inverse_gaussian_cdf_y.py
--rw-r--r--   0 runner    (1001) docker     (123)     4386 2023-05-08 20:41:24.000000 ax-platform-0.3.2/ax/modelbridge/tests/test_ivw_transform.py
--rw-r--r--   0 runner    (1001) docker     (123)     4010 2023-05-08 20:41:24.000000 ax-platform-0.3.2/ax/modelbridge/tests/test_log_transform.py
--rw-r--r--   0 runner    (1001) docker     (123)    10890 2023-05-08 20:41:24.000000 ax-platform-0.3.2/ax/modelbridge/tests/test_log_y_transform.py
--rw-r--r--   0 runner    (1001) docker     (123)     5587 2023-05-08 20:41:24.000000 ax-platform-0.3.2/ax/modelbridge/tests/test_logit_transform.py
--rw-r--r--   0 runner    (1001) docker     (123)     5704 2023-05-08 20:41:24.000000 ax-platform-0.3.2/ax/modelbridge/tests/test_map_torch_modelbridge.py
--rw-r--r--   0 runner    (1001) docker     (123)     4511 2023-05-08 20:41:24.000000 ax-platform-0.3.2/ax/modelbridge/tests/test_map_unit_x_transform.py
--rw-r--r--   0 runner    (1001) docker     (123)     6338 2023-05-08 20:41:24.000000 ax-platform-0.3.2/ax/modelbridge/tests/test_merge_repeated_measurements_transform.py
--rw-r--r--   0 runner    (1001) docker     (123)     5101 2023-05-08 20:41:24.000000 ax-platform-0.3.2/ax/modelbridge/tests/test_metrics_as_task_transform.py
--rw-r--r--   0 runner    (1001) docker     (123)     6723 2023-05-08 20:41:24.000000 ax-platform-0.3.2/ax/modelbridge/tests/test_model_spec.py
--rw-r--r--   0 runner    (1001) docker     (123)    10369 2023-05-08 20:41:24.000000 ax-platform-0.3.2/ax/modelbridge/tests/test_modelbridge_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     7739 2023-05-08 20:41:24.000000 ax-platform-0.3.2/ax/modelbridge/tests/test_one_hot_transform.py
--rw-r--r--   0 runner    (1001) docker     (123)     4896 2023-05-08 20:41:24.000000 ax-platform-0.3.2/ax/modelbridge/tests/test_pairwise_modelbridge.py
--rw-r--r--   0 runner    (1001) docker     (123)     4963 2023-05-08 20:41:24.000000 ax-platform-0.3.2/ax/modelbridge/tests/test_percentile_y_transform.py
--rw-r--r--   0 runner    (1001) docker     (123)    15128 2023-05-08 20:41:24.000000 ax-platform-0.3.2/ax/modelbridge/tests/test_power_transform_y.py
--rw-r--r--   0 runner    (1001) docker     (123)     5127 2023-05-08 20:41:24.000000 ax-platform-0.3.2/ax/modelbridge/tests/test_prediction_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     6752 2023-05-08 20:41:24.000000 ax-platform-0.3.2/ax/modelbridge/tests/test_random_modelbridge.py
--rw-r--r--   0 runner    (1001) docker     (123)    20119 2023-05-08 20:41:24.000000 ax-platform-0.3.2/ax/modelbridge/tests/test_registry.py
--rw-r--r--   0 runner    (1001) docker     (123)    14157 2023-05-08 20:41:24.000000 ax-platform-0.3.2/ax/modelbridge/tests/test_relativize_transform.py
--rw-r--r--   0 runner    (1001) docker     (123)     5022 2023-05-08 20:41:24.000000 ax-platform-0.3.2/ax/modelbridge/tests/test_rembo_strategy.py
--rw-r--r--   0 runner    (1001) docker     (123)     4303 2023-05-08 20:41:24.000000 ax-platform-0.3.2/ax/modelbridge/tests/test_remove_fixed_transform.py
--rw-r--r--   0 runner    (1001) docker     (123)     4592 2023-05-08 20:41:24.000000 ax-platform-0.3.2/ax/modelbridge/tests/test_robust.py
--rw-r--r--   0 runner    (1001) docker     (123)      952 2023-05-08 20:41:24.000000 ax-platform-0.3.2/ax/modelbridge/tests/test_rounding.py
--rw-r--r--   0 runner    (1001) docker     (123)     5358 2023-05-08 20:41:24.000000 ax-platform-0.3.2/ax/modelbridge/tests/test_search_space_to_choice_transform.py
--rw-r--r--   0 runner    (1001) docker     (123)     2193 2023-05-08 20:41:24.000000 ax-platform-0.3.2/ax/modelbridge/tests/test_search_space_to_float_transform.py
--rw-r--r--   0 runner    (1001) docker     (123)     6044 2023-05-08 20:41:24.000000 ax-platform-0.3.2/ax/modelbridge/tests/test_standardize_y_transform.py
--rw-r--r--   0 runner    (1001) docker     (123)     8992 2023-05-08 20:41:24.000000 ax-platform-0.3.2/ax/modelbridge/tests/test_stratified_standardize_y.py
--rw-r--r--   0 runner    (1001) docker     (123)     5681 2023-05-08 20:41:24.000000 ax-platform-0.3.2/ax/modelbridge/tests/test_task_encode_transform.py
--rw-r--r--   0 runner    (1001) docker     (123)    29980 2023-05-08 20:41:24.000000 ax-platform-0.3.2/ax/modelbridge/tests/test_torch_modelbridge.py
--rw-r--r--   0 runner    (1001) docker     (123)    33129 2023-05-08 20:41:24.000000 ax-platform-0.3.2/ax/modelbridge/tests/test_torch_modelbridge_moo.py
--rw-r--r--   0 runner    (1001) docker     (123)     3194 2023-05-08 20:41:24.000000 ax-platform-0.3.2/ax/modelbridge/tests/test_transform_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     6410 2023-05-08 20:41:24.000000 ax-platform-0.3.2/ax/modelbridge/tests/test_trial_as_task_transform.py
--rw-r--r--   0 runner    (1001) docker     (123)    10996 2023-05-08 20:41:24.000000 ax-platform-0.3.2/ax/modelbridge/tests/test_unit_x_transform.py
--rw-r--r--   0 runner    (1001) docker     (123)    26757 2023-05-08 20:41:24.000000 ax-platform-0.3.2/ax/modelbridge/tests/test_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)    29969 2023-05-08 20:41:24.000000 ax-platform-0.3.2/ax/modelbridge/tests/test_winsorize_transform.py
--rw-r--r--   0 runner    (1001) docker     (123)     8282 2023-05-08 20:41:24.000000 ax-platform-0.3.2/ax/modelbridge/tests/test_winsorize_transform_legacy.py
--rw-r--r--   0 runner    (1001) docker     (123)    39444 2023-05-08 20:41:24.000000 ax-platform-0.3.2/ax/modelbridge/torch.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 20:45:13.972664 ax-platform-0.3.2/ax/modelbridge/transforms/
--rw-r--r--   0 runner    (1001) docker     (123)      202 2023-05-08 20:41:24.000000 ax-platform-0.3.2/ax/modelbridge/transforms/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     9830 2023-05-08 20:41:24.000000 ax-platform-0.3.2/ax/modelbridge/transforms/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     2125 2023-05-08 20:41:24.000000 ax-platform-0.3.2/ax/modelbridge/transforms/cap_parameter.py
--rw-r--r--   0 runner    (1001) docker     (123)     5137 2023-05-08 20:41:24.000000 ax-platform-0.3.2/ax/modelbridge/transforms/cast.py
--rw-r--r--   0 runner    (1001) docker     (123)      463 2023-05-08 20:41:24.000000 ax-platform-0.3.2/ax/modelbridge/transforms/centered_unit_x.py
--rw-r--r--   0 runner    (1001) docker     (123)     9272 2023-05-08 20:41:24.000000 ax-platform-0.3.2/ax/modelbridge/transforms/choice_encode.py
--rw-r--r--   0 runner    (1001) docker     (123)     6049 2023-05-08 20:41:24.000000 ax-platform-0.3.2/ax/modelbridge/transforms/convert_metric_names.py
--rw-r--r--   0 runner    (1001) docker     (123)     4952 2023-05-08 20:41:24.000000 ax-platform-0.3.2/ax/modelbridge/transforms/derelativize.py
--rw-r--r--   0 runner    (1001) docker     (123)     3310 2023-05-08 20:41:24.000000 ax-platform-0.3.2/ax/modelbridge/transforms/int_range_to_choice.py
--rw-r--r--   0 runner    (1001) docker     (123)     7500 2023-05-08 20:41:24.000000 ax-platform-0.3.2/ax/modelbridge/transforms/int_to_float.py
--rw-r--r--   0 runner    (1001) docker     (123)     2535 2023-05-08 20:41:24.000000 ax-platform-0.3.2/ax/modelbridge/transforms/inverse_gaussian_cdf_y.py
--rw-r--r--   0 runner    (1001) docker     (123)     5265 2023-05-08 20:41:24.000000 ax-platform-0.3.2/ax/modelbridge/transforms/ivw.py
--rw-r--r--   0 runner    (1001) docker     (123)     3245 2023-05-08 20:41:24.000000 ax-platform-0.3.2/ax/modelbridge/transforms/log.py
--rw-r--r--   0 runner    (1001) docker     (123)     7978 2023-05-08 20:41:24.000000 ax-platform-0.3.2/ax/modelbridge/transforms/log_y.py
--rw-r--r--   0 runner    (1001) docker     (123)     2974 2023-05-08 20:41:24.000000 ax-platform-0.3.2/ax/modelbridge/transforms/logit.py
--rw-r--r--   0 runner    (1001) docker     (123)     3477 2023-05-08 20:41:24.000000 ax-platform-0.3.2/ax/modelbridge/transforms/map_unit_x.py
--rw-r--r--   0 runner    (1001) docker     (123)     5362 2023-05-08 20:41:24.000000 ax-platform-0.3.2/ax/modelbridge/transforms/merge_repeated_measurements.py
--rw-r--r--   0 runner    (1001) docker     (123)     5841 2023-05-08 20:41:24.000000 ax-platform-0.3.2/ax/modelbridge/transforms/metrics_as_task.py
--rw-r--r--   0 runner    (1001) docker     (123)     7819 2023-05-08 20:41:24.000000 ax-platform-0.3.2/ax/modelbridge/transforms/one_hot.py
--rw-r--r--   0 runner    (1001) docker     (123)     4149 2023-05-08 20:41:24.000000 ax-platform-0.3.2/ax/modelbridge/transforms/percentile_y.py
--rw-r--r--   0 runner    (1001) docker     (123)     9196 2023-05-08 20:41:24.000000 ax-platform-0.3.2/ax/modelbridge/transforms/power_transform_y.py
--rw-r--r--   0 runner    (1001) docker     (123)     8163 2023-05-08 20:41:24.000000 ax-platform-0.3.2/ax/modelbridge/transforms/relativize.py
--rw-r--r--   0 runner    (1001) docker     (123)     3637 2023-05-08 20:41:24.000000 ax-platform-0.3.2/ax/modelbridge/transforms/remove_fixed.py
--rw-r--r--   0 runner    (1001) docker     (123)     2335 2023-05-08 20:41:24.000000 ax-platform-0.3.2/ax/modelbridge/transforms/rounding.py
--rw-r--r--   0 runner    (1001) docker     (123)     3923 2023-05-08 20:41:24.000000 ax-platform-0.3.2/ax/modelbridge/transforms/search_space_to_choice.py
--rw-r--r--   0 runner    (1001) docker     (123)     1588 2023-05-08 20:41:24.000000 ax-platform-0.3.2/ax/modelbridge/transforms/search_space_to_float.py
--rw-r--r--   0 runner    (1001) docker     (123)     7298 2023-05-08 20:41:24.000000 ax-platform-0.3.2/ax/modelbridge/transforms/standardize_y.py
--rw-r--r--   0 runner    (1001) docker     (123)     7571 2023-05-08 20:41:24.000000 ax-platform-0.3.2/ax/modelbridge/transforms/stratified_standardize_y.py
--rw-r--r--   0 runner    (1001) docker     (123)     3965 2023-05-08 20:41:24.000000 ax-platform-0.3.2/ax/modelbridge/transforms/task_encode.py
--rw-r--r--   0 runner    (1001) docker     (123)     6336 2023-05-08 20:41:24.000000 ax-platform-0.3.2/ax/modelbridge/transforms/trial_as_task.py
--rw-r--r--   0 runner    (1001) docker     (123)    10934 2023-05-08 20:41:24.000000 ax-platform-0.3.2/ax/modelbridge/transforms/unit_x.py
--rw-r--r--   0 runner    (1001) docker     (123)     6008 2023-05-08 20:41:24.000000 ax-platform-0.3.2/ax/modelbridge/transforms/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)    20930 2023-05-08 20:41:24.000000 ax-platform-0.3.2/ax/modelbridge/transforms/winsorize.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 20:45:13.976665 ax-platform-0.3.2/ax/models/
--rw-r--r--   0 runner    (1001) docker     (123)      202 2023-05-08 20:41:24.000000 ax-platform-0.3.2/ax/models/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2601 2023-05-08 20:41:24.000000 ax-platform-0.3.2/ax/models/base.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 20:45:13.976665 ax-platform-0.3.2/ax/models/discrete/
--rw-r--r--   0 runner    (1001) docker     (123)      202 2023-05-08 20:41:24.000000 ax-platform-0.3.2/ax/models/discrete/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1753 2023-05-08 20:41:24.000000 ax-platform-0.3.2/ax/models/discrete/eb_thompson.py
--rw-r--r--   0 runner    (1001) docker     (123)     2980 2023-05-08 20:41:24.000000 ax-platform-0.3.2/ax/models/discrete/full_factorial.py
--rw-r--r--   0 runner    (1001) docker     (123)    11208 2023-05-08 20:41:24.000000 ax-platform-0.3.2/ax/models/discrete/thompson.py
--rw-r--r--   0 runner    (1001) docker     (123)     5699 2023-05-08 20:41:24.000000 ax-platform-0.3.2/ax/models/discrete_base.py
--rw-r--r--   0 runner    (1001) docker     (123)    22672 2023-05-08 20:41:24.000000 ax-platform-0.3.2/ax/models/model_utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 20:45:13.980665 ax-platform-0.3.2/ax/models/random/
--rw-r--r--   0 runner    (1001) docker     (123)      202 2023-05-08 20:41:24.000000 ax-platform-0.3.2/ax/models/random/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3598 2023-05-08 20:41:24.000000 ax-platform-0.3.2/ax/models/random/alebo_initializer.py
--rw-r--r--   0 runner    (1001) docker     (123)    11659 2023-05-08 20:41:24.000000 ax-platform-0.3.2/ax/models/random/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     2567 2023-05-08 20:41:24.000000 ax-platform-0.3.2/ax/models/random/rembo_initializer.py
--rw-r--r--   0 runner    (1001) docker     (123)     6195 2023-05-08 20:41:24.000000 ax-platform-0.3.2/ax/models/random/sobol.py
--rw-r--r--   0 runner    (1001) docker     (123)     1551 2023-05-08 20:41:24.000000 ax-platform-0.3.2/ax/models/random/uniform.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 20:45:13.992666 ax-platform-0.3.2/ax/models/tests/
--rw-r--r--   0 runner    (1001) docker     (123)      202 2023-05-08 20:41:24.000000 ax-platform-0.3.2/ax/models/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    14633 2023-05-08 20:41:24.000000 ax-platform-0.3.2/ax/models/tests/test_alebo.py
--rw-r--r--   0 runner    (1001) docker     (123)     1057 2023-05-08 20:41:24.000000 ax-platform-0.3.2/ax/models/tests/test_alebo_initializer.py
--rw-r--r--   0 runner    (1001) docker     (123)      773 2023-05-08 20:41:24.000000 ax-platform-0.3.2/ax/models/tests/test_base.py
--rw-r--r--   0 runner    (1001) docker     (123)    17805 2023-05-08 20:41:24.000000 ax-platform-0.3.2/ax/models/tests/test_botorch_defaults.py
--rw-r--r--   0 runner    (1001) docker     (123)    17944 2023-05-08 20:41:24.000000 ax-platform-0.3.2/ax/models/tests/test_botorch_kg.py
--rw-r--r--   0 runner    (1001) docker     (123)    13434 2023-05-08 20:41:24.000000 ax-platform-0.3.2/ax/models/tests/test_botorch_mes.py
--rw-r--r--   0 runner    (1001) docker     (123)    30863 2023-05-08 20:41:24.000000 ax-platform-0.3.2/ax/models/tests/test_botorch_model.py
--rw-r--r--   0 runner    (1001) docker     (123)    20926 2023-05-08 20:41:24.000000 ax-platform-0.3.2/ax/models/tests/test_botorch_moo_defaults.py
--rw-r--r--   0 runner    (1001) docker     (123)    33596 2023-05-08 20:41:24.000000 ax-platform-0.3.2/ax/models/tests/test_botorch_moo_model.py
--rw-r--r--   0 runner    (1001) docker     (123)     3947 2023-05-08 20:41:24.000000 ax-platform-0.3.2/ax/models/tests/test_cbo_lcea.py
--rw-r--r--   0 runner    (1001) docker     (123)     2638 2023-05-08 20:41:24.000000 ax-platform-0.3.2/ax/models/tests/test_cbo_lcem.py
--rw-r--r--   0 runner    (1001) docker     (123)     3712 2023-05-08 20:41:24.000000 ax-platform-0.3.2/ax/models/tests/test_cbo_sac.py
--rw-r--r--   0 runner    (1001) docker     (123)     1760 2023-05-08 20:41:24.000000 ax-platform-0.3.2/ax/models/tests/test_discrete.py
--rw-r--r--   0 runner    (1001) docker     (123)     7743 2023-05-08 20:41:24.000000 ax-platform-0.3.2/ax/models/tests/test_eb_thompson.py
--rw-r--r--   0 runner    (1001) docker     (123)     3062 2023-05-08 20:41:24.000000 ax-platform-0.3.2/ax/models/tests/test_full_factorial.py
--rw-r--r--   0 runner    (1001) docker     (123)    49865 2023-05-08 20:41:24.000000 ax-platform-0.3.2/ax/models/tests/test_fully_bayesian.py
--rw-r--r--   0 runner    (1001) docker     (123)     7163 2023-05-08 20:41:24.000000 ax-platform-0.3.2/ax/models/tests/test_model_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     4777 2023-05-08 20:41:24.000000 ax-platform-0.3.2/ax/models/tests/test_posterior_mean.py
--rw-r--r--   0 runner    (1001) docker     (123)     3458 2023-05-08 20:41:24.000000 ax-platform-0.3.2/ax/models/tests/test_random.py
--rw-r--r--   0 runner    (1001) docker     (123)     1654 2023-05-08 20:41:24.000000 ax-platform-0.3.2/ax/models/tests/test_randomforest.py
--rw-r--r--   0 runner    (1001) docker     (123)     5470 2023-05-08 20:41:24.000000 ax-platform-0.3.2/ax/models/tests/test_rembo.py
--rw-r--r--   0 runner    (1001) docker     (123)     1185 2023-05-08 20:41:24.000000 ax-platform-0.3.2/ax/models/tests/test_rembo_initializer.py
--rw-r--r--   0 runner    (1001) docker     (123)    12435 2023-05-08 20:41:24.000000 ax-platform-0.3.2/ax/models/tests/test_sobol.py
--rw-r--r--   0 runner    (1001) docker     (123)    13220 2023-05-08 20:41:24.000000 ax-platform-0.3.2/ax/models/tests/test_thompson.py
--rw-r--r--   0 runner    (1001) docker     (123)     2613 2023-05-08 20:41:24.000000 ax-platform-0.3.2/ax/models/tests/test_torch.py
--rw-r--r--   0 runner    (1001) docker     (123)     8406 2023-05-08 20:41:24.000000 ax-platform-0.3.2/ax/models/tests/test_torch_model_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     9238 2023-05-08 20:41:24.000000 ax-platform-0.3.2/ax/models/tests/test_torch_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     6722 2023-05-08 20:41:24.000000 ax-platform-0.3.2/ax/models/tests/test_uniform.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 20:45:14.000666 ax-platform-0.3.2/ax/models/torch/
--rw-r--r--   0 runner    (1001) docker     (123)      202 2023-05-08 20:41:24.000000 ax-platform-0.3.2/ax/models/torch/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    29602 2023-05-08 20:41:24.000000 ax-platform-0.3.2/ax/models/torch/alebo.py
--rw-r--r--   0 runner    (1001) docker     (123)    24182 2023-05-08 20:41:24.000000 ax-platform-0.3.2/ax/models/torch/botorch.py
--rw-r--r--   0 runner    (1001) docker     (123)    31561 2023-05-08 20:41:24.000000 ax-platform-0.3.2/ax/models/torch/botorch_defaults.py
--rw-r--r--   0 runner    (1001) docker     (123)    15542 2023-05-08 20:41:24.000000 ax-platform-0.3.2/ax/models/torch/botorch_kg.py
--rw-r--r--   0 runner    (1001) docker     (123)    10264 2023-05-08 20:41:24.000000 ax-platform-0.3.2/ax/models/torch/botorch_mes.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 20:45:14.004667 ax-platform-0.3.2/ax/models/torch/botorch_modular/
--rw-r--r--   0 runner    (1001) docker     (123)      202 2023-05-08 20:41:24.000000 ax-platform-0.3.2/ax/models/torch/botorch_modular/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    25780 2023-05-08 20:41:24.000000 ax-platform-0.3.2/ax/models/torch/botorch_modular/acquisition.py
--rw-r--r--   0 runner    (1001) docker     (123)      488 2023-05-08 20:41:24.000000 ax-platform-0.3.2/ax/models/torch/botorch_modular/list_surrogate.py
--rw-r--r--   0 runner    (1001) docker     (123)    28867 2023-05-08 20:41:24.000000 ax-platform-0.3.2/ax/models/torch/botorch_modular/model.py
--rw-r--r--   0 runner    (1001) docker     (123)     3751 2023-05-08 20:41:24.000000 ax-platform-0.3.2/ax/models/torch/botorch_modular/multi_fidelity.py
--rw-r--r--   0 runner    (1001) docker     (123)     6223 2023-05-08 20:41:24.000000 ax-platform-0.3.2/ax/models/torch/botorch_modular/optimizer_argparse.py
--rw-r--r--   0 runner    (1001) docker     (123)    35511 2023-05-08 20:41:24.000000 ax-platform-0.3.2/ax/models/torch/botorch_modular/surrogate.py
--rw-r--r--   0 runner    (1001) docker     (123)    14652 2023-05-08 20:41:24.000000 ax-platform-0.3.2/ax/models/torch/botorch_modular/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)    15753 2023-05-08 20:41:24.000000 ax-platform-0.3.2/ax/models/torch/botorch_moo.py
--rw-r--r--   0 runner    (1001) docker     (123)    23861 2023-05-08 20:41:24.000000 ax-platform-0.3.2/ax/models/torch/botorch_moo_defaults.py
--rw-r--r--   0 runner    (1001) docker     (123)     7547 2023-05-08 20:41:24.000000 ax-platform-0.3.2/ax/models/torch/cbo_lcea.py
--rw-r--r--   0 runner    (1001) docker     (123)     3549 2023-05-08 20:41:24.000000 ax-platform-0.3.2/ax/models/torch/cbo_lcem.py
--rw-r--r--   0 runner    (1001) docker     (123)     4438 2023-05-08 20:41:24.000000 ax-platform-0.3.2/ax/models/torch/cbo_sac.py
--rw-r--r--   0 runner    (1001) docker     (123)      510 2023-05-08 20:41:24.000000 ax-platform-0.3.2/ax/models/torch/frontier_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)    24477 2023-05-08 20:41:24.000000 ax-platform-0.3.2/ax/models/torch/fully_bayesian.py
--rw-r--r--   0 runner    (1001) docker     (123)     7198 2023-05-08 20:41:24.000000 ax-platform-0.3.2/ax/models/torch/fully_bayesian_model_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     3531 2023-05-08 20:41:24.000000 ax-platform-0.3.2/ax/models/torch/posterior_mean.py
--rw-r--r--   0 runner    (1001) docker     (123)     4628 2023-05-08 20:41:24.000000 ax-platform-0.3.2/ax/models/torch/randomforest.py
--rw-r--r--   0 runner    (1001) docker     (123)     9745 2023-05-08 20:41:24.000000 ax-platform-0.3.2/ax/models/torch/rembo.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 20:45:14.004667 ax-platform-0.3.2/ax/models/torch/tests/
--rw-r--r--   0 runner    (1001) docker     (123)      202 2023-05-08 20:41:24.000000 ax-platform-0.3.2/ax/models/torch/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    28354 2023-05-08 20:41:24.000000 ax-platform-0.3.2/ax/models/torch/tests/test_acquisition.py
--rw-r--r--   0 runner    (1001) docker     (123)    39724 2023-05-08 20:41:24.000000 ax-platform-0.3.2/ax/models/torch/tests/test_model.py
--rw-r--r--   0 runner    (1001) docker     (123)     7248 2023-05-08 20:41:24.000000 ax-platform-0.3.2/ax/models/torch/tests/test_multi_fidelity.py
--rw-r--r--   0 runner    (1001) docker     (123)     5899 2023-05-08 20:41:24.000000 ax-platform-0.3.2/ax/models/torch/tests/test_optimizer_argparse.py
--rw-r--r--   0 runner    (1001) docker     (123)    51649 2023-05-08 20:41:24.000000 ax-platform-0.3.2/ax/models/torch/tests/test_surrogate.py
--rw-r--r--   0 runner    (1001) docker     (123)    19896 2023-05-08 20:41:24.000000 ax-platform-0.3.2/ax/models/torch/tests/test_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)    26784 2023-05-08 20:41:24.000000 ax-platform-0.3.2/ax/models/torch/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)    10947 2023-05-08 20:41:24.000000 ax-platform-0.3.2/ax/models/torch_base.py
--rw-r--r--   0 runner    (1001) docker     (123)      625 2023-05-08 20:41:24.000000 ax-platform-0.3.2/ax/models/types.py
--rw-r--r--   0 runner    (1001) docker     (123)     1452 2023-05-08 20:41:24.000000 ax-platform-0.3.2/ax/models/winsorization_config.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 20:45:14.016667 ax-platform-0.3.2/ax/plot/
--rw-r--r--   0 runner    (1001) docker     (123)      202 2023-05-08 20:41:24.000000 ax-platform-0.3.2/ax/plot/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2464 2023-05-08 20:41:24.000000 ax-platform-0.3.2/ax/plot/bandit_rollout.py
--rw-r--r--   0 runner    (1001) docker     (123)     2444 2023-05-08 20:41:24.000000 ax-platform-0.3.2/ax/plot/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     8617 2023-05-08 20:41:24.000000 ax-platform-0.3.2/ax/plot/benchmark.py
--rw-r--r--   0 runner    (1001) docker     (123)     2718 2023-05-08 20:41:24.000000 ax-platform-0.3.2/ax/plot/color.py
--rw-r--r--   0 runner    (1001) docker     (123)    32766 2023-05-08 20:41:24.000000 ax-platform-0.3.2/ax/plot/contour.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 20:45:14.016667 ax-platform-0.3.2/ax/plot/css/
--rw-r--r--   0 runner    (1001) docker     (123)      202 2023-05-08 20:41:24.000000 ax-platform-0.3.2/ax/plot/css/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      992 2023-05-08 20:41:24.000000 ax-platform-0.3.2/ax/plot/css/base.css
--rw-r--r--   0 runner    (1001) docker     (123)    24550 2023-05-08 20:41:24.000000 ax-platform-0.3.2/ax/plot/diagnostic.py
--rw-r--r--   0 runner    (1001) docker     (123)     9943 2023-05-08 20:41:24.000000 ax-platform-0.3.2/ax/plot/feature_importances.py
--rw-r--r--   0 runner    (1001) docker     (123)    31776 2023-05-08 20:41:24.000000 ax-platform-0.3.2/ax/plot/helper.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 20:45:14.016667 ax-platform-0.3.2/ax/plot/js/
--rw-r--r--   0 runner    (1001) docker     (123)      202 2023-05-08 20:41:24.000000 ax-platform-0.3.2/ax/plot/js/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 20:45:14.016667 ax-platform-0.3.2/ax/plot/js/common/
--rw-r--r--   0 runner    (1001) docker     (123)      202 2023-05-08 20:41:24.000000 ax-platform-0.3.2/ax/plot/js/common/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      344 2023-05-08 20:41:24.000000 ax-platform-0.3.2/ax/plot/js/common/css.js
--rw-r--r--   0 runner    (1001) docker     (123)     5344 2023-05-08 20:41:24.000000 ax-platform-0.3.2/ax/plot/js/common/helpers.js
--rw-r--r--   0 runner    (1001) docker     (123)      369 2023-05-08 20:41:24.000000 ax-platform-0.3.2/ax/plot/js/common/plotly_offline.js
--rw-r--r--   0 runner    (1001) docker     (123)      385 2023-05-08 20:41:24.000000 ax-platform-0.3.2/ax/plot/js/common/plotly_online.js
--rw-r--r--   0 runner    (1001) docker     (123)      342 2023-05-08 20:41:24.000000 ax-platform-0.3.2/ax/plot/js/common/plotly_requires.js
--rw-r--r--   0 runner    (1001) docker     (123)      269 2023-05-08 20:41:24.000000 ax-platform-0.3.2/ax/plot/js/generic_plotly.js
--rw-r--r--   0 runner    (1001) docker     (123)     2378 2023-05-08 20:41:24.000000 ax-platform-0.3.2/ax/plot/marginal_effects.py
--rw-r--r--   0 runner    (1001) docker     (123)     3159 2023-05-08 20:41:24.000000 ax-platform-0.3.2/ax/plot/parallel_coordinates.py
--rw-r--r--   0 runner    (1001) docker     (123)    38724 2023-05-08 20:41:24.000000 ax-platform-0.3.2/ax/plot/pareto_frontier.py
--rw-r--r--   0 runner    (1001) docker     (123)    26196 2023-05-08 20:41:24.000000 ax-platform-0.3.2/ax/plot/pareto_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     4362 2023-05-08 20:41:24.000000 ax-platform-0.3.2/ax/plot/render.py
--rw-r--r--   0 runner    (1001) docker     (123)    58188 2023-05-08 20:41:24.000000 ax-platform-0.3.2/ax/plot/scatter.py
--rw-r--r--   0 runner    (1001) docker     (123)    19873 2023-05-08 20:41:24.000000 ax-platform-0.3.2/ax/plot/slice.py
--rw-r--r--   0 runner    (1001) docker     (123)     5646 2023-05-08 20:41:24.000000 ax-platform-0.3.2/ax/plot/table_view.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 20:45:14.020668 ax-platform-0.3.2/ax/plot/tests/
--rw-r--r--   0 runner    (1001) docker     (123)      202 2023-05-08 20:41:24.000000 ax-platform-0.3.2/ax/plot/tests/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 20:45:14.020668 ax-platform-0.3.2/ax/plot/tests/long_running/
--rw-r--r--   0 runner    (1001) docker     (123)     2339 2023-05-08 20:41:24.000000 ax-platform-0.3.2/ax/plot/tests/long_running/test_pareto_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     2160 2023-05-08 20:41:24.000000 ax-platform-0.3.2/ax/plot/tests/test_contours.py
--rw-r--r--   0 runner    (1001) docker     (123)     2125 2023-05-08 20:41:24.000000 ax-platform-0.3.2/ax/plot/tests/test_diagnostic.py
--rw-r--r--   0 runner    (1001) docker     (123)     4372 2023-05-08 20:41:24.000000 ax-platform-0.3.2/ax/plot/tests/test_feature_importances.py
--rw-r--r--   0 runner    (1001) docker     (123)     1609 2023-05-08 20:41:24.000000 ax-platform-0.3.2/ax/plot/tests/test_fitted_scatter.py
--rw-r--r--   0 runner    (1001) docker     (123)     1291 2023-05-08 20:41:24.000000 ax-platform-0.3.2/ax/plot/tests/test_helper.py
--rw-r--r--   0 runner    (1001) docker     (123)      822 2023-05-08 20:41:24.000000 ax-platform-0.3.2/ax/plot/tests/test_parallel_coordinates.py
--rw-r--r--   0 runner    (1001) docker     (123)    14241 2023-05-08 20:41:24.000000 ax-platform-0.3.2/ax/plot/tests/test_pareto_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     1552 2023-05-08 20:41:24.000000 ax-platform-0.3.2/ax/plot/tests/test_slices.py
--rw-r--r--   0 runner    (1001) docker     (123)     4752 2023-05-08 20:41:24.000000 ax-platform-0.3.2/ax/plot/tests/test_tile_fitted.py
--rw-r--r--   0 runner    (1001) docker     (123)     2563 2023-05-08 20:41:24.000000 ax-platform-0.3.2/ax/plot/tests/test_traces.py
--rw-r--r--   0 runner    (1001) docker     (123)    27668 2023-05-08 20:41:24.000000 ax-platform-0.3.2/ax/plot/trace.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 20:45:14.024668 ax-platform-0.3.2/ax/runners/
--rw-r--r--   0 runner    (1001) docker     (123)      394 2023-05-08 20:41:24.000000 ax-platform-0.3.2/ax/runners/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5514 2023-05-08 20:41:24.000000 ax-platform-0.3.2/ax/runners/botorch_test_problem.py
--rw-r--r--   0 runner    (1001) docker     (123)     3386 2023-05-08 20:41:24.000000 ax-platform-0.3.2/ax/runners/simulated_backend.py
--rw-r--r--   0 runner    (1001) docker     (123)     1220 2023-05-08 20:41:24.000000 ax-platform-0.3.2/ax/runners/synthetic.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 20:45:14.024668 ax-platform-0.3.2/ax/runners/tests/
--rw-r--r--   0 runner    (1001) docker     (123)      202 2023-05-08 20:41:24.000000 ax-platform-0.3.2/ax/runners/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6264 2023-05-08 20:41:24.000000 ax-platform-0.3.2/ax/runners/tests/test_torchx.py
--rw-r--r--   0 runner    (1001) docker     (123)     6993 2023-05-08 20:41:24.000000 ax-platform-0.3.2/ax/runners/torchx.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 20:45:14.028668 ax-platform-0.3.2/ax/service/
--rw-r--r--   0 runner    (1001) docker     (123)      311 2023-05-08 20:41:24.000000 ax-platform-0.3.2/ax/service/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    78094 2023-05-08 20:41:24.000000 ax-platform-0.3.2/ax/service/ax_client.py
--rw-r--r--   0 runner    (1001) docker     (123)     7891 2023-05-08 20:41:24.000000 ax-platform-0.3.2/ax/service/interactive_loop.py
--rw-r--r--   0 runner    (1001) docker     (123)    11683 2023-05-08 20:41:24.000000 ax-platform-0.3.2/ax/service/managed_loop.py
--rw-r--r--   0 runner    (1001) docker     (123)    76782 2023-05-08 20:41:24.000000 ax-platform-0.3.2/ax/service/scheduler.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 20:45:14.032668 ax-platform-0.3.2/ax/service/tests/
--rw-r--r--   0 runner    (1001) docker     (123)      202 2023-05-08 20:41:24.000000 ax-platform-0.3.2/ax/service/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)   119626 2023-05-08 20:41:24.000000 ax-platform-0.3.2/ax/service/tests/test_ax_client.py
--rw-r--r--   0 runner    (1001) docker     (123)     3862 2023-05-08 20:41:24.000000 ax-platform-0.3.2/ax/service/tests/test_best_point.py
--rw-r--r--   0 runner    (1001) docker     (123)    21148 2023-05-08 20:41:24.000000 ax-platform-0.3.2/ax/service/tests/test_best_point_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     1668 2023-05-08 20:41:24.000000 ax-platform-0.3.2/ax/service/tests/test_early_stopping.py
--rw-r--r--   0 runner    (1001) docker     (123)     5335 2023-05-08 20:41:24.000000 ax-platform-0.3.2/ax/service/tests/test_global_stopping.py
--rw-r--r--   0 runner    (1001) docker     (123)    12675 2023-05-08 20:41:24.000000 ax-platform-0.3.2/ax/service/tests/test_instantiation_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     3457 2023-05-08 20:41:24.000000 ax-platform-0.3.2/ax/service/tests/test_interactive_loop.py
--rw-r--r--   0 runner    (1001) docker     (123)    20401 2023-05-08 20:41:24.000000 ax-platform-0.3.2/ax/service/tests/test_managed_loop.py
--rw-r--r--   0 runner    (1001) docker     (123)    19334 2023-05-08 20:41:24.000000 ax-platform-0.3.2/ax/service/tests/test_report_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)    51692 2023-05-08 20:41:24.000000 ax-platform-0.3.2/ax/service/tests/test_scheduler.py
--rw-r--r--   0 runner    (1001) docker     (123)    14129 2023-05-08 20:41:24.000000 ax-platform-0.3.2/ax/service/tests/test_with_db_settings_base.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 20:45:14.036669 ax-platform-0.3.2/ax/service/utils/
--rw-r--r--   0 runner    (1001) docker     (123)      202 2023-05-08 20:41:24.000000 ax-platform-0.3.2/ax/service/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    34580 2023-05-08 20:41:24.000000 ax-platform-0.3.2/ax/service/utils/best_point.py
--rw-r--r--   0 runner    (1001) docker     (123)    23798 2023-05-08 20:41:24.000000 ax-platform-0.3.2/ax/service/utils/best_point_mixin.py
--rw-r--r--   0 runner    (1001) docker     (123)     1916 2023-05-08 20:41:24.000000 ax-platform-0.3.2/ax/service/utils/early_stopping.py
--rw-r--r--   0 runner    (1001) docker     (123)    37588 2023-05-08 20:41:24.000000 ax-platform-0.3.2/ax/service/utils/instantiation.py
--rw-r--r--   0 runner    (1001) docker     (123)    42578 2023-05-08 20:41:24.000000 ax-platform-0.3.2/ax/service/utils/report_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     6625 2023-05-08 20:41:24.000000 ax-platform-0.3.2/ax/service/utils/scheduler_options.py
--rw-r--r--   0 runner    (1001) docker     (123)    21704 2023-05-08 20:41:24.000000 ax-platform-0.3.2/ax/service/utils/with_db_settings_base.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 20:45:14.040669 ax-platform-0.3.2/ax/storage/
--rw-r--r--   0 runner    (1001) docker     (123)      313 2023-05-08 20:41:24.000000 ax-platform-0.3.2/ax/storage/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7250 2023-05-08 20:41:24.000000 ax-platform-0.3.2/ax/storage/botorch_modular_registry.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 20:45:14.044669 ax-platform-0.3.2/ax/storage/json_store/
--rw-r--r--   0 runner    (1001) docker     (123)      378 2023-05-08 20:41:24.000000 ax-platform-0.3.2/ax/storage/json_store/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    28491 2023-05-08 20:41:24.000000 ax-platform-0.3.2/ax/storage/json_store/decoder.py
--rw-r--r--   0 runner    (1001) docker     (123)    10555 2023-05-08 20:41:24.000000 ax-platform-0.3.2/ax/storage/json_store/decoders.py
--rw-r--r--   0 runner    (1001) docker     (123)     6670 2023-05-08 20:41:24.000000 ax-platform-0.3.2/ax/storage/json_store/encoder.py
--rw-r--r--   0 runner    (1001) docker     (123)    25060 2023-05-08 20:41:24.000000 ax-platform-0.3.2/ax/storage/json_store/encoders.py
--rw-r--r--   0 runner    (1001) docker     (123)     1217 2023-05-08 20:41:24.000000 ax-platform-0.3.2/ax/storage/json_store/load.py
--rw-r--r--   0 runner    (1001) docker     (123)    15396 2023-05-08 20:41:24.000000 ax-platform-0.3.2/ax/storage/json_store/registry.py
--rw-r--r--   0 runner    (1001) docker     (123)     1743 2023-05-08 20:41:24.000000 ax-platform-0.3.2/ax/storage/json_store/save.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 20:45:14.044669 ax-platform-0.3.2/ax/storage/json_store/tests/
--rw-r--r--   0 runner    (1001) docker     (123)      202 2023-05-08 20:41:24.000000 ax-platform-0.3.2/ax/storage/json_store/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    22778 2023-05-08 20:41:24.000000 ax-platform-0.3.2/ax/storage/json_store/tests/test_json_store.py
--rw-r--r--   0 runner    (1001) docker     (123)     4675 2023-05-08 20:41:24.000000 ax-platform-0.3.2/ax/storage/metric_registry.py
--rw-r--r--   0 runner    (1001) docker     (123)     9327 2023-05-08 20:41:24.000000 ax-platform-0.3.2/ax/storage/registry_bundle.py
--rw-r--r--   0 runner    (1001) docker     (123)     4177 2023-05-08 20:41:24.000000 ax-platform-0.3.2/ax/storage/runner_registry.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 20:45:14.052670 ax-platform-0.3.2/ax/storage/sqa_store/
--rw-r--r--   0 runner    (1001) docker     (123)      543 2023-05-08 20:41:24.000000 ax-platform-0.3.2/ax/storage/sqa_store/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     9573 2023-05-08 20:41:24.000000 ax-platform-0.3.2/ax/storage/sqa_store/db.py
--rw-r--r--   0 runner    (1001) docker     (123)    49885 2023-05-08 20:41:24.000000 ax-platform-0.3.2/ax/storage/sqa_store/decoder.py
--rw-r--r--   0 runner    (1001) docker     (123)      620 2023-05-08 20:41:24.000000 ax-platform-0.3.2/ax/storage/sqa_store/delete.py
--rw-r--r--   0 runner    (1001) docker     (123)    44346 2023-05-08 20:41:24.000000 ax-platform-0.3.2/ax/storage/sqa_store/encoder.py
--rw-r--r--   0 runner    (1001) docker     (123)     3359 2023-05-08 20:41:24.000000 ax-platform-0.3.2/ax/storage/sqa_store/json.py
--rw-r--r--   0 runner    (1001) docker     (123)    19755 2023-05-08 20:41:24.000000 ax-platform-0.3.2/ax/storage/sqa_store/load.py
--rw-r--r--   0 runner    (1001) docker     (123)     1637 2023-05-08 20:41:24.000000 ax-platform-0.3.2/ax/storage/sqa_store/reduced_state.py
--rw-r--r--   0 runner    (1001) docker     (123)    18600 2023-05-08 20:41:24.000000 ax-platform-0.3.2/ax/storage/sqa_store/save.py
--rw-r--r--   0 runner    (1001) docker     (123)    25389 2023-05-08 20:41:24.000000 ax-platform-0.3.2/ax/storage/sqa_store/sqa_classes.py
--rw-r--r--   0 runner    (1001) docker     (123)     4480 2023-05-08 20:41:24.000000 ax-platform-0.3.2/ax/storage/sqa_store/sqa_config.py
--rw-r--r--   0 runner    (1001) docker     (123)     2456 2023-05-08 20:41:24.000000 ax-platform-0.3.2/ax/storage/sqa_store/sqa_enum.py
--rw-r--r--   0 runner    (1001) docker     (123)      841 2023-05-08 20:41:24.000000 ax-platform-0.3.2/ax/storage/sqa_store/structs.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 20:45:14.056670 ax-platform-0.3.2/ax/storage/sqa_store/tests/
--rw-r--r--   0 runner    (1001) docker     (123)      202 2023-05-08 20:41:24.000000 ax-platform-0.3.2/ax/storage/sqa_store/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    73084 2023-05-08 20:41:24.000000 ax-platform-0.3.2/ax/storage/sqa_store/tests/test_sqa_store.py
--rw-r--r--   0 runner    (1001) docker     (123)     4304 2023-05-08 20:41:24.000000 ax-platform-0.3.2/ax/storage/sqa_store/tests/test_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     6577 2023-05-08 20:41:24.000000 ax-platform-0.3.2/ax/storage/sqa_store/tests/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)      984 2023-05-08 20:41:24.000000 ax-platform-0.3.2/ax/storage/sqa_store/timestamp.py
--rw-r--r--   0 runner    (1001) docker     (123)     6376 2023-05-08 20:41:24.000000 ax-platform-0.3.2/ax/storage/sqa_store/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     4008 2023-05-08 20:41:24.000000 ax-platform-0.3.2/ax/storage/sqa_store/validation.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 20:45:14.056670 ax-platform-0.3.2/ax/storage/tests/
--rw-r--r--   0 runner    (1001) docker     (123)     1706 2023-05-08 20:41:24.000000 ax-platform-0.3.2/ax/storage/tests/test_registry_bundle.py
--rw-r--r--   0 runner    (1001) docker     (123)     2980 2023-05-08 20:41:24.000000 ax-platform-0.3.2/ax/storage/transform_registry.py
--rw-r--r--   0 runner    (1001) docker     (123)     1328 2023-05-08 20:41:24.000000 ax-platform-0.3.2/ax/storage/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 20:45:14.056670 ax-platform-0.3.2/ax/telemetry/
--rw-r--r--   0 runner    (1001) docker     (123)      488 2023-05-08 20:41:24.000000 ax-platform-0.3.2/ax/telemetry/common.py
--rw-r--r--   0 runner    (1001) docker     (123)    10913 2023-05-08 20:41:24.000000 ax-platform-0.3.2/ax/telemetry/experiment.py
--rw-r--r--   0 runner    (1001) docker     (123)     2355 2023-05-08 20:41:24.000000 ax-platform-0.3.2/ax/telemetry/generation_strategy.py
--rw-r--r--   0 runner    (1001) docker     (123)     2630 2023-05-08 20:41:24.000000 ax-platform-0.3.2/ax/telemetry/optimization.py
--rw-r--r--   0 runner    (1001) docker     (123)     6951 2023-05-08 20:41:24.000000 ax-platform-0.3.2/ax/telemetry/scheduler.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 20:45:14.060670 ax-platform-0.3.2/ax/telemetry/tests/
--rw-r--r--   0 runner    (1001) docker     (123)     2464 2023-05-08 20:41:24.000000 ax-platform-0.3.2/ax/telemetry/tests/test_experiment.py
--rw-r--r--   0 runner    (1001) docker     (123)     1015 2023-05-08 20:41:24.000000 ax-platform-0.3.2/ax/telemetry/tests/test_generation_strategy.py
--rw-r--r--   0 runner    (1001) docker     (123)     3073 2023-05-08 20:41:24.000000 ax-platform-0.3.2/ax/telemetry/tests/test_optimization.py
--rw-r--r--   0 runner    (1001) docker     (123)     3873 2023-05-08 20:41:24.000000 ax-platform-0.3.2/ax/telemetry/tests/test_scheduler.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 20:45:14.060670 ax-platform-0.3.2/ax/utils/
--rw-r--r--   0 runner    (1001) docker     (123)      202 2023-05-08 20:41:24.000000 ax-platform-0.3.2/ax/utils/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 20:45:14.068671 ax-platform-0.3.2/ax/utils/common/
--rw-r--r--   0 runner    (1001) docker     (123)      202 2023-05-08 20:41:24.000000 ax-platform-0.3.2/ax/utils/common/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1586 2023-05-08 20:41:24.000000 ax-platform-0.3.2/ax/utils/common/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     2867 2023-05-08 20:41:24.000000 ax-platform-0.3.2/ax/utils/common/constants.py
--rw-r--r--   0 runner    (1001) docker     (123)     2829 2023-05-08 20:41:24.000000 ax-platform-0.3.2/ax/utils/common/decorator.py
--rw-r--r--   0 runner    (1001) docker     (123)     1631 2023-05-08 20:41:24.000000 ax-platform-0.3.2/ax/utils/common/docutils.py
--rw-r--r--   0 runner    (1001) docker     (123)     8237 2023-05-08 20:41:24.000000 ax-platform-0.3.2/ax/utils/common/equality.py
--rw-r--r--   0 runner    (1001) docker     (123)    10612 2023-05-08 20:41:24.000000 ax-platform-0.3.2/ax/utils/common/executils.py
--rw-r--r--   0 runner    (1001) docker     (123)     5226 2023-05-08 20:41:24.000000 ax-platform-0.3.2/ax/utils/common/kwargs.py
--rw-r--r--   0 runner    (1001) docker     (123)     7720 2023-05-08 20:41:24.000000 ax-platform-0.3.2/ax/utils/common/logger.py
--rw-r--r--   0 runner    (1001) docker     (123)     1110 2023-05-08 20:41:24.000000 ax-platform-0.3.2/ax/utils/common/mock.py
--rw-r--r--   0 runner    (1001) docker     (123)     6748 2023-05-08 20:41:24.000000 ax-platform-0.3.2/ax/utils/common/result.py
--rw-r--r--   0 runner    (1001) docker     (123)     5082 2023-05-08 20:41:24.000000 ax-platform-0.3.2/ax/utils/common/serialization.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 20:45:14.072671 ax-platform-0.3.2/ax/utils/common/tests/
--rw-r--r--   0 runner    (1001) docker     (123)      202 2023-05-08 20:41:24.000000 ax-platform-0.3.2/ax/utils/common/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1187 2023-05-08 20:41:24.000000 ax-platform-0.3.2/ax/utils/common/tests/test_docutils.py
--rw-r--r--   0 runner    (1001) docker     (123)     2666 2023-05-08 20:41:24.000000 ax-platform-0.3.2/ax/utils/common/tests/test_equality.py
--rw-r--r--   0 runner    (1001) docker     (123)    10218 2023-05-08 20:41:24.000000 ax-platform-0.3.2/ax/utils/common/tests/test_executils.py
--rw-r--r--   0 runner    (1001) docker     (123)     5761 2023-05-08 20:41:24.000000 ax-platform-0.3.2/ax/utils/common/tests/test_kwargutils.py
--rw-r--r--   0 runner    (1001) docker     (123)     2887 2023-05-08 20:41:24.000000 ax-platform-0.3.2/ax/utils/common/tests/test_logger.py
--rw-r--r--   0 runner    (1001) docker     (123)     2250 2023-05-08 20:41:24.000000 ax-platform-0.3.2/ax/utils/common/tests/test_result.py
--rw-r--r--   0 runner    (1001) docker     (123)      824 2023-05-08 20:41:24.000000 ax-platform-0.3.2/ax/utils/common/tests/test_serialization.py
--rw-r--r--   0 runner    (1001) docker     (123)     3393 2023-05-08 20:41:24.000000 ax-platform-0.3.2/ax/utils/common/tests/test_testutils.py
--rw-r--r--   0 runner    (1001) docker     (123)     2363 2023-05-08 20:41:24.000000 ax-platform-0.3.2/ax/utils/common/tests/test_typeutils.py
--rw-r--r--   0 runner    (1001) docker     (123)    16165 2023-05-08 20:41:24.000000 ax-platform-0.3.2/ax/utils/common/testutils.py
--rw-r--r--   0 runner    (1001) docker     (123)     1405 2023-05-08 20:41:24.000000 ax-platform-0.3.2/ax/utils/common/timeutils.py
--rw-r--r--   0 runner    (1001) docker     (123)     4993 2023-05-08 20:41:24.000000 ax-platform-0.3.2/ax/utils/common/typeutils.py
--rw-r--r--   0 runner    (1001) docker     (123)     1188 2023-05-08 20:41:24.000000 ax-platform-0.3.2/ax/utils/common/typeutils_torch.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 20:45:14.076672 ax-platform-0.3.2/ax/utils/flake8_plugins/
--rw-r--r--   0 runner    (1001) docker     (123)      202 2023-05-08 20:41:24.000000 ax-platform-0.3.2/ax/utils/flake8_plugins/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3279 2023-05-08 20:41:24.000000 ax-platform-0.3.2/ax/utils/flake8_plugins/docstring_checker.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 20:45:14.076672 ax-platform-0.3.2/ax/utils/measurement/
--rw-r--r--   0 runner    (1001) docker     (123)      202 2023-05-08 20:41:24.000000 ax-platform-0.3.2/ax/utils/measurement/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    11368 2023-05-08 20:41:24.000000 ax-platform-0.3.2/ax/utils/measurement/synthetic_functions.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 20:45:14.076672 ax-platform-0.3.2/ax/utils/measurement/tests/
--rw-r--r--   0 runner    (1001) docker     (123)      202 2023-05-08 20:41:24.000000 ax-platform-0.3.2/ax/utils/measurement/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6182 2023-05-08 20:41:24.000000 ax-platform-0.3.2/ax/utils/measurement/tests/test_synthetic_functions.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 20:45:14.076672 ax-platform-0.3.2/ax/utils/notebook/
--rw-r--r--   0 runner    (1001) docker     (123)      202 2023-05-08 20:41:24.000000 ax-platform-0.3.2/ax/utils/notebook/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1408 2023-05-08 20:41:24.000000 ax-platform-0.3.2/ax/utils/notebook/plotting.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 20:45:14.076672 ax-platform-0.3.2/ax/utils/report/
--rw-r--r--   0 runner    (1001) docker     (123)      202 2023-05-08 20:41:24.000000 ax-platform-0.3.2/ax/utils/report/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4236 2023-05-08 20:41:24.000000 ax-platform-0.3.2/ax/utils/report/render.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 20:45:14.080672 ax-platform-0.3.2/ax/utils/report/resources/
--rw-r--r--   0 runner    (1001) docker     (123)      202 2023-05-08 20:41:24.000000 ax-platform-0.3.2/ax/utils/report/resources/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1240 2023-05-08 20:41:24.000000 ax-platform-0.3.2/ax/utils/report/resources/base_template.html
--rw-r--r--   0 runner    (1001) docker     (123)     3150 2023-05-08 20:41:24.000000 ax-platform-0.3.2/ax/utils/report/resources/report.css
--rw-r--r--   0 runner    (1001) docker     (123)      215 2023-05-08 20:41:24.000000 ax-platform-0.3.2/ax/utils/report/resources/simple_template.html
--rw-r--r--   0 runner    (1001) docker     (123)      657 2023-05-08 20:41:24.000000 ax-platform-0.3.2/ax/utils/report/resources/sufficient_statistic.html
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 20:45:14.080672 ax-platform-0.3.2/ax/utils/report/tests/
--rw-r--r--   0 runner    (1001) docker     (123)      202 2023-05-08 20:41:24.000000 ax-platform-0.3.2/ax/utils/report/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1099 2023-05-08 20:41:24.000000 ax-platform-0.3.2/ax/utils/report/tests/test_render.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 20:45:14.084672 ax-platform-0.3.2/ax/utils/sensitivity/
--rw-r--r--   0 runner    (1001) docker     (123)      202 2023-05-08 20:41:24.000000 ax-platform-0.3.2/ax/utils/sensitivity/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4884 2023-05-08 20:41:24.000000 ax-platform-0.3.2/ax/utils/sensitivity/derivative_gp.py
--rw-r--r--   0 runner    (1001) docker     (123)    15644 2023-05-08 20:41:24.000000 ax-platform-0.3.2/ax/utils/sensitivity/derivative_measures.py
--rw-r--r--   0 runner    (1001) docker     (123)    35734 2023-05-08 20:41:24.000000 ax-platform-0.3.2/ax/utils/sensitivity/sobol_measures.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 20:45:14.084672 ax-platform-0.3.2/ax/utils/sensitivity/tests/
--rw-r--r--   0 runner    (1001) docker     (123)      202 2023-05-08 20:41:24.000000 ax-platform-0.3.2/ax/utils/sensitivity/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    14117 2023-05-08 20:41:24.000000 ax-platform-0.3.2/ax/utils/sensitivity/tests/test_sensitivity.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 20:45:14.084672 ax-platform-0.3.2/ax/utils/stats/
--rw-r--r--   0 runner    (1001) docker     (123)      202 2023-05-08 20:41:24.000000 ax-platform-0.3.2/ax/utils/stats/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    13192 2023-05-08 20:41:24.000000 ax-platform-0.3.2/ax/utils/stats/statstools.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 20:45:14.088672 ax-platform-0.3.2/ax/utils/stats/tests/
--rw-r--r--   0 runner    (1001) docker     (123)      202 2023-05-08 20:41:24.000000 ax-platform-0.3.2/ax/utils/stats/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4973 2023-05-08 20:41:24.000000 ax-platform-0.3.2/ax/utils/stats/tests/test_statstools.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 20:45:14.092673 ax-platform-0.3.2/ax/utils/testing/
--rw-r--r--   0 runner    (1001) docker     (123)      202 2023-05-08 20:41:24.000000 ax-platform-0.3.2/ax/utils/testing/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4277 2023-05-08 20:41:24.000000 ax-platform-0.3.2/ax/utils/testing/backend_scheduler.py
--rw-r--r--   0 runner    (1001) docker     (123)    18626 2023-05-08 20:41:24.000000 ax-platform-0.3.2/ax/utils/testing/backend_simulator.py
--rw-r--r--   0 runner    (1001) docker     (123)     4213 2023-05-08 20:41:24.000000 ax-platform-0.3.2/ax/utils/testing/benchmark_stubs.py
--rw-r--r--   0 runner    (1001) docker     (123)    65879 2023-05-08 20:41:24.000000 ax-platform-0.3.2/ax/utils/testing/core_stubs.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-08 20:41:24.000000 ax-platform-0.3.2/ax/utils/testing/manifest.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 20:45:14.092673 ax-platform-0.3.2/ax/utils/testing/metrics/
--rw-r--r--   0 runner    (1001) docker     (123)      202 2023-05-08 20:41:24.000000 ax-platform-0.3.2/ax/utils/testing/metrics/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1649 2023-05-08 20:41:24.000000 ax-platform-0.3.2/ax/utils/testing/metrics/backend_simulator_map.py
--rw-r--r--   0 runner    (1001) docker     (123)     2432 2023-05-08 20:41:24.000000 ax-platform-0.3.2/ax/utils/testing/metrics/branin_backend_map.py
--rw-r--r--   0 runner    (1001) docker     (123)     5511 2023-05-08 20:41:24.000000 ax-platform-0.3.2/ax/utils/testing/mock.py
--rw-r--r--   0 runner    (1001) docker     (123)    12305 2023-05-08 20:41:24.000000 ax-platform-0.3.2/ax/utils/testing/modeling_stubs.py
--rw-r--r--   0 runner    (1001) docker     (123)      791 2023-05-08 20:41:24.000000 ax-platform-0.3.2/ax/utils/testing/test_init_files.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 20:45:14.096673 ax-platform-0.3.2/ax/utils/testing/tests/
--rw-r--r--   0 runner    (1001) docker     (123)      202 2023-05-08 20:41:24.000000 ax-platform-0.3.2/ax/utils/testing/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5402 2023-05-08 20:41:24.000000 ax-platform-0.3.2/ax/utils/testing/tests/test_backend_simulator.py
--rw-r--r--   0 runner    (1001) docker     (123)     2012 2023-05-08 20:41:24.000000 ax-platform-0.3.2/ax/utils/testing/tests/test_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     1544 2023-05-08 20:41:24.000000 ax-platform-0.3.2/ax/utils/testing/torch_stubs.py
--rw-r--r--   0 runner    (1001) docker     (123)     1086 2023-05-08 20:41:24.000000 ax-platform-0.3.2/ax/utils/testing/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 20:45:14.096673 ax-platform-0.3.2/ax/utils/tutorials/
--rw-r--r--   0 runner    (1001) docker     (123)      202 2023-05-08 20:41:24.000000 ax-platform-0.3.2/ax/utils/tutorials/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     9247 2023-05-08 20:41:24.000000 ax-platform-0.3.2/ax/utils/tutorials/cnn_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)      160 2023-05-08 20:45:13.000000 ax-platform-0.3.2/ax/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 20:45:14.096673 ax-platform-0.3.2/ax_platform.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     9979 2023-05-08 20:45:13.000000 ax-platform-0.3.2/ax_platform.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    21178 2023-05-08 20:45:13.000000 ax-platform-0.3.2/ax_platform.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-08 20:45:13.000000 ax-platform-0.3.2/ax_platform.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1005 2023-05-08 20:45:13.000000 ax-platform-0.3.2/ax_platform.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        3 2023-05-08 20:45:13.000000 ax-platform-0.3.2/ax_platform.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 20:45:14.104674 ax-platform-0.3.2/docs/
--rw-r--r--   0 runner    (1001) docker     (123)      145 2023-05-08 20:41:24.000000 ax-platform-0.3.2/docs/algo-overview.md
--rw-r--r--   0 runner    (1001) docker     (123)     6270 2023-05-08 20:41:24.000000 ax-platform-0.3.2/docs/api.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 20:45:14.116675 ax-platform-0.3.2/docs/assets/
--rw-r--r--   0 runner    (1001) docker     (123)    81587 2023-05-08 20:41:24.000000 ax-platform-0.3.2/docs/assets/bandit_allocation.png
--rw-r--r--   0 runner    (1001) docker     (123)   345484 2023-05-08 20:41:24.000000 ax-platform-0.3.2/docs/assets/bo_1d_opt.gif
--rw-r--r--   0 runner    (1001) docker     (123)   156260 2023-05-08 20:41:24.000000 ax-platform-0.3.2/docs/assets/contour.js
--rw-r--r--   0 runner    (1001) docker     (123)    14875 2023-05-08 20:41:24.000000 ax-platform-0.3.2/docs/assets/cv.js
--rw-r--r--   0 runner    (1001) docker     (123)   131612 2023-05-08 20:41:24.000000 ax-platform-0.3.2/docs/assets/example_shrinkage.png
--rw-r--r--   0 runner    (1001) docker     (123)    13598 2023-05-08 20:41:24.000000 ax-platform-0.3.2/docs/assets/fitted.js
--rw-r--r--   0 runner    (1001) docker     (123)    65905 2023-05-08 20:41:24.000000 ax-platform-0.3.2/docs/assets/gp_opt.png
--rw-r--r--   0 runner    (1001) docker     (123)   349223 2023-05-08 20:41:24.000000 ax-platform-0.3.2/docs/assets/gp_posterior.png
--rw-r--r--   0 runner    (1001) docker     (123)   121838 2023-05-08 20:41:24.000000 ax-platform-0.3.2/docs/assets/mab_animate.gif
--rw-r--r--   0 runner    (1001) docker     (123)   132372 2023-05-08 20:41:24.000000 ax-platform-0.3.2/docs/assets/mab_probs.png
--rw-r--r--   0 runner    (1001) docker     (123)   325134 2023-05-08 20:41:24.000000 ax-platform-0.3.2/docs/assets/mab_regret.png
--rw-r--r--   0 runner    (1001) docker     (123)    26226 2023-05-08 20:41:24.000000 ax-platform-0.3.2/docs/assets/slice.js
--rw-r--r--   0 runner    (1001) docker     (123)     8863 2023-05-08 20:41:24.000000 ax-platform-0.3.2/docs/banditopt.md
--rw-r--r--   0 runner    (1001) docker     (123)    10181 2023-05-08 20:41:24.000000 ax-platform-0.3.2/docs/bayesopt.md
--rw-r--r--   0 runner    (1001) docker     (123)     9871 2023-05-08 20:41:24.000000 ax-platform-0.3.2/docs/core.md
--rw-r--r--   0 runner    (1001) docker     (123)     2484 2023-05-08 20:41:24.000000 ax-platform-0.3.2/docs/data.md
--rw-r--r--   0 runner    (1001) docker     (123)     6876 2023-05-08 20:41:24.000000 ax-platform-0.3.2/docs/glossary.md
--rw-r--r--   0 runner    (1001) docker     (123)     3374 2023-05-08 20:41:24.000000 ax-platform-0.3.2/docs/installation.md
--rw-r--r--   0 runner    (1001) docker     (123)    22509 2023-05-08 20:41:24.000000 ax-platform-0.3.2/docs/models.md
--rw-r--r--   0 runner    (1001) docker     (123)     5596 2023-05-08 20:41:24.000000 ax-platform-0.3.2/docs/storage.md
--rw-r--r--   0 runner    (1001) docker     (123)     7784 2023-05-08 20:41:24.000000 ax-platform-0.3.2/docs/trial-evaluation.md
--rw-r--r--   0 runner    (1001) docker     (123)     2218 2023-05-08 20:41:24.000000 ax-platform-0.3.2/docs/why-ax.md
--rw-r--r--   0 runner    (1001) docker     (123)      158 2023-05-08 20:41:24.000000 ax-platform-0.3.2/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)      319 2023-05-08 20:41:24.000000 ax-platform-0.3.2/pytest.ini
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 20:45:14.124675 ax-platform-0.3.2/scripts/
--rwxr-xr-x   0 runner    (1001) docker     (123)      632 2023-05-08 20:41:24.000000 ax-platform-0.3.2/scripts/build_ax.sh
--rwxr-xr-x   0 runner    (1001) docker     (123)      535 2023-05-08 20:41:24.000000 ax-platform-0.3.2/scripts/docker_install.sh
--rw-r--r--   0 runner    (1001) docker     (123)      342 2023-05-08 20:41:24.000000 ax-platform-0.3.2/scripts/import_ax.py
--rw-r--r--   0 runner    (1001) docker     (123)     2263 2023-05-08 20:41:24.000000 ax-platform-0.3.2/scripts/insert_api_refs.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     4160 2023-05-08 20:41:24.000000 ax-platform-0.3.2/scripts/make_docs.sh
--rw-r--r--   0 runner    (1001) docker     (123)     8020 2023-05-08 20:41:24.000000 ax-platform-0.3.2/scripts/make_tutorials.py
--rw-r--r--   0 runner    (1001) docker     (123)     3195 2023-05-08 20:41:24.000000 ax-platform-0.3.2/scripts/parse_sphinx.py
--rw-r--r--   0 runner    (1001) docker     (123)     1444 2023-05-08 20:41:24.000000 ax-platform-0.3.2/scripts/patch_site_config.py
--rw-r--r--   0 runner    (1001) docker     (123)     8357 2023-05-08 20:41:24.000000 ax-platform-0.3.2/scripts/publish_site.sh
--rw-r--r--   0 runner    (1001) docker     (123)     2477 2023-05-08 20:41:24.000000 ax-platform-0.3.2/scripts/update_versions_html.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     4119 2023-05-08 20:41:24.000000 ax-platform-0.3.2/scripts/validate_sphinx.py
--rw-r--r--   0 runner    (1001) docker     (123)     2981 2023-05-08 20:41:24.000000 ax-platform-0.3.2/scripts/versions.js
--rw-r--r--   0 runner    (1001) docker     (123)      846 2023-05-08 20:41:24.000000 ax-platform-0.3.2/scripts/wheels_build.ps1
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-08 20:45:14.172678 ax-platform-0.3.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     3736 2023-05-08 20:41:24.000000 ax-platform-0.3.2/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 20:45:14.124675 ax-platform-0.3.2/sphinx/
--rw-r--r--   0 runner    (1001) docker     (123)     7466 2023-05-08 20:41:24.000000 ax-platform-0.3.2/sphinx/Makefile
--rw-r--r--   0 runner    (1001) docker     (123)     7442 2023-05-08 20:41:24.000000 ax-platform-0.3.2/sphinx/make.bat
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 20:45:14.132676 ax-platform-0.3.2/sphinx/source/
--rw-r--r--   0 runner    (1001) docker     (123)      151 2023-05-08 20:41:24.000000 ax-platform-0.3.2/sphinx/source/ax.rst
--rw-r--r--   0 runner    (1001) docker     (123)     2860 2023-05-08 20:41:24.000000 ax-platform-0.3.2/sphinx/source/benchmark.rst
--rw-r--r--   0 runner    (1001) docker     (123)     8425 2023-05-08 20:41:24.000000 ax-platform-0.3.2/sphinx/source/conf.py
--rw-r--r--   0 runner    (1001) docker     (123)     3450 2023-05-08 20:41:24.000000 ax-platform-0.3.2/sphinx/source/core.rst
--rw-r--r--   0 runner    (1001) docker     (123)      959 2023-05-08 20:41:24.000000 ax-platform-0.3.2/sphinx/source/early_stopping.rst
--rw-r--r--   0 runner    (1001) docker     (123)      928 2023-05-08 20:41:24.000000 ax-platform-0.3.2/sphinx/source/exceptions.rst
--rw-r--r--   0 runner    (1001) docker     (123)      526 2023-05-08 20:41:24.000000 ax-platform-0.3.2/sphinx/source/global_stopping.rst
--rw-r--r--   0 runner    (1001) docker     (123)      538 2023-05-08 20:41:24.000000 ax-platform-0.3.2/sphinx/source/index.rst
--rw-r--r--   0 runner    (1001) docker     (123)     1941 2023-05-08 20:41:24.000000 ax-platform-0.3.2/sphinx/source/metrics.rst
--rw-r--r--   0 runner    (1001) docker     (123)     9235 2023-05-08 20:41:24.000000 ax-platform-0.3.2/sphinx/source/modelbridge.rst
--rw-r--r--   0 runner    (1001) docker     (123)     7524 2023-05-08 20:41:24.000000 ax-platform-0.3.2/sphinx/source/models.rst
--rw-r--r--   0 runner    (1001) docker     (123)     2252 2023-05-08 20:41:24.000000 ax-platform-0.3.2/sphinx/source/plot.rst
--rw-r--r--   0 runner    (1001) docker     (123)      686 2023-05-08 20:41:24.000000 ax-platform-0.3.2/sphinx/source/runners.rst
--rw-r--r--   0 runner    (1001) docker     (123)     1601 2023-05-08 20:41:24.000000 ax-platform-0.3.2/sphinx/source/service.rst
--rw-r--r--   0 runner    (1001) docker     (123)     4954 2023-05-08 20:41:24.000000 ax-platform-0.3.2/sphinx/source/storage.rst
--rw-r--r--   0 runner    (1001) docker     (123)      520 2023-05-08 20:41:24.000000 ax-platform-0.3.2/sphinx/source/telemetry.rst
--rw-r--r--   0 runner    (1001) docker     (123)     5837 2023-05-08 20:41:24.000000 ax-platform-0.3.2/sphinx/source/utils.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 20:45:14.148677 ax-platform-0.3.2/tutorials/
--rw-r--r--   0 runner    (1001) docker     (123)    39419 2023-05-08 20:41:24.000000 ax-platform-0.3.2/tutorials/Setup_and_Usage_of_BoTorch_Models_in_Ax.ipynb
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 20:45:14.148677 ax-platform-0.3.2/tutorials/early_stopping/
--rw-r--r--   0 runner    (1001) docker     (123)   224156 2023-05-08 20:41:24.000000 ax-platform-0.3.2/tutorials/early_stopping/early_stopping.ipynb
--rw-r--r--   0 runner    (1001) docker     (123)     5450 2023-05-08 20:41:24.000000 ax-platform-0.3.2/tutorials/early_stopping/mnist_train_nas.py
--rw-r--r--   0 runner    (1001) docker     (123)    20665 2023-05-08 20:41:24.000000 ax-platform-0.3.2/tutorials/factorial.ipynb
--rw-r--r--   0 runner    (1001) docker     (123)    25591 2023-05-08 20:41:24.000000 ax-platform-0.3.2/tutorials/generation_strategy.ipynb
--rw-r--r--   0 runner    (1001) docker     (123)    24090 2023-05-08 20:41:24.000000 ax-platform-0.3.2/tutorials/gpei_hartmann_developer.ipynb
--rw-r--r--   0 runner    (1001) docker     (123)   273139 2023-05-08 20:41:24.000000 ax-platform-0.3.2/tutorials/gpei_hartmann_loop.ipynb
--rw-r--r--   0 runner    (1001) docker     (123)    17887 2023-05-08 20:41:24.000000 ax-platform-0.3.2/tutorials/gpei_hartmann_service.ipynb
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 20:45:14.160678 ax-platform-0.3.2/tutorials/human_in_the_loop/
--rw-r--r--   0 runner    (1001) docker     (123)    16283 2023-05-08 20:41:24.000000 ax-platform-0.3.2/tutorials/human_in_the_loop/hitl_data.json
--rw-r--r--   0 runner    (1001) docker     (123)   634579 2023-05-08 20:41:24.000000 ax-platform-0.3.2/tutorials/human_in_the_loop/hitl_exp.json
--rw-r--r--   0 runner    (1001) docker     (123)   276956 2023-05-08 20:41:24.000000 ax-platform-0.3.2/tutorials/human_in_the_loop/human_in_the_loop.ipynb
--rw-r--r--   0 runner    (1001) docker     (123)    51566 2023-05-08 20:41:24.000000 ax-platform-0.3.2/tutorials/modular_botax.ipynb
--rw-r--r--   0 runner    (1001) docker     (123)    19346 2023-05-08 20:41:24.000000 ax-platform-0.3.2/tutorials/multi_task.ipynb
--rw-r--r--   0 runner    (1001) docker     (123)   462391 2023-05-08 20:41:24.000000 ax-platform-0.3.2/tutorials/multiobjective_optimization.ipynb
--rw-r--r--   0 runner    (1001) docker     (123)    10408 2023-05-08 20:41:24.000000 ax-platform-0.3.2/tutorials/raytune_pytorch_cnn.ipynb
--rw-r--r--   0 runner    (1001) docker     (123)    63574 2023-05-08 20:41:24.000000 ax-platform-0.3.2/tutorials/saasbo.ipynb
--rw-r--r--   0 runner    (1001) docker     (123)    22246 2023-05-08 20:41:24.000000 ax-platform-0.3.2/tutorials/saasbo_nehvi.ipynb
--rw-r--r--   0 runner    (1001) docker     (123)   286300 2023-05-08 20:41:24.000000 ax-platform-0.3.2/tutorials/scheduler.ipynb
--rw-r--r--   0 runner    (1001) docker     (123)   138095 2023-05-08 20:41:24.000000 ax-platform-0.3.2/tutorials/tune_cnn.ipynb
--rw-r--r--   0 runner    (1001) docker     (123)    10235 2023-05-08 20:41:24.000000 ax-platform-0.3.2/tutorials/visualizations.ipynb
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 20:45:14.160678 ax-platform-0.3.2/website/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 20:45:14.160678 ax-platform-0.3.2/website/core/
--rw-r--r--   0 runner    (1001) docker     (123)     1880 2023-05-08 20:41:24.000000 ax-platform-0.3.2/website/core/Footer.js
--rw-r--r--   0 runner    (1001) docker     (123)     4320 2023-05-08 20:41:24.000000 ax-platform-0.3.2/website/core/Tutorial.js
--rw-r--r--   0 runner    (1001) docker     (123)     2238 2023-05-08 20:41:24.000000 ax-platform-0.3.2/website/core/TutorialSidebar.js
--rw-r--r--   0 runner    (1001) docker     (123)      375 2023-05-08 20:41:24.000000 ax-platform-0.3.2/website/package.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 20:45:13.860656 ax-platform-0.3.2/website/pages/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 20:45:14.164678 ax-platform-0.3.2/website/pages/en/
--rw-r--r--   0 runner    (1001) docker     (123)     6646 2023-05-08 20:41:24.000000 ax-platform-0.3.2/website/pages/en/index.js
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 20:45:14.164678 ax-platform-0.3.2/website/pages/tutorials/
--rw-r--r--   0 runner    (1001) docker     (123)     6809 2023-05-08 20:41:24.000000 ax-platform-0.3.2/website/pages/tutorials/index.js
--rw-r--r--   0 runner    (1001) docker     (123)      233 2023-05-08 20:41:24.000000 ax-platform-0.3.2/website/sidebars.json
--rw-r--r--   0 runner    (1001) docker     (123)     2740 2023-05-08 20:41:24.000000 ax-platform-0.3.2/website/siteConfig.js
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 20:45:14.164678 ax-platform-0.3.2/website/static/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-08 20:41:24.000000 ax-platform-0.3.2/website/static/.nojekyll
--rw-r--r--   0 runner    (1001) docker     (123)        7 2023-05-08 20:41:24.000000 ax-platform-0.3.2/website/static/CNAME
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 20:45:14.164678 ax-platform-0.3.2/website/static/css/
--rw-r--r--   0 runner    (1001) docker     (123)    10913 2023-05-08 20:41:24.000000 ax-platform-0.3.2/website/static/css/base_sphinx.css
--rw-r--r--   0 runner    (1001) docker     (123)     4960 2023-05-08 20:41:24.000000 ax-platform-0.3.2/website/static/css/custom.css
--rw-r--r--   0 runner    (1001) docker     (123)    15413 2023-05-08 20:41:24.000000 ax-platform-0.3.2/website/static/css/custom_sphinx.css
--rw-r--r--   0 runner    (1001) docker     (123)     4315 2023-05-08 20:41:24.000000 ax-platform-0.3.2/website/static/css/pygments.css
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 20:45:14.168678 ax-platform-0.3.2/website/static/img/
--rw-r--r--   0 runner    (1001) docker     (123)     1981 2023-05-08 20:41:24.000000 ax-platform-0.3.2/website/static/img/ax.svg
--rw-r--r--   0 runner    (1001) docker     (123)     2230 2023-05-08 20:41:24.000000 ax-platform-0.3.2/website/static/img/ax_lockup.svg
--rw-r--r--   0 runner    (1001) docker     (123)     2244 2023-05-08 20:41:24.000000 ax-platform-0.3.2/website/static/img/ax_lockup_white.svg
--rw-r--r--   0 runner    (1001) docker     (123)     2230 2023-05-08 20:41:24.000000 ax-platform-0.3.2/website/static/img/ax_logo_lockup.svg
--rw-r--r--   0 runner    (1001) docker     (123)      369 2023-05-08 20:41:24.000000 ax-platform-0.3.2/website/static/img/ax_wireframe.svg
--rw-r--r--   0 runner    (1001) docker     (123)      785 2023-05-08 20:41:24.000000 ax-platform-0.3.2/website/static/img/database-solid.svg
--rw-r--r--   0 runner    (1001) docker     (123)     1360 2023-05-08 20:41:24.000000 ax-platform-0.3.2/website/static/img/dice-solid.svg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 20:45:14.168678 ax-platform-0.3.2/website/static/img/favicon/
--rw-r--r--   0 runner    (1001) docker     (123)     9662 2023-05-08 20:41:24.000000 ax-platform-0.3.2/website/static/img/favicon/favicon.ico
--rw-r--r--   0 runner    (1001) docker     (123)     2731 2023-05-08 20:41:24.000000 ax-platform-0.3.2/website/static/img/favicon.png
--rw-r--r--   0 runner    (1001) docker     (123)     4370 2023-05-08 20:41:24.000000 ax-platform-0.3.2/website/static/img/oss_logo.png
--rw-r--r--   0 runner    (1001) docker     (123)      910 2023-05-08 20:41:24.000000 ax-platform-0.3.2/website/static/img/th-large-solid.svg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 20:45:14.172678 ax-platform-0.3.2/website/static/js/
--rw-r--r--   0 runner    (1001) docker     (123)      716 2023-05-08 20:41:24.000000 ax-platform-0.3.2/website/static/js/mathjax.js
--rw-r--r--   0 runner    (1001) docker     (123)     1491 2023-05-08 20:41:24.000000 ax-platform-0.3.2/website/static/js/plotUtils.js
--rw-r--r--   0 runner    (1001) docker     (123)     1609 2023-05-08 20:41:24.000000 ax-platform-0.3.2/website/tutorials.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 20:45:14.172678 ax-platform-0.3.2/website/versioned_docs/
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-08 20:41:24.000000 ax-platform-0.3.2/website/versioned_docs/.gitkeep
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 20:45:14.172678 ax-platform-0.3.2/website/versioned_sidebars/
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-08 20:41:24.000000 ax-platform-0.3.2/website/versioned_sidebars/.gitkeep
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 21:06:04.689276 ax-platform-0.3.3/
+-rw-r--r--   0 runner    (1001) docker     (123)      407 2023-06-26 21:02:24.000000 ax-platform-0.3.3/.flake8
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 21:06:04.377255 ax-platform-0.3.3/.github/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 21:06:04.389255 ax-platform-0.3.3/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)     2401 2023-06-26 21:02:24.000000 ax-platform-0.3.3/.github/workflows/build-and-test.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     3968 2023-06-26 21:02:24.000000 ax-platform-0.3.3/.github/workflows/cron.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     2639 2023-06-26 21:02:24.000000 ax-platform-0.3.3/.github/workflows/deploy.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      847 2023-06-26 21:02:24.000000 ax-platform-0.3.3/.github/workflows/reusable_tutorials.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      354 2023-06-26 21:02:24.000000 ax-platform-0.3.3/.github/workflows/tutorials.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     2058 2023-06-26 21:02:24.000000 ax-platform-0.3.3/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)      106 2023-06-26 21:02:24.000000 ax-platform-0.3.3/CHANGELOG.md
+-rw-r--r--   0 runner    (1001) docker     (123)     3355 2023-06-26 21:02:24.000000 ax-platform-0.3.3/CODE_OF_CONDUCT.md
+-rw-r--r--   0 runner    (1001) docker     (123)     5500 2023-06-26 21:02:24.000000 ax-platform-0.3.3/CONTRIBUTING.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1088 2023-06-26 21:02:24.000000 ax-platform-0.3.3/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     9979 2023-06-26 21:06:04.689276 ax-platform-0.3.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     7877 2023-06-26 21:02:24.000000 ax-platform-0.3.3/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 21:06:04.389255 ax-platform-0.3.3/ax/
+-rw-r--r--   0 runner    (1001) docker     (123)     1393 2023-06-26 21:02:24.000000 ax-platform-0.3.3/ax/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      207 2023-06-26 21:02:24.000000 ax-platform-0.3.3/ax/__version__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 21:06:04.389255 ax-platform-0.3.3/ax/benchmark/
+-rw-r--r--   0 runner    (1001) docker     (123)      202 2023-06-26 21:02:24.000000 ax-platform-0.3.3/ax/benchmark/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5310 2023-06-26 21:02:24.000000 ax-platform-0.3.3/ax/benchmark/benchmark.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1440 2023-06-26 21:02:24.000000 ax-platform-0.3.3/ax/benchmark/benchmark_method.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8726 2023-06-26 21:02:24.000000 ax-platform-0.3.3/ax/benchmark/benchmark_problem.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3594 2023-06-26 21:02:24.000000 ax-platform-0.3.3/ax/benchmark/benchmark_result.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 21:06:04.393256 ax-platform-0.3.3/ax/benchmark/methods/
+-rw-r--r--   0 runner    (1001) docker     (123)      179 2023-06-26 21:02:24.000000 ax-platform-0.3.3/ax/benchmark/methods/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      934 2023-06-26 21:02:24.000000 ax-platform-0.3.3/ax/benchmark/methods/choose_generation_strategy.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1594 2023-06-26 21:02:24.000000 ax-platform-0.3.3/ax/benchmark/methods/gpei_and_moo.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7190 2023-06-26 21:02:24.000000 ax-platform-0.3.3/ax/benchmark/methods/modular_botorch.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1647 2023-06-26 21:02:24.000000 ax-platform-0.3.3/ax/benchmark/methods/saasbo.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 21:06:04.393256 ax-platform-0.3.3/ax/benchmark/problems/
+-rw-r--r--   0 runner    (1001) docker     (123)      179 2023-06-26 21:02:24.000000 ax-platform-0.3.3/ax/benchmark/problems/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2027 2023-06-26 21:02:24.000000 ax-platform-0.3.3/ax/benchmark/problems/hd_embedding.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 21:06:04.393256 ax-platform-0.3.3/ax/benchmark/problems/hpo/
+-rw-r--r--   0 runner    (1001) docker     (123)      179 2023-06-26 21:02:24.000000 ax-platform-0.3.3/ax/benchmark/problems/hpo/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7815 2023-06-26 21:02:24.000000 ax-platform-0.3.3/ax/benchmark/problems/hpo/pytorch_cnn.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3762 2023-06-26 21:02:24.000000 ax-platform-0.3.3/ax/benchmark/problems/hpo/torchvision.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8375 2023-06-26 21:02:24.000000 ax-platform-0.3.3/ax/benchmark/problems/registry.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8401 2023-06-26 21:02:24.000000 ax-platform-0.3.3/ax/benchmark/problems/surrogate.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 21:06:04.393256 ax-platform-0.3.3/ax/benchmark/problems/synthetic/
+-rw-r--r--   0 runner    (1001) docker     (123)      179 2023-06-26 21:02:24.000000 ax-platform-0.3.3/ax/benchmark/problems/synthetic/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 21:06:04.397256 ax-platform-0.3.3/ax/benchmark/problems/synthetic/discretized/
+-rw-r--r--   0 runner    (1001) docker     (123)      179 2023-06-26 21:02:24.000000 ax-platform-0.3.3/ax/benchmark/problems/synthetic/discretized/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5634 2023-06-26 21:02:24.000000 ax-platform-0.3.3/ax/benchmark/problems/synthetic/discretized/mixed_integer.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 21:06:04.397256 ax-platform-0.3.3/ax/benchmark/problems/synthetic/hss/
+-rw-r--r--   0 runner    (1001) docker     (123)      179 2023-06-26 21:02:24.000000 ax-platform-0.3.3/ax/benchmark/problems/synthetic/hss/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2451 2023-06-26 21:02:24.000000 ax-platform-0.3.3/ax/benchmark/problems/synthetic/hss/jenatton.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 21:06:04.401256 ax-platform-0.3.3/ax/benchmark/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)      202 2023-06-26 21:02:24.000000 ax-platform-0.3.3/ax/benchmark/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4760 2023-06-26 21:02:24.000000 ax-platform-0.3.3/ax/benchmark/tests/test_benchmark.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1065 2023-06-26 21:02:24.000000 ax-platform-0.3.3/ax/benchmark/tests/test_benchmark_method.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3649 2023-06-26 21:02:24.000000 ax-platform-0.3.3/ax/benchmark/tests/test_benchmark_problem.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1951 2023-06-26 21:02:24.000000 ax-platform-0.3.3/ax/benchmark/tests/test_methods.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4493 2023-06-26 21:02:24.000000 ax-platform-0.3.3/ax/benchmark/tests/test_mixed_integer_problems.py
+-rw-r--r--   0 runner    (1001) docker     (123)      869 2023-06-26 21:02:24.000000 ax-platform-0.3.3/ax/benchmark/tests/test_problem_storage.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1487 2023-06-26 21:02:24.000000 ax-platform-0.3.3/ax/benchmark/tests/test_problems.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2603 2023-06-26 21:02:24.000000 ax-platform-0.3.3/ax/benchmark/tests/test_surrogate_runner.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 21:06:04.413257 ax-platform-0.3.3/ax/core/
+-rw-r--r--   0 runner    (1001) docker     (123)     1883 2023-06-26 21:02:24.000000 ax-platform-0.3.3/ax/core/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4629 2023-06-26 21:02:24.000000 ax-platform-0.3.3/ax/core/arm.py
+-rw-r--r--   0 runner    (1001) docker     (123)    32199 2023-06-26 21:02:24.000000 ax-platform-0.3.3/ax/core/base_trial.py
+-rw-r--r--   0 runner    (1001) docker     (123)    27441 2023-06-26 21:02:24.000000 ax-platform-0.3.3/ax/core/batch_trial.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21717 2023-06-26 21:02:24.000000 ax-platform-0.3.3/ax/core/data.py
+-rw-r--r--   0 runner    (1001) docker     (123)    63234 2023-06-26 21:02:24.000000 ax-platform-0.3.3/ax/core/experiment.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5088 2023-06-26 21:02:24.000000 ax-platform-0.3.3/ax/core/formatting_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15255 2023-06-26 21:02:24.000000 ax-platform-0.3.3/ax/core/generator_run.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16558 2023-06-26 21:02:24.000000 ax-platform-0.3.3/ax/core/map_data.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1156 2023-06-26 21:02:24.000000 ax-platform-0.3.3/ax/core/map_metric.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19322 2023-06-26 21:02:24.000000 ax-platform-0.3.3/ax/core/metric.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10616 2023-06-26 21:02:24.000000 ax-platform-0.3.3/ax/core/multi_type_experiment.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8264 2023-06-26 21:02:24.000000 ax-platform-0.3.3/ax/core/objective.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20542 2023-06-26 21:02:24.000000 ax-platform-0.3.3/ax/core/observation.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19264 2023-06-26 21:02:24.000000 ax-platform-0.3.3/ax/core/optimization_config.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10024 2023-06-26 21:02:24.000000 ax-platform-0.3.3/ax/core/outcome_constraint.py
+-rw-r--r--   0 runner    (1001) docker     (123)    25791 2023-06-26 21:02:24.000000 ax-platform-0.3.3/ax/core/parameter.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10253 2023-06-26 21:02:24.000000 ax-platform-0.3.3/ax/core/parameter_constraint.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5723 2023-06-26 21:02:24.000000 ax-platform-0.3.3/ax/core/parameter_distribution.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2270 2023-06-26 21:02:24.000000 ax-platform-0.3.3/ax/core/risk_measures.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5664 2023-06-26 21:02:24.000000 ax-platform-0.3.3/ax/core/runner.py
+-rw-r--r--   0 runner    (1001) docker     (123)    45576 2023-06-26 21:02:24.000000 ax-platform-0.3.3/ax/core/search_space.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 21:06:04.425258 ax-platform-0.3.3/ax/core/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)      202 2023-06-26 21:02:24.000000 ax-platform-0.3.3/ax/core/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2434 2023-06-26 21:02:24.000000 ax-platform-0.3.3/ax/core/tests/test_arm.py
+-rw-r--r--   0 runner    (1001) docker     (123)    30540 2023-06-26 21:02:24.000000 ax-platform-0.3.3/ax/core/tests/test_batch_trial.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12917 2023-06-26 21:02:24.000000 ax-platform-0.3.3/ax/core/tests/test_data.py
+-rw-r--r--   0 runner    (1001) docker     (123)    49318 2023-06-26 21:02:24.000000 ax-platform-0.3.3/ax/core/tests/test_experiment.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3942 2023-06-26 21:02:24.000000 ax-platform-0.3.3/ax/core/tests/test_formatting_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7352 2023-06-26 21:02:24.000000 ax-platform-0.3.3/ax/core/tests/test_generator_run.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12229 2023-06-26 21:02:24.000000 ax-platform-0.3.3/ax/core/tests/test_map_data.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1875 2023-06-26 21:02:24.000000 ax-platform-0.3.3/ax/core/tests/test_map_metric.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3256 2023-06-26 21:02:24.000000 ax-platform-0.3.3/ax/core/tests/test_metric.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5328 2023-06-26 21:02:24.000000 ax-platform-0.3.3/ax/core/tests/test_multi_type_experiment.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5451 2023-06-26 21:02:24.000000 ax-platform-0.3.3/ax/core/tests/test_objective.py
+-rw-r--r--   0 runner    (1001) docker     (123)    31569 2023-06-26 21:02:24.000000 ax-platform-0.3.3/ax/core/tests/test_observation.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22183 2023-06-26 21:02:24.000000 ax-platform-0.3.3/ax/core/tests/test_optimization_config.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8604 2023-06-26 21:02:24.000000 ax-platform-0.3.3/ax/core/tests/test_outcome_constraint.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18129 2023-06-26 21:02:24.000000 ax-platform-0.3.3/ax/core/tests/test_parameter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8345 2023-06-26 21:02:24.000000 ax-platform-0.3.3/ax/core/tests/test_parameter_constraint.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2888 2023-06-26 21:02:24.000000 ax-platform-0.3.3/ax/core/tests/test_parameter_distribution.py
+-rw-r--r--   0 runner    (1001) docker     (123)      885 2023-06-26 21:02:24.000000 ax-platform-0.3.3/ax/core/tests/test_risk_measures.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2027 2023-06-26 21:02:24.000000 ax-platform-0.3.3/ax/core/tests/test_runner.py
+-rw-r--r--   0 runner    (1001) docker     (123)    44614 2023-06-26 21:02:24.000000 ax-platform-0.3.3/ax/core/tests/test_search_space.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10538 2023-06-26 21:02:24.000000 ax-platform-0.3.3/ax/core/tests/test_trial.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3157 2023-06-26 21:02:24.000000 ax-platform-0.3.3/ax/core/tests/test_types.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6914 2023-06-26 21:02:24.000000 ax-platform-0.3.3/ax/core/tests/test_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12074 2023-06-26 21:02:24.000000 ax-platform-0.3.3/ax/core/trial.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7150 2023-06-26 21:02:24.000000 ax-platform-0.3.3/ax/core/types.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6975 2023-06-26 21:02:24.000000 ax-platform-0.3.3/ax/core/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 21:06:04.425258 ax-platform-0.3.3/ax/early_stopping/
+-rw-r--r--   0 runner    (1001) docker     (123)      271 2023-06-26 21:02:24.000000 ax-platform-0.3.3/ax/early_stopping/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 21:06:04.429258 ax-platform-0.3.3/ax/early_stopping/strategies/
+-rw-r--r--   0 runner    (1001) docker     (123)      961 2023-06-26 21:02:24.000000 ax-platform-0.3.3/ax/early_stopping/strategies/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    24312 2023-06-26 21:02:24.000000 ax-platform-0.3.3/ax/early_stopping/strategies/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2552 2023-06-26 21:02:24.000000 ax-platform-0.3.3/ax/early_stopping/strategies/logical.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10738 2023-06-26 21:02:24.000000 ax-platform-0.3.3/ax/early_stopping/strategies/percentile.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8594 2023-06-26 21:02:24.000000 ax-platform-0.3.3/ax/early_stopping/strategies/threshold.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 21:06:04.429258 ax-platform-0.3.3/ax/early_stopping/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)      202 2023-06-26 21:02:24.000000 ax-platform-0.3.3/ax/early_stopping/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    31888 2023-06-26 21:02:24.000000 ax-platform-0.3.3/ax/early_stopping/tests/test_strategies.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4977 2023-06-26 21:02:24.000000 ax-platform-0.3.3/ax/early_stopping/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 21:06:04.433258 ax-platform-0.3.3/ax/exceptions/
+-rw-r--r--   0 runner    (1001) docker     (123)      202 2023-06-26 21:02:24.000000 ax-platform-0.3.3/ax/exceptions/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      891 2023-06-26 21:02:24.000000 ax-platform-0.3.3/ax/exceptions/constants.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4940 2023-06-26 21:02:24.000000 ax-platform-0.3.3/ax/exceptions/core.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1650 2023-06-26 21:02:24.000000 ax-platform-0.3.3/ax/exceptions/data_provider.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1569 2023-06-26 21:02:24.000000 ax-platform-0.3.3/ax/exceptions/generation_strategy.py
+-rw-r--r--   0 runner    (1001) docker     (123)      480 2023-06-26 21:02:24.000000 ax-platform-0.3.3/ax/exceptions/model.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1082 2023-06-26 21:02:24.000000 ax-platform-0.3.3/ax/exceptions/storage.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 21:06:04.433258 ax-platform-0.3.3/ax/global_stopping/
+-rw-r--r--   0 runner    (1001) docker     (123)      272 2023-06-26 21:02:24.000000 ax-platform-0.3.3/ax/global_stopping/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 21:06:04.433258 ax-platform-0.3.3/ax/global_stopping/strategies/
+-rw-r--r--   0 runner    (1001) docker     (123)      456 2023-06-26 21:02:24.000000 ax-platform-0.3.3/ax/global_stopping/strategies/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3067 2023-06-26 21:02:24.000000 ax-platform-0.3.3/ax/global_stopping/strategies/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13811 2023-06-26 21:02:24.000000 ax-platform-0.3.3/ax/global_stopping/strategies/improvement.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 21:06:04.433258 ax-platform-0.3.3/ax/global_stopping/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)      202 2023-06-26 21:02:24.000000 ax-platform-0.3.3/ax/global_stopping/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13851 2023-06-26 21:02:24.000000 ax-platform-0.3.3/ax/global_stopping/tests/tests_strategies.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 21:06:04.441259 ax-platform-0.3.3/ax/metrics/
+-rw-r--r--   0 runner    (1001) docker     (123)      511 2023-06-26 21:02:24.000000 ax-platform-0.3.3/ax/metrics/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2190 2023-06-26 21:02:24.000000 ax-platform-0.3.3/ax/metrics/botorch_test_problem.py
+-rw-r--r--   0 runner    (1001) docker     (123)      840 2023-06-26 21:02:24.000000 ax-platform-0.3.3/ax/metrics/branin.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5649 2023-06-26 21:02:24.000000 ax-platform-0.3.3/ax/metrics/branin_map.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4692 2023-06-26 21:02:24.000000 ax-platform-0.3.3/ax/metrics/chemistry.py
+-rw-r--r--   0 runner    (1001) docker     (123)    31150 2023-06-26 21:02:24.000000 ax-platform-0.3.3/ax/metrics/chemistry_data.zip
+-rw-r--r--   0 runner    (1001) docker     (123)    20145 2023-06-26 21:02:24.000000 ax-platform-0.3.3/ax/metrics/curve.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3897 2023-06-26 21:02:24.000000 ax-platform-0.3.3/ax/metrics/dict_lookup.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4602 2023-06-26 21:02:24.000000 ax-platform-0.3.3/ax/metrics/factorial.py
+-rw-r--r--   0 runner    (1001) docker     (123)      694 2023-06-26 21:02:24.000000 ax-platform-0.3.3/ax/metrics/hartmann6.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2176 2023-06-26 21:02:24.000000 ax-platform-0.3.3/ax/metrics/jenatton.py
+-rw-r--r--   0 runner    (1001) docker     (123)      401 2023-06-26 21:02:24.000000 ax-platform-0.3.3/ax/metrics/l2norm.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5196 2023-06-26 21:02:24.000000 ax-platform-0.3.3/ax/metrics/noisy_function.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3968 2023-06-26 21:02:24.000000 ax-platform-0.3.3/ax/metrics/noisy_function_map.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6708 2023-06-26 21:02:24.000000 ax-platform-0.3.3/ax/metrics/sklearn.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4835 2023-06-26 21:02:24.000000 ax-platform-0.3.3/ax/metrics/tensorboard.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 21:06:04.441259 ax-platform-0.3.3/ax/metrics/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)      202 2023-06-26 21:02:24.000000 ax-platform-0.3.3/ax/metrics/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3652 2023-06-26 21:02:24.000000 ax-platform-0.3.3/ax/metrics/tests/test_chemistry.py
+-rw-r--r--   0 runner    (1001) docker     (123)      640 2023-06-26 21:02:24.000000 ax-platform-0.3.3/ax/metrics/tests/test_curve.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2620 2023-06-26 21:02:24.000000 ax-platform-0.3.3/ax/metrics/tests/test_dict_lookup.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2617 2023-06-26 21:02:24.000000 ax-platform-0.3.3/ax/metrics/tests/test_noisy_function.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4367 2023-06-26 21:02:24.000000 ax-platform-0.3.3/ax/metrics/tests/test_sklearn.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7279 2023-06-26 21:02:24.000000 ax-platform-0.3.3/ax/metrics/tests/test_tensorboard.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2679 2023-06-26 21:02:24.000000 ax-platform-0.3.3/ax/metrics/torchx.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 21:06:04.449259 ax-platform-0.3.3/ax/modelbridge/
+-rw-r--r--   0 runner    (1001) docker     (123)      772 2023-06-26 21:02:24.000000 ax-platform-0.3.3/ax/modelbridge/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    49292 2023-06-26 21:02:24.000000 ax-platform-0.3.3/ax/modelbridge/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1603 2023-06-26 21:02:24.000000 ax-platform-0.3.3/ax/modelbridge/completion_criterion.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15838 2023-06-26 21:02:24.000000 ax-platform-0.3.3/ax/modelbridge/cross_validation.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9872 2023-06-26 21:02:24.000000 ax-platform-0.3.3/ax/modelbridge/discrete.py
+-rw-r--r--   0 runner    (1001) docker     (123)    28288 2023-06-26 21:02:24.000000 ax-platform-0.3.3/ax/modelbridge/dispatch_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)    24504 2023-06-26 21:02:24.000000 ax-platform-0.3.3/ax/modelbridge/factory.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19309 2023-06-26 21:02:24.000000 ax-platform-0.3.3/ax/modelbridge/generation_node.py
+-rw-r--r--   0 runner    (1001) docker     (123)    40066 2023-06-26 21:02:24.000000 ax-platform-0.3.3/ax/modelbridge/generation_strategy.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17579 2023-06-26 21:02:24.000000 ax-platform-0.3.3/ax/modelbridge/map_torch.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13878 2023-06-26 21:02:24.000000 ax-platform-0.3.3/ax/modelbridge/model_spec.py
+-rw-r--r--   0 runner    (1001) docker     (123)    58407 2023-06-26 21:02:24.000000 ax-platform-0.3.3/ax/modelbridge/modelbridge_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4409 2023-06-26 21:02:24.000000 ax-platform-0.3.3/ax/modelbridge/pairwise.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3421 2023-06-26 21:02:24.000000 ax-platform-0.3.3/ax/modelbridge/prediction_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4103 2023-06-26 21:02:24.000000 ax-platform-0.3.3/ax/modelbridge/random.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21913 2023-06-26 21:02:24.000000 ax-platform-0.3.3/ax/modelbridge/registry.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 21:06:04.453260 ax-platform-0.3.3/ax/modelbridge/strategies/
+-rw-r--r--   0 runner    (1001) docker     (123)      202 2023-06-26 21:02:24.000000 ax-platform-0.3.3/ax/modelbridge/strategies/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4582 2023-06-26 21:02:24.000000 ax-platform-0.3.3/ax/modelbridge/strategies/alebo.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10030 2023-06-26 21:02:24.000000 ax-platform-0.3.3/ax/modelbridge/strategies/rembo.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 21:06:04.477261 ax-platform-0.3.3/ax/modelbridge/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)      202 2023-06-26 21:02:24.000000 ax-platform-0.3.3/ax/modelbridge/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2807 2023-06-26 21:02:24.000000 ax-platform-0.3.3/ax/modelbridge/tests/test_alebo_strategy.py
+-rw-r--r--   0 runner    (1001) docker     (123)    32245 2023-06-26 21:02:24.000000 ax-platform-0.3.3/ax/modelbridge/tests/test_base_modelbridge.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2236 2023-06-26 21:02:24.000000 ax-platform-0.3.3/ax/modelbridge/tests/test_base_transform.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2340 2023-06-26 21:02:24.000000 ax-platform-0.3.3/ax/modelbridge/tests/test_cap_parameter_transform.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8209 2023-06-26 21:02:24.000000 ax-platform-0.3.3/ax/modelbridge/tests/test_cast_transform.py
+-rw-r--r--   0 runner    (1001) docker     (123)      593 2023-06-26 21:02:24.000000 ax-platform-0.3.3/ax/modelbridge/tests/test_centered_unit_x_transform.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10982 2023-06-26 21:02:24.000000 ax-platform-0.3.3/ax/modelbridge/tests/test_choice_encode_transform.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4751 2023-06-26 21:02:24.000000 ax-platform-0.3.3/ax/modelbridge/tests/test_completion_criterion.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4059 2023-06-26 21:02:24.000000 ax-platform-0.3.3/ax/modelbridge/tests/test_convert_metric_names.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14248 2023-06-26 21:02:24.000000 ax-platform-0.3.3/ax/modelbridge/tests/test_cross_validation.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11305 2023-06-26 21:02:24.000000 ax-platform-0.3.3/ax/modelbridge/tests/test_derelativize_transform.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11824 2023-06-26 21:02:24.000000 ax-platform-0.3.3/ax/modelbridge/tests/test_discrete_modelbridge.py
+-rw-r--r--   0 runner    (1001) docker     (123)    33932 2023-06-26 21:02:24.000000 ax-platform-0.3.3/ax/modelbridge/tests/test_dispatch_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22595 2023-06-26 21:02:24.000000 ax-platform-0.3.3/ax/modelbridge/tests/test_factory.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10464 2023-06-26 21:02:24.000000 ax-platform-0.3.3/ax/modelbridge/tests/test_generation_node.py
+-rw-r--r--   0 runner    (1001) docker     (123)    36153 2023-06-26 21:02:24.000000 ax-platform-0.3.3/ax/modelbridge/tests/test_generation_strategy.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7123 2023-06-26 21:02:24.000000 ax-platform-0.3.3/ax/modelbridge/tests/test_int_range_to_choice_transform.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13466 2023-06-26 21:02:24.000000 ax-platform-0.3.3/ax/modelbridge/tests/test_int_to_float_transform.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2600 2023-06-26 21:02:24.000000 ax-platform-0.3.3/ax/modelbridge/tests/test_inverse_gaussian_cdf_y.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4386 2023-06-26 21:02:24.000000 ax-platform-0.3.3/ax/modelbridge/tests/test_ivw_transform.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4010 2023-06-26 21:02:24.000000 ax-platform-0.3.3/ax/modelbridge/tests/test_log_transform.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10890 2023-06-26 21:02:24.000000 ax-platform-0.3.3/ax/modelbridge/tests/test_log_y_transform.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5587 2023-06-26 21:02:24.000000 ax-platform-0.3.3/ax/modelbridge/tests/test_logit_transform.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5704 2023-06-26 21:02:24.000000 ax-platform-0.3.3/ax/modelbridge/tests/test_map_torch_modelbridge.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4511 2023-06-26 21:02:24.000000 ax-platform-0.3.3/ax/modelbridge/tests/test_map_unit_x_transform.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6338 2023-06-26 21:02:24.000000 ax-platform-0.3.3/ax/modelbridge/tests/test_merge_repeated_measurements_transform.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5101 2023-06-26 21:02:24.000000 ax-platform-0.3.3/ax/modelbridge/tests/test_metrics_as_task_transform.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3261 2023-06-26 21:02:24.000000 ax-platform-0.3.3/ax/modelbridge/tests/test_model_fit_metrics.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6723 2023-06-26 21:02:24.000000 ax-platform-0.3.3/ax/modelbridge/tests/test_model_spec.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10369 2023-06-26 21:02:24.000000 ax-platform-0.3.3/ax/modelbridge/tests/test_modelbridge_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7739 2023-06-26 21:02:24.000000 ax-platform-0.3.3/ax/modelbridge/tests/test_one_hot_transform.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4896 2023-06-26 21:02:24.000000 ax-platform-0.3.3/ax/modelbridge/tests/test_pairwise_modelbridge.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4963 2023-06-26 21:02:24.000000 ax-platform-0.3.3/ax/modelbridge/tests/test_percentile_y_transform.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15128 2023-06-26 21:02:24.000000 ax-platform-0.3.3/ax/modelbridge/tests/test_power_transform_y.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5127 2023-06-26 21:02:24.000000 ax-platform-0.3.3/ax/modelbridge/tests/test_prediction_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6752 2023-06-26 21:02:24.000000 ax-platform-0.3.3/ax/modelbridge/tests/test_random_modelbridge.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20119 2023-06-26 21:02:24.000000 ax-platform-0.3.3/ax/modelbridge/tests/test_registry.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14157 2023-06-26 21:02:24.000000 ax-platform-0.3.3/ax/modelbridge/tests/test_relativize_transform.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5022 2023-06-26 21:02:24.000000 ax-platform-0.3.3/ax/modelbridge/tests/test_rembo_strategy.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4303 2023-06-26 21:02:24.000000 ax-platform-0.3.3/ax/modelbridge/tests/test_remove_fixed_transform.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4592 2023-06-26 21:02:24.000000 ax-platform-0.3.3/ax/modelbridge/tests/test_robust.py
+-rw-r--r--   0 runner    (1001) docker     (123)      952 2023-06-26 21:02:24.000000 ax-platform-0.3.3/ax/modelbridge/tests/test_rounding.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5358 2023-06-26 21:02:24.000000 ax-platform-0.3.3/ax/modelbridge/tests/test_search_space_to_choice_transform.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2193 2023-06-26 21:02:24.000000 ax-platform-0.3.3/ax/modelbridge/tests/test_search_space_to_float_transform.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6044 2023-06-26 21:02:24.000000 ax-platform-0.3.3/ax/modelbridge/tests/test_standardize_y_transform.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8992 2023-06-26 21:02:24.000000 ax-platform-0.3.3/ax/modelbridge/tests/test_stratified_standardize_y.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5681 2023-06-26 21:02:24.000000 ax-platform-0.3.3/ax/modelbridge/tests/test_task_encode_transform.py
+-rw-r--r--   0 runner    (1001) docker     (123)    29980 2023-06-26 21:02:24.000000 ax-platform-0.3.3/ax/modelbridge/tests/test_torch_modelbridge.py
+-rw-r--r--   0 runner    (1001) docker     (123)    33129 2023-06-26 21:02:24.000000 ax-platform-0.3.3/ax/modelbridge/tests/test_torch_modelbridge_moo.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3194 2023-06-26 21:02:24.000000 ax-platform-0.3.3/ax/modelbridge/tests/test_transform_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6410 2023-06-26 21:02:24.000000 ax-platform-0.3.3/ax/modelbridge/tests/test_trial_as_task_transform.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10996 2023-06-26 21:02:24.000000 ax-platform-0.3.3/ax/modelbridge/tests/test_unit_x_transform.py
+-rw-r--r--   0 runner    (1001) docker     (123)    26757 2023-06-26 21:02:24.000000 ax-platform-0.3.3/ax/modelbridge/tests/test_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)    29964 2023-06-26 21:02:24.000000 ax-platform-0.3.3/ax/modelbridge/tests/test_winsorize_transform.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8282 2023-06-26 21:02:24.000000 ax-platform-0.3.3/ax/modelbridge/tests/test_winsorize_transform_legacy.py
+-rw-r--r--   0 runner    (1001) docker     (123)    40950 2023-06-26 21:02:24.000000 ax-platform-0.3.3/ax/modelbridge/torch.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 21:06:04.489262 ax-platform-0.3.3/ax/modelbridge/transforms/
+-rw-r--r--   0 runner    (1001) docker     (123)      202 2023-06-26 21:02:24.000000 ax-platform-0.3.3/ax/modelbridge/transforms/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9830 2023-06-26 21:02:24.000000 ax-platform-0.3.3/ax/modelbridge/transforms/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2125 2023-06-26 21:02:24.000000 ax-platform-0.3.3/ax/modelbridge/transforms/cap_parameter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5137 2023-06-26 21:02:24.000000 ax-platform-0.3.3/ax/modelbridge/transforms/cast.py
+-rw-r--r--   0 runner    (1001) docker     (123)      463 2023-06-26 21:02:24.000000 ax-platform-0.3.3/ax/modelbridge/transforms/centered_unit_x.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9272 2023-06-26 21:02:24.000000 ax-platform-0.3.3/ax/modelbridge/transforms/choice_encode.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6049 2023-06-26 21:02:24.000000 ax-platform-0.3.3/ax/modelbridge/transforms/convert_metric_names.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4952 2023-06-26 21:02:24.000000 ax-platform-0.3.3/ax/modelbridge/transforms/derelativize.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3310 2023-06-26 21:02:24.000000 ax-platform-0.3.3/ax/modelbridge/transforms/int_range_to_choice.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7500 2023-06-26 21:02:24.000000 ax-platform-0.3.3/ax/modelbridge/transforms/int_to_float.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2535 2023-06-26 21:02:24.000000 ax-platform-0.3.3/ax/modelbridge/transforms/inverse_gaussian_cdf_y.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5265 2023-06-26 21:02:24.000000 ax-platform-0.3.3/ax/modelbridge/transforms/ivw.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3245 2023-06-26 21:02:24.000000 ax-platform-0.3.3/ax/modelbridge/transforms/log.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7978 2023-06-26 21:02:24.000000 ax-platform-0.3.3/ax/modelbridge/transforms/log_y.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2974 2023-06-26 21:02:24.000000 ax-platform-0.3.3/ax/modelbridge/transforms/logit.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3477 2023-06-26 21:02:24.000000 ax-platform-0.3.3/ax/modelbridge/transforms/map_unit_x.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5362 2023-06-26 21:02:24.000000 ax-platform-0.3.3/ax/modelbridge/transforms/merge_repeated_measurements.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5841 2023-06-26 21:02:24.000000 ax-platform-0.3.3/ax/modelbridge/transforms/metrics_as_task.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7819 2023-06-26 21:02:24.000000 ax-platform-0.3.3/ax/modelbridge/transforms/one_hot.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4149 2023-06-26 21:02:24.000000 ax-platform-0.3.3/ax/modelbridge/transforms/percentile_y.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9196 2023-06-26 21:02:24.000000 ax-platform-0.3.3/ax/modelbridge/transforms/power_transform_y.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8163 2023-06-26 21:02:24.000000 ax-platform-0.3.3/ax/modelbridge/transforms/relativize.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3637 2023-06-26 21:02:24.000000 ax-platform-0.3.3/ax/modelbridge/transforms/remove_fixed.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2335 2023-06-26 21:02:24.000000 ax-platform-0.3.3/ax/modelbridge/transforms/rounding.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3923 2023-06-26 21:02:24.000000 ax-platform-0.3.3/ax/modelbridge/transforms/search_space_to_choice.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1588 2023-06-26 21:02:24.000000 ax-platform-0.3.3/ax/modelbridge/transforms/search_space_to_float.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7298 2023-06-26 21:02:24.000000 ax-platform-0.3.3/ax/modelbridge/transforms/standardize_y.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7571 2023-06-26 21:02:24.000000 ax-platform-0.3.3/ax/modelbridge/transforms/stratified_standardize_y.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3965 2023-06-26 21:02:24.000000 ax-platform-0.3.3/ax/modelbridge/transforms/task_encode.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6336 2023-06-26 21:02:24.000000 ax-platform-0.3.3/ax/modelbridge/transforms/trial_as_task.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10934 2023-06-26 21:02:24.000000 ax-platform-0.3.3/ax/modelbridge/transforms/unit_x.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6008 2023-06-26 21:02:24.000000 ax-platform-0.3.3/ax/modelbridge/transforms/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21307 2023-06-26 21:02:24.000000 ax-platform-0.3.3/ax/modelbridge/transforms/winsorize.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 21:06:04.489262 ax-platform-0.3.3/ax/models/
+-rw-r--r--   0 runner    (1001) docker     (123)      202 2023-06-26 21:02:24.000000 ax-platform-0.3.3/ax/models/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2601 2023-06-26 21:02:24.000000 ax-platform-0.3.3/ax/models/base.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 21:06:04.493262 ax-platform-0.3.3/ax/models/discrete/
+-rw-r--r--   0 runner    (1001) docker     (123)      202 2023-06-26 21:02:24.000000 ax-platform-0.3.3/ax/models/discrete/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1753 2023-06-26 21:02:24.000000 ax-platform-0.3.3/ax/models/discrete/eb_thompson.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2980 2023-06-26 21:02:24.000000 ax-platform-0.3.3/ax/models/discrete/full_factorial.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11208 2023-06-26 21:02:24.000000 ax-platform-0.3.3/ax/models/discrete/thompson.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5699 2023-06-26 21:02:24.000000 ax-platform-0.3.3/ax/models/discrete_base.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22672 2023-06-26 21:02:24.000000 ax-platform-0.3.3/ax/models/model_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 21:06:04.493262 ax-platform-0.3.3/ax/models/random/
+-rw-r--r--   0 runner    (1001) docker     (123)      202 2023-06-26 21:02:24.000000 ax-platform-0.3.3/ax/models/random/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3598 2023-06-26 21:02:24.000000 ax-platform-0.3.3/ax/models/random/alebo_initializer.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11659 2023-06-26 21:02:24.000000 ax-platform-0.3.3/ax/models/random/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2567 2023-06-26 21:02:24.000000 ax-platform-0.3.3/ax/models/random/rembo_initializer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6195 2023-06-26 21:02:24.000000 ax-platform-0.3.3/ax/models/random/sobol.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1551 2023-06-26 21:02:24.000000 ax-platform-0.3.3/ax/models/random/uniform.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 21:06:04.509263 ax-platform-0.3.3/ax/models/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)      202 2023-06-26 21:02:24.000000 ax-platform-0.3.3/ax/models/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14772 2023-06-26 21:02:24.000000 ax-platform-0.3.3/ax/models/tests/test_alebo.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1057 2023-06-26 21:02:24.000000 ax-platform-0.3.3/ax/models/tests/test_alebo_initializer.py
+-rw-r--r--   0 runner    (1001) docker     (123)      773 2023-06-26 21:02:24.000000 ax-platform-0.3.3/ax/models/tests/test_base.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18114 2023-06-26 21:02:24.000000 ax-platform-0.3.3/ax/models/tests/test_botorch_defaults.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17944 2023-06-26 21:02:24.000000 ax-platform-0.3.3/ax/models/tests/test_botorch_kg.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13434 2023-06-26 21:02:24.000000 ax-platform-0.3.3/ax/models/tests/test_botorch_mes.py
+-rw-r--r--   0 runner    (1001) docker     (123)    30863 2023-06-26 21:02:24.000000 ax-platform-0.3.3/ax/models/tests/test_botorch_model.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20926 2023-06-26 21:02:24.000000 ax-platform-0.3.3/ax/models/tests/test_botorch_moo_defaults.py
+-rw-r--r--   0 runner    (1001) docker     (123)    33596 2023-06-26 21:02:24.000000 ax-platform-0.3.3/ax/models/tests/test_botorch_moo_model.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3947 2023-06-26 21:02:24.000000 ax-platform-0.3.3/ax/models/tests/test_cbo_lcea.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2638 2023-06-26 21:02:24.000000 ax-platform-0.3.3/ax/models/tests/test_cbo_lcem.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3712 2023-06-26 21:02:24.000000 ax-platform-0.3.3/ax/models/tests/test_cbo_sac.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1760 2023-06-26 21:02:24.000000 ax-platform-0.3.3/ax/models/tests/test_discrete.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7743 2023-06-26 21:02:24.000000 ax-platform-0.3.3/ax/models/tests/test_eb_thompson.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3062 2023-06-26 21:02:24.000000 ax-platform-0.3.3/ax/models/tests/test_full_factorial.py
+-rw-r--r--   0 runner    (1001) docker     (123)    49865 2023-06-26 21:02:24.000000 ax-platform-0.3.3/ax/models/tests/test_fully_bayesian.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7163 2023-06-26 21:02:24.000000 ax-platform-0.3.3/ax/models/tests/test_model_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4777 2023-06-26 21:02:24.000000 ax-platform-0.3.3/ax/models/tests/test_posterior_mean.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3458 2023-06-26 21:02:24.000000 ax-platform-0.3.3/ax/models/tests/test_random.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1654 2023-06-26 21:02:24.000000 ax-platform-0.3.3/ax/models/tests/test_randomforest.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5470 2023-06-26 21:02:24.000000 ax-platform-0.3.3/ax/models/tests/test_rembo.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1185 2023-06-26 21:02:24.000000 ax-platform-0.3.3/ax/models/tests/test_rembo_initializer.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12435 2023-06-26 21:02:24.000000 ax-platform-0.3.3/ax/models/tests/test_sobol.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13220 2023-06-26 21:02:24.000000 ax-platform-0.3.3/ax/models/tests/test_thompson.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2613 2023-06-26 21:02:24.000000 ax-platform-0.3.3/ax/models/tests/test_torch.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8406 2023-06-26 21:02:24.000000 ax-platform-0.3.3/ax/models/tests/test_torch_model_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9238 2023-06-26 21:02:24.000000 ax-platform-0.3.3/ax/models/tests/test_torch_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6722 2023-06-26 21:02:24.000000 ax-platform-0.3.3/ax/models/tests/test_uniform.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 21:06:04.513264 ax-platform-0.3.3/ax/models/torch/
+-rw-r--r--   0 runner    (1001) docker     (123)      202 2023-06-26 21:02:24.000000 ax-platform-0.3.3/ax/models/torch/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    29766 2023-06-26 21:02:24.000000 ax-platform-0.3.3/ax/models/torch/alebo.py
+-rw-r--r--   0 runner    (1001) docker     (123)    24182 2023-06-26 21:02:24.000000 ax-platform-0.3.3/ax/models/torch/botorch.py
+-rw-r--r--   0 runner    (1001) docker     (123)    31561 2023-06-26 21:02:24.000000 ax-platform-0.3.3/ax/models/torch/botorch_defaults.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15542 2023-06-26 21:02:24.000000 ax-platform-0.3.3/ax/models/torch/botorch_kg.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10264 2023-06-26 21:02:24.000000 ax-platform-0.3.3/ax/models/torch/botorch_mes.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 21:06:04.521264 ax-platform-0.3.3/ax/models/torch/botorch_modular/
+-rw-r--r--   0 runner    (1001) docker     (123)      202 2023-06-26 21:02:24.000000 ax-platform-0.3.3/ax/models/torch/botorch_modular/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    25780 2023-06-26 21:02:24.000000 ax-platform-0.3.3/ax/models/torch/botorch_modular/acquisition.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 21:06:04.521264 ax-platform-0.3.3/ax/models/torch/botorch_modular/input_constructors/
+-rw-r--r--   0 runner    (1001) docker     (123)      202 2023-06-26 21:02:24.000000 ax-platform-0.3.3/ax/models/torch/botorch_modular/input_constructors/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4898 2023-06-26 21:02:24.000000 ax-platform-0.3.3/ax/models/torch/botorch_modular/input_constructors/covar_modules.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1825 2023-06-26 21:02:24.000000 ax-platform-0.3.3/ax/models/torch/botorch_modular/kernels.py
+-rw-r--r--   0 runner    (1001) docker     (123)      488 2023-06-26 21:02:24.000000 ax-platform-0.3.3/ax/models/torch/botorch_modular/list_surrogate.py
+-rw-r--r--   0 runner    (1001) docker     (123)    28867 2023-06-26 21:02:24.000000 ax-platform-0.3.3/ax/models/torch/botorch_modular/model.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3751 2023-06-26 21:02:24.000000 ax-platform-0.3.3/ax/models/torch/botorch_modular/multi_fidelity.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6223 2023-06-26 21:02:24.000000 ax-platform-0.3.3/ax/models/torch/botorch_modular/optimizer_argparse.py
+-rw-r--r--   0 runner    (1001) docker     (123)    36129 2023-06-26 21:02:24.000000 ax-platform-0.3.3/ax/models/torch/botorch_modular/surrogate.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14652 2023-06-26 21:02:24.000000 ax-platform-0.3.3/ax/models/torch/botorch_modular/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15753 2023-06-26 21:02:24.000000 ax-platform-0.3.3/ax/models/torch/botorch_moo.py
+-rw-r--r--   0 runner    (1001) docker     (123)    23861 2023-06-26 21:02:24.000000 ax-platform-0.3.3/ax/models/torch/botorch_moo_defaults.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7547 2023-06-26 21:02:24.000000 ax-platform-0.3.3/ax/models/torch/cbo_lcea.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3549 2023-06-26 21:02:24.000000 ax-platform-0.3.3/ax/models/torch/cbo_lcem.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4438 2023-06-26 21:02:24.000000 ax-platform-0.3.3/ax/models/torch/cbo_sac.py
+-rw-r--r--   0 runner    (1001) docker     (123)      510 2023-06-26 21:02:24.000000 ax-platform-0.3.3/ax/models/torch/frontier_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)    24477 2023-06-26 21:02:24.000000 ax-platform-0.3.3/ax/models/torch/fully_bayesian.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7511 2023-06-26 21:02:24.000000 ax-platform-0.3.3/ax/models/torch/fully_bayesian_model_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3531 2023-06-26 21:02:24.000000 ax-platform-0.3.3/ax/models/torch/posterior_mean.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4628 2023-06-26 21:02:24.000000 ax-platform-0.3.3/ax/models/torch/randomforest.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9745 2023-06-26 21:02:24.000000 ax-platform-0.3.3/ax/models/torch/rembo.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 21:06:04.525264 ax-platform-0.3.3/ax/models/torch/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)      202 2023-06-26 21:02:24.000000 ax-platform-0.3.3/ax/models/torch/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    28354 2023-06-26 21:02:24.000000 ax-platform-0.3.3/ax/models/torch/tests/test_acquisition.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4620 2023-06-26 21:02:24.000000 ax-platform-0.3.3/ax/models/torch/tests/test_covar_modules_argparse.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1412 2023-06-26 21:02:24.000000 ax-platform-0.3.3/ax/models/torch/tests/test_kernels.py
+-rw-r--r--   0 runner    (1001) docker     (123)    39724 2023-06-26 21:02:24.000000 ax-platform-0.3.3/ax/models/torch/tests/test_model.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7248 2023-06-26 21:02:24.000000 ax-platform-0.3.3/ax/models/torch/tests/test_multi_fidelity.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5899 2023-06-26 21:02:24.000000 ax-platform-0.3.3/ax/models/torch/tests/test_optimizer_argparse.py
+-rw-r--r--   0 runner    (1001) docker     (123)    53294 2023-06-26 21:02:24.000000 ax-platform-0.3.3/ax/models/torch/tests/test_surrogate.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19896 2023-06-26 21:02:24.000000 ax-platform-0.3.3/ax/models/torch/tests/test_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)    26784 2023-06-26 21:02:24.000000 ax-platform-0.3.3/ax/models/torch/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10947 2023-06-26 21:02:24.000000 ax-platform-0.3.3/ax/models/torch_base.py
+-rw-r--r--   0 runner    (1001) docker     (123)      625 2023-06-26 21:02:24.000000 ax-platform-0.3.3/ax/models/types.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1452 2023-06-26 21:02:24.000000 ax-platform-0.3.3/ax/models/winsorization_config.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 21:06:04.533265 ax-platform-0.3.3/ax/plot/
+-rw-r--r--   0 runner    (1001) docker     (123)      202 2023-06-26 21:02:24.000000 ax-platform-0.3.3/ax/plot/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2464 2023-06-26 21:02:24.000000 ax-platform-0.3.3/ax/plot/bandit_rollout.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2444 2023-06-26 21:02:24.000000 ax-platform-0.3.3/ax/plot/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2718 2023-06-26 21:02:24.000000 ax-platform-0.3.3/ax/plot/color.py
+-rw-r--r--   0 runner    (1001) docker     (123)    32766 2023-06-26 21:02:24.000000 ax-platform-0.3.3/ax/plot/contour.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 21:06:04.533265 ax-platform-0.3.3/ax/plot/css/
+-rw-r--r--   0 runner    (1001) docker     (123)      202 2023-06-26 21:02:24.000000 ax-platform-0.3.3/ax/plot/css/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      992 2023-06-26 21:02:24.000000 ax-platform-0.3.3/ax/plot/css/base.css
+-rw-r--r--   0 runner    (1001) docker     (123)    24550 2023-06-26 21:02:24.000000 ax-platform-0.3.3/ax/plot/diagnostic.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9969 2023-06-26 21:02:24.000000 ax-platform-0.3.3/ax/plot/feature_importances.py
+-rw-r--r--   0 runner    (1001) docker     (123)    31776 2023-06-26 21:02:24.000000 ax-platform-0.3.3/ax/plot/helper.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 21:06:04.533265 ax-platform-0.3.3/ax/plot/js/
+-rw-r--r--   0 runner    (1001) docker     (123)      202 2023-06-26 21:02:24.000000 ax-platform-0.3.3/ax/plot/js/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 21:06:04.537265 ax-platform-0.3.3/ax/plot/js/common/
+-rw-r--r--   0 runner    (1001) docker     (123)      202 2023-06-26 21:02:24.000000 ax-platform-0.3.3/ax/plot/js/common/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      344 2023-06-26 21:02:24.000000 ax-platform-0.3.3/ax/plot/js/common/css.js
+-rw-r--r--   0 runner    (1001) docker     (123)     5344 2023-06-26 21:02:24.000000 ax-platform-0.3.3/ax/plot/js/common/helpers.js
+-rw-r--r--   0 runner    (1001) docker     (123)      369 2023-06-26 21:02:24.000000 ax-platform-0.3.3/ax/plot/js/common/plotly_offline.js
+-rw-r--r--   0 runner    (1001) docker     (123)      385 2023-06-26 21:02:24.000000 ax-platform-0.3.3/ax/plot/js/common/plotly_online.js
+-rw-r--r--   0 runner    (1001) docker     (123)      342 2023-06-26 21:02:24.000000 ax-platform-0.3.3/ax/plot/js/common/plotly_requires.js
+-rw-r--r--   0 runner    (1001) docker     (123)      269 2023-06-26 21:02:24.000000 ax-platform-0.3.3/ax/plot/js/generic_plotly.js
+-rw-r--r--   0 runner    (1001) docker     (123)     2383 2023-06-26 21:02:24.000000 ax-platform-0.3.3/ax/plot/marginal_effects.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3159 2023-06-26 21:02:24.000000 ax-platform-0.3.3/ax/plot/parallel_coordinates.py
+-rw-r--r--   0 runner    (1001) docker     (123)    38724 2023-06-26 21:02:24.000000 ax-platform-0.3.3/ax/plot/pareto_frontier.py
+-rw-r--r--   0 runner    (1001) docker     (123)    26242 2023-06-26 21:02:24.000000 ax-platform-0.3.3/ax/plot/pareto_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4362 2023-06-26 21:02:24.000000 ax-platform-0.3.3/ax/plot/render.py
+-rw-r--r--   0 runner    (1001) docker     (123)    58188 2023-06-26 21:02:24.000000 ax-platform-0.3.3/ax/plot/scatter.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19873 2023-06-26 21:02:24.000000 ax-platform-0.3.3/ax/plot/slice.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5646 2023-06-26 21:02:24.000000 ax-platform-0.3.3/ax/plot/table_view.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 21:06:04.541266 ax-platform-0.3.3/ax/plot/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)      202 2023-06-26 21:02:24.000000 ax-platform-0.3.3/ax/plot/tests/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 21:06:04.541266 ax-platform-0.3.3/ax/plot/tests/long_running/
+-rw-r--r--   0 runner    (1001) docker     (123)     2339 2023-06-26 21:02:24.000000 ax-platform-0.3.3/ax/plot/tests/long_running/test_pareto_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2160 2023-06-26 21:02:24.000000 ax-platform-0.3.3/ax/plot/tests/test_contours.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2125 2023-06-26 21:02:24.000000 ax-platform-0.3.3/ax/plot/tests/test_diagnostic.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4372 2023-06-26 21:02:24.000000 ax-platform-0.3.3/ax/plot/tests/test_feature_importances.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1609 2023-06-26 21:02:24.000000 ax-platform-0.3.3/ax/plot/tests/test_fitted_scatter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1291 2023-06-26 21:02:24.000000 ax-platform-0.3.3/ax/plot/tests/test_helper.py
+-rw-r--r--   0 runner    (1001) docker     (123)      822 2023-06-26 21:02:24.000000 ax-platform-0.3.3/ax/plot/tests/test_parallel_coordinates.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14241 2023-06-26 21:02:24.000000 ax-platform-0.3.3/ax/plot/tests/test_pareto_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1552 2023-06-26 21:02:24.000000 ax-platform-0.3.3/ax/plot/tests/test_slices.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4752 2023-06-26 21:02:24.000000 ax-platform-0.3.3/ax/plot/tests/test_tile_fitted.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2563 2023-06-26 21:02:24.000000 ax-platform-0.3.3/ax/plot/tests/test_traces.py
+-rw-r--r--   0 runner    (1001) docker     (123)    27668 2023-06-26 21:02:24.000000 ax-platform-0.3.3/ax/plot/trace.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 21:06:04.541266 ax-platform-0.3.3/ax/runners/
+-rw-r--r--   0 runner    (1001) docker     (123)      394 2023-06-26 21:02:24.000000 ax-platform-0.3.3/ax/runners/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5514 2023-06-26 21:02:24.000000 ax-platform-0.3.3/ax/runners/botorch_test_problem.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3386 2023-06-26 21:02:24.000000 ax-platform-0.3.3/ax/runners/simulated_backend.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1220 2023-06-26 21:02:24.000000 ax-platform-0.3.3/ax/runners/synthetic.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 21:06:04.545266 ax-platform-0.3.3/ax/runners/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)      202 2023-06-26 21:02:24.000000 ax-platform-0.3.3/ax/runners/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6264 2023-06-26 21:02:24.000000 ax-platform-0.3.3/ax/runners/tests/test_torchx.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6993 2023-06-26 21:02:24.000000 ax-platform-0.3.3/ax/runners/torchx.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 21:06:04.545266 ax-platform-0.3.3/ax/service/
+-rw-r--r--   0 runner    (1001) docker     (123)      311 2023-06-26 21:02:24.000000 ax-platform-0.3.3/ax/service/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    78508 2023-06-26 21:02:24.000000 ax-platform-0.3.3/ax/service/ax_client.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7891 2023-06-26 21:02:24.000000 ax-platform-0.3.3/ax/service/interactive_loop.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11683 2023-06-26 21:02:24.000000 ax-platform-0.3.3/ax/service/managed_loop.py
+-rw-r--r--   0 runner    (1001) docker     (123)    78162 2023-06-26 21:02:24.000000 ax-platform-0.3.3/ax/service/scheduler.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 21:06:04.553266 ax-platform-0.3.3/ax/service/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)      202 2023-06-26 21:02:24.000000 ax-platform-0.3.3/ax/service/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)   119430 2023-06-26 21:02:24.000000 ax-platform-0.3.3/ax/service/tests/test_ax_client.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4650 2023-06-26 21:02:24.000000 ax-platform-0.3.3/ax/service/tests/test_best_point.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21148 2023-06-26 21:02:24.000000 ax-platform-0.3.3/ax/service/tests/test_best_point_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1668 2023-06-26 21:02:24.000000 ax-platform-0.3.3/ax/service/tests/test_early_stopping.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5335 2023-06-26 21:02:24.000000 ax-platform-0.3.3/ax/service/tests/test_global_stopping.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12675 2023-06-26 21:02:24.000000 ax-platform-0.3.3/ax/service/tests/test_instantiation_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3457 2023-06-26 21:02:24.000000 ax-platform-0.3.3/ax/service/tests/test_interactive_loop.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20401 2023-06-26 21:02:24.000000 ax-platform-0.3.3/ax/service/tests/test_managed_loop.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19334 2023-06-26 21:02:24.000000 ax-platform-0.3.3/ax/service/tests/test_report_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)    54710 2023-06-26 21:02:24.000000 ax-platform-0.3.3/ax/service/tests/test_scheduler.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14129 2023-06-26 21:02:24.000000 ax-platform-0.3.3/ax/service/tests/test_with_db_settings_base.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 21:06:04.557267 ax-platform-0.3.3/ax/service/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)      202 2023-06-26 21:02:24.000000 ax-platform-0.3.3/ax/service/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    34580 2023-06-26 21:02:24.000000 ax-platform-0.3.3/ax/service/utils/best_point.py
+-rw-r--r--   0 runner    (1001) docker     (123)    25699 2023-06-26 21:02:24.000000 ax-platform-0.3.3/ax/service/utils/best_point_mixin.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1916 2023-06-26 21:02:24.000000 ax-platform-0.3.3/ax/service/utils/early_stopping.py
+-rw-r--r--   0 runner    (1001) docker     (123)    38477 2023-06-26 21:02:24.000000 ax-platform-0.3.3/ax/service/utils/instantiation.py
+-rw-r--r--   0 runner    (1001) docker     (123)    42771 2023-06-26 21:02:24.000000 ax-platform-0.3.3/ax/service/utils/report_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6625 2023-06-26 21:02:24.000000 ax-platform-0.3.3/ax/service/utils/scheduler_options.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21704 2023-06-26 21:02:24.000000 ax-platform-0.3.3/ax/service/utils/with_db_settings_base.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 21:06:04.561267 ax-platform-0.3.3/ax/storage/
+-rw-r--r--   0 runner    (1001) docker     (123)      313 2023-06-26 21:02:24.000000 ax-platform-0.3.3/ax/storage/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7397 2023-06-26 21:02:24.000000 ax-platform-0.3.3/ax/storage/botorch_modular_registry.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 21:06:04.565267 ax-platform-0.3.3/ax/storage/json_store/
+-rw-r--r--   0 runner    (1001) docker     (123)      378 2023-06-26 21:02:24.000000 ax-platform-0.3.3/ax/storage/json_store/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    28491 2023-06-26 21:02:24.000000 ax-platform-0.3.3/ax/storage/json_store/decoder.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10555 2023-06-26 21:02:24.000000 ax-platform-0.3.3/ax/storage/json_store/decoders.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6670 2023-06-26 21:02:24.000000 ax-platform-0.3.3/ax/storage/json_store/encoder.py
+-rw-r--r--   0 runner    (1001) docker     (123)    25060 2023-06-26 21:02:24.000000 ax-platform-0.3.3/ax/storage/json_store/encoders.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1217 2023-06-26 21:02:24.000000 ax-platform-0.3.3/ax/storage/json_store/load.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15396 2023-06-26 21:02:24.000000 ax-platform-0.3.3/ax/storage/json_store/registry.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1743 2023-06-26 21:02:24.000000 ax-platform-0.3.3/ax/storage/json_store/save.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 21:06:04.565267 ax-platform-0.3.3/ax/storage/json_store/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)      202 2023-06-26 21:02:24.000000 ax-platform-0.3.3/ax/storage/json_store/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22778 2023-06-26 21:02:24.000000 ax-platform-0.3.3/ax/storage/json_store/tests/test_json_store.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4675 2023-06-26 21:02:24.000000 ax-platform-0.3.3/ax/storage/metric_registry.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9327 2023-06-26 21:02:24.000000 ax-platform-0.3.3/ax/storage/registry_bundle.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4177 2023-06-26 21:02:24.000000 ax-platform-0.3.3/ax/storage/runner_registry.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 21:06:04.577268 ax-platform-0.3.3/ax/storage/sqa_store/
+-rw-r--r--   0 runner    (1001) docker     (123)      543 2023-06-26 21:02:24.000000 ax-platform-0.3.3/ax/storage/sqa_store/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9573 2023-06-26 21:02:24.000000 ax-platform-0.3.3/ax/storage/sqa_store/db.py
+-rw-r--r--   0 runner    (1001) docker     (123)    49885 2023-06-26 21:02:24.000000 ax-platform-0.3.3/ax/storage/sqa_store/decoder.py
+-rw-r--r--   0 runner    (1001) docker     (123)      620 2023-06-26 21:02:24.000000 ax-platform-0.3.3/ax/storage/sqa_store/delete.py
+-rw-r--r--   0 runner    (1001) docker     (123)    44346 2023-06-26 21:02:24.000000 ax-platform-0.3.3/ax/storage/sqa_store/encoder.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3359 2023-06-26 21:02:24.000000 ax-platform-0.3.3/ax/storage/sqa_store/json.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19755 2023-06-26 21:02:24.000000 ax-platform-0.3.3/ax/storage/sqa_store/load.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1637 2023-06-26 21:02:24.000000 ax-platform-0.3.3/ax/storage/sqa_store/reduced_state.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19930 2023-06-26 21:02:24.000000 ax-platform-0.3.3/ax/storage/sqa_store/save.py
+-rw-r--r--   0 runner    (1001) docker     (123)    25389 2023-06-26 21:02:24.000000 ax-platform-0.3.3/ax/storage/sqa_store/sqa_classes.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4480 2023-06-26 21:02:24.000000 ax-platform-0.3.3/ax/storage/sqa_store/sqa_config.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2456 2023-06-26 21:02:24.000000 ax-platform-0.3.3/ax/storage/sqa_store/sqa_enum.py
+-rw-r--r--   0 runner    (1001) docker     (123)      841 2023-06-26 21:02:24.000000 ax-platform-0.3.3/ax/storage/sqa_store/structs.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 21:06:04.581268 ax-platform-0.3.3/ax/storage/sqa_store/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)      202 2023-06-26 21:02:24.000000 ax-platform-0.3.3/ax/storage/sqa_store/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    73084 2023-06-26 21:02:24.000000 ax-platform-0.3.3/ax/storage/sqa_store/tests/test_sqa_store.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4304 2023-06-26 21:02:24.000000 ax-platform-0.3.3/ax/storage/sqa_store/tests/test_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6577 2023-06-26 21:02:24.000000 ax-platform-0.3.3/ax/storage/sqa_store/tests/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)      984 2023-06-26 21:02:24.000000 ax-platform-0.3.3/ax/storage/sqa_store/timestamp.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6376 2023-06-26 21:02:24.000000 ax-platform-0.3.3/ax/storage/sqa_store/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4008 2023-06-26 21:02:24.000000 ax-platform-0.3.3/ax/storage/sqa_store/validation.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 21:06:04.581268 ax-platform-0.3.3/ax/storage/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     1706 2023-06-26 21:02:24.000000 ax-platform-0.3.3/ax/storage/tests/test_registry_bundle.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2980 2023-06-26 21:02:24.000000 ax-platform-0.3.3/ax/storage/transform_registry.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1328 2023-06-26 21:02:24.000000 ax-platform-0.3.3/ax/storage/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 21:06:04.581268 ax-platform-0.3.3/ax/telemetry/
+-rw-r--r--   0 runner    (1001) docker     (123)     4504 2023-06-26 21:02:24.000000 ax-platform-0.3.3/ax/telemetry/ax_client.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2776 2023-06-26 21:02:24.000000 ax-platform-0.3.3/ax/telemetry/common.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10913 2023-06-26 21:02:24.000000 ax-platform-0.3.3/ax/telemetry/experiment.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2355 2023-06-26 21:02:24.000000 ax-platform-0.3.3/ax/telemetry/generation_strategy.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16844 2023-06-26 21:02:24.000000 ax-platform-0.3.3/ax/telemetry/optimization.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5735 2023-06-26 21:02:24.000000 ax-platform-0.3.3/ax/telemetry/scheduler.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 21:06:04.581268 ax-platform-0.3.3/ax/telemetry/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     4800 2023-06-26 21:02:24.000000 ax-platform-0.3.3/ax/telemetry/tests/test_ax_client.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2464 2023-06-26 21:02:24.000000 ax-platform-0.3.3/ax/telemetry/tests/test_experiment.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1015 2023-06-26 21:02:24.000000 ax-platform-0.3.3/ax/telemetry/tests/test_generation_strategy.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5947 2023-06-26 21:02:24.000000 ax-platform-0.3.3/ax/telemetry/tests/test_optimization.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7614 2023-06-26 21:02:24.000000 ax-platform-0.3.3/ax/telemetry/tests/test_scheduler.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 21:06:04.585269 ax-platform-0.3.3/ax/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)      202 2023-06-26 21:02:24.000000 ax-platform-0.3.3/ax/utils/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 21:06:04.589269 ax-platform-0.3.3/ax/utils/common/
+-rw-r--r--   0 runner    (1001) docker     (123)      202 2023-06-26 21:02:24.000000 ax-platform-0.3.3/ax/utils/common/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1586 2023-06-26 21:02:24.000000 ax-platform-0.3.3/ax/utils/common/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2867 2023-06-26 21:02:24.000000 ax-platform-0.3.3/ax/utils/common/constants.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2829 2023-06-26 21:02:24.000000 ax-platform-0.3.3/ax/utils/common/decorator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1631 2023-06-26 21:02:24.000000 ax-platform-0.3.3/ax/utils/common/docutils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8237 2023-06-26 21:02:24.000000 ax-platform-0.3.3/ax/utils/common/equality.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10612 2023-06-26 21:02:24.000000 ax-platform-0.3.3/ax/utils/common/executils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5226 2023-06-26 21:02:24.000000 ax-platform-0.3.3/ax/utils/common/kwargs.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7741 2023-06-26 21:02:24.000000 ax-platform-0.3.3/ax/utils/common/logger.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1110 2023-06-26 21:02:24.000000 ax-platform-0.3.3/ax/utils/common/mock.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6748 2023-06-26 21:02:24.000000 ax-platform-0.3.3/ax/utils/common/result.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5074 2023-06-26 21:02:24.000000 ax-platform-0.3.3/ax/utils/common/serialization.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 21:06:04.593269 ax-platform-0.3.3/ax/utils/common/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)      202 2023-06-26 21:02:24.000000 ax-platform-0.3.3/ax/utils/common/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1187 2023-06-26 21:02:24.000000 ax-platform-0.3.3/ax/utils/common/tests/test_docutils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2666 2023-06-26 21:02:24.000000 ax-platform-0.3.3/ax/utils/common/tests/test_equality.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10218 2023-06-26 21:02:24.000000 ax-platform-0.3.3/ax/utils/common/tests/test_executils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5761 2023-06-26 21:02:24.000000 ax-platform-0.3.3/ax/utils/common/tests/test_kwargutils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2887 2023-06-26 21:02:24.000000 ax-platform-0.3.3/ax/utils/common/tests/test_logger.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2250 2023-06-26 21:02:24.000000 ax-platform-0.3.3/ax/utils/common/tests/test_result.py
+-rw-r--r--   0 runner    (1001) docker     (123)      824 2023-06-26 21:02:24.000000 ax-platform-0.3.3/ax/utils/common/tests/test_serialization.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3393 2023-06-26 21:02:24.000000 ax-platform-0.3.3/ax/utils/common/tests/test_testutils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2070 2023-06-26 21:02:24.000000 ax-platform-0.3.3/ax/utils/common/tests/test_typeutils.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17314 2023-06-26 21:02:24.000000 ax-platform-0.3.3/ax/utils/common/testutils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1405 2023-06-26 21:02:24.000000 ax-platform-0.3.3/ax/utils/common/timeutils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3941 2023-06-26 21:02:24.000000 ax-platform-0.3.3/ax/utils/common/typeutils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1188 2023-06-26 21:02:24.000000 ax-platform-0.3.3/ax/utils/common/typeutils_torch.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 21:06:04.593269 ax-platform-0.3.3/ax/utils/flake8_plugins/
+-rw-r--r--   0 runner    (1001) docker     (123)      202 2023-06-26 21:02:24.000000 ax-platform-0.3.3/ax/utils/flake8_plugins/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3279 2023-06-26 21:02:24.000000 ax-platform-0.3.3/ax/utils/flake8_plugins/docstring_checker.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 21:06:04.597269 ax-platform-0.3.3/ax/utils/measurement/
+-rw-r--r--   0 runner    (1001) docker     (123)      202 2023-06-26 21:02:24.000000 ax-platform-0.3.3/ax/utils/measurement/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11368 2023-06-26 21:02:24.000000 ax-platform-0.3.3/ax/utils/measurement/synthetic_functions.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 21:06:04.597269 ax-platform-0.3.3/ax/utils/measurement/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)      202 2023-06-26 21:02:24.000000 ax-platform-0.3.3/ax/utils/measurement/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6182 2023-06-26 21:02:24.000000 ax-platform-0.3.3/ax/utils/measurement/tests/test_synthetic_functions.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 21:06:04.597269 ax-platform-0.3.3/ax/utils/notebook/
+-rw-r--r--   0 runner    (1001) docker     (123)      202 2023-06-26 21:02:24.000000 ax-platform-0.3.3/ax/utils/notebook/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1408 2023-06-26 21:02:24.000000 ax-platform-0.3.3/ax/utils/notebook/plotting.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 21:06:04.597269 ax-platform-0.3.3/ax/utils/report/
+-rw-r--r--   0 runner    (1001) docker     (123)      202 2023-06-26 21:02:24.000000 ax-platform-0.3.3/ax/utils/report/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4236 2023-06-26 21:02:24.000000 ax-platform-0.3.3/ax/utils/report/render.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 21:06:04.601270 ax-platform-0.3.3/ax/utils/report/resources/
+-rw-r--r--   0 runner    (1001) docker     (123)      202 2023-06-26 21:02:24.000000 ax-platform-0.3.3/ax/utils/report/resources/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1240 2023-06-26 21:02:24.000000 ax-platform-0.3.3/ax/utils/report/resources/base_template.html
+-rw-r--r--   0 runner    (1001) docker     (123)     3150 2023-06-26 21:02:24.000000 ax-platform-0.3.3/ax/utils/report/resources/report.css
+-rw-r--r--   0 runner    (1001) docker     (123)      215 2023-06-26 21:02:24.000000 ax-platform-0.3.3/ax/utils/report/resources/simple_template.html
+-rw-r--r--   0 runner    (1001) docker     (123)      657 2023-06-26 21:02:24.000000 ax-platform-0.3.3/ax/utils/report/resources/sufficient_statistic.html
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 21:06:04.601270 ax-platform-0.3.3/ax/utils/report/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)      202 2023-06-26 21:02:24.000000 ax-platform-0.3.3/ax/utils/report/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1099 2023-06-26 21:02:24.000000 ax-platform-0.3.3/ax/utils/report/tests/test_render.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 21:06:04.601270 ax-platform-0.3.3/ax/utils/sensitivity/
+-rw-r--r--   0 runner    (1001) docker     (123)      202 2023-06-26 21:02:24.000000 ax-platform-0.3.3/ax/utils/sensitivity/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4884 2023-06-26 21:02:24.000000 ax-platform-0.3.3/ax/utils/sensitivity/derivative_gp.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15644 2023-06-26 21:02:24.000000 ax-platform-0.3.3/ax/utils/sensitivity/derivative_measures.py
+-rw-r--r--   0 runner    (1001) docker     (123)    35734 2023-06-26 21:02:24.000000 ax-platform-0.3.3/ax/utils/sensitivity/sobol_measures.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 21:06:04.605270 ax-platform-0.3.3/ax/utils/sensitivity/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)      202 2023-06-26 21:02:24.000000 ax-platform-0.3.3/ax/utils/sensitivity/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14117 2023-06-26 21:02:24.000000 ax-platform-0.3.3/ax/utils/sensitivity/tests/test_sensitivity.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 21:06:04.605270 ax-platform-0.3.3/ax/utils/stats/
+-rw-r--r--   0 runner    (1001) docker     (123)      202 2023-06-26 21:02:24.000000 ax-platform-0.3.3/ax/utils/stats/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6403 2023-06-26 21:02:24.000000 ax-platform-0.3.3/ax/utils/stats/model_fit_stats.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13566 2023-06-26 21:02:24.000000 ax-platform-0.3.3/ax/utils/stats/statstools.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 21:06:04.605270 ax-platform-0.3.3/ax/utils/stats/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)      202 2023-06-26 21:02:24.000000 ax-platform-0.3.3/ax/utils/stats/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4973 2023-06-26 21:02:24.000000 ax-platform-0.3.3/ax/utils/stats/tests/test_statstools.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 21:06:04.609270 ax-platform-0.3.3/ax/utils/testing/
+-rw-r--r--   0 runner    (1001) docker     (123)      202 2023-06-26 21:02:24.000000 ax-platform-0.3.3/ax/utils/testing/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4277 2023-06-26 21:02:24.000000 ax-platform-0.3.3/ax/utils/testing/backend_scheduler.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18626 2023-06-26 21:02:24.000000 ax-platform-0.3.3/ax/utils/testing/backend_simulator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4213 2023-06-26 21:02:24.000000 ax-platform-0.3.3/ax/utils/testing/benchmark_stubs.py
+-rw-r--r--   0 runner    (1001) docker     (123)    65880 2023-06-26 21:02:24.000000 ax-platform-0.3.3/ax/utils/testing/core_stubs.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-26 21:02:24.000000 ax-platform-0.3.3/ax/utils/testing/manifest.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 21:06:04.613270 ax-platform-0.3.3/ax/utils/testing/metrics/
+-rw-r--r--   0 runner    (1001) docker     (123)      202 2023-06-26 21:02:24.000000 ax-platform-0.3.3/ax/utils/testing/metrics/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1649 2023-06-26 21:02:24.000000 ax-platform-0.3.3/ax/utils/testing/metrics/backend_simulator_map.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2432 2023-06-26 21:02:24.000000 ax-platform-0.3.3/ax/utils/testing/metrics/branin_backend_map.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5511 2023-06-26 21:02:24.000000 ax-platform-0.3.3/ax/utils/testing/mock.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12305 2023-06-26 21:02:24.000000 ax-platform-0.3.3/ax/utils/testing/modeling_stubs.py
+-rw-r--r--   0 runner    (1001) docker     (123)      791 2023-06-26 21:02:24.000000 ax-platform-0.3.3/ax/utils/testing/test_init_files.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 21:06:04.613270 ax-platform-0.3.3/ax/utils/testing/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)      202 2023-06-26 21:02:24.000000 ax-platform-0.3.3/ax/utils/testing/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5402 2023-06-26 21:02:24.000000 ax-platform-0.3.3/ax/utils/testing/tests/test_backend_simulator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2012 2023-06-26 21:02:24.000000 ax-platform-0.3.3/ax/utils/testing/tests/test_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1544 2023-06-26 21:02:24.000000 ax-platform-0.3.3/ax/utils/testing/torch_stubs.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1086 2023-06-26 21:02:24.000000 ax-platform-0.3.3/ax/utils/testing/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 21:06:04.613270 ax-platform-0.3.3/ax/utils/tutorials/
+-rw-r--r--   0 runner    (1001) docker     (123)      202 2023-06-26 21:02:24.000000 ax-platform-0.3.3/ax/utils/tutorials/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9247 2023-06-26 21:02:24.000000 ax-platform-0.3.3/ax/utils/tutorials/cnn_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)      160 2023-06-26 21:06:03.000000 ax-platform-0.3.3/ax/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 21:06:04.617271 ax-platform-0.3.3/ax_platform.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     9979 2023-06-26 21:06:04.000000 ax-platform-0.3.3/ax_platform.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    21630 2023-06-26 21:06:04.000000 ax-platform-0.3.3/ax_platform.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-26 21:06:04.000000 ax-platform-0.3.3/ax_platform.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1005 2023-06-26 21:06:04.000000 ax-platform-0.3.3/ax_platform.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        3 2023-06-26 21:06:04.000000 ax-platform-0.3.3/ax_platform.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 21:06:04.621271 ax-platform-0.3.3/docs/
+-rw-r--r--   0 runner    (1001) docker     (123)      145 2023-06-26 21:02:24.000000 ax-platform-0.3.3/docs/algo-overview.md
+-rw-r--r--   0 runner    (1001) docker     (123)     6270 2023-06-26 21:02:24.000000 ax-platform-0.3.3/docs/api.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 21:06:04.637272 ax-platform-0.3.3/docs/assets/
+-rw-r--r--   0 runner    (1001) docker     (123)    81587 2023-06-26 21:02:24.000000 ax-platform-0.3.3/docs/assets/bandit_allocation.png
+-rw-r--r--   0 runner    (1001) docker     (123)   345484 2023-06-26 21:02:24.000000 ax-platform-0.3.3/docs/assets/bo_1d_opt.gif
+-rw-r--r--   0 runner    (1001) docker     (123)   156260 2023-06-26 21:02:24.000000 ax-platform-0.3.3/docs/assets/contour.js
+-rw-r--r--   0 runner    (1001) docker     (123)    14875 2023-06-26 21:02:24.000000 ax-platform-0.3.3/docs/assets/cv.js
+-rw-r--r--   0 runner    (1001) docker     (123)   131612 2023-06-26 21:02:24.000000 ax-platform-0.3.3/docs/assets/example_shrinkage.png
+-rw-r--r--   0 runner    (1001) docker     (123)    13598 2023-06-26 21:02:24.000000 ax-platform-0.3.3/docs/assets/fitted.js
+-rw-r--r--   0 runner    (1001) docker     (123)    65905 2023-06-26 21:02:24.000000 ax-platform-0.3.3/docs/assets/gp_opt.png
+-rw-r--r--   0 runner    (1001) docker     (123)   349223 2023-06-26 21:02:24.000000 ax-platform-0.3.3/docs/assets/gp_posterior.png
+-rw-r--r--   0 runner    (1001) docker     (123)   121838 2023-06-26 21:02:24.000000 ax-platform-0.3.3/docs/assets/mab_animate.gif
+-rw-r--r--   0 runner    (1001) docker     (123)   132372 2023-06-26 21:02:24.000000 ax-platform-0.3.3/docs/assets/mab_probs.png
+-rw-r--r--   0 runner    (1001) docker     (123)   325134 2023-06-26 21:02:24.000000 ax-platform-0.3.3/docs/assets/mab_regret.png
+-rw-r--r--   0 runner    (1001) docker     (123)    26226 2023-06-26 21:02:24.000000 ax-platform-0.3.3/docs/assets/slice.js
+-rw-r--r--   0 runner    (1001) docker     (123)     8863 2023-06-26 21:02:24.000000 ax-platform-0.3.3/docs/banditopt.md
+-rw-r--r--   0 runner    (1001) docker     (123)    10181 2023-06-26 21:02:24.000000 ax-platform-0.3.3/docs/bayesopt.md
+-rw-r--r--   0 runner    (1001) docker     (123)     9871 2023-06-26 21:02:24.000000 ax-platform-0.3.3/docs/core.md
+-rw-r--r--   0 runner    (1001) docker     (123)     2484 2023-06-26 21:02:24.000000 ax-platform-0.3.3/docs/data.md
+-rw-r--r--   0 runner    (1001) docker     (123)     6876 2023-06-26 21:02:24.000000 ax-platform-0.3.3/docs/glossary.md
+-rw-r--r--   0 runner    (1001) docker     (123)     3374 2023-06-26 21:02:24.000000 ax-platform-0.3.3/docs/installation.md
+-rw-r--r--   0 runner    (1001) docker     (123)    22509 2023-06-26 21:02:24.000000 ax-platform-0.3.3/docs/models.md
+-rw-r--r--   0 runner    (1001) docker     (123)     7440 2023-06-26 21:02:24.000000 ax-platform-0.3.3/docs/storage.md
+-rw-r--r--   0 runner    (1001) docker     (123)     7784 2023-06-26 21:02:24.000000 ax-platform-0.3.3/docs/trial-evaluation.md
+-rw-r--r--   0 runner    (1001) docker     (123)     2218 2023-06-26 21:02:24.000000 ax-platform-0.3.3/docs/why-ax.md
+-rw-r--r--   0 runner    (1001) docker     (123)      158 2023-06-26 21:02:24.000000 ax-platform-0.3.3/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      319 2023-06-26 21:02:24.000000 ax-platform-0.3.3/pytest.ini
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 21:06:04.645273 ax-platform-0.3.3/scripts/
+-rwxr-xr-x   0 runner    (1001) docker     (123)      632 2023-06-26 21:02:24.000000 ax-platform-0.3.3/scripts/build_ax.sh
+-rwxr-xr-x   0 runner    (1001) docker     (123)      535 2023-06-26 21:02:24.000000 ax-platform-0.3.3/scripts/docker_install.sh
+-rw-r--r--   0 runner    (1001) docker     (123)      342 2023-06-26 21:02:24.000000 ax-platform-0.3.3/scripts/import_ax.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2263 2023-06-26 21:02:24.000000 ax-platform-0.3.3/scripts/insert_api_refs.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     4160 2023-06-26 21:02:24.000000 ax-platform-0.3.3/scripts/make_docs.sh
+-rw-r--r--   0 runner    (1001) docker     (123)     9398 2023-06-26 21:02:24.000000 ax-platform-0.3.3/scripts/make_tutorials.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3195 2023-06-26 21:02:24.000000 ax-platform-0.3.3/scripts/parse_sphinx.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1444 2023-06-26 21:02:24.000000 ax-platform-0.3.3/scripts/patch_site_config.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8357 2023-06-26 21:02:24.000000 ax-platform-0.3.3/scripts/publish_site.sh
+-rw-r--r--   0 runner    (1001) docker     (123)     2477 2023-06-26 21:02:24.000000 ax-platform-0.3.3/scripts/update_versions_html.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     4119 2023-06-26 21:02:24.000000 ax-platform-0.3.3/scripts/validate_sphinx.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2981 2023-06-26 21:02:24.000000 ax-platform-0.3.3/scripts/versions.js
+-rw-r--r--   0 runner    (1001) docker     (123)      846 2023-06-26 21:02:24.000000 ax-platform-0.3.3/scripts/wheels_build.ps1
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-26 21:06:04.689276 ax-platform-0.3.3/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     3736 2023-06-26 21:02:24.000000 ax-platform-0.3.3/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 21:06:04.645273 ax-platform-0.3.3/sphinx/
+-rw-r--r--   0 runner    (1001) docker     (123)     7466 2023-06-26 21:02:24.000000 ax-platform-0.3.3/sphinx/Makefile
+-rw-r--r--   0 runner    (1001) docker     (123)     7442 2023-06-26 21:02:24.000000 ax-platform-0.3.3/sphinx/make.bat
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 21:06:04.653273 ax-platform-0.3.3/sphinx/source/
+-rw-r--r--   0 runner    (1001) docker     (123)      151 2023-06-26 21:02:24.000000 ax-platform-0.3.3/sphinx/source/ax.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     2860 2023-06-26 21:02:24.000000 ax-platform-0.3.3/sphinx/source/benchmark.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     8425 2023-06-26 21:02:24.000000 ax-platform-0.3.3/sphinx/source/conf.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3450 2023-06-26 21:02:24.000000 ax-platform-0.3.3/sphinx/source/core.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      959 2023-06-26 21:02:24.000000 ax-platform-0.3.3/sphinx/source/early_stopping.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      928 2023-06-26 21:02:24.000000 ax-platform-0.3.3/sphinx/source/exceptions.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      526 2023-06-26 21:02:24.000000 ax-platform-0.3.3/sphinx/source/global_stopping.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      538 2023-06-26 21:02:24.000000 ax-platform-0.3.3/sphinx/source/index.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1941 2023-06-26 21:02:24.000000 ax-platform-0.3.3/sphinx/source/metrics.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     9235 2023-06-26 21:02:24.000000 ax-platform-0.3.3/sphinx/source/modelbridge.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     8010 2023-06-26 21:02:24.000000 ax-platform-0.3.3/sphinx/source/models.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     2252 2023-06-26 21:02:24.000000 ax-platform-0.3.3/sphinx/source/plot.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      686 2023-06-26 21:02:24.000000 ax-platform-0.3.3/sphinx/source/runners.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1601 2023-06-26 21:02:24.000000 ax-platform-0.3.3/sphinx/source/service.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     4954 2023-06-26 21:02:24.000000 ax-platform-0.3.3/sphinx/source/storage.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      520 2023-06-26 21:02:24.000000 ax-platform-0.3.3/sphinx/source/telemetry.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     6001 2023-06-26 21:02:24.000000 ax-platform-0.3.3/sphinx/source/utils.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 21:06:04.669274 ax-platform-0.3.3/tutorials/
+-rw-r--r--   0 runner    (1001) docker     (123)    39419 2023-06-26 21:02:24.000000 ax-platform-0.3.3/tutorials/Setup_and_Usage_of_BoTorch_Models_in_Ax.ipynb
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 21:06:04.669274 ax-platform-0.3.3/tutorials/early_stopping/
+-rw-r--r--   0 runner    (1001) docker     (123)    23921 2023-06-26 21:02:24.000000 ax-platform-0.3.3/tutorials/early_stopping/early_stopping.ipynb
+-rw-r--r--   0 runner    (1001) docker     (123)     5450 2023-06-26 21:02:24.000000 ax-platform-0.3.3/tutorials/early_stopping/mnist_train_nas.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20665 2023-06-26 21:02:24.000000 ax-platform-0.3.3/tutorials/factorial.ipynb
+-rw-r--r--   0 runner    (1001) docker     (123)    25591 2023-06-26 21:02:24.000000 ax-platform-0.3.3/tutorials/generation_strategy.ipynb
+-rw-r--r--   0 runner    (1001) docker     (123)    24090 2023-06-26 21:02:24.000000 ax-platform-0.3.3/tutorials/gpei_hartmann_developer.ipynb
+-rw-r--r--   0 runner    (1001) docker     (123)   273139 2023-06-26 21:02:24.000000 ax-platform-0.3.3/tutorials/gpei_hartmann_loop.ipynb
+-rw-r--r--   0 runner    (1001) docker     (123)    17887 2023-06-26 21:02:24.000000 ax-platform-0.3.3/tutorials/gpei_hartmann_service.ipynb
+-rw-r--r--   0 runner    (1001) docker     (123)    20391 2023-06-26 21:02:24.000000 ax-platform-0.3.3/tutorials/gss.ipynb
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 21:06:04.677275 ax-platform-0.3.3/tutorials/human_in_the_loop/
+-rw-r--r--   0 runner    (1001) docker     (123)    16283 2023-06-26 21:02:24.000000 ax-platform-0.3.3/tutorials/human_in_the_loop/hitl_data.json
+-rw-r--r--   0 runner    (1001) docker     (123)   634579 2023-06-26 21:02:24.000000 ax-platform-0.3.3/tutorials/human_in_the_loop/hitl_exp.json
+-rw-r--r--   0 runner    (1001) docker     (123)   276956 2023-06-26 21:02:24.000000 ax-platform-0.3.3/tutorials/human_in_the_loop/human_in_the_loop.ipynb
+-rw-r--r--   0 runner    (1001) docker     (123)    48123 2023-06-26 21:02:24.000000 ax-platform-0.3.3/tutorials/modular_botax.ipynb
+-rw-r--r--   0 runner    (1001) docker     (123)    19596 2023-06-26 21:02:24.000000 ax-platform-0.3.3/tutorials/multi_task.ipynb
+-rw-r--r--   0 runner    (1001) docker     (123)   462391 2023-06-26 21:02:24.000000 ax-platform-0.3.3/tutorials/multiobjective_optimization.ipynb
+-rw-r--r--   0 runner    (1001) docker     (123)    10560 2023-06-26 21:02:24.000000 ax-platform-0.3.3/tutorials/raytune_pytorch_cnn.ipynb
+-rw-r--r--   0 runner    (1001) docker     (123)    12864 2023-06-26 21:02:24.000000 ax-platform-0.3.3/tutorials/saasbo.ipynb
+-rw-r--r--   0 runner    (1001) docker     (123)    22980 2023-06-26 21:02:24.000000 ax-platform-0.3.3/tutorials/saasbo_nehvi.ipynb
+-rw-r--r--   0 runner    (1001) docker     (123)   287043 2023-06-26 21:02:24.000000 ax-platform-0.3.3/tutorials/scheduler.ipynb
+-rw-r--r--   0 runner    (1001) docker     (123)   138095 2023-06-26 21:02:24.000000 ax-platform-0.3.3/tutorials/tune_cnn.ipynb
+-rw-r--r--   0 runner    (1001) docker     (123)    10235 2023-06-26 21:02:24.000000 ax-platform-0.3.3/tutorials/visualizations.ipynb
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 21:06:04.677275 ax-platform-0.3.3/website/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 21:06:04.677275 ax-platform-0.3.3/website/core/
+-rw-r--r--   0 runner    (1001) docker     (123)     1880 2023-06-26 21:02:24.000000 ax-platform-0.3.3/website/core/Footer.js
+-rw-r--r--   0 runner    (1001) docker     (123)     4320 2023-06-26 21:02:24.000000 ax-platform-0.3.3/website/core/Tutorial.js
+-rw-r--r--   0 runner    (1001) docker     (123)     2238 2023-06-26 21:02:24.000000 ax-platform-0.3.3/website/core/TutorialSidebar.js
+-rw-r--r--   0 runner    (1001) docker     (123)      375 2023-06-26 21:02:24.000000 ax-platform-0.3.3/website/package.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 21:06:04.381255 ax-platform-0.3.3/website/pages/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 21:06:04.681275 ax-platform-0.3.3/website/pages/en/
+-rw-r--r--   0 runner    (1001) docker     (123)     6646 2023-06-26 21:02:24.000000 ax-platform-0.3.3/website/pages/en/index.js
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 21:06:04.681275 ax-platform-0.3.3/website/pages/tutorials/
+-rw-r--r--   0 runner    (1001) docker     (123)     6824 2023-06-26 21:02:24.000000 ax-platform-0.3.3/website/pages/tutorials/index.js
+-rw-r--r--   0 runner    (1001) docker     (123)      233 2023-06-26 21:02:24.000000 ax-platform-0.3.3/website/sidebars.json
+-rw-r--r--   0 runner    (1001) docker     (123)     2740 2023-06-26 21:02:24.000000 ax-platform-0.3.3/website/siteConfig.js
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 21:06:04.681275 ax-platform-0.3.3/website/static/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-26 21:02:24.000000 ax-platform-0.3.3/website/static/.nojekyll
+-rw-r--r--   0 runner    (1001) docker     (123)        7 2023-06-26 21:02:24.000000 ax-platform-0.3.3/website/static/CNAME
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 21:06:04.681275 ax-platform-0.3.3/website/static/css/
+-rw-r--r--   0 runner    (1001) docker     (123)    10913 2023-06-26 21:02:24.000000 ax-platform-0.3.3/website/static/css/base_sphinx.css
+-rw-r--r--   0 runner    (1001) docker     (123)     4960 2023-06-26 21:02:24.000000 ax-platform-0.3.3/website/static/css/custom.css
+-rw-r--r--   0 runner    (1001) docker     (123)    15413 2023-06-26 21:02:24.000000 ax-platform-0.3.3/website/static/css/custom_sphinx.css
+-rw-r--r--   0 runner    (1001) docker     (123)     4315 2023-06-26 21:02:24.000000 ax-platform-0.3.3/website/static/css/pygments.css
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 21:06:04.685275 ax-platform-0.3.3/website/static/img/
+-rw-r--r--   0 runner    (1001) docker     (123)     1981 2023-06-26 21:02:24.000000 ax-platform-0.3.3/website/static/img/ax.svg
+-rw-r--r--   0 runner    (1001) docker     (123)     2230 2023-06-26 21:02:24.000000 ax-platform-0.3.3/website/static/img/ax_lockup.svg
+-rw-r--r--   0 runner    (1001) docker     (123)     2244 2023-06-26 21:02:24.000000 ax-platform-0.3.3/website/static/img/ax_lockup_white.svg
+-rw-r--r--   0 runner    (1001) docker     (123)     2230 2023-06-26 21:02:24.000000 ax-platform-0.3.3/website/static/img/ax_logo_lockup.svg
+-rw-r--r--   0 runner    (1001) docker     (123)      369 2023-06-26 21:02:24.000000 ax-platform-0.3.3/website/static/img/ax_wireframe.svg
+-rw-r--r--   0 runner    (1001) docker     (123)      785 2023-06-26 21:02:24.000000 ax-platform-0.3.3/website/static/img/database-solid.svg
+-rw-r--r--   0 runner    (1001) docker     (123)     1360 2023-06-26 21:02:24.000000 ax-platform-0.3.3/website/static/img/dice-solid.svg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 21:06:04.685275 ax-platform-0.3.3/website/static/img/favicon/
+-rw-r--r--   0 runner    (1001) docker     (123)     9662 2023-06-26 21:02:24.000000 ax-platform-0.3.3/website/static/img/favicon/favicon.ico
+-rw-r--r--   0 runner    (1001) docker     (123)     2731 2023-06-26 21:02:24.000000 ax-platform-0.3.3/website/static/img/favicon.png
+-rw-r--r--   0 runner    (1001) docker     (123)     4370 2023-06-26 21:02:24.000000 ax-platform-0.3.3/website/static/img/oss_logo.png
+-rw-r--r--   0 runner    (1001) docker     (123)      910 2023-06-26 21:02:24.000000 ax-platform-0.3.3/website/static/img/th-large-solid.svg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 21:06:04.685275 ax-platform-0.3.3/website/static/js/
+-rw-r--r--   0 runner    (1001) docker     (123)      716 2023-06-26 21:02:24.000000 ax-platform-0.3.3/website/static/js/mathjax.js
+-rw-r--r--   0 runner    (1001) docker     (123)     1491 2023-06-26 21:02:24.000000 ax-platform-0.3.3/website/static/js/plotUtils.js
+-rw-r--r--   0 runner    (1001) docker     (123)     1708 2023-06-26 21:02:24.000000 ax-platform-0.3.3/website/tutorials.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 21:06:04.685275 ax-platform-0.3.3/website/versioned_docs/
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-26 21:02:24.000000 ax-platform-0.3.3/website/versioned_docs/.gitkeep
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 21:06:04.689276 ax-platform-0.3.3/website/versioned_sidebars/
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-26 21:02:24.000000 ax-platform-0.3.3/website/versioned_sidebars/.gitkeep
```

### Comparing `ax-platform-0.3.2/.github/workflows/build-and-test.yml` & `ax-platform-0.3.3/.github/workflows/build-and-test.yml`

 * *Files identical despite different names*

### Comparing `ax-platform-0.3.2/.github/workflows/cron.yml` & `ax-platform-0.3.3/.github/workflows/cron.yml`

 * *Files 2% similar despite different names*

```diff
@@ -63,14 +63,16 @@
       if: matrix.requirements == 'full'
       run: |
         pytest -ra
 
   build-tutorials-with-pinned-botorch:
     name: Build tutorials with pinned BoTorch
     uses: ./.github/workflows/reusable_tutorials.yml
+    with:
+      smoke_test: false
 
   publish-latest-website:
 
     runs-on: ubuntu-latest
 
     steps:
     - uses: actions/checkout@v2
```

### Comparing `ax-platform-0.3.2/.github/workflows/deploy.yml` & `ax-platform-0.3.3/.github/workflows/deploy.yml`

 * *Files identical despite different names*

### Comparing `ax-platform-0.3.2/.gitignore` & `ax-platform-0.3.3/.gitignore`

 * *Files identical despite different names*

### Comparing `ax-platform-0.3.2/CODE_OF_CONDUCT.md` & `ax-platform-0.3.3/CODE_OF_CONDUCT.md`

 * *Files identical despite different names*

### Comparing `ax-platform-0.3.2/CONTRIBUTING.md` & `ax-platform-0.3.3/CONTRIBUTING.md`

 * *Files identical despite different names*

### Comparing `ax-platform-0.3.2/LICENSE` & `ax-platform-0.3.3/LICENSE`

 * *Files identical despite different names*

### Comparing `ax-platform-0.3.2/PKG-INFO` & `ax-platform-0.3.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ax-platform
-Version: 0.3.2
+Version: 0.3.3
 Summary: Adaptive Experimentation
 Home-page: https://github.com/facebook/Ax
 Author: Facebook, Inc.
 License: MIT
 Description: <img width="300" src="https://ax.dev/img/ax_logo_lockup.svg" alt="Ax Logo" />
         
         <hr/>
@@ -171,15 +171,15 @@
         pip install git+https://github.com/cornellius-gp/linear_operator.git
         pip install git+https://github.com/cornellius-gp/gpytorch.git
         export ALLOW_LATEST_GPYTORCH_LINOP=true
         pip install git+https://github.com/pytorch/botorch.git
         export ALLOW_BOTORCH_LATEST=true
         git clone https://github.com/facebook/ax.git --depth 1
         cd ax
-        pip install -e .[unittest]
+        pip install -e .[tutorial]
         ```
         
         See recommendation for installing PyTorch for MacOS users above.
         
         The above example limits the cloned directory size via the
         [`--depth`](https://git-scm.com/docs/git-clone#Documentation/git-clone.txt---depthltdepthgt)
         argument to `git clone`. If you require the entire commit history you may remove this
```

### Comparing `ax-platform-0.3.2/README.md` & `ax-platform-0.3.3/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -164,15 +164,15 @@
 pip install git+https://github.com/cornellius-gp/linear_operator.git
 pip install git+https://github.com/cornellius-gp/gpytorch.git
 export ALLOW_LATEST_GPYTORCH_LINOP=true
 pip install git+https://github.com/pytorch/botorch.git
 export ALLOW_BOTORCH_LATEST=true
 git clone https://github.com/facebook/ax.git --depth 1
 cd ax
-pip install -e .[unittest]
+pip install -e .[tutorial]
 ```
 
 See recommendation for installing PyTorch for MacOS users above.
 
 The above example limits the cloned directory size via the
 [`--depth`](https://git-scm.com/docs/git-clone#Documentation/git-clone.txt---depthltdepthgt)
 argument to `git clone`. If you require the entire commit history you may remove this
```

### Comparing `ax-platform-0.3.2/ax/__init__.py` & `ax-platform-0.3.3/ax/__init__.py`

 * *Files identical despite different names*

### Comparing `ax-platform-0.3.2/ax/benchmark/benchmark.py` & `ax-platform-0.3.3/ax/benchmark/benchmark.py`

 * *Files 21% similar despite different names*

```diff
@@ -13,33 +13,71 @@
 * Full run: multiple tests on many (BenchmarkProblem, BenchmarkMethod) pairs.
 * Method: (one of) the algorithm(s) being benchmarked.
 * Problem: a synthetic function, a surrogate surface, or an ML model, on which
   to assess the performance of algorithms.
 
 """
 
-from functools import partial
 from itertools import product
+from logging import Logger
 from time import time
-from typing import Any, Iterable, List
+from typing import Iterable, List
 
 import numpy as np
 
 from ax.benchmark.benchmark_method import BenchmarkMethod
 from ax.benchmark.benchmark_problem import (
     BenchmarkProblem,
     MultiObjectiveBenchmarkProblem,
     SingleObjectiveBenchmarkProblem,
 )
 from ax.benchmark.benchmark_result import AggregatedBenchmarkResult, BenchmarkResult
 from ax.core.experiment import Experiment
 from ax.core.utils import get_model_times
 from ax.service.scheduler import Scheduler
+from ax.utils.common.logger import get_logger
 from botorch.utils.sampling import manual_seed
 
+logger: Logger = get_logger(__name__)
+
+
+def compute_score_trace(
+    optimization_trace: np.ndarray,
+    num_baseline_trials: int,
+    problem: BenchmarkProblem,
+) -> np.ndarray:
+    """Computes a score trace from the optimization trace."""
+
+    # Use the first GenerationStep's best found point as baseline. Sometimes (ex. in
+    # a timeout) the first GenerationStep will not have not completed and we will not
+    # have enough trials; in this case we do not score.
+    baseline = (
+        optimization_trace[num_baseline_trials - 1]
+        if len(optimization_trace) > num_baseline_trials
+        else None
+    )
+
+    if isinstance(problem, SingleObjectiveBenchmarkProblem):
+        optimum = problem.optimal_value
+    elif isinstance(problem, MultiObjectiveBenchmarkProblem):
+        optimum = problem.maximum_hypervolume
+    else:
+        # If no known optimum exists scoring cannot take place in a meaningful way
+        optimum = None
+
+    if optimum is None or baseline is None:
+        return np.full(len(optimization_trace), np.nan)
+    score_trace = 100 * (1 - (optimization_trace - optimum) / (baseline - optimum))
+    if score_trace.max() > 100:
+        logger.info(
+            "Observed scores above 100. This indicates that we found a trial that is "
+            "better than the optimum. Clipping scores to 100 for now."
+        )
+    return score_trace.clip(min=0, max=100)
+
 
 def benchmark_replication(
     problem: BenchmarkProblem,
     method: BenchmarkMethod,
     seed: int,
 ) -> BenchmarkResult:
     """Runs one benchmarking replication (equivalent to one optimization loop).
@@ -65,37 +103,19 @@
         options=method.scheduler_options,
     )
 
     with manual_seed(seed=seed):
         scheduler.run_n_trials(max_trials=problem.num_trials)
 
     optimization_trace = np.array(scheduler.get_trace())
-
-    # Use the first GenerationStep's best found point as baseline. Sometimes (ex. in
-    # a timeout) the first GenerationStep will not have not completed and we will not
-    # have enough trials; in this case we do not score.
     num_baseline_trials = scheduler.generation_strategy._steps[0].num_trials
-    baseline = (
-        optimization_trace[num_baseline_trials - 1]
-        if len(optimization_trace) > num_baseline_trials
-        else None
-    )
-
-    if isinstance(problem, SingleObjectiveBenchmarkProblem):
-        optimum = problem.optimal_value
-    elif isinstance(problem, MultiObjectiveBenchmarkProblem):
-        optimum = problem.maximum_hypervolume
-    else:
-        # If no known optimum exists scoring cannot take place in a meaningful way
-        optimum = None
-
-    score_trace = (
-        (100 * (1 - (optimization_trace - optimum) / (baseline - optimum))).clip(min=0)
-        if optimum is not None and baseline is not None
-        else np.full(len(optimization_trace), np.nan)
+    score_trace = compute_score_trace(
+        optimization_trace=optimization_trace,
+        num_baseline_trials=num_baseline_trials,
+        problem=problem,
     )
 
     fit_time, gen_time = get_model_times(experiment=scheduler.experiment)
 
     return BenchmarkResult(
         name=scheduler.experiment.name,
         seed=seed,
@@ -103,27 +123,35 @@
         optimization_trace=optimization_trace,
         score_trace=score_trace,
         fit_time=fit_time,
         gen_time=gen_time,
     )
 
 
-def benchmark_test(
+def benchmark_one_method_problem(
     problem: BenchmarkProblem,
     method: BenchmarkMethod,
     seeds: Iterable[int],
-    **kwargs: Any,
 ) -> AggregatedBenchmarkResult:
-    base_case = partial(benchmark_replication, problem=problem, method=method, **kwargs)
     return AggregatedBenchmarkResult.from_benchmark_results(
-        results=[base_case(seed=seed) for seed in seeds]
+        results=[
+            benchmark_replication(problem=problem, method=method, seed=seed)
+            for seed in seeds
+        ]
     )
 
 
-def benchmark_full_run(
+def benchmark_multiple_problems_methods(
     problems: Iterable[BenchmarkProblem],
     methods: Iterable[BenchmarkMethod],
     seeds: Iterable[int],
-    **kwargs: Any,
 ) -> List[AggregatedBenchmarkResult]:
-    test_env = partial(benchmark_test, seeds=seeds, **kwargs)
-    return [test_env(problem=p, method=m) for p, m in product(problems, methods)]
+    """
+    For each `problem` and `method` in the Cartesian product of `problems` and
+    `methods`, run the replication on each seed in `seeds` and get the results
+    as an `AggregatedBenchmarkResult`, then return a list of each
+    `AggregatedBenchmarkResult`.
+    """
+    return [
+        benchmark_one_method_problem(problem=p, method=m, seeds=seeds)
+        for p, m in product(problems, methods)
+    ]
```

### Comparing `ax-platform-0.3.2/ax/benchmark/benchmark_method.py` & `ax-platform-0.3.3/ax/benchmark/benchmark_method.py`

 * *Files identical despite different names*

### Comparing `ax-platform-0.3.2/ax/benchmark/benchmark_problem.py` & `ax-platform-0.3.3/ax/benchmark/benchmark_problem.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # Copyright (c) Meta Platforms, Inc. and affiliates.
 #
 # This source code is licensed under the MIT license found in the
 # LICENSE file in the root directory of this source tree.
 
 
 from dataclasses import dataclass, field
-from typing import Any, Dict, List, Type
+from typing import Any, Dict, List, Optional, Type
 
 from ax.core.metric import Metric
 
 from ax.core.objective import MultiObjective, Objective
 from ax.core.optimization_config import (
     MultiObjectiveOptimizationConfig,
     ObjectiveThreshold,
@@ -28,14 +28,28 @@
 
 # NOTE: Do not add `from __future__ import annotatations` to this file. Adding
 # `annotations` postpones evaluation of types and will break FBLearner's usage of
 # `BenchmarkProblem` as return type annotation, used for serialization and rendering
 # in the UI.
 
 
+def _get_name(
+    test_problem: BaseTestProblem, infer_noise: bool, dim: Optional[int] = None
+) -> str:
+    """
+    Get a string name describing the problem, in a format such as
+    "hartmann_fixed_noise_6d" or "jenatton" (where the latter would
+    not have fixed noise and have the default dimensionality).
+    """
+    base_name = f"{test_problem.__class__.__name__}"
+    fixed_noise = "" if infer_noise else "_fixed_noise"
+    dim_str = "" if dim is None else f"_{dim}d"
+    return f"{base_name}{fixed_noise}{dim_str}"
+
+
 @dataclass(frozen=True)
 class BenchmarkProblem(Base):
     """Benchmark problem, represented in terms of Ax search space, optimization
     config, and runner.
     """
 
     name: str
@@ -70,26 +84,29 @@
                     lower=test_problem._bounds[i][0],
                     upper=test_problem._bounds[i][1],
                 )
                 for i in range(test_problem.dim)
             ]
         )
 
+        dim = test_problem_kwargs.get("dim", None)
+        name = _get_name(test_problem, infer_noise, dim)
+
         optimization_config = OptimizationConfig(
             objective=Objective(
                 metric=BotorchTestProblemMetric(
-                    name=f"{test_problem.__class__.__name__}",
+                    name=name,
                     noise_sd=None if infer_noise else (test_problem.noise_std or 0),
                 ),
                 minimize=True,
             )
         )
 
         return cls(
-            name=f"{test_problem.__class__.__name__}",
+            name=name,
             search_space=search_space,
             optimization_config=optimization_config,
             runner=BotorchTestProblemRunner(
                 test_problem_class=test_problem_class,
                 test_problem_kwargs=test_problem_kwargs,
             ),
             num_trials=num_trials,
@@ -128,16 +145,19 @@
         problem = BenchmarkProblem.from_botorch(
             test_problem_class=test_problem_class,
             test_problem_kwargs=test_problem_kwargs,
             num_trials=num_trials,
             infer_noise=infer_noise,
         )
 
+        dim = test_problem_kwargs.get("dim", None)
+        name = _get_name(test_problem, infer_noise, dim)
+
         return cls(
-            name=f"{test_problem.__class__.__name__}",
+            name=name,
             search_space=problem.search_space,
             optimization_config=problem.optimization_config,
             runner=problem.runner,
             num_trials=num_trials,
             infer_noise=infer_noise,
             optimal_value=test_problem.optimal_value,
         )
@@ -182,17 +202,20 @@
         problem = BenchmarkProblem.from_botorch(
             test_problem_class=test_problem_class,
             test_problem_kwargs=test_problem_kwargs,
             num_trials=num_trials,
             infer_noise=infer_noise,
         )
 
+        dim = test_problem_kwargs.get("dim", None)
+        name = _get_name(test_problem, infer_noise, dim)
+
         metrics = [
             BotorchTestProblemMetric(
-                name=f"{test_problem.__class__.__name__}_{i}",
+                name=f"{name}_{i}",
                 noise_sd=None if infer_noise else (test_problem.noise_std or 0),
                 index=i,
             )
             for i in range(test_problem.num_objectives)
         ]
         optimization_config = MultiObjectiveOptimizationConfig(
             objective=MultiObjective(
@@ -203,25 +226,24 @@
                     )
                     for metric in metrics
                 ]
             ),
             objective_thresholds=[
                 ObjectiveThreshold(
                     metric=metrics[i],
-                    # pyre-fixme[6]: For 2nd param expected `float` but got `Tensor`.
-                    bound=test_problem.ref_point[i],
+                    bound=test_problem.ref_point[i].item(),
                     relative=False,
                     op=ComparisonOp.LEQ,
                 )
                 for i in range(test_problem.num_objectives)
             ],
         )
 
         return cls(
-            name=f"{test_problem.__class__.__name__}",
+            name=name,
             search_space=problem.search_space,
             optimization_config=optimization_config,
             runner=problem.runner,
             num_trials=num_trials,
             infer_noise=infer_noise,
             maximum_hypervolume=test_problem.max_hv,
             reference_point=test_problem._ref_point,
```

### Comparing `ax-platform-0.3.2/ax/benchmark/methods/choose_generation_strategy.py` & `ax-platform-0.3.3/ax/benchmark/methods/choose_generation_strategy.py`

 * *Files identical despite different names*

### Comparing `ax-platform-0.3.2/ax/benchmark/methods/gpei_and_moo.py` & `ax-platform-0.3.3/ax/benchmark/methods/gpei_and_moo.py`

 * *Files identical despite different names*

### Comparing `ax-platform-0.3.2/ax/benchmark/methods/modular_botorch.py` & `ax-platform-0.3.3/ax/benchmark/methods/modular_botorch.py`

 * *Files identical despite different names*

### Comparing `ax-platform-0.3.2/ax/benchmark/methods/saasbo.py` & `ax-platform-0.3.3/ax/benchmark/methods/saasbo.py`

 * *Files identical despite different names*

### Comparing `ax-platform-0.3.2/ax/benchmark/problems/hd_embedding.py` & `ax-platform-0.3.3/ax/benchmark/problems/hd_embedding.py`

 * *Files 20% similar despite different names*

```diff
@@ -9,14 +9,22 @@
 from ax.core.parameter import ParameterType, RangeParameter
 from ax.core.search_space import SearchSpace
 
 
 def embed_higher_dimension(
     problem: BenchmarkProblem, total_dimensionality: int
 ) -> BenchmarkProblem:
+    """
+    Return a new `BenchmarkProblem` with enough `RangeParameter`s added to the
+    search space to make its total dimensionality equal to `total_dimensionality`
+    and add `total_dimensionality` to its name.
+
+    The search space of the original `problem` is within the search space of the
+    new problem, and the constraints are copied from the original problem.
+    """
     num_dummy_dimensions = total_dimensionality - len(problem.search_space.parameters)
 
     search_space = SearchSpace(
         parameters=[
             *problem.search_space.parameters.values(),
             *[
                 RangeParameter(
@@ -27,12 +35,21 @@
                 )
                 for i in range(num_dummy_dimensions)
             ],
         ],
         parameter_constraints=problem.search_space.parameter_constraints,
     )
 
+    # if problem name already has dimensionality in it, strip it
+    def _is_dim_suffix(s: str) -> bool:
+        return s[-1] == "d" and all(char in "0123456789" for char in s[:-1])
+
+    orig_name_without_dimensionality = "_".join(
+        [substr for substr in problem.name.split("_") if not _is_dim_suffix(substr)]
+    )
+    new_name = f"{orig_name_without_dimensionality}_{total_dimensionality}d"
+
     problem_kwargs = asdict(problem)
-    problem_kwargs["name"] = f"{problem_kwargs['name']}_{total_dimensionality}d"
+    problem_kwargs["name"] = new_name
     problem_kwargs["search_space"] = search_space
 
     return problem.__class__(**problem_kwargs)
```

### Comparing `ax-platform-0.3.2/ax/benchmark/problems/hpo/pytorch_cnn.py` & `ax-platform-0.3.3/ax/benchmark/problems/hpo/pytorch_cnn.py`

 * *Files identical despite different names*

### Comparing `ax-platform-0.3.2/ax/benchmark/problems/hpo/torchvision.py` & `ax-platform-0.3.3/ax/benchmark/problems/hpo/torchvision.py`

 * *Files identical despite different names*

### Comparing `ax-platform-0.3.2/ax/benchmark/problems/registry.py` & `ax-platform-0.3.3/ax/benchmark/problems/registry.py`

 * *Files identical despite different names*

### Comparing `ax-platform-0.3.2/ax/benchmark/problems/surrogate.py` & `ax-platform-0.3.3/ax/benchmark/problems/surrogate.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,35 +1,41 @@
 # Copyright (c) Meta Platforms, Inc. and affiliates.
 #
 # This source code is licensed under the MIT license found in the
 # LICENSE file in the root directory of this source tree.
 
-from typing import Any, Dict, Iterable, List, Set
+from typing import Any, Dict, Iterable, List, Optional, Set, Tuple
 
 import pandas as pd
 import torch
 from ax.benchmark.benchmark_problem import (
     MultiObjectiveBenchmarkProblem,
     SingleObjectiveBenchmarkProblem,
 )
 from ax.core.base_trial import BaseTrial, TrialStatus
 from ax.core.data import Data
 from ax.core.metric import Metric, MetricFetchE, MetricFetchResult
+from ax.core.observation import ObservationFeatures
 from ax.core.optimization_config import (
     MultiObjectiveOptimizationConfig,
     OptimizationConfig,
 )
+from ax.core.parameter import RangeParameter
 from ax.core.runner import Runner
 from ax.core.search_space import SearchSpace
+from ax.core.types import TParameterization
 from ax.exceptions.core import UnsupportedError
+from ax.modelbridge.transforms.int_to_float import IntToFloat
+from ax.modelbridge.transforms.log import Log
 from ax.models.torch.botorch_modular.surrogate import Surrogate
 
 from ax.utils.common.base import Base
 from ax.utils.common.equality import equality_typechecker
 from ax.utils.common.result import Err, Ok
+from ax.utils.common.typeutils import not_none
 from botorch.utils.datasets import SupervisedDataset
 
 
 class SurrogateBenchmarkProblem(SingleObjectiveBenchmarkProblem):
     @equality_typechecker
     def __eq__(self, other: Base) -> bool:
         if not isinstance(other, SurrogateBenchmarkProblem):
@@ -167,21 +173,50 @@
         self.metric_names = metric_names
         self.datasets = datasets
         self.search_space = search_space
 
         self.results: Dict[int, float] = {}
         self.statuses: Dict[int, TrialStatus] = {}
 
+        # If there are log scale parameters, these need to be transformed.
+        if any(
+            isinstance(p, RangeParameter) and p.log_scale
+            for p in search_space.parameters.values()
+        ):
+            int_to_float_tf = IntToFloat(search_space=search_space)
+            log_tf = Log(
+                search_space=int_to_float_tf.transform_search_space(
+                    search_space.clone()
+                )
+            )
+            self.transforms: Optional[Tuple[IntToFloat, Log]] = (
+                int_to_float_tf,
+                log_tf,
+            )
+        else:
+            self.transforms = None
+
+    def _get_transformed_parameters(
+        self, parameters: TParameterization
+    ) -> TParameterization:
+        if self.transforms is None:
+            return parameters
+
+        obs_ft = ObservationFeatures(parameters=parameters)
+        for t in not_none(self.transforms):
+            obs_ft = t.transform_observation_features([obs_ft])[0]
+        return obs_ft.parameters
+
     def run(self, trial: BaseTrial) -> Dict[str, Any]:
         self.statuses[trial.index] = TrialStatus.COMPLETED
         preds = {  # Cache predictions for each arm
             arm.name: self.surrogate.predict(
-                X=torch.tensor([*arm.parameters.values()]).reshape(
-                    [1, len(arm.parameters)]
-                )
+                X=torch.tensor(
+                    [*self._get_transformed_parameters(arm.parameters).values()]
+                ).reshape([1, len(arm.parameters)])
             )[0].squeeze(0)
             for arm in trial.arms
         }
         return {
             metric_name: {arm_name: pred[i] for arm_name, pred in preds.items()}
             for i, metric_name in enumerate(self.metric_names)
         }
```

### Comparing `ax-platform-0.3.2/ax/benchmark/problems/synthetic/discretized/mixed_integer.py` & `ax-platform-0.3.3/ax/benchmark/problems/synthetic/discretized/mixed_integer.py`

 * *Files identical despite different names*

### Comparing `ax-platform-0.3.2/ax/benchmark/problems/synthetic/hss/jenatton.py` & `ax-platform-0.3.3/ax/benchmark/problems/synthetic/hss/jenatton.py`

 * *Files 2% similar despite different names*

```diff
@@ -56,16 +56,18 @@
 
     optimization_config = OptimizationConfig(
         objective=Objective(
             metric=JenattonMetric(infer_noise=infer_noise), minimize=True
         )
     )
 
+    name = "Jenatton" + ("" if infer_noise else "_fixed_noise")
+
     return SingleObjectiveBenchmarkProblem(
-        name="Jenatton",
+        name=name,
         search_space=search_space,
         optimization_config=optimization_config,
         runner=SyntheticRunner(),
         num_trials=num_trials,
         infer_noise=infer_noise,
         optimal_value=0.1,
     )
```

### Comparing `ax-platform-0.3.2/ax/benchmark/tests/test_benchmark.py` & `ax-platform-0.3.3/ax/benchmark/tests/test_benchmark.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,17 +1,17 @@
 # Copyright (c) Meta Platforms, Inc. and affiliates.
 #
 # This source code is licensed under the MIT license found in the
 # LICENSE file in the root directory of this source tree.
 
 import numpy as np
 from ax.benchmark.benchmark import (
-    benchmark_full_run,
+    benchmark_multiple_problems_methods,
+    benchmark_one_method_problem,
     benchmark_replication,
-    benchmark_test,
 )
 from ax.benchmark.benchmark_method import BenchmarkMethod
 from ax.benchmark.benchmark_problem import SingleObjectiveBenchmarkProblem
 from ax.modelbridge.generation_strategy import GenerationStep, GenerationStrategy
 from ax.modelbridge.registry import Models
 from ax.service.utils.scheduler_options import SchedulerOptions
 from ax.utils.common.testutils import TestCase
@@ -54,46 +54,46 @@
         self.assertEqual(
             problem.num_trials * 2,
             len(res.experiment.fetch_data().df),
         )
 
         self.assertTrue(np.all(res.score_trace <= 100))
 
-    def test_test(self) -> None:
+    def test_benchmark_one_method_problem(self) -> None:
         problem = get_single_objective_benchmark_problem()
-        agg = benchmark_test(
+        agg = benchmark_one_method_problem(
             problem=problem,
             method=get_sobol_benchmark_method(),
             seeds=(0, 1),
         )
 
         self.assertEqual(len(agg.results), 2)
         self.assertTrue(
             all(
                 len(result.experiment.trials) == problem.num_trials
                 for result in agg.results
             ),
             "All experiments must have 4 trials",
         )
 
-        for col in ["mean", "P10", "P25", "P50", "P75", "P90"]:
+        for col in ["mean", "P25", "P50", "P75"]:
             self.assertTrue((agg.score_trace[col] <= 100).all())
 
     @fast_botorch_optimize
-    def test_full_run(self) -> None:
-        aggs = benchmark_full_run(
+    def test_benchmark_multiple_problems_methods(self) -> None:
+        aggs = benchmark_multiple_problems_methods(
             problems=[get_single_objective_benchmark_problem()],
             methods=[get_sobol_benchmark_method(), get_sobol_gpei_benchmark_method()],
             seeds=(0, 1),
         )
 
         self.assertEqual(len(aggs), 2)
 
         for agg in aggs:
-            for col in ["mean", "P10", "P25", "P50", "P75", "P90"]:
+            for col in ["mean", "P25", "P50", "P75"]:
                 self.assertTrue((agg.score_trace[col] <= 100).all())
 
     def test_timeout(self) -> None:
         problem = SingleObjectiveBenchmarkProblem.from_botorch_synthetic(
             test_problem_class=Branin,
             test_problem_kwargs={},
             num_trials=1000,  # Unachievable num_trials
@@ -119,14 +119,16 @@
                 init_seconds_between_polls=0,
                 min_seconds_before_poll=0,
                 timeout_hours=0.001,  # Strict timeout of 3.6 seconds
             ),
         )
 
         # Each replication will have a different number of trials
-        result = benchmark_test(problem=problem, method=method, seeds=(0, 1, 2, 3))
+        result = benchmark_one_method_problem(
+            problem=problem, method=method, seeds=(0, 1, 2, 3)
+        )
 
         # Test the traces get composited correctly. The AggregatedResult's traces
         # should be the length of the shortest trace in the BenchmarkResults
         min_num_trials = min(len(res.optimization_trace) for res in result.results)
         self.assertEqual(len(result.optimization_trace), min_num_trials)
         self.assertEqual(len(result.score_trace), min_num_trials)
```

### Comparing `ax-platform-0.3.2/ax/benchmark/tests/test_benchmark_method.py` & `ax-platform-0.3.3/ax/benchmark/tests/test_benchmark_method.py`

 * *Files identical despite different names*

### Comparing `ax-platform-0.3.2/ax/benchmark/tests/test_benchmark_problem.py` & `ax-platform-0.3.3/ax/benchmark/tests/test_benchmark_problem.py`

 * *Files identical despite different names*

### Comparing `ax-platform-0.3.2/ax/benchmark/tests/test_methods.py` & `ax-platform-0.3.3/ax/benchmark/tests/test_methods.py`

 * *Files identical despite different names*

### Comparing `ax-platform-0.3.2/ax/benchmark/tests/test_mixed_integer_problems.py` & `ax-platform-0.3.3/ax/benchmark/tests/test_mixed_integer_problems.py`

 * *Files identical despite different names*

### Comparing `ax-platform-0.3.2/ax/benchmark/tests/test_problem_storage.py` & `ax-platform-0.3.3/ax/benchmark/tests/test_problem_storage.py`

 * *Files identical despite different names*

### Comparing `ax-platform-0.3.2/ax/core/__init__.py` & `ax-platform-0.3.3/ax/core/__init__.py`

 * *Files identical despite different names*

### Comparing `ax-platform-0.3.2/ax/core/arm.py` & `ax-platform-0.3.3/ax/core/arm.py`

 * *Files identical despite different names*

### Comparing `ax-platform-0.3.2/ax/core/base_trial.py` & `ax-platform-0.3.3/ax/core/base_trial.py`

 * *Files 0% similar despite different names*

```diff
@@ -638,17 +638,18 @@
 
     def mark_running(
         self, no_runner_required: bool = False, unsafe: bool = False
     ) -> BaseTrial:
         """Mark trial has started running.
 
         Args:
-            no_runner_required: Whether to skip the check for presence of a ``Runner``
-            on experiment.
+            no_runner_required: Whether to skip the check for presence of a
+                ``Runner`` on the experiment.
             unsafe: Ignore sanity checks on state transitions.
+
         Returns:
             The trial instance.
         """
         if self._runner is None and not no_runner_required:
             raise ValueError("Cannot mark trial running without setting runner.")
 
         prev_step = (
```

### Comparing `ax-platform-0.3.2/ax/core/batch_trial.py` & `ax-platform-0.3.3/ax/core/batch_trial.py`

 * *Files 2% similar despite different names*

```diff
@@ -24,21 +24,25 @@
 
 import numpy as np
 from ax.core.arm import Arm
 from ax.core.base_trial import BaseTrial
 from ax.core.data import Data
 from ax.core.generator_run import ArmWeight, GeneratorRun, GeneratorRunType
 from ax.core.trial import immutable_once_run
-from ax.core.types import TCandidateMetadata, TEvaluationOutcome
+from ax.core.types import (
+    TCandidateMetadata,
+    TEvaluationOutcome,
+    validate_evaluation_outcome,
+)
 from ax.exceptions.core import AxError, UserInputError
 from ax.utils.common.base import SortableBase
 from ax.utils.common.docutils import copy_doc
 from ax.utils.common.equality import datetime_equals, equality_typechecker
 from ax.utils.common.logger import _round_floats_for_logging, get_logger
-from ax.utils.common.typeutils import checked_cast, checked_cast_complex, not_none
+from ax.utils.common.typeutils import checked_cast, not_none
 
 
 logger: Logger = get_logger(__name__)
 
 
 if TYPE_CHECKING:
     # import as module to make sphinx-autodoc-typehints happy
@@ -564,31 +568,36 @@
             raw_data: Map from arm name to metric outcomes.
             sample_sizes: Dict from arm name to sample size.
             metadata: Additional metadata to track about this run.
                 importantly the start_date and end_date
             complete_trial: Whether to mark trial as complete after
                 attaching data. Defaults to False.
         """
+        # Validate type of raw_data
+        if not isinstance(raw_data, dict):
+            raise ValueError(BATCH_TRIAL_RAW_DATA_FORMAT_ERROR_MESSAGE)
+
+        for key, value in raw_data.items():
+            if not isinstance(key, str):
+                raise ValueError(BATCH_TRIAL_RAW_DATA_FORMAT_ERROR_MESSAGE)
+
+            try:
+                validate_evaluation_outcome(outcome=value)
+            except TypeError:
+                raise ValueError(BATCH_TRIAL_RAW_DATA_FORMAT_ERROR_MESSAGE)
 
         # Format the data to save.
-        raw_data_by_arm = checked_cast_complex(
-            Dict[str, TEvaluationOutcome],
-            raw_data,
-            message=BATCH_TRIAL_RAW_DATA_FORMAT_ERROR_MESSAGE,
-        )
-        not_trial_arm_names = set(raw_data_by_arm.keys()) - set(
-            self.arms_by_name.keys()
-        )
+        not_trial_arm_names = set(raw_data.keys()) - set(self.arms_by_name.keys())
         if not_trial_arm_names:
             raise UserInputError(  # pragma: no cover
                 f"Arms {not_trial_arm_names} are not part of trial #{self.index}."
             )
 
         evaluations, data = self._make_evaluations_and_data(
-            raw_data=raw_data_by_arm, metadata=metadata, sample_sizes=sample_sizes
+            raw_data=raw_data, metadata=metadata, sample_sizes=sample_sizes
         )
         self._validate_batch_trial_data(data=data)
 
         self._run_metadata = metadata or {}
         self.experiment.attach_data(data)
 
         data_for_logging = _round_floats_for_logging(item=evaluations)
```

### Comparing `ax-platform-0.3.2/ax/core/data.py` & `ax-platform-0.3.3/ax/core/data.py`

 * *Files 12% similar despite different names*

```diff
@@ -3,67 +3,72 @@
 #
 # This source code is licensed under the MIT license found in the
 # LICENSE file in the root directory of this source tree.
 
 from __future__ import annotations
 
 import json
+from abc import abstractmethod
 from functools import reduce
 from hashlib import md5
-from typing import Any, Dict, Iterable, Optional, Set, Type, Union
+from typing import Any, Dict, Iterable, List, Optional, Set, Type, TypeVar, Union
 
 import numpy as np
 import pandas as pd
 from ax.core.types import TFidelityTrialEvaluation, TTrialEvaluation
 from ax.utils.common.base import Base
 from ax.utils.common.serialization import (
     extract_init_args,
     SerializationMixin,
     serialize_init_args,
 )
 from ax.utils.common.typeutils import checked_cast, not_none
 
+TBaseData = TypeVar("TBaseData", bound="BaseData")
 
-class Data(Base, SerializationMixin):
+
+class BaseData(Base, SerializationMixin):
     """Class storing data for an experiment.
 
     The dataframe is retrieved via the `df` property. The data can be stored
     to an external store for future use by attaching it to an experiment using
     `experiment.attach_data()` (this requires a description to be set.)
 
 
     Attributes:
-        df: DataFrame with underlying data, and required columns.
+        df: DataFrame with underlying data, and required columns. For BaseData, the
+            one required column is "arm_name".
         description: Human-readable description of data.
 
     """
 
-    # Note: Although the SEM (standard error of the mean) is a required column in data,
-    # downstream models can infer missing SEMs. Simply specify NaN as the SEM value,
-    # either in your Metric class or in Data explicitly.
-    REQUIRED_COLUMNS = {"arm_name", "metric_name", "mean", "sem"}
+    REQUIRED_COLUMNS = {"arm_name"}
 
-    COLUMN_DATA_TYPES = {
+    COLUMN_DATA_TYPES: Dict[str, Any] = {
+        # Ubiquitous columns.
         "arm_name": str,
+        # Metric data-related columns.
         "metric_name": str,
         "mean": np.float64,
         "sem": np.float64,
+        # Metadata columns available for all subclasses.
         "trial_index": np.int64,
         "start_time": pd.Timestamp,
         "end_time": pd.Timestamp,
         "n": np.int64,
+        # Metadata columns available for only some subclasses.
         "frac_nonnull": np.float64,
         "random_split": np.int64,
         "fidelities": str,  # Dictionary stored as json
     }
 
     _df: pd.DataFrame
 
     def __init__(
-        self,
+        self: TBaseData,
         df: Optional[pd.DataFrame] = None,
         description: Optional[str] = None,
     ) -> None:
         """Init Data.
 
         Args:
             df: DataFrame with underlying data, and required columns.
@@ -90,15 +95,15 @@
             col_order = [c for c in self.column_data_types() if c in df.columns]
             self._df = df[col_order]
 
         self.description = description
 
     @classmethod
     def _safecast_df(
-        cls,
+        cls: Type[TBaseData],
         df: pd.DataFrame,
         # pyre-fixme[24]: Generic type `type` expects 1 type parameter, use
         #  `typing.Type` to avoid runtime subscripting errors.
         extra_column_types: Optional[Dict[str, Type]] = None,
     ) -> pd.DataFrame:
         """Function for safely casting df to standard data types.
 
@@ -171,20 +176,20 @@
 
     @classmethod
     # pyre-fixme[2]: Parameter annotation cannot be `Any`.
     def serialize_init_args(cls, obj: Any) -> Dict[str, Any]:
         """Serialize the class-dependent properties needed to initialize this Data.
         Used for storage and to help construct new similar Data.
         """
-        data = checked_cast(Data, obj)
+        data = checked_cast(cls, obj)
         return serialize_init_args(object=data)
 
     @classmethod
     def deserialize_init_args(cls, args: Dict[str, Any]) -> Dict[str, Any]:
-        """Given a dictionary, extract the properties needed to initialize the metric.
+        """Given a dictionary, extract the properties needed to initialize the object.
         Used for storage.
         """
         # Extract `df` only if present, since certain inputs to this fn, e.g.
         # SQAData.structure_metadata_json, don't have a `df` attribute.
         if "df" in args and not isinstance(args["df"], pd.DataFrame):
             # NOTE: Need dtype=False, otherwise infers arm_names like
             # "4_1" should be int 41.
@@ -216,64 +221,17 @@
 
         Returns
             str: The hash of the DataFrame.
 
         """
         return md5(not_none(self.df.to_json()).encode("utf-8")).hexdigest()
 
-    @property
-    def metric_names(self) -> Set[str]:
-        """Set of metric names that appear in the underlying dataframe of
-        this object.
-        """
-        return set() if self.df.empty else set(self.df["metric_name"].values)
-
-    def filter(
-        self,
-        trial_indices: Optional[Iterable[int]] = None,
-        metric_names: Optional[Iterable[str]] = None,
-    ) -> Data:
-        """Construct a new Data object with the subset of rows corresponding to the
-        provided trial indices AND metric names. If either trial_indices or
-        metric_names are not provided, that dimension will not be filtered.
-        """
-
-        return Data(
-            df=self._filter_df(
-                df=self.df, trial_indices=trial_indices, metric_names=metric_names
-            )
-        )
-
-    @staticmethod
-    def _filter_df(
-        df: pd.DataFrame,
-        trial_indices: Optional[Iterable[int]] = None,
-        metric_names: Optional[Iterable[str]] = None,
+    def get_filtered_results(
+        self: TBaseData, **filters: Dict[str, Any]
     ) -> pd.DataFrame:
-        trial_indices_mask = (
-            reduce(
-                lambda left, right: left | right,
-                [df["trial_index"] == trial_index for trial_index in trial_indices],
-            )
-            if trial_indices is not None
-            else pd.Series([True] * len(df))
-        )
-
-        metric_names_mask = (
-            reduce(
-                lambda left, right: left | right,
-                [df["metric_name"] == metric_name for metric_name in metric_names],
-            )
-            if metric_names is not None
-            else pd.Series([True] * len(df))
-        )
-
-        return df.loc[trial_indices_mask & metric_names_mask]
-
-    def get_filtered_results(self, **filters: Dict[str, Any]) -> pd.DataFrame:
         """Return filtered subset of data.
 
         Args:
             filter: Column names and values they must match.
 
         Returns
             df: The filtered DataFrame.
@@ -288,159 +246,307 @@
                 raise ValueError(
                     f"{colname} not in the set of columns: {columns}"
                     f"in this data object of type: {str(type(self))}."
                 )
             df = df[df[colname] == value]
         return df
 
-    @staticmethod
-    def from_multiple_data(
-        data: Iterable[Data], subset_metrics: Optional[Iterable[str]] = None
-    ) -> Data:
-        """Combines multiple data objects into one (with the concatenated
+    @classmethod
+    def from_multiple(
+        cls: Type[TBaseData],
+        data: Iterable[TBaseData],
+    ) -> TBaseData:
+        """Combines multiple objects into one (with the concatenated
         underlying dataframe).
 
         Args:
-            data: Iterable of Ax `Data` objects to combine.
-            subset_metrics: If specified, combined `Data` will only contain
-                metrics, names of which appear in this iterable,
-                in the underlying dataframe.
+            data: Iterable of Ax objects of this class to combine.
         """
+        incompatible_types = {
+            type(datum) for datum in data if not isinstance(datum, cls)
+        }
+        if incompatible_types:
+            raise TypeError(
+                f"All data objects must be instances of class {cls}. Got "
+                f"{incompatible_types}."
+            )
         dfs = [datum.df for datum in data]
 
         if len(dfs) == 0:
-            return Data()
+            return cls()
 
-        if subset_metrics:
-            dfs = [df.loc[df["metric_name"].isin(subset_metrics)] for df in dfs]
-
-        return Data(df=pd.concat(dfs, axis=0, sort=True))
+        return cls(df=pd.concat(dfs, axis=0, sort=True))
 
-    @staticmethod
+    @classmethod
     def from_evaluations(
+        cls: Type[TBaseData],
         evaluations: Dict[str, TTrialEvaluation],
         trial_index: int,
         sample_sizes: Optional[Dict[str, int]] = None,
         start_time: Optional[Union[int, str]] = None,
         end_time: Optional[Union[int, str]] = None,
-    ) -> Data:
+    ) -> TBaseData:
         """
         Convert dict of evaluations to Ax data object.
 
         Args:
-            evaluations: Map from arm name to metric outcomes, which itself is  a
-                mapping of metric names to means or tuples of mean and an SEM). If
-                SEM is not specified, it will be set to None and inferred from data.
+            evaluations: Map from arm name to outcomes, which itself is a mapping of
+                outcome names to values, means, or tuples of mean and SEM. If SEM is
+                not specified, it will be set to None and inferred from data.
             trial_index: Trial index to which this data belongs.
             sample_sizes: Number of samples collected for each arm.
             start_time: Optional start time of run of the trial that produced this
                 data, in milliseconds or iso format.  Milliseconds will be automatically
                 converted to iso format because iso format automatically works with the
                 pandas column type `Timestamp`.
             end_time: Optional end time of run of the trial that produced this
                 data, in milliseconds or iso format.  Milliseconds will be automatically
                 converted to iso format because iso format automatically works with the
                 pandas column type `Timestamp`.
 
         Returns:
-            Ax Data object.
+            Ax object of the enclosing class.
         """
-        records = [
-            {
-                "arm_name": name,
-                "metric_name": metric_name,
-                "mean": value[0] if isinstance(value, tuple) else value,
-                "sem": value[1] if isinstance(value, tuple) else None,
-                "trial_index": trial_index,
-            }
-            for name, evaluation in evaluations.items()
-            for metric_name, value in evaluation.items()
-        ]
-        if start_time is not None or end_time is not None:
-            if isinstance(start_time, int):
-                start_time = _ms_epoch_to_isoformat(start_time)
-            if isinstance(end_time, int):
-                end_time = _ms_epoch_to_isoformat(end_time)
-
-            for record in records:
-                record.update({"start_time": start_time, "end_time": end_time})
-        if sample_sizes:
-            for record in records:
-                record["n"] = sample_sizes[str(record["arm_name"])]
-        return Data(df=pd.DataFrame(records))
+        records = cls._get_records(evaluations=evaluations, trial_index=trial_index)
+        records = cls._add_cols_to_records(
+            records=records,
+            sample_sizes=sample_sizes,
+            start_time=start_time,
+            end_time=end_time,
+        )
+        return cls(df=pd.DataFrame(records))
 
     @staticmethod
+    @abstractmethod
+    def _get_records(
+        evaluations: Dict[str, TTrialEvaluation], trial_index: int
+    ) -> List[Dict[str, Any]]:
+        pass  # pragma: no cover
+
+    @classmethod
     def from_fidelity_evaluations(
+        cls: Type[TBaseData],
         evaluations: Dict[str, TFidelityTrialEvaluation],
         trial_index: int,
         sample_sizes: Optional[Dict[str, int]] = None,
         start_time: Optional[int] = None,
         end_time: Optional[int] = None,
-    ) -> Data:
+    ) -> TBaseData:
         """
         Convert dict of fidelity evaluations to Ax data object.
 
         Args:
-            evaluations: Map from arm name to list of (fidelity, metric outcomes)
-                where metric outcomes is itself a mapping of metric names to means
+            evaluations: Map from arm name to list of (fidelity, outcomes)
+                where outcomes is itself a mapping of outcome names to values, means,
                 or tuples of mean and SEM. If SEM is not specified, it will be set
                 to None and inferred from data.
             trial_index: Trial index to which this data belongs.
             sample_sizes: Number of samples collected for each arm.
             start_time: Optional start time of run of the trial that produced this
                 data, in milliseconds.
             end_time: Optional end time of run of the trial that produced this
                 data, in milliseconds.
 
         Returns:
-            Ax Data object.
+            Ax object of type ``cls``.
         """
-        records = [
+        records = cls._get_fidelity_records(
+            evaluations=evaluations, trial_index=trial_index
+        )
+        records = cls._add_cols_to_records(
+            records=records,
+            sample_sizes=sample_sizes,
+            start_time=start_time,
+            end_time=end_time,
+        )
+        return cls(df=pd.DataFrame(records))
+
+    @staticmethod
+    @abstractmethod
+    def _get_fidelity_records(
+        evaluations: Dict[str, TFidelityTrialEvaluation], trial_index: int
+    ) -> List[Dict[str, Any]]:
+        pass  # pragma: no cover
+
+    @staticmethod
+    def _add_cols_to_records(
+        records: List[Dict[str, Any]],
+        sample_sizes: Optional[Dict[str, int]] = None,
+        start_time: Optional[Union[int, str]] = None,
+        end_time: Optional[Union[int, str]] = None,
+    ) -> List[Dict[str, Any]]:
+        """Adds to records metadata columns that are available for all
+        BaseData subclasses.
+        """
+        if start_time is not None or end_time is not None:
+            if isinstance(start_time, int):
+                start_time = _ms_epoch_to_isoformat(start_time)
+            if isinstance(end_time, int):
+                end_time = _ms_epoch_to_isoformat(end_time)
+
+            for record in records:
+                record.update({"start_time": start_time, "end_time": end_time})
+        if sample_sizes:
+            for record in records:
+                record["n"] = sample_sizes[str(record["arm_name"])]
+
+        return records
+
+    def copy_structure_with_df(self: TBaseData, df: pd.DataFrame) -> TBaseData:
+        """Serialize the structural properties needed to initialize this class.
+        Used for storage and to help construct new similar objects. All kwargs
+        other than ``df`` and ``description`` are considered structural.
+        """
+        cls = type(self)
+        return cls(df=df, **cls.serialize_init_args(self))
+
+
+class Data(BaseData):
+    """Class storing numerical data for an experiment.
+
+    The dataframe is retrieved via the `df` property. The data can be stored
+    to an external store for future use by attaching it to an experiment using
+    `experiment.attach_data()` (this requires a description to be set.)
+
+
+    Attributes:
+        df: DataFrame with underlying data, and required columns. For BaseData, the
+            required columns are "arm_name", "metric_name", "mean", and "sem", the
+            latter two of which must be numeric.
+        description: Human-readable description of data.
+
+    """
+
+    # Note: Although the SEM (standard error of the mean) is a required column in data,
+    # downstream models can infer missing SEMs. Simply specify NaN as the SEM value,
+    # either in your Metric class or in Data explicitly.
+    REQUIRED_COLUMNS: Set[str] = BaseData.REQUIRED_COLUMNS.union(
+        {"metric_name", "mean", "sem"}
+    )
+
+    @staticmethod
+    def _get_records(
+        evaluations: Dict[str, TTrialEvaluation], trial_index: int
+    ) -> List[Dict[str, Any]]:
+        return [
+            {
+                "arm_name": name,
+                "metric_name": metric_name,
+                "mean": value[0] if isinstance(value, tuple) else value,
+                "sem": value[1] if isinstance(value, tuple) else None,
+                "trial_index": trial_index,
+            }
+            for name, evaluation in evaluations.items()
+            for metric_name, value in evaluation.items()
+        ]
+
+    @staticmethod
+    def _get_fidelity_records(
+        evaluations: Dict[str, TFidelityTrialEvaluation], trial_index: int
+    ) -> List[Dict[str, Any]]:
+        return [
             {
                 "arm_name": name,
                 "metric_name": metric_name,
                 "mean": value[0] if isinstance(value, tuple) else value,
                 "sem": value[1] if isinstance(value, tuple) else None,
                 "trial_index": trial_index,
                 "fidelities": json.dumps(fidelity),
             }
             for name, fidelity_and_metrics_list in evaluations.items()
             for fidelity, evaluation in fidelity_and_metrics_list
             for metric_name, value in evaluation.items()
         ]
-        if start_time is not None or end_time is not None:
-            for record in records:
-                record.update({"start_time": start_time, "end_time": end_time})
-        if sample_sizes:
-            for record in records:
-                record["n"] = sample_sizes[str(record["arm_name"])]
-        return Data(df=pd.DataFrame(records))
 
-    def copy_structure_with_df(self, df: pd.DataFrame) -> Data:
-        """Serialize the structural properties needed to initialize this Data.
-        Used for storage and to help construct new similar Data. All kwargs
-        other than ``df`` and ``description`` are considered structural.
+    @property
+    def metric_names(self) -> Set[str]:
+        """Set of metric names that appear in the underlying dataframe of
+        this object.
         """
-        cls = type(self)
-        return cls(df=df, **cls.serialize_init_args(self))
+        return set() if self.df.empty else set(self.df["metric_name"].values)
+
+    def filter(
+        self,
+        trial_indices: Optional[Iterable[int]] = None,
+        metric_names: Optional[Iterable[str]] = None,
+    ) -> Data:
+        """Construct a new object with the subset of rows corresponding to the
+        provided trial indices AND metric names. If either trial_indices or
+        metric_names are not provided, that dimension will not be filtered.
+        """
+
+        return self.__class__(
+            df=self._filter_df(
+                df=self.df, trial_indices=trial_indices, metric_names=metric_names
+            )
+        )
+
+    @staticmethod
+    def _filter_df(
+        df: pd.DataFrame,
+        trial_indices: Optional[Iterable[int]] = None,
+        metric_names: Optional[Iterable[str]] = None,
+    ) -> pd.DataFrame:
+        trial_indices_mask = (
+            reduce(
+                lambda left, right: left | right,
+                [df["trial_index"] == trial_index for trial_index in trial_indices],
+            )
+            if trial_indices is not None
+            else pd.Series([True] * len(df))
+        )
+
+        metric_names_mask = (
+            reduce(
+                lambda left, right: left | right,
+                [df["metric_name"] == metric_name for metric_name in metric_names],
+            )
+            if metric_names is not None
+            else pd.Series([True] * len(df))
+        )
+
+        return df.loc[trial_indices_mask & metric_names_mask]
+
+    @staticmethod
+    def from_multiple_data(
+        data: Iterable[Data], subset_metrics: Optional[Iterable[str]] = None
+    ) -> Data:
+        """Combines multiple objects into one (with the concatenated
+        underlying dataframe).
+
+        Args:
+            data: Iterable of Ax objects of this class to combine.
+            subset_metrics: If specified, combined object will only contain
+                metrics, names of which appear in this iterable,
+                in the underlying dataframe.
+        """
+        data_out = Data.from_multiple(data=data)
+        if len(data_out.df.index) == 0:
+            return data_out
+        if subset_metrics:
+            data_out._df = data_out.df.loc[
+                data_out.df["metric_name"].isin(subset_metrics)
+            ]
+
+        return data_out
 
 
 def set_single_trial(data: Data) -> Data:
     """Returns a new Data object where we set all rows to have the same
     trial index (i.e. 0). This is meant to be used with our IVW transform,
-    which will combine multiple observations of the same metric.
+    which will combine multiple observations of the same outcome.
     """
     df = data._df.copy()
     if "trial_index" in df:
         df["trial_index"] = 0
     return Data(df=df)
 
 
 def clone_without_metrics(data: Data, excluded_metric_names: Iterable[str]) -> Data:
-    """Returns a new data object where rows containing the metrics specified by
+    """Returns a new data object where rows containing the outcomes specified by
     `metric_names` are filtered out. Used to sanitize data before using it as
     training data for a model that requires data rectangularity.
 
     Args:
         data: Original data to clone.
         excluded_metric_names: Metrics to avoid copying
```

### Comparing `ax-platform-0.3.2/ax/core/experiment.py` & `ax-platform-0.3.3/ax/core/experiment.py`

 * *Files 2% similar despite different names*

```diff
@@ -3,14 +3,15 @@
 #
 # This source code is licensed under the MIT license found in the
 # LICENSE file in the root directory of this source tree.
 
 from __future__ import annotations
 
 import logging
+import re
 import warnings
 from collections import defaultdict, OrderedDict
 from datetime import datetime
 from enum import Enum
 from functools import partial, reduce
 from typing import Any, Dict, Iterable, List, Mapping, Optional, Set, Tuple, Type
 
@@ -751,31 +752,18 @@
             data_init_args["df"] = trial_df
             current_trial_data = (
                 self._data_by_trial[trial_index]
                 if trial_index in self._data_by_trial
                 else OrderedDict()
             )
             if combine_with_last_data and len(current_trial_data) > 0:
-                last_ts, last_data = list(current_trial_data.items())[-1]
-                last_data_type = type(last_data)
-                merge_keys = ["trial_index", "metric_name", "arm_name"] + (
-                    last_data.map_keys if issubclass(last_data_type, MapData) else []
+                last_data_type, last_data = self._get_last_data_without_similar_rows(
+                    current_trial_data=current_trial_data, new_df=trial_df
                 )
-                merged = pd.merge(
-                    last_data.true_df,
-                    trial_df,
-                    on=merge_keys,
-                    how="inner",
-                )
-                if not merged.empty:
-                    raise ValueError(
-                        f"Last data for trial {trial_index} already contained an "
-                        f"observation for metric {merged.head()['metric_name']}."
-                    )
-                del current_trial_data[last_ts]
+                current_trial_data.popitem()
                 current_trial_data[cur_time_millis] = last_data_type.from_multiple_data(
                     [
                         last_data,
                         last_data_type(**data_init_args),
                     ]
                 )
             elif overwrite_existing_data:
@@ -795,14 +783,74 @@
                 )
             else:
                 current_trial_data[cur_time_millis] = data_type(**data_init_args)
             self._data_by_trial[trial_index] = current_trial_data
 
         return cur_time_millis
 
+    @staticmethod
+    def _get_last_data_without_similar_rows(
+        current_trial_data: OrderedDict[int, Data], new_df: pd.DataFrame
+    ) -> Tuple[Type[Data], Data]:
+        """Get a copy of last data with rows filtered out sharing values for
+        "trial_index", "metric_name", and "arm_name" with the new data so we
+        can cleanly combine them.
+
+        Args:
+            current_trial_data: The data currently attached to a trial
+            new_df: A DataFrame containing new data to be attached
+
+        Returns:
+            A tuple of two things:
+                - The type of the last data that was attached
+                - A Data object with the most recent data attached, minus the
+                    rows that share the same values
+                    for "trial_index", "metric_name", and "arm_name" in new_df
+        """
+        last_ts, last_data = list(current_trial_data.items())[-1]
+        # Get the init args other than 'df' for last data
+        # in case it was a child class of `Data`
+        last_data_init_args = last_data.deserialize_init_args(
+            last_data.serialize_init_args(last_data)
+        )
+        del last_data_init_args["df"]
+
+        last_data_type = type(last_data)
+        merge_keys = ["trial_index", "metric_name", "arm_name"] + (
+            # pyre-ignore[16]
+            last_data.map_keys
+            if issubclass(last_data_type, MapData)
+            else []
+        )
+        # this merge is like a SQL left join on merge keys
+        # it will return a dataframe with the columns in merge_keys
+        # plus "_merge" and any other columns in last_data.true_df with _left appended
+        # plus any other columns in new_df with _right appended
+        merged = pd.merge(
+            last_data.true_df,
+            new_df,
+            on=merge_keys,
+            how="left",
+            indicator=True,
+            suffixes=("_left", "_right"),
+        )
+        # Filter out all rows that are also present in new_df
+        last_df = merged[merged["_merge"] == "left_only"]
+
+        # Drop the _merge column
+        last_df = last_df.drop(columns=["_merge"])
+        # Drop columns ending with "_right", which should all have null values
+        right_columns = [c for c in last_df.columns if re.match(r".*_right$", c)]
+        last_df = last_df.drop(columns=right_columns)
+
+        # Remove the "_left" suffix from the column names
+        last_df.columns = last_df.columns.str.replace(r"_left$", "", regex=True)
+
+        return type(last_data), last_data_type(df=last_df, **last_data_init_args)
+
     def attach_fetch_results(
         self,
         results: Mapping[int, Mapping[str, MetricFetchResult]],
         combine_with_last_data: bool = False,
         overwrite_existing_data: bool = False,
     ) -> Optional[int]:
         """
@@ -1119,15 +1167,16 @@
 
         NOTE: Currently only handles experiments with 1-arm ``Trial``-s, not
         ``BatchTrial``-s as there has not yet been need for support of the latter.
 
         Args:
             old_experiment: The experiment from which to transfer trials and data
             copy_run_metadata_keys: A list of keys denoting which items to copy over
-                from each trial's run_metadata.
+                from each trial's run_metadata. Defaults to
+                ``old_experiment.runner.run_metadata_report_keys``.
             trial_statuses_to_copy: All trials with a status in this list will be
                 copied. By default, copies all ``RUNNING``, ``COMPLETED``,
                 ``ABANDONED``, and ``EARLY_STOPPED`` trials.
             search_space_check_membership_raise_error: Whether to raise an exception
                 if the warm started trials being imported fall outside of the
                 defined search space.
 
@@ -1136,14 +1185,17 @@
         """
         if len(self.trials) > 0:
             raise ValueError(  # pragma: no cover
                 f"Can only warm-start experiments that don't yet have trials. "
                 f"Experiment {self._name} has {len(self.trials)} trials."
             )
 
+        if copy_run_metadata_keys is None and old_experiment.runner is not None:
+            copy_run_metadata_keys = old_experiment.runner.run_metadata_report_keys
+
         old_parameter_names = set(old_experiment.search_space.parameters.keys())
         parameter_names = set(self.search_space.parameters.keys())
         if old_parameter_names.symmetric_difference(parameter_names):
             raise ValueError(  # pragma: no cover
                 f"Cannot warm-start experiment '{self._name}' from experiment "
                 f"'{old_experiment._name}' due to mismatch in search space parameters."
                 f"Parameters in '{self._name}' but not in '{old_experiment._name}': "
```

### Comparing `ax-platform-0.3.2/ax/core/formatting_utils.py` & `ax-platform-0.3.3/ax/core/formatting_utils.py`

 * *Files identical despite different names*

### Comparing `ax-platform-0.3.2/ax/core/generator_run.py` & `ax-platform-0.3.3/ax/core/generator_run.py`

 * *Files identical despite different names*

### Comparing `ax-platform-0.3.2/ax/core/map_data.py` & `ax-platform-0.3.3/ax/core/map_data.py`

 * *Files identical despite different names*

### Comparing `ax-platform-0.3.2/ax/core/map_metric.py` & `ax-platform-0.3.3/ax/core/map_metric.py`

 * *Files identical despite different names*

### Comparing `ax-platform-0.3.2/ax/core/metric.py` & `ax-platform-0.3.3/ax/core/metric.py`

 * *Files 4% similar despite different names*

```diff
@@ -104,84 +104,82 @@
             properties: Dictionary of this metric's properties
         """
         self._name = name
         self.lower_is_better = lower_is_better
         # pyre-fixme[4]: Attribute must be annotated.
         self.properties = properties or {}
 
+    # ---------- Properties and methods that subclasses often override. ----------
+
+    # NOTE: Override this if your metric can be fetched before the trial is complete,
+    # especially if new data is available over time while the trial continues running.
     @classmethod
     def is_available_while_running(cls) -> bool:
         """Whether metrics of this class are available while the trial is running.
         Metrics that are not available while the trial is running are assumed to be
         available only upon trial completion. For such metrics, data is assumed to
         never change once the trial is completed.
 
         NOTE: If this method returns `False`, data-fetching via `experiment.fetch_data`
         will return the data cached on the experiment (for the metrics of the given
         class) whenever its available. Data is cached on experiment when attached
         via `experiment.attach_data`.
         """
         return False
 
-    @property
-    def name(self) -> str:
-        """Get name of metric."""
-        return self._name
-
+    # NOTE: This is rarely overridden –– oonly if you want to fetch data in groups
+    # consisting of multiple different metric classes, for data to be fetched together.
+    # This makes sense only if `fetch_trial data_multi` or `fetch_experiment_data_multi`
+    # leverages fetching multiple metrics at once instead of fetching each serially,
+    # and that fetching logic is shared across the metric group.
     @property
     def fetch_multi_group_by_metric(self) -> Type[Metric]:
         """Metric class, with which to group this metric in
         `Experiment._metrics_by_class`, which is used to combine metrics on experiment
         into groups and then fetch their data via `Metric.fetch_trial_data_multi` for
         each group.
 
         NOTE: By default, this property will just return the class on which it is
         defined; however, in some cases it is useful to group metrics by their
         superclass, in which case this property should return that superclass.
         """
         return self.__class__
 
+    # NOTE: This is always overridden by subclasses, sometimes along with `fetch_trial_
+    # data_multi` and/or `fetch_experiment_data_multi`.`
     def fetch_trial_data(
         self, trial: core.base_trial.BaseTrial, **kwargs: Any
     ) -> MetricFetchResult:
         """Fetch data for one trial."""
         raise NotImplementedError(
             f"Metric {self.name} does not implement data-fetching logic."
         )  # pragma: no cover
 
-    def fetch_experiment_data(
-        self, experiment: core.experiment.Experiment, **kwargs: Any
-    ) -> Dict[int, MetricFetchResult]:
-        """Fetch this metric's data for an experiment.
-
-        Returns Dict of trial_index => Result
-        """
-
-        return {
-            trial.index: self.fetch_trial_data(trial=trial, **kwargs)
-            for trial in experiment.trials.values()
-            if trial.status.expecting_data
-        }
-
+    # NOTE: This should be overridden if there is a benefit to fetching multiple
+    # metrics that all share the `fetch_multi_group_by_metric` setting, at once.
+    # This gives an opportunity to perform a given operation (e.g. retrieve results
+    # of some remote job) only once, and then use the result to fetch each metric's
+    # value (via `fetch_trial_data` for that metric).
     @classmethod
     def fetch_trial_data_multi(
         cls, trial: core.base_trial.BaseTrial, metrics: Iterable[Metric], **kwargs: Any
     ) -> Dict[str, MetricFetchResult]:
         """Fetch multiple metrics data for one trial.
 
         Returns Dict of metric_name => Result
         Default behavior calls `fetch_trial_data` for each metric.
         Subclasses should override this to trial data computation for multiple metrics.
         """
-
         return {
             metric.name: metric.fetch_trial_data(trial=trial, **kwargs)
             for metric in metrics
         }
 
+    # NOTE: Same note as for `fetch_trial_data_multi`, except for the case where
+    # fetching data multiple trials is beneficial.
     @classmethod
     def fetch_experiment_data_multi(
         cls,
         experiment: core.experiment.Experiment,
         metrics: Iterable[Metric],
         trials: Optional[Iterable[core.base_trial.BaseTrial]] = None,
         **kwargs: Any,
@@ -197,14 +195,56 @@
             trial.index: cls.fetch_trial_data_multi(
                 trial=trial, metrics=metrics, **kwargs
             )
             for trial in (trials if trials is not None else experiment.trials.values())
             if trial.status.expecting_data
         }
 
+    # NOTE: Override this if your metric requires custom string representation with
+    # more attributes included than just the name.
+    def __repr__(self) -> str:
+        return "{class_name}('{metric_name}')".format(
+            class_name=self.__class__.__name__, metric_name=self.name
+        )
+
+    # NOTE: Also overridable are `serialize_init_args` and `deserialize_init_args`,
+    # which are inherited from the `SerializationMixin` base class.
+    # Override those iff your metric requires custom serialization; e.g. if
+    # some of its attributes are not readily serializable and require pre-processing.
+    # Note that all these serialized attributes will be deserialized by the
+    # `deserialize_init_args` method on the same class.
+
+    # ---------- Properties and methods that should not be overridden. ----------
+
+    @property
+    def name(self) -> str:
+        """Get name of metric."""
+        return self._name
+
+    def clone(self) -> Metric:
+        """Create a copy of this Metric."""
+        cls = type(self)
+        return cls(
+            **cls.deserialize_init_args(args=cls.serialize_init_args(obj=self)),
+        )
+
+    def fetch_experiment_data(
+        self, experiment: core.experiment.Experiment, **kwargs: Any
+    ) -> Dict[int, MetricFetchResult]:
+        """Fetch this metric's data for an experiment.
+
+        Returns Dict of trial_index => Result
+        """
+        return {
+            trial_index: results_by_metric_name[self.name]
+            for trial_index, results_by_metric_name in self.fetch_experiment_data_multi(
+                experiment, [self], **kwargs
+            ).items()
+        }
+
     @classmethod
     def lookup_or_fetch_experiment_data_multi(
         cls,
         experiment: core.experiment.Experiment,
         metrics: Iterable[Metric],
         trials: Optional[Iterable[core.base_trial.BaseTrial]] = None,
         **kwargs: Any,
@@ -270,14 +310,17 @@
                 )[trial.index]
 
                 contains_new_data = any(
                     result.is_ok() for result in fetched_trial_data.values()
                 )
             except NotImplementedError:
                 # Metric does not implement fetching logic and only uses lookup.
+                # TODO: This is only useful for base `Metric` –– all other metrics
+                # do implement fetching logic. Should this exist then or is it only
+                # adding complexity?
                 fetched_trial_data = {}
 
             trials_results[trial.index] = {
                 **cls._wrap_trial_data_multi(data=cached_trial_data),
                 **fetched_trial_data,
             }
 
@@ -289,26 +332,14 @@
                     if metric_name in [metric.name for metric in metrics]
                 }
                 for trial_index, results_by_metric_name in trials_results.items()
             },
             contains_new_data,
         )
 
-    def clone(self) -> Metric:
-        """Create a copy of this Metric."""
-        cls = type(self)
-        return cls(
-            **cls.deserialize_init_args(args=cls.serialize_init_args(obj=self)),
-        )
-
-    def __repr__(self) -> str:
-        return "{class_name}('{metric_name}')".format(
-            class_name=self.__class__.__name__, metric_name=self.name
-        )
-
     @property
     def _unique_id(self) -> str:
         return str(self)
 
     @classmethod
     def _unwrap_experiment_data(cls, results: Mapping[int, MetricFetchResult]) -> Data:
         # NOTE: This can be lossy (ex. a MapData could get implicitly cast to a Data and
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `ax-platform-0.3.2/ax/core/multi_type_experiment.py` & `ax-platform-0.3.3/ax/core/multi_type_experiment.py`

 * *Files identical despite different names*

### Comparing `ax-platform-0.3.2/ax/core/objective.py` & `ax-platform-0.3.3/ax/core/objective.py`

 * *Files identical despite different names*

### Comparing `ax-platform-0.3.2/ax/core/observation.py` & `ax-platform-0.3.3/ax/core/observation.py`

 * *Files identical despite different names*

### Comparing `ax-platform-0.3.2/ax/core/optimization_config.py` & `ax-platform-0.3.3/ax/core/optimization_config.py`

 * *Files identical despite different names*

### Comparing `ax-platform-0.3.2/ax/core/outcome_constraint.py` & `ax-platform-0.3.3/ax/core/outcome_constraint.py`

 * *Files identical despite different names*

### Comparing `ax-platform-0.3.2/ax/core/parameter.py` & `ax-platform-0.3.3/ax/core/parameter.py`

 * *Files 1% similar despite different names*

```diff
@@ -18,15 +18,15 @@
 from ax.utils.common.typeutils import not_none
 
 # Tolerance for floating point comparisons. This is relatively permissive,
 # and allows for serializing at rather low numerical precision.
 # TODO: Do a more comprehensive audit of how floating point precision issues
 # may creep up and implement a more principled fix
 EPS = 1.5e-7
-
+MAX_VALUES_CHOICE_PARAM = 1000
 FIXED_CHOICE_PARAM_ERROR = (
     "ChoiceParameters require multiple feasible values. "
     "Please use FixedParameter instead when setting a single possible value."
 )
 
 
 class ParameterType(Enum):
@@ -470,14 +470,20 @@
         self._is_task = is_task
         self._is_fidelity = is_fidelity
         # pyre-fixme[4]: Attribute must be annotated.
         self._target_value = self.cast(target_value)
         # A choice parameter with only one value is a FixedParameter.
         if not len(values) > 1:
             raise UserInputError(f"{self._name}({values}): {FIXED_CHOICE_PARAM_ERROR}")
+        # Cap the number of possible values
+        if len(values) > MAX_VALUES_CHOICE_PARAM:
+            raise UserInputError(
+                f"`ChoiceParameter` with more than {MAX_VALUES_CHOICE_PARAM} values "
+                "is not supported! Use a `RangeParameter` instead."
+            )
         # pyre-fixme[4]: Attribute must be annotated.
         self._values = self._cast_values(values)
         # pyre-fixme[4]: Attribute must be annotated.
         self._is_ordered = (
             is_ordered
             if is_ordered is not None
             else self._get_default_bool_and_warn(param_string="is_ordered")
```

### Comparing `ax-platform-0.3.2/ax/core/parameter_constraint.py` & `ax-platform-0.3.3/ax/core/parameter_constraint.py`

 * *Files identical despite different names*

### Comparing `ax-platform-0.3.2/ax/core/parameter_distribution.py` & `ax-platform-0.3.3/ax/core/parameter_distribution.py`

 * *Files identical despite different names*

### Comparing `ax-platform-0.3.2/ax/core/risk_measures.py` & `ax-platform-0.3.3/ax/core/risk_measures.py`

 * *Files identical despite different names*

### Comparing `ax-platform-0.3.2/ax/core/runner.py` & `ax-platform-0.3.3/ax/core/runner.py`

 * *Files 4% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 #
 # This source code is licensed under the MIT license found in the
 # LICENSE file in the root directory of this source tree.
 
 from __future__ import annotations
 
 from abc import ABC, abstractmethod
-from typing import Any, Dict, Iterable, Optional, Set, TYPE_CHECKING
+from typing import Any, Dict, Iterable, List, Optional, Set, TYPE_CHECKING
 
 from ax.utils.common.base import Base
 from ax.utils.common.serialization import SerializationMixin
 
 
 if TYPE_CHECKING:  # pragma: no cover
     # import as module to make sphinx-autodoc-typehints happy
@@ -22,14 +22,21 @@
     """Abstract base class for custom runner classes"""
 
     @property
     def staging_required(self) -> bool:
         """Whether the trial goes to staged or running state once deployed."""
         return False
 
+    @property
+    def run_metadata_report_keys(self) -> List[str]:
+        """A list of keys of the metadata dict returned by `run()` that are
+        relevant outside the runner-internal impolementation. These can e.g.
+        be reported in `Scheduler.report_results()`."""
+        return []
+
     @abstractmethod
     def run(self, trial: core.base_trial.BaseTrial) -> Dict[str, Any]:
         """Deploys a trial based on custom runner subclass implementation.
 
         Args:
             trial: The trial to deploy.
```

### Comparing `ax-platform-0.3.2/ax/core/search_space.py` & `ax-platform-0.3.3/ax/core/search_space.py`

 * *Files 1% similar despite different names*

```diff
@@ -690,15 +690,15 @@
     @property
     def height(self) -> int:
         """
         Height of the underlying tree structure of this hierarchical search space.
         """
 
         def _height_from_parameter(parameter: Parameter) -> int:
-            if len(parameter.dependents) == 0:
+            if not parameter.is_hierarchical:
                 return 1
 
             return (
                 max(
                     _height_from_parameter(parameter=self[param_name])
                     for deps in parameter.dependents.values()
                     for param_name in deps
```

### Comparing `ax-platform-0.3.2/ax/core/tests/test_arm.py` & `ax-platform-0.3.3/ax/core/tests/test_arm.py`

 * *Files identical despite different names*

### Comparing `ax-platform-0.3.2/ax/core/tests/test_batch_trial.py` & `ax-platform-0.3.3/ax/core/tests/test_batch_trial.py`

 * *Files identical despite different names*

### Comparing `ax-platform-0.3.2/ax/core/tests/test_data.py` & `ax-platform-0.3.3/ax/core/tests/test_data.py`

 * *Files identical despite different names*

### Comparing `ax-platform-0.3.2/ax/core/tests/test_experiment.py` & `ax-platform-0.3.3/ax/core/tests/test_experiment.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 #!/usr/bin/env python3
 # Copyright (c) Meta Platforms, Inc. and affiliates.
 #
 # This source code is licensed under the MIT license found in the
 # LICENSE file in the root directory of this source tree.
 
 import logging
-from typing import Dict, Type
+from typing import Dict, List, Type
 from unittest.mock import patch
 
 import pandas as pd
 from ax.core import BatchTrial, Trial
 from ax.core.arm import Arm
 from ax.core.base_trial import TrialStatus
 from ax.core.data import Data
@@ -47,14 +47,20 @@
 DUMMY_RUN_METADATA_KEY = "test_run_metadata_key"
 DUMMY_RUN_METADATA_VALUE = "test_run_metadata_value"
 DUMMY_RUN_METADATA: Dict[str, str] = {DUMMY_RUN_METADATA_KEY: DUMMY_RUN_METADATA_VALUE}
 DUMMY_ABANDONED_REASON = "test abandoned reason"
 DUMMY_ARM_NAME = "test_arm_name"
 
 
+class SyntheticRunnerWithMetadataKeys(SyntheticRunner):
+    @property
+    def run_metadata_report_keys(self) -> List[str]:
+        return [DUMMY_RUN_METADATA_KEY]
+
+
 class ExperimentTest(TestCase):
     def setUp(self) -> None:
         self.experiment = get_experiment()
 
     def _setupBraninExperiment(self, n: int) -> Experiment:
         exp = Experiment(
             name="test3",
@@ -444,28 +450,33 @@
         # Test retrieving original batch 0 data
         self.assertEqual(len(exp.lookup_data_for_ts(t1).df), n)
         self.assertEqual(len(exp.lookup_data_for_trial(0)[0].df), n)
 
         # Test retrieving full exp data
         self.assertEqual(len(exp.lookup_data_for_ts(t2).df), 4 * n)
 
-        with self.assertRaisesRegex(ValueError, ".* for metric"):
-            exp.attach_data(batch_data, combine_with_last_data=True)
-
         self.assertEqual(len(full_dict[0]), 5)  # 5 data objs for batch 0
         new_data = Data(
             df=pd.DataFrame.from_records(
                 [
                     {
                         "arm_name": "0_0",
+                        # but now it is
+                        "metric_name": "not_yet_on_experiment",
+                        "mean": 3,
+                        "sem": 0,
+                        "trial_index": 0,
+                    },
+                    {
+                        "arm_name": "0_0",
                         "metric_name": "z",
                         "mean": 3,
                         "sem": 0,
                         "trial_index": 0,
-                    }
+                    },
                 ]
             )
         )
         t3 = exp.attach_data(new_data, combine_with_last_data=True)
         # still 5 data objs, since we combined last one
         self.assertEqual(len(full_dict[0]), 5)
         self.assertIn("z", exp.lookup_data_for_ts(t3).df["metric_name"].tolist())
@@ -826,14 +837,15 @@
     def testWarmStartFromOldExperiment(self) -> None:
         # create old_experiment
         len_old_trials = 7
         i_failed_trial = 1
         i_abandoned_trial = 3
         i_running_trial = 5
         old_experiment = get_branin_experiment()
+        old_experiment.runner = SyntheticRunnerWithMetadataKeys()
         for i_old_trial in range(len_old_trials):
             sobol_run = get_sobol(search_space=old_experiment.search_space).gen(n=1)
             trial = old_experiment.new_trial(generator_run=sobol_run)
             trial.mark_running(no_runner_required=True)
             if i_old_trial == i_failed_trial:
                 trial.mark_failed()
             elif i_old_trial == i_abandoned_trial:
@@ -863,15 +875,14 @@
         new_experiment.optimization_config.objective.metric.noise_sd = 0
         for _, trial in old_experiment.trials.items():
             trial._run_metadata = DUMMY_RUN_METADATA
         # name one arm to test name-preserving logic.
         old_experiment.trials[0].arm._name = DUMMY_ARM_NAME
         new_experiment.warm_start_from_old_experiment(
             old_experiment=old_experiment,
-            copy_run_metadata_keys=[DUMMY_RUN_METADATA_KEY],
         )
         self.assertEqual(len(new_experiment.trials), len(old_experiment.trials) - 1)
         i_old_trial = 0
         for idx, trial in new_experiment.trials.items():
             # skip failed trial
             i_old_trial += i_old_trial == i_failed_trial
             # pyre-fixme[16]: `BaseTrial` has no attribute `arm`.
```

### Comparing `ax-platform-0.3.2/ax/core/tests/test_formatting_utils.py` & `ax-platform-0.3.3/ax/core/tests/test_formatting_utils.py`

 * *Files identical despite different names*

### Comparing `ax-platform-0.3.2/ax/core/tests/test_generator_run.py` & `ax-platform-0.3.3/ax/core/tests/test_generator_run.py`

 * *Files identical despite different names*

### Comparing `ax-platform-0.3.2/ax/core/tests/test_map_data.py` & `ax-platform-0.3.3/ax/core/tests/test_map_data.py`

 * *Files identical despite different names*

### Comparing `ax-platform-0.3.2/ax/core/tests/test_map_metric.py` & `ax-platform-0.3.3/ax/core/tests/test_map_metric.py`

 * *Files identical despite different names*

### Comparing `ax-platform-0.3.2/ax/core/tests/test_metric.py` & `ax-platform-0.3.3/ax/core/tests/test_metric.py`

 * *Files identical despite different names*

### Comparing `ax-platform-0.3.2/ax/core/tests/test_multi_type_experiment.py` & `ax-platform-0.3.3/ax/core/tests/test_multi_type_experiment.py`

 * *Files identical despite different names*

### Comparing `ax-platform-0.3.2/ax/core/tests/test_objective.py` & `ax-platform-0.3.3/ax/core/tests/test_objective.py`

 * *Files identical despite different names*

### Comparing `ax-platform-0.3.2/ax/core/tests/test_observation.py` & `ax-platform-0.3.3/ax/core/tests/test_observation.py`

 * *Files identical despite different names*

### Comparing `ax-platform-0.3.2/ax/core/tests/test_optimization_config.py` & `ax-platform-0.3.3/ax/core/tests/test_optimization_config.py`

 * *Files identical despite different names*

### Comparing `ax-platform-0.3.2/ax/core/tests/test_outcome_constraint.py` & `ax-platform-0.3.3/ax/core/tests/test_outcome_constraint.py`

 * *Files identical despite different names*

### Comparing `ax-platform-0.3.2/ax/core/tests/test_parameter.py` & `ax-platform-0.3.3/ax/core/tests/test_parameter.py`

 * *Files 1% similar despite different names*

```diff
@@ -311,14 +311,31 @@
                 parameter_type=ParameterType.BOOL,
                 values=[True, False],
                 # pyre-fixme[6]: For 4th param expected `Optional[Dict[Union[None,
                 #  bool, float, int, str], List[str]]]` but got `Dict[str, str]`.
                 dependents={"not_a_value": "other_param"},
             )
 
+    def testMaxValuesValidation(self) -> None:
+        ChoiceParameter(
+            name="x",
+            parameter_type=ParameterType.INT,
+            values=list(range(999)),  # pyre-ignore
+        )
+        with self.assertRaisesRegex(
+            UserInputError,
+            "`ChoiceParameter` with more than 1000 values is not supported! Use a "
+            "`RangeParameter` instead.",
+        ):
+            ChoiceParameter(
+                name="x",
+                parameter_type=ParameterType.INT,
+                values=list(range(1001)),  # pyre-ignore
+            )
+
     def testHierarchical(self) -> None:
         # Test case where only some of the values entail dependents.
         hierarchical_param = ChoiceParameter(
             name="x",
             parameter_type=ParameterType.BOOL,
             values=[True, False],
             # pyre-fixme[6]: For 4th param expected `Optional[Dict[Union[None, bool,
```

### Comparing `ax-platform-0.3.2/ax/core/tests/test_parameter_constraint.py` & `ax-platform-0.3.3/ax/core/tests/test_parameter_constraint.py`

 * *Files identical despite different names*

### Comparing `ax-platform-0.3.2/ax/core/tests/test_parameter_distribution.py` & `ax-platform-0.3.3/ax/core/tests/test_parameter_distribution.py`

 * *Files identical despite different names*

### Comparing `ax-platform-0.3.2/ax/core/tests/test_risk_measures.py` & `ax-platform-0.3.3/ax/core/tests/test_risk_measures.py`

 * *Files identical despite different names*

### Comparing `ax-platform-0.3.2/ax/core/tests/test_runner.py` & `ax-platform-0.3.3/ax/core/tests/test_runner.py`

 * *Files 4% similar despite different names*

```diff
@@ -45,7 +45,10 @@
 
     def test_base_runner_poll_trial_status(self) -> None:
         with self.assertRaises(NotImplementedError):
             self.dummy_runner.poll_trial_status(trials=self.trials)
 
     def test_poll_available_capacity(self) -> None:
         self.assertEqual(self.dummy_runner.poll_available_capacity(), -1)
+
+    def test_run_metadata_report_keys(self) -> None:
+        self.assertEqual(self.dummy_runner.run_metadata_report_keys, [])
```

### Comparing `ax-platform-0.3.2/ax/core/tests/test_search_space.py` & `ax-platform-0.3.3/ax/core/tests/test_search_space.py`

 * *Files identical despite different names*

### Comparing `ax-platform-0.3.2/ax/core/tests/test_trial.py` & `ax-platform-0.3.3/ax/core/tests/test_trial.py`

 * *Files identical despite different names*

### Comparing `ax-platform-0.3.2/ax/core/tests/test_utils.py` & `ax-platform-0.3.3/ax/core/tests/test_utils.py`

 * *Files identical despite different names*

### Comparing `ax-platform-0.3.2/ax/core/trial.py` & `ax-platform-0.3.3/ax/core/trial.py`

 * *Files 2% similar despite different names*

```diff
@@ -12,18 +12,22 @@
 
 from typing import Any, Dict, List, Optional, TYPE_CHECKING, Union
 
 from ax.core.arm import Arm
 from ax.core.base_trial import BaseTrial, immutable_once_run
 from ax.core.data import Data
 from ax.core.generator_run import GeneratorRun, GeneratorRunType
-from ax.core.types import TCandidateMetadata, TEvaluationOutcome
+from ax.core.types import (
+    TCandidateMetadata,
+    TEvaluationOutcome,
+    validate_evaluation_outcome,
+)
 from ax.utils.common.docutils import copy_doc
 from ax.utils.common.logger import _round_floats_for_logging, get_logger
-from ax.utils.common.typeutils import checked_cast_complex, not_none
+from ax.utils.common.typeutils import not_none
 
 logger: Logger = get_logger(__name__)
 
 TRIAL_RAW_DATA_FORMAT_ERROR_MESSAGE = (
     "Raw data must be data for a single arm for non batched trials."
 )
 
@@ -290,21 +294,19 @@
     ) -> str:
         """Utility method that attaches data to a trial,
         returns a str of the update."""
         # Format the data to save.
         sample_sizes = {not_none(self.arm).name: sample_size} if sample_size else {}
 
         arm_name = not_none(self.arm).name
-        raw_data_by_arm = {
-            arm_name: checked_cast_complex(
-                TEvaluationOutcome,
-                raw_data,
-                message=TRIAL_RAW_DATA_FORMAT_ERROR_MESSAGE,
-            )
-        }
+        try:
+            validate_evaluation_outcome(outcome=raw_data)
+        except Exception:
+            raise ValueError(TRIAL_RAW_DATA_FORMAT_ERROR_MESSAGE)
+        raw_data_by_arm = {arm_name: raw_data}
         not_trial_arm_names = set(raw_data_by_arm.keys()) - set(
             self.arms_by_name.keys()
         )
         if not_trial_arm_names:
             raise ValueError(  # pragma: no cover
                 f"Arms {not_trial_arm_names} are not part of trial #{self.index}."
             )
```

### Comparing `ax-platform-0.3.2/ax/core/utils.py` & `ax-platform-0.3.3/ax/core/utils.py`

 * *Files identical despite different names*

### Comparing `ax-platform-0.3.2/ax/early_stopping/strategies/__init__.py` & `ax-platform-0.3.3/ax/early_stopping/strategies/__init__.py`

 * *Files identical despite different names*

### Comparing `ax-platform-0.3.2/ax/early_stopping/strategies/base.py` & `ax-platform-0.3.3/ax/early_stopping/strategies/base.py`

 * *Files identical despite different names*

### Comparing `ax-platform-0.3.2/ax/early_stopping/strategies/logical.py` & `ax-platform-0.3.3/ax/early_stopping/strategies/logical.py`

 * *Files identical despite different names*

### Comparing `ax-platform-0.3.2/ax/early_stopping/strategies/percentile.py` & `ax-platform-0.3.3/ax/early_stopping/strategies/percentile.py`

 * *Files identical despite different names*

### Comparing `ax-platform-0.3.2/ax/early_stopping/strategies/threshold.py` & `ax-platform-0.3.3/ax/early_stopping/strategies/threshold.py`

 * *Files identical despite different names*

### Comparing `ax-platform-0.3.2/ax/early_stopping/tests/test_strategies.py` & `ax-platform-0.3.3/ax/early_stopping/tests/test_strategies.py`

 * *Files identical despite different names*

### Comparing `ax-platform-0.3.2/ax/early_stopping/utils.py` & `ax-platform-0.3.3/ax/early_stopping/utils.py`

 * *Files identical despite different names*

### Comparing `ax-platform-0.3.2/ax/exceptions/constants.py` & `ax-platform-0.3.3/ax/exceptions/constants.py`

 * *Files identical despite different names*

### Comparing `ax-platform-0.3.2/ax/exceptions/core.py` & `ax-platform-0.3.3/ax/exceptions/core.py`

 * *Files identical despite different names*

### Comparing `ax-platform-0.3.2/ax/exceptions/data_provider.py` & `ax-platform-0.3.3/ax/exceptions/data_provider.py`

 * *Files identical despite different names*

### Comparing `ax-platform-0.3.2/ax/exceptions/generation_strategy.py` & `ax-platform-0.3.3/ax/exceptions/generation_strategy.py`

 * *Files identical despite different names*

### Comparing `ax-platform-0.3.2/ax/exceptions/storage.py` & `ax-platform-0.3.3/ax/exceptions/storage.py`

 * *Files identical despite different names*

### Comparing `ax-platform-0.3.2/ax/global_stopping/strategies/base.py` & `ax-platform-0.3.3/ax/global_stopping/strategies/base.py`

 * *Files 15% similar despite different names*

```diff
@@ -3,14 +3,15 @@
 #
 # This source code is licensed under the MIT license found in the
 # LICENSE file in the root directory of this source tree.
 
 from abc import ABC, abstractmethod
 from typing import Any, Tuple
 
+from ax.core.base_trial import TrialStatus
 from ax.core.experiment import Experiment
 from ax.utils.common.base import Base
 
 
 class BaseGlobalStoppingStrategy(ABC, Base):
     """Interface for strategies used to stop the optimization.
 
@@ -34,25 +35,50 @@
             inactive_when_pending_trials: If set, the optimization will not stopped as
                 long as it has running trials.
         """
         self.min_trials = min_trials
         self.inactive_when_pending_trials = inactive_when_pending_trials
 
     @abstractmethod
+    def _should_stop_optimization(
+        self, experiment: Experiment, **kwargs: Any
+    ) -> Tuple[bool, str]:
+        """
+        Decide whether to stop optimization.
+
+        Must be implemented by the subclass. Typical examples include stopping
+        the optimization loop when the objective appears to not improve anymore.
+
+        Args:
+            experiment: Experiment that contains the trials and other contextual data.
+
+        Returns:
+            A Tuple with a boolean determining whether the optimization should stop,
+            and a str declaring the reason for stopping.
+        """
+
     def should_stop_optimization(
         self,
         experiment: Experiment,
         **kwargs: Any,
     ) -> Tuple[bool, str]:
         """Decide whether to stop optimization.
 
-        Typical examples include stopping the optimization loop when the objective
-        appears to not improve anymore.
-
         Args:
             experiment: Experiment that contains the trials and other contextual data.
 
         Returns:
             A Tuple with a boolean determining whether the optimization should stop,
             and a str declaring the reason for stopping.
         """
-        pass  # pragma: nocover
+        if (
+            self.inactive_when_pending_trials
+            and len(experiment.trials_by_status[TrialStatus.RUNNING]) > 0
+        ):
+            message = "There are pending trials in the experiment."
+            return False, message
+
+        if len(experiment.trials_by_status[TrialStatus.COMPLETED]) == 0:
+            message = "There are no completed trials yet."
+            return False, message
+
+        return self._should_stop_optimization(experiment, **kwargs)
```

### Comparing `ax-platform-0.3.2/ax/global_stopping/strategies/improvement.py` & `ax-platform-0.3.3/ax/global_stopping/strategies/improvement.py`

 * *Files 7% similar despite different names*

```diff
@@ -27,85 +27,87 @@
 
 
 logger: Logger = get_logger(__name__)
 
 
 class ImprovementGlobalStoppingStrategy(BaseGlobalStoppingStrategy):
     """
-    A stopping strategy which stops the optimization if there is no significant
-    improvement over the iterations. For single-objective optimizations, this
-    strategy stops the loop if the feasible (mean) objective has not improved
-    over the past "window_size" iterations. In MOO loops, it stops the optimization
-    loop if the hyper-volume of the pareto front has not improved in the past
-    "window_size" iterations.
+    A Global Stopping Strategy which recommends stopping optimization if there
+    is no significant improvement over recent iterations.
+
+    This stopping strategy recommends stopping if there is no significant improvement
+    over the past `window_size` trials, among those that are feasible
+    (satisfying constraints). The meaning of a "significant"
+    improvement differs between single-objective and multi-objective optimizations.
+    For single-objective optimizations, improvement is as a fraction of the
+    interquartile range (IQR) of the objective values seen so far. For
+    multi-objective optimizations (MOO), improvement is as a fraction of the hypervolume
+    obtained `window_size` iterations ago.
     """
 
     def __init__(
         self,
         min_trials: int,
         window_size: int = 5,
         improvement_bar: float = 0.1,
         inactive_when_pending_trials: bool = True,
     ) -> None:
         """
         Initialize an improvement-based stopping strategy.
 
         Args:
-            min_trials: Minimum number of trials before the stopping strategy kicks in.
+            min_trials: Minimum number of trials before the stopping strategy
+                kicks in.
             window_size: Number of recent trials to check the improvement in.
+                The first trial that could be used for analysis is
+                `min_trials - window_size`; the first trial for which stopping
+                might be recommended is `min_trials`.
             improvement_bar: Threshold (in [0,1]) for considering relative improvement
                 over the best point.
             inactive_when_pending_trials: If set, the optimization will not stopped as
                 long as it has running trials.
         """
         super().__init__(
             min_trials=min_trials,
             inactive_when_pending_trials=inactive_when_pending_trials,
         )
         self.window_size = window_size
         self.improvement_bar = improvement_bar
         self.hv_by_trial: Dict[int, float] = {}
 
-    def should_stop_optimization(
+    def _should_stop_optimization(
         self,
         experiment: Experiment,
         trial_to_check: Optional[int] = None,
         objective_thresholds: Optional[List[ObjectiveThreshold]] = None,
         **kwargs: Dict[str, Any],
     ) -> Tuple[bool, str]:
         """
-        Check if the optimization has improved in the past "window_size" iterations.
+        Check if the objective has improved significantly in the past
+        "window_size" iterations.
+
         For single-objective optimization experiments, it will call
         _should_stop_single_objective() and for MOO experiments, it will call
         _should_stop_moo(). Before making either of these calls, this function carries
-        out some sanity checks to handle obvious/invalid cases.
+        out some sanity checks to handle obvious/invalid cases. For more detail
+        on what it means to "significantly" improve, see the class docstring.
 
         Args:
             experiment: The experiment to apply the strategy on.
             trial_to_check: The trial in the experiment at which we want to check
                 for stopping. If None, we check at the latest trial.
             objective_thresholds: Custom objective thresholds to use as reference pooint
                 when computing hv of the pareto front against. This is used only in the
                 MOO setting. If not specified, the objective thresholds on the
                 experiment's optimization config will be used for the purpose.
 
         Returns:
             A Tuple with a boolean determining whether the optimization should stop,
             and a str declaring the reason for stopping.
         """
-        if (
-            self.inactive_when_pending_trials
-            and len(experiment.trials_by_status[TrialStatus.RUNNING]) > 0
-        ):
-            message = "There are pending trials in the experiment."
-            return False, message
-
-        if len(experiment.trials_by_status[TrialStatus.COMPLETED]) == 0:
-            message = "There are no completed trials yet."
-            return False, message
 
         max_completed_trial = max(
             experiment.trial_indices_by_status[TrialStatus.COMPLETED]
         )
 
         if trial_to_check is None:
             trial_to_check = max_completed_trial
@@ -143,18 +145,26 @@
     def _should_stop_moo(
         self,
         experiment: Experiment,
         trial_to_check: int,
         objective_thresholds: Optional[List[ObjectiveThreshold]] = None,
     ) -> Tuple[bool, str]:
         """
-        This is just the "should_stop_optimization" method of the class specialized to
-        MOO experiments. It computes the (feasible) hypervolume of the pareto front at
-        "trial_to_check" trial and "window_size" trials before, and suggest to stop the
-        optimization if there is no significant improvement.
+        This is the "should_stop_optimization" method of this class, specialized
+        to MOO experiments.
+
+        It computes the (feasible) hypervolume of the Pareto front at
+        `trial_to_check` trial and `window_size` trials before, and suggest to stop the
+        optimization if the improvment in hypervolume over the past
+        `window_size` trials, as a fraction of the hypervolume at the start of
+        the window, is less than `self.improvement_bar`. When the hypervolume is
+        zero at the beginning of the window, stopping is never recommended.
+
+        Becaues hypervolume computations are expensive, these are stored to
+        increase the speed of future checks.
 
         Args:
             experiment: The experiment to apply the strategy on.
             trial_to_check: The trial in the experiment at which we want to check
                 for stopping. If None, we check at the latest trial.
             objective_thresholds: Custom objective thresholds to use as reference pooint
                 when computing hv of the pareto front against. This is used only in the
@@ -200,28 +210,33 @@
 
         hv_improvement = (hv - hv_reference) / hv_reference
         stop = hv_improvement < self.improvement_bar
 
         if stop:
             message = (
                 f"The improvement in hypervolume in the past {self.window_size} "
-                f"trials (={hv_improvement:.3f}) is less than {self.improvement_bar}."
+                f"trials (={hv_improvement:.3f}) is less than improvement_bar "
+                f"(={self.improvement_bar}) times the hypervolume at the start "
+                f"of the window (={hv_reference:.3f})."
             )
         else:
             message = ""
         return stop, message
 
     def _should_stop_single_objective(
         self, experiment: Experiment, trial_to_check: int
     ) -> Tuple[bool, str]:
         """
-        This is the "should_stop_optimization" method of the class specialized to
-        single-objective experiments. It computes the best feasible objective  at
-        "trial_to_check" trial and "window_size" trials before, and suggest to stop
-        the trial if there is no significant improvement.
+        This is the `_should_stop_optimization` method of this class,
+        specialized to single-objective experiments.
+
+        It computes the interquartile range (IQR) of feasible objective values
+        found so far, then computes the improvement in the best seen over the
+        last `window_size` trials. If the recent improvement as a fraction of
+        the IQR is less than `self.improvement_bar`, it recommends stopping.
 
         Args:
             experiment: The experiment to apply the strategy on.
             trial_to_check: The trial in the experiment at which we want to check
                 for stopping. If None, we check at the latest trial.
 
         Returns:
@@ -261,15 +276,16 @@
         )
         stop = relative_improvement < self.improvement_bar
 
         if stop:
             message = (
                 f"The improvement in best objective in the past {self.window_size} "
                 f"trials (={relative_improvement:.3f}) is less than "
-                f"{self.improvement_bar}."
+                f"{self.improvement_bar} times the interquartile range (IQR) of "
+                f"objectives attained so far (IQR={iqr:.3f})."
             )
         else:
             message = ""
 
         return stop, message
```

### Comparing `ax-platform-0.3.2/ax/global_stopping/tests/tests_strategies.py` & `ax-platform-0.3.3/ax/global_stopping/tests/tests_strategies.py`

 * *Files 2% similar despite different names*

```diff
@@ -267,18 +267,20 @@
         )
         stop, message = gss.should_stop_optimization(experiment=exp, trial_to_check=4)
         self.assertFalse(stop)
         self.assertEqual(message, "")
 
         stop, message = gss.should_stop_optimization(experiment=exp, trial_to_check=5)
         self.assertTrue(stop)
+
         self.assertEqual(
             message,
-            "The improvement in hypervolume in the past 3 trials (=0.000) is less than "
-            "0.1.",
+            "The improvement in hypervolume in the past 3 trials (=0.000) is "
+            "less than improvement_bar (=0.1) times the hypervolume at the "
+            "start of the window (=0.055).",
         )
 
         # Now we select a very far custom reference point against which the pareto front
         # has not increased in hypervolume at trial 4. Hence, it should stop the
         # optimization at this trial.
         gss = ImprovementGlobalStoppingStrategy(
             min_trials=3, window_size=3, improvement_bar=0.1
@@ -302,16 +304,17 @@
             experiment=exp,
             trial_to_check=4,
             objective_thresholds=custom_objective_thresholds,
         )
         self.assertTrue(stop)
         self.assertEqual(
             message,
-            "The improvement in hypervolume in the past 3 trials (=0.033) is less than "
-            "0.1.",
+            "The improvement in hypervolume in the past 3 trials (=0.033) is "
+            "less than improvement_bar (=0.1) times the hypervolume at the "
+            "start of the window (=108.640).",
         )
 
         # Test with no objective thresholds specified.
         checked_cast(
             MultiObjectiveOptimizationConfig, exp._optimization_config
         )._objective_thresholds = []
         stop, message = gss.should_stop_optimization(
@@ -339,15 +342,16 @@
         self.assertEqual(message, "")
 
         top, message = gss.should_stop_optimization(experiment=exp, trial_to_check=5)
         self.assertFalse(stop)
         self.assertEqual(
             message,
             "The improvement in best objective in the past 3 trials (=0.000) is "
-            "less than 0.1.",
+            "less than 0.1 times the interquartile range (IQR) of objectives "
+            "attained so far (IQR=0.100).",
         )
 
     def test_safety_check(self) -> None:
         experiment = get_experiment()
         gss = ImprovementGlobalStoppingStrategy(min_trials=2, window_size=3)
 
         stop, message = gss.should_stop_optimization(experiment=experiment)
```

### Comparing `ax-platform-0.3.2/ax/metrics/botorch_test_problem.py` & `ax-platform-0.3.3/ax/metrics/botorch_test_problem.py`

 * *Files identical despite different names*

### Comparing `ax-platform-0.3.2/ax/metrics/branin.py` & `ax-platform-0.3.3/ax/metrics/branin.py`

 * *Files identical despite different names*

### Comparing `ax-platform-0.3.2/ax/metrics/branin_map.py` & `ax-platform-0.3.3/ax/metrics/branin_map.py`

 * *Files identical despite different names*

### Comparing `ax-platform-0.3.2/ax/metrics/chemistry.py` & `ax-platform-0.3.3/ax/metrics/chemistry.py`

 * *Files identical despite different names*

### Comparing `ax-platform-0.3.2/ax/metrics/chemistry_data.zip` & `ax-platform-0.3.3/ax/metrics/chemistry_data.zip`

 * *Files identical despite different names*

### Comparing `ax-platform-0.3.2/ax/metrics/curve.py` & `ax-platform-0.3.3/ax/metrics/curve.py`

 * *Files identical despite different names*

### Comparing `ax-platform-0.3.2/ax/metrics/dict_lookup.py` & `ax-platform-0.3.3/ax/metrics/dict_lookup.py`

 * *Files identical despite different names*

### Comparing `ax-platform-0.3.2/ax/metrics/factorial.py` & `ax-platform-0.3.3/ax/metrics/factorial.py`

 * *Files identical despite different names*

### Comparing `ax-platform-0.3.2/ax/metrics/hartmann6.py` & `ax-platform-0.3.3/ax/metrics/hartmann6.py`

 * *Files identical despite different names*

### Comparing `ax-platform-0.3.2/ax/metrics/jenatton.py` & `ax-platform-0.3.3/ax/metrics/jenatton.py`

 * *Files identical despite different names*

### Comparing `ax-platform-0.3.2/ax/metrics/noisy_function.py` & `ax-platform-0.3.3/ax/metrics/noisy_function.py`

 * *Files identical despite different names*

### Comparing `ax-platform-0.3.2/ax/metrics/noisy_function_map.py` & `ax-platform-0.3.3/ax/metrics/noisy_function_map.py`

 * *Files identical despite different names*

### Comparing `ax-platform-0.3.2/ax/metrics/sklearn.py` & `ax-platform-0.3.3/ax/metrics/sklearn.py`

 * *Files identical despite different names*

### Comparing `ax-platform-0.3.2/ax/metrics/tensorboard.py` & `ax-platform-0.3.3/ax/metrics/tensorboard.py`

 * *Files identical despite different names*

### Comparing `ax-platform-0.3.2/ax/metrics/tests/test_chemistry.py` & `ax-platform-0.3.3/ax/metrics/tests/test_chemistry.py`

 * *Files identical despite different names*

### Comparing `ax-platform-0.3.2/ax/metrics/tests/test_curve.py` & `ax-platform-0.3.3/ax/metrics/tests/test_curve.py`

 * *Files identical despite different names*

### Comparing `ax-platform-0.3.2/ax/metrics/tests/test_dict_lookup.py` & `ax-platform-0.3.3/ax/metrics/tests/test_dict_lookup.py`

 * *Files identical despite different names*

### Comparing `ax-platform-0.3.2/ax/metrics/tests/test_noisy_function.py` & `ax-platform-0.3.3/ax/metrics/tests/test_noisy_function.py`

 * *Files identical despite different names*

### Comparing `ax-platform-0.3.2/ax/metrics/tests/test_sklearn.py` & `ax-platform-0.3.3/ax/metrics/tests/test_sklearn.py`

 * *Files identical despite different names*

### Comparing `ax-platform-0.3.2/ax/metrics/tests/test_tensorboard.py` & `ax-platform-0.3.3/ax/metrics/tests/test_tensorboard.py`

 * *Files identical despite different names*

### Comparing `ax-platform-0.3.2/ax/metrics/torchx.py` & `ax-platform-0.3.3/ax/metrics/torchx.py`

 * *Files identical despite different names*

### Comparing `ax-platform-0.3.2/ax/modelbridge/__init__.py` & `ax-platform-0.3.3/ax/modelbridge/__init__.py`

 * *Files identical despite different names*

### Comparing `ax-platform-0.3.2/ax/modelbridge/base.py` & `ax-platform-0.3.3/ax/modelbridge/base.py`

 * *Files 4% similar despite different names*

```diff
@@ -8,16 +8,17 @@
 import warnings
 from abc import ABC
 from collections import OrderedDict
 from copy import deepcopy
 from dataclasses import dataclass, field
 
 from logging import Logger
-from typing import Any, Dict, List, MutableMapping, Optional, Set, Tuple, Type
+from typing import Any, cast, Dict, List, MutableMapping, Optional, Set, Tuple, Type
 
+import numpy as np
 from ax.core.arm import Arm
 from ax.core.data import Data
 from ax.core.experiment import Experiment
 from ax.core.generator_run import extract_arm_predictions, GeneratorRun
 from ax.core.observation import (
     Observation,
     ObservationData,
@@ -32,14 +33,21 @@
 from ax.core.types import TCandidateMetadata, TModelCov, TModelMean, TModelPredict
 from ax.exceptions.core import UserInputError
 from ax.modelbridge.transforms.base import Transform
 from ax.modelbridge.transforms.cast import Cast
 from ax.models.types import TConfig
 from ax.utils.common.logger import get_logger
 from ax.utils.common.typeutils import checked_cast, not_none
+from ax.utils.stats.model_fit_stats import (
+    coefficient_of_determination,
+    compute_model_fit_metrics,
+    mean_of_the_standardized_error,
+    ModelFitMetricProtocol,
+    std_of_the_standardized_error,
+)
 from botorch.exceptions.warnings import InputDataWarning
 
 logger: Logger = get_logger(__name__)
 
 
 @dataclass(frozen=True)
 class BaseGenArgs:
@@ -914,14 +922,59 @@
         cv_test_points: List[ObservationFeatures],
     ) -> List[ObservationData]:
         """Apply the terminal transform, make predictions on the test points,
         and reverse terminal transform on the results.
         """
         raise NotImplementedError  # pragma: no cover
 
+    def compute_model_fit_metrics(
+        self,
+        experiment: Experiment,
+        fit_metrics_dict: Optional[Dict[str, ModelFitMetricProtocol]] = None,
+    ) -> Dict[str, Dict[str, float]]:
+        """Computes the model fit metrics from the scheduler state.
+
+        Args:
+            experiment: The experiment with whose data to compute the model fit metrics.
+            fit_metrics_dict: An optional dictionary with model fit metric functions,
+            i.e. a ModelFitMetricProtocol, as values and their names as keys.
+
+        Returns:
+            A nested dictionary mapping from the *model fit* metric names and the
+            *experimental metric* names to the values of the model fit metrics.
+
+            Example for an imaginary AutoML experiment that seeks to minimize the test
+            error after training an expensive model, with respect to hyper-parameters:
+
+            ```
+            model_fit_dict = model_fit_metrics_from_scheduler(scheduler)
+            model_fit_dict["coefficient_of_determination"]["test error"] =
+                `coefficient of determination of the test error predictions`
+            ```
+        """
+        # TODO: cross_validate_by_trial-based generalization quality
+        # IDEA: store y_obs, y_pred, se_pred as well
+        y_obs, y_pred, se_pred = _predict_on_training_data(
+            model_bridge=self, experiment=experiment
+        )
+        if fit_metrics_dict is None:
+            fit_metrics_dict = {
+                "coefficient_of_determination": coefficient_of_determination,
+                "mean_of_the_standardized_error": mean_of_the_standardized_error,
+                "std_of_the_standardized_error": std_of_the_standardized_error,
+            }
+            fit_metrics_dict = cast(Dict[str, ModelFitMetricProtocol], fit_metrics_dict)
+
+        return compute_model_fit_metrics(
+            y_obs=y_obs,
+            y_pred=y_pred,
+            se_pred=se_pred,
+            fit_metrics_dict=fit_metrics_dict,
+        )
+
     def _set_kwargs_to_save(
         self,
         model_key: str,
         model_kwargs: Dict[str, Any],
         bridge_kwargs: Dict[str, Any],
     ) -> None:
         """Set properties used to save the model that created a given generator
@@ -1095,7 +1148,60 @@
             elif val > p.upper:
                 logger.info(
                     f"Untransformed parameter {val} "
                     f"greater than upper bound {p.upper}, clamping"
                 )
                 obsf.parameters[p.name] = p.upper
     return observation_features
+
+
+"""
+############################## Model Fit Metrics Utils ##############################
+"""
+
+
+def _predict_on_training_data(
+    model_bridge: ModelBridge,
+    experiment: Experiment,
+) -> Tuple[Dict[str, np.ndarray], Dict[str, np.ndarray], Dict[str, np.ndarray],]:
+    """Makes predictions on the training data of a given experiment using a ModelBridge
+    and returning the observed values, and the corresponding predictive means and
+    predictive standard deviations of the model.
+
+     NOTE: This is a helper function for `ModelBridge.compute_model_fit_metrics` and
+    could be attached to the class.
+
+    Args:
+        model_bridge: A ModelBridge object with which to make predictions.
+        experiment: The experiment with whose data to compute the model fit metrics.
+
+    Returns:
+        A tuple containing three dictionaries for 1) observed metric values, and the
+        model's associated 2) predictive means and 3) predictive standard deviations.
+    """
+    data = experiment.fetch_data()
+    observations = observations_from_data(
+        experiment=experiment, data=data
+    )  # List[Observation]
+    observation_features = [obs.features for obs in observations]
+    mean_predicted, cov_predicted = model_bridge.predict(
+        observation_features=observation_features
+    )  # Dict[str, List[float]]
+    mean_observed = [
+        obs.data.means_dict for obs in observations
+    ]  # List[Dict[str, float]]
+    metric_names = list(data.metric_names)
+    mean_observed = _list_of_dicts_to_dict_of_lists(
+        list_of_dicts=mean_observed, keys=metric_names
+    )
+    # converting dictionary values to arrays
+    mean_observed = {k: np.array(v) for k, v in mean_observed.items()}
+    mean_predicted = {k: np.array(v) for k, v in mean_predicted.items()}
+    std_predicted = {m: np.sqrt(np.array(cov_predicted[m][m])) for m in cov_predicted}
+    return mean_observed, mean_predicted, std_predicted
+
+
+def _list_of_dicts_to_dict_of_lists(
+    list_of_dicts: List[Dict[str, float]], keys: List[str]
+) -> Dict[str, List[float]]:
+    """Converts a list of dicts indexed by a string to a dict of lists."""
+    return {key: [d[key] for d in list_of_dicts] for key in keys}
```

### Comparing `ax-platform-0.3.2/ax/modelbridge/completion_criterion.py` & `ax-platform-0.3.3/ax/modelbridge/completion_criterion.py`

 * *Files identical despite different names*

### Comparing `ax-platform-0.3.2/ax/modelbridge/cross_validation.py` & `ax-platform-0.3.3/ax/modelbridge/cross_validation.py`

 * *Files 6% similar despite different names*

```diff
@@ -7,22 +7,45 @@
 from abc import ABC, abstractmethod
 from collections import defaultdict
 from enum import Enum
 from functools import partial
 
 from logging import Logger
 from numbers import Number
-from typing import Any, Callable, Dict, Iterable, List, NamedTuple, Optional, Set, Tuple
+from typing import (
+    Any,
+    Callable,
+    cast,
+    Dict,
+    Iterable,
+    List,
+    Mapping,
+    NamedTuple,
+    Optional,
+    Set,
+    Tuple,
+)
 
 import numpy as np
 from ax.core.observation import Observation, ObservationData
 from ax.core.optimization_config import OptimizationConfig
 from ax.modelbridge.base import ModelBridge
 from ax.utils.common.logger import get_logger
-from scipy.stats import fisher_exact, norm, pearsonr, spearmanr
+
+from ax.utils.stats.model_fit_stats import (
+    _correlation_coefficient,
+    _fisher_exact_test_p,
+    _log_likelihood,
+    _mape,
+    _mean_prediction_ci,
+    _rank_correlation,
+    _total_raw_effect,
+    compute_model_fit_metrics,
+    ModelFitMetricProtocol,
+)
 
 logger: Logger = get_logger(__name__)
 
 CVDiagnostics = Dict[str, Dict[str, float]]
 
 MEAN_PREDICTION_CI = "Mean prediction CI"
 MAPE = "MAPE"
@@ -221,35 +244,44 @@
     for res in result:
         for j, metric_name in enumerate(res.observed.data.metric_names):
             y_obs[metric_name].append(res.observed.data.means[j])
             # Find the matching prediction
             k = res.predicted.metric_names.index(metric_name)
             y_pred[metric_name].append(res.predicted.means[k])
             se_pred[metric_name].append(np.sqrt(res.predicted.covariance[k, k]))
+    y_obs = _arrayify_dict_values(y_obs)
+    y_pred = _arrayify_dict_values(y_pred)
+    se_pred = _arrayify_dict_values(se_pred)
+
+    # We need to cast here since pyre infers specific types T < ModelFitMetricProtocol
+    # for the dict values, which is type variant upon initialization, leading
+    # diagnostic_fns to not be recognized as a Mapping[str, ModelFitMetricProtocol],
+    # see the last tip in the Pyre docs on [9] Incompatible Variable Type:
+    # https://staticdocs.internalfb.com/pyre/docs/errors/#9-incompatible-variable-type
+    diagnostic_fns = cast(
+        Mapping[str, ModelFitMetricProtocol],
+        {
+            MEAN_PREDICTION_CI: _mean_prediction_ci,
+            MAPE: _mape,
+            TOTAL_RAW_EFFECT: _total_raw_effect,
+            CORRELATION_COEFFICIENT: _correlation_coefficient,
+            RANK_CORRELATION: _rank_correlation,
+            FISHER_EXACT_TEST_P: _fisher_exact_test_p,
+            LOG_LIKELIHOOD: _log_likelihood,
+        },
+    )
+    diagnostics = compute_model_fit_metrics(
+        y_obs=y_obs, y_pred=y_pred, se_pred=se_pred, fit_metrics_dict=diagnostic_fns
+    )
+    return diagnostics
 
-    diagnostic_fns = {
-        MEAN_PREDICTION_CI: _mean_prediction_ci,
-        MAPE: _mape,
-        TOTAL_RAW_EFFECT: _total_raw_effect,
-        CORRELATION_COEFFICIENT: _correlation_coefficient,
-        RANK_CORRELATION: _rank_correlation,
-        FISHER_EXACT_TEST_P: _fisher_exact_test_p,
-        LOG_LIKELIHOOD: _log_likelihood,
-    }
 
-    diagnostics: Dict[str, Dict[str, float]] = defaultdict(dict)
-    # Get all per-metric diagnostics.
-    for metric_name in y_obs:
-        for name, fn in diagnostic_fns.items():
-            diagnostics[name][metric_name] = fn(
-                y_obs=np.array(y_obs[metric_name]),
-                y_pred=np.array(y_pred[metric_name]),
-                se_pred=np.array(se_pred[metric_name]),
-            )
-    return diagnostics
+def _arrayify_dict_values(d: Dict[str, List[float]]) -> Dict[str, np.ndarray]:
+    """Helper to convert dictionary values to numpy arrays."""
+    return {k: np.array(v) for k, v in d.items()}
 
 
 def assess_model_fit(
     diagnostics: CVDiagnostics,
     significance_level: float = 0.1,
 ) -> AssessModelFitResult:
     """Assess model fit for given diagnostics results.
@@ -335,71 +367,14 @@
         # We will take the test set from the back of the array.
         # Roll the list of arm names to get a fresh test set
         arm_names = np.roll(arm_names, test_size)
         n_test = test_size if fold < folds - 1 else final_size
         yield set(arm_names[:-n_test]), set(arm_names[-n_test:])
 
 
-def _mean_prediction_ci(
-    y_obs: np.ndarray, y_pred: np.ndarray, se_pred: np.ndarray
-) -> float:
-    # Pyre does not allow float * np.ndarray.
-    return float(np.mean(1.96 * 2 * se_pred / np.abs(y_obs)))
-
-
-def _log_likelihood(
-    y_obs: np.ndarray, y_pred: np.ndarray, se_pred: np.ndarray
-) -> float:
-    return float(np.sum(norm.logpdf(y_obs, loc=y_pred, scale=se_pred)))
-
-
-def _mape(y_obs: np.ndarray, y_pred: np.ndarray, se_pred: np.ndarray) -> float:
-    return float(np.mean(np.abs((y_pred - y_obs) / y_obs)))
-
-
-def _total_raw_effect(
-    y_obs: np.ndarray, y_pred: np.ndarray, se_pred: np.ndarray
-) -> float:
-    min_y_obs = np.min(y_obs)
-    return float((np.max(y_obs) - min_y_obs) / min_y_obs)
-
-
-def _correlation_coefficient(
-    y_obs: np.ndarray, y_pred: np.ndarray, se_pred: np.ndarray
-) -> float:
-    with np.errstate(invalid="ignore"):
-        rho, _ = pearsonr(y_pred, y_obs)
-    return float(rho)
-
-
-def _rank_correlation(
-    y_obs: np.ndarray, y_pred: np.ndarray, se_pred: np.ndarray
-) -> float:
-    with np.errstate(invalid="ignore"):
-        rho, _ = spearmanr(y_pred, y_obs)
-    return float(rho)
-
-
-def _fisher_exact_test_p(
-    y_obs: np.ndarray, y_pred: np.ndarray, se_pred: np.ndarray
-) -> float:
-    n_half = len(y_obs) // 2
-    top_obs = y_obs.argsort(axis=0)[-n_half:]
-    top_est = y_pred.argsort(axis=0)[-n_half:]
-    # Construct contingency table
-    tp = len(set(top_est).intersection(top_obs))
-    fp = n_half - tp
-    fn = n_half - tp
-    tn = (len(y_obs) - n_half) - (n_half - tp)
-    table = np.array([[tp, fp], [fn, tn]])
-    # Compute the test statistic
-    _, p = fisher_exact(table, alternative="greater")
-    return float(p)
-
-
 class BestModelSelector(ABC):
     @abstractmethod
     def best_diagnostic(self, diagnostics: List[CVDiagnostics]) -> int:
         """
         Return the index of the best diagnostic.
         """
         pass  # pragma: no cover
```

### Comparing `ax-platform-0.3.2/ax/modelbridge/discrete.py` & `ax-platform-0.3.3/ax/modelbridge/discrete.py`

 * *Files identical despite different names*

### Comparing `ax-platform-0.3.2/ax/modelbridge/dispatch_utils.py` & `ax-platform-0.3.3/ax/modelbridge/dispatch_utils.py`

 * *Files identical despite different names*

### Comparing `ax-platform-0.3.2/ax/modelbridge/factory.py` & `ax-platform-0.3.3/ax/modelbridge/factory.py`

 * *Files identical despite different names*

### Comparing `ax-platform-0.3.2/ax/modelbridge/generation_node.py` & `ax-platform-0.3.3/ax/modelbridge/generation_node.py`

 * *Files identical despite different names*

### Comparing `ax-platform-0.3.2/ax/modelbridge/generation_strategy.py` & `ax-platform-0.3.3/ax/modelbridge/generation_strategy.py`

 * *Files identical despite different names*

### Comparing `ax-platform-0.3.2/ax/modelbridge/map_torch.py` & `ax-platform-0.3.3/ax/modelbridge/map_torch.py`

 * *Files identical despite different names*

### Comparing `ax-platform-0.3.2/ax/modelbridge/model_spec.py` & `ax-platform-0.3.3/ax/modelbridge/model_spec.py`

 * *Files identical despite different names*

### Comparing `ax-platform-0.3.2/ax/modelbridge/modelbridge_utils.py` & `ax-platform-0.3.3/ax/modelbridge/modelbridge_utils.py`

 * *Files 1% similar despite different names*

```diff
@@ -1011,14 +1011,15 @@
         modelbridge=modelbridge,
         observation_features=observation_features,
         observation_data=observation_data,
         objective_thresholds=objective_thresholds,
         optimization_config=optimization_config,
         arm_names=arm_names,
         use_model_predictions=use_model_predictions,
+        transform_outcomes_and_configs=False,
     )[0]
 
 
 def predicted_pareto_frontier(
     modelbridge: modelbridge_module.torch.TorchModelBridge,
     objective_thresholds: Optional[TRefPoint] = None,
     observation_features: Optional[List[ObservationFeatures]] = None,
@@ -1133,14 +1134,15 @@
     frontier_observations, f, obj_w, obj_t = get_pareto_frontier_and_configs(
         modelbridge=modelbridge,
         observation_features=observation_features,
         observation_data=observation_data,
         objective_thresholds=objective_thresholds,
         optimization_config=optimization_config,
         use_model_predictions=use_model_predictions,
+        transform_outcomes_and_configs=False,
     )
     if obj_t is None:
         raise ValueError(  # pragma: no cover
             "Cannot compute hypervolume without having objective thresholds specified."
         )
     oc = _get_multiobjective_optimization_config(
         modelbridge=modelbridge,
```

### Comparing `ax-platform-0.3.2/ax/modelbridge/pairwise.py` & `ax-platform-0.3.3/ax/modelbridge/pairwise.py`

 * *Files identical despite different names*

### Comparing `ax-platform-0.3.2/ax/modelbridge/prediction_utils.py` & `ax-platform-0.3.3/ax/modelbridge/prediction_utils.py`

 * *Files identical despite different names*

### Comparing `ax-platform-0.3.2/ax/modelbridge/random.py` & `ax-platform-0.3.3/ax/modelbridge/random.py`

 * *Files identical despite different names*

### Comparing `ax-platform-0.3.2/ax/modelbridge/registry.py` & `ax-platform-0.3.3/ax/modelbridge/registry.py`

 * *Files identical despite different names*

### Comparing `ax-platform-0.3.2/ax/modelbridge/strategies/alebo.py` & `ax-platform-0.3.3/ax/modelbridge/strategies/alebo.py`

 * *Files identical despite different names*

### Comparing `ax-platform-0.3.2/ax/modelbridge/strategies/rembo.py` & `ax-platform-0.3.3/ax/modelbridge/strategies/rembo.py`

 * *Files identical despite different names*

### Comparing `ax-platform-0.3.2/ax/modelbridge/tests/test_alebo_strategy.py` & `ax-platform-0.3.3/ax/modelbridge/tests/test_alebo_strategy.py`

 * *Files identical despite different names*

### Comparing `ax-platform-0.3.2/ax/modelbridge/tests/test_base_modelbridge.py` & `ax-platform-0.3.3/ax/modelbridge/tests/test_base_modelbridge.py`

 * *Files identical despite different names*

### Comparing `ax-platform-0.3.2/ax/modelbridge/tests/test_base_transform.py` & `ax-platform-0.3.3/ax/modelbridge/tests/test_base_transform.py`

 * *Files identical despite different names*

### Comparing `ax-platform-0.3.2/ax/modelbridge/tests/test_cap_parameter_transform.py` & `ax-platform-0.3.3/ax/modelbridge/tests/test_cap_parameter_transform.py`

 * *Files identical despite different names*

### Comparing `ax-platform-0.3.2/ax/modelbridge/tests/test_cast_transform.py` & `ax-platform-0.3.3/ax/modelbridge/tests/test_cast_transform.py`

 * *Files identical despite different names*

### Comparing `ax-platform-0.3.2/ax/modelbridge/tests/test_centered_unit_x_transform.py` & `ax-platform-0.3.3/ax/modelbridge/tests/test_centered_unit_x_transform.py`

 * *Files identical despite different names*

### Comparing `ax-platform-0.3.2/ax/modelbridge/tests/test_choice_encode_transform.py` & `ax-platform-0.3.3/ax/modelbridge/tests/test_choice_encode_transform.py`

 * *Files identical despite different names*

### Comparing `ax-platform-0.3.2/ax/modelbridge/tests/test_completion_criterion.py` & `ax-platform-0.3.3/ax/modelbridge/tests/test_completion_criterion.py`

 * *Files identical despite different names*

### Comparing `ax-platform-0.3.2/ax/modelbridge/tests/test_convert_metric_names.py` & `ax-platform-0.3.3/ax/modelbridge/tests/test_convert_metric_names.py`

 * *Files identical despite different names*

### Comparing `ax-platform-0.3.2/ax/modelbridge/tests/test_cross_validation.py` & `ax-platform-0.3.3/ax/modelbridge/tests/test_cross_validation.py`

 * *Files identical despite different names*

### Comparing `ax-platform-0.3.2/ax/modelbridge/tests/test_derelativize_transform.py` & `ax-platform-0.3.3/ax/modelbridge/tests/test_derelativize_transform.py`

 * *Files identical despite different names*

### Comparing `ax-platform-0.3.2/ax/modelbridge/tests/test_discrete_modelbridge.py` & `ax-platform-0.3.3/ax/modelbridge/tests/test_discrete_modelbridge.py`

 * *Files identical despite different names*

### Comparing `ax-platform-0.3.2/ax/modelbridge/tests/test_dispatch_utils.py` & `ax-platform-0.3.3/ax/modelbridge/tests/test_dispatch_utils.py`

 * *Files identical despite different names*

### Comparing `ax-platform-0.3.2/ax/modelbridge/tests/test_factory.py` & `ax-platform-0.3.3/ax/modelbridge/tests/test_factory.py`

 * *Files identical despite different names*

### Comparing `ax-platform-0.3.2/ax/modelbridge/tests/test_generation_node.py` & `ax-platform-0.3.3/ax/modelbridge/tests/test_generation_node.py`

 * *Files identical despite different names*

### Comparing `ax-platform-0.3.2/ax/modelbridge/tests/test_generation_strategy.py` & `ax-platform-0.3.3/ax/modelbridge/tests/test_generation_strategy.py`

 * *Files identical despite different names*

### Comparing `ax-platform-0.3.2/ax/modelbridge/tests/test_int_range_to_choice_transform.py` & `ax-platform-0.3.3/ax/modelbridge/tests/test_int_range_to_choice_transform.py`

 * *Files identical despite different names*

### Comparing `ax-platform-0.3.2/ax/modelbridge/tests/test_int_to_float_transform.py` & `ax-platform-0.3.3/ax/modelbridge/tests/test_int_to_float_transform.py`

 * *Files identical despite different names*

### Comparing `ax-platform-0.3.2/ax/modelbridge/tests/test_inverse_gaussian_cdf_y.py` & `ax-platform-0.3.3/ax/modelbridge/tests/test_inverse_gaussian_cdf_y.py`

 * *Files identical despite different names*

### Comparing `ax-platform-0.3.2/ax/modelbridge/tests/test_ivw_transform.py` & `ax-platform-0.3.3/ax/modelbridge/tests/test_ivw_transform.py`

 * *Files identical despite different names*

### Comparing `ax-platform-0.3.2/ax/modelbridge/tests/test_log_transform.py` & `ax-platform-0.3.3/ax/modelbridge/tests/test_log_transform.py`

 * *Files identical despite different names*

### Comparing `ax-platform-0.3.2/ax/modelbridge/tests/test_log_y_transform.py` & `ax-platform-0.3.3/ax/modelbridge/tests/test_log_y_transform.py`

 * *Files identical despite different names*

### Comparing `ax-platform-0.3.2/ax/modelbridge/tests/test_logit_transform.py` & `ax-platform-0.3.3/ax/modelbridge/tests/test_logit_transform.py`

 * *Files identical despite different names*

### Comparing `ax-platform-0.3.2/ax/modelbridge/tests/test_map_torch_modelbridge.py` & `ax-platform-0.3.3/ax/modelbridge/tests/test_map_torch_modelbridge.py`

 * *Files identical despite different names*

### Comparing `ax-platform-0.3.2/ax/modelbridge/tests/test_map_unit_x_transform.py` & `ax-platform-0.3.3/ax/modelbridge/tests/test_map_unit_x_transform.py`

 * *Files identical despite different names*

### Comparing `ax-platform-0.3.2/ax/modelbridge/tests/test_merge_repeated_measurements_transform.py` & `ax-platform-0.3.3/ax/modelbridge/tests/test_merge_repeated_measurements_transform.py`

 * *Files identical despite different names*

### Comparing `ax-platform-0.3.2/ax/modelbridge/tests/test_metrics_as_task_transform.py` & `ax-platform-0.3.3/ax/modelbridge/tests/test_metrics_as_task_transform.py`

 * *Files identical despite different names*

### Comparing `ax-platform-0.3.2/ax/modelbridge/tests/test_model_spec.py` & `ax-platform-0.3.3/ax/modelbridge/tests/test_model_spec.py`

 * *Files identical despite different names*

### Comparing `ax-platform-0.3.2/ax/modelbridge/tests/test_modelbridge_utils.py` & `ax-platform-0.3.3/ax/modelbridge/tests/test_modelbridge_utils.py`

 * *Files identical despite different names*

### Comparing `ax-platform-0.3.2/ax/modelbridge/tests/test_one_hot_transform.py` & `ax-platform-0.3.3/ax/modelbridge/tests/test_one_hot_transform.py`

 * *Files identical despite different names*

### Comparing `ax-platform-0.3.2/ax/modelbridge/tests/test_pairwise_modelbridge.py` & `ax-platform-0.3.3/ax/modelbridge/tests/test_pairwise_modelbridge.py`

 * *Files identical despite different names*

### Comparing `ax-platform-0.3.2/ax/modelbridge/tests/test_percentile_y_transform.py` & `ax-platform-0.3.3/ax/modelbridge/tests/test_percentile_y_transform.py`

 * *Files identical despite different names*

### Comparing `ax-platform-0.3.2/ax/modelbridge/tests/test_power_transform_y.py` & `ax-platform-0.3.3/ax/modelbridge/tests/test_power_transform_y.py`

 * *Files identical despite different names*

### Comparing `ax-platform-0.3.2/ax/modelbridge/tests/test_prediction_utils.py` & `ax-platform-0.3.3/ax/modelbridge/tests/test_prediction_utils.py`

 * *Files identical despite different names*

### Comparing `ax-platform-0.3.2/ax/modelbridge/tests/test_random_modelbridge.py` & `ax-platform-0.3.3/ax/modelbridge/tests/test_random_modelbridge.py`

 * *Files identical despite different names*

### Comparing `ax-platform-0.3.2/ax/modelbridge/tests/test_registry.py` & `ax-platform-0.3.3/ax/modelbridge/tests/test_registry.py`

 * *Files identical despite different names*

### Comparing `ax-platform-0.3.2/ax/modelbridge/tests/test_relativize_transform.py` & `ax-platform-0.3.3/ax/modelbridge/tests/test_relativize_transform.py`

 * *Files identical despite different names*

### Comparing `ax-platform-0.3.2/ax/modelbridge/tests/test_rembo_strategy.py` & `ax-platform-0.3.3/ax/modelbridge/tests/test_rembo_strategy.py`

 * *Files identical despite different names*

### Comparing `ax-platform-0.3.2/ax/modelbridge/tests/test_remove_fixed_transform.py` & `ax-platform-0.3.3/ax/modelbridge/tests/test_remove_fixed_transform.py`

 * *Files identical despite different names*

### Comparing `ax-platform-0.3.2/ax/modelbridge/tests/test_robust.py` & `ax-platform-0.3.3/ax/modelbridge/tests/test_robust.py`

 * *Files identical despite different names*

### Comparing `ax-platform-0.3.2/ax/modelbridge/tests/test_rounding.py` & `ax-platform-0.3.3/ax/modelbridge/tests/test_rounding.py`

 * *Files identical despite different names*

### Comparing `ax-platform-0.3.2/ax/modelbridge/tests/test_search_space_to_choice_transform.py` & `ax-platform-0.3.3/ax/modelbridge/tests/test_search_space_to_choice_transform.py`

 * *Files identical despite different names*

### Comparing `ax-platform-0.3.2/ax/modelbridge/tests/test_search_space_to_float_transform.py` & `ax-platform-0.3.3/ax/modelbridge/tests/test_search_space_to_float_transform.py`

 * *Files identical despite different names*

### Comparing `ax-platform-0.3.2/ax/modelbridge/tests/test_standardize_y_transform.py` & `ax-platform-0.3.3/ax/modelbridge/tests/test_standardize_y_transform.py`

 * *Files identical despite different names*

### Comparing `ax-platform-0.3.2/ax/modelbridge/tests/test_stratified_standardize_y.py` & `ax-platform-0.3.3/ax/modelbridge/tests/test_stratified_standardize_y.py`

 * *Files identical despite different names*

### Comparing `ax-platform-0.3.2/ax/modelbridge/tests/test_task_encode_transform.py` & `ax-platform-0.3.3/ax/modelbridge/tests/test_task_encode_transform.py`

 * *Files identical despite different names*

### Comparing `ax-platform-0.3.2/ax/modelbridge/tests/test_torch_modelbridge.py` & `ax-platform-0.3.3/ax/modelbridge/tests/test_torch_modelbridge.py`

 * *Files identical despite different names*

### Comparing `ax-platform-0.3.2/ax/modelbridge/tests/test_torch_modelbridge_moo.py` & `ax-platform-0.3.3/ax/modelbridge/tests/test_torch_modelbridge_moo.py`

 * *Files identical despite different names*

### Comparing `ax-platform-0.3.2/ax/modelbridge/tests/test_transform_utils.py` & `ax-platform-0.3.3/ax/modelbridge/tests/test_transform_utils.py`

 * *Files identical despite different names*

### Comparing `ax-platform-0.3.2/ax/modelbridge/tests/test_trial_as_task_transform.py` & `ax-platform-0.3.3/ax/modelbridge/tests/test_trial_as_task_transform.py`

 * *Files identical despite different names*

### Comparing `ax-platform-0.3.2/ax/modelbridge/tests/test_unit_x_transform.py` & `ax-platform-0.3.3/ax/modelbridge/tests/test_unit_x_transform.py`

 * *Files identical despite different names*

### Comparing `ax-platform-0.3.2/ax/modelbridge/tests/test_utils.py` & `ax-platform-0.3.3/ax/modelbridge/tests/test_utils.py`

 * *Files identical despite different names*

### Comparing `ax-platform-0.3.2/ax/modelbridge/tests/test_winsorize_transform.py` & `ax-platform-0.3.3/ax/modelbridge/tests/test_winsorize_transform.py`

 * *Files 0% similar despite different names*

```diff
@@ -492,34 +492,34 @@
             for i in range(2):
                 self.assertTrue(
                     "Automatic winsorization isn't supported for a "
                     "`ScalarizedOutcomeConstraint`. Specify the winsorization settings "
                     f"manually if you want to winsorize metric m{['1', '3'][i]}."
                     in [str(w.message) for w in ws]
                 )
-        # Multi-objective without objective thresholds (should print a warning)
+        # Multi-objective without objective thresholds should warn and winsorize
         moo_objective = MultiObjective(
             [Objective(m1, minimize=False), Objective(m2, minimize=True)]
         )
         optimization_config = MultiObjectiveOptimizationConfig(objective=moo_objective)
         warnings.simplefilter("always", append=True)
         with warnings.catch_warnings(record=True) as ws:
             transform = get_transform(
                 observation_data=deepcopy(all_obsd),
                 optimization_config=optimization_config,
             )
-            for i in range(2):
+            for _ in range(2):
                 self.assertTrue(
-                    "Automatic winsorization isn't supported for an objective in "
-                    "`MultiObjective` without objective thresholds. Specify the "
-                    "winsorization settings manually if you want to winsorize "
-                    f"metric m{i + 1}." in [str(w.message) for w in ws]
+                    "Encountered a `MultiObjective` without objective thresholds. We "
+                    "will winsorize each objective separately. We strongly recommend "
+                    "specifying the objective thresholds when using multi-objective "
+                    "optimization." in [str(w.message) for w in ws]
                 )
-        self.assertEqual(transform.cutoffs["m1"], (-float("inf"), float("inf")))
-        self.assertEqual(transform.cutoffs["m2"], (-float("inf"), float("inf")))
+        self.assertEqual(transform.cutoffs["m1"], (-6.5, float("inf")))
+        self.assertEqual(transform.cutoffs["m2"], (-float("inf"), 10.0))
         self.assertEqual(transform.cutoffs["m3"], (-float("inf"), float("inf")))
         # Add relative objective thresholds (should raise an error)
         objective_thresholds = [
             ObjectiveThreshold(m1, 3, relative=True),
             ObjectiveThreshold(m2, 4, relative=True),
         ]
         optimization_config = MultiObjectiveOptimizationConfig(
```

### Comparing `ax-platform-0.3.2/ax/modelbridge/tests/test_winsorize_transform_legacy.py` & `ax-platform-0.3.3/ax/modelbridge/tests/test_winsorize_transform_legacy.py`

 * *Files identical despite different names*

### Comparing `ax-platform-0.3.2/ax/modelbridge/torch.py` & `ax-platform-0.3.3/ax/modelbridge/torch.py`

 * *Files 2% similar despite different names*

```diff
@@ -347,32 +347,28 @@
         """Make predictions at cv_test_points using only the data in obs_feats
         and obs_data.
         """
         if self.model is None:
             raise ValueError(  # pragma: no cover
                 FIT_MODEL_ERROR.format(action="_cross_validate")
             )
-        if parameters is None:
-            parameters = self.parameters
-        observation_features, observation_data = separate_observations(cv_training_data)
-        datasets, candidate_metadata = self._convert_observations(
-            observation_data=observation_data,
-            observation_features=observation_features,
-            outcomes=self.outcomes,
+        datasets, candidate_metadata, search_space_digest = self._get_fit_args(
+            search_space=search_space,
+            observations=cv_training_data,
             parameters=parameters,
+            update_outcomes_and_parameters=False,
         )
         for outcome, dataset in zip(self.outcomes, datasets):
             if dataset is None:
                 raise UnsupportedError(  # pragma: no cover
                     f"{self.__class__._cross_validate} requires observations "
                     f"for all outcomes, but no observations for {outcome}"
                 )
-        search_space_digest = extract_search_space_digest(
-            search_space=search_space, param_names=self.parameters
-        )
+        if parameters is None:
+            parameters = self.parameters
         X_test = torch.tensor(
             [[obsf.parameters[p] for p in parameters] for obsf in cv_test_points],
             dtype=self.dtype,
             device=self.device,
         )
         # Use the model to do the cross validation
         f_test, cov_test = not_none(self.model).cross_validate(
@@ -485,48 +481,87 @@
             X=self._array_to_tensor(X),
             search_space_digest=search_space_digest,
             torch_opt_config=torch_opt_config,
             acq_options=acq_options,
         )
         return evals.tolist()
 
-    def _fit(
+    def _get_fit_args(
         self,
-        model: TorchModel,
         search_space: SearchSpace,
         observations: List[Observation],
-        parameters: Optional[List[str]] = None,
-        **kwargs: Any,
-    ) -> None:  # pragma: no cover
-        if self.model is not None and observations == self._last_observations:
-            logger.info(
-                "The observations are identical to the last set of observations "
-                "used to fit the model. Skipping model fitting."
-            )
-            return
+        parameters: Optional[List[str]],
+        update_outcomes_and_parameters: bool,
+    ) -> Tuple[
+        List[Optional[SupervisedDataset]],
+        Optional[List[List[TCandidateMetadata]]],
+        SearchSpaceDigest,
+    ]:
+        """Helper for consolidating some common argument processing between
+        fit and cross validate methods. Extracts datasets and candidate metadate
+        from observations and the search space digest from the search space.
+
+        Args:
+            search_space: A transformed search space for fitting the model.
+            observations: The observations to fit the model with. These should
+                also be transformed.
+            parameters: Names of parameters to be used in the model. Defaults to
+                all parameters in the search space.
+            update_outcomes_and_parameters: Whether to update `self.outcomes` with
+                all outcomes found in the observations and `self.parameters` with
+                all parameters in the search space. Typically only used in `_fit`.
+
+        Returns:
+            The datasets & metadata extracted from the observations and the
+            search space digest.
+        """
         self._last_observations = observations
-        self.parameters = list(search_space.parameters.keys())
+        if update_outcomes_and_parameters:
+            self.parameters = list(search_space.parameters.keys())
         if parameters is None:
             parameters = self.parameters
         all_metric_names: Set[str] = set()
         observation_features, observation_data = separate_observations(observations)
-        for od in observation_data:
-            all_metric_names.update(od.metric_names)
-        self.outcomes = sorted(all_metric_names)  # Deterministic order
+        if update_outcomes_and_parameters:
+            for od in observation_data:
+                all_metric_names.update(od.metric_names)
+            self.outcomes = sorted(all_metric_names)  # Deterministic order
         # Convert observations to datasets
         datasets, candidate_metadata = self._convert_observations(
             observation_data=observation_data,
             observation_features=observation_features,
             outcomes=self.outcomes,
             parameters=parameters,
         )
         # Get all relevant information on the parameters
         search_space_digest = extract_search_space_digest(
             search_space=search_space, param_names=self.parameters
         )
+        return datasets, candidate_metadata, search_space_digest
+
+    def _fit(
+        self,
+        model: TorchModel,
+        search_space: SearchSpace,
+        observations: List[Observation],
+        parameters: Optional[List[str]] = None,
+        **kwargs: Any,
+    ) -> None:  # pragma: no cover
+        if self.model is not None and observations == self._last_observations:
+            logger.info(
+                "The observations are identical to the last set of observations "
+                "used to fit the model. Skipping model fitting."
+            )
+            return
+        datasets, candidate_metadata, search_space_digest = self._get_fit_args(
+            search_space=search_space,
+            observations=observations,
+            parameters=parameters,
+            update_outcomes_and_parameters=True,
+        )
         # Fit
         self.model = model
         self.model.fit(
             # datasets are guaranteed to have all outcomes here by construction
             datasets=[not_none(dataset) for dataset in datasets],
             metric_names=self.outcomes,
             search_space_digest=search_space_digest,
```

### Comparing `ax-platform-0.3.2/ax/modelbridge/transforms/base.py` & `ax-platform-0.3.3/ax/modelbridge/transforms/base.py`

 * *Files identical despite different names*

### Comparing `ax-platform-0.3.2/ax/modelbridge/transforms/cap_parameter.py` & `ax-platform-0.3.3/ax/modelbridge/transforms/cap_parameter.py`

 * *Files identical despite different names*

### Comparing `ax-platform-0.3.2/ax/modelbridge/transforms/cast.py` & `ax-platform-0.3.3/ax/modelbridge/transforms/cast.py`

 * *Files identical despite different names*

### Comparing `ax-platform-0.3.2/ax/modelbridge/transforms/choice_encode.py` & `ax-platform-0.3.3/ax/modelbridge/transforms/choice_encode.py`

 * *Files identical despite different names*

### Comparing `ax-platform-0.3.2/ax/modelbridge/transforms/convert_metric_names.py` & `ax-platform-0.3.3/ax/modelbridge/transforms/convert_metric_names.py`

 * *Files identical despite different names*

### Comparing `ax-platform-0.3.2/ax/modelbridge/transforms/derelativize.py` & `ax-platform-0.3.3/ax/modelbridge/transforms/derelativize.py`

 * *Files identical despite different names*

### Comparing `ax-platform-0.3.2/ax/modelbridge/transforms/int_range_to_choice.py` & `ax-platform-0.3.3/ax/modelbridge/transforms/int_range_to_choice.py`

 * *Files identical despite different names*

### Comparing `ax-platform-0.3.2/ax/modelbridge/transforms/int_to_float.py` & `ax-platform-0.3.3/ax/modelbridge/transforms/int_to_float.py`

 * *Files identical despite different names*

### Comparing `ax-platform-0.3.2/ax/modelbridge/transforms/inverse_gaussian_cdf_y.py` & `ax-platform-0.3.3/ax/modelbridge/transforms/inverse_gaussian_cdf_y.py`

 * *Files identical despite different names*

### Comparing `ax-platform-0.3.2/ax/modelbridge/transforms/ivw.py` & `ax-platform-0.3.3/ax/modelbridge/transforms/ivw.py`

 * *Files identical despite different names*

### Comparing `ax-platform-0.3.2/ax/modelbridge/transforms/log.py` & `ax-platform-0.3.3/ax/modelbridge/transforms/log.py`

 * *Files identical despite different names*

### Comparing `ax-platform-0.3.2/ax/modelbridge/transforms/log_y.py` & `ax-platform-0.3.3/ax/modelbridge/transforms/log_y.py`

 * *Files identical despite different names*

### Comparing `ax-platform-0.3.2/ax/modelbridge/transforms/logit.py` & `ax-platform-0.3.3/ax/modelbridge/transforms/logit.py`

 * *Files identical despite different names*

### Comparing `ax-platform-0.3.2/ax/modelbridge/transforms/map_unit_x.py` & `ax-platform-0.3.3/ax/modelbridge/transforms/map_unit_x.py`

 * *Files identical despite different names*

### Comparing `ax-platform-0.3.2/ax/modelbridge/transforms/merge_repeated_measurements.py` & `ax-platform-0.3.3/ax/modelbridge/transforms/merge_repeated_measurements.py`

 * *Files identical despite different names*

### Comparing `ax-platform-0.3.2/ax/modelbridge/transforms/metrics_as_task.py` & `ax-platform-0.3.3/ax/modelbridge/transforms/metrics_as_task.py`

 * *Files identical despite different names*

### Comparing `ax-platform-0.3.2/ax/modelbridge/transforms/one_hot.py` & `ax-platform-0.3.3/ax/modelbridge/transforms/one_hot.py`

 * *Files identical despite different names*

### Comparing `ax-platform-0.3.2/ax/modelbridge/transforms/percentile_y.py` & `ax-platform-0.3.3/ax/modelbridge/transforms/percentile_y.py`

 * *Files identical despite different names*

### Comparing `ax-platform-0.3.2/ax/modelbridge/transforms/power_transform_y.py` & `ax-platform-0.3.3/ax/modelbridge/transforms/power_transform_y.py`

 * *Files identical despite different names*

### Comparing `ax-platform-0.3.2/ax/modelbridge/transforms/relativize.py` & `ax-platform-0.3.3/ax/modelbridge/transforms/relativize.py`

 * *Files identical despite different names*

### Comparing `ax-platform-0.3.2/ax/modelbridge/transforms/remove_fixed.py` & `ax-platform-0.3.3/ax/modelbridge/transforms/remove_fixed.py`

 * *Files identical despite different names*

### Comparing `ax-platform-0.3.2/ax/modelbridge/transforms/rounding.py` & `ax-platform-0.3.3/ax/modelbridge/transforms/rounding.py`

 * *Files identical despite different names*

### Comparing `ax-platform-0.3.2/ax/modelbridge/transforms/search_space_to_choice.py` & `ax-platform-0.3.3/ax/modelbridge/transforms/search_space_to_choice.py`

 * *Files identical despite different names*

### Comparing `ax-platform-0.3.2/ax/modelbridge/transforms/search_space_to_float.py` & `ax-platform-0.3.3/ax/modelbridge/transforms/search_space_to_float.py`

 * *Files identical despite different names*

### Comparing `ax-platform-0.3.2/ax/modelbridge/transforms/standardize_y.py` & `ax-platform-0.3.3/ax/modelbridge/transforms/standardize_y.py`

 * *Files identical despite different names*

### Comparing `ax-platform-0.3.2/ax/modelbridge/transforms/stratified_standardize_y.py` & `ax-platform-0.3.3/ax/modelbridge/transforms/stratified_standardize_y.py`

 * *Files identical despite different names*

### Comparing `ax-platform-0.3.2/ax/modelbridge/transforms/task_encode.py` & `ax-platform-0.3.3/ax/modelbridge/transforms/task_encode.py`

 * *Files identical despite different names*

### Comparing `ax-platform-0.3.2/ax/modelbridge/transforms/trial_as_task.py` & `ax-platform-0.3.3/ax/modelbridge/transforms/trial_as_task.py`

 * *Files identical despite different names*

### Comparing `ax-platform-0.3.2/ax/modelbridge/transforms/unit_x.py` & `ax-platform-0.3.3/ax/modelbridge/transforms/unit_x.py`

 * *Files identical despite different names*

### Comparing `ax-platform-0.3.2/ax/modelbridge/transforms/utils.py` & `ax-platform-0.3.3/ax/modelbridge/transforms/utils.py`

 * *Files identical despite different names*

### Comparing `ax-platform-0.3.2/ax/modelbridge/transforms/winsorize.py` & `ax-platform-0.3.3/ax/modelbridge/transforms/winsorize.py`

 * *Files 3% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 # LICENSE file in the root directory of this source tree.
 
 import warnings
 from logging import Logger
 from typing import Dict, List, Optional, Tuple, TYPE_CHECKING, Union
 
 import numpy as np
-from ax.core.objective import ScalarizedObjective
+from ax.core.objective import MultiObjective, ScalarizedObjective
 from ax.core.observation import Observation, ObservationData
 from ax.core.optimization_config import (
     MultiObjectiveOptimizationConfig,
     OptimizationConfig,
 )
 from ax.core.outcome_constraint import (
     ComparisonOp,
@@ -268,20 +268,30 @@
         optimization_config=optimization_config, metric_name=metric_name
     )
     if objective_threshold:
         return _get_auto_winsorization_cutoffs_outcome_constraint(
             metric_values=metric_values,
             outcome_constraints=objective_threshold,
         )
-    warnings.warn(
-        "Automatic winsorization isn't supported for an objective in `MultiObjective` "
-        "without objective thresholds. Specify the winsorization settings manually if "
-        f"you want to winsorize metric {metric_name}."
-    )
-    return DEFAULT_CUTOFFS  # Don't winsorize if there is no threshold
+    else:
+        warnings.warn(
+            "Encountered a `MultiObjective` without objective thresholds. We will "
+            "winsorize each objective separately. We strongly recommend specifying "
+            "the objective thresholds when using multi-objective optimization."
+        )
+        objectives = checked_cast(MultiObjective, optimization_config.objective)
+        minimize = [
+            objective.minimize
+            for objective in objectives.objectives
+            if objective.metric.name == metric_name
+        ][0]
+        return _get_auto_winsorization_cutoffs_single_objective(
+            metric_values=metric_values,
+            minimize=minimize,
+        )
 
 
 def _obtain_cutoffs_from_outcome_constraints(
     optimization_config: OptimizationConfig,
     metric_name: str,
     metric_values: List[float],
 ) -> Tuple[float, float]:
```

### Comparing `ax-platform-0.3.2/ax/models/base.py` & `ax-platform-0.3.3/ax/models/base.py`

 * *Files identical despite different names*

### Comparing `ax-platform-0.3.2/ax/models/discrete/eb_thompson.py` & `ax-platform-0.3.3/ax/models/discrete/eb_thompson.py`

 * *Files identical despite different names*

### Comparing `ax-platform-0.3.2/ax/models/discrete/full_factorial.py` & `ax-platform-0.3.3/ax/models/discrete/full_factorial.py`

 * *Files identical despite different names*

### Comparing `ax-platform-0.3.2/ax/models/discrete/thompson.py` & `ax-platform-0.3.3/ax/models/discrete/thompson.py`

 * *Files identical despite different names*

### Comparing `ax-platform-0.3.2/ax/models/discrete_base.py` & `ax-platform-0.3.3/ax/models/discrete_base.py`

 * *Files identical despite different names*

### Comparing `ax-platform-0.3.2/ax/models/model_utils.py` & `ax-platform-0.3.3/ax/models/model_utils.py`

 * *Files identical despite different names*

### Comparing `ax-platform-0.3.2/ax/models/random/alebo_initializer.py` & `ax-platform-0.3.3/ax/models/random/alebo_initializer.py`

 * *Files identical despite different names*

### Comparing `ax-platform-0.3.2/ax/models/random/base.py` & `ax-platform-0.3.3/ax/models/random/base.py`

 * *Files identical despite different names*

### Comparing `ax-platform-0.3.2/ax/models/random/rembo_initializer.py` & `ax-platform-0.3.3/ax/models/random/rembo_initializer.py`

 * *Files identical despite different names*

### Comparing `ax-platform-0.3.2/ax/models/random/sobol.py` & `ax-platform-0.3.3/ax/models/random/sobol.py`

 * *Files identical despite different names*

### Comparing `ax-platform-0.3.2/ax/models/random/uniform.py` & `ax-platform-0.3.3/ax/models/random/uniform.py`

 * *Files identical despite different names*

### Comparing `ax-platform-0.3.2/ax/models/tests/test_alebo.py` & `ax-platform-0.3.3/ax/models/tests/test_alebo.py`

 * *Files 4% similar despite different names*

```diff
@@ -18,19 +18,21 @@
     extract_map_statedict,
     get_batch_model,
     get_fitted_model,
     get_map_model,
 )
 from ax.models.torch_base import TorchOptConfig
 from ax.utils.common.testutils import TestCase
+from ax.utils.common.typeutils import checked_cast
 from ax.utils.testing.mock import fast_botorch_optimize
 from botorch.acquisition.analytic import ExpectedImprovement
 from botorch.acquisition.monte_carlo import qNoisyExpectedImprovement
 from botorch.models.model_list_gp_regression import ModelListGP
 from botorch.utils.datasets import FixedNoiseDataset
+from torch.nn.parameter import Parameter
 
 
 class ALEBOTest(TestCase):
     def testALEBOKernel(self) -> None:
         B = torch.tensor(
             [[1.0, 2.0, 3.0, 4.0, 5.0], [2.0, 3.0, 4.0, 5.0, 6.0]], dtype=torch.double
         )
@@ -43,15 +45,17 @@
         )
         self.assertTrue(
             torch.equal(k.triu_indx[1], torch.tensor([0, 1, 1], dtype=torch.long))
         )
         self.assertEqual(k.Uvec.shape, torch.Size([3]))
 
         k.Uvec.requires_grad_(False)
-        k.Uvec.copy_(torch.tensor([1.0, 2.0, 3.0], dtype=torch.double))
+        checked_cast(Parameter, k.Uvec).copy_(
+            torch.tensor([1.0, 2.0, 3.0], dtype=torch.double)
+        )
         k.Uvec.requires_grad_(True)
         x1 = torch.tensor([[0.0, 0.0], [1.0, 1.0]], dtype=torch.double)
         x2 = torch.tensor([[1.0, 1.0], [0.0, 0.0]], dtype=torch.double)
 
         K = k.forward(x1, x2)
         Ktrue = torch.tensor(
             [[np.exp(-0.5 * 18), 1.0], [1.0, np.exp(-0.5 * 18)]], dtype=torch.double
```

### Comparing `ax-platform-0.3.2/ax/models/tests/test_alebo_initializer.py` & `ax-platform-0.3.3/ax/models/tests/test_alebo_initializer.py`

 * *Files identical despite different names*

### Comparing `ax-platform-0.3.2/ax/models/tests/test_base.py` & `ax-platform-0.3.3/ax/models/tests/test_base.py`

 * *Files identical despite different names*

### Comparing `ax-platform-0.3.2/ax/models/tests/test_botorch_defaults.py` & `ax-platform-0.3.3/ax/models/tests/test_botorch_defaults.py`

 * *Files 8% similar despite different names*

```diff
@@ -12,14 +12,15 @@
     _get_acquisition_func,
     _get_customized_covar_module,
     _get_model,
     get_and_fit_model,
     get_warping_transform,
 )
 from ax.utils.common.testutils import TestCase
+from ax.utils.common.typeutils import checked_cast
 from ax.utils.testing.mock import fast_botorch_optimize
 from botorch.acquisition.penalized import PenalizedMCObjective
 from botorch.models import FixedNoiseGP, SingleTaskGP
 from botorch.models.gp_regression_fidelity import SingleTaskMultiFidelityGP
 from botorch.models.multitask import FixedNoiseMultiTaskGP, MultiTaskGP
 from botorch.models.transforms.input import Warp
 from gpytorch.kernels import MaternKernel, ScaleKernel
@@ -380,43 +381,55 @@
             ard_num_dims=ard_num_dims,
             batch_shape=batch_shape,
             task_feature=None,
         )
         self.assertIsInstance(covar_module, Module)
         self.assertIsInstance(covar_module, ScaleKernel)
         self.assertIsInstance(covar_module.outputscale_prior, GammaPrior)
-        self.assertEqual(covar_module.outputscale_prior.concentration, 2.0)
-        self.assertEqual(covar_module.outputscale_prior.rate, 0.15)
+        prior = checked_cast(GammaPrior, covar_module.outputscale_prior)
+        self.assertEqual(prior.concentration, 2.0)
+        self.assertEqual(prior.rate, 0.15)
         self.assertIsInstance(covar_module.base_kernel, MaternKernel)
-        self.assertIsInstance(covar_module.base_kernel.lengthscale_prior, GammaPrior)
-        self.assertEqual(covar_module.base_kernel.lengthscale_prior.concentration, 3.0)
-        self.assertEqual(covar_module.base_kernel.lengthscale_prior.rate, 6.0)
-        self.assertEqual(covar_module.base_kernel.ard_num_dims, ard_num_dims)
-        self.assertEqual(covar_module.base_kernel.batch_shape, batch_shape)
+        base_kernel = checked_cast(MaternKernel, covar_module.base_kernel)
+        self.assertIsInstance(base_kernel.lengthscale_prior, GammaPrior)
+        self.assertEqual(
+            checked_cast(GammaPrior, base_kernel.lengthscale_prior).concentration, 3.0
+        )
+        self.assertEqual(
+            checked_cast(GammaPrior, base_kernel.lengthscale_prior).rate, 6.0
+        )
+        self.assertEqual(base_kernel.ard_num_dims, ard_num_dims)
+        self.assertEqual(base_kernel.batch_shape, batch_shape)
 
         covar_module = _get_customized_covar_module(
             covar_module_prior_dict={
                 "lengthscale_prior": GammaPrior(12.0, 2.0),
                 "outputscale_prior": GammaPrior(2.0, 12.0),
             },
             ard_num_dims=ard_num_dims,
             batch_shape=batch_shape,
             task_feature=3,
         )
         self.assertIsInstance(covar_module, Module)
         self.assertIsInstance(covar_module, ScaleKernel)
         self.assertIsInstance(covar_module.outputscale_prior, GammaPrior)
-        self.assertEqual(covar_module.outputscale_prior.concentration, 2.0)
-        self.assertEqual(covar_module.outputscale_prior.rate, 12.0)
+        prior = checked_cast(GammaPrior, covar_module.outputscale_prior)
+        self.assertEqual(prior.concentration, 2.0)
+        self.assertEqual(prior.rate, 12.0)
         self.assertIsInstance(covar_module.base_kernel, MaternKernel)
-        self.assertIsInstance(covar_module.base_kernel.lengthscale_prior, GammaPrior)
-        self.assertEqual(covar_module.base_kernel.lengthscale_prior.concentration, 12.0)
-        self.assertEqual(covar_module.base_kernel.lengthscale_prior.rate, 2.0)
-        self.assertEqual(covar_module.base_kernel.ard_num_dims, ard_num_dims - 1)
-        self.assertEqual(covar_module.base_kernel.batch_shape, batch_shape)
+        base_kernel = checked_cast(MaternKernel, covar_module.base_kernel)
+        self.assertIsInstance(base_kernel.lengthscale_prior, GammaPrior)
+        self.assertEqual(
+            checked_cast(GammaPrior, base_kernel.lengthscale_prior).concentration, 12.0
+        )
+        self.assertEqual(
+            checked_cast(GammaPrior, base_kernel.lengthscale_prior).rate, 2.0
+        )
+        self.assertEqual(base_kernel.ard_num_dims, ard_num_dims - 1)
+        self.assertEqual(base_kernel.batch_shape, batch_shape)
 
     def test_get_warping_transform(self) -> None:
         warp_tf = get_warping_transform(d=4)
         self.assertIsInstance(warp_tf, Warp)
         self.assertEqual(warp_tf.indices.tolist(), list(range(4)))
         warp_tf = get_warping_transform(d=4, task_feature=2)
         self.assertEqual(warp_tf.indices.tolist(), [0, 1, 3])
```

### Comparing `ax-platform-0.3.2/ax/models/tests/test_botorch_kg.py` & `ax-platform-0.3.3/ax/models/tests/test_botorch_kg.py`

 * *Files identical despite different names*

### Comparing `ax-platform-0.3.2/ax/models/tests/test_botorch_mes.py` & `ax-platform-0.3.3/ax/models/tests/test_botorch_mes.py`

 * *Files identical despite different names*

### Comparing `ax-platform-0.3.2/ax/models/tests/test_botorch_model.py` & `ax-platform-0.3.3/ax/models/tests/test_botorch_model.py`

 * *Files identical despite different names*

### Comparing `ax-platform-0.3.2/ax/models/tests/test_botorch_moo_defaults.py` & `ax-platform-0.3.3/ax/models/tests/test_botorch_moo_defaults.py`

 * *Files identical despite different names*

### Comparing `ax-platform-0.3.2/ax/models/tests/test_botorch_moo_model.py` & `ax-platform-0.3.3/ax/models/tests/test_botorch_moo_model.py`

 * *Files identical despite different names*

### Comparing `ax-platform-0.3.2/ax/models/tests/test_cbo_lcea.py` & `ax-platform-0.3.3/ax/models/tests/test_cbo_lcea.py`

 * *Files identical despite different names*

### Comparing `ax-platform-0.3.2/ax/models/tests/test_cbo_lcem.py` & `ax-platform-0.3.3/ax/models/tests/test_cbo_lcem.py`

 * *Files identical despite different names*

### Comparing `ax-platform-0.3.2/ax/models/tests/test_cbo_sac.py` & `ax-platform-0.3.3/ax/models/tests/test_cbo_sac.py`

 * *Files identical despite different names*

### Comparing `ax-platform-0.3.2/ax/models/tests/test_discrete.py` & `ax-platform-0.3.3/ax/models/tests/test_discrete.py`

 * *Files identical despite different names*

### Comparing `ax-platform-0.3.2/ax/models/tests/test_eb_thompson.py` & `ax-platform-0.3.3/ax/models/tests/test_eb_thompson.py`

 * *Files identical despite different names*

### Comparing `ax-platform-0.3.2/ax/models/tests/test_full_factorial.py` & `ax-platform-0.3.3/ax/models/tests/test_full_factorial.py`

 * *Files identical despite different names*

### Comparing `ax-platform-0.3.2/ax/models/tests/test_fully_bayesian.py` & `ax-platform-0.3.3/ax/models/tests/test_fully_bayesian.py`

 * *Files identical despite different names*

### Comparing `ax-platform-0.3.2/ax/models/tests/test_model_utils.py` & `ax-platform-0.3.3/ax/models/tests/test_model_utils.py`

 * *Files identical despite different names*

### Comparing `ax-platform-0.3.2/ax/models/tests/test_posterior_mean.py` & `ax-platform-0.3.3/ax/models/tests/test_posterior_mean.py`

 * *Files identical despite different names*

### Comparing `ax-platform-0.3.2/ax/models/tests/test_random.py` & `ax-platform-0.3.3/ax/models/tests/test_random.py`

 * *Files identical despite different names*

### Comparing `ax-platform-0.3.2/ax/models/tests/test_randomforest.py` & `ax-platform-0.3.3/ax/models/tests/test_randomforest.py`

 * *Files identical despite different names*

### Comparing `ax-platform-0.3.2/ax/models/tests/test_rembo.py` & `ax-platform-0.3.3/ax/models/tests/test_rembo.py`

 * *Files identical despite different names*

### Comparing `ax-platform-0.3.2/ax/models/tests/test_rembo_initializer.py` & `ax-platform-0.3.3/ax/models/tests/test_rembo_initializer.py`

 * *Files identical despite different names*

### Comparing `ax-platform-0.3.2/ax/models/tests/test_sobol.py` & `ax-platform-0.3.3/ax/models/tests/test_sobol.py`

 * *Files identical despite different names*

### Comparing `ax-platform-0.3.2/ax/models/tests/test_thompson.py` & `ax-platform-0.3.3/ax/models/tests/test_thompson.py`

 * *Files identical despite different names*

### Comparing `ax-platform-0.3.2/ax/models/tests/test_torch.py` & `ax-platform-0.3.3/ax/models/tests/test_torch.py`

 * *Files identical despite different names*

### Comparing `ax-platform-0.3.2/ax/models/tests/test_torch_model_utils.py` & `ax-platform-0.3.3/ax/models/tests/test_torch_model_utils.py`

 * *Files identical despite different names*

### Comparing `ax-platform-0.3.2/ax/models/tests/test_torch_utils.py` & `ax-platform-0.3.3/ax/models/tests/test_torch_utils.py`

 * *Files identical despite different names*

### Comparing `ax-platform-0.3.2/ax/models/tests/test_uniform.py` & `ax-platform-0.3.3/ax/models/tests/test_uniform.py`

 * *Files identical despite different names*

### Comparing `ax-platform-0.3.2/ax/models/torch/alebo.py` & `ax-platform-0.3.3/ax/models/torch/alebo.py`

 * *Files 2% similar despite different names*

```diff
@@ -20,14 +20,15 @@
 from ax.models.random.alebo_initializer import ALEBOInitializer
 from ax.models.torch.botorch import BotorchModel
 from ax.models.torch.botorch_defaults import get_NEI
 from ax.models.torch.utils import _datasets_to_legacy_inputs
 from ax.models.torch_base import TorchGenResults, TorchModel, TorchOptConfig
 from ax.utils.common.docutils import copy_doc
 from ax.utils.common.logger import get_logger
+from ax.utils.common.typeutils import checked_cast
 from botorch.acquisition.acquisition import AcquisitionFunction
 from botorch.acquisition.analytic import ExpectedImprovement
 from botorch.acquisition.objective import PosteriorTransform
 from botorch.models.gp_regression import FixedNoiseGP
 from botorch.models.gpytorch import GPyTorchModel
 from botorch.models.model_list_gp_regression import ModelListGP
 from botorch.optim.fit import fit_gpytorch_mll_scipy
@@ -39,14 +40,15 @@
 from gpytorch.distributions.multivariate_normal import MultivariateNormal
 from gpytorch.kernels.kernel import Kernel
 from gpytorch.kernels.rbf_kernel import postprocess_rbf
 from gpytorch.kernels.scale_kernel import ScaleKernel
 from gpytorch.mlls.exact_marginal_log_likelihood import ExactMarginalLogLikelihood
 from scipy.optimize import approx_fprime
 from torch import Tensor
+from torch.nn.parameter import Parameter
 
 
 logger: Logger = get_logger(__name__)
 
 
 class ALEBOKernel(Kernel):
     """The kernel for ALEBO.
@@ -94,15 +96,15 @@
         last_dim_is_batch: bool = False,
         **params: Any,
     ) -> Tensor:
         """Compute kernel distance."""
         # Unpack Uvec into an upper triangular matrix U
         shapeU = self.Uvec.shape[:-1] + torch.Size([self.d, self.d])
         U_t = torch.zeros(shapeU, dtype=self.B.dtype, device=self.B.device)
-        U_t[..., self.triu_indx[1], self.triu_indx[0]] = self.Uvec
+        U_t[..., self.triu_indx[1], self.triu_indx[0]] = checked_cast(Tensor, self.Uvec)
         # Compute kernel distance
         z1 = torch.matmul(x1, U_t)
         z2 = torch.matmul(x2, U_t)
 
         diff = self.covar_dist(
             z1,
             z2,
@@ -390,19 +392,19 @@
     # Set mean constant
     # pyre-fixme[16]: `Optional` has no attribute `raw_constant`.
     m_b.mean_module.raw_constant.requires_grad_(False)
     m_b.mean_module.raw_constant.copy_(mean_constant_batch)
     m_b.mean_module.raw_constant.requires_grad_(True)
     # Set output scale
     m_b.covar_module.raw_outputscale.requires_grad_(False)
-    m_b.covar_module.raw_outputscale.copy_(output_scale_batch)
+    checked_cast(Parameter, m_b.covar_module.raw_outputscale).copy_(output_scale_batch)
     m_b.covar_module.raw_outputscale.requires_grad_(True)
     # Set Uvec
     m_b.covar_module.base_kernel.Uvec.requires_grad_(False)
-    m_b.covar_module.base_kernel.Uvec.copy_(Uvec_batch)
+    checked_cast(Parameter, m_b.covar_module.base_kernel.Uvec).copy_(Uvec_batch)
     m_b.covar_module.base_kernel.Uvec.requires_grad_(True)
     m_b.eval()
     return m_b
 
 
 def extract_map_statedict(
     m_b: Union[ALEBOGP, ModelListGP], num_outputs: int
```

### Comparing `ax-platform-0.3.2/ax/models/torch/botorch.py` & `ax-platform-0.3.3/ax/models/torch/botorch.py`

 * *Files identical despite different names*

### Comparing `ax-platform-0.3.2/ax/models/torch/botorch_defaults.py` & `ax-platform-0.3.3/ax/models/torch/botorch_defaults.py`

 * *Files identical despite different names*

### Comparing `ax-platform-0.3.2/ax/models/torch/botorch_kg.py` & `ax-platform-0.3.3/ax/models/torch/botorch_kg.py`

 * *Files identical despite different names*

### Comparing `ax-platform-0.3.2/ax/models/torch/botorch_mes.py` & `ax-platform-0.3.3/ax/models/torch/botorch_mes.py`

 * *Files identical despite different names*

### Comparing `ax-platform-0.3.2/ax/models/torch/botorch_modular/acquisition.py` & `ax-platform-0.3.3/ax/models/torch/botorch_modular/acquisition.py`

 * *Files identical despite different names*

### Comparing `ax-platform-0.3.2/ax/models/torch/botorch_modular/model.py` & `ax-platform-0.3.3/ax/models/torch/botorch_modular/model.py`

 * *Files identical despite different names*

### Comparing `ax-platform-0.3.2/ax/models/torch/botorch_modular/multi_fidelity.py` & `ax-platform-0.3.3/ax/models/torch/botorch_modular/multi_fidelity.py`

 * *Files identical despite different names*

### Comparing `ax-platform-0.3.2/ax/models/torch/botorch_modular/optimizer_argparse.py` & `ax-platform-0.3.3/ax/models/torch/botorch_modular/optimizer_argparse.py`

 * *Files identical despite different names*

### Comparing `ax-platform-0.3.2/ax/models/torch/botorch_modular/surrogate.py` & `ax-platform-0.3.3/ax/models/torch/botorch_modular/surrogate.py`

 * *Files 2% similar despite different names*

```diff
@@ -7,21 +7,25 @@
 from __future__ import annotations
 
 import dataclasses
 import inspect
 import warnings
 from copy import deepcopy
 from logging import Logger
+
 from typing import Any, Dict, Iterable, List, Mapping, Optional, Sequence, Tuple, Type
 
 import torch
 from ax.core.search_space import SearchSpaceDigest
 from ax.core.types import TCandidateMetadata
 from ax.exceptions.core import AxWarning, UnsupportedError, UserInputError
 from ax.models.model_utils import best_in_sample_point
+from ax.models.torch.botorch_modular.input_constructors.covar_modules import (
+    covar_module_argparse,
+)
 from ax.models.torch.botorch_modular.utils import (
     choose_model_class,
     convert_to_block_design,
     fit_botorch_model,
     use_model_list,
 )
 from ax.models.torch.utils import (
@@ -368,18 +372,19 @@
         self._training_data = datasets
 
         (
             fidelity_features,
             task_feature,
             submodel_input_transforms,
         ) = self._extract_construct_model_list_kwargs(
-            fidelity_features=kwargs.get(Keys.FIDELITY_FEATURES, []),
-            task_features=kwargs.get(Keys.TASK_FEATURES, []),
-            robust_digest=kwargs.get("robust_digest", None),
+            fidelity_features=kwargs.pop(Keys.FIDELITY_FEATURES, []),
+            task_features=kwargs.pop(Keys.TASK_FEATURES, []),
+            robust_digest=kwargs.pop("robust_digest", None),
         )
+        input_constructor_kwargs = {**self.model_options, **(kwargs or {})}
 
         submodels = []
         for m, dataset in zip(metric_names, datasets):
             model_cls = self.botorch_model_class or choose_model_class(
                 datasets=[dataset], search_space_digest=not_none(search_space_digest)
             )
 
@@ -387,16 +392,15 @@
                 logger.warning(f"Metric {m} not in training data.")
                 continue
 
             formatted_model_inputs = model_cls.construct_inputs(
                 training_data=dataset,
                 fidelity_features=fidelity_features,
                 task_feature=task_feature,
-                categorical_features=kwargs.get("categorical_features", None),
-                **self.model_options,
+                **input_constructor_kwargs,
             )
             # Add input / outcome transforms.
             # TODO: The use of `inspect` here is not ideal. We should find a better
             # way to filter the arguments. See the comment in `Surrogate.construct`
             # regarding potential use of a `ModelFactory` in the future.
             model_cls_args = inspect.getfullargspec(model_cls).args
             self._set_formatted_inputs(
@@ -457,15 +461,29 @@
                     f"The BoTorch model class {self.botorch_model_class} does not "
                     f"support the input {input_name}."
                 )
             if input_class is not None and input_object is not None:  # pragma: no cover
                 raise RuntimeError(f"Got both a class and an object for {input_name}.")
             if input_class is not None:
                 input_options = input_options or {}
-                formatted_model_inputs[input_name] = input_class(**input_options)
+
+                if input_name == "covar_module":
+                    covar_module_with_defaults = covar_module_argparse(
+                        input_class,
+                        dataset=dataset,
+                        botorch_model_class=self.botorch_model_class,
+                        **input_options,
+                    )
+
+                    formatted_model_inputs[input_name] = input_class(
+                        **covar_module_with_defaults
+                    )
+                else:
+                    formatted_model_inputs[input_name] = input_class(**input_options)
+
             else:
                 formatted_model_inputs[input_name] = input_object
 
         # Construct input perturbation if doing robust optimization.
         if robust_digest is not None:
             if len(robust_digest["environmental_variables"]):
                 # TODO[T131759269]: support env variables.
```

### Comparing `ax-platform-0.3.2/ax/models/torch/botorch_modular/utils.py` & `ax-platform-0.3.3/ax/models/torch/botorch_modular/utils.py`

 * *Files identical despite different names*

### Comparing `ax-platform-0.3.2/ax/models/torch/botorch_moo.py` & `ax-platform-0.3.3/ax/models/torch/botorch_moo.py`

 * *Files identical despite different names*

### Comparing `ax-platform-0.3.2/ax/models/torch/botorch_moo_defaults.py` & `ax-platform-0.3.3/ax/models/torch/botorch_moo_defaults.py`

 * *Files identical despite different names*

### Comparing `ax-platform-0.3.2/ax/models/torch/cbo_lcea.py` & `ax-platform-0.3.3/ax/models/torch/cbo_lcea.py`

 * *Files identical despite different names*

### Comparing `ax-platform-0.3.2/ax/models/torch/cbo_lcem.py` & `ax-platform-0.3.3/ax/models/torch/cbo_lcem.py`

 * *Files identical despite different names*

### Comparing `ax-platform-0.3.2/ax/models/torch/cbo_sac.py` & `ax-platform-0.3.3/ax/models/torch/cbo_sac.py`

 * *Files identical despite different names*

### Comparing `ax-platform-0.3.2/ax/models/torch/fully_bayesian.py` & `ax-platform-0.3.3/ax/models/torch/fully_bayesian.py`

 * *Files identical despite different names*

### Comparing `ax-platform-0.3.2/ax/models/torch/fully_bayesian_model_utils.py` & `ax-platform-0.3.3/ax/models/torch/fully_bayesian_model_utils.py`

 * *Files 3% similar despite different names*

```diff
@@ -173,18 +173,23 @@
 
 
 # pyre-fixme[24]: Generic type `dict` expects 2 type parameters, use `typing.Dict`
 #  to avoid runtime subscripting errors.
 def load_mcmc_samples_to_model(model: GPyTorchModel, mcmc_samples: Dict) -> None:
     """Load MCMC samples into GPyTorchModel."""
     if "noise" in mcmc_samples:
+        # pyre-ignore Undefined attribute [16]: `torch._tensor.Tensor` has
+        # no attribute `noise`.
         model.likelihood.noise_covar.noise = (
             mcmc_samples["noise"]
             .detach()
             .clone()
+            # pyre-ignore Undefined attribute [16]: Item `torch._tensor.Tensor` of
+            # `typing.Union[torch._tensor.Tensor, torch.nn.modules.module.Module]`
+            # has no attribute `noise`.
             .view(model.likelihood.noise_covar.noise.shape)
             .clamp_min(MIN_INFERRED_NOISE_LEVEL)
         )
     model.covar_module.base_kernel.lengthscale = (
         mcmc_samples["lengthscale"]
         .detach()
         .clone()
```

### Comparing `ax-platform-0.3.2/ax/models/torch/posterior_mean.py` & `ax-platform-0.3.3/ax/models/torch/posterior_mean.py`

 * *Files identical despite different names*

### Comparing `ax-platform-0.3.2/ax/models/torch/randomforest.py` & `ax-platform-0.3.3/ax/models/torch/randomforest.py`

 * *Files identical despite different names*

### Comparing `ax-platform-0.3.2/ax/models/torch/rembo.py` & `ax-platform-0.3.3/ax/models/torch/rembo.py`

 * *Files identical despite different names*

### Comparing `ax-platform-0.3.2/ax/models/torch/tests/test_acquisition.py` & `ax-platform-0.3.3/ax/models/torch/tests/test_acquisition.py`

 * *Files identical despite different names*

### Comparing `ax-platform-0.3.2/ax/models/torch/tests/test_model.py` & `ax-platform-0.3.3/ax/models/torch/tests/test_model.py`

 * *Files identical despite different names*

### Comparing `ax-platform-0.3.2/ax/models/torch/tests/test_multi_fidelity.py` & `ax-platform-0.3.3/ax/models/torch/tests/test_multi_fidelity.py`

 * *Files identical despite different names*

### Comparing `ax-platform-0.3.2/ax/models/torch/tests/test_optimizer_argparse.py` & `ax-platform-0.3.3/ax/models/torch/tests/test_optimizer_argparse.py`

 * *Files identical despite different names*

### Comparing `ax-platform-0.3.2/ax/models/torch/tests/test_surrogate.py` & `ax-platform-0.3.3/ax/models/torch/tests/test_surrogate.py`

 * *Files 4% similar despite different names*

```diff
@@ -718,24 +718,52 @@
             search_space_digest=search_space_digest,
         )
         self.assertIsInstance(surrogate.model, MixedSingleTaskGP)
         # _ignore_X_dims_scaling_check is the easiest way to check cat dims.
         self.assertEqual(surrogate.model._ignore_X_dims_scaling_check, [0])
         covar_module = checked_cast(Kernel, surrogate.model.covar_module)
         self.assertEqual(
-            covar_module.kernels[0].base_kernel.kernels[1].active_dims.tolist(), [0]
+            # pyre-ignore Call error [29]: `typing.Union[BoundMethod[typing.Callable
+            # (torch._C._TensorBase.__getitem__)[[Named(self, torch._C._TensorBase),
+            # Named(indices, typing.Union[None, typing.List[typing.Any], int, slice,
+            # torch._tensor.Tensor, typing.Tuple[typing.Any, ...]])], torch._tensor.
+            # Tensor], torch._tensor.Tensor], torch._tensor.Tensor, torch.nn.modules.
+            # module.Module]` is not a function.
+            covar_module.kernels[0].base_kernel.kernels[1].active_dims.tolist(),
+            [0],
         )
         self.assertEqual(
-            covar_module.kernels[0].base_kernel.kernels[0].active_dims.tolist(), [1, 2]
+            # pyre-ignore Call error [29]: `typing.Union[BoundMethod[typing.Callable
+            # (torch._C._TensorBase.__getitem__)[[Named(self, torch._C._TensorBase),
+            # Named(indices, typing.Union[None, typing.List[typing.Any], int, slice,
+            # torch._tensor.Tensor, typing.Tuple[typing.Any, ...]])], torch._tensor.
+            # Tensor], torch._tensor.Tensor], torch._tensor.Tensor, torch.nn.modules.
+            # module.Module]` is not a function.
+            covar_module.kernels[0].base_kernel.kernels[0].active_dims.tolist(),
+            [1, 2],
         )
         self.assertEqual(
-            covar_module.kernels[1].base_kernel.kernels[1].active_dims.tolist(), [0]
+            # pyre-ignore Call error [29]: `typing.Union[BoundMethod[typing.Callable
+            # (torch._C._TensorBase.__getitem__)[[Named(self, torch._C._TensorBase),
+            # Named(indices, typing.Union[None, typing.List[typing.Any], int, slice,
+            # torch._tensor.Tensor, typing.Tuple[typing.Any, ...]])], torch._tensor.
+            # Tensor], torch._tensor.Tensor], torch._tensor.Tensor, torch.nn.modules.
+            # module.Module]` is not a function.
+            covar_module.kernels[1].base_kernel.kernels[1].active_dims.tolist(),
+            [0],
         )
         self.assertEqual(
-            covar_module.kernels[1].base_kernel.kernels[0].active_dims.tolist(), [1, 2]
+            # pyre-ignore Call error [29]: `typing.Union[BoundMethod[typing.Callable
+            # (torch._C._TensorBase.__getitem__)[[Named(self, torch._C._TensorBase),
+            # Named(indices, typing.Union[None, typing.List[typing.Any], int, slice,
+            # torch._tensor.Tensor, typing.Tuple[typing.Any, ...]])], torch._tensor.
+            # Tensor], torch._tensor.Tensor], torch._tensor.Tensor, torch.nn.modules.
+            # module.Module]` is not a function.
+            covar_module.kernels[1].base_kernel.kernels[0].active_dims.tolist(),
+            [1, 2],
         )
         # With modellist.
         training_data = [self.training_data[0], self.training_data[0]]
         surrogate = Surrogate(allow_batched_models=False)
         surrogate.fit(
             datasets=training_data,
             metric_names=self.original_metric_names,
@@ -827,34 +855,31 @@
     def test_construct_per_outcome_options(
         self, mock_MTGP_construct_inputs: Mock
     ) -> None:
         self.surrogate.construct(
             datasets=self.fixed_noise_training_data,
             metric_names=self.outcomes,
             task_features=self.task_features,
+            output_tasks=[2],
         )
         # Should construct inputs for MTGP twice.
         self.assertEqual(len(mock_MTGP_construct_inputs.call_args_list), 2)
         # First construct inputs should be called for MTGP with training data #0.
         for idx in range(len(mock_MTGP_construct_inputs.call_args_list)):
             self.assertEqual(
                 # `call_args` is a tuple of (args, kwargs), and we check kwargs.
                 mock_MTGP_construct_inputs.call_args_list[idx][1],
                 {
                     "fidelity_features": [],
                     "task_feature": self.task_features[0],
-                    "categorical_features": None,
-                    # TODO: Figure out how to handle Multitask GPs and construct-inputs.
-                    # I believe this functionality with modlular botorch model is
-                    # currently broken as MultiTaskGP.construct_inputs expects a dict
-                    # mapping string keys (outcomes) to input datasets
                     "training_data": FixedNoiseDataset(
                         X=self.Xs[idx], Y=self.Ys[idx], Yvar=self.Yvars[idx]
                     ),
                     "rank": 1,
+                    "output_tasks": [2],
                 },
             )
 
     @patch.object(
         MultiTaskGP,
         "construct_inputs",
         wraps=MultiTaskGP.construct_inputs,
```

### Comparing `ax-platform-0.3.2/ax/models/torch/tests/test_utils.py` & `ax-platform-0.3.3/ax/models/torch/tests/test_utils.py`

 * *Files identical despite different names*

### Comparing `ax-platform-0.3.2/ax/models/torch/utils.py` & `ax-platform-0.3.3/ax/models/torch/utils.py`

 * *Files identical despite different names*

### Comparing `ax-platform-0.3.2/ax/models/torch_base.py` & `ax-platform-0.3.3/ax/models/torch_base.py`

 * *Files identical despite different names*

### Comparing `ax-platform-0.3.2/ax/models/types.py` & `ax-platform-0.3.3/ax/models/types.py`

 * *Files identical despite different names*

### Comparing `ax-platform-0.3.2/ax/models/winsorization_config.py` & `ax-platform-0.3.3/ax/models/winsorization_config.py`

 * *Files identical despite different names*

### Comparing `ax-platform-0.3.2/ax/plot/bandit_rollout.py` & `ax-platform-0.3.3/ax/plot/bandit_rollout.py`

 * *Files identical despite different names*

### Comparing `ax-platform-0.3.2/ax/plot/base.py` & `ax-platform-0.3.3/ax/plot/base.py`

 * *Files identical despite different names*

### Comparing `ax-platform-0.3.2/ax/plot/color.py` & `ax-platform-0.3.3/ax/plot/color.py`

 * *Files identical despite different names*

### Comparing `ax-platform-0.3.2/ax/plot/contour.py` & `ax-platform-0.3.3/ax/plot/contour.py`

 * *Files identical despite different names*

### Comparing `ax-platform-0.3.2/ax/plot/css/base.css` & `ax-platform-0.3.3/ax/plot/css/base.css`

 * *Files identical despite different names*

### Comparing `ax-platform-0.3.2/ax/plot/diagnostic.py` & `ax-platform-0.3.3/ax/plot/diagnostic.py`

 * *Files identical despite different names*

### Comparing `ax-platform-0.3.2/ax/plot/feature_importances.py` & `ax-platform-0.3.3/ax/plot/feature_importances.py`

 * *Files 2% similar despite different names*

```diff
@@ -72,15 +72,15 @@
         )
     df = pd.DataFrame(importances)
 
     # plot_feature_importance expects index in first column
     df = df.reindex(columns=(["index"] + [a for a in df.columns if a != "index"]))
 
     plot_fi = plot_feature_importance_plotly(
-        df, "Absolute Feature Importances by Metric"
+        df, "Absolute Parameter Importances by Metric"
     )
     num_subplots = len(df.columns)
     num_features = len(df)
     # Include per-subplot margin for subplot titles (feature names).
     plot_fi["layout"]["height"] = num_subplots * (num_features + 1) * 50
     return plot_fi
 
@@ -194,15 +194,17 @@
             "pad": {
                 "t": -40
             },  # hack to put dropdown below title regardless of number of features
         }
     ]
     features = traces[0].y
     title = (
-        "Relative Feature Importances" if relative else "Absolute Feature Importances"
+        "Relative Parameter Importances"
+        if relative
+        else "Absolute Parameter Importances"
     )
     if importance_measure:
         title = title + " based on " + importance_measure
     layout = go.Layout(
         height=200 + len(features) * 20,
         hovermode="closest",
         margin=go.layout.Margin(
@@ -260,17 +262,17 @@
         go.Bar(y=df.index, x=df[column_name], name=column_name, orientation="h")
         for column_name in df.columns
     ]
     layout = go.Layout(
         margin=go.layout.Margin(l=250),  # noqa E741
         barmode="group",
         yaxis={"title": ""},
-        xaxis={"title": "Relative Feature importance"},
+        xaxis={"title": "Relative Parameter importance"},
         showlegend=False,
-        title="Relative Feature Importance per Metric",
+        title="Relative Parameter Importance per Metric",
     )
     return go.Figure(data=data, layout=layout)
 
 
 def plot_relative_feature_importance(model: ModelBridge) -> AxPlotConfig:
     """Wrapper method to convert plot_relative_feature_importance_plotly to
     AxPlotConfig"""
```

### Comparing `ax-platform-0.3.2/ax/plot/helper.py` & `ax-platform-0.3.3/ax/plot/helper.py`

 * *Files identical despite different names*

### Comparing `ax-platform-0.3.2/ax/plot/js/common/helpers.js` & `ax-platform-0.3.3/ax/plot/js/common/helpers.js`

 * *Files identical despite different names*

### Comparing `ax-platform-0.3.2/ax/plot/marginal_effects.py` & `ax-platform-0.3.3/ax/plot/marginal_effects.py`

 * *Files 2% similar despite different names*

```diff
@@ -32,15 +32,15 @@
 
     arm_dfs = []
     for arm in plot_data.in_sample.values():
         arm_df = pd.DataFrame(arm.parameters, index=[arm.name])
         arm_df["mean"] = arm.y_hat[metric]
         arm_df["sem"] = arm.se_hat[metric]
         arm_dfs.append(arm_df)
-    effect_table = marginal_effects(pd.concat(arm_dfs, 0))
+    effect_table = marginal_effects(pd.concat(arm_dfs, axis=0))
 
     varnames = effect_table["Name"].unique()
     # pyre-fixme[33]: Given annotation cannot contain `Any`.
     data: List[Any] = []
     for varname in varnames:
         var_df = effect_table[effect_table["Name"] == varname]
         data += [
```

### Comparing `ax-platform-0.3.2/ax/plot/parallel_coordinates.py` & `ax-platform-0.3.3/ax/plot/parallel_coordinates.py`

 * *Files identical despite different names*

### Comparing `ax-platform-0.3.2/ax/plot/pareto_frontier.py` & `ax-platform-0.3.3/ax/plot/pareto_frontier.py`

 * *Files identical despite different names*

### Comparing `ax-platform-0.3.2/ax/plot/pareto_utils.py` & `ax-platform-0.3.3/ax/plot/pareto_utils.py`

 * *Files 1% similar despite different names*

```diff
@@ -625,14 +625,15 @@
     # Finding the pareto frontier
     frontier_observations, f, obj_w, _ = get_pareto_frontier_and_configs(
         modelbridge=mb_reference,
         observation_features=obs_feats,
         observation_data=obs_data,
         objective_thresholds=dummy_rp,
         use_model_predictions=False,
+        transform_outcomes_and_configs=False,
     )
 
     # Need to reshuffle columns of `f` and `obj_w` to be consistent
     # with objective_orders.
     order = [
         objective_orders.index(metric_name)
         for metric_name in frontier_observations[0].data.metric_names
```

### Comparing `ax-platform-0.3.2/ax/plot/render.py` & `ax-platform-0.3.3/ax/plot/render.py`

 * *Files identical despite different names*

### Comparing `ax-platform-0.3.2/ax/plot/scatter.py` & `ax-platform-0.3.3/ax/plot/scatter.py`

 * *Files identical despite different names*

### Comparing `ax-platform-0.3.2/ax/plot/slice.py` & `ax-platform-0.3.3/ax/plot/slice.py`

 * *Files identical despite different names*

### Comparing `ax-platform-0.3.2/ax/plot/table_view.py` & `ax-platform-0.3.3/ax/plot/table_view.py`

 * *Files identical despite different names*

### Comparing `ax-platform-0.3.2/ax/plot/tests/long_running/test_pareto_utils.py` & `ax-platform-0.3.3/ax/plot/tests/long_running/test_pareto_utils.py`

 * *Files identical despite different names*

### Comparing `ax-platform-0.3.2/ax/plot/tests/test_contours.py` & `ax-platform-0.3.3/ax/plot/tests/test_contours.py`

 * *Files identical despite different names*

### Comparing `ax-platform-0.3.2/ax/plot/tests/test_diagnostic.py` & `ax-platform-0.3.3/ax/plot/tests/test_diagnostic.py`

 * *Files identical despite different names*

### Comparing `ax-platform-0.3.2/ax/plot/tests/test_feature_importances.py` & `ax-platform-0.3.3/ax/plot/tests/test_feature_importances.py`

 * *Files identical despite different names*

### Comparing `ax-platform-0.3.2/ax/plot/tests/test_fitted_scatter.py` & `ax-platform-0.3.3/ax/plot/tests/test_fitted_scatter.py`

 * *Files identical despite different names*

### Comparing `ax-platform-0.3.2/ax/plot/tests/test_helper.py` & `ax-platform-0.3.3/ax/plot/tests/test_helper.py`

 * *Files identical despite different names*

### Comparing `ax-platform-0.3.2/ax/plot/tests/test_parallel_coordinates.py` & `ax-platform-0.3.3/ax/plot/tests/test_parallel_coordinates.py`

 * *Files identical despite different names*

### Comparing `ax-platform-0.3.2/ax/plot/tests/test_pareto_utils.py` & `ax-platform-0.3.3/ax/plot/tests/test_pareto_utils.py`

 * *Files identical despite different names*

### Comparing `ax-platform-0.3.2/ax/plot/tests/test_slices.py` & `ax-platform-0.3.3/ax/plot/tests/test_slices.py`

 * *Files identical despite different names*

### Comparing `ax-platform-0.3.2/ax/plot/tests/test_tile_fitted.py` & `ax-platform-0.3.3/ax/plot/tests/test_tile_fitted.py`

 * *Files identical despite different names*

### Comparing `ax-platform-0.3.2/ax/plot/tests/test_traces.py` & `ax-platform-0.3.3/ax/plot/tests/test_traces.py`

 * *Files identical despite different names*

### Comparing `ax-platform-0.3.2/ax/plot/trace.py` & `ax-platform-0.3.3/ax/plot/trace.py`

 * *Files identical despite different names*

### Comparing `ax-platform-0.3.2/ax/runners/botorch_test_problem.py` & `ax-platform-0.3.3/ax/runners/botorch_test_problem.py`

 * *Files identical despite different names*

### Comparing `ax-platform-0.3.2/ax/runners/simulated_backend.py` & `ax-platform-0.3.3/ax/runners/simulated_backend.py`

 * *Files identical despite different names*

### Comparing `ax-platform-0.3.2/ax/runners/synthetic.py` & `ax-platform-0.3.3/ax/runners/synthetic.py`

 * *Files identical despite different names*

### Comparing `ax-platform-0.3.2/ax/runners/tests/test_torchx.py` & `ax-platform-0.3.3/ax/runners/tests/test_torchx.py`

 * *Files identical despite different names*

### Comparing `ax-platform-0.3.2/ax/runners/torchx.py` & `ax-platform-0.3.3/ax/runners/torchx.py`

 * *Files identical despite different names*

### Comparing `ax-platform-0.3.2/ax/service/ax_client.py` & `ax-platform-0.3.3/ax/service/ax_client.py`

 * *Files 2% similar despite different names*

```diff
@@ -1461,14 +1461,24 @@
 
     @property
     def metric_names(self) -> Set[str]:
         """Returns the names of all metrics on the attached experiment."""
         return set(self.experiment.metrics)
 
     @property
+    def early_stopping_strategy(self) -> Optional[BaseEarlyStoppingStrategy]:
+        """The early stopping strategy used on the experiment."""
+        return self._early_stopping_strategy
+
+    @early_stopping_strategy.setter
+    def early_stopping_strategy(self, ess: BaseEarlyStoppingStrategy) -> None:
+        """Update the early stopping strategy."""
+        self._early_stopping_strategy = ess
+
+    @property
     def global_stopping_strategy(self) -> Optional[BaseGlobalStoppingStrategy]:
         """The global stopping strategy used on the experiment."""
         return self._global_stopping_strategy
 
     @global_stopping_strategy.setter
     def global_stopping_strategy(self, gss: BaseGlobalStoppingStrategy) -> None:
         """Update the global stopping strategy."""
```

### Comparing `ax-platform-0.3.2/ax/service/interactive_loop.py` & `ax-platform-0.3.3/ax/service/interactive_loop.py`

 * *Files identical despite different names*

### Comparing `ax-platform-0.3.2/ax/service/managed_loop.py` & `ax-platform-0.3.3/ax/service/managed_loop.py`

 * *Files identical despite different names*

### Comparing `ax-platform-0.3.2/ax/service/scheduler.py` & `ax-platform-0.3.3/ax/service/scheduler.py`

 * *Files 1% similar despite different names*

```diff
@@ -43,14 +43,15 @@
     AxError,
     DataRequiredError,
     OptimizationComplete,
     UnsupportedError,
     UserInputError,
 )
 from ax.exceptions.generation_strategy import MaxParallelismReachedException
+from ax.modelbridge.base import ModelBridge
 from ax.modelbridge.generation_strategy import GenerationStrategy
 
 from ax.modelbridge.modelbridge_utils import (
     get_pending_observation_features_based_on_trial_status,
 )
 from ax.plot.pareto_utils import infer_reference_point_from_experiment
 from ax.service.utils.best_point_mixin import BestPointMixin
@@ -771,21 +772,17 @@
                 self.logger.warn(
                     "MetricFetchE INFO: Sweep aborted due to an exceeded error rate, "
                     "which was primarily caused by failure to fetch metrics. Please "
                     "check if anything could cause your metrics to be flakey or "
                     "broken."
                 )
 
-            raise FailureRateExceededError(
-                FAILURE_EXCEEDED_MSG.format(
-                    f_rate=self.options.tolerated_trial_failure_rate,
-                    n_failed=num_bad_in_scheduler,
-                    n_ran=num_ran_in_scheduler,
-                    min_failed=self.options.min_failed_trials_for_failure_rate_check,
-                )
+            raise self._get_failure_rate_exceeded_error(
+                num_bad_in_scheduler=num_bad_in_scheduler,
+                num_ran_in_scheduler=num_ran_in_scheduler,
             )
 
     def run_trials_and_yield_results(
         self,
         max_trials: int,
         ignore_global_stopping_strategy: bool = False,
         timeout_hours: Optional[int] = None,
@@ -1474,15 +1471,21 @@
         """
 
         # pyre-fixme[3]: Return type must be annotated.
         # pyre-fixme[2]: Parameter must be annotated.
         def _process_trial(trial):
             if trial.index in metadata:
                 trial.update_run_metadata(metadata=metadata[trial.index])
-                trial.mark_running(no_runner_required=True)
+                try:
+                    trial.mark_running(no_runner_required=True)
+                except ValueError as e:
+                    self.logger.warn(
+                        "Unable to mark trial as RUNNING due to the following error:\n"
+                        + str(e)
+                    )
             else:
                 self.logger.debug(
                     f"Trial {trial.index} did not deploy, status: {trial.status}."
                 )
 
         new_generator_runs = []
         for trial in existing_trials:
@@ -1741,7 +1744,40 @@
         trial: BaseTrial,
         metric_name: Optional[str] = None,
         metric_fetch_e: Optional[MetricFetchE] = None,
     ) -> TrialStatus:
         trial.mark_failed(unsafe=True)
 
         return TrialStatus.FAILED
+
+    def _get_failure_rate_exceeded_error(
+        self,
+        num_bad_in_scheduler: int,
+        num_ran_in_scheduler: int,
+    ) -> FailureRateExceededError:
+        return FailureRateExceededError(
+            FAILURE_EXCEEDED_MSG.format(
+                f_rate=self.options.tolerated_trial_failure_rate,
+                n_failed=num_bad_in_scheduler,
+                n_ran=num_ran_in_scheduler,
+                min_failed=self.options.min_failed_trials_for_failure_rate_check,
+            )
+        )
+
+
+def get_fitted_model_bridge(scheduler: Scheduler) -> ModelBridge:
+    """Returns a fitted ModelBridge object. If the model is fit already, directly
+    returns the already fitted model. Otherwise, fits and returns a new one.
+
+    Args:
+        scheduler: The scheduler object from which to get the fitted model.
+
+    Returns:
+        A ModelBridge object fitted to the observations of the scheduler's experiment.
+    """
+    gs = scheduler.generation_strategy  # GenerationStrategy
+    model_bridge = gs.model  # Optional[ModelBridge]
+    if model_bridge is None:  # Need to re-fit the model.
+        data = scheduler.experiment.fetch_data()
+        gs._fit_or_update_current_model(data=data)
+        model_bridge = cast(ModelBridge, gs.model)
+    return model_bridge
```

### Comparing `ax-platform-0.3.2/ax/service/tests/test_ax_client.py` & `ax-platform-0.3.3/ax/service/tests/test_ax_client.py`

 * *Files 2% similar despite different names*

```diff
@@ -362,34 +362,37 @@
             opt_config.objective.objectives[1].minimize,
             False,
         )
         self.assertEqual(
             # pyre-fixme[16]: `Optional` has no attribute `objective_thresholds`.
             opt_config.objective_thresholds[0],
             ObjectiveThreshold(
-                metric=Metric(name="foo"),
+                metric=Metric(name="foo", lower_is_better=True),
                 bound=3.1,
                 relative=False,
                 op=ComparisonOp.LEQ,
             ),
         )
         self.assertEqual(
             opt_config.objective_thresholds[1],
             ObjectiveThreshold(
-                metric=Metric(name="bar"),
+                metric=Metric(name="bar", lower_is_better=False),
                 bound=1.0,
                 relative=False,
                 op=ComparisonOp.GEQ,
             ),
         )
         self.assertEqual(
             # pyre-fixme[16]: `Optional` has no attribute `outcome_constraints`.
             opt_config.outcome_constraints[0],
             OutcomeConstraint(
-                metric=Metric(name="baz"), bound=7.2, relative=True, op=ComparisonOp.GEQ
+                metric=Metric(name="baz", lower_is_better=False),
+                bound=7.2,
+                relative=True,
+                op=ComparisonOp.GEQ,
             ),
         )
 
     def test_set_optimization_config_to_single_objective(self) -> None:
         ax_client = AxClient()
         ax_client.create_experiment(
             name="test",
@@ -415,15 +418,18 @@
             opt_config.objective.minimize,
             True,
         )
         self.assertEqual(
             # pyre-fixme[16]: `Optional` has no attribute `outcome_constraints`.
             opt_config.outcome_constraints[0],
             OutcomeConstraint(
-                metric=Metric(name="baz"), bound=7.2, relative=True, op=ComparisonOp.GEQ
+                metric=Metric(name="baz", lower_is_better=False),
+                bound=7.2,
+                relative=True,
+                op=ComparisonOp.GEQ,
             ),
         )
 
     def test_set_optimization_config_without_objectives_raises_error(self) -> None:
         ax_client = AxClient()
         ax_client.create_experiment(
             name="test",
@@ -809,24 +815,24 @@
                 values=["one", "two", "three"],
             ),
         )
         self.assertEqual(
             # pyre-fixme[16]: `Optional` has no attribute `optimization_config`.
             ax_client._experiment.optimization_config.outcome_constraints[0],
             OutcomeConstraint(
-                metric=Metric(name="some_metric"),
+                metric=Metric(name="some_metric", lower_is_better=False),
                 op=ComparisonOp.GEQ,
                 bound=3.0,
                 relative=False,
             ),
         )
         self.assertEqual(
             ax_client._experiment.optimization_config.outcome_constraints[1],
             OutcomeConstraint(
-                metric=Metric(name="some_metric"),
+                metric=Metric(name="some_metric", lower_is_better=True),
                 op=ComparisonOp.LEQ,
                 bound=4.0,
                 relative=False,
             ),
         )
         self.assertTrue(ax_client._experiment.optimization_config.objective.minimize)
         self.assertDictEqual(
@@ -1341,24 +1347,24 @@
         self.assertEqual(
             [t.relative for t in optimization_config.objective_thresholds],
             [False, False],
         )
         self.assertEqual(
             optimization_config.outcome_constraints[0],
             OutcomeConstraint(
-                metric=Metric(name="some_metric"),
+                metric=Metric(name="some_metric", lower_is_better=False),
                 op=ComparisonOp.GEQ,
                 bound=3.0,
                 relative=False,
             ),
         )
         self.assertEqual(
             optimization_config.outcome_constraints[1],
             OutcomeConstraint(
-                metric=Metric(name="some_metric"),
+                metric=Metric(name="some_metric", lower_is_better=True),
                 op=ComparisonOp.LEQ,
                 bound=4.0,
                 relative=False,
             ),
         )
         self.assertDictEqual(
             # pyre-fixme[16]: `Optional` has no attribute `_tracking_metrics`.
@@ -1547,20 +1553,14 @@
         # Can't update before completing.
         with self.assertRaisesRegex(ValueError, ".* not yet"):
             ax_client.update_trial_data(trial_index=idx, raw_data={"branin": (0, 0.0)})
         ax_client.complete_trial(trial_index=idx, raw_data={"branin": (0, 0.0)})
         # Cannot complete a trial twice, should use `update_trial_data`.
         with self.assertRaisesRegex(UnsupportedError, ".* already been completed"):
             ax_client.complete_trial(trial_index=idx, raw_data={"branin": (0, 0.0)})
-        # Cannot update trial data with observation for a metric it already has.
-        with self.assertRaisesRegex(ValueError, ".* contained an observation"):
-            ax_client.update_trial_data(trial_index=idx, raw_data={"branin": (0, 0.0)})
-        # Same as above, except objective name should be getting inferred.
-        with self.assertRaisesRegex(ValueError, ".* contained an observation"):
-            ax_client.update_trial_data(trial_index=idx, raw_data=1.0)
         ax_client.update_trial_data(trial_index=idx, raw_data={"m1": (1, 0.0)})
         metrics_in_data = ax_client.experiment.fetch_data().df["metric_name"].values
         self.assertNotIn("m1", metrics_in_data)
         self.assertIn("branin", metrics_in_data)
         # pyre-fixme[16]: `Optional` has no attribute `__getitem__`.
         self.assertEqual(ax_client.get_best_parameters()[0], params)
         params2, idy = ax_client.get_next_trial()
```

### Comparing `ax-platform-0.3.2/ax/service/tests/test_best_point.py` & `ax-platform-0.3.3/ax/service/tests/test_best_point.py`

 * *Files 13% similar despite different names*

```diff
@@ -95,7 +95,28 @@
         exp = get_experiment_with_trial()
         self.assertEqual(get_trace(exp), [])
 
     def test_get_hypervolume(self) -> None:
         # W/ empty data.
         exp = get_experiment_with_trial()
         self.assertEqual(BestPointMixin._get_hypervolume(exp, Mock()), 0.0)
+
+    def test_get_best_observed_value(self) -> None:
+        # Alias for easier access.
+        get_best = BestPointMixin._get_best_observed_value
+
+        # Single objective, minimize.
+        exp = get_experiment_with_observations(
+            observations=[[11], [10], [9], [15], [5]], minimize=True
+        )
+        self.assertEqual(get_best(exp), 5)
+        # Same experiment with maximize via new optimization config.
+        opt_conf = not_none(exp.optimization_config).clone()
+        opt_conf.objective.minimize = False
+        self.assertEqual(get_best(exp, opt_conf), 15)
+
+        # Scalarized.
+        exp = get_experiment_with_observations(
+            observations=[[1, 1], [2, 2], [3, 3]],
+            scalarized=True,
+        )
+        self.assertEqual(get_best(exp), 6)
```

### Comparing `ax-platform-0.3.2/ax/service/tests/test_best_point_utils.py` & `ax-platform-0.3.3/ax/service/tests/test_best_point_utils.py`

 * *Files identical despite different names*

### Comparing `ax-platform-0.3.2/ax/service/tests/test_early_stopping.py` & `ax-platform-0.3.3/ax/service/tests/test_early_stopping.py`

 * *Files identical despite different names*

### Comparing `ax-platform-0.3.2/ax/service/tests/test_global_stopping.py` & `ax-platform-0.3.3/ax/service/tests/test_global_stopping.py`

 * *Files identical despite different names*

### Comparing `ax-platform-0.3.2/ax/service/tests/test_instantiation_utils.py` & `ax-platform-0.3.3/ax/service/tests/test_instantiation_utils.py`

 * *Files identical despite different names*

### Comparing `ax-platform-0.3.2/ax/service/tests/test_interactive_loop.py` & `ax-platform-0.3.3/ax/service/tests/test_interactive_loop.py`

 * *Files identical despite different names*

### Comparing `ax-platform-0.3.2/ax/service/tests/test_managed_loop.py` & `ax-platform-0.3.3/ax/service/tests/test_managed_loop.py`

 * *Files identical despite different names*

### Comparing `ax-platform-0.3.2/ax/service/tests/test_report_utils.py` & `ax-platform-0.3.3/ax/service/tests/test_report_utils.py`

 * *Files identical despite different names*

### Comparing `ax-platform-0.3.2/ax/service/tests/test_scheduler.py` & `ax-platform-0.3.3/ax/service/tests/test_scheduler.py`

 * *Files 2% similar despite different names*

```diff
@@ -5,19 +5,20 @@
 # LICENSE file in the root directory of this source tree.
 
 import os
 from logging import WARNING
 from math import ceil
 from random import randint
 from tempfile import NamedTemporaryFile
-from typing import Any, Callable, Dict, Iterable, Optional, Set
-from unittest.mock import Mock, patch
+from typing import Any, Callable, cast, Dict, Iterable, Optional, Set
+from unittest.mock import Mock, patch, PropertyMock
 
 from ax.core.arm import Arm
 from ax.core.base_trial import BaseTrial, TrialStatus
+
 from ax.core.experiment import Experiment
 from ax.core.metric import Metric
 from ax.core.objective import Objective
 from ax.core.optimization_config import OptimizationConfig
 from ax.early_stopping.strategies import BaseEarlyStoppingStrategy
 from ax.exceptions.core import OptimizationComplete, UnsupportedError, UserInputError
 from ax.metrics.branin import BraninMetric
@@ -27,14 +28,15 @@
     get_pending_observation_features_based_on_trial_status,
 )
 from ax.modelbridge.registry import Models
 from ax.runners.synthetic import SyntheticRunner
 from ax.service.scheduler import (
     ExperimentStatusProperties,
     FailureRateExceededError,
+    get_fitted_model_bridge,
     OptimizationResult,
     Scheduler,
     SchedulerInternalError,
     SchedulerOptions,
 )
 from ax.service.utils.scheduler_options import TrialType
 from ax.service.utils.with_db_settings_base import WithDBSettingsBase
@@ -1193,7 +1195,83 @@
         for _ in range(5):
             sobol_run = sobol_generator.gen(n=1)
             self.branin_experiment.new_trial(generator_run=sobol_run)
         self.assertEqual(len(self.branin_experiment.trials), 5)
         should_stop, message = scheduler.completion_criterion()
         self.assertTrue(should_stop)
         self.assertEqual(message, "Exceeding the total number of trials.")
+
+    def test_get_fitted_model_bridge(self) -> None:
+        # setting up experiment and generation strategy
+        branin_experiment = Experiment(
+            name="branin_test_experiment",
+            search_space=get_branin_search_space(),
+            runner=SyntheticRunner(),
+            optimization_config=OptimizationConfig(
+                objective=Objective(
+                    metric=BraninMetric(name="branin", param_names=["x1", "x2"]),
+                    minimize=True,
+                ),
+            ),
+            is_test=True,
+        )
+        branin_experiment._properties[Keys.IMMUTABLE_SEARCH_SPACE_AND_OPT_CONF] = True
+        # generation strategy
+        NUM_SOBOL = 5
+        generation_strategy = GenerationStrategy(
+            steps=[
+                GenerationStep(
+                    model=Models.SOBOL, num_trials=NUM_SOBOL, max_parallelism=NUM_SOBOL
+                ),
+                GenerationStep(model=Models.GPEI, num_trials=-1),
+            ]
+        )
+        scheduler = Scheduler(
+            experiment=branin_experiment,
+            generation_strategy=generation_strategy,
+            options=SchedulerOptions(),
+        )
+        # need to run some trials to initialize the ModelBridge
+        scheduler.run_n_trials(max_trials=NUM_SOBOL + 1)
+
+        # testing path that refits the _model, if it is not already initialized
+        with patch.object(
+            GenerationStrategy,
+            "model",
+            new_callable=PropertyMock,
+            return_value=None,
+        ):
+            with patch.object(
+                GenerationStrategy,
+                "_fit_or_update_current_model",
+                wraps=scheduler.generation_strategy._fit_or_update_current_model,
+            ) as fit_model:
+                get_fitted_model_bridge(scheduler)
+                fit_model.assert_called_once()
+
+        # testing get_fitted_model_bridge
+        model_bridge = get_fitted_model_bridge(scheduler)
+
+        # testing compatibility with model_bridge.compute_model_fit_metrics
+        fit_metrics = model_bridge.compute_model_fit_metrics(
+            experiment=scheduler.experiment
+        )
+        r2 = fit_metrics.get("coefficient_of_determination")
+        self.assertIsInstance(r2, dict)
+        r2 = cast(Dict[str, float], r2)
+        self.assertTrue("branin" in r2)
+        r2_branin = r2["branin"]
+        self.assertIsInstance(r2_branin, float)
+
+        std = fit_metrics.get("std_of_the_standardized_error")
+        self.assertIsInstance(std, dict)
+        std = cast(Dict[str, float], std)
+        self.assertTrue("branin" in std)
+        std_branin = std["branin"]
+        self.assertIsInstance(std_branin, float)
+
+        # testing with empty metrics dict
+        empty_metrics = model_bridge.compute_model_fit_metrics(
+            experiment=scheduler.experiment, fit_metrics_dict={}
+        )
+        self.assertIsInstance(empty_metrics, dict)
+        self.assertTrue(len(empty_metrics) == 0)
```

### Comparing `ax-platform-0.3.2/ax/service/tests/test_with_db_settings_base.py` & `ax-platform-0.3.3/ax/service/tests/test_with_db_settings_base.py`

 * *Files identical despite different names*

### Comparing `ax-platform-0.3.2/ax/service/utils/best_point.py` & `ax-platform-0.3.3/ax/service/utils/best_point.py`

 * *Files identical despite different names*

### Comparing `ax-platform-0.3.2/ax/service/utils/best_point_mixin.py` & `ax-platform-0.3.3/ax/service/utils/best_point_mixin.py`

 * *Files 4% similar despite different names*

```diff
@@ -9,14 +9,15 @@
 from logging import Logger
 from typing import Dict, Iterable, List, Optional, Tuple
 
 import numpy as np
 import torch
 from ax.core.experiment import Experiment
 from ax.core.map_data import MapData
+from ax.core.objective import ScalarizedObjective
 from ax.core.optimization_config import (
     MultiObjectiveOptimizationConfig,
     OptimizationConfig,
 )
 from ax.core.types import TModelPredictArm, TParameterization
 from ax.modelbridge.generation_strategy import GenerationStrategy
 from ax.modelbridge.modelbridge_utils import (
@@ -290,14 +291,61 @@
         return best_point_utils.get_best_by_raw_objective_with_trial_index(
             experiment=experiment,
             optimization_config=optimization_config,
             trial_indices=trial_indices,
         )
 
     @staticmethod
+    def _get_best_observed_value(
+        experiment: Experiment,
+        optimization_config: Optional[OptimizationConfig] = None,
+        trial_indices: Optional[Iterable[int]] = None,
+    ) -> Optional[float]:
+        """Identifies the best objective value observed in the experiment
+        among the trials indicated by `trial_indices`.
+
+        Args:
+            experiment: The experiment to get the best objective value for.
+            optimization_config: Optimization config to use in place of the one stored
+                on the experiment.
+            trial_indices: Indices of trials for which to retrieve data. If None will
+                retrieve data from all available trials.
+
+        Returns:
+            The best objective value so far.
+        """
+        if optimization_config is None:
+            optimization_config = not_none(experiment.optimization_config)
+        if optimization_config.is_moo_problem:
+            raise NotImplementedError(  # pragma: no cover
+                "Please use `get_hypervolume` for multi-objective problems."
+            )
+
+        res = best_point_utils.get_best_by_raw_objective_with_trial_index(
+            experiment=experiment,
+            optimization_config=optimization_config,
+            trial_indices=trial_indices,
+        )
+
+        predictions = res[2] if res is not None else None
+        if predictions is None:
+            return None  # pragma: no cover
+
+        means = not_none(predictions)[0]
+        objective = optimization_config.objective
+        if isinstance(objective, ScalarizedObjective):
+            value = 0
+            for metric, weight in objective.metric_weights:
+                value += means[metric.name] * weight
+            return value
+        else:
+            name = objective.metric_names[0]
+            return means[name]
+
+    @staticmethod
     def _get_pareto_optimal_parameters(
         experiment: Experiment,
         generation_strategy: GenerationStrategy,
         optimization_config: Optional[OptimizationConfig] = None,
         trial_indices: Optional[Iterable[int]] = None,
         use_model_predictions: bool = True,
     ) -> Dict[int, Tuple[TParameterization, TModelPredictArm]]:
```

### Comparing `ax-platform-0.3.2/ax/service/utils/early_stopping.py` & `ax-platform-0.3.3/ax/service/utils/early_stopping.py`

 * *Files identical despite different names*

### Comparing `ax-platform-0.3.2/ax/service/utils/instantiation.py` & `ax-platform-0.3.3/ax/service/utils/instantiation.py`

 * *Files 2% similar despite different names*

```diff
@@ -112,25 +112,45 @@
     """
     This is a lightweight stateless class that bundles together instantiation utils.
     It is used both on its own and as a mixin to AxClient, with the intent that
     these methods can be overridden by its subclasses for specific use cases.
     """
 
     @staticmethod
+    def _get_deserialized_metric_kwargs(
+        metric_class: Type[Metric],
+        name: str,
+        metric_definitions: Optional[Dict[str, Dict[str, Any]]],
+    ) -> Dict[str, Any]:
+        """Get metric kwargs from metric_definitions if available and deserialize
+        if so.  Deserialization is necessary because they were serialized on creation"""
+        metric_kwargs = (metric_definitions or {}).get(name, {})
+        metric_class = metric_kwargs.pop("metric_class", metric_class)
+        metric_kwargs["name"] = name
+        metric_kwargs = metric_class.deserialize_init_args(metric_kwargs)
+        metric_kwargs.pop("name")
+        return metric_kwargs
+
+    @classmethod
     def _make_metric(
+        cls,
         name: str,
         lower_is_better: Optional[bool] = None,
         metric_class: Type[Metric] = Metric,
         for_opt_config: bool = False,
         metric_definitions: Optional[Dict[str, Dict[str, Any]]] = None,
     ) -> Metric:
         return metric_class(
             name=name,
             lower_is_better=lower_is_better,
-            **(metric_definitions or {}).get(name, {}),
+            **cls._get_deserialized_metric_kwargs(
+                name=name,
+                metric_definitions=metric_definitions,
+                metric_class=metric_class,
+            ),
         )
 
     @staticmethod
     def _get_parameter_type(python_type: TParameterType) -> ParameterType:
         for param_type, py_type in PARAMETER_PYTHON_TYPE_MAP.items():
             if py_type is python_type:
                 return param_type
@@ -437,14 +457,15 @@
         except ValueError:
             raise ValueError("Outcome constraint bound should be a float.")
         return OutcomeConstraint(
             cls._make_metric(
                 name=tokens[0],
                 for_opt_config=True,
                 metric_definitions=metric_definitions,
+                lower_is_better=op is ComparisonOp.LEQ,
             ),
             op=op,
             bound=bound,
             relative=rel,
         )
 
     @classmethod
```

### Comparing `ax-platform-0.3.2/ax/service/utils/report_utils.py` & `ax-platform-0.3.3/ax/service/utils/report_utils.py`

 * *Files 1% similar despite different names*

```diff
@@ -302,17 +302,17 @@
         - model_transitions: The arm numbers at which shifts in generation_strategy
             occur.
         - true_objective_metric_name: Name of the metric to use as the true objective.
         - early_stopping_strategy: Early stopping strategy used throughout the
             experiment; used for visualizing when curves are stopped.
         - limit_points_per_plot: Limit the number of points used per metric in
             each curve plot. Passed to `_get_curve_plot_dropdown`.
-        - global_sensitivity_analysis: If True, plot total Sobol indices for the model
-            parameters. If False, plot sensitivities based on GP kernel lengthscales.
-            Defaults to True.
+        - global_sensitivity_analysis: If True, plot total Variance-based sensitivity
+            analysis for the model parameters. If False, plot sensitivities based on
+            GP kernel lengthscales. Defaults to True.
     Returns:
         - a plot of objective value vs. trial index, to show experiment progression
         - a plot of objective value vs. range parameter values, only included if the
           model associated with generation_strategy can create predictions. This
           consists of:
 
             - a plot_slice plot if the search space contains one range parameter
@@ -387,15 +387,18 @@
 
             # sensitivity plot
             sens = None
             importance_measure = ""
             if global_sensitivity_analysis and isinstance(model, TorchModelBridge):
                 try:
                     sens = ax_parameter_sens(model, order="total")
-                    importance_measure = "Total Sobol Indices"
+                    importance_measure = (
+                        '<a href="https://en.wikipedia.org/wiki/Variance-based_'
+                        'sensitivity_analysis">Variance-based sensitivity analysis</a>'
+                    )
                 except NotImplementedError as e:
                     logger.info(f"Failed to compute global feature sensitivities: {e}")
             feature_importance_plot = plot_feature_importance_by_feature_plotly(
                 model=model,
                 # pyre-ignore [6]: In call for argument `sensitivity_values`,
                 # expected `Optional[Dict[str, Dict[str, Union[float, ndarray]]]]`
                 # but got `Dict[str, Dict[str, ndarray]]`.
```

### Comparing `ax-platform-0.3.2/ax/service/utils/scheduler_options.py` & `ax-platform-0.3.3/ax/service/utils/scheduler_options.py`

 * *Files identical despite different names*

### Comparing `ax-platform-0.3.2/ax/service/utils/with_db_settings_base.py` & `ax-platform-0.3.3/ax/service/utils/with_db_settings_base.py`

 * *Files identical despite different names*

### Comparing `ax-platform-0.3.2/ax/storage/botorch_modular_registry.py` & `ax-platform-0.3.3/ax/storage/botorch_modular_registry.py`

 * *Files 2% similar despite different names*

```diff
@@ -27,14 +27,15 @@
     qNoisyExpectedImprovement,
 )
 from botorch.acquisition.multi_objective.monte_carlo import (
     qExpectedHypervolumeImprovement,
     qNoisyExpectedHypervolumeImprovement,
 )
 from botorch.models import SaasFullyBayesianSingleTaskGP
+from botorch.models.fully_bayesian_multitask import SaasFullyBayesianMultiTaskGP
 
 # BoTorch `Model` imports
 from botorch.models.gp_regression import FixedNoiseGP, SingleTaskGP
 from botorch.models.gp_regression_fidelity import (
     FixedNoiseMultiFidelityGP,
     SingleTaskMultiFidelityGP,
 )
@@ -81,14 +82,15 @@
     FixedNoiseMultiTaskGP: "FixedNoiseMultiTaskGP",
     MixedSingleTaskGP: "MixedSingleTaskGP",
     ModelListGP: "ModelListGP",
     MultiTaskGP: "MultiTaskGP",
     SingleTaskGP: "SingleTaskGP",
     SingleTaskMultiFidelityGP: "SingleTaskMultiFidelityGP",
     SaasFullyBayesianSingleTaskGP: "SaasFullyBayesianSingleTaskGP",
+    SaasFullyBayesianMultiTaskGP: "SaasFullyBayesianMultiTaskGP",
 }
 
 
 """
 Mapping of Botorch `AcquisitionFunction` classes to class name strings.
 """
 ACQUISITION_FUNCTION_REGISTRY: Dict[Type[AcquisitionFunction], str] = {
```

### Comparing `ax-platform-0.3.2/ax/storage/json_store/decoder.py` & `ax-platform-0.3.3/ax/storage/json_store/decoder.py`

 * *Files identical despite different names*

### Comparing `ax-platform-0.3.2/ax/storage/json_store/decoders.py` & `ax-platform-0.3.3/ax/storage/json_store/decoders.py`

 * *Files identical despite different names*

### Comparing `ax-platform-0.3.2/ax/storage/json_store/encoder.py` & `ax-platform-0.3.3/ax/storage/json_store/encoder.py`

 * *Files identical despite different names*

### Comparing `ax-platform-0.3.2/ax/storage/json_store/encoders.py` & `ax-platform-0.3.3/ax/storage/json_store/encoders.py`

 * *Files identical despite different names*

### Comparing `ax-platform-0.3.2/ax/storage/json_store/load.py` & `ax-platform-0.3.3/ax/storage/json_store/load.py`

 * *Files identical despite different names*

### Comparing `ax-platform-0.3.2/ax/storage/json_store/registry.py` & `ax-platform-0.3.3/ax/storage/json_store/registry.py`

 * *Files identical despite different names*

### Comparing `ax-platform-0.3.2/ax/storage/json_store/save.py` & `ax-platform-0.3.3/ax/storage/json_store/save.py`

 * *Files identical despite different names*

### Comparing `ax-platform-0.3.2/ax/storage/json_store/tests/test_json_store.py` & `ax-platform-0.3.3/ax/storage/json_store/tests/test_json_store.py`

 * *Files identical despite different names*

### Comparing `ax-platform-0.3.2/ax/storage/metric_registry.py` & `ax-platform-0.3.3/ax/storage/metric_registry.py`

 * *Files identical despite different names*

### Comparing `ax-platform-0.3.2/ax/storage/registry_bundle.py` & `ax-platform-0.3.3/ax/storage/registry_bundle.py`

 * *Files identical despite different names*

### Comparing `ax-platform-0.3.2/ax/storage/runner_registry.py` & `ax-platform-0.3.3/ax/storage/runner_registry.py`

 * *Files identical despite different names*

### Comparing `ax-platform-0.3.2/ax/storage/sqa_store/__init__.py` & `ax-platform-0.3.3/ax/storage/sqa_store/__init__.py`

 * *Files identical despite different names*

### Comparing `ax-platform-0.3.2/ax/storage/sqa_store/db.py` & `ax-platform-0.3.3/ax/storage/sqa_store/db.py`

 * *Files identical despite different names*

### Comparing `ax-platform-0.3.2/ax/storage/sqa_store/decoder.py` & `ax-platform-0.3.3/ax/storage/sqa_store/decoder.py`

 * *Files identical despite different names*

### Comparing `ax-platform-0.3.2/ax/storage/sqa_store/delete.py` & `ax-platform-0.3.3/ax/storage/sqa_store/delete.py`

 * *Files identical despite different names*

### Comparing `ax-platform-0.3.2/ax/storage/sqa_store/encoder.py` & `ax-platform-0.3.3/ax/storage/sqa_store/encoder.py`

 * *Files identical despite different names*

### Comparing `ax-platform-0.3.2/ax/storage/sqa_store/json.py` & `ax-platform-0.3.3/ax/storage/sqa_store/json.py`

 * *Files identical despite different names*

### Comparing `ax-platform-0.3.2/ax/storage/sqa_store/load.py` & `ax-platform-0.3.3/ax/storage/sqa_store/load.py`

 * *Files identical despite different names*

### Comparing `ax-platform-0.3.2/ax/storage/sqa_store/reduced_state.py` & `ax-platform-0.3.3/ax/storage/sqa_store/reduced_state.py`

 * *Files identical despite different names*

### Comparing `ax-platform-0.3.2/ax/storage/sqa_store/save.py` & `ax-platform-0.3.3/ax/storage/sqa_store/save.py`

 * *Files 2% similar despite different names*

```diff
@@ -8,23 +8,27 @@
 
 from logging import Logger
 from typing import Any, Callable, Dict, List, Optional, Sequence, Union
 
 from ax.core.base_trial import BaseTrial
 from ax.core.experiment import Experiment
 from ax.core.generator_run import GeneratorRun
+from ax.core.metric import Metric
+from ax.core.outcome_constraint import ObjectiveThreshold, OutcomeConstraint
 from ax.core.runner import Runner
+from ax.exceptions.core import UserInputError
 from ax.exceptions.storage import SQADecodeError
 from ax.modelbridge.generation_strategy import GenerationStrategy
 from ax.storage.sqa_store.db import session_scope, SQABase
 from ax.storage.sqa_store.decoder import Decoder
 from ax.storage.sqa_store.encoder import Encoder
 from ax.storage.sqa_store.sqa_classes import (
     SQAData,
     SQAGeneratorRun,
+    SQAMetric,
     SQARunner,
     SQATrial,
 )
 from ax.storage.sqa_store.sqa_config import SQAConfig
 from ax.storage.sqa_store.utils import copy_db_ids
 from ax.utils.common.base import Base
 from ax.utils.common.logger import get_logger
@@ -379,14 +383,50 @@
         obj=runner,
         encode_func=encoder.runner_to_sqa,
         decode_func=decoder.runner_from_sqa,
         modify_sqa=add_experiment_id,
     )
 
 
+def update_outcome_constraint_on_experiment(
+    experiment: Experiment,
+    outcome_constraint: OutcomeConstraint,
+    encoder: Encoder,
+    decoder: Decoder,
+) -> None:
+    oc_sqa_class = encoder.config.class_to_sqa_class[Metric]
+
+    exp_id = experiment.db_id
+    if exp_id is None:
+        raise UserInputError("Experiment must be saved before being updated.")
+    oc_id = outcome_constraint.db_id
+    if oc_id is not None:
+        with session_scope() as session:
+            session.query(oc_sqa_class).filter_by(experiment_id=exp_id).filter_by(
+                id=oc_id
+            ).delete()
+
+    # pyre-fixme[53]: Captured variable `exp_id` is not annotated.
+    # pyre-fixme[3]: Return type must be annotated.
+    def add_experiment_id(sqa: SQAMetric):
+        sqa.experiment_id = exp_id
+
+    encode_func = (
+        encoder.objective_threshold_to_sqa
+        if isinstance(outcome_constraint, ObjectiveThreshold)
+        else encoder.outcome_constraint_to_sqa
+    )
+    _merge_into_session(
+        obj=outcome_constraint,
+        encode_func=encode_func,
+        decode_func=decoder.metric_from_sqa,
+        modify_sqa=add_experiment_id,
+    )
+
+
 def update_properties_on_experiment(
     experiment_with_updated_properties: Experiment,
     config: Optional[SQAConfig] = None,
 ) -> None:
     config = config or SQAConfig()
     exp_sqa_class = config.class_to_sqa_class[Experiment]
```

### Comparing `ax-platform-0.3.2/ax/storage/sqa_store/sqa_classes.py` & `ax-platform-0.3.3/ax/storage/sqa_store/sqa_classes.py`

 * *Files identical despite different names*

### Comparing `ax-platform-0.3.2/ax/storage/sqa_store/sqa_config.py` & `ax-platform-0.3.3/ax/storage/sqa_store/sqa_config.py`

 * *Files identical despite different names*

### Comparing `ax-platform-0.3.2/ax/storage/sqa_store/sqa_enum.py` & `ax-platform-0.3.3/ax/storage/sqa_store/sqa_enum.py`

 * *Files identical despite different names*

### Comparing `ax-platform-0.3.2/ax/storage/sqa_store/structs.py` & `ax-platform-0.3.3/ax/storage/sqa_store/structs.py`

 * *Files identical despite different names*

### Comparing `ax-platform-0.3.2/ax/storage/sqa_store/tests/test_sqa_store.py` & `ax-platform-0.3.3/ax/storage/sqa_store/tests/test_sqa_store.py`

 * *Files identical despite different names*

### Comparing `ax-platform-0.3.2/ax/storage/sqa_store/tests/test_utils.py` & `ax-platform-0.3.3/ax/storage/sqa_store/tests/test_utils.py`

 * *Files identical despite different names*

### Comparing `ax-platform-0.3.2/ax/storage/sqa_store/tests/utils.py` & `ax-platform-0.3.3/ax/storage/sqa_store/tests/utils.py`

 * *Files identical despite different names*

### Comparing `ax-platform-0.3.2/ax/storage/sqa_store/timestamp.py` & `ax-platform-0.3.3/ax/storage/sqa_store/timestamp.py`

 * *Files identical despite different names*

### Comparing `ax-platform-0.3.2/ax/storage/sqa_store/utils.py` & `ax-platform-0.3.3/ax/storage/sqa_store/utils.py`

 * *Files identical despite different names*

### Comparing `ax-platform-0.3.2/ax/storage/sqa_store/validation.py` & `ax-platform-0.3.3/ax/storage/sqa_store/validation.py`

 * *Files identical despite different names*

### Comparing `ax-platform-0.3.2/ax/storage/tests/test_registry_bundle.py` & `ax-platform-0.3.3/ax/storage/tests/test_registry_bundle.py`

 * *Files identical despite different names*

### Comparing `ax-platform-0.3.2/ax/storage/transform_registry.py` & `ax-platform-0.3.3/ax/storage/transform_registry.py`

 * *Files identical despite different names*

### Comparing `ax-platform-0.3.2/ax/storage/utils.py` & `ax-platform-0.3.3/ax/storage/utils.py`

 * *Files identical despite different names*

### Comparing `ax-platform-0.3.2/ax/telemetry/experiment.py` & `ax-platform-0.3.3/ax/telemetry/experiment.py`

 * *Files identical despite different names*

### Comparing `ax-platform-0.3.2/ax/telemetry/generation_strategy.py` & `ax-platform-0.3.3/ax/telemetry/generation_strategy.py`

 * *Files identical despite different names*

### Comparing `ax-platform-0.3.2/ax/telemetry/scheduler.py` & `ax-platform-0.3.3/ax/telemetry/scheduler.py`

 * *Files 26% similar despite different names*

```diff
@@ -2,26 +2,19 @@
 #
 # This source code is licensed under the MIT license found in the
 # LICENSE file in the root directory of this source tree.
 
 from __future__ import annotations
 
 from dataclasses import asdict, dataclass
-from typing import Any, Dict, List, Optional, Tuple, Type
+from typing import Any, Dict, Optional
+from warnings import warn
 
-from ax.modelbridge.generation_strategy import GenerationStep, GenerationStrategy
-
-from ax.modelbridge.modelbridge_utils import (
-    extract_search_space_digest,
-    transform_search_space,
-)
-from ax.modelbridge.registry import ModelRegistryBase, SearchSpace
-from ax.modelbridge.transforms.base import Transform
-
-from ax.service.scheduler import Scheduler
+from ax.service.scheduler import get_fitted_model_bridge, Scheduler
+from ax.telemetry.common import _get_max_transformed_dimensionality
 
 from ax.telemetry.experiment import ExperimentCompletedRecord, ExperimentCreatedRecord
 from ax.telemetry.generation_strategy import GenerationStrategyCreatedRecord
 
 
 @dataclass(frozen=True)
 class SchedulerCreatedRecord:
@@ -108,20 +101,39 @@
     model_fit_quality: float
 
     num_metric_fetch_e_encountered: int
     num_trials_bad_due_to_err: int
 
     @classmethod
     def from_scheduler(cls, scheduler: Scheduler) -> SchedulerCompletedRecord:
+        try:
+            model_bridge = get_fitted_model_bridge(scheduler)
+            model_fit_dict = model_bridge.compute_model_fit_metrics(
+                experiment=scheduler.experiment
+            )
+            # We'd ideally log the entire `model_fit_dict` as a single model fit metric
+            # can't capture the nuances of multiple experimental metrics, but this might
+            # lead to database performance issues. So instead, we take the worst
+            # coefficient of determination as model fit quality and store the full data
+            # in Manifold (TODO).
+            model_fit_quality = min(
+                model_fit_dict["coefficient_of_determination"].values()
+            )
+
+        except Exception as e:
+            warn("Encountered exception in computing model fit quality: " + str(e))
+            model_fit_quality = float("-inf")
+            # model_std_quality = float("-inf")
+
         return cls(
             experiment_completed_record=ExperimentCompletedRecord.from_experiment(
                 experiment=scheduler.experiment
             ),
-            best_point_quality=-1,  # TODO[T147907632]
-            model_fit_quality=-1,  # TODO[T147907632]
+            best_point_quality=float("-inf"),  # TODO[T147907632]
+            model_fit_quality=model_fit_quality,
             num_metric_fetch_e_encountered=scheduler._num_metric_fetch_e_encountered,
             num_trials_bad_due_to_err=scheduler._num_trials_bad_due_to_err,
         )
 
     def flatten(self) -> Dict[str, Any]:
         """
         Flatten into an appropriate format for logging to a tabular database.
@@ -130,68 +142,7 @@
         self_dict = asdict(self)
         experiment_completed_record_dict = self_dict.pop("experiment_completed_record")
 
         return {
             **self_dict,
             **experiment_completed_record_dict,
         }
-
-
-def _get_max_transformed_dimensionality(
-    search_space: SearchSpace, generation_strategy: GenerationStrategy
-) -> int:
-    """
-    Get dimensionality of transformed SearchSpace for all steps in the
-    GenerationStrategy and return the maximum.
-    """
-
-    transforms_by_step = [
-        _extract_transforms_and_configs(step=step)
-        for step in generation_strategy._steps
-    ]
-
-    transformed_search_spaces = [
-        transform_search_space(
-            search_space=search_space,
-            transforms=transforms,
-            transform_configs=transform_configs,
-        )
-        for transforms, transform_configs in transforms_by_step
-    ]
-
-    # The length of the bounds of a SearchSpaceDigest is equal to the number of
-    # dimensions present.
-    dimensionalities = [
-        len(
-            extract_search_space_digest(
-                search_space=tf_search_space,
-                param_names=list(tf_search_space.parameters.keys()),
-            ).bounds
-        )
-        for tf_search_space in transformed_search_spaces
-    ]
-
-    return max(dimensionalities)
-
-
-def _extract_transforms_and_configs(
-    step: GenerationStep,
-) -> Tuple[List[Type[Transform]], Dict[str, Any]]:
-    """
-    Extract Transforms and their configs from the GenerationStep. Prefer kwargs
-    provided over the model's defaults.
-    """
-
-    kwargs = step.model_spec.model_kwargs or {}
-    transforms = kwargs.get("transforms")
-    transform_configs = kwargs.get("transform_configs")
-
-    if transforms is not None and transform_configs is not None:
-        return transforms, transform_configs
-
-    model = step.model
-    if isinstance(model, ModelRegistryBase):
-        _, bridge_kwargs = model.view_defaults()
-        transforms = transforms or bridge_kwargs.get("transforms")
-        transform_configs = transform_configs or bridge_kwargs.get("transform_configs")
-
-    return (transforms or [], transform_configs or {})
```

### Comparing `ax-platform-0.3.2/ax/telemetry/tests/test_experiment.py` & `ax-platform-0.3.3/ax/telemetry/tests/test_experiment.py`

 * *Files identical despite different names*

### Comparing `ax-platform-0.3.2/ax/telemetry/tests/test_generation_strategy.py` & `ax-platform-0.3.3/ax/telemetry/tests/test_generation_strategy.py`

 * *Files identical despite different names*

### Comparing `ax-platform-0.3.2/ax/utils/common/base.py` & `ax-platform-0.3.3/ax/utils/common/base.py`

 * *Files identical despite different names*

### Comparing `ax-platform-0.3.2/ax/utils/common/constants.py` & `ax-platform-0.3.3/ax/utils/common/constants.py`

 * *Files identical despite different names*

### Comparing `ax-platform-0.3.2/ax/utils/common/decorator.py` & `ax-platform-0.3.3/ax/utils/common/decorator.py`

 * *Files identical despite different names*

### Comparing `ax-platform-0.3.2/ax/utils/common/docutils.py` & `ax-platform-0.3.3/ax/utils/common/docutils.py`

 * *Files identical despite different names*

### Comparing `ax-platform-0.3.2/ax/utils/common/equality.py` & `ax-platform-0.3.3/ax/utils/common/equality.py`

 * *Files identical despite different names*

### Comparing `ax-platform-0.3.2/ax/utils/common/executils.py` & `ax-platform-0.3.3/ax/utils/common/executils.py`

 * *Files identical despite different names*

### Comparing `ax-platform-0.3.2/ax/utils/common/kwargs.py` & `ax-platform-0.3.3/ax/utils/common/kwargs.py`

 * *Files identical despite different names*

### Comparing `ax-platform-0.3.2/ax/utils/common/logger.py` & `ax-platform-0.3.3/ax/utils/common/logger.py`

 * *Files 3% similar despite different names*

```diff
@@ -158,15 +158,15 @@
         """
         self.name = name
         self.level = level
 
     def decorate_callable(self, func: Callable[..., T]) -> Callable[..., T]:
         @wraps(func)
         def inner(*args: Any, **kwargs: Any) -> T:
-            logger = get_logger(self.name)
+            logger = logging.getLogger(self.name)
             prev_level = logger.getEffectiveLevel()
             logger.setLevel(self.level)
             t = self._call_func(func, *args, **kwargs)
             logger.setLevel(prev_level)
             return t
 
         return inner
@@ -181,20 +181,20 @@
         self.level = level
 
     def decorate_callable(self, func: Callable[..., T]) -> Callable[..., T]:
         @wraps(func)
         def inner(*args: Any, **kwargs: Any) -> T:
             prev_levels = {}
             for name in self.names:
-                logger = get_logger(name)
+                logger = logging.getLogger(name)
                 prev_levels[name] = logger.getEffectiveLevel()
                 logger.setLevel(self.level)
             t = self._call_func(func, *args, **kwargs)
             for name in self.names:
-                get_logger(name).setLevel(prev_levels[name])
+                logging.getLogger(name).setLevel(prev_levels[name])
             return t
 
         return inner
 
 
 """Sets up Ax's root logger to not propogate to Python's root logger and
 use the default stream handler.
```

### Comparing `ax-platform-0.3.2/ax/utils/common/mock.py` & `ax-platform-0.3.3/ax/utils/common/mock.py`

 * *Files identical despite different names*

### Comparing `ax-platform-0.3.2/ax/utils/common/result.py` & `ax-platform-0.3.3/ax/utils/common/result.py`

 * *Files identical despite different names*

### Comparing `ax-platform-0.3.2/ax/utils/common/serialization.py` & `ax-platform-0.3.3/ax/utils/common/serialization.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,15 @@
 #!/usr/bin/env python3
 # Copyright (c) Meta Platforms, Inc. and affiliates.
 #
 # This source code is licensed under the MIT license found in the
 # LICENSE file in the root directory of this source tree.
 
+from __future__ import annotations
+
 import inspect
 import pydoc
 from abc import ABC
 from types import FunctionType
 from typing import Any, Callable, Dict, List, Optional, Type
 
 
@@ -118,16 +120,15 @@
                 continue  # pragma: no cover
         init_args[arg] = value
     return init_args
 
 
 class SerializationMixin(ABC):
     @classmethod
-    # pyre-fixme[2]: Parameter annotation cannot be `Any`.
-    def serialize_init_args(cls, obj: Any) -> Dict[str, Any]:
+    def serialize_init_args(cls, obj: SerializationMixin) -> Dict[str, Any]:
         """Serialize the properties needed to initialize the object.
         Used for storage.
         """
         return serialize_init_args(object=obj)
 
     @classmethod
     def deserialize_init_args(cls, args: Dict[str, Any]) -> Dict[str, Any]:
```

### Comparing `ax-platform-0.3.2/ax/utils/common/tests/test_docutils.py` & `ax-platform-0.3.3/ax/utils/common/tests/test_docutils.py`

 * *Files identical despite different names*

### Comparing `ax-platform-0.3.2/ax/utils/common/tests/test_equality.py` & `ax-platform-0.3.3/ax/utils/common/tests/test_equality.py`

 * *Files identical despite different names*

### Comparing `ax-platform-0.3.2/ax/utils/common/tests/test_executils.py` & `ax-platform-0.3.3/ax/utils/common/tests/test_executils.py`

 * *Files identical despite different names*

### Comparing `ax-platform-0.3.2/ax/utils/common/tests/test_kwargutils.py` & `ax-platform-0.3.3/ax/utils/common/tests/test_kwargutils.py`

 * *Files identical despite different names*

### Comparing `ax-platform-0.3.2/ax/utils/common/tests/test_logger.py` & `ax-platform-0.3.3/ax/utils/common/tests/test_logger.py`

 * *Files identical despite different names*

### Comparing `ax-platform-0.3.2/ax/utils/common/tests/test_result.py` & `ax-platform-0.3.3/ax/utils/common/tests/test_result.py`

 * *Files identical despite different names*

### Comparing `ax-platform-0.3.2/ax/utils/common/tests/test_serialization.py` & `ax-platform-0.3.3/ax/utils/common/tests/test_serialization.py`

 * *Files identical despite different names*

### Comparing `ax-platform-0.3.2/ax/utils/common/tests/test_testutils.py` & `ax-platform-0.3.3/ax/utils/common/tests/test_testutils.py`

 * *Files identical despite different names*

### Comparing `ax-platform-0.3.2/ax/utils/common/tests/test_typeutils.py` & `ax-platform-0.3.3/ax/utils/common/tests/test_typeutils.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,20 +1,18 @@
 #!/usr/bin/env python3
 # Copyright (c) Meta Platforms, Inc. and affiliates.
 #
 # This source code is licensed under the MIT license found in the
 # LICENSE file in the root directory of this source tree.
 
-from typing import Dict
 
 import numpy as np
 from ax.utils.common.testutils import TestCase
 from ax.utils.common.typeutils import (
     checked_cast,
-    checked_cast_complex,
     checked_cast_dict,
     checked_cast_list,
     checked_cast_optional,
     not_none,
     numpy_type_to_python_type,
 )
 
@@ -33,20 +31,14 @@
     def test_checked_cast_with_error_override(self) -> None:
         self.assertEqual(checked_cast(float, 2.0), 2.0)
         with self.assertRaises(NotImplementedError):
             checked_cast(
                 float, 2, exception=NotImplementedError("foo() doesn't support ints")
             )
 
-    def test_checked_cast_complex(self) -> None:
-        t = Dict[int, str]
-        self.assertEqual(checked_cast_complex(t, {1: "one"}), {1: "one"})
-        with self.assertRaises(ValueError):
-            checked_cast_complex(t, {"one": 1})
-
     def test_checked_cast_list(self) -> None:
         self.assertEqual(checked_cast_list(float, [1.0, 2.0]), [1.0, 2.0])
         with self.assertRaises(ValueError):
             checked_cast_list(float, [1.0, 2])
 
     def test_checked_cast_optional(self) -> None:
         self.assertEqual(checked_cast_optional(float, None), None)
```

### Comparing `ax-platform-0.3.2/ax/utils/common/testutils.py` & `ax-platform-0.3.3/ax/utils/common/testutils.py`

 * *Files 4% similar despite different names*

```diff
@@ -5,17 +5,19 @@
 # LICENSE file in the root directory of this source tree.
 
 # pyre-strict
 
 """Support functions for tests
 """
 
+import builtins
 import contextlib
 import io
 import linecache
+import logging
 import signal
 import sys
 import types
 import unittest
 from functools import wraps
 from logging import Logger
 from types import FrameType
@@ -253,21 +255,37 @@
                 level=level + 1,
                 values_in_suffix=f" in {bul}",
                 skip_db_id_check=skip_db_id_check,
             )
     return msg
 
 
-def setup_import_mocks(mocked_import_paths: List[str]) -> None:
+def setup_import_mocks(
+    mocked_import_paths: List[str], mock_config_dict: Optional[Dict[str, Any]] = None
+) -> None:
+    # pyre-fixme[3]
+    def custom_import(name: str, *args: Any, **kwargs: Any) -> Any:
+        for import_path in mocked_import_paths:
+            if name == import_path or name.startswith(f"{import_path}."):
+                mymock = MagicMock()
+                if mock_config_dict is not None:
+                    mymock.configure_mock(**mock_config_dict)
+                return mymock
+        return original_import(name, *args, **kwargs)
+
     for import_path in mocked_import_paths:
         if import_path in sys.modules and not isinstance(
             sys.modules[import_path], MagicMock
         ):
             raise Exception(f"{import_path} has already been imported!")
-        sys.modules[import_path] = MagicMock()
+
+    # Replace the original import with the custom one
+    # pyre-fixme[61]
+    original_import = builtins.__import__
+    builtins.__import__ = custom_import
 
 
 class TestCase(fake_filesystem_unittest.TestCase):
     """The base Ax test case, contains various helper functions to write unittests."""
 
     MAX_TEST_SECONDS = 480
     MIN_TTOT = 1.0
@@ -295,14 +313,26 @@
                 ).sort(sort_type="ttot", sort_order="asc").print_all(
                     columns=self.PROFILER_COLUMNS
                 )
 
         super().__init__(methodName=methodName)
         signal.signal(signal.SIGALRM, signal_handler)
 
+    def setUp(self) -> None:
+        """
+        Only show log messages of WARNING or higher while testing.
+
+        Ax prints a lot of INFO logs that are not relevant for unit tests.
+        """
+        logger = get_logger(__name__, level=logging.WARNING)
+        # Parent handlers are shared, so setting the level this
+        # way applies it to all Ax loggers.
+        if logger.parent is not None and hasattr(logger.parent, "handlers"):
+            logger.parent.handlers[0].setLevel(logging.WARNING)
+
     def run(
         self, result: Optional[unittest.result.TestResult] = ...
     ) -> Optional[unittest.result.TestResult]:
         # Arrange for a SIGALRM signal to be delivered to the calling process
         # in specified number of seconds.
         signal.alarm(self.MAX_TEST_SECONDS)
         try:
```

### Comparing `ax-platform-0.3.2/ax/utils/common/timeutils.py` & `ax-platform-0.3.3/ax/utils/common/timeutils.py`

 * *Files identical despite different names*

### Comparing `ax-platform-0.3.2/ax/utils/common/typeutils.py` & `ax-platform-0.3.3/ax/utils/common/typeutils.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,17 +1,16 @@
 #!/usr/bin/env python3
 # Copyright (c) Meta Platforms, Inc. and affiliates.
 #
 # This source code is licensed under the MIT license found in the
 # LICENSE file in the root directory of this source tree.
 
-from typing import Any, cast, Dict, List, Optional, Tuple, Type, TypeVar
+from typing import Any, Dict, List, Optional, Tuple, Type, TypeVar
 
 import numpy as np
-from typeguard import check_type
 
 
 T = TypeVar("T")
 V = TypeVar("V")
 K = TypeVar("K")
 X = TypeVar("X")
 Y = TypeVar("Y")
@@ -57,42 +56,14 @@
     if not isinstance(val, typ):
         raise exception if exception is not None else ValueError(
             f"Value was not of type {typ}:\n{val}"
         )
     return val
 
 
-def checked_cast_complex(typ: Type[T], val: V, message: Optional[str] = None) -> T:
-    """
-    Cast a value to a type (with a runtime safety check).  Used for subscripted generics
-    which isinstance cannot run against.
-
-    Returns the value unchanged and checks its type at runtime. This signals to the
-    typechecker that the value has the designated type.
-
-    Like `typing.cast`_ ``check_cast`` performs no runtime conversion on its argument,
-    but, unlike ``typing.cast``, ``checked_cast`` will throw an error if the value is
-    not of the expected type.
-
-    Args:
-        typ: the type to cast to
-        val: the value that we are casting
-        message: message to print on error
-    Returns:
-        the ``val`` argument casted to typ
-
-    .. _typing.cast: https://docs.python.org/3/library/typing.html#typing.cast
-    """
-    try:
-        check_type("val", val, typ)
-        return cast(T, val)
-    except TypeError:
-        raise ValueError(message or f"Value was not of type {typ}: {val}")
-
-
 def checked_cast_optional(typ: Type[T], val: Optional[V]) -> Optional[T]:
     """Calls checked_cast only if value is not None."""
     if val is None:
         return val
     return checked_cast(typ, val)
```

### Comparing `ax-platform-0.3.2/ax/utils/common/typeutils_torch.py` & `ax-platform-0.3.3/ax/utils/common/typeutils_torch.py`

 * *Files identical despite different names*

### Comparing `ax-platform-0.3.2/ax/utils/flake8_plugins/docstring_checker.py` & `ax-platform-0.3.3/ax/utils/flake8_plugins/docstring_checker.py`

 * *Files identical despite different names*

### Comparing `ax-platform-0.3.2/ax/utils/measurement/synthetic_functions.py` & `ax-platform-0.3.3/ax/utils/measurement/synthetic_functions.py`

 * *Files identical despite different names*

### Comparing `ax-platform-0.3.2/ax/utils/measurement/tests/test_synthetic_functions.py` & `ax-platform-0.3.3/ax/utils/measurement/tests/test_synthetic_functions.py`

 * *Files identical despite different names*

### Comparing `ax-platform-0.3.2/ax/utils/notebook/plotting.py` & `ax-platform-0.3.3/ax/utils/notebook/plotting.py`

 * *Files identical despite different names*

### Comparing `ax-platform-0.3.2/ax/utils/report/render.py` & `ax-platform-0.3.3/ax/utils/report/render.py`

 * *Files identical despite different names*

### Comparing `ax-platform-0.3.2/ax/utils/report/resources/base_template.html` & `ax-platform-0.3.3/ax/utils/report/resources/base_template.html`

 * *Files identical despite different names*

### Comparing `ax-platform-0.3.2/ax/utils/report/resources/report.css` & `ax-platform-0.3.3/ax/utils/report/resources/report.css`

 * *Files identical despite different names*

### Comparing `ax-platform-0.3.2/ax/utils/report/resources/sufficient_statistic.html` & `ax-platform-0.3.3/ax/utils/report/resources/sufficient_statistic.html`

 * *Files identical despite different names*

### Comparing `ax-platform-0.3.2/ax/utils/report/tests/test_render.py` & `ax-platform-0.3.3/ax/utils/report/tests/test_render.py`

 * *Files identical despite different names*

### Comparing `ax-platform-0.3.2/ax/utils/sensitivity/derivative_gp.py` & `ax-platform-0.3.3/ax/utils/sensitivity/derivative_gp.py`

 * *Files identical despite different names*

### Comparing `ax-platform-0.3.2/ax/utils/sensitivity/derivative_measures.py` & `ax-platform-0.3.3/ax/utils/sensitivity/derivative_measures.py`

 * *Files identical despite different names*

### Comparing `ax-platform-0.3.2/ax/utils/sensitivity/sobol_measures.py` & `ax-platform-0.3.3/ax/utils/sensitivity/sobol_measures.py`

 * *Files identical despite different names*

### Comparing `ax-platform-0.3.2/ax/utils/sensitivity/tests/test_sensitivity.py` & `ax-platform-0.3.3/ax/utils/sensitivity/tests/test_sensitivity.py`

 * *Files identical despite different names*

### Comparing `ax-platform-0.3.2/ax/utils/stats/statstools.py` & `ax-platform-0.3.3/ax/utils/stats/statstools.py`

 * *Files 4% similar despite different names*

```diff
@@ -298,22 +298,27 @@
 
 
 def relativize_data(
     data: Data,
     status_quo_name: str = "status_quo",
     as_percent: bool = False,
     include_sq: bool = False,
+    bias_correction: bool = True,
 ) -> Data:
     """Relativize a data object w.r.t. a status_quo arm.
 
     Args:
         data: The data object to be relativized.
         status_quo_name: The name of the status_quo arm.
         as_percent: If True, return results as percentage change.
         include_sq: Include status quo in final df.
+        bias_correction: Whether to apply bias correction when computing relativized
+            metric values. Uses a second-order Taylor expansion for approximating
+            the means and standard errors or the ratios, see
+            ax.utils.stats.statstools.relativize for more details.
 
     Returns:
         The new data object with the relativized metrics (excluding the
             status_quo arm)
 
     """
     df = data.df.copy()
@@ -333,14 +338,15 @@
             subgroup_df = subgroup_df[~is_sq]
         means_rel, sems_rel = relativize(
             means_t=subgroup_df["mean"].values,
             sems_t=subgroup_df["sem"].values,
             mean_c=sq_mean,
             sem_c=sq_sem,
             as_percent=as_percent,
+            bias_correction=bias_correction,
         )
         dfs.append(
             pd.concat(
                 [
                     subgroup_df.drop(["mean", "sem"], axis=1),
                     pd.DataFrame(
                         np.array([means_rel, sems_rel]).T,
```

### Comparing `ax-platform-0.3.2/ax/utils/stats/tests/test_statstools.py` & `ax-platform-0.3.3/ax/utils/stats/tests/test_statstools.py`

 * *Files identical despite different names*

### Comparing `ax-platform-0.3.2/ax/utils/testing/backend_scheduler.py` & `ax-platform-0.3.3/ax/utils/testing/backend_scheduler.py`

 * *Files identical despite different names*

### Comparing `ax-platform-0.3.2/ax/utils/testing/backend_simulator.py` & `ax-platform-0.3.3/ax/utils/testing/backend_simulator.py`

 * *Files identical despite different names*

### Comparing `ax-platform-0.3.2/ax/utils/testing/benchmark_stubs.py` & `ax-platform-0.3.3/ax/utils/testing/benchmark_stubs.py`

 * *Files identical despite different names*

### Comparing `ax-platform-0.3.2/ax/utils/testing/core_stubs.py` & `ax-platform-0.3.3/ax/utils/testing/core_stubs.py`

 * *Files 0% similar despite different names*

```diff
@@ -1899,15 +1899,15 @@
     a pre-specified number of trials are completed.
     """
 
     def __init__(self, min_trials: int, trial_to_stop: int) -> None:
         super().__init__(min_trials=min_trials)
         self.trial_to_stop = trial_to_stop
 
-    def should_stop_optimization(
+    def _should_stop_optimization(
         self, experiment: Experiment, **kwargs: Dict[str, Any]
     ) -> Tuple[bool, str]:
         num_completed_trials = len(experiment.trials_by_status[TrialStatus.COMPLETED])
 
         if num_completed_trials >= max([self.min_trials, self.trial_to_stop]):
             return True, "Stop the optimization."
         else:
```

### Comparing `ax-platform-0.3.2/ax/utils/testing/metrics/backend_simulator_map.py` & `ax-platform-0.3.3/ax/utils/testing/metrics/backend_simulator_map.py`

 * *Files identical despite different names*

### Comparing `ax-platform-0.3.2/ax/utils/testing/metrics/branin_backend_map.py` & `ax-platform-0.3.3/ax/utils/testing/metrics/branin_backend_map.py`

 * *Files identical despite different names*

### Comparing `ax-platform-0.3.2/ax/utils/testing/mock.py` & `ax-platform-0.3.3/ax/utils/testing/mock.py`

 * *Files identical despite different names*

### Comparing `ax-platform-0.3.2/ax/utils/testing/modeling_stubs.py` & `ax-platform-0.3.3/ax/utils/testing/modeling_stubs.py`

 * *Files identical despite different names*

### Comparing `ax-platform-0.3.2/ax/utils/testing/test_init_files.py` & `ax-platform-0.3.3/ax/utils/testing/test_init_files.py`

 * *Files identical despite different names*

### Comparing `ax-platform-0.3.2/ax/utils/testing/tests/test_backend_simulator.py` & `ax-platform-0.3.3/ax/utils/testing/tests/test_backend_simulator.py`

 * *Files identical despite different names*

### Comparing `ax-platform-0.3.2/ax/utils/testing/tests/test_utils.py` & `ax-platform-0.3.3/ax/utils/testing/tests/test_utils.py`

 * *Files identical despite different names*

### Comparing `ax-platform-0.3.2/ax/utils/testing/torch_stubs.py` & `ax-platform-0.3.3/ax/utils/testing/torch_stubs.py`

 * *Files identical despite different names*

### Comparing `ax-platform-0.3.2/ax/utils/testing/utils.py` & `ax-platform-0.3.3/ax/utils/testing/utils.py`

 * *Files identical despite different names*

### Comparing `ax-platform-0.3.2/ax/utils/tutorials/cnn_utils.py` & `ax-platform-0.3.3/ax/utils/tutorials/cnn_utils.py`

 * *Files identical despite different names*

### Comparing `ax-platform-0.3.2/ax_platform.egg-info/PKG-INFO` & `ax-platform-0.3.3/ax_platform.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ax-platform
-Version: 0.3.2
+Version: 0.3.3
 Summary: Adaptive Experimentation
 Home-page: https://github.com/facebook/Ax
 Author: Facebook, Inc.
 License: MIT
 Description: <img width="300" src="https://ax.dev/img/ax_logo_lockup.svg" alt="Ax Logo" />
         
         <hr/>
@@ -171,15 +171,15 @@
         pip install git+https://github.com/cornellius-gp/linear_operator.git
         pip install git+https://github.com/cornellius-gp/gpytorch.git
         export ALLOW_LATEST_GPYTORCH_LINOP=true
         pip install git+https://github.com/pytorch/botorch.git
         export ALLOW_BOTORCH_LATEST=true
         git clone https://github.com/facebook/ax.git --depth 1
         cd ax
-        pip install -e .[unittest]
+        pip install -e .[tutorial]
         ```
         
         See recommendation for installing PyTorch for MacOS users above.
         
         The above example limits the cloned directory size via the
         [`--depth`](https://git-scm.com/docs/git-clone#Documentation/git-clone.txt---depthltdepthgt)
         argument to `git clone`. If you require the entire commit history you may remove this
```

### Comparing `ax-platform-0.3.2/ax_platform.egg-info/SOURCES.txt` & `ax-platform-0.3.3/ax_platform.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -42,14 +42,15 @@
 ax/benchmark/tests/test_benchmark.py
 ax/benchmark/tests/test_benchmark_method.py
 ax/benchmark/tests/test_benchmark_problem.py
 ax/benchmark/tests/test_methods.py
 ax/benchmark/tests/test_mixed_integer_problems.py
 ax/benchmark/tests/test_problem_storage.py
 ax/benchmark/tests/test_problems.py
+ax/benchmark/tests/test_surrogate_runner.py
 ax/core/__init__.py
 ax/core/arm.py
 ax/core/base_trial.py
 ax/core/batch_trial.py
 ax/core/data.py
 ax/core/experiment.py
 ax/core/formatting_utils.py
@@ -185,14 +186,15 @@
 ax/modelbridge/tests/test_log_transform.py
 ax/modelbridge/tests/test_log_y_transform.py
 ax/modelbridge/tests/test_logit_transform.py
 ax/modelbridge/tests/test_map_torch_modelbridge.py
 ax/modelbridge/tests/test_map_unit_x_transform.py
 ax/modelbridge/tests/test_merge_repeated_measurements_transform.py
 ax/modelbridge/tests/test_metrics_as_task_transform.py
+ax/modelbridge/tests/test_model_fit_metrics.py
 ax/modelbridge/tests/test_model_spec.py
 ax/modelbridge/tests/test_modelbridge_utils.py
 ax/modelbridge/tests/test_one_hot_transform.py
 ax/modelbridge/tests/test_pairwise_modelbridge.py
 ax/modelbridge/tests/test_percentile_y_transform.py
 ax/modelbridge/tests/test_power_transform_y.py
 ax/modelbridge/tests/test_prediction_utils.py
@@ -311,31 +313,35 @@
 ax/models/torch/fully_bayesian_model_utils.py
 ax/models/torch/posterior_mean.py
 ax/models/torch/randomforest.py
 ax/models/torch/rembo.py
 ax/models/torch/utils.py
 ax/models/torch/botorch_modular/__init__.py
 ax/models/torch/botorch_modular/acquisition.py
+ax/models/torch/botorch_modular/kernels.py
 ax/models/torch/botorch_modular/list_surrogate.py
 ax/models/torch/botorch_modular/model.py
 ax/models/torch/botorch_modular/multi_fidelity.py
 ax/models/torch/botorch_modular/optimizer_argparse.py
 ax/models/torch/botorch_modular/surrogate.py
 ax/models/torch/botorch_modular/utils.py
+ax/models/torch/botorch_modular/input_constructors/__init__.py
+ax/models/torch/botorch_modular/input_constructors/covar_modules.py
 ax/models/torch/tests/__init__.py
 ax/models/torch/tests/test_acquisition.py
+ax/models/torch/tests/test_covar_modules_argparse.py
+ax/models/torch/tests/test_kernels.py
 ax/models/torch/tests/test_model.py
 ax/models/torch/tests/test_multi_fidelity.py
 ax/models/torch/tests/test_optimizer_argparse.py
 ax/models/torch/tests/test_surrogate.py
 ax/models/torch/tests/test_utils.py
 ax/plot/__init__.py
 ax/plot/bandit_rollout.py
 ax/plot/base.py
-ax/plot/benchmark.py
 ax/plot/color.py
 ax/plot/contour.py
 ax/plot/diagnostic.py
 ax/plot/feature_importances.py
 ax/plot/helper.py
 ax/plot/marginal_effects.py
 ax/plot/parallel_coordinates.py
@@ -434,19 +440,21 @@
 ax/storage/sqa_store/utils.py
 ax/storage/sqa_store/validation.py
 ax/storage/sqa_store/tests/__init__.py
 ax/storage/sqa_store/tests/test_sqa_store.py
 ax/storage/sqa_store/tests/test_utils.py
 ax/storage/sqa_store/tests/utils.py
 ax/storage/tests/test_registry_bundle.py
+ax/telemetry/ax_client.py
 ax/telemetry/common.py
 ax/telemetry/experiment.py
 ax/telemetry/generation_strategy.py
 ax/telemetry/optimization.py
 ax/telemetry/scheduler.py
+ax/telemetry/tests/test_ax_client.py
 ax/telemetry/tests/test_experiment.py
 ax/telemetry/tests/test_generation_strategy.py
 ax/telemetry/tests/test_optimization.py
 ax/telemetry/tests/test_scheduler.py
 ax/utils/__init__.py
 ax/utils/common/__init__.py
 ax/utils/common/base.py
@@ -494,14 +502,15 @@
 ax/utils/sensitivity/__init__.py
 ax/utils/sensitivity/derivative_gp.py
 ax/utils/sensitivity/derivative_measures.py
 ax/utils/sensitivity/sobol_measures.py
 ax/utils/sensitivity/tests/__init__.py
 ax/utils/sensitivity/tests/test_sensitivity.py
 ax/utils/stats/__init__.py
+ax/utils/stats/model_fit_stats.py
 ax/utils/stats/statstools.py
 ax/utils/stats/tests/__init__.py
 ax/utils/stats/tests/test_statstools.py
 ax/utils/testing/__init__.py
 ax/utils/testing/backend_scheduler.py
 ax/utils/testing/backend_simulator.py
 ax/utils/testing/benchmark_stubs.py
@@ -583,14 +592,15 @@
 sphinx/source/utils.rst
 tutorials/Setup_and_Usage_of_BoTorch_Models_in_Ax.ipynb
 tutorials/factorial.ipynb
 tutorials/generation_strategy.ipynb
 tutorials/gpei_hartmann_developer.ipynb
 tutorials/gpei_hartmann_loop.ipynb
 tutorials/gpei_hartmann_service.ipynb
+tutorials/gss.ipynb
 tutorials/modular_botax.ipynb
 tutorials/multi_task.ipynb
 tutorials/multiobjective_optimization.ipynb
 tutorials/raytune_pytorch_cnn.ipynb
 tutorials/saasbo.ipynb
 tutorials/saasbo_nehvi.ipynb
 tutorials/scheduler.ipynb
```

### Comparing `ax-platform-0.3.2/ax_platform.egg-info/requires.txt` & `ax-platform-0.3.3/ax_platform.egg-info/requires.txt`

 * *Files identical despite different names*

### Comparing `ax-platform-0.3.2/docs/api.md` & `ax-platform-0.3.3/docs/api.md`

 * *Files identical despite different names*

### Comparing `ax-platform-0.3.2/docs/assets/bandit_allocation.png` & `ax-platform-0.3.3/docs/assets/bandit_allocation.png`

 * *Files identical despite different names*

### Comparing `ax-platform-0.3.2/docs/assets/bo_1d_opt.gif` & `ax-platform-0.3.3/docs/assets/bo_1d_opt.gif`

 * *Files identical despite different names*

### Comparing `ax-platform-0.3.2/docs/assets/contour.js` & `ax-platform-0.3.3/docs/assets/contour.js`

 * *Files identical despite different names*

### Comparing `ax-platform-0.3.2/docs/assets/cv.js` & `ax-platform-0.3.3/docs/assets/cv.js`

 * *Files identical despite different names*

### Comparing `ax-platform-0.3.2/docs/assets/example_shrinkage.png` & `ax-platform-0.3.3/docs/assets/example_shrinkage.png`

 * *Files identical despite different names*

### Comparing `ax-platform-0.3.2/docs/assets/fitted.js` & `ax-platform-0.3.3/docs/assets/fitted.js`

 * *Files identical despite different names*

### Comparing `ax-platform-0.3.2/docs/assets/gp_opt.png` & `ax-platform-0.3.3/docs/assets/gp_opt.png`

 * *Files identical despite different names*

### Comparing `ax-platform-0.3.2/docs/assets/gp_posterior.png` & `ax-platform-0.3.3/docs/assets/gp_posterior.png`

 * *Files identical despite different names*

### Comparing `ax-platform-0.3.2/docs/assets/mab_animate.gif` & `ax-platform-0.3.3/docs/assets/mab_animate.gif`

 * *Files identical despite different names*

### Comparing `ax-platform-0.3.2/docs/assets/mab_probs.png` & `ax-platform-0.3.3/docs/assets/mab_probs.png`

 * *Files identical despite different names*

### Comparing `ax-platform-0.3.2/docs/assets/mab_regret.png` & `ax-platform-0.3.3/docs/assets/mab_regret.png`

 * *Files identical despite different names*

### Comparing `ax-platform-0.3.2/docs/assets/slice.js` & `ax-platform-0.3.3/docs/assets/slice.js`

 * *Files identical despite different names*

### Comparing `ax-platform-0.3.2/docs/banditopt.md` & `ax-platform-0.3.3/docs/banditopt.md`

 * *Files identical despite different names*

### Comparing `ax-platform-0.3.2/docs/bayesopt.md` & `ax-platform-0.3.3/docs/bayesopt.md`

 * *Files identical despite different names*

### Comparing `ax-platform-0.3.2/docs/core.md` & `ax-platform-0.3.3/docs/core.md`

 * *Files identical despite different names*

### Comparing `ax-platform-0.3.2/docs/data.md` & `ax-platform-0.3.3/docs/data.md`

 * *Files identical despite different names*

### Comparing `ax-platform-0.3.2/docs/glossary.md` & `ax-platform-0.3.3/docs/glossary.md`

 * *Files identical despite different names*

### Comparing `ax-platform-0.3.2/docs/installation.md` & `ax-platform-0.3.3/docs/installation.md`

 * *Files identical despite different names*

### Comparing `ax-platform-0.3.2/docs/models.md` & `ax-platform-0.3.3/docs/models.md`

 * *Files identical despite different names*

### Comparing `ax-platform-0.3.2/docs/storage.md` & `ax-platform-0.3.3/docs/storage.md`

 * *Files 26% similar despite different names*

```diff
@@ -8,52 +8,72 @@
 ## JSON
 
 ### Saving
 
 To save an experiment to JSON, specify the filepath:
 
 ```py
-from ax import Experiment, save
+from ax import Experiment
+from ax.storage.json_store.save import save_experiment
 
 experiment = Experiment(...)
 filepath = "experiments/experiment.json"
-save(experiment, filepath)
+save_experiment(experiment, filepath)
 ```
 
 The experiment (including attached data) will be serialized and saved to the specified file.
 
 ### Updating
 
 To update a JSON-backed experiment, re-save to the same file.
 
 ### Loading
 
 To load an experiment from JSON, specify the filepath again:
 
 ```py
-from ax import load
+from ax.storage.json_store.load import load_experiment
 experiment = load_experiment(filepath)
 ```
 
 ### Customizing
 
-If you add a custom [`Metric`](/api/core.html#module-ax.core.metric) or [`Runner`](../api/core.html#ax.core.runner.Runner) and want to ensure it is saved to JSON properly, simply call [`register_metric`](/api/data.html#.data.users.adamobeng.fbsource.fbcode.ax.ax.storage.metric_registry.register_metric) or [`register_runner`](/api/data.html#.data.users.adamobeng.fbsource.fbcode.ax.ax.storage.runner_registry.register_runner):
+If you add a custom [`Metric`](/api/core.html#module-ax.core.metric) or [`Runner`](../api/core.html#ax.core.runner.Runner) and want to ensure it is saved to JSON properly, create a [`RegistryBundle`](/api/storage.html#ax.storage.registry_bundle.RegistryBundle), which bundles together encoding and decoding logic for use in the various save/load functions as follows:
 
 ```py
-from ax.storage.metric_registry import register_metric
-from ax.storage.runner_registry import register_runner
+from ax import Experiment, Metric, Runner, SearchSpace
+from ax.storage.json_store.load import load_experiment
+from ax.storage.json_store.save import save_experiment
+from ax.storage.registry_bundle import RegistryBundle
 
+# Minimal custom runner/metric.
 class MyRunner(Runner):
-    pass
+    def run():
+        pass
 
 class MyMetric(Metric):
     pass
 
-register_metric(MyMetric)
-register_runner(MyRunner)
+# Minimal experiment must have a search space, plus our custom classes.
+experiment = Experiment(
+    search_space=SearchSpace(parameters=[]),
+    runner=MyRunner(),
+    tracking_metrics=[MyMetric(name="my_metric")]
+)
+
+# A RegistryBundle allows Ax to encode/decode the custom classes.
+bundle = RegistryBundle(
+    runner_clss={MyRunner: None}
+    metric_clss={MyMetric: None},
+)
+
+filepath = "experiments/experiment.json"
+save_experiment(experiment=experiment, filepath=filepath, encoder_registry=bundle.encoder_registry)
+
+loaded_experiment=load_experiment(filepath=filepath, decoder_registry=bundle.decoder_registry)
 ```
 
 ## SQL
 
 ### Saving
 
 To save an experiment to SQL, first initialize a session by passing a URL pointing to your database. Such a URL is typically composed of a dialect (e.g. sqlite, mysql, postgresql), optional driver (DBAPI used to connect to the database; e.g. psycopg2 for postgresql), username, password, hostname, and database name. A more detailed explanation how to generate a URL can be found in the [SQLAlchemy docs](https://docs.sqlalchemy.org/en/13/core/engines.html#database-urls).
@@ -113,29 +133,64 @@
 experiment = load_experiment(experiment_name)
 ```
 
 ### Customizing
 
 **Adding a new metric or runner:**
 
-If you add a custom [`Metric`](/api/core.html#module-ax.core.metric) or [`Runner`](../api/core.html#ax.core.runner.Runner) and want to ensure it is saved to SQL properly, simply call [`register_metric`](/api/data.html#.data.users.adamobeng.fbsource.fbcode.ax.ax.storage.metric_registry.register_metric) or [`register_runner`](/api/data.html#.data.users.adamobeng.fbsource.fbcode.ax.ax.storage.runner_registry.register_runner):
+If you add a custom [`Metric`](/api/core.html#module-ax.core.metric) or [`Runner`](../api/core.html#ax.core.runner.Runner) and want to ensure it is saved to SQL properly, create a [`RegistryBundle`](/api/storage.html#ax.storage.registry_bundle.RegistryBundle), which bundles together encoding and decoding logic for use in the various save/load functions as follows:
 
 ```py
-from ax.storage.metric_registry import register_metric
-from ax.storage.runner_registry import register_runner
+from ax import Experiment, RangeParameter, ParameterType
+from ax.storage.sqa_store.load import load_experiment
+from ax.storage.sqa_store.save import save_experiment
+from ax.storage.sqa_store.sqa_config import SQAConfig
 
+# Minimal custom runner/metric.
 class MyRunner(Runner):
     def run():
         pass
 
 class MyMetric(Metric):
     pass
 
-register_metric(MyMetric)
-register_runner(MyRunner)
+# Minimal experiment for SQA must have a name and a nonempty SearchSpace, plus our custom classes.
+experiment = Experiment(
+    name="my_experiment",
+    search_space=SearchSpace(
+        parameters=[
+            RangeParameter(
+                lower=0,
+                upper=1,
+                name="my_parameter",
+                parameter_type=ParameterType.FLOAT
+            )
+        ]
+    ),
+    runner=MyRunner(),
+    tracking_metrics=[MyMetric(name="my_metric")],
+)
+
+# The RegistryBundle contains our custom classes.
+bundle = RegistryBundle(
+    metric_clss={MyMetric: None},
+    runner_clss={MyRunner: None}
+)
+
+# Abstract this into a SQAConfig as follows, to make loading/saving a bit simpler.
+sqa_config = SQAConfig(
+    json_encoder_registry=bundle.encoder_registry,
+    json_decoder_registry=bundle.decoder_registry,
+    metric_registry=bundle.metric_registry,
+    runner_registry=bundle.runner_registry,
+)
+
+save_experiment(experiment, config=sqa_config)
+
+loaded_experiment = load_experiment(experiment_name="my_experiment", config=sqa_config)
 ```
 
 **Specifying experiment types:**
 
 If you choose to add types to your experiments, create an Enum mapping experiment types to integer representations, pass this Enum to a custom instance of `SQAConfig`, and then pass the config to `sqa_store.save`:
```

### Comparing `ax-platform-0.3.2/docs/trial-evaluation.md` & `ax-platform-0.3.3/docs/trial-evaluation.md`

 * *Files 1% similar despite different names*

```diff
@@ -30,24 +30,24 @@
 
 For example, this evaluation function computes mean and SEM for [Hartmann6](https://www.sfu.ca/~ssurjano/hart6.html) function and for the L2-norm. We return `0.0` for SEM since the observations are noiseless:
 
 ```python
 from ax.utils.measurement.synthetic_functions import hartmann6
 def hartmann_evaluation_function(parameterization):
     x = np.array([parameterization.get(f"x{i+1}") for i in range(6)])
-    # Standard error is 0, since we are computing a synthetic function.
+    # Standard error is 0 since we are computing a synthetic function.
     return {"hartmann6": (hartmann6(x), 0.0), "l2norm": (np.sqrt((x ** 2).sum()), 0.0)}
 ```
 
-This function computes just the objective mean and SEM, assuming the [Branin](https://www.sfu.ca/~ssurjano/branin.html) function is the objective on the experiment:
+This function computes just the objective mean and SEM, assuming the [Branin](https://www.sfu.ca/~ssurjano/branin.html) function is the objective of the experiment:
 
 ```python
 from ax.utils.measurement.synthetic_functions import branin
 def branin_evaluation_function(parameterization):
-    # Standard error is 0, since we are computing a synthetic function.
+    # Standard error is 0 since we are computing a synthetic function.
     return (branin(parameterization.get("x1"), parameterization.get("x2")), 0.0)
 ```
 
 Alternatively, if the SEM is unknown, we could use the following form:
 
 ```python
 lambda parameterization: branin(parameterization.get("x1"), parameterization.get("x2"))
@@ -65,15 +65,15 @@
 The [```optimize```](/api/service.html#ax.service.managed_loop.optimize) function requires an `evaluation_function`, which accepts parameters and returns raw data in the format described above.
 It can also accept a `weight` parameter, a nullable `float` representing the fraction of available data on which the parameterization should be evaluated. For example, this could be a downsampling rate in case of hyperparameter optimization (what portion of data the ML model should be trained on for evaluation) or the percentage of users exposed to a given configuration in A/B testing. This weight is not used in unweighted experiments and defaults to `None`.
 
 ## Developer API
 
 The Developer API is supported by the [```Experiment```](/api/core.html#module-ax.core.experiment) class. In this paradigm, the user specifies:
   * [`Runner`](../api/core.html#ax.core.runner.Runner): Defines how to deploy the experiment.
-  * List of [`Metrics`](../api/core.html#ax.core.metric.Metric): Each defining how to compute/fetch data for a given objective or outcome.
+  * List of [`Metrics`](../api/core.html#ax.core.metric.Metric): Each defines how to compute/fetch data for a given objective or outcome.
 
 The experiment requires a `generator_run` to create a new trial or batch trial.  A generator run can be generated by a model.  The trial then has its own `run` and `mark_complete` methods.
 ```python
 ...
 sobol = Models.SOBOL(exp.search_space)
 for i in range(5):
     trial = exp.new_trial(generator_run=sobol.gen(1))
@@ -86,15 +86,15 @@
     trial = exp.new_trial(generator_run=generator_run)
     trial.run()
     trial.mark_completed()
 ```
 
 ### Custom Metrics
 
-Similar to trial evaluation in the Service API, a custom metric computes a mean and SEM for each arm of a trial.  However, the metric's `fetch_trial_data` method will be called automatically by the experiment's [```fetch_data```](/api/core.html#ax.core.base_trial.BaseTrial.fetch_data) method.  If there are multiple objetives or outcomes that need to be optimized for, each needs its own metric.
+Similar to a trial evaluation in the Service API, a custom metric computes a mean and SEM for each arm of a trial.  However, the metric's `fetch_trial_data` method will be called automatically by the experiment's [```fetch_data```](/api/core.html#ax.core.base_trial.BaseTrial.fetch_data) method.  If there are multiple objectives or outcomes that need to be optimized for, each needs its own metric.
 
 ```python
 class MyMetric(Metric):
     def fetch_trial_data(self, trial):
         records = []
         for arm_name, arm in trial.arms_by_name.items():
             params = arm.parameters
```

### Comparing `ax-platform-0.3.2/docs/why-ax.md` & `ax-platform-0.3.3/docs/why-ax.md`

 * *Files identical despite different names*

### Comparing `ax-platform-0.3.2/scripts/build_ax.sh` & `ax-platform-0.3.3/scripts/build_ax.sh`

 * *Files identical despite different names*

### Comparing `ax-platform-0.3.2/scripts/docker_install.sh` & `ax-platform-0.3.3/scripts/docker_install.sh`

 * *Files identical despite different names*

### Comparing `ax-platform-0.3.2/scripts/insert_api_refs.py` & `ax-platform-0.3.3/scripts/insert_api_refs.py`

 * *Files identical despite different names*

### Comparing `ax-platform-0.3.2/scripts/make_docs.sh` & `ax-platform-0.3.3/scripts/make_docs.sh`

 * *Files identical despite different names*

### Comparing `ax-platform-0.3.2/scripts/make_tutorials.py` & `ax-platform-0.3.3/scripts/make_tutorials.py`

 * *Files 14% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 # LICENSE file in the root directory of this source tree.
 
 import argparse
 import json
 import os
 import tarfile
 import time
-from typing import Optional
+from typing import Dict, Optional
 
 import nbformat
 from bs4 import BeautifulSoup
 from nbconvert import HTMLExporter, ScriptExporter
 from nbconvert.preprocessors import ExecutePreprocessor
 
 
@@ -56,109 +56,136 @@
 function require(deps, fxn) {
     return fxn(...deps.map(dep => dependencyMap[dep]));
 };
 </script>
 """
 
 
+def _get_paths(repo_dir: str, t_dir: Optional[str], tid: str) -> Dict[str, str]:
+    if t_dir is not None:
+        tutorial_dir = os.path.join(repo_dir, "tutorials", t_dir)
+        html_dir = os.path.join(repo_dir, "website", "_tutorials", t_dir)
+        js_dir = os.path.join(repo_dir, "website", "pages", "tutorials", t_dir)
+        py_dir = os.path.join(repo_dir, "website", "static", "files", t_dir)
+
+        for d in [tutorial_dir, html_dir, js_dir, py_dir]:
+            os.makedirs(d, exist_ok=True)
+
+        tutorial_path = os.path.join(tutorial_dir, "{}.ipynb".format(tid))
+        html_path = os.path.join(html_dir, "{}.html".format(tid))
+        js_path = os.path.join(js_dir, "{}.js".format(tid))
+        ipynb_path = os.path.join(py_dir, "{}.ipynb".format(tid))
+        py_path = os.path.join(py_dir, "{}.py".format(tid))
+    else:
+        tutorial_dir = os.path.join(repo_dir, "tutorials")
+        tutorial_path = os.path.join(repo_dir, "tutorials", "{}.ipynb".format(tid))
+        html_path = os.path.join(
+            repo_dir, "website", "_tutorials", "{}.html".format(tid)
+        )
+        js_path = os.path.join(
+            repo_dir, "website", "pages", "tutorials", "{}.js".format(tid)
+        )
+        ipynb_path = os.path.join(
+            repo_dir, "website", "static", "files", "{}.ipynb".format(tid)
+        )
+        py_path = os.path.join(
+            repo_dir, "website", "static", "files", "{}.py".format(tid)
+        )
+
+    paths = {
+        "tutorial_dir": tutorial_dir,
+        "tutorial_path": tutorial_path,
+        "html_path": html_path,
+        "js_path": js_path,
+        "ipynb_path": ipynb_path,
+        "py_path": py_path,
+    }
+    if t_dir is not None:
+        paths["tar_path"] = os.path.join(py_dir, "{}.tar.gz".format(tid))
+    return paths
+
+
 def gen_tutorials(
-    repo_dir: str, exec_tutorials: bool, kernel_name: Optional[str] = None
+    repo_dir: str,
+    exec_tutorials: bool,
+    kernel_name: Optional[str] = None,
+    name: Optional[str] = None,
+    smoke_test: bool = False,
 ) -> None:
     """Generate HTML tutorials for Docusaurus Ax site from Jupyter notebooks.
 
     Also create ipynb and py versions of tutorial in Docusaurus site for
     download.
     """
     has_errors = False
+
     with open(os.path.join(repo_dir, "website", "tutorials.json"), "r") as infile:
         tutorial_config = json.loads(infile.read())
 
     # flatten config dict
     tutorial_configs = [
         config for category in tutorial_config.values() for config in category
     ]
+    # Running only the tutorial described by "name"
+    if name is not None:
+        tutorial_configs = [d for d in tutorial_configs if d["id"] == name]
+        if len(tutorial_configs) == 0:
+            raise RuntimeError(f"No tutorial found with name {name}.")
 
     # prepare paths for converted tutorials & files
     os.makedirs(os.path.join(repo_dir, "website", "_tutorials"), exist_ok=True)
     os.makedirs(os.path.join(repo_dir, "website", "static", "files"), exist_ok=True)
+    if smoke_test:
+        os.environ["SMOKE_TEST"] = str(smoke_test)
 
     for config in tutorial_configs:
         tid = config["id"]
         t_dir = config.get("dir")
         exec_on_build = config.get("exec_on_build", True)
 
         print("Generating {} tutorial".format(tid))
 
-        if t_dir is not None:
-            tutorial_dir = os.path.join(repo_dir, "tutorials", t_dir)
-            html_dir = os.path.join(repo_dir, "website", "_tutorials", t_dir)
-            js_dir = os.path.join(repo_dir, "website", "pages", "tutorials", t_dir)
-            py_dir = os.path.join(repo_dir, "website", "static", "files", t_dir)
-
-            for d in [tutorial_dir, html_dir, js_dir, py_dir]:
-                os.makedirs(d, exist_ok=True)
-
-            tutorial_path = os.path.join(tutorial_dir, "{}.ipynb".format(tid))
-            html_path = os.path.join(html_dir, "{}.html".format(tid))
-            js_path = os.path.join(js_dir, "{}.js".format(tid))
-            ipynb_path = os.path.join(py_dir, "{}.ipynb".format(tid))
-            py_path = os.path.join(py_dir, "{}.py".format(tid))
-            tar_path = os.path.join(py_dir, "{}.tar.gz".format(tid))
-        else:
-            tutorial_dir = os.path.join(repo_dir, "tutorials")
-            tutorial_path = os.path.join(repo_dir, "tutorials", "{}.ipynb".format(tid))
-            html_path = os.path.join(
-                repo_dir, "website", "_tutorials", "{}.html".format(tid)
-            )
-            js_path = os.path.join(
-                repo_dir, "website", "pages", "tutorials", "{}.js".format(tid)
-            )
-            ipynb_path = os.path.join(
-                repo_dir, "website", "static", "files", "{}.ipynb".format(tid)
-            )
-            py_path = os.path.join(
-                repo_dir, "website", "static", "files", "{}.py".format(tid)
-            )
+        paths = _get_paths(repo_dir=repo_dir, t_dir=t_dir, tid=tid)
 
         # load notebook
-        with open(tutorial_path, "r") as infile:
+        with open(paths["tutorial_path"], "r") as infile:
             nb_str = infile.read()
             nb = nbformat.reads(nb_str, nbformat.NO_CONVERT)
 
         # track total exec time (non-None if exec_on_build=True)
         total_time = None
 
         if exec_tutorials and exec_on_build:
             print("Executing tutorial {}".format(tid))
             kwargs = {"kernel_name": kernel_name} if kernel_name is not None else {}
-            # 2.5 hours, in seconds
-            timeout = int(60 * 60 * 2.5)
+            # 2.5 hours, in seconds; 1 hour if smoke test mode
+            timeout = int(60 * 60) if smoke_test else int(60 * 60 * 2.5)
             ep = ExecutePreprocessor(timeout=timeout, **kwargs)
             start_time = time.time()
 
             # try / catch failures for now
             # will re-raise at the end
             try:
                 # execute notebook, using `tutorial_dir` as working directory
-                ep.preprocess(nb, {"metadata": {"path": tutorial_dir}})
+                ep.preprocess(nb, {"metadata": {"path": paths["tutorial_dir"]}})
                 total_time = time.time() - start_time
                 print(
                     "Done executing tutorial {}. Took {:.2f} seconds.".format(
                         tid, total_time
                     )
                 )
             except Exception as exc:
                 has_errors = True
                 print("Couldn't execute tutorial {}!".format(tid))
                 print(exc)
                 total_time = None
 
         # convert notebook to HTML
         exporter = HTMLExporter(template_name="classic")
-        html, meta = exporter.from_notebook_node(nb)
+        html, _ = exporter.from_notebook_node(nb)
 
         # pull out html div for notebook
         soup = BeautifulSoup(html, "html.parser")
         nb_meat = soup.find("div", {"id": "notebook-container"})
         del nb_meat.attrs["id"]
         nb_meat.attrs["class"] = ["notebook"]
 
@@ -172,60 +199,79 @@
                 # replace `#` in CSS
                 iframe.attrs["src"] = iframe.attrs["src"].replace("#", "%23")
                 html_div.contents = [iframe]
 
         html_out = MOCK_JS_REQUIRES + str(nb_meat)
 
         # generate HTML file
-        with open(html_path, "w") as html_outfile:
+        with open(paths["html_path"], "w") as html_outfile:
             html_outfile.write(html_out)
 
         # generate JS file
         t_dir_js = t_dir if t_dir else ""
         script = TEMPLATE.format(
             t_dir=t_dir_js,
             tid=tid,
             total_time=total_time if total_time is not None else "null",
         )
-        with open(js_path, "w") as js_outfile:
+        with open(paths["js_path"], "w") as js_outfile:
             js_outfile.write(script)
 
         # output tutorial in both ipynb & py form
-        nbformat.write(nb, ipynb_path)
+        nbformat.write(nb, paths["ipynb_path"])
         exporter = ScriptExporter()
-        script, meta = exporter.from_notebook_node(nb)
-        with open(py_path, "w") as py_outfile:
+        script, _ = exporter.from_notebook_node(nb)
+        with open(paths["py_path"], "w") as py_outfile:
             py_outfile.write(script)
 
         # create .tar archive (if necessary)
         if t_dir is not None:
-            with tarfile.open(tar_path, "w:gz") as tar:
-                tar.add(tutorial_dir, arcname=os.path.basename(tutorial_dir))
+            with tarfile.open(paths["tar_path"], "w:gz") as tar:
+                tar.add(
+                    paths["tutorial_dir"],
+                    arcname=os.path.basename(paths["tutorial_dir"]),
+                )
 
     if has_errors:
         raise Exception("There are errors in tutorials, will not continue to publish")
 
 
 if __name__ == "__main__":
     parser = argparse.ArgumentParser(
         description="Generate JS, HTML, ipynb, and py files for tutorials."
     )
     parser.add_argument(
         "-w", "--repo_dir", metavar="path", required=True, help="Ax repo directory."
     )
     parser.add_argument(
+        "-s", "--smoke", action="store_true", help="Run in smoke test mode."
+    )
+    parser.add_argument(
         "-e",
         "--exec_tutorials",
         action="store_true",
         default=False,
         help="Execute tutorials (instead of just converting).",
     )
     parser.add_argument(
         "-k",
         "--kernel_name",
         required=False,
         default=None,
         type=str,
         help="Name of IPython / Jupyter kernel to use for executing notebooks.",
     )
+    parser.add_argument(
+        "-n",
+        "--name",
+        help="Run a specific tutorial by name. The name should not include the "
+        ".ipynb extension. If the tutorial is on the ignore list, you still need "
+        "to specify --include-ignored.",
+    )
     args = parser.parse_args()
-    gen_tutorials(args.repo_dir, args.exec_tutorials, args.kernel_name)
+    gen_tutorials(
+        args.repo_dir,
+        args.exec_tutorials,
+        args.kernel_name,
+        smoke_test=args.smoke,
+        name=args.name,
+    )
```

### Comparing `ax-platform-0.3.2/scripts/parse_sphinx.py` & `ax-platform-0.3.3/scripts/parse_sphinx.py`

 * *Files identical despite different names*

### Comparing `ax-platform-0.3.2/scripts/patch_site_config.py` & `ax-platform-0.3.3/scripts/patch_site_config.py`

 * *Files identical despite different names*

### Comparing `ax-platform-0.3.2/scripts/publish_site.sh` & `ax-platform-0.3.3/scripts/publish_site.sh`

 * *Files identical despite different names*

### Comparing `ax-platform-0.3.2/scripts/update_versions_html.py` & `ax-platform-0.3.3/scripts/update_versions_html.py`

 * *Files identical despite different names*

### Comparing `ax-platform-0.3.2/scripts/validate_sphinx.py` & `ax-platform-0.3.3/scripts/validate_sphinx.py`

 * *Files identical despite different names*

### Comparing `ax-platform-0.3.2/scripts/versions.js` & `ax-platform-0.3.3/scripts/versions.js`

 * *Files identical despite different names*

### Comparing `ax-platform-0.3.2/scripts/wheels_build.ps1` & `ax-platform-0.3.3/scripts/wheels_build.ps1`

 * *Files identical despite different names*

### Comparing `ax-platform-0.3.2/setup.py` & `ax-platform-0.3.3/setup.py`

 * *Files identical despite different names*

### Comparing `ax-platform-0.3.2/sphinx/Makefile` & `ax-platform-0.3.3/sphinx/Makefile`

 * *Files identical despite different names*

### Comparing `ax-platform-0.3.2/sphinx/make.bat` & `ax-platform-0.3.3/sphinx/make.bat`

 * *Files identical despite different names*

### Comparing `ax-platform-0.3.2/sphinx/source/benchmark.rst` & `ax-platform-0.3.3/sphinx/source/benchmark.rst`

 * *Files identical despite different names*

### Comparing `ax-platform-0.3.2/sphinx/source/conf.py` & `ax-platform-0.3.3/sphinx/source/conf.py`

 * *Files identical despite different names*

### Comparing `ax-platform-0.3.2/sphinx/source/core.rst` & `ax-platform-0.3.3/sphinx/source/core.rst`

 * *Files identical despite different names*

### Comparing `ax-platform-0.3.2/sphinx/source/early_stopping.rst` & `ax-platform-0.3.3/sphinx/source/early_stopping.rst`

 * *Files identical despite different names*

### Comparing `ax-platform-0.3.2/sphinx/source/exceptions.rst` & `ax-platform-0.3.3/sphinx/source/exceptions.rst`

 * *Files identical despite different names*

### Comparing `ax-platform-0.3.2/sphinx/source/global_stopping.rst` & `ax-platform-0.3.3/sphinx/source/global_stopping.rst`

 * *Files identical despite different names*

### Comparing `ax-platform-0.3.2/sphinx/source/index.rst` & `ax-platform-0.3.3/sphinx/source/index.rst`

 * *Files identical despite different names*

### Comparing `ax-platform-0.3.2/sphinx/source/metrics.rst` & `ax-platform-0.3.3/sphinx/source/metrics.rst`

 * *Files identical despite different names*

### Comparing `ax-platform-0.3.2/sphinx/source/modelbridge.rst` & `ax-platform-0.3.3/sphinx/source/modelbridge.rst`

 * *Files identical despite different names*

### Comparing `ax-platform-0.3.2/sphinx/source/models.rst` & `ax-platform-0.3.3/sphinx/source/models.rst`

 * *Files 2% similar despite different names*

```diff
@@ -260,14 +260,30 @@
 ~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~
 
 .. automodule:: ax.models.torch.botorch_modular.utils
     :members:
     :undoc-members:
     :show-inheritance:
 
+ax.models.torch.botorch_modular.kernels module
+~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~
+
+.. automodule:: ax.models.torch.botorch_modular.kernels
+    :members:
+    :undoc-members:
+    :show-inheritance:
+
+ax.models.torch.botorch_modular.input_constructors.covar_modules module
+~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~
+
+.. automodule:: ax.models.torch.botorch_modular.input_constructors.covar_modules
+    :members:
+    :undoc-members:
+    :show-inheritance:
+
 ax.models.torch.cbo_lcea module
 ~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~
 
 .. automodule:: ax.models.torch.cbo_lcea
     :members:
     :undoc-members:
     :show-inheritance:
```

### Comparing `ax-platform-0.3.2/sphinx/source/plot.rst` & `ax-platform-0.3.3/sphinx/source/plot.rst`

 * *Files identical despite different names*

### Comparing `ax-platform-0.3.2/sphinx/source/runners.rst` & `ax-platform-0.3.3/sphinx/source/runners.rst`

 * *Files identical despite different names*

### Comparing `ax-platform-0.3.2/sphinx/source/service.rst` & `ax-platform-0.3.3/sphinx/source/service.rst`

 * *Files identical despite different names*

### Comparing `ax-platform-0.3.2/sphinx/source/storage.rst` & `ax-platform-0.3.3/sphinx/source/storage.rst`

 * *Files identical despite different names*

### Comparing `ax-platform-0.3.2/sphinx/source/telemetry.rst` & `ax-platform-0.3.3/sphinx/source/telemetry.rst`

 * *Files identical despite different names*

### Comparing `ax-platform-0.3.2/sphinx/source/utils.rst` & `ax-platform-0.3.3/sphinx/source/utils.rst`

 * *Files 1% similar despite different names*

```diff
@@ -209,14 +209,22 @@
 ~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~
 
 .. automodule:: ax.utils.stats.statstools
     :members:
     :undoc-members:
     :show-inheritance:
 
+Model Fit Metrics
+~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~
+
+.. automodule:: ax.utils.stats.model_fit_stats
+    :members:
+    :undoc-members:
+    :show-inheritance:
+
 Storage
 ---------------
 
 Deletion
 ~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~
 
 .. automodule:: ax.utils.storage.sqa.delete
```

### Comparing `ax-platform-0.3.2/tutorials/Setup_and_Usage_of_BoTorch_Models_in_Ax.ipynb` & `ax-platform-0.3.3/tutorials/Setup_and_Usage_of_BoTorch_Models_in_Ax.ipynb`

 * *Files identical despite different names*

### Comparing `ax-platform-0.3.2/tutorials/early_stopping/mnist_train_nas.py` & `ax-platform-0.3.3/tutorials/early_stopping/mnist_train_nas.py`

 * *Files identical despite different names*

### Comparing `ax-platform-0.3.2/tutorials/factorial.ipynb` & `ax-platform-0.3.3/tutorials/factorial.ipynb`

 * *Files identical despite different names*

### Comparing `ax-platform-0.3.2/tutorials/generation_strategy.ipynb` & `ax-platform-0.3.3/tutorials/generation_strategy.ipynb`

 * *Files identical despite different names*

### Comparing `ax-platform-0.3.2/tutorials/gpei_hartmann_developer.ipynb` & `ax-platform-0.3.3/tutorials/gpei_hartmann_developer.ipynb`

 * *Files identical despite different names*

### Comparing `ax-platform-0.3.2/tutorials/gpei_hartmann_loop.ipynb` & `ax-platform-0.3.3/tutorials/gpei_hartmann_loop.ipynb`

 * *Files identical despite different names*

### Comparing `ax-platform-0.3.2/tutorials/gpei_hartmann_service.ipynb` & `ax-platform-0.3.3/tutorials/gpei_hartmann_service.ipynb`

 * *Files identical despite different names*

### Comparing `ax-platform-0.3.2/tutorials/human_in_the_loop/hitl_data.json` & `ax-platform-0.3.3/tutorials/human_in_the_loop/hitl_data.json`

 * *Files identical despite different names*

### Comparing `ax-platform-0.3.2/tutorials/human_in_the_loop/hitl_exp.json` & `ax-platform-0.3.3/tutorials/human_in_the_loop/hitl_exp.json`

 * *Files identical despite different names*

### Comparing `ax-platform-0.3.2/tutorials/human_in_the_loop/human_in_the_loop.ipynb` & `ax-platform-0.3.3/tutorials/human_in_the_loop/human_in_the_loop.ipynb`

 * *Files identical despite different names*

### Comparing `ax-platform-0.3.2/tutorials/modular_botax.ipynb` & `ax-platform-0.3.3/tutorials/modular_botax.ipynb`

 * *Files 11% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9949490129651328%*

 * *Differences: {"'cells'": "{3: {'outputs': {0: {'text': ['[INFO 06-07 16:00:42] ax.core.experiment: The is_test "*

 * *            'flag has been set to True. This flag is meant purely for development and integration '*

 * *            'testing purposes. If you are running a live experiment, please set this flag to '*

 * *            "False\\n']}}}, 4: {'outputs': {0: {'text': ['[INFO 06-07 16:00:42] "*

 * *            'ax.modelbridge.transforms.standardize_y: Outcome branin is constant, within '*

 * *            "tolerance.\\n']}}}, 6: {'output […]*

```diff
@@ -89,15 +89,15 @@
                 "originalKey": "72934cf2-4ecf-483a-93bd-4df88b19a7b8"
             },
             "outputs": [
                 {
                     "name": "stderr",
                     "output_type": "stream",
                     "text": [
-                        "[INFO 05-05 14:54:04] ax.core.experiment: The is_test flag has been set to True. This flag is meant purely for development and integration testing purposes. If you are running a live experiment, please set this flag to False\n"
+                        "[INFO 06-07 16:00:42] ax.core.experiment: The is_test flag has been set to True. This flag is meant purely for development and integration testing purposes. If you are running a live experiment, please set this flag to False\n"
                     ]
                 }
             ],
             "source": [
                 "experiment = get_branin_experiment(with_trial=True)\n",
                 "data = get_branin_data(trials=[experiment.trials[0]])"
             ]
@@ -110,15 +110,15 @@
                 "originalKey": "e571212c-7872-4ebc-b646-8dad8d4266fd"
             },
             "outputs": [
                 {
                     "name": "stderr",
                     "output_type": "stream",
                     "text": [
-                        "[INFO 05-05 14:54:04] ax.modelbridge.transforms.standardize_y: Outcome branin is constant, within tolerance.\n"
+                        "[INFO 06-07 16:00:42] ax.modelbridge.transforms.standardize_y: Outcome branin is constant, within tolerance.\n"
                     ]
                 }
             ],
             "source": [
                 "# `Models` automatically selects a model + model bridge combination.\n",
                 "# For `BOTORCH_MODULAR`, it will select `BoTorchModel` and `TorchModelBridge`.\n",
                 "model_bridge_with_GPEI = Models.BOTORCH_MODULAR(\n",
@@ -144,22 +144,14 @@
             "execution_count": 4,
             "id": "consecutive-summary",
             "metadata": {
                 "originalKey": "59582fc6-8089-4320-864e-d98ee271d4f7"
             },
             "outputs": [
                 {
-                    "name": "stderr",
-                    "output_type": "stream",
-                    "text": [
-                        "/Users/balandat/Code/gpytorch/gpytorch/distributions/multivariate_normal.py:259: NumericalWarning: Negative variance values detected. This is likely due to numerical instabilities. Rounding negative variances up to 1e-10.\n",
-                        "  warnings.warn(\n"
-                    ]
-                },
-                {
                     "data": {
                         "text/plain": [
                             "Arm(parameters={'x1': 10.0, 'x2': 0.0})"
                         ]
                     },
                     "execution_count": 4,
                     "metadata": {},
@@ -315,15 +307,15 @@
                 "originalKey": "db0feafe-8af9-40a3-9f67-72c7d1fd808e"
             },
             "source": [
                 "## 2D. `Surrogate` and `Acquisition` Q&A\n",
                 "\n",
                 "**Why is the `surrogate` argument expected to be an instance, but `botorch_acqf_class` \u2013\u2013 a class?** Because a BoTorch `AcquisitionFunction` object (and therefore its Ax wrapper, `Acquisition`) is ephemeral: it is constructed, immediately used, and destroyed during `BoTorchModel.gen`, so there is no reason to keep around an `Acquisition` instance. A `Surrogate`, on another hand, is kept in memory as long as its parent `BoTorchModel` is.\n",
                 "\n",
-                "**How to know when to use specify acquisition_class (and thereby a non-default Acquisition type) instead of just passing in botorch_acqf_class?** In short, custom `Acquisition` subclasses are needed when a given `AcquisitionFunction` in BoTorch needs some non-standard subcomponents or inputs (e.g. a custom BoTorch `AcquisitionObjective`). <TODO>\n",
+                "**How to know when to use specify acquisition_class (and thereby a non-default Acquisition type) instead of just passing in botorch_acqf_class?** In short, custom `Acquisition` subclasses are needed when a given `AcquisitionFunction` in BoTorch needs some non-standard subcomponents or inputs (e.g. a custom BoTorch `MCAcquisitionObjective`). <TODO>\n",
                 "\n",
                 "**Please post any other questions you have to our dedicated issue on Github: https://github.com/facebook/Ax/issues/363.** This functionality is in beta-release and your feedback will be of great help to us!"
             ]
         },
         {
             "cell_type": "markdown",
             "id": "violent-course",
@@ -428,53 +420,51 @@
                 "2. (Optional) If a given `AcquisitionFunction` requires specific options passed to the BoTorch `optimize_acqf`, it's possible to add default optimizer options for a given `AcquisitionFunction` to avoid always manually passing them via `acquisition_options`.\n",
                 "3. Specify the BoTorch `AcquisitionFunction` class as `botorch_acqf_class` to `BoTorchModel`\n",
                 "4. (Optional) Pass any additional keyword arguments to acquisition function constructor or to the optimizer function via `acquisition_options` argument to `BoTorchModel`."
             ]
         },
         {
             "cell_type": "code",
-            "execution_count": 11,
+            "execution_count": 9,
             "id": "interested-search",
             "metadata": {
                 "code_folding": [],
                 "hidden_ranges": [],
                 "originalKey": "6967ce3e-929b-4d9a-8cd1-72bf94f0be3a"
             },
             "outputs": [
                 {
                     "data": {
                         "text/plain": [
-                            "<ax.models.torch.botorch_modular.model.BoTorchModel at 0x7fabd0852b50>"
+                            "<ax.models.torch.botorch_modular.model.BoTorchModel at 0x7fd2d820b4c0>"
                         ]
                     },
-                    "execution_count": 11,
+                    "execution_count": 9,
                     "metadata": {},
                     "output_type": "execute_result"
                 }
             ],
             "source": [
                 "from ax.models.torch.botorch_modular.optimizer_argparse import optimizer_argparse\n",
                 "from botorch.acquisition.acquisition import AcquisitionFunction\n",
                 "from botorch.acquisition.input_constructors import MaybeDict, acqf_input_constructor\n",
-                "from botorch.acquisition.objective import AcquisitionObjective\n",
                 "from botorch.utils.datasets import SupervisedDataset\n",
                 "from torch import Tensor\n",
                 "\n",
                 "\n",
                 "class MyAcquisitionFunctionClass(AcquisitionFunction):\n",
                 "    ...  # Actual contents of the acquisition function class.\n",
                 "\n",
                 "\n",
                 "# 1. Add input constructor\n",
                 "@acqf_input_constructor(MyAcquisitionFunctionClass)\n",
                 "def construct_inputs_my_acqf(\n",
                 "    model: Model,\n",
                 "    training_data: MaybeDict[SupervisedDataset],\n",
                 "    objective_thresholds: Tensor,\n",
-                "    objective: Optional[AcquisitionObjective] = None,\n",
                 "    **kwargs: Any,\n",
                 ") -> Dict[str, Any]:\n",
                 "    pass\n",
                 "\n",
                 "\n",
                 "# 2. Register default optimizer options\n",
                 "@optimizer_argparse.register(MyAcquisitionFunctionClass)\n",
@@ -522,86 +512,84 @@
                 "To simplify the instantiation of an Ax ModelBridge and its undelying Model, Ax provides a [`Models` registry enum](https://github.com/facebook/Ax/blob/main/ax/modelbridge/registry.py#L355). When calling entries of that enum (e.g. `Models.BOTORCH_MODULAR(experiment, data)`), the inputs are automatically distributed between a `Model` and a `ModelBridge` for a given setup. A call to a `Model` enum member yields a model bridge with an underlying model, ready for use to generate candidates.\n",
                 "\n",
                 "Here we use `Models.BOTORCH_MODULAR` to set up a model with all-default subcomponents:"
             ]
         },
         {
             "cell_type": "code",
-            "execution_count": 12,
+            "execution_count": 10,
             "id": "attached-border",
             "metadata": {
                 "originalKey": "385b2f30-fd86-4d88-8784-f238ea8a6abb"
             },
             "outputs": [
                 {
                     "name": "stderr",
                     "output_type": "stream",
                     "text": [
-                        "[INFO 05-05 14:54:04] ax.modelbridge.transforms.standardize_y: Outcome branin is constant, within tolerance.\n",
-                        "/Users/balandat/Code/gpytorch/gpytorch/distributions/multivariate_normal.py:259: NumericalWarning: Negative variance values detected. This is likely due to numerical instabilities. Rounding negative variances up to 1e-10.\n",
-                        "  warnings.warn(\n"
+                        "[INFO 06-07 16:00:43] ax.modelbridge.transforms.standardize_y: Outcome branin is constant, within tolerance.\n"
                     ]
                 },
                 {
                     "data": {
                         "text/plain": [
                             "GeneratorRun(1 arms, total weight 1.0)"
                         ]
                     },
-                    "execution_count": 12,
+                    "execution_count": 10,
                     "metadata": {},
                     "output_type": "execute_result"
                 }
             ],
             "source": [
                 "model_bridge_with_GPEI = Models.BOTORCH_MODULAR(\n",
                 "    experiment=experiment,\n",
                 "    data=data,\n",
                 ")\n",
                 "model_bridge_with_GPEI.gen(1)"
             ]
         },
         {
             "cell_type": "code",
-            "execution_count": 13,
+            "execution_count": 11,
             "id": "powerful-gamma",
             "metadata": {
                 "originalKey": "89930a31-e058-434b-b587-181931e247b6"
             },
             "outputs": [
                 {
                     "data": {
                         "text/plain": [
                             "botorch.acquisition.monte_carlo.qNoisyExpectedImprovement"
                         ]
                     },
-                    "execution_count": 13,
+                    "execution_count": 11,
                     "metadata": {},
                     "output_type": "execute_result"
                 }
             ],
             "source": [
                 "model_bridge_with_GPEI.model.botorch_acqf_class"
             ]
         },
         {
             "cell_type": "code",
-            "execution_count": 14,
+            "execution_count": 12,
             "id": "improved-replication",
             "metadata": {
                 "originalKey": "f9a9cb14-20c3-4e1d-93a3-6a35c281ae01"
             },
             "outputs": [
                 {
                     "data": {
                         "text/plain": [
                             "botorch.models.gp_regression.FixedNoiseGP"
                         ]
                     },
-                    "execution_count": 14,
+                    "execution_count": 12,
                     "metadata": {},
                     "output_type": "execute_result"
                 }
             ],
             "source": [
                 "model_bridge_with_GPEI.model.surrogate.botorch_model_class"
             ]
@@ -614,38 +602,38 @@
             },
             "source": [
                 "We can use the same `Models.BOTORCH_MODULAR` to set up a model for multi-objective optimization:"
             ]
         },
         {
             "cell_type": "code",
-            "execution_count": 15,
+            "execution_count": 13,
             "id": "documentary-jurisdiction",
             "metadata": {
                 "originalKey": "8001de33-d9d9-4888-a5d1-7a59ebeccfd5"
             },
             "outputs": [
                 {
                     "name": "stderr",
                     "output_type": "stream",
                     "text": [
-                        "[INFO 05-05 14:54:04] ax.core.experiment: The is_test flag has been set to True. This flag is meant purely for development and integration testing purposes. If you are running a live experiment, please set this flag to False\n",
-                        "[INFO 05-05 14:54:04] ax.modelbridge.transforms.standardize_y: Outcome branin_a is constant, within tolerance.\n",
-                        "[INFO 05-05 14:54:04] ax.modelbridge.transforms.standardize_y: Outcome branin_b is constant, within tolerance.\n",
-                        "/Users/balandat/Code/gpytorch/gpytorch/distributions/multivariate_normal.py:259: NumericalWarning: Negative variance values detected. This is likely due to numerical instabilities. Rounding negative variances up to 1e-10.\n",
+                        "[INFO 06-07 16:00:43] ax.core.experiment: The is_test flag has been set to True. This flag is meant purely for development and integration testing purposes. If you are running a live experiment, please set this flag to False\n",
+                        "[INFO 06-07 16:00:43] ax.modelbridge.transforms.standardize_y: Outcome branin_a is constant, within tolerance.\n",
+                        "[INFO 06-07 16:00:43] ax.modelbridge.transforms.standardize_y: Outcome branin_b is constant, within tolerance.\n",
+                        "/Users/santorella/repos/botorch/botorch/optim/initializers.py:403: BadInitialCandidatesWarning: Unable to find non-zero acquisition function values - initial conditions are being selected randomly.\n",
                         "  warnings.warn(\n"
                     ]
                 },
                 {
                     "data": {
                         "text/plain": [
                             "GeneratorRun(1 arms, total weight 1.0)"
                         ]
                     },
-                    "execution_count": 15,
+                    "execution_count": 13,
                     "metadata": {},
                     "output_type": "execute_result"
                 }
             ],
             "source": [
                 "model_bridge_with_EHVI = Models.BOTORCH_MODULAR(\n",
                 "    experiment=get_branin_experiment_with_multi_objective(\n",
@@ -654,50 +642,50 @@
                 "    data=get_branin_data_multi_objective(),\n",
                 ")\n",
                 "model_bridge_with_EHVI.gen(1)"
             ]
         },
         {
             "cell_type": "code",
-            "execution_count": 16,
+            "execution_count": 14,
             "id": "changed-maintenance",
             "metadata": {
                 "originalKey": "dcfdbecc-4a9a-49ac-ad55-0bc04b2ec566"
             },
             "outputs": [
                 {
                     "data": {
                         "text/plain": [
                             "botorch.acquisition.multi_objective.monte_carlo.qNoisyExpectedHypervolumeImprovement"
                         ]
                     },
-                    "execution_count": 16,
+                    "execution_count": 14,
                     "metadata": {},
                     "output_type": "execute_result"
                 }
             ],
             "source": [
                 "model_bridge_with_EHVI.model.botorch_acqf_class"
             ]
         },
         {
             "cell_type": "code",
-            "execution_count": 17,
+            "execution_count": 15,
             "id": "operating-shelf",
             "metadata": {
                 "originalKey": "16727a51-337d-4715-bf51-9cb6637a950f"
             },
             "outputs": [
                 {
                     "data": {
                         "text/plain": [
                             "botorch.models.gp_regression.FixedNoiseGP"
                         ]
                     },
-                    "execution_count": 17,
+                    "execution_count": 15,
                     "metadata": {},
                     "output_type": "execute_result"
                 }
             ],
             "source": [
                 "model_bridge_with_EHVI.model.surrogate.botorch_model_class"
             ]
@@ -724,15 +712,15 @@
                 "Generation strategy is a key concept in Ax, enabling use of Service API (a.k.a. `AxClient`) and many other higher-level abstractions. A `GenerationStrategy` allows to chain multiple models in Ax and thereby automate candidate generation. Refer to the \"Generation Strategy\" tutorial for more detail in generation strategies.\n",
                 "\n",
                 "An example generation stategy with the modular `BoTorchModel` would look like this:"
             ]
         },
         {
             "cell_type": "code",
-            "execution_count": 18,
+            "execution_count": 16,
             "id": "received-registration",
             "metadata": {
                 "originalKey": "f7eabbcf-607c-4bed-9a0e-6ac6e8b04350"
             },
             "outputs": [],
             "source": [
                 "from ax.modelbridge.generation_strategy import GenerationStep, GenerationStrategy\n",
@@ -772,34 +760,34 @@
             },
             "source": [
                 "Set up an experiment and generate 10 trials in it, adding synthetic data to experiment after each one:"
             ]
         },
         {
             "cell_type": "code",
-            "execution_count": 19,
+            "execution_count": 17,
             "id": "viral-cheese",
             "metadata": {
                 "originalKey": "30cfcdd7-721d-4f89-b851-7a94140dfad6"
             },
             "outputs": [
                 {
                     "name": "stderr",
                     "output_type": "stream",
                     "text": [
-                        "[INFO 05-05 14:54:04] ax.core.experiment: The is_test flag has been set to True. This flag is meant purely for development and integration testing purposes. If you are running a live experiment, please set this flag to False\n"
+                        "[INFO 06-07 16:00:44] ax.core.experiment: The is_test flag has been set to True. This flag is meant purely for development and integration testing purposes. If you are running a live experiment, please set this flag to False\n"
                     ]
                 },
                 {
                     "data": {
                         "text/plain": [
                             "SearchSpace(parameters=[RangeParameter(name='x1', parameter_type=FLOAT, range=[-5.0, 10.0]), RangeParameter(name='x2', parameter_type=FLOAT, range=[0.0, 15.0])], parameter_constraints=[])"
                         ]
                     },
-                    "execution_count": 19,
+                    "execution_count": 17,
                     "metadata": {},
                     "output_type": "execute_result"
                 }
             ],
             "source": [
                 "experiment = get_branin_experiment(minimize=True)\n",
                 "\n",
@@ -818,115 +806,35 @@
                 "Note that it's important to **specify pending observations** to the call to `gen` to avoid getting the same points re-suggested. Without `pending_observations` argument, Ax models are not aware of points that should be excluded from generation. Points are considered \"pending\" when they belong to `STAGED`, `RUNNING`, or `ABANDONED` trials (with the latter included so model does not re-suggest points that are considered \"bad\" and should not be re-suggested).\n",
                 "\n",
                 "If the call to `get_pending_observation_features` becomes slow in your setup (since it performs data-fetching etc.), you can opt for `get_pending_observation_features_based_on_trial_status` (also from `ax.modelbridge.modelbridge_utils`), but note the limitations of that utility (detailed in its docstring)."
             ]
         },
         {
             "cell_type": "code",
-            "execution_count": 20,
+            "execution_count": 18,
             "id": "casual-spread",
             "metadata": {
                 "originalKey": "58aafd65-a366-4b66-a1b1-31b207037a2e"
             },
             "outputs": [
                 {
-                    "name": "stderr",
-                    "output_type": "stream",
-                    "text": [
-                        "/Users/balandat/Code/gpytorch/gpytorch/utils/cholesky.py:40: NumericalWarning: A not p.d., added jitter of 1.0e-08 to the diagonal\n",
-                        "  warnings.warn(\n"
-                    ]
-                },
-                {
                     "name": "stdout",
                     "output_type": "stream",
                     "text": [
                         "Completed trial #0, suggested by Sobol.\n",
                         "Completed trial #1, suggested by Sobol.\n",
                         "Completed trial #2, suggested by Sobol.\n",
                         "Completed trial #3, suggested by Sobol.\n",
-                        "Completed trial #4, suggested by Sobol.\n"
-                    ]
-                },
-                {
-                    "name": "stderr",
-                    "output_type": "stream",
-                    "text": [
-                        "/Users/balandat/Code/gpytorch/gpytorch/distributions/multivariate_normal.py:259: NumericalWarning: Negative variance values detected. This is likely due to numerical instabilities. Rounding negative variances up to 1e-10.\n",
-                        "  warnings.warn(\n",
-                        "/Users/balandat/Code/gpytorch/gpytorch/utils/cholesky.py:40: NumericalWarning: A not p.d., added jitter of 1.0e-08 to the diagonal\n",
-                        "  warnings.warn(\n"
-                    ]
-                },
-                {
-                    "name": "stdout",
-                    "output_type": "stream",
-                    "text": [
-                        "Completed trial #5, suggested by BoTorch.\n"
-                    ]
-                },
-                {
-                    "name": "stderr",
-                    "output_type": "stream",
-                    "text": [
-                        "/Users/balandat/Code/gpytorch/gpytorch/distributions/multivariate_normal.py:259: NumericalWarning: Negative variance values detected. This is likely due to numerical instabilities. Rounding negative variances up to 1e-10.\n",
-                        "  warnings.warn(\n",
-                        "/Users/balandat/Code/gpytorch/gpytorch/utils/cholesky.py:40: NumericalWarning: A not p.d., added jitter of 1.0e-08 to the diagonal\n",
-                        "  warnings.warn(\n"
-                    ]
-                },
-                {
-                    "name": "stdout",
-                    "output_type": "stream",
-                    "text": [
-                        "Completed trial #6, suggested by BoTorch.\n"
-                    ]
-                },
-                {
-                    "name": "stderr",
-                    "output_type": "stream",
-                    "text": [
-                        "/Users/balandat/Code/gpytorch/gpytorch/distributions/multivariate_normal.py:259: NumericalWarning: Negative variance values detected. This is likely due to numerical instabilities. Rounding negative variances up to 1e-10.\n",
-                        "  warnings.warn(\n",
-                        "/Users/balandat/Code/gpytorch/gpytorch/utils/cholesky.py:40: NumericalWarning: A not p.d., added jitter of 1.0e-08 to the diagonal\n",
-                        "  warnings.warn(\n"
-                    ]
-                },
-                {
-                    "name": "stdout",
-                    "output_type": "stream",
-                    "text": [
-                        "Completed trial #7, suggested by BoTorch.\n"
-                    ]
-                },
-                {
-                    "name": "stderr",
-                    "output_type": "stream",
-                    "text": [
-                        "/Users/balandat/Code/gpytorch/gpytorch/distributions/multivariate_normal.py:259: NumericalWarning: Negative variance values detected. This is likely due to numerical instabilities. Rounding negative variances up to 1e-10.\n",
-                        "  warnings.warn(\n",
-                        "/Users/balandat/Code/gpytorch/gpytorch/utils/cholesky.py:40: NumericalWarning: A not p.d., added jitter of 1.0e-08 to the diagonal\n",
-                        "  warnings.warn(\n"
-                    ]
-                },
-                {
-                    "name": "stdout",
-                    "output_type": "stream",
-                    "text": [
+                        "Completed trial #4, suggested by Sobol.\n",
+                        "Completed trial #5, suggested by BoTorch.\n",
+                        "Completed trial #6, suggested by BoTorch.\n",
+                        "Completed trial #7, suggested by BoTorch.\n",
                         "Completed trial #8, suggested by BoTorch.\n",
                         "Completed trial #9, suggested by BoTorch.\n"
                     ]
-                },
-                {
-                    "name": "stderr",
-                    "output_type": "stream",
-                    "text": [
-                        "/Users/balandat/Code/gpytorch/gpytorch/distributions/multivariate_normal.py:259: NumericalWarning: Negative variance values detected. This is likely due to numerical instabilities. Rounding negative variances up to 1e-10.\n",
-                        "  warnings.warn(\n"
-                    ]
                 }
             ],
             "source": [
                 "for _ in range(10):\n",
                 "    # Produce a new generator run and attach it to experiment as a trial\n",
                 "    generator_run = gs.gen(\n",
                 "        experiment=experiment,\n",
@@ -953,15 +861,15 @@
             },
             "source": [
                 "Now we examine the experiment and observe the trials that were added to it and produced by the generation strategy:"
             ]
         },
         {
             "cell_type": "code",
-            "execution_count": 21,
+            "execution_count": 19,
             "id": "significant-particular",
             "metadata": {
                 "originalKey": "ca12913d-e3fd-4617-a247-e3432665bac1"
             },
             "outputs": [
                 {
                     "data": {
@@ -980,155 +888,155 @@
                             "        text-align: right;\n",
                             "    }\n",
                             "</style>\n",
                             "<table border=\"1\" class=\"dataframe\">\n",
                             "  <thead>\n",
                             "    <tr style=\"text-align: right;\">\n",
                             "      <th></th>\n",
-                            "      <th>branin</th>\n",
                             "      <th>trial_index</th>\n",
                             "      <th>arm_name</th>\n",
-                            "      <th>x1</th>\n",
-                            "      <th>x2</th>\n",
                             "      <th>trial_status</th>\n",
                             "      <th>generation_method</th>\n",
+                            "      <th>branin</th>\n",
+                            "      <th>x1</th>\n",
+                            "      <th>x2</th>\n",
                             "    </tr>\n",
                             "  </thead>\n",
                             "  <tbody>\n",
                             "    <tr>\n",
                             "      <th>0</th>\n",
-                            "      <td>2.516686</td>\n",
                             "      <td>0</td>\n",
                             "      <td>0_0</td>\n",
-                            "      <td>-3.452563</td>\n",
-                            "      <td>11.747097</td>\n",
                             "      <td>COMPLETED</td>\n",
                             "      <td>Sobol</td>\n",
+                            "      <td>18.295380</td>\n",
+                            "      <td>-4.560280</td>\n",
+                            "      <td>12.821902</td>\n",
                             "    </tr>\n",
                             "    <tr>\n",
                             "      <th>1</th>\n",
-                            "      <td>20.213358</td>\n",
                             "      <td>1</td>\n",
                             "      <td>1_0</td>\n",
-                            "      <td>0.016540</td>\n",
-                            "      <td>6.756372</td>\n",
                             "      <td>COMPLETED</td>\n",
                             "      <td>Sobol</td>\n",
+                            "      <td>17.709690</td>\n",
+                            "      <td>0.695902</td>\n",
+                            "      <td>4.371646</td>\n",
                             "    </tr>\n",
                             "    <tr>\n",
                             "      <th>2</th>\n",
-                            "      <td>2.814679</td>\n",
                             "      <td>2</td>\n",
                             "      <td>2_0</td>\n",
-                            "      <td>8.801378</td>\n",
-                            "      <td>2.780774</td>\n",
                             "      <td>COMPLETED</td>\n",
                             "      <td>Sobol</td>\n",
+                            "      <td>55.483925</td>\n",
+                            "      <td>8.846689</td>\n",
+                            "      <td>9.346672</td>\n",
                             "    </tr>\n",
                             "    <tr>\n",
                             "      <th>3</th>\n",
-                            "      <td>8.135274</td>\n",
                             "      <td>3</td>\n",
                             "      <td>3_0</td>\n",
-                            "      <td>9.412488</td>\n",
-                            "      <td>5.246138</td>\n",
                             "      <td>COMPLETED</td>\n",
                             "      <td>Sobol</td>\n",
+                            "      <td>21.169355</td>\n",
+                            "      <td>-0.904083</td>\n",
+                            "      <td>9.831698</td>\n",
                             "    </tr>\n",
                             "    <tr>\n",
                             "      <th>4</th>\n",
-                            "      <td>86.629987</td>\n",
                             "      <td>4</td>\n",
                             "      <td>4_0</td>\n",
-                            "      <td>-2.326716</td>\n",
-                            "      <td>1.280123</td>\n",
                             "      <td>COMPLETED</td>\n",
                             "      <td>Sobol</td>\n",
+                            "      <td>41.183817</td>\n",
+                            "      <td>8.152092</td>\n",
+                            "      <td>7.442010</td>\n",
                             "    </tr>\n",
                             "    <tr>\n",
                             "      <th>5</th>\n",
-                            "      <td>92.951388</td>\n",
                             "      <td>5</td>\n",
                             "      <td>5_0</td>\n",
-                            "      <td>1.478336</td>\n",
-                            "      <td>12.988449</td>\n",
                             "      <td>COMPLETED</td>\n",
                             "      <td>BoTorch</td>\n",
+                            "      <td>129.479026</td>\n",
+                            "      <td>-5.000000</td>\n",
+                            "      <td>6.382025</td>\n",
                             "    </tr>\n",
                             "    <tr>\n",
                             "      <th>6</th>\n",
-                            "      <td>68.276197</td>\n",
                             "      <td>6</td>\n",
                             "      <td>6_0</td>\n",
-                            "      <td>-5.000000</td>\n",
-                            "      <td>9.734009</td>\n",
                             "      <td>COMPLETED</td>\n",
                             "      <td>BoTorch</td>\n",
+                            "      <td>44.640343</td>\n",
+                            "      <td>-1.675659</td>\n",
+                            "      <td>15.000000</td>\n",
                             "    </tr>\n",
                             "    <tr>\n",
                             "      <th>7</th>\n",
-                            "      <td>7.770399</td>\n",
                             "      <td>7</td>\n",
                             "      <td>7_0</td>\n",
-                            "      <td>-2.838986</td>\n",
-                            "      <td>14.193263</td>\n",
                             "      <td>COMPLETED</td>\n",
                             "      <td>BoTorch</td>\n",
+                            "      <td>21.171942</td>\n",
+                            "      <td>2.527968</td>\n",
+                            "      <td>7.163640</td>\n",
                             "    </tr>\n",
                             "    <tr>\n",
                             "      <th>8</th>\n",
-                            "      <td>4.334985</td>\n",
                             "      <td>8</td>\n",
                             "      <td>8_0</td>\n",
-                            "      <td>-2.251821</td>\n",
-                            "      <td>10.855681</td>\n",
                             "      <td>COMPLETED</td>\n",
                             "      <td>BoTorch</td>\n",
+                            "      <td>1.585450</td>\n",
+                            "      <td>3.511702</td>\n",
+                            "      <td>2.737128</td>\n",
                             "    </tr>\n",
                             "    <tr>\n",
                             "      <th>9</th>\n",
-                            "      <td>27.557474</td>\n",
                             "      <td>9</td>\n",
                             "      <td>9_0</td>\n",
-                            "      <td>7.033479</td>\n",
-                            "      <td>4.442162</td>\n",
                             "      <td>COMPLETED</td>\n",
                             "      <td>BoTorch</td>\n",
+                            "      <td>11.785506</td>\n",
+                            "      <td>2.374472</td>\n",
+                            "      <td>0.000000</td>\n",
                             "    </tr>\n",
                             "  </tbody>\n",
                             "</table>\n",
                             "</div>"
                         ],
                         "text/plain": [
-                            "      branin  trial_index arm_name        x1         x2 trial_status  \\\n",
-                            "0   2.516686            0      0_0 -3.452563  11.747097    COMPLETED   \n",
-                            "1  20.213358            1      1_0  0.016540   6.756372    COMPLETED   \n",
-                            "2   2.814679            2      2_0  8.801378   2.780774    COMPLETED   \n",
-                            "3   8.135274            3      3_0  9.412488   5.246138    COMPLETED   \n",
-                            "4  86.629987            4      4_0 -2.326716   1.280123    COMPLETED   \n",
-                            "5  92.951388            5      5_0  1.478336  12.988449    COMPLETED   \n",
-                            "6  68.276197            6      6_0 -5.000000   9.734009    COMPLETED   \n",
-                            "7   7.770399            7      7_0 -2.838986  14.193263    COMPLETED   \n",
-                            "8   4.334985            8      8_0 -2.251821  10.855681    COMPLETED   \n",
-                            "9  27.557474            9      9_0  7.033479   4.442162    COMPLETED   \n",
+                            "   trial_index arm_name trial_status generation_method      branin        x1   \n",
+                            "0            0      0_0    COMPLETED             Sobol   18.295380 -4.560280  \\\n",
+                            "1            1      1_0    COMPLETED             Sobol   17.709690  0.695902   \n",
+                            "2            2      2_0    COMPLETED             Sobol   55.483925  8.846689   \n",
+                            "3            3      3_0    COMPLETED             Sobol   21.169355 -0.904083   \n",
+                            "4            4      4_0    COMPLETED             Sobol   41.183817  8.152092   \n",
+                            "5            5      5_0    COMPLETED           BoTorch  129.479026 -5.000000   \n",
+                            "6            6      6_0    COMPLETED           BoTorch   44.640343 -1.675659   \n",
+                            "7            7      7_0    COMPLETED           BoTorch   21.171942  2.527968   \n",
+                            "8            8      8_0    COMPLETED           BoTorch    1.585450  3.511702   \n",
+                            "9            9      9_0    COMPLETED           BoTorch   11.785506  2.374472   \n",
                             "\n",
-                            "  generation_method  \n",
-                            "0             Sobol  \n",
-                            "1             Sobol  \n",
-                            "2             Sobol  \n",
-                            "3             Sobol  \n",
-                            "4             Sobol  \n",
-                            "5           BoTorch  \n",
-                            "6           BoTorch  \n",
-                            "7           BoTorch  \n",
-                            "8           BoTorch  \n",
-                            "9           BoTorch  "
+                            "          x2  \n",
+                            "0  12.821902  \n",
+                            "1   4.371646  \n",
+                            "2   9.346672  \n",
+                            "3   9.831698  \n",
+                            "4   7.442010  \n",
+                            "5   6.382025  \n",
+                            "6  15.000000  \n",
+                            "7   7.163640  \n",
+                            "8   2.737128  \n",
+                            "9   0.000000  "
                         ]
                     },
-                    "execution_count": 21,
+                    "execution_count": 19,
                     "metadata": {},
                     "output_type": "execute_result"
                 }
             ],
             "source": [
                 "exp_to_df(experiment)"
             ]
@@ -1140,37 +1048,41 @@
                 "originalKey": "c25da720-6d3d-4f16-b878-24f2d2755783"
             },
             "source": [
                 "## 6. Customizing a `Surrogate` or `Acquisition`\n",
                 "\n",
                 "We expect the base `Surrogate` and `Acquisition` classes to work with most BoTorch components, but there could be a case where you would need to subclass one of aforementioned abstractions to handle a given BoTorch component. If you run into a case like this, feel free to open an issue on our [Github issues page](https://github.com/facebook/Ax/issues) \u2013\u2013\u00a0it would be very useful for us to know \n",
                 "\n",
-                "One such example would be a need for a custom `AcquisitionObjective` or for a custom acquisition function optimization utility. To subclass `Acquisition` accordingly, one would override the `get_botorch_objective` method:"
+                "One such example would be a need for a custom `MCAcquisitionObjective` or posterior transform. To subclass `Acquisition` accordingly, one would override the `get_botorch_objective_and_transform` method:"
             ]
         },
         {
             "cell_type": "code",
             "execution_count": 22,
             "id": "organizational-balance",
             "metadata": {
                 "originalKey": "e7f8e413-f01e-4f9d-82c1-4912097637af"
             },
             "outputs": [],
             "source": [
+                "from botorch.acquisition.objective import MCAcquisitionObjective, PosteriorTransform\n",
+                "from botorch.acquisition.risk_measures import RiskMeasureMCObjective\n",
+                "\n",
                 "class CustomObjectiveAcquisition(Acquisition):\n",
-                "    def get_botorch_objective(\n",
+                "    def get_botorch_objective_and_transform(\n",
                 "        self,\n",
                 "        botorch_acqf_class: Type[AcquisitionFunction],\n",
                 "        model: Model,\n",
                 "        objective_weights: Tensor,\n",
                 "        objective_thresholds: Optional[Tensor] = None,\n",
                 "        outcome_constraints: Optional[Tuple[Tensor, Tensor]] = None,\n",
                 "        X_observed: Optional[Tensor] = None,\n",
-                "    ) -> AcquisitionObjective:\n",
-                "        ...  # Produce the desired `AcquisitionObjective` instead of the default"
+                "        risk_measure: Optional[RiskMeasureMCObjective] = None,\n",
+                "    ) -> Tuple[Optional[MCAcquisitionObjective], Optional[PosteriorTransform]]:\n",
+                "        ...  # Produce the desired `MCAcquisitionObjective` and `PosteriorTransform` instead of the default"
             ]
         },
         {
             "cell_type": "markdown",
             "id": "theoretical-horizon",
             "metadata": {
                 "originalKey": "7299f0fc-e19e-4383-99de-ef7a9a987fe9"
@@ -1187,21 +1099,21 @@
                 "originalKey": "07fe169a-78de-437e-9857-7c99cc48eedc"
             },
             "outputs": [
                 {
                     "name": "stderr",
                     "output_type": "stream",
                     "text": [
-                        "[INFO 05-05 14:54:07] ax.modelbridge.transforms.standardize_y: Outcome branin is constant, within tolerance.\n"
+                        "[INFO 06-07 16:01:54] ax.modelbridge.transforms.standardize_y: Outcome branin is constant, within tolerance.\n"
                     ]
                 },
                 {
                     "data": {
                         "text/plain": [
-                            "<ax.modelbridge.torch.TorchModelBridge at 0x7fabd08529d0>"
+                            "<ax.modelbridge.torch.TorchModelBridge at 0x7fd2d821c3a0>"
                         ]
                     },
                     "execution_count": 23,
                     "metadata": {},
                     "output_type": "execute_result"
                 }
             ],
@@ -1308,29 +1220,29 @@
                 "2. specifying serialization logic for a given object that needs to occur among the `Model` or `AcquisitionFunction` options. Tutorial for this is in the works, but in the meantime you can [post an issue on the Ax GitHub](https://github.com/facebook/Ax/issues) to get help with this."
             ]
         }
     ],
     "metadata": {
         "dataExplorerConfig": {},
         "kernelspec": {
-            "display_name": "Python 3",
+            "display_name": "Python 3 (ipykernel)",
             "language": "python",
             "name": "python3"
         },
         "language_info": {
             "codemirror_mode": {
                 "name": "ipython",
                 "version": 3
             },
             "file_extension": ".py",
             "mimetype": "text/x-python",
             "name": "python",
             "nbconvert_exporter": "python",
             "pygments_lexer": "ipython3",
-            "version": "3.8.13"
+            "version": "3.10.8"
         },
         "last_base_url": "https://devbig824.prn1.facebook.com:8090/",
         "last_kernel_id": "249fdd46-baf9-4864-b6fa-cf420e16c166",
         "last_msg_id": "89881794-5fb20f784ca983ce24c9203c_20",
         "last_server_session_id": "4bcf6e9b-c629-479c-bdc2-492a9eca41ef",
         "outputWidgetContext": {}
     },
```

### Comparing `ax-platform-0.3.2/tutorials/multi_task.ipynb` & `ax-platform-0.3.3/tutorials/multi_task.ipynb`

 * *Files 0% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9898677248677249%*

 * *Differences: {"'cells'": "{1: {'source': {insert: [(0, 'import os\\n'), (1, 'import time\\n'), (2, '\\n')], "*

 * *            "delete: [4]}}, 10: {'source': {insert: [(2, '# Number of repeated experiments, each "*

 * *            "with independent observation noise.\\n'), (4, 'if SMOKE_TEST:\\n'), (5, '    n_reps = "*

 * *            "3\\n'), (6, 'else:\\n'), (7, '    n_reps = 1\\n')], delete: [3]}}, 17: {'metadata': "*

 * *            "{delete: ['collapsed']}}, insert: [(2, OrderedDict([('cell_type', 'code'), "*

 * *            "('execution_c […]*

```diff
@@ -28,19 +28,21 @@
             "metadata": {
                 "code_folding": [],
                 "hidden_ranges": [],
                 "originalKey": "3ce827be-d20b-48d3-a6ff-291bd442c748"
             },
             "outputs": [],
             "source": [
+                "import os\n",
+                "import time\n",
+                "\n",
                 "from copy import deepcopy\n",
                 "import numpy as np\n",
                 "import pandas as pd\n",
                 "from scipy.stats import norm\n",
-                "import time\n",
                 "\n",
                 "from ax.core.data import Data\n",
                 "from ax.core.observation import ObservationFeatures, observations_from_data\n",
                 "from ax.core.optimization_config import OptimizationConfig\n",
                 "from ax.core.search_space import SearchSpace\n",
                 "from ax.core.objective import Objective\n",
                 "from ax.runners.synthetic import SyntheticRunner\n",
@@ -56,14 +58,23 @@
                 "from ax.plot.trace import optimization_trace_all_methods\n",
                 "from ax.utils.notebook.plotting import init_notebook_plotting, render\n",
                 "\n",
                 "init_notebook_plotting()"
             ]
         },
         {
+            "cell_type": "code",
+            "execution_count": null,
+            "metadata": {},
+            "outputs": [],
+            "source": [
+                "SMOKE_TEST = os.environ.get(\"SMOKE_TEST\")"
+            ]
+        },
+        {
             "cell_type": "markdown",
             "metadata": {
                 "code_folding": [],
                 "hidden_ranges": [],
                 "originalKey": "76100312-e604-46ed-a123-9b0296ced6ff",
                 "showInput": false
             },
@@ -229,16 +240,20 @@
             "metadata": {
                 "originalKey": "3d124563-8a1f-411e-9822-972568ce1970"
             },
             "outputs": [],
             "source": [
                 "# Settings for the optimization benchmark.\n",
                 "\n",
+                "# Number of repeated experiments, each with independent observation noise.\n",
                 "# This should be changed to 50 to reproduce the results from the paper.\n",
-                "n_reps = 3  # Number of repeated experiments, each with independent observation noise\n",
+                "if SMOKE_TEST:\n",
+                "    n_reps = 3\n",
+                "else:\n",
+                "    n_reps = 1\n",
                 "\n",
                 "n_init_online = 5  # Size of the quasirandom initialization run online\n",
                 "n_init_offline = 20  # Size of the quasirandom initialization run offline\n",
                 "n_opt_online = 5  # Batch size for BO selected points to be run online\n",
                 "n_opt_offline = 20  # Batch size for BO selected to be run offline\n",
                 "n_batches = 3  # Number of optimized BO batches"
             ]
@@ -430,15 +445,14 @@
                 "    for k, r in runners.items():\n",
                 "        r()"
             ]
         },
         {
             "cell_type": "markdown",
             "metadata": {
-                "collapsed": true,
                 "originalKey": "1de5ae27-c925-4599-9425-332765a03416"
             },
             "source": [
                 "#### References\n",
                 "Benjamin Letham and Eytan Bakshy. Bayesian optimization for policy search via online-offline experimentation. _arXiv preprint arXiv:1603.09326_, 2019.\n",
                 "\n",
                 "Kevin Swersky, Jasper Snoek, and Ryan P Adams.  Multi-task Bayesian optimization.  In _Advances in Neural Information Processing Systems_ 26, NIPS, pages 2004\u20132012, 2013."
@@ -457,13 +471,13 @@
                 "version": 3
             },
             "file_extension": ".py",
             "mimetype": "text/x-python",
             "name": "python",
             "nbconvert_exporter": "python",
             "pygments_lexer": "ipython3",
-            "version": "3.9.15"
+            "version": "3.10.8"
         }
     },
     "nbformat": 4,
     "nbformat_minor": 2
 }
```

### Comparing `ax-platform-0.3.2/tutorials/multiobjective_optimization.ipynb` & `ax-platform-0.3.3/tutorials/multiobjective_optimization.ipynb`

 * *Files identical despite different names*

### Comparing `ax-platform-0.3.2/tutorials/raytune_pytorch_cnn.ipynb` & `ax-platform-0.3.3/tutorials/raytune_pytorch_cnn.ipynb`

 * *Files 4% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9888527097902098%*

 * *Differences: {"'cells'": "{0: {'attachments': OrderedDict()}, 1: {'source': {insert: [(4, 'from "*

 * *            "ray.tune.search.ax import AxSearch\\n')], delete: [4]}}, 3: {'attachments': "*

 * *            "OrderedDict()}, 5: {'attachments': OrderedDict()}, 10: {'attachments': "*

 * *            "OrderedDict()}, 12: {'attachments': OrderedDict()}, 13: {'source': {insert: [(4, "*

 * *            "'algo = tune.search.ConcurrencyLimiter(algo, max_concurrent=3)\\n')], delete: [4]}}, "*

 * *            "14: {'attachments': OrderedDict()}, 17: { […]*

```diff
@@ -1,10 +1,11 @@
 {
     "cells": [
         {
+            "attachments": {},
             "cell_type": "markdown",
             "metadata": {
                 "originalKey": "6dba2bea-d97e-4545-9803-4242850e1807"
             },
             "source": [
                 "# Ax Service API with RayTune on PyTorch CNN\n",
                 "\n",
@@ -23,15 +24,15 @@
             },
             "outputs": [],
             "source": [
                 "import logging\n",
                 "\n",
                 "from ray import tune\n",
                 "from ray.tune import report\n",
-                "from ray.tune.suggest.ax import AxSearch\n",
+                "from ray.tune.search.ax import AxSearch\n",
                 "\n",
                 "logger = logging.getLogger(tune.__name__)\n",
                 "logger.setLevel(\n",
                 "    level=logging.CRITICAL\n",
                 ")  # Reduce the number of Ray warnings that are not relevant here."
             ]
         },
@@ -51,14 +52,15 @@
                 "from ax.utils.notebook.plotting import init_notebook_plotting, render\n",
                 "from ax.utils.tutorials.cnn_utils import CNN, evaluate, load_mnist, train\n",
                 "\n",
                 "init_notebook_plotting()"
             ]
         },
         {
+            "attachments": {},
             "cell_type": "markdown",
             "metadata": {
                 "originalKey": "a26e18f8-caa7-411d-809a-61a9229cd6c6"
             },
             "source": [
                 "## 1. Initialize client\n",
                 "We specify `enforce_sequential_optimization` as False, because Ray runs many trials in parallel. With the sequential optimization enforcement, `AxClient` would expect the first few trials to be completed with data before generating more trials.\n",
@@ -74,14 +76,15 @@
             },
             "outputs": [],
             "source": [
                 "ax = AxClient(enforce_sequential_optimization=False)"
             ]
         },
         {
+            "attachments": {},
             "cell_type": "markdown",
             "metadata": {
                 "originalKey": "1766919c-fb6f-4271-a8e1-6f972eee78f3"
             },
             "source": [
                 "## 2. Set up experiment\n",
                 "Here we set up the search space and specify the objective; refer to the Ax API tutorials for more detail."
@@ -138,14 +141,15 @@
             "source": [
                 "load_mnist(\n",
                 "    data_path=\"~/.data\"\n",
                 ")  # Pre-load the dataset before the initial evaluations are executed."
             ]
         },
         {
+            "attachments": {},
             "cell_type": "markdown",
             "metadata": {
                 "originalKey": "5fec848a-3538-489c-bcdd-a74051f48140"
             },
             "source": [
                 "## 3. Define how to evaluate trials\n",
                 "Since we use the Ax Service API here, we evaluate the parameterizations that Ax suggests, using RayTune. The evaluation function follows its usual pattern, taking in a parameterization and outputting an objective value. For detail on evaluation functions, see [Trial Evaluation](https://ax.dev/docs/runner.html). "
@@ -176,14 +180,15 @@
                 "            dtype=torch.float,\n",
                 "            device=device,\n",
                 "        )\n",
                 "    )"
             ]
         },
         {
+            "attachments": {},
             "cell_type": "markdown",
             "metadata": {
                 "originalKey": "dda3574c-5967-43ea-8d23-7a151dc59ec9"
             },
             "source": [
                 "## 4. Run optimization\n",
                 "Execute the Ax optimization and trial evaluation in RayTune using [AxSearch algorithm](https://ray.readthedocs.io/en/latest/tune-searchalg.html#ax-search):"
@@ -199,25 +204,26 @@
             },
             "outputs": [],
             "source": [
                 "# Set up AxSearcher in RayTune\n",
                 "algo = AxSearch(ax_client=ax)\n",
                 "# Wrap AxSearcher in a concurrently limiter, to ensure that Bayesian optimization receives the\n",
                 "# data for completed trials before creating more trials\n",
-                "algo = tune.suggest.ConcurrencyLimiter(algo, max_concurrent=3)\n",
+                "algo = tune.search.ConcurrencyLimiter(algo, max_concurrent=3)\n",
                 "tune.run(\n",
                 "    train_evaluate,\n",
                 "    num_samples=30,\n",
                 "    search_alg=algo,\n",
                 "    verbose=0,  # Set this level to 1 to see status updates and to 2 to also see trial results.\n",
                 "    # To use GPU, specify: resources_per_trial={\"gpu\": 1}.\n",
                 ")"
             ]
         },
         {
+            "attachments": {},
             "cell_type": "markdown",
             "metadata": {
                 "originalKey": "cb00f812-e9e5-4208-a680-adf6619d74c4"
             },
             "source": [
                 "## 5. Retrieve the optimization results"
             ]
@@ -243,14 +249,15 @@
             "outputs": [],
             "source": [
                 "means, covariances = values\n",
                 "means"
             ]
         },
         {
+            "attachments": {},
             "cell_type": "markdown",
             "metadata": {
                 "originalKey": "12a87817-4409-4f07-a912-8d60eff71d68"
             },
             "source": [
                 "## 6. Plot the response surface and optimization trace"
             ]
```

### Comparing `ax-platform-0.3.2/tutorials/saasbo_nehvi.ipynb` & `ax-platform-0.3.3/tutorials/saasbo_nehvi.ipynb`

 * *Files 2% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9863366500490356%*

 * *Differences: {"'cells'": "{7: {'source': {insert: [(0, 'import os\\n'), (1, '\\n')]}}, 21: {'source': ['N_INIT "*

 * *            "= 2 * (d + 1)']}, 28: {'source': {insert: [(7, '        "*

 * *            "num_samples=num_samples,\\n'), (8, '        warmup_steps=warmup_steps,\\n')], delete: "*

 * *            "[13, 12, 4, 3, 2, 1, 0]}}, 29: {'metadata': {delete: ['collapsed']}}, 30: "*

 * *            "{'metadata': {delete: ['collapsed']}}, insert: [(8, OrderedDict([('cell_type', "*

 * *            "'code'), ('execution_count', None), ('metada […]*

```diff
@@ -123,14 +123,16 @@
             "metadata": {
                 "code_folding": [],
                 "hidden_ranges": [],
                 "originalKey": "03b8cd70-54f4-4d4d-8445-60439ba00e27"
             },
             "outputs": [],
             "source": [
+                "import os\n",
+                "\n",
                 "import pandas as pd\n",
                 "from ax import *\n",
                 "\n",
                 "import torch\n",
                 "import numpy as np\n",
                 "\n",
                 "from ax.metrics.noisy_function import GenericNoisyFunctionMetric\n",
@@ -149,14 +151,23 @@
                 "from ax.modelbridge.registry import Models\n",
                 "\n",
                 "# Analysis utilities, including a method to evaluate hypervolumes\n",
                 "from ax.modelbridge.modelbridge_utils import observed_hypervolume"
             ]
         },
         {
+            "cell_type": "code",
+            "execution_count": null,
+            "metadata": {},
+            "outputs": [],
+            "source": [
+                "SMOKE_TEST = os.environ.get(\"SMOKE_TEST\")"
+            ]
+        },
+        {
             "cell_type": "markdown",
             "metadata": {
                 "originalKey": "122d77fa-21b8-4b01-9522-eae5990aba86"
             },
             "source": [
                 "### Load our sample 2-objective problem"
             ]
@@ -335,17 +346,15 @@
             "cell_type": "code",
             "execution_count": null,
             "metadata": {
                 "originalKey": "fb09ef7d-e744-472b-9290-ec24eb40d3fe"
             },
             "outputs": [],
             "source": [
-                "N_INIT = 2 * (d + 1)\n",
-                "N_BATCH = 10\n",
-                "BATCH_SIZE = 4"
+                "N_INIT = 2 * (d + 1)"
             ]
         },
         {
             "cell_type": "code",
             "execution_count": null,
             "metadata": {
                 "code_folding": [],
@@ -410,35 +419,61 @@
                 "experiment = build_experiment()\n",
                 "data = initialize_experiment(experiment)"
             ]
         },
         {
             "cell_type": "code",
             "execution_count": null,
+            "metadata": {},
+            "outputs": [],
+            "source": [
+                "BATCH_SIZE = 4\n",
+                "\n",
+                "if SMOKE_TEST:\n",
+                "    N_BATCH = 1\n",
+                "    num_samples = 128\n",
+                "    warmup_steps = 256\n",
+                "else:\n",
+                "    N_BATCH = 10\n",
+                "    BATCH_SIZE = 4\n",
+                "    num_samples = 256\n",
+                "    warmup_steps = 512"
+            ]
+        },
+        {
+            "cell_type": "code",
+            "execution_count": null,
+            "metadata": {},
+            "outputs": [],
+            "source": [
+                "from ax.core.metric import Metric\n",
+                "from botorch.utils.multi_objective.box_decompositions.dominated import (\n",
+                "    DominatedPartitioning,\n",
+                ")"
+            ]
+        },
+        {
+            "cell_type": "code",
+            "execution_count": null,
             "metadata": {
                 "code_folding": [],
                 "hidden_ranges": [],
                 "originalKey": "8ec2a5a3-bb79-435d-834c-55510ec52b15"
             },
             "outputs": [],
             "source": [
-                "from ax.core.metric import Metric\n",
-                "from botorch.utils.multi_objective.box_decompositions.dominated import (\n",
-                "    DominatedPartitioning,\n",
-                ")\n",
-                "\n",
                 "hv_list = []\n",
                 "model = None\n",
                 "for i in range(N_BATCH):\n",
                 "    model = Models.FULLYBAYESIANMOO(\n",
                 "        experiment=experiment,\n",
                 "        data=data,\n",
                 "        # use fewer num_samples and warmup_steps to speed up this tutorial\n",
-                "        num_samples=256,\n",
-                "        warmup_steps=512,\n",
+                "        num_samples=num_samples,\n",
+                "        warmup_steps=warmup_steps,\n",
                 "        torch_device=tkwargs[\"device\"],\n",
                 "        verbose=False,  # Set to True to print stats from MCMC\n",
                 "        disable_progbar=True,  # Set to False to print a progress bar from MCMC\n",
                 "    )\n",
                 "    generator_run = model.gen(BATCH_SIZE)\n",
                 "    trial = experiment.new_batch_trial(generator_run=generator_run)\n",
                 "    trial.run()\n",
@@ -459,27 +494,25 @@
                 "outcomes = df[[\"a\", \"b\"]].values"
             ]
         },
         {
             "cell_type": "markdown",
             "metadata": {
                 "code_folding": [],
-                "collapsed": true,
                 "hidden_ranges": [],
                 "originalKey": "bafe189b-88cb-4a9e-aeff-2d2945d497da"
             },
             "source": [
                 "## Plot empirical data"
             ]
         },
         {
             "cell_type": "markdown",
             "metadata": {
                 "code_folding": [],
-                "collapsed": true,
                 "hidden_ranges": [],
                 "originalKey": "5cc39663-a778-4600-bf39-57e63a7c2f39",
                 "showInput": false
             },
             "source": [
                 "#### Plot observed hypervolume, with color representing the iteration that a point was generated on."
             ]
@@ -657,14 +690,21 @@
             "execution_count": null,
             "metadata": {},
             "outputs": [],
             "source": [
                 "# compute out-of-sample log likelihood\n",
                 "compute_diagnostics(map_cv)[\"Log likelihood\"]"
             ]
+        },
+        {
+            "cell_type": "code",
+            "execution_count": null,
+            "metadata": {},
+            "outputs": [],
+            "source": []
         }
     ],
     "metadata": {
         "kernelspec": {
             "display_name": "Python 3 (ipykernel)",
             "language": "python",
             "name": "python3"
@@ -675,13 +715,13 @@
                 "version": 3
             },
             "file_extension": ".py",
             "mimetype": "text/x-python",
             "name": "python",
             "nbconvert_exporter": "python",
             "pygments_lexer": "ipython3",
-            "version": "3.9.15"
+            "version": "3.10.8"
         }
     },
     "nbformat": 4,
     "nbformat_minor": 2
 }
```

### Comparing `ax-platform-0.3.2/tutorials/scheduler.ipynb` & `ax-platform-0.3.3/tutorials/scheduler.ipynb`

 * *Files 1% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9997863247863248%*

 * *Differences: {"'cells'": "{37: {'source': {insert: [(0, '## 7. Configuring the scheduler with "*

 * *            "`SchedulerOptions`, like early stopping\\n'), (7, '- `early_stopping_strategy` -- "*

 * *            'determines whether a trial should be stopped given the current state of the '*

 * *            'experiment, so that less promising trials can be terminated quickly. For more on '*

 * *            'this, see the Trial-Level Early Stopping tutorial: '*

 * *            "https://ax.dev/tutorials/early_stopping/early_stopping.html\\n'),  […]*

```diff
@@ -727,23 +727,25 @@
         {
             "cell_type": "markdown",
             "metadata": {
                 "originalKey": "e3f24c9e-3da1-4ee0-ab1c-741f624a6014",
                 "showInput": false
             },
             "source": [
-                "## 7. Configuring the scheduler\n",
+                "## 7. Configuring the scheduler with `SchedulerOptions`, like early stopping\n",
                 "\n",
                 "`Scheduler` exposes many options to configure the exact settings of the closed-loop optimization to perform. A few notable ones are:\n",
                 "- `trial_type` \u2013\u2013\u00a0currently only `Trial` and not `BatchTrial` is supported, but support for `BatchTrial`-s will follow,\n",
                 "- `tolerated_trial_failure_rate` and `min_failed_trials_for_failure_rate_check` \u2013\u2013 together these two settings control how the scheduler monitors the failure rate among trial runs it deploys. Once `min_failed_trials_for_failure_rate_check` is deployed, the scheduler will start checking whether the ratio of failed to total trials is greater than `tolerated_trial_failure_rate`, and if it is, scheduler will exit the optimization with a `FailureRateExceededError`,\n",
                 "- `ttl_seconds_for_trials` \u2013\u2013\u00a0sometimes a failure in a trial run means that it will be difficult to query its status (e.g. due to a crash). If this setting is specified, the Ax `Experiment` will automatically mark trials that have been running for too long (more than their 'time-to-live' (TTL) seconds) as failed,\n",
                 "- `run_trials_in_batches` \u2013\u2013\u00a0if `True`, the scheduler will attempt to run trials not by calling `Scheduler.run_trial` in a loop, but by calling `Scheduler.run_trials` on all ready-to-deploy trials at once. This could allow for saving compute in cases where the deployment operation has large overhead and deploying many trials at once saves compute. Note that using this option successfully will require your scheduler subclass to implement `MySchedulerSubclass.run_trials` and `MySchedulerSubclass.poll_available_capacity`.\n",
+                "- `early_stopping_strategy` -- determines whether a trial should be stopped given the current state of the experiment, so that less promising trials can be terminated quickly. For more on this, see the Trial-Level Early Stopping tutorial: https://ax.dev/tutorials/early_stopping/early_stopping.html\n",
+                "- `global_stopping_strategy` -- determines whether the full optimization should be stopped or not, so that the run terminates when little progress is being made. A `global_stopping_strategy` instance can be passed to `SchedulerOptions` just as it is passed to `AxClient`, as illustrated in the tutorial on Global Stopping Strategy with AxClient: https://ax.dev/tutorials/gss.html\n",
                 "\n",
-                "The rest of the options is described in the docstring below:"
+                "The rest of the options are described in the docstring below:"
             ]
         },
         {
             "cell_type": "code",
             "execution_count": null,
             "metadata": {
                 "executionStartTime": 1646325050451,
```

### Comparing `ax-platform-0.3.2/tutorials/tune_cnn.ipynb` & `ax-platform-0.3.3/tutorials/tune_cnn.ipynb`

 * *Files identical despite different names*

### Comparing `ax-platform-0.3.2/tutorials/visualizations.ipynb` & `ax-platform-0.3.3/tutorials/visualizations.ipynb`

 * *Files identical despite different names*

### Comparing `ax-platform-0.3.2/website/core/Footer.js` & `ax-platform-0.3.3/website/core/Footer.js`

 * *Files identical despite different names*

### Comparing `ax-platform-0.3.2/website/core/Tutorial.js` & `ax-platform-0.3.3/website/core/Tutorial.js`

 * *Files identical despite different names*

### Comparing `ax-platform-0.3.2/website/core/TutorialSidebar.js` & `ax-platform-0.3.3/website/core/TutorialSidebar.js`

 * *Files identical despite different names*

### Comparing `ax-platform-0.3.2/website/pages/en/index.js` & `ax-platform-0.3.3/website/pages/en/index.js`

 * *Files identical despite different names*

### Comparing `ax-platform-0.3.2/website/pages/tutorials/index.js` & `ax-platform-0.3.3/website/pages/tutorials/index.js`

 * *Files 1% similar despite different names*

#### js-beautify {}

```diff
@@ -141,15 +141,15 @@
             function. <
             /li> <
             /ul> <
             ul >
             <
             li >
             <
-            a href = "early_stopping.html" >
+            a href = "early_stopping/early_stopping.html" >
             Trial - Level Early Stopping <
             /a> &
             nbsp; shows how to use trial - level early stopping on an ML training job to save resources and iterate faster. <
             /li> <
             /ul>
 
             {
```

### Comparing `ax-platform-0.3.2/website/siteConfig.js` & `ax-platform-0.3.3/website/siteConfig.js`

 * *Files identical despite different names*

### Comparing `ax-platform-0.3.2/website/static/css/base_sphinx.css` & `ax-platform-0.3.3/website/static/css/base_sphinx.css`

 * *Files identical despite different names*

### Comparing `ax-platform-0.3.2/website/static/css/custom.css` & `ax-platform-0.3.3/website/static/css/custom.css`

 * *Files identical despite different names*

### Comparing `ax-platform-0.3.2/website/static/css/custom_sphinx.css` & `ax-platform-0.3.3/website/static/css/custom_sphinx.css`

 * *Files identical despite different names*

### Comparing `ax-platform-0.3.2/website/static/css/pygments.css` & `ax-platform-0.3.3/website/static/css/pygments.css`

 * *Files identical despite different names*

### Comparing `ax-platform-0.3.2/website/static/img/ax.svg` & `ax-platform-0.3.3/website/static/img/ax.svg`

 * *Files identical despite different names*

### Comparing `ax-platform-0.3.2/website/static/img/ax_lockup.svg` & `ax-platform-0.3.3/website/static/img/ax_lockup.svg`

 * *Files identical despite different names*

### Comparing `ax-platform-0.3.2/website/static/img/ax_lockup_white.svg` & `ax-platform-0.3.3/website/static/img/ax_lockup_white.svg`

 * *Files identical despite different names*

### Comparing `ax-platform-0.3.2/website/static/img/ax_logo_lockup.svg` & `ax-platform-0.3.3/website/static/img/ax_logo_lockup.svg`

 * *Files identical despite different names*

### Comparing `ax-platform-0.3.2/website/static/img/database-solid.svg` & `ax-platform-0.3.3/website/static/img/database-solid.svg`

 * *Files identical despite different names*

### Comparing `ax-platform-0.3.2/website/static/img/dice-solid.svg` & `ax-platform-0.3.3/website/static/img/dice-solid.svg`

 * *Files identical despite different names*

### Comparing `ax-platform-0.3.2/website/static/img/favicon/favicon.ico` & `ax-platform-0.3.3/website/static/img/favicon/favicon.ico`

 * *Files identical despite different names*

### Comparing `ax-platform-0.3.2/website/static/img/favicon.png` & `ax-platform-0.3.3/website/static/img/favicon.png`

 * *Files identical despite different names*

### Comparing `ax-platform-0.3.2/website/static/img/oss_logo.png` & `ax-platform-0.3.3/website/static/img/oss_logo.png`

 * *Files identical despite different names*

### Comparing `ax-platform-0.3.2/website/static/img/th-large-solid.svg` & `ax-platform-0.3.3/website/static/img/th-large-solid.svg`

 * *Files identical despite different names*

### Comparing `ax-platform-0.3.2/website/static/js/mathjax.js` & `ax-platform-0.3.3/website/static/js/mathjax.js`

 * *Files identical despite different names*

### Comparing `ax-platform-0.3.2/website/static/js/plotUtils.js` & `ax-platform-0.3.3/website/static/js/plotUtils.js`

 * *Files identical despite different names*

### Comparing `ax-platform-0.3.2/website/tutorials.json` & `ax-platform-0.3.3/website/tutorials.json`

 * *Files 2% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.984375%*

 * *Differences: {"'Bayesian Optimization'": "{insert: [(7, OrderedDict([('id', 'gss'), ('title', 'Global Stopping "*

 * *                            "(Experiment-Level Early Stopping)')]))]}"}*

```diff
@@ -38,14 +38,18 @@
             "id": "saasbo_nehvi",
             "title": "Fully Bayesian, High-Dimensional, Multi-Objective Optimization"
         },
         {
             "dir": "early_stopping",
             "id": "early_stopping",
             "title": "Trial-Level Early Stopping"
+        },
+        {
+            "id": "gss",
+            "title": "Global Stopping (Experiment-Level Early Stopping)"
         }
     ],
     "Deep Dives": [
         {
             "id": "visualizations",
             "title": "Visualizations"
         },
```

