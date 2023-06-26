# Comparing `tmp/causal_testing_framework-4.1.0.tar.gz` & `tmp/causal_testing_framework-4.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "causal_testing_framework-4.1.0.tar", last modified: Wed May  3 14:59:03 2023, max compression
+gzip compressed data, was "causal_testing_framework-4.2.0.tar", last modified: Mon Jun 26 10:51:37 2023, max compression
```

## Comparing `causal_testing_framework-4.1.0.tar` & `causal_testing_framework-4.2.0.tar`

### file list

```diff
@@ -1,157 +1,163 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 14:59:03.705007 causal_testing_framework-4.1.0/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 14:59:03.677007 causal_testing_framework-4.1.0/.github/
--rw-r--r--   0 runner    (1001) docker     (123)     3489 2023-05-03 14:58:12.000000 causal_testing_framework-4.1.0/.github/CONTRIBUTING.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 14:59:03.677007 causal_testing_framework-4.1.0/.github/ISSUE_TEMPLATE/
--rw-r--r--   0 runner    (1001) docker     (123)      834 2023-05-03 14:58:12.000000 causal_testing_framework-4.1.0/.github/ISSUE_TEMPLATE/bug_report.md
--rw-r--r--   0 runner    (1001) docker     (123)      595 2023-05-03 14:58:12.000000 causal_testing_framework-4.1.0/.github/ISSUE_TEMPLATE/feature_request.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 14:59:03.677007 causal_testing_framework-4.1.0/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)     1136 2023-05-03 14:58:12.000000 causal_testing_framework-4.1.0/.github/workflows/ci-tests.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      752 2023-05-03 14:58:12.000000 causal_testing_framework-4.1.0/.github/workflows/lint-format.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      791 2023-05-03 14:58:12.000000 causal_testing_framework-4.1.0/.github/workflows/publish-to-pypi.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      681 2023-05-03 14:58:12.000000 causal_testing_framework-4.1.0/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)      276 2023-05-03 14:58:12.000000 causal_testing_framework-4.1.0/.mega-linter.yaml
--rw-r--r--   0 runner    (1001) docker     (123)    20375 2023-05-03 14:58:12.000000 causal_testing_framework-4.1.0/.pylintrc
--rw-r--r--   0 runner    (1001) docker     (123)      584 2023-05-03 14:58:12.000000 causal_testing_framework-4.1.0/.readthedocs.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     1084 2023-05-03 14:58:12.000000 causal_testing_framework-4.1.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     2297 2023-05-03 14:59:03.705007 causal_testing_framework-4.1.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1702 2023-05-03 14:58:12.000000 causal_testing_framework-4.1.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 14:59:03.677007 causal_testing_framework-4.1.0/causal_testing/
--rw-r--r--   0 runner    (1001) docker     (123)      221 2023-05-03 14:58:12.000000 causal_testing_framework-4.1.0/causal_testing/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 14:59:03.677007 causal_testing_framework-4.1.0/causal_testing/data_collection/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-03 14:58:12.000000 causal_testing_framework-4.1.0/causal_testing/data_collection/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6772 2023-05-03 14:58:12.000000 causal_testing_framework-4.1.0/causal_testing/data_collection/data_collector.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 14:59:03.677007 causal_testing_framework-4.1.0/causal_testing/generation/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-03 14:58:12.000000 causal_testing_framework-4.1.0/causal_testing/generation/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    12764 2023-05-03 14:58:12.000000 causal_testing_framework-4.1.0/causal_testing/generation/abstract_causal_test_case.py
--rw-r--r--   0 runner    (1001) docker     (123)     1387 2023-05-03 14:58:12.000000 causal_testing_framework-4.1.0/causal_testing/generation/enum_gen.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 14:59:03.677007 causal_testing_framework-4.1.0/causal_testing/json_front/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-03 14:58:12.000000 causal_testing_framework-4.1.0/causal_testing/json_front/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    18897 2023-05-03 14:58:12.000000 causal_testing_framework-4.1.0/causal_testing/json_front/json_class.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 14:59:03.681007 causal_testing_framework-4.1.0/causal_testing/specification/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-03 14:58:12.000000 causal_testing_framework-4.1.0/causal_testing/specification/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    26803 2023-05-03 14:58:12.000000 causal_testing_framework-4.1.0/causal_testing/specification/causal_dag.py
--rw-r--r--   0 runner    (1001) docker     (123)      680 2023-05-03 14:58:12.000000 causal_testing_framework-4.1.0/causal_testing/specification/causal_specification.py
--rw-r--r--   0 runner    (1001) docker     (123)    10510 2023-05-03 14:58:12.000000 causal_testing_framework-4.1.0/causal_testing/specification/metamorphic_relation.py
--rw-r--r--   0 runner    (1001) docker     (123)     5752 2023-05-03 14:58:12.000000 causal_testing_framework-4.1.0/causal_testing/specification/scenario.py
--rw-r--r--   0 runner    (1001) docker     (123)     9665 2023-05-03 14:58:12.000000 causal_testing_framework-4.1.0/causal_testing/specification/variable.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 14:59:03.681007 causal_testing_framework-4.1.0/causal_testing/testing/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-03 14:58:12.000000 causal_testing_framework-4.1.0/causal_testing/testing/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      785 2023-05-03 14:58:12.000000 causal_testing_framework-4.1.0/causal_testing/testing/base_test_case.py
--rw-r--r--   0 runner    (1001) docker     (123)     3782 2023-05-03 14:58:12.000000 causal_testing_framework-4.1.0/causal_testing/testing/causal_test_case.py
--rw-r--r--   0 runner    (1001) docker     (123)    13663 2023-05-03 14:58:12.000000 causal_testing_framework-4.1.0/causal_testing/testing/causal_test_engine.py
--rw-r--r--   0 runner    (1001) docker     (123)     3833 2023-05-03 14:58:12.000000 causal_testing_framework-4.1.0/causal_testing/testing/causal_test_outcome.py
--rw-r--r--   0 runner    (1001) docker     (123)     3950 2023-05-03 14:58:12.000000 causal_testing_framework-4.1.0/causal_testing/testing/causal_test_result.py
--rw-r--r--   0 runner    (1001) docker     (123)     2129 2023-05-03 14:58:12.000000 causal_testing_framework-4.1.0/causal_testing/testing/causal_test_suite.py
--rw-r--r--   0 runner    (1001) docker     (123)      229 2023-05-03 14:58:12.000000 causal_testing_framework-4.1.0/causal_testing/testing/effect.py
--rw-r--r--   0 runner    (1001) docker     (123)    30782 2023-05-03 14:58:12.000000 causal_testing_framework-4.1.0/causal_testing/testing/estimators.py
--rw-r--r--   0 runner    (1001) docker     (123)     1685 2023-05-03 14:58:12.000000 causal_testing_framework-4.1.0/causal_testing/testing/intervention.py
--rw-r--r--   0 runner    (1001) docker     (123)     2325 2023-05-03 14:58:12.000000 causal_testing_framework-4.1.0/causal_testing/testing/validation.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 14:59:03.681007 causal_testing_framework-4.1.0/causal_testing_framework.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     2297 2023-05-03 14:59:03.000000 causal_testing_framework-4.1.0/causal_testing_framework.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     4543 2023-05-03 14:59:03.000000 causal_testing_framework-4.1.0/causal_testing_framework.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-03 14:59:03.000000 causal_testing_framework-4.1.0/causal_testing_framework.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      271 2023-05-03 14:59:03.000000 causal_testing_framework-4.1.0/causal_testing_framework.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       53 2023-05-03 14:59:03.000000 causal_testing_framework-4.1.0/causal_testing_framework.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      301 2023-05-03 14:58:12.000000 causal_testing_framework-4.1.0/codecov.yml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 14:59:03.681007 causal_testing_framework-4.1.0/docs/
--rw-r--r--   0 runner    (1001) docker     (123)      638 2023-05-03 14:58:12.000000 causal_testing_framework-4.1.0/docs/Makefile
--rw-r--r--   0 runner    (1001) docker     (123)      775 2023-05-03 14:58:12.000000 causal_testing_framework-4.1.0/docs/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      804 2023-05-03 14:58:12.000000 causal_testing_framework-4.1.0/docs/make.bat
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 14:59:03.681007 causal_testing_framework-4.1.0/docs/source/
--rw-r--r--   0 runner    (1001) docker     (123)     2231 2023-05-03 14:58:12.000000 causal_testing_framework-4.1.0/docs/source/conf.py
--rw-r--r--   0 runner    (1001) docker     (123)     5424 2023-05-03 14:58:12.000000 causal_testing_framework-4.1.0/docs/source/description.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 14:59:03.681007 causal_testing_framework-4.1.0/docs/source/frontends/
--rw-r--r--   0 runner    (1001) docker     (123)     2985 2023-05-03 14:58:12.000000 causal_testing_framework-4.1.0/docs/source/frontends/json_front_end.rst
--rw-r--r--   0 runner    (1001) docker     (123)     1965 2023-05-03 14:58:12.000000 causal_testing_framework-4.1.0/docs/source/frontends/test_suite.rst
--rw-r--r--   0 runner    (1001) docker     (123)       16 2023-05-03 14:58:12.000000 causal_testing_framework-4.1.0/docs/source/glossary.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 14:59:03.681007 causal_testing_framework-4.1.0/docs/source/images/
--rw-r--r--   0 runner    (1001) docker     (123)   184134 2023-05-03 14:58:12.000000 causal_testing_framework-4.1.0/docs/source/images/workflow.png
--rw-r--r--   0 runner    (1001) docker     (123)     1531 2023-05-03 14:58:12.000000 causal_testing_framework-4.1.0/docs/source/index.rst
--rw-r--r--   0 runner    (1001) docker     (123)     1396 2023-05-03 14:58:12.000000 causal_testing_framework-4.1.0/docs/source/installation.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 14:59:03.681007 causal_testing_framework-4.1.0/docs/source/modules/
--rw-r--r--   0 runner    (1001) docker     (123)     3693 2023-05-03 14:58:12.000000 causal_testing_framework-4.1.0/docs/source/modules/causal_specification.rst
--rw-r--r--   0 runner    (1001) docker     (123)     5629 2023-05-03 14:58:12.000000 causal_testing_framework-4.1.0/docs/source/modules/causal_tests.rst
--rw-r--r--   0 runner    (1001) docker     (123)     1805 2023-05-03 14:58:12.000000 causal_testing_framework-4.1.0/docs/source/modules/data_collector.rst
--rw-r--r--   0 runner    (1001) docker     (123)       79 2023-05-03 14:58:12.000000 causal_testing_framework-4.1.0/docs/source/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)     6459 2023-05-03 14:58:12.000000 causal_testing_framework-4.1.0/docs/source/usage.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 14:59:03.685007 causal_testing_framework-4.1.0/examples/
--rw-r--r--   0 runner    (1001) docker     (123)       15 2023-05-03 14:58:12.000000 causal_testing_framework-4.1.0/examples/.gitignore
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 14:59:03.673007 causal_testing_framework-4.1.0/examples/covasim_/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 14:59:03.685007 causal_testing_framework-4.1.0/examples/covasim_/doubling_beta/
--rw-r--r--   0 runner    (1001) docker     (123)     1219 2023-05-03 14:58:12.000000 causal_testing_framework-4.1.0/examples/covasim_/doubling_beta/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      255 2023-05-03 14:58:12.000000 causal_testing_framework-4.1.0/examples/covasim_/doubling_beta/dag.dot
--rw-r--r--   0 runner    (1001) docker     (123)    24596 2023-05-03 14:58:12.000000 causal_testing_framework-4.1.0/examples/covasim_/doubling_beta/dag.png
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 14:59:03.685007 causal_testing_framework-4.1.0/examples/covasim_/doubling_beta/data/
--rw-r--r--   0 runner    (1001) docker     (123)  1355776 2023-05-03 14:58:12.000000 causal_testing_framework-4.1.0/examples/covasim_/doubling_beta/data/10k_observational_data.csv
--rw-r--r--   0 runner    (1001) docker     (123)    15718 2023-05-03 14:58:12.000000 causal_testing_framework-4.1.0/examples/covasim_/doubling_beta/example_beta.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 14:59:03.685007 causal_testing_framework-4.1.0/examples/covasim_/vaccinating_elderly/
--rw-r--r--   0 runner    (1001) docker     (123)     1820 2023-05-03 14:58:12.000000 causal_testing_framework-4.1.0/examples/covasim_/vaccinating_elderly/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      161 2023-05-03 14:58:12.000000 causal_testing_framework-4.1.0/examples/covasim_/vaccinating_elderly/dag.dot
--rw-r--r--   0 runner    (1001) docker     (123)    23290 2023-05-03 14:58:12.000000 causal_testing_framework-4.1.0/examples/covasim_/vaccinating_elderly/dag.png
--rw-r--r--   0 runner    (1001) docker     (123)    11845 2023-05-03 14:58:12.000000 causal_testing_framework-4.1.0/examples/covasim_/vaccinating_elderly/example_vaccine.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 14:59:03.685007 causal_testing_framework-4.1.0/examples/lr91/
--rw-r--r--   0 runner    (1001) docker     (123)     1658 2023-05-03 14:58:12.000000 causal_testing_framework-4.1.0/examples/lr91/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      561 2023-05-03 14:58:12.000000 causal_testing_framework-4.1.0/examples/lr91/dag.dot
--rw-r--r--   0 runner    (1001) docker     (123)    73886 2023-05-03 14:58:12.000000 causal_testing_framework-4.1.0/examples/lr91/dag.png
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 14:59:03.685007 causal_testing_framework-4.1.0/examples/lr91/data/
--rw-r--r--   0 runner    (1001) docker     (123)    40715 2023-05-03 14:58:12.000000 causal_testing_framework-4.1.0/examples/lr91/data/normalised_results.csv
--rw-r--r--   0 runner    (1001) docker     (123)    40686 2023-05-03 14:58:12.000000 causal_testing_framework-4.1.0/examples/lr91/data/results.csv
--rw-r--r--   0 runner    (1001) docker     (123)     8827 2023-05-03 14:58:12.000000 causal_testing_framework-4.1.0/examples/lr91/example_max_conductances.py
--rw-r--r--   0 runner    (1001) docker     (123)     8582 2023-05-03 14:58:12.000000 causal_testing_framework-4.1.0/examples/lr91/example_max_conductances_test_suite.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 14:59:03.693007 causal_testing_framework-4.1.0/examples/poisson/
--rw-r--r--   0 runner    (1001) docker     (123)      826 2023-05-03 14:58:12.000000 causal_testing_framework-4.1.0/examples/poisson/README.md
--rw-r--r--   0 runner    (1001) docker     (123)     7603 2023-05-03 14:58:12.000000 causal_testing_framework-4.1.0/examples/poisson/causal_tests.json
--rw-r--r--   0 runner    (1001) docker     (123)      518 2023-05-03 14:58:12.000000 causal_testing_framework-4.1.0/examples/poisson/dag.dot
--rw-r--r--   0 runner    (1001) docker     (123)    61017 2023-05-03 14:58:12.000000 causal_testing_framework-4.1.0/examples/poisson/data.csv
--rw-r--r--   0 runner    (1001) docker     (123)     7314 2023-05-03 14:58:12.000000 causal_testing_framework-4.1.0/examples/poisson/example_run_causal_tests.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 14:59:03.693007 causal_testing_framework-4.1.0/examples/poisson-line-process/
--rw-r--r--   0 runner    (1001) docker     (123)       86 2023-05-03 14:58:12.000000 causal_testing_framework-4.1.0/examples/poisson-line-process/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)     1062 2023-05-03 14:58:12.000000 causal_testing_framework-4.1.0/examples/poisson-line-process/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      404 2023-05-03 14:58:12.000000 causal_testing_framework-4.1.0/examples/poisson-line-process/dag.dot
--rw-r--r--   0 runner    (1001) docker     (123)    53765 2023-05-03 14:58:12.000000 causal_testing_framework-4.1.0/examples/poisson-line-process/dag.png
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 14:59:03.673007 causal_testing_framework-4.1.0/examples/poisson-line-process/data/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 14:59:03.693007 causal_testing_framework-4.1.0/examples/poisson-line-process/data/random/
--rw-r--r--   0 runner    (1001) docker     (123)   102007 2023-05-03 14:58:12.000000 causal_testing_framework-4.1.0/examples/poisson-line-process/data/random/data_random_1000.csv
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 14:59:03.697007 causal_testing_framework-4.1.0/examples/poisson-line-process/data/smt_100/
--rw-r--r--   0 runner    (1001) docker     (123)    15080 2023-05-03 14:58:12.000000 causal_testing_framework-4.1.0/examples/poisson-line-process/data/smt_100/data_smt_wh10_100.csv
--rw-r--r--   0 runner    (1001) docker     (123)    12100 2023-05-03 14:58:12.000000 causal_testing_framework-4.1.0/examples/poisson-line-process/data/smt_100/data_smt_wh1_100.csv
--rw-r--r--   0 runner    (1001) docker     (123)    12945 2023-05-03 14:58:12.000000 causal_testing_framework-4.1.0/examples/poisson-line-process/data/smt_100/data_smt_wh2_100.csv
--rw-r--r--   0 runner    (1001) docker     (123)    24851 2023-05-03 14:58:12.000000 causal_testing_framework-4.1.0/examples/poisson-line-process/data/smt_100/data_smt_wh3_100.csv
--rw-r--r--   0 runner    (1001) docker     (123)    14925 2023-05-03 14:58:12.000000 causal_testing_framework-4.1.0/examples/poisson-line-process/data/smt_100/data_smt_wh4_100.csv
--rw-r--r--   0 runner    (1001) docker     (123)    13682 2023-05-03 14:58:12.000000 causal_testing_framework-4.1.0/examples/poisson-line-process/data/smt_100/data_smt_wh5_100.csv
--rw-r--r--   0 runner    (1001) docker     (123)    25451 2023-05-03 14:58:12.000000 causal_testing_framework-4.1.0/examples/poisson-line-process/data/smt_100/data_smt_wh6_100.csv
--rw-r--r--   0 runner    (1001) docker     (123)    26544 2023-05-03 14:58:12.000000 causal_testing_framework-4.1.0/examples/poisson-line-process/data/smt_100/data_smt_wh7_100.csv
--rw-r--r--   0 runner    (1001) docker     (123)    17103 2023-05-03 14:58:12.000000 causal_testing_framework-4.1.0/examples/poisson-line-process/data/smt_100/data_smt_wh8_100.csv
--rw-r--r--   0 runner    (1001) docker     (123)    26889 2023-05-03 14:58:12.000000 causal_testing_framework-4.1.0/examples/poisson-line-process/data/smt_100/data_smt_wh9_100.csv
--rw-r--r--   0 runner    (1001) docker     (123)     9104 2023-05-03 14:58:12.000000 causal_testing_framework-4.1.0/examples/poisson-line-process/example_poisson_process.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 14:59:03.697007 causal_testing_framework-4.1.0/images/
--rw-r--r--   0 runner    (1001) docker     (123)   184134 2023-05-03 14:58:12.000000 causal_testing_framework-4.1.0/images/workflow.png
--rw-r--r--   0 runner    (1001) docker     (123)     1579 2023-05-03 14:58:12.000000 causal_testing_framework-4.1.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-03 14:59:03.705007 causal_testing_framework-4.1.0/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 14:59:03.697007 causal_testing_framework-4.1.0/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-03 14:58:12.000000 causal_testing_framework-4.1.0/tests/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 14:59:03.697007 causal_testing_framework-4.1.0/tests/data/
--rw-r--r--   0 runner    (1001) docker     (123)   374288 2023-05-03 14:58:12.000000 causal_testing_framework-4.1.0/tests/data/nhefs.csv
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 14:59:03.697007 causal_testing_framework-4.1.0/tests/data_collection_tests/
--rw-r--r--   0 runner    (1001) docker     (123)     3322 2023-05-03 14:58:12.000000 causal_testing_framework-4.1.0/tests/data_collection_tests/test_observational_data_collector.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 14:59:03.697007 causal_testing_framework-4.1.0/tests/generation_tests/
--rw-r--r--   0 runner    (1001) docker     (123)     8842 2023-05-03 14:58:12.000000 causal_testing_framework-4.1.0/tests/generation_tests/test_abstract_test_case.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 14:59:03.701007 causal_testing_framework-4.1.0/tests/json_front_tests/
--rw-r--r--   0 runner    (1001) docker     (123)    10798 2023-05-03 14:58:12.000000 causal_testing_framework-4.1.0/tests/json_front_tests/test_json_class.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 14:59:03.677007 causal_testing_framework-4.1.0/tests/resources/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 14:59:03.701007 causal_testing_framework-4.1.0/tests/resources/data/
--rw-r--r--   0 runner    (1001) docker     (123)      102 2023-05-03 14:58:12.000000 causal_testing_framework-4.1.0/tests/resources/data/dag.dot
--rw-r--r--   0 runner    (1001) docker     (123)       56 2023-05-03 14:58:12.000000 causal_testing_framework-4.1.0/tests/resources/data/data.csv
--rw-r--r--   0 runner    (1001) docker     (123)       68 2023-05-03 14:58:12.000000 causal_testing_framework-4.1.0/tests/resources/data/data_with_meta.csv
--rw-r--r--   0 runner    (1001) docker     (123)      151 2023-05-03 14:58:12.000000 causal_testing_framework-4.1.0/tests/resources/data/tests.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 14:59:03.701007 causal_testing_framework-4.1.0/tests/specification_tests/
--rw-r--r--   0 runner    (1001) docker     (123)    17967 2023-05-03 14:58:12.000000 causal_testing_framework-4.1.0/tests/specification_tests/test_causal_dag.py
--rw-r--r--   0 runner    (1001) docker     (123)    13719 2023-05-03 14:58:12.000000 causal_testing_framework-4.1.0/tests/specification_tests/test_metamorphic_relations.py
--rw-r--r--   0 runner    (1001) docker     (123)     5819 2023-05-03 14:58:12.000000 causal_testing_framework-4.1.0/tests/specification_tests/test_variable.py
--rw-r--r--   0 runner    (1001) docker     (123)      997 2023-05-03 14:58:12.000000 causal_testing_framework-4.1.0/tests/test_helpers.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 14:59:03.705007 causal_testing_framework-4.1.0/tests/testing_tests/
--rw-r--r--   0 runner    (1001) docker     (123)     2005 2023-05-03 14:58:12.000000 causal_testing_framework-4.1.0/tests/testing_tests/test_causal_test_case.py
--rw-r--r--   0 runner    (1001) docker     (123)    13873 2023-05-03 14:58:12.000000 causal_testing_framework-4.1.0/tests/testing_tests/test_causal_test_engine.py
--rw-r--r--   0 runner    (1001) docker     (123)     9100 2023-05-03 14:58:12.000000 causal_testing_framework-4.1.0/tests/testing_tests/test_causal_test_outcome.py
--rw-r--r--   0 runner    (1001) docker     (123)     6275 2023-05-03 14:58:12.000000 causal_testing_framework-4.1.0/tests/testing_tests/test_causal_test_suite.py
--rw-r--r--   0 runner    (1001) docker     (123)    18696 2023-05-03 14:58:12.000000 causal_testing_framework-4.1.0/tests/testing_tests/test_estimators.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 10:51:37.001812 causal_testing_framework-4.2.0/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 10:51:36.985812 causal_testing_framework-4.2.0/.github/
+-rw-r--r--   0 runner    (1001) docker     (123)     3489 2023-06-26 10:50:35.000000 causal_testing_framework-4.2.0/.github/CONTRIBUTING.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 10:51:36.985812 causal_testing_framework-4.2.0/.github/ISSUE_TEMPLATE/
+-rw-r--r--   0 runner    (1001) docker     (123)      834 2023-06-26 10:50:35.000000 causal_testing_framework-4.2.0/.github/ISSUE_TEMPLATE/bug_report.md
+-rw-r--r--   0 runner    (1001) docker     (123)      595 2023-06-26 10:50:35.000000 causal_testing_framework-4.2.0/.github/ISSUE_TEMPLATE/feature_request.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 10:51:36.985812 causal_testing_framework-4.2.0/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)     1151 2023-06-26 10:50:35.000000 causal_testing_framework-4.2.0/.github/workflows/ci-tests.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      752 2023-06-26 10:50:35.000000 causal_testing_framework-4.2.0/.github/workflows/lint-format.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      791 2023-06-26 10:50:35.000000 causal_testing_framework-4.2.0/.github/workflows/publish-to-pypi.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      681 2023-06-26 10:50:35.000000 causal_testing_framework-4.2.0/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)      276 2023-06-26 10:50:35.000000 causal_testing_framework-4.2.0/.mega-linter.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)    20375 2023-06-26 10:50:35.000000 causal_testing_framework-4.2.0/.pylintrc
+-rw-r--r--   0 runner    (1001) docker     (123)      584 2023-06-26 10:50:35.000000 causal_testing_framework-4.2.0/.readthedocs.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     1084 2023-06-26 10:50:35.000000 causal_testing_framework-4.2.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     2297 2023-06-26 10:51:37.001812 causal_testing_framework-4.2.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1702 2023-06-26 10:50:35.000000 causal_testing_framework-4.2.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 10:51:36.985812 causal_testing_framework-4.2.0/causal_testing/
+-rw-r--r--   0 runner    (1001) docker     (123)      221 2023-06-26 10:50:35.000000 causal_testing_framework-4.2.0/causal_testing/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 10:51:36.985812 causal_testing_framework-4.2.0/causal_testing/data_collection/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-26 10:50:35.000000 causal_testing_framework-4.2.0/causal_testing/data_collection/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6772 2023-06-26 10:50:35.000000 causal_testing_framework-4.2.0/causal_testing/data_collection/data_collector.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 10:51:36.985812 causal_testing_framework-4.2.0/causal_testing/generation/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-26 10:50:35.000000 causal_testing_framework-4.2.0/causal_testing/generation/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12764 2023-06-26 10:50:35.000000 causal_testing_framework-4.2.0/causal_testing/generation/abstract_causal_test_case.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1387 2023-06-26 10:50:35.000000 causal_testing_framework-4.2.0/causal_testing/generation/enum_gen.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 10:51:36.985812 causal_testing_framework-4.2.0/causal_testing/json_front/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-26 10:50:35.000000 causal_testing_framework-4.2.0/causal_testing/json_front/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19090 2023-06-26 10:50:35.000000 causal_testing_framework-4.2.0/causal_testing/json_front/json_class.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 10:51:36.985812 causal_testing_framework-4.2.0/causal_testing/specification/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-26 10:50:35.000000 causal_testing_framework-4.2.0/causal_testing/specification/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    26803 2023-06-26 10:50:35.000000 causal_testing_framework-4.2.0/causal_testing/specification/causal_dag.py
+-rw-r--r--   0 runner    (1001) docker     (123)      680 2023-06-26 10:50:35.000000 causal_testing_framework-4.2.0/causal_testing/specification/causal_specification.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11932 2023-06-26 10:50:35.000000 causal_testing_framework-4.2.0/causal_testing/specification/metamorphic_relation.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5752 2023-06-26 10:50:35.000000 causal_testing_framework-4.2.0/causal_testing/specification/scenario.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9665 2023-06-26 10:50:35.000000 causal_testing_framework-4.2.0/causal_testing/specification/variable.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 10:51:36.989812 causal_testing_framework-4.2.0/causal_testing/testing/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-26 10:50:35.000000 causal_testing_framework-4.2.0/causal_testing/testing/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      785 2023-06-26 10:50:35.000000 causal_testing_framework-4.2.0/causal_testing/testing/base_test_case.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3782 2023-06-26 10:50:35.000000 causal_testing_framework-4.2.0/causal_testing/testing/causal_test_case.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13464 2023-06-26 10:50:35.000000 causal_testing_framework-4.2.0/causal_testing/testing/causal_test_engine.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4792 2023-06-26 10:50:35.000000 causal_testing_framework-4.2.0/causal_testing/testing/causal_test_outcome.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4276 2023-06-26 10:50:35.000000 causal_testing_framework-4.2.0/causal_testing/testing/causal_test_result.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2129 2023-06-26 10:50:35.000000 causal_testing_framework-4.2.0/causal_testing/testing/causal_test_suite.py
+-rw-r--r--   0 runner    (1001) docker     (123)      229 2023-06-26 10:50:35.000000 causal_testing_framework-4.2.0/causal_testing/testing/effect.py
+-rw-r--r--   0 runner    (1001) docker     (123)    29468 2023-06-26 10:50:35.000000 causal_testing_framework-4.2.0/causal_testing/testing/estimators.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1685 2023-06-26 10:50:35.000000 causal_testing_framework-4.2.0/causal_testing/testing/intervention.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 10:51:36.989812 causal_testing_framework-4.2.0/causal_testing/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-26 10:50:35.000000 causal_testing_framework-4.2.0/causal_testing/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2361 2023-06-26 10:50:35.000000 causal_testing_framework-4.2.0/causal_testing/utils/validation.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 10:51:36.989812 causal_testing_framework-4.2.0/causal_testing_framework.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     2297 2023-06-26 10:51:36.000000 causal_testing_framework-4.2.0/causal_testing_framework.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     4685 2023-06-26 10:51:36.000000 causal_testing_framework-4.2.0/causal_testing_framework.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-26 10:51:36.000000 causal_testing_framework-4.2.0/causal_testing_framework.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      273 2023-06-26 10:51:36.000000 causal_testing_framework-4.2.0/causal_testing_framework.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       53 2023-06-26 10:51:36.000000 causal_testing_framework-4.2.0/causal_testing_framework.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      301 2023-06-26 10:50:35.000000 causal_testing_framework-4.2.0/codecov.yml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 10:51:36.989812 causal_testing_framework-4.2.0/docs/
+-rw-r--r--   0 runner    (1001) docker     (123)      638 2023-06-26 10:50:35.000000 causal_testing_framework-4.2.0/docs/Makefile
+-rw-r--r--   0 runner    (1001) docker     (123)      775 2023-06-26 10:50:35.000000 causal_testing_framework-4.2.0/docs/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      804 2023-06-26 10:50:35.000000 causal_testing_framework-4.2.0/docs/make.bat
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 10:51:36.989812 causal_testing_framework-4.2.0/docs/source/
+-rw-r--r--   0 runner    (1001) docker     (123)     2231 2023-06-26 10:50:35.000000 causal_testing_framework-4.2.0/docs/source/conf.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5424 2023-06-26 10:50:35.000000 causal_testing_framework-4.2.0/docs/source/description.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 10:51:36.989812 causal_testing_framework-4.2.0/docs/source/dev/
+-rw-r--r--   0 runner    (1001) docker     (123)      858 2023-06-26 10:50:35.000000 causal_testing_framework-4.2.0/docs/source/dev/actions_and_webhooks.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     2397 2023-06-26 10:50:35.000000 causal_testing_framework-4.2.0/docs/source/dev/documentation.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1619 2023-06-26 10:50:35.000000 causal_testing_framework-4.2.0/docs/source/dev/version_release.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 10:51:36.989812 causal_testing_framework-4.2.0/docs/source/frontends/
+-rw-r--r--   0 runner    (1001) docker     (123)     4247 2023-06-26 10:50:35.000000 causal_testing_framework-4.2.0/docs/source/frontends/json_front_end.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1965 2023-06-26 10:50:35.000000 causal_testing_framework-4.2.0/docs/source/frontends/test_suite.rst
+-rw-r--r--   0 runner    (1001) docker     (123)       16 2023-06-26 10:50:35.000000 causal_testing_framework-4.2.0/docs/source/glossary.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 10:51:36.989812 causal_testing_framework-4.2.0/docs/source/images/
+-rw-r--r--   0 runner    (1001) docker     (123)   184134 2023-06-26 10:50:35.000000 causal_testing_framework-4.2.0/docs/source/images/workflow.png
+-rw-r--r--   0 runner    (1001) docker     (123)     1676 2023-06-26 10:50:35.000000 causal_testing_framework-4.2.0/docs/source/index.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1396 2023-06-26 10:50:35.000000 causal_testing_framework-4.2.0/docs/source/installation.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 10:51:36.989812 causal_testing_framework-4.2.0/docs/source/modules/
+-rw-r--r--   0 runner    (1001) docker     (123)     3693 2023-06-26 10:50:35.000000 causal_testing_framework-4.2.0/docs/source/modules/causal_specification.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     5629 2023-06-26 10:50:35.000000 causal_testing_framework-4.2.0/docs/source/modules/causal_tests.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1805 2023-06-26 10:50:35.000000 causal_testing_framework-4.2.0/docs/source/modules/data_collector.rst
+-rw-r--r--   0 runner    (1001) docker     (123)       79 2023-06-26 10:50:35.000000 causal_testing_framework-4.2.0/docs/source/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     6429 2023-06-26 10:50:35.000000 causal_testing_framework-4.2.0/docs/source/usage.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 10:51:36.989812 causal_testing_framework-4.2.0/examples/
+-rw-r--r--   0 runner    (1001) docker     (123)       15 2023-06-26 10:50:35.000000 causal_testing_framework-4.2.0/examples/.gitignore
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 10:51:36.981812 causal_testing_framework-4.2.0/examples/covasim_/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 10:51:36.993812 causal_testing_framework-4.2.0/examples/covasim_/doubling_beta/
+-rw-r--r--   0 runner    (1001) docker     (123)     1219 2023-06-26 10:50:35.000000 causal_testing_framework-4.2.0/examples/covasim_/doubling_beta/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      255 2023-06-26 10:50:35.000000 causal_testing_framework-4.2.0/examples/covasim_/doubling_beta/dag.dot
+-rw-r--r--   0 runner    (1001) docker     (123)    24596 2023-06-26 10:50:35.000000 causal_testing_framework-4.2.0/examples/covasim_/doubling_beta/dag.png
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 10:51:36.993812 causal_testing_framework-4.2.0/examples/covasim_/doubling_beta/data/
+-rw-r--r--   0 runner    (1001) docker     (123)  1355776 2023-06-26 10:50:35.000000 causal_testing_framework-4.2.0/examples/covasim_/doubling_beta/data/10k_observational_data.csv
+-rw-r--r--   0 runner    (1001) docker     (123)    15697 2023-06-26 10:50:35.000000 causal_testing_framework-4.2.0/examples/covasim_/doubling_beta/example_beta.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 10:51:36.993812 causal_testing_framework-4.2.0/examples/covasim_/vaccinating_elderly/
+-rw-r--r--   0 runner    (1001) docker     (123)     1820 2023-06-26 10:50:35.000000 causal_testing_framework-4.2.0/examples/covasim_/vaccinating_elderly/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      161 2023-06-26 10:50:35.000000 causal_testing_framework-4.2.0/examples/covasim_/vaccinating_elderly/dag.dot
+-rw-r--r--   0 runner    (1001) docker     (123)    23290 2023-06-26 10:50:35.000000 causal_testing_framework-4.2.0/examples/covasim_/vaccinating_elderly/dag.png
+-rw-r--r--   0 runner    (1001) docker     (123)    11838 2023-06-26 10:50:35.000000 causal_testing_framework-4.2.0/examples/covasim_/vaccinating_elderly/example_vaccine.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 10:51:36.993812 causal_testing_framework-4.2.0/examples/lr91/
+-rw-r--r--   0 runner    (1001) docker     (123)     1658 2023-06-26 10:50:35.000000 causal_testing_framework-4.2.0/examples/lr91/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      561 2023-06-26 10:50:35.000000 causal_testing_framework-4.2.0/examples/lr91/dag.dot
+-rw-r--r--   0 runner    (1001) docker     (123)    73886 2023-06-26 10:50:35.000000 causal_testing_framework-4.2.0/examples/lr91/dag.png
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 10:51:36.993812 causal_testing_framework-4.2.0/examples/lr91/data/
+-rw-r--r--   0 runner    (1001) docker     (123)    40715 2023-06-26 10:50:35.000000 causal_testing_framework-4.2.0/examples/lr91/data/normalised_results.csv
+-rw-r--r--   0 runner    (1001) docker     (123)    40686 2023-06-26 10:50:35.000000 causal_testing_framework-4.2.0/examples/lr91/data/results.csv
+-rw-r--r--   0 runner    (1001) docker     (123)     8820 2023-06-26 10:50:35.000000 causal_testing_framework-4.2.0/examples/lr91/example_max_conductances.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8582 2023-06-26 10:50:35.000000 causal_testing_framework-4.2.0/examples/lr91/example_max_conductances_test_suite.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 10:51:36.993812 causal_testing_framework-4.2.0/examples/poisson/
+-rw-r--r--   0 runner    (1001) docker     (123)      826 2023-06-26 10:50:35.000000 causal_testing_framework-4.2.0/examples/poisson/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)     7603 2023-06-26 10:50:35.000000 causal_testing_framework-4.2.0/examples/poisson/causal_tests.json
+-rw-r--r--   0 runner    (1001) docker     (123)      518 2023-06-26 10:50:35.000000 causal_testing_framework-4.2.0/examples/poisson/dag.dot
+-rw-r--r--   0 runner    (1001) docker     (123)    61017 2023-06-26 10:50:35.000000 causal_testing_framework-4.2.0/examples/poisson/data.csv
+-rw-r--r--   0 runner    (1001) docker     (123)     7307 2023-06-26 10:50:35.000000 causal_testing_framework-4.2.0/examples/poisson/example_run_causal_tests.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 10:51:36.997812 causal_testing_framework-4.2.0/examples/poisson-line-process/
+-rw-r--r--   0 runner    (1001) docker     (123)       86 2023-06-26 10:50:35.000000 causal_testing_framework-4.2.0/examples/poisson-line-process/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)     1062 2023-06-26 10:50:35.000000 causal_testing_framework-4.2.0/examples/poisson-line-process/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      404 2023-06-26 10:50:35.000000 causal_testing_framework-4.2.0/examples/poisson-line-process/dag.dot
+-rw-r--r--   0 runner    (1001) docker     (123)    53765 2023-06-26 10:50:35.000000 causal_testing_framework-4.2.0/examples/poisson-line-process/dag.png
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 10:51:36.981812 causal_testing_framework-4.2.0/examples/poisson-line-process/data/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 10:51:36.997812 causal_testing_framework-4.2.0/examples/poisson-line-process/data/random/
+-rw-r--r--   0 runner    (1001) docker     (123)   102007 2023-06-26 10:50:35.000000 causal_testing_framework-4.2.0/examples/poisson-line-process/data/random/data_random_1000.csv
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 10:51:36.997812 causal_testing_framework-4.2.0/examples/poisson-line-process/data/smt_100/
+-rw-r--r--   0 runner    (1001) docker     (123)    15080 2023-06-26 10:50:35.000000 causal_testing_framework-4.2.0/examples/poisson-line-process/data/smt_100/data_smt_wh10_100.csv
+-rw-r--r--   0 runner    (1001) docker     (123)    12100 2023-06-26 10:50:35.000000 causal_testing_framework-4.2.0/examples/poisson-line-process/data/smt_100/data_smt_wh1_100.csv
+-rw-r--r--   0 runner    (1001) docker     (123)    12945 2023-06-26 10:50:35.000000 causal_testing_framework-4.2.0/examples/poisson-line-process/data/smt_100/data_smt_wh2_100.csv
+-rw-r--r--   0 runner    (1001) docker     (123)    24851 2023-06-26 10:50:35.000000 causal_testing_framework-4.2.0/examples/poisson-line-process/data/smt_100/data_smt_wh3_100.csv
+-rw-r--r--   0 runner    (1001) docker     (123)    14925 2023-06-26 10:50:35.000000 causal_testing_framework-4.2.0/examples/poisson-line-process/data/smt_100/data_smt_wh4_100.csv
+-rw-r--r--   0 runner    (1001) docker     (123)    13682 2023-06-26 10:50:35.000000 causal_testing_framework-4.2.0/examples/poisson-line-process/data/smt_100/data_smt_wh5_100.csv
+-rw-r--r--   0 runner    (1001) docker     (123)    25451 2023-06-26 10:50:35.000000 causal_testing_framework-4.2.0/examples/poisson-line-process/data/smt_100/data_smt_wh6_100.csv
+-rw-r--r--   0 runner    (1001) docker     (123)    26544 2023-06-26 10:50:35.000000 causal_testing_framework-4.2.0/examples/poisson-line-process/data/smt_100/data_smt_wh7_100.csv
+-rw-r--r--   0 runner    (1001) docker     (123)    17103 2023-06-26 10:50:35.000000 causal_testing_framework-4.2.0/examples/poisson-line-process/data/smt_100/data_smt_wh8_100.csv
+-rw-r--r--   0 runner    (1001) docker     (123)    26889 2023-06-26 10:50:35.000000 causal_testing_framework-4.2.0/examples/poisson-line-process/data/smt_100/data_smt_wh9_100.csv
+-rw-r--r--   0 runner    (1001) docker     (123)     9067 2023-06-26 10:50:35.000000 causal_testing_framework-4.2.0/examples/poisson-line-process/example_poisson_process.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 10:51:36.997812 causal_testing_framework-4.2.0/images/
+-rw-r--r--   0 runner    (1001) docker     (123)   184134 2023-06-26 10:50:35.000000 causal_testing_framework-4.2.0/images/workflow.png
+-rw-r--r--   0 runner    (1001) docker     (123)     1580 2023-06-26 10:50:35.000000 causal_testing_framework-4.2.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-26 10:51:37.001812 causal_testing_framework-4.2.0/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 10:51:36.997812 causal_testing_framework-4.2.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-26 10:50:35.000000 causal_testing_framework-4.2.0/tests/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 10:51:36.997812 causal_testing_framework-4.2.0/tests/data/
+-rw-r--r--   0 runner    (1001) docker     (123)   374288 2023-06-26 10:50:35.000000 causal_testing_framework-4.2.0/tests/data/nhefs.csv
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 10:51:36.997812 causal_testing_framework-4.2.0/tests/data_collection_tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     3322 2023-06-26 10:50:35.000000 causal_testing_framework-4.2.0/tests/data_collection_tests/test_observational_data_collector.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 10:51:36.997812 causal_testing_framework-4.2.0/tests/generation_tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     8842 2023-06-26 10:50:35.000000 causal_testing_framework-4.2.0/tests/generation_tests/test_abstract_test_case.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 10:51:36.997812 causal_testing_framework-4.2.0/tests/json_front_tests/
+-rw-r--r--   0 runner    (1001) docker     (123)    11837 2023-06-26 10:50:35.000000 causal_testing_framework-4.2.0/tests/json_front_tests/test_json_class.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 10:51:36.985812 causal_testing_framework-4.2.0/tests/resources/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 10:51:36.997812 causal_testing_framework-4.2.0/tests/resources/data/
+-rw-r--r--   0 runner    (1001) docker     (123)      102 2023-06-26 10:50:35.000000 causal_testing_framework-4.2.0/tests/resources/data/dag.dot
+-rw-r--r--   0 runner    (1001) docker     (123)       56 2023-06-26 10:50:35.000000 causal_testing_framework-4.2.0/tests/resources/data/data.csv
+-rw-r--r--   0 runner    (1001) docker     (123)       68 2023-06-26 10:50:35.000000 causal_testing_framework-4.2.0/tests/resources/data/data_with_meta.csv
+-rw-r--r--   0 runner    (1001) docker     (123)      151 2023-06-26 10:50:35.000000 causal_testing_framework-4.2.0/tests/resources/data/tests.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 10:51:37.001812 causal_testing_framework-4.2.0/tests/specification_tests/
+-rw-r--r--   0 runner    (1001) docker     (123)    17967 2023-06-26 10:50:35.000000 causal_testing_framework-4.2.0/tests/specification_tests/test_causal_dag.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13830 2023-06-26 10:50:35.000000 causal_testing_framework-4.2.0/tests/specification_tests/test_metamorphic_relations.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5819 2023-06-26 10:50:35.000000 causal_testing_framework-4.2.0/tests/specification_tests/test_variable.py
+-rw-r--r--   0 runner    (1001) docker     (123)      997 2023-06-26 10:50:35.000000 causal_testing_framework-4.2.0/tests/test_helpers.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 10:51:37.001812 causal_testing_framework-4.2.0/tests/testing_tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     2005 2023-06-26 10:50:35.000000 causal_testing_framework-4.2.0/tests/testing_tests/test_causal_test_case.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13931 2023-06-26 10:50:35.000000 causal_testing_framework-4.2.0/tests/testing_tests/test_causal_test_engine.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10472 2023-06-26 10:50:35.000000 causal_testing_framework-4.2.0/tests/testing_tests/test_causal_test_outcome.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6275 2023-06-26 10:50:35.000000 causal_testing_framework-4.2.0/tests/testing_tests/test_causal_test_suite.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19217 2023-06-26 10:50:35.000000 causal_testing_framework-4.2.0/tests/testing_tests/test_estimators.py
```

### Comparing `causal_testing_framework-4.1.0/.github/CONTRIBUTING.md` & `causal_testing_framework-4.2.0/.github/CONTRIBUTING.md`

 * *Files identical despite different names*

### Comparing `causal_testing_framework-4.1.0/.github/ISSUE_TEMPLATE/bug_report.md` & `causal_testing_framework-4.2.0/.github/ISSUE_TEMPLATE/bug_report.md`

 * *Files identical despite different names*

### Comparing `causal_testing_framework-4.1.0/.github/ISSUE_TEMPLATE/feature_request.md` & `causal_testing_framework-4.2.0/.github/ISSUE_TEMPLATE/feature_request.md`

 * *Files identical despite different names*

### Comparing `causal_testing_framework-4.1.0/.github/workflows/ci-tests.yaml` & `causal_testing_framework-4.2.0/.github/workflows/ci-tests.yaml`

 * *Files 2% similar despite different names*

```diff
@@ -20,15 +20,15 @@
         with:
           auto-update-conda: true
           python-version: ${{ matrix.python-version }}
       - name: Install package and dependencies
         run: |
           conda install -c conda-forge pygraphviz
           python --version
-          pip install -e .
+          pip install -e . --no-cache-dir
           pip install -e .[test]
           pip install pytest pytest-cov
         shell: bash -l {0}
       - name: Test with pytest
         run: |
           pytest --cov=causal_testing --cov-report=xml
         shell: bash -l {0}
```

### Comparing `causal_testing_framework-4.1.0/.github/workflows/lint-format.yaml` & `causal_testing_framework-4.2.0/.github/workflows/lint-format.yaml`

 * *Files identical despite different names*

### Comparing `causal_testing_framework-4.1.0/.github/workflows/publish-to-pypi.yaml` & `causal_testing_framework-4.2.0/.github/workflows/publish-to-pypi.yaml`

 * *Files identical despite different names*

### Comparing `causal_testing_framework-4.1.0/.gitignore` & `causal_testing_framework-4.2.0/.gitignore`

 * *Files identical despite different names*

### Comparing `causal_testing_framework-4.1.0/.pylintrc` & `causal_testing_framework-4.2.0/.pylintrc`

 * *Files identical despite different names*

### Comparing `causal_testing_framework-4.1.0/.readthedocs.yaml` & `causal_testing_framework-4.2.0/.readthedocs.yaml`

 * *Files identical despite different names*

### Comparing `causal_testing_framework-4.1.0/LICENSE` & `causal_testing_framework-4.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `causal_testing_framework-4.1.0/PKG-INFO` & `causal_testing_framework-4.2.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: causal_testing_framework
-Version: 4.1.0
+Version: 4.2.0
 Summary: A framework for causal testing using causal directed acyclic graphs.
 Author: The CITCOM team
 License: MIT
 Project-URL: Bug_Tracker, https://github.com/CITCOM-project/CausalTestingFramework/issues
 Project-URL: Documentation, https://causal-testing-framework.readthedocs.io/
 Project-URL: Source, https://github.com/CITCOM-project/CausalTestingFramework
 Keywords: causal inference,verification
```

### Comparing `causal_testing_framework-4.1.0/README.md` & `causal_testing_framework-4.2.0/README.md`

 * *Files identical despite different names*

### Comparing `causal_testing_framework-4.1.0/causal_testing/data_collection/data_collector.py` & `causal_testing_framework-4.2.0/causal_testing/data_collection/data_collector.py`

 * *Files identical despite different names*

### Comparing `causal_testing_framework-4.1.0/causal_testing/generation/abstract_causal_test_case.py` & `causal_testing_framework-4.2.0/causal_testing/generation/abstract_causal_test_case.py`

 * *Files identical despite different names*

### Comparing `causal_testing_framework-4.1.0/causal_testing/generation/enum_gen.py` & `causal_testing_framework-4.2.0/causal_testing/generation/enum_gen.py`

 * *Files identical despite different names*

### Comparing `causal_testing_framework-4.1.0/causal_testing/json_front/json_class.py` & `causal_testing_framework-4.2.0/causal_testing/json_front/json_class.py`

 * *Files 5% similar despite different names*

```diff
@@ -52,32 +52,44 @@
         self.data = []
         self.test_plan = None
         self.scenario = None
         self.causal_specification = None
         self.output_path = Path(output_path)
         self.check_file_exists(self.output_path, output_overwrite)
 
-    def set_paths(self, json_path: str, dag_path: str, data_paths: str):
+    def set_paths(self, json_path: str, dag_path: str, data_paths: list[str] = None):
         """
         Takes a path of the directory containing all scenario specific files and creates individual paths for each file
         :param json_path: string path representation to .json file containing test specifications
         :param dag_path: string path representation to the .dot file containing the Causal DAG
         :param data_paths: string path representation to the data files
         """
+        if data_paths is None:
+            data_paths = []
         self.input_paths = JsonClassPaths(json_path=json_path, dag_path=dag_path, data_paths=data_paths)
 
     def setup(self, scenario: Scenario):
         """Function to populate all the necessary parts of the json_class needed to execute tests"""
         self.scenario = scenario
         self._get_scenario_variables()
         self.scenario.setup_treatment_variables()
         self.causal_specification = CausalSpecification(
             scenario=self.scenario, causal_dag=CausalDAG(self.input_paths.dag_path)
         )
-        self._json_parse()
+        # Parse the JSON test plan
+        with open(self.input_paths.json_path, encoding="utf-8") as f:
+            self.test_plan = json.load(f)
+        # Populate the data
+        if self.input_paths.data_paths:
+            self.data = pd.concat([pd.read_csv(data_file, header=0) for data_file in self.input_paths.data_paths])
+        if len(self.data) == 0:
+            raise ValueError(
+                "No data found, either provide a path to a file containing data or manually populate the .data "
+                "attribute with a dataframe before calling .setup()"
+            )
         self._populate_metas()
 
     def _create_abstract_test_case(self, test, mutates, effects):
         assert len(test["mutations"]) == 1
         treatment_var = next(self.scenario.variables[v] for v in test["mutations"])
 
         if not treatment_var.distribution:
@@ -140,14 +152,15 @@
                         f"Executing test: {test['name']} \n"
                         + f"  {causal_test_case} \n"
                         + "  "
                         + ("\n  ").join(str(result[1]).split("\n"))
                         + "==============\n"
                         + f"  Result: {'FAILED' if result[0] else 'Passed'}"
                     )
+                    print(msg)
                 else:
                     abstract_test = self._create_abstract_test_case(test, mutates, effects)
                     concrete_tests, _ = abstract_test.generate_concrete_tests(5, 0.05)
                     failures, _ = self._execute_tests(concrete_tests, test, f_flag)
 
                     msg = (
                         f"Executing test: {test['name']} \n"
@@ -194,23 +207,14 @@
         for concrete_test in concrete_tests:
             failed, result = self._execute_test_case(concrete_test, test, f_flag)
             details.append(result)
             if failed:
                 failures += 1
         return failures, details
 
-    def _json_parse(self):
-        """Parse a JSON input file into inputs, outputs, metas and a test plan"""
-        with open(self.input_paths.json_path, encoding="utf-8") as f:
-            self.test_plan = json.load(f)
-        for data_file in self.input_paths.data_paths:
-            df = pd.read_csv(data_file, header=0)
-            self.data.append(df)
-        self.data = pd.concat(self.data)
-
     def _populate_metas(self):
         """
         Populate data with meta-variable values and add distributions to Causal Testing Framework Variables
         """
         for meta in self.scenario.variables_of_type(Meta):
             meta.populate(self.data)
 
@@ -226,21 +230,19 @@
         :rtype: bool
         """
         failed = False
 
         causal_test_engine, estimation_model = self._setup_test(
             causal_test_case, test, test["conditions"] if "conditions" in test else None
         )
-        causal_test_result = causal_test_engine.execute_test(
-            estimation_model, causal_test_case, estimate_type=causal_test_case.estimate_type
-        )
+        causal_test_result = causal_test_engine.execute_test(estimation_model, causal_test_case)
 
         test_passes = causal_test_case.expected_causal_effect.apply(causal_test_result)
 
-        if causal_test_result.ci_low() and causal_test_result.ci_high():
+        if causal_test_result.ci_low() is not None and causal_test_result.ci_high() is not None:
             result_string = (
                 f"{causal_test_result.ci_low()} < {causal_test_result.test_value.value} <  "
                 f"{causal_test_result.ci_high()}"
             )
         else:
             result_string = f"{causal_test_result.test_value.value} no confidence intervals"
 
@@ -347,15 +349,14 @@
             "--log_path",
             help="Specify a directory to change the location of the log file",
             default="./json_frontend.log",
         )
         parser.add_argument(
             "--data_path",
             help="Specify path to file containing runtime data",
-            required=True,
             nargs="+",
         )
         parser.add_argument(
             "--dag_path",
             help="Specify path to file containing the DAG, normally a .dot file",
             required=True,
         )
```

### Comparing `causal_testing_framework-4.1.0/causal_testing/specification/causal_dag.py` & `causal_testing_framework-4.2.0/causal_testing/specification/causal_dag.py`

 * *Files identical despite different names*

### Comparing `causal_testing_framework-4.1.0/causal_testing/specification/causal_specification.py` & `causal_testing_framework-4.2.0/causal_testing/specification/causal_specification.py`

 * *Files identical despite different names*

### Comparing `causal_testing_framework-4.1.0/causal_testing/specification/metamorphic_relation.py` & `causal_testing_framework-4.2.0/causal_testing/specification/metamorphic_relation.py`

 * *Files 4% similar despite different names*

```diff
@@ -3,21 +3,26 @@
 defined in our ICST paper [https://eprints.whiterose.ac.uk/195317/].
 """
 
 from dataclasses import dataclass
 from abc import abstractmethod
 from typing import Iterable
 from itertools import combinations
-import numpy as np
-import pandas as pd
+import argparse
+import logging
+import json
 import networkx as nx
+import pandas as pd
+import numpy as np
 
 from causal_testing.specification.causal_specification import CausalDAG, Node
 from causal_testing.data_collection.data_collector import ExperimentalDataCollector
 
+logger = logging.getLogger(__name__)
+
 
 @dataclass(order=True)
 class MetamorphicRelation:
     """Class representing a metamorphic relation."""
 
     treatment_var: Node
     output_var: Node
@@ -138,14 +143,15 @@
         return {
             "name": str(self),
             "estimator": "LinearRegressionEstimator",
             "estimate_type": "coefficient",
             "effect": "direct",
             "mutations": [self.treatment_var],
             "expected_effect": {self.output_var: "SomeEffect"},
+            "formula": f"{self.output_var} ~ {' + '.join([self.treatment_var] + self.adjustment_vars)}",
             "skip": skip,
         }
 
     def __str__(self):
         formatted_str = f"{self.treatment_var} --> {self.output_var}"
         if self.adjustment_vars:
             formatted_str += f" | {self.adjustment_vars}"
@@ -170,14 +176,15 @@
         return {
             "name": str(self),
             "estimator": "LinearRegressionEstimator",
             "estimate_type": "coefficient",
             "effect": "direct",
             "mutations": [self.treatment_var],
             "expected_effect": {self.output_var: "NoEffect"},
+            "formula": f"{self.output_var} ~ {' + '.join([self.treatment_var] + self.adjustment_vars)}",
             "skip": skip,
         }
 
     def __str__(self):
         formatted_str = f"{self.treatment_var} _||_ {self.output_var}"
         if self.adjustment_vars:
             formatted_str += f" | {self.adjustment_vars}"
@@ -240,7 +247,39 @@
             adj_set = list(dag.direct_effect_adjustment_sets([u], [v])[0])
             metamorphic_relations.append(ShouldCause(u, v, adj_set, dag))
         else:
             adj_set = list(dag.direct_effect_adjustment_sets([v], [u])[0])
             metamorphic_relations.append(ShouldCause(v, u, adj_set, dag))
 
     return metamorphic_relations
+
+
+if __name__ == "__main__":  # pragma: no cover
+    logging.basicConfig(format="%(levelname)s: %(message)s", level=logging.INFO)
+    parser = argparse.ArgumentParser(
+        description="A script for generating metamorphic relations to test the causal relationships in a given DAG."
+    )
+    parser.add_argument(
+        "--dag_path",
+        "-d",
+        help="Specify path to file containing the DAG, normally a .dot file.",
+        required=True,
+    )
+    parser.add_argument(
+        "--output_path",
+        "-o",
+        help="Specify path where tests should be saved, normally a .json file.",
+        required=True,
+    )
+    args = parser.parse_args()
+
+    causal_dag = CausalDAG(args.dag_path)
+    relations = generate_metamorphic_relations(causal_dag)
+    tests = [
+        relation.to_json_stub(skip=False)
+        for relation in relations
+        if len(list(causal_dag.graph.predecessors(relation.output_var))) > 0
+    ]
+
+    logger.info(f"Generated {len(tests)} tests. Saving to {args.output_path}.")
+    with open(args.output_path, "w", encoding="utf-8") as f:
+        json.dump({"tests": tests}, f, indent=2)
```

### Comparing `causal_testing_framework-4.1.0/causal_testing/specification/scenario.py` & `causal_testing_framework-4.2.0/causal_testing/specification/scenario.py`

 * *Files identical despite different names*

### Comparing `causal_testing_framework-4.1.0/causal_testing/specification/variable.py` & `causal_testing_framework-4.2.0/causal_testing/specification/variable.py`

 * *Files identical despite different names*

### Comparing `causal_testing_framework-4.1.0/causal_testing/testing/base_test_case.py` & `causal_testing_framework-4.2.0/causal_testing/testing/base_test_case.py`

 * *Files identical despite different names*

### Comparing `causal_testing_framework-4.1.0/causal_testing/testing/causal_test_case.py` & `causal_testing_framework-4.2.0/causal_testing/testing/causal_test_case.py`

 * *Files identical despite different names*

### Comparing `causal_testing_framework-4.1.0/causal_testing/testing/causal_test_engine.py` & `causal_testing_framework-4.2.0/causal_testing/testing/causal_test_engine.py`

 * *Files 2% similar despite different names*

```diff
@@ -77,54 +77,50 @@
             ]
 
             if self._check_positivity_violation(variables_for_positivity):
                 raise ValueError("POSITIVITY VIOLATION -- Cannot proceed.")
 
             estimators = test_suite[edge]["estimators"]
             tests = test_suite[edge]["tests"]
-            estimate_type = test_suite[edge]["estimate_type"]
             results = {}
             for estimator_class in estimators:
                 causal_test_results = []
 
                 for test in tests:
                     estimator = estimator_class(
                         test.treatment_variable.name,
                         test.treatment_value,
                         test.control_value,
                         minimal_adjustment_set,
                         test.outcome_variable.name,
                     )
                     if estimator.df is None:
                         estimator.df = self.scenario_execution_data_df
-                    causal_test_result = self._return_causal_test_results(estimate_type, estimator, test)
+                    causal_test_result = self._return_causal_test_results(estimator, test)
                     causal_test_results.append(causal_test_result)
 
                 results[estimator_class.__name__] = causal_test_results
             test_suite_results[edge] = results
         return test_suite_results
 
-    def execute_test(
-        self, estimator: type(Estimator), causal_test_case: CausalTestCase, estimate_type: str = "ate"
-    ) -> CausalTestResult:
+    def execute_test(self, estimator: type(Estimator), causal_test_case: CausalTestCase) -> CausalTestResult:
         """Execute a causal test case and return the causal test result.
 
         Test case execution proceeds with the following steps:
         (1) Check that data has been loaded using the method load_data
         (2) Check loaded data for any positivity violations and warn the user if so
         (3) Instantiate the estimator with the values of the causal test case.
         (4) Using the estimator, estimate the average treatment effect of the changing the treatment from control value
             to treatment value on the outcome of interest, adjusting for the identified adjustment set.
         (5) Depending on the estimator used, compute 95% confidence intervals for the estimate.
         (6) Store results in an instance of CausalTestResults.
         (7) Apply test oracle procedure to assign a pass/fail to the CausalTestResult and return.
 
         :param estimator: A reference to an Estimator class.
         :param causal_test_case: The CausalTestCase object to be tested
-        :param estimate_type: A string which denotes the type of estimate to return, ATE or CATE.
         :return causal_test_result: A CausalTestResult for the executed causal test case.
         """
         if self.scenario_execution_data_df.empty:
             raise ValueError("No data has been loaded. Please call load_data prior to executing a causal test case.")
         if estimator.df is None:
             estimator.df = self.scenario_execution_data_df
         treatment_variable = causal_test_case.treatment_variable
@@ -138,79 +134,80 @@
         minimal_adjustment_set = minimal_adjustment_set - set(outcome_variable.name)
 
         variables_for_positivity = list(minimal_adjustment_set) + [treatment_variable.name] + [outcome_variable.name]
 
         if self._check_positivity_violation(variables_for_positivity):
             raise ValueError("POSITIVITY VIOLATION -- Cannot proceed.")
 
-        causal_test_result = self._return_causal_test_results(estimate_type, estimator, causal_test_case)
+        causal_test_result = self._return_causal_test_results(estimator, causal_test_case)
         return causal_test_result
 
-    def _return_causal_test_results(self, estimate_type, estimator, causal_test_case):
+    def _return_causal_test_results(self, estimator, causal_test_case):
         """Depending on the estimator used, calculate the 95% confidence intervals and return in a causal_test_result
 
-        :param estimate_type: A string which denotes the type of estimate to return
         :param estimator: An Estimator class object
         :param causal_test_case: The concrete test case to be executed
         :return: a CausalTestResult object containing the confidence intervals
         """
-        if estimate_type == "cate":
+        if causal_test_case.estimate_type == "cate":
             logger.debug("calculating cate")
             if not hasattr(estimator, "estimate_cates"):
                 raise NotImplementedError(f"{estimator.__class__} has no CATE method.")
 
             cates_df, confidence_intervals = estimator.estimate_cates()
             causal_test_result = CausalTestResult(
                 estimator=estimator,
                 test_value=TestValue("ate", cates_df),
                 effect_modifier_configuration=causal_test_case.effect_modifier_configuration,
                 confidence_intervals=confidence_intervals,
             )
-        elif estimate_type == "risk_ratio":
+        elif causal_test_case.estimate_type == "risk_ratio":
             logger.debug("calculating risk_ratio")
             risk_ratio, confidence_intervals = estimator.estimate_risk_ratio()
             causal_test_result = CausalTestResult(
                 estimator=estimator,
                 test_value=TestValue("risk_ratio", risk_ratio),
                 effect_modifier_configuration=causal_test_case.effect_modifier_configuration,
                 confidence_intervals=confidence_intervals,
             )
-        elif estimate_type == "coefficient":
+        elif causal_test_case.estimate_type == "coefficient":
             logger.debug("calculating coefficient")
             coefficient, confidence_intervals = estimator.estimate_unit_ate()
             causal_test_result = CausalTestResult(
                 estimator=estimator,
                 test_value=TestValue("coefficient", coefficient),
                 effect_modifier_configuration=causal_test_case.effect_modifier_configuration,
                 confidence_intervals=confidence_intervals,
             )
-        elif estimate_type == "ate":
+        elif causal_test_case.estimate_type == "ate":
             logger.debug("calculating ate")
             ate, confidence_intervals = estimator.estimate_ate()
             causal_test_result = CausalTestResult(
                 estimator=estimator,
                 test_value=TestValue("ate", ate),
                 effect_modifier_configuration=causal_test_case.effect_modifier_configuration,
                 confidence_intervals=confidence_intervals,
             )
             # causal_test_result = CausalTestResult(minimal_adjustment_set, ate, confidence_intervals)
             # causal_test_result.apply_test_oracle_procedure(self.causal_test_case.expected_causal_effect)
-        elif estimate_type == "ate_calculated":
+        elif causal_test_case.estimate_type == "ate_calculated":
             logger.debug("calculating ate")
             ate, confidence_intervals = estimator.estimate_ate_calculated()
             causal_test_result = CausalTestResult(
                 estimator=estimator,
                 test_value=TestValue("ate", ate),
                 effect_modifier_configuration=causal_test_case.effect_modifier_configuration,
                 confidence_intervals=confidence_intervals,
             )
             # causal_test_result = CausalTestResult(minimal_adjustment_set, ate, confidence_intervals)
             # causal_test_result.apply_test_oracle_procedure(self.causal_test_case.expected_causal_effect)
         else:
-            raise ValueError(f"Invalid estimate type {estimate_type}, expected 'ate', 'cate', or 'risk_ratio'")
+            raise ValueError(
+                f"Invalid estimate type {causal_test_case.estimate_type}, expected 'ate', 'cate', or 'risk_ratio'"
+            )
         return causal_test_result
 
     def _check_positivity_violation(self, variables_list):
         """Check whether the dataframe has a positivity violation relative to the specified variables list.
 
         A positivity violation occurs when there is a stratum of the dataframe which does not have any data. Put simply,
         if we split the dataframe into covariate sub-groups, each sub-group must contain both a treated and untreated
```

### Comparing `causal_testing_framework-4.1.0/causal_testing/testing/causal_test_outcome.py` & `causal_testing_framework-4.2.0/causal_testing/testing/causal_test_outcome.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 # pylint: disable=too-few-public-methods
 """This module contains the CausalTestOutcome abstract class, as well as the concrete extension classes:
 ExactValue, Positive, Negative, SomeEffect, NoEffect"""
 
 from abc import ABC, abstractmethod
+from collections.abc import Iterable
 import numpy as np
 
 from causal_testing.testing.causal_test_result import CausalTestResult
 
 
 class CausalTestOutcome(ABC):
     """An abstract class representing an expected causal effect."""
@@ -22,69 +23,84 @@
         return type(self).__name__
 
 
 class SomeEffect(CausalTestOutcome):
     """An extension of TestOutcome representing that the expected causal effect should not be zero."""
 
     def apply(self, res: CausalTestResult) -> bool:
-        if res.test_value.type in {"ate", "coefficient"}:
+        if res.test_value.type == "ate":
             return (0 < res.ci_low() < res.ci_high()) or (res.ci_low() < res.ci_high() < 0)
+        if res.test_value.type == "coefficient":
+            ci_low = res.ci_low() if isinstance(res.ci_low(), Iterable) else [res.ci_low()]
+            ci_high = res.ci_high() if isinstance(res.ci_high(), Iterable) else [res.ci_high()]
+            return any(0 < ci_low < ci_high or ci_low < ci_high < 0 for ci_low, ci_high in zip(ci_low, ci_high))
         if res.test_value.type == "risk_ratio":
             return (1 < res.ci_low() < res.ci_high()) or (res.ci_low() < res.ci_high() < 1)
         raise ValueError(f"Test Value type {res.test_value.type} is not valid for this TestOutcome")
 
 
 class NoEffect(CausalTestOutcome):
     """An extension of TestOutcome representing that the expected causal effect should be zero."""
 
+    def __init__(self, atol: float = 1e-10):
+        self.atol = atol
+
     def apply(self, res: CausalTestResult) -> bool:
-        print("RESULT", res)
-        if res.test_value.type in {"ate", "coefficient"}:
-            return (res.ci_low() < 0 < res.ci_high()) or (abs(res.test_value.value) < 1e-10)
+        if res.test_value.type == "ate":
+            return (res.ci_low() < 0 < res.ci_high()) or (abs(res.test_value.value) < self.atol)
+        if res.test_value.type == "coefficient":
+            ci_low = res.ci_low() if isinstance(res.ci_low(), Iterable) else [res.ci_low()]
+            ci_high = res.ci_high() if isinstance(res.ci_high(), Iterable) else [res.ci_high()]
+            value = res.test_value.value if isinstance(res.ci_high(), Iterable) else [res.test_value.value]
+            return all(ci_low < 0 < ci_high for ci_low, ci_high in zip(ci_low, ci_high)) or all(
+                abs(v) < self.atol for v in value
+            )
         if res.test_value.type == "risk_ratio":
-            return (res.ci_low() < 1 < res.ci_high()) or np.isclose(res.test_value.value, 1.0, atol=1e-10)
+            return (res.ci_low() < 1 < res.ci_high()) or np.isclose(res.test_value.value, 1.0, atol=self.atol)
         raise ValueError(f"Test Value type {res.test_value.type} is not valid for this TestOutcome")
 
 
 class ExactValue(SomeEffect):
     """An extension of TestOutcome representing that the expected causal effect should be a specific value."""
 
-    def __init__(self, value: float, tolerance: float = None):
+    def __init__(self, value: float, atol: float = None):
         self.value = value
-        if tolerance is None:
-            self.tolerance = value * 0.05
+        if atol is None:
+            self.atol = value * 0.05
         else:
-            self.tolerance = tolerance
+            self.atol = atol
 
     def apply(self, res: CausalTestResult) -> bool:
         if res.ci_valid():
-            return super().apply(res) and np.isclose(res.test_value.value, self.value, atol=self.tolerance)
-        return np.isclose(res.test_value.value, self.value, atol=self.tolerance)
+            return super().apply(res) and np.isclose(res.test_value.value, self.value, atol=self.atol)
+        return np.isclose(res.test_value.value, self.value, atol=self.atol)
 
     def __str__(self):
-        return f"ExactValue: {self.value}±{self.tolerance}"
+        return f"ExactValue: {self.value}±{self.atol}"
 
 
 class Positive(SomeEffect):
     """An extension of TestOutcome representing that the expected causal effect should be positive."""
 
     def apply(self, res: CausalTestResult) -> bool:
         if res.ci_valid() and not super().apply(res):
             return False
         if res.test_value.type in {"ate", "coefficient"}:
             return res.test_value.value > 0
         if res.test_value.type == "risk_ratio":
             return res.test_value.value > 1
+        # Dead code but necessary for pylint
         raise ValueError(f"Test Value type {res.test_value.type} is not valid for this TestOutcome")
 
 
 class Negative(SomeEffect):
     """An extension of TestOutcome representing that the expected causal effect should be negative."""
 
     def apply(self, res: CausalTestResult) -> bool:
         if res.ci_valid() and not super().apply(res):
             return False
         if res.test_value.type in {"ate", "coefficient"}:
             return res.test_value.value < 0
         if res.test_value.type == "risk_ratio":
             return res.test_value.value < 1
+        # Dead code but necessary for pylint
         raise ValueError(f"Test Value type {res.test_value.type} is not valid for this TestOutcome")
```

### Comparing `causal_testing_framework-4.1.0/causal_testing/testing/causal_test_result.py` & `causal_testing_framework-4.2.0/causal_testing/testing/causal_test_result.py`

 * *Files 12% similar despite different names*

```diff
@@ -39,26 +39,35 @@
 
         if effect_modifier_configuration is not None:
             self.effect_modifier_configuration = effect_modifier_configuration
         else:
             self.effect_modifier_configuration = {}
 
     def __str__(self):
+        def push(s, inc="  "):
+            return inc + str(s).replace("\n", "\n" + inc)
+
+        result_str = str(self.test_value.value)
+        if "\n" in result_str:
+            result_str = "\n" + push(self.test_value.value)
         base_str = (
             f"Causal Test Result\n==============\n"
             f"Treatment: {self.estimator.treatment}\n"
             f"Control value: {self.estimator.control_value}\n"
             f"Treatment value: {self.estimator.treatment_value}\n"
             f"Outcome: {self.estimator.outcome}\n"
             f"Adjustment set: {self.adjustment_set}\n"
-            f"{self.test_value.type}: {self.test_value.value}\n"
+            f"{self.test_value.type}: {result_str}\n"
         )
         confidence_str = ""
         if self.confidence_intervals:
-            confidence_str += f"Confidence intervals: {self.confidence_intervals}\n"
+            ci_str = " " + str(self.confidence_intervals)
+            if "\n" in ci_str:
+                ci_str = " " + push(pd.DataFrame(self.confidence_intervals).transpose().to_string(header=False))
+            confidence_str += f"Confidence intervals:{ci_str}\n"
         return base_str + confidence_str
 
     def to_dict(self):
         """Return result contents as a dictionary
         :return: Dictionary containing contents of causal_test_result
         """
         base_dict = {
@@ -72,22 +81,22 @@
         if self.confidence_intervals and all(self.confidence_intervals):
             base_dict["ci_low"] = min(self.confidence_intervals)
             base_dict["ci_high"] = max(self.confidence_intervals)
         return base_dict
 
     def ci_low(self):
         """Return the lower bracket of the confidence intervals."""
-        if self.confidence_intervals and all(self.confidence_intervals):
-            return min(self.confidence_intervals)
+        if self.confidence_intervals:
+            return self.confidence_intervals[0]
         return None
 
     def ci_high(self):
         """Return the higher bracket of the confidence intervals."""
-        if self.confidence_intervals and all(self.confidence_intervals):
-            return max(self.confidence_intervals)
+        if self.confidence_intervals:
+            return self.confidence_intervals[1]
         return None
 
     def ci_valid(self) -> bool:
         """Return whether or not the result has valid confidence invervals"""
         return self.ci_low() and (not pd.isnull(self.ci_low())) and self.ci_high() and (not pd.isnull(self.ci_high()))
 
     def summary(self):
```

### Comparing `causal_testing_framework-4.1.0/causal_testing/testing/causal_test_suite.py` & `causal_testing_framework-4.2.0/causal_testing/testing/causal_test_suite.py`

 * *Files identical despite different names*

### Comparing `causal_testing_framework-4.1.0/causal_testing/testing/estimators.py` & `causal_testing_framework-4.2.0/causal_testing/testing/estimators.py`

 * *Files 2% similar despite different names*

```diff
@@ -331,38 +331,43 @@
     def estimate_unit_ate(self) -> float:
         """Estimate the unit average treatment effect of the treatment on the outcome. That is, the change in outcome
         caused by a unit change in treatment.
 
         :return: The unit average treatment effect and the 95% Wald confidence intervals.
         """
         model = self._run_linear_regression()
-        assert self.treatment in model.params, f"{self.treatment} not in {model.params}"
-        unit_effect = model.params[[self.treatment]].values[0]  # Unit effect is the coefficient of the treatment
-        [ci_low, ci_high] = self._get_confidence_intervals(model)
-
+        newline = "\n"
+        print(model.conf_int())
+        treatment = [self.treatment]
+        if str(self.df.dtypes[self.treatment]) == "object":
+            design_info = dmatrix(self.formula.split("~")[1], self.df).design_info
+            treatment = design_info.column_names[design_info.term_name_slices[self.treatment]]
+        assert set(treatment).issubset(
+            model.params.index.tolist()
+        ), f"{treatment} not in\n{'  '+str(model.params.index).replace(newline, newline+'  ')}"
+        unit_effect = model.params[treatment]  # Unit effect is the coefficient of the treatment
+        [ci_low, ci_high] = self._get_confidence_intervals(model, treatment)
+        if str(self.df.dtypes[self.treatment]) != "object":
+            unit_effect = unit_effect[0]
+            ci_low = ci_low[0]
+            ci_high = ci_high[0]
         return unit_effect, [ci_low, ci_high]
 
     def estimate_ate(self) -> tuple[float, list[float, float], float]:
         """Estimate the average treatment effect of the treatment on the outcome. That is, the change in outcome caused
         by changing the treatment variable from the control value to the treatment value.
 
         :return: The average treatment effect and the 95% Wald confidence intervals.
         """
         model = self._run_linear_regression()
         self.model = model
 
         # Create an empty individual for the control and treated
         individuals = pd.DataFrame(1, index=["control", "treated"], columns=model.params.index)
 
-        # This is a temporary hack
-        # for t in self.square_terms:
-        #     individuals[t + "^2"] = individuals[t] ** 2
-        # for a, b in self.product_terms:
-        #     individuals[f"{a}*{b}"] = individuals[a] * individuals[b]
-
         # It is ABSOLUTELY CRITICAL that these go last, otherwise we can't index
         # the effect with "ate = t_test_results.effect[0]"
         individuals.loc["control", [self.treatment]] = self.control_value
         individuals.loc["treated", [self.treatment]] = self.treatment_value
 
         # Perform a t-test to compare the predicted outcome of the control and treated individual (ATE)
         t_test_results = model.t_test(individuals.loc["treated"] - individuals.loc["control"])
@@ -420,43 +425,14 @@
         """
         control_outcome, treatment_outcome = self.estimate_control_treatment(adjustment_config=adjustment_config)
         ci_low = treatment_outcome["mean_ci_lower"] - control_outcome["mean_ci_upper"]
         ci_high = treatment_outcome["mean_ci_upper"] - control_outcome["mean_ci_lower"]
 
         return (treatment_outcome["mean"] - control_outcome["mean"]), [ci_low, ci_high]
 
-    def estimate_cates(self) -> tuple[float, list[float, float]]:
-        """Estimate the conditional average treatment effect of the treatment on the outcome. That is, the change
-        in outcome caused by changing the treatment variable from the control value to the treatment value.
-
-        :return: The conditional average treatment effect and the 95% Wald confidence intervals.
-        """
-        assert (
-            self.effect_modifiers
-        ), f"Must have at least one effect modifier to compute CATE - {self.effect_modifiers}."
-        x = pd.DataFrame()
-        x[self.treatment] = [self.treatment_value, self.control_value]
-        x["Intercept"] = 1  # self.intercept
-        for k, v in self.effect_modifiers.items():
-            self.adjustment_set.add(k)
-            x[k] = v
-        if hasattr(self, "square_terms"):
-            for t in self.square_terms:
-                x[t + "^2"] = x[t] ** 2
-        if hasattr(self, "product_terms"):
-            for a, b in self.product_terms:
-                x[f"{a}*{b}"] = x[a] * x[b]
-
-        model = self._run_linear_regression()
-        y = model.predict(x)
-        treatment_outcome = y.iloc[0]
-        control_outcome = y.iloc[1]
-
-        return treatment_outcome - control_outcome, None
-
     def _run_linear_regression(self) -> RegressionResultsWrapper:
         """Run linear regression of the treatment and adjustment set against the outcome and return the model.
 
         :return: The model after fitting to data.
         """
         # 1. Reduce dataframe to contain only the necessary columns
         reduced_df = self.df.copy()
@@ -468,30 +444,24 @@
 
         # 2. Add intercept
         reduced_df["Intercept"] = 1  # self.intercept
 
         # 3. Estimate the unit difference in outcome caused by unit difference in treatment
         cols = [self.treatment]
         cols += [x for x in self.adjustment_set if x not in cols]
-        treatment_and_adjustments_cols = reduced_df[cols + ["Intercept"]]
-        for col in treatment_and_adjustments_cols:
-            if str(treatment_and_adjustments_cols.dtypes[col]) == "object":
-                treatment_and_adjustments_cols = pd.get_dummies(
-                    treatment_and_adjustments_cols, columns=[col], drop_first=True
-                )
         model = smf.ols(formula=self.formula, data=self.df).fit()
         return model
 
-    def _get_confidence_intervals(self, model):
+    def _get_confidence_intervals(self, model, treatment):
         confidence_intervals = model.conf_int(alpha=0.05, cols=None)
         ci_low, ci_high = (
-            confidence_intervals[0][[self.treatment]],
-            confidence_intervals[1][[self.treatment]],
+            confidence_intervals[0].loc[treatment],
+            confidence_intervals[1].loc[treatment],
         )
-        return [ci_low.values[0], ci_high.values[0]]
+        return [ci_low, ci_high]
 
 
 class InstrumentalVariableEstimator(Estimator):
     """
     Carry out estimation using instrumental variable adjustment rather than conventional adjustment. This means we do
     not need to observe all confounders in order to adjust for them. A key assumption here is linearity.
     """
```

### Comparing `causal_testing_framework-4.1.0/causal_testing/testing/intervention.py` & `causal_testing_framework-4.2.0/causal_testing/testing/intervention.py`

 * *Files identical despite different names*

### Comparing `causal_testing_framework-4.1.0/causal_testing/testing/validation.py` & `causal_testing_framework-4.2.0/causal_testing/utils/validation.py`

 * *Files 11% similar despite different names*

```diff
@@ -4,15 +4,16 @@
 from scipy.stats import t
 from statsmodels.regression.linear_model import RegressionResultsWrapper
 
 
 class CausalValidator:
     """A suite of validation tools to perform Quantitive Bias Analysis to back up causal claims"""
 
-    def estimate_robustness(self, model: RegressionResultsWrapper, q=1, alpha=1):
+    @staticmethod
+    def estimate_robustness(model: RegressionResultsWrapper, q=1, alpha=1):
         """Calculate the robustness of a linear regression model. This allow
         the user to identify how large an unidentified confounding variable
         would need to be to nullify the causal relationship under test."""
 
         dof = model.df_resid
         t_values = model.tvalues
 
@@ -20,27 +21,29 @@
         f_crit = abs(t.ppf(alpha / 2, dof - 1)) / math.sqrt(dof - 1)
         fqa = fq - f_crit
 
         rv = 0.5 * (np.sqrt(fqa**4 + (4 * fqa**2)) - fqa**2)
 
         return rv
 
-    def estimate_e_value(self, risk_ratio: float) -> float:
+    @staticmethod
+    def estimate_e_value(risk_ratio: float) -> float:
         """Calculate the E value from a risk ratio. This allow
         the user to identify how large a risk an unidentified confounding
         variable would need to be to nullify the causal relationship
         under test."""
 
         if risk_ratio >= 1:
             return risk_ratio + math.sqrt(risk_ratio * (risk_ratio - 1))
 
         risk_ratio_prime = 1 / risk_ratio
         return risk_ratio_prime + math.sqrt(risk_ratio_prime * (risk_ratio_prime - 1))
 
-    def estimate_e_value_using_ci(self, risk_ratio: float, confidence_intervals: tuple[float, float]) -> float:
+    @staticmethod
+    def estimate_e_value_using_ci(risk_ratio: float, confidence_intervals: tuple[float, float]) -> float:
         """Calculate the E value from a risk ratio and it's confidence intervals.
         This allow the user to identify how large a risk an unidentified
         confounding variable would need to be to nullify the causal relationship
         under test."""
 
         if risk_ratio >= 1:
             lower_limit = confidence_intervals[0]
```

### Comparing `causal_testing_framework-4.1.0/causal_testing_framework.egg-info/PKG-INFO` & `causal_testing_framework-4.2.0/causal_testing_framework.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: causal-testing-framework
-Version: 4.1.0
+Version: 4.2.0
 Summary: A framework for causal testing using causal directed acyclic graphs.
 Author: The CITCOM team
 License: MIT
 Project-URL: Bug_Tracker, https://github.com/CITCOM-project/CausalTestingFramework/issues
 Project-URL: Documentation, https://causal-testing-framework.readthedocs.io/
 Project-URL: Source, https://github.com/CITCOM-project/CausalTestingFramework
 Keywords: causal inference,verification
```

### Comparing `causal_testing_framework-4.1.0/causal_testing_framework.egg-info/SOURCES.txt` & `causal_testing_framework-4.2.0/causal_testing_framework.egg-info/SOURCES.txt`

 * *Files 3% similar despite different names*

```diff
@@ -32,15 +32,16 @@
 causal_testing/testing/causal_test_engine.py
 causal_testing/testing/causal_test_outcome.py
 causal_testing/testing/causal_test_result.py
 causal_testing/testing/causal_test_suite.py
 causal_testing/testing/effect.py
 causal_testing/testing/estimators.py
 causal_testing/testing/intervention.py
-causal_testing/testing/validation.py
+causal_testing/utils/__init__.py
+causal_testing/utils/validation.py
 causal_testing_framework.egg-info/PKG-INFO
 causal_testing_framework.egg-info/SOURCES.txt
 causal_testing_framework.egg-info/dependency_links.txt
 causal_testing_framework.egg-info/requires.txt
 causal_testing_framework.egg-info/top_level.txt
 docs/Makefile
 docs/README.md
@@ -48,14 +49,17 @@
 docs/source/conf.py
 docs/source/description.rst
 docs/source/glossary.md
 docs/source/index.rst
 docs/source/installation.rst
 docs/source/requirements.txt
 docs/source/usage.rst
+docs/source/dev/actions_and_webhooks.rst
+docs/source/dev/documentation.rst
+docs/source/dev/version_release.rst
 docs/source/frontends/json_front_end.rst
 docs/source/frontends/test_suite.rst
 docs/source/images/workflow.png
 docs/source/modules/causal_specification.rst
 docs/source/modules/causal_tests.rst
 docs/source/modules/data_collector.rst
 examples/.gitignore
```

### Comparing `causal_testing_framework-4.1.0/docs/Makefile` & `causal_testing_framework-4.2.0/docs/Makefile`

 * *Files identical despite different names*

### Comparing `causal_testing_framework-4.1.0/docs/README.md` & `causal_testing_framework-4.2.0/docs/README.md`

 * *Files identical despite different names*

### Comparing `causal_testing_framework-4.1.0/docs/make.bat` & `causal_testing_framework-4.2.0/docs/make.bat`

 * *Files identical despite different names*

### Comparing `causal_testing_framework-4.1.0/docs/source/conf.py` & `causal_testing_framework-4.2.0/docs/source/conf.py`

 * *Files identical despite different names*

### Comparing `causal_testing_framework-4.1.0/docs/source/description.rst` & `causal_testing_framework-4.2.0/docs/source/description.rst`

 * *Files identical despite different names*

### Comparing `causal_testing_framework-4.1.0/docs/source/frontends/test_suite.rst` & `causal_testing_framework-4.2.0/docs/source/frontends/test_suite.rst`

 * *Files identical despite different names*

### Comparing `causal_testing_framework-4.1.0/docs/source/images/workflow.png` & `causal_testing_framework-4.2.0/docs/source/images/workflow.png`

 * *Files identical despite different names*

### Comparing `causal_testing_framework-4.1.0/docs/source/index.rst` & `causal_testing_framework-4.2.0/docs/source/index.rst`

 * *Files 5% similar despite different names*

```diff
@@ -45,12 +45,20 @@
 
 .. toctree::
    :maxdepth: 1
    :caption: Glossary
 
    glossary
 
+.. toctree::
+   :maxdepth: 1
+   :caption: Development Documentation
+
+   /dev/version_release
+   /dev/documentation
+   /dev/actions_and_webhooks
+
 Indices and tables
 ==================
 
 * :ref:`genindex`
 * :ref:`modindex`
```

### Comparing `causal_testing_framework-4.1.0/docs/source/installation.rst` & `causal_testing_framework-4.2.0/docs/source/installation.rst`

 * *Files identical despite different names*

### Comparing `causal_testing_framework-4.1.0/docs/source/modules/causal_specification.rst` & `causal_testing_framework-4.2.0/docs/source/modules/causal_specification.rst`

 * *Files identical despite different names*

### Comparing `causal_testing_framework-4.1.0/docs/source/modules/causal_tests.rst` & `causal_testing_framework-4.2.0/docs/source/modules/causal_tests.rst`

 * *Files identical despite different names*

### Comparing `causal_testing_framework-4.1.0/docs/source/modules/data_collector.rst` & `causal_testing_framework-4.2.0/docs/source/modules/data_collector.rst`

 * *Files identical despite different names*

### Comparing `causal_testing_framework-4.1.0/docs/source/usage.rst` & `causal_testing_framework-4.2.0/docs/source/usage.rst`

 * *Files 3% similar despite different names*

```diff
@@ -103,14 +103,13 @@
 We can now execute the test using the estimation model. This returns a causal test result, from which we can extract
 various information. Here, we simply assert that the observed result is (on average) what we expect to see.
 
 .. code-block:: python
 
    causal_test_result = causal_test_engine.execute_test(
        estimator = estimation_model,
-       causal_test_case = causal_test_case,
-       estimate_type = "ate")
+       causal_test_case = causal_test_case)
    test_passes = causal_test_case.expected_causal_effect.apply(causal_test_result)
    assert test_passes, "Expected to see a positive change in y."
 
 Multiple tests can be executed at once using the test engines `test_suite <https://causal-testing-framework.readthedocs.io/en/test_suite.html>`_
 feature
```

### Comparing `causal_testing_framework-4.1.0/examples/covasim_/doubling_beta/README.md` & `causal_testing_framework-4.2.0/examples/covasim_/doubling_beta/README.md`

 * *Files identical despite different names*

### Comparing `causal_testing_framework-4.1.0/examples/covasim_/doubling_beta/dag.png` & `causal_testing_framework-4.2.0/examples/covasim_/doubling_beta/dag.png`

 * *Files identical despite different names*

### Comparing `causal_testing_framework-4.1.0/examples/covasim_/doubling_beta/data/10k_observational_data.csv` & `causal_testing_framework-4.2.0/examples/covasim_/doubling_beta/data/10k_observational_data.csv`

 * *Files identical despite different names*

### Comparing `causal_testing_framework-4.1.0/examples/covasim_/doubling_beta/example_beta.py` & `causal_testing_framework-4.2.0/examples/covasim_/doubling_beta/example_beta.py`

 * *Files 0% similar despite different names*

```diff
@@ -61,28 +61,28 @@
         {"avg_age", "contacts"},  # We use custom adjustment set
         "cum_infections",
         df=past_execution_df,
         formula="cum_infections ~ beta + np.power(beta, 2) + avg_age + contacts",
     )
 
     # Add squared terms for beta, since it has a quadratic relationship with cumulative infections
-    causal_test_result = causal_test_engine.execute_test(linear_regression_estimator, causal_test_case, "ate")
+    causal_test_result = causal_test_engine.execute_test(linear_regression_estimator, causal_test_case)
 
     # Repeat for association estimate (no adjustment)
     no_adjustment_linear_regression_estimator = LinearRegressionEstimator(
         "beta",
         0.032,
         0.016,
         set(),
         "cum_infections",
         df=past_execution_df,
         formula="cum_infections ~ beta + np.power(beta, 2)",
     )
     association_test_result = causal_test_engine.execute_test(
-        no_adjustment_linear_regression_estimator, causal_test_case, "ate"
+        no_adjustment_linear_regression_estimator, causal_test_case
     )
 
     # Store results for plotting
     results_dict["association"] = {
         "ate": association_test_result.test_value.value,
         "cis": association_test_result.confidence_intervals,
         "df": past_execution_df,
@@ -106,15 +106,15 @@
             0.016,
             {"avg_age", "contacts"},
             "cum_infections",
             df=counterfactual_past_execution_df,
             formula="cum_infections ~ beta + np.power(beta, 2) + avg_age + contacts",
         )
         counterfactual_causal_test_result = causal_test_engine.execute_test(
-            linear_regression_estimator, causal_test_case, "ate"
+            linear_regression_estimator, causal_test_case
         )
         results_dict["counterfactual"] = {
             "ate": counterfactual_causal_test_result.test_value.value,
             "cis": counterfactual_causal_test_result.confidence_intervals,
             "df": counterfactual_past_execution_df,
         }
         if verbose:
```

### Comparing `causal_testing_framework-4.1.0/examples/covasim_/vaccinating_elderly/README.md` & `causal_testing_framework-4.2.0/examples/covasim_/vaccinating_elderly/README.md`

 * *Files identical despite different names*

### Comparing `causal_testing_framework-4.1.0/examples/covasim_/vaccinating_elderly/dag.png` & `causal_testing_framework-4.2.0/examples/covasim_/vaccinating_elderly/dag.png`

 * *Files identical despite different names*

### Comparing `causal_testing_framework-4.1.0/examples/covasim_/vaccinating_elderly/example_vaccine.py` & `causal_testing_framework-4.2.0/examples/covasim_/vaccinating_elderly/example_vaccine.py`

 * *Files 0% similar despite different names*

```diff
@@ -95,15 +95,15 @@
 
         # 9. Build statistical model
         linear_regression_estimator = LinearRegressionEstimator(
             vaccine.name, 1, 0, minimal_adjustment_set, outcome_variable.name
         )
 
         # 10. Execute test and save results in dict
-        causal_test_result = causal_test_engine.execute_test(linear_regression_estimator, causal_test_case, "ate")
+        causal_test_result = causal_test_engine.execute_test(linear_regression_estimator, causal_test_case)
         if verbose:
             logging.info("Causation:\n%s", causal_test_result)
         results_dict[outcome_variable.name]["ate"] = causal_test_result.test_value.value
         results_dict[outcome_variable.name]["cis"] = causal_test_result.confidence_intervals
         results_dict[outcome_variable.name]["test_passes"] = causal_test_case.expected_causal_effect.apply(
             causal_test_result
         )
```

### Comparing `causal_testing_framework-4.1.0/examples/lr91/README.md` & `causal_testing_framework-4.2.0/examples/lr91/README.md`

 * *Files identical despite different names*

### Comparing `causal_testing_framework-4.1.0/examples/lr91/dag.dot` & `causal_testing_framework-4.2.0/examples/lr91/dag.dot`

 * *Files identical despite different names*

### Comparing `causal_testing_framework-4.1.0/examples/lr91/dag.png` & `causal_testing_framework-4.2.0/examples/lr91/dag.png`

 * *Files identical despite different names*

### Comparing `causal_testing_framework-4.1.0/examples/lr91/data/normalised_results.csv` & `causal_testing_framework-4.2.0/examples/lr91/data/normalised_results.csv`

 * *Files identical despite different names*

### Comparing `causal_testing_framework-4.1.0/examples/lr91/data/results.csv` & `causal_testing_framework-4.2.0/examples/lr91/data/results.csv`

 * *Files identical despite different names*

### Comparing `causal_testing_framework-4.1.0/examples/lr91/example_max_conductances.py` & `causal_testing_framework-4.2.0/examples/lr91/example_max_conductances.py`

 * *Files 0% similar despite different names*

```diff
@@ -144,15 +144,15 @@
     # 9. Obtain the minimal adjustment set from the causal DAG
     minimal_adjustment_set = causal_dag.identification(base_test_case)
     linear_regression_estimator = LinearRegressionEstimator(
         treatment_var.name, treatment_val, control_val, minimal_adjustment_set, "APD90"
     )
 
     # 10. Run the causal test and print results
-    causal_test_result = causal_test_engine.execute_test(linear_regression_estimator, causal_test_case, "ate")
+    causal_test_result = causal_test_engine.execute_test(linear_regression_estimator, causal_test_case)
     logger.info("%s", causal_test_result)
     return causal_test_result.test_value.value, causal_test_result.confidence_intervals
 
 
 def plot_ates_with_cis(results_dict: dict, xs: list, save: bool = False, show: bool = False):
     """Plot the average treatment effects for a given treatment against a list of x-values with confidence intervals.
```

### Comparing `causal_testing_framework-4.1.0/examples/lr91/example_max_conductances_test_suite.py` & `causal_testing_framework-4.2.0/examples/lr91/example_max_conductances_test_suite.py`

 * *Files identical despite different names*

### Comparing `causal_testing_framework-4.1.0/examples/poisson/README.md` & `causal_testing_framework-4.2.0/examples/poisson/README.md`

 * *Files identical despite different names*

### Comparing `causal_testing_framework-4.1.0/examples/poisson/causal_tests.json` & `causal_testing_framework-4.2.0/examples/poisson/causal_tests.json`

 * *Files identical despite different names*

### Comparing `causal_testing_framework-4.1.0/examples/poisson/dag.dot` & `causal_testing_framework-4.2.0/examples/poisson/dag.dot`

 * *Files identical despite different names*

### Comparing `causal_testing_framework-4.1.0/examples/poisson/data.csv` & `causal_testing_framework-4.2.0/examples/poisson/data.csv`

 * *Files identical despite different names*

### Comparing `causal_testing_framework-4.1.0/examples/poisson/example_run_causal_tests.py` & `causal_testing_framework-4.2.0/examples/poisson/example_run_causal_tests.py`

 * *Files 4% similar despite different names*

```diff
@@ -61,34 +61,34 @@
 
         return treatment_outcome - control_outcome, None
 
 
 class PoissonWidthHeight(CausalTestOutcome):
     """An extension of TestOutcome representing that the expected causal effect should be positive."""
 
-    def __init__(self, tolerance=0.5):
-        self.tolerance = tolerance
+    def __init__(self, atol=0.5):
+        self.atol = atol
         self.i2c = None
 
     def apply(self, res: CausalTestResult) -> bool:
         # TODO: confidence intervals?
         logger.info("=== APPLYING ===")
         logger.info("effect_modifier_configuration", res.effect_modifier_configuration)
         effect_modifier_configuration = {k.name: v for k, v in res.effect_modifier_configuration.items()}
         c = res.treatment_value - res.control_value
         i = effect_modifier_configuration["intensity"]
         self.i2c = i * 2 * c
         logger.info("2ic: 2 * %s * %s = %s", i, c, self.i2c)
         logger.info("ate: %s", res.test_value.value)
-        return np.isclose(res.test_value.value, self.i2c, atol=self.tolerance)
+        return np.isclose(res.test_value.value, self.i2c, atol=self.atol)
 
     def __str__(self):
         if self.i2c is None:
-            return f"PoissonWidthHeight±{self.tolerance}"
-        return f"PoissonWidthHeight:{self.i2c}±{self.tolerance}"
+            return f"PoissonWidthHeight±{self.atol}"
+        return f"PoissonWidthHeight:{self.i2c}±{self.atol}"
 
 
 def populate_width_height(data):
     data["width_plus_height"] = data["width"] + data["height"]
 
 
 def populate_num_lines_unit(data):
@@ -117,15 +117,15 @@
 
 constraints = ["width > 0", "height > 0", "intensity > 0"]
 
 effects = {
     "PoissonWidthHeight": PoissonWidthHeight(),
     "Positive": Positive(),
     "Negative": Negative(),
-    "ExactValue4_05": ExactValue(4, tolerance=0.5),
+    "ExactValue4_05": ExactValue(4, atol=0.5),
     "NoEffect": NoEffect(),
 }
 
 estimators = {
     "WidthHeightEstimator": WidthHeightEstimator,
     "CausalForestEstimator": CausalForestEstimator,
     "LinearRegressionEstimator": LinearRegressionEstimator,
@@ -159,23 +159,27 @@
 
     json_utility = JsonUtility(log_path)  # Create an instance of the extended JsonUtility class
     json_utility.set_paths(
         json_path, dag_path, [data_path]
     )  # Set the path to the data.csv, dag.dot and causal_tests.json file
 
     # Load the Causal Variables into the JsonUtility class ready to be used in the tests
-    json_utility.setup(scenario=modelling_scenario)  # Sets up all the necessary parts of the json_class needed to execute tests
+    json_utility.setup(
+        scenario=modelling_scenario
+    )  # Sets up all the necessary parts of the json_class needed to execute tests
 
     json_utility.run_json_tests(effects=effects, mutates=mutates, estimators=estimators, f_flag=False)
 
 
 if __name__ == "__main__":
     args = JsonUtility.get_args()
     json_utility = JsonUtility(args.log_path)  # Create an instance of the extended JsonUtility class
     json_utility.set_paths(
         args.json_path, args.dag_path, args.data_path
     )  # Set the path to the data.csv, dag.dot and causal_tests.json file
 
     # Load the Causal Variables into the JsonUtility class ready to be used in the tests
-    json_utility.setup(scenario=modelling_scenario)  # Sets up all the necessary parts of the json_class needed to execute tests
+    json_utility.setup(
+        scenario=modelling_scenario
+    )  # Sets up all the necessary parts of the json_class needed to execute tests
 
     json_utility.run_json_tests(effects=effects, mutates=mutates, estimators=estimators, f_flag=args.f)
```

### Comparing `causal_testing_framework-4.1.0/examples/poisson-line-process/README.md` & `causal_testing_framework-4.2.0/examples/poisson-line-process/README.md`

 * *Files identical despite different names*

### Comparing `causal_testing_framework-4.1.0/examples/poisson-line-process/dag.png` & `causal_testing_framework-4.2.0/examples/poisson-line-process/dag.png`

 * *Files identical despite different names*

### Comparing `causal_testing_framework-4.1.0/examples/poisson-line-process/data/random/data_random_1000.csv` & `causal_testing_framework-4.2.0/examples/poisson-line-process/data/random/data_random_1000.csv`

 * *Files identical despite different names*

### Comparing `causal_testing_framework-4.1.0/examples/poisson-line-process/data/smt_100/data_smt_wh10_100.csv` & `causal_testing_framework-4.2.0/examples/poisson-line-process/data/smt_100/data_smt_wh10_100.csv`

 * *Files identical despite different names*

### Comparing `causal_testing_framework-4.1.0/examples/poisson-line-process/data/smt_100/data_smt_wh1_100.csv` & `causal_testing_framework-4.2.0/examples/poisson-line-process/data/smt_100/data_smt_wh1_100.csv`

 * *Files identical despite different names*

### Comparing `causal_testing_framework-4.1.0/examples/poisson-line-process/data/smt_100/data_smt_wh2_100.csv` & `causal_testing_framework-4.2.0/examples/poisson-line-process/data/smt_100/data_smt_wh2_100.csv`

 * *Files identical despite different names*

### Comparing `causal_testing_framework-4.1.0/examples/poisson-line-process/data/smt_100/data_smt_wh3_100.csv` & `causal_testing_framework-4.2.0/examples/poisson-line-process/data/smt_100/data_smt_wh3_100.csv`

 * *Files identical despite different names*

### Comparing `causal_testing_framework-4.1.0/examples/poisson-line-process/data/smt_100/data_smt_wh4_100.csv` & `causal_testing_framework-4.2.0/examples/poisson-line-process/data/smt_100/data_smt_wh4_100.csv`

 * *Files identical despite different names*

### Comparing `causal_testing_framework-4.1.0/examples/poisson-line-process/data/smt_100/data_smt_wh5_100.csv` & `causal_testing_framework-4.2.0/examples/poisson-line-process/data/smt_100/data_smt_wh5_100.csv`

 * *Files identical despite different names*

### Comparing `causal_testing_framework-4.1.0/examples/poisson-line-process/data/smt_100/data_smt_wh6_100.csv` & `causal_testing_framework-4.2.0/examples/poisson-line-process/data/smt_100/data_smt_wh6_100.csv`

 * *Files identical despite different names*

### Comparing `causal_testing_framework-4.1.0/examples/poisson-line-process/data/smt_100/data_smt_wh7_100.csv` & `causal_testing_framework-4.2.0/examples/poisson-line-process/data/smt_100/data_smt_wh7_100.csv`

 * *Files identical despite different names*

### Comparing `causal_testing_framework-4.1.0/examples/poisson-line-process/data/smt_100/data_smt_wh8_100.csv` & `causal_testing_framework-4.2.0/examples/poisson-line-process/data/smt_100/data_smt_wh8_100.csv`

 * *Files identical despite different names*

### Comparing `causal_testing_framework-4.1.0/examples/poisson-line-process/data/smt_100/data_smt_wh9_100.csv` & `causal_testing_framework-4.2.0/examples/poisson-line-process/data/smt_100/data_smt_wh9_100.csv`

 * *Files identical despite different names*

### Comparing `causal_testing_framework-4.1.0/examples/poisson-line-process/example_poisson_process.py` & `causal_testing_framework-4.2.0/examples/poisson-line-process/example_poisson_process.py`

 * *Files 2% similar despite different names*

```diff
@@ -119,15 +119,15 @@
             outcome=outcome,
             df=data,
             effect_modifiers=causal_test_case.effect_modifier_configuration,
             formula=f"{outcome} ~ {treatment} + {'+'.join(square_terms + inverse_terms + list([e for e in causal_test_case.effect_modifier_configuration]))} -1",
         )
 
     # 10. Execute the test
-    causal_test_result = causal_test_engine.execute_test(estimator, causal_test_case, causal_test_case.estimate_type)
+    causal_test_result = causal_test_engine.execute_test(estimator, causal_test_case)
 
     return causal_test_result
 
 
 def test_poisson_intensity_num_shapes(save=False):
     intensity_num_shapes_results = []
     for wh in range(1, 11):
@@ -135,15 +135,15 @@
         for control_value, treatment_value in [(1, 2), (2, 4), (4, 8), (8, 16)]:
             logger.info("%s CAUSAL TEST %s", "=" * 33, "=" * 33)
             logger.info("WIDTH = HEIGHT = %s", wh)
             logger.info("Identifying")
             base_test_case = BaseTestCase(treatment_variable=intensity, outcome_variable=num_shapes_unit)
             causal_test_case = CausalTestCase(
                 base_test_case=base_test_case,
-                expected_causal_effect=ExactValue(4, tolerance=0.5),
+                expected_causal_effect=ExactValue(4, atol=0.5),
                 treatment_value=treatment_value,
                 control_value=control_value,
                 estimate_type="risk_ratio",
             )
             obs_causal_test_result = causal_test_intensity_num_shapes(
                 observational_data_path,
                 causal_test_case,
```

### Comparing `causal_testing_framework-4.1.0/images/workflow.png` & `causal_testing_framework-4.2.0/images/workflow.png`

 * *Files identical despite different names*

### Comparing `causal_testing_framework-4.1.0/pyproject.toml` & `causal_testing_framework-4.2.0/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -11,26 +11,26 @@
 authors = [{ name = "The CITCOM team" }]
 description = "A framework for causal testing using causal directed acyclic graphs."
 readme = "README.md"
 requires-python = ">=3.9"
 license = { text = "MIT" }
 keywords = ["causal inference", "verification"]
 dependencies = [
+    "z3_solver~=4.11.2", # z3_solver does not follow semantic versioning and tying to 4.11 introduces problems
     "econml~=0.12",
     "fitter~=1.4",
     "lhsmdu~=1.1",
     "networkx~=2.6",
-    "numpy~=1.22",
+    "numpy~=1.22.0",
     "pandas~=1.3",
     "scikit_learn~=1.1",
     "scipy~=1.7",
     "statsmodels~=0.13",
-    "tabulate~=0.8",
-    "z3_solver~=4.11.2",
-] # z3_solver does not follow semantic versioning and tying to 4.11 introduces problems
+    "tabulate~=0.8"
+]
 dynamic = ["version"]
 
 [project.optional-dependencies]
 dev = [
     "autopep8",
     "isort",
     "pytest",
```

### Comparing `causal_testing_framework-4.1.0/tests/data/nhefs.csv` & `causal_testing_framework-4.2.0/tests/data/nhefs.csv`

 * *Files identical despite different names*

### Comparing `causal_testing_framework-4.1.0/tests/data_collection_tests/test_observational_data_collector.py` & `causal_testing_framework-4.2.0/tests/data_collection_tests/test_observational_data_collector.py`

 * *Files identical despite different names*

### Comparing `causal_testing_framework-4.1.0/tests/generation_tests/test_abstract_test_case.py` & `causal_testing_framework-4.2.0/tests/generation_tests/test_abstract_test_case.py`

 * *Files identical despite different names*

### Comparing `causal_testing_framework-4.1.0/tests/json_front_tests/test_json_class.py` & `causal_testing_framework-4.2.0/tests/json_front_tests/test_json_class.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,12 @@
 import unittest
 from pathlib import Path
 from statistics import StatisticsError
 import scipy
 
-
 from causal_testing.testing.estimators import LinearRegressionEstimator
 from causal_testing.testing.causal_test_outcome import NoEffect, Positive
 from tests.test_helpers import remove_temp_dir_if_existent
 from causal_testing.json_front.json_class import JsonUtility, CausalVariables
 from causal_testing.specification.variable import Input, Output, Meta
 from causal_testing.specification.scenario import Scenario
 from causal_testing.specification.causal_specification import CausalSpecification
@@ -39,14 +38,19 @@
         variables = CausalVariables(
             inputs=self.input_dict_list, outputs=self.output_dict_list, metas=self.meta_dict_list
         )
         self.scenario = Scenario(variables=variables, constraints=None)
         self.json_class.set_paths(self.json_path, self.dag_path, self.data_path)
         self.json_class.setup(self.scenario)
 
+    def test_setting_no_path(self):
+        json_class = JsonUtility("temp_out.txt", True)
+        json_class.set_paths(self.json_path, self.dag_path, None)
+        self.assertEqual(json_class.input_paths.data_paths, [])  # Needs to be list of Paths
+
     def test_setting_paths(self):
         self.assertEqual(self.json_class.input_paths.json_path, Path(self.json_path))
         self.assertEqual(self.json_class.input_paths.dag_path, Path(self.dag_path))
         self.assertEqual(self.json_class.input_paths.data_paths, [Path(self.data_path[0])])  # Needs to be list of Paths
 
     def test_set_inputs(self):
         ctf_input = [Input("test_input", float, self.example_distribution)]
@@ -90,15 +94,15 @@
                 }
             ]
         }
         self.json_class.test_plan = example_test
         effects = {"NoEffect": NoEffect()}
         mutates = {
             "Increase": lambda x: self.json_class.scenario.treatment_variables[x].z3
-            > self.json_class.scenario.variables[x].z3
+                                  > self.json_class.scenario.variables[x].z3
         }
         estimators = {"LinearRegressionEstimator": LinearRegressionEstimator}
         with self.assertRaises(StatisticsError):
             self.json_class.run_json_tests(effects, estimators, True, mutates)
 
     def test_generate_coefficient_tests_from_json(self):
         example_test = {
@@ -139,15 +143,15 @@
                 }
             ]
         }
         self.json_class.test_plan = example_test
         effects = {"NoEffect": NoEffect()}
         mutates = {
             "Increase": lambda x: self.json_class.scenario.treatment_variables[x].z3
-            > self.json_class.scenario.variables[x].z3
+                                  > self.json_class.scenario.variables[x].z3
         }
         estimators = {"LinearRegressionEstimator": LinearRegressionEstimator}
 
         self.json_class.run_json_tests(effects=effects, estimators=estimators, f_flag=False, mutates=mutates)
 
         # Test that the final log message prints that failed tests are printed, which is expected behaviour for this
         # scenario
@@ -169,15 +173,15 @@
                 }
             ]
         }
         self.json_class.test_plan = example_test
         effects = {"NoEffect": NoEffect()}
         mutates = {
             "Increase": lambda x: self.json_class.scenario.treatment_variables[x].z3
-            > self.json_class.scenario.variables[x].z3
+                                  > self.json_class.scenario.variables[x].z3
         }
         estimators = {"LinearRegressionEstimator": LinearRegressionEstimator}
 
         self.json_class.run_json_tests(effects=effects, mutates=mutates, estimators=estimators, f_flag=False)
 
         # Test that the final log message prints that failed tests are printed, which is expected behaviour for this scenario
         with open("temp_out.txt", "r") as reader:
@@ -199,15 +203,15 @@
                 }
             ]
         }
         self.json_class.test_plan = example_test
         effects = {"Positive": Positive()}
         mutates = {
             "Increase": lambda x: self.json_class.scenario.treatment_variables[x].z3
-            > self.json_class.scenario.variables[x].z3
+                                  > self.json_class.scenario.variables[x].z3
         }
         estimators = {"LinearRegressionEstimator": LinearRegressionEstimator}
 
         self.json_class.run_json_tests(effects=effects, mutates=mutates, estimators=estimators, f_flag=False)
         with open("temp_out.txt", "r") as reader:
             temp_out = reader.readlines()
         self.assertIn("test_output ~ test_input", "".join(temp_out))
@@ -232,13 +236,33 @@
         estimators = {"LinearRegressionEstimator": LinearRegressionEstimator}
 
         self.json_class.run_json_tests(effects=effects, estimators=estimators, f_flag=False)
         with open("temp_out.txt", "r") as reader:
             temp_out = reader.readlines()
         self.assertIn("FAILED", temp_out[-1])
 
+    def test_no_data_provided(self):
+        example_test = {
+            "tests": [
+                {
+                    "name": "test1",
+                    "mutations": {"test_input": "Increase"},
+                    "estimator": "LinearRegressionEstimator",
+                    "estimate_type": "ate",
+                    "effect_modifiers": [],
+                    "expected_effect": {"test_output": "NoEffect"},
+                    "skip": False,
+                }
+            ]
+        }
+        json_class = JsonUtility("temp_out.txt", True)
+        json_class.set_paths(self.json_path, self.dag_path)
+
+        with self.assertRaises(ValueError):
+            json_class.setup(self.scenario)
+
     def tearDown(self) -> None:
         remove_temp_dir_if_existent()
 
 
 def populate_example(*args, **kwargs):
     pass
```

### Comparing `causal_testing_framework-4.1.0/tests/specification_tests/test_causal_dag.py` & `causal_testing_framework-4.2.0/tests/specification_tests/test_causal_dag.py`

 * *Files identical despite different names*

### Comparing `causal_testing_framework-4.1.0/tests/specification_tests/test_metamorphic_relations.py` & `causal_testing_framework-4.2.0/tests/specification_tests/test_metamorphic_relations.py`

 * *Files 2% similar despite different names*

```diff
@@ -112,16 +112,18 @@
         self.assertEqual(
             should_not_cause_MR.to_json_stub(),
             {
                 "effect": "direct",
                 "estimate_type": "coefficient",
                 "estimator": "LinearRegressionEstimator",
                 "expected_effect": {"Z": "NoEffect"},
+                "formula": "Z ~ X1",
                 "mutations": ["X1"],
                 "name": "X1 _||_ Z",
+                "formula": "Z ~ X1",
                 "skip": True,
             },
         )
 
     def test_should_cause_json_stub(self):
         """Test if the ShouldCause MR passes all metamorphic tests where the DAG perfectly represents the program
         and there is only a single input."""
@@ -135,14 +137,15 @@
         self.assertEqual(
             should_cause_MR.to_json_stub(),
             {
                 "effect": "direct",
                 "estimate_type": "coefficient",
                 "estimator": "LinearRegressionEstimator",
                 "expected_effect": {"Z": "SomeEffect"},
+                "formula": "Z ~ X1",
                 "mutations": ["X1"],
                 "name": "X1 --> Z",
                 "skip": True,
             },
         )
 
     def test_should_cause_metamorphic_relations_correct_spec_one_input(self):
```

### Comparing `causal_testing_framework-4.1.0/tests/specification_tests/test_variable.py` & `causal_testing_framework-4.2.0/tests/specification_tests/test_variable.py`

 * *Files identical despite different names*

### Comparing `causal_testing_framework-4.1.0/tests/test_helpers.py` & `causal_testing_framework-4.2.0/tests/test_helpers.py`

 * *Files identical despite different names*

### Comparing `causal_testing_framework-4.1.0/tests/testing_tests/test_causal_test_case.py` & `causal_testing_framework-4.2.0/tests/testing_tests/test_causal_test_case.py`

 * *Files identical despite different names*

### Comparing `causal_testing_framework-4.1.0/tests/testing_tests/test_causal_test_engine.py` & `causal_testing_framework-4.2.0/tests/testing_tests/test_causal_test_engine.py`

 * *Files 2% similar despite different names*

```diff
@@ -185,48 +185,47 @@
             "D",
             self.treatment_value,
             self.control_value,
             self.minimal_adjustment_set,
             "A",
             self.causal_test_engine.scenario_execution_data_df,
         )
-        causal_test_result = self.causal_test_engine.execute_test(
-            estimation_model, self.causal_test_case, estimate_type="coefficient"
-        )
+        self.causal_test_case.estimate_type = "coefficient"
+        causal_test_result = self.causal_test_engine.execute_test(estimation_model, self.causal_test_case)
         self.assertEqual(int(causal_test_result.test_value.value), 0)
 
     def test_execute_test_observational_linear_regression_estimator_risk_ratio(self):
         """Check that executing the causal test case returns the correct results for dummy data using a linear
         regression estimator."""
         estimation_model = LinearRegressionEstimator(
             "D",
             self.treatment_value,
             self.control_value,
             self.minimal_adjustment_set,
             "A",
             self.causal_test_engine.scenario_execution_data_df,
         )
-        causal_test_result = self.causal_test_engine.execute_test(
-            estimation_model, self.causal_test_case, estimate_type="risk_ratio"
-        )
+        self.causal_test_case.estimate_type = "risk_ratio"
+        causal_test_result = self.causal_test_engine.execute_test(estimation_model, self.causal_test_case)
         self.assertEqual(int(causal_test_result.test_value.value), 0)
 
     def test_invalid_estimate_type(self):
         """Check that executing the causal test case returns the correct results for dummy data using a linear
         regression estimator."""
         estimation_model = LinearRegressionEstimator(
             "D",
             self.treatment_value,
             self.control_value,
             self.minimal_adjustment_set,
             "A",
             self.causal_test_engine.scenario_execution_data_df,
         )
+        self.causal_test_case.estimate_type = "invalid"
         with self.assertRaises(ValueError):
-            self.causal_test_engine.execute_test(estimation_model, self.causal_test_case, estimate_type="invalid")
+            self.causal_test_engine.execute_test(estimation_model, self.causal_test_case)
 
     def test_execute_test_observational_linear_regression_estimator_squared_term(self):
         """Check that executing the causal test case returns the correct results for dummy data with a squared term
         using a linear regression estimator. C ~ 4*(A+2) + D + D^2"""
         estimation_model = LinearRegressionEstimator(
             "A",
             self.treatment_value,
@@ -254,17 +253,16 @@
             self.treatment_value,
             self.control_value,
             self.minimal_adjustment_set,
             "C",
             self.causal_test_engine.scenario_execution_data_df,
             effect_modifiers={"M": None},
         )
-        causal_test_result = self.causal_test_engine.execute_test(
-            estimation_model, self.causal_test_case, estimate_type="cate"
-        )
+        self.causal_test_case.estimate_type = "cate"
+        causal_test_result = self.causal_test_engine.execute_test(estimation_model, self.causal_test_case)
         causal_test_result = causal_test_result.test_value.value
         # Check that each effect modifier's strata has a greater ATE than the last (ascending order)
         causal_test_result_m1 = causal_test_result.loc[causal_test_result["M"] == 1]
         causal_test_result_m2 = causal_test_result.loc[causal_test_result["M"] == 2]
         causal_test_result_m3 = causal_test_result.loc[causal_test_result["M"] == 3]
         causal_test_result_m4 = causal_test_result.loc[causal_test_result["M"] == 4]
         self.assertLess(causal_test_result_m1["cate"].mean(), causal_test_result_m2["cate"].mean())
```

### Comparing `causal_testing_framework-4.1.0/tests/testing_tests/test_causal_test_outcome.py` & `causal_testing_framework-4.2.0/tests/testing_tests/test_causal_test_outcome.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 import unittest
 from causal_testing.testing.causal_test_outcome import ExactValue, SomeEffect, Positive, Negative, NoEffect
 from causal_testing.testing.causal_test_result import CausalTestResult, TestValue
 from causal_testing.testing.estimators import LinearRegressionEstimator
-from causal_testing.testing.validation import CausalValidator
+from causal_testing.utils.validation import CausalValidator
 
 
 class TestCausalTestOutcome(unittest.TestCase):
     """Test the TestCausalTestOutcome basic methods."""
 
     def setUp(self) -> None:
         self.estimator = LinearRegressionEstimator(
@@ -60,25 +60,36 @@
                 "Treatment value: 1\n"
                 "Outcome: A\n"
                 "Adjustment set: set()\n"
                 "ate: 0\n"
             ),
         )
 
-    def test_Positive_pass(self):
+    def test_Positive_ate_pass(self):
         test_value = TestValue(type="ate", value=5.05)
         ctr = CausalTestResult(
             estimator=self.estimator,
             test_value=test_value,
             confidence_intervals=None,
             effect_modifier_configuration=None,
         )
         ev = Positive()
         self.assertTrue(ev.apply(ctr))
 
+    def test_Positive_risk_ratio_pass(self):
+        test_value = TestValue(type="risk_ratio", value=2)
+        ctr = CausalTestResult(
+            estimator=self.estimator,
+            test_value=test_value,
+            confidence_intervals=None,
+            effect_modifier_configuration=None,
+        )
+        ev = Positive()
+        self.assertTrue(ev.apply(ctr))
+
     def test_Positive_fail(self):
         test_value = TestValue(type="ate", value=0)
         ctr = CausalTestResult(
             estimator=self.estimator,
             test_value=test_value,
             confidence_intervals=None,
             effect_modifier_configuration=None,
@@ -93,25 +104,36 @@
             test_value=test_value,
             confidence_intervals=[-1, 1],
             effect_modifier_configuration=None,
         )
         ev = Positive()
         self.assertFalse(ev.apply(ctr))
 
-    def test_Negative_pass(self):
+    def test_Negative_ate_pass(self):
         test_value = TestValue(type="ate", value=-5.05)
         ctr = CausalTestResult(
             estimator=self.estimator,
             test_value=test_value,
             confidence_intervals=None,
             effect_modifier_configuration=None,
         )
         ev = Negative()
         self.assertTrue(ev.apply(ctr))
 
+    def test_Negative_risk_ratio_pass(self):
+        test_value = TestValue(type="risk_ratio", value=0.2)
+        ctr = CausalTestResult(
+            estimator=self.estimator,
+            test_value=test_value,
+            confidence_intervals=None,
+            effect_modifier_configuration=None,
+        )
+        ev = Negative()
+        self.assertTrue(ev.apply(ctr))
+
     def test_Negative_fail(self):
         test_value = TestValue(type="ate", value=0)
         ctr = CausalTestResult(
             estimator=self.estimator,
             test_value=test_value,
             confidence_intervals=None,
             effect_modifier_configuration=None,
@@ -159,25 +181,41 @@
             test_value=test_value,
             confidence_intervals=None,
             effect_modifier_configuration=None,
         )
         ev = ExactValue(5, 0.1)
         self.assertFalse(ev.apply(ctr))
 
-    def test_someEffect_invalid(self):
+    def test_invalid(self):
         test_value = TestValue(type="invalid", value=5.05)
         ctr = CausalTestResult(
             estimator=self.estimator,
             test_value=test_value,
             confidence_intervals=[4.8, 6.7],
             effect_modifier_configuration=None,
         )
-        ev = SomeEffect()
         with self.assertRaises(ValueError):
-            ev.apply(ctr)
+            SomeEffect().apply(ctr)
+        with self.assertRaises(ValueError):
+            NoEffect().apply(ctr)
+        with self.assertRaises(ValueError):
+            Positive().apply(ctr)
+        with self.assertRaises(ValueError):
+            Negative().apply(ctr)
+
+    def test_someEffect_pass_coefficient(self):
+        test_value = TestValue(type="coefficient", value=5.05)
+        ctr = CausalTestResult(
+            estimator=self.estimator,
+            test_value=test_value,
+            confidence_intervals=[4.8, 6.7],
+            effect_modifier_configuration=None,
+        )
+        self.assertTrue(SomeEffect().apply(ctr))
+        self.assertFalse(NoEffect().apply(ctr))
 
     def test_someEffect_pass_ate(self):
         test_value = TestValue(type="ate", value=5.05)
         ctr = CausalTestResult(
             estimator=self.estimator,
             test_value=test_value,
             confidence_intervals=[4.8, 6.7],
```

### Comparing `causal_testing_framework-4.1.0/tests/testing_tests/test_causal_test_suite.py` & `causal_testing_framework-4.2.0/tests/testing_tests/test_causal_test_suite.py`

 * *Files identical despite different names*

### Comparing `causal_testing_framework-4.1.0/tests/testing_tests/test_estimators.py` & `causal_testing_framework-4.2.0/tests/testing_tests/test_estimators.py`

 * *Files 2% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 from causal_testing.testing.estimators import (
     LinearRegressionEstimator,
     CausalForestEstimator,
     LogisticRegressionEstimator,
     InstrumentalVariableEstimator,
 )
 from causal_testing.specification.variable import Input
-from causal_testing.testing.validation import CausalValidator
+from causal_testing.utils.validation import CausalValidator
 
 
 def plot_results_df(df):
     """A helper method to plot results dataframe for estimators, where the df parameter must have columns for the cate,
     ci_low, and ci_high.
 
     :param df: A dataframe containing the columns cate, ci_low, and ci_high, where each row is an observation.
@@ -89,14 +89,22 @@
                 {"length_in": 82, "large_gauge": 1, "color": "grey", "completed": 1},
                 {"length_in": 82, "large_gauge": 0, "color": "brown", "completed": 0},
                 {"length_in": 82, "large_gauge": 0, "color": "orange", "completed": 0},
                 {"length_in": 82, "large_gauge": 1, "color": "brown", "completed": 0},
             ]
         )
 
+    # Yes, this probably shouldn't be in here, but it uses the scarf data so it makes more sense to put it
+    # here than duplicating the scarf data for a single test
+    def test_linear_regression_categorical_ate(self):
+        df = self.scarf_df.copy()
+        logistic_regression_estimator = LinearRegressionEstimator("color", None, None, set(), "completed", df)
+        ate, confidence = logistic_regression_estimator.estimate_unit_ate()
+        self.assertTrue(all([ci_low < 0 < ci_high for ci_low, ci_high in zip(confidence[0], confidence[1])]))
+
     def test_ate(self):
         df = self.scarf_df.copy()
         logistic_regression_estimator = LogisticRegressionEstimator("length_in", 65, 55, set(), "completed", df)
         ate, _ = logistic_regression_estimator.estimate_ate()
         self.assertEqual(round(ate, 4), -0.1987)
 
     def test_risk_ratio(self):
@@ -208,15 +216,14 @@
     def test_program_11_2(self):
         """Test whether our linear regression implementation produces the same results as program 11.2 (p. 141)."""
         df = self.chapter_11_df
         linear_regression_estimator = LinearRegressionEstimator("treatments", None, None, set(), "outcomes", df)
         model = linear_regression_estimator._run_linear_regression()
         ate, _ = linear_regression_estimator.estimate_unit_ate()
 
-        print(model.summary())
         self.assertEqual(round(model.params["Intercept"] + 90 * model.params["treatments"], 1), 216.9)
 
         # Increasing treatments from 90 to 100 should be the same as 10 times the unit ATE
         self.assertEqual(round(model.params["treatments"], 1), round(ate, 1))
 
     def test_program_11_3(self):
         """Test whether our linear regression implementation produces the same results as program 11.3 (p. 144)."""
```

