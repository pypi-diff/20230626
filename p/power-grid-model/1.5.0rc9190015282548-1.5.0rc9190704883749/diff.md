# Comparing `tmp/power-grid-model-1.5.0rc9190015282548.tar.gz` & `tmp/power-grid-model-1.5.0rc9190704883749.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "power-grid-model-1.5.0rc9190015282548.tar", last modified: Mon Jun 26 12:57:57 2023, max compression
+gzip compressed data, was "power-grid-model-1.5.0rc9190704883749.tar", last modified: Mon Jun 26 15:22:14 2023, max compression
```

## Comparing `power-grid-model-1.5.0rc9190015282548.tar` & `power-grid-model-1.5.0rc9190704883749.tar`

### file list

```diff
@@ -1,620 +1,620 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 12:57:57.983416 power-grid-model-1.5.0rc9190015282548/
--rw-r--r--   0 runner    (1001) docker     (123)    14907 2023-06-26 12:57:01.000000 power-grid-model-1.5.0rc9190015282548/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      354 2023-06-26 12:57:01.000000 power-grid-model-1.5.0rc9190015282548/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     8142 2023-06-26 12:57:57.983416 power-grid-model-1.5.0rc9190015282548/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)       20 2023-06-26 12:57:05.000000 power-grid-model-1.5.0rc9190015282548/PYPI_VERSION
--rw-r--r--   0 runner    (1001) docker     (123)     6818 2023-06-26 12:57:01.000000 power-grid-model-1.5.0rc9190015282548/README.md
--rw-r--r--   0 runner    (1001) docker     (123)        4 2023-06-26 12:57:01.000000 power-grid-model-1.5.0rc9190015282548/VERSION
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 12:57:57.895410 power-grid-model-1.5.0rc9190015282548/power_grid_model_c/
--rw-r--r--   0 runner    (1001) docker     (123)      231 2023-06-26 12:57:01.000000 power-grid-model-1.5.0rc9190015282548/power_grid_model_c/CMakeLists.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 12:57:57.895410 power-grid-model-1.5.0rc9190015282548/power_grid_model_c/power_grid_model/
--rw-r--r--   0 runner    (1001) docker     (123)      573 2023-06-26 12:57:01.000000 power-grid-model-1.5.0rc9190015282548/power_grid_model_c/power_grid_model/CMakeLists.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 12:57:57.883409 power-grid-model-1.5.0rc9190015282548/power_grid_model_c/power_grid_model/include/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 12:57:57.895410 power-grid-model-1.5.0rc9190015282548/power_grid_model_c/power_grid_model/include/power_grid_model/
--rw-r--r--   0 runner    (1001) docker     (123)     1118 2023-06-26 12:57:01.000000 power-grid-model-1.5.0rc9190015282548/power_grid_model_c/power_grid_model/include/power_grid_model/all_components.hpp
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 12:57:57.899410 power-grid-model-1.5.0rc9190015282548/power_grid_model_c/power_grid_model/include/power_grid_model/auxiliary/
--rw-r--r--   0 runner    (1001) docker     (123)     4220 2023-06-26 12:57:01.000000 power-grid-model-1.5.0rc9190015282548/power_grid_model_c/power_grid_model/include/power_grid_model/auxiliary/dataset.hpp
--rw-r--r--   0 runner    (1001) docker     (123)    28564 2023-06-26 12:57:01.000000 power-grid-model-1.5.0rc9190015282548/power_grid_model_c/power_grid_model/include/power_grid_model/auxiliary/input.hpp
--rw-r--r--   0 runner    (1001) docker     (123)     9937 2023-06-26 12:57:01.000000 power-grid-model-1.5.0rc9190015282548/power_grid_model_c/power_grid_model/include/power_grid_model/auxiliary/meta_data.hpp
--rw-r--r--   0 runner    (1001) docker     (123)     1838 2023-06-26 12:57:01.000000 power-grid-model-1.5.0rc9190015282548/power_grid_model_c/power_grid_model/include/power_grid_model/auxiliary/meta_data_gen.hpp
--rw-r--r--   0 runner    (1001) docker     (123)    17078 2023-06-26 12:57:01.000000 power-grid-model-1.5.0rc9190015282548/power_grid_model_c/power_grid_model/include/power_grid_model/auxiliary/output.hpp
--rw-r--r--   0 runner    (1001) docker     (123)     9396 2023-06-26 12:57:01.000000 power-grid-model-1.5.0rc9190015282548/power_grid_model_c/power_grid_model/include/power_grid_model/auxiliary/update.hpp
--rw-r--r--   0 runner    (1001) docker     (123)     8983 2023-06-26 12:57:01.000000 power-grid-model-1.5.0rc9190015282548/power_grid_model_c/power_grid_model/include/power_grid_model/calculation_parameters.hpp
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 12:57:57.903411 power-grid-model-1.5.0rc9190015282548/power_grid_model_c/power_grid_model/include/power_grid_model/component/
--rw-r--r--   0 runner    (1001) docker     (123)     4214 2023-06-26 12:57:01.000000 power-grid-model-1.5.0rc9190015282548/power_grid_model_c/power_grid_model/include/power_grid_model/component/appliance.hpp
--rw-r--r--   0 runner    (1001) docker     (123)     1103 2023-06-26 12:57:01.000000 power-grid-model-1.5.0rc9190015282548/power_grid_model_c/power_grid_model/include/power_grid_model/component/base.hpp
--rw-r--r--   0 runner    (1001) docker     (123)     8931 2023-06-26 12:57:01.000000 power-grid-model-1.5.0rc9190015282548/power_grid_model_c/power_grid_model/include/power_grid_model/component/branch.hpp
--rw-r--r--   0 runner    (1001) docker     (123)     6780 2023-06-26 12:57:01.000000 power-grid-model-1.5.0rc9190015282548/power_grid_model_c/power_grid_model/include/power_grid_model/component/branch3.hpp
--rw-r--r--   0 runner    (1001) docker     (123)     4445 2023-06-26 12:57:01.000000 power-grid-model-1.5.0rc9190015282548/power_grid_model_c/power_grid_model/include/power_grid_model/component/fault.hpp
--rw-r--r--   0 runner    (1001) docker     (123)     2320 2023-06-26 12:57:01.000000 power-grid-model-1.5.0rc9190015282548/power_grid_model_c/power_grid_model/include/power_grid_model/component/line.hpp
--rw-r--r--   0 runner    (1001) docker     (123)     1629 2023-06-26 12:57:01.000000 power-grid-model-1.5.0rc9190015282548/power_grid_model_c/power_grid_model/include/power_grid_model/component/link.hpp
--rw-r--r--   0 runner    (1001) docker     (123)     5350 2023-06-26 12:57:01.000000 power-grid-model-1.5.0rc9190015282548/power_grid_model_c/power_grid_model/include/power_grid_model/component/load_gen.hpp
--rw-r--r--   0 runner    (1001) docker     (123)     2693 2023-06-26 12:57:01.000000 power-grid-model-1.5.0rc9190015282548/power_grid_model_c/power_grid_model/include/power_grid_model/component/node.hpp
--rw-r--r--   0 runner    (1001) docker     (123)     4775 2023-06-26 12:57:01.000000 power-grid-model-1.5.0rc9190015282548/power_grid_model_c/power_grid_model/include/power_grid_model/component/power_sensor.hpp
--rw-r--r--   0 runner    (1001) docker     (123)     1678 2023-06-26 12:57:01.000000 power-grid-model-1.5.0rc9190015282548/power_grid_model_c/power_grid_model/include/power_grid_model/component/sensor.hpp
--rw-r--r--   0 runner    (1001) docker     (123)     2873 2023-06-26 12:57:01.000000 power-grid-model-1.5.0rc9190015282548/power_grid_model_c/power_grid_model/include/power_grid_model/component/shunt.hpp
--rw-r--r--   0 runner    (1001) docker     (123)     4396 2023-06-26 12:57:01.000000 power-grid-model-1.5.0rc9190015282548/power_grid_model_c/power_grid_model/include/power_grid_model/component/source.hpp
--rw-r--r--   0 runner    (1001) docker     (123)    20093 2023-06-26 12:57:01.000000 power-grid-model-1.5.0rc9190015282548/power_grid_model_c/power_grid_model/include/power_grid_model/component/three_winding_transformer.hpp
--rw-r--r--   0 runner    (1001) docker     (123)    10973 2023-06-26 12:57:01.000000 power-grid-model-1.5.0rc9190015282548/power_grid_model_c/power_grid_model/include/power_grid_model/component/transformer.hpp
--rw-r--r--   0 runner    (1001) docker     (123)     1088 2023-06-26 12:57:01.000000 power-grid-model-1.5.0rc9190015282548/power_grid_model_c/power_grid_model/include/power_grid_model/component/transformer_utils.hpp
--rw-r--r--   0 runner    (1001) docker     (123)     5581 2023-06-26 12:57:01.000000 power-grid-model-1.5.0rc9190015282548/power_grid_model_c/power_grid_model/include/power_grid_model/component/voltage_sensor.hpp
--rw-r--r--   0 runner    (1001) docker     (123)    15129 2023-06-26 12:57:01.000000 power-grid-model-1.5.0rc9190015282548/power_grid_model_c/power_grid_model/include/power_grid_model/container.hpp
--rw-r--r--   0 runner    (1001) docker     (123)     2058 2023-06-26 12:57:01.000000 power-grid-model-1.5.0rc9190015282548/power_grid_model_c/power_grid_model/include/power_grid_model/enum.hpp
--rw-r--r--   0 runner    (1001) docker     (123)     5302 2023-06-26 12:57:01.000000 power-grid-model-1.5.0rc9190015282548/power_grid_model_c/power_grid_model/include/power_grid_model/exception.hpp
--rw-r--r--   0 runner    (1001) docker     (123)    67807 2023-06-26 12:57:01.000000 power-grid-model-1.5.0rc9190015282548/power_grid_model_c/power_grid_model/include/power_grid_model/main_model.hpp
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 12:57:57.903411 power-grid-model-1.5.0rc9190015282548/power_grid_model_c/power_grid_model/include/power_grid_model/math_solver/
--rw-r--r--   0 runner    (1001) docker     (123)     2436 2023-06-26 12:57:01.000000 power-grid-model-1.5.0rc9190015282548/power_grid_model_c/power_grid_model/include/power_grid_model/math_solver/block_matrix.hpp
--rw-r--r--   0 runner    (1001) docker     (123)     8948 2023-06-26 12:57:01.000000 power-grid-model-1.5.0rc9190015282548/power_grid_model_c/power_grid_model/include/power_grid_model/math_solver/iterative_current_pf_solver.hpp
--rw-r--r--   0 runner    (1001) docker     (123)    41694 2023-06-26 12:57:01.000000 power-grid-model-1.5.0rc9190015282548/power_grid_model_c/power_grid_model/include/power_grid_model/math_solver/iterative_linear_se_solver.hpp
--rw-r--r--   0 runner    (1001) docker     (123)     7158 2023-06-26 12:57:01.000000 power-grid-model-1.5.0rc9190015282548/power_grid_model_c/power_grid_model/include/power_grid_model/math_solver/iterative_pf_solver.hpp
--rw-r--r--   0 runner    (1001) docker     (123)     6446 2023-06-26 12:57:01.000000 power-grid-model-1.5.0rc9190015282548/power_grid_model_c/power_grid_model/include/power_grid_model/math_solver/linear_pf_solver.hpp
--rw-r--r--   0 runner    (1001) docker     (123)     6267 2023-06-26 12:57:01.000000 power-grid-model-1.5.0rc9190015282548/power_grid_model_c/power_grid_model/include/power_grid_model/math_solver/math_solver.hpp
--rw-r--r--   0 runner    (1001) docker     (123)    16064 2023-06-26 12:57:01.000000 power-grid-model-1.5.0rc9190015282548/power_grid_model_c/power_grid_model/include/power_grid_model/math_solver/newton_raphson_pf_solver.hpp
--rw-r--r--   0 runner    (1001) docker     (123)    16203 2023-06-26 12:57:01.000000 power-grid-model-1.5.0rc9190015282548/power_grid_model_c/power_grid_model/include/power_grid_model/math_solver/sparse_lu_solver.hpp
--rw-r--r--   0 runner    (1001) docker     (123)    20148 2023-06-26 12:57:01.000000 power-grid-model-1.5.0rc9190015282548/power_grid_model_c/power_grid_model/include/power_grid_model/math_solver/y_bus.hpp
--rw-r--r--   0 runner    (1001) docker     (123)     3110 2023-06-26 12:57:01.000000 power-grid-model-1.5.0rc9190015282548/power_grid_model_c/power_grid_model/include/power_grid_model/power_grid_model.hpp
--rw-r--r--   0 runner    (1001) docker     (123)     2753 2023-06-26 12:57:01.000000 power-grid-model-1.5.0rc9190015282548/power_grid_model_c/power_grid_model/include/power_grid_model/sparse_mapping.hpp
--rw-r--r--   0 runner    (1001) docker     (123)    11394 2023-06-26 12:57:01.000000 power-grid-model-1.5.0rc9190015282548/power_grid_model_c/power_grid_model/include/power_grid_model/three_phase_tensor.hpp
--rw-r--r--   0 runner    (1001) docker     (123)     1849 2023-06-26 12:57:01.000000 power-grid-model-1.5.0rc9190015282548/power_grid_model_c/power_grid_model/include/power_grid_model/timer.hpp
--rw-r--r--   0 runner    (1001) docker     (123)    30877 2023-06-26 12:57:01.000000 power-grid-model-1.5.0rc9190015282548/power_grid_model_c/power_grid_model/include/power_grid_model/topology.hpp
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 12:57:57.903411 power-grid-model-1.5.0rc9190015282548/power_grid_model_c/power_grid_model_c/
--rw-r--r--   0 runner    (1001) docker     (123)      729 2023-06-26 12:57:01.000000 power-grid-model-1.5.0rc9190015282548/power_grid_model_c/power_grid_model_c/CMakeLists.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 12:57:57.903411 power-grid-model-1.5.0rc9190015282548/power_grid_model_c/power_grid_model_c/include/
--rw-r--r--   0 runner    (1001) docker     (123)    26085 2023-06-26 12:57:01.000000 power-grid-model-1.5.0rc9190015282548/power_grid_model_c/power_grid_model_c/include/power_grid_model_c.h
--rw-r--r--   0 runner    (1001) docker     (123)    15360 2023-06-26 12:57:01.000000 power-grid-model-1.5.0rc9190015282548/power_grid_model_c/power_grid_model_c/power_grid_model_c.cpp
--rw-r--r--   0 runner    (1001) docker     (123)     3634 2023-06-26 12:57:01.000000 power-grid-model-1.5.0rc9190015282548/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-26 12:57:57.987416 power-grid-model-1.5.0rc9190015282548/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     7078 2023-06-26 12:57:01.000000 power-grid-model-1.5.0rc9190015282548/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 12:57:57.883409 power-grid-model-1.5.0rc9190015282548/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 12:57:57.903411 power-grid-model-1.5.0rc9190015282548/src/power_grid_model/
--rw-r--r--   0 runner    (1001) docker     (123)      509 2023-06-26 12:57:01.000000 power-grid-model-1.5.0rc9190015282548/src/power_grid_model/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 12:57:57.907411 power-grid-model-1.5.0rc9190015282548/src/power_grid_model/core/
--rw-r--r--   0 runner    (1001) docker     (123)      154 2023-06-26 12:57:01.000000 power-grid-model-1.5.0rc9190015282548/src/power_grid_model/core/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2100 2023-06-26 12:57:01.000000 power-grid-model-1.5.0rc9190015282548/src/power_grid_model/core/error_handling.py
--rw-r--r--   0 runner    (1001) docker     (123)      367 2023-06-26 12:57:01.000000 power-grid-model-1.5.0rc9190015282548/src/power_grid_model/core/index_integer.py
--rw-r--r--   0 runner    (1001) docker     (123)     1682 2023-06-26 12:57:01.000000 power-grid-model-1.5.0rc9190015282548/src/power_grid_model/core/options.py
--rw-r--r--   0 runner    (1001) docker     (123)     9994 2023-06-26 12:57:01.000000 power-grid-model-1.5.0rc9190015282548/src/power_grid_model/core/power_grid_core.py
--rw-r--r--   0 runner    (1001) docker     (123)     9240 2023-06-26 12:57:01.000000 power-grid-model-1.5.0rc9190015282548/src/power_grid_model/core/power_grid_meta.py
--rw-r--r--   0 runner    (1001) docker     (123)    17761 2023-06-26 12:57:01.000000 power-grid-model-1.5.0rc9190015282548/src/power_grid_model/core/power_grid_model.py
--rw-r--r--   0 runner    (1001) docker     (123)     5239 2023-06-26 12:57:01.000000 power-grid-model-1.5.0rc9190015282548/src/power_grid_model/data_types.py
--rw-r--r--   0 runner    (1001) docker     (123)     2183 2023-06-26 12:57:01.000000 power-grid-model-1.5.0rc9190015282548/src/power_grid_model/enum.py
--rw-r--r--   0 runner    (1001) docker     (123)      505 2023-06-26 12:57:01.000000 power-grid-model-1.5.0rc9190015282548/src/power_grid_model/errors.py
--rw-r--r--   0 runner    (1001) docker     (123)    21645 2023-06-26 12:57:01.000000 power-grid-model-1.5.0rc9190015282548/src/power_grid_model/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 12:57:57.907411 power-grid-model-1.5.0rc9190015282548/src/power_grid_model/validation/
--rw-r--r--   0 runner    (1001) docker     (123)      547 2023-06-26 12:57:01.000000 power-grid-model-1.5.0rc9190015282548/src/power_grid_model/validation/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4166 2023-06-26 12:57:01.000000 power-grid-model-1.5.0rc9190015282548/src/power_grid_model/validation/assertions.py
--rw-r--r--   0 runner    (1001) docker     (123)    14686 2023-06-26 12:57:01.000000 power-grid-model-1.5.0rc9190015282548/src/power_grid_model/validation/errors.py
--rw-r--r--   0 runner    (1001) docker     (123)    30704 2023-06-26 12:57:01.000000 power-grid-model-1.5.0rc9190015282548/src/power_grid_model/validation/rules.py
--rw-r--r--   0 runner    (1001) docker     (123)     8601 2023-06-26 12:57:01.000000 power-grid-model-1.5.0rc9190015282548/src/power_grid_model/validation/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)    28618 2023-06-26 12:57:01.000000 power-grid-model-1.5.0rc9190015282548/src/power_grid_model/validation/validation.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 12:57:57.907411 power-grid-model-1.5.0rc9190015282548/src/power_grid_model.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     8142 2023-06-26 12:57:57.000000 power-grid-model-1.5.0rc9190015282548/src/power_grid_model.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    37119 2023-06-26 12:57:57.000000 power-grid-model-1.5.0rc9190015282548/src/power_grid_model.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-26 12:57:57.000000 power-grid-model-1.5.0rc9190015282548/src/power_grid_model.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      195 2023-06-26 12:57:57.000000 power-grid-model-1.5.0rc9190015282548/src/power_grid_model.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       17 2023-06-26 12:57:57.000000 power-grid-model-1.5.0rc9190015282548/src/power_grid_model.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 12:57:57.891410 power-grid-model-1.5.0rc9190015282548/tests/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 12:57:57.891410 power-grid-model-1.5.0rc9190015282548/tests/data/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 12:57:57.891410 power-grid-model-1.5.0rc9190015282548/tests/data/power_flow/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 12:57:57.907411 power-grid-model-1.5.0rc9190015282548/tests/data/power_flow/1os2msr/
--rw-r--r--   0 runner    (1001) docker     (123)     1100 2023-06-26 12:57:01.000000 power-grid-model-1.5.0rc9190015282548/tests/data/power_flow/1os2msr/input.json
--rw-r--r--   0 runner    (1001) docker     (123)      148 2023-06-26 12:57:01.000000 power-grid-model-1.5.0rc9190015282548/tests/data/power_flow/1os2msr/input.json.license
--rw-r--r--   0 runner    (1001) docker     (123)       76 2023-06-26 12:57:01.000000 power-grid-model-1.5.0rc9190015282548/tests/data/power_flow/1os2msr/params.json
--rw-r--r--   0 runner    (1001) docker     (123)      148 2023-06-26 12:57:01.000000 power-grid-model-1.5.0rc9190015282548/tests/data/power_flow/1os2msr/params.json.license
--rw-r--r--   0 runner    (1001) docker     (123)     1582 2023-06-26 12:57:01.000000 power-grid-model-1.5.0rc9190015282548/tests/data/power_flow/1os2msr/sym_output.json
--rw-r--r--   0 runner    (1001) docker     (123)      148 2023-06-26 12:57:01.000000 power-grid-model-1.5.0rc9190015282548/tests/data/power_flow/1os2msr/sym_output.json.license
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 12:57:57.911411 power-grid-model-1.5.0rc9190015282548/tests/data/power_flow/dummy-test/
--rw-r--r--   0 runner    (1001) docker     (123)     1429 2023-06-26 12:57:01.000000 power-grid-model-1.5.0rc9190015282548/tests/data/power_flow/dummy-test/input.json
--rw-r--r--   0 runner    (1001) docker     (123)      148 2023-06-26 12:57:01.000000 power-grid-model-1.5.0rc9190015282548/tests/data/power_flow/dummy-test/input.json.license
--rw-r--r--   0 runner    (1001) docker     (123)       99 2023-06-26 12:57:01.000000 power-grid-model-1.5.0rc9190015282548/tests/data/power_flow/dummy-test/params.json
--rw-r--r--   0 runner    (1001) docker     (123)      148 2023-06-26 12:57:01.000000 power-grid-model-1.5.0rc9190015282548/tests/data/power_flow/dummy-test/params.json.license
--rw-r--r--   0 runner    (1001) docker     (123)      666 2023-06-26 12:57:01.000000 power-grid-model-1.5.0rc9190015282548/tests/data/power_flow/dummy-test/sym_output.json
--rw-r--r--   0 runner    (1001) docker     (123)      148 2023-06-26 12:57:01.000000 power-grid-model-1.5.0rc9190015282548/tests/data/power_flow/dummy-test/sym_output.json.license
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 12:57:57.911411 power-grid-model-1.5.0rc9190015282548/tests/data/power_flow/dummy-test-batch/
--rw-r--r--   0 runner    (1001) docker     (123)      764 2023-06-26 12:57:01.000000 power-grid-model-1.5.0rc9190015282548/tests/data/power_flow/dummy-test-batch/input.json
--rw-r--r--   0 runner    (1001) docker     (123)      148 2023-06-26 12:57:01.000000 power-grid-model-1.5.0rc9190015282548/tests/data/power_flow/dummy-test-batch/input.json.license
--rw-r--r--   0 runner    (1001) docker     (123)       68 2023-06-26 12:57:01.000000 power-grid-model-1.5.0rc9190015282548/tests/data/power_flow/dummy-test-batch/params.json
--rw-r--r--   0 runner    (1001) docker     (123)      148 2023-06-26 12:57:01.000000 power-grid-model-1.5.0rc9190015282548/tests/data/power_flow/dummy-test-batch/params.json.license
--rw-r--r--   0 runner    (1001) docker     (123)      107 2023-06-26 12:57:01.000000 power-grid-model-1.5.0rc9190015282548/tests/data/power_flow/dummy-test-batch/sym_output.json
--rw-r--r--   0 runner    (1001) docker     (123)      148 2023-06-26 12:57:01.000000 power-grid-model-1.5.0rc9190015282548/tests/data/power_flow/dummy-test-batch/sym_output.json.license
--rw-r--r--   0 runner    (1001) docker     (123)      392 2023-06-26 12:57:01.000000 power-grid-model-1.5.0rc9190015282548/tests/data/power_flow/dummy-test-batch/sym_output_batch.json
--rw-r--r--   0 runner    (1001) docker     (123)      148 2023-06-26 12:57:01.000000 power-grid-model-1.5.0rc9190015282548/tests/data/power_flow/dummy-test-batch/sym_output_batch.json.license
--rw-r--r--   0 runner    (1001) docker     (123)      359 2023-06-26 12:57:01.000000 power-grid-model-1.5.0rc9190015282548/tests/data/power_flow/dummy-test-batch/update_batch.json
--rw-r--r--   0 runner    (1001) docker     (123)      148 2023-06-26 12:57:01.000000 power-grid-model-1.5.0rc9190015282548/tests/data/power_flow/dummy-test-batch/update_batch.json.license
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 12:57:57.911411 power-grid-model-1.5.0rc9190015282548/tests/data/power_flow/dummy-test-batch-dependent-cacheable/
--rw-r--r--   0 runner    (1001) docker     (123)      764 2023-06-26 12:57:01.000000 power-grid-model-1.5.0rc9190015282548/tests/data/power_flow/dummy-test-batch-dependent-cacheable/input.json
--rw-r--r--   0 runner    (1001) docker     (123)      148 2023-06-26 12:57:01.000000 power-grid-model-1.5.0rc9190015282548/tests/data/power_flow/dummy-test-batch-dependent-cacheable/input.json.license
--rw-r--r--   0 runner    (1001) docker     (123)       99 2023-06-26 12:57:01.000000 power-grid-model-1.5.0rc9190015282548/tests/data/power_flow/dummy-test-batch-dependent-cacheable/params.json
--rw-r--r--   0 runner    (1001) docker     (123)      148 2023-06-26 12:57:01.000000 power-grid-model-1.5.0rc9190015282548/tests/data/power_flow/dummy-test-batch-dependent-cacheable/params.json.license
--rw-r--r--   0 runner    (1001) docker     (123)      107 2023-06-26 12:57:01.000000 power-grid-model-1.5.0rc9190015282548/tests/data/power_flow/dummy-test-batch-dependent-cacheable/sym_output.json
--rw-r--r--   0 runner    (1001) docker     (123)      148 2023-06-26 12:57:01.000000 power-grid-model-1.5.0rc9190015282548/tests/data/power_flow/dummy-test-batch-dependent-cacheable/sym_output.json.license
--rw-r--r--   0 runner    (1001) docker     (123)      392 2023-06-26 12:57:01.000000 power-grid-model-1.5.0rc9190015282548/tests/data/power_flow/dummy-test-batch-dependent-cacheable/sym_output_batch.json
--rw-r--r--   0 runner    (1001) docker     (123)      148 2023-06-26 12:57:01.000000 power-grid-model-1.5.0rc9190015282548/tests/data/power_flow/dummy-test-batch-dependent-cacheable/sym_output_batch.json.license
--rw-r--r--   0 runner    (1001) docker     (123)      466 2023-06-26 12:57:01.000000 power-grid-model-1.5.0rc9190015282548/tests/data/power_flow/dummy-test-batch-dependent-cacheable/update_batch.json
--rw-r--r--   0 runner    (1001) docker     (123)      148 2023-06-26 12:57:01.000000 power-grid-model-1.5.0rc9190015282548/tests/data/power_flow/dummy-test-batch-dependent-cacheable/update_batch.json.license
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 12:57:57.915411 power-grid-model-1.5.0rc9190015282548/tests/data/power_flow/dummy-test-batch-dependent-not-cacheable/
--rw-r--r--   0 runner    (1001) docker     (123)      764 2023-06-26 12:57:01.000000 power-grid-model-1.5.0rc9190015282548/tests/data/power_flow/dummy-test-batch-dependent-not-cacheable/input.json
--rw-r--r--   0 runner    (1001) docker     (123)      148 2023-06-26 12:57:01.000000 power-grid-model-1.5.0rc9190015282548/tests/data/power_flow/dummy-test-batch-dependent-not-cacheable/input.json.license
--rw-r--r--   0 runner    (1001) docker     (123)       99 2023-06-26 12:57:01.000000 power-grid-model-1.5.0rc9190015282548/tests/data/power_flow/dummy-test-batch-dependent-not-cacheable/params.json
--rw-r--r--   0 runner    (1001) docker     (123)      148 2023-06-26 12:57:01.000000 power-grid-model-1.5.0rc9190015282548/tests/data/power_flow/dummy-test-batch-dependent-not-cacheable/params.json.license
--rw-r--r--   0 runner    (1001) docker     (123)      107 2023-06-26 12:57:01.000000 power-grid-model-1.5.0rc9190015282548/tests/data/power_flow/dummy-test-batch-dependent-not-cacheable/sym_output.json
--rw-r--r--   0 runner    (1001) docker     (123)      148 2023-06-26 12:57:01.000000 power-grid-model-1.5.0rc9190015282548/tests/data/power_flow/dummy-test-batch-dependent-not-cacheable/sym_output.json.license
--rw-r--r--   0 runner    (1001) docker     (123)      392 2023-06-26 12:57:01.000000 power-grid-model-1.5.0rc9190015282548/tests/data/power_flow/dummy-test-batch-dependent-not-cacheable/sym_output_batch.json
--rw-r--r--   0 runner    (1001) docker     (123)      148 2023-06-26 12:57:01.000000 power-grid-model-1.5.0rc9190015282548/tests/data/power_flow/dummy-test-batch-dependent-not-cacheable/sym_output_batch.json.license
--rw-r--r--   0 runner    (1001) docker     (123)      542 2023-06-26 12:57:01.000000 power-grid-model-1.5.0rc9190015282548/tests/data/power_flow/dummy-test-batch-dependent-not-cacheable/update_batch.json
--rw-r--r--   0 runner    (1001) docker     (123)      148 2023-06-26 12:57:01.000000 power-grid-model-1.5.0rc9190015282548/tests/data/power_flow/dummy-test-batch-dependent-not-cacheable/update_batch.json.license
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 12:57:57.915411 power-grid-model-1.5.0rc9190015282548/tests/data/power_flow/dummy-test-batch-incomplete-input/
--rw-r--r--   0 runner    (1001) docker     (123)      738 2023-06-26 12:57:01.000000 power-grid-model-1.5.0rc9190015282548/tests/data/power_flow/dummy-test-batch-incomplete-input/input.json
--rw-r--r--   0 runner    (1001) docker     (123)      148 2023-06-26 12:57:01.000000 power-grid-model-1.5.0rc9190015282548/tests/data/power_flow/dummy-test-batch-incomplete-input/input.json.license
--rw-r--r--   0 runner    (1001) docker     (123)       68 2023-06-26 12:57:01.000000 power-grid-model-1.5.0rc9190015282548/tests/data/power_flow/dummy-test-batch-incomplete-input/params.json
--rw-r--r--   0 runner    (1001) docker     (123)      148 2023-06-26 12:57:01.000000 power-grid-model-1.5.0rc9190015282548/tests/data/power_flow/dummy-test-batch-incomplete-input/params.json.license
--rw-r--r--   0 runner    (1001) docker     (123)      148 2023-06-26 12:57:01.000000 power-grid-model-1.5.0rc9190015282548/tests/data/power_flow/dummy-test-batch-incomplete-input/sym_output.json.license
--rw-r--r--   0 runner    (1001) docker     (123)      392 2023-06-26 12:57:01.000000 power-grid-model-1.5.0rc9190015282548/tests/data/power_flow/dummy-test-batch-incomplete-input/sym_output_batch.json
--rw-r--r--   0 runner    (1001) docker     (123)      148 2023-06-26 12:57:01.000000 power-grid-model-1.5.0rc9190015282548/tests/data/power_flow/dummy-test-batch-incomplete-input/sym_output_batch.json.license
--rw-r--r--   0 runner    (1001) docker     (123)      401 2023-06-26 12:57:01.000000 power-grid-model-1.5.0rc9190015282548/tests/data/power_flow/dummy-test-batch-incomplete-input/update_batch.json
--rw-r--r--   0 runner    (1001) docker     (123)      148 2023-06-26 12:57:01.000000 power-grid-model-1.5.0rc9190015282548/tests/data/power_flow/dummy-test-batch-incomplete-input/update_batch.json.license
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 12:57:57.915411 power-grid-model-1.5.0rc9190015282548/tests/data/power_flow/dummy-test-batch-independent-cacheable/
--rw-r--r--   0 runner    (1001) docker     (123)      764 2023-06-26 12:57:01.000000 power-grid-model-1.5.0rc9190015282548/tests/data/power_flow/dummy-test-batch-independent-cacheable/input.json
--rw-r--r--   0 runner    (1001) docker     (123)      148 2023-06-26 12:57:01.000000 power-grid-model-1.5.0rc9190015282548/tests/data/power_flow/dummy-test-batch-independent-cacheable/input.json.license
--rw-r--r--   0 runner    (1001) docker     (123)       99 2023-06-26 12:57:01.000000 power-grid-model-1.5.0rc9190015282548/tests/data/power_flow/dummy-test-batch-independent-cacheable/params.json
--rw-r--r--   0 runner    (1001) docker     (123)      148 2023-06-26 12:57:01.000000 power-grid-model-1.5.0rc9190015282548/tests/data/power_flow/dummy-test-batch-independent-cacheable/params.json.license
--rw-r--r--   0 runner    (1001) docker     (123)      107 2023-06-26 12:57:01.000000 power-grid-model-1.5.0rc9190015282548/tests/data/power_flow/dummy-test-batch-independent-cacheable/sym_output.json
--rw-r--r--   0 runner    (1001) docker     (123)      148 2023-06-26 12:57:01.000000 power-grid-model-1.5.0rc9190015282548/tests/data/power_flow/dummy-test-batch-independent-cacheable/sym_output.json.license
--rw-r--r--   0 runner    (1001) docker     (123)      392 2023-06-26 12:57:01.000000 power-grid-model-1.5.0rc9190015282548/tests/data/power_flow/dummy-test-batch-independent-cacheable/sym_output_batch.json
--rw-r--r--   0 runner    (1001) docker     (123)      148 2023-06-26 12:57:01.000000 power-grid-model-1.5.0rc9190015282548/tests/data/power_flow/dummy-test-batch-independent-cacheable/sym_output_batch.json.license
--rw-r--r--   0 runner    (1001) docker     (123)      466 2023-06-26 12:57:01.000000 power-grid-model-1.5.0rc9190015282548/tests/data/power_flow/dummy-test-batch-independent-cacheable/update_batch.json
--rw-r--r--   0 runner    (1001) docker     (123)      148 2023-06-26 12:57:01.000000 power-grid-model-1.5.0rc9190015282548/tests/data/power_flow/dummy-test-batch-independent-cacheable/update_batch.json.license
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 12:57:57.919412 power-grid-model-1.5.0rc9190015282548/tests/data/power_flow/dummy-test-batch-independent-not-cacheable/
--rw-r--r--   0 runner    (1001) docker     (123)      764 2023-06-26 12:57:01.000000 power-grid-model-1.5.0rc9190015282548/tests/data/power_flow/dummy-test-batch-independent-not-cacheable/input.json
--rw-r--r--   0 runner    (1001) docker     (123)      148 2023-06-26 12:57:01.000000 power-grid-model-1.5.0rc9190015282548/tests/data/power_flow/dummy-test-batch-independent-not-cacheable/input.json.license
--rw-r--r--   0 runner    (1001) docker     (123)       99 2023-06-26 12:57:01.000000 power-grid-model-1.5.0rc9190015282548/tests/data/power_flow/dummy-test-batch-independent-not-cacheable/params.json
--rw-r--r--   0 runner    (1001) docker     (123)      148 2023-06-26 12:57:01.000000 power-grid-model-1.5.0rc9190015282548/tests/data/power_flow/dummy-test-batch-independent-not-cacheable/params.json.license
--rw-r--r--   0 runner    (1001) docker     (123)      107 2023-06-26 12:57:01.000000 power-grid-model-1.5.0rc9190015282548/tests/data/power_flow/dummy-test-batch-independent-not-cacheable/sym_output.json
--rw-r--r--   0 runner    (1001) docker     (123)      148 2023-06-26 12:57:01.000000 power-grid-model-1.5.0rc9190015282548/tests/data/power_flow/dummy-test-batch-independent-not-cacheable/sym_output.json.license
--rw-r--r--   0 runner    (1001) docker     (123)      392 2023-06-26 12:57:01.000000 power-grid-model-1.5.0rc9190015282548/tests/data/power_flow/dummy-test-batch-independent-not-cacheable/sym_output_batch.json
--rw-r--r--   0 runner    (1001) docker     (123)      148 2023-06-26 12:57:01.000000 power-grid-model-1.5.0rc9190015282548/tests/data/power_flow/dummy-test-batch-independent-not-cacheable/sym_output_batch.json.license
--rw-r--r--   0 runner    (1001) docker     (123)      694 2023-06-26 12:57:01.000000 power-grid-model-1.5.0rc9190015282548/tests/data/power_flow/dummy-test-batch-independent-not-cacheable/update_batch.json
--rw-r--r--   0 runner    (1001) docker     (123)      148 2023-06-26 12:57:01.000000 power-grid-model-1.5.0rc9190015282548/tests/data/power_flow/dummy-test-batch-independent-not-cacheable/update_batch.json.license
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 12:57:57.919412 power-grid-model-1.5.0rc9190015282548/tests/data/power_flow/dummy-test-batch-newton/
--rw-r--r--   0 runner    (1001) docker     (123)      764 2023-06-26 12:57:01.000000 power-grid-model-1.5.0rc9190015282548/tests/data/power_flow/dummy-test-batch-newton/input.json
--rw-r--r--   0 runner    (1001) docker     (123)      148 2023-06-26 12:57:01.000000 power-grid-model-1.5.0rc9190015282548/tests/data/power_flow/dummy-test-batch-newton/input.json.license
--rw-r--r--   0 runner    (1001) docker     (123)       99 2023-06-26 12:57:01.000000 power-grid-model-1.5.0rc9190015282548/tests/data/power_flow/dummy-test-batch-newton/params.json
--rw-r--r--   0 runner    (1001) docker     (123)      148 2023-06-26 12:57:01.000000 power-grid-model-1.5.0rc9190015282548/tests/data/power_flow/dummy-test-batch-newton/params.json.license
--rw-r--r--   0 runner    (1001) docker     (123)      107 2023-06-26 12:57:01.000000 power-grid-model-1.5.0rc9190015282548/tests/data/power_flow/dummy-test-batch-newton/sym_output.json
--rw-r--r--   0 runner    (1001) docker     (123)      148 2023-06-26 12:57:01.000000 power-grid-model-1.5.0rc9190015282548/tests/data/power_flow/dummy-test-batch-newton/sym_output.json.license
--rw-r--r--   0 runner    (1001) docker     (123)      476 2023-06-26 12:57:01.000000 power-grid-model-1.5.0rc9190015282548/tests/data/power_flow/dummy-test-batch-newton/sym_output_batch.json
--rw-r--r--   0 runner    (1001) docker     (123)      148 2023-06-26 12:57:01.000000 power-grid-model-1.5.0rc9190015282548/tests/data/power_flow/dummy-test-batch-newton/sym_output_batch.json.license
--rw-r--r--   0 runner    (1001) docker     (123)      400 2023-06-26 12:57:01.000000 power-grid-model-1.5.0rc9190015282548/tests/data/power_flow/dummy-test-batch-newton/update_batch.json
--rw-r--r--   0 runner    (1001) docker     (123)      148 2023-06-26 12:57:01.000000 power-grid-model-1.5.0rc9190015282548/tests/data/power_flow/dummy-test-batch-newton/update_batch.json.license
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 12:57:57.919412 power-grid-model-1.5.0rc9190015282548/tests/data/power_flow/dummy-test-i-n-optional/
--rw-r--r--   0 runner    (1001) docker     (123)     1411 2023-06-26 12:57:01.000000 power-grid-model-1.5.0rc9190015282548/tests/data/power_flow/dummy-test-i-n-optional/input.json
--rw-r--r--   0 runner    (1001) docker     (123)      148 2023-06-26 12:57:01.000000 power-grid-model-1.5.0rc9190015282548/tests/data/power_flow/dummy-test-i-n-optional/input.json.license
--rw-r--r--   0 runner    (1001) docker     (123)       99 2023-06-26 12:57:01.000000 power-grid-model-1.5.0rc9190015282548/tests/data/power_flow/dummy-test-i-n-optional/params.json
--rw-r--r--   0 runner    (1001) docker     (123)      148 2023-06-26 12:57:01.000000 power-grid-model-1.5.0rc9190015282548/tests/data/power_flow/dummy-test-i-n-optional/params.json.license
--rw-r--r--   0 runner    (1001) docker     (123)      666 2023-06-26 12:57:01.000000 power-grid-model-1.5.0rc9190015282548/tests/data/power_flow/dummy-test-i-n-optional/sym_output.json
--rw-r--r--   0 runner    (1001) docker     (123)      148 2023-06-26 12:57:01.000000 power-grid-model-1.5.0rc9190015282548/tests/data/power_flow/dummy-test-i-n-optional/sym_output.json.license
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 12:57:57.923412 power-grid-model-1.5.0rc9190015282548/tests/data/power_flow/gaia-example/
--rw-r--r--   0 runner    (1001) docker     (123)      678 2023-06-26 12:57:01.000000 power-grid-model-1.5.0rc9190015282548/tests/data/power_flow/gaia-example/asym_output.json
--rw-r--r--   0 runner    (1001) docker     (123)      148 2023-06-26 12:57:01.000000 power-grid-model-1.5.0rc9190015282548/tests/data/power_flow/gaia-example/asym_output.json.license
--rw-r--r--   0 runner    (1001) docker     (123)     2631 2023-06-26 12:57:01.000000 power-grid-model-1.5.0rc9190015282548/tests/data/power_flow/gaia-example/gaia_grid.gnf
--rw-r--r--   0 runner    (1001) docker     (123)      148 2023-06-26 12:57:01.000000 power-grid-model-1.5.0rc9190015282548/tests/data/power_flow/gaia-example/gaia_grid.gnf.license
--rw-r--r--   0 runner    (1001) docker     (123)     1638 2023-06-26 12:57:01.000000 power-grid-model-1.5.0rc9190015282548/tests/data/power_flow/gaia-example/input.json
--rw-r--r--   0 runner    (1001) docker     (123)      148 2023-06-26 12:57:01.000000 power-grid-model-1.5.0rc9190015282548/tests/data/power_flow/gaia-example/input.json.license
--rw-r--r--   0 runner    (1001) docker     (123)      100 2023-06-26 12:57:01.000000 power-grid-model-1.5.0rc9190015282548/tests/data/power_flow/gaia-example/params.json
--rw-r--r--   0 runner    (1001) docker     (123)      148 2023-06-26 12:57:01.000000 power-grid-model-1.5.0rc9190015282548/tests/data/power_flow/gaia-example/params.json.license
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 12:57:57.923412 power-grid-model-1.5.0rc9190015282548/tests/data/power_flow/multi-source-with-angle/
--rw-r--r--   0 runner    (1001) docker     (123)     1088 2023-06-26 12:57:01.000000 power-grid-model-1.5.0rc9190015282548/tests/data/power_flow/multi-source-with-angle/input.json
--rw-r--r--   0 runner    (1001) docker     (123)      148 2023-06-26 12:57:01.000000 power-grid-model-1.5.0rc9190015282548/tests/data/power_flow/multi-source-with-angle/input.json.license
--rw-r--r--   0 runner    (1001) docker     (123)      111 2023-06-26 12:57:01.000000 power-grid-model-1.5.0rc9190015282548/tests/data/power_flow/multi-source-with-angle/params.json
--rw-r--r--   0 runner    (1001) docker     (123)      148 2023-06-26 12:57:01.000000 power-grid-model-1.5.0rc9190015282548/tests/data/power_flow/multi-source-with-angle/params.json.license
--rw-r--r--   0 runner    (1001) docker     (123)      399 2023-06-26 12:57:01.000000 power-grid-model-1.5.0rc9190015282548/tests/data/power_flow/multi-source-with-angle/sym_output.json
--rw-r--r--   0 runner    (1001) docker     (123)      148 2023-06-26 12:57:01.000000 power-grid-model-1.5.0rc9190015282548/tests/data/power_flow/multi-source-with-angle/sym_output.json.license
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 12:57:57.887410 power-grid-model-1.5.0rc9190015282548/tests/data/power_flow/pandapower/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 12:57:57.887410 power-grid-model-1.5.0rc9190015282548/tests/data/power_flow/pandapower/components/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 12:57:57.887410 power-grid-model-1.5.0rc9190015282548/tests/data/power_flow/pandapower/components/asymmetric/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 12:57:57.923412 power-grid-model-1.5.0rc9190015282548/tests/data/power_flow/pandapower/components/asymmetric/asym_gen/
--rw-r--r--   0 runner    (1001) docker     (123)      672 2023-06-26 12:57:01.000000 power-grid-model-1.5.0rc9190015282548/tests/data/power_flow/pandapower/components/asymmetric/asym_gen/README.md
--rw-r--r--   0 runner    (1001) docker     (123)     1743 2023-06-26 12:57:01.000000 power-grid-model-1.5.0rc9190015282548/tests/data/power_flow/pandapower/components/asymmetric/asym_gen/asym_output.json
--rw-r--r--   0 runner    (1001) docker     (123)      148 2023-06-26 12:57:01.000000 power-grid-model-1.5.0rc9190015282548/tests/data/power_flow/pandapower/components/asymmetric/asym_gen/asym_output.json.license
--rw-r--r--   0 runner    (1001) docker     (123)     1089 2023-06-26 12:57:01.000000 power-grid-model-1.5.0rc9190015282548/tests/data/power_flow/pandapower/components/asymmetric/asym_gen/input.json
--rw-r--r--   0 runner    (1001) docker     (123)      148 2023-06-26 12:57:01.000000 power-grid-model-1.5.0rc9190015282548/tests/data/power_flow/pandapower/components/asymmetric/asym_gen/input.json.license
--rw-r--r--   0 runner    (1001) docker     (123)      101 2023-06-26 12:57:01.000000 power-grid-model-1.5.0rc9190015282548/tests/data/power_flow/pandapower/components/asymmetric/asym_gen/params.json
--rw-r--r--   0 runner    (1001) docker     (123)      148 2023-06-26 12:57:01.000000 power-grid-model-1.5.0rc9190015282548/tests/data/power_flow/pandapower/components/asymmetric/asym_gen/params.json.license
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 12:57:57.923412 power-grid-model-1.5.0rc9190015282548/tests/data/power_flow/pandapower/components/asymmetric/asym_load/
--rw-r--r--   0 runner    (1001) docker     (123)      659 2023-06-26 12:57:01.000000 power-grid-model-1.5.0rc9190015282548/tests/data/power_flow/pandapower/components/asymmetric/asym_load/README.md
--rw-r--r--   0 runner    (1001) docker     (123)     1749 2023-06-26 12:57:01.000000 power-grid-model-1.5.0rc9190015282548/tests/data/power_flow/pandapower/components/asymmetric/asym_load/asym_output.json
--rw-r--r--   0 runner    (1001) docker     (123)      148 2023-06-26 12:57:01.000000 power-grid-model-1.5.0rc9190015282548/tests/data/power_flow/pandapower/components/asymmetric/asym_load/asym_output.json.license
--rw-r--r--   0 runner    (1001) docker     (123)     1090 2023-06-26 12:57:01.000000 power-grid-model-1.5.0rc9190015282548/tests/data/power_flow/pandapower/components/asymmetric/asym_load/input.json
--rw-r--r--   0 runner    (1001) docker     (123)      148 2023-06-26 12:57:01.000000 power-grid-model-1.5.0rc9190015282548/tests/data/power_flow/pandapower/components/asymmetric/asym_load/input.json.license
--rw-r--r--   0 runner    (1001) docker     (123)      101 2023-06-26 12:57:01.000000 power-grid-model-1.5.0rc9190015282548/tests/data/power_flow/pandapower/components/asymmetric/asym_load/params.json
--rw-r--r--   0 runner    (1001) docker     (123)      148 2023-06-26 12:57:01.000000 power-grid-model-1.5.0rc9190015282548/tests/data/power_flow/pandapower/components/asymmetric/asym_load/params.json.license
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 12:57:57.927412 power-grid-model-1.5.0rc9190015282548/tests/data/power_flow/pandapower/components/asymmetric/line/
--rw-r--r--   0 runner    (1001) docker     (123)      910 2023-06-26 12:57:01.000000 power-grid-model-1.5.0rc9190015282548/tests/data/power_flow/pandapower/components/asymmetric/line/README.md
--rw-r--r--   0 runner    (1001) docker     (123)     3462 2023-06-26 12:57:01.000000 power-grid-model-1.5.0rc9190015282548/tests/data/power_flow/pandapower/components/asymmetric/line/asym_output.json
--rw-r--r--   0 runner    (1001) docker     (123)      148 2023-06-26 12:57:01.000000 power-grid-model-1.5.0rc9190015282548/tests/data/power_flow/pandapower/components/asymmetric/line/asym_output.json.license
--rw-r--r--   0 runner    (1001) docker     (123)     2031 2023-06-26 12:57:01.000000 power-grid-model-1.5.0rc9190015282548/tests/data/power_flow/pandapower/components/asymmetric/line/input.json
--rw-r--r--   0 runner    (1001) docker     (123)      148 2023-06-26 12:57:01.000000 power-grid-model-1.5.0rc9190015282548/tests/data/power_flow/pandapower/components/asymmetric/line/input.json.license
--rw-r--r--   0 runner    (1001) docker     (123)      101 2023-06-26 12:57:01.000000 power-grid-model-1.5.0rc9190015282548/tests/data/power_flow/pandapower/components/asymmetric/line/params.json
--rw-r--r--   0 runner    (1001) docker     (123)      148 2023-06-26 12:57:01.000000 power-grid-model-1.5.0rc9190015282548/tests/data/power_flow/pandapower/components/asymmetric/line/params.json.license
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 12:57:57.927412 power-grid-model-1.5.0rc9190015282548/tests/data/power_flow/pandapower/components/asymmetric/node/
--rw-r--r--   0 runner    (1001) docker     (123)      595 2023-06-26 12:57:01.000000 power-grid-model-1.5.0rc9190015282548/tests/data/power_flow/pandapower/components/asymmetric/node/README.md
--rw-r--r--   0 runner    (1001) docker     (123)     1635 2023-06-26 12:57:01.000000 power-grid-model-1.5.0rc9190015282548/tests/data/power_flow/pandapower/components/asymmetric/node/asym_output.json
--rw-r--r--   0 runner    (1001) docker     (123)      148 2023-06-26 12:57:01.000000 power-grid-model-1.5.0rc9190015282548/tests/data/power_flow/pandapower/components/asymmetric/node/asym_output.json.license
--rw-r--r--   0 runner    (1001) docker     (123)      642 2023-06-26 12:57:01.000000 power-grid-model-1.5.0rc9190015282548/tests/data/power_flow/pandapower/components/asymmetric/node/input.json
--rw-r--r--   0 runner    (1001) docker     (123)      148 2023-06-26 12:57:01.000000 power-grid-model-1.5.0rc9190015282548/tests/data/power_flow/pandapower/components/asymmetric/node/input.json.license
--rw-r--r--   0 runner    (1001) docker     (123)      100 2023-06-26 12:57:01.000000 power-grid-model-1.5.0rc9190015282548/tests/data/power_flow/pandapower/components/asymmetric/node/params.json
--rw-r--r--   0 runner    (1001) docker     (123)      148 2023-06-26 12:57:01.000000 power-grid-model-1.5.0rc9190015282548/tests/data/power_flow/pandapower/components/asymmetric/node/params.json.license
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 12:57:57.927412 power-grid-model-1.5.0rc9190015282548/tests/data/power_flow/pandapower/components/asymmetric/shunt/
--rw-r--r--   0 runner    (1001) docker     (123)      629 2023-06-26 12:57:01.000000 power-grid-model-1.5.0rc9190015282548/tests/data/power_flow/pandapower/components/asymmetric/shunt/README.md
--rw-r--r--   0 runner    (1001) docker     (123)     1385 2023-06-26 12:57:01.000000 power-grid-model-1.5.0rc9190015282548/tests/data/power_flow/pandapower/components/asymmetric/shunt/asym_output.json
--rw-r--r--   0 runner    (1001) docker     (123)      148 2023-06-26 12:57:01.000000 power-grid-model-1.5.0rc9190015282548/tests/data/power_flow/pandapower/components/asymmetric/shunt/asym_output.json.license
--rw-r--r--   0 runner    (1001) docker     (123)      884 2023-06-26 12:57:01.000000 power-grid-model-1.5.0rc9190015282548/tests/data/power_flow/pandapower/components/asymmetric/shunt/input.json
--rw-r--r--   0 runner    (1001) docker     (123)      148 2023-06-26 12:57:01.000000 power-grid-model-1.5.0rc9190015282548/tests/data/power_flow/pandapower/components/asymmetric/shunt/input.json.license
--rw-r--r--   0 runner    (1001) docker     (123)      101 2023-06-26 12:57:01.000000 power-grid-model-1.5.0rc9190015282548/tests/data/power_flow/pandapower/components/asymmetric/shunt/params.json
--rw-r--r--   0 runner    (1001) docker     (123)      148 2023-06-26 12:57:01.000000 power-grid-model-1.5.0rc9190015282548/tests/data/power_flow/pandapower/components/asymmetric/shunt/params.json.license
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 12:57:57.927412 power-grid-model-1.5.0rc9190015282548/tests/data/power_flow/pandapower/components/asymmetric/source/
--rw-r--r--   0 runner    (1001) docker     (123)      579 2023-06-26 12:57:01.000000 power-grid-model-1.5.0rc9190015282548/tests/data/power_flow/pandapower/components/asymmetric/source/README.md
--rw-r--r--   0 runner    (1001) docker     (123)     2453 2023-06-26 12:57:01.000000 power-grid-model-1.5.0rc9190015282548/tests/data/power_flow/pandapower/components/asymmetric/source/asym_output.json
--rw-r--r--   0 runner    (1001) docker     (123)      148 2023-06-26 12:57:01.000000 power-grid-model-1.5.0rc9190015282548/tests/data/power_flow/pandapower/components/asymmetric/source/asym_output.json.license
--rw-r--r--   0 runner    (1001) docker     (123)     1073 2023-06-26 12:57:01.000000 power-grid-model-1.5.0rc9190015282548/tests/data/power_flow/pandapower/components/asymmetric/source/input.json
--rw-r--r--   0 runner    (1001) docker     (123)      148 2023-06-26 12:57:01.000000 power-grid-model-1.5.0rc9190015282548/tests/data/power_flow/pandapower/components/asymmetric/source/input.json.license
--rw-r--r--   0 runner    (1001) docker     (123)      101 2023-06-26 12:57:01.000000 power-grid-model-1.5.0rc9190015282548/tests/data/power_flow/pandapower/components/asymmetric/source/params.json
--rw-r--r--   0 runner    (1001) docker     (123)      148 2023-06-26 12:57:01.000000 power-grid-model-1.5.0rc9190015282548/tests/data/power_flow/pandapower/components/asymmetric/source/params.json.license
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 12:57:57.931412 power-grid-model-1.5.0rc9190015282548/tests/data/power_flow/pandapower/components/asymmetric/sym_gen/
--rw-r--r--   0 runner    (1001) docker     (123)      853 2023-06-26 12:57:01.000000 power-grid-model-1.5.0rc9190015282548/tests/data/power_flow/pandapower/components/asymmetric/sym_gen/README.md
--rw-r--r--   0 runner    (1001) docker     (123)     1803 2023-06-26 12:57:01.000000 power-grid-model-1.5.0rc9190015282548/tests/data/power_flow/pandapower/components/asymmetric/sym_gen/asym_output.json
--rw-r--r--   0 runner    (1001) docker     (123)      148 2023-06-26 12:57:01.000000 power-grid-model-1.5.0rc9190015282548/tests/data/power_flow/pandapower/components/asymmetric/sym_gen/asym_output.json.license
--rw-r--r--   0 runner    (1001) docker     (123)      886 2023-06-26 12:57:01.000000 power-grid-model-1.5.0rc9190015282548/tests/data/power_flow/pandapower/components/asymmetric/sym_gen/input.json
--rw-r--r--   0 runner    (1001) docker     (123)      148 2023-06-26 12:57:01.000000 power-grid-model-1.5.0rc9190015282548/tests/data/power_flow/pandapower/components/asymmetric/sym_gen/input.json.license
--rw-r--r--   0 runner    (1001) docker     (123)      101 2023-06-26 12:57:01.000000 power-grid-model-1.5.0rc9190015282548/tests/data/power_flow/pandapower/components/asymmetric/sym_gen/params.json
--rw-r--r--   0 runner    (1001) docker     (123)      148 2023-06-26 12:57:01.000000 power-grid-model-1.5.0rc9190015282548/tests/data/power_flow/pandapower/components/asymmetric/sym_gen/params.json.license
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 12:57:57.931412 power-grid-model-1.5.0rc9190015282548/tests/data/power_flow/pandapower/components/asymmetric/sym_load/
--rw-r--r--   0 runner    (1001) docker     (123)      841 2023-06-26 12:57:01.000000 power-grid-model-1.5.0rc9190015282548/tests/data/power_flow/pandapower/components/asymmetric/sym_load/README.md
--rw-r--r--   0 runner    (1001) docker     (123)     1802 2023-06-26 12:57:01.000000 power-grid-model-1.5.0rc9190015282548/tests/data/power_flow/pandapower/components/asymmetric/sym_load/asym_output.json
--rw-r--r--   0 runner    (1001) docker     (123)      148 2023-06-26 12:57:01.000000 power-grid-model-1.5.0rc9190015282548/tests/data/power_flow/pandapower/components/asymmetric/sym_load/asym_output.json.license
--rw-r--r--   0 runner    (1001) docker     (123)      887 2023-06-26 12:57:01.000000 power-grid-model-1.5.0rc9190015282548/tests/data/power_flow/pandapower/components/asymmetric/sym_load/input.json
--rw-r--r--   0 runner    (1001) docker     (123)      148 2023-06-26 12:57:01.000000 power-grid-model-1.5.0rc9190015282548/tests/data/power_flow/pandapower/components/asymmetric/sym_load/input.json.license
--rw-r--r--   0 runner    (1001) docker     (123)      101 2023-06-26 12:57:01.000000 power-grid-model-1.5.0rc9190015282548/tests/data/power_flow/pandapower/components/asymmetric/sym_load/params.json
--rw-r--r--   0 runner    (1001) docker     (123)      148 2023-06-26 12:57:01.000000 power-grid-model-1.5.0rc9190015282548/tests/data/power_flow/pandapower/components/asymmetric/sym_load/params.json.license
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 12:57:57.931412 power-grid-model-1.5.0rc9190015282548/tests/data/power_flow/pandapower/components/asymmetric/transformer/
--rw-r--r--   0 runner    (1001) docker     (123)     1065 2023-06-26 12:57:01.000000 power-grid-model-1.5.0rc9190015282548/tests/data/power_flow/pandapower/components/asymmetric/transformer/README.md
--rw-r--r--   0 runner    (1001) docker     (123)    17633 2023-06-26 12:57:01.000000 power-grid-model-1.5.0rc9190015282548/tests/data/power_flow/pandapower/components/asymmetric/transformer/asym_output_batch.json
--rw-r--r--   0 runner    (1001) docker     (123)      148 2023-06-26 12:57:01.000000 power-grid-model-1.5.0rc9190015282548/tests/data/power_flow/pandapower/components/asymmetric/transformer/asym_output_batch.json.license
--rw-r--r--   0 runner    (1001) docker     (123)      919 2023-06-26 12:57:01.000000 power-grid-model-1.5.0rc9190015282548/tests/data/power_flow/pandapower/components/asymmetric/transformer/input.json
--rw-r--r--   0 runner    (1001) docker     (123)      148 2023-06-26 12:57:01.000000 power-grid-model-1.5.0rc9190015282548/tests/data/power_flow/pandapower/components/asymmetric/transformer/input.json.license
--rw-r--r--   0 runner    (1001) docker     (123)      102 2023-06-26 12:57:01.000000 power-grid-model-1.5.0rc9190015282548/tests/data/power_flow/pandapower/components/asymmetric/transformer/params.json
--rw-r--r--   0 runner    (1001) docker     (123)      148 2023-06-26 12:57:01.000000 power-grid-model-1.5.0rc9190015282548/tests/data/power_flow/pandapower/components/asymmetric/transformer/params.json.license
--rw-r--r--   0 runner    (1001) docker     (123)      997 2023-06-26 12:57:01.000000 power-grid-model-1.5.0rc9190015282548/tests/data/power_flow/pandapower/components/asymmetric/transformer/update_batch.json
--rw-r--r--   0 runner    (1001) docker     (123)      148 2023-06-26 12:57:01.000000 power-grid-model-1.5.0rc9190015282548/tests/data/power_flow/pandapower/components/asymmetric/transformer/update_batch.json.license
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 12:57:57.887410 power-grid-model-1.5.0rc9190015282548/tests/data/power_flow/pandapower/components/symmetric/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 12:57:57.935413 power-grid-model-1.5.0rc9190015282548/tests/data/power_flow/pandapower/components/symmetric/basic-node/
--rw-r--r--   0 runner    (1001) docker     (123)      448 2023-06-26 12:57:01.000000 power-grid-model-1.5.0rc9190015282548/tests/data/power_flow/pandapower/components/symmetric/basic-node/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      299 2023-06-26 12:57:01.000000 power-grid-model-1.5.0rc9190015282548/tests/data/power_flow/pandapower/components/symmetric/basic-node/input.json
--rw-r--r--   0 runner    (1001) docker     (123)      148 2023-06-26 12:57:01.000000 power-grid-model-1.5.0rc9190015282548/tests/data/power_flow/pandapower/components/symmetric/basic-node/input.json.license
--rw-r--r--   0 runner    (1001) docker     (123)      101 2023-06-26 12:57:01.000000 power-grid-model-1.5.0rc9190015282548/tests/data/power_flow/pandapower/components/symmetric/basic-node/params.json
--rw-r--r--   0 runner    (1001) docker     (123)      148 2023-06-26 12:57:01.000000 power-grid-model-1.5.0rc9190015282548/tests/data/power_flow/pandapower/components/symmetric/basic-node/params.json.license
--rw-r--r--   0 runner    (1001) docker     (123)      301 2023-06-26 12:57:01.000000 power-grid-model-1.5.0rc9190015282548/tests/data/power_flow/pandapower/components/symmetric/basic-node/sym_output.json
--rw-r--r--   0 runner    (1001) docker     (123)      148 2023-06-26 12:57:01.000000 power-grid-model-1.5.0rc9190015282548/tests/data/power_flow/pandapower/components/symmetric/basic-node/sym_output.json.license
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 12:57:57.935413 power-grid-model-1.5.0rc9190015282548/tests/data/power_flow/pandapower/components/symmetric/line/
--rw-r--r--   0 runner    (1001) docker     (123)      775 2023-06-26 12:57:01.000000 power-grid-model-1.5.0rc9190015282548/tests/data/power_flow/pandapower/components/symmetric/line/README.md
--rw-r--r--   0 runner    (1001) docker     (123)     1938 2023-06-26 12:57:01.000000 power-grid-model-1.5.0rc9190015282548/tests/data/power_flow/pandapower/components/symmetric/line/input.json
--rw-r--r--   0 runner    (1001) docker     (123)      148 2023-06-26 12:57:01.000000 power-grid-model-1.5.0rc9190015282548/tests/data/power_flow/pandapower/components/symmetric/line/input.json.license
--rw-r--r--   0 runner    (1001) docker     (123)      101 2023-06-26 12:57:01.000000 power-grid-model-1.5.0rc9190015282548/tests/data/power_flow/pandapower/components/symmetric/line/params.json
--rw-r--r--   0 runner    (1001) docker     (123)      148 2023-06-26 12:57:01.000000 power-grid-model-1.5.0rc9190015282548/tests/data/power_flow/pandapower/components/symmetric/line/params.json.license
--rw-r--r--   0 runner    (1001) docker     (123)     2305 2023-06-26 12:57:01.000000 power-grid-model-1.5.0rc9190015282548/tests/data/power_flow/pandapower/components/symmetric/line/sym_output.json
--rw-r--r--   0 runner    (1001) docker     (123)      148 2023-06-26 12:57:01.000000 power-grid-model-1.5.0rc9190015282548/tests/data/power_flow/pandapower/components/symmetric/line/sym_output.json.license
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 12:57:57.939413 power-grid-model-1.5.0rc9190015282548/tests/data/power_flow/pandapower/components/symmetric/node/
--rw-r--r--   0 runner    (1001) docker     (123)      462 2023-06-26 12:57:01.000000 power-grid-model-1.5.0rc9190015282548/tests/data/power_flow/pandapower/components/symmetric/node/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      651 2023-06-26 12:57:01.000000 power-grid-model-1.5.0rc9190015282548/tests/data/power_flow/pandapower/components/symmetric/node/input.json
--rw-r--r--   0 runner    (1001) docker     (123)      148 2023-06-26 12:57:01.000000 power-grid-model-1.5.0rc9190015282548/tests/data/power_flow/pandapower/components/symmetric/node/input.json.license
--rw-r--r--   0 runner    (1001) docker     (123)      101 2023-06-26 12:57:01.000000 power-grid-model-1.5.0rc9190015282548/tests/data/power_flow/pandapower/components/symmetric/node/params.json
--rw-r--r--   0 runner    (1001) docker     (123)      148 2023-06-26 12:57:01.000000 power-grid-model-1.5.0rc9190015282548/tests/data/power_flow/pandapower/components/symmetric/node/params.json.license
--rw-r--r--   0 runner    (1001) docker     (123)      907 2023-06-26 12:57:01.000000 power-grid-model-1.5.0rc9190015282548/tests/data/power_flow/pandapower/components/symmetric/node/sym_output.json
--rw-r--r--   0 runner    (1001) docker     (123)      148 2023-06-26 12:57:01.000000 power-grid-model-1.5.0rc9190015282548/tests/data/power_flow/pandapower/components/symmetric/node/sym_output.json.license
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 12:57:57.943413 power-grid-model-1.5.0rc9190015282548/tests/data/power_flow/pandapower/components/symmetric/shunt/
--rw-r--r--   0 runner    (1001) docker     (123)      496 2023-06-26 12:57:01.000000 power-grid-model-1.5.0rc9190015282548/tests/data/power_flow/pandapower/components/symmetric/shunt/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      892 2023-06-26 12:57:01.000000 power-grid-model-1.5.0rc9190015282548/tests/data/power_flow/pandapower/components/symmetric/shunt/input.json
--rw-r--r--   0 runner    (1001) docker     (123)      148 2023-06-26 12:57:01.000000 power-grid-model-1.5.0rc9190015282548/tests/data/power_flow/pandapower/components/symmetric/shunt/input.json.license
--rw-r--r--   0 runner    (1001) docker     (123)      101 2023-06-26 12:57:01.000000 power-grid-model-1.5.0rc9190015282548/tests/data/power_flow/pandapower/components/symmetric/shunt/params.json
--rw-r--r--   0 runner    (1001) docker     (123)      148 2023-06-26 12:57:01.000000 power-grid-model-1.5.0rc9190015282548/tests/data/power_flow/pandapower/components/symmetric/shunt/params.json.license
--rw-r--r--   0 runner    (1001) docker     (123)      977 2023-06-26 12:57:01.000000 power-grid-model-1.5.0rc9190015282548/tests/data/power_flow/pandapower/components/symmetric/shunt/sym_output.json
--rw-r--r--   0 runner    (1001) docker     (123)      148 2023-06-26 12:57:01.000000 power-grid-model-1.5.0rc9190015282548/tests/data/power_flow/pandapower/components/symmetric/shunt/sym_output.json.license
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 12:57:57.943413 power-grid-model-1.5.0rc9190015282548/tests/data/power_flow/pandapower/components/symmetric/source/
--rw-r--r--   0 runner    (1001) docker     (123)      483 2023-06-26 12:57:01.000000 power-grid-model-1.5.0rc9190015282548/tests/data/power_flow/pandapower/components/symmetric/source/README.md
--rw-r--r--   0 runner    (1001) docker     (123)     1089 2023-06-26 12:57:01.000000 power-grid-model-1.5.0rc9190015282548/tests/data/power_flow/pandapower/components/symmetric/source/input.json
--rw-r--r--   0 runner    (1001) docker     (123)      148 2023-06-26 12:57:01.000000 power-grid-model-1.5.0rc9190015282548/tests/data/power_flow/pandapower/components/symmetric/source/input.json.license
--rw-r--r--   0 runner    (1001) docker     (123)      101 2023-06-26 12:57:01.000000 power-grid-model-1.5.0rc9190015282548/tests/data/power_flow/pandapower/components/symmetric/source/params.json
--rw-r--r--   0 runner    (1001) docker     (123)      148 2023-06-26 12:57:01.000000 power-grid-model-1.5.0rc9190015282548/tests/data/power_flow/pandapower/components/symmetric/source/params.json.license
--rw-r--r--   0 runner    (1001) docker     (123)     1461 2023-06-26 12:57:01.000000 power-grid-model-1.5.0rc9190015282548/tests/data/power_flow/pandapower/components/symmetric/source/sym_output.json
--rw-r--r--   0 runner    (1001) docker     (123)      148 2023-06-26 12:57:01.000000 power-grid-model-1.5.0rc9190015282548/tests/data/power_flow/pandapower/components/symmetric/source/sym_output.json.license
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 12:57:57.947413 power-grid-model-1.5.0rc9190015282548/tests/data/power_flow/pandapower/components/symmetric/sym_gen/
--rw-r--r--   0 runner    (1001) docker     (123)      753 2023-06-26 12:57:01.000000 power-grid-model-1.5.0rc9190015282548/tests/data/power_flow/pandapower/components/symmetric/sym_gen/README.md
--rw-r--r--   0 runner    (1001) docker     (123)     1172 2023-06-26 12:57:01.000000 power-grid-model-1.5.0rc9190015282548/tests/data/power_flow/pandapower/components/symmetric/sym_gen/input.json
--rw-r--r--   0 runner    (1001) docker     (123)      148 2023-06-26 12:57:01.000000 power-grid-model-1.5.0rc9190015282548/tests/data/power_flow/pandapower/components/symmetric/sym_gen/input.json.license
--rw-r--r--   0 runner    (1001) docker     (123)      101 2023-06-26 12:57:01.000000 power-grid-model-1.5.0rc9190015282548/tests/data/power_flow/pandapower/components/symmetric/sym_gen/params.json
--rw-r--r--   0 runner    (1001) docker     (123)      148 2023-06-26 12:57:01.000000 power-grid-model-1.5.0rc9190015282548/tests/data/power_flow/pandapower/components/symmetric/sym_gen/params.json.license
--rw-r--r--   0 runner    (1001) docker     (123)     1136 2023-06-26 12:57:01.000000 power-grid-model-1.5.0rc9190015282548/tests/data/power_flow/pandapower/components/symmetric/sym_gen/sym_output.json
--rw-r--r--   0 runner    (1001) docker     (123)      148 2023-06-26 12:57:01.000000 power-grid-model-1.5.0rc9190015282548/tests/data/power_flow/pandapower/components/symmetric/sym_gen/sym_output.json.license
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 12:57:57.947413 power-grid-model-1.5.0rc9190015282548/tests/data/power_flow/pandapower/components/symmetric/sym_load/
--rw-r--r--   0 runner    (1001) docker     (123)      741 2023-06-26 12:57:01.000000 power-grid-model-1.5.0rc9190015282548/tests/data/power_flow/pandapower/components/symmetric/sym_load/README.md
--rw-r--r--   0 runner    (1001) docker     (123)     1173 2023-06-26 12:57:01.000000 power-grid-model-1.5.0rc9190015282548/tests/data/power_flow/pandapower/components/symmetric/sym_load/input.json
--rw-r--r--   0 runner    (1001) docker     (123)      148 2023-06-26 12:57:01.000000 power-grid-model-1.5.0rc9190015282548/tests/data/power_flow/pandapower/components/symmetric/sym_load/input.json.license
--rw-r--r--   0 runner    (1001) docker     (123)       78 2023-06-26 12:57:01.000000 power-grid-model-1.5.0rc9190015282548/tests/data/power_flow/pandapower/components/symmetric/sym_load/params.json
--rw-r--r--   0 runner    (1001) docker     (123)      148 2023-06-26 12:57:01.000000 power-grid-model-1.5.0rc9190015282548/tests/data/power_flow/pandapower/components/symmetric/sym_load/params.json.license
--rw-r--r--   0 runner    (1001) docker     (123)     1131 2023-06-26 12:57:01.000000 power-grid-model-1.5.0rc9190015282548/tests/data/power_flow/pandapower/components/symmetric/sym_load/sym_output.json
--rw-r--r--   0 runner    (1001) docker     (123)      148 2023-06-26 12:57:01.000000 power-grid-model-1.5.0rc9190015282548/tests/data/power_flow/pandapower/components/symmetric/sym_load/sym_output.json.license
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 12:57:57.947413 power-grid-model-1.5.0rc9190015282548/tests/data/power_flow/pandapower/components/symmetric/three_winding_transformer/
--rw-r--r--   0 runner    (1001) docker     (123)      917 2023-06-26 12:57:01.000000 power-grid-model-1.5.0rc9190015282548/tests/data/power_flow/pandapower/components/symmetric/three_winding_transformer/README.md
--rw-r--r--   0 runner    (1001) docker     (123)     1095 2023-06-26 12:57:01.000000 power-grid-model-1.5.0rc9190015282548/tests/data/power_flow/pandapower/components/symmetric/three_winding_transformer/input.json
--rw-r--r--   0 runner    (1001) docker     (123)      148 2023-06-26 12:57:01.000000 power-grid-model-1.5.0rc9190015282548/tests/data/power_flow/pandapower/components/symmetric/three_winding_transformer/input.json.license
--rw-r--r--   0 runner    (1001) docker     (123)       78 2023-06-26 12:57:01.000000 power-grid-model-1.5.0rc9190015282548/tests/data/power_flow/pandapower/components/symmetric/three_winding_transformer/params.json
--rw-r--r--   0 runner    (1001) docker     (123)      148 2023-06-26 12:57:01.000000 power-grid-model-1.5.0rc9190015282548/tests/data/power_flow/pandapower/components/symmetric/three_winding_transformer/params.json.license
--rw-r--r--   0 runner    (1001) docker     (123)     8883 2023-06-26 12:57:01.000000 power-grid-model-1.5.0rc9190015282548/tests/data/power_flow/pandapower/components/symmetric/three_winding_transformer/sym_output_batch.json
--rw-r--r--   0 runner    (1001) docker     (123)      148 2023-06-26 12:57:01.000000 power-grid-model-1.5.0rc9190015282548/tests/data/power_flow/pandapower/components/symmetric/three_winding_transformer/sym_output_batch.json.license
--rw-r--r--   0 runner    (1001) docker     (123)     1737 2023-06-26 12:57:01.000000 power-grid-model-1.5.0rc9190015282548/tests/data/power_flow/pandapower/components/symmetric/three_winding_transformer/update_batch.json
--rw-r--r--   0 runner    (1001) docker     (123)      148 2023-06-26 12:57:01.000000 power-grid-model-1.5.0rc9190015282548/tests/data/power_flow/pandapower/components/symmetric/three_winding_transformer/update_batch.json.license
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 12:57:57.951413 power-grid-model-1.5.0rc9190015282548/tests/data/power_flow/pandapower/components/symmetric/transformer/
--rw-r--r--   0 runner    (1001) docker     (123)      883 2023-06-26 12:57:01.000000 power-grid-model-1.5.0rc9190015282548/tests/data/power_flow/pandapower/components/symmetric/transformer/README.md
--rw-r--r--   0 runner    (1001) docker     (123)     2275 2023-06-26 12:57:01.000000 power-grid-model-1.5.0rc9190015282548/tests/data/power_flow/pandapower/components/symmetric/transformer/input.json
--rw-r--r--   0 runner    (1001) docker     (123)      148 2023-06-26 12:57:01.000000 power-grid-model-1.5.0rc9190015282548/tests/data/power_flow/pandapower/components/symmetric/transformer/input.json.license
--rw-r--r--   0 runner    (1001) docker     (123)      101 2023-06-26 12:57:01.000000 power-grid-model-1.5.0rc9190015282548/tests/data/power_flow/pandapower/components/symmetric/transformer/params.json
--rw-r--r--   0 runner    (1001) docker     (123)      148 2023-06-26 12:57:01.000000 power-grid-model-1.5.0rc9190015282548/tests/data/power_flow/pandapower/components/symmetric/transformer/params.json.license
--rw-r--r--   0 runner    (1001) docker     (123)    15639 2023-06-26 12:57:01.000000 power-grid-model-1.5.0rc9190015282548/tests/data/power_flow/pandapower/components/symmetric/transformer/sym_output_batch.json
--rw-r--r--   0 runner    (1001) docker     (123)      148 2023-06-26 12:57:01.000000 power-grid-model-1.5.0rc9190015282548/tests/data/power_flow/pandapower/components/symmetric/transformer/sym_output_batch.json.license
--rw-r--r--   0 runner    (1001) docker     (123)     2827 2023-06-26 12:57:01.000000 power-grid-model-1.5.0rc9190015282548/tests/data/power_flow/pandapower/components/symmetric/transformer/update_batch.json
--rw-r--r--   0 runner    (1001) docker     (123)      148 2023-06-26 12:57:01.000000 power-grid-model-1.5.0rc9190015282548/tests/data/power_flow/pandapower/components/symmetric/transformer/update_batch.json.license
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 12:57:57.891410 power-grid-model-1.5.0rc9190015282548/tests/data/power_flow/pandapower/networks/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 12:57:57.891410 power-grid-model-1.5.0rc9190015282548/tests/data/power_flow/pandapower/networks/asymmetric/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 12:57:57.951413 power-grid-model-1.5.0rc9190015282548/tests/data/power_flow/pandapower/networks/asymmetric/distribution-case/
--rw-r--r--   0 runner    (1001) docker     (123)     1281 2023-06-26 12:57:01.000000 power-grid-model-1.5.0rc9190015282548/tests/data/power_flow/pandapower/networks/asymmetric/distribution-case/README.md
--rw-r--r--   0 runner    (1001) docker     (123)    15865 2023-06-26 12:57:01.000000 power-grid-model-1.5.0rc9190015282548/tests/data/power_flow/pandapower/networks/asymmetric/distribution-case/asym_output_batch.json
--rw-r--r--   0 runner    (1001) docker     (123)      148 2023-06-26 12:57:01.000000 power-grid-model-1.5.0rc9190015282548/tests/data/power_flow/pandapower/networks/asymmetric/distribution-case/asym_output_batch.json.license
--rw-r--r--   0 runner    (1001) docker     (123)     8935 2023-06-26 12:57:01.000000 power-grid-model-1.5.0rc9190015282548/tests/data/power_flow/pandapower/networks/asymmetric/distribution-case/input.json
--rw-r--r--   0 runner    (1001) docker     (123)      148 2023-06-26 12:57:01.000000 power-grid-model-1.5.0rc9190015282548/tests/data/power_flow/pandapower/networks/asymmetric/distribution-case/input.json.license
--rw-r--r--   0 runner    (1001) docker     (123)      101 2023-06-26 12:57:01.000000 power-grid-model-1.5.0rc9190015282548/tests/data/power_flow/pandapower/networks/asymmetric/distribution-case/params.json
--rw-r--r--   0 runner    (1001) docker     (123)      148 2023-06-26 12:57:01.000000 power-grid-model-1.5.0rc9190015282548/tests/data/power_flow/pandapower/networks/asymmetric/distribution-case/params.json.license
--rw-r--r--   0 runner    (1001) docker     (123)     6642 2023-06-26 12:57:01.000000 power-grid-model-1.5.0rc9190015282548/tests/data/power_flow/pandapower/networks/asymmetric/distribution-case/update_batch.json
--rw-r--r--   0 runner    (1001) docker     (123)      148 2023-06-26 12:57:01.000000 power-grid-model-1.5.0rc9190015282548/tests/data/power_flow/pandapower/networks/asymmetric/distribution-case/update_batch.json.license
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 12:57:57.951413 power-grid-model-1.5.0rc9190015282548/tests/data/power_flow/pandapower/networks/asymmetric/transmission-case/
--rw-r--r--   0 runner    (1001) docker     (123)     1068 2023-06-26 12:57:01.000000 power-grid-model-1.5.0rc9190015282548/tests/data/power_flow/pandapower/networks/asymmetric/transmission-case/README.md
--rw-r--r--   0 runner    (1001) docker     (123)    10605 2023-06-26 12:57:01.000000 power-grid-model-1.5.0rc9190015282548/tests/data/power_flow/pandapower/networks/asymmetric/transmission-case/asym_output.json
--rw-r--r--   0 runner    (1001) docker     (123)      148 2023-06-26 12:57:01.000000 power-grid-model-1.5.0rc9190015282548/tests/data/power_flow/pandapower/networks/asymmetric/transmission-case/asym_output.json.license
--rw-r--r--   0 runner    (1001) docker     (123)     6208 2023-06-26 12:57:01.000000 power-grid-model-1.5.0rc9190015282548/tests/data/power_flow/pandapower/networks/asymmetric/transmission-case/input.json
--rw-r--r--   0 runner    (1001) docker     (123)      148 2023-06-26 12:57:01.000000 power-grid-model-1.5.0rc9190015282548/tests/data/power_flow/pandapower/networks/asymmetric/transmission-case/input.json.license
--rw-r--r--   0 runner    (1001) docker     (123)       78 2023-06-26 12:57:01.000000 power-grid-model-1.5.0rc9190015282548/tests/data/power_flow/pandapower/networks/asymmetric/transmission-case/params.json
--rw-r--r--   0 runner    (1001) docker     (123)      148 2023-06-26 12:57:01.000000 power-grid-model-1.5.0rc9190015282548/tests/data/power_flow/pandapower/networks/asymmetric/transmission-case/params.json.license
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 12:57:57.891410 power-grid-model-1.5.0rc9190015282548/tests/data/power_flow/pandapower/networks/symmetric/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 12:57:57.955414 power-grid-model-1.5.0rc9190015282548/tests/data/power_flow/pandapower/networks/symmetric/distribution-case/
--rw-r--r--   0 runner    (1001) docker     (123)     1365 2023-06-26 12:57:01.000000 power-grid-model-1.5.0rc9190015282548/tests/data/power_flow/pandapower/networks/symmetric/distribution-case/README.md
--rw-r--r--   0 runner    (1001) docker     (123)     8939 2023-06-26 12:57:01.000000 power-grid-model-1.5.0rc9190015282548/tests/data/power_flow/pandapower/networks/symmetric/distribution-case/input.json
--rw-r--r--   0 runner    (1001) docker     (123)      148 2023-06-26 12:57:01.000000 power-grid-model-1.5.0rc9190015282548/tests/data/power_flow/pandapower/networks/symmetric/distribution-case/input.json.license
--rw-r--r--   0 runner    (1001) docker     (123)      101 2023-06-26 12:57:01.000000 power-grid-model-1.5.0rc9190015282548/tests/data/power_flow/pandapower/networks/symmetric/distribution-case/params.json
--rw-r--r--   0 runner    (1001) docker     (123)      148 2023-06-26 12:57:01.000000 power-grid-model-1.5.0rc9190015282548/tests/data/power_flow/pandapower/networks/symmetric/distribution-case/params.json.license
--rw-r--r--   0 runner    (1001) docker     (123)     8702 2023-06-26 12:57:01.000000 power-grid-model-1.5.0rc9190015282548/tests/data/power_flow/pandapower/networks/symmetric/distribution-case/sym_output_batch.json
--rw-r--r--   0 runner    (1001) docker     (123)      148 2023-06-26 12:57:01.000000 power-grid-model-1.5.0rc9190015282548/tests/data/power_flow/pandapower/networks/symmetric/distribution-case/sym_output_batch.json.license
--rw-r--r--   0 runner    (1001) docker     (123)     6642 2023-06-26 12:57:01.000000 power-grid-model-1.5.0rc9190015282548/tests/data/power_flow/pandapower/networks/symmetric/distribution-case/update_batch.json
--rw-r--r--   0 runner    (1001) docker     (123)      148 2023-06-26 12:57:01.000000 power-grid-model-1.5.0rc9190015282548/tests/data/power_flow/pandapower/networks/symmetric/distribution-case/update_batch.json.license
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 12:57:57.955414 power-grid-model-1.5.0rc9190015282548/tests/data/power_flow/pandapower/networks/symmetric/transmission-case/
--rw-r--r--   0 runner    (1001) docker     (123)     1068 2023-06-26 12:57:01.000000 power-grid-model-1.5.0rc9190015282548/tests/data/power_flow/pandapower/networks/symmetric/transmission-case/README.md
--rw-r--r--   0 runner    (1001) docker     (123)     6216 2023-06-26 12:57:01.000000 power-grid-model-1.5.0rc9190015282548/tests/data/power_flow/pandapower/networks/symmetric/transmission-case/input.json
--rw-r--r--   0 runner    (1001) docker     (123)      148 2023-06-26 12:57:01.000000 power-grid-model-1.5.0rc9190015282548/tests/data/power_flow/pandapower/networks/symmetric/transmission-case/input.json.license
--rw-r--r--   0 runner    (1001) docker     (123)       78 2023-06-26 12:57:01.000000 power-grid-model-1.5.0rc9190015282548/tests/data/power_flow/pandapower/networks/symmetric/transmission-case/params.json
--rw-r--r--   0 runner    (1001) docker     (123)      148 2023-06-26 12:57:01.000000 power-grid-model-1.5.0rc9190015282548/tests/data/power_flow/pandapower/networks/symmetric/transmission-case/params.json.license
--rw-r--r--   0 runner    (1001) docker     (123)     5384 2023-06-26 12:57:01.000000 power-grid-model-1.5.0rc9190015282548/tests/data/power_flow/pandapower/networks/symmetric/transmission-case/sym_output.json
--rw-r--r--   0 runner    (1001) docker     (123)      148 2023-06-26 12:57:01.000000 power-grid-model-1.5.0rc9190015282548/tests/data/power_flow/pandapower/networks/symmetric/transmission-case/sym_output.json.license
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 12:57:57.955414 power-grid-model-1.5.0rc9190015282548/tests/data/power_flow/r-state-estimation/
--rw-r--r--   0 runner    (1001) docker     (123)     1492 2023-06-26 12:57:01.000000 power-grid-model-1.5.0rc9190015282548/tests/data/power_flow/r-state-estimation/input.json
--rw-r--r--   0 runner    (1001) docker     (123)      148 2023-06-26 12:57:01.000000 power-grid-model-1.5.0rc9190015282548/tests/data/power_flow/r-state-estimation/input.json.license
--rw-r--r--   0 runner    (1001) docker     (123)       68 2023-06-26 12:57:01.000000 power-grid-model-1.5.0rc9190015282548/tests/data/power_flow/r-state-estimation/params.json
--rw-r--r--   0 runner    (1001) docker     (123)      148 2023-06-26 12:57:01.000000 power-grid-model-1.5.0rc9190015282548/tests/data/power_flow/r-state-estimation/params.json.license
--rw-r--r--   0 runner    (1001) docker     (123)      575 2023-06-26 12:57:01.000000 power-grid-model-1.5.0rc9190015282548/tests/data/power_flow/r-state-estimation/sym_output.json
--rw-r--r--   0 runner    (1001) docker     (123)      148 2023-06-26 12:57:01.000000 power-grid-model-1.5.0rc9190015282548/tests/data/power_flow/r-state-estimation/sym_output.json.license
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 12:57:57.959414 power-grid-model-1.5.0rc9190015282548/tests/data/power_flow/three-winding-transformer/
--rw-r--r--   0 runner    (1001) docker     (123)    21196 2023-06-26 12:57:01.000000 power-grid-model-1.5.0rc9190015282548/tests/data/power_flow/three-winding-transformer/asym_output_batch.json
--rw-r--r--   0 runner    (1001) docker     (123)      148 2023-06-26 12:57:01.000000 power-grid-model-1.5.0rc9190015282548/tests/data/power_flow/three-winding-transformer/asym_output_batch.json.license
--rw-r--r--   0 runner    (1001) docker     (123)     1089 2023-06-26 12:57:01.000000 power-grid-model-1.5.0rc9190015282548/tests/data/power_flow/three-winding-transformer/input.json
--rw-r--r--   0 runner    (1001) docker     (123)      148 2023-06-26 12:57:01.000000 power-grid-model-1.5.0rc9190015282548/tests/data/power_flow/three-winding-transformer/input.json.license
--rw-r--r--   0 runner    (1001) docker     (123)      101 2023-06-26 12:57:01.000000 power-grid-model-1.5.0rc9190015282548/tests/data/power_flow/three-winding-transformer/params.json
--rw-r--r--   0 runner    (1001) docker     (123)      148 2023-06-26 12:57:01.000000 power-grid-model-1.5.0rc9190015282548/tests/data/power_flow/three-winding-transformer/params.json.license
--rw-r--r--   0 runner    (1001) docker     (123)     7374 2023-06-26 12:57:01.000000 power-grid-model-1.5.0rc9190015282548/tests/data/power_flow/three-winding-transformer/sym_output_batch.json
--rw-r--r--   0 runner    (1001) docker     (123)      148 2023-06-26 12:57:01.000000 power-grid-model-1.5.0rc9190015282548/tests/data/power_flow/three-winding-transformer/sym_output_batch.json.license
--rw-r--r--   0 runner    (1001) docker     (123)     1737 2023-06-26 12:57:01.000000 power-grid-model-1.5.0rc9190015282548/tests/data/power_flow/three-winding-transformer/update_batch.json
--rw-r--r--   0 runner    (1001) docker     (123)      148 2023-06-26 12:57:01.000000 power-grid-model-1.5.0rc9190015282548/tests/data/power_flow/three-winding-transformer/update_batch.json.license
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 12:57:57.959414 power-grid-model-1.5.0rc9190015282548/tests/data/power_flow/vision-example/
--rw-r--r--   0 runner    (1001) docker     (123)      623 2023-06-26 12:57:01.000000 power-grid-model-1.5.0rc9190015282548/tests/data/power_flow/vision-example/asym_output.json
--rw-r--r--   0 runner    (1001) docker     (123)      148 2023-06-26 12:57:01.000000 power-grid-model-1.5.0rc9190015282548/tests/data/power_flow/vision-example/asym_output.json.license
--rw-r--r--   0 runner    (1001) docker     (123)     1575 2023-06-26 12:57:01.000000 power-grid-model-1.5.0rc9190015282548/tests/data/power_flow/vision-example/input.json
--rw-r--r--   0 runner    (1001) docker     (123)      148 2023-06-26 12:57:01.000000 power-grid-model-1.5.0rc9190015282548/tests/data/power_flow/vision-example/input.json.license
--rw-r--r--   0 runner    (1001) docker     (123)       74 2023-06-26 12:57:01.000000 power-grid-model-1.5.0rc9190015282548/tests/data/power_flow/vision-example/params.json
--rw-r--r--   0 runner    (1001) docker     (123)      148 2023-06-26 12:57:01.000000 power-grid-model-1.5.0rc9190015282548/tests/data/power_flow/vision-example/params.json.license
--rw-r--r--   0 runner    (1001) docker     (123)     2450 2023-06-26 12:57:01.000000 power-grid-model-1.5.0rc9190015282548/tests/data/power_flow/vision-example/vision_grid.vnf
--rw-r--r--   0 runner    (1001) docker     (123)      148 2023-06-26 12:57:01.000000 power-grid-model-1.5.0rc9190015282548/tests/data/power_flow/vision-example/vision_grid.vnf.license
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 12:57:57.959414 power-grid-model-1.5.0rc9190015282548/tests/data/power_flow/vision-validation-network/
--rw-r--r--   0 runner    (1001) docker     (123)    20486 2023-06-26 12:57:01.000000 power-grid-model-1.5.0rc9190015282548/tests/data/power_flow/vision-validation-network/asym_output.json
--rw-r--r--   0 runner    (1001) docker     (123)      148 2023-06-26 12:57:01.000000 power-grid-model-1.5.0rc9190015282548/tests/data/power_flow/vision-validation-network/asym_output.json.license
--rw-r--r--   0 runner    (1001) docker     (123)    30756 2023-06-26 12:57:01.000000 power-grid-model-1.5.0rc9190015282548/tests/data/power_flow/vision-validation-network/input.json
--rw-r--r--   0 runner    (1001) docker     (123)      148 2023-06-26 12:57:01.000000 power-grid-model-1.5.0rc9190015282548/tests/data/power_flow/vision-validation-network/input.json.license
--rw-r--r--   0 runner    (1001) docker     (123)      363 2023-06-26 12:57:01.000000 power-grid-model-1.5.0rc9190015282548/tests/data/power_flow/vision-validation-network/params.json
--rw-r--r--   0 runner    (1001) docker     (123)      148 2023-06-26 12:57:01.000000 power-grid-model-1.5.0rc9190015282548/tests/data/power_flow/vision-validation-network/params.json.license
--rw-r--r--   0 runner    (1001) docker     (123)    11853 2023-06-26 12:57:01.000000 power-grid-model-1.5.0rc9190015282548/tests/data/power_flow/vision-validation-network/sym_output.json
--rw-r--r--   0 runner    (1001) docker     (123)      148 2023-06-26 12:57:01.000000 power-grid-model-1.5.0rc9190015282548/tests/data/power_flow/vision-validation-network/sym_output.json.license
--rw-r--r--   0 runner    (1001) docker     (123)    35119 2023-06-26 12:57:01.000000 power-grid-model-1.5.0rc9190015282548/tests/data/power_flow/vision-validation-network/vision_validation_network.vnf
--rw-r--r--   0 runner    (1001) docker     (123)      148 2023-06-26 12:57:01.000000 power-grid-model-1.5.0rc9190015282548/tests/data/power_flow/vision-validation-network/vision_validation_network.vnf.license
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 12:57:57.891410 power-grid-model-1.5.0rc9190015282548/tests/data/short_circuit/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 12:57:57.963414 power-grid-model-1.5.0rc9190015282548/tests/data/short_circuit/single_phase_to_ground_a/
--rw-r--r--   0 runner    (1001) docker     (123)    60746 2023-06-26 12:57:01.000000 power-grid-model-1.5.0rc9190015282548/tests/data/short_circuit/single_phase_to_ground_a/asym_sc_output_batch.json
--rw-r--r--   0 runner    (1001) docker     (123)      148 2023-06-26 12:57:01.000000 power-grid-model-1.5.0rc9190015282548/tests/data/short_circuit/single_phase_to_ground_a/asym_sc_output_batch.json.license
--rw-r--r--   0 runner    (1001) docker     (123)     1248 2023-06-26 12:57:01.000000 power-grid-model-1.5.0rc9190015282548/tests/data/short_circuit/single_phase_to_ground_a/input.json
--rw-r--r--   0 runner    (1001) docker     (123)      148 2023-06-26 12:57:01.000000 power-grid-model-1.5.0rc9190015282548/tests/data/short_circuit/single_phase_to_ground_a/input.json.license
--rw-r--r--   0 runner    (1001) docker     (123)      141 2023-06-26 12:57:01.000000 power-grid-model-1.5.0rc9190015282548/tests/data/short_circuit/single_phase_to_ground_a/params.json
--rw-r--r--   0 runner    (1001) docker     (123)      148 2023-06-26 12:57:01.000000 power-grid-model-1.5.0rc9190015282548/tests/data/short_circuit/single_phase_to_ground_a/params.json.license
--rw-r--r--   0 runner    (1001) docker     (123)     5042 2023-06-26 12:57:01.000000 power-grid-model-1.5.0rc9190015282548/tests/data/short_circuit/single_phase_to_ground_a/update_batch.json
--rw-r--r--   0 runner    (1001) docker     (123)      148 2023-06-26 12:57:01.000000 power-grid-model-1.5.0rc9190015282548/tests/data/short_circuit/single_phase_to_ground_a/update_batch.json.license
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 12:57:57.963414 power-grid-model-1.5.0rc9190015282548/tests/data/short_circuit/single_phase_to_ground_b/
--rw-r--r--   0 runner    (1001) docker     (123)    60938 2023-06-26 12:57:01.000000 power-grid-model-1.5.0rc9190015282548/tests/data/short_circuit/single_phase_to_ground_b/asym_sc_output_batch.json
--rw-r--r--   0 runner    (1001) docker     (123)      148 2023-06-26 12:57:01.000000 power-grid-model-1.5.0rc9190015282548/tests/data/short_circuit/single_phase_to_ground_b/asym_sc_output_batch.json.license
--rw-r--r--   0 runner    (1001) docker     (123)     1248 2023-06-26 12:57:01.000000 power-grid-model-1.5.0rc9190015282548/tests/data/short_circuit/single_phase_to_ground_b/input.json
--rw-r--r--   0 runner    (1001) docker     (123)      148 2023-06-26 12:57:01.000000 power-grid-model-1.5.0rc9190015282548/tests/data/short_circuit/single_phase_to_ground_b/input.json.license
--rw-r--r--   0 runner    (1001) docker     (123)      141 2023-06-26 12:57:01.000000 power-grid-model-1.5.0rc9190015282548/tests/data/short_circuit/single_phase_to_ground_b/params.json
--rw-r--r--   0 runner    (1001) docker     (123)      148 2023-06-26 12:57:01.000000 power-grid-model-1.5.0rc9190015282548/tests/data/short_circuit/single_phase_to_ground_b/params.json.license
--rw-r--r--   0 runner    (1001) docker     (123)     5042 2023-06-26 12:57:01.000000 power-grid-model-1.5.0rc9190015282548/tests/data/short_circuit/single_phase_to_ground_b/update_batch.json
--rw-r--r--   0 runner    (1001) docker     (123)      148 2023-06-26 12:57:01.000000 power-grid-model-1.5.0rc9190015282548/tests/data/short_circuit/single_phase_to_ground_b/update_batch.json.license
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 12:57:57.963414 power-grid-model-1.5.0rc9190015282548/tests/data/short_circuit/single_phase_to_ground_c/
--rw-r--r--   0 runner    (1001) docker     (123)    60902 2023-06-26 12:57:01.000000 power-grid-model-1.5.0rc9190015282548/tests/data/short_circuit/single_phase_to_ground_c/asym_sc_output_batch.json
--rw-r--r--   0 runner    (1001) docker     (123)      148 2023-06-26 12:57:01.000000 power-grid-model-1.5.0rc9190015282548/tests/data/short_circuit/single_phase_to_ground_c/asym_sc_output_batch.json.license
--rw-r--r--   0 runner    (1001) docker     (123)     1248 2023-06-26 12:57:01.000000 power-grid-model-1.5.0rc9190015282548/tests/data/short_circuit/single_phase_to_ground_c/input.json
--rw-r--r--   0 runner    (1001) docker     (123)      148 2023-06-26 12:57:01.000000 power-grid-model-1.5.0rc9190015282548/tests/data/short_circuit/single_phase_to_ground_c/input.json.license
--rw-r--r--   0 runner    (1001) docker     (123)      141 2023-06-26 12:57:01.000000 power-grid-model-1.5.0rc9190015282548/tests/data/short_circuit/single_phase_to_ground_c/params.json
--rw-r--r--   0 runner    (1001) docker     (123)      148 2023-06-26 12:57:01.000000 power-grid-model-1.5.0rc9190015282548/tests/data/short_circuit/single_phase_to_ground_c/params.json.license
--rw-r--r--   0 runner    (1001) docker     (123)     5042 2023-06-26 12:57:01.000000 power-grid-model-1.5.0rc9190015282548/tests/data/short_circuit/single_phase_to_ground_c/update_batch.json
--rw-r--r--   0 runner    (1001) docker     (123)      148 2023-06-26 12:57:01.000000 power-grid-model-1.5.0rc9190015282548/tests/data/short_circuit/single_phase_to_ground_c/update_batch.json.license
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 12:57:57.967414 power-grid-model-1.5.0rc9190015282548/tests/data/short_circuit/three_phase/
--rw-r--r--   0 runner    (1001) docker     (123)     1248 2023-06-26 12:57:01.000000 power-grid-model-1.5.0rc9190015282548/tests/data/short_circuit/three_phase/input.json
--rw-r--r--   0 runner    (1001) docker     (123)      148 2023-06-26 12:57:01.000000 power-grid-model-1.5.0rc9190015282548/tests/data/short_circuit/three_phase/input.json.license
--rw-r--r--   0 runner    (1001) docker     (123)      132 2023-06-26 12:57:01.000000 power-grid-model-1.5.0rc9190015282548/tests/data/short_circuit/three_phase/params.json
--rw-r--r--   0 runner    (1001) docker     (123)      148 2023-06-26 12:57:01.000000 power-grid-model-1.5.0rc9190015282548/tests/data/short_circuit/three_phase/params.json.license
--rw-r--r--   0 runner    (1001) docker     (123)    28484 2023-06-26 12:57:01.000000 power-grid-model-1.5.0rc9190015282548/tests/data/short_circuit/three_phase/sym_sc_output_batch.json
--rw-r--r--   0 runner    (1001) docker     (123)      148 2023-06-26 12:57:01.000000 power-grid-model-1.5.0rc9190015282548/tests/data/short_circuit/three_phase/sym_sc_output_batch.json.license
--rw-r--r--   0 runner    (1001) docker     (123)     5042 2023-06-26 12:57:01.000000 power-grid-model-1.5.0rc9190015282548/tests/data/short_circuit/three_phase/update_batch.json
--rw-r--r--   0 runner    (1001) docker     (123)      148 2023-06-26 12:57:01.000000 power-grid-model-1.5.0rc9190015282548/tests/data/short_circuit/three_phase/update_batch.json.license
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 12:57:57.967414 power-grid-model-1.5.0rc9190015282548/tests/data/short_circuit/two_phase_ab/
--rw-r--r--   0 runner    (1001) docker     (123)    59648 2023-06-26 12:57:01.000000 power-grid-model-1.5.0rc9190015282548/tests/data/short_circuit/two_phase_ab/asym_sc_output_batch.json
--rw-r--r--   0 runner    (1001) docker     (123)      148 2023-06-26 12:57:01.000000 power-grid-model-1.5.0rc9190015282548/tests/data/short_circuit/two_phase_ab/asym_sc_output_batch.json.license
--rw-r--r--   0 runner    (1001) docker     (123)     1248 2023-06-26 12:57:01.000000 power-grid-model-1.5.0rc9190015282548/tests/data/short_circuit/two_phase_ab/input.json
--rw-r--r--   0 runner    (1001) docker     (123)      148 2023-06-26 12:57:01.000000 power-grid-model-1.5.0rc9190015282548/tests/data/short_circuit/two_phase_ab/input.json.license
--rw-r--r--   0 runner    (1001) docker     (123)      129 2023-06-26 12:57:01.000000 power-grid-model-1.5.0rc9190015282548/tests/data/short_circuit/two_phase_ab/params.json
--rw-r--r--   0 runner    (1001) docker     (123)      148 2023-06-26 12:57:01.000000 power-grid-model-1.5.0rc9190015282548/tests/data/short_circuit/two_phase_ab/params.json.license
--rw-r--r--   0 runner    (1001) docker     (123)     5042 2023-06-26 12:57:01.000000 power-grid-model-1.5.0rc9190015282548/tests/data/short_circuit/two_phase_ab/update_batch.json
--rw-r--r--   0 runner    (1001) docker     (123)      148 2023-06-26 12:57:01.000000 power-grid-model-1.5.0rc9190015282548/tests/data/short_circuit/two_phase_ab/update_batch.json.license
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 12:57:57.967414 power-grid-model-1.5.0rc9190015282548/tests/data/short_circuit/two_phase_ac/
--rw-r--r--   0 runner    (1001) docker     (123)    58856 2023-06-26 12:57:01.000000 power-grid-model-1.5.0rc9190015282548/tests/data/short_circuit/two_phase_ac/asym_sc_output_batch.json
--rw-r--r--   0 runner    (1001) docker     (123)      148 2023-06-26 12:57:01.000000 power-grid-model-1.5.0rc9190015282548/tests/data/short_circuit/two_phase_ac/asym_sc_output_batch.json.license
--rw-r--r--   0 runner    (1001) docker     (123)     1248 2023-06-26 12:57:01.000000 power-grid-model-1.5.0rc9190015282548/tests/data/short_circuit/two_phase_ac/input.json
--rw-r--r--   0 runner    (1001) docker     (123)      148 2023-06-26 12:57:01.000000 power-grid-model-1.5.0rc9190015282548/tests/data/short_circuit/two_phase_ac/input.json.license
--rw-r--r--   0 runner    (1001) docker     (123)      129 2023-06-26 12:57:01.000000 power-grid-model-1.5.0rc9190015282548/tests/data/short_circuit/two_phase_ac/params.json
--rw-r--r--   0 runner    (1001) docker     (123)      148 2023-06-26 12:57:01.000000 power-grid-model-1.5.0rc9190015282548/tests/data/short_circuit/two_phase_ac/params.json.license
--rw-r--r--   0 runner    (1001) docker     (123)     5042 2023-06-26 12:57:01.000000 power-grid-model-1.5.0rc9190015282548/tests/data/short_circuit/two_phase_ac/update_batch.json
--rw-r--r--   0 runner    (1001) docker     (123)      148 2023-06-26 12:57:01.000000 power-grid-model-1.5.0rc9190015282548/tests/data/short_circuit/two_phase_ac/update_batch.json.license
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 12:57:57.971415 power-grid-model-1.5.0rc9190015282548/tests/data/short_circuit/two_phase_bc/
--rw-r--r--   0 runner    (1001) docker     (123)    58682 2023-06-26 12:57:01.000000 power-grid-model-1.5.0rc9190015282548/tests/data/short_circuit/two_phase_bc/asym_sc_output_batch.json
--rw-r--r--   0 runner    (1001) docker     (123)      148 2023-06-26 12:57:01.000000 power-grid-model-1.5.0rc9190015282548/tests/data/short_circuit/two_phase_bc/asym_sc_output_batch.json.license
--rw-r--r--   0 runner    (1001) docker     (123)     1248 2023-06-26 12:57:01.000000 power-grid-model-1.5.0rc9190015282548/tests/data/short_circuit/two_phase_bc/input.json
--rw-r--r--   0 runner    (1001) docker     (123)      148 2023-06-26 12:57:01.000000 power-grid-model-1.5.0rc9190015282548/tests/data/short_circuit/two_phase_bc/input.json.license
--rw-r--r--   0 runner    (1001) docker     (123)      129 2023-06-26 12:57:01.000000 power-grid-model-1.5.0rc9190015282548/tests/data/short_circuit/two_phase_bc/params.json
--rw-r--r--   0 runner    (1001) docker     (123)      148 2023-06-26 12:57:01.000000 power-grid-model-1.5.0rc9190015282548/tests/data/short_circuit/two_phase_bc/params.json.license
--rw-r--r--   0 runner    (1001) docker     (123)     5042 2023-06-26 12:57:01.000000 power-grid-model-1.5.0rc9190015282548/tests/data/short_circuit/two_phase_bc/update_batch.json
--rw-r--r--   0 runner    (1001) docker     (123)      148 2023-06-26 12:57:01.000000 power-grid-model-1.5.0rc9190015282548/tests/data/short_circuit/two_phase_bc/update_batch.json.license
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 12:57:57.971415 power-grid-model-1.5.0rc9190015282548/tests/data/short_circuit/two_phase_to_ground_ab/
--rw-r--r--   0 runner    (1001) docker     (123)    60884 2023-06-26 12:57:01.000000 power-grid-model-1.5.0rc9190015282548/tests/data/short_circuit/two_phase_to_ground_ab/asym_sc_output_batch.json
--rw-r--r--   0 runner    (1001) docker     (123)      148 2023-06-26 12:57:01.000000 power-grid-model-1.5.0rc9190015282548/tests/data/short_circuit/two_phase_to_ground_ab/asym_sc_output_batch.json.license
--rw-r--r--   0 runner    (1001) docker     (123)     1248 2023-06-26 12:57:01.000000 power-grid-model-1.5.0rc9190015282548/tests/data/short_circuit/two_phase_to_ground_ab/input.json
--rw-r--r--   0 runner    (1001) docker     (123)      148 2023-06-26 12:57:01.000000 power-grid-model-1.5.0rc9190015282548/tests/data/short_circuit/two_phase_to_ground_ab/input.json.license
--rw-r--r--   0 runner    (1001) docker     (123)      139 2023-06-26 12:57:01.000000 power-grid-model-1.5.0rc9190015282548/tests/data/short_circuit/two_phase_to_ground_ab/params.json
--rw-r--r--   0 runner    (1001) docker     (123)      148 2023-06-26 12:57:01.000000 power-grid-model-1.5.0rc9190015282548/tests/data/short_circuit/two_phase_to_ground_ab/params.json.license
--rw-r--r--   0 runner    (1001) docker     (123)     5042 2023-06-26 12:57:01.000000 power-grid-model-1.5.0rc9190015282548/tests/data/short_circuit/two_phase_to_ground_ab/update_batch.json
--rw-r--r--   0 runner    (1001) docker     (123)      148 2023-06-26 12:57:01.000000 power-grid-model-1.5.0rc9190015282548/tests/data/short_circuit/two_phase_to_ground_ab/update_batch.json.license
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 12:57:57.971415 power-grid-model-1.5.0rc9190015282548/tests/data/short_circuit/two_phase_to_ground_ac/
--rw-r--r--   0 runner    (1001) docker     (123)    60740 2023-06-26 12:57:01.000000 power-grid-model-1.5.0rc9190015282548/tests/data/short_circuit/two_phase_to_ground_ac/asym_sc_output_batch.json
--rw-r--r--   0 runner    (1001) docker     (123)      148 2023-06-26 12:57:01.000000 power-grid-model-1.5.0rc9190015282548/tests/data/short_circuit/two_phase_to_ground_ac/asym_sc_output_batch.json.license
--rw-r--r--   0 runner    (1001) docker     (123)     1248 2023-06-26 12:57:01.000000 power-grid-model-1.5.0rc9190015282548/tests/data/short_circuit/two_phase_to_ground_ac/input.json
--rw-r--r--   0 runner    (1001) docker     (123)      148 2023-06-26 12:57:01.000000 power-grid-model-1.5.0rc9190015282548/tests/data/short_circuit/two_phase_to_ground_ac/input.json.license
--rw-r--r--   0 runner    (1001) docker     (123)      139 2023-06-26 12:57:01.000000 power-grid-model-1.5.0rc9190015282548/tests/data/short_circuit/two_phase_to_ground_ac/params.json
--rw-r--r--   0 runner    (1001) docker     (123)      148 2023-06-26 12:57:01.000000 power-grid-model-1.5.0rc9190015282548/tests/data/short_circuit/two_phase_to_ground_ac/params.json.license
--rw-r--r--   0 runner    (1001) docker     (123)     5042 2023-06-26 12:57:01.000000 power-grid-model-1.5.0rc9190015282548/tests/data/short_circuit/two_phase_to_ground_ac/update_batch.json
--rw-r--r--   0 runner    (1001) docker     (123)      148 2023-06-26 12:57:01.000000 power-grid-model-1.5.0rc9190015282548/tests/data/short_circuit/two_phase_to_ground_ac/update_batch.json.license
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 12:57:57.975415 power-grid-model-1.5.0rc9190015282548/tests/data/short_circuit/two_phase_to_ground_bc/
--rw-r--r--   0 runner    (1001) docker     (123)    60629 2023-06-26 12:57:01.000000 power-grid-model-1.5.0rc9190015282548/tests/data/short_circuit/two_phase_to_ground_bc/asym_sc_output_batch.json
--rw-r--r--   0 runner    (1001) docker     (123)      148 2023-06-26 12:57:01.000000 power-grid-model-1.5.0rc9190015282548/tests/data/short_circuit/two_phase_to_ground_bc/asym_sc_output_batch.json.license
--rw-r--r--   0 runner    (1001) docker     (123)     1248 2023-06-26 12:57:01.000000 power-grid-model-1.5.0rc9190015282548/tests/data/short_circuit/two_phase_to_ground_bc/input.json
--rw-r--r--   0 runner    (1001) docker     (123)      148 2023-06-26 12:57:01.000000 power-grid-model-1.5.0rc9190015282548/tests/data/short_circuit/two_phase_to_ground_bc/input.json.license
--rw-r--r--   0 runner    (1001) docker     (123)      139 2023-06-26 12:57:01.000000 power-grid-model-1.5.0rc9190015282548/tests/data/short_circuit/two_phase_to_ground_bc/params.json
--rw-r--r--   0 runner    (1001) docker     (123)      148 2023-06-26 12:57:01.000000 power-grid-model-1.5.0rc9190015282548/tests/data/short_circuit/two_phase_to_ground_bc/params.json.license
--rw-r--r--   0 runner    (1001) docker     (123)     5042 2023-06-26 12:57:01.000000 power-grid-model-1.5.0rc9190015282548/tests/data/short_circuit/two_phase_to_ground_bc/update_batch.json
--rw-r--r--   0 runner    (1001) docker     (123)      148 2023-06-26 12:57:01.000000 power-grid-model-1.5.0rc9190015282548/tests/data/short_circuit/two_phase_to_ground_bc/update_batch.json.license
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 12:57:57.891410 power-grid-model-1.5.0rc9190015282548/tests/data/state_estimation/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 12:57:57.975415 power-grid-model-1.5.0rc9190015282548/tests/data/state_estimation/1os2msr/
--rw-r--r--   0 runner    (1001) docker     (123)     2910 2023-06-26 12:57:01.000000 power-grid-model-1.5.0rc9190015282548/tests/data/state_estimation/1os2msr/input.json
--rw-r--r--   0 runner    (1001) docker     (123)      148 2023-06-26 12:57:01.000000 power-grid-model-1.5.0rc9190015282548/tests/data/state_estimation/1os2msr/input.json.license
--rw-r--r--   0 runner    (1001) docker     (123)      124 2023-06-26 12:57:01.000000 power-grid-model-1.5.0rc9190015282548/tests/data/state_estimation/1os2msr/params.json
--rw-r--r--   0 runner    (1001) docker     (123)      148 2023-06-26 12:57:01.000000 power-grid-model-1.5.0rc9190015282548/tests/data/state_estimation/1os2msr/params.json.license
--rw-r--r--   0 runner    (1001) docker     (123)     2731 2023-06-26 12:57:01.000000 power-grid-model-1.5.0rc9190015282548/tests/data/state_estimation/1os2msr/sym_output.json
--rw-r--r--   0 runner    (1001) docker     (123)      148 2023-06-26 12:57:01.000000 power-grid-model-1.5.0rc9190015282548/tests/data/state_estimation/1os2msr/sym_output.json.license
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 12:57:57.975415 power-grid-model-1.5.0rc9190015282548/tests/data/state_estimation/1os2msr-no-angle/
--rw-r--r--   0 runner    (1001) docker     (123)     2786 2023-06-26 12:57:01.000000 power-grid-model-1.5.0rc9190015282548/tests/data/state_estimation/1os2msr-no-angle/input.json
--rw-r--r--   0 runner    (1001) docker     (123)      148 2023-06-26 12:57:01.000000 power-grid-model-1.5.0rc9190015282548/tests/data/state_estimation/1os2msr-no-angle/input.json.license
--rw-r--r--   0 runner    (1001) docker     (123)       78 2023-06-26 12:57:01.000000 power-grid-model-1.5.0rc9190015282548/tests/data/state_estimation/1os2msr-no-angle/params.json
--rw-r--r--   0 runner    (1001) docker     (123)      148 2023-06-26 12:57:01.000000 power-grid-model-1.5.0rc9190015282548/tests/data/state_estimation/1os2msr-no-angle/params.json.license
--rw-r--r--   0 runner    (1001) docker     (123)     1836 2023-06-26 12:57:01.000000 power-grid-model-1.5.0rc9190015282548/tests/data/state_estimation/1os2msr-no-angle/sym_output.json
--rw-r--r--   0 runner    (1001) docker     (123)      148 2023-06-26 12:57:01.000000 power-grid-model-1.5.0rc9190015282548/tests/data/state_estimation/1os2msr-no-angle/sym_output.json.license
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 12:57:57.975415 power-grid-model-1.5.0rc9190015282548/tests/data/state_estimation/distribution-case/
--rw-r--r--   0 runner    (1001) docker     (123)     1395 2023-06-26 12:57:01.000000 power-grid-model-1.5.0rc9190015282548/tests/data/state_estimation/distribution-case/README.md
--rw-r--r--   0 runner    (1001) docker     (123)     8939 2023-06-26 12:57:01.000000 power-grid-model-1.5.0rc9190015282548/tests/data/state_estimation/distribution-case/input.json
--rw-r--r--   0 runner    (1001) docker     (123)      148 2023-06-26 12:57:01.000000 power-grid-model-1.5.0rc9190015282548/tests/data/state_estimation/distribution-case/input.json.license
--rw-r--r--   0 runner    (1001) docker     (123)      123 2023-06-26 12:57:01.000000 power-grid-model-1.5.0rc9190015282548/tests/data/state_estimation/distribution-case/params.json
--rw-r--r--   0 runner    (1001) docker     (123)      148 2023-06-26 12:57:01.000000 power-grid-model-1.5.0rc9190015282548/tests/data/state_estimation/distribution-case/params.json.license
--rw-r--r--   0 runner    (1001) docker     (123)    19468 2023-06-26 12:57:01.000000 power-grid-model-1.5.0rc9190015282548/tests/data/state_estimation/distribution-case/sym_output_batch.json
--rw-r--r--   0 runner    (1001) docker     (123)      148 2023-06-26 12:57:01.000000 power-grid-model-1.5.0rc9190015282548/tests/data/state_estimation/distribution-case/sym_output_batch.json.license
--rw-r--r--   0 runner    (1001) docker     (123)     6642 2023-06-26 12:57:01.000000 power-grid-model-1.5.0rc9190015282548/tests/data/state_estimation/distribution-case/update_batch.json
--rw-r--r--   0 runner    (1001) docker     (123)      148 2023-06-26 12:57:01.000000 power-grid-model-1.5.0rc9190015282548/tests/data/state_estimation/distribution-case/update_batch.json.license
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 12:57:57.979415 power-grid-model-1.5.0rc9190015282548/tests/data/state_estimation/dummy-test-sym/
--rw-r--r--   0 runner    (1001) docker     (123)     3196 2023-06-26 12:57:01.000000 power-grid-model-1.5.0rc9190015282548/tests/data/state_estimation/dummy-test-sym/input.json
--rw-r--r--   0 runner    (1001) docker     (123)      148 2023-06-26 12:57:01.000000 power-grid-model-1.5.0rc9190015282548/tests/data/state_estimation/dummy-test-sym/input.json.license
--rw-r--r--   0 runner    (1001) docker     (123)      116 2023-06-26 12:57:01.000000 power-grid-model-1.5.0rc9190015282548/tests/data/state_estimation/dummy-test-sym/params.json
--rw-r--r--   0 runner    (1001) docker     (123)      148 2023-06-26 12:57:01.000000 power-grid-model-1.5.0rc9190015282548/tests/data/state_estimation/dummy-test-sym/params.json.license
--rw-r--r--   0 runner    (1001) docker     (123)     2174 2023-06-26 12:57:01.000000 power-grid-model-1.5.0rc9190015282548/tests/data/state_estimation/dummy-test-sym/sym_output.json
--rw-r--r--   0 runner    (1001) docker     (123)      148 2023-06-26 12:57:01.000000 power-grid-model-1.5.0rc9190015282548/tests/data/state_estimation/dummy-test-sym/sym_output.json.license
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 12:57:57.979415 power-grid-model-1.5.0rc9190015282548/tests/data/state_estimation/node-injection-sensor-and-zero-injection/
--rw-r--r--   0 runner    (1001) docker     (123)      780 2023-06-26 12:57:01.000000 power-grid-model-1.5.0rc9190015282548/tests/data/state_estimation/node-injection-sensor-and-zero-injection/input.json
--rw-r--r--   0 runner    (1001) docker     (123)      148 2023-06-26 12:57:01.000000 power-grid-model-1.5.0rc9190015282548/tests/data/state_estimation/node-injection-sensor-and-zero-injection/input.json.license
--rw-r--r--   0 runner    (1001) docker     (123)       78 2023-06-26 12:57:01.000000 power-grid-model-1.5.0rc9190015282548/tests/data/state_estimation/node-injection-sensor-and-zero-injection/params.json
--rw-r--r--   0 runner    (1001) docker     (123)      148 2023-06-26 12:57:01.000000 power-grid-model-1.5.0rc9190015282548/tests/data/state_estimation/node-injection-sensor-and-zero-injection/params.json.license
--rw-r--r--   0 runner    (1001) docker     (123)      824 2023-06-26 12:57:01.000000 power-grid-model-1.5.0rc9190015282548/tests/data/state_estimation/node-injection-sensor-and-zero-injection/sym_output.json
--rw-r--r--   0 runner    (1001) docker     (123)      148 2023-06-26 12:57:01.000000 power-grid-model-1.5.0rc9190015282548/tests/data/state_estimation/node-injection-sensor-and-zero-injection/sym_output.json.license
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 12:57:57.979415 power-grid-model-1.5.0rc9190015282548/tests/data/state_estimation/residual-test/
--rw-r--r--   0 runner    (1001) docker     (123)      448 2023-06-26 12:57:01.000000 power-grid-model-1.5.0rc9190015282548/tests/data/state_estimation/residual-test/input.json
--rw-r--r--   0 runner    (1001) docker     (123)      148 2023-06-26 12:57:01.000000 power-grid-model-1.5.0rc9190015282548/tests/data/state_estimation/residual-test/input.json.license
--rw-r--r--   0 runner    (1001) docker     (123)      124 2023-06-26 12:57:01.000000 power-grid-model-1.5.0rc9190015282548/tests/data/state_estimation/residual-test/params.json
--rw-r--r--   0 runner    (1001) docker     (123)      148 2023-06-26 12:57:01.000000 power-grid-model-1.5.0rc9190015282548/tests/data/state_estimation/residual-test/params.json.license
--rw-r--r--   0 runner    (1001) docker     (123)      374 2023-06-26 12:57:01.000000 power-grid-model-1.5.0rc9190015282548/tests/data/state_estimation/residual-test/sym_output.json
--rw-r--r--   0 runner    (1001) docker     (123)      148 2023-06-26 12:57:01.000000 power-grid-model-1.5.0rc9190015282548/tests/data/state_estimation/residual-test/sym_output.json.license
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 12:57:57.979415 power-grid-model-1.5.0rc9190015282548/tests/data/state_estimation/single-line-load/
--rw-r--r--   0 runner    (1001) docker     (123)     1057 2023-06-26 12:57:01.000000 power-grid-model-1.5.0rc9190015282548/tests/data/state_estimation/single-line-load/input.json
--rw-r--r--   0 runner    (1001) docker     (123)      148 2023-06-26 12:57:01.000000 power-grid-model-1.5.0rc9190015282548/tests/data/state_estimation/single-line-load/input.json.license
--rw-r--r--   0 runner    (1001) docker     (123)       78 2023-06-26 12:57:01.000000 power-grid-model-1.5.0rc9190015282548/tests/data/state_estimation/single-line-load/params.json
--rw-r--r--   0 runner    (1001) docker     (123)      148 2023-06-26 12:57:01.000000 power-grid-model-1.5.0rc9190015282548/tests/data/state_estimation/single-line-load/params.json.license
--rw-r--r--   0 runner    (1001) docker     (123)      529 2023-06-26 12:57:01.000000 power-grid-model-1.5.0rc9190015282548/tests/data/state_estimation/single-line-load/sym_output.json
--rw-r--r--   0 runner    (1001) docker     (123)      148 2023-06-26 12:57:01.000000 power-grid-model-1.5.0rc9190015282548/tests/data/state_estimation/single-line-load/sym_output.json.license
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 12:57:57.979415 power-grid-model-1.5.0rc9190015282548/tests/data/state_estimation/three_winding_transformer/
--rw-r--r--   0 runner    (1001) docker     (123)     2166 2023-06-26 12:57:01.000000 power-grid-model-1.5.0rc9190015282548/tests/data/state_estimation/three_winding_transformer/input.json
--rw-r--r--   0 runner    (1001) docker     (123)      148 2023-06-26 12:57:01.000000 power-grid-model-1.5.0rc9190015282548/tests/data/state_estimation/three_winding_transformer/input.json.license
--rw-r--r--   0 runner    (1001) docker     (123)       78 2023-06-26 12:57:01.000000 power-grid-model-1.5.0rc9190015282548/tests/data/state_estimation/three_winding_transformer/params.json
--rw-r--r--   0 runner    (1001) docker     (123)      148 2023-06-26 12:57:01.000000 power-grid-model-1.5.0rc9190015282548/tests/data/state_estimation/three_winding_transformer/params.json.license
--rw-r--r--   0 runner    (1001) docker     (123)      868 2023-06-26 12:57:01.000000 power-grid-model-1.5.0rc9190015282548/tests/data/state_estimation/three_winding_transformer/sym_output.json
--rw-r--r--   0 runner    (1001) docker     (123)      148 2023-06-26 12:57:01.000000 power-grid-model-1.5.0rc9190015282548/tests/data/state_estimation/three_winding_transformer/sym_output.json.license
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 12:57:57.983416 power-grid-model-1.5.0rc9190015282548/tests/data/state_estimation/transmission-case/
--rw-r--r--   0 runner    (1001) docker     (123)     1196 2023-06-26 12:57:01.000000 power-grid-model-1.5.0rc9190015282548/tests/data/state_estimation/transmission-case/README.md
--rw-r--r--   0 runner    (1001) docker     (123)    29158 2023-06-26 12:57:01.000000 power-grid-model-1.5.0rc9190015282548/tests/data/state_estimation/transmission-case/asym_output.json
--rw-r--r--   0 runner    (1001) docker     (123)      148 2023-06-26 12:57:01.000000 power-grid-model-1.5.0rc9190015282548/tests/data/state_estimation/transmission-case/asym_output.json.license
--rw-r--r--   0 runner    (1001) docker     (123)    11996 2023-06-26 12:57:01.000000 power-grid-model-1.5.0rc9190015282548/tests/data/state_estimation/transmission-case/input.json
--rw-r--r--   0 runner    (1001) docker     (123)      148 2023-06-26 12:57:01.000000 power-grid-model-1.5.0rc9190015282548/tests/data/state_estimation/transmission-case/input.json.license
--rw-r--r--   0 runner    (1001) docker     (123)      125 2023-06-26 12:57:01.000000 power-grid-model-1.5.0rc9190015282548/tests/data/state_estimation/transmission-case/params.json
--rw-r--r--   0 runner    (1001) docker     (123)      148 2023-06-26 12:57:01.000000 power-grid-model-1.5.0rc9190015282548/tests/data/state_estimation/transmission-case/params.json.license
--rw-r--r--   0 runner    (1001) docker     (123)     7827 2023-06-26 12:57:01.000000 power-grid-model-1.5.0rc9190015282548/tests/data/state_estimation/transmission-case/sym_output.json
--rw-r--r--   0 runner    (1001) docker     (123)      148 2023-06-26 12:57:01.000000 power-grid-model-1.5.0rc9190015282548/tests/data/state_estimation/transmission-case/sym_output.json.license
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 12:57:57.983416 power-grid-model-1.5.0rc9190015282548/tests/unit/
--rw-r--r--   0 runner    (1001) docker     (123)      154 2023-06-26 12:57:01.000000 power-grid-model-1.5.0rc9190015282548/tests/unit/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4005 2023-06-26 12:57:01.000000 power-grid-model-1.5.0rc9190015282548/tests/unit/test_0Z_model_validation.py
--rw-r--r--   0 runner    (1001) docker     (123)      794 2023-06-26 12:57:01.000000 power-grid-model-1.5.0rc9190015282548/tests/unit/test_error_handling.py
--rw-r--r--   0 runner    (1001) docker     (123)     2225 2023-06-26 12:57:01.000000 power-grid-model-1.5.0rc9190015282548/tests/unit/test_meta_data.py
--rw-r--r--   0 runner    (1001) docker     (123)     6422 2023-06-26 12:57:01.000000 power-grid-model-1.5.0rc9190015282548/tests/unit/test_power_grid_model.py
--rw-r--r--   0 runner    (1001) docker     (123)    20807 2023-06-26 12:57:01.000000 power-grid-model-1.5.0rc9190015282548/tests/unit/test_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     7996 2023-06-26 12:57:01.000000 power-grid-model-1.5.0rc9190015282548/tests/unit/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 12:57:57.983416 power-grid-model-1.5.0rc9190015282548/tests/unit/validation/
--rw-r--r--   0 runner    (1001) docker     (123)      154 2023-06-26 12:57:01.000000 power-grid-model-1.5.0rc9190015282548/tests/unit/validation/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2330 2023-06-26 12:57:01.000000 power-grid-model-1.5.0rc9190015282548/tests/unit/validation/test_assertions.py
--rw-r--r--   0 runner    (1001) docker     (123)     2886 2023-06-26 12:57:01.000000 power-grid-model-1.5.0rc9190015282548/tests/unit/validation/test_batch_validation.py
--rw-r--r--   0 runner    (1001) docker     (123)     4855 2023-06-26 12:57:01.000000 power-grid-model-1.5.0rc9190015282548/tests/unit/validation/test_errors.py
--rw-r--r--   0 runner    (1001) docker     (123)    27362 2023-06-26 12:57:01.000000 power-grid-model-1.5.0rc9190015282548/tests/unit/validation/test_input_validation.py
--rw-r--r--   0 runner    (1001) docker     (123)    14325 2023-06-26 12:57:01.000000 power-grid-model-1.5.0rc9190015282548/tests/unit/validation/test_rules.py
--rw-r--r--   0 runner    (1001) docker     (123)     6991 2023-06-26 12:57:01.000000 power-grid-model-1.5.0rc9190015282548/tests/unit/validation/test_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)    23023 2023-06-26 12:57:01.000000 power-grid-model-1.5.0rc9190015282548/tests/unit/validation/test_validation_functions.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 15:22:14.456745 power-grid-model-1.5.0rc9190704883749/
+-rw-r--r--   0 runner    (1001) docker     (123)    14907 2023-06-26 15:21:20.000000 power-grid-model-1.5.0rc9190704883749/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      354 2023-06-26 15:21:20.000000 power-grid-model-1.5.0rc9190704883749/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     8142 2023-06-26 15:22:14.456745 power-grid-model-1.5.0rc9190704883749/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)       20 2023-06-26 15:21:23.000000 power-grid-model-1.5.0rc9190704883749/PYPI_VERSION
+-rw-r--r--   0 runner    (1001) docker     (123)     6818 2023-06-26 15:21:20.000000 power-grid-model-1.5.0rc9190704883749/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)        4 2023-06-26 15:21:20.000000 power-grid-model-1.5.0rc9190704883749/VERSION
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 15:22:14.376742 power-grid-model-1.5.0rc9190704883749/power_grid_model_c/
+-rw-r--r--   0 runner    (1001) docker     (123)      231 2023-06-26 15:21:20.000000 power-grid-model-1.5.0rc9190704883749/power_grid_model_c/CMakeLists.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 15:22:14.376742 power-grid-model-1.5.0rc9190704883749/power_grid_model_c/power_grid_model/
+-rw-r--r--   0 runner    (1001) docker     (123)      573 2023-06-26 15:21:20.000000 power-grid-model-1.5.0rc9190704883749/power_grid_model_c/power_grid_model/CMakeLists.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 15:22:14.368742 power-grid-model-1.5.0rc9190704883749/power_grid_model_c/power_grid_model/include/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 15:22:14.376742 power-grid-model-1.5.0rc9190704883749/power_grid_model_c/power_grid_model/include/power_grid_model/
+-rw-r--r--   0 runner    (1001) docker     (123)     1118 2023-06-26 15:21:20.000000 power-grid-model-1.5.0rc9190704883749/power_grid_model_c/power_grid_model/include/power_grid_model/all_components.hpp
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 15:22:14.376742 power-grid-model-1.5.0rc9190704883749/power_grid_model_c/power_grid_model/include/power_grid_model/auxiliary/
+-rw-r--r--   0 runner    (1001) docker     (123)     4220 2023-06-26 15:21:20.000000 power-grid-model-1.5.0rc9190704883749/power_grid_model_c/power_grid_model/include/power_grid_model/auxiliary/dataset.hpp
+-rw-r--r--   0 runner    (1001) docker     (123)    28564 2023-06-26 15:21:20.000000 power-grid-model-1.5.0rc9190704883749/power_grid_model_c/power_grid_model/include/power_grid_model/auxiliary/input.hpp
+-rw-r--r--   0 runner    (1001) docker     (123)     9937 2023-06-26 15:21:20.000000 power-grid-model-1.5.0rc9190704883749/power_grid_model_c/power_grid_model/include/power_grid_model/auxiliary/meta_data.hpp
+-rw-r--r--   0 runner    (1001) docker     (123)     1838 2023-06-26 15:21:20.000000 power-grid-model-1.5.0rc9190704883749/power_grid_model_c/power_grid_model/include/power_grid_model/auxiliary/meta_data_gen.hpp
+-rw-r--r--   0 runner    (1001) docker     (123)    17078 2023-06-26 15:21:20.000000 power-grid-model-1.5.0rc9190704883749/power_grid_model_c/power_grid_model/include/power_grid_model/auxiliary/output.hpp
+-rw-r--r--   0 runner    (1001) docker     (123)     9396 2023-06-26 15:21:20.000000 power-grid-model-1.5.0rc9190704883749/power_grid_model_c/power_grid_model/include/power_grid_model/auxiliary/update.hpp
+-rw-r--r--   0 runner    (1001) docker     (123)     9078 2023-06-26 15:21:20.000000 power-grid-model-1.5.0rc9190704883749/power_grid_model_c/power_grid_model/include/power_grid_model/calculation_parameters.hpp
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 15:22:14.380742 power-grid-model-1.5.0rc9190704883749/power_grid_model_c/power_grid_model/include/power_grid_model/component/
+-rw-r--r--   0 runner    (1001) docker     (123)     4214 2023-06-26 15:21:20.000000 power-grid-model-1.5.0rc9190704883749/power_grid_model_c/power_grid_model/include/power_grid_model/component/appliance.hpp
+-rw-r--r--   0 runner    (1001) docker     (123)     1103 2023-06-26 15:21:20.000000 power-grid-model-1.5.0rc9190704883749/power_grid_model_c/power_grid_model/include/power_grid_model/component/base.hpp
+-rw-r--r--   0 runner    (1001) docker     (123)     8931 2023-06-26 15:21:20.000000 power-grid-model-1.5.0rc9190704883749/power_grid_model_c/power_grid_model/include/power_grid_model/component/branch.hpp
+-rw-r--r--   0 runner    (1001) docker     (123)     6780 2023-06-26 15:21:20.000000 power-grid-model-1.5.0rc9190704883749/power_grid_model_c/power_grid_model/include/power_grid_model/component/branch3.hpp
+-rw-r--r--   0 runner    (1001) docker     (123)     4445 2023-06-26 15:21:20.000000 power-grid-model-1.5.0rc9190704883749/power_grid_model_c/power_grid_model/include/power_grid_model/component/fault.hpp
+-rw-r--r--   0 runner    (1001) docker     (123)     2320 2023-06-26 15:21:20.000000 power-grid-model-1.5.0rc9190704883749/power_grid_model_c/power_grid_model/include/power_grid_model/component/line.hpp
+-rw-r--r--   0 runner    (1001) docker     (123)     1629 2023-06-26 15:21:20.000000 power-grid-model-1.5.0rc9190704883749/power_grid_model_c/power_grid_model/include/power_grid_model/component/link.hpp
+-rw-r--r--   0 runner    (1001) docker     (123)     5344 2023-06-26 15:21:20.000000 power-grid-model-1.5.0rc9190704883749/power_grid_model_c/power_grid_model/include/power_grid_model/component/load_gen.hpp
+-rw-r--r--   0 runner    (1001) docker     (123)     2693 2023-06-26 15:21:20.000000 power-grid-model-1.5.0rc9190704883749/power_grid_model_c/power_grid_model/include/power_grid_model/component/node.hpp
+-rw-r--r--   0 runner    (1001) docker     (123)     4775 2023-06-26 15:21:20.000000 power-grid-model-1.5.0rc9190704883749/power_grid_model_c/power_grid_model/include/power_grid_model/component/power_sensor.hpp
+-rw-r--r--   0 runner    (1001) docker     (123)     1678 2023-06-26 15:21:20.000000 power-grid-model-1.5.0rc9190704883749/power_grid_model_c/power_grid_model/include/power_grid_model/component/sensor.hpp
+-rw-r--r--   0 runner    (1001) docker     (123)     2873 2023-06-26 15:21:20.000000 power-grid-model-1.5.0rc9190704883749/power_grid_model_c/power_grid_model/include/power_grid_model/component/shunt.hpp
+-rw-r--r--   0 runner    (1001) docker     (123)     4396 2023-06-26 15:21:20.000000 power-grid-model-1.5.0rc9190704883749/power_grid_model_c/power_grid_model/include/power_grid_model/component/source.hpp
+-rw-r--r--   0 runner    (1001) docker     (123)    20048 2023-06-26 15:21:20.000000 power-grid-model-1.5.0rc9190704883749/power_grid_model_c/power_grid_model/include/power_grid_model/component/three_winding_transformer.hpp
+-rw-r--r--   0 runner    (1001) docker     (123)    10954 2023-06-26 15:21:20.000000 power-grid-model-1.5.0rc9190704883749/power_grid_model_c/power_grid_model/include/power_grid_model/component/transformer.hpp
+-rw-r--r--   0 runner    (1001) docker     (123)     1088 2023-06-26 15:21:20.000000 power-grid-model-1.5.0rc9190704883749/power_grid_model_c/power_grid_model/include/power_grid_model/component/transformer_utils.hpp
+-rw-r--r--   0 runner    (1001) docker     (123)     5581 2023-06-26 15:21:20.000000 power-grid-model-1.5.0rc9190704883749/power_grid_model_c/power_grid_model/include/power_grid_model/component/voltage_sensor.hpp
+-rw-r--r--   0 runner    (1001) docker     (123)    15119 2023-06-26 15:21:20.000000 power-grid-model-1.5.0rc9190704883749/power_grid_model_c/power_grid_model/include/power_grid_model/container.hpp
+-rw-r--r--   0 runner    (1001) docker     (123)     2058 2023-06-26 15:21:20.000000 power-grid-model-1.5.0rc9190704883749/power_grid_model_c/power_grid_model/include/power_grid_model/enum.hpp
+-rw-r--r--   0 runner    (1001) docker     (123)     5302 2023-06-26 15:21:20.000000 power-grid-model-1.5.0rc9190704883749/power_grid_model_c/power_grid_model/include/power_grid_model/exception.hpp
+-rw-r--r--   0 runner    (1001) docker     (123)    67158 2023-06-26 15:21:20.000000 power-grid-model-1.5.0rc9190704883749/power_grid_model_c/power_grid_model/include/power_grid_model/main_model.hpp
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 15:22:14.380742 power-grid-model-1.5.0rc9190704883749/power_grid_model_c/power_grid_model/include/power_grid_model/math_solver/
+-rw-r--r--   0 runner    (1001) docker     (123)     2436 2023-06-26 15:21:20.000000 power-grid-model-1.5.0rc9190704883749/power_grid_model_c/power_grid_model/include/power_grid_model/math_solver/block_matrix.hpp
+-rw-r--r--   0 runner    (1001) docker     (123)     8954 2023-06-26 15:21:20.000000 power-grid-model-1.5.0rc9190704883749/power_grid_model_c/power_grid_model/include/power_grid_model/math_solver/iterative_current_pf_solver.hpp
+-rw-r--r--   0 runner    (1001) docker     (123)    41694 2023-06-26 15:21:20.000000 power-grid-model-1.5.0rc9190704883749/power_grid_model_c/power_grid_model/include/power_grid_model/math_solver/iterative_linear_se_solver.hpp
+-rw-r--r--   0 runner    (1001) docker     (123)     7164 2023-06-26 15:21:20.000000 power-grid-model-1.5.0rc9190704883749/power_grid_model_c/power_grid_model/include/power_grid_model/math_solver/iterative_pf_solver.hpp
+-rw-r--r--   0 runner    (1001) docker     (123)     6446 2023-06-26 15:21:20.000000 power-grid-model-1.5.0rc9190704883749/power_grid_model_c/power_grid_model/include/power_grid_model/math_solver/linear_pf_solver.hpp
+-rw-r--r--   0 runner    (1001) docker     (123)     6192 2023-06-26 15:21:20.000000 power-grid-model-1.5.0rc9190704883749/power_grid_model_c/power_grid_model/include/power_grid_model/math_solver/math_solver.hpp
+-rw-r--r--   0 runner    (1001) docker     (123)    16064 2023-06-26 15:21:20.000000 power-grid-model-1.5.0rc9190704883749/power_grid_model_c/power_grid_model/include/power_grid_model/math_solver/newton_raphson_pf_solver.hpp
+-rw-r--r--   0 runner    (1001) docker     (123)    16203 2023-06-26 15:21:20.000000 power-grid-model-1.5.0rc9190704883749/power_grid_model_c/power_grid_model/include/power_grid_model/math_solver/sparse_lu_solver.hpp
+-rw-r--r--   0 runner    (1001) docker     (123)    20148 2023-06-26 15:21:20.000000 power-grid-model-1.5.0rc9190704883749/power_grid_model_c/power_grid_model/include/power_grid_model/math_solver/y_bus.hpp
+-rw-r--r--   0 runner    (1001) docker     (123)     3055 2023-06-26 15:21:20.000000 power-grid-model-1.5.0rc9190704883749/power_grid_model_c/power_grid_model/include/power_grid_model/power_grid_model.hpp
+-rw-r--r--   0 runner    (1001) docker     (123)     2753 2023-06-26 15:21:20.000000 power-grid-model-1.5.0rc9190704883749/power_grid_model_c/power_grid_model/include/power_grid_model/sparse_mapping.hpp
+-rw-r--r--   0 runner    (1001) docker     (123)    11399 2023-06-26 15:21:20.000000 power-grid-model-1.5.0rc9190704883749/power_grid_model_c/power_grid_model/include/power_grid_model/three_phase_tensor.hpp
+-rw-r--r--   0 runner    (1001) docker     (123)     1960 2023-06-26 15:21:20.000000 power-grid-model-1.5.0rc9190704883749/power_grid_model_c/power_grid_model/include/power_grid_model/timer.hpp
+-rw-r--r--   0 runner    (1001) docker     (123)    30797 2023-06-26 15:21:20.000000 power-grid-model-1.5.0rc9190704883749/power_grid_model_c/power_grid_model/include/power_grid_model/topology.hpp
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 15:22:14.380742 power-grid-model-1.5.0rc9190704883749/power_grid_model_c/power_grid_model_c/
+-rw-r--r--   0 runner    (1001) docker     (123)      729 2023-06-26 15:21:20.000000 power-grid-model-1.5.0rc9190704883749/power_grid_model_c/power_grid_model_c/CMakeLists.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 15:22:14.384742 power-grid-model-1.5.0rc9190704883749/power_grid_model_c/power_grid_model_c/include/
+-rw-r--r--   0 runner    (1001) docker     (123)    26085 2023-06-26 15:21:20.000000 power-grid-model-1.5.0rc9190704883749/power_grid_model_c/power_grid_model_c/include/power_grid_model_c.h
+-rw-r--r--   0 runner    (1001) docker     (123)    15382 2023-06-26 15:21:20.000000 power-grid-model-1.5.0rc9190704883749/power_grid_model_c/power_grid_model_c/power_grid_model_c.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     3634 2023-06-26 15:21:20.000000 power-grid-model-1.5.0rc9190704883749/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-26 15:22:14.456745 power-grid-model-1.5.0rc9190704883749/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     7078 2023-06-26 15:21:20.000000 power-grid-model-1.5.0rc9190704883749/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 15:22:14.368742 power-grid-model-1.5.0rc9190704883749/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 15:22:14.384742 power-grid-model-1.5.0rc9190704883749/src/power_grid_model/
+-rw-r--r--   0 runner    (1001) docker     (123)      509 2023-06-26 15:21:20.000000 power-grid-model-1.5.0rc9190704883749/src/power_grid_model/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 15:22:14.384742 power-grid-model-1.5.0rc9190704883749/src/power_grid_model/core/
+-rw-r--r--   0 runner    (1001) docker     (123)      154 2023-06-26 15:21:20.000000 power-grid-model-1.5.0rc9190704883749/src/power_grid_model/core/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2100 2023-06-26 15:21:20.000000 power-grid-model-1.5.0rc9190704883749/src/power_grid_model/core/error_handling.py
+-rw-r--r--   0 runner    (1001) docker     (123)      367 2023-06-26 15:21:20.000000 power-grid-model-1.5.0rc9190704883749/src/power_grid_model/core/index_integer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1682 2023-06-26 15:21:20.000000 power-grid-model-1.5.0rc9190704883749/src/power_grid_model/core/options.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9994 2023-06-26 15:21:20.000000 power-grid-model-1.5.0rc9190704883749/src/power_grid_model/core/power_grid_core.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9240 2023-06-26 15:21:20.000000 power-grid-model-1.5.0rc9190704883749/src/power_grid_model/core/power_grid_meta.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17761 2023-06-26 15:21:20.000000 power-grid-model-1.5.0rc9190704883749/src/power_grid_model/core/power_grid_model.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5239 2023-06-26 15:21:20.000000 power-grid-model-1.5.0rc9190704883749/src/power_grid_model/data_types.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2183 2023-06-26 15:21:20.000000 power-grid-model-1.5.0rc9190704883749/src/power_grid_model/enum.py
+-rw-r--r--   0 runner    (1001) docker     (123)      505 2023-06-26 15:21:20.000000 power-grid-model-1.5.0rc9190704883749/src/power_grid_model/errors.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21645 2023-06-26 15:21:20.000000 power-grid-model-1.5.0rc9190704883749/src/power_grid_model/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 15:22:14.384742 power-grid-model-1.5.0rc9190704883749/src/power_grid_model/validation/
+-rw-r--r--   0 runner    (1001) docker     (123)      547 2023-06-26 15:21:20.000000 power-grid-model-1.5.0rc9190704883749/src/power_grid_model/validation/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4166 2023-06-26 15:21:20.000000 power-grid-model-1.5.0rc9190704883749/src/power_grid_model/validation/assertions.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14686 2023-06-26 15:21:20.000000 power-grid-model-1.5.0rc9190704883749/src/power_grid_model/validation/errors.py
+-rw-r--r--   0 runner    (1001) docker     (123)    30704 2023-06-26 15:21:20.000000 power-grid-model-1.5.0rc9190704883749/src/power_grid_model/validation/rules.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8601 2023-06-26 15:21:20.000000 power-grid-model-1.5.0rc9190704883749/src/power_grid_model/validation/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)    28618 2023-06-26 15:21:20.000000 power-grid-model-1.5.0rc9190704883749/src/power_grid_model/validation/validation.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 15:22:14.384742 power-grid-model-1.5.0rc9190704883749/src/power_grid_model.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     8142 2023-06-26 15:22:14.000000 power-grid-model-1.5.0rc9190704883749/src/power_grid_model.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    37119 2023-06-26 15:22:14.000000 power-grid-model-1.5.0rc9190704883749/src/power_grid_model.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-26 15:22:14.000000 power-grid-model-1.5.0rc9190704883749/src/power_grid_model.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      195 2023-06-26 15:22:14.000000 power-grid-model-1.5.0rc9190704883749/src/power_grid_model.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       17 2023-06-26 15:22:14.000000 power-grid-model-1.5.0rc9190704883749/src/power_grid_model.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 15:22:14.376742 power-grid-model-1.5.0rc9190704883749/tests/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 15:22:14.372742 power-grid-model-1.5.0rc9190704883749/tests/data/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 15:22:14.372742 power-grid-model-1.5.0rc9190704883749/tests/data/power_flow/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 15:22:14.388742 power-grid-model-1.5.0rc9190704883749/tests/data/power_flow/1os2msr/
+-rw-r--r--   0 runner    (1001) docker     (123)     1100 2023-06-26 15:21:20.000000 power-grid-model-1.5.0rc9190704883749/tests/data/power_flow/1os2msr/input.json
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-06-26 15:21:20.000000 power-grid-model-1.5.0rc9190704883749/tests/data/power_flow/1os2msr/input.json.license
+-rw-r--r--   0 runner    (1001) docker     (123)       76 2023-06-26 15:21:20.000000 power-grid-model-1.5.0rc9190704883749/tests/data/power_flow/1os2msr/params.json
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-06-26 15:21:20.000000 power-grid-model-1.5.0rc9190704883749/tests/data/power_flow/1os2msr/params.json.license
+-rw-r--r--   0 runner    (1001) docker     (123)     1582 2023-06-26 15:21:20.000000 power-grid-model-1.5.0rc9190704883749/tests/data/power_flow/1os2msr/sym_output.json
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-06-26 15:21:20.000000 power-grid-model-1.5.0rc9190704883749/tests/data/power_flow/1os2msr/sym_output.json.license
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 15:22:14.388742 power-grid-model-1.5.0rc9190704883749/tests/data/power_flow/dummy-test/
+-rw-r--r--   0 runner    (1001) docker     (123)     1429 2023-06-26 15:21:20.000000 power-grid-model-1.5.0rc9190704883749/tests/data/power_flow/dummy-test/input.json
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-06-26 15:21:20.000000 power-grid-model-1.5.0rc9190704883749/tests/data/power_flow/dummy-test/input.json.license
+-rw-r--r--   0 runner    (1001) docker     (123)       99 2023-06-26 15:21:20.000000 power-grid-model-1.5.0rc9190704883749/tests/data/power_flow/dummy-test/params.json
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-06-26 15:21:20.000000 power-grid-model-1.5.0rc9190704883749/tests/data/power_flow/dummy-test/params.json.license
+-rw-r--r--   0 runner    (1001) docker     (123)      666 2023-06-26 15:21:20.000000 power-grid-model-1.5.0rc9190704883749/tests/data/power_flow/dummy-test/sym_output.json
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-06-26 15:21:20.000000 power-grid-model-1.5.0rc9190704883749/tests/data/power_flow/dummy-test/sym_output.json.license
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 15:22:14.388742 power-grid-model-1.5.0rc9190704883749/tests/data/power_flow/dummy-test-batch/
+-rw-r--r--   0 runner    (1001) docker     (123)      764 2023-06-26 15:21:20.000000 power-grid-model-1.5.0rc9190704883749/tests/data/power_flow/dummy-test-batch/input.json
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-06-26 15:21:20.000000 power-grid-model-1.5.0rc9190704883749/tests/data/power_flow/dummy-test-batch/input.json.license
+-rw-r--r--   0 runner    (1001) docker     (123)       68 2023-06-26 15:21:20.000000 power-grid-model-1.5.0rc9190704883749/tests/data/power_flow/dummy-test-batch/params.json
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-06-26 15:21:20.000000 power-grid-model-1.5.0rc9190704883749/tests/data/power_flow/dummy-test-batch/params.json.license
+-rw-r--r--   0 runner    (1001) docker     (123)      107 2023-06-26 15:21:20.000000 power-grid-model-1.5.0rc9190704883749/tests/data/power_flow/dummy-test-batch/sym_output.json
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-06-26 15:21:20.000000 power-grid-model-1.5.0rc9190704883749/tests/data/power_flow/dummy-test-batch/sym_output.json.license
+-rw-r--r--   0 runner    (1001) docker     (123)      392 2023-06-26 15:21:20.000000 power-grid-model-1.5.0rc9190704883749/tests/data/power_flow/dummy-test-batch/sym_output_batch.json
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-06-26 15:21:20.000000 power-grid-model-1.5.0rc9190704883749/tests/data/power_flow/dummy-test-batch/sym_output_batch.json.license
+-rw-r--r--   0 runner    (1001) docker     (123)      359 2023-06-26 15:21:20.000000 power-grid-model-1.5.0rc9190704883749/tests/data/power_flow/dummy-test-batch/update_batch.json
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-06-26 15:21:20.000000 power-grid-model-1.5.0rc9190704883749/tests/data/power_flow/dummy-test-batch/update_batch.json.license
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 15:22:14.388742 power-grid-model-1.5.0rc9190704883749/tests/data/power_flow/dummy-test-batch-dependent-cacheable/
+-rw-r--r--   0 runner    (1001) docker     (123)      764 2023-06-26 15:21:20.000000 power-grid-model-1.5.0rc9190704883749/tests/data/power_flow/dummy-test-batch-dependent-cacheable/input.json
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-06-26 15:21:20.000000 power-grid-model-1.5.0rc9190704883749/tests/data/power_flow/dummy-test-batch-dependent-cacheable/input.json.license
+-rw-r--r--   0 runner    (1001) docker     (123)       99 2023-06-26 15:21:20.000000 power-grid-model-1.5.0rc9190704883749/tests/data/power_flow/dummy-test-batch-dependent-cacheable/params.json
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-06-26 15:21:20.000000 power-grid-model-1.5.0rc9190704883749/tests/data/power_flow/dummy-test-batch-dependent-cacheable/params.json.license
+-rw-r--r--   0 runner    (1001) docker     (123)      107 2023-06-26 15:21:20.000000 power-grid-model-1.5.0rc9190704883749/tests/data/power_flow/dummy-test-batch-dependent-cacheable/sym_output.json
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-06-26 15:21:20.000000 power-grid-model-1.5.0rc9190704883749/tests/data/power_flow/dummy-test-batch-dependent-cacheable/sym_output.json.license
+-rw-r--r--   0 runner    (1001) docker     (123)      392 2023-06-26 15:21:20.000000 power-grid-model-1.5.0rc9190704883749/tests/data/power_flow/dummy-test-batch-dependent-cacheable/sym_output_batch.json
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-06-26 15:21:20.000000 power-grid-model-1.5.0rc9190704883749/tests/data/power_flow/dummy-test-batch-dependent-cacheable/sym_output_batch.json.license
+-rw-r--r--   0 runner    (1001) docker     (123)      466 2023-06-26 15:21:20.000000 power-grid-model-1.5.0rc9190704883749/tests/data/power_flow/dummy-test-batch-dependent-cacheable/update_batch.json
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-06-26 15:21:20.000000 power-grid-model-1.5.0rc9190704883749/tests/data/power_flow/dummy-test-batch-dependent-cacheable/update_batch.json.license
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 15:22:14.392742 power-grid-model-1.5.0rc9190704883749/tests/data/power_flow/dummy-test-batch-dependent-not-cacheable/
+-rw-r--r--   0 runner    (1001) docker     (123)      764 2023-06-26 15:21:20.000000 power-grid-model-1.5.0rc9190704883749/tests/data/power_flow/dummy-test-batch-dependent-not-cacheable/input.json
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-06-26 15:21:20.000000 power-grid-model-1.5.0rc9190704883749/tests/data/power_flow/dummy-test-batch-dependent-not-cacheable/input.json.license
+-rw-r--r--   0 runner    (1001) docker     (123)       99 2023-06-26 15:21:20.000000 power-grid-model-1.5.0rc9190704883749/tests/data/power_flow/dummy-test-batch-dependent-not-cacheable/params.json
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-06-26 15:21:20.000000 power-grid-model-1.5.0rc9190704883749/tests/data/power_flow/dummy-test-batch-dependent-not-cacheable/params.json.license
+-rw-r--r--   0 runner    (1001) docker     (123)      107 2023-06-26 15:21:20.000000 power-grid-model-1.5.0rc9190704883749/tests/data/power_flow/dummy-test-batch-dependent-not-cacheable/sym_output.json
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-06-26 15:21:20.000000 power-grid-model-1.5.0rc9190704883749/tests/data/power_flow/dummy-test-batch-dependent-not-cacheable/sym_output.json.license
+-rw-r--r--   0 runner    (1001) docker     (123)      392 2023-06-26 15:21:20.000000 power-grid-model-1.5.0rc9190704883749/tests/data/power_flow/dummy-test-batch-dependent-not-cacheable/sym_output_batch.json
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-06-26 15:21:20.000000 power-grid-model-1.5.0rc9190704883749/tests/data/power_flow/dummy-test-batch-dependent-not-cacheable/sym_output_batch.json.license
+-rw-r--r--   0 runner    (1001) docker     (123)      542 2023-06-26 15:21:20.000000 power-grid-model-1.5.0rc9190704883749/tests/data/power_flow/dummy-test-batch-dependent-not-cacheable/update_batch.json
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-06-26 15:21:20.000000 power-grid-model-1.5.0rc9190704883749/tests/data/power_flow/dummy-test-batch-dependent-not-cacheable/update_batch.json.license
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 15:22:14.392742 power-grid-model-1.5.0rc9190704883749/tests/data/power_flow/dummy-test-batch-incomplete-input/
+-rw-r--r--   0 runner    (1001) docker     (123)      738 2023-06-26 15:21:20.000000 power-grid-model-1.5.0rc9190704883749/tests/data/power_flow/dummy-test-batch-incomplete-input/input.json
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-06-26 15:21:20.000000 power-grid-model-1.5.0rc9190704883749/tests/data/power_flow/dummy-test-batch-incomplete-input/input.json.license
+-rw-r--r--   0 runner    (1001) docker     (123)       68 2023-06-26 15:21:20.000000 power-grid-model-1.5.0rc9190704883749/tests/data/power_flow/dummy-test-batch-incomplete-input/params.json
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-06-26 15:21:20.000000 power-grid-model-1.5.0rc9190704883749/tests/data/power_flow/dummy-test-batch-incomplete-input/params.json.license
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-06-26 15:21:20.000000 power-grid-model-1.5.0rc9190704883749/tests/data/power_flow/dummy-test-batch-incomplete-input/sym_output.json.license
+-rw-r--r--   0 runner    (1001) docker     (123)      392 2023-06-26 15:21:20.000000 power-grid-model-1.5.0rc9190704883749/tests/data/power_flow/dummy-test-batch-incomplete-input/sym_output_batch.json
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-06-26 15:21:20.000000 power-grid-model-1.5.0rc9190704883749/tests/data/power_flow/dummy-test-batch-incomplete-input/sym_output_batch.json.license
+-rw-r--r--   0 runner    (1001) docker     (123)      401 2023-06-26 15:21:20.000000 power-grid-model-1.5.0rc9190704883749/tests/data/power_flow/dummy-test-batch-incomplete-input/update_batch.json
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-06-26 15:21:20.000000 power-grid-model-1.5.0rc9190704883749/tests/data/power_flow/dummy-test-batch-incomplete-input/update_batch.json.license
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 15:22:14.392742 power-grid-model-1.5.0rc9190704883749/tests/data/power_flow/dummy-test-batch-independent-cacheable/
+-rw-r--r--   0 runner    (1001) docker     (123)      764 2023-06-26 15:21:20.000000 power-grid-model-1.5.0rc9190704883749/tests/data/power_flow/dummy-test-batch-independent-cacheable/input.json
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-06-26 15:21:20.000000 power-grid-model-1.5.0rc9190704883749/tests/data/power_flow/dummy-test-batch-independent-cacheable/input.json.license
+-rw-r--r--   0 runner    (1001) docker     (123)       99 2023-06-26 15:21:20.000000 power-grid-model-1.5.0rc9190704883749/tests/data/power_flow/dummy-test-batch-independent-cacheable/params.json
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-06-26 15:21:20.000000 power-grid-model-1.5.0rc9190704883749/tests/data/power_flow/dummy-test-batch-independent-cacheable/params.json.license
+-rw-r--r--   0 runner    (1001) docker     (123)      107 2023-06-26 15:21:20.000000 power-grid-model-1.5.0rc9190704883749/tests/data/power_flow/dummy-test-batch-independent-cacheable/sym_output.json
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-06-26 15:21:20.000000 power-grid-model-1.5.0rc9190704883749/tests/data/power_flow/dummy-test-batch-independent-cacheable/sym_output.json.license
+-rw-r--r--   0 runner    (1001) docker     (123)      392 2023-06-26 15:21:20.000000 power-grid-model-1.5.0rc9190704883749/tests/data/power_flow/dummy-test-batch-independent-cacheable/sym_output_batch.json
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-06-26 15:21:20.000000 power-grid-model-1.5.0rc9190704883749/tests/data/power_flow/dummy-test-batch-independent-cacheable/sym_output_batch.json.license
+-rw-r--r--   0 runner    (1001) docker     (123)      466 2023-06-26 15:21:20.000000 power-grid-model-1.5.0rc9190704883749/tests/data/power_flow/dummy-test-batch-independent-cacheable/update_batch.json
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-06-26 15:21:20.000000 power-grid-model-1.5.0rc9190704883749/tests/data/power_flow/dummy-test-batch-independent-cacheable/update_batch.json.license
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 15:22:14.396742 power-grid-model-1.5.0rc9190704883749/tests/data/power_flow/dummy-test-batch-independent-not-cacheable/
+-rw-r--r--   0 runner    (1001) docker     (123)      764 2023-06-26 15:21:20.000000 power-grid-model-1.5.0rc9190704883749/tests/data/power_flow/dummy-test-batch-independent-not-cacheable/input.json
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-06-26 15:21:20.000000 power-grid-model-1.5.0rc9190704883749/tests/data/power_flow/dummy-test-batch-independent-not-cacheable/input.json.license
+-rw-r--r--   0 runner    (1001) docker     (123)       99 2023-06-26 15:21:20.000000 power-grid-model-1.5.0rc9190704883749/tests/data/power_flow/dummy-test-batch-independent-not-cacheable/params.json
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-06-26 15:21:20.000000 power-grid-model-1.5.0rc9190704883749/tests/data/power_flow/dummy-test-batch-independent-not-cacheable/params.json.license
+-rw-r--r--   0 runner    (1001) docker     (123)      107 2023-06-26 15:21:20.000000 power-grid-model-1.5.0rc9190704883749/tests/data/power_flow/dummy-test-batch-independent-not-cacheable/sym_output.json
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-06-26 15:21:20.000000 power-grid-model-1.5.0rc9190704883749/tests/data/power_flow/dummy-test-batch-independent-not-cacheable/sym_output.json.license
+-rw-r--r--   0 runner    (1001) docker     (123)      392 2023-06-26 15:21:20.000000 power-grid-model-1.5.0rc9190704883749/tests/data/power_flow/dummy-test-batch-independent-not-cacheable/sym_output_batch.json
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-06-26 15:21:20.000000 power-grid-model-1.5.0rc9190704883749/tests/data/power_flow/dummy-test-batch-independent-not-cacheable/sym_output_batch.json.license
+-rw-r--r--   0 runner    (1001) docker     (123)      694 2023-06-26 15:21:20.000000 power-grid-model-1.5.0rc9190704883749/tests/data/power_flow/dummy-test-batch-independent-not-cacheable/update_batch.json
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-06-26 15:21:20.000000 power-grid-model-1.5.0rc9190704883749/tests/data/power_flow/dummy-test-batch-independent-not-cacheable/update_batch.json.license
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 15:22:14.396742 power-grid-model-1.5.0rc9190704883749/tests/data/power_flow/dummy-test-batch-newton/
+-rw-r--r--   0 runner    (1001) docker     (123)      764 2023-06-26 15:21:20.000000 power-grid-model-1.5.0rc9190704883749/tests/data/power_flow/dummy-test-batch-newton/input.json
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-06-26 15:21:20.000000 power-grid-model-1.5.0rc9190704883749/tests/data/power_flow/dummy-test-batch-newton/input.json.license
+-rw-r--r--   0 runner    (1001) docker     (123)       99 2023-06-26 15:21:20.000000 power-grid-model-1.5.0rc9190704883749/tests/data/power_flow/dummy-test-batch-newton/params.json
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-06-26 15:21:20.000000 power-grid-model-1.5.0rc9190704883749/tests/data/power_flow/dummy-test-batch-newton/params.json.license
+-rw-r--r--   0 runner    (1001) docker     (123)      107 2023-06-26 15:21:20.000000 power-grid-model-1.5.0rc9190704883749/tests/data/power_flow/dummy-test-batch-newton/sym_output.json
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-06-26 15:21:20.000000 power-grid-model-1.5.0rc9190704883749/tests/data/power_flow/dummy-test-batch-newton/sym_output.json.license
+-rw-r--r--   0 runner    (1001) docker     (123)      476 2023-06-26 15:21:20.000000 power-grid-model-1.5.0rc9190704883749/tests/data/power_flow/dummy-test-batch-newton/sym_output_batch.json
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-06-26 15:21:20.000000 power-grid-model-1.5.0rc9190704883749/tests/data/power_flow/dummy-test-batch-newton/sym_output_batch.json.license
+-rw-r--r--   0 runner    (1001) docker     (123)      400 2023-06-26 15:21:20.000000 power-grid-model-1.5.0rc9190704883749/tests/data/power_flow/dummy-test-batch-newton/update_batch.json
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-06-26 15:21:20.000000 power-grid-model-1.5.0rc9190704883749/tests/data/power_flow/dummy-test-batch-newton/update_batch.json.license
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 15:22:14.396742 power-grid-model-1.5.0rc9190704883749/tests/data/power_flow/dummy-test-i-n-optional/
+-rw-r--r--   0 runner    (1001) docker     (123)     1411 2023-06-26 15:21:20.000000 power-grid-model-1.5.0rc9190704883749/tests/data/power_flow/dummy-test-i-n-optional/input.json
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-06-26 15:21:20.000000 power-grid-model-1.5.0rc9190704883749/tests/data/power_flow/dummy-test-i-n-optional/input.json.license
+-rw-r--r--   0 runner    (1001) docker     (123)       99 2023-06-26 15:21:20.000000 power-grid-model-1.5.0rc9190704883749/tests/data/power_flow/dummy-test-i-n-optional/params.json
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-06-26 15:21:20.000000 power-grid-model-1.5.0rc9190704883749/tests/data/power_flow/dummy-test-i-n-optional/params.json.license
+-rw-r--r--   0 runner    (1001) docker     (123)      666 2023-06-26 15:21:20.000000 power-grid-model-1.5.0rc9190704883749/tests/data/power_flow/dummy-test-i-n-optional/sym_output.json
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-06-26 15:21:20.000000 power-grid-model-1.5.0rc9190704883749/tests/data/power_flow/dummy-test-i-n-optional/sym_output.json.license
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 15:22:14.396742 power-grid-model-1.5.0rc9190704883749/tests/data/power_flow/gaia-example/
+-rw-r--r--   0 runner    (1001) docker     (123)      678 2023-06-26 15:21:20.000000 power-grid-model-1.5.0rc9190704883749/tests/data/power_flow/gaia-example/asym_output.json
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-06-26 15:21:20.000000 power-grid-model-1.5.0rc9190704883749/tests/data/power_flow/gaia-example/asym_output.json.license
+-rw-r--r--   0 runner    (1001) docker     (123)     2631 2023-06-26 15:21:20.000000 power-grid-model-1.5.0rc9190704883749/tests/data/power_flow/gaia-example/gaia_grid.gnf
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-06-26 15:21:20.000000 power-grid-model-1.5.0rc9190704883749/tests/data/power_flow/gaia-example/gaia_grid.gnf.license
+-rw-r--r--   0 runner    (1001) docker     (123)     1638 2023-06-26 15:21:20.000000 power-grid-model-1.5.0rc9190704883749/tests/data/power_flow/gaia-example/input.json
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-06-26 15:21:20.000000 power-grid-model-1.5.0rc9190704883749/tests/data/power_flow/gaia-example/input.json.license
+-rw-r--r--   0 runner    (1001) docker     (123)      100 2023-06-26 15:21:20.000000 power-grid-model-1.5.0rc9190704883749/tests/data/power_flow/gaia-example/params.json
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-06-26 15:21:20.000000 power-grid-model-1.5.0rc9190704883749/tests/data/power_flow/gaia-example/params.json.license
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 15:22:14.400743 power-grid-model-1.5.0rc9190704883749/tests/data/power_flow/multi-source-with-angle/
+-rw-r--r--   0 runner    (1001) docker     (123)     1088 2023-06-26 15:21:20.000000 power-grid-model-1.5.0rc9190704883749/tests/data/power_flow/multi-source-with-angle/input.json
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-06-26 15:21:20.000000 power-grid-model-1.5.0rc9190704883749/tests/data/power_flow/multi-source-with-angle/input.json.license
+-rw-r--r--   0 runner    (1001) docker     (123)      111 2023-06-26 15:21:20.000000 power-grid-model-1.5.0rc9190704883749/tests/data/power_flow/multi-source-with-angle/params.json
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-06-26 15:21:20.000000 power-grid-model-1.5.0rc9190704883749/tests/data/power_flow/multi-source-with-angle/params.json.license
+-rw-r--r--   0 runner    (1001) docker     (123)      399 2023-06-26 15:21:20.000000 power-grid-model-1.5.0rc9190704883749/tests/data/power_flow/multi-source-with-angle/sym_output.json
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-06-26 15:21:20.000000 power-grid-model-1.5.0rc9190704883749/tests/data/power_flow/multi-source-with-angle/sym_output.json.license
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 15:22:14.372742 power-grid-model-1.5.0rc9190704883749/tests/data/power_flow/pandapower/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 15:22:14.372742 power-grid-model-1.5.0rc9190704883749/tests/data/power_flow/pandapower/components/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 15:22:14.372742 power-grid-model-1.5.0rc9190704883749/tests/data/power_flow/pandapower/components/asymmetric/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 15:22:14.400743 power-grid-model-1.5.0rc9190704883749/tests/data/power_flow/pandapower/components/asymmetric/asym_gen/
+-rw-r--r--   0 runner    (1001) docker     (123)      672 2023-06-26 15:21:20.000000 power-grid-model-1.5.0rc9190704883749/tests/data/power_flow/pandapower/components/asymmetric/asym_gen/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1743 2023-06-26 15:21:20.000000 power-grid-model-1.5.0rc9190704883749/tests/data/power_flow/pandapower/components/asymmetric/asym_gen/asym_output.json
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-06-26 15:21:20.000000 power-grid-model-1.5.0rc9190704883749/tests/data/power_flow/pandapower/components/asymmetric/asym_gen/asym_output.json.license
+-rw-r--r--   0 runner    (1001) docker     (123)     1089 2023-06-26 15:21:20.000000 power-grid-model-1.5.0rc9190704883749/tests/data/power_flow/pandapower/components/asymmetric/asym_gen/input.json
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-06-26 15:21:20.000000 power-grid-model-1.5.0rc9190704883749/tests/data/power_flow/pandapower/components/asymmetric/asym_gen/input.json.license
+-rw-r--r--   0 runner    (1001) docker     (123)      101 2023-06-26 15:21:20.000000 power-grid-model-1.5.0rc9190704883749/tests/data/power_flow/pandapower/components/asymmetric/asym_gen/params.json
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-06-26 15:21:20.000000 power-grid-model-1.5.0rc9190704883749/tests/data/power_flow/pandapower/components/asymmetric/asym_gen/params.json.license
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 15:22:14.400743 power-grid-model-1.5.0rc9190704883749/tests/data/power_flow/pandapower/components/asymmetric/asym_load/
+-rw-r--r--   0 runner    (1001) docker     (123)      659 2023-06-26 15:21:20.000000 power-grid-model-1.5.0rc9190704883749/tests/data/power_flow/pandapower/components/asymmetric/asym_load/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1749 2023-06-26 15:21:20.000000 power-grid-model-1.5.0rc9190704883749/tests/data/power_flow/pandapower/components/asymmetric/asym_load/asym_output.json
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-06-26 15:21:20.000000 power-grid-model-1.5.0rc9190704883749/tests/data/power_flow/pandapower/components/asymmetric/asym_load/asym_output.json.license
+-rw-r--r--   0 runner    (1001) docker     (123)     1090 2023-06-26 15:21:20.000000 power-grid-model-1.5.0rc9190704883749/tests/data/power_flow/pandapower/components/asymmetric/asym_load/input.json
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-06-26 15:21:20.000000 power-grid-model-1.5.0rc9190704883749/tests/data/power_flow/pandapower/components/asymmetric/asym_load/input.json.license
+-rw-r--r--   0 runner    (1001) docker     (123)      101 2023-06-26 15:21:20.000000 power-grid-model-1.5.0rc9190704883749/tests/data/power_flow/pandapower/components/asymmetric/asym_load/params.json
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-06-26 15:21:20.000000 power-grid-model-1.5.0rc9190704883749/tests/data/power_flow/pandapower/components/asymmetric/asym_load/params.json.license
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 15:22:14.404743 power-grid-model-1.5.0rc9190704883749/tests/data/power_flow/pandapower/components/asymmetric/line/
+-rw-r--r--   0 runner    (1001) docker     (123)      910 2023-06-26 15:21:20.000000 power-grid-model-1.5.0rc9190704883749/tests/data/power_flow/pandapower/components/asymmetric/line/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)     3462 2023-06-26 15:21:20.000000 power-grid-model-1.5.0rc9190704883749/tests/data/power_flow/pandapower/components/asymmetric/line/asym_output.json
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-06-26 15:21:20.000000 power-grid-model-1.5.0rc9190704883749/tests/data/power_flow/pandapower/components/asymmetric/line/asym_output.json.license
+-rw-r--r--   0 runner    (1001) docker     (123)     2031 2023-06-26 15:21:20.000000 power-grid-model-1.5.0rc9190704883749/tests/data/power_flow/pandapower/components/asymmetric/line/input.json
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-06-26 15:21:20.000000 power-grid-model-1.5.0rc9190704883749/tests/data/power_flow/pandapower/components/asymmetric/line/input.json.license
+-rw-r--r--   0 runner    (1001) docker     (123)      101 2023-06-26 15:21:20.000000 power-grid-model-1.5.0rc9190704883749/tests/data/power_flow/pandapower/components/asymmetric/line/params.json
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-06-26 15:21:20.000000 power-grid-model-1.5.0rc9190704883749/tests/data/power_flow/pandapower/components/asymmetric/line/params.json.license
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 15:22:14.404743 power-grid-model-1.5.0rc9190704883749/tests/data/power_flow/pandapower/components/asymmetric/node/
+-rw-r--r--   0 runner    (1001) docker     (123)      595 2023-06-26 15:21:20.000000 power-grid-model-1.5.0rc9190704883749/tests/data/power_flow/pandapower/components/asymmetric/node/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1635 2023-06-26 15:21:20.000000 power-grid-model-1.5.0rc9190704883749/tests/data/power_flow/pandapower/components/asymmetric/node/asym_output.json
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-06-26 15:21:20.000000 power-grid-model-1.5.0rc9190704883749/tests/data/power_flow/pandapower/components/asymmetric/node/asym_output.json.license
+-rw-r--r--   0 runner    (1001) docker     (123)      642 2023-06-26 15:21:20.000000 power-grid-model-1.5.0rc9190704883749/tests/data/power_flow/pandapower/components/asymmetric/node/input.json
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-06-26 15:21:20.000000 power-grid-model-1.5.0rc9190704883749/tests/data/power_flow/pandapower/components/asymmetric/node/input.json.license
+-rw-r--r--   0 runner    (1001) docker     (123)      100 2023-06-26 15:21:20.000000 power-grid-model-1.5.0rc9190704883749/tests/data/power_flow/pandapower/components/asymmetric/node/params.json
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-06-26 15:21:20.000000 power-grid-model-1.5.0rc9190704883749/tests/data/power_flow/pandapower/components/asymmetric/node/params.json.license
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 15:22:14.404743 power-grid-model-1.5.0rc9190704883749/tests/data/power_flow/pandapower/components/asymmetric/shunt/
+-rw-r--r--   0 runner    (1001) docker     (123)      629 2023-06-26 15:21:20.000000 power-grid-model-1.5.0rc9190704883749/tests/data/power_flow/pandapower/components/asymmetric/shunt/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1385 2023-06-26 15:21:20.000000 power-grid-model-1.5.0rc9190704883749/tests/data/power_flow/pandapower/components/asymmetric/shunt/asym_output.json
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-06-26 15:21:20.000000 power-grid-model-1.5.0rc9190704883749/tests/data/power_flow/pandapower/components/asymmetric/shunt/asym_output.json.license
+-rw-r--r--   0 runner    (1001) docker     (123)      884 2023-06-26 15:21:20.000000 power-grid-model-1.5.0rc9190704883749/tests/data/power_flow/pandapower/components/asymmetric/shunt/input.json
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-06-26 15:21:20.000000 power-grid-model-1.5.0rc9190704883749/tests/data/power_flow/pandapower/components/asymmetric/shunt/input.json.license
+-rw-r--r--   0 runner    (1001) docker     (123)      101 2023-06-26 15:21:20.000000 power-grid-model-1.5.0rc9190704883749/tests/data/power_flow/pandapower/components/asymmetric/shunt/params.json
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-06-26 15:21:20.000000 power-grid-model-1.5.0rc9190704883749/tests/data/power_flow/pandapower/components/asymmetric/shunt/params.json.license
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 15:22:14.408743 power-grid-model-1.5.0rc9190704883749/tests/data/power_flow/pandapower/components/asymmetric/source/
+-rw-r--r--   0 runner    (1001) docker     (123)      579 2023-06-26 15:21:20.000000 power-grid-model-1.5.0rc9190704883749/tests/data/power_flow/pandapower/components/asymmetric/source/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)     2453 2023-06-26 15:21:20.000000 power-grid-model-1.5.0rc9190704883749/tests/data/power_flow/pandapower/components/asymmetric/source/asym_output.json
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-06-26 15:21:20.000000 power-grid-model-1.5.0rc9190704883749/tests/data/power_flow/pandapower/components/asymmetric/source/asym_output.json.license
+-rw-r--r--   0 runner    (1001) docker     (123)     1073 2023-06-26 15:21:20.000000 power-grid-model-1.5.0rc9190704883749/tests/data/power_flow/pandapower/components/asymmetric/source/input.json
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-06-26 15:21:20.000000 power-grid-model-1.5.0rc9190704883749/tests/data/power_flow/pandapower/components/asymmetric/source/input.json.license
+-rw-r--r--   0 runner    (1001) docker     (123)      101 2023-06-26 15:21:20.000000 power-grid-model-1.5.0rc9190704883749/tests/data/power_flow/pandapower/components/asymmetric/source/params.json
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-06-26 15:21:20.000000 power-grid-model-1.5.0rc9190704883749/tests/data/power_flow/pandapower/components/asymmetric/source/params.json.license
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 15:22:14.408743 power-grid-model-1.5.0rc9190704883749/tests/data/power_flow/pandapower/components/asymmetric/sym_gen/
+-rw-r--r--   0 runner    (1001) docker     (123)      853 2023-06-26 15:21:20.000000 power-grid-model-1.5.0rc9190704883749/tests/data/power_flow/pandapower/components/asymmetric/sym_gen/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1803 2023-06-26 15:21:20.000000 power-grid-model-1.5.0rc9190704883749/tests/data/power_flow/pandapower/components/asymmetric/sym_gen/asym_output.json
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-06-26 15:21:20.000000 power-grid-model-1.5.0rc9190704883749/tests/data/power_flow/pandapower/components/asymmetric/sym_gen/asym_output.json.license
+-rw-r--r--   0 runner    (1001) docker     (123)      886 2023-06-26 15:21:20.000000 power-grid-model-1.5.0rc9190704883749/tests/data/power_flow/pandapower/components/asymmetric/sym_gen/input.json
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-06-26 15:21:20.000000 power-grid-model-1.5.0rc9190704883749/tests/data/power_flow/pandapower/components/asymmetric/sym_gen/input.json.license
+-rw-r--r--   0 runner    (1001) docker     (123)      101 2023-06-26 15:21:20.000000 power-grid-model-1.5.0rc9190704883749/tests/data/power_flow/pandapower/components/asymmetric/sym_gen/params.json
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-06-26 15:21:20.000000 power-grid-model-1.5.0rc9190704883749/tests/data/power_flow/pandapower/components/asymmetric/sym_gen/params.json.license
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 15:22:14.412743 power-grid-model-1.5.0rc9190704883749/tests/data/power_flow/pandapower/components/asymmetric/sym_load/
+-rw-r--r--   0 runner    (1001) docker     (123)      841 2023-06-26 15:21:20.000000 power-grid-model-1.5.0rc9190704883749/tests/data/power_flow/pandapower/components/asymmetric/sym_load/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1802 2023-06-26 15:21:20.000000 power-grid-model-1.5.0rc9190704883749/tests/data/power_flow/pandapower/components/asymmetric/sym_load/asym_output.json
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-06-26 15:21:20.000000 power-grid-model-1.5.0rc9190704883749/tests/data/power_flow/pandapower/components/asymmetric/sym_load/asym_output.json.license
+-rw-r--r--   0 runner    (1001) docker     (123)      887 2023-06-26 15:21:20.000000 power-grid-model-1.5.0rc9190704883749/tests/data/power_flow/pandapower/components/asymmetric/sym_load/input.json
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-06-26 15:21:20.000000 power-grid-model-1.5.0rc9190704883749/tests/data/power_flow/pandapower/components/asymmetric/sym_load/input.json.license
+-rw-r--r--   0 runner    (1001) docker     (123)      101 2023-06-26 15:21:20.000000 power-grid-model-1.5.0rc9190704883749/tests/data/power_flow/pandapower/components/asymmetric/sym_load/params.json
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-06-26 15:21:20.000000 power-grid-model-1.5.0rc9190704883749/tests/data/power_flow/pandapower/components/asymmetric/sym_load/params.json.license
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 15:22:14.412743 power-grid-model-1.5.0rc9190704883749/tests/data/power_flow/pandapower/components/asymmetric/transformer/
+-rw-r--r--   0 runner    (1001) docker     (123)     1065 2023-06-26 15:21:20.000000 power-grid-model-1.5.0rc9190704883749/tests/data/power_flow/pandapower/components/asymmetric/transformer/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)    17633 2023-06-26 15:21:20.000000 power-grid-model-1.5.0rc9190704883749/tests/data/power_flow/pandapower/components/asymmetric/transformer/asym_output_batch.json
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-06-26 15:21:20.000000 power-grid-model-1.5.0rc9190704883749/tests/data/power_flow/pandapower/components/asymmetric/transformer/asym_output_batch.json.license
+-rw-r--r--   0 runner    (1001) docker     (123)      919 2023-06-26 15:21:20.000000 power-grid-model-1.5.0rc9190704883749/tests/data/power_flow/pandapower/components/asymmetric/transformer/input.json
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-06-26 15:21:20.000000 power-grid-model-1.5.0rc9190704883749/tests/data/power_flow/pandapower/components/asymmetric/transformer/input.json.license
+-rw-r--r--   0 runner    (1001) docker     (123)      102 2023-06-26 15:21:20.000000 power-grid-model-1.5.0rc9190704883749/tests/data/power_flow/pandapower/components/asymmetric/transformer/params.json
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-06-26 15:21:20.000000 power-grid-model-1.5.0rc9190704883749/tests/data/power_flow/pandapower/components/asymmetric/transformer/params.json.license
+-rw-r--r--   0 runner    (1001) docker     (123)      997 2023-06-26 15:21:20.000000 power-grid-model-1.5.0rc9190704883749/tests/data/power_flow/pandapower/components/asymmetric/transformer/update_batch.json
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-06-26 15:21:20.000000 power-grid-model-1.5.0rc9190704883749/tests/data/power_flow/pandapower/components/asymmetric/transformer/update_batch.json.license
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 15:22:14.372742 power-grid-model-1.5.0rc9190704883749/tests/data/power_flow/pandapower/components/symmetric/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 15:22:14.416743 power-grid-model-1.5.0rc9190704883749/tests/data/power_flow/pandapower/components/symmetric/basic-node/
+-rw-r--r--   0 runner    (1001) docker     (123)      448 2023-06-26 15:21:20.000000 power-grid-model-1.5.0rc9190704883749/tests/data/power_flow/pandapower/components/symmetric/basic-node/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      299 2023-06-26 15:21:20.000000 power-grid-model-1.5.0rc9190704883749/tests/data/power_flow/pandapower/components/symmetric/basic-node/input.json
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-06-26 15:21:20.000000 power-grid-model-1.5.0rc9190704883749/tests/data/power_flow/pandapower/components/symmetric/basic-node/input.json.license
+-rw-r--r--   0 runner    (1001) docker     (123)      101 2023-06-26 15:21:20.000000 power-grid-model-1.5.0rc9190704883749/tests/data/power_flow/pandapower/components/symmetric/basic-node/params.json
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-06-26 15:21:20.000000 power-grid-model-1.5.0rc9190704883749/tests/data/power_flow/pandapower/components/symmetric/basic-node/params.json.license
+-rw-r--r--   0 runner    (1001) docker     (123)      301 2023-06-26 15:21:20.000000 power-grid-model-1.5.0rc9190704883749/tests/data/power_flow/pandapower/components/symmetric/basic-node/sym_output.json
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-06-26 15:21:20.000000 power-grid-model-1.5.0rc9190704883749/tests/data/power_flow/pandapower/components/symmetric/basic-node/sym_output.json.license
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 15:22:14.416743 power-grid-model-1.5.0rc9190704883749/tests/data/power_flow/pandapower/components/symmetric/line/
+-rw-r--r--   0 runner    (1001) docker     (123)      775 2023-06-26 15:21:20.000000 power-grid-model-1.5.0rc9190704883749/tests/data/power_flow/pandapower/components/symmetric/line/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1938 2023-06-26 15:21:20.000000 power-grid-model-1.5.0rc9190704883749/tests/data/power_flow/pandapower/components/symmetric/line/input.json
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-06-26 15:21:20.000000 power-grid-model-1.5.0rc9190704883749/tests/data/power_flow/pandapower/components/symmetric/line/input.json.license
+-rw-r--r--   0 runner    (1001) docker     (123)      101 2023-06-26 15:21:20.000000 power-grid-model-1.5.0rc9190704883749/tests/data/power_flow/pandapower/components/symmetric/line/params.json
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-06-26 15:21:20.000000 power-grid-model-1.5.0rc9190704883749/tests/data/power_flow/pandapower/components/symmetric/line/params.json.license
+-rw-r--r--   0 runner    (1001) docker     (123)     2305 2023-06-26 15:21:20.000000 power-grid-model-1.5.0rc9190704883749/tests/data/power_flow/pandapower/components/symmetric/line/sym_output.json
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-06-26 15:21:20.000000 power-grid-model-1.5.0rc9190704883749/tests/data/power_flow/pandapower/components/symmetric/line/sym_output.json.license
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 15:22:14.416743 power-grid-model-1.5.0rc9190704883749/tests/data/power_flow/pandapower/components/symmetric/node/
+-rw-r--r--   0 runner    (1001) docker     (123)      462 2023-06-26 15:21:20.000000 power-grid-model-1.5.0rc9190704883749/tests/data/power_flow/pandapower/components/symmetric/node/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      651 2023-06-26 15:21:20.000000 power-grid-model-1.5.0rc9190704883749/tests/data/power_flow/pandapower/components/symmetric/node/input.json
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-06-26 15:21:20.000000 power-grid-model-1.5.0rc9190704883749/tests/data/power_flow/pandapower/components/symmetric/node/input.json.license
+-rw-r--r--   0 runner    (1001) docker     (123)      101 2023-06-26 15:21:20.000000 power-grid-model-1.5.0rc9190704883749/tests/data/power_flow/pandapower/components/symmetric/node/params.json
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-06-26 15:21:20.000000 power-grid-model-1.5.0rc9190704883749/tests/data/power_flow/pandapower/components/symmetric/node/params.json.license
+-rw-r--r--   0 runner    (1001) docker     (123)      907 2023-06-26 15:21:20.000000 power-grid-model-1.5.0rc9190704883749/tests/data/power_flow/pandapower/components/symmetric/node/sym_output.json
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-06-26 15:21:20.000000 power-grid-model-1.5.0rc9190704883749/tests/data/power_flow/pandapower/components/symmetric/node/sym_output.json.license
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 15:22:14.416743 power-grid-model-1.5.0rc9190704883749/tests/data/power_flow/pandapower/components/symmetric/shunt/
+-rw-r--r--   0 runner    (1001) docker     (123)      496 2023-06-26 15:21:20.000000 power-grid-model-1.5.0rc9190704883749/tests/data/power_flow/pandapower/components/symmetric/shunt/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      892 2023-06-26 15:21:20.000000 power-grid-model-1.5.0rc9190704883749/tests/data/power_flow/pandapower/components/symmetric/shunt/input.json
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-06-26 15:21:20.000000 power-grid-model-1.5.0rc9190704883749/tests/data/power_flow/pandapower/components/symmetric/shunt/input.json.license
+-rw-r--r--   0 runner    (1001) docker     (123)      101 2023-06-26 15:21:20.000000 power-grid-model-1.5.0rc9190704883749/tests/data/power_flow/pandapower/components/symmetric/shunt/params.json
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-06-26 15:21:20.000000 power-grid-model-1.5.0rc9190704883749/tests/data/power_flow/pandapower/components/symmetric/shunt/params.json.license
+-rw-r--r--   0 runner    (1001) docker     (123)      977 2023-06-26 15:21:20.000000 power-grid-model-1.5.0rc9190704883749/tests/data/power_flow/pandapower/components/symmetric/shunt/sym_output.json
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-06-26 15:21:20.000000 power-grid-model-1.5.0rc9190704883749/tests/data/power_flow/pandapower/components/symmetric/shunt/sym_output.json.license
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 15:22:14.420744 power-grid-model-1.5.0rc9190704883749/tests/data/power_flow/pandapower/components/symmetric/source/
+-rw-r--r--   0 runner    (1001) docker     (123)      483 2023-06-26 15:21:20.000000 power-grid-model-1.5.0rc9190704883749/tests/data/power_flow/pandapower/components/symmetric/source/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1089 2023-06-26 15:21:20.000000 power-grid-model-1.5.0rc9190704883749/tests/data/power_flow/pandapower/components/symmetric/source/input.json
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-06-26 15:21:20.000000 power-grid-model-1.5.0rc9190704883749/tests/data/power_flow/pandapower/components/symmetric/source/input.json.license
+-rw-r--r--   0 runner    (1001) docker     (123)      101 2023-06-26 15:21:20.000000 power-grid-model-1.5.0rc9190704883749/tests/data/power_flow/pandapower/components/symmetric/source/params.json
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-06-26 15:21:20.000000 power-grid-model-1.5.0rc9190704883749/tests/data/power_flow/pandapower/components/symmetric/source/params.json.license
+-rw-r--r--   0 runner    (1001) docker     (123)     1461 2023-06-26 15:21:20.000000 power-grid-model-1.5.0rc9190704883749/tests/data/power_flow/pandapower/components/symmetric/source/sym_output.json
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-06-26 15:21:20.000000 power-grid-model-1.5.0rc9190704883749/tests/data/power_flow/pandapower/components/symmetric/source/sym_output.json.license
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 15:22:14.420744 power-grid-model-1.5.0rc9190704883749/tests/data/power_flow/pandapower/components/symmetric/sym_gen/
+-rw-r--r--   0 runner    (1001) docker     (123)      753 2023-06-26 15:21:20.000000 power-grid-model-1.5.0rc9190704883749/tests/data/power_flow/pandapower/components/symmetric/sym_gen/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1172 2023-06-26 15:21:20.000000 power-grid-model-1.5.0rc9190704883749/tests/data/power_flow/pandapower/components/symmetric/sym_gen/input.json
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-06-26 15:21:20.000000 power-grid-model-1.5.0rc9190704883749/tests/data/power_flow/pandapower/components/symmetric/sym_gen/input.json.license
+-rw-r--r--   0 runner    (1001) docker     (123)      101 2023-06-26 15:21:20.000000 power-grid-model-1.5.0rc9190704883749/tests/data/power_flow/pandapower/components/symmetric/sym_gen/params.json
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-06-26 15:21:20.000000 power-grid-model-1.5.0rc9190704883749/tests/data/power_flow/pandapower/components/symmetric/sym_gen/params.json.license
+-rw-r--r--   0 runner    (1001) docker     (123)     1136 2023-06-26 15:21:20.000000 power-grid-model-1.5.0rc9190704883749/tests/data/power_flow/pandapower/components/symmetric/sym_gen/sym_output.json
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-06-26 15:21:20.000000 power-grid-model-1.5.0rc9190704883749/tests/data/power_flow/pandapower/components/symmetric/sym_gen/sym_output.json.license
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 15:22:14.420744 power-grid-model-1.5.0rc9190704883749/tests/data/power_flow/pandapower/components/symmetric/sym_load/
+-rw-r--r--   0 runner    (1001) docker     (123)      741 2023-06-26 15:21:20.000000 power-grid-model-1.5.0rc9190704883749/tests/data/power_flow/pandapower/components/symmetric/sym_load/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1173 2023-06-26 15:21:20.000000 power-grid-model-1.5.0rc9190704883749/tests/data/power_flow/pandapower/components/symmetric/sym_load/input.json
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-06-26 15:21:20.000000 power-grid-model-1.5.0rc9190704883749/tests/data/power_flow/pandapower/components/symmetric/sym_load/input.json.license
+-rw-r--r--   0 runner    (1001) docker     (123)       78 2023-06-26 15:21:20.000000 power-grid-model-1.5.0rc9190704883749/tests/data/power_flow/pandapower/components/symmetric/sym_load/params.json
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-06-26 15:21:20.000000 power-grid-model-1.5.0rc9190704883749/tests/data/power_flow/pandapower/components/symmetric/sym_load/params.json.license
+-rw-r--r--   0 runner    (1001) docker     (123)     1131 2023-06-26 15:21:20.000000 power-grid-model-1.5.0rc9190704883749/tests/data/power_flow/pandapower/components/symmetric/sym_load/sym_output.json
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-06-26 15:21:20.000000 power-grid-model-1.5.0rc9190704883749/tests/data/power_flow/pandapower/components/symmetric/sym_load/sym_output.json.license
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 15:22:14.424744 power-grid-model-1.5.0rc9190704883749/tests/data/power_flow/pandapower/components/symmetric/three_winding_transformer/
+-rw-r--r--   0 runner    (1001) docker     (123)      917 2023-06-26 15:21:20.000000 power-grid-model-1.5.0rc9190704883749/tests/data/power_flow/pandapower/components/symmetric/three_winding_transformer/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1095 2023-06-26 15:21:20.000000 power-grid-model-1.5.0rc9190704883749/tests/data/power_flow/pandapower/components/symmetric/three_winding_transformer/input.json
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-06-26 15:21:20.000000 power-grid-model-1.5.0rc9190704883749/tests/data/power_flow/pandapower/components/symmetric/three_winding_transformer/input.json.license
+-rw-r--r--   0 runner    (1001) docker     (123)       78 2023-06-26 15:21:20.000000 power-grid-model-1.5.0rc9190704883749/tests/data/power_flow/pandapower/components/symmetric/three_winding_transformer/params.json
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-06-26 15:21:20.000000 power-grid-model-1.5.0rc9190704883749/tests/data/power_flow/pandapower/components/symmetric/three_winding_transformer/params.json.license
+-rw-r--r--   0 runner    (1001) docker     (123)     8883 2023-06-26 15:21:20.000000 power-grid-model-1.5.0rc9190704883749/tests/data/power_flow/pandapower/components/symmetric/three_winding_transformer/sym_output_batch.json
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-06-26 15:21:20.000000 power-grid-model-1.5.0rc9190704883749/tests/data/power_flow/pandapower/components/symmetric/three_winding_transformer/sym_output_batch.json.license
+-rw-r--r--   0 runner    (1001) docker     (123)     1737 2023-06-26 15:21:20.000000 power-grid-model-1.5.0rc9190704883749/tests/data/power_flow/pandapower/components/symmetric/three_winding_transformer/update_batch.json
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-06-26 15:21:20.000000 power-grid-model-1.5.0rc9190704883749/tests/data/power_flow/pandapower/components/symmetric/three_winding_transformer/update_batch.json.license
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 15:22:14.424744 power-grid-model-1.5.0rc9190704883749/tests/data/power_flow/pandapower/components/symmetric/transformer/
+-rw-r--r--   0 runner    (1001) docker     (123)      883 2023-06-26 15:21:20.000000 power-grid-model-1.5.0rc9190704883749/tests/data/power_flow/pandapower/components/symmetric/transformer/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)     2275 2023-06-26 15:21:20.000000 power-grid-model-1.5.0rc9190704883749/tests/data/power_flow/pandapower/components/symmetric/transformer/input.json
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-06-26 15:21:20.000000 power-grid-model-1.5.0rc9190704883749/tests/data/power_flow/pandapower/components/symmetric/transformer/input.json.license
+-rw-r--r--   0 runner    (1001) docker     (123)      101 2023-06-26 15:21:20.000000 power-grid-model-1.5.0rc9190704883749/tests/data/power_flow/pandapower/components/symmetric/transformer/params.json
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-06-26 15:21:20.000000 power-grid-model-1.5.0rc9190704883749/tests/data/power_flow/pandapower/components/symmetric/transformer/params.json.license
+-rw-r--r--   0 runner    (1001) docker     (123)    15639 2023-06-26 15:21:20.000000 power-grid-model-1.5.0rc9190704883749/tests/data/power_flow/pandapower/components/symmetric/transformer/sym_output_batch.json
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-06-26 15:21:20.000000 power-grid-model-1.5.0rc9190704883749/tests/data/power_flow/pandapower/components/symmetric/transformer/sym_output_batch.json.license
+-rw-r--r--   0 runner    (1001) docker     (123)     2827 2023-06-26 15:21:20.000000 power-grid-model-1.5.0rc9190704883749/tests/data/power_flow/pandapower/components/symmetric/transformer/update_batch.json
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-06-26 15:21:20.000000 power-grid-model-1.5.0rc9190704883749/tests/data/power_flow/pandapower/components/symmetric/transformer/update_batch.json.license
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 15:22:14.372742 power-grid-model-1.5.0rc9190704883749/tests/data/power_flow/pandapower/networks/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 15:22:14.372742 power-grid-model-1.5.0rc9190704883749/tests/data/power_flow/pandapower/networks/asymmetric/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 15:22:14.424744 power-grid-model-1.5.0rc9190704883749/tests/data/power_flow/pandapower/networks/asymmetric/distribution-case/
+-rw-r--r--   0 runner    (1001) docker     (123)     1281 2023-06-26 15:21:20.000000 power-grid-model-1.5.0rc9190704883749/tests/data/power_flow/pandapower/networks/asymmetric/distribution-case/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)    15865 2023-06-26 15:21:20.000000 power-grid-model-1.5.0rc9190704883749/tests/data/power_flow/pandapower/networks/asymmetric/distribution-case/asym_output_batch.json
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-06-26 15:21:20.000000 power-grid-model-1.5.0rc9190704883749/tests/data/power_flow/pandapower/networks/asymmetric/distribution-case/asym_output_batch.json.license
+-rw-r--r--   0 runner    (1001) docker     (123)     8935 2023-06-26 15:21:20.000000 power-grid-model-1.5.0rc9190704883749/tests/data/power_flow/pandapower/networks/asymmetric/distribution-case/input.json
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-06-26 15:21:20.000000 power-grid-model-1.5.0rc9190704883749/tests/data/power_flow/pandapower/networks/asymmetric/distribution-case/input.json.license
+-rw-r--r--   0 runner    (1001) docker     (123)      101 2023-06-26 15:21:20.000000 power-grid-model-1.5.0rc9190704883749/tests/data/power_flow/pandapower/networks/asymmetric/distribution-case/params.json
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-06-26 15:21:20.000000 power-grid-model-1.5.0rc9190704883749/tests/data/power_flow/pandapower/networks/asymmetric/distribution-case/params.json.license
+-rw-r--r--   0 runner    (1001) docker     (123)     6642 2023-06-26 15:21:20.000000 power-grid-model-1.5.0rc9190704883749/tests/data/power_flow/pandapower/networks/asymmetric/distribution-case/update_batch.json
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-06-26 15:21:20.000000 power-grid-model-1.5.0rc9190704883749/tests/data/power_flow/pandapower/networks/asymmetric/distribution-case/update_batch.json.license
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 15:22:14.424744 power-grid-model-1.5.0rc9190704883749/tests/data/power_flow/pandapower/networks/asymmetric/transmission-case/
+-rw-r--r--   0 runner    (1001) docker     (123)     1068 2023-06-26 15:21:20.000000 power-grid-model-1.5.0rc9190704883749/tests/data/power_flow/pandapower/networks/asymmetric/transmission-case/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)    10605 2023-06-26 15:21:20.000000 power-grid-model-1.5.0rc9190704883749/tests/data/power_flow/pandapower/networks/asymmetric/transmission-case/asym_output.json
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-06-26 15:21:20.000000 power-grid-model-1.5.0rc9190704883749/tests/data/power_flow/pandapower/networks/asymmetric/transmission-case/asym_output.json.license
+-rw-r--r--   0 runner    (1001) docker     (123)     6208 2023-06-26 15:21:20.000000 power-grid-model-1.5.0rc9190704883749/tests/data/power_flow/pandapower/networks/asymmetric/transmission-case/input.json
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-06-26 15:21:20.000000 power-grid-model-1.5.0rc9190704883749/tests/data/power_flow/pandapower/networks/asymmetric/transmission-case/input.json.license
+-rw-r--r--   0 runner    (1001) docker     (123)       78 2023-06-26 15:21:20.000000 power-grid-model-1.5.0rc9190704883749/tests/data/power_flow/pandapower/networks/asymmetric/transmission-case/params.json
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-06-26 15:21:20.000000 power-grid-model-1.5.0rc9190704883749/tests/data/power_flow/pandapower/networks/asymmetric/transmission-case/params.json.license
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 15:22:14.372742 power-grid-model-1.5.0rc9190704883749/tests/data/power_flow/pandapower/networks/symmetric/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 15:22:14.428744 power-grid-model-1.5.0rc9190704883749/tests/data/power_flow/pandapower/networks/symmetric/distribution-case/
+-rw-r--r--   0 runner    (1001) docker     (123)     1365 2023-06-26 15:21:20.000000 power-grid-model-1.5.0rc9190704883749/tests/data/power_flow/pandapower/networks/symmetric/distribution-case/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)     8939 2023-06-26 15:21:20.000000 power-grid-model-1.5.0rc9190704883749/tests/data/power_flow/pandapower/networks/symmetric/distribution-case/input.json
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-06-26 15:21:20.000000 power-grid-model-1.5.0rc9190704883749/tests/data/power_flow/pandapower/networks/symmetric/distribution-case/input.json.license
+-rw-r--r--   0 runner    (1001) docker     (123)      101 2023-06-26 15:21:20.000000 power-grid-model-1.5.0rc9190704883749/tests/data/power_flow/pandapower/networks/symmetric/distribution-case/params.json
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-06-26 15:21:20.000000 power-grid-model-1.5.0rc9190704883749/tests/data/power_flow/pandapower/networks/symmetric/distribution-case/params.json.license
+-rw-r--r--   0 runner    (1001) docker     (123)     8702 2023-06-26 15:21:20.000000 power-grid-model-1.5.0rc9190704883749/tests/data/power_flow/pandapower/networks/symmetric/distribution-case/sym_output_batch.json
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-06-26 15:21:20.000000 power-grid-model-1.5.0rc9190704883749/tests/data/power_flow/pandapower/networks/symmetric/distribution-case/sym_output_batch.json.license
+-rw-r--r--   0 runner    (1001) docker     (123)     6642 2023-06-26 15:21:20.000000 power-grid-model-1.5.0rc9190704883749/tests/data/power_flow/pandapower/networks/symmetric/distribution-case/update_batch.json
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-06-26 15:21:20.000000 power-grid-model-1.5.0rc9190704883749/tests/data/power_flow/pandapower/networks/symmetric/distribution-case/update_batch.json.license
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 15:22:14.428744 power-grid-model-1.5.0rc9190704883749/tests/data/power_flow/pandapower/networks/symmetric/transmission-case/
+-rw-r--r--   0 runner    (1001) docker     (123)     1068 2023-06-26 15:21:20.000000 power-grid-model-1.5.0rc9190704883749/tests/data/power_flow/pandapower/networks/symmetric/transmission-case/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)     6216 2023-06-26 15:21:20.000000 power-grid-model-1.5.0rc9190704883749/tests/data/power_flow/pandapower/networks/symmetric/transmission-case/input.json
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-06-26 15:21:20.000000 power-grid-model-1.5.0rc9190704883749/tests/data/power_flow/pandapower/networks/symmetric/transmission-case/input.json.license
+-rw-r--r--   0 runner    (1001) docker     (123)       78 2023-06-26 15:21:20.000000 power-grid-model-1.5.0rc9190704883749/tests/data/power_flow/pandapower/networks/symmetric/transmission-case/params.json
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-06-26 15:21:20.000000 power-grid-model-1.5.0rc9190704883749/tests/data/power_flow/pandapower/networks/symmetric/transmission-case/params.json.license
+-rw-r--r--   0 runner    (1001) docker     (123)     5384 2023-06-26 15:21:20.000000 power-grid-model-1.5.0rc9190704883749/tests/data/power_flow/pandapower/networks/symmetric/transmission-case/sym_output.json
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-06-26 15:21:20.000000 power-grid-model-1.5.0rc9190704883749/tests/data/power_flow/pandapower/networks/symmetric/transmission-case/sym_output.json.license
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 15:22:14.428744 power-grid-model-1.5.0rc9190704883749/tests/data/power_flow/r-state-estimation/
+-rw-r--r--   0 runner    (1001) docker     (123)     1492 2023-06-26 15:21:20.000000 power-grid-model-1.5.0rc9190704883749/tests/data/power_flow/r-state-estimation/input.json
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-06-26 15:21:20.000000 power-grid-model-1.5.0rc9190704883749/tests/data/power_flow/r-state-estimation/input.json.license
+-rw-r--r--   0 runner    (1001) docker     (123)       68 2023-06-26 15:21:20.000000 power-grid-model-1.5.0rc9190704883749/tests/data/power_flow/r-state-estimation/params.json
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-06-26 15:21:20.000000 power-grid-model-1.5.0rc9190704883749/tests/data/power_flow/r-state-estimation/params.json.license
+-rw-r--r--   0 runner    (1001) docker     (123)      575 2023-06-26 15:21:20.000000 power-grid-model-1.5.0rc9190704883749/tests/data/power_flow/r-state-estimation/sym_output.json
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-06-26 15:21:20.000000 power-grid-model-1.5.0rc9190704883749/tests/data/power_flow/r-state-estimation/sym_output.json.license
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 15:22:14.428744 power-grid-model-1.5.0rc9190704883749/tests/data/power_flow/three-winding-transformer/
+-rw-r--r--   0 runner    (1001) docker     (123)    21196 2023-06-26 15:21:20.000000 power-grid-model-1.5.0rc9190704883749/tests/data/power_flow/three-winding-transformer/asym_output_batch.json
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-06-26 15:21:20.000000 power-grid-model-1.5.0rc9190704883749/tests/data/power_flow/three-winding-transformer/asym_output_batch.json.license
+-rw-r--r--   0 runner    (1001) docker     (123)     1089 2023-06-26 15:21:20.000000 power-grid-model-1.5.0rc9190704883749/tests/data/power_flow/three-winding-transformer/input.json
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-06-26 15:21:20.000000 power-grid-model-1.5.0rc9190704883749/tests/data/power_flow/three-winding-transformer/input.json.license
+-rw-r--r--   0 runner    (1001) docker     (123)      101 2023-06-26 15:21:20.000000 power-grid-model-1.5.0rc9190704883749/tests/data/power_flow/three-winding-transformer/params.json
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-06-26 15:21:20.000000 power-grid-model-1.5.0rc9190704883749/tests/data/power_flow/three-winding-transformer/params.json.license
+-rw-r--r--   0 runner    (1001) docker     (123)     7374 2023-06-26 15:21:20.000000 power-grid-model-1.5.0rc9190704883749/tests/data/power_flow/three-winding-transformer/sym_output_batch.json
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-06-26 15:21:20.000000 power-grid-model-1.5.0rc9190704883749/tests/data/power_flow/three-winding-transformer/sym_output_batch.json.license
+-rw-r--r--   0 runner    (1001) docker     (123)     1737 2023-06-26 15:21:20.000000 power-grid-model-1.5.0rc9190704883749/tests/data/power_flow/three-winding-transformer/update_batch.json
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-06-26 15:21:20.000000 power-grid-model-1.5.0rc9190704883749/tests/data/power_flow/three-winding-transformer/update_batch.json.license
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 15:22:14.432744 power-grid-model-1.5.0rc9190704883749/tests/data/power_flow/vision-example/
+-rw-r--r--   0 runner    (1001) docker     (123)      623 2023-06-26 15:21:20.000000 power-grid-model-1.5.0rc9190704883749/tests/data/power_flow/vision-example/asym_output.json
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-06-26 15:21:20.000000 power-grid-model-1.5.0rc9190704883749/tests/data/power_flow/vision-example/asym_output.json.license
+-rw-r--r--   0 runner    (1001) docker     (123)     1575 2023-06-26 15:21:20.000000 power-grid-model-1.5.0rc9190704883749/tests/data/power_flow/vision-example/input.json
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-06-26 15:21:20.000000 power-grid-model-1.5.0rc9190704883749/tests/data/power_flow/vision-example/input.json.license
+-rw-r--r--   0 runner    (1001) docker     (123)       74 2023-06-26 15:21:20.000000 power-grid-model-1.5.0rc9190704883749/tests/data/power_flow/vision-example/params.json
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-06-26 15:21:20.000000 power-grid-model-1.5.0rc9190704883749/tests/data/power_flow/vision-example/params.json.license
+-rw-r--r--   0 runner    (1001) docker     (123)     2450 2023-06-26 15:21:20.000000 power-grid-model-1.5.0rc9190704883749/tests/data/power_flow/vision-example/vision_grid.vnf
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-06-26 15:21:20.000000 power-grid-model-1.5.0rc9190704883749/tests/data/power_flow/vision-example/vision_grid.vnf.license
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 15:22:14.432744 power-grid-model-1.5.0rc9190704883749/tests/data/power_flow/vision-validation-network/
+-rw-r--r--   0 runner    (1001) docker     (123)    20486 2023-06-26 15:21:20.000000 power-grid-model-1.5.0rc9190704883749/tests/data/power_flow/vision-validation-network/asym_output.json
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-06-26 15:21:20.000000 power-grid-model-1.5.0rc9190704883749/tests/data/power_flow/vision-validation-network/asym_output.json.license
+-rw-r--r--   0 runner    (1001) docker     (123)    30756 2023-06-26 15:21:20.000000 power-grid-model-1.5.0rc9190704883749/tests/data/power_flow/vision-validation-network/input.json
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-06-26 15:21:20.000000 power-grid-model-1.5.0rc9190704883749/tests/data/power_flow/vision-validation-network/input.json.license
+-rw-r--r--   0 runner    (1001) docker     (123)      363 2023-06-26 15:21:20.000000 power-grid-model-1.5.0rc9190704883749/tests/data/power_flow/vision-validation-network/params.json
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-06-26 15:21:20.000000 power-grid-model-1.5.0rc9190704883749/tests/data/power_flow/vision-validation-network/params.json.license
+-rw-r--r--   0 runner    (1001) docker     (123)    11853 2023-06-26 15:21:20.000000 power-grid-model-1.5.0rc9190704883749/tests/data/power_flow/vision-validation-network/sym_output.json
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-06-26 15:21:20.000000 power-grid-model-1.5.0rc9190704883749/tests/data/power_flow/vision-validation-network/sym_output.json.license
+-rw-r--r--   0 runner    (1001) docker     (123)    35119 2023-06-26 15:21:20.000000 power-grid-model-1.5.0rc9190704883749/tests/data/power_flow/vision-validation-network/vision_validation_network.vnf
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-06-26 15:21:20.000000 power-grid-model-1.5.0rc9190704883749/tests/data/power_flow/vision-validation-network/vision_validation_network.vnf.license
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 15:22:14.372742 power-grid-model-1.5.0rc9190704883749/tests/data/short_circuit/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 15:22:14.432744 power-grid-model-1.5.0rc9190704883749/tests/data/short_circuit/single_phase_to_ground_a/
+-rw-r--r--   0 runner    (1001) docker     (123)    60746 2023-06-26 15:21:20.000000 power-grid-model-1.5.0rc9190704883749/tests/data/short_circuit/single_phase_to_ground_a/asym_sc_output_batch.json
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-06-26 15:21:20.000000 power-grid-model-1.5.0rc9190704883749/tests/data/short_circuit/single_phase_to_ground_a/asym_sc_output_batch.json.license
+-rw-r--r--   0 runner    (1001) docker     (123)     1248 2023-06-26 15:21:20.000000 power-grid-model-1.5.0rc9190704883749/tests/data/short_circuit/single_phase_to_ground_a/input.json
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-06-26 15:21:20.000000 power-grid-model-1.5.0rc9190704883749/tests/data/short_circuit/single_phase_to_ground_a/input.json.license
+-rw-r--r--   0 runner    (1001) docker     (123)      141 2023-06-26 15:21:20.000000 power-grid-model-1.5.0rc9190704883749/tests/data/short_circuit/single_phase_to_ground_a/params.json
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-06-26 15:21:20.000000 power-grid-model-1.5.0rc9190704883749/tests/data/short_circuit/single_phase_to_ground_a/params.json.license
+-rw-r--r--   0 runner    (1001) docker     (123)     5042 2023-06-26 15:21:20.000000 power-grid-model-1.5.0rc9190704883749/tests/data/short_circuit/single_phase_to_ground_a/update_batch.json
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-06-26 15:21:20.000000 power-grid-model-1.5.0rc9190704883749/tests/data/short_circuit/single_phase_to_ground_a/update_batch.json.license
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 15:22:14.436744 power-grid-model-1.5.0rc9190704883749/tests/data/short_circuit/single_phase_to_ground_b/
+-rw-r--r--   0 runner    (1001) docker     (123)    60938 2023-06-26 15:21:20.000000 power-grid-model-1.5.0rc9190704883749/tests/data/short_circuit/single_phase_to_ground_b/asym_sc_output_batch.json
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-06-26 15:21:20.000000 power-grid-model-1.5.0rc9190704883749/tests/data/short_circuit/single_phase_to_ground_b/asym_sc_output_batch.json.license
+-rw-r--r--   0 runner    (1001) docker     (123)     1248 2023-06-26 15:21:20.000000 power-grid-model-1.5.0rc9190704883749/tests/data/short_circuit/single_phase_to_ground_b/input.json
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-06-26 15:21:20.000000 power-grid-model-1.5.0rc9190704883749/tests/data/short_circuit/single_phase_to_ground_b/input.json.license
+-rw-r--r--   0 runner    (1001) docker     (123)      141 2023-06-26 15:21:20.000000 power-grid-model-1.5.0rc9190704883749/tests/data/short_circuit/single_phase_to_ground_b/params.json
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-06-26 15:21:20.000000 power-grid-model-1.5.0rc9190704883749/tests/data/short_circuit/single_phase_to_ground_b/params.json.license
+-rw-r--r--   0 runner    (1001) docker     (123)     5042 2023-06-26 15:21:20.000000 power-grid-model-1.5.0rc9190704883749/tests/data/short_circuit/single_phase_to_ground_b/update_batch.json
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-06-26 15:21:20.000000 power-grid-model-1.5.0rc9190704883749/tests/data/short_circuit/single_phase_to_ground_b/update_batch.json.license
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 15:22:14.436744 power-grid-model-1.5.0rc9190704883749/tests/data/short_circuit/single_phase_to_ground_c/
+-rw-r--r--   0 runner    (1001) docker     (123)    60902 2023-06-26 15:21:20.000000 power-grid-model-1.5.0rc9190704883749/tests/data/short_circuit/single_phase_to_ground_c/asym_sc_output_batch.json
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-06-26 15:21:20.000000 power-grid-model-1.5.0rc9190704883749/tests/data/short_circuit/single_phase_to_ground_c/asym_sc_output_batch.json.license
+-rw-r--r--   0 runner    (1001) docker     (123)     1248 2023-06-26 15:21:20.000000 power-grid-model-1.5.0rc9190704883749/tests/data/short_circuit/single_phase_to_ground_c/input.json
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-06-26 15:21:20.000000 power-grid-model-1.5.0rc9190704883749/tests/data/short_circuit/single_phase_to_ground_c/input.json.license
+-rw-r--r--   0 runner    (1001) docker     (123)      141 2023-06-26 15:21:20.000000 power-grid-model-1.5.0rc9190704883749/tests/data/short_circuit/single_phase_to_ground_c/params.json
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-06-26 15:21:20.000000 power-grid-model-1.5.0rc9190704883749/tests/data/short_circuit/single_phase_to_ground_c/params.json.license
+-rw-r--r--   0 runner    (1001) docker     (123)     5042 2023-06-26 15:21:20.000000 power-grid-model-1.5.0rc9190704883749/tests/data/short_circuit/single_phase_to_ground_c/update_batch.json
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-06-26 15:21:20.000000 power-grid-model-1.5.0rc9190704883749/tests/data/short_circuit/single_phase_to_ground_c/update_batch.json.license
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 15:22:14.436744 power-grid-model-1.5.0rc9190704883749/tests/data/short_circuit/three_phase/
+-rw-r--r--   0 runner    (1001) docker     (123)     1248 2023-06-26 15:21:20.000000 power-grid-model-1.5.0rc9190704883749/tests/data/short_circuit/three_phase/input.json
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-06-26 15:21:20.000000 power-grid-model-1.5.0rc9190704883749/tests/data/short_circuit/three_phase/input.json.license
+-rw-r--r--   0 runner    (1001) docker     (123)      132 2023-06-26 15:21:20.000000 power-grid-model-1.5.0rc9190704883749/tests/data/short_circuit/three_phase/params.json
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-06-26 15:21:20.000000 power-grid-model-1.5.0rc9190704883749/tests/data/short_circuit/three_phase/params.json.license
+-rw-r--r--   0 runner    (1001) docker     (123)    28484 2023-06-26 15:21:20.000000 power-grid-model-1.5.0rc9190704883749/tests/data/short_circuit/three_phase/sym_sc_output_batch.json
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-06-26 15:21:20.000000 power-grid-model-1.5.0rc9190704883749/tests/data/short_circuit/three_phase/sym_sc_output_batch.json.license
+-rw-r--r--   0 runner    (1001) docker     (123)     5042 2023-06-26 15:21:20.000000 power-grid-model-1.5.0rc9190704883749/tests/data/short_circuit/three_phase/update_batch.json
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-06-26 15:21:20.000000 power-grid-model-1.5.0rc9190704883749/tests/data/short_circuit/three_phase/update_batch.json.license
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 15:22:14.436744 power-grid-model-1.5.0rc9190704883749/tests/data/short_circuit/two_phase_ab/
+-rw-r--r--   0 runner    (1001) docker     (123)    59648 2023-06-26 15:21:20.000000 power-grid-model-1.5.0rc9190704883749/tests/data/short_circuit/two_phase_ab/asym_sc_output_batch.json
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-06-26 15:21:20.000000 power-grid-model-1.5.0rc9190704883749/tests/data/short_circuit/two_phase_ab/asym_sc_output_batch.json.license
+-rw-r--r--   0 runner    (1001) docker     (123)     1248 2023-06-26 15:21:20.000000 power-grid-model-1.5.0rc9190704883749/tests/data/short_circuit/two_phase_ab/input.json
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-06-26 15:21:20.000000 power-grid-model-1.5.0rc9190704883749/tests/data/short_circuit/two_phase_ab/input.json.license
+-rw-r--r--   0 runner    (1001) docker     (123)      129 2023-06-26 15:21:20.000000 power-grid-model-1.5.0rc9190704883749/tests/data/short_circuit/two_phase_ab/params.json
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-06-26 15:21:20.000000 power-grid-model-1.5.0rc9190704883749/tests/data/short_circuit/two_phase_ab/params.json.license
+-rw-r--r--   0 runner    (1001) docker     (123)     5042 2023-06-26 15:21:20.000000 power-grid-model-1.5.0rc9190704883749/tests/data/short_circuit/two_phase_ab/update_batch.json
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-06-26 15:21:20.000000 power-grid-model-1.5.0rc9190704883749/tests/data/short_circuit/two_phase_ab/update_batch.json.license
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 15:22:14.440744 power-grid-model-1.5.0rc9190704883749/tests/data/short_circuit/two_phase_ac/
+-rw-r--r--   0 runner    (1001) docker     (123)    58856 2023-06-26 15:21:20.000000 power-grid-model-1.5.0rc9190704883749/tests/data/short_circuit/two_phase_ac/asym_sc_output_batch.json
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-06-26 15:21:20.000000 power-grid-model-1.5.0rc9190704883749/tests/data/short_circuit/two_phase_ac/asym_sc_output_batch.json.license
+-rw-r--r--   0 runner    (1001) docker     (123)     1248 2023-06-26 15:21:20.000000 power-grid-model-1.5.0rc9190704883749/tests/data/short_circuit/two_phase_ac/input.json
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-06-26 15:21:20.000000 power-grid-model-1.5.0rc9190704883749/tests/data/short_circuit/two_phase_ac/input.json.license
+-rw-r--r--   0 runner    (1001) docker     (123)      129 2023-06-26 15:21:20.000000 power-grid-model-1.5.0rc9190704883749/tests/data/short_circuit/two_phase_ac/params.json
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-06-26 15:21:20.000000 power-grid-model-1.5.0rc9190704883749/tests/data/short_circuit/two_phase_ac/params.json.license
+-rw-r--r--   0 runner    (1001) docker     (123)     5042 2023-06-26 15:21:20.000000 power-grid-model-1.5.0rc9190704883749/tests/data/short_circuit/two_phase_ac/update_batch.json
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-06-26 15:21:20.000000 power-grid-model-1.5.0rc9190704883749/tests/data/short_circuit/two_phase_ac/update_batch.json.license
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 15:22:14.440744 power-grid-model-1.5.0rc9190704883749/tests/data/short_circuit/two_phase_bc/
+-rw-r--r--   0 runner    (1001) docker     (123)    58682 2023-06-26 15:21:20.000000 power-grid-model-1.5.0rc9190704883749/tests/data/short_circuit/two_phase_bc/asym_sc_output_batch.json
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-06-26 15:21:20.000000 power-grid-model-1.5.0rc9190704883749/tests/data/short_circuit/two_phase_bc/asym_sc_output_batch.json.license
+-rw-r--r--   0 runner    (1001) docker     (123)     1248 2023-06-26 15:21:20.000000 power-grid-model-1.5.0rc9190704883749/tests/data/short_circuit/two_phase_bc/input.json
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-06-26 15:21:20.000000 power-grid-model-1.5.0rc9190704883749/tests/data/short_circuit/two_phase_bc/input.json.license
+-rw-r--r--   0 runner    (1001) docker     (123)      129 2023-06-26 15:21:20.000000 power-grid-model-1.5.0rc9190704883749/tests/data/short_circuit/two_phase_bc/params.json
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-06-26 15:21:20.000000 power-grid-model-1.5.0rc9190704883749/tests/data/short_circuit/two_phase_bc/params.json.license
+-rw-r--r--   0 runner    (1001) docker     (123)     5042 2023-06-26 15:21:20.000000 power-grid-model-1.5.0rc9190704883749/tests/data/short_circuit/two_phase_bc/update_batch.json
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-06-26 15:21:20.000000 power-grid-model-1.5.0rc9190704883749/tests/data/short_circuit/two_phase_bc/update_batch.json.license
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 15:22:14.440744 power-grid-model-1.5.0rc9190704883749/tests/data/short_circuit/two_phase_to_ground_ab/
+-rw-r--r--   0 runner    (1001) docker     (123)    60884 2023-06-26 15:21:20.000000 power-grid-model-1.5.0rc9190704883749/tests/data/short_circuit/two_phase_to_ground_ab/asym_sc_output_batch.json
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-06-26 15:21:20.000000 power-grid-model-1.5.0rc9190704883749/tests/data/short_circuit/two_phase_to_ground_ab/asym_sc_output_batch.json.license
+-rw-r--r--   0 runner    (1001) docker     (123)     1248 2023-06-26 15:21:20.000000 power-grid-model-1.5.0rc9190704883749/tests/data/short_circuit/two_phase_to_ground_ab/input.json
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-06-26 15:21:20.000000 power-grid-model-1.5.0rc9190704883749/tests/data/short_circuit/two_phase_to_ground_ab/input.json.license
+-rw-r--r--   0 runner    (1001) docker     (123)      139 2023-06-26 15:21:20.000000 power-grid-model-1.5.0rc9190704883749/tests/data/short_circuit/two_phase_to_ground_ab/params.json
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-06-26 15:21:20.000000 power-grid-model-1.5.0rc9190704883749/tests/data/short_circuit/two_phase_to_ground_ab/params.json.license
+-rw-r--r--   0 runner    (1001) docker     (123)     5042 2023-06-26 15:21:20.000000 power-grid-model-1.5.0rc9190704883749/tests/data/short_circuit/two_phase_to_ground_ab/update_batch.json
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-06-26 15:21:20.000000 power-grid-model-1.5.0rc9190704883749/tests/data/short_circuit/two_phase_to_ground_ab/update_batch.json.license
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 15:22:14.440744 power-grid-model-1.5.0rc9190704883749/tests/data/short_circuit/two_phase_to_ground_ac/
+-rw-r--r--   0 runner    (1001) docker     (123)    60740 2023-06-26 15:21:20.000000 power-grid-model-1.5.0rc9190704883749/tests/data/short_circuit/two_phase_to_ground_ac/asym_sc_output_batch.json
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-06-26 15:21:20.000000 power-grid-model-1.5.0rc9190704883749/tests/data/short_circuit/two_phase_to_ground_ac/asym_sc_output_batch.json.license
+-rw-r--r--   0 runner    (1001) docker     (123)     1248 2023-06-26 15:21:20.000000 power-grid-model-1.5.0rc9190704883749/tests/data/short_circuit/two_phase_to_ground_ac/input.json
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-06-26 15:21:20.000000 power-grid-model-1.5.0rc9190704883749/tests/data/short_circuit/two_phase_to_ground_ac/input.json.license
+-rw-r--r--   0 runner    (1001) docker     (123)      139 2023-06-26 15:21:20.000000 power-grid-model-1.5.0rc9190704883749/tests/data/short_circuit/two_phase_to_ground_ac/params.json
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-06-26 15:21:20.000000 power-grid-model-1.5.0rc9190704883749/tests/data/short_circuit/two_phase_to_ground_ac/params.json.license
+-rw-r--r--   0 runner    (1001) docker     (123)     5042 2023-06-26 15:21:20.000000 power-grid-model-1.5.0rc9190704883749/tests/data/short_circuit/two_phase_to_ground_ac/update_batch.json
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-06-26 15:21:20.000000 power-grid-model-1.5.0rc9190704883749/tests/data/short_circuit/two_phase_to_ground_ac/update_batch.json.license
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 15:22:14.448744 power-grid-model-1.5.0rc9190704883749/tests/data/short_circuit/two_phase_to_ground_bc/
+-rw-r--r--   0 runner    (1001) docker     (123)    60629 2023-06-26 15:21:20.000000 power-grid-model-1.5.0rc9190704883749/tests/data/short_circuit/two_phase_to_ground_bc/asym_sc_output_batch.json
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-06-26 15:21:20.000000 power-grid-model-1.5.0rc9190704883749/tests/data/short_circuit/two_phase_to_ground_bc/asym_sc_output_batch.json.license
+-rw-r--r--   0 runner    (1001) docker     (123)     1248 2023-06-26 15:21:20.000000 power-grid-model-1.5.0rc9190704883749/tests/data/short_circuit/two_phase_to_ground_bc/input.json
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-06-26 15:21:20.000000 power-grid-model-1.5.0rc9190704883749/tests/data/short_circuit/two_phase_to_ground_bc/input.json.license
+-rw-r--r--   0 runner    (1001) docker     (123)      139 2023-06-26 15:21:20.000000 power-grid-model-1.5.0rc9190704883749/tests/data/short_circuit/two_phase_to_ground_bc/params.json
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-06-26 15:21:20.000000 power-grid-model-1.5.0rc9190704883749/tests/data/short_circuit/two_phase_to_ground_bc/params.json.license
+-rw-r--r--   0 runner    (1001) docker     (123)     5042 2023-06-26 15:21:20.000000 power-grid-model-1.5.0rc9190704883749/tests/data/short_circuit/two_phase_to_ground_bc/update_batch.json
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-06-26 15:21:20.000000 power-grid-model-1.5.0rc9190704883749/tests/data/short_circuit/two_phase_to_ground_bc/update_batch.json.license
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 15:22:14.376742 power-grid-model-1.5.0rc9190704883749/tests/data/state_estimation/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 15:22:14.448744 power-grid-model-1.5.0rc9190704883749/tests/data/state_estimation/1os2msr/
+-rw-r--r--   0 runner    (1001) docker     (123)     2910 2023-06-26 15:21:20.000000 power-grid-model-1.5.0rc9190704883749/tests/data/state_estimation/1os2msr/input.json
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-06-26 15:21:20.000000 power-grid-model-1.5.0rc9190704883749/tests/data/state_estimation/1os2msr/input.json.license
+-rw-r--r--   0 runner    (1001) docker     (123)      124 2023-06-26 15:21:20.000000 power-grid-model-1.5.0rc9190704883749/tests/data/state_estimation/1os2msr/params.json
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-06-26 15:21:20.000000 power-grid-model-1.5.0rc9190704883749/tests/data/state_estimation/1os2msr/params.json.license
+-rw-r--r--   0 runner    (1001) docker     (123)     2731 2023-06-26 15:21:20.000000 power-grid-model-1.5.0rc9190704883749/tests/data/state_estimation/1os2msr/sym_output.json
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-06-26 15:21:20.000000 power-grid-model-1.5.0rc9190704883749/tests/data/state_estimation/1os2msr/sym_output.json.license
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 15:22:14.448744 power-grid-model-1.5.0rc9190704883749/tests/data/state_estimation/1os2msr-no-angle/
+-rw-r--r--   0 runner    (1001) docker     (123)     2786 2023-06-26 15:21:20.000000 power-grid-model-1.5.0rc9190704883749/tests/data/state_estimation/1os2msr-no-angle/input.json
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-06-26 15:21:20.000000 power-grid-model-1.5.0rc9190704883749/tests/data/state_estimation/1os2msr-no-angle/input.json.license
+-rw-r--r--   0 runner    (1001) docker     (123)       78 2023-06-26 15:21:20.000000 power-grid-model-1.5.0rc9190704883749/tests/data/state_estimation/1os2msr-no-angle/params.json
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-06-26 15:21:20.000000 power-grid-model-1.5.0rc9190704883749/tests/data/state_estimation/1os2msr-no-angle/params.json.license
+-rw-r--r--   0 runner    (1001) docker     (123)     1836 2023-06-26 15:21:20.000000 power-grid-model-1.5.0rc9190704883749/tests/data/state_estimation/1os2msr-no-angle/sym_output.json
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-06-26 15:21:20.000000 power-grid-model-1.5.0rc9190704883749/tests/data/state_estimation/1os2msr-no-angle/sym_output.json.license
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 15:22:14.448744 power-grid-model-1.5.0rc9190704883749/tests/data/state_estimation/distribution-case/
+-rw-r--r--   0 runner    (1001) docker     (123)     1395 2023-06-26 15:21:20.000000 power-grid-model-1.5.0rc9190704883749/tests/data/state_estimation/distribution-case/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)     8939 2023-06-26 15:21:20.000000 power-grid-model-1.5.0rc9190704883749/tests/data/state_estimation/distribution-case/input.json
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-06-26 15:21:20.000000 power-grid-model-1.5.0rc9190704883749/tests/data/state_estimation/distribution-case/input.json.license
+-rw-r--r--   0 runner    (1001) docker     (123)      123 2023-06-26 15:21:20.000000 power-grid-model-1.5.0rc9190704883749/tests/data/state_estimation/distribution-case/params.json
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-06-26 15:21:20.000000 power-grid-model-1.5.0rc9190704883749/tests/data/state_estimation/distribution-case/params.json.license
+-rw-r--r--   0 runner    (1001) docker     (123)    19468 2023-06-26 15:21:20.000000 power-grid-model-1.5.0rc9190704883749/tests/data/state_estimation/distribution-case/sym_output_batch.json
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-06-26 15:21:20.000000 power-grid-model-1.5.0rc9190704883749/tests/data/state_estimation/distribution-case/sym_output_batch.json.license
+-rw-r--r--   0 runner    (1001) docker     (123)     6642 2023-06-26 15:21:20.000000 power-grid-model-1.5.0rc9190704883749/tests/data/state_estimation/distribution-case/update_batch.json
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-06-26 15:21:20.000000 power-grid-model-1.5.0rc9190704883749/tests/data/state_estimation/distribution-case/update_batch.json.license
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 15:22:14.448744 power-grid-model-1.5.0rc9190704883749/tests/data/state_estimation/dummy-test-sym/
+-rw-r--r--   0 runner    (1001) docker     (123)     3196 2023-06-26 15:21:20.000000 power-grid-model-1.5.0rc9190704883749/tests/data/state_estimation/dummy-test-sym/input.json
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-06-26 15:21:20.000000 power-grid-model-1.5.0rc9190704883749/tests/data/state_estimation/dummy-test-sym/input.json.license
+-rw-r--r--   0 runner    (1001) docker     (123)      116 2023-06-26 15:21:20.000000 power-grid-model-1.5.0rc9190704883749/tests/data/state_estimation/dummy-test-sym/params.json
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-06-26 15:21:20.000000 power-grid-model-1.5.0rc9190704883749/tests/data/state_estimation/dummy-test-sym/params.json.license
+-rw-r--r--   0 runner    (1001) docker     (123)     2174 2023-06-26 15:21:20.000000 power-grid-model-1.5.0rc9190704883749/tests/data/state_estimation/dummy-test-sym/sym_output.json
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-06-26 15:21:20.000000 power-grid-model-1.5.0rc9190704883749/tests/data/state_estimation/dummy-test-sym/sym_output.json.license
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 15:22:14.452745 power-grid-model-1.5.0rc9190704883749/tests/data/state_estimation/node-injection-sensor-and-zero-injection/
+-rw-r--r--   0 runner    (1001) docker     (123)      780 2023-06-26 15:21:20.000000 power-grid-model-1.5.0rc9190704883749/tests/data/state_estimation/node-injection-sensor-and-zero-injection/input.json
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-06-26 15:21:20.000000 power-grid-model-1.5.0rc9190704883749/tests/data/state_estimation/node-injection-sensor-and-zero-injection/input.json.license
+-rw-r--r--   0 runner    (1001) docker     (123)       78 2023-06-26 15:21:20.000000 power-grid-model-1.5.0rc9190704883749/tests/data/state_estimation/node-injection-sensor-and-zero-injection/params.json
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-06-26 15:21:20.000000 power-grid-model-1.5.0rc9190704883749/tests/data/state_estimation/node-injection-sensor-and-zero-injection/params.json.license
+-rw-r--r--   0 runner    (1001) docker     (123)      824 2023-06-26 15:21:20.000000 power-grid-model-1.5.0rc9190704883749/tests/data/state_estimation/node-injection-sensor-and-zero-injection/sym_output.json
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-06-26 15:21:20.000000 power-grid-model-1.5.0rc9190704883749/tests/data/state_estimation/node-injection-sensor-and-zero-injection/sym_output.json.license
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 15:22:14.452745 power-grid-model-1.5.0rc9190704883749/tests/data/state_estimation/residual-test/
+-rw-r--r--   0 runner    (1001) docker     (123)      448 2023-06-26 15:21:20.000000 power-grid-model-1.5.0rc9190704883749/tests/data/state_estimation/residual-test/input.json
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-06-26 15:21:20.000000 power-grid-model-1.5.0rc9190704883749/tests/data/state_estimation/residual-test/input.json.license
+-rw-r--r--   0 runner    (1001) docker     (123)      124 2023-06-26 15:21:20.000000 power-grid-model-1.5.0rc9190704883749/tests/data/state_estimation/residual-test/params.json
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-06-26 15:21:20.000000 power-grid-model-1.5.0rc9190704883749/tests/data/state_estimation/residual-test/params.json.license
+-rw-r--r--   0 runner    (1001) docker     (123)      374 2023-06-26 15:21:20.000000 power-grid-model-1.5.0rc9190704883749/tests/data/state_estimation/residual-test/sym_output.json
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-06-26 15:21:20.000000 power-grid-model-1.5.0rc9190704883749/tests/data/state_estimation/residual-test/sym_output.json.license
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 15:22:14.452745 power-grid-model-1.5.0rc9190704883749/tests/data/state_estimation/single-line-load/
+-rw-r--r--   0 runner    (1001) docker     (123)     1057 2023-06-26 15:21:20.000000 power-grid-model-1.5.0rc9190704883749/tests/data/state_estimation/single-line-load/input.json
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-06-26 15:21:20.000000 power-grid-model-1.5.0rc9190704883749/tests/data/state_estimation/single-line-load/input.json.license
+-rw-r--r--   0 runner    (1001) docker     (123)       78 2023-06-26 15:21:20.000000 power-grid-model-1.5.0rc9190704883749/tests/data/state_estimation/single-line-load/params.json
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-06-26 15:21:20.000000 power-grid-model-1.5.0rc9190704883749/tests/data/state_estimation/single-line-load/params.json.license
+-rw-r--r--   0 runner    (1001) docker     (123)      529 2023-06-26 15:21:20.000000 power-grid-model-1.5.0rc9190704883749/tests/data/state_estimation/single-line-load/sym_output.json
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-06-26 15:21:20.000000 power-grid-model-1.5.0rc9190704883749/tests/data/state_estimation/single-line-load/sym_output.json.license
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 15:22:14.452745 power-grid-model-1.5.0rc9190704883749/tests/data/state_estimation/three_winding_transformer/
+-rw-r--r--   0 runner    (1001) docker     (123)     2166 2023-06-26 15:21:20.000000 power-grid-model-1.5.0rc9190704883749/tests/data/state_estimation/three_winding_transformer/input.json
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-06-26 15:21:20.000000 power-grid-model-1.5.0rc9190704883749/tests/data/state_estimation/three_winding_transformer/input.json.license
+-rw-r--r--   0 runner    (1001) docker     (123)       78 2023-06-26 15:21:20.000000 power-grid-model-1.5.0rc9190704883749/tests/data/state_estimation/three_winding_transformer/params.json
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-06-26 15:21:20.000000 power-grid-model-1.5.0rc9190704883749/tests/data/state_estimation/three_winding_transformer/params.json.license
+-rw-r--r--   0 runner    (1001) docker     (123)      868 2023-06-26 15:21:20.000000 power-grid-model-1.5.0rc9190704883749/tests/data/state_estimation/three_winding_transformer/sym_output.json
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-06-26 15:21:20.000000 power-grid-model-1.5.0rc9190704883749/tests/data/state_estimation/three_winding_transformer/sym_output.json.license
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 15:22:14.452745 power-grid-model-1.5.0rc9190704883749/tests/data/state_estimation/transmission-case/
+-rw-r--r--   0 runner    (1001) docker     (123)     1196 2023-06-26 15:21:20.000000 power-grid-model-1.5.0rc9190704883749/tests/data/state_estimation/transmission-case/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)    29158 2023-06-26 15:21:20.000000 power-grid-model-1.5.0rc9190704883749/tests/data/state_estimation/transmission-case/asym_output.json
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-06-26 15:21:20.000000 power-grid-model-1.5.0rc9190704883749/tests/data/state_estimation/transmission-case/asym_output.json.license
+-rw-r--r--   0 runner    (1001) docker     (123)    11996 2023-06-26 15:21:20.000000 power-grid-model-1.5.0rc9190704883749/tests/data/state_estimation/transmission-case/input.json
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-06-26 15:21:20.000000 power-grid-model-1.5.0rc9190704883749/tests/data/state_estimation/transmission-case/input.json.license
+-rw-r--r--   0 runner    (1001) docker     (123)      125 2023-06-26 15:21:20.000000 power-grid-model-1.5.0rc9190704883749/tests/data/state_estimation/transmission-case/params.json
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-06-26 15:21:20.000000 power-grid-model-1.5.0rc9190704883749/tests/data/state_estimation/transmission-case/params.json.license
+-rw-r--r--   0 runner    (1001) docker     (123)     7827 2023-06-26 15:21:20.000000 power-grid-model-1.5.0rc9190704883749/tests/data/state_estimation/transmission-case/sym_output.json
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-06-26 15:21:20.000000 power-grid-model-1.5.0rc9190704883749/tests/data/state_estimation/transmission-case/sym_output.json.license
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 15:22:14.456745 power-grid-model-1.5.0rc9190704883749/tests/unit/
+-rw-r--r--   0 runner    (1001) docker     (123)      154 2023-06-26 15:21:20.000000 power-grid-model-1.5.0rc9190704883749/tests/unit/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4005 2023-06-26 15:21:20.000000 power-grid-model-1.5.0rc9190704883749/tests/unit/test_0Z_model_validation.py
+-rw-r--r--   0 runner    (1001) docker     (123)      794 2023-06-26 15:21:20.000000 power-grid-model-1.5.0rc9190704883749/tests/unit/test_error_handling.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2225 2023-06-26 15:21:20.000000 power-grid-model-1.5.0rc9190704883749/tests/unit/test_meta_data.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6422 2023-06-26 15:21:20.000000 power-grid-model-1.5.0rc9190704883749/tests/unit/test_power_grid_model.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20807 2023-06-26 15:21:20.000000 power-grid-model-1.5.0rc9190704883749/tests/unit/test_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7996 2023-06-26 15:21:20.000000 power-grid-model-1.5.0rc9190704883749/tests/unit/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 15:22:14.456745 power-grid-model-1.5.0rc9190704883749/tests/unit/validation/
+-rw-r--r--   0 runner    (1001) docker     (123)      154 2023-06-26 15:21:20.000000 power-grid-model-1.5.0rc9190704883749/tests/unit/validation/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2330 2023-06-26 15:21:20.000000 power-grid-model-1.5.0rc9190704883749/tests/unit/validation/test_assertions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2886 2023-06-26 15:21:20.000000 power-grid-model-1.5.0rc9190704883749/tests/unit/validation/test_batch_validation.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4855 2023-06-26 15:21:20.000000 power-grid-model-1.5.0rc9190704883749/tests/unit/validation/test_errors.py
+-rw-r--r--   0 runner    (1001) docker     (123)    27362 2023-06-26 15:21:20.000000 power-grid-model-1.5.0rc9190704883749/tests/unit/validation/test_input_validation.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14325 2023-06-26 15:21:20.000000 power-grid-model-1.5.0rc9190704883749/tests/unit/validation/test_rules.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6991 2023-06-26 15:21:20.000000 power-grid-model-1.5.0rc9190704883749/tests/unit/validation/test_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)    23023 2023-06-26 15:21:20.000000 power-grid-model-1.5.0rc9190704883749/tests/unit/validation/test_validation_functions.py
```

### Comparing `power-grid-model-1.5.0rc9190015282548/LICENSE` & `power-grid-model-1.5.0rc9190704883749/LICENSE`

 * *Files identical despite different names*

### Comparing `power-grid-model-1.5.0rc9190015282548/PKG-INFO` & `power-grid-model-1.5.0rc9190704883749/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: power-grid-model
-Version: 1.5.0rc9190015282548
+Version: 1.5.0rc9190704883749
 Summary: Python/C++ library for distribution power system analysis
 Author-email: Alliander Dynamic Grid Calculation <dynamic.grid.calculation@alliander.com>
 License: MPL-2.0
 Project-URL: Home-page, https://lfenergy.org/projects/power-grid-model/
 Project-URL: GitHub, https://github.com/PowerGridModel/power-grid-model
 Project-URL: Documentation, https://power-grid-model.readthedocs.io/en/stable/
 Project-URL: Mailing-list, https://lists.lfenergy.org/g/powergridmodel
```

### Comparing `power-grid-model-1.5.0rc9190015282548/README.md` & `power-grid-model-1.5.0rc9190704883749/README.md`

 * *Files identical despite different names*

### Comparing `power-grid-model-1.5.0rc9190015282548/power_grid_model_c/power_grid_model/CMakeLists.txt` & `power-grid-model-1.5.0rc9190704883749/power_grid_model_c/power_grid_model/CMakeLists.txt`

 * *Files identical despite different names*

### Comparing `power-grid-model-1.5.0rc9190015282548/power_grid_model_c/power_grid_model/include/power_grid_model/all_components.hpp` & `power-grid-model-1.5.0rc9190704883749/power_grid_model_c/power_grid_model/include/power_grid_model/all_components.hpp`

 * *Files identical despite different names*

### Comparing `power-grid-model-1.5.0rc9190015282548/power_grid_model_c/power_grid_model/include/power_grid_model/auxiliary/dataset.hpp` & `power-grid-model-1.5.0rc9190704883749/power_grid_model_c/power_grid_model/include/power_grid_model/auxiliary/dataset.hpp`

 * *Files identical despite different names*

### Comparing `power-grid-model-1.5.0rc9190015282548/power_grid_model_c/power_grid_model/include/power_grid_model/auxiliary/input.hpp` & `power-grid-model-1.5.0rc9190704883749/power_grid_model_c/power_grid_model/include/power_grid_model/auxiliary/input.hpp`

 * *Files identical despite different names*

### Comparing `power-grid-model-1.5.0rc9190015282548/power_grid_model_c/power_grid_model/include/power_grid_model/auxiliary/meta_data.hpp` & `power-grid-model-1.5.0rc9190704883749/power_grid_model_c/power_grid_model/include/power_grid_model/auxiliary/meta_data.hpp`

 * *Files identical despite different names*

### Comparing `power-grid-model-1.5.0rc9190015282548/power_grid_model_c/power_grid_model/include/power_grid_model/auxiliary/meta_data_gen.hpp` & `power-grid-model-1.5.0rc9190704883749/power_grid_model_c/power_grid_model/include/power_grid_model/auxiliary/meta_data_gen.hpp`

 * *Files identical despite different names*

### Comparing `power-grid-model-1.5.0rc9190015282548/power_grid_model_c/power_grid_model/include/power_grid_model/auxiliary/output.hpp` & `power-grid-model-1.5.0rc9190704883749/power_grid_model_c/power_grid_model/include/power_grid_model/auxiliary/output.hpp`

 * *Files identical despite different names*

### Comparing `power-grid-model-1.5.0rc9190015282548/power_grid_model_c/power_grid_model/include/power_grid_model/auxiliary/update.hpp` & `power-grid-model-1.5.0rc9190704883749/power_grid_model_c/power_grid_model/include/power_grid_model/auxiliary/update.hpp`

 * *Files identical despite different names*

### Comparing `power-grid-model-1.5.0rc9190015282548/power_grid_model_c/power_grid_model/include/power_grid_model/calculation_parameters.hpp` & `power-grid-model-1.5.0rc9190704883749/power_grid_model_c/power_grid_model/include/power_grid_model/calculation_parameters.hpp`

 * *Files 2% similar despite different names*

```diff
@@ -256,14 +256,16 @@
 // sequence numbers of 3 virtual branches are saved in pos
 struct Idx2DBranch3 {
     Idx group;
     // 0: node 0 -> internal node
     // 1: node 1 -> internal node
     // 2: node 2 -> internal node
     std::array<Idx, 3> pos;
+
+    friend constexpr bool operator==(Idx2DBranch3 const& x, Idx2DBranch3 const& y) = default;
 };
 
 // couple component to math model
 // use Idx2D to map component to math model
 //		group = math model sequence number,
 //		group = -1 means isolated component
 //		pos = sequence number in math model,
```

### Comparing `power-grid-model-1.5.0rc9190015282548/power_grid_model_c/power_grid_model/include/power_grid_model/component/appliance.hpp` & `power-grid-model-1.5.0rc9190704883749/power_grid_model_c/power_grid_model/include/power_grid_model/component/appliance.hpp`

 * *Files identical despite different names*

### Comparing `power-grid-model-1.5.0rc9190015282548/power_grid_model_c/power_grid_model/include/power_grid_model/component/base.hpp` & `power-grid-model-1.5.0rc9190704883749/power_grid_model_c/power_grid_model/include/power_grid_model/component/base.hpp`

 * *Files identical despite different names*

### Comparing `power-grid-model-1.5.0rc9190015282548/power_grid_model_c/power_grid_model/include/power_grid_model/component/branch.hpp` & `power-grid-model-1.5.0rc9190704883749/power_grid_model_c/power_grid_model/include/power_grid_model/component/branch.hpp`

 * *Files identical despite different names*

### Comparing `power-grid-model-1.5.0rc9190015282548/power_grid_model_c/power_grid_model/include/power_grid_model/component/branch3.hpp` & `power-grid-model-1.5.0rc9190704883749/power_grid_model_c/power_grid_model/include/power_grid_model/component/branch3.hpp`

 * *Files identical despite different names*

### Comparing `power-grid-model-1.5.0rc9190015282548/power_grid_model_c/power_grid_model/include/power_grid_model/component/fault.hpp` & `power-grid-model-1.5.0rc9190704883749/power_grid_model_c/power_grid_model/include/power_grid_model/component/fault.hpp`

 * *Files identical despite different names*

### Comparing `power-grid-model-1.5.0rc9190015282548/power_grid_model_c/power_grid_model/include/power_grid_model/component/line.hpp` & `power-grid-model-1.5.0rc9190704883749/power_grid_model_c/power_grid_model/include/power_grid_model/component/line.hpp`

 * *Files identical despite different names*

### Comparing `power-grid-model-1.5.0rc9190015282548/power_grid_model_c/power_grid_model/include/power_grid_model/component/link.hpp` & `power-grid-model-1.5.0rc9190704883749/power_grid_model_c/power_grid_model/include/power_grid_model/component/link.hpp`

 * *Files identical despite different names*

### Comparing `power-grid-model-1.5.0rc9190015282548/power_grid_model_c/power_grid_model/include/power_grid_model/component/load_gen.hpp` & `power-grid-model-1.5.0rc9190704883749/power_grid_model_c/power_grid_model/include/power_grid_model/component/load_gen.hpp`

 * *Files 1% similar despite different names*

```diff
@@ -125,21 +125,23 @@
     double injection_direction() const final {
         return direction_;
     }
 
     // scale load
     template <bool sym_calc>
     ComplexValue<sym_calc> scale_power(ComplexValue<sym_calc> u) const {
+        using enum LoadGenType;
+
         ComplexValue<sym_calc> const s = this->template calc_param<sym_calc>();
         switch (this->type()) {
-            case LoadGenType::const_pq:
+            case const_pq:
                 return s;
-            case LoadGenType::const_y:
+            case const_y:
                 return s * abs2(u);
-            case LoadGenType::const_i:
+            case const_i:
                 return s * cabs(u);
             default:
                 throw MissingCaseForEnumError(std::string(this->name) + " power scaling factor", this->type());
         }
     }
 };
```

### Comparing `power-grid-model-1.5.0rc9190015282548/power_grid_model_c/power_grid_model/include/power_grid_model/component/node.hpp` & `power-grid-model-1.5.0rc9190704883749/power_grid_model_c/power_grid_model/include/power_grid_model/component/node.hpp`

 * *Files identical despite different names*

### Comparing `power-grid-model-1.5.0rc9190015282548/power_grid_model_c/power_grid_model/include/power_grid_model/component/power_sensor.hpp` & `power-grid-model-1.5.0rc9190704883749/power_grid_model_c/power_grid_model/include/power_grid_model/component/power_sensor.hpp`

 * *Files identical despite different names*

### Comparing `power-grid-model-1.5.0rc9190015282548/power_grid_model_c/power_grid_model/include/power_grid_model/component/sensor.hpp` & `power-grid-model-1.5.0rc9190704883749/power_grid_model_c/power_grid_model/include/power_grid_model/component/sensor.hpp`

 * *Files identical despite different names*

### Comparing `power-grid-model-1.5.0rc9190015282548/power_grid_model_c/power_grid_model/include/power_grid_model/component/shunt.hpp` & `power-grid-model-1.5.0rc9190704883749/power_grid_model_c/power_grid_model/include/power_grid_model/component/shunt.hpp`

 * *Files identical despite different names*

### Comparing `power-grid-model-1.5.0rc9190015282548/power_grid_model_c/power_grid_model/include/power_grid_model/component/source.hpp` & `power-grid-model-1.5.0rc9190704883749/power_grid_model_c/power_grid_model/include/power_grid_model/component/source.hpp`

 * *Files identical despite different names*

### Comparing `power-grid-model-1.5.0rc9190015282548/power_grid_model_c/power_grid_model/include/power_grid_model/component/three_winding_transformer.hpp` & `power-grid-model-1.5.0rc9190704883749/power_grid_model_c/power_grid_model/include/power_grid_model/component/three_winding_transformer.hpp`

 * *Files 1% similar despite different names*

```diff
@@ -77,18 +77,20 @@
                                                                        : three_winding_transformer_input.pk_23_max},
           base_i_1_{base_power_3p / u1_rated / sqrt3},
           base_i_2_{base_power_3p / u2_rated / sqrt3},
           base_i_3_{base_power_3p / u3_rated / sqrt3},
           z_grounding_1_{three_winding_transformer_input.r_grounding_1, three_winding_transformer_input.x_grounding_1},
           z_grounding_2_{three_winding_transformer_input.r_grounding_2, three_winding_transformer_input.x_grounding_2},
           z_grounding_3_{three_winding_transformer_input.r_grounding_3, three_winding_transformer_input.x_grounding_3} {
+        using enum WindingType;
+
         // check clock number
-        bool const is_1_wye = winding_1_ == WindingType::wye || winding_1_ == WindingType::wye_n;
-        bool const is_2_wye = winding_2_ == WindingType::wye || winding_2_ == WindingType::wye_n;
-        bool const is_3_wye = winding_3_ == WindingType::wye || winding_3_ == WindingType::wye_n;
+        bool const is_1_wye = winding_1_ == wye || winding_1_ == wye_n;
+        bool const is_2_wye = winding_2_ == wye || winding_2_ == wye_n;
+        bool const is_3_wye = winding_3_ == wye || winding_3_ == wye_n;
 
         // check clock 12
         if (  // clock should be between 0 and 12
             clock_12_ < 0 || clock_12_ > 12 ||
             // even number is not possible if one side is wye winding and the other side is not wye winding.
             ((clock_12_ % 2) == 0 && (is_1_wye != is_2_wye)) ||
             // odd number is not possible, if both sides are wye winding or both sides are not wye winding.
```

### Comparing `power-grid-model-1.5.0rc9190015282548/power_grid_model_c/power_grid_model/include/power_grid_model/component/transformer.hpp` & `power-grid-model-1.5.0rc9190704883749/power_grid_model_c/power_grid_model/include/power_grid_model/component/transformer.hpp`

 * *Files 2% similar despite different names*

```diff
@@ -50,17 +50,19 @@
           base_i_from_{base_power_3p / u1_rated / sqrt3},
           base_i_to_{base_power_3p / u2_rated / sqrt3},
           nominal_ratio_{u1_rated / u2_rated},
           z_grounding_from_{
               calculate_z_pu(transformer_input.r_grounding_from, transformer_input.x_grounding_from, u1_rated)},
           z_grounding_to_{
               calculate_z_pu(transformer_input.r_grounding_to, transformer_input.x_grounding_to, u2_rated)} {
+        using enum WindingType;
+
         // check on clock
-        bool const is_from_wye = winding_from_ == WindingType::wye || winding_from_ == WindingType::wye_n;
-        bool const is_to_wye = winding_to_ == WindingType::wye || winding_to_ == WindingType::wye_n;
+        bool const is_from_wye = winding_from_ == wye || winding_from_ == wye_n;
+        bool const is_to_wye = winding_to_ == wye || winding_to_ == wye_n;
         if (  // clock should be between 0 and 12
             clock_ < 0 || clock_ > 12 ||
             // even number is not possible if one side is wye winding and the other side is not wye winding.
             ((clock_ % 2) == 0 && (is_from_wye != is_to_wye)) ||
             // odd number is not possible, if both sides are wye winding or both sides are not wye winding.
             ((clock_ % 2) == 1 && (is_from_wye == is_to_wye))) {
             throw InvalidTransformerClock{id(), clock_};
```

### Comparing `power-grid-model-1.5.0rc9190015282548/power_grid_model_c/power_grid_model/include/power_grid_model/component/transformer_utils.hpp` & `power-grid-model-1.5.0rc9190704883749/power_grid_model_c/power_grid_model/include/power_grid_model/component/transformer_utils.hpp`

 * *Files identical despite different names*

### Comparing `power-grid-model-1.5.0rc9190015282548/power_grid_model_c/power_grid_model/include/power_grid_model/component/voltage_sensor.hpp` & `power-grid-model-1.5.0rc9190704883749/power_grid_model_c/power_grid_model/include/power_grid_model/component/voltage_sensor.hpp`

 * *Files identical despite different names*

### Comparing `power-grid-model-1.5.0rc9190015282548/power_grid_model_c/power_grid_model/include/power_grid_model/container.hpp` & `power-grid-model-1.5.0rc9190704883749/power_grid_model_c/power_grid_model/include/power_grid_model/container.hpp`

 * *Files 0% similar despite different names*

```diff
@@ -71,15 +71,15 @@
 
     // emplace component
     template <class Storageable, class... Args>
     void emplace(ID id, Args&&... args) {
         // template<class... Args> Args&&... args perfect forwarding
         assert(!construction_complete_);
         // throw if id already exists
-        if (map_.find(id) != map_.end()) {
+        if (map_.contains(id)) {
             throw ConflictID{id};
         }
         // find group and position
         Idx const group = static_cast<Idx>(get_cls_pos_v<Storageable, StorageableTypes...>);
         std::vector<Storageable>& vec = std::get<std::vector<Storageable>>(vectors_);
         Idx const pos = static_cast<Idx>(vec.size());
         // create object
```

### Comparing `power-grid-model-1.5.0rc9190015282548/power_grid_model_c/power_grid_model/include/power_grid_model/enum.hpp` & `power-grid-model-1.5.0rc9190704883749/power_grid_model_c/power_grid_model/include/power_grid_model/enum.hpp`

 * *Files identical despite different names*

### Comparing `power-grid-model-1.5.0rc9190015282548/power_grid_model_c/power_grid_model/include/power_grid_model/exception.hpp` & `power-grid-model-1.5.0rc9190704883749/power_grid_model_c/power_grid_model/include/power_grid_model/exception.hpp`

 * *Files identical despite different names*

### Comparing `power-grid-model-1.5.0rc9190015282548/power_grid_model_c/power_grid_model/include/power_grid_model/main_model.hpp` & `power-grid-model-1.5.0rc9190704883749/power_grid_model_c/power_grid_model/include/power_grid_model/main_model.hpp`

 * *Files 3% similar despite different names*

```diff
@@ -181,36 +181,38 @@
                 if (components_.get_idx_by_id(input.measured_object).group ==
                     components_.template get_type_idx<Link>()) {
                     throw InvalidMeasuredObject("Link", "PowerSensor");
                 }
                 ID const measured_object = input.measured_object;
                 // check correctness of measured component type based on measured terminal type
                 switch (input.measured_terminal_type) {
-                    case MeasuredTerminalType::branch_from:
-                    case MeasuredTerminalType::branch_to:
+                    using enum MeasuredTerminalType;
+
+                    case branch_from:
+                    case branch_to:
                         components_.template get_item<Branch>(measured_object);
                         break;
-                    case MeasuredTerminalType::branch3_1:
-                    case MeasuredTerminalType::branch3_2:
-                    case MeasuredTerminalType::branch3_3:
+                    case branch3_1:
+                    case branch3_2:
+                    case branch3_3:
                         components_.template get_item<Branch3>(measured_object);
                         break;
-                    case MeasuredTerminalType::shunt:
+                    case shunt:
                         components_.template get_item<Shunt>(measured_object);
                         break;
-                    case MeasuredTerminalType::source:
+                    case source:
                         components_.template get_item<Source>(measured_object);
                         break;
-                    case MeasuredTerminalType::load:
+                    case load:
                         components_.template get_item<GenericLoad>(measured_object);
                         break;
-                    case MeasuredTerminalType::generator:
+                    case generator:
                         components_.template get_item<GenericGenerator>(measured_object);
                         break;
-                    case MeasuredTerminalType::node:
+                    case node:
                         components_.template get_item<Node>(measured_object);
                         break;
                     default:
                         throw MissingCaseForEnumError(std::string(GenericPowerSensor::name) + " item retrieval",
                                                       input.measured_terminal_type);
                 }
 
@@ -348,29 +350,31 @@
                            return components_.template get_seq<Node>(voltage_sensor.measured_object());
                        });
         comp_topo.power_sensor_object_idx.resize(components_.template size<GenericPowerSensor>());
         std::transform(components_.template citer<GenericPowerSensor>().begin(),
                        components_.template citer<GenericPowerSensor>().end(),
                        comp_topo.power_sensor_object_idx.begin(), [this](GenericPowerSensor const& power_sensor) {
                            switch (power_sensor.get_terminal_type()) {
-                               case MeasuredTerminalType::branch_from:
-                               case MeasuredTerminalType::branch_to:
+                               using enum MeasuredTerminalType;
+
+                               case branch_from:
+                               case branch_to:
                                    return components_.template get_seq<Branch>(power_sensor.measured_object());
-                               case MeasuredTerminalType::source:
+                               case source:
                                    return components_.template get_seq<Source>(power_sensor.measured_object());
-                               case MeasuredTerminalType::shunt:
+                               case shunt:
                                    return components_.template get_seq<Shunt>(power_sensor.measured_object());
-                               case MeasuredTerminalType::load:
-                               case MeasuredTerminalType::generator:
+                               case load:
+                               case generator:
                                    return components_.template get_seq<GenericLoadGen>(power_sensor.measured_object());
-                               case MeasuredTerminalType::branch3_1:
-                               case MeasuredTerminalType::branch3_2:
-                               case MeasuredTerminalType::branch3_3:
+                               case branch3_1:
+                               case branch3_2:
+                               case branch3_3:
                                    return components_.template get_seq<Branch3>(power_sensor.measured_object());
-                               case MeasuredTerminalType::node:
+                               case node:
                                    return components_.template get_seq<Node>(power_sensor.measured_object());
                                default:
                                    throw MissingCaseForEnumError("Power sensor idx to seq transformation",
                                                                  power_sensor.get_terminal_type());
                            }
                        });
         comp_topo.power_sensor_terminal_type.resize(components_.template size<GenericPowerSensor>());
@@ -838,60 +842,64 @@
             components_.template citer<Component>().begin(), components_.template citer<Component>().end(),
             comp_topo_->power_sensor_object_idx.cbegin() +
                 components_.template get_start_idx<GenericPowerSensor, Component>(),
             res_it, [this, &math_output](GenericPowerSensor const& power_sensor, Idx const obj_seq) {
                 auto const terminal_type = power_sensor.get_terminal_type();
                 Idx2D const obj_math_id = [&]() {
                     switch (terminal_type) {
-                        case MeasuredTerminalType::branch_from:
-                        case MeasuredTerminalType::branch_to:
+                        using enum MeasuredTerminalType;
+
+                        case branch_from:
+                        case branch_to:
                             return comp_coup_->branch[obj_seq];
-                        case MeasuredTerminalType::source:
+                        case source:
                             return comp_coup_->source[obj_seq];
-                        case MeasuredTerminalType::shunt:
+                        case shunt:
                             return comp_coup_->shunt[obj_seq];
-                        case MeasuredTerminalType::load:
-                        case MeasuredTerminalType::generator:
+                        case load:
+                        case generator:
                             return comp_coup_->load_gen[obj_seq];
                         // from branch3, get relevant math object branch based on the measured side
-                        case MeasuredTerminalType::branch3_1:
+                        case branch3_1:
                             return Idx2D{comp_coup_->branch3[obj_seq].group, comp_coup_->branch3[obj_seq].pos[0]};
-                        case MeasuredTerminalType::branch3_2:
+                        case branch3_2:
                             return Idx2D{comp_coup_->branch3[obj_seq].group, comp_coup_->branch3[obj_seq].pos[1]};
-                        case MeasuredTerminalType::branch3_3:
+                        case branch3_3:
                             return Idx2D{comp_coup_->branch3[obj_seq].group, comp_coup_->branch3[obj_seq].pos[2]};
-                        case MeasuredTerminalType::node:
+                        case node:
                             return comp_coup_->node[obj_seq];
                         default:
                             throw MissingCaseForEnumError(std::string(GenericPowerSensor::name) + " output_result()",
                                                           terminal_type);
                     }
                 }();
 
                 if (obj_math_id.group == -1) {
                     return power_sensor.get_null_output<sym>();
                 }
 
                 switch (terminal_type) {
-                    case MeasuredTerminalType::branch_from:
+                    using enum MeasuredTerminalType;
+
+                    case branch_from:
                     // all power sensors in branch3 are at from side in the mathematical model
-                    case MeasuredTerminalType::branch3_1:
-                    case MeasuredTerminalType::branch3_2:
-                    case MeasuredTerminalType::branch3_3:
+                    case branch3_1:
+                    case branch3_2:
+                    case branch3_3:
                         return power_sensor.get_output<sym>(math_output[obj_math_id.group].branch[obj_math_id.pos].s_f);
-                    case MeasuredTerminalType::branch_to:
+                    case branch_to:
                         return power_sensor.get_output<sym>(math_output[obj_math_id.group].branch[obj_math_id.pos].s_t);
-                    case MeasuredTerminalType::source:
+                    case source:
                         return power_sensor.get_output<sym>(math_output[obj_math_id.group].source[obj_math_id.pos].s);
-                    case MeasuredTerminalType::shunt:
+                    case shunt:
                         return power_sensor.get_output<sym>(math_output[obj_math_id.group].shunt[obj_math_id.pos].s);
-                    case MeasuredTerminalType::load:
-                    case MeasuredTerminalType::generator:
+                    case load:
+                    case generator:
                         return power_sensor.get_output<sym>(math_output[obj_math_id.group].load_gen[obj_math_id.pos].s);
-                    case MeasuredTerminalType::node:
+                    case node:
                         return power_sensor.get_output<sym>(
                             math_output[obj_math_id.group].bus_injection[obj_math_id.pos]);
                     default:
                         throw MissingCaseForEnumError(std::string(GenericPowerSensor::name) + " output_result()",
                                                       terminal_type);
                 }
             });
```

### Comparing `power-grid-model-1.5.0rc9190015282548/power_grid_model_c/power_grid_model/include/power_grid_model/math_solver/block_matrix.hpp` & `power-grid-model-1.5.0rc9190704883749/power_grid_model_c/power_grid_model/include/power_grid_model/math_solver/block_matrix.hpp`

 * *Files identical despite different names*

### Comparing `power-grid-model-1.5.0rc9190015282548/power_grid_model_c/power_grid_model/include/power_grid_model/math_solver/iterative_current_pf_solver.hpp` & `power-grid-model-1.5.0rc9190704883749/power_grid_model_c/power_grid_model/include/power_grid_model/math_solver/iterative_current_pf_solver.hpp`

 * *Files 1% similar despite different names*

```diff
@@ -137,23 +137,25 @@
         for (Idx bus_number = 0; bus_number != this->n_bus_; ++bus_number) {
             // loop loads/generation: j
             for (Idx load_number = load_gen_bus_indptr[bus_number]; load_number != load_gen_bus_indptr[bus_number + 1];
                  ++load_number) {
                 // load type
                 LoadGenType const type = load_gen_type[load_number];
                 switch (type) {
-                    case LoadGenType::const_pq:
+                    using enum LoadGenType;
+
+                    case const_pq:
                         // I_inj_i = conj(S_inj_j/U_i) for constant PQ type
                         rhs_u_[bus_number] += conj(input.s_injection[load_number] / u[bus_number]);
                         break;
-                    case LoadGenType::const_y:
+                    case const_y:
                         // I_inj_i = conj((S_inj_j * abs(U_i)^2) / U_i) = conj((S_inj_j) * U_i for const impedance type
                         rhs_u_[bus_number] += conj(input.s_injection[load_number]) * u[bus_number];
                         break;
-                    case LoadGenType::const_i:
+                    case const_i:
                         // I_inj_i = conj(S_inj_j*abs(U_i)/U_i) for const current type
                         rhs_u_[bus_number] +=
                             conj(input.s_injection[load_number] * cabs(u[bus_number]) / u[bus_number]);
                         break;
                     default:
                         throw MissingCaseForEnumError("Injection current calculation", type);
                 }
```

### Comparing `power-grid-model-1.5.0rc9190015282548/power_grid_model_c/power_grid_model/include/power_grid_model/math_solver/iterative_linear_se_solver.hpp` & `power-grid-model-1.5.0rc9190704883749/power_grid_model_c/power_grid_model/include/power_grid_model/math_solver/iterative_linear_se_solver.hpp`

 * *Files identical despite different names*

### Comparing `power-grid-model-1.5.0rc9190015282548/power_grid_model_c/power_grid_model/include/power_grid_model/math_solver/iterative_pf_solver.hpp` & `power-grid-model-1.5.0rc9190704883749/power_grid_model_c/power_grid_model/include/power_grid_model/math_solver/iterative_pf_solver.hpp`

 * *Files 2% similar despite different names*

```diff
@@ -126,24 +126,26 @@
             }
 
             // load_gen
             for (Idx load_gen = (*load_gen_bus_indptr_)[bus]; load_gen != (*load_gen_bus_indptr_)[bus + 1];
                  ++load_gen) {
                 LoadGenType const type = (*load_gen_type_)[load_gen];
                 switch (type) {
-                    case LoadGenType::const_pq:
+                    using enum LoadGenType;
+
+                    case const_pq:
                         // always same power
                         output.load_gen[load_gen].s = input.s_injection[load_gen];
                         break;
-                    case LoadGenType::const_y:
+                    case const_y:
                         // power is quadratic relation to voltage
                         output.load_gen[load_gen].s =
                             input.s_injection[load_gen] * cabs(output.u[bus]) * cabs(output.u[bus]);
                         break;
-                    case LoadGenType::const_i:
+                    case const_i:
                         // power is linear relation to voltage
                         output.load_gen[load_gen].s = input.s_injection[load_gen] * cabs(output.u[bus]);
                         break;
                     default:
                         throw MissingCaseForEnumError("Power injection", type);
                 }
                 output.load_gen[load_gen].i = conj(output.load_gen[load_gen].s / output.u[bus]);
```

### Comparing `power-grid-model-1.5.0rc9190015282548/power_grid_model_c/power_grid_model/include/power_grid_model/math_solver/linear_pf_solver.hpp` & `power-grid-model-1.5.0rc9190704883749/power_grid_model_c/power_grid_model/include/power_grid_model/math_solver/linear_pf_solver.hpp`

 * *Files identical despite different names*

### Comparing `power-grid-model-1.5.0rc9190015282548/power_grid_model_c/power_grid_model/include/power_grid_model/math_solver/math_solver.hpp` & `power-grid-model-1.5.0rc9190704883749/power_grid_model_c/power_grid_model/include/power_grid_model/math_solver/math_solver.hpp`

 * *Files 3% similar despite different names*

```diff
@@ -34,27 +34,29 @@
           all_const_y_{std::all_of(topo_ptr->load_gen_type.cbegin(), topo_ptr->load_gen_type.cend(), [](LoadGenType x) {
               return x == LoadGenType::const_y;
           })} {
     }
 
     MathOutput<sym> run_power_flow(PowerFlowInput<sym> const& input, double err_tol, Idx max_iter,
                                    CalculationInfo& calculation_info, CalculationMethod calculation_method) {
+        using enum CalculationMethod;
+
         // set method to always linear if all load_gens have const_y
-        calculation_method = all_const_y_ ? CalculationMethod::linear : calculation_method;
+        calculation_method = all_const_y_ ? linear : calculation_method;
 
         switch (calculation_method) {
-            case CalculationMethod::default_method:
+            case default_method:
                 [[fallthrough]];  // use Newton-Raphson by default
-            case CalculationMethod::newton_raphson:
+            case newton_raphson:
                 return run_power_flow_newton_raphson(input, err_tol, max_iter, calculation_info);
-            case CalculationMethod::linear:
+            case linear:
                 return run_power_flow_linear(input, err_tol, max_iter, calculation_info);
-            case CalculationMethod::linear_current:
+            case linear_current:
                 return run_power_flow_linear_current(input, err_tol, max_iter, calculation_info);
-            case CalculationMethod::iterative_current:
+            case iterative_current:
                 return run_power_flow_iterative_current(input, err_tol, max_iter, calculation_info);
             default:
                 throw InvalidCalculationMethod{};
         }
     }
 
     MathOutput<sym> run_state_estimation(StateEstimationInput<sym> const& input, double err_tol, Idx max_iter,
```

### Comparing `power-grid-model-1.5.0rc9190015282548/power_grid_model_c/power_grid_model/include/power_grid_model/math_solver/newton_raphson_pf_solver.hpp` & `power-grid-model-1.5.0rc9190704883749/power_grid_model_c/power_grid_model/include/power_grid_model/math_solver/newton_raphson_pf_solver.hpp`

 * *Files identical despite different names*

### Comparing `power-grid-model-1.5.0rc9190015282548/power_grid_model_c/power_grid_model/include/power_grid_model/math_solver/sparse_lu_solver.hpp` & `power-grid-model-1.5.0rc9190704883749/power_grid_model_c/power_grid_model/include/power_grid_model/math_solver/sparse_lu_solver.hpp`

 * *Files identical despite different names*

### Comparing `power-grid-model-1.5.0rc9190015282548/power_grid_model_c/power_grid_model/include/power_grid_model/math_solver/y_bus.hpp` & `power-grid-model-1.5.0rc9190704883749/power_grid_model_c/power_grid_model/include/power_grid_model/math_solver/y_bus.hpp`

 * *Files identical despite different names*

### Comparing `power-grid-model-1.5.0rc9190015282548/power_grid_model_c/power_grid_model/include/power_grid_model/power_grid_model.hpp` & `power-grid-model-1.5.0rc9190704883749/power_grid_model_c/power_grid_model/include/power_grid_model/power_grid_model.hpp`

 * *Files 2% similar despite different names*

```diff
@@ -14,14 +14,15 @@
 #include <cmath>
 #include <complex>
 #include <cstddef>
 #include <functional>
 #include <limits>
 #include <map>
 #include <memory>
+#include <numbers>
 #include <numeric>
 #include <string>
 #include <tuple>
 #include <type_traits>
 #include <utility>
 #include <variant>
 #include <vector>
@@ -41,40 +42,41 @@
 // couting iterator
 using IdxCount = boost::counting_iterator<Idx>;
 
 // struct of indexing to sub modules
 struct Idx2D {
     Idx group;  // sequence number of outer module/groups
     Idx pos;    //  sequence number inside the group
+
+    friend constexpr bool operator==(Idx2D x, Idx2D y) = default;
 };
-inline bool operator==(Idx2D x, Idx2D y) {
-    return x.group == y.group && x.pos == y.pos;
-}
 
 // math constant
 using namespace std::complex_literals;
 using DoubleComplex = std::complex<double>;
-constexpr double sqrt3 = 1.73205080756887729;
-constexpr double sqrt3_inv = 1.0 / sqrt3;
+
+using std::numbers::inv_sqrt3;
+using std::numbers::pi;
+using std::numbers::sqrt3;
+
 constexpr DoubleComplex a2{-0.5, -sqrt3 / 2.0};
 constexpr DoubleComplex a{-0.5, sqrt3 / 2.0};
-constexpr double pi = 3.14159265358979323;
 constexpr double deg_30 = 1.0 / 6.0 * pi;
 constexpr double deg_120 = 2.0 / 3.0 * pi;
 constexpr double deg_240 = 4.0 / 3.0 * pi;
 constexpr double numerical_tolerance = 1e-8;
 constexpr double nan = std::numeric_limits<double>::quiet_NaN();
 constexpr IntS na_IntS = std::numeric_limits<IntS>::min();
 constexpr ID na_IntID = std::numeric_limits<ID>::min();
 
 // power grid constant
 constexpr double base_power_3p = 1e6;
 constexpr double base_power_1p = base_power_3p / 3.0;
 template <bool sym>
-constexpr double u_scale = sym ? 1.0 : sqrt3_inv;
+constexpr double u_scale = sym ? 1.0 : inv_sqrt3;
 template <bool sym>
 constexpr double base_power = sym ? base_power_3p : base_power_1p;
 // links are direct line between nodes with infinite element_admittance in theory
 // for numerical calculation, a big link element_admittance is assigned
 // 1e6 Siemens element_admittance in 10kV network
 constexpr double g_link = 1e6 / (base_power_3p / 10e3 / 10e3);
 constexpr DoubleComplex y_link{g_link, g_link};
```

### Comparing `power-grid-model-1.5.0rc9190015282548/power_grid_model_c/power_grid_model/include/power_grid_model/sparse_mapping.hpp` & `power-grid-model-1.5.0rc9190704883749/power_grid_model_c/power_grid_model/include/power_grid_model/sparse_mapping.hpp`

 * *Files identical despite different names*

### Comparing `power-grid-model-1.5.0rc9190015282548/power_grid_model_c/power_grid_model/include/power_grid_model/three_phase_tensor.hpp` & `power-grid-model-1.5.0rc9190704883749/power_grid_model_c/power_grid_model/include/power_grid_model/three_phase_tensor.hpp`

 * *Files 1% similar despite different names*

```diff
@@ -230,15 +230,15 @@
     return z;
 }
 inline double mean_val(double z) {
     return z;
 }
 
 template <bool sym, class T>
-inline auto process_mean_val(T&& m) {
+inline auto process_mean_val(const T& m) {
     if constexpr (sym) {
         return mean_val(m);
     }
     else {
         return m;
     }
 }
```

### Comparing `power-grid-model-1.5.0rc9190015282548/power_grid_model_c/power_grid_model/include/power_grid_model/timer.hpp` & `power-grid-model-1.5.0rc9190704883749/power_grid_model_c/power_grid_model/include/power_grid_model/timer.hpp`

 * *Files 25% similar despite different names*

```diff
@@ -10,31 +10,30 @@
 #include <sstream>
 
 #include "power_grid_model.hpp"
 
 namespace power_grid_model {
 
 class Timer {
-   protected:
+   private:
     CalculationInfo *info_;
     int code_;
     std::string name_;
     Clock::time_point start_;
 
    public:
     Timer() : info_(nullptr){};
 
     Timer(CalculationInfo &info, int code, std::string name)
         : info_(&info), code_(code), name_(std::move(name)), start_(Clock::now()) {
     }
 
-    ~Timer() {
-        if (info_)
-            stop();
-    }
+    Timer(const Timer &) = delete;
+    Timer(Timer &&) = default;
+    Timer &operator=(const Timer &) = delete;
 
     Timer &operator=(Timer &&timer) noexcept {
         // Stop the current timer
         stop();
 
         // Copy/move members
         info_ = timer.info_;
@@ -45,14 +44,19 @@
         // Disable original timer
         timer.info_ = nullptr;
 
         // Return reference
         return *this;
     }
 
+    ~Timer() {
+        if (info_)
+            stop();
+    }
+
     void stop() {
         if (info_) {
             auto const now = Clock::now();
             auto const duration = Duration(now - start_);
             info_->operator[](Timer::make_key(code_, name_)) += (double)duration.count();
             info_ = nullptr;
         }
```

### Comparing `power-grid-model-1.5.0rc9190015282548/power_grid_model_c/power_grid_model/include/power_grid_model/topology.hpp` & `power-grid-model-1.5.0rc9190704883749/power_grid_model_c/power_grid_model/include/power_grid_model/topology.hpp`

 * *Files 2% similar despite different names*

```diff
@@ -507,22 +507,24 @@
     struct SensorBranchObjectFinder {
         Idx size() const {
             return (Idx)sensor_obj_idx.size();
         }
         Idx2D find_math_object(Idx component_i) const {
             Idx const obj_idx = sensor_obj_idx[component_i];
             switch (power_sensor_terminal_type[component_i]) {
-                case MeasuredTerminalType::branch_from:
+                using enum MeasuredTerminalType;
+
+                case branch_from:
                     return branch_coupling[obj_idx];
                 // return relevant branch mapped from branch3
-                case MeasuredTerminalType::branch3_1:
+                case branch3_1:
                     return {branch3_coupling[obj_idx].group, branch3_coupling[obj_idx].pos[0]};
-                case MeasuredTerminalType::branch3_2:
+                case branch3_2:
                     return {branch3_coupling[obj_idx].group, branch3_coupling[obj_idx].pos[1]};
-                case MeasuredTerminalType::branch3_3:
+                case branch3_3:
                     return {branch3_coupling[obj_idx].group, branch3_coupling[obj_idx].pos[2]};
                 default:
                     assert(false);
                     return {};
             }
         }
         IdxVector const& sensor_obj_idx;
@@ -633,19 +635,21 @@
                 return comp_topo_.power_sensor_terminal_type[i] == MeasuredTerminalType::load ||
                        comp_topo_.power_sensor_terminal_type[i] == MeasuredTerminalType::generator;
             });
 
         // branch 'from' power sensors
         // include all branch3 sensors
         auto const predicate_from_sensor = [&](Idx i) {
-            return comp_topo_.power_sensor_terminal_type[i] == MeasuredTerminalType::branch_from ||
+            using enum MeasuredTerminalType;
+
+            return comp_topo_.power_sensor_terminal_type[i] == branch_from ||
                    // all branch3 sensors are at from side in the mathemtical model
-                   comp_topo_.power_sensor_terminal_type[i] == MeasuredTerminalType::branch3_1 ||
-                   comp_topo_.power_sensor_terminal_type[i] == MeasuredTerminalType::branch3_2 ||
-                   comp_topo_.power_sensor_terminal_type[i] == MeasuredTerminalType::branch3_3;
+                   comp_topo_.power_sensor_terminal_type[i] == branch3_1 ||
+                   comp_topo_.power_sensor_terminal_type[i] == branch3_2 ||
+                   comp_topo_.power_sensor_terminal_type[i] == branch3_3;
         };
         SensorBranchObjectFinder const object_finder_from_sensor{comp_topo_.power_sensor_object_idx,
                                                                  comp_topo_.power_sensor_terminal_type,
                                                                  comp_coup_.branch, comp_coup_.branch3};
         couple_object_components<&MathModelTopology::branch_from_power_sensor_indptr, &MathModelTopology::n_branch>(
             object_finder_from_sensor, comp_coup_.power_sensor, predicate_from_sensor);
```

### Comparing `power-grid-model-1.5.0rc9190015282548/power_grid_model_c/power_grid_model_c/CMakeLists.txt` & `power-grid-model-1.5.0rc9190704883749/power_grid_model_c/power_grid_model_c/CMakeLists.txt`

 * *Files identical despite different names*

### Comparing `power-grid-model-1.5.0rc9190015282548/power_grid_model_c/power_grid_model_c/include/power_grid_model_c.h` & `power-grid-model-1.5.0rc9190704883749/power_grid_model_c/power_grid_model_c/include/power_grid_model_c.h`

 * *Files identical despite different names*

### Comparing `power-grid-model-1.5.0rc9190015282548/power_grid_model_c/power_grid_model_c/power_grid_model_c.cpp` & `power-grid-model-1.5.0rc9190704883749/power_grid_model_c/power_grid_model_c/power_grid_model_c.cpp`

 * *Files 0% similar despite different names*

```diff
@@ -31,15 +31,15 @@
 // context handle
 struct PGM_Handle {
     Idx err_code;
     std::string err_msg;
     IdxVector failed_scenarios;
     std::vector<std::string> batch_errs;
     mutable std::vector<char const*> batch_errs_c_str;
-    BatchParameter batch_parameter;
+    [[no_unique_address]] BatchParameter batch_parameter;
 };
 
 // options
 struct PGM_Options {
     Idx calculation_type{PGM_power_flow};
     Idx calculation_method{PGM_default_method};
     Idx symmetric{1};
```

### Comparing `power-grid-model-1.5.0rc9190015282548/pyproject.toml` & `power-grid-model-1.5.0rc9190704883749/pyproject.toml`

 * *Files identical despite different names*

### Comparing `power-grid-model-1.5.0rc9190015282548/setup.py` & `power-grid-model-1.5.0rc9190704883749/setup.py`

 * *Files identical despite different names*

### Comparing `power-grid-model-1.5.0rc9190015282548/src/power_grid_model/core/error_handling.py` & `power-grid-model-1.5.0rc9190704883749/src/power_grid_model/core/error_handling.py`

 * *Files identical despite different names*

### Comparing `power-grid-model-1.5.0rc9190015282548/src/power_grid_model/core/options.py` & `power-grid-model-1.5.0rc9190704883749/src/power_grid_model/core/options.py`

 * *Files identical despite different names*

### Comparing `power-grid-model-1.5.0rc9190015282548/src/power_grid_model/core/power_grid_core.py` & `power-grid-model-1.5.0rc9190704883749/src/power_grid_model/core/power_grid_core.py`

 * *Files identical despite different names*

### Comparing `power-grid-model-1.5.0rc9190015282548/src/power_grid_model/core/power_grid_meta.py` & `power-grid-model-1.5.0rc9190704883749/src/power_grid_model/core/power_grid_meta.py`

 * *Files identical despite different names*

### Comparing `power-grid-model-1.5.0rc9190015282548/src/power_grid_model/core/power_grid_model.py` & `power-grid-model-1.5.0rc9190704883749/src/power_grid_model/core/power_grid_model.py`

 * *Files identical despite different names*

### Comparing `power-grid-model-1.5.0rc9190015282548/src/power_grid_model/data_types.py` & `power-grid-model-1.5.0rc9190704883749/src/power_grid_model/data_types.py`

 * *Files identical despite different names*

### Comparing `power-grid-model-1.5.0rc9190015282548/src/power_grid_model/enum.py` & `power-grid-model-1.5.0rc9190704883749/src/power_grid_model/enum.py`

 * *Files identical despite different names*

### Comparing `power-grid-model-1.5.0rc9190015282548/src/power_grid_model/utils.py` & `power-grid-model-1.5.0rc9190704883749/src/power_grid_model/utils.py`

 * *Files identical despite different names*

### Comparing `power-grid-model-1.5.0rc9190015282548/src/power_grid_model/validation/__init__.py` & `power-grid-model-1.5.0rc9190704883749/src/power_grid_model/validation/__init__.py`

 * *Files identical despite different names*

### Comparing `power-grid-model-1.5.0rc9190015282548/src/power_grid_model/validation/assertions.py` & `power-grid-model-1.5.0rc9190704883749/src/power_grid_model/validation/assertions.py`

 * *Files identical despite different names*

### Comparing `power-grid-model-1.5.0rc9190015282548/src/power_grid_model/validation/errors.py` & `power-grid-model-1.5.0rc9190704883749/src/power_grid_model/validation/errors.py`

 * *Files identical despite different names*

### Comparing `power-grid-model-1.5.0rc9190015282548/src/power_grid_model/validation/rules.py` & `power-grid-model-1.5.0rc9190704883749/src/power_grid_model/validation/rules.py`

 * *Files identical despite different names*

### Comparing `power-grid-model-1.5.0rc9190015282548/src/power_grid_model/validation/utils.py` & `power-grid-model-1.5.0rc9190704883749/src/power_grid_model/validation/utils.py`

 * *Files identical despite different names*

### Comparing `power-grid-model-1.5.0rc9190015282548/src/power_grid_model/validation/validation.py` & `power-grid-model-1.5.0rc9190704883749/src/power_grid_model/validation/validation.py`

 * *Files identical despite different names*

### Comparing `power-grid-model-1.5.0rc9190015282548/src/power_grid_model.egg-info/PKG-INFO` & `power-grid-model-1.5.0rc9190704883749/src/power_grid_model.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: power-grid-model
-Version: 1.5.0rc9190015282548
+Version: 1.5.0rc9190704883749
 Summary: Python/C++ library for distribution power system analysis
 Author-email: Alliander Dynamic Grid Calculation <dynamic.grid.calculation@alliander.com>
 License: MPL-2.0
 Project-URL: Home-page, https://lfenergy.org/projects/power-grid-model/
 Project-URL: GitHub, https://github.com/PowerGridModel/power-grid-model
 Project-URL: Documentation, https://power-grid-model.readthedocs.io/en/stable/
 Project-URL: Mailing-list, https://lists.lfenergy.org/g/powergridmodel
```

### Comparing `power-grid-model-1.5.0rc9190015282548/src/power_grid_model.egg-info/SOURCES.txt` & `power-grid-model-1.5.0rc9190704883749/src/power_grid_model.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `power-grid-model-1.5.0rc9190015282548/tests/data/power_flow/1os2msr/input.json` & `power-grid-model-1.5.0rc9190704883749/tests/data/power_flow/1os2msr/input.json`

 * *Files identical despite different names*

### Comparing `power-grid-model-1.5.0rc9190015282548/tests/data/power_flow/1os2msr/sym_output.json` & `power-grid-model-1.5.0rc9190704883749/tests/data/power_flow/1os2msr/sym_output.json`

 * *Files identical despite different names*

### Comparing `power-grid-model-1.5.0rc9190015282548/tests/data/power_flow/dummy-test/input.json` & `power-grid-model-1.5.0rc9190704883749/tests/data/power_flow/dummy-test/input.json`

 * *Files identical despite different names*

### Comparing `power-grid-model-1.5.0rc9190015282548/tests/data/power_flow/dummy-test/sym_output.json` & `power-grid-model-1.5.0rc9190704883749/tests/data/power_flow/dummy-test/sym_output.json`

 * *Files identical despite different names*

### Comparing `power-grid-model-1.5.0rc9190015282548/tests/data/power_flow/dummy-test-batch/input.json` & `power-grid-model-1.5.0rc9190704883749/tests/data/power_flow/dummy-test-batch/input.json`

 * *Files identical despite different names*

### Comparing `power-grid-model-1.5.0rc9190015282548/tests/data/power_flow/dummy-test-batch-dependent-cacheable/input.json` & `power-grid-model-1.5.0rc9190704883749/tests/data/power_flow/dummy-test-batch-dependent-cacheable/input.json`

 * *Files identical despite different names*

### Comparing `power-grid-model-1.5.0rc9190015282548/tests/data/power_flow/dummy-test-batch-dependent-not-cacheable/input.json` & `power-grid-model-1.5.0rc9190704883749/tests/data/power_flow/dummy-test-batch-dependent-not-cacheable/input.json`

 * *Files identical despite different names*

### Comparing `power-grid-model-1.5.0rc9190015282548/tests/data/power_flow/dummy-test-batch-dependent-not-cacheable/update_batch.json` & `power-grid-model-1.5.0rc9190704883749/tests/data/power_flow/dummy-test-batch-dependent-not-cacheable/update_batch.json`

 * *Files identical despite different names*

### Comparing `power-grid-model-1.5.0rc9190015282548/tests/data/power_flow/dummy-test-batch-incomplete-input/input.json` & `power-grid-model-1.5.0rc9190704883749/tests/data/power_flow/dummy-test-batch-incomplete-input/input.json`

 * *Files identical despite different names*

### Comparing `power-grid-model-1.5.0rc9190015282548/tests/data/power_flow/dummy-test-batch-independent-cacheable/input.json` & `power-grid-model-1.5.0rc9190704883749/tests/data/power_flow/dummy-test-batch-independent-cacheable/input.json`

 * *Files identical despite different names*

### Comparing `power-grid-model-1.5.0rc9190015282548/tests/data/power_flow/dummy-test-batch-independent-not-cacheable/input.json` & `power-grid-model-1.5.0rc9190704883749/tests/data/power_flow/dummy-test-batch-independent-not-cacheable/input.json`

 * *Files identical despite different names*

### Comparing `power-grid-model-1.5.0rc9190015282548/tests/data/power_flow/dummy-test-batch-independent-not-cacheable/update_batch.json` & `power-grid-model-1.5.0rc9190704883749/tests/data/power_flow/dummy-test-batch-independent-not-cacheable/update_batch.json`

 * *Files identical despite different names*

### Comparing `power-grid-model-1.5.0rc9190015282548/tests/data/power_flow/dummy-test-batch-newton/input.json` & `power-grid-model-1.5.0rc9190704883749/tests/data/power_flow/dummy-test-batch-newton/input.json`

 * *Files identical despite different names*

### Comparing `power-grid-model-1.5.0rc9190015282548/tests/data/power_flow/dummy-test-i-n-optional/input.json` & `power-grid-model-1.5.0rc9190704883749/tests/data/power_flow/dummy-test-i-n-optional/input.json`

 * *Files identical despite different names*

### Comparing `power-grid-model-1.5.0rc9190015282548/tests/data/power_flow/dummy-test-i-n-optional/sym_output.json` & `power-grid-model-1.5.0rc9190704883749/tests/data/power_flow/dummy-test-i-n-optional/sym_output.json`

 * *Files identical despite different names*

### Comparing `power-grid-model-1.5.0rc9190015282548/tests/data/power_flow/gaia-example/asym_output.json` & `power-grid-model-1.5.0rc9190704883749/tests/data/power_flow/gaia-example/asym_output.json`

 * *Files identical despite different names*

### Comparing `power-grid-model-1.5.0rc9190015282548/tests/data/power_flow/gaia-example/gaia_grid.gnf` & `power-grid-model-1.5.0rc9190704883749/tests/data/power_flow/gaia-example/gaia_grid.gnf`

 * *Files identical despite different names*

### Comparing `power-grid-model-1.5.0rc9190015282548/tests/data/power_flow/gaia-example/input.json` & `power-grid-model-1.5.0rc9190704883749/tests/data/power_flow/gaia-example/input.json`

 * *Files identical despite different names*

### Comparing `power-grid-model-1.5.0rc9190015282548/tests/data/power_flow/multi-source-with-angle/input.json` & `power-grid-model-1.5.0rc9190704883749/tests/data/power_flow/multi-source-with-angle/input.json`

 * *Files identical despite different names*

### Comparing `power-grid-model-1.5.0rc9190015282548/tests/data/power_flow/pandapower/components/asymmetric/asym_gen/README.md` & `power-grid-model-1.5.0rc9190704883749/tests/data/power_flow/pandapower/components/asymmetric/asym_gen/README.md`

 * *Files identical despite different names*

### Comparing `power-grid-model-1.5.0rc9190015282548/tests/data/power_flow/pandapower/components/asymmetric/asym_gen/asym_output.json` & `power-grid-model-1.5.0rc9190704883749/tests/data/power_flow/pandapower/components/asymmetric/asym_gen/asym_output.json`

 * *Files identical despite different names*

### Comparing `power-grid-model-1.5.0rc9190015282548/tests/data/power_flow/pandapower/components/asymmetric/asym_gen/input.json` & `power-grid-model-1.5.0rc9190704883749/tests/data/power_flow/pandapower/components/asymmetric/asym_gen/input.json`

 * *Files identical despite different names*

### Comparing `power-grid-model-1.5.0rc9190015282548/tests/data/power_flow/pandapower/components/asymmetric/asym_load/README.md` & `power-grid-model-1.5.0rc9190704883749/tests/data/power_flow/pandapower/components/asymmetric/asym_load/README.md`

 * *Files identical despite different names*

### Comparing `power-grid-model-1.5.0rc9190015282548/tests/data/power_flow/pandapower/components/asymmetric/asym_load/asym_output.json` & `power-grid-model-1.5.0rc9190704883749/tests/data/power_flow/pandapower/components/asymmetric/asym_load/asym_output.json`

 * *Files identical despite different names*

### Comparing `power-grid-model-1.5.0rc9190015282548/tests/data/power_flow/pandapower/components/asymmetric/asym_load/input.json` & `power-grid-model-1.5.0rc9190704883749/tests/data/power_flow/pandapower/components/asymmetric/asym_load/input.json`

 * *Files identical despite different names*

### Comparing `power-grid-model-1.5.0rc9190015282548/tests/data/power_flow/pandapower/components/asymmetric/line/README.md` & `power-grid-model-1.5.0rc9190704883749/tests/data/power_flow/pandapower/components/asymmetric/line/README.md`

 * *Files identical despite different names*

### Comparing `power-grid-model-1.5.0rc9190015282548/tests/data/power_flow/pandapower/components/asymmetric/line/asym_output.json` & `power-grid-model-1.5.0rc9190704883749/tests/data/power_flow/pandapower/components/asymmetric/line/asym_output.json`

 * *Files identical despite different names*

### Comparing `power-grid-model-1.5.0rc9190015282548/tests/data/power_flow/pandapower/components/asymmetric/line/input.json` & `power-grid-model-1.5.0rc9190704883749/tests/data/power_flow/pandapower/components/asymmetric/line/input.json`

 * *Files identical despite different names*

### Comparing `power-grid-model-1.5.0rc9190015282548/tests/data/power_flow/pandapower/components/asymmetric/node/README.md` & `power-grid-model-1.5.0rc9190704883749/tests/data/power_flow/pandapower/components/asymmetric/node/README.md`

 * *Files identical despite different names*

### Comparing `power-grid-model-1.5.0rc9190015282548/tests/data/power_flow/pandapower/components/asymmetric/node/asym_output.json` & `power-grid-model-1.5.0rc9190704883749/tests/data/power_flow/pandapower/components/asymmetric/node/asym_output.json`

 * *Files identical despite different names*

### Comparing `power-grid-model-1.5.0rc9190015282548/tests/data/power_flow/pandapower/components/asymmetric/node/input.json` & `power-grid-model-1.5.0rc9190704883749/tests/data/power_flow/pandapower/components/asymmetric/node/input.json`

 * *Files identical despite different names*

### Comparing `power-grid-model-1.5.0rc9190015282548/tests/data/power_flow/pandapower/components/asymmetric/shunt/README.md` & `power-grid-model-1.5.0rc9190704883749/tests/data/power_flow/pandapower/components/asymmetric/shunt/README.md`

 * *Files identical despite different names*

### Comparing `power-grid-model-1.5.0rc9190015282548/tests/data/power_flow/pandapower/components/asymmetric/shunt/asym_output.json` & `power-grid-model-1.5.0rc9190704883749/tests/data/power_flow/pandapower/components/asymmetric/shunt/asym_output.json`

 * *Files identical despite different names*

### Comparing `power-grid-model-1.5.0rc9190015282548/tests/data/power_flow/pandapower/components/asymmetric/shunt/input.json` & `power-grid-model-1.5.0rc9190704883749/tests/data/power_flow/pandapower/components/asymmetric/shunt/input.json`

 * *Files identical despite different names*

### Comparing `power-grid-model-1.5.0rc9190015282548/tests/data/power_flow/pandapower/components/asymmetric/source/README.md` & `power-grid-model-1.5.0rc9190704883749/tests/data/power_flow/pandapower/components/asymmetric/source/README.md`

 * *Files identical despite different names*

### Comparing `power-grid-model-1.5.0rc9190015282548/tests/data/power_flow/pandapower/components/asymmetric/source/asym_output.json` & `power-grid-model-1.5.0rc9190704883749/tests/data/power_flow/pandapower/components/asymmetric/source/asym_output.json`

 * *Files identical despite different names*

### Comparing `power-grid-model-1.5.0rc9190015282548/tests/data/power_flow/pandapower/components/asymmetric/source/input.json` & `power-grid-model-1.5.0rc9190704883749/tests/data/power_flow/pandapower/components/asymmetric/source/input.json`

 * *Files identical despite different names*

### Comparing `power-grid-model-1.5.0rc9190015282548/tests/data/power_flow/pandapower/components/asymmetric/sym_gen/README.md` & `power-grid-model-1.5.0rc9190704883749/tests/data/power_flow/pandapower/components/asymmetric/sym_gen/README.md`

 * *Files identical despite different names*

### Comparing `power-grid-model-1.5.0rc9190015282548/tests/data/power_flow/pandapower/components/asymmetric/sym_gen/asym_output.json` & `power-grid-model-1.5.0rc9190704883749/tests/data/power_flow/pandapower/components/asymmetric/sym_gen/asym_output.json`

 * *Files identical despite different names*

### Comparing `power-grid-model-1.5.0rc9190015282548/tests/data/power_flow/pandapower/components/asymmetric/sym_gen/input.json` & `power-grid-model-1.5.0rc9190704883749/tests/data/power_flow/pandapower/components/asymmetric/sym_gen/input.json`

 * *Files identical despite different names*

### Comparing `power-grid-model-1.5.0rc9190015282548/tests/data/power_flow/pandapower/components/asymmetric/sym_load/README.md` & `power-grid-model-1.5.0rc9190704883749/tests/data/power_flow/pandapower/components/asymmetric/sym_load/README.md`

 * *Files identical despite different names*

### Comparing `power-grid-model-1.5.0rc9190015282548/tests/data/power_flow/pandapower/components/asymmetric/sym_load/asym_output.json` & `power-grid-model-1.5.0rc9190704883749/tests/data/power_flow/pandapower/components/asymmetric/sym_load/asym_output.json`

 * *Files identical despite different names*

### Comparing `power-grid-model-1.5.0rc9190015282548/tests/data/power_flow/pandapower/components/asymmetric/sym_load/input.json` & `power-grid-model-1.5.0rc9190704883749/tests/data/power_flow/pandapower/components/asymmetric/sym_load/input.json`

 * *Files identical despite different names*

### Comparing `power-grid-model-1.5.0rc9190015282548/tests/data/power_flow/pandapower/components/asymmetric/transformer/README.md` & `power-grid-model-1.5.0rc9190704883749/tests/data/power_flow/pandapower/components/asymmetric/transformer/README.md`

 * *Files identical despite different names*

### Comparing `power-grid-model-1.5.0rc9190015282548/tests/data/power_flow/pandapower/components/asymmetric/transformer/asym_output_batch.json` & `power-grid-model-1.5.0rc9190704883749/tests/data/power_flow/pandapower/components/asymmetric/transformer/asym_output_batch.json`

 * *Files identical despite different names*

### Comparing `power-grid-model-1.5.0rc9190015282548/tests/data/power_flow/pandapower/components/asymmetric/transformer/input.json` & `power-grid-model-1.5.0rc9190704883749/tests/data/power_flow/pandapower/components/asymmetric/transformer/input.json`

 * *Files identical despite different names*

### Comparing `power-grid-model-1.5.0rc9190015282548/tests/data/power_flow/pandapower/components/asymmetric/transformer/update_batch.json` & `power-grid-model-1.5.0rc9190704883749/tests/data/power_flow/pandapower/components/asymmetric/transformer/update_batch.json`

 * *Files identical despite different names*

### Comparing `power-grid-model-1.5.0rc9190015282548/tests/data/power_flow/pandapower/components/symmetric/line/README.md` & `power-grid-model-1.5.0rc9190704883749/tests/data/power_flow/pandapower/components/symmetric/line/README.md`

 * *Files identical despite different names*

### Comparing `power-grid-model-1.5.0rc9190015282548/tests/data/power_flow/pandapower/components/symmetric/line/input.json` & `power-grid-model-1.5.0rc9190704883749/tests/data/power_flow/pandapower/components/symmetric/line/input.json`

 * *Files identical despite different names*

### Comparing `power-grid-model-1.5.0rc9190015282548/tests/data/power_flow/pandapower/components/symmetric/line/sym_output.json` & `power-grid-model-1.5.0rc9190704883749/tests/data/power_flow/pandapower/components/symmetric/line/sym_output.json`

 * *Files identical despite different names*

### Comparing `power-grid-model-1.5.0rc9190015282548/tests/data/power_flow/pandapower/components/symmetric/node/input.json` & `power-grid-model-1.5.0rc9190704883749/tests/data/power_flow/pandapower/components/symmetric/node/input.json`

 * *Files identical despite different names*

### Comparing `power-grid-model-1.5.0rc9190015282548/tests/data/power_flow/pandapower/components/symmetric/node/sym_output.json` & `power-grid-model-1.5.0rc9190704883749/tests/data/power_flow/pandapower/components/symmetric/node/sym_output.json`

 * *Files identical despite different names*

### Comparing `power-grid-model-1.5.0rc9190015282548/tests/data/power_flow/pandapower/components/symmetric/shunt/input.json` & `power-grid-model-1.5.0rc9190704883749/tests/data/power_flow/pandapower/components/symmetric/shunt/input.json`

 * *Files identical despite different names*

### Comparing `power-grid-model-1.5.0rc9190015282548/tests/data/power_flow/pandapower/components/symmetric/shunt/sym_output.json` & `power-grid-model-1.5.0rc9190704883749/tests/data/power_flow/pandapower/components/symmetric/shunt/sym_output.json`

 * *Files identical despite different names*

### Comparing `power-grid-model-1.5.0rc9190015282548/tests/data/power_flow/pandapower/components/symmetric/source/input.json` & `power-grid-model-1.5.0rc9190704883749/tests/data/power_flow/pandapower/components/symmetric/source/input.json`

 * *Files identical despite different names*

### Comparing `power-grid-model-1.5.0rc9190015282548/tests/data/power_flow/pandapower/components/symmetric/source/sym_output.json` & `power-grid-model-1.5.0rc9190704883749/tests/data/power_flow/pandapower/components/symmetric/source/sym_output.json`

 * *Files identical despite different names*

### Comparing `power-grid-model-1.5.0rc9190015282548/tests/data/power_flow/pandapower/components/symmetric/sym_gen/README.md` & `power-grid-model-1.5.0rc9190704883749/tests/data/power_flow/pandapower/components/symmetric/sym_gen/README.md`

 * *Files identical despite different names*

### Comparing `power-grid-model-1.5.0rc9190015282548/tests/data/power_flow/pandapower/components/symmetric/sym_gen/input.json` & `power-grid-model-1.5.0rc9190704883749/tests/data/power_flow/pandapower/components/symmetric/sym_gen/input.json`

 * *Files identical despite different names*

### Comparing `power-grid-model-1.5.0rc9190015282548/tests/data/power_flow/pandapower/components/symmetric/sym_gen/sym_output.json` & `power-grid-model-1.5.0rc9190704883749/tests/data/power_flow/pandapower/components/symmetric/sym_gen/sym_output.json`

 * *Files identical despite different names*

### Comparing `power-grid-model-1.5.0rc9190015282548/tests/data/power_flow/pandapower/components/symmetric/sym_load/README.md` & `power-grid-model-1.5.0rc9190704883749/tests/data/power_flow/pandapower/components/symmetric/sym_load/README.md`

 * *Files identical despite different names*

### Comparing `power-grid-model-1.5.0rc9190015282548/tests/data/power_flow/pandapower/components/symmetric/sym_load/input.json` & `power-grid-model-1.5.0rc9190704883749/tests/data/power_flow/pandapower/components/symmetric/sym_load/input.json`

 * *Files identical despite different names*

### Comparing `power-grid-model-1.5.0rc9190015282548/tests/data/power_flow/pandapower/components/symmetric/sym_load/sym_output.json` & `power-grid-model-1.5.0rc9190704883749/tests/data/power_flow/pandapower/components/symmetric/sym_load/sym_output.json`

 * *Files identical despite different names*

### Comparing `power-grid-model-1.5.0rc9190015282548/tests/data/power_flow/pandapower/components/symmetric/three_winding_transformer/README.md` & `power-grid-model-1.5.0rc9190704883749/tests/data/power_flow/pandapower/components/symmetric/three_winding_transformer/README.md`

 * *Files identical despite different names*

### Comparing `power-grid-model-1.5.0rc9190015282548/tests/data/power_flow/pandapower/components/symmetric/three_winding_transformer/input.json` & `power-grid-model-1.5.0rc9190704883749/tests/data/power_flow/pandapower/components/symmetric/three_winding_transformer/input.json`

 * *Files identical despite different names*

### Comparing `power-grid-model-1.5.0rc9190015282548/tests/data/power_flow/pandapower/components/symmetric/three_winding_transformer/sym_output_batch.json` & `power-grid-model-1.5.0rc9190704883749/tests/data/power_flow/pandapower/components/symmetric/three_winding_transformer/sym_output_batch.json`

 * *Files identical despite different names*

### Comparing `power-grid-model-1.5.0rc9190015282548/tests/data/power_flow/pandapower/components/symmetric/three_winding_transformer/update_batch.json` & `power-grid-model-1.5.0rc9190704883749/tests/data/power_flow/pandapower/components/symmetric/three_winding_transformer/update_batch.json`

 * *Files identical despite different names*

### Comparing `power-grid-model-1.5.0rc9190015282548/tests/data/power_flow/pandapower/components/symmetric/transformer/README.md` & `power-grid-model-1.5.0rc9190704883749/tests/data/power_flow/pandapower/components/symmetric/transformer/README.md`

 * *Files identical despite different names*

### Comparing `power-grid-model-1.5.0rc9190015282548/tests/data/power_flow/pandapower/components/symmetric/transformer/input.json` & `power-grid-model-1.5.0rc9190704883749/tests/data/power_flow/pandapower/components/symmetric/transformer/input.json`

 * *Files identical despite different names*

### Comparing `power-grid-model-1.5.0rc9190015282548/tests/data/power_flow/pandapower/components/symmetric/transformer/sym_output_batch.json` & `power-grid-model-1.5.0rc9190704883749/tests/data/power_flow/pandapower/components/symmetric/transformer/sym_output_batch.json`

 * *Files identical despite different names*

### Comparing `power-grid-model-1.5.0rc9190015282548/tests/data/power_flow/pandapower/components/symmetric/transformer/update_batch.json` & `power-grid-model-1.5.0rc9190704883749/tests/data/power_flow/pandapower/components/symmetric/transformer/update_batch.json`

 * *Files identical despite different names*

### Comparing `power-grid-model-1.5.0rc9190015282548/tests/data/power_flow/pandapower/networks/asymmetric/distribution-case/README.md` & `power-grid-model-1.5.0rc9190704883749/tests/data/power_flow/pandapower/networks/asymmetric/distribution-case/README.md`

 * *Files identical despite different names*

### Comparing `power-grid-model-1.5.0rc9190015282548/tests/data/power_flow/pandapower/networks/asymmetric/distribution-case/asym_output_batch.json` & `power-grid-model-1.5.0rc9190704883749/tests/data/power_flow/pandapower/networks/asymmetric/distribution-case/asym_output_batch.json`

 * *Files identical despite different names*

### Comparing `power-grid-model-1.5.0rc9190015282548/tests/data/power_flow/pandapower/networks/asymmetric/distribution-case/input.json` & `power-grid-model-1.5.0rc9190704883749/tests/data/power_flow/pandapower/networks/asymmetric/distribution-case/input.json`

 * *Files identical despite different names*

### Comparing `power-grid-model-1.5.0rc9190015282548/tests/data/power_flow/pandapower/networks/asymmetric/distribution-case/update_batch.json` & `power-grid-model-1.5.0rc9190704883749/tests/data/power_flow/pandapower/networks/asymmetric/distribution-case/update_batch.json`

 * *Files identical despite different names*

### Comparing `power-grid-model-1.5.0rc9190015282548/tests/data/power_flow/pandapower/networks/asymmetric/transmission-case/README.md` & `power-grid-model-1.5.0rc9190704883749/tests/data/power_flow/pandapower/networks/asymmetric/transmission-case/README.md`

 * *Files identical despite different names*

### Comparing `power-grid-model-1.5.0rc9190015282548/tests/data/power_flow/pandapower/networks/asymmetric/transmission-case/asym_output.json` & `power-grid-model-1.5.0rc9190704883749/tests/data/power_flow/pandapower/networks/asymmetric/transmission-case/asym_output.json`

 * *Files identical despite different names*

### Comparing `power-grid-model-1.5.0rc9190015282548/tests/data/power_flow/pandapower/networks/asymmetric/transmission-case/input.json` & `power-grid-model-1.5.0rc9190704883749/tests/data/power_flow/pandapower/networks/asymmetric/transmission-case/input.json`

 * *Files identical despite different names*

### Comparing `power-grid-model-1.5.0rc9190015282548/tests/data/power_flow/pandapower/networks/symmetric/distribution-case/README.md` & `power-grid-model-1.5.0rc9190704883749/tests/data/power_flow/pandapower/networks/symmetric/distribution-case/README.md`

 * *Files identical despite different names*

### Comparing `power-grid-model-1.5.0rc9190015282548/tests/data/power_flow/pandapower/networks/symmetric/distribution-case/input.json` & `power-grid-model-1.5.0rc9190704883749/tests/data/power_flow/pandapower/networks/symmetric/distribution-case/input.json`

 * *Files identical despite different names*

### Comparing `power-grid-model-1.5.0rc9190015282548/tests/data/power_flow/pandapower/networks/symmetric/distribution-case/sym_output_batch.json` & `power-grid-model-1.5.0rc9190704883749/tests/data/power_flow/pandapower/networks/symmetric/distribution-case/sym_output_batch.json`

 * *Files identical despite different names*

### Comparing `power-grid-model-1.5.0rc9190015282548/tests/data/power_flow/pandapower/networks/symmetric/distribution-case/update_batch.json` & `power-grid-model-1.5.0rc9190704883749/tests/data/power_flow/pandapower/networks/symmetric/distribution-case/update_batch.json`

 * *Files identical despite different names*

### Comparing `power-grid-model-1.5.0rc9190015282548/tests/data/power_flow/pandapower/networks/symmetric/transmission-case/README.md` & `power-grid-model-1.5.0rc9190704883749/tests/data/power_flow/pandapower/networks/symmetric/transmission-case/README.md`

 * *Files identical despite different names*

### Comparing `power-grid-model-1.5.0rc9190015282548/tests/data/power_flow/pandapower/networks/symmetric/transmission-case/input.json` & `power-grid-model-1.5.0rc9190704883749/tests/data/power_flow/pandapower/networks/symmetric/transmission-case/input.json`

 * *Files identical despite different names*

### Comparing `power-grid-model-1.5.0rc9190015282548/tests/data/power_flow/pandapower/networks/symmetric/transmission-case/sym_output.json` & `power-grid-model-1.5.0rc9190704883749/tests/data/power_flow/pandapower/networks/symmetric/transmission-case/sym_output.json`

 * *Files identical despite different names*

### Comparing `power-grid-model-1.5.0rc9190015282548/tests/data/power_flow/r-state-estimation/input.json` & `power-grid-model-1.5.0rc9190704883749/tests/data/power_flow/r-state-estimation/input.json`

 * *Files identical despite different names*

### Comparing `power-grid-model-1.5.0rc9190015282548/tests/data/power_flow/r-state-estimation/sym_output.json` & `power-grid-model-1.5.0rc9190704883749/tests/data/power_flow/r-state-estimation/sym_output.json`

 * *Files identical despite different names*

### Comparing `power-grid-model-1.5.0rc9190015282548/tests/data/power_flow/three-winding-transformer/asym_output_batch.json` & `power-grid-model-1.5.0rc9190704883749/tests/data/power_flow/three-winding-transformer/asym_output_batch.json`

 * *Files identical despite different names*

### Comparing `power-grid-model-1.5.0rc9190015282548/tests/data/power_flow/three-winding-transformer/input.json` & `power-grid-model-1.5.0rc9190704883749/tests/data/power_flow/three-winding-transformer/input.json`

 * *Files identical despite different names*

### Comparing `power-grid-model-1.5.0rc9190015282548/tests/data/power_flow/three-winding-transformer/sym_output_batch.json` & `power-grid-model-1.5.0rc9190704883749/tests/data/power_flow/three-winding-transformer/sym_output_batch.json`

 * *Files identical despite different names*

### Comparing `power-grid-model-1.5.0rc9190015282548/tests/data/power_flow/three-winding-transformer/update_batch.json` & `power-grid-model-1.5.0rc9190704883749/tests/data/power_flow/three-winding-transformer/update_batch.json`

 * *Files identical despite different names*

### Comparing `power-grid-model-1.5.0rc9190015282548/tests/data/power_flow/vision-example/asym_output.json` & `power-grid-model-1.5.0rc9190704883749/tests/data/power_flow/vision-example/asym_output.json`

 * *Files identical despite different names*

### Comparing `power-grid-model-1.5.0rc9190015282548/tests/data/power_flow/vision-example/input.json` & `power-grid-model-1.5.0rc9190704883749/tests/data/power_flow/vision-example/input.json`

 * *Files identical despite different names*

### Comparing `power-grid-model-1.5.0rc9190015282548/tests/data/power_flow/vision-example/vision_grid.vnf` & `power-grid-model-1.5.0rc9190704883749/tests/data/power_flow/vision-example/vision_grid.vnf`

 * *Files identical despite different names*

### Comparing `power-grid-model-1.5.0rc9190015282548/tests/data/power_flow/vision-validation-network/asym_output.json` & `power-grid-model-1.5.0rc9190704883749/tests/data/power_flow/vision-validation-network/asym_output.json`

 * *Files identical despite different names*

### Comparing `power-grid-model-1.5.0rc9190015282548/tests/data/power_flow/vision-validation-network/input.json` & `power-grid-model-1.5.0rc9190704883749/tests/data/power_flow/vision-validation-network/input.json`

 * *Files identical despite different names*

### Comparing `power-grid-model-1.5.0rc9190015282548/tests/data/power_flow/vision-validation-network/sym_output.json` & `power-grid-model-1.5.0rc9190704883749/tests/data/power_flow/vision-validation-network/sym_output.json`

 * *Files identical despite different names*

### Comparing `power-grid-model-1.5.0rc9190015282548/tests/data/power_flow/vision-validation-network/vision_validation_network.vnf` & `power-grid-model-1.5.0rc9190704883749/tests/data/power_flow/vision-validation-network/vision_validation_network.vnf`

 * *Files identical despite different names*

### Comparing `power-grid-model-1.5.0rc9190015282548/tests/data/short_circuit/single_phase_to_ground_a/asym_sc_output_batch.json` & `power-grid-model-1.5.0rc9190704883749/tests/data/short_circuit/single_phase_to_ground_a/asym_sc_output_batch.json`

 * *Files identical despite different names*

### Comparing `power-grid-model-1.5.0rc9190015282548/tests/data/short_circuit/single_phase_to_ground_a/input.json` & `power-grid-model-1.5.0rc9190704883749/tests/data/short_circuit/single_phase_to_ground_a/input.json`

 * *Files identical despite different names*

### Comparing `power-grid-model-1.5.0rc9190015282548/tests/data/short_circuit/single_phase_to_ground_a/update_batch.json` & `power-grid-model-1.5.0rc9190704883749/tests/data/short_circuit/single_phase_to_ground_a/update_batch.json`

 * *Files identical despite different names*

### Comparing `power-grid-model-1.5.0rc9190015282548/tests/data/short_circuit/single_phase_to_ground_b/asym_sc_output_batch.json` & `power-grid-model-1.5.0rc9190704883749/tests/data/short_circuit/single_phase_to_ground_b/asym_sc_output_batch.json`

 * *Files identical despite different names*

### Comparing `power-grid-model-1.5.0rc9190015282548/tests/data/short_circuit/single_phase_to_ground_b/input.json` & `power-grid-model-1.5.0rc9190704883749/tests/data/short_circuit/single_phase_to_ground_b/input.json`

 * *Files identical despite different names*

### Comparing `power-grid-model-1.5.0rc9190015282548/tests/data/short_circuit/single_phase_to_ground_b/update_batch.json` & `power-grid-model-1.5.0rc9190704883749/tests/data/short_circuit/single_phase_to_ground_b/update_batch.json`

 * *Files identical despite different names*

### Comparing `power-grid-model-1.5.0rc9190015282548/tests/data/short_circuit/single_phase_to_ground_c/asym_sc_output_batch.json` & `power-grid-model-1.5.0rc9190704883749/tests/data/short_circuit/single_phase_to_ground_c/asym_sc_output_batch.json`

 * *Files identical despite different names*

### Comparing `power-grid-model-1.5.0rc9190015282548/tests/data/short_circuit/single_phase_to_ground_c/input.json` & `power-grid-model-1.5.0rc9190704883749/tests/data/short_circuit/single_phase_to_ground_c/input.json`

 * *Files identical despite different names*

### Comparing `power-grid-model-1.5.0rc9190015282548/tests/data/short_circuit/single_phase_to_ground_c/update_batch.json` & `power-grid-model-1.5.0rc9190704883749/tests/data/short_circuit/single_phase_to_ground_c/update_batch.json`

 * *Files identical despite different names*

### Comparing `power-grid-model-1.5.0rc9190015282548/tests/data/short_circuit/three_phase/input.json` & `power-grid-model-1.5.0rc9190704883749/tests/data/short_circuit/three_phase/input.json`

 * *Files identical despite different names*

### Comparing `power-grid-model-1.5.0rc9190015282548/tests/data/short_circuit/three_phase/sym_sc_output_batch.json` & `power-grid-model-1.5.0rc9190704883749/tests/data/short_circuit/three_phase/sym_sc_output_batch.json`

 * *Files identical despite different names*

### Comparing `power-grid-model-1.5.0rc9190015282548/tests/data/short_circuit/three_phase/update_batch.json` & `power-grid-model-1.5.0rc9190704883749/tests/data/short_circuit/three_phase/update_batch.json`

 * *Files identical despite different names*

### Comparing `power-grid-model-1.5.0rc9190015282548/tests/data/short_circuit/two_phase_ab/asym_sc_output_batch.json` & `power-grid-model-1.5.0rc9190704883749/tests/data/short_circuit/two_phase_ab/asym_sc_output_batch.json`

 * *Files identical despite different names*

### Comparing `power-grid-model-1.5.0rc9190015282548/tests/data/short_circuit/two_phase_ab/input.json` & `power-grid-model-1.5.0rc9190704883749/tests/data/short_circuit/two_phase_ab/input.json`

 * *Files identical despite different names*

### Comparing `power-grid-model-1.5.0rc9190015282548/tests/data/short_circuit/two_phase_ab/update_batch.json` & `power-grid-model-1.5.0rc9190704883749/tests/data/short_circuit/two_phase_ab/update_batch.json`

 * *Files identical despite different names*

### Comparing `power-grid-model-1.5.0rc9190015282548/tests/data/short_circuit/two_phase_ac/asym_sc_output_batch.json` & `power-grid-model-1.5.0rc9190704883749/tests/data/short_circuit/two_phase_ac/asym_sc_output_batch.json`

 * *Files identical despite different names*

### Comparing `power-grid-model-1.5.0rc9190015282548/tests/data/short_circuit/two_phase_ac/input.json` & `power-grid-model-1.5.0rc9190704883749/tests/data/short_circuit/two_phase_ac/input.json`

 * *Files identical despite different names*

### Comparing `power-grid-model-1.5.0rc9190015282548/tests/data/short_circuit/two_phase_ac/update_batch.json` & `power-grid-model-1.5.0rc9190704883749/tests/data/short_circuit/two_phase_ac/update_batch.json`

 * *Files identical despite different names*

### Comparing `power-grid-model-1.5.0rc9190015282548/tests/data/short_circuit/two_phase_bc/asym_sc_output_batch.json` & `power-grid-model-1.5.0rc9190704883749/tests/data/short_circuit/two_phase_bc/asym_sc_output_batch.json`

 * *Files identical despite different names*

### Comparing `power-grid-model-1.5.0rc9190015282548/tests/data/short_circuit/two_phase_bc/input.json` & `power-grid-model-1.5.0rc9190704883749/tests/data/short_circuit/two_phase_bc/input.json`

 * *Files identical despite different names*

### Comparing `power-grid-model-1.5.0rc9190015282548/tests/data/short_circuit/two_phase_bc/update_batch.json` & `power-grid-model-1.5.0rc9190704883749/tests/data/short_circuit/two_phase_bc/update_batch.json`

 * *Files identical despite different names*

### Comparing `power-grid-model-1.5.0rc9190015282548/tests/data/short_circuit/two_phase_to_ground_ab/asym_sc_output_batch.json` & `power-grid-model-1.5.0rc9190704883749/tests/data/short_circuit/two_phase_to_ground_ab/asym_sc_output_batch.json`

 * *Files identical despite different names*

### Comparing `power-grid-model-1.5.0rc9190015282548/tests/data/short_circuit/two_phase_to_ground_ab/input.json` & `power-grid-model-1.5.0rc9190704883749/tests/data/short_circuit/two_phase_to_ground_ab/input.json`

 * *Files identical despite different names*

### Comparing `power-grid-model-1.5.0rc9190015282548/tests/data/short_circuit/two_phase_to_ground_ab/update_batch.json` & `power-grid-model-1.5.0rc9190704883749/tests/data/short_circuit/two_phase_to_ground_ab/update_batch.json`

 * *Files identical despite different names*

### Comparing `power-grid-model-1.5.0rc9190015282548/tests/data/short_circuit/two_phase_to_ground_ac/asym_sc_output_batch.json` & `power-grid-model-1.5.0rc9190704883749/tests/data/short_circuit/two_phase_to_ground_ac/asym_sc_output_batch.json`

 * *Files identical despite different names*

### Comparing `power-grid-model-1.5.0rc9190015282548/tests/data/short_circuit/two_phase_to_ground_ac/input.json` & `power-grid-model-1.5.0rc9190704883749/tests/data/short_circuit/two_phase_to_ground_ac/input.json`

 * *Files identical despite different names*

### Comparing `power-grid-model-1.5.0rc9190015282548/tests/data/short_circuit/two_phase_to_ground_ac/update_batch.json` & `power-grid-model-1.5.0rc9190704883749/tests/data/short_circuit/two_phase_to_ground_ac/update_batch.json`

 * *Files identical despite different names*

### Comparing `power-grid-model-1.5.0rc9190015282548/tests/data/short_circuit/two_phase_to_ground_bc/asym_sc_output_batch.json` & `power-grid-model-1.5.0rc9190704883749/tests/data/short_circuit/two_phase_to_ground_bc/asym_sc_output_batch.json`

 * *Files identical despite different names*

### Comparing `power-grid-model-1.5.0rc9190015282548/tests/data/short_circuit/two_phase_to_ground_bc/input.json` & `power-grid-model-1.5.0rc9190704883749/tests/data/short_circuit/two_phase_to_ground_bc/input.json`

 * *Files identical despite different names*

### Comparing `power-grid-model-1.5.0rc9190015282548/tests/data/short_circuit/two_phase_to_ground_bc/update_batch.json` & `power-grid-model-1.5.0rc9190704883749/tests/data/short_circuit/two_phase_to_ground_bc/update_batch.json`

 * *Files identical despite different names*

### Comparing `power-grid-model-1.5.0rc9190015282548/tests/data/state_estimation/1os2msr/input.json` & `power-grid-model-1.5.0rc9190704883749/tests/data/state_estimation/1os2msr/input.json`

 * *Files identical despite different names*

### Comparing `power-grid-model-1.5.0rc9190015282548/tests/data/state_estimation/1os2msr/sym_output.json` & `power-grid-model-1.5.0rc9190704883749/tests/data/state_estimation/1os2msr/sym_output.json`

 * *Files identical despite different names*

### Comparing `power-grid-model-1.5.0rc9190015282548/tests/data/state_estimation/1os2msr-no-angle/input.json` & `power-grid-model-1.5.0rc9190704883749/tests/data/state_estimation/1os2msr-no-angle/input.json`

 * *Files identical despite different names*

### Comparing `power-grid-model-1.5.0rc9190015282548/tests/data/state_estimation/1os2msr-no-angle/sym_output.json` & `power-grid-model-1.5.0rc9190704883749/tests/data/state_estimation/1os2msr-no-angle/sym_output.json`

 * *Files identical despite different names*

### Comparing `power-grid-model-1.5.0rc9190015282548/tests/data/state_estimation/distribution-case/README.md` & `power-grid-model-1.5.0rc9190704883749/tests/data/state_estimation/distribution-case/README.md`

 * *Files identical despite different names*

### Comparing `power-grid-model-1.5.0rc9190015282548/tests/data/state_estimation/distribution-case/input.json` & `power-grid-model-1.5.0rc9190704883749/tests/data/state_estimation/distribution-case/input.json`

 * *Files identical despite different names*

### Comparing `power-grid-model-1.5.0rc9190015282548/tests/data/state_estimation/distribution-case/sym_output_batch.json` & `power-grid-model-1.5.0rc9190704883749/tests/data/state_estimation/distribution-case/sym_output_batch.json`

 * *Files identical despite different names*

### Comparing `power-grid-model-1.5.0rc9190015282548/tests/data/state_estimation/distribution-case/update_batch.json` & `power-grid-model-1.5.0rc9190704883749/tests/data/state_estimation/distribution-case/update_batch.json`

 * *Files identical despite different names*

### Comparing `power-grid-model-1.5.0rc9190015282548/tests/data/state_estimation/dummy-test-sym/input.json` & `power-grid-model-1.5.0rc9190704883749/tests/data/state_estimation/dummy-test-sym/input.json`

 * *Files identical despite different names*

### Comparing `power-grid-model-1.5.0rc9190015282548/tests/data/state_estimation/dummy-test-sym/sym_output.json` & `power-grid-model-1.5.0rc9190704883749/tests/data/state_estimation/dummy-test-sym/sym_output.json`

 * *Files identical despite different names*

### Comparing `power-grid-model-1.5.0rc9190015282548/tests/data/state_estimation/node-injection-sensor-and-zero-injection/input.json` & `power-grid-model-1.5.0rc9190704883749/tests/data/state_estimation/node-injection-sensor-and-zero-injection/input.json`

 * *Files identical despite different names*

### Comparing `power-grid-model-1.5.0rc9190015282548/tests/data/state_estimation/node-injection-sensor-and-zero-injection/sym_output.json` & `power-grid-model-1.5.0rc9190704883749/tests/data/state_estimation/node-injection-sensor-and-zero-injection/sym_output.json`

 * *Files identical despite different names*

### Comparing `power-grid-model-1.5.0rc9190015282548/tests/data/state_estimation/single-line-load/input.json` & `power-grid-model-1.5.0rc9190704883749/tests/data/state_estimation/single-line-load/input.json`

 * *Files identical despite different names*

### Comparing `power-grid-model-1.5.0rc9190015282548/tests/data/state_estimation/single-line-load/sym_output.json` & `power-grid-model-1.5.0rc9190704883749/tests/data/state_estimation/single-line-load/sym_output.json`

 * *Files identical despite different names*

### Comparing `power-grid-model-1.5.0rc9190015282548/tests/data/state_estimation/three_winding_transformer/input.json` & `power-grid-model-1.5.0rc9190704883749/tests/data/state_estimation/three_winding_transformer/input.json`

 * *Files identical despite different names*

### Comparing `power-grid-model-1.5.0rc9190015282548/tests/data/state_estimation/three_winding_transformer/sym_output.json` & `power-grid-model-1.5.0rc9190704883749/tests/data/state_estimation/three_winding_transformer/sym_output.json`

 * *Files identical despite different names*

### Comparing `power-grid-model-1.5.0rc9190015282548/tests/data/state_estimation/transmission-case/README.md` & `power-grid-model-1.5.0rc9190704883749/tests/data/state_estimation/transmission-case/README.md`

 * *Files identical despite different names*

### Comparing `power-grid-model-1.5.0rc9190015282548/tests/data/state_estimation/transmission-case/asym_output.json` & `power-grid-model-1.5.0rc9190704883749/tests/data/state_estimation/transmission-case/asym_output.json`

 * *Files identical despite different names*

### Comparing `power-grid-model-1.5.0rc9190015282548/tests/data/state_estimation/transmission-case/input.json` & `power-grid-model-1.5.0rc9190704883749/tests/data/state_estimation/transmission-case/input.json`

 * *Files identical despite different names*

### Comparing `power-grid-model-1.5.0rc9190015282548/tests/data/state_estimation/transmission-case/sym_output.json` & `power-grid-model-1.5.0rc9190704883749/tests/data/state_estimation/transmission-case/sym_output.json`

 * *Files identical despite different names*

### Comparing `power-grid-model-1.5.0rc9190015282548/tests/unit/test_0Z_model_validation.py` & `power-grid-model-1.5.0rc9190704883749/tests/unit/test_0Z_model_validation.py`

 * *Files identical despite different names*

### Comparing `power-grid-model-1.5.0rc9190015282548/tests/unit/test_error_handling.py` & `power-grid-model-1.5.0rc9190704883749/tests/unit/test_error_handling.py`

 * *Files identical despite different names*

### Comparing `power-grid-model-1.5.0rc9190015282548/tests/unit/test_meta_data.py` & `power-grid-model-1.5.0rc9190704883749/tests/unit/test_meta_data.py`

 * *Files identical despite different names*

### Comparing `power-grid-model-1.5.0rc9190015282548/tests/unit/test_power_grid_model.py` & `power-grid-model-1.5.0rc9190704883749/tests/unit/test_power_grid_model.py`

 * *Files identical despite different names*

### Comparing `power-grid-model-1.5.0rc9190015282548/tests/unit/test_utils.py` & `power-grid-model-1.5.0rc9190704883749/tests/unit/test_utils.py`

 * *Files identical despite different names*

### Comparing `power-grid-model-1.5.0rc9190015282548/tests/unit/utils.py` & `power-grid-model-1.5.0rc9190704883749/tests/unit/utils.py`

 * *Files identical despite different names*

### Comparing `power-grid-model-1.5.0rc9190015282548/tests/unit/validation/test_assertions.py` & `power-grid-model-1.5.0rc9190704883749/tests/unit/validation/test_assertions.py`

 * *Files identical despite different names*

### Comparing `power-grid-model-1.5.0rc9190015282548/tests/unit/validation/test_batch_validation.py` & `power-grid-model-1.5.0rc9190704883749/tests/unit/validation/test_batch_validation.py`

 * *Files identical despite different names*

### Comparing `power-grid-model-1.5.0rc9190015282548/tests/unit/validation/test_errors.py` & `power-grid-model-1.5.0rc9190704883749/tests/unit/validation/test_errors.py`

 * *Files identical despite different names*

### Comparing `power-grid-model-1.5.0rc9190015282548/tests/unit/validation/test_input_validation.py` & `power-grid-model-1.5.0rc9190704883749/tests/unit/validation/test_input_validation.py`

 * *Files identical despite different names*

### Comparing `power-grid-model-1.5.0rc9190015282548/tests/unit/validation/test_rules.py` & `power-grid-model-1.5.0rc9190704883749/tests/unit/validation/test_rules.py`

 * *Files identical despite different names*

### Comparing `power-grid-model-1.5.0rc9190015282548/tests/unit/validation/test_utils.py` & `power-grid-model-1.5.0rc9190704883749/tests/unit/validation/test_utils.py`

 * *Files identical despite different names*

### Comparing `power-grid-model-1.5.0rc9190015282548/tests/unit/validation/test_validation_functions.py` & `power-grid-model-1.5.0rc9190704883749/tests/unit/validation/test_validation_functions.py`

 * *Files identical despite different names*

