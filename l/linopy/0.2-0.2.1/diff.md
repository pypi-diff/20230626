# Comparing `tmp/linopy-0.2.tar.gz` & `tmp/linopy-0.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "linopy-0.2.tar", last modified: Fri Jun 23 13:03:08 2023, max compression
+gzip compressed data, was "linopy-0.2.1.tar", last modified: Mon Jun 26 14:27:42 2023, max compression
```

## Comparing `linopy-0.2.tar` & `linopy-0.2.1.tar`

### file list

```diff
@@ -1,148 +1,148 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 13:03:08.100946 linopy-0.2/
--rw-r--r--   0 runner    (1001) docker     (123)   180224 2023-06-23 13:02:58.000000 linopy-0.2/.coverage
--rw-r--r--   0 runner    (1001) docker     (123)       67 2023-06-23 13:02:58.000000 linopy-0.2/.coveragerc
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 13:03:08.084946 linopy-0.2/.github/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 13:03:08.084946 linopy-0.2/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)     1802 2023-06-23 13:02:58.000000 linopy-0.2/.github/workflows/CI.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      837 2023-06-23 13:02:58.000000 linopy-0.2/.github/workflows/deploy.yml
--rw-r--r--   0 runner    (1001) docker     (123)      399 2023-06-23 13:02:58.000000 linopy-0.2/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)     1228 2023-06-23 13:02:58.000000 linopy-0.2/.pre-commit-config.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      119 2023-06-23 13:02:58.000000 linopy-0.2/.readthedocs.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      137 2023-06-23 13:02:58.000000 linopy-0.2/CONTRIBUTING.md
--rw-r--r--   0 runner    (1001) docker     (123)     1075 2023-06-23 13:02:58.000000 linopy-0.2/LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (123)     3478 2023-06-23 13:03:08.100946 linopy-0.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2786 2023-06-23 13:02:58.000000 linopy-0.2/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 13:03:08.088946 linopy-0.2/benchmark/
--rw-r--r--   0 runner    (1001) docker     (123)     2857 2023-06-23 13:02:58.000000 linopy-0.2/benchmark/README.md
--rw-r--r--   0 runner    (1001) docker     (123)     7509 2023-06-23 13:02:58.000000 linopy-0.2/benchmark/Snakefile
--rw-r--r--   0 runner    (1001) docker     (123)    21144 2023-06-23 13:02:58.000000 linopy-0.2/benchmark/benchmark-absolute.pdf
--rw-r--r--   0 runner    (1001) docker     (123)   188981 2023-06-23 13:02:58.000000 linopy-0.2/benchmark/benchmark-absolute.png
--rw-r--r--   0 runner    (1001) docker     (123)    20512 2023-06-23 13:02:58.000000 linopy-0.2/benchmark/benchmark-overhead.pdf
--rw-r--r--   0 runner    (1001) docker     (123)   179946 2023-06-23 13:02:58.000000 linopy-0.2/benchmark/benchmark-overhead.png
--rw-r--r--   0 runner    (1001) docker     (123)    18784 2023-06-23 13:02:58.000000 linopy-0.2/benchmark/benchmark_resource-absolute.pdf
--rw-r--r--   0 runner    (1001) docker     (123)   149975 2023-06-23 13:02:58.000000 linopy-0.2/benchmark/benchmark_resource-absolute.png
--rw-r--r--   0 runner    (1001) docker     (123)    18038 2023-06-23 13:02:58.000000 linopy-0.2/benchmark/benchmark_resource-overhead.pdf
--rw-r--r--   0 runner    (1001) docker     (123)   132957 2023-06-23 13:02:58.000000 linopy-0.2/benchmark/benchmark_resource-overhead.png
--rw-r--r--   0 runner    (1001) docker     (123)      339 2023-06-23 13:02:58.000000 linopy-0.2/benchmark/config.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     7011 2023-06-23 13:02:58.000000 linopy-0.2/benchmark/environment.fixed.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      249 2023-06-23 13:02:58.000000 linopy-0.2/benchmark/environment.yaml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 13:03:08.088946 linopy-0.2/benchmark/notebooks/
--rw-r--r--   0 runner    (1001) docker     (123)     3362 2023-06-23 13:02:58.000000 linopy-0.2/benchmark/notebooks/plot-benchmarks.py.ipynb
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 13:03:08.088946 linopy-0.2/benchmark/scripts/
--rwxr-xr-x   0 runner    (1001) docker     (123)     1450 2023-06-23 13:02:58.000000 linopy-0.2/benchmark/scripts/benchmark_cvxpy.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1537 2023-06-23 13:02:58.000000 linopy-0.2/benchmark/scripts/benchmark_gurobipy.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1541 2023-06-23 13:02:58.000000 linopy-0.2/benchmark/scripts/benchmark_jump.jl
--rwxr-xr-x   0 runner    (1001) docker     (123)     1458 2023-06-23 13:02:58.000000 linopy-0.2/benchmark/scripts/benchmark_linopy.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     2007 2023-06-23 13:02:58.000000 linopy-0.2/benchmark/scripts/benchmark_ortools.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1796 2023-06-23 13:02:58.000000 linopy-0.2/benchmark/scripts/benchmark_pulp.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     2043 2023-06-23 13:02:58.000000 linopy-0.2/benchmark/scripts/benchmark_pyomo.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 13:03:08.092946 linopy-0.2/benchmark/scripts/benchmarks-pypsa-eur/
--rw-r--r--   0 runner    (1001) docker     (123)      451 2023-06-23 13:02:58.000000 linopy-0.2/benchmark/scripts/benchmarks-pypsa-eur/benchmark-linopy.py
--rw-r--r--   0 runner    (1001) docker     (123)      503 2023-06-23 13:02:58.000000 linopy-0.2/benchmark/scripts/benchmarks-pypsa-eur/benchmark-pyomo.py
--rw-r--r--   0 runner    (1001) docker     (123)      477 2023-06-23 13:02:58.000000 linopy-0.2/benchmark/scripts/benchmarks-pypsa-eur/benchmark-pypsa-linopf.py
--rw-r--r--   0 runner    (1001) docker     (123)      247 2023-06-23 13:02:58.000000 linopy-0.2/benchmark/scripts/benchmarks-pypsa-eur/common.py
--rw-r--r--   0 runner    (1001) docker     (123)      708 2023-06-23 13:02:58.000000 linopy-0.2/benchmark/scripts/benchmarks-pypsa-eur/plot-benchmarks.py
--rwxr-xr-x   0 runner    (1001) docker     (123)      469 2023-06-23 13:02:58.000000 linopy-0.2/benchmark/scripts/common.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1050 2023-06-23 13:02:58.000000 linopy-0.2/benchmark/scripts/concat-benchmarks.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 13:03:08.092946 linopy-0.2/benchmark/scripts/leftovers/
--rw-r--r--   0 runner    (1001) docker     (123)      698 2023-06-23 13:02:58.000000 linopy-0.2/benchmark/scripts/leftovers/benchmark-linopy.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 13:03:08.092946 linopy-0.2/benchmark/scripts/leftovers/benchmarks-pypsa-eur/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 13:03:08.092946 linopy-0.2/benchmark/scripts/leftovers/benchmarks-pypsa-eur/__pycache__/
--rw-r--r--   0 runner    (1001) docker     (123)      742 2023-06-23 13:02:58.000000 linopy-0.2/benchmark/scripts/leftovers/benchmarks-pypsa-eur/__pycache__/benchmark-linopy.cpython-310.pyc
--rw-r--r--   0 runner    (1001) docker     (123)      777 2023-06-23 13:02:58.000000 linopy-0.2/benchmark/scripts/leftovers/benchmarks-pypsa-eur/__pycache__/benchmark-pyomo.cpython-310.pyc
--rw-r--r--   0 runner    (1001) docker     (123)      764 2023-06-23 13:02:58.000000 linopy-0.2/benchmark/scripts/leftovers/benchmarks-pypsa-eur/__pycache__/benchmark-pypsa-linopf.cpython-310.pyc
--rw-r--r--   0 runner    (1001) docker     (123)      380 2023-06-23 13:02:58.000000 linopy-0.2/benchmark/scripts/leftovers/benchmarks-pypsa-eur/__pycache__/common.cpython-39.pyc
--rw-r--r--   0 runner    (1001) docker     (123)      909 2023-06-23 13:02:58.000000 linopy-0.2/benchmark/scripts/leftovers/benchmarks-pypsa-eur/__pycache__/plot-benchmarks.cpython-310.pyc
--rw-r--r--   0 runner    (1001) docker     (123)    18477 2023-06-23 13:02:58.000000 linopy-0.2/benchmark/scripts/leftovers/benchmarks-pypsa-eur/benchmark-linopy-pypsa-eur.dat
--rw-r--r--   0 runner    (1001) docker     (123)      451 2023-06-23 13:02:58.000000 linopy-0.2/benchmark/scripts/leftovers/benchmarks-pypsa-eur/benchmark-linopy.py
--rw-r--r--   0 runner    (1001) docker     (123)   103087 2023-06-23 13:02:58.000000 linopy-0.2/benchmark/scripts/leftovers/benchmarks-pypsa-eur/benchmark-pyomo-pypsa-eur.dat
--rw-r--r--   0 runner    (1001) docker     (123)      503 2023-06-23 13:02:58.000000 linopy-0.2/benchmark/scripts/leftovers/benchmarks-pypsa-eur/benchmark-pyomo.py
--rw-r--r--   0 runner    (1001) docker     (123)    26681 2023-06-23 13:02:58.000000 linopy-0.2/benchmark/scripts/leftovers/benchmarks-pypsa-eur/benchmark-pypsa-eur-with-pypsa.pdf
--rw-r--r--   0 runner    (1001) docker     (123)    18332 2023-06-23 13:02:58.000000 linopy-0.2/benchmark/scripts/leftovers/benchmarks-pypsa-eur/benchmark-pypsa-eur.pdf
--rw-r--r--   0 runner    (1001) docker     (123)      477 2023-06-23 13:02:58.000000 linopy-0.2/benchmark/scripts/leftovers/benchmarks-pypsa-eur/benchmark-pypsa-linopf.py
--rw-r--r--   0 runner    (1001) docker     (123)   381819 2023-06-23 13:02:58.000000 linopy-0.2/benchmark/scripts/leftovers/benchmarks-pypsa-eur/benchmark-pypsa_linopf-pypsa-eur.dat
--rw-r--r--   0 runner    (1001) docker     (123)      247 2023-06-23 13:02:58.000000 linopy-0.2/benchmark/scripts/leftovers/benchmarks-pypsa-eur/common.py
--rw-r--r--   0 runner    (1001) docker     (123)      708 2023-06-23 13:02:58.000000 linopy-0.2/benchmark/scripts/leftovers/benchmarks-pypsa-eur/plot-benchmarks.py
--rw-r--r--   0 runner    (1001) docker     (123)     1471 2023-06-23 13:02:58.000000 linopy-0.2/benchmark/scripts/leftovers/common.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1392 2023-06-23 13:02:58.000000 linopy-0.2/benchmark/scripts/merge-benchmarks.py
--rw-r--r--   0 runner    (1001) docker     (123)      613 2023-06-23 13:02:58.000000 linopy-0.2/benchmark/scripts/plot-benchmarks.py
--rwxr-xr-x   0 runner    (1001) docker     (123)      291 2023-06-23 13:02:58.000000 linopy-0.2/benchmark/scripts/run-cvxpy.py
--rwxr-xr-x   0 runner    (1001) docker     (123)      291 2023-06-23 13:02:58.000000 linopy-0.2/benchmark/scripts/run-gurobipy.py
--rwxr-xr-x   0 runner    (1001) docker     (123)      399 2023-06-23 13:02:58.000000 linopy-0.2/benchmark/scripts/run-linopy.py
--rwxr-xr-x   0 runner    (1001) docker     (123)      290 2023-06-23 13:02:58.000000 linopy-0.2/benchmark/scripts/run-ortools.py
--rwxr-xr-x   0 runner    (1001) docker     (123)      287 2023-06-23 13:02:58.000000 linopy-0.2/benchmark/scripts/run-pulp.py
--rwxr-xr-x   0 runner    (1001) docker     (123)      399 2023-06-23 13:02:58.000000 linopy-0.2/benchmark/scripts/run-pyomo.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1023 2023-06-23 13:02:58.000000 linopy-0.2/benchmark/scripts/write-lp-file.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 13:03:08.096946 linopy-0.2/doc/
--rw-r--r--   0 runner    (1001) docker     (123)      634 2023-06-23 13:02:58.000000 linopy-0.2/doc/Makefile
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 13:03:08.096946 linopy-0.2/doc/_static/
--rw-r--r--   0 runner    (1001) docker     (123)     1393 2023-06-23 13:02:58.000000 linopy-0.2/doc/_static/theme_overrides.css
--rw-r--r--   0 runner    (1001) docker     (123)     3647 2023-06-23 13:02:58.000000 linopy-0.2/doc/api.rst
--rw-r--r--   0 runner    (1001) docker     (123)    57997 2023-06-23 13:02:58.000000 linopy-0.2/doc/benchmark.png
--rw-r--r--   0 runner    (1001) docker     (123)     1087 2023-06-23 13:02:58.000000 linopy-0.2/doc/benchmark.rst
--rw-r--r--   0 runner    (1001) docker     (123)     4054 2023-06-23 13:02:58.000000 linopy-0.2/doc/conf.py
--rw-r--r--   0 runner    (1001) docker     (123)     2964 2023-06-23 13:02:58.000000 linopy-0.2/doc/contributing.rst
--rw-r--r--   0 runner    (1001) docker     (123)       51 2023-06-23 13:02:58.000000 linopy-0.2/doc/create-a-model.nblink
--rw-r--r--   0 runner    (1001) docker     (123)       57 2023-06-23 13:02:58.000000 linopy-0.2/doc/creating-constraints.nblink
--rw-r--r--   0 runner    (1001) docker     (123)       55 2023-06-23 13:02:58.000000 linopy-0.2/doc/creating-variables.nblink
--rw-r--r--   0 runner    (1001) docker     (123)     3334 2023-06-23 13:02:58.000000 linopy-0.2/doc/index.rst
--rw-r--r--   0 runner    (1001) docker     (123)    80342 2023-06-23 13:02:58.000000 linopy-0.2/doc/logo.pdf
--rw-r--r--   0 runner    (1001) docker     (123)   132092 2023-06-23 13:02:58.000000 linopy-0.2/doc/logo.png
--rw-r--r--   0 runner    (1001) docker     (123)     1135 2023-06-23 13:02:58.000000 linopy-0.2/doc/logo.py
--rw-r--r--   0 runner    (1001) docker     (123)      795 2023-06-23 13:02:58.000000 linopy-0.2/doc/make.bat
--rw-r--r--   0 runner    (1001) docker     (123)       56 2023-06-23 13:02:58.000000 linopy-0.2/doc/manipulating-models.nblink
--rw-r--r--   0 runner    (1001) docker     (123)       57 2023-06-23 13:02:58.000000 linopy-0.2/doc/migrating-from-pyomo.nblink
--rw-r--r--   0 runner    (1001) docker     (123)    19583 2023-06-23 13:02:59.000000 linopy-0.2/doc/release_notes.rst
--rw-r--r--   0 runner    (1001) docker     (123)       52 2023-06-23 13:02:59.000000 linopy-0.2/doc/solve-on-remote.nblink
--rw-r--r--   0 runner    (1001) docker     (123)     1579 2023-06-23 13:02:59.000000 linopy-0.2/doc/solvers.rst
--rw-r--r--   0 runner    (1001) docker     (123)     2415 2023-06-23 13:02:59.000000 linopy-0.2/doc/syntax.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 13:03:08.096946 linopy-0.2/examples/
--rw-r--r--   0 runner    (1001) docker     (123)    10175 2023-06-23 13:02:59.000000 linopy-0.2/examples/create-a-model.ipynb
--rw-r--r--   0 runner    (1001) docker     (123)     8419 2023-06-23 13:02:59.000000 linopy-0.2/examples/creating-constraints.ipynb
--rw-r--r--   0 runner    (1001) docker     (123)    10367 2023-06-23 13:02:59.000000 linopy-0.2/examples/creating-variables.ipynb
--rw-r--r--   0 runner    (1001) docker     (123)     7586 2023-06-23 13:02:59.000000 linopy-0.2/examples/manipulating-models.ipynb
--rw-r--r--   0 runner    (1001) docker     (123)      705 2023-06-23 13:02:59.000000 linopy-0.2/examples/migrating-from-pyomo.ipynb
--rw-r--r--   0 runner    (1001) docker     (123)    27151 2023-06-23 13:02:59.000000 linopy-0.2/examples/solve-on-remote.ipynb
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 13:03:08.100946 linopy-0.2/linopy/
--rw-r--r--   0 runner    (1001) docker     (123)      720 2023-06-23 13:02:59.000000 linopy-0.2/linopy/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    10767 2023-06-23 13:02:59.000000 linopy-0.2/linopy/common.py
--rw-r--r--   0 runner    (1001) docker     (123)     1324 2023-06-23 13:02:59.000000 linopy-0.2/linopy/config.py
--rw-r--r--   0 runner    (1001) docker     (123)     6148 2023-06-23 13:02:59.000000 linopy-0.2/linopy/constants.py
--rw-r--r--   0 runner    (1001) docker     (123)    29212 2023-06-23 13:02:59.000000 linopy-0.2/linopy/constraints.py
--rw-r--r--   0 runner    (1001) docker     (123)    46449 2023-06-23 13:02:59.000000 linopy-0.2/linopy/expressions.py
--rw-r--r--   0 runner    (1001) docker     (123)    18671 2023-06-23 13:02:59.000000 linopy-0.2/linopy/io.py
--rw-r--r--   0 runner    (1001) docker     (123)     3693 2023-06-23 13:02:59.000000 linopy-0.2/linopy/matrices.py
--rw-r--r--   0 runner    (1001) docker     (123)    37414 2023-06-23 13:02:59.000000 linopy-0.2/linopy/model.py
--rw-r--r--   0 runner    (1001) docker     (123)      731 2023-06-23 13:02:59.000000 linopy-0.2/linopy/monkey_patch_xarray.py
--rw-r--r--   0 runner    (1001) docker     (123)     8138 2023-06-23 13:02:59.000000 linopy-0.2/linopy/remote.py
--rw-r--r--   0 runner    (1001) docker     (123)    20119 2023-06-23 13:02:59.000000 linopy-0.2/linopy/solvers.py
--rw-r--r--   0 runner    (1001) docker     (123)      578 2023-06-23 13:02:59.000000 linopy-0.2/linopy/testing.py
--rw-r--r--   0 runner    (1001) docker     (123)    35858 2023-06-23 13:02:59.000000 linopy-0.2/linopy/variables.py
--rw-r--r--   0 runner    (1001) docker     (123)      155 2023-06-23 13:03:08.000000 linopy-0.2/linopy/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 13:03:08.100946 linopy-0.2/linopy.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     3478 2023-06-23 13:03:08.000000 linopy-0.2/linopy.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     4364 2023-06-23 13:03:08.000000 linopy-0.2/linopy.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-23 13:03:08.000000 linopy-0.2/linopy.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      286 2023-06-23 13:03:08.000000 linopy-0.2/linopy.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        7 2023-06-23 13:03:08.000000 linopy-0.2/linopy.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      131 2023-06-23 13:02:59.000000 linopy-0.2/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-23 13:03:08.100946 linopy-0.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1963 2023-06-23 13:02:59.000000 linopy-0.2/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 13:03:08.100946 linopy-0.2/test/
--rw-r--r--   0 runner    (1001) docker     (123)     5066 2023-06-23 13:02:59.000000 linopy-0.2/test/test_common.py
--rw-r--r--   0 runner    (1001) docker     (123)    12044 2023-06-23 13:02:59.000000 linopy-0.2/test/test_constraint.py
--rw-r--r--   0 runner    (1001) docker     (123)     4721 2023-06-23 13:02:59.000000 linopy-0.2/test/test_constraints.py
--rw-r--r--   0 runner    (1001) docker     (123)     1709 2023-06-23 13:02:59.000000 linopy-0.2/test/test_inconsistency_checks.py
--rw-r--r--   0 runner    (1001) docker     (123)     2644 2023-06-23 13:02:59.000000 linopy-0.2/test/test_io.py
--rw-r--r--   0 runner    (1001) docker     (123)    17138 2023-06-23 13:02:59.000000 linopy-0.2/test/test_linear_expression.py
--rw-r--r--   0 runner    (1001) docker     (123)     1919 2023-06-23 13:02:59.000000 linopy-0.2/test/test_matrices.py
--rw-r--r--   0 runner    (1001) docker     (123)     2698 2023-06-23 13:02:59.000000 linopy-0.2/test/test_model.py
--rw-r--r--   0 runner    (1001) docker     (123)    15044 2023-06-23 13:02:59.000000 linopy-0.2/test/test_optimization.py
--rw-r--r--   0 runner    (1001) docker     (123)     1466 2023-06-23 13:02:59.000000 linopy-0.2/test/test_options.py
--rw-r--r--   0 runner    (1001) docker     (123)     3702 2023-06-23 13:02:59.000000 linopy-0.2/test/test_quadratic_expression.py
--rw-r--r--   0 runner    (1001) docker     (123)     4002 2023-06-23 13:02:59.000000 linopy-0.2/test/test_repr.py
--rw-r--r--   0 runner    (1001) docker     (123)      951 2023-06-23 13:02:59.000000 linopy-0.2/test/test_scalar_constraint.py
--rw-r--r--   0 runner    (1001) docker     (123)     2086 2023-06-23 13:02:59.000000 linopy-0.2/test/test_scalar_linear_expression.py
--rw-r--r--   0 runner    (1001) docker     (123)     4528 2023-06-23 13:02:59.000000 linopy-0.2/test/test_variable.py
--rw-r--r--   0 runner    (1001) docker     (123)     7468 2023-06-23 13:02:59.000000 linopy-0.2/test/test_variable_assignment.py
--rw-r--r--   0 runner    (1001) docker     (123)     2313 2023-06-23 13:02:59.000000 linopy-0.2/test/test_variables.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 14:27:42.676888 linopy-0.2.1/
+-rw-r--r--   0 runner    (1001) docker     (123)   180224 2023-06-26 14:27:32.000000 linopy-0.2.1/.coverage
+-rw-r--r--   0 runner    (1001) docker     (123)       67 2023-06-26 14:27:32.000000 linopy-0.2.1/.coveragerc
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 14:27:42.652886 linopy-0.2.1/.github/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 14:27:42.656886 linopy-0.2.1/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)     2230 2023-06-26 14:27:32.000000 linopy-0.2.1/.github/workflows/CI.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      837 2023-06-26 14:27:32.000000 linopy-0.2.1/.github/workflows/deploy.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      399 2023-06-26 14:27:32.000000 linopy-0.2.1/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)     1228 2023-06-26 14:27:32.000000 linopy-0.2.1/.pre-commit-config.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      119 2023-06-26 14:27:32.000000 linopy-0.2.1/.readthedocs.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      137 2023-06-26 14:27:32.000000 linopy-0.2.1/CONTRIBUTING.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1075 2023-06-26 14:27:32.000000 linopy-0.2.1/LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     3480 2023-06-26 14:27:42.676888 linopy-0.2.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2786 2023-06-26 14:27:32.000000 linopy-0.2.1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 14:27:42.660887 linopy-0.2.1/benchmark/
+-rw-r--r--   0 runner    (1001) docker     (123)     2857 2023-06-26 14:27:32.000000 linopy-0.2.1/benchmark/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)     7509 2023-06-26 14:27:32.000000 linopy-0.2.1/benchmark/Snakefile
+-rw-r--r--   0 runner    (1001) docker     (123)    21144 2023-06-26 14:27:32.000000 linopy-0.2.1/benchmark/benchmark-absolute.pdf
+-rw-r--r--   0 runner    (1001) docker     (123)   188981 2023-06-26 14:27:32.000000 linopy-0.2.1/benchmark/benchmark-absolute.png
+-rw-r--r--   0 runner    (1001) docker     (123)    20512 2023-06-26 14:27:32.000000 linopy-0.2.1/benchmark/benchmark-overhead.pdf
+-rw-r--r--   0 runner    (1001) docker     (123)   179946 2023-06-26 14:27:32.000000 linopy-0.2.1/benchmark/benchmark-overhead.png
+-rw-r--r--   0 runner    (1001) docker     (123)    18784 2023-06-26 14:27:32.000000 linopy-0.2.1/benchmark/benchmark_resource-absolute.pdf
+-rw-r--r--   0 runner    (1001) docker     (123)   149975 2023-06-26 14:27:32.000000 linopy-0.2.1/benchmark/benchmark_resource-absolute.png
+-rw-r--r--   0 runner    (1001) docker     (123)    18038 2023-06-26 14:27:32.000000 linopy-0.2.1/benchmark/benchmark_resource-overhead.pdf
+-rw-r--r--   0 runner    (1001) docker     (123)   132957 2023-06-26 14:27:32.000000 linopy-0.2.1/benchmark/benchmark_resource-overhead.png
+-rw-r--r--   0 runner    (1001) docker     (123)      339 2023-06-26 14:27:32.000000 linopy-0.2.1/benchmark/config.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     7011 2023-06-26 14:27:32.000000 linopy-0.2.1/benchmark/environment.fixed.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      249 2023-06-26 14:27:32.000000 linopy-0.2.1/benchmark/environment.yaml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 14:27:42.660887 linopy-0.2.1/benchmark/notebooks/
+-rw-r--r--   0 runner    (1001) docker     (123)     3362 2023-06-26 14:27:32.000000 linopy-0.2.1/benchmark/notebooks/plot-benchmarks.py.ipynb
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 14:27:42.660887 linopy-0.2.1/benchmark/scripts/
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1450 2023-06-26 14:27:32.000000 linopy-0.2.1/benchmark/scripts/benchmark_cvxpy.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1537 2023-06-26 14:27:32.000000 linopy-0.2.1/benchmark/scripts/benchmark_gurobipy.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1541 2023-06-26 14:27:32.000000 linopy-0.2.1/benchmark/scripts/benchmark_jump.jl
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1458 2023-06-26 14:27:32.000000 linopy-0.2.1/benchmark/scripts/benchmark_linopy.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     2007 2023-06-26 14:27:32.000000 linopy-0.2.1/benchmark/scripts/benchmark_ortools.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1796 2023-06-26 14:27:32.000000 linopy-0.2.1/benchmark/scripts/benchmark_pulp.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     2043 2023-06-26 14:27:32.000000 linopy-0.2.1/benchmark/scripts/benchmark_pyomo.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 14:27:42.660887 linopy-0.2.1/benchmark/scripts/benchmarks-pypsa-eur/
+-rw-r--r--   0 runner    (1001) docker     (123)      451 2023-06-26 14:27:32.000000 linopy-0.2.1/benchmark/scripts/benchmarks-pypsa-eur/benchmark-linopy.py
+-rw-r--r--   0 runner    (1001) docker     (123)      503 2023-06-26 14:27:32.000000 linopy-0.2.1/benchmark/scripts/benchmarks-pypsa-eur/benchmark-pyomo.py
+-rw-r--r--   0 runner    (1001) docker     (123)      477 2023-06-26 14:27:32.000000 linopy-0.2.1/benchmark/scripts/benchmarks-pypsa-eur/benchmark-pypsa-linopf.py
+-rw-r--r--   0 runner    (1001) docker     (123)      247 2023-06-26 14:27:32.000000 linopy-0.2.1/benchmark/scripts/benchmarks-pypsa-eur/common.py
+-rw-r--r--   0 runner    (1001) docker     (123)      708 2023-06-26 14:27:32.000000 linopy-0.2.1/benchmark/scripts/benchmarks-pypsa-eur/plot-benchmarks.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      469 2023-06-26 14:27:32.000000 linopy-0.2.1/benchmark/scripts/common.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1050 2023-06-26 14:27:32.000000 linopy-0.2.1/benchmark/scripts/concat-benchmarks.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 14:27:42.660887 linopy-0.2.1/benchmark/scripts/leftovers/
+-rw-r--r--   0 runner    (1001) docker     (123)      698 2023-06-26 14:27:32.000000 linopy-0.2.1/benchmark/scripts/leftovers/benchmark-linopy.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 14:27:42.664887 linopy-0.2.1/benchmark/scripts/leftovers/benchmarks-pypsa-eur/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 14:27:42.664887 linopy-0.2.1/benchmark/scripts/leftovers/benchmarks-pypsa-eur/__pycache__/
+-rw-r--r--   0 runner    (1001) docker     (123)      742 2023-06-26 14:27:32.000000 linopy-0.2.1/benchmark/scripts/leftovers/benchmarks-pypsa-eur/__pycache__/benchmark-linopy.cpython-310.pyc
+-rw-r--r--   0 runner    (1001) docker     (123)      777 2023-06-26 14:27:32.000000 linopy-0.2.1/benchmark/scripts/leftovers/benchmarks-pypsa-eur/__pycache__/benchmark-pyomo.cpython-310.pyc
+-rw-r--r--   0 runner    (1001) docker     (123)      764 2023-06-26 14:27:32.000000 linopy-0.2.1/benchmark/scripts/leftovers/benchmarks-pypsa-eur/__pycache__/benchmark-pypsa-linopf.cpython-310.pyc
+-rw-r--r--   0 runner    (1001) docker     (123)      380 2023-06-26 14:27:32.000000 linopy-0.2.1/benchmark/scripts/leftovers/benchmarks-pypsa-eur/__pycache__/common.cpython-39.pyc
+-rw-r--r--   0 runner    (1001) docker     (123)      909 2023-06-26 14:27:32.000000 linopy-0.2.1/benchmark/scripts/leftovers/benchmarks-pypsa-eur/__pycache__/plot-benchmarks.cpython-310.pyc
+-rw-r--r--   0 runner    (1001) docker     (123)    18477 2023-06-26 14:27:32.000000 linopy-0.2.1/benchmark/scripts/leftovers/benchmarks-pypsa-eur/benchmark-linopy-pypsa-eur.dat
+-rw-r--r--   0 runner    (1001) docker     (123)      451 2023-06-26 14:27:32.000000 linopy-0.2.1/benchmark/scripts/leftovers/benchmarks-pypsa-eur/benchmark-linopy.py
+-rw-r--r--   0 runner    (1001) docker     (123)   103087 2023-06-26 14:27:32.000000 linopy-0.2.1/benchmark/scripts/leftovers/benchmarks-pypsa-eur/benchmark-pyomo-pypsa-eur.dat
+-rw-r--r--   0 runner    (1001) docker     (123)      503 2023-06-26 14:27:32.000000 linopy-0.2.1/benchmark/scripts/leftovers/benchmarks-pypsa-eur/benchmark-pyomo.py
+-rw-r--r--   0 runner    (1001) docker     (123)    26681 2023-06-26 14:27:32.000000 linopy-0.2.1/benchmark/scripts/leftovers/benchmarks-pypsa-eur/benchmark-pypsa-eur-with-pypsa.pdf
+-rw-r--r--   0 runner    (1001) docker     (123)    18332 2023-06-26 14:27:32.000000 linopy-0.2.1/benchmark/scripts/leftovers/benchmarks-pypsa-eur/benchmark-pypsa-eur.pdf
+-rw-r--r--   0 runner    (1001) docker     (123)      477 2023-06-26 14:27:32.000000 linopy-0.2.1/benchmark/scripts/leftovers/benchmarks-pypsa-eur/benchmark-pypsa-linopf.py
+-rw-r--r--   0 runner    (1001) docker     (123)   381819 2023-06-26 14:27:32.000000 linopy-0.2.1/benchmark/scripts/leftovers/benchmarks-pypsa-eur/benchmark-pypsa_linopf-pypsa-eur.dat
+-rw-r--r--   0 runner    (1001) docker     (123)      247 2023-06-26 14:27:32.000000 linopy-0.2.1/benchmark/scripts/leftovers/benchmarks-pypsa-eur/common.py
+-rw-r--r--   0 runner    (1001) docker     (123)      708 2023-06-26 14:27:32.000000 linopy-0.2.1/benchmark/scripts/leftovers/benchmarks-pypsa-eur/plot-benchmarks.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1471 2023-06-26 14:27:32.000000 linopy-0.2.1/benchmark/scripts/leftovers/common.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1392 2023-06-26 14:27:32.000000 linopy-0.2.1/benchmark/scripts/merge-benchmarks.py
+-rw-r--r--   0 runner    (1001) docker     (123)      613 2023-06-26 14:27:32.000000 linopy-0.2.1/benchmark/scripts/plot-benchmarks.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      291 2023-06-26 14:27:32.000000 linopy-0.2.1/benchmark/scripts/run-cvxpy.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      291 2023-06-26 14:27:32.000000 linopy-0.2.1/benchmark/scripts/run-gurobipy.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      399 2023-06-26 14:27:32.000000 linopy-0.2.1/benchmark/scripts/run-linopy.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      290 2023-06-26 14:27:32.000000 linopy-0.2.1/benchmark/scripts/run-ortools.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      287 2023-06-26 14:27:32.000000 linopy-0.2.1/benchmark/scripts/run-pulp.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      399 2023-06-26 14:27:32.000000 linopy-0.2.1/benchmark/scripts/run-pyomo.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1023 2023-06-26 14:27:32.000000 linopy-0.2.1/benchmark/scripts/write-lp-file.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 14:27:42.668887 linopy-0.2.1/doc/
+-rw-r--r--   0 runner    (1001) docker     (123)      634 2023-06-26 14:27:32.000000 linopy-0.2.1/doc/Makefile
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 14:27:42.668887 linopy-0.2.1/doc/_static/
+-rw-r--r--   0 runner    (1001) docker     (123)     1393 2023-06-26 14:27:32.000000 linopy-0.2.1/doc/_static/theme_overrides.css
+-rw-r--r--   0 runner    (1001) docker     (123)     3647 2023-06-26 14:27:32.000000 linopy-0.2.1/doc/api.rst
+-rw-r--r--   0 runner    (1001) docker     (123)    57997 2023-06-26 14:27:32.000000 linopy-0.2.1/doc/benchmark.png
+-rw-r--r--   0 runner    (1001) docker     (123)     1087 2023-06-26 14:27:32.000000 linopy-0.2.1/doc/benchmark.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     4054 2023-06-26 14:27:32.000000 linopy-0.2.1/doc/conf.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2964 2023-06-26 14:27:32.000000 linopy-0.2.1/doc/contributing.rst
+-rw-r--r--   0 runner    (1001) docker     (123)       51 2023-06-26 14:27:32.000000 linopy-0.2.1/doc/create-a-model.nblink
+-rw-r--r--   0 runner    (1001) docker     (123)       57 2023-06-26 14:27:32.000000 linopy-0.2.1/doc/creating-constraints.nblink
+-rw-r--r--   0 runner    (1001) docker     (123)       55 2023-06-26 14:27:32.000000 linopy-0.2.1/doc/creating-variables.nblink
+-rw-r--r--   0 runner    (1001) docker     (123)     3334 2023-06-26 14:27:32.000000 linopy-0.2.1/doc/index.rst
+-rw-r--r--   0 runner    (1001) docker     (123)    80342 2023-06-26 14:27:32.000000 linopy-0.2.1/doc/logo.pdf
+-rw-r--r--   0 runner    (1001) docker     (123)   132092 2023-06-26 14:27:32.000000 linopy-0.2.1/doc/logo.png
+-rw-r--r--   0 runner    (1001) docker     (123)     1135 2023-06-26 14:27:32.000000 linopy-0.2.1/doc/logo.py
+-rw-r--r--   0 runner    (1001) docker     (123)      795 2023-06-26 14:27:32.000000 linopy-0.2.1/doc/make.bat
+-rw-r--r--   0 runner    (1001) docker     (123)       56 2023-06-26 14:27:32.000000 linopy-0.2.1/doc/manipulating-models.nblink
+-rw-r--r--   0 runner    (1001) docker     (123)       57 2023-06-26 14:27:32.000000 linopy-0.2.1/doc/migrating-from-pyomo.nblink
+-rw-r--r--   0 runner    (1001) docker     (123)    19816 2023-06-26 14:27:32.000000 linopy-0.2.1/doc/release_notes.rst
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-06-26 14:27:32.000000 linopy-0.2.1/doc/solve-on-remote.nblink
+-rw-r--r--   0 runner    (1001) docker     (123)     1579 2023-06-26 14:27:32.000000 linopy-0.2.1/doc/solvers.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     2415 2023-06-26 14:27:32.000000 linopy-0.2.1/doc/syntax.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 14:27:42.668887 linopy-0.2.1/examples/
+-rw-r--r--   0 runner    (1001) docker     (123)    10175 2023-06-26 14:27:32.000000 linopy-0.2.1/examples/create-a-model.ipynb
+-rw-r--r--   0 runner    (1001) docker     (123)     8419 2023-06-26 14:27:32.000000 linopy-0.2.1/examples/creating-constraints.ipynb
+-rw-r--r--   0 runner    (1001) docker     (123)    10367 2023-06-26 14:27:32.000000 linopy-0.2.1/examples/creating-variables.ipynb
+-rw-r--r--   0 runner    (1001) docker     (123)     7586 2023-06-26 14:27:32.000000 linopy-0.2.1/examples/manipulating-models.ipynb
+-rw-r--r--   0 runner    (1001) docker     (123)      705 2023-06-26 14:27:32.000000 linopy-0.2.1/examples/migrating-from-pyomo.ipynb
+-rw-r--r--   0 runner    (1001) docker     (123)    27151 2023-06-26 14:27:32.000000 linopy-0.2.1/examples/solve-on-remote.ipynb
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 14:27:42.672888 linopy-0.2.1/linopy/
+-rw-r--r--   0 runner    (1001) docker     (123)      741 2023-06-26 14:27:32.000000 linopy-0.2.1/linopy/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11018 2023-06-26 14:27:32.000000 linopy-0.2.1/linopy/common.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1324 2023-06-26 14:27:32.000000 linopy-0.2.1/linopy/config.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6148 2023-06-26 14:27:32.000000 linopy-0.2.1/linopy/constants.py
+-rw-r--r--   0 runner    (1001) docker     (123)    29733 2023-06-26 14:27:32.000000 linopy-0.2.1/linopy/constraints.py
+-rw-r--r--   0 runner    (1001) docker     (123)    47153 2023-06-26 14:27:32.000000 linopy-0.2.1/linopy/expressions.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18671 2023-06-26 14:27:32.000000 linopy-0.2.1/linopy/io.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3693 2023-06-26 14:27:32.000000 linopy-0.2.1/linopy/matrices.py
+-rw-r--r--   0 runner    (1001) docker     (123)    37414 2023-06-26 14:27:32.000000 linopy-0.2.1/linopy/model.py
+-rw-r--r--   0 runner    (1001) docker     (123)      731 2023-06-26 14:27:32.000000 linopy-0.2.1/linopy/monkey_patch_xarray.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8138 2023-06-26 14:27:32.000000 linopy-0.2.1/linopy/remote.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20119 2023-06-26 14:27:32.000000 linopy-0.2.1/linopy/solvers.py
+-rw-r--r--   0 runner    (1001) docker     (123)      578 2023-06-26 14:27:32.000000 linopy-0.2.1/linopy/testing.py
+-rw-r--r--   0 runner    (1001) docker     (123)    36288 2023-06-26 14:27:32.000000 linopy-0.2.1/linopy/variables.py
+-rw-r--r--   0 runner    (1001) docker     (123)      160 2023-06-26 14:27:42.000000 linopy-0.2.1/linopy/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 14:27:42.672888 linopy-0.2.1/linopy.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     3480 2023-06-26 14:27:42.000000 linopy-0.2.1/linopy.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     4364 2023-06-26 14:27:42.000000 linopy-0.2.1/linopy.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-26 14:27:42.000000 linopy-0.2.1/linopy.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      273 2023-06-26 14:27:42.000000 linopy-0.2.1/linopy.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        7 2023-06-26 14:27:42.000000 linopy-0.2.1/linopy.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      131 2023-06-26 14:27:32.000000 linopy-0.2.1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-26 14:27:42.676888 linopy-0.2.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1849 2023-06-26 14:27:32.000000 linopy-0.2.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 14:27:42.676888 linopy-0.2.1/test/
+-rw-r--r--   0 runner    (1001) docker     (123)     5066 2023-06-26 14:27:32.000000 linopy-0.2.1/test/test_common.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12044 2023-06-26 14:27:32.000000 linopy-0.2.1/test/test_constraint.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4721 2023-06-26 14:27:32.000000 linopy-0.2.1/test/test_constraints.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1709 2023-06-26 14:27:32.000000 linopy-0.2.1/test/test_inconsistency_checks.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2644 2023-06-26 14:27:32.000000 linopy-0.2.1/test/test_io.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17139 2023-06-26 14:27:32.000000 linopy-0.2.1/test/test_linear_expression.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1919 2023-06-26 14:27:32.000000 linopy-0.2.1/test/test_matrices.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2698 2023-06-26 14:27:32.000000 linopy-0.2.1/test/test_model.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15044 2023-06-26 14:27:32.000000 linopy-0.2.1/test/test_optimization.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1466 2023-06-26 14:27:32.000000 linopy-0.2.1/test/test_options.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4348 2023-06-26 14:27:32.000000 linopy-0.2.1/test/test_quadratic_expression.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4054 2023-06-26 14:27:32.000000 linopy-0.2.1/test/test_repr.py
+-rw-r--r--   0 runner    (1001) docker     (123)      951 2023-06-26 14:27:32.000000 linopy-0.2.1/test/test_scalar_constraint.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2086 2023-06-26 14:27:32.000000 linopy-0.2.1/test/test_scalar_linear_expression.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4529 2023-06-26 14:27:32.000000 linopy-0.2.1/test/test_variable.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7468 2023-06-26 14:27:32.000000 linopy-0.2.1/test/test_variable_assignment.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2313 2023-06-26 14:27:32.000000 linopy-0.2.1/test/test_variables.py
```

### Comparing `linopy-0.2/.coverage` & `linopy-0.2.1/.coverage`

 * *Files identical despite different names*

### Comparing `linopy-0.2/.github/workflows/CI.yaml` & `linopy-0.2.1/.github/workflows/CI.yaml`

 * *Files 16% similar despite different names*

```diff
@@ -11,25 +11,29 @@
 jobs:
   build:
 
     runs-on: ${{ matrix.os }}
     strategy:
       fail-fast: false
       matrix:
+        python-version:
+        - 3.8
+        - 3.9
+        - "3.10"
+        - "3.11"
         os:
         - ubuntu-latest
         - macos-latest
         - windows-latest
-
     steps:
     - uses: actions/checkout@v2
-    - name: Set up Python 3.9
-      uses: actions/setup-python@v1
+    - name: Set up Python ${{ matrix.python-version }}
+      uses: actions/setup-python@v2
       with:
-        python-version: 3.9
+        python-version: ${{ matrix.python-version }}
 
     - name: Install ubuntu dependencies
       if: matrix.os == 'ubuntu-latest'
       run: |
         sudo apt-get install glpk-utils
         sudo apt-get install coinor-cbc
         pip install highspy
@@ -46,19 +50,26 @@
           args: -h
 
     - name: Install windows dependencies
       if: matrix.os == 'windows-latest'
       run: |
         choco install glpk
 
-    - name: Install dependencies
+    - name: Install dependencies for python ${{ matrix.python-version }}
+      if: matrix.python-version == '3.11'
       run: |
         python -m pip install --upgrade pip
         pip install -e .[dev]
 
+    - name: Install dependencies for python ${{ matrix.python-version }}
+      if: matrix.python-version != '3.11'
+      run: |
+        python -m pip install --upgrade pip
+        pip install -e .[dev,solvers]
+
     - name: Lint with flake8
       run: |
         pip install flake8
         # stop the build if there are Python syntax errors or undefined names
         flake8 . --count --select=E9,F63,F7,F82 --show-source --statistics --exclude=benchmark/scripts
         # exit-zero treats all errors as warnings. The GitHub editor is 127 chars wide
         flake8 . --count --exit-zero --max-complexity=10 --max-line-length=127 --statistics
```

### Comparing `linopy-0.2/.github/workflows/deploy.yml` & `linopy-0.2.1/.github/workflows/deploy.yml`

 * *Files identical despite different names*

### Comparing `linopy-0.2/.pre-commit-config.yaml` & `linopy-0.2.1/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `linopy-0.2/LICENSE.txt` & `linopy-0.2.1/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `linopy-0.2/PKG-INFO` & `linopy-0.2.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: linopy
-Version: 0.2
+Version: 0.2.1
 Summary: Linear optimization with N-D labeled arrays in Python
 Home-page: https://github.com/PyPSA/linopy
 Author: Fabian Hofmann
 Author-email: hofmann@fias.uni-frankfurt.de
 License: MIT
 Classifier: Development Status :: 3 - Alpha
 Classifier: Environment :: Console
```

### Comparing `linopy-0.2/README.md` & `linopy-0.2.1/README.md`

 * *Files identical despite different names*

### Comparing `linopy-0.2/benchmark/README.md` & `linopy-0.2.1/benchmark/README.md`

 * *Files identical despite different names*

### Comparing `linopy-0.2/benchmark/Snakefile` & `linopy-0.2.1/benchmark/Snakefile`

 * *Files identical despite different names*

### Comparing `linopy-0.2/benchmark/benchmark-absolute.pdf` & `linopy-0.2.1/benchmark/benchmark-absolute.pdf`

 * *Files identical despite different names*

### Comparing `linopy-0.2/benchmark/benchmark-absolute.png` & `linopy-0.2.1/benchmark/benchmark-absolute.png`

 * *Files identical despite different names*

### Comparing `linopy-0.2/benchmark/benchmark-overhead.pdf` & `linopy-0.2.1/benchmark/benchmark-overhead.pdf`

 * *Files identical despite different names*

### Comparing `linopy-0.2/benchmark/benchmark-overhead.png` & `linopy-0.2.1/benchmark/benchmark-overhead.png`

 * *Files identical despite different names*

### Comparing `linopy-0.2/benchmark/benchmark_resource-absolute.pdf` & `linopy-0.2.1/benchmark/benchmark_resource-absolute.pdf`

 * *Files identical despite different names*

### Comparing `linopy-0.2/benchmark/benchmark_resource-absolute.png` & `linopy-0.2.1/benchmark/benchmark_resource-absolute.png`

 * *Files identical despite different names*

### Comparing `linopy-0.2/benchmark/benchmark_resource-overhead.pdf` & `linopy-0.2.1/benchmark/benchmark_resource-overhead.pdf`

 * *Files identical despite different names*

### Comparing `linopy-0.2/benchmark/benchmark_resource-overhead.png` & `linopy-0.2.1/benchmark/benchmark_resource-overhead.png`

 * *Files identical despite different names*

### Comparing `linopy-0.2/benchmark/environment.fixed.yaml` & `linopy-0.2.1/benchmark/environment.fixed.yaml`

 * *Files identical despite different names*

### Comparing `linopy-0.2/benchmark/notebooks/plot-benchmarks.py.ipynb` & `linopy-0.2.1/benchmark/notebooks/plot-benchmarks.py.ipynb`

 * *Files identical despite different names*

### Comparing `linopy-0.2/benchmark/scripts/benchmark_cvxpy.py` & `linopy-0.2.1/benchmark/scripts/benchmark_cvxpy.py`

 * *Files identical despite different names*

### Comparing `linopy-0.2/benchmark/scripts/benchmark_gurobipy.py` & `linopy-0.2.1/benchmark/scripts/benchmark_gurobipy.py`

 * *Files identical despite different names*

### Comparing `linopy-0.2/benchmark/scripts/benchmark_jump.jl` & `linopy-0.2.1/benchmark/scripts/benchmark_jump.jl`

 * *Files identical despite different names*

### Comparing `linopy-0.2/benchmark/scripts/benchmark_linopy.py` & `linopy-0.2.1/benchmark/scripts/benchmark_linopy.py`

 * *Files identical despite different names*

### Comparing `linopy-0.2/benchmark/scripts/benchmark_ortools.py` & `linopy-0.2.1/benchmark/scripts/benchmark_ortools.py`

 * *Files identical despite different names*

### Comparing `linopy-0.2/benchmark/scripts/benchmark_pulp.py` & `linopy-0.2.1/benchmark/scripts/benchmark_pulp.py`

 * *Files identical despite different names*

### Comparing `linopy-0.2/benchmark/scripts/benchmark_pyomo.py` & `linopy-0.2.1/benchmark/scripts/benchmark_pyomo.py`

 * *Files identical despite different names*

### Comparing `linopy-0.2/benchmark/scripts/benchmarks-pypsa-eur/plot-benchmarks.py` & `linopy-0.2.1/benchmark/scripts/benchmarks-pypsa-eur/plot-benchmarks.py`

 * *Files identical despite different names*

### Comparing `linopy-0.2/benchmark/scripts/concat-benchmarks.py` & `linopy-0.2.1/benchmark/scripts/concat-benchmarks.py`

 * *Files identical despite different names*

### Comparing `linopy-0.2/benchmark/scripts/leftovers/benchmark-linopy.py` & `linopy-0.2.1/benchmark/scripts/leftovers/benchmark-linopy.py`

 * *Files identical despite different names*

### Comparing `linopy-0.2/benchmark/scripts/leftovers/benchmarks-pypsa-eur/__pycache__/benchmark-linopy.cpython-310.pyc` & `linopy-0.2.1/benchmark/scripts/leftovers/benchmarks-pypsa-eur/__pycache__/benchmark-linopy.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `linopy-0.2/benchmark/scripts/leftovers/benchmarks-pypsa-eur/__pycache__/benchmark-pyomo.cpython-310.pyc` & `linopy-0.2.1/benchmark/scripts/leftovers/benchmarks-pypsa-eur/__pycache__/benchmark-pyomo.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `linopy-0.2/benchmark/scripts/leftovers/benchmarks-pypsa-eur/__pycache__/benchmark-pypsa-linopf.cpython-310.pyc` & `linopy-0.2.1/benchmark/scripts/leftovers/benchmarks-pypsa-eur/__pycache__/benchmark-pypsa-linopf.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `linopy-0.2/benchmark/scripts/leftovers/benchmarks-pypsa-eur/__pycache__/plot-benchmarks.cpython-310.pyc` & `linopy-0.2.1/benchmark/scripts/leftovers/benchmarks-pypsa-eur/__pycache__/plot-benchmarks.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `linopy-0.2/benchmark/scripts/leftovers/benchmarks-pypsa-eur/benchmark-linopy-pypsa-eur.dat` & `linopy-0.2.1/benchmark/scripts/leftovers/benchmarks-pypsa-eur/benchmark-linopy-pypsa-eur.dat`

 * *Files identical despite different names*

### Comparing `linopy-0.2/benchmark/scripts/leftovers/benchmarks-pypsa-eur/benchmark-pyomo-pypsa-eur.dat` & `linopy-0.2.1/benchmark/scripts/leftovers/benchmarks-pypsa-eur/benchmark-pyomo-pypsa-eur.dat`

 * *Files identical despite different names*

### Comparing `linopy-0.2/benchmark/scripts/leftovers/benchmarks-pypsa-eur/benchmark-pypsa-eur-with-pypsa.pdf` & `linopy-0.2.1/benchmark/scripts/leftovers/benchmarks-pypsa-eur/benchmark-pypsa-eur-with-pypsa.pdf`

 * *Files identical despite different names*

### Comparing `linopy-0.2/benchmark/scripts/leftovers/benchmarks-pypsa-eur/benchmark-pypsa-eur.pdf` & `linopy-0.2.1/benchmark/scripts/leftovers/benchmarks-pypsa-eur/benchmark-pypsa-eur.pdf`

 * *Files identical despite different names*

### Comparing `linopy-0.2/benchmark/scripts/leftovers/benchmarks-pypsa-eur/benchmark-pypsa_linopf-pypsa-eur.dat` & `linopy-0.2.1/benchmark/scripts/leftovers/benchmarks-pypsa-eur/benchmark-pypsa_linopf-pypsa-eur.dat`

 * *Files identical despite different names*

### Comparing `linopy-0.2/benchmark/scripts/leftovers/benchmarks-pypsa-eur/plot-benchmarks.py` & `linopy-0.2.1/benchmark/scripts/leftovers/benchmarks-pypsa-eur/plot-benchmarks.py`

 * *Files identical despite different names*

### Comparing `linopy-0.2/benchmark/scripts/leftovers/common.py` & `linopy-0.2.1/benchmark/scripts/leftovers/common.py`

 * *Files identical despite different names*

### Comparing `linopy-0.2/benchmark/scripts/merge-benchmarks.py` & `linopy-0.2.1/benchmark/scripts/merge-benchmarks.py`

 * *Files identical despite different names*

### Comparing `linopy-0.2/benchmark/scripts/plot-benchmarks.py` & `linopy-0.2.1/benchmark/scripts/plot-benchmarks.py`

 * *Files identical despite different names*

### Comparing `linopy-0.2/benchmark/scripts/write-lp-file.py` & `linopy-0.2.1/benchmark/scripts/write-lp-file.py`

 * *Files identical despite different names*

### Comparing `linopy-0.2/doc/Makefile` & `linopy-0.2.1/doc/Makefile`

 * *Files identical despite different names*

### Comparing `linopy-0.2/doc/_static/theme_overrides.css` & `linopy-0.2.1/doc/_static/theme_overrides.css`

 * *Files identical despite different names*

### Comparing `linopy-0.2/doc/api.rst` & `linopy-0.2.1/doc/api.rst`

 * *Files identical despite different names*

### Comparing `linopy-0.2/doc/benchmark.png` & `linopy-0.2.1/doc/benchmark.png`

 * *Files identical despite different names*

### Comparing `linopy-0.2/doc/benchmark.rst` & `linopy-0.2.1/doc/benchmark.rst`

 * *Files identical despite different names*

### Comparing `linopy-0.2/doc/conf.py` & `linopy-0.2.1/doc/conf.py`

 * *Files identical despite different names*

### Comparing `linopy-0.2/doc/contributing.rst` & `linopy-0.2.1/doc/contributing.rst`

 * *Files identical despite different names*

### Comparing `linopy-0.2/doc/index.rst` & `linopy-0.2.1/doc/index.rst`

 * *Files identical despite different names*

### Comparing `linopy-0.2/doc/logo.pdf` & `linopy-0.2.1/doc/logo.pdf`

 * *Files identical despite different names*

### Comparing `linopy-0.2/doc/logo.png` & `linopy-0.2.1/doc/logo.png`

 * *Files identical despite different names*

### Comparing `linopy-0.2/doc/logo.py` & `linopy-0.2.1/doc/logo.py`

 * *Files identical despite different names*

### Comparing `linopy-0.2/doc/make.bat` & `linopy-0.2.1/doc/make.bat`

 * *Files identical despite different names*

### Comparing `linopy-0.2/doc/release_notes.rst` & `linopy-0.2.1/doc/release_notes.rst`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,20 @@
 Release Notes
 =============
 
 .. Upcoming Release
 .. ----------------
 
+Version 0.2.1
+-------------
+
+
+* Backwards compatibility for python 3.8.
+* `Variable`, `LinearExpression` and `Constraint` now have a print function to easily print the objects with larger layouts, i.e. showing more terms and lines.
+
 
 Version 0.2.0
 -------------
 
 
 **New Features**
```

### Comparing `linopy-0.2/doc/solvers.rst` & `linopy-0.2.1/doc/solvers.rst`

 * *Files identical despite different names*

### Comparing `linopy-0.2/doc/syntax.rst` & `linopy-0.2.1/doc/syntax.rst`

 * *Files identical despite different names*

### Comparing `linopy-0.2/examples/create-a-model.ipynb` & `linopy-0.2.1/examples/create-a-model.ipynb`

 * *Files identical despite different names*

### Comparing `linopy-0.2/examples/creating-constraints.ipynb` & `linopy-0.2.1/examples/creating-constraints.ipynb`

 * *Files identical despite different names*

### Comparing `linopy-0.2/examples/creating-variables.ipynb` & `linopy-0.2.1/examples/creating-variables.ipynb`

 * *Files identical despite different names*

### Comparing `linopy-0.2/examples/manipulating-models.ipynb` & `linopy-0.2.1/examples/manipulating-models.ipynb`

 * *Files identical despite different names*

### Comparing `linopy-0.2/examples/migrating-from-pyomo.ipynb` & `linopy-0.2.1/examples/migrating-from-pyomo.ipynb`

 * *Files identical despite different names*

### Comparing `linopy-0.2/examples/solve-on-remote.ipynb` & `linopy-0.2.1/examples/solve-on-remote.ipynb`

 * *Files identical despite different names*

### Comparing `linopy-0.2/linopy/__init__.py` & `linopy-0.2.1/linopy/__init__.py`

 * *Files 10% similar despite different names*

```diff
@@ -9,12 +9,12 @@
 # Note: For intercepting multiplications between xarray dataarrays, Variables and Expressions
 # we need to extend their __mul__ functions with a quick special case
 import linopy.monkey_patch_xarray
 from linopy import model, remote
 from linopy.config import options
 from linopy.constants import EQUAL, GREATER_EQUAL, LESS_EQUAL
 from linopy.constraints import Constraint
-from linopy.expressions import merge
+from linopy.expressions import LinearExpression, QuadraticExpression, merge
 from linopy.io import read_netcdf
-from linopy.model import LinearExpression, Model, Variable, available_solvers
+from linopy.model import Model, Variable, available_solvers
 from linopy.remote import RemoteHandler
 from linopy.version import version as __version__
```

### Comparing `linopy-0.2/linopy/common.py` & `linopy-0.2.1/linopy/common.py`

 * *Files 2% similar despite different names*

```diff
@@ -14,15 +14,21 @@
 import numpy as np
 import pandas as pd
 from numpy import arange, hstack
 from xarray import DataArray, Dataset, align, apply_ufunc, merge
 from xarray.core import indexing, utils
 
 from linopy.config import options
-from linopy.constants import SIGNS, TERM_DIM, SIGNS_alternative, sign_replace_dict
+from linopy.constants import (
+    HELPER_DIMS,
+    SIGNS,
+    TERM_DIM,
+    SIGNS_alternative,
+    sign_replace_dict,
+)
 
 
 def maybe_replace_sign(sign):
     if sign in SIGNS_alternative:
         return sign_replace_dict[sign]
     elif sign in SIGNS:
         return sign
@@ -90,32 +96,37 @@
     except ValueError:
         warn("Coordinates across variables not equal. Perform outer join.", UserWarning)
         labels = align(*dataarrays, join="outer")
         labels = [ds.fillna(-1).astype(int) for ds in labels]
     return Dataset({ds.name: ds for ds in labels})
 
 
-def fill_missing_coords(ds):
+def fill_missing_coords(ds, fill_helper_dims=False):
     """
     Fill coordinates of a xarray Dataset or DataArray with integer coordinates.
 
     This function fills in the integer coordinates for all dimensions of a
     Dataset or DataArray that have no coordinates assigned yet.
 
     Parameters
     ----------
     ds : xarray.DataArray or xarray.Dataset
+    fill_helper_dims : bool, optional
+        Whether to fill in integer coordinates for helper dimensions, by default False.
+
     """
     ds = ds.copy()
     if not isinstance(ds, (Dataset, DataArray)):
         raise TypeError(f"Expected xarray.DataArray or xarray.Dataset, got {type(ds)}.")
 
+    skip_dims = [] if fill_helper_dims else HELPER_DIMS
+
     # Fill in missing integer coordinates
     for dim in ds.dims:
-        if dim not in ds.coords and dim != TERM_DIM:
+        if dim not in ds.coords and dim not in skip_dims:
             ds.coords[dim] = arange(ds.sizes[dim])
 
     return ds
 
 
 def _remap(array, mapping):
     return mapping[array.ravel()].reshape(array.shape)
```

### Comparing `linopy-0.2/linopy/config.py` & `linopy-0.2.1/linopy/config.py`

 * *Files identical despite different names*

### Comparing `linopy-0.2/linopy/constants.py` & `linopy-0.2.1/linopy/constants.py`

 * *Files identical despite different names*

### Comparing `linopy-0.2/linopy/constraints.py` & `linopy-0.2.1/linopy/constraints.py`

 * *Files 2% similar despite different names*

```diff
@@ -204,14 +204,31 @@
                 f"{header_string}\n{'-'*len(header_string)}\n{expr} {SIGNS_pretty[self.sign.item()]} {self.rhs.item()}"
             )
         else:
             lines.append(f"{header_string}\n{'-'*len(header_string)}\n<empty>")
 
         return "\n".join(lines)
 
+    def print(self, display_max_rows=20, display_max_terms=20):
+        """
+        Print the linear expression.
+
+        Parameters
+        ----------
+        display_max_rows : int
+            Maximum number of rows to be displayed.
+        display_max_terms : int
+            Maximum number of terms to be displayed.
+        """
+        with options as opts:
+            opts.set_value(
+                display_max_rows=display_max_rows, display_max_terms=display_max_terms
+            )
+            print(self)
+
     def __contains__(self, value):
         return self.data.__contains__(value)
 
     @property
     def type(self):
         """
         Get the type of the constraint.
@@ -454,15 +471,15 @@
             # fallback for weird error raised due to missing index
             df = pd.DataFrame({k: ds[k].item() for k in ds}, index=[0])
         else:
             df = ds.to_dataframe()
         df = df[(df.labels != -1) & (df.vars != -1) & (df.coeffs != 0)]
         # Group repeated variables in the same constraint
         agg = dict(coeffs="sum", rhs="first", sign="first")
-        agg |= {k: "first" for k in df.columns if k not in agg}
+        agg.update({k: "first" for k in df.columns if k not in agg})
         df = df.groupby(["labels", "vars"], as_index=False).aggregate(agg)
 
         any_nan = df.isna().any()
         if any_nan.any():
             fields = ", ".join("`" + df.columns[any_nan] + "`")
             raise ValueError(
                 f"Constraint `{self.name}` contains nan's in field(s) {fields}"
```

### Comparing `linopy-0.2/linopy/expressions.py` & `linopy-0.2.1/linopy/expressions.py`

 * *Files 0% similar despite different names*

```diff
@@ -164,15 +164,15 @@
 
             group_dim = group.index.name
             arrays = [group, group.groupby(group).cumcount()]
             idx = pd.MultiIndex.from_arrays(
                 arrays, names=[group_name, GROUPED_TERM_DIM]
             )
             ds = self.data.assign_coords({group_dim: idx})
-            ds = ds.unstack(group_dim, fill_value=LinearExpression.fill_value)
+            ds = ds.unstack(group_dim, fill_value=LinearExpression._fill_value)
             ds = LinearExpression._sum(ds, dims=GROUPED_TERM_DIM)
 
             if int_map is not None:
                 index = ds.indexes["group"].map({v: k for k, v in int_map.items()})
                 index.names = orig_group.columns
                 index.name = group_name
                 ds = xr.Dataset(ds.assign_coords({group_name: index}))
@@ -361,14 +361,31 @@
             )
             lines.append(f"{header_string}\n{'-'*len(header_string)}\n{expr}")
         else:
             lines.append(f"{header_string}\n{'-'*len(header_string)}\n<empty>")
 
         return "\n".join(lines)
 
+    def print(self, display_max_rows=20, display_max_terms=20):
+        """
+        Print the linear expression.
+
+        Parameters
+        ----------
+        display_max_rows : int
+            Maximum number of rows to be displayed.
+        display_max_terms : int
+            Maximum number of terms to be displayed.
+        """
+        with options as opts:
+            opts.set_value(
+                display_max_rows=display_max_rows, display_max_terms=display_max_terms
+            )
+            print(self)
+
     def __add__(self, other):
         """
         Add an expression to others.
         """
         other = as_expression(
             other, model=self.model, coords=self.coords, dims=self.coord_dims
         )
@@ -709,15 +726,15 @@
         ds = Dataset({"coeffs": coeffs, "vars": vars}).transpose(..., TERM_DIM)
 
         return cls(ds, model)
 
     def to_quadexpr(self):
         """Convert LinearExpression to QuadraticExpression."""
         vars = self.data.vars.expand_dims(FACTOR_DIM)
-        fill_value = self.fill_value["vars"]
+        fill_value = self._fill_value["vars"]
         vars = xr.concat([vars, xr.full_like(vars, fill_value)], dim=FACTOR_DIM)
         data = self.data.assign(vars=vars)
         return QuadraticExpression(data, self.model)
 
     def to_constraint(self, sign, rhs):
         """
         Convert a linear expression to a constraint.
@@ -1241,29 +1258,37 @@
 
     Returns
     -------
     res : linopy.LinearExpression
     """
     linopy_types = (variables.Variable, LinearExpression, QuadraticExpression)
 
+    if (
+        cls is QuadraticExpression
+        and dim == TERM_DIM
+        and any(type(e) is LinearExpression for e in exprs)
+    ):
+        raise ValueError(
+            "Cannot merge linear and quadratic expressions along term dimension."
+            "Convert to QuadraticExpression first."
+        )
+
     exprs = exprs[0] if len(exprs) == 1 else list(exprs)  # allow passing a list
     model = exprs[0].model
 
     if cls in linopy_types and dim in HELPER_DIMS:
         coord_dims = [
             {k: v for k, v in e.dims.items() if k not in HELPER_DIMS} for e in exprs
         ]
         override = check_common_keys_values(coord_dims)
     else:
         override = False
 
     data = [e.data if isinstance(e, linopy_types) else e for e in exprs]
-    for d in set(HELPER_DIMS) & set(_ for ds in data for _ in ds.dims):
-        if len({ds.dims[d] for ds in data}) > 1:
-            data = [ds.assign_coords({d: arange(ds.dims[d])}) for ds in data]
+    data = [fill_missing_coords(ds, fill_helper_dims=True) for ds in data]
 
     if not kwargs:
         kwargs = {
             "fill_value": cls._fill_value,
             "coords": "minimal",
             "compat": "override",
         }
```

### Comparing `linopy-0.2/linopy/io.py` & `linopy-0.2.1/linopy/io.py`

 * *Files identical despite different names*

### Comparing `linopy-0.2/linopy/matrices.py` & `linopy-0.2.1/linopy/matrices.py`

 * *Files identical despite different names*

### Comparing `linopy-0.2/linopy/model.py` & `linopy-0.2.1/linopy/model.py`

 * *Files identical despite different names*

### Comparing `linopy-0.2/linopy/monkey_patch_xarray.py` & `linopy-0.2.1/linopy/monkey_patch_xarray.py`

 * *Files identical despite different names*

### Comparing `linopy-0.2/linopy/remote.py` & `linopy-0.2.1/linopy/remote.py`

 * *Files identical despite different names*

### Comparing `linopy-0.2/linopy/solvers.py` & `linopy-0.2.1/linopy/solvers.py`

 * *Files identical despite different names*

### Comparing `linopy-0.2/linopy/testing.py` & `linopy-0.2.1/linopy/testing.py`

 * *Files identical despite different names*

### Comparing `linopy-0.2/linopy/variables.py` & `linopy-0.2.1/linopy/variables.py`

 * *Files 1% similar despite different names*

```diff
@@ -248,14 +248,29 @@
         else:
             lines.append(
                 f"Variable\n{'-'*8}\n{print_single_variable(self.model, self.labels.item())}"
             )
 
         return "\n".join(lines)
 
+    def print(self, display_max_rows=20):
+        """
+        Print the linear expression.
+
+        Parameters
+        ----------
+        display_max_rows : int
+            Maximum number of rows to be displayed.
+        display_max_terms : int
+            Maximum number of terms to be displayed.
+        """
+        with options as opts:
+            opts.set_value(display_max_rows=display_max_rows)
+            print(self)
+
     def __neg__(self):
         """
         Calculate the negative of the variables (converts coefficients only).
         """
         return self.to_linexpr(-1)
 
     def __mul__(self, other):
@@ -468,15 +483,15 @@
         The mask indicates on which coordinates the variable array is enabled
         (True) and disabled (False).
 
         Returns
         -------
         xr.DataArray
         """
-        return (self.labels != self.fill_value["labels"]).astype(bool)
+        return (self.labels != self._fill_value["labels"]).astype(bool)
 
     @property
     def upper(self):
         """
         Get the upper bounds of the variables.
 
         The function raises an error in case no model is set as a
@@ -672,15 +687,15 @@
         -------
         linopy.Variable
         """
         data = (
             self.data.where(self.labels != -1)
             # .ffill(dim, limit=limit)
             # breaks with Dataset.ffill, use map instead
-            .map(DataArray.ffill, dim=dim, limit=limit).fillna(self.fill_value)
+            .map(DataArray.ffill, dim=dim, limit=limit).fillna(self._fill_value)
         )
         data = data.assign(labels=data.labels.astype(int))
         return self.__class__(data, self.model, self.name)
 
     def bfill(self, dim, limit=None):
         """
         Backward fill the variable along a dimension.
@@ -699,15 +714,15 @@
         -------
         linopy.Variable
         """
         data = (
             self.data.where(self.labels != -1)
             # .bfill(dim, limit=limit)
             # breaks with Dataset.bfill, use map instead
-            .map(DataArray.bfill, dim=dim, limit=limit).fillna(self.fill_value)
+            .map(DataArray.bfill, dim=dim, limit=limit).fillna(self._fill_value)
         )
         data = data.assign(labels=data.labels.astype(int))
         return self.__class__(data, self.model, self.name)
 
     def sanitize(self):
         """
         Sanitize variable by ensuring int dtype with fill value of -1.
```

### Comparing `linopy-0.2/linopy.egg-info/PKG-INFO` & `linopy-0.2.1/linopy.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: linopy
-Version: 0.2
+Version: 0.2.1
 Summary: Linear optimization with N-D labeled arrays in Python
 Home-page: https://github.com/PyPSA/linopy
 Author: Fabian Hofmann
 Author-email: hofmann@fias.uni-frankfurt.de
 License: MIT
 Classifier: Development Status :: 3 - Alpha
 Classifier: Environment :: Console
```

### Comparing `linopy-0.2/linopy.egg-info/SOURCES.txt` & `linopy-0.2.1/linopy.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `linopy-0.2/setup.py` & `linopy-0.2.1/setup.py`

 * *Files 5% similar despite different names*

```diff
@@ -51,18 +51,14 @@
         ],
         "dev": [
             "pytest",
             "pytest-cov",
             "pre-commit",
             "paramiko",
             "gurobipy",
-            # until available for windows/mac
-            # "highspy",
-            "cplex",
-            "xpress",
         ],
         "solvers": [
             "gurobipy",
             # until available for windows/mac
             # "highspy",
             "cplex",
             "xpress",
```

### Comparing `linopy-0.2/test/test_common.py` & `linopy-0.2.1/test/test_common.py`

 * *Files identical despite different names*

### Comparing `linopy-0.2/test/test_constraint.py` & `linopy-0.2.1/test/test_constraint.py`

 * *Files identical despite different names*

### Comparing `linopy-0.2/test/test_constraints.py` & `linopy-0.2.1/test/test_constraints.py`

 * *Files identical despite different names*

### Comparing `linopy-0.2/test/test_inconsistency_checks.py` & `linopy-0.2.1/test/test_inconsistency_checks.py`

 * *Files identical despite different names*

### Comparing `linopy-0.2/test/test_io.py` & `linopy-0.2.1/test/test_io.py`

 * *Files identical despite different names*

### Comparing `linopy-0.2/test/test_linear_expression.py` & `linopy-0.2.1/test/test_linear_expression.py`

 * *Files 1% similar despite different names*

```diff
@@ -93,15 +93,15 @@
 
 def test_repr(m):
     expr = m.linexpr((10, "x"), (1, "y"))
     expr.__repr__()
 
 
 def test_fill_value():
-    isinstance(LinearExpression.fill_value, dict)
+    isinstance(LinearExpression._fill_value, dict)
 
 
 def test_linexpr_with_scalars(m):
     expr = m.linexpr((10, "x"), (1, "y"))
     target = xr.DataArray(
         [[10, 1], [10, 1]], coords={"dim_0": [0, 1]}, dims=["dim_0", TERM_DIM]
     )
```

### Comparing `linopy-0.2/test/test_matrices.py` & `linopy-0.2.1/test/test_matrices.py`

 * *Files identical despite different names*

### Comparing `linopy-0.2/test/test_model.py` & `linopy-0.2.1/test/test_model.py`

 * *Files identical despite different names*

### Comparing `linopy-0.2/test/test_optimization.py` & `linopy-0.2.1/test/test_optimization.py`

 * *Files identical despite different names*

### Comparing `linopy-0.2/test/test_options.py` & `linopy-0.2.1/test/test_options.py`

 * *Files identical despite different names*

### Comparing `linopy-0.2/test/test_quadratic_expression.py` & `linopy-0.2.1/test/test_quadratic_expression.py`

 * *Files 18% similar despite different names*

```diff
@@ -2,16 +2,16 @@
 # -*- coding: utf-8 -*-
 
 import numpy as np
 import pandas as pd
 import pytest
 from scipy.sparse import csc_matrix
 
-from linopy import Model
-from linopy.constants import FACTOR_DIM
+from linopy import Model, merge
+from linopy.constants import FACTOR_DIM, TERM_DIM
 from linopy.expressions import QuadraticExpression
 
 
 @pytest.fixture
 def model():
     return Model()
 
@@ -96,14 +96,33 @@
 
 
 def test_quadratic_expression_wrong_multiplication(x, y):
     with pytest.raises(TypeError):
         x * x * y
 
 
+def test_merge_linear_expression_and_quadratic_expression(x, y):
+    linexpr = 10 * x + y + 5
+    quadexpr = x * y
+
+    with pytest.raises(ValueError):
+        expr = merge(linexpr, quadexpr, cls=QuadraticExpression)
+
+    linexpr = linexpr.to_quadexpr()
+    expr = merge(linexpr, quadexpr, cls=QuadraticExpression)
+    assert isinstance(expr, QuadraticExpression)
+    assert expr.nterm == 3
+    assert expr.const.sum() == 10
+    assert FACTOR_DIM not in expr.coeffs.dims
+    assert FACTOR_DIM not in expr.const.dims
+
+    first_term = expr.data.isel({TERM_DIM: 0})
+    assert (first_term.vars.isel({FACTOR_DIM: 1}) == -1).all()
+
+
 def test_quadratic_expression_loc(x):
     expr = x * x
     assert expr.loc[0].size < expr.loc[:5].size
 
 
 def test_quadratic_expression_flat(x, y):
     expr = x * y + x + 5
```

### Comparing `linopy-0.2/test/test_repr.py` & `linopy-0.2.1/test/test_repr.py`

 * *Files 2% similar despite different names*

```diff
@@ -144,7 +144,9 @@
 def test_print_options():
     for o in [v, lv, cv_, cv]:
         default_repr = repr(o)
         with options as opts:
             opts.set_value(display_max_rows=20)
             longer_repr = repr(o)
         assert len(default_repr) < len(longer_repr)
+
+        longer_repr = o.print(display_max_rows=20)
```

### Comparing `linopy-0.2/test/test_scalar_constraint.py` & `linopy-0.2.1/test/test_scalar_constraint.py`

 * *Files identical despite different names*

### Comparing `linopy-0.2/test/test_scalar_linear_expression.py` & `linopy-0.2.1/test/test_scalar_linear_expression.py`

 * *Files identical despite different names*

### Comparing `linopy-0.2/test/test_variable.py` & `linopy-0.2.1/test/test_variable.py`

 * *Files 1% similar despite different names*

```diff
@@ -142,15 +142,15 @@
     res = x.sum()
     assert res.nterm == 10
 
 
 def test_variable_where(x):
     x = x.where([True] * 4 + [False] * 6)
     assert isinstance(x, linopy.variables.Variable)
-    assert x.labels[9] == x.fill_value["labels"]
+    assert x.labels[9] == x._fill_value["labels"]
 
     x = x.where([True] * 4 + [False] * 6, x[0])
     assert isinstance(x, linopy.variables.Variable)
     assert x.labels[9] == x[0].label
 
     x = x.where([True] * 4 + [False] * 6, x.loc[0])
     assert isinstance(x, linopy.variables.Variable)
```

### Comparing `linopy-0.2/test/test_variable_assignment.py` & `linopy-0.2.1/test/test_variable_assignment.py`

 * *Files identical despite different names*

### Comparing `linopy-0.2/test/test_variables.py` & `linopy-0.2.1/test/test_variables.py`

 * *Files identical despite different names*

